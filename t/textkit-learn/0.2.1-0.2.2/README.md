# Comparing `tmp/textkit_learn-0.2.1.tar.gz` & `tmp/textkit_learn-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `textkit_learn-0.2.1.tar` & `textkit_learn-0.2.2.tar`

### file list

```diff
@@ -1,35 +1,85 @@
--rw-r--r--   0        0        0      567 1970-01-01 00:00:00.000000 textkit_learn-0.2.1/rust/Cargo.toml
--rw-r--r--   0      501       20      547 2024-03-21 17:12:17.000000 textkit_learn-0.2.1/rust/src/lib.rs
--rw-r--r--   0      501       20     8327 2024-03-21 17:18:10.000000 textkit_learn-0.2.1/rust/Cargo.lock
--rw-r--r--   0      501       20     3626 2024-03-21 17:05:54.000000 textkit_learn-0.2.1/pyproject.toml
--rw-r--r--   0      501       20     8079 2024-03-11 16:47:24.000000 textkit_learn-0.2.1/src/tklearn/metrics/classification.py
--rw-r--r--   0      501       20      192 2024-03-19 16:25:13.000000 textkit_learn-0.2.1/src/tklearn/metrics/__init__.py
--rw-r--r--   0      501       20     2381 2024-03-11 16:47:24.000000 textkit_learn-0.2.1/src/tklearn/metrics/common.py
--rw-r--r--   0      501       20     7372 2024-03-11 16:47:24.000000 textkit_learn-0.2.1/src/tklearn/metrics/confusion_matrix.py
--rw-r--r--   0      501       20     6948 2024-03-19 17:22:32.000000 textkit_learn-0.2.1/src/tklearn/metrics/base.py
--rw-r--r--   0      501       20     1791 2024-03-13 23:56:37.000000 textkit_learn-0.2.1/src/tklearn/nn/callbacks/checkpoint.py
--rw-r--r--   0      501       20      477 2024-03-11 17:54:23.000000 textkit_learn-0.2.1/src/tklearn/nn/callbacks/__init__.py
--rw-r--r--   0      501       20     4377 2024-03-11 18:32:32.000000 textkit_learn-0.2.1/src/tklearn/nn/callbacks/early_stopping.py
--rw-r--r--   0      501       20     1439 2024-03-13 23:37:34.000000 textkit_learn-0.2.1/src/tklearn/nn/callbacks/progbar_logger.py
--rw-r--r--   0      501       20     1269 2024-03-19 00:21:37.000000 textkit_learn-0.2.1/src/tklearn/nn/callbacks/tracking.py
--rw-r--r--   0      501       20     7850 2024-03-11 19:42:38.000000 textkit_learn-0.2.1/src/tklearn/nn/callbacks/base.py
--rw-r--r--   0      501       20       63 2024-03-11 16:47:24.000000 textkit_learn-0.2.1/src/tklearn/nn/__init__.py
--rw-r--r--   0      501       20        0 2024-03-11 16:47:24.000000 textkit_learn-0.2.1/src/tklearn/nn/utils/__init__.py
--rw-r--r--   0      501       20     5150 2024-03-13 22:56:52.000000 textkit_learn-0.2.1/src/tklearn/nn/utils/data.py
--rw-r--r--   0      501       20    13409 2024-03-20 19:45:57.000000 textkit_learn-0.2.1/src/tklearn/nn/torch.py
--rw-r--r--   0      501       20       59 2024-03-21 17:12:58.000000 textkit_learn-0.2.1/src/tklearn/__init__.py
--rw-r--r--   0      501       20     1351 2024-03-11 17:24:43.000000 textkit_learn-0.2.1/src/tklearn/utils/logging.py
--rw-r--r--   0      501       20        0 2024-03-11 16:47:24.000000 textkit_learn-0.2.1/src/tklearn/utils/__init__.py
--rw-r--r--   0      501       20     2682 2024-03-11 16:47:24.000000 textkit_learn-0.2.1/src/tklearn/utils/collections.py
--rw-r--r--   0      501       20     1506 2024-03-11 16:47:24.000000 textkit_learn-0.2.1/src/tklearn/utils/target_types.py
--rw-r--r--   0      501       20     9310 2024-03-19 21:54:54.000000 textkit_learn-0.2.1/src/tklearn/utils/array.py
--rw-r--r--   0      501       20       84 2024-03-11 16:47:24.000000 textkit_learn-0.2.1/src/tklearn/utils/progbar.py
--rw-r--r--   0      501       20     1683 2024-03-11 16:47:24.000000 textkit_learn-0.2.1/src/tklearn/utils/func.py
--rw-r--r--   0      501       20        0 2024-03-21 15:00:18.000000 textkit_learn-0.2.1/src/tklearn/py.typed
--rw-r--r--   0      501       20     6557 2024-03-11 16:47:24.000000 textkit_learn-0.2.1/src/tklearn/preprocessing/tokenization.py
--rw-r--r--   0      501       20       64 2024-03-21 16:59:58.000000 textkit_learn-0.2.1/src/tklearn/rslib.pyi
--rw-r--r--   0      501       20     6333 2024-03-11 21:28:18.000000 textkit_learn-0.2.1/src/tklearn/base/callback.py
--rw-r--r--   0      501       20        0 2024-03-11 16:47:24.000000 textkit_learn-0.2.1/src/tklearn/base/__init__.py
--rw-r--r--   0      501       20      644 2024-03-11 16:47:24.000000 textkit_learn-0.2.1/src/tklearn/base/model.py
--rw-r--r--   0      501       20      188 2023-09-30 16:23:07.000000 textkit_learn-0.2.1/README.md
--rw-r--r--   0        0        0     1910 1970-01-01 00:00:00.000000 textkit_learn-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/Makefile
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/requirements.txt
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/requirements_dev.txt
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/.vscode/settings.json
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/examples/example_RoBERTa-base-go_emotions_emotion.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/examples/example_arrow_base_types.py
+-rw-r--r--   0        0        0     5060 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/examples/example_arrow_types.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/examples/example_check_tracked.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/examples/example_conceptnet_v_5_7_kb.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/examples/example_dask.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/examples/example_document.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/examples/example_documents_benchmark.py
+-rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/examples/example_hf_model_finetune.py
+-rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/examples/example_llm_emotion.py
+-rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/examples/example_llm_hate_speech_detection.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/examples/example_metadata.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/examples/example_text_kb.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/examples/example_tokenizer.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/examples/example_triple_extractor.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/examples/text_callbacks.py
+-rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/notebooks/example_knowledge_base.ipynb
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/scratch/base.py
+-rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/scratch/graph.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/scratch/index.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/__init__.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/py.typed
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/scripts.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/base/__init__.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/base/resource.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/kb/__init__.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/kb/conceptnet/__init__.py
+-rw-r--r--   0        0        0     8203 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/kb/conceptnet/concept.py
+-rw-r--r--   0        0        0     5531 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/kb/conceptnet/io.py
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/kb/conceptnet/relation.py
+-rw-r--r--   0        0        0    14237 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/kb/conceptnet/uri.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/kb/emolex/__init__.py
+-rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/kb/emolex/io.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/lang/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/lang/en/__init__.py
+-rw-r--r--   0        0        0    19066 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/lang/en/_contractions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/llm/__init__.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/llm/constraint.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/llm/verbalizer.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/nn/__init__.py
+-rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/nn/loss.py
+-rw-r--r--   0        0        0    15673 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/nn/module.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/nn/callbacks/__init__.py
+-rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/nn/callbacks/base.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/nn/callbacks/checkpoint.py
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/nn/callbacks/early_stopping.py
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/nn/callbacks/progbar_logger.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/nn/callbacks/tracking.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/nn/metrics/__init__.py
+-rw-r--r--   0        0        0     7194 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/nn/metrics/base.py
+-rw-r--r--   0        0        0     8270 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/nn/metrics/classification.py
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/nn/metrics/common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/nn/utils/__init__.py
+-rw-r--r--   0        0        0    10373 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/nn/utils/array.py
+-rw-r--r--   0        0        0     4466 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/nn/utils/data.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/nn/utils/logging.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/nn/utils/progbar.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/preprocessing/__init__.py
+-rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/preprocessing/annotator.py
+-rw-r--r--   0        0        0    18813 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/preprocessing/emoticons.py
+-rw-r--r--   0        0        0    34925 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/preprocessing/keyword_processor.py
+-rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/preprocessing/preprocessor.py
+-rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/preprocessing/tokenization.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/utils/__init__.py
+-rw-r--r--   0        0        0    10163 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/utils/array.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/utils/collections.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/utils/download.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/utils/func.py
+-rw-r--r--   0        0        0     7668 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/utils/html.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/utils/logging.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/utils/progbar.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/utils/string.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/src/tklearn/utils/target_types.py
+-rw-r--r--   0        0        0    11866 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/tests/test_classification_metrics.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/LICENSE
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/README.md
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 textkit_learn-0.2.2/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `textkit_learn-0.2.1/pyproject.toml` & `textkit_learn-0.2.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,10 @@
 [build-system]
-build-backend = "maturin"
-requires = ["maturin>=1,<2"]
-
-[tool.maturin]
-# "extension-module" tells pyo3 we want to build an extension module 
-#   (skips linking against libpython.so)
-features = ["pyo3/extension-module"]
-# Python source directory
-python-source = "src"
-module-name = "tklearn.rslib"
-# Python packages to include
-python-packages = ["tklearn"]
-# Strip the library for minimum file size
-strip = true
-include = [{ format = "sdist", path = "rust/Cargo.lock" }]
-# Source distribution generator, supports cargo (default) and git.
-sdist-generator = "cargo"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
 [project]
 name = "textkit-learn"
 requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -55,23 +40,29 @@
     "datasets",
     "evaluate",
     "accelerate",
     "nltk",
     "sortedcontainers",
     "hnswlib",
     "flashtext",
-    "octoflow>=0.0.8",
+    "octoflow~=0.1.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
-homepage = "https://github.com/ysenarath/textkit-learn"
-repository = "https://github.com/ysenarath/textkit-learn"
-issues = "https://github.com/ysenarath/textkit-learn/issues"
-changelog = "https://github.com/ysenarath/textkit-learn/blob/master/CHANGELOG.md"
+Homepage = "https://github.com/ysenarath/textkit-learn"
+Repository = "https://github.com/ysenarath/textkit-learn"
+Issues = "https://github.com/ysenarath/textkit-learn/issues"
+Changelog = "https://github.com/ysenarath/textkit-learn/blob/master/CHANGELOG.md"
+
+[tool.hatch.version]
+path = "src/tklearn/__init__.py"
+
+[tool.hatch.build.targets.wheel]
+packages = ["src/tklearn"]
 
 [tool.ruff]
 extend-include = ["*.ipynb"]
 target-version = "py38"
 line-length = 88
 indent-width = 4
 preview = true # preview features & checks, use with caution
@@ -109,12 +100,7 @@
 docstring-code-format = false
 # Set the line length limit used when formatting code snippets in
 # docstrings.
 #
 # This only has an effect when the `docstring-code-format` setting is
 # enabled.
 docstring-code-line-length = "dynamic"
-
-[tool.mypy]
-python_version = "3.8"
-# ignore stubs
-ignore_missing_imports = true
```

### Comparing `textkit_learn-0.2.1/src/tklearn/metrics/classification.py` & `textkit_learn-0.2.2/src/tklearn/nn/metrics/classification.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
 from typing import (
     Any,
+    Dict,
+    List,
     Literal,
     Optional,
     Union,
 )
 
 import numpy as np
 import torch
@@ -17,28 +19,28 @@
     precision_recall_curve,
     precision_score,
     recall_score,
     roc_auc_score,
     roc_curve,
 )
 
-from tklearn.metrics.base import Metric
-from tklearn.metrics.common import (
-    SAMPLE_WEIGHT,
-    Y_PRED,
-    Y_SCORE,
-    Y_TRUE,
+from tklearn.nn.metrics.base import Metric
+from tklearn.nn.metrics.common import (
     AccumMetric,
+    sample_weight_getter,
+    y_pred_getter,
+    y_score_getter,
+    y_true_getter,
 )
 
 
 class Accuracy(Metric):
-    y_true: AccumMetric = Y_TRUE
-    y_pred: AccumMetric = Y_PRED
-    sample_weight: AccumMetric = SAMPLE_WEIGHT
+    y_true: AccumMetric = y_true_getter
+    y_pred: AccumMetric = y_pred_getter
+    sample_weight: AccumMetric = sample_weight_getter
 
     def __init__(
         self,
         normalize: bool = True,
         balanced: bool = False,
         adjusted: Optional[bool] = None,
     ):
@@ -65,23 +67,21 @@
             y_pred,
             normalize=self.normalize,
             sample_weight=sample_weight,
         )
 
 
 class RocAuc(Metric):
-    y_true: AccumMetric = Y_TRUE
-    y_score: AccumMetric = Y_SCORE
-    sample_weight: AccumMetric = SAMPLE_WEIGHT
+    y_true: AccumMetric = y_true_getter
+    y_score: AccumMetric = y_score_getter
+    sample_weight: AccumMetric = sample_weight_getter
 
     def __init__(
         self,
-        average: Optional[
-            Literal["micro", "macro", "samples", "weighted"]
-        ] = "macro",
+        average: Optional[Literal["micro", "macro", "samples", "weighted"]] = "macro",
         max_fpr: Optional[float] = None,
         multi_class: Literal["raise", "ovr", "ovo"] = "raise",
         labels: Optional[ArrayLike] = None,
     ) -> None:
         super().__init__()
         self.average = average
         self.max_fpr = max_fpr
@@ -100,17 +100,17 @@
             max_fpr=self.max_fpr,
             multi_class=self.multi_class,
             labels=self.labels,
         )
 
 
 class Precision(Metric):
-    y_true: AccumMetric = Y_TRUE
-    y_pred: AccumMetric = Y_PRED
-    sample_weight: AccumMetric = SAMPLE_WEIGHT
+    y_true: AccumMetric = y_true_getter
+    y_pred: AccumMetric = y_pred_getter
+    sample_weight: AccumMetric = sample_weight_getter
 
     def __init__(
         self,
         average: Optional[
             Literal["binary", "micro", "macro", "samples", "weighted"]
         ] = "macro",
         pos_label: Union[int, str] = 1,
@@ -135,17 +135,17 @@
             average=self.average,
             sample_weight=sample_weight,
             zero_division=self.zero_division,
         )
 
 
 class Recall(Metric):
-    y_true: AccumMetric = Y_TRUE
-    y_pred: AccumMetric = Y_PRED
-    sample_weight: AccumMetric = SAMPLE_WEIGHT
+    y_true: AccumMetric = y_true_getter
+    y_pred: AccumMetric = y_pred_getter
+    sample_weight: AccumMetric = sample_weight_getter
 
     def __init__(
         self,
         average: Optional[
             Literal["binary", "micro", "macro", "samples", "weighted"]
         ] = "macro",
         pos_label: Union[int, str] = 1,
@@ -170,17 +170,17 @@
             average=self.average,
             sample_weight=sample_weight,
             zero_division=self.zero_division,
         )
 
 
 class F1Score(Metric):
-    y_true: AccumMetric = Y_TRUE
-    y_pred: AccumMetric = Y_PRED
-    sample_weight: AccumMetric = SAMPLE_WEIGHT
+    y_true: AccumMetric = y_true_getter
+    y_pred: AccumMetric = y_pred_getter
+    sample_weight: AccumMetric = sample_weight_getter
 
     def __init__(
         self,
         average: Optional[
             Literal["binary", "micro", "macro", "samples", "weighted"]
         ] = "macro",
         labels: Optional[ArrayLike] = None,
@@ -205,28 +205,28 @@
             average=self.average,
             sample_weight=sample_weight,
             zero_division=self.zero_division,
         )
 
 
 class OptimalRocAucThreshold(Metric):
-    y_true: AccumMetric = Y_TRUE
-    y_score: AccumMetric = Y_SCORE
-    sample_weight: AccumMetric = SAMPLE_WEIGHT
+    y_true: AccumMetric = y_true_getter
+    y_score: AccumMetric = y_score_getter
+    sample_weight: AccumMetric = sample_weight_getter
 
     def __init__(
         self,
         pos_label: Union[int, str, None] = None,
         drop_intermediate: bool = True,
     ) -> None:
         super().__init__()
         self.pos_label = pos_label
         self.drop_intermediate = drop_intermediate
 
-    def result(self) -> float:
+    def result(self) -> List[Dict[str, float]]:
         y_true = self.y_true.result()
         y_score = self.y_score.result()
         sample_weight = self.sample_weight.result()
         fpr, tpr, thresholds = roc_curve(
             y_true,
             y_score,
             pos_label=self.pos_label,
@@ -242,43 +242,41 @@
                 "optimal": i == optimal_idx,
             }
             for i, (f, t, th) in enumerate(zip(fpr, tpr, thresholds))
         ]
 
 
 class OptimalPRThreshold(Metric):
-    y_true: AccumMetric = Y_TRUE
-    y_score: AccumMetric = Y_SCORE
-    sample_weight: AccumMetric = SAMPLE_WEIGHT
+    y_true: AccumMetric = y_true_getter
+    y_score: AccumMetric = y_score_getter
+    sample_weight: AccumMetric = sample_weight_getter
 
     def __init__(
         self,
         pos_label: Union[int, str, None] = None,
         drop_intermediate: bool = True,
         zero_division: Any = 0.0,
     ) -> None:
         super().__init__()
         self.pos_label = pos_label
         self.drop_intermediate = drop_intermediate
         self.zero_division = zero_division
 
-    def result(self) -> float:
+    def result(self) -> List[Dict[str, float]]:
         y_true = self.y_true.result()
         y_score = self.y_score.result()
         sample_weight = self.sample_weight.result()
         precision, recall, thresholds = precision_recall_curve(
             y_true,
             y_score,
             pos_label=self.pos_label,
             sample_weight=sample_weight,
             drop_intermediate=self.drop_intermediate,
         )
-        optimal_idx = np.argmax(
-            2 * precision * recall / (precision + recall + 1e-12)
-        )
+        optimal_idx = np.argmax(2 * precision * recall / (precision + recall + 1e-12))
         return [
             {
                 "precision": p,
                 "recall": r,
                 "f1": 2 * p * r / (p + r) if p + r > 0 else self.zero_division,
                 "thresholds": t,
                 "optimal": i == optimal_idx,
```

### Comparing `textkit_learn-0.2.1/src/tklearn/metrics/common.py` & `textkit_learn-0.2.2/src/tklearn/nn/metrics/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,39 +5,37 @@
     Literal,
     Optional,
 )
 
 import numpy as np
 import torch
 
-from tklearn.metrics.base import Metric
+from tklearn.nn.metrics.base import Metric
 
 
 class StepsCounter(Metric):
     def reset(self) -> None:
         self.state = {"value": 0}
 
     def update(self, *args, **kwargs: Any) -> None:
         self.state["value"] += 1
 
     def result(self) -> int:
         return self.state["value"]
 
 
-STEPS_COUNTER = StepsCounter()
+count_steps = StepsCounter()
 
 
 class AccumMetric(Metric):
-    steps_counter: StepsCounter = STEPS_COUNTER
+    steps_counter: StepsCounter = count_steps
 
     def __init__(
         self,
-        field: Literal[
-            "y_true", "y_pred", "sample_weight", "y_score"
-        ] = "y_true",
+        field: Literal["y_true", "y_pred", "sample_weight", "y_score"] = "y_true",
         axis: int = 0,
     ) -> None:
         super().__init__()
         self.field = field
         self.axis = axis
 
     def reset(self) -> None:
@@ -77,14 +75,14 @@
             curr_value = np.concatenate([curr_value, value], axis=self.axis)
         self.state["value"] = curr_value
 
     def result(self) -> torch.Tensor:
         return self.state["value"]
 
 
-Y_TRUE = AccumMetric("y_true", axis=0)
+y_true_getter = AccumMetric("y_true", axis=0)
 
-Y_PRED = AccumMetric("y_pred", axis=0)
+y_pred_getter = AccumMetric("y_pred", axis=0)
 
-Y_SCORE = AccumMetric("y_score", axis=0)
+y_score_getter = AccumMetric("y_score", axis=0)
 
-SAMPLE_WEIGHT = AccumMetric("sample_weight", axis=0)
+sample_weight_getter = AccumMetric("sample_weight", axis=0)
```

### Comparing `textkit_learn-0.2.1/src/tklearn/metrics/base.py` & `textkit_learn-0.2.2/src/tklearn/nn/metrics/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from __future__ import annotations
 
 import base64
 import contextlib
 import contextvars
 import copy
-import functools
 import uuid
 from collections import OrderedDict
 from dataclasses import MISSING
 from typing import (
     Any,
     Dict,
     List,
+    Literal,
     Mapping,
     MutableMapping,
     Optional,
     Sequence,
     Tuple,
     TypeVar,
     Union,
+    overload,
 )
 
 import cloudpickle
 from typing_extensions import ParamSpec
 
 __all__ = [
+    "Evaluator",
     "Metric",
     "MetricState",
 ]
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
@@ -67,14 +69,25 @@
     if current_state is MISSING:
         msg = "trying to set state of a metric outside the context"
         raise ValueError(msg)
     current_state[var] = value
     _current_state_cv.set(current_state)
 
 
+def update_state(__var: Union[Metric, str], **kwargs: Any) -> Any:
+    if isinstance(__var, Metric):
+        __var = __var.id
+    current_state: MetricState = _current_state_cv.get()
+    if current_state is MISSING:
+        msg = "trying to set state of a metric outside the context"
+        raise ValueError(msg)
+    current_state[__var].update(**kwargs)
+    _current_state_cv.set(current_state)
+
+
 def urlsafe_b64encoded_uuid4() -> str:
     return base64.urlsafe_b64encode(uuid.uuid4().bytes).decode().rstrip("=")
 
 
 class Metric:
     def __init__(self) -> None:
         self.id = urlsafe_b64encoded_uuid4()
@@ -86,27 +99,30 @@
     @state.setter
     def state(self, value: Any) -> None:
         set_state(self, value)
 
     def reset(self) -> None:
         self.state = {}
 
-    def update(
-        self, y_true: Any = None, y_pred: Any = None, **kwargs: Any
-    ) -> None:
+    def update(self, **kwargs: Any) -> None:
         pass
 
     def result(self) -> Any:
         raise NotImplementedError
 
     def copy(self, deep: bool = True) -> Metric:
         if deep:
             return cloudpickle.loads(cloudpickle.dumps(self))
         return copy.copy(self)
 
+    def __call__(self, **kwargs: Any) -> Any:
+        evaluator = Evaluator(self)
+        evaluator.update_state(**kwargs)
+        return evaluator.result()[0]
+
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(...)"
 
 
 class MetricState(MutableMapping[str, MetricStateValue]):
     def __init__(self) -> None:
         super().__init__()
@@ -114,17 +130,15 @@
         self._vals_dict: MutableMapping[str, MetricStateValue] = {}
 
     def __getitem__(self, key: Union[Metric, str]) -> MetricStateValue:
         if isinstance(key, Metric):
             key = key.id
         return self._vals_dict[key]
 
-    def __setitem__(
-        self, key: Union[Metric, str], value: MetricStateValue
-    ) -> None:
+    def __setitem__(self, key: Union[Metric, str], value: MetricStateValue) -> None:
         if isinstance(key, Metric):
             key = key.id
         self._vals_dict[key] = value
 
     def __delitem__(self, key: Union[Metric, str]) -> None:
         if isinstance(key, Metric):
             key = key.id
@@ -154,23 +168,18 @@
             if not isinstance(class_var_val, Metric):
                 continue
             self.add_metric(class_var_val)
         if metric.id not in self._vars_dict:
             self._vars_dict[metric.id] = metric
         self.reset()
 
-    def update(
-        self,
-        y_true: Any = None,
-        y_pred: Any = None,
-        **kwargs: Any,
-    ) -> None:
+    def update(self, **kwargs: Any) -> None:
         with self.ctx():
             for var in self._vars_dict.values():
-                var.update(y_true, y_pred, **kwargs)
+                var.update(**kwargs)
 
     def reset(self) -> None:
         with self.ctx():
             for var in self._vars_dict.values():
                 var.reset()
 
     def result(self, metric: Metric) -> Any:
@@ -180,18 +189,21 @@
     def ctx(self) -> contextlib.AbstractContextManager:
         return set_state_context(self)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self._vals_dict!r})"
 
 
+EvaluatorMetricsInput = Union[Metric, Sequence[Metric], Dict[str, Metric], None]
+
+
 class Evaluator:
     def __init__(
         self,
-        metrics: Union[Sequence[Metric], Dict[str, Metric], None] = None,
+        metrics: EvaluatorMetricsInput = None,
         metric_names: Optional[List[str]] = None,
         state: Optional[MetricState] = None,
     ) -> None:
         if metrics is None:
             metrics = []
         elif isinstance(metrics, Metric):
             metrics = [metrics]
@@ -208,43 +220,31 @@
         self.state = state
         for metric in self.metrics:
             self.state.add_metric(metric)
 
     def reset(self):
         self.state.reset()
 
-    def update_state(self, y_true, y_pred, **kwargs):
-        self.state.update(y_true=y_true, y_pred=y_pred, **kwargs)
+    def update_state(self, **kwargs):
+        self.state.update(**kwargs)
+
+    @overload
+    def result(self, return_dict: Literal[False]) -> Tuple: ...
 
-    def result(
-        self, return_dict: bool = False
-    ) -> Union[Dict[str, Any], Tuple[Any, ...]]:
+    @overload
+    def result(self, return_dict: Literal[True]) -> Dict[str, Any]: ...
+
+    def result(self, return_dict: bool = True) -> Any:
         if return_dict:
-            if len(self.metrics) == 0:
-                return {}
-            if self.metric_names is None:
-                msg = (
-                    "'metric_names' should be provided to return a dictionary"
-                )
-                raise ValueError(msg)
-            return {
-                name: self.state.result(metric)
-                for name, metric in zip(self.metric_names, self.metrics)
-            }
+            return self._result_return_dict()
         return tuple(self.state.result(metric) for metric in self.metrics)
 
-
-@functools.wraps(
-    Evaluator,
-    updated=(),
-    assigned=(
-        "__annotations__",
-        "__doc__",
-    ),
-)
-def create_evaluator(
-    *args: Any,
-    **kwargs: Any,
-) -> Evaluator:
-    if len(args) == 1 and not kwargs and isinstance(args[0], Evaluator):
-        return args[0]
-    return Evaluator(*args, **kwargs)
+    def _result_return_dict(self) -> Dict[str, Any]:
+        if len(self.metrics) == 0:
+            return {}
+        if self.metric_names is None:
+            msg = "'metric_names' should be provided to return a dictionary"
+            raise ValueError(msg)
+        return {
+            name: self.state.result(metric)
+            for name, metric in zip(self.metric_names, self.metrics)
+        }
```

### Comparing `textkit_learn-0.2.1/src/tklearn/nn/callbacks/checkpoint.py` & `textkit_learn-0.2.2/src/tklearn/nn/callbacks/checkpoint.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from pathlib import Path
 from typing import Union
 
 import torch
 from transformers import PreTrainedModel
 
-from tklearn.nn.callbacks.base import ModelCallback
+from tklearn.nn.callbacks.base import Callback
 
 __all__ = [
     "ModelCheckpoint",
 ]
 
 
-class ModelCheckpoint(ModelCallback):
+class ModelCheckpoint(Callback):
     def __init__(
         self,
         filepath: Union[str, Path],
         # monitor: str = 'val_loss',
         verbose: int = 0,
         # save_best_only: bool = False,
         # save_weights_only: bool = False,
@@ -36,15 +36,15 @@
         self.filepath.mkdir(parents=True, exist_ok=True)
         self.step = 0
 
     def on_epoch_end(self, epoch: int, logs=None):
         if self.save_freq == "epoch":
             self.save_model()
 
-    def on_batch_end(self, batch: int, logs=None):
+    def on_train_batch_end(self, batch, logs=None):
         self.step += 1
         if self.save_freq == "batch":
             self.save_model()
 
     def save_model(self):
         model = self.model
         if model is None:
```

### Comparing `textkit_learn-0.2.1/src/tklearn/nn/callbacks/early_stopping.py` & `textkit_learn-0.2.2/src/tklearn/nn/callbacks/early_stopping.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import copy
 from typing import Optional
 
 import numpy as np
 
-from tklearn.nn.callbacks.base import ModelCallback
-from tklearn.utils.logging import get_logger
+from tklearn.nn.callbacks.base import Callback
+from tklearn.nn.utils.logging import get_logger
 
 __all__ = [
     "EarlyStopping",
 ]
 
 logger = get_logger(__name__)
 
 
-class EarlyStopping(ModelCallback):
+class EarlyStopping(Callback):
     def __init__(
         self,
         monitor: str = "valid_loss",
         min_delta: float = 0,
         patience: int = 0,
         verbose: int = 0,
         mode: str = "auto",
@@ -44,28 +44,25 @@
     @property
     def mode(self) -> str:
         return self._mode
 
     @mode.setter
     def mode(self, mode):
         if mode not in {"auto", "min", "max"}:
-            msg = (
-                f"mode {mode} is unknown, "
-                'expected one of ("auto", "min", "max")'
-            )
+            msg = f"mode {mode} is unknown, " 'expected one of ("auto", "min", "max")'
             raise ValueError(msg)
         self._mode = mode
         if mode == "min":
             self.monitor_op = np.less
         elif mode == "max":
             self.monitor_op = np.greater
         elif (
             self.monitor.endswith("acc")
-            or self.monitor.endswith("accuracy")
             or self.monitor.endswith("auc")
+            or self.monitor.endswith("_score")
         ):
             self.monitor_op = np.greater
         elif self.monitor.endswith("loss") or self.monitor.endswith("error"):
             self.monitor_op = np.less
         else:
             msg = f"could not infer the metric direction for {self.monitor}."
             raise ValueError(msg)
@@ -100,17 +97,15 @@
                 logger.debug(msg)
             self.best = current
             self.best_epoch = epoch
             if self.restore_best_weights:
                 self.best_weights = copy.deepcopy(self.model.state_dict())
             # Only restart wait if we beat both the baseline and our previous
             # best.
-            if self.baseline is None or self._is_improvement(
-                current, self.baseline
-            ):
+            if self.baseline is None or self._is_improvement(current, self.baseline):
                 self.wait = 0
             return
         # Only check after the first epoch.
         if self.wait >= self.patience and epoch > 0:
             self.stopped_epoch = epoch
             if self.restore_best_weights and self.best_weights is not None:
                 if self.verbose > 0:
```

### Comparing `textkit_learn-0.2.1/src/tklearn/nn/utils/data.py` & `textkit_learn-0.2.2/src/tklearn/nn/utils/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 from __future__ import annotations
 
 import operator
 from typing import (
     Any,
     Generator,
     Generic,
-    List,
     Optional,
     Sequence,
     Tuple,
     TypeVar,
     Union,
     overload,
 )
 
 import numpy as np
 import torch
 from torch.utils.data import Dataset as TorchDataset
 from torch.utils.data import IterableDataset as IterableTorchDataset
-from torch.utils.data.dataloader import default_collate
 from typing_extensions import Self, TypedDict
 
-from tklearn.utils.array import (
+from tklearn.nn.utils.array import (
     MovableToDeviceMixin,
     get_index,
     length_of_first_array_like_in_nested_dict,
     move_to_device,
     to_numpy,
 )
 
 __all__ = [
     "Dataset",
     "IterableDataset",
     "Record",
     "RecordBatch",
-    "create_dataset",
 ]
 
 XT, YT = TypeVar("XT"), TypeVar("YT")
 
 
 class Record(TypedDict, Generic[XT, YT]):
     x: XT
@@ -158,34 +155,14 @@
         return {"x": ix, "y": iy, "index": __item}
 
     def __len__(self) -> int:
         if self._length is None:
             self._length = length_of_first_array_like_in_nested_dict(self.x)
         return self._length
 
-    def collate(self, batch: List[Record[XT, YT]]) -> RecordBatch:  # noqa: PLR6301
-        batch = default_collate(batch)
-        index = batch.pop("index")
-        batch = batch["x"], batch.get("y", None)
-        return RecordBatch(*batch, index=index)
-
     def __repr__(self) -> str:
         return repr(self._data)
 
 
 class IterableDataset(Dataset, IterableTorchDataset):
     def __iter__(self) -> Generator[Record, None, None]:
         yield from (self[i] for i in range(len(self)))
-
-
-def create_dataset(
-    x: Sequence[XT],
-    y: Optional[Sequence[YT]] = None,
-    /,
-    iterable: bool = False,
-) -> Dataset[XT, YT]:
-    if isinstance(x, Dataset):
-        if y is not None:
-            msg = "y must be None if x is a Dataset"
-            raise ValueError(msg)
-        return x
-    return Dataset(x, y, iterable=iterable)
```

### Comparing `textkit_learn-0.2.1/src/tklearn/nn/torch.py` & `textkit_learn-0.2.2/src/tklearn/nn/module.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,38 +2,38 @@
 
 import functools
 import gc
 from typing import (
     Any,
     Dict,
     Generator,
+    Generic,
     Optional,
     Sequence,
     Tuple,
     TypedDict,
     TypeVar,
     Union,
 )
 
 import torch
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
 from torch.utils.data import DataLoader
+from torch.utils.data.dataloader import default_collate
 from typing_extensions import ParamSpec, Self, Unpack
 
-from tklearn.base.model import ModelBase
-from tklearn.metrics import Evaluator, Metric, create_evaluator
-from tklearn.nn.callbacks import ModelCallback, ModelCallbackList
-from tklearn.nn.utils.data import RecordBatch, create_dataset
-from tklearn.utils.array import concat, detach, move_to_device
+from tklearn.nn.callbacks import Callback, CallbackList
+from tklearn.nn.loss import LossDict
+from tklearn.nn.metrics import Evaluator, Metric
+from tklearn.nn.utils.array import concat, detach, move_to_device
+from tklearn.nn.utils.data import Dataset, Record, RecordBatch
 
 P = ParamSpec("P")
 
-TorchModule = TypeVar("TorchModule", bound=torch.nn.Module)
-
 X, Y, Z = TypeVar("X"), TypeVar("Y"), TypeVar("Z")
 
 XY = Union[
     X,
     Tuple[X, Y],
     None,
 ]
@@ -43,16 +43,19 @@
     torch.cuda.empty_cache()
     gc.collect()
 
 
 def get_available_device() -> str:
     if torch.cuda.is_available():
         return "cuda"
-    elif torch.backends.mps.is_available():
-        return "mps" if not torch.backends.mps.is_built() else "cpu"
+    try:
+        if torch.backends.mps.is_available():
+            return "mps" if not torch.backends.mps.is_built() else "cpu"
+    except AttributeError:
+        pass
     return "cpu"
 
 
 class TrainingArgs(TypedDict):
     batch_size: int
     epochs: int
     shuffle: bool
@@ -62,21 +65,22 @@
     optimizer: Union[str, Dict[str, Any], Optimizer]
     optimizer_args: Optional[Dict[str, Any]]
     lr_scheduler: Union[str, Dict[str, Any], LRScheduler, None]
     lr_scheduler_args: Optional[Dict[str, Any]]
     lr_scheduler_step: Optional[Dict[str, Any]]
     clip_grad_norm: Union[bool, float, Dict[str, Any], None]
     clip_grad_norm_args: Optional[Dict[str, Any]]
-    callbacks: Optional[ModelCallbackList]
+    callbacks: Optional[CallbackList]
+    loss_args: Optional[Dict[str, Any]]
 
 
-class Model(torch.nn.Module, ModelBase[X, Y, Z]):
+class Module(torch.nn.Module, Generic[X, Y, Z]):
     def to(
         self, device: Union[str, torch.device, None] = None, **kwargs: Any
-    ) -> Model:
+    ) -> Module:
         if device is None:
             device = get_available_device()
         return super().to(device, **kwargs)
 
     @property
     def device(self) -> torch.device:
         return next(self.parameters()).device
@@ -87,48 +91,62 @@
             return self._stop_training
         return False
 
     @stop_training.setter
     def stop_training(self, value: bool) -> None:
         self._stop_training = value
 
-    def fit(
+    @property
+    def training_args(self) -> Dict[str, Any]:
+        if not hasattr(self, "_training_args"):
+            self._training_args = {}
+        return self._training_args
+
+    def fit(  # noqa: PLR0914
         self,
         x: XY,
         y: Y = None,
         /,
         **kwargs: Unpack[TrainingArgs],
     ) -> Self:
         self.training_args.clear()
         self.training_args.update(kwargs)
         batch_size = self.training_args.get("batch_size", 32)
-        train_dataset = create_dataset(x, y)
+        loss_args = self.training_args.get("loss_args", {})
+        if isinstance(x, Dataset) and y is not None:
+            msg = "y should be None when x is a Dataset"
+            raise ValueError(msg)
+        train_dataset = x if isinstance(x, Dataset) else Dataset(x, y)
         shuffle = self.training_args.get("shuffle", True)
         train_dataloader = DataLoader(
             train_dataset,
             batch_size=batch_size,
             shuffle=shuffle,
-            collate_fn=train_dataset.collate,
+            collate_fn=self.collate_fn,
         )
         callbacks = self.training_args.get("callbacks", None)
-        if not isinstance(callbacks, ModelCallbackList):
-            callbacks = ModelCallbackList(callbacks)
+        if not isinstance(callbacks, CallbackList):
+            callbacks = CallbackList(callbacks)
         validation_data = self.training_args.get("validation_data")
         validation_batch_size = self.training_args.get(
             "validation_batch_size", batch_size
         )
         metrics = self.training_args.get("metrics")
-        evaluate = functools.partial(
-            self.evaluate,
-            validation_data,
-            metrics=metrics,
-            prefix="valid_",
-            callbacks=callbacks,
-            batch_size=validation_batch_size,
-            return_dict=True,
+        evaluate = (
+            functools.partial(
+                self.evaluate,
+                validation_data,
+                metrics=metrics,
+                prefix="valid_",
+                callbacks=callbacks,
+                batch_size=validation_batch_size,
+                return_dict=True,
+            )
+            if validation_data is not None and metrics is not None
+            else None
         )
         self.stop_training = False
         device = self.device
         self.train()
         optimizer = self._fit_configure_optimizers()
         steps = len(train_dataloader)
         lr_scheduler = self._fit_configure_lr_scheduler(optimizer)
@@ -140,90 +158,94 @@
         }
         callbacks.set_params(params)
         callbacks.set_model(self)
         callbacks.on_train_begin()
         epoch_logs = {}
         for epoch_idx in range(epochs):
             callbacks.on_epoch_begin(epoch_idx)
-            batch_idx, total_loss = 0, 0.0
+            batch_idx, total_loss_dict = 0, None
             for batch_idx, batch in enumerate(train_dataloader):
-                total_loss += self._fit_on_batch(
-                    batch=batch,
-                    batch_idx=batch_idx,
-                    callbacks=callbacks,
-                    device=device,
-                    optimizer=optimizer,
-                    lr_scheduler=lr_scheduler,
+                total_loss_dict = (
+                    self._fit_on_batch(
+                        batch=batch,
+                        batch_idx=batch_idx,
+                        callbacks=callbacks,
+                        device=device,
+                        optimizer=optimizer,
+                        lr_scheduler=lr_scheduler,
+                        loss_args=loss_args,
+                    )
+                    + total_loss_dict
                 )
-                empty_cache()
             self._fit_lr_scheduler_step(lr_scheduler, "epoch")
             n_batches = batch_idx + 1
-            epoch_logs = {
-                "loss": (total_loss / n_batches) if n_batches > 0 else None,
-            }
-            eval_results = evaluate()
-            epoch_logs.update(eval_results)
+            if n_batches > 0 and total_loss_dict is not None:
+                epoch_logs = (total_loss_dict / n_batches).to_dict()
+            else:
+                epoch_logs = {}
+            if evaluate is not None:
+                eval_results = evaluate()
+                epoch_logs.update(eval_results)
             callbacks.on_epoch_end(epoch_idx, logs=epoch_logs)
             if self.stop_training:
                 break
         callbacks.on_train_end(epoch_logs)
         self.training_args.clear()
         return self
 
     def _fit_on_batch(
         self,
         batch: RecordBatch,
         *,
         device: Union[str, torch.device],
         optimizer: Optimizer,
         lr_scheduler: Union[LRScheduler, Any, None],
-        callbacks: Optional[ModelCallbackList] = None,
+        callbacks: Optional[CallbackList] = None,
         batch_idx: Optional[int] = None,
-    ) -> float:
+        loss_args: Optional[Dict[str, Any]] = None,
+    ) -> LossDict[float]:
+        if loss_args is None:
+            loss_args = {}
         if callbacks:
             callbacks.on_train_batch_begin(batch_idx)
         if not self.training:
             self.train()
         batch = move_to_device(batch, device)
         batch_output = self.predict_on_batch(batch)
-        loss = self.compute_loss(batch, batch_output)
+        loss = self.compute_loss(batch, batch_output, **loss_args)
+        loss_dict = LossDict.from_loss(loss)
         optimizer.zero_grad()
-        loss.backward()
+        loss_dict.loss.backward()
         self._fit_clip_grad_norm()
         optimizer.step()
         self._fit_lr_scheduler_step(lr_scheduler, "batch")
-        loss_value = loss.item()
         batch_logs = {}
         if callbacks:
             callbacks.on_train_batch_end(
                 batch_idx,
                 logs=batch_logs,
             )
-        return loss_value
+        return loss_dict.item()
 
     def _fit_clip_grad_norm(self) -> None:
         clip_grad_norm = self.training_args.get("clip_grad_norm")
         if clip_grad_norm is False or clip_grad_norm is None:
             return
-        clip_grad_norm_args: dict = self.training_args.get(
-            "clip_grad_norm_args", {}
-        )
+        clip_grad_norm_args: dict = self.training_args.get("clip_grad_norm_args", {})
         if isinstance(clip_grad_norm, (int, float)):
             clip_grad_norm_args["max_norm"] = clip_grad_norm
         elif isinstance(clip_grad_norm, dict):
             clip_grad_norm_args.update(clip_grad_norm)
         else:
             msg = (
                 "clip_grad_norm should be a boolean, int, "
                 f"float, or dict, but got {clip_grad_norm}"
             )
             raise ValueError(msg)
-        torch.nn.utils.clip_grad_norm_(
-            self.parameters(), **clip_grad_norm_args
-        )
+        torch.nn.utils.clip_grad_norm_(self.parameters(), **clip_grad_norm_args)
 
     def _fit_configure_optimizers(self) -> Optimizer:
         optimizer = self.training_args.get("optimizer")
         if isinstance(optimizer, str):
             optimizer_type = getattr(torch.optim, optimizer)
             optimizer_args = self.training_args.get("optimizer_args", {})
             return optimizer_type(
@@ -249,17 +271,15 @@
             lr_scheduler_type = getattr(torch.optim.lr_scheduler, lr_scheduler)
             lr_scheduler_args = self.training_args.get("lr_schedule_args", {})
             return lr_scheduler_type(
                 optimizer,
                 **lr_scheduler_args,
             )
         if isinstance(lr_scheduler, dict):
-            lr_scheduler_type = getattr(
-                torch.optim.lr_scheduler, lr_scheduler["$type"]
-            )
+            lr_scheduler_type = getattr(torch.optim.lr_scheduler, lr_scheduler["$type"])
             lr_scheduler_args = {
                 k: v for k, v in lr_scheduler.items() if not k.startswith("$")
             }
             return lr_scheduler_type(
                 optimizer,
                 **lr_scheduler_args,
             )
@@ -284,123 +304,144 @@
 
     def predict(
         self,
         x: XY,
         y: Y = None,
         /,
         batch_size: int = 32,
-        callbacks: Optional[Sequence[ModelCallback]] = None,
+        callbacks: Optional[Sequence[Callback]] = None,
     ) -> Z:
-        output = []
+        logits = None
         for _, _, batch_output, _ in self.predict_iter(
             x,
             y,
             batch_size=batch_size,
             callbacks=callbacks,
         ):
-            output.append(batch_output)
-        return concat(output)
+            logits = concat((logits, batch_output["logits"]))
+        if logits is None:
+            msg = (
+                f"no predictions found for the given input data of "
+                f"type '{type(x).__name__}' and size {len(x)}"
+            )
+            raise ValueError(msg)
+        return logits
 
     def predict_iter(
         self,
         x: XY,
         y: Y = None,
         /,
         batch_size: int = 32,
-        callbacks: Optional[Sequence[ModelCallback]] = None,
-    ) -> Generator[Tuple[int, RecordBatch, Z, float], None, None]:
+        callbacks: Optional[Sequence[Callback]] = None,
+        loss_args: Optional[Dict[str, Any]] = None,
+    ) -> Generator[Tuple[int, RecordBatch, Z, LossDict[float]], None, None]:
         device = next(self.parameters()).device
-        if not isinstance(callbacks, ModelCallbackList):
-            callbacks = ModelCallbackList(callbacks)
-        test_dataset = create_dataset(x, y)
+        if not isinstance(callbacks, CallbackList):
+            callbacks = CallbackList(callbacks)
+        if isinstance(x, Dataset) and y is not None:
+            msg = "y should be None when x is a Dataset"
+            raise ValueError(msg)
+        test_dataset = x if isinstance(x, Dataset) else Dataset(x, y)
         test_dataloader = DataLoader(
             test_dataset,
             shuffle=False,
             batch_size=batch_size,
-            collate_fn=test_dataset.collate,
+            collate_fn=self.collate_fn,
         )
+        callback_params = {}
+        if callbacks.params is not None:
+            callback_params.update(callbacks.params)
+        callback_params.update({"pred_steps": len(test_dataloader)})
+        callbacks.set_params(callback_params)
         self.eval()
         callbacks.on_predict_begin()
-        batch_idx, total_loss = 0, 0.0
+        batch_idx, total_loss_dict = 0, None
         for batch_idx, batch in enumerate(test_dataloader):
             callbacks.on_predict_batch_begin(batch_idx)
             if self.training:
                 self.eval()
             batch = move_to_device(batch, device)
-            batch_output = self.predict_on_batch(batch)
-            loss = self.compute_loss(batch, batch_output)
+            with torch.no_grad():
+                batch_output = self.predict_on_batch(batch)
+            loss = self.compute_loss(batch, batch_output, **(loss_args or {}))
             batch_output = move_to_device(detach(batch_output), "cpu")
-            batch_loss = loss.item()
-            total_loss += batch_loss
+            batch_loss_dict = LossDict.from_loss(loss).item()
+            total_loss_dict = batch_loss_dict + total_loss_dict
             batch_logs = {}
             callbacks.on_predict_batch_end(batch_idx, logs=batch_logs)
-            yield batch_idx, batch, batch_output, batch_loss
+            yield batch_idx, batch, batch_output, batch_loss_dict
             # clear memory cache
-            del batch, batch_output, loss, batch_loss
-            empty_cache()
+            del batch, batch_output, loss, batch_loss_dict
         n_batches = batch_idx + 1
-        average_loss = total_loss / n_batches if n_batches > 0 else None
-        logs = {
-            "loss": average_loss,
-        }
+        logs = {}
+        if n_batches > 0 and total_loss_dict is not None:
+            average_loss_dict = (total_loss_dict / n_batches).to_dict()
+            logs.update(average_loss_dict)
         callbacks.on_predict_end(logs)
 
     def predict_on_batch(self, batch: RecordBatch) -> Z:
         raise NotImplementedError
 
     def evaluate(
         self,
         x: XY,
         y: Y = None,
         /,
-        metrics: Union[
-            Evaluator, Sequence[Metric], Dict[str, Metric], None
-        ] = None,
+        metrics: Union[Evaluator, Sequence[Metric], Dict[str, Metric], None] = None,
         batch_size: int = 32,
         include_loss: bool = True,
         return_dict: bool = False,
         prefix: str = "",
-        callbacks: Optional[Sequence[ModelCallback]] = None,
+        callbacks: Optional[Sequence[Callback]] = None,
+        loss_args: Optional[Dict[str, Any]] = None,
     ) -> Union[Dict[str, Any], Tuple[Any, ...]]:
-        n_batches = 0
-        total_loss = 0.0
-        evaluator = create_evaluator(metrics)
+        evaluator = metrics if isinstance(metrics, Evaluator) else Evaluator(metrics)
         evaluator.reset()
-        for _, batch, output, batch_loss in self.predict_iter(
+        n_batches, total_loss_dict = 0, None
+        for _, batch, output, batch_loss_dict in self.predict_iter(
             x,
             y,
             callbacks=callbacks,
             batch_size=batch_size,
+            loss_args=loss_args,
         ):
             n_batches += 1
-            total_loss += batch_loss
+            total_loss_dict = batch_loss_dict + total_loss_dict
             eval_input = self.extract_eval_input(batch, output)
             evaluator.update_state(**eval_input)
-        average_loss = (total_loss / n_batches) if n_batches > 0 else None
+        average_loss_dict = {}
+        if include_loss:
+            if n_batches > 0 and total_loss_dict is not None:
+                average_loss_dict = (total_loss_dict / n_batches).to_dict()
+            # add prefix to loss keys
+            average_loss_dict = {
+                f"{prefix}{key}": value for key, value in average_loss_dict.items()
+            }
         if return_dict:
             return {
-                **({f"{prefix}loss": average_loss} if include_loss else {}),
+                **average_loss_dict,
                 **{
                     f"{prefix}{name}": value
-                    for name, value in evaluator.result(
-                        return_dict=True
-                    ).items()
+                    for name, value in evaluator.result(return_dict=True).items()
                 },
             }
         return (
-            *((average_loss,) if include_loss else ()),
+            *(v for _, v in sorted(average_loss_dict.items())),
             *evaluator.result(),
         )
 
     def extract_eval_input(  # noqa: PLR6301
         self, batch: RecordBatch, output: Z
     ) -> Dict[str, Any]:
-        return {"y_true": batch.y, "y_pred": output}
+        return {"y_true": batch.y, "y_pred": output, "y_score": output}
 
-    def compute_loss(self, batch: RecordBatch, output: Z) -> torch.Tensor:
+    def compute_loss(
+        self, batch: RecordBatch, output: Z, **kwargs: Any
+    ) -> torch.Tensor:
         raise NotImplementedError
 
-    @property
-    def training_args(self) -> Dict[str, Any]:
-        if not hasattr(self, "_training_args"):
-            self._training_args = {}
-        return self._training_args
+    def collate_fn(self, batch: Sequence[Record[XY, Y]]) -> RecordBatch:  # noqa: PLR6301
+        batch = default_collate(batch)
+        index = batch.pop("index")
+        batch = batch["x"], batch.get("y", None)
+        return RecordBatch(*batch, index=index)
```

### Comparing `textkit_learn-0.2.1/src/tklearn/utils/logging.py` & `textkit_learn-0.2.2/src/tklearn/utils/logging.py`

 * *Files identical despite different names*

### Comparing `textkit_learn-0.2.1/src/tklearn/utils/collections.py` & `textkit_learn-0.2.2/src/tklearn/utils/collections.py`

 * *Files identical despite different names*

### Comparing `textkit_learn-0.2.1/src/tklearn/utils/target_types.py` & `textkit_learn-0.2.2/src/tklearn/utils/target_types.py`

 * *Files identical despite different names*

### Comparing `textkit_learn-0.2.1/src/tklearn/utils/array.py` & `textkit_learn-0.2.2/src/tklearn/utils/array.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 import pandas as pd
 import torch
 from datasets import Dataset as HuggingFaceDataset
 from numpy import typing as nt
 from torch import Tensor
 from typing_extensions import Self
 
+from octoflow.data import Dataset as OctoFlowDataset
+
 __all__ = [
     "move_to_device",
     "to_numpy",
     "to_torch",
 ]
 
 T = TypeVar("T")
@@ -208,26 +210,28 @@
         # if all objects were None
         return None
     elem = objs[0]
     if len(objs) == 1:
         return elem
     if isinstance(elem, Dict):
         keys = set(elem.keys())
-        return {k: concat([o[k] for o in objs], axis=axis) for k in keys}
+        output = {k: concat([o[k] for o in objs], axis=axis) for k in keys}
+        try:
+            # try to convert to original type assuming dict style constructor
+            return type(elem)(**output)
+        except TypeError:
+            # if not possible, return as a dictionary
+            return output
     if isinstance(elem, Tuple) and hasattr(elem, "_fields"):  # namedtuple
         dtype = type(elem)
         size = len(elem)
-        return dtype(
-            concat([o[i] for o in objs], axis=axis) for i in range(size)
-        )
+        return dtype(concat([o[i] for o in objs], axis=axis) for i in range(size))
     if isinstance(elem, Tuple):
         size = len(elem)
-        return tuple(
-            concat([o[i] for o in objs], axis=axis) for i in range(size)
-        )
+        return tuple(concat([o[i] for o in objs], axis=axis) for i in range(size))
     if isinstance(elem, np.ndarray):
         return np.concatenate(objs, axis=axis)
     if isinstance(elem, torch.Tensor):
         return torch.cat(objs, dim=axis)
     if isinstance(elem, List):
         return functools.reduce(operator.iadd, objs, [])
     msg = f"cannot concatenate objects of type '{type(elem).__name__}'"
@@ -243,16 +247,31 @@
         The nested dictionary to search for the first list.
 
     Returns
     -------
     length : int
         The length of the first list in the nested dictionary.
     """
-    if isinstance(data, HuggingFaceDataset):
+    if isinstance(data, (HuggingFaceDataset, OctoFlowDataset)):
+        return len(data)
+    if isinstance(data, (np.ndarray, pd.DataFrame)):
+        return data.shape[0]
+    if isinstance(data, torch.Tensor):
+        return data.size(0)
+    if isinstance(data, (List, pd.Series)):
         return len(data)
+    if isinstance(data, Tuple) and hasattr(data, "_fields"):
+        # namedtuple
+        for v in data:
+            return length_of_first_array_like_in_nested_dict(v)
+        return 0
+    if not isinstance(data, Dict):
+        raise TypeError(
+            f"expected data type array-like or dict, got {type(data).__name__}"
+        )
     for v in data.values():
         if isinstance(v, Mapping):
             return length_of_first_array_like_in_nested_dict(v)
         elif isinstance(v, Tensor):
             return v.size(0)
         elif isinstance(v, (np.ndarray, pd.DataFrame)):
             return v.shape[0]
@@ -289,15 +308,17 @@
         The index to search for in the nested dictionary.
 
     Returns
     -------
     value : Any
         The value at the index in the nested dictionary.
     """
-    if isinstance(data, (torch.Tensor, np.ndarray, HuggingFaceDataset)):
+    if isinstance(
+        data, (torch.Tensor, np.ndarray, HuggingFaceDataset, OctoFlowDataset)
+    ):
         # will return dtyped value
         return data[index]
     if isinstance(data, (pd.DataFrame, pd.Series)):
         # will return dtyped value
         return data.iloc[index]
     if isinstance(data, Dict):
         return {k: get_index(v, index=index) for k, v in data.items()}
```

### Comparing `textkit_learn-0.2.1/src/tklearn/utils/func.py` & `textkit_learn-0.2.2/src/tklearn/utils/func.py`

 * *Files identical despite different names*

### Comparing `textkit_learn-0.2.1/src/tklearn/preprocessing/tokenization.py` & `textkit_learn-0.2.2/src/tklearn/preprocessing/tokenization.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,57 @@
 from __future__ import annotations
 
 import abc
 import functools
 from dataclasses import dataclass
 from os import PathLike
-from types import FunctionType
 from typing import (
     Any,
     Callable,
     Dict,
     Generic,
     List,
-    Protocol,
     Tuple,
     Type,
     TypeVar,
     Union,
-    overload,
-    runtime_checkable,
 )
 
 import nltk
 import pandas as pd
 from nltk.tokenize import TweetTokenizer as _TweetTokenizer
 from nltk.tokenize import word_tokenize
 from transformers import AutoTokenizer, PreTrainedTokenizer
 from typing_extensions import ParamSpec
 
 __all__ = [
-    "FunctionTokenizer",
-    "HuggingFaceTokenizer",
     "Tokenizer",
-    "TokenizerLike",
-    "TweetTokenizer",
+    "FunctionTokenizer",
     "WordTokenizer",
-    "tokenizer",
+    "TweetTokenizer",
+    "WhitespaceTokenizer",
+    "HuggingFaceTokenizer",
 ]
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
 class BatchTokenizeMethod(Generic[P, T]):
     def __init__(self, func: Callable[P, T], batched: bool = False):
         self.func = func
         self.batched = batched
 
     def __call__(
         self,
-        inst: Tokenizer,
+        tokenizer: Tokenizer,
         *args: P.args,
         **kwargs: P.kwargs,
     ) -> T:
-        func = functools.partial(self.func, inst)
+        func = functools.partial(self.func, tokenizer)
         text, args = args[0], args[1:]
         if self.batched:
             if isinstance(text, str):
                 text = [text]
             return func(text, *args, **kwargs)
         if isinstance(text, pd.Series):
             return text.apply(func, args=args, **kwargs)
@@ -90,40 +85,34 @@
         if not isinstance(tokenize, BatchTokenizeMethod):
             tokenize = BatchTokenizeMethod(tokenize, batched=batched)
         namespace["tokenize"] = tokenize
         cls = super().__new__(cls, name, bases, namespace, **kwargs)
         return cls
 
 
-class Tokenizer(metaclass=TokenizerMeta):
+class Tokenizer(Generic[P, T], metaclass=TokenizerMeta):
     @abc.abstractmethod
-    def tokenize(
-        self,
-        text: Union[str, List[str], List[List[str]]],
-        *args: Any,
-        **kwargs: Any,
-    ) -> Any:
+    def tokenize(self, *args: P.args, **kwargs: P.kwargs) -> T:
         raise NotImplementedError
 
-
-# ---------- FUNCTION TOKENIZER ----------
+    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> T:
+        return self.tokenize(*args, **kwargs)
 
 
-class FunctionTokenizer(Tokenizer, Generic[P, T]):
+class FunctionTokenizer(Tokenizer[P, T]):
     def __init__(self, func: Callable[P, T]):
         self._func = func
 
-    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> T:
-        return self._func(*args, **kwargs)
-
     def tokenize(self, *args: P.args, **kwargs: P.kwargs) -> T:
-        return self(*args, **kwargs)
+        return self._func(*args, **kwargs)
 
 
-# ---------- NLTK WORD TOKENIZER ----------
+class WhitespaceTokenizer(Tokenizer):
+    def tokenize(self, text: str) -> List[str]:
+        return text.split()
 
 
 @dataclass
 class WordTokenizer(Tokenizer):
     language: str = "en"
     preserve_line: bool = False
 
@@ -132,17 +121,14 @@
             self.language = "english"
         nltk.download("punkt")
 
     def tokenize(self, text: str) -> List[str]:
         return word_tokenize(text, language=self.language)
 
 
-# ---------- NLTK TWEET TOKENIZER ----------
-
-
 @dataclass
 class TweetTokenizer(Tokenizer):
     preserve_case: bool = True
     reduce_len: bool = False
     strip_handles: bool = False
     match_phone_numbers: bool = True
 
@@ -154,85 +140,30 @@
             match_phone_numbers=self.match_phone_numbers,
         )
 
     def tokenize(self, text: str) -> List[str]:
         return self._tweet_tokenizer.tokenize(text)
 
 
-# ---------- HUGGINGFACE TOKENIZER ----------
-
-
 class HuggingFaceTokenizer(Tokenizer, Generic[P, T], batched=True):
     def __init__(self, tokenizer: Callable[P, T]):
         self.hf_tokenizer = tokenizer
 
     def tokenize(self, *args: P.args, **kwargs: P.kwargs) -> T:
         return self.hf_tokenizer(*args, **kwargs)
 
-    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> T:
-        return self.tokenize(*args, **kwargs)
+    def __getattr__(self, name: str) -> Any:
+        if hasattr(self.hf_tokenizer, name):
+            return getattr(self.hf_tokenizer, name)
+        raise AttributeError
 
     @classmethod
     def from_pretrained(
         cls,
         pretrained_model_name_or_path: Union[str, PathLike[str]],
         *inputs: Any,
         **kwargs: Any,
     ):
         tokenizer: PreTrainedTokenizer = AutoTokenizer.from_pretrained(
             pretrained_model_name_or_path, *inputs, **kwargs
         )
         return HuggingFaceTokenizer(tokenizer)
-
-    def __getattr__(self, name: str) -> Any:
-        if hasattr(self.hf_tokenizer, name):
-            return getattr(self.hf_tokenizer, name)
-        raise AttributeError
-
-
-# ---------- TYPE CHECKING PROTOCOLS ----------
-
-
-@runtime_checkable
-class TokenizerLike(Protocol):
-    def tokenize(
-        self, text: Union[str, List[str], pd.Series]
-    ) -> Union[List[List[str]], pd.Series]: ...
-
-
-# ---------- ADDITIONAL DECORATORS ----------
-
-
-@overload
-def tokenizer(cls: Type[TokenizerLike]) -> Type[Tokenizer]: ...
-
-
-@overload
-def tokenizer(cls: Callable[[str], List[str]]) -> Tokenizer: ...
-
-
-def tokenizer(
-    func: Union[Callable[[str], List[str]], Type[TokenizerLike]],
-) -> Union[Type[Tokenizer], Tokenizer]:
-    if isinstance(func, FunctionType):
-        return functools.wraps(
-            func,
-            assigned=("__module__", "__name__", "__qualname__", "__doc__"),
-            updated=(),
-        )(FunctionTokenizer(func))
-    elif not issubclass(func, Tokenizer) and isinstance(func, TokenizerLike):
-
-        class WrappedTokenizer(func, Tokenizer):
-            def tokenize(
-                self, text: Union[str, List[str], pd.Series]
-            ) -> Union[List[List[str]], pd.Series]:
-                return super().tokenize(text)
-
-        return functools.wraps(
-            func,
-            assigned=("__module__", "__name__", "__qualname__", "__doc__"),
-            updated=(),
-        )(WrappedTokenizer)
-    if issubclass(func, Tokenizer):
-        return func
-    msg = f"expected tokenizer-like, but got {type(func).__name__}"
-    raise TypeError(msg)
```

### Comparing `textkit_learn-0.2.1/PKG-INFO` & `textkit_learn-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,53 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: textkit-learn
-Version: 0.2.1
+Version: 0.2.2
+Summary: Helps computers to understand human languages.
+Project-URL: Homepage, https://github.com/ysenarath/textkit-learn
+Project-URL: Repository, https://github.com/ysenarath/textkit-learn
+Project-URL: Issues, https://github.com/ysenarath/textkit-learn/issues
+Project-URL: Changelog, https://github.com/ysenarath/textkit-learn/blob/master/CHANGELOG.md
+Author: Yasas Senarath
+License-Expression: MIT
+License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Rust
 Classifier: Typing :: Typed
-Requires-Dist: pandas
-Requires-Dist: polars
-Requires-Dist: numpy
-Requires-Dist: scikit-learn >=1.4.0, !=1.3
-Requires-Dist: torch
-Requires-Dist: werkzeug
-Requires-Dist: pyarrow
-Requires-Dist: transformers
+Requires-Python: >=3.8
+Requires-Dist: accelerate
 Requires-Dist: datasets
 Requires-Dist: evaluate
-Requires-Dist: accelerate
+Requires-Dist: flashtext
+Requires-Dist: hnswlib
 Requires-Dist: nltk
+Requires-Dist: numpy
+Requires-Dist: octoflow~=0.1.0
+Requires-Dist: pandas
+Requires-Dist: polars
+Requires-Dist: pyarrow
+Requires-Dist: scikit-learn!=1.3,>=1.4.0
 Requires-Dist: sortedcontainers
-Requires-Dist: hnswlib
-Requires-Dist: flashtext
-Requires-Dist: octoflow >=0.0.8
-License-File: LICENSE
-Summary: Helps computers to understand human languages.
-Keywords: 
-Author: Yasas Senarath
-License: MIT
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: homepage, https://github.com/ysenarath/textkit-learn
-Project-URL: repository, https://github.com/ysenarath/textkit-learn
-Project-URL: issues, https://github.com/ysenarath/textkit-learn/issues
-Project-URL: changelog, https://github.com/ysenarath/textkit-learn/blob/master/CHANGELOG.md
+Requires-Dist: torch
+Requires-Dist: transformers
+Requires-Dist: werkzeug
+Description-Content-Type: text/markdown
 
 # textkit-learn
 
 *Helps computers to understand human languages.*
 
 ---
 
 TextKit-Learn (tklearn) Extends existing tools for machine learning, deep learning and text analysis for NLP tasks.
-
```

