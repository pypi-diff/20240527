# Comparing `tmp/pyVIA-0.1.993.tar.gz` & `tmp/pyVIA-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyVIA-0.1.993.tar", last modified: Tue May  7 07:53:14 2024, max compression
+gzip compressed data, was "pyVIA-0.2.0.tar", last modified: Mon May 27 03:54:10 2024, max compression
```

## Comparing `pyVIA-0.1.993.tar` & `pyVIA-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-07 07:53:14.779527 pyVIA-0.1.993/
--rwxr-xr-x   0 user      (1000) user      (1000)     1091 2020-09-15 01:01:11.000000 pyVIA-0.1.993/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)    19679 2024-05-07 07:53:14.779527 pyVIA-0.1.993/PKG-INFO
--rwxr-xr-x   0 user      (1000) user      (1000)    19436 2021-04-06 00:42:30.000000 pyVIA-0.1.993/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-07 07:53:14.779527 pyVIA-0.1.993/pyVIA/
--rwxr-xr-x   0 user      (1000) user      (1000)      142 2022-08-25 22:07:17.000000 pyVIA-0.1.993/pyVIA/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)   198816 2024-05-07 07:51:17.000000 pyVIA-0.1.993/pyVIA/core.py
--rwxr-xr-x   0 user      (1000) user      (1000)    14901 2024-02-20 06:46:27.000000 pyVIA-0.1.993/pyVIA/datasets_via.py
--rw-rw-r--   0 user      (1000) user      (1000)   160718 2024-02-20 03:31:08.000000 pyVIA-0.1.993/pyVIA/examples.py
--rw-rw-rw-   0 user      (1000) user      (1000)   236438 2024-05-07 07:35:16.000000 pyVIA-0.1.993/pyVIA/plotting_via.py
--rwxr-xr-x   0 user      (1000) user      (1000)    97075 2024-04-12 02:40:43.000000 pyVIA-0.1.993/pyVIA/utils_via.py
--rw-rw-r--   0 user      (1000) user      (1000)     7987 2024-02-20 03:31:08.000000 pyVIA-0.1.993/pyVIA/windmap.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-07 07:53:14.779527 pyVIA-0.1.993/pyVIA.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    19679 2024-05-07 07:53:14.000000 pyVIA-0.1.993/pyVIA.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      304 2024-05-07 07:53:14.000000 pyVIA-0.1.993/pyVIA.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-07 07:53:14.000000 pyVIA-0.1.993/pyVIA.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      211 2024-05-07 07:53:14.000000 pyVIA-0.1.993/pyVIA.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        6 2024-05-07 07:53:14.000000 pyVIA-0.1.993/pyVIA.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-07 07:53:14.779527 pyVIA-0.1.993/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      957 2024-05-07 07:52:30.000000 pyVIA-0.1.993/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-27 03:54:10.729852 pyVIA-0.2.0/
+-rwxr-xr-x   0 user      (1000) user      (1000)     1091 2020-09-15 01:01:11.000000 pyVIA-0.2.0/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)    19677 2024-05-27 03:54:10.729852 pyVIA-0.2.0/PKG-INFO
+-rwxr-xr-x   0 user      (1000) user      (1000)    19436 2021-04-06 00:42:30.000000 pyVIA-0.2.0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-27 03:54:10.725852 pyVIA-0.2.0/pyVIA/
+-rwxr-xr-x   0 user      (1000) user      (1000)      142 2022-08-25 22:07:17.000000 pyVIA-0.2.0/pyVIA/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)   198816 2024-05-27 03:53:35.000000 pyVIA-0.2.0/pyVIA/core.py
+-rwxr-xr-x   0 user      (1000) user      (1000)    14901 2024-02-20 06:46:27.000000 pyVIA-0.2.0/pyVIA/datasets_via.py
+-rw-rw-r--   0 user      (1000) user      (1000)   160718 2024-02-20 03:31:08.000000 pyVIA-0.2.0/pyVIA/examples.py
+-rw-rw-rw-   0 user      (1000) user      (1000)   236438 2024-05-07 07:35:16.000000 pyVIA-0.2.0/pyVIA/plotting_via.py
+-rwxr-xr-x   0 user      (1000) user      (1000)    97075 2024-04-12 02:40:43.000000 pyVIA-0.2.0/pyVIA/utils_via.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7987 2024-02-20 03:31:08.000000 pyVIA-0.2.0/pyVIA/windmap.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-27 03:54:10.725852 pyVIA-0.2.0/pyVIA.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    19677 2024-05-27 03:54:10.000000 pyVIA-0.2.0/pyVIA.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      304 2024-05-27 03:54:10.000000 pyVIA-0.2.0/pyVIA.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-27 03:54:10.000000 pyVIA-0.2.0/pyVIA.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      211 2024-05-27 03:54:10.000000 pyVIA-0.2.0/pyVIA.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        6 2024-05-27 03:54:10.000000 pyVIA-0.2.0/pyVIA.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-27 03:54:10.729852 pyVIA-0.2.0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      957 2024-05-27 03:52:59.000000 pyVIA-0.2.0/setup.py
```

### Comparing `pyVIA-0.1.993/LICENSE.txt` & `pyVIA-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyVIA-0.1.993/PKG-INFO` & `pyVIA-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyVIA
-Version: 0.1.993
+Version: 0.2.0
 Home-page: https://github.com/ShobiStassen/VIA
 Author-email: shobana.venkat88@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `pyVIA-0.1.993/README.md` & `pyVIA-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyVIA-0.1.993/pyVIA/core.py` & `pyVIA-0.2.0/pyVIA/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -661,15 +661,15 @@
         if edgebundle_pruning is None: edgebundle_pruning = cluster_graph_pruning
         self.edgebundle_pruning = edgebundle_pruning
         if (root_user is None) & (velocity_matrix is None):
             root_user = []
             dataset = ''
         self.root_user = root_user
         if root_user is None:  dataset = ''
-        elif (type(root_user[0] == str)): dataset = 'group'
+        elif (type(root_user[0]) == str): dataset = 'group'
         else: dataset = ''
         self.dataset = dataset
         self.knn_struct = None
         if isinstance(labels, list):
             labels = np.asarray(labels).flatten()
         self.labels = labels  # np.asarray(pre_labels).flatten() where pre_labels is a list
         self.connected_comp_labels = None
```

### Comparing `pyVIA-0.1.993/pyVIA/datasets_via.py` & `pyVIA-0.2.0/pyVIA/datasets_via.py`

 * *Files identical despite different names*

### Comparing `pyVIA-0.1.993/pyVIA/examples.py` & `pyVIA-0.2.0/pyVIA/examples.py`

 * *Files identical despite different names*

### Comparing `pyVIA-0.1.993/pyVIA/plotting_via.py` & `pyVIA-0.2.0/pyVIA/plotting_via.py`

 * *Files identical despite different names*

### Comparing `pyVIA-0.1.993/pyVIA/utils_via.py` & `pyVIA-0.2.0/pyVIA/utils_via.py`

 * *Files identical despite different names*

### Comparing `pyVIA-0.1.993/pyVIA/windmap.py` & `pyVIA-0.2.0/pyVIA/windmap.py`

 * *Files identical despite different names*

### Comparing `pyVIA-0.1.993/pyVIA.egg-info/PKG-INFO` & `pyVIA-0.2.0/pyVIA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyVIA
-Version: 0.1.993
+Version: 0.2.0
 Home-page: https://github.com/ShobiStassen/VIA
 Author-email: shobana.venkat88@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `pyVIA-0.1.993/setup.py` & `pyVIA-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='pyVIA',
-    version='0.1.993', ##May 7, 2024
+    version='0.2.00', ##May 27, 2024
     packages=['pyVIA',],
     license='MIT',
     author_email = 'shobana.venkat88@gmail.com',
     url = 'https://github.com/ShobiStassen/VIA',
     setup_requires = ['numpy>=1.17','pybind11'],
     python_requires = ">=3.8",
     install_requires=['pybind11','numpy>=1.17','scipy','pandas>=0.25','hnswlib','igraph','leidenalg>=0.7.0', 'scikit-learn', 'termcolor','pygam', 'matplotlib','scanpy','umap-learn>=0.5.0','phate','datashader', 'scikit-image', 'pillow','wget','gdown','seaborn','pecanpy','holoviews'],
```

