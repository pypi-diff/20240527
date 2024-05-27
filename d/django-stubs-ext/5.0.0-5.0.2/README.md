# Comparing `tmp/django_stubs_ext-5.0.0.tar.gz` & `tmp/django_stubs_ext-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_stubs_ext-5.0.0.tar", last modified: Tue Apr 30 10:02:55 2024, max compression
+gzip compressed data, was "django_stubs_ext-5.0.2.tar", last modified: Mon May 27 12:17:31 2024, max compression
```

## Comparing `django_stubs_ext-5.0.0.tar` & `django_stubs_ext-5.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:02:55.564887 django_stubs_ext-5.0.0/
--rw-r--r--   0 marti     (1000) marti     (1000)     1075 2023-10-18 16:47:22.000000 django_stubs_ext-5.0.0/LICENSE.md
--rw-r--r--   0 marti     (1000) marti     (1000)     3578 2024-04-30 10:02:55.564887 django_stubs_ext-5.0.0/PKG-INFO
--rw-r--r--   0 marti     (1000) marti     (1000)     2496 2023-10-18 16:47:22.000000 django_stubs_ext-5.0.0/README.md
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:02:55.564887 django_stubs_ext-5.0.0/django_stubs_ext/
--rw-r--r--   0 marti     (1000) marti     (1000)      535 2023-10-18 16:47:22.000000 django_stubs_ext-5.0.0/django_stubs_ext/__init__.py
--rw-r--r--   0 marti     (1000) marti     (1000)      620 2023-10-18 16:47:22.000000 django_stubs_ext-5.0.0/django_stubs_ext/aliases.py
--rw-r--r--   0 marti     (1000) marti     (1000)      693 2023-10-18 16:47:22.000000 django_stubs_ext-5.0.0/django_stubs_ext/annotations.py
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:02:55.564887 django_stubs_ext-5.0.0/django_stubs_ext/db/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-10-18 16:47:22.000000 django_stubs_ext-5.0.0/django_stubs_ext/db/__init__.py
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:02:55.564887 django_stubs_ext-5.0.0/django_stubs_ext/db/models/
--rw-r--r--   0 marti     (1000) marti     (1000)     1911 2023-12-05 19:01:16.000000 django_stubs_ext-5.0.0/django_stubs_ext/db/models/__init__.py
--rw-r--r--   0 marti     (1000) marti     (1000)      814 2024-04-30 10:01:49.000000 django_stubs_ext-5.0.0/django_stubs_ext/db/models/manager.py
--rw-r--r--   0 marti     (1000) marti     (1000)      930 2024-04-30 10:01:49.000000 django_stubs_ext-5.0.0/django_stubs_ext/db/router.py
--rw-r--r--   0 marti     (1000) marti     (1000)     3902 2024-04-30 10:01:49.000000 django_stubs_ext-5.0.0/django_stubs_ext/patch.py
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-10-18 16:47:22.000000 django_stubs_ext-5.0.0/django_stubs_ext/py.typed
--rw-r--r--   0 marti     (1000) marti     (1000)      220 2024-04-30 10:01:49.000000 django_stubs_ext-5.0.0/django_stubs_ext/types.py
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:02:55.564887 django_stubs_ext-5.0.0/django_stubs_ext.egg-info/
--rw-r--r--   0 marti     (1000) marti     (1000)     3578 2024-04-30 10:02:55.000000 django_stubs_ext-5.0.0/django_stubs_ext.egg-info/PKG-INFO
--rw-r--r--   0 marti     (1000) marti     (1000)      585 2024-04-30 10:02:55.000000 django_stubs_ext-5.0.0/django_stubs_ext.egg-info/SOURCES.txt
--rw-r--r--   0 marti     (1000) marti     (1000)        1 2024-04-30 10:02:55.000000 django_stubs_ext-5.0.0/django_stubs_ext.egg-info/dependency_links.txt
--rw-r--r--   0 marti     (1000) marti     (1000)       25 2024-04-30 10:02:55.000000 django_stubs_ext-5.0.0/django_stubs_ext.egg-info/requires.txt
--rw-r--r--   0 marti     (1000) marti     (1000)       17 2024-04-30 10:02:55.000000 django_stubs_ext-5.0.0/django_stubs_ext.egg-info/top_level.txt
--rw-r--r--   0 marti     (1000) marti     (1000)       38 2024-04-30 10:02:55.564887 django_stubs_ext-5.0.0/setup.cfg
--rwxr-xr-x   0 marti     (1000) marti     (1000)     1736 2024-04-30 10:01:49.000000 django_stubs_ext-5.0.0/setup.py
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:02:55.564887 django_stubs_ext-5.0.0/tests/
--rw-r--r--   0 marti     (1000) marti     (1000)      169 2023-10-18 16:47:22.000000 django_stubs_ext-5.0.0/tests/test_aliases.py
--rw-r--r--   0 marti     (1000) marti     (1000)     3928 2024-04-30 10:01:49.000000 django_stubs_ext-5.0.0/tests/test_monkeypatching.py
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-05-27 12:17:31.964842 django_stubs_ext-5.0.2/
+-rw-r--r--   0 marti     (1000) marti     (1000)     1075 2023-10-18 16:47:22.000000 django_stubs_ext-5.0.2/LICENSE.md
+-rw-r--r--   0 marti     (1000) marti     (1000)     3539 2024-05-27 12:17:31.964842 django_stubs_ext-5.0.2/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti     (1000)     2496 2023-10-18 16:47:22.000000 django_stubs_ext-5.0.2/README.md
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-05-27 12:17:31.961509 django_stubs_ext-5.0.2/django_stubs_ext/
+-rw-r--r--   0 marti     (1000) marti     (1000)      535 2023-10-18 16:47:22.000000 django_stubs_ext-5.0.2/django_stubs_ext/__init__.py
+-rw-r--r--   0 marti     (1000) marti     (1000)      727 2024-05-27 12:17:03.000000 django_stubs_ext-5.0.2/django_stubs_ext/aliases.py
+-rw-r--r--   0 marti     (1000) marti     (1000)      693 2023-10-18 16:47:22.000000 django_stubs_ext-5.0.2/django_stubs_ext/annotations.py
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-05-27 12:17:31.964842 django_stubs_ext-5.0.2/django_stubs_ext/db/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-10-18 16:47:22.000000 django_stubs_ext-5.0.2/django_stubs_ext/db/__init__.py
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-05-27 12:17:31.964842 django_stubs_ext-5.0.2/django_stubs_ext/db/models/
+-rw-r--r--   0 marti     (1000) marti     (1000)     1911 2023-12-05 19:01:16.000000 django_stubs_ext-5.0.2/django_stubs_ext/db/models/__init__.py
+-rw-r--r--   0 marti     (1000) marti     (1000)      814 2024-04-30 10:01:49.000000 django_stubs_ext-5.0.2/django_stubs_ext/db/models/manager.py
+-rw-r--r--   0 marti     (1000) marti     (1000)      930 2024-04-30 10:01:49.000000 django_stubs_ext-5.0.2/django_stubs_ext/db/router.py
+-rw-r--r--   0 marti     (1000) marti     (1000)     3902 2024-04-30 10:01:49.000000 django_stubs_ext-5.0.2/django_stubs_ext/patch.py
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-10-18 16:47:22.000000 django_stubs_ext-5.0.2/django_stubs_ext/py.typed
+-rw-r--r--   0 marti     (1000) marti     (1000)      220 2024-04-30 10:01:49.000000 django_stubs_ext-5.0.2/django_stubs_ext/types.py
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-05-27 12:17:31.964842 django_stubs_ext-5.0.2/django_stubs_ext.egg-info/
+-rw-r--r--   0 marti     (1000) marti     (1000)     3539 2024-05-27 12:17:31.000000 django_stubs_ext-5.0.2/django_stubs_ext.egg-info/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti     (1000)      585 2024-05-27 12:17:31.000000 django_stubs_ext-5.0.2/django_stubs_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 marti     (1000) marti     (1000)        1 2024-05-27 12:17:31.000000 django_stubs_ext-5.0.2/django_stubs_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 marti     (1000) marti     (1000)       25 2024-05-27 12:17:31.000000 django_stubs_ext-5.0.2/django_stubs_ext.egg-info/requires.txt
+-rw-r--r--   0 marti     (1000) marti     (1000)       17 2024-05-27 12:17:31.000000 django_stubs_ext-5.0.2/django_stubs_ext.egg-info/top_level.txt
+-rw-r--r--   0 marti     (1000) marti     (1000)       38 2024-05-27 12:17:31.964842 django_stubs_ext-5.0.2/setup.cfg
+-rwxr-xr-x   0 marti     (1000) marti     (1000)     1698 2024-05-27 12:17:03.000000 django_stubs_ext-5.0.2/setup.py
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-05-27 12:17:31.964842 django_stubs_ext-5.0.2/tests/
+-rw-r--r--   0 marti     (1000) marti     (1000)      169 2023-10-18 16:47:22.000000 django_stubs_ext-5.0.2/tests/test_aliases.py
+-rw-r--r--   0 marti     (1000) marti     (1000)     3928 2024-04-30 10:01:49.000000 django_stubs_ext-5.0.2/tests/test_monkeypatching.py
```

### Comparing `django_stubs_ext-5.0.0/LICENSE.md` & `django_stubs_ext-5.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_stubs_ext-5.0.0/PKG-INFO` & `django_stubs_ext-5.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-stubs-ext
-Version: 5.0.0
+Version: 5.0.2
 Summary: Monkey-patching and extensions for django-stubs
 Home-page: https://github.com/typeddjango/django-stubs
 Author: Simula Proxy
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
 Project-URL: Funding, https://github.com/sponsors/typeddjango
@@ -14,15 +14,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: django
 Requires-Dist: typing-extensions
```

### Comparing `django_stubs_ext-5.0.0/README.md` & `django_stubs_ext-5.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django_stubs_ext-5.0.0/django_stubs_ext/__init__.py` & `django_stubs_ext-5.0.2/django_stubs_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `django_stubs_ext-5.0.0/django_stubs_ext/annotations.py` & `django_stubs_ext-5.0.2/django_stubs_ext/annotations.py`

 * *Files identical despite different names*

### Comparing `django_stubs_ext-5.0.0/django_stubs_ext/db/models/__init__.py` & `django_stubs_ext-5.0.2/django_stubs_ext/db/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django_stubs_ext-5.0.0/django_stubs_ext/db/models/manager.py` & `django_stubs_ext-5.0.2/django_stubs_ext/db/models/manager.py`

 * *Files identical despite different names*

### Comparing `django_stubs_ext-5.0.0/django_stubs_ext/db/router.py` & `django_stubs_ext-5.0.2/django_stubs_ext/db/router.py`

 * *Files identical despite different names*

### Comparing `django_stubs_ext-5.0.0/django_stubs_ext/patch.py` & `django_stubs_ext-5.0.2/django_stubs_ext/patch.py`

 * *Files identical despite different names*

### Comparing `django_stubs_ext-5.0.0/django_stubs_ext.egg-info/PKG-INFO` & `django_stubs_ext-5.0.2/django_stubs_ext.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-stubs-ext
-Version: 5.0.0
+Version: 5.0.2
 Summary: Monkey-patching and extensions for django-stubs
 Home-page: https://github.com/typeddjango/django-stubs
 Author: Simula Proxy
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
 Project-URL: Funding, https://github.com/sponsors/typeddjango
@@ -14,15 +14,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: django
 Requires-Dist: typing-extensions
```

### Comparing `django_stubs_ext-5.0.0/django_stubs_ext.egg-info/SOURCES.txt` & `django_stubs_ext-5.0.2/django_stubs_ext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_stubs_ext-5.0.0/setup.py` & `django_stubs_ext-5.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "typing-extensions",
 ]
 
 # NB! For clarity, keep version major.minor.patch in sync with django-stubs.
 # It's fine to skip django-stubs-ext releases, but when doing a release, update this to newest django-stubs version.
 setup(
     name="django-stubs-ext",
-    version="5.0.0",
+    version="5.0.2",
     description="Monkey-patching and extensions for django-stubs",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",
     license_files=["LICENSE.md"],
     url="https://github.com/typeddjango/django-stubs",
     author="Simula Proxy",
@@ -34,15 +34,14 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Typing :: Typed",
         "Framework :: Django",
-        "Framework :: Django :: 4.1",
         "Framework :: Django :: 4.2",
         "Framework :: Django :: 5.0",
     ],
     project_urls={
         "Funding": "https://github.com/sponsors/typeddjango",
         "Release notes": "https://github.com/typeddjango/django-stubs/releases",
     },
```

### Comparing `django_stubs_ext-5.0.0/tests/test_monkeypatching.py` & `django_stubs_ext-5.0.2/tests/test_monkeypatching.py`

 * *Files identical despite different names*

