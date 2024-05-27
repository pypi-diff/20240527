# Comparing `tmp/shopcloud_django_toolbox-1.7.1.tar.gz` & `tmp/shopcloud_django_toolbox-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shopcloud_django_toolbox-1.7.1.tar", last modified: Wed Sep 14 09:30:02 2022, max compression
+gzip compressed data, was "shopcloud_django_toolbox-1.8.0.tar", last modified: Fri Sep 16 10:18:18 2022, max compression
```

## Comparing `shopcloud_django_toolbox-1.7.1.tar` & `shopcloud_django_toolbox-1.8.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 seibti     (501) staff       (20)        0 2022-09-14 09:30:02.865201 shopcloud_django_toolbox-1.7.1/
--rw-r--r--   0 seibti     (501) staff       (20)     1072 2022-09-12 09:40:49.000000 shopcloud_django_toolbox-1.7.1/LICENSE
--rw-r--r--   0 seibti     (501) staff       (20)     3628 2022-09-14 09:30:02.863488 shopcloud_django_toolbox-1.7.1/PKG-INFO
--rw-r--r--   0 seibti     (501) staff       (20)     3311 2022-09-14 09:12:24.000000 shopcloud_django_toolbox-1.7.1/README.md
--rw-r--r--   0 seibti     (501) staff       (20)       38 2022-09-14 09:30:02.865435 shopcloud_django_toolbox-1.7.1/setup.cfg
--rw-r--r--   0 seibti     (501) staff       (20)      683 2022-09-14 09:29:15.000000 shopcloud_django_toolbox-1.7.1/setup.py
-drwxr-xr-x   0 seibti     (501) staff       (20)        0 2022-09-14 09:30:02.851884 shopcloud_django_toolbox-1.7.1/shopcloud_django_toolbox/
--rw-r--r--   0 seibti     (501) staff       (20)      128 2022-09-12 12:00:51.000000 shopcloud_django_toolbox-1.7.1/shopcloud_django_toolbox/__init__.py
--rw-r--r--   0 seibti     (501) staff       (20)      695 2022-09-12 09:40:49.000000 shopcloud_django_toolbox-1.7.1/shopcloud_django_toolbox/admin.py
--rw-r--r--   0 seibti     (501) staff       (20)     1817 2022-09-12 09:40:49.000000 shopcloud_django_toolbox-1.7.1/shopcloud_django_toolbox/events.py
--rw-r--r--   0 seibti     (501) staff       (20)     1843 2022-09-12 09:40:49.000000 shopcloud_django_toolbox-1.7.1/shopcloud_django_toolbox/models.py
--rw-r--r--   0 seibti     (501) staff       (20)     1262 2022-09-12 09:40:49.000000 shopcloud_django_toolbox-1.7.1/shopcloud_django_toolbox/renders.py
--rw-r--r--   0 seibti     (501) staff       (20)     3162 2022-09-14 09:29:15.000000 shopcloud_django_toolbox-1.7.1/shopcloud_django_toolbox/signer.py
--rw-r--r--   0 seibti     (501) staff       (20)     4538 2022-09-12 09:40:49.000000 shopcloud_django_toolbox-1.7.1/shopcloud_django_toolbox/tests.py
--rw-r--r--   0 seibti     (501) staff       (20)      479 2022-09-12 09:40:49.000000 shopcloud_django_toolbox-1.7.1/shopcloud_django_toolbox/views.py
-drwxr-xr-x   0 seibti     (501) staff       (20)        0 2022-09-14 09:30:02.862381 shopcloud_django_toolbox-1.7.1/shopcloud_django_toolbox.egg-info/
--rw-r--r--   0 seibti     (501) staff       (20)     3628 2022-09-14 09:30:02.000000 shopcloud_django_toolbox-1.7.1/shopcloud_django_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 seibti     (501) staff       (20)      545 2022-09-14 09:30:02.000000 shopcloud_django_toolbox-1.7.1/shopcloud_django_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 seibti     (501) staff       (20)        1 2022-09-14 09:30:02.000000 shopcloud_django_toolbox-1.7.1/shopcloud_django_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 seibti     (501) staff       (20)       32 2022-09-14 09:30:02.000000 shopcloud_django_toolbox-1.7.1/shopcloud_django_toolbox.egg-info/requires.txt
--rw-r--r--   0 seibti     (501) staff       (20)       25 2022-09-14 09:30:02.000000 shopcloud_django_toolbox-1.7.1/shopcloud_django_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 seibti     (501) staff       (20)        0 2022-09-16 10:18:18.860622 shopcloud_django_toolbox-1.8.0/
+-rw-r--r--   0 seibti     (501) staff       (20)     1072 2022-09-12 09:40:49.000000 shopcloud_django_toolbox-1.8.0/LICENSE
+-rw-r--r--   0 seibti     (501) staff       (20)     4232 2022-09-16 10:18:18.858644 shopcloud_django_toolbox-1.8.0/PKG-INFO
+-rw-r--r--   0 seibti     (501) staff       (20)     3915 2022-09-16 10:17:26.000000 shopcloud_django_toolbox-1.8.0/README.md
+-rw-r--r--   0 seibti     (501) staff       (20)       38 2022-09-16 10:18:18.861051 shopcloud_django_toolbox-1.8.0/setup.cfg
+-rw-r--r--   0 seibti     (501) staff       (20)      683 2022-09-16 10:15:56.000000 shopcloud_django_toolbox-1.8.0/setup.py
+drwxr-xr-x   0 seibti     (501) staff       (20)        0 2022-09-16 10:18:18.844821 shopcloud_django_toolbox-1.8.0/shopcloud_django_toolbox/
+-rw-r--r--   0 seibti     (501) staff       (20)      154 2022-09-16 10:15:56.000000 shopcloud_django_toolbox-1.8.0/shopcloud_django_toolbox/__init__.py
+-rw-r--r--   0 seibti     (501) staff       (20)      695 2022-09-12 09:40:49.000000 shopcloud_django_toolbox-1.8.0/shopcloud_django_toolbox/admin.py
+-rw-r--r--   0 seibti     (501) staff       (20)      935 2022-09-16 10:15:56.000000 shopcloud_django_toolbox-1.8.0/shopcloud_django_toolbox/decorators.py
+-rw-r--r--   0 seibti     (501) staff       (20)     1817 2022-09-12 09:40:49.000000 shopcloud_django_toolbox-1.8.0/shopcloud_django_toolbox/events.py
+-rw-r--r--   0 seibti     (501) staff       (20)     1843 2022-09-12 09:40:49.000000 shopcloud_django_toolbox-1.8.0/shopcloud_django_toolbox/models.py
+-rw-r--r--   0 seibti     (501) staff       (20)     1262 2022-09-12 09:40:49.000000 shopcloud_django_toolbox-1.8.0/shopcloud_django_toolbox/renders.py
+-rw-r--r--   0 seibti     (501) staff       (20)     3162 2022-09-14 09:29:15.000000 shopcloud_django_toolbox-1.8.0/shopcloud_django_toolbox/signer.py
+-rw-r--r--   0 seibti     (501) staff       (20)     4538 2022-09-12 09:40:49.000000 shopcloud_django_toolbox-1.8.0/shopcloud_django_toolbox/tests.py
+-rw-r--r--   0 seibti     (501) staff       (20)      479 2022-09-12 09:40:49.000000 shopcloud_django_toolbox-1.8.0/shopcloud_django_toolbox/views.py
+drwxr-xr-x   0 seibti     (501) staff       (20)        0 2022-09-16 10:18:18.854901 shopcloud_django_toolbox-1.8.0/shopcloud_django_toolbox.egg-info/
+-rw-r--r--   0 seibti     (501) staff       (20)     4232 2022-09-16 10:18:18.000000 shopcloud_django_toolbox-1.8.0/shopcloud_django_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 seibti     (501) staff       (20)      584 2022-09-16 10:18:18.000000 shopcloud_django_toolbox-1.8.0/shopcloud_django_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 seibti     (501) staff       (20)        1 2022-09-16 10:18:18.000000 shopcloud_django_toolbox-1.8.0/shopcloud_django_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 seibti     (501) staff       (20)       32 2022-09-16 10:18:18.000000 shopcloud_django_toolbox-1.8.0/shopcloud_django_toolbox.egg-info/requires.txt
+-rw-r--r--   0 seibti     (501) staff       (20)       25 2022-09-16 10:18:18.000000 shopcloud_django_toolbox-1.8.0/shopcloud_django_toolbox.egg-info/top_level.txt
```

### Comparing `shopcloud_django_toolbox-1.7.1/LICENSE` & `shopcloud_django_toolbox-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shopcloud_django_toolbox-1.7.1/PKG-INFO` & `shopcloud_django_toolbox-1.8.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: shopcloud_django_toolbox
-Version: 1.7.1
-Summary: Django tool
-Home-page: https://github.com/Talk-Point/shopcloud-django-toolbox
-Author: Konstantin Stoldt
-Author-email: konstantin.stoldt@talk-point.de
-License: MIT
-Keywords: CLI
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # shopcloud-django-toolbox
 
 ## install
 
 ```sh
 $ pip install shopcloud-django-toolbox
 ```
@@ -27,15 +15,15 @@
 
 class FooBarModel(models.Model, GID):
     pass
 ```
 
 ## URL-Signing
 
-generate or load encrypted data versioned and with expiration date for access-control
+generate or load signed base64  encoded dict containing versioned with expiration date for access-control
 
 ### Usage
 
 `settings.py`
 ```python3
 DJ_TOOLBOX_SIGNER = {
     'VERSION': "1",
@@ -50,38 +38,61 @@
 
 ```
 
 __load values dict:__
 
 ```python3
 from shopcloud django.toolbox import signer
+from django.http import HttpResponseForbidden
 
-
-def get_request(request):
+def some_view(request):
     sign_str = request.GET.get("sign")
     is_valid, data = signer.loads(sign_str)
     if not is_valid(request):
         return HttpResponseForbidden("Not allowed")
     data.get("xxx")
-    ...
+    #
+    ## … some view logic
+    #
 ```
 
 __alternative for a django Request:__
+
 ```python3
 from shopcloud django.toolbox import signer
+from django.http import HttpResponseForbidden
 
-def get_request(request):
-    is_valid, data = signer.loads_from_request(signing_str)
+def some_view(request):
+    sign_str = request.GET.get("sign")
+    is_valid, data = signer.loads_from_request(sign_str)
     if not is_valid(request):
             return HttpResponseForbidden("Not allowed")
     data.get("xxx")
-    ...
+    #
+    ## … some view logic
+    #
+```
+
+__Django View Decorator__
+
+check if GET-parameter `sign` is set and has required keys in data objects
+
 ```
+from shopcloud_django_toolbox import signer
+from shopcloud_django_toolbox.decorators import 
 
 
+@require_toolbox_sign(needed_keys=['key_that_must_exist', 'foo', 'bar'])
+def some_view(request):
+    is_valid, data = signer.loads_from_request(request)
+    #
+    ## … some view logic
+    #
+```
+
 
 ## Testing
 
 ### API standart tests
 
 Standart template for the `tests.py` file in all modules with admin and REST API`s
```

### Comparing `shopcloud_django_toolbox-1.7.1/setup.py` & `shopcloud_django_toolbox-1.8.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='shopcloud_django_toolbox',
-    version='1.7.1',
+    version='1.8.0',
     description='Django tool',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
     author='Konstantin Stoldt',
     author_email='konstantin.stoldt@talk-point.de',
```

### Comparing `shopcloud_django_toolbox-1.7.1/shopcloud_django_toolbox/admin.py` & `shopcloud_django_toolbox-1.8.0/shopcloud_django_toolbox/admin.py`

 * *Files identical despite different names*

### Comparing `shopcloud_django_toolbox-1.7.1/shopcloud_django_toolbox/events.py` & `shopcloud_django_toolbox-1.8.0/shopcloud_django_toolbox/events.py`

 * *Files identical despite different names*

### Comparing `shopcloud_django_toolbox-1.7.1/shopcloud_django_toolbox/models.py` & `shopcloud_django_toolbox-1.8.0/shopcloud_django_toolbox/models.py`

 * *Files identical despite different names*

### Comparing `shopcloud_django_toolbox-1.7.1/shopcloud_django_toolbox/renders.py` & `shopcloud_django_toolbox-1.8.0/shopcloud_django_toolbox/renders.py`

 * *Files identical despite different names*

### Comparing `shopcloud_django_toolbox-1.7.1/shopcloud_django_toolbox/signer.py` & `shopcloud_django_toolbox-1.8.0/shopcloud_django_toolbox/signer.py`

 * *Files identical despite different names*

### Comparing `shopcloud_django_toolbox-1.7.1/shopcloud_django_toolbox/tests.py` & `shopcloud_django_toolbox-1.8.0/shopcloud_django_toolbox/tests.py`

 * *Files identical despite different names*

### Comparing `shopcloud_django_toolbox-1.7.1/shopcloud_django_toolbox.egg-info/PKG-INFO` & `shopcloud_django_toolbox-1.8.0/shopcloud_django_toolbox.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shopcloud-django-toolbox
-Version: 1.7.1
+Version: 1.8.0
 Summary: Django tool
 Home-page: https://github.com/Talk-Point/shopcloud-django-toolbox
 Author: Konstantin Stoldt
 Author-email: konstantin.stoldt@talk-point.de
 License: MIT
 Keywords: CLI
 Description-Content-Type: text/markdown
@@ -27,15 +27,15 @@
 
 class FooBarModel(models.Model, GID):
     pass
 ```
 
 ## URL-Signing
 
-generate or load encrypted data versioned and with expiration date for access-control
+generate or load signed base64  encoded dict containing versioned with expiration date for access-control
 
 ### Usage
 
 `settings.py`
 ```python3
 DJ_TOOLBOX_SIGNER = {
     'VERSION': "1",
@@ -50,37 +50,60 @@
 
 ```
 
 __load values dict:__
 
 ```python3
 from shopcloud django.toolbox import signer
+from django.http import HttpResponseForbidden
 
-
-def get_request(request):
+def some_view(request):
     sign_str = request.GET.get("sign")
     is_valid, data = signer.loads(sign_str)
     if not is_valid(request):
         return HttpResponseForbidden("Not allowed")
     data.get("xxx")
-    ...
+    #
+    ## … some view logic
+    #
 ```
 
 __alternative for a django Request:__
+
 ```python3
 from shopcloud django.toolbox import signer
+from django.http import HttpResponseForbidden
 
-def get_request(request):
-    is_valid, data = signer.loads_from_request(signing_str)
+def some_view(request):
+    sign_str = request.GET.get("sign")
+    is_valid, data = signer.loads_from_request(sign_str)
     if not is_valid(request):
             return HttpResponseForbidden("Not allowed")
     data.get("xxx")
-    ...
+    #
+    ## … some view logic
+    #
 ```
 
+__Django View Decorator__
+
+check if GET-parameter `sign` is set and has required keys in data objects
+
+```
+from shopcloud_django_toolbox import signer
+from shopcloud_django_toolbox.decorators import 
+
+
+@require_toolbox_sign(needed_keys=['key_that_must_exist', 'foo', 'bar'])
+def some_view(request):
+    is_valid, data = signer.loads_from_request(request)
+    #
+    ## … some view logic
+    #
+```
 
 
 ## Testing
 
 ### API standart tests
 
 Standart template for the `tests.py` file in all modules with admin and REST API`s
```

### Comparing `shopcloud_django_toolbox-1.7.1/shopcloud_django_toolbox.egg-info/SOURCES.txt` & `shopcloud_django_toolbox-1.8.0/shopcloud_django_toolbox.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 shopcloud_django_toolbox/__init__.py
 shopcloud_django_toolbox/admin.py
+shopcloud_django_toolbox/decorators.py
 shopcloud_django_toolbox/events.py
 shopcloud_django_toolbox/models.py
 shopcloud_django_toolbox/renders.py
 shopcloud_django_toolbox/signer.py
 shopcloud_django_toolbox/tests.py
 shopcloud_django_toolbox/views.py
 shopcloud_django_toolbox.egg-info/PKG-INFO
```

