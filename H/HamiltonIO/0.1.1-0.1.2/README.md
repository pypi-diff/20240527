# Comparing `tmp/hamiltonio-0.1.1.tar.gz` & `tmp/hamiltonio-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hamiltonio-0.1.1.tar", last modified: Sun Apr 28 20:25:15 2024, max compression
+gzip compressed data, was "hamiltonio-0.1.2.tar", last modified: Mon May 27 17:47:37 2024, max compression
```

## Comparing `hamiltonio-0.1.1.tar` & `hamiltonio-0.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-04-28 20:25:15.526590 hamiltonio-0.1.1/
-drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-04-28 20:25:15.523225 hamiltonio-0.1.1/HamiltonIO/
--rw-r--r--   0 hexu       (501) staff       (20)       87 2024-04-28 11:37:36.000000 hamiltonio-0.1.1/HamiltonIO/__init__.py
-drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-04-28 20:25:15.524721 hamiltonio-0.1.1/HamiltonIO/abacus/
--rw-r--r--   0 hexu       (501) staff       (20)       56 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/HamiltonIO/abacus/__init__.py
--rw-r--r--   0 hexu       (501) staff       (20)     7267 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/HamiltonIO/abacus/abacus_api.py
--rw-r--r--   0 hexu       (501) staff       (20)     8492 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/HamiltonIO/abacus/abacus_wrapper.py
--rw-r--r--   0 hexu       (501) staff       (20)     1562 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/HamiltonIO/abacus/orbital_api.py
--rw-r--r--   0 hexu       (501) staff       (20)    67888 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/HamiltonIO/abacus/stru_api.py
--rw-r--r--   0 hexu       (501) staff       (20)     1254 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/HamiltonIO/abacus/test_read_HRSR.py
--rw-r--r--   0 hexu       (501) staff       (20)      785 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/HamiltonIO/abacus/test_read_stru.py
-drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-04-28 20:25:15.524828 hamiltonio-0.1.1/HamiltonIO/format/
--rw-r--r--   0 hexu       (501) staff       (20)      325 2024-04-27 12:46:18.000000 hamiltonio-0.1.1/HamiltonIO/format/spmat.py
--rw-r--r--   0 hexu       (501) staff       (20)     6136 2024-04-28 13:14:07.000000 hamiltonio-0.1.1/HamiltonIO/hamiltonian.py
--rw-r--r--   0 hexu       (501) staff       (20)      241 2024-04-28 11:03:11.000000 hamiltonio-0.1.1/HamiltonIO/orbital.py
-drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-04-28 20:25:15.525025 hamiltonio-0.1.1/HamiltonIO/siesta/
--rw-r--r--   0 hexu       (501) staff       (20)      104 2024-04-27 13:50:08.000000 hamiltonio-0.1.1/HamiltonIO/siesta/__init__.py
--rw-r--r--   0 hexu       (501) staff       (20)    15997 2024-04-28 20:21:16.000000 hamiltonio-0.1.1/HamiltonIO/siesta/sisl_wrapper.py
-drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-04-28 20:25:15.525594 hamiltonio-0.1.1/HamiltonIO/wannier/
--rw-r--r--   0 hexu       (501) staff       (20)       68 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/HamiltonIO/wannier/__init__.py
--rw-r--r--   0 hexu       (501) staff       (20)    16289 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/HamiltonIO/wannier/myTB.py
--rw-r--r--   0 hexu       (501) staff       (20)     6709 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/HamiltonIO/wannier/utils.py
--rw-r--r--   0 hexu       (501) staff       (20)     4616 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/HamiltonIO/wannier/w90_parser.py
--rw-r--r--   0 hexu       (501) staff       (20)     4610 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/HamiltonIO/wannier/w90_tb_parser.py
-drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-04-28 20:25:15.525846 hamiltonio-0.1.1/HamiltonIO/wantibexos/
--rw-r--r--   0 hexu       (501) staff       (20)    12752 2024-04-27 21:04:30.000000 hamiltonio-0.1.1/HamiltonIO/wantibexos/H_extract-siesta.py
--rw-r--r--   0 hexu       (501) staff       (20)    23160 2024-04-27 13:15:06.000000 hamiltonio-0.1.1/HamiltonIO/wantibexos/output_wantibexos.py
-drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-04-28 20:25:15.525996 hamiltonio-0.1.1/HamiltonIO.egg-info/
--rw-r--r--   0 hexu       (501) staff       (20)     1537 2024-04-28 20:25:15.000000 hamiltonio-0.1.1/HamiltonIO.egg-info/PKG-INFO
--rw-r--r--   0 hexu       (501) staff       (20)      836 2024-04-28 20:25:15.000000 hamiltonio-0.1.1/HamiltonIO.egg-info/SOURCES.txt
--rw-r--r--   0 hexu       (501) staff       (20)        1 2024-04-28 20:25:15.000000 hamiltonio-0.1.1/HamiltonIO.egg-info/dependency_links.txt
--rw-r--r--   0 hexu       (501) staff       (20)      157 2024-04-28 20:25:15.000000 hamiltonio-0.1.1/HamiltonIO.egg-info/requires.txt
--rw-r--r--   0 hexu       (501) staff       (20)       11 2024-04-28 20:25:15.000000 hamiltonio-0.1.1/HamiltonIO.egg-info/top_level.txt
--rw-r--r--   0 hexu       (501) staff       (20)     1294 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/LICENSE
--rw-r--r--   0 hexu       (501) staff       (20)     1537 2024-04-28 20:25:15.526421 hamiltonio-0.1.1/PKG-INFO
--rw-r--r--   0 hexu       (501) staff       (20)      145 2024-04-28 19:16:43.000000 hamiltonio-0.1.1/README.md
--rw-r--r--   0 hexu       (501) staff       (20)     1488 2024-04-28 20:22:55.000000 hamiltonio-0.1.1/pyproject.toml
--rw-r--r--   0 hexu       (501) staff       (20)       38 2024-04-28 20:25:15.526624 hamiltonio-0.1.1/setup.cfg
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:47:37.284235 hamiltonio-0.1.2/
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:47:37.284235 hamiltonio-0.1.2/HamiltonIO/
+-rw-r--r--   0 hexu      (1032) phythema   (500)      129 2024-05-10 07:33:00.000000 hamiltonio-0.1.2/HamiltonIO/__init__.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:47:37.284235 hamiltonio-0.1.2/HamiltonIO/abacus/
+-rw-r--r--   0 hexu      (1032) phythema   (500)       56 2024-04-19 11:11:36.000000 hamiltonio-0.1.2/HamiltonIO/abacus/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     7267 2024-04-19 11:11:05.000000 hamiltonio-0.1.2/HamiltonIO/abacus/abacus_api.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     8937 2024-05-27 17:47:01.000000 hamiltonio-0.1.2/HamiltonIO/abacus/abacus_wrapper.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1562 2024-04-19 11:11:05.000000 hamiltonio-0.1.2/HamiltonIO/abacus/orbital_api.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    67888 2024-04-19 11:11:05.000000 hamiltonio-0.1.2/HamiltonIO/abacus/stru_api.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1254 2024-04-19 11:11:05.000000 hamiltonio-0.1.2/HamiltonIO/abacus/test_read_HRSR.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      785 2024-04-19 11:12:00.000000 hamiltonio-0.1.2/HamiltonIO/abacus/test_read_stru.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:47:37.284235 hamiltonio-0.1.2/HamiltonIO/format/
+-rw-r--r--   0 hexu      (1032) phythema   (500)      325 2024-04-28 11:22:37.000000 hamiltonio-0.1.2/HamiltonIO/format/spmat.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6136 2024-04-28 18:20:59.000000 hamiltonio-0.1.2/HamiltonIO/hamiltonian.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1067 2024-05-10 07:33:00.000000 hamiltonio-0.1.2/HamiltonIO/orbital.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:47:37.284235 hamiltonio-0.1.2/HamiltonIO/siesta/
+-rw-r--r--   0 hexu      (1032) phythema   (500)      104 2024-04-28 11:22:37.000000 hamiltonio-0.1.2/HamiltonIO/siesta/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    15997 2024-04-29 12:52:02.000000 hamiltonio-0.1.2/HamiltonIO/siesta/sisl_wrapper.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:47:37.284235 hamiltonio-0.1.2/HamiltonIO/wannier/
+-rw-r--r--   0 hexu      (1032) phythema   (500)      112 2024-05-10 07:33:00.000000 hamiltonio-0.1.2/HamiltonIO/wannier/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6709 2024-04-19 12:56:02.000000 hamiltonio-0.1.2/HamiltonIO/wannier/utils.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4616 2024-04-19 12:54:53.000000 hamiltonio-0.1.2/HamiltonIO/wannier/w90_parser.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4610 2024-04-19 12:54:29.000000 hamiltonio-0.1.2/HamiltonIO/wannier/w90_tb_parser.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    16305 2024-05-27 09:25:18.000000 hamiltonio-0.1.2/HamiltonIO/wannier/wannier_hamiltonian.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:47:37.284235 hamiltonio-0.1.2/HamiltonIO/wantibexos/
+-rw-r--r--   0 hexu      (1032) phythema   (500)    12752 2024-04-19 11:10:44.000000 hamiltonio-0.1.2/HamiltonIO/wantibexos/H_extract-siesta.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    23160 2024-04-28 11:22:37.000000 hamiltonio-0.1.2/HamiltonIO/wantibexos/output_wantibexos.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:47:37.284235 hamiltonio-0.1.2/HamiltonIO.egg-info/
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1537 2024-05-27 17:47:37.000000 hamiltonio-0.1.2/HamiltonIO.egg-info/PKG-INFO
+-rw-r--r--   0 hexu      (1032) phythema   (500)      851 2024-05-27 17:47:37.000000 hamiltonio-0.1.2/HamiltonIO.egg-info/SOURCES.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)        1 2024-05-27 17:47:37.000000 hamiltonio-0.1.2/HamiltonIO.egg-info/dependency_links.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)      157 2024-05-27 17:47:37.000000 hamiltonio-0.1.2/HamiltonIO.egg-info/requires.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)       11 2024-05-27 17:47:37.000000 hamiltonio-0.1.2/HamiltonIO.egg-info/top_level.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1294 2024-04-08 08:08:40.000000 hamiltonio-0.1.2/LICENSE
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1537 2024-05-27 17:47:37.284235 hamiltonio-0.1.2/PKG-INFO
+-rw-r--r--   0 hexu      (1032) phythema   (500)      145 2024-04-29 12:52:02.000000 hamiltonio-0.1.2/README.md
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1488 2024-05-27 17:47:19.000000 hamiltonio-0.1.2/pyproject.toml
+-rw-r--r--   0 hexu      (1032) phythema   (500)       38 2024-05-27 17:47:37.284235 hamiltonio-0.1.2/setup.cfg
```

### Comparing `hamiltonio-0.1.1/HamiltonIO/abacus/abacus_api.py` & `hamiltonio-0.1.2/HamiltonIO/abacus/abacus_api.py`

 * *Files identical despite different names*

### Comparing `hamiltonio-0.1.1/HamiltonIO/abacus/abacus_wrapper.py` & `hamiltonio-0.1.2/HamiltonIO/abacus/abacus_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -159,14 +159,26 @@
             nspin=4,
             binary=self.binary,
             HR_fileName=HR_filename,
             SR_fileName=SR_filename,
         )
         return nbasis, Rlist, HR, SR
 
+    def read_HSR_noncollinear_plus_SOC(self, outpath_plus_SOC=None, binary=None):
+        p = Path(outpath_plus_SOC)
+        HR_filename = str(p / "data-HR-sparse_SPIN0.csr")
+        SR_filename = str(p / "data-SR-sparse_SPIN0.csr")
+        nbasis, Rlist, HR, SR = read_HR_SR(
+            nspin=4,
+            binary=self.binary,
+            HR_fileName=HR_filename,
+            SR_fileName=None,
+        )
+        return nbasis, Rlist, HR, SR
+
     def get_models(self):
         if self.spin == "collinear":
             nbasis, Rlist, HR_up, HR_dn, SR = self.read_HSR_collinear()
             model_up = AbacusWrapper(HR_up, SR, Rlist, nbasis, nspin=1)
             model_dn = AbacusWrapper(HR_dn, SR, Rlist, nbasis, nspin=1)
             model_up.efermi = self.efermi
             model_dn.efermi = self.efermi
```

### Comparing `hamiltonio-0.1.1/HamiltonIO/abacus/orbital_api.py` & `hamiltonio-0.1.2/HamiltonIO/abacus/orbital_api.py`

 * *Files identical despite different names*

### Comparing `hamiltonio-0.1.1/HamiltonIO/abacus/stru_api.py` & `hamiltonio-0.1.2/HamiltonIO/abacus/stru_api.py`

 * *Files identical despite different names*

### Comparing `hamiltonio-0.1.1/HamiltonIO/abacus/test_read_HRSR.py` & `hamiltonio-0.1.2/HamiltonIO/abacus/test_read_HRSR.py`

 * *Files identical despite different names*

### Comparing `hamiltonio-0.1.1/HamiltonIO/abacus/test_read_stru.py` & `hamiltonio-0.1.2/HamiltonIO/abacus/test_read_stru.py`

 * *Files identical despite different names*

### Comparing `hamiltonio-0.1.1/HamiltonIO/hamiltonian.py` & `hamiltonio-0.1.2/HamiltonIO/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `hamiltonio-0.1.1/HamiltonIO/siesta/sisl_wrapper.py` & `hamiltonio-0.1.2/HamiltonIO/siesta/sisl_wrapper.py`

 * *Files identical despite different names*

### Comparing `hamiltonio-0.1.1/HamiltonIO/wannier/myTB.py` & `hamiltonio-0.1.2/HamiltonIO/wannier/wannier_hamiltonian.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import numpy as np
 import copy
 from scipy.linalg import eigh
 from scipy.sparse import csr_matrix
 from scipy.io import netcdf_file
 from collections import defaultdict
 
-from HamiltonIO.abstractTB import AbstractTB
+from HamiltonIO.hamiltonian import Hamiltonian
 from ase.atoms import Atoms
 from .utils import auto_assign_basis_name
 from .w90_parser import parse_ham, parse_xyz, parse_atoms, parse_tb
 
 
-class MyTB(AbstractTB):
+class WannierHam(Hamiltonian):
     def __init__(
         self,
         nbasis,
         data=None,
         R_degens=None,
         positions=None,
         sparse=False,
@@ -146,15 +146,15 @@
                 dtmp = copy.deepcopy(val)
                 data[key][::2, ::2] = dtmp[:norb, :norb]
                 data[key][::2, 1::2] = dtmp[:norb, norb:]
                 data[key][1::2, ::2] = dtmp[norb:, :norb]
                 data[key][1::2, 1::2] = dtmp[norb:, norb:]
         if has_xyz:
             ind, positions = auto_assign_basis_name(xred, atoms)
-        m = MyTB(nbasis=nbasis, data=data, positions=xred, R_degens=R_degens)
+        m = Hamiltonian(nbasis=nbasis, data=data, positions=xred, R_degens=R_degens)
         if has_xyz:
             nm = m.shift_position(positions)
         else:
             nm = m
         nm.set_atoms(atoms)
         return nm
```

### Comparing `hamiltonio-0.1.1/HamiltonIO/wannier/utils.py` & `hamiltonio-0.1.2/HamiltonIO/wannier/utils.py`

 * *Files identical despite different names*

### Comparing `hamiltonio-0.1.1/HamiltonIO/wannier/w90_parser.py` & `hamiltonio-0.1.2/HamiltonIO/wannier/w90_parser.py`

 * *Files identical despite different names*

### Comparing `hamiltonio-0.1.1/HamiltonIO/wannier/w90_tb_parser.py` & `hamiltonio-0.1.2/HamiltonIO/wannier/w90_tb_parser.py`

 * *Files identical despite different names*

### Comparing `hamiltonio-0.1.1/HamiltonIO/wantibexos/H_extract-siesta.py` & `hamiltonio-0.1.2/HamiltonIO/wantibexos/H_extract-siesta.py`

 * *Files identical despite different names*

### Comparing `hamiltonio-0.1.1/HamiltonIO/wantibexos/output_wantibexos.py` & `hamiltonio-0.1.2/HamiltonIO/wantibexos/output_wantibexos.py`

 * *Files identical despite different names*

### Comparing `hamiltonio-0.1.1/HamiltonIO.egg-info/PKG-INFO` & `hamiltonio-0.1.2/HamiltonIO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HamiltonIO
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for reading/writting Hamiltonian with localized basis set.
 Author-email: Xu He <mailhexu@gmail.com>
 License: BSD-2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
```

### Comparing `hamiltonio-0.1.1/HamiltonIO.egg-info/SOURCES.txt` & `hamiltonio-0.1.2/HamiltonIO.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,13 +16,13 @@
 HamiltonIO/abacus/stru_api.py
 HamiltonIO/abacus/test_read_HRSR.py
 HamiltonIO/abacus/test_read_stru.py
 HamiltonIO/format/spmat.py
 HamiltonIO/siesta/__init__.py
 HamiltonIO/siesta/sisl_wrapper.py
 HamiltonIO/wannier/__init__.py
-HamiltonIO/wannier/myTB.py
 HamiltonIO/wannier/utils.py
 HamiltonIO/wannier/w90_parser.py
 HamiltonIO/wannier/w90_tb_parser.py
+HamiltonIO/wannier/wannier_hamiltonian.py
 HamiltonIO/wantibexos/H_extract-siesta.py
 HamiltonIO/wantibexos/output_wantibexos.py
```

### Comparing `hamiltonio-0.1.1/LICENSE` & `hamiltonio-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hamiltonio-0.1.1/PKG-INFO` & `hamiltonio-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HamiltonIO
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for reading/writting Hamiltonian with localized basis set.
 Author-email: Xu He <mailhexu@gmail.com>
 License: BSD-2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
```

### Comparing `hamiltonio-0.1.1/pyproject.toml` & `hamiltonio-0.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "HamiltonIO"
-version = "0.1.1"
+version = "0.1.2"
 description = "A library for reading/writting Hamiltonian with localized basis set."
 authors = [
     {name = "Xu He", email = "mailhexu@gmail.com"},
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 license = {text = "BSD-2"}
```

