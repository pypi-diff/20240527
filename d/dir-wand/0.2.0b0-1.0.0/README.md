# Comparing `tmp/dir_wand-0.2.0b0.tar.gz` & `tmp/dir_wand-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dir_wand-0.2.0b0.tar", last modified: Sat May 25 11:35:39 2024, max compression
+gzip compressed data, was "dir_wand-1.0.0.tar", last modified: Mon May 27 16:38:30 2024, max compression
```

## Comparing `dir_wand-0.2.0b0.tar` & `dir_wand-1.0.0.tar`

### file list

```diff
@@ -1,39 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:35:39.261930 dir_wand-0.2.0b0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:35:39.257930 dir_wand-0.2.0b0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:35:39.257930 dir_wand-0.2.0b0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-25 11:35:28.000000 dir_wand-0.2.0b0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-25 11:35:28.000000 dir_wand-0.2.0b0/.github/workflows/python-app.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-25 11:35:28.000000 dir_wand-0.2.0b0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-25 11:35:28.000000 dir_wand-0.2.0b0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-25 11:35:28.000000 dir_wand-0.2.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    46320 2024-05-25 11:35:39.261930 dir_wand-0.2.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-25 11:35:28.000000 dir_wand-0.2.0b0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-25 11:35:28.000000 dir_wand-0.2.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 11:35:39.261930 dir_wand-0.2.0b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:35:39.257930 dir_wand-0.2.0b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:35:39.261930 dir_wand-0.2.0b0/src/dir_wand/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-25 11:35:39.000000 dir_wand-0.2.0b0/src/dir_wand/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-05-25 11:35:28.000000 dir_wand-0.2.0b0/src/dir_wand/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-05-25 11:35:28.000000 dir_wand-0.2.0b0/src/dir_wand/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-25 11:35:28.000000 dir_wand-0.2.0b0/src/dir_wand/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-25 11:35:28.000000 dir_wand-0.2.0b0/src/dir_wand/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-05-25 11:35:28.000000 dir_wand-0.2.0b0/src/dir_wand/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:35:39.261930 dir_wand-0.2.0b0/src/dir_wand.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    46320 2024-05-25 11:35:39.000000 dir_wand-0.2.0b0/src/dir_wand.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-25 11:35:39.000000 dir_wand-0.2.0b0/src/dir_wand.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 11:35:39.000000 dir_wand-0.2.0b0/src/dir_wand.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-25 11:35:39.000000 dir_wand-0.2.0b0/src/dir_wand.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-25 11:35:39.000000 dir_wand-0.2.0b0/src/dir_wand.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-25 11:35:39.000000 dir_wand-0.2.0b0/src/dir_wand.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:35:39.257930 dir_wand-0.2.0b0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:35:39.261930 dir_wand-0.2.0b0/tests/results/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-25 11:35:28.000000 dir_wand-0.2.0b0/tests/results/README
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:35:39.261930 dir_wand-0.2.0b0/tests/simple_test_{num}/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:35:39.261930 dir_wand-0.2.0b0/tests/simple_test_{num}/empty_dir/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-25 11:35:28.000000 dir_wand-0.2.0b0/tests/simple_test_{num}/empty_dir/README
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:35:39.261930 dir_wand-0.2.0b0/tests/simple_test_{num}/nested_dir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:35:39.257930 dir_wand-0.2.0b0/tests/simple_test_{num}/nested_dir/another_nested_dir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:35:39.261930 dir_wand-0.2.0b0/tests/simple_test_{num}/nested_dir/another_nested_dir/another_another_dir/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-25 11:35:28.000000 dir_wand-0.2.0b0/tests/simple_test_{num}/nested_dir/another_nested_dir/another_another_dir/nested_file.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-25 11:35:28.000000 dir_wand-0.2.0b0/tests/simple_test_{num}/nested_dir/text.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-25 11:35:28.000000 dir_wand-0.2.0b0/tests/simple_test_{num}/simple_test_{num}.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:38:30.790964 dir_wand-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:38:30.782964 dir_wand-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:38:30.786964 dir_wand-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-27 16:38:19.000000 dir_wand-1.0.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-27 16:38:19.000000 dir_wand-1.0.0/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-27 16:38:19.000000 dir_wand-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-27 16:38:19.000000 dir_wand-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 16:38:19.000000 dir_wand-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    51474 2024-05-27 16:38:30.790964 dir_wand-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9695 2024-05-27 16:38:19.000000 dir_wand-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-27 16:38:19.000000 dir_wand-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 16:38:30.790964 dir_wand-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:38:30.782964 dir_wand-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:38:30.786964 dir_wand-1.0.0/src/dir_wand/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-27 16:38:30.000000 dir_wand-1.0.0/src/dir_wand/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-27 16:38:19.000000 dir_wand-1.0.0/src/dir_wand/art.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-27 16:38:19.000000 dir_wand-1.0.0/src/dir_wand/command_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-05-27 16:38:19.000000 dir_wand-1.0.0/src/dir_wand/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-05-27 16:38:19.000000 dir_wand-1.0.0/src/dir_wand/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-05-27 16:38:19.000000 dir_wand-1.0.0/src/dir_wand/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-27 16:38:19.000000 dir_wand-1.0.0/src/dir_wand/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9753 2024-05-27 16:38:19.000000 dir_wand-1.0.0/src/dir_wand/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-27 16:38:19.000000 dir_wand-1.0.0/src/dir_wand/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-27 16:38:19.000000 dir_wand-1.0.0/src/dir_wand/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:38:30.790964 dir_wand-1.0.0/src/dir_wand.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    51474 2024-05-27 16:38:30.000000 dir_wand-1.0.0/src/dir_wand.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-27 16:38:30.000000 dir_wand-1.0.0/src/dir_wand.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:38:30.000000 dir_wand-1.0.0/src/dir_wand.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-27 16:38:30.000000 dir_wand-1.0.0/src/dir_wand.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-27 16:38:30.000000 dir_wand-1.0.0/src/dir_wand.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-27 16:38:30.000000 dir_wand-1.0.0/src/dir_wand.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:38:30.786964 dir_wand-1.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:38:30.786964 dir_wand-1.0.0/tests/results/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 16:38:19.000000 dir_wand-1.0.0/tests/results/README
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-27 16:38:19.000000 dir_wand-1.0.0/tests/simple_test_swaps.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:38:30.786964 dir_wand-1.0.0/tests/simple_test_{num}/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:38:30.786964 dir_wand-1.0.0/tests/simple_test_{num}/empty_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-27 16:38:19.000000 dir_wand-1.0.0/tests/simple_test_{num}/empty_dir/README
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:38:30.790964 dir_wand-1.0.0/tests/simple_test_{num}/nested_dir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:38:30.782964 dir_wand-1.0.0/tests/simple_test_{num}/nested_dir/another_nested_dir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:38:30.790964 dir_wand-1.0.0/tests/simple_test_{num}/nested_dir/another_nested_dir/another_another_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-27 16:38:19.000000 dir_wand-1.0.0/tests/simple_test_{num}/nested_dir/another_nested_dir/another_another_dir/nested_file.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-27 16:38:19.000000 dir_wand-1.0.0/tests/simple_test_{num}/nested_dir/text.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-27 16:38:19.000000 dir_wand-1.0.0/tests/simple_test_{num}/simple_test_{num}.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 16:38:19.000000 dir_wand-1.0.0/tests/test_flag.swaps
+-rw-r--r--   0 runner    (1001) docker     (127)    64349 2024-05-27 16:38:19.000000 dir_wand-1.0.0/wand-logo.jpg
```

### Comparing `dir_wand-0.2.0b0/.github/workflows/deploy.yml` & `dir_wand-1.0.0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `dir_wand-0.2.0b0/.gitignore` & `dir_wand-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dir_wand-0.2.0b0/.pre-commit-config.yaml` & `dir_wand-1.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dir_wand-0.2.0b0/LICENSE` & `dir_wand-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dir_wand-0.2.0b0/PKG-INFO` & `dir_wand-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dir-wand
-Version: 0.2.0b0
+Version: 1.0.0
 Summary: A CLI tool for making many directories from a template automagically.
 Author-email: Will Roper <w.roper@sussex.ac.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -694,23 +694,30 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyyaml
 Provides-Extra: dev
 Requires-Dist: ruff>=0.3.0; extra == "dev"
 
 # WAND: WAND Automates Nested Directories
 
 [![workflow](https://github.com/WillJRoper/dir-wand/actions/workflows/python-app.yml/badge.svg)](https://github.com/WillJRoper/dir-wand/actions)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![License: GPLv3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![PyPI version](https://badge.fury.io/py/dir-wand.svg)](https://badge.fury.io/py/dir-wand)
+
+<p align="center">
+  <img src="https://github.com/WillJRoper/dir-wand/assets/40025495/8ad6d775-c7e8-45df-88bd-21511d6ce6f1" alt="wand-logo" height="300">
+</p>
+
 
 WAND is a Python CLI tool for creating a large number of directories from a single template and executing commands globally throughout every directory.
 
 ## Installation
 
 To install WAND simply run
 
@@ -718,15 +725,19 @@
 pip install dir-wand
 ```
 
 in the root directory of WAND. This will install the `dir-wand` CLI. 
 
 ## Using WAND to make arbitrarily many directories
 
-To use WAND you first need have a template directory structure you want to make copies of. A template directory can include any number of subdirectories and files. WAND will correctly handle the copying of:
+WAND can efficiently make an arbitrary number of complex directory structures from a single template directory. This can be useful for creating a large number of directories with similar structures, such as for running many simulations, performance testing, or experiments. In the sections below we'll show how to create a template directory structure and use WAND to make copies of this structure with placeholders populated by a set of values.
+
+### Creating a template
+
+A template directory can include any number of subdirectories and files. WAND will correctly handle the copying of:
 
 - Empty directories.
 - Executables with the correct permissions.
 - Softlinks.
 - Human readable text files (e.g. `.txt`, `.yaml`, `.csv`, `.html`, etc.).
 - Binary files.
 - And many more...
@@ -755,25 +766,29 @@
   run_number:       {num}
   run_directory:    simple_example_{num}
   variable:         {x}
   another_variable: {y}
   some_flag:        {flag}
 ```
 
+where `num`, `x`, `y`, and `flag` are placeholders that will be replaced by values when making copies of the template directory.
+
+### Making copies
+
 To make copies of this template directory we can use the `dir-wand` CLI tool. `dir-wand` needs a set of values for each placeholder along with the path to the template directory, e.g.:
 
 ``` sh
-dir-wand simple_example_{num}/ --root /where/to/put/copies/ --num 0-2 --x 1-3 --y 2-4 -flag 0 1 0
+dir-wand --template simple_example_{num}/ --root /where/to/put/copies/ --num 0-2 --x 1-3 --y 2-4 -flag 0 1 0
 ```
 
-Here we've passed the filepath to the template directory (which can be an absolute or relative path), an optional root for the copies (if not given the copies will be made in the directory the command was run in) and a set of key-value pairs for each placeholder (of the form --key value). These values can be:
+Here we've passed the filepath to the template directory (which can be an absolute or relative path), an _optional_ root directory to contain the copies (if not given the copies will be made in the current working directory) and a set of key-value pairs for each placeholder (of the form --key value). These values can be:
 
 - The definition of an inclusive range using 2 dashes (e.g. `--num 0-2` will replace `num` with values of 0, 1, and 2).
 - A list of values using 1 dash (e.g. `-flag 0 1 0` will replace `flag` with 0, 1, and 0).
-- The path to a file containing a list of strings (Coming soon...).
+- The path to a file containing a list of strings using 2 dashes (for details see below).
 
 NOTE: The number of values for each placeholder must be the same. If not, WAND will raise an error.
 
 This will create 3 directories in `/where/to/put/copies/`:
 
 ```
 ├── simple_example_0/
@@ -811,10 +826,109 @@
   variable:         1
   another_variable: 2
   some_flag:        0
 ```
 
 with the other files made accordingly.
 
-## Running commands
+#### Using a file for values
+
+Rather than explicitly stating the values for a placeholder, you can pass the path to a file containing a list of values. For example, if we have a file `values.txt` containing values split by newlines,
+
+```
+0
+1
+0
+```
+
+we could instead pass this file to the flag argument,
+
+``` sh
+dir-wand --template simple_example_{num}/ --root /where/to/put/copies/ --num 0-2 --x 1-3 --y 2-4 --flag values.txt
+```
+
+which will create the same directories as before.
+
+### Using a swap file
+
+If you have a large number of placeholders or a large number of values for placeholders, it could be cumbersome to pass them all as arguments. Instead, you can pass a "swapfile", a yaml file defining the values to swap with each placeholder. If we have a swapfile `swapfile.yaml` containing:
+
+``` yaml
+num:
+  range: 0-2
+x:
+  list:
+    - 1
+    - 2
+    - 3
+y:
+  range: 2-4
+flag:
+  file: values.txt
+```
+
+we could instead pass this file to the `--swapfile` argument,
+
+``` sh
+dir-wand --template simple_example_{num}/ --root /where/to/put/copies/ --swapfile swapfile.yaml
+```
+
+ignoring the need to pass the placeholders as arguments explictly to get the same result as the calls detailed above. This not only makes working with a large number of placeholders easier but also allows for easy reuse of the same values across different runs.
+
+### Running commands after a copy
+
+When making copies of a template directory, WAND can also run commands in each directory. This can be done by passing the `--run` argument followed by the command to run wrapped by `"`. For example:
+
+``` sh
+dir-wand --template simple_example_{num}/ --root /where/to/put/copies/ --num 0-2 --x 1-3 --y 2-4 -flag 0 1 0 --run "echo 'Hello from simple_example_{num}'"
+```
+
+will create the directories as before and run the command `echo 'Hello from simple_example_{num}'` in each directory. This will output:
+
+```
+Hello from simple_example_0
+Hello from simple_example_1
+Hello from simple_example_2
+```
+
+These commands can be any valid shell command or even a script. The commands will be run on concurrent threads to ensure the main thread making the copies is not blocked so the world is your oyster!
+
+## Using WAND to run commands in existing directories
+
+WAND can also be used to run commands in existing directories with identical structures and "placeholder compliant" naming. 
+
+This can be done by passing the `--run` argument including placeholders and any required swaps (which can be defined in any of the ways detailed above including a swapfile). For example, if we assume the example template directory above is already made, where we have the directories (including all their contents):
+
+```
+├── simple_example_0/
+├── simple_example_1/
+└── simple_example_2/
+```
+
+Then we can run a command in each directory using:
+
+``` sh
+dir-wand --run "cd simple_example_{num}; head -2 simple_example_{num}.yaml" --num 0-2
+```
+
+This will output the first 2 lines of each `simple_example_{num}.yaml` file in each directory. Note that any command passed to `--run` will be run in the current working directory. 
+
+## Runtime arguments
+
+Invoking `dir-wand` with the `--help` flag (or not arguments at all) will display all possible options:
+
+```
+usage: dir-wand [-h] [--template TEMPLATE] [--root ROOT] [--run RUN] [--swapfile SWAPFILE] [--silent] [-- VALUE] [- VALUE [VALUE ...]]
+
+Wave your Directory WAND and make magic happen.
+
+options:
+  -h, --help           show this help message and exit
+  --template TEMPLATE  The template to use for the model.
+  --root ROOT          The root directory for the outputs.
+  --run RUN            A command to run in each copy once the copy is complete. The command will be run in the current working directory.
+  --swapfile SWAPFILE  A yaml file defining the swaps for each placeholder.
+  --silent             Suppress all WAND prints.
+  -- VALUE             A key-value pair for a placeholder replacement. Should be in the form --key value, where key is the name ({name}) to replace in directory paths and files, and value is an inclusive range (1-5), or a filepath to a file contain a list.of values.
+  - VALUE [VALUE ...]  A key-value pair for a placeholder replacement. Should be in the form -key value1 value2 value3, where key is the name ({name}) to replace in directory paths and files, and value is a list.
+```
 
-Coming soon...
```

### Comparing `dir_wand-0.2.0b0/pyproject.toml` & `dir_wand-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 ]
 readme = "README.md"
 license = { file = "LICENSE" }
 
 # Minimum Python version
 requires-python = ">=3.8"
 
-# No dependencies to run
-dependencies = []
+dependencies = ["pyyaml"]
 
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License (GPL)",
```

### Comparing `dir_wand-0.2.0b0/src/dir_wand/directory.py` & `dir_wand-1.0.0/src/dir_wand/directory.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,19 @@
         placeholder="value"
     )
 """
 
 import os
 
 from dir_wand.file import File
+from dir_wand.logger import Logger
+from dir_wand.utils import swap_in_str
+
+# Get the logger
+logger = Logger()
 
 
 class Directory:
     """
     A class for defining the directory.
 
     A directory is a tree structure containing files and other directories.
@@ -68,15 +73,15 @@
 
         Returns:
             str:
                 The string representation of the directory.
         """
         return self._str_helper()
 
-    def _str_helper(self, prefix="", is_last=True):
+    def _str_helper(self, prefix="  ", is_last=True):
         """
         Build the string representation with lines and indentation.
 
         Args:
             prefix (str):
                 The prefix to add to the string.
             is_last (bool):
@@ -147,30 +152,42 @@
             elif os.path.isfile(item_path):
                 # Create a new file instance
                 f = File(item_path)
 
                 # Add the file to the files
                 self.files.append(f)
 
+    @logger.count("directory")
+    def _make_dir_copy(self, path):
+        """
+        Make a copy of the directory.
+
+        Args:
+            path (str):
+                The path to the new directory.
+        """
+        os.makedirs(path, exist_ok=True)
+
     def make_copy_with_swaps(self, path, **swaps):
         """
         Make a copy of the directory with the placeholders swapped out.
 
         Args:
             path (str):
                 The path to the new directory.
             **swaps:
                 The placeholders to swap out.
         """
         # Get the new file path handling any possible placeholders
         path += "/" if not path.endswith("/") else ""
-        path = path + self.name.format(**swaps)
+        path = path + self.name
+        path = swap_in_str(path, **swaps)
 
         # Make the new directory
-        os.makedirs(path, exist_ok=True)
+        self._make_dir_copy(path)
 
         # Iterate over the files
         for file in self.files:
             # Make a copy of the file with the swaps
             file.make_copy_with_swaps(path, **swaps)
 
         # Iterate over the children
```

### Comparing `dir_wand-0.2.0b0/src/dir_wand/file.py` & `dir_wand-1.0.0/src/dir_wand/file.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,20 @@
     file.make_copy_with_swaps("path/to/new/file", placeholder="value")
 
 """
 
 import os
 import re
 
+from dir_wand.logger import Logger
+from dir_wand.utils import swap_in_str
+
+# Get the logger
+logger = Logger()
+
 
 class File:
     """
     A class for defining the file.
 
     A file contains all the information to make copies of a template file.
 
@@ -146,14 +152,75 @@
                 # Store the line index for later
                 self._place_holder_lines.append(index)
 
                 # Add the placeholders to the set
                 for match in matches:
                     self._placeholders.add(match)
 
+    @logger.count("file")
+    def _make_softlink_copy(self, path):
+        """Make a copy of a softlink."""
+        link = os.readlink(self.path)
+        os.symlink(link, path)
+
+    @logger.count("file")
+    def _make_executable_copy(self, path):
+        """Make a copy of an executable file."""
+        # Copy the file
+        with open(self.path, "rb") as file:
+            with open(path, "wb") as new_file:
+                new_file.write(file.read())
+
+        # Copy the permissions
+        os.chmod(path, os.stat(path).st_mode)
+
+    @logger.count("file")
+    def _make_simple_copy(self, path):
+        """Make a simple copy of a file."""
+        # Copy the file
+        with open(self.path, "rb") as file:
+            with open(path, "wb") as new_file:
+                new_file.write(file.read())
+
+    @logger.count("file")
+    def _make_copy_with_placeholders(self, path, **swaps):
+        """
+        Make a copy of the file with the placeholders swapped out.
+
+        This method will only work if the file has placeholders.
+
+        Args:
+            path (str):
+                The path to save the new file.
+            **swaps:
+                The placeholders to swap out.
+        """
+        # Ensure we have all the placeholders before we start swapping
+        missing = self._placeholders - set(swaps.keys())
+        if len(missing) > 0:
+            raise ValueError(f"Missing placeholders: {missing}")
+
+        # Open the file and read the lines
+        with open(self.path, "r") as file:
+            lines = file.readlines()
+
+        # Iterate over the lines and swap out the placeholders
+        for index in self._place_holder_lines:
+            # Get the line
+            line = lines[index]
+
+            line = swap_in_str(line, **swaps)
+
+            # Update the line
+            lines[index] = line
+
+        # Write the new file
+        with open(path, "w") as file:
+            file.writelines(lines)
+
     def make_copy_with_swaps(self, path, **swaps):
         """
         Make a copy of the file with the placeholders swapped out.
 
         This will correctly handle softlinks, executable files, and files
         with placeholders. If the file has placeholders, you must provide
         the values to swap out, otherwise an error will be raised.
@@ -162,60 +229,29 @@
             path (str):
                 The path to save the new file.
             **swaps:
                 The placeholders to swap out.
         """
         # Get the new file path handling any possible placeholders
         path += "/" if not path.endswith("/") else ""
-        path = path + self.name.format(**swaps)
+        path = path + self.name
+        path = swap_in_str(path, **swaps)
 
         # Before checking for swaps we might have a softlink, so we need to
         # copy the link
         if self.is_softlink:
-            link = os.readlink(self.path)
-            os.symlink(link, path)
+            self._make_softlink_copy(path)
             return
 
         # We might have an executable file, so we need to copy the permissions
         # and then the file
         if self.is_executable:
-            # Copy the file
-            with open(self.path, "rb") as file:
-                with open(path, "wb") as new_file:
-                    new_file.write(file.read())
-
-            # Copy the permissions
-            os.chmod(path, os.stat(path).st_mode)
+            self._make_executable_copy(path)
             return
 
         # We might only need to make a straight copy
         if not self.has_placeholders:
-            # Copy the file
-            with open(self.path, "rb") as file:
-                with open(path, "wb") as new_file:
-                    new_file.write(file.read())
+            self._make_simple_copy(path)
             return
 
         # OK, we dont have a simple case, lets handle the placeholders
-
-        # Ensure we have all the placeholders before we start swapping
-        missing = self._placeholders - set(swaps.keys())
-        if len(missing) > 0:
-            raise ValueError(f"Missing placeholders: {missing}")
-
-        # Open the file and read the lines
-        with open(self.path, "r") as file:
-            lines = file.readlines()
-
-        # Iterate over the lines and swap out the placeholders
-        for index in self._place_holder_lines:
-            # Get the line
-            line = lines[index]
-
-            line = line.format(**swaps)
-
-            # Update the line
-            lines[index] = line
-
-        # Write the new file
-        with open(path, "w") as file:
-            file.writelines(lines)
+        self._make_copy_with_placeholders(path, **swaps)
```

### Comparing `dir_wand-0.2.0b0/src/dir_wand/template.py` & `dir_wand-1.0.0/src/dir_wand/template.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     # Make copies of the template
     template.make_copies("path/to/new/template")
 
 """
 
 import os
 
+from dir_wand.command_runner import CommandRunner
 from dir_wand.directory import Directory
 
 
 class Template:
     """
     A class for defining the template.
 
@@ -37,92 +38,53 @@
             A dictionary of the swaps to make.
         nswap_vars (int):
             The number of swap variables.
         nswaps (int):
             The number of swaps to make.
     """
 
-    def __init__(self, root, **swaps):
+    def __init__(self, root, run=None, **swaps):
         """
         Create the template instance.
 
         Args:
             root (str):
                 The path to the root of the template.
+            run (str):
+                The command to run after the template is copied.
             **swaps (dict):
                 The swaps to make in the template.
         """
         # Attach a pointer to the root of the template
         self.root_path = root
         self.root = os.path.basename(root)
 
         # We will store the directory structure as a tree, by creating
         # the root we'll recursively collect the whole directory structure
         # including files
         self.directory = Directory(self.root_path)
         self.directory.unpack_contents()
 
-        # Print the directory structure
-        print("Template structure:")
-        print(self.directory)
-
         # Parse the swaps, we'll store these in a dictionary
-        self.swaps = self.parse_swaps(**swaps)
+        self.swaps = swaps
         self.nswap_vars = len(self.swaps)
         self.nswaps = len(list(self.swaps.values())[0])
 
+        # Store the run command (if not given this will be None)
+        self.run_cmd = CommandRunner(run) if run is not None else None
+
     def __str__(self):
         """
         Return the string representation of the template.
 
         Returns:
             str:
                 The string representation of the template.
         """
-        swaps = ", ".join(
-            f"{key}={value}" for key, value in self.swaps.items()
-        )
-        return (
-            f"Template(template_path={self.root_path},"
-            f" root={self.root}, swaps={swaps})"
-        )
-
-    def parse_swaps(self, **swaps):
-        """
-        Parse the swaps.
-
-        Args:
-            **swaps (dict):
-                The swaps to make in the template.
-
-        Raises:
-            ValueError:
-                If the number of swaps isn't equal between all placeholders.
-        """
-        for key, value in swaps.items():
-            # Do we have a list?
-            if isinstance(value, (list, tuple)):
-                swaps[key] = value
-
-            # Do we have the defintion of a range, i.e. 1-10?
-            elif "-" in value:
-                # Split the range
-                start, end = value.split("-")
-
-                # Convert the range to a dictionary
-                swaps[key] = list(range(int(start), int(end) + 1))
-            else:
-                raise ValueError(f"Invalid swap value: {value}")
-
-        # Ensure we have the same number of elements for all swaps
-        lengths = {len(value) for value in swaps.values()}
-        if len(lengths) > 1:
-            raise ValueError("All swaps must have the same number of elements")
-
-        return swaps
+        return f"Waving the directory WAND on {self.root_path}..."
 
     def make_copies(self, new_root):
         """
         Make copies of the template.
 
         This method is the main interface to copying the template. It will call
         the copy method of the template root directory, which will recursively
@@ -134,12 +96,38 @@
         """
         # Unpack all the swaps into each set of directories we'll need to make
         swaps = [
             {swap: self.swaps[swap][i] for swap in self.swaps}
             for i in range(self.nswaps)
         ]
 
+        print(f"Copying {self.root}...")
+
+        # Set up the header of the table we'll print
+        header = f" {'#':<5} "
+        for swap in self.swaps:
+            header += f" {swap:<20} "
+        print(header)
+        print("-" * len(header))
+
         # Loop over the swaps we'll have to make
-        for swap in swaps:
+        for i, swap in enumerate(swaps):
             # Make a copy of the root directory, this will recursively copy all
             # the files and directories handling the swaps
             self.directory.make_copy_with_swaps(new_root, **swap)
+
+            # Print the swap
+            line = f" {i:<5} "
+            for key in swap:
+                line += f" {swap[key]:<20} "
+            print(line)
+
+            # If we have a command to run, run it (this will be done on a
+            # concurrent thread so we don't block the main thread)
+            if self.run_cmd is not None:
+                self.run_cmd.run_command(**swap)
+
+        print("-" * len(header))
+
+        # Wait for the command threads before exiting if we need to
+        if self.run_cmd is not None:
+            self.run_cmd.wait_for_all()
```

### Comparing `dir_wand-0.2.0b0/src/dir_wand.egg-info/PKG-INFO` & `dir_wand-1.0.0/src/dir_wand.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dir-wand
-Version: 0.2.0b0
+Version: 1.0.0
 Summary: A CLI tool for making many directories from a template automagically.
 Author-email: Will Roper <w.roper@sussex.ac.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -694,23 +694,30 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyyaml
 Provides-Extra: dev
 Requires-Dist: ruff>=0.3.0; extra == "dev"
 
 # WAND: WAND Automates Nested Directories
 
 [![workflow](https://github.com/WillJRoper/dir-wand/actions/workflows/python-app.yml/badge.svg)](https://github.com/WillJRoper/dir-wand/actions)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![License: GPLv3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![PyPI version](https://badge.fury.io/py/dir-wand.svg)](https://badge.fury.io/py/dir-wand)
+
+<p align="center">
+  <img src="https://github.com/WillJRoper/dir-wand/assets/40025495/8ad6d775-c7e8-45df-88bd-21511d6ce6f1" alt="wand-logo" height="300">
+</p>
+
 
 WAND is a Python CLI tool for creating a large number of directories from a single template and executing commands globally throughout every directory.
 
 ## Installation
 
 To install WAND simply run
 
@@ -718,15 +725,19 @@
 pip install dir-wand
 ```
 
 in the root directory of WAND. This will install the `dir-wand` CLI. 
 
 ## Using WAND to make arbitrarily many directories
 
-To use WAND you first need have a template directory structure you want to make copies of. A template directory can include any number of subdirectories and files. WAND will correctly handle the copying of:
+WAND can efficiently make an arbitrary number of complex directory structures from a single template directory. This can be useful for creating a large number of directories with similar structures, such as for running many simulations, performance testing, or experiments. In the sections below we'll show how to create a template directory structure and use WAND to make copies of this structure with placeholders populated by a set of values.
+
+### Creating a template
+
+A template directory can include any number of subdirectories and files. WAND will correctly handle the copying of:
 
 - Empty directories.
 - Executables with the correct permissions.
 - Softlinks.
 - Human readable text files (e.g. `.txt`, `.yaml`, `.csv`, `.html`, etc.).
 - Binary files.
 - And many more...
@@ -755,25 +766,29 @@
   run_number:       {num}
   run_directory:    simple_example_{num}
   variable:         {x}
   another_variable: {y}
   some_flag:        {flag}
 ```
 
+where `num`, `x`, `y`, and `flag` are placeholders that will be replaced by values when making copies of the template directory.
+
+### Making copies
+
 To make copies of this template directory we can use the `dir-wand` CLI tool. `dir-wand` needs a set of values for each placeholder along with the path to the template directory, e.g.:
 
 ``` sh
-dir-wand simple_example_{num}/ --root /where/to/put/copies/ --num 0-2 --x 1-3 --y 2-4 -flag 0 1 0
+dir-wand --template simple_example_{num}/ --root /where/to/put/copies/ --num 0-2 --x 1-3 --y 2-4 -flag 0 1 0
 ```
 
-Here we've passed the filepath to the template directory (which can be an absolute or relative path), an optional root for the copies (if not given the copies will be made in the directory the command was run in) and a set of key-value pairs for each placeholder (of the form --key value). These values can be:
+Here we've passed the filepath to the template directory (which can be an absolute or relative path), an _optional_ root directory to contain the copies (if not given the copies will be made in the current working directory) and a set of key-value pairs for each placeholder (of the form --key value). These values can be:
 
 - The definition of an inclusive range using 2 dashes (e.g. `--num 0-2` will replace `num` with values of 0, 1, and 2).
 - A list of values using 1 dash (e.g. `-flag 0 1 0` will replace `flag` with 0, 1, and 0).
-- The path to a file containing a list of strings (Coming soon...).
+- The path to a file containing a list of strings using 2 dashes (for details see below).
 
 NOTE: The number of values for each placeholder must be the same. If not, WAND will raise an error.
 
 This will create 3 directories in `/where/to/put/copies/`:
 
 ```
 ├── simple_example_0/
@@ -811,10 +826,109 @@
   variable:         1
   another_variable: 2
   some_flag:        0
 ```
 
 with the other files made accordingly.
 
-## Running commands
+#### Using a file for values
+
+Rather than explicitly stating the values for a placeholder, you can pass the path to a file containing a list of values. For example, if we have a file `values.txt` containing values split by newlines,
+
+```
+0
+1
+0
+```
+
+we could instead pass this file to the flag argument,
+
+``` sh
+dir-wand --template simple_example_{num}/ --root /where/to/put/copies/ --num 0-2 --x 1-3 --y 2-4 --flag values.txt
+```
+
+which will create the same directories as before.
+
+### Using a swap file
+
+If you have a large number of placeholders or a large number of values for placeholders, it could be cumbersome to pass them all as arguments. Instead, you can pass a "swapfile", a yaml file defining the values to swap with each placeholder. If we have a swapfile `swapfile.yaml` containing:
+
+``` yaml
+num:
+  range: 0-2
+x:
+  list:
+    - 1
+    - 2
+    - 3
+y:
+  range: 2-4
+flag:
+  file: values.txt
+```
+
+we could instead pass this file to the `--swapfile` argument,
+
+``` sh
+dir-wand --template simple_example_{num}/ --root /where/to/put/copies/ --swapfile swapfile.yaml
+```
+
+ignoring the need to pass the placeholders as arguments explictly to get the same result as the calls detailed above. This not only makes working with a large number of placeholders easier but also allows for easy reuse of the same values across different runs.
+
+### Running commands after a copy
+
+When making copies of a template directory, WAND can also run commands in each directory. This can be done by passing the `--run` argument followed by the command to run wrapped by `"`. For example:
+
+``` sh
+dir-wand --template simple_example_{num}/ --root /where/to/put/copies/ --num 0-2 --x 1-3 --y 2-4 -flag 0 1 0 --run "echo 'Hello from simple_example_{num}'"
+```
+
+will create the directories as before and run the command `echo 'Hello from simple_example_{num}'` in each directory. This will output:
+
+```
+Hello from simple_example_0
+Hello from simple_example_1
+Hello from simple_example_2
+```
+
+These commands can be any valid shell command or even a script. The commands will be run on concurrent threads to ensure the main thread making the copies is not blocked so the world is your oyster!
+
+## Using WAND to run commands in existing directories
+
+WAND can also be used to run commands in existing directories with identical structures and "placeholder compliant" naming. 
+
+This can be done by passing the `--run` argument including placeholders and any required swaps (which can be defined in any of the ways detailed above including a swapfile). For example, if we assume the example template directory above is already made, where we have the directories (including all their contents):
+
+```
+├── simple_example_0/
+├── simple_example_1/
+└── simple_example_2/
+```
+
+Then we can run a command in each directory using:
+
+``` sh
+dir-wand --run "cd simple_example_{num}; head -2 simple_example_{num}.yaml" --num 0-2
+```
+
+This will output the first 2 lines of each `simple_example_{num}.yaml` file in each directory. Note that any command passed to `--run` will be run in the current working directory. 
+
+## Runtime arguments
+
+Invoking `dir-wand` with the `--help` flag (or not arguments at all) will display all possible options:
+
+```
+usage: dir-wand [-h] [--template TEMPLATE] [--root ROOT] [--run RUN] [--swapfile SWAPFILE] [--silent] [-- VALUE] [- VALUE [VALUE ...]]
+
+Wave your Directory WAND and make magic happen.
+
+options:
+  -h, --help           show this help message and exit
+  --template TEMPLATE  The template to use for the model.
+  --root ROOT          The root directory for the outputs.
+  --run RUN            A command to run in each copy once the copy is complete. The command will be run in the current working directory.
+  --swapfile SWAPFILE  A yaml file defining the swaps for each placeholder.
+  --silent             Suppress all WAND prints.
+  -- VALUE             A key-value pair for a placeholder replacement. Should be in the form --key value, where key is the name ({name}) to replace in directory paths and files, and value is an inclusive range (1-5), or a filepath to a file contain a list.of values.
+  - VALUE [VALUE ...]  A key-value pair for a placeholder replacement. Should be in the form -key value1 value2 value3, where key is the name ({name}) to replace in directory paths and files, and value is a list.
+```
 
-Coming soon...
```

### Comparing `dir_wand-0.2.0b0/src/dir_wand.egg-info/SOURCES.txt` & `dir_wand-1.0.0/src/dir_wand.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.md
 pyproject.toml
+wand-logo.jpg
 .github/workflows/deploy.yml
 .github/workflows/python-app.yml
 src/dir_wand/_version.py
+src/dir_wand/art.py
+src/dir_wand/command_runner.py
 src/dir_wand/directory.py
 src/dir_wand/file.py
+src/dir_wand/logger.py
 src/dir_wand/main.py
 src/dir_wand/parser.py
 src/dir_wand/template.py
+src/dir_wand/utils.py
 src/dir_wand.egg-info/PKG-INFO
 src/dir_wand.egg-info/SOURCES.txt
 src/dir_wand.egg-info/dependency_links.txt
 src/dir_wand.egg-info/entry_points.txt
 src/dir_wand.egg-info/requires.txt
 src/dir_wand.egg-info/top_level.txt
+tests/simple_test_swaps.yaml
+tests/test_flag.swaps
 tests/results/README
 tests/simple_test_{num}/simple_test_{num}.yaml
 tests/simple_test_{num}/empty_dir/README
 tests/simple_test_{num}/nested_dir/text.txt
 tests/simple_test_{num}/nested_dir/another_nested_dir/another_another_dir/nested_file.txt
```

