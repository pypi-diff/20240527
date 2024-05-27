# Comparing `tmp/track2p-0.5.6.tar.gz` & `tmp/track2p-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "track2p-0.5.6.tar", last modified: Mon May 27 14:24:20 2024, max compression
+gzip compressed data, was "track2p-0.5.7.tar", last modified: Mon May 27 15:08:08 2024, max compression
```

## Comparing `track2p-0.5.6.tar` & `track2p-0.5.7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-27 14:24:20.926358 track2p-0.5.6/
--rw-r--r--   0 manonmantez   (501) staff       (20)    35149 2024-02-12 15:58:33.000000 track2p-0.5.6/LICENSE
--rw-r--r--   0 manonmantez   (501) staff       (20)     5281 2024-05-27 14:24:20.926149 track2p-0.5.6/PKG-INFO
--rw-r--r--   0 manonmantez   (501) staff       (20)     4862 2024-05-27 11:38:23.000000 track2p-0.5.6/README.md
--rw-r--r--   0 manonmantez   (501) staff       (20)       38 2024-05-27 14:24:20.926400 track2p-0.5.6/setup.cfg
--rw-r--r--   0 manonmantez   (501) staff       (20)      583 2024-05-27 14:24:02.000000 track2p-0.5.6/setup.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-27 14:24:20.918291 track2p-0.5.6/track2p/
--rw-r--r--   0 manonmantez   (501) staff       (20)       48 2024-02-22 09:56:18.000000 track2p-0.5.6/track2p/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      376 2024-05-27 11:38:23.000000 track2p-0.5.6/track2p/__main__.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-27 14:24:20.921452 track2p-0.5.6/track2p/gui/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.6/track2p/gui/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     8045 2024-05-27 11:38:23.000000 track2p-0.5.6/track2p/gui/cell_plot.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     7779 2024-05-27 14:18:01.000000 track2p-0.5.6/track2p/gui/central_widget.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     6646 2024-05-27 14:17:46.000000 track2p-0.5.6/track2p/gui/data_management.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     6538 2024-05-27 11:38:23.000000 track2p-0.5.6/track2p/gui/fluo_plot.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1825 2024-05-27 11:38:23.000000 track2p-0.5.6/track2p/gui/import_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     2026 2024-05-27 11:38:23.000000 track2p-0.5.6/track2p/gui/main_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    15563 2024-05-27 11:38:23.000000 track2p-0.5.6/track2p/gui/raster_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     8677 2024-05-23 17:37:24.000000 track2p-0.5.6/track2p/gui/roi_plot.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     3679 2024-05-27 13:24:03.000000 track2p-0.5.6/track2p/gui/statusbar.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     8166 2024-05-27 11:38:23.000000 track2p-0.5.6/track2p/gui/t2p_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1570 2024-05-27 11:38:23.000000 track2p-0.5.6/track2p/gui/toolbar.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      815 2024-05-27 11:38:23.000000 track2p-0.5.6/track2p/gui/window_manager.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-27 14:24:20.922800 track2p-0.5.6/track2p/io/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.6/track2p/io/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1726 2024-04-26 14:30:23.000000 track2p-0.5.6/track2p/io/loaders.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     4238 2024-04-16 14:56:02.000000 track2p-0.5.6/track2p/io/s2p_loaders.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      773 2024-02-12 11:04:52.000000 track2p-0.5.6/track2p/io/savers.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      252 2024-01-09 12:56:24.000000 track2p-0.5.6/track2p/io/utils.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-27 14:24:20.923514 track2p-0.5.6/track2p/match/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.6/track2p/match/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     4471 2024-01-09 12:56:24.000000 track2p-0.5.6/track2p/match/loop.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     5807 2024-04-16 14:56:02.000000 track2p-0.5.6/track2p/match/utils.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-27 14:24:20.923879 track2p-0.5.6/track2p/ops/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.6/track2p/ops/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     3307 2024-05-27 14:18:04.000000 track2p-0.5.6/track2p/ops/default.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-27 14:24:20.924696 track2p-0.5.6/track2p/plot/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.6/track2p/plot/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    15443 2024-04-16 14:56:02.000000 track2p-0.5.6/track2p/plot/output.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      914 2024-05-07 11:31:47.000000 track2p-0.5.6/track2p/plot/progress.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1859 2024-05-07 12:40:06.000000 track2p-0.5.6/track2p/plot/utils.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-27 14:24:20.925652 track2p-0.5.6/track2p/register/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.6/track2p/register/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1348 2024-01-10 11:16:47.000000 track2p-0.5.6/track2p/register/elastix.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     4054 2024-01-09 12:56:24.000000 track2p-0.5.6/track2p/register/loop.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     2345 2024-05-07 11:31:47.000000 track2p-0.5.6/track2p/register/utils.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    10608 2024-05-27 11:38:23.000000 track2p-0.5.6/track2p/t2p.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-27 14:24:20.925912 track2p-0.5.6/track2p.egg-info/
--rw-r--r--   0 manonmantez   (501) staff       (20)     5281 2024-05-27 14:24:20.000000 track2p-0.5.6/track2p.egg-info/PKG-INFO
--rw-r--r--   0 manonmantez   (501) staff       (20)     1000 2024-05-27 14:24:20.000000 track2p-0.5.6/track2p.egg-info/SOURCES.txt
--rw-r--r--   0 manonmantez   (501) staff       (20)        1 2024-05-27 14:24:20.000000 track2p-0.5.6/track2p.egg-info/dependency_links.txt
--rw-r--r--   0 manonmantez   (501) staff       (20)      155 2024-05-27 14:24:20.000000 track2p-0.5.6/track2p.egg-info/requires.txt
--rw-r--r--   0 manonmantez   (501) staff       (20)        8 2024-05-27 14:24:20.000000 track2p-0.5.6/track2p.egg-info/top_level.txt
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-27 15:08:08.950394 track2p-0.5.7/
+-rw-r--r--   0 manonmantez   (501) staff       (20)    35149 2024-02-12 15:58:33.000000 track2p-0.5.7/LICENSE
+-rw-r--r--   0 manonmantez   (501) staff       (20)     5281 2024-05-27 15:08:08.950039 track2p-0.5.7/PKG-INFO
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4862 2024-05-27 11:38:23.000000 track2p-0.5.7/README.md
+-rw-r--r--   0 manonmantez   (501) staff       (20)       38 2024-05-27 15:08:08.950465 track2p-0.5.7/setup.cfg
+-rw-r--r--   0 manonmantez   (501) staff       (20)      583 2024-05-27 15:07:43.000000 track2p-0.5.7/setup.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-27 15:08:08.941305 track2p-0.5.7/track2p/
+-rw-r--r--   0 manonmantez   (501) staff       (20)       48 2024-02-22 09:56:18.000000 track2p-0.5.7/track2p/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      376 2024-05-27 11:38:23.000000 track2p-0.5.7/track2p/__main__.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-27 15:08:08.946184 track2p-0.5.7/track2p/gui/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.7/track2p/gui/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     8045 2024-05-27 11:38:23.000000 track2p-0.5.7/track2p/gui/cell_plot.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     7779 2024-05-27 14:18:01.000000 track2p-0.5.7/track2p/gui/central_widget.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     6646 2024-05-27 14:17:46.000000 track2p-0.5.7/track2p/gui/data_management.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     6538 2024-05-27 11:38:23.000000 track2p-0.5.7/track2p/gui/fluo_plot.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1825 2024-05-27 11:38:23.000000 track2p-0.5.7/track2p/gui/import_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     2026 2024-05-27 11:38:23.000000 track2p-0.5.7/track2p/gui/main_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    15559 2024-05-27 15:03:32.000000 track2p-0.5.7/track2p/gui/raster_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     8677 2024-05-23 17:37:24.000000 track2p-0.5.7/track2p/gui/roi_plot.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     3679 2024-05-27 13:24:03.000000 track2p-0.5.7/track2p/gui/statusbar.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     8166 2024-05-27 11:38:23.000000 track2p-0.5.7/track2p/gui/t2p_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1570 2024-05-27 11:38:23.000000 track2p-0.5.7/track2p/gui/toolbar.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      815 2024-05-27 11:38:23.000000 track2p-0.5.7/track2p/gui/window_manager.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-27 15:08:08.947089 track2p-0.5.7/track2p/io/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.7/track2p/io/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1726 2024-04-26 14:30:23.000000 track2p-0.5.7/track2p/io/loaders.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4238 2024-04-16 14:56:02.000000 track2p-0.5.7/track2p/io/s2p_loaders.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      773 2024-02-12 11:04:52.000000 track2p-0.5.7/track2p/io/savers.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      252 2024-01-09 12:56:24.000000 track2p-0.5.7/track2p/io/utils.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-27 15:08:08.947607 track2p-0.5.7/track2p/match/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.7/track2p/match/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4471 2024-01-09 12:56:24.000000 track2p-0.5.7/track2p/match/loop.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     5807 2024-04-16 14:56:02.000000 track2p-0.5.7/track2p/match/utils.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-27 15:08:08.947933 track2p-0.5.7/track2p/ops/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.7/track2p/ops/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     3307 2024-05-27 14:18:04.000000 track2p-0.5.7/track2p/ops/default.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-27 15:08:08.948742 track2p-0.5.7/track2p/plot/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.7/track2p/plot/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    15443 2024-04-16 14:56:02.000000 track2p-0.5.7/track2p/plot/output.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      914 2024-05-07 11:31:47.000000 track2p-0.5.7/track2p/plot/progress.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1859 2024-05-07 12:40:06.000000 track2p-0.5.7/track2p/plot/utils.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-27 15:08:08.949428 track2p-0.5.7/track2p/register/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.7/track2p/register/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1348 2024-01-10 11:16:47.000000 track2p-0.5.7/track2p/register/elastix.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4054 2024-01-09 12:56:24.000000 track2p-0.5.7/track2p/register/loop.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     2345 2024-05-07 11:31:47.000000 track2p-0.5.7/track2p/register/utils.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    10679 2024-05-27 15:03:33.000000 track2p-0.5.7/track2p/t2p.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-27 15:08:08.949670 track2p-0.5.7/track2p.egg-info/
+-rw-r--r--   0 manonmantez   (501) staff       (20)     5281 2024-05-27 15:08:08.000000 track2p-0.5.7/track2p.egg-info/PKG-INFO
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1000 2024-05-27 15:08:08.000000 track2p-0.5.7/track2p.egg-info/SOURCES.txt
+-rw-r--r--   0 manonmantez   (501) staff       (20)        1 2024-05-27 15:08:08.000000 track2p-0.5.7/track2p.egg-info/dependency_links.txt
+-rw-r--r--   0 manonmantez   (501) staff       (20)      155 2024-05-27 15:08:08.000000 track2p-0.5.7/track2p.egg-info/requires.txt
+-rw-r--r--   0 manonmantez   (501) staff       (20)        8 2024-05-27 15:08:08.000000 track2p-0.5.7/track2p.egg-info/top_level.txt
```

### Comparing `track2p-0.5.6/LICENSE` & `track2p-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/PKG-INFO` & `track2p-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: track2p
-Version: 0.5.6
+Version: 0.5.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.23.5
 Requires-Dist: matplotlib==3.5.3
 Requires-Dist: scikit-image==0.20.0
 Requires-Dist: itk==5.4rc2
 Requires-Dist: PyQt5==5.15.10
```

### Comparing `track2p-0.5.6/README.md` & `track2p-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/setup.py` & `track2p-0.5.7/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='track2p',
-    version='0.5.6',
+    version='0.5.7',
     packages=find_packages(),
     install_requires=[
         'numpy==1.23.5',
         'matplotlib==3.5.3',
         'scikit-image==0.20.0',
         'itk==5.4rc2',
         'PyQt5==5.15.10',
```

### Comparing `track2p-0.5.6/track2p/gui/cell_plot.py` & `track2p-0.5.7/track2p/gui/cell_plot.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/track2p/gui/central_widget.py` & `track2p-0.5.7/track2p/gui/central_widget.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/track2p/gui/data_management.py` & `track2p-0.5.7/track2p/gui/data_management.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/track2p/gui/fluo_plot.py` & `track2p-0.5.7/track2p/gui/fluo_plot.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/track2p/gui/import_wd.py` & `track2p-0.5.7/track2p/gui/import_wd.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/track2p/gui/main_wd.py` & `track2p-0.5.7/track2p/gui/main_wd.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/track2p/gui/raster_wd.py` & `track2p-0.5.7/track2p/gui/raster_wd.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,15 +278,15 @@
                 ax[i].set_yticks([0, f.shape[0]-1])
                 ax[i].set_yticklabels([0, f.shape[0]])
                 # move the text of the yticklabels a bit: the first one down and the last one up
                 ax[i].set_yticklabels(ax[i].get_yticklabels(), rotation=0, va='center', ha='right')
         
                 # only first and last xticks on y axis in minutes
                 if i == len(all_f_t2p)-1:
-                    ax[i].set_xlabel('Time (min)')
+                    ax[i].set_xlabel('Frames')
                     ax[i].set_xticks([0, f.shape[1]/2, f.shape[1]-1])
                     ax[i].set_xticklabels([0, int((f.shape[1]*bin_size)/2), int(f.shape[1]*bin_size)])
             
                 else:
                     ax[i].set_xticks([])
                     ax[i].set_xticklabels([])
```

### Comparing `track2p-0.5.6/track2p/gui/roi_plot.py` & `track2p-0.5.7/track2p/gui/roi_plot.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/track2p/gui/statusbar.py` & `track2p-0.5.7/track2p/gui/statusbar.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/track2p/gui/t2p_wd.py` & `track2p-0.5.7/track2p/gui/t2p_wd.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/track2p/gui/toolbar.py` & `track2p-0.5.7/track2p/gui/toolbar.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/track2p/gui/window_manager.py` & `track2p-0.5.7/track2p/gui/window_manager.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/track2p/io/loaders.py` & `track2p-0.5.7/track2p/io/loaders.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/track2p/io/s2p_loaders.py` & `track2p-0.5.7/track2p/io/s2p_loaders.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/track2p/io/savers.py` & `track2p-0.5.7/track2p/io/savers.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/track2p/match/loop.py` & `track2p-0.5.7/track2p/match/loop.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/track2p/match/utils.py` & `track2p-0.5.7/track2p/match/utils.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/track2p/ops/default.py` & `track2p-0.5.7/track2p/ops/default.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/track2p/plot/output.py` & `track2p-0.5.7/track2p/plot/output.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/track2p/plot/progress.py` & `track2p-0.5.7/track2p/plot/progress.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/track2p/plot/utils.py` & `track2p-0.5.7/track2p/plot/utils.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/track2p/register/elastix.py` & `track2p-0.5.7/track2p/register/elastix.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/track2p/register/loop.py` & `track2p-0.5.7/track2p/register/loop.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/track2p/register/utils.py` & `track2p-0.5.7/track2p/register/utils.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.6/track2p/t2p.py` & `track2p-0.5.7/track2p/t2p.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,26 +96,29 @@
         print(f'Found {n_planes} planes in {ds_path}')
 
     folderpath=track_ops.save_path
     track_ops_dict = np.load(os.path.join(folderpath,  "track_ops.npy"), allow_pickle=True).item()
     track_ops = SimpleNamespace(**track_ops_dict)
     iscell_thr = track_ops.iscell_thr
 
-    all_f_t2p= []
-    all_ops = []
-    all_stat_t2p = []
-    all_iscell_t2p = []
-    fneu_iscell_t2p= []
-    spks_iscell_t2p= []
-    
-    fneu_chan2_iscell_t2p = []
-    f_chan2_iscell_t2p = []
-    redcell_iscell_t2p = []
 
     for j in range(track_ops.nplanes):
+        
+        all_f_t2p= []
+        all_ops = []
+        all_stat_t2p = []
+        all_iscell_t2p = []
+        fneu_iscell_t2p= []
+        spks_iscell_t2p= []
+        
+        fneu_chan2_iscell_t2p = []
+        f_chan2_iscell_t2p = []
+        redcell_iscell_t2p = []
+            
+        
         print(f'nplanes{j}')
         t2p_match_mat = np.load(os.path.join(folderpath,f'plane{str(j)}_match_mat.npy'), allow_pickle=True)
         t2p_match_mat_allday = t2p_match_mat[~np.any(t2p_match_mat == None, axis=1), :]
         for (i, ds_path) in enumerate(track_ops.all_ds_path):
                     ops = np.load(os.path.join(ds_path, 'suite2p', f'plane{str(j)}', 'ops.npy'), allow_pickle=True).item()
                     stat = np.load(os.path.join(ds_path, 'suite2p', f'plane{str(j)}', 'stat.npy'), allow_pickle=True)
                     f = np.load(os.path.join(ds_path, 'suite2p', f'plane{str(j)}', 'F.npy'), allow_pickle=True)
```

### Comparing `track2p-0.5.6/track2p.egg-info/PKG-INFO` & `track2p-0.5.7/track2p.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: track2p
-Version: 0.5.6
+Version: 0.5.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.23.5
 Requires-Dist: matplotlib==3.5.3
 Requires-Dist: scikit-image==0.20.0
 Requires-Dist: itk==5.4rc2
 Requires-Dist: PyQt5==5.15.10
```

### Comparing `track2p-0.5.6/track2p.egg-info/SOURCES.txt` & `track2p-0.5.7/track2p.egg-info/SOURCES.txt`

 * *Files identical despite different names*

