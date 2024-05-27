# Comparing `tmp/vxutils-20240424.tar.gz` & `tmp/vxutils-20240522.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vxutils-20240424.tar", max compression
+gzip compressed data, was "vxutils-20240522.tar", max compression
```

## Comparing `vxutils-20240424.tar` & `vxutils-20240522.tar`

### file list

```diff
@@ -1,24 +1,27 @@
--rw-r--r--   0        0        0     1998 2024-04-24 07:58:46.880003 vxutils-20240424/pyproject.toml
--rw-r--r--   0        0        0       24 2024-02-28 02:40:58.487414 vxutils-20240424/README.md
--rw-r--r--   0        0        0      421 2024-04-02 02:11:16.355963 vxutils-20240424/src/vxsched/__init__.py
--rw-r--r--   0        0        0     1374 2024-04-14 08:23:52.813822 vxutils-20240424/src/vxsched/__main__.py
--rw-r--r--   0        0        0     7776 2024-03-15 02:21:02.576581 vxutils-20240424/src/vxsched/core.py
--rw-r--r--   0        0        0    11734 2024-03-07 05:59:56.919198 vxutils-20240424/src/vxsched/event.py
--rw-r--r--   0        0        0        0 2024-03-07 06:18:59.347092 vxutils-20240424/src/vxsched/py.typed
--rw-r--r--   0        0        0     1202 2024-04-02 02:11:10.194079 vxutils-20240424/src/vxsched/subpubs.py
--rw-r--r--   0        0        0     1375 2024-04-03 04:23:00.014767 vxutils-20240424/src/vxutils/__init__.py
--rw-r--r--   0        0        0     3738 2024-03-31 05:45:39.670502 vxutils-20240424/src/vxutils/context.py
--rw-r--r--   0        0        0     9225 2024-02-20 02:25:26.235753 vxutils-20240424/src/vxutils/convertors.py
--rw-r--r--   0        0        0        0 2024-02-17 13:24:20.316286 vxutils-20240424/src/vxutils/datamodel/__init__.py
--rw-r--r--   0        0        0     4436 2024-04-23 09:59:47.736934 vxutils-20240424/src/vxutils/datamodel/adapter.py
--rw-r--r--   0        0        0     2451 2024-04-24 07:58:33.970839 vxutils-20240424/src/vxutils/datamodel/core.py
--rw-r--r--   0        0        0    15247 2024-03-12 05:04:59.968100 vxutils-20240424/src/vxutils/datamodel/dborm.py
--rw-r--r--   0        0        0     9071 2024-04-07 01:14:57.773870 vxutils-20240424/src/vxutils/decorators.py
--rw-r--r--   0        0        0     9568 2024-04-07 01:16:17.431751 vxutils-20240424/src/vxutils/dtutils.py
--rw-r--r--   0        0        0     7430 2024-04-10 02:46:27.989670 vxutils-20240424/src/vxutils/logger.py
--rw-r--r--   0        0        0    14529 2024-02-20 08:56:31.979240 vxutils-20240424/src/vxutils/networking/requests.py
--rw-r--r--   0        0        0     7987 2024-03-31 01:34:06.580192 vxutils-20240424/src/vxutils/networking/wechat.py
--rw-r--r--   0        0        0     6161 2024-04-24 04:51:26.814405 vxutils-20240424/src/vxutils/provider.py
--rw-r--r--   0        0        0        0 2024-02-15 15:46:34.000000 vxutils-20240424/src/vxutils/py.typed
--rw-r--r--   0        0        0      446 2024-03-10 03:13:04.515372 vxutils-20240424/src/vxutils/typehints.py
--rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 vxutils-20240424/PKG-INFO
+-rw-r--r--   0        0        0     2015 2024-05-23 06:50:44.625940 vxutils-20240522/pyproject.toml
+-rw-r--r--   0        0        0       24 2024-02-28 02:40:58.487414 vxutils-20240522/README.md
+-rw-r--r--   0        0        0      387 2024-04-30 07:57:04.146601 vxutils-20240522/src/vxsched/__init__.py
+-rw-r--r--   0        0        0     1374 2024-04-14 08:23:52.813822 vxutils-20240522/src/vxsched/__main__.py
+-rw-r--r--   0        0        0     1325 2024-04-30 07:48:16.967272 vxutils-20240522/src/vxsched/__subpubs.py
+-rw-r--r--   0        0        0     9403 2024-04-30 08:01:53.820604 vxutils-20240522/src/vxsched/core.py
+-rw-r--r--   0        0        0    11734 2024-03-07 05:59:56.919198 vxutils-20240522/src/vxsched/event.py
+-rw-r--r--   0        0        0        0 2024-03-07 06:18:59.347092 vxutils-20240522/src/vxsched/py.typed
+-rw-r--r--   0        0        0        0 2024-04-30 08:02:48.493272 vxutils-20240522/src/vxsched/subpubs/__init__.py
+-rw-r--r--   0        0        0     3162 2024-04-30 09:13:45.564793 vxutils-20240522/src/vxsched/subpubs/mqtt.py
+-rw-r--r--   0        0        0     3950 2024-04-30 09:12:29.598846 vxutils-20240522/src/vxsched/subpubs/tt.py
+-rw-r--r--   0        0        0     1375 2024-04-03 04:23:00.014767 vxutils-20240522/src/vxutils/__init__.py
+-rw-r--r--   0        0        0     3738 2024-05-22 11:03:46.262964 vxutils-20240522/src/vxutils/context.py
+-rw-r--r--   0        0        0     9225 2024-02-20 02:25:26.235753 vxutils-20240522/src/vxutils/convertors.py
+-rw-r--r--   0        0        0      263 2024-05-23 06:52:47.629334 vxutils-20240522/src/vxutils/datamodel/__init__.py
+-rw-r--r--   0        0        0     4633 2024-04-25 04:13:01.084260 vxutils-20240522/src/vxutils/datamodel/adapter.py
+-rw-r--r--   0        0        0     2536 2024-04-24 08:08:56.901548 vxutils-20240522/src/vxutils/datamodel/core.py
+-rw-r--r--   0        0        0    14712 2024-05-27 07:24:48.165629 vxutils-20240522/src/vxutils/datamodel/dborm.py
+-rw-r--r--   0        0        0     9071 2024-04-07 01:14:57.773870 vxutils-20240522/src/vxutils/decorators.py
+-rw-r--r--   0        0        0     9568 2024-04-07 01:16:17.431751 vxutils-20240522/src/vxutils/dtutils.py
+-rw-r--r--   0        0        0     7430 2024-04-10 02:46:27.989670 vxutils-20240522/src/vxutils/logger.py
+-rw-r--r--   0        0        0    14529 2024-02-20 08:56:31.979240 vxutils-20240522/src/vxutils/networking/requests.py
+-rw-r--r--   0        0        0     7999 2024-05-23 06:50:24.656143 vxutils-20240522/src/vxutils/networking/wechat.py
+-rw-r--r--   0        0        0     6161 2024-04-24 04:51:26.814405 vxutils-20240522/src/vxutils/provider.py
+-rw-r--r--   0        0        0        0 2024-02-15 15:46:34.000000 vxutils-20240522/src/vxutils/py.typed
+-rw-r--r--   0        0        0      446 2024-03-10 03:13:04.515372 vxutils-20240522/src/vxutils/typehints.py
+-rw-r--r--   0        0        0     1092 1970-01-01 00:00:00.000000 vxutils-20240522/PKG-INFO
```

### Comparing `vxutils-20240424/pyproject.toml` & `vxutils-20240522/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vxutils"
-version = "20240424"
+version = "20240522"
 description = "python 常用工具箱"
 license = "MIT"
 authors = ["vex1023 <vex1023@qq.com>"]
 homepage = "https://gitee.com/vxquant/vxutils"
 keywords = ["quant", "tools"]
 readme = "README.md"
 
@@ -32,15 +32,16 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 python-dateutil = "*"
 pydantic = "^2.0"
 sqlalchemy = "^1.4"
-httpx = "*"
+joblib = "*"
+requests = "*"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 flake8 = "*"
 pylint = "*"
 twine = "*"
```

### Comparing `vxutils-20240424/src/vxsched/__main__.py` & `vxutils-20240522/src/vxsched/__main__.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240424/src/vxsched/core.py` & `vxutils-20240522/src/vxsched/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,32 +72,32 @@
             self._handlers.pop(event_type, [])
         elif callback in self._handlers[event_type]:
             self._handlers[event_type].remove(callback)
             logging.debug(f"Unregister event handler: {event_type} -> {callback}")
 
     @async_task(10, "logging")
     def _run_handler(
-        self, callback: Callable[[VXContext, VXEvent], Any], event: VXEvent
+        self, handler: Callable[[VXContext, VXEvent], Any], event: VXEvent
     ) -> Any:
         """运行事件
 
         Arguments:
-            callback {Callable[[VXContext, VXEvent], Any]} -- 事件回调函数
+            handler {Callable[[VXContext, VXEvent], Any]} -- 事件回调函数
             event {VXEvent} -- 事件
 
         Returns:
             Any -- _description_
         """
         try:
             start = time.perf_counter()
-            return callback(self.context, event)
+            return handler(self.context, event)
         finally:
             cost = time.perf_counter() - start
             if cost > 1:
-                logging.warning(f"Event handler {callback} cost {cost*1000:,.2f}ms")
+                logging.warning(f"Event handler {handler} cost {cost*1000:,.2f}ms")
 
     def trigger_event(
         self, event: Optional[VXEvent] = None, *, is_async: bool = True
     ) -> Any:
         """触发消息（同步触发）
 
         Arguments:
@@ -174,15 +174,15 @@
             self.start()
             for event in events:
                 self.trigger_event(event, is_async=False)
         finally:
             self.stop()
 
 
-sched = VXScheduler()
+vxsched = VXScheduler()
 
 
 def load_modules(mod_path: Union[str, Path]) -> Any:
     """加载策略目录"""
     if not os.path.exists(mod_path):
         logging.warning(msg=f"{mod_path} is not exists")
         return
@@ -204,14 +204,71 @@
                 logging.info(f"Load Module: {strategy_mod} Sucess.")
                 logging.info("+" * 80)
             except Exception as err:
                 logging.error(f"Load Module: {mod} Failed. {err}", exc_info=True)
                 logging.error("-" * 80)
 
 
+class VXSubscriber:
+    """订阅器"""
+
+    def __init__(self, *, target_scheduler: Optional[VXScheduler] = None) -> None:
+        self._sched = target_scheduler or vxsched
+
+    def __call__(self, *args: Any, **kwds: Any) -> Any:
+        raise NotImplementedError
+
+    def on_event(
+        self,
+        event: Union[str, VXEvent],
+        *,
+        trigger: Optional[VXTrigger] = None,
+        data: Optional[Dict[str, Any]] = None,
+        channel: str = "default",
+        priority: int = 10,
+        reply_to: str = "",
+    ) -> None:
+        self._sched.publish(
+            event=event,
+            trigger=trigger,
+            data=data,
+            channel=channel,
+            priority=priority,
+            reply_to=reply_to,
+        )
+        logging.debug(f"Put event: {event} with trigger: {trigger} into queue.")
+
+
+class VXPublisher:
+    """发布器"""
+
+    def __init__(self, *, target_scheduler: Optional[VXScheduler] = None) -> None:
+        self._sched = target_scheduler or vxsched
+
+    def __call__(
+        self,
+        event: Union[str, VXEvent],
+        *,
+        trigger: Optional[VXTrigger] = None,
+        data: Optional[Dict[str, Any]] = None,
+        channel: str = "default",
+        priority: int = 10,
+        reply_to: str = "",
+    ) -> None:
+        self._sched.publish(
+            event=event,
+            trigger=trigger,
+            data=data,
+            channel=channel,
+            priority=priority,
+            reply_to=reply_to,
+        )
+        logging.debug(f"Put event: {event} with trigger: {trigger} into queue.")
+
+
 if __name__ == "__main__":
     import time
     from vxutils import loggerConfig
 
     loggerConfig(filename="")
 
     sched = VXScheduler()
```

### Comparing `vxutils-20240424/src/vxsched/event.py` & `vxutils-20240522/src/vxsched/event.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240424/src/vxsched/subpubs.py` & `vxutils-20240522/src/vxsched/__subpubs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """事件处理器模块"""
 
 import logging
 from typing import Any, Optional, Union, Dict
-from vxsched.event import VXEventQueue, VXEvent, VXTrigger
+from vxsched.event import VXEvent, VXTrigger
+from vxsched import vxsched, VXScheduler
 
 
 class VXSubscriber:
     """订阅器"""
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         pass
@@ -14,16 +15,16 @@
     def __call__(self) -> VXEvent:
         raise NotImplementedError
 
 
 class VXPublisher:
     """发布器"""
 
-    def __init__(self, event_queue: VXEventQueue) -> None:
-        self._queue = event_queue
+    def __init__(self, *, target_scheduler: Optional[VXScheduler] = None) -> None:
+        self._sched = target_scheduler or vxsched
 
     def __call__(
         self,
         event: Union[str, VXEvent],
         *,
         trigger: Optional[VXTrigger] = None,
         data: Optional[Dict[str, Any]] = None,
@@ -35,13 +36,14 @@
             event = VXEvent(
                 type=event,
                 data=data or {},
                 priority=priority,
                 channel=channel,
                 reply_to=reply_to,
             )
-        self._queue.put(event, trigger=trigger)
+        # self._queue.put(event, trigger=trigger)
+        self._sched.publish(event, trigger=trigger)
         logging.debug(f"Put event: {event} with trigger: {trigger} into queue.")
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `vxutils-20240424/src/vxutils/__init__.py` & `vxutils-20240522/src/vxutils/__init__.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240424/src/vxutils/context.py` & `vxutils-20240522/src/vxutils/context.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240424/src/vxutils/convertors.py` & `vxutils-20240522/src/vxutils/convertors.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240424/src/vxutils/datamodel/adapter.py` & `vxutils-20240522/src/vxutils/datamodel/adapter.py`

 * *Files 14% similar despite different names*

```diff
@@ -85,29 +85,32 @@
     }
     """
 
     def __init__(
         self,
         target_cls: Union[Type[BaseModel], Type[Dict[str, Any]]],
         coladapters: Dict[str, Union[str, Callable[[Any], Any]]],
+        pre_process: Optional[Callable[[Any], Any]] = None,
     ) -> None:
         self._target_cls = target_cls
         self._coladapters: Dict[str, Callable[[Any], Any]] = {}
         for target_col, coladapter in coladapters.items():
             if isinstance(coladapter, VXColAdapter):
                 self._coladapters[target_col] = coladapter
             if isinstance(coladapter, str):
                 self._coladapters[target_col] = OriginCol(coladapter)
             elif callable(coladapter):
                 self._coladapters[target_col] = TransCol(coladapter)
+        self._pre_process = pre_process if callable(pre_process) else lambda x: x
 
     def __call__(
         self, other_data: Any, *, key: str = "", ignore_col_error: bool = False
     ) -> Any:
         try:
+            other_data = self._pre_process(other_data)
             data = {}
             for target_col, coladapter in self._coladapters.items():
                 try:
                     data[target_col] = coladapter(other_data)
                 except DataAdapterError as e:
                     if not ignore_col_error:
                         raise e
```

### Comparing `vxutils-20240424/src/vxutils/datamodel/core.py` & `vxutils-20240522/src/vxutils/datamodel/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,48 +19,50 @@
 
 DatetimeType = datetime.datetime
 
 
 class VXDataModel(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
-    updated_dt: Annotated[VXDatetime, PlainValidator(to_vxdatetime)] = Field(
-        default_factory=VXDatetime.now, validate_default=True
+    updated_dt: Annotated[datetime.datetime, PlainValidator(to_vxdatetime)] = Field(
+        default_factory=datetime.datetime.now, validate_default=True
     )
-    created_dt: Annotated[VXDatetime, PlainValidator(to_vxdatetime)] = Field(
-        default_factory=VXDatetime.now, validate_default=True
+    created_dt: Annotated[datetime.datetime, PlainValidator(to_vxdatetime)] = Field(
+        default_factory=datetime.datetime.now, validate_default=True
     )
 
     def __init__(self, **data: Dict[str, Any]) -> None:
-        created_dt: VXDatetime = data.setdefault("created_dt", VXDatetime.now())
-        updated_dt: VXDatetime = data.setdefault("updated_dt", created_dt)
+        created_dt: datetime.datetime = data.setdefault(
+            "created_dt", datetime.datetime.now()
+        )
+        updated_dt: datetime.datetime = data.setdefault("updated_dt", created_dt)
 
         super().__init__(**data)
         self.__dict__.pop("created_dt", None)
         self.__dict__.pop("updated_dt", None)
         self.created_dt = created_dt
         self.updated_dt = updated_dt
 
     def __setattr__(self, name: str, value: Any) -> None:
         field_info = self.model_fields.get(name)
         if field_info and field_info.annotation != type(value) and field_info.metadata:
             value = TypeAdapter(field_info.annotation).validate_python(value)
 
         if name not in ["updated_dt", "created_dt"]:
-            self.updated_dt = VXDatetime.now()
+            self.updated_dt = datetime.datetime.now()
         return super().__setattr__(name, value)
 
     def __str__(self) -> str:
         return self.model_dump_json(indent=4)
 
     def __repr__(self) -> str:
         return self.model_dump_json(indent=4)
 
     @field_validator("updated_dt", "created_dt", mode="plain")
-    def validate_datetime(cls, value: Any) -> VXDatetime:
+    def validate_datetime(cls, value: Any) -> datetime.datetime:
         return to_vxdatetime(value)
 
 
 if __name__ == "__main__":
     from pprint import pprint
 
     class vxTick(VXDataModel):
```

### Comparing `vxutils-20240424/src/vxutils/datamodel/dborm.py` & `vxutils-20240522/src/vxutils/datamodel/dborm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,462 +1,483 @@
 """数据库ORM抽象"""
 
-import contextlib
+import logging
 from enum import Enum
-from typing import Iterator, List, Optional, Type, Union, Dict, Tuple, Any
+from typing import (
+    Iterator,
+    List,
+    Optional,
+    Type,
+    Union,
+    Dict,
+    Tuple,
+    Any,
+    Literal,
+    Generator,
+)
+from functools import singledispatch
+from collections import namedtuple
+from contextlib import contextmanager
 from multiprocessing import Lock
 import sqlite3
 from sqlalchemy import (
     create_engine,
     Connection,
     MetaData,
     Table,
     Column,
     Boolean,
     Float,
     Integer,
     LargeBinary,
     Text,
+    DateTime,
+    Date,
+    Time,
     text,
 )
+from sqlalchemy.sql import Insert, Update, Delete
+from sqlalchemy.dialects.sqlite import insert as sqlite_insert
+from sqlalchemy.types import TypeEngine
+from datetime import datetime, date, time as dt_time, timedelta
 from vxutils.datamodel.core import VXDataModel
-from vxutils.typehints import Datetime
 
 
-__columns_mapping__ = {
-    str: Text(256),
-    float: Float,
+SHARED_MEMORY_DATABASE = "file:vxquantdb?mode=memory&cache=shared"
+
+__columns_mapping__: Dict[Any, TypeEngine] = {
     int: Integer,
+    float: Float,
     bool: Boolean,
     bytes: LargeBinary,
     Enum: Text(256),
-    Datetime: Float,
+    datetime: DateTime,
+    date: Date,
+    dt_time: Time,
+    timedelta: Float,
 }
 
-SHARED_MEMORY_DATABASE = "file:vxquantdb?mode=memory&cache=shared"
+VXTableInfo = namedtuple("VXTableInfo", ["table", "model", "primary_keys"])
 
 
-def _normalize(value: Any) -> Any:
+@singledispatch
+def db_normalize(value: Any) -> Any:
     """标准化处理数据库数值"""
+    return value
+
+
+@db_normalize.register(Enum)
+def _(value: Enum) -> str:
+    return value.name
+
+
+@db_normalize.register(datetime)
+def _(value: datetime) -> str:
+    return value.strftime("%Y-%m-%d %H:%M:%S")
+
+
+@db_normalize.register(date)
+def _(value: date) -> str:
+    return value.strftime("%Y-%m-%d")
+
 
-    if value is None:
-        return ""
-    elif value is False:
-        return 0
-    elif value is True:
-        return 1
-    elif isinstance(value, Enum):
-        return value.name
-    else:
-        return value
+@db_normalize.register(dt_time)
+def _(value: dt_time) -> str:
+    return value.strftime("%H:%M:%S")
 
 
-def creator() -> sqlite3.Connection:
-    return sqlite3.connect(SHARED_MEMORY_DATABASE, uri=True)
+@db_normalize.register(timedelta)
+def _(value: timedelta) -> float:
+    return value.total_seconds()
 
 
-class vxDataBase:
-    """基于vxDataClass 数据管理"""
+@db_normalize.register(bool)
+def _(value: bool) -> int:
+    return 1 if value else 0
+
+
+@db_normalize.register(type(None))
+def _(value: None) -> str:
+    return ""
+
+
+class VXDataBase:
 
     def __init__(self, db_uri: str = "", **kwargs: Any) -> None:
-        if not db_uri:
-            kwargs["creator"] = creator
-            db_uri = "sqlite:///:memory:"
 
-        self._dbengine = create_engine(db_uri, **kwargs)
+        self._lock = Lock()
         self._metadata = MetaData()
         self._tblmapping: Dict[str, Type[VXDataModel]] = {}
-        self._lock = Lock()
 
-    @classmethod
-    def connect(cls, db_uri: str = "", **kwargs: Any) -> "vxDataBase":
-        """连接数据库"""
-        return cls(db_uri, **kwargs)
+        if not db_uri:
+            kwargs["creator"] = lambda: sqlite3.connect(
+                SHARED_MEMORY_DATABASE, uri=True
+            )
+            self._dbengine = create_engine("sqlite:///:memory:", **kwargs)
+        else:
+            self._dbengine = create_engine(db_uri, **kwargs)
 
     def create_table(
         self,
         table_name: str,
         primary_keys: List[str],
         vxdatacls: Type[VXDataModel],
-        if_exists: str = "ignore",
-    ) -> "vxDataBase":
+        if_exists: Literal["ignore", "replace"] = "ignore",
+    ) -> "VXDataBase":
         """创建数据表
 
         Arguments:
             table_name {str} -- 数据表名称
             primary_keys {List[str]} -- 表格主键
             vxdatacls {_type_} -- 表格数据格式
             if_exists {str} -- 如果table已经存在，若参数为ignore ，则忽略；若参数为 replace，则replace掉已经存在的表格，然后再重新创建
 
         Returns:
             vxDataBase -- 返回数据表格实例
         """
         column_defs = [
             Column(
                 name,
-                __columns_mapping__.get(vxfield.__dbtype__, Text(256)),
+                __columns_mapping__.get(field_info.annotation, Text(256)),
                 primary_key=(name in primary_keys),
                 nullable=(name in primary_keys),
             )
-            for name, vxfield in vxdatacls.__vxfields__.items()
+            for name, field_info in vxdatacls.model_fields.items()
         ]
-        tbl = Table(table_name, self._metadata, *column_defs)
 
-        self._tblmapping[table_name] = (tbl, vxdatacls, primary_keys)
+        if table_name in self._metadata.tables.keys():
+            if if_exists == "ignore":
+                logging.warning("Table %s already exists", table_name)
+                return self
+            elif if_exists == "replace":
+                tbl = self._metadata.tables[table_name]
+                tbl.drop(bind=self._dbengine, checkfirst=True)
+                logging.warning("Table %s already exists, replace it", table_name)
+                self._metadata.remove(self._metadata.tables[table_name])
 
-        if if_exists == "replace":
-            tbl.drop(bind=self._dbengine, checkfirst=True)
+        tbl = Table(table_name, self._metadata, *column_defs)
+        self._tblmapping[table_name] = vxdatacls
         tbl.create(bind=self._dbengine, checkfirst=True)
+        logging.warning("Table: %s ==> %s", table_name, vxdatacls)
         return self
 
-    def drop_table(self, table_name: str) -> "vxDataBase":
+    def drop_table(self, table_name: str) -> "VXDataBase":
         """删除数据表
 
         Arguments:
             table_name {str} -- 数据表名称
+
+        Returns:
+            vxDataBase -- 返回数据表格实例
         """
-        if table_name in self._tblmapping:
-            tbl, _, _ = self._tblmapping.pop(table_name)
+        if table_name in self._metadata.tables.keys():
+            tbl = self._metadata.tables[table_name]
             tbl.drop(bind=self._dbengine, checkfirst=True)
+            logging.warning("Table %s dropped", table_name)
+            self._metadata.remove(self._metadata.tables[table_name])
+
+        if table_name in self._tblmapping.keys():
+            self._tblmapping.pop(table_name)
+
         return self
 
-    def truncate(self, table_name: str) -> "vxDataBase":
+    def truncate(self, table_name: str) -> "VXDataBase":
         """清空表格
 
         Arguments:
             table_name {str} -- 待清空的表格名称
         """
-        if table_name in self._tblmapping:
-            tbl, _, _ = self._tblmapping.pop(table_name)
+        if table_name in self._metadata.tables.keys():
+            tbl = self._metadata.tables[table_name]
 
             with self._dbengine.begin() as conn:
                 conn.execute(tbl.delete())
+            logging.warning("Table %s truncated", table_name)
         return self
 
-    @contextlib.contextmanager
-    def start_session(self, with_lock=True):
+    @contextmanager
+    def start_session(self, with_lock: bool = True) -> Generator[Any, Any, Any]:
         """开始session，锁定python线程加锁，保障一致性"""
         if with_lock:
             with self._lock, self._dbengine.begin() as conn:
-                yield vxDBSession(conn, self._tblmapping)
+                yield VXDBSession(conn, self._tblmapping, self._metadata)
         else:
             with self._dbengine.begin() as conn:
-                yield vxDBSession(conn, self._tblmapping)
+                yield VXDBSession(conn, self._tblmapping, self._metadata)
 
-    def get_dbsession(self):
+    def get_dbsession(self) -> "VXDBSession":
         """获取一个session"""
-        return vxDBSession(self._dbengine.connect(), self._tblmapping)
+        return VXDBSession(self._dbengine.connect(), self._tblmapping, self._metadata)
 
 
-class vxDBSession:
+class VXDBSession:
+
     def __init__(
-        self, conn: Connection, tblmapping: Dict[str, Tuple[Table, Type[vxDataClass]]]
+        self,
+        conn: Connection,
+        tblmapping: Dict[str, Type[VXDataModel]],
+        metadata: MetaData,
     ) -> None:
         self._conn = conn
         self._tblmapping = tblmapping
+        self._metadata = metadata
 
-    def save(self, table_name: str, *vxdataobjs) -> None:
-        """保存vxdataclass的objects
+    def save(self, table_name: str, *vxdataobjs: VXDataModel) -> "VXDBSession":
+        """插入数据
 
         Arguments:
-            table_name {str} -- 数据表名称
-            vxdataobjs [vxdataobj] -- 需要保存的vxdataclass objects
+            table_name {str} -- 表格名称
+            vxdataobjs {VXDataModel} -- 数据
         """
-        if len(vxdataobjs) == 1 and isinstance(vxdataobjs[0], (list, tuple)):
-            vxdataobjs = vxdataobjs[0]
-        if table_name not in self._tblmapping:
-            raise KeyError(f"{table_name} is not in tblmapping.")
-
-        _, vxdatacls, _ = self._tblmapping[table_name]
-        fields = list(vxdatacls.__vxfields__.keys())
-        cols = " , ".join(fields)
-        col_ids = " , ".join([f":{f}" for f in fields])
-        sql = text(
-            f"""INSERT OR REPLACE INTO `{table_name}`
-            ({cols})
-            VALUES ({col_ids})"""
-        )
-
-        datas = [
-            {col: _normalize(getattr(obj, col)) for col in fields}
-            for obj in vxdataobjs
-            if isinstance(obj, vxDataClass)
-        ]
 
-        self._conn.execute(sql, datas)
+        tbl = self._metadata.tables[table_name]
+        insert_stmt = (
+            sqlite_insert(tbl)
+            .values(
+                [
+                    {k: v for k, v in vxdataobj.model_dump().items()}
+                    for vxdataobj in vxdataobjs
+                ]
+            )
+            .execution_options()
+        ).on_conflict_do_update(
+            index_elements=tbl.primary_key,
+            set_={
+                k: v
+                for k, v in vxdataobjs[0].model_dump().items()
+                if k not in tbl.primary_key
+            },
+        )
+        self._conn.execute(insert_stmt)
+        logging.warning("Table %s saved, %s", table_name, insert_stmt.compile())
         return self
 
-    def find(self, table_name: str, *conditions, **query) -> Iterator:
-        """查询数据
+    def remove(self, table_name: str, *vxdataobjs: VXDataModel) -> "VXDBSession":
+        """删除数据
 
         Arguments:
-            table_name {str} -- 数据表名称
-            conditions [list[str]] -- 查询条件
-            query {str} -- 查询条件
+            table_name {str} -- 表格名称
+            vxdataobjs {VXDataModel} -- 数据
         """
-        sql = f"""SELECT * FROM `{table_name}`"""
-        query_conditions = list(conditions)
-        _, vxdatacls, _ = self._tblmapping[table_name]
-        if query:
-            query_conditions.extend(
-                [f"{key}='{value or ''}'" for key, value in query.items()]
-            )
-        if query_conditions:
-            sql += f""" WHERE {' and '.join(query_conditions)}"""
-        sql += ";"
-
-        for row in self._conn.execute(text(sql)):
-            yield vxdatacls(**row._mapping)
+        tbl = self._metadata.tables[table_name]
+        delete_stmt = tbl.delete().where(
+            tbl.c[tbl.primary_key.columns.keys()[0]]
+            == vxdataobjs[0].model_dump()[tbl.primary_key.columns.keys()[0]]
+        )
+        self._conn.execute(delete_stmt)
+        logging.warning("Table %s deleted, %s", table_name, delete_stmt)
+        return self
 
-    def findone(self, table_name: str, *conditions, **query) -> Optional[vxDataClass]:
-        """查询数据
+    def delete(self, table_name: str, *exprs: str, **options: Any) -> "VXDBSession":
+        """删除数据
 
         Arguments:
-            table_name {str} -- 数据表名称
-            conditions [list[str]] -- 查询条件
-            query {str} -- 查询条件
+            table_name {str} -- 表格名称
+
+        Returns:
+            Iterator[VXDataModel] -- 返回查询结果
         """
-        sql = f"""SELECT * FROM `{table_name}`"""
-        query_conditions = list(conditions)
-        _, vxdatacls, _ = self._tblmapping[table_name]
-        if query:
-            query_conditions.extend(
-                [f"{key}='{value or ''}'" for key, value in query.items()]
-            )
-        if query_conditions:
-            sql += f""" WHERE {' and '.join(query_conditions)}"""
-        sql += ";"
+        query = list(exprs)
+        if options:
+            query.extend(f"{k}={v}" for k, v in options.items())
+
+        delete_stmt = (
+            f"delete from {table_name} where {' and '.join(query)};"
+            if query
+            else f"delete from {table_name} ; "
+        )
 
-        row = self._conn.execute(text(sql)).fetchone()
-        return vxdatacls(**row._mapping) if row else None
+        result = self._conn.execute(text(delete_stmt))
+        logging.warning("Table %s deleted  %s rows", table_name, result.rowcount)
+        return self
 
-    def remove(self, table_name: str, *vxdataobjs) -> None:
-        """删除数据vxdataclass objects
+    def find(
+        self,
+        table_name: str,
+        *exprs: str,
+        **options: Any,
+    ) -> Iterator[VXDataModel]:
+        """查询数据
 
         Arguments:
-            table_name {str} -- 数据表名称
-            vxdataobjs {vxdatacls_obj} -- 待删除的objects
+            table_name {str} -- 表格名称
 
+        Returns:
+            Iterator[VXDataModel] -- 返回查询结果
         """
-        if len(vxdataobjs) == 1 and isinstance(vxdataobjs[0], (list, tuple)):
-            vxdataobjs = vxdataobjs[0]
-
-        if table_name not in self._tblmapping:
-            raise KeyError(f"{table_name} is not in tblmapping.")
-
-        _, vxdatacls, primary_keys = self._tblmapping[table_name]
-
-        if not primary_keys:
-            primary_keys = vxdatacls.__vxfields__
-            primary_keys.pop("created_dt")
-            primary_keys.pop("updated_dt")
-
-        query_str = " and ".join([f"{key} =:{key}" for key in primary_keys])
-        sql = f"DELETE FROM `{table_name}` WHERE {query_str}"
-
-        datas = [
-            {key: _normalize(getattr(vxdataobj, key)) for key in primary_keys}
-            for vxdataobj in vxdataobjs
-        ]
-        self._conn.execute(text(sql), datas)
+        query = list(exprs)
+        if options:
+            query.extend(f"{k}='{v}'" for k, v in options.items())
+
+        query_stmt = text(
+            f"select * from {table_name} where {' and '.join(query)};"
+            if query
+            else f"select * from {table_name};"
+        )
+        result = self._conn.execute(query_stmt)
+        for row in result:
+            yield self._tblmapping[table_name](**dict(zip(row._fields, row)))
 
-    def delete(self, table_name: str, *conditions, **query) -> None:
-        """批量删除
+    def findone(
+        self,
+        table_name: str,
+        *exprs: str,
+        **options: Any,
+    ) -> Optional[VXDataModel]:
+        """查询数据
 
         Arguments:
-            table_name {str} -- 数据表名称
-            conditions [list(str)] -- 查询条件
-            query {str} -- 查询条件
-        """
-        sql = f"""DELETE FROM `{table_name}`"""
-        query_conditions = list(conditions)
+            table_name {str} -- 表格名称
 
-        if query:
-            query_conditions.extend(
-                [f"{key}='{value or ''}'" for key, value in query.items()]
-            )
-        if query_conditions:
-            sql += f""" WHERE {' and '.join(query_conditions)}"""
-        sql += ";"
-        self._conn.execute(text(sql))
+        Returns:
+            Iterator[VXDataModel] -- 返回查询结果
+        """
+        query = list(exprs)
+        if options:
+            query.extend(f"{k}='{v}'" for k, v in options.items())
+
+        query_stmt = text(
+            f"select * from {table_name} where {' and '.join(query)};"
+            if query
+            else f"select * from {table_name};"
+        )
+        result = self._conn.execute(query_stmt)
+        row = result.fetchone()
+        if row:
+            return self._tblmapping[table_name](**dict(zip(row._fields, row)))
+        return None
 
-    def insert(self, table_name: str, vxdataobj: vxDataClass) -> None:
-        """插入数据vxdataclass object
+    def distinct(self, table_name: str, column: str) -> List[VXDataModel]:
+        """查询数据
 
         Arguments:
-            table_name {str} -- 数据表格名称
-            vxdataobj [vxDataClass] -- 被插入对象
+            table_name {str} -- 表格名称
 
-        Raises:
-            Valueerror -- 若插入对象以存在数据库时，抛出异常
+        Returns:
+            Iterator[VXDataModel] -- 返回查询结果
         """
-        _, vxdatacls, primary_keys = self._tblmapping[table_name]
-        if not isinstance(vxdataobj, (vxDataClass, vxdatacls)):
-            raise TypeError(f"vxdataobj 类型{type(vxdataobj)}非{vxdatacls.__name__}")
-
-        col_names = []
-        values = []
-        update_string = []
-
-        for col, value in vxdataobj.items():
-            col_names.append(f"'{col}'")
-            values.append(f"'{_normalize(value)}'")
-            if col not in primary_keys:
-                update_string.append(f"{col}=excluded.{col}")
-
-            sql = f"""INSERT INTO {table_name}
-                    ({','.join(col_names)}) \n\tVALUES ({','.join(values)})"""
-
-        self._conn.execute(text(sql))
+        query_stmt = text(f"select distinct {column} from {table_name};")
+        result = self._conn.execute(query_stmt)
+        return [row for row in result]
 
-    def distinct(self, table_name: str, col: str, *conditions, **query) -> List:
-        """去重
+    def count(self, table_name: str, *exprs: str, **options: Any) -> int:
+        """查询数据
 
         Arguments:
-            table_name {str} -- 数据表格名称
-            col {str} -- 字段名称
-            conditions / query -- 查询条件
+            table_name {str} -- 表格名称
 
         Returns:
-            List -- _description_
+            Iterator[VXDataModel] -- 返回查询结果
         """
-        sql = f"""SELECT DISTINCT `{col}` FROM `{table_name}`"""
-        query_conditions = list(conditions)
+        query = list(exprs)
+        if options:
+            query.extend(f"{k}='{v}'" for k, v in options.items())
+
+        query_stmt = text(
+            f"select count(1) as count from {table_name} where {' and '.join(query)};"
+            if query
+            else f"select count(1) as count from {table_name};"
+        )
+        row = self._conn.execute(query_stmt).fetchone()
+        return row[0]
 
-        if query:
-            query_conditions.extend(
-                [f"{key}='{value or ''}'" for key, value in query.items()]
-            )
-        if query_conditions:
-            sql += f""" WHERE {' and '.join(query_conditions)}"""
-        sql += ";"
-        return [row[0] for row in self._conn.execute(text(sql))]
-
-    def count(self, table_name: str, *conditions, **query) -> int:
-        """返回数据表格中的数据条数
+    def max(self, table_name: str, column: str, *exprs: str, **options: Any) -> Any:
+        """查询数据
 
         Arguments:
-            table_name {str} -- 数据表格名称
-            conditions {List[str]} -- 查询条件
-            query {Dict[str,str]} -- 查询条件
+            table_name {str} -- 表格名称
 
         Returns:
-            int -- 返回数据条数
+            Iterator[VXDataModel] -- 返回查询结果
         """
-        sql = f"""SELECT COUNT(1) AS cnt FROM `{table_name}`"""
-        query_conditions = list(conditions)
+        query = list(exprs)
+        if options:
+            query.extend(f"{k}='{v}'" for k, v in options.items())
+
+        query_stmt = text(
+            f"select max({column}) as max from {table_name} where {' and '.join(query)};"
+            if query
+            else f"select max({column}) as max from {table_name};"
+        )
+        row = self._conn.execute(query_stmt).fetchone()
+        return row[0]
 
-        if query:
-            query_conditions.extend(
-                [f"{key}='{value or ''}'" for key, value in query.items()]
-            )
-        if query_conditions:
-            sql += f""" WHERE {' and '.join(query_conditions)}"""
-        sql += ";"
-        return self._conn.execute(text(sql)).fetchone()[0]
-
-    def max(self, table_name: str, col: str, *conditions, **query) -> Union[int, float]:
-        """获取数据表格中的最大值
+    def min(self, table_name: str, column: str, *exprs: str, **options: Any) -> Any:
+        """查询数据
 
         Arguments:
-            table_name {str} -- 数据表格名称
-            col {str} -- 字段名称
-            conditions {List[str]} -- 查询条件
-            query {Dict[str,str]} -- 查询条件
+            table_name {str} -- 表格名称
+
         Returns:
-            Union[int, float] -- 最大值
+            Iterator[VXDataModel] -- 返回查询结果
         """
-        sql = f"""SELECT MAX(`{col}`) AS col_max FROM `{table_name}`"""
-        query_conditions = list(conditions)
+        query = list(exprs)
+        if options:
+            query.extend(f"{k}='{v}'" for k, v in options.items())
+
+        query_stmt = text(
+            f"select min({column}) as min from {table_name} where {' and '.join(query)};"
+            if query
+            else f"select min({column}) as min from {table_name};"
+        )
+        row = self._conn.execute(query_stmt).fetchone()
+        return row[0]
 
-        if query:
-            query_conditions.extend(
-                [f"{key}='{value or ''}'" for key, value in query.items()]
-            )
-        if query_conditions:
-            sql += f""" WHERE {' and '.join(query_conditions)}"""
-        sql += ";"
-        return self._conn.execute(text(sql)).fetchone()[0]
-
-    def min(self, table_name: str, col: str, *conditions, **query) -> Union[int, float]:
-        """获取数据表格中的最小值
+    def mean(self, table_name: str, column: str, *exprs: str, **options: Any) -> Any:
+        """查询数据
 
         Arguments:
-            table_name {str} -- 数据表格名称
-            col {str} -- 字段名称
-            conditions {List[str]} -- 查询条件
-            query {Dict[str,str]} -- 查询条件
+            table_name {str} -- 表格名称
+
         Returns:
-            Union[int, float] -- 最小值
+            Iterator[VXDataModel] -- 返回查询结果
         """
-        sql = f"""SELECT MIN(`{col}`) AS col_min FROM `{table_name}`"""
-        query_conditions = list(conditions)
-
-        if query:
-            query_conditions.extend(
-                [f"{key}='{value or ''}'" for key, value in query.items()]
-            )
-        if query_conditions:
-            sql += f""" WHERE {' and '.join(query_conditions)}"""
-        sql += ";"
-        return self._conn.execute(text(sql)).fetchone()[0]
+        query = list(exprs)
+        if options:
+            query.extend(f"{k}='{v}'" for k, v in options.items())
+
+        query_stmt = text(
+            f"select avg({column}) as mean from {table_name} where {' and '.join(query)};"
+            if query
+            else f"select avg({column}) as mean from {table_name};"
+        )
+        row = self._conn.execute(query_stmt).fetchone()
+        return row[0]
 
-    def execute(self, sql: str, params: Union[Tuple, Dict, List] = None) -> Any:
+    def execute(
+        self, sql: str, params: Optional[Union[Tuple, Dict, List]] = None
+    ) -> Any:
         return self._conn.execute(text(sql), params)
 
     def commit(self) -> None:
         return self._conn.commit()
 
     def rollback(self) -> None:
         return self._conn.rollback()
 
     def __enter__(self) -> None:
         pass
 
-    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
-        if exc_tb and exc_type and exc_val:
-            self._conn.rollback()
-        else:
-            self._conn.commit()
-
-
-memdb = vxDataBase()
 
 if __name__ == "__main__":
-    from vxutils import vxtime
-    from vxutils.database.fields import (
-        vxUUIDField,
-        vxDatetimeField,
-        vxStringField,
-    )
-
-    # from vxquant.model.exchange import vxCashPosition
-
-    class Status(Enum):
-        SUCCESS = 0
-        FAILED = 1
-
-    class vxTest(vxDataClass):
-        id = vxUUIDField("学号", prefix="studentid", auto=True)
-        name = vxStringField("姓名")
-        dt = vxDatetimeField("修改时间")
-
-    db = vxDataBase("sqlite:///./dist/test1.db")
-    db.create_table("st", ["id"], vxTest, if_exists="replace")
-    with db.start_session() as session, vxtime.timeit():
-        t1 = vxTest()
-        session.save("st", t1)
-        objs = [vxTest(name=f"std_{i}", dt=vxtime.now() + i) for i in range(1, 10000)]
-        session.save("st", objs)
-        # obj = objs.pop(3)
-        # for i in session.find("st"):
-        #    print(i)
-        #    break
-        # session.remove("st", objs)
-        # print(session.count("st"))
-        # print(session.max("st", "age"))
-        # print(session.min("st", "age"))
-        # print(session.distinct("st", "age"))
-        # print(obj)
-        # session.insert("st", obj)
 
-        # print(session.min("st", "age", "age>=500"))
+    class Test(VXDataModel):
+        a: int
+        b: float
+        c: str
+
+    db = VXDataBase()
+    db.create_table("test", ["a"], Test)
+    db.create_table("test", ["b"], Test, if_exists="replace")
+    db.create_table("test", ["a"], Test)
+    print(db._metadata.tables)
+    test1 = Test(a=1, b=2.0, c="3")
+    test2 = Test(a=2, b=3.0, c="4")
+    test3 = Test(a=1, b=4.0, c="5")
+    with db.start_session() as session:
+        session.save("test", test1, test2, test3)
+        print(list(session.find("test", "b>2")))
+        session.delete("test", "a>1", b=3)
+        print(session.count("test"))
+        print(session.max("test", "b"))
+        print(session.min("test", "b"))
+        print(session.mean("test", "b"))
```

### Comparing `vxutils-20240424/src/vxutils/decorators.py` & `vxutils-20240522/src/vxutils/decorators.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240424/src/vxutils/dtutils.py` & `vxutils-20240522/src/vxutils/dtutils.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240424/src/vxutils/logger.py` & `vxutils-20240522/src/vxutils/logger.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240424/src/vxutils/networking/requests.py` & `vxutils-20240522/src/vxutils/networking/requests.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240424/src/vxutils/networking/wechat.py` & `vxutils-20240522/src/vxutils/networking/wechat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """wechat 通知接口"""
 
 import time
 import logging
 from typing import List, Dict, Optional, Union, Collection, Any
 import json
-import httpx
+import requests
 from concurrent.futures import Future
 from vxutils.decorators import async_task
 
 __all__ = ["vxWeChatBot", "vxWeChatClient"]
 
 
 class vxWeChatClient:
@@ -40,15 +40,15 @@
             "errcode": 0,
             "errmsg": "ok",
             "access_token": "accesstoken000001",
             "expires_in": 7200
         }
         """
         if (not self._access_token) or self._expire_time < time.time():
-            resp = httpx.get(
+            resp = requests.get(
                 f"https://qyapi.weixin.qq.com/cgi-bin/gettoken?corpid={self._corpid}&corpsecret={self._secret}",
                 timeout=self._timeout,
             )
             resp.raise_for_status()
             ret_mesg = json.loads(resp.text)
             if ret_mesg.get("errcode") != 0:
                 logging.warning("获取access_token失败. %s", ret_mesg)
@@ -110,15 +110,15 @@
             "totag": "|".join(tags) if tags else "",
             "msgtype": "markdown",
             "agentid": self._agentid,
             "markdown": {"content": markdown_content},
             "enable_duplicate_check": 0,
             "duplicate_check_interval": 1800,
         }
-        resp = httpx.post(post_url, json=msg, timeout=self._timeout)
+        resp = requests.post(post_url, json=msg, timeout=self._timeout)
         resp.raise_for_status()
         ret_msg = json.loads(resp.text)
         if ret_msg.get("errcode") != 0:
             logging.error("发送消息失败. %s", ret_msg)
             raise ConnectionError(f"发送消息失败. {ret_msg}")
 
         return str(ret_msg.get("msgid", ""))
@@ -131,15 +131,15 @@
         self._url = url
 
     @async_task(3)
     def send_message(self, message: Dict[str, Collection[str]]) -> bool:
         """发送消息"""
 
         headers = {"Content-Type": "application/json"}
-        resp = httpx.post(
+        resp = requests.post(
             self._url,
             json=message,
             headers=headers,
             timeout=5,
         )
         resp.raise_for_status()
         ret_message = json.loads(resp.text)
```

### Comparing `vxutils-20240424/src/vxutils/provider.py` & `vxutils-20240522/src/vxutils/provider.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240424/PKG-INFO` & `vxutils-20240522/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vxutils
-Version: 20240424
+Version: 20240522
 Summary: python 常用工具箱
 Home-page: https://gitee.com/vxquant/vxutils
 License: MIT
 Keywords: quant,tools
 Author: vex1023
 Author-email: vex1023@qq.com
 Requires-Python: >=3.8,<4.0
@@ -16,17 +16,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: httpx
+Requires-Dist: joblib
 Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: python-dateutil
+Requires-Dist: requests
 Requires-Dist: sqlalchemy (>=1.4,<2.0)
 Description-Content-Type: text/markdown
 
 # vxutils
 
 # vxsched
```

