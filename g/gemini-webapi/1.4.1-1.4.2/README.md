# Comparing `tmp/gemini_webapi-1.4.1.tar.gz` & `tmp/gemini_webapi-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemini_webapi-1.4.1.tar", last modified: Sat May 25 23:13:31 2024, max compression
+gzip compressed data, was "gemini_webapi-1.4.2.tar", last modified: Sun May 26 02:56:08 2024, max compression
```

## Comparing `gemini_webapi-1.4.1.tar` & `gemini_webapi-1.4.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:13:31.522483 gemini_webapi-1.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:13:31.514484 gemini_webapi-1.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:13:31.514484 gemini_webapi-1.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/.github/workflows/github-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:13:31.514484 gemini_webapi-1.4.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    55249 2024-05-25 23:13:31.518483 gemini_webapi-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14677 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:13:31.514484 gemini_webapi-1.4.1/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   149995 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/assets/banner.png
--rw-r--r--   0 runner    (1001) docker     (127)    17780 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/assets/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 23:13:31.522483 gemini_webapi-1.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:13:31.514484 gemini_webapi-1.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:13:31.518483 gemini_webapi-1.4.1/src/gemini_webapi/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20882 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:13:31.518483 gemini_webapi-1.4.1/src/gemini_webapi/types/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/types/candidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/types/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/types/modeloutput.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:13:31.518483 gemini_webapi-1.4.1/src/gemini_webapi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/utils/get_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/utils/load_browser_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/utils/rotate_1psidts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/utils/upload_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:13:31.518483 gemini_webapi-1.4.1/src/gemini_webapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    55249 2024-05-25 23:13:31.000000 gemini_webapi-1.4.1/src/gemini_webapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-25 23:13:31.000000 gemini_webapi-1.4.1/src/gemini_webapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 23:13:31.000000 gemini_webapi-1.4.1/src/gemini_webapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-25 23:13:31.000000 gemini_webapi-1.4.1/src/gemini_webapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-25 23:13:31.000000 gemini_webapi-1.4.1/src/gemini_webapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:13:31.518483 gemini_webapi-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/tests/test_client_features.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/tests/test_rotate_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/tests/test_save_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:56:08.013870 gemini_webapi-1.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:56:08.005870 gemini_webapi-1.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:56:08.009870 gemini_webapi-1.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/.github/workflows/github-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:56:08.009870 gemini_webapi-1.4.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    55249 2024-05-26 02:56:08.013870 gemini_webapi-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14677 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:56:08.009870 gemini_webapi-1.4.2/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   149995 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/assets/banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17780 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/assets/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 02:56:08.013870 gemini_webapi-1.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:56:08.005870 gemini_webapi-1.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:56:08.009870 gemini_webapi-1.4.2/src/gemini_webapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/src/gemini_webapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20882 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/src/gemini_webapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/src/gemini_webapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/src/gemini_webapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:56:08.013870 gemini_webapi-1.4.2/src/gemini_webapi/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/src/gemini_webapi/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/src/gemini_webapi/types/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/src/gemini_webapi/types/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/src/gemini_webapi/types/modeloutput.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:56:08.013870 gemini_webapi-1.4.2/src/gemini_webapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/src/gemini_webapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/src/gemini_webapi/utils/get_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/src/gemini_webapi/utils/load_browser_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/src/gemini_webapi/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/src/gemini_webapi/utils/rotate_1psidts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/src/gemini_webapi/utils/upload_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:56:08.013870 gemini_webapi-1.4.2/src/gemini_webapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55249 2024-05-26 02:56:07.000000 gemini_webapi-1.4.2/src/gemini_webapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-26 02:56:08.000000 gemini_webapi-1.4.2/src/gemini_webapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 02:56:07.000000 gemini_webapi-1.4.2/src/gemini_webapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-26 02:56:07.000000 gemini_webapi-1.4.2/src/gemini_webapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-26 02:56:07.000000 gemini_webapi-1.4.2/src/gemini_webapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:56:08.013870 gemini_webapi-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/tests/test_client_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/tests/test_rotate_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-26 02:55:56.000000 gemini_webapi-1.4.2/tests/test_save_image.py
```

### Comparing `gemini_webapi-1.4.1/.github/workflows/pypi-publish.yml` & `gemini_webapi-1.4.2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.1/.gitignore` & `gemini_webapi-1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.1/LICENSE` & `gemini_webapi-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.1/PKG-INFO` & `gemini_webapi-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini-webapi
-Version: 1.4.1
+Version: 1.4.2
 Summary: ✨ An elegant async Python wrapper for Google Gemini web app
 Author: UZQueen
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `gemini_webapi-1.4.1/README.md` & `gemini_webapi-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.1/assets/banner.png` & `gemini_webapi-1.4.2/assets/banner.png`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.1/assets/favicon.png` & `gemini_webapi-1.4.2/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.1/assets/logo.svg` & `gemini_webapi-1.4.2/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.1/pyproject.toml` & `gemini_webapi-1.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.1/src/gemini_webapi/client.py` & `gemini_webapi-1.4.2/src/gemini_webapi/client.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.1/src/gemini_webapi/constants.py` & `gemini_webapi-1.4.2/src/gemini_webapi/constants.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.1/src/gemini_webapi/exceptions.py` & `gemini_webapi-1.4.2/src/gemini_webapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.1/src/gemini_webapi/types/candidate.py` & `gemini_webapi-1.4.2/src/gemini_webapi/types/candidate.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.1/src/gemini_webapi/types/image.py` & `gemini_webapi-1.4.2/src/gemini_webapi/types/image.py`

 * *Files 10% similar despite different names*

```diff
@@ -132,25 +132,30 @@
         if len(v) == 0:
             raise ValueError(
                 "GeneratedImage is designed to be initialized with same cookies as GeminiClient."
             )
         return v
 
     # @override
-    async def save(self, **kwargs) -> None:
+    async def save(self, **kwargs) -> str | None:
         """
         Save the image to disk.
 
         Parameters
         ----------
         filename: `str`, optional
             Filename to save the image, generated images are always in .png format, but file extension will not be included in the URL.
             And since the URL ends with a long hash, by default will use timestamp + end of the hash as the filename.
         kwargs: `dict`, optional
             Other arguments to pass to `Image.save`.
+
+        Returns
+        -------
+        `str | None`
+            Absolute path of the saved image if successfully saved.
         """
-        await super().save(
+        return await super().save(
             filename=kwargs.pop("filename", None)
             or f"{datetime.now().strftime('%Y%m%d%H%M%S')}_{self.url[-10:]}.png",
             cookies=self.cookies,
             **kwargs,
         )
```

### Comparing `gemini_webapi-1.4.1/src/gemini_webapi/types/modeloutput.py` & `gemini_webapi-1.4.2/src/gemini_webapi/types/modeloutput.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.1/src/gemini_webapi/utils/get_access_token.py` & `gemini_webapi-1.4.2/src/gemini_webapi/utils/get_access_token.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.1/src/gemini_webapi/utils/load_browser_cookies.py` & `gemini_webapi-1.4.2/src/gemini_webapi/utils/load_browser_cookies.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.1/src/gemini_webapi/utils/logger.py` & `gemini_webapi-1.4.2/src/gemini_webapi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.1/src/gemini_webapi/utils/rotate_1psidts.py` & `gemini_webapi-1.4.2/src/gemini_webapi/utils/rotate_1psidts.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.1/src/gemini_webapi/utils/upload_file.py` & `gemini_webapi-1.4.2/src/gemini_webapi/utils/upload_file.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.1/src/gemini_webapi.egg-info/PKG-INFO` & `gemini_webapi-1.4.2/src/gemini_webapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini-webapi
-Version: 1.4.1
+Version: 1.4.2
 Summary: ✨ An elegant async Python wrapper for Google Gemini web app
 Author: UZQueen
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `gemini_webapi-1.4.1/src/gemini_webapi.egg-info/SOURCES.txt` & `gemini_webapi-1.4.2/src/gemini_webapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.1/tests/test_client_features.py` & `gemini_webapi-1.4.2/tests/test_client_features.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.1/tests/test_rotate_cookies.py` & `gemini_webapi-1.4.2/tests/test_rotate_cookies.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.1/tests/test_save_image.py` & `gemini_webapi-1.4.2/tests/test_save_image.py`

 * *Files identical despite different names*

