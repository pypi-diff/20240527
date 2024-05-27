# Comparing `tmp/peelpreter-1.0.1.tar.gz` & `tmp/peelpreter-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peelpreter-1.0.1.tar", last modified: Thu May 23 11:38:13 2024, max compression
+gzip compressed data, was "peelpreter-1.1.2.tar", last modified: Mon May 27 09:18:29 2024, max compression
```

## Comparing `peelpreter-1.0.1.tar` & `peelpreter-1.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 jeebak    (1000) jeebak    (1000)        0 2024-05-23 11:38:13.118106 peelpreter-1.0.1/
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)    35150 2024-05-21 06:44:48.000000 peelpreter-1.0.1/COPYING
--rw-r--r--   0 jeebak    (1000) jeebak    (1000)     3688 2024-05-23 11:38:13.118106 peelpreter-1.0.1/PKG-INFO
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     2559 2024-05-23 08:20:27.000000 peelpreter-1.0.1/README.md
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     1475 2024-05-23 11:38:10.000000 peelpreter-1.0.1/pyproject.toml
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)       38 2024-05-23 11:38:13.118106 peelpreter-1.0.1/setup.cfg
-drwxrwxr-x   0 jeebak    (1000) jeebak    (1000)        0 2024-05-23 11:38:13.118106 peelpreter-1.0.1/src/
-drwxrwxr-x   0 jeebak    (1000) jeebak    (1000)        0 2024-05-23 11:38:13.118106 peelpreter-1.0.1/src/Peelpreter.egg-info/
--rw-r--r--   0 jeebak    (1000) jeebak    (1000)     3688 2024-05-23 11:38:13.000000 peelpreter-1.0.1/src/Peelpreter.egg-info/PKG-INFO
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)      832 2024-05-23 11:38:13.000000 peelpreter-1.0.1/src/Peelpreter.egg-info/SOURCES.txt
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)        1 2024-05-23 11:38:13.000000 peelpreter-1.0.1/src/Peelpreter.egg-info/dependency_links.txt
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)       52 2024-05-23 11:38:13.000000 peelpreter-1.0.1/src/Peelpreter.egg-info/entry_points.txt
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)       11 2024-05-23 11:38:13.000000 peelpreter-1.0.1/src/Peelpreter.egg-info/top_level.txt
-drwxrwxr-x   0 jeebak    (1000) jeebak    (1000)        0 2024-05-23 11:38:13.118106 peelpreter-1.0.1/src/peelpreter/
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     1095 2024-05-23 08:23:24.000000 peelpreter-1.0.1/src/peelpreter/__init__.py
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     4481 2024-05-22 05:31:32.000000 peelpreter-1.0.1/src/peelpreter/__main__.py
-drwxrwxr-x   0 jeebak    (1000) jeebak    (1000)        0 2024-05-23 11:38:13.118106 peelpreter-1.0.1/src/peelpreter/astt/
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     1733 2024-05-22 05:27:53.000000 peelpreter-1.0.1/src/peelpreter/astt/__init__.py
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     7698 2024-05-23 08:27:28.000000 peelpreter-1.0.1/src/peelpreter/astt/astt.py
-drwxrwxr-x   0 jeebak    (1000) jeebak    (1000)        0 2024-05-23 11:38:13.118106 peelpreter-1.0.1/src/peelpreter/error/
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     1589 2024-05-22 05:28:18.000000 peelpreter-1.0.1/src/peelpreter/error/__init__.py
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     4728 2024-05-22 05:28:09.000000 peelpreter-1.0.1/src/peelpreter/error/error.py
-drwxrwxr-x   0 jeebak    (1000) jeebak    (1000)        0 2024-05-23 11:38:13.118106 peelpreter-1.0.1/src/peelpreter/evaluator/
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     1070 2024-05-22 05:28:41.000000 peelpreter-1.0.1/src/peelpreter/evaluator/__init__.py
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)    12503 2024-05-22 05:28:29.000000 peelpreter-1.0.1/src/peelpreter/evaluator/evaluator.py
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     5583 2024-05-22 05:28:49.000000 peelpreter-1.0.1/src/peelpreter/evaluator/mbuiltins.py
-drwxrwxr-x   0 jeebak    (1000) jeebak    (1000)        0 2024-05-23 11:38:13.118106 peelpreter-1.0.1/src/peelpreter/lexer/
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     1026 2024-05-22 05:29:05.000000 peelpreter-1.0.1/src/peelpreter/lexer/__init__.py
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     6528 2024-05-22 05:29:20.000000 peelpreter-1.0.1/src/peelpreter/lexer/tokenizer.py
-drwxrwxr-x   0 jeebak    (1000) jeebak    (1000)        0 2024-05-23 11:38:13.118106 peelpreter-1.0.1/src/peelpreter/objectt/
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     1738 2024-05-22 05:29:38.000000 peelpreter-1.0.1/src/peelpreter/objectt/__init__.py
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     1465 2024-05-22 05:29:31.000000 peelpreter-1.0.1/src/peelpreter/objectt/enviroment.py
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     5180 2024-05-22 05:29:52.000000 peelpreter-1.0.1/src/peelpreter/objectt/objectt.py
-drwxrwxr-x   0 jeebak    (1000) jeebak    (1000)        0 2024-05-23 11:38:13.118106 peelpreter-1.0.1/src/peelpreter/parser/
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     1017 2024-05-22 05:30:06.000000 peelpreter-1.0.1/src/peelpreter/parser/__init__.py
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)    17749 2024-05-22 05:30:14.000000 peelpreter-1.0.1/src/peelpreter/parser/parser.py
-drwxrwxr-x   0 jeebak    (1000) jeebak    (1000)        0 2024-05-23 11:38:13.118106 peelpreter-1.0.1/src/peelpreter/token_type/
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     1884 2024-05-22 05:30:25.000000 peelpreter-1.0.1/src/peelpreter/token_type/__init__.py
--rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     2493 2024-05-22 05:30:44.000000 peelpreter-1.0.1/src/peelpreter/token_type/token_type.py
+drwxrwxr-x   0 jeebak    (1000) jeebak    (1000)        0 2024-05-27 09:18:29.004609 peelpreter-1.1.2/
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)    35150 2024-05-21 06:44:48.000000 peelpreter-1.1.2/COPYING
+-rw-r--r--   0 jeebak    (1000) jeebak    (1000)     3766 2024-05-27 09:18:29.000609 peelpreter-1.1.2/PKG-INFO
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     2488 2024-05-26 05:53:02.000000 peelpreter-1.1.2/README.md
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     1610 2024-05-27 09:16:22.000000 peelpreter-1.1.2/pyproject.toml
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)       38 2024-05-27 09:18:29.004609 peelpreter-1.1.2/setup.cfg
+drwxrwxr-x   0 jeebak    (1000) jeebak    (1000)        0 2024-05-27 09:18:28.996609 peelpreter-1.1.2/src/
+drwxrwxr-x   0 jeebak    (1000) jeebak    (1000)        0 2024-05-27 09:18:29.000609 peelpreter-1.1.2/src/Peelpreter.egg-info/
+-rw-r--r--   0 jeebak    (1000) jeebak    (1000)     3766 2024-05-27 09:18:28.000000 peelpreter-1.1.2/src/Peelpreter.egg-info/PKG-INFO
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)      832 2024-05-27 09:18:28.000000 peelpreter-1.1.2/src/Peelpreter.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)        1 2024-05-27 09:18:28.000000 peelpreter-1.1.2/src/Peelpreter.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)       52 2024-05-27 09:18:28.000000 peelpreter-1.1.2/src/Peelpreter.egg-info/entry_points.txt
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)       11 2024-05-27 09:18:28.000000 peelpreter-1.1.2/src/Peelpreter.egg-info/top_level.txt
+drwxrwxr-x   0 jeebak    (1000) jeebak    (1000)        0 2024-05-27 09:18:29.000609 peelpreter-1.1.2/src/peelpreter/
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     1095 2024-05-27 09:07:37.000000 peelpreter-1.1.2/src/peelpreter/__init__.py
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     4516 2024-05-27 08:53:30.000000 peelpreter-1.1.2/src/peelpreter/__main__.py
+drwxrwxr-x   0 jeebak    (1000) jeebak    (1000)        0 2024-05-27 09:18:29.000609 peelpreter-1.1.2/src/peelpreter/astt/
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     1733 2024-05-22 05:27:53.000000 peelpreter-1.1.2/src/peelpreter/astt/__init__.py
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     7733 2024-05-27 06:35:48.000000 peelpreter-1.1.2/src/peelpreter/astt/astt.py
+drwxrwxr-x   0 jeebak    (1000) jeebak    (1000)        0 2024-05-27 09:18:29.000609 peelpreter-1.1.2/src/peelpreter/error/
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     1555 2024-05-27 02:52:06.000000 peelpreter-1.1.2/src/peelpreter/error/__init__.py
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     4736 2024-05-27 08:53:30.000000 peelpreter-1.1.2/src/peelpreter/error/error.py
+drwxrwxr-x   0 jeebak    (1000) jeebak    (1000)        0 2024-05-27 09:18:29.000609 peelpreter-1.1.2/src/peelpreter/evaluator/
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     1070 2024-05-22 05:28:41.000000 peelpreter-1.1.2/src/peelpreter/evaluator/__init__.py
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)    12661 2024-05-27 08:53:30.000000 peelpreter-1.1.2/src/peelpreter/evaluator/evaluator.py
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     5549 2024-05-27 08:53:30.000000 peelpreter-1.1.2/src/peelpreter/evaluator/mbuiltins.py
+drwxrwxr-x   0 jeebak    (1000) jeebak    (1000)        0 2024-05-27 09:18:29.000609 peelpreter-1.1.2/src/peelpreter/lexer/
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     1026 2024-05-22 05:29:05.000000 peelpreter-1.1.2/src/peelpreter/lexer/__init__.py
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     6499 2024-05-27 08:53:30.000000 peelpreter-1.1.2/src/peelpreter/lexer/tokenizer.py
+drwxrwxr-x   0 jeebak    (1000) jeebak    (1000)        0 2024-05-27 09:18:29.000609 peelpreter-1.1.2/src/peelpreter/objectt/
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     1738 2024-05-22 05:29:38.000000 peelpreter-1.1.2/src/peelpreter/objectt/__init__.py
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     1465 2024-05-22 05:29:31.000000 peelpreter-1.1.2/src/peelpreter/objectt/enviroment.py
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     5177 2024-05-27 06:35:48.000000 peelpreter-1.1.2/src/peelpreter/objectt/objectt.py
+drwxrwxr-x   0 jeebak    (1000) jeebak    (1000)        0 2024-05-27 09:18:29.000609 peelpreter-1.1.2/src/peelpreter/parser/
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     1017 2024-05-22 05:30:06.000000 peelpreter-1.1.2/src/peelpreter/parser/__init__.py
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)    18097 2024-05-27 08:53:30.000000 peelpreter-1.1.2/src/peelpreter/parser/parser.py
+drwxrwxr-x   0 jeebak    (1000) jeebak    (1000)        0 2024-05-27 09:18:29.000609 peelpreter-1.1.2/src/peelpreter/token_type/
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     1884 2024-05-26 17:20:36.000000 peelpreter-1.1.2/src/peelpreter/token_type/__init__.py
+-rw-rw-r--   0 jeebak    (1000) jeebak    (1000)     2493 2024-05-26 17:20:36.000000 peelpreter-1.1.2/src/peelpreter/token_type/token_type.py
```

### Comparing `peelpreter-1.0.1/COPYING` & `peelpreter-1.1.2/COPYING`

 * *Files identical despite different names*

### Comparing `peelpreter-1.0.1/PKG-INFO` & `peelpreter-1.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,71 @@
 Metadata-Version: 2.1
 Name: Peelpreter
-Version: 1.0.1
+Version: 1.1.2
 Summary: A interpreter written in Python for the language, Monkey
 Author: Jeebak Samajdwar
 Maintainer: Jeebak Samajdwar
 License: GPL
 Project-URL: Repository, https://github.com/GogiBoy102/Peelpreter
 Keywords: monkey,interpreter,ast,treewalker,vm,programing language,language
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Interpreters
 Classifier: Typing :: Typed
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: COPYING
 
-### Monkey
+# Monkey
 Peelpreter is a interpreter for the language Monkey specified in the book `Writing an Interpreter in Go`.
 It is not not designed to be the fastest implementation but instead a (mostly) readable one. 
 I, personally don't find encapsulating every little function of a program in classes to be particularly readable.
 Hence, I have kept things bare-bone functions where I thought it made sense and used classes to encapsulate data like C-Structs
 and sometimes to store methods.
 
-## Monkey Features
+### Monkey Features
 Peelpreter supports all features of the canon implementation as well as some more.
 They are:-
-    1. Variables
-    2. If expressions
-    3. First-Class Functions
-    4. Closures
-    5. Array
-    6. Hash Map (Dictionary)
-    7. Builtin Functions
-    8. Array and Hash mutability
-    9. Improved `puts` function
+1. Variables
+2. If expressions
+3. First-Class Functions
+4. Closures
+5. Array
+6. Hash Map (Dictionary)
+7. Builtin Functions
+8. Array and Hash mutability
+9. Improved `puts` function
 
-## Features Planned to be added
+### Features Planned to be added
 Some features which I wish for in a programming language are not present yet in this.
 Suppport for them will be added as soon as type annotations are improved for the existing code base.
 They are:-
-    1. Input function
-    2. Type conversion
-    3. Chaining variable assignments. E.g, `let x = y = 7`
-    3. Constants
-    4. Loops
-    5. Structs
-    6. Import System
-    7. Extension modules using Python
+1. Input function
+2. Type conversion
+3. Chaining variable assignments. E.g, `let x = y = 7`
+3. Constants
+4. Loops
+5. Structs
+6. Import System
+7. Extension modules using Python
 
-### Installation
+## Installation
 For installation of the package run,
 ```
 pip install peelpreter
 ```
 Or if you would prefer to build and install yourself, clone the repository and cd into it,
 ```
 git clone https://github.com/GogiBoy102/Peelpreter.git
@@ -79,24 +82,24 @@
 After the build process end, cd into `dist` and install the tar with,
 ```
 cd dist
 pip install peelpreter-<version>.tar.gz
 ```
 And, voila! Peelpreter has been installed! For usage, follow the next section.
 
-### Usage
+## Usage
 Peelpreter comes with a script called `monkey` which is the entry point for the interpreter and also the reccomended way for it to be used.
 
 Files in monkey usually have the extension ".mon".
 
 `monkey`, when executed with no command line arguments starts the REPL for Monkey. However, it can also execute files if the path to those files are supplied as a command line argument.
 The examples directory can be looked at for example programs writen in Monkey.
 ```
 monkey (for starting a repl)
 ```
 ```
 monkey /path/to/file (for running a file)
 ```
 
-### License
+## License
 Peelpreter is license under the GNU General Public License version 3 or above with it also being copyrighted by `Jeebak Samajdwar`
```

### Comparing `peelpreter-1.0.1/README.md` & `peelpreter-1.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-### Monkey
+# Monkey
 Peelpreter is a interpreter for the language Monkey specified in the book `Writing an Interpreter in Go`.
 It is not not designed to be the fastest implementation but instead a (mostly) readable one. 
 I, personally don't find encapsulating every little function of a program in classes to be particularly readable.
 Hence, I have kept things bare-bone functions where I thought it made sense and used classes to encapsulate data like C-Structs
 and sometimes to store methods.
 
-## Monkey Features
+### Monkey Features
 Peelpreter supports all features of the canon implementation as well as some more.
 They are:-
-    1. Variables
-    2. If expressions
-    3. First-Class Functions
-    4. Closures
-    5. Array
-    6. Hash Map (Dictionary)
-    7. Builtin Functions
-    8. Array and Hash mutability
-    9. Improved `puts` function
+1. Variables
+2. If expressions
+3. First-Class Functions
+4. Closures
+5. Array
+6. Hash Map (Dictionary)
+7. Builtin Functions
+8. Array and Hash mutability
+9. Improved `puts` function
 
-## Features Planned to be added
+### Features Planned to be added
 Some features which I wish for in a programming language are not present yet in this.
 Suppport for them will be added as soon as type annotations are improved for the existing code base.
 They are:-
-    1. Input function
-    2. Type conversion
-    3. Chaining variable assignments. E.g, `let x = y = 7`
-    3. Constants
-    4. Loops
-    5. Structs
-    6. Import System
-    7. Extension modules using Python
+1. Input function
+2. Type conversion
+3. Chaining variable assignments. E.g, `let x = y = 7`
+3. Constants
+4. Loops
+5. Structs
+6. Import System
+7. Extension modules using Python
 
-### Installation
+## Installation
 For installation of the package run,
 ```
 pip install peelpreter
 ```
 Or if you would prefer to build and install yourself, clone the repository and cd into it,
 ```
 git clone https://github.com/GogiBoy102/Peelpreter.git
@@ -52,24 +52,24 @@
 After the build process end, cd into `dist` and install the tar with,
 ```
 cd dist
 pip install peelpreter-<version>.tar.gz
 ```
 And, voila! Peelpreter has been installed! For usage, follow the next section.
 
-### Usage
+## Usage
 Peelpreter comes with a script called `monkey` which is the entry point for the interpreter and also the reccomended way for it to be used.
 
 Files in monkey usually have the extension ".mon".
 
 `monkey`, when executed with no command line arguments starts the REPL for Monkey. However, it can also execute files if the path to those files are supplied as a command line argument.
 The examples directory can be looked at for example programs writen in Monkey.
 ```
 monkey (for starting a repl)
 ```
 ```
 monkey /path/to/file (for running a file)
 ```
 
-### License
+## License
 Peelpreter is license under the GNU General Public License version 3 or above with it also being copyrighted by `Jeebak Samajdwar`
```

### Comparing `peelpreter-1.0.1/pyproject.toml` & `peelpreter-1.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -9,26 +9,29 @@
 authors = [
     {name = "Jeebak Samajdwar"}
 ]
 maintainers = [
     {name = "Jeebak Samajdwar"}
 ]
 license = {text = "GPL"}
-requires-python = ">= 3.10"
+requires-python = ">= 3.7"
 dynamic = ["version"]
 keywords = ["monkey", "interpreter", "ast", "treewalker", "vm", "programing language", "language"]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9", 
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Software Development",
     "Topic :: Software Development :: Interpreters",
     "Typing :: Typed"
 ]
```

### Comparing `peelpreter-1.0.1/src/Peelpreter.egg-info/PKG-INFO` & `peelpreter-1.1.2/src/Peelpreter.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,71 @@
 Metadata-Version: 2.1
 Name: Peelpreter
-Version: 1.0.1
+Version: 1.1.2
 Summary: A interpreter written in Python for the language, Monkey
 Author: Jeebak Samajdwar
 Maintainer: Jeebak Samajdwar
 License: GPL
 Project-URL: Repository, https://github.com/GogiBoy102/Peelpreter
 Keywords: monkey,interpreter,ast,treewalker,vm,programing language,language
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Interpreters
 Classifier: Typing :: Typed
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: COPYING
 
-### Monkey
+# Monkey
 Peelpreter is a interpreter for the language Monkey specified in the book `Writing an Interpreter in Go`.
 It is not not designed to be the fastest implementation but instead a (mostly) readable one. 
 I, personally don't find encapsulating every little function of a program in classes to be particularly readable.
 Hence, I have kept things bare-bone functions where I thought it made sense and used classes to encapsulate data like C-Structs
 and sometimes to store methods.
 
-## Monkey Features
+### Monkey Features
 Peelpreter supports all features of the canon implementation as well as some more.
 They are:-
-    1. Variables
-    2. If expressions
-    3. First-Class Functions
-    4. Closures
-    5. Array
-    6. Hash Map (Dictionary)
-    7. Builtin Functions
-    8. Array and Hash mutability
-    9. Improved `puts` function
+1. Variables
+2. If expressions
+3. First-Class Functions
+4. Closures
+5. Array
+6. Hash Map (Dictionary)
+7. Builtin Functions
+8. Array and Hash mutability
+9. Improved `puts` function
 
-## Features Planned to be added
+### Features Planned to be added
 Some features which I wish for in a programming language are not present yet in this.
 Suppport for them will be added as soon as type annotations are improved for the existing code base.
 They are:-
-    1. Input function
-    2. Type conversion
-    3. Chaining variable assignments. E.g, `let x = y = 7`
-    3. Constants
-    4. Loops
-    5. Structs
-    6. Import System
-    7. Extension modules using Python
+1. Input function
+2. Type conversion
+3. Chaining variable assignments. E.g, `let x = y = 7`
+3. Constants
+4. Loops
+5. Structs
+6. Import System
+7. Extension modules using Python
 
-### Installation
+## Installation
 For installation of the package run,
 ```
 pip install peelpreter
 ```
 Or if you would prefer to build and install yourself, clone the repository and cd into it,
 ```
 git clone https://github.com/GogiBoy102/Peelpreter.git
@@ -79,24 +82,24 @@
 After the build process end, cd into `dist` and install the tar with,
 ```
 cd dist
 pip install peelpreter-<version>.tar.gz
 ```
 And, voila! Peelpreter has been installed! For usage, follow the next section.
 
-### Usage
+## Usage
 Peelpreter comes with a script called `monkey` which is the entry point for the interpreter and also the reccomended way for it to be used.
 
 Files in monkey usually have the extension ".mon".
 
 `monkey`, when executed with no command line arguments starts the REPL for Monkey. However, it can also execute files if the path to those files are supplied as a command line argument.
 The examples directory can be looked at for example programs writen in Monkey.
 ```
 monkey (for starting a repl)
 ```
 ```
 monkey /path/to/file (for running a file)
 ```
 
-### License
+## License
 Peelpreter is license under the GNU General Public License version 3 or above with it also being copyrighted by `Jeebak Samajdwar`
```

### Comparing `peelpreter-1.0.1/src/Peelpreter.egg-info/SOURCES.txt` & `peelpreter-1.1.2/src/Peelpreter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peelpreter-1.0.1/src/peelpreter/__init__.py` & `peelpreter-1.1.2/src/peelpreter/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ########################################################################################
 
 from .objectt import Object as Object
 
 __author__ = "Jeebak Samajdwar"
 __license__ = "GPL"
-__version__ = "1.0.1"
+__version__ = "1.1.2"
```

### Comparing `peelpreter-1.0.1/src/peelpreter/__main__.py` & `peelpreter-1.1.2/src/peelpreter/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ########################################################################################
 
+from __future__ import annotations
 import readline  # noqa: F401
 from sys import argv
 from typing import Optional, Union
 
 from .astt import Program
 from . import error
 from .evaluator import evaluate
```

### Comparing `peelpreter-1.0.1/src/peelpreter/astt/__init__.py` & `peelpreter-1.1.2/src/peelpreter/astt/__init__.py`

 * *Files identical despite different names*

### Comparing `peelpreter-1.0.1/src/peelpreter/astt/astt.py` & `peelpreter-1.1.2/src/peelpreter/astt/astt.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ########################################################################################
 
+from __future__ import annotations
 from typing import Union
 
 from .. import token_type as ttype
 
 class Node:
     def __init__(self, literal: str) -> None:
         self.literal = literal
```

### Comparing `peelpreter-1.0.1/src/peelpreter/error/__init__.py` & `peelpreter-1.1.2/src/peelpreter/error/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 ########################################################################################
 
 from .error import (
     Error as Error,
     IllegalCharErr as IllegalCharErr,
     UnexpectedToken as UnexpectedToken,
     NoPrefixFunc as NoPrefixFunc,
-    TypeMismatch as TypeMismatch,
     UnknownOperator as UnknownOperator,
     UnknownIdentifier as UnknownIdentifier,
     NotAFunction as NotAFunction,
     UnexpectedEOF as UnexpectedEOF,
     ArgumentError as ArgumentError,
     UnsupportedType as UnsupportedType,
     UnsupportedIndexAccessType as UnsupportedIndexAccessType,
```

### Comparing `peelpreter-1.0.1/src/peelpreter/error/error.py` & `peelpreter-1.1.2/src/peelpreter/error/error.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,21 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ########################################################################################
 
+from __future__ import annotations
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from ..token_type import Token
+    from ..objectt import Object
+
 class Error:
     def __init__(self, fname: str, errtype: str, info: str, location: tuple[int, int]) -> None:
         self.fname = fname
         self.errtype = errtype
         self.info = info
         self.location = location
 
@@ -29,60 +36,56 @@
         return f"File <{self.fname}> at line {self.location[0]} and column {self.location[1]},\n{self.errtype}: {self.info}"
 
 class IllegalCharErr(Error):
     def __init__(self, fname: str, char: str, location: tuple[int, int]) -> None:
         super().__init__(fname, "IllegalCharErr", f"illegal charecter '{char}'", location)
 
 class UnexpectedToken(Error):
-    def __init__(self, fname: str, expected_token, got_token, location: tuple[int, int]) -> None:
+    def __init__(self, fname: str, expected_token: str, got_token: str, location: tuple[int, int]) -> None:
         super().__init__(fname, "UnexpectedToken", f"expected token {expected_token}, got {got_token}", location)
 
 class NoPrefixFunc(Error):
-    def __init__(self, fname: str, token, location: tuple[int, int]) -> None:
+    def __init__(self, fname: str, token: "Token", location: tuple[int, int]) -> None:
         super().__init__(fname, "NoPrefixFunc", f"no prefix function for parsing {token.string} found", location)
 
-class TypeMismatch(Error):
-    def __init__(self, fname: str, operator, left_type, right_type, location: tuple[int, int]) -> None:
-        super().__init__(fname, "TypeMismatch", f"Type mismatched in expression with operator: {operator} between {left_type} and {right_type}", location)
-
 class UnknownOperator(Error):
-    def __init__(self, fname: str, operator, left_type, right_type, location: tuple[int, int]) -> None:
+    def __init__(self, fname: str, operator: str, left_type: str | None, right_type: str, location: tuple[int, int]) -> None:
         if left_type is not None:
             super().__init__(fname, "UnknownOperator", f"unknown operator: {operator} between {left_type} and {right_type}", location)
         else:
             super().__init__(fname, "UnknownOperator", f"unknown operator: {operator} for {right_type}", location)
 
 class UnknownIdentifier(Error):
     def __init__(self, fname: str, name: str, location: tuple[int, int]) -> None:
         super().__init__(fname, "UnknownIdentifier", f"unknown identifier '{name}'", location)
 
 class NotAFunction(Error):
-    def __init__(self, fname: str, obj, location: tuple[int, int]) -> None:
+    def __init__(self, fname: str, obj: "Object", location: tuple[int, int]) -> None:
         super().__init__(fname, "NotAFunction", f"{obj.type()} is not a function", location)
 
 class UnexpectedEOF(Error):
     def __init__(self, fname: str, location: tuple[int, int]) -> None:
         super().__init__(fname, "UnexpectedEOF", "sudden unexpected EOF token encountered", location)
 
 class ArgumentError(Error):
-    def __init__(self, fname: str, expected, got, func, location: tuple[int, int]) -> None:
+    def __init__(self, fname: str, expected: int, got: int, func: str, location: tuple[int, int]) -> None:
         super().__init__(fname, "ArgumentError", f"wrong number of arguments, expected {expected} but got {got} for function {func}", location)
 
 class UnsupportedType(Error):
-    def __init__(self, fname: str, got, func, location: tuple[int, int]) -> None:
-        super().__init__(fname, "UnsupportedType", f"argument of type {got} not supported for function {func}", location)
+    def __init__(self, fname: str, got: "Object", func: str, location: tuple[int, int]) -> None:
+        super().__init__(fname, "UnsupportedType", f"argument of type {got.type()} not supported for function {func}", location)
 
 class UnsupportedIndexAccessType(Error):
-    def __init__(self, fname: str, type, location: tuple[int, int]) -> None:
-        super().__init__(fname, "UnsupportedIndexAccessType", f"{type} not supported for index access expressions", location)
+    def __init__(self, fname: str, type: "Object", location: tuple[int, int]) -> None:
+        super().__init__(fname, "UnsupportedIndexAccessType", f"{type.type()} not supported for index access expressions", location)
 
 class UnsupportedIndexType(Error):
-    def __init__(self, fname: str, got, location: tuple[int, int]) -> None:
-        super().__init__(fname, "UnsupportedIndexType", f"index of type {got} is not supported for array", location)
+    def __init__(self, fname: str, got: "Object", location: tuple[int, int]) -> None:
+        super().__init__(fname, "UnsupportedIndexType", f"index of type {got.type()} is not supported for array", location)
 
 class UnsupporteKeyType(Error):
-    def __init__(self, fname: str, type, location: tuple[int, int]) -> None:
-        super().__init__(fname, "UnsupportedKeyType", f"unsupported type {type} as key", location)
+    def __init__(self, fname: str, type: "Object", location: tuple[int, int]) -> None:
+        super().__init__(fname, "UnsupportedKeyType", f"unsupported type {type.type()} as key", location)
 
 class UnknownNode(Error):
     def __init__(self, fname: str, location: tuple[int, int]) -> None:
         super().__init__(fname, "UnknownNode", "unknown ast node encountered", location)
```

### Comparing `peelpreter-1.0.1/src/peelpreter/evaluator/__init__.py` & `peelpreter-1.1.2/src/peelpreter/evaluator/__init__.py`

 * *Files identical despite different names*

### Comparing `peelpreter-1.0.1/src/peelpreter/evaluator/evaluator.py` & `peelpreter-1.1.2/src/peelpreter/evaluator/evaluator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-########################################################################################
+##############################################################################
 #    Peelpreter is a interpreter designed to interpret the language, Monkey.
 #    Copyright (C) 2024 Jeebak Samajdwar
 #
 #    This file is part of Peelpreter
 #
 #    Peelpreter is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
@@ -12,54 +12,52 @@
 #    Peelpreter is distributed in the hope that it will be useful,
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-########################################################################################
+##############################################################################
 
 from sys import setrecursionlimit
 from typing import Union
 
 from .. import astt
 from ..objectt.enviroment import Enviroment
 from .. import error
 from ..evaluator.mbuiltins import builtins
 from .. import objectt as obj
 
 setrecursionlimit(10**6)
 
 
-def evaluate(
-    node: astt.Node, env: Enviroment, fname="stdin"
-) -> obj.Object:
-    def istruthy(cond_object):
+def evaluate(node: astt.Node, env: Enviroment, fname="stdin") -> obj.Object:
+    def istruthy(cond_object: obj.Object):
         if cond_object == obj.NULL:
             return False
         elif cond_object == obj.TRUE:
             return True
         elif cond_object == obj.FALSE:
             return False
         else:
             return True
 
-    def is_error(tobject):
+    def is_error(tobject: obj.Object):
         if tobject is not None:
             return tobject.type() == obj.OBJ_ERROR
         return False
 
     def eval_program(statements):
         result = obj.Object()
         for statement in statements:
             result = evaluate(statement, env)
 
-            if type(result) == obj.ReturnValue:
+            if isinstance(result, obj.ReturnValue):
                 return result.value
-            elif type(result) == obj.Error:
+            elif isinstance(result, obj.Error):
                 return result
 
         return result
 
     def eval_blockstmt(block: astt.BlockStatement):
         result: Union[obj.Object, None] = obj.Object()
 
@@ -71,71 +69,73 @@
                     result.type() == obj.OBJ_RETURN_VALUE
                     or result.type() == obj.OBJ_ERROR
                 ):
                     return result
 
         return result
 
-    def eval_prefixexpr(operator, right):
-        match operator:
-            case "!":
-                return eval_bang(right)
-            case "-":
-                return eval_minus(right)
-            case _:
-                return obj.Error(error.
-                    UnknownOperator(fname, operator, None, right.type(), (-1, -1))
-                )
+    def eval_prefixexpr(operator: str, right):
+        if operator ==  "!":
+            return eval_bang(right)
+        elif operator ==  "-":
+            return eval_minus(right)
+        else:
+            return obj.Error(
+                error.UnknownOperator(fname, operator, None, right.type(), (-1, -1))
+            )
 
     def eval_infixexpr(operator, left, right):
         if left.type() == obj.OBJ_NUM and right.type() == obj.OBJ_NUM:
             return eval_num_infixexpr(operator, left, right)
         elif left.type() == obj.OBJ_STRING and right.type() == obj.OBJ_STRING:
             return eval_str_infixexpr(operator, left, right)
         elif operator == "==":
             return obj.TRUE if left == right else obj.FALSE
         elif operator == "!=":
             return obj.TRUE if left != right else obj.FALSE
         else:
-            return obj.Error(error.
-                UnknownOperator(fname, operator, left.type(), right.type(), (-1, -1))
+            return obj.Error(
+                error.UnknownOperator(
+                    fname, operator, left.type(), right.type(), (-1, -1)
+                )
             )
 
     def eval_num_infixexpr(operator, left, right):
         leftval = left.value
         rightval = right.value
 
-        match operator:
-            case "+":
-                return obj.Number(leftval + rightval)
-            case "-":
-                return obj.Number(leftval - rightval)
-            case "*":
-                return obj.Number(leftval * rightval)
-            case "/":
-                return obj.Number(leftval / rightval)
-            case "<":
-                return obj.TRUE if leftval < rightval else obj.FALSE
-            case ">":
-                return obj.TRUE if leftval > rightval else obj.FALSE
-            case "==":
-                return obj.TRUE if leftval == rightval else obj.FALSE
-            case "!=":
-                return obj.TRUE if leftval != rightval else obj.FALSE
-            case _:
-                return obj.Error(error.
-                    UnknownOperator(
-                        fname, operator, left.type(), right.type(), (-1, -1)
-                    )
+        if operator == "+":
+            return obj.Number(leftval + rightval)
+        elif operator == "-":
+            return obj.Number(leftval - rightval)
+        elif operator == "*":
+            return obj.Number(leftval * rightval)
+        elif operator == "/":
+            return obj.Number(leftval / rightval)
+        elif operator == "<":
+            return obj.TRUE if leftval < rightval else obj.FALSE
+        elif operator == ">":
+            return obj.TRUE if leftval > rightval else obj.FALSE
+        elif operator == "==":
+            return obj.TRUE if leftval == rightval else obj.FALSE
+        elif operator == "!=":
+            return obj.TRUE if leftval != rightval else obj.FALSE
+        else:
+            return obj.Error(
+                error.UnknownOperator(
+                    fname, operator, left.type(), right.type(), (-1, -1)
                 )
+            )
 
     def eval_str_infixexpr(operator, left, right):
         if operator != "+":
-            return obj.Error(error.
-                UnknownOperator(fname, operator, left.type(), right.type(), (-1, -1))
+            return obj.Error(
+                error.UnknownOperator(
+                    fname, operator, left.type(), right.type(), (-1, -1)
+                )
             )
         left_val = left.value
         right_val = right.value
 
         return obj.String(left_val + right_val)
 
     def eval_exprs(expressions, env):
@@ -164,45 +164,44 @@
         pairs = dict()
 
         for key_node, val_node in node.pairs.items():
             key = evaluate(key_node, env)
             if is_error(key):
                 return key
             if not isinstance(key, obj.Hashable):
-                return obj.Error(error.UnsupporteKeyType(fname, key.type(), (-1, -1)))
- 
+                return obj.Error(error.UnsupporteKeyType(fname, key, (-1, -1)))
             value = evaluate(val_node, env)
             if is_error(value):
                 return value
             hashed = key.hash_key()
             pairs[hashed] = obj.HashPair(key, value)
 
         return obj.Hash(pairs)
 
     def eval_indexexpr(left, indexexpr):
         if left.type() == obj.OBJ_ARRAY and indexexpr.type() == obj.OBJ_NUM:
             return eval_arr_indexexpr(left, indexexpr)
         elif left.type() == obj.OBJ_HASH:
             return eval_hash_indexexpr(left, indexexpr)
         elif indexexpr.type() != obj.OBJ_NUM:
-            return obj.Error(error.UnsupportedIndexType(fname, indexexpr.type(), (-1, -1)))
+            return obj.Error(error.UnsupportedIndexType(fname, indexexpr, (-1, -1)))
         else:
-            return obj.Error(error.UnsupportedIndexAccessType(fname, left.type(), (-1, -1)))
+            return obj.Error(error.UnsupportedIndexAccessType(fname, left, (-1, -1)))
 
     def eval_hash_indexexpr(hash, indexexpr):
         if not isinstance(indexexpr, obj.Hashable):
-            return obj.Error(error.UnsupporteKeyType(fname, indexexpr.type(), (-1, -1)))
+            return obj.Error(error.UnsupporteKeyType(fname, indexexpr, (-1, -1)))
         pair = hash.pairs.get(indexexpr.hash_key())
         if pair is None:
             return obj.NULL
         return pair.value
 
     def eval_hash_reassign(hash, key, value):
         if not isinstance(key, obj.Hashable):
-            return obj.Error(error.UnsupporteKeyType(fname, key.type(), (-1, -1)))
+            return obj.Error(error.UnsupporteKeyType(fname, key, (-1, -1)))
 
         hash.pairs[key.hash_key()] = obj.HashPair(key, value)
 
         return value
 
     def eval_arr_indexexpr(array, indexexpr):
         index = int(indexexpr.value)
@@ -230,127 +229,130 @@
         builtin = builtins.get(node.literal)
         if builtin is not None:
             return builtin
 
         return obj.Error(error.UnknownIdentifier(fname, node.literal, (-1, -1)))
 
     def eval_minus(right):
-        if type(right) != obj.Number:
-            return obj.Error(error.UnknownOperator(fname, "-", None, right.type(), (-1, -1)))
+        if isinstance(right, obj.Number):
+            return obj.Error(
+                error.UnknownOperator(fname, "-", None, right.type(), (-1, -1))
+            )
         value = right.value
         return obj.Number(-value)
 
     def eval_bang(right):
         if right == obj.TRUE:
             return obj.FALSE
         elif right == obj.FALSE:
             return obj.TRUE
         elif right == obj.NULL:
             return obj.TRUE
         else:
             return obj.FALSE
 
     def apply_func(func, arguments):
-        if type(func) == obj.Function:
+        if isinstance(func, obj.Function):
             extended_env = extend_funcenv(func, arguments)
             evaluated = evaluate(func.body, extended_env)
             return unwrap_rtrvalue(evaluated)
-        elif type(func) == obj.Builtin:
+        elif isinstance(func, obj.Builtin):
             return func.func(fname, arguments)
 
         return obj.Error(error.NotAFunction(fname, func, (-1, -1)))
 
     def extend_funcenv(func: obj.Function, arguments):
         env = Enviroment(func.env)
         for index, parameter in enumerate(func.parametres):
             env.set_iden(parameter.literal, arguments[index])
         return env
 
     def unwrap_rtrvalue(tobject):
-        if type(tobject) == obj.ReturnValue:
+        if isinstance(tobject, obj.ReturnValue):
             return tobject.value
         return tobject
 
-    if type(node) == astt.Program:
-        return eval_program(node.statements)
-    elif type(node) == astt.ExpressionStatement:
+    if isinstance(node, astt.Program):
+        program: astt.Program = node
+        return eval_program(program.statements)
+    elif isinstance(node, astt.ExpressionStatement):
         return evaluate(node.expression, env)
-    elif type(node) == astt.PrefixExpression:
+    elif isinstance(node, astt.PrefixExpression):
         rightexpr = evaluate(node.rightexpr, env)
         if is_error(rightexpr):
             return rightexpr
         return eval_prefixexpr(node.operator, rightexpr)
-    elif type(node) == astt.InfixExpression:
+    elif isinstance(node, astt.InfixExpression):
         left = evaluate(node.leftexpr, env)
         if is_error(left):
             return left
         right = evaluate(node.rightexpr, env)
         if is_error(right):
             return right
         return eval_infixexpr(node.operator, left, right)
-    elif type(node) == astt.BlockStatement:
+    elif isinstance(node, astt.BlockStatement):
         return eval_blockstmt(node)
-    elif type(node) == astt.FunctionLiteral:
+    elif isinstance(node, astt.FunctionLiteral):
         parametres = node.parameters
         body = node.body
         return obj.Function(parametres, body, env)
-    elif type(node) == astt.CallExpression:
+    elif isinstance(node, astt.CallExpression):
         function = evaluate(node.function, env)
         if is_error(function):
             return function
         arguments = eval_exprs(node.arguments, env)
         if len(arguments) == 1 and is_error(arguments[0]):
             return arguments[0]
         return apply_func(function, arguments)
-    elif type(node) == astt.HashLiteral:
+    elif isinstance(node, astt.HashLiteral):
         return eval_hashlit(node, env)
-    elif type(node) == astt.ArrayLiteral:
+    elif isinstance(node, astt.ArrayLiteral):
         elements = eval_exprs(node.elements, env)
         if len(elements) == 1 and is_error(elements[0]):
             return elements[0]
         return obj.Array(elements)
-    elif type(node) == astt.IndexExpression:
+    elif isinstance(node, astt.IndexExpression):
         leftexpr = evaluate(node.left, env)
         if is_error(leftexpr):
             return leftexpr
         indexexpr = evaluate(node.index, env)
         if is_error(indexexpr):
             return indexexpr
         return eval_indexexpr(leftexpr, indexexpr)
-    elif type(node) == astt.IfExpression:
+    elif isinstance(node, astt.IfExpression):
         return eval_ifexpr(node)
-    elif type(node) == astt.ReturnStatement:
+    elif isinstance(node, astt.ReturnStatement):
         value = evaluate(node.valuexp, env)
         if is_error(value):
             return value
         return obj.ReturnValue(value)
-    elif type(node) == astt.LetStatement:
+    elif isinstance(node, astt.LetStatement):
         value = evaluate(node.value, env)
         if is_error(value):
             return value
         env.set_iden(name=node.name.literal, value=value)
         return value
-    elif type(node) == astt.ReassignmentStatement:
+    elif isinstance(node, astt.ReassignmentStatement):
         structure = evaluate(node.index_expr.left, env)
         index = evaluate(node.index_expr.index, env)
         value = evaluate(node.value, env)
         if isinstance(structure, obj.Array):
             return eval_arr_reassign(structure, index, value)
         elif isinstance(structure, obj.Hash):
             return eval_hash_reassign(structure, index, value)
         else:
             return obj.Error("Unsupported")
 
-    elif type(node) == astt.Identifier:
+    elif isinstance(node, astt.Identifier):
         return eval_identifier(node, env)
-    elif type(node) == astt.Number:
+    elif isinstance(node, astt.Number):
         return obj.Number(node.value)
-    elif type(node) == astt.String:
+    elif isinstance(node, astt.String):
         return obj.String(node.string)
-    elif type(node) == astt.Boolean:
+    elif isinstance(node, astt.Boolean):
         if node.value:
             return obj.TRUE
         return obj.FALSE
-    elif type(node) == astt.Null:
+    elif isinstance(node, astt.Null):
         return obj.NULL
 
     return obj.Error(error.UnknownNode(fname, (-1, -1)))
```

### Comparing `peelpreter-1.0.1/src/peelpreter/evaluator/mbuiltins.py` & `peelpreter-1.1.2/src/peelpreter/evaluator/mbuiltins.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ########################################################################################
 
+from __future__ import annotations
 from .. import error
 from .. import objectt as obj
 
 
 def arg_error(fname, expected, got, func):
     return obj.Error(error.ArgumentError(fname, expected, got, func, (-1, -1)))
 
@@ -29,15 +30,15 @@
     if len(args) != 1:
         return obj.Error(error.ArgumentError(fname, 1, len(args), "len", (-1, -1)))
     if type(args[0]) == obj.String:
         return obj.Number(len(args[0].value))
     elif type(args[0]) == obj.Array:
         return obj.Number(len(args[0].elements))
     else:
-        return obj.Error(error.UnsupportedType(fname, type(args[0]), "len", (-1, -1)))
+        return obj.Error(error.UnsupportedType(fname, args[0], "len", (-1, -1)))
 
 
 def m_type(fname, args):
     if len(args) != 1:
         return obj.Error(error.ArgumentError(fname, 1, len(args), "type", (-1, -1)))
     return obj.String(args[0].type())
 
@@ -53,15 +54,15 @@
     return obj.NULL
 
 
 def m_push(fname, args):
     if len(args) != 2:
         return obj.Error(error.ArgumentError(fname, 2, len(args), "push", (-1, -1)))
     if args[0].type() != obj.OBJ_ARRAY:
-        return obj.Error(error.UnsupportedType(fname, args[0].type(), "push", (-1, -1)))
+        return obj.Error(error.UnsupportedType(fname, args[0], "push", (-1, -1)))
     arr = args[0].elements
     arr.append(args[1])
 
     return obj.NULL
 
 
 def m_tail(fname, args):
@@ -72,79 +73,79 @@
         _, *tail = sequence
         return obj.Array(tail)
     elif args[0].type() != obj.OBJ_STRING:
         string = args[0].value
         _, *tail = string
         return obj.String(string)
     else:
-        return obj.Error(error.UnsupportedType(fname, args[0].type(), "tail", (-1, -1)))
+        return obj.Error(error.UnsupportedType(fname, args[0], "tail", (-1, -1)))
 
 def m_head(fname, args):
     if len(args) != 1:
         return arg_error(fname, 1, len(args), "head")
     if args[0].type() == obj.OBJ_ARRAY:
         arr = args[0].elements
         head, *_ = arr
         return obj.Array([head])
     elif args[0].type() != obj.OBJ_STRING:
         string = args[0].value
         head, *_ = string
         return obj.String([head])
     else:
-        return obj.Error(error.UnsupportedType(fname, args[0].type(), "head", (-1, -1)))
+        return obj.Error(error.UnsupportedType(fname, args[0], "head", (-1, -1)))
 
 def m_first(fname, args):
     if len(args) != 1:
         return arg_error(fname, 1, len(args), "first")
     if args[0].type() == obj.OBJ_ARRAY:
         arr = args[0].elements
         start = arr[0]
         return start
     elif args[0].type() == obj.OBJ_STRING:
         string = args[0].value
         start = string[0]
         return start
     else:
-        return obj.Error(error.UnsupportedType(fname, args[0].type(), "first", (-1, -1)))
+        return obj.Error(error.UnsupportedType(fname, args[0], "first", (-1, -1)))
 
 def m_last(fname, args):
     if len(args) != 1:
         return arg_error(fname, 1, len(args), "last")
     if args[0].type() == obj.OBJ_ARRAY:
         arr = args[0].elements
         end = arr[-1]
         return end
     elif args[0].type() == obj.OBJ_STRING:
         arr = args[0].elements
         end = arr[-1]
         return end
     else:
-        return obj.Error(error.UnsupportedType(fname, args[0].type(), "last", (-1, -1)))
+        return obj.Error(error.UnsupportedType(fname, args[0], "last", (-1, -1)))
 
 def m_insert(fname, args):
     if len(args) != 3:
         return arg_error(fname, 1, len(args), "insert")
     if args[0].type() != obj.OBJ_ARRAY:
-       return obj.Error(error.UnsupportedType(fname, args[0].type(), "insert", (-1, -1)))
+       return obj.Error(error.UnsupportedType(fname, args[0], "insert", (-1, -1)))
     elif args[1].type() != obj.OBJ_NUM:
-        return obj.Error(error.UnsupportedType(fname, args[0].type(), "insert", (-1, -1)))
+        return obj.Error(error.UnsupportedType(fname, args[0], "insert", (-1, -1)))
     arr = args[0].elements.copy()
     if len(arr) < args[1].value:
         arr = arr + [obj.NULL] * (int(args[1].value) - len(arr))
     arr.insert(int(args[1].value), args[2])
 
     return obj.Array(arr)
 
 def m_change(fname, args):
     if len(args) != 3:
         return arg_error(fname, 1, len(args), "change")
     elif args[0].type() != obj.OBJ_ARRAY:
-       return obj.Error(error.UnsupportedType(fname, args[0].type(), "change", (-1, -1)))
+       return obj.Error(error.UnsupportedType(fname, args[0], "change", (-1, -1)))
     elif args[1].type() != obj.OBJ_NUM:
-        return obj.Error(error.UnsupportedType(fname, args[0].type(), "change", (-1, -1)))
+        return obj.Error(error.UnsupportedType(fname, args[0], "change", (-1, -1)))
     
     arr = args[0].elements.copy()
     if args[1].value >= len(arr):
         return obj.Error("Too high")
     arr[int(args[1].value)] = args[2]
 
     return obj.Array(arr)
```

### Comparing `peelpreter-1.0.1/src/peelpreter/lexer/__init__.py` & `peelpreter-1.1.2/src/peelpreter/lexer/__init__.py`

 * *Files identical despite different names*

### Comparing `peelpreter-1.0.1/src/peelpreter/lexer/tokenizer.py` & `peelpreter-1.1.2/src/peelpreter/lexer/tokenizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ########################################################################################
 
+from __future__ import annotations
 from ..error import Error, IllegalCharErr, UnexpectedEOF
 from .. import token_type as ttoken
 
 def tokenize(source: str, fname: str = "stdin") -> list[ttoken.Token]:
     def advance(position: int) -> int:
         return position + 1 if position < len(source) -1 else -1
     def peek(position: int) -> str:
@@ -94,70 +95,68 @@
     while True:
         position = advance(position)
         if position == -1:
             break
         column += 1
         current = source[position]
 
-        match current:
-            case "=":
-                if peek(position) == "=" and peek(position) != "":
-                    position = advance(position)
-                    add_token(ttoken.TT_EQ, "==", tokens)
-                    continue
-                add_token(ttoken.TT_ASSIGN, current, tokens)
-            case "+":
-                add_token(ttoken.TT_PLUS, current, tokens)
-            case "-":
-                add_token(ttoken.TT_MINUS, current, tokens)
-            case "/":
-                add_token(ttoken.TT_SLASH, current, tokens)
-            case "*":
-                add_token(ttoken.TT_ASTERISK, current, tokens)
-            case "!":
-                if peek(position) == "=":
-                    position = advance(position)
-                    add_token(ttoken.TT_NTEQ, "!=", tokens)
-                    continue
-                add_token(ttoken.TT_BANG, current, tokens)
-            case "<":
-                add_token(ttoken.TT_LT, current, tokens)
-            case ">":
-                add_token(ttoken.TT_GT, current, tokens)
-            case "(":
-                add_token(ttoken.TT_LPAREN, current, tokens)
-            case ")":
-                add_token(ttoken.TT_RPAREN, current, tokens)
-            case "{":
-                add_token(ttoken.TT_LBRACE, current, tokens)
-            case "}":
-                add_token(ttoken.TT_RBRACE, current, tokens)
-            case "[":
-                add_token(ttoken.TT_LBRACKET, current, tokens)
-            case "]":
-                add_token(ttoken.TT_RBRACKET, current, tokens)
-            case ",":
-                add_token(ttoken.TT_COMMA, current, tokens)
-            case ":":
-                add_token(ttoken.TT_COLON, current, tokens)
-            case " ":
+        if current == "=":
+            if peek(position) == "=" and peek(position) != "":
+                position = advance(position)
+                add_token(ttoken.TT_EQ, "==", tokens)
                 continue
-            case "\t":
+            add_token(ttoken.TT_ASSIGN, current, tokens)
+        elif current == "+":
+            add_token(ttoken.TT_PLUS, current, tokens)
+        elif current == "-":
+            add_token(ttoken.TT_MINUS, current, tokens)
+        elif current == "/":
+            add_token(ttoken.TT_SLASH, current, tokens)
+        elif current == "*":
+            add_token(ttoken.TT_ASTERISK, current, tokens)
+        elif current == "!":
+            if peek(position) == "=":
+                position = advance(position)
+                add_token(ttoken.TT_NTEQ, "!=", tokens)
                 continue
-            case "\n":
-                column = 1
-                line += 1
-            case ";":
-                add_token(ttoken.TT_SEMICOLON, current, tokens)
-            case "\"":
-                position = handle_str(position, current, tokens, line, column)
-            case _:
-                if current.isalpha():
-                    position = handle_indentifier(position, current, tokens)
-                elif current.isdigit():
-                    position = handle_num(position, current, tokens)
-                else:
-                    add_err(IllegalCharErr(fname, current, (line, column)), current, tokens)
+            add_token(ttoken.TT_BANG, current, tokens)
+        elif current == "<":
+            add_token(ttoken.TT_LT, current, tokens)
+        elif current == ">":
+            add_token(ttoken.TT_GT, current, tokens)
+        elif current == "(":
+            add_token(ttoken.TT_LPAREN, current, tokens)
+        elif current == ")":
+            add_token(ttoken.TT_RPAREN, current, tokens)
+        elif current == "{":
+            add_token(ttoken.TT_LBRACE, current, tokens)
+        elif current == "}":
+            add_token(ttoken.TT_RBRACE, current, tokens)
+        elif current == "[":
+            add_token(ttoken.TT_LBRACKET, current, tokens)
+        elif current == "]":
+            add_token(ttoken.TT_RBRACKET, current, tokens)
+        elif current == ",":
+            add_token(ttoken.TT_COMMA, current, tokens)
+        elif current == ":":
+            add_token(ttoken.TT_COLON, current, tokens)
+        elif current == " ":
+            continue
+        elif current == "\t":
+            continue
+        elif current == "\n":
+            column = 1
+            line += 1
+        elif current == ";":
+            add_token(ttoken.TT_SEMICOLON, current, tokens)
+        elif current == "\"":
+            position = handle_str(position, current, tokens, line, column)
+        elif current.isalpha():
+            position = handle_indentifier(position, current, tokens)
+        elif current.isdigit():
+            position = handle_num(position, current, tokens)
+        else:
+            add_err(IllegalCharErr(fname, current, (line, column)), current, tokens)
                     
     add_token(ttoken.TT_EOF, "", tokens)
 
     return tokens
```

### Comparing `peelpreter-1.0.1/src/peelpreter/objectt/__init__.py` & `peelpreter-1.1.2/src/peelpreter/objectt/__init__.py`

 * *Files identical despite different names*

### Comparing `peelpreter-1.0.1/src/peelpreter/objectt/enviroment.py` & `peelpreter-1.1.2/src/peelpreter/objectt/enviroment.py`

 * *Files identical despite different names*

### Comparing `peelpreter-1.0.1/src/peelpreter/objectt/objectt.py` & `peelpreter-1.1.2/src/peelpreter/objectt/objectt.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def __init__(self, obj_type, value) -> None:
         self.obj_type = obj_type
         self.value = value
     def __eq__(self, value: object) -> bool:
         if not isinstance(value, HashKey):
             return False
         return value.value == self.value
-    def __ne__(self, value: object, /) -> bool:
+    def __ne__(self, value: object) -> bool:
         if not isinstance(value, HashKey):
             return True
         return not value.value == self.value
     def __hash__(self) -> int:
         return hash(f"{self.obj_type}: {self.value}")
     def __repr__(self) -> str:
         return f"{self.value}"
```

### Comparing `peelpreter-1.0.1/src/peelpreter/parser/__init__.py` & `peelpreter-1.1.2/src/peelpreter/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `peelpreter-1.0.1/src/peelpreter/parser/parser.py` & `peelpreter-1.1.2/src/peelpreter/parser/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,19 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ########################################################################################
 
+from __future__ import annotations
 from typing import Callable, Union
 
+from peelpreter.astt.astt import ArrayLiteral, BlockStatement, Expression, IndexExpression, Statement
+
 from .. import astt
 from ..error import Error, NoPrefixFunc, UnexpectedEOF, UnexpectedToken
 from .. import token_type as ttoken
 
 LOWEST = 1
 EQUALS = 2
 LESSGREATER = 3
@@ -45,21 +48,20 @@
 
     def get_precedence(token, precedences):
         if precedences.get(token.ttype) is not None:
             return precedences[token.ttype]
         return LOWEST
 
     def parse_statement(token: ttoken.Token, index):
-        match token.ttype:
-            case ttoken.TT_LET:
-                return parse_let(token, index, errors)
-            case ttoken.TT_RETURN:
-                return parse_return(token, index, errors)
-            case _:
-                return parse_statementexpr(token, index, errors)
+        if token.ttype == ttoken.TT_LET:
+            return parse_let(token, index, errors)
+        elif token.ttype == ttoken.TT_RETURN:
+            return parse_return(token, index, errors)
+        else:
+            return parse_statementexpr(token, index, errors)
 
     def parse_let(token, index, errors):
         index = advance(index)
 
         if peek(index).ttype == ttoken.TT_ASSIGN:
             statement, index = parse_assign(token, index, errors)
         else:
@@ -87,20 +89,21 @@
         if peek(index).ttype == ttoken.TT_SEMICOLON:
             index = advance(index)
             token = tokens[index]
 
         return statement, index
 
     def parse_reassign(token, index, errors):
-        statement = astt.ReassignmentStatement(token, astt.Expression(""), astt.Expression(""))
+        statement = astt.ReassignmentStatement(token, IndexExpression(token, ArrayLiteral(token, [Expression("")]), Expression("")), astt.Expression(""))
         
         token = tokens[index]
         index_expr, index = parse_expression(LOWEST, token, index)
 
         if index_expr is not None:
+            assert isinstance(index_expr, IndexExpression)
             statement.index_expr = index_expr
         
         if peek(index).ttype != ttoken.TT_ASSIGN:
             errors.append(UnexpectedToken(fname, "=", peek(index).string, (-1, -1)))
             return None, index
 
         index = advance(advance(index))
@@ -270,15 +273,15 @@
 
         index = advance(index)
 
         return expression, index
 
     def parse_ifexpr(token, index):
         expression = astt.IfExpression(
-            token, astt.Expression(""), astt.Statement(""), astt.Statement("")
+            token, astt.Expression(""), BlockStatement(token, [Statement("")]), BlockStatement(token, [Statement("")])
         )
 
         if peek(index).ttype != ttoken.TT_LPAREN:
             errors.append(
                 UnexpectedToken(fname, ttoken.TT_LPAREN, peek(index).ttype, (-1, -1))
             )
             return None, index
@@ -319,15 +322,15 @@
             alternative, index = parse_block(token, index)
             if alternative is not None:
                 expression.alternative = alternative
 
         return expression, index
 
     def parse_funcliteral(token, index):
-        expression = astt.FunctionLiteral(token, [], astt.Statement(""))
+        expression = astt.FunctionLiteral(token, [], BlockStatement(token, [Statement("")]))
 
         if peek(index).ttype != ttoken.TT_LPAREN:
             errors.append(
                 UnexpectedToken(fname, ttoken.TT_LPAREN, peek(index).ttype, (-1, -1))
             )
             return None, index
         index = advance(index)
@@ -405,15 +408,16 @@
                 return None, index
             index = advance(advance(index))
             if peek(index).ttype == ttoken.TT_EOF:
                 errors.append(UnexpectedEOF(fname, (-1, -1)))
                 return None, index
             token = tokens[index]
             value, index = parse_expression(LOWEST, token, index)
-            hash_literal.pairs[key] = value
+            if key is not None and value is not None:
+                hash_literal.pairs[key] = value
             if (
                 peek(index).ttype != ttoken.TT_RBRACE
                 and peek(index).ttype != ttoken.TT_COMMA
             ):
                 errors.append(
                     UnexpectedToken(fname, ttoken.TT_COMMA, peek(index).ttype, (-1, -1))
                 )
```

### Comparing `peelpreter-1.0.1/src/peelpreter/token_type/__init__.py` & `peelpreter-1.1.2/src/peelpreter/token_type/__init__.py`

 * *Files identical despite different names*

### Comparing `peelpreter-1.0.1/src/peelpreter/token_type/token_type.py` & `peelpreter-1.1.2/src/peelpreter/token_type/token_type.py`

 * *Files identical despite different names*

