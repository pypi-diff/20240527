# Comparing `tmp/hstream-0.1.54.tar.gz` & `tmp/hstream-0.1.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hstream-0.1.54.tar", max compression
+gzip compressed data, was "hstream-0.1.55.tar", max compression
```

## Comparing `hstream-0.1.54.tar` & `hstream-0.1.55.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1927 2024-05-26 13:11:50.976442 hstream-0.1.54/README.md
--rw-r--r--   0        0        0       53 2024-05-26 13:11:50.984442 hstream-0.1.54/hstream/__init__.py
--rw-r--r--   0        0        0       66 2024-05-26 13:11:50.984442 hstream-0.1.54/hstream/__main__.py
--rw-r--r--   0        0        0     3522 2024-05-26 13:11:50.984442 hstream-0.1.54/hstream/cli.py
--rw-r--r--   0        0        0    19076 2024-05-26 13:11:50.984442 hstream-0.1.54/hstream/components/components.py
--rw-r--r--   0        0        0     4625 2024-05-26 13:11:50.984442 hstream-0.1.54/hstream/components/styling_components.py
--rw-r--r--   0        0        0        0 2024-05-26 13:11:50.984442 hstream-0.1.54/hstream/django_server/hs/__init__.py
--rw-r--r--   0        0        0      136 2024-05-26 13:11:50.984442 hstream-0.1.54/hstream/django_server/hs/apps.py
--rw-r--r--   0        0        0      749 2024-05-26 13:11:50.984442 hstream-0.1.54/hstream/django_server/hs/session_utils.py
--rw-r--r--   0        0        0      424 2024-05-26 13:11:50.984442 hstream-0.1.54/hstream/django_server/hs/urls.py
--rw-r--r--   0        0        0     7872 2024-05-26 13:11:50.984442 hstream-0.1.54/hstream/django_server/hs/views.py
--rwxr-xr-x   0        0        0      661 2024-05-26 13:11:50.984442 hstream-0.1.54/hstream/django_server/manage.py
--rw-r--r--   0        0        0        0 2024-05-26 13:11:50.984442 hstream-0.1.54/hstream/django_server/root/__init__.py
--rw-r--r--   0        0        0      381 2024-05-26 13:11:50.984442 hstream-0.1.54/hstream/django_server/root/asgi.py
--rw-r--r--   0        0        0     3218 2024-05-26 13:11:50.984442 hstream-0.1.54/hstream/django_server/root/settings.py
--rw-r--r--   0        0        0      802 2024-05-26 13:11:50.984442 hstream-0.1.54/hstream/django_server/root/urls.py
--rw-r--r--   0        0        0      381 2024-05-26 13:11:50.984442 hstream-0.1.54/hstream/django_server/root/wsgi.py
--rw-r--r--   0        0        0      683 2024-05-26 13:11:50.984442 hstream-0.1.54/hstream/hs.py
--rw-r--r--   0        0        0      638 2024-05-26 13:11:50.984442 hstream-0.1.54/hstream/run.py
--rw-r--r--   0        0        0      394 2024-05-26 13:11:50.984442 hstream-0.1.54/hstream/template.py
--rw-r--r--   0        0        0      162 2024-05-26 13:11:50.984442 hstream-0.1.54/hstream/templates/error_html.html
--rw-r--r--   0        0        0     2446 2024-05-26 13:11:50.984442 hstream-0.1.54/hstream/templates/format_html.html
--rw-r--r--   0        0        0     2466 2024-05-26 13:11:50.984442 hstream-0.1.54/hstream/utils.py
--rw-r--r--   0        0        0      677 2024-05-26 13:11:50.984442 hstream-0.1.54/pyproject.toml
--rw-r--r--   0        0        0     2509 1970-01-01 00:00:00.000000 hstream-0.1.54/PKG-INFO
+-rw-r--r--   0        0        0     1927 2024-05-27 00:26:00.187594 hstream-0.1.55/README.md
+-rw-r--r--   0        0        0       53 2024-05-27 00:26:00.195594 hstream-0.1.55/hstream/__init__.py
+-rw-r--r--   0        0        0       66 2024-05-27 00:26:00.195594 hstream-0.1.55/hstream/__main__.py
+-rw-r--r--   0        0        0     3522 2024-05-27 00:26:00.195594 hstream-0.1.55/hstream/cli.py
+-rw-r--r--   0        0        0    19076 2024-05-27 00:26:00.195594 hstream-0.1.55/hstream/components/components.py
+-rw-r--r--   0        0        0     4625 2024-05-27 00:26:00.195594 hstream-0.1.55/hstream/components/styling_components.py
+-rw-r--r--   0        0        0        0 2024-05-27 00:26:00.195594 hstream-0.1.55/hstream/django_server/hs/__init__.py
+-rw-r--r--   0        0        0      136 2024-05-27 00:26:00.195594 hstream-0.1.55/hstream/django_server/hs/apps.py
+-rw-r--r--   0        0        0      749 2024-05-27 00:26:00.195594 hstream-0.1.55/hstream/django_server/hs/session_utils.py
+-rw-r--r--   0        0        0      424 2024-05-27 00:26:00.195594 hstream-0.1.55/hstream/django_server/hs/urls.py
+-rw-r--r--   0        0        0     7872 2024-05-27 00:26:00.199594 hstream-0.1.55/hstream/django_server/hs/views.py
+-rwxr-xr-x   0        0        0      661 2024-05-27 00:26:00.199594 hstream-0.1.55/hstream/django_server/manage.py
+-rw-r--r--   0        0        0        0 2024-05-27 00:26:00.199594 hstream-0.1.55/hstream/django_server/root/__init__.py
+-rw-r--r--   0        0        0      381 2024-05-27 00:26:00.199594 hstream-0.1.55/hstream/django_server/root/asgi.py
+-rw-r--r--   0        0        0     3218 2024-05-27 00:26:00.199594 hstream-0.1.55/hstream/django_server/root/settings.py
+-rw-r--r--   0        0        0      802 2024-05-27 00:26:00.199594 hstream-0.1.55/hstream/django_server/root/urls.py
+-rw-r--r--   0        0        0      381 2024-05-27 00:26:00.199594 hstream-0.1.55/hstream/django_server/root/wsgi.py
+-rw-r--r--   0        0        0      683 2024-05-27 00:26:00.199594 hstream-0.1.55/hstream/hs.py
+-rw-r--r--   0        0        0      642 2024-05-27 00:26:00.199594 hstream-0.1.55/hstream/run.py
+-rw-r--r--   0        0        0      394 2024-05-27 00:26:00.199594 hstream-0.1.55/hstream/template.py
+-rw-r--r--   0        0        0      162 2024-05-27 00:26:00.199594 hstream-0.1.55/hstream/templates/error_html.html
+-rw-r--r--   0        0        0     2446 2024-05-27 00:26:00.199594 hstream-0.1.55/hstream/templates/format_html.html
+-rw-r--r--   0        0        0     2466 2024-05-27 00:26:00.199594 hstream-0.1.55/hstream/utils.py
+-rw-r--r--   0        0        0      677 2024-05-27 00:26:00.199594 hstream-0.1.55/pyproject.toml
+-rw-r--r--   0        0        0     2509 1970-01-01 00:00:00.000000 hstream-0.1.55/PKG-INFO
```

### Comparing `hstream-0.1.54/README.md` & `hstream-0.1.55/README.md`

 * *Files identical despite different names*

### Comparing `hstream-0.1.54/hstream/cli.py` & `hstream-0.1.55/hstream/cli.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.54/hstream/components/components.py` & `hstream-0.1.55/hstream/components/components.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.54/hstream/components/styling_components.py` & `hstream-0.1.55/hstream/components/styling_components.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.54/hstream/django_server/hs/session_utils.py` & `hstream-0.1.55/hstream/django_server/hs/session_utils.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.54/hstream/django_server/hs/views.py` & `hstream-0.1.55/hstream/django_server/hs/views.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.54/hstream/django_server/manage.py` & `hstream-0.1.55/hstream/django_server/manage.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.54/hstream/django_server/root/settings.py` & `hstream-0.1.55/hstream/django_server/root/settings.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.54/hstream/django_server/root/urls.py` & `hstream-0.1.55/hstream/django_server/root/urls.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.54/hstream/hs.py` & `hstream-0.1.55/hstream/hs.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.54/hstream/run.py` & `hstream-0.1.55/hstream/run.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 
 
 def run_server(
     file: Path, other_paths: Dict[str, Path] = False, hs_root_path: str = "/"
 ):
     path_to_hstream_dir = os.path.dirname(os.path.abspath(hstream.__file__))
 
-    os.system(f"python {path_to_hstream_dir}/django_server/manage.py migrate")
+    os.system(f'python "{path_to_hstream_dir}/django_server/manage.py" migrate')
     os.environ["HS_FILE_TO_RUN"] = str(file)
-    command = f"python {path_to_hstream_dir}/django_server/manage.py runserver"
+    command = f'python "{path_to_hstream_dir}/django_server/manage.py" runserver'
     if os.environ.get("PORT", False):
         print(f"found port in env, using port {os.environ['PORT']}")
         command += f" 0.0.0.0:{os.environ['PORT']}"
     os.system(command)
```

### Comparing `hstream-0.1.54/hstream/templates/format_html.html` & `hstream-0.1.55/hstream/templates/format_html.html`

 * *Files identical despite different names*

### Comparing `hstream-0.1.54/hstream/utils.py` & `hstream-0.1.55/hstream/utils.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.54/pyproject.toml` & `hstream-0.1.55/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hstream"
-version = "0.1.54"
+version = "0.1.55"
 description = ""
 authors = ["Conrad <conradbez1@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 hstream = "hstream.cli:cli"
```

### Comparing `hstream-0.1.54/PKG-INFO` & `hstream-0.1.55/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hstream
-Version: 0.1.54
+Version: 0.1.55
 Summary: 
 Author: Conrad
 Author-email: conradbez1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

