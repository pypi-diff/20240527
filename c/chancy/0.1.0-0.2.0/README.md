# Comparing `tmp/chancy-0.1.0.tar.gz` & `tmp/chancy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chancy-0.1.0.tar", max compression
+gzip compressed data, was "chancy-0.2.0.tar", max compression
```

## Comparing `chancy-0.1.0.tar` & `chancy-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,16 @@
--rw-r--r--   0        0        0     1124 2024-05-26 07:02:16.300624 chancy-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-26 07:02:16.300624 chancy-0.1.0/chancy/__init__.py
--rw-r--r--   0        0        0    12759 2024-05-26 07:02:16.300624 chancy-0.1.0/chancy/app.py
--rw-r--r--   0        0        0      526 2024-05-26 07:02:16.300624 chancy-0.1.0/chancy/logger.py
--rw-r--r--   0        0        0     6763 2024-05-26 07:02:16.300624 chancy-0.1.0/chancy/migrate.py
--rw-r--r--   0        0        0     2299 2024-05-26 07:02:16.300624 chancy-0.1.0/chancy/migrations/v1.py
--rw-r--r--   0        0        0      212 2024-05-26 07:02:16.300624 chancy-0.1.0/chancy/plugin.py
--rw-r--r--   0        0        0     1108 2024-05-26 07:02:16.300624 chancy-0.1.0/chancy/utils.py
--rw-r--r--   0        0        0    21373 2024-05-26 07:02:16.300624 chancy-0.1.0/chancy/worker.py
--rw-r--r--   0        0        0      481 2024-05-26 07:02:16.304624 chancy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1557 1970-01-01 00:00:00.000000 chancy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1124 2024-05-27 09:04:56.407850 chancy-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 09:04:56.407850 chancy-0.2.0/chancy/__init__.py
+-rw-r--r--   0        0        0    13504 2024-05-27 09:04:56.407850 chancy-0.2.0/chancy/app.py
+-rw-r--r--   0        0        0     1005 2024-05-27 09:04:56.407850 chancy-0.2.0/chancy/hub.py
+-rw-r--r--   0        0        0      526 2024-05-27 09:04:56.407850 chancy-0.2.0/chancy/logger.py
+-rw-r--r--   0        0        0     6763 2024-05-27 09:04:56.407850 chancy-0.2.0/chancy/migrate.py
+-rw-r--r--   0        0        0     3584 2024-05-27 09:04:56.407850 chancy-0.2.0/chancy/migrations/v1.py
+-rw-r--r--   0        0        0      553 2024-05-27 09:04:56.407850 chancy-0.2.0/chancy/plugin.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:04:56.407850 chancy-0.2.0/chancy/plugins/__init__.py
+-rw-r--r--   0        0        0     2857 2024-05-27 09:04:56.407850 chancy-0.2.0/chancy/plugins/pruner.py
+-rw-r--r--   0        0        0     2993 2024-05-27 09:04:56.407850 chancy-0.2.0/chancy/plugins/recovery.py
+-rw-r--r--   0        0        0     1777 2024-05-27 09:04:56.407850 chancy-0.2.0/chancy/plugins/sentry.py
+-rw-r--r--   0        0        0     1108 2024-05-27 09:04:56.407850 chancy-0.2.0/chancy/utils.py
+-rw-r--r--   0        0        0    25929 2024-05-27 09:04:56.407850 chancy-0.2.0/chancy/worker.py
+-rw-r--r--   0        0        0      503 2024-05-27 09:04:56.411850 chancy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1557 1970-01-01 00:00:00.000000 chancy-0.2.0/PKG-INFO
```

### Comparing `chancy-0.1.0/README.md` & `chancy-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `chancy-0.1.0/chancy/app.py` & `chancy-0.2.0/chancy/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 from typing import Optional, Callable
 
 from psycopg import sql
 from psycopg import AsyncCursor, Cursor
 from psycopg.types.json import Json
 from psycopg_pool import AsyncConnectionPool
 
+from chancy.hub import Hub
 from chancy.migrate import Migrator
 from chancy.utils import importable_name
+from chancy.plugin import Plugin
 
 
 @dataclasses.dataclass(frozen=True)
 class JobContext:
     """
     A context object that can be requested by a running job to get information
     about the job itself.
@@ -241,15 +243,15 @@
     """
 
     #: A postgres DSN to connect to the database.
     dsn: str
     #: A list of queues that this app should be aware of for processing jobs.
     queues: list[Queue] = dataclasses.field(default_factory=list)
     #: A list of plugins to enable for this application.
-    plugins: list[str] = dataclasses.field(default_factory=list)
+    plugins: list[Plugin] = dataclasses.field(default_factory=list)
     #: The prefix to use for all Chancy tables in the database.
     prefix: str = "chancy_"
     #: The minimum number of seconds to wait between polling for new jobs.
     job_poller_interval: int = 5
     #: The minimum number of seconds to wait between attempts to acquire
     #: leadership of the cluster.
     leadership_poller_interval: int = 30
@@ -259,14 +261,17 @@
     disable_events: bool = False
 
     #: The minimum number of connections to keep in the pool.
     min_pool_size: int = 1
     #: The maximum number of connections to keep in the pool.
     max_pool_size: int = 3
 
+    #: Event hub for registering and emitting events.
+    hub: Hub = dataclasses.field(default_factory=Hub)
+
     def __post_init__(self):
         # Ensure all defined queues have distinct names.
         queue_names = [queue.name for queue in self.queues]
         if len(queue_names) != len(set(queue_names)):
             raise ValueError("Duplicate queue names are not allowed.")
 
         # Ensure all queue names are valid a-zA-Z and underscore.
@@ -319,15 +324,37 @@
         await self.pool.open()
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.pool.close()
         return False
 
-    async def submit(self, job: Job, queue: Queue):
+    async def open(self):
+        """
+        Open the connection pool.
+
+        When possible, it's preferred to instead use the async context manager
+        interface to ensure the pool is properly opened and closed.
+
+        .. code-block:: python
+
+            async with Chancy(
+                dsn="postgresql://username:password@localhost:8190/postgres",
+            ) as app:
+                ...
+        """
+        await self.pool.open()
+
+    async def close(self):
+        """
+        Close the connection pool.
+        """
+        await self.pool.close()
+
+    async def submit(self, job: Job, queue: Queue | str):
         """
         Submit a job to the specified queue.
 
         This method will insert the job into the database and notify any
         listening workers that a new job is available. It will be submitted
         immediately using a new connection and transaction. To submit multiple
         jobs in a single transaction, use `submit_to_cursor`.
```

### Comparing `chancy-0.1.0/chancy/logger.py` & `chancy-0.2.0/chancy/logger.py`

 * *Files identical despite different names*

### Comparing `chancy-0.1.0/chancy/migrate.py` & `chancy-0.2.0/chancy/migrate.py`

 * *Files identical despite different names*

### Comparing `chancy-0.1.0/chancy/migrations/v1.py` & `chancy-0.2.0/chancy/migrations/v1.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,14 +17,15 @@
                         id BIGSERIAL PRIMARY KEY,
                         queue TEXT NOT NULL,
                         payload JSON NOT NULL,
                         state VARCHAR (25) NOT NULL DEFAULT 'pending',
                         priority INTEGER DEFAULT 0,
                         attempts INTEGER DEFAULT 0,
                         max_attempts INTEGER DEFAULT 1,
+                        taken_by TEXT,
                         created_at TIMESTAMPTZ NOT NULL DEFAULT NOW(),
                         started_at TIMESTAMPTZ,
                         completed_at TIMESTAMPTZ,
                         scheduled_at TIMESTAMPTZ
                     )
                     """
                 ).format(jobs=sql.Identifier(f"{migrator.prefix}jobs"))
@@ -35,19 +36,35 @@
                     """
                     CREATE UNLOGGED TABLE {leader} (
                         id BIGSERIAL PRIMARY KEY,
                         worker_id TEXT NOT NULL,
                         last_seen TIMESTAMPTZ NOT NULL DEFAULT NOW()
                     );
                     ALTER TABLE {leader}
-                        ADD CONSTRAINT worker_id_unique UNIQUE (worker_id);
+                        ADD CONSTRAINT leader_worker_id_unique UNIQUE
+                            (worker_id);
                     """
                 ).format(leader=sql.Identifier(f"{migrator.prefix}leader"))
             )
 
+            await conn.execute(
+                sql.SQL(
+                    """
+                    CREATE UNLOGGED TABLE {workers} (
+                        id BIGSERIAL PRIMARY KEY,
+                        worker_id TEXT NOT NULL,
+                        last_seen TIMESTAMPTZ NOT NULL DEFAULT NOW()
+                    );
+                    ALTER TABLE {workers}
+                        ADD CONSTRAINT workers_worker_id_unique UNIQUE
+                            (worker_id);
+                    """
+                ).format(workers=sql.Identifier(f"{migrator.prefix}workers"))
+            )
+
     async def down(self, migrator: Migrator, conn: AsyncConnection):
         """
         Drop the $prefix_jobs, $prefix_leaders tables.
         """
         async with conn.transaction():
             await conn.execute(
                 sql.SQL("DROP TABLE {jobs}").format(
@@ -55,7 +72,22 @@
                 )
             )
             await conn.execute(
                 sql.SQL("DROP TABLE {leader}").format(
                     leaders=sql.Identifier(f"{migrator.prefix}leader")
                 )
             )
+            await conn.execute(
+                sql.SQL("DROP TABLE {workers}").format(
+                    workers=sql.Identifier(f"{migrator.prefix}workers")
+                )
+            )
+            await conn.execute(
+                sql.SQL("DROP CONSTRAINT leader_worker_id_unique").format(
+                    workers=sql.Identifier(f"{migrator.prefix}leader")
+                )
+            )
+            await conn.execute(
+                sql.SQL("DROP CONSTRAINT workers_worker_id_unique").format(
+                    workers=sql.Identifier(f"{migrator.prefix}workers")
+                )
+            )
```

### Comparing `chancy-0.1.0/chancy/utils.py` & `chancy-0.2.0/chancy/utils.py`

 * *Files identical despite different names*

### Comparing `chancy-0.1.0/chancy/worker.py` & `chancy-0.2.0/chancy/worker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 The :class:`chancy.worker.Worker` class is the main entry point for running
 workers in a Chancy application.
 """
 
-import inspect
+import enum
 import os
 import json
 import uuid
 import signal
 import asyncio
+import inspect
 import resource
 import threading
 import dataclasses
 from asyncio import TaskGroup
 from collections import defaultdict
 from concurrent.futures import ProcessPoolExecutor, Future
 from datetime import datetime, timezone
@@ -23,14 +24,23 @@
 from psycopg import AsyncConnection
 from psycopg.rows import dict_row
 from psycopg.errors import LockNotAvailable
 
 from chancy.app import Chancy, Queue, Job, Limit, JobContext
 from chancy.logger import logger, PrefixAdapter
 from chancy.migrate import Migrator
+from chancy.hub import Hub
+from chancy.utils import timed_block
+
+
+class Leadership(enum.IntEnum):
+    REFRESHED = 1
+    ACQUIRED = 2
+    UNAVAILABLE = 3
+    LOST = 4
 
 
 class _TimeoutThread(threading.Thread):
     """
     A thread that will raise a TimeoutError after a specified number of
     seconds.
     """
@@ -210,23 +220,28 @@
                 await Worker(app).start()
 
     :param app: The Chancy application to run the worker for.
     :param worker_id: An optional, globally-unique worker ID to use for this
                       worker.
     """
 
-    def __init__(self, app: Chancy, worker_id: str = None):
+    class Event(Hub.Event):
+        ON_LEADERSHIP_LOOP = "worker.on_leadership_loop"
+        ON_EXCEPTION = "worker.on_exception"
+
+    def __init__(self, app: Chancy, *, worker_id: str = None):
         self.app = app
         self.worker_id = worker_id or str(uuid.uuid4())
         self.pools: dict[Queue, Nanny] = {
             queue: Nanny(app, queue) for queue in app.queues
         }
         self.pending_changes: dict[Queue, asyncio.Queue] = defaultdict(
             asyncio.Queue
         )
+        self.is_leader: bool = False
 
     async def start(self):
         """
         Start the worker.
 
         The worker will immediately begin pulling jobs from the queue, and
         make itself available as a possible leader in the cluster.
@@ -259,23 +274,30 @@
             if not self.app.disable_events:
                 tg.create_task(self._listen_for_events())
 
     async def _poll_event_loop(self):
         poll_logger = PrefixAdapter(logger, {"prefix": "POLL"})
         poll_logger.info("Started periodic polling for tasks.")
 
+        for plugin in self.app.plugins:
+            if plugin.get_type() == plugin.Type.WORKER:
+                logger.debug(f"Starting worker plugin {plugin!r}.")
+                await plugin.on_startup(self.app.hub)
+
         while True:
             async with self.app.pool.connection() as conn:
                 for queue in self.app.queues:
                     if queue.state == Queue.State.PAUSED:
                         poll_logger.debug(
                             f"Queue {queue.name} is paused, skipping."
                         )
                         continue
 
+                    await self.announce_worker(conn)
+
                     jobs = await self._fetch_available_jobs(conn, queue)
                     poll_logger.debug(
                         f"Found {len(jobs)} job(s) in queue {queue.name}."
                     )
                     for job in jobs:
                         future = self.pools[queue].submit(job)
                         future.add_done_callback(
@@ -318,26 +340,26 @@
                         )
 
                     await cur.executemany(
                         sql.SQL(
                             """
                             UPDATE {jobs}
                             SET
-                                state = %s,
-                                completed_at = %s
+                                state = %(state)s,
+                                completed_at = %(completed_at)s
                             WHERE
-                                id = %s
+                                id = %(job_id)s
                             """
                         ).format(jobs=jobs_table),
                         [
-                            (
-                                change.state,
-                                change.completed_at,
-                                change.context.id,
-                            )
+                            {
+                                "job_id": change.context.id,
+                                "state": change.state,
+                                "completed_at": change.completed_at,
+                            }
                             for change in all_pending_changes
                         ],
                     )
 
                 if maximum_jobs_to_fetch <= 0:
                     return []
 
@@ -366,27 +388,29 @@
                             FOR UPDATE OF {jobs} SKIP LOCKED
                         )
                         UPDATE
                             {jobs}
                         SET
                             started_at = NOW(),
                             attempts = attempts + 1,
-                            state = 'running'
+                            state = 'running',
+                            taken_by = %(worker_id)s
                         FROM
                             selected_jobs
                         WHERE
                             {jobs}.id = selected_jobs.id
                         RETURNING {jobs}.*
                         """
                     ).format(
                         jobs=jobs_table,
                     ),
                     {
                         "queue": queue.name,
                         "maximum_jobs_to_fetch": maximum_jobs_to_fetch,
+                        "worker_id": self.worker_id,
                     },
                 )
                 return [
                     JobContext(
                         job=Job(
                             func=row["payload"]["func"],
                             kwargs=row["payload"]["kwargs"],
@@ -442,14 +466,18 @@
 
         context = self.pools[queue].pop(future)
         job = context.job
 
         # Check to see if something went wrong with the job.
         exc = future.exception()
         if exc is not None:
+            asyncio.run(
+                self.app.hub.emit(self.Event.ON_EXCEPTION, self, exc, context)
+            )
+
             # If the job has a maximum number of attempts, and we haven't
             # exceeded that number, we'll put the job back into the pending
             # state.
             if job.max_attempts and context.attempts < job.max_attempts:
                 self.pending_changes[queue].put_nowait(
                     StateChange(
                         context=context,
@@ -493,40 +521,82 @@
         The leader lock is used to ensure that certain plugins are only run by
         a single worker at a time.
         """
         leader_logger = PrefixAdapter(logger, {"prefix": "LEADER"})
 
         while True:
             async with self.app.pool.connection() as conn:
-                is_leader = await self._try_acquire_leader(conn)
-                if is_leader:
-                    leader_logger.info(
-                        f"Acquired/refreshed leader lock for worker"
-                        f" {self.worker_id}."
-                    )
-                else:
-                    leader_logger.debug(
-                        f"Failed to acquire leader lock for worker"
-                        f" {self.worker_id}."
-                    )
+                result = await self._try_acquire_leader(conn)
+                match result:
+                    case Leadership.REFRESHED:
+                        self.is_leader = True
+                        leader_logger.info(
+                            f"Refreshed leader lock for worker"
+                            f" {self.worker_id}."
+                        )
+                    case Leadership.ACQUIRED:
+                        self.is_leader = True
+                        leader_logger.info(
+                            f"Acquired leader lock for worker"
+                            f" {self.worker_id}."
+                        )
+                        # Bootstrap leadership plugins
+                        for plugin in self.app.plugins:
+                            if plugin.get_type() == plugin.Type.LEADER:
+                                logger.debug(
+                                    f"Starting leader plugin {plugin!r}."
+                                )
+                                await plugin.on_startup(self.app.hub)
+                    case Leadership.UNAVAILABLE:
+                        self.is_leader = False
+                        leader_logger.debug(
+                            f"Failed to acquire leader lock for worker"
+                            f" {self.worker_id}."
+                        )
+                    case Leadership.LOST:
+                        self.is_leader = False
+                        leader_logger.info(
+                            f"Lost leader lock for worker {self.worker_id}."
+                        )
+                        # We've lost leadership, deactivate leadership plugins
+                        for plugin in self.app.plugins:
+                            if plugin.get_type() == plugin.Type.LEADER:
+                                logger.debug(
+                                    f"Shutting down leader plugin"
+                                    f" {plugin!r}."
+                                )
+                                await plugin.on_shutdown(self.app.hub)
+
+                if self.is_leader:
+                    with timed_block() as timer:
+                        await self.app.hub.emit(
+                            self.Event.ON_LEADERSHIP_LOOP, self
+                        )
+                        if timer.elapsed > self.app.leadership_timeout:
+                            leader_logger.warning(
+                                f"Leadership loop took longer than the"
+                                f" leadership timeout of"
+                                f" {self.app.leadership_timeout} seconds."
+                            )
 
                 await asyncio.sleep(self.app.leadership_timeout)
 
-    async def _try_acquire_leader(self, conn: AsyncConnection) -> bool:
+    async def _try_acquire_leader(self, conn: AsyncConnection) -> Leadership:
         """
         Attempt to acquire the leader lock for this worker.
 
         If the leader lock is already held by another worker, this method will
         return False. Otherwise, it will return True.
 
         It's possible for there to be no current valid leader while waiting on
         a worker to time out, but there should never be > 1 leader.
         """
         now = datetime.now(tz=timezone.utc)
         leaders = sql.Identifier(f"{self.app.prefix}leader")
+        was_leader = self.is_leader
 
         async with conn.cursor() as cur:
             try:
                 # It's important that this SELECT covers the entire table to
                 # apply the FOR UPDATE lock.
                 await cur.execute(
                     sql.SQL(
@@ -558,18 +628,24 @@
                                     worker_id = %(worker_id)s,
                                     last_seen = %(last_seen)s
                                 """
                             ).format(leaders=leaders),
                             {"worker_id": self.worker_id, "last_seen": now},
                         )
                         await conn.commit()
-                        return True
+                        if worker_id == self.worker_id:
+                            return Leadership.REFRESHED
+                        return Leadership.ACQUIRED
                     else:
                         await conn.rollback()
-                        return False
+                        return (
+                            Leadership.LOST
+                            if was_leader
+                            else Leadership.UNAVAILABLE
+                        )
                 else:
                     await cur.execute(
                         sql.SQL(
                             """
                             INSERT INTO
                                 {leaders}
                                 (worker_id, last_seen)
@@ -578,11 +654,44 @@
                             ON CONFLICT (worker_id) DO UPDATE SET
                                 last_seen = %(last_seen)s
                             """
                         ).format(leaders=leaders),
                         {"worker_id": self.worker_id, "last_seen": now},
                     )
                     await conn.commit()
-                    return True
+                    return Leadership.ACQUIRED
             except LockNotAvailable:
                 await conn.rollback()
-                return False
+                return Leadership.LOST if was_leader else Leadership.UNAVAILABLE
+
+    async def announce_worker(self, conn: AsyncConnection):
+        """
+        Announce the worker to the cluster.
+        """
+        await conn.execute(
+            sql.SQL(
+                """
+                INSERT INTO {workers}
+                    (worker_id, last_seen)
+                VALUES
+                    (%(worker_id)s, %(last_seen)s)
+                ON CONFLICT (worker_id) DO UPDATE SET
+                    last_seen = %(last_seen)s
+                """
+            ).format(workers=sql.Identifier(f"{self.app.prefix}workers")),
+            {"worker_id": self.worker_id, "last_seen": datetime.now()},
+        )
+
+    async def revoke_worker(self, conn: AsyncConnection):
+        """
+        Revoke the worker from the cluster.
+        """
+        await conn.execute(
+            sql.SQL(
+                """
+                DELETE FROM {workers}
+                WHERE
+                    worker_id = %(worker_id)s
+                """
+            ).format(workers=sql.Identifier(f"{self.app.prefix}workers")),
+            {"worker_id": self.worker_id},
+        )
```

### Comparing `chancy-0.1.0/PKG-INFO` & `chancy-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chancy
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Tyler Kennedy
 Author-email: tk@tkte.ch
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

