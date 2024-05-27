# Comparing `tmp/ambr_py-1.7.5.tar.gz` & `tmp/ambr_py-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambr_py-1.7.5.tar", max compression
+gzip compressed data, was "ambr_py-1.7.6.tar", max compression
```

## Comparing `ambr_py-1.7.5.tar` & `ambr_py-1.7.6.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0       73 2024-01-15 00:08:53.036511 ambr_py-1.7.5/ambr/__init__.py
--rw-r--r--   0        0        0    19669 2024-05-25 05:26:05.892430 ambr_py-1.7.5/ambr/client.py
--rw-r--r--   0        0        0      660 2024-05-21 23:25:02.918034 ambr_py-1.7.5/ambr/exceptions.py
--rw-r--r--   0        0        0      415 2024-02-25 01:39:24.545071 ambr_py-1.7.5/ambr/models/__init__.py
--rw-r--r--   0        0        0     6940 2024-05-21 23:25:02.918034 ambr_py-1.7.5/ambr/models/abyss.py
--rw-r--r--   0        0        0     2615 2024-05-21 23:25:02.918034 ambr_py-1.7.5/ambr/models/achievement.py
--rw-r--r--   0        0        0     3494 2024-05-21 23:25:02.919228 ambr_py-1.7.5/ambr/models/artifact.py
--rw-r--r--   0        0        0     1658 2024-05-21 23:25:02.919228 ambr_py-1.7.5/ambr/models/book.py
--rw-r--r--   0        0        0      820 2024-05-21 23:25:02.919228 ambr_py-1.7.5/ambr/models/changelog.py
--rw-r--r--   0        0        0     8659 2024-05-21 23:25:02.919228 ambr_py-1.7.5/ambr/models/character.py
--rw-r--r--   0        0        0     2590 2024-05-21 23:25:02.919228 ambr_py-1.7.5/ambr/models/character_fetter.py
--rw-r--r--   0        0        0     1299 2024-03-13 06:39:04.183353 ambr_py-1.7.5/ambr/models/domain.py
--rw-r--r--   0        0        0     2994 2024-05-21 23:25:02.919228 ambr_py-1.7.5/ambr/models/food.py
--rw-r--r--   0        0        0     5057 2024-05-21 23:25:02.919228 ambr_py-1.7.5/ambr/models/furniture.py
--rw-r--r--   0        0        0     3050 2024-05-21 23:25:02.919228 ambr_py-1.7.5/ambr/models/material.py
--rw-r--r--   0        0        0     2406 2024-05-21 23:25:02.919228 ambr_py-1.7.5/ambr/models/monster.py
--rw-r--r--   0        0        0     1683 2024-05-21 23:25:02.919228 ambr_py-1.7.5/ambr/models/name_card.py
--rw-r--r--   0        0        0     1221 2024-02-25 01:37:40.383910 ambr_py-1.7.5/ambr/models/quest.py
--rw-r--r--   0        0        0     5209 2024-05-21 23:25:02.920478 ambr_py-1.7.5/ambr/models/tcg.py
--rw-r--r--   0        0        0      996 2024-05-21 23:25:02.920478 ambr_py-1.7.5/ambr/models/upgrade.py
--rw-r--r--   0        0        0     4270 2024-05-21 23:25:02.920478 ambr_py-1.7.5/ambr/models/weapon.py
--rw-r--r--   0        0        0     1117 2024-02-25 01:37:40.384914 ambr_py-1.7.5/ambr/utils.py
--rw-r--r--   0        0        0    35803 2024-01-15 00:08:53.036002 ambr_py-1.7.5/LICENSE
--rw-r--r--   0        0        0     1625 2024-05-25 08:10:47.567573 ambr_py-1.7.5/pyproject.toml
--rw-r--r--   0        0        0     2097 2024-05-15 01:10:41.857221 ambr_py-1.7.5/README.md
--rw-r--r--   0        0        0     2650 1970-01-01 00:00:00.000000 ambr_py-1.7.5/PKG-INFO
+-rw-r--r--   0        0        0      105 2024-05-27 07:20:37.225697 ambr_py-1.7.6/ambr/__init__.py
+-rw-r--r--   0        0        0    19669 2024-05-25 05:26:05.892430 ambr_py-1.7.6/ambr/client.py
+-rw-r--r--   0        0        0      867 2024-05-27 07:21:39.029698 ambr_py-1.7.6/ambr/constants.py
+-rw-r--r--   0        0        0      660 2024-05-21 23:25:02.918034 ambr_py-1.7.6/ambr/exceptions.py
+-rw-r--r--   0        0        0      415 2024-02-25 01:39:24.545071 ambr_py-1.7.6/ambr/models/__init__.py
+-rw-r--r--   0        0        0     6940 2024-05-27 07:30:34.844316 ambr_py-1.7.6/ambr/models/abyss.py
+-rw-r--r--   0        0        0     2615 2024-05-27 07:30:34.844316 ambr_py-1.7.6/ambr/models/achievement.py
+-rw-r--r--   0        0        0     3494 2024-05-27 07:30:34.844316 ambr_py-1.7.6/ambr/models/artifact.py
+-rw-r--r--   0        0        0     1658 2024-05-27 07:30:34.845818 ambr_py-1.7.6/ambr/models/book.py
+-rw-r--r--   0        0        0      820 2024-05-27 07:30:34.845818 ambr_py-1.7.6/ambr/models/changelog.py
+-rw-r--r--   0        0        0     8659 2024-05-27 07:30:34.846819 ambr_py-1.7.6/ambr/models/character.py
+-rw-r--r--   0        0        0     2590 2024-05-27 07:30:34.847212 ambr_py-1.7.6/ambr/models/character_fetter.py
+-rw-r--r--   0        0        0     1299 2024-05-27 07:30:34.847212 ambr_py-1.7.6/ambr/models/domain.py
+-rw-r--r--   0        0        0     2994 2024-05-27 07:30:34.847829 ambr_py-1.7.6/ambr/models/food.py
+-rw-r--r--   0        0        0     5057 2024-05-27 07:30:34.847829 ambr_py-1.7.6/ambr/models/furniture.py
+-rw-r--r--   0        0        0     3050 2024-05-27 07:30:34.847829 ambr_py-1.7.6/ambr/models/material.py
+-rw-r--r--   0        0        0     2406 2024-05-27 07:30:34.849084 ambr_py-1.7.6/ambr/models/monster.py
+-rw-r--r--   0        0        0     1683 2024-05-27 07:30:34.849084 ambr_py-1.7.6/ambr/models/name_card.py
+-rw-r--r--   0        0        0     1221 2024-05-27 07:30:34.849084 ambr_py-1.7.6/ambr/models/quest.py
+-rw-r--r--   0        0        0     5209 2024-05-27 07:30:34.850096 ambr_py-1.7.6/ambr/models/tcg.py
+-rw-r--r--   0        0        0      996 2024-05-27 07:30:34.850096 ambr_py-1.7.6/ambr/models/upgrade.py
+-rw-r--r--   0        0        0     4270 2024-05-27 07:31:17.609192 ambr_py-1.7.6/ambr/models/weapon.py
+-rw-r--r--   0        0        0     4833 2024-05-27 07:24:22.832360 ambr_py-1.7.6/ambr/utils.py
+-rw-r--r--   0        0        0    35803 2024-01-15 00:08:53.036002 ambr_py-1.7.6/LICENSE
+-rw-r--r--   0        0        0      839 2024-05-27 07:33:10.563862 ambr_py-1.7.6/pyproject.toml
+-rw-r--r--   0        0        0     2097 2024-05-27 07:23:30.207490 ambr_py-1.7.6/README.md
+-rw-r--r--   0        0        0     2650 1970-01-01 00:00:00.000000 ambr_py-1.7.6/PKG-INFO
```

### Comparing `ambr_py-1.7.5/ambr/client.py` & `ambr_py-1.7.6/ambr/client.py`

 * *Files identical despite different names*

### Comparing `ambr_py-1.7.5/ambr/exceptions.py` & `ambr_py-1.7.6/ambr/exceptions.py`

 * *Files identical despite different names*

### Comparing `ambr_py-1.7.5/ambr/models/abyss.py` & `ambr_py-1.7.6/ambr/models/abyss.py`

 * *Files identical despite different names*

### Comparing `ambr_py-1.7.5/ambr/models/achievement.py` & `ambr_py-1.7.6/ambr/models/achievement.py`

 * *Files identical despite different names*

### Comparing `ambr_py-1.7.5/ambr/models/artifact.py` & `ambr_py-1.7.6/ambr/models/artifact.py`

 * *Files identical despite different names*

### Comparing `ambr_py-1.7.5/ambr/models/book.py` & `ambr_py-1.7.6/ambr/models/book.py`

 * *Files identical despite different names*

### Comparing `ambr_py-1.7.5/ambr/models/changelog.py` & `ambr_py-1.7.6/ambr/models/changelog.py`

 * *Files identical despite different names*

### Comparing `ambr_py-1.7.5/ambr/models/character.py` & `ambr_py-1.7.6/ambr/models/character.py`

 * *Files identical despite different names*

### Comparing `ambr_py-1.7.5/ambr/models/character_fetter.py` & `ambr_py-1.7.6/ambr/models/character_fetter.py`

 * *Files identical despite different names*

### Comparing `ambr_py-1.7.5/ambr/models/domain.py` & `ambr_py-1.7.6/ambr/models/domain.py`

 * *Files identical despite different names*

### Comparing `ambr_py-1.7.5/ambr/models/food.py` & `ambr_py-1.7.6/ambr/models/food.py`

 * *Files identical despite different names*

### Comparing `ambr_py-1.7.5/ambr/models/furniture.py` & `ambr_py-1.7.6/ambr/models/furniture.py`

 * *Files identical despite different names*

### Comparing `ambr_py-1.7.5/ambr/models/material.py` & `ambr_py-1.7.6/ambr/models/material.py`

 * *Files identical despite different names*

### Comparing `ambr_py-1.7.5/ambr/models/monster.py` & `ambr_py-1.7.6/ambr/models/monster.py`

 * *Files identical despite different names*

### Comparing `ambr_py-1.7.5/ambr/models/name_card.py` & `ambr_py-1.7.6/ambr/models/name_card.py`

 * *Files identical despite different names*

### Comparing `ambr_py-1.7.5/ambr/models/quest.py` & `ambr_py-1.7.6/ambr/models/quest.py`

 * *Files identical despite different names*

### Comparing `ambr_py-1.7.5/ambr/models/tcg.py` & `ambr_py-1.7.6/ambr/models/tcg.py`

 * *Files identical despite different names*

### Comparing `ambr_py-1.7.5/ambr/models/upgrade.py` & `ambr_py-1.7.6/ambr/models/upgrade.py`

 * *Files identical despite different names*

### Comparing `ambr_py-1.7.5/ambr/models/weapon.py` & `ambr_py-1.7.6/ambr/models/weapon.py`

 * *Files identical despite different names*

### Comparing `ambr_py-1.7.5/LICENSE` & `ambr_py-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ambr_py-1.7.5/README.md` & `ambr_py-1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `ambr_py-1.7.5/PKG-INFO` & `ambr_py-1.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambr-py
-Version: 1.7.5
+Version: 1.7.6
 Summary: API wrapper for ambr.top written in Python
 License: GPL-3.0
 Author: seriaati
 Author-email: seria.ati@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

