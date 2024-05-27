# Comparing `tmp/django_email_hosts-0.2.0.tar.gz` & `tmp/django_email_hosts-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_email_hosts-0.2.0.tar", last modified: Mon Feb  7 13:42:07 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `django_email_hosts-0.2.0.tar` & `django_email_hosts-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,25 @@
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-02-07 13:42:07.348964 django_email_hosts-0.2.0/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1553 2022-02-07 13:24:33.000000 django_email_hosts-0.2.0/LICENSE
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      175 2022-02-07 13:24:33.000000 django_email_hosts-0.2.0/MANIFEST.in
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     3240 2022-02-07 13:42:07.348964 django_email_hosts-0.2.0/PKG-INFO
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2541 2022-02-07 13:30:38.000000 django_email_hosts-0.2.0/README.rst
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-02-07 13:42:07.348964 django_email_hosts-0.2.0/django_email_hosts.egg-info/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     3240 2022-02-07 13:42:07.000000 django_email_hosts-0.2.0/django_email_hosts.egg-info/PKG-INFO
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      347 2022-02-07 13:42:07.000000 django_email_hosts-0.2.0/django_email_hosts.egg-info/SOURCES.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2022-02-07 13:42:07.000000 django_email_hosts-0.2.0/django_email_hosts.egg-info/dependency_links.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2022-02-07 13:27:25.000000 django_email_hosts-0.2.0/django_email_hosts.egg-info/not-zip-safe
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       44 2022-02-07 13:42:07.000000 django_email_hosts-0.2.0/django_email_hosts.egg-info/requires.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       12 2022-02-07 13:42:07.000000 django_email_hosts-0.2.0/django_email_hosts.egg-info/top_level.txt
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-02-07 13:42:07.348964 django_email_hosts-0.2.0/email_hosts/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       62 2022-02-07 13:41:51.000000 django_email_hosts-0.2.0/email_hosts/__init__.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1248 2022-02-07 13:28:03.000000 django_email_hosts-0.2.0/email_hosts/backends.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1028 2022-02-07 13:42:07.348964 django_email_hosts-0.2.0/setup.cfg
--rwxrwxr-x   0 matthias  (1000) matthias  (1000)       62 2022-02-07 13:24:33.000000 django_email_hosts-0.2.0/setup.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/.editorconfig
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/CHANGELOG.rst
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/tox.ini
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/docs/Makefile
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/docs/conf.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/docs/index.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/docs/make.bat
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/email_hosts/__init__.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/email_hosts/backends.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/email_hosts/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/email_hosts/management/commands/__init__.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/email_hosts/management/commands/sendtestemailhosts.py
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/tests/manage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/tests/testapp/__init__.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/tests/testapp/settings.py
+-rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/tests/testapp/test_email_hosts.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/tests/testapp/urls.py
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/tests/testapp/views.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/README.rst
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 django_email_hosts-0.2.1/PKG-INFO
```

### Comparing `django_email_hosts-0.2.0/LICENSE` & `django_email_hosts-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_email_hosts-0.2.0/PKG-INFO` & `django_email_hosts-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,32 @@
-Metadata-Version: 2.1
-Name: django_email_hosts
-Version: 0.2.0
+Metadata-Version: 2.3
+Name: django-email-hosts
+Version: 0.2.1
 Summary: Support for several SMTP configurations in a single site
-Home-page: https://github.com/feinheit/django-email-hosts/
-Author: Feinheit AG
-Author-email: dev@feinheit.ch
+Project-URL: Homepage, https://github.com/feinheit/django-email-hosts/
+Author-email: Feinheit AG <dev@feinheit.ch>
 License: BSD-3-Clause
-Platform: OS Independent
+License-File: LICENSE
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
+Requires-Dist: django>=3.2
+Requires-Dist: speckenv>=3.2
 Provides-Extra: tests
-License-File: LICENSE
+Requires-Dist: coverage; extra == 'tests'
+Description-Content-Type: text/x-rst
 
 ==============================================================================
 django-email-hosts -- Support for several SMTP configurations in a single site
 ==============================================================================
 
 .. image:: https://github.com/feinheit/django-email-hosts/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/feinheit/django-email-hosts/
@@ -83,14 +88,12 @@
     from django.core.mail import EmailMessage
     from email_hosts.backends import get_connection
 
     EmailMessage(
         "Hello",
         "World",
         to=["recipient@example.com"],
-        connection=use_backend("sendgrid"),
+        connection=get_connection("sendgrid"),
     ).send()
 
 ``get_connection`` currently silently returns the default email backend if the
 key doesn't exist in the ``EMAIL_HOSTS`` dictionary.
-
-
```

### Comparing `django_email_hosts-0.2.0/README.rst` & `django_email_hosts-0.2.1/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -62,12 +62,12 @@
     from django.core.mail import EmailMessage
     from email_hosts.backends import get_connection
 
     EmailMessage(
         "Hello",
         "World",
         to=["recipient@example.com"],
-        connection=use_backend("sendgrid"),
+        connection=get_connection("sendgrid"),
     ).send()
 
 ``get_connection`` currently silently returns the default email backend if the
 key doesn't exist in the ``EMAIL_HOSTS`` dictionary.
```

### Comparing `django_email_hosts-0.2.0/email_hosts/backends.py` & `django_email_hosts-0.2.1/email_hosts/backends.py`

 * *Files identical despite different names*

