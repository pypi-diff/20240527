# Comparing `tmp/fastapi_namespace_vet1ments-0.1.5.tar.gz` & `tmp/fastapi_namespace_vet1ments-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_namespace_vet1ments-0.1.5.tar", last modified: Wed May 22 21:09:32 2024, max compression
+gzip compressed data, was "fastapi_namespace_vet1ments-0.1.6.tar", last modified: Mon May 27 19:47:19 2024, max compression
```

## Comparing `fastapi_namespace_vet1ments-0.1.5.tar` & `fastapi_namespace_vet1ments-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:09:32.810899 fastapi_namespace_vet1ments-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-22 21:09:25.000000 fastapi_namespace_vet1ments-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-22 21:09:32.810899 fastapi_namespace_vet1ments-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-22 21:09:25.000000 fastapi_namespace_vet1ments-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:09:32.810899 fastapi_namespace_vet1ments-0.1.5/fastapi_namespace/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 21:09:25.000000 fastapi_namespace_vet1ments-0.1.5/fastapi_namespace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-05-22 21:09:25.000000 fastapi_namespace_vet1ments-0.1.5/fastapi_namespace/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    13011 2024-05-22 21:09:25.000000 fastapi_namespace_vet1ments-0.1.5/fastapi_namespace/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-22 21:09:25.000000 fastapi_namespace_vet1ments-0.1.5/fastapi_namespace/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:09:32.810899 fastapi_namespace_vet1ments-0.1.5/fastapi_namespace/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 21:09:25.000000 fastapi_namespace_vet1ments-0.1.5/fastapi_namespace/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-22 21:09:25.000000 fastapi_namespace_vet1ments-0.1.5/fastapi_namespace/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 21:09:25.000000 fastapi_namespace_vet1ments-0.1.5/fastapi_namespace/tests/test2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-22 21:09:25.000000 fastapi_namespace_vet1ments-0.1.5/fastapi_namespace/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-22 21:09:25.000000 fastapi_namespace_vet1ments-0.1.5/fastapi_namespace/typings.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-22 21:09:25.000000 fastapi_namespace_vet1ments-0.1.5/fastapi_namespace/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:09:32.810899 fastapi_namespace_vet1ments-0.1.5/fastapi_namespace_vet1ments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-22 21:09:32.000000 fastapi_namespace_vet1ments-0.1.5/fastapi_namespace_vet1ments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-22 21:09:32.000000 fastapi_namespace_vet1ments-0.1.5/fastapi_namespace_vet1ments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 21:09:32.000000 fastapi_namespace_vet1ments-0.1.5/fastapi_namespace_vet1ments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 21:09:32.000000 fastapi_namespace_vet1ments-0.1.5/fastapi_namespace_vet1ments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 21:09:32.000000 fastapi_namespace_vet1ments-0.1.5/fastapi_namespace_vet1ments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 21:09:32.810899 fastapi_namespace_vet1ments-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-22 21:09:31.000000 fastapi_namespace_vet1ments-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:47:19.485398 fastapi_namespace_vet1ments-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-27 19:47:19.485398 fastapi_namespace_vet1ments-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:47:19.481398 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:47:19.481398 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/mixinBase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:47:19.481398 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/token/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/token/jwtTokenMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/token/opaqueTokenMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16589 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/token/tokenBaseMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/token/typings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/token/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13011 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:47:19.481398 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/tests/test2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/typings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:47:19.485398 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace_vet1ments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-27 19:47:19.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace_vet1ments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-27 19:47:19.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace_vet1ments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:47:19.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace_vet1ments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 19:47:19.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace_vet1ments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 19:47:19.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace_vet1ments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 19:47:19.485398 fastapi_namespace_vet1ments-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-27 19:47:18.000000 fastapi_namespace_vet1ments-0.1.6/setup.py
```

### Comparing `fastapi_namespace_vet1ments-0.1.5/LICENSE` & `fastapi_namespace_vet1ments-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.5/PKG-INFO` & `fastapi_namespace_vet1ments-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_namespace_vet1ments
-Version: 0.1.5
+Version: 0.1.6
 Summary: For FastAPI Routing Class
 Author: no hong seok
 Author-email: vet1ments@naver.com
 Maintainer: no hong seok
 Maintainer-email: vet1ments@naver.com
 License: MIT
 Project-URL: Repository, https://github.com/vet1ments/fastapi_namespace
```

### Comparing `fastapi_namespace_vet1ments-0.1.5/README.md` & `fastapi_namespace_vet1ments-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.5/fastapi_namespace/mixin.py` & `fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/mixinBase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,15 @@
-from .resource import Resource
-from typing import ClassVar, Iterable, Sequence, Literal
+from fastapi_namespace.resource import Resource
+from fastapi_namespace.utils import delete_none
+from fastapi_namespace.typings import MethodType
+from typing import Iterable
+from abc import ABCMeta
 from fastapi.params import Depends
-from .utils import delete_none
-from .typings import DependsType, MethodType
 
 class _Meta(type):
-    global_dependencies: Iterable[Depends]
-    get_dependencies: Iterable[Depends]
-    post_dependencies: Iterable[Depends]
-    put_dependencies: Iterable[Depends]
-    delete_dependencies: Iterable[Depends]
-    options_dependencies: Iterable[Depends]
-    head_dependencies: Iterable[Depends]
-    patch_dependencies: Iterable[Depends]
-    trace_dependencies: Iterable[Depends]
-
     def __new__(mcs, name, bases, namespace):
         global_dependencies: Iterable[Depends] = getattr(bases[0], 'global_dependencies', None)
         if global_dependencies is not None:
             _global_dependencies = namespace.get('global_dependencies', [])
             global_dependencies = [*global_dependencies, *_global_dependencies]
 
         get_dependencies: Iterable[Depends] = getattr(bases[0], 'get_dependencies', None)
@@ -70,51 +61,54 @@
             'options_dependencies': options_dependencies,
             'head_dependencies': head_dependencies,
             'patch_dependencies': patch_dependencies,
             'trace_dependencies': trace_dependencies,
         }))
         return type.__new__(mcs, name, bases, namespace)
 
-class MixinBase(Resource, metaclass=_Meta):
+class __Meta(_Meta, ABCMeta):
+    pass
+
+class MixinBase(Resource, metaclass=__Meta):
     global_dependencies: Iterable[Depends]
     get_dependencies: Iterable[Depends]
     post_dependencies: Iterable[Depends]
     put_dependencies: Iterable[Depends]
     delete_dependencies: Iterable[Depends]
     options_dependencies: Iterable[Depends]
     head_dependencies: Iterable[Depends]
     patch_dependencies: Iterable[Depends]
     trace_dependencies: Iterable[Depends]
 
-    def _add_depends(self, type_: MethodType, depends: Depends):
+    def _add_depends(self, type_: MethodType, depends: Depends) -> None:
         assert isinstance(depends, Depends), "Depends must be a Depends"
         key = f'{type_}_dependencies'
         dependencies = getattr(self, key, [])
         dependencies.append(depends)
         setattr(self, key, dependencies)
 
-    def add_global_depends(self, depends: Depends):
+    def add_global_depends(self, depends: Depends) -> None:
         return self._add_depends('global', depends)
 
-    def add_get_depends(self, depends: Depends):
+    def add_get_depends(self, depends: Depends) -> None:
         return self._add_depends('get', depends)
 
-    def add_post_depends(self, depends: Depends):
+    def add_post_depends(self, depends: Depends) -> None:
         return self._add_depends('post', depends)
 
-    def add_put_depends(self, depends: Depends):
+    def add_put_depends(self, depends: Depends) -> None:
         return self._add_depends('put', depends)
 
-    def add_delete_depends(self, depends: Depends):
+    def add_delete_depends(self, depends: Depends) -> None:
         return self._add_depends('delete', depends)
 
-    def add_options_depends(self, depends: Depends):
+    def add_options_depends(self, depends: Depends) -> None:
         return self._add_depends('options', depends)
 
-    def add_head_depends(self, depends: Depends):
+    def add_head_depends(self, depends: Depends) -> None:
         return self._add_depends('head', depends)
 
-    def add_patch_depends(self, depends: Depends):
+    def add_patch_depends(self, depends: Depends) -> None:
         return self._add_depends('patch', depends)
 
-    def add_trace_depends(self, depends: Depends):
+    def add_trace_depends(self, depends: Depends) -> None:
         return self._add_depends('trace', depends)
```

### Comparing `fastapi_namespace_vet1ments-0.1.5/fastapi_namespace/namespace.py` & `fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/namespace.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.5/fastapi_namespace/resource.py` & `fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/resource.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.5/fastapi_namespace/types.py` & `fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/types.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.5/fastapi_namespace/typings.py` & `fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/typings.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.5/fastapi_namespace_vet1ments.egg-info/PKG-INFO` & `fastapi_namespace_vet1ments-0.1.6/fastapi_namespace_vet1ments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-namespace-vet1ments
-Version: 0.1.5
+Version: 0.1.6
 Summary: For FastAPI Routing Class
 Author: no hong seok
 Author-email: vet1ments@naver.com
 Maintainer: no hong seok
 Maintainer-email: vet1ments@naver.com
 License: MIT
 Project-URL: Repository, https://github.com/vet1ments/fastapi_namespace
```

### Comparing `fastapi_namespace_vet1ments-0.1.5/setup.py` & `fastapi_namespace_vet1ments-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='fastapi_namespace_vet1ments',
     description="For FastAPI Routing Class",
-    version='0.1.5',
+    version='0.1.6',
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.11.0',
     author="no hong seok",
     author_email="vet1ments@naver.com",
     maintainer="no hong seok",
     maintainer_email="vet1ments@naver.com",
```

