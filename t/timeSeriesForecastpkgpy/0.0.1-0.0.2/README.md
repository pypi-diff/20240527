# Comparing `tmp/timeSeriesForecastpkgpy-0.0.1.tar.gz` & `tmp/timeSeriesForecastpkgpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/timeSeriesForecastpkgpy-0.0.1.tar", last modified: Sun May 26 01:19:15 2024, max compression
+gzip compressed data, was "dist/timeSeriesForecastpkgpy-0.0.2.tar", last modified: Mon May 27 15:22:46 2024, max compression
```

## Comparing `timeSeriesForecastpkgpy-0.0.1.tar` & `timeSeriesForecastpkgpy-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-05-26 01:19:15.474519 timeSeriesForecastpkgpy-0.0.1/
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      555 2024-05-26 01:19:15.474519 timeSeriesForecastpkgpy-0.0.1/PKG-INFO
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-05-26 01:19:15.470519 timeSeriesForecastpkgpy-0.0.1/pyTimeSeriesForecast/
--rw-rw-r--   0 miguel    (1000) miguel    (1000)       72 2024-05-26 01:16:25.000000 timeSeriesForecastpkgpy-0.0.1/pyTimeSeriesForecast/__init__.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     3863 2024-05-25 23:14:05.000000 timeSeriesForecastpkgpy-0.0.1/pyTimeSeriesForecast/data.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      845 2024-05-22 00:01:27.000000 timeSeriesForecastpkgpy-0.0.1/pyTimeSeriesForecast/dataPreProcessing.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     1768 2024-05-25 23:04:09.000000 timeSeriesForecastpkgpy-0.0.1/pyTimeSeriesForecast/dataVisualizing.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     2950 2024-05-26 01:16:10.000000 timeSeriesForecastpkgpy-0.0.1/pyTimeSeriesForecast/main.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     1569 2024-05-25 21:44:48.000000 timeSeriesForecastpkgpy-0.0.1/pyTimeSeriesForecast/metrics.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     3261 2024-05-25 23:12:34.000000 timeSeriesForecastpkgpy-0.0.1/pyTimeSeriesForecast/model.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)       38 2024-05-26 01:19:15.474519 timeSeriesForecastpkgpy-0.0.1/setup.cfg
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      789 2024-05-26 01:10:32.000000 timeSeriesForecastpkgpy-0.0.1/setup.py
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-05-26 01:19:15.474519 timeSeriesForecastpkgpy-0.0.1/timeSeriesForecastpkgpy.egg-info/
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      555 2024-05-26 01:19:14.000000 timeSeriesForecastpkgpy-0.0.1/timeSeriesForecastpkgpy.egg-info/PKG-INFO
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      477 2024-05-26 01:19:14.000000 timeSeriesForecastpkgpy-0.0.1/timeSeriesForecastpkgpy.egg-info/SOURCES.txt
--rw-rw-r--   0 miguel    (1000) miguel    (1000)        1 2024-05-26 01:19:14.000000 timeSeriesForecastpkgpy-0.0.1/timeSeriesForecastpkgpy.egg-info/dependency_links.txt
--rw-rw-r--   0 miguel    (1000) miguel    (1000)       62 2024-05-26 01:19:14.000000 timeSeriesForecastpkgpy-0.0.1/timeSeriesForecastpkgpy.egg-info/requires.txt
--rw-rw-r--   0 miguel    (1000) miguel    (1000)       21 2024-05-26 01:19:14.000000 timeSeriesForecastpkgpy-0.0.1/timeSeriesForecastpkgpy.egg-info/top_level.txt
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-05-27 15:22:46.994578 timeSeriesForecastpkgpy-0.0.2/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      553 2024-05-27 15:22:46.994578 timeSeriesForecastpkgpy-0.0.2/PKG-INFO
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-05-27 15:22:46.994578 timeSeriesForecastpkgpy-0.0.2/pyTimeSeriesForecast/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       72 2024-05-26 01:16:25.000000 timeSeriesForecastpkgpy-0.0.2/pyTimeSeriesForecast/__init__.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     3863 2024-05-25 23:14:05.000000 timeSeriesForecastpkgpy-0.0.2/pyTimeSeriesForecast/data.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      800 2024-05-27 03:56:00.000000 timeSeriesForecastpkgpy-0.0.2/pyTimeSeriesForecast/dataPreProcessing.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     2338 2024-05-27 03:39:05.000000 timeSeriesForecastpkgpy-0.0.2/pyTimeSeriesForecast/dataVisualizing.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     3621 2024-05-27 03:35:57.000000 timeSeriesForecastpkgpy-0.0.2/pyTimeSeriesForecast/main.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1570 2024-05-26 23:58:37.000000 timeSeriesForecastpkgpy-0.0.2/pyTimeSeriesForecast/metrics.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     3261 2024-05-25 23:12:34.000000 timeSeriesForecastpkgpy-0.0.2/pyTimeSeriesForecast/model.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       38 2024-05-27 15:22:46.994578 timeSeriesForecastpkgpy-0.0.2/setup.cfg
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      792 2024-05-27 15:21:49.000000 timeSeriesForecastpkgpy-0.0.2/setup.py
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-05-27 15:22:46.994578 timeSeriesForecastpkgpy-0.0.2/timeSeriesForecastpkgpy.egg-info/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      553 2024-05-27 15:22:46.000000 timeSeriesForecastpkgpy-0.0.2/timeSeriesForecastpkgpy.egg-info/PKG-INFO
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      477 2024-05-27 15:22:46.000000 timeSeriesForecastpkgpy-0.0.2/timeSeriesForecastpkgpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)        1 2024-05-27 15:22:46.000000 timeSeriesForecastpkgpy-0.0.2/timeSeriesForecastpkgpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       67 2024-05-27 15:22:46.000000 timeSeriesForecastpkgpy-0.0.2/timeSeriesForecastpkgpy.egg-info/requires.txt
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       21 2024-05-27 15:22:46.000000 timeSeriesForecastpkgpy-0.0.2/timeSeriesForecastpkgpy.egg-info/top_level.txt
```

### Comparing `timeSeriesForecastpkgpy-0.0.1/PKG-INFO` & `timeSeriesForecastpkgpy-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.1
 Name: timeSeriesForecastpkgpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package that supports forecasting tasks in python
 Home-page: UNKNOWN
 Author: Miguel Vuori
-Author-email: <mail@neuralnine.com>
+Author-email: <mfvuori@gmail.com>
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `timeSeriesForecastpkgpy-0.0.1/pyTimeSeriesForecast/data.py` & `timeSeriesForecastpkgpy-0.0.2/pyTimeSeriesForecast/data.py`

 * *Files identical despite different names*

### Comparing `timeSeriesForecastpkgpy-0.0.1/pyTimeSeriesForecast/dataPreProcessing.py` & `timeSeriesForecastpkgpy-0.0.2/pyTimeSeriesForecast/dataPreProcessing.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pandas as pd
-from sklearn.ensemble import IsolationForest
 
 # read teh file from input_path, process and save in the output_path
 # return a pandas df processed
 
 def readAndProcessData(input_path, output_path , file_name):
 
     df = pd.read_csv(input_path, header=0)
```

### Comparing `timeSeriesForecastpkgpy-0.0.1/pyTimeSeriesForecast/dataVisualizing.py` & `timeSeriesForecastpkgpy-0.0.2/pyTimeSeriesForecast/dataVisualizing.py`

 * *Files 18% similar despite different names*

```diff
@@ -59,8 +59,19 @@
 
 
     plt.plot(acf)
     plt.xlabel("Lags")
     plt.ylabel("Autocorrelation")
     plt.title("Autocorrelation Function (ACF)")
     plt.savefig('./images/' + file_name, bbox_inches='tight')
+    plt.show()
+
+# create plot to compare Holt and Naive model
+def compareHoltNaive(test_df, holt, naive, file_name):
+    fig, ax = plt.subplots(figsize=(12, 6))
+    
+    ax.plot(test_df.index, test_df.values, color="gray")
+    ax.plot(test_df.index, holt.predict(test_df), label="alpha="+str(holt.model.params['smoothing_level'])[:4]+", beta="+str(holt.model.params['smoothing_trend'])[:4], color='#ff7823')
+    ax.plot(test_df.index, len(test_df.values)*[naive.predict()], color="#3c763d")
+    plt.legend()
+    plt.savefig('./images/' + file_name, bbox_inches='tight')
     plt.show()
```

### Comparing `timeSeriesForecastpkgpy-0.0.1/pyTimeSeriesForecast/main.py` & `timeSeriesForecastpkgpy-0.0.2/pyTimeSeriesForecast/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     # create visualization
     dv.createLinePlotGroupByDay(ts.df, 'SolarPowerByDay.png')
     dv.createLinePlotGroupByMonth(ts.df, 'SolarPowerByMonth.png')
     dv.createLagPlots(ts.df, 'lagPlot.png')
 
     # holt model training
-    # split series in train and test
+    # split series in train and test with cross validation
     ts.trainTestSplit(0.9)
     smoothing_level_list = [i / 100.0 for i in range(1,10,2)]
     smoothing_trend_list = [i / 100.0 for i in range(1,10,2)]
     n_sets = 5
     holt_rmse_error_list = []
     holt_mape_error_list = []
     for smoothing_level in smoothing_level_list:
@@ -44,14 +44,15 @@
                 holt_mape_errors.append(metrics.evaluateMape(ts.df.loc[valid]['SolarPower'].tolist(),forecasts))
                 holt_rmse_errors.append(metrics.evaluateRmse(ts.df.loc[valid]['SolarPower'].tolist(),forecasts))
                 
             heapq.heappush(holt_mape_error_list, (sum(holt_mape_errors)/len(holt_mape_errors),smoothing_level, smoothing_trend))
             heapq.heappush(holt_rmse_error_list, (sum(holt_rmse_errors)/len(holt_rmse_errors),smoothing_level, smoothing_trend))
     
     # Naive approach
+    # split series in train and test with cross validation
     naive_mape_errors = []
     naive_rmse_errors = []
     ts.crossValidationSplit(n_sets)
     for train_index, test_index in ts.cross_validation_genarator:
         train = ts.df.index[train_index]
         valid = ts.df.index[test_index]
         model = Naive()
@@ -59,10 +60,28 @@
         forecasts = len(valid)*[model.predict()]
         metrics = EvaluationMetrics()
         naive_mape_errors.append(metrics.evaluateMape(ts.df.loc[valid]['SolarPower'].tolist(),np.array(forecasts)))
         naive_rmse_errors.append(metrics.evaluateRmse(ts.df.loc[valid]['SolarPower'].tolist(),np.array(forecasts)))
     
     naive_mape = (sum(naive_mape_errors)/len(naive_mape_errors))
     naive_rmse = (sum(naive_rmse_errors)/len(naive_rmse_errors))
+    best_holt = heapq.heappop(holt_rmse_error_list)
+    with open('./images/validationMetrics.csv', 'w') as f:
+        f.write('Model, RMSE, MAPE\n')
+        f.write(f'Naive, {naive_rmse},{naive_mape}\n')
+        f.write(f'Holt, {best_holt},{heapq.heappop(holt_mape_error_list)}\n')
+
+    model_holt = HoltWinters()
+    model_holt.train(ts.df.resample("D").sum(),optimized=False, smoothing_level= best_holt[1], smoothing_trend=best_holt[2])
+
+    model_naive = Naive()
+    model_naive.train(ts.df['SolarPower'].tolist()[-1])
+
+    dv.compareHoltNaive(ts.df_test, model_holt, model_naive, 'modelsForecasting.png')
+
+    
+
+
+
+    
 
-    print(naive_mape, naive_rmse)
 main()
```

### Comparing `timeSeriesForecastpkgpy-0.0.1/pyTimeSeriesForecast/metrics.py` & `timeSeriesForecastpkgpy-0.0.2/pyTimeSeriesForecast/metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         print(f"  Mean Squared Error (MSE): {mse}")
         print(f"  Root Mean Squared Error (RMSE): {rmse}")
         print(f"  Mean Absolute Error (MAE): {mae}")
         print(f"  Mean Absolute Percentage Error (MAPE): {mape:.2f}%")
 
     def save(self, path, file_name):
         with open(path+file_name+'.csv', 'w') as f:
-            f.write('Metric,Value\n')
+            f.write('Metric,Value,\n')
             if self.mse:
                 f.write(f'MSE,{self.mse}\n')
             if self.rmse:
                 f.write(f'RMSE,{self.rmse}\n')
             if self.mae:
                 f.write(f'MAE,{self.mae}\n')
             if self.mape:
```

### Comparing `timeSeriesForecastpkgpy-0.0.1/pyTimeSeriesForecast/model.py` & `timeSeriesForecastpkgpy-0.0.2/pyTimeSeriesForecast/model.py`

 * *Files identical despite different names*

### Comparing `timeSeriesForecastpkgpy-0.0.1/setup.py` & `timeSeriesForecastpkgpy-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'A package that supports forecasting tasks in python'
 
 # Setting up
 setup(
     name="timeSeriesForecastpkgpy",
     version=VERSION,
     author="Miguel Vuori",
-    author_email="<mail@neuralnine.com>",
+    author_email="<mfvuori@gmail.com>",
     description=DESCRIPTION,
     packages=find_packages(),
-    install_requires=['pandas', 'plotly', 'statsmodels', 'matplotlib', 'numpy', 'sklearn', 'tensorflow'],
+    install_requires=['pandas', 'plotly', 'statsmodels', 'matplotlib', 'numpy', 'scikit-learn', 'tensorflow'],
     keywords=['python'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `timeSeriesForecastpkgpy-0.0.1/timeSeriesForecastpkgpy.egg-info/PKG-INFO` & `timeSeriesForecastpkgpy-0.0.2/timeSeriesForecastpkgpy.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.1
 Name: timeSeriesForecastpkgpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package that supports forecasting tasks in python
 Home-page: UNKNOWN
 Author: Miguel Vuori
-Author-email: <mail@neuralnine.com>
+Author-email: <mfvuori@gmail.com>
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

