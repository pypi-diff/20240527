# Comparing `tmp/pinscrape-3.2.1.tar.gz` & `tmp/pinscrape-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinscrape-3.2.1.tar", last modified: Fri May 24 10:32:50 2024, max compression
+gzip compressed data, was "pinscrape-3.2.2.tar", last modified: Mon May 27 18:51:14 2024, max compression
```

## Comparing `pinscrape-3.2.1.tar` & `pinscrape-3.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:32:50.147877 pinscrape-3.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-24 10:32:36.000000 pinscrape-3.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-24 10:32:50.147877 pinscrape-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-24 10:32:36.000000 pinscrape-3.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:32:50.143877 pinscrape-3.2.1/pinscrape/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-24 10:32:36.000000 pinscrape-3.2.1/pinscrape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-24 10:32:36.000000 pinscrape-3.2.1/pinscrape/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-05-24 10:32:36.000000 pinscrape-3.2.1/pinscrape/pinscrape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:32:50.147877 pinscrape-3.2.1/pinscrape.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-24 10:32:50.000000 pinscrape-3.2.1/pinscrape.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-24 10:32:50.000000 pinscrape-3.2.1/pinscrape.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 10:32:50.000000 pinscrape-3.2.1/pinscrape.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-24 10:32:50.000000 pinscrape-3.2.1/pinscrape.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 10:32:50.000000 pinscrape-3.2.1/pinscrape.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 10:32:50.147877 pinscrape-3.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-24 10:32:36.000000 pinscrape-3.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:51:14.886001 pinscrape-3.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-27 18:51:01.000000 pinscrape-3.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-27 18:51:14.882001 pinscrape-3.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-27 18:51:01.000000 pinscrape-3.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:51:14.882001 pinscrape-3.2.2/pinscrape/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-27 18:51:01.000000 pinscrape-3.2.2/pinscrape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 18:51:01.000000 pinscrape-3.2.2/pinscrape/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-05-27 18:51:01.000000 pinscrape-3.2.2/pinscrape/pinscrape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:51:14.882001 pinscrape-3.2.2/pinscrape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-27 18:51:14.000000 pinscrape-3.2.2/pinscrape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-27 18:51:14.000000 pinscrape-3.2.2/pinscrape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 18:51:14.000000 pinscrape-3.2.2/pinscrape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-27 18:51:14.000000 pinscrape-3.2.2/pinscrape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 18:51:14.000000 pinscrape-3.2.2/pinscrape.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 18:51:14.886001 pinscrape-3.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-27 18:51:01.000000 pinscrape-3.2.2/setup.py
```

### Comparing `pinscrape-3.2.1/LICENSE` & `pinscrape-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pinscrape-3.2.1/PKG-INFO` & `pinscrape-3.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinscrape
-Version: 3.2.1
+Version: 3.2.2
 Summary: Pinterest | a simple data scraper for pinterest
 Home-page: https://github.com/iamatulsingh/pinscrape
 Author: Atul Singh
 Author-email: atulsingh0401@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pinscrape-3.2.1/README.md` & `pinscrape-3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pinscrape-3.2.1/pinscrape/pinscrape.py` & `pinscrape-3.2.2/pinscrape/pinscrape.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     # -------------------------- get user keyword and google search for that keywords ---------------------
     @staticmethod
     def start_scraping(max_images, key=None, proxies: dict = {}):
         assert key is not None, "Please provide keyword for searching images"
         keyword = key + " pinterest"
         keyword = keyword.replace("+", "%20")
         url = f'https://www.bing.com/search?q={keyword}&first=1&FORM=PERE'
-        res = get(url, proxies=proxies)
+        res = get(url, proxies=proxies, headers={"User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/125.0.0.0 Safari/537.36 Edg/125.0.0.0"})
         searched_urls = PinterestImageScraper.get_pinterest_links(res.content, max_images)
 
         return searched_urls, key.replace(" ", "_"), res.status_code
 
     def scrape(self, key: str = None, output_folder: str = "", proxies: dict = {}, threads: int = 10, max_images: int = None) -> dict:
         extracted_urls, keyword, search_engine_status_code = PinterestImageScraper.start_scraping(max_images, key, proxies)
         self.unique_img = []
```

### Comparing `pinscrape-3.2.1/pinscrape.egg-info/PKG-INFO` & `pinscrape-3.2.2/pinscrape.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinscrape
-Version: 3.2.1
+Version: 3.2.2
 Summary: Pinterest | a simple data scraper for pinterest
 Home-page: https://github.com/iamatulsingh/pinscrape
 Author: Atul Singh
 Author-email: atulsingh0401@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pinscrape-3.2.1/setup.py` & `pinscrape-3.2.2/setup.py`

 * *Files identical despite different names*

