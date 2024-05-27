# Comparing `tmp/examon_core-2.0.2.tar.gz` & `tmp/examon_core-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "examon_core-2.0.2.tar", max compression
+gzip compressed data, was "examon_core-2.0.4.tar", max compression
```

## Comparing `examon_core-2.0.2.tar` & `examon_core-2.0.4.tar`

### file list

```diff
@@ -1,45 +1,48 @@
--rw-r--r--   0        0        0        0 2024-05-18 14:31:03.633904 examon_core-2.0.2/examon_core/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 16:51:06.661649 examon_core-2.0.2/examon_core/code_execution/__init__.py
--rw-r--r--   0        0        0      179 2024-05-09 16:51:06.661857 examon_core-2.0.2/examon_core/code_execution/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1192 2024-05-09 16:51:06.661998 examon_core-2.0.2/examon_core/code_execution/__pycache__/print_collector.cpython-39.pyc
--rw-r--r--   0        0        0     1558 2024-05-09 16:51:06.662136 examon_core-2.0.2/examon_core/code_execution/__pycache__/restricted_python_driver.cpython-39.pyc
--rw-r--r--   0        0        0     1381 2024-05-09 16:51:06.662279 examon_core-2.0.2/examon_core/code_execution/__pycache__/unrestricted_driver.cpython-39.pyc
--rw-r--r--   0        0        0      431 2024-05-19 04:26:54.793493 examon_core-2.0.2/examon_core/code_execution/code_execution_sandbox.py
--rw-r--r--   0        0        0      870 2024-05-19 04:26:54.804105 examon_core-2.0.2/examon_core/code_execution/unrestricted_driver.py
--rwxr-xr-x   0        0        0     1798 2024-05-20 03:05:37.574514 examon_core-2.0.2/examon_core/examon.py
--rw-r--r--   0        0        0        0 2024-05-19 00:55:24.523321 examon_core-2.0.2/examon_core/factories/__init__.py
--rw-r--r--   0        0        0      491 2024-05-19 04:45:32.637915 examon_core-2.0.2/examon_core/factories/default_code_to_string_factory.py
--rw-r--r--   0        0        0     4291 2024-05-20 03:07:24.029505 examon_core-2.0.2/examon_core/factories/examon.py
--rw-r--r--   0        0        0     1457 2024-05-20 03:07:24.031498 examon_core-2.0.2/examon_core/factories/metrics.py
--rw-r--r--   0        0        0      529 2024-05-20 03:07:24.027027 examon_core-2.0.2/examon_core/factories/multi_choice.py
--rw-r--r--   0        0        0      585 2024-05-20 03:07:24.036386 examon_core-2.0.2/examon_core/factories/question.py
--rw-r--r--   0        0        0      220 2024-05-20 01:39:45.912421 examon_core-2.0.2/examon_core/filter_options.py
--rw-r--r--   0        0        0      276 2024-05-18 23:56:59.870681 examon_core-2.0.2/examon_core/generate_unique_id.py
--rw-r--r--   0        0        0      924 2024-05-20 03:04:14.951626 examon_core-2.0.2/examon_core/global_settings.py
--rw-r--r--   0        0        0     1915 2024-05-20 01:25:50.546495 examon_core-2.0.2/examon_core/gof/decorators.py
--rwxr-xr-x   0        0        0     2219 2024-05-20 02:59:35.917403 examon_core-2.0.2/examon_core/in_memory_db.py
--rw-r--r--   0        0        0        0 2024-05-09 16:51:06.663463 examon_core-2.0.2/examon_core/metrics/__init__.py
--rw-r--r--   0        0        0      609 2024-05-20 01:37:01.972038 examon_core-2.0.2/examon_core/metrics/calc_standard_metrics.py
--rw-r--r--   0        0        0      459 2024-05-20 01:52:59.926637 examon_core-2.0.2/examon_core/metrics/categorize_difficulty.py
--rw-r--r--   0        0        0     1450 2024-05-20 03:07:24.033821 examon_core-2.0.2/examon_core/metrics/code_analysis_visitor.py
--rw-r--r--   0        0        0     1340 2024-05-09 16:51:06.663807 examon_core-2.0.2/examon_core/metrics/visit_methods.py
--rw-r--r--   0        0        0        0 2024-05-09 16:51:06.663934 examon_core-2.0.2/examon_core/models/__init__.py
--rw-r--r--   0        0        0      171 2024-05-09 16:51:06.664099 examon_core-2.0.2/examon_core/models/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      558 2024-05-09 16:51:06.664204 examon_core-2.0.2/examon_core/models/__pycache__/question_response.cpython-39.pyc
--rw-r--r--   0        0        0      831 2024-05-19 00:25:51.055946 examon_core-2.0.2/examon_core/models/code_metrics.py
--rwxr-xr-x   0        0        0     1848 2024-05-20 03:05:54.150617 examon_core-2.0.2/examon_core/models/python_code_convertor.py
--rwxr-xr-x   0        0        0      494 2024-05-20 03:05:37.571308 examon_core-2.0.2/examon_core/models/question.py
--rwxr-xr-x   0        0        0      201 2024-05-20 03:05:37.567459 examon_core-2.0.2/examon_core/models/question_response.py
--rw-r--r--   0        0        0      630 2024-05-20 01:40:58.773783 examon_core-2.0.2/examon_core/protocols/__init__.py
--rw-r--r--   0        0        0      115 2024-05-19 04:49:09.721246 examon_core-2.0.2/examon_core/protocols/code_decorator.py
--rw-r--r--   0        0        0      203 2024-05-19 00:44:19.220131 examon_core-2.0.2/examon_core/protocols/code_execution_driver_protocol.py
--rw-r--r--   0        0        0      116 2024-05-19 04:40:01.985333 examon_core-2.0.2/examon_core/protocols/code_metrics_protocol.py
--rw-r--r--   0        0        0       96 2024-05-19 04:46:21.579121 examon_core-2.0.2/examon_core/protocols/difficulty_protocol.py
--rw-r--r--   0        0        0      115 2024-05-19 04:45:34.871822 examon_core-2.0.2/examon_core/protocols/function_to_string_protocol.py
--rw-r--r--   0        0        0      497 2024-05-20 01:35:31.253050 examon_core-2.0.2/examon_core/protocols/item_factory_protocol.py
--rw-r--r--   0        0        0      111 2024-05-19 04:46:30.516801 examon_core-2.0.2/examon_core/protocols/multi_choice_protocol.py
--rw-r--r--   0        0        0      188 2024-05-20 01:38:12.228860 examon_core-2.0.2/examon_core/protocols/question.py
--rw-r--r--   0        0        0      113 2024-05-18 23:40:49.036245 examon_core-2.0.2/examon_core/protocols/unique_id.py
--rw-r--r--   0        0        0      193 2024-05-20 01:44:56.733479 examon_core-2.0.2/examon_core/serializer.py
--rw-r--r--   0        0        0      463 2024-05-20 05:31:13.278636 examon_core-2.0.2/pyproject.toml
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 examon_core-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-18 14:31:03.633904 examon_core-2.0.4/examon_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 16:51:06.661649 examon_core-2.0.4/examon_core/code_execution/__init__.py
+-rw-r--r--   0        0        0      179 2024-05-09 16:51:06.661857 examon_core-2.0.4/examon_core/code_execution/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1192 2024-05-09 16:51:06.661998 examon_core-2.0.4/examon_core/code_execution/__pycache__/print_collector.cpython-39.pyc
+-rw-r--r--   0        0        0     1558 2024-05-09 16:51:06.662136 examon_core-2.0.4/examon_core/code_execution/__pycache__/restricted_python_driver.cpython-39.pyc
+-rw-r--r--   0        0        0     1381 2024-05-09 16:51:06.662279 examon_core-2.0.4/examon_core/code_execution/__pycache__/unrestricted_driver.cpython-39.pyc
+-rw-r--r--   0        0        0      431 2024-05-19 04:26:54.793493 examon_core-2.0.4/examon_core/code_execution/code_execution_sandbox.py
+-rw-r--r--   0        0        0      852 2024-05-23 23:41:50.955170 examon_core-2.0.4/examon_core/code_execution/unrestricted_driver.py
+-rwxr-xr-x   0        0        0     2023 2024-05-24 09:08:26.278960 examon_core-2.0.4/examon_core/examon.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:00:45.863555 examon_core-2.0.4/examon_core/factories/__init__.py
+-rw-r--r--   0        0        0      431 2024-05-24 09:17:07.126880 examon_core-2.0.4/examon_core/factories/code_to_string.py
+-rw-r--r--   0        0        0     4896 2024-05-24 09:15:13.819763 examon_core-2.0.4/examon_core/factories/examon.py
+-rw-r--r--   0        0        0      213 2024-05-24 09:09:42.206053 examon_core-2.0.4/examon_core/factories/hints.py
+-rw-r--r--   0        0        0     1444 2024-05-27 10:06:46.307235 examon_core-2.0.4/examon_core/factories/metrics.py
+-rw-r--r--   0        0        0      492 2024-05-24 00:18:31.291990 examon_core-2.0.4/examon_core/factories/multi_choice.py
+-rw-r--r--   0        0        0      198 2024-05-24 03:52:20.394013 examon_core-2.0.4/examon_core/factories/tags.py
+-rw-r--r--   0        0        0      220 2024-05-20 01:39:45.912421 examon_core-2.0.4/examon_core/filter_options.py
+-rw-r--r--   0        0        0     1084 2024-05-24 09:01:15.319200 examon_core-2.0.4/examon_core/global_settings.py
+-rw-r--r--   0        0        0     1915 2024-05-20 01:25:50.546495 examon_core-2.0.4/examon_core/gof/decorators.py
+-rwxr-xr-x   0        0        0     2219 2024-05-20 02:59:35.917403 examon_core-2.0.4/examon_core/in_memory_db.py
+-rw-r--r--   0        0        0        0 2024-05-09 16:51:06.663463 examon_core-2.0.4/examon_core/metrics/__init__.py
+-rw-r--r--   0        0        0     1479 2024-05-27 10:12:25.050305 examon_core-2.0.4/examon_core/metrics/code_analysis_visitor.py
+-rw-r--r--   0        0        0      451 2024-05-24 04:03:39.208158 examon_core-2.0.4/examon_core/metrics/difficulty_categorisor.py
+-rw-r--r--   0        0        0      606 2024-05-24 04:01:31.882652 examon_core-2.0.4/examon_core/metrics/standard_metrics_calculator.py
+-rw-r--r--   0        0        0     1340 2024-05-27 10:24:32.111210 examon_core-2.0.4/examon_core/metrics/visit_methods.py
+-rw-r--r--   0        0        0        0 2024-05-09 16:51:06.663934 examon_core-2.0.4/examon_core/models/__init__.py
+-rw-r--r--   0        0        0      171 2024-05-09 16:51:06.664099 examon_core-2.0.4/examon_core/models/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      558 2024-05-09 16:51:06.664204 examon_core-2.0.4/examon_core/models/__pycache__/question_response.cpython-39.pyc
+-rw-r--r--   0        0        0      831 2024-05-19 00:25:51.055946 examon_core-2.0.4/examon_core/models/code_metrics.py
+-rwxr-xr-x   0        0        0     1667 2024-05-24 09:17:07.130110 examon_core-2.0.4/examon_core/models/python_code_convertor.py
+-rwxr-xr-x   0        0        0      494 2024-05-20 03:05:37.571308 examon_core-2.0.4/examon_core/models/question.py
+-rwxr-xr-x   0        0        0      201 2024-05-20 03:05:37.567459 examon_core-2.0.4/examon_core/models/question_response.py
+-rw-r--r--   0        0        0      661 2024-05-24 03:52:36.925874 examon_core-2.0.4/examon_core/protocols/__init__.py
+-rw-r--r--   0        0        0      115 2024-05-19 04:49:09.721246 examon_core-2.0.4/examon_core/protocols/code_decorator.py
+-rw-r--r--   0        0        0      203 2024-05-19 00:44:19.220131 examon_core-2.0.4/examon_core/protocols/code_execution_driver.py
+-rw-r--r--   0        0        0      155 2024-05-27 10:03:02.465170 examon_core-2.0.4/examon_core/protocols/code_metrics.py
+-rw-r--r--   0        0        0      216 2024-05-27 10:03:02.469545 examon_core-2.0.4/examon_core/protocols/difficulty.py
+-rw-r--r--   0        0        0      460 2024-05-24 03:46:31.142785 examon_core-2.0.4/examon_core/protocols/examon.py
+-rw-r--r--   0        0        0      115 2024-05-19 04:45:34.871822 examon_core-2.0.4/examon_core/protocols/function_to_string.py
+-rw-r--r--   0        0        0      152 2024-05-24 00:02:05.524289 examon_core-2.0.4/examon_core/protocols/hints.py
+-rw-r--r--   0        0        0      172 2024-05-24 00:21:49.966082 examon_core-2.0.4/examon_core/protocols/multi_choice.py
+-rw-r--r--   0        0        0      188 2024-05-20 01:38:12.228860 examon_core-2.0.4/examon_core/protocols/question.py
+-rw-r--r--   0        0        0      150 2024-05-24 03:52:20.401163 examon_core-2.0.4/examon_core/protocols/tags.py
+-rw-r--r--   0        0        0      113 2024-05-18 23:40:49.036245 examon_core-2.0.4/examon_core/protocols/unique_id.py
+-rw-r--r--   0        0        0      308 2024-05-24 09:01:15.322759 examon_core-2.0.4/examon_core/serializer.py
+-rw-r--r--   0        0        0      277 2024-05-24 03:58:27.331629 examon_core-2.0.4/examon_core/unique_id_generator.py
+-rw-r--r--   0        0        0      463 2024-05-27 10:25:34.362408 examon_core-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 examon_core-2.0.4/PKG-INFO
```

### Comparing `examon_core-2.0.2/examon_core/code_execution/__pycache__/print_collector.cpython-39.pyc` & `examon_core-2.0.4/examon_core/code_execution/__pycache__/print_collector.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `examon_core-2.0.2/examon_core/code_execution/__pycache__/restricted_python_driver.cpython-39.pyc` & `examon_core-2.0.4/examon_core/code_execution/__pycache__/restricted_python_driver.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `examon_core-2.0.2/examon_core/code_execution/__pycache__/unrestricted_driver.cpython-39.pyc` & `examon_core-2.0.4/examon_core/code_execution/__pycache__/unrestricted_driver.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `examon_core-2.0.2/examon_core/code_execution/unrestricted_driver.py` & `examon_core-2.0.4/examon_core/code_execution/unrestricted_driver.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import builtins
 import io
 from contextlib import redirect_stdout
 from typing import List
 
-from examon_core.protocols.code_execution_driver_protocol import (
-    CodeExecutionDriverProtocol,
-)
+from examon_core.protocols.code_execution_driver import CodeExecutionDriverProtocol
 
 
 class UnrestrictedDriver(CodeExecutionDriverProtocol):
     def __init__(self) -> None:
         self.default_print = builtins.print
 
     def setup(self) -> None:
```

### Comparing `examon_core-2.0.2/examon_core/examon.py` & `examon_core-2.0.4/examon_core/examon.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,55 @@
 from typing import Any, List
 
+from examon_core.factories.examon import ExamonFactory
+from examon_core.global_settings import ExamonGlobalSettings
 from examon_core.protocols import (
     CodeExecutionDriverProtocol,
     CodeMetricsProtocol,
     DifficultyProtocol,
     FunctionToStringProtocol,
+    HintsProtocol,
+    MultiChoiceProtocol,
     UniqueIdProtocol,
 )
 
-from examon_core.factories.examon import ExamonFactory
-from examon_core.global_settings import ExamonGlobalSettings
-
 
 def examon(
     internal_id: str = None,
     choices: List[Any] = None,
-    choice_list: List[Any] = None,
     tags: List[str] = None,
     hints: List[str] = None,
     repository: str = None,
     record_metrics: bool = None,
     version: str = None,
     code_execution_driver_class: CodeExecutionDriverProtocol = None,
-    calc_standard_metrics_strategy: CodeMetricsProtocol = None,
-    categorize_difficulty_strategy: DifficultyProtocol = None,
-    code_to_string: FunctionToStringProtocol = None,
-    unique_id_strategy: UniqueIdProtocol = None,
+    standard_metrics_calculator_class: CodeMetricsProtocol = None,
+    difficulty_categorise_class: DifficultyProtocol = None,
+    function_to_string_class: FunctionToStringProtocol = None,
+    unique_id_class: UniqueIdProtocol = None,
+    multi_choice_class: MultiChoiceProtocol = None,
+    hints_class: HintsProtocol = None,
 ):
     def inner_function(function):
-        processed_question = ExamonFactory.default_instance(
-            code_execution_driver_class=code_execution_driver_class,
-            calc_standard_metrics_strategy=calc_standard_metrics_strategy,
-            categorize_difficulty_strategy=categorize_difficulty_strategy,
-            unique_id_strategy=unique_id_strategy,
-            code_to_string=code_to_string,
-        ).build(
-            function=function,
-            internal_id=internal_id,
-            choice_list=choices or choice_list,
-            tags=tags,
-            hints=hints,
-            repository=(repository or ExamonGlobalSettings.repository),
-            version=version or ExamonGlobalSettings.version,
-            metrics=(record_metrics or ExamonGlobalSettings.record_metrics),
+        ExamonGlobalSettings.database.add(
+            ExamonFactory.default_instance(
+                code_execution_driver_class=code_execution_driver_class,
+                calc_standard_metrics_class=standard_metrics_calculator_class,
+                categorize_difficulty_class=difficulty_categorise_class,
+                unique_id_class=unique_id_class,
+                code_to_string_class=function_to_string_class,
+                multi_choice_factory_class=multi_choice_class,
+                hints_class=hints_class,
+            ).build(
+                function=function,
+                internal_id=internal_id,
+                choices=choices,
+                tags=tags,
+                hints=hints,
+                repository=(repository or ExamonGlobalSettings.repository),
+                version=version or ExamonGlobalSettings.version,
+                metrics=(record_metrics or ExamonGlobalSettings.record_metrics),
+            )
         )
-        ExamonGlobalSettings.in_memory_db.add(processed_question)
         return function
 
     return inner_function
```

### Comparing `examon_core-2.0.2/examon_core/factories/examon.py` & `examon_core-2.0.4/examon_core/factories/examon.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,105 +1,115 @@
 import logging
 from typing import Callable, List, Type
 
-from examon_core.protocols.function_to_string_protocol import FunctionToStringProtocol
-
 from examon_core.code_execution.code_execution_sandbox import CodeExecutionSandbox
 from examon_core.global_settings import ExamonGlobalSettings
+from examon_core.models.question import Question
 from examon_core.protocols import (
     CodeExecutionDriverProtocol,
     CodeMetricsProtocol,
     DifficultyProtocol,
-    ItemFactoryProtocol,
+    ExamonFactoryProtocol,
+    HintsProtocol,
     MultiChoiceProtocol,
     UniqueIdProtocol,
 )
-from .metrics import CodeMetricsFactory
-from .question import QuestionFactory
+from examon_core.protocols.function_to_string import FunctionToStringProtocol
+from examon_core.protocols.tags import TagsProtocol
+
+from .metrics import MetricsFactory
 
 
-class ExamonFactory(ItemFactoryProtocol):
+class ExamonFactory(ExamonFactoryProtocol):
     def __init__(
         self,
         code_execution_driver_class: Type[CodeExecutionDriverProtocol] = None,
         multi_choice_class: Type[MultiChoiceProtocol] = None,
         calc_standard_metrics_class: Type[CodeMetricsProtocol] = None,
         categorize_difficulty_class: Type[DifficultyProtocol] = None,
-        unique_id_strategy: Type[UniqueIdProtocol] = None,
-        code_to_string: Type[FunctionToStringProtocol] = None,
+        unique_id_class: Type[UniqueIdProtocol] = None,
+        function_to_string_class: Type[FunctionToStringProtocol] = None,
+        hints_class: Type[HintsProtocol] = None,
+        tags_class: Type[TagsProtocol] = None,
     ) -> None:
         self.code_execution_driver_class = code_execution_driver_class
         self.multi_choice_class = multi_choice_class
-        self.calc_standard_metrics_strategy = calc_standard_metrics_class
-        self.categorize_difficulty_strategy = categorize_difficulty_class
-        self.unique_id_strategy = unique_id_strategy
-        self.code_to_string = code_to_string
+        self.calc_standard_metrics_class = calc_standard_metrics_class
+        self.categorize_difficulty_class = categorize_difficulty_class
+        self.unique_id_class = unique_id_class
+        self.function_to_string_class = function_to_string_class
+        self.hints_class = hints_class
+        self.tags_class = tags_class
 
     def build(
         self,
         function: Callable = None,
         tags: List[str] = None,
         internal_id: str = None,
         hints: List[str] = None,
         choices: List[str] = None,
-        choice_list: List[str] = None,
         repository: str = None,
         version: str = None,
         metrics: bool = None,
     ):
+        function_src = self.function_to_string_class().build(function)
+        print_logs = CodeExecutionSandbox(self.code_execution_driver_class).execute(
+            function_src
+        )
+        answer = print_logs[-1]
+        question = Question(
+            function_src=function_src,
+            print_logs=print_logs,
+            correct_answer=answer,
+        )
+        question.hints = self.hints_class().build(function_src, answer, hints)
+        question.unique_id = self.unique_id_class().run(question.function_src)
+        question.tags = self.tags_class().build(function_src, answer, tags)
 
-        result_choice_list = self.choice_list_as_string(choices or choice_list)
-        ces = CodeExecutionSandbox(self.code_execution_driver_class)
-
-        function_src = self.code_to_string().build(function)
-
-        question = QuestionFactory(ces).build(function_src)
-
-        if result_choice_list:
-            question.choices = self.multi_choice_class(
-                question.print_logs[-1], choice_list or choices
-            ).build()
+        if choices := self.normalize_choices(choices):
+            question.choices = self.multi_choice_class(answer, choices).build()
 
         if metrics:
-            question.metrics = CodeMetricsFactory(
-                calc_standard_metrics_class=self.calc_standard_metrics_strategy,
-                categorize_difficulty_class=self.categorize_difficulty_strategy,
+            question.metrics = MetricsFactory(
+                calc_standard_metrics_class=self.calc_standard_metrics_class,
+                categorize_difficulty_class=self.categorize_difficulty_class,
             ).build(question.function_src)
 
-        question.hints = hints
         question.internal_id = internal_id
-        question.tags = tags
         question.repository = repository
         question.version = version
 
-        question.unique_id = self.unique_id_strategy().run(question.function_src)
         logging.debug(f"QuestionFactory.build: {question}")
         return question
 
-    def choice_list_as_string(self, choices) -> List[str]:
+    def normalize_choices(self, choices) -> List[str]:
         result_choice_list = []
         if choices:
             result_choice_list = list(map(lambda x: str(x), choices))
         return result_choice_list
 
     @staticmethod
     def default_instance(
         code_execution_driver_class: Type[CodeExecutionDriverProtocol] = None,
         multi_choice_factory_class: Type[MultiChoiceProtocol] = None,
-        calc_standard_metrics_strategy: Type[CodeMetricsProtocol] = None,
-        categorize_difficulty_strategy: Type[DifficultyProtocol] = None,
-        unique_id_strategy: Type[UniqueIdProtocol] = None,
-        code_to_string: Type[FunctionToStringProtocol] = None,
-    ) -> ItemFactoryProtocol:
+        calc_standard_metrics_class: Type[CodeMetricsProtocol] = None,
+        categorize_difficulty_class: Type[DifficultyProtocol] = None,
+        unique_id_class: Type[UniqueIdProtocol] = None,
+        code_to_string_class: Type[FunctionToStringProtocol] = None,
+        hints_class: Type[HintsProtocol] = None,
+        tags_class: Type[TagsProtocol] = None,
+    ) -> ExamonFactoryProtocol:
         return ExamonFactory(
             code_execution_driver_class=code_execution_driver_class
             or ExamonGlobalSettings.code_execution_driver_class,
             multi_choice_class=multi_choice_factory_class
             or ExamonGlobalSettings.multi_choice_class,
-            calc_standard_metrics_class=calc_standard_metrics_strategy
-            or ExamonGlobalSettings.calc_standard_metrics_strategy,
-            categorize_difficulty_class=categorize_difficulty_strategy
-            or ExamonGlobalSettings.categorize_difficulty_strategy,
-            unique_id_strategy=unique_id_strategy
-            or ExamonGlobalSettings.unique_id_strategy,
-            code_to_string=code_to_string or ExamonGlobalSettings.code_to_string,
+            calc_standard_metrics_class=calc_standard_metrics_class
+            or ExamonGlobalSettings.standard_metrics_calculator_class,
+            categorize_difficulty_class=categorize_difficulty_class
+            or ExamonGlobalSettings.difficulty_class_categorisor,
+            unique_id_class=unique_id_class or ExamonGlobalSettings.unique_id_class,
+            function_to_string_class=code_to_string_class
+            or ExamonGlobalSettings.code_to_string_class,
+            hints_class=hints_class or ExamonGlobalSettings.hints_class,
+            tags_class=tags_class or ExamonGlobalSettings.tags_class,
         )
```

### Comparing `examon_core-2.0.2/examon_core/factories/metrics.py` & `examon_core-2.0.4/examon_core/factories/metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Type
 
 from examon_core.metrics.code_analysis_visitor import CodeAnalysisVisitor
 from examon_core.models.code_metrics import CodeMetrics
 from examon_core.protocols import CodeMetricsProtocol, DifficultyProtocol
 
 
-class CodeMetricsFactory(object):
+class MetricsFactory(object):
     def __init__(
         self,
         calc_standard_metrics_class: Type[CodeMetricsProtocol],
         categorize_difficulty_class: Type[DifficultyProtocol],
     ) -> None:
         self.calc_standard_metrics_strategy = calc_standard_metrics_class
         self.categorize_difficulty_strategy = categorize_difficulty_class
@@ -32,11 +32,11 @@
 
         tree = ast.parse(code)
         m = CodeAnalysisVisitor()
         m.visit(tree)
 
         cm.imports = list(m.modules)
         cm.calls = list(m.calls)
-        cm.extra = list(m.counts)
-        logging.debug(f"CodeMetricsFactory.build: {cm}")
+        cm.counts = m.counts
+        logging.debug(f"MetricsFactory.build: {cm}")
 
         return cm
```

### Comparing `examon_core-2.0.2/examon_core/global_settings.py` & `examon_core-2.0.4/examon_core/global_settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from examon_core.code_execution.unrestricted_driver import UnrestrictedDriver
-from examon_core.factories.default_code_to_string_factory import DefaultCodeToStringFactory
+from examon_core.factories.code_to_string import CodeToStringFactory
+from examon_core.factories.hints import HintsFactory
 from examon_core.factories.multi_choice import MultiChoiceFactory
-from examon_core.generate_unique_id import GenerateUniqueId
+from examon_core.factories.tags import TagsFactory
 from examon_core.in_memory_db import InMemoryDB
-from examon_core.metrics.calc_standard_metrics import CalcStandardMetrics
-from examon_core.metrics.categorize_difficulty import CategorizeDifficulty
+from examon_core.metrics.difficulty_categorisor import DifficultyCategorisor
+from examon_core.metrics.standard_metrics_calculator import StandardMetricsCalculator
+from examon_core.unique_id_generator import UniqueIdGenerator
 
 
 class ExamonGlobalSettings:
     record_metrics = True
     repository = None
     version = None
 
+    code_to_string_class = CodeToStringFactory
     code_execution_driver_class = UnrestrictedDriver
+
+    tags_class = TagsFactory
+    hints_class = HintsFactory
     multi_choice_class = MultiChoiceFactory
-    calc_standard_metrics_strategy = CalcStandardMetrics
-    categorize_difficulty_strategy = CategorizeDifficulty
-    unique_id_strategy = GenerateUniqueId
-    code_to_string = DefaultCodeToStringFactory
 
-    in_memory_db = InMemoryDB
+    unique_id_class = UniqueIdGenerator
+    standard_metrics_calculator_class = StandardMetricsCalculator
+    difficulty_class_categorisor = DifficultyCategorisor
+
+    database = InMemoryDB
```

### Comparing `examon_core-2.0.2/examon_core/gof/decorators.py` & `examon_core-2.0.4/examon_core/gof/decorators.py`

 * *Files identical despite different names*

### Comparing `examon_core-2.0.2/examon_core/in_memory_db.py` & `examon_core-2.0.4/examon_core/in_memory_db.py`

 * *Files identical despite different names*

### Comparing `examon_core-2.0.2/examon_core/metrics/calc_standard_metrics.py` & `examon_core-2.0.4/examon_core/metrics/standard_metrics_calculator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from examon_core.protocols.code_metrics_protocol import CodeMetricsProtocol
+from examon_core.protocols.code_metrics import CodeMetricsProtocol
 from radon.metrics import h_visit
 from radon.raw import analyze
 
 
-class CalcStandardMetrics(CodeMetricsProtocol):
+class StandardMetricsCalculator(CodeMetricsProtocol):
     def __init__(self, code: str) -> None:
         self.code = code
 
     def run(self) -> dict[str, float]:
         raw = analyze(self.code)
         visit_data = h_visit(self.code)
         return {
```

### Comparing `examon_core-2.0.2/examon_core/metrics/code_analysis_visitor.py` & `examon_core-2.0.4/examon_core/metrics/code_analysis_visitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 class CodeAnalysisVisitor(ast.NodeVisitor):
     def __init__(self) -> None:
         self.functions = set()
         self.calls = set()
         self.modules = set()
         self.counts = defaultdict(int)
         for visit_method in visit_methods:
+            self.counts[visit_method] = 0
             env_setter = self.make_visit(visit_method)
             method = MethodType(env_setter, self)
             setattr(self, f"visit_{visit_method}", method)
 
     def record(self, node):
         self.counts[type(node).__name__] += 1
 
-    # record
     def visit_FunctionDef(self, node):
         self.functions.add(node.name)
         self.generic_visit(node)
 
     def visit_Call(self, node) -> None:
         if node.func.__class__ == ast.Name:
             self.calls.add(node.func.id)
```

### Comparing `examon_core-2.0.2/examon_core/metrics/visit_methods.py` & `examon_core-2.0.4/examon_core/metrics/visit_methods.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,98 +1,98 @@
 visit_methods = [
-    "Expression",
-    "Return",
-    "ClassDef",
-    "Delete",
-    "NotIn",
-    "comprehension",
-    "ExceptHandler",
-    "arguments",
-    "arg",
-    "keyword",
-    "alias",
-    "withitem",
-    "Index",
-    "Suite",
-    "AugLoad",
-    "AugStore",
-    "Param",
-    "Num",
-    "Str",
-    "Bytes",
-    "NameConstant",
-    "Ellipsis",
-    "Assign",
-    "AugAssign",
+    "Add",
+    "And",
     "AnnAssign",
-    "For",
+    "Assert",
+    "Assign",
     "AsyncFor",
-    "While",
-    "If",
-    "With",
     "AsyncWith",
-    "Raise",
-    "Try",
-    "Assert",
-    "Global",
-    "Nonlocal",
-    "Expr",
-    "Pass",
+    "Attribute",
+    "AugAssign",
+    "AugLoad",
+    "AugStore",
+    "Await",
+    "BinOp",
+    "BitAnd",
+    "BitOr",
+    "BitXor",
+    "BoolOp",
     "Break",
+    "Bytes",
+    "ClassDef",
+    "Compare",
+    "Constant",
     "Continue",
-    "Slice",
-    "BoolOp",
-    "BinOp",
-    "UnaryOp",
-    "Lambda",
-    "IfExp",
+    "Del",
+    "Delete",
     "Dict",
-    "Set",
-    "ListComp",
-    "SetComp",
     "DictComp",
-    "GeneratorExp",
-    "Await",
-    "Yield",
-    "YieldFrom",
-    "Compare",
+    "Div",
+    "Ellipsis",
+    "Eq",
+    "ExceptHandler",
+    "Expr",
+    "Expression",
+    "FloorDiv",
+    "For",
     "FormattedValue",
+    "GeneratorExp",
+    "Global",
+    "Gt",
+    "GtE",
+    "If",
+    "IfExp",
+    "In",
+    "Index",
+    "Invert",
+    "Is",
+    "IsNot",
     "JoinedStr",
-    "Constant",
-    "Attribute",
-    "Subscript",
-    "Starred",
-    "Name",
+    "LShift",
+    "Lambda",
     "List",
-    "Tuple",
-    "Del",
+    "ListComp",
     "Load",
-    "Store",
-    "And",
-    "Or",
-    "Add",
-    "BitAnd",
-    "BitOr",
-    "BitXor",
-    "Div",
-    "FloorDiv",
-    "LShift",
+    "Lt",
+    "LtE",
+    "MatMult",
     "Mod",
     "Mult",
-    "MatMult",
+    "Name",
+    "NameConstant",
+    "Nonlocal",
+    "Not",
+    "NotEq",
+    "NotIn",
+    "Num",
+    "Or",
+    "Param",
+    "Pass",
     "Pow",
     "RShift",
+    "Raise",
+    "Return",
+    "Set",
+    "SetComp",
+    "Slice",
+    "Starred",
+    "Store",
+    "Str",
     "Sub",
-    "Invert",
-    "Not",
+    "Subscript",
+    "Suite",
+    "Try",
+    "Tuple",
     "UAdd",
     "USub",
-    "Eq",
-    "Gt",
-    "GtE",
-    "In",
-    "Is",
-    "IsNot",
-    "Lt",
-    "LtE",
-    "NotEq",
+    "UnaryOp",
+    "While",
+    "With",
+    "Yield",
+    "YieldFrom",
+    "alias",
+    "arg",
+    "arguments",
+    "comprehension",
+    "keyword",
+    "withitem",
 ]
```

### Comparing `examon_core-2.0.2/examon_core/models/__pycache__/question_response.cpython-39.pyc` & `examon_core-2.0.4/examon_core/models/__pycache__/question_response.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `examon_core-2.0.2/examon_core/models/code_metrics.py` & `examon_core-2.0.4/examon_core/models/code_metrics.py`

 * *Files identical despite different names*

### Comparing `examon_core-2.0.2/examon_core/models/python_code_convertor.py` & `examon_core-2.0.4/examon_core/models/python_code_convertor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import inspect
 import logging
 from typing import List
 
 from examon_core.protocols import CodeDecoratorProtocol
-from examon_core.protocols.function_to_string_protocol import FunctionToStringProtocol
+from examon_core.protocols.function_to_string import FunctionToStringProtocol
 
 
 class PythonCodeConvertor(FunctionToStringProtocol):
     def __init__(self, decorators: List = None) -> None:
         self.decorators = [] if decorators is None else decorators
 
     def build(self, function) -> str:
@@ -21,31 +21,28 @@
         return src_code
 
     def function_src(self, function):
         logging.debug(f"PythonCodeConvertor.function_src: {function}")
         return inspect.getsource(function).strip()
 
 
-class SourceCodeCommentsDecorator(CodeDecoratorProtocol):
+class SourceCodeComments(CodeDecoratorProtocol):
     def __init__(self, hints: List[str]) -> None:
         self.hints = hints or []
 
     def decorate(self, src_code) -> str:
         all_hints = "\n".join(f"# {hint}" for hint in self.hints)
         return f"# Hints:\n{all_hints}\n\n{src_code}" if all_hints else src_code
 
 
-class RemoveQuizItemDecorator(CodeDecoratorProtocol):
+class RemovePythonDecorators(CodeDecoratorProtocol):
     def decorate(self, src_code) -> str:
         return src_code[src_code.find("def") :]
 
 
-class AppendPrintDecorator(CodeDecoratorProtocol):
-    def __init__(self, function_name, param="") -> None:
+class AppendPrint(CodeDecoratorProtocol):
+    def __init__(self, function_name) -> None:
         self.function_name = function_name
-        self.param = param
 
     def decorate(self, src_code) -> str:
-        if isinstance(self.param, str) and self.param != "":
-            self.param = f"'{self.param}'"
-        println = f"\n\nprint({self.function_name}({self.param}))"
+        println = f"\n\nprint({self.function_name}())"
         return src_code + println
```

