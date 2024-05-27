# Comparing `tmp/OpenDocument-0.1.tar.gz` & `tmp/opendocument-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenDocument-0.1.tar", last modified: Mon May 27 12:26:01 2024, max compression
+gzip compressed data, was "dist\opendocument-0.1.2.tar", last modified: Mon May 27 13:14:36 2024, max compression
```

## Comparing `OpenDocument-0.1.tar` & `opendocument-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 12:26:01.559650 OpenDocument-0.1/
-drwxrwxrwx   0        0        0        0 2024-05-27 12:26:01.422472 OpenDocument-0.1/OpenDocument/
--rw-rw-rw-   0        0        0      136 2024-05-27 12:00:01.000000 OpenDocument-0.1/OpenDocument/__init__.py
--rw-rw-rw-   0        0        0     2496 2024-05-27 11:55:47.000000 OpenDocument-0.1/OpenDocument/preprocessing.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:26:01.456466 OpenDocument-0.1/OpenDocument.egg-info/
--rw-rw-rw-   0        0        0      145 2024-05-27 12:26:01.000000 OpenDocument-0.1/OpenDocument.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2024-05-27 12:26:01.000000 OpenDocument-0.1/OpenDocument.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 12:26:01.000000 OpenDocument-0.1/OpenDocument.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-05-27 12:26:01.000000 OpenDocument-0.1/OpenDocument.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-27 12:26:01.000000 OpenDocument-0.1/OpenDocument.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      145 2024-05-27 12:26:01.557691 OpenDocument-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1974 2024-05-27 11:46:00.000000 OpenDocument-0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-27 12:26:01.560222 OpenDocument-0.1/setup.cfg
--rw-rw-rw-   0        0        0      455 2024-05-27 12:21:00.000000 OpenDocument-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:14:36.949806 opendocument-0.1.2/
+drwxrwxrwx   0        0        0        0 2024-05-27 13:14:36.851905 opendocument-0.1.2/OpenDocument/
+-rw-rw-rw-   0        0        0      136 2024-05-27 13:12:06.000000 opendocument-0.1.2/OpenDocument/__init__.py
+-rw-rw-rw-   0        0        0     2496 2024-05-27 12:50:30.000000 opendocument-0.1.2/OpenDocument/preprocessing.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:14:36.943870 opendocument-0.1.2/OpenDocument.egg-info/
+-rw-rw-rw-   0        0        0      214 2024-05-27 13:14:36.000000 opendocument-0.1.2/OpenDocument.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2024-05-27 13:14:36.000000 opendocument-0.1.2/OpenDocument.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 13:14:36.000000 opendocument-0.1.2/OpenDocument.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2024-05-27 13:14:36.000000 opendocument-0.1.2/OpenDocument.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-27 13:14:36.000000 opendocument-0.1.2/OpenDocument.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      214 2024-05-27 13:14:36.946808 opendocument-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1974 2024-05-27 11:46:00.000000 opendocument-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-27 13:14:36.950264 opendocument-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      503 2024-05-27 13:14:22.000000 opendocument-0.1.2/setup.py
```

### Comparing `OpenDocument-0.1/OpenDocument/preprocessing.py` & `opendocument-0.1.2/OpenDocument/preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     assert isinstance(window_size, int) and window_size > 0, "Window size must be a positive integer."
     
     thresh_sauvolavalue = threshold_sauvola(grayImage_, window_size=window_size)
     thresholdImage_ = (grayImage_ > thresh_sauvolavalue)
     
     return thresholdImage_
 
-def remove_Lines(binaryImage_, horz_size=12, vert_size=15):
+def remove_lines(binaryImage_, horz_size=12, vert_size=15):
     """
     Removing the horizontal and vertical lines in the image.
     
     binaryImage_ --- Image should be in binary format.
     horz_size -- It represents the Minimum size of horizontal line need to be removed from the image.
     vert_size -- It represents the Minimum size of vertical line need to be removed from the image.
     """
```

### Comparing `OpenDocument-0.1/README.md` & `opendocument-0.1.2/README.md`

 * *Files identical despite different names*

