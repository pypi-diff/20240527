# Comparing `tmp/csv_summary-0.1.0.tar.gz` & `tmp/csv_summary-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv_summary-0.1.0.tar", last modified: Fri May 24 05:51:08 2024, max compression
+gzip compressed data, was "csv_summary-0.1.1.tar", last modified: Mon May 27 05:12:18 2024, max compression
```

## Comparing `csv_summary-0.1.0.tar` & `csv_summary-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nakatomihikaru   (501) staff       (20)        0 2024-05-24 05:51:08.063327 csv_summary-0.1.0/
--rw-r--r--   0 nakatomihikaru   (501) staff       (20)     3087 2024-05-24 05:51:08.063046 csv_summary-0.1.0/PKG-INFO
--rw-r--r--   0 nakatomihikaru   (501) staff       (20)     2608 2024-05-24 05:38:21.000000 csv_summary-0.1.0/README.md
-drwxr-xr-x   0 nakatomihikaru   (501) staff       (20)        0 2024-05-24 05:51:08.061321 csv_summary-0.1.0/csv_summary.egg-info/
--rw-r--r--   0 nakatomihikaru   (501) staff       (20)     3087 2024-05-24 05:51:08.000000 csv_summary-0.1.0/csv_summary.egg-info/PKG-INFO
--rw-r--r--   0 nakatomihikaru   (501) staff       (20)      306 2024-05-24 05:51:08.000000 csv_summary-0.1.0/csv_summary.egg-info/SOURCES.txt
--rw-r--r--   0 nakatomihikaru   (501) staff       (20)        1 2024-05-24 05:51:08.000000 csv_summary-0.1.0/csv_summary.egg-info/dependency_links.txt
--rw-r--r--   0 nakatomihikaru   (501) staff       (20)       66 2024-05-24 05:51:08.000000 csv_summary-0.1.0/csv_summary.egg-info/entry_points.txt
--rw-r--r--   0 nakatomihikaru   (501) staff       (20)        7 2024-05-24 05:51:08.000000 csv_summary-0.1.0/csv_summary.egg-info/requires.txt
--rw-r--r--   0 nakatomihikaru   (501) staff       (20)        8 2024-05-24 05:51:08.000000 csv_summary-0.1.0/csv_summary.egg-info/top_level.txt
--rw-r--r--   0 nakatomihikaru   (501) staff       (20)       38 2024-05-24 05:51:08.063378 csv_summary-0.1.0/setup.cfg
--rw-r--r--   0 nakatomihikaru   (501) staff       (20)      812 2024-05-23 08:05:44.000000 csv_summary-0.1.0/setup.py
-drwxr-xr-x   0 nakatomihikaru   (501) staff       (20)        0 2024-05-24 05:51:08.062260 csv_summary-0.1.0/summary/
--rw-r--r--   0 nakatomihikaru   (501) staff       (20)       64 2024-05-23 08:05:30.000000 csv_summary-0.1.0/summary/__init__.py
--rw-r--r--   0 nakatomihikaru   (501) staff       (20)      199 2024-05-23 08:05:00.000000 csv_summary-0.1.0/summary/cli.py
--rw-r--r--   0 nakatomihikaru   (501) staff       (20)     1174 2024-05-23 08:05:10.000000 csv_summary-0.1.0/summary/summary.py
-drwxr-xr-x   0 nakatomihikaru   (501) staff       (20)        0 2024-05-24 05:51:08.062544 csv_summary-0.1.0/tests/
--rw-r--r--   0 nakatomihikaru   (501) staff       (20)     1274 2024-05-24 04:18:09.000000 csv_summary-0.1.0/tests/test_summary.py
+drwxr-xr-x   0 nakatomihikaru   (501) staff       (20)        0 2024-05-27 05:12:18.288764 csv_summary-0.1.1/
+-rw-r--r--   0 nakatomihikaru   (501) staff       (20)     3090 2024-05-27 05:12:18.288484 csv_summary-0.1.1/PKG-INFO
+-rw-r--r--   0 nakatomihikaru   (501) staff       (20)     2608 2024-05-24 05:38:21.000000 csv_summary-0.1.1/README.md
+drwxr-xr-x   0 nakatomihikaru   (501) staff       (20)        0 2024-05-27 05:12:18.288199 csv_summary-0.1.1/csv_summary.egg-info/
+-rw-r--r--   0 nakatomihikaru   (501) staff       (20)     3090 2024-05-27 05:12:18.000000 csv_summary-0.1.1/csv_summary.egg-info/PKG-INFO
+-rw-r--r--   0 nakatomihikaru   (501) staff       (20)      306 2024-05-27 05:12:18.000000 csv_summary-0.1.1/csv_summary.egg-info/SOURCES.txt
+-rw-r--r--   0 nakatomihikaru   (501) staff       (20)        1 2024-05-27 05:12:18.000000 csv_summary-0.1.1/csv_summary.egg-info/dependency_links.txt
+-rw-r--r--   0 nakatomihikaru   (501) staff       (20)       66 2024-05-27 05:12:18.000000 csv_summary-0.1.1/csv_summary.egg-info/entry_points.txt
+-rw-r--r--   0 nakatomihikaru   (501) staff       (20)        7 2024-05-27 05:12:18.000000 csv_summary-0.1.1/csv_summary.egg-info/requires.txt
+-rw-r--r--   0 nakatomihikaru   (501) staff       (20)        8 2024-05-27 05:12:18.000000 csv_summary-0.1.1/csv_summary.egg-info/top_level.txt
+-rw-r--r--   0 nakatomihikaru   (501) staff       (20)       38 2024-05-27 05:12:18.288821 csv_summary-0.1.1/setup.cfg
+-rw-r--r--   0 nakatomihikaru   (501) staff       (20)      849 2024-05-27 05:04:24.000000 csv_summary-0.1.1/setup.py
+drwxr-xr-x   0 nakatomihikaru   (501) staff       (20)        0 2024-05-27 05:12:18.287568 csv_summary-0.1.1/summary/
+-rw-r--r--   0 nakatomihikaru   (501) staff       (20)       64 2024-05-23 08:05:30.000000 csv_summary-0.1.1/summary/__init__.py
+-rw-r--r--   0 nakatomihikaru   (501) staff       (20)      199 2024-05-23 08:05:00.000000 csv_summary-0.1.1/summary/cli.py
+-rw-r--r--   0 nakatomihikaru   (501) staff       (20)      107 2024-05-24 08:33:57.000000 csv_summary-0.1.1/summary/summary.py
+drwxr-xr-x   0 nakatomihikaru   (501) staff       (20)        0 2024-05-27 05:12:18.287848 csv_summary-0.1.1/tests/
+-rw-r--r--   0 nakatomihikaru   (501) staff       (20)     1274 2024-05-24 04:18:09.000000 csv_summary-0.1.1/tests/test_summary.py
```

### Comparing `csv_summary-0.1.0/PKG-INFO` & `csv_summary-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: csv_summary
-Version: 0.1.0
+Version: 0.1.1
 Summary: 指定したCSVファイルの統計情報を生成するパッケージ
-Home-page: https://github.com/yourusername/csv_summary
-Author: Your Name
-Author-email: your.email@example.com
+Home-page: https://github.com/pika8911/csv_summary
+Author: pika8911
+Author-email: s2122043@stu.musashino-u.ac.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
```

### Comparing `csv_summary-0.1.0/README.md` & `csv_summary-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `csv_summary-0.1.0/csv_summary.egg-info/PKG-INFO` & `csv_summary-0.1.1/csv_summary.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: csv-summary
-Version: 0.1.0
+Name: csv_summary
+Version: 0.1.1
 Summary: 指定したCSVファイルの統計情報を生成するパッケージ
-Home-page: https://github.com/yourusername/csv_summary
-Author: Your Name
-Author-email: your.email@example.com
+Home-page: https://github.com/pika8911/csv_summary
+Author: pika8911
+Author-email: s2122043@stu.musashino-u.ac.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
```

### Comparing `csv_summary-0.1.0/tests/test_summary.py` & `csv_summary-0.1.1/tests/test_summary.py`

 * *Files identical despite different names*

