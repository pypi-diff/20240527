# Comparing `tmp/bboxpy-1.1.7.tar.gz` & `tmp/bboxpy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bboxpy-1.1.7.tar", last modified: Fri Jan 26 07:18:43 2024, max compression
+gzip compressed data, was "bboxpy-1.2.0.tar", last modified: Mon May 27 17:12:26 2024, max compression
```

## Comparing `bboxpy-1.1.7.tar` & `bboxpy-1.2.0.tar`

### file list

```diff
@@ -1,42 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:18:43.886849 bboxpy-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-01-26 07:18:24.000000 bboxpy-1.1.7/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:18:43.882850 bboxpy-1.1.7/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-01-26 07:18:24.000000 bboxpy-1.1.7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:18:43.882850 bboxpy-1.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-01-26 07:18:24.000000 bboxpy-1.1.7/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-01-26 07:18:24.000000 bboxpy-1.1.7/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-01-26 07:18:24.000000 bboxpy-1.1.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-01-26 07:18:24.000000 bboxpy-1.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-01-26 07:18:24.000000 bboxpy-1.1.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-26 07:18:24.000000 bboxpy-1.1.7/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:18:43.882850 bboxpy-1.1.7/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-26 07:18:24.000000 bboxpy-1.1.7/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-26 07:18:24.000000 bboxpy-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-01-26 07:18:24.000000 bboxpy-1.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-01-26 07:18:43.886849 bboxpy-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-01-26 07:18:24.000000 bboxpy-1.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:18:43.882850 bboxpy-1.1.7/bboxpy/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-01-26 07:18:24.000000 bboxpy-1.1.7/bboxpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:18:43.882850 bboxpy-1.1.7/bboxpy/api/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-26 07:18:24.000000 bboxpy-1.1.7/bboxpy/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-01-26 07:18:24.000000 bboxpy-1.1.7/bboxpy/api/ddns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-01-26 07:18:24.000000 bboxpy-1.1.7/bboxpy/api/device.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-01-26 07:18:24.000000 bboxpy-1.1.7/bboxpy/api/iptv.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-01-26 07:18:24.000000 bboxpy-1.1.7/bboxpy/api/lan.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-01-26 07:18:24.000000 bboxpy-1.1.7/bboxpy/api/voip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-01-26 07:18:24.000000 bboxpy-1.1.7/bboxpy/api/wan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-01-26 07:18:24.000000 bboxpy-1.1.7/bboxpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-01-26 07:18:24.000000 bboxpy-1.1.7/bboxpy/bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-01-26 07:18:24.000000 bboxpy-1.1.7/bboxpy/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:18:43.882850 bboxpy-1.1.7/bboxpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-01-26 07:18:43.000000 bboxpy-1.1.7/bboxpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-01-26 07:18:43.000000 bboxpy-1.1.7/bboxpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 07:18:43.000000 bboxpy-1.1.7/bboxpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 07:18:43.000000 bboxpy-1.1.7/bboxpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-26 07:18:43.000000 bboxpy-1.1.7/bboxpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-26 07:18:43.000000 bboxpy-1.1.7/bboxpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-01-26 07:18:24.000000 bboxpy-1.1.7/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-01-26 07:18:36.000000 bboxpy-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-01-26 07:18:24.000000 bboxpy-1.1.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-26 07:18:24.000000 bboxpy-1.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-26 07:18:43.886849 bboxpy-1.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:12:26.422615 bboxpy-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:12:26.418615 bboxpy-1.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-27 17:12:17.000000 bboxpy-1.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:12:26.418615 bboxpy-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-27 17:12:17.000000 bboxpy-1.2.0/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-27 17:12:17.000000 bboxpy-1.2.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-27 17:12:17.000000 bboxpy-1.2.0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-27 17:12:17.000000 bboxpy-1.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-27 17:12:17.000000 bboxpy-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-27 17:12:17.000000 bboxpy-1.2.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:12:26.418615 bboxpy-1.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-27 17:12:17.000000 bboxpy-1.2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 17:12:17.000000 bboxpy-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-27 17:12:17.000000 bboxpy-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-27 17:12:26.422615 bboxpy-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-27 17:12:17.000000 bboxpy-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:12:26.418615 bboxpy-1.2.0/bboxpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-27 17:12:17.000000 bboxpy-1.2.0/bboxpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:12:26.422615 bboxpy-1.2.0/bboxpy/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-27 17:12:17.000000 bboxpy-1.2.0/bboxpy/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-27 17:12:17.000000 bboxpy-1.2.0/bboxpy/api/ddns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-27 17:12:17.000000 bboxpy-1.2.0/bboxpy/api/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-27 17:12:17.000000 bboxpy-1.2.0/bboxpy/api/iptv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-27 17:12:17.000000 bboxpy-1.2.0/bboxpy/api/lan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-27 17:12:17.000000 bboxpy-1.2.0/bboxpy/api/voip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-27 17:12:17.000000 bboxpy-1.2.0/bboxpy/api/wan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-27 17:12:17.000000 bboxpy-1.2.0/bboxpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-27 17:12:17.000000 bboxpy-1.2.0/bboxpy/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-27 17:12:17.000000 bboxpy-1.2.0/bboxpy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:12:26.422615 bboxpy-1.2.0/bboxpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-27 17:12:26.000000 bboxpy-1.2.0/bboxpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-27 17:12:26.000000 bboxpy-1.2.0/bboxpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 17:12:26.000000 bboxpy-1.2.0/bboxpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 17:12:26.000000 bboxpy-1.2.0/bboxpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 17:12:26.000000 bboxpy-1.2.0/bboxpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-27 17:12:26.000000 bboxpy-1.2.0/bboxpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-27 17:12:17.000000 bboxpy-1.2.0/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-27 17:12:17.000000 bboxpy-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-27 17:12:17.000000 bboxpy-1.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 17:12:17.000000 bboxpy-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 17:12:26.422615 bboxpy-1.2.0/setup.cfg
```

### Comparing `bboxpy-1.1.7/.github/dependabot.yml` & `bboxpy-1.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bboxpy-1.1.7/.github/workflows/lint.yml` & `bboxpy-1.2.0/.github/workflows/lint.yml`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 jobs:
   build:
     runs-on: ubuntu-latest
     name: Check the code
     strategy:
       max-parallel: 4
       matrix:
-        python-version: ["3.10", "3.11", "3.12"]
+        python-version: ["3.11", "3.12"]
 
     steps:
       - name: 📥 Checkout the repository
         uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
@@ -22,8 +22,8 @@
 
       - name: 📦 Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r requirements.txt
 
       - name: Run pre-commit
-        uses: pre-commit/action@v3.0.0
+        uses: pre-commit/action@v3.0.1
```

### Comparing `bboxpy-1.1.7/.github/workflows/pythonpublish.yml` & `bboxpy-1.2.0/.github/workflows/pythonpublish.yml`

 * *Files 25% similar despite different names*

```diff
@@ -8,39 +8,31 @@
     tags:
       - "*.*.*"
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     name: Deploy to PyPi
-    # Specifying a GitHub environment is optional, but strongly encouraged
     environment: release
     permissions:
-      # IMPORTANT: this permission is mandatory for trusted publishing
       id-token: write
     steps:
       - name: 📥 Checkout the repository
         uses: actions/checkout@v4
 
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
-          python-version: "3.x"
+          python-version: "3.11"
 
       - name: 📦 Install dependencies
         run: |
-          python3 -m pip install --upgrade pip
+          python -m pip install --upgrade pip
           pip install setuptools wheel twine build
 
-      - name: 🔢 Set version number
-        run: |
-          export version=${{ github.ref }}
-          sed -i "s|replace_by_workflow|${version##*/}|" ./pyproject.toml
-          cat ./pyproject.toml
-
       - name: Build package
         shell: bash
         run: |
           python3 -m build
 
       - name: 🚀 Publish to PyPi
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `bboxpy-1.1.7/.github/workflows/release.yml` & `bboxpy-1.2.0/.github/workflows/release.yml`

 * *Files 10% similar despite different names*

```diff
@@ -10,21 +10,21 @@
       contents: write
     steps:
       # To use this repository's private action, you must check out the repository
       - name: Checkout
         uses: actions/checkout@v4
       - name: Generate changelog
         id: changelog
-        uses: metcalfc/changelog-generator@v4.2.0
+        uses: metcalfc/changelog-generator@v4.3.1
         with:
           myToken: ${{ secrets.GITHUB_TOKEN }}
       - name: Create Release
         id: create_release
         uses: actions/create-release@latest
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         with:
           tag_name: ${{ github.ref }}
           release_name: ${{ github.ref }}
           body: ${{ steps.changelog.outputs.changelog }}
           draft: false
-          prerelease: true
+          prerelease: ${{ contains(github.ref_name,'-') }}
```

### Comparing `bboxpy-1.1.7/.gitignore` & `bboxpy-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bboxpy-1.1.7/.pre-commit-config.yaml` & `bboxpy-1.2.0/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 ---
 repos:
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.1.14
+    rev: v0.4.4
     hooks:
       - id: ruff
         args:
           - --fix
       - id: ruff-format
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
     hooks:
       - id: codespell
         args:
           - --skip="./.*,*.csv,*.json,*.ambr"
           - --quiet-level=2
         exclude_types: [csv, json]
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-executables-have-shebangs
         stages: [manual]
       - id: check-json
         exclude: (.vscode|.devcontainer)
   - repo: https://github.com/adrienverge/yamllint.git
-    rev: v1.33.0
+    rev: v1.35.1
     hooks:
       - id: yamllint
         exclude: (.github|.vscode|.devcontainer)
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v4.0.0-alpha.8
     hooks:
       - id: prettier
@@ -41,11 +41,11 @@
       - id: python-typing-update
         stages: [manual]
         args:
           - --py311-plus
           - --force
           - --keep-updates
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.8.0
+    rev: v1.10.0
     hooks:
       - id: mypy
         args: [--strict, --ignore-missing-imports]
```

### Comparing `bboxpy-1.1.7/LICENSE` & `bboxpy-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bboxpy-1.1.7/PKG-INFO` & `bboxpy-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bboxpy
-Version: 1.1.7
+Version: 1.2.0
 Summary: Fetch data from bouygues bbox
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: bouygues,async,bbox
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bboxpy-1.1.7/README.md` & `bboxpy-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bboxpy-1.1.7/bboxpy/api/device.py` & `bboxpy-1.2.0/bboxpy/api/device.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,62 +1,67 @@
 """Devices."""
+
 from __future__ import annotations
 
+from collections.abc import Callable
+from typing import Any
+
 
 class Device:
     """Device information."""
 
-    def __init__(self, request):
+    def __init__(self, request: Callable[..., Any]) -> None:
         """Initialize."""
         self.async_request = request
 
-    async def async_get_bbox_info(self):
+    async def async_get_bbox_info(self) -> Any:
         """Fetch data information."""
-        return await self.async_request("get", "v1/device")
+        return await self.async_request("device")
 
-    async def async_get_bbox_cpu(self):
+    async def async_get_bbox_cpu(self) -> Any:
         """Fetch data information."""
-        return await self.async_request("get", "v1/device/cpu")
+        return await self.async_request("device/cpu")
 
-    async def async_get_bbox_led(self):
+    async def async_get_bbox_led(self) -> Any:
         """Fetch data information."""
-        return await self.async_request("get", "v1/device/led")
+        return await self.async_request("device/led")
 
-    async def async_get_bbox_mem(self):
+    async def async_get_bbox_mem(self) -> Any:
         """Fetch data information."""
-        return await self.async_request("get", "v1/device/mem")
+        return await self.async_request("device/mem")
 
-    async def async_get_bbox_summary(self):
+    async def async_get_bbox_summary(self) -> Any:
         """Fetch data information."""
-        return await self.async_request("get", "v1/device/summary")
+        return await self.async_request("device/summary")
 
-    async def async_get_bbox_token(self):
+    async def async_get_bbox_token(self) -> Any:
         """Fetch data information."""
-        return await self.async_request("get", "v1/device/token")
+        return await self.async_request("device/token")
 
-    async def async_get_bbox_log(self):
+    async def async_get_bbox_log(self) -> Any:
         """Fetch data information."""
-        return await self.async_request("get", "v1/device/log")
+        return await self.async_request("device/log")
 
-    async def async_reboot(self):
+    async def async_reboot(self) -> None:
         """Fetch data information."""
-        return await self.async_request("post", "v1/device/reboot")
+        await self.async_request("device/reboot", "post")
 
-    async def async_reset(self):
+    async def async_reset(self) -> None:
         """Fetch data information."""
-        return await self.async_request("post", "v1/device/factory")
+        await self.async_request("device/factory", "post")
 
-    async def async_optimization(self, flag: bool):
+    async def async_optimization(self, flag: bool) -> None:
         """Fetch data information."""
-        flag = 1 if flag else 0
-        return await self.async_request(
-            "put", "v1/device/optimization", {"boolean": flag}
+        await self.async_request(
+            "device/optimization", "put", json={"boolean": 1 if flag else 0}
         )
 
-    async def async_display(self, luminosity: int = None, orientation: int = None):
+    async def async_display(
+        self, luminosity: int | None = None, orientation: int | None = None
+    ) -> None:
         """Fetch data information."""
         data = {}
         if luminosity:
             data.update({"luminosity": luminosity})
         if orientation:
             data.update({"orientation": orientation})
-        return await self.async_request("post", "v1/device/display", data)
+        await self.async_request("device/display", "post", json=data)
```

### Comparing `bboxpy-1.1.7/bboxpy/api/lan.py` & `bboxpy-1.2.0/bboxpy/api/lan.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 """Lan."""
+
 from __future__ import annotations
 
+from collections.abc import Callable
+from typing import Any
+
 
 class Lan:
     """Lan information."""
 
-    def __init__(self, request):
+    def __init__(self, request: Callable[..., Any]) -> None:
         """Initialize."""
         self.async_request = request
 
-    async def async_get_connected_devices(self):
+    async def async_get_connected_devices(self) -> Any:
         """Fetch data information."""
-        return await self.async_request("get", "v1/hosts")
+        return await self.async_request("hosts")
 
-    async def async_get_ip_infos(self):
+    async def async_get_ip_infos(self) -> Any:
         """Fetch data information."""
-        return await self.async_request("get", "v1/lan/ip")
+        return await self.async_request("lan/ip")
 
-    async def async_get_lan_stats(self):
+    async def async_get_lan_stats(self) -> Any:
         """Fetch data information."""
-        return await self.async_request("get", "v1/lan/stats")
+        return await self.async_request("lan/stats")
 
-    async def async_get_device_infos(self):
+    async def async_get_device_infos(self) -> Any:
         """Fetch data information."""
-        return await self.async_request("get", "v1/hosts/me")
+        return await self.async_request("hosts/me")
```

### Comparing `bboxpy-1.1.7/bboxpy/api/voip.py` & `bboxpy-1.2.0/bboxpy/api/ddns.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""VOIP."""
+"""Dynamic DNS."""
+
 from __future__ import annotations
 
+from collections.abc import Callable
+from typing import Any
+
 
-class VOIP:
-    """VOIP information."""
+class Ddns:
+    """Dynamic DNS information."""
 
-    def __init__(self, request):
+    def __init__(self, request: Callable[..., Any]) -> None:
         """Initialize."""
         self.async_request = request
 
-    async def async_get_voip_voicemail(self):
-        """Fetch data information."""
-        return await self.async_request("get", "v1/voip/voicemail")
-
-    async def async_get_voip_callforward(self):
+    async def async_get_ddns(self) -> Any:
         """Fetch data information."""
-        return await self.async_request("get", "v1/voip/callforward")
+        return await self.async_request("dyndns")
 
-    async def async_del_voip_calllog_by_id(self, by_id: int):
+    async def async_get_ddns_by_id(self, by_id: int) -> Any:
         """Fetch data information."""
-        return await self.async_request("delete", f"v1/voip/calllog/{by_id}")
+        return await self.async_request(f"dyndns/{by_id}")
```

### Comparing `bboxpy-1.1.7/bboxpy/api/wan.py` & `bboxpy-1.2.0/bboxpy/api/wan.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 """Wan."""
+
 from __future__ import annotations
 
+from collections.abc import Callable
+from typing import Any
+
 
 class Wan:
     """Wan information."""
 
-    def __init__(self, request):
+    def __init__(self, request: Callable[..., Any]) -> None:
         """Initialize."""
         self.async_request = request
 
-    async def async_get_wan_cpl(self):
+    async def async_get_wan_cpl(self) -> Any:
         """Fetch data information."""
-        return await self.async_request("get", "v1/cpl")
+        return await self.async_request("cpl")
 
-    async def async_get_wan_cable(self):
+    async def async_get_wan_cable(self) -> Any:
         """Fetch data information."""
-        return await self.async_request("get", "v1/wan/cable")
+        return await self.async_request("wan/cable")
 
-    async def async_get_wan_ftth(self):
+    async def async_get_wan_ftth(self) -> Any:
         """Fetch data information."""
-        return await self.async_request("get", "v1/wan/ftth/stats")
+        return await self.async_request("wan/ftth/stats")
 
-    async def async_get_wan_diags(self):
+    async def async_get_wan_diags(self) -> Any:
         """Fetch data information."""
-        return await self.async_request("get", "v1/wan/diags")
+        return await self.async_request("wan/diags")
 
-    async def async_get_wan_ip(self):
+    async def async_get_wan_ip(self) -> Any:
         """Fetch data information."""
-        return await self.async_request("get", "v1/wan/ip")
+        return await self.async_request("wan/ip")
 
-    async def async_get_wan_ip_stats(self):
+    async def async_get_wan_ip_stats(self) -> Any:
         """Fetch data information."""
-        return await self.async_request("get", "v1/wan/ip/stats")
+        return await self.async_request("wan/ip/stats")
 
-    async def async_get_wan_xdsl(self):
+    async def async_get_wan_xdsl(self) -> Any:
         """Fetch data information."""
-        return await self.async_request("get", "v1/wan/xdsl")
+        return await self.async_request("wan/xdsl")
 
-    async def async_get_wan_xdsl_stats(self):
+    async def async_get_wan_xdsl_stats(self) -> Any:
         """Fetch data information."""
-        return await self.async_request("get", "v1/wan/xdsl/stats")
+        return await self.async_request("wan/xdsl/stats")
```

### Comparing `bboxpy-1.1.7/bboxpy/auth.py` & `bboxpy-1.2.0/bboxpy/auth.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,111 +1,79 @@
 """Bbox connect."""
+
 from __future__ import annotations
 
 import asyncio
 import json
 import logging
 import socket
-from typing import Any
+from typing import Any, cast
 
-import aiohttp
-import async_timeout
+from aiohttp import ClientError, ClientResponse, ClientResponseError, ClientSession
 
 from .exceptions import HttpRequestError, ServiceNotFoundError, TimeoutExceededError
 
 _LOGGER = logging.getLogger(__name__)
 
+API_VERSION = "api/v1"
+
 
 class BboxRequests:
     """Class request."""
 
     def __init__(
         self,
-        hostname: str = None,
-        password: str = None,
-        timeout: str = 120,
-        session: aiohttp.ClientSession = None,
+        password: str,
+        hostname: str = "mabbox.bytel.fr",
+        timeout: int = 120,
+        session: ClientSession = None,
         use_tls: bool = True,
     ) -> None:
         """Initialize."""
-        self.hostname = hostname or "mabbox.bytel.fr"
         self.password = password
-        self.needs_auth = self.password is not None
-
-        self._session = session or aiohttp.ClientSession()
+        self._session = session
         self._timeout = timeout
         scheme = "https" if use_tls else "http"
-        self._uri = f"{scheme}://{self.hostname}/api"
+        self._uri = f"{scheme}://{hostname}/{API_VERSION}"
 
-    async def async_request(
-        self,
-        method: str,
-        service: str,
-        data: Any | None = None,
-        retry: bool = False,
-        **kwargs: Any,
-    ) -> Any:
+    async def async_request(self, path: str, method: str = "get", **kwargs: Any) -> Any:
         """Request url with method."""
         try:
-            url = f"{self._uri}/{service}"
-            _LOGGER.debug("%s %s %s", method, url, data)
-            if method == "post":
+            url = f"{self._uri}/{path}"
+
+            if path not in ["login", "device/token"]:
                 token = await self.async_get_token()
                 url = f"{url}?btoken={token}"
 
-            async with async_timeout.timeout(self._timeout):
-                response = await self._session.request(method, url, data=data, **kwargs)
-
+            async with asyncio.timeout(self._timeout):
+                _LOGGER.debug("Request: %s (%s) - %s", url, method, kwargs.get("json"))
+                response = await self._session.request(method, url, **kwargs)
+                contents = (await response.read()).decode("utf8")
         except (asyncio.CancelledError, asyncio.TimeoutError) as error:
             raise TimeoutExceededError(
                 "Timeout occurred while connecting to Bbox."
             ) from error
-        except (aiohttp.ClientError, socket.gaierror) as error:
+        except ClientResponseError:
+            if "application/json" in response.headers.get("Content-Type", ""):
+                raise ServiceNotFoundError(response.status, json.loads(contents))
+            raise ServiceNotFoundError(response.status, contents)
+        except (ClientError, socket.gaierror) as error:
             raise HttpRequestError(
                 "Error occurred while communicating with Bbox router."
             ) from error
 
-        content_type = response.headers.get("Content-Type", "")
-        if response.status // 100 in [4, 5]:
-            if response.status == 401 and self.needs_auth:
-                await self.async_auth()
-                if retry is False:
-                    return await self.async_request(
-                        method, url, data, retry=True, **kwargs
-                    )
-
-            contents = await response.read()
-            response.close()
-            if content_type == "application/json":
-                raise ServiceNotFoundError(
-                    response.status, json.loads(contents.decode("utf8"))
-                )
-            raise ServiceNotFoundError(response.status, contents.decode("utf8"))
-
-        if "application/json" in content_type:
-            result = await response.json()
-            _LOGGER.debug("Json mode")
-            _LOGGER.debug(result)
-            return result
-
-        result = await response.text()
-        _LOGGER.debug("Text mode")
-        _LOGGER.debug(result)
-        return result
+        return (
+            await response.json()
+            if "application/json" in response.headers.get("Content-Type", "")
+            else await response.text()
+        )
 
-    async def async_auth(self) -> aiohttp.ClientResponse:
+    async def async_auth(self) -> ClientResponse:
         """Request authentication."""
         if not self.password:
             raise RuntimeError("No password provided!")
-        try:
-            result = await self._session.request(
-                "post", f"{self._url}/v1/login", data={"password": self.password}
-            )
-            if result.status != 200:
-                result.raise_for_status()
-        except (aiohttp.ClientError, socket.gaierror) as error:
-            raise HttpRequestError("Error occurred while authentication.") from error
+        await self.async_request("login", "post", json={"password": self.password})
 
     async def async_get_token(self) -> str:
         """Request token."""
-        result = await self.async_request("get", "v1/device/token")
-        return result["device"]["token"]
+        result = await self.async_request("device/token")
+        return cast(str, result["device"]["token"])
```

### Comparing `bboxpy-1.1.7/bboxpy/bbox.py` & `bboxpy-1.2.0/bboxpy/bbox.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """Bbox API."""
+
 from __future__ import annotations
 
 import inspect
-from typing import Self
+
+from aiohttp import ClientSession
 
 from . import api as Api
 from .auth import BboxRequests
 from .exceptions import AuthorizationError, BboxException
 
 
 class Bbox(BboxRequests):
     """API Bouygues Bbox router."""
 
     def __init__(
         self,
-        hostname: str = None,
-        password: str = None,
+        password: str,
+        hostname: str = "mabbox.bytel.fr",
         timeout: int = 120,
-        session=None,
+        session: ClientSession = ClientSession(),
         use_tls: bool = True,
     ) -> None:
         """Initialize."""
         super().__init__(hostname, password, timeout, session, use_tls)
         self._load_modules()
 
     def _load_modules(self) -> None:
@@ -35,17 +37,21 @@
         try:
             await self.async_auth()
         except BboxException as error:
             raise AuthorizationError(error) from error
 
     async def async_logout(self) -> None:
         """Logout."""
-        await self.async_request("post", "v1/logout")
+        await self.async_request("logout", "post")
 
-    async def __aenter__(self) -> Self:
-        """Async enter."""
+    async def async_close(self) -> None:
+        """Close the session."""
+        if self._session:
+            await self._session.close()
+
+    async def __aenter__(self) -> Bbox:
+        """Asynchronous enter."""
         return self
 
     async def __aexit__(self, *_exc_info: object) -> None:
         """Async exit."""
-        if self._session:
-            await self._session.close()
+        await self.async_close()
```

### Comparing `bboxpy-1.1.7/bboxpy.egg-info/PKG-INFO` & `bboxpy-1.2.0/bboxpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bboxpy
-Version: 1.1.7
+Version: 1.2.0
 Summary: Fetch data from bouygues bbox
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: bouygues,async,bbox
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bboxpy-1.1.7/bboxpy.egg-info/SOURCES.txt` & `bboxpy-1.2.0/bboxpy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-.flake8
 .gitignore
 .pre-commit-config.yaml
-.pylintrc
 LICENSE
 MANIFEST.in
 README.md
 example.py
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 .github/dependabot.yml
+.github/workflows/auto-approve.yml
 .github/workflows/lint.yml
 .github/workflows/pythonpublish.yml
 .github/workflows/release.yml
 .vscode/settings.json
 bboxpy/__init__.py
 bboxpy/auth.py
 bboxpy/bbox.py
```

### Comparing `bboxpy-1.1.7/example.py` & `bboxpy-1.2.0/example.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # create console handler and set level to debug
 ch = logging.StreamHandler()
 formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 ch.setFormatter(formatter)
 logger.addHandler(ch)
 
 
+# mypy: disable-error-code="attr-defined"
 async def async_main() -> None:
     """Instantiate Livebox class."""
     bbox = Bbox(password="xxxxx")
     try:
         await bbox.async_login()
     except (AuthorizationError, HttpRequestError) as err:
         logger.error(err)
```

### Comparing `bboxpy-1.1.7/pyproject.toml` & `bboxpy-1.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools","setuptools-scm","wheel"]
+requires = ["setuptools","setuptools-scm", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "bboxpy"
-version     = "1.1.7"
+dynamic     = ["version"]
 license     = {text = "GPL-3"}
 description = "Fetch data from bouygues bbox"
 readme      = "README.md"
 authors     = [
     {name = "Cyr-ius", email = "cyr-ius@ipocus.net"}
 ]
 keywords    = ["bouygues", "async", "bbox"]
@@ -32,18 +32,14 @@
 [tool.setuptools_scm]
 
 [tool.setuptools]
 platforms = ["any"]
 zip-safe  = false
 include-package-data = true
 
-[tool.ruff.flake8-pytest-style]
+[tool.ruff.lint.flake8-pytest-style]
 fixture-parentheses = false
 
-[tool.ruff.flake8-tidy-imports.banned-api]
-"async_timeout".msg = "use asyncio.timeout instead"
-"pytz".msg = "use zoneinfo instead"
-
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 force-sort-within-sections = true
 combine-as-imports = true
 split-on-trailing-comma = false
```

