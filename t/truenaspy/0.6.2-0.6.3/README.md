# Comparing `tmp/truenaspy-0.6.2.tar.gz` & `tmp/truenaspy-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truenaspy-0.6.2.tar", last modified: Thu Dec 21 13:55:35 2023, max compression
+gzip compressed data, was "truenaspy-0.6.3.tar", last modified: Mon May 27 12:37:48 2024, max compression
```

## Comparing `truenaspy-0.6.2.tar` & `truenaspy-0.6.3.tar`

### file list

```diff
@@ -1,22 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 13:55:35.052246 truenaspy-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-12-21 13:55:18.000000 truenaspy-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-21 13:55:18.000000 truenaspy-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2023-12-21 13:55:35.052246 truenaspy-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      772 2023-12-21 13:55:18.000000 truenaspy-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2023-12-21 13:55:28.000000 truenaspy-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-21 13:55:35.052246 truenaspy-0.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 13:55:35.052246 truenaspy-0.6.2/truenaspy/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2023-12-21 13:55:18.000000 truenaspy-0.6.2/truenaspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18451 2023-12-21 13:55:18.000000 truenaspy-0.6.2/truenaspy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2023-12-21 13:55:18.000000 truenaspy-0.6.2/truenaspy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    12963 2023-12-21 13:55:18.000000 truenaspy-0.6.2/truenaspy/collects.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2023-12-21 13:55:18.000000 truenaspy-0.6.2/truenaspy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2023-12-21 13:55:18.000000 truenaspy-0.6.2/truenaspy/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2023-12-21 13:55:18.000000 truenaspy-0.6.2/truenaspy/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 13:55:35.052246 truenaspy-0.6.2/truenaspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2023-12-21 13:55:35.000000 truenaspy-0.6.2/truenaspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2023-12-21 13:55:35.000000 truenaspy-0.6.2/truenaspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 13:55:35.000000 truenaspy-0.6.2/truenaspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 13:55:34.000000 truenaspy-0.6.2/truenaspy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-21 13:55:35.000000 truenaspy-0.6.2/truenaspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-21 13:55:35.000000 truenaspy-0.6.2/truenaspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:37:48.647072 truenaspy-0.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:37:48.643072 truenaspy-0.6.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-27 12:37:38.000000 truenaspy-0.6.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:37:48.643072 truenaspy-0.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-27 12:37:38.000000 truenaspy-0.6.3/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-27 12:37:38.000000 truenaspy-0.6.3/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-27 12:37:38.000000 truenaspy-0.6.3/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-27 12:37:38.000000 truenaspy-0.6.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-27 12:37:38.000000 truenaspy-0.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-27 12:37:38.000000 truenaspy-0.6.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 12:37:38.000000 truenaspy-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-27 12:37:38.000000 truenaspy-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-27 12:37:48.647072 truenaspy-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-27 12:37:38.000000 truenaspy-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-27 12:37:38.000000 truenaspy-0.6.3/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-27 12:37:38.000000 truenaspy-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-27 12:37:38.000000 truenaspy-0.6.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-27 12:37:38.000000 truenaspy-0.6.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 12:37:48.647072 truenaspy-0.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:37:48.647072 truenaspy-0.6.3/truenaspy/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-27 12:37:38.000000 truenaspy-0.6.3/truenaspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18383 2024-05-27 12:37:38.000000 truenaspy-0.6.3/truenaspy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-27 12:37:38.000000 truenaspy-0.6.3/truenaspy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12964 2024-05-27 12:37:38.000000 truenaspy-0.6.3/truenaspy/collects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-27 12:37:38.000000 truenaspy-0.6.3/truenaspy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-05-27 12:37:38.000000 truenaspy-0.6.3/truenaspy/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-27 12:37:38.000000 truenaspy-0.6.3/truenaspy/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:37:48.647072 truenaspy-0.6.3/truenaspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-27 12:37:48.000000 truenaspy-0.6.3/truenaspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-27 12:37:48.000000 truenaspy-0.6.3/truenaspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:37:48.000000 truenaspy-0.6.3/truenaspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:37:48.000000 truenaspy-0.6.3/truenaspy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 12:37:48.000000 truenaspy-0.6.3/truenaspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 12:37:48.000000 truenaspy-0.6.3/truenaspy.egg-info/top_level.txt
```

### Comparing `truenaspy-0.6.2/LICENSE` & `truenaspy-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.2/PKG-INFO` & `truenaspy-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truenaspy
-Version: 0.6.2
+Version: 0.6.3
 Summary: Provides asynchronous authentication and access to Truenas devices
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: async,truenas,scale,core
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `truenaspy-0.6.2/README.md` & `truenaspy-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.2/truenaspy/api.py` & `truenaspy-0.6.3/truenaspy/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """TrueNAS API."""
+
 from __future__ import annotations
 
 from datetime import datetime, timedelta
 from logging import getLogger
 from typing import Any, Self
 
 from aiohttp import ClientSession
@@ -24,15 +25,15 @@
     Service,
     Smart,
     Snapshottask,
     System,
     Update,
     VirtualMachine,
 )
-from .exceptions import TruenasError, TruenasNotFoundError
+from .exceptions import NotFoundError, TruenasException
 from .helper import (
     ExtendedDict,
     as_local,
     b2gib,
     search_attrs,
     systemstats_process,
     utc_from_timestamp,
@@ -45,30 +46,31 @@
 class TruenasClient(object):
     """Handle all communication with TrueNAS."""
 
     def __init__(
         self,
         host: str,
         token: str,
-        session: ClientSession | None = None,
+        session: ClientSession = ClientSession(),
         use_ssl: bool = False,
         verify_ssl: bool = True,
         scan_intervall: int = 60,
         timeout: int = 300,
     ) -> None:
         """Initialize the TrueNAS API."""
-        self._access = Auth(host, token, use_ssl, verify_ssl, timeout, session)
+        self.auth = Auth(session, host, token, use_ssl, verify_ssl, timeout)
+        self.async_request = self.auth.async_request
+
         self._is_scale: bool = False
         self._is_virtual: bool = False
         self._sub = Subscriptions(
             (self.async_update, self.async_is_alive), scan_intervall
         )
         self.is_connected: bool = False
         self._systemstats_errored: list[str] = []
-        self.query = self._access.async_request
         self.alerts: list[dict[str, Any]] = []
         self.charts: list[dict[str, Any]] = []
         self.cloudsync: list[dict[str, Any]] = []
         self.datasets: list[dict[str, Any]] = []
         self.disks: list[dict[str, Any]] = []
         self.interfaces: list[dict[str, Any]] = []
         self.jails: list[dict[str, Any]] = []
@@ -81,21 +83,21 @@
         self.stats: dict[str, Any] = {}
         self.system_infos: dict[str, Any] = {}
         self.update_infos: dict[str, Any] = {}
         self.virtualmachines: list[dict[str, Any]] = []
 
     async def async_get_system(self) -> dict[str, Any]:
         """Get system info from TrueNAS."""
-        response = await self.query(path="system/info")
+        response = await self.async_request("system/info")
         self.system_infos = search_attrs(System, response)
 
-        response = await self.query(path="system/version_short")
+        response = await self.async_request("system/version_short")
         self.system_infos.update({"short_version": response})
 
-        response = await self.query(path="system/is_freenas")
+        response = await self.async_request("system/is_freenas")
         self._is_scale = response is False
         self._is_virtual = self.system_infos["system_manufacturer"] in [
             "QEMU",
             "VMware, Inc.",
         ] or self.system_infos["system_product"] in ["VirtualBox"]
 
         if (uptime := self.system_infos["uptime_seconds"]) > 0:
@@ -196,15 +198,15 @@
             #     systemstats_process(self.system_infos, tmp_arr, item, "arc")
 
         self._sub.notify(Events.SYSTEM.value)
         return self.system_infos
 
     async def async_get_interfaces(self) -> list[dict[str, Any]]:
         """Get interface info from TrueNAS."""
-        response = await self.query(path="interface")
+        response = await self.async_request("interface")
         self.interfaces = search_attrs(Interfaces, response)
 
         # Get stats
         query = [
             {"name": "interface", "identifier": interface["id"]}
             for interface in self.interfaces
         ]
@@ -237,23 +239,23 @@
 
         for param in query["graphs"]:
             if param["name"] in self._systemstats_errored:
                 query["graphs"].remove(param)
 
         stats = []
         try:
-            stats = await self._access.async_request(
-                "reporting/get_data", method="post", json=query
+            stats = await self.auth.async_request(
+                "reporting/get_data", "post", json=query
             )
 
             if "error" in stats:
                 for param in query["graphs"]:
-                    await self._access.async_request(
+                    await self.auth.async_request(
                         "reporting/get_data",
-                        method="post",
+                        "post",
                         json={
                             "graphs": [param],
                             "reporting_query": {
                                 "start": start,
                                 "end": end,
                                 "aggregate": True,
                             },
@@ -263,40 +265,40 @@
                         self._systemstats_errored.append(param["name"])
 
                 _LOGGER.warning(
                     "Fetching following graphs failed, check your NAS: %s",
                     self._systemstats_errored,
                 )
                 await self.async_get_stats(items)
-        except TruenasError as error:
+        except TruenasException as error:
             # ERROR FIX: Cobia NAS-123862
             if self.system_infos.get("short_version") not in [
                 "23.10.0",
                 "23.10.0.0",
                 "23.10.0.1",
             ]:
                 _LOGGER.error(error)
 
         return stats
 
     async def async_get_services(self) -> list[dict[str, Any]]:
         """Get service info from TrueNAS."""
-        response = await self.query(path="service")
+        response = await self.async_request("service")
         self.services = search_attrs(Service, response)
         self._sub.notify(Events.SERVICES.value)
         return self.services
 
     async def async_get_pools(self) -> list[dict[str, Any]]:
         """Get pools from TrueNAS."""
-        response = await self.query(path="pool")
+        response = await self.async_request("pool")
         self.pools = search_attrs(Pool, response)
 
         try:
-            response = await self.query(path="boot/get_state")
-        except TruenasError as error:
+            response = await self.async_request("boot/get_state")
+        except TruenasException as error:
             _LOGGER.debug(error)
             response = ExtendedDict()
 
         boot = search_attrs(Boot, response)
         self.pools.append(boot)
 
         # Process pools
@@ -327,133 +329,133 @@
                 # self.pools[uid].pop("root_dataset")
 
         self._sub.notify(Events.POOLS.value)
         return self.pools
 
     async def async_get_datasets(self) -> list[dict[str, Any]]:
         """Get datasets from TrueNAS."""
-        # response = await self.query(path="pool/dataset/details")
-        response = await self.query(path="pool/dataset")
+        # response = await self.async_request("pool/dataset/details")
+        response = await self.async_request("pool/dataset")
         self.datasets = search_attrs(Datasets, response)
         self._sub.notify(Events.DATASETS.value)
         return self.datasets
 
     async def async_get_disks(self) -> list[dict[str, Any]]:
         """Get disks from TrueNAS."""
-        response = await self.query(path="disk")
+        response = await self.async_request("disk")
         self.disks = search_attrs(Disk, response)
         # Get disk temperatures
-        temperatures = await self._access.async_request(
-            "disk/temperatures", method="post", json={"names": []}
+        temperatures = await self.auth.async_request(
+            "disk/temperatures", "post", json={"names": []}
         )
         for disk in self.disks:
             disk.update({"temperature": temperatures.get(disk["name"], 0)})
         self._sub.notify(Events.DISKS.value)
         return self.disks
 
     async def async_get_jails(self) -> list[dict[str, Any]] | None:
         """Get jails from TrueNAS."""
         if self._is_scale is False:
             try:
-                response = await self.query(path="jail")
+                response = await self.async_request("jail")
                 self.jails = search_attrs(Jail, response)
-            except TruenasNotFoundError as error:
+            except NotFoundError as error:
                 _LOGGER.warning(error)
                 self.jails = []
         self._sub.notify(Events.JAILS.value)
         return self.jails
 
     async def async_get_virtualmachines(self) -> list[dict[str, Any]]:
         """Get VMs from TrueNAS."""
-        response = await self.query(path="vm")
+        response = await self.async_request("vm")
         self.virtualmachines = search_attrs(VirtualMachine, response)
         self._sub.notify(Events.VMS.value)
         return self.virtualmachines
 
     async def async_get_cloudsync(self) -> list[dict[str, Any]]:
         """Get cloudsync from TrueNAS."""
-        response = await self.query(path="cloudsync")
+        response = await self.async_request("cloudsync")
         self.cloudsync = search_attrs(CloudSync, response)
         self._sub.notify(Events.CLOUD.value)
         return self.cloudsync
 
     async def async_get_replications(self) -> list[dict[str, Any]]:
         """Get replication from TrueNAS."""
-        response = await self.query(path="replication")
+        response = await self.async_request("replication")
         self.replications = search_attrs(Replication, response)
         self._sub.notify(Events.REPLS.value)
         return self.replications
 
     async def async_get_snapshottasks(self) -> list[dict[str, Any]]:
         """Get replication from TrueNAS."""
-        response = await self.query(path="pool/snapshottask")
+        response = await self.async_request("pool/snapshottask")
         self.snapshots = search_attrs(Snapshottask, response)
         self._sub.notify(Events.SNAPS.value)
         return self.snapshots
 
     async def async_get_charts(self) -> list[dict[str, Any]]:
         """Get Charts from TrueNAS."""
-        response = await self.query(path="chart/release")
+        response = await self.async_request("chart/release")
         self.charts = search_attrs(Charts, response)
         self._sub.notify(Events.CHARTS.value)
         return self.charts
 
     async def async_get_smartdisks(self) -> list[dict[str, Any]]:
         """Get smartdisk from TrueNAS."""
-        response = await self.query(path="smart/test/results", params={"offset": 1})
+        response = await self.async_request("smart/test/results", params={"offset": 1})
         self.smartdisks = search_attrs(Smart, response)
         self._sub.notify(Events.SMARTS.value)
         return self.smartdisks
 
     async def async_get_alerts(self) -> list[dict[str, Any]]:
         """Get smartdisk from TrueNAS."""
-        response = await self.query(path="alert/list")
+        response = await self.async_request("alert/list")
         self.alerts = search_attrs(Alerts, response)
         self._sub.notify(Events.ALERTS.value)
         return self.alerts
 
     async def async_get_rsynctasks(self) -> list[dict[str, Any]]:
         """Get smartdisk from TrueNAS."""
-        response = await self.query(path="rsynctask")
+        response = await self.async_request("rsynctask")
         self.rsynctasks = search_attrs(Rsync, response)
         self._sub.notify(Events.RSYNC.value)
         return self.rsynctasks
 
     async def async_get_update(self) -> dict[str, Any]:
         """Get update info from TrueNAS."""
         try:
-            response = await self.query(path="update/check_available", method="post")
-        except TruenasError as error:
+            response = await self.async_request("update/check_available", "post")
+        except TruenasException as error:
             _LOGGER.debug(error)
             response = ExtendedDict()
         self.update_infos = search_attrs(Update, response)
 
         try:
-            response = await self.query(path="update/get_trains")
-        except TruenasError as error:
+            response = await self.async_request("update/get_trains")
+        except TruenasException as error:
             _LOGGER.debug(error)
             response = ExtendedDict()
         self.update_infos.update({"current_train": response.get("current")})
 
         if jobid := self.system_infos.get("job_id", 0):
-            response = await self.query(path="core/get_jobs", params={"id": jobid})
+            response = await self.async_request("core/get_jobs", params={"id": jobid})
             jobs = search_attrs(Job, response)
             for job in jobs:
                 if (
                     job.get("state") != "RUNNING"
                     or not self.update_infos["update_available"]
                 ):
                     self.update_infos.update(
                         {"progress": 0, "status": None, "job_id": 0}
                     )
         return self.update_infos
 
     async def async_is_alive(self) -> bool:
         """Check connection."""
-        result = await self._access.async_request("core/ping")
+        result = await self.auth.async_request("core/ping")
         return "pong" in result
 
     def subscribe(self, _callback: str, *args: Any) -> None:
         """Subscribe event."""
         self._sub.subscribe(_callback, *args)
 
     def unsubscribe(self, _callback: str, *args: Any) -> None:
@@ -466,38 +468,29 @@
             await self.async_is_alive()
             nb_events = len(Events)
             nb_errors = 0
             for event in Events:
                 try:
                     fnc = getattr(self, f"async_get_{event.value}")
                     await fnc()
-                except TruenasError as error:
+                except TruenasException as error:
                     _LOGGER.error(error)
                     nb_errors += 1
             self.is_connected = (
                 False if nb_errors > 0 and nb_events == nb_errors else True
             )
-        except TruenasError as error:
+        except TruenasException as error:
             _LOGGER.error(error)
             self.is_connected = False
 
     async def async_close(self) -> None:
         """Close open client session."""
-        await self._access.async_close()
+        if self.auth._session:
+            await self.auth._session.close()
 
     async def __aenter__(self) -> Self:
-        """Async enter.
-
-        Returns
-        -------
-            The LaMetricCloud object.
-        """
+        """Async enter."""
         return self
 
     async def __aexit__(self, *_exc_info: object) -> None:
-        """Async exit.
-
-        Args:
-        ----
-            _exc_info: Exec type.
-        """
+        """Async exit."""
         await self.async_close()
```

### Comparing `truenaspy-0.6.2/truenaspy/auth.py` & `truenaspy-0.6.3/truenaspy/auth.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,96 +1,88 @@
 """TrueNAS API."""
+
 from __future__ import annotations
 
 import asyncio
-import socket
-from dataclasses import dataclass, field
 from logging import getLogger
+import socket
 from typing import Any
 
 from aiohttp import ClientError, ClientResponseError, ClientSession
 
 from .exceptions import (
-    TruenasAuthenticationError,
-    TruenasConnectionError,
-    TruenasError,
-    TruenasNotFoundError,
+    AuthenticationFailed,
+    NotFoundError,
+    TimeoutExceededError,
+    TruenasException,
+    UnexpectedResponse,
 )
 from .helper import json_loads
 
 _LOGGER = getLogger(__name__)
 
 API_PATH = "api/v2.0"
 
 
-@dataclass
 class Auth:
     """Handle all communication with TrueNAS."""
 
-    host: str
-    api_key: str
-    use_ssl: bool
-    verify_ssl: bool
-    timeout: int = 120
-    session: ClientSession | None = None
-
-    _protocol: str = field(init=False)
     _close_session: bool = False
-    _url: str = field(init=False)
 
-    def __post_init__(self) -> None:
-        self._protocol: str = "https" if self.use_ssl else "http"
-        self._url = f"{self._protocol}://{self.host}/{API_PATH}"
+    def __init__(
+        self,
+        session: ClientSession,
+        host: str,
+        token: str,
+        use_ssl: bool = False,
+        verify_ssl: bool = True,
+        timeout: int = 120,
+    ) -> None:
+        scheme = "https" if use_ssl else "http"
+        self._url = f"{scheme}://{host}/{API_PATH}"
+        self._verify_ssl = verify_ssl
+        self._access_token = token
+        self._timeout = timeout
+        self._session = session
 
-    async def async_request(self, path: str, method: str = "GET", **kwargs: Any) -> Any:
+    async def async_request(self, path: str, method: str = "get", **kwargs: Any) -> Any:
         """Make a request."""
-        if self.session is None:
-            self.session = ClientSession()
-            self._close_session = True
-
-        headers = kwargs.pop("headers", {})
-        headers.update(
+        kwargs.setdefault("headers", {})
+        kwargs.setdefault("verify_ssl", self._verify_ssl)
+        kwargs["headers"].update(
             {
                 "Accept": "application/json",
-                "Authorization": f"Bearer {self.api_key}",
+                "Authorization": f"Bearer {self._access_token}",
             }
         )
         try:
-            _LOGGER.debug("TrueNAS %s query: %s (%s)", self.host, path, method)
-            _LOGGER.debug("POST Content: %s", kwargs.get("json"))
-            async with asyncio.timeout(self.timeout):
-                response = await self.session.request(
-                    method,
-                    f"{self._url}/{path}",
-                    **kwargs,
-                    headers=headers,
-                    verify_ssl=self.verify_ssl,
+            async with asyncio.timeout(self._timeout):
+                _LOGGER.debug(
+                    "Url: %s (%s) - Content: %s", path, method, kwargs.get("json")
+                )
+                response = await self._session.request(
+                    method, f"{self._url}/{path}", **kwargs
                 )
                 response.raise_for_status()
         except (asyncio.CancelledError, asyncio.TimeoutError) as error:
             msg = "Timeout occurred while connecting to the Truenas API"
-            raise TruenasConnectionError(msg) from error
+            raise TimeoutExceededError(msg) from error
         except ClientResponseError as error:
             if error.status in [401, 403]:
                 msg = "Authentication to the Truenas API failed"
-                raise TruenasAuthenticationError(msg) from error
+                raise AuthenticationFailed(msg) from error
             if error.status in [404]:
                 msg = f"API not found ({path} - {error.status})"
-                raise TruenasNotFoundError(msg) from error
+                raise NotFoundError(msg) from error
             msg = f"Error occurred while communicating with Truenas ({error})"
-            raise TruenasError(msg) from error
+            raise TruenasException(msg) from error
         except (ClientError, socket.gaierror) as error:
             msg = "Error occurred while communicating with Truenas"
-            raise TruenasError(msg) from error
+            raise TruenasException(msg) from error
 
         try:
-            data: Any = await response.json(loads=json_loads)
-            _LOGGER.debug("TrueNAS %s query response: %s", self.host, data)
+            data = await response.json(loads=json_loads)
+            _LOGGER.debug("Response: %s", data)
             return data
         except ValueError as error:
             msg = "The Truenas API response is not formatted correctly"
-            raise TruenasError(error) from error
-
-    async def async_close(self) -> None:
-        """Close open client session."""
-        if self.session and self._close_session:
-            await self.session.close()
+            raise UnexpectedResponse(f"Error while decoding Json ({error})") from error
```

### Comparing `truenaspy-0.6.2/truenaspy/collects.py` & `truenaspy-0.6.3/truenaspy/collects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Class to collect a data."""
+
 from .helper import FieldType, b2gib, utc_from_timestamp
 
 
 class System:
     """System."""
 
     attrs = [
```

### Comparing `truenaspy-0.6.2/truenaspy/helper.py` & `truenaspy-0.6.3/truenaspy/helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """API parser for JSON APIs."""
+
 from __future__ import annotations
 
-import json
 from datetime import datetime
 from functools import reduce
+import json
 from logging import getLogger
 from typing import Any, Callable, Type
 
-from pytz import utc
+from pytz import utc  # type: ignore[import-untyped]
 
 _LOGGER = getLogger(__name__)
 
 
 class ExtendedDict(dict[Any, Any]):
     """Extend dictionary class."""
 
@@ -32,15 +33,15 @@
 
     name: str
     default: Any = None
     source: str | None = None
     evaluation: Callable[..., Any] | None = None
 
 
-def utc_from_timestamp(timestamp: float) -> datetime:
+def utc_from_timestamp(timestamp: float) -> Any:
     """Return a UTC time from a timestamp."""
     return utc.localize(datetime.utcfromtimestamp(timestamp))
 
 
 def b2gib(b: int) -> float | None:
     """Convert byte to gigabyte."""
     if isinstance(b, int):
@@ -99,18 +100,18 @@
                     fill_dict[f"{mode}_{item}"] = round(value, 2)
                 else:
                     fill_dict[item] = round(value, 2)
 
 
 def search_attrs(identity: Type[Any], dataref: Any) -> Any:
     """Map attributes."""
-    attributes: list[dict[str, Any]] = []
+    attributes: list[dict[str, Any]] | dict[str, Any] = []
     if dataref is not None and identity.attrs:
         if not isinstance(dataref, list):
-            attributes: dict[str, Any] = {}  # type: ignore[no-redef]
+            attributes = {}
             dataref = [dataref]
         for item in dataref:
             attrs = {}
             for attr in identity.attrs:
                 name = attr["name"]
                 key = attr.get("source", name)
                 value = item.getr(key, attr.get("default"))
@@ -119,10 +120,10 @@
                         value = evaluation(value)
                     except Exception as error:  # pylint: disable=broad-except
                         _LOGGER.error(error)
                 attrs.update({name: value})
             if isinstance(attributes, list):
                 attributes.append(attrs)
             else:
-                attributes.update(attrs)  # type: ignore[unreachable]
+                attributes.update(attrs)
 
     return attributes
```

### Comparing `truenaspy-0.6.2/truenaspy/subscription.py` & `truenaspy-0.6.3/truenaspy/subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """TrueNAS API Subscription."""
+
 from __future__ import annotations
 
 import asyncio
 import time
 from enum import Enum
 from logging import getLogger
 from typing import Any, Callable, List, Tuple
```

### Comparing `truenaspy-0.6.2/truenaspy.egg-info/PKG-INFO` & `truenaspy-0.6.3/truenaspy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truenaspy
-Version: 0.6.2
+Version: 0.6.3
 Summary: Provides asynchronous authentication and access to Truenas devices
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: async,truenas,scale,core
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

