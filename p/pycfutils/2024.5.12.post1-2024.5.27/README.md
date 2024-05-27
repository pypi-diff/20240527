# Comparing `tmp/pycfutils-2024.5.12.post1.tar.gz` & `tmp/pycfutils-2024.5.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycfutils-2024.5.12.post1.tar", last modified: Sun May 12 11:17:24 2024, max compression
+gzip compressed data, was "pycfutils-2024.5.27.tar", last modified: Mon May 27 16:33:01 2024, max compression
```

## Comparing `pycfutils-2024.5.12.post1.tar` & `pycfutils-2024.5.27.tar`

### file list

```diff
@@ -1,44 +1,53 @@
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 11:17:24.425165 pycfutils-2024.5.12.post1/
--rw-r--r--   0 cfati     (1000) cfati     (1000)     2420 2024-05-11 23:28:42.000000 pycfutils-2024.5.12.post1/CHANGELOG
--rw-r--r--   0 cfati     (1000) cfati     (1000)     1073 2024-05-07 19:43:39.000000 pycfutils-2024.5.12.post1/LICENSE
--rw-r--r--   0 cfati     (1000) cfati     (1000)     1722 2024-05-12 11:17:24.417170 pycfutils-2024.5.12.post1/PKG-INFO
--rw-r--r--   0 cfati     (1000) cfati     (1000)      750 2024-05-12 10:58:11.000000 pycfutils-2024.5.12.post1/README.md
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 11:17:23.841164 pycfutils-2024.5.12.post1/pycfutils/
--rw-r--r--   0 cfati     (1000) cfati     (1000)       75 2024-05-10 09:58:59.000000 pycfutils-2024.5.12.post1/pycfutils/__init__.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)     3107 2024-05-11 23:30:52.000000 pycfutils-2024.5.12.post1/pycfutils/ctypes.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)      266 2024-05-11 23:30:52.000000 pycfutils-2024.5.12.post1/pycfutils/exceptions.py
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 11:17:23.984166 pycfutils-2024.5.12.post1/pycfutils/gstreamer/
--rw-r--r--   0 cfati     (1000) cfati     (1000)      193 2024-05-11 23:30:51.000000 pycfutils-2024.5.12.post1/pycfutils/gstreamer/__init__.py
--rwxr-xr-x   0 cfati     (1000) cfati     (1000)     3437 2024-05-10 09:58:59.000000 pycfutils-2024.5.12.post1/pycfutils/gstreamer/registry_access.py
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 11:17:24.031198 pycfutils-2024.5.12.post1/pycfutils/gui/
--rw-r--r--   0 cfati     (1000) cfati     (1000)     1417 2024-05-10 11:22:36.000000 pycfutils-2024.5.12.post1/pycfutils/gui/__init__.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)     2012 2024-05-11 23:38:42.000000 pycfutils-2024.5.12.post1/pycfutils/gui/constants.py
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 11:17:23.641330 pycfutils-2024.5.12.post1/pycfutils/include/
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 11:17:24.366177 pycfutils-2024.5.12.post1/pycfutils/include/pycfutils/
--rw-r--r--   0 cfati     (1000) cfati     (1000)      921 2024-05-07 23:17:59.000000 pycfutils-2024.5.12.post1/pycfutils/include/pycfutils/cinterface.h
--rwxr-xr-x   0 cfati     (1000) cfati     (1000)     1941 2024-05-11 23:30:52.000000 pycfutils-2024.5.12.post1/pycfutils/keyboard.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)     2057 2024-05-10 11:21:36.000000 pycfutils-2024.5.12.post1/pycfutils/miscellaneous.py
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 11:17:24.394164 pycfutils-2024.5.12.post1/pycfutils/src/
--rw-r--r--   0 cfati     (1000) cfati     (1000)     3553 2024-05-07 23:17:59.000000 pycfutils-2024.5.12.post1/pycfutils/src/cinterface_win.cpp
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 11:17:24.225163 pycfutils-2024.5.12.post1/pycfutils/tests/
--rw-r--r--   0 cfati     (1000) cfati     (1000)       75 2024-05-10 09:58:59.000000 pycfutils-2024.5.12.post1/pycfutils/tests/__init__.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)      775 2024-05-10 09:58:59.000000 pycfutils-2024.5.12.post1/pycfutils/tests/test_ctypes.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)     1273 2024-05-12 09:45:15.000000 pycfutils-2024.5.12.post1/pycfutils/tests/test_gstreamer.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)      354 2024-05-10 09:58:59.000000 pycfutils-2024.5.12.post1/pycfutils/tests/test_gui.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)      367 2024-05-11 23:38:41.000000 pycfutils-2024.5.12.post1/pycfutils/tests/test_keyboard.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)     3756 2024-05-10 12:17:28.000000 pycfutils-2024.5.12.post1/pycfutils/tests/test_miscellaneous.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)       99 2024-05-12 11:15:38.000000 pycfutils-2024.5.12.post1/pycfutils/version.py
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 11:17:23.925164 pycfutils-2024.5.12.post1/pycfutils.egg-info/
--rw-r--r--   0 cfati     (1000) cfati     (1000)     1722 2024-05-12 11:17:23.000000 pycfutils-2024.5.12.post1/pycfutils.egg-info/PKG-INFO
--rw-r--r--   0 cfati     (1000) cfati     (1000)      768 2024-05-12 11:17:23.000000 pycfutils-2024.5.12.post1/pycfutils.egg-info/SOURCES.txt
--rw-r--r--   0 cfati     (1000) cfati     (1000)        1 2024-05-12 11:17:23.000000 pycfutils-2024.5.12.post1/pycfutils.egg-info/dependency_links.txt
--rw-r--r--   0 cfati     (1000) cfati     (1000)       10 2024-05-12 11:17:23.000000 pycfutils-2024.5.12.post1/pycfutils.egg-info/top_level.txt
--rw-r--r--   0 cfati     (1000) cfati     (1000)       38 2024-05-12 11:17:24.427168 pycfutils-2024.5.12.post1/setup.cfg
--rwxr-xr-x   0 cfati     (1000) cfati     (1000)     4875 2024-05-10 14:40:36.000000 pycfutils-2024.5.12.post1/setup.py
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 11:17:24.336172 pycfutils-2024.5.12.post1/utils/
--rwxr-xr-x   0 cfati     (1000) cfati     (1000)     1723 2024-05-11 08:49:26.000000 pycfutils-2024.5.12.post1/utils/nix.sh
--rw-r--r--   0 cfati     (1000) cfati     (1000)     1261 2024-05-12 11:13:17.000000 pycfutils-2024.5.12.post1/utils/win.bat
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 11:17:24.302165 pycfutils-2024.5.12.post1/vs/
--rw-r--r--   0 cfati     (1000) cfati     (1000)     1423 2024-05-07 23:17:59.000000 pycfutils-2024.5.12.post1/vs/vs.sln
--rw-r--r--   0 cfati     (1000) cfati     (1000)     8443 2024-05-07 23:17:59.000000 pycfutils-2024.5.12.post1/vs/vs.vcxproj
--rw-r--r--   0 cfati     (1000) cfati     (1000)     1161 2024-05-07 23:17:59.000000 pycfutils-2024.5.12.post1/vs/vs.vcxproj.filters
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-27 16:33:01.161382 pycfutils-2024.5.27/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     2996 2024-05-27 14:46:47.000000 pycfutils-2024.5.27/CHANGELOG
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     1073 2024-05-07 19:43:39.000000 pycfutils-2024.5.27/LICENSE
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     2298 2024-05-27 16:33:01.153648 pycfutils-2024.5.27/PKG-INFO
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     1332 2024-05-27 15:18:50.000000 pycfutils-2024.5.27/README.md
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-27 16:33:01.057716 pycfutils-2024.5.27/_utils/
+-rwxr-xr-x   0 cfati     (1000) cfati     (1000)     1719 2024-05-26 18:50:14.000000 pycfutils-2024.5.27/_utils/nix.sh
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     1257 2024-05-26 18:52:50.000000 pycfutils-2024.5.27/_utils/win.bat
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-27 16:33:00.446176 pycfutils-2024.5.27/pycfutils/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)       75 2024-05-27 14:43:43.000000 pycfutils-2024.5.27/pycfutils/__init__.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     3107 2024-05-27 06:40:19.000000 pycfutils-2024.5.27/pycfutils/ctypes.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)      339 2024-05-25 18:00:02.000000 pycfutils-2024.5.27/pycfutils/exceptions.py
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-27 16:33:00.577443 pycfutils-2024.5.27/pycfutils/gstreamer/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)      193 2024-05-11 23:30:51.000000 pycfutils-2024.5.27/pycfutils/gstreamer/__init__.py
+-rwxr-xr-x   0 cfati     (1000) cfati     (1000)     3437 2024-05-10 09:58:59.000000 pycfutils-2024.5.27/pycfutils/gstreamer/registry_access.py
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-27 16:33:00.615033 pycfutils-2024.5.27/pycfutils/gui/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     1410 2024-05-24 19:40:44.000000 pycfutils-2024.5.27/pycfutils/gui/__init__.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     2012 2024-05-11 23:38:42.000000 pycfutils-2024.5.27/pycfutils/gui/constants.py
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-27 16:33:00.229997 pycfutils-2024.5.27/pycfutils/include/
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-27 16:33:01.093086 pycfutils-2024.5.27/pycfutils/include/pycfutils/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)      921 2024-05-07 23:17:59.000000 pycfutils-2024.5.27/pycfutils/include/pycfutils/cinterface.h
+-rwxr-xr-x   0 cfati     (1000) cfati     (1000)     1941 2024-05-11 23:30:52.000000 pycfutils-2024.5.27/pycfutils/io.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     1599 2024-05-14 18:58:11.000000 pycfutils-2024.5.27/pycfutils/miscellaneous.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     7583 2024-05-27 00:02:52.000000 pycfutils-2024.5.27/pycfutils/network.py
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-27 16:33:01.127488 pycfutils-2024.5.27/pycfutils/src/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     3905 2024-05-27 14:31:51.000000 pycfutils-2024.5.27/pycfutils/src/cinterface_win.cpp
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     1356 2024-05-26 22:53:51.000000 pycfutils-2024.5.27/pycfutils/system.py
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-27 16:33:00.831260 pycfutils-2024.5.27/pycfutils/tests/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)       75 2024-05-27 14:43:43.000000 pycfutils-2024.5.27/pycfutils/tests/__init__.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)      775 2024-05-10 09:58:59.000000 pycfutils-2024.5.27/pycfutils/tests/test_ctypes.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     1273 2024-05-12 09:45:15.000000 pycfutils-2024.5.27/pycfutils/tests/test_gstreamer.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)      354 2024-05-10 09:58:59.000000 pycfutils-2024.5.27/pycfutils/tests/test_gui.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)      349 2024-05-26 18:53:29.000000 pycfutils-2024.5.27/pycfutils/tests/test_io.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     2779 2024-05-14 16:46:06.000000 pycfutils-2024.5.27/pycfutils/tests/test_miscellaneous.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     7132 2024-05-26 23:16:44.000000 pycfutils-2024.5.27/pycfutils/tests/test_network.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     2124 2024-05-24 19:40:45.000000 pycfutils-2024.5.27/pycfutils/tests/test_system.py
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-27 16:33:00.951432 pycfutils-2024.5.27/pycfutils/tools/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)       75 2024-05-27 14:43:43.000000 pycfutils-2024.5.27/pycfutils/tools/__init__.py
+-rwxr-xr-x   0 cfati     (1000) cfati     (1000)     2050 2024-05-27 07:35:15.000000 pycfutils-2024.5.27/pycfutils/tools/connect_to_server.py
+-rwxr-xr-x   0 cfati     (1000) cfati     (1000)     1398 2024-05-27 14:50:24.000000 pycfutils-2024.5.27/pycfutils/tools/cpu_stress.py
+-rwxr-xr-x   0 cfati     (1000) cfati     (1000)     3813 2024-05-27 14:50:58.000000 pycfutils-2024.5.27/pycfutils/tools/tcp_scan.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)       90 2024-05-27 16:25:25.000000 pycfutils-2024.5.27/pycfutils/version.py
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-27 16:33:00.530569 pycfutils-2024.5.27/pycfutils.egg-info/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     2298 2024-05-27 16:32:59.000000 pycfutils-2024.5.27/pycfutils.egg-info/PKG-INFO
+-rw-r--r--   0 cfati     (1000) cfati     (1000)      985 2024-05-27 16:33:00.000000 pycfutils-2024.5.27/pycfutils.egg-info/SOURCES.txt
+-rw-r--r--   0 cfati     (1000) cfati     (1000)        1 2024-05-27 16:32:59.000000 pycfutils-2024.5.27/pycfutils.egg-info/dependency_links.txt
+-rw-r--r--   0 cfati     (1000) cfati     (1000)       10 2024-05-27 16:32:59.000000 pycfutils-2024.5.27/pycfutils.egg-info/top_level.txt
+-rw-r--r--   0 cfati     (1000) cfati     (1000)       38 2024-05-27 16:33:01.163018 pycfutils-2024.5.27/setup.cfg
+-rwxr-xr-x   0 cfati     (1000) cfati     (1000)     4979 2024-05-27 15:00:13.000000 pycfutils-2024.5.27/setup.py
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-27 16:33:01.015964 pycfutils-2024.5.27/vs/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     1423 2024-05-07 23:17:59.000000 pycfutils-2024.5.27/vs/vs.sln
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     8443 2024-05-07 23:17:59.000000 pycfutils-2024.5.27/vs/vs.vcxproj
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     1161 2024-05-07 23:17:59.000000 pycfutils-2024.5.27/vs/vs.vcxproj.filters
```

### Comparing `pycfutils-2024.5.12.post1/CHANGELOG` & `pycfutils-2024.5.27/CHANGELOG`

 * *Files 8% similar despite different names*

```diff
@@ -41,31 +41,51 @@
 ===============================================================================
 C         H         A         N        G        E         L         O         G
 ===============================================================================
 
 
 [TBR]
 
-[2024.05.10]
+[2024.05.27]
+    - Windows hook mechanism improvement
+      @CristiFati, 240527
+    - Add CLI tools
+      @CristiFati, 240527
+    - Add network functions
+      @CristiFati, 240526
+    - Rename module: keyboard -> io (breaking change)
+      @CristiFati, 240526
+    - Add cpu_stress feature
+      @CristiFati, 240524
+    - Move path_ancestor from miscellaneous to system (breaking change)
+      @CristiFati, 240524
+    - Various fixes and improvements
+      @CristiFati, 240512
+
+[2024.05.12.post1]
+    - Bugfix
+      @CristiFati, #50179a8
+
+[2024.05.12]
     - Test (local) utilities
       @CristiFati, 240510
     - Gstreamer stuff
       @CristiFati, 240510
     - Improve versioning
       @CristiFati, 240510
     - Add function for path ancestor
       @CristiFati, 240510
-    - Rename common.py to miscellaneous.py
+    - Rename common.py to miscellaneous.py (breaking change)
       @CristiFati, 240510
 
-[v2024.05.08.post1]
+[v2024.05.08.post1 (deleted)]
     - Bugfix
       @CristiFati, #7e7114a
 
-[v2024.05.08]
+[v2024.05.08 (deleted)]
     - Build and tests
       @CristiFati, 240508
     - GUI package
       @CristiFati, 240508
     - Reorganize file structure
       @CristiFati, 240508, #678a0613e1e5eecd759bca1f3e13dc388ae45dcb
     - CTypes module (utilities)
```

### Comparing `pycfutils-2024.5.12.post1/LICENSE` & `pycfutils-2024.5.27/LICENSE`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12.post1/PKG-INFO` & `pycfutils-2024.5.27/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycfutils
-Version: 2024.5.12.post1
+Version: 2024.5.27
 Summary: PyCFUtils (Cristi Fati's Utils for Python (&& more)) - a collection of (cool) scripts / utilities
 Home-page: https://github.com/CristiFati/pycfutils
 Download-URL: https://pypi.org/project/pycfutils
 Author: Cristi Fati
 Author-email: fati_utcluj@yahoo.com
 Maintainer: Cristi Fati
 Maintainer-email: fati_utcluj@yahoo.com
@@ -22,41 +22,62 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # *PyCFUtils*
 
-*PyCFUtils* (**C**risti **F**ati's ***Utils*** for ***Py**thon* (&& more)) - a collection of (cool) scripts / utilities
+*PyCFUtils* (**C**risti **F**ati's ***Utils*** for ***Py**thon* (&& more)) - a collection of goodies ((cool) scripts / utilities)
 
 
 ## Install
 
 Use *PIP*:
 
 ```shell
 python -m pip install --upgrade pycfutils
 ```
 
 
 ## Usage example
 
 ```python
+import pycfutils.io
 import pycfutils.miscellaneous as misc
-import pycfutils.keyboard
+import pycfutils.network
+import pycfutils.system
+from pycfutils.exceptions import NetworkException
 
 print("Press a key in less than one second...")
-print(pycfutils.keyboard.read_key(timeout=1))
+print(pycfutils.io.read_key(timeout=1))
 print(misc.timestamp_string(human_readable=True))
+try:
+    print(pycfutils.network.connect_to_server("127.0.0.1", 22))
+except NetworkException as e:
+    print(e)
+pycfutils.system.cpu_stress(3)
 
 # --- Windows only ---
 import pycfutils.gui
 
 print(pycfutils.gui.message_box("Title", "Text to display", x=320, y=200))
 
 # --- Requires PyGObject (also might take some time to complete) ---
 from pycfutils.gstreamer import RegistryAccess
 
 ra = RegistryAccess()
 print(ra.element_classes())
 ```
 
+Also, there are some useful (CLI wrapper) scripts **in the *tools* folder**. 
+
+- *Nix*:
+
+    ```lang-bash
+    for script in $(find "pycfutils/tools" -maxdepth 1 -type f); do python "${script}" -h; done
+    ```
+
+- *Win*:
+
+    ```lang-bat
+    for /f %g in ('dir /b /a-d /a-l "pycfutils\tools\*.py"') do (python "pycfutils\tools\%g" -h)
+    ```
```

### Comparing `pycfutils-2024.5.12.post1/pycfutils/ctypes.py` & `pycfutils-2024.5.27/pycfutils/ctypes.py`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12.post1/pycfutils/gstreamer/registry_access.py` & `pycfutils-2024.5.27/pycfutils/gstreamer/registry_access.py`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12.post1/pycfutils/gui/__init__.py` & `pycfutils-2024.5.27/pycfutils/gui/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import atexit
 import ctypes as cts
 import os
 import sys
 from typing import Optional
 
-from pycfutils.miscellaneous import path_ancestor
+from pycfutils.system import path_ancestor
 
 __all__ = ()
 
 _IS_WIN = sys.platform[:3].lower() == "win"
 _DLL_NAME = os.path.join(
     path_ancestor(os.path.abspath(__file__), level=2),
     f"libcinterface.{'dll' if _IS_WIN else 'so'}",
```

### Comparing `pycfutils-2024.5.12.post1/pycfutils/gui/constants.py` & `pycfutils-2024.5.27/pycfutils/gui/constants.py`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12.post1/pycfutils/include/pycfutils/cinterface.h` & `pycfutils-2024.5.27/pycfutils/include/pycfutils/cinterface.h`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12.post1/pycfutils/keyboard.py` & `pycfutils-2024.5.27/pycfutils/io.py`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12.post1/pycfutils/miscellaneous.py` & `pycfutils-2024.5.27/pycfutils/miscellaneous.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import math
 import sys
 import time
 from datetime import datetime
-from os import PathLike
-from os.path import dirname
-from typing import AnyStr, Sequence, Tuple, Union
+from typing import Sequence, Tuple, Union
 
 __all__ = (
     "dimensions_2d",
     "int_format",
-    "path_ancestor",
     "timestamp_string",
     "uniques",
 )
 
 
 def dimensions_2d(n: int) -> Tuple:
     if n <= 0:
@@ -23,29 +20,14 @@
 
 
 def int_format(limit: int) -> str:
     sgn = 1 if limit < 0 else 0
     return f"{{:0{math.ceil(math.log10(max(abs(limit), 2))) + sgn:d}d}}"
 
 
-# pathlib.Path.parents equivalent
-def path_ancestor(path: Union[PathLike, AnyStr], level: int = 1) -> AnyStr:
-    pass
-    if level <= 0:
-        return path if isinstance(path, (str, bytes)) else str(path)
-    ret = dirname(path)
-    while level > 1:
-        path = ret
-        ret = dirname(path)
-        if ret == path:
-            break
-        level -= 1
-    return ret
-
-
 def timestamp_string(
     timestamp: Union[None, int, float, Sequence] = None,
     human_readable: bool = False,
     date_separator: str = "-",
     time_separator: str = ":",
     separator: str = " ",
 ) -> str:
```

### Comparing `pycfutils-2024.5.12.post1/pycfutils/src/cinterface_win.cpp` & `pycfutils-2024.5.27/pycfutils/src/cinterface_win.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 #include <unordered_map>
 #include <utility>
-#include <vector>
 
 #include <Windows.h>
 
 #define LIBCINTERFACE_EXPORTS
 #include "../include/pycfutils/cinterface.h"
 
 #define SENTINEL 0x80000000
 
 
 typedef std::unordered_map<DWORD, HHOOK> HookData;
 typedef std::pair<int, int> XY;
-typedef std::unordered_map<DWORD, std::vector<XY>> XYData;
+typedef std::unordered_map<DWORD, XY> XYData;
 
 CRITICAL_SECTION criticalSection;
 XYData xyData;
 HookData hookData;
 
 
 static LRESULT CALLBACK _hookFunc(int nCode, WPARAM wParam, LPARAM lParam)
@@ -24,30 +23,34 @@
     if (nCode < 0) {
         return CallNextHookEx(NULL, nCode, wParam, lParam);
     }
     switch (nCode) {
         case HCBT_CREATEWND: {
             EnterCriticalSection(&criticalSection);
             DWORD tid = GetCurrentThreadId();
-            if (hookData.find(tid) != hookData.cend()) {
-                auto xyIt = xyData[tid].cbegin();
-                if (xyIt != xyData[tid].cend()) {
+            HookData::const_iterator hIt = hookData.find(tid);
+            if (hIt != hookData.cend()) {
+                XYData::const_iterator xyIt = xyData.find(tid);
+                if (xyIt != xyData.cend()) {
                     LPCBT_CREATEWNDW pcw = (LPCBT_CREATEWNDW)lParam;
                     if (pcw) {
                         LPCREATESTRUCTW pcs = pcw->lpcs;
                         if (pcs) {
-                            if (xyIt->first != SENTINEL) {
-                                pcs->x = xyIt->first;
+                            if (xyIt->second.first != SENTINEL) {
+                                pcs->x = xyIt->second.first;
                             }
-                            if (xyIt->second != SENTINEL) {
-                                pcs->y = xyIt->second;
+                            if (xyIt->second.second != SENTINEL) {
+                                pcs->y = xyIt->second.second;
                             }
                         }
                     }
-                    xyData[tid].erase(xyIt);
+                    xyData.erase(xyIt);
+                }
+                if (UnhookWindowsHookEx(hIt->second)) {  // @TODO - cfati: Unhook from within hook
+                    hookData.erase(hIt);
                 }
             }
             LeaveCriticalSection(&criticalSection);
             break;
         }
         default: {
             break;
@@ -56,23 +59,31 @@
     return CallNextHookEx(NULL, nCode, wParam, lParam);
 }
 
 int MessageBoxXY(HWND hWnd, LPCWSTR lpText, LPCWSTR lpCaption, UINT uType, int x, int y)
 {
     EnterCriticalSection(&criticalSection);
     DWORD tid = GetCurrentThreadId();
+    int err = 0;
     if (hookData.find(tid) == hookData.cend()) {
         HHOOK hook = SetWindowsHookExW(WH_CBT, _hookFunc, 0, tid);
         if (hook) {
-            hookData[tid] = hook;
-        }  // @TODO - cfati: Silently fail?
+            hookData.emplace(std::make_pair(tid, hook));
+        }
+        else {
+            err = GetLastError();
+        }
+    } else {
+        err = -1;
+    }
+    if (!err) {
+        xyData.emplace(std::make_pair(tid, std::make_pair(x, y)));
     }
-    xyData[tid].emplace_back(std::make_pair(x, y));
     LeaveCriticalSection(&criticalSection);
-    return MessageBoxW(hWnd, lpText, lpCaption, uType);
+    return err ? err : MessageBoxW(hWnd, lpText, lpCaption, uType);
 }
 
 
 int clearHooks()
 {
     int ret = 0;
     EnterCriticalSection(&criticalSection);
```

### Comparing `pycfutils-2024.5.12.post1/pycfutils/tests/test_ctypes.py` & `pycfutils-2024.5.27/pycfutils/tests/test_ctypes.py`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12.post1/pycfutils/tests/test_gstreamer.py` & `pycfutils-2024.5.27/pycfutils/tests/test_gstreamer.py`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12.post1/pycfutils/tests/test_miscellaneous.py` & `pycfutils-2024.5.27/pycfutils/tests/test_miscellaneous.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,14 @@
-import os
-import pathlib
 import unittest
 from datetime import datetime
 
 from pycfutils import miscellaneous
 
 
 class MiscellaneousTestCase(unittest.TestCase):
-    def setUp(self):
-        self.cd = os.getcwd()
-        self.cds = (self.cd, self.cd.encode(), pathlib.Path(self.cd))
-
     def test_dimensions_2d(self):
         self.assertEqual(miscellaneous.dimensions_2d(-3), (0, 0))
         self.assertEqual(miscellaneous.dimensions_2d(0), (0, 0))
         self.assertEqual(miscellaneous.dimensions_2d(1), (1, 1))
         self.assertEqual(miscellaneous.dimensions_2d(2), (1, 2))
         self.assertEqual(miscellaneous.dimensions_2d(3), (2, 2))
         self.assertEqual(miscellaneous.dimensions_2d(4), (2, 2))
@@ -36,33 +30,14 @@
         self.assertEqual(miscellaneous.int_format(0), "{:01d}")
         self.assertEqual(miscellaneous.int_format(1), "{:01d}")
         self.assertEqual(miscellaneous.int_format(10), "{:01d}")
         self.assertEqual(miscellaneous.int_format(11), "{:02d}")
         self.assertEqual(miscellaneous.int_format(100), "{:02d}")
         self.assertEqual(miscellaneous.int_format(101), "{:03d}")
 
-    def test_path_ancestor(self):
-        for cd in self.cds:
-            self.assertEqual(
-                miscellaneous.path_ancestor(cd, level=1), os.path.dirname(cd)
-            )
-        self.assertEqual(miscellaneous.path_ancestor(self.cd, 0), self.cd)
-        self.assertEqual(miscellaneous.path_ancestor(""), "")
-        self.assertEqual(miscellaneous.path_ancestor(os.path.sep, level=3), os.path.sep)
-        idx = self.cd.rfind(os.path.sep)
-        level = 1
-        while True:
-            part = self.cd[:idx]
-            # print(idx, part, level, miscellaneous.path_ancestor(self.cd, level))
-            if os.path.dirname(part) == part:
-                break
-            self.assertEqual(miscellaneous.path_ancestor(self.cd, level), part)
-            level += 1
-            idx = self.cd.rfind(os.path.sep, 0, idx)
-
     def test_timestamp_string(self):
         ts = (2024, 5, 6, 12, 34, 56)
         self.assertEqual(
             miscellaneous.timestamp_string(timestamp=ts, human_readable=False),
             "20240506123456",
         )
         self.assertEqual(
```

### Comparing `pycfutils-2024.5.12.post1/pycfutils.egg-info/PKG-INFO` & `pycfutils-2024.5.27/pycfutils.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycfutils
-Version: 2024.5.12.post1
+Version: 2024.5.27
 Summary: PyCFUtils (Cristi Fati's Utils for Python (&& more)) - a collection of (cool) scripts / utilities
 Home-page: https://github.com/CristiFati/pycfutils
 Download-URL: https://pypi.org/project/pycfutils
 Author: Cristi Fati
 Author-email: fati_utcluj@yahoo.com
 Maintainer: Cristi Fati
 Maintainer-email: fati_utcluj@yahoo.com
@@ -22,41 +22,62 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # *PyCFUtils*
 
-*PyCFUtils* (**C**risti **F**ati's ***Utils*** for ***Py**thon* (&& more)) - a collection of (cool) scripts / utilities
+*PyCFUtils* (**C**risti **F**ati's ***Utils*** for ***Py**thon* (&& more)) - a collection of goodies ((cool) scripts / utilities)
 
 
 ## Install
 
 Use *PIP*:
 
 ```shell
 python -m pip install --upgrade pycfutils
 ```
 
 
 ## Usage example
 
 ```python
+import pycfutils.io
 import pycfutils.miscellaneous as misc
-import pycfutils.keyboard
+import pycfutils.network
+import pycfutils.system
+from pycfutils.exceptions import NetworkException
 
 print("Press a key in less than one second...")
-print(pycfutils.keyboard.read_key(timeout=1))
+print(pycfutils.io.read_key(timeout=1))
 print(misc.timestamp_string(human_readable=True))
+try:
+    print(pycfutils.network.connect_to_server("127.0.0.1", 22))
+except NetworkException as e:
+    print(e)
+pycfutils.system.cpu_stress(3)
 
 # --- Windows only ---
 import pycfutils.gui
 
 print(pycfutils.gui.message_box("Title", "Text to display", x=320, y=200))
 
 # --- Requires PyGObject (also might take some time to complete) ---
 from pycfutils.gstreamer import RegistryAccess
 
 ra = RegistryAccess()
 print(ra.element_classes())
 ```
 
+Also, there are some useful (CLI wrapper) scripts **in the *tools* folder**. 
+
+- *Nix*:
+
+    ```lang-bash
+    for script in $(find "pycfutils/tools" -maxdepth 1 -type f); do python "${script}" -h; done
+    ```
+
+- *Win*:
+
+    ```lang-bat
+    for /f %g in ('dir /b /a-d /a-l "pycfutils\tools\*.py"') do (python "pycfutils\tools\%g" -h)
+    ```
```

### Comparing `pycfutils-2024.5.12.post1/pycfutils.egg-info/SOURCES.txt` & `pycfutils-2024.5.27/pycfutils.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 LICENSE
 README.md
 setup.py
 pycfutils/__init__.py
 pycfutils/ctypes.py
 pycfutils/exceptions.py
-pycfutils/keyboard.py
+pycfutils/io.py
 pycfutils/miscellaneous.py
+pycfutils/network.py
+pycfutils/system.py
 pycfutils/version.py
 pycfutils.egg-info/PKG-INFO
 pycfutils.egg-info/SOURCES.txt
 pycfutils.egg-info/dependency_links.txt
 pycfutils.egg-info/top_level.txt
 pycfutils/gstreamer/__init__.py
 pycfutils/gstreamer/registry_access.py
 pycfutils/gui/__init__.py
 pycfutils/gui/constants.py
 pycfutils/tests/__init__.py
 pycfutils/tests/test_ctypes.py
 pycfutils/tests/test_gstreamer.py
 pycfutils/tests/test_gui.py
-pycfutils/tests/test_keyboard.py
+pycfutils/tests/test_io.py
 pycfutils/tests/test_miscellaneous.py
+pycfutils/tests/test_network.py
+pycfutils/tests/test_system.py
+pycfutils/tools/__init__.py
+pycfutils/tools/connect_to_server.py
+pycfutils/tools/cpu_stress.py
+pycfutils/tools/tcp_scan.py
 CHANGELOG
 vs/vs.vcxproj
 vs/vs.vcxproj.filters
 vs/vs.sln
-utils/nix.sh
-utils/win.bat
+_utils/nix.sh
+_utils/win.bat
 pycfutils/include/pycfutils/cinterface.h
 pycfutils/src/cinterface_win.cpp
```

### Comparing `pycfutils-2024.5.12.post1/setup.py` & `pycfutils-2024.5.27/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 # @TODO - cfati (gainarie): Manually add files in the source distribution (built on Nix)
 class SDist(sdist):
     @staticmethod
     def _extra_files():
         ret = ["CHANGELOG"]
         ret.extend(_VS_FILES)
-        ret.extend((os.path.join("utils", e) for e in ("nix.sh", "win.bat")))
+        ret.extend((os.path.join("_utils", e) for e in ("nix.sh", "win.bat")))
         if _IS_WIN:
             return ret
         ret.extend((os.path.join(_NAME, e) for e in _INCLUDE_FILES))
         ret.extend(_SOURCE_FILES)
         return ret
 
     def _adjust_sources(self):
@@ -144,20 +144,28 @@
         "Operating System :: Unix",
         "Programming Language :: C",
         "Programming Language :: C++",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Software Development",
     ],
-    platforms=("All",),
+    platforms=[
+        "All",
+    ],
     license="MIT",
     url=f"https://github.com/CristiFati/{_NAME}",
     download_url=f"https://pypi.org/project/{_NAME}",
     packages=find_packages(
-        include=(f"{_NAME}", f"{_NAME}.gstreamer", f"{_NAME}.gui", f"{_NAME}.tests"),
+        include=(
+            f"{_NAME}",
+            f"{_NAME}.gstreamer",
+            f"{_NAME}.gui",
+            f"{_NAME}.tests",
+            f"{_NAME}.tools",
+        ),
         exclude=("src", "__pycache__"),
     ),
     package_data={
         f"{_NAME}": _INCLUDE_FILES if _IS_WIN else (),
     },
     cmdclass={
         "build_ext": BuildDll,
```

### Comparing `pycfutils-2024.5.12.post1/utils/nix.sh` & `pycfutils-2024.5.27/_utils/nix.sh`

 * *Files 2% similar despite different names*

```diff
@@ -34,13 +34,13 @@
     for _venv in $(ls -d ${TEST_VENV_PATTERN}); do
         printf -- "Using environment: %s\n" ${_venv}
          . "${_venv}/bin/activate"
         python -VV
         python -m pip uninstall -y pycfutils
         python -m pip -v install --no-index -f "${TEST_WHEEL_DIR}" pycfutils
         python -m unittest discover -s "${VIRTUAL_ENV}/lib/python$(python -c "import sys;print(f'{sys.version_info.major}.{sys.version_info.minor}')")/site-packages/pycfutils/tests"
-        python -c "import pycfutils.gui as pg, pycfutils.keyboard as pk;print('Press a key: ', pk.read_key(1))"
+        python -c "import pycfutils.gui as pg, pycfutils.io as pio;print('Press a key: ', pio.read_key(1))"
         python -m pip uninstall -y pycfutils
         deactivate
     done
     export PYTHONPATH=${_PYTHONPATH}
 fi
```

### Comparing `pycfutils-2024.5.12.post1/utils/win.bat` & `pycfutils-2024.5.27/_utils/win.bat`

 * *Files 12% similar despite different names*

```diff
@@ -22,13 +22,13 @@
     for /f %%g in ('dir /b %TEST_VENV_PATTERN:"=%') do (
         echo Using environment: "%_VENVS_DIR%\%%g"
         call "%_VENVS_DIR%\%%g\Scripts\activate.bat"
         python -VV
         python -m pip uninstall -y pycfutils
         python -m pip -v install --no-index -f %TEST_WHEEL_DIR% pycfutils
         python -m unittest discover -s "%_VENVS_DIR%\%%g\Lib\site-packages\pycfutils\tests"
-        python -c "import sys, pycfutils.gui as pg, pycfutils.keyboard as pk;print('Press a key: ', pk.read_key(1));print(pg.message_box('MBox', sys.version, 200, 200))"
+        python -c "import sys, pycfutils.gui as pg, pycfutils.io as pio;print('Press a key: ', pio.read_key(1));print(pg.message_box('MBox', sys.version, 320, 200))"
         python -m pip uninstall -y pycfutils
         call deactivate
     )
     goto :eof
```

### Comparing `pycfutils-2024.5.12.post1/vs/vs.sln` & `pycfutils-2024.5.27/vs/vs.sln`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12.post1/vs/vs.vcxproj` & `pycfutils-2024.5.27/vs/vs.vcxproj`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12.post1/vs/vs.vcxproj.filters` & `pycfutils-2024.5.27/vs/vs.vcxproj.filters`

 * *Files identical despite different names*

