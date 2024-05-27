# Comparing `tmp/hema-0.0.5.tar.gz` & `tmp/hema-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hema-0.0.5.tar", last modified: Thu May 23 09:08:03 2024, max compression
+gzip compressed data, was "hema-0.0.6.tar", last modified: Mon May 27 09:25:22 2024, max compression
```

## Comparing `hema-0.0.5.tar` & `hema-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,31 @@
-drwxr-xr-x   0 qinhanhou   (501) staff       (20)        0 2024-05-23 09:08:03.147264 hema-0.0.5/
--rw-r--r--   0 qinhanhou   (501) staff       (20)      243 2024-05-23 09:08:03.146971 hema-0.0.5/PKG-INFO
-drwxr-xr-x   0 qinhanhou   (501) staff       (20)        0 2024-05-23 09:08:03.142434 hema-0.0.5/hema/
--rw-r--r--   0 qinhanhou   (501) staff       (20)        0 2024-05-23 08:53:50.000000 hema-0.0.5/hema/__init__.py
-drwxr-xr-x   0 qinhanhou   (501) staff       (20)        0 2024-05-23 09:08:03.143253 hema-0.0.5/hema/models/
--rw-r--r--   0 qinhanhou   (501) staff       (20)        0 2024-05-23 09:05:32.000000 hema-0.0.5/hema/models/__init__.py
-drwxr-xr-x   0 qinhanhou   (501) staff       (20)        0 2024-05-23 09:08:03.146304 hema-0.0.5/hema/models/conformer/
--rw-r--r--   0 qinhanhou   (501) staff       (20)        0 2024-05-23 09:01:30.000000 hema-0.0.5/hema/models/conformer/__init__.py
--rw-r--r--   0 qinhanhou   (501) staff       (20)      935 2024-05-21 10:37:02.000000 hema-0.0.5/hema/models/conformer/activation.py
--rw-r--r--   0 qinhanhou   (501) staff       (20)     5864 2024-05-21 17:22:09.000000 hema-0.0.5/hema/models/conformer/attention.py
--rw-r--r--   0 qinhanhou   (501) staff       (20)     1277 2024-05-21 17:23:23.000000 hema-0.0.5/hema/models/conformer/basic.py
--rw-r--r--   0 qinhanhou   (501) staff       (20)        0 2024-05-21 10:37:02.000000 hema-0.0.5/hema/models/conformer/conformer.py
--rw-r--r--   0 qinhanhou   (501) staff       (20)     4978 2024-05-21 10:37:02.000000 hema-0.0.5/hema/models/conformer/convolution.py
--rw-r--r--   0 qinhanhou   (501) staff       (20)     2008 2024-05-21 10:41:20.000000 hema-0.0.5/hema/models/conformer/embedding.py
--rw-r--r--   0 qinhanhou   (501) staff       (20)     8085 2024-05-21 17:22:49.000000 hema-0.0.5/hema/models/conformer/encoder.py
--rw-r--r--   0 qinhanhou   (501) staff       (20)     1458 2024-05-21 10:44:02.000000 hema-0.0.5/hema/models/conformer/feedforward.py
--rw-r--r--   0 qinhanhou   (501) staff       (20)     4168 2024-05-21 17:27:08.000000 hema-0.0.5/hema/models/conformer/model.py
-drwxr-xr-x   0 qinhanhou   (501) staff       (20)        0 2024-05-23 09:08:03.146696 hema-0.0.5/hema.egg-info/
--rw-r--r--   0 qinhanhou   (501) staff       (20)      243 2024-05-23 09:08:03.000000 hema-0.0.5/hema.egg-info/PKG-INFO
--rw-r--r--   0 qinhanhou   (501) staff       (20)      532 2024-05-23 09:08:03.000000 hema-0.0.5/hema.egg-info/SOURCES.txt
--rw-r--r--   0 qinhanhou   (501) staff       (20)        1 2024-05-23 09:08:03.000000 hema-0.0.5/hema.egg-info/dependency_links.txt
--rw-r--r--   0 qinhanhou   (501) staff       (20)       29 2024-05-23 09:08:03.000000 hema-0.0.5/hema.egg-info/requires.txt
--rw-r--r--   0 qinhanhou   (501) staff       (20)        5 2024-05-23 09:08:03.000000 hema-0.0.5/hema.egg-info/top_level.txt
--rw-r--r--   0 qinhanhou   (501) staff       (20)       38 2024-05-23 09:08:03.147314 hema-0.0.5/setup.cfg
--rw-r--r--   0 qinhanhou   (501) staff       (20)      414 2024-05-23 09:07:46.000000 hema-0.0.5/setup.py
+drwxr-xr-x   0 qinhan    (1000) qinhan    (1000)        0 2024-05-27 09:25:22.726335 hema-0.0.6/
+-rw-r--r--   0 qinhan    (1000) qinhan    (1000)      285 2024-05-27 09:25:22.726335 hema-0.0.6/PKG-INFO
+drwxr-xr-x   0 qinhan    (1000) qinhan    (1000)        0 2024-05-27 09:25:22.723002 hema-0.0.6/hema/
+-rw-r--r--   0 qinhan    (1000) qinhan    (1000)        0 2024-05-27 08:47:01.000000 hema-0.0.6/hema/__init__.py
+drwxr-xr-x   0 qinhan    (1000) qinhan    (1000)        0 2024-05-27 09:25:22.723002 hema-0.0.6/hema/models/
+-rw-r--r--   0 qinhan    (1000) qinhan    (1000)        0 2024-05-27 08:47:01.000000 hema-0.0.6/hema/models/__init__.py
+drwxr-xr-x   0 qinhan    (1000) qinhan    (1000)        0 2024-05-27 09:25:22.726335 hema-0.0.6/hema/models/conformer/
+-rw-r--r--   0 qinhan    (1000) qinhan    (1000)        0 2024-05-27 08:47:01.000000 hema-0.0.6/hema/models/conformer/__init__.py
+-rw-r--r--   0 qinhan    (1000) qinhan    (1000)      935 2024-05-27 08:47:01.000000 hema-0.0.6/hema/models/conformer/activation.py
+-rw-r--r--   0 qinhan    (1000) qinhan    (1000)     5864 2024-05-27 08:47:01.000000 hema-0.0.6/hema/models/conformer/attention.py
+-rw-r--r--   0 qinhan    (1000) qinhan    (1000)     1277 2024-05-27 08:47:01.000000 hema-0.0.6/hema/models/conformer/basic.py
+-rw-r--r--   0 qinhan    (1000) qinhan    (1000)        0 2024-05-27 08:47:01.000000 hema-0.0.6/hema/models/conformer/conformer.py
+-rw-r--r--   0 qinhan    (1000) qinhan    (1000)     4978 2024-05-27 08:47:01.000000 hema-0.0.6/hema/models/conformer/convolution.py
+-rw-r--r--   0 qinhan    (1000) qinhan    (1000)     2008 2024-05-27 08:47:01.000000 hema-0.0.6/hema/models/conformer/embedding.py
+-rw-r--r--   0 qinhan    (1000) qinhan    (1000)     8085 2024-05-27 08:47:01.000000 hema-0.0.6/hema/models/conformer/encoder.py
+-rw-r--r--   0 qinhan    (1000) qinhan    (1000)     1458 2024-05-27 08:47:01.000000 hema-0.0.6/hema/models/conformer/feedforward.py
+-rw-r--r--   0 qinhan    (1000) qinhan    (1000)     4168 2024-05-27 08:47:01.000000 hema-0.0.6/hema/models/conformer/model.py
+drwxr-xr-x   0 qinhan    (1000) qinhan    (1000)        0 2024-05-27 09:25:22.726335 hema-0.0.6/hema/nn/
+-rw-r--r--   0 qinhan    (1000) qinhan    (1000)        0 2024-05-27 08:51:40.000000 hema-0.0.6/hema/nn/__init__.py
+-rw-r--r--   0 qinhan    (1000) qinhan    (1000)     2136 2024-05-27 09:23:29.000000 hema-0.0.6/hema/nn/conv_blocks.py
+drwxr-xr-x   0 qinhan    (1000) qinhan    (1000)        0 2024-05-27 09:25:22.726335 hema-0.0.6/hema/visualization/
+-rw-r--r--   0 qinhan    (1000) qinhan    (1000)        0 2024-05-27 08:51:39.000000 hema-0.0.6/hema/visualization/__init__.py
+-rw-r--r--   0 qinhan    (1000) qinhan    (1000)      515 2024-05-27 09:16:51.000000 hema-0.0.6/hema/visualization/psd.py
+drwxr-xr-x   0 qinhan    (1000) qinhan    (1000)        0 2024-05-27 09:25:22.726335 hema-0.0.6/hema.egg-info/
+-rw-r--r--   0 qinhan    (1000) qinhan    (1000)      285 2024-05-27 09:25:22.000000 hema-0.0.6/hema.egg-info/PKG-INFO
+-rw-r--r--   0 qinhan    (1000) qinhan    (1000)      632 2024-05-27 09:25:22.000000 hema-0.0.6/hema.egg-info/SOURCES.txt
+-rw-r--r--   0 qinhan    (1000) qinhan    (1000)        1 2024-05-27 09:25:22.000000 hema-0.0.6/hema.egg-info/dependency_links.txt
+-rw-r--r--   0 qinhan    (1000) qinhan    (1000)       41 2024-05-27 09:25:22.000000 hema-0.0.6/hema.egg-info/requires.txt
+-rw-r--r--   0 qinhan    (1000) qinhan    (1000)        5 2024-05-27 09:25:22.000000 hema-0.0.6/hema.egg-info/top_level.txt
+-rw-r--r--   0 qinhan    (1000) qinhan    (1000)       38 2024-05-27 09:25:22.726335 hema-0.0.6/setup.cfg
+-rw-r--r--   0 qinhan    (1000) qinhan    (1000)      432 2024-05-27 09:24:14.000000 hema-0.0.6/setup.py
```

### Comparing `hema-0.0.5/hema/models/conformer/activation.py` & `hema-0.0.6/hema/models/conformer/activation.py`

 * *Files identical despite different names*

### Comparing `hema-0.0.5/hema/models/conformer/attention.py` & `hema-0.0.6/hema/models/conformer/attention.py`

 * *Files identical despite different names*

### Comparing `hema-0.0.5/hema/models/conformer/basic.py` & `hema-0.0.6/hema/models/conformer/basic.py`

 * *Files identical despite different names*

### Comparing `hema-0.0.5/hema/models/conformer/convolution.py` & `hema-0.0.6/hema/models/conformer/convolution.py`

 * *Files identical despite different names*

### Comparing `hema-0.0.5/hema/models/conformer/embedding.py` & `hema-0.0.6/hema/models/conformer/embedding.py`

 * *Files identical despite different names*

### Comparing `hema-0.0.5/hema/models/conformer/encoder.py` & `hema-0.0.6/hema/models/conformer/encoder.py`

 * *Files identical despite different names*

### Comparing `hema-0.0.5/hema/models/conformer/feedforward.py` & `hema-0.0.6/hema/models/conformer/feedforward.py`

 * *Files identical despite different names*

### Comparing `hema-0.0.5/hema/models/conformer/model.py` & `hema-0.0.6/hema/models/conformer/model.py`

 * *Files identical despite different names*

