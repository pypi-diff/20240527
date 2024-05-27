# Comparing `tmp/donut_llm_tools-24.5.27.tar.gz` & `tmp/donut_llm_tools-24.5.27.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "donut_llm_tools-24.5.27.tar", last modified: Mon May 27 13:49:34 2024, max compression
+gzip compressed data, was "donut_llm_tools-24.5.27.2.tar", last modified: Mon May 27 14:09:53 2024, max compression
```

## Comparing `donut_llm_tools-24.5.27.tar` & `donut_llm_tools-24.5.27.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 13:49:34.556662 donut_llm_tools-24.5.27/
--rw-rw-rw-   0        0        0     1088 2024-05-27 13:43:12.000000 donut_llm_tools-24.5.27/LICENSE
--rw-rw-rw-   0        0        0     3691 2024-05-27 13:49:34.534272 donut_llm_tools-24.5.27/PKG-INFO
--rw-rw-rw-   0        0        0     1859 2024-05-27 13:31:42.000000 donut_llm_tools-24.5.27/README
--rw-rw-rw-   0        0        0      792 2024-05-27 13:43:23.000000 donut_llm_tools-24.5.27/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-27 13:49:34.556662 donut_llm_tools-24.5.27/setup.cfg
--rw-rw-rw-   0        0        0      361 2024-05-27 13:48:31.000000 donut_llm_tools-24.5.27/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-27 13:49:34.327437 donut_llm_tools-24.5.27/src/
-drwxrwxrwx   0        0        0        0 2024-05-27 13:49:34.532539 donut_llm_tools-24.5.27/src/Donut_LLM_Tools.egg-info/
--rw-rw-rw-   0        0        0     3691 2024-05-27 13:49:33.000000 donut_llm_tools-24.5.27/src/Donut_LLM_Tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2024-05-27 13:49:34.000000 donut_llm_tools-24.5.27/src/Donut_LLM_Tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 13:49:33.000000 donut_llm_tools-24.5.27/src/Donut_LLM_Tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-27 13:49:33.000000 donut_llm_tools-24.5.27/src/Donut_LLM_Tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2024-05-27 13:49:33.000000 donut_llm_tools-24.5.27/src/Donut_LLM_Tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-27 13:49:33.000000 donut_llm_tools-24.5.27/src/Donut_LLM_Tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3858 2024-05-27 13:01:04.000000 donut_llm_tools-24.5.27/src/donutllmtools.py
+drwxrwxrwx   0        0        0        0 2024-05-27 14:09:53.272962 donut_llm_tools-24.5.27.2/
+-rw-rw-rw-   0        0        0     1092 2024-05-27 14:06:29.000000 donut_llm_tools-24.5.27.2/LICENSE
+-rw-rw-rw-   0        0        0     3821 2024-05-27 14:09:53.271201 donut_llm_tools-24.5.27.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1980 2024-05-27 14:08:08.000000 donut_llm_tools-24.5.27.2/README
+-rw-rw-rw-   0        0        0      795 2024-05-27 14:06:38.000000 donut_llm_tools-24.5.27.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-27 14:09:53.274890 donut_llm_tools-24.5.27.2/setup.cfg
+-rw-rw-rw-   0        0        0      361 2024-05-27 13:48:31.000000 donut_llm_tools-24.5.27.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 14:09:53.217221 donut_llm_tools-24.5.27.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-27 14:09:53.269182 donut_llm_tools-24.5.27.2/src/Donut_LLM_Tools.egg-info/
+-rw-rw-rw-   0        0        0     3821 2024-05-27 14:09:53.000000 donut_llm_tools-24.5.27.2/src/Donut_LLM_Tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2024-05-27 14:09:53.000000 donut_llm_tools-24.5.27.2/src/Donut_LLM_Tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 14:09:53.000000 donut_llm_tools-24.5.27.2/src/Donut_LLM_Tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-27 14:09:53.000000 donut_llm_tools-24.5.27.2/src/Donut_LLM_Tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2024-05-27 14:09:53.000000 donut_llm_tools-24.5.27.2/src/Donut_LLM_Tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-27 14:09:53.000000 donut_llm_tools-24.5.27.2/src/Donut_LLM_Tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3868 2024-05-27 14:07:27.000000 donut_llm_tools-24.5.27.2/src/donutllmtools.py
```

### Comparing `donut_llm_tools-24.5.27/LICENSE` & `donut_llm_tools-24.5.27.2/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) [year] [fullname]
+Copyright (c) [2024] [Gautham Nair]
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `donut_llm_tools-24.5.27/PKG-INFO` & `donut_llm_tools-24.5.27.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: Donut-LLM-Tools
-Version: 24.5.27
+Version: 24.5.27.2
 Summary: Tools for Creating Datasets and Models locally
 Author-email: Gautham Nair <gautham.nair.2005@gmail.com>
 License: MIT License
         
-        Copyright (c) [year] [fullname]
+        Copyright (c) [2024] [Gautham Nair]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -25,24 +25,24 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/gauthamnair2005/donut-llm-tools
 Keywords: feed,reader,tutorial
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: CreateLLM
 Requires-Dist: Wikipedia
 
 # Donut LLM Tools
 Donut LLM Tools is a suite of two programs that helps you create dataset from wikipedia data and your own LLM with the created or already existing dataset.
 
-*Latest Version 24.05.27*
+*Latest Version 24.05.27 Update 2*
 
 ## How to install, import and use DonutLLM?
 ### Installation
 * Before installing Donut LLM Tools, make sure you have Python `3.9` or later till Python `3.11`. *Note : Python `3.12` is not supported by PyTorch, hence Donut LLM Tools will also have troubles running.* 
 * The dependencies for installing Donut LLM Tools are:
     1. CreateLLM (`pip install CreateLLM`)
     2. torch (Required by CreateLLM)
@@ -74,7 +74,8 @@
 
 HelpAndInfo.create_llm() # Also create LLM from HelpAndInfo class.
 
 HelpAndInfo.create_dataset() # ALso create dataset from HelpAndInfo class.
 
 HelpAndInfo.main() # To get a menu based interface for dataset creation or model load/creation.
 ```
+The above code uses `HelpAndInfo` class which has the same functions from Tools class as well as help functions.
```

### Comparing `donut_llm_tools-24.5.27/README` & `donut_llm_tools-24.5.27.2/README`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Donut LLM Tools
 Donut LLM Tools is a suite of two programs that helps you create dataset from wikipedia data and your own LLM with the created or already existing dataset.
 
-*Latest Version 24.05.27*
+*Latest Version 24.05.27 Update 2*
 
 ## How to install, import and use DonutLLM?
 ### Installation
 * Before installing Donut LLM Tools, make sure you have Python `3.9` or later till Python `3.11`. *Note : Python `3.12` is not supported by PyTorch, hence Donut LLM Tools will also have troubles running.* 
 * The dependencies for installing Donut LLM Tools are:
     1. CreateLLM (`pip install CreateLLM`)
     2. torch (Required by CreateLLM)
@@ -37,7 +37,8 @@
 
 HelpAndInfo.create_llm() # Also create LLM from HelpAndInfo class.
 
 HelpAndInfo.create_dataset() # ALso create dataset from HelpAndInfo class.
 
 HelpAndInfo.main() # To get a menu based interface for dataset creation or model load/creation.
 ```
+The above code uses `HelpAndInfo` class which has the same functions from Tools class as well as help functions.
```

### Comparing `donut_llm_tools-24.5.27/pyproject.toml` & `donut_llm_tools-24.5.27.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Donut-LLM-Tools"
-version = "24.05.27"
+version = "24.05.27.2"
 description = "Tools for Creating Datasets and Models locally"
 readme = "README"
 authors = [{ name = "Gautham Nair", email = "gautham.nair.2005@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["feed", "reader", "tutorial"]
 dependencies = [
     "CreateLLM",
     "Wikipedia",
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.11"
 
 [project.urls]
 Homepage = "https://github.com/gauthamnair2005/donut-llm-tools"
 
 [project.scripts]
 donutllmtools = "donutllmtools"
```

### Comparing `donut_llm_tools-24.5.27/src/Donut_LLM_Tools.egg-info/PKG-INFO` & `donut_llm_tools-24.5.27.2/src/Donut_LLM_Tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: Donut-LLM-Tools
-Version: 24.5.27
+Version: 24.5.27.2
 Summary: Tools for Creating Datasets and Models locally
 Author-email: Gautham Nair <gautham.nair.2005@gmail.com>
 License: MIT License
         
-        Copyright (c) [year] [fullname]
+        Copyright (c) [2024] [Gautham Nair]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -25,24 +25,24 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/gauthamnair2005/donut-llm-tools
 Keywords: feed,reader,tutorial
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: CreateLLM
 Requires-Dist: Wikipedia
 
 # Donut LLM Tools
 Donut LLM Tools is a suite of two programs that helps you create dataset from wikipedia data and your own LLM with the created or already existing dataset.
 
-*Latest Version 24.05.27*
+*Latest Version 24.05.27 Update 2*
 
 ## How to install, import and use DonutLLM?
 ### Installation
 * Before installing Donut LLM Tools, make sure you have Python `3.9` or later till Python `3.11`. *Note : Python `3.12` is not supported by PyTorch, hence Donut LLM Tools will also have troubles running.* 
 * The dependencies for installing Donut LLM Tools are:
     1. CreateLLM (`pip install CreateLLM`)
     2. torch (Required by CreateLLM)
@@ -74,7 +74,8 @@
 
 HelpAndInfo.create_llm() # Also create LLM from HelpAndInfo class.
 
 HelpAndInfo.create_dataset() # ALso create dataset from HelpAndInfo class.
 
 HelpAndInfo.main() # To get a menu based interface for dataset creation or model load/creation.
 ```
+The above code uses `HelpAndInfo` class which has the same functions from Tools class as well as help functions.
```

### Comparing `donut_llm_tools-24.5.27/src/donutllmtools.py` & `donut_llm_tools-24.5.27.2/src/donutllmtools.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,16 +79,16 @@
         print("2. Create Dataset")
         print("3. Exit")
         print("4. Help")
         print("5. About")
 
     def about():
         print("DonutLLM Studio | AI/ML Model Trainer/Loader")
-        print("Version 1.0.0")
-        print("Developed by DonutAI")
+        print("Version 24.05.27.2")
+        print("Developed by Gautham Nair")
 
     def exit():
         print("Exiting DonutLLM Studio")
         exit()
 
     def main():
         while True:
```

