# Comparing `tmp/edurpa_document-0.0.5-py3-none-any.whl.zip` & `tmp/edurpa_document-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6072 bytes, number of entries: 9
+Zip file size: 6325 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-28 07:01 EduRPA/__init__.py
--rw-rw-rw-  2.0 fat     4923 b- defN 24-May-27 14:38 EduRPA/Document/DocumentAutomation.py
--rw-rw-rw-  2.0 fat      540 b- defN 24-May-27 14:39 EduRPA/Document/__init__.py
+-rw-rw-rw-  2.0 fat     5686 b- defN 24-May-27 16:00 EduRPA/Document/DocumentAutomation.py
+-rw-rw-rw-  2.0 fat      617 b- defN 24-May-27 15:57 EduRPA/Document/__init__.py
 -rw-rw-rw-  2.0 fat     2624 b- defN 24-Apr-28 06:18 EduRPA/Document/transform.py
--rw-rw-rw-  2.0 fat     1088 b- defN 24-May-27 14:39 edurpa_document-0.0.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2019 b- defN 24-May-27 14:39 edurpa_document-0.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-27 14:39 edurpa_document-0.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 24-May-27 14:39 edurpa_document-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      759 b- defN 24-May-27 14:39 edurpa_document-0.0.5.dist-info/RECORD
-9 files, 12052 bytes uncompressed, 4748 bytes compressed:  60.6%
+-rw-rw-rw-  2.0 fat     1088 b- defN 24-May-27 16:00 edurpa_document-0.0.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2019 b- defN 24-May-27 16:00 edurpa_document-0.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-27 16:00 edurpa_document-0.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 24-May-27 16:00 edurpa_document-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      759 b- defN 24-May-27 16:00 edurpa_document-0.0.6.dist-info/RECORD
+9 files, 12892 bytes uncompressed, 5001 bytes compressed:  61.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: EduRPA/Document/__init__.py
 Comment: 
 
 Filename: EduRPA/Document/transform.py
 Comment: 
 
-Filename: edurpa_document-0.0.5.dist-info/LICENSE
+Filename: edurpa_document-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: edurpa_document-0.0.5.dist-info/METADATA
+Filename: edurpa_document-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: edurpa_document-0.0.5.dist-info/WHEEL
+Filename: edurpa_document-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: edurpa_document-0.0.5.dist-info/top_level.txt
+Filename: edurpa_document-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: edurpa_document-0.0.5.dist-info/RECORD
+Filename: edurpa_document-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## EduRPA/Document/DocumentAutomation.py

```diff
@@ -3,20 +3,25 @@
 from PIL import Image
 from robot.api.deco import keyword, not_keyword
 import cv2
 import json
 from openpyxl import Workbook
 from datetime import datetime
 from .transform import perspective_transform, resize_image
+import string
+import unicodedata
+import editdistance
 class DocumentAutomation:
-    def __init__(self, lang, performance, **kwargs):
+    def __init__(self, lang, performance, tolerate, **kwargs):
         if kwargs["dryrun"]:
             # If running dryrun, ignore initialization
             return
         
+        self.tolerate = tolerate
+        
         cfg = Cfg.load_config_from_name("vgg_seq2seq")
         cfg["device"] = "cpu"
         vgg_seq2seq = Predictor(cfg)
 
         cfg = Cfg.load_config_from_name("vgg_transformer")
         cfg["device"] = "cpu"
         vgg_transformer = Predictor(cfg)
@@ -76,14 +81,28 @@
             y2 = int(template['dataTemplate'][key]['bottom'])
             extracted_labeled_images[key] = []
             extracted_labeled_images[key] = document[y1:y2, x1:x2]
 
         # extract data from images
         return self.extract(extracted_labeled_images)
     
+    @not_keyword
+    def evaluate_answer(self, answer, correct):
+        pd = unicodedata.normalize("NFKD", answer).encode("ASCII", "ignore").decode("ASCII")
+        gt = unicodedata.normalize("NFKD", correct).encode("ASCII", "ignore").decode("ASCII")
+        
+        pd = pd.translate(str.maketrans("", "", string.punctuation))
+        gt = gt.translate(str.maketrans("", "", string.punctuation))
+        
+        pd_cer, gt_cer = list(pd.lower()), list(gt.lower())
+        dist = editdistance.eval(pd_cer, gt_cer)
+        cer = dist / (max(len(pd_cer), len(gt_cer)))
+        
+        return cer < self.tolerate
+    
     # TODO: update this keyword
     @keyword("Create Grade Report File", types={'correct_answer': dict, 'actual_answers': list[dict], 'file_names': list})
     def create_grade_report_file(self, correct_answer, actual_answers, file_names):
         # Initialize report file
         workbook = Workbook()
         report_file_name = f'report_{datetime.now().strftime("%Y%m%d_%H%M%S")}.xlsx'
         summarizeSheet = workbook.create_sheet(title=f"Summary")
@@ -102,15 +121,15 @@
             # Write header
             header = ['Label', 'Actual answer', 'Correct answer', 'Score']
             sheet.append(header)
 
             # Write data rows
             total_score = 0
             for (label , correct_answer_label, actual_answer_label) in zip(correct_answer.keys(), correct_answer.values(), actual_answer.values()):
-                is_correct = correct_answer_label == actual_answer_label
+                is_correct = self.evaluate_answer(actual_answer_label, correct_answer_label)
                 row = [label, actual_answer_label, correct_answer_label, is_correct]
                 sheet.append(row)
                 
                 summary.append(actual_answer_label)
                 total_score += is_correct
 
             sheet.append(['','','Total',total_score])
```

## EduRPA/Document/__init__.py

```diff
@@ -4,16 +4,18 @@
 
 from robotlibcore import DynamicCore
 from robot.libraries.BuiltIn import BuiltIn
 class Document(DynamicCore):
     def __init__(
         self, lang, performance, **kwargs
     ):
+        self.tolerate = kwargs.get('tolerate', 0.4) 
+        
         # Register keyword libraries to LibCore
         kwargs = {
             "dryrun": BuiltIn().dry_run_active
         }
         
         libraries = [
-            DocumentAutomation(lang, performance, **kwargs)
+            DocumentAutomation(lang, performance,self.tolerate,**kwargs)
         ]
         super().__init__(libraries)
```

## Comparing `edurpa_document-0.0.5.dist-info/LICENSE` & `edurpa_document-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `edurpa_document-0.0.5.dist-info/METADATA` & `edurpa_document-0.0.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edurpa-document
-Version: 0.0.5
+Version: 0.0.6
 Summary: education librabry for RPA
 Home-page: https://github.com/edu-rpa/edu-rpa-library
 Author: david
 Author-email: davidhuynh0222@gmail.com
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

