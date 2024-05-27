# Comparing `tmp/edgegpt_fork-1.0.2.tar.gz` & `tmp/edgegpt_fork-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegpt_fork-1.0.2.tar", last modified: Sat Apr 20 18:37:17 2024, max compression
+gzip compressed data, was "edgegpt_fork-1.0.3.tar", last modified: Mon May 27 12:28:24 2024, max compression
```

## Comparing `edgegpt_fork-1.0.2.tar` & `edgegpt_fork-1.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:37:17.121648 edgegpt_fork-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-20 18:36:57.000000 edgegpt_fork-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12562 2024-04-20 18:37:17.121648 edgegpt_fork-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11539 2024-04-20 18:36:57.000000 edgegpt_fork-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-20 18:37:17.121648 edgegpt_fork-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-20 18:36:57.000000 edgegpt_fork-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:37:17.117648 edgegpt_fork-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:37:17.117648 edgegpt_fork-1.0.2/src/EdgeGPT/
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-04-20 18:36:57.000000 edgegpt_fork-1.0.2/src/EdgeGPT/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-04-20 18:36:57.000000 edgegpt_fork-1.0.2/src/EdgeGPT/EdgeUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-20 18:36:57.000000 edgegpt_fork-1.0.2/src/EdgeGPT/ImageGen.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-20 18:36:57.000000 edgegpt_fork-1.0.2/src/EdgeGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-04-20 18:36:57.000000 edgegpt_fork-1.0.2/src/EdgeGPT/chathub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-20 18:36:57.000000 edgegpt_fork-1.0.2/src/EdgeGPT/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-20 18:36:57.000000 edgegpt_fork-1.0.2/src/EdgeGPT/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-20 18:36:57.000000 edgegpt_fork-1.0.2/src/EdgeGPT/conversation_style.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-20 18:36:57.000000 edgegpt_fork-1.0.2/src/EdgeGPT/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-20 18:36:57.000000 edgegpt_fork-1.0.2/src/EdgeGPT/locale.py
--rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-04-20 18:36:57.000000 edgegpt_fork-1.0.2/src/EdgeGPT/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-20 18:36:57.000000 edgegpt_fork-1.0.2/src/EdgeGPT/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-04-20 18:36:57.000000 edgegpt_fork-1.0.2/src/EdgeGPT/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-20 18:36:57.000000 edgegpt_fork-1.0.2/src/EdgeGPT/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:37:17.121648 edgegpt_fork-1.0.2/src/EdgeGPT_fork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12562 2024-04-20 18:37:17.000000 edgegpt_fork-1.0.2/src/EdgeGPT_fork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-20 18:37:17.000000 edgegpt_fork-1.0.2/src/EdgeGPT_fork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:37:17.000000 edgegpt_fork-1.0.2/src/EdgeGPT_fork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-20 18:37:17.000000 edgegpt_fork-1.0.2/src/EdgeGPT_fork.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-20 18:37:17.000000 edgegpt_fork-1.0.2/src/EdgeGPT_fork.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-20 18:37:17.000000 edgegpt_fork-1.0.2/src/EdgeGPT_fork.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:28:24.858449 edgegpt_fork-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-27 12:28:02.000000 edgegpt_fork-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12562 2024-05-27 12:28:24.858449 edgegpt_fork-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11539 2024-05-27 12:28:02.000000 edgegpt_fork-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-27 12:28:24.858449 edgegpt_fork-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-27 12:28:02.000000 edgegpt_fork-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:28:24.850449 edgegpt_fork-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:28:24.854449 edgegpt_fork-1.0.3/src/EdgeGPT/
+-rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-27 12:28:02.000000 edgegpt_fork-1.0.3/src/EdgeGPT/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-05-27 12:28:02.000000 edgegpt_fork-1.0.3/src/EdgeGPT/EdgeUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-27 12:28:02.000000 edgegpt_fork-1.0.3/src/EdgeGPT/ImageGen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-27 12:28:02.000000 edgegpt_fork-1.0.3/src/EdgeGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13661 2024-05-27 12:28:02.000000 edgegpt_fork-1.0.3/src/EdgeGPT/chathub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-27 12:28:02.000000 edgegpt_fork-1.0.3/src/EdgeGPT/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-05-27 12:28:02.000000 edgegpt_fork-1.0.3/src/EdgeGPT/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-27 12:28:02.000000 edgegpt_fork-1.0.3/src/EdgeGPT/conversation_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-27 12:28:02.000000 edgegpt_fork-1.0.3/src/EdgeGPT/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-27 12:28:02.000000 edgegpt_fork-1.0.3/src/EdgeGPT/locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-05-27 12:28:02.000000 edgegpt_fork-1.0.3/src/EdgeGPT/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-27 12:28:02.000000 edgegpt_fork-1.0.3/src/EdgeGPT/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-27 12:28:02.000000 edgegpt_fork-1.0.3/src/EdgeGPT/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-27 12:28:02.000000 edgegpt_fork-1.0.3/src/EdgeGPT/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:28:24.858449 edgegpt_fork-1.0.3/src/EdgeGPT_fork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12562 2024-05-27 12:28:24.000000 edgegpt_fork-1.0.3/src/EdgeGPT_fork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-27 12:28:24.000000 edgegpt_fork-1.0.3/src/EdgeGPT_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:28:24.000000 edgegpt_fork-1.0.3/src/EdgeGPT_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-27 12:28:24.000000 edgegpt_fork-1.0.3/src/EdgeGPT_fork.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-27 12:28:24.000000 edgegpt_fork-1.0.3/src/EdgeGPT_fork.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 12:28:24.000000 edgegpt_fork-1.0.3/src/EdgeGPT_fork.egg-info/top_level.txt
```

### Comparing `edgegpt_fork-1.0.2/LICENSE` & `edgegpt_fork-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegpt_fork-1.0.2/PKG-INFO` & `edgegpt_fork-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT-fork
-Version: 1.0.2
+Version: 1.0.3
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/xingty/EdgeGPT
 Author: Antonio Cheong,Bigbyto
 Author-email: acheong@student.dalat.org,bigbyto@gmail.com
 License: The Unlicense
 Project-URL: Bug Report, https://github.com/xingty/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT-fork Version: 1.0.2 Summary: Reverse
+Metadata-Version: 2.1 Name: EdgeGPT-fork Version: 1.0.3 Summary: Reverse
 engineered Edge Chat API Home-page: https://github.com/xingty/EdgeGPT Author:
 Antonio Cheong,Bigbyto Author-email:
 acheong@student.dalat.org,bigbyto@gmail.com License: The Unlicense Project-URL:
 Bug Report, https://github.com/xingty/EdgeGPT/issues/new Classifier: License ::
 OSI Approved :: The Unlicense (Unlicense) Classifier: Intended Audience ::
 Developers Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `edgegpt_fork-1.0.2/README.md` & `edgegpt_fork-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `edgegpt_fork-1.0.2/setup.py` & `edgegpt_fork-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with Path.open(DOCS_PATH, encoding="utf-8") as f1:
         with Path.open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT-fork",
-    version="1.0.2",
+    version="1.0.3",
     license="The Unlicense",
     author="Antonio Cheong,Bigbyto",
     author_email="acheong@student.dalat.org,bigbyto@gmail.com",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/xingty/EdgeGPT",
```

### Comparing `edgegpt_fork-1.0.2/src/EdgeGPT/EdgeGPT.py` & `edgegpt_fork-1.0.3/src/EdgeGPT/EdgeGPT.py`

 * *Files identical despite different names*

### Comparing `edgegpt_fork-1.0.2/src/EdgeGPT/EdgeUtils.py` & `edgegpt_fork-1.0.3/src/EdgeGPT/EdgeUtils.py`

 * *Files identical despite different names*

### Comparing `edgegpt_fork-1.0.2/src/EdgeGPT/chathub.py` & `edgegpt_fork-1.0.3/src/EdgeGPT/chathub.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
             no_search=no_search,
             persona=persona,
             plugins=plugins,
             image_url=image_url,
         )
         # Send request
         await wss.asend(append_identifier(self.request.struct).encode("utf-8"))
-        resp_txt = ""
+        prefix_txt = ""
         generate = None
         search_refs = []
         search_keywords = []
         async for obj in self._receive_messages(wss):
             if int(time()) % 6 == 0:
                 await wss.asend(append_identifier({"type": 6}).encode("utf-8"))
 
@@ -182,22 +182,22 @@
                         "content_type": message.get("contentType"),
                         "prompt": text
                     }
                 elif msg_type is None:
                     if message.get("contentOrigin") == "Apology":
                         print('message has been revoked')
                         print(message)
-                        resp_txt = f"{resp_txt}{text} -end- (message has been revoked)"
+                        prefix_txt = f"{prefix_txt}{text} -end- (message has been revoked)"
 
                     if len(search_keywords) > 0:
                         keywords = "\n* ".join(search_keywords)
-                        resp_txt = f"{resp_txt}Searching the web for:\n* {keywords}\n\n"
+                        prefix_txt = f"{prefix_txt}Searching the web for:\n* {keywords}\n\n"
                         search_keywords = []
 
-                    yield False, f"{resp_txt}{text}"
+                    yield False, f"{prefix_txt}{text}"
             elif response.get("type") == 2:
                 if response["item"]["result"].get("error"):
                     raise Exception(
                         f"{response['item']['result']['value']}: {response['item']['result']['message']}",
                     )
 
                 response["media"] = {}
@@ -214,24 +214,25 @@
                                 response["media"] = {
                                     "prompt": generate["prompt"],
                                     "images": images
                                 }
                             except Exception as e:
                                 print(str(e))
                                 hint = "Your prompt has been prohibited by third-service. Please modify it."
-                                resp_txt = f"{resp_txt}{text}\n{e}\n{hint}"
+                                prefix_txt = f"{prefix_txt}{text}\n{e}\n{hint}"
 
                 if len(search_refs) > 0:
                     refs_str = ""
                     for index, item in enumerate(search_refs):
                         refs_str += f'- [^{index}^] [{item["title"]}]({item["url"]})\n'
 
-                    resp_txt = f"{resp_txt}{text}\n{refs_str}"
+                    message["text"] = f"{prefix_txt}{text}\n{refs_str}"
+                else:
+                    message["text"] = f"{prefix_txt}{text}"
 
-                message["text"] = resp_txt
                 if "media" not in response:
                     response["media"] = {}
 
                 yield True, response
                 return
 
     async def _initial_handshake(self, wss) -> None:
```

### Comparing `edgegpt_fork-1.0.2/src/EdgeGPT/constants.py` & `edgegpt_fork-1.0.3/src/EdgeGPT/constants.py`

 * *Files identical despite different names*

### Comparing `edgegpt_fork-1.0.2/src/EdgeGPT/conversation.py` & `edgegpt_fork-1.0.3/src/EdgeGPT/conversation.py`

 * *Files identical despite different names*

### Comparing `edgegpt_fork-1.0.2/src/EdgeGPT/conversation_style.py` & `edgegpt_fork-1.0.3/src/EdgeGPT/conversation_style.py`

 * *Files identical despite different names*

### Comparing `edgegpt_fork-1.0.2/src/EdgeGPT/locale.py` & `edgegpt_fork-1.0.3/src/EdgeGPT/locale.py`

 * *Files identical despite different names*

### Comparing `edgegpt_fork-1.0.2/src/EdgeGPT/main.py` & `edgegpt_fork-1.0.3/src/EdgeGPT/main.py`

 * *Files identical despite different names*

### Comparing `edgegpt_fork-1.0.2/src/EdgeGPT/plugin.py` & `edgegpt_fork-1.0.3/src/EdgeGPT/plugin.py`

 * *Files identical despite different names*

### Comparing `edgegpt_fork-1.0.2/src/EdgeGPT/request.py` & `edgegpt_fork-1.0.3/src/EdgeGPT/request.py`

 * *Files identical despite different names*

### Comparing `edgegpt_fork-1.0.2/src/EdgeGPT/utilities.py` & `edgegpt_fork-1.0.3/src/EdgeGPT/utilities.py`

 * *Files identical despite different names*

### Comparing `edgegpt_fork-1.0.2/src/EdgeGPT_fork.egg-info/PKG-INFO` & `edgegpt_fork-1.0.3/src/EdgeGPT_fork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT-fork
-Version: 1.0.2
+Version: 1.0.3
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/xingty/EdgeGPT
 Author: Antonio Cheong,Bigbyto
 Author-email: acheong@student.dalat.org,bigbyto@gmail.com
 License: The Unlicense
 Project-URL: Bug Report, https://github.com/xingty/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT-fork Version: 1.0.2 Summary: Reverse
+Metadata-Version: 2.1 Name: EdgeGPT-fork Version: 1.0.3 Summary: Reverse
 engineered Edge Chat API Home-page: https://github.com/xingty/EdgeGPT Author:
 Antonio Cheong,Bigbyto Author-email:
 acheong@student.dalat.org,bigbyto@gmail.com License: The Unlicense Project-URL:
 Bug Report, https://github.com/xingty/EdgeGPT/issues/new Classifier: License ::
 OSI Approved :: The Unlicense (Unlicense) Classifier: Intended Audience ::
 Developers Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `edgegpt_fork-1.0.2/src/EdgeGPT_fork.egg-info/SOURCES.txt` & `edgegpt_fork-1.0.3/src/EdgeGPT_fork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

