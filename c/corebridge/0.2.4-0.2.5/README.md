# Comparing `tmp/corebridge-0.2.4.tar.gz` & `tmp/corebridge-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corebridge-0.2.4.tar", last modified: Thu May 16 18:01:00 2024, max compression
+gzip compressed data, was "corebridge-0.2.5.tar", last modified: Mon May 27 09:35:41 2024, max compression
```

## Comparing `corebridge-0.2.4.tar` & `corebridge-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-16 18:01:00.584577 corebridge-0.2.4/
--rw-r--r--   0 fenke     (1000) users      (100)    11337 2024-01-31 12:54:47.000000 corebridge-0.2.4/LICENSE
--rw-r--r--   0 fenke     (1000) users      (100)      111 2024-01-31 12:54:47.000000 corebridge-0.2.4/MANIFEST.in
--rw-r--r--   0 fenke     (1000) users      (100)     2655 2024-05-16 18:01:00.584577 corebridge-0.2.4/PKG-INFO
--rw-r--r--   0 fenke     (1000) users      (100)     1887 2024-05-03 10:28:01.000000 corebridge-0.2.4/README.md
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-16 18:01:00.580577 corebridge-0.2.4/corebridge/
--rw-r--r--   0 fenke     (1000) users      (100)       22 2024-05-16 18:00:41.000000 corebridge-0.2.4/corebridge/__init__.py
--rw-r--r--   0 fenke     (1000) users      (100)     2865 2024-05-16 18:00:41.000000 corebridge-0.2.4/corebridge/_modidx.py
--rw-r--r--   0 fenke     (1000) users      (100)     4613 2024-05-16 18:00:41.000000 corebridge-0.2.4/corebridge/aicorebridge.py
--rw-r--r--   0 fenke     (1000) users      (100)     4464 2024-05-16 18:00:41.000000 corebridge-0.2.4/corebridge/core.py
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-16 18:01:00.584577 corebridge-0.2.4/corebridge.egg-info/
--rw-r--r--   0 fenke     (1000) users      (100)     2655 2024-05-16 18:01:00.000000 corebridge-0.2.4/corebridge.egg-info/PKG-INFO
--rw-r--r--   0 fenke     (1000) users      (100)      381 2024-05-16 18:01:00.000000 corebridge-0.2.4/corebridge.egg-info/SOURCES.txt
--rw-r--r--   0 fenke     (1000) users      (100)        1 2024-05-16 18:01:00.000000 corebridge-0.2.4/corebridge.egg-info/dependency_links.txt
--rw-r--r--   0 fenke     (1000) users      (100)       42 2024-05-16 18:01:00.000000 corebridge-0.2.4/corebridge.egg-info/entry_points.txt
--rw-r--r--   0 fenke     (1000) users      (100)        1 2024-01-31 15:42:47.000000 corebridge-0.2.4/corebridge.egg-info/not-zip-safe
--rw-r--r--   0 fenke     (1000) users      (100)      279 2024-05-16 18:01:00.000000 corebridge-0.2.4/corebridge.egg-info/requires.txt
--rw-r--r--   0 fenke     (1000) users      (100)       11 2024-05-16 18:01:00.000000 corebridge-0.2.4/corebridge.egg-info/top_level.txt
--rw-r--r--   0 fenke     (1000) users      (100)     1200 2024-05-16 18:00:54.000000 corebridge-0.2.4/settings.ini
--rw-r--r--   0 fenke     (1000) users      (100)       38 2024-05-16 18:01:00.584577 corebridge-0.2.4/setup.cfg
--rw-r--r--   0 fenke     (1000) users      (100)     2596 2024-01-31 12:54:47.000000 corebridge-0.2.4/setup.py
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-27 09:35:40.995732 corebridge-0.2.5/
+-rw-r--r--   0 fenke     (1000) users      (100)    11337 2024-01-31 12:54:47.000000 corebridge-0.2.5/LICENSE
+-rw-r--r--   0 fenke     (1000) users      (100)      111 2024-01-31 12:54:47.000000 corebridge-0.2.5/MANIFEST.in
+-rw-r--r--   0 fenke     (1000) users      (100)     3185 2024-05-27 09:35:40.995732 corebridge-0.2.5/PKG-INFO
+-rw-r--r--   0 fenke     (1000) users      (100)     2417 2024-05-27 09:35:23.000000 corebridge-0.2.5/README.md
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-27 09:35:40.995732 corebridge-0.2.5/corebridge/
+-rw-r--r--   0 fenke     (1000) users      (100)       22 2024-05-27 09:35:30.000000 corebridge-0.2.5/corebridge/__init__.py
+-rw-r--r--   0 fenke     (1000) users      (100)     2865 2024-05-27 09:35:30.000000 corebridge-0.2.5/corebridge/_modidx.py
+-rw-r--r--   0 fenke     (1000) users      (100)     4653 2024-05-27 09:35:30.000000 corebridge-0.2.5/corebridge/aicorebridge.py
+-rw-r--r--   0 fenke     (1000) users      (100)     4456 2024-05-27 09:35:30.000000 corebridge-0.2.5/corebridge/core.py
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-27 09:35:40.995732 corebridge-0.2.5/corebridge.egg-info/
+-rw-r--r--   0 fenke     (1000) users      (100)     3185 2024-05-27 09:35:40.000000 corebridge-0.2.5/corebridge.egg-info/PKG-INFO
+-rw-r--r--   0 fenke     (1000) users      (100)      381 2024-05-27 09:35:40.000000 corebridge-0.2.5/corebridge.egg-info/SOURCES.txt
+-rw-r--r--   0 fenke     (1000) users      (100)        1 2024-05-27 09:35:40.000000 corebridge-0.2.5/corebridge.egg-info/dependency_links.txt
+-rw-r--r--   0 fenke     (1000) users      (100)       42 2024-05-27 09:35:40.000000 corebridge-0.2.5/corebridge.egg-info/entry_points.txt
+-rw-r--r--   0 fenke     (1000) users      (100)        1 2024-01-31 15:42:47.000000 corebridge-0.2.5/corebridge.egg-info/not-zip-safe
+-rw-r--r--   0 fenke     (1000) users      (100)      287 2024-05-27 09:35:40.000000 corebridge-0.2.5/corebridge.egg-info/requires.txt
+-rw-r--r--   0 fenke     (1000) users      (100)       11 2024-05-27 09:35:40.000000 corebridge-0.2.5/corebridge.egg-info/top_level.txt
+-rw-r--r--   0 fenke     (1000) users      (100)     1208 2024-05-27 09:34:54.000000 corebridge-0.2.5/settings.ini
+-rw-r--r--   0 fenke     (1000) users      (100)       38 2024-05-27 09:35:40.995732 corebridge-0.2.5/setup.cfg
+-rw-r--r--   0 fenke     (1000) users      (100)     2596 2024-01-31 12:54:47.000000 corebridge-0.2.5/setup.py
```

### Comparing `corebridge-0.2.4/LICENSE` & `corebridge-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `corebridge-0.2.4/PKG-INFO` & `corebridge-0.2.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corebridge
-Version: 0.2.4
+Version: 0.2.5
 Summary: Bridge for Stactics AICore
 Home-page: https://github.com/fenke/corebridge
 Author: Fenke Meijer
 Author-email: fenkemeijer@gmail.com
 License: Apache Software License 2.0
 Keywords: python aicore stactics whysor
 Classifier: Development Status :: 4 - Beta
@@ -24,26 +24,28 @@
 
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 This package provides functions and classes to run wodan style
 processing functions in the Stactics AICore environment.
 
-## Install
+## Installation
+
+Use
 
 ``` sh
 pip install corebridge
 ```
 
+to install corebrdige.
+
 ## How to use
 
 ### Introduction
 
-#### Wodan processing functions
-
 Wodan is a proprietary backend service that applies high performance,
 custom analytical processing to timeseries data in the Whysor data and
 dashboarding environment.
 
 Each wodan module defines one function that operates as the entry point.
 The parameter annotations in this function definition are used to format
 data and retrieve parameters from the originating call to the wodan api.
@@ -56,47 +58,60 @@
 import numpy as np
 
 def multiply(data:np.ndarray, multiplier:float=1.0):
     return data * multiplier
     
 ```
 
-#### AICore modules
+Wodan binds this function to a service endpoint and takes care of
+fetching data and parameters and converting the result for the caller.
+
+### AICore modules
 
-For AICore one defines a class, always named `Module` with a constructor
-`__init__` and a method `infer`.
+For AICore users define a class, always named `Module` with a
+constructor `__init__` and a method `infer`.
 
 This package defines a baseclass to quickly construct a custom `Module`
-class that uses a wodan processor function inside the AICore system:
+class that is able to use a wodan processor function inside the AICore
+system:
 
 ``` {python}
 import numpy as np
 import corebridge
 
 def multiply(data:np.ndarray, multiplier:float=1.0):
     return data * multiplier
 
 class Module(corebridge.aicorebridge.AICoreModule):
     def __init__(self, save_dir, assets_dir, *args, **kwargs):
-        super().__init__(read, save_dir, assets_dir, *args, **kwargs)
+        super().__init__(multiply, save_dir, assets_dir, *args, **kwargs)
     
 ```
 
 That’s it. Well, you can add parameters to `__init__` that can be used
-as hyperparameters and you could override `infer` for the same reason.
+as hyperparameters in the web-interface and you could override `infer`
+for the same reason. The baseclass takes care of converting call
+parameters and data to the function specification and, calls the
+function and converts the result for the caller, similar to the original
+Wodan service.
 
-``` python
-```
+## Development
+
+Setup a virtual environment, activate it and install the development
+package and dependencies with, on linux
+
+        pip install -e ‘.\[dev\]’
+
+or on Windows
 
-    2
+        pip install -e .\[dev\]
 
-## nbdev cycle
+### nbdev cycle
 
 - edit
 - nbdev_export
-- pip install -e ‘.\[dev\]’
 - nbdev_test
 - nbdev_clean
 - nbdev_readme
 - nbdev_prepare
 - git add .
 -
```

### Comparing `corebridge-0.2.4/corebridge/_modidx.py` & `corebridge-0.2.5/corebridge/_modidx.py`

 * *Files identical despite different names*

### Comparing `corebridge-0.2.4/corebridge/aicorebridge.py` & `corebridge-0.2.5/corebridge/aicorebridge.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,22 +10,23 @@
 import datetime
 import json
 import pandas as pd
 import numpy as np
 
 from fastcore.basics import patch_to, patch
 from .core import *
+from . import __version__
 
 
 # %% ../nbs/01_aicorebridge.ipynb 5
 syslog = logging.getLogger(__name__)
 
 # %% ../nbs/01_aicorebridge.ipynb 6
 try:
-    print(f"Loading {__name__} from {__file__}")
+    print(f"Loading {__name__} {__version__} from {__file__}")
 except:
     pass
 
 # %% ../nbs/01_aicorebridge.ipynb 7
 class AICoreModule(): pass
 
 # %% ../nbs/01_aicorebridge.ipynb 8
```

### Comparing `corebridge-0.2.4/corebridge/core.py` & `corebridge-0.2.5/corebridge/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,23 +91,25 @@
     "Convert data dict to dataframe"
 
     orient = recordformat.lower()
     assert orient in ['records', 'table']
     
     if orient == 'records':
         df = pd.DataFrame.from_records(data)
-        time_column = [C for C in df.columns if C.lower() in timecolumns][0]
+        time_column = [C for C in df.columns if C in timecolumns][0]
 
     elif orient == 'table':
         time_column = data['schema']['primaryKey'][0]
         df = pd.DataFrame.from_dict(data['data']).set_index(data['schema']['primaryKey'])
         df.index.name = 'time'
+    else:
+        time_column = [C for C in df.columns if C in timecolumns][0]
 
-    df.columns = [C.lower() for C in df.columns]
-    time_column = [C for C in df.columns if C in timecolumns][0]
+
+    df.columns = list(df.columns)
     df[time_column] = pd.to_datetime(df[time_column],utc=True,format='ISO8601')
     df.set_index(time_column, inplace=True)
     #df.index = pd.DatetimeIndex(df.index).round('ms')
     
     df.index.name = 'time'
 
     return df
```

### Comparing `corebridge-0.2.4/corebridge.egg-info/PKG-INFO` & `corebridge-0.2.5/corebridge.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corebridge
-Version: 0.2.4
+Version: 0.2.5
 Summary: Bridge for Stactics AICore
 Home-page: https://github.com/fenke/corebridge
 Author: Fenke Meijer
 Author-email: fenkemeijer@gmail.com
 License: Apache Software License 2.0
 Keywords: python aicore stactics whysor
 Classifier: Development Status :: 4 - Beta
@@ -24,26 +24,28 @@
 
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 This package provides functions and classes to run wodan style
 processing functions in the Stactics AICore environment.
 
-## Install
+## Installation
+
+Use
 
 ``` sh
 pip install corebridge
 ```
 
+to install corebrdige.
+
 ## How to use
 
 ### Introduction
 
-#### Wodan processing functions
-
 Wodan is a proprietary backend service that applies high performance,
 custom analytical processing to timeseries data in the Whysor data and
 dashboarding environment.
 
 Each wodan module defines one function that operates as the entry point.
 The parameter annotations in this function definition are used to format
 data and retrieve parameters from the originating call to the wodan api.
@@ -56,47 +58,60 @@
 import numpy as np
 
 def multiply(data:np.ndarray, multiplier:float=1.0):
     return data * multiplier
     
 ```
 
-#### AICore modules
+Wodan binds this function to a service endpoint and takes care of
+fetching data and parameters and converting the result for the caller.
+
+### AICore modules
 
-For AICore one defines a class, always named `Module` with a constructor
-`__init__` and a method `infer`.
+For AICore users define a class, always named `Module` with a
+constructor `__init__` and a method `infer`.
 
 This package defines a baseclass to quickly construct a custom `Module`
-class that uses a wodan processor function inside the AICore system:
+class that is able to use a wodan processor function inside the AICore
+system:
 
 ``` {python}
 import numpy as np
 import corebridge
 
 def multiply(data:np.ndarray, multiplier:float=1.0):
     return data * multiplier
 
 class Module(corebridge.aicorebridge.AICoreModule):
     def __init__(self, save_dir, assets_dir, *args, **kwargs):
-        super().__init__(read, save_dir, assets_dir, *args, **kwargs)
+        super().__init__(multiply, save_dir, assets_dir, *args, **kwargs)
     
 ```
 
 That’s it. Well, you can add parameters to `__init__` that can be used
-as hyperparameters and you could override `infer` for the same reason.
+as hyperparameters in the web-interface and you could override `infer`
+for the same reason. The baseclass takes care of converting call
+parameters and data to the function specification and, calls the
+function and converts the result for the caller, similar to the original
+Wodan service.
 
-``` python
-```
+## Development
+
+Setup a virtual environment, activate it and install the development
+package and dependencies with, on linux
+
+        pip install -e ‘.\[dev\]’
+
+or on Windows
 
-    2
+        pip install -e .\[dev\]
 
-## nbdev cycle
+### nbdev cycle
 
 - edit
 - nbdev_export
-- pip install -e ‘.\[dev\]’
 - nbdev_test
 - nbdev_clean
 - nbdev_readme
 - nbdev_prepare
 - git add .
 -
```

### Comparing `corebridge-0.2.4/settings.ini` & `corebridge-0.2.5/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = corebridge
 lib_name = %(repo)s
-version = 0.2.4
+version = 0.2.5
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = corebridge
@@ -35,9 +35,9 @@
 keywords = python aicore stactics whysor
 language = English
 status = 3
 user = fenke
 
 ### Optional ###
 requirements = python-dateutil pytz numpy pandas scipy scikit-learn fastcore twine
-dev_requirements = python-dateutil pytz numpy pyarrow pandas scipy scikit-learn fastcore jupyter ipywidgets jupyterlab>4 jupyter_contrib_nbextensions jupyterlab-git jupyterlab-quarto nbdev aiohttp asyncpg apscheduler twine
+dev_requirements = python-dateutil pytz numpy pyarrow pandas scipy scikit-learn fastcore jupyter ipywidgets jupyterlab>4 jupyter_contrib_nbextensions jupyterlab-git jupyterlab-quarto nbdev aiohttp asyncpg apscheduler twine addroot
 # console_scripts =
```

### Comparing `corebridge-0.2.4/setup.py` & `corebridge-0.2.5/setup.py`

 * *Files identical despite different names*

