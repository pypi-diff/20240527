# Comparing `tmp/nutritious-0.1.0.tar.gz` & `tmp/nutritious-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutritious-0.1.0.tar", max compression
+gzip compressed data, was "nutritious-0.1.1.tar", max compression
```

## Comparing `nutritious-0.1.0.tar` & `nutritious-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2024-05-27 06:38:32.700508 nutritious-0.1.0/LICENSE
--rw-r--r--   0        0        0     3273 2024-05-27 06:38:32.700508 nutritious-0.1.0/README.md
--rw-r--r--   0        0        0    12746 2024-05-27 06:38:32.704508 nutritious-0.1.0/nutritious/__init__.py
--rw-r--r--   0        0        0     1442 2024-05-27 06:38:32.704508 nutritious-0.1.0/nutritious/__main__.py
--rw-r--r--   0        0        0     1434 2024-05-27 06:38:32.704508 nutritious-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4575 1970-01-01 00:00:00.000000 nutritious-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-27 07:13:34.063871 nutritious-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3100 2024-05-27 07:13:34.063871 nutritious-0.1.1/README.md
+-rw-r--r--   0        0        0    12746 2024-05-27 07:13:34.063871 nutritious-0.1.1/nutritious/__init__.py
+-rw-r--r--   0        0        0     1442 2024-05-27 07:13:34.063871 nutritious-0.1.1/nutritious/__main__.py
+-rw-r--r--   0        0        0     1434 2024-05-27 07:13:34.063871 nutritious-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4409 1970-01-01 00:00:00.000000 nutritious-0.1.1/PKG-INFO
```

### Comparing `nutritious-0.1.0/LICENSE` & `nutritious-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nutritious-0.1.0/README.md` & `nutritious-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -6,22 +6,15 @@
 
 **Nutritious Litchi** is a Python package that allows you to write JSX-like syntax in Python for creating HTML elements and components. It contains a CLI which is used to convert XML-JSX to Python Objects. **Feel free to use to make a web framework with this**. This started as a fork of [Packed](https://github.com/michaeljones/packed).
 
 > [!WARNING]  
 > Please note that this is project is in experimental stage. It is a fork of [Packed](https://github.com/michaeljones/packed) and has been modified and optimized.
 
 ## Installation
-
-To install the package, clone the repository and use `pip`:
-
-```bash
-git clone https://github.com/yourusername/nutritious-litchi.git
-cd nutritious-litchi
-pip install .
-
+```
 # you can use any python package manager like pip and poetry to install nutritious instead
 pip install nutritious
 ```
 
 ## Usage
 
 ### Basic Example (located in `app/` folder)
```

#### html2text {}

```diff
@@ -4,22 +4,20 @@
                         ************ NNuuttrriittiioouuss LLiittcchhii ************
 **Nutritious Litchi** is a Python package that allows you to write JSX-like
 syntax in Python for creating HTML elements and components. It contains a CLI
 which is used to convert XML-JSX to Python Objects. **Feel free to use to make
 a web framework with this**. This started as a fork of [Packed](https://
 github.com/michaeljones/packed). > [!WARNING] > Please note that this is
 project is in experimental stage. It is a fork of [Packed](https://github.com/
-michaeljones/packed) and has been modified and optimized. ## Installation To
-install the package, clone the repository and use `pip`: ```bash git clone
-https://github.com/yourusername/nutritious-litchi.git cd nutritious-litchi pip
-install . # you can use any python package manager like pip and poetry to
-install nutritious instead pip install nutritious ``` ## Usage ### Basic
-Example (located in `app/` folder) ```python from nutritious import litchi,
-Element # Element import is required even though it's not in the script.
-@litchi def render(): return (
+michaeljones/packed) and has been modified and optimized. ## Installation ``` #
+you can use any python package manager like pip and poetry to install
+nutritious instead pip install nutritious ``` ## Usage ### Basic Example
+(located in `app/` folder) ```python from nutritious import litchi, Element #
+Element import is required even though it's not in the script. @litchi def
+render(): return (
 ************ HHeelllloo,, WWoorrlldd!! ************
 This is a JSX-like syntax in Python.
 _L_i_n_k
 ) ``` ### Custom Components ```python from nutritious import Component, litchi
 class MyComponent(Component): # type: ignore def render(self): return
 This is a custom component with a prop: {self.props['message']}
 @litchi def app(): return ``` # Output `dist/` folder ```python from nutritious
```

### Comparing `nutritious-0.1.0/nutritious/__init__.py` & `nutritious-0.1.1/nutritious/__init__.py`

 * *Files identical despite different names*

### Comparing `nutritious-0.1.0/nutritious/__main__.py` & `nutritious-0.1.1/nutritious/__main__.py`

 * *Files identical despite different names*

### Comparing `nutritious-0.1.0/pyproject.toml` & `nutritious-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nutritious"
-version = "0.1.0"
+version = "0.1.1"
 description = "A jsx-preprocessor for Python which enables the coder to write JSX directly in Python 🗿"
 authors = ["Adarsh Gourab Mahalik <gourabmahalikadarsh@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/itsmeadarsh2008/nutritious"
 repository = "https://github.com/itsmeadarsh2008/nutritious.git"
 license = "GPL"
 keywords = [
```

### Comparing `nutritious-0.1.0/PKG-INFO` & `nutritious-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutritious
-Version: 0.1.0
+Version: 0.1.1
 Summary: A jsx-preprocessor for Python which enables the coder to write JSX directly in Python 🗿
 Home-page: https://github.com/itsmeadarsh2008/nutritious
 License: GPL
 Keywords: jsx,nutritious,preprocessor,python,jsx-python,jsx-py,jsx-preprocessor,jsx-transpiler,jsx-compiler,jsx-parser,jsx-renderer,jsx-generator,jsx-transformer,jsx-converter,jsx-translation,jsx-translation-tool,jsx-to-python,jsx-in-python,jsx-for-python,jsx-python-integration,jsx-python-support,python-jsx,py-jsx,python-jsx-preprocessor,python-jsx-transpiler,python-jsx-compiler,python-jsx-parser,python-jsx-renderer,python-jsx-generator,python-jsx-transformer,python-jsx-converter,python-jsx-translation,python-jsx-translation-tool,jsx-python-converter
 Author: Adarsh Gourab Mahalik
 Author-email: gourabmahalikadarsh@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -27,22 +27,15 @@
 
 **Nutritious Litchi** is a Python package that allows you to write JSX-like syntax in Python for creating HTML elements and components. It contains a CLI which is used to convert XML-JSX to Python Objects. **Feel free to use to make a web framework with this**. This started as a fork of [Packed](https://github.com/michaeljones/packed).
 
 > [!WARNING]  
 > Please note that this is project is in experimental stage. It is a fork of [Packed](https://github.com/michaeljones/packed) and has been modified and optimized.
 
 ## Installation
-
-To install the package, clone the repository and use `pip`:
-
-```bash
-git clone https://github.com/yourusername/nutritious-litchi.git
-cd nutritious-litchi
-pip install .
-
+```
 # you can use any python package manager like pip and poetry to install nutritious instead
 pip install nutritious
 ```
 
 ## Usage
 
 ### Basic Example (located in `app/` folder)
```

