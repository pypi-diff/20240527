# Comparing `tmp/dragonion-1.0.1-py3-none-any.whl.zip` & `tmp/dragonion-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -62,12 +62,12 @@
 -rw-r--r--  2.0 unx     2825 b- defN 80-Jan-01 00:00 dragonion/utils/core/dirs.py
 -rw-r--r--  2.0 unx      700 b- defN 80-Jan-01 00:00 dragonion/utils/core/emoji.py
 -rw-r--r--  2.0 unx       46 b- defN 80-Jan-01 00:00 dragonion/utils/onion/__init__.py
 -rw-r--r--  2.0 unx     1147 b- defN 80-Jan-01 00:00 dragonion/utils/onion/auth.py
 -rw-r--r--  2.0 unx     6690 b- defN 80-Jan-01 00:00 dragonion/utils/onion/onion.py
 -rw-r--r--  2.0 unx    11047 b- defN 80-Jan-01 00:00 dragonion/utils/onion/stem_process.py
 -rw-r--r--  2.0 unx     2312 b- defN 80-Jan-01 00:00 dragonion/utils/onion/tor_downloader.py
--rw-r--r--  2.0 unx    29464 b- defN 80-Jan-01 00:00 dragonion-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 dragonion-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 80-Jan-01 00:00 dragonion-1.0.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     7512 b- defN 16-Jan-01 00:00 dragonion-1.0.1.dist-info/RECORD
+-rw-r--r--  2.0 unx    29464 b- defN 80-Jan-01 00:00 dragonion-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 dragonion-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 80-Jan-01 00:00 dragonion-1.0.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     7512 b- defN 16-Jan-01 00:00 dragonion-1.0.2.dist-info/RECORD
 71 files, 101007 bytes uncompressed, 29891 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -195,20 +195,20 @@
 
 Filename: dragonion/utils/onion/stem_process.py
 Comment: 
 
 Filename: dragonion/utils/onion/tor_downloader.py
 Comment: 
 
-Filename: dragonion-1.0.1.dist-info/METADATA
+Filename: dragonion-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: dragonion-1.0.1.dist-info/WHEEL
+Filename: dragonion-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: dragonion-1.0.1.dist-info/entry_points.txt
+Filename: dragonion-1.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: dragonion-1.0.1.dist-info/RECORD
+Filename: dragonion-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `dragonion-1.0.1.dist-info/METADATA` & `dragonion-1.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonion
-Version: 1.0.1
+Version: 1.0.2
 Summary: Most modern-looking, encrypted and functional in-console onion chat that you control!
 Author: BarsTiger
 Author-email: zxcbarstiger@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

## Comparing `dragonion-1.0.1.dist-info/RECORD` & `dragonion-1.0.2.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -61,11 +61,11 @@
 dragonion/utils/core/dirs.py,sha256=c9N5OdLxKwnZuYRDpk_uYXVUTJsia_6svliOWklLQiA,2825
 dragonion/utils/core/emoji.py,sha256=ynbNOPtXaPBvbTisXZCxouwBDZ2B6LdbOlNgttbHetE,700
 dragonion/utils/onion/__init__.py,sha256=ZpDhqmhmEmgK8DB-MEBYJc8oUMah-3hrdFYHROaAZos,46
 dragonion/utils/onion/auth.py,sha256=L9YUWRUpvwVLSCDOQtFZ5w9OGLppB5lAnNmGG9JOE5o,1147
 dragonion/utils/onion/onion.py,sha256=pT0wUq-O5hRGHxdHCI1wEffKha31VQlOxvJhSX15pNY,6690
 dragonion/utils/onion/stem_process.py,sha256=Mi4jCU2066aU8yx3rJd91yZr24jo47vvAF6HAz_qbPk,11047
 dragonion/utils/onion/tor_downloader.py,sha256=P-6OMYr_NTS37CBKwMd3LAieWLw0ChmL7whDx-IlG7Y,2312
-dragonion-1.0.1.dist-info/METADATA,sha256=E37HLDF__X89H7P75n3H6ESVhnrAVLVfW_vXeW39cqY,29464
-dragonion-1.0.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-dragonion-1.0.1.dist-info/entry_points.txt,sha256=JVx0FGUdz6RQu1_M4biP7bmduOt6v6Bl8wnAnGZZ9BQ,44
-dragonion-1.0.1.dist-info/RECORD,,
+dragonion-1.0.2.dist-info/METADATA,sha256=aVqtQqqB8pNtPgg9xA1wiUX0VWYcj7VhT6lAtczcQK4,29464
+dragonion-1.0.2.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+dragonion-1.0.2.dist-info/entry_points.txt,sha256=JVx0FGUdz6RQu1_M4biP7bmduOt6v6Bl8wnAnGZZ9BQ,44
+dragonion-1.0.2.dist-info/RECORD,,
```

