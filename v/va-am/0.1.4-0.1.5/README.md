# Comparing `tmp/va_am-0.1.4.tar.gz` & `tmp/va_am-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "va_am-0.1.4.tar", last modified: Mon May 27 07:14:42 2024, max compression
+gzip compressed data, was "va_am-0.1.5.tar", last modified: Mon May 27 16:09:24 2024, max compression
```

## Comparing `va_am-0.1.4.tar` & `va_am-0.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-27 07:14:42.921057 va_am-0.1.4/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    35149 2023-09-29 09:45:51.000000 va_am-0.1.4/LICENSE
--rw-r--r--   0 cosmin    (1000) cosmin    (1000)    46344 2024-05-27 07:14:42.921057 va_am-0.1.4/PKG-INFO
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     5078 2024-02-12 18:26:04.000000 va_am-0.1.4/README.md
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      756 2024-05-27 07:14:10.000000 va_am-0.1.4/pyproject.toml
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       38 2024-05-27 07:14:42.921057 va_am-0.1.4/setup.cfg
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       68 2023-09-28 11:32:10.000000 va_am-0.1.4/setup.py
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-27 07:14:42.917056 va_am-0.1.4/src/
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-27 07:14:42.921057 va_am-0.1.4/src/va_am/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      222 2024-02-20 12:03:10.000000 va_am-0.1.4/src/va_am/__init__.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       66 2023-09-28 11:12:58.000000 va_am-0.1.4/src/va_am/__main__.py
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-27 07:14:42.921057 va_am-0.1.4/src/va_am/utils/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    60986 2024-05-20 13:28:39.000000 va_am-0.1.4/src/va_am/utils/AutoEncoders.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2023-06-29 15:33:10.000000 va_am-0.1.4/src/va_am/utils/__init__.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     3123 2023-09-25 14:36:24.000000 va_am-0.1.4/src/va_am/utils/functions.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)   103166 2024-05-20 13:28:39.000000 va_am-0.1.4/src/va_am/va_am.py
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-27 07:14:42.921057 va_am-0.1.4/src/va_am.egg-info/
--rw-r--r--   0 cosmin    (1000) cosmin    (1000)    46344 2024-05-27 07:14:42.000000 va_am-0.1.4/src/va_am.egg-info/PKG-INFO
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      517 2024-05-27 07:14:42.000000 va_am-0.1.4/src/va_am.egg-info/SOURCES.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        1 2024-05-27 07:14:42.000000 va_am-0.1.4/src/va_am.egg-info/dependency_links.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       46 2024-05-27 07:14:42.000000 va_am-0.1.4/src/va_am.egg-info/entry_points.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       71 2024-05-27 07:14:42.000000 va_am-0.1.4/src/va_am.egg-info/requires.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        6 2024-05-27 07:14:42.000000 va_am-0.1.4/src/va_am.egg-info/top_level.txt
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-27 07:14:42.921057 va_am-0.1.4/test/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2024-05-20 13:28:39.000000 va_am-0.1.4/test/test_AutoEncoders.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1232 2024-05-20 13:28:39.000000 va_am-0.1.4/test/test_aux_va_am.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2024-05-20 13:28:39.000000 va_am-0.1.4/test/test_io_va_am.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2024-05-20 13:28:39.000000 va_am-0.1.4/test/test_main_va_am.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2024-05-20 13:28:39.000000 va_am-0.1.4/test/test_utils_functions.py
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-27 16:09:24.534761 va_am-0.1.5/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    35149 2023-09-29 09:45:51.000000 va_am-0.1.5/LICENSE
+-rw-r--r--   0 cosmin    (1000) cosmin    (1000)    46344 2024-05-27 16:09:24.534761 va_am-0.1.5/PKG-INFO
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     5078 2024-02-12 18:26:04.000000 va_am-0.1.5/README.md
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      756 2024-05-27 11:43:55.000000 va_am-0.1.5/pyproject.toml
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       38 2024-05-27 16:09:24.534761 va_am-0.1.5/setup.cfg
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       68 2023-09-28 11:32:10.000000 va_am-0.1.5/setup.py
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-27 16:09:24.530761 va_am-0.1.5/src/
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-27 16:09:24.530761 va_am-0.1.5/src/va_am/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      222 2024-02-20 12:03:10.000000 va_am-0.1.5/src/va_am/__init__.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       66 2023-09-28 11:12:58.000000 va_am-0.1.5/src/va_am/__main__.py
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-27 16:09:24.530761 va_am-0.1.5/src/va_am/utils/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    60986 2024-05-20 13:28:39.000000 va_am-0.1.5/src/va_am/utils/AutoEncoders.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2023-06-29 15:33:10.000000 va_am-0.1.5/src/va_am/utils/__init__.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     3123 2023-09-25 14:36:24.000000 va_am-0.1.5/src/va_am/utils/functions.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)   103130 2024-05-27 11:43:55.000000 va_am-0.1.5/src/va_am/va_am.py
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-27 16:09:24.534761 va_am-0.1.5/src/va_am.egg-info/
+-rw-r--r--   0 cosmin    (1000) cosmin    (1000)    46344 2024-05-27 16:09:24.000000 va_am-0.1.5/src/va_am.egg-info/PKG-INFO
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      517 2024-05-27 16:09:24.000000 va_am-0.1.5/src/va_am.egg-info/SOURCES.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        1 2024-05-27 16:09:24.000000 va_am-0.1.5/src/va_am.egg-info/dependency_links.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       46 2024-05-27 16:09:24.000000 va_am-0.1.5/src/va_am.egg-info/entry_points.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       71 2024-05-27 16:09:24.000000 va_am-0.1.5/src/va_am.egg-info/requires.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        6 2024-05-27 16:09:24.000000 va_am-0.1.5/src/va_am.egg-info/top_level.txt
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-27 16:09:24.534761 va_am-0.1.5/test/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2024-05-20 13:28:39.000000 va_am-0.1.5/test/test_AutoEncoders.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1232 2024-05-20 13:28:39.000000 va_am-0.1.5/test/test_aux_va_am.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2024-05-20 13:28:39.000000 va_am-0.1.5/test/test_io_va_am.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2024-05-20 13:28:39.000000 va_am-0.1.5/test/test_main_va_am.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2024-05-20 13:28:39.000000 va_am-0.1.5/test/test_utils_functions.py
```

### Comparing `va_am-0.1.4/LICENSE` & `va_am-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `va_am-0.1.4/PKG-INFO` & `va_am-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: va_am
-Version: 0.1.4
+Version: 0.1.5
 Summary: VA-AM method implementation
 Author-email: cosminmarina <cosmin.marina@uah.es>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `va_am-0.1.4/README.md` & `va_am-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `va_am-0.1.4/pyproject.toml` & `va_am-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "va_am"
-version = "0.1.4"
+version = "0.1.5"
 authors = [{name="cosminmarina", email="cosmin.marina@uah.es" }]
 description = "VA-AM method implementation"
 readme = "README.md"
 dependencies = ["requests","sympy","keras","tensorflow","xarray","netcdf4","matplotlib","pandas","numpy"]
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 classifiers = [
```

### Comparing `va_am-0.1.4/src/va_am/utils/AutoEncoders.py` & `va_am-0.1.5/src/va_am/utils/AutoEncoders.py`

 * *Files identical despite different names*

### Comparing `va_am-0.1.4/src/va_am/utils/functions.py` & `va_am-0.1.5/src/va_am/utils/functions.py`

 * *Files identical despite different names*

### Comparing `va_am-0.1.4/src/va_am/va_am.py` & `va_am-0.1.5/src/va_am/va_am.py`

 * *Files 0% similar despite different names*

```diff
@@ -970,18 +970,16 @@
     percentile_threshold_array = percentile_threshold.pctl_th.data
     
     plt.figure()
     plt.plot(time_x, (data_temp_array - 273.15), marker='o', label='Days studied')
     plt.xticks(rotation=45)
     plt.plot(time_x, (percentile_threshold_array - 273.15), color='r', label=f'p{which_percentile} threshold')
     if params["verbose"]:
-        #plt.show()
         print(f'Threshold: {percentile_threshold_array - 273.15}')
         print(f'Amount of days that surpass the threshold: {amount_surpass_threshold}' )
-    plt.close()
 
     if amount_surpass_threshold == len(data_temp_array):
         heatwave_period = time_x#.astype('datetime64[D]')
     elif amount_surpass_threshold == 0:
         heatwave_period = []
     else:
         grouped_surpass = np.array([(val , sum(1 for i in val_to_count)) for val, val_to_count in groupby(surpass_threshold)])
```

### Comparing `va_am-0.1.4/src/va_am.egg-info/PKG-INFO` & `va_am-0.1.5/src/va_am.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: va_am
-Version: 0.1.4
+Version: 0.1.5
 Summary: VA-AM method implementation
 Author-email: cosminmarina <cosmin.marina@uah.es>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `va_am-0.1.4/src/va_am.egg-info/SOURCES.txt` & `va_am-0.1.5/src/va_am.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `va_am-0.1.4/test/test_aux_va_am.py` & `va_am-0.1.5/test/test_aux_va_am.py`

 * *Files identical despite different names*

