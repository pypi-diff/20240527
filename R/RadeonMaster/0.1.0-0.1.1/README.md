# Comparing `tmp/RadeonMaster-0.1.0.tar.gz` & `tmp/radeonmaster-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RadeonMaster-0.1.0.tar", last modified: Sun May 26 17:39:41 2024, max compression
+gzip compressed data, was "radeonmaster-0.1.1.tar", last modified: Mon May 27 18:17:51 2024, max compression
```

## Comparing `RadeonMaster-0.1.0.tar` & `radeonmaster-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 vicky     (1000) vicky     (1000)        0 2024-05-26 17:39:41.159977 RadeonMaster-0.1.0/
--rw-r--r--   0 vicky     (1000) vicky     (1000)     1068 2024-05-26 15:57:57.000000 RadeonMaster-0.1.0/LICENSE
--rw-r--r--   0 vicky     (1000) vicky     (1000)    20103 2024-05-26 17:39:41.159977 RadeonMaster-0.1.0/PKG-INFO
--rw-r--r--   0 vicky     (1000) vicky     (1000)    19601 2024-05-26 16:05:44.000000 RadeonMaster-0.1.0/README.md
-drwxr-xr-x   0 vicky     (1000) vicky     (1000)        0 2024-05-26 17:39:41.159977 RadeonMaster-0.1.0/RadeonMaster.egg-info/
--rw-r--r--   0 vicky     (1000) vicky     (1000)    20103 2024-05-26 17:39:41.000000 RadeonMaster-0.1.0/RadeonMaster.egg-info/PKG-INFO
--rw-r--r--   0 vicky     (1000) vicky     (1000)      186 2024-05-26 17:39:41.000000 RadeonMaster-0.1.0/RadeonMaster.egg-info/SOURCES.txt
--rw-r--r--   0 vicky     (1000) vicky     (1000)        1 2024-05-26 17:39:41.000000 RadeonMaster-0.1.0/RadeonMaster.egg-info/dependency_links.txt
--rw-r--r--   0 vicky     (1000) vicky     (1000)       13 2024-05-26 17:39:41.000000 RadeonMaster-0.1.0/RadeonMaster.egg-info/top_level.txt
--rw-rw-rw-   0 vicky     (1000) vicky     (1000)     7451 2024-05-26 15:47:56.000000 RadeonMaster-0.1.0/RadeonMaster.py
--rw-r--r--   0 vicky     (1000) vicky     (1000)       38 2024-05-26 17:39:41.159977 RadeonMaster-0.1.0/setup.cfg
--rw-r--r--   0 vicky     (1000) vicky     (1000)     1313 2024-05-26 17:39:24.000000 RadeonMaster-0.1.0/setup.py
+drwxr-xr-x   0 vicky     (1000) vicky     (1000)        0 2024-05-27 18:17:51.067007 radeonmaster-0.1.1/
+-rw-r--r--   0 vicky     (1000) vicky     (1000)     1068 2024-05-26 15:57:57.000000 radeonmaster-0.1.1/LICENSE
+-rw-r--r--   0 vicky     (1000) vicky     (1000)    20103 2024-05-27 18:17:51.067007 radeonmaster-0.1.1/PKG-INFO
+-rw-r--r--   0 vicky     (1000) vicky     (1000)    19601 2024-05-26 16:05:44.000000 radeonmaster-0.1.1/README.md
+drwxr-xr-x   0 vicky     (1000) vicky     (1000)        0 2024-05-27 18:17:51.067007 radeonmaster-0.1.1/RadeonMaster.egg-info/
+-rw-r--r--   0 vicky     (1000) vicky     (1000)    20103 2024-05-27 18:17:51.000000 radeonmaster-0.1.1/RadeonMaster.egg-info/PKG-INFO
+-rw-r--r--   0 vicky     (1000) vicky     (1000)      186 2024-05-27 18:17:51.000000 radeonmaster-0.1.1/RadeonMaster.egg-info/SOURCES.txt
+-rw-r--r--   0 vicky     (1000) vicky     (1000)        1 2024-05-27 18:17:51.000000 radeonmaster-0.1.1/RadeonMaster.egg-info/dependency_links.txt
+-rw-r--r--   0 vicky     (1000) vicky     (1000)       13 2024-05-27 18:17:51.000000 radeonmaster-0.1.1/RadeonMaster.egg-info/top_level.txt
+-rw-rw-rw-   0 vicky     (1000) vicky     (1000)     7828 2024-05-27 14:33:38.000000 radeonmaster-0.1.1/RadeonMaster.py
+-rw-r--r--   0 vicky     (1000) vicky     (1000)       38 2024-05-27 18:17:51.067007 radeonmaster-0.1.1/setup.cfg
+-rw-r--r--   0 vicky     (1000) vicky     (1000)      744 2024-05-27 18:17:24.000000 radeonmaster-0.1.1/setup.py
```

### Comparing `RadeonMaster-0.1.0/LICENSE` & `radeonmaster-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `RadeonMaster-0.1.0/PKG-INFO` & `radeonmaster-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RadeonMaster
-Version: 0.1.0
+Version: 0.1.1
 Summary: Radeon monitor for python
 Home-page: https://github.com/MegalosVigneswaran/RadeonMaster
 Author: Vigneswaran S
 Author-email: contactmevigneswaran@gmail.com
 Keywords: radeon gpu amd monitor linux radeontop
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RadeonMaster-0.1.0/README.md` & `radeonmaster-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `RadeonMaster-0.1.0/RadeonMaster.egg-info/PKG-INFO` & `radeonmaster-0.1.1/RadeonMaster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RadeonMaster
-Version: 0.1.0
+Version: 0.1.1
 Summary: Radeon monitor for python
 Home-page: https://github.com/MegalosVigneswaran/RadeonMaster
 Author: Vigneswaran S
 Author-email: contactmevigneswaran@gmail.com
 Keywords: radeon gpu amd monitor linux radeontop
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RadeonMaster-0.1.0/RadeonMaster.py` & `radeonmaster-0.1.1/RadeonMaster.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 - Allows querying of GPU data by bus ID.
 
 Use Cases:
 This package is ideal for developers and system administrators who need to monitor and analyze the performance and thermal characteristics of AMD GPUs in their systems.
 """
 
 import os
+import sys
 import json
 import signal
 import threading
 import subprocess as s
 from time import sleep
 
-
 """
 k2w is a dictionary that have the key and full form for the radeontop output
 """
 k2w = { "bus":"bus",
         "gpu":"GPU usage" , 
         "ee" :"Event Engine" , 
         "vgt" :"Vertex Grouper + Tesselator" , 
@@ -113,15 +113,21 @@
         self.get_avai_gpu()
 
         ''' Start the thread and wait for 1 second to get radeontop . 
             This will stop being get wrong output'''
 
         threading.Thread(target=self.strl).start() 
         sleep(1)
-
+    def check_dependencies():
+        if not sys.platform.startswith('Linux'):
+            raise RuntimeError("This module developed for Linux only!")
+        if s.getoutput("command -v radeontop") == '':
+            raise RuntimeError("`radeontop` not found!")
+        elif s.getoutput("command -v sensors"):
+            raise RuntimeError("`lm-sensors` not found!")
     def stop_logging(self):
 
         self.out = False
         
         pid = s.check_output("pgrep radeontop",shell=True).decode("utf-8")
 
         os.kill(int(pid),signal.SIGKILL)
```

