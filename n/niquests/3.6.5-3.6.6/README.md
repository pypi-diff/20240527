# Comparing `tmp/niquests-3.6.5.tar.gz` & `tmp/niquests-3.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed May 22 05:50:20 2024, max compression
+gzip compressed data, last modified: Mon May 27 05:48:00 2024, max compression
```

## Comparing `niquests-3.6.5.tar` & `niquests-3.6.6.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      718 2024-05-22 05:50:20.000000 niquests-3.6.5/AUTHORS.rst
--rw-r--r--   0        0        0    87660 2024-05-22 05:50:20.000000 niquests-3.6.5/HISTORY.md
--rw-r--r--   0        0        0      377 2024-05-22 05:50:20.000000 niquests-3.6.5/Makefile
--rw-r--r--   0        0        0       38 2024-05-22 05:50:20.000000 niquests-3.6.5/NOTICE
--rw-r--r--   0        0        0      201 2024-05-22 05:50:20.000000 niquests-3.6.5/SECURITY.md
--rw-r--r--   0        0        0      233 2024-05-22 05:50:20.000000 niquests-3.6.5/requirements-dev.txt
--rw-r--r--   0        0        0        1 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/.nojekyll
--rw-r--r--   0        0        0     7664 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/Makefile
--rw-r--r--   0        0        0     5355 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/api.rst
--rw-r--r--   0        0        0    12305 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/conf.py
--rw-r--r--   0        0        0     4084 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/index.rst
--rw-r--r--   0        0        0     7253 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/make.bat
--rw-r--r--   0        0        0      185 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/requirements.txt
--rw-r--r--   0        0        0     2990 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/_static/custom.css
--rw-r--r--   0        0        0   306086 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/_static/requests-sidebar.png
--rw-r--r--   0        0        0     7360 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/community/faq.rst
--rw-r--r--   0        0        0     2720 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/community/recommended.rst
--rw-r--r--   0        0        0     1782 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/community/release-process.rst
--rw-r--r--   0        0        0      285 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/community/support.rst
--rw-r--r--   0        0        0      324 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/community/updates.rst
--rw-r--r--   0        0        0      945 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/community/vulnerabilities.rst
--rw-r--r--   0        0        0       48 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/dev/authors.rst
--rw-r--r--   0        0        0     5768 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/dev/contributing.rst
--rw-r--r--   0        0        0     1885 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/dev/migrate.rst
--rw-r--r--   0        0        0    52818 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/user/advanced.rst
--rw-r--r--   0        0        0     6315 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/user/authentication.rst
--rw-r--r--   0        0        0     1046 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/user/install.rst
--rw-r--r--   0        0        0    34594 2024-05-22 05:50:20.000000 niquests-3.6.5/docs/user/quickstart.rst
--rw-r--r--   0        0        0     2805 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/__init__.py
--rw-r--r--   0        0        0      534 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/__version__.py
--rw-r--r--   0        0        0    47165 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/_async.py
--rw-r--r--   0        0        0     2852 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/_compat.py
--rw-r--r--   0        0        0      480 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/_constant.py
--rw-r--r--   0        0        0     5942 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/_typing.py
--rw-r--r--   0        0        0    87323 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/adapters.py
--rw-r--r--   0        0        0    27567 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/api.py
--rw-r--r--   0        0        0     9906 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/auth.py
--rw-r--r--   0        0        0    20648 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/cookies.py
--rw-r--r--   0        0        0     4363 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/exceptions.py
--rw-r--r--   0        0        0     5248 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/help.py
--rw-r--r--   0        0        0     2776 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/hooks.py
--rw-r--r--   0        0        0    62733 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/models.py
--rw-r--r--   0        0        0        0 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/py.typed
--rw-r--r--   0        0        0    69459 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/sessions.py
--rw-r--r--   0        0        0     4284 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/status_codes.py
--rw-r--r--   0        0        0     7042 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/structures.py
--rw-r--r--   0        0        0    37956 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/utils.py
--rw-r--r--   0        0        0      119 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/extensions/__init__.py
--rw-r--r--   0        0        0    22400 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/extensions/_async_ocsp.py
--rw-r--r--   0        0        0    21160 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/extensions/_ocsp.py
--rw-r--r--   0        0        0    16942 2024-05-22 05:50:20.000000 niquests-3.6.5/src/niquests/extensions/_picotls.py
--rw-r--r--   0        0        0       80 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/__init__.py
--rw-r--r--   0        0        0     2619 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/conftest.py
--rw-r--r--   0        0        0     7540 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/test_async.py
--rw-r--r--   0        0        0      875 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/test_help.py
--rw-r--r--   0        0        0      893 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/test_hooks.py
--rw-r--r--   0        0        0     4022 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/test_live.py
--rw-r--r--   0        0        0    15985 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/test_lowlevel.py
--rw-r--r--   0        0        0     3722 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/test_multiplexed.py
--rw-r--r--   0        0        0   100346 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/test_requests.py
--rw-r--r--   0        0        0     2725 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/test_structures.py
--rw-r--r--   0        0        0     6213 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/test_testserver.py
--rw-r--r--   0        0        0    26728 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/test_utils.py
--rw-r--r--   0        0        0      613 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/utils.py
--rw-r--r--   0        0        0        0 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/testserver/__init__.py
--rw-r--r--   0        0        0     3882 2024-05-22 05:50:20.000000 niquests-3.6.5/tests/testserver/server.py
--rw-r--r--   0        0        0      362 2024-05-22 05:50:20.000000 niquests-3.6.5/.gitignore
--rw-r--r--   0        0        0    10142 2024-05-22 05:50:20.000000 niquests-3.6.5/LICENSE
--rw-r--r--   0        0        0    10882 2024-05-22 05:50:20.000000 niquests-3.6.5/README.md
--rw-r--r--   0        0        0     3660 2024-05-22 05:50:20.000000 niquests-3.6.5/pyproject.toml
--rw-r--r--   0        0        0    13241 2024-05-22 05:50:20.000000 niquests-3.6.5/PKG-INFO
+-rw-r--r--   0        0        0      718 2024-05-27 05:48:00.000000 niquests-3.6.6/AUTHORS.rst
+-rw-r--r--   0        0        0    87814 2024-05-27 05:48:00.000000 niquests-3.6.6/HISTORY.md
+-rw-r--r--   0        0        0      377 2024-05-27 05:48:00.000000 niquests-3.6.6/Makefile
+-rw-r--r--   0        0        0       38 2024-05-27 05:48:00.000000 niquests-3.6.6/NOTICE
+-rw-r--r--   0        0        0      201 2024-05-27 05:48:00.000000 niquests-3.6.6/SECURITY.md
+-rw-r--r--   0        0        0      233 2024-05-27 05:48:00.000000 niquests-3.6.6/requirements-dev.txt
+-rw-r--r--   0        0        0        1 2024-05-27 05:48:00.000000 niquests-3.6.6/docs/.nojekyll
+-rw-r--r--   0        0        0     7664 2024-05-27 05:48:00.000000 niquests-3.6.6/docs/Makefile
+-rw-r--r--   0        0        0     5355 2024-05-27 05:48:00.000000 niquests-3.6.6/docs/api.rst
+-rw-r--r--   0        0        0    12305 2024-05-27 05:48:00.000000 niquests-3.6.6/docs/conf.py
+-rw-r--r--   0        0        0     4084 2024-05-27 05:48:00.000000 niquests-3.6.6/docs/index.rst
+-rw-r--r--   0        0        0     7253 2024-05-27 05:48:00.000000 niquests-3.6.6/docs/make.bat
+-rw-r--r--   0        0        0      185 2024-05-27 05:48:00.000000 niquests-3.6.6/docs/requirements.txt
+-rw-r--r--   0        0        0     2990 2024-05-27 05:48:00.000000 niquests-3.6.6/docs/_static/custom.css
+-rw-r--r--   0        0        0   306086 2024-05-27 05:48:00.000000 niquests-3.6.6/docs/_static/requests-sidebar.png
+-rw-r--r--   0        0        0     7360 2024-05-27 05:48:00.000000 niquests-3.6.6/docs/community/faq.rst
+-rw-r--r--   0        0        0     2720 2024-05-27 05:48:00.000000 niquests-3.6.6/docs/community/recommended.rst
+-rw-r--r--   0        0        0     1782 2024-05-27 05:48:00.000000 niquests-3.6.6/docs/community/release-process.rst
+-rw-r--r--   0        0        0      285 2024-05-27 05:48:00.000000 niquests-3.6.6/docs/community/support.rst
+-rw-r--r--   0        0        0      324 2024-05-27 05:48:00.000000 niquests-3.6.6/docs/community/updates.rst
+-rw-r--r--   0        0        0      945 2024-05-27 05:48:00.000000 niquests-3.6.6/docs/community/vulnerabilities.rst
+-rw-r--r--   0        0        0       48 2024-05-27 05:48:00.000000 niquests-3.6.6/docs/dev/authors.rst
+-rw-r--r--   0        0        0     5768 2024-05-27 05:48:00.000000 niquests-3.6.6/docs/dev/contributing.rst
+-rw-r--r--   0        0        0     1885 2024-05-27 05:48:00.000000 niquests-3.6.6/docs/dev/migrate.rst
+-rw-r--r--   0        0        0    52818 2024-05-27 05:48:00.000000 niquests-3.6.6/docs/user/advanced.rst
+-rw-r--r--   0        0        0     6315 2024-05-27 05:48:00.000000 niquests-3.6.6/docs/user/authentication.rst
+-rw-r--r--   0        0        0     1046 2024-05-27 05:48:00.000000 niquests-3.6.6/docs/user/install.rst
+-rw-r--r--   0        0        0    34594 2024-05-27 05:48:00.000000 niquests-3.6.6/docs/user/quickstart.rst
+-rw-r--r--   0        0        0     2805 2024-05-27 05:48:00.000000 niquests-3.6.6/src/niquests/__init__.py
+-rw-r--r--   0        0        0      534 2024-05-27 05:48:00.000000 niquests-3.6.6/src/niquests/__version__.py
+-rw-r--r--   0        0        0    47165 2024-05-27 05:48:00.000000 niquests-3.6.6/src/niquests/_async.py
+-rw-r--r--   0        0        0     2852 2024-05-27 05:48:00.000000 niquests-3.6.6/src/niquests/_compat.py
+-rw-r--r--   0        0        0      480 2024-05-27 05:48:00.000000 niquests-3.6.6/src/niquests/_constant.py
+-rw-r--r--   0        0        0     5942 2024-05-27 05:48:00.000000 niquests-3.6.6/src/niquests/_typing.py
+-rw-r--r--   0        0        0    87323 2024-05-27 05:48:00.000000 niquests-3.6.6/src/niquests/adapters.py
+-rw-r--r--   0        0        0    27567 2024-05-27 05:48:00.000000 niquests-3.6.6/src/niquests/api.py
+-rw-r--r--   0        0        0     9906 2024-05-27 05:48:00.000000 niquests-3.6.6/src/niquests/auth.py
+-rw-r--r--   0        0        0    20648 2024-05-27 05:48:00.000000 niquests-3.6.6/src/niquests/cookies.py
+-rw-r--r--   0        0        0     4363 2024-05-27 05:48:00.000000 niquests-3.6.6/src/niquests/exceptions.py
+-rw-r--r--   0        0        0     5248 2024-05-27 05:48:00.000000 niquests-3.6.6/src/niquests/help.py
+-rw-r--r--   0        0        0     2776 2024-05-27 05:48:00.000000 niquests-3.6.6/src/niquests/hooks.py
+-rw-r--r--   0        0        0    62733 2024-05-27 05:48:00.000000 niquests-3.6.6/src/niquests/models.py
+-rw-r--r--   0        0        0        0 2024-05-27 05:48:00.000000 niquests-3.6.6/src/niquests/py.typed
+-rw-r--r--   0        0        0    69459 2024-05-27 05:48:00.000000 niquests-3.6.6/src/niquests/sessions.py
+-rw-r--r--   0        0        0     4284 2024-05-27 05:48:00.000000 niquests-3.6.6/src/niquests/status_codes.py
+-rw-r--r--   0        0        0     7042 2024-05-27 05:48:00.000000 niquests-3.6.6/src/niquests/structures.py
+-rw-r--r--   0        0        0    37956 2024-05-27 05:48:00.000000 niquests-3.6.6/src/niquests/utils.py
+-rw-r--r--   0        0        0      119 2024-05-27 05:48:00.000000 niquests-3.6.6/src/niquests/extensions/__init__.py
+-rw-r--r--   0        0        0    22400 2024-05-27 05:48:00.000000 niquests-3.6.6/src/niquests/extensions/_async_ocsp.py
+-rw-r--r--   0        0        0    21175 2024-05-27 05:48:00.000000 niquests-3.6.6/src/niquests/extensions/_ocsp.py
+-rw-r--r--   0        0        0    16942 2024-05-27 05:48:00.000000 niquests-3.6.6/src/niquests/extensions/_picotls.py
+-rw-r--r--   0        0        0       80 2024-05-27 05:48:00.000000 niquests-3.6.6/tests/__init__.py
+-rw-r--r--   0        0        0     2619 2024-05-27 05:48:00.000000 niquests-3.6.6/tests/conftest.py
+-rw-r--r--   0        0        0     8095 2024-05-27 05:48:00.000000 niquests-3.6.6/tests/test_async.py
+-rw-r--r--   0        0        0      875 2024-05-27 05:48:00.000000 niquests-3.6.6/tests/test_help.py
+-rw-r--r--   0        0        0      893 2024-05-27 05:48:00.000000 niquests-3.6.6/tests/test_hooks.py
+-rw-r--r--   0        0        0     4537 2024-05-27 05:48:00.000000 niquests-3.6.6/tests/test_live.py
+-rw-r--r--   0        0        0    15985 2024-05-27 05:48:00.000000 niquests-3.6.6/tests/test_lowlevel.py
+-rw-r--r--   0        0        0     3722 2024-05-27 05:48:00.000000 niquests-3.6.6/tests/test_multiplexed.py
+-rw-r--r--   0        0        0   100346 2024-05-27 05:48:00.000000 niquests-3.6.6/tests/test_requests.py
+-rw-r--r--   0        0        0     2725 2024-05-27 05:48:00.000000 niquests-3.6.6/tests/test_structures.py
+-rw-r--r--   0        0        0     6213 2024-05-27 05:48:00.000000 niquests-3.6.6/tests/test_testserver.py
+-rw-r--r--   0        0        0    26728 2024-05-27 05:48:00.000000 niquests-3.6.6/tests/test_utils.py
+-rw-r--r--   0        0        0      613 2024-05-27 05:48:00.000000 niquests-3.6.6/tests/utils.py
+-rw-r--r--   0        0        0        0 2024-05-27 05:48:00.000000 niquests-3.6.6/tests/testserver/__init__.py
+-rw-r--r--   0        0        0     3882 2024-05-27 05:48:00.000000 niquests-3.6.6/tests/testserver/server.py
+-rw-r--r--   0        0        0      362 2024-05-27 05:48:00.000000 niquests-3.6.6/.gitignore
+-rw-r--r--   0        0        0    10142 2024-05-27 05:48:00.000000 niquests-3.6.6/LICENSE
+-rw-r--r--   0        0        0    10885 2024-05-27 05:48:00.000000 niquests-3.6.6/README.md
+-rw-r--r--   0        0        0     3660 2024-05-27 05:48:00.000000 niquests-3.6.6/pyproject.toml
+-rw-r--r--   0        0        0    13244 2024-05-27 05:48:00.000000 niquests-3.6.6/PKG-INFO
```

### Comparing `niquests-3.6.5/AUTHORS.rst` & `niquests-3.6.6/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/HISTORY.md` & `niquests-3.6.6/HISTORY.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Release History
 ===============
 
+3.6.6 (2024-05-27)
+------------------
+
+**Fixed**
+- ReasonFlag not properly translated to readable text when peer or intermediate certificate is revoked.
+
 3.6.5 (2024-05-22)
 ------------------
 
 **Fixed**
 - Support `localhost` as a valid domain for cookies. The standard library does not allow this special
   domain. Researches showed that a valid domain should have at least two dots (e.g. abc.com. and xyz.tld. but not com.).
   Public suffixes cannot be used as a cookie domain for security reasons, but as `localhost` isn't one we are explicitly
```

### Comparing `niquests-3.6.5/docs/Makefile` & `niquests-3.6.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/docs/api.rst` & `niquests-3.6.6/docs/api.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/docs/conf.py` & `niquests-3.6.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/docs/index.rst` & `niquests-3.6.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/docs/make.bat` & `niquests-3.6.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/docs/_static/custom.css` & `niquests-3.6.6/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/docs/_static/requests-sidebar.png` & `niquests-3.6.6/docs/_static/requests-sidebar.png`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/docs/community/faq.rst` & `niquests-3.6.6/docs/community/faq.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/docs/community/recommended.rst` & `niquests-3.6.6/docs/community/recommended.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/docs/community/release-process.rst` & `niquests-3.6.6/docs/community/release-process.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/docs/community/vulnerabilities.rst` & `niquests-3.6.6/docs/community/vulnerabilities.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/docs/dev/contributing.rst` & `niquests-3.6.6/docs/dev/contributing.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/docs/dev/migrate.rst` & `niquests-3.6.6/docs/dev/migrate.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/docs/user/advanced.rst` & `niquests-3.6.6/docs/user/advanced.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/docs/user/authentication.rst` & `niquests-3.6.6/docs/user/authentication.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/docs/user/install.rst` & `niquests-3.6.6/docs/user/install.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/docs/user/quickstart.rst` & `niquests-3.6.6/docs/user/quickstart.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/src/niquests/__init__.py` & `niquests-3.6.6/src/niquests/__init__.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/src/niquests/__version__.py` & `niquests-3.6.6/src/niquests/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 
 __title__: str = "niquests"
 __description__: str = "Python HTTP for Humans."
 __url__: str = "https://niquests.readthedocs.io"
 
 __version__: str
-__version__ = "3.6.5"
+__version__ = "3.6.6"
 
-__build__: int = 0x030605
+__build__: int = 0x030606
 __author__: str = "Kenneth Reitz"
 __author_email__: str = "me@kennethreitz.org"
 __license__: str = "Apache-2.0"
 __copyright__: str = "Copyright Kenneth Reitz"
 __cake__: str = "\u2728 \U0001f370 \u2728"
```

### Comparing `niquests-3.6.5/src/niquests/_async.py` & `niquests-3.6.6/src/niquests/_async.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/src/niquests/_compat.py` & `niquests-3.6.6/src/niquests/_compat.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/src/niquests/_typing.py` & `niquests-3.6.6/src/niquests/_typing.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/src/niquests/adapters.py` & `niquests-3.6.6/src/niquests/adapters.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/src/niquests/api.py` & `niquests-3.6.6/src/niquests/api.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/src/niquests/auth.py` & `niquests-3.6.6/src/niquests/auth.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/src/niquests/cookies.py` & `niquests-3.6.6/src/niquests/cookies.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/src/niquests/exceptions.py` & `niquests-3.6.6/src/niquests/exceptions.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/src/niquests/help.py` & `niquests-3.6.6/src/niquests/help.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/src/niquests/hooks.py` & `niquests-3.6.6/src/niquests/hooks.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/src/niquests/models.py` & `niquests-3.6.6/src/niquests/models.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/src/niquests/sessions.py` & `niquests-3.6.6/src/niquests/sessions.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/src/niquests/status_codes.py` & `niquests-3.6.6/src/niquests/status_codes.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/src/niquests/structures.py` & `niquests-3.6.6/src/niquests/structures.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/src/niquests/utils.py` & `niquests-3.6.6/src/niquests/utils.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/src/niquests/extensions/_async_ocsp.py` & `niquests-3.6.6/src/niquests/extensions/_async_ocsp.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/src/niquests/extensions/_ocsp.py` & `niquests-3.6.6/src/niquests/extensions/_ocsp.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 def _str_fingerprint_of(certificate: Certificate) -> str:
     return ":".join(
         [format(i, "02x") for i in sha256(certificate.public_bytes()).digest()]
     )
 
 
 def readable_revocation_reason(flag: ReasonFlags | None) -> str | None:
-    return flag.name.lower() if flag is not None else None
+    return str(flag).split(".")[-1].lower() if flag is not None else None
 
 
 def _ask_nicely_for_issuer(
     hostname: str, dst_address: tuple[str, int], timeout: int | float = 0.2
 ) -> Certificate | None:
     """When encountering a problem in development, one should always say that there is many solutions.
     From dirtiest to the cleanest, not always known but with progressive effort, we'll eventually land at the cleanest.
```

### Comparing `niquests-3.6.5/src/niquests/extensions/_picotls.py` & `niquests-3.6.6/src/niquests/extensions/_picotls.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/tests/conftest.py` & `niquests-3.6.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/tests/test_async.py` & `niquests-3.6.6/tests/test_async.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import asyncio
 import json
 import os
 
 import pytest
 
 from niquests import AsyncSession, AsyncResponse, Response
-from niquests.exceptions import MultiplexingError
+from niquests.exceptions import MultiplexingError, ConnectionError
 
 
 @pytest.mark.usefixtures("requires_wan")
 @pytest.mark.asyncio
 class TestAsyncWithoutMultiplex:
     async def test_awaitable_get(self):
         async with AsyncSession() as s:
@@ -224,7 +224,18 @@
         any confidence about Happy Eyeballs. This test is valuable in Github CI where IPv6 addresses are unreachable.
         We're using a custom DNS resolver that will yield the IPv6 addresses and IPv4 ones.
         If this hang in CI, then you did something wrong...!"""
         async with AsyncSession(resolver="doh+cloudflare://", happy_eyeballs=True) as s:
             r = await s.get("https://pie.dev/get")
 
             assert r.ok
+
+    @pytest.mark.xfail(reason="Using flaky revoked.badssl.com")
+    async def test_revoked_certificate(self) -> None:
+        """This test may fail at any moment. Using https://revoked.badssl.com/ as a target tester."""
+
+        async with AsyncSession() as s:
+            with pytest.raises(
+                ConnectionError,
+                match="Unable to establish a secure connection to https://revoked.badssl.com/ because the certificate has been revoked",
+            ):
+                await s.get("https://revoked.badssl.com/")
```

### Comparing `niquests-3.6.5/tests/test_help.py` & `niquests-3.6.6/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/tests/test_hooks.py` & `niquests-3.6.6/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/tests/test_live.py` & `niquests-3.6.6/tests/test_live.py`

 * *Files 8% similar despite different names*

```diff
@@ -106,7 +106,18 @@
         any confidence about Happy Eyeballs. This test is valuable in Github CI where IPv6 addresses are unreachable.
         We're using a custom DNS resolver that will yield the IPv6 addresses and IPv4 ones.
         If this hang in CI, then you did something wrong...!"""
         with Session(resolver="doh+cloudflare://", happy_eyeballs=True) as s:
             r = s.get("https://pie.dev/get")
 
             assert r.ok
+
+    @pytest.mark.xfail(reason="Using flaky revoked.badssl.com")
+    def test_revoked_certificate(self) -> None:
+        """This test may fail at any moment. Using https://revoked.badssl.com/ as a target tester."""
+
+        with Session() as s:
+            with pytest.raises(
+                ConnectionError,
+                match="Unable to establish a secure connection to https://revoked.badssl.com/ because the certificate has been revoked",
+            ):
+                s.get("https://revoked.badssl.com/")
```

### Comparing `niquests-3.6.5/tests/test_lowlevel.py` & `niquests-3.6.6/tests/test_lowlevel.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/tests/test_multiplexed.py` & `niquests-3.6.6/tests/test_multiplexed.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/tests/test_requests.py` & `niquests-3.6.6/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/tests/test_structures.py` & `niquests-3.6.6/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/tests/test_testserver.py` & `niquests-3.6.6/tests/test_testserver.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/tests/test_utils.py` & `niquests-3.6.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/tests/utils.py` & `niquests-3.6.6/tests/utils.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/tests/testserver/server.py` & `niquests-3.6.6/tests/testserver/server.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/LICENSE` & `niquests-3.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/README.md` & `niquests-3.6.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         print(payload)  # Output: {'authenticated': True, ...}
 
 asyncio.run(main())
 ```
 
 Niquests allows you to send HTTP requests extremely easily. There’s no need to manually add query strings to your URLs, or to form-encode your `PUT` & `POST` data — just use the `json` method!
 
-[![Downloads](https://static.pepy.tech/badge/niquests/month)](https://pepy.tech/project/niquests)
+[![Downloads](https://img.shields.io/pypi/dm/niquests.svg)](https://pypistats.org/packages/niquests)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/niquests.svg)](https://pypi.org/project/niquests)
 
 This project does not require any compilation toolchain. The HTTP/3 support is not enforced and installed if your platform can support it natively _(e.g. pre-built wheel available)_.
 
 ## ✨ Installing Niquests and Supported Versions
 
 Niquests is available on PyPI:
```

### Comparing `niquests-3.6.5/pyproject.toml` & `niquests-3.6.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `niquests-3.6.5/PKG-INFO` & `niquests-3.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: niquests
-Version: 3.6.5
+Version: 3.6.6
 Summary: Niquests is a simple, yet elegant, HTTP library. It is a drop-in replacement for Requests, which is under feature freeze.
 Project-URL: Changelog, https://github.com/jawah/niquests/blob/main/HISTORY.md
 Project-URL: Documentation, https://niquests.readthedocs.io
 Project-URL: Code, https://github.com/jawah/niquests
 Project-URL: Issue tracker, https://github.com/jawah/niquests/issues
 Author-email: Kenneth Reitz <me@kennethreitz.org>
 Maintainer-email: "Ahmed R. TAHRI" <ahmed.tahri@cloudnursery.dev>
@@ -156,15 +156,15 @@
         print(payload)  # Output: {'authenticated': True, ...}
 
 asyncio.run(main())
 ```
 
 Niquests allows you to send HTTP requests extremely easily. There’s no need to manually add query strings to your URLs, or to form-encode your `PUT` & `POST` data — just use the `json` method!
 
-[![Downloads](https://static.pepy.tech/badge/niquests/month)](https://pepy.tech/project/niquests)
+[![Downloads](https://img.shields.io/pypi/dm/niquests.svg)](https://pypistats.org/packages/niquests)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/niquests.svg)](https://pypi.org/project/niquests)
 
 This project does not require any compilation toolchain. The HTTP/3 support is not enforced and installed if your platform can support it natively _(e.g. pre-built wheel available)_.
 
 ## ✨ Installing Niquests and Supported Versions
 
 Niquests is available on PyPI:
```

