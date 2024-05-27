# Comparing `tmp/hn-sdk-0.1.0.tar.gz` & `tmp/hn-sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hn-sdk-0.1.0.tar", last modified: Wed Feb 21 02:14:13 2024, max compression
+gzip compressed data, was "hn-sdk-0.1.1.tar", last modified: Mon May 27 21:39:53 2024, max compression
```

## Comparing `hn-sdk-0.1.0.tar` & `hn-sdk-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 joeyagreco   (501) staff       (20)        0 2024-02-21 02:14:13.344808 hn-sdk-0.1.0/
--rw-r--r--   0 joeyagreco   (501) staff       (20)     1067 2024-02-20 01:50:25.000000 hn-sdk-0.1.0/LICENSE
--rw-r--r--   0 joeyagreco   (501) staff       (20)       24 2024-02-20 01:54:16.000000 hn-sdk-0.1.0/MANIFEST.in
--rw-r--r--   0 joeyagreco   (501) staff       (20)     8048 2024-02-21 02:14:13.344705 hn-sdk-0.1.0/PKG-INFO
--rw-r--r--   0 joeyagreco   (501) staff       (20)     7702 2024-02-20 06:01:34.000000 hn-sdk-0.1.0/README.md
-drwxr-xr-x   0 joeyagreco   (501) staff       (20)        0 2024-02-21 02:14:13.343389 hn-sdk-0.1.0/hn_sdk/
--rw-r--r--   0 joeyagreco   (501) staff       (20)        0 2024-02-20 02:49:55.000000 hn-sdk-0.1.0/hn_sdk/__init__.py
--rw-r--r--   0 joeyagreco   (501) staff       (20)       94 2024-02-21 02:13:19.000000 hn-sdk-0.1.0/hn_sdk/_version.py
-drwxr-xr-x   0 joeyagreco   (501) staff       (20)        0 2024-02-21 02:14:13.344036 hn-sdk-0.1.0/hn_sdk/client/
--rw-r--r--   0 joeyagreco   (501) staff       (20)        0 2024-02-20 02:39:32.000000 hn-sdk-0.1.0/hn_sdk/client/__init__.py
--rw-r--r--   0 joeyagreco   (501) staff       (20)      843 2024-02-20 02:55:36.000000 hn-sdk-0.1.0/hn_sdk/client/util.py
-drwxr-xr-x   0 joeyagreco   (501) staff       (20)        0 2024-02-21 02:14:13.344228 hn-sdk-0.1.0/hn_sdk/client/v0/
--rw-r--r--   0 joeyagreco   (501) staff       (20)        0 2024-02-20 02:48:21.000000 hn-sdk-0.1.0/hn_sdk/client/v0/__init__.py
--rw-r--r--   0 joeyagreco   (501) staff       (20)     4495 2024-02-21 01:27:17.000000 hn-sdk-0.1.0/hn_sdk/client/v0/client.py
-drwxr-xr-x   0 joeyagreco   (501) staff       (20)        0 2024-02-21 02:14:13.344462 hn-sdk-0.1.0/hn_sdk/util/
--rw-r--r--   0 joeyagreco   (501) staff       (20)     1158 2024-02-20 05:35:06.000000 hn-sdk-0.1.0/hn_sdk/util/ConfigReader.py
--rw-r--r--   0 joeyagreco   (501) staff       (20)        0 2024-02-20 05:26:18.000000 hn-sdk-0.1.0/hn_sdk/util/__init__.py
-drwxr-xr-x   0 joeyagreco   (501) staff       (20)        0 2024-02-21 02:14:13.343862 hn-sdk-0.1.0/hn_sdk.egg-info/
--rw-r--r--   0 joeyagreco   (501) staff       (20)     8048 2024-02-21 02:14:13.000000 hn-sdk-0.1.0/hn_sdk.egg-info/PKG-INFO
--rw-r--r--   0 joeyagreco   (501) staff       (20)      434 2024-02-21 02:14:13.000000 hn-sdk-0.1.0/hn_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 joeyagreco   (501) staff       (20)        1 2024-02-21 02:14:13.000000 hn-sdk-0.1.0/hn_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 joeyagreco   (501) staff       (20)       17 2024-02-21 02:14:13.000000 hn-sdk-0.1.0/hn_sdk.egg-info/requires.txt
--rw-r--r--   0 joeyagreco   (501) staff       (20)       16 2024-02-21 02:14:13.000000 hn-sdk-0.1.0/hn_sdk.egg-info/top_level.txt
--rw-r--r--   0 joeyagreco   (501) staff       (20)      257 2024-02-20 01:54:39.000000 hn-sdk-0.1.0/pyproject.toml
--rw-r--r--   0 joeyagreco   (501) staff       (20)       16 2024-02-20 04:49:04.000000 hn-sdk-0.1.0/requirements.txt
--rw-r--r--   0 joeyagreco   (501) staff       (20)       38 2024-02-21 02:14:13.344848 hn-sdk-0.1.0/setup.cfg
--rw-r--r--   0 joeyagreco   (501) staff       (20)      972 2024-02-20 04:54:29.000000 hn-sdk-0.1.0/setup.py
-drwxr-xr-x   0 joeyagreco   (501) staff       (20)        0 2024-02-21 02:14:13.344543 hn-sdk-0.1.0/test_e2e/
--rw-r--r--   0 joeyagreco   (501) staff       (20)        0 2024-02-20 04:04:52.000000 hn-sdk-0.1.0/test_e2e/__init__.py
+drwxr-xr-x   0 joeyagreco   (501) staff       (20)        0 2024-05-27 21:39:53.547363 hn-sdk-0.1.1/
+-rw-r--r--   0 joeyagreco   (501) staff       (20)     1067 2024-02-20 01:50:25.000000 hn-sdk-0.1.1/LICENSE
+-rw-r--r--   0 joeyagreco   (501) staff       (20)       50 2024-05-27 21:36:53.000000 hn-sdk-0.1.1/MANIFEST.in
+-rw-r--r--   0 joeyagreco   (501) staff       (20)     8081 2024-05-27 21:39:53.547264 hn-sdk-0.1.1/PKG-INFO
+-rw-r--r--   0 joeyagreco   (501) staff       (20)     7735 2024-05-27 21:32:07.000000 hn-sdk-0.1.1/README.md
+drwxr-xr-x   0 joeyagreco   (501) staff       (20)        0 2024-05-27 21:39:53.545804 hn-sdk-0.1.1/hn_sdk/
+-rw-r--r--   0 joeyagreco   (501) staff       (20)        0 2024-02-20 02:49:55.000000 hn-sdk-0.1.1/hn_sdk/__init__.py
+-rw-r--r--   0 joeyagreco   (501) staff       (20)       94 2024-05-27 21:37:03.000000 hn-sdk-0.1.1/hn_sdk/_version.py
+drwxr-xr-x   0 joeyagreco   (501) staff       (20)        0 2024-05-27 21:39:53.546519 hn-sdk-0.1.1/hn_sdk/client/
+-rw-r--r--   0 joeyagreco   (501) staff       (20)        0 2024-02-20 02:39:32.000000 hn-sdk-0.1.1/hn_sdk/client/__init__.py
+-rw-r--r--   0 joeyagreco   (501) staff       (20)      843 2024-02-20 02:55:36.000000 hn-sdk-0.1.1/hn_sdk/client/util.py
+drwxr-xr-x   0 joeyagreco   (501) staff       (20)        0 2024-05-27 21:39:53.546720 hn-sdk-0.1.1/hn_sdk/client/v0/
+-rw-r--r--   0 joeyagreco   (501) staff       (20)        0 2024-02-20 02:48:21.000000 hn-sdk-0.1.1/hn_sdk/client/v0/__init__.py
+-rw-r--r--   0 joeyagreco   (501) staff       (20)     4495 2024-02-21 01:27:17.000000 hn-sdk-0.1.1/hn_sdk/client/v0/client.py
+drwxr-xr-x   0 joeyagreco   (501) staff       (20)        0 2024-05-27 21:39:53.546825 hn-sdk-0.1.1/hn_sdk/property/
+-rw-r--r--   0 joeyagreco   (501) staff       (20)      317 2024-02-20 05:34:12.000000 hn-sdk-0.1.1/hn_sdk/property/client.properties
+drwxr-xr-x   0 joeyagreco   (501) staff       (20)        0 2024-05-27 21:39:53.547048 hn-sdk-0.1.1/hn_sdk/util/
+-rw-r--r--   0 joeyagreco   (501) staff       (20)     1158 2024-02-20 05:35:06.000000 hn-sdk-0.1.1/hn_sdk/util/ConfigReader.py
+-rw-r--r--   0 joeyagreco   (501) staff       (20)        0 2024-02-20 05:26:18.000000 hn-sdk-0.1.1/hn_sdk/util/__init__.py
+drwxr-xr-x   0 joeyagreco   (501) staff       (20)        0 2024-05-27 21:39:53.546331 hn-sdk-0.1.1/hn_sdk.egg-info/
+-rw-r--r--   0 joeyagreco   (501) staff       (20)     8081 2024-05-27 21:39:53.000000 hn-sdk-0.1.1/hn_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 joeyagreco   (501) staff       (20)      468 2024-05-27 21:39:53.000000 hn-sdk-0.1.1/hn_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 joeyagreco   (501) staff       (20)        1 2024-05-27 21:39:53.000000 hn-sdk-0.1.1/hn_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 joeyagreco   (501) staff       (20)       17 2024-05-27 21:39:53.000000 hn-sdk-0.1.1/hn_sdk.egg-info/requires.txt
+-rw-r--r--   0 joeyagreco   (501) staff       (20)       16 2024-05-27 21:39:53.000000 hn-sdk-0.1.1/hn_sdk.egg-info/top_level.txt
+-rw-r--r--   0 joeyagreco   (501) staff       (20)      257 2024-02-20 01:54:39.000000 hn-sdk-0.1.1/pyproject.toml
+-rw-r--r--   0 joeyagreco   (501) staff       (20)       16 2024-02-20 04:49:04.000000 hn-sdk-0.1.1/requirements.txt
+-rw-r--r--   0 joeyagreco   (501) staff       (20)       38 2024-05-27 21:39:53.547404 hn-sdk-0.1.1/setup.cfg
+-rw-r--r--   0 joeyagreco   (501) staff       (20)      968 2024-05-27 21:29:54.000000 hn-sdk-0.1.1/setup.py
+drwxr-xr-x   0 joeyagreco   (501) staff       (20)        0 2024-05-27 21:39:53.547139 hn-sdk-0.1.1/test_e2e/
+-rw-r--r--   0 joeyagreco   (501) staff       (20)        0 2024-02-20 04:04:52.000000 hn-sdk-0.1.1/test_e2e/__init__.py
```

### Comparing `hn-sdk-0.1.0/LICENSE` & `hn-sdk-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hn-sdk-0.1.0/PKG-INFO` & `hn-sdk-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hn-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python wrapper for the Hacker News API.
 Home-page: https://github.com/joeyagreco/hn-api
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: hacker-news hacker news api sdk
 Requires-Python: >=3.10
@@ -148,101 +148,101 @@
   "poll" : 160704,
   "score" : 335,
   "text" : "Yes, ban them; I'm tired of seeing Valleywag stories on News.YC.",
   "time" : 1207886576,
   "type" : "pollopt"
 }
 ```
-
+---
 ### Get a User by Username
 
 ```python
 from hn_sdk.client.v0.client import get_user_by_username
 
-print(get_item_by_id("joeyagreco"))
+print(get_user_by_username("joeyagreco"))
 ```
 ```sh
 {
     "created": 1663896930,
     "id": "joeyagreco",
     "karma": 4,
     "submitted": [38474886, 35729377, 35729231, 32946977, 32946976],
 }
 ```
-
+---
 ### Get Current Largest Item ID
 ```python
 from hn_sdk.client.v0.client import get_max_item_id
 
 print(get_max_item_id())
 ```
 ```sh
 39438426
 ```
-
+---
 ### Get New Stories
 ```python
 from hn_sdk.client.v0.client import get_new_stories
 
 print(get_new_stories())
 ```
 ```sh
 [ 39431573, 39431552, 39431514, 39431505, ..., 39432231 ]
 ```
-
+---
 ### Get Top Stories
 ```python
 from hn_sdk.client.v0.client import get_top_stories
 
 print(get_top_stories())
 ```
 ```sh
 [ 39396571, 39385098, 39387191, 39389092, ..., 39394528 ]
 ```
-
+---
 ### Get Best Stories
 ```python
 from hn_sdk.client.v0.client import get_best_stories
 
 print(get_best_stories())
 ```
 ```sh
 [ 39437424, 39418810, 39418102, 39422238, ..., 39402906 ]
 ```
-
+---
 ### Get Ask HN Stories
 ```python
 from hn_sdk.client.v0.client import get_ask_stories
 
 print(get_ask_stories())
 ```
 ```sh
 [ 39405805, 39405655, 39400290, 39398791,  ..., 39427773 ]
 ```
-
+---
 ### Get Show HN Stories
 ```python
 from hn_sdk.client.v0.client import get_show_stories
 
 print(get_show_stories())
 ```
 ```sh
 [ 39387382, 39403234, 39410058, 39391731,  ..., 39390544 ]
 ```
-
+---
 ### Get Job Stories
 ```python
 from hn_sdk.client.v0.client import get_job_stories
 
 print(get_job_stories())
 ```
 ```sh
 [ 39057748, 39040718, 39038845, 39019063,  ..., 39006337 ]
 ```
-
+---
 ### Get Changed Items and Profiles
 ```python
 from hn_sdk.client.v0.client import get_updates
 
 print(get_updates())
 ```
 ```sh
```

### Comparing `hn-sdk-0.1.0/README.md` & `hn-sdk-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -135,101 +135,101 @@
   "poll" : 160704,
   "score" : 335,
   "text" : "Yes, ban them; I'm tired of seeing Valleywag stories on News.YC.",
   "time" : 1207886576,
   "type" : "pollopt"
 }
 ```
-
+---
 ### Get a User by Username
 
 ```python
 from hn_sdk.client.v0.client import get_user_by_username
 
-print(get_item_by_id("joeyagreco"))
+print(get_user_by_username("joeyagreco"))
 ```
 ```sh
 {
     "created": 1663896930,
     "id": "joeyagreco",
     "karma": 4,
     "submitted": [38474886, 35729377, 35729231, 32946977, 32946976],
 }
 ```
-
+---
 ### Get Current Largest Item ID
 ```python
 from hn_sdk.client.v0.client import get_max_item_id
 
 print(get_max_item_id())
 ```
 ```sh
 39438426
 ```
-
+---
 ### Get New Stories
 ```python
 from hn_sdk.client.v0.client import get_new_stories
 
 print(get_new_stories())
 ```
 ```sh
 [ 39431573, 39431552, 39431514, 39431505, ..., 39432231 ]
 ```
-
+---
 ### Get Top Stories
 ```python
 from hn_sdk.client.v0.client import get_top_stories
 
 print(get_top_stories())
 ```
 ```sh
 [ 39396571, 39385098, 39387191, 39389092, ..., 39394528 ]
 ```
-
+---
 ### Get Best Stories
 ```python
 from hn_sdk.client.v0.client import get_best_stories
 
 print(get_best_stories())
 ```
 ```sh
 [ 39437424, 39418810, 39418102, 39422238, ..., 39402906 ]
 ```
-
+---
 ### Get Ask HN Stories
 ```python
 from hn_sdk.client.v0.client import get_ask_stories
 
 print(get_ask_stories())
 ```
 ```sh
 [ 39405805, 39405655, 39400290, 39398791,  ..., 39427773 ]
 ```
-
+---
 ### Get Show HN Stories
 ```python
 from hn_sdk.client.v0.client import get_show_stories
 
 print(get_show_stories())
 ```
 ```sh
 [ 39387382, 39403234, 39410058, 39391731,  ..., 39390544 ]
 ```
-
+---
 ### Get Job Stories
 ```python
 from hn_sdk.client.v0.client import get_job_stories
 
 print(get_job_stories())
 ```
 ```sh
 [ 39057748, 39040718, 39038845, 39019063,  ..., 39006337 ]
 ```
-
+---
 ### Get Changed Items and Profiles
 ```python
 from hn_sdk.client.v0.client import get_updates
 
 print(get_updates())
 ```
 ```sh
```

### Comparing `hn-sdk-0.1.0/hn_sdk/client/util.py` & `hn-sdk-0.1.1/hn_sdk/client/util.py`

 * *Files identical despite different names*

### Comparing `hn-sdk-0.1.0/hn_sdk/client/v0/client.py` & `hn-sdk-0.1.1/hn_sdk/client/v0/client.py`

 * *Files identical despite different names*

### Comparing `hn-sdk-0.1.0/hn_sdk/util/ConfigReader.py` & `hn-sdk-0.1.1/hn_sdk/util/ConfigReader.py`

 * *Files identical despite different names*

### Comparing `hn-sdk-0.1.0/hn_sdk.egg-info/PKG-INFO` & `hn-sdk-0.1.1/hn_sdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hn-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python wrapper for the Hacker News API.
 Home-page: https://github.com/joeyagreco/hn-api
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: hacker-news hacker news api sdk
 Requires-Python: >=3.10
@@ -148,101 +148,101 @@
   "poll" : 160704,
   "score" : 335,
   "text" : "Yes, ban them; I'm tired of seeing Valleywag stories on News.YC.",
   "time" : 1207886576,
   "type" : "pollopt"
 }
 ```
-
+---
 ### Get a User by Username
 
 ```python
 from hn_sdk.client.v0.client import get_user_by_username
 
-print(get_item_by_id("joeyagreco"))
+print(get_user_by_username("joeyagreco"))
 ```
 ```sh
 {
     "created": 1663896930,
     "id": "joeyagreco",
     "karma": 4,
     "submitted": [38474886, 35729377, 35729231, 32946977, 32946976],
 }
 ```
-
+---
 ### Get Current Largest Item ID
 ```python
 from hn_sdk.client.v0.client import get_max_item_id
 
 print(get_max_item_id())
 ```
 ```sh
 39438426
 ```
-
+---
 ### Get New Stories
 ```python
 from hn_sdk.client.v0.client import get_new_stories
 
 print(get_new_stories())
 ```
 ```sh
 [ 39431573, 39431552, 39431514, 39431505, ..., 39432231 ]
 ```
-
+---
 ### Get Top Stories
 ```python
 from hn_sdk.client.v0.client import get_top_stories
 
 print(get_top_stories())
 ```
 ```sh
 [ 39396571, 39385098, 39387191, 39389092, ..., 39394528 ]
 ```
-
+---
 ### Get Best Stories
 ```python
 from hn_sdk.client.v0.client import get_best_stories
 
 print(get_best_stories())
 ```
 ```sh
 [ 39437424, 39418810, 39418102, 39422238, ..., 39402906 ]
 ```
-
+---
 ### Get Ask HN Stories
 ```python
 from hn_sdk.client.v0.client import get_ask_stories
 
 print(get_ask_stories())
 ```
 ```sh
 [ 39405805, 39405655, 39400290, 39398791,  ..., 39427773 ]
 ```
-
+---
 ### Get Show HN Stories
 ```python
 from hn_sdk.client.v0.client import get_show_stories
 
 print(get_show_stories())
 ```
 ```sh
 [ 39387382, 39403234, 39410058, 39391731,  ..., 39390544 ]
 ```
-
+---
 ### Get Job Stories
 ```python
 from hn_sdk.client.v0.client import get_job_stories
 
 print(get_job_stories())
 ```
 ```sh
 [ 39057748, 39040718, 39038845, 39019063,  ..., 39006337 ]
 ```
-
+---
 ### Get Changed Items and Profiles
 ```python
 from hn_sdk.client.v0.client import get_updates
 
 print(get_updates())
 ```
 ```sh
```

### Comparing `hn-sdk-0.1.0/setup.py` & `hn-sdk-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,12 +20,12 @@
     author_email="joeyagreco@gmail.com",
     description="A Python wrapper for the Hacker News API.",
     long_description_content_type="text/markdown",
     long_description=read_me,
     license="MIT",
     url="https://github.com/joeyagreco/hn-api",
     include_package_data=True,
-    packages=setuptools.find_packages(exclude=("test", "docs")),
+    packages=setuptools.find_packages(exclude=("test_e2e")),
     install_requires=required_packages,
     python_requires=f">={minimum_python_version_required}",
     keywords="hacker-news hacker news api sdk",
 )
```

