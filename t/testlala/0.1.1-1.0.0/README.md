# Comparing `tmp/testlala-0.1.1-py3-none-any.whl.zip` & `tmp/testlala-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,6 @@
-Zip file size: 1834 bytes, number of entries: 7
--rw-r--r--  2.0 unx       19 b- defN 24-May-27 06:55 test/__init__.py
--rw-r--r--  2.0 unx       77 b- defN 24-May-27 08:13 test/lala.py
--rw-r--r--  2.0 unx      449 b- defN 24-May-27 09:40 testlala-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-27 09:40 testlala-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       62 b- defN 24-May-27 09:40 testlala-0.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 24-May-27 09:40 testlala-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      534 b- defN 24-May-27 09:40 testlala-0.1.1.dist-info/RECORD
-7 files, 1238 bytes uncompressed, 878 bytes compressed:  29.1%
+Zip file size: 1045 bytes, number of entries: 4
+-rw-r--r--  2.0 unx      209 b- defN 24-May-27 10:02 testlala-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-27 10:02 testlala-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-27 10:02 testlala-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      300 b- defN 24-May-27 10:02 testlala-1.0.0.dist-info/RECORD
+4 files, 602 bytes uncompressed, 455 bytes compressed:  24.4%
```

## zipnote {}

```diff
@@ -1,22 +1,13 @@
-Filename: test/__init__.py
+Filename: testlala-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: test/lala.py
+Filename: testlala-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: testlala-0.1.1.dist-info/METADATA
+Filename: testlala-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: testlala-0.1.1.dist-info/WHEEL
-Comment: 
-
-Filename: testlala-0.1.1.dist-info/entry_points.txt
-Comment: 
-
-Filename: testlala-0.1.1.dist-info/top_level.txt
-Comment: 
-
-Filename: testlala-0.1.1.dist-info/RECORD
+Filename: testlala-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

