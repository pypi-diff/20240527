# Comparing `tmp/edurpa_document-0.0.4-py3-none-any.whl.zip` & `tmp/edurpa_document-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6052 bytes, number of entries: 9
+Zip file size: 6072 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-28 07:01 EduRPA/__init__.py
--rw-rw-rw-  2.0 fat     4982 b- defN 24-May-25 10:20 EduRPA/Document/DocumentAutomation.py
--rw-rw-rw-  2.0 fat      428 b- defN 24-Apr-28 06:21 EduRPA/Document/__init__.py
+-rw-rw-rw-  2.0 fat     4923 b- defN 24-May-27 14:38 EduRPA/Document/DocumentAutomation.py
+-rw-rw-rw-  2.0 fat      540 b- defN 24-May-27 14:39 EduRPA/Document/__init__.py
 -rw-rw-rw-  2.0 fat     2624 b- defN 24-Apr-28 06:18 EduRPA/Document/transform.py
--rw-rw-rw-  2.0 fat     1088 b- defN 24-May-25 10:20 edurpa_document-0.0.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2019 b- defN 24-May-25 10:20 edurpa_document-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-25 10:20 edurpa_document-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 24-May-25 10:20 edurpa_document-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      759 b- defN 24-May-25 10:20 edurpa_document-0.0.4.dist-info/RECORD
-9 files, 11999 bytes uncompressed, 4728 bytes compressed:  60.6%
+-rw-rw-rw-  2.0 fat     1088 b- defN 24-May-27 14:39 edurpa_document-0.0.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2019 b- defN 24-May-27 14:39 edurpa_document-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-27 14:39 edurpa_document-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 24-May-27 14:39 edurpa_document-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      759 b- defN 24-May-27 14:39 edurpa_document-0.0.5.dist-info/RECORD
+9 files, 12052 bytes uncompressed, 4748 bytes compressed:  60.6%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: EduRPA/Document/__init__.py
 Comment: 
 
 Filename: EduRPA/Document/transform.py
 Comment: 
 
-Filename: edurpa_document-0.0.4.dist-info/LICENSE
+Filename: edurpa_document-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: edurpa_document-0.0.4.dist-info/METADATA
+Filename: edurpa_document-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: edurpa_document-0.0.4.dist-info/WHEEL
+Filename: edurpa_document-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: edurpa_document-0.0.4.dist-info/top_level.txt
+Filename: edurpa_document-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: edurpa_document-0.0.4.dist-info/RECORD
+Filename: edurpa_document-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## EduRPA/Document/DocumentAutomation.py

```diff
@@ -2,20 +2,18 @@
 from vietocr.tool.config import Cfg
 from PIL import Image
 from robot.api.deco import keyword, not_keyword
 import cv2
 import json
 from openpyxl import Workbook
 from datetime import datetime
-
 from .transform import perspective_transform, resize_image
-from robot.libraries.BuiltIn import BuiltIn
 class DocumentAutomation:
-    def __init__(self, lang, performance, *args, **kwargs):
-        if BuiltIn.dry_run_active:
+    def __init__(self, lang, performance, **kwargs):
+        if kwargs["dryrun"]:
             # If running dryrun, ignore initialization
             return
         
         cfg = Cfg.load_config_from_name("vgg_seq2seq")
         cfg["device"] = "cpu"
         vgg_seq2seq = Predictor(cfg)
 
@@ -56,15 +54,15 @@
         for label, image in labeled_images.items():
             print("Predicting label", label)
             prediction = self.predictor.predict(Image.fromarray(image))
             results[label] = prediction
 
         return results
     
-    @keyword("Extract Data From Document", types={'file_name': 'str', 'template': 'str'})
+    @keyword("Extract Data From Document", types={'file_name': 'str', 'template': 'dict'})
     def extract_data_from_document(self, file_name, template):
         if type (template) is str:
             template = json.loads(template)
         
         # read and preprocess document (image type)
         document = cv2.imread(file_name)
         document = self.image_preprocessing(document, template)
```

## EduRPA/Document/__init__.py

```diff
@@ -1,15 +1,19 @@
 name = 'edurpa_document'
 from .DocumentAutomation import *
 from .transform import *
 
 from robotlibcore import DynamicCore
-
+from robot.libraries.BuiltIn import BuiltIn
 class Document(DynamicCore):
     def __init__(
-        self, lang, performance, *args, **kwargs
+        self, lang, performance, **kwargs
     ):
         # Register keyword libraries to LibCore
+        kwargs = {
+            "dryrun": BuiltIn().dry_run_active
+        }
+        
         libraries = [
-            DocumentAutomation(self, lang, performance, *args, **kwargs)
+            DocumentAutomation(lang, performance, **kwargs)
         ]
         super().__init__(libraries)
```

## Comparing `edurpa_document-0.0.4.dist-info/LICENSE` & `edurpa_document-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `edurpa_document-0.0.4.dist-info/METADATA` & `edurpa_document-0.0.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edurpa-document
-Version: 0.0.4
+Version: 0.0.5
 Summary: education librabry for RPA
 Home-page: https://github.com/edu-rpa/edu-rpa-library
 Author: david
 Author-email: davidhuynh0222@gmail.com
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

