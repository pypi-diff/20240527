# Comparing `tmp/artsem-0.0.42.tar.gz` & `tmp/artsem-0.0.43.tar.gz`

## Comparing `artsem-0.0.42.tar` & `artsem-0.0.43.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 artsem-0.0.42/__about__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 artsem-0.0.42/__init__.py
--rw-r--r--   0        0        0     6986 2020-02-02 00:00:00.000000 artsem-0.0.42/artsem.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 artsem-0.0.42/exitcodes.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 artsem-0.0.42/persistence.py
--rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 artsem-0.0.42/probes.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 artsem-0.0.42/modules/elf_tests.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 artsem-0.0.42/modules/probeDummy/.conf
--rwxr-xr-x   0        0        0      283 2020-02-02 00:00:00.000000 artsem-0.0.42/modules/probeDummy/main.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 artsem-0.0.42/modules/probeDummy2/.conf
--rwxr-xr-x   0        0        0      283 2020-02-02 00:00:00.000000 artsem-0.0.42/modules/probeDummy2/main.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 artsem-0.0.42/modules/probeDummy3/.conf
--rwxr-xr-x   0        0        0      283 2020-02-02 00:00:00.000000 artsem-0.0.42/modules/probeDummy3/main.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 artsem-0.0.42/templates/detailed.md
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 artsem-0.0.42/templates/probe.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 artsem-0.0.42/templates/simple.md
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 artsem-0.0.42/tests/__init__.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 artsem-0.0.42/tests/test.py
--rw-r--r--   0        0        0    16200 2020-02-02 00:00:00.000000 artsem-0.0.42/tests/samples/a.out
--rw-r--r--   0        0        0    16200 2020-02-02 00:00:00.000000 artsem-0.0.42/tests/samples/b.out
--rw-r--r--   0        0        0    23038 2020-02-02 00:00:00.000000 artsem-0.0.42/tests/samples/cat.c
--rw-r--r--   0        0        0   167841 2020-02-02 00:00:00.000000 artsem-0.0.42/tests/samples/ls.c
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 artsem-0.0.42/tests/samples/ls.h
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 artsem-0.0.42/tests/samples/test.c
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 artsem-0.0.42/tests/samples/test.txt
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 artsem-0.0.42/util/mitreConnector.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 artsem-0.0.42/.gitignore
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 artsem-0.0.42/pyproject.toml
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 artsem-0.0.42/../README.md
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 artsem-0.0.42/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 artsem-0.0.43/__about__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 artsem-0.0.43/__init__.py
+-rw-r--r--   0        0        0     6986 2020-02-02 00:00:00.000000 artsem-0.0.43/artsem.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 artsem-0.0.43/exitcodes.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 artsem-0.0.43/persistence.py
+-rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 artsem-0.0.43/probes.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 artsem-0.0.43/modules/elf_tests.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 artsem-0.0.43/modules/probeDummy/.conf
+-rwxr-xr-x   0        0        0      283 2020-02-02 00:00:00.000000 artsem-0.0.43/modules/probeDummy/main.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 artsem-0.0.43/modules/probeDummy2/.conf
+-rwxr-xr-x   0        0        0      283 2020-02-02 00:00:00.000000 artsem-0.0.43/modules/probeDummy2/main.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 artsem-0.0.43/modules/probeDummy3/.conf
+-rwxr-xr-x   0        0        0      283 2020-02-02 00:00:00.000000 artsem-0.0.43/modules/probeDummy3/main.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 artsem-0.0.43/templates/detailed.md
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 artsem-0.0.43/templates/probe.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 artsem-0.0.43/templates/simple.md
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 artsem-0.0.43/tests/__init__.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 artsem-0.0.43/tests/test.py
+-rw-r--r--   0        0        0    16200 2020-02-02 00:00:00.000000 artsem-0.0.43/tests/samples/a.out
+-rw-r--r--   0        0        0    16200 2020-02-02 00:00:00.000000 artsem-0.0.43/tests/samples/b.out
+-rw-r--r--   0        0        0    23038 2020-02-02 00:00:00.000000 artsem-0.0.43/tests/samples/cat.c
+-rw-r--r--   0        0        0   167841 2020-02-02 00:00:00.000000 artsem-0.0.43/tests/samples/ls.c
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 artsem-0.0.43/tests/samples/ls.h
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 artsem-0.0.43/tests/samples/test.c
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 artsem-0.0.43/tests/samples/test.txt
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 artsem-0.0.43/util/mitreConnector.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 artsem-0.0.43/.gitignore
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 artsem-0.0.43/pyproject.toml
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 artsem-0.0.43/../README.md
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 artsem-0.0.43/PKG-INFO
```

### Comparing `artsem-0.0.42/artsem.py` & `artsem-0.0.43/artsem.py`

 * *Files identical despite different names*

### Comparing `artsem-0.0.42/exitcodes.py` & `artsem-0.0.43/exitcodes.py`

 * *Files identical despite different names*

### Comparing `artsem-0.0.42/persistence.py` & `artsem-0.0.43/persistence.py`

 * *Files identical despite different names*

### Comparing `artsem-0.0.42/probes.py` & `artsem-0.0.43/probes.py`

 * *Files identical despite different names*

### Comparing `artsem-0.0.42/modules/elf_tests.py` & `artsem-0.0.43/modules/elf_tests.py`

 * *Files identical despite different names*

### Comparing `artsem-0.0.42/tests/test.py` & `artsem-0.0.43/tests/test.py`

 * *Files identical despite different names*

### Comparing `artsem-0.0.42/tests/samples/a.out` & `artsem-0.0.43/tests/samples/a.out`

 * *Files identical despite different names*

### Comparing `artsem-0.0.42/tests/samples/b.out` & `artsem-0.0.43/tests/samples/b.out`

 * *Files identical despite different names*

### Comparing `artsem-0.0.42/tests/samples/cat.c` & `artsem-0.0.43/tests/samples/cat.c`

 * *Files identical despite different names*

### Comparing `artsem-0.0.42/tests/samples/ls.c` & `artsem-0.0.43/tests/samples/ls.c`

 * *Files identical despite different names*

### Comparing `artsem-0.0.42/util/mitreConnector.py` & `artsem-0.0.43/util/mitreConnector.py`

 * *Files identical despite different names*

### Comparing `artsem-0.0.42/pyproject.toml` & `artsem-0.0.43/pyproject.toml`

 * *Files identical despite different names*

### Comparing `artsem-0.0.42/../README.md` & `artsem-0.0.43/../README.md`

 * *Files identical despite different names*

### Comparing `artsem-0.0.42/PKG-INFO` & `artsem-0.0.43/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: artsem
-Version: 0.0.42
+Version: 0.0.43
 Project-URL: Documentation, https://github.com/unknown/artsem#readme
 Project-URL: Issues, https://github.com/unknown/artsem/issues
 Project-URL: Source, https://github.com/unknown/artsem
 Author-email: uRHL <100383351@alumnos.uc3m.es>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

