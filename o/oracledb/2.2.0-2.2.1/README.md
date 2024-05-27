# Comparing `tmp/oracledb-2.2.0.tar.gz` & `tmp/oracledb-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oracledb-2.2.0.tar", last modified: Wed May  1 21:01:45 2024, max compression
+gzip compressed data, was "oracledb-2.2.1.tar", last modified: Mon May 27 19:14:18 2024, max compression
```

## Comparing `oracledb-2.2.0.tar` & `oracledb-2.2.1.tar`

### file list

```diff
@@ -1,213 +1,213 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 21:01:45.285390 oracledb-2.2.0/
--rw-rw-r--   0 root         (0) root         (0)    12570 2024-03-08 04:11:12.000000 oracledb-2.2.0/LICENSE.txt
--rw-rw-r--   0 root         (0) root         (0)      398 2023-05-22 21:44:58.000000 oracledb-2.2.0/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)       56 2024-03-08 04:11:12.000000 oracledb-2.2.0/NOTICE.txt
--rw-r--r--   0 root         (0) root         (0)     5208 2024-05-01 21:01:45.285390 oracledb-2.2.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3730 2024-03-08 04:11:12.000000 oracledb-2.2.0/README.md
--rw-rw-r--   0 root         (0) root         (0)      166 2023-12-16 03:36:53.000000 oracledb-2.2.0/README.txt
--rw-rw-r--   0 root         (0) root         (0)    28103 2023-12-16 03:36:53.000000 oracledb-2.2.0/THIRD_PARTY_LICENSES.txt
--rw-rw-r--   0 root         (0) root         (0)      310 2024-03-08 04:11:12.000000 oracledb-2.2.0/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)     1608 2024-05-01 21:01:45.285390 oracledb-2.2.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     3878 2023-12-16 03:36:53.000000 oracledb-2.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 21:01:45.256390 oracledb-2.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 21:01:45.262390 oracledb-2.2.0/src/oracledb/
--rw-rw-r--   0 root         (0) root         (0)    11213 2024-04-11 20:42:10.000000 oracledb-2.2.0/src/oracledb/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    19011 2023-12-16 03:36:53.000000 oracledb-2.2.0/src/oracledb/aq.py
--rw-rw-r--   0 root         (0) root         (0)    25835 2024-04-30 01:35:34.000000 oracledb-2.2.0/src/oracledb/base_impl.pxd
--rw-rw-r--   0 root         (0) root         (0)     3711 2024-04-18 22:46:32.000000 oracledb-2.2.0/src/oracledb/base_impl.pyx
--rw-rw-r--   0 root         (0) root         (0)    36682 2024-04-19 20:52:43.000000 oracledb-2.2.0/src/oracledb/connect_params.py
--rw-rw-r--   0 root         (0) root         (0)    75308 2024-04-19 23:14:55.000000 oracledb-2.2.0/src/oracledb/connection.py
--rw-rw-r--   0 root         (0) root         (0)     4144 2024-03-27 19:56:13.000000 oracledb-2.2.0/src/oracledb/constants.py
--rw-rw-r--   0 root         (0) root         (0)     2909 2023-12-16 03:36:53.000000 oracledb-2.2.0/src/oracledb/constructors.py
--rw-rw-r--   0 root         (0) root         (0)    44011 2024-04-19 23:14:55.000000 oracledb-2.2.0/src/oracledb/cursor.py
--rw-rw-r--   0 root         (0) root         (0)    11862 2024-04-11 20:42:10.000000 oracledb-2.2.0/src/oracledb/dbobject.py
--rw-rw-r--   0 root         (0) root         (0)     3492 2024-03-08 04:11:12.000000 oracledb-2.2.0/src/oracledb/defaults.py
--rw-rw-r--   0 root         (0) root         (0)     5483 2023-12-16 03:36:53.000000 oracledb-2.2.0/src/oracledb/driver_mode.py
--rw-rw-r--   0 root         (0) root         (0)     3160 2023-12-16 03:36:53.000000 oracledb-2.2.0/src/oracledb/dsn.py
--rw-rw-r--   0 root         (0) root         (0)    28552 2024-04-26 22:27:56.000000 oracledb-2.2.0/src/oracledb/errors.py
--rw-rw-r--   0 root         (0) root         (0)     1812 2023-12-16 03:36:53.000000 oracledb-2.2.0/src/oracledb/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)     7448 2024-03-25 23:37:27.000000 oracledb-2.2.0/src/oracledb/fetch_info.py
--rw-rw-r--   0 root         (0) root         (0)     1717 2023-12-16 03:36:53.000000 oracledb-2.2.0/src/oracledb/future.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 21:01:45.256390 oracledb-2.2.0/src/oracledb/impl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 21:01:45.265390 oracledb-2.2.0/src/oracledb/impl/base/
--rw-rw-r--   0 root         (0) root         (0)     7341 2024-03-15 22:01:45.000000 oracledb-2.2.0/src/oracledb/impl/base/bind_var.pyx
--rw-rw-r--   0 root         (0) root         (0)    47832 2024-04-30 01:35:34.000000 oracledb-2.2.0/src/oracledb/impl/base/buffer.pyx
--rw-rw-r--   0 root         (0) root         (0)    45302 2024-04-26 22:01:15.000000 oracledb-2.2.0/src/oracledb/impl/base/connect_params.pyx
--rw-rw-r--   0 root         (0) root         (0)    14208 2024-04-26 22:01:15.000000 oracledb-2.2.0/src/oracledb/impl/base/connection.pyx
--rw-rw-r--   0 root         (0) root         (0)     3399 2024-04-26 22:01:15.000000 oracledb-2.2.0/src/oracledb/impl/base/constants.pxi
--rw-rw-r--   0 root         (0) root         (0)    25501 2024-03-25 23:37:27.000000 oracledb-2.2.0/src/oracledb/impl/base/cursor.pyx
--rw-rw-r--   0 root         (0) root         (0)     7066 2024-04-19 23:14:55.000000 oracledb-2.2.0/src/oracledb/impl/base/dbobject.pyx
--rw-rw-r--   0 root         (0) root         (0)     1702 2024-03-08 04:11:12.000000 oracledb-2.2.0/src/oracledb/impl/base/defaults.pyx
--rw-rw-r--   0 root         (0) root         (0)     2741 2023-05-22 21:44:58.000000 oracledb-2.2.0/src/oracledb/impl/base/lob.pyx
--rw-rw-r--   0 root         (0) root         (0)    33590 2024-03-27 15:27:43.000000 oracledb-2.2.0/src/oracledb/impl/base/oson.pyx
--rw-rw-r--   0 root         (0) root         (0)     4215 2023-05-22 21:44:58.000000 oracledb-2.2.0/src/oracledb/impl/base/pool.pyx
--rw-rw-r--   0 root         (0) root         (0)     4288 2024-03-08 04:11:12.000000 oracledb-2.2.0/src/oracledb/impl/base/pool_params.pyx
--rw-rw-r--   0 root         (0) root         (0)     6379 2023-05-22 21:44:58.000000 oracledb-2.2.0/src/oracledb/impl/base/queue.pyx
--rw-rw-r--   0 root         (0) root         (0)     4799 2024-03-25 23:37:27.000000 oracledb-2.2.0/src/oracledb/impl/base/soda.pyx
--rw-rw-r--   0 root         (0) root         (0)     1933 2023-05-22 21:44:58.000000 oracledb-2.2.0/src/oracledb/impl/base/subscr.pyx
--rw-rw-r--   0 root         (0) root         (0)    10416 2024-04-11 20:42:10.000000 oracledb-2.2.0/src/oracledb/impl/base/types.pyx
--rw-rw-r--   0 root         (0) root         (0)     7891 2024-04-18 22:46:32.000000 oracledb-2.2.0/src/oracledb/impl/base/utils.pyx
--rw-rw-r--   0 root         (0) root         (0)    11753 2024-04-19 23:14:55.000000 oracledb-2.2.0/src/oracledb/impl/base/var.pyx
--rw-rw-r--   0 root         (0) root         (0)     5714 2024-04-26 22:01:15.000000 oracledb-2.2.0/src/oracledb/impl/base/vector.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 21:01:45.267390 oracledb-2.2.0/src/oracledb/impl/thick/
--rw-rw-r--   0 root         (0) root         (0)     2264 2024-03-25 23:37:27.000000 oracledb-2.2.0/src/oracledb/impl/thick/buffer.pyx
--rw-rw-r--   0 root         (0) root         (0)    32798 2024-04-19 23:14:55.000000 oracledb-2.2.0/src/oracledb/impl/thick/connection.pyx
--rw-rw-r--   0 root         (0) root         (0)    21322 2024-04-19 23:14:55.000000 oracledb-2.2.0/src/oracledb/impl/thick/cursor.pyx
--rw-rw-r--   0 root         (0) root         (0)    14836 2024-04-19 23:14:55.000000 oracledb-2.2.0/src/oracledb/impl/thick/dbobject.pyx
--rw-rw-r--   0 root         (0) root         (0)     9894 2024-03-25 23:37:27.000000 oracledb-2.2.0/src/oracledb/impl/thick/json.pyx
--rw-rw-r--   0 root         (0) root         (0)     7534 2024-04-19 23:14:55.000000 oracledb-2.2.0/src/oracledb/impl/thick/lob.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 21:01:45.256390 oracledb-2.2.0/src/oracledb/impl/thick/odpi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 21:01:45.267390 oracledb-2.2.0/src/oracledb/impl/thick/odpi/embed/
--rw-rw-r--   0 root         (0) root         (0)     2633 2024-03-08 04:11:18.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/embed/dpi.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 21:01:45.267390 oracledb-2.2.0/src/oracledb/impl/thick/odpi/include/
--rw-rw-r--   0 root         (0) root         (0)    86869 2024-03-08 04:11:18.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/include/dpi.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 21:01:45.273390 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/
--rw-rw-r--   0 root         (0) root         (0)   117539 2024-03-08 04:11:18.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiConn.c
--rw-rw-r--   0 root         (0) root         (0)    16874 2024-03-08 04:11:18.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiContext.c
--rw-rw-r--   0 root         (0) root         (0)    34806 2024-01-08 23:59:29.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiData.c
--rw-rw-r--   0 root         (0) root         (0)     7443 2024-01-08 23:59:29.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiDebug.c
--rw-rw-r--   0 root         (0) root         (0)    15574 2024-01-08 23:59:29.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiDeqOptions.c
--rw-rw-r--   0 root         (0) root         (0)     7552 2024-01-08 23:59:29.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiEnqOptions.c
--rw-rw-r--   0 root         (0) root         (0)     9569 2024-01-08 23:59:29.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiEnv.c
--rw-rw-r--   0 root         (0) root         (0)    14038 2024-03-08 04:11:18.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiError.c
--rw-rw-r--   0 root         (0) root         (0)     9348 2024-03-08 04:11:18.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiErrorMessages.h
--rw-rw-r--   0 root         (0) root         (0)    13273 2024-03-08 04:11:18.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiGen.c
--rw-rw-r--   0 root         (0) root         (0)    15039 2024-01-08 23:59:29.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiGlobal.c
--rw-rw-r--   0 root         (0) root         (0)     5184 2024-01-08 23:59:29.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiHandleList.c
--rw-rw-r--   0 root         (0) root         (0)     5399 2024-01-08 23:59:29.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiHandlePool.c
--rw-rw-r--   0 root         (0) root         (0)   111354 2024-03-08 04:11:18.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiImpl.h
--rw-rw-r--   0 root         (0) root         (0)    37212 2024-03-08 04:11:18.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiJson.c
--rw-rw-r--   0 root         (0) root         (0)    19868 2024-03-08 04:11:18.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiLob.c
--rw-rw-r--   0 root         (0) root         (0)    23232 2024-01-08 23:59:29.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiMsgProps.c
--rw-rw-r--   0 root         (0) root         (0)    40061 2024-03-25 22:46:55.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiObject.c
--rw-rw-r--   0 root         (0) root         (0)     5372 2024-03-08 04:11:18.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiObjectAttr.c
--rw-rw-r--   0 root         (0) root         (0)    15195 2024-03-08 04:11:18.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiObjectType.c
--rw-rw-r--   0 root         (0) root         (0)   182440 2024-03-08 04:11:18.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiOci.c
--rw-rw-r--   0 root         (0) root         (0)    32160 2024-03-08 04:11:18.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiOracleType.c
--rw-rw-r--   0 root         (0) root         (0)    32638 2024-01-08 23:59:29.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiPool.c
--rw-rw-r--   0 root         (0) root         (0)    23704 2024-03-08 04:11:18.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiQueue.c
--rw-rw-r--   0 root         (0) root         (0)     5712 2024-01-08 23:59:29.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiRowid.c
--rw-rw-r--   0 root         (0) root         (0)    42311 2024-03-08 04:11:18.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiSodaColl.c
--rw-rw-r--   0 root         (0) root         (0)     6131 2024-01-08 23:59:29.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiSodaCollCursor.c
--rw-rw-r--   0 root         (0) root         (0)    16800 2024-03-08 04:11:18.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiSodaDb.c
--rw-rw-r--   0 root         (0) root         (0)    12671 2024-03-08 04:11:18.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiSodaDoc.c
--rw-rw-r--   0 root         (0) root         (0)     6134 2024-01-08 23:59:29.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiSodaDocCursor.c
--rw-rw-r--   0 root         (0) root         (0)    79506 2024-03-08 04:11:18.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiStmt.c
--rw-rw-r--   0 root         (0) root         (0)     4221 2024-03-08 04:11:18.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiStringList.c
--rw-rw-r--   0 root         (0) root         (0)    29091 2024-01-08 23:59:29.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiSubscr.c
--rw-rw-r--   0 root         (0) root         (0)    23589 2024-01-08 23:59:29.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiUtils.c
--rw-rw-r--   0 root         (0) root         (0)    81960 2024-03-08 04:11:18.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiVar.c
--rw-rw-r--   0 root         (0) root         (0)     7710 2024-03-08 04:11:18.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiVector.c
--rw-rw-r--   0 root         (0) root         (0)    41686 2024-03-25 23:37:27.000000 oracledb-2.2.0/src/oracledb/impl/thick/odpi.pxd
--rw-rw-r--   0 root         (0) root         (0)    13993 2024-04-01 19:37:04.000000 oracledb-2.2.0/src/oracledb/impl/thick/pool.pyx
--rw-rw-r--   0 root         (0) root         (0)    21424 2023-05-22 21:44:58.000000 oracledb-2.2.0/src/oracledb/impl/thick/queue.pyx
--rw-rw-r--   0 root         (0) root         (0)    25297 2024-03-25 23:37:27.000000 oracledb-2.2.0/src/oracledb/impl/thick/soda.pyx
--rw-rw-r--   0 root         (0) root         (0)     7310 2024-03-25 23:37:27.000000 oracledb-2.2.0/src/oracledb/impl/thick/subscr.pyx
--rw-rw-r--   0 root         (0) root         (0)    23798 2024-04-19 23:14:55.000000 oracledb-2.2.0/src/oracledb/impl/thick/utils.pyx
--rw-rw-r--   0 root         (0) root         (0)    11661 2024-04-19 23:14:55.000000 oracledb-2.2.0/src/oracledb/impl/thick/var.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 21:01:45.276390 oracledb-2.2.0/src/oracledb/impl/thin/
--rw-rw-r--   0 root         (0) root         (0)     6387 2024-04-30 18:59:09.000000 oracledb-2.2.0/src/oracledb/impl/thin/capabilities.pyx
--rw-rw-r--   0 root         (0) root         (0)    21891 2024-04-26 22:27:56.000000 oracledb-2.2.0/src/oracledb/impl/thin/connection.pyx
--rw-rw-r--   0 root         (0) root         (0)    23111 2024-04-30 18:59:09.000000 oracledb-2.2.0/src/oracledb/impl/thin/constants.pxi
--rw-rw-r--   0 root         (0) root         (0)     7891 2024-03-25 23:37:27.000000 oracledb-2.2.0/src/oracledb/impl/thin/conversions.pyx
--rw-rw-r--   0 root         (0) root         (0)     3949 2024-03-08 04:11:12.000000 oracledb-2.2.0/src/oracledb/impl/thin/crypto.pyx
--rw-rw-r--   0 root         (0) root         (0)    12900 2024-04-19 23:14:55.000000 oracledb-2.2.0/src/oracledb/impl/thin/cursor.pyx
--rw-rw-r--   0 root         (0) root         (0)    23990 2024-03-25 23:37:27.000000 oracledb-2.2.0/src/oracledb/impl/thin/data_types.pyx
--rw-rw-r--   0 root         (0) root         (0)    23860 2024-04-19 23:14:55.000000 oracledb-2.2.0/src/oracledb/impl/thin/dbobject.pyx
--rw-rw-r--   0 root         (0) root         (0)    30408 2024-04-24 22:29:32.000000 oracledb-2.2.0/src/oracledb/impl/thin/dbobject_cache.pyx
--rw-rw-r--   0 root         (0) root         (0)    12546 2024-03-08 04:11:12.000000 oracledb-2.2.0/src/oracledb/impl/thin/lob.pyx
--rw-rw-r--   0 root         (0) root         (0)   110107 2024-04-30 18:59:09.000000 oracledb-2.2.0/src/oracledb/impl/thin/messages.pyx
--rw-rw-r--   0 root         (0) root         (0)    34571 2024-04-30 22:06:28.000000 oracledb-2.2.0/src/oracledb/impl/thin/packet.pyx
--rw-rw-r--   0 root         (0) root         (0)    35635 2024-04-30 19:15:50.000000 oracledb-2.2.0/src/oracledb/impl/thin/pool.pyx
--rw-rw-r--   0 root         (0) root         (0)    39709 2024-05-01 20:35:08.000000 oracledb-2.2.0/src/oracledb/impl/thin/protocol.pyx
--rw-rw-r--   0 root         (0) root         (0)    18199 2024-03-27 01:19:00.000000 oracledb-2.2.0/src/oracledb/impl/thin/statement.pyx
--rw-rw-r--   0 root         (0) root         (0)     7444 2024-03-25 23:37:27.000000 oracledb-2.2.0/src/oracledb/impl/thin/statement_cache.pyx
--rw-rw-r--   0 root         (0) root         (0)    13869 2024-04-18 22:46:32.000000 oracledb-2.2.0/src/oracledb/impl/thin/transport.pyx
--rw-rw-r--   0 root         (0) root         (0)     4852 2024-04-30 00:01:15.000000 oracledb-2.2.0/src/oracledb/impl/thin/utils.pyx
--rw-rw-r--   0 root         (0) root         (0)     5544 2024-03-08 04:11:12.000000 oracledb-2.2.0/src/oracledb/impl/thin/var.pyx
--rw-rw-r--   0 root         (0) root         (0)    11397 2024-04-19 23:14:55.000000 oracledb-2.2.0/src/oracledb/lob.py
--rw-rw-r--   0 root         (0) root         (0)    56457 2024-04-19 20:52:43.000000 oracledb-2.2.0/src/oracledb/pool.py
--rw-rw-r--   0 root         (0) root         (0)    33746 2024-04-18 22:46:32.000000 oracledb-2.2.0/src/oracledb/pool_params.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-22 21:44:58.000000 oracledb-2.2.0/src/oracledb/py.typed
--rw-rw-r--   0 root         (0) root         (0)    28590 2024-03-25 23:37:27.000000 oracledb-2.2.0/src/oracledb/soda.py
--rw-rw-r--   0 root         (0) root         (0)    11067 2023-12-16 03:36:53.000000 oracledb-2.2.0/src/oracledb/subscr.py
--rw-rw-r--   0 root         (0) root         (0)     3342 2024-04-11 20:42:10.000000 oracledb-2.2.0/src/oracledb/thick_impl.pyx
--rw-rw-r--   0 root         (0) root         (0)     5156 2024-04-11 20:42:10.000000 oracledb-2.2.0/src/oracledb/thin_impl.pyx
--rw-rw-r--   0 root         (0) root         (0)     3422 2023-12-16 03:36:53.000000 oracledb-2.2.0/src/oracledb/utils.py
--rw-rw-r--   0 root         (0) root         (0)     6604 2023-12-16 03:36:53.000000 oracledb-2.2.0/src/oracledb/var.py
--rw-rw-r--   0 root         (0) root         (0)     1533 2024-04-26 22:01:15.000000 oracledb-2.2.0/src/oracledb/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 21:01:45.284390 oracledb-2.2.0/src/oracledb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5208 2024-05-01 21:01:45.000000 oracledb-2.2.0/src/oracledb.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     6627 2024-05-01 21:01:45.000000 oracledb-2.2.0/src/oracledb.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2024-05-01 21:01:45.000000 oracledb-2.2.0/src/oracledb.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2024-04-11 16:14:40.000000 oracledb-2.2.0/src/oracledb.egg-info/not-zip-safe
--rw-rw-r--   0 root         (0) root         (0)       20 2024-05-01 21:01:45.000000 oracledb-2.2.0/src/oracledb.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)        9 2024-05-01 21:01:45.000000 oracledb-2.2.0/src/oracledb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 21:01:45.284390 oracledb-2.2.0/tests/
--rw-rw-r--   0 root         (0) root         (0)     2403 2024-04-26 22:01:15.000000 oracledb-2.2.0/tests/create_schema.py
--rw-rw-r--   0 root         (0) root         (0)     1897 2023-12-16 03:36:53.000000 oracledb-2.2.0/tests/drop_schema.py
--rw-rw-r--   0 root         (0) root         (0)     6790 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_1000_module.py
--rw-rw-r--   0 root         (0) root         (0)    30266 2024-05-01 17:51:27.000000 oracledb-2.2.0/tests/test_1100_connection.py
--rw-rw-r--   0 root         (0) root         (0)    13794 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_1300_cursor_var.py
--rw-rw-r--   0 root         (0) root         (0)    11040 2024-03-08 04:11:12.000000 oracledb-2.2.0/tests/test_1400_datetime_var.py
--rw-rw-r--   0 root         (0) root         (0)     8894 2024-03-08 04:11:12.000000 oracledb-2.2.0/tests/test_1500_types.py
--rw-rw-r--   0 root         (0) root         (0)    19708 2024-04-30 22:06:28.000000 oracledb-2.2.0/tests/test_1600_dml_returning.py
--rw-rw-r--   0 root         (0) root         (0)     7433 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_1700_error.py
--rw-rw-r--   0 root         (0) root         (0)     7930 2024-04-11 20:42:10.000000 oracledb-2.2.0/tests/test_1800_interval_var.py
--rw-rw-r--   0 root         (0) root         (0)    21081 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_1900_lob_var.py
--rw-rw-r--   0 root         (0) root         (0)     5045 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_2000_long_var.py
--rw-rw-r--   0 root         (0) root         (0)    11361 2024-03-08 04:11:12.000000 oracledb-2.2.0/tests/test_2100_nchar_var.py
--rw-rw-r--   0 root         (0) root         (0)    20614 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_2200_number_var.py
--rw-rw-r--   0 root         (0) root         (0)    29955 2024-04-11 20:42:10.000000 oracledb-2.2.0/tests/test_2300_object_var.py
--rw-rw-r--   0 root         (0) root         (0)    32800 2024-04-24 22:29:32.000000 oracledb-2.2.0/tests/test_2400_pool.py
--rw-rw-r--   0 root         (0) root         (0)    20848 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_2500_string_var.py
--rw-rw-r--   0 root         (0) root         (0)     7757 2024-03-08 04:11:12.000000 oracledb-2.2.0/tests/test_2600_timestamp_var.py
--rw-rw-r--   0 root         (0) root         (0)    29474 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_2700_aq.py
--rw-rw-r--   0 root         (0) root         (0)     8653 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_2800_bulk_aq.py
--rw-rw-r--   0 root         (0) root         (0)     7929 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_2900_rowid.py
--rw-rw-r--   0 root         (0) root         (0)    16130 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_3000_subscription.py
--rw-rw-r--   0 root         (0) root         (0)     4361 2024-04-26 22:01:15.000000 oracledb-2.2.0/tests/test_3100_boolean_var.py
--rw-rw-r--   0 root         (0) root         (0)    23087 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_3200_features_12_1.py
--rw-rw-r--   0 root         (0) root         (0)    10306 2024-04-24 22:29:32.000000 oracledb-2.2.0/tests/test_3300_soda_database.py
--rw-rw-r--   0 root         (0) root         (0)    41340 2024-04-26 22:01:15.000000 oracledb-2.2.0/tests/test_3400_soda_collection.py
--rw-rw-r--   0 root         (0) root         (0)    13612 2024-04-30 22:06:28.000000 oracledb-2.2.0/tests/test_3500_json.py
--rw-rw-r--   0 root         (0) root         (0)    24277 2024-04-30 22:06:28.000000 oracledb-2.2.0/tests/test_3600_outputtypehandler.py
--rw-rw-r--   0 root         (0) root         (0)    21053 2024-03-08 04:11:12.000000 oracledb-2.2.0/tests/test_3700_var.py
--rw-rw-r--   0 root         (0) root         (0)    11285 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_3800_typehandler.py
--rw-rw-r--   0 root         (0) root         (0)    21126 2024-04-26 22:01:15.000000 oracledb-2.2.0/tests/test_3900_cursor_execute.py
--rw-rw-r--   0 root         (0) root         (0)    16487 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_4000_cursor_executemany.py
--rw-rw-r--   0 root         (0) root         (0)     5444 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_4100_cursor_callproc.py
--rw-rw-r--   0 root         (0) root         (0)     8939 2024-04-01 20:35:52.000000 oracledb-2.2.0/tests/test_4200_cursor_scrollable.py
--rw-rw-r--   0 root         (0) root         (0)    38166 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_4300_cursor_other.py
--rw-rw-r--   0 root         (0) root         (0)    13877 2024-04-26 22:27:56.000000 oracledb-2.2.0/tests/test_4400_tpc.py
--rw-rw-r--   0 root         (0) root         (0)    32838 2024-04-24 22:29:32.000000 oracledb-2.2.0/tests/test_4500_connect_params.py
--rw-rw-r--   0 root         (0) root         (0)     8819 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_4600_type_changes.py
--rw-rw-r--   0 root         (0) root         (0)     5061 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_4700_pool_params.py
--rw-rw-r--   0 root         (0) root         (0)     7736 2024-03-08 04:11:12.000000 oracledb-2.2.0/tests/test_4800_timestamp_ltz_var.py
--rw-rw-r--   0 root         (0) root         (0)     7437 2024-03-08 04:11:12.000000 oracledb-2.2.0/tests/test_4900_timestamp_tz_var.py
--rw-rw-r--   0 root         (0) root         (0)    10665 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_5000_externalauth.py
--rw-rw-r--   0 root         (0) root         (0)     3696 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_5100_arrayvar.py
--rw-rw-r--   0 root         (0) root         (0)     7089 2024-03-08 04:11:12.000000 oracledb-2.2.0/tests/test_5200_sql_parser.py
--rw-rw-r--   0 root         (0) root         (0)    24489 2024-05-01 17:51:27.000000 oracledb-2.2.0/tests/test_5300_connection_async.py
--rw-rw-r--   0 root         (0) root         (0)    22559 2024-04-24 22:29:32.000000 oracledb-2.2.0/tests/test_5400_cursor_execute_async.py
--rw-rw-r--   0 root         (0) root         (0)    18392 2024-04-24 22:29:32.000000 oracledb-2.2.0/tests/test_5500_pool_async.py
--rw-rw-r--   0 root         (0) root         (0)    22554 2024-04-11 20:42:10.000000 oracledb-2.2.0/tests/test_5600_dbobject_async.py
--rw-rw-r--   0 root         (0) root         (0)    17851 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_5700_lob_var_async.py
--rw-rw-r--   0 root         (0) root         (0)    14480 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_5800_cursor_var_async.py
--rw-rw-r--   0 root         (0) root         (0)    19301 2024-04-30 22:06:28.000000 oracledb-2.2.0/tests/test_5900_dml_returning_async.py
--rw-rw-r--   0 root         (0) root         (0)    10133 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_6000_typehandler_async.py
--rw-rw-r--   0 root         (0) root         (0)    14724 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_6100_cursor_executemany_async.py
--rw-rw-r--   0 root         (0) root         (0)     5052 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_6200_cursor_callproc_async.py
--rw-rw-r--   0 root         (0) root         (0)    33553 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_6300_cursor_other_async.py
--rw-rw-r--   0 root         (0) root         (0)    20576 2024-04-26 22:01:15.000000 oracledb-2.2.0/tests/test_6400_vector_var.py
--rw-rw-r--   0 root         (0) root         (0)     8733 2024-04-26 22:01:15.000000 oracledb-2.2.0/tests/test_6500_vector_interop.py
--rw-rw-r--   0 root         (0) root         (0)     4544 2024-04-24 22:29:32.000000 oracledb-2.2.0/tests/test_6600_defaults.py
--rw-rw-r--   0 root         (0) root         (0)     6690 2024-04-26 22:01:15.000000 oracledb-2.2.0/tests/test_6700_json_23.py
--rw-rw-r--   0 root         (0) root         (0)     5422 2024-03-08 04:11:12.000000 oracledb-2.2.0/tests/test_6800_error_async.py
--rw-rw-r--   0 root         (0) root         (0)     4568 2024-04-24 22:29:32.000000 oracledb-2.2.0/tests/test_6900_oson.py
--rw-rw-r--   0 root         (0) root         (0)    11087 2024-05-01 02:39:27.000000 oracledb-2.2.0/tests/test_7000_connection_async_shortcut_methods.py
--rw-rw-r--   0 root         (0) root         (0)     6794 2024-04-11 20:42:10.000000 oracledb-2.2.0/tests/test_7100_interval_ym_var.py
--rw-rw-r--   0 root         (0) root         (0)    21545 2024-05-01 19:08:56.000000 oracledb-2.2.0/tests/test_7200_tnsnames.py
--rw-rw-r--   0 root         (0) root         (0)     2375 2024-04-24 22:29:32.000000 oracledb-2.2.0/tests/test_7300_unsupported_features_thin.py
--rw-rw-r--   0 root         (0) root         (0)    24050 2024-03-25 23:37:27.000000 oracledb-2.2.0/tests/test_env.py
--rw-rw-r--   0 root         (0) root         (0)      596 2023-12-16 03:36:53.000000 oracledb-2.2.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 19:14:18.478583 oracledb-2.2.1/
+-rw-rw-r--   0 root         (0) root         (0)    12570 2024-05-08 04:16:30.000000 oracledb-2.2.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      398 2022-05-20 21:47:15.000000 oracledb-2.2.1/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)       56 2024-05-08 04:16:30.000000 oracledb-2.2.1/NOTICE.txt
+-rw-r--r--   0 root         (0) root         (0)     5208 2024-05-27 19:14:18.478583 oracledb-2.2.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3730 2024-03-22 04:07:57.000000 oracledb-2.2.1/README.md
+-rw-rw-r--   0 root         (0) root         (0)      166 2024-03-22 04:07:57.000000 oracledb-2.2.1/README.txt
+-rw-rw-r--   0 root         (0) root         (0)    28103 2024-03-22 04:07:57.000000 oracledb-2.2.1/THIRD_PARTY_LICENSES.txt
+-rw-rw-r--   0 root         (0) root         (0)      310 2024-05-08 04:16:30.000000 oracledb-2.2.1/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)     1608 2024-05-27 19:14:18.478583 oracledb-2.2.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     3878 2024-03-22 04:07:57.000000 oracledb-2.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 19:14:18.453583 oracledb-2.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 19:14:18.458583 oracledb-2.2.1/src/oracledb/
+-rw-rw-r--   0 root         (0) root         (0)    11213 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    19011 2024-03-22 04:07:57.000000 oracledb-2.2.1/src/oracledb/aq.py
+-rw-rw-r--   0 root         (0) root         (0)    25876 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/base_impl.pxd
+-rw-rw-r--   0 root         (0) root         (0)     3711 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/base_impl.pyx
+-rw-rw-r--   0 root         (0) root         (0)    36682 2024-05-22 16:13:32.000000 oracledb-2.2.1/src/oracledb/connect_params.py
+-rw-rw-r--   0 root         (0) root         (0)    75308 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/connection.py
+-rw-rw-r--   0 root         (0) root         (0)     4144 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/constants.py
+-rw-rw-r--   0 root         (0) root         (0)     2909 2024-03-22 04:07:57.000000 oracledb-2.2.1/src/oracledb/constructors.py
+-rw-rw-r--   0 root         (0) root         (0)    44011 2024-05-08 04:16:30.000000 oracledb-2.2.1/src/oracledb/cursor.py
+-rw-rw-r--   0 root         (0) root         (0)    11862 2024-05-22 16:13:32.000000 oracledb-2.2.1/src/oracledb/dbobject.py
+-rw-rw-r--   0 root         (0) root         (0)     3492 2024-05-08 04:16:30.000000 oracledb-2.2.1/src/oracledb/defaults.py
+-rw-rw-r--   0 root         (0) root         (0)     5483 2024-03-22 04:07:57.000000 oracledb-2.2.1/src/oracledb/driver_mode.py
+-rw-rw-r--   0 root         (0) root         (0)     3160 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/dsn.py
+-rw-rw-r--   0 root         (0) root         (0)    28688 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/errors.py
+-rw-rw-r--   0 root         (0) root         (0)     1812 2024-03-22 04:07:57.000000 oracledb-2.2.1/src/oracledb/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)     7448 2024-05-08 04:16:30.000000 oracledb-2.2.1/src/oracledb/fetch_info.py
+-rw-rw-r--   0 root         (0) root         (0)     1717 2024-03-22 04:07:57.000000 oracledb-2.2.1/src/oracledb/future.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 19:14:18.453583 oracledb-2.2.1/src/oracledb/impl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 19:14:18.461583 oracledb-2.2.1/src/oracledb/impl/base/
+-rw-r--r--   0 root         (0) root         (0)     7341 2022-05-20 21:47:15.000000 oracledb-2.2.1/src/oracledb/impl/base/bind_var.pyx
+-rw-rw-r--   0 root         (0) root         (0)    47777 2024-05-24 01:33:13.000000 oracledb-2.2.1/src/oracledb/impl/base/buffer.pyx
+-rw-rw-r--   0 root         (0) root         (0)    45785 2024-05-24 18:07:32.000000 oracledb-2.2.1/src/oracledb/impl/base/connect_params.pyx
+-rw-rw-r--   0 root         (0) root         (0)    14208 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/impl/base/connection.pyx
+-rw-rw-r--   0 root         (0) root         (0)     3399 2024-05-22 16:13:32.000000 oracledb-2.2.1/src/oracledb/impl/base/constants.pxi
+-rw-rw-r--   0 root         (0) root         (0)    25501 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/impl/base/cursor.pyx
+-rw-rw-r--   0 root         (0) root         (0)     7066 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/impl/base/dbobject.pyx
+-rw-rw-r--   0 root         (0) root         (0)     1702 2024-05-08 04:16:30.000000 oracledb-2.2.1/src/oracledb/impl/base/defaults.pyx
+-rw-rw-r--   0 root         (0) root         (0)     2741 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/impl/base/lob.pyx
+-rw-rw-r--   0 root         (0) root         (0)    33590 2024-05-08 04:16:30.000000 oracledb-2.2.1/src/oracledb/impl/base/oson.pyx
+-rw-rw-r--   0 root         (0) root         (0)     4215 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/impl/base/pool.pyx
+-rw-rw-r--   0 root         (0) root         (0)     4288 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/impl/base/pool_params.pyx
+-rw-rw-r--   0 root         (0) root         (0)     6379 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/impl/base/queue.pyx
+-rw-rw-r--   0 root         (0) root         (0)     4799 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/impl/base/soda.pyx
+-rw-rw-r--   0 root         (0) root         (0)     1933 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/impl/base/subscr.pyx
+-rw-rw-r--   0 root         (0) root         (0)    10416 2024-05-22 16:13:32.000000 oracledb-2.2.1/src/oracledb/impl/base/types.pyx
+-rw-rw-r--   0 root         (0) root         (0)     7891 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/impl/base/utils.pyx
+-rw-rw-r--   0 root         (0) root         (0)    11753 2024-05-22 16:13:32.000000 oracledb-2.2.1/src/oracledb/impl/base/var.pyx
+-rw-rw-r--   0 root         (0) root         (0)     5714 2024-05-22 16:13:32.000000 oracledb-2.2.1/src/oracledb/impl/base/vector.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 19:14:18.463583 oracledb-2.2.1/src/oracledb/impl/thick/
+-rw-rw-r--   0 root         (0) root         (0)     2264 2024-05-08 04:16:30.000000 oracledb-2.2.1/src/oracledb/impl/thick/buffer.pyx
+-rw-rw-r--   0 root         (0) root         (0)    32798 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/impl/thick/connection.pyx
+-rw-rw-r--   0 root         (0) root         (0)    21322 2024-05-22 16:13:32.000000 oracledb-2.2.1/src/oracledb/impl/thick/cursor.pyx
+-rw-rw-r--   0 root         (0) root         (0)    14836 2024-05-08 04:16:30.000000 oracledb-2.2.1/src/oracledb/impl/thick/dbobject.pyx
+-rw-rw-r--   0 root         (0) root         (0)     9894 2024-05-08 04:16:30.000000 oracledb-2.2.1/src/oracledb/impl/thick/json.pyx
+-rw-r--r--   0 root         (0) root         (0)     7534 2022-05-20 21:47:15.000000 oracledb-2.2.1/src/oracledb/impl/thick/lob.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 19:14:18.453583 oracledb-2.2.1/src/oracledb/impl/thick/odpi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 19:14:18.463583 oracledb-2.2.1/src/oracledb/impl/thick/odpi/embed/
+-rw-rw-r--   0 root         (0) root         (0)     2633 2024-03-11 15:29:55.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/embed/dpi.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 19:14:18.463583 oracledb-2.2.1/src/oracledb/impl/thick/odpi/include/
+-rw-rw-r--   0 root         (0) root         (0)    86869 2024-03-11 15:29:55.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/include/dpi.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 19:14:18.468583 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/
+-rw-rw-r--   0 root         (0) root         (0)   117539 2024-03-11 15:29:55.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiConn.c
+-rw-rw-r--   0 root         (0) root         (0)    16874 2024-03-11 15:29:55.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiContext.c
+-rw-r--r--   0 root         (0) root         (0)    34806 2022-05-20 22:11:04.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiData.c
+-rw-r--r--   0 root         (0) root         (0)     7443 2022-05-20 22:11:04.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiDebug.c
+-rw-r--r--   0 root         (0) root         (0)    15574 2022-05-20 22:11:04.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiDeqOptions.c
+-rw-r--r--   0 root         (0) root         (0)     7552 2022-05-20 22:11:04.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiEnqOptions.c
+-rw-r--r--   0 root         (0) root         (0)     9569 2022-05-20 22:11:04.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiEnv.c
+-rw-rw-r--   0 root         (0) root         (0)    14038 2024-02-28 17:15:47.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiError.c
+-rw-rw-r--   0 root         (0) root         (0)     9348 2024-03-11 15:29:55.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiErrorMessages.h
+-rw-rw-r--   0 root         (0) root         (0)    13273 2024-03-11 15:29:55.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiGen.c
+-rw-r--r--   0 root         (0) root         (0)    15039 2022-11-07 17:19:09.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiGlobal.c
+-rw-r--r--   0 root         (0) root         (0)     5184 2022-05-20 22:11:04.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiHandleList.c
+-rw-r--r--   0 root         (0) root         (0)     5399 2022-05-20 22:11:04.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiHandlePool.c
+-rw-rw-r--   0 root         (0) root         (0)   111354 2024-03-11 15:29:55.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiImpl.h
+-rw-rw-r--   0 root         (0) root         (0)    37212 2024-03-11 15:29:55.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiJson.c
+-rw-rw-r--   0 root         (0) root         (0)    19868 2024-02-03 18:38:13.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiLob.c
+-rw-r--r--   0 root         (0) root         (0)    23232 2022-08-27 21:56:08.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiMsgProps.c
+-rw-r--r--   0 root         (0) root         (0)    40061 2022-05-20 22:11:04.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiObject.c
+-rw-rw-r--   0 root         (0) root         (0)     5372 2024-02-03 18:38:13.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiObjectAttr.c
+-rw-rw-r--   0 root         (0) root         (0)    15195 2024-02-03 18:38:13.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiObjectType.c
+-rw-rw-r--   0 root         (0) root         (0)   182440 2024-03-11 15:29:55.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiOci.c
+-rw-rw-r--   0 root         (0) root         (0)    32160 2024-03-11 15:29:55.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiOracleType.c
+-rw-r--r--   0 root         (0) root         (0)    32638 2022-08-02 17:00:34.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiPool.c
+-rw-rw-r--   0 root         (0) root         (0)    23704 2024-03-11 15:29:55.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiQueue.c
+-rw-r--r--   0 root         (0) root         (0)     5712 2022-05-20 22:11:04.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiRowid.c
+-rw-rw-r--   0 root         (0) root         (0)    42311 2024-03-11 15:29:55.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiSodaColl.c
+-rw-r--r--   0 root         (0) root         (0)     6131 2022-05-20 22:11:04.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiSodaCollCursor.c
+-rw-rw-r--   0 root         (0) root         (0)    16800 2024-03-11 15:29:55.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiSodaDb.c
+-rw-rw-r--   0 root         (0) root         (0)    12671 2024-03-11 15:29:55.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiSodaDoc.c
+-rw-r--r--   0 root         (0) root         (0)     6134 2022-05-20 22:11:04.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiSodaDocCursor.c
+-rw-rw-r--   0 root         (0) root         (0)    79506 2024-02-03 18:38:13.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiStmt.c
+-rw-rw-r--   0 root         (0) root         (0)     4221 2024-01-05 20:41:23.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiStringList.c
+-rw-r--r--   0 root         (0) root         (0)    29091 2022-05-20 22:11:04.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiSubscr.c
+-rw-r--r--   0 root         (0) root         (0)    23589 2022-11-01 20:30:53.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiUtils.c
+-rw-rw-r--   0 root         (0) root         (0)    81960 2024-03-11 15:29:55.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiVar.c
+-rw-rw-r--   0 root         (0) root         (0)     7710 2024-03-11 15:29:55.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiVector.c
+-rw-rw-r--   0 root         (0) root         (0)    41686 2024-05-08 04:16:30.000000 oracledb-2.2.1/src/oracledb/impl/thick/odpi.pxd
+-rw-rw-r--   0 root         (0) root         (0)    13993 2024-05-08 04:16:30.000000 oracledb-2.2.1/src/oracledb/impl/thick/pool.pyx
+-rw-rw-r--   0 root         (0) root         (0)    21424 2023-12-12 01:18:55.000000 oracledb-2.2.1/src/oracledb/impl/thick/queue.pyx
+-rw-rw-r--   0 root         (0) root         (0)    25297 2024-05-08 04:16:30.000000 oracledb-2.2.1/src/oracledb/impl/thick/soda.pyx
+-rw-rw-r--   0 root         (0) root         (0)     7310 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/impl/thick/subscr.pyx
+-rw-rw-r--   0 root         (0) root         (0)    23798 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/impl/thick/utils.pyx
+-rw-rw-r--   0 root         (0) root         (0)    11661 2024-05-08 04:16:30.000000 oracledb-2.2.1/src/oracledb/impl/thick/var.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 19:14:18.470583 oracledb-2.2.1/src/oracledb/impl/thin/
+-rw-rw-r--   0 root         (0) root         (0)     6387 2024-05-22 16:13:32.000000 oracledb-2.2.1/src/oracledb/impl/thin/capabilities.pyx
+-rw-rw-r--   0 root         (0) root         (0)    21891 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/impl/thin/connection.pyx
+-rw-rw-r--   0 root         (0) root         (0)    23111 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/impl/thin/constants.pxi
+-rw-rw-r--   0 root         (0) root         (0)     7891 2024-05-08 04:16:30.000000 oracledb-2.2.1/src/oracledb/impl/thin/conversions.pyx
+-rw-rw-r--   0 root         (0) root         (0)     3949 2024-03-22 04:07:57.000000 oracledb-2.2.1/src/oracledb/impl/thin/crypto.pyx
+-rw-rw-r--   0 root         (0) root         (0)    12900 2024-05-08 04:16:30.000000 oracledb-2.2.1/src/oracledb/impl/thin/cursor.pyx
+-rw-rw-r--   0 root         (0) root         (0)    23990 2024-05-08 04:16:30.000000 oracledb-2.2.1/src/oracledb/impl/thin/data_types.pyx
+-rw-rw-r--   0 root         (0) root         (0)    25404 2024-05-24 01:34:32.000000 oracledb-2.2.1/src/oracledb/impl/thin/dbobject.pyx
+-rw-rw-r--   0 root         (0) root         (0)    30828 2024-05-24 01:34:32.000000 oracledb-2.2.1/src/oracledb/impl/thin/dbobject_cache.pyx
+-rw-rw-r--   0 root         (0) root         (0)    12546 2024-05-08 04:16:30.000000 oracledb-2.2.1/src/oracledb/impl/thin/lob.pyx
+-rw-rw-r--   0 root         (0) root         (0)   110227 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/impl/thin/messages.pyx
+-rw-rw-r--   0 root         (0) root         (0)    33804 2024-05-24 01:34:32.000000 oracledb-2.2.1/src/oracledb/impl/thin/packet.pyx
+-rw-rw-r--   0 root         (0) root         (0)    35635 2024-05-22 16:13:32.000000 oracledb-2.2.1/src/oracledb/impl/thin/pool.pyx
+-rw-rw-r--   0 root         (0) root         (0)    39711 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/impl/thin/protocol.pyx
+-rw-rw-r--   0 root         (0) root         (0)    18199 2024-05-08 04:16:30.000000 oracledb-2.2.1/src/oracledb/impl/thin/statement.pyx
+-rw-rw-r--   0 root         (0) root         (0)     7566 2024-05-24 01:33:35.000000 oracledb-2.2.1/src/oracledb/impl/thin/statement_cache.pyx
+-rw-rw-r--   0 root         (0) root         (0)    13997 2024-05-24 18:07:09.000000 oracledb-2.2.1/src/oracledb/impl/thin/transport.pyx
+-rw-rw-r--   0 root         (0) root         (0)     4852 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/impl/thin/utils.pyx
+-rw-rw-r--   0 root         (0) root         (0)     5544 2024-05-08 04:16:30.000000 oracledb-2.2.1/src/oracledb/impl/thin/var.pyx
+-rw-rw-r--   0 root         (0) root         (0)    11397 2024-05-08 04:16:30.000000 oracledb-2.2.1/src/oracledb/lob.py
+-rw-rw-r--   0 root         (0) root         (0)    56457 2024-05-08 04:16:30.000000 oracledb-2.2.1/src/oracledb/pool.py
+-rw-rw-r--   0 root         (0) root         (0)    33746 2024-05-08 04:16:30.000000 oracledb-2.2.1/src/oracledb/pool_params.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-05-20 21:47:15.000000 oracledb-2.2.1/src/oracledb/py.typed
+-rw-rw-r--   0 root         (0) root         (0)    28590 2024-05-08 04:16:30.000000 oracledb-2.2.1/src/oracledb/soda.py
+-rw-rw-r--   0 root         (0) root         (0)    11067 2024-03-22 04:07:57.000000 oracledb-2.2.1/src/oracledb/subscr.py
+-rw-rw-r--   0 root         (0) root         (0)     3342 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/thick_impl.pyx
+-rw-rw-r--   0 root         (0) root         (0)     5156 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/thin_impl.pyx
+-rw-rw-r--   0 root         (0) root         (0)     3422 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/utils.py
+-rw-rw-r--   0 root         (0) root         (0)     6604 2024-03-22 04:07:57.000000 oracledb-2.2.1/src/oracledb/var.py
+-rw-rw-r--   0 root         (0) root         (0)     1533 2024-05-27 16:54:08.000000 oracledb-2.2.1/src/oracledb/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 19:14:18.478583 oracledb-2.2.1/src/oracledb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5208 2024-05-27 19:14:18.000000 oracledb-2.2.1/src/oracledb.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     6627 2024-05-27 19:14:18.000000 oracledb-2.2.1/src/oracledb.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2024-05-27 19:14:18.000000 oracledb-2.2.1/src/oracledb.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2024-05-27 17:26:15.000000 oracledb-2.2.1/src/oracledb.egg-info/not-zip-safe
+-rw-rw-r--   0 root         (0) root         (0)       20 2024-05-27 19:14:18.000000 oracledb-2.2.1/src/oracledb.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)        9 2024-05-27 19:14:18.000000 oracledb-2.2.1/src/oracledb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 19:14:18.478583 oracledb-2.2.1/tests/
+-rw-rw-r--   0 root         (0) root         (0)     2403 2024-05-22 16:13:32.000000 oracledb-2.2.1/tests/create_schema.py
+-rw-rw-r--   0 root         (0) root         (0)     1897 2024-03-22 04:07:57.000000 oracledb-2.2.1/tests/drop_schema.py
+-rw-rw-r--   0 root         (0) root         (0)     6790 2024-05-27 16:54:08.000000 oracledb-2.2.1/tests/test_1000_module.py
+-rw-rw-r--   0 root         (0) root         (0)    30266 2024-05-22 16:13:32.000000 oracledb-2.2.1/tests/test_1100_connection.py
+-rw-rw-r--   0 root         (0) root         (0)    13794 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_1300_cursor_var.py
+-rw-rw-r--   0 root         (0) root         (0)    11040 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_1400_datetime_var.py
+-rw-rw-r--   0 root         (0) root         (0)     8894 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_1500_types.py
+-rw-rw-r--   0 root         (0) root         (0)    19708 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_1600_dml_returning.py
+-rw-rw-r--   0 root         (0) root         (0)     7433 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_1700_error.py
+-rw-rw-r--   0 root         (0) root         (0)     7930 2024-05-22 16:13:32.000000 oracledb-2.2.1/tests/test_1800_interval_var.py
+-rw-rw-r--   0 root         (0) root         (0)    21081 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_1900_lob_var.py
+-rw-rw-r--   0 root         (0) root         (0)     5045 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_2000_long_var.py
+-rw-rw-r--   0 root         (0) root         (0)    11361 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_2100_nchar_var.py
+-rw-rw-r--   0 root         (0) root         (0)    20614 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_2200_number_var.py
+-rw-rw-r--   0 root         (0) root         (0)    30544 2024-05-24 01:34:32.000000 oracledb-2.2.1/tests/test_2300_object_var.py
+-rw-rw-r--   0 root         (0) root         (0)    32800 2024-05-22 16:13:32.000000 oracledb-2.2.1/tests/test_2400_pool.py
+-rw-rw-r--   0 root         (0) root         (0)    20848 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_2500_string_var.py
+-rw-rw-r--   0 root         (0) root         (0)     7757 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_2600_timestamp_var.py
+-rw-rw-r--   0 root         (0) root         (0)    29474 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_2700_aq.py
+-rw-rw-r--   0 root         (0) root         (0)     8653 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_2800_bulk_aq.py
+-rw-rw-r--   0 root         (0) root         (0)     7929 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_2900_rowid.py
+-rw-rw-r--   0 root         (0) root         (0)    16130 2024-05-27 16:54:08.000000 oracledb-2.2.1/tests/test_3000_subscription.py
+-rw-rw-r--   0 root         (0) root         (0)     4361 2024-05-27 16:54:08.000000 oracledb-2.2.1/tests/test_3100_boolean_var.py
+-rw-rw-r--   0 root         (0) root         (0)    23087 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_3200_features_12_1.py
+-rw-rw-r--   0 root         (0) root         (0)    10306 2024-05-22 16:13:32.000000 oracledb-2.2.1/tests/test_3300_soda_database.py
+-rw-rw-r--   0 root         (0) root         (0)    41340 2024-05-27 16:54:08.000000 oracledb-2.2.1/tests/test_3400_soda_collection.py
+-rw-rw-r--   0 root         (0) root         (0)    13612 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_3500_json.py
+-rw-rw-r--   0 root         (0) root         (0)    24277 2024-05-22 16:13:32.000000 oracledb-2.2.1/tests/test_3600_outputtypehandler.py
+-rw-rw-r--   0 root         (0) root         (0)    21053 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_3700_var.py
+-rw-rw-r--   0 root         (0) root         (0)    11285 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_3800_typehandler.py
+-rw-rw-r--   0 root         (0) root         (0)    21126 2024-05-22 16:13:32.000000 oracledb-2.2.1/tests/test_3900_cursor_execute.py
+-rw-rw-r--   0 root         (0) root         (0)    16487 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_4000_cursor_executemany.py
+-rw-rw-r--   0 root         (0) root         (0)     5444 2024-05-27 16:54:08.000000 oracledb-2.2.1/tests/test_4100_cursor_callproc.py
+-rw-rw-r--   0 root         (0) root         (0)     8939 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_4200_cursor_scrollable.py
+-rw-rw-r--   0 root         (0) root         (0)    38699 2024-05-27 16:54:25.000000 oracledb-2.2.1/tests/test_4300_cursor_other.py
+-rw-rw-r--   0 root         (0) root         (0)    13877 2024-05-27 16:54:08.000000 oracledb-2.2.1/tests/test_4400_tpc.py
+-rw-rw-r--   0 root         (0) root         (0)    33994 2024-05-24 18:07:32.000000 oracledb-2.2.1/tests/test_4500_connect_params.py
+-rw-rw-r--   0 root         (0) root         (0)     8819 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_4600_type_changes.py
+-rw-rw-r--   0 root         (0) root         (0)     5061 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_4700_pool_params.py
+-rw-rw-r--   0 root         (0) root         (0)     7736 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_4800_timestamp_ltz_var.py
+-rw-rw-r--   0 root         (0) root         (0)     7437 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_4900_timestamp_tz_var.py
+-rw-rw-r--   0 root         (0) root         (0)    10665 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_5000_externalauth.py
+-rw-rw-r--   0 root         (0) root         (0)     3696 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_5100_arrayvar.py
+-rw-rw-r--   0 root         (0) root         (0)     7089 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_5200_sql_parser.py
+-rw-rw-r--   0 root         (0) root         (0)    24489 2024-05-22 16:13:32.000000 oracledb-2.2.1/tests/test_5300_connection_async.py
+-rw-rw-r--   0 root         (0) root         (0)    22559 2024-05-22 16:13:32.000000 oracledb-2.2.1/tests/test_5400_cursor_execute_async.py
+-rw-rw-r--   0 root         (0) root         (0)    18392 2024-05-22 16:13:32.000000 oracledb-2.2.1/tests/test_5500_pool_async.py
+-rw-rw-r--   0 root         (0) root         (0)    22554 2024-05-22 16:13:32.000000 oracledb-2.2.1/tests/test_5600_dbobject_async.py
+-rw-rw-r--   0 root         (0) root         (0)    17851 2024-05-27 16:54:08.000000 oracledb-2.2.1/tests/test_5700_lob_var_async.py
+-rw-rw-r--   0 root         (0) root         (0)    14480 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_5800_cursor_var_async.py
+-rw-rw-r--   0 root         (0) root         (0)    19301 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_5900_dml_returning_async.py
+-rw-rw-r--   0 root         (0) root         (0)    10133 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_6000_typehandler_async.py
+-rw-rw-r--   0 root         (0) root         (0)    14724 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_6100_cursor_executemany_async.py
+-rw-rw-r--   0 root         (0) root         (0)     5052 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_6200_cursor_callproc_async.py
+-rw-rw-r--   0 root         (0) root         (0)    34081 2024-05-24 01:38:20.000000 oracledb-2.2.1/tests/test_6300_cursor_other_async.py
+-rw-rw-r--   0 root         (0) root         (0)    20576 2024-05-22 16:13:32.000000 oracledb-2.2.1/tests/test_6400_vector_var.py
+-rw-rw-r--   0 root         (0) root         (0)     8733 2024-05-22 16:13:32.000000 oracledb-2.2.1/tests/test_6500_vector_interop.py
+-rw-rw-r--   0 root         (0) root         (0)     4544 2024-05-22 16:13:32.000000 oracledb-2.2.1/tests/test_6600_defaults.py
+-rw-rw-r--   0 root         (0) root         (0)     6690 2024-05-22 16:13:32.000000 oracledb-2.2.1/tests/test_6700_json_23.py
+-rw-rw-r--   0 root         (0) root         (0)     5422 2024-05-08 04:16:30.000000 oracledb-2.2.1/tests/test_6800_error_async.py
+-rw-rw-r--   0 root         (0) root         (0)     4568 2024-05-22 16:13:32.000000 oracledb-2.2.1/tests/test_6900_oson.py
+-rw-rw-r--   0 root         (0) root         (0)    11087 2024-05-22 16:13:32.000000 oracledb-2.2.1/tests/test_7000_connection_async_shortcut_methods.py
+-rw-rw-r--   0 root         (0) root         (0)     6794 2024-05-22 16:13:32.000000 oracledb-2.2.1/tests/test_7100_interval_ym_var.py
+-rw-rw-r--   0 root         (0) root         (0)    21545 2024-05-22 16:13:32.000000 oracledb-2.2.1/tests/test_7200_tnsnames.py
+-rw-rw-r--   0 root         (0) root         (0)     2375 2024-05-22 16:13:32.000000 oracledb-2.2.1/tests/test_7300_unsupported_features_thin.py
+-rw-rw-r--   0 root         (0) root         (0)    24050 2024-05-27 16:54:08.000000 oracledb-2.2.1/tests/test_env.py
+-rw-rw-r--   0 root         (0) root         (0)      596 2024-03-22 04:07:57.000000 oracledb-2.2.1/tox.ini
```

### Comparing `oracledb-2.2.0/LICENSE.txt` & `oracledb-2.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/PKG-INFO` & `oracledb-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oracledb
-Version: 2.2.0
+Version: 2.2.1
 Summary: Python interface to Oracle Database
 Home-page: https://oracle.github.io/python-oracledb
 Author: Anthony Tuininga
 Author-email: anthony.tuininga@oracle.com
 License: Apache and/or UPL
 Project-URL: Installation, https://python-oracledb.readthedocs.io/en/latest/user_guide/installation.html
 Project-URL: Samples, https://github.com/oracle/python-oracledb/tree/main/samples
```

### Comparing `oracledb-2.2.0/README.md` & `oracledb-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/THIRD_PARTY_LICENSES.txt` & `oracledb-2.2.1/THIRD_PARTY_LICENSES.txt`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/setup.cfg` & `oracledb-2.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/setup.py` & `oracledb-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/__init__.py` & `oracledb-2.2.1/src/oracledb/__init__.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/aq.py` & `oracledb-2.2.1/src/oracledb/aq.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/base_impl.pxd` & `oracledb-2.2.1/src/oracledb/base_impl.pxd`

 * *Files 0% similar despite different names*

```diff
@@ -187,16 +187,15 @@
     cdef object read_bool(self)
     cdef object read_bytes(self)
     cdef object read_date(self)
     cdef object read_interval_ds(self)
     cdef object read_interval_ym(self)
     cdef int read_int32(self, int32_t *value, int byte_order=*) except -1
     cdef object read_oracle_number(self, int preferred_num_type)
-    cdef inline const char_type* read_raw_bytes(self,
-                                                ssize_t num_bytes) except NULL
+    cdef const char_type* read_raw_bytes(self, ssize_t num_bytes) except NULL
     cdef int read_raw_bytes_and_length(self, const char_type **ptr,
                                        ssize_t *num_bytes) except -1
     cdef int read_sb1(self, int8_t *value) except -1
     cdef int read_sb2(self, int16_t *value) except -1
     cdef int read_sb4(self, int32_t *value) except -1
     cdef int read_sb8(self, int64_t *value) except -1
     cdef bytes read_null_terminated_bytes(self)
@@ -378,14 +377,15 @@
     cdef str _build_duration_str(self, double value)
     cdef str build_connect_string(self, str cid=*)
 
 
 cdef class DescriptionList(ConnectParamsNode):
 
     cdef str build_connect_string(self)
+    cdef list get_addresses(self)
 
 
 cdef class ConnectParamsImpl:
     cdef:
         public str config_dir
         public str user
         public str proxy_user
@@ -427,15 +427,16 @@
     cdef str _get_private_key(self)
     cdef str _get_token(self)
     cdef object _get_token_expires(self, str token)
     cdef str _get_wallet_password(self)
     cdef int _parse_connect_string(self, str connect_string) except -1
     cdef int _parse_easy_connect_string(self, str connect_string,
                                         object match) except -1
-    cdef int _process_connect_descriptor(self, dict args) except -1
+    cdef int _process_connect_descriptor(self, str connecte_string,
+                                         dict args) except -1
     cdef int _set_access_token(self, object val, int error_num) except -1
     cdef int _set_access_token_param(self, object val) except -1
     cdef int _set_new_password(self, str password) except -1
     cdef int _set_password(self, str password) except -1
     cdef int _set_wallet_password(self, str password) except -1
     cdef bytearray _xor_bytes(self, bytearray a, bytearray b)
```

### Comparing `oracledb-2.2.0/src/oracledb/base_impl.pyx` & `oracledb-2.2.1/src/oracledb/base_impl.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/connect_params.py` & `oracledb-2.2.1/src/oracledb/connect_params.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/connection.py` & `oracledb-2.2.1/src/oracledb/connection.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/constants.py` & `oracledb-2.2.1/src/oracledb/constants.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/constructors.py` & `oracledb-2.2.1/src/oracledb/constructors.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/cursor.py` & `oracledb-2.2.1/src/oracledb/cursor.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/dbobject.py` & `oracledb-2.2.1/src/oracledb/dbobject.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/defaults.py` & `oracledb-2.2.1/src/oracledb/defaults.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/driver_mode.py` & `oracledb-2.2.1/src/oracledb/driver_mode.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/dsn.py` & `oracledb-2.2.1/src/oracledb/dsn.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/errors.py` & `oracledb-2.2.1/src/oracledb/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,14 +239,15 @@
 ERR_MISSING_QUOTE_IN_IDENTIFIER = 2042
 ERR_DBOBJECT_ATTR_MAX_SIZE_VIOLATED = 2043
 ERR_DBOBJECT_ELEMENT_MAX_SIZE_VIOLATED = 2044
 ERR_INVALID_ARRAYSIZE = 2045
 ERR_CURSOR_HAS_BEEN_CLOSED = 2046
 ERR_INVALID_LOB_AMOUNT = 2047
 ERR_DML_RETURNING_DUP_BINDS = 2048
+ERR_MISSING_ADDRESS = 2049
 
 # error numbers that result in NotSupportedError
 ERR_TIME_NOT_SUPPORTED = 3000
 ERR_FEATURE_NOT_SUPPORTED = 3001
 ERR_PYTHON_VALUE_NOT_SUPPORTED = 3002
 ERR_PYTHON_TYPE_NOT_SUPPORTED = 3003
 ERR_UNSUPPORTED_TYPE_SET = 3004
@@ -572,14 +573,17 @@
         "{expected_type_name}"
     ),
     ERR_MESSAGE_HAS_NO_PAYLOAD: "message has no payload",
     ERR_MESSAGE_TYPE_UNKNOWN: (
         "internal error: unknown protocol message type {message_type} "
         "at position {position}"
     ),
+    ERR_MISSING_ADDRESS: (
+        "no addresses are defined in connect descriptor: {connect_string}"
+    ),
     ERR_MISSING_BIND_VALUE: (
         'a bind variable replacement value for placeholder ":{name}" was '
         "not provided"
     ),
     ERR_MISSING_FILE: "file '{file_name}' is missing or unreadable",
     ERR_MISSING_QUOTE_IN_IDENTIFIER: 'missing ending quote (") in identifier',
     ERR_MISSING_QUOTE_IN_STRING: "missing ending quote (') in string",
```

### Comparing `oracledb-2.2.0/src/oracledb/exceptions.py` & `oracledb-2.2.1/src/oracledb/exceptions.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/fetch_info.py` & `oracledb-2.2.1/src/oracledb/fetch_info.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/future.py` & `oracledb-2.2.1/src/oracledb/future.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/base/bind_var.pyx` & `oracledb-2.2.1/src/oracledb/impl/base/bind_var.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/base/buffer.pyx` & `oracledb-2.2.1/src/oracledb/impl/base/buffer.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -634,16 +634,15 @@
 
         # read the number of bytes in the number; if the value is 0 or the null
         # length indicator, return None
         self.read_raw_bytes_and_length(&ptr, &num_bytes)
         if ptr != NULL:
             return self.parse_oracle_number(ptr, num_bytes, preferred_num_type)
 
-    cdef inline const char_type* read_raw_bytes(self,
-                                                ssize_t num_bytes) except NULL:
+    cdef const char_type* read_raw_bytes(self, ssize_t num_bytes) except NULL:
         """
         Returns a pointer to a contiguous buffer containing the specified
         number of bytes found in the buffer.
         """
         return self._get_raw(num_bytes)
 
     cdef int read_raw_bytes_and_length(self, const char_type **ptr,
```

### Comparing `oracledb-2.2.0/src/oracledb/impl/base/connect_params.pyx` & `oracledb-2.2.1/src/oracledb/impl/base/connect_params.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -316,15 +316,15 @@
             dict args = {}
             str name
 
         # if a connect string starts with an opening parenthesis it is assumed
         # to be a full connect descriptor
         if connect_string.startswith("("):
             _parse_connect_descriptor(connect_string, args)
-            return self._process_connect_descriptor(args)
+            return self._process_connect_descriptor(connect_string, args)
 
         # otherwise, see if the connect string is an EasyConnect string
         m = re.search(EASY_CONNECT_PATTERN, connect_string)
         if m is not None:
             self._parse_easy_connect_string(connect_string, m)
 
         # otherwise, see if the name is a connect alias in a tnsnames.ora
@@ -338,15 +338,15 @@
                 errors._raise_err(errors.ERR_TNS_ENTRY_NOT_FOUND, name=name,
                                   file_name=tnsnames_file.file_name)
             m = re.search(EASY_CONNECT_PATTERN, connect_string)
             if m is not None:
                 self._parse_easy_connect_string(connect_string, m)
             else:
                 _parse_connect_descriptor(connect_string, args)
-                self._process_connect_descriptor(args)
+                self._process_connect_descriptor(connect_string, args)
 
     cdef int _parse_easy_connect_string(self, str connect_string,
                                         object match) except -1:
         """
         Internal method for parsing an Easy Connect string.
         """
         cdef:
@@ -378,48 +378,54 @@
         description.set_from_description_args(args)
         description.set_from_security_args(args)
         description.children = [AddressList()]
         description.children[0].children.append(address)
         self.description_list = DescriptionList()
         self.description_list.children.append(description)
 
-    cdef int _process_connect_descriptor(self, dict args) except -1:
+    cdef int _process_connect_descriptor(self, str connect_string,
+                                         dict args) except -1:
         """
         Internal method used for processing the parsed connect descriptor into
         the set of DescriptionList, Description, AddressList and Address
         container objects.
         """
         cdef:
+            DescriptionList description_list
             AddressList address_list
             Description description
             Address address
-        self.description_list = DescriptionList()
+        description_list = DescriptionList()
         list_args = args.get("description_list")
         if list_args is not None:
-            self.description_list.set_from_args(list_args)
+            description_list.set_from_args(list_args)
         else:
             list_args = args
         for desc_args in list_args.get("description", [list_args]):
             description = self._default_description.copy()
             description.set_from_description_args(desc_args)
-            self.description_list.children.append(description)
+            description_list.children.append(description)
             sub_args = desc_args.get("connect_data")
             if sub_args is not None:
                 description.set_from_connect_data_args(sub_args)
             sub_args = desc_args.get("security")
             if sub_args is not None:
                 description.set_from_security_args(sub_args)
             for list_args in desc_args.get("address_list", [desc_args]):
                 address_list = AddressList()
                 address_list.set_from_args(list_args)
                 description.children.append(address_list)
                 for addr_args in list_args.get("address", []):
                     address = self._default_address.copy()
                     address.set_from_args(addr_args)
                     address_list.children.append(address)
+        if not description_list.get_addresses():
+            errors._raise_err(errors.ERR_MISSING_ADDRESS,
+                              connect_string=connect_string)
+        self.description_list = description_list
 
     cdef int _set_access_token(self, object val, int error_num) except -1:
         """
         Sets the access token either supplied directly by the user or
         indirectly via a callback.
         """
         cdef:
@@ -509,21 +515,15 @@
         new_params._copy(self)
         return new_params
 
     def _get_addresses(self):
         """
         Return a list of the stored addresses.
         """
-        cdef:
-            AddressList addr_list
-            Description desc
-            Address addr
-        return [addr for desc in self.description_list.children \
-                for addr_list in desc.children \
-                for addr in addr_list.children]
+        return self.description_list.get_addresses()
 
     def get_connect_string(self):
         """
         Returns a connect string generated from the parameters.
         """
         return self.description_list.build_connect_string()
 
@@ -976,14 +976,26 @@
             Description d
             list parts
         parts = [d.build_connect_string() for d in self.children]
         if len(parts) == 1:
             return parts[0]
         return f'(DESCIPTION_LIST={"".join(parts)})'
 
+    cdef list get_addresses(self):
+        """
+        Return a list of the stored addresses.
+        """
+        cdef:
+            AddressList addr_list
+            Description desc
+            Address addr
+        return [addr for desc in self.children \
+                for addr_list in desc.children \
+                for addr in addr_list.children]
+
     def set_from_args(self, dict args):
         """
         Set paramter values from an argument dictionary or a (DESCRIPTION_LIST)
         node in a connect descriptor.
         """
         _set_bool_param(args, "failover", &self.failover)
         _set_bool_param(args, "load_balance", &self.load_balance)
```

### Comparing `oracledb-2.2.0/src/oracledb/impl/base/connection.pyx` & `oracledb-2.2.1/src/oracledb/impl/base/connection.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/base/constants.pxi` & `oracledb-2.2.1/src/oracledb/impl/base/constants.pxi`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/base/cursor.pyx` & `oracledb-2.2.1/src/oracledb/impl/base/cursor.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/base/dbobject.pyx` & `oracledb-2.2.1/src/oracledb/impl/base/dbobject.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/base/defaults.pyx` & `oracledb-2.2.1/src/oracledb/impl/base/defaults.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/base/lob.pyx` & `oracledb-2.2.1/src/oracledb/impl/base/lob.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/base/oson.pyx` & `oracledb-2.2.1/src/oracledb/impl/base/oson.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/base/pool.pyx` & `oracledb-2.2.1/src/oracledb/impl/base/pool.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/base/pool_params.pyx` & `oracledb-2.2.1/src/oracledb/impl/base/pool_params.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/base/queue.pyx` & `oracledb-2.2.1/src/oracledb/impl/base/queue.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/base/soda.pyx` & `oracledb-2.2.1/src/oracledb/impl/base/soda.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/base/subscr.pyx` & `oracledb-2.2.1/src/oracledb/impl/base/subscr.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/base/types.pyx` & `oracledb-2.2.1/src/oracledb/impl/base/types.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/base/utils.pyx` & `oracledb-2.2.1/src/oracledb/impl/base/utils.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/base/var.pyx` & `oracledb-2.2.1/src/oracledb/impl/base/var.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/base/vector.pyx` & `oracledb-2.2.1/src/oracledb/impl/base/vector.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/buffer.pyx` & `oracledb-2.2.1/src/oracledb/impl/thick/buffer.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/connection.pyx` & `oracledb-2.2.1/src/oracledb/impl/thick/connection.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/cursor.pyx` & `oracledb-2.2.1/src/oracledb/impl/thick/cursor.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/dbobject.pyx` & `oracledb-2.2.1/src/oracledb/impl/thick/dbobject.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/json.pyx` & `oracledb-2.2.1/src/oracledb/impl/thick/json.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/lob.pyx` & `oracledb-2.2.1/src/oracledb/impl/thick/lob.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/embed/dpi.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/embed/dpi.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/include/dpi.h` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/include/dpi.h`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiConn.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiConn.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiContext.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiContext.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiData.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiData.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiDebug.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiDebug.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiDeqOptions.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiDeqOptions.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiEnqOptions.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiEnqOptions.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiEnv.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiEnv.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiError.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiError.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiErrorMessages.h` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiErrorMessages.h`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiGen.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiGen.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiGlobal.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiGlobal.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiHandleList.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiHandleList.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiHandlePool.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiHandlePool.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiImpl.h` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiImpl.h`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiJson.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiJson.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiLob.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiLob.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiMsgProps.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiMsgProps.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiObject.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiObject.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiObjectAttr.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiObjectAttr.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiObjectType.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiObjectType.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiOci.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiOci.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiOracleType.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiOracleType.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiPool.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiPool.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiQueue.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiQueue.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiRowid.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiRowid.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiSodaColl.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiSodaColl.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiSodaCollCursor.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiSodaCollCursor.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiSodaDb.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiSodaDb.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiSodaDoc.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiSodaDoc.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiSodaDocCursor.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiSodaDocCursor.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiStmt.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiStmt.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiStringList.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiStringList.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiSubscr.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiSubscr.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiUtils.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiUtils.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiVar.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiVar.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi/src/dpiVector.c` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi/src/dpiVector.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/odpi.pxd` & `oracledb-2.2.1/src/oracledb/impl/thick/odpi.pxd`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/pool.pyx` & `oracledb-2.2.1/src/oracledb/impl/thick/pool.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/queue.pyx` & `oracledb-2.2.1/src/oracledb/impl/thick/queue.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/soda.pyx` & `oracledb-2.2.1/src/oracledb/impl/thick/soda.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/subscr.pyx` & `oracledb-2.2.1/src/oracledb/impl/thick/subscr.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/utils.pyx` & `oracledb-2.2.1/src/oracledb/impl/thick/utils.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thick/var.pyx` & `oracledb-2.2.1/src/oracledb/impl/thick/var.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thin/capabilities.pyx` & `oracledb-2.2.1/src/oracledb/impl/thin/capabilities.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thin/connection.pyx` & `oracledb-2.2.1/src/oracledb/impl/thin/connection.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thin/constants.pxi` & `oracledb-2.2.1/src/oracledb/impl/thin/constants.pxi`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thin/conversions.pyx` & `oracledb-2.2.1/src/oracledb/impl/thin/conversions.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thin/crypto.pyx` & `oracledb-2.2.1/src/oracledb/impl/thin/crypto.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thin/cursor.pyx` & `oracledb-2.2.1/src/oracledb/impl/thin/cursor.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thin/data_types.pyx` & `oracledb-2.2.1/src/oracledb/impl/thin/data_types.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thin/dbobject.pyx` & `oracledb-2.2.1/src/oracledb/impl/thin/dbobject.pyx`

 * *Files 7% similar despite different names*

```diff
@@ -90,14 +90,44 @@
         cdef uint8_t short_length
         self.read_ub1(&short_length)
         if short_length == TNS_LONG_LENGTH_INDICATOR:
             self.read_uint32(length)
         else:
             length[0] = short_length
 
+    cdef object read_xmltype(self, BaseThinConnImpl conn_impl):
+        """
+        Reads an XML type from the buffer. This is similar to reading a
+        database object but with specialized processing.
+        """
+        cdef:
+            uint8_t image_flags, image_version
+            BaseThinLobImpl lob_impl
+            const char_type *ptr
+            ssize_t bytes_left
+            uint32_t xml_flag
+            type cls
+        self.read_header(&image_flags, &image_version)
+        self.skip_raw_bytes(1)              # XML version
+        self.read_uint32(&xml_flag)
+        if xml_flag & TNS_XML_TYPE_FLAG_SKIP_NEXT_4:
+            self.skip_raw_bytes(4)
+        bytes_left = self.bytes_left()
+        ptr = self.read_raw_bytes(bytes_left)
+        if xml_flag & TNS_XML_TYPE_STRING:
+            return ptr[:bytes_left].decode()
+        elif xml_flag & TNS_XML_TYPE_LOB:
+            lob_impl = conn_impl._create_lob_impl(DB_TYPE_CLOB,
+                                                  ptr[:bytes_left])
+            cls = PY_TYPE_ASYNC_LOB \
+                if conn_impl._protocol._transport._is_async \
+                else PY_TYPE_LOB
+            return cls._from_impl(lob_impl)
+        errors._raise_err(errors.ERR_UNEXPECTED_XML_TYPE, flag=xml_flag)
+
     cdef int skip_length(self) except -1:
         """
         Skips the length instead of reading it from the buffer.
         """
         cdef uint8_t short_length
         self.read_ub1(&short_length)
         if short_length == TNS_LONG_LENGTH_INDICATOR:
@@ -325,14 +355,15 @@
                               int preferred_num_type):
         """
         Unpacks a single value and returns it.
         """
         cdef:
             uint8_t ora_type_num = dbtype._ora_type_num
             uint8_t csfrm = dbtype._csfrm
+            DbObjectPickleBuffer xml_buf
             BaseThinConnImpl conn_impl
             ThinDbObjectImpl obj_impl
             BaseThinLobImpl lob_impl
             bytes locator
             bint is_null
             type cls
         if ora_type_num == TNS_DATA_TYPE_NUMBER:
@@ -366,14 +397,18 @@
             return cls._from_impl(lob_impl)
         elif ora_type_num == TNS_DATA_TYPE_BOOLEAN:
             return buf.read_bool()
         elif ora_type_num == TNS_DATA_TYPE_INT_NAMED:
             buf.get_is_atomic_null(&is_null)
             if is_null:
                 return None
+            if objtype is None:
+                xml_buf = DbObjectPickleBuffer.__new__(DbObjectPickleBuffer)
+                xml_buf._populate_from_bytes(buf.read_bytes())
+                return xml_buf.read_xmltype(self.type._conn_impl)
             obj_impl = ThinDbObjectImpl.__new__(ThinDbObjectImpl)
             obj_impl.type = objtype
             if objtype.is_collection or self.type.is_collection:
                 obj_impl.packed_data = buf.read_bytes()
             else:
                 obj_impl._unpack_data_from_buf(buf)
             return PY_TYPE_DB_OBJECT._from_impl(obj_impl)
```

### Comparing `oracledb-2.2.0/src/oracledb/impl/thin/dbobject_cache.pyx` & `oracledb-2.2.1/src/oracledb/impl/thin/dbobject_cache.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -361,14 +361,48 @@
                 pass
         elif attr_type == TNS_OBJ_TDS_TYPE_END_EMBED_ADT:
             return None
         else:
             errors._raise_err(errors.ERR_TDS_TYPE_NOT_SUPPORTED, num=attr_type)
         return DbType._from_ora_type_and_csfrm(ora_type_num, csfrm)
 
+    cdef int _create_attr(self, ThinDbObjectTypeImpl typ_impl, str name,
+                          str type_name, str type_owner,
+                          str type_package_name=None, bytes oid=None,
+                          int8_t precision=0, int8_t scale=0,
+                          uint32_t max_size=0) except -1:
+        """
+        Creates an attribute from the supplied information and adds it to the
+        list of attributes for the type.
+        """
+        cdef:
+            ThinDbObjectTypeImpl attr_typ_impl
+            ThinDbObjectAttrImpl attr_impl
+        attr_impl = ThinDbObjectAttrImpl.__new__(ThinDbObjectAttrImpl)
+        attr_impl.name = name
+        if type_owner is not None:
+            attr_typ_impl = self.get_type_for_info(oid, type_owner,
+                                                   type_package_name,
+                                                   type_name)
+            if attr_typ_impl.is_xml_type:
+                attr_impl.dbtype = DB_TYPE_XMLTYPE
+            else:
+                attr_impl.dbtype = DB_TYPE_OBJECT
+                attr_impl.objtype = attr_typ_impl
+        else:
+            attr_impl.dbtype = DbType._from_ora_name(type_name)
+            attr_impl.max_size = max_size
+            if precision != 0 or scale != 0:
+                attr_impl.precision = precision
+                attr_impl.scale = scale
+                attr_impl._preferred_num_type = \
+                        get_preferred_num_type(precision, scale)
+        typ_impl.attrs.append(attr_impl)
+        typ_impl.attrs_by_name[name] = attr_impl
+
     cdef object _populate_type_info(self, str name, object attrs,
                                     ThinDbObjectTypeImpl typ_impl):
         """
         Populate the type information given the name of the type.
         """
         cdef:
             ssize_t start_pos, end_pos, name_length
@@ -385,56 +419,33 @@
             typ_impl.is_xml_type = \
                     (typ_impl.schema == "SYS" and typ_impl.name == "XMLTYPE")
         typ_impl.attrs = []
         typ_impl.attrs_by_name = {}
         if typ_impl.is_row_type:
             for name, data_type, data_type_owner, max_size, precision, \
                     scale in attrs:
-                attr_impl = ThinDbObjectAttrImpl.__new__(ThinDbObjectAttrImpl)
-                attr_impl.name = name
-                if data_type_owner is not None:
-                    attr_impl.dbtype = DB_TYPE_OBJECT
-                    attr_impl.objtype = self.get_type_for_info(None,
-                                                               data_type_owner,
-                                                               None,
-                                                               data_type)
-                else:
+                if data_type_owner is None:
                     start_pos = data_type.find("(")
                     if start_pos > 0:
                         end_pos = data_type.find(")")
                         if end_pos > start_pos:
                             data_type = data_type[:start_pos] + \
                                     data_type[end_pos + 1:]
-                    attr_impl.dbtype = DbType._from_ora_name(data_type)
-                    attr_impl.max_size = max_size
-                    attr_impl.precision = precision
-                    attr_impl.scale = scale
-                typ_impl.attrs.append(attr_impl)
-                typ_impl.attrs_by_name[name] = attr_impl
+                self._create_attr(typ_impl, name, data_type, data_type_owner,
+                                  None, None, precision, scale, max_size)
         else:
             for cursor_version, attr_name, attr_num, attr_type_name, \
                     attr_type_owner, attr_type_package, attr_type_oid, \
                     attr_instantiable, attr_super_type_owner, \
                     attr_super_type_name in attrs:
                 if attr_name is None:
                     continue
-                attr_impl = ThinDbObjectAttrImpl.__new__(ThinDbObjectAttrImpl)
-                attr_impl.name = attr_name
-                if attr_type_owner is not None:
-                    attr_impl.dbtype = DB_TYPE_OBJECT
-                    attr_impl.objtype = self.get_type_for_info(
-                        attr_type_oid,
-                        attr_type_owner,
-                        attr_type_package,
-                        attr_type_name
-                    )
-                else:
-                    attr_impl.dbtype = DbType._from_ora_name(attr_type_name)
-                typ_impl.attrs.append(attr_impl)
-                typ_impl.attrs_by_name[attr_name] = attr_impl
+                self._create_attr(typ_impl, attr_name, attr_type_name,
+                                  attr_type_owner, attr_type_package,
+                                  attr_type_oid)
             return self._parse_tds(typ_impl, self.tds_var.getvalue())
 
     cdef ThinDbObjectTypeImpl get_type_for_info(self, bytes oid, str schema,
                                                 str package_name, str name):
         """
         Returns a type for the specified fetch info, if one has already been
         cached. If not, a new type object is created and cached. It is also
```

### Comparing `oracledb-2.2.0/src/oracledb/impl/thin/lob.pyx` & `oracledb-2.2.1/src/oracledb/impl/thin/lob.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thin/messages.pyx` & `oracledb-2.2.1/src/oracledb/impl/thin/messages.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,15 @@
         """
         Gets the bit vector from the buffer and stores it for later use by the
         row processing code. Since it is possible that the packet buffer may be
         overwritten by subsequent packet retrieval, the bit vector must be
         copied. An array is stored and a pointer to the underlying memory is
         used for performance reasons.
         """
-        cdef const char_type *ptr = buf._get_raw(num_bytes)
+        cdef const char_type *ptr = buf.read_raw_bytes(num_bytes)
         if self.bit_vector_buf is None:
             self.bit_vector_buf = array.array('B')
             array.resize(self.bit_vector_buf, num_bytes)
         self.bit_vector = <const char_type*> self.bit_vector_buf.data.as_chars
         memcpy(<void*> self.bit_vector, ptr, num_bytes)
 
     cdef bint _is_duplicate_data(self, uint32_t column_num):
@@ -734,19 +734,18 @@
         type_handler = cursor_impl._get_output_type_handler(&uses_fetch_info)
         conn = self.cursor.connection
         for i in range(cursor_impl._num_columns):
             fetch_info = self._process_column_info(buf, cursor_impl)
             if prev_fetch_var_impls is not None \
                     and i < len(prev_fetch_var_impls):
                 self._adjust_fetch_info(prev_fetch_var_impls[i], fetch_info)
-            if not stmt._no_prefetch and \
-                    fetch_info.dbtype._ora_type_num in (TNS_DATA_TYPE_BLOB,
-                                                        TNS_DATA_TYPE_CLOB,
-                                                        TNS_DATA_TYPE_JSON,
-                                                        TNS_DATA_TYPE_VECTOR):
+            if fetch_info.dbtype._ora_type_num in (TNS_DATA_TYPE_BLOB,
+                                                   TNS_DATA_TYPE_CLOB,
+                                                   TNS_DATA_TYPE_JSON,
+                                                   TNS_DATA_TYPE_VECTOR):
                 stmt._requires_define = True
                 stmt._no_prefetch = True
             cursor_impl._create_fetch_var(conn, self.cursor, type_handler,
                                           uses_fetch_info, i, fetch_info)
         buf.read_ub4(&num_bytes)
         if num_bytes > 0:
             buf.skip_raw_bytes_chunked()    # current date
@@ -769,22 +768,25 @@
             BaseThinConnImpl conn_impl = self.conn_impl
             object exc_type
         Message._process_error_info(self, buf)
         if self.error_info.cursor_id != 0:
             cursor_impl._statement._cursor_id = self.error_info.cursor_id
         if not cursor_impl._statement._is_plsql and not self.in_fetch:
             cursor_impl.rowcount = self.error_info.rowcount
+        elif self.in_fetch and self.row_index > 0:
+            cursor_impl._statement._requires_define = False
         cursor_impl._lastrowid = self.error_info.rowid
         cursor_impl._batcherrors = self.error_info.batcherrors
         if self.batcherrors and cursor_impl._batcherrors is None:
             cursor_impl._batcherrors = []
         if self.error_info.num == TNS_ERR_NO_DATA_FOUND and self.in_fetch:
             self.error_info.num = 0
             cursor_impl._more_rows_to_fetch = False
             cursor_impl._last_row_index = 0
+            cursor_impl._statement._requires_define = False
             self.error_occurred = False
         elif self.error_info.num == TNS_ERR_ARRAY_DML_ERRORS:
             self.error_info.num = 0
             self.error_occurred = False
         elif self.retry:
             self.retry = False
         elif cursor_impl._statement._is_query \
@@ -1830,15 +1832,15 @@
             uint32_t flags = 0
             bytes db_uuid
         if buf._current_packet.packet_type == TNS_PACKET_TYPE_REDIRECT:
             if not self.read_redirect_data_len:
                 buf.read_uint16(&self.redirect_data_len)
                 self.read_redirect_data_len = True
             buf.wait_for_packets_sync()
-            redirect_data = buf._get_raw(self.redirect_data_len)
+            redirect_data = buf.read_raw_bytes(self.redirect_data_len)
             if self.redirect_data_len > 0:
                 self.redirect_data = \
                         redirect_data[:self.redirect_data_len].decode()
             self.read_redirect_data_len = False
         elif buf._current_packet.packet_type == TNS_PACKET_TYPE_ACCEPT:
             buf.read_uint16(&protocol_version)
             # check if the protocol version supported by the database is high
```

### Comparing `oracledb-2.2.0/src/oracledb/impl/thin/packet.pyx` & `oracledb-2.2.1/src/oracledb/impl/thin/packet.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -462,14 +462,22 @@
             lob_impl._chunk_size = chunk_size
             lob_impl._has_metadata = True
             cls = PY_TYPE_ASYNC_LOB \
                     if conn_impl._protocol._transport._is_async \
                     else PY_TYPE_LOB
             return cls._from_impl(lob_impl)
 
+    cdef const char_type* read_raw_bytes(self, ssize_t num_bytes) except NULL:
+        """
+        Read the specified number of bytes from the packet and return them.
+        """
+        self._chunked_bytes_buf.start_chunked_read()
+        self._get_raw(num_bytes, in_chunked_read=True)
+        return self._chunked_bytes_buf.end_chunked_read()
+
     cdef int read_rowid(self, Rowid *rowid) except -1:
         """
         Reads a rowid from the buffer and populates the rowid structure.
         """
         self.read_ub4(&rowid.rba)
         self.read_ub2(&rowid.partition_id)
         self.skip_ub1()
@@ -577,56 +585,32 @@
     cdef object read_xmltype(self, BaseThinConnImpl conn_impl):
         """
         Reads an XMLType value from the buffer and returns the string value.
         The XMLType object is a special DbObjectType and is handled separately
         since the structure is a bit different.
         """
         cdef:
-            uint8_t image_flags, image_version
             DbObjectPickleBuffer buf
-            BaseThinLobImpl lob_impl
-            const char_type *ptr
             uint32_t num_bytes
-            ssize_t bytes_left
-            uint32_t xml_flag
-            bytes packed_data
-            type cls
         self.read_ub4(&num_bytes)
         if num_bytes > 0:                   # type OID
             self.read_bytes()
         self.read_ub4(&num_bytes)
         if num_bytes > 0:                   # OID
             self.read_bytes()
         self.read_ub4(&num_bytes)
         if num_bytes > 0:                   # snapshot
             self.read_bytes()
         self.skip_ub2()                     # version
         self.read_ub4(&num_bytes)           # length of data
         self.skip_ub2()                     # flags
         if num_bytes > 0:
-            packed_data = self.read_bytes()
             buf = DbObjectPickleBuffer.__new__(DbObjectPickleBuffer)
-            buf._populate_from_bytes(packed_data)
-            buf.read_header(&image_flags, &image_version)
-            buf.skip_raw_bytes(1)           # XML version
-            buf.read_uint32(&xml_flag)
-            if xml_flag & TNS_XML_TYPE_FLAG_SKIP_NEXT_4:
-                buf.skip_raw_bytes(4)
-            bytes_left = buf.bytes_left()
-            ptr = buf.read_raw_bytes(bytes_left)
-            if xml_flag & TNS_XML_TYPE_STRING:
-                return ptr[:bytes_left].decode()
-            elif xml_flag & TNS_XML_TYPE_LOB:
-                lob_impl = conn_impl._create_lob_impl(DB_TYPE_CLOB,
-                                                      ptr[:bytes_left])
-                cls = PY_TYPE_ASYNC_LOB \
-                    if conn_impl._protocol._transport._is_async \
-                    else PY_TYPE_LOB
-                return cls._from_impl(lob_impl)
-            errors._raise_err(errors.ERR_UNEXPECTED_XML_TYPE, flag=xml_flag)
+            buf._populate_from_bytes(self.read_bytes())
+            return buf.read_xmltype(conn_impl)
 
     cdef int check_control_packet(self) except -1:
         """
         Checks for a control packet or final close packet from the server.
         """
         cdef:
             bint notify_waiter
```

### Comparing `oracledb-2.2.0/src/oracledb/impl/thin/pool.pyx` & `oracledb-2.2.1/src/oracledb/impl/thin/pool.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thin/protocol.pyx` & `oracledb-2.2.1/src/oracledb/impl/thin/protocol.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -462,30 +462,32 @@
             else:
                 ptr = buf.read_raw_bytes(refuse_message_len)
                 message.error_info.message = ptr[:refuse_message_len].decode()
 
     cdef int _reset(self, Message message) except -1:
         cdef uint8_t marker_type, packet_type
 
-        # read and discard all packets until a marker packet is received
+        # send reset marker
+        self._send_marker(self._write_buf, TNS_MARKER_TYPE_RESET)
+
+        # read and discard all packets until a reset marker is received
         while True:
             packet_type = self._read_buf._current_packet.packet_type
             if packet_type == TNS_PACKET_TYPE_MARKER:
                 self._read_buf.skip_raw_bytes(2)
                 self._read_buf.read_ub1(&marker_type)
                 if marker_type == TNS_MARKER_TYPE_RESET:
                     break
             self._read_buf.wait_for_packets_sync()
 
-        # send reset marker and then read error packet; first skip as many
-        # marker packets as may be sent by the server; if the server doesn't
-        # handle out-of-band breaks properly, some quit immediately and others
-        # send multiple reset markers (this addresses both situations without
-        # resulting in strange errors)
-        self._send_marker(self._write_buf, TNS_MARKER_TYPE_RESET)
+        # read error packet; first skip as many marker packets as may be sent
+        # by the server; if the server doesn't handle out-of-band breaks
+        # properly, some quit immediately and others send multiple reset
+        # markers (this addresses both situations without resulting in strange
+        # errors)
         while packet_type == TNS_PACKET_TYPE_MARKER:
             self._read_buf.wait_for_packets_sync()
             packet_type = self._read_buf._current_packet.packet_type
         self._break_in_progress = False
 
 
 cdef class BaseAsyncProtocol(BaseProtocol):
@@ -838,30 +840,32 @@
             else:
                 ptr = buf.read_raw_bytes(refuse_message_len)
                 message.error_info.message = ptr[:refuse_message_len].decode()
 
     async def _reset(self):
         cdef uint8_t marker_type, packet_type
 
-        # read and discard all packets until a marker packet is received
+        # send reset marker
+        self._send_marker(self._write_buf, TNS_MARKER_TYPE_RESET)
+
+        # read and discard all packets until a reset marker is received
         while True:
             packet_type = self._read_buf._current_packet.packet_type
             if packet_type == TNS_PACKET_TYPE_MARKER:
                 self._read_buf.skip_raw_bytes(2)
                 self._read_buf.read_ub1(&marker_type)
                 if marker_type == TNS_MARKER_TYPE_RESET:
                     break
             await self._read_buf.wait_for_packets_async()
 
-        # send reset marker and then read error packet; first skip as many
-        # marker packets as may be sent by the server; if the server doesn't
-        # handle out-of-band breaks properly, some quit immediately and others
-        # send multiple reset markers (this addresses both situations without
-        # resulting in strange errors)
-        self._send_marker(self._write_buf, TNS_MARKER_TYPE_RESET)
+        # read error packet; first skip as many marker packets as may be sent
+        # by the server; if the server doesn't handle out-of-band breaks
+        # properly, some quit immediately and others send multiple reset
+        # markers (this addresses both situations without resulting in strange
+        # errors)
         while packet_type == TNS_PACKET_TYPE_MARKER:
             await self._read_buf.wait_for_packets_async()
             packet_type = self._read_buf._current_packet.packet_type
         self._break_in_progress = False
 
     def connection_lost(self, exc):
         """
```

### Comparing `oracledb-2.2.0/src/oracledb/impl/thin/statement.pyx` & `oracledb-2.2.1/src/oracledb/impl/thin/statement.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thin/statement_cache.pyx` & `oracledb-2.2.1/src/oracledb/impl/thin/statement_cache.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -128,21 +128,25 @@
         return stmt
 
     cdef int initialize(self, uint32_t max_size,
                          uint32_t max_cursors) except -1:
         """
         Initialize the statement cache.
         """
-        self._max_size = max_size
-        self._max_cursors = max_cursors
+        if max_cursors == 0:
+            self._max_size = 0
+            self._max_cursors = 1
+        else:
+            self._max_size = max_size
+            self._max_cursors = max_cursors
         self._cached_statements = collections.OrderedDict()
         self._lock = threading.Lock()
         self._open_cursors = set()
         self._cursors_to_close = array.array('I')
-        array.resize(self._cursors_to_close, max_cursors)
+        array.resize(self._cursors_to_close, self._max_cursors)
         self._num_cursors_to_close = 0
 
     cdef int resize(self, uint32_t new_size) except -1:
         """
         Resizes the statement cache to the new value.
         """
         with self._lock:
```

### Comparing `oracledb-2.2.0/src/oracledb/impl/thin/transport.pyx` & `oracledb-2.2.1/src/oracledb/impl/thin/transport.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,17 @@
                                          description.ssl_server_cert_dn):
                 errors._raise_err(errors.ERR_INVALID_SERVER_CERT_DN)
 
     cdef int renegotiate_tls(self, Description description) except -1:
         """
         Renegotiate TLS on the socket.
         """
-        sock = socket.socket(fileno=self._transport.detach())
+        orig_sock = self._transport
+        sock = socket.socket(family=orig_sock.family, type=orig_sock.type,
+                             proto=orig_sock.proto, fileno=orig_sock.detach())
         self.negotiate_tls(sock, description)
 
     async def negotiate_tls_async(self, BaseAsyncProtocol protocol,
                                   Description description):
         """
         Negotiate TLS on the socket asynchronously.
         """
```

### Comparing `oracledb-2.2.0/src/oracledb/impl/thin/utils.pyx` & `oracledb-2.2.1/src/oracledb/impl/thin/utils.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/impl/thin/var.pyx` & `oracledb-2.2.1/src/oracledb/impl/thin/var.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/lob.py` & `oracledb-2.2.1/src/oracledb/lob.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/pool.py` & `oracledb-2.2.1/src/oracledb/pool.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/pool_params.py` & `oracledb-2.2.1/src/oracledb/pool_params.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/soda.py` & `oracledb-2.2.1/src/oracledb/soda.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/subscr.py` & `oracledb-2.2.1/src/oracledb/subscr.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/thick_impl.pyx` & `oracledb-2.2.1/src/oracledb/thick_impl.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/thin_impl.pyx` & `oracledb-2.2.1/src/oracledb/thin_impl.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/utils.py` & `oracledb-2.2.1/src/oracledb/utils.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/var.py` & `oracledb-2.2.1/src/oracledb/var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/src/oracledb/version.py` & `oracledb-2.2.1/src/oracledb/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 # version.py
 #
 # Defines the version of the package. This is the only place where this is
 # found. The setup.cfg configuration file and the documentation configuration
 # file doc/src/conf.py both reference this file directly.
 # -----------------------------------------------------------------------------
 
-__version__ = "2.2.0"
+__version__ = "2.2.1"
```

### Comparing `oracledb-2.2.0/src/oracledb.egg-info/PKG-INFO` & `oracledb-2.2.1/src/oracledb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oracledb
-Version: 2.2.0
+Version: 2.2.1
 Summary: Python interface to Oracle Database
 Home-page: https://oracle.github.io/python-oracledb
 Author: Anthony Tuininga
 Author-email: anthony.tuininga@oracle.com
 License: Apache and/or UPL
 Project-URL: Installation, https://python-oracledb.readthedocs.io/en/latest/user_guide/installation.html
 Project-URL: Samples, https://github.com/oracle/python-oracledb/tree/main/samples
```

### Comparing `oracledb-2.2.0/src/oracledb.egg-info/SOURCES.txt` & `oracledb-2.2.1/src/oracledb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/create_schema.py` & `oracledb-2.2.1/tests/create_schema.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/drop_schema.py` & `oracledb-2.2.1/tests/drop_schema.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_1000_module.py` & `oracledb-2.2.1/tests/test_1000_module.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_1100_connection.py` & `oracledb-2.2.1/tests/test_1100_connection.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_1300_cursor_var.py` & `oracledb-2.2.1/tests/test_1300_cursor_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_1400_datetime_var.py` & `oracledb-2.2.1/tests/test_1400_datetime_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_1500_types.py` & `oracledb-2.2.1/tests/test_1500_types.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_1600_dml_returning.py` & `oracledb-2.2.1/tests/test_1600_dml_returning.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_1700_error.py` & `oracledb-2.2.1/tests/test_1700_error.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_1800_interval_var.py` & `oracledb-2.2.1/tests/test_1800_interval_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_1900_lob_var.py` & `oracledb-2.2.1/tests/test_1900_lob_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_2000_long_var.py` & `oracledb-2.2.1/tests/test_2000_long_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_2100_nchar_var.py` & `oracledb-2.2.1/tests/test_2100_nchar_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_2200_number_var.py` & `oracledb-2.2.1/tests/test_2200_number_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_2300_object_var.py` & `oracledb-2.2.1/tests/test_2300_object_var.py`

 * *Files 4% similar despite different names*

```diff
@@ -656,30 +656,24 @@
             running_total += i + 1
             obj.append(running_total)
         result = self.cursor.callfunc(
             "pkg_TestNumberArrays.TestInArrays", int, (2327, obj)
         )
         self.assertEqual(result, 7146445847327)
 
-    @unittest.skipIf(
-        test_env.get_is_thin(),
-        "thin mode doesn't have any unknown types currently",
-    )
+    @unittest.skipIf(test_env.get_is_thin(), "thin mode supports xmltype")
     def test_2328(self):
         "2328 - test object with unknown type in one of its attributes"
-        typ = self.conn.gettype("UDT_UNKNOWNATTRIBUTETYPE")
+        typ = self.conn.gettype("UDT_OBJECTWITHXMLTYPE")
         self.assertEqual(typ.attributes[1].type, oracledb.DB_TYPE_UNKNOWN)
 
-    @unittest.skipIf(
-        test_env.get_is_thin(),
-        "thin mode doesn't have any unknown types currently",
-    )
+    @unittest.skipIf(test_env.get_is_thin(), "thin mode supports xmltype")
     def test_2329(self):
         "2329 - test object with unknown type as the element type"
-        typ = self.conn.gettype("UDT_UNKNOWNELEMENTTYPE")
+        typ = self.conn.gettype("UDT_XMLTYPEARRAY")
         self.assertEqual(typ.element_type, oracledb.DB_TYPE_UNKNOWN)
 
     def test_2330(self):
         "2330 - test DB Object repr()"
         typ = self.conn.gettype("UDT_ARRAY")
         obj = typ.newobject()
         fqn = f"{typ.schema}.{typ.name}"
@@ -786,10 +780,29 @@
     def test_2338(self):
         "2338 - test collection iteration"
         self.cursor.execute("select udt_array(5, 10, 15) from dual")
         (obj,) = self.cursor.fetchone()
         result = [i for i in obj]
         self.assertEqual(result, [5, 10, 15])
 
+    @unittest.skipUnless(
+        test_env.get_is_thin(), "thick mode does not support xmltype"
+    )
+    def test_2339(self):
+        "2339 - test fetching an object containing an XmlType instance"
+        num_val = 2339
+        xml_val = "<item>test_2339</item>"
+        str_val = "A string for test 2339"
+        self.cursor.execute(
+            f"""
+            select udt_ObjectWithXmlType({num_val}, sys.xmltype('{xml_val}'),
+                    '{str_val}') from dual
+            """
+        )
+        (obj,) = self.cursor.fetchone()
+        self.assertEqual(obj.NUMBERVALUE, num_val)
+        self.assertEqual(obj.XMLVALUE, xml_val)
+        self.assertEqual(obj.STRINGVALUE, str_val)
+
 
 if __name__ == "__main__":
     test_env.run_test_cases()
```

### Comparing `oracledb-2.2.0/tests/test_2400_pool.py` & `oracledb-2.2.1/tests/test_2400_pool.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_2500_string_var.py` & `oracledb-2.2.1/tests/test_2500_string_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_2600_timestamp_var.py` & `oracledb-2.2.1/tests/test_2600_timestamp_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_2700_aq.py` & `oracledb-2.2.1/tests/test_2700_aq.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_2800_bulk_aq.py` & `oracledb-2.2.1/tests/test_2800_bulk_aq.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_2900_rowid.py` & `oracledb-2.2.1/tests/test_2900_rowid.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_3000_subscription.py` & `oracledb-2.2.1/tests/test_3000_subscription.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_3100_boolean_var.py` & `oracledb-2.2.1/tests/test_3100_boolean_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_3200_features_12_1.py` & `oracledb-2.2.1/tests/test_3200_features_12_1.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_3300_soda_database.py` & `oracledb-2.2.1/tests/test_3300_soda_database.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_3400_soda_collection.py` & `oracledb-2.2.1/tests/test_3400_soda_collection.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_3500_json.py` & `oracledb-2.2.1/tests/test_3500_json.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_3600_outputtypehandler.py` & `oracledb-2.2.1/tests/test_3600_outputtypehandler.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_3700_var.py` & `oracledb-2.2.1/tests/test_3700_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_3800_typehandler.py` & `oracledb-2.2.1/tests/test_3800_typehandler.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_3900_cursor_execute.py` & `oracledb-2.2.1/tests/test_3900_cursor_execute.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_4000_cursor_executemany.py` & `oracledb-2.2.1/tests/test_4000_cursor_executemany.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_4100_cursor_callproc.py` & `oracledb-2.2.1/tests/test_4100_cursor_callproc.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_4200_cursor_scrollable.py` & `oracledb-2.2.1/tests/test_4200_cursor_scrollable.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_4300_cursor_other.py` & `oracledb-2.2.1/tests/test_4300_cursor_other.py`

 * *Files 1% similar despite different names*

```diff
@@ -973,10 +973,25 @@
         with self.assertRaisesFullCode("DPY-2045"):
             self.cursor.arraysize = 0
         with self.assertRaisesFullCode("DPY-2045"):
             self.cursor.arraysize = -1
         with self.assertRaisesFullCode("DPY-2045"):
             self.cursor.arraysize = "not valid"
 
+    def test_4366(self):
+        "4366 - test fetching LOBs after an error"
+        sql = """
+            select
+                to_clob(:val),
+                1 / (dbms_lob.getlength(to_clob(:val)) - 1)
+            from dual"""
+        with self.assertRaisesFullCode("ORA-01476"):
+            self.cursor.execute(sql, val="a")
+            self.cursor.fetchall()
+        self.cursor.execute(sql, val="bb")
+        lob, num_val = self.cursor.fetchone()
+        self.assertEqual(lob.read(), "bb")
+        self.assertEqual(num_val, 1)
+
 
 if __name__ == "__main__":
     test_env.run_test_cases()
```

### Comparing `oracledb-2.2.0/tests/test_4400_tpc.py` & `oracledb-2.2.1/tests/test_4400_tpc.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_4500_connect_params.py` & `oracledb-2.2.1/tests/test_4500_connect_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -725,10 +725,38 @@
         params.set(use_tcp_fast_open="False")
         self.assertFalse(params.use_tcp_fast_open)
         params.set(use_tcp_fast_open=None)
         self.assertFalse(params.use_tcp_fast_open)
         params.set(use_tcp_fast_open=1)
         self.assertTrue(params.use_tcp_fast_open)
 
+    def test_4546(self):
+        "4546 - test connect descriptor without addresses defined"
+        params = oracledb.ConnectParams()
+        host = "host_4546"
+        port = 4546
+        service_name = "service_name_4546"
+        ok_container_names = ("DESCRIPTION", "ADDRESS")
+        options = [
+            ("DESRIPTION", "ADDRESS"),
+            ok_container_names,
+            ("DESCRIPTION", "ADRESS"),
+        ]
+        for option in options:
+            desc_name, addr_name = option
+            connect_string = (
+                f"({desc_name}=({addr_name}=(PROTOCOL=TCP)(HOST={host})"
+                f"(PORT={port}))(CONNECT_DATA=(SERVICE_NAME={service_name})))"
+            )
+            params = oracledb.ConnectParams()
+            if option == ok_container_names:
+                params.parse_connect_string(connect_string)
+                self.assertEqual(params.host, host)
+                self.assertEqual(params.port, port)
+                self.assertEqual(params.service_name, service_name)
+            else:
+                with self.assertRaisesFullCode("DPY-2049"):
+                    params.parse_connect_string(connect_string)
+
 
 if __name__ == "__main__":
     test_env.run_test_cases()
```

### Comparing `oracledb-2.2.0/tests/test_4600_type_changes.py` & `oracledb-2.2.1/tests/test_4600_type_changes.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_4700_pool_params.py` & `oracledb-2.2.1/tests/test_4700_pool_params.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_4800_timestamp_ltz_var.py` & `oracledb-2.2.1/tests/test_4800_timestamp_ltz_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_4900_timestamp_tz_var.py` & `oracledb-2.2.1/tests/test_4900_timestamp_tz_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_5000_externalauth.py` & `oracledb-2.2.1/tests/test_5000_externalauth.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_5100_arrayvar.py` & `oracledb-2.2.1/tests/test_5100_arrayvar.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_5200_sql_parser.py` & `oracledb-2.2.1/tests/test_5200_sql_parser.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_5300_connection_async.py` & `oracledb-2.2.1/tests/test_5300_connection_async.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_5400_cursor_execute_async.py` & `oracledb-2.2.1/tests/test_5400_cursor_execute_async.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_5500_pool_async.py` & `oracledb-2.2.1/tests/test_5500_pool_async.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_5600_dbobject_async.py` & `oracledb-2.2.1/tests/test_5600_dbobject_async.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_5700_lob_var_async.py` & `oracledb-2.2.1/tests/test_5700_lob_var_async.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_5800_cursor_var_async.py` & `oracledb-2.2.1/tests/test_5800_cursor_var_async.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_5900_dml_returning_async.py` & `oracledb-2.2.1/tests/test_5900_dml_returning_async.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_6000_typehandler_async.py` & `oracledb-2.2.1/tests/test_6000_typehandler_async.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_6100_cursor_executemany_async.py` & `oracledb-2.2.1/tests/test_6100_cursor_executemany_async.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_6200_cursor_callproc_async.py` & `oracledb-2.2.1/tests/test_6200_cursor_callproc_async.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_6300_cursor_other_async.py` & `oracledb-2.2.1/tests/test_6300_cursor_other_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -840,10 +840,24 @@
         expected_annotations = {
             "ANNO_1": "first annotation",
             "ANNO_2": "second annotation",
             "ANNO_3": "",
         }
         self.assertEqual(column_2.annotations, expected_annotations)
 
+    async def test_6348(self):
+        "6348 - test fetching LOBs after an error"
+        sql = """
+            select
+                to_clob(:val),
+                1 / (dbms_lob.getlength(to_clob(:val)) - 1)
+            from dual"""
+        with self.assertRaisesFullCode("ORA-01476"):
+            await self.cursor.execute(sql, val="a")
+        await self.cursor.execute(sql, val="bb")
+        lob, num_val = await self.cursor.fetchone()
+        self.assertEqual(await lob.read(), "bb")
+        self.assertEqual(num_val, 1)
+
 
 if __name__ == "__main__":
     test_env.run_test_cases()
```

### Comparing `oracledb-2.2.0/tests/test_6400_vector_var.py` & `oracledb-2.2.1/tests/test_6400_vector_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_6500_vector_interop.py` & `oracledb-2.2.1/tests/test_6500_vector_interop.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_6600_defaults.py` & `oracledb-2.2.1/tests/test_6600_defaults.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_6700_json_23.py` & `oracledb-2.2.1/tests/test_6700_json_23.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_6800_error_async.py` & `oracledb-2.2.1/tests/test_6800_error_async.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_6900_oson.py` & `oracledb-2.2.1/tests/test_6900_oson.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_7000_connection_async_shortcut_methods.py` & `oracledb-2.2.1/tests/test_7000_connection_async_shortcut_methods.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_7100_interval_ym_var.py` & `oracledb-2.2.1/tests/test_7100_interval_ym_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_7200_tnsnames.py` & `oracledb-2.2.1/tests/test_7200_tnsnames.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_7300_unsupported_features_thin.py` & `oracledb-2.2.1/tests/test_7300_unsupported_features_thin.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tests/test_env.py` & `oracledb-2.2.1/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.2.0/tox.ini` & `oracledb-2.2.1/tox.ini`

 * *Files identical despite different names*

