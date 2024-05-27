# Comparing `tmp/datapipe_core-0.13.7.tar.gz` & `tmp/datapipe_core-0.13.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapipe_core-0.13.7.tar", max compression
+gzip compressed data, was "datapipe_core-0.13.9.tar", max compression
```

## Comparing `datapipe_core-0.13.7.tar` & `datapipe_core-0.13.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1514 2022-12-26 14:30:45.008686 datapipe_core-0.13.7/LICENSE
--rw-r--r--   0        0        0      813 2024-01-02 17:35:06.948128 datapipe_core-0.13.7/README.md
--rw-r--r--   0        0        0        0 2023-05-29 09:25:17.932322 datapipe_core-0.13.7/datapipe/__init__.py
--rw-r--r--   0        0        0    16293 2024-01-02 17:35:19.288226 datapipe_core-0.13.7/datapipe/cli.py
--rw-r--r--   0        0        0     9439 2024-01-02 17:35:19.288226 datapipe_core-0.13.7/datapipe/compute.py
--rw-r--r--   0        0        0    21872 2024-01-02 17:35:19.288226 datapipe_core-0.13.7/datapipe/datatable.py
--rw-r--r--   0        0        0     4654 2024-01-02 17:35:19.288226 datapipe_core-0.13.7/datapipe/event_logger.py
--rw-r--r--   0        0        0     1628 2023-08-02 18:17:25.319165 datapipe_core-0.13.7/datapipe/executor/__init__.py
--rw-r--r--   0        0        0     2295 2024-01-02 17:35:06.948128 datapipe_core-0.13.7/datapipe/executor/ray.py
--rw-r--r--   0        0        0     4477 2024-01-02 17:35:19.288226 datapipe_core-0.13.7/datapipe/lints.py
--rw-r--r--   0        0        0        0 2023-08-02 18:17:25.319165 datapipe_core-0.13.7/datapipe/migrations/__init__.py
--rw-r--r--   0        0        0     2985 2023-08-05 17:20:15.969334 datapipe_core-0.13.7/datapipe/migrations/v013.py
--rw-r--r--   0        0        0      969 2024-01-02 16:27:15.057135 datapipe_core-0.13.7/datapipe/run_config.py
--rw-r--r--   0        0        0     2113 2024-01-02 16:27:17.037133 datapipe_core-0.13.7/datapipe/sql_util.py
--rw-r--r--   0        0        0        0 2023-08-02 18:17:25.319165 datapipe_core-0.13.7/datapipe/step/__init__.py
--rw-r--r--   0        0        0     3761 2024-01-02 17:35:19.288226 datapipe_core-0.13.7/datapipe/step/batch_generate.py
--rw-r--r--   0        0        0    32749 2024-01-02 18:08:11.788207 datapipe_core-0.13.7/datapipe/step/batch_transform.py
--rw-r--r--   0        0        0     3747 2024-01-02 17:35:19.288226 datapipe_core-0.13.7/datapipe/step/datatable_transform.py
--rw-r--r--   0        0        0     2548 2024-01-02 16:23:09.555799 datapipe_core-0.13.7/datapipe/step/update_external_table.py
--rw-r--r--   0        0        0        0 2022-12-26 14:30:45.008686 datapipe_core-0.13.7/datapipe/store/__init__.py
--rw-r--r--   0        0        0     8261 2024-01-02 17:35:19.288226 datapipe_core-0.13.7/datapipe/store/database.py
--rw-r--r--   0        0        0    19094 2024-01-02 17:35:19.288226 datapipe_core-0.13.7/datapipe/store/filedir.py
--rw-r--r--   0        0        0     3595 2024-01-02 16:26:11.974354 datapipe_core-0.13.7/datapipe/store/milvus.py
--rw-r--r--   0        0        0     1331 2024-01-02 16:26:14.154354 datapipe_core-0.13.7/datapipe/store/pandas.py
--rw-r--r--   0        0        0    10462 2024-01-02 17:35:06.948128 datapipe_core-0.13.7/datapipe/store/qdrant.py
--rw-r--r--   0        0        0     3554 2024-01-02 17:35:19.288226 datapipe_core-0.13.7/datapipe/store/redis.py
--rw-r--r--   0        0        0     3877 2024-01-02 16:26:20.434354 datapipe_core-0.13.7/datapipe/store/table_store.py
--rw-r--r--   0        0        0     7292 2024-01-02 16:27:19.467131 datapipe_core-0.13.7/datapipe/types.py
--rw-r--r--   0        0        0     2294 2024-01-02 18:12:00.044171 datapipe_core-0.13.7/pyproject.toml
--rw-r--r--   0        0        0     3162 1970-01-01 00:00:00.000000 datapipe_core-0.13.7/PKG-INFO
+-rw-r--r--   0        0        0     1514 2022-12-26 14:30:45.008686 datapipe_core-0.13.9/LICENSE
+-rw-r--r--   0        0        0      813 2024-01-02 17:35:06.948128 datapipe_core-0.13.9/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 09:25:17.932322 datapipe_core-0.13.9/datapipe/__init__.py
+-rw-r--r--   0        0        0    16293 2024-01-02 17:35:19.288226 datapipe_core-0.13.9/datapipe/cli.py
+-rw-r--r--   0        0        0     9439 2024-01-02 17:35:19.288226 datapipe_core-0.13.9/datapipe/compute.py
+-rw-r--r--   0        0        0    21872 2024-01-08 18:20:29.118665 datapipe_core-0.13.9/datapipe/datatable.py
+-rw-r--r--   0        0        0     4654 2024-01-02 17:35:19.288226 datapipe_core-0.13.9/datapipe/event_logger.py
+-rw-r--r--   0        0        0     1628 2023-08-02 18:17:25.319165 datapipe_core-0.13.9/datapipe/executor/__init__.py
+-rw-r--r--   0        0        0     2295 2024-01-02 17:35:06.948128 datapipe_core-0.13.9/datapipe/executor/ray.py
+-rw-r--r--   0        0        0     4477 2024-01-02 17:35:19.288226 datapipe_core-0.13.9/datapipe/lints.py
+-rw-r--r--   0        0        0        0 2023-08-02 18:17:25.319165 datapipe_core-0.13.9/datapipe/migrations/__init__.py
+-rw-r--r--   0        0        0     2985 2023-08-05 17:20:15.969334 datapipe_core-0.13.9/datapipe/migrations/v013.py
+-rw-r--r--   0        0        0      969 2024-01-02 16:27:15.057135 datapipe_core-0.13.9/datapipe/run_config.py
+-rw-r--r--   0        0        0     2113 2024-01-02 16:27:17.037133 datapipe_core-0.13.9/datapipe/sql_util.py
+-rw-r--r--   0        0        0        0 2023-08-02 18:17:25.319165 datapipe_core-0.13.9/datapipe/step/__init__.py
+-rw-r--r--   0        0        0     3761 2024-01-02 17:35:19.288226 datapipe_core-0.13.9/datapipe/step/batch_generate.py
+-rw-r--r--   0        0        0    32749 2024-01-02 18:08:11.788207 datapipe_core-0.13.9/datapipe/step/batch_transform.py
+-rw-r--r--   0        0        0     3747 2024-01-02 17:35:19.288226 datapipe_core-0.13.9/datapipe/step/datatable_transform.py
+-rw-r--r--   0        0        0     2548 2024-01-02 16:23:09.555799 datapipe_core-0.13.9/datapipe/step/update_external_table.py
+-rw-r--r--   0        0        0        0 2022-12-26 14:30:45.008686 datapipe_core-0.13.9/datapipe/store/__init__.py
+-rw-r--r--   0        0        0     8336 2024-01-16 07:27:39.096010 datapipe_core-0.13.9/datapipe/store/database.py
+-rw-r--r--   0        0        0    19429 2024-01-16 07:27:39.096010 datapipe_core-0.13.9/datapipe/store/filedir.py
+-rw-r--r--   0        0        0     3595 2024-01-02 16:26:11.974354 datapipe_core-0.13.9/datapipe/store/milvus.py
+-rw-r--r--   0        0        0     1331 2024-01-02 16:26:14.154354 datapipe_core-0.13.9/datapipe/store/pandas.py
+-rw-r--r--   0        0        0    10462 2024-01-02 17:35:06.948128 datapipe_core-0.13.9/datapipe/store/qdrant.py
+-rw-r--r--   0        0        0     3554 2024-01-02 17:35:19.288226 datapipe_core-0.13.9/datapipe/store/redis.py
+-rw-r--r--   0        0        0     3877 2024-01-02 16:26:20.434354 datapipe_core-0.13.9/datapipe/store/table_store.py
+-rw-r--r--   0        0        0     7292 2024-01-02 16:27:19.467131 datapipe_core-0.13.9/datapipe/types.py
+-rw-r--r--   0        0        0     2294 2024-01-16 07:27:39.096010 datapipe_core-0.13.9/pyproject.toml
+-rw-r--r--   0        0        0     3162 1970-01-01 00:00:00.000000 datapipe_core-0.13.9/PKG-INFO
```

### Comparing `datapipe_core-0.13.7/LICENSE` & `datapipe_core-0.13.9/LICENSE`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.7/README.md` & `datapipe_core-0.13.9/README.md`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.7/datapipe/cli.py` & `datapipe_core-0.13.9/datapipe/cli.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.7/datapipe/compute.py` & `datapipe_core-0.13.9/datapipe/compute.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.7/datapipe/datatable.py` & `datapipe_core-0.13.9/datapipe/datatable.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.7/datapipe/event_logger.py` & `datapipe_core-0.13.9/datapipe/event_logger.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.7/datapipe/executor/__init__.py` & `datapipe_core-0.13.9/datapipe/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.7/datapipe/executor/ray.py` & `datapipe_core-0.13.9/datapipe/executor/ray.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.7/datapipe/lints.py` & `datapipe_core-0.13.9/datapipe/lints.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.7/datapipe/migrations/v013.py` & `datapipe_core-0.13.9/datapipe/migrations/v013.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.7/datapipe/run_config.py` & `datapipe_core-0.13.9/datapipe/run_config.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.7/datapipe/sql_util.py` & `datapipe_core-0.13.9/datapipe/sql_util.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.7/datapipe/step/batch_generate.py` & `datapipe_core-0.13.9/datapipe/step/batch_generate.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.7/datapipe/step/batch_transform.py` & `datapipe_core-0.13.9/datapipe/step/batch_transform.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.7/datapipe/step/datatable_transform.py` & `datapipe_core-0.13.9/datapipe/step/datatable_transform.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.7/datapipe/step/update_external_table.py` & `datapipe_core-0.13.9/datapipe/step/update_external_table.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.7/datapipe/store/database.py` & `datapipe_core-0.13.9/datapipe/store/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,20 +237,23 @@
             return pd.concat(res, ignore_index=True)
 
         else:
             with self.dbconn.con.begin() as con:
                 return pd.read_sql_query(sql, con=con)
 
     def read_rows_meta_pseudo_df(
-        self, chunksize: int = 1000, run_config: Optional[RunConfig] = None
+        self,
+        chunksize: int = 1000,
+        run_config: Optional[RunConfig] = None,
     ) -> Iterator[DataDF]:
-        sql = select(self.data_table.c)
+        sql = select(*self.data_table.c)
 
         sql = sql_apply_runconfig_filter(
             sql, self.data_table, self.primary_keys, run_config
         )
 
-        return pd.read_sql_query(
-            sql,
-            con=self.dbconn.con.execution_options(stream_results=True),
-            chunksize=chunksize,
-        )
+        with self.dbconn.con.execution_options(stream_results=True).begin() as con:
+            yield from pd.read_sql_query(
+                sql,
+                con=con,
+                chunksize=chunksize,
+            )
```

### Comparing `datapipe_core-0.13.7/datapipe/store/filedir.py` & `datapipe_core-0.13.9/datapipe/store/filedir.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,19 +80,23 @@
         return {"image": im}
 
     def dump(self, obj: Dict[str, Any], f: IO) -> None:
         image_data: Any = obj["image"]
 
         if isinstance(image_data, Image.Image):
             image: Image.Image = image_data
+        elif isinstance(image_data, np.ndarray):
+            image = Image.fromarray(image_data)
         elif isinstance(image_data, str):
             image_binary = base64.b64decode(image_data.encode())
             image = Image.open(io.BytesIO(image_binary))
         else:
-            raise Exception("Image must be a bytes string or Pillow Image object")
+            raise Exception(
+                "Image must be a bytes string or np.array or Pillow Image object"
+            )
 
         image.save(f, format=self.format, **self.dump_params)
 
 
 def _pattern_to_attrnames(pat: str) -> List[str]:
     attrnames = re.findall(r"\{([^/]+?)\}", pat)
 
@@ -194,18 +198,21 @@
         add_filepath_column -- если True - в объект добавляется поле filepath с
         адресом файла
 
         read_data -- если False - при чтении не происходит парсинга содержимого
         файла
 
         readonly -- если True, отключить запись файлов; если None, то запись
-        файлов включается в случае, если нету * и ** путей в шаблоне и нет
-        множественных расширений файлов вида (jpg|png|mp4)
-
-        enable_rm -- если True, включить удаление файлов
+        файлов включается в случае, если нету * и ** путей в шаблоне. Если есть
+        множественные суффиксы файлов вида (jpg|png|mp4), то берется файл с
+        первым попавшимся слева направо суффиксом
+
+        enable_rm -- если True, включить удаление файлов. если есть
+        множественные суффиксы файлов вида (jpg|png|mp4), то удаляется каждый из
+        них
 
         fsspec_kwargs -- kwargs для fsspec
         """
 
         self.fsspec_kwargs = fsspec_kwargs or {}
         self.protocol, path = fsspec.core.split_protocol(filename_pattern)
         if "protocol" in self.fsspec_kwargs:
@@ -230,23 +237,16 @@
             else:
                 self.protocol_str = f"{self.protocol}://"
 
         self.filename_patterns = _pattern_to_patterns_or(filename_pattern)
         self.attrnames = _pattern_to_attrnames(filename_pattern)
         self.filename_glob = [_pattern_to_glob(pat) for pat in self.filename_patterns]
         self.filename_match = _pattern_to_match(filename_pattern_for_match)
+        self.filename_match_first_suffix = _pattern_to_match(self.filename_patterns[0])
 
-        # Multiply extensions check
-        if len(self.filename_glob) >= 2:
-            if readonly is not None and not readonly:
-                raise ValueError(
-                    "When `readonly=False`, in filename_pattern shouldn't be several extensions."
-                )
-            elif readonly:
-                readonly = True
         # Any * and ** pattern check
         if "*" in path:
             if readonly is not None and not readonly:
                 raise ValueError(
                     "When `readonly=False`, in filename_pattern shouldn't be any `*` characters."
                 )
             elif readonly is None:
@@ -296,26 +296,35 @@
 
         for row_idx in idx.index:
             attrnames_series = idx.loc[row_idx, self.attrnames]
             assert isinstance(attrnames_series, pd.Series)
 
             attrnames = cast(List[str], attrnames_series.tolist())
 
-            _, path = fsspec.core.split_protocol(
-                self._filenames_from_idxs_values(attrnames)[0]
-            )
-            self.filesystem.rm(path)
+            # Удаляем каждый файл с разными суффиксами, если они есть
+            for filepath in self._filenames_from_idxs_values(attrnames):
+                _, path = fsspec.core.split_protocol(filepath)
+                if self.filesystem.exists(path):
+                    self.filesystem.rm(path)
 
     def _filenames_from_idxs_values(self, idxs_values: List[str]) -> List[str]:
+        """
+        Возвращает по индексам список всевозможных путей согласно шаблону
+        Например для шаблона filedir/{id}.(jpg|png) и индекса id=0
+          ['filedir/0.jpg', 'filedir/0.png']
+        """
         return [
             re.sub(r"\{([^/]+?)\}", Replacer(idxs_values), pat)
             for pat in self.filename_patterns
         ]
 
     def _idxs_values_from_filepath(self, filepath: str) -> Dict[str, Any]:
+        """
+        По пути возвращает список индексов согласно шаблону
+        """
         _, filepath = fsspec.core.split_protocol(filepath)
         m = re.match(self.filename_match, filepath)
         assert (
             m is not None
         ), f"Filepath {filepath} does not match the pattern {self.filename_match}"
 
         data = {}
@@ -356,15 +365,17 @@
                 List[Dict[str, Any]], df.drop(columns=self.attrnames).to_dict("records")
             ),
         ):
             attrnames_series = df.loc[row_idx, self.attrnames]
             assert isinstance(attrnames_series, pd.Series)
 
             idxs_values = attrnames_series.tolist()
-            filepath = self._filenames_from_idxs_values(idxs_values)[0]
+            filepath = self._filenames_from_idxs_values(idxs_values)[
+                0
+            ]  # берем первый суффикс
 
             # Проверяем, что значения ключей не приведут к неоднозначному результату при парсинге регулярки
             self._assert_key_values(filepath, idxs_values)
 
             with self.filesystem.open(filepath, f"w{self.adapter.mode}") as f:
                 self.adapter.dump(data, f)
 
@@ -427,21 +438,17 @@
                         )
                         if self.filesystem.exists(file_open.path)
                     ]
                     if len(found_files) == 0:
                         raise FileNotFoundError(
                             f"No such file: {' or '.join(filepaths)}"
                         )
-                    elif len(found_files) > 1:
-                        raise ValueError(
-                            f"Some files are duplitcated as indexes in filepaths: {found_files}. "
-                            "Change the pattern or delete them."
-                        )
-                    for file_open in found_files:
-                        yield file_open
+                    # Открываем первый попавшися файл согласно суффиксу (aaa|bbb)
+                    file_open = found_files[0]
+                    yield file_open
 
         df_records = []
         for file_open in _iterate_files():
             with file_open as f:
                 data = {}
 
                 if read_data:
@@ -483,32 +490,25 @@
         files = fsspec.open_files(self.filename_glob, **self.fsspec_kwargs)
 
         ids: Dict[str, List[str]] = {attrname: [] for attrname in self.attrnames}
         ukeys = []
         filepaths = []
 
         for f in files:
-            m = re.match(self.filename_match, f.path)
+            m = re.match(self.filename_match_first_suffix, f.path)
+
+            if m is None:
+                continue
 
-            assert m is not None
             for attrname in self.attrnames:
                 ids[attrname].append(m.group(attrname))
 
             ukeys.append(files.fs.ukey(f.path))
             filepaths.append(f"{self.protocol_str}{f.path}")
 
-        keys_values = [
-            (ids[attrname][i] for attrname in self.attrnames) for i in range(len(ukeys))
-        ]
-        duplicates_keys_values = list(duplicates(keys_values))
-        assert len(duplicates_keys_values) == 0, (
-            f"Some files are duplitcated as indexes in filepaths: {duplicates_keys_values}. "
-            "Change the pattern or delete them."
-        )
-
         if len(ids) > 0:
             pseudo_data_df = pd.DataFrame.from_records(
                 {
                     **ids,
                     "ukey": ukeys,
                     **({"filepath": filepaths} if self.add_filepath_column else {}),
                 }
```

### Comparing `datapipe_core-0.13.7/datapipe/store/milvus.py` & `datapipe_core-0.13.9/datapipe/store/milvus.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.7/datapipe/store/pandas.py` & `datapipe_core-0.13.9/datapipe/store/pandas.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.7/datapipe/store/qdrant.py` & `datapipe_core-0.13.9/datapipe/store/qdrant.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.7/datapipe/store/redis.py` & `datapipe_core-0.13.9/datapipe/store/redis.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.7/datapipe/store/table_store.py` & `datapipe_core-0.13.9/datapipe/store/table_store.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.7/datapipe/types.py` & `datapipe_core-0.13.9/datapipe/types.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.7/pyproject.toml` & `datapipe_core-0.13.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datapipe-core"
-version = "0.13.7"
+version = "0.13.9"
 description = "`datapipe` is a realtime incremental ETL library for Python application"
 readme = "README.md"
 repository = "https://github.com/epoch8/datapipe"
 authors = ["Andrey Tatarinov <a@tatarinov.co>"]
 packages = [
     { include = "datapipe" }
 ]
```

### Comparing `datapipe_core-0.13.7/PKG-INFO` & `datapipe_core-0.13.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapipe-core
-Version: 0.13.7
+Version: 0.13.9
 Summary: `datapipe` is a realtime incremental ETL library for Python application
 Home-page: https://github.com/epoch8/datapipe
 Author: Andrey Tatarinov
 Author-email: a@tatarinov.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

