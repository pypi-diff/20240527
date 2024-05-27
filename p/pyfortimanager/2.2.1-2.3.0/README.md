# Comparing `tmp/pyfortimanager-2.2.1.tar.gz` & `tmp/pyfortimanager-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfortimanager-2.2.1.tar", last modified: Wed Mar 27 09:55:27 2024, max compression
+gzip compressed data, was "pyfortimanager-2.3.0.tar", last modified: Mon May 27 14:45:02 2024, max compression
```

## Comparing `pyfortimanager-2.2.1.tar` & `pyfortimanager-2.3.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 rasmus.thing   (502) staff       (20)        0 2024-03-27 09:55:27.905063 pyfortimanager-2.2.1/
--rw-r--r--   0 rasmus.thing   (502) staff       (20)     9612 2024-02-06 17:05:47.000000 pyfortimanager-2.2.1/LICENSE
--rw-r--r--   0 rasmus.thing   (502) staff       (20)     8887 2024-03-27 09:55:27.904820 pyfortimanager-2.2.1/PKG-INFO
--rw-r--r--   0 rasmus.thing   (502) staff       (20)     8172 2024-02-23 10:29:27.000000 pyfortimanager-2.2.1/README.md
-drwxr-xr-x   0 rasmus.thing   (502) staff       (20)        0 2024-03-27 09:55:27.897827 pyfortimanager-2.2.1/pyfortimanager/
--rw-r--r--   0 rasmus.thing   (502) staff       (20)       47 2024-02-06 17:05:47.000000 pyfortimanager-2.2.1/pyfortimanager/__init__.py
-drwxr-xr-x   0 rasmus.thing   (502) staff       (20)        0 2024-03-27 09:55:27.899324 pyfortimanager-2.2.1/pyfortimanager/core/
--rw-r--r--   0 rasmus.thing   (502) staff       (20)        0 2024-02-06 17:05:47.000000 pyfortimanager-2.2.1/pyfortimanager/core/__init__.py
--rw-r--r--   0 rasmus.thing   (502) staff       (20)     3687 2024-02-22 11:37:40.000000 pyfortimanager-2.2.1/pyfortimanager/core/api.py
--rw-r--r--   0 rasmus.thing   (502) staff       (20)      938 2024-02-22 12:01:18.000000 pyfortimanager-2.2.1/pyfortimanager/core/fortimanager.py
-drwxr-xr-x   0 rasmus.thing   (502) staff       (20)        0 2024-03-27 09:55:27.904236 pyfortimanager-2.2.1/pyfortimanager/models/
--rw-r--r--   0 rasmus.thing   (502) staff       (20)        0 2024-02-06 17:05:47.000000 pyfortimanager-2.2.1/pyfortimanager/models/__init__.py
--rw-r--r--   0 rasmus.thing   (502) staff       (20)     1642 2024-02-06 17:05:47.000000 pyfortimanager-2.2.1/pyfortimanager/models/adoms.py
--rw-r--r--   0 rasmus.thing   (502) staff       (20)     5142 2024-02-06 17:05:47.000000 pyfortimanager-2.2.1/pyfortimanager/models/cli_template_groups.py
--rw-r--r--   0 rasmus.thing   (502) staff       (20)     4597 2024-02-22 13:02:17.000000 pyfortimanager-2.2.1/pyfortimanager/models/device_groups.py
--rw-r--r--   0 rasmus.thing   (502) staff       (20)    11104 2024-03-26 08:29:15.000000 pyfortimanager-2.2.1/pyfortimanager/models/fortiaps.py
--rw-r--r--   0 rasmus.thing   (502) staff       (20)     6381 2024-02-22 12:29:28.000000 pyfortimanager-2.2.1/pyfortimanager/models/fortiaps_proxy.py
--rw-r--r--   0 rasmus.thing   (502) staff       (20)     8437 2024-03-27 09:54:37.000000 pyfortimanager-2.2.1/pyfortimanager/models/fortigates.py
--rw-r--r--   0 rasmus.thing   (502) staff       (20)     7388 2024-02-06 17:05:47.000000 pyfortimanager-2.2.1/pyfortimanager/models/fortigates_proxy.py
--rw-r--r--   0 rasmus.thing   (502) staff       (20)    11076 2024-02-08 07:45:45.000000 pyfortimanager-2.2.1/pyfortimanager/models/fortiswitches.py
--rw-r--r--   0 rasmus.thing   (502) staff       (20)     5568 2024-02-22 12:32:18.000000 pyfortimanager-2.2.1/pyfortimanager/models/fortiswitches_proxy.py
--rw-r--r--   0 rasmus.thing   (502) staff       (20)     2068 2024-02-06 17:05:47.000000 pyfortimanager-2.2.1/pyfortimanager/models/install_wizard.py
--rw-r--r--   0 rasmus.thing   (502) staff       (20)     6425 2024-02-09 00:17:37.000000 pyfortimanager-2.2.1/pyfortimanager/models/metadata_variables.py
--rw-r--r--   0 rasmus.thing   (502) staff       (20)    10736 2024-02-22 13:57:47.000000 pyfortimanager-2.2.1/pyfortimanager/models/policy_packages.py
--rw-r--r--   0 rasmus.thing   (502) staff       (20)     5028 2024-02-06 17:05:47.000000 pyfortimanager-2.2.1/pyfortimanager/models/radius_servers.py
--rw-r--r--   0 rasmus.thing   (502) staff       (20)     2140 2024-03-18 09:18:05.000000 pyfortimanager-2.2.1/pyfortimanager/models/scripts.py
--rw-r--r--   0 rasmus.thing   (502) staff       (20)     3061 2024-02-06 17:05:47.000000 pyfortimanager-2.2.1/pyfortimanager/models/sdwan_templates.py
--rw-r--r--   0 rasmus.thing   (502) staff       (20)     4504 2024-02-22 11:55:35.000000 pyfortimanager-2.2.1/pyfortimanager/models/system.py
-drwxr-xr-x   0 rasmus.thing   (502) staff       (20)        0 2024-03-27 09:55:27.904569 pyfortimanager-2.2.1/pyfortimanager.egg-info/
--rw-r--r--   0 rasmus.thing   (502) staff       (20)     8887 2024-03-27 09:55:27.000000 pyfortimanager-2.2.1/pyfortimanager.egg-info/PKG-INFO
--rw-r--r--   0 rasmus.thing   (502) staff       (20)     1030 2024-03-27 09:55:27.000000 pyfortimanager-2.2.1/pyfortimanager.egg-info/SOURCES.txt
--rw-r--r--   0 rasmus.thing   (502) staff       (20)        1 2024-03-27 09:55:27.000000 pyfortimanager-2.2.1/pyfortimanager.egg-info/dependency_links.txt
--rw-r--r--   0 rasmus.thing   (502) staff       (20)        1 2024-02-08 21:02:57.000000 pyfortimanager-2.2.1/pyfortimanager.egg-info/not-zip-safe
--rw-r--r--   0 rasmus.thing   (502) staff       (20)       22 2024-03-27 09:55:27.000000 pyfortimanager-2.2.1/pyfortimanager.egg-info/requires.txt
--rw-r--r--   0 rasmus.thing   (502) staff       (20)       15 2024-03-27 09:55:27.000000 pyfortimanager-2.2.1/pyfortimanager.egg-info/top_level.txt
--rw-r--r--   0 rasmus.thing   (502) staff       (20)       38 2024-03-27 09:55:27.905101 pyfortimanager-2.2.1/setup.cfg
--rw-r--r--   0 rasmus.thing   (502) staff       (20)     1081 2024-03-27 09:55:05.000000 pyfortimanager-2.2.1/setup.py
+drwxr-xr-x   0 rasmus.thing   (502) staff       (20)        0 2024-05-27 14:45:02.911608 pyfortimanager-2.3.0/
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)     9612 2024-02-06 17:05:47.000000 pyfortimanager-2.3.0/LICENSE
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)     8882 2024-05-27 14:45:02.911424 pyfortimanager-2.3.0/PKG-INFO
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)     8172 2024-02-23 10:29:27.000000 pyfortimanager-2.3.0/README.md
+drwxr-xr-x   0 rasmus.thing   (502) staff       (20)        0 2024-05-27 14:45:02.905410 pyfortimanager-2.3.0/pyfortimanager/
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)       47 2024-02-06 17:05:47.000000 pyfortimanager-2.3.0/pyfortimanager/__init__.py
+drwxr-xr-x   0 rasmus.thing   (502) staff       (20)        0 2024-05-27 14:45:02.907113 pyfortimanager-2.3.0/pyfortimanager/core/
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)        0 2024-02-06 17:05:47.000000 pyfortimanager-2.3.0/pyfortimanager/core/__init__.py
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)     3687 2024-02-22 11:37:40.000000 pyfortimanager-2.3.0/pyfortimanager/core/api.py
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)      938 2024-02-22 12:01:18.000000 pyfortimanager-2.3.0/pyfortimanager/core/fortimanager.py
+drwxr-xr-x   0 rasmus.thing   (502) staff       (20)        0 2024-05-27 14:45:02.911094 pyfortimanager-2.3.0/pyfortimanager/models/
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)        0 2024-02-06 17:05:47.000000 pyfortimanager-2.3.0/pyfortimanager/models/__init__.py
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)     1642 2024-02-06 17:05:47.000000 pyfortimanager-2.3.0/pyfortimanager/models/adoms.py
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)     5142 2024-02-06 17:05:47.000000 pyfortimanager-2.3.0/pyfortimanager/models/cli_template_groups.py
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)     4596 2024-05-27 14:32:10.000000 pyfortimanager-2.3.0/pyfortimanager/models/device_groups.py
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)    11104 2024-03-26 08:29:15.000000 pyfortimanager-2.3.0/pyfortimanager/models/fortiaps.py
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)     6381 2024-02-22 12:29:28.000000 pyfortimanager-2.3.0/pyfortimanager/models/fortiaps_proxy.py
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)     8437 2024-03-27 09:54:37.000000 pyfortimanager-2.3.0/pyfortimanager/models/fortigates.py
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)     7388 2024-02-06 17:05:47.000000 pyfortimanager-2.3.0/pyfortimanager/models/fortigates_proxy.py
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)    11076 2024-02-08 07:45:45.000000 pyfortimanager-2.3.0/pyfortimanager/models/fortiswitches.py
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)     5568 2024-02-22 12:32:18.000000 pyfortimanager-2.3.0/pyfortimanager/models/fortiswitches_proxy.py
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)     2068 2024-02-06 17:05:47.000000 pyfortimanager-2.3.0/pyfortimanager/models/install_wizard.py
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)     6425 2024-02-09 00:17:37.000000 pyfortimanager-2.3.0/pyfortimanager/models/metadata_variables.py
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)    11262 2024-05-27 14:37:24.000000 pyfortimanager-2.3.0/pyfortimanager/models/policy_packages.py
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)     5028 2024-02-06 17:05:47.000000 pyfortimanager-2.3.0/pyfortimanager/models/radius_servers.py
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)     2140 2024-03-18 09:18:05.000000 pyfortimanager-2.3.0/pyfortimanager/models/scripts.py
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)     3061 2024-02-06 17:05:47.000000 pyfortimanager-2.3.0/pyfortimanager/models/sdwan_templates.py
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)     5563 2024-05-27 14:38:10.000000 pyfortimanager-2.3.0/pyfortimanager/models/system.py
+drwxr-xr-x   0 rasmus.thing   (502) staff       (20)        0 2024-05-27 14:45:02.911235 pyfortimanager-2.3.0/pyfortimanager.egg-info/
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)     8882 2024-05-27 14:45:02.000000 pyfortimanager-2.3.0/pyfortimanager.egg-info/PKG-INFO
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)     1030 2024-05-27 14:45:02.000000 pyfortimanager-2.3.0/pyfortimanager.egg-info/SOURCES.txt
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)        1 2024-05-27 14:45:02.000000 pyfortimanager-2.3.0/pyfortimanager.egg-info/dependency_links.txt
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)        1 2024-02-08 21:02:57.000000 pyfortimanager-2.3.0/pyfortimanager.egg-info/not-zip-safe
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)       22 2024-05-27 14:45:02.000000 pyfortimanager-2.3.0/pyfortimanager.egg-info/requires.txt
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)       15 2024-05-27 14:45:02.000000 pyfortimanager-2.3.0/pyfortimanager.egg-info/top_level.txt
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)       38 2024-05-27 14:45:02.911754 pyfortimanager-2.3.0/setup.cfg
+-rw-r--r--   0 rasmus.thing   (502) staff       (20)     1076 2024-05-27 14:44:37.000000 pyfortimanager-2.3.0/setup.py
```

### Comparing `pyfortimanager-2.2.1/LICENSE` & `pyfortimanager-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfortimanager-2.2.1/PKG-INFO` & `pyfortimanager-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pyfortimanager
-Version: 2.2.1
+Version: 2.3.0
 Summary: Python API client library for Fortinet's FortiManager.
 Home-page: https://github.com/BESTSELLER/pyfortimanager
 Author: Rasmus Thing
-Author-email: rasmus.thing@bestseller.com
+Author-email: network@bestseller.com
 License: Apache2
 Keywords: fortinet,fortimanager
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `pyfortimanager-2.2.1/README.md` & `pyfortimanager-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyfortimanager-2.2.1/pyfortimanager/core/api.py` & `pyfortimanager-2.3.0/pyfortimanager/core/api.py`

 * *Files identical despite different names*

### Comparing `pyfortimanager-2.2.1/pyfortimanager/core/fortimanager.py` & `pyfortimanager-2.3.0/pyfortimanager/core/fortimanager.py`

 * *Files identical despite different names*

### Comparing `pyfortimanager-2.2.1/pyfortimanager/models/adoms.py` & `pyfortimanager-2.3.0/pyfortimanager/models/adoms.py`

 * *Files identical despite different names*

### Comparing `pyfortimanager-2.2.1/pyfortimanager/models/cli_template_groups.py` & `pyfortimanager-2.3.0/pyfortimanager/models/cli_template_groups.py`

 * *Files identical despite different names*

### Comparing `pyfortimanager-2.2.1/pyfortimanager/models/device_groups.py` & `pyfortimanager-2.3.0/pyfortimanager/models/device_groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             dict: JSON data.
         """
 
         params = {
             "url": f"/dvmdb/adom/{adom or self.api.adom}/group",
             "option": [
                 "object member"
-            ],
+            ]
         }
 
         # Retrieve a specific device group
         if name:
             params['url'] += f"/{name}"
 
         return self.post(method="get", params=params)
```

### Comparing `pyfortimanager-2.2.1/pyfortimanager/models/fortiaps.py` & `pyfortimanager-2.3.0/pyfortimanager/models/fortiaps.py`

 * *Files identical despite different names*

### Comparing `pyfortimanager-2.2.1/pyfortimanager/models/fortiaps_proxy.py` & `pyfortimanager-2.3.0/pyfortimanager/models/fortiaps_proxy.py`

 * *Files identical despite different names*

### Comparing `pyfortimanager-2.2.1/pyfortimanager/models/fortigates.py` & `pyfortimanager-2.3.0/pyfortimanager/models/fortigates.py`

 * *Files identical despite different names*

### Comparing `pyfortimanager-2.2.1/pyfortimanager/models/fortigates_proxy.py` & `pyfortimanager-2.3.0/pyfortimanager/models/fortigates_proxy.py`

 * *Files identical despite different names*

### Comparing `pyfortimanager-2.2.1/pyfortimanager/models/fortiswitches.py` & `pyfortimanager-2.3.0/pyfortimanager/models/fortiswitches.py`

 * *Files identical despite different names*

### Comparing `pyfortimanager-2.2.1/pyfortimanager/models/fortiswitches_proxy.py` & `pyfortimanager-2.3.0/pyfortimanager/models/fortiswitches_proxy.py`

 * *Files identical despite different names*

### Comparing `pyfortimanager-2.2.1/pyfortimanager/models/install_wizard.py` & `pyfortimanager-2.3.0/pyfortimanager/models/install_wizard.py`

 * *Files identical despite different names*

### Comparing `pyfortimanager-2.2.1/pyfortimanager/models/metadata_variables.py` & `pyfortimanager-2.3.0/pyfortimanager/models/metadata_variables.py`

 * *Files identical despite different names*

### Comparing `pyfortimanager-2.2.1/pyfortimanager/models/policy_packages.py` & `pyfortimanager-2.3.0/pyfortimanager/models/policy_packages.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,7 +300,24 @@
                     "name": fortigate,
                     "vdom": vdom
                 }
             ]
         }
 
         return self.post(method="delete", params=params)
+
+    def firewall_policies(self, name: str, adom: str = None):
+        """Retrieves all firewall policies in a policy package.
+
+        Args:
+            name (str): Name of the policy package.
+            adom (str): Name of the ADOM. Defaults to the ADOM set when the API was instantiated.
+
+        Returns:
+            dict: JSON data.
+        """
+
+        params = {
+            "url": f"/pm/config/adom/{adom or self.api.adom}/pkg/{name}/firewall/policy",
+        }
+
+        return self.post(method="get", params=params)
```

### Comparing `pyfortimanager-2.2.1/pyfortimanager/models/radius_servers.py` & `pyfortimanager-2.3.0/pyfortimanager/models/radius_servers.py`

 * *Files identical despite different names*

### Comparing `pyfortimanager-2.2.1/pyfortimanager/models/scripts.py` & `pyfortimanager-2.3.0/pyfortimanager/models/scripts.py`

 * *Files identical despite different names*

### Comparing `pyfortimanager-2.2.1/pyfortimanager/models/sdwan_templates.py` & `pyfortimanager-2.3.0/pyfortimanager/models/sdwan_templates.py`

 * *Files identical despite different names*

### Comparing `pyfortimanager-2.2.1/pyfortimanager/models/system.py` & `pyfortimanager-2.3.0/pyfortimanager/models/system.py`

 * *Files 10% similar despite different names*

```diff
@@ -117,14 +117,34 @@
 
         params = {
             "url": "/sys/status"
         }
 
         return self.post(method="get", params=params)
 
+    def refresh_hitcount(self, policy_package: str, adom: str = None):
+        """Refreshes the hitcount of firewall policies for a specific policy package in FortiManager.
+
+        Args:
+            policy_package (str): Name of the policy package.
+            adom (str): Name of the ADOM. Defaults to the ADOM set when the API was instantiated.
+
+        Returns:
+            dict: JSON data.
+        """
+
+        params = {
+            "url": "/sys/hitcount",
+            "data": {
+                "adom": adom or self.api.adom,
+                "pkg": policy_package
+            }
+        }
+        return self.post(method="exec", params=params)
+
     def tasks(self, task: int = None, filter: list = None, loadsub: bool = True):
         """Retrieves all FortiManager tasks or a single task.
 
         Args:
             task (int): ID of a specific task.
             filter (list): Filter the result according to a set of criteria. example: List [ "{attribute}", "==", "{value}" ]
             loadsub (bool): Enable or disable the return of any sub-objects. Default is enabled.
@@ -140,7 +160,26 @@
         }
 
         # Retrieve a single task
         if task:
             params['url'] = f"/task/task/{task}/line"
 
         return self.post(method="get", params=params)
+
+    def task_result(self, task: int = None):
+        """Returns the result of a task in FortiManager.
+
+        Args:
+            task (int): ID of the task.
+
+        Returns:
+            dict: JSON data.
+        """
+
+        params = {
+            "url": "/sys/task/result",
+            "data": {
+                "taskid": task
+            }
+        }
+
+        return self.post(method="exec", params=params)
```

### Comparing `pyfortimanager-2.2.1/pyfortimanager.egg-info/PKG-INFO` & `pyfortimanager-2.3.0/pyfortimanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pyfortimanager
-Version: 2.2.1
+Version: 2.3.0
 Summary: Python API client library for Fortinet's FortiManager.
 Home-page: https://github.com/BESTSELLER/pyfortimanager
 Author: Rasmus Thing
-Author-email: rasmus.thing@bestseller.com
+Author-email: network@bestseller.com
 License: Apache2
 Keywords: fortinet,fortimanager
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `pyfortimanager-2.2.1/pyfortimanager.egg-info/SOURCES.txt` & `pyfortimanager-2.3.0/pyfortimanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfortimanager-2.2.1/setup.py` & `pyfortimanager-2.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="pyfortimanager",
-    version="2.2.1",
+    version="2.3.0",
     description="Python API client library for Fortinet's FortiManager.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache2",
     author="Rasmus Thing",
-    author_email="rasmus.thing@bestseller.com",
+    author_email="network@bestseller.com",
     url="https://github.com/BESTSELLER/pyfortimanager",
     python_requires=">=3.8, <4",
     install_requires=[
         "requests>=2.20.0,<3.0"
     ],
     zip_safe=False,
     keywords=[
```

