# Comparing `tmp/ip_searcher-2024.5.27.11.29.53.tar.gz` & `tmp/ip_searcher-2024.5.27.11.45.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ip_searcher-2024.5.27.11.29.53.tar", last modified: Mon May 27 03:29:54 2024, max compression
+gzip compressed data, was "ip_searcher-2024.5.27.11.45.27.tar", last modified: Mon May 27 03:45:27 2024, max compression
```

## Comparing `ip_searcher-2024.5.27.11.29.53.tar` & `ip_searcher-2024.5.27.11.45.27.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-05-27 03:29:54.163609 ip_searcher-2024.5.27.11.29.53/
--rw-r--r--   0 betterme   (501) staff       (20)    11357 2023-03-20 02:44:39.000000 ip_searcher-2024.5.27.11.29.53/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)    12640 2024-05-27 02:50:47.000000 ip_searcher-2024.5.27.11.29.53/LICENSE.md
--rw-r--r--   0 betterme   (501) staff       (20)      335 2024-05-27 03:21:47.000000 ip_searcher-2024.5.27.11.29.53/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)    10091 2024-05-27 03:29:54.163289 ip_searcher-2024.5.27.11.29.53/PKG-INFO
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-05-27 03:29:54.161912 ip_searcher-2024.5.27.11.29.53/ip_searcher/
--rw-r--r--   0 betterme   (501) staff       (20)     1312 2024-05-27 03:26:54.000000 ip_searcher-2024.5.27.11.29.53/ip_searcher/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5677 2024-05-27 03:08:30.000000 ip_searcher-2024.5.27.11.29.53/ip_searcher/xdbSearcher.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-05-27 03:29:54.162948 ip_searcher-2024.5.27.11.29.53/ip_searcher.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)    10091 2024-05-27 03:29:54.000000 ip_searcher-2024.5.27.11.29.53/ip_searcher.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)      302 2024-05-27 03:29:54.000000 ip_searcher-2024.5.27.11.29.53/ip_searcher.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2024-05-27 03:29:54.000000 ip_searcher-2024.5.27.11.29.53/ip_searcher.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)      312 2024-05-27 03:29:54.000000 ip_searcher-2024.5.27.11.29.53/ip_searcher.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)      244 2024-05-27 03:29:54.000000 ip_searcher-2024.5.27.11.29.53/ip_searcher.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)       12 2024-05-27 03:29:54.000000 ip_searcher-2024.5.27.11.29.53/ip_searcher.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2024-05-27 03:29:54.163659 ip_searcher-2024.5.27.11.29.53/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     2466 2023-11-29 08:25:30.000000 ip_searcher-2024.5.27.11.29.53/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-05-27 03:45:27.548537 ip_searcher-2024.5.27.11.45.27/
+-rw-r--r--   0 betterme   (501) staff       (20)    11357 2023-03-20 02:44:39.000000 ip_searcher-2024.5.27.11.45.27/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)    12640 2024-05-27 02:50:47.000000 ip_searcher-2024.5.27.11.45.27/LICENSE.md
+-rw-r--r--   0 betterme   (501) staff       (20)      335 2024-05-27 03:21:47.000000 ip_searcher-2024.5.27.11.45.27/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     1333 2024-05-27 03:45:27.548349 ip_searcher-2024.5.27.11.45.27/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)      674 2024-05-27 03:40:48.000000 ip_searcher-2024.5.27.11.45.27/README.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-05-27 03:45:27.547389 ip_searcher-2024.5.27.11.45.27/ip_searcher/
+-rw-r--r--   0 betterme   (501) staff       (20)     1351 2024-05-27 03:45:26.000000 ip_searcher-2024.5.27.11.45.27/ip_searcher/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5677 2024-05-27 03:08:30.000000 ip_searcher-2024.5.27.11.45.27/ip_searcher/xdbSearcher.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-05-27 03:45:27.548111 ip_searcher-2024.5.27.11.45.27/ip_searcher.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     1333 2024-05-27 03:45:27.000000 ip_searcher-2024.5.27.11.45.27/ip_searcher.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)      312 2024-05-27 03:45:27.000000 ip_searcher-2024.5.27.11.45.27/ip_searcher.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2024-05-27 03:45:27.000000 ip_searcher-2024.5.27.11.45.27/ip_searcher.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      312 2024-05-27 03:45:27.000000 ip_searcher-2024.5.27.11.45.27/ip_searcher.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       15 2024-05-27 03:45:27.000000 ip_searcher-2024.5.27.11.45.27/ip_searcher.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       12 2024-05-27 03:45:27.000000 ip_searcher-2024.5.27.11.45.27/ip_searcher.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2024-05-27 03:45:27.548579 ip_searcher-2024.5.27.11.45.27/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     2466 2024-05-27 03:30:54.000000 ip_searcher-2024.5.27.11.45.27/setup.py
```

### Comparing `ip_searcher-2024.5.27.11.29.53/LICENSE` & `ip_searcher-2024.5.27.11.45.27/LICENSE`

 * *Files identical despite different names*

### Comparing `ip_searcher-2024.5.27.11.29.53/LICENSE.md` & `ip_searcher-2024.5.27.11.45.27/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ip_searcher-2024.5.27.11.29.53/ip_searcher/__init__.py` & `ip_searcher-2024.5.27.11.45.27/ip_searcher/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  : 
 
 from meutils.pipe import *
 from meutils.request_utils.crawler import Crawler
 
-from ip2region.xdbSearcher import XdbSearcher as _XdbSearcher
+from ip2region.xdbSearcher import XdbSearcher
 
-searcher = _XdbSearcher(dbfile=get_resolve_path(__file__, 'data/ip2region.xdb'))
+dbPath = get_resolve_path(__file__, 'data/ip2region.xdb')
+cb = XdbSearcher.loadContentFromFile(dbfile=dbPath)
+searcher = XdbSearcher(contentBuff=cb)
 
 
-# is_open()
-
 @lru_cache()
 def search(ip: str, enhance: Optional[bool] = None):
     region = searcher.searchByIPStr(ip) or []
     searcher.close()
     if is_open('baidu.com:80') if enhance is None else enhance:
         region = enhance_search(ip) + region
     return region  # 可能出现多个候选
```

### Comparing `ip_searcher-2024.5.27.11.29.53/ip_searcher/xdbSearcher.py` & `ip_searcher-2024.5.27.11.45.27/ip_searcher/xdbSearcher.py`

 * *Files identical despite different names*

### Comparing `ip_searcher-2024.5.27.11.29.53/setup.py` & `ip_searcher-2024.5.27.11.45.27/setup.py`

 * *Files identical despite different names*

