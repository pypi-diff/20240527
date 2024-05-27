# Comparing `tmp/video_background_extractor-1.1.0-py3-none-any.whl.zip` & `tmp/video_background_extractor-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,10 @@
-Zip file size: 4378 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     1094 b- defN 24-May-27 02:35 video_background_extractor-1.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6101 b- defN 24-May-27 02:35 video_background_extractor-1.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-27 02:35 video_background_extractor-1.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-May-27 02:35 video_background_extractor-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      480 b- defN 24-May-27 02:35 video_background_extractor-1.1.0.dist-info/RECORD
-5 files, 7775 bytes uncompressed, 3468 bytes compressed:  55.4%
+Zip file size: 6811 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      170 b- defN 24-May-23 02:08 video_background_extractor/Types.py
+-rw-rw-rw-  2.0 fat     8053 b- defN 24-May-26 20:27 video_background_extractor/VideoBackgroundExtractor.py
+-rw-rw-rw-  2.0 fat       64 b- defN 24-May-23 02:08 video_background_extractor/__init__.py
+-rw-rw-rw-  2.0 fat     1094 b- defN 24-May-27 02:46 video_background_extractor-1.1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6166 b- defN 24-May-27 02:46 video_background_extractor-1.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-27 02:46 video_background_extractor-1.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       27 b- defN 24-May-27 02:46 video_background_extractor-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      776 b- defN 24-May-27 02:46 video_background_extractor-1.1.1.dist-info/RECORD
+8 files, 16442 bytes uncompressed, 5419 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -1,16 +1,25 @@
-Filename: video_background_extractor-1.1.0.dist-info/LICENSE
+Filename: video_background_extractor/Types.py
 Comment: 
 
-Filename: video_background_extractor-1.1.0.dist-info/METADATA
+Filename: video_background_extractor/VideoBackgroundExtractor.py
 Comment: 
 
-Filename: video_background_extractor-1.1.0.dist-info/WHEEL
+Filename: video_background_extractor/__init__.py
 Comment: 
 
-Filename: video_background_extractor-1.1.0.dist-info/top_level.txt
+Filename: video_background_extractor-1.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: video_background_extractor-1.1.0.dist-info/RECORD
+Filename: video_background_extractor-1.1.1.dist-info/METADATA
+Comment: 
+
+Filename: video_background_extractor-1.1.1.dist-info/WHEEL
+Comment: 
+
+Filename: video_background_extractor-1.1.1.dist-info/top_level.txt
+Comment: 
+
+Filename: video_background_extractor-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `video_background_extractor-1.1.0.dist-info/LICENSE` & `video_background_extractor-1.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `video_background_extractor-1.1.0.dist-info/METADATA` & `video_background_extractor-1.1.1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video-background-extractor
-Version: 1.1.0
+Version: 1.1.1
 Summary: Library to extract background from static video. 
 Author-email: Henrique Schmitz <sch.henrique@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Henrique Schmitz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -91,14 +91,15 @@
 
 **Original Image:**
 ![Original Image](https://github.com/HenriqueSchmitz/VideoBackgroundExtractor/blob/main/samples/originalImage.png?raw=true)
 
 Getting background from video:
 
 ```
+from video_background_extractor import VideoBackgroundExtractor
 extractor = VideoBackgroundExtractor()
 extractor.loadVideo(video)
 background = extractor.getBackgroundFrame()
 ```
 
 **Background Extracted from Video:**
 ![Background from Video](https://github.com/HenriqueSchmitz/VideoBackgroundExtractor/blob/main/samples/background.png?raw=true)
```

