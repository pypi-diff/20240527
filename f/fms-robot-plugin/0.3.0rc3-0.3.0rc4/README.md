# Comparing `tmp/fms_robot_plugin-0.3.0rc3.tar.gz` & `tmp/fms_robot_plugin-0.3.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fms_robot_plugin-0.3.0rc3.tar", max compression
+gzip compressed data, was "fms_robot_plugin-0.3.0rc4.tar", max compression
```

## Comparing `fms_robot_plugin-0.3.0rc3.tar` & `fms_robot_plugin-0.3.0rc4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       26 2024-05-22 04:59:27.882549 fms_robot_plugin-0.3.0rc3/README.md
--rw-r--r--   0        0        0       49 2024-05-22 04:59:27.886549 fms_robot_plugin-0.3.0rc3/fms_robot_plugin/__init__.py
--rw-r--r--   0        0        0     1601 2024-05-22 04:59:27.886549 fms_robot_plugin-0.3.0rc3/fms_robot_plugin/constants.py
--rw-r--r--   0        0        0     1824 2024-05-22 04:59:27.886549 fms_robot_plugin-0.3.0rc3/fms_robot_plugin/mqtt.py
--rw-r--r--   0        0        0     9461 2024-05-22 04:59:27.886549 fms_robot_plugin-0.3.0rc3/fms_robot_plugin/robot.py
--rw-r--r--   0        0        0     3488 2024-05-22 04:59:27.886549 fms_robot_plugin-0.3.0rc3/fms_robot_plugin/typings.py
--rw-r--r--   0        0        0      657 2024-05-22 04:59:27.886549 fms_robot_plugin-0.3.0rc3/pyproject.toml
--rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 fms_robot_plugin-0.3.0rc3/setup.py
--rw-r--r--   0        0        0      502 1970-01-01 00:00:00.000000 fms_robot_plugin-0.3.0rc3/PKG-INFO
+-rw-r--r--   0        0        0       26 2024-05-27 05:45:58.239719 fms_robot_plugin-0.3.0rc4/README.md
+-rw-r--r--   0        0        0       49 2024-05-27 05:45:58.239719 fms_robot_plugin-0.3.0rc4/fms_robot_plugin/__init__.py
+-rw-r--r--   0        0        0     1601 2024-05-27 05:45:58.239719 fms_robot_plugin-0.3.0rc4/fms_robot_plugin/constants.py
+-rw-r--r--   0        0        0     1824 2024-05-27 05:45:58.239719 fms_robot_plugin-0.3.0rc4/fms_robot_plugin/mqtt.py
+-rw-r--r--   0        0        0     9461 2024-05-27 05:45:58.243719 fms_robot_plugin-0.3.0rc4/fms_robot_plugin/robot.py
+-rw-r--r--   0        0        0     3911 2024-05-27 05:45:58.243719 fms_robot_plugin-0.3.0rc4/fms_robot_plugin/typings.py
+-rw-r--r--   0        0        0      657 2024-05-27 05:45:58.243719 fms_robot_plugin-0.3.0rc4/pyproject.toml
+-rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 fms_robot_plugin-0.3.0rc4/setup.py
+-rw-r--r--   0        0        0      502 1970-01-01 00:00:00.000000 fms_robot_plugin-0.3.0rc4/PKG-INFO
```

### Comparing `fms_robot_plugin-0.3.0rc3/fms_robot_plugin/constants.py` & `fms_robot_plugin-0.3.0rc4/fms_robot_plugin/constants.py`

 * *Files identical despite different names*

### Comparing `fms_robot_plugin-0.3.0rc3/fms_robot_plugin/mqtt.py` & `fms_robot_plugin-0.3.0rc4/fms_robot_plugin/mqtt.py`

 * *Files identical despite different names*

### Comparing `fms_robot_plugin-0.3.0rc3/fms_robot_plugin/robot.py` & `fms_robot_plugin-0.3.0rc4/fms_robot_plugin/robot.py`

 * *Files identical despite different names*

### Comparing `fms_robot_plugin-0.3.0rc3/fms_robot_plugin/typings.py` & `fms_robot_plugin-0.3.0rc4/fms_robot_plugin/typings.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import enum
 import datetime
 
 from typing import List, Union, Optional
-from pydantic import BaseModel
+from pydantic import BaseModel, validator
 
 
 class TaskType(str, enum.Enum):
     """
     Possible types of tasks in FMS2
     """
 
@@ -158,14 +158,26 @@
     id: str
     type: TaskType
     data: Union[Waypoint, WaypointTraffic, DynamicTask, dict]
     map_id: str
     linear_velocity: Optional[float] = None
     angular_velocity: Optional[float] = None
 
+    @validator("data", pre=True, always=True)
+    def validate_data(cls, v, values):
+        task_type = values.get("type")
+        if task_type == TaskType.WaypointTraffic:
+            return WaypointTraffic(**v)
+        elif task_type == TaskType.Waypoint:
+            return Waypoint(**v)
+        elif task_type == TaskType.DynamicTask:
+            return DynamicTask(**v)
+        else:
+            return v
+
 
 class DecimatedPlan(BaseModel):
     poses: List[Pose]
 
 
 class Result(BaseModel):
     class StatusResponse(BaseModel):
```

### Comparing `fms_robot_plugin-0.3.0rc3/pyproject.toml` & `fms_robot_plugin-0.3.0rc4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fms-robot-plugin"
-version = "0.3.0rc3"
+version = "0.3.0rc4"
 description = ""
 authors = [
   "Dionesius Agung <dionesius@movel.ai>",
   "Steven Hansel <steven@movel.ai>"
 ]
 readme = "README.md"
 packages = [{include = "fms_robot_plugin"}]
```

### Comparing `fms_robot_plugin-0.3.0rc3/setup.py` & `fms_robot_plugin-0.3.0rc4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['paho-mqtt>=1.6.1,<2.0.0', 'pydantic>=2.3.0,<3.0.0', 'requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'fms-robot-plugin',
-    'version': '0.3.0rc3',
+    'version': '0.3.0rc4',
     'description': '',
     'long_description': '# FMS Robot Plugin Library',
     'author': 'Dionesius Agung',
     'author_email': 'dionesius@movel.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

