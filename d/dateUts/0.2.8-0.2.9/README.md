# Comparing `tmp/dateUts-0.2.8.tar.gz` & `tmp/dateUts-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dateUts-0.2.8.tar", last modified: Thu Nov  9 01:07:20 2023, max compression
+gzip compressed data, was "dateUts-0.2.9.tar", last modified: Mon May 27 12:50:56 2024, max compression
```

## Comparing `dateUts-0.2.8.tar` & `dateUts-0.2.9.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-11-09 01:07:20.760235 dateUts-0.2.8/
--rw-rw-rw-   0        0        0      828 2023-09-25 20:45:13.000000 dateUts-0.2.8/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2023-04-26 21:06:44.000000 dateUts-0.2.8/LICENCE.txt
--rw-rw-rw-   0        0        0       30 2023-04-26 21:06:44.000000 dateUts-0.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4859 2023-11-09 01:07:20.759235 dateUts-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     3464 2023-07-11 17:38:55.000000 dateUts-0.2.8/README.md
--rw-rw-rw-   0        0        0      122 2023-04-26 21:06:44.000000 dateUts-0.2.8/commands.txt
-drwxrwxrwx   0        0        0        0 2023-11-09 01:07:20.722235 dateUts-0.2.8/dateUts/
--rw-rw-rw-   0        0        0     7356 2023-11-09 01:06:47.000000 dateUts-0.2.8/dateUts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-09 01:07:20.757235 dateUts-0.2.8/dateUts.egg-info/
--rw-rw-rw-   0        0        0     4859 2023-11-09 01:07:20.000000 dateUts-0.2.8/dateUts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-11-09 01:07:20.000000 dateUts-0.2.8/dateUts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-09 01:07:20.000000 dateUts-0.2.8/dateUts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-11-09 01:07:20.000000 dateUts-0.2.8/dateUts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-11-09 01:07:20.000000 dateUts-0.2.8/dateUts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-09 01:07:20.761237 dateUts-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-11-09 01:07:14.000000 dateUts-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:50:56.726213 dateUts-0.2.9/
+-rw-rw-rw-   0        0        0      828 2023-09-25 20:45:13.000000 dateUts-0.2.9/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2023-04-26 21:06:44.000000 dateUts-0.2.9/LICENCE.txt
+-rw-rw-rw-   0        0        0       30 2023-04-26 21:06:44.000000 dateUts-0.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4909 2024-05-27 12:50:56.723216 dateUts-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3514 2024-05-27 12:48:13.000000 dateUts-0.2.9/README.md
+-rw-rw-rw-   0        0        0      205 2024-05-27 12:50:53.000000 dateUts-0.2.9/commands.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 12:50:56.702212 dateUts-0.2.9/dateUts/
+-rw-rw-rw-   0        0        0     6897 2024-05-27 12:49:02.000000 dateUts-0.2.9/dateUts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:50:56.719211 dateUts-0.2.9/dateUts.egg-info/
+-rw-rw-rw-   0        0        0     4909 2024-05-27 12:50:56.000000 dateUts-0.2.9/dateUts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-27 12:50:56.000000 dateUts-0.2.9/dateUts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 12:50:56.000000 dateUts-0.2.9/dateUts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-27 12:50:56.000000 dateUts-0.2.9/dateUts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-27 12:50:56.000000 dateUts-0.2.9/dateUts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      615 2024-05-27 12:49:35.000000 dateUts-0.2.9/run.py
+-rw-rw-rw-   0        0        0       42 2024-05-27 12:50:56.727212 dateUts-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      761 2024-05-27 12:49:49.000000 dateUts-0.2.9/setup.py
```

### Comparing `dateUts-0.2.8/CHANGELOG.txt` & `dateUts-0.2.9/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `dateUts-0.2.8/LICENCE.txt` & `dateUts-0.2.9/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `dateUts-0.2.8/PKG-INFO` & `dateUts-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dateUts
-Version: 0.2.8
+Version: 0.2.9
 Summary: Date package
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: dateUts
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,14 +20,17 @@
 #
 ### Installation
 
 ```sh
 pip install dateUts
 ```
 
+## GitHub
+https://github.com/ZdekPyPi/DateUts
+
 ### Usage
 #
 #### sqlToDate
 ```py
 from dateUts import sqlToDate
 result = sqlToDate('1991-12-23')
 print(result)
```

### Comparing `dateUts-0.2.8/README.md` & `dateUts-0.2.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 #
 ### Installation
 
 ```sh
 pip install dateUts
 ```
 
+## GitHub
+https://github.com/ZdekPyPi/DateUts
+
 ### Usage
 #
 #### sqlToDate
 ```py
 from dateUts import sqlToDate
 result = sqlToDate('1991-12-23')
 print(result)
```

### Comparing `dateUts-0.2.8/dateUts/__init__.py` & `dateUts-0.2.9/dateUts/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from datetime import date, datetime, timedelta as td
 from dateutil.relativedelta import relativedelta
 
-version = '0.2.8'
-
 class DateUts():
     date = None
 
     def __init__(self,date):
         self.date = date
 
     def is_weekend(self):
@@ -211,18 +209,7 @@
     
 
     
 
 Fnc_noWeekends = lambda dt:dt.weekday() not in [5,6]
 
 
-#print(interval(today(),tomorrow().date,in_seconds=True))
-#a = nextWorkingDate()
-#a = fmtDate("202306","%Y%m")
-#a = dateRange(firstDay(today()).date,lastDay(today()).date,filter_lbd = Fnc_noWeekends)
-#a[0].weekday()
-# a = DateUts(dt.now())
-# print(a)
-# a = lastWorkingDate(fmt="%Y-%m-%d")
-# rng = dateRange(sqlToDate("2022-05-01"),sqlToDate("2022-05-10"))
-# rng = dateRange(sqlToDate("2022-05-10"),sqlToDate("2022-05-01"))
-# a=1
```

### Comparing `dateUts-0.2.8/dateUts.egg-info/PKG-INFO` & `dateUts-0.2.9/dateUts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dateUts
-Version: 0.2.8
+Version: 0.2.9
 Summary: Date package
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: dateUts
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,14 +20,17 @@
 #
 ### Installation
 
 ```sh
 pip install dateUts
 ```
 
+## GitHub
+https://github.com/ZdekPyPi/DateUts
+
 ### Usage
 #
 #### sqlToDate
 ```py
 from dateUts import sqlToDate
 result = sqlToDate('1991-12-23')
 print(result)
```

### Comparing `dateUts-0.2.8/setup.py` & `dateUts-0.2.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='dateUts',
-  version='0.2.8',
+  version='0.2.9',
   description='Date package',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='',  
   author='Melque Lima',
   author_email='melque_ex@yahoo.com.br',
   license='MIT',
```

