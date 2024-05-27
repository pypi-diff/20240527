# Comparing `tmp/caerp_oidc_client-2024.1.4.tar.gz` & `tmp/caerp_oidc_client-2024.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caerp_oidc_client-2024.1.4.tar", last modified: Fri Mar 15 11:01:12 2024, max compression
+gzip compressed data, was "caerp_oidc_client-2024.1.5.tar", last modified: Mon May 27 16:55:23 2024, max compression
```

## Comparing `caerp_oidc_client-2024.1.4.tar` & `caerp_oidc_client-2024.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-03-15 11:01:12.772693 caerp_oidc_client-2024.1.4/
--rw-r--r--   0 gas       (1000) gas       (1000)    35147 2023-03-10 16:27:25.000000 caerp_oidc_client-2024.1.4/LICENSE.txt
--rw-r--r--   0 gas       (1000) gas       (1000)      182 2024-02-27 15:53:54.000000 caerp_oidc_client-2024.1.4/MANIFEST.in
--rw-r--r--   0 gas       (1000) gas       (1000)     2629 2024-03-15 11:01:12.772693 caerp_oidc_client-2024.1.4/PKG-INFO
--rw-r--r--   0 gas       (1000) gas       (1000)     1953 2024-03-05 16:07:37.000000 caerp_oidc_client-2024.1.4/README.md
--rw-r--r--   0 gas       (1000) gas       (1000)      250 2024-02-27 15:39:05.000000 caerp_oidc_client-2024.1.4/pyproject.toml
--rw-r--r--   0 gas       (1000) gas       (1000)       79 2024-03-15 11:01:12.773693 caerp_oidc_client-2024.1.4/setup.cfg
--rw-r--r--   0 gas       (1000) gas       (1000)     1181 2024-03-15 11:00:51.000000 caerp_oidc_client-2024.1.4/setup.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-03-15 11:01:12.768693 caerp_oidc_client-2024.1.4/src/
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-03-15 11:01:12.770693 caerp_oidc_client-2024.1.4/src/caerp_oidc_client/
--rw-r--r--   0 gas       (1000) gas       (1000)      194 2024-03-05 16:07:39.000000 caerp_oidc_client-2024.1.4/src/caerp_oidc_client/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)     1255 2024-03-05 16:07:42.000000 caerp_oidc_client-2024.1.4/src/caerp_oidc_client/models.py
--rw-r--r--   0 gas       (1000) gas       (1000)     1103 2024-02-28 18:38:04.000000 caerp_oidc_client-2024.1.4/src/caerp_oidc_client/utils.py
--rw-r--r--   0 gas       (1000) gas       (1000)     9882 2024-03-15 10:58:54.000000 caerp_oidc_client-2024.1.4/src/caerp_oidc_client/views.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-03-15 11:01:12.772693 caerp_oidc_client-2024.1.4/src/caerp_oidc_client.egg-info/
--rw-r--r--   0 gas       (1000) gas       (1000)     2629 2024-03-15 11:01:12.000000 caerp_oidc_client-2024.1.4/src/caerp_oidc_client.egg-info/PKG-INFO
--rw-r--r--   0 gas       (1000) gas       (1000)      463 2024-03-15 11:01:12.000000 caerp_oidc_client-2024.1.4/src/caerp_oidc_client.egg-info/SOURCES.txt
--rw-r--r--   0 gas       (1000) gas       (1000)        1 2024-03-15 11:01:12.000000 caerp_oidc_client-2024.1.4/src/caerp_oidc_client.egg-info/dependency_links.txt
--rw-r--r--   0 gas       (1000) gas       (1000)        1 2024-02-27 15:46:08.000000 caerp_oidc_client-2024.1.4/src/caerp_oidc_client.egg-info/not-zip-safe
--rw-r--r--   0 gas       (1000) gas       (1000)       15 2024-03-15 11:01:12.000000 caerp_oidc_client-2024.1.4/src/caerp_oidc_client.egg-info/requires.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       18 2024-03-15 11:01:12.000000 caerp_oidc_client-2024.1.4/src/caerp_oidc_client.egg-info/top_level.txt
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-27 16:55:23.510403 caerp_oidc_client-2024.1.5/
+-rw-r--r--   0 gas       (1000) gas       (1000)    35147 2023-03-10 16:27:25.000000 caerp_oidc_client-2024.1.5/LICENSE.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)      182 2024-02-27 15:53:54.000000 caerp_oidc_client-2024.1.5/MANIFEST.in
+-rw-r--r--   0 gas       (1000) gas       (1000)     2629 2024-05-27 16:55:23.511404 caerp_oidc_client-2024.1.5/PKG-INFO
+-rw-r--r--   0 gas       (1000) gas       (1000)     1953 2024-03-05 16:07:37.000000 caerp_oidc_client-2024.1.5/README.md
+-rw-r--r--   0 gas       (1000) gas       (1000)      250 2024-02-27 15:39:05.000000 caerp_oidc_client-2024.1.5/pyproject.toml
+-rw-r--r--   0 gas       (1000) gas       (1000)       79 2024-05-27 16:55:23.512404 caerp_oidc_client-2024.1.5/setup.cfg
+-rw-r--r--   0 gas       (1000) gas       (1000)     1181 2024-05-27 16:55:00.000000 caerp_oidc_client-2024.1.5/setup.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-27 16:55:23.505404 caerp_oidc_client-2024.1.5/src/
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-27 16:55:23.509404 caerp_oidc_client-2024.1.5/src/caerp_oidc_client/
+-rw-r--r--   0 gas       (1000) gas       (1000)      194 2024-03-05 16:07:39.000000 caerp_oidc_client-2024.1.5/src/caerp_oidc_client/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     1255 2024-03-05 16:07:42.000000 caerp_oidc_client-2024.1.5/src/caerp_oidc_client/models.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     1112 2024-05-27 16:54:02.000000 caerp_oidc_client-2024.1.5/src/caerp_oidc_client/utils.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     9947 2024-04-24 13:14:11.000000 caerp_oidc_client-2024.1.5/src/caerp_oidc_client/views.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-27 16:55:23.510403 caerp_oidc_client-2024.1.5/src/caerp_oidc_client.egg-info/
+-rw-r--r--   0 gas       (1000) gas       (1000)     2629 2024-05-27 16:55:23.000000 caerp_oidc_client-2024.1.5/src/caerp_oidc_client.egg-info/PKG-INFO
+-rw-r--r--   0 gas       (1000) gas       (1000)      463 2024-05-27 16:55:23.000000 caerp_oidc_client-2024.1.5/src/caerp_oidc_client.egg-info/SOURCES.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)        1 2024-05-27 16:55:23.000000 caerp_oidc_client-2024.1.5/src/caerp_oidc_client.egg-info/dependency_links.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)        1 2024-02-27 15:46:08.000000 caerp_oidc_client-2024.1.5/src/caerp_oidc_client.egg-info/not-zip-safe
+-rw-r--r--   0 gas       (1000) gas       (1000)       15 2024-05-27 16:55:23.000000 caerp_oidc_client-2024.1.5/src/caerp_oidc_client.egg-info/requires.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       18 2024-05-27 16:55:23.000000 caerp_oidc_client-2024.1.5/src/caerp_oidc_client.egg-info/top_level.txt
```

### Comparing `caerp_oidc_client-2024.1.4/LICENSE.txt` & `caerp_oidc_client-2024.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `caerp_oidc_client-2024.1.4/PKG-INFO` & `caerp_oidc_client-2024.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caerp_oidc_client
-Version: 2024.1.4
+Version: 2024.1.5
 Summary: OpenID Connect client for CAERP
 Home-page: https://framagit.org/caerp/caerp_oidc_client
 Author: Gaston Tjebbes - Majerti
 Author-email: tech@majerti.fr
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `caerp_oidc_client-2024.1.4/README.md` & `caerp_oidc_client-2024.1.5/README.md`

 * *Files identical despite different names*

### Comparing `caerp_oidc_client-2024.1.4/setup.py` & `caerp_oidc_client-2024.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name='caerp_oidc_client',
-    version='2024.1.4',
+    version='2024.1.5',
     package_dir={"": "src"},
     packages=find_packages(where='src'),
     include_package_data=True,
     license='GPLv3',
     url="https://framagit.org/caerp/caerp_oidc_client",
     description="OpenID Connect client for CAERP",
     author='Gaston Tjebbes - Majerti',
```

### Comparing `caerp_oidc_client-2024.1.4/src/caerp_oidc_client/models.py` & `caerp_oidc_client-2024.1.5/src/caerp_oidc_client/models.py`

 * *Files identical despite different names*

### Comparing `caerp_oidc_client-2024.1.4/src/caerp_oidc_client/utils.py` & `caerp_oidc_client-2024.1.5/src/caerp_oidc_client/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Set of utilities implementing a set of openid connect specs related actions"""
+
 import base64
 import json
 
 SETTINGS_KEYS = (
     "oidc.client_secret",
     "oidc.scope",
     "oidc.client_id",
@@ -33,9 +34,9 @@
     """
     parts = token.split(".")
     if len(parts) != 3:
         raise Exception("Incorrect id token format")
 
     payload = parts[1]
     padded = payload + "=" * (4 - len(payload) % 4)
-    decoded = base64.b64decode(padded)
+    decoded = base64.urlsafe_b64decode(padded)
     return json.loads(decoded)
```

### Comparing `caerp_oidc_client-2024.1.4/src/caerp_oidc_client/views.py` & `caerp_oidc_client-2024.1.5/src/caerp_oidc_client/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,14 +182,15 @@
                 logger.exception("Erreur")
                 raise HTTPForbidden()
 
             login = self._get_user_login(auth_data)
             try:
                 connect_user(self.request, login)
             except Exception:
+                logger.exception("Erreur en connectant le user")
                 raise HTTPUnauthorized()
             remember(self.request, login)
             return self.success_response()
 
     def logout_view(self):
         """Logout view"""
         forget(self.request)
```

### Comparing `caerp_oidc_client-2024.1.4/src/caerp_oidc_client.egg-info/PKG-INFO` & `caerp_oidc_client-2024.1.5/src/caerp_oidc_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caerp-oidc-client
-Version: 2024.1.4
+Version: 2024.1.5
 Summary: OpenID Connect client for CAERP
 Home-page: https://framagit.org/caerp/caerp_oidc_client
 Author: Gaston Tjebbes - Majerti
 Author-email: tech@majerti.fr
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

