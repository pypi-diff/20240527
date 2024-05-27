# Comparing `tmp/aiosysbus-1.1.7.tar.gz` & `tmp/aiosysbus-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosysbus-1.1.7.tar", last modified: Wed May  8 07:43:46 2024, max compression
+gzip compressed data, was "aiosysbus-1.1.8.tar", last modified: Mon May 27 16:19:41 2024, max compression
```

## Comparing `aiosysbus-1.1.7.tar` & `aiosysbus-1.1.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:43:46.727547 aiosysbus-1.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:43:46.719547 aiosysbus-1.1.7/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:43:46.723547 aiosysbus-1.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/.github/workflows/auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-08 07:43:46.727547 aiosysbus-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:43:46.723547 aiosysbus-1.1.7/aiosysbus/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/aiosysbus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:43:46.727547 aiosysbus-1.1.7/aiosysbus/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10386 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/call.py
--rw-r--r--   0 runner    (1001) docker     (127)    11999 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/diagnostic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/dnsdhcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/nemo.py
--rw-r--r--   0 runner    (1001) docker     (127)    16914 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    13796 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/nmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/powermgmt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11163 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    11794 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:43:46.727547 aiosysbus-1.1.7/aiosysbus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-08 07:43:46.000000 aiosysbus-1.1.7/aiosysbus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-08 07:43:46.000000 aiosysbus-1.1.7/aiosysbus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 07:43:46.000000 aiosysbus-1.1.7/aiosysbus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 07:43:46.000000 aiosysbus-1.1.7/aiosysbus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 07:43:46.000000 aiosysbus-1.1.7/aiosysbus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 07:43:46.727547 aiosysbus-1.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:43:46.727547 aiosysbus-1.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:43:46.727547 aiosysbus-1.1.7/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/tests/fixtures/deviceinfo.json
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/tests/test_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:41.835683 aiosysbus-1.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:41.831683 aiosysbus-1.1.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:41.831683 aiosysbus-1.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-27 16:19:41.835683 aiosysbus-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:41.831683 aiosysbus-1.1.8/aiosysbus/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/aiosysbus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/aiosysbus/aiosysbus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:41.835683 aiosysbus-1.1.8/aiosysbus/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/aiosysbus/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10386 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/aiosysbus/api/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11999 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/aiosysbus/api/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/aiosysbus/api/diagnostic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/aiosysbus/api/dnsdhcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15290 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/aiosysbus/api/nemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16914 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/aiosysbus/api/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13796 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/aiosysbus/api/nmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/aiosysbus/api/powermgmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/aiosysbus/api/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11163 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/aiosysbus/api/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/aiosysbus/api/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11794 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/aiosysbus/api/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/aiosysbus/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/aiosysbus/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/aiosysbus/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/aiosysbus/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:41.835683 aiosysbus-1.1.8/aiosysbus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-27 16:19:41.000000 aiosysbus-1.1.8/aiosysbus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-27 16:19:41.000000 aiosysbus-1.1.8/aiosysbus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:19:41.000000 aiosysbus-1.1.8/aiosysbus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 16:19:41.000000 aiosysbus-1.1.8/aiosysbus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 16:19:41.000000 aiosysbus-1.1.8/aiosysbus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 16:19:41.835683 aiosysbus-1.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:41.835683 aiosysbus-1.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:41.835683 aiosysbus-1.1.8/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/tests/fixtures/deviceinfo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-27 16:19:26.000000 aiosysbus-1.1.8/tests/test_connection.py
```

### Comparing `aiosysbus-1.1.7/.github/dependabot.yml` & `aiosysbus-1.1.8/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/.github/workflows/auto-approve.yml` & `aiosysbus-1.1.8/.github/workflows/auto-approve.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: Dependency auto-merge
 on: pull_request
 
 permissions:
   pull-requests: write
-  content: write
+  contents: write
 
 jobs:
   dependency:
     runs-on: ubuntu-latest
     if: ${{ github.actor == 'dependabot[bot]' || github.actor == 'pre-commit-ci[bot]' }}
     steps:
       - name: Approve a PR
```

### Comparing `aiosysbus-1.1.7/.github/workflows/lint.yml` & `aiosysbus-1.1.8/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/.github/workflows/pythonpublish.yml` & `aiosysbus-1.1.8/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/.github/workflows/release.yml` & `aiosysbus-1.1.8/.github/workflows/release.yml`

 * *Files 9% similar despite different names*

```diff
@@ -23,8 +23,8 @@
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         with:
           tag_name: ${{ github.ref }}
           release_name: ${{ github.ref }}
           body: ${{ steps.changelog.outputs.changelog }}
           draft: false
-          prerelease: false
+          prerelease: ${{ contains(github.ref_name,'-') }}
```

### Comparing `aiosysbus-1.1.7/.gitignore` & `aiosysbus-1.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/.pre-commit-config.yaml` & `aiosysbus-1.1.8/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ---
 repos:
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.4.3
+    rev: v0.4.4
     hooks:
       - id: ruff
         args:
           - --fix
       - id: ruff-format
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
```

### Comparing `aiosysbus-1.1.7/LICENSE` & `aiosysbus-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/PKG-INFO` & `aiosysbus-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosysbus
-Version: 1.1.7
+Version: 1.1.8
 Summary: Provides asynchronous authentication and access to Livebox
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: livebox,async
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `aiosysbus-1.1.7/README.md` & `aiosysbus-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/aiosysbus/__init__.py` & `aiosysbus-1.1.8/aiosysbus/__init__.py`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/aiosysbus/aiosysbus.py` & `aiosysbus-1.1.8/aiosysbus/aiosysbus.py`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/aiosysbus/api/__init__.py` & `aiosysbus-1.1.8/aiosysbus/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/aiosysbus/api/call.py` & `aiosysbus-1.1.8/aiosysbus/api/call.py`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/aiosysbus/api/device.py` & `aiosysbus-1.1.8/aiosysbus/api/device.py`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/aiosysbus/api/diagnostic.py` & `aiosysbus-1.1.8/aiosysbus/api/diagnostic.py`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/aiosysbus/api/dnsdhcp.py` & `aiosysbus-1.1.8/aiosysbus/api/dnsdhcp.py`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/aiosysbus/api/nemo.py` & `aiosysbus-1.1.8/aiosysbus/api/nemo.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,15 +335,15 @@
         """Get DSL Line Stats."""
         return await self._auth.post("NeMo.Intf.dsl0", "getDSLLineStats")
 
     async def async_get_dsl0_stats(self) -> None:
         """Get DSL Stats."""
         return await self._auth.post("NeMo.Intf.dsl0", "getDSLStats")
 
-    async def async_getxdsl0_noise_measure(self, conf: dict["str", Any]) -> None:
+    async def async_getxdsl0_noise_measure(self, conf: dict[str, Any]) -> None:
         """Get XDSL Noise Measure.
 
         Argument:
         - typeMeasure (str)
         """
         return await self._auth.post("NeMo.Intf.dsl0", "getXDSLNoiseMeasure", conf)
```

### Comparing `aiosysbus-1.1.7/aiosysbus/api/network.py` & `aiosysbus-1.1.8/aiosysbus/api/network.py`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/aiosysbus/api/nmc.py` & `aiosysbus-1.1.8/aiosysbus/api/nmc.py`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/aiosysbus/api/powermgmt.py` & `aiosysbus-1.1.8/aiosysbus/api/powermgmt.py`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/aiosysbus/api/schedule.py` & `aiosysbus-1.1.8/aiosysbus/api/schedule.py`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/aiosysbus/api/services.py` & `aiosysbus-1.1.8/aiosysbus/api/services.py`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/aiosysbus/api/storage.py` & `aiosysbus-1.1.8/aiosysbus/api/storage.py`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/aiosysbus/api/system.py` & `aiosysbus-1.1.8/aiosysbus/api/system.py`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/aiosysbus/api/user.py` & `aiosysbus-1.1.8/aiosysbus/api/user.py`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/aiosysbus/auth.py` & `aiosysbus-1.1.8/aiosysbus/auth.py`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/aiosysbus/exceptions.py` & `aiosysbus-1.1.8/aiosysbus/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/aiosysbus.egg-info/PKG-INFO` & `aiosysbus-1.1.8/aiosysbus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosysbus
-Version: 1.1.7
+Version: 1.1.8
 Summary: Provides asynchronous authentication and access to Livebox
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: livebox,async
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `aiosysbus-1.1.7/aiosysbus.egg-info/SOURCES.txt` & `aiosysbus-1.1.8/aiosysbus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/example.py` & `aiosysbus-1.1.8/example.py`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/pyproject.toml` & `aiosysbus-1.1.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 requires-python = ">=3.11"
 dependencies    = [
     "aiohttp>=3.9.1",
     "yarl>=1.9.4",
 ]
 [tool.setuptools_scm]
 
-[tool.ruff.flake8-pytest-style]
+[tool.ruff.lint.flake8-pytest-style]
 fixture-parentheses = false
 
-[tool.ruff.flake8-tidy-imports.banned-api]
+[tool.ruff.lint.flake8-tidy-imports.banned-api]
 "async_timeout".msg = "use asyncio.timeout instead"
 "pytz".msg = "use zoneinfo instead"
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 force-sort-within-sections = true
 combine-as-imports = true
 split-on-trailing-comma = false
```

### Comparing `aiosysbus-1.1.7/tests/fixtures/deviceinfo.json` & `aiosysbus-1.1.8/tests/fixtures/deviceinfo.json`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.7/tests/test_connection.py` & `aiosysbus-1.1.8/tests/test_connection.py`

 * *Files identical despite different names*

