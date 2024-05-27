# Comparing `tmp/pyexmars-1.0.2.tar.gz` & `tmp/pyexmars-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyexmars-1.0.2.tar", last modified: Mon May 27 08:48:55 2024, max compression
+gzip compressed data, was "pyexmars-1.0.3.tar", last modified: Mon May 27 08:59:09 2024, max compression
```

## Comparing `pyexmars-1.0.2.tar` & `pyexmars-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 08:48:55.627059 pyexmars-1.0.2/
--rw-rw-rw-   0        0        0       55 2024-05-27 08:48:55.626060 pyexmars-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-27 08:48:55.594231 pyexmars-1.0.2/pyexmars/
--rw-rw-rw-   0        0        0        0 2024-05-27 08:43:52.000000 pyexmars-1.0.2/pyexmars/__init__.py
--rw-rw-rw-   0        0        0      683 2024-05-10 06:20:11.000000 pyexmars-1.0.2/pyexmars/pyexmars.py
-drwxrwxrwx   0        0        0        0 2024-05-27 08:48:55.624044 pyexmars-1.0.2/pyexmars.egg-info/
--rw-rw-rw-   0        0        0       55 2024-05-27 08:48:55.000000 pyexmars-1.0.2/pyexmars.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2024-05-27 08:48:55.000000 pyexmars-1.0.2/pyexmars.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 08:48:55.000000 pyexmars-1.0.2/pyexmars.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-27 08:48:55.000000 pyexmars-1.0.2/pyexmars.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 08:48:55.627059 pyexmars-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      261 2024-05-27 08:44:32.000000 pyexmars-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 08:59:09.348026 pyexmars-1.0.3/
+-rw-rw-rw-   0        0        0       55 2024-05-27 08:59:09.347030 pyexmars-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-27 08:59:09.316024 pyexmars-1.0.3/pyexmars/
+-rw-rw-rw-   0        0        0        0 2024-05-27 08:43:52.000000 pyexmars-1.0.3/pyexmars/__init__.py
+-rw-rw-rw-   0        0        0      683 2024-05-27 08:57:25.000000 pyexmars-1.0.3/pyexmars/pyexmars.py
+drwxrwxrwx   0        0        0        0 2024-05-27 08:59:09.345018 pyexmars-1.0.3/pyexmars.egg-info/
+-rw-rw-rw-   0        0        0       55 2024-05-27 08:59:09.000000 pyexmars-1.0.3/pyexmars.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2024-05-27 08:59:09.000000 pyexmars-1.0.3/pyexmars.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 08:59:09.000000 pyexmars-1.0.3/pyexmars.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-27 08:59:09.000000 pyexmars-1.0.3/pyexmars.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 08:59:09.348026 pyexmars-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      261 2024-05-27 08:58:57.000000 pyexmars-1.0.3/setup.py
```

### Comparing `pyexmars-1.0.2/pyexmars/pyexmars.py` & `pyexmars-1.0.3/pyexmars/pyexmars.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-class Protocal():
+class Protocol():
     def __init__(self):
         self.buffers = []
         for i in range(11):
             self.buffers.append(0)
 
     def makePacket(self, index, para1, para2, para3, para4):
         self.buffers[0] = 0
```

