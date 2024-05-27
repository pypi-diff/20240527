# Comparing `tmp/jasmine_astro-0.1.1.tar.gz` & `tmp/jasmine_astro-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jasmine_astro-0.1.1.tar", last modified: Sat May 25 12:04:05 2024, max compression
+gzip compressed data, was "jasmine_astro-0.1.2.tar", last modified: Mon May 27 15:05:05 2024, max compression
```

## Comparing `jasmine_astro-0.1.1.tar` & `jasmine_astro-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 stela      (501) staff       (20)        0 2024-05-25 12:04:05.316265 jasmine_astro-0.1.1/
--rw-r--r--   0 stela      (501) staff       (20)     1065 2024-05-24 16:36:41.000000 jasmine_astro-0.1.1/LICENSE
--rw-r--r--   0 stela      (501) staff       (20)      523 2024-05-25 12:04:05.316109 jasmine_astro-0.1.1/PKG-INFO
--rw-r--r--   0 stela      (501) staff       (20)     2517 2024-05-25 12:03:16.000000 jasmine_astro-0.1.1/README.md
-drwxr-xr-x   0 stela      (501) staff       (20)        0 2024-05-25 12:04:05.314090 jasmine_astro-0.1.1/jasmine/
--rw-r--r--   0 stela      (501) staff       (20)      242 2024-05-25 11:57:17.000000 jasmine_astro-0.1.1/jasmine/__init__.py
-drwxr-xr-x   0 stela      (501) staff       (20)        0 2024-05-25 12:04:05.314644 jasmine_astro-0.1.1/jasmine/classes_and_files_reader/
--rw-r--r--   0 stela      (501) staff       (20)    12083 2024-05-25 11:39:10.000000 jasmine_astro-0.1.1/jasmine/classes_and_files_reader/RTModel_results_cls.py
--rw-r--r--   0 stela      (501) staff       (20)     5538 2024-05-25 11:57:17.000000 jasmine_astro-0.1.1/jasmine/classes_and_files_reader/RTModel_results_reader.py
--rw-r--r--   0 stela      (501) staff       (20)        0 2024-05-25 11:48:28.000000 jasmine_astro-0.1.1/jasmine/classes_and_files_reader/__init__.py
--rw-r--r--   0 stela      (501) staff       (20)    15442 2024-05-25 11:57:17.000000 jasmine_astro-0.1.1/jasmine/classes_and_files_reader/datachallenge_lightcurve_cls.py
--rw-r--r--   0 stela      (501) staff       (20)     3679 2024-05-24 16:36:41.000000 jasmine_astro-0.1.1/jasmine/classes_and_files_reader/datachallenge_reader.py
-drwxr-xr-x   0 stela      (501) staff       (20)        0 2024-05-25 12:04:05.315041 jasmine_astro-0.1.1/jasmine/files_organizer/
--rw-r--r--   0 stela      (501) staff       (20)     4660 2024-05-24 16:36:41.000000 jasmine_astro-0.1.1/jasmine/files_organizer/RTModel_ephemerides_tools.py
--rw-r--r--   0 stela      (501) staff       (20)        0 2024-05-24 16:36:41.000000 jasmine_astro-0.1.1/jasmine/files_organizer/__init__.py
--rw-r--r--   0 stela      (501) staff       (20)     5001 2024-05-24 16:36:41.000000 jasmine_astro-0.1.1/jasmine/files_organizer/data_challenge_prep.py
--rw-r--r--   0 stela      (501) staff       (20)     6926 2024-05-25 11:57:17.000000 jasmine_astro-0.1.1/jasmine/files_organizer/data_challenge_to_RTModel.py
-drwxr-xr-x   0 stela      (501) staff       (20)        0 2024-05-25 12:04:05.315253 jasmine_astro-0.1.1/jasmine/investigater/
--rw-r--r--   0 stela      (501) staff       (20)        0 2024-05-24 16:36:41.000000 jasmine_astro-0.1.1/jasmine/investigater/__init__.py
--rw-r--r--   0 stela      (501) staff       (20)     1610 2024-05-25 11:57:17.000000 jasmine_astro-0.1.1/jasmine/investigater/bound_planets.py
-drwxr-xr-x   0 stela      (501) staff       (20)        0 2024-05-25 12:04:05.315936 jasmine_astro-0.1.1/jasmine_astro.egg-info/
--rw-r--r--   0 stela      (501) staff       (20)      523 2024-05-25 12:04:05.000000 jasmine_astro-0.1.1/jasmine_astro.egg-info/PKG-INFO
--rw-r--r--   0 stela      (501) staff       (20)      808 2024-05-25 12:04:05.000000 jasmine_astro-0.1.1/jasmine_astro.egg-info/SOURCES.txt
--rw-r--r--   0 stela      (501) staff       (20)        1 2024-05-25 12:04:05.000000 jasmine_astro-0.1.1/jasmine_astro.egg-info/dependency_links.txt
--rw-r--r--   0 stela      (501) staff       (20)        1 2024-05-25 12:03:34.000000 jasmine_astro-0.1.1/jasmine_astro.egg-info/not-zip-safe
--rw-r--r--   0 stela      (501) staff       (20)      124 2024-05-25 12:04:05.000000 jasmine_astro-0.1.1/jasmine_astro.egg-info/requires.txt
--rw-r--r--   0 stela      (501) staff       (20)        8 2024-05-25 12:04:05.000000 jasmine_astro-0.1.1/jasmine_astro.egg-info/top_level.txt
--rw-r--r--   0 stela      (501) staff       (20)       38 2024-05-25 12:04:05.316306 jasmine_astro-0.1.1/setup.cfg
--rw-r--r--   0 stela      (501) staff       (20)      870 2024-05-25 12:04:03.000000 jasmine_astro-0.1.1/setup.py
+drwxr-xr-x   0 stela      (501) staff       (20)        0 2024-05-27 15:05:05.022769 jasmine_astro-0.1.2/
+-rw-r--r--   0 stela      (501) staff       (20)     1065 2024-05-24 16:36:41.000000 jasmine_astro-0.1.2/LICENSE
+-rw-r--r--   0 stela      (501) staff       (20)      561 2024-05-27 15:05:05.022583 jasmine_astro-0.1.2/PKG-INFO
+-rw-r--r--   0 stela      (501) staff       (20)     3158 2024-05-27 14:28:36.000000 jasmine_astro-0.1.2/README.md
+drwxr-xr-x   0 stela      (501) staff       (20)        0 2024-05-27 15:05:05.019026 jasmine_astro-0.1.2/jasmine/
+-rw-r--r--   0 stela      (501) staff       (20)      382 2024-05-27 14:28:36.000000 jasmine_astro-0.1.2/jasmine/__init__.py
+drwxr-xr-x   0 stela      (501) staff       (20)        0 2024-05-27 15:05:05.020356 jasmine_astro-0.1.2/jasmine/classes_and_files_reader/
+-rw-r--r--   0 stela      (501) staff       (20)    12083 2024-05-25 11:39:10.000000 jasmine_astro-0.1.2/jasmine/classes_and_files_reader/RTModel_results_cls.py
+-rw-r--r--   0 stela      (501) staff       (20)     5538 2024-05-25 11:57:17.000000 jasmine_astro-0.1.2/jasmine/classes_and_files_reader/RTModel_results_reader.py
+-rw-r--r--   0 stela      (501) staff       (20)        0 2024-05-25 11:48:28.000000 jasmine_astro-0.1.2/jasmine/classes_and_files_reader/__init__.py
+-rw-r--r--   0 stela      (501) staff       (20)    15442 2024-05-25 11:57:17.000000 jasmine_astro-0.1.2/jasmine/classes_and_files_reader/datachallenge_lightcurve_cls.py
+-rw-r--r--   0 stela      (501) staff       (20)     3679 2024-05-24 16:36:41.000000 jasmine_astro-0.1.2/jasmine/classes_and_files_reader/datachallenge_reader.py
+-rw-r--r--   0 stela      (501) staff       (20)     4239 2024-05-27 14:28:36.000000 jasmine_astro-0.1.2/jasmine/classes_and_files_reader/rtmodel_template_cls.py
+drwxr-xr-x   0 stela      (501) staff       (20)        0 2024-05-27 15:05:05.021237 jasmine_astro-0.1.2/jasmine/files_organizer/
+-rw-r--r--   0 stela      (501) staff       (20)     4660 2024-05-24 16:36:41.000000 jasmine_astro-0.1.2/jasmine/files_organizer/RTModel_ephemerides_tools.py
+-rw-r--r--   0 stela      (501) staff       (20)        0 2024-05-24 16:36:41.000000 jasmine_astro-0.1.2/jasmine/files_organizer/__init__.py
+-rw-r--r--   0 stela      (501) staff       (20)     5300 2024-05-27 14:28:36.000000 jasmine_astro-0.1.2/jasmine/files_organizer/data_challenge_prep.py
+-rw-r--r--   0 stela      (501) staff       (20)     6926 2024-05-25 11:57:17.000000 jasmine_astro-0.1.2/jasmine/files_organizer/data_challenge_to_RTModel.py
+drwxr-xr-x   0 stela      (501) staff       (20)        0 2024-05-27 15:05:05.021508 jasmine_astro-0.1.2/jasmine/investigator/
+-rw-r--r--   0 stela      (501) staff       (20)        0 2024-05-27 14:28:36.000000 jasmine_astro-0.1.2/jasmine/investigator/__init__.py
+-rw-r--r--   0 stela      (501) staff       (20)     1610 2024-05-27 14:28:36.000000 jasmine_astro-0.1.2/jasmine/investigator/bound_planets.py
+drwxr-xr-x   0 stela      (501) staff       (20)        0 2024-05-27 15:05:05.022389 jasmine_astro-0.1.2/jasmine_astro.egg-info/
+-rw-r--r--   0 stela      (501) staff       (20)      561 2024-05-27 15:05:04.000000 jasmine_astro-0.1.2/jasmine_astro.egg-info/PKG-INFO
+-rw-r--r--   0 stela      (501) staff       (20)      865 2024-05-27 15:05:04.000000 jasmine_astro-0.1.2/jasmine_astro.egg-info/SOURCES.txt
+-rw-r--r--   0 stela      (501) staff       (20)        1 2024-05-27 15:05:04.000000 jasmine_astro-0.1.2/jasmine_astro.egg-info/dependency_links.txt
+-rw-r--r--   0 stela      (501) staff       (20)        1 2024-05-25 12:03:34.000000 jasmine_astro-0.1.2/jasmine_astro.egg-info/not-zip-safe
+-rw-r--r--   0 stela      (501) staff       (20)      147 2024-05-27 15:05:04.000000 jasmine_astro-0.1.2/jasmine_astro.egg-info/requires.txt
+-rw-r--r--   0 stela      (501) staff       (20)        8 2024-05-27 15:05:04.000000 jasmine_astro-0.1.2/jasmine_astro.egg-info/top_level.txt
+-rw-r--r--   0 stela      (501) staff       (20)       38 2024-05-27 15:05:05.022805 jasmine_astro-0.1.2/setup.cfg
+-rw-r--r--   0 stela      (501) staff       (20)      920 2024-05-27 15:04:53.000000 jasmine_astro-0.1.2/setup.py
```

### Comparing `jasmine_astro-0.1.1/LICENSE` & `jasmine_astro-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jasmine_astro-0.1.1/PKG-INFO` & `jasmine_astro-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: jasmine-astro
-Version: 0.1.1
+Version: 0.1.2
 Summary: JASMINE: Joint Analysis of Simulations for Microlensing INterest Events
 Home-page: https://github.com/stelais/jasmine
 Author: Stela IS
 Author-email: stela.ishitanisilva@nasa.gov
 License: MIT
 License-File: LICENSE
 Requires-Dist: pandas==2.1.4
 Requires-Dist: jupyter==1.0.0
 Requires-Dist: notebook==7.1.3
 Requires-Dist: ipykernel==6.29.4
 Requires-Dist: matplotlib==3.8.4
 Requires-Dist: astropy==6.1.0
 Requires-Dist: jplephem==2.22
 Requires-Dist: bokeh==3.4.1
+Requires-Dist: VBBinaryLensing==3.7.0
```

### Comparing `jasmine_astro-0.1.1/README.md` & `jasmine_astro-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,28 @@
 model = ModelResults(file_to_be_read='[your_path]/[Final]Models/LX0000-1.txt')
 print(model.model_type, model.model_extensive_name)
 print(model.model_parameters)
 ```
 See notebook `analysis/reading_rtmodel_models.ipynb`
 
 ---
-## 2. Microlensing Data Challenge Simulations
+## 2. Generating a Binary lens signal based on one of the 113 RTModel templates
+### `RTModelTemplateForBinaryLightCurve` class
+```
+from jasmine import RTModelTemplateForBinaryLightCurve
+rtmodel_template_two_lenses = RTModelTemplateForBinaryLightCurve(template_line=2,
+                                                                     path_to_template=template_path,
+                                                                     input_peak_t1=300,
+                                                                     input_peak_t2=302)
+magnification, times = rtmodel_template_two_lenses_.rtmodel_magnification_using_vbb()
+```
+
+
+---
+## 3. Microlensing Data Challenge Simulations
 
 ### Splitting master file
 1. Make sure you downloaded the `master_file.txt` and `wfirstColumnNumbers.txt`  from the data challenge folder:  
    https://github.com/microlensing-data-challenge/data-challenge-1/tree/master/Answers
 2. Run `python jasmine/files_organizer/data_challenge_prep.py` , changing path as needed. It splits master file and create 4 new files:
    * binary_star.csv
    * bound_planet.csv
```

### Comparing `jasmine_astro-0.1.1/jasmine/classes_and_files_reader/RTModel_results_cls.py` & `jasmine_astro-0.1.2/jasmine/classes_and_files_reader/RTModel_results_cls.py`

 * *Files identical despite different names*

### Comparing `jasmine_astro-0.1.1/jasmine/classes_and_files_reader/RTModel_results_reader.py` & `jasmine_astro-0.1.2/jasmine/classes_and_files_reader/RTModel_results_reader.py`

 * *Files identical despite different names*

### Comparing `jasmine_astro-0.1.1/jasmine/classes_and_files_reader/datachallenge_lightcurve_cls.py` & `jasmine_astro-0.1.2/jasmine/classes_and_files_reader/datachallenge_lightcurve_cls.py`

 * *Files identical despite different names*

### Comparing `jasmine_astro-0.1.1/jasmine/classes_and_files_reader/datachallenge_reader.py` & `jasmine_astro-0.1.2/jasmine/classes_and_files_reader/datachallenge_reader.py`

 * *Files identical despite different names*

### Comparing `jasmine_astro-0.1.1/jasmine/files_organizer/RTModel_ephemerides_tools.py` & `jasmine_astro-0.1.2/jasmine/files_organizer/RTModel_ephemerides_tools.py`

 * *Files identical despite different names*

### Comparing `jasmine_astro-0.1.1/jasmine/files_organizer/data_challenge_prep.py` & `jasmine_astro-0.1.2/jasmine/files_organizer/data_challenge_prep.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,19 +8,20 @@
     :param path_to_wfirstcolumn_file_:
     :return:
     """
     wfirstcolumn_df = pd.read_csv(path_to_wfirstcolumn_file_, sep="\s+")
     return wfirstcolumn_df
 
 
-def master_file_spliter(path_to_master_file_, path_to_wfirstcolumn_file_):
+def master_file_spliter(path_to_master_file_, path_to_wfirstcolumn_file_, path_to_output_folder_):
     """
     This function reads the master file and splits it into 4 different files based on the type of event.
     :param path_to_master_file_:
     :param path_to_wfirstcolumn_file_:
+    :param path_to_output_folder_:
     :return:
     """
     single_lens_lines = []  # dcnormffp
     binary_star_lines = []  # ombin
     bound_planet_lines = []  # omcassan
     cataclysmic_variables_lines = []  # dccv
     header_line = str(master_head_getter(path_to_wfirstcolumn_file_)['name'].values)
@@ -45,56 +46,58 @@
                     bound_planet_lines.append(line)
                 elif "dccv" in line:
                     cataclysmic_variables_lines.append(line)
 
                 else:
                     raise ValueError("Unknown type of event\n", line)
 
-    with open('data/single_lens.csv', 'w') as single_lens_file:
+    with open(f'{path_to_output_folder_}/single_lens.csv', 'w') as single_lens_file:
         single_lens_header_line = header_line+(',unimportant0,unimportant1,unimportant2,'
                                                'event_type,unimportant3,lc_root,data_challenge_lc_number\n')
         single_lens_file.write(single_lens_header_line)
         for line in single_lens_lines:
             single_lens_file.write(line)
 
-    with open('data/binary_star.csv', 'w') as binary_star_file:
+    with open(f'{path_to_output_folder_}/binary_star.csv', 'w') as binary_star_file:
         binary_lens_header_line = header_line.replace(',normw,sigma_t0,sigma_tE,sigma_u0,sigma_alpha,sigma_s,'
                                                       'sigma_q,sigma_rs,sigma_F00,sigma_fs0,sigma_F01,sigma_fs1,'
                                                       'sigma_thetaE',
                                                       ',normw,event_type,unimportant0,lc_root,'
                                                       'data_challenge_lc_number\n')
         binary_star_file.write(binary_lens_header_line)
         for line in binary_star_lines:
             line = line.replace(',,,', ',')
             binary_star_file.write(line)
 
-    with open('data/bound_planet.csv', 'w') as bound_planet_file:
+    with open(f'{path_to_output_folder_}/bound_planet.csv', 'w') as bound_planet_file:
         bound_planet_header_line = header_line.replace(',normw,sigma_t0,sigma_tE,sigma_u0,sigma_alpha,sigma_s,'
                                                        'sigma_q,sigma_rs,sigma_F00,sigma_fs0,sigma_F01,sigma_fs1,'
                                                        'sigma_thetaE',
                                                        ',normw,event_type,unimportant0,lc_root,'
                                                        'data_challenge_lc_number\n')
         bound_planet_file.write(bound_planet_header_line)
         for line in bound_planet_lines:
             line = line.replace(',,,', ',')
             bound_planet_file.write(line)
 
-    with open('data/cataclysmic_variables.csv', 'w') as cataclysmic_variables_file:
+    with open(f'{path_to_output_folder_}/cataclysmic_variables.csv', 'w') as cataclysmic_variables_file:
         cataclysmic_variables_header_line = header_line.replace(',normw,sigma_t0,sigma_tE,sigma_u0,sigma_alpha,sigma_s,'
                                                                 'sigma_q,sigma_rs,sigma_F00,sigma_fs0,sigma_F01,'
                                                                 'sigma_fs1,'
                                                                 'sigma_thetaE',
                                                                 ',event_type,unimportant0,lc_root,'
                                                                 'data_challenge_lc_number\n')
         cataclysmic_variables_file.write(cataclysmic_variables_header_line)
         for line in cataclysmic_variables_lines:
             cataclysmic_variables_file.write(line)
 
 
 if __name__ == '__main__':
     # Write where you can find the master files
-    path_to_master_file = 'data/master_file.txt'
-    path_to_wfirstcolumn_file = 'data/wfirstColumnNumbers.txt'
-    master_file_spliter(path_to_master_file, path_to_wfirstcolumn_file)
+    root_path = '/Users/stela/Documents/Scripts/RTModel_project/datachallenge'
+    path_to_master_file = f'{root_path}/master_file.txt'
+    path_to_wfirstcolumn_file = f'{root_path}/wfirstColumnNumbers.txt'
+    path_to_output_folder = root_path
+    master_file_spliter(path_to_master_file, path_to_wfirstcolumn_file, path_to_output_folder)
     print("Files have been created successfully")
```

### Comparing `jasmine_astro-0.1.1/jasmine/files_organizer/data_challenge_to_RTModel.py` & `jasmine_astro-0.1.2/jasmine/files_organizer/data_challenge_to_RTModel.py`

 * *Files identical despite different names*

### Comparing `jasmine_astro-0.1.1/jasmine/investigater/bound_planets.py` & `jasmine_astro-0.1.2/jasmine/investigator/bound_planets.py`

 * *Files identical despite different names*

### Comparing `jasmine_astro-0.1.1/jasmine_astro.egg-info/PKG-INFO` & `jasmine_astro-0.1.2/jasmine_astro.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: jasmine-astro
-Version: 0.1.1
+Version: 0.1.2
 Summary: JASMINE: Joint Analysis of Simulations for Microlensing INterest Events
 Home-page: https://github.com/stelais/jasmine
 Author: Stela IS
 Author-email: stela.ishitanisilva@nasa.gov
 License: MIT
 License-File: LICENSE
 Requires-Dist: pandas==2.1.4
 Requires-Dist: jupyter==1.0.0
 Requires-Dist: notebook==7.1.3
 Requires-Dist: ipykernel==6.29.4
 Requires-Dist: matplotlib==3.8.4
 Requires-Dist: astropy==6.1.0
 Requires-Dist: jplephem==2.22
 Requires-Dist: bokeh==3.4.1
+Requires-Dist: VBBinaryLensing==3.7.0
```

### Comparing `jasmine_astro-0.1.1/jasmine_astro.egg-info/SOURCES.txt` & `jasmine_astro-0.1.2/jasmine_astro.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 setup.py
 jasmine/__init__.py
 jasmine/classes_and_files_reader/RTModel_results_cls.py
 jasmine/classes_and_files_reader/RTModel_results_reader.py
 jasmine/classes_and_files_reader/__init__.py
 jasmine/classes_and_files_reader/datachallenge_lightcurve_cls.py
 jasmine/classes_and_files_reader/datachallenge_reader.py
+jasmine/classes_and_files_reader/rtmodel_template_cls.py
 jasmine/files_organizer/RTModel_ephemerides_tools.py
 jasmine/files_organizer/__init__.py
 jasmine/files_organizer/data_challenge_prep.py
 jasmine/files_organizer/data_challenge_to_RTModel.py
-jasmine/investigater/__init__.py
-jasmine/investigater/bound_planets.py
+jasmine/investigator/__init__.py
+jasmine/investigator/bound_planets.py
 jasmine_astro.egg-info/PKG-INFO
 jasmine_astro.egg-info/SOURCES.txt
 jasmine_astro.egg-info/dependency_links.txt
 jasmine_astro.egg-info/not-zip-safe
 jasmine_astro.egg-info/requires.txt
 jasmine_astro.egg-info/top_level.txt
```

### Comparing `jasmine_astro-0.1.1/setup.py` & `jasmine_astro-0.1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup
 
 setup(name='jasmine-astro',
-      version='0.1.1',
+      version='0.1.2',
       description='JASMINE: Joint Analysis of Simulations for Microlensing INterest Events',
       url='https://github.com/stelais/jasmine',
       author='Stela IS',
       author_email='stela.ishitanisilva@nasa.gov',
       license='MIT',
       packages=['jasmine',
                 'jasmine.classes_and_files_reader',
                 'jasmine.files_organizer',
-                'jasmine.investigater'],
+                'jasmine.investigator'],
       zip_safe=False,
       install_requires=["pandas==2.1.4",
                         "jupyter==1.0.0",
                         "notebook==7.1.3",
                         "ipykernel==6.29.4",
                         "matplotlib==3.8.4",
                         "astropy==6.1.0",
                         "jplephem==2.22",
-                        "bokeh==3.4.1"
+                        "bokeh==3.4.1",
+                        "VBBinaryLensing==3.7.0"
                         ])
```

