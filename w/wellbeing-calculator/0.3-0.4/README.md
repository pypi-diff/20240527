# Comparing `tmp/wellbeing_calculator-0.3.tar.gz` & `tmp/wellbeing_calculator-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wellbeing_calculator-0.3.tar", last modified: Mon May 27 04:52:48 2024, max compression
+gzip compressed data, was "wellbeing_calculator-0.4.tar", last modified: Mon May 27 05:05:28 2024, max compression
```

## Comparing `wellbeing_calculator-0.3.tar` & `wellbeing_calculator-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mochidzukidaiki   (501) staff       (20)        0 2024-05-27 04:52:48.994932 wellbeing_calculator-0.3/
--rw-r--r--   0 mochidzukidaiki   (501) staff       (20)     2522 2024-05-27 04:52:48.994747 wellbeing_calculator-0.3/PKG-INFO
--rw-r--r--   0 mochidzukidaiki   (501) staff       (20)     1607 2024-05-27 04:29:35.000000 wellbeing_calculator-0.3/README.md
--rw-r--r--   0 mochidzukidaiki   (501) staff       (20)       38 2024-05-27 04:52:48.994975 wellbeing_calculator-0.3/setup.cfg
--rw-r--r--   0 mochidzukidaiki   (501) staff       (20)     1273 2024-05-27 04:52:13.000000 wellbeing_calculator-0.3/setup.py
-drwxr-xr-x   0 mochidzukidaiki   (501) staff       (20)        0 2024-05-27 04:52:48.993327 wellbeing_calculator-0.3/src/
-drwxr-xr-x   0 mochidzukidaiki   (501) staff       (20)        0 2024-05-27 04:52:48.993760 wellbeing_calculator-0.3/src/wellbeing_calculator/
--rw-r--r--   0 mochidzukidaiki   (501) staff       (20)        0 2024-05-25 07:46:53.000000 wellbeing_calculator-0.3/src/wellbeing_calculator/__init__.py
--rw-r--r--   0 mochidzukidaiki   (501) staff       (20)      846 2024-05-27 01:52:17.000000 wellbeing_calculator-0.3/src/wellbeing_calculator/calculator.py
-drwxr-xr-x   0 mochidzukidaiki   (501) staff       (20)        0 2024-05-27 04:52:48.994578 wellbeing_calculator-0.3/src/wellbeing_calculator.egg-info/
--rw-r--r--   0 mochidzukidaiki   (501) staff       (20)     2522 2024-05-27 04:52:48.000000 wellbeing_calculator-0.3/src/wellbeing_calculator.egg-info/PKG-INFO
--rw-r--r--   0 mochidzukidaiki   (501) staff       (20)      384 2024-05-27 04:52:48.000000 wellbeing_calculator-0.3/src/wellbeing_calculator.egg-info/SOURCES.txt
--rw-r--r--   0 mochidzukidaiki   (501) staff       (20)        1 2024-05-27 04:52:48.000000 wellbeing_calculator-0.3/src/wellbeing_calculator.egg-info/dependency_links.txt
--rw-r--r--   0 mochidzukidaiki   (501) staff       (20)       79 2024-05-27 04:52:48.000000 wellbeing_calculator-0.3/src/wellbeing_calculator.egg-info/entry_points.txt
--rw-r--r--   0 mochidzukidaiki   (501) staff       (20)        7 2024-05-27 04:52:48.000000 wellbeing_calculator-0.3/src/wellbeing_calculator.egg-info/requires.txt
--rw-r--r--   0 mochidzukidaiki   (501) staff       (20)       21 2024-05-27 04:52:48.000000 wellbeing_calculator-0.3/src/wellbeing_calculator.egg-info/top_level.txt
+drwxr-xr-x   0 mochidzukidaiki   (501) staff       (20)        0 2024-05-27 05:05:28.195792 wellbeing_calculator-0.4/
+-rw-r--r--   0 mochidzukidaiki   (501) staff       (20)     2738 2024-05-27 05:05:28.195634 wellbeing_calculator-0.4/PKG-INFO
+-rw-r--r--   0 mochidzukidaiki   (501) staff       (20)     1759 2024-05-27 05:02:31.000000 wellbeing_calculator-0.4/README.md
+-rw-r--r--   0 mochidzukidaiki   (501) staff       (20)       38 2024-05-27 05:05:28.195829 wellbeing_calculator-0.4/setup.cfg
+-rw-r--r--   0 mochidzukidaiki   (501) staff       (20)     1273 2024-05-27 05:05:15.000000 wellbeing_calculator-0.4/setup.py
+drwxr-xr-x   0 mochidzukidaiki   (501) staff       (20)        0 2024-05-27 05:05:28.194348 wellbeing_calculator-0.4/src/
+drwxr-xr-x   0 mochidzukidaiki   (501) staff       (20)        0 2024-05-27 05:05:28.194744 wellbeing_calculator-0.4/src/wellbeing_calculator/
+-rw-r--r--   0 mochidzukidaiki   (501) staff       (20)        0 2024-05-25 07:46:53.000000 wellbeing_calculator-0.4/src/wellbeing_calculator/__init__.py
+-rw-r--r--   0 mochidzukidaiki   (501) staff       (20)      846 2024-05-27 01:52:17.000000 wellbeing_calculator-0.4/src/wellbeing_calculator/calculator.py
+drwxr-xr-x   0 mochidzukidaiki   (501) staff       (20)        0 2024-05-27 05:05:28.195479 wellbeing_calculator-0.4/src/wellbeing_calculator.egg-info/
+-rw-r--r--   0 mochidzukidaiki   (501) staff       (20)     2738 2024-05-27 05:05:28.000000 wellbeing_calculator-0.4/src/wellbeing_calculator.egg-info/PKG-INFO
+-rw-r--r--   0 mochidzukidaiki   (501) staff       (20)      384 2024-05-27 05:05:28.000000 wellbeing_calculator-0.4/src/wellbeing_calculator.egg-info/SOURCES.txt
+-rw-r--r--   0 mochidzukidaiki   (501) staff       (20)        1 2024-05-27 05:05:28.000000 wellbeing_calculator-0.4/src/wellbeing_calculator.egg-info/dependency_links.txt
+-rw-r--r--   0 mochidzukidaiki   (501) staff       (20)       79 2024-05-27 05:05:28.000000 wellbeing_calculator-0.4/src/wellbeing_calculator.egg-info/entry_points.txt
+-rw-r--r--   0 mochidzukidaiki   (501) staff       (20)        7 2024-05-27 05:05:28.000000 wellbeing_calculator-0.4/src/wellbeing_calculator.egg-info/requires.txt
+-rw-r--r--   0 mochidzukidaiki   (501) staff       (20)       21 2024-05-27 05:05:28.000000 wellbeing_calculator-0.4/src/wellbeing_calculator.egg-info/top_level.txt
```

### Comparing `wellbeing_calculator-0.3/PKG-INFO` & `wellbeing_calculator-0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 Metadata-Version: 2.1
 Name: wellbeing_calculator
-Version: 0.3
+Version: 0.4
 Summary: A tool to evaluate the impact of social media usage on personal wellbeing and lifestyle habits
 Home-page: https://github.com/yourusername/wellbeing_calculator
 Author: Your Name
 Author-email: your-email@example.com
 License: MIT
-Description: # Wellbeing Calculator
+Description: 
+        # Wellbeing Calculator
         
         This tool evaluates the impact of social media usage on personal wellbeing and lifestyle habits. It uses data such as social media usage time, sleep time, exercise time, and stress levels to calculate a wellbeing score for each individual.
         
         ## Installation
         
+        You can install the Wellbeing Calculator via pip:
         
-        ### 2. `setup.py`ファイルの更新
-        次に、`setup.py`ファイルを更新して、`README.md`の内容を`long_description`として設定します。
+        ```bash
+        pip install wellbeing_calculator
+        
+        
+        ### `setup.py` ファイルの内容
+        `setup.py`ファイルも確認のために再掲します。
         
-        #### `setup.py`
         ```python
+        # -*- coding: utf-8 -*-
         from setuptools import setup, find_packages
-        import pathlib
+        import os
         
         # プロジェクトのルートディレクトリを取得
-        HERE = pathlib.Path(__file__).parent
+        HERE = os.path.abspath(os.path.dirname(__file__))
         
         # README.mdの内容を読み込む
-        long_description = (HERE / "README.md").read_text()
+        with open(os.path.join(HERE, "README.md"), encoding="utf-8") as f:
+            long_description = f.read()
         
         setup(
             name='wellbeing_calculator',
-            version='0.1',
+            version='0.3',  # バージョン番号を更新
             packages=find_packages(where='src'),
             package_dir={'': 'src'},
             install_requires=[
                 'pandas',
             ],
             entry_points={
                 'console_scripts': [
@@ -48,14 +55,15 @@
             url='https://github.com/yourusername/wellbeing_calculator',  # プロジェクトのリポジトリURL
             classifiers=[
                 'Programming Language :: Python :: 3',
                 'License :: OSI Approved :: MIT License',
                 'Operating System :: OS Independent',
             ],
             python_requires='>=3.6',
+            license='MIT',
         )
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `wellbeing_calculator-0.3/README.md` & `wellbeing_calculator-0.4/src/wellbeing_calculator.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,70 @@
-# Wellbeing Calculator
-
-This tool evaluates the impact of social media usage on personal wellbeing and lifestyle habits. It uses data such as social media usage time, sleep time, exercise time, and stress levels to calculate a wellbeing score for each individual.
-
-## Installation
-
-
-### 2. `setup.py`ファイルの更新
-次に、`setup.py`ファイルを更新して、`README.md`の内容を`long_description`として設定します。
-
-#### `setup.py`
-```python
-from setuptools import setup, find_packages
-import pathlib
-
-# プロジェクトのルートディレクトリを取得
-HERE = pathlib.Path(__file__).parent
-
-# README.mdの内容を読み込む
-long_description = (HERE / "README.md").read_text()
-
-setup(
-    name='wellbeing_calculator',
-    version='0.1',
-    packages=find_packages(where='src'),
-    package_dir={'': 'src'},
-    install_requires=[
-        'pandas',
-    ],
-    entry_points={
-        'console_scripts': [
-            'wellbeing_calculator=wellbeing_calculator.calculator:main',
-        ],
-    },
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    author='Your Name',
-    author_email='your-email@example.com',
-    description='A tool to evaluate the impact of social media usage on personal wellbeing and lifestyle habits',
-    url='https://github.com/yourusername/wellbeing_calculator',  # プロジェクトのリポジトリURL
-    classifiers=[
-        'Programming Language :: Python :: 3',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-    ],
-    python_requires='>=3.6',
-)
+Metadata-Version: 2.1
+Name: wellbeing-calculator
+Version: 0.4
+Summary: A tool to evaluate the impact of social media usage on personal wellbeing and lifestyle habits
+Home-page: https://github.com/yourusername/wellbeing_calculator
+Author: Your Name
+Author-email: your-email@example.com
+License: MIT
+Description: 
+        # Wellbeing Calculator
+        
+        This tool evaluates the impact of social media usage on personal wellbeing and lifestyle habits. It uses data such as social media usage time, sleep time, exercise time, and stress levels to calculate a wellbeing score for each individual.
+        
+        ## Installation
+        
+        You can install the Wellbeing Calculator via pip:
+        
+        ```bash
+        pip install wellbeing_calculator
+        
+        
+        ### `setup.py` ファイルの内容
+        `setup.py`ファイルも確認のために再掲します。
+        
+        ```python
+        # -*- coding: utf-8 -*-
+        from setuptools import setup, find_packages
+        import os
+        
+        # プロジェクトのルートディレクトリを取得
+        HERE = os.path.abspath(os.path.dirname(__file__))
+        
+        # README.mdの内容を読み込む
+        with open(os.path.join(HERE, "README.md"), encoding="utf-8") as f:
+            long_description = f.read()
+        
+        setup(
+            name='wellbeing_calculator',
+            version='0.3',  # バージョン番号を更新
+            packages=find_packages(where='src'),
+            package_dir={'': 'src'},
+            install_requires=[
+                'pandas',
+            ],
+            entry_points={
+                'console_scripts': [
+                    'wellbeing_calculator=wellbeing_calculator.calculator:main',
+                ],
+            },
+            long_description=long_description,
+            long_description_content_type='text/markdown',
+            author='Your Name',
+            author_email='your-email@example.com',
+            description='A tool to evaluate the impact of social media usage on personal wellbeing and lifestyle habits',
+            url='https://github.com/yourusername/wellbeing_calculator',  # プロジェクトのリポジトリURL
+            classifiers=[
+                'Programming Language :: Python :: 3',
+                'License :: OSI Approved :: MIT License',
+                'Operating System :: OS Independent',
+            ],
+            python_requires='>=3.6',
+            license='MIT',
+        )
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
```

### Comparing `wellbeing_calculator-0.3/setup.py` & `wellbeing_calculator-0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # README.mdの内容を読み込む
 with open(os.path.join(HERE, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='wellbeing_calculator',
-    version='0.3',  # バージョン番号を更新
+    version='0.4',  # バージョン番号を更新
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[
         'pandas',
     ],
     entry_points={
         'console_scripts': [
```

### Comparing `wellbeing_calculator-0.3/src/wellbeing_calculator/calculator.py` & `wellbeing_calculator-0.4/src/wellbeing_calculator/calculator.py`

 * *Files identical despite different names*

