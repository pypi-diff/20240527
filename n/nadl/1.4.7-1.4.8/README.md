# Comparing `tmp/nadl-1.4.7.tar.gz` & `tmp/nadl-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadl-1.4.7.tar", last modified: Sun May 26 19:06:24 2024, max compression
+gzip compressed data, was "nadl-1.4.8.tar", last modified: Mon May 27 00:34:29 2024, max compression
```

## Comparing `nadl-1.4.7.tar` & `nadl-1.4.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2275 2024-05-26 19:06:24.482114 nadl-1.4.7/pyproject.toml
--rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.4.7/readme.org
--rw-r--r--   0        0        0     6148 2024-05-22 06:49:46.036737 nadl-1.4.7/src/nadl/.DS_Store
--rw-r--r--   0        0        0     1806 2024-05-26 19:05:55.999203 nadl-1.4.7/src/nadl/__init__.py
--rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.4.7/src/nadl/blocks.py
--rw-r--r--   0        0        0     5812 2024-05-26 19:04:18.524496 nadl-1.4.7/src/nadl/data.py
--rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.4.7/src/nadl/images.py
--rw-r--r--   0        0        0     3564 2024-05-22 05:17:23.233277 nadl-1.4.7/src/nadl/keys.py
--rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.4.7/src/nadl/loops.py
--rw-r--r--   0        0        0     1828 2024-04-19 19:57:58.670986 nadl-1.4.7/src/nadl/metrics.py
--rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.4.7/src/nadl/nets.py
--rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.4.7/src/nadl/preprocessing.py
--rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.4.7/src/nadl/py.typed
--rw-r--r--   0        0        0     3887 2024-05-26 18:22:56.769573 nadl-1.4.7/src/nadl/states.py
--rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.4.7/src/nadl/transformers.py
--rw-r--r--   0        0        0     2363 2024-05-14 05:16:59.307787 nadl-1.4.7/src/nadl/utils.py
--rw-r--r--   0        0        0     1368 1970-01-01 00:00:00.000000 nadl-1.4.7/PKG-INFO
+-rw-r--r--   0        0        0     2275 2024-05-27 00:34:29.348197 nadl-1.4.8/pyproject.toml
+-rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.4.8/readme.org
+-rw-r--r--   0        0        0     6148 2024-05-22 06:49:46.036737 nadl-1.4.8/src/nadl/.DS_Store
+-rw-r--r--   0        0        0     1806 2024-05-27 00:34:06.699967 nadl-1.4.8/src/nadl/__init__.py
+-rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.4.8/src/nadl/blocks.py
+-rw-r--r--   0        0        0     5812 2024-05-27 00:33:58.408806 nadl-1.4.8/src/nadl/data.py
+-rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.4.8/src/nadl/images.py
+-rw-r--r--   0        0        0     3564 2024-05-22 05:17:23.233277 nadl-1.4.8/src/nadl/keys.py
+-rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.4.8/src/nadl/loops.py
+-rw-r--r--   0        0        0     1828 2024-04-19 19:57:58.670986 nadl-1.4.8/src/nadl/metrics.py
+-rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.4.8/src/nadl/nets.py
+-rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.4.8/src/nadl/preprocessing.py
+-rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.4.8/src/nadl/py.typed
+-rw-r--r--   0        0        0     3887 2024-05-26 18:22:56.769573 nadl-1.4.8/src/nadl/states.py
+-rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.4.8/src/nadl/transformers.py
+-rw-r--r--   0        0        0     2363 2024-05-14 05:16:59.307787 nadl-1.4.8/src/nadl/utils.py
+-rw-r--r--   0        0        0     1368 1970-01-01 00:00:00.000000 nadl-1.4.8/PKG-INFO
```

### Comparing `nadl-1.4.7/pyproject.toml` & `nadl-1.4.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "optax>=0.2.2",
     "equinox>=0.11.4",
     "beartype>=0.18.5",
     "scikit-image>=0.23.2",
     "orbax-checkpoint>=0.5.11",
 ]
 requires-python = ">=3.12"
-version = "1.4.7"
+version = "1.4.8"
 
 [project.readme]
 content-type = "text/plain"
 file = "readme.org"
 
 [project.license]
 text = "GPLv3"
```

### Comparing `nadl-1.4.7/readme.org` & `nadl-1.4.8/readme.org`

 * *Files identical despite different names*

### Comparing `nadl-1.4.7/src/nadl/.DS_Store` & `nadl-1.4.8/src/nadl/.DS_Store`

 * *Files identical despite different names*

### Comparing `nadl-1.4.7/src/nadl/__init__.py` & `nadl-1.4.8/src/nadl/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 from .states import BaseTrainState, state_fn
 from .utils import (
   classit,
   rle,
   rle_array,
 )
 
-__version__ = "1.4.7"
+__version__ = "1.4.8"
 
 __all__ = [
   "PG",
   "RESC",
   "SCALER",
   "BaseTrainState",
   "DState",
```

### Comparing `nadl-1.4.7/src/nadl/blocks.py` & `nadl-1.4.8/src/nadl/blocks.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.7/src/nadl/data.py` & `nadl-1.4.8/src/nadl/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         axis=0,
       )
     length = self.length if not self.drop_num else self.length - self.drop_num
 
     idxes = jnp.r_[idxes, jnp.full(self.pad, -1, idxes.dtype)]
     idxes = idxes[: length + self.pad].reshape(-1, self.batch_size)
     return DState(
-      self.transform(idxes), jnp.where(idxes == -1, 0, 1).astype(bool), idxes.shape
+      self.transform(idxes), jnp.where(idxes == -1, 1, 0).astype(bool), idxes.shape
     )
 
 
 def es_loop[T](
   loader: IdxDataloader[T],
   pg: PG,
   keys: Keys | None = None,
```

### Comparing `nadl-1.4.7/src/nadl/images.py` & `nadl-1.4.8/src/nadl/images.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.7/src/nadl/keys.py` & `nadl-1.4.8/src/nadl/keys.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.7/src/nadl/loops.py` & `nadl-1.4.8/src/nadl/loops.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.7/src/nadl/metrics.py` & `nadl-1.4.8/src/nadl/metrics.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.7/src/nadl/nets.py` & `nadl-1.4.8/src/nadl/nets.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.7/src/nadl/preprocessing.py` & `nadl-1.4.8/src/nadl/preprocessing.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.7/src/nadl/states.py` & `nadl-1.4.8/src/nadl/states.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.7/src/nadl/transformers.py` & `nadl-1.4.8/src/nadl/transformers.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.7/src/nadl/utils.py` & `nadl-1.4.8/src/nadl/utils.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.7/PKG-INFO` & `nadl-1.4.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadl
-Version: 1.4.7
+Version: 1.4.8
 Summary: Nasy's Deep Learning Toolkit
 Author-Email: Nasy <nasyxx+python@gmail.com>, Nasy <nasyxx+dl@gmail.com>, Nasy <nasyxx+git@gmail.com>
 License: GPLv3
 Requires-Python: >=3.12
 Requires-Dist: jax>=0.4.28
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: rich>=13.7.1
```
