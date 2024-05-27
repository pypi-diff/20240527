# Comparing `tmp/scrapy_selenium_addon-0.0.8.tar.gz` & `tmp/scrapy_selenium_addon-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy_selenium_addon-0.0.8.tar", last modified: Mon May 27 09:04:11 2024, max compression
+gzip compressed data, was "scrapy_selenium_addon-0.0.9.tar", last modified: Mon May 27 12:03:09 2024, max compression
```

## Comparing `scrapy_selenium_addon-0.0.8.tar` & `scrapy_selenium_addon-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sulthan   (1000) sulthan   (1000)        0 2024-05-27 09:04:11.924952 scrapy_selenium_addon-0.0.8/
--rw-r--r--   0 sulthan   (1000) sulthan   (1000)      496 2024-05-19 10:04:26.000000 scrapy_selenium_addon-0.0.8/LICENCE
--rw-r--r--   0 sulthan   (1000) sulthan   (1000)       38 2024-05-19 10:04:26.000000 scrapy_selenium_addon-0.0.8/MANIFEST.in
--rw-r--r--   0 sulthan   (1000) sulthan   (1000)      329 2024-05-27 09:04:11.924952 scrapy_selenium_addon-0.0.8/PKG-INFO
--rw-r--r--   0 sulthan   (1000) sulthan   (1000)     2952 2024-05-27 08:52:17.000000 scrapy_selenium_addon-0.0.8/README.md
-drwxr-xr-x   0 sulthan   (1000) sulthan   (1000)        0 2024-05-27 09:04:11.921619 scrapy_selenium_addon-0.0.8/requirements/
--rw-r--r--   0 sulthan   (1000) sulthan   (1000)       30 2024-05-19 10:04:26.000000 scrapy_selenium_addon-0.0.8/requirements/requirements.txt
-drwxr-xr-x   0 sulthan   (1000) sulthan   (1000)        0 2024-05-27 09:04:11.924952 scrapy_selenium_addon-0.0.8/scrapy_selenium_addon/
--rw-r--r--   0 sulthan   (1000) sulthan   (1000)       78 2024-05-19 10:04:26.000000 scrapy_selenium_addon-0.0.8/scrapy_selenium_addon/__init__.py
--rw-r--r--   0 sulthan   (1000) sulthan   (1000)     1060 2024-05-19 10:04:26.000000 scrapy_selenium_addon-0.0.8/scrapy_selenium_addon/http.py
--rw-r--r--   0 sulthan   (1000) sulthan   (1000)     5178 2024-05-27 05:37:26.000000 scrapy_selenium_addon-0.0.8/scrapy_selenium_addon/middlewares.py
-drwxr-xr-x   0 sulthan   (1000) sulthan   (1000)        0 2024-05-27 09:04:11.924952 scrapy_selenium_addon-0.0.8/scrapy_selenium_addon.egg-info/
--rw-r--r--   0 sulthan   (1000) sulthan   (1000)      329 2024-05-27 09:04:11.000000 scrapy_selenium_addon-0.0.8/scrapy_selenium_addon.egg-info/PKG-INFO
--rw-r--r--   0 sulthan   (1000) sulthan   (1000)      467 2024-05-27 09:04:11.000000 scrapy_selenium_addon-0.0.8/scrapy_selenium_addon.egg-info/SOURCES.txt
--rw-r--r--   0 sulthan   (1000) sulthan   (1000)        1 2024-05-27 09:04:11.000000 scrapy_selenium_addon-0.0.8/scrapy_selenium_addon.egg-info/dependency_links.txt
--rw-r--r--   0 sulthan   (1000) sulthan   (1000)       30 2024-05-27 09:04:11.000000 scrapy_selenium_addon-0.0.8/scrapy_selenium_addon.egg-info/requires.txt
--rw-r--r--   0 sulthan   (1000) sulthan   (1000)       28 2024-05-27 09:04:11.000000 scrapy_selenium_addon-0.0.8/scrapy_selenium_addon.egg-info/top_level.txt
--rw-r--r--   0 sulthan   (1000) sulthan   (1000)      424 2024-05-27 09:04:11.924952 scrapy_selenium_addon-0.0.8/setup.cfg
--rw-r--r--   0 sulthan   (1000) sulthan   (1000)      450 2024-05-19 10:04:26.000000 scrapy_selenium_addon-0.0.8/setup.py
-drwxr-xr-x   0 sulthan   (1000) sulthan   (1000)        0 2024-05-27 09:04:11.924952 scrapy_selenium_addon-0.0.8/tests/
--rw-r--r--   0 sulthan   (1000) sulthan   (1000)        0 2024-05-19 10:04:26.000000 scrapy_selenium_addon-0.0.8/tests/__init__.py
--rw-r--r--   0 sulthan   (1000) sulthan   (1000)      954 2024-05-27 07:40:05.000000 scrapy_selenium_addon-0.0.8/tests/test_cases.py
--rw-r--r--   0 sulthan   (1000) sulthan   (1000)     4432 2024-05-27 07:40:33.000000 scrapy_selenium_addon-0.0.8/tests/test_middlewares.py
+drwxr-xr-x   0 sulthan   (1000) sulthan   (1000)        0 2024-05-27 12:03:09.902717 scrapy_selenium_addon-0.0.9/
+-rw-r--r--   0 sulthan   (1000) sulthan   (1000)      496 2024-05-19 10:04:26.000000 scrapy_selenium_addon-0.0.9/LICENCE
+-rw-r--r--   0 sulthan   (1000) sulthan   (1000)       38 2024-05-19 10:04:26.000000 scrapy_selenium_addon-0.0.9/MANIFEST.in
+-rw-r--r--   0 sulthan   (1000) sulthan   (1000)      329 2024-05-27 12:03:09.902717 scrapy_selenium_addon-0.0.9/PKG-INFO
+-rw-r--r--   0 sulthan   (1000) sulthan   (1000)     3975 2024-05-27 11:29:38.000000 scrapy_selenium_addon-0.0.9/README.md
+drwxr-xr-x   0 sulthan   (1000) sulthan   (1000)        0 2024-05-27 12:03:09.902717 scrapy_selenium_addon-0.0.9/requirements/
+-rw-r--r--   0 sulthan   (1000) sulthan   (1000)       30 2024-05-19 10:04:26.000000 scrapy_selenium_addon-0.0.9/requirements/requirements.txt
+drwxr-xr-x   0 sulthan   (1000) sulthan   (1000)        0 2024-05-27 12:03:09.902717 scrapy_selenium_addon-0.0.9/scrapy_selenium_addon/
+-rw-r--r--   0 sulthan   (1000) sulthan   (1000)      117 2024-05-27 11:30:41.000000 scrapy_selenium_addon-0.0.9/scrapy_selenium_addon/__init__.py
+-rw-r--r--   0 sulthan   (1000) sulthan   (1000)     1060 2024-05-19 10:04:26.000000 scrapy_selenium_addon-0.0.9/scrapy_selenium_addon/http.py
+-rw-r--r--   0 sulthan   (1000) sulthan   (1000)     5333 2024-05-27 11:25:57.000000 scrapy_selenium_addon-0.0.9/scrapy_selenium_addon/middlewares.py
+drwxr-xr-x   0 sulthan   (1000) sulthan   (1000)        0 2024-05-27 12:03:09.902717 scrapy_selenium_addon-0.0.9/scrapy_selenium_addon.egg-info/
+-rw-r--r--   0 sulthan   (1000) sulthan   (1000)      329 2024-05-27 12:03:09.000000 scrapy_selenium_addon-0.0.9/scrapy_selenium_addon.egg-info/PKG-INFO
+-rw-r--r--   0 sulthan   (1000) sulthan   (1000)      467 2024-05-27 12:03:09.000000 scrapy_selenium_addon-0.0.9/scrapy_selenium_addon.egg-info/SOURCES.txt
+-rw-r--r--   0 sulthan   (1000) sulthan   (1000)        1 2024-05-27 12:03:09.000000 scrapy_selenium_addon-0.0.9/scrapy_selenium_addon.egg-info/dependency_links.txt
+-rw-r--r--   0 sulthan   (1000) sulthan   (1000)       30 2024-05-27 12:03:09.000000 scrapy_selenium_addon-0.0.9/scrapy_selenium_addon.egg-info/requires.txt
+-rw-r--r--   0 sulthan   (1000) sulthan   (1000)       28 2024-05-27 12:03:09.000000 scrapy_selenium_addon-0.0.9/scrapy_selenium_addon.egg-info/top_level.txt
+-rw-r--r--   0 sulthan   (1000) sulthan   (1000)      424 2024-05-27 12:03:09.906050 scrapy_selenium_addon-0.0.9/setup.cfg
+-rw-r--r--   0 sulthan   (1000) sulthan   (1000)      450 2024-05-19 10:04:26.000000 scrapy_selenium_addon-0.0.9/setup.py
+drwxr-xr-x   0 sulthan   (1000) sulthan   (1000)        0 2024-05-27 12:03:09.902717 scrapy_selenium_addon-0.0.9/tests/
+-rw-r--r--   0 sulthan   (1000) sulthan   (1000)        0 2024-05-19 10:04:26.000000 scrapy_selenium_addon-0.0.9/tests/__init__.py
+-rw-r--r--   0 sulthan   (1000) sulthan   (1000)      954 2024-05-27 07:40:05.000000 scrapy_selenium_addon-0.0.9/tests/test_cases.py
+-rw-r--r--   0 sulthan   (1000) sulthan   (1000)     4432 2024-05-27 07:40:33.000000 scrapy_selenium_addon-0.0.9/tests/test_middlewares.py
```

### Comparing `scrapy_selenium_addon-0.0.8/scrapy_selenium_addon/http.py` & `scrapy_selenium_addon-0.0.9/scrapy_selenium_addon/http.py`

 * *Files identical despite different names*

### Comparing `scrapy_selenium_addon-0.0.8/scrapy_selenium_addon/middlewares.py` & `scrapy_selenium_addon-0.0.9/scrapy_selenium_addon/middlewares.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 from scrapy.exceptions import NotConfigured
 from scrapy.http import HtmlResponse
 from selenium.webdriver.support.ui import WebDriverWait
 
 from .http import SeleniumRequest
 
 
+class seleniumAddon:
+    def update_settings(self, settings):
+        settings['DOWNLOAD_MIDDLEWARES']['scrapy_selenium_addon.seleniumMiddleware'] = 800
+
+
 class SeleniumMiddleware:
     """Scrapy middleware handling the requests using selenium"""
 
     def __init__(self, driver_name, driver_executable_path,
                  browser_executable_path, command_executor, driver_arguments):
         """Initialize the selenium webdriver
```

### Comparing `scrapy_selenium_addon-0.0.8/tests/test_cases.py` & `scrapy_selenium_addon-0.0.9/tests/test_cases.py`

 * *Files identical despite different names*

### Comparing `scrapy_selenium_addon-0.0.8/tests/test_middlewares.py` & `scrapy_selenium_addon-0.0.9/tests/test_middlewares.py`

 * *Files identical despite different names*

