# Comparing `tmp/basketball_reference_webscrapper-0.1.3.tar.gz` & `tmp/basketball_reference_webscrapper-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basketball_reference_webscrapper-0.1.3.tar", max compression
+gzip compressed data, was "basketball_reference_webscrapper-0.1.5.tar", max compression
```

## Comparing `basketball_reference_webscrapper-0.1.3.tar` & `basketball_reference_webscrapper-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0      120 2024-05-22 13:14:05.246337 basketball_reference_webscrapper-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-05-22 13:14:05.246337 basketball_reference_webscrapper-0.1.3/basketball_reference_webscrapper/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 13:14:05.246337 basketball_reference_webscrapper-0.1.3/basketball_reference_webscrapper/constants/__init__.py
--rw-r--r--   0        0        0     1223 2024-05-22 13:14:05.246337 basketball_reference_webscrapper-0.1.3/basketball_reference_webscrapper/constants/team_city_refdata.csv
--rw-r--r--   0        0        0        0 2024-05-22 13:14:05.246337 basketball_reference_webscrapper-0.1.3/basketball_reference_webscrapper/utils/__init__.py
--rw-r--r--   0        0        0     1083 2024-05-22 13:14:05.246337 basketball_reference_webscrapper-0.1.3/basketball_reference_webscrapper/utils/logs.py
--rw-r--r--   0        0        0     4326 2024-05-22 13:14:05.246337 basketball_reference_webscrapper-0.1.3/basketball_reference_webscrapper/webscrapping_basketball_reference.py
--rw-r--r--   0        0        0      938 2024-05-22 13:14:05.250337 basketball_reference_webscrapper-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      775 1970-01-01 00:00:00.000000 basketball_reference_webscrapper-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      120 2024-05-27 12:50:32.637539 basketball_reference_webscrapper-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 12:50:32.637539 basketball_reference_webscrapper-0.1.5/basketball_reference_webscrapper/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 12:50:32.637539 basketball_reference_webscrapper-0.1.5/basketball_reference_webscrapper/constants/__init__.py
+-rw-r--r--   0        0        0     1223 2024-05-27 12:50:32.637539 basketball_reference_webscrapper-0.1.5/basketball_reference_webscrapper/constants/team_city_refdata.csv
+-rw-r--r--   0        0        0        0 2024-05-27 12:50:32.637539 basketball_reference_webscrapper-0.1.5/basketball_reference_webscrapper/data_models/__init_.py
+-rw-r--r--   0        0        0      324 2024-05-27 12:50:32.637539 basketball_reference_webscrapper-0.1.5/basketball_reference_webscrapper/data_models/feature_model.py
+-rw-r--r--   0        0        0        0 2024-05-27 12:50:32.637539 basketball_reference_webscrapper-0.1.5/basketball_reference_webscrapper/utils/__init__.py
+-rw-r--r--   0        0        0     1083 2024-05-27 12:50:32.637539 basketball_reference_webscrapper-0.1.5/basketball_reference_webscrapper/utils/logs.py
+-rw-r--r--   0        0        0     7541 2024-05-27 12:50:32.637539 basketball_reference_webscrapper-0.1.5/basketball_reference_webscrapper/webscrapping_basketball_reference.py
+-rw-r--r--   0        0        0      958 2024-05-27 12:50:32.637539 basketball_reference_webscrapper-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 basketball_reference_webscrapper-0.1.5/PKG-INFO
```

### Comparing `basketball_reference_webscrapper-0.1.3/basketball_reference_webscrapper/constants/team_city_refdata.csv` & `basketball_reference_webscrapper-0.1.5/basketball_reference_webscrapper/constants/team_city_refdata.csv`

 * *Files identical despite different names*

### Comparing `basketball_reference_webscrapper-0.1.3/basketball_reference_webscrapper/utils/logs.py` & `basketball_reference_webscrapper-0.1.5/basketball_reference_webscrapper/utils/logs.py`

 * *Files identical despite different names*

### Comparing `basketball_reference_webscrapper-0.1.3/pyproject.toml` & `basketball_reference_webscrapper-0.1.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "basketball-reference-webscrapper"
-version = "0.1.3"
+version = "0.1.5"
 description = "Python package for Basketball Reference that gathers data by scraping the website"
 authors = ["Yannick Flores <yannick.flores1992@gmail.com>"]
 readme = "README.md"
 exclude = ["tests", "docs"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pandas = "2.*"
 numpy = "1.26.*"
 pytest = "*"
 pylint = "^2.15.10"
 beautifulsoup4 = "4.12.*"
 requests = "2.32.*"
+pydantic = "^2.6.1"
 
 [tool.poetry.dev-dependencies]
 coverage = {extras = ["toml"], version = "6.5.*"}
 black = {version = "22.10.*", allow-prereleases = true}
 pytest = "7.2.*"
 pytest-html = "3.1.*"
 pytest-cov = "2.12.*"
```

### Comparing `basketball_reference_webscrapper-0.1.3/PKG-INFO` & `basketball_reference_webscrapper-0.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: basketball-reference-webscrapper
-Version: 0.1.3
+Version: 0.1.5
 Summary: Python package for Basketball Reference that gathers data by scraping the website
 Author: Yannick Flores
 Author-email: yannick.flores1992@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (==4.12.*)
 Requires-Dist: numpy (==1.26.*)
 Requires-Dist: pandas (==2.*)
+Requires-Dist: pydantic (>=2.6.1,<3.0.0)
 Requires-Dist: pylint (>=2.15.10,<3.0.0)
 Requires-Dist: pytest
 Requires-Dist: requests (==2.32.*)
 Description-Content-Type: text/markdown
 
 # basketball-reference-webscrapper
 A python package for Basketball Reference that gathers data by scraping the website.
```

