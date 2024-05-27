# Comparing `tmp/drf-rw-serializers-1.1.1.tar.gz` & `tmp/drf_rw_serializers-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-rw-serializers-1.1.1.tar", last modified: Wed Feb  7 21:08:05 2024, max compression
+gzip compressed data, was "drf_rw_serializers-1.2.0.tar", max compression
```

## Comparing `drf-rw-serializers-1.1.1.tar` & `drf_rw_serializers-1.2.0.tar`

### file list

```diff
@@ -1,27 +1,10 @@
-drwxrwxr-x   0 fjsj      (1000) fjsj      (1000)        0 2024-02-07 21:08:05.527481 drf-rw-serializers-1.1.1/
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)      198 2023-12-22 18:55:00.000000 drf-rw-serializers-1.1.1/AUTHORS.rst
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)     1790 2024-02-07 19:54:36.000000 drf-rw-serializers-1.1.1/CHANGELOG.rst
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)        0 2023-12-22 18:55:00.000000 drf-rw-serializers-1.1.1/CONTRIBUTING.rst
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)     1104 2023-12-22 18:55:00.000000 drf-rw-serializers-1.1.1/LICENSE.txt
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)      188 2023-12-22 18:55:00.000000 drf-rw-serializers-1.1.1/MANIFEST.in
--rw-r--r--   0 fjsj      (1000) fjsj      (1000)     6293 2024-02-07 21:08:05.527481 drf-rw-serializers-1.1.1/PKG-INFO
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)     3168 2023-12-22 18:55:00.000000 drf-rw-serializers-1.1.1/README.rst
-drwxrwxr-x   0 fjsj      (1000) fjsj      (1000)        0 2024-02-07 21:08:05.523481 drf-rw-serializers-1.1.1/drf_rw_serializers/
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)      359 2024-02-07 19:54:36.000000 drf-rw-serializers-1.1.1/drf_rw_serializers/__init__.py
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)      336 2023-12-22 18:55:00.000000 drf-rw-serializers-1.1.1/drf_rw_serializers/apps.py
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)     5267 2023-12-22 18:55:00.000000 drf-rw-serializers-1.1.1/drf_rw_serializers/generics.py
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)     2210 2023-12-22 18:55:00.000000 drf-rw-serializers-1.1.1/drf_rw_serializers/mixins.py
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)      678 2023-12-22 18:55:00.000000 drf-rw-serializers-1.1.1/drf_rw_serializers/viewsets.py
-drwxrwxr-x   0 fjsj      (1000) fjsj      (1000)        0 2024-02-07 21:08:05.527481 drf-rw-serializers-1.1.1/drf_rw_serializers.egg-info/
--rw-r--r--   0 fjsj      (1000) fjsj      (1000)     6293 2024-02-07 21:08:05.000000 drf-rw-serializers-1.1.1/drf_rw_serializers.egg-info/PKG-INFO
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)      562 2024-02-07 21:08:05.000000 drf-rw-serializers-1.1.1/drf_rw_serializers.egg-info/SOURCES.txt
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)        1 2024-02-07 21:08:05.000000 drf-rw-serializers-1.1.1/drf_rw_serializers.egg-info/dependency_links.txt
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)        1 2024-02-07 21:07:03.000000 drf-rw-serializers-1.1.1/drf_rw_serializers.egg-info/not-zip-safe
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)       16 2024-02-07 21:08:05.000000 drf-rw-serializers-1.1.1/drf_rw_serializers.egg-info/requires.txt
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)       19 2024-02-07 21:08:05.000000 drf-rw-serializers-1.1.1/drf_rw_serializers.egg-info/top_level.txt
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)      255 2024-02-07 21:08:05.527481 drf-rw-serializers-1.1.1/setup.cfg
--rwxrwxr-x   0 fjsj      (1000) fjsj      (1000)     2587 2024-02-07 19:54:36.000000 drf-rw-serializers-1.1.1/setup.py
-drwxrwxr-x   0 fjsj      (1000) fjsj      (1000)        0 2024-02-07 21:08:05.523481 drf-rw-serializers-1.1.1/tests/
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)     4376 2023-12-22 18:55:00.000000 drf-rw-serializers-1.1.1/tests/test_generics.py
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)     2414 2023-12-22 18:55:00.000000 drf-rw-serializers-1.1.1/tests/test_mixins.py
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)     1810 2023-12-22 18:55:00.000000 drf-rw-serializers-1.1.1/tests/test_viewsets.py
+-rw-r--r--   0        0        0      198 2024-05-27 19:09:53.315386 drf_rw_serializers-1.2.0/AUTHORS.rst
+-rw-r--r--   0        0        0     1104 2024-05-27 19:09:53.315386 drf_rw_serializers-1.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     3167 2024-05-27 19:09:53.315386 drf_rw_serializers-1.2.0/README.rst
+-rw-r--r--   0        0        0      359 2024-05-27 19:09:53.319386 drf_rw_serializers-1.2.0/drf_rw_serializers/__init__.py
+-rw-r--r--   0        0        0      336 2024-05-27 19:09:53.319386 drf_rw_serializers-1.2.0/drf_rw_serializers/apps.py
+-rw-r--r--   0        0        0     6945 2024-05-27 19:09:53.319386 drf_rw_serializers-1.2.0/drf_rw_serializers/generics.py
+-rw-r--r--   0        0        0     2192 2024-05-27 19:09:53.319386 drf_rw_serializers-1.2.0/drf_rw_serializers/mixins.py
+-rw-r--r--   0        0        0      535 2024-05-27 19:09:53.319386 drf_rw_serializers-1.2.0/drf_rw_serializers/viewsets.py
+-rw-r--r--   0        0        0     1436 2024-05-27 19:09:53.319386 drf_rw_serializers-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3918 1970-01-01 00:00:00.000000 drf_rw_serializers-1.2.0/PKG-INFO
```

### Comparing `drf-rw-serializers-1.1.1/LICENSE.txt` & `drf_rw_serializers-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `drf-rw-serializers-1.1.1/README.rst` & `drf_rw_serializers-1.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/drf-rw-serializers.svg
     :target: https://pypi.python.org/pypi/drf-rw-serializers/
     :alt: PyPI
 
-.. |ga-badge| image:: https://github.com/vintasoftware/drf-rw-serializers/actions/workflows/config.yml/badge.svg?branch=master
+.. |ga-badge| image:: https://github.com/vintasoftware/drf-rw-serializers/actions/workflows/tests.yml/badge.svg?branch=master
     :target: https://github.com/vintasoftware/drf-rw-serializers
     :alt: GitHub Actions
 
 .. |codecov-badge| image:: http://codecov.io/github/vintasoftware/drf-rw-serializers/coverage.svg?branch=master
     :target: http://codecov.io/github/vintasoftware/drf-rw-serializers?branch=master
     :alt: Codecov
```

### Comparing `drf-rw-serializers-1.1.1/drf_rw_serializers/mixins.py` & `drf_rw_serializers-1.2.0/drf_rw_serializers/mixins.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,61 +1,55 @@
 # -*- coding: utf-8 -*-
 
 from rest_framework import mixins, status
 from rest_framework.response import Response
 
 
 class UpdateModelMixin(mixins.UpdateModelMixin):
-
     def update(self, request, *args, **kwargs):
-        partial = kwargs.pop('partial', False)
+        partial = kwargs.pop("partial", False)
         instance = self.get_object()
-        write_serializer = self.get_write_serializer(
-            instance, data=request.data, partial=partial)
+        write_serializer = self.get_write_serializer(instance, data=request.data, partial=partial)
         write_serializer.is_valid(raise_exception=True)
         self.perform_update(write_serializer)
 
         # pylint: disable=protected-access
-        if getattr(instance, '_prefetched_objects_cache', None) is not None:
-
+        if getattr(instance, "_prefetched_objects_cache", None) is not None:
             # If 'prefetch_related' has been applied to a queryset, we need to
             # forcibly invalidate the prefetch cache on the instance.
             instance._prefetched_objects_cache = {}
         # pylint: enable=protected-access
         read_serializer = self.get_read_serializer(instance)
 
         return Response(read_serializer.data)
 
 
 class CreateModelMixin(mixins.CreateModelMixin):
-
     def create(self, request, *args, **kwargs):
         write_serializer = self.get_write_serializer(data=request.data)
         write_serializer.is_valid(raise_exception=True)
         self.perform_create(write_serializer)
 
         read_serializer = self.get_read_serializer(write_serializer.instance)
         headers = self.get_success_headers(read_serializer.data)
 
         return Response(read_serializer.data, status=status.HTTP_201_CREATED, headers=headers)
 
 
 class ListModelMixin(mixins.ListModelMixin):
-
     def list(self, request, *args, **kwargs):
         queryset = self.filter_queryset(self.get_queryset())
 
         page = self.paginate_queryset(queryset)
         if page is not None:
             serializer = self.get_read_serializer(page, many=True)
             return self.get_paginated_response(serializer.data)
 
         serializer = self.get_read_serializer(queryset, many=True)
         return Response(serializer.data)
 
 
 class RetrieveModelMixin(mixins.RetrieveModelMixin):
-
     def retrieve(self, request, *args, **kwargs):
         instance = self.get_object()
         serializer = self.get_read_serializer(instance)
         return Response(serializer.data)
```

