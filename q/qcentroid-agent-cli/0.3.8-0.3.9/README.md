# Comparing `tmp/qcentroid_agent_cli-0.3.8.tar.gz` & `tmp/qcentroid_agent_cli-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcentroid_agent_cli-0.3.8.tar", max compression
+gzip compressed data, was "qcentroid_agent_cli-0.3.9.tar", max compression
```

## Comparing `qcentroid_agent_cli-0.3.8.tar` & `qcentroid_agent_cli-0.3.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1298 2024-01-16 08:07:51.658323 qcentroid_agent_cli-0.3.8/LICENSE
--rw-r--r--   0        0        0     1559 2024-01-16 08:07:51.658323 qcentroid_agent_cli-0.3.8/README.md
--rw-r--r--   0        0        0      794 2024-01-16 08:07:51.658323 qcentroid_agent_cli-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     7372 2024-01-16 08:07:51.658323 qcentroid_agent_cli-0.3.8/qcentroid_agent_cli/__init__.py
--rw-r--r--   0        0        0      566 2024-01-16 08:07:51.658323 qcentroid_agent_cli-0.3.8/qcentroid_agent_cli/model/StatusEntity.py
--rw-r--r--   0        0        0        0 2024-01-16 08:07:51.658323 qcentroid_agent_cli-0.3.8/qcentroid_agent_cli/model/__init__.py
--rw-r--r--   0        0        0     2251 1970-01-01 00:00:00.000000 qcentroid_agent_cli-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1298 2024-01-16 08:13:04.712774 qcentroid_agent_cli-0.3.9/LICENSE
+-rw-r--r--   0        0        0     1559 2024-01-16 08:13:04.712774 qcentroid_agent_cli-0.3.9/README.md
+-rw-r--r--   0        0        0      794 2024-01-16 08:13:04.712774 qcentroid_agent_cli-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     9503 2024-01-16 08:13:04.712774 qcentroid_agent_cli-0.3.9/qcentroid_agent_cli/__init__.py
+-rw-r--r--   0        0        0      566 2024-01-16 08:13:04.712774 qcentroid_agent_cli-0.3.9/qcentroid_agent_cli/model/StatusEntity.py
+-rw-r--r--   0        0        0        0 2024-01-16 08:13:04.712774 qcentroid_agent_cli-0.3.9/qcentroid_agent_cli/model/__init__.py
+-rw-r--r--   0        0        0     2251 1970-01-01 00:00:00.000000 qcentroid_agent_cli-0.3.9/PKG-INFO
```

### Comparing `qcentroid_agent_cli-0.3.8/LICENSE` & `qcentroid_agent_cli-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qcentroid_agent_cli-0.3.8/README.md` & `qcentroid_agent_cli-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `qcentroid_agent_cli-0.3.8/pyproject.toml` & `qcentroid_agent_cli-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2271 6365 6e74 726f 6964  ame = "qcentroid
 00000020: 2d61 6765 6e74 2d63 6c69 220d 0a76 6572  -agent-cli"..ver
-00000030: 7369 6f6e 203d 2022 302e 332e 3822 0d0a  sion = "0.3.8"..
+00000030: 7369 6f6e 203d 2022 302e 332e 3922 0d0a  sion = "0.3.9"..
 00000040: 6465 7363 7269 7074 696f 6e20 3d20 224c  description = "L
 00000050: 6962 7261 7279 2074 6f20 696e 7465 7261  ibrary to intera
 00000060: 6374 2077 6974 6820 7163 656e 7472 6f69  ct with qcentroi
 00000070: 6420 6167 656e 7420 6170 6922 0d0a 6175  d agent api"..au
 00000080: 7468 6f72 7320 3d20 5b0d 0a20 2022 5143  thors = [..  "QC
 00000090: 656e 7472 6f69 6420 3c69 6e66 6f40 7163  entroid <info@qc
 000000a0: 656e 7472 6f69 642e 7879 7a3e 2220 5d0d  entroid.xyz>" ].
```

### Comparing `qcentroid_agent_cli-0.3.8/qcentroid_agent_cli/__init__.py` & `qcentroid_agent_cli-0.3.9/qcentroid_agent_cli/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -189,7 +189,56 @@
     def end(self):
         self.status(StatusEntity(Status.DONE))
 
     def error(self, be:BaseException):        
         self.status(StatusEntity(Status.FAILED))
         self.sendExecutionLog(str(be)) 
 
+class QCentroidSolverClient:
+    # Init class with base parameters
+    def __init__(self, base_url=None, api_key=None, solver_id=None):
+        self.base_url = api_base_url #default production url
+        
+        if base_url is not None:
+            self.base_url = base_url
+        else:
+            self.base_url = os.environ.get('QCENTROID_PUBLIC_API', api_base_url)
+        if api_key is not None:             
+            self.api_key = api_key
+        else:
+            self.api_key = os.environ.get('QCENTROID_AGENT_API_TOKEN')
+        if solver_id is not None:             
+            self.solver_id = solver_id
+        else:
+            self.solver_id = os.environ.get('QCENTROID_SOLVER_ID')
+
+    def getHeaders(self):
+        return {
+            "Authorization": f"Bearer {self.api_key}",
+            "Accept": "application/json",  # Set the content type based on your API's requirements
+            "Content-Type": "application/json",  # Set the content type based on your API's requirements
+        }
+    #GET [core]/agent/job/{job_name}/data/input
+    def obtainJob(self) -> QCentroidAgentClient:
+        try:
+            response = requests.get(f"{self.base_url}/agent/solver/{self.solver_id}/webhook", headers=self.getHeaders())
+
+            # Check if the request was successful (status code 200)
+            if response.status_code == 200:
+                # Parse and use the response data as needed
+                data = response.json()
+                print("API Response:", data)
+                return QCentroidAgentClient(self.base_url, data.token, data.job_id) #return  QCentroidAgentClient
+            # No jobs
+            if response.status_code == 204:                
+                return None
+            else:
+                print(f"Error: {response.status_code} - {response.text}")
+                response.raise_for_status()
+
+        except requests.RequestException as e:
+            print(f"Request failed: {e}")
+            raise e            
+        except Exception as e:
+            # Handle any exceptions or errors here
+            print(f"Unexpected Error: {e}")
+            raise e
```

### Comparing `qcentroid_agent_cli-0.3.8/qcentroid_agent_cli/model/StatusEntity.py` & `qcentroid_agent_cli-0.3.9/qcentroid_agent_cli/model/StatusEntity.py`

 * *Files identical despite different names*

### Comparing `qcentroid_agent_cli-0.3.8/PKG-INFO` & `qcentroid_agent_cli-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcentroid-agent-cli
-Version: 0.3.8
+Version: 0.3.9
 Summary: Library to interact with qcentroid agent api
 License: MIT
 Author: QCentroid
 Author-email: info@qcentroid.xyz
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

