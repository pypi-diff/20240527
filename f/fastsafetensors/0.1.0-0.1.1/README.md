# Comparing `tmp/fastsafetensors-0.1.0.tar.gz` & `tmp/fastsafetensors-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastsafetensors-0.1.0.tar", last modified: Thu May 23 04:54:53 2024, max compression
+gzip compressed data, was "fastsafetensors-0.1.1.tar", last modified: Mon May 27 07:03:07 2024, max compression
```

## Comparing `fastsafetensors-0.1.0.tar` & `fastsafetensors-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-23 04:54:53.053095 fastsafetensors-0.1.0/
--rw-rw-r--   0     1001 root         (0)    11334 2024-05-13 06:37:40.000000 fastsafetensors-0.1.0/LICENSE
--rw-r--r--   0     1001 root         (0)     2881 2024-05-23 04:54:53.053095 fastsafetensors-0.1.0/PKG-INFO
--rw-rw-r--   0     1001 root         (0)     2154 2024-05-15 06:26:06.000000 fastsafetensors-0.1.0/README.md
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-23 04:54:53.045096 fastsafetensors-0.1.0/fastsafetensors/
--rw-rw-r--   0     1001 root         (0)      273 2024-05-14 05:40:16.000000 fastsafetensors-0.1.0/fastsafetensors/__init__.py
--rw-rw-r--   0     1001 root         (0)    10219 2024-05-14 04:08:15.000000 fastsafetensors-0.1.0/fastsafetensors/common.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-23 04:54:53.049095 fastsafetensors-0.1.0/fastsafetensors/connectors/
--rw-rw-r--   0     1001 root         (0)     6001 2024-05-15 09:34:35.000000 fastsafetensors-0.1.0/fastsafetensors/connectors/tgis_weights.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-23 04:54:53.049095 fastsafetensors-0.1.0/fastsafetensors/copier/
--rw-rw-r--   0     1001 root         (0)     3961 2024-05-14 04:08:27.000000 fastsafetensors-0.1.0/fastsafetensors/copier/gds.py
--rw-rw-r--   0     1001 root         (0)     1876 2024-05-15 06:52:33.000000 fastsafetensors-0.1.0/fastsafetensors/copier/nogds.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-23 04:54:53.049095 fastsafetensors-0.1.0/fastsafetensors/cpp/
--rw-rw-r--   0     1001 root         (0)    25792 2024-05-15 07:56:17.000000 fastsafetensors-0.1.0/fastsafetensors/cpp/ext.cpp
--rw-rw-r--   0     1001 root         (0)     6492 2024-05-15 07:27:07.000000 fastsafetensors-0.1.0/fastsafetensors/cpp/ext.hpp
--rw-rw-r--   0     1001 root         (0)     6095 2024-05-13 06:38:01.000000 fastsafetensors-0.1.0/fastsafetensors/dlpack.py
--rw-rw-r--   0     1001 root         (0)     6652 2024-05-14 05:34:13.000000 fastsafetensors-0.1.0/fastsafetensors/file_buffer.py
--rw-rw-r--   0     1001 root         (0)     6775 2024-05-21 05:58:00.000000 fastsafetensors-0.1.0/fastsafetensors/loader.py
--rw-rw-r--   0     1001 root         (0)     9805 2024-05-14 04:08:07.000000 fastsafetensors-0.1.0/fastsafetensors/tensor_factory.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-23 04:54:53.049095 fastsafetensors-0.1.0/fastsafetensors.egg-info/
--rw-r--r--   0     1001 root         (0)     2881 2024-05-23 04:54:53.000000 fastsafetensors-0.1.0/fastsafetensors.egg-info/PKG-INFO
--rw-r--r--   0     1001 root         (0)      597 2024-05-23 04:54:53.000000 fastsafetensors-0.1.0/fastsafetensors.egg-info/SOURCES.txt
--rw-r--r--   0     1001 root         (0)        1 2024-05-23 04:54:53.000000 fastsafetensors-0.1.0/fastsafetensors.egg-info/dependency_links.txt
--rw-r--r--   0     1001 root         (0)      109 2024-05-23 04:54:53.000000 fastsafetensors-0.1.0/fastsafetensors.egg-info/requires.txt
--rw-r--r--   0     1001 root         (0)       16 2024-05-23 04:54:53.000000 fastsafetensors-0.1.0/fastsafetensors.egg-info/top_level.txt
--rw-rw-r--   0     1001 root         (0)      847 2024-05-22 09:58:14.000000 fastsafetensors-0.1.0/pyproject.toml
--rw-r--r--   0     1001 root         (0)       38 2024-05-23 04:54:53.053095 fastsafetensors-0.1.0/setup.cfg
--rw-rw-r--   0     1001 root         (0)     2658 2024-05-22 02:30:51.000000 fastsafetensors-0.1.0/setup.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-23 04:54:53.049095 fastsafetensors-0.1.0/tests/
--rw-rw-r--   0     1001 root         (0)     6929 2024-05-14 05:41:11.000000 fastsafetensors-0.1.0/tests/test_fastsfaetensors.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-27 07:03:07.969879 fastsafetensors-0.1.1/
+-rw-rw-r--   0     1001 root         (0)    11334 2024-05-13 06:37:40.000000 fastsafetensors-0.1.1/LICENSE
+-rw-r--r--   0     1001 root         (0)     2850 2024-05-27 07:03:07.969879 fastsafetensors-0.1.1/PKG-INFO
+-rw-rw-r--   0     1001 root         (0)     2124 2024-05-24 02:56:05.000000 fastsafetensors-0.1.1/README.md
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-27 07:03:07.961878 fastsafetensors-0.1.1/fastsafetensors/
+-rw-rw-r--   0     1001 root         (0)      273 2024-05-14 05:40:16.000000 fastsafetensors-0.1.1/fastsafetensors/__init__.py
+-rw-rw-r--   0     1001 root         (0)    10275 2024-05-27 06:51:14.000000 fastsafetensors-0.1.1/fastsafetensors/common.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-27 07:03:07.965879 fastsafetensors-0.1.1/fastsafetensors/connectors/
+-rw-rw-r--   0     1001 root         (0)     6001 2024-05-15 09:34:35.000000 fastsafetensors-0.1.1/fastsafetensors/connectors/tgis_weights.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-27 07:03:07.965879 fastsafetensors-0.1.1/fastsafetensors/copier/
+-rw-rw-r--   0     1001 root         (0)     3961 2024-05-14 04:08:27.000000 fastsafetensors-0.1.1/fastsafetensors/copier/gds.py
+-rw-rw-r--   0     1001 root         (0)     1876 2024-05-15 06:52:33.000000 fastsafetensors-0.1.1/fastsafetensors/copier/nogds.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-27 07:03:07.965879 fastsafetensors-0.1.1/fastsafetensors/cpp/
+-rw-rw-r--   0     1001 root         (0)    25792 2024-05-15 07:56:17.000000 fastsafetensors-0.1.1/fastsafetensors/cpp/ext.cpp
+-rw-rw-r--   0     1001 root         (0)     6492 2024-05-15 07:27:07.000000 fastsafetensors-0.1.1/fastsafetensors/cpp/ext.hpp
+-rw-rw-r--   0     1001 root         (0)     6095 2024-05-13 06:38:01.000000 fastsafetensors-0.1.1/fastsafetensors/dlpack.py
+-rw-rw-r--   0     1001 root         (0)     6655 2024-05-27 06:30:11.000000 fastsafetensors-0.1.1/fastsafetensors/file_buffer.py
+-rw-rw-r--   0     1001 root         (0)     6775 2024-05-21 05:58:00.000000 fastsafetensors-0.1.1/fastsafetensors/loader.py
+-rw-rw-r--   0     1001 root         (0)     9805 2024-05-14 04:08:07.000000 fastsafetensors-0.1.1/fastsafetensors/tensor_factory.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-27 07:03:07.965879 fastsafetensors-0.1.1/fastsafetensors.egg-info/
+-rw-r--r--   0     1001 root         (0)     2850 2024-05-27 07:03:07.000000 fastsafetensors-0.1.1/fastsafetensors.egg-info/PKG-INFO
+-rw-r--r--   0     1001 root         (0)      597 2024-05-27 07:03:07.000000 fastsafetensors-0.1.1/fastsafetensors.egg-info/SOURCES.txt
+-rw-r--r--   0     1001 root         (0)        1 2024-05-27 07:03:07.000000 fastsafetensors-0.1.1/fastsafetensors.egg-info/dependency_links.txt
+-rw-r--r--   0     1001 root         (0)      109 2024-05-27 07:03:07.000000 fastsafetensors-0.1.1/fastsafetensors.egg-info/requires.txt
+-rw-r--r--   0     1001 root         (0)       16 2024-05-27 07:03:07.000000 fastsafetensors-0.1.1/fastsafetensors.egg-info/top_level.txt
+-rw-rw-r--   0     1001 root         (0)      847 2024-05-27 06:58:06.000000 fastsafetensors-0.1.1/pyproject.toml
+-rw-r--r--   0     1001 root         (0)       38 2024-05-27 07:03:07.969879 fastsafetensors-0.1.1/setup.cfg
+-rw-rw-r--   0     1001 root         (0)     2658 2024-05-22 02:30:51.000000 fastsafetensors-0.1.1/setup.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-27 07:03:07.965879 fastsafetensors-0.1.1/tests/
+-rw-rw-r--   0     1001 root         (0)     6929 2024-05-14 05:41:11.000000 fastsafetensors-0.1.1/tests/test_fastsfaetensors.py
```

### Comparing `fastsafetensors-0.1.0/LICENSE` & `fastsafetensors-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastsafetensors-0.1.0/PKG-INFO` & `fastsafetensors-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastsafetensors
-Version: 0.1.0
+Version: 0.1.1
 Summary: High-performance safetensors model loader
 Author-email: Takeshi Yoshimura <tyos@jp.ibm.com>
 Maintainer-email: Takeshi Yoshimura <tyos@jp.ibm.com>
 License: Apache-2.0
 Project-URL: Repository, https://github.com/foundation-model-stack/fastsafetensors
 Keywords: fastsafetensors,safetensors,GDS
 Requires-Python: >=3.10
@@ -14,15 +14,15 @@
 Requires-Dist: torch<2.3,>=2.1
 Provides-Extra: test
 Requires-Dist: pytest>=8.1.1; extra == "test"
 Requires-Dist: pytest-cov>=5.0.0; extra == "test"
 Requires-Dist: transformers>=4.40.2; extra == "test"
 Requires-Dist: safetensors>=0.4.0; extra == "test"
 
-fastsafetensors is a reimplementation of safetensors model loader to improve efficiency.
+fastsafetensors is an efficient safetensors model loader.
 We introduced three major features to optimize model loading performance:
 1. Batched, lazy tensor instantiations
 2. GPU offloading for sharding, type conversions, and device pointer alignment.
 3. GPU Direct Storage enablement for file loading from storage to GPU memory
 
 A major design difference from the original safetensors file loader is *NOT* to use `mmap`.
 It loads tensors on-demand with mmap'ed files,
```

### Comparing `fastsafetensors-0.1.0/README.md` & `fastsafetensors-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-fastsafetensors is a reimplementation of safetensors model loader to improve efficiency.
+fastsafetensors is an efficient safetensors model loader.
 We introduced three major features to optimize model loading performance:
 1. Batched, lazy tensor instantiations
 2. GPU offloading for sharding, type conversions, and device pointer alignment.
 3. GPU Direct Storage enablement for file loading from storage to GPU memory
 
 A major design difference from the original safetensors file loader is *NOT* to use `mmap`.
 It loads tensors on-demand with mmap'ed files,
@@ -50,8 +50,8 @@
 ```bash
 make install-test # install stub'ed fastsafetensors without torch, cuda, and numa
 make unittest
 ```
 
 ## Sample code
 
-see `example/load.py`
+see `example/load.py`
```

### Comparing `fastsafetensors-0.1.0/fastsafetensors/common.py` & `fastsafetensors-0.1.1/fastsafetensors/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,15 @@
             t2 = torch.from_dlpack(from_cuda_buffer(dst_dev_ptr, t.shape, t.strides, t.dtype, device))
             if dtype is not None and dtype != t.dtype:
                 if dtype.itemsize > t.dtype.itemsize:
                     raise Exception(f"Online type conversion to larger sizes is not supported ({t.dtype} -> {dtype})")
                 t3 = t2.to(dtype=dtype)
                 t2 = torch.from_dlpack(from_cuda_buffer(dst_dev_ptr, t.shape, t.strides, dtype, device))
                 t2.copy_(t3)
+                self.tensors[tensor_name].dtype = dtype
             ret[tensor_name] = t2
         return ret
 
     def __repr__(self)->str:
         return str({"__metadata__": self.metadata, "tensors": self.tensors})
 
 class TensorFrame:
```

### Comparing `fastsafetensors-0.1.0/fastsafetensors/connectors/tgis_weights.py` & `fastsafetensors-0.1.1/fastsafetensors/connectors/tgis_weights.py`

 * *Files identical despite different names*

### Comparing `fastsafetensors-0.1.0/fastsafetensors/copier/gds.py` & `fastsafetensors-0.1.1/fastsafetensors/copier/gds.py`

 * *Files identical despite different names*

### Comparing `fastsafetensors-0.1.0/fastsafetensors/copier/nogds.py` & `fastsafetensors-0.1.1/fastsafetensors/copier/nogds.py`

 * *Files identical despite different names*

### Comparing `fastsafetensors-0.1.0/fastsafetensors/cpp/ext.cpp` & `fastsafetensors-0.1.1/fastsafetensors/cpp/ext.cpp`

 * *Files identical despite different names*

### Comparing `fastsafetensors-0.1.0/fastsafetensors/cpp/ext.hpp` & `fastsafetensors-0.1.1/fastsafetensors/cpp/ext.hpp`

 * *Files identical despite different names*

### Comparing `fastsafetensors-0.1.0/fastsafetensors/dlpack.py` & `fastsafetensors-0.1.1/fastsafetensors/dlpack.py`

 * *Files identical despite different names*

### Comparing `fastsafetensors-0.1.0/fastsafetensors/file_buffer.py` & `fastsafetensors-0.1.1/fastsafetensors/file_buffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             else:
                 rank_lidixs[ranklidx] = [tensor_name]
         ts: List[torch.Tensor] = []
         for (rank, lidix), tns in sorted(rank_lidixs.items(), key=lambda x:x[0]):
             ts.append(self.rank_loaders[rank][lidix].shuffle_multi_cols(self.pg, tns, dim))
         if len(ts) == 1:
             # fastpath: tensors at the same layer are often in the same file
-            return self._get_tensor(rank, lidix, rank_lidixs[(rank, lidix)], ts[0], device, dtype)
+            return self._get_tensor(rank, lidix, rank_lidixs[(rank, lidix)][0], ts[0], device, dtype)
         ret = torch.cat(ts, dim=dim)
         if self.auto_mem_delete:
             for tensor_name in tensor_names:
                 (rank, lidx) = self._get_rank_lidx(tensor_name)
                 loader = self.rank_loaders[rank][lidix]
                 self.instantiated[rank][lidx][tensor_name] = True
                 if len(self.instantiated[rank][lidx]) == len(loader.metadata.tensors):
```

### Comparing `fastsafetensors-0.1.0/fastsafetensors/loader.py` & `fastsafetensors-0.1.1/fastsafetensors/loader.py`

 * *Files identical despite different names*

### Comparing `fastsafetensors-0.1.0/fastsafetensors/tensor_factory.py` & `fastsafetensors-0.1.1/fastsafetensors/tensor_factory.py`

 * *Files identical despite different names*

### Comparing `fastsafetensors-0.1.0/fastsafetensors.egg-info/PKG-INFO` & `fastsafetensors-0.1.1/fastsafetensors.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastsafetensors
-Version: 0.1.0
+Version: 0.1.1
 Summary: High-performance safetensors model loader
 Author-email: Takeshi Yoshimura <tyos@jp.ibm.com>
 Maintainer-email: Takeshi Yoshimura <tyos@jp.ibm.com>
 License: Apache-2.0
 Project-URL: Repository, https://github.com/foundation-model-stack/fastsafetensors
 Keywords: fastsafetensors,safetensors,GDS
 Requires-Python: >=3.10
@@ -14,15 +14,15 @@
 Requires-Dist: torch<2.3,>=2.1
 Provides-Extra: test
 Requires-Dist: pytest>=8.1.1; extra == "test"
 Requires-Dist: pytest-cov>=5.0.0; extra == "test"
 Requires-Dist: transformers>=4.40.2; extra == "test"
 Requires-Dist: safetensors>=0.4.0; extra == "test"
 
-fastsafetensors is a reimplementation of safetensors model loader to improve efficiency.
+fastsafetensors is an efficient safetensors model loader.
 We introduced three major features to optimize model loading performance:
 1. Batched, lazy tensor instantiations
 2. GPU offloading for sharding, type conversions, and device pointer alignment.
 3. GPU Direct Storage enablement for file loading from storage to GPU memory
 
 A major design difference from the original safetensors file loader is *NOT* to use `mmap`.
 It loads tensors on-demand with mmap'ed files,
```

### Comparing `fastsafetensors-0.1.0/fastsafetensors.egg-info/SOURCES.txt` & `fastsafetensors-0.1.1/fastsafetensors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastsafetensors-0.1.0/pyproject.toml` & `fastsafetensors-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fastsafetensors"
-version = "0.1.0"
+version = "0.1.1"
 description = "High-performance safetensors model loader"
 authors = [{name = "Takeshi Yoshimura", email = "tyos@jp.ibm.com"}]
 maintainers = [{name = "Takeshi Yoshimura", email = "tyos@jp.ibm.com"}]
 readme = "README.md"
 license = {text = "Apache-2.0"}
 keywords = ["fastsafetensors", "safetensors", "GDS"]
 requires-python = ">= 3.10"
```

### Comparing `fastsafetensors-0.1.0/setup.py` & `fastsafetensors-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `fastsafetensors-0.1.0/tests/test_fastsfaetensors.py` & `fastsafetensors-0.1.1/tests/test_fastsfaetensors.py`

 * *Files identical despite different names*

