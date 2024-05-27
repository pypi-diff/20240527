# Comparing `tmp/graphene_django_query_optimizer-0.6.1.tar.gz` & `tmp/graphene_django_query_optimizer-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene_django_query_optimizer-0.6.1.tar", max compression
+gzip compressed data, was "graphene_django_query_optimizer-0.6.2.tar", max compression
```

## Comparing `graphene_django_query_optimizer-0.6.1.tar` & `graphene_django_query_optimizer-0.6.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1064 2024-05-27 07:09:48.252355 graphene_django_query_optimizer-0.6.1/LICENSE
--rw-r--r--   0        0        0     3151 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/README.md
--rw-r--r--   0        0        0     6906 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      496 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/__init__.py
--rw-r--r--   0        0        0    11972 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/ast.py
--rw-r--r--   0        0        0     8967 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/compiler.py
--rw-r--r--   0        0        0     2847 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/converters.py
--rw-r--r--   0        0        0      177 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/errors.py
--rw-r--r--   0        0        0    17282 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/fields.py
--rw-r--r--   0        0        0     1686 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/filter.py
--rw-r--r--   0        0        0     5687 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/filter_info.py
--rw-r--r--   0        0        0    11776 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/optimizer.py
--rw-r--r--   0        0        0     4130 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/prefetch_hack.py
--rw-r--r--   0        0        0        0 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/py.typed
--rw-r--r--   0        0        0     3600 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/selections.py
--rw-r--r--   0        0        0     2520 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/settings.py
--rw-r--r--   0        0        0     3212 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/types.py
--rw-r--r--   0        0        0     3845 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/typing.py
--rw-r--r--   0        0        0     6842 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/utils.py
--rw-r--r--   0        0        0     3888 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/validators.py
--rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 graphene_django_query_optimizer-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-27 07:58:38.722235 graphene_django_query_optimizer-0.6.2/LICENSE
+-rw-r--r--   0        0        0     3151 2024-05-27 07:58:38.722235 graphene_django_query_optimizer-0.6.2/README.md
+-rw-r--r--   0        0        0     6906 2024-05-27 07:58:38.722235 graphene_django_query_optimizer-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      496 2024-05-27 07:58:38.722235 graphene_django_query_optimizer-0.6.2/query_optimizer/__init__.py
+-rw-r--r--   0        0        0    11972 2024-05-27 07:58:38.722235 graphene_django_query_optimizer-0.6.2/query_optimizer/ast.py
+-rw-r--r--   0        0        0     8967 2024-05-27 07:58:38.722235 graphene_django_query_optimizer-0.6.2/query_optimizer/compiler.py
+-rw-r--r--   0        0        0     2847 2024-05-27 07:58:38.722235 graphene_django_query_optimizer-0.6.2/query_optimizer/converters.py
+-rw-r--r--   0        0        0      177 2024-05-27 07:58:38.722235 graphene_django_query_optimizer-0.6.2/query_optimizer/errors.py
+-rw-r--r--   0        0        0    17282 2024-05-27 07:58:38.722235 graphene_django_query_optimizer-0.6.2/query_optimizer/fields.py
+-rw-r--r--   0        0        0     1686 2024-05-27 07:58:38.722235 graphene_django_query_optimizer-0.6.2/query_optimizer/filter.py
+-rw-r--r--   0        0        0     5687 2024-05-27 07:58:38.722235 graphene_django_query_optimizer-0.6.2/query_optimizer/filter_info.py
+-rw-r--r--   0        0        0    12012 2024-05-27 07:58:38.722235 graphene_django_query_optimizer-0.6.2/query_optimizer/optimizer.py
+-rw-r--r--   0        0        0     4130 2024-05-27 07:58:38.722235 graphene_django_query_optimizer-0.6.2/query_optimizer/prefetch_hack.py
+-rw-r--r--   0        0        0        0 2024-05-27 07:58:38.722235 graphene_django_query_optimizer-0.6.2/query_optimizer/py.typed
+-rw-r--r--   0        0        0     3600 2024-05-27 07:58:38.722235 graphene_django_query_optimizer-0.6.2/query_optimizer/selections.py
+-rw-r--r--   0        0        0     2520 2024-05-27 07:58:38.722235 graphene_django_query_optimizer-0.6.2/query_optimizer/settings.py
+-rw-r--r--   0        0        0     3212 2024-05-27 07:58:38.722235 graphene_django_query_optimizer-0.6.2/query_optimizer/types.py
+-rw-r--r--   0        0        0     3845 2024-05-27 07:58:38.722235 graphene_django_query_optimizer-0.6.2/query_optimizer/typing.py
+-rw-r--r--   0        0        0     6842 2024-05-27 07:58:38.722235 graphene_django_query_optimizer-0.6.2/query_optimizer/utils.py
+-rw-r--r--   0        0        0     3888 2024-05-27 07:58:38.722235 graphene_django_query_optimizer-0.6.2/query_optimizer/validators.py
+-rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 graphene_django_query_optimizer-0.6.2/PKG-INFO
```

### Comparing `graphene_django_query_optimizer-0.6.1/LICENSE` & `graphene_django_query_optimizer-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.1/README.md` & `graphene_django_query_optimizer-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.1/pyproject.toml` & `graphene_django_query_optimizer-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graphene-django-query-optimizer"
-version = "0.6.1"
+version = "0.6.2"
 description = "Automatically optimize SQL queries in Graphene-Django schemas."
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "query_optimizer" },
 ]
```

### Comparing `graphene_django_query_optimizer-0.6.1/query_optimizer/ast.py` & `graphene_django_query_optimizer-0.6.2/query_optimizer/ast.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.1/query_optimizer/compiler.py` & `graphene_django_query_optimizer-0.6.2/query_optimizer/compiler.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.1/query_optimizer/converters.py` & `graphene_django_query_optimizer-0.6.2/query_optimizer/converters.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.1/query_optimizer/fields.py` & `graphene_django_query_optimizer-0.6.2/query_optimizer/fields.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.1/query_optimizer/filter.py` & `graphene_django_query_optimizer-0.6.2/query_optimizer/filter.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.1/query_optimizer/filter_info.py` & `graphene_django_query_optimizer-0.6.2/query_optimizer/filter_info.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.1/query_optimizer/optimizer.py` & `graphene_django_query_optimizer-0.6.2/query_optimizer/optimizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
         :param queryset: QuerySet to optimize.
         :param filter_info: Additional filtering info to use for the optimization.
         """
         if filter_info is None:
             filter_info = get_filter_info(self.info, queryset.model)
 
-        self.pre_compilation(queryset.model)
+        self.pre_compilation()
         results = self.compile(filter_info=filter_info)
 
         if filter_info is not None and filter_info.get("filterset_class") is not None:
             filterset = filter_info["filterset_class"](
                 data=self.process_filters(filter_info["filters"]),
                 queryset=queryset,
                 request=self.info.context,
@@ -270,11 +270,16 @@
 
     def run_pre_resolvers(self, queryset: QuerySet, filter_info: GraphQLFilterInfo) -> QuerySet:
         for name, resolver in self.pre_resolvers.items():
             filters = filter_info["children"][name]["filters"]
             queryset = resolver(queryset, self.info, **filters)
         return queryset
 
-    def pre_compilation(self, model: type[Model]) -> None:
-        object_type: Optional[DjangoObjectType] = get_global_registry().get_type_for_model(model)
+    def pre_compilation(self) -> None:
+        object_type: Optional[DjangoObjectType] = get_global_registry().get_type_for_model(self.model)
         if callable(getattr(object_type, "pre_compilation_hook", None)):
             object_type.pre_compilation_hook(self)
+
+        # Run pre-compilation for all select related optimizers, since they might add annotations,
+        # which would promote the select related to prefetch related.
+        for optimizer in self.select_related.values():
+            optimizer.pre_compilation()
```

### Comparing `graphene_django_query_optimizer-0.6.1/query_optimizer/prefetch_hack.py` & `graphene_django_query_optimizer-0.6.2/query_optimizer/prefetch_hack.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.1/query_optimizer/selections.py` & `graphene_django_query_optimizer-0.6.2/query_optimizer/selections.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.1/query_optimizer/settings.py` & `graphene_django_query_optimizer-0.6.2/query_optimizer/settings.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.1/query_optimizer/types.py` & `graphene_django_query_optimizer-0.6.2/query_optimizer/types.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.1/query_optimizer/typing.py` & `graphene_django_query_optimizer-0.6.2/query_optimizer/typing.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.1/query_optimizer/utils.py` & `graphene_django_query_optimizer-0.6.2/query_optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.1/query_optimizer/validators.py` & `graphene_django_query_optimizer-0.6.2/query_optimizer/validators.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.1/PKG-INFO` & `graphene_django_query_optimizer-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django-query-optimizer
-Version: 0.6.1
+Version: 0.6.2
 Summary: Automatically optimize SQL queries in Graphene-Django schemas.
 Home-page: https://mrthearman.github.io/graphene-django-query-optimizer
 License: MIT
 Keywords: django,graphene,sql,graphql,python,query,optimizer,optimization
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.9,<4
```

