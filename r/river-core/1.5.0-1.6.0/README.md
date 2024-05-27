# Comparing `tmp/river_core-1.5.0.tar.gz` & `tmp/river_core-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/river_core-1.5.0.tar", last modified: Wed May  8 12:37:59 2024, max compression
+gzip compressed data, was "dist/river_core-1.6.0.tar", last modified: Mon May 27 16:57:57 2024, max compression
```

## Comparing `river_core-1.5.0.tar` & `river_core-1.6.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:59.000000 river_core-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-08 12:37:47.000000 river_core-1.5.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-08 12:37:47.000000 river_core-1.5.0/LICENSE.incore
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-08 12:37:47.000000 river_core-1.5.0/LICENSE.tessolve
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-08 12:37:47.000000 river_core-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-08 12:37:59.000000 river_core-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-08 12:37:47.000000 river_core-1.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:59.000000 river_core-1.5.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-08 12:37:47.000000 river_core-1.5.0/examples/sample-config.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:59.000000 river_core-1.5.0/river_core/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    42989 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/rivercore.py
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/sim_hookspecs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:59.000000 river_core-1.5.0/river_core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/coverage_report.html
--rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/report.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:59.000000 river_core-1.5.0/river_core/templates/setup/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:59.000000 river_core-1.5.0/river_core/templates/setup/dut/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/dut/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:59.000000 river_core-1.5.0/river_core/templates/setup/dut/boot/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/dut/boot/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/dut/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/dut/gen_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/dut/sample_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:59.000000 river_core-1.5.0/river_core/templates/setup/generator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/generator/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/generator/gen_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/generator/sample_gen_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/generator/sample_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:59.000000 river_core-1.5.0/river_core/templates/setup/reference/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/reference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/reference/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/reference/gen_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/reference/sample_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/style.css
--rw-r--r--   0 runner    (1001) docker     (127)    18760 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:59.000000 river_core-1.5.0/river_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-08 12:37:58.000000 river_core-1.5.0/river_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-08 12:37:59.000000 river_core-1.5.0/river_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:37:58.000000 river_core-1.5.0/river_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 12:37:58.000000 river_core-1.5.0/river_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:37:58.000000 river_core-1.5.0/river_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-08 12:37:58.000000 river_core-1.5.0/river_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 12:37:58.000000 river_core-1.5.0/river_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-08 12:37:59.000000 river_core-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-08 12:37:47.000000 river_core-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:57.000000 river_core-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-27 16:57:42.000000 river_core-1.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-27 16:57:42.000000 river_core-1.6.0/LICENSE.incore
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-27 16:57:42.000000 river_core-1.6.0/LICENSE.tessolve
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-27 16:57:42.000000 river_core-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-27 16:57:57.000000 river_core-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-27 16:57:42.000000 river_core-1.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:57.000000 river_core-1.6.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-27 16:57:42.000000 river_core-1.6.0/examples/sample-config.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    42985 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/rivercore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/sim_hookspecs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/coverage_report.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/report.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core/templates/setup/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core/templates/setup/dut/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/dut/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core/templates/setup/dut/boot/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/dut/boot/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/dut/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/dut/gen_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/dut/sample_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core/templates/setup/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/generator/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/generator/gen_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/generator/sample_gen_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/generator/sample_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core/templates/setup/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/reference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/reference/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/reference/gen_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/setup/reference/sample_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/templates/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)    20706 2024-05-27 16:57:42.000000 river_core-1.6.0/river_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 16:57:57.000000 river_core-1.6.0/river_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-27 16:57:57.000000 river_core-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-27 16:57:42.000000 river_core-1.6.0/setup.py
```

### Comparing `river_core-1.5.0/CONTRIBUTING.rst` & `river_core-1.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `river_core-1.5.0/LICENSE.incore` & `river_core-1.6.0/LICENSE.incore`

 * *Files identical despite different names*

### Comparing `river_core-1.5.0/LICENSE.tessolve` & `river_core-1.6.0/LICENSE.tessolve`

 * *Files identical despite different names*

### Comparing `river_core-1.5.0/PKG-INFO` & `river_core-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: river_core
-Version: 1.5.0
+Version: 1.6.0
 Summary: RiVer Core Verification Framework
 Home-page: https://github.com/incoresemi/river_core
 Author: InCore Semiconductors Pvt. Ltd.; Tessolve
 Author-email: neelgala@incoresemi.com
 License: BSD-3-Clause
 Description: **RiVer Core** : RISC-V Core Verification Framework 
         ###################################################################################
```

### Comparing `river_core-1.5.0/examples/sample-config.ini` & `river_core-1.6.0/examples/sample-config.ini`

 * *Files identical despite different names*

### Comparing `river_core-1.5.0/river_core/constants.py` & `river_core-1.6.0/river_core/constants.py`

 * *Files identical despite different names*

### Comparing `river_core-1.5.0/river_core/log.py` & `river_core-1.6.0/river_core/log.py`

 * *Files identical despite different names*

### Comparing `river_core-1.5.0/river_core/main.py` & `river_core-1.6.0/river_core/main.py`

 * *Files identical despite different names*

### Comparing `river_core-1.5.0/river_core/rivercore.py` & `river_core-1.6.0/river_core/rivercore.py`

 * *Files 1% similar despite different names*

```diff
@@ -637,15 +637,15 @@
                       continue
                   if not os.path.isfile(test_wd + '/ref.dump'):
                       logger.error(f'{test:<30} : REF dump is missing')
                       test_dict[test]['result'] = 'Unavailable'
                       test_dict[test]['log'] = "REF dump is missing"
                       success = False
                       continue
-                  result, log, insnsize = utils.compare_signature(test_wd + '/dut.dump', test_wd + '/ref.dump')
+                  result, log, insnsize = utils.compare_dumps(test_wd + '/dut.dump', test_wd + '/ref.dump')
                 else:
                   if not os.path.isfile(test_wd + '/dut.signature'):
                       logger.error(f'{test:<30} : DUT signature is missing')
                       test_dict[test]['result'] = 'Unavailable'
                       test_dict[test]['log'] = "DUT signature is missing"
                       success = False
                       continue
```

### Comparing `river_core-1.5.0/river_core/sim_hookspecs.py` & `river_core-1.6.0/river_core/sim_hookspecs.py`

 * *Files identical despite different names*

### Comparing `river_core-1.5.0/river_core/templates/coverage_report.html` & `river_core-1.6.0/river_core/templates/coverage_report.html`

 * *Files identical despite different names*

### Comparing `river_core-1.5.0/river_core/templates/report.html` & `river_core-1.6.0/river_core/templates/report.html`

 * *Files identical despite different names*

### Comparing `river_core-1.5.0/river_core/templates/setup/dut/gen_framework.py` & `river_core-1.6.0/river_core/templates/setup/dut/gen_framework.py`

 * *Files identical despite different names*

### Comparing `river_core-1.5.0/river_core/templates/setup/dut/sample_plugin.py` & `river_core-1.6.0/river_core/templates/setup/dut/sample_plugin.py`

 * *Files identical despite different names*

### Comparing `river_core-1.5.0/river_core/templates/setup/generator/gen_framework.py` & `river_core-1.6.0/river_core/templates/setup/generator/gen_framework.py`

 * *Files identical despite different names*

### Comparing `river_core-1.5.0/river_core/templates/setup/generator/sample_plugin.py` & `river_core-1.6.0/river_core/templates/setup/generator/sample_plugin.py`

 * *Files identical despite different names*

### Comparing `river_core-1.5.0/river_core/templates/setup/reference/gen_framework.py` & `river_core-1.6.0/river_core/templates/setup/reference/gen_framework.py`

 * *Files identical despite different names*

### Comparing `river_core-1.5.0/river_core/templates/setup/reference/sample_plugin.py` & `river_core-1.6.0/river_core/templates/setup/reference/sample_plugin.py`

 * *Files identical despite different names*

### Comparing `river_core-1.5.0/river_core/templates/style.css` & `river_core-1.6.0/river_core/templates/style.css`

 * *Files identical despite different names*

### Comparing `river_core-1.5.0/river_core/utils.py` & `river_core-1.6.0/river_core/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 from river_core.log import logger
 import distutils.util
 import ruamel
 import signal
 from ruamel.yaml import YAML
 from threading import Timer
 import pathlib
-import difflib
 import shlex
 import riscv_config.isa_validator as isa_val
+import re
+
+dump_regex = re.compile(r'.*core\s*(?P<coreid>\d):\s*(?P<priv>\d)\s*(?P<pc>.*?)\s+\((?P<instr>.*?)\)(?P<change>.*?)$')
 
 yaml = YAML(typ="safe")
 yaml.default_flow_style = False
 yaml.allow_unicode = True
 
 def self_check(file1):
   '''
@@ -38,69 +40,120 @@
     '''
     Function to give the number of lines
     '''
     with open(f'{file}','r') as fd:
       rcount = len(fd.readlines())
     return rcount
 
-def compare_signature(file1, file2):
+def compare_dumps(file1, file2):
     '''
-        Function to check whether two signature files are equivalent. This funcion uses the
-        :py:mod:`difflib` to perform the comparision and obtain the difference.
+        Function to check whether two dump files are equivalent. This funcion ucore\s*(?P<coreid>\d):\s*(?P<priv>\d)\s*(?P<pc>.*?)\s+\((?P<instr>.*?)\)(?P<change>.*?)$ses the
         :param file1: The path to the first signature.
         :param file2: The path to the second signature.
         :type file1: str
         :type file2: str
         :return: A string indicating whether the test "Passed" (if files are the same)
             or "Failed" (if the files are different) and the diff of the files.
     '''
     if not os.path.exists(file1) :
         logger.error('Signature file : ' + file1 + ' does not exist')
         raise SystemExit(1)
     cmd = f'diff -iw {file1} {file2}'
     errcode, rout, rerr = sys_command(cmd, logging=False)
+
     if errcode != 0:
-        status = 'Failed'
+
+        rout += '\nMismatch infos:'
+
+        # initial status
+        status = 'Passed'
+
+        # get lines that start with < or >
+        mismatch_str_lst = list(filter(lambda x: x[0] in ['<', '>'], rout.split('\n')))
+
+        # for each mismatched strings
+        start_val = -1
+        for i in range(len(mismatch_str_lst)):
+            
+            file1_str = mismatch_str_lst[i]
+            if file1_str[0] != '<':
+                continue
+            
+            for j in range(start_val + 1, len(mismatch_str_lst)):
+                
+                file2_str = mismatch_str_lst[j] 
+                if file2_str[0] != '>':
+                    continue
+                else:
+                    start_val = j
+
+                # get regex strings
+                try:
+                    file1_dat = dump_regex.findall(file1_str)[0]
+                    file2_dat = dump_regex.findall(file2_str)[0]
+                except IndexError:
+                    status = 'Failed'
+                    break
+
+                # ensure commit message exists in same line number else fail
+                # if any of coreid, priv, pc or instr encoding fails, the diff has failed
+                if file1_dat[0:3] != file2_dat[0:3]:
+                    rout = rout + f'\nBM: {file1} at PC: {file1_dat[2]} and {file2} at PC: {file2_dat[2]}'
+                    status = 'Failed'
+                else:
+
+                    # some cleanup
+                    change1 = file1_dat[-1].split() 
+
+                    # if odd number, it's a store
+                    if len(change1) % 2:
+                        change1.remove('mem')
+
+                    # check if the architectural change is the same
+                    file1dat_iter = iter(change1)
+                    file2dat_iter = iter(file2_dat[-1].split())
+
+                    file1_change = dict(zip(file1dat_iter, file1dat_iter))
+                    file2_change = dict(zip(file2dat_iter, file2dat_iter))
+
+                    if file1_change != file2_change:
+                        rout = rout + f'\nSM: at PC: {file1_dat[2]}'
+                        status = 'Failed'
+                break
     else:
         status = 'Passed'
+    
+    # get number of instructions executed
     with open(f'{file1}','r') as fd:
       rcount = len(fd.readlines())
 
+    return status, rout, rcount
+    
+def compare_signature(file1, file2):
+    '''
+        Function to check whether two signature files are equivalent. This funcion uses the
+        :param file1: The path to the first signature.
+        :param file2: The path to the second signature.raise
+        :return: A string indicating whether the test "Passed" (if files are the same)
+            or "Failed" (if the files are different) and the diff of the files.
+    '''
+    if not os.path.exists(file1) :
+        logger.error('Signature file : ' + file1 + ' does not exist')
+        raise SystemExit(1)
+    cmd = f'diff -iw {file1} {file2}'
+    errcode, rout, rerr = sys_command(cmd, logging=False)
+    if errcode != 0:
+        status = 'Failed'
+    else:
+        status = 'Passed'
 
-#    file1_lines = open(file1, "r").readlines()
-#    file2_lines = open(file2, "r").readlines()
-#    res = ("".join(
-#        difflib.unified_diff(file1_lines,file2_lines, file1, file2))).strip()
-#    if res == "":
-#        if len(file1_lines)==0:
-#            return 'Failed', '---- \nBoth FIles empty\n'
-#        else:
-#            status = 'Passed'
-#    else:
-#        status = 'Failed'
-#
-#        error_report = '\nFile1 Path:{0}\nFile2 Path:{1}\nMatch  Line#    File1    File2\n'.format(
-#                            file1,file2)
-#        fmt = "{0:5s} {1:6d} {2:100s} {3:100s}\n"
-#        prev = ''
-#        include = False
-#        for lnum,lines in enumerate(zip(file1_lines,file2_lines)):
-#            if lines[0] != lines[1]:
-#                include = True
-#                if not include:
-#                    error_report += prev
-#                rline = fmt.format("*",lnum,lines[0].strip(),lines[1].strip())
-#                error_report += rline
-#                prev = rline
-#            elif include:
-#                rline = fmt.format("",lnum,lines[0].strip(),lines[1].strip())
-#                error_report += rline
-#                include = False
-#                prev = rline
-##        res = error_report
+    # number of lines in the signature file
+    with open(f'{file1}','r') as fd:
+      rcount = len(fd.readlines())
+    
     return status, rout, rcount
 
 def str_2_bool(string):
     """
         Simple String to Bool conversion
         
         :param string: A string to convert
```

### Comparing `river_core-1.5.0/river_core.egg-info/PKG-INFO` & `river_core-1.6.0/river_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: river-core
-Version: 1.5.0
+Version: 1.6.0
 Summary: RiVer Core Verification Framework
 Home-page: https://github.com/incoresemi/river_core
 Author: InCore Semiconductors Pvt. Ltd.; Tessolve
 Author-email: neelgala@incoresemi.com
 License: BSD-3-Clause
 Description: **RiVer Core** : RISC-V Core Verification Framework 
         ###################################################################################
```

### Comparing `river_core-1.5.0/river_core.egg-info/SOURCES.txt` & `river_core-1.6.0/river_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `river_core-1.5.0/setup.py` & `river_core-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,10 +58,10 @@
         ]
     },
     setup_requires=setup_requirements,
     test_suite='',
     tests_require=test_requirements,
     url=
     'https://github.com/incoresemi/river_core',
-    version='1.5.0',
+    version='1.6.0',
     zip_safe=False,
 )
```

