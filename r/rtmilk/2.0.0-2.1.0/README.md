# Comparing `tmp/rtmilk-2.0.0.tar.gz` & `tmp/rtmilk-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtmilk-2.0.0.tar", max compression
+gzip compressed data, was "rtmilk-2.1.0.tar", max compression
```

## Comparing `rtmilk-2.0.0.tar` & `rtmilk-2.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1069 2021-07-04 08:58:00.981162 rtmilk-2.0.0/LICENSE
--rw-r--r--   0        0        0     1986 2024-05-23 05:03:47.521968 rtmilk-2.0.0/README.md
--rw-r--r--   0        0        0     1841 2024-05-23 05:03:47.522175 rtmilk-2.0.0/pyproject.toml
--rw-r--r--   0        0        0       90 2023-04-06 03:33:10.229614 rtmilk-2.0.0/src/rtmilk/__init__.py
--rw-r--r--   0        0        0     4645 2024-05-23 05:03:55.274923 rtmilk-2.0.0/src/rtmilk/_properties.py
--rw-r--r--   0        0        0    13945 2024-05-23 05:03:47.523215 rtmilk-2.0.0/src/rtmilk/_sansio.py
--rw-r--r--   0        0        0      964 2023-09-20 04:37:24.283564 rtmilk-2.0.0/src/rtmilk/_secrets.py
--rw-r--r--   0        0        0      433 2024-05-23 04:55:38.745255 rtmilk-2.0.0/src/rtmilk/_utils.py
--rw-r--r--   0        0        0    10224 2024-03-18 04:08:07.411228 rtmilk-2.0.0/src/rtmilk/api_async.py
--rw-r--r--   0        0        0      529 2023-06-11 07:06:45.144843 rtmilk-2.0.0/src/rtmilk/api_base.py
--rw-r--r--   0        0        0    10198 2024-05-23 04:37:13.012851 rtmilk-2.0.0/src/rtmilk/api_sync.py
--rw-r--r--   0        0        0      699 2024-05-23 05:03:47.523404 rtmilk-2.0.0/src/rtmilk/authorization.py
--rw-r--r--   0        0        0     4994 2024-05-23 05:03:47.523638 rtmilk-2.0.0/src/rtmilk/client.py
--rw-r--r--   0        0        0     6394 2023-09-20 04:37:24.284599 rtmilk-2.0.0/src/rtmilk/filter.py
--rw-r--r--   0        0        0     4049 2024-05-13 04:07:34.314265 rtmilk-2.0.0/src/rtmilk/mirror.py
--rw-r--r--   0        0        0     5302 2024-05-23 05:03:47.523873 rtmilk-2.0.0/src/rtmilk/models.py
--rw-r--r--   0        0        0        0 2022-01-03 07:25:19.434211 rtmilk-2.0.0/src/rtmilk/py.typed
--rw-r--r--   0        0        0     2886 1970-01-01 00:00:00.000000 rtmilk-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2021-07-04 08:58:00.981162 rtmilk-2.1.0/LICENSE
+-rw-r--r--   0        0        0     1986 2024-05-26 04:22:11.580994 rtmilk-2.1.0/README.md
+-rw-r--r--   0        0        0     1841 2024-05-27 05:40:34.985440 rtmilk-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0       90 2023-04-06 03:33:10.229614 rtmilk-2.1.0/src/rtmilk/__init__.py
+-rw-r--r--   0        0        0     4645 2024-05-27 05:40:47.354472 rtmilk-2.1.0/src/rtmilk/_properties.py
+-rw-r--r--   0        0        0    14178 2024-05-27 05:40:34.986453 rtmilk-2.1.0/src/rtmilk/_sansio.py
+-rw-r--r--   0        0        0      964 2023-09-20 04:37:24.283564 rtmilk-2.1.0/src/rtmilk/_secrets.py
+-rw-r--r--   0        0        0      433 2024-05-23 04:55:38.745255 rtmilk-2.1.0/src/rtmilk/_utils.py
+-rw-r--r--   0        0        0    10224 2024-03-18 04:08:07.411228 rtmilk-2.1.0/src/rtmilk/api_async.py
+-rw-r--r--   0        0        0      529 2023-06-11 07:06:45.144843 rtmilk-2.1.0/src/rtmilk/api_base.py
+-rw-r--r--   0        0        0    10198 2024-05-23 04:37:13.012851 rtmilk-2.1.0/src/rtmilk/api_sync.py
+-rw-r--r--   0        0        0      699 2024-05-26 04:22:11.583005 rtmilk-2.1.0/src/rtmilk/authorization.py
+-rw-r--r--   0        0        0     4994 2024-05-26 04:22:11.583597 rtmilk-2.1.0/src/rtmilk/client.py
+-rw-r--r--   0        0        0     6394 2023-09-20 04:37:24.284599 rtmilk-2.1.0/src/rtmilk/filter.py
+-rw-r--r--   0        0        0     4049 2024-05-13 04:07:34.314265 rtmilk-2.1.0/src/rtmilk/mirror.py
+-rw-r--r--   0        0        0     5302 2024-05-26 04:22:11.585219 rtmilk-2.1.0/src/rtmilk/models.py
+-rw-r--r--   0        0        0        0 2022-01-03 07:25:19.434211 rtmilk-2.1.0/src/rtmilk/py.typed
+-rw-r--r--   0        0        0     2886 1970-01-01 00:00:00.000000 rtmilk-2.1.0/PKG-INFO
```

### Comparing `rtmilk-2.0.0/LICENSE` & `rtmilk-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rtmilk-2.0.0/README.md` & `rtmilk-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `rtmilk-2.0.0/pyproject.toml` & `rtmilk-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rtmilk"
-version = "2.0.0"
+version = "2.1.0"
 description = "RTM API wrapper"
 authors = ["Rehan Khwaja <rehan@khwaja.name>"]
 license = "MIT"
 homepage = "https://github.com/rkhwaja/rtmilk"
 keywords = ["RememberTheMilk"]
 readme = "README.md"
 classifiers = [
```

### Comparing `rtmilk-2.0.0/src/rtmilk/_properties.py` & `rtmilk-2.1.0/src/rtmilk/_properties.py`

 * *Files identical despite different names*

### Comparing `rtmilk-2.0.0/src/rtmilk/_sansio.py` & `rtmilk-2.1.0/src/rtmilk/_sansio.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from datetime import date, datetime
+from datetime import date, datetime, UTC
 from hashlib import md5
 from logging import getLogger
 from pprint import pformat
 
 from pydantic import validate_call, ValidationError
 
 from .models import AuthResponse, EchoResponse, FailStat, ListsResponse, NotesResponse, PriorityDirectionEnum, PriorityEnum, RTMError, SettingsResponse, SingleListResponse, SubscriptionListResponse, SubscriptionResponse, TagListResponse, TaskListResponse, TaskPayload, TaskResponse, TimelineResponse, TopicListResponse
@@ -257,16 +257,22 @@
 	@classmethod
 	def Out(cls, **rsp):
 		return _ValidateReturn(TaskResponse, rsp)
 
 class TasksGetList(AuthorizedCall):
 	def In(self, list_id: str | None = None, filter: str | None = None, last_sync: datetime | None = None):
 		kwargs = _RebuildArgs(list_id=list_id, filter=filter, last_sync=last_sync)
-		if 'last_sync' in kwargs and isinstance(kwargs['last_sync'], (datetime)):
-			kwargs['last_sync'] = _RtmDatetime(kwargs['last_sync'])
+		if 'last_sync' in kwargs:
+			if not isinstance(kwargs['last_sync'], (datetime)):
+				raise TypeError('last_sync should be a datetime')
+			lastSyncDt = kwargs['last_sync']
+			if lastSyncDt.tzinfo is not None:
+				# switch to naive datetime in UTC
+				lastSyncDt = lastSyncDt.astimezone(UTC).replace(tzinfo=None)
+			kwargs['last_sync'] = _RtmDatetime(lastSyncDt)
 		return self.CommonParams('rtm.tasks.getList', **kwargs)
 
 	@classmethod
 	def Out(cls, **rsp):
 		return _ValidateReturn(TaskListResponse, rsp)
 
 class TasksMovePriority(AuthorizedCall):
```

### Comparing `rtmilk-2.0.0/src/rtmilk/_secrets.py` & `rtmilk-2.1.0/src/rtmilk/_secrets.py`

 * *Files identical despite different names*

### Comparing `rtmilk-2.0.0/src/rtmilk/api_async.py` & `rtmilk-2.1.0/src/rtmilk/api_async.py`

 * *Files identical despite different names*

### Comparing `rtmilk-2.0.0/src/rtmilk/api_base.py` & `rtmilk-2.1.0/src/rtmilk/api_base.py`

 * *Files identical despite different names*

### Comparing `rtmilk-2.0.0/src/rtmilk/api_sync.py` & `rtmilk-2.1.0/src/rtmilk/api_sync.py`

 * *Files identical despite different names*

### Comparing `rtmilk-2.0.0/src/rtmilk/authorization.py` & `rtmilk-2.1.0/src/rtmilk/authorization.py`

 * *Files identical despite different names*

### Comparing `rtmilk-2.0.0/src/rtmilk/client.py` & `rtmilk-2.1.0/src/rtmilk/client.py`

 * *Files identical despite different names*

### Comparing `rtmilk-2.0.0/src/rtmilk/filter.py` & `rtmilk-2.1.0/src/rtmilk/filter.py`

 * *Files identical despite different names*

### Comparing `rtmilk-2.0.0/src/rtmilk/mirror.py` & `rtmilk-2.1.0/src/rtmilk/mirror.py`

 * *Files identical despite different names*

### Comparing `rtmilk-2.0.0/src/rtmilk/models.py` & `rtmilk-2.1.0/src/rtmilk/models.py`

 * *Files identical despite different names*

### Comparing `rtmilk-2.0.0/PKG-INFO` & `rtmilk-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtmilk
-Version: 2.0.0
+Version: 2.1.0
 Summary: RTM API wrapper
 Home-page: https://github.com/rkhwaja/rtmilk
 License: MIT
 Keywords: RememberTheMilk
 Author: Rehan Khwaja
 Author-email: rehan@khwaja.name
 Requires-Python: >=3.9,<4
```

