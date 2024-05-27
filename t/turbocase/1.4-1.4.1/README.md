# Comparing `tmp/turbocase-1.4.tar.gz` & `tmp/turbocase-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbocase-1.4.tar", last modified: Sun May 26 18:44:54 2024, max compression
+gzip compressed data, was "turbocase-1.4.1.tar", last modified: Mon May 27 10:44:55 2024, max compression
```

## Comparing `turbocase-1.4.tar` & `turbocase-1.4.1.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 18:44:54.718432 turbocase-1.4/
--rw-r--r--   0 root         (0) root         (0)     1069 2024-05-15 14:32:06.000000 turbocase-1.4/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      269 2024-05-26 18:44:54.718432 turbocase-1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2844 2024-05-17 13:48:51.000000 turbocase-1.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-26 18:44:54.718432 turbocase-1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      438 2024-05-26 18:42:45.000000 turbocase-1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 18:44:54.715099 turbocase-1.4/turbocase/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 00:06:28.000000 turbocase-1.4/turbocase/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1048 2024-05-17 16:22:48.000000 turbocase-1.4/turbocase/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1687 2024-05-26 14:19:02.000000 turbocase-1.4/turbocase/cases.py
--rw-r--r--   0 root         (0) root         (0)    12315 2024-05-26 14:19:02.000000 turbocase-1.4/turbocase/kicad.py
--rw-r--r--   0 root         (0) root         (0)     4603 2024-05-26 14:26:10.000000 turbocase-1.4/turbocase/scad.py
--rw-r--r--   0 root         (0) root         (0)     1279 2024-05-15 18:26:04.000000 turbocase-1.4/turbocase/vector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 18:44:54.718432 turbocase-1.4/turbocase.egg-info/
--rw-r--r--   0 root         (0) root         (0)      269 2024-05-26 18:44:54.000000 turbocase-1.4/turbocase.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      350 2024-05-26 18:44:54.000000 turbocase-1.4/turbocase.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-26 18:44:54.000000 turbocase-1.4/turbocase.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2024-05-26 18:44:54.000000 turbocase-1.4/turbocase.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-26 18:44:54.000000 turbocase-1.4/turbocase.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-26 18:44:54.000000 turbocase-1.4/turbocase.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 10:44:55.952627 turbocase-1.4.1/
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-05-15 14:32:06.000000 turbocase-1.4.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      271 2024-05-27 10:44:55.952627 turbocase-1.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2844 2024-05-17 13:48:51.000000 turbocase-1.4.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 10:44:55.952627 turbocase-1.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      459 2024-05-27 10:44:46.000000 turbocase-1.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 10:44:55.949294 turbocase-1.4.1/turbocase/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 00:06:28.000000 turbocase-1.4.1/turbocase/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2024-05-17 16:22:48.000000 turbocase-1.4.1/turbocase/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2024-05-26 14:19:02.000000 turbocase-1.4.1/turbocase/cases.py
+-rw-r--r--   0 root         (0) root         (0)    12315 2024-05-26 14:19:02.000000 turbocase-1.4.1/turbocase/kicad.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 10:44:55.952627 turbocase-1.4.1/turbocase/parts/
+-rw-r--r--   0 root         (0) root         (0)     1664 2024-05-26 14:17:50.000000 turbocase-1.4.1/turbocase/parts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2024-05-23 00:53:13.000000 turbocase-1.4.1/turbocase/parts/batteryholder.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-05-26 14:25:33.000000 turbocase-1.4.1/turbocase/parts/cutout.py
+-rw-r--r--   0 root         (0) root         (0)     3008 2024-05-26 13:34:36.000000 turbocase-1.4.1/turbocase/parts/keyhole.py
+-rw-r--r--   0 root         (0) root         (0)     3472 2024-05-26 13:51:45.000000 turbocase-1.4.1/turbocase/parts/screws.py
+-rw-r--r--   0 root         (0) root         (0)     2373 2024-05-23 01:24:44.000000 turbocase-1.4.1/turbocase/parts/shape.py
+-rw-r--r--   0 root         (0) root         (0)     4585 2024-05-27 09:39:56.000000 turbocase-1.4.1/turbocase/scad.py
+-rw-r--r--   0 root         (0) root         (0)     1279 2024-05-15 18:26:04.000000 turbocase-1.4.1/turbocase/vector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 10:44:55.952627 turbocase-1.4.1/turbocase.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      271 2024-05-27 10:44:55.000000 turbocase-1.4.1/turbocase.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      515 2024-05-27 10:44:55.000000 turbocase-1.4.1/turbocase.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 10:44:55.000000 turbocase-1.4.1/turbocase.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2024-05-27 10:44:55.000000 turbocase-1.4.1/turbocase.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-27 10:44:55.000000 turbocase-1.4.1/turbocase.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-27 10:44:55.000000 turbocase-1.4.1/turbocase.egg-info/top_level.txt
```

### Comparing `turbocase-1.4/LICENSE.txt` & `turbocase-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `turbocase-1.4/README.md` & `turbocase-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `turbocase-1.4/turbocase/__main__.py` & `turbocase-1.4.1/turbocase/__main__.py`

 * *Files identical despite different names*

### Comparing `turbocase-1.4/turbocase/cases.py` & `turbocase-1.4.1/turbocase/cases.py`

 * *Files identical despite different names*

### Comparing `turbocase-1.4/turbocase/kicad.py` & `turbocase-1.4.1/turbocase/kicad.py`

 * *Files identical despite different names*

### Comparing `turbocase-1.4/turbocase/scad.py` & `turbocase-1.4.1/turbocase/scad.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     result += f'    standoff_height = {case.standoff_height};\n'
     result += f'    floor_height = {case.floor_thickness};\n'
     result += f'    pcb_thickness = {case.pcb_thickness};\n'
     result += f'    inner_height = standoff_height + pcb_thickness + {max(case.max_connector_height, case.max_part_height - case.standoff_height - case.pcb_thickness)};\n'
     result += f'    pcb_top = floor_height + standoff_height + pcb_thickness;\n'
     result += '\n'
     result += '    difference() {\n'
-    result += f'        box({case.wall_thickness}, {case.floor_thickness}, inner_height) ' + '{\n'
+    result += f'        box({case.wall_thickness}, floor_height, inner_height) ' + '{\n'
     result += '            ' + _make_scad_polygon(case.inner_path)
     result += '        }\n\n'
 
     for shape in case.cutouts:
         if shape.is_circle:
             result += f'    translate([{shape.point[0]}, {shape.point[1]}, -1])\n'
             result += f'        #cylinder(floor_height+2, {shape.radius}, {shape.radius});\n'
@@ -93,36 +93,36 @@
         result += f'    translate([{conn.position[0]}, {conn.position[1]}, pcb_top])\n' \
                   f'    rotate([0, 0, {conn.position[2] + 180}])\n' \
                   f'        #connector({conn.bounds[0]},{conn.bounds[1]},{conn.bounds[2]},{conn.bounds[3]},{conn.prop_height + 0.2});\n\n'
 
     for part in case.parts:
         if part.substract is None:
             continue
-        z = case.floor_thickness
+        z = 'floor_height'
         if part.offset_pcb:
             z = 'pcb_top'
         result += f'    // {part.description}\n'
         result += f'    translate([{part.position[0]}, {part.position[1]}, {z}])\n'
         if len(part.position) == 3:
             result += f'    rotate([0, 0, {part.position[2] + 180}])\n'
         result += f'        {part.substract}\n'
 
     result += '    }\n\n'
 
     for mount in case.pcb_mount:
         result += f'    // {mount[3]}\n'
-        result += f'    translate([{mount[0][0]}, {mount[0][1]}, {case.floor_thickness}])\n'
+        result += f'    translate([{mount[0][0]}, {mount[0][1]}, floor_height])\n'
         # This currently creates correct holes for the M3 threaded metal inserts I have. Not generic
-        result += f'    mount({mount[1] + 0.2}, {mount[2]}, 5);\n\n'
+        result += f'    mount({mount[1] + 0.2}, {mount[2]}, standoff_height);\n\n'
 
     for part in case.parts:
         if part.add is None:
             continue
         result += f'    // {part.description}\n'
-        z = case.floor_thickness
+        z = 'floor_height'
         if part.offset_pcb:
             z = 'pcb_top'
         result += f'    translate([{part.position[0]}, {part.position[1]}, {z}])\n'
         if len(part.position) == 3:
             result += f'    rotate([0, 0, {part.position[2] + 180}])\n'
         result += f'        {part.add}\n'
```

### Comparing `turbocase-1.4/turbocase/vector.py` & `turbocase-1.4.1/turbocase/vector.py`

 * *Files identical despite different names*

