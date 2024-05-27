# Comparing `tmp/lckytools-0.0.0a4.tar.gz` & `tmp/lckytools-0.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lckytools-0.0.0a4.tar", max compression
+gzip compressed data, was "lckytools-0.0.0a5.tar", max compression
```

## Comparing `lckytools-0.0.0a4.tar` & `lckytools-0.0.0a5.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0      294 2024-05-27 02:49:07.194502 lckytools-0.0.0a4/pyproject.toml
--rw-r--r--   0        0        0     1423 2024-05-27 01:01:39.126939 lckytools-0.0.0a4/README.md
--rw-r--r--   0        0        0        0 2024-05-27 02:47:26.411528 lckytools-0.0.0a4/src/lckytools/__init__.py
--rw-r--r--   0        0        0       40 2024-05-27 02:47:26.695814 lckytools-0.0.0a4/src/lckytools/ai/__init__.py
--rw-r--r--   0        0        0      144 2024-05-27 02:10:58.751794 lckytools-0.0.0a4/src/lckytools/ai/metrics/__init__.py
--rw-r--r--   0        0        0      829 2024-05-27 02:10:59.000094 lckytools-0.0.0a4/src/lckytools/ai/metrics/confusion_matrix.py
--rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 lckytools-0.0.0a4/PKG-INFO
+-rw-r--r--   0        0        0      294 2024-05-27 02:52:50.801135 lckytools-0.0.0a5/pyproject.toml
+-rw-r--r--   0        0        0     1423 2024-05-27 01:01:39.126939 lckytools-0.0.0a5/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 02:47:26.411528 lckytools-0.0.0a5/src/lckytools/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 02:49:11.736063 lckytools-0.0.0a5/src/lckytools/ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 02:49:12.032838 lckytools-0.0.0a5/src/lckytools/ai/metrics/__init__.py
+-rw-r--r--   0        0        0      794 2024-05-27 02:49:12.249780 lckytools-0.0.0a5/src/lckytools/ai/metrics/confusion_matrix.py
+-rw-r--r--   0        0        0        0 2024-05-27 01:21:26.273683 lckytools-0.0.0a5/src/lckytools/ai/torch/__init__.py
+-rw-r--r--   0        0        0       34 2024-05-27 01:45:10.349737 lckytools-0.0.0a5/src/lckytools/ai/torch/summary_model.py
+-rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 lckytools-0.0.0a5/PKG-INFO
```

### Comparing `lckytools-0.0.0a4/README.md` & `lckytools-0.0.0a5/README.md`

 * *Files identical despite different names*

### Comparing `lckytools-0.0.0a4/src/lckytools/ai/metrics/confusion_matrix.py` & `lckytools-0.0.0a5/src/lckytools/ai/metrics/confusion_matrix.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,11 +17,7 @@
     size = confusion_matrix.shape[0]
     df_cm = pd.DataFrame(confusion_matrix, index=list(range(size)), columns=list(range(size)))
 
     sns.heatmap(df_cm, annot=True, fmt="0.0f")
     plt.xlabel("Predicted Class", fontsize=14)
     plt.ylabel("Actual Class", fontsize=14)
     plt.title("Confusion Matrix", fontsize=16)
-
-
-def test():
-    print("asd")
```

### Comparing `lckytools-0.0.0a4/PKG-INFO` & `lckytools-0.0.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lckytools
-Version: 0.0.0a4
+Version: 0.0.0a5
 Summary: 
 License: MIT
 Author: LCKYN
 Author-email: T.Pawarit@lckyn.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

