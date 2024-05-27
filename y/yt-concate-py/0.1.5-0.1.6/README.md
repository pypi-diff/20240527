# Comparing `tmp/yt_concate_py-0.1.5-py3-none-any.whl.zip` & `tmp/yt_concate_py-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 14252 bytes, number of entries: 26
+Zip file size: 14237 bytes, number of entries: 26
 -rw-r--r--  2.0 unx        0 b- defN 23-Nov-10 19:05 yt_concate_py/__init__.py
 -rw-r--r--  2.0 unx      462 b- defN 24-Mar-04 23:29 yt_concate_py/logger.py
--rw-r--r--  2.0 unx     2647 b- defN 24-Mar-04 23:28 yt_concate_py/main.py
+-rw-r--r--  2.0 unx     2563 b- defN 24-May-27 15:49 yt_concate_py/main.py
 -rw-r--r--  2.0 unx      247 b- defN 24-Jan-12 09:09 yt_concate_py/settings.py
 -rw-r--r--  2.0 unx     1131 b- defN 24-Mar-04 23:28 yt_concate_py/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Mar-06 19:42 yt_concate_py/model/__init__.py
 -rw-r--r--  2.0 unx      467 b- defN 23-Dec-24 15:29 yt_concate_py/model/found.py
 -rw-r--r--  2.0 unx     1506 b- defN 24-Mar-04 23:28 yt_concate_py/model/yt.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 07:56 yt_concate_py/pipeline/__init__.py
 -rw-r--r--  2.0 unx      385 b- defN 24-Mar-04 23:28 yt_concate_py/pipeline/pipeline.py
@@ -16,13 +16,13 @@
 -rw-r--r--  2.0 unx     2176 b- defN 24-Mar-04 23:28 yt_concate_py/pipeline/steps/get_video_list.py
 -rw-r--r--  2.0 unx      298 b- defN 24-Mar-04 23:28 yt_concate_py/pipeline/steps/initialize_yt.py
 -rw-r--r--  2.0 unx      201 b- defN 24-Mar-04 23:28 yt_concate_py/pipeline/steps/postflight.py
 -rw-r--r--  2.0 unx      423 b- defN 24-Mar-04 23:28 yt_concate_py/pipeline/steps/prefligt.py
 -rw-r--r--  2.0 unx     1336 b- defN 24-Mar-04 23:28 yt_concate_py/pipeline/steps/read_captions.py
 -rw-r--r--  2.0 unx      736 b- defN 24-Mar-04 23:28 yt_concate_py/pipeline/steps/search.py
 -rw-r--r--  2.0 unx      228 b- defN 23-Dec-06 03:15 yt_concate_py/pipeline/steps/step.py
--rw-r--r--  2.0 unx     1066 b- defN 24-Mar-12 22:48 yt_concate_py-0.1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     4204 b- defN 24-Mar-12 22:48 yt_concate_py-0.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-12 22:48 yt_concate_py-0.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 24-Mar-12 22:48 yt_concate_py-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2330 b- defN 24-Mar-12 22:48 yt_concate_py-0.1.5.dist-info/RECORD
-26 files, 26089 bytes uncompressed, 10400 bytes compressed:  60.1%
+-rw-r--r--  2.0 unx     1066 b- defN 24-May-27 19:26 yt_concate_py-0.1.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4269 b- defN 24-May-27 19:26 yt_concate_py-0.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-27 19:26 yt_concate_py-0.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 24-May-27 19:26 yt_concate_py-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2330 b- defN 24-May-27 19:26 yt_concate_py-0.1.6.dist-info/RECORD
+26 files, 26070 bytes uncompressed, 10385 bytes compressed:  60.2%
```

## zipnote {}

```diff
@@ -57,23 +57,23 @@
 
 Filename: yt_concate_py/pipeline/steps/search.py
 Comment: 
 
 Filename: yt_concate_py/pipeline/steps/step.py
 Comment: 
 
-Filename: yt_concate_py-0.1.5.dist-info/LICENSE
+Filename: yt_concate_py-0.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: yt_concate_py-0.1.5.dist-info/METADATA
+Filename: yt_concate_py-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: yt_concate_py-0.1.5.dist-info/WHEEL
+Filename: yt_concate_py-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: yt_concate_py-0.1.5.dist-info/top_level.txt
+Filename: yt_concate_py-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: yt_concate_py-0.1.5.dist-info/RECORD
+Filename: yt_concate_py-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yt_concate_py/main.py

```diff
@@ -1,11 +1,10 @@
 import sys
 import getopt
 sys.path.append('../')
-sys.path.append('/Users/cindy/Desktop/yt-concate/venv/lib/python3.9/site-packages')
 
 from yt_concate_py.pipeline.pipeline import Pipeline
 from yt_concate_py.pipeline.steps.prefligt import Preflight
 from yt_concate_py.pipeline.steps.get_video_list import GetVideoList
 from yt_concate_py.pipeline.steps.initialize_yt import InitializeYT
 from yt_concate_py.pipeline.steps.download_captions import DownloadCaptions
 from yt_concate_py.pipeline.steps.read_captions import ReadCaptions
```

## Comparing `yt_concate_py-0.1.5.dist-info/LICENSE` & `yt_concate_py-0.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `yt_concate_py-0.1.5.dist-info/METADATA` & `yt_concate_py-0.1.6.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-concate-py
-Version: 0.1.5
+Version: 0.1.6
 Summary: Produce a consolidated video by concatenating YouTube video clips that mention a specific word.
 Home-page: https://github.com/whygreedy/yt-concate-py
 Author: Cindy Yeh
 Author-email: cindyyeah9@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -63,14 +63,18 @@
 ```bash
 virtualenv venv
 ```
 Activate venv
 ```bash
 source venv/bin/activate
 ```
+Install dependencies
+```bash
+pip install -r requirements.txt
+```
 Change directory to the folder that includes main.py file
 ```bash
 cd yt_concate_py
 ```
 Execute main.py file
 ```bash
 python3 main.py -c <channel_id> -s <search_term> -l <limit>
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yt-concate-py Version: 0.1.5 Summary: Produce a
+Metadata-Version: 2.1 Name: yt-concate-py Version: 0.1.6 Summary: Produce a
 consolidated video by concatenating YouTube video clips that mention a specific
 word. Home-page: https://github.com/whygreedy/yt-concate-py Author: Cindy Yeh
 Author-email: cindyyeah9@gmail.com License: MIT Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy Requires-
@@ -26,19 +26,20 @@
 subtitle option of a video) - supports for customizing the number of clips to
 be concatenated\ (Default number: 10) ## Quickstart ### Using the command line
 interface Clone this repo from GitHub to your local directory ```bash git clone
 https://github.com/whygreedy/yt-concate-py.git ``` Change directory to the repo
 folder just downloaded ```bash cd yt-concate-py ``` Add `.env file` that
 includes *your YouTube Data API Key* to the repo folder ``` # your .env file
 API_KEY= ``` Create venv ```bash virtualenv venv ``` Activate venv ```bash
-source venv/bin/activate ``` Change directory to the folder that includes
-main.py file ```bash cd yt_concate_py ``` Execute main.py file ```bash python3
-main.py -c -s -l ``` > If you want to concatenate a large number of clips, you
-could change ulimit to 2048 in terminal with command line `ulimit -n 2048` to
-avoid error message [Errno 24] Too many open files ### Using yt-concate-py in a
+source venv/bin/activate ``` Install dependencies ```bash pip install -
+r requirements.txt ``` Change directory to the folder that includes main.py
+file ```bash cd yt_concate_py ``` Execute main.py file ```bash python3 main.py
+-c -s -l ``` > If you want to concatenate a large number of clips, you could
+change ulimit to 2048 in terminal with command line `ulimit -n 2048` to avoid
+error message [Errno 24] Too many open files ### Using yt-concate-py in a
 Python script Create venv ```bash virtualenv venv ``` Activate venv ```bash
 source venv/bin/activate ``` Install from PyPI with pip ```bash pip install yt-
 concate-py ``` Add `.env file` that includes *your YouTube Data API Key* ``` #
 your .env file API_KEY= ``` Import the package and execute it with a Python
 Script ```python # your Python script from yt_concate_py import main main.main
 () ``` ## Example & Result Using the command line interface concatenate video
 clips that mentioned "BMW" from default [YouTube channel of Supercar Blondie]
```

## Comparing `yt_concate_py-0.1.5.dist-info/RECORD` & `yt_concate_py-0.1.6.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 yt_concate_py/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 yt_concate_py/logger.py,sha256=F6Qv3XaR_k7ir6PWPCQoikhRySLLBV1hsPjHVOxpeto,462
-yt_concate_py/main.py,sha256=0wQ2WNy_Cucn4b65mQM-FR9AkaWxC5ybdkNRAxKFxcc,2647
+yt_concate_py/main.py,sha256=MI0b2CTKA1psfEjUfHvocNAiBCuxDKRRioOqdLYqoQw,2563
 yt_concate_py/settings.py,sha256=4Zqg-QQBz9nqyRT6ewDrUANAO1sjU0hqpuxhX_VbLvw,247
 yt_concate_py/utils.py,sha256=bXfnC5mYWT7fpnW2Gb7566ZFfsu3bp2oXy1ATiJt4WY,1131
 yt_concate_py/model/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 yt_concate_py/model/found.py,sha256=Rua0g6uJYWumUGPgOWM5CKv-x-9lkHpEiHQMBFP5wWY,467
 yt_concate_py/model/yt.py,sha256=h9xTGkAxr9WNKHeeR3TQwzBPQ7NFhKDapm9VVzmVI0I,1506
 yt_concate_py/pipeline/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 yt_concate_py/pipeline/pipeline.py,sha256=JUn9P1KsA74PLuZ429N6fz7v_IbnLKcGd3JFkfLVZEY,385
@@ -15,12 +15,12 @@
 yt_concate_py/pipeline/steps/get_video_list.py,sha256=UZOVE9ouFOCbHfS7sv9mDlt0KxUqL7Pbp4Ylcyylyo0,2176
 yt_concate_py/pipeline/steps/initialize_yt.py,sha256=OFknZ0YlZifB7U1lyU49TkXIj4kJGQMb7Q6dymYRwr8,298
 yt_concate_py/pipeline/steps/postflight.py,sha256=6ZAHYbWacSWrGBC9YAAY0y_yCMq6bKUSZsxkw2UalIw,201
 yt_concate_py/pipeline/steps/prefligt.py,sha256=52PeO1gQ2KRRlj4bSr8EmO8IR4-TUPE0eU6h_LTAZ20,423
 yt_concate_py/pipeline/steps/read_captions.py,sha256=5VeOjWaK2JiZPk-30ZLm0NxLSz7mvzWY5zgbUsdi7x8,1336
 yt_concate_py/pipeline/steps/search.py,sha256=8MSrAEsT1Sqh8vRaL9mGzxgnQ4MbaNb2ujAXxJ-nCeM,736
 yt_concate_py/pipeline/steps/step.py,sha256=Op8BukqYt8fcDBCRLqptpkr3gCj0NP-1g8b4578lmuc,228
-yt_concate_py-0.1.5.dist-info/LICENSE,sha256=wbc6JmiTg5jU1fjiMr9pqDl5tM80Byo1_0nmhyze-no,1066
-yt_concate_py-0.1.5.dist-info/METADATA,sha256=-lJbCnw-fFwkIRKYMlNnyblG-JCWXRXQ0Mr86_URLq0,4204
-yt_concate_py-0.1.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-yt_concate_py-0.1.5.dist-info/top_level.txt,sha256=9ZsUxNOhV5Fzj7Rhs7HvGnK-b6YxQgoJIq5qOt92oo0,14
-yt_concate_py-0.1.5.dist-info/RECORD,,
+yt_concate_py-0.1.6.dist-info/LICENSE,sha256=wbc6JmiTg5jU1fjiMr9pqDl5tM80Byo1_0nmhyze-no,1066
+yt_concate_py-0.1.6.dist-info/METADATA,sha256=wIyDfjdHxVvh155j_Fs-xsOxMk-rbZuUqtjsAOJjV44,4269
+yt_concate_py-0.1.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+yt_concate_py-0.1.6.dist-info/top_level.txt,sha256=9ZsUxNOhV5Fzj7Rhs7HvGnK-b6YxQgoJIq5qOt92oo0,14
+yt_concate_py-0.1.6.dist-info/RECORD,,
```

