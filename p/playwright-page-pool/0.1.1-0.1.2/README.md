# Comparing `tmp/playwright_page_pool-0.1.1.tar.gz` & `tmp/playwright_page_pool-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwright_page_pool-0.1.1.tar", max compression
+gzip compressed data, was "playwright_page_pool-0.1.2.tar", max compression
```

## Comparing `playwright_page_pool-0.1.1.tar` & `playwright_page_pool-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-05-26 11:31:26.371890 playwright_page_pool-0.1.1/LICENSE
--rw-r--r--   0        0        0     3786 2024-05-26 14:44:02.032762 playwright_page_pool-0.1.1/README.md
--rw-r--r--   0        0        0       44 2024-05-26 14:43:52.481726 playwright_page_pool-0.1.1/playwright_page_pool/__init__.py
--rw-r--r--   0        0        0     4292 2024-05-26 14:43:52.481964 playwright_page_pool-0.1.1/playwright_page_pool/page_pool.py
--rw-r--r--   0        0        0        0 2024-05-26 15:00:17.715334 playwright_page_pool-0.1.1/playwright_page_pool/py.typed
--rw-r--r--   0        0        0      879 2024-05-26 15:00:07.442946 playwright_page_pool-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4489 1970-01-01 00:00:00.000000 playwright_page_pool-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-26 11:31:26.371890 playwright_page_pool-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3786 2024-05-26 14:44:02.032762 playwright_page_pool-0.1.2/README.md
+-rw-r--r--   0        0        0       44 2024-05-26 14:43:52.481726 playwright_page_pool-0.1.2/playwright_page_pool/__init__.py
+-rw-r--r--   0        0        0     4292 2024-05-26 14:43:52.481964 playwright_page_pool-0.1.2/playwright_page_pool/page_pool.py
+-rw-r--r--   0        0        0        0 2024-05-26 15:00:17.715334 playwright_page_pool-0.1.2/playwright_page_pool/py.typed
+-rw-r--r--   0        0        0     1013 2024-05-26 15:14:45.187367 playwright_page_pool-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4631 1970-01-01 00:00:00.000000 playwright_page_pool-0.1.2/PKG-INFO
```

### Comparing `playwright_page_pool-0.1.1/LICENSE` & `playwright_page_pool-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `playwright_page_pool-0.1.1/README.md` & `playwright_page_pool-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `playwright_page_pool-0.1.1/playwright_page_pool/page_pool.py` & `playwright_page_pool-0.1.2/playwright_page_pool/page_pool.py`

 * *Files identical despite different names*

### Comparing `playwright_page_pool-0.1.1/pyproject.toml` & `playwright_page_pool-0.1.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [tool.poetry]
 name = "playwright-page-pool"
-version = "0.1.1"
+version = "0.1.2"
 description = "A utility for managing Playwright browser pages in a pool, inspired by Python's ThreadPool."
 authors = ["YeonGyu-Kim <code.yeon.gyu@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
+repository = "https://github.com/code-yeongyu/playwright-page-pool"
+homepage = "https://github.com/code-yeongyu/playwright-page-pool"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 playwright = "*"
 pip = "*"
```

### Comparing `playwright_page_pool-0.1.1/PKG-INFO` & `playwright_page_pool-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: playwright-page-pool
-Version: 0.1.1
+Version: 0.1.2
 Summary: A utility for managing Playwright browser pages in a pool, inspired by Python's ThreadPool.
+Home-page: https://github.com/code-yeongyu/playwright-page-pool
 License: MIT
 Author: YeonGyu-Kim
 Author-email: code.yeon.gyu@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pip
 Requires-Dist: playwright
+Project-URL: Repository, https://github.com/code-yeongyu/playwright-page-pool
 Description-Content-Type: text/markdown
 
 # Playwright Page Pool 🎭🏊‍♀️
 
 [![PyPI version](https://badge.fury.io/py/playwright-page-pool.svg)](https://badge.fury.io/py/playwright-page-pool)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

