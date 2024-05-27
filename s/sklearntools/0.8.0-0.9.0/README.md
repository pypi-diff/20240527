# Comparing `tmp/sklearntools-0.8.0.tar.gz` & `tmp/sklearntools-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearntools-0.8.0.tar", last modified: Wed May 22 05:23:21 2024, max compression
+gzip compressed data, was "sklearntools-0.9.0.tar", last modified: Mon May 27 01:19:30 2024, max compression
```

## Comparing `sklearntools-0.8.0.tar` & `sklearntools-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-22 05:23:21.641316 sklearntools-0.8.0/
--rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-22 05:23:21.640056 sklearntools-0.8.0/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      761 2024-05-21 10:29:01.000000 sklearntools-0.8.0/README.rst
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-22 05:23:21.643701 sklearntools-0.8.0/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)      882 2024-05-22 05:23:16.000000 sklearntools-0.8.0/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-22 05:23:21.633133 sklearntools-0.8.0/sklearntools/
--rw-r--r--   0 summy      (501) staff       (20)     8784 2024-05-22 05:21:10.000000 sklearntools-0.8.0/sklearntools/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-22 05:23:21.638610 sklearntools-0.8.0/sklearntools.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-22 05:23:21.000000 sklearntools-0.8.0/sklearntools.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      258 2024-05-22 05:23:21.000000 sklearntools-0.8.0/sklearntools.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-22 05:23:21.000000 sklearntools-0.8.0/sklearntools.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-22 05:23:21.000000 sklearntools-0.8.0/sklearntools.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)       32 2024-05-22 05:23:21.000000 sklearntools-0.8.0/sklearntools.egg-info/requires.txt
--rw-r--r--   0 summy      (501) staff       (20)       13 2024-05-22 05:23:21.000000 sklearntools-0.8.0/sklearntools.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 01:19:30.342853 sklearntools-0.9.0/
+-rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-27 01:19:30.342125 sklearntools-0.9.0/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      761 2024-05-21 10:29:01.000000 sklearntools-0.9.0/README.rst
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-27 01:19:30.343120 sklearntools-0.9.0/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)      882 2024-05-27 01:19:20.000000 sklearntools-0.9.0/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 01:19:30.335368 sklearntools-0.9.0/sklearntools/
+-rw-r--r--   0 summy      (501) staff       (20)     8796 2024-05-27 01:16:03.000000 sklearntools-0.9.0/sklearntools/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 01:19:30.341109 sklearntools-0.9.0/sklearntools.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-27 01:19:30.000000 sklearntools-0.9.0/sklearntools.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      258 2024-05-27 01:19:30.000000 sklearntools-0.9.0/sklearntools.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-27 01:19:30.000000 sklearntools-0.9.0/sklearntools.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-27 01:19:30.000000 sklearntools-0.9.0/sklearntools.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       32 2024-05-27 01:19:30.000000 sklearntools-0.9.0/sklearntools.egg-info/requires.txt
+-rw-r--r--   0 summy      (501) staff       (20)       13 2024-05-27 01:19:30.000000 sklearntools-0.9.0/sklearntools.egg-info/top_level.txt
```

### Comparing `sklearntools-0.8.0/PKG-INFO` & `sklearntools-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearntools
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tools of sklearn.
 Home-page: https://gitee.com/summry/sklearntools
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sklearn
 Platform: UNKNOWN
```

### Comparing `sklearntools-0.8.0/README.rst` & `sklearntools-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `sklearntools-0.8.0/setup.py` & `sklearntools-0.9.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 setup(
     name='sklearntools',
     packages=['sklearntools'],
     description="Tools of sklearn.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.8.0',
+    version='0.9.0',
     install_requires=[
         'joblib>=1.1.0',
         'scikit-learn>=1.0',
     ],
     url='https://gitee.com/summry/sklearntools',
     author='summy',
     author_email='xiazhongbiao@126.com',
```

### Comparing `sklearntools-0.8.0/sklearntools/__init__.py` & `sklearntools-0.9.0/sklearntools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 from sklearn.metrics import accuracy_score, mean_squared_error, root_mean_squared_error
 from logging import basicConfig, INFO, getLogger
 
 logger = getLogger(__name__)
 basicConfig(level=INFO, format='[%(asctime)s %(levelname)s] %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
 
 
-def train_evaluate(model, X_train, X_test, y_train, y_test, print=True, describe='准确率', return_predict=False, evaluate_func=accuracy_score):
+def train_evaluate(model, X_train, X_test, y_train, y_test, describe='准确率', verbose=True, return_predict=False, evaluate_func=accuracy_score):
 	"""Train and evaluate a model
 
 	Parameters
     ----------
 	model: Model
 	X_train:
 	X_test:
 	y_train:
 	y_test:
-	print:
+	verbose:
 	describe:
 	return_predict: whether return predictions
 	evaluate_func: accuracy_score, mean_squared_error, root_mean_squared_error etc.
 
 	Returns
     -------
     score or (score, predictions)
@@ -45,39 +45,39 @@
 	model.fit(X_train, y_train)
 	prediction = model.predict(X_test)
 	if 'classifier' == model._estimator_type:
 		evaluate_func = accuracy_score
 	else:
 		evaluate_func = evaluate_func or mean_squared_error
 	score = evaluate_func(y_test, prediction)
-	if print:
+	if verbose:
 		if evaluate_func == accuracy_score:
 			logger.info(f'{describe}: {score:.1%}')
 		else:
 			if '准确率' == describe:
 				if evaluate_func == mean_squared_error:
 					describe = 'MSE'
 				elif evaluate_func == root_mean_squared_error:
 					describe = 'RMSE'
 			logger.info(f'{describe}: {score:.2f}')
 	if return_predict:
 		return score, prediction
 	return score
 
 
-def train_evaluate_split(model, X, y, test_size=0.2, print=True, describe='准确率', return_predict=False, random_state=42, evaluate_func=accuracy_score):
+def train_evaluate_split(model, X, y, test_size=0.2, describe='准确率', verbose=True, return_predict=False, random_state=42, evaluate_func=accuracy_score):
 	"""Train and evaluate a model
 
 	Parameters
 	----------
 	model: Model
 	X:
 	y:
 	test_size:
-	print:
+	verbose:
 	describe:
 	return_predict: whether return predictions
 	random_state:
 	evaluate_func: accuracy_score, mean_squared_error, root_mean_squared_error etc.
 
 	Returns
 	-------
@@ -90,15 +90,15 @@
 	>>> from sklearntools import train_evaluate_split
 	>>> X, y = np.arange(20).reshape((10, 2)), range(10)
 	>>> model = RandomForestClassifier(n_estimators=837, bootstrap=False)
 	>>> train_evaluate_split(model, X, y, test_size=0.2)
 	0.88
 	"""
 	X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=test_size, random_state=random_state)
-	return train_evaluate(model, X_train, X_test, y_train, y_test, print, describe, return_predict, evaluate_func)
+	return train_evaluate(model, X_train, X_test, y_train, y_test, describe, verbose, return_predict, evaluate_func)
 
 
 def search_model_params(model_name, X_train, X_test, y_train, y_test, param_grid, result_num=5, iter_num=8):
 	"""
 	Train and evaluate a model
 
 	Parameters
@@ -215,23 +215,23 @@
 		if classifier:
 			logger.info(f'random_state: {random_state} \t score: {score:.2%}')
 		else:
 			logger.info(f'random_state: {random_state} \t score: {score}:4f')
 
 
 def _search_test_size(model, X, y, test_size, random_state, evaluate_func):
-	return test_size, train_evaluate_split(model, X, y, test_size, False, None, False, random_state, evaluate_func)
+	return test_size, train_evaluate_split(model, X, y, test_size, None, False, False, random_state, evaluate_func)
 
 
 def _search_random_state(model, X, y, test_size, random_state, evaluate_func):
-	return random_state, train_evaluate_split(model, X, y, test_size, False, None, False, random_state, evaluate_func)
+	return random_state, train_evaluate_split(model, X, y, test_size, None, False, False, random_state, evaluate_func)
 
 
 def _search_random_state2(model, X_train, X_test, y_train, y_test, random_state, evaluate_func):
-	return random_state, train_evaluate(model, X_train, X_test, y_train, y_test, False, None, False, evaluate_func)
+	return random_state, train_evaluate(model, X_train, X_test, y_train, y_test, None, False, False, evaluate_func)
 
 
 def _search_params(model_name, classifier, X_train, X_test, y_train, y_test, params):
 	model = model_name(**params)
 	model.fit(X_train, y_train)
 	score = model.score(X_test, y_test)
 	if not classifier:
```

### Comparing `sklearntools-0.8.0/sklearntools.egg-info/PKG-INFO` & `sklearntools-0.9.0/sklearntools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearntools
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tools of sklearn.
 Home-page: https://gitee.com/summry/sklearntools
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sklearn
 Platform: UNKNOWN
```

