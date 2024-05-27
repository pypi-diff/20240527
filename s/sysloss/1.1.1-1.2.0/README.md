# Comparing `tmp/sysloss-1.1.1.tar.gz` & `tmp/sysloss-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysloss-1.1.1.tar", max compression
+gzip compressed data, was "sysloss-1.2.0.tar", max compression
```

## Comparing `sysloss-1.1.1.tar` & `sysloss-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2024-05-22 15:06:08.168418 sysloss-1.1.1/LICENSE
--rw-r--r--   0        0        0     2673 2024-05-22 15:06:08.168418 sysloss-1.1.1/README.md
--rw-r--r--   0        0        0     1613 2024-05-22 15:06:17.660491 sysloss-1.1.1/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-22 15:06:17.660491 sysloss-1.1.1/src/sysloss/__init__.py
--rw-r--r--   0        0        0    29244 2024-05-22 15:06:08.176418 sysloss-1.1.1/src/sysloss/components.py
--rw-r--r--   0        0        0    51545 2024-05-22 15:06:08.176418 sysloss-1.1.1/src/sysloss/system.py
--rw-r--r--   0        0        0     3615 1970-01-01 00:00:00.000000 sysloss-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-27 17:43:18.727499 sysloss-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2673 2024-05-27 17:43:18.727499 sysloss-1.2.0/README.md
+-rw-r--r--   0        0        0     1613 2024-05-27 17:43:28.059499 sysloss-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-27 17:43:28.059499 sysloss-1.2.0/src/sysloss/__init__.py
+-rw-r--r--   0        0        0    35541 2024-05-27 17:43:18.735499 sysloss-1.2.0/src/sysloss/components.py
+-rw-r--r--   0        0        0    50312 2024-05-27 17:43:18.735499 sysloss-1.2.0/src/sysloss/system.py
+-rw-r--r--   0        0        0     3615 1970-01-01 00:00:00.000000 sysloss-1.2.0/PKG-INFO
```

### Comparing `sysloss-1.1.1/LICENSE` & `sysloss-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sysloss-1.1.1/README.md` & `sysloss-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sysloss-1.1.1/pyproject.toml` & `sysloss-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sysloss"
-version = "1.1.1"
+version = "1.2.0"
 description = "Power analysis of circuits and systems."
 authors = ["Geir Drange"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/geddy11/sysloss"
 repository = "https://github.com/geddy11/sysloss"
 documentation = "https://sysloss.readthedocs.io/en/latest/Getting%20started.html#"
```

### Comparing `sysloss-1.1.1/src/sysloss/components.py` & `sysloss-1.2.0/src/sysloss/components.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,14 +48,17 @@
 VDROP_DEFAULT = 0.0
 PWRS_DEFAULT = 0.0
 LIMITS_DEFAULT = {
     "vi": [0.0, MAX_DEFAULT],
     "vo": [0.0, MAX_DEFAULT],
     "ii": [0.0, MAX_DEFAULT],
     "io": [0.0, MAX_DEFAULT],
+    "pi": [0.0, MAX_DEFAULT],
+    "po": [0.0, MAX_DEFAULT],
+    "pl": [0.0, MAX_DEFAULT],
 }
 
 
 def _get_opt(params, key, default):
     """Get optional parameter from dict"""
     if key in params:
         return params[key]
@@ -177,15 +180,15 @@
     name : str
         Source name.
     vo : float
         Output voltage.
     rs : float, optional
         Source resistance., by default 0.0
     limits : dict, optional
-        Voltage and current limits., by default LIMITS_DEFAULT
+        Voltage, current and power limits., by default LIMITS_DEFAULT. The following limits apply: io, po, pl.
     """
 
     @property
     def _component_type(self):
         """Defines the Source component type"""
         return _ComponentTypes.SOURCE
 
@@ -215,15 +218,15 @@
     def from_file(cls, name: str, *, fname: str):
         """Read source parameters from .toml file.
 
         Parameters
         ----------
         name : str
             Source name
-        fname : str, optional
+        fname : str
             File name.
         """
         with open(fname, "r") as f:
             config = toml.load(f)
 
         v = _get_mand(config["source"], "vo")
         r = _get_opt(config["source"], "rs", RS_DEFAULT)
@@ -255,28 +258,37 @@
         ipwr = abs(self._params["vo"] * io)
         loss = self._params["rs"] * io * io
         opwr = ipwr - loss
         return ipwr, loss, _get_eff(ipwr, opwr)
 
     def _solv_get_warns(self, vi, vo, ii, io, phase, phase_conf={}):
         """Check limits"""
-        return _get_warns(self._limits, {"ii": ii, "io": io})
+        return _get_warns(
+            self._limits, {"io": io, "po": vo * io, "pl": self._params["rs"] * io * io}
+        )
+
+    def _get_params(self, pdict):
+        """Return dict with component parameters"""
+        ret = pdict
+        ret["vo"] = self._params["vo"]
+        ret["rs"] = self._params["rs"]
+        return ret
 
 
 class PLoad:
     """Power load.
 
     Parameters
     ----------
     name : str
         Load name.
     pwr : float
         Load power (W).
     limits : dict, optional
-         Voltage and current limits., by default LIMITS_DEFAULT
+         Voltage, current and power limits., by default LIMITS_DEFAULT. The following limits apply: vi, ii
     pwrs : float, optional
         Load sleep power (W), by default PWRS_DEFAULT
     """
 
     @property
     def _component_type(self):
         """Defines the Load component type"""
@@ -306,15 +318,15 @@
     def from_file(cls, name: str, *, fname: str):
         """Read PLoad parameters from .toml file.
 
         Parameters
         ----------
         name : str
             Load name
-        fname : str, optional
+        fname : str
             File name.
         """
         with open(fname, "r") as f:
             config = toml.load(f)
 
         p = _get_mand(config["pload"], "pwr")
         lim = _get_opt(config, "limits", LIMITS_DEFAULT)
@@ -353,26 +365,33 @@
     def _solv_get_warns(self, vi, vo, ii, io, phase, phase_conf={}):
         """Check limits"""
         if phase_conf and phase != "":
             if phase not in phase_conf:
                 return ""
         return _get_warns(self._limits, {"vi": vi, "ii": ii})
 
+    def _get_params(self, pdict):
+        """Return dict with component parameters"""
+        ret = pdict
+        ret["pwr"] = self._params["pwr"]
+        ret["pwrs"] = self._params["pwrs"]
+        return ret
+
 
 class ILoad(PLoad):
     """Current load.
 
     Parameters
     ----------
     name : str
         Load name.
     ii : float
         Load current (A).
     limits : dict, optional
-         Voltage and current limits., by default LIMITS_DEFAULT
+         Voltage, current and power limits., by default LIMITS_DEFAULT. The following limits apply: vi, pi
     iis : float, optional
         Load sleep current (A), by default PWRS_DEFAULT
     """
 
     def __init__(
         self,
         name: str,
@@ -392,15 +411,15 @@
     def from_file(cls, name: str, *, fname: str):
         """Read ILoad parameters from .toml file.
 
         Parameters
         ----------
         name : str
             Load name
-        fname : str, optional
+        fname : str
             File name.
         """
         with open(fname, "r") as f:
             config = toml.load(f)
 
         i = _get_mand(config["iload"], "ii")
         lim = _get_opt(config, "limits", LIMITS_DEFAULT)
@@ -418,26 +437,40 @@
         elif phase not in phase_conf:
             i = self._params["iis"]
         else:
             i = phase_conf[phase]
 
         return abs(i)
 
+    def _solv_get_warns(self, vi, vo, ii, io, phase, phase_conf={}):
+        """Check limits"""
+        if phase_conf and phase != "":
+            if phase not in phase_conf:
+                return ""
+        return _get_warns(self._limits, {"vi": vi, "pi": vi * ii})
+
+    def _get_params(self, pdict):
+        """Return dict with component parameters"""
+        ret = pdict
+        ret["ii"] = self._params["ii"]
+        ret["iis"] = self._params["iis"]
+        return ret
+
 
 class RLoad(PLoad):
     """Resistive load.
 
     Parameters
     ----------
     name : str
         Load name.
     rs : float
         Load resistance (ohm).
     limits : dict, optional
-         Voltage and current limits., by default LIMITS_DEFAULT
+         Voltage, current and power limits., by default LIMITS_DEFAULT. The following limits apply: vi, ii, pi
     """
 
     def __init__(
         self,
         name: str,
         *,
         rs: float,
@@ -455,15 +488,15 @@
     def from_file(cls, name: str, *, fname: str):
         """Read RLoad parameters from .toml file.
 
         Parameters
         ----------
         name : str
             Load name
-        fname : str, optional
+        fname : str
             File name.
         """
         with open(fname, "r") as f:
             config = toml.load(f)
 
         r = _get_mand(config["rload"], "rs")
         lim = _get_opt(config, "limits", LIMITS_DEFAULT)
@@ -475,28 +508,41 @@
             pass
         elif phase not in phase_conf:
             pass
         else:
             r = phase_conf[phase]
         return abs(vi) / r
 
+    def _solv_get_warns(self, vi, vo, ii, io, phase, phase_conf={}):
+        """Check limits"""
+        if phase_conf and phase != "":
+            if phase not in phase_conf:
+                return ""
+        return _get_warns(self._limits, {"vi": vi, "ii": ii, "pi": vi * ii})
+
+    def _get_params(self, pdict):
+        """Return dict with component parameters"""
+        ret = pdict
+        ret["rs"] = self._params["rs"]
+        return ret
+
 
 class RLoss:
     """Resistive loss.
 
     This loss element is connected in series with other elements.
 
     Parameters
     ----------
     name : str
         Loss name.
     rs : float
         Loss resistance (ohm).
     limits : dict, optional
-         Voltage and current limits., by default LIMITS_DEFAULT
+         Voltage, current and power limits., by default LIMITS_DEFAULT. The following limits apply: vi, vo, ii, io, pi, po, pl
     """
 
     @property
     def _component_type(self):
         """Defines the Loss component type"""
         return _ComponentTypes.SLOSS
 
@@ -524,15 +570,15 @@
     def from_file(cls, name: str, *, fname: str):
         """Read RLoss parameters from .toml file.
 
         Parameters
         ----------
         name : str
             Loss name
-        fname : str, optional
+        fname : str
             File name.
         """
         with open(fname, "r") as f:
             config = toml.load(f)
 
         r = _get_mand(config["rloss"], "rs")
         lim = _get_opt(config, "limits", LIMITS_DEFAULT)
@@ -570,30 +616,47 @@
             return 0.0, 0.0, 0.0
         loss = abs(vi - vout) * io
         pwr = abs(vi * ii)
         return pwr, loss, _get_eff(pwr, pwr - loss, 100.0)
 
     def _solv_get_warns(self, vi, vo, ii, io, phase, phase_conf={}):
         """Check limits"""
-        return _get_warns(self._limits, {"vi": vi, "vo": vo, "ii": ii, "io": io})
+        return _get_warns(
+            self._limits,
+            {
+                "vi": vi,
+                "vo": vo,
+                "ii": ii,
+                "io": io,
+                "pi": vi * ii,
+                "po": vo * io,
+                "pl": vi * ii - vo * io,
+            },
+        )
+
+    def _get_params(self, pdict):
+        """Return dict with component parameters"""
+        ret = pdict
+        ret["rs"] = self._params["rs"]
+        return ret
 
 
 class VLoss:
     """Voltage loss.
 
     This loss element is connected in series with other elements.
 
     Parameters
     ----------
     name : str
         Loss name.
     vdrop : float | dict
         Voltage drop (V), a constant value (float) or interpolation data (dict).
     limits : dict, optional
-         Voltage and current limits., by default LIMITS_DEFAULT
+         Voltage, current and power limits., by default LIMITS_DEFAULT. The following limits apply: vi, vo, ii, io, pi, po, pl
     """
 
     @property
     def _component_type(self):
         """Defines the Loss component type"""
         return _ComponentTypes.SLOSS
 
@@ -636,15 +699,15 @@
     def from_file(cls, name: str, *, fname: str):
         """Read VLoss parameters from .toml file.
 
         Parameters
         ----------
         name : str
             Loss name
-        fname : str, optional
+        fname : str
             File name.
         """
         with open(fname, "r") as f:
             config = toml.load(f)
 
         vd = _get_mand(config["vloss"], "vdrop")
         lim = _get_opt(config, "limits", LIMITS_DEFAULT)
@@ -682,15 +745,49 @@
             return 0.0, 0.0, 0.0
         loss = abs(vi - vout) * io
         pwr = abs(vi * ii)
         return pwr, loss, _get_eff(pwr, pwr - loss, 100.0)
 
     def _solv_get_warns(self, vi, vo, ii, io, phase, phase_conf={}):
         """Check limits"""
-        return _get_warns(self._limits, {"vi": vi, "vo": vo, "ii": ii, "io": io})
+        return _get_warns(
+            self._limits,
+            {
+                "vi": vi,
+                "vo": vo,
+                "ii": ii,
+                "io": io,
+                "pi": vi * ii,
+                "po": vo * io,
+                "pl": vi * ii - vo * io,
+            },
+        )
+
+    def _get_annot(self):
+        """Get interpolation figure annotations in format [xlabel, ylabel, title]"""
+        if isinstance(self._ipr, _Interp1d):
+            return [
+                "Output current (A)",
+                "Voltage drop (V)",
+                "{} voltage drop".format(self._params["name"]),
+            ]
+        return [
+            "Output current (A)",
+            "Input voltage (V)",
+            "{} voltage drop".format(self._params["name"]),
+        ]
+
+    def _get_params(self, pdict):
+        """Return dict with component parameters"""
+        ret = pdict
+        if isinstance(self._ipr, _Interp0d):
+            ret["vdrop"] = abs(self._params["vdrop"])
+        else:
+            ret["vdrop"] = "interp"
+        return ret
 
 
 class Converter:
     """Voltage converter.
 
     Parameters
     ----------
@@ -699,15 +796,15 @@
     vo : float
         Output voltage (V).
     eff : float | dict
         Converter efficiency, a constant value (float) or interpolation data (dict).
     iq : float, optional
         Quiescent (no-load) current (A)., by default 0.0
     limits : dict, optional
-        Voltage and current limits., by default LIMITS_DEFAULT
+        Voltage, current and power limits., by default LIMITS_DEFAULT. The following limits apply: vi, vo, ii, io, pi, po, pl
     iis : float, optional
         Sleep (shut-down) current (A), by default 0.0
 
     Raises
     ------
     ValueError
         If efficiency is 0.0 or > 1.0.
@@ -770,15 +867,15 @@
     def from_file(cls, name: str, *, fname: str):
         """Read Converter parameters from .toml file.
 
         Parameters
         ----------
         name : str
             Converter name
-        fname : str, optional
+        fname : str
             File name.
         """
         with open(fname, "r") as f:
             config = toml.load(f)
 
         v = _get_mand(config["converter"], "vo")
         e = _get_mand(config["converter"], "eff")
@@ -840,34 +937,73 @@
         return pwr, loss, _get_eff(pwr, pwr - loss, 0.0)
 
     def _solv_get_warns(self, vi, vo, ii, io, phase, phase_conf=[]):
         """Check limits"""
         if phase_conf:
             if phase not in phase_conf:
                 return ""
-        return _get_warns(self._limits, {"vi": vi, "vo": vo, "ii": ii, "io": io})
+        pi, pl, _ = self._solv_pwr_loss(vi, vo, ii, io, phase, phase_conf=[])
+        return _get_warns(
+            self._limits,
+            {"vi": vi, "vo": vo, "ii": ii, "io": io, "pi": pi, "po": pi - pl, "pl": pl},
+        )
+
+    def _get_annot(self):
+        """Get interpolation figure annotations in format [xlabel, ylabel, title]"""
+        if isinstance(self._ipr, _Interp1d):
+            return [
+                "Output current (A)",
+                "Efficiency",
+                "{} efficiency for Vo={}V".format(
+                    self._params["name"], self._params["vo"]
+                ),
+            ]
+        return [
+            "Output current (A)",
+            "Input voltage (V)",
+            "{} efficiency for Vo={}V".format(self._params["name"], self._params["vo"]),
+        ]
+
+    def _get_params(self, pdict):
+        """Return dict with component parameters"""
+        ret = pdict
+        ret["vo"] = self._params["vo"]
+        ret["iq"] = self._params["iq"]
+        if isinstance(self._ipr, _Interp0d):
+            ret["eff"] = abs(self._params["eff"])
+        else:
+            ret["eff"] = "interp"
+        ret["iis"] = self._params["iis"]
+        return ret
 
 
 class LinReg:
     """Linear voltage converter.
 
+    If vi - vo < vdrop, the output voltage is reduced to vi - vdrop during analysis.
+
     Parameters
     ----------
     name : str
         Converter name.
     vo : float
         Output voltage (V).
     vdrop : float
         Dropout voltage (V).
-    iq : float, optional
-        Quiescent (no-load) current (A)., by default 0.0
+    iq : float | dict, optional
+        Ground current (A)., by default 0.0
     limits : dict, optional
-        Voltage and current limits., by default LIMITS_DEFAULT
+        Voltage, current and power limits., by default LIMITS_DEFAULT. The following limits apply: vi, vo, ii, io, pi, po, pl
     iis : float, optional
         Sleep (shut-down) current (A), by default 0.0
+
+    Raises
+    ------
+    ValueError
+        If vdrop > vo.
     """
 
     @property
     def _component_type(self):
         """Defines the LinReg component type"""
         return _ComponentTypes.LINREG
 
@@ -890,42 +1026,58 @@
     ):
         self._params = {}
         self._params["name"] = name
         self._params["vo"] = vo
         if not (abs(vdrop) < abs(vo)):
             raise ValueError("Voltage drop must be < vo")
         self._params["vdrop"] = abs(vdrop)
-        self._params["iq"] = abs(iq)
+        if isinstance(iq, dict):
+            if not np.all(np.diff(iq["io"]) > 0):
+                raise ValueError("iq values must be monotonic increasing")
+            if np.min(iq["iq"]) < 0.0:
+                raise ValueError("iq values must be >= 0.0")
+            if len(iq["vi"]) == 1:
+                self._ipr = _Interp1d(iq["io"], iq["iq"][0])
+            else:
+                cur = []
+                volt = []
+                for v in iq["vi"]:
+                    cur += iq["io"]
+                    volt += len(iq["io"]) * [v]
+                    iqi = np.asarray(iq["iq"]).reshape(1, -1)[0].tolist()
+                self._ipr = _Interp2d(cur, volt, iqi)
+        else:
+            self._ipr = _Interp0d(abs(iq))
+        self._params["iq"] = iq
         self._params["iis"] = abs(iis)
         self._limits = limits
-        self._ipr = None
 
     @classmethod
     def from_file(cls, name: str, *, fname: str):
         """Read LinReg parameters from .toml file.
 
         Parameters
         ----------
         name : str
             LinReg name
-        fname : str, optional
+        fname : str
             File name.
         """
         with open(fname, "r") as f:
             config = toml.load(f)
 
         v = _get_mand(config["linreg"], "vo")
         vd = _get_opt(config["linreg"], "vdrop", VDROP_DEFAULT)
         iq = _get_opt(config["linreg"], "iq", IQ_DEFAULT)
         lim = _get_opt(config, "limits", LIMITS_DEFAULT)
         iis = _get_opt(config["linreg"], "iis", IIS_DEFAULT)
         return cls(name, vo=v, vdrop=vd, iq=iq, limits=lim, iis=iis)
 
     def _get_inp_current(self, phase, phase_conf=[]):
-        i = self._params["iq"]
+        i = self._ipr._interp(0.0, 0.0)
         if not phase_conf:
             pass
         elif phase not in phase_conf:
             i = self._params["iis"]
         return i
 
     def _get_outp_voltage(self, phase, phase_conf=[]):
@@ -936,18 +1088,15 @@
             v = 0.0
         return v
 
     def _solv_inp_curr(self, vi, vo, io, phase, phase_conf=[]):
         """Calculate component input current from vi, vo and io"""
         if abs(vi) == 0.0:
             return 0.0
-        if io == 0.0:
-            i = self._params["iq"]
-        else:
-            i = io
+        i = io + self._ipr._interp(abs(io), abs(vi))
         if not phase_conf:
             pass
         elif phase not in phase_conf:
             i = self._params["iis"]
         return i
 
     def _solv_outp_volt(self, vi, ii, io, phase, phase_conf=[]):
@@ -962,25 +1111,59 @@
         return -v
 
     def _solv_pwr_loss(self, vi, vo, ii, io, phase, phase_conf=[]):
         """Calculate power and loss in component"""
         v = min(abs(self._params["vo"]), max(abs(vi) - self._params["vdrop"], 0.0))
         if vi == 0.0 or v == 0.0:
             loss = 0.0
-        elif io > 0.0:
-            loss = (abs(vi) - abs(v)) * io
         else:
-            loss = abs(vi) * self._params["iq"]
+            loss = self._ipr._interp(abs(io), abs(vi)) * abs(vi)
+        if abs(io) > 0.0:
+            loss += (abs(vi) - abs(v)) * io
         pwr = abs(vi * ii)
         if not phase_conf:
             pass
         elif phase not in phase_conf:
             loss = abs(self._params["iis"] * vi)
             pwr = abs(self._params["iis"] * vi)
         return pwr, loss, _get_eff(pwr, pwr - loss, 0.0)
 
     def _solv_get_warns(self, vi, vo, ii, io, phase, phase_conf=[]):
         """Check limits"""
         if phase_conf:
             if phase not in phase_conf:
                 return ""
-        return _get_warns(self._limits, {"vi": vi, "vo": vo, "ii": ii, "io": io})
+        pi, pl, _ = self._solv_pwr_loss(vi, vo, ii, io, phase, phase_conf=[])
+        return _get_warns(
+            self._limits,
+            {"vi": vi, "vo": vo, "ii": ii, "io": io, "pi": pi, "po": pi - pl, "pl": pl},
+        )
+
+    def _get_annot(self):
+        """Get interpolation figure annotations in format [xlabel, ylabel, title]"""
+        if isinstance(self._ipr, _Interp1d):
+            return [
+                "Output current (A)",
+                "Ground current (A)",
+                "{} ground current for Vo={}V".format(
+                    self._params["name"], self._params["vo"]
+                ),
+            ]
+        return [
+            "Output current (A)",
+            "Input voltage (V)",
+            "{} ground current for Vo={}V".format(
+                self._params["name"], self._params["vo"]
+            ),
+        ]
+
+    def _get_params(self, pdict):
+        """Return dict with component parameters"""
+        ret = pdict
+        ret["vo"] = self._params["vo"]
+        ret["vdrop"] = self._params["vdrop"]
+        if isinstance(self._ipr, _Interp0d):
+            ret["iq"] = abs(self._params["iq"])
+        else:
+            ret["iq"] = "interp"
+        ret["iis"] = self._params["iis"]
+        return ret
```

### Comparing `sysloss-1.1.1/src/sysloss/system.py` & `sysloss-1.2.0/src/sysloss/system.py`

 * *Files 6% similar despite different names*

```diff
@@ -861,74 +861,55 @@
         -------
         pd.DataFrame
             System parameters.
         """
         self._rel_update()
         names, typ, parent, vo, vdrop = [], [], [], [], []
         iq, rs, eff, ii, pwr, iis = [], [], [], [], [], []
-        lii, lio, lvi, lvo, pwrs = [], [], [], [], []
+        lii, lio, lvi, lvo, lpi, lpo, lpl, pwrs = [], [], [], [], [], [], [], []
         domain, dname = [], "none"
         src_cnt = 0
+
         for n in self._topo_nodes:
             names += [self._g[n]._params["name"]]
             typ += [self._g[n]._component_type.name]
             if self._g[n]._component_type.name == "SOURCE":
                 dname = self._g[n]._params["name"]
                 src_cnt += 1
             domain += [dname]
-            _vo, _vdrop, _iq, _rs, _eff, _ii, _pwr = "", "", "", "", "", "", ""
-            _iis, _pwrs = "", ""
-            if self._g[n]._component_type == _ComponentTypes.SOURCE:
-                _vo = self._g[n]._params["vo"]
-                _rs = self._g[n]._params["rs"]
-            elif self._g[n]._component_type == _ComponentTypes.LOAD:
-                if "pwr" in self._g[n]._params:
-                    _pwr = self._g[n]._params["pwr"]
-                    _pwrs = self._g[n]._params["pwrs"]
-                elif "rs" in self._g[n]._params:
-                    _rs = self._g[n]._params["rs"]
-                else:
-                    _ii = self._g[n]._params["ii"]
-                    _iis = self._g[n]._params["iis"]
-            elif self._g[n]._component_type == _ComponentTypes.CONVERTER:
-                _vo = self._g[n]._params["vo"]
-                _iq = self._g[n]._params["iq"]
-                if isinstance(self._g[n]._ipr, _Interp0d):
-                    _eff = self._g[n]._params["eff"]
-                else:
-                    _eff = "interp"
-                _iis = self._g[n]._params["iis"]
-            elif self._g[n]._component_type == _ComponentTypes.LINREG:
-                _vo = self._g[n]._params["vo"]
-                _vdrop = self._g[n]._params["vdrop"]
-                _iq = self._g[n]._params["iq"]
-                _iis = self._g[n]._params["iis"]
-            elif self._g[n]._component_type == _ComponentTypes.SLOSS:
-                if "rs" in self._g[n]._params:
-                    _rs = self._g[n]._params["rs"]
-                else:
-                    if isinstance(self._g[n]._ipr, _Interp0d):
-                        _vdrop = self._g[n]._params["vdrop"]
-                    else:
-                        _vdrop = "interp"
-            vo += [_vo]
-            vdrop += [_vdrop]
-            iq += [_iq]
-            rs += [_rs]
-            eff += [_eff]
-            ii += [_ii]
-            pwr += [_pwr]
-            iis += [_iis]
-            pwrs += [_pwrs]
+            pdict = {
+                "vo": "",
+                "vdrop": "",
+                "iq": "",
+                "rs": "",
+                "eff": "",
+                "ii": "",
+                "pwr": "",
+                "iis": "",
+                "pwrs": "",
+            }
+            cparams = self._g[n]._get_params(pdict)
+            vo += [cparams["vo"]]
+            vdrop += [cparams["vdrop"]]
+            iq += [cparams["iq"]]
+            rs += [cparams["rs"]]
+            eff += [cparams["eff"]]
+            ii += [cparams["ii"]]
+            pwr += [cparams["pwr"]]
+            iis += [cparams["iis"]]
+            pwrs += [cparams["pwrs"]]
             parent += [self._get_parent_name(n)]
             if limits:
                 lii += [_get_opt(self._g[n]._limits, "ii", LIMITS_DEFAULT["ii"])]
                 lio += [_get_opt(self._g[n]._limits, "io", LIMITS_DEFAULT["io"])]
                 lvi += [_get_opt(self._g[n]._limits, "vi", LIMITS_DEFAULT["vi"])]
                 lvo += [_get_opt(self._g[n]._limits, "vo", LIMITS_DEFAULT["vo"])]
+                lpi += [_get_opt(self._g[n]._limits, "pi", LIMITS_DEFAULT["pi"])]
+                lpo += [_get_opt(self._g[n]._limits, "po", LIMITS_DEFAULT["po"])]
+                lpl += [_get_opt(self._g[n]._limits, "pl", LIMITS_DEFAULT["pl"])]
         # report
         res = {}
         res["Component"] = names
         res["Type"] = typ
         res["Parent"] = parent
         if src_cnt > 1:
             res["Domain"] = domain
@@ -938,18 +919,22 @@
         res["eff (%)"] = eff
         res["iq (A)"] = iq
         res["ii (A)"] = ii
         res["iis (A)"] = iis
         res["pwr (W)"] = pwr
         res["pwrs (W)"] = pwrs
         if limits:
-            res["vi limits (V)"] = lvi
-            res["vo limits (V)"] = lvo
-            res["ii limits (A)"] = lii
-            res["io limits (A)"] = lio
+            res["vi limit (V)"] = lvi
+            res["vo limit (V)"] = lvo
+            res["ii limit (A)"] = lii
+            res["io limit (A)"] = lio
+            res["pi limit (A)"] = lpi
+            res["po limit (A)"] = lpo
+            res["pl limit (A)"] = lpl
+
         return pd.DataFrame(res)
 
     def set_sys_phases(self, phases: dict):
         """Define system level load phases.
 
         Parameters
         ----------
@@ -1180,38 +1165,34 @@
         ValueError
             If component name is not found.
         """
         if not name in self._g.attrs["nodes"].keys():
             raise ValueError("Component name is not valid!")
         n = self._g.attrs["nodes"][name]
         if isinstance(self._g[n]._ipr, _Interp1d):
+            annot = self._g[n]._get_annot()
             fig = plt.figure()
             xmin = max(self._g[n]._ipr._x[0] - 0.15 * max(self._g[n]._ipr._x), 0.0)
             xmax = 1.15 * max(self._g[n]._ipr._x)
             x = np.linspace(xmin, xmax, num=200)
             fx = np.interp(x, self._g[n]._ipr._x, self._g[n]._ipr._fx)
             plt.plot(x, fx, "-")
             if inpdata:
                 plt.plot(
                     self._g[n]._ipr._x, self._g[n]._ipr._fx, ".r", label="input data"
                 )
                 plt.legend(loc="lower right")
-            plt.xlabel("Output current (A)")
-            if "vo" in self._g[n]._params:
-                plt.ylabel("Efficiency")
-                plt.title(
-                    "{} efficiency for Vo={}V".format(name, self._g[n]._params["vo"])
-                )
-            else:
-                plt.ylabel("Voltage drop (V)")
-                plt.title("{} voltage drop".format(name))
+            plt.xlabel(annot[0])
+            plt.ylabel(annot[1])
+            plt.title(annot[2])
             plt.rc("axes", axisbelow=True)
             plt.grid()
             return fig
         elif isinstance(self._g[n]._ipr, _Interp2d):
+            annot = self._g[n]._get_annot()
             xmin = max(min(self._g[n]._ipr._x) - 0.15 * max(self._g[n]._ipr._x), 0.0)
             xmax = 1.15 * max(self._g[n]._ipr._x)
             X = np.linspace(xmin, xmax, num=100)
             ymin = max(min(self._g[n]._ipr._y) - 0.15 * max(self._g[n]._ipr._y), 0.0)
             ymax = 1.15 * max(self._g[n]._ipr._y)
             Y = np.linspace(ymin, ymax, num=100)
             X, Y = np.meshgrid(X, Y)
@@ -1228,42 +1209,41 @@
                 plt.pcolormesh(X, Y, Z, shading="auto", cmap=cmap)
                 if inpdata:
                     plt.plot(
                         self._g[n]._ipr._x, self._g[n]._ipr._y, ".r", label="input data"
                     )
                     plt.legend(loc="upper left")
                 plt.colorbar()
-                plt.xlabel("Output current (A)")
-                plt.ylabel("Input voltage (V)")
+                plt.xlabel(annot[0])
+                plt.ylabel(annot[1])
             else:
                 fig, ax = plt.subplots(subplot_kw={"projection": "3d"})
                 surf = ax.plot_surface(
                     Y, X, Z, cmap=cmap, linewidth=0, antialiased=False
                 )
-                ax.set_zlim(np.nanmin(Z), 1.0)
+                if self._g[n]._component_type.name == "CONVERTER":
+                    ax.set_zlim(np.nanmin(Z), 1.0)
+                else:
+                    ax.set_zlim(np.nanmin(Z), np.nanmax(Z))
                 ax.zaxis.set_major_locator(LinearLocator(10))
                 ax.zaxis.set_major_formatter("{x:.02f}")
                 if inpdata:
                     plt.plot(
                         self._g[n]._ipr._y,
                         self._g[n]._ipr._x,
                         self._g[n]._ipr._fxy,
                         ".r",
                         label="input data",
                     )
                     plt.legend(loc="upper left")
                 fig.colorbar(surf, shrink=0.5, aspect=10, pad=0.1)
-                plt.ylabel("Output current (A)")
-                plt.xlabel("Input voltage (V)")
-            if "vo" in self._g[n]._params:
-                plt.title(
-                    "{} efficiency for Vo={}V".format(name, self._g[n]._params["vo"])
-                )
-            else:
-                plt.title("{} voltage drop".format(name))
+                # labels swapped
+                plt.xlabel(annot[1])
+                plt.ylabel(annot[0])
+            plt.title(annot[2])
             return fig
         else:
             print("Component does not have interpolation data")
             return None
 
     def batt_life(
         self,
```

### Comparing `sysloss-1.1.1/PKG-INFO` & `sysloss-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysloss
-Version: 1.1.1
+Version: 1.2.0
 Summary: Power analysis of circuits and systems.
 Home-page: https://github.com/geddy11/sysloss
 License: MIT
 Keywords: system,power,loss,efficiency,energy,component
 Author: Geir Drange
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sysloss Version: 1.1.1 Summary: Power analysis of
+Metadata-Version: 2.1 Name: sysloss Version: 1.2.0 Summary: Power analysis of
 circuits and systems. Home-page: https://github.com/geddy11/sysloss License:
 MIT Keywords: system,power,loss,efficiency,energy,component Author: Geir Drange
 Requires-Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: matplotlib
 (>=3.0,<4.0) Requires-Dist: pandas (>=2.0,<3.0) Requires-Dist: rich (>=12.0)
```

