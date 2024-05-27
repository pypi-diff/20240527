# Comparing `tmp/playwright_page_pool-0.1.2.tar.gz` & `tmp/playwright_page_pool-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwright_page_pool-0.1.2.tar", max compression
+gzip compressed data, was "playwright_page_pool-0.1.3.tar", max compression
```

## Comparing `playwright_page_pool-0.1.2.tar` & `playwright_page_pool-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-05-26 11:31:26.371890 playwright_page_pool-0.1.2/LICENSE
--rw-r--r--   0        0        0     3786 2024-05-26 14:44:02.032762 playwright_page_pool-0.1.2/README.md
--rw-r--r--   0        0        0       44 2024-05-26 14:43:52.481726 playwright_page_pool-0.1.2/playwright_page_pool/__init__.py
--rw-r--r--   0        0        0     4292 2024-05-26 14:43:52.481964 playwright_page_pool-0.1.2/playwright_page_pool/page_pool.py
--rw-r--r--   0        0        0        0 2024-05-26 15:00:17.715334 playwright_page_pool-0.1.2/playwright_page_pool/py.typed
--rw-r--r--   0        0        0     1013 2024-05-26 15:14:45.187367 playwright_page_pool-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4631 1970-01-01 00:00:00.000000 playwright_page_pool-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-26 11:31:26.371890 playwright_page_pool-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4075 2024-05-27 03:25:21.578057 playwright_page_pool-0.1.3/README.md
+-rw-r--r--   0        0        0       44 2024-05-26 14:43:52.481726 playwright_page_pool-0.1.3/playwright_page_pool/__init__.py
+-rw-r--r--   0        0        0     4292 2024-05-26 14:43:52.481964 playwright_page_pool-0.1.3/playwright_page_pool/page_pool.py
+-rw-r--r--   0        0        0        0 2024-05-26 15:00:17.715334 playwright_page_pool-0.1.3/playwright_page_pool/py.typed
+-rw-r--r--   0        0        0      988 2024-05-27 03:26:04.579181 playwright_page_pool-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4895 1970-01-01 00:00:00.000000 playwright_page_pool-0.1.3/PKG-INFO
```

### Comparing `playwright_page_pool-0.1.2/LICENSE` & `playwright_page_pool-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `playwright_page_pool-0.1.2/README.md` & `playwright_page_pool-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -70,9 +70,15 @@
 - max_pages: The maximum number of pages that can be opened at once. Defaults to the number of CPU cores.
 - page_initiator: An optional asynchronous callable that is called each time a new page is created. This allows you to perform custom initialization on each page.
 - reuse_pages: Determines whether pages should be reused. If False, a new page is created for each acquisition. Defaults to False. When set to True, it eliminates the overhead of opening and closing pages repeatedly, thereby improving performance.
 
 ## Contributing 🤝
 Contributions to Playwright Page Pool are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the GitHub repository.
 
+
+## Related Projects 🔗
+
+If you are here looking for a project to help with web crawling, we recommend [playwright-network-spy](https://github.com/code-yeongyu/playwright-page-pool). It's a powerful tool for crawling any website on Earth by capturing HTTP responses, using Playwright.
+
+
 ## License 📄
 This project is licensed under the MIT License. See the LICENSE file for more details.
```

### Comparing `playwright_page_pool-0.1.2/playwright_page_pool/page_pool.py` & `playwright_page_pool-0.1.3/playwright_page_pool/page_pool.py`

 * *Files identical despite different names*

### Comparing `playwright_page_pool-0.1.2/pyproject.toml` & `playwright_page_pool-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "playwright-page-pool"
-version = "0.1.2"
-description = "A utility for managing Playwright browser pages in a pool, inspired by Python's ThreadPool."
+version = "0.1.3"
+description = "Handle multiple playwright pages concurrently with ease and speed."
 authors = ["YeonGyu-Kim <code.yeon.gyu@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 repository = "https://github.com/code-yeongyu/playwright-page-pool"
 homepage = "https://github.com/code-yeongyu/playwright-page-pool"
 
 [tool.poetry.dependencies]
```

### Comparing `playwright_page_pool-0.1.2/PKG-INFO` & `playwright_page_pool-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: playwright-page-pool
-Version: 0.1.2
-Summary: A utility for managing Playwright browser pages in a pool, inspired by Python's ThreadPool.
+Version: 0.1.3
+Summary: Handle multiple playwright pages concurrently with ease and speed.
 Home-page: https://github.com/code-yeongyu/playwright-page-pool
 License: MIT
 Author: YeonGyu-Kim
 Author-email: code.yeon.gyu@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -91,10 +91,16 @@
 - max_pages: The maximum number of pages that can be opened at once. Defaults to the number of CPU cores.
 - page_initiator: An optional asynchronous callable that is called each time a new page is created. This allows you to perform custom initialization on each page.
 - reuse_pages: Determines whether pages should be reused. If False, a new page is created for each acquisition. Defaults to False. When set to True, it eliminates the overhead of opening and closing pages repeatedly, thereby improving performance.
 
 ## Contributing 🤝
 Contributions to Playwright Page Pool are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the GitHub repository.
 
+
+## Related Projects 🔗
+
+If you are here looking for a project to help with web crawling, we recommend [playwright-network-spy](https://github.com/code-yeongyu/playwright-page-pool). It's a powerful tool for crawling any website on Earth by capturing HTTP responses, using Playwright.
+
+
 ## License 📄
 This project is licensed under the MIT License. See the LICENSE file for more details.
```

