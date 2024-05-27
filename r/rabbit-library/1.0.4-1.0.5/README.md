# Comparing `tmp/rabbit_library-1.0.4.tar.gz` & `tmp/rabbit_library-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbit_library-1.0.4.tar", max compression
+gzip compressed data, was "rabbit_library-1.0.5.tar", max compression
```

## Comparing `rabbit_library-1.0.4.tar` & `rabbit_library-1.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1130 2024-05-13 16:48:34.469873 rabbit_library-1.0.4/pyproject.toml
--rw-r--r--   0        0        0       26 2023-07-03 17:14:02.867213 rabbit_library-1.0.4/rabbit_library/__init__.py
--rw-r--r--   0        0        0     9327 2024-05-13 16:46:57.259220 rabbit_library-1.0.4/rabbit_library/Rabbit.py
--rw-r--r--   0        0        0     3448 2023-10-26 20:38:03.049544 rabbit_library-1.0.4/README.md
--rw-r--r--   0        0        0     4076 1970-01-01 00:00:00.000000 rabbit_library-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1130 2024-05-27 20:47:51.000761 rabbit_library-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-07-03 17:14:02.867213 rabbit_library-1.0.5/rabbit_library/__init__.py
+-rw-r--r--   0        0        0     9395 2024-05-27 20:44:17.968557 rabbit_library-1.0.5/rabbit_library/Rabbit.py
+-rw-r--r--   0        0        0     3448 2023-10-26 20:38:03.049544 rabbit_library-1.0.5/README.md
+-rw-r--r--   0        0        0     4076 1970-01-01 00:00:00.000000 rabbit_library-1.0.5/PKG-INFO
```

### Comparing `rabbit_library-1.0.4/pyproject.toml` & `rabbit_library-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rabbit-library"
-version = "1.0.4"
+version = "1.0.5"
 description = "Biblioteca para se conectar ao rabbit e possibilitar trabalhar com o serviço de mensageria"
 license = "MIT"
 authors = ["Eliézer Schwartz <eliezer.mail090@gmail.com>"]
 readme = "README.md"
 packages = [{include = "rabbit_library"}]
 classifiers = [    
     "Environment :: Console",
```

### Comparing `rabbit_library-1.0.4/rabbit_library/Rabbit.py` & `rabbit_library-1.0.5/rabbit_library/Rabbit.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,16 +82,17 @@
                     "Caught a channel error: {}, stopping...".format(err))
                 self.reconnect = False
                 break
             except KeyboardInterrupt:
                 self.reconnect = False
                 break
             except Exception as e:
+                error_message = str(e).encode('ascii', 'ignore').decode('ascii')
                 logging.error(
-                    "Error receiving message from rabbit: {} ".format(e).encode('ascii', 'ignore'), stack_info=True)
+                    "Error receiving message from rabbit: {} ".format(error_message), stack_info=True)
                 self.reconnect = False
                 break
             finally:
                 if not self.continue_execution:
                     if self.reconnect:
                         if self.qtd_reconnects >= 10 and self.qtd_reconnects < 30:
                             self.reconnect_delay_system = 3600
```

### Comparing `rabbit_library-1.0.4/README.md` & `rabbit_library-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `rabbit_library-1.0.4/PKG-INFO` & `rabbit_library-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbit-library
-Version: 1.0.4
+Version: 1.0.5
 Summary: Biblioteca para se conectar ao rabbit e possibilitar trabalhar com o serviço de mensageria
 License: MIT
 Author: Eliézer Schwartz
 Author-email: eliezer.mail090@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

