# Comparing `tmp/c4m_flexio-0.4.4.tar.gz` & `tmp/c4m_flexio-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4m_flexio-0.4.4.tar", last modified: Fri May 24 09:57:54 2024, max compression
+gzip compressed data, was "c4m_flexio-0.4.5.tar", last modified: Mon May 27 07:48:34 2024, max compression
```

## Comparing `c4m_flexio-0.4.4.tar` & `c4m_flexio-0.4.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      992 2024-05-21 16:32:45.122863 c4m_flexio-0.4.4/LICENSE.md
--rw-r--r--   0        0        0     2958 2024-05-24 09:48:44.314177 c4m_flexio-0.4.4/README.md
--rw-r--r--   0        0        0      170 2024-05-21 16:32:45.122863 c4m_flexio-0.4.4/c4m/flexio/__init__.py
--rw-r--r--   0        0        0    18938 2024-05-21 16:32:45.122863 c4m_flexio-0.4.4/c4m/flexio/_helpers.py
--rw-r--r--   0        0        0   106573 2024-05-21 16:45:20.491928 c4m_flexio-0.4.4/c4m/flexio/cell.py
--rw-r--r--   0        0        0   236164 2024-05-21 16:32:45.122863 c4m_flexio-0.4.4/c4m/flexio/factory.py
--rw-r--r--   0        0        0    37990 2024-05-21 16:32:45.122863 c4m_flexio-0.4.4/c4m/flexio/specification.py
--rw-r--r--   0        0        0      706 2024-05-24 09:57:54.349282 c4m_flexio-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     3297 1970-01-01 00:00:00.000000 c4m_flexio-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      992 2024-05-21 16:32:45.122863 c4m_flexio-0.4.5/LICENSE.md
+-rw-r--r--   0        0        0     3072 2024-05-27 07:34:10.843948 c4m_flexio-0.4.5/README.md
+-rw-r--r--   0        0        0      170 2024-05-21 16:32:45.122863 c4m_flexio-0.4.5/c4m/flexio/__init__.py
+-rw-r--r--   0        0        0    18938 2024-05-21 16:32:45.122863 c4m_flexio-0.4.5/c4m/flexio/_helpers.py
+-rw-r--r--   0        0        0   106573 2024-05-21 16:45:20.491928 c4m_flexio-0.4.5/c4m/flexio/cell.py
+-rw-r--r--   0        0        0   236334 2024-05-24 11:39:49.641620 c4m_flexio-0.4.5/c4m/flexio/factory.py
+-rw-r--r--   0        0        0    37990 2024-05-21 16:32:45.122863 c4m_flexio-0.4.5/c4m/flexio/specification.py
+-rw-r--r--   0        0        0      706 2024-05-27 07:48:34.968058 c4m_flexio-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     3411 1970-01-01 00:00:00.000000 c4m_flexio-0.4.5/PKG-INFO
```

### Comparing `c4m_flexio-0.4.4/LICENSE.md` & `c4m_flexio-0.4.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `c4m_flexio-0.4.4/README.md` & `c4m_flexio-0.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 A IO library is a collection of cells that allows to do the input and output from on-chip signals to outside the chip. Typically these libraries with a fixed set of cells with a fixed layout and functionality and provided by the foundry or a third party.
 
 Purpose of c4m-flexio library is to have a library that is easily scalable between different technologies using the [PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster) framework. It will also be configurable to adapt the cells to one's needs.
 
 ## Release history
 
+* [v0.4.5](https://gitlab.com/Chips4Makers/c4m-flexio/-/commits/v0.4.5):
+  * Obey min. width for generated diodes
 * [v0.4.4](https://gitlab.com/Chips4Makers/c4m-flexio/-/commits/v0.4.4):
   * IOPadVdd needed another fix as a guard was wrongly connected to vdd
 * [v0.4.3](https://gitlab.com/Chips4Makers/c4m-flexio/-/commits/v0.4.3):
   * Critical fix for IOPadVdd layout.
   * make this repo part of project Arrakeen; use common setup like license, DCO check etc.
 * [v0.4.2](https://gitlab.com/Chips4Makers/c4m-flexio/-/commits/v0.4.2):
   Several features for IHP SG13G2 support: RCClamp in IOPadVdd, custom layout manipulation
```

### Comparing `c4m_flexio-0.4.4/c4m/flexio/_helpers.py` & `c4m_flexio-0.4.5/c4m/flexio/_helpers.py`

 * *Files identical despite different names*

### Comparing `c4m_flexio-0.4.4/c4m/flexio/cell.py` & `c4m_flexio-0.4.5/c4m/flexio/cell.py`

 * *Files identical despite different names*

### Comparing `c4m_flexio-0.4.4/c4m/flexio/factory.py` & `c4m_flexio-0.4.5/c4m/flexio/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,16 +319,16 @@
             well_args = {} if type_ == "n" else {"well_net": iovdd, "bottom_well": nwell}
             l_ch = layoutfab.layout_primitive(
                 prim=cont, portnets={"conn": gate}, **well_args, rows=2,
                 bottom=diode.wire, bottom_implant=diode.implant,
             )
             chact_bounds = l_ch.bounds(mask=diode.wire.mask)
             dgate = ckt.instantiate(diode, name="DGATE",
-                width=(chact_bounds.right - chact_bounds.left),
-                height=(chact_bounds.top - chact_bounds.bottom),
+                width=max(chact_bounds.right - chact_bounds.left, diode.min_width),
+                height=max(chact_bounds.top - chact_bounds.bottom, diode.min_width),
             )
             an = dgate.ports.anode
             cath = dgate.ports.cathode
             gate.childports += an if type_ == "p" else cath
             source.childports += an if type_ == "n" else cath
 
             x = tech.on_grid(0.5*spec.monocell_width + 0.5*(
@@ -717,14 +717,15 @@
         l_ch = layouter.fab.layout_primitive(
             cont, portnets={"conn": core}, columns=2,
             bottom=dn_prim.wire, bottom_implant=dn_prim.implant,
             bottom_height=diode_height,
         )
         dnchact_bounds = l_ch.bounds(mask=comp.active.mask)
         diode_width = dnchact_bounds.right - dnchact_bounds.left
+        assert diode_width > (dn_prim.min_width - _geo.epsilon)
         dn = ckt.instantiate(
             dn_prim, name="DN", width=diode_width, height=diode_height,
         )
         core.childports += dn.ports.cathode
         iovss.childports += dn.ports.anode
 
         guard2_width = (
@@ -780,14 +781,15 @@
         l_ch = layouter.fab.layout_primitive(
             cont, portnets={"conn": core}, rows=2,
             bottom=dp_prim.wire, bottom_implant=dp_prim.implant,
             bottom_width=diode2_width,
         )
         dpchact_bounds = l_ch.bounds(mask=comp.active.mask)
         diode2_height = dpchact_bounds.top - dpchact_bounds.bottom
+        assert diode2_height > (dn_prim.min_width - _geo.epsilon)
         dp = ckt.instantiate(
             dp_prim, name="DP", width=diode2_width, height=diode2_height,
         )
         core.childports += dp.ports.anode
         iovdd.childports += dp.ports.cathode
 
         guard3_height = (
```

### Comparing `c4m_flexio-0.4.4/c4m/flexio/specification.py` & `c4m_flexio-0.4.5/c4m/flexio/specification.py`

 * *Files identical despite different names*

### Comparing `c4m_flexio-0.4.4/pyproject.toml` & `c4m_flexio-0.4.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 dependencies = [
     "PDKMaster>=0.10.2,<0.12.0",
     "c4m-flexcell~=0.4.2",
 ]
 requires-python = "~=3.8"
 readme = "README.md"
-version = "0.4.4"
+version = "0.4.5"
 
 [project.license]
 text = "GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `c4m_flexio-0.4.4/PKG-INFO` & `c4m_flexio-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4m-flexio
-Version: 0.4.4
+Version: 0.4.5
 Summary: PDKMaster based scalable IO library
 Author: Chips4Makers contributors
 License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
 Requires-Python: ~=3.8
 Requires-Dist: PDKMaster<0.12.0,>=0.10.2
 Requires-Dist: c4m-flexcell~=0.4.2
 Description-Content-Type: text/markdown
@@ -13,14 +13,16 @@
 
 A IO library is a collection of cells that allows to do the input and output from on-chip signals to outside the chip. Typically these libraries with a fixed set of cells with a fixed layout and functionality and provided by the foundry or a third party.
 
 Purpose of c4m-flexio library is to have a library that is easily scalable between different technologies using the [PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster) framework. It will also be configurable to adapt the cells to one's needs.
 
 ## Release history
 
+* [v0.4.5](https://gitlab.com/Chips4Makers/c4m-flexio/-/commits/v0.4.5):
+  * Obey min. width for generated diodes
 * [v0.4.4](https://gitlab.com/Chips4Makers/c4m-flexio/-/commits/v0.4.4):
   * IOPadVdd needed another fix as a guard was wrongly connected to vdd
 * [v0.4.3](https://gitlab.com/Chips4Makers/c4m-flexio/-/commits/v0.4.3):
   * Critical fix for IOPadVdd layout.
   * make this repo part of project Arrakeen; use common setup like license, DCO check etc.
 * [v0.4.2](https://gitlab.com/Chips4Makers/c4m-flexio/-/commits/v0.4.2):
   Several features for IHP SG13G2 support: RCClamp in IOPadVdd, custom layout manipulation
```

