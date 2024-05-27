# Comparing `tmp/bergmann-0.0.0.tar.gz` & `tmp/bergmann-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bergmann-0.0.0.tar", max compression
+gzip compressed data, was "bergmann-0.0.1.tar", max compression
```

## Comparing `bergmann-0.0.0.tar` & `bergmann-0.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0        0 2024-05-18 12:52:48.721725 bergmann-0.0.0/bergmann/__init__.py
--rw-r--r--   0        0        0     1976 2024-05-26 20:21:46.156882 bergmann-0.0.0/bergmann/app.py
--rw-r--r--   0        0        0      731 2024-05-26 13:58:21.110133 bergmann-0.0.0/bergmann/bergmann.tcss
--rw-r--r--   0        0        0       43 2024-05-22 06:35:43.989359 bergmann-0.0.0/bergmann/common/__init__.py
--rw-r--r--   0        0        0      148 2024-05-22 06:35:41.595793 bergmann-0.0.0/bergmann/common/logger.py
--rw-r--r--   0        0        0      402 2024-05-26 20:23:14.282739 bergmann-0.0.0/bergmann/common/ru_keys.py
--rw-r--r--   0        0        0      242 2024-05-25 20:35:07.309684 bergmann-0.0.0/bergmann/convention.py
--rw-r--r--   0        0        0        0 2024-05-25 12:02:16.855189 bergmann-0.0.0/bergmann/crypto/__init__.py
--rw-r--r--   0        0        0     2339 2024-05-26 20:29:18.474882 bergmann-0.0.0/bergmann/crypto/kuzcypher.py
--rw-r--r--   0        0        0      543 2024-05-25 20:56:51.960256 bergmann-0.0.0/bergmann/di.py
--rw-r--r--   0        0        0        0 2024-05-25 20:28:39.226320 bergmann-0.0.0/bergmann/entities/__init__.py
--rw-r--r--   0        0        0     1503 2024-05-26 09:59:05.700116 bergmann-0.0.0/bergmann/entities/db_meta.py
--rw-r--r--   0        0        0      294 2024-05-25 20:30:02.258601 bergmann-0.0.0/bergmann/entities/encrypted_item.py
--rw-r--r--   0        0        0      554 2024-05-26 10:43:22.376604 bergmann-0.0.0/bergmann/entities/item.py
--rw-r--r--   0        0        0      160 2024-05-25 20:56:39.170139 bergmann-0.0.0/bergmann/failures_presenter.py
--rw-r--r--   0        0        0      669 2024-05-23 17:31:09.586496 bergmann-0.0.0/bergmann/file_db_helper.py
--rw-r--r--   0        0        0      365 2024-05-26 10:27:35.146538 bergmann-0.0.0/bergmann/key.py
--rw-r--r--   0        0        0      141 2024-05-18 14:02:04.376373 bergmann-0.0.0/bergmann/main.py
--rw-r--r--   0        0        0     6142 2024-05-26 20:28:20.240117 bergmann-0.0.0/bergmann/passwords_interactor.py
--rw-r--r--   0        0        0        0 2024-05-20 20:13:18.527883 bergmann-0.0.0/bergmann/validators/__init__.py
--rw-r--r--   0        0        0      290 2024-05-20 20:19:20.594943 bergmann-0.0.0/bergmann/validators/bmn_filename_validator.py
--rw-r--r--   0        0        0      297 2024-05-20 20:19:20.594943 bergmann-0.0.0/bergmann/validators/file_already_exists_validator.py
--rw-r--r--   0        0        0        0 2024-05-18 15:11:59.912197 bergmann-0.0.0/bergmann/widgets/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 06:39:29.413504 bergmann-0.0.0/bergmann/widgets/passwords_modal/__init__.py
--rw-r--r--   0        0        0     4339 2024-05-26 13:03:46.311855 bergmann-0.0.0/bergmann/widgets/passwords_modal/initialize_new_db_modal.py
--rw-r--r--   0        0        0     4538 2024-05-26 20:29:33.584953 bergmann-0.0.0/bergmann/widgets/passwords_modal/load_db_modal.py
--rw-r--r--   0        0        0     8681 2024-05-26 20:27:20.432783 bergmann-0.0.0/bergmann/widgets/passwords_modal/passwords_explorer.py
--rw-r--r--   0        0        0        0 2024-05-21 19:09:06.210254 bergmann-0.0.0/bergmann/widgets/select_file_modal/__init__.py
--rw-r--r--   0        0        0      824 2024-05-22 06:36:47.034082 bergmann-0.0.0/bergmann/widgets/select_file_modal/bmn_filtered_directory_tree.py
--rw-r--r--   0        0        0     2472 2024-05-25 20:58:52.355228 bergmann-0.0.0/bergmann/widgets/select_file_modal/create_file_modal.py
--rw-r--r--   0        0        0     2239 2024-05-22 20:04:24.217620 bergmann-0.0.0/bergmann/widgets/select_file_modal/select_file_header.py
--rw-r--r--   0        0        0     3508 2024-05-26 20:21:46.159884 bergmann-0.0.0/bergmann/widgets/select_file_modal/select_file_modal.py
--rw-r--r--   0        0        0      642 2024-05-22 19:50:41.465429 bergmann-0.0.0/bergmann/widgets/welcome.py
--rw-r--r--   0        0        0     1098 2024-05-18 12:33:01.482303 bergmann-0.0.0/LICENSE
--rw-r--r--   0        0        0      915 2024-05-26 10:52:12.082975 bergmann-0.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-18 13:59:46.985035 bergmann-0.0.0/README.md
--rw-r--r--   0        0        0      430 1970-01-01 00:00:00.000000 bergmann-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-18 12:52:48.721725 bergmann-0.0.1/bergmann/__init__.py
+-rw-r--r--   0        0        0     2201 2024-05-27 17:40:15.917021 bergmann-0.0.1/bergmann/app.py
+-rw-r--r--   0        0        0      731 2024-05-26 13:58:21.110133 bergmann-0.0.1/bergmann/bergmann.tcss
+-rw-r--r--   0        0        0       43 2024-05-22 06:35:43.989359 bergmann-0.0.1/bergmann/common/__init__.py
+-rw-r--r--   0        0        0      148 2024-05-22 06:35:41.595793 bergmann-0.0.1/bergmann/common/logger.py
+-rw-r--r--   0        0        0      402 2024-05-26 20:23:14.282739 bergmann-0.0.1/bergmann/common/ru_keys.py
+-rw-r--r--   0        0        0      242 2024-05-25 20:35:07.309684 bergmann-0.0.1/bergmann/convention.py
+-rw-r--r--   0        0        0        0 2024-05-25 12:02:16.855189 bergmann-0.0.1/bergmann/crypto/__init__.py
+-rw-r--r--   0        0        0     2339 2024-05-26 20:29:18.474882 bergmann-0.0.1/bergmann/crypto/kuzcypher.py
+-rw-r--r--   0        0        0      543 2024-05-25 20:56:51.960256 bergmann-0.0.1/bergmann/di.py
+-rw-r--r--   0        0        0        0 2024-05-25 20:28:39.226320 bergmann-0.0.1/bergmann/entities/__init__.py
+-rw-r--r--   0        0        0     1503 2024-05-26 09:59:05.700116 bergmann-0.0.1/bergmann/entities/db_meta.py
+-rw-r--r--   0        0        0      294 2024-05-25 20:30:02.258601 bergmann-0.0.1/bergmann/entities/encrypted_item.py
+-rw-r--r--   0        0        0      554 2024-05-26 10:43:22.376604 bergmann-0.0.1/bergmann/entities/item.py
+-rw-r--r--   0        0        0      160 2024-05-25 20:56:39.170139 bergmann-0.0.1/bergmann/failures_presenter.py
+-rw-r--r--   0        0        0      669 2024-05-23 17:31:09.586496 bergmann-0.0.1/bergmann/file_db_helper.py
+-rw-r--r--   0        0        0      365 2024-05-26 10:27:35.146538 bergmann-0.0.1/bergmann/key.py
+-rw-r--r--   0        0        0      376 2024-05-27 17:41:03.042521 bergmann-0.0.1/bergmann/main.py
+-rw-r--r--   0        0        0     6142 2024-05-26 20:28:20.240117 bergmann-0.0.1/bergmann/passwords_interactor.py
+-rw-r--r--   0        0        0        0 2024-05-20 20:13:18.527883 bergmann-0.0.1/bergmann/validators/__init__.py
+-rw-r--r--   0        0        0      290 2024-05-20 20:19:20.594943 bergmann-0.0.1/bergmann/validators/bmn_filename_validator.py
+-rw-r--r--   0        0        0      297 2024-05-20 20:19:20.594943 bergmann-0.0.1/bergmann/validators/file_already_exists_validator.py
+-rw-r--r--   0        0        0        0 2024-05-18 15:11:59.912197 bergmann-0.0.1/bergmann/widgets/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 06:39:29.413504 bergmann-0.0.1/bergmann/widgets/passwords_modal/__init__.py
+-rw-r--r--   0        0        0     4339 2024-05-26 13:03:46.311855 bergmann-0.0.1/bergmann/widgets/passwords_modal/initialize_new_db_modal.py
+-rw-r--r--   0        0        0     4538 2024-05-26 20:29:33.584953 bergmann-0.0.1/bergmann/widgets/passwords_modal/load_db_modal.py
+-rw-r--r--   0        0        0     8681 2024-05-26 20:27:20.432783 bergmann-0.0.1/bergmann/widgets/passwords_modal/passwords_explorer.py
+-rw-r--r--   0        0        0        0 2024-05-21 19:09:06.210254 bergmann-0.0.1/bergmann/widgets/select_file_modal/__init__.py
+-rw-r--r--   0        0        0      824 2024-05-22 06:36:47.034082 bergmann-0.0.1/bergmann/widgets/select_file_modal/bmn_filtered_directory_tree.py
+-rw-r--r--   0        0        0     2472 2024-05-25 20:58:52.355228 bergmann-0.0.1/bergmann/widgets/select_file_modal/create_file_modal.py
+-rw-r--r--   0        0        0     2239 2024-05-22 20:04:24.217620 bergmann-0.0.1/bergmann/widgets/select_file_modal/select_file_header.py
+-rw-r--r--   0        0        0     3508 2024-05-26 20:21:46.159884 bergmann-0.0.1/bergmann/widgets/select_file_modal/select_file_modal.py
+-rw-r--r--   0        0        0      642 2024-05-22 19:50:41.465429 bergmann-0.0.1/bergmann/widgets/welcome.py
+-rw-r--r--   0        0        0     1098 2024-05-18 12:33:01.482303 bergmann-0.0.1/LICENSE
+-rw-r--r--   0        0        0      915 2024-05-27 17:41:20.555821 bergmann-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-18 13:59:46.985035 bergmann-0.0.1/README.md
+-rw-r--r--   0        0        0      430 1970-01-01 00:00:00.000000 bergmann-0.0.1/PKG-INFO
```

### Comparing `bergmann-0.0.0/bergmann/app.py` & `bergmann-0.0.1/bergmann/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,22 +18,29 @@
 class Bergmann(App[None]):
     BINDINGS = [
         Binding(key="f", action="select_file", description="Select passwords file"),
         Binding(key=RU_KEY_FOR_EN__F, action="select_file", show=False),
     ]
     CSS_PATH = "bergmann.tcss"
 
-    def __init__(self):
+    def __init__(self, debug: bool):
         super().__init__()
         self._file_db_helper = FileDBHelper()
         self._passwords_interactor = di.passwords_interactor
+        self._debug = debug
+
+    def _handle_exception(self, error: Exception) -> None:
+        if not self._debug:
+            raise error
+        super()._handle_exception(error)
 
     def compose(self) -> ComposeResult:
         yield WelcomeWidget(select_source_binding="f")
         yield Footer()
+        raise Exception
 
     @work
     async def action_select_file(self) -> None:
         path = await self.app.push_screen_wait(SelectFileModal())
         if path is None:
             self.notify("file not selected", severity="warning")
             return
```

### Comparing `bergmann-0.0.0/bergmann/bergmann.tcss` & `bergmann-0.0.1/bergmann/bergmann.tcss`

 * *Files identical despite different names*

### Comparing `bergmann-0.0.0/bergmann/crypto/kuzcypher.py` & `bergmann-0.0.1/bergmann/crypto/kuzcypher.py`

 * *Files identical despite different names*

### Comparing `bergmann-0.0.0/bergmann/di.py` & `bergmann-0.0.1/bergmann/di.py`

 * *Files identical despite different names*

### Comparing `bergmann-0.0.0/bergmann/entities/db_meta.py` & `bergmann-0.0.1/bergmann/entities/db_meta.py`

 * *Files identical despite different names*

### Comparing `bergmann-0.0.0/bergmann/entities/item.py` & `bergmann-0.0.1/bergmann/entities/item.py`

 * *Files identical despite different names*

### Comparing `bergmann-0.0.0/bergmann/file_db_helper.py` & `bergmann-0.0.1/bergmann/file_db_helper.py`

 * *Files identical despite different names*

### Comparing `bergmann-0.0.0/bergmann/passwords_interactor.py` & `bergmann-0.0.1/bergmann/passwords_interactor.py`

 * *Files identical despite different names*

### Comparing `bergmann-0.0.0/bergmann/widgets/passwords_modal/initialize_new_db_modal.py` & `bergmann-0.0.1/bergmann/widgets/passwords_modal/initialize_new_db_modal.py`

 * *Files identical despite different names*

### Comparing `bergmann-0.0.0/bergmann/widgets/passwords_modal/load_db_modal.py` & `bergmann-0.0.1/bergmann/widgets/passwords_modal/load_db_modal.py`

 * *Files identical despite different names*

### Comparing `bergmann-0.0.0/bergmann/widgets/passwords_modal/passwords_explorer.py` & `bergmann-0.0.1/bergmann/widgets/passwords_modal/passwords_explorer.py`

 * *Files identical despite different names*

### Comparing `bergmann-0.0.0/bergmann/widgets/select_file_modal/bmn_filtered_directory_tree.py` & `bergmann-0.0.1/bergmann/widgets/select_file_modal/bmn_filtered_directory_tree.py`

 * *Files identical despite different names*

### Comparing `bergmann-0.0.0/bergmann/widgets/select_file_modal/create_file_modal.py` & `bergmann-0.0.1/bergmann/widgets/select_file_modal/create_file_modal.py`

 * *Files identical despite different names*

### Comparing `bergmann-0.0.0/bergmann/widgets/select_file_modal/select_file_header.py` & `bergmann-0.0.1/bergmann/widgets/select_file_modal/select_file_header.py`

 * *Files identical despite different names*

### Comparing `bergmann-0.0.0/bergmann/widgets/select_file_modal/select_file_modal.py` & `bergmann-0.0.1/bergmann/widgets/select_file_modal/select_file_modal.py`

 * *Files identical despite different names*

### Comparing `bergmann-0.0.0/bergmann/widgets/welcome.py` & `bergmann-0.0.1/bergmann/widgets/welcome.py`

 * *Files identical despite different names*

### Comparing `bergmann-0.0.0/LICENSE` & `bergmann-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bergmann-0.0.0/pyproject.toml` & `bergmann-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bergmann"
-version = "0.0.0"
+version = "0.0.1"
 description = "Password manager"
 authors = ["Sviatoslav Bobryshev <wstswsb@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 bergmann = "bergmann.main:main"
```

