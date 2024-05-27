# Comparing `tmp/taskara-0.1.91.tar.gz` & `tmp/taskara-0.1.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskara-0.1.91.tar", max compression
+gzip compressed data, was "taskara-0.1.92.tar", max compression
```

## Comparing `taskara-0.1.91.tar` & `taskara-0.1.92.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2024-04-17 17:09:32.374116 taskara-0.1.91/LICENSE
--rw-r--r--   0        0        0     2060 2024-05-18 03:15:36.175112 taskara-0.1.91/README.md
--rw-r--r--   0        0        0     1149 2024-05-23 03:44:29.517271 taskara-0.1.91/pyproject.toml
--rw-r--r--   0        0        0       81 2024-04-30 21:36:12.359132 taskara-0.1.91/taskara/__init__.py
--rw-r--r--   0        0        0     1725 2024-04-30 21:35:45.162984 taskara-0.1.91/taskara/agent.py
--rw-r--r--   0        0        0       23 2024-04-25 16:52:45.140876 taskara-0.1.91/taskara/auth/default.py
--rw-r--r--   0        0        0     2548 2024-05-18 03:15:36.178446 taskara-0.1.91/taskara/auth/key.py
--rw-r--r--   0        0        0     3106 2024-05-18 03:15:36.178774 taskara-0.1.91/taskara/auth/provider.py
--rw-r--r--   0        0        0     1446 2024-05-18 03:15:36.179051 taskara-0.1.91/taskara/auth/transport.py
--rw-r--r--   0        0        0    12082 2024-05-23 03:34:03.414355 taskara-0.1.91/taskara/benchmark.py
--rw-r--r--   0        0        0     3250 2024-05-18 03:15:36.179410 taskara-0.1.91/taskara/cli/main.py
--rw-r--r--   0        0        0      672 2024-05-23 03:23:29.445785 taskara-0.1.91/taskara/config.py
--rw-r--r--   0        0        0     2128 2024-05-23 03:34:03.414774 taskara-0.1.91/taskara/db/conn.py
--rw-r--r--   0        0        0     3504 2024-05-23 03:34:03.415046 taskara-0.1.91/taskara/db/models.py
--rw-r--r--   0        0        0      195 2024-04-30 21:35:42.361364 taskara-0.1.91/taskara/env.py
--rw-r--r--   0        0        0     1520 2024-04-30 21:35:40.978077 taskara-0.1.91/taskara/metrics.py
--rw-r--r--   0        0        0    12133 2024-05-22 04:12:34.676830 taskara-0.1.91/taskara/runtime/base.py
--rw-r--r--   0        0        0    14316 2024-05-23 03:44:21.827171 taskara-0.1.91/taskara/runtime/docker.py
--rw-r--r--   0        0        0    30554 2024-05-23 03:34:03.415905 taskara-0.1.91/taskara/runtime/kube.py
--rw-r--r--   0        0        0     1983 2024-05-18 03:15:36.181027 taskara-0.1.91/taskara/runtime/load.py
--rw-r--r--   0        0        0    16258 2024-05-23 03:34:03.416381 taskara-0.1.91/taskara/runtime/process.py
--rw-r--r--   0        0        0     2243 2024-05-18 03:15:36.181763 taskara-0.1.91/taskara/server/app.py
--rw-r--r--   0        0        0     3511 2024-05-23 03:34:03.416593 taskara-0.1.91/taskara/server/models.py
--rw-r--r--   0        0        0     8468 2024-05-18 03:15:36.182433 taskara-0.1.91/taskara/server/router/tasks.py
--rw-r--r--   0        0        0    36105 2024-05-23 03:34:03.417001 taskara-0.1.91/taskara/task.py
--rw-r--r--   0        0        0     1822 2024-05-20 20:35:44.827574 taskara-0.1.91/taskara/util.py
--rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 taskara-0.1.91/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-17 17:09:32.374116 taskara-0.1.92/LICENSE
+-rw-r--r--   0        0        0     2060 2024-05-18 03:15:36.175112 taskara-0.1.92/README.md
+-rw-r--r--   0        0        0     1171 2024-05-27 19:24:00.552013 taskara-0.1.92/pyproject.toml
+-rw-r--r--   0        0        0       93 2024-05-23 21:05:47.914823 taskara-0.1.92/taskara/__init__.py
+-rw-r--r--   0        0        0     1725 2024-04-30 21:35:45.162984 taskara-0.1.92/taskara/agent.py
+-rw-r--r--   0        0        0       23 2024-04-25 16:52:45.140876 taskara-0.1.92/taskara/auth/default.py
+-rw-r--r--   0        0        0     2548 2024-05-18 03:15:36.178446 taskara-0.1.92/taskara/auth/key.py
+-rw-r--r--   0        0        0     3106 2024-05-18 03:15:36.178774 taskara-0.1.92/taskara/auth/provider.py
+-rw-r--r--   0        0        0     1446 2024-05-18 03:15:36.179051 taskara-0.1.92/taskara/auth/transport.py
+-rw-r--r--   0        0        0    12065 2024-05-27 17:42:48.069524 taskara-0.1.92/taskara/benchmark.py
+-rw-r--r--   0        0        0     3250 2024-05-18 03:15:36.179410 taskara-0.1.92/taskara/cli/main.py
+-rw-r--r--   0        0        0      672 2024-05-23 03:23:29.445785 taskara-0.1.92/taskara/config.py
+-rw-r--r--   0        0        0     2128 2024-05-23 03:34:03.414774 taskara-0.1.92/taskara/db/conn.py
+-rw-r--r--   0        0        0     3504 2024-05-23 03:34:03.415046 taskara-0.1.92/taskara/db/models.py
+-rw-r--r--   0        0        0      195 2024-04-30 21:35:42.361364 taskara-0.1.92/taskara/env.py
+-rw-r--r--   0        0        0     1520 2024-04-30 21:35:40.978077 taskara-0.1.92/taskara/metrics.py
+-rw-r--r--   0        0        0    12137 2024-05-23 03:59:01.085005 taskara-0.1.92/taskara/runtime/base.py
+-rw-r--r--   0        0        0    14316 2024-05-23 03:44:21.827171 taskara-0.1.92/taskara/runtime/docker.py
+-rw-r--r--   0        0        0    30554 2024-05-23 03:34:03.415905 taskara-0.1.92/taskara/runtime/kube.py
+-rw-r--r--   0        0        0     1983 2024-05-18 03:15:36.181027 taskara-0.1.92/taskara/runtime/load.py
+-rw-r--r--   0        0        0    16258 2024-05-23 03:34:03.416381 taskara-0.1.92/taskara/runtime/process.py
+-rw-r--r--   0        0        0     2243 2024-05-18 03:15:36.181763 taskara-0.1.92/taskara/server/app.py
+-rw-r--r--   0        0        0     3514 2024-05-23 03:59:01.025899 taskara-0.1.92/taskara/server/models.py
+-rw-r--r--   0        0        0     8554 2024-05-23 21:06:30.131717 taskara-0.1.92/taskara/server/router/tasks.py
+-rw-r--r--   0        0        0    36645 2024-05-23 23:07:24.530078 taskara-0.1.92/taskara/task.py
+-rw-r--r--   0        0        0     1822 2024-05-20 20:35:44.827574 taskara-0.1.92/taskara/util.py
+-rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 taskara-0.1.92/PKG-INFO
```

### Comparing `taskara-0.1.91/LICENSE` & `taskara-0.1.92/LICENSE`

 * *Files identical despite different names*

### Comparing `taskara-0.1.91/README.md` & `taskara-0.1.92/README.md`

 * *Files identical despite different names*

### Comparing `taskara-0.1.91/pyproject.toml` & `taskara-0.1.92/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskara"
-version = "0.1.91"
+version = "0.1.92"
 description = "Task management for AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -14,16 +14,17 @@
 docker = {version = "^7.0.0", optional = true}
 kubernetes = {version = "^29.0.0", optional = true}
 google-auth = {version = "^2.29.0", optional = true}
 google-cloud-container = {version = "^2.45.0", optional = true}
 namesgenerator = "^0.3"
 typer = {version = "^0.12.3", optional = true}
 tabulate = {version = "^0.9.0", optional = true}
-skillpacks = "^0.1.29"
 devicebay = "^0.1.25"
+shortuuid = "^1.0.13"
+skillpacks = "^0.1.30"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 flake8 = "^7.0.0"
 black = "^24.2.0"
 pytest-env = "^1.1.3"
```

### Comparing `taskara-0.1.91/taskara/agent.py` & `taskara-0.1.92/taskara/agent.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.91/taskara/auth/key.py` & `taskara-0.1.92/taskara/auth/key.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.91/taskara/auth/provider.py` & `taskara-0.1.92/taskara/auth/provider.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.91/taskara/auth/transport.py` & `taskara-0.1.92/taskara/auth/transport.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.91/taskara/benchmark.py` & `taskara-0.1.92/taskara/benchmark.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import List, Optional, Type, Dict, Any
-import uuid
 import json
 import time
+from typing import Any, Dict, List, Optional, Type
 
+import shortuuid
 from devicebay import V1Device, V1DeviceType
 from pydantic import BaseModel
 
-from taskara.task import Task
 from taskara.db.conn import WithDB
 from taskara.db.models import (
-    TaskTemplateRecord,
     BenchmarkRecord,
+    TaskTemplateRecord,
     benchmark_task_association,
 )
-from taskara.server.models import V1TaskTemplate, V1TaskTemplates, V1Benchmark
+from taskara.server.models import V1Benchmark, V1TaskTemplate
+from taskara.task import Task
 
 
 class TaskTemplate(WithDB):
     """A task template"""
 
     def __init__(
         self,
@@ -27,15 +27,15 @@
         device: Optional[V1Device] = None,
         device_type: Optional[V1DeviceType] = None,
         expect: Optional[Type[BaseModel]] = None,
         parameters: Dict[str, Any] = {},
         labels: Dict[str, str] = {},
         tags: List[str] = [],
     ) -> None:
-        self._id = str(uuid.uuid4())
+        self._id = shortuuid.uuid()
         self._description = description
         self._max_steps = max_steps
         self._owner_id = owner_id
         self._device = device
         self._device_type = device_type
         self._expect_schema = expect.model_json_schema() if expect else None
         self._parameters = parameters
@@ -204,15 +204,15 @@
     ) -> "TaskTemplate":
         obj = cls.__new__(cls)
 
         owner_id = owner_id if owner_id else v1.owner_id
         if not owner_id:
             raise ValueError("Owner id is required in v1 or as parameter")
 
-        obj._id = v1.id if v1.id else str(uuid.uuid4())
+        obj._id = v1.id if v1.id else shortuuid.uuid()
         obj._owner_id = owner_id
         obj._description = v1.description
         obj._max_steps = v1.max_steps
         obj._device = v1.device
         obj._device_type = v1.device_type
         obj._expect_schema = v1.expect_schema
         obj._parameters = v1.parameters
@@ -239,15 +239,15 @@
         tasks: List[TaskTemplate],
         owner_id: Optional[str] = None,
         labels: Dict[str, str] = {},
         tags: List[str] = [],
         public: bool = False,
     ):
         self._tasks = tasks
-        self._id = str(uuid.uuid4())
+        self._id = shortuuid.uuid()
         self._name = name
         self._description = description
         self._owner_id = owner_id
         self._labels = labels
         self._tags = tags
         self._public = public
         self._created = time.time()
@@ -338,15 +338,15 @@
         tasks = [TaskTemplate.from_v1(task) for task in v1.tasks]
 
         obj = cls.__new__(cls)
         owner_id = owner_id if owner_id else v1.owner_id
         if not owner_id:
             raise ValueError("Owner id is required in v1 or as parameter")
 
-        obj._id = v1.id if v1.id else str(uuid.uuid4())
+        obj._id = v1.id if v1.id else shortuuid.uuid()
         obj._owner_id = owner_id
         obj._name = v1.name
         obj._description = v1.description
         obj._tasks = tasks
         obj._labels = v1.labels
         obj._tags = v1.tags
         obj._created = v1.created
@@ -380,15 +380,15 @@
         self,
         benchmark: Benchmark,
         assigned_to: str | None = None,
         assigned_type: str | None = None,
         remote: str | None = None,
         owner_id: str | None = None,
     ) -> None:
-        self._id = str(uuid.uuid4())
+        self._id = shortuuid.uuid()
         self._benchmark = benchmark
         self._tasks: List[Task] = []
         self._owner_id = owner_id
 
         for tpl in self._benchmark.tasks:
             task = tpl.to_task(
                 assigned_to=assigned_to,
```

### Comparing `taskara-0.1.91/taskara/cli/main.py` & `taskara-0.1.92/taskara/cli/main.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.91/taskara/config.py` & `taskara-0.1.92/taskara/config.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.91/taskara/db/conn.py` & `taskara-0.1.92/taskara/db/conn.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.91/taskara/db/models.py` & `taskara-0.1.92/taskara/db/models.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.91/taskara/metrics.py` & `taskara-0.1.92/taskara/metrics.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.91/taskara/runtime/base.py` & `taskara-0.1.92/taskara/runtime/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, TypeVar, Type, Generic, Union, Iterator, Optional, Dict, Tuple
 from abc import ABC, abstractmethod
-import uuid
+import shortuuid
 import time
 import json
 
 from pydantic import BaseModel
 
 from taskara.db.conn import WithDB
 from taskara.db.models import TrackerRecord
@@ -27,15 +27,15 @@
         name: str,
         port: int,
         runtime: "TrackerRuntime",
         status: str = "running",
         owner_id: Optional[str] = None,
         labels: Optional[Dict[str, str]] = None,
     ) -> None:
-        self._id = str(uuid.uuid4())
+        self._id = shortuuid.uuid()
         self._name = name
         self._port = port
         self._status = status
         self._runtime = runtime
         self._owner_id = owner_id
         self._created = time.time()
         self._updated = time.time()
```

### Comparing `taskara-0.1.91/taskara/runtime/docker.py` & `taskara-0.1.92/taskara/runtime/docker.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.91/taskara/runtime/kube.py` & `taskara-0.1.92/taskara/runtime/kube.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.91/taskara/runtime/load.py` & `taskara-0.1.92/taskara/runtime/load.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.91/taskara/runtime/process.py` & `taskara-0.1.92/taskara/runtime/process.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.91/taskara/server/app.py` & `taskara-0.1.92/taskara/server/app.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.91/taskara/server/models.py` & `taskara-0.1.92/taskara/server/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional, List, Dict, Any
-import uuid
+import shortuuid
 import time
 
 from threadmem.server.models import V1RoleThread
 from pydantic import BaseModel, Field
 from devicebay.models import V1Device
 from devicebay import V1Device, V1DeviceType
 from mllm import V1Prompt
@@ -17,15 +17,15 @@
     output: Optional[str] = None
     assigned_to: Optional[str] = None
     completed: Optional[float] = None
     version: Optional[str] = None
 
 
 class V1Task(BaseModel):
-    id: str = Field(default_factory=lambda: str(uuid.uuid4()))
+    id: str = Field(default_factory=lambda: shortuuid.uuid())
     description: str
     max_steps: int = 30
     device: Optional[V1Device] = None
     device_type: Optional[V1DeviceType] = None
     expect_schema: Optional[Dict[str, Any]] = None
     status: Optional[str] = None
     threads: Optional[List[V1RoleThread]] = None
@@ -47,15 +47,15 @@
 
 
 class V1Tasks(BaseModel):
     tasks: List[V1Task]
 
 
 class V1TaskTemplate(BaseModel):
-    id: str = Field(default_factory=lambda: str(uuid.uuid4()))
+    id: str = Field(default_factory=lambda: shortuuid.uuid())
     description: str
     max_steps: int = 30
     device: Optional[V1Device] = None
     device_type: Optional[V1DeviceType] = None
     expect_schema: Optional[Dict[str, Any]] = None
     parameters: Optional[Dict[str, Any]] = {}
     owner_id: Optional[str] = None
```

### Comparing `taskara-0.1.91/taskara/server/router/tasks.py` & `taskara-0.1.92/taskara/server/router/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 
 from fastapi import APIRouter, Depends, HTTPException
 from threadmem import RoleMessage, RoleThread, V1RoleThreads, V1RoleThread
 from mllm import Prompt, V1Prompt
 from skillpacks import V1ActionEvent, ActionEvent, V1Episode, Episode
 
-from taskara import Task
+from taskara import Task, TaskStatus
 from taskara.server.models import (
     V1TaskUpdate,
     V1Task,
     V1Tasks,
     V1UserProfile,
     V1PostMessage,
     V1AddThread,
@@ -36,22 +36,24 @@
         if not episodes:
             raise HTTPException(status_code=404, detail="Episode not found")
         episode = episodes[0]
 
     if not episode:
         episode = Episode()
 
+    status = data.status or "created"
+    task_status = TaskStatus(status)
     task = Task(
         id=data.id,
         max_steps=data.max_steps,
         device=data.device,
         device_type=data.device_type,
         owner_id=current_user.email,
         description=data.description,
-        status=data.status or "created",
+        status=task_status,
         parameters=data.parameters if data.parameters else {},
         assigned_to=data.assigned_to,
         assigned_type=data.assigned_type,
         labels=data.labels if data.labels else {},
         tags=data.tags if data.tags else [],
         episode=episode,
     )
@@ -101,15 +103,15 @@
         raise HTTPException(status_code=404, detail="Task not found")
     task = task[0]
 
     logger.debug(f"found task: {task.__dict__}")
     if data.description:
         task.description = data.description
     if data.status:
-        task.status = data.status
+        task.status = TaskStatus(data.status)
     if data.assigned_to:
         task.assigned_to = data.assigned_to
     if data.error:
         task.error = data.error
     if data.output:
         task.output = data.output
     if data.completed:
```

### Comparing `taskara-0.1.91/taskara/task.py` & `taskara-0.1.92/taskara/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,61 @@
-import uuid
-import time
-from typing import List, Optional, TypeVar, Any, Dict, Type
-import requests
-import os
-import json
+import copy
 import hashlib
+import json
 import logging
-import copy
+import os
+import time
+from enum import Enum
+from typing import Any, Dict, List, Optional, Type, TypeVar
 
-from threadmem import RoleThread, RoleMessage, V1RoleThreads
-from mllm import Prompt, V1Prompt
-from skillpacks import Episode, ActionEvent, V1Action, V1ToolRef, V1Episode
+import requests
+import shortuuid
 from devicebay import V1Device, V1DeviceType
+from mllm import Prompt, V1Prompt
 from pydantic import BaseModel
+from skillpacks import ActionEvent, Episode, V1Action, V1Episode, V1ToolRef
+from threadmem import RoleMessage, RoleThread, V1RoleThreads
 
-from .db.models import TaskRecord
 from .db.conn import WithDB
-from .server.models import V1Prompts, V1Task, V1TaskUpdate, V1Tasks
+from .db.models import TaskRecord
 from .env import HUB_API_KEY_ENV
+from .server.models import V1Prompts, V1Task, V1Tasks, V1TaskUpdate
 
 T = TypeVar("T", bound="Task")
 logger = logging.getLogger(__name__)
 
 
+class TaskStatus(Enum):
+    """Task status"""
+
+    DEFINED = "defined"
+    CREATED = "created"
+    RUNNING = "running"
+    COMPLETED = "completed"
+    FAILED = "failed"
+    ERROR = "error"
+    WAITING = "waiting"
+    CANCELING = "canceling"
+    CANCELED = "canceled"
+    REVIEW = "review"
+
+
 class Task(WithDB):
     """An agent task"""
 
     def __init__(
         self,
         description: Optional[str] = None,
         max_steps: int = 30,
         owner_id: Optional[str] = None,
         device: Optional[V1Device] = None,
         device_type: Optional[V1DeviceType] = None,
         expect: Optional[Type[BaseModel]] = None,
         id: Optional[str] = None,
-        status: str = "defined",
+        status: TaskStatus = TaskStatus.DEFINED,
         created: Optional[float] = None,
         started: float = 0.0,
         completed: float = 0.0,
         threads: List[RoleThread] = [],
         prompts: List[Prompt] = [],
         assigned_to: Optional[str] = None,
         assigned_type: Optional[str] = None,
@@ -48,15 +64,15 @@
         parameters: Dict[str, Any] = {},
         remote: Optional[str] = None,
         version: Optional[str] = None,
         labels: Dict[str, str] = {},
         tags: List[str] = [],
         episode: Optional[Episode] = None,
     ):
-        self._id = id if id is not None else str(uuid.uuid4())
+        self._id = id if id is not None else shortuuid.uuid()
         self._description = description
         self._max_steps = max_steps
         self._owner_id = owner_id
         self._device = device
         self._device_type = device_type
         self._status = status
         self._created = created if created is not None else time.time()
@@ -149,19 +165,19 @@
         return self._owner_id
 
     @owner_id.setter
     def owner_id(self, value: Optional[str]):
         self._owner_id = value
 
     @property
-    def status(self) -> str:
+    def status(self) -> TaskStatus:
         return self._status
 
     @status.setter
-    def status(self, value: str):
+    def status(self, value: TaskStatus):
         self._status = value
 
     @property
     def created(self) -> float:
         return self._created
 
     @created.setter
@@ -285,15 +301,15 @@
             id=self._id,
             owner_id=self._owner_id,
             description=self._description,
             max_steps=self._max_steps,
             device=device,
             device_type=device_type,
             expect=expect,
-            status=self._status,
+            status=self._status.value,
             created=self._created,
             started=self._started,
             completed=self._completed,
             assigned_to=self._assigned_to,
             assigned_type=self._assigned_type,
             error=self._error,
             output=self._output,
@@ -335,15 +351,15 @@
         obj._id = record.id
         obj._owner_id = record.owner_id
         obj._description = record.description
         obj._max_steps = record.max_steps
         obj._device = device
         obj._device_type = device_type
         obj._expect_schema = expect
-        obj._status = record.status
+        obj._status = TaskStatus(record.status)
         obj._created = record.created
         obj._started = record.started
         obj._completed = record.completed
         obj._assigned_to = record.assigned_to
         obj._assigned_type = record.assigned_type
         obj._error = record.error
         obj._output = record.output
@@ -552,15 +568,15 @@
         Returns:
             Task: A new Task instance that is a copy of the current instance with a new unique ID and timestamps.
         """
         # Use the copy.deepcopy function to ensure that all mutable objects are also copied.
         copied_task = copy.deepcopy(self)
 
         # Resetting the unique ID and timestamps
-        copied_task._id = str(uuid.uuid4())
+        copied_task._id = shortuuid.uuid()
         now = time.time()
         copied_task._created = now
         copied_task._started = 0.0
         copied_task._completed = 0.0
 
         # Assuming you may want to start with an undefined status or any other initial value
         copied_task._status = "defined"
@@ -868,15 +884,15 @@
             description=self._description if self._description else "",
             max_steps=self._max_steps,
             device=self._device,
             device_type=self.device_type,
             expect_schema=self._expect_schema,
             threads=[t.to_v1() for t in self._threads],
             prompts=[p.id for p in self._prompts],
-            status=self._status,
+            status=self._status.value,
             created=self._created,
             started=self._started,
             completed=self._completed,
             assigned_to=self._assigned_to,
             assigned_type=self._assigned_type,
             error=self._error,
             output=self._output,
@@ -889,15 +905,15 @@
             episode_id=episode_id,
         )
 
     def to_update_v1(self) -> V1TaskUpdate:
         return V1TaskUpdate(
             description=self._description,
             max_steps=self._max_steps,
-            status=self._status,
+            status=self._status.value,
             assigned_to=self._assigned_to,
             error=self._error,
             output=self._output,
             completed=self._completed,
             version=self._version,
         )
 
@@ -905,23 +921,26 @@
     def from_v1(cls, v1: V1Task, owner_id: Optional[str] = None) -> "Task":
         obj = cls.__new__(cls)  # Create a new instance without calling __init__
 
         owner_id = owner_id if owner_id else v1.owner_id
         if not owner_id:
             raise ValueError("Owner id is required in v1 or as parameter")
 
+        status = v1.status if v1.status else "defined"
+        task_status = TaskStatus(status)
+
         # Manually set attributes on the object
-        obj._id = v1.id if v1.id else str(uuid.uuid4())
+        obj._id = v1.id if v1.id else shortuuid.uuid()
         obj._owner_id = owner_id
         obj._description = v1.description
         obj._max_steps = v1.max_steps
         obj._device = v1.device
         obj._device_type = v1.device_type
         obj._expect_schema = v1.expect_schema
-        obj._status = v1.status if v1.status else "defined"
+        obj._status = task_status
         obj._created = v1.created
         obj._started = v1.started
         obj._completed = v1.completed
         obj._assigned_to = v1.assigned_to
         obj._assigned_type = v1.assigned_type
         obj._error = v1.error
         obj._output = v1.output
@@ -959,20 +978,22 @@
 
                 remote_task = self._remote_request(
                     self._remote, "GET", f"/v1/tasks/{self._id}", auth_token=auth_token
                 )
                 logger.debug(f"found remote task {remote_task}")
                 if remote_task:
                     v1 = V1Task(**remote_task)
+                    status = v1.status if v1.status else "defined"
+                    task_status = TaskStatus(status)
                     self._description = v1.description
                     self._max_steps = v1.max_steps
                     self._device = v1.device
                     self._device_type = v1.device_type
                     self._expect_schema = v1.expect_schema
-                    self._status = v1.status if v1.status else "defined"
+                    self._status = task_status
                     self._created = v1.created
                     self._started = v1.started
                     self._completed = v1.completed
                     self._assigned_to = v1.assigned_to
                     self._assigned_type = v1.assigned_type
                     self._error = v1.error
                     self._output = v1.output
```

### Comparing `taskara-0.1.91/taskara/util.py` & `taskara-0.1.92/taskara/util.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.91/PKG-INFO` & `taskara-0.1.92/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskara
-Version: 0.1.91
+Version: 0.1.92
 Summary: Task management for AI agents
 License: MIT
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,16 @@
 Requires-Dist: devicebay (>=0.1.25,<0.2.0)
 Requires-Dist: docker (>=7.0.0,<8.0.0) ; extra == "runtime" or extra == "all"
 Requires-Dist: google-auth (>=2.29.0,<3.0.0) ; extra == "runtime" or extra == "all"
 Requires-Dist: google-cloud-container (>=2.45.0,<3.0.0) ; extra == "runtime" or extra == "all"
 Requires-Dist: kubernetes (>=29.0.0,<30.0.0) ; extra == "runtime" or extra == "all"
 Requires-Dist: namesgenerator (>=0.3,<0.4)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
-Requires-Dist: skillpacks (>=0.1.29,<0.2.0)
+Requires-Dist: shortuuid (>=1.0.13,<2.0.0)
+Requires-Dist: skillpacks (>=0.1.30,<0.2.0)
 Requires-Dist: sqlalchemy (>=2.0.29,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0) ; extra == "cli" or extra == "all"
 Requires-Dist: threadmem (>=0.2.26,<0.3.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0) ; extra == "cli" or extra == "all"
 Description-Content-Type: text/markdown
 
 <!-- PROJECT LOGO -->
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: taskara Version: 0.1.91 Summary: Task management
+Metadata-Version: 2.1 Name: taskara Version: 0.1.92 Summary: Task management
 for AI agents License: MIT Author: Patrick Barker Author-email:
 patrickbarkerco@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: all Provides-Extra: cli Provides-
 Extra: runtime Requires-Dist: devicebay (>=0.1.25,<0.2.0) Requires-Dist: docker
 (>=7.0.0,<8.0.0) ; extra == "runtime" or extra == "all" Requires-Dist: google-
 auth (>=2.29.0,<3.0.0) ; extra == "runtime" or extra == "all" Requires-Dist:
 google-cloud-container (>=2.45.0,<3.0.0) ; extra == "runtime" or extra == "all"
 Requires-Dist: kubernetes (>=29.0.0,<30.0.0) ; extra == "runtime" or extra ==
 "all" Requires-Dist: namesgenerator (>=0.3,<0.4) Requires-Dist: pydantic
-(>=2.6.4,<3.0.0) Requires-Dist: skillpacks (>=0.1.29,<0.2.0) Requires-Dist:
-sqlalchemy (>=2.0.29,<3.0.0) Requires-Dist: tabulate (>=0.9.0,<0.10.0) ; extra
-== "cli" or extra == "all" Requires-Dist: threadmem (>=0.2.26,<0.3.0) Requires-
-Dist: typer (>=0.12.3,<0.13.0) ; extra == "cli" or extra == "all" Description-
-Content-Type: text/markdown
+(>=2.6.4,<3.0.0) Requires-Dist: shortuuid (>=1.0.13,<2.0.0) Requires-Dist:
+skillpacks (>=0.1.30,<0.2.0) Requires-Dist: sqlalchemy (>=2.0.29,<3.0.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0) ; extra == "cli" or extra == "all"
+Requires-Dist: threadmem (>=0.2.26,<0.3.0) Requires-Dist: typer
+(>=0.12.3,<0.13.0) ; extra == "cli" or extra == "all" Description-Content-Type:
+text/markdown
                              ************ TTaasskkaarraa ************
                         Task management for AI agents
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 
                   _V_i_e_w_ _D_e_m_o Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 
 ## Installation ```sh pip install taskara ``` ## Usage Create a task ```python
```

