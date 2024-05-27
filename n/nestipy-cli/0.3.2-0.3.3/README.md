# Comparing `tmp/nestipy_cli-0.3.2.tar.gz` & `tmp/nestipy_cli-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy_cli-0.3.2.tar", max compression
+gzip compressed data, was "nestipy_cli-0.3.3.tar", max compression
```

## Comparing `nestipy_cli-0.3.2.tar` & `nestipy_cli-0.3.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1906 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/README.md
--rw-r--r--   0        0        0      646 2024-05-24 13:49:57.822062 nestipy_cli-0.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/__init__.py
--rw-r--r--   0        0        0     2769 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/cli.py
--rw-r--r--   0        0        0     5054 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/handler.py
--rw-r--r--   0        0        0      502 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/style.py
--rw-r--r--   0        0        0        0 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/__init__.py
--rw-r--r--   0        0        0      184 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2906 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/__pycache__/generator.cpython-311.pyc
--rw-r--r--   0        0        0     1068 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/generator.py
--rw-r--r--   0        0        0       56 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/project/.gitignore
--rw-r--r--   0        0        0      988 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/project/README.md
--rw-r--r--   0        0        0        0 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/project/__init__.py
--rw-r--r--   0        0        0      192 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/project/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1301 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/project/__pycache__/app_service.cpython-311.pyc
--rw-r--r--   0        0        0      805 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/project/app_controller.py
--rw-r--r--   0        0        0      209 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/project/app_module.py
--rw-r--r--   0        0        0      376 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/project/app_service.py
--rw-r--r--   0        0        0      225 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/project/main.py
--rw-r--r--   0        0        0        7 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/project/requirements.txt
--rw-r--r--   0        0        0        0 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/project/src/__init__.py
--rw-r--r--   0        0        0     1210 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/views/controller.txt
--rw-r--r--   0        0        0      187 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/views/dto.txt
--rw-r--r--   0        0        0      311 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/views/graphql_module.txt
--rw-r--r--   0        0        0      294 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/views/graphql_service.txt
--rw-r--r--   0        0        0      102 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/views/input.txt
--rw-r--r--   0        0        0      312 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/views/module.txt
--rw-r--r--   0        0        0      618 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/views/resolver.txt
--rw-r--r--   0        0        0      471 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/views/service.txt
--rw-r--r--   0        0        0      168 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/views/single_controller.txt
--rw-r--r--   0        0        0       86 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/views/single_module.txt
--rw-r--r--   0        0        0      303 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/views/single_resolver.txt
--rw-r--r--   0        0        0      127 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/views/single_service.txt
--rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 nestipy_cli-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1906 2024-05-27 13:22:21.064712 nestipy_cli-0.3.3/README.md
+-rw-r--r--   0        0        0      646 2024-05-27 13:22:30.716674 nestipy_cli-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-27 13:22:21.064712 nestipy_cli-0.3.3/src/nestipy_cli/__init__.py
+-rw-r--r--   0        0        0     2769 2024-05-27 13:22:21.064712 nestipy_cli-0.3.3/src/nestipy_cli/cli.py
+-rw-r--r--   0        0        0     5054 2024-05-27 13:22:21.064712 nestipy_cli-0.3.3/src/nestipy_cli/handler.py
+-rw-r--r--   0        0        0      502 2024-05-27 13:22:21.064712 nestipy_cli-0.3.3/src/nestipy_cli/style.py
+-rw-r--r--   0        0        0        0 2024-05-27 13:22:21.064712 nestipy_cli-0.3.3/src/nestipy_cli/templates/__init__.py
+-rw-r--r--   0        0        0      184 2024-05-27 13:22:21.064712 nestipy_cli-0.3.3/src/nestipy_cli/templates/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2906 2024-05-27 13:22:21.064712 nestipy_cli-0.3.3/src/nestipy_cli/templates/__pycache__/generator.cpython-311.pyc
+-rw-r--r--   0        0        0     1068 2024-05-27 13:22:21.064712 nestipy_cli-0.3.3/src/nestipy_cli/templates/generator.py
+-rw-r--r--   0        0        0       56 2024-05-27 13:22:21.064712 nestipy_cli-0.3.3/src/nestipy_cli/templates/project/.gitignore
+-rw-r--r--   0        0        0      988 2024-05-27 13:22:21.064712 nestipy_cli-0.3.3/src/nestipy_cli/templates/project/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 13:22:21.064712 nestipy_cli-0.3.3/src/nestipy_cli/templates/project/__init__.py
+-rw-r--r--   0        0        0      192 2024-05-27 13:22:21.064712 nestipy_cli-0.3.3/src/nestipy_cli/templates/project/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1301 2024-05-27 13:22:21.064712 nestipy_cli-0.3.3/src/nestipy_cli/templates/project/__pycache__/app_service.cpython-311.pyc
+-rw-r--r--   0        0        0      802 2024-05-27 13:22:21.064712 nestipy_cli-0.3.3/src/nestipy_cli/templates/project/app_controller.py
+-rw-r--r--   0        0        0      209 2024-05-27 13:22:21.064712 nestipy_cli-0.3.3/src/nestipy_cli/templates/project/app_module.py
+-rw-r--r--   0        0        0      376 2024-05-27 13:22:21.064712 nestipy_cli-0.3.3/src/nestipy_cli/templates/project/app_service.py
+-rw-r--r--   0        0        0      225 2024-05-27 13:22:21.064712 nestipy_cli-0.3.3/src/nestipy_cli/templates/project/main.py
+-rw-r--r--   0        0        0        7 2024-05-27 13:22:21.064712 nestipy_cli-0.3.3/src/nestipy_cli/templates/project/requirements.txt
+-rw-r--r--   0        0        0        0 2024-05-27 13:22:21.064712 nestipy_cli-0.3.3/src/nestipy_cli/templates/project/src/__init__.py
+-rw-r--r--   0        0        0     1207 2024-05-27 13:22:21.064712 nestipy_cli-0.3.3/src/nestipy_cli/templates/views/controller.txt
+-rw-r--r--   0        0        0      187 2024-05-27 13:22:21.068712 nestipy_cli-0.3.3/src/nestipy_cli/templates/views/dto.txt
+-rw-r--r--   0        0        0      311 2024-05-27 13:22:21.068712 nestipy_cli-0.3.3/src/nestipy_cli/templates/views/graphql_module.txt
+-rw-r--r--   0        0        0      294 2024-05-27 13:22:21.068712 nestipy_cli-0.3.3/src/nestipy_cli/templates/views/graphql_service.txt
+-rw-r--r--   0        0        0      102 2024-05-27 13:22:21.068712 nestipy_cli-0.3.3/src/nestipy_cli/templates/views/input.txt
+-rw-r--r--   0        0        0      312 2024-05-27 13:22:21.068712 nestipy_cli-0.3.3/src/nestipy_cli/templates/views/module.txt
+-rw-r--r--   0        0        0      641 2024-05-27 13:22:21.068712 nestipy_cli-0.3.3/src/nestipy_cli/templates/views/resolver.txt
+-rw-r--r--   0        0        0      471 2024-05-27 13:22:21.068712 nestipy_cli-0.3.3/src/nestipy_cli/templates/views/service.txt
+-rw-r--r--   0        0        0      168 2024-05-27 13:22:21.068712 nestipy_cli-0.3.3/src/nestipy_cli/templates/views/single_controller.txt
+-rw-r--r--   0        0        0       86 2024-05-27 13:22:21.068712 nestipy_cli-0.3.3/src/nestipy_cli/templates/views/single_module.txt
+-rw-r--r--   0        0        0      379 2024-05-27 13:22:21.068712 nestipy_cli-0.3.3/src/nestipy_cli/templates/views/single_resolver.txt
+-rw-r--r--   0        0        0      127 2024-05-27 13:22:21.068712 nestipy_cli-0.3.3/src/nestipy_cli/templates/views/single_service.txt
+-rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 nestipy_cli-0.3.3/PKG-INFO
```

### Comparing `nestipy_cli-0.3.2/README.md` & `nestipy_cli-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `nestipy_cli-0.3.2/pyproject.toml` & `nestipy_cli-0.3.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nestipy-cli"
-version = "0.3.2"
+version = "0.3.3"
 description = "Nestipy is a Python framework built on top of FastAPI that follows the modular architecture of NestJS"
 authors = ["tsiresymila <tsiresymila@gmail.com>"]
 readme = "README.md"
 packages = [{include = "nestipy_cli", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `nestipy_cli-0.3.2/src/nestipy_cli/cli.py` & `nestipy_cli-0.3.3/src/nestipy_cli/cli.py`

 * *Files identical despite different names*

### Comparing `nestipy_cli-0.3.2/src/nestipy_cli/handler.py` & `nestipy_cli-0.3.3/src/nestipy_cli/handler.py`

 * *Files identical despite different names*

### Comparing `nestipy_cli-0.3.2/src/nestipy_cli/templates/__pycache__/generator.cpython-311.pyc` & `nestipy_cli-0.3.3/src/nestipy_cli/templates/__pycache__/generator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy_cli-0.3.2/src/nestipy_cli/templates/generator.py` & `nestipy_cli-0.3.3/src/nestipy_cli/templates/generator.py`

 * *Files identical despite different names*

### Comparing `nestipy_cli-0.3.2/src/nestipy_cli/templates/project/README.md` & `nestipy_cli-0.3.3/src/nestipy_cli/templates/project/README.md`

 * *Files identical despite different names*

### Comparing `nestipy_cli-0.3.2/src/nestipy_cli/templates/project/__pycache__/app_service.cpython-311.pyc` & `nestipy_cli-0.3.3/src/nestipy_cli/templates/project/__pycache__/app_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy_cli-0.3.2/src/nestipy_cli/templates/project/app_controller.py` & `nestipy_cli-0.3.3/src/nestipy_cli/templates/project/app_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Annotated
 
 from nestipy.common import Controller, Get, Post, Put, Delete
-from nestipy.ioc import Inject, Body, Params
+from nestipy.ioc import Inject, Body, Param
 
 from app_service import AppService
 
 
 @Controller()
 class AppController:
     service: Annotated[AppService, Inject()]
@@ -15,13 +15,13 @@
         return await self.service.get()
 
     @Post()
     async def post(self, data: Annotated[dict, Body()]) -> str:
         return await self.service.post(data=data)
 
     @Put('/{app_id}')
-    async def put(self, app_id: Annotated[int, Params('app_id')], data: Annotated[dict, Body()]) -> str:
+    async def put(self, app_id: Annotated[int, Param('app_id')], data: Annotated[dict, Body()]) -> str:
         return await self.service.put(id_=app_id, data=data)
 
     @Delete('/{app_id}')
-    async def delete(self, app_id: Annotated[int, Params('app_id')]) -> None:
+    async def delete(self, app_id: Annotated[int, Param('app_id')]) -> None:
         await self.service.delete(id_=app_id)
```

### Comparing `nestipy_cli-0.3.2/src/nestipy_cli/templates/views/controller.txt` & `nestipy_cli-0.3.3/src/nestipy_cli/templates/views/controller.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Annotated
 
 from nestipy.common import Controller, Get, Post, Put, Delete
-from nestipy.ioc import Inject, Body, Params
+from nestipy.ioc import Inject, Body, Param
 
 from .{{name|lower}}_dto import Create{{name|capitalize}}Dto, Update{{name|capitalize}}Dto
 from .{{name|lower}}_service import {{name|capitalize}}Service
 
 
 @Controller('{{name|lower}}s')
 class {{name|capitalize}}Controller:
@@ -17,13 +17,13 @@
         return await self.{{name|lower}}_service.list()
 
     @Post()
     async def create(self, data: Annotated[Create{{name|capitalize}}Dto, Body()]) -> str:
         return await self.{{name|lower}}_service.create(data)
 
     @Put('/{{'{'}}{{name|lower}}{{'_id}'}}')
-    async def update(self, {{name|lower}}_id: Annotated[int, Params('{{name|lower}}_id')], data: Annotated[Update{{name|capitalize}}Dto, Body()]) -> str:
+    async def update(self, {{name|lower}}_id: Annotated[int, Param('{{name|lower}}_id')], data: Annotated[Update{{name|capitalize}}Dto, Body()]) -> str:
         return await self.{{name|lower}}_service.update({{name|lower}}_id, data)
 
     @Delete('/{{'{'}}{{name|lower}}{{'_id}'}}')
-    async def delete(self, {{name|lower}}_id: Annotated[int,Params('{{name|lower}}_id')] ) -> None:
+    async def delete(self, {{name|lower}}_id: Annotated[int,Param('{{name|lower}}_id')] ) -> None:
         return await self.{{name|lower}}_service.delete({{name|lower}}_id)
```

### Comparing `nestipy_cli-0.3.2/PKG-INFO` & `nestipy_cli-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestipy-cli
-Version: 0.3.2
+Version: 0.3.3
 Summary: Nestipy is a Python framework built on top of FastAPI that follows the modular architecture of NestJS
 Author: tsiresymila
 Author-email: tsiresymila@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nestipy-cli Version: 0.3.2 Summary: Nestipy is a
+Metadata-Version: 2.1 Name: nestipy-cli Version: 0.3.3 Summary: Nestipy is a
 Python framework built on top of FastAPI that follows the modular architecture
 of NestJS Author: tsiresymila Author-email: tsiresymila@gmail.com Requires-
 Python: >=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Dist: aiofile (>=3.8.8,<4.0.0) Requires-Dist: autoflake (>=2.3.1,<3.0.0)
 Requires-Dist: autopep8 (>=2.1.0,<3.0.0) Requires-Dist: click (>=8.1.7,<9.0.0)
```

