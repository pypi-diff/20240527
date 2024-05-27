# Comparing `tmp/movoid_config-1.2.2.tar.gz` & `tmp/movoid_config-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_config-1.2.2.tar", last modified: Thu May  9 13:04:03 2024, max compression
+gzip compressed data, was "movoid_config-1.2.3.tar", last modified: Mon May 27 03:15:26 2024, max compression
```

## Comparing `movoid_config-1.2.2.tar` & `movoid_config-1.2.3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 13:04:03.723173 movoid_config-1.2.2/
--rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_config-1.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2330 2024-05-09 13:04:03.714546 movoid_config-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2163 2024-01-08 15:32:17.000000 movoid_config-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 13:04:03.706133 movoid_config-1.2.2/movoid_config/
--rw-rw-rw-   0        0        0      243 2024-05-09 13:02:56.000000 movoid_config-1.2.2/movoid_config/__init__.py
--rw-rw-rw-   0        0        0    20705 2024-05-09 13:02:56.000000 movoid_config-1.2.2/movoid_config/config.py
--rw-rw-rw-   0        0        0     1477 2024-05-09 13:02:56.000000 movoid_config-1.2.2/movoid_config/loop_run.py
-drwxrwxrwx   0        0        0        0 2024-05-09 13:04:03.713511 movoid_config-1.2.2/movoid_config.egg-info/
--rw-rw-rw-   0        0        0     2330 2024-05-09 13:04:03.000000 movoid_config-1.2.2/movoid_config.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-05-09 13:04:03.000000 movoid_config-1.2.2/movoid_config.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 13:04:03.000000 movoid_config-1.2.2/movoid_config.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-09 13:04:03.000000 movoid_config-1.2.2/movoid_config.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 13:04:03.724193 movoid_config-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      460 2024-05-09 13:03:26.000000 movoid_config-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 03:15:26.659194 movoid_config-1.2.3/
+-rw-rw-rw-   0        0        0     2330 2024-05-27 03:15:26.656203 movoid_config-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2163 2024-03-05 06:42:09.000000 movoid_config-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 03:15:26.637266 movoid_config-1.2.3/movoid_config/
+-rw-rw-rw-   0        0        0      243 2024-03-05 07:28:09.000000 movoid_config-1.2.3/movoid_config/__init__.py
+-rw-rw-rw-   0        0        0    20862 2024-05-24 06:45:56.000000 movoid_config-1.2.3/movoid_config/config.py
+-rw-rw-rw-   0        0        0     1477 2024-05-09 03:25:35.000000 movoid_config-1.2.3/movoid_config/loop_run.py
+drwxrwxrwx   0        0        0        0 2024-05-27 03:15:26.654210 movoid_config-1.2.3/movoid_config.egg-info/
+-rw-rw-rw-   0        0        0     2330 2024-05-27 03:15:26.000000 movoid_config-1.2.3/movoid_config.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-05-27 03:15:26.000000 movoid_config-1.2.3/movoid_config.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 03:15:26.000000 movoid_config-1.2.3/movoid_config.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-27 03:15:26.000000 movoid_config-1.2.3/movoid_config.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 03:15:26.659194 movoid_config-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      460 2024-05-27 03:15:00.000000 movoid_config-1.2.3/setup.py
```

### Comparing `movoid_config-1.2.2/PKG-INFO` & `movoid_config-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: movoid_config
-Version: 1.2.2
+Version: 1.2.3
 Home-page: 
 Author: movoid
 Author-email: bobrobotsun@163.com
 Description-Content-Type: text/markdown
 
 This is a simple program for developer to create a param-config reader.
 It only need config_dict and config_file_name to analyse all param and config
```

### Comparing `movoid_config-1.2.2/README.md` & `movoid_config-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `movoid_config-1.2.2/movoid_config/config.py` & `movoid_config-1.2.3/movoid_config/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,22 @@
         self.__config_file = _file
         self.__config_key = None
         self.__value = {}
         self.__tk = None
         if _dict is not None:
             self.init(_dict, _file)
 
+    @property
+    def file(self):
+        return self.__config_file
+
+    @file.setter
+    def file(self, value):
+        self.__config_file = value
+
     def __getitem__(self, item):
         return self.__value[item]
 
     def __setitem__(self, item, value):
         self.__value[item] = value
 
     def __getattr__(self, item):
```

### Comparing `movoid_config-1.2.2/movoid_config/loop_run.py` & `movoid_config-1.2.3/movoid_config/loop_run.py`

 * *Files identical despite different names*

### Comparing `movoid_config-1.2.2/movoid_config.egg-info/PKG-INFO` & `movoid_config-1.2.3/movoid_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: movoid_config
-Version: 1.2.2
+Version: 1.2.3
 Home-page: 
 Author: movoid
 Author-email: bobrobotsun@163.com
 Description-Content-Type: text/markdown
 
 This is a simple program for developer to create a param-config reader.
 It only need config_dict and config_file_name to analyse all param and config
```

