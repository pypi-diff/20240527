# Comparing `tmp/ralium-2.0.1.tar.gz` & `tmp/ralium-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralium-2.0.1.tar", last modified: Tue May 21 15:40:11 2024, max compression
+gzip compressed data, was "ralium-2.0.2.tar", last modified: Mon May 27 18:23:48 2024, max compression
```

## Comparing `ralium-2.0.1.tar` & `ralium-2.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 15:40:11.419403 ralium-2.0.1/
--rw-rw-rw-   0        0        0    35823 2024-05-21 00:22:26.000000 ralium-2.0.1/LICENSE
--rw-rw-rw-   0        0        0    41897 2024-05-21 15:40:11.418157 ralium-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       52 2024-05-21 00:22:26.000000 ralium-2.0.1/README.md
--rw-rw-rw-   0        0        0      970 2024-05-21 15:39:27.000000 ralium-2.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-21 15:40:11.384180 ralium-2.0.1/ralium/
--rw-rw-rw-   0        0        0      357 2024-05-21 05:00:06.000000 ralium-2.0.1/ralium/__init__.py
--rw-rw-rw-   0        0        0     2600 2024-05-21 15:39:34.000000 ralium-2.0.1/ralium/_util.py
--rw-rw-rw-   0        0        0     1194 2024-05-21 06:24:20.000000 ralium-2.0.1/ralium/_util.pyi
--rw-rw-rw-   0        0        0     7555 2024-05-21 04:21:31.000000 ralium-2.0.1/ralium/api.py
--rw-rw-rw-   0        0        0     1066 2024-05-21 00:25:27.000000 ralium-2.0.1/ralium/api.pyi
--rw-rw-rw-   0        0        0      680 2024-05-21 00:25:27.000000 ralium-2.0.1/ralium/builtins.py
--rw-rw-rw-   0        0        0      541 2024-05-21 00:25:27.000000 ralium-2.0.1/ralium/builtins.pyi
--rw-rw-rw-   0        0        0     8231 2024-05-21 06:11:47.000000 ralium-2.0.1/ralium/bundle.py
--rw-rw-rw-   0        0        0     1581 2024-05-21 00:26:03.000000 ralium-2.0.1/ralium/bundle.pyi
--rw-rw-rw-   0        0        0     3332 2024-05-21 00:25:27.000000 ralium-2.0.1/ralium/config.py
--rw-rw-rw-   0        0        0      467 2024-05-21 00:25:27.000000 ralium-2.0.1/ralium/config.pyi
--rw-rw-rw-   0        0        0     6425 2024-05-21 00:25:27.000000 ralium-2.0.1/ralium/element.py
--rw-rw-rw-   0        0        0     1376 2024-05-21 00:26:03.000000 ralium-2.0.1/ralium/element.pyi
--rw-rw-rw-   0        0        0     4402 2024-05-21 00:26:03.000000 ralium-2.0.1/ralium/engine.py
--rw-rw-rw-   0        0        0     1389 2024-05-21 00:25:27.000000 ralium-2.0.1/ralium/engine.pyi
--rw-rw-rw-   0        0        0     1233 2024-05-21 06:18:29.000000 ralium-2.0.1/ralium/errors.py
--rw-rw-rw-   0        0        0     2387 2024-05-21 00:25:27.000000 ralium-2.0.1/ralium/listener.py
--rw-rw-rw-   0        0        0      890 2024-05-21 00:25:27.000000 ralium-2.0.1/ralium/listener.pyi
--rw-rw-rw-   0        0        0      804 2024-05-21 00:25:27.000000 ralium-2.0.1/ralium/navigation.py
--rw-rw-rw-   0        0        0      376 2024-05-21 00:25:27.000000 ralium-2.0.1/ralium/navigation.pyi
--rw-rw-rw-   0        0        0     4805 2024-05-21 15:38:14.000000 ralium-2.0.1/ralium/pyhtml.py
--rw-rw-rw-   0        0        0      531 2024-05-21 07:20:26.000000 ralium-2.0.1/ralium/pyhtml.pyi
--rw-rw-rw-   0        0        0     7851 2024-05-21 05:23:35.000000 ralium-2.0.1/ralium/setuptools.py
--rw-rw-rw-   0        0        0      965 2024-05-21 05:19:13.000000 ralium-2.0.1/ralium/setuptools.pyi
--rw-rw-rw-   0        0        0     6936 2024-05-21 00:26:03.000000 ralium-2.0.1/ralium/webpage.py
--rw-rw-rw-   0        0        0     1870 2024-05-21 00:26:03.000000 ralium-2.0.1/ralium/webpage.pyi
--rw-rw-rw-   0        0        0     6078 2024-05-21 06:47:26.000000 ralium-2.0.1/ralium/window.py
--rw-rw-rw-   0        0        0      693 2024-05-21 00:25:27.000000 ralium-2.0.1/ralium/window.pyi
-drwxrwxrwx   0        0        0        0 2024-05-21 15:40:11.416675 ralium-2.0.1/ralium.egg-info/
--rw-rw-rw-   0        0        0    41897 2024-05-21 15:40:11.000000 ralium-2.0.1/ralium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      692 2024-05-21 15:40:11.000000 ralium-2.0.1/ralium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 15:40:11.000000 ralium-2.0.1/ralium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 15:40:11.000000 ralium-2.0.1/ralium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-21 15:40:11.000000 ralium-2.0.1/ralium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 15:40:11.419403 ralium-2.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-27 18:23:48.303274 ralium-2.0.2/
+-rw-rw-rw-   0        0        0    35823 2024-05-21 00:22:26.000000 ralium-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0    41897 2024-05-27 18:23:48.302168 ralium-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2024-05-21 00:22:26.000000 ralium-2.0.2/README.md
+-rw-rw-rw-   0        0        0      970 2024-05-27 18:23:05.000000 ralium-2.0.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-27 18:23:48.277866 ralium-2.0.2/ralium/
+-rw-rw-rw-   0        0        0      357 2024-05-21 05:00:06.000000 ralium-2.0.2/ralium/__init__.py
+-rw-rw-rw-   0        0        0     1845 2024-05-27 18:23:09.000000 ralium-2.0.2/ralium/_util.py
+-rw-rw-rw-   0        0        0     1098 2024-05-27 18:21:08.000000 ralium-2.0.2/ralium/_util.pyi
+-rw-rw-rw-   0        0        0     7555 2024-05-21 04:21:31.000000 ralium-2.0.2/ralium/api.py
+-rw-rw-rw-   0        0        0     1066 2024-05-21 00:25:27.000000 ralium-2.0.2/ralium/api.pyi
+-rw-rw-rw-   0        0        0      680 2024-05-21 00:25:27.000000 ralium-2.0.2/ralium/builtins.py
+-rw-rw-rw-   0        0        0      541 2024-05-21 00:25:27.000000 ralium-2.0.2/ralium/builtins.pyi
+-rw-rw-rw-   0        0        0     8231 2024-05-21 06:11:47.000000 ralium-2.0.2/ralium/bundle.py
+-rw-rw-rw-   0        0        0     1581 2024-05-21 00:26:03.000000 ralium-2.0.2/ralium/bundle.pyi
+-rw-rw-rw-   0        0        0     3332 2024-05-21 00:25:27.000000 ralium-2.0.2/ralium/config.py
+-rw-rw-rw-   0        0        0      467 2024-05-21 00:25:27.000000 ralium-2.0.2/ralium/config.pyi
+-rw-rw-rw-   0        0        0     6425 2024-05-21 00:25:27.000000 ralium-2.0.2/ralium/element.py
+-rw-rw-rw-   0        0        0     1376 2024-05-21 00:26:03.000000 ralium-2.0.2/ralium/element.pyi
+-rw-rw-rw-   0        0        0     4402 2024-05-21 00:26:03.000000 ralium-2.0.2/ralium/engine.py
+-rw-rw-rw-   0        0        0     1389 2024-05-21 00:25:27.000000 ralium-2.0.2/ralium/engine.pyi
+-rw-rw-rw-   0        0        0     1147 2024-05-27 18:22:26.000000 ralium-2.0.2/ralium/errors.py
+-rw-rw-rw-   0        0        0     2387 2024-05-21 00:25:27.000000 ralium-2.0.2/ralium/listener.py
+-rw-rw-rw-   0        0        0      890 2024-05-21 00:25:27.000000 ralium-2.0.2/ralium/listener.pyi
+-rw-rw-rw-   0        0        0      804 2024-05-21 00:25:27.000000 ralium-2.0.2/ralium/navigation.py
+-rw-rw-rw-   0        0        0      376 2024-05-21 00:25:27.000000 ralium-2.0.2/ralium/navigation.pyi
+-rw-rw-rw-   0        0        0     4805 2024-05-21 15:38:14.000000 ralium-2.0.2/ralium/pyhtml.py
+-rw-rw-rw-   0        0        0      531 2024-05-21 07:20:26.000000 ralium-2.0.2/ralium/pyhtml.pyi
+-rw-rw-rw-   0        0        0     7851 2024-05-21 05:23:35.000000 ralium-2.0.2/ralium/setuptools.py
+-rw-rw-rw-   0        0        0      965 2024-05-21 05:19:13.000000 ralium-2.0.2/ralium/setuptools.pyi
+-rw-rw-rw-   0        0        0     6452 2024-05-27 18:22:15.000000 ralium-2.0.2/ralium/webpage.py
+-rw-rw-rw-   0        0        0     1870 2024-05-21 00:26:03.000000 ralium-2.0.2/ralium/webpage.pyi
+-rw-rw-rw-   0        0        0     6078 2024-05-27 18:21:30.000000 ralium-2.0.2/ralium/window.py
+-rw-rw-rw-   0        0        0      693 2024-05-21 00:25:27.000000 ralium-2.0.2/ralium/window.pyi
+drwxrwxrwx   0        0        0        0 2024-05-27 18:23:48.300131 ralium-2.0.2/ralium.egg-info/
+-rw-rw-rw-   0        0        0    41897 2024-05-27 18:23:48.000000 ralium-2.0.2/ralium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      692 2024-05-27 18:23:48.000000 ralium-2.0.2/ralium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 18:23:48.000000 ralium-2.0.2/ralium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 18:23:48.000000 ralium-2.0.2/ralium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-27 18:23:48.000000 ralium-2.0.2/ralium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 18:23:48.303274 ralium-2.0.2/setup.cfg
```

### Comparing `ralium-2.0.1/LICENSE` & `ralium-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ralium-2.0.1/PKG-INFO` & `ralium-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 2.0.1
+Version: 2.0.2
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-2.0.1/pyproject.toml` & `ralium-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools >= 69.5.0", "wheel >= 0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ralium"
-version = "2.0.1"
+version = "2.0.2"
 description = "An easy to use wrapper for pywebview."
 readme = "README.md"
 authors = [{ name = "Isaiah Coroama", email = "coroamaisaiah@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

### Comparing `ralium-2.0.1/ralium/_util.pyi` & `ralium-2.0.2/ralium/_util.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     ModuleType
 )
 
 import http.server
 
 __all__ = [
     "__version__", "BasicHTTPServer", "NamedDict", "_get_http_server_handler", "_get_bundle", 
-    "_norm_url", "_check_exists",  "_check_is_dir", "_get_path_limit", "_read_file", "_get_path"
+    "_norm_url", "_check_exists",  "_check_is_dir", "_read_file", "_get_path"
 ]
 
 __version__: str
 
 _RT = TypeVar("_RT") # Return Type
 ClassType: TypeAlias = object
 DirPathStr: TypeAlias = str
@@ -34,11 +34,9 @@
     def __init__(self, iterable: dict[str, Any]) -> None: ...
 
 def _get_bundle() -> FileSystem | None: ...
 def _get_http_server_handler() -> BasicHTTPServer | BundledHTTPServer: ...
 def _check_exists(path: str) -> bool: ...
 def _check_is_dir(path: str) -> bool: ...
 def _norm_url(path: str) -> str: ...
-def _get_path_limit_winreg() -> int: ...
-def _get_path_limit() -> int: ...
 def _read_file(path: str, encoding: str = "UTF-8") -> str: ...
 def _get_path(path: str) -> str: ...
```

### Comparing `ralium-2.0.1/ralium/api.py` & `ralium-2.0.2/ralium/api.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.1/ralium/api.pyi` & `ralium-2.0.2/ralium/api.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.1/ralium/builtins.py` & `ralium-2.0.2/ralium/builtins.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.1/ralium/builtins.pyi` & `ralium-2.0.2/ralium/builtins.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.1/ralium/bundle.py` & `ralium-2.0.2/ralium/bundle.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.1/ralium/bundle.pyi` & `ralium-2.0.2/ralium/bundle.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.1/ralium/config.py` & `ralium-2.0.2/ralium/config.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.1/ralium/element.py` & `ralium-2.0.2/ralium/element.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.1/ralium/element.pyi` & `ralium-2.0.2/ralium/element.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.1/ralium/engine.py` & `ralium-2.0.2/ralium/engine.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.1/ralium/engine.pyi` & `ralium-2.0.2/ralium/engine.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.1/ralium/errors.py` & `ralium-2.0.2/ralium/errors.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 global __RALIUM_WARNING_MESSAGES__
 __RALIUM_WARNING_MESSAGES__ = True
 
 class SetupError(Exception): pass
 class WindowLoadError(Exception): pass
 class BridgeEventError(Exception): pass
 class PyHTMLSyntaxError(Exception): pass
-class FilePathLimitError(Exception): pass
 class RegistryNotFoundError(Exception): pass
 class WindowNotRunningError(Exception): pass
 
 class WebFunctionApiError(Exception): pass
 
 class WebHookNotFoundError(Exception): pass
 class WebHookHomepageError(Exception): pass
@@ -19,15 +18,14 @@
 class WebFolderNotFoundError(Exception): pass
 class WebRoutesNotFoundError(Exception): pass
 
 class WebFolderDirectoryError(Exception): pass
 class WebRoutesDirectoryError(Exception): pass
 
 class FileNotFoundWarning(Warning): pass
-class FilePathLimitWarning(Warning): pass
 
 def DisableWarnings():
     """
     Disables Ralium warnings from being displayed.
     """
 
     global __RALIUM_WARNING_MESSAGES__
```

### Comparing `ralium-2.0.1/ralium/listener.py` & `ralium-2.0.2/ralium/listener.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.1/ralium/listener.pyi` & `ralium-2.0.2/ralium/listener.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.1/ralium/navigation.py` & `ralium-2.0.2/ralium/navigation.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.1/ralium/pyhtml.py` & `ralium-2.0.2/ralium/pyhtml.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.1/ralium/pyhtml.pyi` & `ralium-2.0.2/ralium/pyhtml.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.1/ralium/setuptools.py` & `ralium-2.0.2/ralium/setuptools.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.1/ralium/setuptools.pyi` & `ralium-2.0.2/ralium/setuptools.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.1/ralium/webpage.py` & `ralium-2.0.2/ralium/webpage.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,20 +12,14 @@
 </html>"""
 
 class FileReader:
     def __init__(self, file, encoding):
         self.__data = file
         self.__read = False
         self.__encoding = encoding
-
-        path_length = len(self.__data)
-        path_limit = _get_path_limit()
-
-        if path_length > path_limit:
-            raise FilePathLimitError(f"Failed to load file, exceeds the max path limit of '{path_limit}'")
         
     @property
     def content(self):
         self._read()
         return self.__data
     
     def _read(self):
@@ -40,17 +34,14 @@
 
 class CSSReader:
     def __init__(self, *files, encoding):
         self.__readers = []
 
         for file in files:
             if _check_exists(file):
-                if len(file) <= _get_path_limit():
-                    warn(f"File '{file}' exceeds path limit.", FilePathLimitWarning, major=True)
-                
                 self.__readers.append(FileReader(file, encoding))
                 continue
 
             self.__readers.append(file)
 
     @property
     def content(self):
@@ -107,15 +98,14 @@
     :param css: A file path or list of file paths to style the HTML.
     :param functions: Functions to expose to JavaScript.
     :param namespaces: Namespaces to expose to JavaScript.
     :param homepage: If this WebHook is a homepage, it will be the fallback page if something goes wrong with the `Navigation` handler.
     :param encoding: The file encoding of the HTML and CSS files.
 
     :raises FileNotFoundWarning: Displays a warning if a file doesn't exist. (Only if warnings are enabled.)
-    :raises FilePathLimitError: If a path exceeds the system limit for path lengths.
     """
 
     def __init__(self, url, html, css = None, functions = None, namespaces = None, homepage = False, encoding = "UTF-8"):
         self.url = _norm_url(url)
         self.css = css or ""
         self.html = html
         self.window = None
```

### Comparing `ralium-2.0.1/ralium/webpage.pyi` & `ralium-2.0.2/ralium/webpage.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.1/ralium/window.py` & `ralium-2.0.2/ralium/window.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.1/ralium/window.pyi` & `ralium-2.0.2/ralium/window.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.1/ralium.egg-info/PKG-INFO` & `ralium-2.0.2/ralium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 2.0.1
+Version: 2.0.2
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-2.0.1/ralium.egg-info/SOURCES.txt` & `ralium-2.0.2/ralium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

