# Comparing `tmp/link_mongodb-1.0.0.tar.gz` & `tmp/link_mongodb-2.0.0.tar.gz`

## Comparing `link_mongodb-1.0.0.tar` & `link_mongodb-2.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 link_mongodb-1.0.0/mkdocs.yml
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 link_mongodb-1.0.0/src/link_mongodb/__init__.py
--rw-r--r--   0        0        0    17807 2020-02-02 00:00:00.000000 link_mongodb-1.0.0/src/link_mongodb/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 link_mongodb-1.0.0/src/link_mongodb/py.typed
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 link_mongodb-1.0.0/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 link_mongodb-1.0.0/LICENSE
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 link_mongodb-1.0.0/README.md
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 link_mongodb-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 link_mongodb-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 link_mongodb-2.0.0/mkdocs.yml
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 link_mongodb-2.0.0/src/link_mongodb/__init__.py
+-rw-r--r--   0        0        0     9579 2020-02-02 00:00:00.000000 link_mongodb-2.0.0/src/link_mongodb/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 link_mongodb-2.0.0/src/link_mongodb/py.typed
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 link_mongodb-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 link_mongodb-2.0.0/LICENSE
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 link_mongodb-2.0.0/README.md
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 link_mongodb-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6276 2020-02-02 00:00:00.000000 link_mongodb-2.0.0/PKG-INFO
```

### Comparing `link_mongodb-1.0.0/mkdocs.yml` & `link_mongodb-2.0.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `link_mongodb-1.0.0/.gitignore` & `link_mongodb-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `link_mongodb-1.0.0/LICENSE` & `link_mongodb-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `link_mongodb-1.0.0/README.md` & `link_mongodb-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `link_mongodb-1.0.0/pyproject.toml` & `link_mongodb-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "pymongo == 4.5.0",
+  "motor == 3.4.0",
 ]
 description = "link mongo database"
 dynamic = ["version"]
 keywords = []
 license = "MIT"
 name = "link_mongodb"
 readme = "README.md"
```

### Comparing `link_mongodb-1.0.0/PKG-INFO` & `link_mongodb-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: link_mongodb
-Version: 1.0.0
+Version: 2.0.0
 Summary: link mongo database
 Project-URL: Documentation, https://asmitul.github.io/link-mongodb
 Project-URL: Issues, https://github.com/asmitul/link-mongodb/issues
 Project-URL: Source, https://github.com/asmitul/link-mongodb
 Author: asmitul
 License-Expression: MIT
 License-File: LICENSE
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: <3.12,>=3.8
-Requires-Dist: pymongo==4.5.0
+Requires-Dist: motor==3.4.0
 Provides-Extra: docs
 Requires-Dist: mkdocs-git-revision-date-localized-plugin~=1.1.0; extra == 'docs'
 Requires-Dist: mkdocs-material~=8.5.4; extra == 'docs'
 Requires-Dist: mkdocstrings[python]~=0.19.0; extra == 'docs'
 Requires-Dist: mkdocs~=1.4.0; extra == 'docs'
 Provides-Extra: quality
 Requires-Dist: black~=22.10.0; extra == 'quality'
```

