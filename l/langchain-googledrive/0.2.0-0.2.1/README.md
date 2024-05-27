# Comparing `tmp/langchain_googledrive-0.2.0.tar.gz` & `tmp/langchain_googledrive-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_googledrive-0.2.0.tar", max compression
+gzip compressed data, was "langchain_googledrive-0.2.1.tar", max compression
```

## Comparing `langchain_googledrive-0.2.0.tar` & `langchain_googledrive-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-09-29 15:31:57.756473 langchain_googledrive-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     1391 2024-03-12 07:53:57.458994 langchain_googledrive-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-09-05 14:03:36.513202 langchain_googledrive-0.2.0/langchain_googledrive/__init__.py
--rw-r--r--   0        0        0       84 2023-09-05 14:03:36.513202 langchain_googledrive-0.2.0/langchain_googledrive/document_loaders/__init__.py
--rw-r--r--   0        0        0    13362 2024-01-23 17:23:17.423814 langchain_googledrive-0.2.0/langchain_googledrive/document_loaders/google_drive.py
--rw-r--r--   0        0        0       90 2023-09-05 14:03:36.513202 langchain_googledrive-0.2.0/langchain_googledrive/retrievers/__init__.py
--rw-r--r--   0        0        0     2214 2024-01-23 17:23:17.423814 langchain_googledrive-0.2.0/langchain_googledrive/retrievers/google_drive.py
--rw-r--r--   0        0        0       97 2023-09-05 14:03:36.513202 langchain_googledrive-0.2.0/langchain_googledrive/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-09-05 14:03:36.513202 langchain_googledrive-0.2.0/langchain_googledrive/tools/google_drive/__init__.py
--rw-r--r--   0        0        0     1183 2024-01-23 17:23:17.423814 langchain_googledrive-0.2.0/langchain_googledrive/tools/google_drive/tool.py
--rw-r--r--   0        0        0      109 2023-09-05 14:03:36.513202 langchain_googledrive-0.2.0/langchain_googledrive/utilities/__init__.py
--rw-r--r--   0        0        0    77814 2024-05-21 10:34:08.671404 langchain_googledrive-0.2.0/langchain_googledrive/utilities/google_drive.py
--rw-r--r--   0        0        0     3376 2024-05-21 10:33:05.007999 langchain_googledrive-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2760 1970-01-01 00:00:00.000000 langchain_googledrive-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-09-29 15:31:57.756473 langchain_googledrive-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     1391 2024-03-12 07:53:57.458994 langchain_googledrive-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-09-05 14:03:36.513202 langchain_googledrive-0.2.1/langchain_googledrive/__init__.py
+-rw-r--r--   0        0        0       84 2023-09-05 14:03:36.513202 langchain_googledrive-0.2.1/langchain_googledrive/document_loaders/__init__.py
+-rw-r--r--   0        0        0    13362 2024-01-23 17:23:17.423814 langchain_googledrive-0.2.1/langchain_googledrive/document_loaders/google_drive.py
+-rw-r--r--   0        0        0       90 2023-09-05 14:03:36.513202 langchain_googledrive-0.2.1/langchain_googledrive/retrievers/__init__.py
+-rw-r--r--   0        0        0     2214 2024-01-23 17:23:17.423814 langchain_googledrive-0.2.1/langchain_googledrive/retrievers/google_drive.py
+-rw-r--r--   0        0        0       97 2023-09-05 14:03:36.513202 langchain_googledrive-0.2.1/langchain_googledrive/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-05 14:03:36.513202 langchain_googledrive-0.2.1/langchain_googledrive/tools/google_drive/__init__.py
+-rw-r--r--   0        0        0     1183 2024-01-23 17:23:17.423814 langchain_googledrive-0.2.1/langchain_googledrive/tools/google_drive/tool.py
+-rw-r--r--   0        0        0      109 2023-09-05 14:03:36.513202 langchain_googledrive-0.2.1/langchain_googledrive/utilities/__init__.py
+-rw-r--r--   0        0        0    77900 2024-05-27 08:43:53.120055 langchain_googledrive-0.2.1/langchain_googledrive/utilities/google_drive.py
+-rw-r--r--   0        0        0     2834 2024-05-27 09:15:36.201175 langchain_googledrive-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2412 1970-01-01 00:00:00.000000 langchain_googledrive-0.2.1/PKG-INFO
```

### Comparing `langchain_googledrive-0.2.0/LICENSE.txt` & `langchain_googledrive-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langchain_googledrive-0.2.0/README.md` & `langchain_googledrive-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `langchain_googledrive-0.2.0/langchain_googledrive/document_loaders/google_drive.py` & `langchain_googledrive-0.2.1/langchain_googledrive/document_loaders/google_drive.py`

 * *Files identical despite different names*

### Comparing `langchain_googledrive-0.2.0/langchain_googledrive/retrievers/google_drive.py` & `langchain_googledrive-0.2.1/langchain_googledrive/retrievers/google_drive.py`

 * *Files identical despite different names*

### Comparing `langchain_googledrive-0.2.0/langchain_googledrive/tools/google_drive/tool.py` & `langchain_googledrive-0.2.1/langchain_googledrive/tools/google_drive/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_googledrive-0.2.0/langchain_googledrive/utilities/google_drive.py` & `langchain_googledrive-0.2.1/langchain_googledrive/utilities/google_drive.py`

 * *Files 0% similar despite different names*

```diff
@@ -959,32 +959,32 @@
         from googleapiclient.http import MediaIoBaseDownload  # type: ignore
 
         suffix = mimetypes.guess_extension(file["mimeType"])
         if not suffix:
             suffix = Path(file["name"]).suffix
         if suffix not in self._not_supported:  # Already see this suffix?
             try:
-                with tempfile.NamedTemporaryFile(mode="w", suffix=suffix) as tf:
-                    path = tf.name
+                with tempfile.TemporaryDirectory() as temp_dir:
+                    unique_filename = str(uuid4()) + suffix
+                    path = os.path.join(temp_dir, unique_filename)
                     logger.debug(
                         f"Get '{file['name']}' with type "
                         f"'{file.get('mimeType', 'unknown')}'"
                     )
 
                     request = self.files.get_media(fileId=file["id"])
 
-                    fh = io.FileIO(path, mode="wb")
                     try:
-                        downloader = MediaIoBaseDownload(fh, request)
-                        done = False
-                        while done is False:
-                            status, done = downloader.next_chunk()
-
+                        with open(path, 'wb') as tf:
+                            downloader = MediaIoBaseDownload(tf, request)
+                            done = False
+                            while not done:
+                                status, done = downloader.next_chunk()
                     finally:
-                        fh.close()
+                        tf.close()
 
                     if self.file_loader_cls:
                         # Deprecated
                         request = self.files.get_media(fileId=file["id"])
                         bfh = io.BytesIO()
                         downloader = MediaIoBaseDownload(bfh, request)
                         done = False
```

### Comparing `langchain_googledrive-0.2.0/pyproject.toml` & `langchain_googledrive-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -6,28 +6,19 @@
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://www.github.com/pprados/langchain-googledrive"
 packages = [{ include = "langchain_googledrive" }]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-langchain_core = ">=0.2.0"
-langchain_community = ">=0.2.0"
+langchain_core = ">=0.2.1"
+langchain_community = ">=0.2.1"
 google-api-python-client = "^2.97"
 google-auth-httplib2 = ">=0.1"
 google-auth-oauthlib = ">=1.0"
-#pydantic = "^1.10.0"
-pdf2image = { version = "^1.16", optional = true }
-pypandoc_binary = { version = "^1.11", optional = true }
-torch = { version = ">=1,<3", optional = true }
-#detectron2 = { git = "https://github.com/facebookresearch/detectron2.git", optional = true }
-
-pytesseract = { version = "^0.3.10", optional = true }
-unstructured = { version = "^0.10.12", extras = ["local-inference"], optional = true }
-pytest = "^7.4.2"
 
 [tool.poetry.extras]
 all = [
     "pdf2image",
     "pypandoc_binary",
     "torch",
 #    "detectron2",
@@ -49,26 +40,20 @@
 [tool.poetry.group.test.dependencies]
 # The only dependencies that should be added are
 # dependencies used for running tests (e.g., pytest, freezegun, response).
 # Any dependencies that do not meet that criteria will be removed.
 pytest = "^7.3.0"
 pytest-cov = "^4.0.0"
 pytest-dotenv = "^0.5.2"
-duckdb = "^0.9.0"
 pytest-watcher = "^0.2.6"
-freezegun = "^1.2.2"
-responses = "^0.22.0"
 pytest-asyncio = "^0.20.3"
-lark = "^1.1.5"
-pandas = "^2.0.0"
 pytest-mock = "^3.10.0"
 pytest-socket = "^0.6.0"
-syrupy = "^4.0.2"
-unstructured = "^0.10.8"
 twine = "^4.0.0"
+langchain-openai = ">=0.1.7"
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 mypy = "^0.991"
 ruff = "^0.0.249"
```

### Comparing `langchain_googledrive-0.2.0/PKG-INFO` & `langchain_googledrive-0.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-googledrive
-Version: 0.2.0
+Version: 0.2.1
 Summary: This is a temporary project while I wait for my langchain [pull-request](https://github.com/hwchase17/langchain/pull/5135) to be validated.
 Home-page: https://www.github.com/pprados/langchain-googledrive
 License: Apache 2.0
 Author: Philippe PRADOS
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -12,22 +12,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
 Requires-Dist: google-api-python-client (>=2.97,<3.0)
 Requires-Dist: google-auth-httplib2 (>=0.1)
 Requires-Dist: google-auth-oauthlib (>=1.0)
-Requires-Dist: langchain_community (>=0.2.0)
-Requires-Dist: langchain_core (>=0.2.0)
-Requires-Dist: pdf2image (>=1.16,<2.0) ; extra == "all"
-Requires-Dist: pypandoc_binary (>=1.11,<2.0) ; extra == "all"
-Requires-Dist: pytesseract (>=0.3.10,<0.4.0) ; extra == "all"
-Requires-Dist: pytest (>=7.4.2,<8.0.0)
-Requires-Dist: torch (>=1,<3) ; extra == "all"
-Requires-Dist: unstructured[local-inference] (>=0.10.12,<0.11.0) ; extra == "all"
+Requires-Dist: langchain_community (>=0.2.1)
+Requires-Dist: langchain_core (>=0.2.1)
 Project-URL: Repository, https://www.github.com/pprados/langchain-googledrive
 Description-Content-Type: text/markdown
 
 This is a more advanced integration of Google Drive with langchain.
 
 # Install
 ```
```

