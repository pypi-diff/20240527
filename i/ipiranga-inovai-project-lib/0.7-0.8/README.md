# Comparing `tmp/ipiranga-inovai-project-lib-0.7.tar.gz` & `tmp/ipiranga-inovai-project-lib-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipiranga-inovai-project-lib-0.7.tar", last modified: Wed May 22 17:59:32 2024, max compression
+gzip compressed data, was "ipiranga-inovai-project-lib-0.8.tar", last modified: Mon May 27 20:48:56 2024, max compression
```

## Comparing `ipiranga-inovai-project-lib-0.7.tar` & `ipiranga-inovai-project-lib-0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 17:59:32.204436 ipiranga-inovai-project-lib-0.7/
--rw-rw-rw-   0        0        0      198 2024-04-05 19:57:15.000000 ipiranga-inovai-project-lib-0.7/LICENSE
--rw-rw-rw-   0        0        0      516 2024-05-22 17:59:32.202439 ipiranga-inovai-project-lib-0.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-05 19:18:28.000000 ipiranga-inovai-project-lib-0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 17:59:32.186511 ipiranga-inovai-project-lib-0.7/inovai/
--rw-rw-rw-   0        0        0        0 2024-04-05 20:33:51.000000 ipiranga-inovai-project-lib-0.7/inovai/__init__.py
--rw-rw-rw-   0        0        0    12749 2024-05-22 17:57:29.000000 ipiranga-inovai-project-lib-0.7/inovai/entities.py
--rw-rw-rw-   0        0        0      847 2024-05-22 17:58:20.000000 ipiranga-inovai-project-lib-0.7/inovai/enums.py
-drwxrwxrwx   0        0        0        0 2024-05-22 17:59:32.200231 ipiranga-inovai-project-lib-0.7/ipiranga_inovai_project_lib.egg-info/
--rw-rw-rw-   0        0        0      516 2024-05-22 17:59:32.000000 ipiranga-inovai-project-lib-0.7/ipiranga_inovai_project_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2024-05-22 17:59:32.000000 ipiranga-inovai-project-lib-0.7/ipiranga_inovai_project_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 17:59:32.000000 ipiranga-inovai-project-lib-0.7/ipiranga_inovai_project_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-22 17:59:32.000000 ipiranga-inovai-project-lib-0.7/ipiranga_inovai_project_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 17:59:32.205599 ipiranga-inovai-project-lib-0.7/setup.cfg
--rw-rw-rw-   0        0        0      689 2024-05-22 17:59:20.000000 ipiranga-inovai-project-lib-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:48:56.166191 ipiranga-inovai-project-lib-0.8/
+-rw-rw-rw-   0        0        0      198 2024-04-05 19:57:15.000000 ipiranga-inovai-project-lib-0.8/LICENSE
+-rw-rw-rw-   0        0        0      516 2024-05-27 20:48:56.163037 ipiranga-inovai-project-lib-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-05 19:18:28.000000 ipiranga-inovai-project-lib-0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 20:48:56.143769 ipiranga-inovai-project-lib-0.8/inovai/
+-rw-rw-rw-   0        0        0        0 2024-04-05 20:33:51.000000 ipiranga-inovai-project-lib-0.8/inovai/__init__.py
+-rw-rw-rw-   0        0        0    12749 2024-05-22 17:57:29.000000 ipiranga-inovai-project-lib-0.8/inovai/entities.py
+-rw-rw-rw-   0        0        0      887 2024-05-27 20:47:20.000000 ipiranga-inovai-project-lib-0.8/inovai/enums.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:48:56.160578 ipiranga-inovai-project-lib-0.8/ipiranga_inovai_project_lib.egg-info/
+-rw-rw-rw-   0        0        0      516 2024-05-27 20:48:56.000000 ipiranga-inovai-project-lib-0.8/ipiranga_inovai_project_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2024-05-27 20:48:56.000000 ipiranga-inovai-project-lib-0.8/ipiranga_inovai_project_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 20:48:56.000000 ipiranga-inovai-project-lib-0.8/ipiranga_inovai_project_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-27 20:48:56.000000 ipiranga-inovai-project-lib-0.8/ipiranga_inovai_project_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 20:48:56.167242 ipiranga-inovai-project-lib-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      689 2024-05-27 20:48:40.000000 ipiranga-inovai-project-lib-0.8/setup.py
```

### Comparing `ipiranga-inovai-project-lib-0.7/PKG-INFO` & `ipiranga-inovai-project-lib-0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipiranga-inovai-project-lib
-Version: 0.7
+Version: 0.8
 Summary: Projeto criado para importação genérica de entidades
 Home-page: https://gitlab.ipirangacloud.com/clayton.monteiro.ext/ipiranga-inovai-project-lib
 Author: Clayton Sandes Monteiro
 Author-email: clayton.monteiro.ext@ipiranga.ipiranga
 License: MIT
 Keywords: inovai
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ipiranga-inovai-project-lib-0.7/inovai/entities.py` & `ipiranga-inovai-project-lib-0.8/inovai/entities.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-0.7/inovai/enums.py` & `ipiranga-inovai-project-lib-0.8/inovai/enums.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from enum import Enum
 
 
 class DocumentStatus(Enum):
     INTEGRATED = 'INTEGRADO'
     PENDING_INTEGRATION = 'PENDENTE_INTEGRACAO'
+    CONVERTER_ERROR = 'ERRO_CONVERSAO'
 
 
 class DocumentMovementType(Enum):
     INPUT = 'E',
     OUTPUT = 'S'
```

### Comparing `ipiranga-inovai-project-lib-0.7/ipiranga_inovai_project_lib.egg-info/PKG-INFO` & `ipiranga-inovai-project-lib-0.8/ipiranga_inovai_project_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipiranga-inovai-project-lib
-Version: 0.7
+Version: 0.8
 Summary: Projeto criado para importação genérica de entidades
 Home-page: https://gitlab.ipirangacloud.com/clayton.monteiro.ext/ipiranga-inovai-project-lib
 Author: Clayton Sandes Monteiro
 Author-email: clayton.monteiro.ext@ipiranga.ipiranga
 License: MIT
 Keywords: inovai
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ipiranga-inovai-project-lib-0.7/setup.py` & `ipiranga-inovai-project-lib-0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ipiranga-inovai-project-lib",
-    version="0.7",
+    version="0.8",
     packages=find_packages(),
     description="Projeto criado para importação genérica de entidades",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author="Clayton Sandes Monteiro",
     author_email="clayton.monteiro.ext@ipiranga.ipiranga",
     url="https://gitlab.ipirangacloud.com/clayton.monteiro.ext/ipiranga-inovai-project-lib",
```

