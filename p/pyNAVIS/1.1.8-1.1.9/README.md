# Comparing `tmp/pyNAVIS-1.1.8.tar.gz` & `tmp/pyNAVIS-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyNAVIS-1.1.8.tar", last modified: Wed Nov 15 15:36:59 2023, max compression
+gzip compressed data, was "pyNAVIS-1.1.9.tar", last modified: Wed Nov 15 15:56:42 2023, max compression
```

## Comparing `pyNAVIS-1.1.8.tar` & `pyNAVIS-1.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-11-15 15:36:59.421838 pyNAVIS-1.1.8/
--rw-rw-rw-   0        0        0     6337 2023-11-15 15:36:59.420839 pyNAVIS-1.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-11-15 15:36:59.398320 pyNAVIS-1.1.8/pyNAVIS/
--rw-rw-rw-   0        0        0      399 2023-11-15 15:31:26.000000 pyNAVIS-1.1.8/pyNAVIS/__init__.py
--rw-rw-rw-   0        0        0     8495 2023-11-15 15:01:01.000000 pyNAVIS-1.1.8/pyNAVIS/dataset_gen.py
--rw-rw-rw-   0        0        0    18813 2023-11-15 15:20:05.000000 pyNAVIS-1.1.8/pyNAVIS/functions.py
--rw-rw-rw-   0        0        0     8149 2022-03-29 07:23:34.000000 pyNAVIS-1.1.8/pyNAVIS/generators.py
--rw-rw-rw-   0        0        0    22338 2023-11-15 15:20:11.000000 pyNAVIS-1.1.8/pyNAVIS/loaders.py
--rw-rw-rw-   0        0        0     5287 2022-03-29 07:23:34.000000 pyNAVIS-1.1.8/pyNAVIS/main_settings.py
--rw-rw-rw-   0        0        0     2268 2022-03-29 07:23:34.000000 pyNAVIS-1.1.8/pyNAVIS/objects.py
--rw-rw-rw-   0        0        0    35391 2023-11-15 15:22:00.000000 pyNAVIS-1.1.8/pyNAVIS/plots.py
--rw-rw-rw-   0        0        0     7950 2022-03-29 07:23:34.000000 pyNAVIS-1.1.8/pyNAVIS/report_functions.py
--rw-rw-rw-   0        0        0    10205 2021-06-16 10:15:53.000000 pyNAVIS-1.1.8/pyNAVIS/savers.py
--rw-rw-rw-   0        0        0     9241 2022-03-29 07:23:34.000000 pyNAVIS-1.1.8/pyNAVIS/splitters.py
--rw-rw-rw-   0        0        0     3974 2022-03-29 07:23:34.000000 pyNAVIS-1.1.8/pyNAVIS/utils.py
-drwxrwxrwx   0        0        0        0 2023-11-15 15:36:59.420839 pyNAVIS-1.1.8/pyNAVIS.egg-info/
--rw-rw-rw-   0        0        0     6337 2023-11-15 15:36:58.000000 pyNAVIS-1.1.8/pyNAVIS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      412 2023-11-15 15:36:58.000000 pyNAVIS-1.1.8/pyNAVIS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-15 15:36:58.000000 pyNAVIS-1.1.8/pyNAVIS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-11-15 15:36:58.000000 pyNAVIS-1.1.8/pyNAVIS.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-11-15 15:36:58.000000 pyNAVIS-1.1.8/pyNAVIS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-15 15:36:59.421838 pyNAVIS-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0      979 2023-11-15 15:33:32.000000 pyNAVIS-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-11-15 15:56:42.416544 pyNAVIS-1.1.9/
+-rw-rw-rw-   0        0        0     6337 2023-11-15 15:56:42.416544 pyNAVIS-1.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-11-15 15:56:42.400587 pyNAVIS-1.1.9/pyNAVIS/
+-rw-rw-rw-   0        0        0      399 2023-11-15 15:31:26.000000 pyNAVIS-1.1.9/pyNAVIS/__init__.py
+-rw-rw-rw-   0        0        0     8495 2023-11-15 15:01:01.000000 pyNAVIS-1.1.9/pyNAVIS/dataset_gen.py
+-rw-rw-rw-   0        0        0    18813 2023-11-15 15:20:05.000000 pyNAVIS-1.1.9/pyNAVIS/functions.py
+-rw-rw-rw-   0        0        0     8149 2022-03-29 07:23:34.000000 pyNAVIS-1.1.9/pyNAVIS/generators.py
+-rw-rw-rw-   0        0        0    22338 2023-11-15 15:20:11.000000 pyNAVIS-1.1.9/pyNAVIS/loaders.py
+-rw-rw-rw-   0        0        0     5287 2022-03-29 07:23:34.000000 pyNAVIS-1.1.9/pyNAVIS/main_settings.py
+-rw-rw-rw-   0        0        0     2268 2022-03-29 07:23:34.000000 pyNAVIS-1.1.9/pyNAVIS/objects.py
+-rw-rw-rw-   0        0        0    35391 2023-11-15 15:22:00.000000 pyNAVIS-1.1.9/pyNAVIS/plots.py
+-rw-rw-rw-   0        0        0     7950 2022-03-29 07:23:34.000000 pyNAVIS-1.1.9/pyNAVIS/report_functions.py
+-rw-rw-rw-   0        0        0    10205 2021-06-16 10:15:53.000000 pyNAVIS-1.1.9/pyNAVIS/savers.py
+-rw-rw-rw-   0        0        0     9241 2022-03-29 07:23:34.000000 pyNAVIS-1.1.9/pyNAVIS/splitters.py
+-rw-rw-rw-   0        0        0     3974 2022-03-29 07:23:34.000000 pyNAVIS-1.1.9/pyNAVIS/utils.py
+drwxrwxrwx   0        0        0        0 2023-11-15 15:56:42.415545 pyNAVIS-1.1.9/pyNAVIS.egg-info/
+-rw-rw-rw-   0        0        0     6337 2023-11-15 15:56:42.000000 pyNAVIS-1.1.9/pyNAVIS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2023-11-15 15:56:42.000000 pyNAVIS-1.1.9/pyNAVIS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-15 15:56:42.000000 pyNAVIS-1.1.9/pyNAVIS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-11-15 15:56:42.000000 pyNAVIS-1.1.9/pyNAVIS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-11-15 15:56:42.000000 pyNAVIS-1.1.9/pyNAVIS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-11-15 15:56:42.417556 pyNAVIS-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      979 2023-11-15 15:44:44.000000 pyNAVIS-1.1.9/setup.py
```

### Comparing `pyNAVIS-1.1.8/PKG-INFO` & `pyNAVIS-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNAVIS
-Version: 1.1.8
+Version: 1.1.9
 Summary: Useful tools to analyze and process spiking information from neuromorphic auditory sensors.
 Home-page: https://github.com/jpdominguez/pyNAVIS
 Author: Juan P. Dominguez-Morales
 Author-email: jpdominguez@us.es
 License: GPL
 Download-URL: https://pypi.org/project/pyNAVIS/
 Description: ## pyNAVIS: an open-source cross-platform Neuromorphic Auditory VISualizer
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyNAVIS Version: 1.1.8 Summary: Useful tools to
+Metadata-Version: 2.1 Name: pyNAVIS Version: 1.1.9 Summary: Useful tools to
 analyze and process spiking information from neuromorphic auditory sensors.
 Home-page: https://github.com/jpdominguez/pyNAVIS Author: Juan P. Dominguez-
 Morales Author-email: jpdominguez@us.es License: GPL Download-URL: https://
 pypi.org/project/pyNAVIS/ Description: ## pyNAVIS: an open-source cross-
 platform Neuromorphic Auditory VISualizer
 [https://github.com/jpdominguez/pyNAVIS/blob/master/images/wiki-images/
 pynavis_logo.png?raw=true]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_G_P_L_%_2_0_v_3_-
```

### Comparing `pyNAVIS-1.1.8/pyNAVIS/dataset_gen.py` & `pyNAVIS-1.1.9/pyNAVIS/dataset_gen.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.8/pyNAVIS/functions.py` & `pyNAVIS-1.1.9/pyNAVIS/functions.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.8/pyNAVIS/generators.py` & `pyNAVIS-1.1.9/pyNAVIS/generators.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.8/pyNAVIS/loaders.py` & `pyNAVIS-1.1.9/pyNAVIS/loaders.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.8/pyNAVIS/main_settings.py` & `pyNAVIS-1.1.9/pyNAVIS/main_settings.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.8/pyNAVIS/objects.py` & `pyNAVIS-1.1.9/pyNAVIS/objects.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.8/pyNAVIS/plots.py` & `pyNAVIS-1.1.9/pyNAVIS/plots.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.8/pyNAVIS/report_functions.py` & `pyNAVIS-1.1.9/pyNAVIS/report_functions.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.8/pyNAVIS/savers.py` & `pyNAVIS-1.1.9/pyNAVIS/savers.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.8/pyNAVIS/splitters.py` & `pyNAVIS-1.1.9/pyNAVIS/splitters.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.8/pyNAVIS/utils.py` & `pyNAVIS-1.1.9/pyNAVIS/utils.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.8/pyNAVIS.egg-info/PKG-INFO` & `pyNAVIS-1.1.9/pyNAVIS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNAVIS
-Version: 1.1.8
+Version: 1.1.9
 Summary: Useful tools to analyze and process spiking information from neuromorphic auditory sensors.
 Home-page: https://github.com/jpdominguez/pyNAVIS
 Author: Juan P. Dominguez-Morales
 Author-email: jpdominguez@us.es
 License: GPL
 Download-URL: https://pypi.org/project/pyNAVIS/
 Description: ## pyNAVIS: an open-source cross-platform Neuromorphic Auditory VISualizer
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyNAVIS Version: 1.1.8 Summary: Useful tools to
+Metadata-Version: 2.1 Name: pyNAVIS Version: 1.1.9 Summary: Useful tools to
 analyze and process spiking information from neuromorphic auditory sensors.
 Home-page: https://github.com/jpdominguez/pyNAVIS Author: Juan P. Dominguez-
 Morales Author-email: jpdominguez@us.es License: GPL Download-URL: https://
 pypi.org/project/pyNAVIS/ Description: ## pyNAVIS: an open-source cross-
 platform Neuromorphic Auditory VISualizer
 [https://github.com/jpdominguez/pyNAVIS/blob/master/images/wiki-images/
 pynavis_logo.png?raw=true]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_G_P_L_%_2_0_v_3_-
```

### Comparing `pyNAVIS-1.1.8/setup.py` & `pyNAVIS-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     README = readme_file.read()
 """
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 """
 setup_args = dict(
     name='pyNAVIS',
-    version='1.1.8',
+    version='1.1.9',
     description='Useful tools to analyze and process spiking information from neuromorphic auditory sensors.',
     long_description_content_type="text/markdown",
     long_description=README,
     license='GPL',
     packages=find_packages(),
     author='Juan P. Dominguez-Morales',
     author_email='jpdominguez@us.es',
```

