# Comparing `tmp/silgeai-1.3.1.tar.gz` & `tmp/silgeai-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silgeai-1.3.1.tar", last modified: Sun May 26 23:42:47 2024, max compression
+gzip compressed data, was "silgeai-1.3.2.tar", last modified: Sun May 26 23:51:33 2024, max compression
```

## Comparing `silgeai-1.3.1.tar` & `silgeai-1.3.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 23:42:47.416352 silgeai-1.3.1/
--rw-rw-rw-   0        0        0     1088 2024-05-15 08:19:43.000000 silgeai-1.3.1/LICENSE
--rw-rw-rw-   0        0        0      355 2024-05-26 23:42:47.405993 silgeai-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0       43 2024-05-15 10:16:06.000000 silgeai-1.3.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 23:42:47.416352 silgeai-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      785 2024-05-26 23:42:02.000000 silgeai-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 23:42:47.398997 silgeai-1.3.1/silgeai/
--rw-rw-rw-   0        0        0      161 2024-05-26 23:29:12.000000 silgeai-1.3.1/silgeai/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 23:42:47.404993 silgeai-1.3.1/silgeai/api/
--rw-rw-rw-   0        0        0      140 2024-05-26 22:45:15.000000 silgeai-1.3.1/silgeai/api/__init__.py
--rw-rw-rw-   0        0        0    14203 2024-05-26 23:41:34.000000 silgeai-1.3.1/silgeai/api/asrapi.py
--rw-rw-rw-   0        0        0      785 2024-05-26 23:41:34.000000 silgeai-1.3.1/silgeai/api/getauth.py
--rw-rw-rw-   0        0        0      293 2024-05-26 23:32:01.000000 silgeai-1.3.1/silgeai/api/test.py
--rw-rw-rw-   0        0        0      257 2024-05-15 08:24:53.000000 silgeai-1.3.1/silgeai/demo.py
--rw-rw-rw-   0        0        0     1291 2024-05-15 08:10:33.000000 silgeai-1.3.1/silgeai/dictPrint.py
--rw-rw-rw-   0        0        0     2274 2024-05-15 10:21:08.000000 silgeai-1.3.1/silgeai/folderAnalysis.py
--rw-rw-rw-   0        0        0      309 2024-05-26 23:39:40.000000 silgeai-1.3.1/silgeai/test.py
-drwxrwxrwx   0        0        0        0 2024-05-26 23:42:47.401994 silgeai-1.3.1/silgeai.egg-info/
--rw-rw-rw-   0        0        0      355 2024-05-26 23:42:47.000000 silgeai-1.3.1/silgeai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2024-05-26 23:42:47.000000 silgeai-1.3.1/silgeai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 23:42:47.000000 silgeai-1.3.1/silgeai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 23:42:47.000000 silgeai-1.3.1/silgeai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 23:51:33.995266 silgeai-1.3.2/
+-rw-rw-rw-   0        0        0     1088 2024-05-15 08:19:43.000000 silgeai-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0      355 2024-05-26 23:51:33.994275 silgeai-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2024-05-15 10:16:06.000000 silgeai-1.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 23:51:33.995266 silgeai-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      821 2024-05-26 23:51:26.000000 silgeai-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 23:51:33.986268 silgeai-1.3.2/silgeai/
+-rw-rw-rw-   0        0        0      163 2024-05-26 23:51:26.000000 silgeai-1.3.2/silgeai/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 23:51:33.993265 silgeai-1.3.2/silgeai/api/
+-rw-rw-rw-   0        0        0      140 2024-05-26 22:45:15.000000 silgeai-1.3.2/silgeai/api/__init__.py
+-rw-rw-rw-   0        0        0    14203 2024-05-26 23:41:34.000000 silgeai-1.3.2/silgeai/api/asrapi.py
+-rw-rw-rw-   0        0        0      785 2024-05-26 23:41:34.000000 silgeai-1.3.2/silgeai/api/getauth.py
+-rw-rw-rw-   0        0        0      293 2024-05-26 23:32:01.000000 silgeai-1.3.2/silgeai/api/test.py
+-rw-rw-rw-   0        0        0      257 2024-05-15 08:24:53.000000 silgeai-1.3.2/silgeai/demo.py
+-rw-rw-rw-   0        0        0     1291 2024-05-15 08:10:33.000000 silgeai-1.3.2/silgeai/dictPrint.py
+-rw-rw-rw-   0        0        0     2274 2024-05-15 10:21:08.000000 silgeai-1.3.2/silgeai/folderAnalysis.py
+-rw-rw-rw-   0        0        0      309 2024-05-26 23:39:40.000000 silgeai-1.3.2/silgeai/test.py
+drwxrwxrwx   0        0        0        0 2024-05-26 23:51:33.990268 silgeai-1.3.2/silgeai.egg-info/
+-rw-rw-rw-   0        0        0      355 2024-05-26 23:51:33.000000 silgeai-1.3.2/silgeai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2024-05-26 23:51:33.000000 silgeai-1.3.2/silgeai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 23:51:33.000000 silgeai-1.3.2/silgeai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-26 23:51:33.000000 silgeai-1.3.2/silgeai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 23:51:33.000000 silgeai-1.3.2/silgeai.egg-info/top_level.txt
```

### Comparing `silgeai-1.3.1/LICENSE` & `silgeai-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `silgeai-1.3.1/setup.py` & `silgeai-1.3.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,25 +6,28 @@
 @Date: 2024/5/15 16:15
 @Describe: 
 """
 from setuptools import setup, find_packages
 
 setup(
     name='silgeai',
-    version='1.3.1',
+    version='1.3.2',
     packages=find_packages(),
     description='洞墟科技有限公司AI产品SDK',
   #  long_description=open('README.md').read(),
     # python3，readme文件中文报错
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='http://github.com/yourusername/my_package',
     author='WhiteCome',
     author_email='waitKey1@outlook.com',
     license='MIT',
     install_requires=[
         # 依赖列表
+        'websockets'
+'requests'
+
     ],
     classifiers=[
         # 分类信息
     ]
 )
```

### Comparing `silgeai-1.3.1/silgeai/api/asrapi.py` & `silgeai-1.3.2/silgeai/api/asrapi.py`

 * *Files identical despite different names*

### Comparing `silgeai-1.3.1/silgeai/api/getauth.py` & `silgeai-1.3.2/silgeai/api/getauth.py`

 * *Files identical despite different names*

### Comparing `silgeai-1.3.1/silgeai/dictPrint.py` & `silgeai-1.3.2/silgeai/dictPrint.py`

 * *Files identical despite different names*

### Comparing `silgeai-1.3.1/silgeai/folderAnalysis.py` & `silgeai-1.3.2/silgeai/folderAnalysis.py`

 * *Files identical despite different names*

