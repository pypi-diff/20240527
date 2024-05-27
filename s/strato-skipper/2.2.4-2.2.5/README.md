# Comparing `tmp/strato-skipper-2.2.4.tar.gz` & `tmp/strato-skipper-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strato-skipper-2.2.4.tar", last modified: Sun Feb 18 14:38:24 2024, max compression
+gzip compressed data, was "strato-skipper-2.2.5.tar", last modified: Mon May 27 14:47:13 2024, max compression
```

## Comparing `strato-skipper-2.2.4.tar` & `strato-skipper-2.2.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-02-18 14:38:24.350865 strato-skipper-2.2.4/
--rw-r--r--   0 runner    (1001) runner    (1001)      101 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-02-18 14:38:24.346865 strato-skipper-2.2.4/.github/
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-02-18 14:38:24.346865 strato-skipper-2.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) runner    (1001)     1816 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) runner    (1001)      701 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) runner    (1001)    11123 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/.pylintrc
--rw-r--r--   0 runner    (1001) runner    (1001)     1324 2024-02-18 14:38:24.000000 strato-skipper-2.2.4/AUTHORS
--rw-r--r--   0 runner    (1001) runner    (1001)    16204 2024-02-18 14:38:24.000000 strato-skipper-2.2.4/ChangeLog
--rw-r--r--   0 runner    (1001) runner    (1001)      232 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/Dockerfile.skipper-build
--rw-r--r--   0 runner    (1001) runner    (1001)    11351 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/LICENSE
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) runner    (1001)      431 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/Makefile
--rw-r--r--   0 runner    (1001) runner    (1001)    13005 2024-02-18 14:38:24.350865 strato-skipper-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)    12696 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/README.md
--rw-r--r--   0 runner    (1001) runner    (1001)       36 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/dev-requirements.txt
--rw-r--r--   0 runner    (1001) runner    (1001)      120 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) runner    (1001)      498 2024-02-18 14:38:24.354865 strato-skipper-2.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) runner    (1001)      132 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-02-18 14:38:24.350865 strato-skipper-2.2.4/skipper/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/skipper/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5502 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/skipper/builder.py
--rw-r--r--   0 runner    (1001) runner    (1001)    18452 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/skipper/cli.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1498 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/skipper/config.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-02-18 14:38:24.350865 strato-skipper-2.2.4/skipper/data/
--rw-r--r--   0 runner    (1001) runner    (1001)     6644 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/skipper/data/skipper-complete.sh
--rwxr-xr-x   0 runner    (1001) runner    (1001)      935 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/skipper/data/skipper-entrypoint.sh
--rw-r--r--   0 runner    (1001) runner    (1001)      682 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/skipper/git.py
--rw-r--r--   0 runner    (1001) runner    (1001)      585 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/skipper/main.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7987 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/skipper/runner.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6894 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/skipper/utils.py
--rw-r--r--   0 runner    (1001) runner    (1001)       37 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/skipper.yaml
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-02-18 14:38:24.350865 strato-skipper-2.2.4/strato_skipper.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)    13005 2024-02-18 14:38:24.000000 strato-skipper-2.2.4/strato_skipper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      927 2024-02-18 14:38:24.000000 strato-skipper-2.2.4/strato_skipper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-02-18 14:38:24.000000 strato-skipper-2.2.4/strato_skipper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       46 2024-02-18 14:38:24.000000 strato-skipper-2.2.4/strato_skipper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-02-18 14:38:24.000000 strato-skipper-2.2.4/strato_skipper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) runner    (1001)       46 2024-02-18 14:38:24.000000 strato-skipper-2.2.4/strato_skipper.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) runner    (1001)      131 2024-02-18 14:38:24.000000 strato-skipper-2.2.4/strato_skipper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        8 2024-02-18 14:38:24.000000 strato-skipper-2.2.4/strato_skipper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-02-18 14:38:24.350865 strato-skipper-2.2.4/tests/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      297 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/tests/consts.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6265 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/tests/test_builder.py
--rw-r--r--   0 runner    (1001) runner    (1001)    91175 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3550 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1842 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/tests/test_git.py
--rw-r--r--   0 runner    (1001) runner    (1001)    28193 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/tests/test_runner.py
--rw-r--r--   0 runner    (1001) runner    (1001)    14735 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/tests/test_runner_podman.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2034 2024-02-18 14:37:50.000000 strato-skipper-2.2.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-27 14:47:13.503896 strato-skipper-2.2.5/
+-rw-r--r--   0 runner    (1001) runner    (1001)      101 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/.coveragerc
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-27 14:47:13.499896 strato-skipper-2.2.5/.github/
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-27 14:47:13.499896 strato-skipper-2.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1816 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) runner    (1001)      701 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) runner    (1001)    11123 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/.pylintrc
+-rw-r--r--   0 runner    (1001) runner    (1001)     1369 2024-05-27 14:47:13.000000 strato-skipper-2.2.5/AUTHORS
+-rw-r--r--   0 runner    (1001) runner    (1001)    16260 2024-05-27 14:47:13.000000 strato-skipper-2.2.5/ChangeLog
+-rw-r--r--   0 runner    (1001) runner    (1001)      232 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/Dockerfile.skipper-build
+-rw-r--r--   0 runner    (1001) runner    (1001)    11351 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) runner    (1001)      431 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/Makefile
+-rw-r--r--   0 runner    (1001) runner    (1001)    13005 2024-05-27 14:47:13.503896 strato-skipper-2.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)    12696 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/README.md
+-rw-r--r--   0 runner    (1001) runner    (1001)       36 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)      120 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)      498 2024-05-27 14:47:13.507896 strato-skipper-2.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) runner    (1001)      132 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-27 14:47:13.503896 strato-skipper-2.2.5/skipper/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/skipper/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5502 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/skipper/builder.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18452 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/skipper/cli.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1498 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/skipper/config.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-27 14:47:13.503896 strato-skipper-2.2.5/skipper/data/
+-rw-r--r--   0 runner    (1001) runner    (1001)     6644 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/skipper/data/skipper-complete.sh
+-rwxr-xr-x   0 runner    (1001) runner    (1001)      935 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/skipper/data/skipper-entrypoint.sh
+-rw-r--r--   0 runner    (1001) runner    (1001)      907 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/skipper/git.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      585 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/skipper/main.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7987 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/skipper/runner.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6894 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/skipper/utils.py
+-rw-r--r--   0 runner    (1001) runner    (1001)       37 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/skipper.yaml
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-27 14:47:13.503896 strato-skipper-2.2.5/strato_skipper.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)    13005 2024-05-27 14:47:13.000000 strato-skipper-2.2.5/strato_skipper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      927 2024-05-27 14:47:13.000000 strato-skipper-2.2.5/strato_skipper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-05-27 14:47:13.000000 strato-skipper-2.2.5/strato_skipper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       46 2024-05-27 14:47:13.000000 strato-skipper-2.2.5/strato_skipper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-05-27 14:47:13.000000 strato-skipper-2.2.5/strato_skipper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) runner    (1001)       47 2024-05-27 14:47:13.000000 strato-skipper-2.2.5/strato_skipper.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) runner    (1001)      131 2024-05-27 14:47:13.000000 strato-skipper-2.2.5/strato_skipper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        8 2024-05-27 14:47:13.000000 strato-skipper-2.2.5/strato_skipper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-27 14:47:13.503896 strato-skipper-2.2.5/tests/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      297 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/tests/consts.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6265 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    91175 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3550 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2896 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/tests/test_git.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    28193 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    14735 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/tests/test_runner_podman.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2034 2024-05-27 14:46:46.000000 strato-skipper-2.2.5/tests/test_utils.py
```

### Comparing `strato-skipper-2.2.4/.github/workflows/build.yml` & `strato-skipper-2.2.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.2.4/.github/workflows/publish-to-pypi.yml` & `strato-skipper-2.2.5/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.2.4/.pylintrc` & `strato-skipper-2.2.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.2.4/AUTHORS` & `strato-skipper-2.2.5/AUTHORS`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 Eran Cohen <eran@stratoscale.com>
 Eran Cohen <eranco@redhat.com>
 Eran Ifrach <eifrach@redhat.com>
 Eyal <posener@gmail.com>
 Eyal Posener <eyal@stratoscale.com>
 Igal Tsoiref <igal.tsoiref@stratoscale.com>
 Igal Tsoiref <itsoiref@redhat.com>
+IliaFeldgun <ilia.feldgun@zadarastorage.com>
 Juan Hernandez <juan.hernandez@redhat.com>
 Michael Filanov <michael.filanov@stratoscale.com>
 Michael Levy <milevy@redhat.com>
 Ofir Amir <ofamir@gmail.com>
 Omer Tuchfeld <omer@tuchfeld.dev>
 Osher De Paz <osherdepaz@gmail.com>
 Ravid Brown <ravid.brown@stratoscale.com>
```

### Comparing `strato-skipper-2.2.4/ChangeLog` & `strato-skipper-2.2.5/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+v2.2.5
+------
+
+* Fix #174 detect git in project subdir
+
 v2.2.4
 ------
 
 * fix empty env
 * ignore boolean in env interpolation
 * enable the option for users to choose whether to utilize sudo
```

### Comparing `strato-skipper-2.2.4/LICENSE` & `strato-skipper-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.2.4/PKG-INFO` & `strato-skipper-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strato-skipper
-Version: 2.2.4
+Version: 2.2.5
 Summary: Easily dockerize your Git repository
 Home-page: http://github.com/Stratoscale/skipper
 Author: Adir Gabai
 Author-email: adir@stratoscale.com
 License: Apache-2
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `strato-skipper-2.2.4/README.md` & `strato-skipper-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.2.4/skipper/builder.py` & `strato-skipper-2.2.5/skipper/builder.py`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.2.4/skipper/cli.py` & `strato-skipper-2.2.5/skipper/cli.py`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.2.4/skipper/config.py` & `strato-skipper-2.2.5/skipper/config.py`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.2.4/skipper/data/skipper-complete.sh` & `strato-skipper-2.2.5/skipper/data/skipper-complete.sh`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.2.4/skipper/data/skipper-entrypoint.sh` & `strato-skipper-2.2.5/skipper/data/skipper-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.2.4/skipper/git.py` & `strato-skipper-2.2.5/skipper/git.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import os.path
 import logging
+import os
 import subprocess
 
 
 def get_hash(short=False):
-    if not os.path.exists('.git'):
+    if not is_git_repository():
         logging.warning('*** Not working in a git repository ***')
         return 'none'
 
     git_command = ['git', 'rev-parse']
     if short:
         git_command += ['--short']
     git_command += ['HEAD']
@@ -18,7 +18,14 @@
 
     return subprocess.check_output(git_command).strip().decode('utf-8')
 
 
 def uncommitted_changes():
     """Return True is there are uncommitted changes."""
     return subprocess.call(['git', 'diff', '--quiet', 'HEAD']) != 0
+
+
+def is_git_repository():
+    if os.path.exists('.git'):
+        return True
+    command = ['git', 'rev-parse', '--is-inside-work-tree']
+    return subprocess.call(command, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL) == 0
```

### Comparing `strato-skipper-2.2.4/skipper/main.py` & `strato-skipper-2.2.5/skipper/main.py`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.2.4/skipper/runner.py` & `strato-skipper-2.2.5/skipper/runner.py`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.2.4/skipper/utils.py` & `strato-skipper-2.2.5/skipper/utils.py`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.2.4/strato_skipper.egg-info/PKG-INFO` & `strato-skipper-2.2.5/strato_skipper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strato-skipper
-Version: 2.2.4
+Version: 2.2.5
 Summary: Easily dockerize your Git repository
 Home-page: http://github.com/Stratoscale/skipper
 Author: Adir Gabai
 Author-email: adir@stratoscale.com
 License: Apache-2
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `strato-skipper-2.2.4/strato_skipper.egg-info/SOURCES.txt` & `strato-skipper-2.2.5/strato_skipper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.2.4/tests/test_builder.py` & `strato-skipper-2.2.5/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.2.4/tests/test_cli.py` & `strato-skipper-2.2.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.2.4/tests/test_config.py` & `strato-skipper-2.2.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.2.4/tests/test_git.py` & `strato-skipper-2.2.5/tests/test_git.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,58 @@
+import subprocess
 import unittest
 import mock
 from skipper import git
 
 
 GIT_HASH_FULL = b'00efe974e3cf18c3493f110f5aeda04ff78b125f'
 GIT_HASH_SHORT = b'00efe97'
 
 
 class TestGit(unittest.TestCase):
     @mock.patch('subprocess.check_output', return_value=GIT_HASH_FULL)
-    @mock.patch('os.path.exists', return_value=True)
-    def test_get_hash_with_default_argument(self, exists_mock, check_output_mock):
+    @mock.patch('skipper.git.is_git_repository', return_value=True)
+    def test_get_hash_with_default_argument(self, is_git_repository_mock, check_output_mock):
         git_hash = git.get_hash()
-        exists_mock.assert_called_once_with('.git')
+        is_git_repository_mock.assert_called_once()
         check_output_mock.assert_called_once_with(['git', 'rev-parse', 'HEAD'])
         self.assertEqual(git_hash, GIT_HASH_FULL.decode('utf-8'))
 
     @mock.patch('subprocess.check_output', return_value=GIT_HASH_FULL)
-    @mock.patch('os.path.exists', return_value=True)
-    def test_get_full_hash(self, exists_mock, check_output_mock):
+    @mock.patch('skipper.git.is_git_repository', return_value=True)
+    def test_get_full_hash(self, is_git_repository_mock, check_output_mock):
         git_hash = git.get_hash(short=False)
-        exists_mock.assert_called_once_with('.git')
+        is_git_repository_mock.assert_called_once()
         check_output_mock.assert_called_once_with(['git', 'rev-parse', 'HEAD'])
         self.assertEqual(git_hash, GIT_HASH_FULL.decode('utf-8'))
 
     @mock.patch('subprocess.check_output', return_value=GIT_HASH_SHORT)
-    @mock.patch('os.path.exists', return_value=True)
-    def test_get_short_hash(self, exists_mock, check_output_mock):
+    @mock.patch('skipper.git.is_git_repository', return_value=True)
+    def test_get_short_hash(self, is_git_repository_mock, check_output_mock):
         git_hash = git.get_hash(short=True)
-        exists_mock.assert_called_once_with('.git')
+        is_git_repository_mock.assert_called_once()
         check_output_mock.assert_called_once_with(['git', 'rev-parse', '--short', 'HEAD'])
         self.assertEqual(git_hash, GIT_HASH_SHORT.decode('utf-8'))
 
-    @mock.patch('subprocess.check_output')
+    @mock.patch('skipper.git.is_git_repository', return_value=False)
+    def test_not_in_git_project(self, is_git_repository_mock):
+        self.assertEqual(git.get_hash(), 'none')
+        is_git_repository_mock.assert_called_once()
+
+    @mock.patch('os.path.exists', return_value=True)
+    def test_should_be_in_git_project_os_path(self, exists_mock):
+        self.assertTrue(git.is_git_repository())
+        exists_mock.assert_called_once_with('.git')
+
+    @mock.patch('subprocess.call', return_value=0)
     @mock.patch('os.path.exists', return_value=False)
-    def test_not_in_git_project(self, exists_mock, check_output_mock):
-        git_hash = git.get_hash()
+    def test_should_be_in_git_project_git(self, exists_mock, call_mock):
+        self.assertTrue(git.is_git_repository())
+        exists_mock.assert_called_once_with('.git')
+        call_mock.assert_called_once_with(['git', 'rev-parse', '--is-inside-work-tree'], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+
+    @mock.patch('subprocess.call', return_value=1)
+    @mock.patch('os.path.exists', return_value=False)
+    def test_should_not_be_in_git_project(self, exists_mock, call_mock):
+        self.assertFalse(git.is_git_repository())
         exists_mock.assert_called_once_with('.git')
-        check_output_mock.assert_not_called()
-        self.assertEqual(git_hash, 'none')
+        call_mock.assert_called_once_with(['git', 'rev-parse', '--is-inside-work-tree'], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
```

### Comparing `strato-skipper-2.2.4/tests/test_runner.py` & `strato-skipper-2.2.5/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.2.4/tests/test_runner_podman.py` & `strato-skipper-2.2.5/tests/test_runner_podman.py`

 * *Files identical despite different names*

### Comparing `strato-skipper-2.2.4/tests/test_utils.py` & `strato-skipper-2.2.5/tests/test_utils.py`

 * *Files identical despite different names*

