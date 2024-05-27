# Comparing `tmp/pyelq_sdk-1.0.4.tar.gz` & `tmp/pyelq_sdk-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyelq_sdk-1.0.4.tar", max compression
+gzip compressed data, was "pyelq_sdk-1.0.5.tar", max compression
```

## Comparing `pyelq_sdk-1.0.4.tar` & `pyelq_sdk-1.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    11358 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/LICENSE.md
-drwxr-xr-x   0        0        0        0 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/LICENSES/
--rw-r--r--   0        0        0    10280 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/LICENSES/Apache-2.0.txt
--rw-r--r--   0        0        0     6099 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/README.md
--rw-r--r--   0        0        0     1838 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      414 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/src/pyelq/__init__.py
--rw-r--r--   0        0        0      245 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/src/pyelq/component/__init__.py
--rw-r--r--   0        0        0    18705 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/src/pyelq/component/background.py
--rw-r--r--   0        0        0     2360 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/src/pyelq/component/component.py
--rw-r--r--   0        0        0    16261 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/src/pyelq/component/error_model.py
--rw-r--r--   0        0        0     7718 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/src/pyelq/component/offset.py
--rw-r--r--   0        0        0    37479 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/src/pyelq/component/source_model.py
--rw-r--r--   0        0        0    22281 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/src/pyelq/coordinate_system.py
--rw-r--r--   0        0        0      186 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/src/pyelq/data_access/__init__.py
--rw-r--r--   0        0        0     3973 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/src/pyelq/data_access/data_access.py
--rw-r--r--   0        0        0      194 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/src/pyelq/dispersion_model/__init__.py
--rw-r--r--   0        0        0    31586 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/src/pyelq/dispersion_model/gaussian_plume.py
--rw-r--r--   0        0        0    25293 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/src/pyelq/dlm.py
--rw-r--r--   0        0        0     6504 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/src/pyelq/gas_species.py
--rw-r--r--   0        0        0    13207 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/src/pyelq/meteorology.py
--rw-r--r--   0        0        0     9173 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/src/pyelq/model.py
--rw-r--r--   0        0        0      176 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/src/pyelq/plotting/__init__.py
--rw-r--r--   0        0        0    58335 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/src/pyelq/plotting/plot.py
--rw-r--r--   0        0        0    12658 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/src/pyelq/preprocessing.py
--rw-r--r--   0        0        0      197 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/src/pyelq/sensor/__init__.py
--rw-r--r--   0        0        0     1806 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/src/pyelq/sensor/beam.py
--rw-r--r--   0        0        0     2316 2024-03-13 12:40:41.328050 pyelq_sdk-1.0.4/src/pyelq/sensor/satellite.py
--rw-r--r--   0        0        0     9190 2024-03-13 12:40:41.332050 pyelq_sdk-1.0.4/src/pyelq/sensor/sensor.py
--rw-r--r--   0        0        0     5741 2024-03-13 12:40:41.332050 pyelq_sdk-1.0.4/src/pyelq/source_map.py
--rw-r--r--   0        0        0      210 2024-03-13 12:40:41.332050 pyelq_sdk-1.0.4/src/pyelq/support_functions/__init__.py
--rw-r--r--   0        0        0    10609 2024-03-13 12:40:41.332050 pyelq_sdk-1.0.4/src/pyelq/support_functions/spatio_temporal_interpolation.py
--rw-r--r--   0        0        0     7064 1970-01-01 00:00:00.000000 pyelq_sdk-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/LICENSE.md
+drwxr-xr-x   0        0        0        0 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/LICENSES/
+-rw-r--r--   0        0        0    10280 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0     7491 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/README.md
+-rw-r--r--   0        0        0     1838 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      414 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/src/pyelq/__init__.py
+-rw-r--r--   0        0        0      245 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/src/pyelq/component/__init__.py
+-rw-r--r--   0        0        0    18705 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/src/pyelq/component/background.py
+-rw-r--r--   0        0        0     2360 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/src/pyelq/component/component.py
+-rw-r--r--   0        0        0    16261 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/src/pyelq/component/error_model.py
+-rw-r--r--   0        0        0     7718 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/src/pyelq/component/offset.py
+-rw-r--r--   0        0        0    37479 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/src/pyelq/component/source_model.py
+-rw-r--r--   0        0        0    22281 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/src/pyelq/coordinate_system.py
+-rw-r--r--   0        0        0      186 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/src/pyelq/data_access/__init__.py
+-rw-r--r--   0        0        0     3973 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/src/pyelq/data_access/data_access.py
+-rw-r--r--   0        0        0      194 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/src/pyelq/dispersion_model/__init__.py
+-rw-r--r--   0        0        0    31586 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/dispersion_model/gaussian_plume.py
+-rw-r--r--   0        0        0    25293 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/dlm.py
+-rw-r--r--   0        0        0     6504 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/gas_species.py
+-rw-r--r--   0        0        0    13207 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/meteorology.py
+-rw-r--r--   0        0        0     9173 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/model.py
+-rw-r--r--   0        0        0      176 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/plotting/__init__.py
+-rw-r--r--   0        0        0    58335 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/plotting/plot.py
+-rw-r--r--   0        0        0    12658 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/preprocessing.py
+-rw-r--r--   0        0        0      197 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/sensor/__init__.py
+-rw-r--r--   0        0        0     1806 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/sensor/beam.py
+-rw-r--r--   0        0        0     2316 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/sensor/satellite.py
+-rw-r--r--   0        0        0     9190 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/sensor/sensor.py
+-rw-r--r--   0        0        0     5741 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/source_map.py
+-rw-r--r--   0        0        0      210 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/support_functions/__init__.py
+-rw-r--r--   0        0        0    10609 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/support_functions/spatio_temporal_interpolation.py
+-rw-r--r--   0        0        0     8437 1970-01-01 00:00:00.000000 pyelq_sdk-1.0.5/PKG-INFO
```

### Comparing `pyelq_sdk-1.0.4/LICENSE.md` & `pyelq_sdk-1.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.4/LICENSES/Apache-2.0.txt` & `pyelq_sdk-1.0.5/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.4/README.md` & `pyelq_sdk-1.0.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 <div align="center">
 
 [![PyPI version](https://img.shields.io/pypi/v/pyelq-sdk.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/pyelq-sdk/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/pyelq-sdk.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/pyelq-sdk/)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Code Style Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Tests](https://github.com/sede-open/pyelq/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/sede-open/pyelq/actions/workflows/main.yml)
 
 [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=pyelq_pyelq&metric=coverage)](https://sonarcloud.io/summary/new_code?id=pyelq_pyelq)
 [![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=pyelq_pyelq&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=pyelq_pyelq)
 [![Bugs](https://sonarcloud.io/api/project_badges/measure?project=pyelq_pyelq&metric=bugs)](https://sonarcloud.io/summary/new_code?id=pyelq_pyelq)
 [![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=pyelq_pyelq&metric=ncloc)](https://sonarcloud.io/summary/new_code?id=pyelq_pyelq)
 [![Duplicated Lines (%)](https://sonarcloud.io/api/project_badges/measure?project=pyelq_pyelq&metric=duplicated_lines_density)](https://sonarcloud.io/summary/new_code?id=pyelq_pyelq)
 [![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=pyelq_pyelq&metric=code_smells)](https://sonarcloud.io/summary/new_code?id=pyelq_pyelq)
@@ -47,14 +46,34 @@
 to support various assets in their quest to reduce methane emissions.
 
 Use cases where the pyELQ code has been applied are described in the following papers:
 
 * IJzermans, R., Jones, M., Weidmann, D. et al. "Long-term continuous monitoring of methane emissions at an oil and gas facility using a multi-open-path laser dispersion spectrometer." Sci Rep 14, 623 (2024). (https://doi.org/10.1038/s41598-023-50081-9)
 
 * Weidmann, D., Hirst, B. et al. "Locating and Quantifying Methane Emissions by Inverse Analysis of Path-Integrated Concentration Data Using a Markov-Chain Monte Carlo Approach." ACS Earth and Space Chemistry 2022 6 (9), 2190-2198  (https://doi.org/10.1021/acsearthspacechem.2c00093)
+
+## Deployment design
+The pyELQ code needs high-quality methane concentration and wind data to be able to provide reliable output on location 
+and quantification of methane emission sources. This requires methane concentration sensors of sufficiently high 
+precision in a layout that allows the detection of relevant methane emission sources, in combination with wind 
+measurements of high enough frequency and accuracy. The optimal sensor layout typically depends on the prevailing 
+meteorological conditions at the site of interest and requires multiple concentration sensors to cover the site under 
+different wind directions. 
+
+## pyELQ data interpretation
+The results from pyELQ come with uncertainty ranges that are representative of probability density functions sampled 
+by a Markov Chain Monte Carlo method. One should take these uncertainty ranges into account when interpreting the pyELQ 
+output data. Remember that absence of evidence for methane emissions does not always imply evidence for absence of 
+methane emissions; for instance, when meteorological conditions are such that there is no sensor downwind of a methane 
+source during the selected monitoring period, then it will be impossible to detect, localize and quantify 
+this particular source. 
+Also, there are limitations to the forward dispersion model which is used in the analysis. 
+For example, the performance of the Gaussian plume dispersion model will degrade at lower wind speeds. 
+Therefore, careful interpretation of the data is always required. 
+
 ***
 # Installing pyELQ as a package
 Suppose you want to use this pyELQ package in a different project.
 You can install it from [PyPi](https://pypi.org/project/pyelq-sdk/) through pip 
 `pip install pyelq-sdk`.
 Or you could clone the repository and install it from the source code. 
 After activating the environment you want to install pyELQ in, open a terminal, move to the main pyELQ folder
```

### Comparing `pyelq_sdk-1.0.4/pyproject.toml` & `pyelq_sdk-1.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyelq-sdk"
-version = "1.0.4"
+version = "1.0.5"
 description = "Package for detection, localization and quantification code."
 authors = ["Bas van de Kerkhof", "Matthew Jones", "David Randell"]
 homepage = "https://sede-open.github.io/pyELQ/"
 repository = "https://github.com/sede-open/pyELQ"
 documentation = "https://sede-open.github.io/pyELQ/"
 readme = "README.md"
 license = "Apache-2.0"
```

### Comparing `pyelq_sdk-1.0.4/src/pyelq/component/background.py` & `pyelq_sdk-1.0.5/src/pyelq/component/background.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.4/src/pyelq/component/component.py` & `pyelq_sdk-1.0.5/src/pyelq/component/component.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.4/src/pyelq/component/error_model.py` & `pyelq_sdk-1.0.5/src/pyelq/component/error_model.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.4/src/pyelq/component/offset.py` & `pyelq_sdk-1.0.5/src/pyelq/component/offset.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.4/src/pyelq/component/source_model.py` & `pyelq_sdk-1.0.5/src/pyelq/component/source_model.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.4/src/pyelq/coordinate_system.py` & `pyelq_sdk-1.0.5/src/pyelq/coordinate_system.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.4/src/pyelq/data_access/data_access.py` & `pyelq_sdk-1.0.5/src/pyelq/data_access/data_access.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.4/src/pyelq/dispersion_model/gaussian_plume.py` & `pyelq_sdk-1.0.5/src/pyelq/dispersion_model/gaussian_plume.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.4/src/pyelq/dlm.py` & `pyelq_sdk-1.0.5/src/pyelq/dlm.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.4/src/pyelq/gas_species.py` & `pyelq_sdk-1.0.5/src/pyelq/gas_species.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.4/src/pyelq/meteorology.py` & `pyelq_sdk-1.0.5/src/pyelq/meteorology.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.4/src/pyelq/model.py` & `pyelq_sdk-1.0.5/src/pyelq/model.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.4/src/pyelq/plotting/plot.py` & `pyelq_sdk-1.0.5/src/pyelq/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.4/src/pyelq/preprocessing.py` & `pyelq_sdk-1.0.5/src/pyelq/preprocessing.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.4/src/pyelq/sensor/beam.py` & `pyelq_sdk-1.0.5/src/pyelq/sensor/beam.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.4/src/pyelq/sensor/satellite.py` & `pyelq_sdk-1.0.5/src/pyelq/sensor/satellite.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.4/src/pyelq/sensor/sensor.py` & `pyelq_sdk-1.0.5/src/pyelq/sensor/sensor.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.4/src/pyelq/source_map.py` & `pyelq_sdk-1.0.5/src/pyelq/source_map.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.4/src/pyelq/support_functions/spatio_temporal_interpolation.py` & `pyelq_sdk-1.0.5/src/pyelq/support_functions/spatio_temporal_interpolation.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.4/PKG-INFO` & `pyelq_sdk-1.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyelq-sdk
-Version: 1.0.4
+Version: 1.0.5
 Summary: Package for detection, localization and quantification code.
 Home-page: https://sede-open.github.io/pyELQ/
 License: Apache-2.0
 Keywords: gas dispersion,emission,detection,localization,quantification
 Author: Bas van de Kerkhof
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
@@ -33,15 +33,14 @@
 
 <div align="center">
 
 [![PyPI version](https://img.shields.io/pypi/v/pyelq-sdk.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/pyelq-sdk/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/pyelq-sdk.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/pyelq-sdk/)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Code Style Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Tests](https://github.com/sede-open/pyelq/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/sede-open/pyelq/actions/workflows/main.yml)
 
 [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=pyelq_pyelq&metric=coverage)](https://sonarcloud.io/summary/new_code?id=pyelq_pyelq)
 [![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=pyelq_pyelq&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=pyelq_pyelq)
 [![Bugs](https://sonarcloud.io/api/project_badges/measure?project=pyelq_pyelq&metric=bugs)](https://sonarcloud.io/summary/new_code?id=pyelq_pyelq)
 [![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=pyelq_pyelq&metric=ncloc)](https://sonarcloud.io/summary/new_code?id=pyelq_pyelq)
 [![Duplicated Lines (%)](https://sonarcloud.io/api/project_badges/measure?project=pyelq_pyelq&metric=duplicated_lines_density)](https://sonarcloud.io/summary/new_code?id=pyelq_pyelq)
 [![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=pyelq_pyelq&metric=code_smells)](https://sonarcloud.io/summary/new_code?id=pyelq_pyelq)
@@ -74,14 +73,34 @@
 to support various assets in their quest to reduce methane emissions.
 
 Use cases where the pyELQ code has been applied are described in the following papers:
 
 * IJzermans, R., Jones, M., Weidmann, D. et al. "Long-term continuous monitoring of methane emissions at an oil and gas facility using a multi-open-path laser dispersion spectrometer." Sci Rep 14, 623 (2024). (https://doi.org/10.1038/s41598-023-50081-9)
 
 * Weidmann, D., Hirst, B. et al. "Locating and Quantifying Methane Emissions by Inverse Analysis of Path-Integrated Concentration Data Using a Markov-Chain Monte Carlo Approach." ACS Earth and Space Chemistry 2022 6 (9), 2190-2198  (https://doi.org/10.1021/acsearthspacechem.2c00093)
+
+## Deployment design
+The pyELQ code needs high-quality methane concentration and wind data to be able to provide reliable output on location 
+and quantification of methane emission sources. This requires methane concentration sensors of sufficiently high 
+precision in a layout that allows the detection of relevant methane emission sources, in combination with wind 
+measurements of high enough frequency and accuracy. The optimal sensor layout typically depends on the prevailing 
+meteorological conditions at the site of interest and requires multiple concentration sensors to cover the site under 
+different wind directions. 
+
+## pyELQ data interpretation
+The results from pyELQ come with uncertainty ranges that are representative of probability density functions sampled 
+by a Markov Chain Monte Carlo method. One should take these uncertainty ranges into account when interpreting the pyELQ 
+output data. Remember that absence of evidence for methane emissions does not always imply evidence for absence of 
+methane emissions; for instance, when meteorological conditions are such that there is no sensor downwind of a methane 
+source during the selected monitoring period, then it will be impossible to detect, localize and quantify 
+this particular source. 
+Also, there are limitations to the forward dispersion model which is used in the analysis. 
+For example, the performance of the Gaussian plume dispersion model will degrade at lower wind speeds. 
+Therefore, careful interpretation of the data is always required. 
+
 ***
 # Installing pyELQ as a package
 Suppose you want to use this pyELQ package in a different project.
 You can install it from [PyPi](https://pypi.org/project/pyelq-sdk/) through pip 
 `pip install pyelq-sdk`.
 Or you could clone the repository and install it from the source code. 
 After activating the environment you want to install pyELQ in, open a terminal, move to the main pyELQ folder
```

