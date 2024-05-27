# Comparing `tmp/freerec-0.8.1.tar.gz` & `tmp/freerec-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freerec-0.8.1.tar", last modified: Tue Apr 23 11:27:49 2024, max compression
+gzip compressed data, was "freerec-0.8.3.tar", last modified: Mon May 27 13:13:59 2024, max compression
```

## Comparing `freerec-0.8.1.tar` & `freerec-0.8.3.tar`

### file list

```diff
@@ -1,53 +1,56 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 11:27:49.096286 freerec-0.8.1/
--rw-rw-rw-   0        0        0     1085 2022-09-12 08:50:27.000000 freerec-0.8.1/LICENSE
--rw-rw-rw-   0        0        0     2348 2024-04-23 11:27:49.095037 freerec-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     1782 2024-04-22 01:25:03.000000 freerec-0.8.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 11:27:49.050667 freerec-0.8.1/freerec/
--rw-rw-rw-   0        0        0      554 2024-04-23 07:10:43.000000 freerec-0.8.1/freerec/__init__.py
--rw-rw-rw-   0        0        0     4116 2024-04-14 08:06:45.000000 freerec-0.8.1/freerec/__main__.py
--rw-rw-rw-   0        0        0     6270 2024-04-17 09:20:21.000000 freerec-0.8.1/freerec/criterions.py
-drwxrwxrwx   0        0        0        0 2024-04-23 11:27:49.079465 freerec-0.8.1/freerec/data/
--rw-rw-rw-   0        0        0       78 2024-04-22 08:24:53.000000 freerec-0.8.1/freerec/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 11:27:49.084968 freerec-0.8.1/freerec/data/datasets/
--rw-rw-rw-   0        0        0     2297 2024-04-21 05:44:43.000000 freerec-0.8.1/freerec/data/datasets/__init__.py
--rw-rw-rw-   0        0        0      848 2024-04-21 03:05:02.000000 freerec-0.8.1/freerec/data/datasets/allrecipes.py
--rw-rw-rw-   0        0        0    18450 2024-04-21 05:33:17.000000 freerec-0.8.1/freerec/data/datasets/amazon2014.py
--rw-rw-rw-   0        0        0     6405 2024-04-21 06:09:58.000000 freerec-0.8.1/freerec/data/datasets/amazon2018.py
--rw-rw-rw-   0        0        0    25273 2024-04-23 02:45:52.000000 freerec-0.8.1/freerec/data/datasets/base.py
--rw-rw-rw-   0        0        0     1436 2024-04-21 02:32:56.000000 freerec-0.8.1/freerec/data/datasets/gowalla.py
--rw-rw-rw-   0        0        0    11008 2024-04-21 02:34:07.000000 freerec-0.8.1/freerec/data/datasets/movielens.py
--rw-rw-rw-   0        0        0      831 2024-04-21 03:02:57.000000 freerec-0.8.1/freerec/data/datasets/tiktok.py
--rw-rw-rw-   0        0        0     6649 2024-04-21 02:37:51.000000 freerec-0.8.1/freerec/data/datasets/yelp.py
--rw-rw-rw-   0        0        0    13268 2024-04-17 06:58:28.000000 freerec-0.8.1/freerec/data/fields.py
-drwxrwxrwx   0        0        0        0 2024-04-23 11:27:49.090975 freerec-0.8.1/freerec/data/postprocessing/
--rw-rw-rw-   0        0        0      956 2024-04-16 11:37:36.000000 freerec-0.8.1/freerec/data/postprocessing/__init__.py
--rw-rw-rw-   0        0        0     2919 2024-04-23 03:23:48.000000 freerec-0.8.1/freerec/data/postprocessing/base.py
--rw-rw-rw-   0        0        0    24772 2024-04-23 03:09:55.000000 freerec-0.8.1/freerec/data/postprocessing/base.pyi
--rw-rw-rw-   0        0        0     1825 2024-04-23 07:56:44.000000 freerec-0.8.1/freerec/data/postprocessing/column.py
--rw-rw-rw-   0        0        0     9732 2024-04-22 05:44:09.000000 freerec-0.8.1/freerec/data/postprocessing/row.py
--rw-rw-rw-   0        0        0    19109 2024-04-23 07:48:46.000000 freerec-0.8.1/freerec/data/postprocessing/sampler.py
--rw-rw-rw-   0        0        0     2807 2024-04-23 03:21:07.000000 freerec-0.8.1/freerec/data/postprocessing/source.py
-drwxrwxrwx   0        0        0        0 2024-04-23 11:27:49.091975 freerec-0.8.1/freerec/data/preprocessing/
--rw-rw-rw-   0        0        0       37 2024-04-14 08:01:15.000000 freerec-0.8.1/freerec/data/preprocessing/__init__.py
--rw-rw-rw-   0        0        0    28235 2024-04-20 06:56:44.000000 freerec-0.8.1/freerec/data/preprocessing/base.py
--rw-rw-rw-   0        0        0      789 2024-04-20 07:59:27.000000 freerec-0.8.1/freerec/data/tags.py
--rw-rw-rw-   0        0        0     9778 2024-04-22 07:01:44.000000 freerec-0.8.1/freerec/data/utils.py
--rw-rw-rw-   0        0        0     9147 2023-12-25 08:54:45.000000 freerec-0.8.1/freerec/ddp.py
--rw-rw-rw-   0        0        0     3101 2023-02-24 08:54:11.000000 freerec-0.8.1/freerec/dict2obj.py
--rw-rw-rw-   0        0        0     4806 2024-04-14 12:22:40.000000 freerec-0.8.1/freerec/graph.py
--rw-rw-rw-   0        0        0    34594 2024-04-23 07:34:48.000000 freerec-0.8.1/freerec/launcher.py
--rw-rw-rw-   0        0        0    23293 2023-04-30 11:44:17.000000 freerec-0.8.1/freerec/metrics.py
-drwxrwxrwx   0        0        0        0 2024-04-23 11:27:49.094532 freerec-0.8.1/freerec/models/
--rw-rw-rw-   0        0        0       66 2024-04-23 06:25:12.000000 freerec-0.8.1/freerec/models/__init__.py
--rw-rw-rw-   0        0        0     6997 2024-04-23 06:37:08.000000 freerec-0.8.1/freerec/models/base.py
--rw-rw-rw-   0        0        0    16893 2024-04-22 08:21:05.000000 freerec-0.8.1/freerec/parser.py
--rw-rw-rw-   0        0        0    16048 2024-04-17 03:34:43.000000 freerec-0.8.1/freerec/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 11:27:49.076458 freerec-0.8.1/freerec.egg-info/
--rw-rw-rw-   0        0        0     2348 2024-04-23 11:27:48.000000 freerec-0.8.1/freerec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1182 2024-04-23 11:27:48.000000 freerec-0.8.1/freerec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 11:27:48.000000 freerec-0.8.1/freerec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-23 11:27:48.000000 freerec-0.8.1/freerec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2024-04-23 11:27:48.000000 freerec-0.8.1/freerec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-23 11:27:48.000000 freerec-0.8.1/freerec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 11:27:49.097048 freerec-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0     1234 2024-04-23 06:22:49.000000 freerec-0.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:13:59.187868 freerec-0.8.3/
+-rw-rw-rw-   0        0        0     1085 2022-09-12 08:50:27.000000 freerec-0.8.3/LICENSE
+-rw-rw-rw-   0        0        0     2348 2024-05-27 13:13:59.186869 freerec-0.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1782 2024-04-22 01:25:03.000000 freerec-0.8.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 13:13:59.032143 freerec-0.8.3/freerec/
+-rw-rw-rw-   0        0        0      554 2024-05-27 13:12:45.000000 freerec-0.8.3/freerec/__init__.py
+-rw-rw-rw-   0        0        0     4124 2024-05-05 06:15:25.000000 freerec-0.8.3/freerec/__main__.py
+-rw-rw-rw-   0        0        0     6270 2024-04-17 09:20:21.000000 freerec-0.8.3/freerec/criterions.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:13:59.141285 freerec-0.8.3/freerec/data/
+-rw-rw-rw-   0        0        0       78 2024-04-22 08:24:53.000000 freerec-0.8.3/freerec/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:13:59.151372 freerec-0.8.3/freerec/data/datasets/
+-rw-rw-rw-   0        0        0     2647 2024-05-27 12:15:15.000000 freerec-0.8.3/freerec/data/datasets/__init__.py
+-rw-rw-rw-   0        0        0      848 2024-04-21 03:05:02.000000 freerec-0.8.3/freerec/data/datasets/allrecipes.py
+-rw-rw-rw-   0        0        0    18450 2024-04-21 05:33:17.000000 freerec-0.8.3/freerec/data/datasets/amazon2014.py
+-rw-rw-rw-   0        0        0     6405 2024-04-21 06:09:58.000000 freerec-0.8.3/freerec/data/datasets/amazon2018.py
+-rw-rw-rw-   0        0        0     6481 2024-05-27 11:30:00.000000 freerec-0.8.3/freerec/data/datasets/amazon2023.py
+-rw-rw-rw-   0        0        0    25283 2024-04-25 12:06:52.000000 freerec-0.8.3/freerec/data/datasets/base.py
+-rw-rw-rw-   0        0        0     1436 2024-04-21 02:32:56.000000 freerec-0.8.3/freerec/data/datasets/gowalla.py
+-rw-rw-rw-   0        0        0      819 2024-05-27 12:20:36.000000 freerec-0.8.3/freerec/data/datasets/microlens.py
+-rw-rw-rw-   0        0        0    12256 2024-04-24 05:48:14.000000 freerec-0.8.3/freerec/data/datasets/movielens.py
+-rw-rw-rw-   0        0        0      831 2024-04-21 03:02:57.000000 freerec-0.8.3/freerec/data/datasets/tiktok.py
+-rw-rw-rw-   0        0        0     6649 2024-04-21 02:37:51.000000 freerec-0.8.3/freerec/data/datasets/yelp.py
+-rw-rw-rw-   0        0        0    12990 2024-05-10 06:45:32.000000 freerec-0.8.3/freerec/data/fields.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:13:59.177823 freerec-0.8.3/freerec/data/postprocessing/
+-rw-rw-rw-   0        0        0      956 2024-04-16 11:37:36.000000 freerec-0.8.3/freerec/data/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2919 2024-04-23 03:23:48.000000 freerec-0.8.3/freerec/data/postprocessing/base.py
+-rw-rw-rw-   0        0        0    24772 2024-04-23 03:09:55.000000 freerec-0.8.3/freerec/data/postprocessing/base.pyi
+-rw-rw-rw-   0        0        0     1825 2024-04-23 07:56:44.000000 freerec-0.8.3/freerec/data/postprocessing/column.py
+-rw-rw-rw-   0        0        0     9818 2024-05-06 01:08:59.000000 freerec-0.8.3/freerec/data/postprocessing/row.py
+-rw-rw-rw-   0        0        0    19116 2024-05-10 06:34:02.000000 freerec-0.8.3/freerec/data/postprocessing/sampler.py
+-rw-rw-rw-   0        0        0     2807 2024-04-23 03:21:07.000000 freerec-0.8.3/freerec/data/postprocessing/source.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:13:59.182860 freerec-0.8.3/freerec/data/preprocessing/
+-rw-rw-rw-   0        0        0       88 2024-05-24 09:17:43.000000 freerec-0.8.3/freerec/data/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     4491 2024-05-26 05:54:26.000000 freerec-0.8.3/freerec/data/preprocessing/amazon2023.py
+-rw-rw-rw-   0        0        0    28251 2024-05-05 06:07:17.000000 freerec-0.8.3/freerec/data/preprocessing/base.py
+-rw-rw-rw-   0        0        0      789 2024-04-20 07:59:27.000000 freerec-0.8.3/freerec/data/tags.py
+-rw-rw-rw-   0        0        0     9778 2024-05-24 09:00:14.000000 freerec-0.8.3/freerec/data/utils.py
+-rw-rw-rw-   0        0        0     9147 2023-12-25 08:54:45.000000 freerec-0.8.3/freerec/ddp.py
+-rw-rw-rw-   0        0        0     3101 2023-02-24 08:54:11.000000 freerec-0.8.3/freerec/dict2obj.py
+-rw-rw-rw-   0        0        0     4806 2024-04-14 12:22:40.000000 freerec-0.8.3/freerec/graph.py
+-rw-rw-rw-   0        0        0    34594 2024-04-23 07:34:48.000000 freerec-0.8.3/freerec/launcher.py
+-rw-rw-rw-   0        0        0    23293 2023-04-30 11:44:17.000000 freerec-0.8.3/freerec/metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:13:59.185870 freerec-0.8.3/freerec/models/
+-rw-rw-rw-   0        0        0       66 2024-04-23 06:25:12.000000 freerec-0.8.3/freerec/models/__init__.py
+-rw-rw-rw-   0        0        0     6997 2024-04-23 06:37:08.000000 freerec-0.8.3/freerec/models/base.py
+-rw-rw-rw-   0        0        0    16893 2024-04-22 08:21:05.000000 freerec-0.8.3/freerec/parser.py
+-rw-rw-rw-   0        0        0    16048 2024-04-17 03:34:43.000000 freerec-0.8.3/freerec/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:13:59.126952 freerec-0.8.3/freerec.egg-info/
+-rw-rw-rw-   0        0        0     2348 2024-05-27 13:13:58.000000 freerec-0.8.3/freerec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1294 2024-05-27 13:13:58.000000 freerec-0.8.3/freerec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 13:13:58.000000 freerec-0.8.3/freerec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-27 13:13:58.000000 freerec-0.8.3/freerec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2024-05-27 13:13:58.000000 freerec-0.8.3/freerec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-27 13:13:58.000000 freerec-0.8.3/freerec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 13:13:59.187868 freerec-0.8.3/setup.cfg
+-rw-rw-rw-   0        0        0     1234 2024-04-23 06:22:49.000000 freerec-0.8.3/setup.py
```

### Comparing `freerec-0.8.1/LICENSE` & `freerec-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `freerec-0.8.1/PKG-INFO` & `freerec-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freerec
-Version: 0.8.1
+Version: 0.8.3
 Summary: PyTorch library for recommender systems
 Home-page: https://github.com/MTandHJ/freerec
 Author: MTandHJ
 Author-email: congxueric@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: freerec Version: 0.8.1 Summary: PyTorch library for
+Metadata-Version: 2.1 Name: freerec Version: 0.8.3 Summary: PyTorch library for
 recommender systems Home-page: https://github.com/MTandHJ/freerec Author:
 MTandHJ Author-email: congxueric@gmail.com License: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 PyYAML>=6.0 Requires-Dist: tensorboard>=2.10.0 Requires-Dist:
 prettytable>=3.4.1 ![](docs/src/logo.png)
```

### Comparing `freerec-0.8.1/README.md` & `freerec-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `freerec-0.8.1/freerec/__init__.py` & `freerec-0.8.3/freerec/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.8.1'
+__version__ = '0.8.3'
 
 from . import data, models, criterions, ddp, graph, launcher, metrics, parser, utils
 from .utils import infoLogger
 from freerec.dict2obj import Config
 
 
 def declare(*, version: str):
```

### Comparing `freerec-0.8.1/freerec/__main__.py` & `freerec-0.8.3/freerec/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     make_parser.add_argument(
         "--filedir", type=str, default=None, 
         help="filedir saving data. Using `dataset` instead if None (default)"
     )
 
     make_parser.add_argument(
         "--splitting", type=str, choices=('ROU', 'ROD', 'LOU', 'DOU', 'DOD'), default='ROU',
-        help="ROU: Ratio On User (default); ROD: Ratio On Dataset; LOU: Leave-One-Out; DOU: Day on User; DOD: Day on Dataset"
+        help="ROU: Ratio On User (default); ROD: Ratio On Dataset; LOU: Leave-one-out On User; DOU: Day On User; DOD: Day On Dataset"
     )
 
     make_parser.add_argument("-sp", "--star4pos", type=int, default=0, help="select interactions with `Rating >= star4pos (default: 0)'")
     make_parser.add_argument("-ku", "--kcore4user", type=int, default=10, help="select kcore (default: 10) interactions according to User")
     make_parser.add_argument("-ki", "--kcore4item", type=int, default=10, help="select kcore interactions (default: 10) according to Item")
     make_parser.add_argument("-rs", "--ratios", type=str, default="8,1,1", help="the ratios (default: 8,1,1) of training|validation|test set")
     make_parser.add_argument("--days", type=int, default=7, help="the second last days (default: 7) for validation and last days (default: 7) for test")
```

### Comparing `freerec-0.8.1/freerec/criterions.py` & `freerec-0.8.3/freerec/criterions.py`

 * *Files identical despite different names*

### Comparing `freerec-0.8.1/freerec/data/datasets/__init__.py` & `freerec-0.8.3/freerec/data/datasets/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,14 +39,26 @@
     Amazon2018Movies_550_LOU,
     Amazon2018Office_550_LOU,
     Amazon2018Sports_550_LOU,
     Amazon2018Tools_550_LOU,
     Amazon2018Toys_550_LOU
 )
 
+
+from .amazon2023 import(
+    # Matching
+    Amazon2023Baby_554811_ROU,
+    Amazon2023Beauty_554811_ROU, Amazon2023Beauty_10104811_ROU,
+    Amazon2023Fashion_554811_ROU,
+    Amazon2023Games_554811_ROU,
+    Amazon2023Office_554811_ROU,
+    Amazon2023Toys_554811_ROU, Amazon2023Toys_10104811_ROU
+)
+
+
 from .gowalla import (
     # Matching
     Gowalla2010_10100811_ROU, Gowalla2010_10100712_ROU
 )
 
 from .movielens import (
     # Matching
@@ -74,8 +86,10 @@
 
     # NextItem
     Yelp2018_550_LOU, Yelp2018_500_LOU,
     Yelp2021_550_LOU, Yelp2021_500_LOU,
 
     # NextItem (S3Rec)
     Yelp2019_550_S3Rec,
-)
+)
+
+from .microlens import MicroLens100K
```

### Comparing `freerec-0.8.1/freerec/data/datasets/allrecipes.py` & `freerec-0.8.3/freerec/data/datasets/allrecipes.py`

 * *Files identical despite different names*

### Comparing `freerec-0.8.1/freerec/data/datasets/amazon2014.py` & `freerec-0.8.3/freerec/data/datasets/amazon2014.py`

 * *Files identical despite different names*

### Comparing `freerec-0.8.1/freerec/data/datasets/amazon2018.py` & `freerec-0.8.3/freerec/data/datasets/amazon2018.py`

 * *Files identical despite different names*

### Comparing `freerec-0.8.1/freerec/data/datasets/base.py` & `freerec-0.8.3/freerec/data/datasets/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -435,15 +435,15 @@
                 )
 
         return roll_seqs
 
     def seqlens(self) -> List[int]:
         ISeq = self.fields[ITEM, ID].fork(SEQUENCE)
         seqlens = [len(row[ISeq]) for row in self.to_seqs()]
-        return list(filter(lambda x: x > 0, seqlens))
+        return seqlens
 
     @property
     def maxlen(self) -> int:
         return np.max(self.seqlens()).item()
 
     @property
     def minlen(self) -> int:
@@ -463,16 +463,16 @@
 
         for triplet in zip(traindata, validdata, testdata):
             seq = triplet[0][ISeq] + triplet[1][ISeq] + triplet[2][ISeq]
             if len(seq) != len(set(seq)):
                 return True
         return False
 
-    @timemeter
     @safe_mode('train')
+    @timemeter
     def to_heterograph(self, *edge_types: Tuple[Tuple[FieldTags], Optional[str], Tuple[FieldTags]]):
         r"""
         Convert datapipe to a heterograph.
 
         Parameters:
         -----------
         *edge_types: Tuple[Tuple[str, str], Optional[str], Tuple[str, str]]
@@ -749,15 +749,15 @@
     def summary(self):
         super().summary()
         from prettytable import PrettyTable
         User, Item = self.fields[USER, ID], self.fields[ITEM, ID]
 
         table = PrettyTable(['#Users', '#Items', 'Avg.Len', '#Interactions', '#Train', '#Valid', '#Test', 'Density'])
         table.add_row([
-            User.count, Item.count, self.train().meanlen + 2,
+            User.count, Item.count, self.train().meanlen + self.valid().meanlen + self.test().meanlen,
             self.trainsize + self.validsize + self.testsize,
             self.trainsize, self.validsize, self.testsize,
             (self.trainsize + self.validsize + self.testsize) / (User.count * Item.count)
         ])
 
         infoLogger(table)
```

### Comparing `freerec-0.8.1/freerec/data/datasets/gowalla.py` & `freerec-0.8.3/freerec/data/datasets/gowalla.py`

 * *Files identical despite different names*

### Comparing `freerec-0.8.1/freerec/data/datasets/movielens.py` & `freerec-0.8.3/freerec/data/datasets/movielens.py`

 * *Files 25% similar despite different names*

```diff
@@ -181,14 +181,18 @@
     Statistics:
     -----------
     +-------+-------+---------------+--------+--------+-------+---------------------+
     | #User | #Item | #Interactions | #Train | #Valid | #Test |       Density       |
     +-------+-------+---------------+--------+--------+-------+---------------------+
     |  943  |  1349 |     99287     | 97401  |  943   |  943  | 0.07804925214624242 |
     +-------+-------+---------------+--------+--------+-------+---------------------+
+
+    Notes:
+    MovieLens is not suitable for next-item recommendation.
+    Refer to [this paper](https://ceur-ws.org/Vol-2955/paper8.pdf) for details.
     """
 
 
 class MovieLens100K_500_LOU(NextItemRecDataSet):
     r"""
     Settings:
     ---------
@@ -200,14 +204,18 @@
     Statistics:
     -----------
     +-------+-------+---------------+--------+--------+-------+---------------------+
     | #User | #Item | #Interactions | #Train | #Valid | #Test |       Density       |
     +-------+-------+---------------+--------+--------+-------+---------------------+
     |  943  |  1682 |     100000    | 98114  |  943   |  943  | 0.06304669364224531 |
     +-------+-------+---------------+--------+--------+-------+---------------------+
+
+    Notes:
+    MovieLens is not suitable for next-item recommendation.
+    Refer to [this paper](https://ceur-ws.org/Vol-2955/paper8.pdf) for details.
     """
 
 
 class MovieLens1M_550_LOU(NextItemRecDataSet):
     r"""
     Settings:
     ---------
@@ -219,14 +227,18 @@
     Statistics:
     -----------
     +-------+-------+---------------+--------+--------+-------+----------------------+
     | #User | #Item | #Interactions | #Train | #Valid | #Test |       Density        |
     +-------+-------+---------------+--------+--------+-------+----------------------+
     |  6040 |  3416 |     999611    | 987531 |  6040  |  6040 | 0.048448041549699894 |
     +-------+-------+---------------+--------+--------+-------+----------------------+
+
+    Notes:
+    MovieLens is not suitable for next-item recommendation.
+    Refer to [this paper](https://ceur-ws.org/Vol-2955/paper8.pdf) for details.
     """
 
 
 class MovieLens1M_500_LOU(NextItemRecDataSet):
     r"""
     Settings:
     ---------
@@ -238,14 +250,18 @@
     Statistics:
     -----------
     +-------+-------+---------------+--------+--------+-------+----------------------+
     | #User | #Item | #Interactions | #Train | #Valid | #Test |       Density        |
     +-------+-------+---------------+--------+--------+-------+----------------------+
     |  6040 |  3706 |    1000209    | 988129 |  6040  |  6040 | 0.044683625622312845 |
     +-------+-------+---------------+--------+--------+-------+----------------------+
+
+    Notes:
+    MovieLens is not suitable for next-item recommendation.
+    Refer to [this paper](https://ceur-ws.org/Vol-2955/paper8.pdf) for details.
     """
 
 
 class MovieLens10M_550_LOU(NextItemRecDataSet):
     r"""
     Settings:
     ---------
@@ -257,14 +273,18 @@
     Statistics:
     -----------
     +-------+-------+---------------+---------+--------+-------+---------------------+
     | #User | #Item | #Interactions |  #Train | #Valid | #Test |       Density       |
     +-------+-------+---------------+---------+--------+-------+---------------------+
     | 69878 | 10196 |    9998816    | 9859060 | 69878  | 69878 | 0.01403389695234235 |
     +-------+-------+---------------+---------+--------+-------+---------------------+
+
+    Notes:
+    MovieLens is not suitable for next-item recommendation.
+    Refer to [this paper](https://ceur-ws.org/Vol-2955/paper8.pdf) for details.
     """
 
 
 class MovieLens10M_500_LOU(NextItemRecDataSet):
     r"""
     Settings:
     ---------
@@ -276,14 +296,18 @@
     Statistics:
     -----------
     +-------+-------+---------------+---------+--------+-------+----------------------+
     | #User | #Item | #Interactions |  #Train | #Valid | #Test |       Density        |
     +-------+-------+---------------+---------+--------+-------+----------------------+
     | 69878 | 10677 |    10000054   | 9860298 | 69878  | 69878 | 0.013403327706083809 |
     +-------+-------+---------------+---------+--------+-------+----------------------+
+
+    Notes:
+    MovieLens is not suitable for next-item recommendation.
+    Refer to [this paper](https://ceur-ws.org/Vol-2955/paper8.pdf) for details.
     """
 
 
 class MovieLens20M_550_LOU(NextItemRecDataSet):
     r"""
     Settings:
     ---------
@@ -295,14 +319,18 @@
     Statistics:
     -----------
     +--------+-------+---------------+----------+--------+--------+----------------------+
     | #User  | #Item | #Interactions |  #Train  | #Valid | #Test  |       Density        |
     +--------+-------+---------------+----------+--------+--------+----------------------+
     | 138493 | 18345 |    19984024   | 19707038 | 138493 | 138493 | 0.007865700457998398 |
     +--------+-------+---------------+----------+--------+--------+----------------------+
+
+    Notes:
+    MovieLens is not suitable for next-item recommendation.
+    Refer to [this paper](https://ceur-ws.org/Vol-2955/paper8.pdf) for details.
     """
 
 
 class MovieLens20M_500_LOU(NextItemRecDataSet):
     r"""
     Settings:
     ---------
@@ -314,8 +342,12 @@
     Statistics:
     -----------
     +--------+-------+---------------+----------+--------+--------+-----------------------+
     | #User  | #Item | #Interactions |  #Train  | #Valid | #Test  |        Density        |
     +--------+-------+---------------+----------+--------+--------+-----------------------+
     | 138493 | 26744 |    20000263   | 19723277 | 138493 | 138493 | 0.0053998478135544505 |
     +--------+-------+---------------+----------+--------+--------+-----------------------+
+
+    Notes:
+    MovieLens is not suitable for next-item recommendation.
+    Refer to [this paper](https://ceur-ws.org/Vol-2955/paper8.pdf) for details.
     """
```

### Comparing `freerec-0.8.1/freerec/data/datasets/tiktok.py` & `freerec-0.8.3/freerec/data/datasets/tiktok.py`

 * *Files identical despite different names*

### Comparing `freerec-0.8.1/freerec/data/datasets/yelp.py` & `freerec-0.8.3/freerec/data/datasets/yelp.py`

 * *Files identical despite different names*

### Comparing `freerec-0.8.1/freerec/data/fields.py` & `freerec-0.8.3/freerec/data/fields.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,20 +28,14 @@
     ---------
     >>> User = Field('User', USER)
     >>> User
     Field(User:USER)
     >>> UserID = User.fork(ID)
     >>> UserID
     Field(User:ID,USER)
-    >>> UserID == User
-    False
-    >>> UserID >= User
-    False
-    >>> UserID <= User
-    True
     >>> Field.issubfield(UserID, User)
     True
     >>> Field.issuperfield(User, UserID)
     True
     >>> UserID.match(USER)
     True
     >>> UserID.match(ID)
@@ -53,23 +47,22 @@
     >>> UserID.match_any()
     False
     >>> list(UserID)
     [<FieldTags.ID: 'ID'>, <FieldTags.USER: 'USER'>]
     >>> UserID1 = Field('UserID1', USER, ID)
     >>> UserID2 = Field('UserID2', USER, ID)
     >>> UserID1 == UserID2
-    True
-    >>> hash(UserID1) == hash(UserID2)
     False
     """
 
     def __init__(self, name: str,  *tags: FieldTags) -> None:
-        self.__name = name
+        self.__name = str(name)
         self.__tags = set(tags)
         self.__identifier = (name,) + tuple(sorted(self.__tags, key=lambda tag: tag.value))
+        self.__hash_value = hash(self.identifier)
         self.count = None
 
     @property
     def name(self) -> str:
         return self.__name
 
     @property
@@ -124,25 +117,19 @@
     def issuperfield(self, other: 'Field') -> bool:
         """True if `other` matches all tags of `self`."""
         return other.match(*self.tags)
 
     def __iter__(self):
         return iter(self.tags)
 
-    def __eq__(self, other) -> bool:
-        return isinstance(other, Field) and self.tags == other.tags
-
-    def __le__(self, other: 'Field') -> bool:
-        return self.issubfield(other)
-
-    def __ge__(self, other: 'Field') -> bool:
-        return self.issuperfield(other)
-
     def __hash__(self) -> int:
-        return hash(self.identifier)
+        return self.__hash_value
+
+    def __eq__(self, other) -> bool:
+        return isinstance(other, Field) and hash(self) == hash(other)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({str(self)})"
 
     def __str__(self) -> str:
         return f"{self.name}:{','.join(map(lambda tag: tag.name, self.tags))}"
```

### Comparing `freerec-0.8.1/freerec/data/postprocessing/__init__.py` & `freerec-0.8.3/freerec/data/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `freerec-0.8.1/freerec/data/postprocessing/base.py` & `freerec-0.8.3/freerec/data/postprocessing/base.py`

 * *Files identical despite different names*

### Comparing `freerec-0.8.1/freerec/data/postprocessing/base.pyi` & `freerec-0.8.3/freerec/data/postprocessing/base.pyi`

 * *Files identical despite different names*

### Comparing `freerec-0.8.1/freerec/data/postprocessing/column.py` & `freerec-0.8.3/freerec/data/postprocessing/column.py`

 * *Files identical despite different names*

### Comparing `freerec-0.8.1/freerec/data/postprocessing/row.py` & `freerec-0.8.3/freerec/data/postprocessing/row.py`

 * *Files 1% similar despite different names*

```diff
@@ -482,128 +482,133 @@
 00001e10: 6c66 293a 0d0a 2020 2020 2020 2020 6465  lf):..        de
 00001e20: 6620 6775 6573 735f 7a65 726f 2866 6965  f guess_zero(fie
 00001e30: 6c64 3a20 4669 656c 642c 2076 616c 7565  ld: Field, value
 00001e40: 3a20 4974 6572 6162 6c65 293a 0d0a 2020  : Iterable):..  
 00001e50: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
 00001e60: 6e73 7461 6e63 6528 7661 6c75 652c 2049  nstance(value, I
 00001e70: 7465 7261 626c 6529 3a0d 0a20 2020 2020  terable):..     
-00001e80: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-00001e90: 696e 7374 616e 6365 2876 616c 7565 5b30  instance(value[0
-00001ea0: 5d2c 2049 7465 7261 626c 6529 3a0d 0a20  ], Iterable):.. 
-00001eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ec0: 2020 2072 6574 7572 6e20 2873 656c 662e     return (self.
-00001ed0: 7061 6464 696e 675f 7661 6c75 652c 2920  padding_value,) 
-00001ee0: 2a20 6c65 6e28 7661 6c75 655b 305d 290d  * len(value[0]).
-00001ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001f00: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00001f10: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00001f20: 726e 2073 656c 662e 7061 6464 696e 675f  rn self.padding_
-00001f30: 7661 6c75 650d 0a20 2020 2020 2020 2020  value..         
-00001f40: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00001f50: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00001f60: 5661 6c75 6545 7272 6f72 2866 227b 7661  ValueError(f"{va
-00001f70: 6c75 657d 2066 6f72 207b 6669 656c 647d  lue} for {field}
-00001f80: 2069 7320 6e6f 7420 6e6f 6e2d 6974 6572   is not non-iter
-00001f90: 6162 6c65 202e 2e2e 2229 0d0a 0d0a 2020  able ...")....  
-00001fa0: 2020 2020 2020 726f 7720 3d20 6e65 7874        row = next
-00001fb0: 2869 7465 7228 7365 6c66 2e73 6f75 7263  (iter(self.sourc
-00001fc0: 6529 290d 0a20 2020 2020 2020 2073 656c  e))..        sel
-00001fd0: 662e 7a65 726f 7320 3d20 6469 6374 2829  f.zeros = dict()
-00001fe0: 0d0a 2020 2020 2020 2020 666f 7220 6669  ..        for fi
-00001ff0: 656c 6420 696e 2073 656c 662e 6d6f 6469  eld in self.modi
-00002000: 6669 6564 5f66 6965 6c64 733a 0d0a 2020  fied_fields:..  
-00002010: 2020 2020 2020 2020 2020 7365 6c66 2e7a            self.z
-00002020: 6572 6f73 5b66 6965 6c64 5d20 3d20 6775  eros[field] = gu
-00002030: 6573 735f 7a65 726f 2866 6965 6c64 2c20  ess_zero(field, 
-00002040: 726f 775b 6669 656c 645d 290d 0a0d 0a20  row[field]).... 
-00002050: 2020 2064 6566 205f 7061 6428 7365 6c66     def _pad(self
-00002060: 2c20 6669 656c 643a 2046 6965 6c64 2c20  , field: Field, 
-00002070: 783a 2049 7465 7261 626c 6529 202d 3e20  x: Iterable) -> 
-00002080: 4c69 7374 3a0d 0a20 2020 2020 2020 2072  List:..        r
-00002090: 6574 7572 6e20 6c69 7374 2863 6861 696e  eturn list(chain
-000020a0: 2872 6570 6561 7428 7365 6c66 2e7a 6572  (repeat(self.zer
-000020b0: 6f73 5b66 6965 6c64 5d2c 2073 656c 662e  os[field], self.
-000020c0: 6d61 786c 656e 202d 206c 656e 2878 2929  maxlen - len(x))
-000020d0: 2c20 7829 290d 0a0d 0a0d 0a40 6470 2e66  , x))......@dp.f
-000020e0: 756e 6374 696f 6e61 6c5f 6461 7461 7069  unctional_datapi
-000020f0: 7065 2822 7270 6164 5f22 290d 0a63 6c61  pe("rpad_")..cla
-00002100: 7373 2052 6967 6874 5061 6464 696e 6752  ss RightPaddingR
-00002110: 6f77 284c 6566 7450 6164 6469 6e67 526f  ow(LeftPaddingRo
-00002120: 7729 3a0d 0a20 2020 2072 2222 220d 0a20  w):..    r""".. 
-00002130: 2020 2041 2066 756e 6374 696f 6e61 6c20     A functional 
-00002140: 6461 7461 2070 6970 656c 696e 6520 636f  data pipeline co
-00002150: 6d70 6f6e 656e 7420 7468 6174 2072 6967  mponent that rig
-00002160: 6874 2070 6164 7320 7365 7175 656e 6365  ht pads sequence
-00002170: 7320 746f 2061 206d 6178 696d 756d 206c  s to a maximum l
-00002180: 656e 6774 682e 0d0a 0d0a 2020 2020 5061  ength.....    Pa
-00002190: 7261 6d65 7465 7273 3a0d 0a20 2020 202d  rameters:..    -
-000021a0: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020  ----------..    
-000021b0: 6d61 786c 656e 203a 2069 6e74 0d0a 2020  maxlen : int..  
-000021c0: 2020 2020 2020 5468 6520 6d61 7869 6d75        The maximu
-000021d0: 6d20 6c65 6e67 7468 2074 6f20 7061 6420  m length to pad 
-000021e0: 7468 6520 7365 7175 656e 6365 7320 746f  the sequences to
-000021f0: 2e0d 0a20 2020 206d 6f64 6966 6965 6c64  ...    modifield
-00002200: 735f 6669 656c 6473 3a20 4974 6572 6162  s_fields: Iterab
-00002210: 6c65 5b46 6965 6c64 5d0d 0a20 2020 2020  le[Field]..     
-00002220: 2020 2054 6865 2066 6965 6c64 7320 746f     The fields to
-00002230: 2062 6520 6d6f 6469 6669 6564 2e0d 0a20   be modified... 
-00002240: 2020 2070 6164 6469 6e67 5f76 616c 7565     padding_value
-00002250: 203a 2069 6e74 2c20 6f70 7469 6f6e 616c   : int, optional
-00002260: 2028 6465 6661 756c 743d 3029 0d0a 2020   (default=0)..  
-00002270: 2020 2020 2020 5468 6520 7661 6c75 6520        The value 
-00002280: 746f 2075 7365 2066 6f72 2070 6164 6469  to use for paddi
-00002290: 6e67 2e0d 0a0d 0a20 2020 2046 6c6f 7773  ng.....    Flows
-000022a0: 3a0d 0a20 2020 202d 2d2d 2d2d 2d0d 0a20  :..    ------.. 
-000022b0: 2020 205b 312c 2032 2c20 332c 2034 5d20     [1, 2, 3, 4] 
-000022c0: 2d2d 286d 6178 6c65 6e3d 372c 2070 6164  --(maxlen=7, pad
-000022d0: 6469 6e67 5f76 616c 7565 3d30 292d 2d3e  ding_value=0)-->
-000022e0: 205b 312c 2032 2c20 332c 2034 2c20 302c   [1, 2, 3, 4, 0,
-000022f0: 2030 2c20 305d 0d0a 2020 2020 5b31 2c20   0, 0]..    [1, 
-00002300: 322c 2033 2c20 345d 202d 2d28 6d61 786c  2, 3, 4] --(maxl
-00002310: 656e 3d34 2c20 7061 6464 696e 675f 7661  en=4, padding_va
-00002320: 6c75 653d 3029 2d2d 3e20 5b31 2c20 322c  lue=0)--> [1, 2,
-00002330: 2033 2c20 345d 0d0a 0d0a 2020 2020 4578   3, 4]....    Ex
-00002340: 616d 706c 6573 3a0d 0a20 2020 202d 2d2d  amples:..    ---
-00002350: 2d2d 2d2d 2d2d 0d0a 2020 2020 3e3e 3e20  ------..    >>> 
-00002360: 6461 7461 7365 743a 2052 6563 4461 7461  dataset: RecData
-00002370: 5365 740d 0a20 2020 203e 3e3e 2049 5365  Set..    >>> ISe
-00002380: 7120 3d20 6461 7461 7365 745b 4954 454d  q = dataset[ITEM
-00002390: 2c20 4944 5d2e 666f 726b 2853 4551 5545  , ID].fork(SEQUE
-000023a0: 4e43 4529 0d0a 2020 2020 3e3e 3e20 6461  NCE)..    >>> da
-000023b0: 7461 7069 7065 203d 2064 6174 6173 6574  tapipe = dataset
-000023c0: 2e76 616c 6964 2829 2e6f 7264 6572 6564  .valid().ordered
-000023d0: 5f75 7365 725f 6964 735f 736f 7572 6365  _user_ids_source
-000023e0: 280d 0a20 2020 2029 2e76 616c 6964 5f73  (..    ).valid_s
-000023f0: 616d 706c 696e 675f 2829 2e72 7072 756e  ampling_().rprun
-00002400: 655f 280d 0a20 2020 2020 2020 2033 2c20  e_(..        3, 
-00002410: 6d6f 6469 6669 6564 5f66 6965 6c64 733d  modified_fields=
-00002420: 2849 5365 712c 290d 0a20 2020 2029 2e61  (ISeq,)..    ).a
-00002430: 6464 5f28 0d0a 2020 2020 2020 2020 312c  dd_(..        1,
-00002440: 206d 6f64 6966 6965 645f 6669 656c 6473   modified_fields
-00002450: 3d28 4953 6571 2c29 0d0a 2020 2020 292e  =(ISeq,)..    ).
-00002460: 7270 6164 5f28 0d0a 2020 2020 2020 2020  rpad_(..        
-00002470: 352c 206d 6f64 6966 6965 645f 6669 656c  5, modified_fiel
-00002480: 6473 3d28 4953 6571 2c29 0d0a 2020 2020  ds=(ISeq,)..    
-00002490: 290d 0a20 2020 203e 3e3e 206e 6578 7428  )..    >>> next(
-000024a0: 6974 6572 2864 6174 6170 6970 6529 290d  iter(datapipe)).
-000024b0: 0a20 2020 207b 4669 656c 6428 5553 4552  .    {Field(USER
-000024c0: 3a49 442c 5553 4552 293a 2030 2c0d 0a20  :ID,USER): 0,.. 
-000024d0: 2020 2046 6965 6c64 2849 5445 4d3a 4944     Field(ITEM:ID
-000024e0: 2c49 5445 4d2c 5345 5155 454e 4345 293a  ,ITEM,SEQUENCE):
-000024f0: 205b 3934 3530 2c20 3938 3430 2c20 3130   [9450, 9840, 10
-00002500: 3037 372c 2030 2c20 305d 2c0d 0a20 2020  077, 0, 0],..   
-00002510: 2046 6965 6c64 2849 5445 4d3a 4944 2c49   Field(ITEM:ID,I
-00002520: 5445 4d2c 554e 5345 454e 293a 2028 3131  TEM,UNSEEN): (11
-00002530: 3735 322c 292c 0d0a 2020 2020 4669 656c  752,),..    Fiel
-00002540: 6428 4954 454d 3a49 442c 4954 454d 2c53  d(ITEM:ID,ITEM,S
-00002550: 4545 4e29 3a20 2839 3434 392c 2039 3833  EEN): (9449, 983
-00002560: 392c 2031 3030 3736 2c20 3131 3135 3529  9, 10076, 11155)
-00002570: 7d0d 0a20 2020 2022 2222 0d0a 0d0a 2020  }..    """....  
-00002580: 2020 6465 6620 5f70 6164 2873 656c 662c    def _pad(self,
-00002590: 2066 6965 6c64 3a20 4669 656c 642c 2078   field: Field, x
-000025a0: 3a20 4974 6572 6162 6c65 2920 2d3e 204c  : Iterable) -> L
-000025b0: 6973 743a 0d0a 2020 2020 2020 2020 7265  ist:..        re
-000025c0: 7475 726e 206c 6973 7428 6368 6169 6e28  turn list(chain(
-000025d0: 782c 2072 6570 6561 7428 7365 6c66 2e7a  x, repeat(self.z
-000025e0: 6572 6f73 5b66 6965 6c64 5d2c 2073 656c  eros[field], sel
-000025f0: 662e 6d61 786c 656e 202d 206c 656e 2878  f.maxlen - len(x
-00002600: 2929 2929                                ))))
+00001e80: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+00001e90: 6e28 7661 6c75 6529 203d 3d20 303a 0d0a  n(value) == 0:..
+00001ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001eb0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00001ec0: 7061 6464 696e 675f 7661 6c75 650d 0a20  padding_value.. 
+00001ed0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00001ee0: 6c69 6620 6973 696e 7374 616e 6365 2876  lif isinstance(v
+00001ef0: 616c 7565 5b30 5d2c 2049 7465 7261 626c  alue[0], Iterabl
+00001f00: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
+00001f10: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00001f20: 2873 656c 662e 7061 6464 696e 675f 7661  (self.padding_va
+00001f30: 6c75 652c 2920 2a20 6c65 6e28 7661 6c75  lue,) * len(valu
+00001f40: 655b 305d 290d 0a20 2020 2020 2020 2020  e[0])..         
+00001f50: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00001f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f70: 2020 7265 7475 726e 2073 656c 662e 7061    return self.pa
+00001f80: 6464 696e 675f 7661 6c75 650d 0a20 2020  dding_value..   
+00001f90: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00001fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fb0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00001fc0: 2866 227b 7661 6c75 657d 2066 6f72 207b  (f"{value} for {
+00001fd0: 6669 656c 647d 2069 7320 6e6f 7420 6e6f  field} is not no
+00001fe0: 6e2d 6974 6572 6162 6c65 202e 2e2e 2229  n-iterable ...")
+00001ff0: 0d0a 0d0a 2020 2020 2020 2020 726f 7720  ....        row 
+00002000: 3d20 6e65 7874 2869 7465 7228 7365 6c66  = next(iter(self
+00002010: 2e73 6f75 7263 6529 290d 0a20 2020 2020  .source))..     
+00002020: 2020 2073 656c 662e 7a65 726f 7320 3d20     self.zeros = 
+00002030: 6469 6374 2829 0d0a 2020 2020 2020 2020  dict()..        
+00002040: 666f 7220 6669 656c 6420 696e 2073 656c  for field in sel
+00002050: 662e 6d6f 6469 6669 6564 5f66 6965 6c64  f.modified_field
+00002060: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00002070: 7365 6c66 2e7a 6572 6f73 5b66 6965 6c64  self.zeros[field
+00002080: 5d20 3d20 6775 6573 735f 7a65 726f 2866  ] = guess_zero(f
+00002090: 6965 6c64 2c20 726f 775b 6669 656c 645d  ield, row[field]
+000020a0: 290d 0a0d 0a20 2020 2064 6566 205f 7061  )....    def _pa
+000020b0: 6428 7365 6c66 2c20 6669 656c 643a 2046  d(self, field: F
+000020c0: 6965 6c64 2c20 783a 2049 7465 7261 626c  ield, x: Iterabl
+000020d0: 6529 202d 3e20 4c69 7374 3a0d 0a20 2020  e) -> List:..   
+000020e0: 2020 2020 2072 6574 7572 6e20 6c69 7374       return list
+000020f0: 2863 6861 696e 2872 6570 6561 7428 7365  (chain(repeat(se
+00002100: 6c66 2e7a 6572 6f73 5b66 6965 6c64 5d2c  lf.zeros[field],
+00002110: 2073 656c 662e 6d61 786c 656e 202d 206c   self.maxlen - l
+00002120: 656e 2878 2929 2c20 7829 290d 0a0d 0a0d  en(x)), x)).....
+00002130: 0a40 6470 2e66 756e 6374 696f 6e61 6c5f  .@dp.functional_
+00002140: 6461 7461 7069 7065 2822 7270 6164 5f22  datapipe("rpad_"
+00002150: 290d 0a63 6c61 7373 2052 6967 6874 5061  )..class RightPa
+00002160: 6464 696e 6752 6f77 284c 6566 7450 6164  ddingRow(LeftPad
+00002170: 6469 6e67 526f 7729 3a0d 0a20 2020 2072  dingRow):..    r
+00002180: 2222 220d 0a20 2020 2041 2066 756e 6374  """..    A funct
+00002190: 696f 6e61 6c20 6461 7461 2070 6970 656c  ional data pipel
+000021a0: 696e 6520 636f 6d70 6f6e 656e 7420 7468  ine component th
+000021b0: 6174 2072 6967 6874 2070 6164 7320 7365  at right pads se
+000021c0: 7175 656e 6365 7320 746f 2061 206d 6178  quences to a max
+000021d0: 696d 756d 206c 656e 6774 682e 0d0a 0d0a  imum length.....
+000021e0: 2020 2020 5061 7261 6d65 7465 7273 3a0d      Parameters:.
+000021f0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
+00002200: 0d0a 2020 2020 6d61 786c 656e 203a 2069  ..    maxlen : i
+00002210: 6e74 0d0a 2020 2020 2020 2020 5468 6520  nt..        The 
+00002220: 6d61 7869 6d75 6d20 6c65 6e67 7468 2074  maximum length t
+00002230: 6f20 7061 6420 7468 6520 7365 7175 656e  o pad the sequen
+00002240: 6365 7320 746f 2e0d 0a20 2020 206d 6f64  ces to...    mod
+00002250: 6966 6965 6c64 735f 6669 656c 6473 3a20  ifields_fields: 
+00002260: 4974 6572 6162 6c65 5b46 6965 6c64 5d0d  Iterable[Field].
+00002270: 0a20 2020 2020 2020 2054 6865 2066 6965  .        The fie
+00002280: 6c64 7320 746f 2062 6520 6d6f 6469 6669  lds to be modifi
+00002290: 6564 2e0d 0a20 2020 2070 6164 6469 6e67  ed...    padding
+000022a0: 5f76 616c 7565 203a 2069 6e74 2c20 6f70  _value : int, op
+000022b0: 7469 6f6e 616c 2028 6465 6661 756c 743d  tional (default=
+000022c0: 3029 0d0a 2020 2020 2020 2020 5468 6520  0)..        The 
+000022d0: 7661 6c75 6520 746f 2075 7365 2066 6f72  value to use for
+000022e0: 2070 6164 6469 6e67 2e0d 0a0d 0a20 2020   padding.....   
+000022f0: 2046 6c6f 7773 3a0d 0a20 2020 202d 2d2d   Flows:..    ---
+00002300: 2d2d 2d0d 0a20 2020 205b 312c 2032 2c20  ---..    [1, 2, 
+00002310: 332c 2034 5d20 2d2d 286d 6178 6c65 6e3d  3, 4] --(maxlen=
+00002320: 372c 2070 6164 6469 6e67 5f76 616c 7565  7, padding_value
+00002330: 3d30 292d 2d3e 205b 312c 2032 2c20 332c  =0)--> [1, 2, 3,
+00002340: 2034 2c20 302c 2030 2c20 305d 0d0a 2020   4, 0, 0, 0]..  
+00002350: 2020 5b31 2c20 322c 2033 2c20 345d 202d    [1, 2, 3, 4] -
+00002360: 2d28 6d61 786c 656e 3d34 2c20 7061 6464  -(maxlen=4, padd
+00002370: 696e 675f 7661 6c75 653d 3029 2d2d 3e20  ing_value=0)--> 
+00002380: 5b31 2c20 322c 2033 2c20 345d 0d0a 0d0a  [1, 2, 3, 4]....
+00002390: 2020 2020 4578 616d 706c 6573 3a0d 0a20      Examples:.. 
+000023a0: 2020 202d 2d2d 2d2d 2d2d 2d2d 0d0a 2020     ---------..  
+000023b0: 2020 3e3e 3e20 6461 7461 7365 743a 2052    >>> dataset: R
+000023c0: 6563 4461 7461 5365 740d 0a20 2020 203e  ecDataSet..    >
+000023d0: 3e3e 2049 5365 7120 3d20 6461 7461 7365  >> ISeq = datase
+000023e0: 745b 4954 454d 2c20 4944 5d2e 666f 726b  t[ITEM, ID].fork
+000023f0: 2853 4551 5545 4e43 4529 0d0a 2020 2020  (SEQUENCE)..    
+00002400: 3e3e 3e20 6461 7461 7069 7065 203d 2064  >>> datapipe = d
+00002410: 6174 6173 6574 2e76 616c 6964 2829 2e6f  ataset.valid().o
+00002420: 7264 6572 6564 5f75 7365 725f 6964 735f  rdered_user_ids_
+00002430: 736f 7572 6365 280d 0a20 2020 2029 2e76  source(..    ).v
+00002440: 616c 6964 5f73 616d 706c 696e 675f 2829  alid_sampling_()
+00002450: 2e72 7072 756e 655f 280d 0a20 2020 2020  .rprune_(..     
+00002460: 2020 2033 2c20 6d6f 6469 6669 6564 5f66     3, modified_f
+00002470: 6965 6c64 733d 2849 5365 712c 290d 0a20  ields=(ISeq,).. 
+00002480: 2020 2029 2e61 6464 5f28 0d0a 2020 2020     ).add_(..    
+00002490: 2020 2020 312c 206d 6f64 6966 6965 645f      1, modified_
+000024a0: 6669 656c 6473 3d28 4953 6571 2c29 0d0a  fields=(ISeq,)..
+000024b0: 2020 2020 292e 7270 6164 5f28 0d0a 2020      ).rpad_(..  
+000024c0: 2020 2020 2020 352c 206d 6f64 6966 6965        5, modifie
+000024d0: 645f 6669 656c 6473 3d28 4953 6571 2c29  d_fields=(ISeq,)
+000024e0: 0d0a 2020 2020 290d 0a20 2020 203e 3e3e  ..    )..    >>>
+000024f0: 206e 6578 7428 6974 6572 2864 6174 6170   next(iter(datap
+00002500: 6970 6529 290d 0a20 2020 207b 4669 656c  ipe))..    {Fiel
+00002510: 6428 5553 4552 3a49 442c 5553 4552 293a  d(USER:ID,USER):
+00002520: 2030 2c0d 0a20 2020 2046 6965 6c64 2849   0,..    Field(I
+00002530: 5445 4d3a 4944 2c49 5445 4d2c 5345 5155  TEM:ID,ITEM,SEQU
+00002540: 454e 4345 293a 205b 3934 3530 2c20 3938  ENCE): [9450, 98
+00002550: 3430 2c20 3130 3037 372c 2030 2c20 305d  40, 10077, 0, 0]
+00002560: 2c0d 0a20 2020 2046 6965 6c64 2849 5445  ,..    Field(ITE
+00002570: 4d3a 4944 2c49 5445 4d2c 554e 5345 454e  M:ID,ITEM,UNSEEN
+00002580: 293a 2028 3131 3735 322c 292c 0d0a 2020  ): (11752,),..  
+00002590: 2020 4669 656c 6428 4954 454d 3a49 442c    Field(ITEM:ID,
+000025a0: 4954 454d 2c53 4545 4e29 3a20 2839 3434  ITEM,SEEN): (944
+000025b0: 392c 2039 3833 392c 2031 3030 3736 2c20  9, 9839, 10076, 
+000025c0: 3131 3135 3529 7d0d 0a20 2020 2022 2222  11155)}..    """
+000025d0: 0d0a 0d0a 2020 2020 6465 6620 5f70 6164  ....    def _pad
+000025e0: 2873 656c 662c 2066 6965 6c64 3a20 4669  (self, field: Fi
+000025f0: 656c 642c 2078 3a20 4974 6572 6162 6c65  eld, x: Iterable
+00002600: 2920 2d3e 204c 6973 743a 0d0a 2020 2020  ) -> List:..    
+00002610: 2020 2020 7265 7475 726e 206c 6973 7428      return list(
+00002620: 6368 6169 6e28 782c 2072 6570 6561 7428  chain(x, repeat(
+00002630: 7365 6c66 2e7a 6572 6f73 5b66 6965 6c64  self.zeros[field
+00002640: 5d2c 2073 656c 662e 6d61 786c 656e 202d  ], self.maxlen -
+00002650: 206c 656e 2878 2929 2929                  len(x))))
```

### Comparing `freerec-0.8.1/freerec/data/postprocessing/sampler.py` & `freerec-0.8.3/freerec/data/postprocessing/sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,16 +186,17 @@
                 seen, self.Item.count, self.num_negatives
             )
         else:
             return [self._sample_one(seen) for _ in range(self.num_negatives)]
 
     def __iter__(self):
         for row in self.source:
-            user = row[self.User]
-            row[self.INeg] = self._sample_neg(user)
+            row[self.INeg] = self._sample_neg(
+                row[self.User]
+            )
             yield row
 
 
 @dp.functional_datapipe("seq_train_yielding_pos_")
 class SeqTrainPositiveYielder(BaseSampler):
     r"""
     Yielding positive sequence for each user sequence.
```

### Comparing `freerec-0.8.1/freerec/data/postprocessing/source.py` & `freerec-0.8.3/freerec/data/postprocessing/source.py`

 * *Files identical despite different names*

### Comparing `freerec-0.8.1/freerec/data/preprocessing/base.py` & `freerec-0.8.3/freerec/data/preprocessing/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,15 +349,15 @@
         self.trainiter = self.interactions.iloc[:markers[0]]
         self.validiter = self.interactions.iloc[markers[0]:markers[1]]
         self.testiter = self.interactions.iloc[markers[1]:]
 
         return ''.join(map(str, ratios)) + '_ROD'
 
     def split_by_LOU(self):
-        infoLogger(f"[Converter] >>> Split by LOU (Leave-One-Out) ...")
+        infoLogger(f"[Converter] >>> Split by LOU (Leave-one-out On User) ...")
         traingroups = []
         validgroups = []
         testgroups = []
         for _, group in self.interactions.groupby(USER.name):
             if len(group) == 0:
                 continue
             if len(group) <= 3:
@@ -486,15 +486,15 @@
         kcore4item: int, default to 10
             Select kcore interactions according to Item.
         star4pos: int, default to 0
             Select interactions with `Rating >= star4pos'.
         splitting: str ('ROU', 'ROD', 'LOU', 'DOU', 'DOD')
             `ROU`: Ratio on User
             `ROD`: Ratio on Dataset
-            `LOU`: Leave-One-Out
+            `LOU`: Leave-one-out on User
             `DOU`: Day on User
             `DOD`: Day on Dataset
         ratios: Tuple[int, int, int], default to (8, 1, 1)
             ROU|ROD: The ratios of training|validation|test set.
         days: int
             DOU|DOD: The days remained for validation|test set
         strict: bool, default to `True`
```

### Comparing `freerec-0.8.1/freerec/data/tags.py` & `freerec-0.8.3/freerec/data/tags.py`

 * *Files identical despite different names*

### Comparing `freerec-0.8.1/freerec/data/utils.py` & `freerec-0.8.3/freerec/data/utils.py`

 * *Files identical despite different names*

### Comparing `freerec-0.8.1/freerec/ddp.py` & `freerec-0.8.3/freerec/ddp.py`

 * *Files identical despite different names*

### Comparing `freerec-0.8.1/freerec/dict2obj.py` & `freerec-0.8.3/freerec/dict2obj.py`

 * *Files identical despite different names*

### Comparing `freerec-0.8.1/freerec/graph.py` & `freerec-0.8.3/freerec/graph.py`

 * *Files identical despite different names*

### Comparing `freerec-0.8.1/freerec/launcher.py` & `freerec-0.8.3/freerec/launcher.py`

 * *Files identical despite different names*

### Comparing `freerec-0.8.1/freerec/metrics.py` & `freerec-0.8.3/freerec/metrics.py`

 * *Files identical despite different names*

### Comparing `freerec-0.8.1/freerec/models/base.py` & `freerec-0.8.3/freerec/models/base.py`

 * *Files identical despite different names*

### Comparing `freerec-0.8.1/freerec/parser.py` & `freerec-0.8.3/freerec/parser.py`

 * *Files identical despite different names*

### Comparing `freerec-0.8.1/freerec/utils.py` & `freerec-0.8.3/freerec/utils.py`

 * *Files identical despite different names*

### Comparing `freerec-0.8.1/freerec.egg-info/PKG-INFO` & `freerec-0.8.3/freerec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freerec
-Version: 0.8.1
+Version: 0.8.3
 Summary: PyTorch library for recommender systems
 Home-page: https://github.com/MTandHJ/freerec
 Author: MTandHJ
 Author-email: congxueric@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: freerec Version: 0.8.1 Summary: PyTorch library for
+Metadata-Version: 2.1 Name: freerec Version: 0.8.3 Summary: PyTorch library for
 recommender systems Home-page: https://github.com/MTandHJ/freerec Author:
 MTandHJ Author-email: congxueric@gmail.com License: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 PyYAML>=6.0 Requires-Dist: tensorboard>=2.10.0 Requires-Dist:
 prettytable>=3.4.1 ![](docs/src/logo.png)
```

### Comparing `freerec-0.8.1/freerec.egg-info/SOURCES.txt` & `freerec-0.8.3/freerec.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -21,23 +21,26 @@
 freerec/data/fields.py
 freerec/data/tags.py
 freerec/data/utils.py
 freerec/data/datasets/__init__.py
 freerec/data/datasets/allrecipes.py
 freerec/data/datasets/amazon2014.py
 freerec/data/datasets/amazon2018.py
+freerec/data/datasets/amazon2023.py
 freerec/data/datasets/base.py
 freerec/data/datasets/gowalla.py
+freerec/data/datasets/microlens.py
 freerec/data/datasets/movielens.py
 freerec/data/datasets/tiktok.py
 freerec/data/datasets/yelp.py
 freerec/data/postprocessing/__init__.py
 freerec/data/postprocessing/base.py
 freerec/data/postprocessing/base.pyi
 freerec/data/postprocessing/column.py
 freerec/data/postprocessing/row.py
 freerec/data/postprocessing/sampler.py
 freerec/data/postprocessing/source.py
 freerec/data/preprocessing/__init__.py
+freerec/data/preprocessing/amazon2023.py
 freerec/data/preprocessing/base.py
 freerec/models/__init__.py
 freerec/models/base.py
```

### Comparing `freerec-0.8.1/setup.py` & `freerec-0.8.3/setup.py`

 * *Files identical despite different names*

