# Comparing `tmp/wellbeing_calculator-0.1.tar.gz` & `tmp/wellbeing_calculator-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wellbeing_calculator-0.1.tar", last modified: Sun May 26 13:38:43 2024, max compression
+gzip compressed data, was "wellbeing_calculator-0.3.tar", last modified: Mon May 27 04:52:48 2024, max compression
```

## Comparing `wellbeing_calculator-0.1.tar` & `wellbeing_calculator-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mochidzukidaiki   (501) staff       (20)        0 2024-05-26 13:38:43.000000 wellbeing_calculator-0.1/
--rw-r--r--   0 mochidzukidaiki   (501) staff       (20)      192 2024-05-26 13:38:43.000000 wellbeing_calculator-0.1/PKG-INFO
--rw-r--r--   0 mochidzukidaiki   (501) staff       (20)      282 2024-05-26 13:03:53.000000 wellbeing_calculator-0.1/README.md
--rw-r--r--   0 mochidzukidaiki   (501) staff       (20)      363 2024-05-25 08:03:59.000000 wellbeing_calculator-0.1/setup.py
--rw-r--r--   0 mochidzukidaiki   (501) staff       (20)       38 2024-05-26 13:38:43.000000 wellbeing_calculator-0.1/setup.cfg
-drwxr-xr-x   0 mochidzukidaiki   (501) staff       (20)        0 2024-05-26 13:38:43.000000 wellbeing_calculator-0.1/src/
-drwxr-xr-x   0 mochidzukidaiki   (501) staff       (20)        0 2024-05-26 13:38:43.000000 wellbeing_calculator-0.1/src/wellbeing_calculator/
--rw-r--r--   0 mochidzukidaiki   (501) staff       (20)        0 2024-05-25 07:46:53.000000 wellbeing_calculator-0.1/src/wellbeing_calculator/__init__.py
--rw-r--r--   0 mochidzukidaiki   (501) staff       (20)      894 2024-05-26 13:04:57.000000 wellbeing_calculator-0.1/src/wellbeing_calculator/calculator.py
-drwxr-xr-x   0 mochidzukidaiki   (501) staff       (20)        0 2024-05-26 13:38:43.000000 wellbeing_calculator-0.1/src/wellbeing_calculator.egg-info/
--rw-r--r--   0 mochidzukidaiki   (501) staff       (20)      192 2024-05-26 13:38:43.000000 wellbeing_calculator-0.1/src/wellbeing_calculator.egg-info/PKG-INFO
--rw-r--r--   0 mochidzukidaiki   (501) staff       (20)      384 2024-05-26 13:38:43.000000 wellbeing_calculator-0.1/src/wellbeing_calculator.egg-info/SOURCES.txt
--rw-r--r--   0 mochidzukidaiki   (501) staff       (20)       79 2024-05-26 13:38:43.000000 wellbeing_calculator-0.1/src/wellbeing_calculator.egg-info/entry_points.txt
--rw-r--r--   0 mochidzukidaiki   (501) staff       (20)        7 2024-05-26 13:38:43.000000 wellbeing_calculator-0.1/src/wellbeing_calculator.egg-info/requires.txt
--rw-r--r--   0 mochidzukidaiki   (501) staff       (20)       21 2024-05-26 13:38:43.000000 wellbeing_calculator-0.1/src/wellbeing_calculator.egg-info/top_level.txt
--rw-r--r--   0 mochidzukidaiki   (501) staff       (20)        1 2024-05-26 13:38:43.000000 wellbeing_calculator-0.1/src/wellbeing_calculator.egg-info/dependency_links.txt
+drwxr-xr-x   0 mochidzukidaiki   (501) staff       (20)        0 2024-05-27 04:52:48.994932 wellbeing_calculator-0.3/
+-rw-r--r--   0 mochidzukidaiki   (501) staff       (20)     2522 2024-05-27 04:52:48.994747 wellbeing_calculator-0.3/PKG-INFO
+-rw-r--r--   0 mochidzukidaiki   (501) staff       (20)     1607 2024-05-27 04:29:35.000000 wellbeing_calculator-0.3/README.md
+-rw-r--r--   0 mochidzukidaiki   (501) staff       (20)       38 2024-05-27 04:52:48.994975 wellbeing_calculator-0.3/setup.cfg
+-rw-r--r--   0 mochidzukidaiki   (501) staff       (20)     1273 2024-05-27 04:52:13.000000 wellbeing_calculator-0.3/setup.py
+drwxr-xr-x   0 mochidzukidaiki   (501) staff       (20)        0 2024-05-27 04:52:48.993327 wellbeing_calculator-0.3/src/
+drwxr-xr-x   0 mochidzukidaiki   (501) staff       (20)        0 2024-05-27 04:52:48.993760 wellbeing_calculator-0.3/src/wellbeing_calculator/
+-rw-r--r--   0 mochidzukidaiki   (501) staff       (20)        0 2024-05-25 07:46:53.000000 wellbeing_calculator-0.3/src/wellbeing_calculator/__init__.py
+-rw-r--r--   0 mochidzukidaiki   (501) staff       (20)      846 2024-05-27 01:52:17.000000 wellbeing_calculator-0.3/src/wellbeing_calculator/calculator.py
+drwxr-xr-x   0 mochidzukidaiki   (501) staff       (20)        0 2024-05-27 04:52:48.994578 wellbeing_calculator-0.3/src/wellbeing_calculator.egg-info/
+-rw-r--r--   0 mochidzukidaiki   (501) staff       (20)     2522 2024-05-27 04:52:48.000000 wellbeing_calculator-0.3/src/wellbeing_calculator.egg-info/PKG-INFO
+-rw-r--r--   0 mochidzukidaiki   (501) staff       (20)      384 2024-05-27 04:52:48.000000 wellbeing_calculator-0.3/src/wellbeing_calculator.egg-info/SOURCES.txt
+-rw-r--r--   0 mochidzukidaiki   (501) staff       (20)        1 2024-05-27 04:52:48.000000 wellbeing_calculator-0.3/src/wellbeing_calculator.egg-info/dependency_links.txt
+-rw-r--r--   0 mochidzukidaiki   (501) staff       (20)       79 2024-05-27 04:52:48.000000 wellbeing_calculator-0.3/src/wellbeing_calculator.egg-info/entry_points.txt
+-rw-r--r--   0 mochidzukidaiki   (501) staff       (20)        7 2024-05-27 04:52:48.000000 wellbeing_calculator-0.3/src/wellbeing_calculator.egg-info/requires.txt
+-rw-r--r--   0 mochidzukidaiki   (501) staff       (20)       21 2024-05-27 04:52:48.000000 wellbeing_calculator-0.3/src/wellbeing_calculator.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `wellbeing_calculator-0.1/src/wellbeing_calculator/calculator.py` & `wellbeing_calculator-0.3/src/wellbeing_calculator/calculator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pandas as pd
 import sys
 
 def calculate_wellbeing_score(row):
-    # Example formula to calculate wellbeing score
     score = (
         (24 - row['sns_usage']) * 0.2 +
         row['sleep_time'] * 0.3 +
         row['exercise_time'] * 0.3 -
         row['stress_level'] * 0.2
     )
     return score
@@ -24,7 +23,10 @@
         sys.exit(1)
     
     data['wellbeing_score'] = data.apply(calculate_wellbeing_score, axis=1)
     print(data[['user_id', 'wellbeing_score']])
 
 if __name__ == "__main__":
     main()
+
+
+
```

