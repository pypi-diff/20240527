# Comparing `tmp/lyyhttpd-1.2.tar.gz` & `tmp/lyyhttpd-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyyhttpd-1.2.tar", last modified: Wed May  1 15:19:14 2024, max compression
+gzip compressed data, was "lyyhttpd-1.3.tar", last modified: Mon May 27 10:28:30 2024, max compression
```

## Comparing `lyyhttpd-1.2.tar` & `lyyhttpd-1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 15:19:14.429288 lyyhttpd-1.2/
--rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyyhttpd-1.2/LICENSE
--rw-rw-rw-   0        0        0      145 2024-05-01 15:19:14.428785 lyyhttpd-1.2/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyyhttpd-1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 15:19:14.426782 lyyhttpd-1.2/lyyhttpd.egg-info/
--rw-rw-rw-   0        0        0      145 2024-05-01 15:19:14.000000 lyyhttpd-1.2/lyyhttpd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-05-01 15:19:14.000000 lyyhttpd-1.2/lyyhttpd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 15:19:14.000000 lyyhttpd-1.2/lyyhttpd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-01 15:19:14.000000 lyyhttpd-1.2/lyyhttpd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-01 15:19:14.000000 lyyhttpd-1.2/lyyhttpd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4871 2024-05-01 15:19:02.000000 lyyhttpd-1.2/lyyhttpd.py
--rw-rw-rw-   0        0        0       42 2024-05-01 15:19:14.429288 lyyhttpd-1.2/setup.cfg
--rw-rw-rw-   0        0        0      270 2024-05-01 15:19:13.000000 lyyhttpd-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:28:30.200840 lyyhttpd-1.3/
+-rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyyhttpd-1.3/LICENSE
+-rw-rw-rw-   0        0        0      172 2024-05-27 10:28:30.198839 lyyhttpd-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyyhttpd-1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 10:28:30.196840 lyyhttpd-1.3/lyyhttpd.egg-info/
+-rw-rw-rw-   0        0        0      172 2024-05-27 10:28:30.000000 lyyhttpd-1.3/lyyhttpd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-05-27 10:28:30.000000 lyyhttpd-1.3/lyyhttpd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 10:28:30.000000 lyyhttpd-1.3/lyyhttpd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-27 10:28:30.000000 lyyhttpd-1.3/lyyhttpd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-27 10:28:30.000000 lyyhttpd-1.3/lyyhttpd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4831 2024-05-27 10:28:23.000000 lyyhttpd-1.3/lyyhttpd.py
+-rw-rw-rw-   0        0        0       42 2024-05-27 10:28:30.200840 lyyhttpd-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      270 2024-05-27 10:28:29.000000 lyyhttpd-1.3/setup.py
```

### Comparing `lyyhttpd-1.2/LICENSE` & `lyyhttpd-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lyyhttpd-1.2/lyyhttpd.py` & `lyyhttpd-1.3/lyyhttpd.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # http_server.py
-from fastapi import FastAPI, Request,HTTPException
+from fastapi import FastAPI, Request,HTTPException, Query
 from typing import Callable
 import queue
 from starlette.responses import Response
-from f1999 import handle_root, handle_showmsg, handle_path2, show_reason  # 确保从正确的模块导入你的处理函数
 
 
 from flask import Flask,request,Response,send_file
 
 def flask_app(ip="127.0.0.1",port=8080,queue=None):
     app = Flask(__name__)
 
@@ -39,35 +38,39 @@
         queue.put(data)
         return 'ok', 200
         # df["msgtype"] = "showsql"
         # json_text_list = df.iloc[::-1].apply(lambda row: json.dumps({k: (v.strftime("%Y-%m-%d %H:%M:%S") if isinstance(v, datetime) else v) for k, v in row.to_dict().items()}), axis=1).to_list()
         # data = json.dumps(json_text_list)
         # send_post_request("http://127.0.0.1:8088/showmsg",data=data, headers={'Content-Type': 'application/json'})
 
+    @app.get("/showmsg")
+    async def showmsg_get(code: Query(None), cmd: Query(None)):
+        # 检查是否提供了 code 和 cmd 参数
+        if code is None or cmd is None:
+            return {"error": "Missing code or cmd parameter"}
+
+        # 将数据放入队列
+        data = {"code": code, "cmd": cmd}
+        print("showmsg_get", data)
+        queue.put(data)
+        
+        # 直接返回字典作为响应
+        return {"message": "Data received", "data": data}
     @app.route('/{path_param}', methods=['GET', 'POST'])
     def route_handler(path_param):
         print(f"get /{path_param}")        
         return Response("Hello, World!")
     
     @app.errorhandler(404)
     def page_not_found(e):
         print(f"{request.method} request: {request.path} with args {dict(request.args)}, but not found")
         return "lyy404 Not Found", 404
     return app
 
 
-# 定义一个字典，映射路径参数到不同的处理函数
-path_to_handler: dict[str, Callable[[str, queue.Queue], Response]] = {
-    "root": handle_root,
-    "showmsg": lambda data, queue: handle_showmsg(data, queue),
-    "path2": lambda data, queue: handle_path2(data, queue),
-    "reason": lambda data, queue: show_reason(data, queue),
-    # 可以根据需要添加更多的路径和处理函数
-}
-
 def lyyfastapi_multi(path_to_handler: dict[str, Callable[[str, queue.Queue], Response]], fastapi_queue: queue.Queue) -> FastAPI:
     app = FastAPI()
 
     @app.get("/favicon.ico")
     async def favicon():
         return Response(content="", media_type="image/x-icon")
```

