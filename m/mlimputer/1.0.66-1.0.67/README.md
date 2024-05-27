# Comparing `tmp/mlimputer-1.0.66-py3-none-any.whl.zip` & `tmp/mlimputer-1.0.67-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 13213 bytes, number of entries: 10
+Zip file size: 13228 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Jan-02 00:48 mlimputer/__init__.py
--rw-rw-rw-  2.0 fat     5174 b- defN 24-Jan-02 00:54 mlimputer/imputation.py
--rw-rw-rw-  2.0 fat     6482 b- defN 24-Apr-20 22:10 mlimputer/model_selection.py
+-rw-rw-rw-  2.0 fat     5192 b- defN 24-May-27 21:06 mlimputer/imputation.py
+-rw-rw-rw-  2.0 fat     6458 b- defN 24-May-27 21:09 mlimputer/model_selection.py
 -rw-rw-rw-  2.0 fat    21184 b- defN 24-Apr-20 22:05 mlimputer/models_imputation.py
 -rw-rw-rw-  2.0 fat     2801 b- defN 24-Apr-20 22:18 mlimputer/parameters.py
--rw-rw-rw-  2.0 fat     1090 b- defN 24-May-07 21:34 mlimputer-1.0.66.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     7038 b- defN 24-May-07 21:34 mlimputer-1.0.66.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 21:34 mlimputer-1.0.66.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-May-07 21:34 mlimputer-1.0.66.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      809 b- defN 24-May-07 21:34 mlimputer-1.0.66.dist-info/RECORD
-10 files, 44680 bytes uncompressed, 11833 bytes compressed:  73.5%
+-rw-rw-rw-  2.0 fat     1090 b- defN 24-May-27 21:11 mlimputer-1.0.67.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     7038 b- defN 24-May-27 21:11 mlimputer-1.0.67.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-27 21:11 mlimputer-1.0.67.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-May-27 21:11 mlimputer-1.0.67.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      809 b- defN 24-May-27 21:11 mlimputer-1.0.67.dist-info/RECORD
+10 files, 44674 bytes uncompressed, 11848 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: mlimputer/models_imputation.py
 Comment: 
 
 Filename: mlimputer/parameters.py
 Comment: 
 
-Filename: mlimputer-1.0.66.dist-info/LICENSE
+Filename: mlimputer-1.0.67.dist-info/LICENSE
 Comment: 
 
-Filename: mlimputer-1.0.66.dist-info/METADATA
+Filename: mlimputer-1.0.67.dist-info/METADATA
 Comment: 
 
-Filename: mlimputer-1.0.66.dist-info/WHEEL
+Filename: mlimputer-1.0.67.dist-info/WHEEL
 Comment: 
 
-Filename: mlimputer-1.0.66.dist-info/top_level.txt
+Filename: mlimputer-1.0.67.dist-info/top_level.txt
 Comment: 
 
-Filename: mlimputer-1.0.66.dist-info/RECORD
+Filename: mlimputer-1.0.67.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mlimputer/imputation.py

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 from tqdm import tqdm
-from atlantic.processing import AutoLabelEncoder
-from atlantic.imputation import AutoSimpleImputer
+from atlantic.processing.encoders import AutoLabelEncoder
+from atlantic.imputers.imputation import AutoSimpleImputer
 from mlimputer.parameters import imputer_parameters
 from mlimputer.model_selection import missing_report, imput_models
 
 parameters=imputer_parameters()
 
 class MLimputer:
     def __init__ (self,
```

## mlimputer/model_selection.py

```diff
@@ -1,9 +1,9 @@
-from atlantic.analysis import Analysis
-from atlantic.evaluation import Evaluation
+from atlantic.processing.analysis import Analysis
+from atlantic.optimizer.metrics import metrics_classification, metrics_regression
 from sklearn.model_selection import train_test_split
 import pandas as pd
 from mlimputer.models_imputation import (RandomForestImputation,
                                          ExtraTreesImputation,
                                          GBRImputation,
                                          KNNImputation,
                                          XGBoostImputation,
@@ -141,17 +141,17 @@
         for model in models:
             print(f"Fitting {model.__class__.__name__} model")
             model.fit(X_train, y_train)
             y_pred = model.predict(X_test)
             score = model.score(X_test, y_test)
             print(f"{model.__class__.__name__} model score: {round(score,4)}")
             if sv_pred == 'Class':
-                metrics = pd.DataFrame(Evaluation.metrics_classification(y_test,y_pred),index = [0])
+                metrics = metrics_classification(y_test,y_pred)
             elif sv_pred == 'Reg':
-                metrics = pd.DataFrame(Evaluation.metrics_regression(y_test,y_pred),index = [0])
+                metrics = metrics_regression(y_test,y_pred)
             metrics["model"] = model.__class__.__name__
             metrics["cv_folder"] = i+1
             metrics = metrics.reset_index(drop = True)
             list_metrics.append(metrics)
 
     leaderboard = pd.concat(list_metrics)
     leaderboard = leaderboard.reset_index(drop = True)
```

## Comparing `mlimputer-1.0.66.dist-info/LICENSE` & `mlimputer-1.0.67.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mlimputer-1.0.66.dist-info/METADATA` & `mlimputer-1.0.67.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlimputer
-Version: 1.0.66
+Version: 1.0.67
 Summary: MLimputer - Missing Data Imputation Framework for Supervised Machine Learning
 Home-page: https://github.com/TsLu1s/MLimputer
 Author: Luís Santos
 Author-email: luisf_ssantos@hotmail.com
 License: MIT
 Keywords: data science,machine learning,data preprecessing,null imputation,missing data imputation,predictive null imputation,multiple null imputation,automated machine learning
 Classifier: Intended Audience :: Education
@@ -20,15 +20,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scikit-learn (>=1.0.2)
-Requires-Dist: atlantic (>=1.1.25)
+Requires-Dist: atlantic (>=1.1.50)
 Requires-Dist: catboost (>=1.1.1)
 Requires-Dist: xgboost (>=1.7.3)
 Requires-Dist: lightgbm (>=3.3.5)
 
 <br>
 <p align="center">
   <h2 align="center"> MLimputer - Missing Data Imputation Framework for Supervised Machine Learning
```

## Comparing `mlimputer-1.0.66.dist-info/RECORD` & `mlimputer-1.0.67.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 mlimputer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mlimputer/imputation.py,sha256=ZKn907nYvO42fII-dGCcQzqlbPIonm3c2fAYJO74irQ,5174
-mlimputer/model_selection.py,sha256=CswNu3KBkmtynGewC4uTtBFCl1k3Qide9Y16Ec18iXk,6482
+mlimputer/imputation.py,sha256=ELCWXrfZ-kSkY1_7iHBUc6zQOXZ-zEH-Vty2I_4_h84,5192
+mlimputer/model_selection.py,sha256=qAZQL8E0HBTxDuUECQ27KrMl-AgjsFnNJJstpQKp-uE,6458
 mlimputer/models_imputation.py,sha256=A6tCTUyCJz80Ihii1UQjQBk1_W-tkFC4bW3rYGdKFwA,21184
 mlimputer/parameters.py,sha256=bj8vYDpndwYwK4iEVlXZYTTWRtQU9yPPhLO5IvpqUK4,2801
-mlimputer-1.0.66.dist-info/LICENSE,sha256=BMKwnVd_OgrW1_Ls-_WlfHpr-s7KFtcT6t9t9tfFk8g,1090
-mlimputer-1.0.66.dist-info/METADATA,sha256=gNDLnUusvk365vjQT46cZGiRHpxXA1iaV0n2BJv2NJk,7038
-mlimputer-1.0.66.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mlimputer-1.0.66.dist-info/top_level.txt,sha256=6qseujMDdh0A5GoDaKPU6kp9vnXciE1XKZIvz88dVzE,10
-mlimputer-1.0.66.dist-info/RECORD,,
+mlimputer-1.0.67.dist-info/LICENSE,sha256=BMKwnVd_OgrW1_Ls-_WlfHpr-s7KFtcT6t9t9tfFk8g,1090
+mlimputer-1.0.67.dist-info/METADATA,sha256=ucp-Vz_wet0eg2B55xmFDpn608DHbCGiyQkUZKR6TmU,7038
+mlimputer-1.0.67.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+mlimputer-1.0.67.dist-info/top_level.txt,sha256=6qseujMDdh0A5GoDaKPU6kp9vnXciE1XKZIvz88dVzE,10
+mlimputer-1.0.67.dist-info/RECORD,,
```

