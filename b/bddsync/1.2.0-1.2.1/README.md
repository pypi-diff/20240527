# Comparing `tmp/bddsync-1.2.0.tar.gz` & `tmp/bddsync-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bddsync-1.2.0.tar", last modified: Fri Mar  8 10:23:03 2024, max compression
+gzip compressed data, was "bddsync-1.2.1.tar", last modified: Mon May 27 12:09:55 2024, max compression
```

## Comparing `bddsync-1.2.0.tar` & `bddsync-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-08 10:23:03.226670 bddsync-1.2.0/
--rw-rw-rw-   0        0        0     1105 2022-09-01 14:24:54.000000 bddsync-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     6126 2024-03-08 10:23:03.226670 bddsync-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     5390 2022-09-01 13:22:28.000000 bddsync-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-08 10:23:03.179787 bddsync-1.2.0/bddsync/
--rw-rw-rw-   0        0        0        0 2024-03-08 09:21:27.000000 bddsync-1.2.0/bddsync/__init__.py
--rw-rw-rw-   0        0        0    15094 2024-03-08 10:19:50.000000 bddsync-1.2.0/bddsync/__main__.py
--rw-rw-rw-   0        0        0     9001 2022-09-01 10:13:47.000000 bddsync-1.2.0/bddsync/cucumber_wrapper.py
--rw-rw-rw-   0        0        0    10433 2024-02-27 14:18:28.000000 bddsync-1.2.0/bddsync/xray_wrapper.py
-drwxrwxrwx   0        0        0        0 2024-03-08 10:23:03.226670 bddsync-1.2.0/bddsync.egg-info/
--rw-rw-rw-   0        0        0     6126 2024-03-08 10:23:03.000000 bddsync-1.2.0/bddsync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2024-03-08 10:23:03.000000 bddsync-1.2.0/bddsync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-08 10:23:03.000000 bddsync-1.2.0/bddsync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-03-08 10:23:03.000000 bddsync-1.2.0/bddsync.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2024-03-08 10:23:03.000000 bddsync-1.2.0/bddsync.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-08 10:23:03.000000 bddsync-1.2.0/bddsync.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-03-08 10:23:03.226670 bddsync-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1209 2024-03-08 10:22:45.000000 bddsync-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:09:55.113230 bddsync-1.2.1/
+-rw-rw-rw-   0        0        0     1105 2024-05-27 12:01:18.000000 bddsync-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     6153 2024-05-27 12:09:55.113230 bddsync-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5390 2024-05-27 12:01:18.000000 bddsync-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 12:09:55.065841 bddsync-1.2.1/bddsync/
+-rw-rw-rw-   0        0        0        0 2024-05-27 12:01:18.000000 bddsync-1.2.1/bddsync/__init__.py
+-rw-rw-rw-   0        0        0    15103 2024-05-27 12:05:54.000000 bddsync-1.2.1/bddsync/__main__.py
+-rw-rw-rw-   0        0        0     9001 2024-05-27 12:01:18.000000 bddsync-1.2.1/bddsync/cucumber_wrapper.py
+-rw-rw-rw-   0        0        0    10433 2024-05-27 12:01:18.000000 bddsync-1.2.1/bddsync/xray_wrapper.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:09:55.113230 bddsync-1.2.1/bddsync.egg-info/
+-rw-rw-rw-   0        0        0     6153 2024-05-27 12:09:54.000000 bddsync-1.2.1/bddsync.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2024-05-27 12:09:54.000000 bddsync-1.2.1/bddsync.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 12:09:54.000000 bddsync-1.2.1/bddsync.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-27 12:09:54.000000 bddsync-1.2.1/bddsync.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2024-05-27 12:09:54.000000 bddsync-1.2.1/bddsync.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-27 12:09:54.000000 bddsync-1.2.1/bddsync.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-27 12:09:55.128867 bddsync-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2024-05-27 12:02:40.000000 bddsync-1.2.1/setup.py
```

### Comparing `bddsync-1.2.0/LICENSE` & `bddsync-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bddsync-1.2.0/PKG-INFO` & `bddsync-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: bddsync
-Version: 1.2.0
+Version: 1.2.1
 Summary: Tools to synchronize BDD files with test management tools like Jira-Xray
 Home-page: https://github.com/Manzanero/bddsync
+Download-URL: https://github.com/Manzanero/bddsync/archive/refs/tags/v1.2.1.tar.gz
 Author: Alejandro Manzanero
 Author-email: alejmans@gmail.com
 License: MIT
-Download-URL: https://github.com/Manzanero/bddsync/archive/refs/tags/v1.2.0.tar.gz
 Keywords: bdd,cucumber,behave,jira,xray,testing
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: PyYAML
 
 # bddsync
 
 Tools to synchronize BDD files with test management tools like Jira-Xray
 
 ## Setting Up
 
@@ -175,8 +176,7 @@
 
 ```
 $ bddsync [...] generate-docs [-h]
 
 optional arguments:
   -h, --help       show this help message and exit
 ```
-
```

### Comparing `bddsync-1.2.0/README.md` & `bddsync-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bddsync-1.2.0/bddsync/__main__.py` & `bddsync-1.2.1/bddsync/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 
 import yaml
 from bddsync.cucumber_wrapper import CucumberWrapper
 from bddsync.xray_wrapper import XrayWrapper
 
 NAME = 'bddsync'
-VERSION = 'v1.2.0'
+VERSION = 'v1.2.1'
 
 
 class Commands:
     TEST_REPOSITORY_FOLDERS = 'test-repository-folders'
     FEATURES = 'features'
     SCENARIOS = 'scenarios'
     UPLOAD_FEATURES = 'upload-features'
@@ -196,27 +196,27 @@
                 continue
 
             issues = xray.get_issue(new_scenario_id,
                                     ['labels', 'status', xray.test_repository_path_field, xray.test_plans_field])
 
             # manage labels
             labels = issues['fields']['labels']
-            if labels_to_remove := [label for label in labels if label not in scenario.effective_tags]:
-                xray.remove_labels(new_scenario_id, labels_to_remove)
+            labels_to_remove = [scenario.id] + [label for label in labels if label not in scenario.effective_tags]
+            xray.remove_labels(new_scenario_id, labels_to_remove)
             if labels_to_add := [tag for tag in feature.tags if tag not in scenario.effective_tags]:
                 xray.add_labels(new_scenario_id, labels_to_add)
 
             # manage path
             test_dir = issues['fields'][xray.test_repository_path_field]
             if scenario.test_dir and scenario.test_dir != test_dir:
                 xray.make_dirs(scenario.test_dir)
                 xray.move_test_dir(new_scenario_id, scenario.test_dir)
 
             # manage plans
-            tracked_test_plans = list(config.get('test_plans', {}).keys())
+            tracked_test_plans = list(config.get('test_plans', {}).values())
             in_xray_test_plans = issues['fields'][xray.test_plans_field]
             in_code_test_plans = [plan.id for plan in scenario.test_plans]
             in_code_test_plans_to_add = [plan for plan in in_code_test_plans if plan not in in_xray_test_plans]
             in_code_test_plans_to_add = [plan for plan in in_code_test_plans_to_add if plan in tracked_test_plans]
             in_xray_test_plans_to_remove = [plan for plan in in_xray_test_plans if plan not in in_code_test_plans]
             in_xray_test_plans_to_remove = [plan for plan in in_xray_test_plans_to_remove if plan in tracked_test_plans]
             xray.add_tests_to_test_plans([new_scenario_id], in_code_test_plans_to_add)
```

### Comparing `bddsync-1.2.0/bddsync/cucumber_wrapper.py` & `bddsync-1.2.1/bddsync/cucumber_wrapper.py`

 * *Files identical despite different names*

### Comparing `bddsync-1.2.0/bddsync/xray_wrapper.py` & `bddsync-1.2.1/bddsync/xray_wrapper.py`

 * *Files identical despite different names*

### Comparing `bddsync-1.2.0/bddsync.egg-info/PKG-INFO` & `bddsync-1.2.1/bddsync.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: bddsync
-Version: 1.2.0
+Version: 1.2.1
 Summary: Tools to synchronize BDD files with test management tools like Jira-Xray
 Home-page: https://github.com/Manzanero/bddsync
+Download-URL: https://github.com/Manzanero/bddsync/archive/refs/tags/v1.2.1.tar.gz
 Author: Alejandro Manzanero
 Author-email: alejmans@gmail.com
 License: MIT
-Download-URL: https://github.com/Manzanero/bddsync/archive/refs/tags/v1.2.0.tar.gz
 Keywords: bdd,cucumber,behave,jira,xray,testing
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: PyYAML
 
 # bddsync
 
 Tools to synchronize BDD files with test management tools like Jira-Xray
 
 ## Setting Up
 
@@ -175,8 +176,7 @@
 
 ```
 $ bddsync [...] generate-docs [-h]
 
 optional arguments:
   -h, --help       show this help message and exit
 ```
-
```

### Comparing `bddsync-1.2.0/setup.py` & `bddsync-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
     name='bddsync',
     packages=['bddsync'],
     entry_points={
         "console_scripts": [
             "bddsync = bddsync.__main__:main"
         ],
     },
-    version='1.2.0',
+    version='1.2.1',
     license='MIT',
     description='Tools to synchronize BDD files with test management tools like Jira-Xray',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Alejandro Manzanero',
     author_email='alejmans@gmail.com',
     url='https://github.com/Manzanero/bddsync',
-    download_url='https://github.com/Manzanero/bddsync/archive/refs/tags/v1.2.0.tar.gz',
+    download_url='https://github.com/Manzanero/bddsync/archive/refs/tags/v1.2.1.tar.gz',
     keywords=['bdd', 'cucumber', 'behave', 'jira', 'xray', 'testing'],
     install_requires=[
         'requests',
         'PyYAML',
     ],
     classifiers=[
         'Development Status :: 4 - Beta',      # "3 - Alpha", "4 - Beta" or "5 - Production/Stable"
```

