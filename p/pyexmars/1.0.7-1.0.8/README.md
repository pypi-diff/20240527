# Comparing `tmp/pyexmars-1.0.7.tar.gz` & `tmp/pyexmars-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyexmars-1.0.7.tar", last modified: Mon May 27 09:30:00 2024, max compression
+gzip compressed data, was "pyexmars-1.0.8.tar", last modified: Mon May 27 10:55:10 2024, max compression
```

## Comparing `pyexmars-1.0.7.tar` & `pyexmars-1.0.8.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 09:30:00.601238 pyexmars-1.0.7/
--rw-rw-rw-   0        0        0       55 2024-05-27 09:30:00.601238 pyexmars-1.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-27 09:30:00.585137 pyexmars-1.0.7/pyexmars/
--rw-rw-rw-   0        0        0        0 2024-05-27 08:43:52.000000 pyexmars-1.0.7/pyexmars/__init__.py
--rw-rw-rw-   0        0        0     1006 2024-05-27 09:28:54.000000 pyexmars-1.0.7/pyexmars/pyexmars.cpython-310.pyc
--rw-rw-rw-   0        0        0      683 2024-05-27 09:27:47.000000 pyexmars-1.0.7/pyexmars/pyexmars.py
-drwxrwxrwx   0        0        0        0 2024-05-27 09:30:00.599729 pyexmars-1.0.7/pyexmars.egg-info/
--rw-rw-rw-   0        0        0       55 2024-05-27 09:30:00.000000 pyexmars-1.0.7/pyexmars.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-05-27 09:30:00.000000 pyexmars-1.0.7/pyexmars.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 09:30:00.000000 pyexmars-1.0.7/pyexmars.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-27 09:30:00.000000 pyexmars-1.0.7/pyexmars.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 09:30:00.601238 pyexmars-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      261 2024-05-27 09:29:54.000000 pyexmars-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:55:10.543564 pyexmars-1.0.8/
+-rw-rw-rw-   0        0        0       55 2024-05-27 10:55:10.542411 pyexmars-1.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-27 10:55:10.523420 pyexmars-1.0.8/pyexmars/
+-rw-rw-rw-   0        0        0        0 2024-05-27 08:43:52.000000 pyexmars-1.0.8/pyexmars/__init__.py
+-rw-rw-rw-   0        0        0      687 2024-05-27 10:51:19.000000 pyexmars-1.0.8/pyexmars/pyexmars.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:55:10.540228 pyexmars-1.0.8/pyexmars.egg-info/
+-rw-rw-rw-   0        0        0       55 2024-05-27 10:55:10.000000 pyexmars-1.0.8/pyexmars.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2024-05-27 10:55:10.000000 pyexmars-1.0.8/pyexmars.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 10:55:10.000000 pyexmars-1.0.8/pyexmars.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-27 10:55:10.000000 pyexmars-1.0.8/pyexmars.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 10:55:10.543564 pyexmars-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      260 2024-05-27 10:54:46.000000 pyexmars-1.0.8/setup.py
```

### Comparing `pyexmars-1.0.7/pyexmars/pyexmars.py` & `pyexmars-1.0.8/pyexmars/pyexmars.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-
-class Protocol():
+#pyexmars.py
+class Protocol:
     def __init__(self):
         self.buffers = []
         for i in range(11):
             self.buffers.append(0)
 
     def makePacket(self, index, para1, para2, para3, para4):
         self.buffers[0] = 0
@@ -17,8 +17,7 @@
         self.buffers[8] = 253
         self.buffers[9] = 254
         self.buffers[10] = 254
 
     def makePacketMenuSetting(self, main, sub):
         self.makePacket(0, 11, main, sub, 255)
         return self.buffers
-
```

