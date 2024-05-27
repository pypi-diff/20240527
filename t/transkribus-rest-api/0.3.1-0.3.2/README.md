# Comparing `tmp/transkribus_rest_api-0.3.1.tar.gz` & `tmp/transkribus_rest_api-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transkribus_rest_api-0.3.1.tar", last modified: Fri May 17 08:13:49 2024, max compression
+gzip compressed data, was "transkribus_rest_api-0.3.2.tar", last modified: Mon May 27 15:27:06 2024, max compression
```

## Comparing `transkribus_rest_api-0.3.1.tar` & `transkribus_rest_api-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:13:49.329691 transkribus_rest_api-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-17 08:13:35.000000 transkribus_rest_api-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-17 08:13:49.329691 transkribus_rest_api-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-17 08:13:35.000000 transkribus_rest_api-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-17 08:13:35.000000 transkribus_rest_api-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-17 08:13:35.000000 transkribus_rest_api-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 08:13:49.329691 transkribus_rest_api-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:13:49.325691 transkribus_rest_api-0.3.1/transkribus_rest_api/
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-17 08:13:35.000000 transkribus_rest_api-0.3.1/transkribus_rest_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-05-17 08:13:35.000000 transkribus_rest_api-0.3.1/transkribus_rest_api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-17 08:13:35.000000 transkribus_rest_api-0.3.1/transkribus_rest_api/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-17 08:13:35.000000 transkribus_rest_api-0.3.1/transkribus_rest_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:13:49.329691 transkribus_rest_api-0.3.1/transkribus_rest_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-17 08:13:49.000000 transkribus_rest_api-0.3.1/transkribus_rest_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-17 08:13:49.000000 transkribus_rest_api-0.3.1/transkribus_rest_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 08:13:49.000000 transkribus_rest_api-0.3.1/transkribus_rest_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-17 08:13:49.000000 transkribus_rest_api-0.3.1/transkribus_rest_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-17 08:13:49.000000 transkribus_rest_api-0.3.1/transkribus_rest_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:27:06.712866 transkribus_rest_api-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 15:26:55.000000 transkribus_rest_api-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-27 15:27:06.712866 transkribus_rest_api-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-27 15:26:55.000000 transkribus_rest_api-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-27 15:26:55.000000 transkribus_rest_api-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-27 15:26:55.000000 transkribus_rest_api-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 15:27:06.712866 transkribus_rest_api-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:27:06.708866 transkribus_rest_api-0.3.2/transkribus_rest_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-27 15:26:55.000000 transkribus_rest_api-0.3.2/transkribus_rest_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17773 2024-05-27 15:26:55.000000 transkribus_rest_api-0.3.2/transkribus_rest_api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-27 15:26:55.000000 transkribus_rest_api-0.3.2/transkribus_rest_api/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-27 15:26:55.000000 transkribus_rest_api-0.3.2/transkribus_rest_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:27:06.712866 transkribus_rest_api-0.3.2/transkribus_rest_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-27 15:27:06.000000 transkribus_rest_api-0.3.2/transkribus_rest_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-27 15:27:06.000000 transkribus_rest_api-0.3.2/transkribus_rest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 15:27:06.000000 transkribus_rest_api-0.3.2/transkribus_rest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-27 15:27:06.000000 transkribus_rest_api-0.3.2/transkribus_rest_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 15:27:06.000000 transkribus_rest_api-0.3.2/transkribus_rest_api.egg-info/top_level.txt
```

### Comparing `transkribus_rest_api-0.3.1/LICENSE` & `transkribus_rest_api-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `transkribus_rest_api-0.3.1/PKG-INFO` & `transkribus_rest_api-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transkribus_rest_api
-Version: 0.3.1
+Version: 0.3.2
 Summary: Transkribus Metagrapho API Client.
 Author-email: "J. Nathanael Philipp" <nathanael@philipp.land>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/jnphilipp/transkribus_rest_api
 Project-URL: Bug Tracker, http://github.com/jnphilipp/transkribus_rest_api/issues
 Keywords: transkribus,api
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `transkribus_rest_api-0.3.1/pyproject.toml` & `transkribus_rest_api-0.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "transkribus_rest_api"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
     {name = "J. Nathanael Philipp", email = "nathanael@philipp.land"}
 ]
 description="Transkribus Metagrapho API Client."
 readme = "README.md"
 license = {text = "GPLv3+"}
 requires-python = ">=3.10"
```

### Comparing `transkribus_rest_api-0.3.1/transkribus_rest_api/__init__.py` & `transkribus_rest_api-0.3.2/transkribus_rest_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 __all__ = ["TranskribusRestApi", "transkribus_rest_api"]
 
 __app_name__ = "transkribus-rest-api"
 __author__ = "J. Nathanael Philipp"
 __email__ = "nathanael@philipp.land"
 __copyright__ = "Copyright 2024 J. Nathanael Philipp (jnphilipp)"
 __license__ = "GPLv3"
-__version_info__ = (0, 3, 1)
+__version_info__ = (0, 3, 2)
 __version__ = ".".join(str(e) for e in __version_info__)
 __github__ = "https://github.com/jnphilipp/transkribus-rest-api"
 VERSION = (
     f"%(prog)s v{__version__}\n{__copyright__}\n"
     + "License GPLv3+: GNU GPL version 3 or later <https://gnu.org/licenses/gpl.html>."
     + "\nThis is free software: you are free to change and redistribute it.\n"
     + "There is NO WARRANTY, to the extent permitted by law.\n\n"
```

### Comparing `transkribus_rest_api-0.3.1/transkribus_rest_api/api.py` & `transkribus_rest_api-0.3.2/transkribus_rest_api/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -259,14 +259,79 @@
                     "nValues": n_values,
                     "sortColumn": sort_column,
                     "sortDirection": sort_direction,
                     "isDeleted": is_deleted,
                 },
             ).json()
 
+    class Job:
+        """Group all job requests together."""
+
+        def __init__(self, api: "TranskribusRestApi"):
+            """Create a new job.
+
+            Args:
+             * api: transkribus rest api
+            """
+            self.api = api
+
+        def get_jobs(
+            self,
+            user_id: int | None = None,
+            filter_by_user: bool | None = None,
+            status: str | None = None,
+            collection_id: int | None = None,
+            job_id: int | None = None,
+            type: str | None = None,
+            job_impl: str | None = None,
+            index: int = 0,
+            n_values: int = 50,
+            sort_column: str | None = None,
+            sort_direction: str | None = None,
+        ):
+            """List jobs.
+
+            Args:
+             * user_id
+             * filter_by_user
+             * status
+             * collection_id
+             * job_id
+             * type
+             * job_impl
+             * index: default 0
+             * n_values: default 50
+             * sort_column
+             * sort_direction
+            """
+            return self.api._get(
+                "jobs/list",
+                params={
+                    "userid": user_id,
+                    "filterByUser": filter_by_user,
+                    "status": status,
+                    "collId": collection_id,
+                    "id": job_id,
+                    "type": type,
+                    "jobImpl": job_impl,
+                    "index": index,
+                    "nValues": n_values,
+                    "sortColumn": sort_column,
+                    "sortDirection": sort_direction,
+                },
+            ).json()
+
+        def get_job_by_id(self, job_id: int | str) -> dict:
+            """Get a job by ID.
+
+            Args:
+             * job_id: job ID
+            """
+            return self.api._get(f"jobs/{job_id}").json()
+
     class Uploads:
         """Group all uploads requests together."""
 
         def __init__(self, api: "TranskribusRestApi"):
             """Create a new uploads.
 
             Args:
@@ -300,14 +365,22 @@
             """
             return parse_xml(
                 self.api._post(
                     "uploads", params={"collId": collection_id}, json=json
                 ).content
             )
 
+        def get_status(self, upload_id: int) -> dict:
+            """Get status.
+
+            Args:
+             * upload_id
+            """
+            return self.api._get(f"uploads/{upload_id}").json()
+
         def upload_page(
             self,
             upload_id: int,
             image: str | Path,
             xml: str | Path | None = None,
         ) -> None:
             """Upload a single page.
@@ -326,14 +399,15 @@
                     xml = Path(xml)
                 files["xml"] = (xml.name, open(xml, "rb"), "application/octet-stream")
             self.api._put(f"uploads/{upload_id}", files=files)
 
     def __init__(self, username: str, password: str):
         """Init."""
         self.collections = TranskribusRestApi.Collections(self)
+        self.job = TranskribusRestApi.Job(self)
         self.session_id = TranskribusRestApi.SessionId.login(username, password)
         self.uploads = TranskribusRestApi.Uploads(self)
 
     def _get(self, path: str, params: dict = {}) -> requests.models.Response:
         r = requests.get(
             f"{self.BASE_URL}/{path}",
             headers=self.session_id.get_auth_header(),
@@ -415,15 +489,16 @@
         }
 
         doc = self.uploads.create_upload_doc_structure(collection_id, data)
         upload_id = int(doc.xpath("//uploadId/text()")[0])
 
         for page in pages:
             self.uploads.upload_page(upload_id, page.image, page.page_xml)
-        return int(doc.xpath("//docId/text()")[0])
+        job_id = self.uploads.get_status(upload_id)["jobId"]
+        return self.job.get_job_by_id(job_id)["docId"]
 
     def download_document(
         self,
         collection_id: int,
         document_id: int,
         target: str | Path,
     ) -> None:
```

### Comparing `transkribus_rest_api-0.3.1/transkribus_rest_api/types.py` & `transkribus_rest_api-0.3.2/transkribus_rest_api/types.py`

 * *Files identical despite different names*

### Comparing `transkribus_rest_api-0.3.1/transkribus_rest_api/utils.py` & `transkribus_rest_api-0.3.2/transkribus_rest_api/utils.py`

 * *Files identical despite different names*

### Comparing `transkribus_rest_api-0.3.1/transkribus_rest_api.egg-info/PKG-INFO` & `transkribus_rest_api-0.3.2/transkribus_rest_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transkribus_rest_api
-Version: 0.3.1
+Version: 0.3.2
 Summary: Transkribus Metagrapho API Client.
 Author-email: "J. Nathanael Philipp" <nathanael@philipp.land>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/jnphilipp/transkribus_rest_api
 Project-URL: Bug Tracker, http://github.com/jnphilipp/transkribus_rest_api/issues
 Keywords: transkribus,api
 Classifier: Development Status :: 5 - Production/Stable
```

