# Comparing `tmp/pyodide_build-0.26.0a5.tar.gz` & `tmp/pyodide_build-0.26.0a6.tar.gz`

## Comparing `pyodide_build-0.26.0a5.tar` & `pyodide_build-0.26.0a6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/__init__.py
--rw-r--r--   0        0        0    21297 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/_f2c_fixes.py
--rw-r--r--   0        0        0    11764 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/_py_compile.py
--rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/bash_runner.py
--rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/build_env.py
--rwxr-xr-x   0        0        0    30967 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/buildall.py
--rwxr-xr-x   0        0        0    24052 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/buildpkg.py
--rw-r--r--   0        0        0    12643 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/common.py
--rw-r--r--   0        0        0     6920 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/config.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/create_package_index.py
--rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/create_xbuildenv.py
--rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/io.py
--rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/logger.py
--rwxr-xr-x   0        0        0     8707 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/mkpkg.py
--rw-r--r--   0        0        0     9904 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/pypabuild.py
--rwxr-xr-x   0        0        0    19753 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/pywasmcross.py
--rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/pyzip.py
--rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/recipe.py
--rw-r--r--   0        0        0    11605 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/xbuildenv.py
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/xbuildenv_releases.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/cli/__init__.py
--rw-r--r--   0        0        0    10069 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/cli/build.py
--rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/cli/build_recipes.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/cli/config.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/cli/create_zipfile.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/cli/py_compile.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/cli/skeleton.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/cli/venv.py
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/cli/xbuildenv.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/out_of_tree/__init__.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/out_of_tree/build.py
--rw-r--r--   0        0        0    15500 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/out_of_tree/pypi.py
--rw-r--r--   0        0        0     9604 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/out_of_tree/venv.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/tools/emscripten.meson.cross
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/tools/pyo3_config.ini
--rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake
--rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/vendor/_pypabuild.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/LICENSE
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/README.md
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyproject.toml
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/__init__.py
+-rw-r--r--   0        0        0    21297 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/_f2c_fixes.py
+-rw-r--r--   0        0        0    11764 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/_py_compile.py
+-rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/bash_runner.py
+-rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/build_env.py
+-rwxr-xr-x   0        0        0    30967 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/buildall.py
+-rwxr-xr-x   0        0        0    24052 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/buildpkg.py
+-rw-r--r--   0        0        0    12660 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/common.py
+-rw-r--r--   0        0        0     6920 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/config.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/create_package_index.py
+-rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/create_xbuildenv.py
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/io.py
+-rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/logger.py
+-rwxr-xr-x   0        0        0     8707 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/mkpkg.py
+-rw-r--r--   0        0        0     9904 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/pypabuild.py
+-rwxr-xr-x   0        0        0    19753 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/pywasmcross.py
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/pyzip.py
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/recipe.py
+-rw-r--r--   0        0        0    11605 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/xbuildenv.py
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/xbuildenv_releases.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/cli/__init__.py
+-rw-r--r--   0        0        0    10069 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/cli/build.py
+-rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/cli/build_recipes.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/cli/config.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/cli/create_zipfile.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/cli/py_compile.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/cli/skeleton.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/cli/venv.py
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/cli/xbuildenv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/out_of_tree/__init__.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/out_of_tree/build.py
+-rw-r--r--   0        0        0    15500 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/out_of_tree/pypi.py
+-rw-r--r--   0        0        0     9604 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/out_of_tree/venv.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/tools/emscripten.meson.cross
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/tools/pyo3_config.ini
+-rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake
+-rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyodide_build/vendor/_pypabuild.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/LICENSE
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/README.md
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/pyproject.toml
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a6/PKG-INFO
```

### Comparing `pyodide_build-0.26.0a5/pyodide_build/_f2c_fixes.py` & `pyodide_build-0.26.0a6/pyodide_build/_f2c_fixes.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/_py_compile.py` & `pyodide_build-0.26.0a6/pyodide_build/_py_compile.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/bash_runner.py` & `pyodide_build-0.26.0a6/pyodide_build/bash_runner.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/build_env.py` & `pyodide_build-0.26.0a6/pyodide_build/build_env.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/buildall.py` & `pyodide_build-0.26.0a6/pyodide_build/buildall.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/buildpkg.py` & `pyodide_build-0.26.0a6/pyodide_build/buildpkg.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/common.py` & `pyodide_build-0.26.0a6/pyodide_build/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,15 +345,15 @@
         check=False,
         encoding="utf-8",
         capture_output=True,
     )
     if result.returncode != 0:
         logger.error(f"ERROR: Retagging wheel {wheel_path} to {platform} failed")
         exit_with_stdio(result)
-    return wheel_path.parent / result.stdout.strip()
+    return wheel_path.parent / result.stdout.splitlines()[-1].strip()
 
 
 def extract_wheel_metadata_file(wheel_path: Path, output_path: Path) -> None:
     """Extracts the METADATA file from the given wheel and writes it to the
     output path.
 
     Raises a RuntimeError if the METADATA file does not exist.
```

### Comparing `pyodide_build-0.26.0a5/pyodide_build/config.py` & `pyodide_build-0.26.0a6/pyodide_build/config.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/create_package_index.py` & `pyodide_build-0.26.0a6/pyodide_build/create_package_index.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/create_xbuildenv.py` & `pyodide_build-0.26.0a6/pyodide_build/create_xbuildenv.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/io.py` & `pyodide_build-0.26.0a6/pyodide_build/io.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/logger.py` & `pyodide_build-0.26.0a6/pyodide_build/logger.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/mkpkg.py` & `pyodide_build-0.26.0a6/pyodide_build/mkpkg.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/pypabuild.py` & `pyodide_build-0.26.0a6/pyodide_build/pypabuild.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/pywasmcross.py` & `pyodide_build-0.26.0a6/pyodide_build/pywasmcross.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/pyzip.py` & `pyodide_build-0.26.0a6/pyodide_build/pyzip.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/recipe.py` & `pyodide_build-0.26.0a6/pyodide_build/recipe.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/xbuildenv.py` & `pyodide_build-0.26.0a6/pyodide_build/xbuildenv.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/xbuildenv_releases.py` & `pyodide_build-0.26.0a6/pyodide_build/xbuildenv_releases.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/cli/build.py` & `pyodide_build-0.26.0a6/pyodide_build/cli/build.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/cli/build_recipes.py` & `pyodide_build-0.26.0a6/pyodide_build/cli/build_recipes.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/cli/config.py` & `pyodide_build-0.26.0a6/pyodide_build/cli/config.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/cli/create_zipfile.py` & `pyodide_build-0.26.0a6/pyodide_build/cli/create_zipfile.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/cli/py_compile.py` & `pyodide_build-0.26.0a6/pyodide_build/cli/py_compile.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/cli/skeleton.py` & `pyodide_build-0.26.0a6/pyodide_build/cli/skeleton.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/cli/xbuildenv.py` & `pyodide_build-0.26.0a6/pyodide_build/cli/xbuildenv.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/out_of_tree/build.py` & `pyodide_build-0.26.0a6/pyodide_build/out_of_tree/build.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from pathlib import Path
 
 from build import ConfigSettingsType
 
 from .. import build_env, common, pypabuild
-from ..build_env import get_pyodide_root
+from ..build_env import get_pyodide_root, wheel_platform
 from ..io import _BuildSpecExports
 
 
 def run(
     srcdir: Path,
     outdir: Path,
     exports: _BuildSpecExports,
@@ -37,11 +37,12 @@
         exports=exports,
     )
 
     with build_env_ctx as env:
         built_wheel = pypabuild.build(srcdir, outdir, env, config_settings)
 
     wheel_path = Path(built_wheel)
+    wheel_path = common.retag_wheel(wheel_path, wheel_platform())
     with common.modify_wheel(wheel_path) as wheel_dir:
         build_env.replace_so_abi_tags(wheel_dir)
 
     return wheel_path
```

### Comparing `pyodide_build-0.26.0a5/pyodide_build/out_of_tree/pypi.py` & `pyodide_build-0.26.0a6/pyodide_build/out_of_tree/pypi.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/out_of_tree/venv.py` & `pyodide_build-0.26.0a6/pyodide_build/out_of_tree/venv.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake` & `pyodide_build-0.26.0a6/pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyodide_build/vendor/_pypabuild.py` & `pyodide_build-0.26.0a6/pyodide_build/vendor/_pypabuild.py`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/LICENSE` & `pyodide_build-0.26.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/pyproject.toml` & `pyodide_build-0.26.0a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyodide_build-0.26.0a5/PKG-INFO` & `pyodide_build-0.26.0a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyodide-build
-Version: 0.26.0a5
+Version: 0.26.0a6
 Summary: "Tools for building Pyodide"
 Project-URL: Homepage, https://github.com/pyodide/pyodide
 Project-URL: Bug Tracker, https://github.com/pyodide/pyodide/issues
 Project-URL: Documentation, https://pyodide.org/en/stable/
 Author: Pyodide developers
 License: MPL-2.0
 License-File: LICENSE
```

