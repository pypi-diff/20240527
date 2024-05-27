# Comparing `tmp/asynch_lxneng-0.2.4.tar.gz` & `tmp/asynch_lxneng-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asynch_lxneng-0.2.4.tar", max compression
+gzip compressed data, was "asynch_lxneng-0.2.5.tar", max compression
```

## Comparing `asynch_lxneng-0.2.4.tar` & `asynch_lxneng-0.2.5.tar`

### file list

```diff
@@ -1,60 +1,59 @@
--rw-r--r--   0        0        0     1041 2023-10-18 07:31:20.647700 asynch_lxneng-0.2.4/CHANGELOG.md
--rw-r--r--   0        0        0    11338 2023-10-18 07:31:20.647789 asynch_lxneng-0.2.4/LICENSE
--rw-r--r--   0        0        0     4394 2023-10-18 07:31:20.647937 asynch_lxneng-0.2.4/README.md
--rw-r--r--   0        0        0       88 2023-10-18 07:31:20.648023 asynch_lxneng-0.2.4/asynch/__init__.py
--rw-r--r--   0        0        0     5596 2023-10-18 07:31:20.648097 asynch_lxneng-0.2.4/asynch/connection.py
--rw-r--r--   0        0        0    10868 2023-10-18 07:31:20.648191 asynch_lxneng-0.2.4/asynch/cursors.py
--rw-r--r--   0        0        0    14806 2023-10-18 07:31:20.648295 asynch_lxneng-0.2.4/asynch/errors.py
--rw-r--r--   0        0        0     7005 2023-10-20 07:16:18.174750 asynch_lxneng-0.2.4/asynch/pool.py
--rw-r--r--   0        0        0        0 2023-10-18 07:31:20.648445 asynch_lxneng-0.2.4/asynch/proto/__init__.py
--rw-r--r--   0        0        0     6746 2023-10-18 07:31:20.648541 asynch_lxneng-0.2.4/asynch/proto/block.py
--rw-r--r--   0        0        0     5748 2023-10-18 07:31:20.648671 asynch_lxneng-0.2.4/asynch/proto/columns/__init__.py
--rw-r--r--   0        0        0     6911 2023-10-18 07:31:20.648753 asynch_lxneng-0.2.4/asynch/proto/columns/arraycolumn.py
--rw-r--r--   0        0        0     4913 2023-10-18 07:31:20.648820 asynch_lxneng-0.2.4/asynch/proto/columns/base.py
--rw-r--r--   0        0        0      146 2023-10-18 07:31:20.648877 asynch_lxneng-0.2.4/asynch/proto/columns/boolcolumn.py
--rw-r--r--   0        0        0     1368 2023-10-18 07:31:20.648951 asynch_lxneng-0.2.4/asynch/proto/columns/datecolumn.py
--rw-r--r--   0        0        0     7093 2023-10-18 07:31:20.649029 asynch_lxneng-0.2.4/asynch/proto/columns/datetimecolumn.py
--rw-r--r--   0        0        0     3440 2023-10-18 07:31:20.649098 asynch_lxneng-0.2.4/asynch/proto/columns/decimalcolumn.py
--rw-r--r--   0        0        0     3275 2023-10-18 07:31:20.649166 asynch_lxneng-0.2.4/asynch/proto/columns/enumcolumn.py
--rw-r--r--   0        0        0      953 2023-10-18 07:31:20.649243 asynch_lxneng-0.2.4/asynch/proto/columns/floatcolumn.py
--rw-r--r--   0        0        0     3543 2023-10-18 07:31:20.649302 asynch_lxneng-0.2.4/asynch/proto/columns/intcolumn.py
--rw-r--r--   0        0        0      600 2023-10-18 07:31:20.649378 asynch_lxneng-0.2.4/asynch/proto/columns/intervalcolumn.py
--rw-r--r--   0        0        0     4173 2023-10-18 07:31:20.649474 asynch_lxneng-0.2.4/asynch/proto/columns/ipcolumn.py
--rw-r--r--   0        0        0     1025 2023-10-18 07:31:20.649551 asynch_lxneng-0.2.4/asynch/proto/columns/jsoncolumn.py
--rw-r--r--   0        0        0     4301 2023-10-18 07:31:20.649627 asynch_lxneng-0.2.4/asynch/proto/columns/lowcardinalitycolumn.py
--rw-r--r--   0        0        0     2053 2023-10-18 07:31:20.649697 asynch_lxneng-0.2.4/asynch/proto/columns/mapcolumn.py
--rw-r--r--   0        0        0      621 2023-10-18 07:31:20.649760 asynch_lxneng-0.2.4/asynch/proto/columns/nestedcolumn.py
--rw-r--r--   0        0        0      258 2023-10-18 07:31:20.649835 asynch_lxneng-0.2.4/asynch/proto/columns/nothingcolumn.py
--rw-r--r--   0        0        0      167 2023-10-18 07:31:20.649897 asynch_lxneng-0.2.4/asynch/proto/columns/nullablecolumn.py
--rw-r--r--   0        0        0      330 2023-10-18 07:31:20.650008 asynch_lxneng-0.2.4/asynch/proto/columns/nullcolumn.py
--rw-r--r--   0        0        0      305 2023-10-18 07:31:20.650097 asynch_lxneng-0.2.4/asynch/proto/columns/simpleaggregatefunctioncolumn.py
--rw-r--r--   0        0        0     1824 2023-10-18 07:31:20.650179 asynch_lxneng-0.2.4/asynch/proto/columns/stringcolumn.py
--rw-r--r--   0        0        0     2069 2023-10-18 07:31:20.650249 asynch_lxneng-0.2.4/asynch/proto/columns/tuplecolumn.py
--rw-r--r--   0        0        0     1351 2023-10-18 07:31:20.650326 asynch_lxneng-0.2.4/asynch/proto/columns/util.py
--rw-r--r--   0        0        0     1926 2023-10-18 07:31:20.650418 asynch_lxneng-0.2.4/asynch/proto/columns/uuidcolumn.py
--rw-r--r--   0        0        0     3284 2023-10-18 07:31:20.650585 asynch_lxneng-0.2.4/asynch/proto/compression/__init__.py
--rw-r--r--   0        0        0      767 2023-10-18 07:31:20.650671 asynch_lxneng-0.2.4/asynch/proto/compression/lz4.py
--rw-r--r--   0        0        0      211 2023-10-18 07:31:20.650730 asynch_lxneng-0.2.4/asynch/proto/compression/lz4hc.py
--rw-r--r--   0        0        0      640 2023-10-18 07:31:20.650787 asynch_lxneng-0.2.4/asynch/proto/compression/zstd.py
--rw-r--r--   0        0        0    34939 2023-10-18 07:31:20.650952 asynch_lxneng-0.2.4/asynch/proto/connection.py
--rw-r--r--   0        0        0     1483 2023-10-18 07:31:20.651031 asynch_lxneng-0.2.4/asynch/proto/constants.py
--rw-r--r--   0        0        0     1588 2023-10-18 07:31:20.651093 asynch_lxneng-0.2.4/asynch/proto/context.py
--rw-r--r--   0        0        0     5427 2023-10-18 07:31:20.651185 asynch_lxneng-0.2.4/asynch/proto/cs.py
--rw-r--r--   0        0        0     1591 2023-10-18 07:31:20.651248 asynch_lxneng-0.2.4/asynch/proto/opentelemetry.py
--rw-r--r--   0        0        0     1183 2023-10-18 07:31:20.651310 asynch_lxneng-0.2.4/asynch/proto/progress.py
--rw-r--r--   0        0        0     2593 2023-10-18 07:31:20.651390 asynch_lxneng-0.2.4/asynch/proto/protocol.py
--rw-r--r--   0        0        0     5248 2023-10-18 07:31:20.651479 asynch_lxneng-0.2.4/asynch/proto/result.py
--rw-r--r--   0        0        0     1208 2023-10-18 07:31:20.651594 asynch_lxneng-0.2.4/asynch/proto/settings/__init__.py
--rw-r--r--   0        0        0    16595 2023-10-18 07:31:20.651703 asynch_lxneng-0.2.4/asynch/proto/settings/available.py
--rw-r--r--   0        0        0     1249 2023-10-18 07:31:20.651778 asynch_lxneng-0.2.4/asynch/proto/settings/types.py
--rw-r--r--   0        0        0        0 2023-10-18 07:31:20.651837 asynch_lxneng-0.2.4/asynch/proto/streams/__init__.py
--rw-r--r--   0        0        0     2960 2023-10-18 07:31:20.651917 asynch_lxneng-0.2.4/asynch/proto/streams/block.py
--rw-r--r--   0        0        0     7515 2023-10-18 07:31:20.652003 asynch_lxneng-0.2.4/asynch/proto/streams/buffered.py
--rw-r--r--   0        0        0     2267 2023-10-18 07:31:20.652068 asynch_lxneng-0.2.4/asynch/proto/streams/compressed.py
--rw-r--r--   0        0        0        0 2023-10-18 07:31:20.652119 asynch_lxneng-0.2.4/asynch/proto/utils/__init__.py
--rw-r--r--   0        0        0      599 2023-10-18 07:31:20.652190 asynch_lxneng-0.2.4/asynch/proto/utils/compat.py
--rw-r--r--   0        0        0     1227 2023-10-18 07:31:20.652248 asynch_lxneng-0.2.4/asynch/proto/utils/escape.py
--rw-r--r--   0        0        0      783 2023-10-18 07:31:20.652304 asynch_lxneng-0.2.4/asynch/proto/utils/helpers.py
--rw-r--r--   0        0        0     1231 2023-10-20 07:21:40.874218 asynch_lxneng-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     5512 1970-01-01 00:00:00.000000 asynch_lxneng-0.2.4/setup.py
--rw-r--r--   0        0        0     5444 1970-01-01 00:00:00.000000 asynch_lxneng-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1243 2024-05-27 02:04:39.179127 asynch_lxneng-0.2.5/CHANGELOG.md
+-rw-r--r--   0        0        0    11338 2024-05-27 02:04:39.179283 asynch_lxneng-0.2.5/LICENSE
+-rw-r--r--   0        0        0     4394 2024-05-27 02:04:39.179472 asynch_lxneng-0.2.5/README.md
+-rw-r--r--   0        0        0       88 2024-05-27 02:04:39.179576 asynch_lxneng-0.2.5/asynch/__init__.py
+-rw-r--r--   0        0        0     5543 2024-05-27 02:04:39.179677 asynch_lxneng-0.2.5/asynch/connection.py
+-rw-r--r--   0        0        0    10941 2024-05-27 02:04:39.179823 asynch_lxneng-0.2.5/asynch/cursors.py
+-rw-r--r--   0        0        0    14806 2024-05-27 02:04:39.179954 asynch_lxneng-0.2.5/asynch/errors.py
+-rw-r--r--   0        0        0     7215 2024-05-27 02:04:39.180050 asynch_lxneng-0.2.5/asynch/pool.py
+-rw-r--r--   0        0        0        0 2024-05-27 02:04:39.180115 asynch_lxneng-0.2.5/asynch/proto/__init__.py
+-rw-r--r--   0        0        0     6746 2024-05-27 02:04:39.180227 asynch_lxneng-0.2.5/asynch/proto/block.py
+-rw-r--r--   0        0        0     5784 2024-05-27 02:04:39.180368 asynch_lxneng-0.2.5/asynch/proto/columns/__init__.py
+-rw-r--r--   0        0        0     6911 2024-05-27 02:04:39.180466 asynch_lxneng-0.2.5/asynch/proto/columns/arraycolumn.py
+-rw-r--r--   0        0        0     4913 2024-05-27 02:04:39.180560 asynch_lxneng-0.2.5/asynch/proto/columns/base.py
+-rw-r--r--   0        0        0      146 2024-05-27 02:04:39.180622 asynch_lxneng-0.2.5/asynch/proto/columns/boolcolumn.py
+-rw-r--r--   0        0        0     2098 2024-05-27 02:04:39.180686 asynch_lxneng-0.2.5/asynch/proto/columns/datecolumn.py
+-rw-r--r--   0        0        0     7093 2024-05-27 02:04:39.180784 asynch_lxneng-0.2.5/asynch/proto/columns/datetimecolumn.py
+-rw-r--r--   0        0        0     3440 2024-05-27 02:04:39.180863 asynch_lxneng-0.2.5/asynch/proto/columns/decimalcolumn.py
+-rw-r--r--   0        0        0     3275 2024-05-27 02:04:39.180936 asynch_lxneng-0.2.5/asynch/proto/columns/enumcolumn.py
+-rw-r--r--   0        0        0      953 2024-05-27 02:04:39.181016 asynch_lxneng-0.2.5/asynch/proto/columns/floatcolumn.py
+-rw-r--r--   0        0        0     3543 2024-05-27 02:04:39.181077 asynch_lxneng-0.2.5/asynch/proto/columns/intcolumn.py
+-rw-r--r--   0        0        0      600 2024-05-27 02:04:39.181139 asynch_lxneng-0.2.5/asynch/proto/columns/intervalcolumn.py
+-rw-r--r--   0        0        0     4173 2024-05-27 02:04:39.181233 asynch_lxneng-0.2.5/asynch/proto/columns/ipcolumn.py
+-rw-r--r--   0        0        0     1025 2024-05-27 02:04:39.181320 asynch_lxneng-0.2.5/asynch/proto/columns/jsoncolumn.py
+-rw-r--r--   0        0        0     4301 2024-05-27 02:04:39.181429 asynch_lxneng-0.2.5/asynch/proto/columns/lowcardinalitycolumn.py
+-rw-r--r--   0        0        0     2053 2024-05-27 02:04:39.181518 asynch_lxneng-0.2.5/asynch/proto/columns/mapcolumn.py
+-rw-r--r--   0        0        0      621 2024-05-27 02:04:39.181598 asynch_lxneng-0.2.5/asynch/proto/columns/nestedcolumn.py
+-rw-r--r--   0        0        0      258 2024-05-27 02:04:39.181690 asynch_lxneng-0.2.5/asynch/proto/columns/nothingcolumn.py
+-rw-r--r--   0        0        0      167 2024-05-27 02:04:39.181768 asynch_lxneng-0.2.5/asynch/proto/columns/nullablecolumn.py
+-rw-r--r--   0        0        0      330 2024-05-27 02:04:39.181839 asynch_lxneng-0.2.5/asynch/proto/columns/nullcolumn.py
+-rw-r--r--   0        0        0      305 2024-05-27 02:04:39.181916 asynch_lxneng-0.2.5/asynch/proto/columns/simpleaggregatefunctioncolumn.py
+-rw-r--r--   0        0        0     1824 2024-05-27 02:04:39.181983 asynch_lxneng-0.2.5/asynch/proto/columns/stringcolumn.py
+-rw-r--r--   0        0        0     2069 2024-05-27 02:04:39.182058 asynch_lxneng-0.2.5/asynch/proto/columns/tuplecolumn.py
+-rw-r--r--   0        0        0     1351 2024-05-27 02:04:39.182129 asynch_lxneng-0.2.5/asynch/proto/columns/util.py
+-rw-r--r--   0        0        0     1926 2024-05-27 02:04:39.182214 asynch_lxneng-0.2.5/asynch/proto/columns/uuidcolumn.py
+-rw-r--r--   0        0        0     3284 2024-05-27 02:04:39.182334 asynch_lxneng-0.2.5/asynch/proto/compression/__init__.py
+-rw-r--r--   0        0        0      767 2024-05-27 02:04:39.182410 asynch_lxneng-0.2.5/asynch/proto/compression/lz4.py
+-rw-r--r--   0        0        0      211 2024-05-27 02:04:39.182471 asynch_lxneng-0.2.5/asynch/proto/compression/lz4hc.py
+-rw-r--r--   0        0        0      640 2024-05-27 02:04:39.182532 asynch_lxneng-0.2.5/asynch/proto/compression/zstd.py
+-rw-r--r--   0        0        0    34971 2024-05-27 02:04:39.182686 asynch_lxneng-0.2.5/asynch/proto/connection.py
+-rw-r--r--   0        0        0     1483 2024-05-27 02:04:39.182817 asynch_lxneng-0.2.5/asynch/proto/constants.py
+-rw-r--r--   0        0        0     1722 2024-05-27 02:04:39.182913 asynch_lxneng-0.2.5/asynch/proto/context.py
+-rw-r--r--   0        0        0     5427 2024-05-27 02:04:39.183070 asynch_lxneng-0.2.5/asynch/proto/cs.py
+-rw-r--r--   0        0        0     1591 2024-05-27 02:04:39.183136 asynch_lxneng-0.2.5/asynch/proto/opentelemetry.py
+-rw-r--r--   0        0        0     1183 2024-05-27 02:04:39.183204 asynch_lxneng-0.2.5/asynch/proto/progress.py
+-rw-r--r--   0        0        0     2593 2024-05-27 02:04:39.183284 asynch_lxneng-0.2.5/asynch/proto/protocol.py
+-rw-r--r--   0        0        0     5248 2024-05-27 02:04:39.183390 asynch_lxneng-0.2.5/asynch/proto/result.py
+-rw-r--r--   0        0        0     1207 2024-05-27 02:04:39.183499 asynch_lxneng-0.2.5/asynch/proto/settings/__init__.py
+-rw-r--r--   0        0        0    16595 2024-05-27 02:04:39.183587 asynch_lxneng-0.2.5/asynch/proto/settings/available.py
+-rw-r--r--   0        0        0     1249 2024-05-27 02:04:39.183672 asynch_lxneng-0.2.5/asynch/proto/settings/types.py
+-rw-r--r--   0        0        0        0 2024-05-27 02:04:39.183735 asynch_lxneng-0.2.5/asynch/proto/streams/__init__.py
+-rw-r--r--   0        0        0     2960 2024-05-27 02:04:39.183822 asynch_lxneng-0.2.5/asynch/proto/streams/block.py
+-rw-r--r--   0        0        0     7627 2024-05-27 02:04:39.183930 asynch_lxneng-0.2.5/asynch/proto/streams/buffered.py
+-rw-r--r--   0        0        0     2267 2024-05-27 02:04:39.184008 asynch_lxneng-0.2.5/asynch/proto/streams/compressed.py
+-rw-r--r--   0        0        0        0 2024-05-27 02:04:39.184074 asynch_lxneng-0.2.5/asynch/proto/utils/__init__.py
+-rw-r--r--   0        0        0      599 2024-05-27 02:04:39.184154 asynch_lxneng-0.2.5/asynch/proto/utils/compat.py
+-rw-r--r--   0        0        0     1227 2024-05-27 02:04:39.184218 asynch_lxneng-0.2.5/asynch/proto/utils/escape.py
+-rw-r--r--   0        0        0      783 2024-05-27 02:04:39.184285 asynch_lxneng-0.2.5/asynch/proto/utils/helpers.py
+-rw-r--r--   0        0        0     1196 2024-05-27 02:16:36.939313 asynch_lxneng-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     5496 1970-01-01 00:00:00.000000 asynch_lxneng-0.2.5/PKG-INFO
```

### Comparing `asynch_lxneng-0.2.4/CHANGELOG.md` & `asynch_lxneng-0.2.5/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # ChangeLog
 
 ## 0.2
 
+### 0.2.3
+
+- Support json column. (#73)
+- Fix connection with `secure=True` and `verify=False`.
+- Fix compression.
+- Fix exception `Cannot set verify_mode to CERT_NONE when check_hostname is enabled`.
+
 ### 0.2.2
 
 - Add `Int128Column`, `Int256Column`, `UInt128Column`, `UInt256Column`, `Decimal256Column`. (#57)
 - Add Geo type support. (#56)
 - Add decimals in map support. (#55)
 - Add `NestedColumn`. (#54)
 - Add execution_options support. (#53)
```

### Comparing `asynch_lxneng-0.2.4/LICENSE` & `asynch_lxneng-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/README.md` & `asynch_lxneng-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/connection.py` & `asynch_lxneng-0.2.5/asynch/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         self._host = host
         self._port = port
         self._database = database
         self._connection_kwargs = kwargs
         self._is_closed = False
         self._echo = echo
         self._cursor_cls = cursor_cls
-        self._connected = False
         if dsn:
             self._connection = ProtoConnection(
                 **self._parse_dsn(dsn), stack_track=stack_track, **kwargs
             )
         else:
             self._connection = ProtoConnection(
                 host=host,
@@ -50,15 +49,15 @@
             )
 
     def __repr__(self):
         return "<connection object at 0x{0:x}; closed: {1:}>".format(id(self), self._is_closed)
 
     @property
     def connected(self):
-        return self._connected
+        return self._connection.connected
 
     @property
     def host(self):
         return self._host
 
     @property
     def port(self):
@@ -89,18 +88,17 @@
     async def commit(self):
         raise errors.NotSupportedError
 
     async def rollback(self):
         raise errors.NotSupportedError
 
     async def connect(self):
-        if self._connected:
+        if self.connected:
             return
         await self._connection.connect()
-        self._connected = True
 
     def cursor(self, cursor: Type[Cursor] = None) -> Cursor:
         cursor_cls = cursor or self._cursor_cls
         return cursor_cls(self, self._echo)
 
     def _parse_dsn(self, url):
         """
```

### Comparing `asynch_lxneng-0.2.4/asynch/cursors.py` & `asynch_lxneng-0.2.5/asynch/cursors.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,19 +276,21 @@
 
     def _check_query_started(self):
         if self._state == self._states.NONE:
             raise ProgrammingError("no results to fetch")
 
     def _check_query_executing(self):
         if self._connection._connection.is_query_executing:
-            raise ProgrammingError("records have not fetched, fetch all before execute next")
+            raise ProgrammingError(
+                "some records have not been fetched. fetch the remaining records before executing the next query"
+            )
 
     def _check_cursor_closed(self):
         if self._state == self._states.CURSOR_CLOSED:
-            raise InterfaceError("cursor already closed")
+            raise InterfaceError("cursor is already closed")
 
     def _begin_query(self):
         self._state = self._states.RUNNING
 
     def _end_query(self):
         self._state = self._states.FINISHED
```

### Comparing `asynch_lxneng-0.2.4/asynch/errors.py` & `asynch_lxneng-0.2.5/asynch/errors.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/pool.py` & `asynch_lxneng-0.2.5/asynch/pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
             return fut
         self._used.remove(connection)
         if connection.connected:
             if self._closing:
                 await connection.close()
             else:
                 self._free.append(connection)
-            fut = self._loop.create_task(self._wakeup())
+        fut = self._loop.create_task(self._wakeup())
         return fut
 
     async def _wakeup(self):
         async with self._cond:
             self._cond.notify()
 
     def _wait(self):
@@ -171,30 +171,37 @@
         return _PoolAcquireContextManager(self._acquire(), self)
 
     async def _acquire(self) -> Connection:
         if self._closing:
             raise RuntimeError("Cannot acquire connection after closing pool")
         async with self._cond:
             while True:
-                await self.initialize()
+                await self.initialize()  # Restore minsize
+
+                if not self._free and self.size < self.maxsize:
+                    await self.init_one_connection()
+
                 if self._free:
                     conn = self._free.popleft()
                     if await self._check_conn(conn):
                         self._used.add(conn)
                         return conn
                     else:
                         continue
                 else:
                     await self._cond.wait()
 
     async def initialize(self):
-        while self.freesize < self.minsize and self.size < self.maxsize:
-            conn = await connect(**self._connection_kwargs)
-            self._free.append(conn)
-            self._cond.notify()
+        while self.freesize < self.minsize and self.size <= self.maxsize:
+            await self.init_one_connection()
+
+    async def init_one_connection(self):
+        conn = await connect(**self._connection_kwargs)
+        self._free.append(conn)
+        self._cond.notify()
 
     async def clear(self):
         """Close all free connections in pool."""
         async with self._cond:
             while self._free:
                 conn = self._free.popleft()
                 await conn.close()
```

### Comparing `asynch_lxneng-0.2.4/asynch/proto/block.py` & `asynch_lxneng-0.2.5/asynch/proto/block.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/columns/__init__.py` & `asynch_lxneng-0.2.5/asynch/proto/columns/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     StructPackException,
     TypeMismatchError,
     UnknownTypeError,
 )
 from ..streams.buffered import BufferedReader, BufferedWriter
 from .arraycolumn import create_array_column
 from .boolcolumn import BoolColumn
-from .datecolumn import DateColumn
+from .datecolumn import DateColumn, Date32Column
 from .datetimecolumn import create_datetime_column
 from .decimalcolumn import create_decimal_column
 from .enumcolumn import create_enum_column
 from .floatcolumn import Float32, Float64
 from .intcolumn import (
     Int8Column,
     Int16Column,
@@ -48,14 +48,15 @@
 from .tuplecolumn import create_tuple_column
 from .uuidcolumn import UUIDColumn
 
 column_by_type = {
     c.ch_type: c
     for c in [
         DateColumn,
+        Date32Column,
         Float32,
         Float64,
         BoolColumn,
         Int8Column,
         Int16Column,
         Int32Column,
         Int64Column,
```

### Comparing `asynch_lxneng-0.2.4/asynch/proto/columns/arraycolumn.py` & `asynch_lxneng-0.2.5/asynch/proto/columns/arraycolumn.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/columns/base.py` & `asynch_lxneng-0.2.5/asynch/proto/columns/base.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/columns/datetimecolumn.py` & `asynch_lxneng-0.2.5/asynch/proto/columns/datetimecolumn.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/columns/decimalcolumn.py` & `asynch_lxneng-0.2.5/asynch/proto/columns/decimalcolumn.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/columns/enumcolumn.py` & `asynch_lxneng-0.2.5/asynch/proto/columns/enumcolumn.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/columns/floatcolumn.py` & `asynch_lxneng-0.2.5/asynch/proto/columns/floatcolumn.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/columns/intcolumn.py` & `asynch_lxneng-0.2.5/asynch/proto/columns/intcolumn.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/columns/intervalcolumn.py` & `asynch_lxneng-0.2.5/asynch/proto/columns/intervalcolumn.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/columns/ipcolumn.py` & `asynch_lxneng-0.2.5/asynch/proto/columns/ipcolumn.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/columns/jsoncolumn.py` & `asynch_lxneng-0.2.5/asynch/proto/columns/jsoncolumn.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/columns/lowcardinalitycolumn.py` & `asynch_lxneng-0.2.5/asynch/proto/columns/lowcardinalitycolumn.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/columns/mapcolumn.py` & `asynch_lxneng-0.2.5/asynch/proto/columns/mapcolumn.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/columns/nestedcolumn.py` & `asynch_lxneng-0.2.5/asynch/proto/columns/nestedcolumn.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/columns/stringcolumn.py` & `asynch_lxneng-0.2.5/asynch/proto/columns/stringcolumn.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/columns/tuplecolumn.py` & `asynch_lxneng-0.2.5/asynch/proto/columns/tuplecolumn.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/columns/util.py` & `asynch_lxneng-0.2.5/asynch/proto/columns/util.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/columns/uuidcolumn.py` & `asynch_lxneng-0.2.5/asynch/proto/columns/uuidcolumn.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/compression/__init__.py` & `asynch_lxneng-0.2.5/asynch/proto/compression/__init__.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/compression/lz4.py` & `asynch_lxneng-0.2.5/asynch/proto/compression/lz4.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/compression/zstd.py` & `asynch_lxneng-0.2.5/asynch/proto/compression/zstd.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/connection.py` & `asynch_lxneng-0.2.5/asynch/proto/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,21 +9,30 @@
 from asynch.errors import (
     PartiallyConsumedQueryError,
     ServerException,
     UnexpectedPacketFromServerError,
     UnknownPacketFromServerError,
 )
 from asynch.proto import constants
-from asynch.proto.block import BlockStreamProfileInfo, ColumnOrientedBlock, RowOrientedBlock
+from asynch.proto.block import (
+    BlockStreamProfileInfo,
+    ColumnOrientedBlock,
+    RowOrientedBlock,
+)
 from asynch.proto.compression import get_compressor_cls
 from asynch.proto.context import Context, ExecuteContext
 from asynch.proto.cs import ClientInfo, QueryKind, ServerInfo
 from asynch.proto.progress import Progress
 from asynch.proto.protocol import ClientPacket, Compression, ServerPacket
-from asynch.proto.result import IterQueryResult, ProgressQueryResult, QueryInfo, QueryResult
+from asynch.proto.result import (
+    IterQueryResult,
+    ProgressQueryResult,
+    QueryInfo,
+    QueryResult,
+)
 from asynch.proto.settings import write_settings
 from asynch.proto.streams.block import BlockReader, BlockWriter
 from asynch.proto.streams.buffered import BufferedReader, BufferedWriter
 from asynch.proto.utils.escape import escape_params
 from asynch.proto.utils.helpers import chunks, column_chunks
 
 logger = logging.getLogger(__name__)
@@ -471,15 +480,14 @@
 
             if packet is True:
                 continue
 
             yield packet
 
     async def receive_result(self, with_column_types=False, progress=False, columnar=False):
-
         generator = self.packet_generator()
 
         if progress:
             return ProgressQueryResult(
                 self.reader, generator, with_column_types=with_column_types, columnar=columnar
             )
 
@@ -538,15 +546,14 @@
         self.block_writer = self.get_block_writer()
 
         self.connected = True
         await self.send_hello()
         await self.receive_hello()
 
     def reset_state(self):
-
         self.writer = None
         self.reader = None
         self.block_reader = None
         self.block_reader_raw = None
         self.block_writer = None
         self.connected = False
 
@@ -620,15 +627,14 @@
                       rows/columns.
                     * The second element information is about columns: names
                       and types.
         """
 
         start_time = time()
         async with ExecuteContext(self, query, settings):
-
             # INSERT queries can use list/tuple/generator of list/tuples/dicts.
             # For SELECT parameters can be passed in only in dict right now.
             is_insert = isinstance(args, (list, tuple, GeneratorType))
 
             if is_insert:
                 rv = await self.process_insert_query(
                     query,
@@ -705,15 +711,14 @@
         params=None,
         with_column_types=False,
         external_tables=None,
         query_id=None,
         types_check=False,
         columnar=False,
     ):
-
         if params is not None:
             query = self.substitute_params(query, params)
 
         await self.send_query(query, query_id=query_id)
         await self.send_external_tables(external_tables, types_check=types_check)
         return self.receive_result(
             with_column_types=with_column_types, progress=True, columnar=columnar
@@ -758,15 +763,14 @@
         params=None,
         with_column_types=False,
         external_tables=None,
         query_id="",
         types_check=False,
         columnar=False,
     ):
-
         if params is not None:
             query = self.substitute_params(query, params)
 
         await self.send_query(query, query_id=query_id)
         await self.send_external_tables(external_tables, types_check=types_check)
         return await self.receive_result(with_column_types=with_column_types, columnar=columnar)
 
@@ -866,15 +870,14 @@
         query,
         params=None,
         with_column_types=False,
         external_tables=None,
         query_id=None,
         types_check=False,
     ):
-
         if params is not None:
             query = self.substitute_params(query, params)
 
         await self.send_query(query, query_id=query_id)
         await self.send_external_tables(external_tables, types_check=types_check)
         return self.iter_receive_result(with_column_types=with_column_types)
```

### Comparing `asynch_lxneng-0.2.4/asynch/proto/constants.py` & `asynch_lxneng-0.2.5/asynch/proto/constants.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/context.py` & `asynch_lxneng-0.2.5/asynch/proto/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,16 +42,20 @@
     def __init__(self, connection: "Connection", query, settings):
         self._query = query
         self._settings = settings
         self._connection = connection
         self._connection.make_query_settings(settings)
 
     async def __aenter__(self):
-        await self._connection.force_connect()
-        self._connection.last_query = QueryInfo(self._connection.reader)
+        try:
+            await self._connection.force_connect()
+            self._connection.last_query = QueryInfo(self._connection.reader)
+        except (Exception, KeyboardInterrupt):
+            await self._connection.disconnect()
+            raise
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         if exc_type:
             if issubclass(exc_type, (Exception, KeyboardInterrupt)):
                 await self._connection.disconnect()
                 raise exc_val
         self._connection.track_current_database(self._query)
```

### Comparing `asynch_lxneng-0.2.4/asynch/proto/cs.py` & `asynch_lxneng-0.2.5/asynch/proto/cs.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/opentelemetry.py` & `asynch_lxneng-0.2.5/asynch/proto/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/progress.py` & `asynch_lxneng-0.2.5/asynch/proto/progress.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/protocol.py` & `asynch_lxneng-0.2.5/asynch/proto/protocol.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/result.py` & `asynch_lxneng-0.2.5/asynch/proto/result.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/settings/__init__.py` & `asynch_lxneng-0.2.5/asynch/proto/settings/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 logger = logging.getLogger(__name__)
 
 
 async def write_settings(
     writer: BufferedWriter, settings: Dict, settings_as_strings, settings_is_important: bool
 ):
-
     for setting, value in (settings or {}).items():
         # If the server support settings as string we do not need to know
         # anything about them, so we can write any setting.
         if settings_as_strings:
             await writer.write_str(setting)
             await writer.write_uint8(int(settings_is_important))
             await writer.write_str(str(value))
```

### Comparing `asynch_lxneng-0.2.4/asynch/proto/settings/available.py` & `asynch_lxneng-0.2.5/asynch/proto/settings/available.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/settings/types.py` & `asynch_lxneng-0.2.5/asynch/proto/settings/types.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/streams/block.py` & `asynch_lxneng-0.2.5/asynch/proto/streams/block.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/streams/buffered.py` & `asynch_lxneng-0.2.5/asynch/proto/streams/buffered.py`

 * *Files 9% similar despite different names*

```diff
@@ -107,116 +107,105 @@
     def __init__(self, reader: StreamReader, buffer_max_size: int = constants.BUFFER_SIZE):
         self.buffer_max_size = buffer_max_size
         self.reader = reader
         self.buffer = bytearray()
         self.current_buffer_size = 0
         self.position = 0
 
+    async def _refill_buffer(self):
+        if self.position == self.current_buffer_size:
+            self._reset_buffer()
+            await self._read_into_buffer()
+
+    def _is_buffer_empty(self):
+        return not (self.buffer or self.position)
+
+    async def _is_buffer_readable(self) -> bool:
+        await self._refill_buffer()
+        if self._is_buffer_empty():
+            return False
+        return True
+
+    def _reset_buffer(self):
+        self.position = 0
+        self.buffer = bytearray()
+
     async def _read_into_buffer(self):
         packet = await self.reader.read(self.buffer_max_size)
         self.buffer.extend(packet)
         self.current_buffer_size = len(self.buffer)
 
     def _read_one(self):
         packet = self.buffer[self.position]
         self.position += 1
         return packet
 
     async def read_varint(self):
-        if self.position == self.current_buffer_size:
-            self._reset_buffer()
-            await self._read_into_buffer()
         packets = bytearray()
         while True:
+            if not (await self._is_buffer_readable()):
+                break
             packet = self._read_one()
             packets.append(packet)
             if packet < 0x80:
                 break
         return leb128.u.decode(packets)
 
-    def _reset_buffer(self):
-        self.position = 0
-        self.buffer = bytearray()
-
-    async def read_str(self, as_bytes: bool = False):
-        length = await self.read_varint()
-        packet = await self.read_bytes(length)
-        if as_bytes:
-            return packet
-        return packet.decode()
-
-    async def read_fixed_str(self, length: int, as_bytes: bool = False):
-        packet = await self.read_bytes(length)
-        if as_bytes:
-            return packet
-        return packet.decode()
-
     async def read_bytes(self, length: int):
         packets = bytearray()
         while length > 0:
-            if self.position == self.current_buffer_size:
-                self._reset_buffer()
-                await self._read_into_buffer()
-
+            if not (await self._is_buffer_readable()):
+                break
             read_position = self.position + length
             packet = self.buffer[self.position : read_position]  # noqa: E203
             length -= len(packet)
             self.position += len(packet)
             packets.extend(packet)
-
         return packets
 
+    async def read_fixed_str(self, length: int, as_bytes: bool = False):
+        packet = await self.read_bytes(length)
+        if as_bytes:
+            return packet
+        return packet.decode()
+
+    async def read_str(self, as_bytes: bool = False):
+        length = await self.read_varint()
+        return await self.read_fixed_str(length=length, as_bytes=as_bytes)
+
     async def read_int(self, fmt: str):
         s = struct.Struct("<" + fmt)
         packet = await self.read_bytes(s.size)
         return s.unpack(packet)[0]
 
-    async def read_int8(
-        self,
-    ):
+    async def read_int8(self):
         return await self.read_int("b")
 
-    async def read_int16(
-        self,
-    ):
+    async def read_int16(self):
         return await self.read_int("h")
 
-    async def read_int32(
-        self,
-    ):
+    async def read_int32(self):
         return await self.read_int("i")
 
-    async def read_int64(
-        self,
-    ):
+    async def read_int64(self):
         return await self.read_int("q")
 
-    async def read_uint8(
-        self,
-    ):
+    async def read_uint8(self):
         return await self.read_int("B")
 
-    async def read_uint16(
-        self,
-    ):
+    async def read_uint16(self):
         return await self.read_int("H")
 
-    async def read_uint32(
-        self,
-    ):
+    async def read_uint32(self):
         return await self.read_int("I")
 
-    async def read_uint64(
-        self,
-    ):
+    async def read_uint64(self):
         return await self.read_int("Q")
 
-    async def read_uint128(
-        self,
-    ):
+    async def read_uint128(self):
         hi = await self.read_int("Q")
         lo = await self.read_int("Q")
         return (hi << 64) + lo
 
 
 class CompressedBufferedWriter(BufferedWriter):
     def __init__(
```

### Comparing `asynch_lxneng-0.2.4/asynch/proto/streams/compressed.py` & `asynch_lxneng-0.2.5/asynch/proto/streams/compressed.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/utils/compat.py` & `asynch_lxneng-0.2.5/asynch/proto/utils/compat.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/utils/escape.py` & `asynch_lxneng-0.2.5/asynch/proto/utils/escape.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/asynch/proto/utils/helpers.py` & `asynch_lxneng-0.2.5/asynch/proto/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `asynch_lxneng-0.2.4/pyproject.toml` & `asynch_lxneng-0.2.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asynch-lxneng"
-version = "0.2.4"
+version = "0.2.5"
 description = "A asyncio driver for ClickHouse with native tcp protocol"
 authors = ["long2ice <long2ice@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/long2ice/asynch"
 repository = "https://github.com/long2ice/asynch.git"
 documentation = "https://github.com/long2ice/asynch"
@@ -24,32 +24,33 @@
 tzlocal = "*"
 ciso8601 = "*"
 
 [tool.poetry.extras]
 compression = ["clickhouse-cityhash"]
 
 [tool.poetry.dev-dependencies]
-flake8 = "*"
-pyproject-flake8 = "*"
+ruff = "*"
 isort = "*"
 black = "*"
 pytest = "*"
 pytest-mock = "*"
 bandit = "*"
 pytest-asyncio = "*"
 clickhouse-driver = "*"
 uvloop = "*"
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core"]
+
+[tool.isort]
+profile = "black"
 
 [tool.black]
 line-length = 100
-target-version = ["py36", "py37", "py38", "py39"]
-
-[tool.flake8]
-ignore = "E501,W503,DAR101,DAR201,DAR402"
-max-line-length = 100
+target-version = ['py38', 'py39', 'py310', 'py311']
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
+
+[tool.ruff]
+line-length = 100
```

### Comparing `asynch_lxneng-0.2.4/setup.py` & `asynch_lxneng-0.2.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,198 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: asynch-lxneng
+Version: 0.2.5
+Summary: A asyncio driver for ClickHouse with native tcp protocol
+Home-page: https://github.com/long2ice/asynch
+License: Apache-2.0
+Keywords: ClickHouse,asyncio,driver
+Author: long2ice
+Author-email: long2ice@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: compression
+Requires-Dist: ciso8601
+Requires-Dist: clickhouse-cityhash ; extra == "compression"
+Requires-Dist: leb128
+Requires-Dist: lz4
+Requires-Dist: pytz
+Requires-Dist: tzlocal
+Requires-Dist: zstd
+Project-URL: Documentation, https://github.com/long2ice/asynch
+Project-URL: Repository, https://github.com/long2ice/asynch.git
+Description-Content-Type: text/markdown
+
+# asynch
+
+![pypi](https://img.shields.io/pypi/v/asynch.svg?style=flat)
+![license](https://img.shields.io/github/license/long2ice/asynch)
+![workflows](https://github.com/long2ice/asynch/workflows/pypi/badge.svg)
+![workflows](https://github.com/long2ice/asynch/workflows/ci/badge.svg)
+
+## Introduction
+
+`asynch` is an asyncio ClickHouse Python Driver with native (TCP) interface support, which reuse most of [clickhouse-driver](https://github.com/mymarilyn/clickhouse-driver) and comply with [PEP249](https://www.python.org/dev/peps/pep-0249/).
+
+## Install
+
+```shell
+> pip install asynch
+```
+
+or if you want to install [`clickhouse-cityhash`](https://pypi.org/project/clickhouse-cityhash/) to enable
+transport compression
+
+```shell
+> pip install asynch[compression]
+```
+
+## Usage
+
+Connect to ClickHouse
+
+```python
+from asynch import connect
+
+async def connect_database():
+    conn = await connect(
+        host = "127.0.0.1",
+        port = 9000,
+        database = "default",
+        user = "default",
+        password = "",
+    )
+```
+
+Create table by sql
+
+```python
+async def create_table():
+    async with conn.cursor(cursor=DictCursor) as cursor:
+        await cursor.execute('create database if not exists test')
+        await cursor.execute("""
+        CREATE TABLE if not exists test.asynch
+            (
+                `id`       Int32,
+                `decimal`  Decimal(10, 2),
+                `date`     Date,
+                `datetime` DateTime,
+                `float`    Float32,
+                `uuid`     UUID,
+                `string`   String,
+                `ipv4`     IPv4,
+                `ipv6`     IPv6
+
+            )
+            ENGINE = MergeTree
+                ORDER BY id"""
+        )
+```
+
+Use `fetchone`
+
+```python
+async def fetchone():
+    async with conn.cursor() as cursor:
+        await cursor.execute("SELECT 1")
+        ret = await cursor.fetchone()
+        assert ret == (1,)
+```
+
+Use `fetchmany`
+
+```python
+async def fetchall():
+    async with conn.cursor() as cursor:
+        await cursor.execute("SELECT 1")
+        ret = await cursor.fetchall()
+        assert ret == [(1,)]
+```
+
+Use `DictCursor` to get result with dict
+
+```python
+async def dict_cursor():
+    async with conn.cursor(cursor=DictCursor) as cursor:
+        await cursor.execute("SELECT 1")
+        ret = await cursor.fetchall()
+        assert ret == [{"1": 1}]
+```
+
+Insert data with dict
+
+```python
+from asynch.cursors import DictCursor
+
+async def insert_dict():
+    async with conn.cursor(cursor=DictCursor) as cursor:
+        ret = await cursor.execute(
+            """INSERT INTO test.asynch(id,decimal,date,datetime,float,uuid,string,ipv4,ipv6) VALUES""",
+            [
+                {
+                    "id": 1,
+                    "decimal": 1,
+                    "date": "2020-08-08",
+                    "datetime": "2020-08-08 00:00:00",
+                    "float": 1,
+                    "uuid": "59e182c4-545d-4f30-8b32-cefea2d0d5ba",
+                    "string": "1",
+                    "ipv4": "0.0.0.0",
+                    "ipv6": "::",
+                }
+            ],
+        )
+        assert ret == 1
+```
+
+Insert data with tuple
+
+```python
+async def insert_tuple():
+    async with conn.cursor(cursor=DictCursor) as cursor:
+        ret = await cursor.execute(
+            """INSERT INTO test.asynch(id,decimal,date,datetime,float,uuid,string,ipv4,ipv6) VALUES""",
+            [
+                (
+                    1,
+                    1,
+                    "2020-08-08",
+                    "2020-08-08 00:00:00",
+                    1,
+                    "59e182c4-545d-4f30-8b32-cefea2d0d5ba",
+                    "1",
+                    "0.0.0.0",
+                    "::",
+                )
+            ],
+        )
+        assert ret == 1
+```
+
+Use connection pool
+
+```python
+async def use_pool():
+    pool = await asynch.create_pool()
+    async with pool.acquire() as conn:
+        async with conn.cursor() as cursor:
+            await cursor.execute("SELECT 1")
+            ret = await cursor.fetchone()
+            assert ret == (1,)
+    pool.close()
+    await pool.wait_closed()
+```
 
-packages = \
-['asynch',
- 'asynch.proto',
- 'asynch.proto.columns',
- 'asynch.proto.compression',
- 'asynch.proto.settings',
- 'asynch.proto.streams',
- 'asynch.proto.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['ciso8601', 'leb128', 'lz4', 'pytz', 'tzlocal', 'zstd']
-
-extras_require = \
-{'compression': ['clickhouse-cityhash']}
-
-setup_kwargs = {
-    'name': 'asynch-lxneng',
-    'version': '0.2.4',
-    'description': 'A asyncio driver for ClickHouse with native tcp protocol',
-    'long_description': '# asynch\n\n![pypi](https://img.shields.io/pypi/v/asynch.svg?style=flat)\n![license](https://img.shields.io/github/license/long2ice/asynch)\n![workflows](https://github.com/long2ice/asynch/workflows/pypi/badge.svg)\n![workflows](https://github.com/long2ice/asynch/workflows/ci/badge.svg)\n\n## Introduction\n\n`asynch` is an asyncio ClickHouse Python Driver with native (TCP) interface support, which reuse most of [clickhouse-driver](https://github.com/mymarilyn/clickhouse-driver) and comply with [PEP249](https://www.python.org/dev/peps/pep-0249/).\n\n## Install\n\n```shell\n> pip install asynch\n```\n\nor if you want to install [`clickhouse-cityhash`](https://pypi.org/project/clickhouse-cityhash/) to enable\ntransport compression\n\n```shell\n> pip install asynch[compression]\n```\n\n## Usage\n\nConnect to ClickHouse\n\n```python\nfrom asynch import connect\n\nasync def connect_database():\n    conn = await connect(\n        host = "127.0.0.1",\n        port = 9000,\n        database = "default",\n        user = "default",\n        password = "",\n    )\n```\n\nCreate table by sql\n\n```python\nasync def create_table():\n    async with conn.cursor(cursor=DictCursor) as cursor:\n        await cursor.execute(\'create database if not exists test\')\n        await cursor.execute("""\n        CREATE TABLE if not exists test.asynch\n            (\n                `id`       Int32,\n                `decimal`  Decimal(10, 2),\n                `date`     Date,\n                `datetime` DateTime,\n                `float`    Float32,\n                `uuid`     UUID,\n                `string`   String,\n                `ipv4`     IPv4,\n                `ipv6`     IPv6\n\n            )\n            ENGINE = MergeTree\n                ORDER BY id"""\n        )\n```\n\nUse `fetchone`\n\n```python\nasync def fetchone():\n    async with conn.cursor() as cursor:\n        await cursor.execute("SELECT 1")\n        ret = await cursor.fetchone()\n        assert ret == (1,)\n```\n\nUse `fetchmany`\n\n```python\nasync def fetchall():\n    async with conn.cursor() as cursor:\n        await cursor.execute("SELECT 1")\n        ret = await cursor.fetchall()\n        assert ret == [(1,)]\n```\n\nUse `DictCursor` to get result with dict\n\n```python\nasync def dict_cursor():\n    async with conn.cursor(cursor=DictCursor) as cursor:\n        await cursor.execute("SELECT 1")\n        ret = await cursor.fetchall()\n        assert ret == [{"1": 1}]\n```\n\nInsert data with dict\n\n```python\nfrom asynch.cursors import DictCursor\n\nasync def insert_dict():\n    async with conn.cursor(cursor=DictCursor) as cursor:\n        ret = await cursor.execute(\n            """INSERT INTO test.asynch(id,decimal,date,datetime,float,uuid,string,ipv4,ipv6) VALUES""",\n            [\n                {\n                    "id": 1,\n                    "decimal": 1,\n                    "date": "2020-08-08",\n                    "datetime": "2020-08-08 00:00:00",\n                    "float": 1,\n                    "uuid": "59e182c4-545d-4f30-8b32-cefea2d0d5ba",\n                    "string": "1",\n                    "ipv4": "0.0.0.0",\n                    "ipv6": "::",\n                }\n            ],\n        )\n        assert ret == 1\n```\n\nInsert data with tuple\n\n```python\nasync def insert_tuple():\n    async with conn.cursor(cursor=DictCursor) as cursor:\n        ret = await cursor.execute(\n            """INSERT INTO test.asynch(id,decimal,date,datetime,float,uuid,string,ipv4,ipv6) VALUES""",\n            [\n                (\n                    1,\n                    1,\n                    "2020-08-08",\n                    "2020-08-08 00:00:00",\n                    1,\n                    "59e182c4-545d-4f30-8b32-cefea2d0d5ba",\n                    "1",\n                    "0.0.0.0",\n                    "::",\n                )\n            ],\n        )\n        assert ret == 1\n```\n\nUse connection pool\n\n```python\nasync def use_pool():\n    pool = await asynch.create_pool()\n    async with pool.acquire() as conn:\n        async with conn.cursor() as cursor:\n            await cursor.execute("SELECT 1")\n            ret = await cursor.fetchone()\n            assert ret == (1,)\n    pool.close()\n    await pool.wait_closed()\n```\n\n## ThanksTo\n\n- [clickhouse-driver](https://github.com/mymarilyn/clickhouse-driver), ClickHouse Python Driver with native interface support.\n\n## License\n\nThis project is licensed under the [Apache-2.0](https://github.com/long2ice/asynch/blob/master/LICENSE) License.\n',
-    'author': 'long2ice',
-    'author_email': 'long2ice@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/long2ice/asynch',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+## ThanksTo
 
+- [clickhouse-driver](https://github.com/mymarilyn/clickhouse-driver), ClickHouse Python Driver with native interface support.
+
+## License
+
+This project is licensed under the [Apache-2.0](https://github.com/long2ice/asynch/blob/master/LICENSE) License.
 
-setup(**setup_kwargs)
```

