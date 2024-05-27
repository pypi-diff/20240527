# Comparing `tmp/FIT_Testcase_Sender-0.1.0.tar.gz` & `tmp/FIT_Testcase_Sender-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FIT_Testcase_Sender-0.1.0.tar", last modified: Fri May 24 06:28:29 2024, max compression
+gzip compressed data, was "FIT_Testcase_Sender-0.1.1.tar", last modified: Sun May 26 23:19:40 2024, max compression
```

## Comparing `FIT_Testcase_Sender-0.1.0.tar` & `FIT_Testcase_Sender-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 06:28:29.933900 FIT_Testcase_Sender-0.1.0/
-drwxrwxrwx   0        0        0        0 2024-05-24 06:28:29.931901 FIT_Testcase_Sender-0.1.0/FIT_Testcase_Sender.egg-info/
--rw-rw-rw-   0        0        0      414 2024-05-24 06:28:29.000000 FIT_Testcase_Sender-0.1.0/FIT_Testcase_Sender.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-24 06:28:29.000000 FIT_Testcase_Sender-0.1.0/FIT_Testcase_Sender.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 06:28:29.000000 FIT_Testcase_Sender-0.1.0/FIT_Testcase_Sender.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-24 06:28:29.000000 FIT_Testcase_Sender-0.1.0/FIT_Testcase_Sender.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      414 2024-05-24 06:28:29.932901 FIT_Testcase_Sender-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       22 2024-05-24 06:28:26.000000 FIT_Testcase_Sender-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 06:28:29.929901 FIT_Testcase_Sender-0.1.0/fit_testcase_sender/
--rw-rw-rw-   0        0        0       21 2024-05-24 06:25:16.000000 FIT_Testcase_Sender-0.1.0/fit_testcase_sender/__init__.py
--rw-rw-rw-   0        0        0      650 2024-05-24 06:25:56.000000 FIT_Testcase_Sender-0.1.0/fit_testcase_sender/func.py
--rw-rw-rw-   0        0        0       42 2024-05-24 06:28:29.933900 FIT_Testcase_Sender-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      582 2024-05-24 06:27:34.000000 FIT_Testcase_Sender-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 23:19:40.939489 FIT_Testcase_Sender-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-05-26 23:19:40.937489 FIT_Testcase_Sender-0.1.1/FIT_Testcase_Sender.egg-info/
+-rw-rw-rw-   0        0        0      687 2024-05-26 23:19:40.000000 FIT_Testcase_Sender-0.1.1/FIT_Testcase_Sender.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-26 23:19:40.000000 FIT_Testcase_Sender-0.1.1/FIT_Testcase_Sender.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 23:19:40.000000 FIT_Testcase_Sender-0.1.1/FIT_Testcase_Sender.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-26 23:19:40.000000 FIT_Testcase_Sender-0.1.1/FIT_Testcase_Sender.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      687 2024-05-26 23:19:40.937489 FIT_Testcase_Sender-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2024-05-26 23:19:27.000000 FIT_Testcase_Sender-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 23:19:40.935489 FIT_Testcase_Sender-0.1.1/fit_testcase_sender/
+-rw-rw-rw-   0        0        0       21 2024-05-26 23:15:00.000000 FIT_Testcase_Sender-0.1.1/fit_testcase_sender/__init__.py
+-rw-rw-rw-   0        0        0      713 2024-05-26 23:03:51.000000 FIT_Testcase_Sender-0.1.1/fit_testcase_sender/func.py
+-rw-rw-rw-   0        0        0       42 2024-05-26 23:19:40.939489 FIT_Testcase_Sender-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      582 2024-05-26 23:05:05.000000 FIT_Testcase_Sender-0.1.1/setup.py
```

### Comparing `FIT_Testcase_Sender-0.1.0/fit_testcase_sender/func.py` & `FIT_Testcase_Sender-0.1.1/fit_testcase_sender/func.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 class FIT_Remote:
     def __init__(self, ip_address: str, port: int) -> None:
         self.ip_address = ip_address
         self.port = port
     
     def excute_testcase(self, scenario_number: list) -> dict:
         with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
+            scenario_number = {"ScenarioNo": scenario_number}
             sock.connect((self.ip_address, self.port))
             sock.sendall(json.dumps(scenario_number).encode('utf-8') + b'\n')
             return json.loads(sock.recv(1024).decode('utf-8'))       
     
     def is_testcase_result(scenario_response: dict) -> bool:
         return scenario_response['Result'] == 'Complete'
```

### Comparing `FIT_Testcase_Sender-0.1.0/setup.py` & `FIT_Testcase_Sender-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FIT_Testcase_Sender',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     description='A utility for sending scenarios via TCP/IP and checking their completion',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='suresofttech',
     author_email='sdhan@suresofttch.com',
     license='MIT',
```

