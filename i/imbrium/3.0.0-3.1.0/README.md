# Comparing `tmp/imbrium-3.0.0.tar.gz` & `tmp/imbrium-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imbrium-3.0.0.tar", last modified: Mon May 13 23:47:49 2024, max compression
+gzip compressed data, was "imbrium-3.1.0.tar", last modified: Mon May 27 00:33:58 2024, max compression
```

## Comparing `imbrium-3.0.0.tar` & `imbrium-3.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 23:47:49.841497 imbrium-3.0.0/
--rw-rw-rw-   0        0        0     2990 2024-05-13 01:00:22.000000 imbrium-3.0.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1096 2022-10-31 01:25:26.000000 imbrium-3.0.0/LICENSE
--rw-rw-rw-   0        0        0       58 2022-10-31 01:25:26.000000 imbrium-3.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0   102154 2024-05-13 23:47:49.825900 imbrium-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0   101412 2024-05-13 23:07:01.000000 imbrium-3.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 23:47:49.653997 imbrium-3.0.0/imbrium/
--rw-rw-rw-   0        0        0      245 2023-12-03 16:02:47.000000 imbrium-3.0.0/imbrium/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 23:47:49.716493 imbrium-3.0.0/imbrium/architectures/
--rw-rw-rw-   0        0        0        0 2023-09-24 18:43:43.000000 imbrium-3.0.0/imbrium/architectures/__init__.py
--rw-rw-rw-   0        0        0    54099 2024-05-13 22:58:17.000000 imbrium-3.0.0/imbrium/architectures/models.py
-drwxrwxrwx   0        0        0        0 2024-05-13 23:47:49.732121 imbrium-3.0.0/imbrium/blueprints/
--rw-rw-rw-   0        0        0        0 2022-10-31 01:25:26.000000 imbrium-3.0.0/imbrium/blueprints/__init__.py
--rw-rw-rw-   0        0        0     2375 2024-05-13 22:58:14.000000 imbrium-3.0.0/imbrium/blueprints/abstract_multivariate.py
--rw-rw-rw-   0        0        0     2247 2024-05-13 22:58:14.000000 imbrium-3.0.0/imbrium/blueprints/abstract_univariate.py
-drwxrwxrwx   0        0        0        0 2024-05-13 23:47:49.778998 imbrium-3.0.0/imbrium/predictors/
--rw-rw-rw-   0        0        0        0 2023-09-24 18:43:58.000000 imbrium-3.0.0/imbrium/predictors/__init__.py
--rw-rw-rw-   0        0        0    43757 2024-05-13 22:58:18.000000 imbrium-3.0.0/imbrium/predictors/multivarhybrid.py
--rw-rw-rw-   0        0        0    42043 2024-05-13 22:58:18.000000 imbrium-3.0.0/imbrium/predictors/multivarpure.py
--rw-rw-rw-   0        0        0    42846 2024-05-13 22:58:18.000000 imbrium-3.0.0/imbrium/predictors/univarhybrid.py
--rw-rw-rw-   0        0        0    41739 2024-05-13 22:58:18.000000 imbrium-3.0.0/imbrium/predictors/univarpure.py
-drwxrwxrwx   0        0        0        0 2024-05-13 23:47:49.810251 imbrium-3.0.0/imbrium/utils/
--rw-rw-rw-   0        0        0        0 2023-09-24 18:44:13.000000 imbrium-3.0.0/imbrium/utils/__init__.py
--rw-rw-rw-   0        0        0      726 2023-12-03 12:53:22.000000 imbrium-3.0.0/imbrium/utils/optimizer.py
--rw-rw-rw-   0        0        0    10924 2024-05-12 19:50:14.000000 imbrium-3.0.0/imbrium/utils/transformer.py
-drwxrwxrwx   0        0        0        0 2024-05-13 23:47:49.700871 imbrium-3.0.0/imbrium.egg-info/
--rw-rw-rw-   0        0        0   102154 2024-05-13 23:47:49.000000 imbrium-3.0.0/imbrium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      661 2024-05-13 23:47:49.000000 imbrium-3.0.0/imbrium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 23:47:49.000000 imbrium-3.0.0/imbrium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-13 23:47:49.000000 imbrium-3.0.0/imbrium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-13 23:47:49.000000 imbrium-3.0.0/imbrium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 23:47:49.841497 imbrium-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1142 2024-05-11 21:54:00.000000 imbrium-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 00:33:58.471729 imbrium-3.1.0/
+-rw-rw-rw-   0        0        0     3241 2024-05-26 18:59:07.000000 imbrium-3.1.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1096 2022-10-31 01:25:26.000000 imbrium-3.1.0/LICENSE
+-rw-rw-rw-   0        0        0       58 2022-10-31 01:25:26.000000 imbrium-3.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    49941 2024-05-27 00:33:58.471729 imbrium-3.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    49198 2024-05-26 17:15:13.000000 imbrium-3.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 00:33:58.315538 imbrium-3.1.0/imbrium/
+-rw-rw-rw-   0        0        0      245 2024-05-24 00:48:39.000000 imbrium-3.1.0/imbrium/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 00:33:58.362363 imbrium-3.1.0/imbrium/architectures/
+-rw-rw-rw-   0        0        0        0 2023-09-24 18:43:43.000000 imbrium-3.1.0/imbrium/architectures/__init__.py
+-rw-rw-rw-   0        0        0    54099 2024-05-26 18:57:58.000000 imbrium-3.1.0/imbrium/architectures/models.py
+drwxrwxrwx   0        0        0        0 2024-05-27 00:33:58.377984 imbrium-3.1.0/imbrium/blueprints/
+-rw-rw-rw-   0        0        0        0 2022-10-31 01:25:26.000000 imbrium-3.1.0/imbrium/blueprints/__init__.py
+-rw-rw-rw-   0        0        0     2493 2024-05-26 17:32:22.000000 imbrium-3.1.0/imbrium/blueprints/abstract_multivariate.py
+-rw-rw-rw-   0        0        0     2365 2024-05-26 17:52:06.000000 imbrium-3.1.0/imbrium/blueprints/abstract_univariate.py
+drwxrwxrwx   0        0        0        0 2024-05-27 00:33:58.424855 imbrium-3.1.0/imbrium/predictors/
+-rw-rw-rw-   0        0        0        0 2023-09-24 18:43:58.000000 imbrium-3.1.0/imbrium/predictors/__init__.py
+-rw-rw-rw-   0        0        0    45302 2024-05-26 18:57:58.000000 imbrium-3.1.0/imbrium/predictors/multivarhybrid.py
+-rw-rw-rw-   0        0        0    43739 2024-05-26 18:57:58.000000 imbrium-3.1.0/imbrium/predictors/multivarpure.py
+-rw-rw-rw-   0        0        0    44385 2024-05-26 18:57:58.000000 imbrium-3.1.0/imbrium/predictors/univarhybrid.py
+-rw-rw-rw-   0        0        0    43162 2024-05-26 18:57:58.000000 imbrium-3.1.0/imbrium/predictors/univarpure.py
+drwxrwxrwx   0        0        0        0 2024-05-27 00:33:58.440481 imbrium-3.1.0/imbrium/utils/
+-rw-rw-rw-   0        0        0        0 2023-09-24 18:44:13.000000 imbrium-3.1.0/imbrium/utils/__init__.py
+-rw-rw-rw-   0        0        0      800 2024-05-26 18:57:58.000000 imbrium-3.1.0/imbrium/utils/optimizer.py
+-rw-rw-rw-   0        0        0    11058 2024-05-26 18:56:15.000000 imbrium-3.1.0/imbrium/utils/transformer.py
+drwxrwxrwx   0        0        0        0 2024-05-27 00:33:58.346737 imbrium-3.1.0/imbrium.egg-info/
+-rw-rw-rw-   0        0        0    49941 2024-05-27 00:33:57.000000 imbrium-3.1.0/imbrium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      661 2024-05-27 00:33:57.000000 imbrium-3.1.0/imbrium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 00:33:57.000000 imbrium-3.1.0/imbrium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-27 00:33:57.000000 imbrium-3.1.0/imbrium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-27 00:33:57.000000 imbrium-3.1.0/imbrium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 00:33:58.471729 imbrium-3.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1152 2024-05-26 18:12:03.000000 imbrium-3.1.0/setup.py
```

### Comparing `imbrium-3.0.0/CHANGELOG.md` & `imbrium-3.1.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -85,26 +85,34 @@
 ### 2.0.0
 
 - adapted `keras`
 - removed internal hyperparameter tuning
 - removed encoder-decoder architectures
 - improved layer configuration via dictionary input
 - split data argument into target and feature numpy arrays
- 
+
 ### 2.0.1
 
-- fix: removed dead pandas imports 
+- fix: removed dead pandas imports
 - chore: added tensorflow as base requirement
- 
+
 ### 2.1.0
 
 - feat!: removed data preparation out of predictor class, sub_seq, steps_past, steps_future need now to be defined in each model method
   - allows for advanced hyper parameter tuning
 - fix: removed tensor board activation logic bug
 
 ### 3.0.0
 
 - chore!: changed from temp library keras_core to keras > 3.0.0
 - chore!: removed python 3.8 support to accomodate tensorflow and keras dependiencies
 - chore: increased major to 3.0.0 to align with keras major
 - feat: added evaluate_model method to test model performance on test data
-- refactor!: removed validation split from `fit_model`. Control validation and test split via evaluation_split and validation_split paramters in class variables 
+- refactor!: removed validation split from `fit_model`. Control validation and test split via evaluation_split and validation_split paramters in class variables
+
+### 3.1.0
+
+- feat: added optional `batch_size` paramter to `fit_model`
+- feat: added Tensor Board to `evaluate_model`
+- refactor!: train, test, validation split default change
+- chore: added pre-commit checks
+- refactor: added, improved typing
```

### Comparing `imbrium-3.0.0/LICENSE` & `imbrium-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imbrium-3.0.0/imbrium/architectures/models.py` & `imbrium-3.1.0/imbrium/architectures/models.py`

 * *Files identical despite different names*

### Comparing `imbrium-3.0.0/imbrium/blueprints/abstract_multivariate.py` & `imbrium-3.1.0/imbrium/blueprints/abstract_univariate.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 from abc import ABC, abstractmethod
 
-from numpy import array
+import numpy as np
 
 
-class MultiVariateMultiStep(ABC):
-    """Abstract class that defines the general blueprint of a multivariate
+class UniVariateMultiStep(ABC):
+    """Abstract class that defines the general blueprint of a univariate
     multistep prediction object.
     """
 
     @abstractmethod
     def __init__(
         self,
-        target: array = array([]),
-        features: array = array([]),
+        target: np.ndarray = np.array([]),
+        features: np.ndarray = np.array([]),
         evaluation_split: float = 0.2,
         validation_split: float = 0.2,
     ):
         pass
 
     def _model_intake_prep(self, steps_past: int, steps_future: int) -> None:
         pass
 
     @abstractmethod
     def set_model_id(self, name: str):
         pass
 
     @property
     @abstractmethod
-    def get_target(self) -> array:
+    def get_target(self) -> np.ndarray:
         pass
 
     @property
     @abstractmethod
-    def get_target_shape(self) -> array:
+    def get_target_shape(self) -> np.ndarray:
         pass
 
     @property
     @abstractmethod
     def get_model_id(self) -> str:
         pass
 
     @property
     @abstractmethod
-    def get_X_input(self) -> array:
+    def get_X_input(self) -> np.ndarray:
         pass
 
     @property
     @abstractmethod
     def get_X_input_shape(self) -> tuple:
         pass
 
     @property
     @abstractmethod
-    def get_y_input(self) -> array:
+    def get_y_input(self) -> np.ndarray:
         pass
 
     @property
     @abstractmethod
     def get_y_input_shape(self) -> tuple:
         pass
 
@@ -75,22 +75,24 @@
     def get_metrics(self) -> str:
         pass
 
     @abstractmethod
     def fit_model(
         self,
         epochs: int,
+        board: bool = False,
+        batch_size=None,
         show_progress: int = 1,
         validation_split: float = 0.20,
         **callback_setting: dict
     ):
         pass
 
     @abstractmethod
-    def evaluate_model(self):
+    def evaluate_model(self, board: bool = False):
         pass
 
     @abstractmethod
     def model_blueprint(self):
         pass
 
     @abstractmethod
@@ -98,21 +100,15 @@
         pass
 
     @abstractmethod
     def show_evaluation(self):
         pass
 
     @abstractmethod
-    def predict(
-        self,
-        data: array,
-        sub_seq: int = None,
-        steps_past: int = None,
-        steps_future: int = None,
-    ) -> array:
+    def predict(self, data: np.ndarray) -> np.ndarray:
         pass
 
     @abstractmethod
     def freeze(self, absolute_path: str):
         pass
 
     @abstractmethod
```

### Comparing `imbrium-3.0.0/imbrium/blueprints/abstract_univariate.py` & `imbrium-3.1.0/imbrium/blueprints/abstract_multivariate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 from abc import ABC, abstractmethod
 
-from numpy import array
+import numpy as np
 
 
-class UniVariateMultiStep(ABC):
-    """Abstract class that defines the general blueprint of a univariate
+class MultiVariateMultiStep(ABC):
+    """Abstract class that defines the general blueprint of a multivariate
     multistep prediction object.
     """
 
     @abstractmethod
     def __init__(
         self,
-        target: array = array([]),
-        features: array = array([]),
+        target: np.ndarray = np.array([]),
+        features: np.ndarray = np.array([]),
         evaluation_split: float = 0.2,
         validation_split: float = 0.2,
     ):
         pass
 
     def _model_intake_prep(self, steps_past: int, steps_future: int) -> None:
         pass
 
     @abstractmethod
     def set_model_id(self, name: str):
         pass
 
     @property
     @abstractmethod
-    def get_target(self) -> array:
+    def get_target(self) -> np.ndarray:
         pass
 
     @property
     @abstractmethod
-    def get_target_shape(self) -> array:
+    def get_target_shape(self) -> np.ndarray:
         pass
 
     @property
     @abstractmethod
     def get_model_id(self) -> str:
         pass
 
     @property
     @abstractmethod
-    def get_X_input(self) -> array:
+    def get_X_input(self) -> np.ndarray:
         pass
 
     @property
     @abstractmethod
     def get_X_input_shape(self) -> tuple:
         pass
 
     @property
     @abstractmethod
-    def get_y_input(self) -> array:
+    def get_y_input(self) -> np.ndarray:
         pass
 
     @property
     @abstractmethod
     def get_y_input_shape(self) -> tuple:
         pass
 
@@ -75,22 +75,24 @@
     def get_metrics(self) -> str:
         pass
 
     @abstractmethod
     def fit_model(
         self,
         epochs: int,
+        board: bool = False,
+        batch_size=None,
         show_progress: int = 1,
         validation_split: float = 0.20,
         **callback_setting: dict
     ):
         pass
 
     @abstractmethod
-    def evaluate_model(self):
+    def evaluate_model(self, board: bool = False):
         pass
 
     @abstractmethod
     def model_blueprint(self):
         pass
 
     @abstractmethod
@@ -98,15 +100,21 @@
         pass
 
     @abstractmethod
     def show_evaluation(self):
         pass
 
     @abstractmethod
-    def predict(self, data: array) -> array:
+    def predict(
+        self,
+        data: np.ndarray,
+        sub_seq: int = None,
+        steps_past: int = None,
+        steps_future: int = None,
+    ) -> np.ndarray:
         pass
 
     @abstractmethod
     def freeze(self, absolute_path: str):
         pass
 
     @abstractmethod
```

### Comparing `imbrium-3.0.0/imbrium/predictors/multivarhybrid.py` & `imbrium-3.1.0/imbrium/predictors/multivarhybrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
 import os
+from typing import Any
 
+import numpy as np
 from keras.callbacks import EarlyStopping, TensorBoard
 from keras.saving import load_model
-from numpy import array
 
 from imbrium.architectures.models import (cnnbigru, cnnbilstm, cnnbirnn,
                                           cnngru, cnnlstm, cnnrnn)
 from imbrium.blueprints.abstract_multivariate import MultiVariateMultiStep
 from imbrium.utils.optimizer import get_optimizer
 from imbrium.utils.transformer import (data_prep_multi, multistep_prep_hybrid,
                                        train_test_split)
@@ -16,18 +17,18 @@
 class BaseHybridMulti(MultiVariateMultiStep):
     """Implements neural network based multivariate multipstep hybrid predictors."""
 
     CURRENT_PATH = os.getcwd()
 
     def __init__(
         self,
-        target: array = array([]),
-        features: array = array([]),
-        evaluation_split: float = 0.20,
-        validation_split: float = 0.20,
+        target: np.ndarray = np.array([]),
+        features: np.ndarray = np.array([]),
+        evaluation_split: float = 0.10,  # train: 90%, test: 10%
+        validation_split: float = 0.20,  # train: 72%, test: 10%, val: 18%
     ) -> object:
         """
         Parameters:
             target (array): Input target array.
             features (array): Input feature array.
             evaluation_split (float): train test split.
             validation_split (float): validation size of train set.
@@ -58,53 +59,53 @@
             )
             self.input_y, self.input_y_test = train_test_split(
                 self.input_y, test_size=self.evaluation_split
             )
         else:
             pass
 
-    def set_model_id(self, name: str):
+    def set_model_id(self, name: str) -> None:
         """Setter method to change model id field.
         Parameters:
             name (str): Name for selected Model.
         """
         self.model_id = name
 
     @property
     def get_model_id(self) -> str:
         """Get model id."""
         return self.model_id
 
     @property
-    def get_target(self) -> array:
+    def get_target(self) -> np.ndarray:
         """Get original target data."""
         return self.target
 
     @property
-    def get_target_shape(self) -> array:
+    def get_target_shape(self) -> np.ndarray:
         """Get shape of original target data."""
         return self.target.shape
 
     @property
-    def get_X_input(self) -> array:
+    def get_X_input(self) -> np.ndarray:
         """Get transformed feature data."""
         return self.input_x
 
     @property
-    def get_X_input_shape(self) -> tuple:
+    def get_X_input_shape(self) -> tuple[int, int]:
         """Get shape fo transformed feature data."""
         return self.input_x.shape
 
     @property
-    def get_y_input(self) -> array:
+    def get_y_input(self) -> np.ndarray:
         """Get transformed target data."""
         return self.input_y
 
     @property
-    def get_y_input_shape(self) -> tuple:
+    def get_y_input_shape(self) -> tuple[int, int]:
         """Get shape fo transformed target data."""
         return self.input_y.shape
 
     @property
     def get_optimizer(self) -> str:
         """Get model optimizer."""
         return self.optimizer
@@ -168,15 +169,15 @@
                 "config": {
                     "neurons": 32,
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
-    ):
+    ) -> None:
         """Creates CNN-RNN hybrid model.
         Parameters:
             sub_seq (int): Divide data into further subsequences.
             steps_past (int): Steps predictor will look backward.
             steps_future (int): Steps predictor will look forward.
             optimizer (str): Optimization algorithm.
             optimizer_args (dict): Arguments for optimizer.
@@ -263,15 +264,15 @@
                 "config": {
                     "neurons": 32,
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
-    ):
+    ) -> None:
         """Creates CNN-LSTM hybrid model.
         Parameters:
             sub_seq (int): Divide data into further subsequences.
             steps_past (int): Steps predictor will look backward.
             steps_future (int): Steps predictor will look forward.
             optimizer (str): Optimization algorithm.
             optimizer_args (dict): Arguments for optimizer.
@@ -358,15 +359,15 @@
                 "config": {
                     "neurons": 32,
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
-    ):
+    ) -> None:
         """Creates CNN-GRU hybrid model.
         Parameters:
             sub_seq (int): Divide data into further subsequences.
             steps_past (int): Steps predictor will look backward.
             steps_future (int): Steps predictor will look forward.
             optimizer (str): Optimization algorithm.
             optimizer_args (dict): Arguments for optimizer.
@@ -453,15 +454,15 @@
                 "config": {
                     "neurons": 32,
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
-    ):
+    ) -> None:
         """Creates CNN-BI-RNN hybrid model.
         Parameters:
             sub_seq (int): Divide data into further subsequences.
             steps_past (int): Steps predictor will look backward.
             steps_future (int): Steps predictor will look forward.
             optimizer (str): Optimization algorithm.
             optimizer_args (dict): Arguments for optimizer.
@@ -548,15 +549,15 @@
                 "config": {
                     "neurons": 32,
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
-    ):
+    ) -> None:
         """Creates CNN-BI-LSTM hybrid model.
         Parameters:
             sub_seq (int): Divide data into further subsequences.
             steps_past (int): Steps predictor will look backward.
             steps_future (int): Steps predictor will look forward.
             optimizer (str): Optimization algorithm.
             optimizer_args (dict): Arguments for optimizer.
@@ -643,15 +644,15 @@
                 "config": {
                     "neurons": 32,
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
-    ):
+    ) -> None:
         """Creates CNN-BI-GRU hybrid model.
         Parameters:
             sub_seq (int): Divide data into further subsequences.
             steps_past (int): Steps predictor will look backward.
             steps_future (int): Steps predictor will look forward.
             optimizer (str): Optimization algorithm.
             optimizer_args (dict): Arguments for optimizer.
@@ -690,21 +691,23 @@
         )
 
     def fit_model(
         self,
         epochs: int,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
-    ):
+    ) -> Any:
         """Trains the model on data provided. Perfroms validation.
         Parameters:
             epochs (int): Number of epochs to train the model.
             show_progress (int): Prints training progress.
             board (bool): Creates TensorBoard.
+            batch_size (float): Create Batch size.
             callback_settings (dict): Create a Keras EarlyStopping object.
         """
         if callback_setting == {}:
             if board == True:
                 callback_board = TensorBoard(
                     log_dir="logs/fit/"
                     + self.model_id
@@ -715,23 +718,25 @@
                     self.input_x,
                     self.input_y,
                     validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     callbacks=[callback_board],
                     shuffle=False,
+                    batch_size=batch_size,
                 )
             else:
                 self.details = self.model.fit(
                     self.input_x,
                     self.input_y,
                     validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     shuffle=False,
+                    batch_size=batch_size,
                 )
 
         else:
             if board == True:
                 callback_board = TensorBoard(
                     log_dir="logs/fit/"
                     + self.model_id
@@ -743,54 +748,72 @@
                     self.input_x,
                     self.input_y,
                     validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     callbacks=[callback, callback_board],
                     shuffle=False,
+                    batch_size=batch_size,
                 )
             else:
                 callback = EarlyStopping(**callback_setting)
                 self.details = self.model.fit(
                     self.input_x,
                     self.input_y,
                     validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     callbacks=[callback],
                     shuffle=False,
+                    batch_size=batch_size,
                 )
         return self.details
 
-    def evaluate_model(self):
-        self.evaluation_details = self.model.evaluate(
-            x=self.input_x_test, y=self.input_y_test
-        )
+    def evaluate_model(self, board: bool = False) -> Any:
+        """Evaluate model on test set.
+        Parameters:
+            board (bool): Create TensorBoard.
+        """
+        if board == True:
+            callback_board = TensorBoard(
+                log_dir="logs/eval/"
+                + self.model_id
+                + datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S"),
+                histogram_freq=1,
+            )
+            self.evaluation_details = self.model.evaluate(
+                x=self.input_x_test, y=self.input_y_test, callbacks=[callback_board]
+            )
+        else:
+            self.evaluation_details = self.model.evaluate(
+                x=self.input_x_test,
+                y=self.input_y_test,
+            )
 
         return self.evaluation_details
 
-    def model_blueprint(self):
+    def model_blueprint(self) -> Any:
         """Prints a summary of the models layer structure."""
         self.model.summary()
 
-    def show_performance(self):
+    def show_performance(self) -> Any:
         """Returns performance details."""
         return self.details
 
-    def show_evaluation(self):
+    def show_evaluation(self) -> Any:
         """Returns performance details on test data."""
         return self.evaluation_details
 
     def predict(
         self,
-        data: array,
+        data: np.ndarray,
         sub_seq: int = None,
         steps_past: int = None,
         steps_future: int = None,
-    ) -> array:
+    ) -> np.ndarray:
         """Takes in a sequence of values and outputs a forecast.
         Parameters:
             data (array): Input sequence which needs to be forecasted.
         Returns:
             (array): Forecast for sequence provided.
         """
         if sub_seq != None:
@@ -805,22 +828,22 @@
 
         y_pred = self.model.predict(data, verbose=0)
 
         y_pred = y_pred.reshape(y_pred.shape[1], y_pred.shape[0])
 
         return y_pred
 
-    def freeze(self, absolute_path: str = CURRENT_PATH):
+    def freeze(self, absolute_path: str = CURRENT_PATH) -> None:
         """Save the current model to the current directory.
         Parameters:
            absolute_path (str): Path to save model to.
         """
         self.model.save(absolute_path)
 
-    def retrieve(self, location: str):
+    def retrieve(self, location: str) -> None:
         """Load a keras model from the path specified.
         Parameters:
             location (str): Path of keras model location.
         """
         self.model = load_model(location)
 
 
@@ -877,16 +900,17 @@
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
-    ):
+    ) -> float:
         """Creates CNN-RNN hybrid model."""
         self.create_cnnrnn(
             sub_seq=sub_seq,
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
             optimizer_args=optimizer_args,
@@ -898,14 +922,15 @@
             rnn_block_two=rnn_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnlstm(
         self,
         sub_seq: int,
@@ -958,16 +983,17 @@
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
-    ):
+    ) -> float:
         """Creates CNN-LSTM hybrid model."""
         self.create_cnnlstm(
             sub_seq=sub_seq,
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
             optimizer_args=optimizer_args,
@@ -979,14 +1005,15 @@
             lstm_block_two=lstm_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnngru(
         self,
         sub_seq: int,
@@ -1039,16 +1066,17 @@
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
-    ):
+    ) -> float:
         """Creates CNN-GRU hybrid model."""
         self.create_cnngru(
             sub_seq=sub_seq,
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
             optimizer_args=optimizer_args,
@@ -1060,14 +1088,15 @@
             gru_block_two=gru_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnbirnn(
         self,
         sub_seq: int,
@@ -1120,16 +1149,17 @@
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
-    ):
+    ) -> float:
         """Creates CNN-BiRNN hybrid model."""
         self.create_cnnbirnn(
             sub_seq=sub_seq,
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
             optimizer_args=optimizer_args,
@@ -1141,14 +1171,15 @@
             rnn_block_one=rnn_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnbilstm(
         self,
         sub_seq: int,
@@ -1201,16 +1232,17 @@
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
-    ):
+    ) -> float:
         """Creates CNN-BiLSTM hybrid model."""
         self.create_cnnbilstm(
             sub_seq=sub_seq,
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
             optimizer_args=optimizer_args,
@@ -1222,14 +1254,15 @@
             lstm_block_one=lstm_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnbigru(
         self,
         sub_seq: int,
@@ -1282,16 +1315,17 @@
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
-    ):
+    ) -> float:
         """Creates CNN-BiGRU hybrid model."""
         self.create_cnnbigru(
             sub_seq=sub_seq,
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
             optimizer_args=optimizer_args,
@@ -1303,13 +1337,14 @@
             gru_block_one=gru_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
 
 __all__ = ["HybridMulti"]
```

### Comparing `imbrium-3.0.0/imbrium/predictors/multivarpure.py` & `imbrium-3.1.0/imbrium/predictors/multivarpure.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
 import os
+from typing import Any
 
+import numpy as np
 from keras.callbacks import EarlyStopping, TensorBoard
 from keras.saving import load_model
-from numpy import array
 
 from imbrium.architectures.models import (bigru, bilstm, birnn, cnn, gru, lstm,
                                           mlp, rnn)
 from imbrium.blueprints.abstract_multivariate import MultiVariateMultiStep
 from imbrium.utils.optimizer import get_optimizer
 from imbrium.utils.transformer import (data_prep_multi,
                                        multistep_prep_standard,
@@ -18,18 +19,18 @@
     """Implements deep neural networks based on multivariate multipstep
     standard predictors."""
 
     CURRENT_PATH = os.getcwd()
 
     def __init__(
         self,
-        target: array = array([]),
-        features: array = array([]),
-        evaluation_split: float = 0.20,
-        validation_split: float = 0.20,
+        target: np.ndarray = np.array([]),
+        features: np.ndarray = np.array([]),
+        evaluation_split: float = 0.10,  # train: 90%, test: 10%
+        validation_split: float = 0.20,  # train: 72%, test: 10%, val: 18%
     ) -> object:
         """
         Parameters:
             target (array): Input target data numpy array.
             features (array): Input feature data numpy array.
             evaluation_split (float): train test split.
             validation_split (float): validation size of train set.
@@ -55,53 +56,53 @@
             )
             self.input_y, self.input_y_test = train_test_split(
                 self.input_y, test_size=self.evaluation_split
             )
         else:
             pass
 
-    def set_model_id(self, name: str):
+    def set_model_id(self, name: str) -> None:
         """Setter method to change model id field.
         Parameters:
             name (str): Name for selected Model.
         """
         self.model_id = name
 
     @property
     def get_model_id(self) -> str:
         """Get model id."""
         return self.model_id
 
     @property
-    def get_target(self) -> array:
+    def get_target(self) -> np.ndarray:
         """Get original target data."""
         return self.target
 
     @property
-    def get_target_shape(self) -> array:
+    def get_target_shape(self) -> np.ndarray:
         """Get shape of original target data."""
         return self.target.shape
 
     @property
-    def get_X_input(self) -> array:
+    def get_X_input(self) -> np.ndarray:
         """Get transformed feature data."""
         return self.input_x
 
     @property
-    def get_X_input_shape(self) -> tuple:
+    def get_X_input_shape(self) -> tuple[int, int]:
         """Get shape fo transformed feature data."""
         return self.input_x.shape
 
     @property
-    def get_y_input(self) -> array:
+    def get_y_input(self) -> np.ndarray:
         """Get transformed target data."""
         return self.input_y
 
     @property
-    def get_y_input_shape(self) -> tuple:
+    def get_y_input_shape(self) -> tuple[int, int]:
         """Get shape fo transformed target data."""
         return self.input_y.shape
 
     @property
     def get_optimizer(self) -> str:
         """Get model optimizer."""
         return self.optimizer
@@ -144,15 +145,15 @@
                     "dropout": 0.0,
                 }
             },
             "layer2": {
                 "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
             },
         },
-    ):
+    ) -> None:
         """Creates MLP model.
         Parameters:
             steps_past (int): Steps predictor will look backward.
             steps_future (int): Steps predictor will look forward.
             optimizer (str): Optimization algorithm.
             optimizer_args (dict): Arguments for optimizer.
             loss (str): Loss function.
@@ -221,15 +222,15 @@
                     "dropout": 0.0,
                 }
             },
             "layer2": {
                 "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
             },
         },
-    ):
+    ) -> None:
         """Creates RNN model.
         Parameters:
             steps_past (int): Steps predictor will look backward.
             steps_future (int): Steps predictor will look forward.
             optimizer (str): Optimization algorithm.
             optimizer_args (dict): Arguments for optimizer.
             loss (str): Loss function.
@@ -288,15 +289,15 @@
                     "dropout": 0.0,
                 }
             },
             "layer2": {
                 "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
             },
         },
-    ):
+    ) -> None:
         """Creates LSTM model.
         Parameters:
             steps_past (int): Steps predictor will look backward.
             steps_future (int): Steps predictor will look forward.
             optimizer (str): Optimization algorithm.
             optimizer_args (dict): Arguments for optimizer.
             loss (str): Loss function.
@@ -366,15 +367,15 @@
                 "config": {
                     "neurons": 32,
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
-    ):
+    ) -> None:
         """Creates CNN model.
         Parameters:
             steps_past (int): Steps predictor will look backward.
             steps_future (int): Steps predictor will look forward.
             optimizer (str): Optimization algorithm.
             optimizer_args (dict): Arguments for optimizer.
             loss (str): Loss function.
@@ -437,15 +438,15 @@
                 "config": {
                     "neurons": 50,
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
-    ):
+    ) -> None:
         """Creates GRU model.
         Parameters:
             steps_past (int): Steps predictor will look backward.
             steps_future (int): Steps predictor will look forward.
             optimizer (str): Optimization algorithm.
             optimizer_args (dict): Arguments for optimizer.
             loss (str): Loss function.
@@ -499,15 +500,15 @@
                 "config": {
                     "neurons": 50,
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
-    ):
+    ) -> None:
         """Creates BI-RNN model.
         Parameters:
             steps_past (int): Steps predictor will look backward.
             steps_future (int): Steps predictor will look forward.
             optimizer (str): Optimization algorithm.
             optimizer_args (dict): Arguments for optimizer.
             loss (str): Loss function.
@@ -559,15 +560,15 @@
                 "config": {
                     "neurons": 50,
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
-    ):
+    ) -> None:
         """Creates BI-LSTM model.
         Parameters:
             steps_past (int): Steps predictor will look backward.
             steps_future (int): Steps predictor will look forward.
             optimizer (str): Optimization algorithm.
             optimizer_args (dict): Arguments for optimizer.
             loss (str): Loss function.
@@ -619,15 +620,15 @@
                 "config": {
                     "neurons": 50,
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
-    ):
+    ) -> None:
         """Creates BI-GRU model.
         Parameters:
             steps_past (int): Steps predictor will look backward.
             steps_future (int): Steps predictor will look forward.
             optimizer (str): Optimization algorithm.
             optimizer_args (dict): Arguments for optimizer.
             loss (str): Loss function.
@@ -657,21 +658,23 @@
         )
 
     def fit_model(
         self,
         epochs: int,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
-    ):
+    ) -> Any:
         """Trains the model on data provided. Perfroms validation.
         Parameters:
             epochs (int): Number of epochs to train the model.
             show_progress (int): Prints training progress.
             board (bool): Create TensorBoard.
+            batch_size (float): Batch size.
             callback_settings (dict): Create a Keras EarlyStopping object.
         """
         if callback_setting == {}:
             if board == True:
                 callback_board = TensorBoard(
                     log_dir="logs/fit/"
                     + self.model_id
@@ -682,23 +685,25 @@
                     self.input_x,
                     self.input_y,
                     validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     callbacks=[callback_board],
                     shuffle=False,
+                    batch_size=batch_size,
                 )
             else:
                 self.details = self.model.fit(
                     self.input_x,
                     self.input_y,
                     validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     shuffle=False,
+                    batch_size=batch_size,
                 )
 
         else:
             if board == True:
                 callback_board = TensorBoard(
                     log_dir="logs/fit/"
                     + self.model_id
@@ -710,48 +715,66 @@
                     self.input_x,
                     self.input_y,
                     validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     callbacks=[callback, callback_board],
                     shuffle=False,
+                    batch_size=batch_size,
                 )
             else:
                 callback = EarlyStopping(**callback_setting)
                 self.details = self.model.fit(
                     self.input_x,
                     self.input_y,
                     validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     callbacks=[callback],
                     shuffle=False,
+                    batch_size=batch_size,
                 )
         return self.details
 
-    def evaluate_model(self):
-        self.evaluation_details = self.model.evaluate(
-            x=self.input_x_test, y=self.input_y_test
-        )
+    def evaluate_model(self, board: bool = False) -> Any:
+        """Evaluate model on test set.
+        Parameters:
+            board (bool): Create TensorBoard.
+        """
+        if board == True:
+            callback_board = TensorBoard(
+                log_dir="logs/eval/"
+                + self.model_id
+                + datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S"),
+                histogram_freq=1,
+            )
+            self.evaluation_details = self.model.evaluate(
+                x=self.input_x_test, y=self.input_y_test, callbacks=[callback_board]
+            )
+        else:
+            self.evaluation_details = self.model.evaluate(
+                x=self.input_x_test,
+                y=self.input_y_test,
+            )
 
         return self.evaluation_details
 
-    def model_blueprint(self):
+    def model_blueprint(self) -> Any:
         """Prints a summary of the models layer structure."""
         self.model.summary()
 
-    def show_performance(self):
+    def show_performance(self) -> Any:
         """Returns performance details."""
         return self.details
 
-    def show_evaluation(self):
+    def show_evaluation(self) -> Any:
         """Returns performance details on test data."""
         return self.evaluation_details
 
-    def predict(self, data: array) -> array:
+    def predict(self, data: np.ndarray) -> np.ndarray:
         """Takes in a sequence of values and outputs a forecast.
         Parameters:
             data (array): Input sequence which needs to be forecasted.
         Returns:
             (array): Forecast for sequence provided.
         """
 
@@ -765,22 +788,22 @@
             data = data.reshape((1, dimension))  # MLP case
             y_pred = self.model.predict(data, verbose=0)
 
         y_pred = y_pred.reshape(y_pred.shape[1], y_pred.shape[0])
 
         return y_pred
 
-    def freeze(self, absolute_path: str = CURRENT_PATH):
+    def freeze(self, absolute_path: str = CURRENT_PATH) -> None:
         """Save the current model to the current directory.
         Parameters:
            absolute_path (str): Path to save model to.
         """
         self.model.save(absolute_path)
 
-    def retrieve(self, location: str):
+    def retrieve(self, location: str) -> None:
         """Load a keras model from the path specified.
         Parameters:
             location (str): Path of keras model location.
         """
         self.model = load_model(location)
 
 
@@ -816,16 +839,17 @@
             "layer2": {
                 "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
-    ):
+    ) -> float:
         """Creates and trains a Multi-Layer-Perceptron model."""
         self.create_mlp(
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
             optimizer_args=optimizer_args,
             loss=loss,
@@ -835,14 +859,15 @@
             dense_block_three=dense_block_three,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_rnn(
         self,
         steps_past: int,
@@ -874,16 +899,17 @@
             "layer2": {
                 "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
-    ):
+    ) -> float:
         """Creates and trains a RNN model."""
         self.create_rnn(
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
             optimizer_args=optimizer_args,
             loss=loss,
@@ -893,14 +919,15 @@
             rnn_block_three=rnn_block_three,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_lstm(
         self,
         steps_past: int,
@@ -932,16 +959,17 @@
             "layer2": {
                 "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
-    ):
+    ) -> float:
         """Creates and trains a LSTM model."""
         self.create_lstm(
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
             optimizer_args=optimizer_args,
             loss=loss,
@@ -951,14 +979,15 @@
             lstm_block_three=lstm_block_three,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnn(
         self,
         steps_past: int,
@@ -1001,16 +1030,17 @@
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
-    ):
+    ) -> float:
         """Creates and trains a CNN model."""
         self.create_cnn(
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
             optimizer_args=optimizer_args,
             loss=loss,
@@ -1020,14 +1050,15 @@
             dense_block_one=dense_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_gru(
         self,
         steps_past: int,
@@ -1063,16 +1094,17 @@
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
-    ):
+    ) -> float:
         """Creates and trains a GRU model."""
         self.create_gru(
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
             optimizer_args=optimizer_args,
             loss=loss,
@@ -1082,14 +1114,15 @@
             gru_block_three=gru_block_three,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_birnn(
         self,
         steps_past: int,
@@ -1116,16 +1149,17 @@
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
-    ):
+    ) -> float:
         """Creates and trains a BI-RNN model."""
         self.create_birnn(
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
             optimizer_args=optimizer_args,
             loss=loss,
@@ -1134,14 +1168,15 @@
             rnn_block_one=rnn_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_bilstm(
         self,
         steps_past: int,
@@ -1168,16 +1203,17 @@
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
-    ):
+    ) -> float:
         """Creates and trains a BI-LSTM model."""
         self.create_bilstm(
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
             optimizer_args=optimizer_args,
             loss=loss,
@@ -1186,14 +1222,15 @@
             lstm_block_one=lstm_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_bigru(
         self,
         steps_past: int,
@@ -1220,16 +1257,17 @@
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
-    ):
+    ) -> float:
         """Creates and trains a BI-GRU model."""
         self.create_bigru(
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
             optimizer_args=optimizer_args,
             loss=loss,
@@ -1238,13 +1276,14 @@
             gru_block_one=gru_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
 
 __all__ = ["PureMulti"]
```

### Comparing `imbrium-3.0.0/imbrium/predictors/univarhybrid.py` & `imbrium-3.1.0/imbrium/predictors/univarhybrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
 import os
+from typing import Any
 
+import numpy as np
 from keras.callbacks import EarlyStopping, TensorBoard
 from keras.saving import load_model
-from numpy import array
 
 from imbrium.architectures.models import (cnnbigru, cnnbilstm, cnnbirnn,
                                           cnngru, cnnlstm, cnnrnn)
 from imbrium.blueprints.abstract_univariate import UniVariateMultiStep
 from imbrium.utils.optimizer import get_optimizer
 from imbrium.utils.transformer import (data_prep_uni, sequence_prep_hybrid_uni,
                                        train_test_split)
@@ -16,17 +17,17 @@
 class BaseHybridUni(UniVariateMultiStep):
     """Implements neural network based univariate multipstep hybrid predictors."""
 
     CURRENT_PATH = os.getcwd()
 
     def __init__(
         self,
-        target=array([]),
-        evaluation_split: float = 0.20,
-        validation_split: float = 0.20,
+        target: np.ndarray = np.array([]),
+        evaluation_split: float = 0.10,  # train: 90%, test: 10%
+        validation_split: float = 0.20,  # train: 72%, test: 10%, val: 18%
     ) -> object:
         """
         Parameters:
             target (array): Input target data numpy array.
             evaluation_split (float): train test split.
             validation_split (float): validation size of train set.
         """
@@ -54,53 +55,53 @@
             )
             self.input_y, self.input_y_test = train_test_split(
                 self.input_y, test_size=self.evaluation_split
             )
         else:
             pass
 
-    def set_model_id(self, name: str):
+    def set_model_id(self, name: str) -> None:
         """Setter method to change model id field.
         Parameters:
             name (str): Name for selected Model.
         """
         self.model_id = name
 
     @property
     def get_model_id(self) -> str:
         """Get model id."""
         return self.model_id
 
     @property
-    def get_target(self) -> array:
+    def get_target(self) -> np.ndarray:
         """Get original target data."""
         return self.target
 
     @property
-    def get_target_shape(self) -> array:
+    def get_target_shape(self) -> np.ndarray:
         """Get shape of original target data."""
         return self.target.shape
 
     @property
-    def get_X_input(self) -> array:
+    def get_X_input(self) -> np.ndarray:
         """Get transformed feature data."""
         return self.input_x
 
     @property
-    def get_X_input_shape(self) -> tuple:
+    def get_X_input_shape(self) -> tuple[int, int]:
         """Get shape fo transformed feature data."""
         return self.input_x.shape
 
     @property
-    def get_y_input(self) -> array:
+    def get_y_input(self) -> np.ndarray:
         """Get transformed target data."""
         return self.input_y
 
     @property
-    def get_y_input_shape(self) -> tuple:
+    def get_y_input_shape(self) -> tuple[int, int]:
         """Get shape fo transformed target data."""
         return self.input_y.shape
 
     @property
     def get_optimizer(self) -> str:
         """Get model optimizer."""
         return self.optimizer
@@ -164,15 +165,15 @@
                 "config": {
                     "neurons": 32,
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
-    ):
+    ) -> None:
         """Creates CNN-RNN hybrid model.
         Parameters:
             sub_seq (int): Divide data into further subsequences.
             steps_past (int): Steps to look back.
             steps_future (int): Steps to predict into the future.
             optimizer (str): Optimization algorithm.
             optimizer_args (dict): Arguments for optimizer.
@@ -255,15 +256,15 @@
                 "config": {
                     "neurons": 32,
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
-    ):
+    ) -> None:
         """Creates CNN-LSTM hybrid model.
         Parameters:
             sub_seq (int): Divide data into further subsequences.
             steps_past (int): Steps to look back.
             steps_future (int): Steps to predict into the future.
             optimizer (str): Optimization algorithm.
             optimizer_args (dict): Arguments for optimizer.
@@ -346,15 +347,15 @@
                 "config": {
                     "neurons": 32,
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
-    ):
+    ) -> None:
         """Creates CNN-GRU hybrid model.
         Parameters:
             sub_seq (int): Divide data into further subsequences.
             steps_past (int): Steps to look back.
             steps_future (int): Steps to predict into the future.
             optimizer (str): Optimization algorithm.
             optimizer_args (dict): Arguments for optimizer.
@@ -437,15 +438,15 @@
                 "config": {
                     "neurons": 32,
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
-    ):
+    ) -> None:
         """Creates CNN-BI-RNN hybrid model.
         Parameters:
             sub_seq (int): Divide data into further subsequences.
             steps_past (int): Steps to look back.
             steps_future (int): Steps to predict into the future.
             optimizer (str): Optimization algorithm.
             optimizer_args (dict): Arguments for optimizer.
@@ -528,15 +529,15 @@
                 "config": {
                     "neurons": 32,
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
-    ):
+    ) -> None:
         """Creates CNN-BI-LSTM hybrid model.
         Parameters:
             sub_seq (int): Divide data into further subsequences.
             steps_past (int): Steps to look back.
             steps_future (int): Steps to predict into the future.
             optimizer (str): Optimization algorithm.
             optimizer_args (dict): Arguments for optimizer.
@@ -619,15 +620,15 @@
                 "config": {
                     "neurons": 32,
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
-    ):
+    ) -> None:
         """Creates CNN-BI-GRU hybrid model.
         Parameters:
             sub_seq (int): Divide data into further subsequences.
             steps_past (int): Steps to look back.
             steps_future (int): Steps to predict into the future.
             optimizer (str): Optimization algorithm.
             optimizer_args (dict): Arguments for optimizer.
@@ -662,21 +663,23 @@
         )
 
     def fit_model(
         self,
         epochs: int,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
-    ):
+    ) -> Any:
         """Trains the model on data provided. Perfroms validation.
         Parameters:
             epochs (int): Number of epochs to train the model.
             show_progress (int): Prints training progress.
             board (bool): Create TensorBoard.
+            batch_size (float): Batch size.
             callback_settings (dict): Create a Keras EarlyStopping object.
         """
         if callback_setting == {}:
             if board == True:
                 callback_board = TensorBoard(
                     log_dir="logs/fit/"
                     + self.model_id
@@ -687,23 +690,25 @@
                     self.input_x,
                     self.input_y,
                     validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     callbacks=[callback_board],
                     shuffle=False,
+                    batch_size=batch_size,
                 )
             else:
                 self.details = self.model.fit(
                     self.input_x,
                     self.input_y,
                     validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     shuffle=False,
+                    batch_size=batch_size,
                 )
 
         else:
             if board == True:
                 callback_board = TensorBoard(
                     log_dir="logs/fit/"
                     + self.model_id
@@ -715,50 +720,68 @@
                     self.input_x,
                     self.input_y,
                     validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     callbacks=[callback, callback_board],
                     shuffle=False,
+                    batch_size=batch_size,
                 )
             else:
                 callback = EarlyStopping(**callback_setting)
                 self.details = self.model.fit(
                     self.input_x,
                     self.input_y,
                     validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     callbacks=[callback],
                     shuffle=False,
+                    batch_size=batch_size,
                 )
         return self.details
 
-    def evaluate_model(self):
-        self.evaluation_details = self.model.evaluate(
-            x=self.input_x_test, y=self.input_y_test
-        )
+    def evaluate_model(self, board: bool = False) -> Any:
+        """Evaluate model on test set.
+        Parameters:
+            board (bool): Create TensorBoard.
+        """
+        if board == True:
+            callback_board = TensorBoard(
+                log_dir="logs/eval/"
+                + self.model_id
+                + datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S"),
+                histogram_freq=1,
+            )
+            self.evaluation_details = self.model.evaluate(
+                x=self.input_x_test, y=self.input_y_test, callbacks=[callback_board]
+            )
+        else:
+            self.evaluation_details = self.model.evaluate(
+                x=self.input_x_test,
+                y=self.input_y_test,
+            )
 
         return self.evaluation_details
 
-    def model_blueprint(self):
+    def model_blueprint(self) -> Any:
         """Prints a summary of the models layer structure."""
         self.model.summary()
 
-    def show_performance(self):
+    def show_performance(self) -> Any:
         """Returns performance details."""
         return self.details
 
-    def show_evaluation(self):
+    def show_evaluation(self) -> Any:
         """Returns performance details on test data."""
         return self.evaluation_details
 
     def predict(
-        self, data: array, sub_seq: int = None, steps_past=None, steps_future=None
-    ) -> array:
+        self, data: np.ndarray, sub_seq: int = None, steps_past=None, steps_future=None
+    ) -> np.ndarray:
         """Takes in a sequence of values and outputs a forecast.
         Parameters:
             data (array): Input sequence which needs to be forecasted.
         Returns:
             (array): Forecast for sequence provided.
         """
         if sub_seq != None:
@@ -775,22 +798,22 @@
 
         y_pred = self.model.predict(data, verbose=0)
 
         y_pred = y_pred.reshape(y_pred.shape[1], y_pred.shape[0])
 
         return y_pred
 
-    def freeze(self, absolute_path: str = CURRENT_PATH):
+    def freeze(self, absolute_path: str = CURRENT_PATH) -> None:
         """Save the current model to the current directory.
         Parameters:
            absolute_path (str): Path to save model to.
         """
         self.model.save(absolute_path)
 
-    def retrieve(self, location: str):
+    def retrieve(self, location: str) -> None:
         """Load a keras model from the path specified.
         Parameters:
             location (str): Path of keras model location.
         """
         self.model = load_model(location)
 
 
@@ -847,16 +870,17 @@
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
-    ):
+    ) -> float:
         """Creates CNN-RNN hybrid model."""
         self.create_cnnrnn(
             sub_seq=sub_seq,
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
             optimizer_args=optimizer_args,
@@ -868,14 +892,15 @@
             rnn_block_two=rnn_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnlstm(
         self,
         sub_seq: int,
@@ -928,16 +953,17 @@
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
-    ):
+    ) -> float:
         """Creates CNN-LSTM hybrid model."""
         self.create_cnnlstm(
             sub_seq=sub_seq,
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
             optimizer_args=optimizer_args,
@@ -949,14 +975,15 @@
             lstm_block_two=lstm_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnngru(
         self,
         sub_seq: int,
@@ -1009,16 +1036,17 @@
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
-    ):
+    ) -> float:
         """Creates CNN-GRU hybrid model."""
         self.create_cnngru(
             sub_seq=sub_seq,
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
             optimizer_args=optimizer_args,
@@ -1030,14 +1058,15 @@
             gru_block_two=gru_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnbirnn(
         self,
         sub_seq: int,
@@ -1090,16 +1119,17 @@
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
-    ):
+    ) -> float:
         """Creates CNN-BiRNN hybrid model."""
         self.create_cnnbirnn(
             sub_seq=sub_seq,
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
             optimizer_args=optimizer_args,
@@ -1111,14 +1141,15 @@
             rnn_block_one=rnn_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnbilstm(
         self,
         sub_seq: int,
@@ -1171,16 +1202,17 @@
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
-    ):
+    ) -> float:
         """Creates CNN-BiLSTM hybrid model."""
         self.create_cnnbilstm(
             sub_seq=sub_seq,
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
             optimizer_args=optimizer_args,
@@ -1192,14 +1224,15 @@
             lstm_block_one=lstm_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnbigru(
         self,
         sub_seq: int,
@@ -1252,16 +1285,17 @@
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
-    ):
+    ) -> float:
         """Creates CNN-BiGRU hybrid model."""
         self.create_cnnbigru(
             sub_seq=sub_seq,
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
             optimizer_args=optimizer_args,
@@ -1273,13 +1307,14 @@
             gru_block_one=gru_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
 
 __all__ = ["HybridUni"]
```

### Comparing `imbrium-3.0.0/imbrium/predictors/univarpure.py` & `imbrium-3.1.0/imbrium/predictors/univarpure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import datetime
 import os
-from typing import Tuple
 
+import numpy as np
 from keras.callbacks import EarlyStopping, TensorBoard
 from keras.saving import load_model
-from numpy import array
 
 from imbrium.architectures.models import (bigru, bilstm, birnn, cnn, gru, lstm,
                                           mlp, rnn)
 from imbrium.blueprints.abstract_univariate import UniVariateMultiStep
 from imbrium.utils.optimizer import get_optimizer
 from imbrium.utils.transformer import (data_prep_uni,
                                        sequence_prep_standard_uni,
@@ -18,17 +17,17 @@
 class BasePureUni(UniVariateMultiStep):
     """Implements neural network based univariate multipstep predictors."""
 
     CURRENT_PATH = os.getcwd()
 
     def __init__(
         self,
-        target: array = array([]),
-        evaluation_split: float = 0.20,
-        validation_split: float = 0.20,
+        target: np.ndarray = np.array([]),
+        evaluation_split: float = 0.10,  # train: 90%, test: 10%
+        validation_split: float = 0.20,  # train: 72%, test: 10%, val: 18%
     ) -> object:
         """
         Parameters:
             target (array): Input target data numpy array.
             evaluation_split (float): train test split.
             validation_split (float): validation size of train set.
         """
@@ -65,35 +64,35 @@
 
     @property
     def get_model_id(self) -> str:
         """Get model id."""
         return self.model_id
 
     @property
-    def get_target(self) -> array:
+    def get_target(self) -> np.ndarray:
         """Get original target data."""
         return self.target
 
     @property
-    def get_target_shape(self) -> array:
+    def get_target_shape(self) -> np.ndarray:
         """Get shape of original target data."""
         return self.target.shape
 
     @property
-    def get_X_input(self) -> array:
+    def get_X_input(self) -> np.ndarray:
         """Get transformed feature data."""
         return self.input_x
 
     @property
     def get_X_input_shape(self) -> tuple:
         """Get shape fo transformed feature data."""
         return self.input_x.shape
 
     @property
-    def get_y_input(self) -> array:
+    def get_y_input(self) -> np.ndarray:
         """Get transformed target data."""
         return self.input_y
 
     @property
     def get_y_input_shape(self) -> tuple:
         """Get shape fo transformed target data."""
         return self.input_y.shape
@@ -652,21 +651,23 @@
         )
 
     def fit_model(
         self,
         epochs: int,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
     ):
         """Trains the model on data provided. Perfroms validation.
         Parameters:
             epochs (int): Number of epochs to train the model.
             show_progress (int): Prints training progress.
             board (bool): Creates TensorBoard.
+            batch_size (float): Batch size.
             callback_settings (dict): Create a Keras EarlyStopping object.
         """
         if callback_setting == {}:
             if board == True:
                 callback_board = TensorBoard(
                     log_dir="logs/fit/"
                     + self.model_id
@@ -677,23 +678,25 @@
                     self.input_x,
                     self.input_y,
                     validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     callbacks=[callback_board],
                     shuffle=False,
+                    batch_size=batch_size,
                 )
             else:
                 self.details = self.model.fit(
                     self.input_x,
                     self.input_y,
                     validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     shuffle=False,
+                    batch_size=batch_size,
                 )
 
         else:
             if board == True:
                 callback_board = TensorBoard(
                     log_dir="logs/fit/"
                     + self.model_id
@@ -705,32 +708,50 @@
                     self.input_x,
                     self.input_y,
                     validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     callbacks=[callback, callback_board],
                     shuffle=False,
+                    batch_size=batch_size,
                 )
             else:
                 callback = EarlyStopping(**callback_setting)
                 self.details = self.model.fit(
                     self.input_x,
                     self.input_y,
                     validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     callbacks=[callback],
                     shuffle=False,
+                    batch_size=batch_size,
                 )
         return self.details
 
-    def evaluate_model(self):
-        self.evaluation_details = self.model.evaluate(
-            x=self.input_x_test, y=self.input_y_test
-        )
+    def evaluate_model(self, board: bool = False):
+        """Evaluate model on test set.
+        Parameters:
+            board (bool): Create TensorBoard.
+        """
+        if board == True:
+            callback_board = TensorBoard(
+                log_dir="logs/eval/"
+                + self.model_id
+                + datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S"),
+                histogram_freq=1,
+            )
+            self.evaluation_details = self.model.evaluate(
+                x=self.input_x_test, y=self.input_y_test, callbacks=[callback_board]
+            )
+        else:
+            self.evaluation_details = self.model.evaluate(
+                x=self.input_x_test,
+                y=self.input_y_test,
+            )
 
         return self.evaluation_details
 
     def model_blueprint(self):
         """Prints a summary of the models layer structure."""
         self.model.summary()
 
@@ -738,15 +759,15 @@
         """Returns performance details."""
         return self.details
 
     def show_evaluation(self):
         """Returns performance details on test data."""
         return self.evaluation_details
 
-    def predict(self, data: array) -> array:
+    def predict(self, data: np.ndarray) -> np.ndarray:
         """Takes in a sequence of values and outputs a forecast.
         Parameters:
             data (array): Input sequence which needs to be forecasted.
         Returns:
             (array): Forecast for sequence provided.
         """
         data = data.reshape(-1, 1)
@@ -812,14 +833,15 @@
             "layer2": {
                 "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
     ):
         """Creates and trains a Multi-Layer-Perceptron model."""
         self.create_mlp(
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
@@ -831,14 +853,15 @@
             dense_block_three=dense_block_three,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_rnn(
         self,
         steps_past: int,
@@ -870,14 +893,15 @@
             "layer2": {
                 "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
     ):
         """Creates and trains a Recurrent Neural Network model."""
         self.create_rnn(
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
@@ -889,14 +913,15 @@
             rnn_block_three=rnn_block_three,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_lstm(
         self,
         steps_past: int,
@@ -928,14 +953,15 @@
             "layer2": {
                 "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
     ):
         """Creates and trains a LSTM model."""
         self.create_lstm(
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
@@ -947,14 +973,15 @@
             lstm_block_three=lstm_block_three,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnn(
         self,
         steps_past: int,
@@ -997,14 +1024,15 @@
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
     ):
         """Creates and trains a Convolutional Neural Network model."""
         self.create_cnn(
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
@@ -1016,14 +1044,15 @@
             dense_block_one=dense_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_gru(
         self,
         steps_past: int,
@@ -1059,14 +1088,15 @@
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
     ):
         """Creates and trains a GRU model."""
         self.create_gru(
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
@@ -1078,14 +1108,15 @@
             gru_block_three=gru_block_three,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_birnn(
         self,
         steps_past: int,
@@ -1112,14 +1143,15 @@
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
     ):
         """Creates and trains a Bidirectional RNN model."""
         self.create_birnn(
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
@@ -1130,14 +1162,15 @@
             rnn_block_one=rnn_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_bilstm(
         self,
         steps_past: int,
@@ -1164,14 +1197,15 @@
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
     ):
         """Creates and trains a Bidirectional LSTM model."""
         self.create_bilstm(
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
@@ -1182,14 +1216,15 @@
             lstm_block_one=lstm_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_bigru(
         self,
         steps_past: int,
@@ -1216,14 +1251,15 @@
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
         board: bool = False,
+        batch_size=None,
         **callback_setting: dict,
     ):
         """Creates and trains a Bidirectional GRU model."""
         self.create_bigru(
             steps_past=steps_past,
             steps_future=steps_future,
             optimizer=optimizer,
@@ -1234,13 +1270,14 @@
             gru_block_one=gru_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             board=board,
+            batch_size=batch_size,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
 
 __all__ = ["PureUni"]
```

### Comparing `imbrium-3.0.0/imbrium/utils/transformer.py` & `imbrium-3.1.0/imbrium/utils/transformer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,40 @@
-from typing import Tuple
+import numpy as np
 
-from numpy import array, dstack, empty, vstack
 
-
-def data_prep_uni(data: array) -> array:
+def data_prep_uni(data: np.ndarray) -> np.ndarray:
     """Prepares data for model intake.
     Parameters:
         data (array): Input time series.
     Returns:
         data (array): Input time series.
     """
     data = data.reshape(-1, 1)
 
     return data
 
 
-def data_prep_multi(target: array, features: array) -> array:
+def data_prep_multi(target: np.ndarray, features: np.ndarray) -> np.ndarray:
     """Prepare target and feature numpy arrays for mulitvariate model intake.
     Parameters:
         target (array): Array containing multi-feature data.
         features (array): All features that should be considered.
     Returns:
         data (array): Array containing sequences of selected features.
     """
     if target.ndim == 2:
         target = target.T
-    data = vstack((target, features.T))
+    data = np.vstack((target, features.T))
 
     return data
 
 
 def sequence_prep_standard_uni(
-    input_sequence: array, steps_past: int, steps_future: int
-) -> [(array, array)]:
+    input_sequence: np.ndarray, steps_past: int, steps_future: int
+) -> tuple[np.ndarray, np.ndarray]:
     """Prepares data input into X and y sequences. Length of the X sequence
     is determined by steps_past while the length of y is determined by
     steps_future. In detail, the predictor looks at sequence X and
     predicts sequence y.
      Parameters:
          input_sequence (array): Sequence that contains time series in
          array format
@@ -44,15 +42,15 @@
          steps_future (int): Steps the predictor will look forward
      Returns:
          X (array): Array containing all looking back sequences
          y (array): Array containing all looking forward sequences
     """
     length = len(input_sequence)
     if length == 0:
-        return (empty(shape=[steps_past, steps_past]), 0)
+        return (np.empty(shape=[steps_past, steps_past]), 0)
     X = []
     y = []
     if length <= steps_past:
         raise ValueError(
             "Input sequence is equal to or shorter than steps to look backwards"
         )
     if steps_future <= 0:
@@ -60,35 +58,35 @@
 
     for i in range(length):
         last = i + steps_past
         if last > length - steps_future:
             break
         X.append(input_sequence[i:last])
         y.append(input_sequence[last : last + steps_future])
-    y = array(y)
-    X = array(X)
+    y = np.array(y)
+    X = np.array(X)
     X = X.reshape((X.shape[0], X.shape[1], 1))
     return X, y
 
 
 def sequence_prep_standard_multi(
-    input_sequence: array, steps_past: int, steps_future: int
-) -> [(array, array)]:
+    input_sequence: np.ndarray, steps_past: int, steps_future: int
+) -> tuple[np.ndarray, np.ndarray]:
     """Prepares data input into X and y sequences. Lenght of the X sequence is dertermined by steps_past while the length of y is determined by steps_future. In detail, the predictor looks at sequence X and predicts sequence y.
     Parameters:
         input_sequence (array): Sequence that contains time series in array format
         steps_past (int): Steps the predictor will look backward
         steps_future (int): Steps the predictor will look forward
     Returns:
         X (array): Array containing all looking back sequences
         y (array): Array containing all looking forward sequences
     """
     length = len(input_sequence)
     if length == 0:
-        return (empty(shape=[steps_past, steps_past]), 0)
+        return (np.empty(shape=[steps_past, steps_past]), 0)
     X = []
     y = []
     if length <= steps_past:
         raise ValueError(
             "Input sequence is equal to or shorter than steps to look backwards"
         )
     if steps_future <= 0:
@@ -99,23 +97,23 @@
         if last > length - steps_future:
             X.append(input_sequence[i:last])
             y.append(input_sequence[last - 1 : last - 1 + steps_future])
             break
         X.append(input_sequence[i:last])
         # modification to use correct target y sequence
         y.append(input_sequence[last - 1 : last - 1 + steps_future])
-    y = array(y)
-    X = array(X)
+    y = np.array(y)
+    X = np.array(X)
     X = X.reshape((X.shape[0], X.shape[1], 1))
     return X, y
 
 
 def sequence_prep_hybrid_uni(
-    input_sequence: array, sub_seq: int, steps_past: int, steps_future: int
-) -> [(array, array, int)]:
+    input_sequence: np.ndarray, sub_seq: int, steps_past: int, steps_future: int
+) -> tuple[np.ndarray, np.ndarray, int]:
     """Prepares data input into X and y sequences. Length of the X sequence
     is determined by steps_past while the length of y is determined by
     steps_future. In detail, the predictor looks at sequence X and
     predicts sequence y.
      Parameters:
          input_sequence (array): Sequence that contains time series in
          array format.
@@ -142,24 +140,24 @@
 
     for i in range(length):
         last = i + steps_past
         if last > length - steps_future:
             break
         X.append(input_sequence[i:last])
         y.append(input_sequence[last : last + steps_future])
-    y = array(y)
-    X = array(X)
+    y = np.array(y)
+    X = np.array(X)
     modified_back = X.shape[1] // sub_seq
     X = X.reshape((X.shape[0], sub_seq, modified_back, 1))
     return X, y, modified_back
 
 
 def sequence_prep_hybrid_multi(
-    input_sequence: array, sub_seq: int, steps_past: int, steps_future: int
-) -> [(array, array, int)]:
+    input_sequence: np.ndarray, sub_seq: int, steps_past: int, steps_future: int
+) -> tuple[np.ndarray, np.ndarray, int]:
     """Prepares data input into X and y sequences. Lenght of the X sequence
     is dertermined by steps_past while the length of y is determined by
     steps_future. In detail, the predictor looks at sequence X and
     predicts sequence y.
          Parameters:
              input_sequence (array): Sequence that contains time series in
              array format
@@ -168,15 +166,15 @@
              steps_future (int): Steps the predictor will look forward
          Returns:
              X (array): Array containing all looking back sequences
              y (array): Array containing all looking forward sequences
     """
     length = len(input_sequence)
     if length == 0:
-        return (empty(shape=[steps_past, steps_past]), 0)
+        return (np.empty(shape=[steps_past, steps_past]), 0)
     X = []
     y = []
     if length <= steps_past:
         raise ValueError(
             "Input sequence is equal to or shorter than steps to look backwards"
         )
     if steps_future <= 0:
@@ -187,28 +185,28 @@
         if last > length - steps_future:
             X.append(input_sequence[i:last])
             y.append(input_sequence[last - 1 : last - 1 + steps_future])
             break
         X.append(input_sequence[i:last])
         # modification to use correct target y sequence
         y.append(input_sequence[last - 1 : last - 1 + steps_future])
-    y = array(y)
-    X = array(X)
+    y = np.array(y)
+    X = np.array(X)
     modified_back = X.shape[1] // sub_seq
     X = X.reshape((X.shape[0], sub_seq, modified_back, 1))
     return (
         X,
         y,
         modified_back,
     )  # special treatment to account for sub sequence division
 
 
 def multistep_prep_standard(
-    input_sequence: array, steps_past: int, steps_future: int
-) -> [(array, array)]:
+    input_sequence: np.ndarray, steps_past: int, steps_future: int
+) -> tuple[np.ndarray, np.ndarray]:
     """This function prepares input sequences into a suitable input format for a multivariate multistep model. The first seqeunce in the array needs to be the target variable y.
     Parameters:
         input_sequence (array): Sequence that contains time series in array format
         steps_past (int): Steps the predictor will look backward
         steps_future (int): Steps the predictor will look forward
     Returns:
         X (array): Array containing all looking back sequences
@@ -221,22 +219,22 @@
             _, y = sequence_prep_standard_multi(
                 input_sequence[0], steps_past, steps_future
             )
             Y.append(y)
             continue  # skip since target column not requiered in X array
         x, _ = sequence_prep_standard_multi(input_sequence[i], steps_past, steps_future)
         X.append(x)
-    X = dstack(X)
+    X = np.dstack(X)
     Y = Y[0]  # getting array out of list
     return X, Y
 
 
 def multistep_prep_hybrid(
-    input_sequence: array, sub_seq: int, steps_past: int, steps_future: int
-) -> [(array, array)]:
+    input_sequence: np.ndarray, sub_seq: int, steps_past: int, steps_future: int
+) -> tuple[np.ndarray, np.ndarray]:
     """This function prepares input sequences into a suitable input format
     for a multivariate multistep model. The first seqeunce in the array
     needs to be the target variable y.
          Parameters:
              input_sequence (array): Sequence that contains time series
              in array format
              sub_seq (int): Devision into subsequences.
@@ -255,20 +253,20 @@
             )
             Y.append(y)
             continue  # skip since target column not requiered in X array
         x, _, mod = sequence_prep_hybrid_multi(
             input_sequence[i], sub_seq, steps_past, steps_future
         )
         X.append(x)
-    X = dstack(X)
+    X = np.dstack(X)
     Y = Y[0]  # getting array out of list
     return X, Y, mod
 
 
-def train_test_split(data: array, test_size=0.2) -> Tuple[array, array]:
+def train_test_split(data: np.ndarray, test_size=0.2) -> tuple[np.ndarray, np.ndarray]:
     """Splits the time series data into training and testing sets.
     Parameters:
         data (array): Sequence that contains time series
         in array format
         test_size (float): % of original data used as test dataset
     Returns:
         train_data (array): Array containing train data
```

### Comparing `imbrium-3.0.0/imbrium.egg-info/SOURCES.txt` & `imbrium-3.1.0/imbrium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imbrium-3.0.0/setup.py` & `imbrium-3.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,19 +9,19 @@
     author="Maximilian Mekiska",
     author_email="maxmekiska@gmail.com",
     url="https://github.com/maxmekiska/imbrium",
     description="Standard and Hybrid Deep Learning Multivariate-Multi-Step & Univariate-Multi-Step Time Series Forecasting.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     name="imbrium",
-    version="3.0.0",
+    version="3.1.0",
     packages=find_packages(include=["imbrium", "imbrium.*"]),
     install_requires=[
         "setuptools >= 41.0.0",
-        "tensorflow>=2.16.0",
+        "tensorflow >=2.16.0, <2.17.0",
     ],
     classifiers=[
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: Microsoft :: Windows",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
```

