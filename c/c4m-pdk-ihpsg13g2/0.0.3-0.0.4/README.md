# Comparing `tmp/c4m_pdk_ihpsg13g2-0.0.3.tar.gz` & `tmp/c4m_pdk_ihpsg13g2-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4m_pdk_ihpsg13g2-0.0.3.tar", last modified: Tue May 14 11:16:44 2024, max compression
+gzip compressed data, was "c4m_pdk_ihpsg13g2-0.0.4.tar", last modified: Mon May 27 12:47:09 2024, max compression
```

## Comparing `c4m_pdk_ihpsg13g2-0.0.3.tar` & `c4m_pdk_ihpsg13g2-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      992 2024-04-29 12:22:37.734462 c4m_pdk_ihpsg13g2-0.0.3/LICENSE.md
--rw-r--r--   0        0        0     5552 2024-05-13 16:42:35.930939 c4m_pdk_ihpsg13g2-0.0.3/README.md
--rw-r--r--   0        0        0      449 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/__init__.py
--rw-r--r--   0        0        0     4572 2024-04-29 11:09:33.917013 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/_io_compliance.py
--rw-r--r--   0        0        0     6918 2024-04-29 11:12:09.911800 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/io.py
--rw-r--r--   0        0        0      517 2024-04-29 11:12:20.003724 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/klayout.py
--rw-r--r--   0        0        0       23 2024-05-07 14:17:03.642346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/__init__.py
--rw-r--r--   0        0        0      775 2024-05-07 14:17:03.662346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/all.spice
--rw-r--r--   0        0        0    24555 2024-05-07 14:17:03.654346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/cornerMOShv.lib
--rw-r--r--   0        0        0    22926 2024-05-07 14:17:03.646346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/cornerMOSlv.lib
--rw-r--r--   0        0        0     2460 2024-05-07 14:17:03.658346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/cornerRES.lib
--rw-r--r--   0        0        0     3580 2024-05-07 14:17:03.658346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/diodes.lib
--rw-r--r--   0        0        0     1935 2024-05-07 14:17:03.654346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/resistors_mod.lib
--rw-r--r--   0        0        0     1039 2024-05-07 14:17:03.654346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/resistors_parm.lib
--rw-r--r--   0        0        0     1045 2024-05-07 14:17:03.658346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/resistors_stat.lib
--rw-r--r--   0        0        0     6144 2024-05-07 14:17:03.650346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_mod.lib
--rw-r--r--   0        0        0    40662 2024-05-07 14:17:03.650346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_parm.lib
--rw-r--r--   0        0        0     4027 2024-05-07 14:17:03.650346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_stat.lib
--rw-r--r--   0        0        0     6110 2024-05-07 14:17:03.642346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_mod.lib
--rw-r--r--   0        0        0    40995 2024-05-07 14:17:03.642346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_parm.lib
--rw-r--r--   0        0        0     3667 2024-05-07 14:17:03.646346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_stat.lib
--rw-r--r--   0        0        0    18379 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/pdkmaster.py
--rw-r--r--   0        0        0     2617 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/pyspice.py
--rw-r--r--   0        0        0     4300 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/stdcell.py
--rw-r--r--   0        0        0     1551 2024-05-14 11:16:44.088064 c4m_pdk_ihpsg13g2-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        6 2024-05-14 11:16:44.084064 c4m_pdk_ihpsg13g2-0.0.3/version.txt
--rw-r--r--   0        0        0     6003 1970-01-01 00:00:00.000000 c4m_pdk_ihpsg13g2-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      992 2024-05-21 16:32:05.503229 c4m_pdk_ihpsg13g2-0.0.4/LICENSE.md
+-rw-r--r--   0        0        0     5900 2024-05-27 09:15:13.730661 c4m_pdk_ihpsg13g2-0.0.4/README.md
+-rw-r--r--   0        0        0      449 2024-04-12 16:31:42.068929 c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/__init__.py
+-rw-r--r--   0        0        0     4282 2024-05-24 10:27:07.769535 c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/_io_compliance.py
+-rw-r--r--   0        0        0     6918 2024-05-21 16:32:05.503229 c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/io.py
+-rw-r--r--   0        0        0      517 2024-05-21 16:32:05.503229 c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/klayout.py
+-rw-r--r--   0        0        0       23 2024-05-21 16:49:14.793773 c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/__init__.py
+-rw-r--r--   0        0        0      775 2024-05-21 16:49:14.813773 c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/all.spice
+-rw-r--r--   0        0        0    24555 2024-05-21 16:49:14.805773 c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/cornerMOShv.lib
+-rw-r--r--   0        0        0    22926 2024-05-21 16:49:14.801773 c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/cornerMOSlv.lib
+-rw-r--r--   0        0        0     2460 2024-05-21 16:49:14.813773 c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/cornerRES.lib
+-rw-r--r--   0        0        0     3580 2024-05-21 16:49:14.813773 c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/diodes.lib
+-rw-r--r--   0        0        0     1935 2024-05-21 16:49:14.809773 c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/resistors_mod.lib
+-rw-r--r--   0        0        0     1039 2024-05-21 16:49:14.809773 c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/resistors_parm.lib
+-rw-r--r--   0        0        0     1045 2024-05-21 16:49:14.809773 c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/resistors_stat.lib
+-rw-r--r--   0        0        0     6144 2024-05-21 16:49:14.801773 c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_mod.lib
+-rw-r--r--   0        0        0    40662 2024-05-21 16:49:14.801773 c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_parm.lib
+-rw-r--r--   0        0        0     4027 2024-05-21 16:49:14.805773 c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_stat.lib
+-rw-r--r--   0        0        0     6110 2024-05-21 16:49:14.797773 c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_mod.lib
+-rw-r--r--   0        0        0    40995 2024-05-21 16:49:14.797773 c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_parm.lib
+-rw-r--r--   0        0        0     3667 2024-05-21 16:49:14.797773 c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_stat.lib
+-rw-r--r--   0        0        0    18487 2024-05-24 11:22:53.458741 c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/pdkmaster.py
+-rw-r--r--   0        0        0     2617 2024-02-14 16:48:41.345718 c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/pyspice.py
+-rw-r--r--   0        0        0     4300 2024-02-14 17:18:42.851496 c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/stdcell.py
+-rw-r--r--   0        0        0     1551 2024-05-27 12:47:09.546287 c4m_pdk_ihpsg13g2-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        6 2024-05-27 12:47:09.542287 c4m_pdk_ihpsg13g2-0.0.4/version.txt
+-rw-r--r--   0        0        0     6351 1970-01-01 00:00:00.000000 c4m_pdk_ihpsg13g2-0.0.4/PKG-INFO
```

### Comparing `c4m_pdk_ihpsg13g2-0.0.3/LICENSE.md` & `c4m_pdk_ihpsg13g2-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.3/README.md` & `c4m_pdk_ihpsg13g2-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 This is the Chips4Makers' PDK for the SG13G2 open source PDK.
 
 # Versions
 
+* [v0.0.4](https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/-/commits/v0.0.4):
+  * Fix for wrongly connected guard ring in sg13g2_IOPadVdd
+  * Don't try to extract modified ESD diodes as ESD diodes but extract them as regular d(p)antenna diodes
+  * Use minimum width of 0.48µm for diodes, this is new rule not yet present in design rules.
 * [v0.0.3](https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/-/commits/v0.0.3):
-  * Critical fix IOPadVdd
+  * Critical fix sg13g2_IOPadVdd
   * Improved generation of all the files for upstreaming
 * [v0.0.2](https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/-/commits/v0.0.2): build infrastructure and dependencies update; no major code changes but KLayout PCell lib support added.
 * [v0.0.1](https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/-/commits/v0.0.1): First public release; main achievement is that code can generate a version of the IO library ready for upstreaming to [IHP-Open-PDK](https://github.com/IHP-GmbH/IHP-Open-PDK/).  
   It can also generate standard cells but these have not been used yet in P&R.
 
 ## Alpha Version of Code
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/_io_compliance.py` & `c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/_io_compliance.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,23 +37,14 @@
     TEXT = cast(_prm.Auxiliary, _prims["TEXT"])
     if dio.type_ == "n":
         p = _geo.Point(x=0.5*dio.active_width, y=0.5*dio.active_width)
         lbl = _geo.Label(origin=p, text="sub!")
         dio.layout.add_shape(
             shape=lbl, layer=TEXT, net=None,
         )
-        dio_lbl = "diodevss_4kv"
-    else:
-        assert dio.type_ == "p"
-        dio_lbl = "diodevdd_4kv"
-    p = _geo.Point(x=0.5*dio.innerwidth, y=0.5*dio.outerheight)
-    lbl = _geo.Label(origin=p, text=dio_lbl)
-    dio.layout.add_shape(
-        shape=lbl, layer=TEXT, net=None,
-    )
     if create_cb:
         create_cb(dio)
 
 
 class PadIn(PadInT):
     "Add PAD label for Calibre ESD diode extraction"
     def _create_layout(self):
```

### Comparing `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/io.py` & `c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/io.py`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/klayout.py` & `c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/klayout.py`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/all.spice` & `c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/all.spice`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/cornerMOShv.lib` & `c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/cornerMOShv.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/cornerMOSlv.lib` & `c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/cornerMOSlv.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/cornerRES.lib` & `c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/cornerRES.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/diodes.lib` & `c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/diodes.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/resistors_mod.lib` & `c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/resistors_mod.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/resistors_parm.lib` & `c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/resistors_parm.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/resistors_stat.lib` & `c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/resistors_stat.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_mod.lib` & `c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_mod.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_parm.lib` & `c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_parm.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_stat.lib` & `c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_stat.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_mod.lib` & `c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_mod.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_parm.lib` & `c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_parm.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_stat.lib` & `c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_stat.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/pdkmaster.py` & `c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/pdkmaster.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,20 +311,22 @@
 
         # diodes
         recog_dio = _prm.Marker(name="Recog.dio")
         prims += (
             recog_dio,
             _prm.Diode(
                 name="ndiode", wire=Activ,
+                min_width=0.48, # rule not yet in DRM
                 indicator=recog_dio,
                 min_indicator_enclosure=_prp.Enclosure(0.02), # From GDSII
                 implant=(), min_implant_enclosure=(),
             ),
             _prm.Diode(
                 name="pdiode", wire=Activ,
+                min_width=0.48, # rule not yet in DRM
                 indicator=recog_dio,
                 min_indicator_enclosure=_prp.Enclosure(0.02), # From GDSII
                 implant=pSD, min_implant_enclosure=(),
                 well=NWell,
             ),
         )
```

### Comparing `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/pyspice.py` & `c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/pyspice.py`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/stdcell.py` & `c4m_pdk_ihpsg13g2-0.0.4/c4m/pdk/ihpsg13g2/stdcell.py`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.3/pyproject.toml` & `c4m_pdk_ihpsg13g2-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 authors = [
     { name = "Chips4Makers contributors" },
 ]
 dependencies = [
     "PDKMaster~=0.11.0.post2",
     "pdkmaster-io-klayout~=0.1.1.post1",
     "c4m-flexcell~=0.4.2.post3",
-    "c4m-flexio~=0.4.3",
+    "c4m-flexio~=0.4.5",
 ]
 requires-python = "~=3.8"
 readme = "README.md"
-version = "0.0.3"
+version = "0.0.4"
 
 [project.license]
 text = "GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `c4m_pdk_ihpsg13g2-0.0.3/PKG-INFO` & `c4m_pdk_ihpsg13g2-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: c4m-pdk-ihpsg13g2
-Version: 0.0.3
+Version: 0.0.4
 Summary: PDKMaster based PDK for open source IHP SG13G2 process
 Author: Chips4Makers contributors
 License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
 Requires-Python: ~=3.8
 Requires-Dist: PDKMaster~=0.11.0.post2
 Requires-Dist: pdkmaster-io-klayout~=0.1.1.post1
 Requires-Dist: c4m-flexcell~=0.4.2.post3
-Requires-Dist: c4m-flexio~=0.4.3
+Requires-Dist: c4m-flexio~=0.4.5
 Description-Content-Type: text/markdown
 
 This is the Chips4Makers' PDK for the SG13G2 open source PDK.
 
 # Versions
 
+* [v0.0.4](https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/-/commits/v0.0.4):
+  * Fix for wrongly connected guard ring in sg13g2_IOPadVdd
+  * Don't try to extract modified ESD diodes as ESD diodes but extract them as regular d(p)antenna diodes
+  * Use minimum width of 0.48µm for diodes, this is new rule not yet present in design rules.
 * [v0.0.3](https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/-/commits/v0.0.3):
-  * Critical fix IOPadVdd
+  * Critical fix sg13g2_IOPadVdd
   * Improved generation of all the files for upstreaming
 * [v0.0.2](https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/-/commits/v0.0.2): build infrastructure and dependencies update; no major code changes but KLayout PCell lib support added.
 * [v0.0.1](https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/-/commits/v0.0.1): First public release; main achievement is that code can generate a version of the IO library ready for upstreaming to [IHP-Open-PDK](https://github.com/IHP-GmbH/IHP-Open-PDK/).  
   It can also generate standard cells but these have not been used yet in P&R.
 
 ## Alpha Version of Code
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

