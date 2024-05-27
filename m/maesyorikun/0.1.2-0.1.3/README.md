# Comparing `tmp/maesyorikun-0.1.2-py3-none-any.whl.zip` & `tmp/maesyorikun-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4460 bytes, number of entries: 7
--rw-r--r--  2.0 unx      222 b- defN 24-May-26 22:25 maesyorikun/__init__.py
+Zip file size: 4458 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      222 b- defN 24-May-26 23:11 maesyorikun/__init__.py
 -rw-r--r--  2.0 unx     7443 b- defN 24-May-26 21:00 maesyorikun/maesyorikun.py
 -rw-r--r--  2.0 unx      135 b- defN 24-May-26 21:17 maesyorikun/test.py
--rw-r--r--  2.0 unx     1747 b- defN 24-May-26 22:25 maesyorikun-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-26 22:25 maesyorikun-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-May-26 22:25 maesyorikun-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      551 b- defN 24-May-26 22:25 maesyorikun-0.1.2.dist-info/RECORD
-7 files, 10202 bytes uncompressed, 3482 bytes compressed:  65.9%
+-rw-r--r--  2.0 unx     1747 b- defN 24-May-26 23:12 maesyorikun-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-26 23:12 maesyorikun-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-26 23:12 maesyorikun-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      551 b- defN 24-May-26 23:12 maesyorikun-0.1.3.dist-info/RECORD
+7 files, 10202 bytes uncompressed, 3480 bytes compressed:  65.9%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: maesyorikun/maesyorikun.py
 Comment: 
 
 Filename: maesyorikun/test.py
 Comment: 
 
-Filename: maesyorikun-0.1.2.dist-info/METADATA
+Filename: maesyorikun-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: maesyorikun-0.1.2.dist-info/WHEEL
+Filename: maesyorikun-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: maesyorikun-0.1.2.dist-info/top_level.txt
+Filename: maesyorikun-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: maesyorikun-0.1.2.dist-info/RECORD
+Filename: maesyorikun-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## maesyorikun/__init__.py

```diff
@@ -1,8 +1,8 @@
 from .maesyorikun import *
 
 __copyright__    = 'Copyright (C) 2024 makimoto eita'
-__version__      = '0.1.2'
+__version__      = '0.1.3'
 __author__       = 'Makimoto-eita'
 __author_email__ = 's2222034@stu.musahino-u.ac.jp'
 
 __all__ = ['maesyorikun']
```

## Comparing `maesyorikun-0.1.2.dist-info/METADATA` & `maesyorikun-0.1.3.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maesyorikun
-Version: 0.1.2
+Version: 0.1.3
 Summary: This app can interactively preprocess and graph CSV data.
 Home-page: UNKNOWN
 Author: Makimoto-eita
 Author-email: s2222034@stu.musashino-u.ac.jp
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

