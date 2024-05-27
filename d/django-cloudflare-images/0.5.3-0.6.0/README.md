# Comparing `tmp/django-cloudflare-images-0.5.3.tar.gz` & `tmp/django_cloudflare_images-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cloudflare-images-0.5.3.tar", last modified: Wed Dec  6 05:29:18 2023, max compression
+gzip compressed data, was "django_cloudflare_images-0.6.0.tar", last modified: Mon May 27 06:15:37 2024, max compression
```

## Comparing `django-cloudflare-images-0.5.3.tar` & `django_cloudflare_images-0.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-12-06 05:29:18.197336 django-cloudflare-images-0.5.3/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1093 2022-03-21 07:51:01.000000 django-cloudflare-images-0.5.3/LICENSE
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2452 2023-12-06 05:29:18.197336 django-cloudflare-images-0.5.3/PKG-INFO
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1823 2023-12-06 05:08:37.000000 django-cloudflare-images-0.5.3/README.md
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-12-06 05:29:18.194003 django-cloudflare-images-0.5.3/cloudflare_images/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2022-03-20 12:51:13.000000 django-cloudflare-images-0.5.3/cloudflare_images/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1228 2022-07-05 09:09:39.000000 django-cloudflare-images-0.5.3/cloudflare_images/config.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1649 2022-07-05 09:09:39.000000 django-cloudflare-images-0.5.3/cloudflare_images/field.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2452 2023-02-22 05:42:20.000000 django-cloudflare-images-0.5.3/cloudflare_images/service.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4350 2023-02-22 05:42:20.000000 django-cloudflare-images-0.5.3/cloudflare_images/storage.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-12-06 05:29:18.197336 django-cloudflare-images-0.5.3/django_cloudflare_images.egg-info/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2452 2023-12-06 05:29:18.000000 django-cloudflare-images-0.5.3/django_cloudflare_images.egg-info/PKG-INFO
--rw-r--r--   0 pierre    (1000) pierre    (1000)      509 2023-12-06 05:29:18.000000 django-cloudflare-images-0.5.3/django_cloudflare_images.egg-info/SOURCES.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2023-12-06 05:29:18.000000 django-cloudflare-images-0.5.3/django_cloudflare_images.egg-info/dependency_links.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)       74 2023-12-06 05:29:18.000000 django-cloudflare-images-0.5.3/django_cloudflare_images.egg-info/requires.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)       18 2023-12-06 05:29:18.000000 django-cloudflare-images-0.5.3/django_cloudflare_images.egg-info/top_level.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)       81 2023-02-27 06:09:33.000000 django-cloudflare-images-0.5.3/pyproject.toml
--rw-r--r--   0 pierre    (1000) pierre    (1000)      629 2023-12-06 05:29:18.200670 django-cloudflare-images-0.5.3/setup.cfg
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-12-06 05:29:18.197336 django-cloudflare-images-0.5.3/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1217 2022-07-05 09:09:39.000000 django-cloudflare-images-0.5.3/tests/test_config.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2651 2022-07-05 09:09:39.000000 django-cloudflare-images-0.5.3/tests/test_field.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3333 2023-02-22 05:42:20.000000 django-cloudflare-images-0.5.3/tests/test_service.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3798 2023-02-22 05:42:20.000000 django-cloudflare-images-0.5.3/tests/test_storage.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-05-27 06:15:37.038344 django_cloudflare_images-0.6.0/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1093 2022-03-21 07:51:01.000000 django_cloudflare_images-0.6.0/LICENSE
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2686 2024-05-27 06:15:37.038344 django_cloudflare_images-0.6.0/PKG-INFO
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2060 2024-05-27 06:06:39.000000 django_cloudflare_images-0.6.0/README.md
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-05-27 06:15:37.035011 django_cloudflare_images-0.6.0/cloudflare_images/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2022-03-20 12:51:13.000000 django_cloudflare_images-0.6.0/cloudflare_images/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1523 2024-05-27 06:06:39.000000 django_cloudflare_images-0.6.0/cloudflare_images/config.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1649 2022-07-05 09:09:39.000000 django_cloudflare_images-0.6.0/cloudflare_images/field.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2595 2024-05-27 06:10:42.000000 django_cloudflare_images-0.6.0/cloudflare_images/service.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4350 2023-02-22 05:42:20.000000 django_cloudflare_images-0.6.0/cloudflare_images/storage.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-05-27 06:15:37.038344 django_cloudflare_images-0.6.0/django_cloudflare_images.egg-info/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2686 2024-05-27 06:15:37.000000 django_cloudflare_images-0.6.0/django_cloudflare_images.egg-info/PKG-INFO
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      509 2024-05-27 06:15:37.000000 django_cloudflare_images-0.6.0/django_cloudflare_images.egg-info/SOURCES.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2024-05-27 06:15:37.000000 django_cloudflare_images-0.6.0/django_cloudflare_images.egg-info/dependency_links.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       71 2024-05-27 06:15:37.000000 django_cloudflare_images-0.6.0/django_cloudflare_images.egg-info/requires.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       18 2024-05-27 06:15:37.000000 django_cloudflare_images-0.6.0/django_cloudflare_images.egg-info/top_level.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       81 2023-02-27 06:09:33.000000 django_cloudflare_images-0.6.0/pyproject.toml
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      626 2024-05-27 06:15:37.038344 django_cloudflare_images-0.6.0/setup.cfg
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-05-27 06:15:37.038344 django_cloudflare_images-0.6.0/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1525 2024-05-27 06:06:39.000000 django_cloudflare_images-0.6.0/tests/test_config.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2651 2022-07-05 09:09:39.000000 django_cloudflare_images-0.6.0/tests/test_field.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3333 2023-02-22 05:42:20.000000 django_cloudflare_images-0.6.0/tests/test_service.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3799 2024-03-04 04:33:51.000000 django_cloudflare_images-0.6.0/tests/test_storage.py
```

### Comparing `django-cloudflare-images-0.5.3/LICENSE` & `django_cloudflare_images-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cloudflare-images-0.5.3/PKG-INFO` & `django_cloudflare_images-0.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: django-cloudflare-images
-Version: 0.5.3
+Version: 0.6.0
 Summary: Cloudflare Images integration for Django
 Home-page: https://github.com/KalvadTech/django-cloudflare-images/
 Author: Pierre Guillemot
 Author-email: pierre@kalvad.com
 License: MIT
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=3
 Requires-Dist: requests>=2.20.0
 Provides-Extra: dev
-Requires-Dist: black==23.11.0; extra == "dev"
-Requires-Dist: build==1.0.3; extra == "dev"
-Requires-Dist: tox==4.11.4; extra == "dev"
+Requires-Dist: build==1.2.1; extra == "dev"
+Requires-Dist: ruff==0.4.5; extra == "dev"
+Requires-Dist: tox==4.15.0; extra == "dev"
 
 # django-cloudflare-images
 
 This is a Django library to add support to Cloudflare Images to the ImageField.
 
 It supports:
 
@@ -74,23 +74,27 @@
 
 Please note that you will need to migrate your model(s) once you swapped the field(s). No SQL will actually be applied (you can check by running `sqlmigrate <module> <number>`).
 
 If you wish to use a custom domain to serve your images you need to add the following to your settings.py:
 
 ```python
 CLOUDFLARE_IMAGES_DOMAIN = "example.com"
-
 ```
 
 If you wish to use a default variant other than "public" to serve your images you need to add the following to your settings.py:
 
 ```python
 CLOUDFLARE_IMAGES_VARIANT = "custom"
 ```
 
+If you wish to override the default timeout of 60 seconds for API requests, you need to add the following to your settings.py:
+
+```python
+CLOUDFLARE_IMAGES_API_TIMEOUT = 120
+```
 ## Development
 
 Installing for development:
 
 ```sh
 make install
 ```
@@ -103,14 +107,20 @@
 
 Format the code:
 
 ```sh
 make format
 ```
 
+Check the code (for linting errors):
+
+```sh
+make check
+```
+
 Running all tests:
 
 ```sh
 make test
 ```
 
 Create a sdist+bdist package in dist/:
```

### Comparing `django-cloudflare-images-0.5.3/README.md` & `django_cloudflare_images-0.6.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -54,23 +54,27 @@
 
 Please note that you will need to migrate your model(s) once you swapped the field(s). No SQL will actually be applied (you can check by running `sqlmigrate <module> <number>`).
 
 If you wish to use a custom domain to serve your images you need to add the following to your settings.py:
 
 ```python
 CLOUDFLARE_IMAGES_DOMAIN = "example.com"
-
 ```
 
 If you wish to use a default variant other than "public" to serve your images you need to add the following to your settings.py:
 
 ```python
 CLOUDFLARE_IMAGES_VARIANT = "custom"
 ```
 
+If you wish to override the default timeout of 60 seconds for API requests, you need to add the following to your settings.py:
+
+```python
+CLOUDFLARE_IMAGES_API_TIMEOUT = 120
+```
 ## Development
 
 Installing for development:
 
 ```sh
 make install
 ```
@@ -83,14 +87,20 @@
 
 Format the code:
 
 ```sh
 make format
 ```
 
+Check the code (for linting errors):
+
+```sh
+make check
+```
+
 Running all tests:
 
 ```sh
 make test
 ```
 
 Create a sdist+bdist package in dist/:
```

### Comparing `django-cloudflare-images-0.5.3/cloudflare_images/config.py` & `django_cloudflare_images-0.6.0/cloudflare_images/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -48,7 +48,18 @@
         Returns the default variant
         """
         return (
             settings.CLOUDFLARE_IMAGES_VARIANT
             if hasattr(settings, "CLOUDFLARE_IMAGES_VARIANT")
             else "public"
         )
+
+    @property
+    def api_timeout(self):
+        """
+        Returns the timeout if set, else a default of 60 seconds
+        """
+        return (
+            settings.CLOUDFLARE_IMAGES_API_TIMEOUT
+            if hasattr(settings, "CLOUDFLARE_IMAGES_API_TIMEOUT")
+            else 60
+        )
```

### Comparing `django-cloudflare-images-0.5.3/cloudflare_images/field.py` & `django_cloudflare_images-0.6.0/cloudflare_images/field.py`

 * *Files identical despite different names*

### Comparing `django-cloudflare-images-0.5.3/cloudflare_images/service.py` & `django_cloudflare_images-0.6.0/cloudflare_images/service.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,15 +33,17 @@
             self.config.account_id
         )
 
         headers = {"Authorization": "Bearer {}".format(self.config.api_token)}
 
         files = {"file": file}
 
-        response = requests.post(url, headers=headers, files=files)
+        response = requests.post(
+            url, headers=headers, timeout=self.config.api_timeout, files=files
+        )
 
         status_code = response.status_code
         if status_code != 200:
             raise ApiException(response.content)
 
         response_body = response.json()
         return response_body.get("result").get("id")
@@ -62,15 +64,15 @@
     def open(self, name, variant=None):
         """
         Retrieves a file and return its content, otherwise raise an exception
         """
 
         url = self.get_url(name, variant or self.config.variant)
 
-        response = requests.get(url)
+        response = requests.get(url, timeout=self.config.api_timeout)
 
         status_code = response.status_code
         if status_code != 200:
             raise ApiException(response.content)
 
         return response.content
 
@@ -81,12 +83,14 @@
 
         url = "https://api.cloudflare.com/client/v4/accounts/{}/images/v1/{}".format(
             self.config.account_id, name
         )
 
         headers = {"Authorization": "Bearer {}".format(self.config.api_token)}
 
-        response = requests.delete(url, headers=headers)
+        response = requests.delete(
+            url, timeout=self.config.api_timeout, headers=headers
+        )
 
         status_code = response.status_code
         if status_code != 200:
             raise ApiException(str(response.text))
```

### Comparing `django-cloudflare-images-0.5.3/cloudflare_images/storage.py` & `django_cloudflare_images-0.6.0/cloudflare_images/storage.py`

 * *Files identical despite different names*

### Comparing `django-cloudflare-images-0.5.3/django_cloudflare_images.egg-info/PKG-INFO` & `django_cloudflare_images-0.6.0/django_cloudflare_images.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: django-cloudflare-images
-Version: 0.5.3
+Version: 0.6.0
 Summary: Cloudflare Images integration for Django
 Home-page: https://github.com/KalvadTech/django-cloudflare-images/
 Author: Pierre Guillemot
 Author-email: pierre@kalvad.com
 License: MIT
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=3
 Requires-Dist: requests>=2.20.0
 Provides-Extra: dev
-Requires-Dist: black==23.11.0; extra == "dev"
-Requires-Dist: build==1.0.3; extra == "dev"
-Requires-Dist: tox==4.11.4; extra == "dev"
+Requires-Dist: build==1.2.1; extra == "dev"
+Requires-Dist: ruff==0.4.5; extra == "dev"
+Requires-Dist: tox==4.15.0; extra == "dev"
 
 # django-cloudflare-images
 
 This is a Django library to add support to Cloudflare Images to the ImageField.
 
 It supports:
 
@@ -74,23 +74,27 @@
 
 Please note that you will need to migrate your model(s) once you swapped the field(s). No SQL will actually be applied (you can check by running `sqlmigrate <module> <number>`).
 
 If you wish to use a custom domain to serve your images you need to add the following to your settings.py:
 
 ```python
 CLOUDFLARE_IMAGES_DOMAIN = "example.com"
-
 ```
 
 If you wish to use a default variant other than "public" to serve your images you need to add the following to your settings.py:
 
 ```python
 CLOUDFLARE_IMAGES_VARIANT = "custom"
 ```
 
+If you wish to override the default timeout of 60 seconds for API requests, you need to add the following to your settings.py:
+
+```python
+CLOUDFLARE_IMAGES_API_TIMEOUT = 120
+```
 ## Development
 
 Installing for development:
 
 ```sh
 make install
 ```
@@ -103,14 +107,20 @@
 
 Format the code:
 
 ```sh
 make format
 ```
 
+Check the code (for linting errors):
+
+```sh
+make check
+```
+
 Running all tests:
 
 ```sh
 make test
 ```
 
 Create a sdist+bdist package in dist/:
```

### Comparing `django-cloudflare-images-0.5.3/setup.cfg` & `django_cloudflare_images-0.6.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-cloudflare-images
-version = 0.5.3
+version = 0.6.0
 description = Cloudflare Images integration for Django
 long_description_content_type = text/markdown
 long_description = file: README.md
 author = Pierre Guillemot
 author_email = pierre@kalvad.com
 url = https://github.com/KalvadTech/django-cloudflare-images/
 license = MIT
@@ -17,15 +17,15 @@
 python_requires = >=3
 install_requires = 
 	Django>=3
 	requests>=2.20.0
 
 [options.extras_require]
 dev = 
-	black==23.11.0
-	build==1.0.3
-	tox==4.11.4
+	build==1.2.1
+	ruff==0.4.5
+	tox==4.15.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `django-cloudflare-images-0.5.3/tests/test_config.py` & `django_cloudflare_images-0.6.0/tests/test_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,7 +39,16 @@
         variant = self.config.variant
         self.assertEqual(variant, "public")
 
     @override_settings(CLOUDFLARE_IMAGES_VARIANT="custom")
     def test_custom_variant(self):
         variant = self.config.variant
         self.assertEqual(variant, "custom")
+
+    def test_api_timeout(self):
+        api_timeout = self.config.api_timeout
+        self.assertEqual(api_timeout, 60)
+
+    @override_settings(CLOUDFLARE_IMAGES_API_TIMEOUT=100)
+    def test_custom_api_timeout(self):
+        api_timeout = self.config.api_timeout
+        self.assertEqual(api_timeout, 100)
```

### Comparing `django-cloudflare-images-0.5.3/tests/test_field.py` & `django_cloudflare_images-0.6.0/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `django-cloudflare-images-0.5.3/tests/test_service.py` & `django_cloudflare_images-0.6.0/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `django-cloudflare-images-0.5.3/tests/test_storage.py` & `django_cloudflare_images-0.6.0/tests/test_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Test related to the CloudflareImagesStorage
 """
+
 from unittest.mock import patch
 from django.test import TestCase, override_settings
 from cloudflare_images.storage import CloudflareImagesStorage
 from cloudflare_images.service import ApiException
 from .utils import get_dummy_image, get_dummy_image_name
```

