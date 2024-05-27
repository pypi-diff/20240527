# Comparing `tmp/py_alpaca_daily_losers-0.2.8.tar.gz` & `tmp/py_alpaca_daily_losers-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_daily_losers-0.2.8.tar", max compression
+gzip compressed data, was "py_alpaca_daily_losers-0.2.9.tar", max compression
```

## Comparing `py_alpaca_daily_losers-0.2.8.tar` & `py_alpaca_daily_losers-0.2.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1066 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.2.8/LICENSE
--rw-r--r--   0        0        0    13887 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.2.8/README.md
--rw-r--r--   0        0        0        0 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.2.8/py_alpaca_daily_losers/__init__.py
--rw-r--r--   0        0        0    27210 2024-05-26 21:14:23.531821 py_alpaca_daily_losers-0.2.8/py_alpaca_daily_losers/daily_losers.py
--rw-r--r--   0        0        0        0 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.2.8/py_alpaca_daily_losers/src/__init__.py
--rw-r--r--   0        0        0     1407 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.2.8/py_alpaca_daily_losers/src/article_extractor.py
--rw-r--r--   0        0        0      481 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.2.8/py_alpaca_daily_losers/src/global_fuctions.py
--rw-r--r--   0        0        0      936 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.2.8/py_alpaca_daily_losers/src/marketaux.py
--rw-r--r--   0        0        0     2183 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.2.8/py_alpaca_daily_losers/src/openai.py
--rw-r--r--   0        0        0     1941 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.2.8/py_alpaca_daily_losers/src/slack.py
--rw-r--r--   0        0        0      893 2024-05-26 21:14:23.531821 py_alpaca_daily_losers-0.2.8/py_alpaca_daily_losers/src/yahoo.py
--rw-r--r--   0        0        0      713 2024-05-26 21:14:23.531821 py_alpaca_daily_losers-0.2.8/pyproject.toml
--rw-r--r--   0        0        0    14591 1970-01-01 00:00:00.000000 py_alpaca_daily_losers-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.2.9/LICENSE
+-rw-r--r--   0        0        0    13887 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.2.9/README.md
+-rw-r--r--   0        0        0        0 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.2.9/py_alpaca_daily_losers/__init__.py
+-rw-r--r--   0        0        0    27210 2024-05-26 21:14:23.531821 py_alpaca_daily_losers-0.2.9/py_alpaca_daily_losers/daily_losers.py
+-rw-r--r--   0        0        0        0 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.2.9/py_alpaca_daily_losers/src/__init__.py
+-rw-r--r--   0        0        0     1407 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.2.9/py_alpaca_daily_losers/src/article_extractor.py
+-rw-r--r--   0        0        0      481 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.2.9/py_alpaca_daily_losers/src/global_fuctions.py
+-rw-r--r--   0        0        0      936 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.2.9/py_alpaca_daily_losers/src/marketaux.py
+-rw-r--r--   0        0        0     2183 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.2.9/py_alpaca_daily_losers/src/openai.py
+-rw-r--r--   0        0        0     1941 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.2.9/py_alpaca_daily_losers/src/slack.py
+-rw-r--r--   0        0        0      893 2024-05-26 21:14:23.531821 py_alpaca_daily_losers-0.2.9/py_alpaca_daily_losers/src/yahoo.py
+-rw-r--r--   0        0        0      713 2024-05-27 00:04:27.339609 py_alpaca_daily_losers-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0    14591 1970-01-01 00:00:00.000000 py_alpaca_daily_losers-0.2.9/PKG-INFO
```

### Comparing `py_alpaca_daily_losers-0.2.8/LICENSE` & `py_alpaca_daily_losers-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.2.8/README.md` & `py_alpaca_daily_losers-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.2.8/py_alpaca_daily_losers/daily_losers.py` & `py_alpaca_daily_losers-0.2.9/py_alpaca_daily_losers/daily_losers.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.2.8/py_alpaca_daily_losers/src/article_extractor.py` & `py_alpaca_daily_losers-0.2.9/py_alpaca_daily_losers/src/article_extractor.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.2.8/py_alpaca_daily_losers/src/marketaux.py` & `py_alpaca_daily_losers-0.2.9/py_alpaca_daily_losers/src/marketaux.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.2.8/py_alpaca_daily_losers/src/openai.py` & `py_alpaca_daily_losers-0.2.9/py_alpaca_daily_losers/src/openai.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.2.8/py_alpaca_daily_losers/src/slack.py` & `py_alpaca_daily_losers-0.2.9/py_alpaca_daily_losers/src/slack.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.2.8/py_alpaca_daily_losers/src/yahoo.py` & `py_alpaca_daily_losers-0.2.9/py_alpaca_daily_losers/src/yahoo.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.2.8/pyproject.toml` & `py_alpaca_daily_losers-0.2.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "py-alpaca-daily-losers"
-version = "0.2.8"
+version = "0.2.9"
 description = "Daily Losers strategy, uses py-alpaca-api for Alpaca Markets integration."
 authors = ["TexasCoding <jeff10278@me.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 python-dotenv = "^1.0.1"
 requests = "^2.31.0"
 openai = "^1.30.1"
 slack-sdk = "^3.27.2"
 ta = "^0.11.0"
-py-alpaca-api = "^0.5.8"
+py-alpaca-api = "^0.6.0"
 tqdm = "^4.66.4"
 yfinance = "^0.2.40"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.4.2"
 
 [build-system]
```

### Comparing `py_alpaca_daily_losers-0.2.8/PKG-INFO` & `py_alpaca_daily_losers-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: py-alpaca-daily-losers
-Version: 0.2.8
+Version: 0.2.9
 Summary: Daily Losers strategy, uses py-alpaca-api for Alpaca Markets integration.
 Author: TexasCoding
 Author-email: jeff10278@me.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: openai (>=1.30.1,<2.0.0)
-Requires-Dist: py-alpaca-api (>=0.5.8,<0.6.0)
+Requires-Dist: py-alpaca-api (>=0.6.0,<0.7.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: slack-sdk (>=3.27.2,<4.0.0)
 Requires-Dist: ta (>=0.11.0,<0.12.0)
 Requires-Dist: tqdm (>=4.66.4,<5.0.0)
 Requires-Dist: yfinance (>=0.2.40,<0.3.0)
 Description-Content-Type: text/markdown
```

