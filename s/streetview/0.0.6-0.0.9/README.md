# Comparing `tmp/streetview-0.0.6.tar.gz` & `tmp/streetview-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streetview-0.0.6.tar", last modified: Sun Jul 23 17:28:00 2023, max compression
+gzip compressed data, was "streetview-0.0.9.tar", last modified: Mon May 27 10:50:37 2024, max compression
```

## Comparing `streetview-0.0.6.tar` & `streetview-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 17:28:00.188691 streetview-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-23 17:27:41.000000 streetview-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-23 17:28:00.188691 streetview-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-23 17:27:41.000000 streetview-0.0.6/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 17:28:00.188691 streetview-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-23 17:27:41.000000 streetview-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 17:28:00.188691 streetview-0.0.6/streetview/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-23 17:27:41.000000 streetview-0.0.6/streetview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-23 17:27:41.000000 streetview-0.0.6/streetview/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-23 17:27:41.000000 streetview-0.0.6/streetview/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-23 17:27:41.000000 streetview-0.0.6/streetview/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 17:28:00.188691 streetview-0.0.6/streetview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-23 17:28:00.000000 streetview-0.0.6/streetview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-23 17:28:00.000000 streetview-0.0.6/streetview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 17:28:00.000000 streetview-0.0.6/streetview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 17:28:00.000000 streetview-0.0.6/streetview.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-23 17:28:00.000000 streetview-0.0.6/streetview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-23 17:28:00.000000 streetview-0.0.6/streetview.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 17:28:00.188691 streetview-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-23 17:27:41.000000 streetview-0.0.6/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-23 17:27:41.000000 streetview-0.0.6/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-23 17:27:41.000000 streetview-0.0.6/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-23 17:27:42.000000 streetview-0.0.6/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:37.939720 streetview-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-27 10:50:30.000000 streetview-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-27 10:50:37.939720 streetview-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-27 10:50:30.000000 streetview-0.0.9/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 10:50:37.939720 streetview-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-27 10:50:30.000000 streetview-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:37.935720 streetview-0.0.9/streetview/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-27 10:50:30.000000 streetview-0.0.9/streetview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-27 10:50:30.000000 streetview-0.0.9/streetview/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-05-27 10:50:30.000000 streetview-0.0.9/streetview/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-27 10:50:30.000000 streetview-0.0.9/streetview/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:37.939720 streetview-0.0.9/streetview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-27 10:50:37.000000 streetview-0.0.9/streetview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-27 10:50:37.000000 streetview-0.0.9/streetview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 10:50:37.000000 streetview-0.0.9/streetview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 10:50:37.000000 streetview-0.0.9/streetview.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-27 10:50:37.000000 streetview-0.0.9/streetview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 10:50:37.000000 streetview-0.0.9/streetview.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:37.939720 streetview-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-27 10:50:30.000000 streetview-0.0.9/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-27 10:50:30.000000 streetview-0.0.9/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-27 10:50:30.000000 streetview-0.0.9/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-27 10:50:30.000000 streetview-0.0.9/version.py
```

### Comparing `streetview-0.0.6/PKG-INFO` & `streetview-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: streetview
-Version: 0.0.6
+Version: 0.0.9
 Summary: Retrieve current and historical photos from Google Street View
 Home-page: https://github.com/robolyst/streetview
 Author: Adrian Letchford
 Author-email: me@dradrian.com
 License: MIT
 Description-Content-Type: text/markdown
+Requires-Dist: requests
+Requires-Dist: pillow
+Requires-Dist: pydantic
+Requires-Dist: httpx
 
 # streetview
 
 This is a light module for downloading photos from Google street view. The
 functions allow you to retrieve current and **old** photos. Google does have an
 API for accessing Street View. However, it does not allow you to access old
 photos. Their javascript API allows you to download segments of current photos.
@@ -68,14 +72,24 @@
     pano_id="z80QZ1_QgCbYwj7RrmlS0Q",
     api_key=GOOGLE_MAPS_API_KEY,
 )
 
 image.save("image.jpg", "jpeg")
 ```
 
+To download the panorama in an asynchronous context:
+
+```python
+from streetview import get_panorama_async
+
+image = await get_panorama_async(pano_id="z80QZ1_QgCbYwj7RrmlS0Q")
+
+image.save("image.jpg", "jpeg")
+```
+
 ## Download panorama
 
 You can download a full panorama like this:
 
 ```python
 from streetview import get_panorama
```

### Comparing `streetview-0.0.6/readme.md` & `streetview-0.0.9/readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,24 @@
     pano_id="z80QZ1_QgCbYwj7RrmlS0Q",
     api_key=GOOGLE_MAPS_API_KEY,
 )
 
 image.save("image.jpg", "jpeg")
 ```
 
+To download the panorama in an asynchronous context:
+
+```python
+from streetview import get_panorama_async
+
+image = await get_panorama_async(pano_id="z80QZ1_QgCbYwj7RrmlS0Q")
+
+image.save("image.jpg", "jpeg")
+```
+
 ## Download panorama
 
 You can download a full panorama like this:
 
 ```python
 from streetview import get_panorama
```

### Comparing `streetview-0.0.6/setup.py` & `streetview-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,9 +20,10 @@
     license="MIT",
     packages=["streetview"],
     zip_safe=False,
     install_requires=[
         "requests",
         "pillow",
         "pydantic",
+        "httpx"
     ],
 )
```

### Comparing `streetview-0.0.6/streetview/api.py` & `streetview-0.0.9/streetview/api.py`

 * *Files identical despite different names*

### Comparing `streetview-0.0.6/streetview/search.py` & `streetview-0.0.9/streetview/search.py`

 * *Files identical despite different names*

### Comparing `streetview-0.0.6/streetview.egg-info/PKG-INFO` & `streetview-0.0.9/streetview.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: streetview
-Version: 0.0.6
+Version: 0.0.9
 Summary: Retrieve current and historical photos from Google Street View
 Home-page: https://github.com/robolyst/streetview
 Author: Adrian Letchford
 Author-email: me@dradrian.com
 License: MIT
 Description-Content-Type: text/markdown
+Requires-Dist: requests
+Requires-Dist: pillow
+Requires-Dist: pydantic
+Requires-Dist: httpx
 
 # streetview
 
 This is a light module for downloading photos from Google street view. The
 functions allow you to retrieve current and **old** photos. Google does have an
 API for accessing Street View. However, it does not allow you to access old
 photos. Their javascript API allows you to download segments of current photos.
@@ -68,14 +72,24 @@
     pano_id="z80QZ1_QgCbYwj7RrmlS0Q",
     api_key=GOOGLE_MAPS_API_KEY,
 )
 
 image.save("image.jpg", "jpeg")
 ```
 
+To download the panorama in an asynchronous context:
+
+```python
+from streetview import get_panorama_async
+
+image = await get_panorama_async(pano_id="z80QZ1_QgCbYwj7RrmlS0Q")
+
+image.save("image.jpg", "jpeg")
+```
+
 ## Download panorama
 
 You can download a full panorama like this:
 
 ```python
 from streetview import get_panorama
```

### Comparing `streetview-0.0.6/tests/test_api.py` & `streetview-0.0.9/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `streetview-0.0.6/tests/test_download.py` & `streetview-0.0.9/tests/test_download.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import hashlib
 from io import BytesIO
 
 import pytest
 from PIL import Image
 
-from streetview import get_panorama
+from streetview import get_panorama, get_panorama_async
 from streetview.download import (
     TileInfo,
     fetch_panorama_tile,
     get_width_and_height_from_zoom,
     iter_tile_info,
     iter_tiles,
     make_download_url,
@@ -77,7 +77,20 @@
     next(tiles)
 
 
 @pytest.mark.vcr()
 def test_that_panorama_downloads_successfully():
     image = get_panorama(pano_id="z80QZ1_QgCbYwj7RrmlS0Q", zoom=1)
     image.save("image.jpg", "jpeg")
+
+
+@pytest.mark.vcr()
+def test_that_panorama_downloads_successfully_multi_threaded():
+    image = get_panorama(pano_id="z80QZ1_QgCbYwj7RrmlS0Q", zoom=1, multi_threaded=True)
+    image.save("image.jpg", "jpeg")
+
+
+@pytest.mark.asyncio
+@pytest.mark.vcr()
+async def test_that_panorama_downloads_successfully_async():
+    image = await get_panorama_async(pano_id="z80QZ1_QgCbYwj7RrmlS0Q", zoom=1)
+    image.save("image.jpg", "jpeg")
```

### Comparing `streetview-0.0.6/tests/test_search.py` & `streetview-0.0.9/tests/test_search.py`

 * *Files identical despite different names*

