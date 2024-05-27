# Comparing `tmp/dicio_py-1.4.tar.gz` & `tmp/dicio_py-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicio_py-1.4.tar", last modified: Mon May 27 12:17:12 2024, max compression
+gzip compressed data, was "dicio_py-1.5.tar", last modified: Mon May 27 12:26:02 2024, max compression
```

## Comparing `dicio_py-1.4.tar` & `dicio_py-1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 12:17:12.289124 dicio_py-1.4/
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)    35149 2024-05-26 14:04:54.000000 dicio_py-1.4/LICENSE
--rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1619 2024-05-27 12:17:12.289124 dicio_py-1.4/PKG-INFO
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1236 2024-05-26 14:43:55.000000 dicio_py-1.4/README.md
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 12:17:12.281124 dicio_py-1.4/dicio_my/
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        0 2024-05-26 14:28:37.000000 dicio_py-1.4/dicio_my/__init__.py
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     4044 2024-05-27 12:13:57.000000 dicio_py-1.4/dicio_my/__main__.py
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 12:17:12.289124 dicio_py-1.4/dicio_py.egg-info/
--rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1619 2024-05-27 12:17:12.000000 dicio_py-1.4/dicio_py.egg-info/PKG-INFO
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      231 2024-05-27 12:17:12.000000 dicio_py-1.4/dicio_py.egg-info/SOURCES.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        1 2024-05-27 12:17:12.000000 dicio_py-1.4/dicio_py.egg-info/dependency_links.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       43 2024-05-27 12:17:12.000000 dicio_py-1.4/dicio_py.egg-info/entry_points.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        9 2024-05-27 12:17:12.000000 dicio_py-1.4/dicio_py.egg-info/top_level.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       38 2024-05-27 12:17:12.289124 dicio_py-1.4/setup.cfg
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      738 2024-05-27 12:15:45.000000 dicio_py-1.4/setup.py
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 12:26:02.297423 dicio_py-1.5/
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)    35149 2024-05-26 14:04:54.000000 dicio_py-1.5/LICENSE
+-rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 12:26:02.297423 dicio_py-1.5/PKG-INFO
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1236 2024-05-26 14:43:55.000000 dicio_py-1.5/README.md
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 12:26:02.289424 dicio_py-1.5/dicio_my/
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        0 2024-05-26 14:28:37.000000 dicio_py-1.5/dicio_my/__init__.py
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     3317 2024-05-27 12:24:23.000000 dicio_py-1.5/dicio_my/__main__.py
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 12:26:02.297423 dicio_py-1.5/dicio_py.egg-info/
+-rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 12:26:02.000000 dicio_py-1.5/dicio_py.egg-info/PKG-INFO
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      231 2024-05-27 12:26:02.000000 dicio_py-1.5/dicio_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        1 2024-05-27 12:26:02.000000 dicio_py-1.5/dicio_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       52 2024-05-27 12:26:02.000000 dicio_py-1.5/dicio_py.egg-info/entry_points.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        9 2024-05-27 12:26:02.000000 dicio_py-1.5/dicio_py.egg-info/top_level.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       38 2024-05-27 12:26:02.297423 dicio_py-1.5/setup.cfg
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      760 2024-05-27 12:23:42.000000 dicio_py-1.5/setup.py
```

### Comparing `dicio_py-1.4/LICENSE` & `dicio_py-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dicio_py-1.4/PKG-INFO` & `dicio_py-1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: dicio-py
-Version: 1.4
+Version: 1.5
 Summary: Dicionário via CLI
 Home-page: https://github.com/Jetrom17/dicio-py
 Author: Jetrom17
 Author-email: Jeiel@duck.com
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dicio-py
```

### Comparing `dicio_py-1.4/README.md` & `dicio_py-1.5/README.md`

 * *Files identical despite different names*

### Comparing `dicio_py-1.4/dicio_my/__main__.py` & `dicio_py-1.5/dicio_my/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,9 @@
-# dicio_py/__main__.py
 #!/usr/bin/env python3
 
-"""
-Dicio-Py: Script para buscar o significado de palavras no dicionário online Dicio.
-Versão: 1.0
-Autor: Jeiel Lima Miranda.
-Data: 26 de maio de 2024
-Fork: https://github.com/ludovici-philippus/dicio-py
-
-Descrição:
-Este script recebe uma palavra como argumento de linha de comando e busca seu significado no site dicio.com.br.
-O significado é formatado e exibido no terminal com cores para facilitar a leitura.
-
-Uso:
-python3 -m dicio_py [PALAVRA]
-
-Dependências:
-- Nenhuma dependência externa necessária. O script utiliza apenas bibliotecas padrão do Python 3.
-"""
-
 import sys
 import re
 import os
 from unicodedata import normalize
 from urllib.request import urlopen
 
 BASE_URL = 'https://www.dicio.com.br/'
@@ -33,19 +14,18 @@
     'BLUE': "\033[1;34m",
     'MAGENTA': "\033[1;35m",
     'END': "\033[m",
     'ITALIC': '\033[3m'
 }
 
 def clear_terminal():
-    # Verifica o sistema operacional e executa o comando apropriado
     if os.name == 'nt':
-        os.system('cls')  # Comando para Windows
+        os.system('cls')
     else:
-        os.system('clear')  # Comando para Unix (Linux e macOS)
+        os.system('clear')
 
 def colorize(text, color):
     return f"{COLORS[color.upper()]}{text}{COLORS['END']}"
 
 def print_with_color(text: str, color: str):
     print(colorize(text, color))
```

### Comparing `dicio_py-1.4/dicio_py.egg-info/PKG-INFO` & `dicio_py-1.5/dicio_py.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: dicio-py
-Version: 1.4
+Version: 1.5
 Summary: Dicionário via CLI
 Home-page: https://github.com/Jetrom17/dicio-py
 Author: Jetrom17
 Author-email: Jeiel@duck.com
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dicio-py
```

### Comparing `dicio_py-1.4/setup.py` & `dicio_py-1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name="dicio-py",  # Replace with your own username
-    version="1.4",
+    name="dicio-py",
+    version="1.5",
     author="Jetrom17",
     author_email="Jeiel@duck.com",
     description="Dicionário via CLI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Jetrom17/dicio-py",
     packages=setuptools.find_packages(),
     classifiers=[
+        "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     entry_points={
         'console_scripts': [
-            'dicio-py=dicio_py:main',
+            'dicio-py=dicio_py.__main__:main',
         ],
     },
     python_requires='>=3.0',
 )
```

