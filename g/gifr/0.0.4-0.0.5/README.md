# Comparing `tmp/gifr-0.0.4.tar.gz` & `tmp/gifr-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gifr-0.0.4.tar", last modified: Tue Feb 27 03:20:37 2024, max compression
+gzip compressed data, was "gifr-0.0.5.tar", last modified: Mon May 27 04:38:02 2024, max compression
```

## Comparing `gifr-0.0.4.tar` & `gifr-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-02-27 03:20:37.960017 gifr-0.0.4/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      539 2024-02-27 03:19:41.000000 gifr-0.0.4/CHANGES.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      393 2024-02-13 21:25:01.000000 gifr-0.0.4/DESCRIPTION.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 gifr-0.0.4/MANIFEST.in
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1775 2024-02-27 03:20:37.960017 gifr-0.0.4/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    15029 2024-02-27 03:06:10.000000 gifr-0.0.4/README.md
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2024-02-27 03:20:37.960017 gifr-0.0.4/setup.cfg
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1433 2024-02-27 03:19:41.000000 gifr-0.0.4/setup.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-02-27 03:20:37.956017 gifr-0.0.4/src/
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-02-27 03:20:37.960017 gifr-0.0.4/src/gifr/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2023-10-30 02:28:46.000000 gifr-0.0.4/src/gifr/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     4138 2023-11-02 03:43:18.000000 gifr-0.0.4/src/gifr/colors.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     7454 2023-11-12 00:01:32.000000 gifr-0.0.4/src/gifr/common.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1255 2023-11-02 03:53:09.000000 gifr-0.0.4/src/gifr/fonts.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2940 2023-11-12 00:04:23.000000 gifr-0.0.4/src/gifr/image_classification.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6592 2023-11-12 00:04:23.000000 gifr-0.0.4/src/gifr/image_segmentation.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    10904 2023-11-12 00:04:23.000000 gifr-0.0.4/src/gifr/object_detection.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3113 2024-02-15 00:30:01.000000 gifr-0.0.4/src/gifr/text_classification.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5737 2024-02-27 03:05:43.000000 gifr-0.0.4/src/gifr/text_generation.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-02-27 03:20:37.960017 gifr-0.0.4/src/gifr.egg-info/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1775 2024-02-27 03:20:37.000000 gifr-0.0.4/src/gifr.egg-info/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      482 2024-02-27 03:20:37.000000 gifr-0.0.4/src/gifr.egg-info/SOURCES.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2024-02-27 03:20:37.000000 gifr-0.0.4/src/gifr.egg-info/dependency_links.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      256 2024-02-27 03:20:37.000000 gifr-0.0.4/src/gifr.egg-info/entry_points.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       18 2024-02-27 03:20:37.000000 gifr-0.0.4/src/gifr.egg-info/requires.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        5 2024-02-27 03:20:37.000000 gifr-0.0.4/src/gifr.egg-info/top_level.txt
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-27 04:38:02.045384 gifr-0.0.5/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      637 2024-05-27 04:35:04.000000 gifr-0.0.5/CHANGES.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      430 2024-05-27 04:31:21.000000 gifr-0.0.5/DESCRIPTION.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 gifr-0.0.5/MANIFEST.in
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1966 2024-05-27 04:38:02.045384 gifr-0.0.5/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    17039 2024-05-27 04:36:31.000000 gifr-0.0.5/README.md
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2024-05-27 04:38:02.045384 gifr-0.0.5/setup.cfg
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1492 2024-05-27 04:35:04.000000 gifr-0.0.5/setup.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-27 04:38:02.045384 gifr-0.0.5/src/
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-27 04:38:02.045384 gifr-0.0.5/src/gifr/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2023-10-30 02:28:46.000000 gifr-0.0.5/src/gifr/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3157 2024-05-27 04:31:32.000000 gifr-0.0.5/src/gifr/asr.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4138 2023-11-02 03:43:18.000000 gifr-0.0.5/src/gifr/colors.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     7454 2023-11-12 00:01:32.000000 gifr-0.0.5/src/gifr/common.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1255 2023-11-02 03:53:09.000000 gifr-0.0.5/src/gifr/fonts.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2940 2023-11-12 00:04:23.000000 gifr-0.0.5/src/gifr/image_classification.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6592 2023-11-12 00:04:23.000000 gifr-0.0.5/src/gifr/image_segmentation.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    10904 2023-11-12 00:04:23.000000 gifr-0.0.5/src/gifr/object_detection.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3113 2024-02-15 00:30:01.000000 gifr-0.0.5/src/gifr/text_classification.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     5737 2024-02-27 03:05:43.000000 gifr-0.0.5/src/gifr/text_generation.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-27 04:38:02.045384 gifr-0.0.5/src/gifr.egg-info/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1966 2024-05-27 04:38:01.000000 gifr-0.0.5/src/gifr.egg-info/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      498 2024-05-27 04:38:02.000000 gifr-0.0.5/src/gifr.egg-info/SOURCES.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2024-05-27 04:38:01.000000 gifr-0.0.5/src/gifr.egg-info/dependency_links.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      285 2024-05-27 04:38:01.000000 gifr-0.0.5/src/gifr.egg-info/entry_points.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       24 2024-05-27 04:38:01.000000 gifr-0.0.5/src/gifr.egg-info/requires.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        5 2024-05-27 04:38:01.000000 gifr-0.0.5/src/gifr.egg-info/top_level.txt
```

### Comparing `gifr-0.0.4/CHANGES.rst` & `gifr-0.0.5/CHANGES.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+0.0.5 (2024-05-27)
+------------------
+
+- added interface for automatic speech recognition (ASR)
+
+
 0.0.4 (2024-02-27)
 ------------------
 
 - extended text generation interface to keep track of inputs and #turns (*history*);
   added support for JSON responses; field name in JSON prompt is now customizable
```

### Comparing `gifr-0.0.4/PKG-INFO` & `gifr-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 Metadata-Version: 1.1
 Name: gifr
-Version: 0.0.4
+Version: 0.0.5
 Summary: gradio interfaces for Deep Learning Docker images that use Redis for receiving data to make predictions on.
 Home-page: https://github.com/waikato-datamining/gifr
 Author: Peter Reutemann
 Author-email: fracpete@waikato.ac.nz
 License: MIT License
 Description: `gradio <https://www.gradio.app/>`__ interfaces for Deep Learning Docker images that
         use Redis for receiving data to make predictions on.
         
         `https://www.data-mining.co.nz/docker-images/ <https://www.data-mining.co.nz/docker-images/>`__
         
         Interfaces are available for:
         
+        - automatic speech recognition (ASR)
         - image classification
         - image segmentation
         - object detection/instance segmentation
         - text classification
         - text generation
         
         
         Changelog
         =========
         
+        0.0.5 (2024-05-27)
+        ------------------
+        
+        - added interface for automatic speech recognition (ASR)
+        
+        
         0.0.4 (2024-02-27)
         ------------------
         
         - extended text generation interface to keep track of inputs and #turns (*history*);
           added support for JSON responses; field name in JSON prompt is now customizable
```

### Comparing `gifr-0.0.4/README.md` & `gifr-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,54 @@
 * [Image segmentation](https://www.data-mining.co.nz/applied-deep-learning/image_segmentation/)
 * [Instance segmentation](https://www.data-mining.co.nz/applied-deep-learning/instance_segmentation/) (can use Object detection interface as well)  
 * [Object detection](https://www.data-mining.co.nz/applied-deep-learning/object_detection/)
 
 
 ## Interfaces
 
+### Automatic Speech Recognition (ASR)
+
+![Screenshot automatic speech recognition](doc/img/asr.png)
+
+```
+usage: gifr-asr [-h] [--redis_host HOST] [--redis_port PORT] [--redis_db DB]
+                [--model_channel_in CHANNEL] [--model_channel_out CHANNEL]
+                [--timeout SECONDS] [--title TITLE] [--description DESC]
+                [--launch_browser] [--share_interface]
+                [--logging_level {DEBUG,INFO,WARN,ERROR,CRITICAL}]
+
+Automatic Speech Recognition (ASR) interface. Allows the user to enter text
+and display the text transcribed by the model.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --redis_host HOST     The host with the redis server. (default: localhost)
+  --redis_port PORT     The port of the redis server. (default: 6379)
+  --redis_db DB         The redis database to use. (default: 0)
+  --model_channel_in CHANNEL
+                        The channel to send the data to for making
+                        predictions. (default: audio)
+  --model_channel_out CHANNEL
+                        The channel to receive the predictions on. (default:
+                        transcription)
+  --timeout SECONDS     The number of seconds to wait for a prediction.
+                        (default: 2.0)
+  --title TITLE         The title to use for interface. (default: Automatic
+                        Speech Recognition (ASR))
+  --description DESC    The description to use in the interface. (default:
+                        Sends the recorded/uploaded audio to the model to
+                        transcribe and displays the result.)
+  --launch_browser      Whether to automatically launch the interface in a new
+                        tab of the default browser. (default: False)
+  --share_interface     Whether to publicly share the interface at
+                        https://XYZ.gradio.live/. (default: False)
+  --logging_level {DEBUG,INFO,WARN,ERROR,CRITICAL}
+                        The logging level to use (default: WARN)
+```
+
 ### Image classification
 
 ![Screenshot image classification](doc/img/imgcls.png)
 
 ```
 usage: gifr-imgcls [-h] [--redis_host HOST] [--redis_port PORT]
                    [--redis_db DB] [--model_channel_in CHANNEL]
```

### Comparing `gifr-0.0.4/setup.py` & `gifr-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,20 +30,22 @@
         '': 'src'
     },
     packages=find_namespace_packages(where='src'),
     install_requires=[
         "gradio",
         "redis",
         "opex",
+        "scipy",
     ],
-    version="0.0.4",
+    version="0.0.5",
     author='Peter Reutemann',
     author_email='fracpete@waikato.ac.nz',
     entry_points={
         "console_scripts": [
+            "gifr-asr=gifr.asr:sys_main",
             "gifr-imgcls=gifr.image_classification:sys_main",
             "gifr-imgseg=gifr.image_segmentation:sys_main",
             "gifr-objdet=gifr.object_detection:sys_main",
             "gifr-textclass=gifr.text_classification:sys_main",
             "gifr-textgen=gifr.text_generation:sys_main",
         ],
     },
```

### Comparing `gifr-0.0.4/src/gifr/colors.py` & `gifr-0.0.5/src/gifr/colors.py`

 * *Files identical despite different names*

### Comparing `gifr-0.0.4/src/gifr/common.py` & `gifr-0.0.5/src/gifr/common.py`

 * *Files identical despite different names*

### Comparing `gifr-0.0.4/src/gifr/fonts.py` & `gifr-0.0.5/src/gifr/fonts.py`

 * *Files identical despite different names*

### Comparing `gifr-0.0.4/src/gifr/image_classification.py` & `gifr-0.0.5/src/gifr/image_classification.py`

 * *Files identical despite different names*

### Comparing `gifr-0.0.4/src/gifr/image_segmentation.py` & `gifr-0.0.5/src/gifr/image_segmentation.py`

 * *Files identical despite different names*

### Comparing `gifr-0.0.4/src/gifr/object_detection.py` & `gifr-0.0.5/src/gifr/object_detection.py`

 * *Files identical despite different names*

### Comparing `gifr-0.0.4/src/gifr/text_classification.py` & `gifr-0.0.5/src/gifr/text_classification.py`

 * *Files identical despite different names*

### Comparing `gifr-0.0.4/src/gifr/text_generation.py` & `gifr-0.0.5/src/gifr/text_generation.py`

 * *Files identical despite different names*

### Comparing `gifr-0.0.4/src/gifr.egg-info/PKG-INFO` & `gifr-0.0.5/src/gifr.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 Metadata-Version: 1.1
 Name: gifr
-Version: 0.0.4
+Version: 0.0.5
 Summary: gradio interfaces for Deep Learning Docker images that use Redis for receiving data to make predictions on.
 Home-page: https://github.com/waikato-datamining/gifr
 Author: Peter Reutemann
 Author-email: fracpete@waikato.ac.nz
 License: MIT License
 Description: `gradio <https://www.gradio.app/>`__ interfaces for Deep Learning Docker images that
         use Redis for receiving data to make predictions on.
         
         `https://www.data-mining.co.nz/docker-images/ <https://www.data-mining.co.nz/docker-images/>`__
         
         Interfaces are available for:
         
+        - automatic speech recognition (ASR)
         - image classification
         - image segmentation
         - object detection/instance segmentation
         - text classification
         - text generation
         
         
         Changelog
         =========
         
+        0.0.5 (2024-05-27)
+        ------------------
+        
+        - added interface for automatic speech recognition (ASR)
+        
+        
         0.0.4 (2024-02-27)
         ------------------
         
         - extended text generation interface to keep track of inputs and #turns (*history*);
           added support for JSON responses; field name in JSON prompt is now customizable
```

