# Comparing `tmp/pycitysim-1.13.0.tar.gz` & `tmp/pycitysim-1.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycitysim-1.13.0.tar", last modified: Sun May 19 17:29:20 2024, max compression
+gzip compressed data, was "pycitysim-1.14.0.tar", last modified: Mon May 27 06:56:08 2024, max compression
```

## Comparing `pycitysim-1.13.0.tar` & `pycitysim-1.14.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:29:20.603683 pycitysim-1.13.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-19 17:29:14.000000 pycitysim-1.13.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-19 17:29:20.603683 pycitysim-1.13.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-19 17:29:14.000000 pycitysim-1.13.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:29:20.595683 pycitysim-1.13.0/pycitysim/
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:29:20.595683 pycitysim-1.13.0/pycitysim/apphub/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/apphub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/apphub/apphub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:29:20.595683 pycitysim-1.13.0/pycitysim/map/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37630 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/map/map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:29:20.599683 pycitysim-1.13.0/pycitysim/routing/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/routing/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:29:20.599683 pycitysim-1.13.0/pycitysim/sidecar/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sidecar/sidecar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:29:20.599683 pycitysim-1.13.0/pycitysim/sim/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sim/aoi_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sim/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sim/clock_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sim/economy_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sim/event_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sim/lane_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sim/light_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sim/person_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sim/road_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sim/social_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:29:20.599683 pycitysim-1.13.0/pycitysim/urbankg/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/urbankg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/urbankg/kg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:29:20.599683 pycitysim-1.13.0/pycitysim/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/utils/geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/utils/grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/utils/protobuf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:29:20.603683 pycitysim-1.13.0/pycitysim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-19 17:29:20.000000 pycitysim-1.13.0/pycitysim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-19 17:29:20.000000 pycitysim-1.13.0/pycitysim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:29:20.000000 pycitysim-1.13.0/pycitysim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-19 17:29:20.000000 pycitysim-1.13.0/pycitysim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 17:29:20.000000 pycitysim-1.13.0/pycitysim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 17:29:20.603683 pycitysim-1.13.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:56:08.891726 pycitysim-1.14.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-27 06:56:02.000000 pycitysim-1.14.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-27 06:56:08.891726 pycitysim-1.14.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-27 06:56:02.000000 pycitysim-1.14.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:56:08.883726 pycitysim-1.14.0/pycitysim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:56:08.887726 pycitysim-1.14.0/pycitysim/apphub/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/apphub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/apphub/apphub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:56:08.887726 pycitysim-1.14.0/pycitysim/map/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37630 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/map/map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:56:08.887726 pycitysim-1.14.0/pycitysim/routing/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/routing/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:56:08.887726 pycitysim-1.14.0/pycitysim/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/sidecar/sidecar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:56:08.887726 pycitysim-1.14.0/pycitysim/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/sim/aoi_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/sim/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/sim/clock_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/sim/economy_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/sim/event_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/sim/lane_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/sim/light_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/sim/person_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/sim/road_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/sim/social_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:56:08.887726 pycitysim-1.14.0/pycitysim/urbankg/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/urbankg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/urbankg/kg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:56:08.891726 pycitysim-1.14.0/pycitysim/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/utils/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/utils/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pycitysim/utils/protobuf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:56:08.891726 pycitysim-1.14.0/pycitysim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-27 06:56:08.000000 pycitysim-1.14.0/pycitysim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-27 06:56:08.000000 pycitysim-1.14.0/pycitysim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 06:56:08.000000 pycitysim-1.14.0/pycitysim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-27 06:56:08.000000 pycitysim-1.14.0/pycitysim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 06:56:08.000000 pycitysim-1.14.0/pycitysim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-27 06:56:02.000000 pycitysim-1.14.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 06:56:08.891726 pycitysim-1.14.0/setup.cfg
```

### Comparing `pycitysim-1.13.0/LICENSE` & `pycitysim-1.14.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycitysim-1.13.0/PKG-INFO` & `pycitysim-1.14.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycitysim
-Version: 1.13.0
+Version: 1.14.0
 Summary: City Simulator and OpenCity Databases Python SDK
 Author-email: Jun Zhang <zhangjun990222@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,15 +37,15 @@
 License-File: LICENSE
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: geojson>=3.1.0
 Requires-Dist: grpcio<2.0.0,>=1.42.0
 Requires-Dist: lru-dict>=1.3.0
 Requires-Dist: numpy>=1.24.0
 Requires-Dist: Pillow>=10.0.0
-Requires-Dist: pycityproto==1.13.1
+Requires-Dist: pycityproto==1.14.0
 Requires-Dist: pymongo>=3.12.1
 Requires-Dist: pyproj>=3.0.0
 Requires-Dist: shapely>=2.0.0
 
 # pycitysim
 
 City Simulator and OpenCity databases Python SDK
```

### Comparing `pycitysim-1.13.0/README.md` & `pycitysim-1.14.0/README.md`

 * *Files identical despite different names*

### Comparing `pycitysim-1.13.0/pycitysim/__init__.py` & `pycitysim-1.14.0/pycitysim/__init__.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.13.0/pycitysim/apphub/apphub.py` & `pycitysim-1.14.0/pycitysim/apphub/apphub.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.13.0/pycitysim/map/map.py` & `pycitysim-1.14.0/pycitysim/map/map.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.13.0/pycitysim/routing/client.py` & `pycitysim-1.14.0/pycitysim/routing/client.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.13.0/pycitysim/sidecar/sidecar.py` & `pycitysim-1.14.0/pycitysim/sidecar/sidecar.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.13.0/pycitysim/sim/__init__.py` & `pycitysim-1.14.0/pycitysim/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.13.0/pycitysim/sim/aoi_service.py` & `pycitysim-1.14.0/pycitysim/sim/aoi_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.13.0/pycitysim/sim/client.py` & `pycitysim-1.14.0/pycitysim/sim/client.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.13.0/pycitysim/sim/clock_service.py` & `pycitysim-1.14.0/pycitysim/sim/clock_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.13.0/pycitysim/sim/economy_services.py` & `pycitysim-1.14.0/pycitysim/sim/economy_services.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.13.0/pycitysim/sim/event_service.py` & `pycitysim-1.14.0/pycitysim/sim/event_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.13.0/pycitysim/sim/lane_service.py` & `pycitysim-1.14.0/pycitysim/sim/lane_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.13.0/pycitysim/sim/light_service.py` & `pycitysim-1.14.0/pycitysim/sim/light_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.13.0/pycitysim/sim/road_service.py` & `pycitysim-1.14.0/pycitysim/sim/road_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.13.0/pycitysim/sim/social_service.py` & `pycitysim-1.14.0/pycitysim/sim/social_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.13.0/pycitysim/urbankg/kg.py` & `pycitysim-1.14.0/pycitysim/urbankg/kg.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.13.0/pycitysim/utils/geojson.py` & `pycitysim-1.14.0/pycitysim/utils/geojson.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.13.0/pycitysim/utils/grpc.py` & `pycitysim-1.14.0/pycitysim/utils/grpc.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.13.0/pycitysim/utils/protobuf.py` & `pycitysim-1.14.0/pycitysim/utils/protobuf.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.13.0/pycitysim.egg-info/PKG-INFO` & `pycitysim-1.14.0/pycitysim.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycitysim
-Version: 1.13.0
+Version: 1.14.0
 Summary: City Simulator and OpenCity Databases Python SDK
 Author-email: Jun Zhang <zhangjun990222@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,15 +37,15 @@
 License-File: LICENSE
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: geojson>=3.1.0
 Requires-Dist: grpcio<2.0.0,>=1.42.0
 Requires-Dist: lru-dict>=1.3.0
 Requires-Dist: numpy>=1.24.0
 Requires-Dist: Pillow>=10.0.0
-Requires-Dist: pycityproto==1.13.1
+Requires-Dist: pycityproto==1.14.0
 Requires-Dist: pymongo>=3.12.1
 Requires-Dist: pyproj>=3.0.0
 Requires-Dist: shapely>=2.0.0
 
 # pycitysim
 
 City Simulator and OpenCity databases Python SDK
```

### Comparing `pycitysim-1.13.0/pycitysim.egg-info/SOURCES.txt` & `pycitysim-1.14.0/pycitysim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycitysim-1.13.0/pyproject.toml` & `pycitysim-1.14.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 dependencies = [
     'importlib-metadata; python_version<"3.8"',
     "geojson >= 3.1.0",
     "grpcio >= 1.42.0, < 2.0.0",
     "lru-dict >= 1.3.0",
     "numpy >= 1.24.0",
     "Pillow >= 10.0.0",
-    "pycityproto == 1.13.1",
+    "pycityproto == 1.14.0",
     "pymongo >= 3.12.1",
     "pyproj >= 3.0.0",
     "shapely >= 2.0.0",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
```

