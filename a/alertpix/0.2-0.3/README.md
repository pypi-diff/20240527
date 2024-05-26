# Comparing `tmp/alertpix-0.2.tar.gz` & `tmp/alertpix-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alertpix-0.2.tar", last modified: Wed May  8 19:27:05 2024, max compression
+gzip compressed data, was "alertpix-0.3.tar", last modified: Mon May 27 02:07:09 2024, max compression
```

## Comparing `alertpix-0.2.tar` & `alertpix-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 tubilo    (1000) tubilo    (1000)        0 2024-05-08 19:27:05.983156 alertpix-0.2/
--rw-rw-r--   0 tubilo    (1000) tubilo    (1000)      819 2024-05-08 19:27:05.983156 alertpix-0.2/PKG-INFO
--rw-rw-r--   0 tubilo    (1000) tubilo    (1000)      308 2024-05-08 18:56:37.000000 alertpix-0.2/README.md
-drwxrwxr-x   0 tubilo    (1000) tubilo    (1000)        0 2024-05-08 19:27:05.983156 alertpix-0.2/alertpix/
--rw-rw-r--   0 tubilo    (1000) tubilo    (1000)      118 2024-05-08 19:06:04.000000 alertpix-0.2/alertpix/__init__.py
-drwxrwxr-x   0 tubilo    (1000) tubilo    (1000)        0 2024-05-08 19:27:05.983156 alertpix-0.2/alertpix.egg-info/
--rw-rw-r--   0 tubilo    (1000) tubilo    (1000)      819 2024-05-08 19:27:05.000000 alertpix-0.2/alertpix.egg-info/PKG-INFO
--rw-rw-r--   0 tubilo    (1000) tubilo    (1000)      198 2024-05-08 19:27:05.000000 alertpix-0.2/alertpix.egg-info/SOURCES.txt
--rw-rw-r--   0 tubilo    (1000) tubilo    (1000)        1 2024-05-08 19:27:05.000000 alertpix-0.2/alertpix.egg-info/dependency_links.txt
--rw-rw-r--   0 tubilo    (1000) tubilo    (1000)       16 2024-05-08 19:27:05.000000 alertpix-0.2/alertpix.egg-info/requires.txt
--rw-rw-r--   0 tubilo    (1000) tubilo    (1000)        9 2024-05-08 19:27:05.000000 alertpix-0.2/alertpix.egg-info/top_level.txt
--rw-rw-r--   0 tubilo    (1000) tubilo    (1000)       38 2024-05-08 19:27:05.983156 alertpix-0.2/setup.cfg
--rw-rw-r--   0 tubilo    (1000) tubilo    (1000)      927 2024-05-08 19:26:35.000000 alertpix-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 02:07:09.834204 alertpix-0.3/
+-rw-rw-rw-   0        0        0      889 2024-05-27 02:07:09.832296 alertpix-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2024-05-11 22:33:38.000000 alertpix-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 02:07:09.807047 alertpix-0.3/alertpix/
+drwxrwxrwx   0        0        0        0 2024-05-27 02:07:09.807047 alertpix-0.3/alertpix/src/
+drwxrwxrwx   0        0        0        0 2024-05-27 02:07:09.831294 alertpix-0.3/alertpix/src/alertpix.egg-info/
+-rw-rw-rw-   0        0        0      889 2024-05-27 02:07:09.000000 alertpix-0.3/alertpix/src/alertpix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2024-05-27 02:07:09.000000 alertpix-0.3/alertpix/src/alertpix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 02:07:09.000000 alertpix-0.3/alertpix/src/alertpix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-27 02:07:09.000000 alertpix-0.3/alertpix/src/alertpix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 02:07:09.000000 alertpix-0.3/alertpix/src/alertpix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 02:07:09.834204 alertpix-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      985 2024-05-27 02:06:33.000000 alertpix-0.3/setup.py
```

### Comparing `alertpix-0.2/PKG-INFO` & `alertpix-0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-Metadata-Version: 2.1
-Name: alertpix
-Version: 0.2
-Summary: Python library for communication with the alertpix api
-Home-page: https://github.com/JoaquimCassano/Alertpix.py
-Author: Joaquim Cassano
-Author-email: joaquim@cassano.com.br
-License: MIT
-Keywords: api,alertpix,payments,pix
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-<div align="center">
-<img src="https://i.imgur.com/ir3vFwk.png" width=100px>
-<br>
-<h1>Alertpix.py</h1>
-
-![OS](https://img.shields.io/badge/OS-linux%20%7C%20windows-blue??style=flat&logo=Linux&logoColor=b0c0c0&labelColor=363D44)
-<br>
-<i>Uma biblioteca python para facilitar o uso da API do AlertPix</i>
-<br>
-
-
-
+Metadata-Version: 2.1
+Name: alertpix
+Version: 0.3
+Summary: Python library for communication with the alertpix api
+Home-page: https://github.com/JoaquimCassano/Alertpix.py
+Author: Joaquim Cassano
+Author-email: joaquim@cassano.com.br
+License: MIT
+Keywords: api,alertpix,payments,pix
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Requires-Dist: qrcode
+Requires-Dist: requests
+
+<div align="center">
+<img src="https://i.imgur.com/ir3vFwk.png" width=100px>
+<br>
+<h1>Alertpix.py</h1>
+
+![OS](https://img.shields.io/badge/OS-linux%20%7C%20windows-blue??style=flat&logo=Linux&logoColor=b0c0c0&labelColor=363D44)
+<br>
+<i>Uma biblioteca *não-oficial* python para facilitar o uso da API do AlertPix</i>  
+<br>
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alertpix-0.2/alertpix.egg-info/PKG-INFO` & `alertpix-0.3/alertpix/src/alertpix.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-Metadata-Version: 2.1
-Name: alertpix
-Version: 0.2
-Summary: Python library for communication with the alertpix api
-Home-page: https://github.com/JoaquimCassano/Alertpix.py
-Author: Joaquim Cassano
-Author-email: joaquim@cassano.com.br
-License: MIT
-Keywords: api,alertpix,payments,pix
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-<div align="center">
-<img src="https://i.imgur.com/ir3vFwk.png" width=100px>
-<br>
-<h1>Alertpix.py</h1>
-
-![OS](https://img.shields.io/badge/OS-linux%20%7C%20windows-blue??style=flat&logo=Linux&logoColor=b0c0c0&labelColor=363D44)
-<br>
-<i>Uma biblioteca python para facilitar o uso da API do AlertPix</i>
-<br>
-
-
-
+Metadata-Version: 2.1
+Name: alertpix
+Version: 0.3
+Summary: Python library for communication with the alertpix api
+Home-page: https://github.com/JoaquimCassano/Alertpix.py
+Author: Joaquim Cassano
+Author-email: joaquim@cassano.com.br
+License: MIT
+Keywords: api,alertpix,payments,pix
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Requires-Dist: qrcode
+Requires-Dist: requests
+
+<div align="center">
+<img src="https://i.imgur.com/ir3vFwk.png" width=100px>
+<br>
+<h1>Alertpix.py</h1>
+
+![OS](https://img.shields.io/badge/OS-linux%20%7C%20windows-blue??style=flat&logo=Linux&logoColor=b0c0c0&labelColor=363D44)
+<br>
+<i>Uma biblioteca *não-oficial* python para facilitar o uso da API do AlertPix</i>  
+<br>
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alertpix-0.2/setup.py` & `alertpix-0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 requirements = [
     "qrcode",
     "requests"
 ]
 
 setuptools.setup(
     name="alertpix",
-    version="0.2",
+    version="0.3",
     author="Joaquim Cassano",
     license='MIT',
     author_email="joaquim@cassano.com.br",
     description='Python library for communication with the alertpix api',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=requirements,
     keywords=["api", "alertpix", "payments", "pix"],
     url="https://github.com/JoaquimCassano/Alertpix.py",
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_packages(where="alertpix/src"),
+    package_dir={"": "alertpix/src"},
     python_requires=">=3.7",
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

