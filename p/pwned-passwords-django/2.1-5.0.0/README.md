# Comparing `tmp/pwned-passwords-django-2.1.tar.gz` & `tmp/pwned_passwords_django-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwned-passwords-django-2.1.tar", last modified: Tue Feb 27 07:47:32 2024, max compression
+gzip compressed data, was "pwned_passwords_django-5.0.0.tar", last modified: Mon May 27 07:13:13 2024, max compression
```

## Comparing `pwned-passwords-django-2.1.tar` & `pwned_passwords_django-5.0.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 james      (503) staff       (20)        0 2024-02-27 07:47:32.441645 pwned-passwords-django-2.1/
--rw-r--r--   0 james      (503) staff       (20)      299 2023-01-09 05:47:40.000000 pwned-passwords-django-2.1/.editorconfig
--rw-r--r--   0 james      (503) staff       (20)      107 2022-12-28 21:58:57.000000 pwned-passwords-django-2.1/.flake8
--rw-r--r--   0 james      (503) staff       (20)     1307 2024-02-26 06:00:59.000000 pwned-passwords-django-2.1/.pre-commit-config.yaml
--rw-r--r--   0 james      (503) staff       (20)      295 2023-01-09 06:02:40.000000 pwned-passwords-django-2.1/.readthedocs.yaml
--rw-r--r--   0 james      (503) staff       (20)     1530 2024-02-23 06:59:25.000000 pwned-passwords-django-2.1/LICENSE
--rw-r--r--   0 james      (503) staff       (20)      293 2023-06-09 05:52:25.000000 pwned-passwords-django-2.1/MANIFEST.in
--rw-r--r--   0 james      (503) staff       (20)     4179 2024-02-27 07:47:32.441457 pwned-passwords-django-2.1/PKG-INFO
--rw-r--r--   0 james      (503) staff       (20)     2370 2024-02-27 07:32:39.000000 pwned-passwords-django-2.1/README.rst
-drwxr-xr-x   0 james      (503) staff       (20)        0 2024-02-27 07:47:32.438480 pwned-passwords-django-2.1/docs/
--rw-r--r--   0 james      (503) staff       (20)      620 2023-02-14 08:30:32.000000 pwned-passwords-django-2.1/docs/Makefile
--rw-r--r--   0 james      (503) staff       (20)     2337 2024-02-27 06:50:09.000000 pwned-passwords-django-2.1/docs/api.rst
--rw-r--r--   0 james      (503) staff       (20)    12654 2024-02-27 07:38:00.000000 pwned-passwords-django-2.1/docs/changelog.rst
--rw-r--r--   0 james      (503) staff       (20)     1796 2024-02-24 08:12:21.000000 pwned-passwords-django-2.1/docs/conf.py
--rw-r--r--   0 james      (503) staff       (20)      109 2023-01-20 05:49:41.000000 pwned-passwords-django-2.1/docs/docs_settings.py
--rw-r--r--   0 james      (503) staff       (20)     5732 2024-02-27 06:51:04.000000 pwned-passwords-django-2.1/docs/exceptions.rst
--rw-r--r--   0 james      (503) staff       (20)     6633 2024-02-27 06:48:17.000000 pwned-passwords-django-2.1/docs/faq.rst
--rw-r--r--   0 james      (503) staff       (20)     2343 2024-02-27 07:32:48.000000 pwned-passwords-django-2.1/docs/index.rst
--rw-r--r--   0 james      (503) staff       (20)     2327 2024-02-27 07:30:27.000000 pwned-passwords-django-2.1/docs/install.rst
--rw-r--r--   0 james      (503) staff       (20)      826 2018-03-06 07:00:02.000000 pwned-passwords-django-2.1/docs/make.bat
--rw-r--r--   0 james      (503) staff       (20)      504 2024-02-27 06:51:48.000000 pwned-passwords-django-2.1/docs/middleware.rst
--rw-r--r--   0 james      (503) staff       (20)     2435 2024-02-27 06:52:03.000000 pwned-passwords-django-2.1/docs/settings.rst
--rw-r--r--   0 james      (503) staff       (20)      235 2023-01-09 05:54:25.000000 pwned-passwords-django-2.1/docs/spelling_wordlist.txt
--rw-r--r--   0 james      (503) staff       (20)     4909 2024-02-27 06:52:29.000000 pwned-passwords-django-2.1/docs/validator.rst
--rw-r--r--   0 james      (503) staff       (20)    11173 2024-02-26 06:11:39.000000 pwned-passwords-django-2.1/noxfile.py
--rw-r--r--   0 james      (503) staff       (20)     1948 2024-02-27 07:42:37.000000 pwned-passwords-django-2.1/pyproject.toml
--rw-r--r--   0 james      (503) staff       (20)      374 2024-02-27 07:39:56.000000 pwned-passwords-django-2.1/runtests.py
--rw-r--r--   0 james      (503) staff       (20)       38 2024-02-27 07:47:32.441685 pwned-passwords-django-2.1/setup.cfg
-drwxr-xr-x   0 james      (503) staff       (20)        0 2024-02-27 07:47:32.435442 pwned-passwords-django-2.1/src/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2024-02-27 07:47:32.439110 pwned-passwords-django-2.1/src/pwned_passwords_django/
--rw-r--r--   0 james      (503) staff       (20)      122 2024-02-27 07:40:52.000000 pwned-passwords-django-2.1/src/pwned_passwords_django/__init__.py
--rw-r--r--   0 james      (503) staff       (20)    11560 2024-02-26 05:27:25.000000 pwned-passwords-django-2.1/src/pwned_passwords_django/api.py
--rw-r--r--   0 james      (503) staff       (20)      716 2024-02-23 06:56:55.000000 pwned-passwords-django-2.1/src/pwned_passwords_django/exceptions.py
--rw-r--r--   0 james      (503) staff       (20)     8812 2024-02-27 06:54:28.000000 pwned-passwords-django-2.1/src/pwned_passwords_django/middleware.py
--rw-r--r--   0 james      (503) staff       (20)     4922 2024-02-23 06:57:06.000000 pwned-passwords-django-2.1/src/pwned_passwords_django/validators.py
-drwxr-xr-x   0 james      (503) staff       (20)        0 2024-02-27 07:47:32.440891 pwned-passwords-django-2.1/src/pwned_passwords_django.egg-info/
--rw-r--r--   0 james      (503) staff       (20)     4179 2024-02-27 07:47:32.000000 pwned-passwords-django-2.1/src/pwned_passwords_django.egg-info/PKG-INFO
--rw-r--r--   0 james      (503) staff       (20)      953 2024-02-27 07:47:32.000000 pwned-passwords-django-2.1/src/pwned_passwords_django.egg-info/SOURCES.txt
--rw-r--r--   0 james      (503) staff       (20)        1 2024-02-27 07:47:32.000000 pwned-passwords-django-2.1/src/pwned_passwords_django.egg-info/dependency_links.txt
--rw-r--r--   0 james      (503) staff       (20)      219 2024-02-27 07:47:32.000000 pwned-passwords-django-2.1/src/pwned_passwords_django.egg-info/requires.txt
--rw-r--r--   0 james      (503) staff       (20)       23 2024-02-27 07:47:32.000000 pwned-passwords-django-2.1/src/pwned_passwords_django.egg-info/top_level.txt
-drwxr-xr-x   0 james      (503) staff       (20)        0 2024-02-27 07:47:32.440675 pwned-passwords-django-2.1/tests/
--rw-r--r--   0 james      (503) staff       (20)        0 2018-05-25 00:24:50.000000 pwned-passwords-django-2.1/tests/__init__.py
--rw-r--r--   0 james      (503) staff       (20)     6701 2024-02-24 01:50:20.000000 pwned-passwords-django-2.1/tests/base.py
--rw-r--r--   0 james      (503) staff       (20)      764 2024-02-23 06:55:59.000000 pwned-passwords-django-2.1/tests/settings.py
--rw-r--r--   0 james      (503) staff       (20)    13630 2024-02-25 02:26:59.000000 pwned-passwords-django-2.1/tests/test_api.py
--rw-r--r--   0 james      (503) staff       (20)     9793 2024-02-23 06:56:13.000000 pwned-passwords-django-2.1/tests/test_middleware.py
--rw-r--r--   0 james      (503) staff       (20)     6517 2024-02-23 08:00:05.000000 pwned-passwords-django-2.1/tests/test_validators.py
--rw-r--r--   0 james      (503) staff       (20)     2356 2024-02-23 06:56:31.000000 pwned-passwords-django-2.1/tests/urls.py
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 07:13:13.522167 pwned_passwords_django-5.0.0/
+-rw-r--r--   0 james      (503) staff       (20)      299 2023-01-09 05:47:40.000000 pwned_passwords_django-5.0.0/.editorconfig
+-rw-r--r--   0 james      (503) staff       (20)      107 2022-12-28 21:58:57.000000 pwned_passwords_django-5.0.0/.flake8
+-rw-r--r--   0 james      (503) staff       (20)     1307 2024-05-27 01:50:45.000000 pwned_passwords_django-5.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 james      (503) staff       (20)      295 2023-01-09 06:02:40.000000 pwned_passwords_django-5.0.0/.readthedocs.yaml
+-rw-r--r--   0 james      (503) staff       (20)     1530 2024-02-23 06:59:25.000000 pwned_passwords_django-5.0.0/LICENSE
+-rw-r--r--   0 james      (503) staff       (20)      293 2023-06-09 05:52:25.000000 pwned_passwords_django-5.0.0/MANIFEST.in
+-rw-r--r--   0 james      (503) staff       (20)     4126 2024-05-27 07:13:13.521999 pwned_passwords_django-5.0.0/PKG-INFO
+-rw-r--r--   0 james      (503) staff       (20)     2370 2024-02-27 07:32:39.000000 pwned_passwords_django-5.0.0/README.rst
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 07:13:13.519355 pwned_passwords_django-5.0.0/docs/
+-rw-r--r--   0 james      (503) staff       (20)      620 2023-02-14 08:30:32.000000 pwned_passwords_django-5.0.0/docs/Makefile
+-rw-r--r--   0 james      (503) staff       (20)     2327 2024-05-27 07:02:11.000000 pwned_passwords_django-5.0.0/docs/api.rst
+-rw-r--r--   0 james      (503) staff       (20)    15145 2024-05-27 07:04:28.000000 pwned_passwords_django-5.0.0/docs/changelog.rst
+-rw-r--r--   0 james      (503) staff       (20)     1796 2024-02-28 06:54:06.000000 pwned_passwords_django-5.0.0/docs/conf.py
+-rw-r--r--   0 james      (503) staff       (20)      109 2023-01-20 05:49:41.000000 pwned_passwords_django-5.0.0/docs/docs_settings.py
+-rw-r--r--   0 james      (503) staff       (20)     5732 2024-02-27 06:51:04.000000 pwned_passwords_django-5.0.0/docs/exceptions.rst
+-rw-r--r--   0 james      (503) staff       (20)     6629 2024-05-27 07:03:40.000000 pwned_passwords_django-5.0.0/docs/faq.rst
+-rw-r--r--   0 james      (503) staff       (20)     2502 2024-05-27 06:50:20.000000 pwned_passwords_django-5.0.0/docs/index.rst
+-rw-r--r--   0 james      (503) staff       (20)     2321 2024-05-27 01:47:50.000000 pwned_passwords_django-5.0.0/docs/install.rst
+-rw-r--r--   0 james      (503) staff       (20)      826 2018-03-06 07:00:02.000000 pwned_passwords_django-5.0.0/docs/make.bat
+-rw-r--r--   0 james      (503) staff       (20)      528 2024-05-27 07:01:57.000000 pwned_passwords_django-5.0.0/docs/middleware.rst
+-rw-r--r--   0 james      (503) staff       (20)     2435 2024-02-27 06:52:03.000000 pwned_passwords_django-5.0.0/docs/settings.rst
+-rw-r--r--   0 james      (503) staff       (20)      252 2024-05-27 02:29:28.000000 pwned_passwords_django-5.0.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 james      (503) staff       (20)     2592 2024-05-27 07:01:12.000000 pwned_passwords_django-5.0.0/docs/usage.rst
+-rw-r--r--   0 james      (503) staff       (20)     4897 2024-05-27 07:01:47.000000 pwned_passwords_django-5.0.0/docs/validator.rst
+-rw-r--r--   0 james      (503) staff       (20)    11106 2024-05-27 02:30:05.000000 pwned_passwords_django-5.0.0/noxfile.py
+-rw-r--r--   0 james      (503) staff       (20)     1900 2024-05-27 01:47:22.000000 pwned_passwords_django-5.0.0/pyproject.toml
+-rw-r--r--   0 james      (503) staff       (20)      374 2024-02-27 07:39:56.000000 pwned_passwords_django-5.0.0/runtests.py
+-rw-r--r--   0 james      (503) staff       (20)       38 2024-05-27 07:13:13.522210 pwned_passwords_django-5.0.0/setup.cfg
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 07:13:13.516338 pwned_passwords_django-5.0.0/src/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 07:13:13.519939 pwned_passwords_django-5.0.0/src/pwned_passwords_django/
+-rw-r--r--   0 james      (503) staff       (20)      124 2024-05-27 07:12:19.000000 pwned_passwords_django-5.0.0/src/pwned_passwords_django/__init__.py
+-rw-r--r--   0 james      (503) staff       (20)    11560 2024-02-26 05:27:25.000000 pwned_passwords_django-5.0.0/src/pwned_passwords_django/api.py
+-rw-r--r--   0 james      (503) staff       (20)      716 2024-02-23 06:56:55.000000 pwned_passwords_django-5.0.0/src/pwned_passwords_django/exceptions.py
+-rw-r--r--   0 james      (503) staff       (20)     8812 2024-02-27 06:54:28.000000 pwned_passwords_django-5.0.0/src/pwned_passwords_django/middleware.py
+-rw-r--r--   0 james      (503) staff       (20)     4922 2024-02-23 06:57:06.000000 pwned_passwords_django-5.0.0/src/pwned_passwords_django/validators.py
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 07:13:13.521470 pwned_passwords_django-5.0.0/src/pwned_passwords_django.egg-info/
+-rw-r--r--   0 james      (503) staff       (20)     4126 2024-05-27 07:13:13.000000 pwned_passwords_django-5.0.0/src/pwned_passwords_django.egg-info/PKG-INFO
+-rw-r--r--   0 james      (503) staff       (20)      968 2024-05-27 07:13:13.000000 pwned_passwords_django-5.0.0/src/pwned_passwords_django.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (503) staff       (20)        1 2024-05-27 07:13:13.000000 pwned_passwords_django-5.0.0/src/pwned_passwords_django.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (503) staff       (20)      203 2024-05-27 07:13:13.000000 pwned_passwords_django-5.0.0/src/pwned_passwords_django.egg-info/requires.txt
+-rw-r--r--   0 james      (503) staff       (20)       23 2024-05-27 07:13:13.000000 pwned_passwords_django-5.0.0/src/pwned_passwords_django.egg-info/top_level.txt
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 07:13:13.521309 pwned_passwords_django-5.0.0/tests/
+-rw-r--r--   0 james      (503) staff       (20)        0 2018-05-25 00:24:50.000000 pwned_passwords_django-5.0.0/tests/__init__.py
+-rw-r--r--   0 james      (503) staff       (20)     6701 2024-02-24 01:50:20.000000 pwned_passwords_django-5.0.0/tests/base.py
+-rw-r--r--   0 james      (503) staff       (20)      764 2024-02-23 06:55:59.000000 pwned_passwords_django-5.0.0/tests/settings.py
+-rw-r--r--   0 james      (503) staff       (20)    13630 2024-02-25 02:26:59.000000 pwned_passwords_django-5.0.0/tests/test_api.py
+-rw-r--r--   0 james      (503) staff       (20)     9793 2024-02-23 06:56:13.000000 pwned_passwords_django-5.0.0/tests/test_middleware.py
+-rw-r--r--   0 james      (503) staff       (20)     6517 2024-02-23 08:00:05.000000 pwned_passwords_django-5.0.0/tests/test_validators.py
+-rw-r--r--   0 james      (503) staff       (20)     2356 2024-02-23 06:56:31.000000 pwned_passwords_django-5.0.0/tests/urls.py
```

### Comparing `pwned-passwords-django-2.1/.pre-commit-config.yaml` & `pwned_passwords_django-5.0.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.5.0
+  rev: v4.6.0
   hooks:
     - id: check-added-large-files
     - id: check-ast
     - id: check-byte-order-marker
     - id: check-case-conflict
     - id: check-docstring-first
     - id: check-merge-conflict
     - id: check-toml
     - id: check-yaml
     - id: debug-statements
     - id: end-of-file-fixer
     - id: trailing-whitespace
 - repo: https://github.com/psf/black
-  rev: 24.2.0
+  rev: 24.4.2
   hooks:
     - id: black
       language_version: python3.12
       name: black (Python formatter)
 - repo: https://github.com/pycqa/flake8
   rev: 7.0.0
   hooks:
     - id: flake8
       name: flake8 (Python linter)
 - repo: https://github.com/econchick/interrogate
-  rev: 1.5.0
+  rev: 1.7.0
   hooks:
     - id: interrogate
       name: interrogate (Python docstring enforcer)
       args: [--quiet]
 - repo: https://github.com/pycqa/isort
   rev: 5.13.2
   hooks:
```

### Comparing `pwned-passwords-django-2.1/LICENSE` & `pwned_passwords_django-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pwned-passwords-django-2.1/PKG-INFO` & `pwned_passwords_django-5.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: pwned-passwords-django
-Version: 2.1
+Version: 5.0.0
 Summary: A Pwned Passwords implementation for Django sites.
 Author-email: James Bennett <james@b-list.org>
 License: BSD-3-Clause
 Project-URL: Documentation, https://pwned-passwords-django.readthedocs.io/
 Project-URL: Homepage, https://github.com/ubernostrum/pwned-passwords-django
 Keywords: django,security,passwords,auth,authentication
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -23,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: Django!=4.0.*,!=4.1.*,>=3.2
+Requires-Dist: Django>=4.2
 Requires-Dist: httpx
 Provides-Extra: docs
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinx-inline-tabs; extra == "docs"
 Requires-Dist: sphinx-notfound-page; extra == "docs"
```

### Comparing `pwned-passwords-django-2.1/README.rst` & `pwned_passwords_django-5.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pwned-passwords-django-2.1/docs/Makefile` & `pwned_passwords_django-5.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pwned-passwords-django-2.1/docs/api.rst` & `pwned_passwords_django-5.0.0/docs/api.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .. module:: pwned_passwords_django.api
 
 .. _api:
 
-Using the Pwned Passwords API directly
-======================================
+Direct Pwned Passwords API access
+=================================
 
 If :ref:`the validator <validator>` and :ref:`middleware <middleware>` do not
 meet your needs, you can also directly check a password against Pwned
 Passwords. The following two functions handle this use case, depending on
 whether you are writing synchronous or asynchronous Python:
 
 .. autofunction:: check_password
```

### Comparing `pwned-passwords-django-2.1/docs/changelog.rst` & `pwned_passwords_django-5.0.0/docs/changelog.rst`

 * *Files 18% similar despite different names*

```diff
@@ -3,35 +3,110 @@
 
 Changelog
 =========
 
 This document lists changes between released versions of
 ``pwned-passwords-django``.
 
-2.1 -- released 2024-02-26
---------------------------
+Version numbering
+-----------------
 
-No new features or bug fixes. Supported Django versions are now 3.2, 4.2, and
-5.0; supported Python versions are 3.8, 3.9, 3.10, 3.11, and 3.12.
+``pwned-passwords-django`` uses "DjangoVer", a version number system based on
+the corresponding supported Django versions. The format of a
+``pwned-passwords-django`` version number is ``A.B.C``, where ``A.B`` is the
+version number of the latest Django feature release supported by that version
+of ``pwned-passwords-django``, and ``C`` is an incrementing value for releases
+of ``pwned-passwords-django`` paired to that Django feature release.
+
+The policy of ``pwned-passwords-django`` is to support the Django feature
+release indicated in the version number, along with any other lower-numbered
+Django feature releases receiving support from the Django project at the time
+of release.
+
+For example, consider a hypothetical ``pwned-passwords-django`` version
+5.0.2. This indicates that the most recent supported Django feature release is
+5.0, and that it is the third release of ``pwned-passwords-django`` to support
+Django 5.0 (after 5.0.0 and 5.0.1). Since the Django project at the time was
+supporting Django 5.0 and 4.2, that version of ``pwned-passwords-django`` would
+also support Django 5.0 and 4.2.
+
+
+API stability and deprecations
+------------------------------
+
+The API stability/deprecation policy for ``pwned-passwords-django`` is as follows:
+
+* The supported stable public API is the set of symbols which are documented in
+  this documentation. For classes, the supported stable public API is the set
+  of methods and attributes of those classes whose names do not begin with one
+  or more underscore (``_``) characters and which are documented in this
+  documentation.
+
+* When a public API is to be removed, or undergo a backwards-incompatible
+  change, it will emit a deprecation warning which serves as notice of the
+  intended removal or change. This warning will be emitted for at least two
+  releases, after which the removal or change may occur without further
+  warning. This is different from Django's own deprecation policy, which avoids
+  completing a removal/change in "LTS"-designated releases. Since
+  ``pwned-passwords-django`` does not have "LTS" releases, it does not need
+  that exception.
+
+* Security fixes, and fixes for high-severity bugs (such as those which might
+  cause unrecoverable crash or data loss), are not required to emit deprecation
+  warnings, and may -- if needed -- impose backwards-incompatible change in any
+  release. If this occurs, this changelog document will contain a note
+  explaining why the usual deprecation process could not be followed for that
+  case.
 
-Source code formatting was updated to Black 2024 style.
+* This policy is in effect as of the adoption of "DjangoVer" versioning, with
+  version 5.0.0 of ``pwned-passwords-django``.
 
-Some internal test code was rewritten to use HTTPX ``MockTransport`` objects.
 
+Releases under DjangoVer
+------------------------
 
-2.0 -- released 2023-03-26
---------------------------
+Version 5.0.0
+~~~~~~~~~~~~~
 
-Major version bump. Much of the codebase has been rewritten and improved.
+Released May 2024
 
-The following changes in 2.0 are backwards-incompatible with 1.x releases:
+* Adopted "DjangoVer" versioning.
+
+* Supported Django versions are now 4.2 and 5.0.
+
+* Expanded/reorganized documentation.
 
 
+Releases not under DjangoVer
+----------------------------
+
+Version 2.1
+~~~~~~~~~~~
+
+Released February 2024
+
+* Supported Django versions are now 3.2, 4.2, and 5.0; supported Python
+  versions are 3.8, 3.9, 3.10, 3.11, and 3.12.
+
+* Source code formatting was updated to Black 2024 style.
+
+* Some internal test code was rewritten to use HTTPX ``MockTransport`` objects.
+
+
+Version 2.0
+~~~~~~~~~~~
+
+Released March 2023
+
+* Major version bump. Much of the codebase has been rewritten and improved.
+
+The following changes in 2.0 are backwards-incompatible with 1.x releases:
+
 Configuration changes
-~~~~~~~~~~~~~~~~~~~~~
++++++++++++++++++++++
 
 In 1.x, ``pwned-passwords-django`` was configured by two top-level Django
 settings: ``PWNED_PASSWORDS_API_TIMEOUT`` and ``PWNED_PASSWORDS_REGEX``. As of
 2.0, configuration uses one top-level Django setting, ``PWNED_PASSWORDS``,
 which is a :class:`dict` containing any of :ref:`several optional keys
 <settings>` to configure behavior.
 
@@ -50,26 +125,26 @@
    PWNED_PASSWORDS = {
        "API_TIMEOUT": 1.5, # one and a half seconds
        "PASSWORD_REGEX": r"TOKEN",
    }
 
 
 Validator changes
-~~~~~~~~~~~~~~~~~
++++++++++++++++++
 
 In 1.x, when the password validator encountered an error communicating with
 Pwned Passwords, it would fall back to Django's
 :class:`~django.contrib.auth.password_validation.CommonPasswordValidator` after
 logging a message of log level :data:`logging.WARNING`. In 2.0, it continues to
 fall back to ``CommonPasswordValidator``, but the log message is now of log
 level :data:`logging.ERROR`.
 
 
 Middleware changes
-~~~~~~~~~~~~~~~~~~
+++++++++++++++++++
 
 In 1.x, the middleware was a class --
 ``pwned_passwords_django.middleware.PwnedPasswordsMiddleware`` -- while in 2.0
 it is a factory function,
 :func:`pwned_passwords_django.middleware.pwned_passwords_middleware`. If you
 were using the middleware, you will need to update your :setting:`MIDDLEWARE`
 setting.
@@ -100,15 +175,15 @@
 
 Also, as with the validator, the log message recorded when an error occurs
 communicating with Pwned Passwords has been changed from log level
 :data:`logging.WARNING` to :data:`logging.ERROR`.
 
 
 Direct API changes
-~~~~~~~~~~~~~~~~~~
+++++++++++++++++++
 
 In 1.x, direct access to the Pwned Passwords API was available through the
 function ``pwned_passwords_django.api.pwned_password``, which took a password
 and returned either the count of times it had been breached, or :data:`None` in
 the event of an error.
 
 In 2.0, this has been replaced by two functions: the synchronous
@@ -124,15 +199,15 @@
 A new :class:`~pwned_passwords_django.api.PwnedPasswords` API client class is
 also provided; the above-mentioned functions are aliases to methods of a
 default instance of this client class. See :ref:`the direct API access
 documentation <api>` for details of how it may be used and customized.
 
 
 Error handling changes
-~~~~~~~~~~~~~~~~~~~~~~
+++++++++++++++++++++++
 
 In 1.x, errors were caught and handled in a variety of different ways by
 different parts of ``pwned-passwords-django``. In 2.0, error handling is much
 more unified:
 
 * All external exceptions raised when communicating with Pwned Passwords are
   caught and wrapped in
@@ -156,15 +231,15 @@
 minimizes the amount of information reported for unknown/unanticipated
 exceptions, to further reduce the risk of this issue.
 
 See :ref:`the error-handling documentation <error-handling>` for details.
 
 
 Dependency changes
-~~~~~~~~~~~~~~~~~~
+++++++++++++++++++
 
 In 1.x, the underlying HTTP client library for communicating with Pwned
 Passwords was `requests <https://requests.readthedocs.io/en/latest/>`_. In 2.0,
 it is `HTTPX <https://www.python-httpx.org>`_, which is broadly API-compatible
 but provides several additional features (such as async support). The new
 :class:`~pwned_passwords_django.api.PwnedPasswords` API client class can use an
 instance of any object API-compatible with ``httpx.Client`` as its synchronous
@@ -177,88 +252,99 @@
 with alternate HTTP clients).
 
 In 1.x, the test suite and continuous integration of ``pwned-passwords-django``
 were orchestrated using the ``tox`` automation tool. In 2.0, they are
 orchestrated using `nox <https://nox.thea.codes/en/stable/>`_ instead.
 
 
-1.6.1 -- released 2022-12-26
-----------------------------
+Version 1.6.1
+~~~~~~~~~~~~~
+
+Released December 2022
 
-"Bugfix" release: the Pwned Passwords API now sometimes returns the count as a
-value with a comma in it, which requires additional handling. No other changes;
-a release for official compatibility with Python 3.11 and Django 4.1 will occur
-later.
+* Bugfix release: the Pwned Passwords API was reported to sometimes return the
+  count as a value with a comma in it, which requires additional handling. No
+  other changes; a release for official compatibility with Python 3.11 and
+  Django 4.1 will occur later.
 
-1.6 -- released 2022-05-19
---------------------------
 
-No new features. No new bug fixes. Django 4.0 is now supported. Python 3.6,
-Django 2.2, and Django 3.1 are no longer supported, as they have reached the
-end of their upstream support cycles.
+Version 1.6
+~~~~~~~~~~~
 
-1.5 -- released 2021-06-21
---------------------------
+Released May 2022
 
-No new features. No bug fixes. Django 3.2 is now supported; Django 3.0 and
-Python 3.5 are no longer supported, as they have both reached the end of their
-upstream support cycles.
+* Django 4.0 is now supported. Python 3.6, Django 2.2, and Django 3.1 are no
+  longer supported, as they have reached the end of their upstream support
+  cycles.
 
-1.4 -- released 2020-01-28
---------------------------
 
-New features:
-~~~~~~~~~~~~~
+Version 1.5
+~~~~~~~~~~~
+
+Released June 2021
+
+* Django 3.2 is now supported; Django 3.0 and Python 3.5 are no longer
+  supported, as they have both reached the end of their upstream support
+  cycles.
+
+
+Version 1.4
+~~~~~~~~~~~
+
+Released January 2020
 
 * The :class:`~pwned_passwords_django.validators.PwnedPasswordsValidator` is
   now serializable. This is unlikely to be useful, however, as the validator is
   not intended to be attached to a model.
 
-Other changes:
-~~~~~~~~~~~~~~
-
 * The supported versions of Django are now 2.2 and 3.0. This means Python 2
   support is dropped; if you still need to use ``pwned-passwords-django`` on
   Python 2 with Django 1.11, stay with the 1.3 release series of
   ``pwned-passwords-django``.
 
-1.3.2 -- released 2019-05-07
-----------------------------
 
-No new features. No bug fixes. Released to add explicit markers of Django 2.2
-compatibility.
+Version 1.3.2
+~~~~~~~~~~~~~
 
+Released May 2019
 
-1.3.1 -- released 2018-09-18
-----------------------------
+* Released to add explicit markers of Django 2.2 compatibility.
 
-Released to include documentation updates which were inadvertently left out of
-the 1.3 package.
 
+Version 1.3.1
+~~~~~~~~~~~~~
 
-1.3 -- released 2018-09-18
---------------------------
+Released September 2018
 
-No new features. No bug fixes. Released only to add explicit markers of Python
-3.7 and Django 2.1 compatibility.
+* Released to include documentation updates which were inadvertently left out
+  of the 1.3 package.
 
 
-1.2.1 -- released 2018-06-18
-----------------------------
+Version 1.3
+~~~~~~~~~~~
 
-Released to correct the date of the 1.2 release listed in this changelog
-document. No other changes.
+Released September 2018
 
+* Released to add explicit markers of Python 3.7 and Django 2.1 compatibility.
 
-1.2 -- released 2018-06-18
---------------------------
 
-New features:
+Version 1.2.1
 ~~~~~~~~~~~~~
 
+Released June 2018
+
+* Released to correct the date of the 1.2 release listed in this changelog
+  document.
+
+
+Version 1.2
+~~~~~~~~~~~
+
+Released June 2018
+
 * Password-validator error messages are now :ref:`customizable
   <validator-messages>`.
 
 * The request-timeout value for contacting the Pwned Passwords API defaults to
   one second, and is customizable via the setting
   :data:`~django.conf.settings.PWNED_PASSWORDS_API_TIMEOUT`.
 
@@ -268,22 +354,14 @@
   back to
   :class:`~django.contrib.auth.password_validation.CommonPasswordValidator`,
   which has a smaller list of common passwords. The
   :class:`~pwned_passwords_django.middleware.PwnedPasswordsMiddleware` does not
   have a fallback behavior; :func:`~pwned_passwords_django.api.pwned_password`
   will return :data:`None` to indicate the error case.
 
-Bugs fixed:
-~~~~~~~~~~~
-
-N/A
-
-Other changes:
-~~~~~~~~~~~~~~
-
 * :func:`~pwned_passwords_django.api.pwned_password` will now raise
   :exc:`TypeError` if its argument is not a Unicode string (the type
   :class:`unicode` on Python 2, :class:`str` on Python 3). This is debatably
   backwards-incompatible; :func:`~pwned_passwords_django.api.pwned_password`
   encodes its argument to UTF-8 bytes, which will raise :exc:`AttributeError`
   if attempted on a :class:`bytes` object in Python 3. As a result, all
   supported environments other than Python 2.7/Django 1.11 would already raise
@@ -303,32 +381,23 @@
   back to
   :class:`~django.contrib.auth.password_validation.CommonPasswordValidator`
   when the Pwned Passwords API is unresponsive, this provides consistency of
   messages, and also ensures the messages are translated (Django provides
   translations for its built-in messages).
 
 
-1.1 -- released 2018-03-06
-----------------------------
-
-New features:
-~~~~~~~~~~~~~
-
-N/A
-
-Bugs fixed:
+Version 1.1
 ~~~~~~~~~~~
 
-* Case sensitivity issue. The Pwned Passwords API always uses uppercase
+Released March 2018
+
+* Fixed case sensitivity issue. The Pwned Passwords API always uses uppercase
   hexadecimal digits for password hashes; ``pwned-passwords-django`` was using
   lowercase. Fixed by switching ``pwned-passwords-django`` to use uppercase.
 
-Other changes
-~~~~~~~~~~~~~
-
-N/A
 
+Version 1.0
+~~~~~~~~~~~
 
-1.0 -- released 2018-03-06
---------------------------
+Released March 2018
 
-Initial public release.
+* Initial public release.
```

### Comparing `pwned-passwords-django-2.1/docs/conf.py` & `pwned_passwords_django-5.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pwned-passwords-django-2.1/docs/exceptions.rst` & `pwned_passwords_django-5.0.0/docs/exceptions.rst`

 * *Files identical despite different names*

### Comparing `pwned-passwords-django-2.1/docs/faq.rst` & `pwned_passwords_django-5.0.0/docs/faq.rst`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 The following notes answer some common questions, and may be useful to you when
 using ``pwned-passwords-django``.
 
 
 What versions of Django and Python are supported?
 -------------------------------------------------
 
-``pwned-passwords-django`` |release| supports Django 3.2, 4.2, and 5.0, and
-Python 3.8 through 3.12. See `Django's Python support matrix
+``pwned-passwords-django`` |release| supports Django 4.2, and 5.0, and Python
+3.8 through 3.12. See `Django's Python support matrix
 <https://docs.djangoproject.com/en/dev/faq/install/#what-python-version-can-i-use-with-django>`_
 for details of which Python versions are compatible with each version of
 Django.
 
 
 Should I use the validator, the middleware, or the API directly?
 ----------------------------------------------------------------
@@ -140,15 +140,15 @@
 
    .. code-block:: shell
 
       py -m nox --python "3.10"
 
 By default, ``nox`` will only run the tasks whose associated Python versions
 are available on your system. For example, if you have only Python 3.8 and 3.9
-installed, test runs for Python 3.7, 3.10, and 3.11 would be skipped.
+installed, test runs for Python 3.10, 3.11, and 3.12 would be skipped.
 
 
 How am I allowed to use this code?
 ----------------------------------
 
 ``pwned-passwords-django`` is distributed under a `three-clause BSD license
 <http://opensource.org/licenses/BSD-3-Clause>`_. This is an open-source license
```

### Comparing `pwned-passwords-django-2.1/docs/index.rst` & `pwned_passwords_django-5.0.0/docs/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-``pwned-passwords-django`` |release|
-====================================
+pwned-passwords-django |release|
+================================
 
 ``pwned-passwords-django`` provides helpers for working with the `Pwned
 Passwords database from Have I Been Pwned
 <https://haveibeenpwned.com/Passwords>`_ in `Django
 <https://www.djangoproject.com/>`_ powered sites. Pwned Passwords is an
 extremely large database of passwords known to have been compromised through
 data breaches, and is useful as a tool for rejecting common or weak passwords.
@@ -56,22 +56,34 @@
    ]
 
 
 Documentation contents
 ----------------------
 
 .. toctree::
+   :caption: Installation and usage
    :maxdepth: 1
 
    install
+   usage
+
+.. toctree::
+   :caption: API reference
+   :maxdepth: 1
+
    validator
    middleware
    api
    exceptions
    settings
+
+.. toctree::
+   :caption: Other documentation
+   :maxdepth: 1
+
    faq
    changelog
 
 
 .. seealso::
 
   * `About Have I Been Pwned <https://haveibeenpwned.com/About>`_
```

### Comparing `pwned-passwords-django-2.1/docs/install.rst` & `pwned_passwords_django-5.0.0/docs/install.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. _install:
 
 
 Installation guide
 ==================
 
-``pwned-passwords-django`` |release| supports Django 3.2, 4.2, and 5.0, and Python
+``pwned-passwords-django`` |release| supports Django 4.2 and 5.0, and Python
 3.8 through 3.12. See `Django's Python support matrix
 <https://docs.djangoproject.com/en/dev/faq/install/#what-python-version-can-i-use-with-django>`_
 for details of which Python versions are compatible with each version of
 Django.
 
 Installing ``pwned-passwords-django``
 -------------------------------------
```

### Comparing `pwned-passwords-django-2.1/docs/make.bat` & `pwned_passwords_django-5.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pwned-passwords-django-2.1/docs/settings.rst` & `pwned_passwords_django-5.0.0/docs/settings.rst`

 * *Files identical despite different names*

### Comparing `pwned-passwords-django-2.1/docs/validator.rst` & `pwned_passwords_django-5.0.0/docs/validator.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. module:: pwned_passwords_django.validators
 
 .. _validator:
 
 
-Using the password validator
-============================
+The password validator
+======================
 
 .. class:: PwnedPasswordsValidator
 
    Django's auth system (located in ``django.contrib.auth``) includes `a
    configurable password-validation framework
    <https://docs.djangoproject.com/en/stable/topics/auth/passwords/#module-django.contrib.auth.password_validation>`_
    with several built-in validators, and ``pwned-passwords-django`` provides an
```

### Comparing `pwned-passwords-django-2.1/noxfile.py` & `pwned_passwords_django-5.0.0/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,23 +54,21 @@
 # -----------------------------------------------------------------------------------
 
 
 @nox.session(tags=["tests"])
 @nox.parametrize(
     "python,django",
     [
-        # Python/Django testing matrix. Tests Django 3.2, 4.2, 5.0, on Python 3.8
-        # through 3.11, skipping unsupported combinations.
+        # Python/Django testing matrix. Tests Django 4. and, 5.0, on Python 3.8 through
+        # 3.12, skipping unsupported combinations.
         (python, django)
         for python in ["3.8", "3.9", "3.10", "3.11", "3.12"]
-        for django in ["3.2", "4.2", "5.0"]
+        for django in ["4.2", "5.0"]
         if (python, django)
         not in [
-            ("3.11", "3.2"),
-            ("3.12", "3.2"),
             ("3.8", "5.0"),
             ("3.9", "5.0"),
         ]
     ],
 )
 def tests_with_coverage(session: nox.Session, django: str) -> None:
     """
@@ -111,15 +109,15 @@
     clean()
 
 
 # Tasks which test the package's documentation.
 # -----------------------------------------------------------------------------------
 
 
-@nox.session(python=["3.11"], tags=["docs"])
+@nox.session(python=["3.12"], tags=["docs"])
 def docs_build(session: nox.Session) -> None:
     """
     Build the package's documentation as HTML.
 
     """
     session.install(".[docs]")
     session.chdir("docs")
@@ -133,15 +131,15 @@
         f"{session.bin}/../tmp/doctrees",
         ".",
         f"{session.bin}/../tmp/html",
     )
     clean()
 
 
-@nox.session(python=["3.11"], tags=["docs"])
+@nox.session(python=["3.12"], tags=["docs"])
 def docs_docstrings(session: nox.Session) -> None:
     """
     Enforce the presence of docstrings on all modules, classes, functions, and
     methods.
 
     """
     session.install("interrogate")
@@ -156,15 +154,15 @@
         "src/",
         "tests/",
         "noxfile.py",
     )
     clean()
 
 
-@nox.session(python=["3.11"], tags=["docs"])
+@nox.session(python=["3.12"], tags=["docs"])
 def docs_spellcheck(session: nox.Session) -> None:
     """
     Spell-check the package's documentation.
 
     """
     session.install("pyenchant", "sphinxcontrib-spelling", ".[docs]")
     build_dir = session.create_tmp()
@@ -191,15 +189,15 @@
 # Code formatting checks.
 #
 # These checks do *not* reformat code -- that happens in pre-commit hooks -- but will
 # fail a CI build if they find any code that needs reformatting.
 # -----------------------------------------------------------------------------------
 
 
-@nox.session(python=["3.11"], tags=["formatters"])
+@nox.session(python=["3.12"], tags=["formatters"])
 def format_black(session: nox.Session) -> None:
     """
     Check code formatting with Black.
 
     """
     session.install("black>=24.0,<25.0")
     session.run(f"{session.bin}/python{session.python}", "-Im", "black", "--version")
@@ -213,15 +211,15 @@
         "tests/",
         "docs/",
         "noxfile.py",
     )
     clean()
 
 
-@nox.session(python=["3.11"], tags=["formatters"])
+@nox.session(python=["3.12"], tags=["formatters"])
 def format_isort(session: nox.Session) -> None:
     """
     Check code formating with Black.
 
     """
     session.install("isort")
     session.run(f"{session.bin}/python{session.python}", "-Im", "isort", "--version")
@@ -239,15 +237,15 @@
     clean()
 
 
 # Linters.
 # -----------------------------------------------------------------------------------
 
 
-@nox.session(python=["3.11"], tags=["linters", "security"])
+@nox.session(python=["3.12"], tags=["linters", "security"])
 def lint_bandit(session: nox.Session) -> None:
     """
     Lint code with the Bandit security analyzer.
 
     """
     session.install("bandit[toml]")
     session.run(f"{session.bin}/python{session.python}", "-Im", "bandit", "--version")
@@ -260,15 +258,15 @@
         "-r",
         "src/",
         "tests/",
     )
     clean()
 
 
-@nox.session(python=["3.11"], tags=["linters"])
+@nox.session(python=["3.12"], tags=["linters"])
 def lint_flake8(session: nox.Session) -> None:
     """
     Lint code with flake8.
 
     """
     session.install("flake8", "flake8-bugbear")
     session.run(f"{session.bin}/python{session.python}", "-Im", "flake8", "--version")
@@ -280,15 +278,15 @@
         "tests/",
         "docs/",
         "noxfile.py",
     )
     clean()
 
 
-@nox.session(python=["3.11"], tags=["linters"])
+@nox.session(python=["3.12"], tags=["linters"])
 def lint_pylint(session: nox.Session) -> None:
     """
     Lint code with Pyling.
 
     """
     # Pylint requires that all dependencies be importable during the run. This package
     # does not have any direct dependencies, nor does the normal test suite, but the
@@ -299,27 +297,27 @@
     session.run(f"python{session.python}", "-Im", "pylint", "src/", "tests/")
 
 
 # Packaging checks.
 # -----------------------------------------------------------------------------------
 
 
-@nox.session(python=["3.11"], tags=["packaging"])
+@nox.session(python=["3.12"], tags=["packaging"])
 def package_build(session: nox.Session) -> None:
     """
     Check that the package builds.
 
     """
     clean()
     session.install("build")
     session.run(f"{session.bin}/python{session.python}", "-Im", "build", "--version")
     session.run(f"{session.bin}/python{session.python}", "-Im", "build")
 
 
-@nox.session(python=["3.11"], tags=["packaging"])
+@nox.session(python=["3.12"], tags=["packaging"])
 def package_description(session: nox.Session) -> None:
     """
     Check that the package description will render on the Python Package Index.
 
     """
     package_dir = session.create_tmp()
     session.install("build", "twine")
@@ -339,15 +337,15 @@
         "twine",
         "check",
         f"{package_dir}/build/*",
     )
     clean()
 
 
-@nox.session(python=["3.11"], tags=["packaging"])
+@nox.session(python=["3.12"], tags=["packaging"])
 def package_manifest(session: nox.Session) -> None:
     """
     Check that the set of files in the package matches the set under version control.
 
     """
     session.install("check-manifest")
     session.run(
@@ -355,15 +353,15 @@
     )
     session.run(
         f"{session.bin}/python{session.python}", "-Im", "check_manifest", "--verbose"
     )
     clean()
 
 
-@nox.session(python=["3.11"], tags=["packaging"])
+@nox.session(python=["3.12"], tags=["packaging"])
 def package_pyroma(session: nox.Session) -> None:
     """
     Check package quality with pyroma.
 
     """
     session.install("pyroma")
     session.run(
@@ -371,15 +369,15 @@
         "-c",
         'from importlib.metadata import version; print(version("pyroma"))',
     )
     session.run(f"{session.bin}/python{session.python}", "-Im", "pyroma", ".")
     clean()
 
 
-@nox.session(python=["3.11"], tags=["packaging"])
+@nox.session(python=["3.12"], tags=["packaging"])
 def package_wheel(session: nox.Session) -> None:
     """
     Check the built wheel package for common errors.
 
     """
     package_dir = session.create_tmp()
     session.install("build", "check-wheel-contents")
```

### Comparing `pwned-passwords-django-2.1/pyproject.toml` & `pwned_passwords_django-5.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 authors = [
   {name = "James Bennett", email = "james@b-list.org"}
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Web Environment",
   "Framework :: Django",
-  "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.2",
   "Framework :: Django :: 5.0",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
@@ -24,15 +23,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Utilities",
 ]
 name = "pwned-passwords-django"
 description = "A Pwned Passwords implementation for Django sites."
 dependencies = [
-  "Django>=3.2,!=4.0.*,!=4.1.*",
+  "Django>=4.2",
   "httpx"
 ]
 dynamic = ["version"]
 keywords = ["django", "security", "passwords", "auth", "authentication"]
 license = {text = "BSD-3-Clause"}
 readme = "README.rst"
 requires-python = ">=3.8"
```

### Comparing `pwned-passwords-django-2.1/src/pwned_passwords_django/api.py` & `pwned_passwords_django-5.0.0/src/pwned_passwords_django/api.py`

 * *Files identical despite different names*

### Comparing `pwned-passwords-django-2.1/src/pwned_passwords_django/exceptions.py` & `pwned_passwords_django-5.0.0/src/pwned_passwords_django/exceptions.py`

 * *Files identical despite different names*

### Comparing `pwned-passwords-django-2.1/src/pwned_passwords_django/middleware.py` & `pwned_passwords_django-5.0.0/src/pwned_passwords_django/middleware.py`

 * *Files identical despite different names*

### Comparing `pwned-passwords-django-2.1/src/pwned_passwords_django/validators.py` & `pwned_passwords_django-5.0.0/src/pwned_passwords_django/validators.py`

 * *Files identical despite different names*

### Comparing `pwned-passwords-django-2.1/src/pwned_passwords_django.egg-info/PKG-INFO` & `pwned_passwords_django-5.0.0/src/pwned_passwords_django.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: pwned-passwords-django
-Version: 2.1
+Version: 5.0.0
 Summary: A Pwned Passwords implementation for Django sites.
 Author-email: James Bennett <james@b-list.org>
 License: BSD-3-Clause
 Project-URL: Documentation, https://pwned-passwords-django.readthedocs.io/
 Project-URL: Homepage, https://github.com/ubernostrum/pwned-passwords-django
 Keywords: django,security,passwords,auth,authentication
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -23,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: Django!=4.0.*,!=4.1.*,>=3.2
+Requires-Dist: Django>=4.2
 Requires-Dist: httpx
 Provides-Extra: docs
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinx-inline-tabs; extra == "docs"
 Requires-Dist: sphinx-notfound-page; extra == "docs"
```

### Comparing `pwned-passwords-django-2.1/src/pwned_passwords_django.egg-info/SOURCES.txt` & `pwned_passwords_django-5.0.0/src/pwned_passwords_django.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 docs/faq.rst
 docs/index.rst
 docs/install.rst
 docs/make.bat
 docs/middleware.rst
 docs/settings.rst
 docs/spelling_wordlist.txt
+docs/usage.rst
 docs/validator.rst
 src/pwned_passwords_django/__init__.py
 src/pwned_passwords_django/api.py
 src/pwned_passwords_django/exceptions.py
 src/pwned_passwords_django/middleware.py
 src/pwned_passwords_django/validators.py
 src/pwned_passwords_django.egg-info/PKG-INFO
```

### Comparing `pwned-passwords-django-2.1/tests/base.py` & `pwned_passwords_django-5.0.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `pwned-passwords-django-2.1/tests/settings.py` & `pwned_passwords_django-5.0.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `pwned-passwords-django-2.1/tests/test_api.py` & `pwned_passwords_django-5.0.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pwned-passwords-django-2.1/tests/test_middleware.py` & `pwned_passwords_django-5.0.0/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `pwned-passwords-django-2.1/tests/test_validators.py` & `pwned_passwords_django-5.0.0/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `pwned-passwords-django-2.1/tests/urls.py` & `pwned_passwords_django-5.0.0/tests/urls.py`

 * *Files identical despite different names*

