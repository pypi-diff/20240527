# Comparing `tmp/danila-lib-1.7.6.tar.gz` & `tmp/danila-lib-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.7.6.tar", last modified: Thu May 23 05:47:00 2024, max compression
+gzip compressed data, was "danila-lib-1.7.7.tar", last modified: Mon May 27 07:27:39 2024, max compression
```

## Comparing `danila-lib-1.7.6.tar` & `danila-lib-1.7.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 05:47:00.908108 danila-lib-1.7.6/
--rw-rw-rw-   0        0        0     9615 2024-05-23 05:47:00.908108 danila-lib-1.7.6/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.7.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 05:47:00.798762 danila-lib-1.7.6/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.7.6/danila/__init__.py
--rw-rw-rw-   0        0        0     2123 2024-05-22 05:28:12.000000 danila-lib-1.7.6/danila/danila.py
--rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.7.6/danila/danila_v1.py
--rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.7.6/danila/danila_v2.py
--rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.7.6/danila/danila_v3.py
--rw-rw-rw-   0        0        0    15682 2024-05-22 11:32:57.000000 danila-lib-1.7.6/danila/danila_v4.py
-drwxrwxrwx   0        0        0        0 2024-05-23 05:47:00.814383 danila-lib-1.7.6/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     9615 2024-05-23 05:47:00.000000 danila-lib-1.7.6/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      940 2024-05-23 05:47:00.000000 danila-lib-1.7.6/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 05:47:00.000000 danila-lib-1.7.6/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1879 2024-05-23 05:47:00.000000 danila-lib-1.7.6/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-23 05:47:00.000000 danila-lib-1.7.6/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 05:47:00.814383 danila-lib-1.7.6/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.7.6/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 05:47:00.861246 danila-lib-1.7.6/data/neuro/
--rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.7.6/data/neuro/Letters_recognize.py
--rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.7.6/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.7.6/data/neuro/Rama_detect_class.py
--rw-rw-rw-   0        0        0     2614 2024-05-14 12:37:43.000000 danila-lib-1.7.6/data/neuro/Rama_prod_classify_class.py
--rw-rw-rw-   0        0        0     3153 2024-05-23 05:46:54.000000 danila-lib-1.7.6/data/neuro/Text_detect_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.7.6/data/neuro/__init__.py
--rw-rw-rw-   0        0        0     6373 2024-05-06 15:05:03.000000 danila-lib-1.7.6/data/neuro/letters_in_image.py
--rw-rw-rw-   0        0        0      654 2024-05-22 10:13:34.000000 danila-lib-1.7.6/data/neuro/models.py
--rw-rw-rw-   0        0        0     2975 2024-05-14 11:04:15.000000 danila-lib-1.7.6/data/neuro/objs_in_image.py
--rw-rw-rw-   0        0        0     4390 2024-05-22 07:22:08.000000 danila-lib-1.7.6/data/neuro/text_recognize_yolo.py
-drwxrwxrwx   0        0        0        0 2024-05-23 05:47:00.908108 danila-lib-1.7.6/data/result/
--rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.7.6/data/result/Class_im.py
--rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.7.6/data/result/Class_text.py
--rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.7.6/data/result/Image_text_areas.py
--rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.7.6/data/result/Label_area.py
--rw-rw-rw-   0        0        0      105 2024-05-14 11:34:55.000000 danila-lib-1.7.6/data/result/Rama_prod.py
--rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.7.6/data/result/Rect.py
--rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.7.6/data/result/Text_area.py
--rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.7.6/data/result/Yolo_label_rect.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.7.6/data/result/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.7.6/data/result/prod_classify_result.py
--rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.7.6/data/result/word_compare_result.py
--rw-rw-rw-   0        0        0       42 2024-05-23 05:47:00.908108 danila-lib-1.7.6/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-05-23 05:46:54.000000 danila-lib-1.7.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 07:27:39.618196 danila-lib-1.7.7/
+-rw-rw-rw-   0        0        0     9615 2024-05-27 07:27:39.618196 danila-lib-1.7.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.7.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 07:27:39.394200 danila-lib-1.7.7/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.7.7/danila/__init__.py
+-rw-rw-rw-   0        0        0     2123 2024-05-22 05:28:12.000000 danila-lib-1.7.7/danila/danila.py
+-rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.7.7/danila/danila_v1.py
+-rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.7.7/danila/danila_v2.py
+-rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.7.7/danila/danila_v3.py
+-rw-rw-rw-   0        0        0    17794 2024-05-27 07:27:16.000000 danila-lib-1.7.7/danila/danila_v4.py
+drwxrwxrwx   0        0        0        0 2024-05-27 07:27:39.424065 danila-lib-1.7.7/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     9615 2024-05-27 07:27:39.000000 danila-lib-1.7.7/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      940 2024-05-27 07:27:39.000000 danila-lib-1.7.7/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 07:27:39.000000 danila-lib-1.7.7/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1879 2024-05-27 07:27:39.000000 danila-lib-1.7.7/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-27 07:27:39.000000 danila-lib-1.7.7/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 07:27:39.425061 danila-lib-1.7.7/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.7.7/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 07:27:39.513664 danila-lib-1.7.7/data/neuro/
+-rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.7.7/data/neuro/Letters_recognize.py
+-rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.7.7/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.7.7/data/neuro/Rama_detect_class.py
+-rw-rw-rw-   0        0        0     2802 2024-05-27 07:12:44.000000 danila-lib-1.7.7/data/neuro/Rama_prod_classify_class.py
+-rw-rw-rw-   0        0        0     3153 2024-05-23 05:46:54.000000 danila-lib-1.7.7/data/neuro/Text_detect_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.7.7/data/neuro/__init__.py
+-rw-rw-rw-   0        0        0     6373 2024-05-06 15:05:03.000000 danila-lib-1.7.7/data/neuro/letters_in_image.py
+-rw-rw-rw-   0        0        0      654 2024-05-22 10:13:34.000000 danila-lib-1.7.7/data/neuro/models.py
+-rw-rw-rw-   0        0        0     2975 2024-05-14 11:04:15.000000 danila-lib-1.7.7/data/neuro/objs_in_image.py
+-rw-rw-rw-   0        0        0     4603 2024-05-27 07:27:16.000000 danila-lib-1.7.7/data/neuro/text_recognize_yolo.py
+drwxrwxrwx   0        0        0        0 2024-05-27 07:27:39.616204 danila-lib-1.7.7/data/result/
+-rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.7.7/data/result/Class_im.py
+-rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.7.7/data/result/Class_text.py
+-rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.7.7/data/result/Image_text_areas.py
+-rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.7.7/data/result/Label_area.py
+-rw-rw-rw-   0        0        0      105 2024-05-14 11:34:55.000000 danila-lib-1.7.7/data/result/Rama_prod.py
+-rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.7.7/data/result/Rect.py
+-rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.7.7/data/result/Text_area.py
+-rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.7.7/data/result/Yolo_label_rect.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.7.7/data/result/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.7.7/data/result/prod_classify_result.py
+-rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.7.7/data/result/word_compare_result.py
+-rw-rw-rw-   0        0        0       42 2024-05-27 07:27:39.625164 danila-lib-1.7.7/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-05-27 07:27:35.000000 danila-lib-1.7.7/setup.py
```

### Comparing `danila-lib-1.7.6/PKG-INFO` & `danila-lib-1.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.7.6
+Version: 1.7.7
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.7.6/README.md` & `danila-lib-1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.6/danila/danila.py` & `danila-lib-1.7.7/danila/danila.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.6/danila/danila_v1.py` & `danila-lib-1.7.7/danila/danila_v1.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.6/danila/danila_v2.py` & `danila-lib-1.7.7/danila/danila_v2.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.6/danila/danila_v3.py` & `danila-lib-1.7.7/danila/danila_v3.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.6/danila/danila_v4.py` & `danila-lib-1.7.7/danila/danila_v4.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import hashlib
 import os
+from datetime import datetime
 
 import cv2
 
 from data.neuro.Letters_recognize import Letters_recognize
 from data.neuro.Rama_detect_class import Rama_detect_class
 from data.neuro.Rama_prod_classify_class import Rama_prod_classify_class
 from data.neuro.Text_detect_class import Text_detect_class
@@ -48,136 +50,168 @@
         # img = cv2.imread(img_path)
         rama_prod = self.rama_prod_classify_model.classify(img, size)
         return rama_prod.name
 
     # returns openCV frame with rama from openCV frame\
     def rama_detect(self, img, size = 256):
         """rama_detect(img : openCV img) -> openCV image with drawn rama rectangle"""
-        initial_image_path = 'initial_image.jpg'
+        hash_object = hashlib.md5(str(datetime.now()))
+        hash_str = hash_object.hexdigest()
+        initial_image_path = 'initial_image' + hash_str + '.jpg'
         cv2.imwrite(initial_image_path, img)
         rama_prod = self.rama_prod_classify_model.classify(img, size)
         if rama_prod == Rama_Prod.no_rama:
+            os.remove(initial_image_path)
             return img
         rect = Rect()
         if (rama_prod == Rama_Prod.ruzhimmash):
             rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
         else:
             rect = self.rama_no_spring_detect_model.rama_detect(initial_image_path)
         new_img = img.copy()
-        os.remove('initial_image.jpg')
+        os.remove(initial_image_path)
         if rect is None:
+            os.remove(initial_image_path)
             return img
         cv2.rectangle(new_img, (rect.xmin, rect.ymin), (rect.xmax, rect.ymax), (0, 0, 255), 2)
         cv2.putText(new_img, rama_prod.name, (rect.xmin, rect.ymin), cv2.FONT_HERSHEY_SIMPLEX, 0.5, (0,0,255), 2)
         return new_img
 
     # returns openCV image with cut_rama
     def rama_cut(self, img, size = 256):
         """rama_cut(img : openCV img) -> openCV image of rama rectangle"""
-        initial_image_path = 'initial_image.jpg'
-        cv2.imwrite(initial_image_path, img, size)
-        rama_prod = self.rama_prod_classify_model.classify(img)
+        hash_object = hashlib.md5(str(datetime.now()))
+        hash_str = hash_object.hexdigest()
+        initial_image_path = 'initial_image' + hash_str + '.jpg'
+        cv2.imwrite(initial_image_path, img)
+        rama_prod = self.rama_prod_classify_model.classify(img, size)
         if rama_prod == Rama_Prod.no_rama:
+            os.remove(initial_image_path)
             return img
         rect = Rect()
         if (rama_prod == Rama_Prod.ruzhimmash):
             rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
         else:
             rect = self.rama_no_spring_detect_model.rama_detect(initial_image_path)
         if rect is None:
+            os.remove(initial_image_path)
             return img
         img_res = img[rect.ymin:rect.ymax, rect.xmin:rect.xmax]
-        os.remove('initial_image.jpg')
+        os.remove(initial_image_path)
         return img_res
     #
     # returns openCV cut rama with drawn text areas
     def text_detect_cut(self, img, size = 256):
         """returns openCV cut rama with drawn text areas"""
-        initial_image_path = 'initial_image.jpg'
+        hash_object = hashlib.md5(str(datetime.now()))
+        hash_str = hash_object.hexdigest()
+        initial_image_path = 'initial_image' + hash_str + '.jpg'
         cv2.imwrite(initial_image_path, img)
         rama_prod = self.rama_prod_classify_model.classify(img, size)
         if rama_prod == Rama_Prod.no_rama:
+            os.remove(initial_image_path)
             return {'result': 'no_rama'}
         rect = Rect()
         if (rama_prod == Rama_Prod.ruzhimmash):
             rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
             if rect is None:
+                os.remove(initial_image_path)
                 return img
             img_cut = img[rect.ymin:rect.ymax, rect.xmin:rect.xmax]
-            img_cut_path = 'cut_img.jpg'
+            hash_object = hashlib.md5(str(datetime.now()))
+            hash_str = hash_object.hexdigest()
+            img_cut_path = 'cut_img' + hash_str + '.jpg'
             cv2.imwrite(img_cut_path, img_cut)
             image_text_areas = self.rama_spring_ruzhimmash_text_detect_model.text_detect(img_cut_path)
             image_drawn_text_areas = self.rama_spring_ruzhimmash_text_detect_model.draw_text_areas_in_opencv(image_text_areas, img_cut)
             os.remove(initial_image_path)
             os.remove(img_cut_path)
             return image_drawn_text_areas
         else:
             rect = self.rama_no_spring_detect_model.rama_detect(initial_image_path)
             if rect is None:
+                os.remove(initial_image_path)
                 return img
             img_cut = img[rect.ymin:rect.ymax, rect.xmin:rect.xmax]
-            img_cut_path = 'cut_img.jpg'
+            hash_object = hashlib.md5(str(datetime.now()))
+            hash_str = hash_object.hexdigest()
+            img_cut_path = 'cut_img' + hash_str + '.jpg'
             cv2.imwrite(img_cut_path, img_cut)
             image_text_areas = self.rama_no_spring_bejickaya_text_detect_model.text_detect(img_cut_path)
             image_drawn_text_areas = self.rama_no_spring_bejickaya_text_detect_model.draw_text_areas_in_opencv(image_text_areas, img_cut)
             os.remove(initial_image_path)
             os.remove(img_cut_path)
             return image_drawn_text_areas
 
     # returns openCV img with drawn text areas
     def text_detect(self, img, size = 256):
         """returns openCV img with drawn text areas"""
-        initial_image_path = 'initial_image.jpg'
+        hash_object = hashlib.md5(str(datetime.now()))
+        hash_str = hash_object.hexdigest()
+        initial_image_path = 'initial_image' + hash_str + '.jpg'
         cv2.imwrite(initial_image_path, img)
         rama_prod = self.rama_prod_classify_model.classify(img, size)
         if rama_prod == Rama_Prod.no_rama:
+            os.remove(initial_image_path)
             return img
         rect = Rect()
         if (rama_prod == Rama_Prod.ruzhimmash):
             rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
             if rect is None:
+                os.remove(initial_image_path)
                 return img
             img_cut = img[rect.ymin:rect.ymax, rect.xmin:rect.xmax]
-            img_cut_path = 'cut_img.jpg'
+            hash_object = hashlib.md5(str(datetime.now()))
+            hash_str = hash_object.hexdigest()
+            img_cut_path = 'cut_img' + hash_str + '.jpg'
             cv2.imwrite(img_cut_path, img_cut)
             image_text_areas = self.rama_spring_ruzhimmash_text_detect_model.text_detect(img_cut_path)
             image_text_areas.explore_to_whole_image(rect)
             image_drawn_text_areas = self.rama_spring_ruzhimmash_text_detect_model.draw_text_areas_in_opencv(image_text_areas, img)
             os.remove(initial_image_path)
             os.remove(img_cut_path)
             return image_drawn_text_areas
         else:
             rect = self.rama_no_spring_detect_model.rama_detect(initial_image_path)
             if rect is None:
+                os.remove(initial_image_path)
                 return img
             img_cut = img[rect.ymin:rect.ymax, rect.xmin:rect.xmax]
-            img_cut_path = 'cut_img.jpg'
+            hash_object = hashlib.md5(str(datetime.now()))
+            hash_str = hash_object.hexdigest()
+            img_cut_path = 'cut_img' + hash_str + '.jpg'
             cv2.imwrite(img_cut_path, img_cut)
             image_text_areas = self.rama_no_spring_bejickaya_text_detect_model.text_detect(img_cut_path)
             image_text_areas.explore_to_whole_image(rect)
             image_drawn_text_areas = self.rama_no_spring_bejickaya_text_detect_model.draw_text_areas_in_opencv(image_text_areas, img)
             os.remove(initial_image_path)
             os.remove(img_cut_path)
             return image_drawn_text_areas
 
     # returns dict {'number', 'prod', 'year'} for openCV rama img or 'no_rama'
     def text_recognize(self, img, size = 256):
         """returns dict {'number', 'prod', 'year'} for openCV rama img or 'no_rama'"""
-        initial_image_path = 'initial_image.jpg'
+        hash_object = hashlib.md5(str(datetime.now()))
+        hash_str = hash_object.hexdigest()
+        initial_image_path = 'initial_image' + hash_str + '.jpg'
         cv2.imwrite(initial_image_path, img)
         rama_prod = self.rama_prod_classify_model.classify(img, size)
         if rama_prod == Rama_Prod.no_rama:
+            os.remove(initial_image_path)
             return {'result': 'no_rama'}
         rect = Rect()
         if (rama_prod == Rama_Prod.ruzhimmash):
             rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
             if rect is None:
+                os.remove(initial_image_path)
                 return {'result': 'no_rama'}
             img_cut = img[rect.ymin:rect.ymax, rect.xmin:rect.xmax]
-            img_cut_path = 'cut_img.jpg'
+            hash_object = hashlib.md5(str(datetime.now()))
+            hash_str = hash_object.hexdigest()
+            img_cut_path = 'cut_img' + hash_str + '.jpg'
             cv2.imwrite(img_cut_path, img_cut)
             image_text_areas = self.rama_spring_ruzhimmash_text_detect_model.text_detect(img_cut_path)
 
             label_area = self.text_recognize_ruzhimmash_model.work_image_cut(image_text_areas, img_cut, 5, 64,128,
                                                                   4, 64,128, 2, 64,64)
             res_labels = {}
             if len(label_area.labels[Class_text.number]) == 5:
@@ -211,21 +245,26 @@
                     else:
                         res_labels['number'] = label_area.labels[Class_text.number]
             res_labels['prod'] = '1275'
             if (len(label_area.labels[Class_text.year]) == 2) and (int(label_area.labels[Class_text.year]) < 25):
                 res_labels['year'] = label_area.labels[Class_text.year]
             else:
                 res_labels['year'] = '23'
+            os.remove(initial_image_path)
+            os.remove(img_cut_path)
             return res_labels
         else:
             rect = self.rama_no_spring_detect_model.rama_detect(initial_image_path)
             if rect is None:
+                os.remove(initial_image_path)
                 return {"result" : "no_rama"}
             img_cut = img[rect.ymin:rect.ymax, rect.xmin:rect.xmax]
-            img_cut_path = 'cut_img.jpg'
+            hash_object = hashlib.md5(str(datetime.now()))
+            hash_str = hash_object.hexdigest()
+            img_cut_path = 'cut_img' + hash_str + '.jpg'
             cv2.imwrite(img_cut_path, img_cut)
             image_text_areas = self.rama_no_spring_bejickaya_text_detect_model.text_detect(img_cut_path)
             label_area = self.text_recognize_begickaya_model.work_image_cut(image_text_areas, img_cut, 6, 64, 192,
                                                                   2, 64, 64, 2, 64,64)
             res_labels = {}
             if len(label_area.labels[Class_text.number]) == 6:
                 res_labels['number'] = label_area.labels[Class_text.number]
@@ -258,8 +297,10 @@
                     else:
                         res_labels['number'] = label_area.labels[Class_text.number]
             res_labels['prod'] = '12'
             if (len(label_area.labels[Class_text.year]) == 2) and (int(label_area.labels[Class_text.year]) < 25):
                 res_labels['year'] = label_area.labels[Class_text.year]
             else:
                 res_labels['year'] = '23'
+            os.remove(initial_image_path)
+            os.remove(img_cut_path)
             return res_labels
```

### Comparing `danila-lib-1.7.6/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.7.7/danila_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.7.6
+Version: 1.7.7
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.7.6/danila_lib.egg-info/SOURCES.txt` & `danila-lib-1.7.7/danila_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.6/danila_lib.egg-info/requires.txt` & `danila-lib-1.7.7/danila_lib.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.6/data/neuro/Letters_recognize.py` & `danila-lib-1.7.7/data/neuro/Letters_recognize.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.6/data/neuro/Rama_classify_class.py` & `danila-lib-1.7.7/data/neuro/Rama_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.6/data/neuro/Rama_detect_class.py` & `danila-lib-1.7.7/data/neuro/Rama_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.6/data/neuro/Rama_prod_classify_class.py` & `danila-lib-1.7.7/data/neuro/Rama_prod_classify_class.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import os
 import zipfile
 
 import cv2
 import requests
 from urllib.parse import urlencode
 import torch
-
+import hashlib
+from datetime import datetime
 from data.neuro.letters_in_image import Letters_In_Image
 from data.neuro.objs_in_image import Objs_In_Image
 from data.result.Class_text import Class_text
 from data.result.Label_area import Label_area
 from data.result.Rama_prod import Rama_Prod
 
 
@@ -36,21 +37,24 @@
         # weights_file_path = model_name + '_weights.pt'
         self.model = torch.hub.load(yolo_path, 'custom', 'prod_classify.pt', source='local')
 
         # for every text_class try to recognize text from all areas of text_class, length is depends on class and prod, returns string
 
 
     def work_image(self, img, size):
-        cv2.imwrite('img.jpg', img)
-        results = self.model(['img.jpg'], size = size)
+        hash_object = hashlib.md5(str(datetime.now()))
+        hash_str = hash_object.hexdigest()
+        img_name = 'img' + hash_str + '.jpg'
+        cv2.imwrite(img_name, img)
+        results = self.model([img_name], size = size)
         json_res = results.pandas().xyxy[0].to_json(orient="records")
         res2 = json.loads(json_res)
         img_objs = Objs_In_Image.get_objs_in_image_from_yolo_json(res2)
         img_objs.delete_intersections()
-        os.remove('img.jpg')
+        os.remove(img_name)
         return img_objs
 
     def classify(self, img, size):
         image_objs = self.work_image(img, size)
         b_list_r = any(obj.obj == 'bejickaya' for obj in image_objs.objs)
         r_list_r = any(obj.obj == 'ruzhimmash' for obj in image_objs.objs)
         if (b_list_r == False) and (r_list_r == False):
```

### Comparing `danila-lib-1.7.6/data/neuro/Text_detect_class.py` & `danila-lib-1.7.7/data/neuro/Text_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.6/data/neuro/letters_in_image.py` & `danila-lib-1.7.7/data/neuro/letters_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.6/data/neuro/models.py` & `danila-lib-1.7.7/data/neuro/models.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.6/data/neuro/objs_in_image.py` & `danila-lib-1.7.7/data/neuro/objs_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.6/data/neuro/text_recognize_yolo.py` & `danila-lib-1.7.7/data/neuro/text_recognize_yolo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import hashlib
 import json
 import os
 import zipfile
+from datetime import datetime
 
 import cv2
 import requests
 from urllib.parse import urlencode
 import torch
 
 from data.neuro.letters_in_image import Letters_In_Image
@@ -65,23 +67,26 @@
         label_area.labels[Class_text.number] = number
         label_area.labels[Class_text.prod] = prod
         label_area.labels[Class_text.year] = year
         return label_area
 
     def work_img_word(self, number_image_cut, l, number_h, number_w):
         h, w = number_image_cut.shape[:2]
-        cv2.imwrite('img.jpg', number_image_cut)
+        hash_object = hashlib.md5(str(datetime.now()))
+        hash_str = hash_object.hexdigest()
+        img_cut_path = 'cut_text_img' + hash_str + '.jpg'
+        cv2.imwrite(img_cut_path, number_image_cut)
         self.model.max_det = l
-        results = self.model(['img.jpg'], size=(number_h, number_w))
+        results = self.model(img_cut_path, size=(number_h, number_w))
         json_res = results.pandas().xyxy[0].to_json(orient="records")
         res2 = json.loads(json_res)
         img_letters = Letters_In_Image.get_letters_in_image_from_yolo_json(res2)
         img_letters.sort_letters()
         img_letters.delete_intersections()
-        os.remove('img.jpg')
+        os.remove(img_cut_path)
         return img_letters.make_word()
 
 
 
     # cut text_areas imgs for each Rect from rect_array returns openCv imgs list
     def make_cuts(self, img_rama_cut, rect_array):
         """cut text_areas imgs for each Rect from rect_array returns openCv imgs list"""
```

### Comparing `danila-lib-1.7.6/data/result/Image_text_areas.py` & `danila-lib-1.7.7/data/result/Image_text_areas.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.6/data/result/Rect.py` & `danila-lib-1.7.7/data/result/Rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.6/data/result/Text_area.py` & `danila-lib-1.7.7/data/result/Text_area.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.6/data/result/Yolo_label_rect.py` & `danila-lib-1.7.7/data/result/Yolo_label_rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.6/setup.py` & `danila-lib-1.7.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.7.6',
+  version='1.7.7',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```

