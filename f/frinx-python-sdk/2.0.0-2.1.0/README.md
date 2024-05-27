# Comparing `tmp/frinx_python_sdk-2.0.0.tar.gz` & `tmp/frinx_python_sdk-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frinx_python_sdk-2.0.0.tar", max compression
+gzip compressed data, was "frinx_python_sdk-2.1.0.tar", max compression
```

## Comparing `frinx_python_sdk-2.0.0.tar` & `frinx_python_sdk-2.1.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1239 2024-03-22 14:03:52.910737 frinx_python_sdk-2.0.0/README.md
--rw-r--r--   0        0        0        0 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/client/__init__.py
--rw-r--r--   0        0        0      134 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/client/frinx_conductor_wrapper.py
--rw-r--r--   0        0        0        0 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/client/v1/__init__.py
--rw-r--r--   0        0        0    12317 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/client/v1/conductor.py
--rw-r--r--   0        0        0    10107 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/client/v1/frinx_conductor_wrapper.py
--rw-r--r--   0        0        0        0 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/client/v2/__init__.py
--rw-r--r--   0        0        0    12317 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/client/v2/conductor.py
--rw-r--r--   0        0        0     9808 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/client/v2/frinx_conductor_wrapper.py
--rw-r--r--   0        0        0        0 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/__init__.py
--rw-r--r--   0        0        0      836 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/conductor_enums.py
--rw-r--r--   0        0        0     1907 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/frinx_rest.py
--rw-r--r--   0        0        0        0 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/graphql/__init__.py
--rw-r--r--   0        0        0     3961 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/graphql/client.py
--rw-r--r--   0        0        0     3213 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/import_workflows.py
--rw-r--r--   0        0        0      115 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/logging/__init__.py
--rw-r--r--   0        0        0      739 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/logging/logging-config.json
--rw-r--r--   0        0        0     3537 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/logging/logging_common.py
--rw-r--r--   0        0        0        0 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/telemetry/__init__.py
--rw-r--r--   0        0        0     5247 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/telemetry/common.py
--rw-r--r--   0        0        0     1993 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/telemetry/enums.py
--rw-r--r--   0        0        0     3574 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/telemetry/metrics.py
--rw-r--r--   0        0        0      187 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/type_aliases.py
--rw-r--r--   0        0        0     2819 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/util.py
--rw-r--r--   0        0        0        0 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/worker/__init__.py
--rw-r--r--   0        0        0     2182 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/worker/service.py
--rw-r--r--   0        0        0     2937 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/worker/task.py
--rw-r--r--   0        0        0     4228 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/worker/task_def.py
--rw-r--r--   0        0        0     1159 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/worker/task_result.py
--rw-r--r--   0        0        0    16610 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/worker/worker.py
--rw-r--r--   0        0        0    13581 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/workflow/WORKFLOW_GENERATOR.md
--rw-r--r--   0        0        0        0 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/workflow/__init__.py
--rw-r--r--   0        0        0     2773 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/workflow/service.py
--rw-r--r--   0        0        0    17751 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/workflow/task.py
--rw-r--r--   0        0        0     5564 2024-03-22 14:03:52.914737 frinx_python_sdk-2.0.0/frinx/common/workflow/workflow.py
--rw-r--r--   0        0        0     2922 2024-03-22 14:04:10.662753 frinx_python_sdk-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1967 1970-01-01 00:00:00.000000 frinx_python_sdk-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1239 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/client/__init__.py
+-rw-r--r--   0        0        0      134 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/client/frinx_conductor_wrapper.py
+-rw-r--r--   0        0        0        0 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/client/v1/__init__.py
+-rw-r--r--   0        0        0    12317 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/client/v1/conductor.py
+-rw-r--r--   0        0        0    10107 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/client/v1/frinx_conductor_wrapper.py
+-rw-r--r--   0        0        0        0 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/client/v2/__init__.py
+-rw-r--r--   0        0        0    12317 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/client/v2/conductor.py
+-rw-r--r--   0        0        0     9808 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/client/v2/frinx_conductor_wrapper.py
+-rw-r--r--   0        0        0        0 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/__init__.py
+-rw-r--r--   0        0        0      836 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/conductor_enums.py
+-rw-r--r--   0        0        0     1907 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/frinx_rest.py
+-rw-r--r--   0        0        0        0 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/graphql/__init__.py
+-rw-r--r--   0        0        0     3961 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/graphql/client.py
+-rw-r--r--   0        0        0     3213 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/import_workflows.py
+-rw-r--r--   0        0        0      115 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/logging/__init__.py
+-rw-r--r--   0        0        0      739 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/logging/logging-config.json
+-rw-r--r--   0        0        0     3537 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/logging/logging_common.py
+-rw-r--r--   0        0        0        0 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/telemetry/__init__.py
+-rw-r--r--   0        0        0     5247 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/telemetry/common.py
+-rw-r--r--   0        0        0     1993 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/telemetry/enums.py
+-rw-r--r--   0        0        0     3574 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/telemetry/metrics.py
+-rw-r--r--   0        0        0      187 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/type_aliases.py
+-rw-r--r--   0        0        0     2819 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/util.py
+-rw-r--r--   0        0        0        0 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/worker/__init__.py
+-rw-r--r--   0        0        0     2182 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/worker/service.py
+-rw-r--r--   0        0        0     2937 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/worker/task.py
+-rw-r--r--   0        0        0     5900 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/worker/task_def.py
+-rw-r--r--   0        0        0     1159 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/worker/task_result.py
+-rw-r--r--   0        0        0    16666 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/worker/worker.py
+-rw-r--r--   0        0        0    13581 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/workflow/WORKFLOW_GENERATOR.md
+-rw-r--r--   0        0        0        0 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/workflow/__init__.py
+-rw-r--r--   0        0        0     2773 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/workflow/service.py
+-rw-r--r--   0        0        0    17751 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/workflow/task.py
+-rw-r--r--   0        0        0     5564 2024-05-27 07:34:59.603936 frinx_python_sdk-2.1.0/frinx/common/workflow/workflow.py
+-rw-r--r--   0        0        0     2922 2024-05-27 07:35:10.095831 frinx_python_sdk-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1967 1970-01-01 00:00:00.000000 frinx_python_sdk-2.1.0/PKG-INFO
```

### Comparing `frinx_python_sdk-2.0.0/README.md` & `frinx_python_sdk-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-2.0.0/frinx/client/v1/conductor.py` & `frinx_python_sdk-2.1.0/frinx/client/v1/conductor.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-2.0.0/frinx/client/v1/frinx_conductor_wrapper.py` & `frinx_python_sdk-2.1.0/frinx/client/v1/frinx_conductor_wrapper.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-2.0.0/frinx/client/v2/conductor.py` & `frinx_python_sdk-2.1.0/frinx/client/v2/conductor.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-2.0.0/frinx/client/v2/frinx_conductor_wrapper.py` & `frinx_python_sdk-2.1.0/frinx/client/v2/frinx_conductor_wrapper.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-2.0.0/frinx/common/conductor_enums.py` & `frinx_python_sdk-2.1.0/frinx/common/conductor_enums.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-2.0.0/frinx/common/frinx_rest.py` & `frinx_python_sdk-2.1.0/frinx/common/frinx_rest.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-2.0.0/frinx/common/graphql/client.py` & `frinx_python_sdk-2.1.0/frinx/common/graphql/client.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-2.0.0/frinx/common/import_workflows.py` & `frinx_python_sdk-2.1.0/frinx/common/import_workflows.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-2.0.0/frinx/common/logging/logging-config.json` & `frinx_python_sdk-2.1.0/frinx/common/logging/logging-config.json`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-2.0.0/frinx/common/logging/logging_common.py` & `frinx_python_sdk-2.1.0/frinx/common/logging/logging_common.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-2.0.0/frinx/common/telemetry/common.py` & `frinx_python_sdk-2.1.0/frinx/common/telemetry/common.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-2.0.0/frinx/common/telemetry/enums.py` & `frinx_python_sdk-2.1.0/frinx/common/telemetry/enums.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-2.0.0/frinx/common/telemetry/metrics.py` & `frinx_python_sdk-2.1.0/frinx/common/telemetry/metrics.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-2.0.0/frinx/common/util.py` & `frinx_python_sdk-2.1.0/frinx/common/util.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-2.0.0/frinx/common/worker/service.py` & `frinx_python_sdk-2.1.0/frinx/common/worker/service.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-2.0.0/frinx/common/worker/task.py` & `frinx_python_sdk-2.1.0/frinx/common/worker/task.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-2.0.0/frinx/common/worker/task_result.py` & `frinx_python_sdk-2.1.0/frinx/common/worker/task_result.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-2.0.0/frinx/common/worker/worker.py` & `frinx_python_sdk-2.1.0/frinx/common/worker/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,27 +220,29 @@
         execution_properties: TaskExecutionProperties = kwargs.get('execution_properties', TaskExecutionProperties())
 
         task_result: TaskResult[Any] = TaskResult(
             status=TaskResultStatus.FAILED,
             logs=[TaskExecLog(f'{error_name}: {error}')]
         )
 
-        match error:
-            case ValidationError():
-                formatted_error: DictAny = self._validate_exception_format(error)
-                task_result.logs = [TaskExecLog(f'{error_name}: {formatted_error}')]
-
-                if execution_properties.pass_worker_input_exception_to_task_output:
-                    task_result.output = self._parse_exception_output_path_to_dict(
-                        dot_path={
-                            execution_properties.worker_input_exception_task_output_path: formatted_error
-                        }
-                    )
+        if execution_properties.pass_worker_input_exception_to_task_output:
+            match error:
+                case ValidationError():
+                    error_info: str | DictAny = self._validate_exception_format(error)
+                case _:
+                    error_info = str(error)
+
+            error_dict = {'error_name': error_name, 'error_info': error_info}
+            error_dict_with_output_path = self._parse_exception_output_path_to_dict(
+                dot_path={execution_properties.pass_task_error_to_task_output_path: error_dict})
+
+            task_result.output = TaskOutput(**error_dict_with_output_path)
+
+            logger.error('%s error occurred: %s \n%s', error_name, error, str(traceback.format_exc()))
 
-        logger.error('%s error occurred: %s \n%s', error_name, error, str(traceback.format_exc()))
         return task_result
 
     def execute_wrapper(self, task: RawTaskIO) -> Any:
         """Wrap the execution of the worker logic.
 
         This internal method wraps the execution of the worker logic, handling the task type
         and reporting any errors or exceptions that may occur during execution.
```

### Comparing `frinx_python_sdk-2.0.0/frinx/common/workflow/WORKFLOW_GENERATOR.md` & `frinx_python_sdk-2.1.0/frinx/common/workflow/WORKFLOW_GENERATOR.md`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-2.0.0/frinx/common/workflow/service.py` & `frinx_python_sdk-2.1.0/frinx/common/workflow/service.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-2.0.0/frinx/common/workflow/task.py` & `frinx_python_sdk-2.1.0/frinx/common/workflow/task.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-2.0.0/frinx/common/workflow/workflow.py` & `frinx_python_sdk-2.1.0/frinx/common/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-2.0.0/pyproject.toml` & `frinx_python_sdk-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 [tool.poetry]
 packages = [{ include = "frinx" }]
 name = "frinx-python-sdk"
 description = "Python SDK for Frinx Machine Workflow Manager"
 authors = ["Jozef Volak <jozef.volak@elisapolystar.com>",
     "Maros Marsalek <maros.marsalek@elisapolystar.com>"]
-version = "v2.0.0" # dynamically generated
+version = "v2.1.0" # dynamically generated
 readme = "README.md"
 keywords = ["frinx-machine", "workflow-manager", "conductor"]
 license = "Apache 2.0"
 
 [project.urls]
 Homepage = 'https://github.com/FRINXio/frinx_python_sdk'
 Source = 'https://github.com/FRINXio/frinx_python_sdk'
```

### Comparing `frinx_python_sdk-2.0.0/PKG-INFO` & `frinx_python_sdk-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frinx-python-sdk
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python SDK for Frinx Machine Workflow Manager
 License: Apache 2.0
 Keywords: frinx-machine,workflow-manager,conductor
 Author: Jozef Volak
 Author-email: jozef.volak@elisapolystar.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

