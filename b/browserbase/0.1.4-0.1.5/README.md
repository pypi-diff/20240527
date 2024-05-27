# Comparing `tmp/browserbase-0.1.4.tar.gz` & `tmp/browserbase-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browserbase-0.1.4.tar", last modified: Sat May 18 11:35:52 2024, max compression
+gzip compressed data, was "browserbase-0.1.5.tar", last modified: Mon May 27 14:42:47 2024, max compression
```

## Comparing `browserbase-0.1.4.tar` & `browserbase-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-18 11:35:52.871099 browserbase-0.1.4/
--rw-r--r--   0 mish       (501) staff       (20)     1064 2024-04-09 17:45:47.000000 browserbase-0.1.4/LICENSE
--rw-r--r--   0 mish       (501) staff       (20)     1575 2024-05-18 11:35:52.870814 browserbase-0.1.4/PKG-INFO
--rw-r--r--   0 mish       (501) staff       (20)      933 2024-04-19 10:57:22.000000 browserbase-0.1.4/README.md
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-18 11:35:52.868841 browserbase-0.1.4/browserbase/
--rw-r--r--   0 mish       (501) staff       (20)    10500 2024-05-18 11:35:32.000000 browserbase-0.1.4/browserbase/__init__.py
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-18 11:35:52.870128 browserbase-0.1.4/browserbase/helpers/
--rw-r--r--   0 mish       (501) staff       (20)      301 2024-04-16 18:32:01.000000 browserbase-0.1.4/browserbase/helpers/anthropic.py
--rw-r--r--   0 mish       (501) staff       (20)      503 2024-04-15 12:54:51.000000 browserbase-0.1.4/browserbase/helpers/gpt4.py
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-18 11:35:52.870533 browserbase-0.1.4/browserbase.egg-info/
--rw-r--r--   0 mish       (501) staff       (20)     1575 2024-05-18 11:35:52.000000 browserbase-0.1.4/browserbase.egg-info/PKG-INFO
--rw-r--r--   0 mish       (501) staff       (20)      291 2024-05-18 11:35:52.000000 browserbase-0.1.4/browserbase.egg-info/SOURCES.txt
--rw-r--r--   0 mish       (501) staff       (20)        1 2024-05-18 11:35:52.000000 browserbase-0.1.4/browserbase.egg-info/dependency_links.txt
--rw-r--r--   0 mish       (501) staff       (20)       49 2024-05-18 11:35:52.000000 browserbase-0.1.4/browserbase.egg-info/requires.txt
--rw-r--r--   0 mish       (501) staff       (20)       12 2024-05-18 11:35:52.000000 browserbase-0.1.4/browserbase.egg-info/top_level.txt
--rw-r--r--   0 mish       (501) staff       (20)      697 2024-05-18 11:35:48.000000 browserbase-0.1.4/pyproject.toml
--rw-r--r--   0 mish       (501) staff       (20)       38 2024-05-18 11:35:52.871156 browserbase-0.1.4/setup.cfg
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-27 14:42:47.354598 browserbase-0.1.5/
+-rw-r--r--   0 mish       (501) staff       (20)     1064 2024-04-09 17:45:47.000000 browserbase-0.1.5/LICENSE
+-rw-r--r--   0 mish       (501) staff       (20)     1575 2024-05-27 14:42:47.354291 browserbase-0.1.5/PKG-INFO
+-rw-r--r--   0 mish       (501) staff       (20)      933 2024-04-19 10:57:22.000000 browserbase-0.1.5/README.md
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-27 14:42:47.352172 browserbase-0.1.5/browserbase/
+-rw-r--r--   0 mish       (501) staff       (20)     9995 2024-05-27 14:42:03.000000 browserbase-0.1.5/browserbase/__init__.py
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-27 14:42:47.353469 browserbase-0.1.5/browserbase/helpers/
+-rw-r--r--   0 mish       (501) staff       (20)      301 2024-04-16 18:32:01.000000 browserbase-0.1.5/browserbase/helpers/anthropic.py
+-rw-r--r--   0 mish       (501) staff       (20)      503 2024-04-15 12:54:51.000000 browserbase-0.1.5/browserbase/helpers/gpt4.py
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-27 14:42:47.353943 browserbase-0.1.5/browserbase.egg-info/
+-rw-r--r--   0 mish       (501) staff       (20)     1575 2024-05-27 14:42:47.000000 browserbase-0.1.5/browserbase.egg-info/PKG-INFO
+-rw-r--r--   0 mish       (501) staff       (20)      291 2024-05-27 14:42:47.000000 browserbase-0.1.5/browserbase.egg-info/SOURCES.txt
+-rw-r--r--   0 mish       (501) staff       (20)        1 2024-05-27 14:42:47.000000 browserbase-0.1.5/browserbase.egg-info/dependency_links.txt
+-rw-r--r--   0 mish       (501) staff       (20)       49 2024-05-27 14:42:47.000000 browserbase-0.1.5/browserbase.egg-info/requires.txt
+-rw-r--r--   0 mish       (501) staff       (20)       12 2024-05-27 14:42:47.000000 browserbase-0.1.5/browserbase.egg-info/top_level.txt
+-rw-r--r--   0 mish       (501) staff       (20)      697 2024-05-27 14:42:34.000000 browserbase-0.1.5/pyproject.toml
+-rw-r--r--   0 mish       (501) staff       (20)       38 2024-05-27 14:42:47.354664 browserbase-0.1.5/setup.cfg
```

### Comparing `browserbase-0.1.4/LICENSE` & `browserbase-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `browserbase-0.1.4/PKG-INFO` & `browserbase-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserbase
-Version: 0.1.4
+Version: 0.1.5
 Summary: Browserbase Python SDK
 Author-email: Browserbase <info@browserbase.com>
 Project-URL: Homepage, https://browserbase.com
 Project-URL: Source, https://github.com/browserbase/python-sdk
 Project-URL: Issues, https://github.com/browserbase/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `browserbase-0.1.4/README.md` & `browserbase-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `browserbase-0.1.4/browserbase/__init__.py` & `browserbase-0.1.5/browserbase/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,18 +28,28 @@
     browsers: Optional[list[BrowserType]] = None
     devices: Optional[list[DeviceType]] = None
     locales: Optional[list[str]] = None
     operatingSystems: Optional[list[OperatingSystem]] = None
     screen: Optional[Screen] = None
 
 
+class Viewport(BaseModel):
+    width: Optional[int] = None
+    height: Optional[int] = None
+
+
+class BrowserSettings(BaseModel):
+    fingerprint: Optional[Fingerprint] = None
+    viewport: Optional[Viewport] = None
+
+
 class CreateSessionOptions(BaseModel):
     projectId: Optional[str] = None
     extensionId: Optional[str] = None
-    fingerprint: Optional[Fingerprint] = None
+    browserSettings: Optional[BrowserSettings] = None
 
 
 class Session(BaseModel):
     id: str
     createdAt: str
     startedAt: str
     endedAt: Optional[str]
@@ -50,19 +60,14 @@
     expiresAt: Optional[str] = None
     avg_cpu_usage: Optional[float] = None
     memory_usage: Optional[int] = None
     details: Optional[str] = None
     logs: Optional[str] = None
 
 
-class UpdateSessionOptions(BaseModel):
-    projectId: Optional[str] = None
-    status: Optional[SessionStatus] = None
-
-
 class SessionRecording(BaseModel):
     type: Optional[str] = None
     time: Optional[str] = None
     data: Optional[dict] = None
 
 
 class DebugConnectionURLs(BaseModel):
@@ -155,33 +160,14 @@
                 "Content-Type": "application/json",
             },
         )
 
         response.raise_for_status()
         return Session(**response.json())
 
-    def update_session(
-        self, session_id: str, options: Optional[UpdateSessionOptions] = None
-    ) -> Session:
-        payload = {"projectId": self.project_id}
-        if options:
-            payload.update(options.model_dump(by_alias=True, exclude_none=True))
-
-        response = httpx.post(
-            f"{self.api_url}/v1/sessions/{session_id}",
-            headers={
-                "x-bb-api-key": self.api_key,
-                "Content-Type": "application/json",
-            },
-            json=payload,
-        )
-
-        response.raise_for_status()
-        return Session(**response.json())
-
     def get_session_recording(self, session_id: str) -> list[SessionRecording]:
         response = httpx.get(
             f"{self.api_url}/v1/sessions/{session_id}/recording",
             headers={
                 "x-bb-api-key": self.api_key,
                 "Content-Type": "application/json",
             },
```

### Comparing `browserbase-0.1.4/browserbase.egg-info/PKG-INFO` & `browserbase-0.1.5/browserbase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserbase
-Version: 0.1.4
+Version: 0.1.5
 Summary: Browserbase Python SDK
 Author-email: Browserbase <info@browserbase.com>
 Project-URL: Homepage, https://browserbase.com
 Project-URL: Source, https://github.com/browserbase/python-sdk
 Project-URL: Issues, https://github.com/browserbase/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `browserbase-0.1.4/pyproject.toml` & `browserbase-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "browserbase"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Browserbase", email="info@browserbase.com" },
 ]
 description = "Browserbase Python SDK"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

