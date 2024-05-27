# Comparing `tmp/postgres-tq-0.0.6.tar.gz` & `tmp/postgres_tq-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgres-tq-0.0.6.tar", last modified: Tue Feb 13 11:24:30 2024, max compression
+gzip compressed data, was "postgres_tq-1.0.0.tar", last modified: Mon May 27 10:11:31 2024, max compression
```

## Comparing `postgres-tq-0.0.6.tar` & `postgres_tq-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 11:24:30.040675 postgres-tq-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-02-13 11:24:16.000000 postgres-tq-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-02-13 11:24:30.040675 postgres-tq-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-02-13 11:24:16.000000 postgres-tq-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 11:24:30.040675 postgres-tq-0.0.6/postgres_tq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-02-13 11:24:30.000000 postgres-tq-0.0.6/postgres_tq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-13 11:24:30.000000 postgres-tq-0.0.6/postgres_tq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 11:24:30.000000 postgres-tq-0.0.6/postgres_tq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-13 11:24:30.000000 postgres-tq-0.0.6/postgres_tq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-13 11:24:30.000000 postgres-tq-0.0.6/postgres_tq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 11:24:30.040675 postgres-tq-0.0.6/postgrestq/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-13 11:24:16.000000 postgres-tq-0.0.6/postgrestq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17772 2024-02-13 11:24:16.000000 postgres-tq-0.0.6/postgrestq/task_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-02-13 11:24:16.000000 postgres-tq-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 11:24:30.040675 postgres-tq-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 11:24:30.040675 postgres-tq-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8336 2024-02-13 11:24:16.000000 postgres-tq-0.0.6/tests/test_task_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:11:31.761587 postgres_tq-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-27 10:11:18.000000 postgres_tq-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-05-27 10:11:31.761587 postgres_tq-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-05-27 10:11:18.000000 postgres_tq-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:11:31.757588 postgres_tq-1.0.0/postgres_tq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-05-27 10:11:31.000000 postgres_tq-1.0.0/postgres_tq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-27 10:11:31.000000 postgres_tq-1.0.0/postgres_tq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 10:11:31.000000 postgres_tq-1.0.0/postgres_tq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-27 10:11:31.000000 postgres_tq-1.0.0/postgres_tq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 10:11:31.000000 postgres_tq-1.0.0/postgres_tq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:11:31.757588 postgres_tq-1.0.0/postgrestq/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-27 10:11:18.000000 postgres_tq-1.0.0/postgrestq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 10:11:18.000000 postgres_tq-1.0.0/postgrestq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    23221 2024-05-27 10:11:18.000000 postgres_tq-1.0.0/postgrestq/task_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-27 10:11:18.000000 postgres_tq-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 10:11:31.761587 postgres_tq-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:11:31.757588 postgres_tq-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-05-27 10:11:18.000000 postgres_tq-1.0.0/tests/test_task_queue.py
```

### Comparing `postgres-tq-0.0.6/LICENSE` & `postgres_tq-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `postgres-tq-0.0.6/PKG-INFO` & `postgres_tq-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,138 +1,101 @@
 Metadata-Version: 2.1
 Name: postgres-tq
-Version: 0.0.6
+Version: 1.0.0
 Summary: Postgres Based Task Queue
 Author-email: FlixTech <open-source@flixbus.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: psycopg[binary]>=3.1.12
 
 [![postgres-tq Actions Status](https://github.com/flix-tech/postgres-tq/workflows/CI/CD%20Pipeline/badge.svg?branch=main)](https://github.com/flix-tech/postgres-tq/actions)
 [![License](https://img.shields.io/github/license/flix-tech/postgres-tq)](https://pypi.org/project/postgres-tq/)
 [![PyPI - Python Version](https://img.shields.io/pypi/v/postgres-tq)](https://pypi.org/project/postgres-tq/)
 
 # Postgres Task Queue
 
-This repo will contain the [Postgres](https://www.postgresql.org/) based task queue logic, similar to [our redis-tq](https://github.com/flix-tech/redis-tq) but based on postgres instead.
+This library makes it possible to define a list of tasks to be persisted in a Postgres database and executed by multiple workers. Tasks are retried automatically after a given timeout and for a given number of time. Tasks are persisted in the database and executed in order of insertion unless a specific start timestamp is provided.
+
+This is similar to [our redis-tq](https://github.com/flix-tech/redis-tq) but based on Postgres thanks to the `FOR UPDATE SKIP LOCKED` feature.
 
 Similar to redis-tq, this package allows for sharing data between multiple processes or hosts.
 
 Tasks support a "lease time". After that time other workers may consider this client to have crashed or stalled and pick up the item instead. The number of retries can also be configured.
 
 By default it keeps all the queues and tasks in a single table `task_queue`. If you want to use a different table for different queues for example it could also be configured when instantiating the queue.
 
-You can either set the `create_table=True` when instantiating the queue or create the table yourself with the following query:
+You can set the `create_table=True` when instantiating the queue to have the table created for you. If the table already exist it will not be touched.
 
-```sql
-CREATE TABLE task_queue (
-    id UUID PRIMARY KEY,
-    queue_name TEXT NOT NULL,
-    task JSONB NOT NULL,
-    ttl INT NOT NULL,
-    created_at TIMESTAMP NOT NULL DEFAULT CURRENT_TIMESTAMP,
-    processing BOOLEAN NOT NULL DEFAULT false,
-    lease_timeout FLOAT,
-    deadline TIMESTAMP,
-    completed_at TIMESTAMP
-)
-```
+When defining a task you can provide a `can_start_at` timestamp parameter, and the task will not be executed until then, which can be useful to schedule tasks. By default the current timestamp is used.
 
 ## Installation
 
 postgres-tq is available on [PyPI][] so you can simply install via:
 
 ```bash
 $ pip install postgres-tq
 ```
 
 [PyPI]: https://pypi.org/project/postgres-tq/
 
-## How it works
-
-It uses row level locks of postgres to mimic the atomic pop and atomic push of redis-tq when getting a new task from the queue:
-
-```sql
-UPDATE task_queue
-SET processing = true,
-    deadline =
-        current_timestamp + CAST(lease_timeout || ' seconds' AS INTERVAL)
-WHERE id = (
-    SELECT id
-    FROM task_queue
-    WHERE completed_at IS NULL
-        AND processing = false
-        AND queue_name = <your_queue_name>
-        AND ttl > 0
-    ORDER BY created_at
-    FOR UPDATE SKIP LOCKED
-    LIMIT 1
-)
-RETURNING id, task;
-```
-
-Let's say two workers try to get a new task at the same time, assuming that they will probably see the same task to be picked up using the subquery:
-
-```sql
-SELECT id
-FROM task_queue
-WHERE completed_at IS NULL
-    AND processing = false
-    AND queue_name = <your_queue_name>
-    AND ttl > 0
-ORDER BY created_at
-```
-
-The first worker locks the row with the `FOR UPDATE` clause until the update is completed and committed. If we hadn't used the `SKIP LOCKED` clause, the second worker would have seen the same row and waited for the first worker to finish the update. However, since the first worker already updated it, the subquery would no longer be valid, and the second worker would return zero rows because `WHERE id = NULL`.
-
-However, since we are using `FOR UPDATE SKIP LOCKED` the first worker locks the row for update and the second worker, skips that locked row and chooses another row for itself to update. This way we can avoid the race condition.
-
-The other methods `complete()` and `reschedule()` work similarly under the hood.
-
 ## How to use
 
 On the producing side, populate the queue with tasks and a respective lease timeout:
 
 ```py
+from datetime import datetime, UTC, timedelta
 from postgrestq import TaskQueue
 
-task_queue = TaskQueue(POSTGRES_CONN_STR, queue_name, reset=True)
+task_queue = TaskQueue(
+    POSTGRES_CONN_STR,
+    queue_name, # name of the queue as a string
+    reset=True, # delete existing tasks for this queue
+    ttl_zero_callback=handle_failure, # will call handle_failure(task_id, task) when the task failed too many times
+)
 
 for i in range(10):
-    task_queue.add(some_task, lease_timeout, ttl=3)
+    task_queue.add(
+        some_task,
+        lease_timeout, # in seconds, after this interval it will be assumed to have failed (and the callback is called)
+        ttl=3, # attempts before abandoning
+        can_start_at=datetime.now(UTC) + timedelta(minutes=5), # start it not before than 5 minutes in the future
+    )
 ```
 
 On the consuming side:
 
 ```py
 from postgrestq import TaskQueue
 
 task_queue = TaskQueue(POSTGRES_CONN_STR, queue_name, reset=True)
 while True:
-    task, task_id = task_queue.get()
+    task, task_id, _queue_name = task_queue.get()
     if task is not None:
         # do something with task and mark it as complete afterwards
         task_queue.complete(task_id)
     if task_queue.is_empty():
         break
     # task_queue.get is non-blocking, so you may want to sleep a
     # bit before the next iteration
     time.sleep(1)
 ```
 
+Notice that `get()` returns the queue name too, in case in future multi-queue is implemented.
+At the moment it's always the same as the queue_name given to the class.
+
 Or you can even use the \_\_iter\_\_() method of the class TaskQueue and loop over the queue:
 
 ```py
 from postgrestq import TaskQueue
 
 task_queue = TaskQueue(POSTGRES_CONN_STR, queue_name, reset=True)
 
-for task, id_ in taskqueue:
+for task, id_, queue_name in taskqueue:
     # do something with task and it's automatically
     # marked as completed by the iterator at the end
     # of the iteration
 
 ```
 
 If the consumer crashes (i.e. the task is not marked as completed after lease_timeout seconds), the task will be put back into the task queue. This rescheduling will happen at most ttl times and then the task will be dropped. A callback can be provided if you want to monitor such cases.
@@ -151,14 +114,56 @@
 # Prune all tasks from queue completed more than 1 hour (in seconds)
 # ago. Tasks in progress, not started and completed recently will
 # stay in the postgres task_queue table
 task_queue.prune_completed_tasks(3600)
 
 ```
 
+
+## How it works
+
+It uses row level locks of postgres to mimic the atomic pop and atomic push of redis-tq when getting a new task from the queue:
+
+```sql
+UPDATE task_queue
+SET processing = true,
+    deadline =
+        current_timestamp + CAST(lease_timeout || ' seconds' AS INTERVAL)
+WHERE id = (
+    SELECT id
+    FROM task_queue
+    WHERE completed_at IS NULL
+        AND processing = false
+        AND queue_name = <your_queue_name>
+        AND ttl > 0
+    ORDER BY created_at
+    FOR UPDATE SKIP LOCKED
+    LIMIT 1
+)
+RETURNING id, task;
+```
+
+Let's say two workers try to get a new task at the same time, assuming that they will probably see the same task to be picked up using the subquery:
+
+```sql
+SELECT id
+FROM task_queue
+WHERE completed_at IS NULL
+    AND processing = false
+    AND queue_name = <your_queue_name>
+    AND ttl > 0
+ORDER BY created_at
+```
+
+The first worker locks the row with the `FOR UPDATE` clause until the update is completed and committed. If we hadn't used the `SKIP LOCKED` clause, the second worker would have seen the same row and waited for the first worker to finish the update. However, since the first worker already updated it, the subquery would no longer be valid, and the second worker would return zero rows because `WHERE id = NULL`.
+
+However, since we are using `FOR UPDATE SKIP LOCKED` the first worker locks the row for update and the second worker, skips that locked row and chooses another row for itself to update. This way we can avoid the race condition.
+
+The other methods `complete()` and `reschedule()` work similarly under the hood.
+
 ## Running the tests
 
 The tests will check a presence of an Postgres DB in the port 15432. To initiate one using docker you can run:
 
 ```bash
 $ make run-postgres
 ```
```

### Comparing `postgres-tq-0.0.6/README.md` & `postgres_tq-1.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,127 +1,90 @@
 [![postgres-tq Actions Status](https://github.com/flix-tech/postgres-tq/workflows/CI/CD%20Pipeline/badge.svg?branch=main)](https://github.com/flix-tech/postgres-tq/actions)
 [![License](https://img.shields.io/github/license/flix-tech/postgres-tq)](https://pypi.org/project/postgres-tq/)
 [![PyPI - Python Version](https://img.shields.io/pypi/v/postgres-tq)](https://pypi.org/project/postgres-tq/)
 
 # Postgres Task Queue
 
-This repo will contain the [Postgres](https://www.postgresql.org/) based task queue logic, similar to [our redis-tq](https://github.com/flix-tech/redis-tq) but based on postgres instead.
+This library makes it possible to define a list of tasks to be persisted in a Postgres database and executed by multiple workers. Tasks are retried automatically after a given timeout and for a given number of time. Tasks are persisted in the database and executed in order of insertion unless a specific start timestamp is provided.
+
+This is similar to [our redis-tq](https://github.com/flix-tech/redis-tq) but based on Postgres thanks to the `FOR UPDATE SKIP LOCKED` feature.
 
 Similar to redis-tq, this package allows for sharing data between multiple processes or hosts.
 
 Tasks support a "lease time". After that time other workers may consider this client to have crashed or stalled and pick up the item instead. The number of retries can also be configured.
 
 By default it keeps all the queues and tasks in a single table `task_queue`. If you want to use a different table for different queues for example it could also be configured when instantiating the queue.
 
-You can either set the `create_table=True` when instantiating the queue or create the table yourself with the following query:
+You can set the `create_table=True` when instantiating the queue to have the table created for you. If the table already exist it will not be touched.
 
-```sql
-CREATE TABLE task_queue (
-    id UUID PRIMARY KEY,
-    queue_name TEXT NOT NULL,
-    task JSONB NOT NULL,
-    ttl INT NOT NULL,
-    created_at TIMESTAMP NOT NULL DEFAULT CURRENT_TIMESTAMP,
-    processing BOOLEAN NOT NULL DEFAULT false,
-    lease_timeout FLOAT,
-    deadline TIMESTAMP,
-    completed_at TIMESTAMP
-)
-```
+When defining a task you can provide a `can_start_at` timestamp parameter, and the task will not be executed until then, which can be useful to schedule tasks. By default the current timestamp is used.
 
 ## Installation
 
 postgres-tq is available on [PyPI][] so you can simply install via:
 
 ```bash
 $ pip install postgres-tq
 ```
 
 [PyPI]: https://pypi.org/project/postgres-tq/
 
-## How it works
-
-It uses row level locks of postgres to mimic the atomic pop and atomic push of redis-tq when getting a new task from the queue:
-
-```sql
-UPDATE task_queue
-SET processing = true,
-    deadline =
-        current_timestamp + CAST(lease_timeout || ' seconds' AS INTERVAL)
-WHERE id = (
-    SELECT id
-    FROM task_queue
-    WHERE completed_at IS NULL
-        AND processing = false
-        AND queue_name = <your_queue_name>
-        AND ttl > 0
-    ORDER BY created_at
-    FOR UPDATE SKIP LOCKED
-    LIMIT 1
-)
-RETURNING id, task;
-```
-
-Let's say two workers try to get a new task at the same time, assuming that they will probably see the same task to be picked up using the subquery:
-
-```sql
-SELECT id
-FROM task_queue
-WHERE completed_at IS NULL
-    AND processing = false
-    AND queue_name = <your_queue_name>
-    AND ttl > 0
-ORDER BY created_at
-```
-
-The first worker locks the row with the `FOR UPDATE` clause until the update is completed and committed. If we hadn't used the `SKIP LOCKED` clause, the second worker would have seen the same row and waited for the first worker to finish the update. However, since the first worker already updated it, the subquery would no longer be valid, and the second worker would return zero rows because `WHERE id = NULL`.
-
-However, since we are using `FOR UPDATE SKIP LOCKED` the first worker locks the row for update and the second worker, skips that locked row and chooses another row for itself to update. This way we can avoid the race condition.
-
-The other methods `complete()` and `reschedule()` work similarly under the hood.
-
 ## How to use
 
 On the producing side, populate the queue with tasks and a respective lease timeout:
 
 ```py
+from datetime import datetime, UTC, timedelta
 from postgrestq import TaskQueue
 
-task_queue = TaskQueue(POSTGRES_CONN_STR, queue_name, reset=True)
+task_queue = TaskQueue(
+    POSTGRES_CONN_STR,
+    queue_name, # name of the queue as a string
+    reset=True, # delete existing tasks for this queue
+    ttl_zero_callback=handle_failure, # will call handle_failure(task_id, task) when the task failed too many times
+)
 
 for i in range(10):
-    task_queue.add(some_task, lease_timeout, ttl=3)
+    task_queue.add(
+        some_task,
+        lease_timeout, # in seconds, after this interval it will be assumed to have failed (and the callback is called)
+        ttl=3, # attempts before abandoning
+        can_start_at=datetime.now(UTC) + timedelta(minutes=5), # start it not before than 5 minutes in the future
+    )
 ```
 
 On the consuming side:
 
 ```py
 from postgrestq import TaskQueue
 
 task_queue = TaskQueue(POSTGRES_CONN_STR, queue_name, reset=True)
 while True:
-    task, task_id = task_queue.get()
+    task, task_id, _queue_name = task_queue.get()
     if task is not None:
         # do something with task and mark it as complete afterwards
         task_queue.complete(task_id)
     if task_queue.is_empty():
         break
     # task_queue.get is non-blocking, so you may want to sleep a
     # bit before the next iteration
     time.sleep(1)
 ```
 
+Notice that `get()` returns the queue name too, in case in future multi-queue is implemented.
+At the moment it's always the same as the queue_name given to the class.
+
 Or you can even use the \_\_iter\_\_() method of the class TaskQueue and loop over the queue:
 
 ```py
 from postgrestq import TaskQueue
 
 task_queue = TaskQueue(POSTGRES_CONN_STR, queue_name, reset=True)
 
-for task, id_ in taskqueue:
+for task, id_, queue_name in taskqueue:
     # do something with task and it's automatically
     # marked as completed by the iterator at the end
     # of the iteration
 
 ```
 
 If the consumer crashes (i.e. the task is not marked as completed after lease_timeout seconds), the task will be put back into the task queue. This rescheduling will happen at most ttl times and then the task will be dropped. A callback can be provided if you want to monitor such cases.
@@ -140,14 +103,56 @@
 # Prune all tasks from queue completed more than 1 hour (in seconds)
 # ago. Tasks in progress, not started and completed recently will
 # stay in the postgres task_queue table
 task_queue.prune_completed_tasks(3600)
 
 ```
 
+
+## How it works
+
+It uses row level locks of postgres to mimic the atomic pop and atomic push of redis-tq when getting a new task from the queue:
+
+```sql
+UPDATE task_queue
+SET processing = true,
+    deadline =
+        current_timestamp + CAST(lease_timeout || ' seconds' AS INTERVAL)
+WHERE id = (
+    SELECT id
+    FROM task_queue
+    WHERE completed_at IS NULL
+        AND processing = false
+        AND queue_name = <your_queue_name>
+        AND ttl > 0
+    ORDER BY created_at
+    FOR UPDATE SKIP LOCKED
+    LIMIT 1
+)
+RETURNING id, task;
+```
+
+Let's say two workers try to get a new task at the same time, assuming that they will probably see the same task to be picked up using the subquery:
+
+```sql
+SELECT id
+FROM task_queue
+WHERE completed_at IS NULL
+    AND processing = false
+    AND queue_name = <your_queue_name>
+    AND ttl > 0
+ORDER BY created_at
+```
+
+The first worker locks the row with the `FOR UPDATE` clause until the update is completed and committed. If we hadn't used the `SKIP LOCKED` clause, the second worker would have seen the same row and waited for the first worker to finish the update. However, since the first worker already updated it, the subquery would no longer be valid, and the second worker would return zero rows because `WHERE id = NULL`.
+
+However, since we are using `FOR UPDATE SKIP LOCKED` the first worker locks the row for update and the second worker, skips that locked row and chooses another row for itself to update. This way we can avoid the race condition.
+
+The other methods `complete()` and `reschedule()` work similarly under the hood.
+
 ## Running the tests
 
 The tests will check a presence of an Postgres DB in the port 15432. To initiate one using docker you can run:
 
 ```bash
 $ make run-postgres
 ```
```

### Comparing `postgres-tq-0.0.6/postgres_tq.egg-info/PKG-INFO` & `postgres_tq-1.0.0/postgres_tq.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,138 +1,101 @@
 Metadata-Version: 2.1
 Name: postgres-tq
-Version: 0.0.6
+Version: 1.0.0
 Summary: Postgres Based Task Queue
 Author-email: FlixTech <open-source@flixbus.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: psycopg[binary]>=3.1.12
 
 [![postgres-tq Actions Status](https://github.com/flix-tech/postgres-tq/workflows/CI/CD%20Pipeline/badge.svg?branch=main)](https://github.com/flix-tech/postgres-tq/actions)
 [![License](https://img.shields.io/github/license/flix-tech/postgres-tq)](https://pypi.org/project/postgres-tq/)
 [![PyPI - Python Version](https://img.shields.io/pypi/v/postgres-tq)](https://pypi.org/project/postgres-tq/)
 
 # Postgres Task Queue
 
-This repo will contain the [Postgres](https://www.postgresql.org/) based task queue logic, similar to [our redis-tq](https://github.com/flix-tech/redis-tq) but based on postgres instead.
+This library makes it possible to define a list of tasks to be persisted in a Postgres database and executed by multiple workers. Tasks are retried automatically after a given timeout and for a given number of time. Tasks are persisted in the database and executed in order of insertion unless a specific start timestamp is provided.
+
+This is similar to [our redis-tq](https://github.com/flix-tech/redis-tq) but based on Postgres thanks to the `FOR UPDATE SKIP LOCKED` feature.
 
 Similar to redis-tq, this package allows for sharing data between multiple processes or hosts.
 
 Tasks support a "lease time". After that time other workers may consider this client to have crashed or stalled and pick up the item instead. The number of retries can also be configured.
 
 By default it keeps all the queues and tasks in a single table `task_queue`. If you want to use a different table for different queues for example it could also be configured when instantiating the queue.
 
-You can either set the `create_table=True` when instantiating the queue or create the table yourself with the following query:
+You can set the `create_table=True` when instantiating the queue to have the table created for you. If the table already exist it will not be touched.
 
-```sql
-CREATE TABLE task_queue (
-    id UUID PRIMARY KEY,
-    queue_name TEXT NOT NULL,
-    task JSONB NOT NULL,
-    ttl INT NOT NULL,
-    created_at TIMESTAMP NOT NULL DEFAULT CURRENT_TIMESTAMP,
-    processing BOOLEAN NOT NULL DEFAULT false,
-    lease_timeout FLOAT,
-    deadline TIMESTAMP,
-    completed_at TIMESTAMP
-)
-```
+When defining a task you can provide a `can_start_at` timestamp parameter, and the task will not be executed until then, which can be useful to schedule tasks. By default the current timestamp is used.
 
 ## Installation
 
 postgres-tq is available on [PyPI][] so you can simply install via:
 
 ```bash
 $ pip install postgres-tq
 ```
 
 [PyPI]: https://pypi.org/project/postgres-tq/
 
-## How it works
-
-It uses row level locks of postgres to mimic the atomic pop and atomic push of redis-tq when getting a new task from the queue:
-
-```sql
-UPDATE task_queue
-SET processing = true,
-    deadline =
-        current_timestamp + CAST(lease_timeout || ' seconds' AS INTERVAL)
-WHERE id = (
-    SELECT id
-    FROM task_queue
-    WHERE completed_at IS NULL
-        AND processing = false
-        AND queue_name = <your_queue_name>
-        AND ttl > 0
-    ORDER BY created_at
-    FOR UPDATE SKIP LOCKED
-    LIMIT 1
-)
-RETURNING id, task;
-```
-
-Let's say two workers try to get a new task at the same time, assuming that they will probably see the same task to be picked up using the subquery:
-
-```sql
-SELECT id
-FROM task_queue
-WHERE completed_at IS NULL
-    AND processing = false
-    AND queue_name = <your_queue_name>
-    AND ttl > 0
-ORDER BY created_at
-```
-
-The first worker locks the row with the `FOR UPDATE` clause until the update is completed and committed. If we hadn't used the `SKIP LOCKED` clause, the second worker would have seen the same row and waited for the first worker to finish the update. However, since the first worker already updated it, the subquery would no longer be valid, and the second worker would return zero rows because `WHERE id = NULL`.
-
-However, since we are using `FOR UPDATE SKIP LOCKED` the first worker locks the row for update and the second worker, skips that locked row and chooses another row for itself to update. This way we can avoid the race condition.
-
-The other methods `complete()` and `reschedule()` work similarly under the hood.
-
 ## How to use
 
 On the producing side, populate the queue with tasks and a respective lease timeout:
 
 ```py
+from datetime import datetime, UTC, timedelta
 from postgrestq import TaskQueue
 
-task_queue = TaskQueue(POSTGRES_CONN_STR, queue_name, reset=True)
+task_queue = TaskQueue(
+    POSTGRES_CONN_STR,
+    queue_name, # name of the queue as a string
+    reset=True, # delete existing tasks for this queue
+    ttl_zero_callback=handle_failure, # will call handle_failure(task_id, task) when the task failed too many times
+)
 
 for i in range(10):
-    task_queue.add(some_task, lease_timeout, ttl=3)
+    task_queue.add(
+        some_task,
+        lease_timeout, # in seconds, after this interval it will be assumed to have failed (and the callback is called)
+        ttl=3, # attempts before abandoning
+        can_start_at=datetime.now(UTC) + timedelta(minutes=5), # start it not before than 5 minutes in the future
+    )
 ```
 
 On the consuming side:
 
 ```py
 from postgrestq import TaskQueue
 
 task_queue = TaskQueue(POSTGRES_CONN_STR, queue_name, reset=True)
 while True:
-    task, task_id = task_queue.get()
+    task, task_id, _queue_name = task_queue.get()
     if task is not None:
         # do something with task and mark it as complete afterwards
         task_queue.complete(task_id)
     if task_queue.is_empty():
         break
     # task_queue.get is non-blocking, so you may want to sleep a
     # bit before the next iteration
     time.sleep(1)
 ```
 
+Notice that `get()` returns the queue name too, in case in future multi-queue is implemented.
+At the moment it's always the same as the queue_name given to the class.
+
 Or you can even use the \_\_iter\_\_() method of the class TaskQueue and loop over the queue:
 
 ```py
 from postgrestq import TaskQueue
 
 task_queue = TaskQueue(POSTGRES_CONN_STR, queue_name, reset=True)
 
-for task, id_ in taskqueue:
+for task, id_, queue_name in taskqueue:
     # do something with task and it's automatically
     # marked as completed by the iterator at the end
     # of the iteration
 
 ```
 
 If the consumer crashes (i.e. the task is not marked as completed after lease_timeout seconds), the task will be put back into the task queue. This rescheduling will happen at most ttl times and then the task will be dropped. A callback can be provided if you want to monitor such cases.
@@ -151,14 +114,56 @@
 # Prune all tasks from queue completed more than 1 hour (in seconds)
 # ago. Tasks in progress, not started and completed recently will
 # stay in the postgres task_queue table
 task_queue.prune_completed_tasks(3600)
 
 ```
 
+
+## How it works
+
+It uses row level locks of postgres to mimic the atomic pop and atomic push of redis-tq when getting a new task from the queue:
+
+```sql
+UPDATE task_queue
+SET processing = true,
+    deadline =
+        current_timestamp + CAST(lease_timeout || ' seconds' AS INTERVAL)
+WHERE id = (
+    SELECT id
+    FROM task_queue
+    WHERE completed_at IS NULL
+        AND processing = false
+        AND queue_name = <your_queue_name>
+        AND ttl > 0
+    ORDER BY created_at
+    FOR UPDATE SKIP LOCKED
+    LIMIT 1
+)
+RETURNING id, task;
+```
+
+Let's say two workers try to get a new task at the same time, assuming that they will probably see the same task to be picked up using the subquery:
+
+```sql
+SELECT id
+FROM task_queue
+WHERE completed_at IS NULL
+    AND processing = false
+    AND queue_name = <your_queue_name>
+    AND ttl > 0
+ORDER BY created_at
+```
+
+The first worker locks the row with the `FOR UPDATE` clause until the update is completed and committed. If we hadn't used the `SKIP LOCKED` clause, the second worker would have seen the same row and waited for the first worker to finish the update. However, since the first worker already updated it, the subquery would no longer be valid, and the second worker would return zero rows because `WHERE id = NULL`.
+
+However, since we are using `FOR UPDATE SKIP LOCKED` the first worker locks the row for update and the second worker, skips that locked row and chooses another row for itself to update. This way we can avoid the race condition.
+
+The other methods `complete()` and `reschedule()` work similarly under the hood.
+
 ## Running the tests
 
 The tests will check a presence of an Postgres DB in the port 15432. To initiate one using docker you can run:
 
 ```bash
 $ make run-postgres
 ```
```

### Comparing `postgres-tq-0.0.6/postgrestq/task_queue.py` & `postgres_tq-1.0.0/postgrestq/task_queue.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,30 @@
 import json
 import logging
+from datetime import datetime
 
 from uuid import uuid4, UUID
-from typing import Optional, Tuple, Iterator, Dict, Any, Callable
+from typing import (
+    Optional,
+    Tuple,
+    Iterator,
+    Dict,
+    Any,
+    Callable,
+    List,
+    Sequence,
+)
 
 from psycopg import sql, connect
 
+# supported only from 3.11 onwards:
+# from datetime import UTC
+# workaround for older versions:
+from datetime import timezone
+UTC = timezone.utc
 
 logger = logging.getLogger(__name__)
 
 
 class TaskQueue:
     def __init__(
         self,
@@ -74,70 +89,86 @@
         """
         # TODO: check if the table already exist
         # whether it has the same schema
         with self.conn.cursor() as cur:
             cur.execute(
                 sql.SQL(
                     """CREATE TABLE IF NOT EXISTS {} (
-                            id UUID PRIMARY KEY,
-                            queue_name TEXT NOT NULL,
-                            task JSONB NOT NULL,
-                            ttl INT NOT NULL,
-                            created_at TIMESTAMP NOT NULL
-                                DEFAULT CURRENT_TIMESTAMP,
-                            processing BOOLEAN NOT NULL
-                                DEFAULT false,
+                            id            UUID PRIMARY KEY,
+                            queue_name    TEXT NOT NULL,
+                            task          JSONB NOT NULL,
+                            ttl           SMALLINT NOT NULL,
+                            can_start_at  TIMESTAMPTZ NOT NULL
+                                          DEFAULT CURRENT_TIMESTAMP,
                             lease_timeout FLOAT,
-                            deadline TIMESTAMP,
-                            completed_at TIMESTAMP
+                            started_at    TIMESTAMPTZ,
+                            completed_at  TIMESTAMPTZ
                         )"""
                 ).format(sql.Identifier(self._table_name))
             )
+            cur.execute(
+                sql.SQL(
+                    """CREATE INDEX IF NOT EXISTS
+                        task_queue_queue_name_can_start_at_idx
+                        ON {} (queue_name, can_start_at)
+                    """
+                ).format(sql.Identifier(self._table_name))
+            )
+            self.conn.commit()
 
     def __len__(self) -> int:
         """
         Returns the length of processing or to be processed tasks
         """
         with self.conn.cursor() as cursor:
             cursor.execute(
                 sql.SQL(
                     """
-                SELECT count(1) as count
+                SELECT count(*) as count
                 FROM {}
                 WHERE queue_name = %s
                     AND completed_at IS NULL
             """
                 ).format(sql.Identifier(self._table_name)),
                 (self._queue_name,),
             )
             row = cursor.fetchone()
             count: int = row[0] if row else 0
             self.conn.commit()
             return count
 
     def add(
-        self, task: Dict[str, Any], lease_timeout: float, ttl: int = 3
+        self,
+        task: Dict[str, Any],
+        lease_timeout: float,
+        ttl: int = 3,
+        can_start_at: Optional[datetime] = None
     ) -> str:
         """Add a task to the task queue.
 
         Parameters
         ----------
         task : something that can be JSON-serialized
         lease_timeout : float
             lease timeout in seconds, i.e. how much time we give the
             task to process until we can assume it didn't succeed
         ttl : int
             Number of (re-)tries, including the initial one, in case the
             job dies.
-
+        can_start_at : datetime
+            The earliest time the task can be started.
+            If None, set current time. A task will not be started before this
+            time.
         Returns
         -------
         task_id :
             The random UUID that was generated for this task
         """
+        if can_start_at is None:
+            can_start_at = datetime.now(UTC)
         # make sure the timeout is an actual number, otherwise we'll run
         # into problems later when we calculate the actual deadline
         lease_timeout = float(lease_timeout)
 
         id_ = str(uuid4())
 
         serialized_task = self._serialize(task)
@@ -148,106 +179,233 @@
                 sql.SQL(
                     """
                 INSERT INTO {} (
                     id,
                     queue_name,
                     task,
                     ttl,
-                    lease_timeout
+                    lease_timeout,
+                    can_start_at
                 )
-                VALUES (%s, %s, %s, %s, %s)
+                VALUES (%s, %s, %s, %s, %s, %s)
             """
                 ).format(sql.Identifier(self._table_name)),
-                (id_, self._queue_name, serialized_task, ttl, lease_timeout),
+                (
+                    id_, self._queue_name, serialized_task,
+                    ttl, lease_timeout, can_start_at
+                ),
             )
             self.conn.commit()
         return id_
 
-    def get(self) -> Tuple[Optional[Dict[str, Any]], Optional[UUID]]:
+    def add_many(
+        self,
+        tasks: List[Dict[str, Any]],
+        lease_timeout: float,
+        ttl: int = 3,
+        can_start_at: Optional[datetime] = None
+    ) -> List[str]:
+        """Like add(), but optimized for a batch of tasks.
+
+        When inserting many tasks, it is faster than multiple calls to
+        add() because it uses a single transaction.
+
+        After the creation the tasks will be independent from each other.
+
+        Parameters
+        ----------
+        tasks : list of something that can be JSON-serialized
+        lease_timeout : float
+            lease timeout in seconds, i.e. how much time we give the
+            tasks to process until we can assume it didn't succeed
+        ttl : int
+            Number of (re-)tries, including the initial one, in case the
+            job dies.
+        can_start_at : datetime
+            The earliest time the task can be started.
+            If None, set current time. A task will not be started before this
+            time.
+        Returns
+        -------
+        task_ids :
+            List of random UUIDs that were generated for this task.
+            The order is the same of the given tasks
+        """
+        if can_start_at is None:
+            can_start_at = datetime.now(UTC)
+        # make sure the timeout is an actual number, otherwise we'll run
+        # into problems later when we calculate the actual deadline
+        lease_timeout = float(lease_timeout)
+        ret_ids = []
+        with self.conn.cursor() as cursor:
+            for task in tasks:
+                id_ = str(uuid4())
+
+                serialized_task = self._serialize(task)
+
+                cursor.execute(
+                    sql.SQL(
+                        """
+                    INSERT INTO {} (
+                        id,
+                        queue_name,
+                        task,
+                        ttl,
+                        lease_timeout,
+                        can_start_at
+                    )
+                    VALUES (%s, %s, %s, %s, %s, %s)
+                """
+                    ).format(sql.Identifier(self._table_name)),
+                    (
+                        id_, self._queue_name, serialized_task,
+                        ttl, lease_timeout, can_start_at
+                    ),
+                )
+                ret_ids.append(id_)
+            self.conn.commit()
+        return ret_ids
+
+    def get(self) -> Tuple[
+            Optional[Dict[str, Any]],
+            Optional[UUID],
+            Optional[str],
+            ]:
         """Get a task from the task queue (non-blocking).
 
         This statement marks the next available task in the queue as
         "processing" and returns its ID and task details. The query
         uses a FOR UPDATE SKIP LOCKED clause to lock the selected
         task so that other workers can't select the same task simultaneously.
 
         After executing the query, the method fetches the result using
         cur.fetchone(). If no task is found, the method returns None, None.
         Otherwise, it returns the task and its ID.
 
         Note that this method is non-blocking, which means it returns
-        immediately even if there is no task available in the queue..
-        In order to mark that task as done, you have
-        to use:
+        immediately even if there is no task available in the queue.
 
-            >>> task, task_id = taskqueue.get()
+        In order to mark that task as done, you have to do:
+
+            >>> task, task_id, queue_name = taskqueue.get()
             >>> # do something
             >>> taskqueue.complete(task_id)
 
         After some time (i.e. `lease_timeout`) tasks expire and are
         marked as not processing and the TTL is decreased by
         one. If TTL is still > 0 the task will be retried.
 
         Note, this method is non-blocking, i.e. it returns immediately
         even if there is nothing to return. See below for the return
         value for this case.
 
         Returns
         -------
-        (task, task_id) :
-            The next item from the task list or (None, None) if it's
+        (task, task_id, queue_name) :
+            The next item from the task list or (None, None, None) if it's
             empty
 
         """
         conn = self.conn
 
         with conn.cursor() as cur:
             cur.execute(
                 sql.SQL(
                     """
                 UPDATE {}
-                SET processing = true,
-                    deadline =
-                        current_timestamp +
-                        CAST(lease_timeout || ' seconds' AS INTERVAL)
+                SET started_at = current_timestamp
                 WHERE id = (
                     SELECT id
                     FROM {}
                     WHERE completed_at IS NULL
-                        AND processing = false
+                        AND started_at IS NULL
                         AND queue_name = %s
                         AND ttl > 0
-                    ORDER BY created_at
+                        AND can_start_at <= current_timestamp
+                    ORDER BY can_start_at
                     FOR UPDATE SKIP LOCKED
                     LIMIT 1
                 )
                 RETURNING id, task;"""
                 ).format(
                     sql.Identifier(self._table_name),
                     sql.Identifier(self._table_name),
                 ),
                 (self._queue_name,),
             )
 
             row = cur.fetchone()
+            conn.commit()
             if row is None:
-                return None, None
+                return None, None, None
             task_id, task = row
             logger.info(f"Got task with id {task_id}")
+            return task, task_id, self._queue_name
+
+    def get_many(self, amount: int) -> Sequence[
+        Tuple[Optional[Dict[str, Any]], Optional[UUID], Optional[str]],
+            ]:
+        """Same as get() but retrieves multiple tasks.
+
+        If there are less than `amount` tasks in the queue, it will return
+        whatever is available.
+
+        If no task is available it will return an empty list.
+
+        This is faster than multiple calls to get(), as it uses a single query.
+
+        Returns
+        -------
+        list of (task, task_id, queue_name) :
+            The tasks and their IDs, and the queue_name
+
+        """
+        conn = self.conn
+
+        with conn.cursor() as cur:
+            cur.execute(
+                sql.SQL(
+                    """
+                UPDATE {}
+                SET started_at = current_timestamp
+                WHERE id IN (
+                    SELECT id
+                    FROM {}
+                    WHERE completed_at IS NULL
+                        AND started_at IS NULL
+                        AND queue_name = %s
+                        AND ttl > 0
+                        AND can_start_at <= current_timestamp
+                    ORDER BY can_start_at
+                    FOR UPDATE SKIP LOCKED
+                    LIMIT %s
+                )
+                RETURNING task, id;"""
+                ).format(
+                    sql.Identifier(self._table_name),
+                    sql.Identifier(self._table_name),
+                ),
+                (self._queue_name, amount),
+            )
+
+            ret = []
+            for task, task_id in cur.fetchall():
+                logger.info(f"Got task with id {task_id}")
+                ret.append((task, task_id, self._queue_name,))
             conn.commit()
-            return task, task_id
+            return ret
 
     def complete(self, task_id: Optional[UUID]) -> None:
         """Mark a task as completed.
 
         Marks a task as completed by setting completed_at column by
         the current timestamp.
 
         If the job is in the queue, which happens if it took too long
-        and it expired, is removed from that too.
+        and it expired, it is removed from there as well.
 
 
         Parameters
         ----------
         task_id : UUID | None
             the task ID
 
@@ -255,16 +413,15 @@
         logger.info(f"Marking task {task_id} as completed")
         conn = self.conn
         with conn.cursor() as cur:
             cur.execute(
                 sql.SQL(
                     """
                 UPDATE {}
-                SET completed_at = current_timestamp,
-                    processing = false
+                SET completed_at = current_timestamp
                 WHERE id = %s"""
                 ).format(sql.Identifier(self._table_name)),
                 (task_id,),
             )
             conn.commit()
 
     def is_empty(self) -> bool:
@@ -282,38 +439,43 @@
         self.check_expired_leases()
         return len(self) == 0
 
     def check_expired_leases(self) -> None:
         """Check for expired leases and put the task back if needed.
 
         This method goes through all tasks that are currently processed
-        and checks if their deadline expired. If not we assume the
-        worker died. We decrease the TTL and if TTL is still > 0 we
+        and checks if their deadline expired. If so, we assume the
+        worker failed. We decrease the TTL and if TTL is still > 0 we
         reschedule the task into the task queue or, if the TTL is
         exhausted, we mark the task as completed by setting
         `completed_at` column with current timestamp and call the
         expired task callback if it's set.
 
+        This means a task that takes longer than the lease_timeout can be
+        executed more than once.
+
         Note: lease check is only performed against the tasks
-        that are processing.
+        that are processing (started_at is not null).
 
         """
-        # goes through all the tasks that are marked as processing
+        # goes through all the tasks that are marked as started
         # and check the ones with expired timeout
         with self.conn.cursor() as cur:
             cur.execute(
                 sql.SQL(
                     """
                 SELECT id
                 FROM {}
                 WHERE completed_at IS NULL
-                    AND processing = true
+                    AND started_at IS NOT NULL
                     AND queue_name = %s
-                    AND deadline < NOW()
-                ORDER BY created_at;
+                    AND (
+                        started_at + (lease_timeout || ' seconds')::INTERVAL
+                        ) < current_timestamp
+                ORDER BY can_start_at;
             """
                 ).format(sql.Identifier(self._table_name)),
                 (self._queue_name,),
             )
             expired_tasks = cur.fetchall()
             self.conn.commit()
             logger.debug(f"Expired tasks {expired_tasks}")
@@ -347,39 +509,38 @@
                     self.ttl_zero_callback(task_id, task)
             self.conn.commit()
 
     def get_updated_expired_task(
         self, task_id: UUID
     ) -> Tuple[Optional[str], Optional[int]]:
         """
-        Given the id of an expired task, it tries to reschedule the
-        task by marking it as not processing, resetting the deadline
-        and decreaasing TTL by one. It returns None if the task is
-        already updated or (being updated) by another worker.
+        Given the id of an expired task, it tries to reschedule it by
+        marking it as not processing, resetting the deadline
+        and decreasing TTL by one. It returns None if the task is
+        already updated (or being updated) by another worker.
 
         Returns
         -------
         (task, ttl) :
             The updated task and ttl values for the expired task with
             task_id after it's rescheduled
 
         """
         with self.conn.cursor() as cur:
             cur.execute(
                 sql.SQL(
                     """
                 UPDATE {}
                 SET ttl = ttl - 1,
-                    processing = false,
-                    deadline = NULL
+                    started_at = NULL
                 WHERE id = (
                     SELECT id
                     FROM {}
                     WHERE completed_at IS NULL
-                        AND processing = true
+                        AND started_at IS NOT NULL
                         AND queue_name = %s
                         AND id = %s
                     FOR UPDATE SKIP LOCKED
                     LIMIT 1
                 )
                 RETURNING task, ttl;
             """
@@ -432,20 +593,19 @@
         logger.info(f"Rescheduling task {task_id}..")
         conn = self.conn
         with conn.cursor() as cur:
             cur.execute(
                 sql.SQL(
                     """
                 UPDATE {}
-                SET processing = false,
-                    deadline = NULL
+                SET started_at = NULL
                 WHERE id = (
                     SELECT id
                     FROM {}
-                    WHERE processing = true
+                    WHERE started_at IS NOT NULL
                         AND id = %s
                     FOR UPDATE SKIP LOCKED
                 )
                 RETURNING id;"""
                 ).format(
                     sql.Identifier(self._table_name),
                     sql.Identifier(self._table_name),
@@ -487,50 +647,55 @@
         with self.conn.cursor() as cursor:
             cursor.execute(
                 sql.SQL(
                     """
                     DELETE FROM {}
                     WHERE queue_name = %s
                         AND completed_at IS NOT NULL
-                        AND processing = false
                         AND completed_at < current_timestamp - CAST(
                             %s || ' seconds' AS INTERVAL);
                     """
                 ).format(sql.Identifier(self._table_name)),
                 (self._queue_name, before),
             )
 
             self.conn.commit()
 
     def __iter__(
         self,
-    ) -> Iterator[Tuple[Optional[Dict[str, Any]], Optional[UUID]]]:
+    ) -> Iterator[
+                Tuple[
+                    Optional[Dict[str, Any]],
+                    Optional[UUID],
+                    Optional[str]
+                ]
+            ]:
         """Iterate over tasks and mark them as complete.
 
         This allows to easily iterate over the tasks to process them:
 
-            >>> for task in task_queue:
+            >>> for task, task_id in task_queue:
                     execute_task(task)
 
         it takes care of marking the tasks as done once they are processed
         and checking the emptiness of the queue before leaving.
 
         Notice that this iterator can wait for a long time waiting for work
         units to appear, depending on the value set as lease_timeout.
 
         Yields
         -------
-        (any, str) :
-            A tuple containing the task content and its id
+        (any, UUID, str) :
+            A tuple containing the task content, its id and the queue name
 
         """
         while True:
-            task, id_ = self.get()
+            task, id_, queue_name = self.get()
             if id_ is not None:
-                yield task, id_
+                yield task, id_, queue_name
                 self.complete(id_)
             if self.is_empty():
                 logger.debug(
                     f"{self._queue_name} is empty. "
                     "Nothing to process anymore..."
                 )
                 break
```

### Comparing `postgres-tq-0.0.6/pyproject.toml` & `postgres_tq-1.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -14,22 +14,25 @@
 log_cli = true
 log_cli_level = "INFO"
 log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
 log_cli_date_format = "%Y-%m-%d %H:%M:%S"
 
 [project]
 name = "postgres-tq"
-version = "0.0.6"
+version = "1.0.0"
 description = "Postgres Based Task Queue"
 authors = [
     {name = "FlixTech", email = "open-source@flixbus.com"},
 ]
 dependencies = [
     "psycopg[binary]>=3.1.12",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 license = {text = "MIT"}
 
 [build-system]
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
+
+[tool.setuptools.package-data]
+"postgrestq" = ["py.typed"]
```

### Comparing `postgres-tq-0.0.6/tests/test_task_queue.py` & `postgres_tq-1.0.0/tests/test_task_queue.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+from datetime import datetime, timedelta
+# supported only from 3.11 onwards:
+# from datetime import UTC
+# workaround for older versions:
+from datetime import timezone
+UTC = timezone.utc
+
 import logging
 import time
 import os
 from unittest import mock
 from uuid import UUID
 
 import pytest
@@ -29,59 +36,67 @@
 
     # delete the stuff
     tq._reset()
 
 
 def test_add(task_queue: TaskQueue):
     # add two tasks and get them back in correct order
-    TASKS = [{"foo": 1}, {"bar": 2}]
+    TASKS = [{"foo": 1}, {"bar": 2}, {"d": 56}]
     task_ids = set()
-    for task in TASKS:
-        tid = task_queue.add(task, LEASE_TIMEOUT)
+    for idx, task in enumerate(TASKS):
+        tid = task_queue.add(
+            task,
+            LEASE_TIMEOUT,
+            can_start_at=datetime.now(UTC) - timedelta(seconds=100) + timedelta(seconds=idx)
+        )
         task_ids.add(tid)
-    assert len(task_ids) == 2
-    task, _ = task_queue.get()
+    assert len(task_ids) == 3
+    task, _, qname = task_queue.get()
     assert task == TASKS[0]
-    task, _ = task_queue.get()
+    assert qname == "test_queue"
+    task, _, qname = task_queue.get()
     assert task == TASKS[1]
+    assert qname == "test_queue"
 
 
 def test_get(task_queue: TaskQueue):
     TASK = {"foo": 1}
     task_queue.add(TASK, LEASE_TIMEOUT)
-    task, _ = task_queue.get()
+    task, _, _ = task_queue.get()
     assert task == TASK
     # calling on empty queue returns None
-    assert task_queue.get() == (None, None)
+    assert task_queue.get() == (None, None, None)
 
 
 def test_is_empty(task_queue: TaskQueue):
     assert task_queue.is_empty()
 
     task_queue.add({"foo": 1}, LEASE_TIMEOUT)
     assert not task_queue.is_empty()
 
-    task, id_ = task_queue.get()
+    task, id_, _qname = task_queue.get()
     assert not task_queue.is_empty()
-
+    assert _qname == "test_queue"
     task_queue.complete(id_)
     assert task_queue.is_empty()
 
 
 def test_complete(task_queue: TaskQueue):
     # boring case
     task_queue.add({"foo": 1}, LEASE_TIMEOUT, ttl=1)
-    _, id_ = task_queue.get()
+    _, id_, qname = task_queue.get()
     assert not task_queue.is_empty()
+    assert qname == "test_queue"
     task_queue.complete(id_)
     assert task_queue.is_empty()
 
     # interesting case: we complete the task after it expired already
     task_queue.add({"foo": 1}, LEASE_TIMEOUT, ttl=1)
-    _, id_ = task_queue.get()
+    _, id_, qname = task_queue.get()
+    assert qname == "test_queue"
     time.sleep(LEASE_TIMEOUT + 0.1)
     assert task_queue.is_empty()
     task_queue.complete(id_)
     assert task_queue.is_empty()
 
 
 def test_expired(task_queue: TaskQueue):
@@ -147,21 +162,22 @@
     time.sleep(LEASE_TIMEOUT + 0.1)
     assert task_queue.is_empty()
     assert mock_cb.called
 
 
 def test_reschedule(task_queue: TaskQueue):
     task_queue.add({"foo": 1}, LEASE_TIMEOUT)
-    _, id_ = task_queue.get()
+    _, id_, qname = task_queue.get()
     # task queue should be empty as 'foo' is in the processing queue
-    assert task_queue.get() == (None, None)
-
+    assert task_queue.get() == (None, None, None)
+    assert qname == "test_queue"
     task_queue.reschedule(id_)
-    task, _ = task_queue.get()
+    task, _, qname = task_queue.get()
     assert task == {"foo": 1}
+    assert qname == "test_queue"
 
 
 def test_reschedule_error(task_queue: TaskQueue):
     with pytest.raises(ValueError):
         task_queue.reschedule("bar")
 
 
@@ -172,58 +188,60 @@
         {"BAZ": 3, "c": "another thing"},
     ]
     for t in TASKS:
         task_queue.add(t, LEASE_TIMEOUT)
 
     counter = 0
     while True:
-        task, task_id = task_queue.get()
+        task, task_id, qname = task_queue.get()
         if task is not None:
             task_queue.complete(task_id)
             counter += 1
         if task_queue.is_empty():
             break
 
     assert counter == len(TASKS)
+    assert qname == "test_queue"
 
 
 def test_complete_rescheduled_task(task_queue: TaskQueue):
     TASK_CONTENT = {"sloth": 1}
     task_queue.add(TASK_CONTENT, LEASE_TIMEOUT, ttl=3)
 
     # start a task and let it expire...
-    _, task_id = task_queue.get()
+    _, task_id, qname = task_queue.get()
     time.sleep(LEASE_TIMEOUT + 0.1)
 
     # check and put it back into task queue
     assert not task_queue.is_empty()
-
+    assert qname == "test_queue"
     # now the task is completed, although it took a long time...
     task_queue.complete(task_id)
 
     # it is NOT in the task_queue, because it was finished
     assert task_queue.is_empty()
 
 
 #
 def test_tolerate_double_completion(task_queue: TaskQueue):
     TASK_CONTENT = {"sloth": 1}
     task_queue.add(TASK_CONTENT, LEASE_TIMEOUT, ttl=3)
 
     # start a task and let it expire...
-    task, task_id = task_queue.get()
+    task, task_id, qname = task_queue.get()
+    assert qname == "test_queue"
     time.sleep(LEASE_TIMEOUT + 0.1)
 
     # check and put it back into task queue
     assert not task_queue.is_empty()
 
     # get it again
-    _, task_redo_id = task_queue.get()
+    _, task_redo_id, qname = task_queue.get()
     assert task_redo_id == task_id
-
+    assert qname == "test_queue"
     # now the task is completed, although it took a long time...
     task_queue.complete(task_id)
 
     # but the other worker doesn't know and keep processing, until...
     task_queue.complete(task_redo_id)
 
     # no crashes, the double completion is fine and queues are empty
@@ -252,15 +270,15 @@
 
 
 def test_iterator(task_queue: TaskQueue):
     task_queue.add({"bla": "bla"}, LEASE_TIMEOUT, ttl=3)
     task_queue.add({"blip": "blop"}, LEASE_TIMEOUT, ttl=3)
 
     found_tasks = []
-    for task, id in task_queue:
+    for task, id, qname in task_queue:
         found_tasks.append(task)
     assert found_tasks == [{"bla": "bla"}, {"blip": "blop"}]
 
 
 def test_expired_leases_race(
     task_queue: TaskQueue, monkeypatch: MonkeyPatch, caplog: LogCaptureFixture
 ):
```

