# Comparing `tmp/featransform-0.9.16-py3-none-any.whl.zip` & `tmp/featransform-0.9.20-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 18589 bytes, number of entries: 18
+Zip file size: 18592 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat        2 b- defN 24-Apr-01 18:31 featransform/__init__.py
--rw-rw-rw-  2.0 fat    11351 b- defN 24-Apr-07 17:41 featransform/pipeline.py
+-rw-rw-rw-  2.0 fat    11362 b- defN 24-May-27 21:18 featransform/pipeline.py
 -rw-rw-rw-  2.0 fat        2 b- defN 24-Apr-01 18:31 featransform/configs/__init__.py
 -rw-rw-rw-  2.0 fat     2140 b- defN 24-Apr-01 18:31 featransform/configs/parameters.py
 -rw-rw-rw-  2.0 fat        2 b- defN 24-Apr-01 18:31 featransform/feature_engineering/__init__.py
 -rw-rw-rw-  2.0 fat     3574 b- defN 24-Apr-07 17:39 featransform/feature_engineering/anomalies.py
 -rw-rw-rw-  2.0 fat     3388 b- defN 24-Apr-07 17:39 featransform/feature_engineering/clustering.py
 -rw-rw-rw-  2.0 fat     4042 b- defN 24-Apr-07 17:39 featransform/feature_engineering/dimensionality.py
 -rw-rw-rw-  2.0 fat        2 b- defN 24-Apr-01 18:31 featransform/optimizer/__init__.py
--rw-rw-rw-  2.0 fat    11425 b- defN 24-Apr-07 17:40 featransform/optimizer/evaluator.py
--rw-rw-rw-  2.0 fat     5277 b- defN 24-Apr-07 17:40 featransform/optimizer/selector.py
+-rw-rw-rw-  2.0 fat    11436 b- defN 24-May-27 21:16 featransform/optimizer/evaluator.py
+-rw-rw-rw-  2.0 fat     5288 b- defN 24-May-27 21:16 featransform/optimizer/selector.py
 -rw-rw-rw-  2.0 fat        2 b- defN 24-Apr-01 18:31 featransform/processing/__init__.py
 -rw-rw-rw-  2.0 fat     3512 b- defN 24-Apr-01 20:48 featransform/processing/processor.py
--rw-rw-rw-  2.0 fat     1090 b- defN 24-Apr-19 22:15 featransform-0.9.16.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     7196 b- defN 24-Apr-19 22:15 featransform-0.9.16.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-19 22:15 featransform-0.9.16.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-19 22:15 featransform-0.9.16.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1617 b- defN 24-Apr-19 22:15 featransform-0.9.16.dist-info/RECORD
-18 files, 54727 bytes uncompressed, 15875 bytes compressed:  71.0%
+-rw-rw-rw-  2.0 fat     1090 b- defN 24-May-27 21:20 featransform-0.9.20.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     7196 b- defN 24-May-27 21:20 featransform-0.9.20.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-27 21:20 featransform-0.9.20.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-May-27 21:20 featransform-0.9.20.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1617 b- defN 24-May-27 21:20 featransform-0.9.20.dist-info/RECORD
+18 files, 54760 bytes uncompressed, 15878 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: featransform/processing/__init__.py
 Comment: 
 
 Filename: featransform/processing/processor.py
 Comment: 
 
-Filename: featransform-0.9.16.dist-info/LICENSE
+Filename: featransform-0.9.20.dist-info/LICENSE
 Comment: 
 
-Filename: featransform-0.9.16.dist-info/METADATA
+Filename: featransform-0.9.20.dist-info/METADATA
 Comment: 
 
-Filename: featransform-0.9.16.dist-info/WHEEL
+Filename: featransform-0.9.20.dist-info/WHEEL
 Comment: 
 
-Filename: featransform-0.9.16.dist-info/top_level.txt
+Filename: featransform-0.9.20.dist-info/top_level.txt
 Comment: 
 
-Filename: featransform-0.9.16.dist-info/RECORD
+Filename: featransform-0.9.20.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## featransform/pipeline.py

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import pandas as pd
-from atlantic.analysis import Analysis
+from atlantic.processing.analysis import Analysis
 from featransform.processing.processor import AutoLabelEncoder, AutoIterativeImputer
 from featransform.feature_engineering.anomalies import Anomaly_Engineering
 from featransform.feature_engineering.clustering import Clustering_Engineering
 from featransform.feature_engineering.dimensionality import PCAensemble
 from featransform.optimizer.evaluator import Evaluation
 from featransform.optimizer.selector import Selector
 from featransform.configs.parameters import configurations
```

## featransform/optimizer/evaluator.py

```diff
@@ -1,9 +1,9 @@
 import pandas as pd
-from atlantic.analysis import Analysis 
+from atlantic.processing.analysis import Analysis 
 from featransform.optimizer.selector import Selector
 from featransform.configs.parameters import configurations
 from sklearn.metrics import (mean_absolute_error,
                              mean_absolute_percentage_error,
                              mean_squared_error,
                              explained_variance_score,
                              max_error,
```

## featransform/optimizer/selector.py

```diff
@@ -1,9 +1,9 @@
 import pandas as pd
-from atlantic.analysis import Analysis
+from atlantic.processing.analysis import Analysis
 from featransform.configs.parameters import configurations
 from sklearn.preprocessing import LabelEncoder
 from catboost import CatBoostClassifier, CatBoostRegressor
 import xgboost as xgb
 
 sec_conf = configurations()
```

## Comparing `featransform-0.9.16.dist-info/LICENSE` & `featransform-0.9.20.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `featransform-0.9.16.dist-info/METADATA` & `featransform-0.9.20.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: featransform
-Version: 0.9.16
-Summary: Featransform is an automated feature engineering framework for supervised machine learning
+Version: 0.9.20
+Summary: Featransform is an automated feature engineering framework for Supervised Machine Learning
 Home-page: https://github.com/TsLu1s/Featransform
 Author: Luís Santos
 Author-email: luisf_ssantos@hotmail.com
 License: MIT
 Keywords: data science,machine learning,data processing,feature engineering,feature selection,feature construction,feature optimization,automated feature engineering,automated machine learning,predictive modeling
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
@@ -19,15 +19,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: atlantic (>=1.1.25)
+Requires-Dist: atlantic (>=1.1.50)
 Requires-Dist: catboost (>=1.2.2)
 Requires-Dist: pandas (>=1.2.0)
 Requires-Dist: numpy (>=1.19.5)
 Requires-Dist: scikit-learn (>=1.2.2)
 Requires-Dist: h2o (>=3.44.0.1)
 Requires-Dist: xgboost (>=1.7.3)
 Requires-Dist: optuna (>=2.10.1)
```

## Comparing `featransform-0.9.16.dist-info/RECORD` & `featransform-0.9.20.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 featransform/__init__.py,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-featransform/pipeline.py,sha256=xfY795suvNgl828yKturwnNN8kSc5_DshUiZW0ntia4,11351
+featransform/pipeline.py,sha256=3Jby7UptVfNdjmLs6aAC5M4YjbqNIo98YVJXTXFx46k,11362
 featransform/configs/__init__.py,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
 featransform/configs/parameters.py,sha256=QFj-tFzBo4EpVrMK-Id0WKWkNeT7GsNWrkxftNuzxhc,2140
 featransform/feature_engineering/__init__.py,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
 featransform/feature_engineering/anomalies.py,sha256=zRYZUJQHewVRZIiYEQKAemnjRelMHPZnxewaobxYMok,3574
 featransform/feature_engineering/clustering.py,sha256=Ypkdh__1eMk1uIOungD3qM1ozHFsaZIBxEV8aRK_bYs,3388
 featransform/feature_engineering/dimensionality.py,sha256=ZQBSHppc43BmQJyS3duyHaFTiiSW057cQxnM87aamFM,4042
 featransform/optimizer/__init__.py,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-featransform/optimizer/evaluator.py,sha256=lsj3pEexLig0XXmjJClsiUfu-n-4e2kflsyhA5W29dA,11425
-featransform/optimizer/selector.py,sha256=Zf8OccuTg1qe070letEn3GmJDawUzJLRIXCCSO5yOeI,5277
+featransform/optimizer/evaluator.py,sha256=HfoIghKsVI8pP6YEo1v8gBc2M_nOu0z4URjTYDctxU0,11436
+featransform/optimizer/selector.py,sha256=nESe-f22_P0CHQAB0yRBmIf5ktcQheB6RLzCkwWWe-s,5288
 featransform/processing/__init__.py,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
 featransform/processing/processor.py,sha256=_eVGVNOF3RiJEabRwrq3G1AxY0c21MAleYdtaw3xGT4,3512
-featransform-0.9.16.dist-info/LICENSE,sha256=VMXkEvDFBFiT1owkPDp8dUVbidhkemgBSzG9qsUhs54,1090
-featransform-0.9.16.dist-info/METADATA,sha256=6V63AuY2rYgsXfkXwwPvUZg0VNiz85PkYc7wa-fbiH4,7196
-featransform-0.9.16.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-featransform-0.9.16.dist-info/top_level.txt,sha256=nGf-wp6SDVDIawemhMuwByTbpGahhv92kQ1dQbRdYwo,13
-featransform-0.9.16.dist-info/RECORD,,
+featransform-0.9.20.dist-info/LICENSE,sha256=VMXkEvDFBFiT1owkPDp8dUVbidhkemgBSzG9qsUhs54,1090
+featransform-0.9.20.dist-info/METADATA,sha256=VKzG5BiKPTeDKmsyrXQuFAqAbNrLVtODPofwXZrCMxk,7196
+featransform-0.9.20.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+featransform-0.9.20.dist-info/top_level.txt,sha256=nGf-wp6SDVDIawemhMuwByTbpGahhv92kQ1dQbRdYwo,13
+featransform-0.9.20.dist-info/RECORD,,
```

