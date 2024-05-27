# Comparing `tmp/lazy_type_hint-2.2.3.tar.gz` & `tmp/lazy_type_hint-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_type_hint-2.2.3.tar", max compression
+gzip compressed data, was "lazy_type_hint-2.2.4.tar", max compression
```

## Comparing `lazy_type_hint-2.2.3.tar` & `lazy_type_hint-2.2.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      257 2024-04-03 13:39:39.210757 lazy_type_hint-2.2.3/lazy_type_hint/__init__.py
--rw-r--r--   0        0        0      495 2024-04-03 08:50:18.646693 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/__init__.py
--rw-r--r--   0        0        0    12413 2024-04-29 13:45:53.508452 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/data_type_tree.py
--rw-r--r--   0        0        0     7793 2024-05-07 20:41:03.159890 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/factory.py
--rw-r--r--   0        0        0     1279 2024-04-29 13:45:53.522867 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/__init__.py
--rw-r--r--   0        0        0    17314 2024-04-19 13:25:22.433858 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py
--rw-r--r--   0        0        0     2963 2024-04-20 12:20:31.948128 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py
--rw-r--r--   0        0        0      803 2024-04-23 15:02:40.562766 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/iterator_data_type_tree.py
--rw-r--r--   0        0        0     1144 2024-04-23 15:02:40.563766 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py
--rw-r--r--   0        0        0     5922 2024-04-23 15:02:40.570766 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py
--rw-r--r--   0        0        0      601 2024-04-19 13:25:22.452857 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py
--rw-r--r--   0        0        0     7806 2024-05-08 07:23:27.799663 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py
--rw-r--r--   0        0        0     1779 2024-05-07 20:57:24.444184 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/pandas_series_data_type_tree.py
--rw-r--r--   0        0        0     1309 2024-04-20 12:20:31.951328 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py
--rw-r--r--   0        0        0     6646 2024-04-29 13:45:53.539888 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py
--rw-r--r--   0        0        0     1988 2024-04-23 15:02:40.576999 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py
--rw-r--r--   0        0        0     2129 2024-04-23 15:02:40.576999 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py
--rw-r--r--   0        0        0     1039 2024-04-29 13:45:53.548265 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py
--rw-r--r--   0        0        0     3114 2024-04-23 15:02:40.585280 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py
--rw-r--r--   0        0        0     1478 2024-04-23 15:02:40.585280 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py
--rw-r--r--   0        0        0      396 2024-04-23 15:02:40.591280 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/io_data_type_tree.py
--rw-r--r--   0        0        0      432 2024-04-23 15:02:40.597509 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/module_data_type_tree.py
--rw-r--r--   0        0        0      511 2024-04-23 15:02:40.606702 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/numpy_data_type_tree.py
--rw-r--r--   0        0        0     1003 2024-04-14 10:39:38.880313 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py
--rw-r--r--   0        0        0      794 2024-04-23 15:02:40.615914 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py
--rw-r--r--   0        0        0      192 2024-04-03 08:50:18.656845 lazy_type_hint-2.2.3/lazy_type_hint/file_modifiers/__init__.py
--rw-r--r--   0        0        0    11392 2024-04-03 15:48:14.641664 lazy_type_hint-2.2.3/lazy_type_hint/file_modifiers/py_file_modifier.py
--rw-r--r--   0        0        0    17473 2024-04-03 08:50:18.657845 lazy_type_hint-2.2.3/lazy_type_hint/file_modifiers/yaml_file_modifier.py
--rw-r--r--   0        0        0     2340 2024-04-29 13:45:49.656127 lazy_type_hint-2.2.3/lazy_type_hint/generators/lazy_type_hint.py
--rw-r--r--   0        0        0     3137 2024-04-29 13:45:49.662517 lazy_type_hint-2.2.3/lazy_type_hint/generators/lazy_type_hint_abc.py
--rw-r--r--   0        0        0    10092 2024-04-29 13:45:49.712316 lazy_type_hint-2.2.3/lazy_type_hint/generators/lazy_type_hint_live.py
--rw-r--r--   0        0        0        0 2024-04-03 08:50:18.658845 lazy_type_hint-2.2.3/lazy_type_hint/py.typed
--rw-r--r--   0        0        0     2222 2024-04-23 15:02:15.663344 lazy_type_hint-2.2.3/lazy_type_hint/strategies.py
--rw-r--r--   0        0        0      732 2024-04-19 13:25:22.511264 lazy_type_hint-2.2.3/lazy_type_hint/utils/__init__.py
--rw-r--r--   0        0        0     2303 2024-04-03 08:50:18.660845 lazy_type_hint-2.2.3/lazy_type_hint/utils/docstring_formatter.py
--rw-r--r--   0        0        0     5900 2024-04-29 13:45:53.555265 lazy_type_hint-2.2.3/lazy_type_hint/utils/import_manager.py
--rw-r--r--   0        0        0     5008 2024-04-14 13:10:20.018341 lazy_type_hint-2.2.3/lazy_type_hint/utils/mypy.py
--rw-r--r--   0        0        0     1275 2024-04-03 08:50:18.662845 lazy_type_hint-2.2.3/lazy_type_hint/utils/ordered_set.py
--rw-r--r--   0        0        0      669 2024-04-03 08:50:18.662845 lazy_type_hint-2.2.3/lazy_type_hint/utils/test_ordered_set.py
--rw-r--r--   0        0        0     3712 2024-04-20 12:20:31.953328 lazy_type_hint-2.2.3/lazy_type_hint/utils/utils.py
--rw-r--r--   0        0        0     2664 2024-05-08 07:23:27.800664 lazy_type_hint-2.2.3/pyproject.toml
--rw-r--r--   0        0        0    12338 2024-04-29 13:45:49.641764 lazy_type_hint-2.2.3/README.md
--rw-r--r--   0        0        0    12602 1970-01-01 00:00:00.000000 lazy_type_hint-2.2.3/PKG-INFO
+-rw-r--r--   0        0        0      257 2024-04-03 13:39:39.210757 lazy_type_hint-2.2.4/lazy_type_hint/__init__.py
+-rw-r--r--   0        0        0      495 2024-04-03 08:50:18.646693 lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/__init__.py
+-rw-r--r--   0        0        0    12413 2024-04-29 13:45:53.508452 lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/data_type_tree.py
+-rw-r--r--   0        0        0     7793 2024-05-07 20:41:03.159890 lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/factory.py
+-rw-r--r--   0        0        0     1279 2024-04-29 13:45:53.522867 lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/__init__.py
+-rw-r--r--   0        0        0    17419 2024-05-27 09:44:55.198168 lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py
+-rw-r--r--   0        0        0     2963 2024-04-20 12:20:31.948128 lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py
+-rw-r--r--   0        0        0      803 2024-04-23 15:02:40.562766 lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/iterator_data_type_tree.py
+-rw-r--r--   0        0        0     1144 2024-04-23 15:02:40.563766 lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py
+-rw-r--r--   0        0        0     5922 2024-04-23 15:02:40.570766 lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py
+-rw-r--r--   0        0        0      601 2024-04-19 13:25:22.452857 lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py
+-rw-r--r--   0        0        0     7806 2024-05-08 07:23:27.799663 lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py
+-rw-r--r--   0        0        0     1779 2024-05-07 20:57:24.444184 lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/pandas_series_data_type_tree.py
+-rw-r--r--   0        0        0     1309 2024-04-20 12:20:31.951328 lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py
+-rw-r--r--   0        0        0     6646 2024-04-29 13:45:53.539888 lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py
+-rw-r--r--   0        0        0     1988 2024-04-23 15:02:40.576999 lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py
+-rw-r--r--   0        0        0     2129 2024-04-23 15:02:40.576999 lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py
+-rw-r--r--   0        0        0     1039 2024-04-29 13:45:53.548265 lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py
+-rw-r--r--   0        0        0     3114 2024-04-23 15:02:40.585280 lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py
+-rw-r--r--   0        0        0     1478 2024-04-23 15:02:40.585280 lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py
+-rw-r--r--   0        0        0      396 2024-04-23 15:02:40.591280 lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/simple_data_type_tree/io_data_type_tree.py
+-rw-r--r--   0        0        0      432 2024-04-23 15:02:40.597509 lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/simple_data_type_tree/module_data_type_tree.py
+-rw-r--r--   0        0        0      511 2024-04-23 15:02:40.606702 lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/simple_data_type_tree/numpy_data_type_tree.py
+-rw-r--r--   0        0        0     1003 2024-04-14 10:39:38.880313 lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py
+-rw-r--r--   0        0        0      794 2024-04-23 15:02:40.615914 lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py
+-rw-r--r--   0        0        0      192 2024-04-03 08:50:18.656845 lazy_type_hint-2.2.4/lazy_type_hint/file_modifiers/__init__.py
+-rw-r--r--   0        0        0    11392 2024-04-03 15:48:14.641664 lazy_type_hint-2.2.4/lazy_type_hint/file_modifiers/py_file_modifier.py
+-rw-r--r--   0        0        0    17473 2024-04-03 08:50:18.657845 lazy_type_hint-2.2.4/lazy_type_hint/file_modifiers/yaml_file_modifier.py
+-rw-r--r--   0        0        0     2340 2024-04-29 13:45:49.656127 lazy_type_hint-2.2.4/lazy_type_hint/generators/lazy_type_hint.py
+-rw-r--r--   0        0        0     3137 2024-04-29 13:45:49.662517 lazy_type_hint-2.2.4/lazy_type_hint/generators/lazy_type_hint_abc.py
+-rw-r--r--   0        0        0    10092 2024-04-29 13:45:49.712316 lazy_type_hint-2.2.4/lazy_type_hint/generators/lazy_type_hint_live.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:50:18.658845 lazy_type_hint-2.2.4/lazy_type_hint/py.typed
+-rw-r--r--   0        0        0     2222 2024-04-23 15:02:15.663344 lazy_type_hint-2.2.4/lazy_type_hint/strategies.py
+-rw-r--r--   0        0        0      732 2024-04-19 13:25:22.511264 lazy_type_hint-2.2.4/lazy_type_hint/utils/__init__.py
+-rw-r--r--   0        0        0     2303 2024-04-03 08:50:18.660845 lazy_type_hint-2.2.4/lazy_type_hint/utils/docstring_formatter.py
+-rw-r--r--   0        0        0     5900 2024-04-29 13:45:53.555265 lazy_type_hint-2.2.4/lazy_type_hint/utils/import_manager.py
+-rw-r--r--   0        0        0     5008 2024-04-14 13:10:20.018341 lazy_type_hint-2.2.4/lazy_type_hint/utils/mypy.py
+-rw-r--r--   0        0        0     1275 2024-04-03 08:50:18.662845 lazy_type_hint-2.2.4/lazy_type_hint/utils/ordered_set.py
+-rw-r--r--   0        0        0      669 2024-04-03 08:50:18.662845 lazy_type_hint-2.2.4/lazy_type_hint/utils/test_ordered_set.py
+-rw-r--r--   0        0        0     3712 2024-04-20 12:20:31.953328 lazy_type_hint-2.2.4/lazy_type_hint/utils/utils.py
+-rw-r--r--   0        0        0     2664 2024-05-27 09:44:55.199168 lazy_type_hint-2.2.4/pyproject.toml
+-rw-r--r--   0        0        0    12338 2024-04-29 13:45:49.641764 lazy_type_hint-2.2.4/README.md
+-rw-r--r--   0        0        0    12602 1970-01-01 00:00:00.000000 lazy_type_hint-2.2.4/PKG-INFO
```

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/data_type_tree.py` & `lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/factory.py` & `lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/factory.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/__init__.py` & `lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py` & `lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,14 +331,16 @@
                 modified_line += lines[idx_to_repeat].format(key=key, value=value) + "\n"
             else:
                 docstring = key_docstrings.get(key, "")
                 modified_line += lines[idx_to_repeat].format(key=key, value=value, optional_key_docstring=docstring)
                 if not docstring:
                     modified_line += "\n"
         lines[idx_to_repeat] = modified_line[:-1]
+        if not functional_syntax and not modified_line:
+            lines[idx_to_repeat] = f"{TAB}..."
 
         # Append class docstring if found
         if key_used_as_class_docstring in self.data and key_used_as_class_docstring:
             lines = self._insert_class_docstring(lines, key_used_as_doc=key_used_as_class_docstring)
         return "\n".join(lines)
 
     def update_data_and_metadata(self, other: "DictDataTypeTree") -> None:
```

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py` & `lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/iterator_data_type_tree.py` & `lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/iterator_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py` & `lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py` & `lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py` & `lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py` & `lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/pandas_series_data_type_tree.py` & `lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/pandas_series_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py` & `lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py` & `lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py` & `lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py` & `lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py` & `lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py` & `lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py` & `lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py` & `lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py` & `lazy_type_hint-2.2.4/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/file_modifiers/py_file_modifier.py` & `lazy_type_hint-2.2.4/lazy_type_hint/file_modifiers/py_file_modifier.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/file_modifiers/yaml_file_modifier.py` & `lazy_type_hint-2.2.4/lazy_type_hint/file_modifiers/yaml_file_modifier.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/generators/lazy_type_hint.py` & `lazy_type_hint-2.2.4/lazy_type_hint/generators/lazy_type_hint.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/generators/lazy_type_hint_abc.py` & `lazy_type_hint-2.2.4/lazy_type_hint/generators/lazy_type_hint_abc.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/generators/lazy_type_hint_live.py` & `lazy_type_hint-2.2.4/lazy_type_hint/generators/lazy_type_hint_live.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/strategies.py` & `lazy_type_hint-2.2.4/lazy_type_hint/strategies.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/utils/__init__.py` & `lazy_type_hint-2.2.4/lazy_type_hint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/utils/docstring_formatter.py` & `lazy_type_hint-2.2.4/lazy_type_hint/utils/docstring_formatter.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/utils/import_manager.py` & `lazy_type_hint-2.2.4/lazy_type_hint/utils/import_manager.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/utils/mypy.py` & `lazy_type_hint-2.2.4/lazy_type_hint/utils/mypy.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/utils/ordered_set.py` & `lazy_type_hint-2.2.4/lazy_type_hint/utils/ordered_set.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/utils/test_ordered_set.py` & `lazy_type_hint-2.2.4/lazy_type_hint/utils/test_ordered_set.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/lazy_type_hint/utils/utils.py` & `lazy_type_hint-2.2.4/lazy_type_hint/utils/utils.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/pyproject.toml` & `lazy_type_hint-2.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazy-type-hint"
-version = "2.2.3"
+version = "2.2.4"
 description = "Automate type hint generation in a single line."
 authors = ["Manuel Floriano Vázquez <mflovaa@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.urls]
 Source = "https://github.com/mflova/lazy-type-hint"
```

### Comparing `lazy_type_hint-2.2.3/README.md` & `lazy_type_hint-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.3/PKG-INFO` & `lazy_type_hint-2.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-type-hint
-Version: 2.2.3
+Version: 2.2.4
 Summary: Automate type hint generation in a single line.
 Author: Manuel Floriano Vázquez
 Author-email: mflovaa@gmail.com
 Requires-Python: >=3.8,<=3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

