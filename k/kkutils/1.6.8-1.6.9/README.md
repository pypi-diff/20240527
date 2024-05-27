# Comparing `tmp/kkutils-1.6.8.tar.gz` & `tmp/kkutils-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kkutils-1.6.8.tar", last modified: Sun Mar 24 10:57:03 2024, max compression
+gzip compressed data, was "kkutils-1.6.9.tar", last modified: Mon May 27 08:23:02 2024, max compression
```

## Comparing `kkutils-1.6.8.tar` & `kkutils-1.6.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 10:57:03.122549 kkutils-1.6.8/
--rw-r--r--   0 root         (0) root         (0)      703 2024-03-24 10:57:03.122549 kkutils-1.6.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 10:57:03.122549 kkutils-1.6.8/kkutils.egg-info/
--rw-r--r--   0 root         (0) root         (0)      703 2024-03-24 10:57:03.000000 kkutils-1.6.8/kkutils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      619 2024-03-24 10:57:03.000000 kkutils-1.6.8/kkutils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-24 10:57:03.000000 kkutils-1.6.8/kkutils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      260 2024-03-24 10:57:03.000000 kkutils-1.6.8/kkutils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-03-24 10:57:03.000000 kkutils-1.6.8/kkutils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3985 2024-03-05 03:08:57.000000 kkutils-1.6.8/processor.py
--rw-r--r--   0 root         (0) root         (0)      245 2023-03-04 16:36:32.000000 kkutils-1.6.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-24 10:57:03.122549 kkutils-1.6.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1190 2024-03-24 10:45:59.000000 kkutils-1.6.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 10:57:03.122549 kkutils-1.6.8/tornado_utils/
--rw-r--r--   0 root         (0) root         (0)      408 2024-03-05 03:08:57.000000 kkutils-1.6.8/tornado_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6036 2024-03-24 10:52:44.000000 kkutils-1.6.8/tornado_utils/application.py
--rw-r--r--   0 root         (0) root         (0)    11012 2024-03-24 08:37:31.000000 kkutils-1.6.8/tornado_utils/basehandler.py
--rw-r--r--   0 root         (0) root         (0)    14578 2024-03-15 10:58:15.000000 kkutils-1.6.8/tornado_utils/userhandler.py
--rw-r--r--   0 root         (0) root         (0)     3803 2024-03-05 03:08:57.000000 kkutils-1.6.8/tornado_utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 10:57:03.122549 kkutils-1.6.8/utils/
--rw-r--r--   0 root         (0) root         (0)     1964 2024-03-11 10:41:32.000000 kkutils-1.6.8/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10568 2024-03-05 03:17:09.000000 kkutils-1.6.8/utils/base_utils.py
--rw-r--r--   0 root         (0) root         (0)     4219 2024-03-05 03:08:57.000000 kkutils-1.6.8/utils/cached_property.py
--rw-r--r--   0 root         (0) root         (0)     5562 2024-03-05 03:08:57.000000 kkutils-1.6.8/utils/config_utils.py
--rw-r--r--   0 root         (0) root         (0)     2749 2024-03-05 03:08:57.000000 kkutils-1.6.8/utils/crypto.py
--rw-r--r--   0 root         (0) root         (0)    10699 2024-03-05 03:08:57.000000 kkutils-1.6.8/utils/curl_utils.py
--rw-r--r--   0 root         (0) root         (0)    15860 2024-03-13 04:52:53.000000 kkutils-1.6.8/utils/db_utils.py
--rw-r--r--   0 root         (0) root         (0)     2078 2024-03-05 03:08:57.000000 kkutils-1.6.8/utils/decorator.py
--rw-r--r--   0 root         (0) root         (0)     3718 2024-03-05 03:08:57.000000 kkutils-1.6.8/utils/email_utils.py
--rw-r--r--   0 root         (0) root         (0)     1182 2024-03-05 03:08:57.000000 kkutils-1.6.8/utils/fire.py
--rw-r--r--   0 root         (0) root         (0)    26557 2024-03-05 03:08:57.000000 kkutils-1.6.8/utils/http_utils.py
--rw-r--r--   0 root         (0) root         (0)     2688 2024-03-05 03:08:57.000000 kkutils-1.6.8/utils/log_utils.py
--rw-r--r--   0 root         (0) root         (0)     6167 2024-03-13 04:49:29.000000 kkutils-1.6.8/utils/rabbitmq.py
--rw-r--r--   0 root         (0) root         (0)     1083 2024-03-05 03:08:57.000000 kkutils-1.6.8/utils/stopwatch.py
--rw-r--r--   0 root         (0) root         (0)     5796 2024-03-05 03:08:57.000000 kkutils-1.6.8/utils/xdb_searcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:23:02.422402 kkutils-1.6.9/
+-rw-r--r--   0 root         (0) root         (0)      703 2024-05-27 08:23:02.422402 kkutils-1.6.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:23:02.418402 kkutils-1.6.9/kkutils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      703 2024-05-27 08:23:02.000000 kkutils-1.6.9/kkutils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      619 2024-05-27 08:23:02.000000 kkutils-1.6.9/kkutils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 08:23:02.000000 kkutils-1.6.9/kkutils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      260 2024-05-27 08:23:02.000000 kkutils-1.6.9/kkutils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-27 08:23:02.000000 kkutils-1.6.9/kkutils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3985 2024-03-05 03:08:57.000000 kkutils-1.6.9/processor.py
+-rw-r--r--   0 root         (0) root         (0)      245 2023-03-04 16:36:32.000000 kkutils-1.6.9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 08:23:02.422402 kkutils-1.6.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1190 2024-05-27 08:22:07.000000 kkutils-1.6.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:23:02.418402 kkutils-1.6.9/tornado_utils/
+-rw-r--r--   0 root         (0) root         (0)      408 2024-03-05 03:08:57.000000 kkutils-1.6.9/tornado_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6105 2024-05-27 08:22:58.000000 kkutils-1.6.9/tornado_utils/application.py
+-rw-r--r--   0 root         (0) root         (0)    11012 2024-04-08 03:16:00.000000 kkutils-1.6.9/tornado_utils/basehandler.py
+-rw-r--r--   0 root         (0) root         (0)    14678 2024-04-08 03:16:00.000000 kkutils-1.6.9/tornado_utils/userhandler.py
+-rw-r--r--   0 root         (0) root         (0)     3782 2024-05-25 09:06:00.000000 kkutils-1.6.9/tornado_utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:23:02.422402 kkutils-1.6.9/utils/
+-rw-r--r--   0 root         (0) root         (0)     2098 2024-05-08 03:16:58.000000 kkutils-1.6.9/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10952 2024-05-08 02:43:45.000000 kkutils-1.6.9/utils/base_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2024-03-05 03:08:57.000000 kkutils-1.6.9/utils/cached_property.py
+-rw-r--r--   0 root         (0) root         (0)     5562 2024-03-05 03:08:57.000000 kkutils-1.6.9/utils/config_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3339 2024-05-07 15:28:29.000000 kkutils-1.6.9/utils/crypto.py
+-rw-r--r--   0 root         (0) root         (0)    10699 2024-03-05 03:08:57.000000 kkutils-1.6.9/utils/curl_utils.py
+-rw-r--r--   0 root         (0) root         (0)    15861 2024-04-02 03:25:29.000000 kkutils-1.6.9/utils/db_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2024-03-05 03:08:57.000000 kkutils-1.6.9/utils/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     3718 2024-03-05 03:08:57.000000 kkutils-1.6.9/utils/email_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1182 2024-03-05 03:08:57.000000 kkutils-1.6.9/utils/fire.py
+-rw-r--r--   0 root         (0) root         (0)    26557 2024-03-05 03:08:57.000000 kkutils-1.6.9/utils/http_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2688 2024-03-05 03:08:57.000000 kkutils-1.6.9/utils/log_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6167 2024-03-13 04:49:29.000000 kkutils-1.6.9/utils/rabbitmq.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-03-05 03:08:57.000000 kkutils-1.6.9/utils/stopwatch.py
+-rw-r--r--   0 root         (0) root         (0)     5796 2024-03-05 03:08:57.000000 kkutils-1.6.9/utils/xdb_searcher.py
```

### Comparing `kkutils-1.6.8/PKG-INFO` & `kkutils-1.6.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kkutils
-Version: 1.6.8
+Version: 1.6.9
 Summary: python utils
 Home-page: https://www.ishield.cn
 Author: digua
 Author-email: zkdfbb@qq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `kkutils-1.6.8/kkutils.egg-info/PKG-INFO` & `kkutils-1.6.9/kkutils.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kkutils
-Version: 1.6.8
+Version: 1.6.9
 Summary: python utils
 Home-page: https://www.ishield.cn
 Author: digua
 Author-email: zkdfbb@qq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `kkutils-1.6.8/kkutils.egg-info/SOURCES.txt` & `kkutils-1.6.9/kkutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.8/processor.py` & `kkutils-1.6.9/processor.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.8/setup.py` & `kkutils-1.6.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Last modified: 2019-04-07 00:07:43
 '''
 
 from setuptools import setup
 
 setup(
     name="kkutils",
-    version="1.6.8",
+    version="1.6.9",
     description="python utils",
     author="digua",
     author_email="zkdfbb@qq.com",
     url="https://www.ishield.cn",
     license="MIT",
     python_requires='>=3.6',
     data_files=[('', ['requirements.txt'])],
```

### Comparing `kkutils-1.6.8/tornado_utils/application.py` & `kkutils-1.6.9/tornado_utils/application.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 
 """Tornado Blueprint蓝图的实现。"""
 import asyncio
 import collections
 import inspect
 import signal
+from concurrent.futures import ThreadPoolExecutor
 
 import tornado.netutil
 import tornado.process
 import tornado.web
 from tornado.httpserver import HTTPServer
 from tornado.ioloop import IOLoop
 from tornado.options import define, options
@@ -80,14 +81,15 @@
 
     def __init__(self, name=None, url_prefix='/', host='.*', strict_slashes=False, **kwargs):
         super().__init__(name, url_prefix, host, strict_slashes)
         self.options = options
         self.prefix = 'web'
         self.logger = Logger()
         self.loop = IOLoop.current().asyncio_loop
+        self.executor = ThreadPoolExecutor(10)
         self._kwargs = kwargs
         self._handlers = []
         self._cache = Cache()
         self._events = collections.defaultdict(list)
         options.parse_command_line()
 
     def register(self, *blueprints, url_prefix='/'):
@@ -121,16 +123,15 @@
         for func in self._events['before_server_stop']:
             ret = func(self)
             if inspect.isawaitable(ret):
                 await ret
 
         self.server.stop()
         self.logger.info('shutting down')
-        # tasks = [task for task in asyncio.Task.all_tasks() if task is not
-        #          asyncio.tasks.Task.current_task()]
+        # tasks = [x for x in asyncio.Task.all_tasks() if x is not asyncio.tasks.Task.current_task()]
         # self.logger.warning(f'canceling {len(tasks)} pending tasks')
         # if tasks:
         #     asyncio.gather(*tasks, return_exceptions=True).cancel()
         IOLoop.current().stop()
 
     def sig_handler(self, sig, frame):
         self.logger.warning(f'received signal {sig}')
```

### Comparing `kkutils-1.6.8/tornado_utils/basehandler.py` & `kkutils-1.6.9/tornado_utils/basehandler.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.8/tornado_utils/userhandler.py` & `kkutils-1.6.9/tornado_utils/userhandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,14 +252,16 @@
 
     async def put(self):
         self.logger.info(f'new user: {self.args}')
         if not self.args.unionId:
             return self.finish({'err': 1, 'msg': '未获取到用户'})
 
         user = None
+        if self.args.token and len(self.args.token) != 32:
+            self.args.pop('token', None)
         if self.args.token:
             user = await self.db.users.find_one({'token': self.args.token})
         if not user and self.args.openId:
             user = await self.db.users.find_one({'openId': self.args.openId})
         if not user and self.args.unionId:
             user = await self.db.users.find_one({'unionId': self.args.unionId})
         if user:
```

### Comparing `kkutils-1.6.8/tornado_utils/utils.py` & `kkutils-1.6.9/tornado_utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 Author: zhangkai
 Email: kai.zhang1@nio.com
 Last modified: 2018-07-30 21:41:46
 '''
 import functools
 import math
 import urllib.parse
-from urllib.parse import urlencode
 
 from tornado.template import Template
 from tornado.web import HTTPError, UIModule
 from utils import awaitable
 
 
 def authorized(method):
@@ -24,18 +23,18 @@
                 if "?" not in url:
                     if urllib.parse.urlsplit(url).scheme:
                         # if login url is absolute, make next absolute too
                         next_url = self.request.full_url()
                     else:
                         assert self.request.uri is not None
                         next_url = self.request.uri
-                    url += "?" + urlencode(dict(next=next_url))
-                self.redirect(url)
-                return None
-            raise HTTPError(403)
+                    url += "?" + urllib.parse.urlencode(dict(next=next_url))
+                return self.redirect(url)
+            else:
+                raise HTTPError(403)
         return await awaitable(method(self, *args, **kwargs))
     return wrapper
 
 
 def cache(method=None, cache_time=86400):
     def decorator(method):
         @functools.wraps(method)
```

### Comparing `kkutils-1.6.8/utils/__init__.py` & `kkutils-1.6.9/utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import warnings
 
 from .base_utils import (Cache, DefaultDict, Dict, DictUnwrapper, DictWrapper,
-                         JSONEncoder, Singleton, awaitable, ceil, connect,
-                         floor, get_ip, int2ip, int2str, ip2int, multi_apply,
-                         pprint, str2int, to_bytes, to_str, tqdm, yaml)
+                         JSONEncoder, Singleton, async_tasks, awaitable, ceil,
+                         connect, floor, get_ip, int2ip, int2str, ip2int,
+                         multi_apply, pprint, str2int, to_bytes, to_str, tqdm,
+                         yaml)
 from .cached_property import cached_property
 from .config_utils import Config
 from .crypto import (aes_decrypt, aes_encrypt, des_decrypt, des_encrypt,
-                     gen_rsa_key, rsa_decrypt, rsa_encrypt)
+                     gen_rsa_key, rsa_decrypt, rsa_encrypt, xor_decrypt,
+                     xor_encrypt)
 from .db_utils import (AioMysql, AioRedis, Mongo, MongoClient, Motor,
                        MotorClient, Mysql, Redis, parse_uri)
 from .decorator import aioretry, retry, smart_decorator, synchronize, timeit
 from .email_utils import AioEmail, Email
 from .fire import Fire
 from .http_utils import Response, patch_connection_pool
 from .log_utils import Logger, WatchedFileHandler
@@ -28,16 +30,17 @@
     from .curl_utils import Request
 except:
     from .http_utils import Request
 
 warnings.filterwarnings("ignore")
 
 __all__ = [
-    'awaitable', 'floor', 'ceil', 'to_str', 'to_bytes', 'tqdm', 'yaml', 'pprint',
-    'timeit', 'retry', 'aioretry', 'smart_decorator', 'synchronize', 'cached_property', 'multi_apply',
+    'awaitable', 'floor', 'ceil', 'to_str', 'to_bytes', 'tqdm', 'yaml', 'pprint', 'timeit',
+    'retry', 'aioretry', 'smart_decorator', 'synchronize', 'cached_property', 'multi_apply', 'async_tasks',
     'get_ip', 'connect', 'ip2int', 'int2ip', 'int2str', 'str2int', 'patch_connection_pool', 'parse_uri',
     'des_encrypt', 'des_decrypt', 'aes_encrypt', 'aes_decrypt', 'gen_rsa_key', 'rsa_encrypt', 'rsa_decrypt',
+    'xor_encrypt', 'xor_decrypt',
     'Fire', 'Singleton', 'JSONEncoder', 'Dict', 'DefaultDict', 'DictWrapper', 'DictUnwrapper',
     'Email', 'AioEmail', 'Config', 'Logger', 'WatchedFileHandler', 'Cache', 'XdbSearcher',
     'Mongo', 'MongoClient', 'Redis', 'AioRedis', 'Motor', 'MotorClient', 'Mysql', 'AioMysql', 'Pika', 'AioPika',
     'Request', 'Response', 'Stopwatch'
 ]
```

### Comparing `kkutils-1.6.8/utils/base_utils.py` & `kkutils-1.6.9/utils/base_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 '''
 Author:        digua
 Created at:    2021-10-30 17:03:31
 Last modified: 2021-11-01 15:26:05
 '''
 
+import asyncio
 import collections
 import datetime
 import decimal
 import inspect
 import json
 import math
 import os
@@ -243,32 +244,45 @@
 
 async def awaitable(ret):
     return await ret if inspect.isawaitable(ret) else ret
 
 
 def multi_apply(func, *args, **kwargs):
     workers = kwargs.pop('workers', os.cpu_count())
-    backend = kwargs.pop('backend', 'thread')
+    pool = kwargs.pop('pool', False)
     batch = kwargs.pop('batch', None)
     size = len(args[0])
     if batch:
         step = math.ceil(size / batch)
         iterables = [[x[i::step] for i in range(step)] for x in args]
     else:
         iterables = [[x[i::workers] for i in range(workers)] for x in args]
     func = partial(func, **kwargs) if kwargs else func
-    Executor = ThreadPoolExecutor if backend == 'thread' else ProcessPoolExecutor
+    Executor = ProcessPoolExecutor if pool else ThreadPoolExecutor
     with Executor(workers) as executor:
         results = executor.map(func, *iterables)
     results = list(results)
     if all([isinstance(x, (list, tuple)) for x in results]):
         results = list(chain(*zip_longest(*results)))[:size]
     return results
 
 
+async def async_tasks(func, *args, **kwargs):
+    workers = kwargs.pop('workers', os.cpu_count())
+    sem = asyncio.Semaphore(workers)
+
+    async def inner(func, *args):
+        async with sem:
+            await func(*args)
+
+    func = partial(func, **kwargs) if kwargs else func
+    tasks = [asyncio.create_task(inner(func, *x)) for x in zip(*args)]
+    return await asyncio.gather(*tasks)
+
+
 def floor(number, ndigits=0):
     '''当ndigits大于等于number的小数点位数时，直接返回
     '''
     if ndigits == 0:
         return math.floor(number)
     else:
         if float(f'{number:.{ndigits}f}') == number:
```

### Comparing `kkutils-1.6.8/utils/cached_property.py` & `kkutils-1.6.9/utils/cached_property.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.8/utils/config_utils.py` & `kkutils-1.6.9/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.8/utils/crypto.py` & `kkutils-1.6.9/utils/crypto.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,32 @@
     return to_str(binascii.b2a_hex(data))
 
 
 def hex_load(text):
     return binascii.a2b_hex(text)
 
 
+def xor_encrypt(text: str, key: int, encode='base64'):
+    encrypt = ''.join([chr(ord(x) ^ ord(chr(key))) for x in to_str(text)])
+    if encode == 'base64':
+        return to_str(base64.b64encode(encrypt.encode()))
+    else:
+        return to_str(binascii.b2a_hex(encrypt.encode()))
+
+
+def xor_decrypt(ciphertext: str, key: int, encode='base64'):
+    if encode == 'base64':
+        data = base64.b64decode(ciphertext)
+    else:
+        data = binascii.a2b_hex(to_bytes(ciphertext))
+
+    decrypted = ''.join([chr(ord(x) ^ ord(chr(key))) for x in to_str(data)])
+    return to_str(decrypted)
+
+
 def des_encrypt(text, key, iv=None, mode=DES.MODE_CBC, encode='base64'):
     ''' key: 8位 '''
     data = _pad(to_bytes(text), DES.block_size)
     key = to_bytes(key)
     iv = iv or key[:8]
     cipher = DES.new(key, mode, iv)
     encrypt_data = cipher.encrypt(data)
```

### Comparing `kkutils-1.6.8/utils/curl_utils.py` & `kkutils-1.6.9/utils/curl_utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.8/utils/db_utils.py` & `kkutils-1.6.9/utils/db_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     def __init__(self, **kwargs):
         uri = kwargs.pop('uri', os.environ.get('MONGO_URI'))
         if not uri:
             host = kwargs.pop('host', os.environ.get('MONGO_HOST', 'localhost'))
             port = kwargs.pop('port', os.environ.get('MONGO_PORT', 27017))
             user = kwargs.pop('user', os.environ.get('MONGO_USER'))
             password = kwargs.pop('password', os.environ.get('MONGO_PWD'))
-            db = kwargs.pop('db', os.environ.get('MONGO_DB', 'test'))
+            db = kwargs.pop('db', os.environ.get('MONGO_DB', 'admin'))
             uri = f"mongodb://{quote_plus(user)}:{quote_plus(password)}@{host}:{port}/{db}" if user and password else f"mongodb://{host}:{port}/{db}"
 
         if not uri.startswith('mongodb') and os.environ.get('MONGO_ENC'):
             uri = des_decrypt(uri, os.environ.get('MONGO_ENC'))
         kwargs.setdefault('document_class', Dict)
         super(MongoClient, self).__init__(uri, **kwargs)
```

### Comparing `kkutils-1.6.8/utils/decorator.py` & `kkutils-1.6.9/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.8/utils/email_utils.py` & `kkutils-1.6.9/utils/email_utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.8/utils/fire.py` & `kkutils-1.6.9/utils/fire.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.8/utils/http_utils.py` & `kkutils-1.6.9/utils/http_utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.8/utils/log_utils.py` & `kkutils-1.6.9/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.8/utils/rabbitmq.py` & `kkutils-1.6.9/utils/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.8/utils/stopwatch.py` & `kkutils-1.6.9/utils/stopwatch.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.8/utils/xdb_searcher.py` & `kkutils-1.6.9/utils/xdb_searcher.py`

 * *Files identical despite different names*

