# Comparing `tmp/alertpix-0.3.5.tar.gz` & `tmp/alertpix-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alertpix-0.3.5.tar", last modified: Tue May 28 00:02:41 2024, max compression
+gzip compressed data, was "alertpix-0.3.6.tar", last modified: Tue May 28 00:21:33 2024, max compression
```

## Comparing `alertpix-0.3.5.tar` & `alertpix-0.3.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 00:02:41.628178 alertpix-0.3.5/
--rw-rw-rw-   0        0        0      891 2024-05-28 00:02:41.627156 alertpix-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0      325 2024-05-11 22:33:38.000000 alertpix-0.3.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 00:02:41.608116 alertpix-0.3.5/alertpix/
--rw-rw-rw-   0        0        0      122 2024-05-28 00:00:40.000000 alertpix-0.3.5/alertpix/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 00:02:41.624155 alertpix-0.3.5/alertpix/src/
--rw-rw-rw-   0        0        0     1192 2024-05-28 00:01:07.000000 alertpix-0.3.5/alertpix/src/account.py
--rw-rw-rw-   0        0        0      164 2024-05-08 18:05:54.000000 alertpix-0.3.5/alertpix/src/brcode.py
--rw-rw-rw-   0        0        0     1929 2024-05-28 00:01:45.000000 alertpix-0.3.5/alertpix/src/charges.py
--rw-rw-rw-   0        0        0      787 2024-05-08 18:46:56.000000 alertpix-0.3.5/alertpix/src/statics.py
-drwxrwxrwx   0        0        0        0 2024-05-28 00:02:41.626187 alertpix-0.3.5/alertpix.egg-info/
--rw-rw-rw-   0        0        0      891 2024-05-28 00:02:41.000000 alertpix-0.3.5/alertpix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2024-05-28 00:02:41.000000 alertpix-0.3.5/alertpix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 00:02:41.000000 alertpix-0.3.5/alertpix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-28 00:02:41.000000 alertpix-0.3.5/alertpix.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-28 00:02:41.000000 alertpix-0.3.5/alertpix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 00:02:41.629490 alertpix-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1005 2024-05-27 23:54:11.000000 alertpix-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 00:21:33.300575 alertpix-0.3.6/
+-rw-rw-rw-   0        0        0      891 2024-05-28 00:21:33.297613 alertpix-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2024-05-11 22:33:38.000000 alertpix-0.3.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 00:21:33.269091 alertpix-0.3.6/alertpix/
+-rw-rw-rw-   0        0        0      122 2024-05-28 00:00:40.000000 alertpix-0.3.6/alertpix/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 00:21:33.292306 alertpix-0.3.6/alertpix/src/
+-rw-rw-rw-   0        0        0     1192 2024-05-28 00:01:07.000000 alertpix-0.3.6/alertpix/src/account.py
+-rw-rw-rw-   0        0        0      164 2024-05-08 18:05:54.000000 alertpix-0.3.6/alertpix/src/brcode.py
+-rw-rw-rw-   0        0        0     2002 2024-05-28 00:18:28.000000 alertpix-0.3.6/alertpix/src/charges.py
+-rw-rw-rw-   0        0        0      787 2024-05-08 18:46:56.000000 alertpix-0.3.6/alertpix/src/statics.py
+drwxrwxrwx   0        0        0        0 2024-05-28 00:21:33.295630 alertpix-0.3.6/alertpix.egg-info/
+-rw-rw-rw-   0        0        0      891 2024-05-28 00:21:33.000000 alertpix-0.3.6/alertpix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-05-28 00:21:33.000000 alertpix-0.3.6/alertpix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 00:21:33.000000 alertpix-0.3.6/alertpix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-28 00:21:33.000000 alertpix-0.3.6/alertpix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-28 00:21:33.000000 alertpix-0.3.6/alertpix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 00:21:33.300575 alertpix-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1005 2024-05-28 00:20:53.000000 alertpix-0.3.6/setup.py
```

### Comparing `alertpix-0.3.5/PKG-INFO` & `alertpix-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alertpix
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python library for communication with the alertpix api
 Home-page: https://github.com/JoaquimCassano/Alertpix.py
 Author: Joaquim Cassano
 Author-email: joaquim@cassano.com.br
 License: MIT
 Keywords: api,alertpix,payments,pix
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alertpix-0.3.5/alertpix/src/account.py` & `alertpix-0.3.6/alertpix/src/account.py`

 * *Files identical despite different names*

### Comparing `alertpix-0.3.5/alertpix/src/charges.py` & `alertpix-0.3.6/alertpix/src/charges.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 from .brcode import BrCODE
 from .statics import BASEURL
 class Charge():
-    def __init__(self, link:str,  amount:int, comment:str=".", username:str=".",) -> None:
+    def __init__(self, link:str,  amount:int, comment:str=".", username:str=None,) -> None:
         """
         Args:x'
             link (str): Username da conta da twitch que IRÁ RECEBER
             comment (str): Mensagem que o usuário irá receber (OPCIONAL)
             username (str): Nome que o pagante será identificado (OPCIONAL)
             amount (int): Quantia que o usuário irá receber
         """
@@ -20,15 +20,17 @@
     def create(self):
         request  =  requests.post(
             url=f'{BASEURL}/create-charge',
             json={
                 "link": self.link,
                 "amount": self.amount,
                 "comment": self.comment,
-                "userName": self.username
+                "userName": self.username,
+                "anonymous": True if self.username == None else False
+
             },
             headers={"content-type": "application/json"}
             
         )
         if request.status_code == 200:
             self.charge_id = request.json()['data']["id"]
             self.brcode = BrCODE(request.json()['data']["brCode"])
```

### Comparing `alertpix-0.3.5/alertpix/src/statics.py` & `alertpix-0.3.6/alertpix/src/statics.py`

 * *Files identical despite different names*

### Comparing `alertpix-0.3.5/alertpix.egg-info/PKG-INFO` & `alertpix-0.3.6/alertpix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alertpix
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python library for communication with the alertpix api
 Home-page: https://github.com/JoaquimCassano/Alertpix.py
 Author: Joaquim Cassano
 Author-email: joaquim@cassano.com.br
 License: MIT
 Keywords: api,alertpix,payments,pix
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alertpix-0.3.5/setup.py` & `alertpix-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 requirements = [
     "qrcode",
     "requests"
 ]
 
 setuptools.setup(
     name="alertpix",
-    version="0.3.5",
+    version="0.3.6",
     author="Joaquim Cassano",
     license='MIT',
     author_email="joaquim@cassano.com.br",
     description='Python library for communication with the alertpix api',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=requirements,
```

