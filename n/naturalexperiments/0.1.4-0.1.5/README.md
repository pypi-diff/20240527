# Comparing `tmp/naturalexperiments-0.1.4.tar.gz` & `tmp/naturalexperiments-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naturalexperiments-0.1.4.tar", last modified: Sun May 26 10:55:59 2024, max compression
+gzip compressed data, was "naturalexperiments-0.1.5.tar", last modified: Sun May 26 23:40:21 2024, max compression
```

## Comparing `naturalexperiments-0.1.4.tar` & `naturalexperiments-0.1.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 10:55:59.358684 naturalexperiments-0.1.4/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1071 2024-05-22 20:16:39.000000 naturalexperiments-0.1.4/LICENSE
--rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-26 10:55:59.358456 naturalexperiments-0.1.4/PKG-INFO
--rw-r--r--   0 rtealwitter   (501) staff       (20)      101 2024-05-22 20:16:39.000000 naturalexperiments-0.1.4/README.md
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 10:55:59.348035 naturalexperiments-0.1.4/naturalexperiments/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      120 2024-05-24 16:16:52.000000 naturalexperiments-0.1.4/naturalexperiments/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)    12686 2024-05-24 20:59:08.000000 naturalexperiments-0.1.4/naturalexperiments/benchmark.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 10:55:59.348757 naturalexperiments-0.1.4/naturalexperiments/data/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      444 2024-05-25 15:10:16.000000 naturalexperiments-0.1.4/naturalexperiments/data/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 10:55:59.349009 naturalexperiments-0.1.4/naturalexperiments/data/acic/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     2267 2024-05-26 10:54:09.000000 naturalexperiments-0.1.4/naturalexperiments/data/acic/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 10:55:59.349319 naturalexperiments-0.1.4/naturalexperiments/data/ihdp/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1420 2024-05-25 15:07:51.000000 naturalexperiments-0.1.4/naturalexperiments/data/ihdp/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 10:55:59.349566 naturalexperiments-0.1.4/naturalexperiments/data/jobs/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1283 2024-05-25 15:30:03.000000 naturalexperiments-0.1.4/naturalexperiments/data/jobs/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 10:55:59.349920 naturalexperiments-0.1.4/naturalexperiments/data/news/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1436 2024-05-25 15:30:29.000000 naturalexperiments-0.1.4/naturalexperiments/data/news/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 10:55:59.350629 naturalexperiments-0.1.4/naturalexperiments/data/rorco/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     2253 2024-05-25 15:30:41.000000 naturalexperiments-0.1.4/naturalexperiments/data/rorco/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)    15535 2024-05-22 21:34:07.000000 naturalexperiments-0.1.4/naturalexperiments/data/rorco/rorco_preprocess.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 10:55:59.350955 naturalexperiments-0.1.4/naturalexperiments/data/twins/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1731 2024-05-25 15:08:21.000000 naturalexperiments-0.1.4/naturalexperiments/data/twins/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     6151 2024-05-24 13:47:10.000000 naturalexperiments-0.1.4/naturalexperiments/data_summary.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 10:55:59.354144 naturalexperiments-0.1.4/naturalexperiments/estimators/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1545 2024-05-26 10:26:15.000000 naturalexperiments-0.1.4/naturalexperiments/estimators/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      690 2024-05-24 20:42:56.000000 naturalexperiments-0.1.4/naturalexperiments/estimators/catenet.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      136 2024-05-22 20:42:14.000000 naturalexperiments-0.1.4/naturalexperiments/estimators/direct_difference.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      330 2024-05-22 20:42:14.000000 naturalexperiments-0.1.4/naturalexperiments/estimators/direct_prediction.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1750 2024-05-22 20:42:14.000000 naturalexperiments-0.1.4/naturalexperiments/estimators/double_double.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      629 2024-05-22 20:42:14.000000 naturalexperiments-0.1.4/naturalexperiments/estimators/doubly_robust.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      138 2024-05-22 20:42:14.000000 naturalexperiments-0.1.4/naturalexperiments/estimators/horvitz_thompson.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      234 2024-05-22 20:42:14.000000 naturalexperiments-0.1.4/naturalexperiments/estimators/learned_direct.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1419 2024-05-22 20:42:14.000000 naturalexperiments-0.1.4/naturalexperiments/estimators/off_policy.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      488 2024-05-22 20:42:14.000000 naturalexperiments-0.1.4/naturalexperiments/estimators/propensity_stratification.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      436 2024-05-22 20:42:14.000000 naturalexperiments-0.1.4/naturalexperiments/estimators/regression_discontinuity.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      872 2024-05-22 20:42:14.000000 naturalexperiments-0.1.4/naturalexperiments/estimators/tmle.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     3546 2024-05-24 13:44:37.000000 naturalexperiments-0.1.4/naturalexperiments/model.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     2185 2024-05-24 13:19:39.000000 naturalexperiments-0.1.4/naturalexperiments/utils.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 10:55:59.354306 naturalexperiments-0.1.4/naturalexperiments.egg-info/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-26 10:55:59.000000 naturalexperiments-0.1.4/naturalexperiments.egg-info/PKG-INFO
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1258 2024-05-26 10:55:59.000000 naturalexperiments-0.1.4/naturalexperiments.egg-info/SOURCES.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)        1 2024-05-26 10:55:59.000000 naturalexperiments-0.1.4/naturalexperiments.egg-info/dependency_links.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)       19 2024-05-26 10:55:59.000000 naturalexperiments-0.1.4/naturalexperiments.egg-info/top_level.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)       38 2024-05-26 10:55:59.358719 naturalexperiments-0.1.4/setup.cfg
--rw-r--r--   0 rtealwitter   (501) staff       (20)      719 2024-05-26 10:55:27.000000 naturalexperiments-0.1.4/setup.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 23:40:21.314527 naturalexperiments-0.1.5/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1071 2024-05-22 20:16:39.000000 naturalexperiments-0.1.5/LICENSE
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-26 23:40:21.314325 naturalexperiments-0.1.5/PKG-INFO
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      101 2024-05-22 20:16:39.000000 naturalexperiments-0.1.5/README.md
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 23:40:21.308286 naturalexperiments-0.1.5/naturalexperiments/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      120 2024-05-24 16:16:52.000000 naturalexperiments-0.1.5/naturalexperiments/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)    13121 2024-05-26 23:39:50.000000 naturalexperiments-0.1.5/naturalexperiments/benchmark.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 23:40:21.309084 naturalexperiments-0.1.5/naturalexperiments/data/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      444 2024-05-25 15:10:16.000000 naturalexperiments-0.1.5/naturalexperiments/data/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 23:40:21.309318 naturalexperiments-0.1.5/naturalexperiments/data/acic/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     2267 2024-05-26 10:54:09.000000 naturalexperiments-0.1.5/naturalexperiments/data/acic/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 23:40:21.309662 naturalexperiments-0.1.5/naturalexperiments/data/ihdp/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1420 2024-05-25 15:07:51.000000 naturalexperiments-0.1.5/naturalexperiments/data/ihdp/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 23:40:21.309905 naturalexperiments-0.1.5/naturalexperiments/data/jobs/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1283 2024-05-25 15:30:03.000000 naturalexperiments-0.1.5/naturalexperiments/data/jobs/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 23:40:21.310161 naturalexperiments-0.1.5/naturalexperiments/data/news/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1436 2024-05-25 15:30:29.000000 naturalexperiments-0.1.5/naturalexperiments/data/news/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 23:40:21.310742 naturalexperiments-0.1.5/naturalexperiments/data/rorco/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     2253 2024-05-25 15:30:41.000000 naturalexperiments-0.1.5/naturalexperiments/data/rorco/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)    15535 2024-05-22 21:34:07.000000 naturalexperiments-0.1.5/naturalexperiments/data/rorco/rorco_preprocess.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 23:40:21.311047 naturalexperiments-0.1.5/naturalexperiments/data/twins/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1731 2024-05-25 15:08:21.000000 naturalexperiments-0.1.5/naturalexperiments/data/twins/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     6151 2024-05-24 13:47:10.000000 naturalexperiments-0.1.5/naturalexperiments/data_summary.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 23:40:21.313925 naturalexperiments-0.1.5/naturalexperiments/estimators/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1545 2024-05-26 10:26:15.000000 naturalexperiments-0.1.5/naturalexperiments/estimators/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      690 2024-05-24 20:42:56.000000 naturalexperiments-0.1.5/naturalexperiments/estimators/catenet.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      136 2024-05-22 20:42:14.000000 naturalexperiments-0.1.5/naturalexperiments/estimators/direct_difference.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      330 2024-05-22 20:42:14.000000 naturalexperiments-0.1.5/naturalexperiments/estimators/direct_prediction.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1750 2024-05-22 20:42:14.000000 naturalexperiments-0.1.5/naturalexperiments/estimators/double_double.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      629 2024-05-22 20:42:14.000000 naturalexperiments-0.1.5/naturalexperiments/estimators/doubly_robust.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      138 2024-05-22 20:42:14.000000 naturalexperiments-0.1.5/naturalexperiments/estimators/horvitz_thompson.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      234 2024-05-22 20:42:14.000000 naturalexperiments-0.1.5/naturalexperiments/estimators/learned_direct.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1419 2024-05-22 20:42:14.000000 naturalexperiments-0.1.5/naturalexperiments/estimators/off_policy.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      488 2024-05-22 20:42:14.000000 naturalexperiments-0.1.5/naturalexperiments/estimators/propensity_stratification.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      436 2024-05-22 20:42:14.000000 naturalexperiments-0.1.5/naturalexperiments/estimators/regression_discontinuity.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      872 2024-05-22 20:42:14.000000 naturalexperiments-0.1.5/naturalexperiments/estimators/tmle.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     3546 2024-05-24 13:44:37.000000 naturalexperiments-0.1.5/naturalexperiments/model.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     2185 2024-05-24 13:19:39.000000 naturalexperiments-0.1.5/naturalexperiments/utils.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 23:40:21.314103 naturalexperiments-0.1.5/naturalexperiments.egg-info/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-26 23:40:21.000000 naturalexperiments-0.1.5/naturalexperiments.egg-info/PKG-INFO
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1258 2024-05-26 23:40:21.000000 naturalexperiments-0.1.5/naturalexperiments.egg-info/SOURCES.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)        1 2024-05-26 23:40:21.000000 naturalexperiments-0.1.5/naturalexperiments.egg-info/dependency_links.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)       19 2024-05-26 23:40:21.000000 naturalexperiments-0.1.5/naturalexperiments.egg-info/top_level.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)       38 2024-05-26 23:40:21.314585 naturalexperiments-0.1.5/setup.cfg
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      719 2024-05-26 23:40:13.000000 naturalexperiments-0.1.5/setup.py
```

### Comparing `naturalexperiments-0.1.4/LICENSE` & `naturalexperiments-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.4/PKG-INFO` & `naturalexperiments-0.1.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalexperiments
-Version: 0.1.4
+Version: 0.1.5
 Summary: Estimators and datasets for treatment effect estimation in natural experiments.
 Home-page: https://github.com/rtealwitter/naturalexperiments
 Author: R. Teal Witter
 Author-email: rtealwitter@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `naturalexperiments-0.1.4/naturalexperiments/benchmark.py` & `naturalexperiments-0.1.5/naturalexperiments/benchmark.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,14 +160,15 @@
         with open(filename, 'a') as f:
             f.write(str(saved) + '\n')
     
     
     output, times = {}, {}
     with open(filename, 'r') as f:
         for line in f:
+            if 'nan' in line: continue
             line = line.replace('Array(', '').replace(', dtype=float32)', '')
             saved = eval(line)
             for method in saved:
                 if method not in output:
                     output[method] = []
                     times[method] = []
                 output[method] += [float(saved[method][0])]
@@ -196,17 +197,19 @@
                 saved[method] = square_difference
             with open(filename, 'a') as f:
                 f.write(str(saved) + '\n')
     
     output = {}
     with open(filename, 'r') as f:
         for line in f:
+            if 'nan' in line: continue
             line = line.replace('Array(', '').replace(', dtype=float32)', '')
             saved = eval(line)
             for method in saved:
+                if method == 'n': continue
                 if method not in output:
                     output[method] = {}
                 n = saved['n']
                 if n not in output[method]:
                     output[method][n] = []
                 output[method][n] += [float(saved[method])]
 
@@ -242,17 +245,19 @@
                 saved[method] = square_difference
             with open(filename, 'a') as f:
                 f.write(str(saved) + '\n')
 
     output = {}
     with open(filename, 'r') as f:
         for line in f:
+            if 'nan' in line: continue
             line = line.replace('Array(', '').replace(', dtype=float32)', '')
             saved = eval(line)
             for method in saved:
+                if method == 'cross_entropy': continue
                 if method not in output:
                     output[method] = {}
                 cross_entropy = saved['cross_entropy']
                 if cross_entropy not in output[method]:
                     output[method][cross_entropy] = []
                 output[method][cross_entropy] += [float(saved[method])]
 
@@ -278,15 +283,20 @@
                 'y0' : (1-p) * (1-alpha) + random_vector * alpha,
                 'y1' : 1-biased_treatment_effect(p) * (1-alpha) + random_vector * alpha
             }, dtype=float)
 
             uniform = np.random.random_sample(X.shape[0])
             z = (uniform < p).astype(int)
 
-            correlation = (np.abs(np.corrcoef(y['y1'], p)[0,1]) + np.abs(np.corrcoef(y['y0'], p)[0,1]))/2
+            # Compute distance correlation between p and y1, y0
+
+            corr1 = compute_distance_correlation(p, y['y1'])
+            corr0 = compute_distance_correlation(p, y['y0'])
+
+            correlation = (corr1 + corr0) / 2
 
             correlation = np.round(correlation / increment) * increment
 
             p_estimated = estimate_propensity(X, z)
 
             true_effect = (y['y1'] - y['y0']).mean()
     
@@ -299,17 +309,19 @@
                 saved[method] = square_difference
             with open(filename, 'a') as f:
                 f.write(str(saved) + '\n')
     
     output = {}
     with open(filename, 'r') as f:
         for line in f:
+            if 'nan' in line: continue
             line = line.replace('Array(', '').replace(', dtype=float32)', '')
             saved = eval(line)
             for method in saved:
+                if method == 'correlation': continue
                 if method not in output:
                     output[method] = {}
                 correlation = saved['correlation']
                 if correlation not in output[method]:
                     output[method][correlation] = []
                 output[method][correlation] += [float(saved[method])]
```

### Comparing `naturalexperiments-0.1.4/naturalexperiments/data/acic/__init__.py` & `naturalexperiments-0.1.5/naturalexperiments/data/acic/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.4/naturalexperiments/data/ihdp/__init__.py` & `naturalexperiments-0.1.5/naturalexperiments/data/ihdp/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.4/naturalexperiments/data/jobs/__init__.py` & `naturalexperiments-0.1.5/naturalexperiments/data/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.4/naturalexperiments/data/news/__init__.py` & `naturalexperiments-0.1.5/naturalexperiments/data/news/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.4/naturalexperiments/data/rorco/__init__.py` & `naturalexperiments-0.1.5/naturalexperiments/data/rorco/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.4/naturalexperiments/data/rorco/rorco_preprocess.py` & `naturalexperiments-0.1.5/naturalexperiments/data/rorco/rorco_preprocess.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.4/naturalexperiments/data/twins/__init__.py` & `naturalexperiments-0.1.5/naturalexperiments/data/twins/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.4/naturalexperiments/data_summary.py` & `naturalexperiments-0.1.5/naturalexperiments/data_summary.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.4/naturalexperiments/estimators/__init__.py` & `naturalexperiments-0.1.5/naturalexperiments/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.4/naturalexperiments/estimators/catenet.py` & `naturalexperiments-0.1.5/naturalexperiments/estimators/catenet.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.4/naturalexperiments/estimators/double_double.py` & `naturalexperiments-0.1.5/naturalexperiments/estimators/double_double.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.4/naturalexperiments/estimators/doubly_robust.py` & `naturalexperiments-0.1.5/naturalexperiments/estimators/doubly_robust.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.4/naturalexperiments/estimators/off_policy.py` & `naturalexperiments-0.1.5/naturalexperiments/estimators/off_policy.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.4/naturalexperiments/estimators/tmle.py` & `naturalexperiments-0.1.5/naturalexperiments/estimators/tmle.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.4/naturalexperiments/model.py` & `naturalexperiments-0.1.5/naturalexperiments/model.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.4/naturalexperiments/utils.py` & `naturalexperiments-0.1.5/naturalexperiments/utils.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.4/naturalexperiments.egg-info/PKG-INFO` & `naturalexperiments-0.1.5/naturalexperiments.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalexperiments
-Version: 0.1.4
+Version: 0.1.5
 Summary: Estimators and datasets for treatment effect estimation in natural experiments.
 Home-page: https://github.com/rtealwitter/naturalexperiments
 Author: R. Teal Witter
 Author-email: rtealwitter@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `naturalexperiments-0.1.4/naturalexperiments.egg-info/SOURCES.txt` & `naturalexperiments-0.1.5/naturalexperiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.4/setup.py` & `naturalexperiments-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="naturalexperiments",
-    version="0.1.4",
+    version="0.1.5",
     author="R. Teal Witter",
     author_email="rtealwitter@gmail.com",
     description="Estimators and datasets for treatment effect estimation in natural experiments.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rtealwitter/naturalexperiments",
     packages=setuptools.find_packages(),
```

