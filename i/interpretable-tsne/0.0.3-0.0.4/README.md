# Comparing `tmp/interpretable_tsne-0.0.3.tar.gz` & `tmp/interpretable_tsne-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interpretable_tsne-0.0.3.tar", last modified: Mon Apr 22 18:28:54 2024, max compression
+gzip compressed data, was "interpretable_tsne-0.0.4.tar", last modified: Mon May 27 15:57:58 2024, max compression
```

## Comparing `interpretable_tsne-0.0.3.tar` & `interpretable_tsne-0.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrws---   0 sciclun4 (3067443)    65534        0 2024-04-22 18:28:54.000000 interpretable_tsne-0.0.3/
--rw-r--r--   0 sciclun4 (3067443)    65534     1487 2023-04-25 18:17:18.000000 interpretable_tsne-0.0.3/COPYING
--rw-r--r--   0 sciclun4 (3067443)    65534      319 2023-04-28 15:14:09.000000 interpretable_tsne-0.0.3/MANIFEST.in
--rw-r--r--   0 sciclun4 (3067443)    65534     4585 2024-04-22 18:28:54.000000 interpretable_tsne-0.0.3/PKG-INFO
--rw-rw----   0 sciclun4 (3067443)    65534     2114 2023-06-21 15:24:28.000000 interpretable_tsne-0.0.3/README.md
--rw-r--r--   0 sciclun4 (3067443)    65534      999 2024-04-22 18:28:16.000000 interpretable_tsne-0.0.3/pyproject.toml
--rw-rw----   0 sciclun4 (3067443)    65534      401 2024-04-22 18:28:54.000000 interpretable_tsne-0.0.3/setup.cfg
--rw-rw----   0 sciclun4 (3067443)    65534     1246 2024-04-22 16:53:10.000000 interpretable_tsne-0.0.3/setup.py
-drwxrws---   0 sciclun4 (3067443)    65534        0 2024-04-22 18:28:53.000000 interpretable_tsne-0.0.3/src/
-drwxrws---   0 sciclun4 (3067443)    65534        0 2024-04-22 18:28:54.000000 interpretable_tsne-0.0.3/src/interpretable_tsne/
--rw-r--r--   0 sciclun4 (3067443)    65534        0 2023-04-25 18:40:54.000000 interpretable_tsne-0.0.3/src/interpretable_tsne/__init__.py
--rw-rw----   0 sciclun4 (3067443)    65534  1235256 2024-04-22 18:28:45.000000 interpretable_tsne-0.0.3/src/interpretable_tsne/_barnes_hut_tsne.c
--rw-r--r--   0 sciclun4 (3067443)    65534    11733 2024-04-22 16:20:04.000000 interpretable_tsne-0.0.3/src/interpretable_tsne/_barnes_hut_tsne.pyx
--rw-rw----   0 sciclun4 (3067443)    65534   442194 2024-04-22 18:28:46.000000 interpretable_tsne-0.0.3/src/interpretable_tsne/_bintree.c
--rw-r--r--   0 sciclun4 (3067443)    65534     4482 2023-04-25 17:32:08.000000 interpretable_tsne-0.0.3/src/interpretable_tsne/_bintree.pyx
--rw-rw----   0 sciclun4 (3067443)    65534  1381366 2024-04-22 18:28:48.000000 interpretable_tsne-0.0.3/src/interpretable_tsne/_grad_comps.c
--rw-r--r--   0 sciclun4 (3067443)    65534    19866 2024-04-22 16:21:58.000000 interpretable_tsne-0.0.3/src/interpretable_tsne/_grad_comps.pyx
--rw-rw----   0 sciclun4 (3067443)    65534  1613259 2024-04-22 18:28:51.000000 interpretable_tsne-0.0.3/src/interpretable_tsne/_quad_tree.c
--rw-r--r--   0 sciclun4 (3067443)    65534     4372 2023-04-25 17:32:08.000000 interpretable_tsne-0.0.3/src/interpretable_tsne/_quad_tree.pxd
--rw-r--r--   0 sciclun4 (3067443)    65534    23710 2024-04-22 16:16:16.000000 interpretable_tsne-0.0.3/src/interpretable_tsne/_quad_tree.pyx
--rw-rw----   0 sciclun4 (3067443)    65534   677260 2024-04-22 18:28:51.000000 interpretable_tsne-0.0.3/src/interpretable_tsne/_utils.c
--rw-r--r--   0 sciclun4 (3067443)    65534     4507 2024-04-22 16:18:01.000000 interpretable_tsne-0.0.3/src/interpretable_tsne/_utils.pxd
--rw-rw----   0 sciclun4 (3067443)    65534    16809 2024-04-22 13:10:35.000000 interpretable_tsne-0.0.3/src/interpretable_tsne/_utils.pyx
--rw-rw----   0 sciclun4 (3067443)    65534    57775 2024-04-22 18:03:17.000000 interpretable_tsne-0.0.3/src/interpretable_tsne/tsne.py
--rw-r--r--   0 sciclun4 (3067443)    65534     8641 2023-07-01 20:43:02.000000 interpretable_tsne-0.0.3/src/interpretable_tsne/umap.py
-drwxrws---   0 sciclun4 (3067443)    65534        0 2024-04-22 18:28:54.000000 interpretable_tsne-0.0.3/src/interpretable_tsne.egg-info/
--rw-r--r--   0 sciclun4 (3067443)    65534     4585 2024-04-22 18:28:53.000000 interpretable_tsne-0.0.3/src/interpretable_tsne.egg-info/PKG-INFO
--rw-rw----   0 sciclun4 (3067443)    65534      881 2024-04-22 18:28:53.000000 interpretable_tsne-0.0.3/src/interpretable_tsne.egg-info/SOURCES.txt
--rw-rw----   0 sciclun4 (3067443)    65534        1 2024-04-22 18:28:53.000000 interpretable_tsne-0.0.3/src/interpretable_tsne.egg-info/dependency_links.txt
--rw-rw----   0 sciclun4 (3067443)    65534       46 2024-04-22 18:28:53.000000 interpretable_tsne-0.0.3/src/interpretable_tsne.egg-info/requires.txt
--rw-rw----   0 sciclun4 (3067443)    65534       19 2024-04-22 18:28:53.000000 interpretable_tsne-0.0.3/src/interpretable_tsne.egg-info/top_level.txt
-drwxrws---   0 sciclun4 (3067443)    65534        0 2024-04-22 18:28:54.000000 interpretable_tsne-0.0.3/tests/
--rw-rw----   0 sciclun4 (3067443)    65534     6295 2024-04-22 17:19:04.000000 interpretable_tsne-0.0.3/tests/test_bn_approx.py
--rw-rw----   0 sciclun4 (3067443)    65534    12840 2023-05-02 14:46:28.000000 interpretable_tsne-0.0.3/tests/test_gradcomps.py
+drwxrws---   0 sciclun4 (3067443)    65534        0 2024-05-27 15:57:58.000000 interpretable_tsne-0.0.4/
+-rw-r--r--   0 sciclun4 (3067443)    65534     1487 2023-04-25 18:17:18.000000 interpretable_tsne-0.0.4/COPYING
+-rw-r--r--   0 sciclun4 (3067443)    65534      319 2023-04-28 15:14:09.000000 interpretable_tsne-0.0.4/MANIFEST.in
+-rw-r--r--   0 sciclun4 (3067443)    65534     4587 2024-05-27 15:57:58.000000 interpretable_tsne-0.0.4/PKG-INFO
+-rw-rw----   0 sciclun4 (3067443)    65534     2114 2023-06-21 15:24:28.000000 interpretable_tsne-0.0.4/README.md
+-rw-rw----   0 sciclun4 (3067443)    65534     1002 2024-05-27 15:21:50.000000 interpretable_tsne-0.0.4/pyproject.toml
+-rw-rw----   0 sciclun4 (3067443)    65534      401 2024-05-27 15:57:58.000000 interpretable_tsne-0.0.4/setup.cfg
+-rw-rw----   0 sciclun4 (3067443)    65534     1246 2024-04-22 16:53:10.000000 interpretable_tsne-0.0.4/setup.py
+drwxrws---   0 sciclun4 (3067443)    65534        0 2024-05-27 15:57:58.000000 interpretable_tsne-0.0.4/src/
+drwxrws---   0 sciclun4 (3067443)    65534        0 2024-05-27 15:57:58.000000 interpretable_tsne-0.0.4/src/interpretable_tsne/
+-rw-r--r--   0 sciclun4 (3067443)    65534        0 2023-04-25 18:40:54.000000 interpretable_tsne-0.0.4/src/interpretable_tsne/__init__.py
+-rw-rw----   0 sciclun4 (3067443)    65534  1234973 2024-05-27 15:57:50.000000 interpretable_tsne-0.0.4/src/interpretable_tsne/_barnes_hut_tsne.c
+-rw-r--r--   0 sciclun4 (3067443)    65534    11733 2024-04-22 16:20:04.000000 interpretable_tsne-0.0.4/src/interpretable_tsne/_barnes_hut_tsne.pyx
+-rw-rw----   0 sciclun4 (3067443)    65534   441912 2024-05-27 15:57:51.000000 interpretable_tsne-0.0.4/src/interpretable_tsne/_bintree.c
+-rw-r--r--   0 sciclun4 (3067443)    65534     4482 2023-04-25 17:32:08.000000 interpretable_tsne-0.0.4/src/interpretable_tsne/_bintree.pyx
+-rw-rw----   0 sciclun4 (3067443)    65534  1381083 2024-05-27 15:57:52.000000 interpretable_tsne-0.0.4/src/interpretable_tsne/_grad_comps.c
+-rw-r--r--   0 sciclun4 (3067443)    65534    19866 2024-04-22 16:21:58.000000 interpretable_tsne-0.0.4/src/interpretable_tsne/_grad_comps.pyx
+-rw-rw----   0 sciclun4 (3067443)    65534  1630657 2024-05-27 15:57:53.000000 interpretable_tsne-0.0.4/src/interpretable_tsne/_quad_tree.c
+-rw-r--r--   0 sciclun4 (3067443)    65534     4372 2023-04-25 17:32:08.000000 interpretable_tsne-0.0.4/src/interpretable_tsne/_quad_tree.pxd
+-rw-r--r--   0 sciclun4 (3067443)    65534    23710 2024-04-22 16:16:16.000000 interpretable_tsne-0.0.4/src/interpretable_tsne/_quad_tree.pyx
+-rw-rw----   0 sciclun4 (3067443)    65534   693608 2024-05-27 15:57:54.000000 interpretable_tsne-0.0.4/src/interpretable_tsne/_utils.c
+-rw-r--r--   0 sciclun4 (3067443)    65534     4507 2024-04-22 16:18:01.000000 interpretable_tsne-0.0.4/src/interpretable_tsne/_utils.pxd
+-rw-rw----   0 sciclun4 (3067443)    65534    16809 2024-04-22 13:10:35.000000 interpretable_tsne-0.0.4/src/interpretable_tsne/_utils.pyx
+-rw-rw----   0 sciclun4 (3067443)    65534    57775 2024-04-22 18:03:17.000000 interpretable_tsne-0.0.4/src/interpretable_tsne/tsne.py
+-rw-r--r--   0 sciclun4 (3067443)    65534     8641 2023-07-01 20:43:02.000000 interpretable_tsne-0.0.4/src/interpretable_tsne/umap.py
+drwxrws---   0 sciclun4 (3067443)    65534        0 2024-05-27 15:57:58.000000 interpretable_tsne-0.0.4/src/interpretable_tsne.egg-info/
+-rw-r--r--   0 sciclun4 (3067443)    65534     4587 2024-05-27 15:57:57.000000 interpretable_tsne-0.0.4/src/interpretable_tsne.egg-info/PKG-INFO
+-rw-rw----   0 sciclun4 (3067443)    65534      881 2024-05-27 15:57:58.000000 interpretable_tsne-0.0.4/src/interpretable_tsne.egg-info/SOURCES.txt
+-rw-rw----   0 sciclun4 (3067443)    65534        1 2024-05-27 15:57:57.000000 interpretable_tsne-0.0.4/src/interpretable_tsne.egg-info/dependency_links.txt
+-rw-rw----   0 sciclun4 (3067443)    65534       48 2024-05-27 15:57:57.000000 interpretable_tsne-0.0.4/src/interpretable_tsne.egg-info/requires.txt
+-rw-rw----   0 sciclun4 (3067443)    65534       19 2024-05-27 15:57:57.000000 interpretable_tsne-0.0.4/src/interpretable_tsne.egg-info/top_level.txt
+drwxrws---   0 sciclun4 (3067443)    65534        0 2024-05-27 15:57:58.000000 interpretable_tsne-0.0.4/tests/
+-rw-rw----   0 sciclun4 (3067443)    65534     6319 2024-05-27 15:02:49.000000 interpretable_tsne-0.0.4/tests/test_bn_approx.py
+-rw-rw----   0 sciclun4 (3067443)    65534    12860 2024-05-27 15:02:50.000000 interpretable_tsne-0.0.4/tests/test_gradcomps.py
```

### Comparing `interpretable_tsne-0.0.3/COPYING` & `interpretable_tsne-0.0.4/COPYING`

 * *Files identical despite different names*

### Comparing `interpretable_tsne-0.0.3/PKG-INFO` & `interpretable_tsne-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: interpretable_tsne
-Version: 0.0.3
-Summary: Implementation of the gradient-based t-SNE sttribution method described in our GLBIO oral presentation: 'Towards Computing Attributions for Dimensionality Reduction Techniques'
+Version: 0.0.4
+Summary: Implementation of the gradient-based t-SNE attribution method described in our GLBIO oral presentation: 'Towards Computing Attributions for Dimensionality Reduction Techniques'
 Author: Matthew Scicluna
 Author-email: Matthew Scicluna <mattcscicluna@gmail.com>
 Maintainer-email: Matthew Scicluna <mattcscicluna@gmail.com>
 License: BSD 3-Clause License
         
         Copyright 2023 Matthew Scicluna.
         
@@ -19,20 +19,20 @@
         
         THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 Project-URL: Repository, https://github.com/MattScicluna/interpretable_tsne.git
 Project-URL: Bug Tracker, https://github.com/MattScicluna/interpretable_tsne/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: COPYING
-Requires-Dist: scikit-learn==0.24.1
-Requires-Dist: scipy==1.7.0
-Requires-Dist: numpy==1.21
+Requires-Dist: scikit-learn>=0.23.0
+Requires-Dist: scipy>=1.5.0
+Requires-Dist: numpy>=1.19.2
 
 Interpretable t-SNE
 ===================
 
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
 `interpretable_tsne` is an implementation of our gradient-based attributiont technique described in our GLBIO oral presentation: 'Towards Computing Attributions for Dimensionality Reduction Techniques'.
```

### Comparing `interpretable_tsne-0.0.3/README.md` & `interpretable_tsne-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `interpretable_tsne-0.0.3/pyproject.toml` & `interpretable_tsne-0.0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [build-system]
-requires = ["setuptools>=61.0", "wheel", "Cython", "numpy==1.21"]
+requires = ["setuptools>=61.0", "wheel", "Cython", "numpy>=1.19.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "interpretable_tsne"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Matthew Scicluna", email="mattcscicluna@gmail.com" }
 ]
 maintainers = [
   { name="Matthew Scicluna", email="mattcscicluna@gmail.com" }
 ]
 
-description = "Implementation of the gradient-based t-SNE sttribution method described in our GLBIO oral presentation: 'Towards Computing Attributions for Dimensionality Reduction Techniques'"
+description = "Implementation of the gradient-based t-SNE attribution method described in our GLBIO oral presentation: 'Towards Computing Attributions for Dimensionality Reduction Techniques'"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.7"
 license = {file = "COPYING"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  'scikit-learn==0.24.1',
-  'scipy==1.7.0',
-  'numpy==1.21',
+  "scikit-learn>=0.23.0",
+  "scipy>=1.5.0",
+  "numpy>=1.19.2"
 ]
 
 [project.urls]
 "Repository" = "https://github.com/MattScicluna/interpretable_tsne.git"
 "Bug Tracker" = "https://github.com/MattScicluna/interpretable_tsne/issues"
```

### Comparing `interpretable_tsne-0.0.3/setup.py` & `interpretable_tsne-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `interpretable_tsne-0.0.3/src/interpretable_tsne/_barnes_hut_tsne.c` & `interpretable_tsne-0.0.4/src/interpretable_tsne/_barnes_hut_tsne.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include"
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include"
         ],
         "name": "interpretable_tsne._barnes_hut_tsne",
         "sources": [
             "src/interpretable_tsne/_barnes_hut_tsne.pyx"
         ]
     },
     "module_name": "interpretable_tsne._barnes_hut_tsne"
@@ -1672,195 +1672,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":734
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":735
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":741
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":742
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":746
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":747
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":756
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
+ * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   longlong_t
- * 
- */
-typedef npy_longlong __pyx_t_5numpy_long_t;
-
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":758
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
+ * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulonglong_t
- * 
- */
-typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
-
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":762
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1930,42 +1912,42 @@
 /*--- Type declarations ---*/
 struct __pyx_obj_18interpretable_tsne_10_quad_tree__QuadTree;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":772
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":775
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -18265,261 +18247,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":246
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":249
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":246
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":252
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":255
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":252
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":258
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":261
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":258
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":264
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":269
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":264
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":272
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":276
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":272
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":279
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":282
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":279
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":285
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":291
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":285
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":777
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18528,29 +18510,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":778
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 778, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18561,15 +18543,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":780
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18578,29 +18560,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":781
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 781, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18611,15 +18593,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":783
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18628,29 +18610,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":784
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 784, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18661,15 +18643,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":786
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18678,29 +18660,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":787
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 787, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18711,15 +18693,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":789
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18728,29 +18710,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":790
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 790, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18761,209 +18743,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":792
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":793
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":794
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":793
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":796
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_L0:;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":975
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":977
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":978
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":977
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":983
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18979,15 +18969,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18995,68 +18985,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":985
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 985, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 986, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 987, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 987, __pyx_L5_except_error)
+      __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":984
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19064,15 +19054,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19087,15 +19077,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":989
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19111,15 +19101,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19127,68 +19117,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":991
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 991, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 992, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 993, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 993, __pyx_L5_except_error)
+      __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":990
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19196,15 +19186,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19219,15 +19209,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":995
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19243,15 +19233,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":996
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19259,68 +19249,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":997
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 997, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":998
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 998, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":999
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 999, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 999, __pyx_L5_except_error)
+      __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":996
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19328,15 +19318,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":995
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19351,170 +19341,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1002
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1002
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1017
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1017
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1032
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1032
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1042
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1049
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1053
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -23307,15 +23297,15 @@
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 141, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 156, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 159, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 408, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 618, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 914, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 987, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 984, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
@@ -23354,33 +23344,33 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 987, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 993, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 990, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
   /* "View.MemoryView":100
  * cdef object __pyx_collections_abc_Sequence "__pyx_collections_abc_Sequence"
  * try:
  *     if __import__("sys").version_info >= (3, 3):             # <<<<<<<<<<<<<<
@@ -23745,31 +23735,31 @@
   #elif CYTHON_COMPILING_IN_LIMITED_API
   sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 203, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 203, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 230, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 829, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 831, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 869, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 866, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("interpretable_tsne._quad_tree"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_18interpretable_tsne_10_quad_tree__QuadTree = __Pyx_ImportType_3_0_10(__pyx_t_1, "interpretable_tsne._quad_tree", "_QuadTree", sizeof(struct __pyx_obj_18interpretable_tsne_10_quad_tree__QuadTree), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_18interpretable_tsne_10_quad_tree__QuadTree),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_18interpretable_tsne_10_quad_tree__QuadTree) __PYX_ERR(4, 50, __pyx_L1_error)
   __pyx_vtabptr_18interpretable_tsne_10_quad_tree__QuadTree = (struct __pyx_vtabstruct_18interpretable_tsne_10_quad_tree__QuadTree*)__Pyx_GetVtable(__pyx_ptype_18interpretable_tsne_10_quad_tree__QuadTree); if (unlikely(!__pyx_vtabptr_18interpretable_tsne_10_quad_tree__QuadTree)) __PYX_ERR(4, 50, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
```

### Comparing `interpretable_tsne-0.0.3/src/interpretable_tsne/_barnes_hut_tsne.pyx` & `interpretable_tsne-0.0.4/src/interpretable_tsne/_barnes_hut_tsne.pyx`

 * *Files identical despite different names*

### Comparing `interpretable_tsne-0.0.3/src/interpretable_tsne/_bintree.c` & `interpretable_tsne-0.0.4/src/interpretable_tsne/_bintree.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/npy_math.h",
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/npy_math.h",
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include"
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include"
         ],
         "name": "interpretable_tsne._bintree",
         "sources": [
             "src/interpretable_tsne/_bintree.pyx"
         ]
     },
     "module_name": "interpretable_tsne._bintree"
@@ -1567,195 +1567,177 @@
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":734
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":735
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":741
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":742
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":746
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":747
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":756
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
+ * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   longlong_t
- * 
- */
-typedef npy_longlong __pyx_t_5numpy_long_t;
-
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":758
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
+ * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulonglong_t
- * 
- */
-typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
-
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":762
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1784,42 +1766,42 @@
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":772
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":775
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3057,261 +3039,261 @@
 #define __pyx_n_s_zeros __pyx_mstate_global->__pyx_n_s_zeros
 #define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
 #define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
 #define __pyx_tuple__5 __pyx_mstate_global->__pyx_tuple__5
 #define __pyx_codeobj__6 __pyx_mstate_global->__pyx_codeobj__6
 /* #### Code section: module_code ### */
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":246
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":249
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":246
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":252
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":255
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":252
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":258
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":261
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":258
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":264
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":269
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":264
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":272
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":276
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":272
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":279
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":282
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":279
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":285
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":291
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":285
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":777
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3320,29 +3302,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":778
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 778, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3353,15 +3335,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":780
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3370,29 +3352,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":781
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 781, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3403,15 +3385,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":783
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3420,29 +3402,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":784
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 784, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3453,15 +3435,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":786
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3470,29 +3452,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":787
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 787, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3503,15 +3485,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":789
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3520,29 +3502,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":790
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 790, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3553,209 +3535,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":792
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":793
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":794
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":793
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":796
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 970, __pyx_L1_error)
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_L0:;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":975
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":977
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":978
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":977
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":983
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3771,15 +3761,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -3787,68 +3777,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":985
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 985, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 982, __pyx_L3_error)
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 986, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 987, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 987, __pyx_L5_except_error)
+      __PYX_ERR(1, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":984
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -3856,15 +3846,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3879,15 +3869,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":989
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3903,15 +3893,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3919,68 +3909,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":991
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 991, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 988, __pyx_L3_error)
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 992, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 993, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 993, __pyx_L5_except_error)
+      __PYX_ERR(1, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":990
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -3988,15 +3978,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4011,15 +4001,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":995
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4035,15 +4025,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":996
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4051,68 +4041,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":997
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 997, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 994, __pyx_L3_error)
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":998
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 998, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":999
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 999, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 999, __pyx_L5_except_error)
+      __PYX_ERR(1, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":996
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4120,15 +4110,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":995
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4143,170 +4133,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1002
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1002
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1017
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1017
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1032
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1032
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1042
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1049
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1053
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -5431,44 +5421,44 @@
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 80, __pyx_L1_error)
   __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 127, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 987, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 984, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 987, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 993, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 990, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "interpretable_tsne/_bintree.pyx":26
  * cdef float PERPLEXITY_TOLERANCE = 1e-5
  * 
  * cpdef _binary_search_perplexity(             # <<<<<<<<<<<<<<
@@ -5556,31 +5546,31 @@
   #elif CYTHON_COMPILING_IN_LIMITED_API
   sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 203, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 203, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 230, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 829, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 831, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 869, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 866, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
```

### Comparing `interpretable_tsne-0.0.3/src/interpretable_tsne/_bintree.pyx` & `interpretable_tsne-0.0.4/src/interpretable_tsne/_bintree.pyx`

 * *Files identical despite different names*

### Comparing `interpretable_tsne-0.0.3/src/interpretable_tsne/_grad_comps.c` & `interpretable_tsne-0.0.4/src/interpretable_tsne/_grad_comps.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include"
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include"
         ],
         "name": "interpretable_tsne._grad_comps",
         "sources": [
             "src/interpretable_tsne/_grad_comps.pyx"
         ]
     },
     "module_name": "interpretable_tsne._grad_comps"
@@ -1672,195 +1672,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":734
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":735
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":741
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":742
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":746
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":747
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":756
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
+ * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   longlong_t
- * 
- */
-typedef npy_longlong __pyx_t_5numpy_long_t;
-
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":758
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
+ * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulonglong_t
- * 
- */
-typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
-
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":762
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1930,42 +1912,42 @@
 /*--- Type declarations ---*/
 struct __pyx_obj_18interpretable_tsne_10_quad_tree__QuadTree;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":772
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":775
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -18400,261 +18382,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":246
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":249
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":246
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":252
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":255
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":252
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":258
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":261
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":258
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":264
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":269
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":264
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":272
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":276
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":272
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":279
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":282
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":279
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":285
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":291
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":285
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":777
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18663,29 +18645,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":778
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 778, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18696,15 +18678,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":780
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18713,29 +18695,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":781
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 781, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18746,15 +18728,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":783
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18763,29 +18745,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":784
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 784, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18796,15 +18778,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":786
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18813,29 +18795,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":787
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 787, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18846,15 +18828,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":789
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18863,29 +18845,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":790
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 790, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18896,209 +18878,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":792
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":793
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":794
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":793
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":796
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_L0:;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":975
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":977
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":978
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":977
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":983
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19114,15 +19104,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -19130,68 +19120,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":985
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 985, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 986, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 987, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 987, __pyx_L5_except_error)
+      __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":984
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19199,15 +19189,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19222,15 +19212,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":989
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19246,15 +19236,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19262,68 +19252,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":991
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 991, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 992, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 993, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 993, __pyx_L5_except_error)
+      __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":990
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19331,15 +19321,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19354,15 +19344,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":995
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19378,15 +19368,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":996
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19394,68 +19384,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":997
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 997, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":998
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 998, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":999
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 999, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 999, __pyx_L5_except_error)
+      __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":996
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19463,15 +19453,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":995
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19486,170 +19476,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1002
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1002
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1017
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1017
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1032
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1032
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1042
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1049
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1053
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -25828,15 +25818,15 @@
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 156, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 159, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(1, 373, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 408, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 618, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 914, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 987, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 984, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
@@ -25875,33 +25865,33 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 987, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 993, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 990, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
   /* "View.MemoryView":100
  * cdef object __pyx_collections_abc_Sequence "__pyx_collections_abc_Sequence"
  * try:
  *     if __import__("sys").version_info >= (3, 3):             # <<<<<<<<<<<<<<
@@ -26289,31 +26279,31 @@
   #elif CYTHON_COMPILING_IN_LIMITED_API
   sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 203, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 203, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 230, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 829, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 831, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 869, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 866, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("interpretable_tsne._quad_tree"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_18interpretable_tsne_10_quad_tree__QuadTree = __Pyx_ImportType_3_0_10(__pyx_t_1, "interpretable_tsne._quad_tree", "_QuadTree", sizeof(struct __pyx_obj_18interpretable_tsne_10_quad_tree__QuadTree), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_18interpretable_tsne_10_quad_tree__QuadTree),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_18interpretable_tsne_10_quad_tree__QuadTree) __PYX_ERR(4, 50, __pyx_L1_error)
   __pyx_vtabptr_18interpretable_tsne_10_quad_tree__QuadTree = (struct __pyx_vtabstruct_18interpretable_tsne_10_quad_tree__QuadTree*)__Pyx_GetVtable(__pyx_ptype_18interpretable_tsne_10_quad_tree__QuadTree); if (unlikely(!__pyx_vtabptr_18interpretable_tsne_10_quad_tree__QuadTree)) __PYX_ERR(4, 50, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
```

### Comparing `interpretable_tsne-0.0.3/src/interpretable_tsne/_grad_comps.pyx` & `interpretable_tsne-0.0.4/src/interpretable_tsne/_grad_comps.pyx`

 * *Files identical despite different names*

### Comparing `interpretable_tsne-0.0.3/src/interpretable_tsne/_quad_tree.c` & `interpretable_tsne-0.0.4/src/interpretable_tsne/_quad_tree.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include"
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include"
         ],
         "name": "interpretable_tsne._quad_tree",
         "sources": [
             "src/interpretable_tsne/_quad_tree.pyx"
         ]
     },
     "module_name": "interpretable_tsne._quad_tree"
@@ -1693,195 +1693,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":734
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":735
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":741
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":742
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":746
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":747
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":756
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
+ * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   longlong_t
- * 
- */
-typedef npy_longlong __pyx_t_5numpy_long_t;
-
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":758
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
+ * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulonglong_t
- * 
- */
-typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
-
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":762
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -2024,42 +2006,42 @@
  *     or the provided default value if no such value was found.
  */
 struct __pyx_opt_args_7cpython_11contextvars_get_value_no_default {
   int __pyx_n;
   PyObject *default_value;
 };
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":772
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":775
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3587,14 +3569,20 @@
 
 /* TypeInfoToFormat.proto */
 struct __pyx_typeinfo_string {
     char string[3];
 };
 static struct __pyx_typeinfo_string __Pyx_TypeInfoToFormat(__Pyx_TypeInfo *type);
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_Py_intptr_t(Py_intptr_t value);
+
+/* CIntFromPy.proto */
+static CYTHON_INLINE Py_intptr_t __Pyx_PyInt_As_Py_intptr_t(PyObject *);
+
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntToPy.proto */
@@ -5776,15 +5764,15 @@
     /* "carray.to_py":119
  *     l = PyList_New(length)
  *     for i in range(<size_t>length):
  *         value = v[i]             # <<<<<<<<<<<<<<
  *         Py_INCREF(value)
  *         PyList_SET_ITEM(l, i, value)
  */
-    __pyx_t_1 = PyInt_FromSsize_t((__pyx_v_v[__pyx_v_i])); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 119, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t((__pyx_v_v[__pyx_v_i])); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 119, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_1);
     __pyx_t_1 = 0;
 
     /* "carray.to_py":120
  *     for i in range(<size_t>length):
  *         value = v[i]
@@ -5887,15 +5875,15 @@
     /* "carray.to_py":131
  *     t = PyTuple_New(length)
  *     for i in range(<size_t>length):
  *         value = v[i]             # <<<<<<<<<<<<<<
  *         Py_INCREF(value)
  *         PyTuple_SET_ITEM(t, i, value)
  */
-    __pyx_t_1 = PyInt_FromSsize_t((__pyx_v_v[__pyx_v_i])); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 131, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t((__pyx_v_v[__pyx_v_i])); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 131, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_1);
     __pyx_t_1 = 0;
 
     /* "carray.to_py":132
  *     for i in range(<size_t>length):
  *         value = v[i]
@@ -6384,15 +6372,15 @@
       /* "carray.from_py":89
  *             if i >= length:
  *                 break
  *             v[i] = item             # <<<<<<<<<<<<<<
  *         else:
  *             i += 1  # convert index to length
  */
-      __pyx_t_11 = __Pyx_PyIndex_AsSsize_t(__pyx_v_item); if (unlikely((__pyx_t_11 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(1, 89, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyInt_As_Py_intptr_t(__pyx_v_item); if (unlikely((__pyx_t_11 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(1, 89, __pyx_L1_error)
       (__pyx_v_v[__pyx_v_i]) = __pyx_t_11;
 
       /* "carray.from_py":86
  *         pass
  *     if i == length:
  *         for i, item in enumerate(o):             # <<<<<<<<<<<<<<
  *             if i >= length:
@@ -6985,15 +6973,15 @@
   /* "FromPyStructUtility":21
  *     except KeyError:
  *         raise ValueError("No value specified for struct attribute 'parent'")
  *     result.parent = value             # <<<<<<<<<<<<<<
  *     try:
  *         value = obj['children']
  */
-  __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_v_value); if (unlikely((__pyx_t_10 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(1, 21, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyInt_As_Py_intptr_t(__pyx_v_value); if (unlikely((__pyx_t_10 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(1, 21, __pyx_L1_error)
   __pyx_v_result.parent = __pyx_t_10;
 
   /* "FromPyStructUtility":22
  *         raise ValueError("No value specified for struct attribute 'parent'")
  *     result.parent = value
  *     try:             # <<<<<<<<<<<<<<
  *         value = obj['children']
@@ -7189,15 +7177,15 @@
   /* "FromPyStructUtility":31
  *     except KeyError:
  *         raise ValueError("No value specified for struct attribute 'cell_id'")
  *     result.cell_id = value             # <<<<<<<<<<<<<<
  *     try:
  *         value = obj['point_index']
  */
-  __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_v_value); if (unlikely((__pyx_t_10 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(1, 31, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyInt_As_Py_intptr_t(__pyx_v_value); if (unlikely((__pyx_t_10 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(1, 31, __pyx_L1_error)
   __pyx_v_result.cell_id = __pyx_t_10;
 
   /* "FromPyStructUtility":32
  *         raise ValueError("No value specified for struct attribute 'cell_id'")
  *     result.cell_id = value
  *     try:             # <<<<<<<<<<<<<<
  *         value = obj['point_index']
@@ -7291,15 +7279,15 @@
   /* "FromPyStructUtility":36
  *     except KeyError:
  *         raise ValueError("No value specified for struct attribute 'point_index'")
  *     result.point_index = value             # <<<<<<<<<<<<<<
  *     try:
  *         value = obj['is_leaf']
  */
-  __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_v_value); if (unlikely((__pyx_t_10 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(1, 36, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyInt_As_Py_intptr_t(__pyx_v_value); if (unlikely((__pyx_t_10 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(1, 36, __pyx_L1_error)
   __pyx_v_result.point_index = __pyx_t_10;
 
   /* "FromPyStructUtility":37
  *         raise ValueError("No value specified for struct attribute 'point_index'")
  *     result.point_index = value
  *     try:             # <<<<<<<<<<<<<<
  *         value = obj['is_leaf']
@@ -7597,15 +7585,15 @@
   /* "FromPyStructUtility":51
  *     except KeyError:
  *         raise ValueError("No value specified for struct attribute 'depth'")
  *     result.depth = value             # <<<<<<<<<<<<<<
  *     try:
  *         value = obj['cumulative_size']
  */
-  __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_v_value); if (unlikely((__pyx_t_10 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(1, 51, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyInt_As_Py_intptr_t(__pyx_v_value); if (unlikely((__pyx_t_10 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(1, 51, __pyx_L1_error)
   __pyx_v_result.depth = __pyx_t_10;
 
   /* "FromPyStructUtility":52
  *         raise ValueError("No value specified for struct attribute 'depth'")
  *     result.depth = value
  *     try:             # <<<<<<<<<<<<<<
  *         value = obj['cumulative_size']
@@ -7699,15 +7687,15 @@
   /* "FromPyStructUtility":56
  *     except KeyError:
  *         raise ValueError("No value specified for struct attribute 'cumulative_size'")
  *     result.cumulative_size = value             # <<<<<<<<<<<<<<
  *     try:
  *         value = obj['center']
  */
-  __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_v_value); if (unlikely((__pyx_t_10 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(1, 56, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyInt_As_Py_intptr_t(__pyx_v_value); if (unlikely((__pyx_t_10 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(1, 56, __pyx_L1_error)
   __pyx_v_result.cumulative_size = __pyx_t_10;
 
   /* "FromPyStructUtility":57
  *         raise ValueError("No value specified for struct attribute 'cumulative_size'")
  *     result.cumulative_size = value
  *     try:             # <<<<<<<<<<<<<<
  *         value = obj['center']
@@ -22139,261 +22127,261 @@
   __Pyx_XDECREF(__pyx_v_parts);
   __Pyx_XDECREF(__pyx_v_extents);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":246
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":249
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":246
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":252
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":255
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":252
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":258
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":261
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":258
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":264
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":269
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":264
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":272
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":276
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":272
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":279
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":282
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":279
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":285
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":291
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":285
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":777
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -22402,29 +22390,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":778
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 778, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -22435,15 +22423,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":780
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -22452,29 +22440,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":781
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 781, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -22485,15 +22473,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":783
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -22502,29 +22490,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":784
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 784, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -22535,15 +22523,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":786
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -22552,29 +22540,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":787
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 787, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -22585,15 +22573,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":789
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -22602,29 +22590,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":790
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 790, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -22635,209 +22623,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":792
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":793
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":794
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":793
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":796
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_L0:;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":975
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":977
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":978
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":977
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":983
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -22853,15 +22849,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -22869,68 +22865,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":985
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 985, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 986, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 987, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 987, __pyx_L5_except_error)
+      __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":984
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -22938,15 +22934,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -22961,15 +22957,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":989
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -22985,15 +22981,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -23001,68 +22997,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":991
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 991, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 992, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 993, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 993, __pyx_L5_except_error)
+      __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":990
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -23070,15 +23066,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -23093,15 +23089,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":995
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -23117,15 +23113,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":996
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -23133,68 +23129,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":997
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 997, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":998
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 998, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":999
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 999, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 999, __pyx_L5_except_error)
+      __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":996
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -23202,15 +23198,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":995
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -23225,170 +23221,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1002
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1002
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1017
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1017
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1032
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1032
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1042
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1049
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1053
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -24562,16 +24558,17 @@
   int __pyx_r;
   __pyx_t_18interpretable_tsne_10_quad_tree_SIZE_t __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
   __pyx_t_18interpretable_tsne_10_quad_tree_DTYPE_t __pyx_t_6;
-  struct __pyx_opt_args_18interpretable_tsne_10_quad_tree_9_QuadTree_insert_point __pyx_t_7;
-  struct __pyx_opt_args_18interpretable_tsne_10_quad_tree_9_QuadTree__insert_point_in_new_child __pyx_t_8;
+  long __pyx_t_7;
+  struct __pyx_opt_args_18interpretable_tsne_10_quad_tree_9_QuadTree_insert_point __pyx_t_8;
+  struct __pyx_opt_args_18interpretable_tsne_10_quad_tree_9_QuadTree__insert_point_in_new_child __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
   if (__pyx_optional_args) {
@@ -24786,16 +24783,16 @@
  *                 # barycenter update using a weighted mean
  *                 cell.barycenter[ax] = (
  *                     n_point * cell.barycenter[ax] + point[ax]) / (n_point + 1)             # <<<<<<<<<<<<<<
  * 
  *             # Increase the size of the subtree starting from this cell
  */
       __pyx_t_6 = ((__pyx_v_n_point * (__pyx_v_cell->barycenter[__pyx_v_ax])) + (__pyx_v_point[__pyx_v_ax]));
-      __pyx_t_1 = (__pyx_v_n_point + 1);
-      if (unlikely(__pyx_t_1 == 0)) {
+      __pyx_t_7 = (__pyx_v_n_point + 1);
+      if (unlikely(__pyx_t_7 == 0)) {
         #ifdef WITH_THREAD
         PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
         #endif
         PyErr_SetString(PyExc_ZeroDivisionError, "float division");
         #ifdef WITH_THREAD
         __Pyx_PyGILState_Release(__pyx_gilstate_save);
         #endif
@@ -24805,15 +24802,15 @@
       /* "interpretable_tsne/_quad_tree.pyx":146
  *             for ax in range(self.n_dimensions):
  *                 # barycenter update using a weighted mean
  *                 cell.barycenter[ax] = (             # <<<<<<<<<<<<<<
  *                     n_point * cell.barycenter[ax] + point[ax]) / (n_point + 1)
  * 
  */
-      (__pyx_v_cell->barycenter[__pyx_v_ax]) = (__pyx_t_6 / ((__pyx_t_18interpretable_tsne_10_quad_tree_DTYPE_t)__pyx_t_1));
+      (__pyx_v_cell->barycenter[__pyx_v_ax]) = (__pyx_t_6 / ((__pyx_t_18interpretable_tsne_10_quad_tree_DTYPE_t)__pyx_t_7));
     }
 
     /* "interpretable_tsne/_quad_tree.pyx":150
  * 
  *             # Increase the size of the subtree starting from this cell
  *             cell.cumulative_size += 1             # <<<<<<<<<<<<<<
  * 
@@ -24901,17 +24898,17 @@
     /* "interpretable_tsne/_quad_tree.pyx":159
  *                 self.n_points += 1
  *                 return self._insert_point_in_new_child(point, cell, point_index)
  *             return self.insert_point(point, point_index, selected_child)             # <<<<<<<<<<<<<<
  * 
  *         # Finally, if the cell is a leaf with a point already inserted,
  */
-    __pyx_t_7.__pyx_n = 1;
-    __pyx_t_7.cell_id = __pyx_v_selected_child;
-    __pyx_t_3 = ((struct __pyx_vtabstruct_18interpretable_tsne_10_quad_tree__QuadTree *)__pyx_v_self->__pyx_vtab)->insert_point(__pyx_v_self, __pyx_v_point, __pyx_v_point_index, &__pyx_t_7); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 159, __pyx_L1_error)
+    __pyx_t_8.__pyx_n = 1;
+    __pyx_t_8.cell_id = __pyx_v_selected_child;
+    __pyx_t_3 = ((struct __pyx_vtabstruct_18interpretable_tsne_10_quad_tree__QuadTree *)__pyx_v_self->__pyx_vtab)->insert_point(__pyx_v_self, __pyx_v_point, __pyx_v_point_index, &__pyx_t_8); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 159, __pyx_L1_error)
     __pyx_r = __pyx_t_3;
     goto __pyx_L0;
 
     /* "interpretable_tsne/_quad_tree.pyx":143
  *         # If the cell is not a leaf, update cell internals and
  *         # recurse in selected child
  *         if not cell.is_leaf:             # <<<<<<<<<<<<<<
@@ -24998,28 +24995,28 @@
   /* "interpretable_tsne/_quad_tree.pyx":173
  *         # In a leaf, the barycenter correspond to the only point included
  *         # in it.
  *         self._insert_point_in_new_child(cell.barycenter, cell, cell.point_index,             # <<<<<<<<<<<<<<
  *                                         cell.cumulative_size)
  *         return self.insert_point(point, point_index, cell_id)
  */
-  __pyx_t_8.__pyx_n = 1;
-  __pyx_t_8.size = __pyx_v_cell->cumulative_size;
-  ((struct __pyx_vtabstruct_18interpretable_tsne_10_quad_tree__QuadTree *)__pyx_v_self->__pyx_vtab)->_insert_point_in_new_child(__pyx_v_self, __pyx_v_cell->barycenter, __pyx_v_cell, __pyx_v_cell->point_index, &__pyx_t_8); if (unlikely(__Pyx_ErrOccurredWithGIL())) __PYX_ERR(0, 173, __pyx_L1_error)
+  __pyx_t_9.__pyx_n = 1;
+  __pyx_t_9.size = __pyx_v_cell->cumulative_size;
+  ((struct __pyx_vtabstruct_18interpretable_tsne_10_quad_tree__QuadTree *)__pyx_v_self->__pyx_vtab)->_insert_point_in_new_child(__pyx_v_self, __pyx_v_cell->barycenter, __pyx_v_cell, __pyx_v_cell->point_index, &__pyx_t_9); if (unlikely(__Pyx_ErrOccurredWithGIL())) __PYX_ERR(0, 173, __pyx_L1_error)
 
   /* "interpretable_tsne/_quad_tree.pyx":175
  *         self._insert_point_in_new_child(cell.barycenter, cell, cell.point_index,
  *                                         cell.cumulative_size)
  *         return self.insert_point(point, point_index, cell_id)             # <<<<<<<<<<<<<<
  * 
  *     # XXX: This operation is not Thread safe
  */
-  __pyx_t_7.__pyx_n = 1;
-  __pyx_t_7.cell_id = __pyx_v_cell_id;
-  __pyx_t_3 = ((struct __pyx_vtabstruct_18interpretable_tsne_10_quad_tree__QuadTree *)__pyx_v_self->__pyx_vtab)->insert_point(__pyx_v_self, __pyx_v_point, __pyx_v_point_index, &__pyx_t_7); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 175, __pyx_L1_error)
+  __pyx_t_8.__pyx_n = 1;
+  __pyx_t_8.cell_id = __pyx_v_cell_id;
+  __pyx_t_3 = ((struct __pyx_vtabstruct_18interpretable_tsne_10_quad_tree__QuadTree *)__pyx_v_self->__pyx_vtab)->insert_point(__pyx_v_self, __pyx_v_point, __pyx_v_point_index, &__pyx_t_8); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 175, __pyx_L1_error)
   __pyx_r = __pyx_t_3;
   goto __pyx_L0;
 
   /* "interpretable_tsne/_quad_tree.pyx":114
  *         self._resize(capacity=self.cell_count)
  * 
  *     cdef int insert_point(self, DTYPE_t[3] point, SIZE_t point_index,             # <<<<<<<<<<<<<<
@@ -25215,15 +25212,15 @@
   /* "interpretable_tsne/_quad_tree.pyx":212
  *         # Set the cell as an inner cell of the Tree
  *         cell.is_leaf = False
  *         cell.point_index = -1             # <<<<<<<<<<<<<<
  * 
  *         # Set the correct boundary for the cell, store the point in the cell
  */
-  __pyx_v_cell->point_index = -1L;
+  __pyx_v_cell->point_index = -1;
 
   /* "interpretable_tsne/_quad_tree.pyx":216
  *         # Set the correct boundary for the cell, store the point in the cell
  *         # and compute its index in the children array.
  *         cell_child_id = 0             # <<<<<<<<<<<<<<
  *         for i in range(self.n_dimensions):
  *             cell_child_id *= 2
@@ -25778,15 +25775,15 @@
   /* "interpretable_tsne/_quad_tree.pyx":291
  *             Cell* root = &self.cells[0]
  * 
  *         self._init_cell(root, -1, 0)             # <<<<<<<<<<<<<<
  *         for i in range(self.n_dimensions):
  *             root.min_bounds[i] = min_bounds[i]
  */
-  ((struct __pyx_vtabstruct_18interpretable_tsne_10_quad_tree__QuadTree *)__pyx_v_self->__pyx_vtab)->_init_cell(__pyx_v_self, __pyx_v_root, -1L, 0); if (unlikely(__Pyx_ErrOccurredWithGIL())) __PYX_ERR(0, 291, __pyx_L1_error)
+  ((struct __pyx_vtabstruct_18interpretable_tsne_10_quad_tree__QuadTree *)__pyx_v_self->__pyx_vtab)->_init_cell(__pyx_v_self, __pyx_v_root, -1, 0); if (unlikely(__Pyx_ErrOccurredWithGIL())) __PYX_ERR(0, 291, __pyx_L1_error)
 
   /* "interpretable_tsne/_quad_tree.pyx":292
  * 
  *         self._init_cell(root, -1, 0)
  *         for i in range(self.n_dimensions):             # <<<<<<<<<<<<<<
  *             root.min_bounds[i] = min_bounds[i]
  *             root.max_bounds[i] = max_bounds[i]
@@ -26343,15 +26340,15 @@
           /* "interpretable_tsne/_quad_tree.pyx":351
  *                     if child_id != -1:
  *                         child = self.cells[child_id]
  *                         n_points += child.cumulative_size             # <<<<<<<<<<<<<<
  *                         assert child.cell_id == child_id, (
  *                             "Cell id not correctly initialized.")
  */
-          __pyx_t_9 = PyInt_FromSsize_t(__pyx_v_child.cumulative_size); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 351, __pyx_L1_error)
+          __pyx_t_9 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_child.cumulative_size); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 351, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_9);
           __pyx_t_10 = PyNumber_InPlaceAdd(__pyx_v_n_points, __pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 351, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_10);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
           __Pyx_DECREF_SET(__pyx_v_n_points, __pyx_t_10);
           __pyx_t_10 = 0;
 
@@ -26387,15 +26384,15 @@
       /* "interpretable_tsne/_quad_tree.pyx":354
  *                         assert child.cell_id == child_id, (
  *                             "Cell id not correctly initialized.")
  *                 if n_points != cell.cumulative_size:             # <<<<<<<<<<<<<<
  *                     raise ValueError(
  *                         "Cell {} is incoherent. Size={} but found {} points "
  */
-      __pyx_t_10 = PyInt_FromSsize_t(__pyx_v_cell.cumulative_size); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 354, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_cell.cumulative_size); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 354, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __pyx_t_9 = PyObject_RichCompare(__pyx_v_n_points, __pyx_t_10, Py_NE); __Pyx_XGOTREF(__pyx_t_9); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 354, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 354, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       if (unlikely(__pyx_t_5)) {
 
@@ -26404,17 +26401,17 @@
  *                         "in children. ({})"
  *                         .format(cell.cell_id, cell.cumulative_size,             # <<<<<<<<<<<<<<
  *                                 n_points, cell.children))
  * 
  */
         __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Cell_is_incoherent_Size_but_foun, __pyx_n_s_format); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 358, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
-        __pyx_t_11 = PyInt_FromSsize_t(__pyx_v_cell.cell_id); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 358, __pyx_L1_error)
+        __pyx_t_11 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_cell.cell_id); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 358, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_11);
-        __pyx_t_12 = PyInt_FromSsize_t(__pyx_v_cell.cumulative_size); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 358, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_cell.cumulative_size); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 358, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
 
         /* "interpretable_tsne/_quad_tree.pyx":359
  *                         "in children. ({})"
  *                         .format(cell.cell_id, cell.cumulative_size,
  *                                 n_points, cell.children))             # <<<<<<<<<<<<<<
  * 
@@ -26496,17 +26493,17 @@
  *                 "in children."
  *                 .format(self.n_points, self.cells[0].cumulative_size))             # <<<<<<<<<<<<<<
  * 
  *     cdef long summarize(self, DTYPE_t[3] point, DTYPE_t* results,
  */
     __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_QuadTree_is_incoherent_Size_but, __pyx_n_s_format); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 367, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_13 = PyInt_FromSsize_t(__pyx_v_self->n_points); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 367, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_self->n_points); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 367, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_13);
-    __pyx_t_12 = PyInt_FromSsize_t((__pyx_v_self->cells[0]).cumulative_size); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 367, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyInt_From_Py_intptr_t((__pyx_v_self->cells[0]).cumulative_size); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 367, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     __pyx_t_11 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_9))) {
       __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_9);
       if (likely(__pyx_t_11)) {
@@ -27684,51 +27681,51 @@
   /* "interpretable_tsne/_quad_tree.pyx":500
  *         d = {}
  *         # capacity is inferred during the __setstate__ using nodes
  *         d["max_depth"] = self.max_depth             # <<<<<<<<<<<<<<
  *         d["cell_count"] = self.cell_count
  *         d["capacity"] = self.capacity
  */
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_self->max_depth); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 500, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_self->max_depth); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 500, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (unlikely((PyDict_SetItem(__pyx_v_d, __pyx_n_u_max_depth, __pyx_t_1) < 0))) __PYX_ERR(0, 500, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "interpretable_tsne/_quad_tree.pyx":501
  *         # capacity is inferred during the __setstate__ using nodes
  *         d["max_depth"] = self.max_depth
  *         d["cell_count"] = self.cell_count             # <<<<<<<<<<<<<<
  *         d["capacity"] = self.capacity
  *         d["n_points"] = self.n_points
  */
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_self->cell_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 501, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_self->cell_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 501, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (unlikely((PyDict_SetItem(__pyx_v_d, __pyx_n_u_cell_count, __pyx_t_1) < 0))) __PYX_ERR(0, 501, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "interpretable_tsne/_quad_tree.pyx":502
  *         d["max_depth"] = self.max_depth
  *         d["cell_count"] = self.cell_count
  *         d["capacity"] = self.capacity             # <<<<<<<<<<<<<<
  *         d["n_points"] = self.n_points
  *         d["cells"] = self._get_cell_ndarray()
  */
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_self->capacity); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 502, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_self->capacity); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 502, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (unlikely((PyDict_SetItem(__pyx_v_d, __pyx_n_u_capacity, __pyx_t_1) < 0))) __PYX_ERR(0, 502, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "interpretable_tsne/_quad_tree.pyx":503
  *         d["cell_count"] = self.cell_count
  *         d["capacity"] = self.capacity
  *         d["n_points"] = self.n_points             # <<<<<<<<<<<<<<
  *         d["cells"] = self._get_cell_ndarray()
  *         return d
  */
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_self->n_points); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 503, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_self->n_points); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 503, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (unlikely((PyDict_SetItem(__pyx_v_d, __pyx_n_u_n_points, __pyx_t_1) < 0))) __PYX_ERR(0, 503, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "interpretable_tsne/_quad_tree.pyx":504
  *         d["capacity"] = self.capacity
  *         d["n_points"] = self.n_points
@@ -27903,54 +27900,54 @@
  *         """Setstate re-implementation, for unpickling."""
  *         self.max_depth = d["max_depth"]             # <<<<<<<<<<<<<<
  *         self.cell_count = d["cell_count"]
  *         self.capacity = d["capacity"]
  */
   __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_d, __pyx_n_u_max_depth); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 509, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_2 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(0, 509, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_Py_intptr_t(__pyx_t_1); if (unlikely((__pyx_t_2 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(0, 509, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_self->max_depth = __pyx_t_2;
 
   /* "interpretable_tsne/_quad_tree.pyx":510
  *         """Setstate re-implementation, for unpickling."""
  *         self.max_depth = d["max_depth"]
  *         self.cell_count = d["cell_count"]             # <<<<<<<<<<<<<<
  *         self.capacity = d["capacity"]
  *         self.n_points = d["n_points"]
  */
   __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_d, __pyx_n_u_cell_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 510, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_2 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(0, 510, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_Py_intptr_t(__pyx_t_1); if (unlikely((__pyx_t_2 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(0, 510, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_self->cell_count = __pyx_t_2;
 
   /* "interpretable_tsne/_quad_tree.pyx":511
  *         self.max_depth = d["max_depth"]
  *         self.cell_count = d["cell_count"]
  *         self.capacity = d["capacity"]             # <<<<<<<<<<<<<<
  *         self.n_points = d["n_points"]
  * 
  */
   __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_d, __pyx_n_u_capacity); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 511, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_2 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(0, 511, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_Py_intptr_t(__pyx_t_1); if (unlikely((__pyx_t_2 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(0, 511, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_self->capacity = __pyx_t_2;
 
   /* "interpretable_tsne/_quad_tree.pyx":512
  *         self.cell_count = d["cell_count"]
  *         self.capacity = d["capacity"]
  *         self.n_points = d["n_points"]             # <<<<<<<<<<<<<<
  * 
  *         if 'cells' not in d:
  */
   __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_d, __pyx_n_u_n_points); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 512, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_2 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(0, 512, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_Py_intptr_t(__pyx_t_1); if (unlikely((__pyx_t_2 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(0, 512, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_self->n_points = __pyx_t_2;
 
   /* "interpretable_tsne/_quad_tree.pyx":514
  *         self.n_points = d["n_points"]
  * 
  *         if 'cells' not in d:             # <<<<<<<<<<<<<<
@@ -28090,15 +28087,15 @@
  *             raise MemoryError("resizing tree to %d" % self.capacity)
  */
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_cell_ndarray, __pyx_n_s_shape); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 525, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_5, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 525, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_2 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_2 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(0, 525, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_Py_intptr_t(__pyx_t_6); if (unlikely((__pyx_t_2 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(0, 525, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_v_self->capacity = __pyx_t_2;
 
   /* "interpretable_tsne/_quad_tree.pyx":526
  * 
  *         self.capacity = cell_ndarray.shape[0]
  *         if self._resize_c(self.capacity) != 0:             # <<<<<<<<<<<<<<
@@ -28114,15 +28111,15 @@
     /* "interpretable_tsne/_quad_tree.pyx":527
  *         self.capacity = cell_ndarray.shape[0]
  *         if self._resize_c(self.capacity) != 0:
  *             raise MemoryError("resizing tree to %d" % self.capacity)             # <<<<<<<<<<<<<<
  * 
  *         cells = memcpy(self.cells, (<cnp.ndarray> cell_ndarray).data,
  */
-    __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_self->capacity); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 527, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_self->capacity); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 527, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_5 = PyUnicode_Format(__pyx_kp_u_resizing_tree_to_d, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 527, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_MemoryError, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 527, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
@@ -29144,15 +29141,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_self->max_depth); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 63, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_self->max_depth); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -29182,15 +29179,15 @@
 
 static int __pyx_pf_18interpretable_tsne_10_quad_tree_9_QuadTree_9max_depth_2__set__(struct __pyx_obj_18interpretable_tsne_10_quad_tree__QuadTree *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __pyx_t_18interpretable_tsne_10_quad_tree_SIZE_t __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_v_value); if (unlikely((__pyx_t_1 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(4, 63, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_Py_intptr_t(__pyx_v_value); if (unlikely((__pyx_t_1 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(4, 63, __pyx_L1_error)
   __pyx_v_self->max_depth = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("interpretable_tsne._quad_tree._QuadTree.max_depth.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -29227,15 +29224,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_self->cell_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 64, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_self->cell_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -29265,15 +29262,15 @@
 
 static int __pyx_pf_18interpretable_tsne_10_quad_tree_9_QuadTree_10cell_count_2__set__(struct __pyx_obj_18interpretable_tsne_10_quad_tree__QuadTree *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __pyx_t_18interpretable_tsne_10_quad_tree_SIZE_t __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_v_value); if (unlikely((__pyx_t_1 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(4, 64, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_Py_intptr_t(__pyx_v_value); if (unlikely((__pyx_t_1 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(4, 64, __pyx_L1_error)
   __pyx_v_self->cell_count = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("interpretable_tsne._quad_tree._QuadTree.cell_count.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -29310,15 +29307,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_self->capacity); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 65, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_self->capacity); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -29348,15 +29345,15 @@
 
 static int __pyx_pf_18interpretable_tsne_10_quad_tree_9_QuadTree_8capacity_2__set__(struct __pyx_obj_18interpretable_tsne_10_quad_tree__QuadTree *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __pyx_t_18interpretable_tsne_10_quad_tree_SIZE_t __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_v_value); if (unlikely((__pyx_t_1 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(4, 65, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_Py_intptr_t(__pyx_v_value); if (unlikely((__pyx_t_1 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(4, 65, __pyx_L1_error)
   __pyx_v_self->capacity = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("interpretable_tsne._quad_tree._QuadTree.capacity.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -29393,15 +29390,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_self->n_points); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 66, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_self->n_points); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -29431,15 +29428,15 @@
 
 static int __pyx_pf_18interpretable_tsne_10_quad_tree_9_QuadTree_8n_points_2__set__(struct __pyx_obj_18interpretable_tsne_10_quad_tree__QuadTree *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __pyx_t_18interpretable_tsne_10_quad_tree_SIZE_t __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_v_value); if (unlikely((__pyx_t_1 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(4, 66, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_Py_intptr_t(__pyx_v_value); if (unlikely((__pyx_t_1 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(4, 66, __pyx_L1_error)
   __pyx_v_self->n_points = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("interpretable_tsne._quad_tree._QuadTree.n_points.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -30913,15 +30910,15 @@
   __pyx_builtin_OverflowError = __Pyx_GetBuiltinName(__pyx_n_s_OverflowError); if (!__pyx_builtin_OverflowError) __PYX_ERR(1, 83, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 86, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 96, __pyx_L1_error)
   __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(1, 19, __pyx_L1_error)
   __pyx_builtin___import__ = __Pyx_GetBuiltinName(__pyx_n_s_import); if (!__pyx_builtin___import__) __PYX_ERR(1, 100, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 408, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 618, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 987, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 984, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
@@ -31092,33 +31089,33 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__20 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(2, 987, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__27);
   __Pyx_GIVEREF(__pyx_tuple__27);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(2, 993, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(2, 990, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
 
   /* "interpretable_tsne/_quad_tree.pyx":479
  *                 return cell_id
  *             with gil:
  *                 raise ValueError("Query point not in the Tree.")             # <<<<<<<<<<<<<<
@@ -31645,31 +31642,31 @@
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(6, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(7, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 203, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 203, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 230, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 829, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 831, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 869, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 866, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("interpretable_tsne._utils"); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_18interpretable_tsne_6_utils_WeightedPQueue = __Pyx_ImportType_3_0_10(__pyx_t_1, "interpretable_tsne._utils", "WeightedPQueue", sizeof(struct __pyx_obj_18interpretable_tsne_6_utils_WeightedPQueue), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_18interpretable_tsne_6_utils_WeightedPQueue),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_18interpretable_tsne_6_utils_WeightedPQueue) __PYX_ERR(8, 83, __pyx_L1_error)
   __pyx_vtabptr_18interpretable_tsne_6_utils_WeightedPQueue = (struct __pyx_vtabstruct_18interpretable_tsne_6_utils_WeightedPQueue*)__Pyx_GetVtable(__pyx_ptype_18interpretable_tsne_6_utils_WeightedPQueue); if (unlikely(!__pyx_vtabptr_18interpretable_tsne_6_utils_WeightedPQueue)) __PYX_ERR(8, 83, __pyx_L1_error)
   __pyx_ptype_18interpretable_tsne_6_utils_WeightedMedianCalculator = __Pyx_ImportType_3_0_10(__pyx_t_1, "interpretable_tsne._utils", "WeightedMedianCalculator", sizeof(struct __pyx_obj_18interpretable_tsne_6_utils_WeightedMedianCalculator), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_18interpretable_tsne_6_utils_WeightedMedianCalculator),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_18interpretable_tsne_6_utils_WeightedMedianCalculator) __PYX_ERR(8, 103, __pyx_L1_error)
   __pyx_vtabptr_18interpretable_tsne_6_utils_WeightedMedianCalculator = (struct __pyx_vtabstruct_18interpretable_tsne_6_utils_WeightedMedianCalculator*)__Pyx_GetVtable(__pyx_ptype_18interpretable_tsne_6_utils_WeightedMedianCalculator); if (unlikely(!__pyx_vtabptr_18interpretable_tsne_6_utils_WeightedMedianCalculator)) __PYX_ERR(8, 103, __pyx_L1_error)
@@ -38045,36 +38042,36 @@
     return (start1 < end2) && (start2 < end1);
 }
 
 static PyObject* __pyx_convert__to_py_struct____pyx_t_18interpretable_tsne_10_quad_tree_Cell(struct __pyx_t_18interpretable_tsne_10_quad_tree_Cell s) {
   PyObject* res;
   PyObject* member;
   res = __Pyx_PyDict_NewPresized(12); if (unlikely(!res)) return NULL;
-  member = PyInt_FromSsize_t(s.parent); if (unlikely(!member)) goto bad;
+  member = __Pyx_PyInt_From_Py_intptr_t(s.parent); if (unlikely(!member)) goto bad;
   if (unlikely(PyDict_SetItem(res, __pyx_n_s_parent, member) < 0)) goto bad;
   Py_DECREF(member);
   member = __Pyx_carray_to_py___pyx_t_18interpretable_tsne_10_quad_tree_SIZE_t(s.children, 8); if (unlikely(!member)) goto bad;
   if (unlikely(PyDict_SetItem(res, __pyx_n_s_children, member) < 0)) goto bad;
   Py_DECREF(member);
-  member = PyInt_FromSsize_t(s.cell_id); if (unlikely(!member)) goto bad;
+  member = __Pyx_PyInt_From_Py_intptr_t(s.cell_id); if (unlikely(!member)) goto bad;
   if (unlikely(PyDict_SetItem(res, __pyx_n_s_cell_id, member) < 0)) goto bad;
   Py_DECREF(member);
-  member = PyInt_FromSsize_t(s.point_index); if (unlikely(!member)) goto bad;
+  member = __Pyx_PyInt_From_Py_intptr_t(s.point_index); if (unlikely(!member)) goto bad;
   if (unlikely(PyDict_SetItem(res, __pyx_n_s_point_index, member) < 0)) goto bad;
   Py_DECREF(member);
   member = __Pyx_PyBool_FromLong(s.is_leaf); if (unlikely(!member)) goto bad;
   if (unlikely(PyDict_SetItem(res, __pyx_n_s_is_leaf, member) < 0)) goto bad;
   Py_DECREF(member);
   member = PyFloat_FromDouble(s.squared_max_width); if (unlikely(!member)) goto bad;
   if (unlikely(PyDict_SetItem(res, __pyx_n_s_squared_max_width, member) < 0)) goto bad;
   Py_DECREF(member);
-  member = PyInt_FromSsize_t(s.depth); if (unlikely(!member)) goto bad;
+  member = __Pyx_PyInt_From_Py_intptr_t(s.depth); if (unlikely(!member)) goto bad;
   if (unlikely(PyDict_SetItem(res, __pyx_n_s_depth, member) < 0)) goto bad;
   Py_DECREF(member);
-  member = PyInt_FromSsize_t(s.cumulative_size); if (unlikely(!member)) goto bad;
+  member = __Pyx_PyInt_From_Py_intptr_t(s.cumulative_size); if (unlikely(!member)) goto bad;
   if (unlikely(PyDict_SetItem(res, __pyx_n_s_cumulative_size, member) < 0)) goto bad;
   Py_DECREF(member);
   member = __Pyx_carray_to_py___pyx_t_18interpretable_tsne_10_quad_tree_DTYPE_t(s.center, 3); if (unlikely(!member)) goto bad;
   if (unlikely(PyDict_SetItem(res, __pyx_n_s_center, member) < 0)) goto bad;
   Py_DECREF(member);
   member = __Pyx_carray_to_py___pyx_t_18interpretable_tsne_10_quad_tree_DTYPE_t(s.barycenter, 3); if (unlikely(!member)) goto bad;
   if (unlikely(PyDict_SetItem(res, __pyx_n_s_barycenter, member) < 0)) goto bad;
@@ -38087,26 +38084,14 @@
   Py_DECREF(member);
   return res;
   bad:
   Py_XDECREF(member);
   Py_DECREF(res);
   return NULL;
 }
-/* MemviewDtypeToObject */
-static CYTHON_INLINE PyObject *__pyx_memview_get_nn_struct____pyx_t_18interpretable_tsne_10_quad_tree_Cell(const char *itemp) {
-    return (PyObject *) __pyx_convert__to_py_struct____pyx_t_18interpretable_tsne_10_quad_tree_Cell(*(struct __pyx_t_18interpretable_tsne_10_quad_tree_Cell *) itemp);
-}
-static CYTHON_INLINE int __pyx_memview_set_nn_struct____pyx_t_18interpretable_tsne_10_quad_tree_Cell(const char *itemp, PyObject *obj) {
-    struct __pyx_t_18interpretable_tsne_10_quad_tree_Cell value = __pyx_convert__from_py_struct____pyx_t_18interpretable_tsne_10_quad_tree_Cell(obj);
-    if (unlikely(PyErr_Occurred()))
-        return 0;
-    *(struct __pyx_t_18interpretable_tsne_10_quad_tree_Cell *) itemp = value;
-    return 1;
-}
-
 /* CIntFromPyVerify */
 #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
 #define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
 #define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
     {\
@@ -38121,14 +38106,26 @@
                 else\
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
+/* MemviewDtypeToObject */
+static CYTHON_INLINE PyObject *__pyx_memview_get_nn_struct____pyx_t_18interpretable_tsne_10_quad_tree_Cell(const char *itemp) {
+    return (PyObject *) __pyx_convert__to_py_struct____pyx_t_18interpretable_tsne_10_quad_tree_Cell(*(struct __pyx_t_18interpretable_tsne_10_quad_tree_Cell *) itemp);
+}
+static CYTHON_INLINE int __pyx_memview_set_nn_struct____pyx_t_18interpretable_tsne_10_quad_tree_Cell(const char *itemp, PyObject *obj) {
+    struct __pyx_t_18interpretable_tsne_10_quad_tree_Cell value = __pyx_convert__from_py_struct____pyx_t_18interpretable_tsne_10_quad_tree_Cell(obj);
+    if (unlikely(PyErr_Occurred()))
+        return 0;
+    *(struct __pyx_t_18interpretable_tsne_10_quad_tree_Cell *) itemp = value;
+    return 1;
+}
+
 /* IsLittleEndian */
 static CYTHON_INLINE int __Pyx_Is_Little_Endian(void)
 {
   union {
     uint32_t u32;
     uint8_t u8[4];
   } S;
@@ -39477,14 +39474,351 @@
             else
                 *buf = 'g';
             break;
     }
     return result;
 }
 
+/* CIntToPy */
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_Py_intptr_t(Py_intptr_t value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const Py_intptr_t neg_one = (Py_intptr_t) -1, const_zero = (Py_intptr_t) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(Py_intptr_t) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(Py_intptr_t) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(Py_intptr_t) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(Py_intptr_t) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(Py_intptr_t) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
+        return _PyLong_FromByteArray(bytes, sizeof(Py_intptr_t),
+                                     little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(Py_intptr_t));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
+        return result;
+#endif
+    }
+}
+
+/* CIntFromPy */
+  static CYTHON_INLINE Py_intptr_t __Pyx_PyInt_As_Py_intptr_t(PyObject *x) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const Py_intptr_t neg_one = (Py_intptr_t) -1, const_zero = (Py_intptr_t) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+#if PY_MAJOR_VERSION < 3
+    if (likely(PyInt_Check(x))) {
+        if ((sizeof(Py_intptr_t) < sizeof(long))) {
+            __PYX_VERIFY_RETURN_INT(Py_intptr_t, long, PyInt_AS_LONG(x))
+        } else {
+            long val = PyInt_AS_LONG(x);
+            if (is_unsigned && unlikely(val < 0)) {
+                goto raise_neg_overflow;
+            }
+            return (Py_intptr_t) val;
+        }
+    } else
+#endif
+    if (likely(PyLong_Check(x))) {
+        if (is_unsigned) {
+#if CYTHON_USE_PYLONG_INTERNALS
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(Py_intptr_t, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(Py_intptr_t) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(Py_intptr_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(Py_intptr_t) >= 2 * PyLong_SHIFT)) {
+                                return (Py_intptr_t) (((((Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0]));
+                            }
+                        }
+                        break;
+                    case 3:
+                        if ((8 * sizeof(Py_intptr_t) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(Py_intptr_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(Py_intptr_t) >= 3 * PyLong_SHIFT)) {
+                                return (Py_intptr_t) (((((((Py_intptr_t)digits[2]) << PyLong_SHIFT) | (Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0]));
+                            }
+                        }
+                        break;
+                    case 4:
+                        if ((8 * sizeof(Py_intptr_t) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(Py_intptr_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(Py_intptr_t) >= 4 * PyLong_SHIFT)) {
+                                return (Py_intptr_t) (((((((((Py_intptr_t)digits[3]) << PyLong_SHIFT) | (Py_intptr_t)digits[2]) << PyLong_SHIFT) | (Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0]));
+                            }
+                        }
+                        break;
+                }
+            }
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+            if (unlikely(Py_SIZE(x) < 0)) {
+                goto raise_neg_overflow;
+            }
+#else
+            {
+                int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                if (unlikely(result < 0))
+                    return (Py_intptr_t) -1;
+                if (unlikely(result == 1))
+                    goto raise_neg_overflow;
+            }
+#endif
+            if ((sizeof(Py_intptr_t) <= sizeof(unsigned long))) {
+                __PYX_VERIFY_RETURN_INT_EXC(Py_intptr_t, unsigned long, PyLong_AsUnsignedLong(x))
+#ifdef HAVE_LONG_LONG
+            } else if ((sizeof(Py_intptr_t) <= sizeof(unsigned PY_LONG_LONG))) {
+                __PYX_VERIFY_RETURN_INT_EXC(Py_intptr_t, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
+#endif
+            }
+        } else {
+#if CYTHON_USE_PYLONG_INTERNALS
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(Py_intptr_t, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(Py_intptr_t) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(Py_intptr_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(Py_intptr_t) - 1 > 2 * PyLong_SHIFT)) {
+                                return (Py_intptr_t) (((Py_intptr_t)-1)*(((((Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0])));
+                            }
+                        }
+                        break;
+                    case 2:
+                        if ((8 * sizeof(Py_intptr_t) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(Py_intptr_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(Py_intptr_t) - 1 > 2 * PyLong_SHIFT)) {
+                                return (Py_intptr_t) ((((((Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0])));
+                            }
+                        }
+                        break;
+                    case -3:
+                        if ((8 * sizeof(Py_intptr_t) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(Py_intptr_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(Py_intptr_t) - 1 > 3 * PyLong_SHIFT)) {
+                                return (Py_intptr_t) (((Py_intptr_t)-1)*(((((((Py_intptr_t)digits[2]) << PyLong_SHIFT) | (Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0])));
+                            }
+                        }
+                        break;
+                    case 3:
+                        if ((8 * sizeof(Py_intptr_t) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(Py_intptr_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(Py_intptr_t) - 1 > 3 * PyLong_SHIFT)) {
+                                return (Py_intptr_t) ((((((((Py_intptr_t)digits[2]) << PyLong_SHIFT) | (Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0])));
+                            }
+                        }
+                        break;
+                    case -4:
+                        if ((8 * sizeof(Py_intptr_t) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(Py_intptr_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(Py_intptr_t) - 1 > 4 * PyLong_SHIFT)) {
+                                return (Py_intptr_t) (((Py_intptr_t)-1)*(((((((((Py_intptr_t)digits[3]) << PyLong_SHIFT) | (Py_intptr_t)digits[2]) << PyLong_SHIFT) | (Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0])));
+                            }
+                        }
+                        break;
+                    case 4:
+                        if ((8 * sizeof(Py_intptr_t) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(Py_intptr_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(Py_intptr_t) - 1 > 4 * PyLong_SHIFT)) {
+                                return (Py_intptr_t) ((((((((((Py_intptr_t)digits[3]) << PyLong_SHIFT) | (Py_intptr_t)digits[2]) << PyLong_SHIFT) | (Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0])));
+                            }
+                        }
+                        break;
+                }
+            }
+#endif
+            if ((sizeof(Py_intptr_t) <= sizeof(long))) {
+                __PYX_VERIFY_RETURN_INT_EXC(Py_intptr_t, long, PyLong_AsLong(x))
+#ifdef HAVE_LONG_LONG
+            } else if ((sizeof(Py_intptr_t) <= sizeof(PY_LONG_LONG))) {
+                __PYX_VERIFY_RETURN_INT_EXC(Py_intptr_t, PY_LONG_LONG, PyLong_AsLongLong(x))
+#endif
+            }
+        }
+        {
+            Py_intptr_t val;
+            PyObject *v = __Pyx_PyNumber_IntOrLong(x);
+#if PY_MAJOR_VERSION < 3
+            if (likely(v) && !PyLong_Check(v)) {
+                PyObject *tmp = v;
+                v = PyNumber_Long(tmp);
+                Py_DECREF(tmp);
+            }
+#endif
+            if (likely(v)) {
+                int ret = -1;
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+                int one = 1; int is_little = (int)*(unsigned char *)&one;
+                unsigned char *bytes = (unsigned char *)&val;
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (Py_intptr_t) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (Py_intptr_t) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (Py_intptr_t) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (Py_intptr_t) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (Py_intptr_t) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(Py_intptr_t) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((Py_intptr_t) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(Py_intptr_t) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((Py_intptr_t) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((Py_intptr_t) 1) << (sizeof(Py_intptr_t) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
+                Py_DECREF(v);
+                if (likely(!ret))
+                    return val;
+            }
+            return (Py_intptr_t) -1;
+        }
+    } else {
+        Py_intptr_t val;
+        PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
+        if (!tmp) return (Py_intptr_t) -1;
+        val = __Pyx_PyInt_As_Py_intptr_t(tmp);
+        Py_DECREF(tmp);
+        return val;
+    }
+raise_overflow:
+    PyErr_SetString(PyExc_OverflowError,
+        "value too large to convert to Py_intptr_t");
+    return (Py_intptr_t) -1;
+raise_neg_overflow:
+    PyErr_SetString(PyExc_OverflowError,
+        "can't convert negative value to Py_intptr_t");
+    return (Py_intptr_t) -1;
+}
+
 /* CIntFromPy */
   static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int neg_one = (int) -1, const_zero = (int) 0;
```

### Comparing `interpretable_tsne-0.0.3/src/interpretable_tsne/_quad_tree.pxd` & `interpretable_tsne-0.0.4/src/interpretable_tsne/_quad_tree.pxd`

 * *Files identical despite different names*

### Comparing `interpretable_tsne-0.0.3/src/interpretable_tsne/_quad_tree.pyx` & `interpretable_tsne-0.0.4/src/interpretable_tsne/_quad_tree.pyx`

 * *Files identical despite different names*

### Comparing `interpretable_tsne-0.0.3/src/interpretable_tsne/_utils.c` & `interpretable_tsne-0.0.4/src/interpretable_tsne/_utils.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/core/include"
+            "/tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/core/include"
         ],
         "name": "interpretable_tsne._utils",
         "sources": [
             "src/interpretable_tsne/_utils.pyx"
         ]
     },
     "module_name": "interpretable_tsne._utils"
@@ -1540,195 +1540,177 @@
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":734
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":735
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":741
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":742
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":746
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":747
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":756
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
+ * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   longlong_t
- * 
- */
-typedef npy_longlong __pyx_t_5numpy_long_t;
-
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":758
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
+ * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulonglong_t
- * 
- */
-typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
-
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":762
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1841,42 +1823,42 @@
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_obj_18interpretable_tsne_10_quad_tree__QuadTree;
 struct __pyx_obj_18interpretable_tsne_6_utils_WeightedPQueue;
 struct __pyx_obj_18interpretable_tsne_6_utils_WeightedMedianCalculator;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":772
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":775
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2393,17 +2375,14 @@
 
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
 /* ExtTypeTest.proto */
 static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
 
-/* ModInt[__pyx_t_18interpretable_tsne_6_utils_SIZE_t].proto */
-static CYTHON_INLINE __pyx_t_18interpretable_tsne_6_utils_SIZE_t __Pyx_mod___pyx_t_18interpretable_tsne_6_utils_SIZE_t(__pyx_t_18interpretable_tsne_6_utils_SIZE_t, __pyx_t_18interpretable_tsne_6_utils_SIZE_t);
-
 /* ErrOccurredWithGIL.proto */
 static CYTHON_INLINE int __Pyx_ErrOccurredWithGIL(void);
 
 /* TupleAndListFromArray.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n);
 static CYTHON_INLINE PyObject* __Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n);
@@ -2842,30 +2821,36 @@
     static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_conj_double(__pyx_t_double_complex);
     #if 1
         static CYTHON_INLINE double __Pyx_c_abs_double(__pyx_t_double_complex);
         static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_pow_double(__pyx_t_double_complex, __pyx_t_double_complex);
     #endif
 #endif
 
+/* CIntFromPy.proto */
+static CYTHON_INLINE Py_intptr_t __Pyx_PyInt_As_Py_intptr_t(PyObject *);
+
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_Py_intptr_t(Py_intptr_t value);
+
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+
 /* FormatTypeName.proto */
 #if CYTHON_COMPILING_IN_LIMITED_API
 typedef PyObject *__Pyx_TypeName;
 #define __Pyx_FMT_TYPENAME "%U"
 static __Pyx_TypeName __Pyx_PyType_GetName(PyTypeObject* tp);
 #define __Pyx_DECREF_TypeName(obj) Py_XDECREF(obj)
 #else
 typedef const char *__Pyx_TypeName;
 #define __Pyx_FMT_TYPENAME "%.200s"
 #define __Pyx_PyType_GetName(tp) ((tp)->tp_name)
 #define __Pyx_DECREF_TypeName(obj)
 #endif
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
-
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* FastTypeChecks.proto */
@@ -3484,261 +3469,261 @@
 #define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
 #define __pyx_codeobj__5 __pyx_mstate_global->__pyx_codeobj__5
 #define __pyx_codeobj__7 __pyx_mstate_global->__pyx_codeobj__7
 #define __pyx_codeobj__8 __pyx_mstate_global->__pyx_codeobj__8
 #define __pyx_codeobj__9 __pyx_mstate_global->__pyx_codeobj__9
 /* #### Code section: module_code ### */
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":246
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":249
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":246
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":252
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":255
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":252
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":258
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":261
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":258
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":264
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":269
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":264
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":272
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":276
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":272
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":279
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":282
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":279
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":285
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":291
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":285
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":777
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3747,29 +3732,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":778
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 778, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3780,15 +3765,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":780
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3797,29 +3782,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":781
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 781, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3830,15 +3815,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":783
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3847,29 +3832,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":784
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 784, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3880,15 +3865,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":786
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3897,29 +3882,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":787
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 787, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3930,15 +3915,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":789
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3947,29 +3932,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":790
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 790, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3980,209 +3965,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":792
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":793
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":794
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":793
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":796
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_L0:;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":975
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":977
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":978
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":977
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":983
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4198,15 +4191,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4214,68 +4207,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":985
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 985, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 986, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 987, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 987, __pyx_L5_except_error)
+      __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":984
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4283,15 +4276,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4306,15 +4299,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":989
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4330,15 +4323,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4346,68 +4339,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":991
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 991, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 992, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 993, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 993, __pyx_L5_except_error)
+      __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":990
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4415,15 +4408,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4438,15 +4431,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":995
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4462,15 +4455,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":996
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4478,68 +4471,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":997
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 997, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":998
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 998, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":999
+      /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 999, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 999, __pyx_L5_except_error)
+      __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":996
+    /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4547,15 +4540,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":995
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4570,170 +4563,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1002
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1002
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1017
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1017
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1032
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1032
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1042
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1049
+/* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1053
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -7427,15 +7420,15 @@
     #endif
     PyErr_SetString(PyExc_ZeroDivisionError, "integer division or modulo by zero");
     #ifdef WITH_THREAD
     __Pyx_PyGILState_Release(__pyx_gilstate_save);
     #endif
     __PYX_ERR(0, 75, __pyx_L1_error)
   }
-  __pyx_r = (__pyx_v_low + __Pyx_mod___pyx_t_18interpretable_tsne_6_utils_SIZE_t(__pyx_t_1, __pyx_t_2));
+  __pyx_r = (__pyx_v_low + (__pyx_t_1 % __pyx_t_2));
   goto __pyx_L0;
 
   /* "interpretable_tsne/_utils.pyx":72
  * 
  * 
  * cdef inline SIZE_t rand_int(SIZE_t low, SIZE_t high,             # <<<<<<<<<<<<<<
  *                             UINT32_t* random_state) nogil:
@@ -7642,15 +7635,15 @@
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__cinit__") < 0)) __PYX_ERR(0, 111, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
     }
-    __pyx_v_capacity = __Pyx_PyIndex_AsSsize_t(values[0]); if (unlikely((__pyx_v_capacity == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(0, 111, __pyx_L3_error)
+    __pyx_v_capacity = __Pyx_PyInt_As_Py_intptr_t(values[0]); if (unlikely((__pyx_v_capacity == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(0, 111, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 111, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
@@ -8123,14 +8116,16 @@
   int __pyx_r;
   __pyx_t_18interpretable_tsne_6_utils_SIZE_t __pyx_t_1;
   struct __pyx_t_18interpretable_tsne_6_utils_WeightedPQueueRecord *__pyx_t_2;
   int __pyx_t_3;
   __pyx_t_18interpretable_tsne_6_utils_SIZE_t __pyx_t_4;
   __pyx_t_18interpretable_tsne_6_utils_SIZE_t __pyx_t_5;
   int __pyx_t_6;
+  long __pyx_t_7;
+  long __pyx_t_8;
 
   /* "interpretable_tsne/_utils.pyx":171
  *         """Remove a specific value/weight record from the array.
  *         Returns 0 if successful, -1 if record not found."""
  *         cdef SIZE_t array_ptr = self.array_ptr             # <<<<<<<<<<<<<<
  *         cdef WeightedPQueueRecord* array = self.array_
  *         cdef SIZE_t idx_to_remove = -1
@@ -8151,15 +8146,15 @@
   /* "interpretable_tsne/_utils.pyx":173
  *         cdef SIZE_t array_ptr = self.array_ptr
  *         cdef WeightedPQueueRecord* array = self.array_
  *         cdef SIZE_t idx_to_remove = -1             # <<<<<<<<<<<<<<
  *         cdef SIZE_t i
  * 
  */
-  __pyx_v_idx_to_remove = -1L;
+  __pyx_v_idx_to_remove = -1;
 
   /* "interpretable_tsne/_utils.pyx":176
  *         cdef SIZE_t i
  * 
  *         if array_ptr <= 0:             # <<<<<<<<<<<<<<
  *             return -1
  * 
@@ -8277,18 +8272,18 @@
   /* "interpretable_tsne/_utils.pyx":190
  *         # shift the elements after the removed element
  *         # to the left.
  *         for i in range(idx_to_remove, array_ptr-1):             # <<<<<<<<<<<<<<
  *             array[i] = array[i+1]
  * 
  */
-  __pyx_t_1 = (__pyx_v_array_ptr - 1);
-  __pyx_t_4 = __pyx_t_1;
-  for (__pyx_t_5 = __pyx_v_idx_to_remove; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
-    __pyx_v_i = __pyx_t_5;
+  __pyx_t_7 = (__pyx_v_array_ptr - 1);
+  __pyx_t_8 = __pyx_t_7;
+  for (__pyx_t_1 = __pyx_v_idx_to_remove; __pyx_t_1 < __pyx_t_8; __pyx_t_1+=1) {
+    __pyx_v_i = __pyx_t_1;
 
     /* "interpretable_tsne/_utils.pyx":191
  *         # to the left.
  *         for i in range(idx_to_remove, array_ptr-1):
  *             array[i] = array[i+1]             # <<<<<<<<<<<<<<
  * 
  *         self.array_ptr = array_ptr - 1
@@ -8341,16 +8336,16 @@
   struct __pyx_t_18interpretable_tsne_6_utils_WeightedPQueueRecord *__pyx_v_array;
   __pyx_t_18interpretable_tsne_6_utils_SIZE_t __pyx_v_i;
   int __pyx_r;
   __pyx_t_18interpretable_tsne_6_utils_SIZE_t __pyx_t_1;
   struct __pyx_t_18interpretable_tsne_6_utils_WeightedPQueueRecord *__pyx_t_2;
   int __pyx_t_3;
   __pyx_t_18interpretable_tsne_6_utils_DOUBLE_t __pyx_t_4;
-  __pyx_t_18interpretable_tsne_6_utils_SIZE_t __pyx_t_5;
-  __pyx_t_18interpretable_tsne_6_utils_SIZE_t __pyx_t_6;
+  long __pyx_t_5;
+  long __pyx_t_6;
 
   /* "interpretable_tsne/_utils.pyx":199
  *         """Remove the top (minimum) element from array.
  *         Returns 0 if successful, -1 if nothing to remove."""
  *         cdef SIZE_t array_ptr = self.array_ptr             # <<<<<<<<<<<<<<
  *         cdef WeightedPQueueRecord* array = self.array_
  *         cdef SIZE_t i
@@ -8420,18 +8415,18 @@
   /* "interpretable_tsne/_utils.pyx":211
  *         # shift the elements after the removed element
  *         # to the left.
  *         for i in range(0, array_ptr-1):             # <<<<<<<<<<<<<<
  *             array[i] = array[i+1]
  * 
  */
-  __pyx_t_1 = (__pyx_v_array_ptr - 1);
-  __pyx_t_5 = __pyx_t_1;
-  for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
-    __pyx_v_i = __pyx_t_6;
+  __pyx_t_5 = (__pyx_v_array_ptr - 1);
+  __pyx_t_6 = __pyx_t_5;
+  for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_6; __pyx_t_1+=1) {
+    __pyx_v_i = __pyx_t_1;
 
     /* "interpretable_tsne/_utils.pyx":212
  *         # to the left.
  *         for i in range(0, array_ptr-1):
  *             array[i] = array[i+1]             # <<<<<<<<<<<<<<
  * 
  *         self.array_ptr = array_ptr - 1
@@ -8926,15 +8921,15 @@
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__cinit__") < 0)) __PYX_ERR(0, 282, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
     }
-    __pyx_v_initial_capacity = __Pyx_PyIndex_AsSsize_t(values[0]); if (unlikely((__pyx_v_initial_capacity == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(0, 282, __pyx_L3_error)
+    __pyx_v_initial_capacity = __Pyx_PyInt_As_Py_intptr_t(values[0]); if (unlikely((__pyx_v_initial_capacity == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(0, 282, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 282, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
@@ -8983,15 +8978,15 @@
   /* "interpretable_tsne/_utils.pyx":284
  *     def __cinit__(self, SIZE_t initial_capacity):
  *         self.initial_capacity = initial_capacity
  *         self.samples = WeightedPQueue(initial_capacity)             # <<<<<<<<<<<<<<
  *         self.total_weight = 0
  *         self.k = 0
  */
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_initial_capacity); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_initial_capacity); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_18interpretable_tsne_6_utils_WeightedPQueue), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF((PyObject *)__pyx_v_self->samples);
   __Pyx_DECREF((PyObject *)__pyx_v_self->samples);
@@ -10914,44 +10909,44 @@
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 45, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 180, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 987, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 984, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(2, 987, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../../tmp/build-env-xkj2h6wc/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../../tmp/build-env-v02rjfxq/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(2, 993, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(2, 990, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
@@ -11161,31 +11156,31 @@
   #elif CYTHON_COMPILING_IN_LIMITED_API
   sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 203, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 203, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 230, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 829, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 831, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 869, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 866, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("interpretable_tsne._quad_tree"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_18interpretable_tsne_10_quad_tree__QuadTree = __Pyx_ImportType_3_0_10(__pyx_t_1, "interpretable_tsne._quad_tree", "_QuadTree", sizeof(struct __pyx_obj_18interpretable_tsne_10_quad_tree__QuadTree), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_18interpretable_tsne_10_quad_tree__QuadTree),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_18interpretable_tsne_10_quad_tree__QuadTree) __PYX_ERR(4, 50, __pyx_L1_error)
   __pyx_vtabptr_18interpretable_tsne_10_quad_tree__QuadTree = (struct __pyx_vtabstruct_18interpretable_tsne_10_quad_tree__QuadTree*)__Pyx_GetVtable(__pyx_ptype_18interpretable_tsne_10_quad_tree__QuadTree); if (unlikely(!__pyx_vtabptr_18interpretable_tsne_10_quad_tree__QuadTree)) __PYX_ERR(4, 50, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
@@ -12662,21 +12657,14 @@
                  "Cannot convert " __Pyx_FMT_TYPENAME " to " __Pyx_FMT_TYPENAME,
                  obj_type_name, type_name);
     __Pyx_DECREF_TypeName(obj_type_name);
     __Pyx_DECREF_TypeName(type_name);
     return 0;
 }
 
-/* ModInt[__pyx_t_18interpretable_tsne_6_utils_SIZE_t] */
-static CYTHON_INLINE __pyx_t_18interpretable_tsne_6_utils_SIZE_t __Pyx_mod___pyx_t_18interpretable_tsne_6_utils_SIZE_t(__pyx_t_18interpretable_tsne_6_utils_SIZE_t a, __pyx_t_18interpretable_tsne_6_utils_SIZE_t b) {
-    __pyx_t_18interpretable_tsne_6_utils_SIZE_t r = a % b;
-    r += ((r != 0) & ((r ^ b) < 0)) * b;
-    return r;
-}
-
 /* ErrOccurredWithGIL */
 static CYTHON_INLINE int __Pyx_ErrOccurredWithGIL(void) {
   int err;
   #ifdef WITH_THREAD
   PyGILState_STATE _save = PyGILState_Ensure();
   #endif
   err = !!PyErr_Occurred();
@@ -15394,14 +15382,36 @@
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
 #endif
 
+/* CIntFromPyVerify */
+#define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
+    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
+#define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
+    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
+#define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
+    {\
+        func_type value = func_value;\
+        if (sizeof(target_type) < sizeof(func_type)) {\
+            if (unlikely(value != (func_type) (target_type) value)) {\
+                func_type zero = 0;\
+                if (exc && unlikely(value == (func_type)-1 && PyErr_Occurred()))\
+                    return (target_type) -1;\
+                if (is_unsigned && unlikely(value < zero))\
+                    goto raise_neg_overflow;\
+                else\
+                    goto raise_overflow;\
+            }\
+        }\
+        return (target_type) value;\
+    }
+
 /* Declarations */
 #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return ::std::complex< float >(x, y);
     }
   #else
@@ -15702,29 +15712,350 @@
             z.real = z_r * cos(z_theta);
             z.imag = z_r * sin(z_theta);
             return z;
         }
     #endif
 #endif
 
-/* FormatTypeName */
-#if CYTHON_COMPILING_IN_LIMITED_API
-static __Pyx_TypeName
-__Pyx_PyType_GetName(PyTypeObject* tp)
-{
-    PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
-                                               __pyx_n_s_name);
-    if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
-        PyErr_Clear();
-        Py_XDECREF(name);
-        name = __Pyx_NewRef(__pyx_n_s__10);
+/* CIntFromPy */
+static CYTHON_INLINE Py_intptr_t __Pyx_PyInt_As_Py_intptr_t(PyObject *x) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const Py_intptr_t neg_one = (Py_intptr_t) -1, const_zero = (Py_intptr_t) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+#if PY_MAJOR_VERSION < 3
+    if (likely(PyInt_Check(x))) {
+        if ((sizeof(Py_intptr_t) < sizeof(long))) {
+            __PYX_VERIFY_RETURN_INT(Py_intptr_t, long, PyInt_AS_LONG(x))
+        } else {
+            long val = PyInt_AS_LONG(x);
+            if (is_unsigned && unlikely(val < 0)) {
+                goto raise_neg_overflow;
+            }
+            return (Py_intptr_t) val;
+        }
+    } else
+#endif
+    if (likely(PyLong_Check(x))) {
+        if (is_unsigned) {
+#if CYTHON_USE_PYLONG_INTERNALS
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(Py_intptr_t, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(Py_intptr_t) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(Py_intptr_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(Py_intptr_t) >= 2 * PyLong_SHIFT)) {
+                                return (Py_intptr_t) (((((Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0]));
+                            }
+                        }
+                        break;
+                    case 3:
+                        if ((8 * sizeof(Py_intptr_t) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(Py_intptr_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(Py_intptr_t) >= 3 * PyLong_SHIFT)) {
+                                return (Py_intptr_t) (((((((Py_intptr_t)digits[2]) << PyLong_SHIFT) | (Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0]));
+                            }
+                        }
+                        break;
+                    case 4:
+                        if ((8 * sizeof(Py_intptr_t) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(Py_intptr_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(Py_intptr_t) >= 4 * PyLong_SHIFT)) {
+                                return (Py_intptr_t) (((((((((Py_intptr_t)digits[3]) << PyLong_SHIFT) | (Py_intptr_t)digits[2]) << PyLong_SHIFT) | (Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0]));
+                            }
+                        }
+                        break;
+                }
+            }
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+            if (unlikely(Py_SIZE(x) < 0)) {
+                goto raise_neg_overflow;
+            }
+#else
+            {
+                int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                if (unlikely(result < 0))
+                    return (Py_intptr_t) -1;
+                if (unlikely(result == 1))
+                    goto raise_neg_overflow;
+            }
+#endif
+            if ((sizeof(Py_intptr_t) <= sizeof(unsigned long))) {
+                __PYX_VERIFY_RETURN_INT_EXC(Py_intptr_t, unsigned long, PyLong_AsUnsignedLong(x))
+#ifdef HAVE_LONG_LONG
+            } else if ((sizeof(Py_intptr_t) <= sizeof(unsigned PY_LONG_LONG))) {
+                __PYX_VERIFY_RETURN_INT_EXC(Py_intptr_t, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
+#endif
+            }
+        } else {
+#if CYTHON_USE_PYLONG_INTERNALS
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(Py_intptr_t, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(Py_intptr_t) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(Py_intptr_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(Py_intptr_t) - 1 > 2 * PyLong_SHIFT)) {
+                                return (Py_intptr_t) (((Py_intptr_t)-1)*(((((Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0])));
+                            }
+                        }
+                        break;
+                    case 2:
+                        if ((8 * sizeof(Py_intptr_t) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(Py_intptr_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(Py_intptr_t) - 1 > 2 * PyLong_SHIFT)) {
+                                return (Py_intptr_t) ((((((Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0])));
+                            }
+                        }
+                        break;
+                    case -3:
+                        if ((8 * sizeof(Py_intptr_t) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(Py_intptr_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(Py_intptr_t) - 1 > 3 * PyLong_SHIFT)) {
+                                return (Py_intptr_t) (((Py_intptr_t)-1)*(((((((Py_intptr_t)digits[2]) << PyLong_SHIFT) | (Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0])));
+                            }
+                        }
+                        break;
+                    case 3:
+                        if ((8 * sizeof(Py_intptr_t) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(Py_intptr_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(Py_intptr_t) - 1 > 3 * PyLong_SHIFT)) {
+                                return (Py_intptr_t) ((((((((Py_intptr_t)digits[2]) << PyLong_SHIFT) | (Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0])));
+                            }
+                        }
+                        break;
+                    case -4:
+                        if ((8 * sizeof(Py_intptr_t) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(Py_intptr_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(Py_intptr_t) - 1 > 4 * PyLong_SHIFT)) {
+                                return (Py_intptr_t) (((Py_intptr_t)-1)*(((((((((Py_intptr_t)digits[3]) << PyLong_SHIFT) | (Py_intptr_t)digits[2]) << PyLong_SHIFT) | (Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0])));
+                            }
+                        }
+                        break;
+                    case 4:
+                        if ((8 * sizeof(Py_intptr_t) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(Py_intptr_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(Py_intptr_t) - 1 > 4 * PyLong_SHIFT)) {
+                                return (Py_intptr_t) ((((((((((Py_intptr_t)digits[3]) << PyLong_SHIFT) | (Py_intptr_t)digits[2]) << PyLong_SHIFT) | (Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0])));
+                            }
+                        }
+                        break;
+                }
+            }
+#endif
+            if ((sizeof(Py_intptr_t) <= sizeof(long))) {
+                __PYX_VERIFY_RETURN_INT_EXC(Py_intptr_t, long, PyLong_AsLong(x))
+#ifdef HAVE_LONG_LONG
+            } else if ((sizeof(Py_intptr_t) <= sizeof(PY_LONG_LONG))) {
+                __PYX_VERIFY_RETURN_INT_EXC(Py_intptr_t, PY_LONG_LONG, PyLong_AsLongLong(x))
+#endif
+            }
+        }
+        {
+            Py_intptr_t val;
+            PyObject *v = __Pyx_PyNumber_IntOrLong(x);
+#if PY_MAJOR_VERSION < 3
+            if (likely(v) && !PyLong_Check(v)) {
+                PyObject *tmp = v;
+                v = PyNumber_Long(tmp);
+                Py_DECREF(tmp);
+            }
+#endif
+            if (likely(v)) {
+                int ret = -1;
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+                int one = 1; int is_little = (int)*(unsigned char *)&one;
+                unsigned char *bytes = (unsigned char *)&val;
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (Py_intptr_t) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (Py_intptr_t) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (Py_intptr_t) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (Py_intptr_t) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (Py_intptr_t) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(Py_intptr_t) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((Py_intptr_t) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(Py_intptr_t) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((Py_intptr_t) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((Py_intptr_t) 1) << (sizeof(Py_intptr_t) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
+                Py_DECREF(v);
+                if (likely(!ret))
+                    return val;
+            }
+            return (Py_intptr_t) -1;
+        }
+    } else {
+        Py_intptr_t val;
+        PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
+        if (!tmp) return (Py_intptr_t) -1;
+        val = __Pyx_PyInt_As_Py_intptr_t(tmp);
+        Py_DECREF(tmp);
+        return val;
     }
-    return name;
+raise_overflow:
+    PyErr_SetString(PyExc_OverflowError,
+        "value too large to convert to Py_intptr_t");
+    return (Py_intptr_t) -1;
+raise_neg_overflow:
+    PyErr_SetString(PyExc_OverflowError,
+        "can't convert negative value to Py_intptr_t");
+    return (Py_intptr_t) -1;
 }
+
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_Py_intptr_t(Py_intptr_t value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const Py_intptr_t neg_one = (Py_intptr_t) -1, const_zero = (Py_intptr_t) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(Py_intptr_t) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(Py_intptr_t) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(Py_intptr_t) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(Py_intptr_t) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(Py_intptr_t) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
+        return _PyLong_FromByteArray(bytes, sizeof(Py_intptr_t),
+                                     little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(Py_intptr_t));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
+        return result;
 #endif
+    }
+}
 
 /* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
@@ -15782,35 +16113,29 @@
         Py_XDECREF(py_bytes);
         Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
-/* CIntFromPyVerify */
-#define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
-    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
-#define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
-    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
-#define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
-    {\
-        func_type value = func_value;\
-        if (sizeof(target_type) < sizeof(func_type)) {\
-            if (unlikely(value != (func_type) (target_type) value)) {\
-                func_type zero = 0;\
-                if (exc && unlikely(value == (func_type)-1 && PyErr_Occurred()))\
-                    return (target_type) -1;\
-                if (is_unsigned && unlikely(value < zero))\
-                    goto raise_neg_overflow;\
-                else\
-                    goto raise_overflow;\
-            }\
-        }\
-        return (target_type) value;\
+/* FormatTypeName */
+#if CYTHON_COMPILING_IN_LIMITED_API
+static __Pyx_TypeName
+__Pyx_PyType_GetName(PyTypeObject* tp)
+{
+    PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
+                                               __pyx_n_s_name);
+    if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
+        PyErr_Clear();
+        Py_XDECREF(name);
+        name = __Pyx_NewRef(__pyx_n_s__10);
     }
+    return name;
+}
+#endif
 
 /* CIntFromPy */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
```

### Comparing `interpretable_tsne-0.0.3/src/interpretable_tsne/_utils.pxd` & `interpretable_tsne-0.0.4/src/interpretable_tsne/_utils.pxd`

 * *Files identical despite different names*

### Comparing `interpretable_tsne-0.0.3/src/interpretable_tsne/_utils.pyx` & `interpretable_tsne-0.0.4/src/interpretable_tsne/_utils.pyx`

 * *Files identical despite different names*

### Comparing `interpretable_tsne-0.0.3/src/interpretable_tsne/tsne.py` & `interpretable_tsne-0.0.4/src/interpretable_tsne/tsne.py`

 * *Files identical despite different names*

### Comparing `interpretable_tsne-0.0.3/src/interpretable_tsne/umap.py` & `interpretable_tsne-0.0.4/src/interpretable_tsne/umap.py`

 * *Files identical despite different names*

### Comparing `interpretable_tsne-0.0.3/src/interpretable_tsne.egg-info/PKG-INFO` & `interpretable_tsne-0.0.4/src/interpretable_tsne.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: interpretable_tsne
-Version: 0.0.3
-Summary: Implementation of the gradient-based t-SNE sttribution method described in our GLBIO oral presentation: 'Towards Computing Attributions for Dimensionality Reduction Techniques'
+Version: 0.0.4
+Summary: Implementation of the gradient-based t-SNE attribution method described in our GLBIO oral presentation: 'Towards Computing Attributions for Dimensionality Reduction Techniques'
 Author: Matthew Scicluna
 Author-email: Matthew Scicluna <mattcscicluna@gmail.com>
 Maintainer-email: Matthew Scicluna <mattcscicluna@gmail.com>
 License: BSD 3-Clause License
         
         Copyright 2023 Matthew Scicluna.
         
@@ -19,20 +19,20 @@
         
         THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 Project-URL: Repository, https://github.com/MattScicluna/interpretable_tsne.git
 Project-URL: Bug Tracker, https://github.com/MattScicluna/interpretable_tsne/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: COPYING
-Requires-Dist: scikit-learn==0.24.1
-Requires-Dist: scipy==1.7.0
-Requires-Dist: numpy==1.21
+Requires-Dist: scikit-learn>=0.23.0
+Requires-Dist: scipy>=1.5.0
+Requires-Dist: numpy>=1.19.2
 
 Interpretable t-SNE
 ===================
 
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
 `interpretable_tsne` is an implementation of our gradient-based attributiont technique described in our GLBIO oral presentation: 'Towards Computing Attributions for Dimensionality Reduction Techniques'.
```

### Comparing `interpretable_tsne-0.0.3/src/interpretable_tsne.egg-info/SOURCES.txt` & `interpretable_tsne-0.0.4/src/interpretable_tsne.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `interpretable_tsne-0.0.3/tests/test_bn_approx.py` & `interpretable_tsne-0.0.4/tests/test_bn_approx.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from sklearn.metrics.pairwise import pairwise_distances
 from scipy.sparse import csr_matrix
 from scipy.stats import spearmanr
 from scipy.spatial.distance import squareform
 import numpy as np
 
 #from _grad_comps import *
-from src.interpretable_tsne.tsne import pairwise_distances, _joint_probabilities, _compute_dp, _openmp_effective_n_threads, _joint_probabilities_nn, _compute_dp_bh, NearestNeighbors, TSNE
-
+from interpretable_tsne.tsne import pairwise_distances, _joint_probabilities, _compute_dp, _openmp_effective_n_threads, _joint_probabilities_nn, _compute_dp_bh, NearestNeighbors, TSNE
+# src.interpretable_tsne ...
 
 def get_dPs(data, perplexity=30):
     # helper function that computes P, dP for regular and barnes-Hut
     n_samples = data.shape[0]
     distances = pairwise_distances(data, metric="euclidean", squared=True)
     P, conditional_P, betas = _joint_probabilities(distances, perplexity, verbose=0)
     _, dP = _compute_dp(data, conditional_P, P, betas)
```

### Comparing `interpretable_tsne-0.0.3/tests/test_gradcomps.py` & `interpretable_tsne-0.0.4/tests/test_gradcomps.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from sklearn.utils._openmp_helpers import _openmp_effective_n_threads
 from sklearn.neighbors import NearestNeighbors
 from sklearn.metrics.pairwise import pairwise_distances
 from scipy.sparse import csr_matrix
 import numpy as np
 
 #from _grad_comps import *
-from src.interpretable_tsne.tsne import _joint_probabilities_nn, _compute_dp_bh, _compute_attr_bh, _kl_divergence_bh
-from src.interpretable_tsne._grad_comps import _compute_q_phi_debug
-
+from interpretable_tsne.tsne import _joint_probabilities_nn, _compute_dp_bh, _compute_attr_bh, _kl_divergence_bh
+from interpretable_tsne._grad_comps import _compute_q_phi_debug
+# src.interpretable_tsne ...
 
 class Test_compute_dp_bh(unittest.TestCase):
 
     def setUp(self):
 
         # for reproducibility
         np.random.seed(seed=42)
```

