# Comparing `tmp/pbc_sjfhsjfh-0.0.1.tar.gz` & `tmp/pbc_sjfhsjfh-0.0.2.tar.gz`

## Comparing `pbc_sjfhsjfh-0.0.1.tar` & `pbc_sjfhsjfh-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.1/requirements.txt
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.1/src/pbc/__init__.py
--rw-r--r--   0        0        0    12294 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.1/src/pbc/bin.py
--rw-r--r--   0        0        0     6662 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.1/src/pbc/phira_chart.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.1/src/pbc/utils/__init__.py
--rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.1/src/pbc/utils/fraction.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.1/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.1/LICENSE
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.1/README.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.2/src/pbc/__init__.py
+-rw-r--r--   0        0        0    13125 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.2/src/pbc/bin.py
+-rw-r--r--   0        0        0     7331 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.2/src/pbc/phira_chart.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.2/src/pbc/utils/__init__.py
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.2/src/pbc/utils/fraction.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.2/LICENSE
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.2/README.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.2/PKG-INFO
```

### Comparing `pbc_sjfhsjfh-0.0.1/src/pbc/bin.py` & `pbc_sjfhsjfh-0.0.2/src/pbc/bin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from io import BytesIO
 import struct
 from typing import Any, List, Literal, Tuple, TypeVar, Union
-from .phira_chart import PhiraAnim, PhiraBpmList, PhiraChart, PhiraChartSettings, PhiraControlObject, PhiraKeyFrame, PhiraLine, PhiraNote, PhiraObject
+from .phira_chart import PhiraAnim, PhiraBpmList, PhiraChart, PhiraChartSettings, PhiraControlObject, PhiraHold, PhiraKeyFrame, PhiraLine, PhiraNote, PhiraObject
 
 
 SupportBinName = Literal["Byte", "Bool", "Int", "Float", "String", "Color",
                          "Object", "CtrlObject", "Note", "JudgeLine", "ChartSettings", "Chart"] | str
 """ "KeyFrame:xxx" for KeyFrame<xxx>, "Anim:xxx" for Anim<xxx>"""
 
 
@@ -111,22 +111,37 @@
                     size=reader.read("Anim:Float"),
                     pos=reader.read("Anim:Float"),
                     y=reader.read("Anim:Float"),
                 )
             case "Note":
                 object = reader.read("Object")
                 kind = ["tap", "hold", "flick", "drag"][reader.read("Byte")]
+                if kind == "hold":
+                    end_time = reader.read("Float")
+                    end_height = reader.read("Float")
                 time = reader.time()
                 height = reader.read("Float")
                 speedB = reader.read("Bool")
                 speed = 1.0
                 if speedB:
                     speed = reader.read("Float")
                 above = reader.read("Bool")
                 fake = reader.read("Bool")
+                if kind == "hold":
+                    return PhiraHold(
+                        object=object,
+                        kind=kind,
+                        time=time,
+                        height=height,
+                        speed=speed,
+                        above=above,
+                        fake=fake,
+                        end_time=end_time,
+                        end_height=end_height,
+                    )
                 return PhiraNote(
                     object=object,
                     kind=kind,
                     time=time,
                     height=height,
                     speed=speed,
                     above=above,
@@ -236,14 +251,18 @@
                 writer.write(value_CtrlObject.pos, "Anim:Float")
                 writer.write(value_CtrlObject.y, "Anim:Float")
             case "Note":
                 value_Note: PhiraNote = value
                 writer.write(value_Note.object, "Object")
                 writer.write(["tap", "hold", "flick", "drag"].index(
                     value_Note.kind), "Byte")
+                if isinstance(value_Note, PhiraHold):
+                    value_Hold: PhiraHold = value_Note
+                    writer.write(value_Hold.end_time, "Float")
+                    writer.write(value_Hold.end_height, "Float")
                 writer.time(value_Note.time)
                 writer.write(value_Note.height, "Float")
                 writer.write(value_Note.speed != 1.0, "Bool")
                 if value_Note.speed != 1.0:
                     writer.write(value_Note.speed, "Float")
                 writer.write(value_Note.above, "Bool")
                 writer.write(value_Note.fake, "Bool")
```

### Comparing `pbc_sjfhsjfh-0.0.1/src/pbc/phira_chart.py` & `pbc_sjfhsjfh-0.0.2/src/pbc/phira_chart.py`

 * *Files 10% similar despite different names*

```diff
@@ -210,7 +210,28 @@
         self.height = height
         self.speed = speed
         self.above = above
         self.multiple_hint = multiple_hint
         self.fake = fake
         self.judge = judge
         """Not sure what this is for, from RPE only"""
+        self.end_time = None
+        self.end_height = None
+
+class PhiraHold(PhiraNote):
+    def __init__(
+        self,
+        time: float,
+        height: float,
+        end_time: float,
+        end_height: float,
+        kind: Literal["tap", "drag", "hold", "flick"] = "hold",
+        multiple_hint: bool = False,
+        object: PhiraObject = PhiraObject(),
+        speed: float = 1.,
+        above: bool = True,
+        fake: bool = False,
+        judge: Literal["NotJudged"] = "NotJudged",
+    ):
+        super().__init__(kind, time, height, multiple_hint, object, speed, above, fake, judge)
+        self.end_time = end_time
+        self.end_height = end_height
```

### Comparing `pbc_sjfhsjfh-0.0.1/src/pbc/utils/fraction.py` & `pbc_sjfhsjfh-0.0.2/src/pbc/utils/fraction.py`

 * *Files identical despite different names*

### Comparing `pbc_sjfhsjfh-0.0.1/LICENSE` & `pbc_sjfhsjfh-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pbc_sjfhsjfh-0.0.1/pyproject.toml` & `pbc_sjfhsjfh-0.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "pbc_sjfhsjfh"
-version = "0.0.1"
+version = "0.0.2"
 authors = [{ name = "sjfhsjfh", email = "sjfhsjfh@qq.com" }]
 description = "Phira chart structure package"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

