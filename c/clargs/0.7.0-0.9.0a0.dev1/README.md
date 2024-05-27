# Comparing `tmp/clargs-0.7.0.tar.gz` & `tmp/clargs-0.9.0a0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clargs-0.7.0.tar", last modified: Sun May 19 18:35:01 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `clargs-0.7.0.tar` & `clargs-0.9.0a0.dev1.tar`

### file list

```diff
@@ -1,37 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:35:01.090004 clargs-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:35:01.082004 clargs-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:35:01.086004 clargs-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-19 18:34:49.000000 clargs-0.7.0/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-19 18:34:49.000000 clargs-0.7.0/.github/workflows/upload.yml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-19 18:34:49.000000 clargs-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-19 18:34:49.000000 clargs-0.7.0/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-05-19 18:35:01.090004 clargs-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-05-19 18:34:49.000000 clargs-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:35:01.086004 clargs-0.7.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-19 18:34:49.000000 clargs-0.7.0/examples/0_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-19 18:34:49.000000 clargs-0.7.0/examples/1_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-19 18:34:49.000000 clargs-0.7.0/examples/2_show_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-19 18:34:49.000000 clargs-0.7.0/examples/3_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-05-19 18:34:49.000000 clargs-0.7.0/examples/4_parse_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    20370 2024-05-19 18:34:49.000000 clargs-0.7.0/examples/5_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-19 18:34:49.000000 clargs-0.7.0/examples/6_validation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1596 2024-05-19 18:34:49.000000 clargs-0.7.0/examples/__generate_example_output__.sh
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-19 18:34:49.000000 clargs-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 18:35:01.090004 clargs-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:35:01.086004 clargs-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:35:01.090004 clargs-0.7.0/src/clargs/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-19 18:34:49.000000 clargs-0.7.0/src/clargs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9530 2024-05-19 18:34:49.000000 clargs-0.7.0/src/clargs/aap_from_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-05-19 18:34:49.000000 clargs-0.7.0/src/clargs/clargs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-19 18:34:49.000000 clargs-0.7.0/src/clargs/docsparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-19 18:34:49.000000 clargs-0.7.0/src/clargs/helper_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:35:01.090004 clargs-0.7.0/src/clargs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-05-19 18:35:01.000000 clargs-0.7.0/src/clargs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-19 18:35:01.000000 clargs-0.7.0/src/clargs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:35:01.000000 clargs-0.7.0/src/clargs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 18:35:01.000000 clargs-0.7.0/src/clargs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:35:01.090004 clargs-0.7.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-05-19 18:34:49.000000 clargs-0.7.0/test/test_docsparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    26301 2024-05-19 18:34:49.000000 clargs-0.7.0/test/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-19 18:34:49.000000 clargs-0.7.0/test/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-19 18:34:49.000000 clargs-0.7.0/tox.ini
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/.github/workflows/run-tests-and-build.yml
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/examples/0_basic.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/examples/1_flags.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/examples/2_show_defaults.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/examples/3_list.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/examples/4_parse_groups.py
+-rw-r--r--   0        0        0    20371 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/examples/5_logging.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/examples/6_validation.py
+-rwxr-xr-x   0        0        0     1986 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/examples/__generate_example_output__.sh
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/src/clargs/__about__.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/src/clargs/__init__.py
+-rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/src/clargs/aap_from_data.py
+-rw-r--r--   0        0        0    10061 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/src/clargs/clargs.py
+-rw-r--r--   0        0        0     5585 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/src/clargs/docsparser.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/src/clargs/helper_types.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/tests/__init__.py
+-rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/tests/test_docsparser.py
+-rw-r--r--   0        0        0    26301 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/tests/test_simple.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/tests/test_validation.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/LICENSE.txt
+-rw-r--r--   0        0        0     8880 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/README.md
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     9840 2020-02-02 00:00:00.000000 clargs-0.9.0a0.dev1/PKG-INFO
```

### Comparing `clargs-0.7.0/LICENCE.txt` & `clargs-0.9.0a0.dev1/LICENSE.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,9 @@
 MIT License
 
-Copyright (c) [year] [fullname]
+Copyright (c) 2023-present Claude <pypi@claude.nl>
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE!.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `clargs-0.7.0/PKG-INFO` & `clargs-0.9.0a0.dev1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,15 @@
-Metadata-Version: 2.1
-Name: clargs
-Version: 0.7.0
-Summary: Easily generate commandline apps from your functions, based on type hints
-Author-email: Claude <pypi@claude.nl>
-Project-URL: Homepage, https://github.com/reinhrst/clargs
-Project-URL: Bug Tracker, https://github.com/reinhrst/clargs/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENCE.txt
+# clargs
 
-# Clargs
+[![PyPI - Version](https://img.shields.io/pypi/v/clargs.svg)](https://pypi.org/project/clargs)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/clargs.svg)](https://pypi.org/project/clargs)
+![Tests](https://github.com/reinhrst/clargs/workflows/Run%20package%20tests/badge.svg)
+-----
 
-The goal of the `clargs` package is to create commandline interfaces from function signatures.
+The goal of the `clargs` package is to create command-line interfaces from function signatures.
 
 - **Hit the ground running**: With a single line, an existing function is turned into a command line program
 - **Extensible**: It is flexible enough to do everything that `argparse` does, and keeps you in control
 - **No magic**: All the extension does is call commands in `argparse`; you can log and see these commands
 - **Safe**: The built-in python `argparse` module does all the work, so safety guarantees from that module apply
 - **Typing**: Parameter types are set as [PEP 484][2] type hints (e.g. `def foo(bar: int)`)
 - **Standard**: By using `argparse`, you get standard behaviour such as long/short parameters, combine flags, help function
@@ -219,7 +210,11 @@
 
 
 [2]: https://peps.python.org/pep-0484/
 [3]: https://github.com/reinhrst/clargs/tree/main/examples/
 [4]: https://github.com/reinhrst/clargs/tree/main/examples/4_parse_groups.py
 [5]: https://github.com/reinhrst/clargs/tree/main/examples/5_logging.py
 [6]: https://github.com/reinhrst/clargs/tree/main/examples/6_validation.py
+
+## License
+
+`clargs` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `clargs-0.7.0/README.md` & `clargs-0.9.0a0.dev1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,37 @@
-# Clargs
+Metadata-Version: 2.3
+Name: clargs
+Version: 0.9.0a0.dev1
+Summary: Easily generate commandline apps from your functions, based on type hints
+Project-URL: Documentation, https://github.com/reinhrst/clargs#readme
+Project-URL: Issues, https://github.com/reinhrst/clargs/issues
+Project-URL: Source, https://github.com/reinhrst/clargs
+Author-email: Claude <pypi@claude.nl>
+License-Expression: MIT
+License-File: LICENSE.txt
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+
+# clargs
+
+[![PyPI - Version](https://img.shields.io/pypi/v/clargs.svg)](https://pypi.org/project/clargs)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/clargs.svg)](https://pypi.org/project/clargs)
+![Tests](https://github.com/reinhrst/clargs/workflows/Run%20package%20tests/badge.svg)
+-----
 
-The goal of the `clargs` package is to create commandline interfaces from function signatures.
+The goal of the `clargs` package is to create command-line interfaces from function signatures.
 
 - **Hit the ground running**: With a single line, an existing function is turned into a command line program
 - **Extensible**: It is flexible enough to do everything that `argparse` does, and keeps you in control
 - **No magic**: All the extension does is call commands in `argparse`; you can log and see these commands
 - **Safe**: The built-in python `argparse` module does all the work, so safety guarantees from that module apply
 - **Typing**: Parameter types are set as [PEP 484][2] type hints (e.g. `def foo(bar: int)`)
 - **Standard**: By using `argparse`, you get standard behaviour such as long/short parameters, combine flags, help function
@@ -205,7 +232,11 @@
 
 
 [2]: https://peps.python.org/pep-0484/
 [3]: https://github.com/reinhrst/clargs/tree/main/examples/
 [4]: https://github.com/reinhrst/clargs/tree/main/examples/4_parse_groups.py
 [5]: https://github.com/reinhrst/clargs/tree/main/examples/5_logging.py
 [6]: https://github.com/reinhrst/clargs/tree/main/examples/6_validation.py
+
+## License
+
+`clargs` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `clargs-0.7.0/examples/0_basic.py` & `clargs-0.9.0a0.dev1/examples/0_basic.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 1 HUMAN
 2 HUMANS
 3 HUMANS
 4 HUMANS
 5 HUMANS
 
 """
+
 import clargs
 
 
 def count(
     singular: str,
     plural: str,
     maxitems: int = 10,
```

### Comparing `clargs-0.7.0/examples/1_flags.py` & `clargs-0.9.0a0.dev1/examples/1_flags.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 5 Humans
 
 >>> python examples/1_flags.py Human Humans 5 --shout=yes (returncode: 2)
 usage: 1_flags.py [-h] [--shout | --no-shout | -s] singular plural [maxitems]
 1_flags.py: error: argument --shout/--no-shout/-s: ignored explicit argument 'yes'
 
 """
+
 import clargs
 
 
 def count(
     singular: str,
     plural: str,
     maxitems: int = 10,
```

### Comparing `clargs-0.7.0/examples/2_show_defaults.py` & `clargs-0.9.0a0.dev1/examples/2_show_defaults.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 options:
   -h, --help            show this help message and exit
   --shout, --no-shout, -s
                         If True, will convert all expressions to capitals
                         (default: False)
 
 """
+
 import argparse
 import clargs
 
 
 def count(
     singular: str,
     plural: str,
```

### Comparing `clargs-0.7.0/examples/3_list.py` & `clargs-0.9.0a0.dev1/examples/3_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 
 >>> python examples/3_list.py Alien Aliens 2 2 --no-shout (returncode: 2)
 usage: 3_list.py [-h] [--shout | --no-shout | -s]
                  {Human,Horse,Sheep} {Humans,Horses,Sheep} [maxitems ...]
 3_list.py: error: argument singular: invalid choice: 'Alien' (choose from 'Human', 'Horse', 'Sheep')
 
 """
+
 import argparse
 import clargs
 import typing as t
 
 
 def count(
     # Limit the choices for singular and plural
```

### Comparing `clargs-0.7.0/examples/4_parse_groups.py` & `clargs-0.9.0a0.dev1/examples/4_parse_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 >>> python examples/4_parse_groups.py math add # Number is required now since type is ListOfAtLeastOne (returncode: 2)
 usage: 4_parse_groups.py math [-h] [--round-to-int | --no-round-to-int | -r]
                               [--absolute-value | --no-absolute-value | -a]
                               {add,mul,sub,truediv} numbers [numbers ...]
 4_parse_groups.py math: error: the following arguments are required: numbers
 
 """
+
 import argparse
 import clargs
 import operator as mod_operator
 import typing as t
 
 
 def count(
```

### Comparing `clargs-0.7.0/examples/5_logging.py` & `clargs-0.9.0a0.dev1/examples/5_logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """
 Examples:
 
 >>> python examples/5_logging.py --help (returncode: 0)
 DEBUG:clargs:Adding (['singular'], {'choices': ('Human', 'Horse', 'Sheep'), 'help': 'The singular form of the thing to count', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['plural'], {'choices': ('Humans', 'Horses', 'Sheep'), 'help': 'The plural form of the thing to count', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['maxitems'], {'action': 'extend', 'help': 'A list of numbers to count to', 'nargs': '*', 'type': <class 'int'>})
-DEBUG:clargs:Adding (['--shout', '-s'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x100d7a5c0>, 'default': None, 'help': 'If True, will convert all expressions to capitals', 'required': False})
+DEBUG:clargs:Adding (['--shout', '-s'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': None, 'help': 'If True, will convert all expressions to capitals', 'required': False})
 DEBUG:clargs:Adding (['operator'], {'choices': ('add', 'mul', 'sub', 'truediv'), 'help': 'Add, Multiply, Subtract or Divide', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['numbers'], {'action': 'extend', 'help': 'List of numbers to operate on', 'nargs': '+', 'type': <class 'float'>})
-DEBUG:clargs:Adding (['--round-to-int', '-r'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x100d7a5c0>, 'default': False, 'help': 'If True, the result will be round to closest int', 'required': False})
-DEBUG:clargs:Adding (['--absolute-value', '-a'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x100d7a5c0>, 'default': False, 'help': 'If True, the result will be made positive', 'required': False})
+DEBUG:clargs:Adding (['--round-to-int', '-r'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': False, 'help': 'If True, the result will be round to closest int', 'required': False})
+DEBUG:clargs:Adding (['--absolute-value', '-a'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': False, 'help': 'If True, the result will be made positive', 'required': False})
 usage: 5_logging.py [-h] {count,math} ...
 
 positional arguments:
   {count,math}
     count       Counts from 1 to given number (default = 10)
     math        Does math on the list of numbers, based on the first term
 
 options:
   -h, --help    show this help message and exit
 
 >>> python examples/5_logging.py count --help (returncode: 0)
 DEBUG:clargs:Adding (['singular'], {'choices': ('Human', 'Horse', 'Sheep'), 'help': 'The singular form of the thing to count', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['plural'], {'choices': ('Humans', 'Horses', 'Sheep'), 'help': 'The plural form of the thing to count', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['maxitems'], {'action': 'extend', 'help': 'A list of numbers to count to', 'nargs': '*', 'type': <class 'int'>})
-DEBUG:clargs:Adding (['--shout', '-s'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x1011725c0>, 'default': None, 'help': 'If True, will convert all expressions to capitals', 'required': False})
+DEBUG:clargs:Adding (['--shout', '-s'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': None, 'help': 'If True, will convert all expressions to capitals', 'required': False})
 DEBUG:clargs:Adding (['operator'], {'choices': ('add', 'mul', 'sub', 'truediv'), 'help': 'Add, Multiply, Subtract or Divide', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['numbers'], {'action': 'extend', 'help': 'List of numbers to operate on', 'nargs': '+', 'type': <class 'float'>})
-DEBUG:clargs:Adding (['--round-to-int', '-r'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x1011725c0>, 'default': False, 'help': 'If True, the result will be round to closest int', 'required': False})
-DEBUG:clargs:Adding (['--absolute-value', '-a'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x1011725c0>, 'default': False, 'help': 'If True, the result will be made positive', 'required': False})
+DEBUG:clargs:Adding (['--round-to-int', '-r'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': False, 'help': 'If True, the result will be round to closest int', 'required': False})
+DEBUG:clargs:Adding (['--absolute-value', '-a'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': False, 'help': 'If True, the result will be made positive', 'required': False})
 usage: 5_logging.py count [-h] [--shout | --no-shout | -s]
                           {Human,Horse,Sheep} {Humans,Horses,Sheep}
                           [maxitems ...]
 
 positional arguments:
   {Human,Horse,Sheep}   The singular form of the thing to count
   {Humans,Horses,Sheep}
@@ -44,19 +44,19 @@
   --shout, --no-shout, -s
                         If True, will convert all expressions to capitals
 
 >>> python examples/5_logging.py math --help (returncode: 0)
 DEBUG:clargs:Adding (['singular'], {'choices': ('Human', 'Horse', 'Sheep'), 'help': 'The singular form of the thing to count', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['plural'], {'choices': ('Humans', 'Horses', 'Sheep'), 'help': 'The plural form of the thing to count', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['maxitems'], {'action': 'extend', 'help': 'A list of numbers to count to', 'nargs': '*', 'type': <class 'int'>})
-DEBUG:clargs:Adding (['--shout', '-s'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x102d8a5c0>, 'default': None, 'help': 'If True, will convert all expressions to capitals', 'required': False})
+DEBUG:clargs:Adding (['--shout', '-s'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': None, 'help': 'If True, will convert all expressions to capitals', 'required': False})
 DEBUG:clargs:Adding (['operator'], {'choices': ('add', 'mul', 'sub', 'truediv'), 'help': 'Add, Multiply, Subtract or Divide', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['numbers'], {'action': 'extend', 'help': 'List of numbers to operate on', 'nargs': '+', 'type': <class 'float'>})
-DEBUG:clargs:Adding (['--round-to-int', '-r'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x102d8a5c0>, 'default': False, 'help': 'If True, the result will be round to closest int', 'required': False})
-DEBUG:clargs:Adding (['--absolute-value', '-a'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x102d8a5c0>, 'default': False, 'help': 'If True, the result will be made positive', 'required': False})
+DEBUG:clargs:Adding (['--round-to-int', '-r'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': False, 'help': 'If True, the result will be round to closest int', 'required': False})
+DEBUG:clargs:Adding (['--absolute-value', '-a'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': False, 'help': 'If True, the result will be made positive', 'required': False})
 usage: 5_logging.py math [-h] [--round-to-int | --no-round-to-int | -r]
                          [--absolute-value | --no-absolute-value | -a]
                          {add,mul,sub,truediv} numbers [numbers ...]
 
 positional arguments:
   {add,mul,sub,truediv}
                         Add, Multiply, Subtract or Divide
@@ -69,99 +69,100 @@
   --absolute-value, --no-absolute-value, -a
                         If True, the result will be made positive
 
 >>> python examples/5_logging.py count Human Humans 2 (returncode: 0)
 DEBUG:clargs:Adding (['singular'], {'choices': ('Human', 'Horse', 'Sheep'), 'help': 'The singular form of the thing to count', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['plural'], {'choices': ('Humans', 'Horses', 'Sheep'), 'help': 'The plural form of the thing to count', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['maxitems'], {'action': 'extend', 'help': 'A list of numbers to count to', 'nargs': '*', 'type': <class 'int'>})
-DEBUG:clargs:Adding (['--shout', '-s'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x102c025c0>, 'default': None, 'help': 'If True, will convert all expressions to capitals', 'required': False})
+DEBUG:clargs:Adding (['--shout', '-s'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': None, 'help': 'If True, will convert all expressions to capitals', 'required': False})
 DEBUG:clargs:Adding (['operator'], {'choices': ('add', 'mul', 'sub', 'truediv'), 'help': 'Add, Multiply, Subtract or Divide', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['numbers'], {'action': 'extend', 'help': 'List of numbers to operate on', 'nargs': '+', 'type': <class 'float'>})
-DEBUG:clargs:Adding (['--round-to-int', '-r'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x102c025c0>, 'default': False, 'help': 'If True, the result will be round to closest int', 'required': False})
-DEBUG:clargs:Adding (['--absolute-value', '-a'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x102c025c0>, 'default': False, 'help': 'If True, the result will be made positive', 'required': False})
-DEBUG:clargs:Received parsed args Namespace(singular='Human', plural='Humans', maxitems=[2], shout=None, _clargs_func_=<function count at 0x10243e020>)
+DEBUG:clargs:Adding (['--round-to-int', '-r'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': False, 'help': 'If True, the result will be round to closest int', 'required': False})
+DEBUG:clargs:Adding (['--absolute-value', '-a'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': False, 'help': 'If True, the result will be made positive', 'required': False})
+DEBUG:clargs:Received parsed args Namespace(singular='Human', plural='Humans', maxitems=[2], shout=None, _clargs_func_=<function count at 0xXXXXXXXXX>)
 maxitems: [2]
 1 Human
 2 Humans
 
 >>> python examples/5_logging.py count Human Humans # normal list may have size 0 (returncode: 0)
 DEBUG:clargs:Adding (['singular'], {'choices': ('Human', 'Horse', 'Sheep'), 'help': 'The singular form of the thing to count', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['plural'], {'choices': ('Humans', 'Horses', 'Sheep'), 'help': 'The plural form of the thing to count', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['maxitems'], {'action': 'extend', 'help': 'A list of numbers to count to', 'nargs': '*', 'type': <class 'int'>})
-DEBUG:clargs:Adding (['--shout', '-s'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x10386e5c0>, 'default': None, 'help': 'If True, will convert all expressions to capitals', 'required': False})
+DEBUG:clargs:Adding (['--shout', '-s'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': None, 'help': 'If True, will convert all expressions to capitals', 'required': False})
 DEBUG:clargs:Adding (['operator'], {'choices': ('add', 'mul', 'sub', 'truediv'), 'help': 'Add, Multiply, Subtract or Divide', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['numbers'], {'action': 'extend', 'help': 'List of numbers to operate on', 'nargs': '+', 'type': <class 'float'>})
-DEBUG:clargs:Adding (['--round-to-int', '-r'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x10386e5c0>, 'default': False, 'help': 'If True, the result will be round to closest int', 'required': False})
-DEBUG:clargs:Adding (['--absolute-value', '-a'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x10386e5c0>, 'default': False, 'help': 'If True, the result will be made positive', 'required': False})
-DEBUG:clargs:Received parsed args Namespace(singular='Human', plural='Humans', maxitems=[], shout=None, _clargs_func_=<function count at 0x1030aa020>)
+DEBUG:clargs:Adding (['--round-to-int', '-r'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': False, 'help': 'If True, the result will be round to closest int', 'required': False})
+DEBUG:clargs:Adding (['--absolute-value', '-a'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': False, 'help': 'If True, the result will be made positive', 'required': False})
+DEBUG:clargs:Received parsed args Namespace(singular='Human', plural='Humans', maxitems=[], shout=None, _clargs_func_=<function count at 0xXXXXXXXXX>)
 maxitems: []
 
 >>> python examples/5_logging.py math add 10 20 6 3 2 1 --round # argparse allows you to shorten parameters (returncode: 0)
 DEBUG:clargs:Adding (['singular'], {'choices': ('Human', 'Horse', 'Sheep'), 'help': 'The singular form of the thing to count', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['plural'], {'choices': ('Humans', 'Horses', 'Sheep'), 'help': 'The plural form of the thing to count', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['maxitems'], {'action': 'extend', 'help': 'A list of numbers to count to', 'nargs': '*', 'type': <class 'int'>})
-DEBUG:clargs:Adding (['--shout', '-s'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x103a125c0>, 'default': None, 'help': 'If True, will convert all expressions to capitals', 'required': False})
+DEBUG:clargs:Adding (['--shout', '-s'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': None, 'help': 'If True, will convert all expressions to capitals', 'required': False})
 DEBUG:clargs:Adding (['operator'], {'choices': ('add', 'mul', 'sub', 'truediv'), 'help': 'Add, Multiply, Subtract or Divide', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['numbers'], {'action': 'extend', 'help': 'List of numbers to operate on', 'nargs': '+', 'type': <class 'float'>})
-DEBUG:clargs:Adding (['--round-to-int', '-r'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x103a125c0>, 'default': False, 'help': 'If True, the result will be round to closest int', 'required': False})
-DEBUG:clargs:Adding (['--absolute-value', '-a'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x103a125c0>, 'default': False, 'help': 'If True, the result will be made positive', 'required': False})
-DEBUG:clargs:Received parsed args Namespace(operator='add', numbers=[10.0, 20.0, 6.0, 3.0, 2.0, 1.0], round_to_int=True, absolute_value=False, _clargs_func_=<function math at 0x1034a9300>)
+DEBUG:clargs:Adding (['--round-to-int', '-r'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': False, 'help': 'If True, the result will be round to closest int', 'required': False})
+DEBUG:clargs:Adding (['--absolute-value', '-a'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': False, 'help': 'If True, the result will be made positive', 'required': False})
+DEBUG:clargs:Received parsed args Namespace(operator='add', numbers=[10.0, 20.0, 6.0, 3.0, 2.0, 1.0], round_to_int=True, absolute_value=False, _clargs_func_=<function math at 0xXXXXXXXXX>)
 Result: 42
 
 >>> python examples/5_logging.py math sub 10 20 6 3 2 1 --abs (returncode: 0)
 DEBUG:clargs:Adding (['singular'], {'choices': ('Human', 'Horse', 'Sheep'), 'help': 'The singular form of the thing to count', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['plural'], {'choices': ('Humans', 'Horses', 'Sheep'), 'help': 'The plural form of the thing to count', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['maxitems'], {'action': 'extend', 'help': 'A list of numbers to count to', 'nargs': '*', 'type': <class 'int'>})
-DEBUG:clargs:Adding (['--shout', '-s'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x1037ba5c0>, 'default': None, 'help': 'If True, will convert all expressions to capitals', 'required': False})
+DEBUG:clargs:Adding (['--shout', '-s'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': None, 'help': 'If True, will convert all expressions to capitals', 'required': False})
 DEBUG:clargs:Adding (['operator'], {'choices': ('add', 'mul', 'sub', 'truediv'), 'help': 'Add, Multiply, Subtract or Divide', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['numbers'], {'action': 'extend', 'help': 'List of numbers to operate on', 'nargs': '+', 'type': <class 'float'>})
-DEBUG:clargs:Adding (['--round-to-int', '-r'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x1037ba5c0>, 'default': False, 'help': 'If True, the result will be round to closest int', 'required': False})
-DEBUG:clargs:Adding (['--absolute-value', '-a'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x1037ba5c0>, 'default': False, 'help': 'If True, the result will be made positive', 'required': False})
-DEBUG:clargs:Received parsed args Namespace(operator='sub', numbers=[10.0, 20.0, 6.0, 3.0, 2.0, 1.0], round_to_int=False, absolute_value=True, _clargs_func_=<function math at 0x103251300>)
+DEBUG:clargs:Adding (['--round-to-int', '-r'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': False, 'help': 'If True, the result will be round to closest int', 'required': False})
+DEBUG:clargs:Adding (['--absolute-value', '-a'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': False, 'help': 'If True, the result will be made positive', 'required': False})
+DEBUG:clargs:Received parsed args Namespace(operator='sub', numbers=[10.0, 20.0, 6.0, 3.0, 2.0, 1.0], round_to_int=False, absolute_value=True, _clargs_func_=<function math at 0xXXXXXXXXX>)
 Result: 22.0
 
 >>> python examples/5_logging.py math truediv 50 -3 (returncode: 0)
 DEBUG:clargs:Adding (['singular'], {'choices': ('Human', 'Horse', 'Sheep'), 'help': 'The singular form of the thing to count', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['plural'], {'choices': ('Humans', 'Horses', 'Sheep'), 'help': 'The plural form of the thing to count', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['maxitems'], {'action': 'extend', 'help': 'A list of numbers to count to', 'nargs': '*', 'type': <class 'int'>})
-DEBUG:clargs:Adding (['--shout', '-s'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x102e3e5c0>, 'default': None, 'help': 'If True, will convert all expressions to capitals', 'required': False})
+DEBUG:clargs:Adding (['--shout', '-s'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': None, 'help': 'If True, will convert all expressions to capitals', 'required': False})
 DEBUG:clargs:Adding (['operator'], {'choices': ('add', 'mul', 'sub', 'truediv'), 'help': 'Add, Multiply, Subtract or Divide', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['numbers'], {'action': 'extend', 'help': 'List of numbers to operate on', 'nargs': '+', 'type': <class 'float'>})
-DEBUG:clargs:Adding (['--round-to-int', '-r'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x102e3e5c0>, 'default': False, 'help': 'If True, the result will be round to closest int', 'required': False})
-DEBUG:clargs:Adding (['--absolute-value', '-a'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x102e3e5c0>, 'default': False, 'help': 'If True, the result will be made positive', 'required': False})
-DEBUG:clargs:Received parsed args Namespace(operator='truediv', numbers=[50.0, -3.0], round_to_int=False, absolute_value=False, _clargs_func_=<function math at 0x1028d5300>)
+DEBUG:clargs:Adding (['--round-to-int', '-r'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': False, 'help': 'If True, the result will be round to closest int', 'required': False})
+DEBUG:clargs:Adding (['--absolute-value', '-a'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': False, 'help': 'If True, the result will be made positive', 'required': False})
+DEBUG:clargs:Received parsed args Namespace(operator='truediv', numbers=[50.0, -3.0], round_to_int=False, absolute_value=False, _clargs_func_=<function math at 0xXXXXXXXXX>)
 Result: -16.666666666666668
 
 >>> python examples/5_logging.py math truediv 50 -3 -ra # -r is --round-to-int and -a is --absolute-value; you can combine them into -ra (returncode: 0)
 DEBUG:clargs:Adding (['singular'], {'choices': ('Human', 'Horse', 'Sheep'), 'help': 'The singular form of the thing to count', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['plural'], {'choices': ('Humans', 'Horses', 'Sheep'), 'help': 'The plural form of the thing to count', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['maxitems'], {'action': 'extend', 'help': 'A list of numbers to count to', 'nargs': '*', 'type': <class 'int'>})
-DEBUG:clargs:Adding (['--shout', '-s'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x1059d25c0>, 'default': None, 'help': 'If True, will convert all expressions to capitals', 'required': False})
+DEBUG:clargs:Adding (['--shout', '-s'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': None, 'help': 'If True, will convert all expressions to capitals', 'required': False})
 DEBUG:clargs:Adding (['operator'], {'choices': ('add', 'mul', 'sub', 'truediv'), 'help': 'Add, Multiply, Subtract or Divide', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['numbers'], {'action': 'extend', 'help': 'List of numbers to operate on', 'nargs': '+', 'type': <class 'float'>})
-DEBUG:clargs:Adding (['--round-to-int', '-r'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x1059d25c0>, 'default': False, 'help': 'If True, the result will be round to closest int', 'required': False})
-DEBUG:clargs:Adding (['--absolute-value', '-a'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x1059d25c0>, 'default': False, 'help': 'If True, the result will be made positive', 'required': False})
-DEBUG:clargs:Received parsed args Namespace(operator='truediv', numbers=[50.0, -3.0], round_to_int=True, absolute_value=True, _clargs_func_=<function math at 0x105469300>)
+DEBUG:clargs:Adding (['--round-to-int', '-r'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': False, 'help': 'If True, the result will be round to closest int', 'required': False})
+DEBUG:clargs:Adding (['--absolute-value', '-a'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': False, 'help': 'If True, the result will be made positive', 'required': False})
+DEBUG:clargs:Received parsed args Namespace(operator='truediv', numbers=[50.0, -3.0], round_to_int=True, absolute_value=True, _clargs_func_=<function math at 0xXXXXXXXXX>)
 Result: 17
 
 >>> python examples/5_logging.py math add # Number is required now since type is ListOfAtLeastOne (returncode: 2)
 DEBUG:clargs:Adding (['singular'], {'choices': ('Human', 'Horse', 'Sheep'), 'help': 'The singular form of the thing to count', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['plural'], {'choices': ('Humans', 'Horses', 'Sheep'), 'help': 'The plural form of the thing to count', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['maxitems'], {'action': 'extend', 'help': 'A list of numbers to count to', 'nargs': '*', 'type': <class 'int'>})
-DEBUG:clargs:Adding (['--shout', '-s'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x1032de5c0>, 'default': None, 'help': 'If True, will convert all expressions to capitals', 'required': False})
+DEBUG:clargs:Adding (['--shout', '-s'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': None, 'help': 'If True, will convert all expressions to capitals', 'required': False})
 DEBUG:clargs:Adding (['operator'], {'choices': ('add', 'mul', 'sub', 'truediv'), 'help': 'Add, Multiply, Subtract or Divide', 'type': <class 'str'>})
 DEBUG:clargs:Adding (['numbers'], {'action': 'extend', 'help': 'List of numbers to operate on', 'nargs': '+', 'type': <class 'float'>})
-DEBUG:clargs:Adding (['--round-to-int', '-r'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x1032de5c0>, 'default': False, 'help': 'If True, the result will be round to closest int', 'required': False})
-DEBUG:clargs:Adding (['--absolute-value', '-a'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0x1032de5c0>, 'default': False, 'help': 'If True, the result will be made positive', 'required': False})
+DEBUG:clargs:Adding (['--round-to-int', '-r'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': False, 'help': 'If True, the result will be round to closest int', 'required': False})
+DEBUG:clargs:Adding (['--absolute-value', '-a'], {'action': <function BooleanOptionalActionWitoutImplicitDefault at 0xXXXXXXXXX>, 'default': False, 'help': 'If True, the result will be made positive', 'required': False})
 usage: 5_logging.py math [-h] [--round-to-int | --no-round-to-int | -r]
                          [--absolute-value | --no-absolute-value | -a]
                          {add,mul,sub,truediv} numbers [numbers ...]
 5_logging.py math: error: the following arguments are required: numbers
 
 """
+
 import argparse
 import clargs
 import operator as mod_operator
 import logging
 import typing as t
```

### Comparing `clargs-0.7.0/examples/6_validation.py` & `clargs-0.9.0a0.dev1/examples/6_validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 The given even number is: 2
 
 >>> python examples/6_validation.py -2 (returncode: 0)
 The given even number is: -2
 
 >>> python examples/6_validation.py 1 (returncode: 2)
 usage: 6_validation.py [-h] number
-6_validation.py: error: argument number: invalid validate value: '1'
+6_validation.py: error: argument number: invalid int-validation value: '1'
 
 """
+
 import clargs
 import typing as t
 
 
 def print_even_number(
     number: t.Annotated[
         int,
         clargs.extra_info(
             validate=lambda n: n % 2 == 0,
         ),
-    ]
+    ],
 ):
     """
     Prints a number
 
     @param number: An even number
     """
     print(f"The given even number is: {number}")
```

### Comparing `clargs-0.7.0/src/clargs/__init__.py` & `clargs-0.9.0a0.dev1/src/clargs/__init__.py`

 * *Files identical despite different names*

### Comparing `clargs-0.7.0/src/clargs/aap_from_data.py` & `clargs-0.9.0a0.dev1/src/clargs/aap_from_data.py`

 * *Files identical despite different names*

### Comparing `clargs-0.7.0/src/clargs/clargs.py` & `clargs-0.9.0a0.dev1/src/clargs/clargs.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,25 +56,29 @@
         assert not (self.short_flag_prefix is None and self.generate_short_flags), (
             "If generate_short_flags is True, short_flag_prefix " "cannot be None"
         )
 
 
 @dataclasses.dataclass(frozen=True, kw_only=True)
 class AddArgumentParameters(t.Generic[T]):
-    action: t.Literal[
-        "store",
-        "store_const",
-        "store_true",
-        "store_false",
-        "append",
-        "append_const",
-        "count",
-        "help",
-        "version",
-    ] | t.Callable | NOT_SET_TYPE = NOT_SET
+    action: (
+        t.Literal[
+            "store",
+            "store_const",
+            "store_true",
+            "store_false",
+            "append",
+            "append_const",
+            "count",
+            "help",
+            "version",
+        ]
+        | t.Callable
+        | NOT_SET_TYPE
+    ) = NOT_SET
     choices: t.Container[str] | NOT_SET_TYPE = NOT_SET
     const: T | NOT_SET_TYPE = NOT_SET
     default: T | NOT_SET_TYPE = NOT_SET
     dest: str | NOT_SET_TYPE = NOT_SET
     help: str | NOT_SET_TYPE = NOT_SET
     metavar: str | NOT_SET_TYPE = NOT_SET
     nargs: int | t.Literal["?", "*", "+"] | NOT_SET_TYPE = NOT_SET
```

### Comparing `clargs-0.7.0/src/clargs/docsparser.py` & `clargs-0.9.0a0.dev1/src/clargs/docsparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import re
 import textwrap
-import inspect
 import dataclasses
 import typing as t
 
 """
 Parses function documentation to get to the parameters.
 
 It supports the following formats:
```

### Comparing `clargs-0.7.0/src/clargs/helper_types.py` & `clargs-0.9.0a0.dev1/src/clargs/helper_types.py`

 * *Files identical despite different names*

### Comparing `clargs-0.7.0/test/test_docsparser.py` & `clargs-0.9.0a0.dev1/tests/test_docsparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import textwrap
-from test_simple import Base
+from .test_simple import Base
 from clargs.docsparser import get_parameter_info_from_docstring, Param
 
 
 class DocParserBase(Base):
     def assertParse(self, docstring, result):
         paraminfo = get_parameter_info_from_docstring(docstring)
         print(docstring)
```

### Comparing `clargs-0.7.0/test/test_simple.py` & `clargs-0.9.0a0.dev1/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `clargs-0.7.0/test/test_validation.py` & `clargs-0.9.0a0.dev1/tests/test_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import clargs
 import typing as t
-from test_simple import Base
+from .test_simple import Base
 
 
 class TestValidationCases(Base):
     def test_validation(self):
         LessThanTenInt = t.Annotated[int, clargs.extra_info(validate=lambda n: n < 10)]
 
         def function(*, less_than_ten: LessThanTenInt):
```

