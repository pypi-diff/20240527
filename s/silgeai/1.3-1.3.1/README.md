# Comparing `tmp/silgeai-1.3.tar.gz` & `tmp/silgeai-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silgeai-1.3.tar", last modified: Wed May 15 10:22:10 2024, max compression
+gzip compressed data, was "silgeai-1.3.1.tar", last modified: Sun May 26 23:42:47 2024, max compression
```

## Comparing `silgeai-1.3.tar` & `silgeai-1.3.1.tar`

### file list

```diff
@@ -1,16 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 10:22:10.915184 silgeai-1.3/
--rw-rw-rw-   0        0        0     1088 2024-05-15 08:19:43.000000 silgeai-1.3/LICENSE
--rw-rw-rw-   0        0        0      332 2024-05-15 10:22:10.904841 silgeai-1.3/PKG-INFO
--rw-rw-rw-   0        0        0       43 2024-05-15 10:16:06.000000 silgeai-1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-15 10:22:10.915184 silgeai-1.3/setup.cfg
--rw-rw-rw-   0        0        0      783 2024-05-15 10:21:54.000000 silgeai-1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:22:10.898841 silgeai-1.3/silgeai/
--rw-rw-rw-   0        0        0      130 2024-05-15 10:16:06.000000 silgeai-1.3/silgeai/__init__.py
--rw-rw-rw-   0        0        0      257 2024-05-15 08:24:53.000000 silgeai-1.3/silgeai/demo.py
--rw-rw-rw-   0        0        0     1291 2024-05-15 08:10:33.000000 silgeai-1.3/silgeai/dictPrint.py
--rw-rw-rw-   0        0        0     2274 2024-05-15 10:21:08.000000 silgeai-1.3/silgeai/folderAnalysis.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:22:10.903851 silgeai-1.3/silgeai.egg-info/
--rw-rw-rw-   0        0        0      332 2024-05-15 10:22:10.000000 silgeai-1.3/silgeai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2024-05-15 10:22:10.000000 silgeai-1.3/silgeai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 10:22:10.000000 silgeai-1.3/silgeai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-15 10:22:10.000000 silgeai-1.3/silgeai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 23:42:47.416352 silgeai-1.3.1/
+-rw-rw-rw-   0        0        0     1088 2024-05-15 08:19:43.000000 silgeai-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0      355 2024-05-26 23:42:47.405993 silgeai-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2024-05-15 10:16:06.000000 silgeai-1.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 23:42:47.416352 silgeai-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      785 2024-05-26 23:42:02.000000 silgeai-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 23:42:47.398997 silgeai-1.3.1/silgeai/
+-rw-rw-rw-   0        0        0      161 2024-05-26 23:29:12.000000 silgeai-1.3.1/silgeai/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 23:42:47.404993 silgeai-1.3.1/silgeai/api/
+-rw-rw-rw-   0        0        0      140 2024-05-26 22:45:15.000000 silgeai-1.3.1/silgeai/api/__init__.py
+-rw-rw-rw-   0        0        0    14203 2024-05-26 23:41:34.000000 silgeai-1.3.1/silgeai/api/asrapi.py
+-rw-rw-rw-   0        0        0      785 2024-05-26 23:41:34.000000 silgeai-1.3.1/silgeai/api/getauth.py
+-rw-rw-rw-   0        0        0      293 2024-05-26 23:32:01.000000 silgeai-1.3.1/silgeai/api/test.py
+-rw-rw-rw-   0        0        0      257 2024-05-15 08:24:53.000000 silgeai-1.3.1/silgeai/demo.py
+-rw-rw-rw-   0        0        0     1291 2024-05-15 08:10:33.000000 silgeai-1.3.1/silgeai/dictPrint.py
+-rw-rw-rw-   0        0        0     2274 2024-05-15 10:21:08.000000 silgeai-1.3.1/silgeai/folderAnalysis.py
+-rw-rw-rw-   0        0        0      309 2024-05-26 23:39:40.000000 silgeai-1.3.1/silgeai/test.py
+drwxrwxrwx   0        0        0        0 2024-05-26 23:42:47.401994 silgeai-1.3.1/silgeai.egg-info/
+-rw-rw-rw-   0        0        0      355 2024-05-26 23:42:47.000000 silgeai-1.3.1/silgeai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2024-05-26 23:42:47.000000 silgeai-1.3.1/silgeai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 23:42:47.000000 silgeai-1.3.1/silgeai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 23:42:47.000000 silgeai-1.3.1/silgeai.egg-info/top_level.txt
```

### Comparing `silgeai-1.3/LICENSE` & `silgeai-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `silgeai-1.3/setup.py` & `silgeai-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 @Date: 2024/5/15 16:15
 @Describe: 
 """
 from setuptools import setup, find_packages
 
 setup(
     name='silgeai',
-    version='1.3',
+    version='1.3.1',
     packages=find_packages(),
     description='洞墟科技有限公司AI产品SDK',
   #  long_description=open('README.md').read(),
     # python3，readme文件中文报错
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='http://github.com/yourusername/my_package',
```

### Comparing `silgeai-1.3/silgeai/dictPrint.py` & `silgeai-1.3.1/silgeai/dictPrint.py`

 * *Files identical despite different names*

### Comparing `silgeai-1.3/silgeai/folderAnalysis.py` & `silgeai-1.3.1/silgeai/folderAnalysis.py`

 * *Files identical despite different names*

