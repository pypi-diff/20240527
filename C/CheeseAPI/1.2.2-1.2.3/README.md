# Comparing `tmp/cheeseapi-1.2.2.tar.gz` & `tmp/cheeseapi-1.2.3.tar.gz`

## Comparing `cheeseapi-1.2.2.tar` & `cheeseapi-1.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/__init__.py
--rw-r--r--   0        0        0     7512 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/app.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/cors.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/exception.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/file.py
--rw-r--r--   0        0        0    33034 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/handle.py
--rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/protocol.py
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/request.py
--rw-r--r--   0        0        0    17620 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/response.py
--rw-r--r--   0        0        0    13136 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/route.py
--rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/schedule.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/server.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/signal.py
--rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/text.py
--rw-r--r--   0        0        0    12949 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/validator.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/websocket.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/CheeseAPI/workspace.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/LICENSE
--rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 cheeseapi-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/__init__.py
+-rw-r--r--   0        0        0     7512 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/app.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/cors.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/exception.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/file.py
+-rw-r--r--   0        0        0    33258 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/handle.py
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/protocol.py
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/request.py
+-rw-r--r--   0        0        0    17620 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/response.py
+-rw-r--r--   0        0        0    13136 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/route.py
+-rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/schedule.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/server.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/signal.py
+-rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/text.py
+-rw-r--r--   0        0        0    13085 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/validator.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/websocket.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/workspace.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/LICENSE
+-rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/PKG-INFO
```

### Comparing `cheeseapi-1.2.2/CheeseAPI/app.py` & `cheeseapi-1.2.3/CheeseAPI/app.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.2/CheeseAPI/cors.py` & `cheeseapi-1.2.3/CheeseAPI/cors.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.2/CheeseAPI/exception.py` & `cheeseapi-1.2.3/CheeseAPI/exception.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.2/CheeseAPI/file.py` & `cheeseapi-1.2.3/CheeseAPI/file.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.2/CheeseAPI/handle.py` & `cheeseapi-1.2.3/CheeseAPI/handle.py`

 * *Files 1% similar despite different names*

```diff
@@ -476,43 +476,46 @@
             logger.http(text[0], text[1])
 
     async def websocket_request(self, protocol: 'WebsocketProtocol'):
         try:
             try:
                 Server, kwargs = self._app.routeBus._match(protocol.request.path, 'WEBSOCKET')
                 protocol.kwargs.update(kwargs)
-            except KeyError as e:
+            except Route_404_Exception as e:
                 await self.websocket_afterRequest(protocol)
                 if self._app.signal.websocket_afterRequest.receivers:
                     await self._app.signal.websocket_afterRequest.async_send(**{
                         'request': protocol.request,
                         **protocol.kwargs
                     })
 
-                if e.args[0] == 0:
-                    await self.websocket_404(protocol)
-                    if self._app.signal.websocket_404.receivers:
-                        await self._app.signal.websocket_404.async_send(**{
-                            'request': protocol.request,
-                            'response': protocol.response,
-                            **protocol.kwargs
-                        })
-                    return await self.websocket_response(protocol)
-
-                elif e.args[0] == 1:
-                    await self.websocket_405(protocol)
-                    if self._app.signal.websocket_405.receivers:
-                        await self._app.signal.websocket_405.async_send(**{
-                            'request': protocol.request,
-                            'response': protocol.response,
-                            **protocol.kwargs
-                        })
-                    return await self.websocket_response(protocol)
+                await self.websocket_404(protocol)
+                if self._app.signal.websocket_404.receivers:
+                    await self._app.signal.websocket_404.async_send(**{
+                        'request': protocol.request,
+                        'response': protocol.response,
+                        **protocol.kwargs
+                    })
+                return await self.websocket_response(protocol)
+            except Route_405_Exception as e:
+                await self.websocket_afterRequest(protocol)
+                if self._app.signal.websocket_afterRequest.receivers:
+                    await self._app.signal.websocket_afterRequest.async_send(**{
+                        'request': protocol.request,
+                        **protocol.kwargs
+                    })
 
-                raise e
+                await self.websocket_405(protocol)
+                if self._app.signal.websocket_405.receivers:
+                    await self._app.signal.websocket_405.async_send(**{
+                        'request': protocol.request,
+                        'response': protocol.response,
+                        **protocol.kwargs
+                    })
+                return await self.websocket_response(protocol)
 
             protocol.server = Server()
 
             await self.websocket_afterRequest(protocol)
             if self._app.signal.websocket_afterRequest.receivers:
                 await self._app.signal.websocket_afterRequest.async_send(**{
                     'request': protocol.request,
```

### Comparing `cheeseapi-1.2.2/CheeseAPI/protocol.py` & `cheeseapi-1.2.3/CheeseAPI/protocol.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.2/CheeseAPI/request.py` & `cheeseapi-1.2.3/CheeseAPI/request.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.2/CheeseAPI/response.py` & `cheeseapi-1.2.3/CheeseAPI/response.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.2/CheeseAPI/route.py` & `cheeseapi-1.2.3/CheeseAPI/route.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.2/CheeseAPI/schedule.py` & `cheeseapi-1.2.3/CheeseAPI/schedule.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.2/CheeseAPI/server.py` & `cheeseapi-1.2.3/CheeseAPI/server.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.2/CheeseAPI/signal.py` & `cheeseapi-1.2.3/CheeseAPI/signal.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.2/CheeseAPI/text.py` & `cheeseapi-1.2.3/CheeseAPI/text.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.2/CheeseAPI/validator.py` & `cheeseapi-1.2.3/CheeseAPI/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,18 @@
                 validatedForm[f'{self.scope}.{self.key}'] = kwargs[self.key]
             else:
                 validatedForm[f'{self.scope}.{self.key}'] = (getattr(request, self.scope) or {}).get(self.key)
 
         if validatedForm[f'{self.scope}.{self.key}'] is None:
             if self.required:
                 raise ValidateError(self.response or Response(app._text.validator_requiredMessage(self.scope, self.key), 400))
-            validatedForm[f'{self.scope}.{self.key}'] = self.default
+            if callable(self.default):
+                validatedForm[f'{self.scope}.{self.key}'] = self.default()
+            else:
+                validatedForm[f'{self.scope}.{self.key}'] = self.default
 
         if validatedForm[f'{self.scope}.{self.key}'] is not None:
             if self.type is not None:
                 try:
                     if isinstance(self.type, list):
                         for type in self.type:
                             validatedForm[f'{self.scope}.{self.key}'] = type(validatedForm[f'{self.scope}.{self.key}'])
```

### Comparing `cheeseapi-1.2.2/CheeseAPI/websocket.py` & `cheeseapi-1.2.3/CheeseAPI/websocket.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.2/CheeseAPI/workspace.py` & `cheeseapi-1.2.3/CheeseAPI/workspace.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.2/LICENSE` & `cheeseapi-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.2/README.md` & `cheeseapi-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.2/pyproject.toml` & `cheeseapi-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "hatchling" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "CheeseAPI"
-version = "1.2.2"
+version = "1.2.3"
 description = "一款web协程框架。"
 readme = "README.md"
 license-files = { paths = [ "LICENSE" ] }
 authors = [
     { name = "Cheese Unknown", email = "cheese@cheese.ren" }
 ]
 keywords = [ 'API', 'BackEnd' ]
```

### Comparing `cheeseapi-1.2.2/PKG-INFO` & `cheeseapi-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: CheeseAPI
-Version: 1.2.2
+Version: 1.2.3
 Summary: 一款web协程框架。
 Project-URL: Source, https://github.com/CheeseUnknown/CheeseAPI
 Author-email: Cheese Unknown <cheese@cheese.ren>
 License-File: LICENSE
 Keywords: API,BackEnd
 Requires-Dist: cheeselog==1.0.*
 Requires-Dist: cheesesignal==1.1.*
```

