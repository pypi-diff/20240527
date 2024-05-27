# Comparing `tmp/vedro-jira-failed-reporter-2.0.0.tar.gz` & `tmp/vedro_jira_failed_reporter-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vedro-jira-failed-reporter-2.0.0.tar", last modified: Thu Apr  4 15:46:30 2024, max compression
+gzip compressed data, was "vedro_jira_failed_reporter-2.1.0.tar", last modified: Mon May 27 05:21:33 2024, max compression
```

## Comparing `vedro-jira-failed-reporter-2.0.0.tar` & `vedro_jira_failed_reporter-2.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:46:30.814412 vedro-jira-failed-reporter-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-04 15:46:19.000000 vedro-jira-failed-reporter-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-04 15:46:30.814412 vedro-jira-failed-reporter-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-04 15:46:19.000000 vedro-jira-failed-reporter-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-04 15:46:30.814412 vedro-jira-failed-reporter-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-04 15:46:19.000000 vedro-jira-failed-reporter-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:46:30.814412 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-04 15:46:19.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10005 2024-04-04 15:46:19.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/_failed_reporter_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-04 15:46:19.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/_jira_stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-04-04 15:46:19.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-04 15:46:19.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/_traceback.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:46:19.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 15:46:19.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/version
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-04 15:46:19.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:46:30.814412 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-04 15:46:30.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-04 15:46:30.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:46:30.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-04 15:46:30.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-04 15:46:30.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 05:21:33.807608 vedro_jira_failed_reporter-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-27 05:21:23.000000 vedro_jira_failed_reporter-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-27 05:21:33.807608 vedro_jira_failed_reporter-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-27 05:21:23.000000 vedro_jira_failed_reporter-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-27 05:21:33.807608 vedro_jira_failed_reporter-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-27 05:21:23.000000 vedro_jira_failed_reporter-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 05:21:33.807608 vedro_jira_failed_reporter-2.1.0/vedro_jira_failed_reporter/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-27 05:21:23.000000 vedro_jira_failed_reporter-2.1.0/vedro_jira_failed_reporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8798 2024-05-27 05:21:23.000000 vedro_jira_failed_reporter-2.1.0/vedro_jira_failed_reporter/_failed_reporter_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-27 05:21:23.000000 vedro_jira_failed_reporter-2.1.0/vedro_jira_failed_reporter/_jira_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-05-27 05:21:23.000000 vedro_jira_failed_reporter-2.1.0/vedro_jira_failed_reporter/_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-27 05:21:23.000000 vedro_jira_failed_reporter-2.1.0/vedro_jira_failed_reporter/_traceback.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 05:21:23.000000 vedro_jira_failed_reporter-2.1.0/vedro_jira_failed_reporter/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 05:21:23.000000 vedro_jira_failed_reporter-2.1.0/vedro_jira_failed_reporter/version
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-27 05:21:23.000000 vedro_jira_failed_reporter-2.1.0/vedro_jira_failed_reporter/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 05:21:33.807608 vedro_jira_failed_reporter-2.1.0/vedro_jira_failed_reporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-27 05:21:33.000000 vedro_jira_failed_reporter-2.1.0/vedro_jira_failed_reporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-27 05:21:33.000000 vedro_jira_failed_reporter-2.1.0/vedro_jira_failed_reporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 05:21:33.000000 vedro_jira_failed_reporter-2.1.0/vedro_jira_failed_reporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-27 05:21:33.000000 vedro_jira_failed_reporter-2.1.0/vedro_jira_failed_reporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 05:21:33.000000 vedro_jira_failed_reporter-2.1.0/vedro_jira_failed_reporter.egg-info/top_level.txt
```

### Comparing `vedro-jira-failed-reporter-2.0.0/LICENSE` & `vedro_jira_failed_reporter-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vedro-jira-failed-reporter-2.0.0/PKG-INFO` & `vedro_jira_failed_reporter-2.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vedro-jira-failed-reporter
-Version: 2.0.0
+Version: 2.1.0
 Summary: vedro.io plugin for reporting about flaky tests into jira (with plugin enabled in flaky check runs)
 Home-page: https://github.com/ko10ok/vedro-jira-failed-reporter
 Author: Yuriy Sagitov
 Author-email: pro100.ko10ok@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vedro-jira-failed-reporter-2.0.0/README.md` & `vedro_jira_failed_reporter-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `vedro-jira-failed-reporter-2.0.0/setup.py` & `vedro_jira_failed_reporter-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/_failed_reporter_plugin.py` & `vedro_jira_failed_reporter-2.1.0/vedro_jira_failed_reporter/_failed_reporter_plugin.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,20 +47,14 @@
         self._jira_flaky_label = config.jira_flaky_label
         self._reporting_language = config.reporting_language
 
     def subscribe(self, dispatcher: Dispatcher) -> None:
         if self._report_enabled:
             dispatcher.listen(ScenarioFailedEvent, self.on_scenario_failed)
 
-    def _make_search_issue_for_test(self, test_name: str) -> str:
-        filtered_test_name = deepcopy(test_name)
-        for char in self._jira_search_forbidden_symbols:
-            filtered_test_name = filtered_test_name.replace(char, '.')
-        return f'{filtered_test_name}'
-
     def _make_search_test_file_link(self, traceback: TracebackType) -> str:
         return get_traceback_entrypoint_filename(traceback)
 
     def _make_new_issue_summary_for_test(self, test_name: str, priority: str) -> str:
         return self._reporting_language.NEW_ISSUE_SUMMARY.format(
             project_name=self._report_project_name,
             test_name=test_name,
@@ -95,14 +89,15 @@
 
     def _make_jira_comment(self, scenario_result: ScenarioResult) -> str:
         test_name = scenario_result.scenario.subject
         priority = self._get_scenario_priority(scenario_result.scenario)
         fail_error = scenario_result._step_results[-1].exc_info.value
         fail_traceback = scenario_result._step_results[-1].exc_info.traceback
         return self._reporting_language.NEW_COMMENT_TEXT.format(
+            test_name=test_name,
             priority=priority,
             job_link=self._job_full_path,
             traceback=render_tb(fail_traceback),
             error=render_error(fail_error),
         )
 
     def on_scenario_failed(self, event: Union[ScenarioPassedEvent, ScenarioFailedEvent]) -> None:
@@ -115,19 +110,20 @@
         fail_error = str(event.scenario_result._step_results[-1].exc_info.value)
         for exception_error in self._exceptions:
             if re.search(exception_error, fail_error):
                 event.scenario_result.add_extra_details(self._reporting_language.FILTERED_OUT_BY_EXCEPTION_REGEXP)
                 return
 
         test_name = event.scenario_result.scenario.subject
+        test_file = self._make_search_test_file_link(event.scenario_result._step_results[-1].exc_info.traceback)
 
         statuses = ",".join([f'"{status}"' for status in self._jira_search_statuses])
         search_prompt = (
             f'project = {self._jira_project} '
-            f'and text ~ "{self._make_search_issue_for_test(test_name)}" '
+            f'and text ~ "{test_file}" '
             f'and status in ({statuses}) '
             f'and labels = {self._jira_flaky_label} '
             'ORDER BY created'
         )
 
         found_issues = self._jira.search_issues(jql_str=search_prompt)
         if isinstance(found_issues, JiraUnavailable):
@@ -179,51 +175,29 @@
             )
             return
 
         event.scenario_result.add_extra_details(
             self._reporting_language.ISSUE_CREATED.format(jira_server=self._jira_server, issue_key=result_issue.key)
         )
 
-        traceback = event.scenario_result._step_results[-1].exc_info.traceback
-        search_linked_prompt = (
-            f'project = {self._jira_project} '
-            f'and text ~ "{self._make_search_test_file_link(traceback)}" '
-            f'and status in ({statuses}) '
-            f'and labels = {self._jira_flaky_label} '
-            'ORDER BY created'
-        )
-        found_issues = self._jira.search_issues(jql_str=search_linked_prompt)
-        if isinstance(result_issue, JiraUnavailable):
-            return
-        if found_issues:
-            related_issues = ', '.join(
-                [f'{self._jira_server}/browse/{issue.key}' for issue in found_issues if issue.key != result_issue.key])
-            event.scenario_result.add_extra_details(
-                self._reporting_language.RELATED_ISSUES_FOUND.format(
-                    issues=related_issues
-                )
-            )
-            for found_issue in found_issues:
-                self._jira.create_issue_link(result_issue.key, found_issue.key)
-
 
 class FailedJiraReporter(PluginConfig):
     plugin = FailedJiraReporterPlugin
     description = "Report to jira about failed tests"
 
     enabled = True
     report_enabled = False  # enable it when flaky run
 
     jira_server: str = 'https://NOT_SET'
     jira_user: str = 'NOT_SET'
     jira_password: str = 'NOT_SET'
     jira_project: str = 'NOT_SET'
     jira_components: list[str] = []
     jira_labels: list[str] = []
-    jira_flaky_label: str = 'auto_flaky'
+    jira_flaky_label: str = 'flaky'
 
     jira_search_statuses: list[str] = ['Взят в бэклог', 'Open', 'Reopened', 'In Progress']
     jira_search_forbidden_symbols: list[str] = ['[', ']', '"']
     report_project_name: str = 'NOT_SET'
     job_path = '{job_id}'
     job_id: str = 'NOT_SET'
```

### Comparing `vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/_jira_stdout.py` & `vedro_jira_failed_reporter-2.1.0/vedro_jira_failed_reporter/_jira_stdout.py`

 * *Files identical despite different names*

### Comparing `vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/_messages.py` & `vedro_jira_failed_reporter-2.1.0/vedro_jira_failed_reporter/_messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,17 @@
         '{job_link}\n'
         'h2. {{color:#172b4d}}Что нужно сделать{{color}}\n'
         '{{task}}Заскипать vedro-flaky-steps плагином место падения{{task}}\n'
         '{{task}}Разобраться в причине падения и починить тест по необходимости{{task}}'
     ),
     NEW_COMMENT_TEXT=(
         'Повторный флак\n'
+        '{{code:python}}\n'
+        '{test_name}\n'
+        '{{code}}\n'
         'Приоритет теста - {priority}\n'
         '{job_link}\n'
         '{{code:python}}\n'
         '{traceback}\n'
         '--------------------------------------------------------------------------------\n'
         '{error}\n'
         '{{code}}\n'
```

### Comparing `vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/_traceback.py` & `vedro_jira_failed_reporter-2.1.0/vedro_jira_failed_reporter/_traceback.py`

 * *Files identical despite different names*

### Comparing `vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter.egg-info/PKG-INFO` & `vedro_jira_failed_reporter-2.1.0/vedro_jira_failed_reporter.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vedro-jira-failed-reporter
-Version: 2.0.0
+Version: 2.1.0
 Summary: vedro.io plugin for reporting about flaky tests into jira (with plugin enabled in flaky check runs)
 Home-page: https://github.com/ko10ok/vedro-jira-failed-reporter
 Author: Yuriy Sagitov
 Author-email: pro100.ko10ok@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter.egg-info/SOURCES.txt` & `vedro_jira_failed_reporter-2.1.0/vedro_jira_failed_reporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

