# Comparing `tmp/brapi_proxy-0.0.6.tar.gz` & `tmp/brapi_proxy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brapi_proxy-0.0.6.tar", last modified: Thu May 23 12:24:23 2024, max compression
+gzip compressed data, was "brapi_proxy-0.0.7.tar", last modified: Mon May 27 07:49:55 2024, max compression
```

## Comparing `brapi_proxy-0.0.6.tar` & `brapi_proxy-0.0.7.tar`

### file list

```diff
@@ -1,37 +1,43 @@
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 12:24:23.494790 brapi_proxy-0.0.6/
--rw-r--r--   0 matthijs   (501) staff       (20)     1079 2024-05-23 06:09:10.000000 brapi_proxy-0.0.6/LICENSE
--rw-r--r--   0 matthijs   (501) staff       (20)     4980 2024-05-23 12:24:23.494434 brapi_proxy-0.0.6/PKG-INFO
--rw-r--r--   0 matthijs   (501) staff       (20)     3002 2024-05-23 11:37:23.000000 brapi_proxy-0.0.6/README.md
--rw-r--r--   0 matthijs   (501) staff       (20)     1038 2024-05-23 09:26:28.000000 brapi_proxy-0.0.6/pyproject.toml
--rw-r--r--   0 matthijs   (501) staff       (20)       65 2024-05-22 18:03:35.000000 brapi_proxy-0.0.6/requirements.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       38 2024-05-23 12:24:23.494859 brapi_proxy-0.0.6/setup.cfg
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 12:24:23.485124 brapi_proxy-0.0.6/src/
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 12:24:23.488037 brapi_proxy-0.0.6/src/brapi_proxy/
--rw-r--r--   0 matthijs   (501) staff       (20)       85 2024-05-21 08:26:30.000000 brapi_proxy-0.0.6/src/brapi_proxy/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)       22 2024-05-23 12:23:20.000000 brapi_proxy-0.0.6/src/brapi_proxy/_version.py
--rw-r--r--   0 matthijs   (501) staff       (20)     8959 2024-05-23 12:21:14.000000 brapi_proxy-0.0.6/src/brapi_proxy/brapi.py
--rw-r--r--   0 matthijs   (501) staff       (20)      780 2024-05-23 11:50:06.000000 brapi_proxy-0.0.6/src/brapi_proxy/config_demo.ini
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 12:24:23.490739 brapi_proxy-0.0.6/src/brapi_proxy/core/
--rw-r--r--   0 matthijs   (501) staff       (20)      607 2024-05-21 08:29:31.000000 brapi_proxy-0.0.6/src/brapi_proxy/core/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)     1921 2024-05-22 17:35:55.000000 brapi_proxy-0.0.6/src/brapi_proxy/core/core_commoncropnames.py
--rw-r--r--   0 matthijs   (501) staff       (20)     2432 2024-05-22 17:35:22.000000 brapi_proxy-0.0.6/src/brapi_proxy/core/core_serverinfo.py
--rw-r--r--   0 matthijs   (501) staff       (20)     7005 2024-05-22 17:37:10.000000 brapi_proxy-0.0.6/src/brapi_proxy/core/core_studies.py
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 12:24:23.493667 brapi_proxy-0.0.6/src/brapi_proxy/genotyping/
--rw-r--r--   0 matthijs   (501) staff       (20)     1745 2024-05-22 17:56:28.000000 brapi_proxy-0.0.6/src/brapi_proxy/genotyping/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)    25351 2024-05-23 07:19:21.000000 brapi_proxy-0.0.6/src/brapi_proxy/genotyping/genotyping_allelematrix.py
--rw-r--r--   0 matthijs   (501) staff       (20)     4030 2024-05-22 17:38:37.000000 brapi_proxy-0.0.6/src/brapi_proxy/genotyping/genotyping_callsets.py
--rw-r--r--   0 matthijs   (501) staff       (20)     6179 2024-05-22 17:39:08.000000 brapi_proxy-0.0.6/src/brapi_proxy/genotyping/genotyping_plates.py
--rw-r--r--   0 matthijs   (501) staff       (20)     5926 2024-05-22 17:39:34.000000 brapi_proxy-0.0.6/src/brapi_proxy/genotyping/genotyping_references.py
--rw-r--r--   0 matthijs   (501) staff       (20)     5573 2024-05-22 17:40:06.000000 brapi_proxy-0.0.6/src/brapi_proxy/genotyping/genotyping_referencesets.py
--rw-r--r--   0 matthijs   (501) staff       (20)     6186 2024-05-22 17:40:30.000000 brapi_proxy-0.0.6/src/brapi_proxy/genotyping/genotyping_samples.py
--rw-r--r--   0 matthijs   (501) staff       (20)     3936 2024-05-22 17:41:59.000000 brapi_proxy-0.0.6/src/brapi_proxy/genotyping/genotyping_variants.py
--rw-r--r--   0 matthijs   (501) staff       (20)     5410 2024-05-22 17:42:26.000000 brapi_proxy-0.0.6/src/brapi_proxy/genotyping/genotyping_variantsets.py
--rw-r--r--   0 matthijs   (501) staff       (20)    13760 2024-04-23 07:04:17.000000 brapi_proxy-0.0.6/src/brapi_proxy/handler.py
--rw-r--r--   0 matthijs   (501) staff       (20)     1394 2024-05-23 07:16:51.000000 brapi_proxy-0.0.6/src/brapi_proxy/service.py
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 12:24:23.494035 brapi_proxy-0.0.6/src/brapi_proxy.egg-info/
--rw-r--r--   0 matthijs   (501) staff       (20)     4980 2024-05-23 12:24:23.000000 brapi_proxy-0.0.6/src/brapi_proxy.egg-info/PKG-INFO
--rw-r--r--   0 matthijs   (501) staff       (20)     1057 2024-05-23 12:24:23.000000 brapi_proxy-0.0.6/src/brapi_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 matthijs   (501) staff       (20)        1 2024-05-23 12:24:23.000000 brapi_proxy-0.0.6/src/brapi_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       60 2024-05-23 12:24:23.000000 brapi_proxy-0.0.6/src/brapi_proxy.egg-info/entry_points.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       65 2024-05-23 12:24:23.000000 brapi_proxy-0.0.6/src/brapi_proxy.egg-info/requires.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       12 2024-05-23 12:24:23.000000 brapi_proxy-0.0.6/src/brapi_proxy.egg-info/top_level.txt
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-27 07:49:55.531463 brapi_proxy-0.0.7/
+-rw-r--r--   0 matthijs   (501) staff       (20)     1079 2024-05-23 06:09:10.000000 brapi_proxy-0.0.7/LICENSE
+-rw-r--r--   0 matthijs   (501) staff       (20)     5173 2024-05-27 07:49:55.531081 brapi_proxy-0.0.7/PKG-INFO
+-rw-r--r--   0 matthijs   (501) staff       (20)     3195 2024-05-24 18:27:47.000000 brapi_proxy-0.0.7/README.md
+-rw-r--r--   0 matthijs   (501) staff       (20)     1038 2024-05-23 09:26:28.000000 brapi_proxy-0.0.7/pyproject.toml
+-rw-r--r--   0 matthijs   (501) staff       (20)       65 2024-05-22 18:03:35.000000 brapi_proxy-0.0.7/requirements.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)       38 2024-05-27 07:49:55.531567 brapi_proxy-0.0.7/setup.cfg
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-27 07:49:55.514703 brapi_proxy-0.0.7/src/
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-27 07:49:55.518734 brapi_proxy-0.0.7/src/brapi_proxy/
+-rw-r--r--   0 matthijs   (501) staff       (20)       85 2024-05-21 08:26:30.000000 brapi_proxy-0.0.7/src/brapi_proxy/__init__.py
+-rw-r--r--   0 matthijs   (501) staff       (20)       22 2024-05-27 07:49:15.000000 brapi_proxy-0.0.7/src/brapi_proxy/_version.py
+-rw-r--r--   0 matthijs   (501) staff       (20)    10059 2024-05-27 07:25:57.000000 brapi_proxy-0.0.7/src/brapi_proxy/brapi.py
+-rw-r--r--   0 matthijs   (501) staff       (20)      827 2024-05-27 05:52:30.000000 brapi_proxy-0.0.7/src/brapi_proxy/config_demo.ini
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-27 07:49:55.525543 brapi_proxy-0.0.7/src/brapi_proxy/core/
+-rw-r--r--   0 matthijs   (501) staff       (20)     2497 2024-05-26 09:58:48.000000 brapi_proxy-0.0.7/src/brapi_proxy/core/__init__.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     1921 2024-05-26 09:59:04.000000 brapi_proxy-0.0.7/src/brapi_proxy/core/core_commoncropnames.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     5214 2024-05-27 07:06:36.000000 brapi_proxy-0.0.7/src/brapi_proxy/core/core_lists.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     5880 2024-05-27 05:51:43.000000 brapi_proxy-0.0.7/src/brapi_proxy/core/core_locations.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     5091 2024-05-24 16:08:00.000000 brapi_proxy-0.0.7/src/brapi_proxy/core/core_people.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     5351 2024-05-24 15:51:59.000000 brapi_proxy-0.0.7/src/brapi_proxy/core/core_programs.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     3703 2024-05-24 16:55:30.000000 brapi_proxy-0.0.7/src/brapi_proxy/core/core_seasons.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     2432 2024-05-22 17:35:22.000000 brapi_proxy-0.0.7/src/brapi_proxy/core/core_serverinfo.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     7012 2024-05-24 15:51:38.000000 brapi_proxy-0.0.7/src/brapi_proxy/core/core_studies.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     7669 2024-05-24 15:51:29.000000 brapi_proxy-0.0.7/src/brapi_proxy/core/core_trials.py
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-27 07:49:55.530010 brapi_proxy-0.0.7/src/brapi_proxy/genotyping/
+-rw-r--r--   0 matthijs   (501) staff       (20)     2598 2024-05-26 08:52:21.000000 brapi_proxy-0.0.7/src/brapi_proxy/genotyping/__init__.py
+-rw-r--r--   0 matthijs   (501) staff       (20)    25296 2024-05-27 07:39:36.000000 brapi_proxy-0.0.7/src/brapi_proxy/genotyping/genotyping_allelematrix.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     4030 2024-05-22 17:38:37.000000 brapi_proxy-0.0.7/src/brapi_proxy/genotyping/genotyping_callsets.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     6179 2024-05-22 17:39:08.000000 brapi_proxy-0.0.7/src/brapi_proxy/genotyping/genotyping_plates.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     5926 2024-05-22 17:39:34.000000 brapi_proxy-0.0.7/src/brapi_proxy/genotyping/genotyping_references.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     5573 2024-05-22 17:40:06.000000 brapi_proxy-0.0.7/src/brapi_proxy/genotyping/genotyping_referencesets.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     6186 2024-05-22 17:40:30.000000 brapi_proxy-0.0.7/src/brapi_proxy/genotyping/genotyping_samples.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     3936 2024-05-22 17:41:59.000000 brapi_proxy-0.0.7/src/brapi_proxy/genotyping/genotyping_variants.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     5410 2024-05-22 17:42:26.000000 brapi_proxy-0.0.7/src/brapi_proxy/genotyping/genotyping_variantsets.py
+-rw-r--r--   0 matthijs   (501) staff       (20)    15749 2024-05-27 07:32:49.000000 brapi_proxy-0.0.7/src/brapi_proxy/handler.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     1394 2024-05-23 07:16:51.000000 brapi_proxy-0.0.7/src/brapi_proxy/service.py
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-27 07:49:55.530592 brapi_proxy-0.0.7/src/brapi_proxy.egg-info/
+-rw-r--r--   0 matthijs   (501) staff       (20)     5173 2024-05-27 07:49:55.000000 brapi_proxy-0.0.7/src/brapi_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 matthijs   (501) staff       (20)     1278 2024-05-27 07:49:55.000000 brapi_proxy-0.0.7/src/brapi_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)        1 2024-05-27 07:49:55.000000 brapi_proxy-0.0.7/src/brapi_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)       60 2024-05-27 07:49:55.000000 brapi_proxy-0.0.7/src/brapi_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)       65 2024-05-27 07:49:55.000000 brapi_proxy-0.0.7/src/brapi_proxy.egg-info/requires.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)       12 2024-05-27 07:49:55.000000 brapi_proxy-0.0.7/src/brapi_proxy.egg-info/top_level.txt
```

### Comparing `brapi_proxy-0.0.6/LICENSE` & `brapi_proxy-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.6/PKG-INFO` & `brapi_proxy-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brapi-proxy
-Version: 0.0.6
+Version: 0.0.7
 Summary: A BRAPI server instance that functions as a proxy to merge and combine endpoints from existing BRAPI services
 Author-email: Matthijs Brouwer <matthijs.brouwer@wur.nl>
 License: MIT License
         
         Copyright (c) 2024 EU H2020 AGENT project
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -80,32 +80,42 @@
 **BrAPI Versions**
 - version 2.1
 
 **Endpoints**
 
 - BrAPI-Core
   - /commoncropnames
+  - /lists
+  - /lists/{listDbId}
+  - /locations
+  - /locations/{locationDbId}
+  - /people
+  - /people/{personDbId}
+  - /programs
+  - /programs/{programDbId}
   - /studies
   - /studies/{studyDbId}
+  - /trials
+  - /trials/{trialDbId}
 - BrAPI-Genotyping
+  - /allelematrix
   - /callsets
   - /callsets/{callSetDbId}
-  - /variants
-  - /variants/{variantDbId}
-  - /variantsets
-  - /variantsets/{variantSetDbId}
   - /plates
   - /plates/{plateDbId}
-  - /samples
-  - /samples/{sampleDbId}
   - /references
   - /references/{referenceDbId}
   - /referencesets
   - /referencesets/{referenceSetDbId}
-  - /allelematrix
+  - /samples
+  - /samples/{sampleDbId}
+  - /variants
+  - /variants/{variantDbId}
+  - /variantsets
+  - /variantsets/{variantSetDbId}
   
 ### ToDo
 
 - Implement additional endpoints
 - Enable authentication for underlying servers
   
 ---
```

### Comparing `brapi_proxy-0.0.6/README.md` & `brapi_proxy-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,32 +40,42 @@
 **BrAPI Versions**
 - version 2.1
 
 **Endpoints**
 
 - BrAPI-Core
   - /commoncropnames
+  - /lists
+  - /lists/{listDbId}
+  - /locations
+  - /locations/{locationDbId}
+  - /people
+  - /people/{personDbId}
+  - /programs
+  - /programs/{programDbId}
   - /studies
   - /studies/{studyDbId}
+  - /trials
+  - /trials/{trialDbId}
 - BrAPI-Genotyping
+  - /allelematrix
   - /callsets
   - /callsets/{callSetDbId}
-  - /variants
-  - /variants/{variantDbId}
-  - /variantsets
-  - /variantsets/{variantSetDbId}
   - /plates
   - /plates/{plateDbId}
-  - /samples
-  - /samples/{sampleDbId}
   - /references
   - /references/{referenceDbId}
   - /referencesets
   - /referencesets/{referenceSetDbId}
-  - /allelematrix
+  - /samples
+  - /samples/{sampleDbId}
+  - /variants
+  - /variants/{variantDbId}
+  - /variantsets
+  - /variantsets/{variantSetDbId}
   
 ### ToDo
 
 - Implement additional endpoints
 - Enable authentication for underlying servers
   
 ---
```

### Comparing `brapi_proxy-0.0.6/pyproject.toml` & `brapi_proxy-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.6/src/brapi_proxy/brapi.py` & `brapi_proxy-0.0.7/src/brapi_proxy/brapi.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 
 from waitress import serve
 
 from . import handler
 from .core import calls_api_core, ns_api_core
 from .genotyping import calls_api_genotyping, ns_api_genotyping
 
-supportedCalls = list(calls_api_core.keys()) + list(calls_api_genotyping.keys())
+supportedCalls = {}
+for key,value in calls_api_core.items(): supportedCalls[key] = (value[0],value[1],value[2])
+for key,value in calls_api_genotyping.items(): supportedCalls[key] = (value[0],value[1],value[2])
 
 class BrAPI:
     """Main BrAPI class"""
 
     def __init__(self,location,config_file="config.ini"):
         #solve reload problem when using spawn method (osx/windows)
         if get_start_method()=="spawn":
@@ -49,14 +51,15 @@
                 process_api = Process(target=self.process_api_messages, args=[])
                 self.logger.debug("try to start server")
                 process_api.start()
                 #wait until ends
                 process_api.join()
             except Exception as e:
                 self.logger.error("error: %s",str(e))
+            break
 
     def process_api_messages(self):
         """
         Processing the API messages, implement BrAPI
         """
         #--- initialize Flask application ---
         app = Flask(__name__, static_url_path="/static",
@@ -78,19 +81,18 @@
         api = Api(blueprint, title=api_title,
                   authorizations=authorizations, security="apikey",
                   description=api_description, version=self.version)
         #config
         apidoc.static_url_path = os.path.join(server_location,"swaggerui")
         api.config = self.config
         api.brapi = {
-            "namespaces": {},
             "servers": {},
-            "calls": {},
+            "calls": {"serverinfo":{}},
             "authorization": {},
-            "supportedCalls": supportedCalls,
+            "identifiers": {call : value[0] for call,value in supportedCalls.items()},
             "version": self.version
         }
         #get configuration
         if self.config.has_section("authorization"):
             for option in self.config.options("authorization"):
                 api.brapi["authorization"][option] = str(self.config.get("authorization",option))
         servers = [entry[7:] for entry in self.config.sections()
@@ -103,76 +105,88 @@
                 api.brapi["servers"][server_name]["name"] = server_name
                 api.brapi["servers"][server_name]["calls"] = []
                 api.brapi["servers"][server_name]["prefixes"] = {}
                 for key in self.config.options(server_section):
                     if key.startswith("prefix."):
                         api.brapi["servers"][server_name]["prefixes"][key[7:]] = str(
                             self.config.get(server_section,key))
-                serverinfo,_,_ = handler.brapiRequest(
+                serverinfo,_,_ = handler.brapiGetRequest(
                     api.brapi["servers"][server_name],"serverinfo")
                 if not serverinfo:
                     self.logger.error("server %s unreachable",server_name)
                     time.sleep(60)
                     raise ConnectionError("retry because server {} unreachable".format(server_name))
                 if self.config.has_option(server_section,"calls"):
                     calls = self.config.get(server_section,"calls").split(",")
                     server_calls = serverinfo.get("result",{}).get("calls",[])
+                    #get available method/services with the right version and contentType
+                    availableServerCalls = set()
+                    for server_call in server_calls:
+                        if (
+                            "application/json" in server_call.get("contentTypes",[])
+                            and
+                            "application/json" in server_call.get("dataTypes",[])
+                            and
+                            self.version in server_call.get("versions",[])
+                        ) :
+                            for method in server_call.get("methods",[]):
+                                availableServerCalls.add((str(method).lower(),server_call.get("service")))
                     for call in calls:
                         if not call in supportedCalls:
                             self.logger.warning(
                                 "call %s for %s not supported by proxy",call,server_name)
+                        elif not availableServerCalls.issuperset(supportedCalls[call][1]):
+                            self.logger.warning(
+                                "call %s not supported by %s",call,server_name)
                         else:
-                            call_found_for_server = False
+                            if not call in api.brapi["calls"]:
+                                api.brapi["calls"][call] = {}
+                            if not server_name in api.brapi["calls"][call]:
+                                api.brapi["calls"][call][server_name] = []
                             for server_call in server_calls:
-                                if call==server_call["service"]:
-                                    api.brapi["servers"][server_name]["calls"].append(call)
-                                    if not call in api.brapi["calls"]:
-                                        api.brapi["calls"][call] = []
-                                    if not "application/json" in server_call.get(
-                                        "contentTypes",[]):
-                                        self.logger.error(
-                                            "contentType application/json not supported "+
-                                            "for %s by %s",call,server_name)
-                                    elif not "application/json" in server_call.get(
-                                        "dataTypes",[]):
-                                        self.logger.error(
-                                            "dataType application/json not supported "+
-                                            "for %s by %s",call,server_name)
-                                    elif not self.version in server_call.get(
-                                        "versions",[]):
-                                        self.logger.error(
-                                            "version %s not supported "+
-                                            "for %s by %s",self.version,call,server_name)
-                                    else:
-                                        api.brapi["calls"][call].append(
-                                            {"server": server_name, "info": server_call})
-                                        call_found_for_server = True
-                            #continue but log error if call not found
-                            if not call_found_for_server:
-                                self.logger.error("call %s for %s not available",
-                                                  call,server_name)
+                                for method in server_call["methods"]:
+                                    callKey = (method.lower(),server_call["service"])
+                                    if callKey in supportedCalls[call][1] or callKey in supportedCalls[call][2]:
+                                        for method in server_call.get("methods"):
+                                            entry = (method.lower(),server_call.get("service"))
+                                            if entry in supportedCalls[call][1] or entry in supportedCalls[call][2]:
+                                                api.brapi["calls"][call][server_name].append(entry)
                 self.logger.debug("checked configuration server %s",server_name)
+        
         #always provide core namespace
         api.add_namespace(ns_api_core)
         core_calls = set(calls_api_core.keys()).intersection(api.brapi["calls"])
         core_calls.add("serverinfo")
         for call in core_calls:
-            for resource in calls_api_core[call]:
-                ns_api_core.add_resource(resource[0], resource[1])
+            for resource in calls_api_core[call][3]:
+                servers = list(api.brapi["calls"][call].keys())
+                if len(servers)>0:
+                    shared = set.intersection(*[set([tuple(entry) for entry in item]) for item in api.brapi["calls"][call].values()])
+                else:
+                    shared = set()
+                methods = resource[0]._methods(shared,servers) if callable(getattr(resource[0], "_methods", None)) else ["get"]
+                ns_api_core.add_resource(resource[0], resource[1], methods=methods)
         #genotyping namespace
         genotyping_calls = set(calls_api_genotyping.keys()).intersection(api.brapi["calls"])
         if len(genotyping_calls)>0:
             api.add_namespace(ns_api_genotyping)
             for call in genotyping_calls:
-                for resource in calls_api_genotyping[call]:
-                    ns_api_genotyping.add_resource(resource[0], resource[1])
+                servers = list(api.brapi["calls"][call].keys())
+                shared = set.intersection(*[set([tuple(entry) for entry in item]) for item in api.brapi["calls"][call].values()])
+                if len(servers)>0:
+                    shared = set.intersection(*[set([tuple(entry) for entry in item]) for item in api.brapi["calls"][call].values()])
+                else:
+                    shared = set()
+                for resource in calls_api_genotyping[call][3]:
+                    methods = resource[0]._methods(shared,servers) if callable(getattr(resource[0], "_methods", None)) else ["get"]
+                    ns_api_genotyping.add_resource(resource[0], resource[1], methods=methods)
         #register blueprint
         app.register_blueprint(blueprint)
         app.config.SWAGGER_UI_DOC_EXPANSION = "list"
-
+        
         #--- start webserver ---
         server_host = self.config.get("brapi","host", fallback="0.0.0.0")
         server_port = self.config.get("brapi","port", fallback="8080")
         server_threads = self.config.get("brapi","threads", fallback="4")
         self.logger.info("start server on host %s and port %s with %s threads",
             server_host,server_port,server_threads)
         serve(app, host=server_host, port=server_port, threads=server_threads)
```

### Comparing `brapi_proxy-0.0.6/src/brapi_proxy/config_demo.ini` & `brapi_proxy-0.0.7/src/brapi_proxy/config_demo.ini`

 * *Files 7% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 prefix.variantsets=wheat:
 prefix.references=wheat:
 prefix.referencesets=wheat:
 prefix.callsets=wheat:
 
 [server.test3]
 url=https://test-server.brapi.org/brapi/v2
-calls=samples,studies,plates,callsets,variantsets,referencesets,references
+calls=people,locations,seasons,lists,samples,studies,programs,trials,plates,callsets,variantsets,referencesets,references
```

### Comparing `brapi_proxy-0.0.6/src/brapi_proxy/core/core_commoncropnames.py` & `brapi_proxy-0.0.7/src/brapi_proxy/core/core_commoncropnames.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.6/src/brapi_proxy/core/core_serverinfo.py` & `brapi_proxy-0.0.7/src/brapi_proxy/core/core_serverinfo.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.6/src/brapi_proxy/core/core_studies.py` & `brapi_proxy-0.0.7/src/brapi_proxy/core/core_studies.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,14 @@
         help="Used to request a specific page of data to be returned<br>The page indexing starts at 0 (the first page is 'page'= 0). Default is `0`")
 parser.add_argument("pageSize", type=int, required=False,
         help="The size of the pages to be returned. Default is `1000`")
 parser.add_argument("Authorization", type=str, required=False,
         help="HTTP HEADER - Token used for Authorization<br>**Bearer {token_string}**", 
         location="headers")
 
-#problem: sorting not working for multiple endpoints
-
 class CoreStudies(Resource):
 
     @namespace.expect(parser, validate=True)
     @handler.authorization
     def get(self):
         args = parser.parse_args(strict=True)
         try:            
@@ -68,15 +66,15 @@
             pageSize = int(args["pageSize"]) if not args["pageSize"] is None else 1000
             params = {"page": page, "pageSize": pageSize}
             for key,value in args.items():
                 if not key in ["page","pageSize","Authorization"]:
                     if not value is None:
                         params[key] = value
             brapiResponse,brapiStatus,brapiError = handler.brapiRepaginateRequestResponse(
-                self.api.brapi, "studies", params=params)
+                self.api.brapi, "studies", params=params, unsupportedForMultipleServerResponse=["sortBy","sortOrder"])
             if brapiResponse:
                 return Response(json.dumps(brapiResponse), mimetype="application/json")
             else:
                 response = Response(json.dumps(str(brapiError)), mimetype="application/json")
                 response.status_code = brapiStatus
                 return response
         except Exception as e:
```

### Comparing `brapi_proxy-0.0.6/src/brapi_proxy/genotyping/__init__.py` & `brapi_proxy-0.0.7/src/brapi_proxy/genotyping/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,24 +9,39 @@
 from .genotyping_plates import GenotypingPlates,GenotypingPlatesId
 from .genotyping_references import GenotypingReferences,GenotypingReferencesId
 from .genotyping_variantsets import GenotypingVariantSets,GenotypingVariantSetsId
 from .genotyping_referencesets import GenotypingReferenceSets,GenotypingReferenceSetsId
 from .genotyping_callsets import GenotypingCallSets,GenotypingCallSetsId
 from .genotyping_allelematrix import GenotypingAllelematrix
 
+# callName: [
+#    <callIdentifierName>,
+#    [<requiredService>,...],
+#    [<optionalService>,...],
+#    [[<resourceClass,<location>],...]
+#]
+
 calls_api_genotyping = {
-    "variants": [(GenotypingVariants,"/variants"),
-                 (GenotypingVariantsId,"/variants/<variantDbId>")],
-    "samples": [(GenotypingSamples,"/samples"),
-                (GenotypingSamplesId,"/samples/<sampleDbId>")],
-    "plates": [(GenotypingPlates,"/plates"),
-                (GenotypingPlatesId,"/plates/<plateDbId>")],
-    "references": [(GenotypingReferences,"/references"),
-                (GenotypingReferencesId,"/references/<referenceDbId>")],
-    "variantsets": [(GenotypingVariantSets,"/variantsets"),
-                (GenotypingVariantSetsId,"/variantsets/<variantSetDbId>")],
-    "referencesets": [(GenotypingReferenceSets,"/referencesets"),
-                (GenotypingReferenceSetsId,"/referencesets/<referenceSetDbId>")],
-    "callsets": [(GenotypingCallSets,"/callsets"),
-                (GenotypingCallSetsId,"/callsets/<callSetDbId>")],
-    "allelematrix": [(GenotypingAllelematrix,"/allelematrix")],
+    "variants": ("variantDbId",[("get","variants")],[("get","variants/{variantDbId}")],
+                 [(GenotypingVariants,"/variants"),
+                 (GenotypingVariantsId,"/variants/<variantDbId>")]),
+    "samples": ("sampleDbId",[("get","samples")],[("get","samples/{sampleDbId}")],
+                [(GenotypingSamples,"/samples"),
+                (GenotypingSamplesId,"/samples/<sampleDbId>")]),
+    "plates": ("plateDbId",[("get","plates")],[("get","plates/{plateDbId}")],
+                [(GenotypingPlates,"/plates"),
+                (GenotypingPlatesId,"/plates/<plateDbId>")]),
+    "references": ("referenceDbId",[("get","references")],[("get","references/{referenceDbId}")],
+                 [(GenotypingReferences,"/references"),
+                (GenotypingReferencesId,"/references/<referenceDbId>")]),
+    "variantsets": ("variantSetDbId",[("get","variantsets")],[("get","variantsets/{variantSetDbId}")],
+                 [(GenotypingVariantSets,"/variantsets"),
+                (GenotypingVariantSetsId,"/variantsets/<variantSetDbId>")]),
+    "referencesets": ("referenceSetDbId",[("get","referencesets")],[("get","referencesets/{referenceSetDbId}")],
+                 [(GenotypingReferenceSets,"/referencesets"),
+                (GenotypingReferenceSetsId,"/referencesets/<referenceSetDbId>")]),
+    "callsets": ("callSetDbId",[("get","callsets")],[("get","callsets/{callSetDbId}")],
+                 [(GenotypingCallSets,"/callsets"),
+                (GenotypingCallSetsId,"/callsets/<callSetDbId>")]),
+    "allelematrix": (None,[("get","allelematrix")],[],
+                 [(GenotypingAllelematrix,"/allelematrix")]),
 }
```

### Comparing `brapi_proxy-0.0.6/src/brapi_proxy/genotyping/genotyping_allelematrix.py` & `brapi_proxy-0.0.7/src/brapi_proxy/genotyping/genotyping_allelematrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             args["preview"] = args["preview"] if not args["preview"] is None else False
             args["expandHomozygotes"] = args["expandHomozygotes"] if not args["expandHomozygotes"] is None else True
             args["unknownString"] = args["unknownString"] if not args["unknownString"] is None else "."
             args["sepPhased"] = args["sepPhased"] if not args["sepPhased"] is None else "|"
             args["sepUnphased"] = args["sepUnphased"] if not args["sepUnphased"] is None else "/"
             params = {"dimensionVariantPage": dimensionVariantPage, 
                       "dimensionVariantPageSize": dimensionVariantPageSize,
-                      "dimensionCallSetPage": dimensionCallSetPage, 
+                      "dimensionCallSetPage": dimensionCallSetPage,
                       "dimensionCallSetPageSize": dimensionCallSetPageSize}
             for key,value in args.items():
                 if not key in ["dimensionVariantPage","dimensionVariantPageSize",
                                "dimensionCallSetPage","dimensionCallSetPageSize","Authorization"]:
                     if not value is None:
                         params[key] = value
             brapiResponse,brapiStatus,brapiError = _brapiRepaginateAllelematrixRequestResponse(
@@ -88,21 +88,21 @@
             response = Response(json.dumps(str(e)), mimetype="application/json")
             response.status_code = 500
             return response
         
         
 logger = logging.getLogger("brapi.handler")
 
-def _brapiRepaginateAllelematrixServerRequest(server, serverParams, supportedCalls,
+def _brapiRepaginateAllelematrixServerRequest(server, serverParams, identifiers,
                                                 subStartVariants, subEndVariants, 
                                                 subStartCallSets, subEndCallSets):
     additionalVariantsRequest = False
     additionalCallSetsRequest = False
     #get page
-    itemResponse,itemStatus,itemError = handler.brapiRequest(server,"allelematrix",params=serverParams)
+    itemResponse,itemStatus,itemError = handler.brapiGetRequest(server,"allelematrix",params=serverParams)
     if not itemResponse:
         return None, 500, "invalid response ({}) from {}: {}".format(
             itemStatus,server["name"],str(itemError))
     subVariantsTotal = 0
     subVariantsPage = 0
     subVariantsPageSize = serverParams["dimensionVariantPageSize"]
     subCallSetsTotal = 0
@@ -115,22 +115,22 @@
             subVariantsPageSize = int(entry.get("pageSize",subVariantsPageSize))
         elif entry.get("dimension","")=="CALLSETS":
             subCallSetsTotal = int(entry.get("totalCount",subCallSetsTotal))
             subCallSetsPage = int(entry.get("page",subCallSetsPage))
             subCallSetsPageSize = int(entry.get("pageSize",subCallSetsPageSize))
     subVariantDbIds = itemResponse.get("result",{}).get("variantDbIds",[]) 
     subVariantDbIds = handler.prefixDataEntry({"variantDbIds": subVariantDbIds},
-                                   server["prefixes"],supportedCalls)["variantDbIds"]
+                                   server["prefixes"],identifiers)["variantDbIds"]
     subVariantSetDbIds = itemResponse.get("result",{}).get("variantSetDbIds",[])
     subVariantSetDbIds = [] if not subVariantSetDbIds else subVariantSetDbIds
     subVariantSetDbIds = handler.prefixDataEntry({"variantSetDbIds": subVariantSetDbIds},
-                                   server["prefixes"],supportedCalls)["variantSetDbIds"]
+                                   server["prefixes"],identifiers)["variantSetDbIds"]
     subCallSetDbIds = itemResponse.get("result",{}).get("callSetDbIds",[])
     subCallSetDbIds = handler.prefixDataEntry({"callSetDbIds": subCallSetDbIds},
-                                   server["prefixes"],supportedCalls)["callSetDbIds"]
+                                   server["prefixes"],identifiers)["callSetDbIds"]
     subDataMatrices = itemResponse.get("result",{}).get("dataMatrices",[]) 
     #check variants
     logger.debug("server {} for allematrix has {} variants, get {} on page {} with size {}".format(
                 server["name"], subVariantsTotal, len(subVariantDbIds), 
         subVariantsPage, subVariantsPageSize))
     if not subVariantsPage==serverParams["dimensionVariantPage"]:
         logger.warning("unexpected variants page: {} instead of {}".format(
@@ -257,19 +257,19 @@
             if k<len(dataMatrix):
                 dataMatrix[k] = dataMatrix[k] + [unknownString]*(variantsEnd-len(dataMatrix[k]))
             else:
                 dataMatrix.append([unknownString]*variantsEnd)
         dataMatrices[j]["dataMatrix"] = dataMatrix
     return dataMatrices
     
-def _brapiRepaginateAllelematrixRequestResponse(apiBrapi, params):
+def _brapiRepaginateAllelematrixRequestResponse(brapi, params):
     #get servers
     servers = []
-    for item in apiBrapi["calls"]["allelematrix"]:
-        servers.append(apiBrapi["servers"].get(item["server"],{}))
+    for server in brapi["calls"]["allelematrix"]:
+        servers.append(brapi["servers"].get(server,{}))
     #initialise result
     result = {
         "callSetDbIds": [],
         "dataMatrices": [],
         "expandHomozygotes": params["expandHomozygotes"],
         "pagination": [
           {
@@ -307,29 +307,29 @@
     for server in servers:
         try:
             subStartVariants = startVariants - totalCountVariants
             subEndVariants = endVariants - totalCountVariants
             subStartCallSets = startCallSets - totalCountCallSets
             subEndCallSets = endCallSets - totalCountCallSets
             serverParams = handler.prefixRewriteParams(
-                params,server["prefixes"],apiBrapi["supportedCalls"])
+                params,server["prefixes"],brapi["identifiers"])
             if not serverParams is None:
                 #recompute page and pageSize
                 serverParams["dimensionVariantPage"] = max(0,math.floor(subStartVariants/params["dimensionVariantPageSize"]))
                 serverParams["dimensionVariantPageSize"] = params["dimensionVariantPageSize"]
                 serverParams["dimensionCallSetPage"] = max(0,math.floor(subStartCallSets/params["dimensionCallSetPageSize"]))
                 serverParams["dimensionCallSetPageSize"] = params["dimensionCallSetPageSize"]
                 #restrict to preview if additional information is not needed
                 if subStartVariants<0 and subEndVariants<0:
                     serverParams["preview"] = True
                 elif subStartCallSets<0 and subEndCallSets<0:
                     serverParams["preview"] = True
                 #get server response
                 serverResponse = _brapiRepaginateAllelematrixServerRequest(
-                                       server, serverParams, apiBrapi["supportedCalls"],
+                                       server, serverParams, brapi["identifiers"],
                                        subStartVariants, subEndVariants, subStartCallSets, subEndCallSets)
                 variantsStart = len(variantDbIds)
                 variantsEnd = variantsStart + len(serverResponse["variantDbIds"])
                 callSetsStart = len(callSetDbIds)
                 callSetsEnd = callSetsStart + len(serverResponse["callSetDbIds"])
                 variantDbIds = variantDbIds + serverResponse["variantDbIds"]
                 variantSetDbIds = list(set(variantSetDbIds + serverResponse["variantSetDbIds"]))
@@ -342,30 +342,30 @@
                 totalCountCallSets += serverResponse["callSetsTotal"]
                 if serverResponse["additionalVariantsRequest"] or serverResponse["additionalCallSetsRequest"]:
                     if serverResponse["additionalVariantsRequest"]:
                         serverParams1 = serverParams.copy()
                         subStartVariants1 = subStartVariants+len(serverResponse["variantDbIds"])
                         serverParams1["dimensionVariantPage"]+=1
                         newServerResponse1 = _brapiRepaginateAllelematrixServerRequest(
-                                               server, serverParams1, apiBrapi["supportedCalls"],
+                                               server, serverParams1, brapi["identifiers"],
                                                subStartVariants1, subEndVariants, subStartCallSets, subEndCallSets)
                         variantDbIds = variantDbIds + newServerResponse1["variantDbIds"]
                         variantSetDbIds = list(set(variantSetDbIds + newServerResponse1["variantSetDbIds"]))
                         variantsStart1 = variantsStart + len(serverResponse["variantDbIds"])
                         variantsEnd1 = variantsStart1 + len(newServerResponse1["variantDbIds"])
                         dataMatrices = _mergeAllematrixDataMatrices(
                             dataMatrices, newServerResponse1["dataMatrices"],
                             variantsStart1,variantsEnd1,
                             callSetsStart,callSetsEnd,serverParams1["unknownString"])
                     if serverResponse["additionalCallSetsRequest"]:
                         serverParams2 = serverParams.copy()
                         subStartCallSets2 = subStartCallSets+len(serverResponse["callSetDbIds"])
                         serverParams2["dimensionCallSetPage"]+=1
                         newServerResponse2 = _brapiRepaginateAllelematrixServerRequest(
-                                               server, serverParams2, apiBrapi["supportedCalls"],
+                                               server, serverParams2, brapi["identifiers"],
                                                subStartVariants, subEndVariants, subStartCallSets2, subEndCallSets)
                         callSetDbIds = callSetDbIds + newServerResponse2["callSetDbIds"]
                         callSetsStart2 = callSetsStart + len(serverResponse["callSetDbIds"])
                         callSetsEnd2 = callSetsStart2 + len(newServerResponse2["callSetDbIds"])
                         dataMatrices = _mergeAllematrixDataMatrices(
                             dataMatrices, newServerResponse2["dataMatrices"],
                             variantsStart,variantsEnd,
@@ -373,15 +373,15 @@
                     if serverResponse["additionalVariantsRequest"] and serverResponse["additionalCallSetsRequest"]:
                         serverParams3 = serverParams.copy()
                         subStartVariants3 = subStartVariants+len(serverResponse["variantDbIds"])
                         subStartCallSets3 = subStartCallSets+len(serverResponse["callSetDbIds"])
                         serverParams3["dimensionVariantPage"]+=1
                         serverParams3["dimensionCallSetPage"]+=1
                         newServerResponse3 = _brapiRepaginateAllelematrixServerRequest(
-                                               server, serverParams3, apiBrapi["supportedCalls"],
+                                               server, serverParams3, brapi["identifiers"],
                                                subStartVariants3, subEndVariants, subStartCallSets3, subEndCallSets)
                         variantsStart3 = variantsStart + len(serverResponse["variantDbIds"])
                         variantsEnd3 = variantsStart3 + len(newServerResponse3["variantDbIds"])
                         callSetsStart3 = callSetsStart + len(serverResponse["callSetDbIds"])
                         callSetsEnd3 = callSetsStart3 + len(newServerResponse3["callSetDbIds"])
                         dataMatrices = _mergeAllematrixDataMatrices(
                             dataMatrices, newServerResponse3["dataMatrices"],
```

### Comparing `brapi_proxy-0.0.6/src/brapi_proxy/genotyping/genotyping_callsets.py` & `brapi_proxy-0.0.7/src/brapi_proxy/genotyping/genotyping_callsets.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.6/src/brapi_proxy/genotyping/genotyping_plates.py` & `brapi_proxy-0.0.7/src/brapi_proxy/genotyping/genotyping_plates.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.6/src/brapi_proxy/genotyping/genotyping_references.py` & `brapi_proxy-0.0.7/src/brapi_proxy/genotyping/genotyping_references.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.6/src/brapi_proxy/genotyping/genotyping_referencesets.py` & `brapi_proxy-0.0.7/src/brapi_proxy/genotyping/genotyping_referencesets.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.6/src/brapi_proxy/genotyping/genotyping_samples.py` & `brapi_proxy-0.0.7/src/brapi_proxy/genotyping/genotyping_samples.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.6/src/brapi_proxy/genotyping/genotyping_variants.py` & `brapi_proxy-0.0.7/src/brapi_proxy/genotyping/genotyping_variants.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.6/src/brapi_proxy/genotyping/genotyping_variantsets.py` & `brapi_proxy-0.0.7/src/brapi_proxy/genotyping/genotyping_variantsets.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.6/src/brapi_proxy/handler.py` & `brapi_proxy-0.0.7/src/brapi_proxy/handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,43 +26,34 @@
                 response = Response("unauthorized", mimetype="content/text")
                 response.status_code = 401
                 return response
         return brapi_call(*args, **kwargs)
     return decorated
 
 
-def prefixDataEntry(data,prefixes,supportedCalls):
+def prefixDataEntry(data,prefixes,identifiers):
     for key,value in prefixes.items():
-        if value and key in supportedCalls:
-            if key.endswith("ies"):
-                idKey = "{}yDbId".format(key[:-3])
-            else:
-                idKey = "{}DbId".format(key[:-1])
+        if value and key in identifiers and not identifiers[key] is None:
+            idKey = identifiers[key]
+            idsKey = "{}s".format(idKey)
             if idKey in data and not data[idKey] is None:
                 if isinstance(data[idKey],str):
                     data[idKey] = "{}{}".format(value,data[idKey])
-            if key.endswith("ies"):
-                idsKey = "{}yDbIds".format(key[:-3])
-            else:
-                idsKey = "{}DbIds".format(key[:-1])
             if idsKey in data and not data[idsKey] is None:
                 if isinstance(data[idsKey],str):
                     data[idsKey] = "{}{}".format(value,data[idsKey])
                 elif isinstance(data[idsKey],list):
                     data[idsKey] = ["{}{}".format(value,entry) for entry in data[idsKey]]
     return data
 
-def prefixRewriteParams(params,prefixes,supportedCalls):
+def prefixRewriteParams(params,prefixes,identifiers):
     newParams = params.copy()
     for key,value in prefixes.items():
-        if value and key in supportedCalls:
-            if key.endswith("ies"):
-                idKey = "{}yDbId".format(key[:-3])
-            else:
-                idKey = "{}DbId".format(key[:-1])
+        if value and key in identifiers and not identifiers[key] is None:
+            idKey = identifiers[key]
             if idKey in newParams and not newParams[idKey] is None:
                 if isinstance(newParams[idKey],str):
                     if newParams[idKey].startswith(value):
                         newParams[idKey] = newParams[idKey][len(value):]
                     else:
                         return None
     return newParams
@@ -70,96 +61,143 @@
 def brapiResponse(result):
     response = {}
     response["@context"] = ["https://brapi.org/jsonld/context/metadata.jsonld"]
     response["metadata"] = {}
     response["result"] = result
     return response
 
-def brapiRequest(server,call,method="get",**args):
+def brapiGetRequest(server,call,**args):
     try:
-        if method=="get":
-            params = args.get("params",{})
-            headers = {"Accept": "application/json"}
-            url = "{}/{}".format(server["url"],call)
-            response = requests.get(url, params=params, headers=headers)
-            try:
-                if response.ok:
-                    return response.json(), response.status_code, None
-                else:
-                    return None, response.status_code, response.text
-            except:
-                return None, 500, response.text
-        else:
-            return None, 501, "unsupported method {} ".format(method)
+        params = args.get("params",{})
+        headers = {"Accept": "application/json"}
+        url = "{}/{}".format(server["url"],call)
+        response = requests.get(url, params=params, headers=headers)
+        try:
+            if response.ok:
+                return response.json(), response.status_code, None
+            else:
+                return None, response.status_code, response.text
+        except:
+            return None, 500, response.text
     except Exception as e:
         return None, 500, "error: {}".format(str(e))
 
+def brapiPostRequest(server,call,payload):
+    try:
+        headers = {"Accept": "application/json"}
+        url = "{}/{}".format(server["url"],call)
+        response = requests.post(url, data=payload, headers=headers)
+        try:
+            if response.ok:
+                return response.json(), response.status_code, None
+            else:
+                return None, response.status_code, response.text
+        except:
+            return None, 500, response.text
+    except Exception as e:
+        return None, 500, "error: {}".format(str(e))
+
+def brapiPostRequestResponse(brapi, call, payload):
+    #get servers
+    servers = []
+    for server in brapi["calls"][call]:
+        servers.append(brapi["servers"].get(server,{}))
+    #construct response
+    response = {}
+    response["@context"] = ["https://brapi.org/jsonld/context/metadata.jsonld"]
+    response["metadata"] = {}
+    for server in servers:
+        try:
+            if ("post", call) in brapi["calls"][call][server["name"]]:
+                itemResponse,itemStatus,itemError = brapiPostRequest(server,serverCall,payload)
+        except Exception as e:
+                return None, 500, "problem processing response from {}: {}".format(
+                    server["name"],str(e))
+    return None, 501, "unsupported post to {}".format(call)
 
 def brapiIdRequestResponse(brapi, call, name, id, method="get", **args):
     #get servers
     servers = []
-    for item in brapi["calls"][call]:
-        servers.append(brapi["servers"].get(item["server"],{}))
+    for server in brapi["calls"][call]:
+        servers.append(brapi["servers"].get(server,{}))
     #handle request
+    callById="{}/{{{}}}".format(call,name)
     if method=="get":
         #construct response
         response = {}
         response["@context"] = ["https://brapi.org/jsonld/context/metadata.jsonld"]
         response["metadata"] = {}
         for server in servers:
             try:
                 serverParams = {}
                 serverParams[name] = id
-                serverParams = prefixRewriteParams(serverParams,server["prefixes"],
-                                                   brapi["supportedCalls"])
+                serverParams = prefixRewriteParams(serverParams,server["prefixes"], brapi["identifiers"])
                 if not serverParams is None:
-                    itemResponse,itemStatus,itemError = brapiRequest(
-                        server,call,params=serverParams)
-                    if itemResponse:
-                        try:
-                            data = itemResponse.get("result").get("data")
-                            data = [prefixDataEntry(
-                                entry,server["prefixes"],
-                                brapi["supportedCalls"]) for entry in data]
-                            if len(data)==1:
-                                if name in data[0]:
-                                    if data[0][name]==id:
-                                        response["result"] = data[0]
-                                        return response, 200, None
+                    if (method, callById) in brapi["calls"][call][server["name"]]:
+                        serverCall = "{}/{}".format(call,serverParams[name])
+                        itemResponse,itemStatus,itemError = brapiGetRequest(server,serverCall)
+                        if itemResponse:
+                            try:
+                                data = itemResponse.get("result")
+                                data = prefixDataEntry(data,server["prefixes"],brapi["identifiers"])
+                                response["result"] = data
+                                return response, 200, None
+                            except:
+                                logger.warning("unexpected response from {}".format(server["name"]))
+                    elif (method, call) in brapi["calls"][call][server["name"]]:
+                        itemResponse,itemStatus,itemError = brapiGetRequest(
+                            server,call,params=serverParams)
+                        if itemResponse:
+                            try:
+                                data = itemResponse.get("result").get("data")
+                                data = [prefixDataEntry(
+                                    entry,server["prefixes"],
+                                    brapi["identifiers"]) for entry in data]
+                                if len(data)==1:
+                                    if name in data[0]:
+                                        if data[0][name]==id:
+                                            response["result"] = data[0]
+                                            return response, 200, None
+                                        else:
+                                            logger.warning("unexpected response with "+
+                                                           "{}: {} from {}".format(
+                                                name,data[0][name],server["name"]))
                                     else:
-                                        logger.warning("unexpected response with "+
-                                                       "{}: {} from {}".format(
-                                            name,data[0][name],server["name"]))
-                                else:
-                                    logger.warning("unexpected response without "+
-                                                   "{} from {}".format(
-                                            name,server["name"]))
-                            elif len(data)>1:
-                                logger.warning("unexpected multiple ({}) ".format(len(data))+
-                                               "entries in response from {}".format(
-                                                   server["name"]))
-                        except:
-                            logger.warning("unexpected response from {}".format(
-                                server["name"]))
+                                        logger.warning("unexpected response without "+
+                                                       "{} from {}".format(
+                                                name,server["name"]))
+                                elif len(data)>1:
+                                    logger.warning("unexpected multiple ({}) ".format(len(data))+
+                                                   "entries in response from {}".format(
+                                                       server["name"]))
+                            except:
+                                logger.warning("unexpected response from {}".format(
+                                    server["name"]))
             except Exception as e:
                 return None, 500, "problem processing response from {}: {}".format(
                     server["name"],str(e))
         return None, 404, "{} {} not found in {}".format(name,id,call)
     else:
         return None, 501, "unsupported method {}".format(method)
 
 
 def brapiRepaginateRequestResponse(brapi, call, method="get", **args):
     #get servers
     servers = []
-    for item in brapi["calls"][call]:
-        servers.append(brapi["servers"].get(item["server"],{}))
+    for server in brapi["calls"][call]:
+        servers.append(brapi["servers"].get(server,{}))
     #handle request
     if method=="get":
         params = args.get("params",{})
+        if len(servers)>1:
+            unsupported = args.get("unsupportedForMultipleServerResponse",[])
+            for key in params:
+                if key in unsupported:
+                    return None, 501, "unsupported parameter {}".format(key)
+        #pagination
         page = params.get("page",0)
         pageSize = params.get("pageSize",1000)
         #construct response
         response = {}
         response["@context"] = ["https://brapi.org/jsonld/context/metadata.jsonld"]
         response["metadata"] = {}
         response["metadata"]["pagination"] = {
@@ -170,35 +208,33 @@
         totalCount = 0
         start = page*pageSize
         end = ((page+1)*pageSize) - 1
         for server in servers:
             try:
                 subStart = start - totalCount
                 subEnd = end - totalCount
-                serverParams = prefixRewriteParams(params,server["prefixes"],
-                                                   brapi["supportedCalls"])
+                serverParams = prefixRewriteParams(params,server["prefixes"], brapi["identifiers"])
                 if not serverParams is None:
                     #recompute page and pageSize
                     serverParams["page"] = max(0,math.floor(subStart/pageSize))
                     serverParams["pageSize"] = pageSize
                     #get page
-                    itemResponse,itemStatus,itemError = brapiRequest(
+                    itemResponse,itemStatus,itemError = brapiGetRequest(
                         server,call,params=serverParams)
                     if not itemResponse:
                         return None, 500, "invalid response ({}) from {}: {}".format(
                             itemStatus,server["name"],str(itemError))
                     subTotal = itemResponse.get("metadata",{}).get(
                         "pagination",{}).get("totalCount",0)
                     subPage = itemResponse.get("metadata",{}).get(
                         "pagination",{}).get("currentPage",0)
                     subPageSize = itemResponse.get("metadata",{}).get(
                         "pagination",{}).get("pageSize",1000)
                     subData = itemResponse.get("result",{}).get("data",[])
-                    subData = [prefixDataEntry(entry,server["prefixes"],
-                                               brapi["supportedCalls"])
+                    subData = [prefixDataEntry(entry,server["prefixes"], brapi["identifiers"])
                                for entry in subData]
                     logger.debug("server {} for {} has {} results, ".format(
                         server["name"], call, subTotal)+
                         "get {} on page {} with size {}".format(
                             len(subData), subPage, subPageSize))
                     if not subPage==serverParams["page"]:
                         logger.warning("unexpected page: {} instead of {}".format(
@@ -217,15 +253,15 @@
                             logger.debug("add {} entries ({} - {}) from {} to {} result".format(
                                 len(subData),s1,s2,server["name"], call))
                             data = data + subData
                             #another page necessary
                             if subEnd>(((subPage+1)*subPageSize)-1):
                                 serverParams["page"]+=1
                                 #get next page
-                                itemResponse = brapiRequest(
+                                itemResponse = brapiGetRequest(
                                     server,call,params=serverParams)
                                 if not itemResponse:
                                     return (None, 500,
                                         "invalid response ({}) from {}: {}".format(
                                         itemStatus,server["name"],str(itemError)))
                                 subTotal = itemResponse.get("metadata",{}).get(
                                     "pagination",{}).get("totalCount",0)
@@ -255,14 +291,15 @@
                                 subData = subData[s1:s2+1]
                                 if s2>=s1:
                                     subData = subData[s1:s2+1]
                                     logger.debug("add {} entries ({} - {}) ".format(
                                         len(subData),s1,s2)+
                                         "from {} to {} result".format(
                                             server["name"], call))
+                                    #update data
                                     data = data + subData
                     totalCount += subTotal
             except Exception as e:
                 return (None, 500, "problem processing response "+
                         "from {}: {}".format(server["name"],str(e)))
         logger.debug("result for {} has in total {} entries".format(call,len(data)))
         response["result"] = {"data": data}
```

### Comparing `brapi_proxy-0.0.6/src/brapi_proxy/service.py` & `brapi_proxy-0.0.7/src/brapi_proxy/service.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.6/src/brapi_proxy.egg-info/PKG-INFO` & `brapi_proxy-0.0.7/src/brapi_proxy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brapi-proxy
-Version: 0.0.6
+Version: 0.0.7
 Summary: A BRAPI server instance that functions as a proxy to merge and combine endpoints from existing BRAPI services
 Author-email: Matthijs Brouwer <matthijs.brouwer@wur.nl>
 License: MIT License
         
         Copyright (c) 2024 EU H2020 AGENT project
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -80,32 +80,42 @@
 **BrAPI Versions**
 - version 2.1
 
 **Endpoints**
 
 - BrAPI-Core
   - /commoncropnames
+  - /lists
+  - /lists/{listDbId}
+  - /locations
+  - /locations/{locationDbId}
+  - /people
+  - /people/{personDbId}
+  - /programs
+  - /programs/{programDbId}
   - /studies
   - /studies/{studyDbId}
+  - /trials
+  - /trials/{trialDbId}
 - BrAPI-Genotyping
+  - /allelematrix
   - /callsets
   - /callsets/{callSetDbId}
-  - /variants
-  - /variants/{variantDbId}
-  - /variantsets
-  - /variantsets/{variantSetDbId}
   - /plates
   - /plates/{plateDbId}
-  - /samples
-  - /samples/{sampleDbId}
   - /references
   - /references/{referenceDbId}
   - /referencesets
   - /referencesets/{referenceSetDbId}
-  - /allelematrix
+  - /samples
+  - /samples/{sampleDbId}
+  - /variants
+  - /variants/{variantDbId}
+  - /variantsets
+  - /variantsets/{variantSetDbId}
   
 ### ToDo
 
 - Implement additional endpoints
 - Enable authentication for underlying servers
   
 ---
```

### Comparing `brapi_proxy-0.0.6/src/brapi_proxy.egg-info/SOURCES.txt` & `brapi_proxy-0.0.7/src/brapi_proxy.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -12,16 +12,22 @@
 src/brapi_proxy.egg-info/SOURCES.txt
 src/brapi_proxy.egg-info/dependency_links.txt
 src/brapi_proxy.egg-info/entry_points.txt
 src/brapi_proxy.egg-info/requires.txt
 src/brapi_proxy.egg-info/top_level.txt
 src/brapi_proxy/core/__init__.py
 src/brapi_proxy/core/core_commoncropnames.py
+src/brapi_proxy/core/core_lists.py
+src/brapi_proxy/core/core_locations.py
+src/brapi_proxy/core/core_people.py
+src/brapi_proxy/core/core_programs.py
+src/brapi_proxy/core/core_seasons.py
 src/brapi_proxy/core/core_serverinfo.py
 src/brapi_proxy/core/core_studies.py
+src/brapi_proxy/core/core_trials.py
 src/brapi_proxy/genotyping/__init__.py
 src/brapi_proxy/genotyping/genotyping_allelematrix.py
 src/brapi_proxy/genotyping/genotyping_callsets.py
 src/brapi_proxy/genotyping/genotyping_plates.py
 src/brapi_proxy/genotyping/genotyping_references.py
 src/brapi_proxy/genotyping/genotyping_referencesets.py
 src/brapi_proxy/genotyping/genotyping_samples.py
```

