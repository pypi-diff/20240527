# Comparing `tmp/absplit-1.4.4.tar.gz` & `tmp/absplit-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absplit-1.4.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "absplit-1.4.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `absplit-1.4.4.tar` & `absplit-1.4.5.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     4976 2023-07-02 18:57:33.878000 absplit-1.4.4/.gitignore
--rw-r--r--   0        0        0       50 2023-02-18 09:46:26.039000 absplit-1.4.4/.idea/.gitignore
--rw-r--r--   0        0        0      291 2023-06-12 08:40:13.087000 absplit-1.4.4/.idea/genetic_algorithm.iml
--rw-r--r--   0        0        0      179 2023-02-18 09:46:26.072000 absplit-1.4.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      303 2023-06-12 08:40:13.168000 absplit-1.4.4/.idea/misc.xml
--rw-r--r--   0        0        0      293 2023-02-18 09:46:26.093000 absplit-1.4.4/.idea/modules.xml
--rw-r--r--   0        0        0      185 2023-02-18 09:46:26.104000 absplit-1.4.4/.idea/vcs.xml
--rw-r--r--   0        0        0     1026 2023-02-18 09:46:26.114000 absplit-1.4.4/LICENSE
--rw-r--r--   0        0        0      152 2023-02-18 09:46:26.124000 absplit-1.4.4/MANIFEST.in
--rw-r--r--   0        0        0     9422 2024-02-10 19:07:25.847000 absplit-1.4.4/README.md
--rw-r--r--   0        0        0       93 2024-02-10 19:07:25.911000 absplit-1.4.4/absplit/__init__.py
--rw-r--r--   0        0        0    14169 2023-07-02 21:37:04.782000 absplit-1.4.4/absplit/data.py
--rw-r--r--   0        0        0    30539 2023-07-02 21:18:26.583000 absplit-1.4.4/absplit/ga.py
--rw-r--r--   0        0        0      948 2023-07-02 21:08:06.736000 absplit-1.4.4/absplit/log.py
--rw-r--r--   0        0        0     1866 2023-02-18 09:46:26.177000 absplit-1.4.4/absplit/param.py
--rw-r--r--   0        0        0     4985 2023-07-02 19:20:22.297000 absplit-1.4.4/absplit/tutorials.py
--rw-r--r--   0        0        0   330866 2024-02-10 18:06:56.174000 absplit-1.4.4/images/calculation_diagram.png
--rw-r--r--   0        0        0    29186 2023-02-18 09:46:26.190000 absplit-1.4.4/images/logo.jpeg
--rw-r--r--   0        0        0     1533 2024-02-10 19:07:25.775000 absplit-1.4.4/pyproject.toml
--rw-r--r--   0        0        0       50 2023-06-05 23:23:06.260000 absplit-1.4.4/requirements.txt
--rw-r--r--   0        0        0        0 2023-02-18 09:46:26.220000 absplit-1.4.4/tests/__init__.py
--rw-r--r--   0        0        0     6678 2023-07-02 21:38:57.605000 absplit-1.4.4/tests/test_data.py
--rw-r--r--   0        0        0     5332 2023-07-02 21:01:43.528000 absplit-1.4.4/tests/test_ga.py
--rw-r--r--   0        0        0    10432 1970-01-01 00:00:00.000000 absplit-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0     5282 2024-05-27 19:47:54.545000 absplit-1.4.5/.gitignore
+-rw-r--r--   0        0        0       50 2023-02-18 09:46:26.039000 absplit-1.4.5/.idea/.gitignore
+-rw-r--r--   0        0        0      291 2023-06-12 08:40:13.087000 absplit-1.4.5/.idea/genetic_algorithm.iml
+-rw-r--r--   0        0        0      179 2023-02-18 09:46:26.072000 absplit-1.4.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      303 2023-06-12 08:40:13.168000 absplit-1.4.5/.idea/misc.xml
+-rw-r--r--   0        0        0      293 2023-02-18 09:46:26.093000 absplit-1.4.5/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2023-02-18 09:46:26.104000 absplit-1.4.5/.idea/vcs.xml
+-rw-r--r--   0        0        0     1026 2023-02-18 09:46:26.114000 absplit-1.4.5/LICENSE
+-rw-r--r--   0        0        0      152 2023-02-18 09:46:26.124000 absplit-1.4.5/MANIFEST.in
+-rw-r--r--   0        0        0     9612 2024-05-27 15:51:20.089000 absplit-1.4.5/README.md
+-rw-r--r--   0        0        0       95 2024-05-27 15:51:36.145000 absplit-1.4.5/absplit/__init__.py
+-rw-r--r--   0        0        0    14169 2023-07-02 21:37:04.782000 absplit-1.4.5/absplit/data.py
+-rw-r--r--   0        0        0    30539 2023-07-02 21:18:26.583000 absplit-1.4.5/absplit/ga.py
+-rw-r--r--   0        0        0      948 2023-07-02 21:08:06.736000 absplit-1.4.5/absplit/log.py
+-rw-r--r--   0        0        0     1866 2023-02-18 09:46:26.177000 absplit-1.4.5/absplit/param.py
+-rw-r--r--   0        0        0     4987 2024-05-27 19:40:16.400000 absplit-1.4.5/absplit/tutorials.py
+-rw-r--r--   0        0        0   330866 2024-02-10 18:06:56.174000 absplit-1.4.5/images/calculation_diagram.png
+-rw-r--r--   0        0        0    29186 2023-02-18 09:46:26.190000 absplit-1.4.5/images/logo.jpeg
+-rw-r--r--   0        0        0     1533 2024-05-27 19:50:36.727000 absplit-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0      137 2024-05-27 19:34:33.107000 absplit-1.4.5/pytest.ini
+-rw-r--r--   0        0        0       50 2024-05-27 19:50:46.239000 absplit-1.4.5/requirements.txt
+-rw-r--r--   0        0        0       31 2024-05-27 19:41:10.559000 absplit-1.4.5/setup.cfg
+-rw-r--r--   0        0        0        0 2023-02-18 09:46:26.220000 absplit-1.4.5/tests/__init__.py
+-rw-r--r--   0        0        0     7260 2024-05-27 19:44:50.618000 absplit-1.4.5/tests/test_data.py
+-rw-r--r--   0        0        0     5354 2024-05-27 19:46:15.671000 absplit-1.4.5/tests/test_ga.py
+-rw-r--r--   0        0        0    10619 1970-01-01 00:00:00.000000 absplit-1.4.5/PKG-INFO
```

### Comparing `absplit-1.4.4/.gitignore` & `absplit-1.4.5/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,29 @@
 archive/
 data/
 notebooks/
 .pypirc
 notes.txt
 absplit/log_flag
 
+# User-specific stuff:
+.idea/workspace.xml
+.idea/tasks.xml
+.idea/dictionaries
+.idea/vcs.xml
+.idea/jsLibraryMappings.xml
+
+# Sensitive or high-churn files:
+.idea/dataSources.ids
+.idea/dataSources.xml
+.idea/dataSources.local.xml
+.idea/sqlDataSources.xml
+.idea/dynamic.xml
+.idea/uiDesigner.xml
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `absplit-1.4.4/LICENSE` & `absplit-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `absplit-1.4.4/README.md` & `absplit-1.4.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg" width="460" height="140">
 <h3><strong>ABSplit</strong></h3>
 Split your data into matching A/B/n groups
 
 ![license](https://img.shields.io/badge/License-MIT-blue.svg)
-![version](https://img.shields.io/badge/version-1.4.4-blue.svg)
+![version](https://img.shields.io/badge/version-1.4.5-blue.svg)
 ![version](https://img.shields.io/badge/python-3-orange.svg)
+[![Downloads](https://static.pepy.tech/badge/absplit)](https://pepy.tech/project/absplit)
+[![Downloads](https://static.pepy.tech/badge/absplit/month)](https://pepy.tech/project/absplit)
 
 </div>
 
 <details open>
   <summary>Table of Contents</summary>
   <ol>
     <li>
@@ -217,8 +219,8 @@
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,12 +1,15 @@
 [https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg]
                                ******** AABBSSpplliitt ********
  Split your data into matching A/B/n groups ![license](https://img.shields.io/
  badge/License-MIT-blue.svg) ![version](https://img.shields.io/badge/version-
- 1.4.4-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
+1.4.5-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg) [!
+[Downloads](https://static.pepy.tech/badge/absplit)](https://pepy.tech/project/
+absplit) [![Downloads](https://static.pepy.tech/badge/absplit/month)](https://
+                          pepy.tech/project/absplit)
 Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _C_a_l_c_u_l_a_t_i_o_n
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
           o _I_n_s_t_a_l_l_a_t_i_o_n
    3. _T_u_t_o_r_i_a_l_s
           o _D_o_ _i_t_ _y_o_u_r_s_e_l_f
```

### Comparing `absplit-1.4.4/absplit/data.py` & `absplit-1.4.5/absplit/data.py`

 * *Files identical despite different names*

### Comparing `absplit-1.4.4/absplit/ga.py` & `absplit-1.4.5/absplit/ga.py`

 * *Files identical despite different names*

### Comparing `absplit-1.4.4/absplit/log.py` & `absplit-1.4.5/absplit/log.py`

 * *Files identical despite different names*

### Comparing `absplit-1.4.4/absplit/param.py` & `absplit-1.4.5/absplit/param.py`

 * *Files identical despite different names*

### Comparing `absplit-1.4.4/absplit/tutorials.py` & `absplit-1.4.5/absplit/tutorials.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     return df
 
 
 def covid(test=False, drop_fips=True):
     url = 'https://raw.githubusercontent.com/nytimes/covid-19-data/master/us-counties.csv'
     if test:
-        url = '../data/us-counties.csv'
+        url = './data/us-counties.csv'
         print(f'TEST mode, pulling file')
     else:
         print(f'Pulling data from {url}')
     df = pd.read_csv(url)
     print(f'Cleaning and resampling data..')
 
     # Remove Puerto Rico because of NaNs
@@ -76,18 +76,19 @@
     cols = cols + ['fips'] if not drop_fips else cols
     df = df.set_index(cols).sort_index()
     df = df.groupby(level=[0, 1]).diff().fillna(0).clip(lower=0)
     resampler = lambda x: x.set_index('date').resample('w').sum()
     df = df.reset_index(level=2).groupby([x for x in cols if x != 'date']).apply(resampler).reset_index()
     return df
 
+
 def retail(test=False):
     url = 'https://raw.githubusercontent.com/nytimes/covid-19-data/master/us-counties.csv'
     if test:
-        url = '../data/online-retail.csv'
+        url = './data/online-retail.csv'
         print(f'TEST mode, pulling file')
     else:
         print(f'Pulling data from {url}')
     df = pd.read_csv(url)
     print(f'Cleaning and resampling data..')
 
     df.columns = [x.lower().replace(' ', '_') for x in df.columns]
@@ -102,14 +103,15 @@
         'cost': 'sum',
         'quantity': 'sum',
         'stockcode': pd.Series.nunique
     }
     df2 = df.groupby(['week', 'customer_id']).agg(agg_dct).reset_index().drop('stockcode', axis=1)
     return df2
 
+
 def display(df):
     for i in range(5):
         df_ = df[df['id'] == i]
         plt.plot(df_['date'].values, df_['metric1'].values, label=f'id: {i}')
 
     plt.xticks(rotation=45)
     plt.title('metric1')
```

### Comparing `absplit-1.4.4/images/calculation_diagram.png` & `absplit-1.4.5/images/calculation_diagram.png`

 * *Files identical despite different names*

### Comparing `absplit-1.4.4/images/logo.jpeg` & `absplit-1.4.5/images/logo.jpeg`

 * *Files identical despite different names*

### Comparing `absplit-1.4.4/pyproject.toml` & `absplit-1.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "absplit"
-version = "1.4.4"
+version = "1.4.5"
 description = "Generates A/B/n test groups"
 readme = "README.md"
 authors = [{name = "Cormac Rynne", email = "cormac.ry@gmail.com"}]
 license = {file = "LICENSE"}
 repository = "https://github.com/cormac-rynne/absplit"
 requires-python = "<=3.11"
 classifiers = [
@@ -33,15 +33,15 @@
     "ab test",
     "ab split",
     "split",
     'set formation',
     'group formation'
 ]
 dependencies = [
-    "pygad==3.0.1",
+    "pygad<=3.3.1",
     "scikit-learn",
     "numpy",
     "pandas",
     "seaborn"
 ]
 
 [tool.flit.external-data]
```

### Comparing `absplit-1.4.4/tests/test_data.py` & `absplit-1.4.5/tests/test_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,137 +2,171 @@
 import datetime
 import numpy as np
 import pandas as pd
 from absplit.data import Data
 from sklearn.preprocessing import MinMaxScaler
 import pytest
 
+
 @pytest.fixture
 def data_dct():
     return {
-        'date': [dt.date(2030,4,1) + dt.timedelta(days=x) for x in range(3)]*5,
+        'date': [dt.date(2030, 4, 1) + dt.timedelta(days=x) for x in range(3)] * 5,
         'country': ['UK'] * 15,
         'region': [item for sublist in [[x]*6 for x in ['z', 'y']] for item in sublist] + ['x']*3,
         'city': [item for sublist in [[x]*3 for x in ['a', 'b', 'c', 'd', 'e']] for item in sublist],
         'metric1': np.arange(0, 15, 1),
         'metric2': np.arange(0, 150, 10)
     }
 
+
 @pytest.fixture
 def df(data_dct):
     return pd.DataFrame(data_dct)
 
+
 @pytest.fixture
 def kwargs():
     return {
         'metrics': ['metric1', 'metric2'],
         'date_col': 'date',
         'splitting': 'city'
     }
 
+
 @pytest.fixture
 def data1(df, kwargs):
     return Data(df=df, **kwargs)
 
+
 def test_initialization(df, kwargs):
     scaler = MinMaxScaler().fit(df[['metric1', 'metric2']])
     data = Data(df=df, scaler=scaler, cutoff_date='2030-04-02', **kwargs)
     assert isinstance(data._pre_fit_scaler, MinMaxScaler)
     assert data._cutoff_date == pd.to_datetime('2030-04-02')
     assert data.stacked.index.get_level_values('date').dtype == 'datetime64[ns]'
 
+
 def test_check_dates_error(df, kwargs):
     with pytest.raises(ValueError):
-        data = Data(df=df, cutoff_date='2040-01-01', **kwargs)
+        _ = Data(df=df, cutoff_date='2040-01-01', **kwargs)
+
 
 def test_run_timeseries_checks_error(df, kwargs):
     with pytest.raises(ValueError):
         df.loc[:, 'metric1'] = np.nan
-        data = Data(df=df, missing_dates='invalid_missing_dates', **kwargs)
+        _ = Data(df=df, missing_dates='invalid_missing_dates', **kwargs)
+
 
 def test_remainder_cols(data1):
     assert data1.remainder_cols == ['country', 'region']
 
+
 def test_stacked(data1):
     dct = {
-        'metric1': {('UK', 'x', 'e', dt.date(2030, 4, 1)): 12,
-        ('UK', 'x', 'e', dt.date(2030, 4, 2)): 13,
-        ('UK', 'x', 'e', dt.date(2030, 4, 3)): 14,
-        ('UK', 'y', 'c', dt.date(2030, 4, 1)): 6,
-        ('UK', 'y', 'c', dt.date(2030, 4, 2)): 7,
-        ('UK', 'y', 'c', dt.date(2030, 4, 3)): 8,
-        ('UK', 'y', 'd', dt.date(2030, 4, 1)): 9,
-        ('UK', 'y', 'd', dt.date(2030, 4, 2)): 10,
-        ('UK', 'y', 'd', dt.date(2030, 4, 3)): 11,
-        ('UK', 'z', 'a', dt.date(2030, 4, 1)): 0,
-        ('UK', 'z', 'a', dt.date(2030, 4, 2)): 1,
-        ('UK', 'z', 'a', dt.date(2030, 4, 3)): 2,
-        ('UK', 'z', 'b', dt.date(2030, 4, 1)): 3,
-        ('UK', 'z', 'b', dt.date(2030, 4, 2)): 4,
-        ('UK', 'z', 'b', dt.date(2030, 4, 3)): 5},
-        'metric2': {('UK', 'x', 'e', dt.date(2030, 4, 1)): 120,
-        ('UK', 'x', 'e', dt.date(2030, 4, 2)): 130,
-        ('UK', 'x', 'e', dt.date(2030, 4, 3)): 140,
-        ('UK', 'y', 'c', dt.date(2030, 4, 1)): 60,
-        ('UK', 'y', 'c', dt.date(2030, 4, 2)): 70,
-        ('UK', 'y', 'c', dt.date(2030, 4, 3)): 80,
-        ('UK', 'y', 'd', dt.date(2030, 4, 1)): 90,
-        ('UK', 'y', 'd', dt.date(2030, 4, 2)): 100,
-        ('UK', 'y', 'd', dt.date(2030, 4, 3)): 110,
-        ('UK', 'z', 'a', dt.date(2030, 4, 1)): 0,
-        ('UK', 'z', 'a', dt.date(2030, 4, 2)): 10,
-        ('UK', 'z', 'a', dt.date(2030, 4, 3)): 20,
-        ('UK', 'z', 'b', dt.date(2030, 4, 1)): 30,
-        ('UK', 'z', 'b', dt.date(2030, 4, 2)): 40,
-        ('UK', 'z', 'b', dt.date(2030, 4, 3)): 50}}
+        'metric1': {
+            ('UK', 'x', 'e', dt.date(2030, 4, 1)): 12,
+            ('UK', 'x', 'e', dt.date(2030, 4, 2)): 13,
+            ('UK', 'x', 'e', dt.date(2030, 4, 3)): 14,
+            ('UK', 'y', 'c', dt.date(2030, 4, 1)): 6,
+            ('UK', 'y', 'c', dt.date(2030, 4, 2)): 7,
+            ('UK', 'y', 'c', dt.date(2030, 4, 3)): 8,
+            ('UK', 'y', 'd', dt.date(2030, 4, 1)): 9,
+            ('UK', 'y', 'd', dt.date(2030, 4, 2)): 10,
+            ('UK', 'y', 'd', dt.date(2030, 4, 3)): 11,
+            ('UK', 'z', 'a', dt.date(2030, 4, 1)): 0,
+            ('UK', 'z', 'a', dt.date(2030, 4, 2)): 1,
+            ('UK', 'z', 'a', dt.date(2030, 4, 3)): 2,
+            ('UK', 'z', 'b', dt.date(2030, 4, 1)): 3,
+            ('UK', 'z', 'b', dt.date(2030, 4, 2)): 4,
+            ('UK', 'z', 'b', dt.date(2030, 4, 3)): 5},
+        'metric2': {
+            ('UK', 'x', 'e', dt.date(2030, 4, 1)): 120,
+            ('UK', 'x', 'e', dt.date(2030, 4, 2)): 130,
+            ('UK', 'x', 'e', dt.date(2030, 4, 3)): 140,
+            ('UK', 'y', 'c', dt.date(2030, 4, 1)): 60,
+            ('UK', 'y', 'c', dt.date(2030, 4, 2)): 70,
+            ('UK', 'y', 'c', dt.date(2030, 4, 3)): 80,
+            ('UK', 'y', 'd', dt.date(2030, 4, 1)): 90,
+            ('UK', 'y', 'd', dt.date(2030, 4, 2)): 100,
+            ('UK', 'y', 'd', dt.date(2030, 4, 3)): 110,
+            ('UK', 'z', 'a', dt.date(2030, 4, 1)): 0,
+            ('UK', 'z', 'a', dt.date(2030, 4, 2)): 10,
+            ('UK', 'z', 'a', dt.date(2030, 4, 3)): 20,
+            ('UK', 'z', 'b', dt.date(2030, 4, 1)): 30,
+            ('UK', 'z', 'b', dt.date(2030, 4, 2)): 40,
+            ('UK', 'z', 'b', dt.date(2030, 4, 3)): 50
+        }
+    }
     assert data1.stacked.to_dict() == dct
 
 
 def test_unstacked(data1):
-    dct = {('metric1', dt.date(2030, 4, 1)): {('UK', 'x', 'e'): 0.8571428571428571,
-        ('UK', 'y', 'c'): 0.42857142857142855,
-        ('UK', 'y', 'd'): 0.6428571428571428,
-        ('UK', 'z', 'a'): 0.0,
-        ('UK', 'z', 'b'): 0.21428571428571427},
-        ('metric1', dt.date(2030, 4, 2)): {('UK', 'x', 'e'): 0.9285714285714285,
-        ('UK', 'y', 'c'): 0.5,
-        ('UK', 'y', 'd'): 0.7142857142857142,
-        ('UK', 'z', 'a'): 0.07142857142857142,
-        ('UK', 'z', 'b'): 0.2857142857142857},
-        ('metric1', dt.date(2030, 4, 3)): {('UK', 'x', 'e'): 1.0,
-        ('UK', 'y', 'c'): 0.5714285714285714,
-        ('UK', 'y', 'd'): 0.7857142857142857,
-        ('UK', 'z', 'a'): 0.14285714285714285,
-        ('UK', 'z', 'b'): 0.3571428571428571},
-        ('metric2', dt.date(2030, 4, 1)): {('UK', 'x', 'e'): 0.8571428571428571,
-        ('UK', 'y', 'c'): 0.42857142857142855,
-        ('UK', 'y', 'd'): 0.6428571428571428,
-        ('UK', 'z', 'a'): 0.0,
-        ('UK', 'z', 'b'): 0.21428571428571427},
-        ('metric2', dt.date(2030, 4, 2)): {('UK', 'x', 'e'): 0.9285714285714285,
-        ('UK', 'y', 'c'): 0.5,
-        ('UK', 'y', 'd'): 0.7142857142857143,
-        ('UK', 'z', 'a'): 0.07142857142857142,
-        ('UK', 'z', 'b'): 0.2857142857142857},
-        ('metric2', dt.date(2030, 4, 3)): {('UK', 'x', 'e'): 1.0,
-        ('UK', 'y', 'c'): 0.5714285714285714,
-        ('UK', 'y', 'd'): 0.7857142857142857,
-        ('UK', 'z', 'a'): 0.14285714285714285,
-        ('UK', 'z', 'b'): 0.35714285714285715}}
+    dct = {
+        ('metric1', dt.date(2030, 4, 1)): {
+            ('UK', 'x', 'e'): 0.8571428571428571,
+            ('UK', 'y', 'c'): 0.42857142857142855,
+            ('UK', 'y', 'd'): 0.6428571428571428,
+            ('UK', 'z', 'a'): 0.0,
+            ('UK', 'z', 'b'): 0.21428571428571427
+        },
+        ('metric1', dt.date(2030, 4, 2)): {
+            ('UK', 'x', 'e'): 0.9285714285714285,
+            ('UK', 'y', 'c'): 0.5,
+            ('UK', 'y', 'd'): 0.7142857142857142,
+            ('UK', 'z', 'a'): 0.07142857142857142,
+            ('UK', 'z', 'b'): 0.2857142857142857
+        },
+        ('metric1', dt.date(2030, 4, 3)): {
+            ('UK', 'x', 'e'): 1.0,
+            ('UK', 'y', 'c'): 0.5714285714285714,
+            ('UK', 'y', 'd'): 0.7857142857142857,
+            ('UK', 'z', 'a'): 0.14285714285714285,
+            ('UK', 'z', 'b'): 0.3571428571428571
+        },
+        ('metric2', dt.date(2030, 4, 1)): {
+            ('UK', 'x', 'e'): 0.8571428571428571,
+            ('UK', 'y', 'c'): 0.42857142857142855,
+            ('UK', 'y', 'd'): 0.6428571428571428,
+            ('UK', 'z', 'a'): 0.0,
+            ('UK', 'z', 'b'): 0.21428571428571427
+        },
+        ('metric2', dt.date(2030, 4, 2)): {
+            ('UK', 'x', 'e'): 0.9285714285714285,
+            ('UK', 'y', 'c'): 0.5,
+            ('UK', 'y', 'd'): 0.7142857142857143,
+            ('UK', 'z', 'a'): 0.07142857142857142,
+            ('UK', 'z', 'b'): 0.2857142857142857
+        },
+        ('metric2', dt.date(2030, 4, 3)): {
+            ('UK', 'x', 'e'): 1.0,
+            ('UK', 'y', 'c'): 0.5714285714285714,
+            ('UK', 'y', 'd'): 0.7857142857142857,
+            ('UK', 'z', 'a'): 0.14285714285714285,
+            ('UK', 'z', 'b'): 0.35714285714285715
+        }
+    }
     assert data1.unstacked.to_dict() == dct
 
 
 def test_filter(data1):
-    df_index = pd.DataFrame({'country': ['UK'], 'region': ['x'], 'city': ['e']}).set_index(['country', 'region', 'city'])
-    dct = {'metric1': {('UK', 'x', 'e', dt.date(2030, 4, 1)): 0.8571428571428571,
-        ('UK', 'x', 'e', dt.date(2030, 4, 2)): 0.9285714285714285,
-        ('UK', 'x', 'e', dt.date(2030, 4, 3)): 1.0},
-        'metric2': {('UK', 'x', 'e', dt.date(2030, 4, 1)): 0.8571428571428571,
-        ('UK', 'x', 'e', dt.date(2030, 4, 2)): 0.9285714285714285,
-        ('UK', 'x', 'e', dt.date(2030, 4, 3)): 1.0}}
+    df_index = pd.DataFrame({'country': ['UK'], 'region': ['x'], 'city': ['e']}) \
+        .set_index(['country', 'region', 'city'])
+    dct = {
+        'metric1': {
+            ('UK', 'x', 'e', dt.date(2030, 4, 1)): 0.8571428571428571,
+            ('UK', 'x', 'e', dt.date(2030, 4, 2)): 0.9285714285714285,
+            ('UK', 'x', 'e', dt.date(2030, 4, 3)): 1.0
+        },
+        'metric2': {
+            ('UK', 'x', 'e', dt.date(2030, 4, 1)): 0.8571428571428571,
+            ('UK', 'x', 'e', dt.date(2030, 4, 2)): 0.9285714285714285,
+            ('UK', 'x', 'e', dt.date(2030, 4, 3)): 1.0
+        }
+    }
     assert data1.filter(df_index).to_dict() == dct
 
 
 def test_matrix(data1):
     matrix = np.array([[[0.85714286, 0.92857143, 1.        ],
         [0.42857143, 0.5       , 0.57142857],
         [0.64285714, 0.71428571, 0.78571429],
@@ -144,21 +178,25 @@
         [0.64285714, 0.71428571, 0.78571429],
         [0.        , 0.07142857, 0.14285714],
         [0.21428571, 0.28571429, 0.35714286]]])
     assert (matrix == np.round(data1.matrix, 8)).all()
 
 
 def test_assign(data1):
-    dct = {'bin': {('UK', 'x', 'e'): 0,
-        ('UK', 'y', 'c'): 1,
-        ('UK', 'y', 'd'): 0,
-        ('UK', 'z', 'a'): 1,
-        ('UK', 'z', 'b'): 0}}
-    assert data1.assign(np.array([0,1,0,1,0])).to_dict()
+    dct = {
+        'bin': {
+            ('UK', 'x', 'e'): 0,
+            ('UK', 'y', 'c'): 1,
+            ('UK', 'y', 'd'): 0,
+            ('UK', 'z', 'a'): 1,
+            ('UK', 'z', 'b'): 0
+        }
+    }
+    assert data1.assign(np.array([0, 1, 0, 1, 0])).to_dict()
 
 
 def test_dim_spec(data1):
     assert data1.dim_spec_columns == ['city', 'date']
 
 
 def test_all_spec(data1):
-    assert data1.all_spec_columns == ['city', 'date', 'metric1', 'metric2']
+    assert data1.all_spec_columns == ['city', 'date', 'metric1', 'metric2']
```

### Comparing `absplit-1.4.4/tests/test_ga.py` & `absplit-1.4.5/tests/test_ga.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 import pytest
-
 from absplit import ABSplit, Match, tutorials
 import pandas as pd
 import datetime as dt
 import numpy as np
 
+
 @pytest.fixture
 def df():
     # Build test data
     data_dct = {
         'date': [dt.date(2030, 4, 1) + dt.timedelta(days=x) for x in range(3)] * 5,
         'country': ['UK'] * 15,
         'region': [item for sublist in [[x]*6 for x in ['z', 'y']] for item in sublist] + ['x']*3,
         'city': [item for sublist in [[x]*3 for x in ['a', 'b', 'c', 'd', 'e']] for item in sublist],
         'metric1': np.arange(0, 15, 1),
         'metric2': np.arange(0, 150, 10)
     }
     return pd.DataFrame(data_dct)
 
+
 @pytest.fixture
 def kwargs():
-    return  {
+    return {
         'metrics': ['metric1', 'metric2'],
         'date_col': 'date',
         'splitting': 'city'
     }
 
+
 @pytest.fixture
 def ab(df, kwargs):
     # Initialise and run
     ab = ABSplit(
         df=df,
         size_penalty=0,
         **kwargs,
     )
     ab.run()
     return ab
 
+
 @pytest.fixture
 def results():
     data_dct1 = {
         'country': {0: 'UK', 1: 'UK', 2: 'UK', 3: 'UK', 4: 'UK'},
         'region': {0: 'x', 1: 'y', 2: 'y', 3: 'z', 4: 'z'},
         'city': {0: 'e', 1: 'c', 2: 'd', 3: 'a', 4: 'b'},
         'bin': {0: '1', 1: '0', 2: '0', 3: '1', 4: '1'}
@@ -51,35 +54,37 @@
         'city': {0: 'e', 1: 'c', 2: 'd', 3: 'a', 4: 'b'},
         'bin': {0: '0', 1: '1', 2: '1', 3: '0', 4: '0'}
     }
     df_data1 = pd.DataFrame(data_dct1)
     df_data2 = pd.DataFrame(data_dct2)
     return df_data1, df_data2
 
+
 def test_ab_results(ab, results):
     """GA output ab.results"""
     df_data1, df_data2 = results
     r1 = len(ab.results.reset_index().compare(df_data1)) == 0
     r2 = len(ab.results.reset_index().compare(df_data2)) == 0
     assert True in (r1, r2)
 
 
 @pytest.fixture
 def sample():
     # Generate sample dataframe
     data_dct = {
-        'date': [dt.date(2030,4,1) + dt.timedelta(days=x) for x in range(3)],
+        'date': [dt.date(2030, 4, 1) + dt.timedelta(days=x) for x in range(3)],
         'country': ['UK'] * 3,
         'region': ['w'] * 3,
         'city': ['f'] * 3,
         'metric1': [3, 6, 7],
         'metric2': [30, 45, 70]
     }
     return pd.DataFrame(data_dct)
 
+
 @pytest.fixture
 def m(df, sample, kwargs):
     # Initialise match and run
     m = Match(
         population=df,
         sample=sample,
         **kwargs
@@ -88,19 +93,21 @@
     return m
 
 
 def test_match_results(m):
     dct = {'bin': {('UK', 'w', 'f'): '0', ('UK', 'z', 'a'): '1', ('UK', 'z', 'b'): '1'}}
     assert m.results.to_dict() == dct
 
+
 @pytest.fixture
 def df2():
     df = tutorials.covid(test=True)
     return df[df['state'] == 'Alabama']
 
+
 def test_absplit_static(df2):
     df2 = df2[df2['date'] == '2022-04-17'].reset_index(drop=True).drop('date', axis=1)
     kwargs = {
         'metrics': ['cases', 'deaths'],
         'splitting': 'county',
     }
     ab = ABSplit(
@@ -135,14 +142,15 @@
     ab = ABSplit(
         df=df2,
         ga_params={'num_generations': 10, 'sol_per_pop': 10},
         **kwargs
     )
     ab.run()
 
+
 def test_absplit_splits(df2):
     kwargs = {
         'metrics': ['cases', 'deaths'],
         'splitting': 'county',
         'date_col': 'date'
     }
     ab = ABSplit(
@@ -165,29 +173,31 @@
         ga_params={'num_generations': 10, 'sol_per_pop': 10},
         cutoff_date='2021-10-01',
         splits=[.25, .25, .5],
         **kwargs
     )
     ab.run()
 
+
 def test_absplit_cutoff_fail(df2):
     kwargs = {
         'metrics': ['cases', 'deaths'],
         'splitting': 'county',
         'date_col': 'date'
     }
     with pytest.raises(ValueError):
-        ab = ABSplit(
+        _ = ABSplit(
             df=df2,
             ga_params={'num_generations': 10, 'sol_per_pop': 10},
             cutoff_date='2030-10-01',
             splits=[.25, .25, .5],
             **kwargs
         )
 
+
 def test_absplit_penalties(df2):
     kwargs = {
         'metrics': ['cases', 'deaths'],
         'splitting': 'county',
         'date_col': 'date'
     }
     ab = ABSplit(
@@ -195,8 +205,8 @@
         ga_params={'num_generations': 10, 'sol_per_pop': 10},
         metric_weights={'cases': 20},
         sum_penalty=1,
         size_penalty=1,
         splits=[.25, .25, .5],
         **kwargs
     )
-    ab.run()
+    ab.run()
```

### Comparing `absplit-1.4.4/PKG-INFO` & `absplit-1.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absplit
-Version: 1.4.4
+Version: 1.4.5
 Summary: Generates A/B/n test groups
 Keywords: absplit,a/b test,ab test,ab split,split,set formation,group formation
 Author-email: Cormac Rynne <cormac.ry@gmail.com>
 Requires-Python: <=3.11
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -16,31 +16,33 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: pygad==3.0.1
+Requires-Dist: pygad<=3.3.1
 Requires-Dist: scikit-learn
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: seaborn
 Project-URL: Home, https://github.com/cormac-rynne/absplit
 
 <a name="readme-top"></a>
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg" width="460" height="140">
 <h3><strong>ABSplit</strong></h3>
 Split your data into matching A/B/n groups
 
 ![license](https://img.shields.io/badge/License-MIT-blue.svg)
-![version](https://img.shields.io/badge/version-1.4.4-blue.svg)
+![version](https://img.shields.io/badge/version-1.4.5-blue.svg)
 ![version](https://img.shields.io/badge/python-3-orange.svg)
+[![Downloads](https://static.pepy.tech/badge/absplit)](https://pepy.tech/project/absplit)
+[![Downloads](https://static.pepy.tech/badge/absplit/month)](https://pepy.tech/project/absplit)
 
 </div>
 
 <details open>
   <summary>Table of Contents</summary>
   <ol>
     <li>
@@ -247,7 +249,8 @@
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
+
```

#### html2text {}

```diff
@@ -1,29 +1,32 @@
-Metadata-Version: 2.1 Name: absplit Version: 1.4.4 Summary: Generates A/B/
+Metadata-Version: 2.1 Name: absplit Version: 1.4.5 Summary: Generates A/B/
 n test groups Keywords: absplit,a/b test,ab test,ab split,split,set
 formation,group formation Author-email: Cormac Rynne
 gmail.com> Requires-Python: <=3.11 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Scientific/Engineering :: Information Analysis Classifier: Topic :: Scientific/
 Engineering :: Visualization Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Requires-Dist: pygad==3.0.1 Requires-Dist: scikit-
+Libraries :: Python Modules Requires-Dist: pygad<=3.3.1 Requires-Dist: scikit-
 learn Requires-Dist: numpy Requires-Dist: pandas Requires-Dist: seaborn
 Project-URL: Home, https://github.com/cormac-rynne/absplit
 [https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg]
                                ******** AABBSSpplliitt ********
  Split your data into matching A/B/n groups ![license](https://img.shields.io/
  badge/License-MIT-blue.svg) ![version](https://img.shields.io/badge/version-
- 1.4.4-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
+1.4.5-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg) [!
+[Downloads](https://static.pepy.tech/badge/absplit)](https://pepy.tech/project/
+absplit) [![Downloads](https://static.pepy.tech/badge/absplit/month)](https://
+                          pepy.tech/project/absplit)
 Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _C_a_l_c_u_l_a_t_i_o_n
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
           o _I_n_s_t_a_l_l_a_t_i_o_n
    3. _T_u_t_o_r_i_a_l_s
           o _D_o_ _i_t_ _y_o_u_r_s_e_l_f
```

