# Comparing `tmp/DjangoSharepointStorage-1.0.4.tar.gz` & `tmp/DjangoSharepointStorage-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DjangoSharepointStorage-1.0.4.tar", last modified: Wed May 22 08:28:31 2024, max compression
+gzip compressed data, was "DjangoSharepointStorage-1.0.5.tar", last modified: Mon May 27 19:33:48 2024, max compression
```

## Comparing `DjangoSharepointStorage-1.0.4.tar` & `DjangoSharepointStorage-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 melihsunbul   (501) staff       (20)        0 2024-05-22 08:28:31.517676 DjangoSharepointStorage-1.0.4/
-drwxr-xr-x   0 melihsunbul   (501) staff       (20)        0 2024-05-22 08:28:31.517340 DjangoSharepointStorage-1.0.4/DjangoSharepointStorage.egg-info/
--rw-r--r--   0 melihsunbul   (501) staff       (20)      613 2024-05-22 08:28:31.000000 DjangoSharepointStorage-1.0.4/DjangoSharepointStorage.egg-info/PKG-INFO
--rw-r--r--   0 melihsunbul   (501) staff       (20)      497 2024-05-22 08:28:31.000000 DjangoSharepointStorage-1.0.4/DjangoSharepointStorage.egg-info/SOURCES.txt
--rw-r--r--   0 melihsunbul   (501) staff       (20)        1 2024-05-22 08:28:31.000000 DjangoSharepointStorage-1.0.4/DjangoSharepointStorage.egg-info/dependency_links.txt
--rw-r--r--   0 melihsunbul   (501) staff       (20)       36 2024-05-22 08:28:31.000000 DjangoSharepointStorage-1.0.4/DjangoSharepointStorage.egg-info/requires.txt
--rw-r--r--   0 melihsunbul   (501) staff       (20)       26 2024-05-22 08:28:31.000000 DjangoSharepointStorage-1.0.4/DjangoSharepointStorage.egg-info/top_level.txt
--rw-r--r--   0 melihsunbul   (501) staff       (20)     1071 2023-11-09 16:23:47.000000 DjangoSharepointStorage-1.0.4/LICENSE.txt
--rw-r--r--   0 melihsunbul   (501) staff       (20)      613 2024-05-22 08:28:31.517509 DjangoSharepointStorage-1.0.4/PKG-INFO
--rw-r--r--   0 melihsunbul   (501) staff       (20)       34 2024-05-21 07:57:25.000000 DjangoSharepointStorage-1.0.4/README.md
-drwxr-xr-x   0 melihsunbul   (501) staff       (20)        0 2024-05-22 08:28:31.517202 DjangoSharepointStorage-1.0.4/django_sharepoint_storage/
--rw-r--r--   0 melihsunbul   (501) staff       (20)      493 2023-11-21 10:32:47.000000 DjangoSharepointStorage-1.0.4/django_sharepoint_storage/SharePointClients.py
--rw-r--r--   0 melihsunbul   (501) staff       (20)      592 2023-11-21 10:32:47.000000 DjangoSharepointStorage-1.0.4/django_sharepoint_storage/SharePointCloudStorageUtils.py
--rw-r--r--   0 melihsunbul   (501) staff       (20)      735 2023-11-16 09:06:38.000000 DjangoSharepointStorage-1.0.4/django_sharepoint_storage/SharePointFile.py
--rw-r--r--   0 melihsunbul   (501) staff       (20)     5167 2024-05-22 08:28:23.000000 DjangoSharepointStorage-1.0.4/django_sharepoint_storage/SharePointStorage.py
--rw-r--r--   0 melihsunbul   (501) staff       (20)        0 2023-10-30 10:29:18.000000 DjangoSharepointStorage-1.0.4/django_sharepoint_storage/__init__.py
--rw-r--r--   0 melihsunbul   (501) staff       (20)       38 2024-05-22 08:28:31.517724 DjangoSharepointStorage-1.0.4/setup.cfg
--rw-r--r--   0 melihsunbul   (501) staff       (20)      853 2024-05-22 08:28:23.000000 DjangoSharepointStorage-1.0.4/setup.py
+drwxr-xr-x   0 melihsunbul   (501) staff       (20)        0 2024-05-27 19:33:48.641785 DjangoSharepointStorage-1.0.5/
+drwxr-xr-x   0 melihsunbul   (501) staff       (20)        0 2024-05-27 19:33:48.641429 DjangoSharepointStorage-1.0.5/DjangoSharepointStorage.egg-info/
+-rw-r--r--   0 melihsunbul   (501) staff       (20)      613 2024-05-27 19:33:48.000000 DjangoSharepointStorage-1.0.5/DjangoSharepointStorage.egg-info/PKG-INFO
+-rw-r--r--   0 melihsunbul   (501) staff       (20)      497 2024-05-27 19:33:48.000000 DjangoSharepointStorage-1.0.5/DjangoSharepointStorage.egg-info/SOURCES.txt
+-rw-r--r--   0 melihsunbul   (501) staff       (20)        1 2024-05-27 19:33:48.000000 DjangoSharepointStorage-1.0.5/DjangoSharepointStorage.egg-info/dependency_links.txt
+-rw-r--r--   0 melihsunbul   (501) staff       (20)       36 2024-05-27 19:33:48.000000 DjangoSharepointStorage-1.0.5/DjangoSharepointStorage.egg-info/requires.txt
+-rw-r--r--   0 melihsunbul   (501) staff       (20)       26 2024-05-27 19:33:48.000000 DjangoSharepointStorage-1.0.5/DjangoSharepointStorage.egg-info/top_level.txt
+-rw-r--r--   0 melihsunbul   (501) staff       (20)     1071 2023-11-09 16:23:47.000000 DjangoSharepointStorage-1.0.5/LICENSE.txt
+-rw-r--r--   0 melihsunbul   (501) staff       (20)      613 2024-05-27 19:33:48.641609 DjangoSharepointStorage-1.0.5/PKG-INFO
+-rw-r--r--   0 melihsunbul   (501) staff       (20)       34 2024-05-27 19:30:48.000000 DjangoSharepointStorage-1.0.5/README.md
+drwxr-xr-x   0 melihsunbul   (501) staff       (20)        0 2024-05-27 19:33:48.641299 DjangoSharepointStorage-1.0.5/django_sharepoint_storage/
+-rw-r--r--   0 melihsunbul   (501) staff       (20)      592 2023-11-21 10:32:47.000000 DjangoSharepointStorage-1.0.5/django_sharepoint_storage/SharePointCloudStorageUtils.py
+-rw-r--r--   0 melihsunbul   (501) staff       (20)     1104 2024-05-27 19:31:26.000000 DjangoSharepointStorage-1.0.5/django_sharepoint_storage/SharePointContext.py
+-rw-r--r--   0 melihsunbul   (501) staff       (20)      735 2023-11-16 09:06:38.000000 DjangoSharepointStorage-1.0.5/django_sharepoint_storage/SharePointFile.py
+-rw-r--r--   0 melihsunbul   (501) staff       (20)     5938 2024-05-27 19:30:55.000000 DjangoSharepointStorage-1.0.5/django_sharepoint_storage/SharePointStorage.py
+-rw-r--r--   0 melihsunbul   (501) staff       (20)        0 2023-10-30 10:29:18.000000 DjangoSharepointStorage-1.0.5/django_sharepoint_storage/__init__.py
+-rw-r--r--   0 melihsunbul   (501) staff       (20)       38 2024-05-27 19:33:48.641826 DjangoSharepointStorage-1.0.5/setup.cfg
+-rw-r--r--   0 melihsunbul   (501) staff       (20)      853 2024-05-27 19:31:26.000000 DjangoSharepointStorage-1.0.5/setup.py
```

### Comparing `DjangoSharepointStorage-1.0.4/DjangoSharepointStorage.egg-info/PKG-INFO` & `DjangoSharepointStorage-1.0.5/DjangoSharepointStorage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DjangoSharepointStorage
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python library to use SharePoint as storage backend for your Django application
 Home-page: https://github.com/LundIT/DjangoSharepointStorage
 Author: Melih Sünbül
 Author-email: m.sunbul@lund-it.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DjangoSharepointStorage-1.0.4/LICENSE.txt` & `DjangoSharepointStorage-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DjangoSharepointStorage-1.0.4/PKG-INFO` & `DjangoSharepointStorage-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DjangoSharepointStorage
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python library to use SharePoint as storage backend for your Django application
 Home-page: https://github.com/LundIT/DjangoSharepointStorage
 Author: Melih Sünbül
 Author-email: m.sunbul@lund-it.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DjangoSharepointStorage-1.0.4/django_sharepoint_storage/SharePointCloudStorageUtils.py` & `DjangoSharepointStorage-1.0.5/django_sharepoint_storage/SharePointCloudStorageUtils.py`

 * *Files identical despite different names*

### Comparing `DjangoSharepointStorage-1.0.4/django_sharepoint_storage/SharePointFile.py` & `DjangoSharepointStorage-1.0.5/django_sharepoint_storage/SharePointFile.py`

 * *Files identical despite different names*

### Comparing `DjangoSharepointStorage-1.0.4/django_sharepoint_storage/SharePointStorage.py` & `DjangoSharepointStorage-1.0.5/django_sharepoint_storage/SharePointStorage.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import datetime
 import time
 from office365.sharepoint.files.file import File
 from io import BytesIO
 from django.conf import settings
 from django.db import connection
 
-from django_sharepoint_storage.SharePointClients import ctx, client_credentials
+from django_sharepoint_storage.SharePointContext import SharePointContext
 from django_sharepoint_storage.SharePointFile import SharePointFile
 
 DB_NAME = connection.settings_dict['NAME']
 class SharePointStorage(Storage):
     sharepoint_url = getattr(settings, 'SHAREPOINT_URL', 'sharepoint_url')
     client_id = getattr(settings, 'SHAREPOINT_APP_CLIENT_ID', 'client_id')
     client_secret = getattr(settings, 'SHAREPOINT_APP_CLIENT_SECRET', 'client_secret')
@@ -23,74 +23,93 @@
 
     @staticmethod
     def print_failure(retry_number, ex):
         print(f"{retry_number}: {ex}")
 
     def _open(self, name, mode='rb'):
         from django_sharepoint_storage.SharePointCloudStorageUtils import get_server_relative_path
+        
         if mode in ['r', 'rb']:
             file_url = self.url(name)
-            file = ctx.web.get_file_by_server_relative_path(get_server_relative_path(file_url)).execute_query_retry(max_retry=5, timeout_secs=5, failure_callback=SharePointStorage.print_failure)
-            binary_file = file.open_binary(ctx, get_server_relative_path(file_url))
+            shrp_ctx = SharePointContext()
+            file = shrp_ctx.ctx.web.get_file_by_server_relative_path(get_server_relative_path(file_url)).execute_query_retry(max_retry=5, timeout_secs=5, failure_callback=SharePointStorage.print_failure)
+            binary_file = file.open_binary(shrp_ctx.ctx, get_server_relative_path(file_url))
             bytesio_object = BytesIO(binary_file.content)
             return bytesio_object
         elif mode in ['w', 'wb']:
             return SharePointFile(name, mode, self)
         else:
             raise ValueError(f"Unsupported file mode: {mode}")
 
     def _save(self, name, content):
-        # Here, name will have the format 'upload_to/filename.ext'
+        shrp_ctx = SharePointContext()
         folder_path = f"Shared Documents/{os.getenv('DEPLOYMENT_ENVIRONMENT', 'LOCAL')}-{os.getenv('K8S_NAMESPACE', 'ENV')}/{os.getenv('KEYCLOAK_INTERNAL_CLIENT_ID', 'Local')}/{os.getenv('INSTANCE_RESOURCE_IDENTIFIER', f'{platform.node()}/{DB_NAME}')}/{self.location}/{os.path.dirname(name)}"
-        target_folder = ctx.web.ensure_folder_path(folder_path).get().select(["ServerRelativePath"]).execute_query_retry(max_retry=5, timeout_secs=5, failure_callback=SharePointStorage.print_failure)
+        target_folder = shrp_ctx.ctx.web.ensure_folder_path(folder_path).get().select(["ServerRelativePath"]).execute_query_retry(max_retry=5, timeout_secs=5, failure_callback=SharePointStorage.print_failure)
         content.seek(0)
         file_content = content.read()
 
         target_folder.upload_file(os.path.basename(name), file_content).execute_query_retry(max_retry=5, timeout_secs=5, failure_callback=SharePointStorage.print_failure)
 
         return name
 
     def delete(self, name):
         from django_sharepoint_storage.SharePointCloudStorageUtils import get_server_relative_path
 
+        shrp_ctx = SharePointContext()
+        
         file_path = get_server_relative_path(self.url(name))
-        file = ctx.web.get_file_by_server_relative_path(file_path).get().execute_query_retry(max_retry=5,
-                                                                                             timeout_secs=5,
-                                                                                             failure_callback=SharePointStorage.print_failure)
-        file.delete_object().execute_query_retry(max_retry=5, timeout_secs=5,
-                                                 failure_callback=SharePointStorage.print_failure)
+        file = shrp_ctx.ctx.web.get_file_by_server_relative_path(file_path).get().execute_query_retry(max_retry=5, timeout_secs=5, failure_callback=SharePointStorage.print_failure)
+        file.delete_object().execute_query_retry(max_retry=5, timeout_secs=5, failure_callback=SharePointStorage.print_failure)
 
     def exists(self, name, retries=5):
         from django_sharepoint_storage.SharePointCloudStorageUtils import get_server_relative_path
 
         file_path = get_server_relative_path(self.url(name))
 
+        shrp_ctx = SharePointContext()
+
         if retries <= 0:
             raise Exception("SharePoint Server cannot handle requests at the moment.")
         try:
             if name.endswith('/'):
-                file = ctx.web.get_folder_by_server_relative_path(file_path[:-1]).get().execute_query()
+                file = shrp_ctx.ctx.web.get_folder_by_server_relative_path(file_path[:-1]).get().execute_query()
             else:
-                file = ctx.web.get_file_by_server_relative_path(file_path).get().execute_query()
+                file = shrp_ctx.ctx.web.get_file_by_server_relative_path(file_path).get().execute_query()
         except Exception as ex:
             if ex.response.status_code == 404:
                 return False
             time.sleep(5)
             return self.exists(name, retries - 1)
 
         return True
 
     def get_modified_time(self, name):
         from django_sharepoint_storage.SharePointCloudStorageUtils import get_server_relative_path
 
         file_path = get_server_relative_path(self.url(name))
 
+        shrp_ctx = SharePointContext()
+
         if name.endswith('/'):
-            file = ctx.web.get_folder_by_server_relative_path(file_path[:-1]).get().expand(["TimeLastModified"]).get().execute_query_retry(max_retry=5, timeout_secs=5, failure_callback=SharePointStorage.print_failure)
+            file = shrp_ctx.ctx.web.get_folder_by_server_relative_path(file_path[:-1]).get().expand(["TimeLastModified"]).get().execute_query_retry(max_retry=5, timeout_secs=5, failure_callback=SharePointStorage.print_failure)
         else:
-            file = ctx.web.get_file_by_server_relative_path(file_path).get().expand(["TimeLastModified"]).get().execute_query_retry(max_retry=5, timeout_secs=5, failure_callback=SharePointStorage.print_failure)
+            file = shrp_ctx.ctx.web.get_file_by_server_relative_path(file_path).get().expand(["TimeLastModified"]).get().execute_query_retry(max_retry=5, timeout_secs=5, failure_callback=SharePointStorage.print_failure)
 
         return datetime.datetime.timestamp(file.time_last_modified)
 
+    def listdir(self, name):
+        from django_sharepoint_storage.SharePointCloudStorageUtils import get_server_relative_path
+
+        shrp_ctx = SharePointContext()
+        
+        folder_path = get_server_relative_path(self.url(name))
+        if name.endswith('/'):
+            target_folder_url = folder_path[:-1]
+
+        root_folder = shrp_ctx.ctx.web.get_folder_by_server_relative_path(target_folder_url).execute_query()
+        folders = root_folder.get_folders(True).execute_query_retry(max_retry=5, timeout_secs=5, failure_callback=SharePointStorage.print_failure)
+        files = root_folder.get_files(True).execute_query_retry(max_retry=5, timeout_secs=5, failure_callback=SharePointStorage.print_failure)
+        return [f.name for f in files], [f.name for f in folders]
+
     def url(self, name):
         # Use the dirname of name as your upload_to equivalent
-        return f"{self.sharepoint_url}/Shared Documents/{os.getenv('DEPLOYMENT_ENVIRONMENT', 'LOCAL')}-{os.getenv('K8S_NAMESPACE', 'ENV')}/{os.getenv('KEYCLOAK_INTERNAL_CLIENT_ID', 'Local')}/{os.getenv('INSTANCE_RESOURCE_IDENTIFIER', f'{platform.node()}/{DB_NAME}')}/{self.location}/{name}"
+        return f"{self.sharepoint_url}/Shared Documents/{os.getenv('DEPLOYMENT_ENVIRONMENT', 'LOCAL')}-{os.getenv('K8S_NAMESPACE', 'ENV')}/{os.getenv('KEYCLOAK_INTERNAL_CLIENT_ID', 'Local')}/{os.getenv('INSTANCE_RESOURCE_IDENTIFIER', f'{platform.node()}/{DB_NAME}')}/{self.location}/{name}"
```

### Comparing `DjangoSharepointStorage-1.0.4/setup.py` & `DjangoSharepointStorage-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="DjangoSharepointStorage",
-    version="1.0.4",
+    version="1.0.5",
     author="Melih Sünbül",
     author_email="m.sunbul@lund-it.com",
     description="A Python library to use SharePoint as storage backend for your Django application",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LundIT/DjangoSharepointStorage",
     packages=find_packages(),
```

