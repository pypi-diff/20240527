# Comparing `tmp/playwright_network_spy-0.1.2.tar.gz` & `tmp/playwright_network_spy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwright_network_spy-0.1.2.tar", max compression
+gzip compressed data, was "playwright_network_spy-0.1.3.tar", max compression
```

## Comparing `playwright_network_spy-0.1.2.tar` & `playwright_network_spy-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-05-26 13:44:37.188146 playwright_network_spy-0.1.2/LICENSE
--rw-r--r--   0        0        0     3076 2024-05-26 14:56:30.202293 playwright_network_spy-0.1.2/README.md
--rw-r--r--   0        0        0      116 2024-05-26 14:43:03.750400 playwright_network_spy-0.1.2/playwright_network_spy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-26 15:01:59.713932 playwright_network_spy-0.1.2/playwright_network_spy/py.typed
--rw-r--r--   0        0        0     5214 2024-05-26 14:43:03.750640 playwright_network_spy-0.1.2/playwright_network_spy/spy.py
--rw-r--r--   0        0        0     1041 2024-05-26 15:15:35.955721 playwright_network_spy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3949 1970-01-01 00:00:00.000000 playwright_network_spy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-26 13:44:37.188146 playwright_network_spy-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3209 2024-05-26 15:34:00.699874 playwright_network_spy-0.1.3/README.md
+-rw-r--r--   0        0        0      116 2024-05-26 14:43:03.750400 playwright_network_spy-0.1.3/playwright_network_spy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-26 15:01:59.713932 playwright_network_spy-0.1.3/playwright_network_spy/py.typed
+-rw-r--r--   0        0        0     5214 2024-05-26 14:43:03.750640 playwright_network_spy-0.1.3/playwright_network_spy/spy.py
+-rw-r--r--   0        0        0     1021 2024-05-26 15:34:06.359356 playwright_network_spy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4062 1970-01-01 00:00:00.000000 playwright_network_spy-0.1.3/PKG-INFO
```

### Comparing `playwright_network_spy-0.1.2/LICENSE` & `playwright_network_spy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `playwright_network_spy-0.1.2/README.md` & `playwright_network_spy-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -59,17 +59,17 @@
     import asyncio
 
     asyncio.run(main())
 ```
 
 Playwright Network Spy is designed for modern websites that are complex to parse from the DOM. Instead of parsing, simply capture the entire JSON response and utilize it. 😝
 
-For more detailed examples, you can refer to the [Example](examples/) in our GitHub repository.
+For more detailed examples, you can refer to the [Example](https://github.com/code-yeongyu/playwright-network-spy/tree/master/examples) in our GitHub repository.
 
-- [**Instagram Post Crawler (Infinite Scroll + REST API)**](examples/instagram.py)
+- [**Instagram Post Crawler (Infinite Scroll + REST API)**](https://github.com/code-yeongyu/playwright-network-spy/tree/master/examples/instagram.py)
 
 
 ## Documentation 📚
 
 For detailed documentation and more examples, please visit our official documentation.
 Contributing 🤝
 We welcome contributions from the community! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request on our GitHub repository.
```

### Comparing `playwright_network_spy-0.1.2/playwright_network_spy/spy.py` & `playwright_network_spy-0.1.3/playwright_network_spy/spy.py`

 * *Files identical despite different names*

### Comparing `playwright_network_spy-0.1.2/pyproject.toml` & `playwright_network_spy-0.1.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "playwright-network-spy"
-version = "0.1.2"
+version = "0.1.3"
 description = "🔥 A powerful tool for crawling any website on Earth with infinite scrolling, using Playwright."
 authors = ["YeonGyu-Kim <code.yeon.gyu@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
-repository = "https://github.com/playwright-network-spy/playwright-page-pool"
-homepage = "https://github.com/playwright-network-spy/playwright-page-pool"
+repository = "https://github.com/code-yeongyu/playwright-page-pool"
+homepage = "https://github.com/code-yeongyu/playwright-page-pool"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 playwright = "*"
 pip = "*"
```

### Comparing `playwright_network_spy-0.1.2/PKG-INFO` & `playwright_network_spy-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: playwright-network-spy
-Version: 0.1.2
+Version: 0.1.3
 Summary: 🔥 A powerful tool for crawling any website on Earth with infinite scrolling, using Playwright.
-Home-page: https://github.com/playwright-network-spy/playwright-page-pool
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
-Project-URL: Repository, https://github.com/playwright-network-spy/playwright-page-pool
+Project-URL: Repository, https://github.com/code-yeongyu/playwright-page-pool
 Description-Content-Type: text/markdown
 
 # Playwright Network Spy 🕵️‍♂️🌐
 
 [![PyPI version](https://badge.fury.io/py/playwright-network-spy.svg)](https://badge.fury.io/py/playwright-network-spy)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
@@ -80,17 +80,17 @@
     import asyncio
 
     asyncio.run(main())
 ```
 
 Playwright Network Spy is designed for modern websites that are complex to parse from the DOM. Instead of parsing, simply capture the entire JSON response and utilize it. 😝
 
-For more detailed examples, you can refer to the [Example](examples/) in our GitHub repository.
+For more detailed examples, you can refer to the [Example](https://github.com/code-yeongyu/playwright-network-spy/tree/master/examples) in our GitHub repository.
 
-- [**Instagram Post Crawler (Infinite Scroll + REST API)**](examples/instagram.py)
+- [**Instagram Post Crawler (Infinite Scroll + REST API)**](https://github.com/code-yeongyu/playwright-network-spy/tree/master/examples/instagram.py)
 
 
 ## Documentation 📚
 
 For detailed documentation and more examples, please visit our official documentation.
 Contributing 🤝
 We welcome contributions from the community! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request on our GitHub repository.
```

