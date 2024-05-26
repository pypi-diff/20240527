# Comparing `tmp/maesyorikun-0.1.0-py3-none-any.whl.zip` & `tmp/maesyorikun-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 3508 bytes, number of entries: 6
--rw-r--r--  2.0 unx      222 b- defN 24-May-26 20:59 maesyorikun/__init__.py
+Zip file size: 3744 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      222 b- defN 24-May-26 22:15 maesyorikun/__init__.py
 -rw-r--r--  2.0 unx     7443 b- defN 24-May-26 21:00 maesyorikun/maesyorikun.py
--rw-r--r--  2.0 unx      493 b- defN 24-May-26 21:03 maesyorikun-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-26 21:03 maesyorikun-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-May-26 21:03 maesyorikun-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      475 b- defN 24-May-26 21:03 maesyorikun-0.1.0.dist-info/RECORD
-6 files, 8737 bytes uncompressed, 2644 bytes compressed:  69.7%
+-rw-r--r--  2.0 unx      135 b- defN 24-May-26 21:17 maesyorikun/test.py
+-rw-r--r--  2.0 unx      493 b- defN 24-May-26 22:16 maesyorikun-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-26 22:16 maesyorikun-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-26 22:16 maesyorikun-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      550 b- defN 24-May-26 22:16 maesyorikun-0.1.1.dist-info/RECORD
+7 files, 8947 bytes uncompressed, 2766 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
 Filename: maesyorikun/__init__.py
 Comment: 
 
 Filename: maesyorikun/maesyorikun.py
 Comment: 
 
-Filename: maesyorikun-0.1.0.dist-info/METADATA
+Filename: maesyorikun/test.py
 Comment: 
 
-Filename: maesyorikun-0.1.0.dist-info/WHEEL
+Filename: maesyorikun-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: maesyorikun-0.1.0.dist-info/top_level.txt
+Filename: maesyorikun-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: maesyorikun-0.1.0.dist-info/RECORD
+Filename: maesyorikun-0.1.1.dist-info/top_level.txt
+Comment: 
+
+Filename: maesyorikun-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## maesyorikun/__init__.py

```diff
@@ -1,8 +1,8 @@
 from .maesyorikun import *
 
 __copyright__    = 'Copyright (C) 2024 makimoto eita'
-__version__      = '0.1.0'
+__version__      = '0.1.1'
 __author__       = 'Makimoto-eita'
 __author_email__ = 's2222034@stu.musahino-u.ac.jp'
 
 __all__ = ['maesyorikun']
```

