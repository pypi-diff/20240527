# Comparing `tmp/impyrialtest-0.1.2.tar.gz` & `tmp/impyrialtest-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/aelkhodary/Documents/GitHub/Python-ETL/Data-Camp/developing-python-packages/mypackages/impyrialTest/dist/impyrialtest-0.", last modified: Sun May 26 18:13:13 2024, max compression
+gzip compressed data, was "dist/impyrialtest-0.1.3.tar", last modified: Sun May 26 18:30:05 2024, max compression
```

## Comparing `impyrialtest-0.1.2.tar` & `impyrialtest-0.1.3.tar`

### file list

```diff
@@ -1,38 +1,21 @@
-drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:13:13.376379 ./
-drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:13:13.376501 ./Users/
-drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:13:13.376616 ./Users/aelkhodary/
-drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:13:13.376729 ./Users/aelkhodary/Documents/
-drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:13:13.376885 ./Users/aelkhodary/Documents/GitHub/
-drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:13:13.377030 ./Users/aelkhodary/Documents/GitHub/Python-ETL/
-drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:13:13.377163 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/
-drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:13:13.377299 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/
-drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:13:13.377417 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/
-drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:13:13.391690 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/
-drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:13:13.384448 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/
--rw-r--r--   0 aelkhodary   (501) staff       (20)      247 2024-05-26 18:03:46.000000 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/__init__.py
-drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:13:13.386932 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/__pycache__/
--rw-r--r--   0 aelkhodary   (501) staff       (20)      431 2024-05-26 18:13:13.384616 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 aelkhodary   (501) staff       (20)      612 2024-05-26 18:13:13.386833 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/__pycache__/utils.cpython-38.pyc
-drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:13:13.384968 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/length/
--rw-r--r--   0 aelkhodary   (501) staff       (20)      140 2024-05-26 16:25:56.000000 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/length/__init__.py
-drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:13:13.386394 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/length/__pycache__/
--rw-r--r--   0 aelkhodary   (501) staff       (20)      337 2024-05-26 18:13:13.385145 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/length/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 aelkhodary   (501) staff       (20)     1171 2024-05-26 18:13:13.386281 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/length/__pycache__/api.cpython-38.pyc
--rw-r--r--   0 aelkhodary   (501) staff       (20)     1555 2024-05-26 18:13:13.385679 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/length/__pycache__/core.cpython-38.pyc
--rw-r--r--   0 aelkhodary   (501) staff       (20)     1221 2024-05-26 16:39:16.000000 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/length/api.py
--rw-r--r--   0 aelkhodary   (501) staff       (20)     1387 2024-05-26 16:13:45.000000 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/length/core.py
--rw-r--r--   0 aelkhodary   (501) staff       (20)      457 2024-05-26 16:13:45.000000 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/utils.py
-drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:13:13.382420 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/weight/
--rw-r--r--   0 aelkhodary   (501) staff       (20)      140 2024-05-26 16:25:56.000000 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/weight/__init__.py
-drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:13:13.384173 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/weight/__pycache__/
--rw-r--r--   0 aelkhodary   (501) staff       (20)      337 2024-05-26 18:13:13.382599 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/weight/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 aelkhodary   (501) staff       (20)     1172 2024-05-26 18:13:13.384053 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/weight/__pycache__/api.cpython-38.pyc
--rw-r--r--   0 aelkhodary   (501) staff       (20)     1568 2024-05-26 18:13:13.383283 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/weight/__pycache__/core.cpython-38.pyc
--rw-r--r--   0 aelkhodary   (501) staff       (20)     1226 2024-05-26 16:40:48.000000 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/weight/api.py
--rw-r--r--   0 aelkhodary   (501) staff       (20)     1410 2024-05-26 18:03:13.000000 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/weight/core.py
-drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:13:13.393767 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest-0.1.2-py3.8.egg-info/
--rw-r--r--   0 aelkhodary   (501) staff       (20)      311 2024-05-26 18:13:13.280324 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest-0.1.2-py3.8.egg-info/PKG-INFO
--rw-r--r--   0 aelkhodary   (501) staff       (20)      408 2024-05-26 18:13:13.293511 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest-0.1.2-py3.8.egg-info/SOURCES.txt
--rw-r--r--   0 aelkhodary   (501) staff       (20)        1 2024-05-26 18:13:13.280819 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest-0.1.2-py3.8.egg-info/dependency_links.txt
--rw-r--r--   0 aelkhodary   (501) staff       (20)        6 2024-05-26 18:13:13.281177 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest-0.1.2-py3.8.egg-info/requires.txt
--rw-r--r--   0 aelkhodary   (501) staff       (20)       13 2024-05-26 18:13:13.281391 ./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest-0.1.2-py3.8.egg-info/top_level.txt
+drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:30:05.849838 impyrialtest-0.1.3/
+-rw-r--r--   0 aelkhodary   (501) staff       (20)      311 2024-05-26 18:30:05.849402 impyrialtest-0.1.3/PKG-INFO
+drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:30:05.842185 impyrialtest-0.1.3/impyrialTest/
+-rw-r--r--   0 aelkhodary   (501) staff       (20)      247 2024-05-26 18:03:46.000000 impyrialtest-0.1.3/impyrialTest/__init__.py
+drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:30:05.845952 impyrialtest-0.1.3/impyrialTest/length/
+-rw-r--r--   0 aelkhodary   (501) staff       (20)      140 2024-05-26 16:25:56.000000 impyrialtest-0.1.3/impyrialTest/length/__init__.py
+-rw-r--r--   0 aelkhodary   (501) staff       (20)     1221 2024-05-26 16:39:16.000000 impyrialtest-0.1.3/impyrialTest/length/api.py
+-rw-r--r--   0 aelkhodary   (501) staff       (20)     1387 2024-05-26 16:13:45.000000 impyrialtest-0.1.3/impyrialTest/length/core.py
+-rw-r--r--   0 aelkhodary   (501) staff       (20)      457 2024-05-26 16:13:45.000000 impyrialtest-0.1.3/impyrialTest/utils.py
+drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:30:05.848034 impyrialtest-0.1.3/impyrialTest/weight/
+-rw-r--r--   0 aelkhodary   (501) staff       (20)      140 2024-05-26 16:25:56.000000 impyrialtest-0.1.3/impyrialTest/weight/__init__.py
+-rw-r--r--   0 aelkhodary   (501) staff       (20)     1226 2024-05-26 16:40:48.000000 impyrialtest-0.1.3/impyrialTest/weight/api.py
+-rw-r--r--   0 aelkhodary   (501) staff       (20)     1410 2024-05-26 18:03:13.000000 impyrialtest-0.1.3/impyrialTest/weight/core.py
+drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:30:05.848912 impyrialtest-0.1.3/impyrialTest.egg-info/
+-rw-r--r--   0 aelkhodary   (501) staff       (20)      311 2024-05-26 18:30:05.000000 impyrialtest-0.1.3/impyrialTest.egg-info/PKG-INFO
+-rw-r--r--   0 aelkhodary   (501) staff       (20)      408 2024-05-26 18:30:05.000000 impyrialtest-0.1.3/impyrialTest.egg-info/SOURCES.txt
+-rw-r--r--   0 aelkhodary   (501) staff       (20)        1 2024-05-26 18:30:05.000000 impyrialtest-0.1.3/impyrialTest.egg-info/dependency_links.txt
+-rw-r--r--   0 aelkhodary   (501) staff       (20)        6 2024-05-26 18:30:05.000000 impyrialtest-0.1.3/impyrialTest.egg-info/requires.txt
+-rw-r--r--   0 aelkhodary   (501) staff       (20)       13 2024-05-26 18:30:05.000000 impyrialtest-0.1.3/impyrialTest.egg-info/top_level.txt
+-rw-r--r--   0 aelkhodary   (501) staff       (20)       38 2024-05-26 18:30:05.849960 impyrialtest-0.1.3/setup.cfg
+-rw-r--r--   0 aelkhodary   (501) staff       (20)      525 2024-05-26 18:29:57.000000 impyrialtest-0.1.3/setup.py
```

### Comparing `./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/length/api.py` & `impyrialtest-0.1.3/impyrialTest/length/api.py`

 * *Files identical despite different names*

### Comparing `./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/length/core.py` & `impyrialtest-0.1.3/impyrialTest/length/core.py`

 * *Files identical despite different names*

### Comparing `./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/weight/api.py` & `impyrialtest-0.1.3/impyrialTest/weight/api.py`

 * *Files identical despite different names*

### Comparing `./Users/aelkhodary/Documents/GitHub/Python-ETL/venv/lib/python3.8/site-packages/impyrialTest/weight/core.py` & `impyrialtest-0.1.3/impyrialTest/weight/core.py`

 * *Files identical despite different names*

