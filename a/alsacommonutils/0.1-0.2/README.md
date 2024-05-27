# Comparing `tmp/alsacommonutils-0.1-py3-none-any.whl.zip` & `tmp/alsacommonutils-0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 3359 bytes, number of entries: 8
+Zip file size: 4483 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 24-May-05 13:17 alsacommonutils/__init__.py
 -rw-r--r--  2.0 unx     1419 b- defN 24-May-05 13:10 alsacommonutils/al_common_aws_utils.py
+-rw-r--r--  2.0 unx     2572 b- defN 24-May-27 08:40 alsacommonutils/al_common_emoji_skin_tone.py
 -rw-r--r--  2.0 unx      111 b- defN 24-May-05 13:11 alsacommonutils/al_common_utils.py
--rw-r--r--  2.0 unx     1074 b- defN 24-May-05 14:24 alsacommonutils-0.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      521 b- defN 24-May-05 14:24 alsacommonutils-0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-05 14:24 alsacommonutils-0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 24-May-05 14:24 alsacommonutils-0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      685 b- defN 24-May-05 14:24 alsacommonutils-0.1.dist-info/RECORD
-8 files, 3918 bytes uncompressed, 2145 bytes compressed:  45.3%
+-rw-r--r--  2.0 unx     1074 b- defN 24-May-27 08:45 alsacommonutils-0.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      619 b- defN 24-May-27 08:45 alsacommonutils-0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-27 08:45 alsacommonutils-0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 24-May-27 08:45 alsacommonutils-0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      786 b- defN 24-May-27 08:45 alsacommonutils-0.2.dist-info/RECORD
+9 files, 6689 bytes uncompressed, 3105 bytes compressed:  53.6%
```

## zipnote {}

```diff
@@ -1,25 +1,28 @@
 Filename: alsacommonutils/__init__.py
 Comment: 
 
 Filename: alsacommonutils/al_common_aws_utils.py
 Comment: 
 
+Filename: alsacommonutils/al_common_emoji_skin_tone.py
+Comment: 
+
 Filename: alsacommonutils/al_common_utils.py
 Comment: 
 
-Filename: alsacommonutils-0.1.dist-info/LICENSE.txt
+Filename: alsacommonutils-0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: alsacommonutils-0.1.dist-info/METADATA
+Filename: alsacommonutils-0.2.dist-info/METADATA
 Comment: 
 
-Filename: alsacommonutils-0.1.dist-info/WHEEL
+Filename: alsacommonutils-0.2.dist-info/WHEEL
 Comment: 
 
-Filename: alsacommonutils-0.1.dist-info/top_level.txt
+Filename: alsacommonutils-0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: alsacommonutils-0.1.dist-info/RECORD
+Filename: alsacommonutils-0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `alsacommonutils-0.1.dist-info/LICENSE.txt` & `alsacommonutils-0.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `alsacommonutils-0.1.dist-info/METADATA` & `alsacommonutils-0.2.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: alsacommonutils
-Version: 0.1
-Summary: Provides general useful common function as well as AWS specific functions
+Version: 0.2
+Summary: Provides general useful common function as well as AWS specific functions. Added the Fitzpatrick scale for emoji skin tone
 Home-page: https://al.co.za/
 Author: Autumn Leaf IT South Africa
 Author-email: jason@al.co.za
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-Provides general useful common function as well as AWS specific functions
+Provides general useful common function as well as AWS specific functions. Added the Fitzpatrick scale for emoji skin tone
```

## Comparing `alsacommonutils-0.1.dist-info/RECORD` & `alsacommonutils-0.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 alsacommonutils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 alsacommonutils/al_common_aws_utils.py,sha256=SkOQF95-J9CvOw_E2d6feouDmoSV-QeZ2znBr67s6kA,1419
+alsacommonutils/al_common_emoji_skin_tone.py,sha256=2ZVTSkcDzT-cn8MPvXj-o-Y1Ax9sfcXaJVlRfWTAzy8,2572
 alsacommonutils/al_common_utils.py,sha256=Iw1yaZmt0hqV4lrwWEenIf07ijQD-KELsIUI7ylCRrU,111
-alsacommonutils-0.1.dist-info/LICENSE.txt,sha256=5OMOiDRmwcyEnOdb28vYXr2yEjfnjwLfMFW8EuRMX4k,1074
-alsacommonutils-0.1.dist-info/METADATA,sha256=EZtnR2auvugcch6TurkXJgBhtjsiTN8FbZqUuy1roQw,521
-alsacommonutils-0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-alsacommonutils-0.1.dist-info/top_level.txt,sha256=Cp_y5PoEVQMuXXAVAvg8Vv8F26tb2C5x4EDoJb9UYtY,16
-alsacommonutils-0.1.dist-info/RECORD,,
+alsacommonutils-0.2.dist-info/LICENSE.txt,sha256=5OMOiDRmwcyEnOdb28vYXr2yEjfnjwLfMFW8EuRMX4k,1074
+alsacommonutils-0.2.dist-info/METADATA,sha256=WvGpcY5mDy6X7h35Oe8a_5wCx_fqajqbTnWfBJu4aCc,619
+alsacommonutils-0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+alsacommonutils-0.2.dist-info/top_level.txt,sha256=Cp_y5PoEVQMuXXAVAvg8Vv8F26tb2C5x4EDoJb9UYtY,16
+alsacommonutils-0.2.dist-info/RECORD,,
```

