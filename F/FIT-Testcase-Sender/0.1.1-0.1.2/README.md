# Comparing `tmp/FIT_Testcase_Sender-0.1.1.tar.gz` & `tmp/FIT_Testcase_Sender-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FIT_Testcase_Sender-0.1.1.tar", last modified: Sun May 26 23:19:40 2024, max compression
+gzip compressed data, was "FIT_Testcase_Sender-0.1.2.tar", last modified: Mon May 27 03:21:13 2024, max compression
```

## Comparing `FIT_Testcase_Sender-0.1.1.tar` & `FIT_Testcase_Sender-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 23:19:40.939489 FIT_Testcase_Sender-0.1.1/
-drwxrwxrwx   0        0        0        0 2024-05-26 23:19:40.937489 FIT_Testcase_Sender-0.1.1/FIT_Testcase_Sender.egg-info/
--rw-rw-rw-   0        0        0      687 2024-05-26 23:19:40.000000 FIT_Testcase_Sender-0.1.1/FIT_Testcase_Sender.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-26 23:19:40.000000 FIT_Testcase_Sender-0.1.1/FIT_Testcase_Sender.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 23:19:40.000000 FIT_Testcase_Sender-0.1.1/FIT_Testcase_Sender.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-26 23:19:40.000000 FIT_Testcase_Sender-0.1.1/FIT_Testcase_Sender.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      687 2024-05-26 23:19:40.937489 FIT_Testcase_Sender-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      297 2024-05-26 23:19:27.000000 FIT_Testcase_Sender-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 23:19:40.935489 FIT_Testcase_Sender-0.1.1/fit_testcase_sender/
--rw-rw-rw-   0        0        0       21 2024-05-26 23:15:00.000000 FIT_Testcase_Sender-0.1.1/fit_testcase_sender/__init__.py
--rw-rw-rw-   0        0        0      713 2024-05-26 23:03:51.000000 FIT_Testcase_Sender-0.1.1/fit_testcase_sender/func.py
--rw-rw-rw-   0        0        0       42 2024-05-26 23:19:40.939489 FIT_Testcase_Sender-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      582 2024-05-26 23:05:05.000000 FIT_Testcase_Sender-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 03:21:13.231640 FIT_Testcase_Sender-0.1.2/
+drwxrwxrwx   0        0        0        0 2024-05-27 03:21:13.229640 FIT_Testcase_Sender-0.1.2/FIT_Testcase_Sender.egg-info/
+-rw-rw-rw-   0        0        0      687 2024-05-27 03:21:13.000000 FIT_Testcase_Sender-0.1.2/FIT_Testcase_Sender.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-27 03:21:13.000000 FIT_Testcase_Sender-0.1.2/FIT_Testcase_Sender.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 03:21:13.000000 FIT_Testcase_Sender-0.1.2/FIT_Testcase_Sender.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-27 03:21:13.000000 FIT_Testcase_Sender-0.1.2/FIT_Testcase_Sender.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      687 2024-05-27 03:21:13.230641 FIT_Testcase_Sender-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2024-05-26 23:19:27.000000 FIT_Testcase_Sender-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 03:21:13.228640 FIT_Testcase_Sender-0.1.2/fit_testcase_sender/
+-rw-rw-rw-   0        0        0       21 2024-05-27 02:59:33.000000 FIT_Testcase_Sender-0.1.2/fit_testcase_sender/__init__.py
+-rw-rw-rw-   0        0        0      719 2024-05-27 02:59:23.000000 FIT_Testcase_Sender-0.1.2/fit_testcase_sender/func.py
+-rw-rw-rw-   0        0        0       42 2024-05-27 03:21:13.231640 FIT_Testcase_Sender-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      582 2024-05-27 03:09:15.000000 FIT_Testcase_Sender-0.1.2/setup.py
```

### Comparing `FIT_Testcase_Sender-0.1.1/FIT_Testcase_Sender.egg-info/PKG-INFO` & `FIT_Testcase_Sender-0.1.2/FIT_Testcase_Sender.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FIT_Testcase_Sender
-Version: 0.1.1
+Version: 0.1.2
 Summary: A utility for sending scenarios via TCP/IP and checking their completion
 Author: suresofttech
 Author-email: sdhan@suresofttch.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `FIT_Testcase_Sender-0.1.1/PKG-INFO` & `FIT_Testcase_Sender-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FIT_Testcase_Sender
-Version: 0.1.1
+Version: 0.1.2
 Summary: A utility for sending scenarios via TCP/IP and checking their completion
 Author: suresofttech
 Author-email: sdhan@suresofttch.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `FIT_Testcase_Sender-0.1.1/fit_testcase_sender/func.py` & `FIT_Testcase_Sender-0.1.2/fit_testcase_sender/func.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,10 +9,10 @@
     def excute_testcase(self, scenario_number: list) -> dict:
         with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
             scenario_number = {"ScenarioNo": scenario_number}
             sock.connect((self.ip_address, self.port))
             sock.sendall(json.dumps(scenario_number).encode('utf-8') + b'\n')
             return json.loads(sock.recv(1024).decode('utf-8'))       
     
-    def is_testcase_result(scenario_response: dict) -> bool:
+    def is_testcase_result(self, scenario_response: dict) -> bool:
         return scenario_response['Result'] == 'Complete'
```

### Comparing `FIT_Testcase_Sender-0.1.1/setup.py` & `FIT_Testcase_Sender-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FIT_Testcase_Sender',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     description='A utility for sending scenarios via TCP/IP and checking their completion',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='suresofttech',
     author_email='sdhan@suresofttch.com',
     license='MIT',
```

