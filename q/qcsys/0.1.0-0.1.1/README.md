# Comparing `tmp/qcsys-0.1.0.tar.gz` & `tmp/qcsys-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcsys-0.1.0.tar", last modified: Mon Mar  4 10:51:12 2024, max compression
+gzip compressed data, was "qcsys-0.1.1.tar", last modified: Mon May 27 05:07:46 2024, max compression
```

## Comparing `qcsys-0.1.0.tar` & `qcsys-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-03-04 10:51:12.252742 qcsys-0.1.0/
--rw-r--r--   0 phionx     (501) staff       (20)    11357 2024-03-04 08:27:48.000000 qcsys-0.1.0/LICENSE
--rw-r--r--   0 phionx     (501) staff       (20)       43 2024-02-09 21:41:40.000000 qcsys-0.1.0/MANIFEST.in
--rw-r--r--   0 phionx     (501) staff       (20)     5769 2024-03-04 10:51:12.252516 qcsys-0.1.0/PKG-INFO
--rw-r--r--   0 phionx     (501) staff       (20)     4200 2024-03-04 10:28:33.000000 qcsys-0.1.0/README.md
-drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-03-04 10:51:12.246004 qcsys-0.1.0/docs/
--rw-r--r--   0 phionx     (501) staff       (20)      938 2024-03-04 07:52:15.000000 qcsys-0.1.0/docs/gen_ref_pages.py
-drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-03-04 10:51:12.246252 qcsys-0.1.0/docs/getting_started/
--rw-r--r--   0 phionx     (501) staff       (20)        0 2024-03-04 10:22:32.000000 qcsys-0.1.0/docs/getting_started/__init__.py
-drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-03-04 10:51:12.246474 qcsys-0.1.0/qcsys/
--rw-r--r--   0 phionx     (501) staff       (20)        5 2022-12-07 22:04:41.000000 qcsys-0.1.0/qcsys/VERSION.txt
--rw-r--r--   0 phionx     (501) staff       (20)      293 2024-02-09 21:46:29.000000 qcsys-0.1.0/qcsys/__init__.py
-drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-03-04 10:51:12.247889 qcsys-0.1.0/qcsys/common/
--rw-r--r--   0 phionx     (501) staff       (20)       44 2023-04-05 18:33:16.000000 qcsys-0.1.0/qcsys/common/__init__.py
--rw-r--r--   0 phionx     (501) staff       (20)     1778 2024-03-04 07:42:21.000000 qcsys-0.1.0/qcsys/common/utils.py
-drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-03-04 10:51:12.251260 qcsys-0.1.0/qcsys/devices/
--rw-r--r--   0 phionx     (501) staff       (20)      295 2024-02-22 22:47:02.000000 qcsys-0.1.0/qcsys/devices/__init__.py
--rw-r--r--   0 phionx     (501) staff       (20)     2532 2024-03-04 07:42:21.000000 qcsys-0.1.0/qcsys/devices/ats.py
--rw-r--r--   0 phionx     (501) staff       (20)     6208 2024-03-04 07:42:21.000000 qcsys-0.1.0/qcsys/devices/base.py
--rw-r--r--   0 phionx     (501) staff       (20)     2107 2024-03-02 06:48:30.000000 qcsys-0.1.0/qcsys/devices/drive.py
--rw-r--r--   0 phionx     (501) staff       (20)     2127 2024-03-04 07:42:21.000000 qcsys-0.1.0/qcsys/devices/fluxonium.py
--rw-r--r--   0 phionx     (501) staff       (20)      941 2024-03-02 06:48:30.000000 qcsys-0.1.0/qcsys/devices/ideal_qubit.py
--rw-r--r--   0 phionx     (501) staff       (20)     1422 2024-03-02 06:48:30.000000 qcsys-0.1.0/qcsys/devices/kno.py
--rw-r--r--   0 phionx     (501) staff       (20)     1302 2024-03-02 06:48:30.000000 qcsys-0.1.0/qcsys/devices/resonator.py
--rw-r--r--   0 phionx     (501) staff       (20)     4486 2024-03-02 06:48:30.000000 qcsys-0.1.0/qcsys/devices/squid_transmon.py
--rw-r--r--   0 phionx     (501) staff       (20)     2468 2024-03-04 07:42:21.000000 qcsys-0.1.0/qcsys/devices/system.py
--rw-r--r--   0 phionx     (501) staff       (20)     1835 2024-03-02 06:48:30.000000 qcsys-0.1.0/qcsys/devices/transmon.py
--rw-r--r--   0 phionx     (501) staff       (20)     3864 2024-03-02 06:48:30.000000 qcsys-0.1.0/qcsys/devices/transmon_single_charge_basis.py
-drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-03-04 10:51:12.251567 qcsys-0.1.0/qcsys.egg-info/
--rw-r--r--   0 phionx     (501) staff       (20)     5769 2024-03-04 10:51:12.000000 qcsys-0.1.0/qcsys.egg-info/PKG-INFO
--rw-r--r--   0 phionx     (501) staff       (20)      644 2024-03-04 10:51:12.000000 qcsys-0.1.0/qcsys.egg-info/SOURCES.txt
--rw-r--r--   0 phionx     (501) staff       (20)        1 2024-03-04 10:51:12.000000 qcsys-0.1.0/qcsys.egg-info/dependency_links.txt
--rw-r--r--   0 phionx     (501) staff       (20)      189 2024-03-04 10:51:12.000000 qcsys-0.1.0/qcsys.egg-info/requires.txt
--rw-r--r--   0 phionx     (501) staff       (20)       11 2024-03-04 10:51:12.000000 qcsys-0.1.0/qcsys.egg-info/top_level.txt
--rw-r--r--   0 phionx     (501) staff       (20)       38 2024-03-04 10:51:12.252783 qcsys-0.1.0/setup.cfg
--rw-r--r--   0 phionx     (501) staff       (20)     2117 2024-03-04 10:35:56.000000 qcsys-0.1.0/setup.py
+drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-05-27 05:07:46.184036 qcsys-0.1.1/
+-rw-r--r--   0 phionx     (501) staff       (20)    11357 2024-03-04 08:27:48.000000 qcsys-0.1.1/LICENSE
+-rw-r--r--   0 phionx     (501) staff       (20)       43 2024-02-09 21:41:40.000000 qcsys-0.1.1/MANIFEST.in
+-rw-r--r--   0 phionx     (501) staff       (20)     5800 2024-05-27 05:07:46.183787 qcsys-0.1.1/PKG-INFO
+-rw-r--r--   0 phionx     (501) staff       (20)     4232 2024-05-27 03:50:21.000000 qcsys-0.1.1/README.md
+drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-05-27 05:07:46.177080 qcsys-0.1.1/docs/
+-rw-r--r--   0 phionx     (501) staff       (20)      938 2024-03-04 07:52:15.000000 qcsys-0.1.1/docs/gen_ref_pages.py
+drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-05-27 05:07:46.177313 qcsys-0.1.1/docs/getting_started/
+-rw-r--r--   0 phionx     (501) staff       (20)        0 2024-03-04 10:22:32.000000 qcsys-0.1.1/docs/getting_started/__init__.py
+drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-05-27 05:07:46.177490 qcsys-0.1.1/qcsys/
+-rw-r--r--   0 phionx     (501) staff       (20)        5 2024-05-27 04:01:08.000000 qcsys-0.1.1/qcsys/VERSION.txt
+-rw-r--r--   0 phionx     (501) staff       (20)      293 2024-02-09 21:46:29.000000 qcsys-0.1.1/qcsys/__init__.py
+drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-05-27 05:07:46.178642 qcsys-0.1.1/qcsys/common/
+-rw-r--r--   0 phionx     (501) staff       (20)       44 2023-04-05 18:33:16.000000 qcsys-0.1.1/qcsys/common/__init__.py
+-rw-r--r--   0 phionx     (501) staff       (20)     1778 2024-03-04 07:42:21.000000 qcsys-0.1.1/qcsys/common/utils.py
+drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-05-27 05:07:46.182598 qcsys-0.1.1/qcsys/devices/
+-rw-r--r--   0 phionx     (501) staff       (20)      327 2024-05-14 21:28:11.000000 qcsys-0.1.1/qcsys/devices/__init__.py
+-rw-r--r--   0 phionx     (501) staff       (20)     2532 2024-03-04 07:42:21.000000 qcsys-0.1.1/qcsys/devices/ats.py
+-rw-r--r--   0 phionx     (501) staff       (20)    10572 2024-05-14 21:28:11.000000 qcsys-0.1.1/qcsys/devices/base.py
+-rw-r--r--   0 phionx     (501) staff       (20)     2107 2024-03-02 06:48:30.000000 qcsys-0.1.1/qcsys/devices/drive.py
+-rw-r--r--   0 phionx     (501) staff       (20)     2301 2024-05-14 21:28:11.000000 qcsys-0.1.1/qcsys/devices/fluxonium.py
+-rw-r--r--   0 phionx     (501) staff       (20)      941 2024-03-02 06:48:30.000000 qcsys-0.1.1/qcsys/devices/ideal_qubit.py
+-rw-r--r--   0 phionx     (501) staff       (20)     1422 2024-03-02 06:48:30.000000 qcsys-0.1.1/qcsys/devices/kno.py
+-rw-r--r--   0 phionx     (501) staff       (20)     1498 2024-05-21 18:54:14.000000 qcsys-0.1.1/qcsys/devices/resonator.py
+-rw-r--r--   0 phionx     (501) staff       (20)     4486 2024-03-02 06:48:30.000000 qcsys-0.1.1/qcsys/devices/squid_transmon.py
+-rw-r--r--   0 phionx     (501) staff       (20)     2461 2024-05-14 21:28:11.000000 qcsys-0.1.1/qcsys/devices/system.py
+-rw-r--r--   0 phionx     (501) staff       (20)     4959 2024-05-14 21:28:11.000000 qcsys-0.1.1/qcsys/devices/transmon.py
+-rw-r--r--   0 phionx     (501) staff       (20)     3864 2024-03-02 06:48:30.000000 qcsys-0.1.1/qcsys/devices/transmon_single_charge_basis.py
+-rw-r--r--   0 phionx     (501) staff       (20)     1844 2024-05-14 21:28:11.000000 qcsys-0.1.1/qcsys/devices/truncated_transmon.py
+-rw-r--r--   0 phionx     (501) staff       (20)      663 2024-05-14 21:28:11.000000 qcsys-0.1.1/qcsys/devices/tunable_transmon.py
+drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-05-27 05:07:46.182875 qcsys-0.1.1/qcsys.egg-info/
+-rw-r--r--   0 phionx     (501) staff       (20)     5800 2024-05-27 05:07:46.000000 qcsys-0.1.1/qcsys.egg-info/PKG-INFO
+-rw-r--r--   0 phionx     (501) staff       (20)      714 2024-05-27 05:07:46.000000 qcsys-0.1.1/qcsys.egg-info/SOURCES.txt
+-rw-r--r--   0 phionx     (501) staff       (20)        1 2024-05-27 05:07:46.000000 qcsys-0.1.1/qcsys.egg-info/dependency_links.txt
+-rw-r--r--   0 phionx     (501) staff       (20)      189 2024-05-27 05:07:46.000000 qcsys-0.1.1/qcsys.egg-info/requires.txt
+-rw-r--r--   0 phionx     (501) staff       (20)       16 2024-05-27 05:07:46.000000 qcsys-0.1.1/qcsys.egg-info/top_level.txt
+-rw-r--r--   0 phionx     (501) staff       (20)       38 2024-05-27 05:07:46.184078 qcsys-0.1.1/setup.cfg
+-rw-r--r--   0 phionx     (501) staff       (20)     2117 2024-03-04 10:35:56.000000 qcsys-0.1.1/setup.py
```

### Comparing `qcsys-0.1.0/LICENSE` & `qcsys-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qcsys-0.1.0/PKG-INFO` & `qcsys-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcsys
-Version: 0.1.0
+Version: 0.1.1
 Summary: qcsys
 Home-page: https://github.com/EQuS/qcsys
 Author: Shantanu Jha, Shoumik Chowdhury
 Author-email: shantanu.rajesh.jha@gmail.com
 License: Apache 2.0
 Project-URL: Documentation, https://equs.github.io/qcsys
 Project-URL: Source Code, https://github.com/EQuS/qcsys
@@ -62,15 +62,15 @@
 
 For more details, please visit the getting started > installation section of our [docs](https://equs.github.io/qcsys/getting_started/installation.html).
 
 ## An Example
 
 Here's an example on how to use `qcsys`:
 
-```
+```python
 import qcsys as qs
 
 
 # Devices ----
 
 
 _, Ec_a, El_a = qs.calculate_lambda_over_four_resonator_zpf(3, 50)
@@ -110,15 +110,15 @@
 
 couplings = []
 couplings.append(-g_rq * (a0 - a0_dag) @ (q0 - q0_dag))
 
 system = qs.System.create(devices, couplings=couplings)
 system.params["g_rq"] = g_rq
 
-Es, kets = system.calculate_eig_linear()
+Es, kets = system.calculate_eig()
 
 # chi ----
 χ_e = Es[1:, 1] - Es[:-1, 1]
 χ_g = Es[1:, 0] - Es[:-1, 0]
 χ = χ_e - χ_g
 
 # kerr ----
@@ -139,20 +139,21 @@
 
 This package was initially developed in early 2023 to aid in the design of a superconducting circuit device made for bosonic quantum error correction. This package was also briefly announced to the world at APS March Meeting 2023. Since then, this package has been open sourced and developed while conducting research in the Engineering Quantum Systems Group at MIT with invaluable advice from [Prof. William D. Oliver](https://equs.mit.edu/william-d-oliver/). 
 
 ## Citation
 
 Thank you for taking the time to try our package out. If you found it useful in your research, please cite us as follows:
 
-``` 
-@unpublished{jha2024jaxquantum,
+```bibtex
+@software{jha2024jaxquantum,
+  author = {Shantanu R. Jha and Shoumik Chowdhury and Max Hays and Jeff A. Grover and William D. Oliver},
   title  = {An auto differentiable and hardware accelerated software toolkit for quantum circuit design, simulation and control},
-  author = {Shantanu R. Jha, Shoumik Chowdhury, Max Hays, Jeff A. Grover, William D. Oliver},
+  url    = {https://github.com/EQuS/jaxquantum, https://github.com/EQuS/bosonic, https://github.com/EQuS/qcsys},
+  version = {0.1.0},
   year   = {2024},
-  url    = {https://github.com/EQuS/jaxquantum, https://github.com/EQuS/bosonic-jax, https://github.com/EQuS/qcsys}
 }
 ```
 > S. R. Jha, S. Chowdhury, M. Hays, J. A. Grover, W. D. Oliver. An auto differentiable and hardware accelerated software toolkit for quantum circuit design, simulation and control (2024), in preparation.
 
 
 ## Contributions & Contact
```

### Comparing `qcsys-0.1.0/README.md` & `qcsys-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 For more details, please visit the getting started > installation section of our [docs](https://equs.github.io/qcsys/getting_started/installation.html).
 
 ## An Example
 
 Here's an example on how to use `qcsys`:
 
-```
+```python
 import qcsys as qs
 
 
 # Devices ----
 
 
 _, Ec_a, El_a = qs.calculate_lambda_over_four_resonator_zpf(3, 50)
@@ -68,15 +68,15 @@
 
 couplings = []
 couplings.append(-g_rq * (a0 - a0_dag) @ (q0 - q0_dag))
 
 system = qs.System.create(devices, couplings=couplings)
 system.params["g_rq"] = g_rq
 
-Es, kets = system.calculate_eig_linear()
+Es, kets = system.calculate_eig()
 
 # chi ----
 χ_e = Es[1:, 1] - Es[:-1, 1]
 χ_g = Es[1:, 0] - Es[:-1, 0]
 χ = χ_e - χ_g
 
 # kerr ----
@@ -97,21 +97,22 @@
 
 This package was initially developed in early 2023 to aid in the design of a superconducting circuit device made for bosonic quantum error correction. This package was also briefly announced to the world at APS March Meeting 2023. Since then, this package has been open sourced and developed while conducting research in the Engineering Quantum Systems Group at MIT with invaluable advice from [Prof. William D. Oliver](https://equs.mit.edu/william-d-oliver/). 
 
 ## Citation
 
 Thank you for taking the time to try our package out. If you found it useful in your research, please cite us as follows:
 
-``` 
-@unpublished{jha2024jaxquantum,
+```bibtex
+@software{jha2024jaxquantum,
+  author = {Shantanu R. Jha and Shoumik Chowdhury and Max Hays and Jeff A. Grover and William D. Oliver},
   title  = {An auto differentiable and hardware accelerated software toolkit for quantum circuit design, simulation and control},
-  author = {Shantanu R. Jha, Shoumik Chowdhury, Max Hays, Jeff A. Grover, William D. Oliver},
+  url    = {https://github.com/EQuS/jaxquantum, https://github.com/EQuS/bosonic, https://github.com/EQuS/qcsys},
+  version = {0.1.0},
   year   = {2024},
-  url    = {https://github.com/EQuS/jaxquantum, https://github.com/EQuS/bosonic-jax, https://github.com/EQuS/qcsys}
 }
 ```
 > S. R. Jha, S. Chowdhury, M. Hays, J. A. Grover, W. D. Oliver. An auto differentiable and hardware accelerated software toolkit for quantum circuit design, simulation and control (2024), in preparation.
 
 
 ## Contributions & Contact
 
-This package is open source and, as such, very open to contributions. Please don't hesitate to open an issue, report a bug, request a feature, or create a pull request. We are also open to deeper collaborations to create a tool that is more useful for everyone. If a discussion would be helpful, please email [shanjha@mit.edu](mailto:shanjha@mit.edu) to set up a meeting. 
+This package is open source and, as such, very open to contributions. Please don't hesitate to open an issue, report a bug, request a feature, or create a pull request. We are also open to deeper collaborations to create a tool that is more useful for everyone. If a discussion would be helpful, please email [shanjha@mit.edu](mailto:shanjha@mit.edu) to set up a meeting.
```

### Comparing `qcsys-0.1.0/docs/gen_ref_pages.py` & `qcsys-0.1.1/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `qcsys-0.1.0/qcsys/common/utils.py` & `qcsys-0.1.1/qcsys/common/utils.py`

 * *Files identical despite different names*

### Comparing `qcsys-0.1.0/qcsys/devices/ats.py` & `qcsys-0.1.1/qcsys/devices/ats.py`

 * *Files identical despite different names*

### Comparing `qcsys-0.1.0/qcsys/devices/base.py` & `qcsys-0.1.1/qcsys/devices/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,127 @@
+
 """ Base device."""
 
 from abc import abstractmethod, ABC
+from enum import Enum
 from typing import Dict, Any, List
 
 from flax import struct
 from jax import config, Array
 import jax.numpy as jnp
 import matplotlib.pyplot as plt
 
 from qcsys.common.utils import harm_osc_wavefunction
 import jaxquantum as jqt
 
 config.update("jax_enable_x64", True)
 
 
+class BasisTypes(str, Enum):
+    fock = "fock"
+    charge = "charge"
+
+    @classmethod
+    def from_str(cls, string: str):
+        return cls(string)
+
+    def __str__(self):
+        return self.value
+
+    def __repr__(self):
+        return self.__str__()
+
+    def __eq__(self, other):
+        return self.value == other.value
+
+    def __ne__(self, other):
+        return self.value != other.value
+
+    def __hash__(self):
+        return hash(self.value)
+
+class HamiltonianTypes(str, Enum):
+    linear = "linear"
+    truncated = "truncated"
+    full = "full"
+
+    @classmethod
+    def from_str(cls, string: str):
+        return cls(string)
+
+    def __str__(self):
+        return self.value
+
+    def __repr__(self):
+        return self.__str__()
+
+    def __eq__(self, other):
+        return self.value == other.value
+
+    def __ne__(self, other):
+        return self.value != other.value
+
+    def __hash__(self):
+        return hash(self.value)
+
 @struct.dataclass
 class Device(ABC):
     N: int = struct.field(pytree_node=False)
     N_pre_diag: int = struct.field(pytree_node=False)
     params: Dict[str, Any]
     _label: int = struct.field(pytree_node=False)
-    _use_linear: bool = struct.field(pytree_node=False)
+    _basis: BasisTypes = struct.field(pytree_node=False)
+    _hamiltonian: HamiltonianTypes = struct.field(pytree_node=False)
 
     @classmethod
-    def create(cls, N, params, label=0, use_linear=True, N_pre_diag=None):
+    def param_validation(cls, N, N_pre_diag, params, hamiltonian, basis):
+        """ This can be overridden by subclasses."""
+        pass
+
+    @classmethod
+    def create(cls, N, params, label=0, use_linear=None, N_pre_diag=None, hamiltonian: HamiltonianTypes = None, basis: BasisTypes = None):
         if N_pre_diag is None:
             N_pre_diag = N
-        return cls(N, N_pre_diag, params, label, use_linear)
+
+        _basis = basis if basis is not None else BasisTypes.fock
+        _hamiltonian = hamiltonian if hamiltonian is not None else HamiltonianTypes.full
+        if use_linear is not None and use_linear:
+            _hamiltonian = HamiltonianTypes.linear
+        
+        cls.param_validation(N, N_pre_diag, params, _hamiltonian, _basis)
+
+        return cls(N, N_pre_diag, params, label, _basis, _hamiltonian)
+    
+    @property
+    def basis(self):
+        return self._basis
+    
+    @property
+    def hamiltonian(self):
+        return self._hamiltonian
 
     @property
     def label(self):
         return self.__class__.__name__ + str(self._label)
 
     @property
     def linear_ops(self):
         return self.common_ops()
+    
+    @property
+    def original_ops(self):
+        return self.common_ops()
 
     @property
     def ops(self):
         return self.full_ops()
 
     @abstractmethod
     def common_ops(self) -> Dict[str, jqt.Qarray]:
-        """Set up common ops in the linear basis."""
+        """Set up common ops in the specified basis."""
 
     @abstractmethod
     def get_linear_ω(self):
         """Get frequency of linear terms."""
 
     @abstractmethod
     def get_H_linear(self):
@@ -56,21 +131,26 @@
     def get_H_full(self):
         """Return full H."""
 
     def get_H(self):
         """
         Return diagonalized H. Explicitly keep only diagonal elements of matrix.
         """
-        return self.get_op_in_H_eigenbasis(self._get_H_in_linear_basis()).keep_only_diag_elements()
+        return self.get_op_in_H_eigenbasis(self._get_H_in_original_basis()).keep_only_diag_elements()
 
-    def _get_H_in_linear_basis(self):
-        return self.get_H_linear() if self._use_linear else self.get_H_full()
+    def _get_H_in_original_basis(self):
+        """ This returns the Hamiltonian in the original specified basis. This can be overridden by subclasses."""
 
+        if self.hamiltonian == HamiltonianTypes.linear:
+            return self.get_H_linear()
+        elif self.hamiltonian == HamiltonianTypes.full:
+            return self.get_H_full()
+        
     def _calculate_eig_systems(self):
-        evs, evecs = jnp.linalg.eigh(self._get_H_in_linear_basis().data)  # Hermitian
+        evs, evecs = jnp.linalg.eigh(self._get_H_in_original_basis().data)  # Hermitian
         idxs_sorted = jnp.argsort(evs)
         return evs[idxs_sorted], evecs[:, idxs_sorted]
 
     @property
     def eig_systems(self):
         eig_systems = {}
         eig_systems["vals"], eig_systems["vecs"] = self._calculate_eig_systems()
@@ -126,71 +206,123 @@
 
 @struct.dataclass
 class FluxDevice(Device):
     @abstractmethod
     def phi_zpf(self):
         """Return Phase ZPF."""
 
-    def calculate_wavefunctions(self, phi_vals):
+    def _calculate_wavefunctions_fock(self, phi_vals):
         """Calculate wavefunctions at phi_exts."""
         phi_osc = self.phi_zpf() * jnp.sqrt(2) # length of oscillator
         phi_vals = jnp.array(phi_vals)
 
         # calculate basis functions
         basis_functions = []
         for n in range(self.N_pre_diag):
             basis_functions.append(
-                harm_osc_wavefunction(n, phi_vals, phi_osc)
+                harm_osc_wavefunction(n, phi_vals, jnp.real(phi_osc))
             )
         basis_functions = jnp.array(basis_functions)
 
         # transform to better diagonal basis
         basis_functions_in_H_eigenbasis = self.get_vec_data_in_H_eigenbasis(basis_functions)
         
         # the below is equivalent to evecs_in_H_eigenbasis @ basis_functions_in_H_eigenbasis
         # since evecs in H_eigenbasis is diagonal, i.e. the identity matrix
         wavefunctions = basis_functions_in_H_eigenbasis 
         return wavefunctions
     
+    def _calculate_wavefunctions_charge(self, phi_vals):
+        phi_vals = jnp.array(phi_vals)
+
+        # calculate basis functions
+        basis_functions = []
+        n_max = (self.N_pre_diag - 1) // 2
+        for n in jnp.arange(-n_max, n_max + 1):
+            basis_functions.append(
+                1/(jnp.sqrt(2*jnp.pi)) * jnp.exp(1j * n * (2*jnp.pi*phi_vals))
+            )
+        basis_functions = jnp.array(basis_functions)
+
+        # transform to better diagonal basis
+        basis_functions_in_H_eigenbasis = self.get_vec_data_in_H_eigenbasis(basis_functions)
+        
+        # the below is equivalent to evecs_in_H_eigenbasis @ basis_functions_in_H_eigenbasis
+        # since evecs in H_eigenbasis is diagonal, i.e. the identity matrix
+        phase_correction_factors =  (1j**(jnp.arange(0,self.N_pre_diag))).reshape(self.N_pre_diag,1) # TODO: review why these are needed...
+        wavefunctions = basis_functions_in_H_eigenbasis * phase_correction_factors
+        return wavefunctions
+    
     @abstractmethod
     def potential(self, phi):
-        """Return potential energy as a funciton of phi."""
+        """Return potential energy as a function of phi."""
+
+    def plot_wavefunctions(self, phi_vals, max_n=None, which=None, ax=None, mode="abs"):
 
+        if self.basis == BasisTypes.fock:
+            _calculate_wavefunctions = self._calculate_wavefunctions_fock
+        elif self.basis == BasisTypes.charge:
+            _calculate_wavefunctions = self._calculate_wavefunctions_charge
+        else:
+            raise NotImplementedError(f"The {self.basis} is not yet supported for plotting wavefunctions.")
 
-    def plot_wavefunctions(self, phi_vals):
         """Plot wavefunctions at phi_exts."""
-        wavefunctions = self.calculate_wavefunctions(phi_vals)
+        wavefunctions = _calculate_wavefunctions(phi_vals)
         energy_levels = self.eig_systems["vals"][:self.N]
 
         potential = self.potential(phi_vals)
 
-        fig, axs = plt.subplots(1,1, figsize=(6,5), dpi=200, squeeze=False)
+        if ax is None:
+            fig, ax = plt.subplots(1,1, figsize = (3.5, 2.5), dpi = 1000)
+        else:
+            fig = ax.get_figure()
 
         min_val = None
         max_val = None
 
-        ax = axs[0][0]
-        for n in range(self.N):
-            wf_vals = wavefunctions[n, :].real + energy_levels[n]
+        assert max_n is None or which is None, "Can't specify both max_n and which"
+
+        max_n = self.N if max_n is None else max_n
+        levels = range(max_n) if which is None else which
+
+        for n in levels:
+            if mode == "abs":
+                wf_vals = jnp.abs(wavefunctions[n, :])**2
+            elif mode == "real":
+                wf_vals = wavefunctions[n, :].real
+            elif mode == "imag":
+                wf_vals = wavefunctions[n, :].imag
+
+            wf_vals += energy_levels[n]
             curr_min_val = min(wf_vals)
             curr_max_val = max(wf_vals)
 
             if min_val is None or curr_min_val < min_val:
                 min_val = curr_min_val
 
             if max_val is None or curr_max_val > max_val:
                 max_val = curr_max_val
 
-            ax.plot(phi_vals, wf_vals, label=f"{n}")
+            ax.plot(phi_vals, wf_vals, label=f"$|${n}$\\rangle$", linestyle = '-', linewidth = 1)
+            ax.fill_between(phi_vals, energy_levels[n], wf_vals, alpha=0.5)
         
-        ax.plot(phi_vals, potential, label="potential", color="black", linestyle="--")
+        ax.plot(phi_vals, potential, label="potential", color="black", linestyle = '-', linewidth = 1)
 
         ax.set_ylim([min_val-1, max_val+1])
 
-        ax.set_xlabel(r"$\varphi/\Phi_0$")
+        ax.set_xlabel(r"$\Phi/\Phi_0$")
         ax.set_ylabel(r"Energy [GHz]")
 
+        if mode == "abs":
+            title_str = r"$|\psi_n(\Phi)|^2$"
+        elif mode == "real":
+            title_str = r"Re($\psi_n(\Phi)$)"
+        elif mode == "imag":
+            title_str = r"Im($\psi_n(\Phi)$)"
+
+        ax.set_title(f"{title_str}")
+
         plt.legend(fontsize=6)
         fig.tight_layout()
 
-        return axs
+        return ax
```

### Comparing `qcsys-0.1.0/qcsys/devices/drive.py` & `qcsys-0.1.1/qcsys/devices/drive.py`

 * *Files identical despite different names*

### Comparing `qcsys-0.1.0/qcsys/devices/fluxonium.py` & `qcsys-0.1.1/qcsys/devices/fluxonium.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ Fluxonium."""
 
 from flax import struct
 from jax import config
 import jaxquantum as jqt
 import jax.numpy as jnp
 
-from qcsys.devices.base import FluxDevice
+from qcsys.devices.base import FluxDevice, HamiltonianTypes
 
 config.update("jax_enable_x64", True)
 
 
 @struct.dataclass
 class Fluxonium(FluxDevice):
     """
@@ -65,9 +65,14 @@
         H = self.get_H_linear() - self.params["Ej"] * Hcos
         return H
 
     def potential(self, phi):
         """Return potential energy for a given phi."""
         phi_ext = self.params["phi_ext"]
         V_linear = 0.5 * self.params["El"] * (2 * jnp.pi * phi) ** 2
+    
+        if self.hamiltonian == HamiltonianTypes.linear:
+            return V_linear
+        
         V_nonlinear = -self.params["Ej"] * jnp.cos(2.0 * jnp.pi * (phi - phi_ext))
-        return V_linear + V_nonlinear
+        if self.hamiltonian == HamiltonianTypes.full:
+            return V_linear + V_nonlinear
```

### Comparing `qcsys-0.1.0/qcsys/devices/ideal_qubit.py` & `qcsys-0.1.1/qcsys/devices/ideal_qubit.py`

 * *Files identical despite different names*

### Comparing `qcsys-0.1.0/qcsys/devices/kno.py` & `qcsys-0.1.1/qcsys/devices/kno.py`

 * *Files identical despite different names*

### Comparing `qcsys-0.1.0/qcsys/devices/resonator.py` & `qcsys-0.1.1/qcsys/devices/resonator.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,28 +19,34 @@
         ops = {}
         
         N = self.N_pre_diag
         ops["id"] = jqt.identity(N)
         ops["a"] = jqt.destroy(N)
         ops["a_dag"] = jqt.create(N)
         ops["phi"] = self.phi_zpf()*(ops["a"] + ops["a_dag"])  
+        ops["n"] = 1j * self.n_zpf() * (ops["a_dag"] - ops["a"])
+
         return ops
 
     def phi_zpf(self):
         """Return Phase ZPF."""
         return (2*self.params["Ec"]/self.params["El"])**(.25)
     
+    def n_zpf(self):
+        n_zpf = (self.params["El"] / (32.0 * self.params["Ec"])) ** (0.25)
+        return n_zpf
+    
     def get_linear_ω(self):
         """Get frequency of linear terms."""
         return jnp.sqrt(8*self.params["El"]*self.params["Ec"])
     
     def get_H_linear(self):
         """Return linear terms in H."""
         w = self.get_linear_ω()
-        return w*self.linear_ops["a_dag"]@self.linear_ops["a"]
+        return w*(self.linear_ops["a_dag"]@self.linear_ops["a"] + 1/2)
   
     def get_H_full(self):
         """Return full H in linear basis."""
         return self.get_H_linear()
     
     def potential(self, phi):
         """Return potential energy for a given phi."""
```

### Comparing `qcsys-0.1.0/qcsys/devices/squid_transmon.py` & `qcsys-0.1.1/qcsys/devices/squid_transmon.py`

 * *Files identical despite different names*

### Comparing `qcsys-0.1.0/qcsys/devices/system.py` & `qcsys-0.1.1/qcsys/devices/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,10 +84,10 @@
         return H
     
     def get_H(self):
         H_bare = self.get_H_bare()
         H_couplings = self.get_H_couplings()
         return H_bare + H_couplings
 
-    def calculate_eig_linear(self):
+    def calculate_eig(self):
         H = self.get_H()
         return calculate_eig(self.Ns, H)
```

### Comparing `qcsys-0.1.0/qcsys/devices/transmon.py` & `qcsys-0.1.1/qcsys/devices/truncated_transmon.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from qcsys.devices.base import FluxDevice
 
 config.update("jax_enable_x64", True)
 
 
 @struct.dataclass
-class Transmon(FluxDevice):
+class TruncatedTransmon(FluxDevice):
     """
     Transmon Device.
     """
 
     def common_ops(self):
         """ Written in the linear basis. """
```

### Comparing `qcsys-0.1.0/qcsys/devices/transmon_single_charge_basis.py` & `qcsys-0.1.1/qcsys/devices/transmon_single_charge_basis.py`

 * *Files identical despite different names*

### Comparing `qcsys-0.1.0/qcsys.egg-info/PKG-INFO` & `qcsys-0.1.1/qcsys.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcsys
-Version: 0.1.0
+Version: 0.1.1
 Summary: qcsys
 Home-page: https://github.com/EQuS/qcsys
 Author: Shantanu Jha, Shoumik Chowdhury
 Author-email: shantanu.rajesh.jha@gmail.com
 License: Apache 2.0
 Project-URL: Documentation, https://equs.github.io/qcsys
 Project-URL: Source Code, https://github.com/EQuS/qcsys
@@ -62,15 +62,15 @@
 
 For more details, please visit the getting started > installation section of our [docs](https://equs.github.io/qcsys/getting_started/installation.html).
 
 ## An Example
 
 Here's an example on how to use `qcsys`:
 
-```
+```python
 import qcsys as qs
 
 
 # Devices ----
 
 
 _, Ec_a, El_a = qs.calculate_lambda_over_four_resonator_zpf(3, 50)
@@ -110,15 +110,15 @@
 
 couplings = []
 couplings.append(-g_rq * (a0 - a0_dag) @ (q0 - q0_dag))
 
 system = qs.System.create(devices, couplings=couplings)
 system.params["g_rq"] = g_rq
 
-Es, kets = system.calculate_eig_linear()
+Es, kets = system.calculate_eig()
 
 # chi ----
 χ_e = Es[1:, 1] - Es[:-1, 1]
 χ_g = Es[1:, 0] - Es[:-1, 0]
 χ = χ_e - χ_g
 
 # kerr ----
@@ -139,20 +139,21 @@
 
 This package was initially developed in early 2023 to aid in the design of a superconducting circuit device made for bosonic quantum error correction. This package was also briefly announced to the world at APS March Meeting 2023. Since then, this package has been open sourced and developed while conducting research in the Engineering Quantum Systems Group at MIT with invaluable advice from [Prof. William D. Oliver](https://equs.mit.edu/william-d-oliver/). 
 
 ## Citation
 
 Thank you for taking the time to try our package out. If you found it useful in your research, please cite us as follows:
 
-``` 
-@unpublished{jha2024jaxquantum,
+```bibtex
+@software{jha2024jaxquantum,
+  author = {Shantanu R. Jha and Shoumik Chowdhury and Max Hays and Jeff A. Grover and William D. Oliver},
   title  = {An auto differentiable and hardware accelerated software toolkit for quantum circuit design, simulation and control},
-  author = {Shantanu R. Jha, Shoumik Chowdhury, Max Hays, Jeff A. Grover, William D. Oliver},
+  url    = {https://github.com/EQuS/jaxquantum, https://github.com/EQuS/bosonic, https://github.com/EQuS/qcsys},
+  version = {0.1.0},
   year   = {2024},
-  url    = {https://github.com/EQuS/jaxquantum, https://github.com/EQuS/bosonic-jax, https://github.com/EQuS/qcsys}
 }
 ```
 > S. R. Jha, S. Chowdhury, M. Hays, J. A. Grover, W. D. Oliver. An auto differentiable and hardware accelerated software toolkit for quantum circuit design, simulation and control (2024), in preparation.
 
 
 ## Contributions & Contact
```

### Comparing `qcsys-0.1.0/qcsys.egg-info/SOURCES.txt` & `qcsys-0.1.1/qcsys.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -20,8 +20,10 @@
 qcsys/devices/fluxonium.py
 qcsys/devices/ideal_qubit.py
 qcsys/devices/kno.py
 qcsys/devices/resonator.py
 qcsys/devices/squid_transmon.py
 qcsys/devices/system.py
 qcsys/devices/transmon.py
-qcsys/devices/transmon_single_charge_basis.py
+qcsys/devices/transmon_single_charge_basis.py
+qcsys/devices/truncated_transmon.py
+qcsys/devices/tunable_transmon.py
```

### Comparing `qcsys-0.1.0/setup.py` & `qcsys-0.1.1/setup.py`

 * *Files identical despite different names*

