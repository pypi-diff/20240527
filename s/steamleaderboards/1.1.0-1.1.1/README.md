# Comparing `tmp/steamleaderboards-1.1.0.tar.gz` & `tmp/steamleaderboards-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steamleaderboards-1.1.0.tar", max compression
+gzip compressed data, was "steamleaderboards-1.1.1.tar", max compression
```

## Comparing `steamleaderboards-1.1.0.tar` & `steamleaderboards-1.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1072 2024-05-24 23:19:06.948186 steamleaderboards-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2076 2024-05-25 01:55:51.395337 steamleaderboards-1.1.0/README.md
--rw-r--r--   0        0        0      983 2024-05-26 08:32:26.181580 steamleaderboards-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     5560 2024-05-26 08:31:57.084580 steamleaderboards-1.1.0/steamleaderboards/__init__.py
--rw-r--r--   0        0        0     2187 2024-05-26 08:28:43.829577 steamleaderboards-1.1.0/steamleaderboards/__main__.py
--rw-r--r--   0        0        0     3278 1970-01-01 00:00:00.000000 steamleaderboards-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-24 23:19:06.948186 steamleaderboards-1.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     2076 2024-05-25 01:55:51.395337 steamleaderboards-1.1.1/README.md
+-rw-r--r--   0        0        0      983 2024-05-27 01:55:13.122589 steamleaderboards-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5616 2024-05-27 01:38:41.811573 steamleaderboards-1.1.1/steamleaderboards/__init__.py
+-rw-r--r--   0        0        0     2187 2024-05-26 08:28:43.829577 steamleaderboards-1.1.1/steamleaderboards/__main__.py
+-rw-r--r--   0        0        0     3278 1970-01-01 00:00:00.000000 steamleaderboards-1.1.1/PKG-INFO
```

### Comparing `steamleaderboards-1.1.0/LICENSE.txt` & `steamleaderboards-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `steamleaderboards-1.1.0/README.md` & `steamleaderboards-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `steamleaderboards-1.1.0/pyproject.toml` & `steamleaderboards-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "steamleaderboards"
-version = "1.1.0"
+version = "1.1.1"
 description = "Retrieve and parse Steam leaderboards"
 authors = ["Stefano Pigozzi <me@steffo.eu>"]
 maintainers = ["Stefano Pigozzi <me@steffo.eu>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Steffo99/steamleaderboards"
 keywords = ["steam", "leaderboards", "csv", "xml", "valve"]
```

### Comparing `steamleaderboards-1.1.0/steamleaderboards/__init__.py` & `steamleaderboards-1.1.1/steamleaderboards/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,15 @@
         while next_request_url:
             xml = requests.get(next_request_url)
             _bs = BeautifulSoup(xml.content, features="lxml-xml")
             for entry in _bs.find_all("entry"):
                 self.entries.append(Entry(entry))
                 if len(self.entries) >= limit:
                     next_request_url = None
+                    self.entries = self.entries[:limit]
                     break
             else:
                 try:
                     next_request_url = _bs.find_all("nextRequestURL")[0].text
                 except IndexError:
                     next_request_url = None
                 else:
```

### Comparing `steamleaderboards-1.1.0/steamleaderboards/__main__.py` & `steamleaderboards-1.1.1/steamleaderboards/__main__.py`

 * *Files identical despite different names*

### Comparing `steamleaderboards-1.1.0/PKG-INFO` & `steamleaderboards-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steamleaderboards
-Version: 1.1.0
+Version: 1.1.1
 Summary: Retrieve and parse Steam leaderboards
 Home-page: https://github.com/Steffo99/steamleaderboards
 License: MIT
 Keywords: steam,leaderboards,csv,xml,valve
 Author: Stefano Pigozzi
 Author-email: me@steffo.eu
 Maintainer: Stefano Pigozzi
```

