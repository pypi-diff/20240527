# Comparing `tmp/simular_evm-0.2.2.tar.gz` & `tmp/simular_evm-0.2.3.tar.gz`

## Comparing `simular_evm-0.2.2.tar` & `simular_evm-0.2.3.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 simular_evm-0.2.2/Cargo.toml
--rw-r--r--   0     1001      127     3198 2024-04-05 13:15:29.000000 simular_evm-0.2.2/.github/workflows/build-release.yml
--rw-r--r--   0     1001      127     1576 2024-04-05 13:15:29.000000 simular_evm-0.2.2/.github/workflows/mdbook.yml
--rw-r--r--   0     1001      127     1292 2024-04-05 13:15:29.000000 simular_evm-0.2.2/.github/workflows/test_pypi.yml
--rw-r--r--   0     1001      127      610 2024-04-05 13:15:29.000000 simular_evm-0.2.2/.gitignore
--rw-r--r--   0     1001      127      817 2024-04-05 13:15:29.000000 simular_evm-0.2.2/.readthedocs.yaml
--rw-r--r--   0     1001      127    11354 2024-04-05 13:15:29.000000 simular_evm-0.2.2/LICENSE
--rw-r--r--   0     1001      127      327 2024-04-05 13:15:29.000000 simular_evm-0.2.2/Makefile
--rw-r--r--   0     1001      127     1805 2024-04-05 13:15:29.000000 simular_evm-0.2.2/README.md
--rw-r--r--   0     1001      127      806 2024-04-05 13:15:29.000000 simular_evm-0.2.2/bench/simple.py
--rw-r--r--   0     1001      127     1116 2024-04-05 13:15:29.000000 simular_evm-0.2.2/docs/conf.py
--rw-r--r--   0     1001      127     2645 2024-04-05 13:15:29.000000 simular_evm-0.2.2/docs/contract.rst
--rw-r--r--   0     1001      127       17 2024-04-05 13:15:29.000000 simular_evm-0.2.2/docs/evm.rst
--rw-r--r--   0     1001      127      854 2024-04-05 13:15:29.000000 simular_evm-0.2.2/docs/getstarted.rst
--rw-r--r--   0     1001      127     1398 2024-04-05 13:15:29.000000 simular_evm-0.2.2/docs/index.rst
--rw-r--r--   0     1001      127      800 2024-04-05 13:15:29.000000 simular_evm-0.2.2/docs/make.bat
--rw-r--r--   0     1001      127       37 2024-04-05 13:15:29.000000 simular_evm-0.2.2/docs/requirements.txt
--rw-r--r--   0     1001      127      145 2024-04-05 13:15:29.000000 simular_evm-0.2.2/docs/toc.rst
--rw-r--r--   0     1001      127       31 2024-04-05 13:15:29.000000 simular_evm-0.2.2/docs/utils.rst
--rw-r--r--   0     1001      127       86 2024-04-05 13:15:29.000000 simular_evm-0.2.2/simular/__init__.py
--rw-r--r--   0     1001      127     4876 2024-04-05 13:15:29.000000 simular_evm-0.2.2/simular/contract.py
--rw-r--r--   0     1001      127     4081 2024-04-05 13:15:29.000000 simular_evm-0.2.2/simular/utils.py
--rw-r--r--   0     1001      127      541 2024-04-05 13:15:29.000000 simular_evm-0.2.2/src/lib.rs
--rw-r--r--   0     1001      127     2509 2024-04-05 13:15:29.000000 simular_evm-0.2.2/src/pyabi.rs
--rw-r--r--   0     1001      127     6141 2024-04-05 13:15:29.000000 simular_evm-0.2.2/src/pyevm.rs
--rw-r--r--   0     1001      127      753 2024-04-05 13:15:29.000000 simular_evm-0.2.2/tests/conftest.py
--rw-r--r--   0     1001      127    26594 2024-04-05 13:15:29.000000 simular_evm-0.2.2/tests/fixtures/KitchenSink.json
--rw-r--r--   0     1001      127      787 2024-04-05 13:15:29.000000 simular_evm-0.2.2/tests/fixtures/contracts/KitchenSink.sol
--rw-r--r--   0     1001      127      653 2024-04-05 13:15:29.000000 simular_evm-0.2.2/tests/fixtures/contracts/MockERC20.sol
--rw-r--r--   0     1001      127     4031 2024-04-05 13:15:29.000000 simular_evm-0.2.2/tests/fixtures/erc20.abi
--rw-r--r--   0     1001      127     8722 2024-04-05 13:15:29.000000 simular_evm-0.2.2/tests/fixtures/erc20.bin
--rw-r--r--   0     1001      127      288 2024-04-05 13:15:29.000000 simular_evm-0.2.2/tests/fixtures/usdc_addresses.json
--rw-r--r--   0     1001      127     2221 2024-04-05 13:15:29.000000 simular_evm-0.2.2/tests/test_contract.py
--rw-r--r--   0     1001      127     1633 2024-04-05 13:15:29.000000 simular_evm-0.2.2/tests/test_pyabi.py
--rw-r--r--   0     1001      127     1592 2024-04-05 13:15:29.000000 simular_evm-0.2.2/tests/test_pyevm.py
--rw-r--r--   0     1001      127    90177 2024-04-05 13:15:35.000000 simular_evm-0.2.2/Cargo.lock
--rw-r--r--   0     1001      127     1429 2024-04-05 13:15:29.000000 simular_evm-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2785 1970-01-01 00:00:00.000000 simular_evm-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 simular_evm-0.2.3/Cargo.toml
+-rw-r--r--   0     1001      127     3198 2024-05-27 14:27:40.000000 simular_evm-0.2.3/.github/workflows/build-release.yml
+-rw-r--r--   0     1001      127     1576 2024-05-27 14:27:40.000000 simular_evm-0.2.3/.github/workflows/mdbook.yml
+-rw-r--r--   0     1001      127     1292 2024-05-27 14:27:40.000000 simular_evm-0.2.3/.github/workflows/test_pypi.yml
+-rw-r--r--   0     1001      127      610 2024-05-27 14:27:40.000000 simular_evm-0.2.3/.gitignore
+-rw-r--r--   0     1001      127      817 2024-05-27 14:27:40.000000 simular_evm-0.2.3/.readthedocs.yaml
+-rw-r--r--   0     1001      127    11354 2024-05-27 14:27:40.000000 simular_evm-0.2.3/LICENSE
+-rw-r--r--   0     1001      127      340 2024-05-27 14:27:40.000000 simular_evm-0.2.3/Makefile
+-rw-r--r--   0     1001      127     1805 2024-05-27 14:27:40.000000 simular_evm-0.2.3/README.md
+-rw-r--r--   0     1001      127      806 2024-05-27 14:27:40.000000 simular_evm-0.2.3/bench/simple.py
+-rw-r--r--   0     1001      127     1116 2024-05-27 14:27:40.000000 simular_evm-0.2.3/docs/conf.py
+-rw-r--r--   0     1001      127     5868 2024-05-27 14:27:40.000000 simular_evm-0.2.3/docs/contract.rst
+-rw-r--r--   0     1001      127     3617 2024-05-27 14:27:40.000000 simular_evm-0.2.3/docs/evm.rst
+-rw-r--r--   0     1001      127     3691 2024-05-27 14:27:40.000000 simular_evm-0.2.3/docs/getstarted.rst
+-rw-r--r--   0     1001      127     1279 2024-05-27 14:27:40.000000 simular_evm-0.2.3/docs/index.rst
+-rw-r--r--   0     1001      127      800 2024-05-27 14:27:40.000000 simular_evm-0.2.3/docs/make.bat
+-rw-r--r--   0     1001      127       37 2024-05-27 14:27:40.000000 simular_evm-0.2.3/docs/requirements.txt
+-rw-r--r--   0     1001      127       72 2024-05-27 14:27:40.000000 simular_evm-0.2.3/docs/toc.rst
+-rw-r--r--   0     1001      127     3553 2024-05-27 14:27:40.000000 simular_evm-0.2.3/docs/utils.rst
+-rw-r--r--   0     1001      127       86 2024-05-27 14:27:40.000000 simular_evm-0.2.3/simular/__init__.py
+-rw-r--r--   0     1001      127     5203 2024-05-27 14:27:40.000000 simular_evm-0.2.3/simular/contract.py
+-rw-r--r--   0     1001      127     4011 2024-05-27 14:27:40.000000 simular_evm-0.2.3/simular/simular.pyi
+-rw-r--r--   0     1001      127     4084 2024-05-27 14:27:40.000000 simular_evm-0.2.3/simular/utils.py
+-rw-r--r--   0     1001      127      541 2024-05-27 14:27:40.000000 simular_evm-0.2.3/src/lib.rs
+-rw-r--r--   0     1001      127     2509 2024-05-27 14:27:40.000000 simular_evm-0.2.3/src/pyabi.rs
+-rw-r--r--   0     1001      127     6705 2024-05-27 14:27:40.000000 simular_evm-0.2.3/src/pyevm.rs
+-rw-r--r--   0     1001      127      895 2024-05-27 14:27:40.000000 simular_evm-0.2.3/tests/conftest.py
+-rw-r--r--   0     1001      127     4995 2024-05-27 14:27:40.000000 simular_evm-0.2.3/tests/fixtures/BlockMeta.json
+-rw-r--r--   0     1001      127    65695 2024-05-27 14:27:40.000000 simular_evm-0.2.3/tests/fixtures/KitchenSink.json
+-rw-r--r--   0     1001      127      787 2024-05-27 14:27:40.000000 simular_evm-0.2.3/tests/fixtures/contracts/KitchenSink.sol
+-rw-r--r--   0     1001      127      653 2024-05-27 14:27:40.000000 simular_evm-0.2.3/tests/fixtures/contracts/MockERC20.sol
+-rw-r--r--   0     1001      127     4031 2024-05-27 14:27:40.000000 simular_evm-0.2.3/tests/fixtures/erc20.abi
+-rw-r--r--   0     1001      127     8722 2024-05-27 14:27:40.000000 simular_evm-0.2.3/tests/fixtures/erc20.bin
+-rw-r--r--   0     1001      127     2221 2024-05-27 14:27:40.000000 simular_evm-0.2.3/tests/test_contract.py
+-rw-r--r--   0     1001      127     2101 2024-05-27 14:27:40.000000 simular_evm-0.2.3/tests/test_pyabi.py
+-rw-r--r--   0     1001      127     2135 2024-05-27 14:27:40.000000 simular_evm-0.2.3/tests/test_pyevm.py
+-rw-r--r--   0     1001      127    89674 2024-05-27 14:27:46.000000 simular_evm-0.2.3/Cargo.lock
+-rw-r--r--   0     1001      127     1432 2024-05-27 14:27:40.000000 simular_evm-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2790 1970-01-01 00:00:00.000000 simular_evm-0.2.3/PKG-INFO
```

### Comparing `simular_evm-0.2.2/Cargo.toml` & `simular_evm-0.2.3/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "simular"
-version = "0.2.2"
+version = "0.2.3"
 edition = "2021"
 authors = ["Dave Bryson"]
 readme = "README.md"
 license = "Apache-2.0"
 description = "smart-contract api and embedded ethereum virtual machine"
 repository = "https://github.com/simular-fi/simular"
 homepage = "https://github.com/simular-fi/simular"
@@ -22,15 +22,15 @@
 alloy-primitives = { version = "0.7.0", default-features = false }
 serde = "1.0.165"
 serde_json = "1.0.99"
 
 hex = { version = "0.4.3", features = ["serde"] }
 pyo3 = { version = "0.20.0", features = ["multiple-pymethods", "anyhow"] }
 
-simular-core = "0.2.3"
+simular-core = "0.2.4"
 
 
 # using this to allow cargo test on rust code. See:
 # https://github.com/PyO3/pyo3/issues/340#issuecomment-461514532
 [features]
 extension-module = ["pyo3/extension-module"]
 default = ["extension-module"]
```

### Comparing `simular_evm-0.2.2/.github/workflows/build-release.yml` & `simular_evm-0.2.3/.github/workflows/build-release.yml`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.2/.github/workflows/mdbook.yml` & `simular_evm-0.2.3/.github/workflows/mdbook.yml`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.2/.github/workflows/test_pypi.yml` & `simular_evm-0.2.3/.github/workflows/test_pypi.yml`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.2/.gitignore` & `simular_evm-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.2/.readthedocs.yaml` & `simular_evm-0.2.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.2/LICENSE` & `simular_evm-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.2/README.md` & `simular_evm-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.2/bench/simple.py` & `simular_evm-0.2.3/bench/simple.py`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.2/docs/conf.py` & `simular_evm-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.2/docs/index.rst` & `simular_evm-0.2.3/docs/index.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 .. _index:
 
 simular
 =======
 
-**Simular** is a Python API you can use to deploy and interact with Ethereum 
-smart contracts and an embedded Ethereum Virtual Machine (EVM). It creates a 
-Python wrapper around production grade Rust based Ethereum APIs making it very fast.
-
+**Simular** is a Python API wrapped around a production grade Ethereum Virtual Machine (EVM).  You can use to 
+locally deploy and interact with smart contracts, create accounts, transfer Ether, and much more.
 
 How is it different than Brownie, Ganache, Anvil?
 
-- It's only an EVM. It doesn't include blocks and mining
+- It's only an EVM.
 - No HTTP/JSON-RPC. You talk directly to the EVM (and it's fast)
 - Full functionality: account transfers, contract interaction, and more.
 
-The primary motivation for this work is to be able to model smart contract 
-interaction in an Agent Based Modeling environment 
-like `Mesa <https://mesa.readthedocs.io/en/main/>`_.
+The primary motivation for this work is to have a lightweight, fast environment for simulating and modeling Ethereum applications.
 
 Features
 --------
 
-- Run a local version with an in-memory database. Or fork db state from a remote node.
-- Parse compiled Solidity json files or define a specific set of functions using `human-readable` notation
-- Dump the current state of the EVM to json for future use in pre-populating EVM storage
 - User-friendy Python API
+- Run a local version with an in-memory database. Or copy (fork) state from a remote node.
+- Parse Solidity ABI json files or define a specific set of functions using `human-readable` notation.
+- Dump the current state of the EVM to json for future use in pre-populating EVM storage.
 
 
 Standing on the shoulders of giants...
 --------------------------------------
 
 Thanks to the following projects for making this work possible!
```

### Comparing `simular_evm-0.2.2/docs/make.bat` & `simular_evm-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.2/simular/contract.py` & `simular_evm-0.2.3/simular/contract.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,23 +5,32 @@
 from eth_utils import is_address
 import typing
 
 from .simular import PyEvm, PyAbi
 
 
 def convert_for_soltypes(args: typing.Tuple):
+    """
+    This converts `args` into a string for processing on the Rust side
+    """
+    if not isinstance(args, tuple):
+        raise Exception("Expected tuple as arguments")
+
+    def clean(v):
+        return str(v).replace("'", "").replace("True", "true").replace("False", "false")
+
     if len(args) == 1:
-        i = str(args[0]).replace("'", "")
-        return f"({i})"
-    return str(args).replace("'", "")
+        return f"({clean(args[0])})"
+    return clean(args)
 
 
 class Function:
     """
-    Contains information needed to interact with a contract function
+    Contains information needed to interact with a contract function. This
+    is attached automatically to the Contract based on the ABI.
     """
 
     def __init__(self, evm: PyEvm, abi: PyAbi, contract_address: str, name: str):
         self.name = name
         self.evm = evm
         self.abi = abi
         self.contract_address = contract_address
@@ -85,28 +94,28 @@
             return result[0]
         return result
 
 
 class Contract:
     def __init__(self, evm: PyEvm, abi: PyAbi):
         """
-        Instantiate a contract from an ABI.
+        Instantiate a contract from an ABI with an EVM.
 
         Maps contract functions to this class.  Making function available
         as attributes on the Contract.
 
         See `utils.py` for helper functions to create a Contract
         """
         self.address = None
         self.evm = evm
         self.abi = abi
 
     def __getattr__(self, name: str) -> Function:
         """
-        Make solidity contract methods available as method calls. For a given function name,
+        Make solidity contract methods available as method calls. For a given function `name`,
         return `Function`.
 
         For example, if the ABI has the contract function 'function hello(uint256)',
         you can invoke it by name: contract.hello.transact(10)
         """
         if self.abi.has_function(name):
             return Function(self.evm, self.abi, self.address, name)
@@ -131,16 +140,16 @@
         """
         self.address = address
         return self
 
     def deploy(self, *args, caller: str = None, value: int = 0) -> str:
         """
         Deploy the contract, returning it's deployed address
-        - `caller`: the address of the requester...`msg.sender`
         - `args`: a list of args (if any)
+        - `caller`: the address of the requester...`msg.sender`
         - `value`: optional amount of Ether for the contract
         Returns the address of the deployed contract
         """
         if not caller:
             raise Exception("Missing required 'caller' address")
 
         if not is_address(caller):
```

### Comparing `simular_evm-0.2.2/simular/utils.py` & `simular_evm-0.2.3/simular/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     return Contract(evm, abi)
 
 
 def contract_from_abi_bytecode(
     evm: PyEvm, raw_abi: str, bytecode: bytes = None
 ) -> Contract:
     """
-    Create a contract given the abi and bytecode.
+    Create a contract given the abi and/or bytecode.
 
     - `evm`     : PyEvm  the EVM client
     - `raw_abi` : abi file as un-parsed json
     - `bytecode`: Optional bytes
     Returns an instance of Contract
     """
     if not isinstance(evm, PyEvm):
```

### Comparing `simular_evm-0.2.2/src/lib.rs` & `simular_evm-0.2.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.2/src/pyabi.rs` & `simular_evm-0.2.3/src/pyabi.rs`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.2/src/pyevm.rs` & `simular_evm-0.2.3/src/pyevm.rs`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 use anyhow::{anyhow, Result};
 use core::ffi::c_uchar;
 use pyo3::{ffi, prelude::*};
 use simular_core::{BaseEvm, CreateFork, SnapShot};
 
 use crate::{pyabi::PyAbi, str_to_address};
 
+/// default block interval for advancing block time (12s)
+const DEFAULT_BLOCK_INTERVAL: u64 = 12;
+
 #[pyclass]
 pub struct PyEvm(BaseEvm);
 
 #[pymethods]
 impl PyEvm {
     /// Create an in-memory EVM
     #[new]
@@ -131,14 +134,24 @@
 
         let (calldata, _is_payable, decoder) = abi.encode_function(fn_name, args)?;
         let output = self.0.simulate(caller_address, to_address, calldata, v)?;
         let dynvalues = decoder.0.abi_decode_params(&output.result)?;
         let dsm = DynSolMap(dynvalues.clone());
         Ok(dsm.into_py(py))
     }
+
+    /// Advance block.number and block.timestamp. Set interval to the amount of
+    /// time in seconds you want to advance the timestamp (default: 12s). Block
+    /// number will automatically increment.
+    ///
+    /// When using a fork the initial block.number/timestamp will come from the snapshot.
+    pub fn advance_block(&mut self, interval: Option<u64>) {
+        let it = interval.unwrap_or(DEFAULT_BLOCK_INTERVAL);
+        self.0.update_block(it);
+    }
 }
 
 // *** Helpers to convert DynSolValues to PyObject *** //
 
 fn walk_list(values: Vec<DynSolValue>, py: Python<'_>) -> PyObject {
     values
         .into_iter()
```

### Comparing `simular_evm-0.2.2/tests/conftest.py` & `simular_evm-0.2.3/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,7 +37,14 @@
 
 
 @pytest.fixture
 def kitchen_sink_json():
     with open(f"{PATH}/./fixtures/KitchenSink.json") as f:
         rawabi = f.read()
     return rawabi
+
+
+@pytest.fixture
+def block_meta_json():
+    with open(f"{PATH}/./fixtures/BlockMeta.json") as f:
+        rawabi = f.read()
+    return rawabi
```

### Comparing `simular_evm-0.2.2/tests/fixtures/contracts/KitchenSink.sol` & `simular_evm-0.2.3/tests/fixtures/contracts/KitchenSink.sol`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.2/tests/fixtures/contracts/MockERC20.sol` & `simular_evm-0.2.3/tests/fixtures/contracts/MockERC20.sol`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.2/tests/fixtures/erc20.abi` & `simular_evm-0.2.3/tests/fixtures/erc20.abi`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.2/tests/fixtures/erc20.bin` & `simular_evm-0.2.3/tests/fixtures/erc20.bin`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.2/tests/test_contract.py` & `simular_evm-0.2.3/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `simular_evm-0.2.2/tests/test_pyevm.py` & `simular_evm-0.2.3/tests/test_pyevm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 from eth_utils import to_wei
 from eth_abi import decode
 
-from simular import PyEvm, PyAbi
+from simular import PyEvm, PyAbi, contract_from_raw_abi
 
 
 def test_create_account_and_balance(evm, bob):
     two_ether = to_wei(2, "ether")
 
     assert evm.get_balance(bob) == 0
     evm.create_account(bob, two_ether)
@@ -50,7 +50,28 @@
     with pytest.raises(BaseException):
         evm.transact(bob, "Ox01", enc, 0)
 
     evm.transact("increment", "()", bob, contract_address, 0, abi)
 
     (enc1, _, _) = abi.encode_function("value", "()")
     assert [1] == evm.call("value", "()", contract_address, abi)
+
+
+def test_advance_block(evm, bob, block_meta_json):
+    # simple contract that can return block.timestamp and number
+    evm.create_account(bob)
+
+    contract = contract_from_raw_abi(evm, block_meta_json)
+    contract.deploy(caller=bob)
+
+    ts1, bn1 = contract.getMeta.call()
+
+    assert bn1 == 1  # start at block 1
+
+    evm.advance_block()
+    evm.advance_block()
+    evm.advance_block()
+
+    ts2, bn2 = contract.getMeta.call()
+
+    assert bn2 == 4  # block advanced
+    assert ts2 == ts1 + 36  # timestamp advanced
```

### Comparing `simular_evm-0.2.2/Cargo.lock` & `simular_evm-0.2.3/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -36,52 +36,52 @@
 checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "allocator-api2"
-version = "0.2.16"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0942ffc6dcaadf03badf6e6a2d0228460359d5e34b57ccdc720b7382dfbd5ec5"
+checksum = "5c6cb57a04249c6480766f7f7cef5467412af1490f8d1e243141daddada3264f"
 
 [[package]]
 name = "alloy-dyn-abi"
-version = "0.7.0"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "872f239c15befa27cc4f0d3d82a70b3365c2d0202562bf906eb93b299fa31882"
+checksum = "8425a283510106b1a6ad25dd4bb648ecde7da3fd2baeb9400a85ad62f51ec90b"
 dependencies = [
  "alloy-json-abi",
  "alloy-primitives",
  "alloy-sol-type-parser",
  "alloy-sol-types",
  "const-hex",
  "itoa",
  "serde",
  "serde_json",
- "winnow 0.6.5",
+ "winnow 0.6.8",
 ]
 
 [[package]]
 name = "alloy-json-abi"
-version = "0.7.0"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "83a35ddfd27576474322a5869e4c123e5f3e7b2177297c18e4e82ea501cb125b"
+checksum = "7e30946aa6173020259055a44971f5cf40a7d76c931d209caeb51b333263df4f"
 dependencies = [
  "alloy-primitives",
  "alloy-sol-type-parser",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "alloy-primitives"
-version = "0.7.0"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99bbad0a6b588ef4aec1b5ddbbfdacd9ef04e00b979617765b03174318ee1f3a"
+checksum = "db8aa973e647ec336810a9356af8aea787249c9d00b1525359f3db29a68d231b"
 dependencies = [
  "alloy-rlp",
  "arbitrary",
  "bytes",
  "cfg-if",
  "const-hex",
  "derive_arbitrary",
@@ -97,85 +97,99 @@
  "ruint",
  "serde",
  "tiny-keccak",
 ]
 
 [[package]]
 name = "alloy-rlp"
-version = "0.3.4"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8d58d9f5da7b40e9bfff0b7e7816700be4019db97d4b6359fe7f94a9e22e42ac"
+checksum = "b155716bab55763c95ba212806cf43d05bcc70e5f35b02bad20cf5ec7fe11fed"
 dependencies = [
  "arrayvec",
  "bytes",
 ]
 
 [[package]]
 name = "alloy-sol-macro"
-version = "0.7.0"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "452d929748ac948a10481fff4123affead32c553cf362841c5103dd508bdfc16"
+checksum = "7dbd17d67f3e89478c8a634416358e539e577899666c927bc3d2b1328ee9b6ca"
+dependencies = [
+ "alloy-sol-macro-expander",
+ "alloy-sol-macro-input",
+ "proc-macro-error",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.66",
+]
+
+[[package]]
+name = "alloy-sol-macro-expander"
+version = "0.7.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c6da95adcf4760bb4b108fefa51d50096c5e5fdd29ee72fed3e86ee414f2e34"
 dependencies = [
  "alloy-json-abi",
  "alloy-sol-macro-input",
  "const-hex",
  "heck 0.4.1",
  "indexmap",
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.66",
  "syn-solidity",
  "tiny-keccak",
 ]
 
 [[package]]
 name = "alloy-sol-macro-input"
-version = "0.7.0"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "df64e094f6d2099339f9e82b5b38440b159757b6920878f28316243f8166c8d1"
+checksum = "32c8da04c1343871fb6ce5a489218f9c85323c8340a36e9106b5fc98d4dd59d5"
 dependencies = [
  "alloy-json-abi",
  "const-hex",
  "dunce",
  "heck 0.5.0",
  "proc-macro2",
  "quote",
  "serde_json",
- "syn 2.0.58",
+ "syn 2.0.66",
  "syn-solidity",
 ]
 
 [[package]]
 name = "alloy-sol-type-parser"
-version = "0.7.0"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "715f4d09a330cc181fc7c361b5c5c2766408fa59a0bac60349dcb7baabd404cc"
+checksum = "368cae4dc052cad1d8f72eb2ae0c38027116933eeb49213c200a9e9875f208d7"
 dependencies = [
- "winnow 0.6.5",
+ "winnow 0.6.8",
 ]
 
 [[package]]
 name = "alloy-sol-types"
-version = "0.7.0"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43bc2d6dfc2a19fd56644494479510f98b1ee929e04cf0d4aa45e98baa3e545b"
+checksum = "40a64d2d2395c1ac636b62419a7b17ec39031d6b2367e66e9acbf566e6055e9c"
 dependencies = [
  "alloy-json-abi",
  "alloy-primitives",
  "alloy-sol-macro",
  "const-hex",
  "serde",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.81"
+version = "1.0.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0952808a6c2afd1aa8947271f3a60f1a6763c7b912d210184c5149b5cf147247"
+checksum = "b3d1d046238990b9cf5bcde22a3fb3584ee5cf65fb2765f454ed428c7a0063da"
 
 [[package]]
 name = "arbitrary"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7d5a26814d8dcb93b0e5a0ff3c6d80a8843bafb21b39e8e18a6f05471870e110"
 
@@ -307,21 +321,21 @@
 name = "arrayvec"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
 
 [[package]]
 name = "async-trait"
-version = "0.1.79"
+version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507401cad91ec6a857ed5513a2073c82a9b9048762b885bb98655b306964681"
+checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "async_io_stream"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6d7b9decdf35d8908a7e3ef02f64c5e9b1695e230154c0e8de3969142d9b94c"
@@ -329,38 +343,38 @@
  "futures",
  "pharos",
  "rustc_version 0.4.0",
 ]
 
 [[package]]
 name = "aurora-engine-modexp"
-version = "1.0.0"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfacad86e9e138fca0670949eb8ed4ffdf73a55bded8887efe0863cd1a3a6f70"
+checksum = "0aef7712851e524f35fbbb74fa6599c5cd8692056a1c36f9ca0d2001b670e7e5"
 dependencies = [
  "hex",
  "num",
 ]
 
 [[package]]
 name = "auto_impl"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c87f3f15e7794432337fc718554eaa4dc8f04c9677a950ffe366f20a162ae42"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "backtrace"
 version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
@@ -446,17 +460,17 @@
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.15.4"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "byte-slice-cast"
 version = "1.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c3ac9f8b63eca6fd385229b3675f6cc0dc5c8a5c8a54a59d4f52ffd670d87b0c"
 
@@ -473,38 +487,38 @@
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.90"
+version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
+checksum = "41c270e7540d725e65ac7f1b212ac8ce349719624d7bcff99f8e2e488e8cf03f"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.37"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "const-hex"
-version = "1.11.3"
+version = "1.11.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ba00838774b4ab0233e355d26710fbfc8327a05c017f6dc4873f876d1f79f78"
+checksum = "70ff96486ccc291d36a958107caf2c0af8c78c0af7d31ae2f35ce055130de1a6"
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "hex",
  "proptest",
  "serde",
 ]
@@ -572,17 +586,17 @@
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
 name = "data-encoding"
-version = "2.5.0"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e962a19be5cfc3f3bf6dd8f61eb50107f356ad6270fbb3ed41476571db78be5"
+checksum = "e8566979429cf69b49a5c740c60791108e86440e8be149bbea4fe54d2c32d6e2"
 
 [[package]]
 name = "der"
 version = "0.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f55bf8e7b65898637379c1b74eb1551107c8294ed26d855ceb9fd1a09cfc9bc0"
 dependencies = [
@@ -614,15 +628,15 @@
 name = "derive_arbitrary"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "67e77553c4162a157adbf834ebae5b415acbecbeafc7a74b0e886657506a7611"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "derive_more"
 version = "0.99.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fb810d30a7c1953f91334de7244731fc3f3c10d7fe163338a35b9f640960321"
@@ -679,17 +693,17 @@
  "rfc6979",
  "signature",
  "spki",
 ]
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "3dca9240753cf90908d7e4aac30f630662b02aebaa1b58a3cadabdb23385b58b"
 
 [[package]]
 name = "elliptic-curve"
 version = "0.13.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b5e6043086bf7973472e0c7dff2142ea0b680d30e18d9cc40f267efbf222bd47"
 dependencies = [
@@ -704,17 +718,17 @@
  "sec1",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "encoding_rs"
-version = "0.8.33"
+version = "0.8.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7268b386296a025e474d5140678f75d6de9493ae55a5d709eeb9dd08149945e1"
+checksum = "b45de904aa0b010bce2ab45264d0631681847fa7b6f2eaa7dab7619943bc4f59"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "enr"
 version = "0.10.0"
@@ -737,28 +751,28 @@
 name = "enumn"
 version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6fd000fd6988e73bbe993ea3db9b1aa64906ab88766d654973924340c8cddb42"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "errno"
-version = "0.3.8"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
+checksum = "534c5cf6194dfab3db3242765c03bbe257cf92f22b38f6bc0c58d59108a820ba"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "ethabi"
@@ -882,17 +896,17 @@
  "wasm-bindgen-futures",
  "web-sys",
  "ws_stream_wasm",
 ]
 
 [[package]]
 name = "fastrand"
-version = "2.0.2"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "658bd65b1cf4c852a3cc96f18a8ce7b5640f6b703f905c7d74532294c2a63984"
+checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
 
 [[package]]
 name = "fastrlp"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "139834ddba373bbdd213dffe02c8d110508dcf1726c2be27e8d1f7d7e1856418"
 dependencies = [
@@ -1012,15 +1026,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -1077,17 +1091,17 @@
  "typenum",
  "version_check",
  "zeroize",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -1136,17 +1150,17 @@
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 dependencies = [
  "ahash",
  "allocator-api2",
 ]
 
 [[package]]
 name = "hashers"
@@ -1346,17 +1360,17 @@
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "instant"
-version = "0.1.12"
+version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
+checksum = "e0242819d153cba4b4b05a5a8f2a7e9bbf97b6055b2a002b395c96b5ff3c0222"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "inventory"
 version = "0.3.15"
@@ -1428,17 +1442,17 @@
 checksum = "ecc2af9a1119c51f12a14607e783cb977bde58bc069ff0c3da1095e635d70654"
 dependencies = [
  "cpufeatures",
 ]
 
 [[package]]
 name = "keccak-asm"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb8515fff80ed850aea4a1595f2e519c003e2a00a82fe168ebf5269196caf444"
+checksum = "47a3633291834c4fbebf8673acbc1b04ec9d151418ff9b8e26dcd79129928758"
 dependencies = [
  "digest 0.10.7",
  "sha3-asm",
 ]
 
 [[package]]
 name = "lazy_static"
@@ -1447,35 +1461,35 @@
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 dependencies = [
  "spin 0.5.2",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.4.13"
+version = "0.4.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
+checksum = "78b3ae25bc7c8c38cec158d1f2757ee79e9b3740fbc7ccf0e59e4b08d793fa89"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
@@ -1502,17 +1516,17 @@
 name = "mime"
 version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.2"
+version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
+checksum = "87dfd01fe195c66b572b37921ad8803d010623c0aca821bea2302239d155cdae"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
 version = "0.8.11"
@@ -1540,42 +1554,41 @@
  "security-framework",
  "security-framework-sys",
  "tempfile",
 ]
 
 [[package]]
 name = "num"
-version = "0.4.1"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b05180d69e3da0e530ba2a1dae5110317e49e3b7f3d41be227dc5f92e49ee7af"
+checksum = "35bd024e8b2ff75562e5f34e7f4905839deb4b22955ef5e73d2fea1b9813cb23"
 dependencies = [
  "num-bigint",
  "num-complex",
  "num-integer",
  "num-iter",
  "num-rational",
  "num-traits",
 ]
 
 [[package]]
 name = "num-bigint"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "608e7659b5c3d7cba262d894801b9ec9d00de989e8a82bd4bef91d08da45cdc0"
+checksum = "c165a9ab64cf766f73521c0dd2cfdff64f488b8f0b3e621face3462d3db536d7"
 dependencies = [
- "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
+checksum = "73f88a1307638156682bada9d7604135552957b7818057dcef22705b4d509495"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-conv"
 version = "0.1.0"
@@ -1589,40 +1602,39 @@
 checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-iter"
-version = "0.1.44"
+version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d869c01cc0c455284163fd0092f1f93835385ccab5a98a0dcc497b2f8bf055a9"
+checksum = "1429034a0490724d0075ebb2bc9e875d6503c3cf69e235a8941aa757d83ef5bf"
 dependencies = [
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-rational"
-version = "0.4.1"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0638a1c9d0a3c0914158145bc76cff373a75a627e6ecbfb71cbe6f453a5a19b0"
+checksum = "f83d14da390562dca69fc84082e73e548e1ad308d24accdedd2720017cb37824"
 dependencies = [
- "autocfg",
  "num-bigint",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
@@ -1645,18 +1657,18 @@
 
 [[package]]
 name = "num_enum_derive"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "681030a937600a36906c185595136d26abfebb4aa9c65701cefcaf8578bb982b"
 dependencies = [
- "proc-macro-crate 3.1.0",
+ "proc-macro-crate",
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "object"
 version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
@@ -1714,28 +1726,28 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-src"
-version = "300.2.3+3.2.1"
+version = "300.3.0+3.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5cff92b6f71555b61bb9315f7c64da3ca43d87531622120fea0195fc761b4843"
+checksum = "eba8804a1c5765b18c4b3f907e6897ebabeedebc9830e1a0046c4a4cf44663e1"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "openssl-sys"
 version = "0.9.102"
@@ -1747,66 +1759,66 @@
  "openssl-src",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
 name = "parity-scale-codec"
-version = "3.6.9"
+version = "3.6.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "881331e34fa842a2fb61cc2db9643a8fedc615e47cfcc52597d1af0db9a7e8fe"
+checksum = "306800abfa29c7f16596b5970a588435e3d5b3149683d00c12b699cc19f895ee"
 dependencies = [
  "arrayvec",
  "bitvec",
  "byte-slice-cast",
  "impl-trait-for-tuples",
  "parity-scale-codec-derive",
  "serde",
 ]
 
 [[package]]
 name = "parity-scale-codec-derive"
-version = "3.6.9"
+version = "3.6.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be30eaf4b0a9fba5336683b38de57bb86d179a35862ba6bfcf57625d006bde5b"
+checksum = "d830939c76d294956402033aee57a6da7b438f2294eb94864c37b0569053a42c"
 dependencies = [
- "proc-macro-crate 2.0.0",
+ "proc-macro-crate",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "f1bf18183cf54e8d6059647fc3063646a1801cf30896933ec2311622cc4b9a27"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.14"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
+checksum = "57c0d7b74b563b49d38dae00a0c37d4d6de9b432382b2892f0574ddcae73fd0a"
 
 [[package]]
 name = "pem"
 version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a8835c273a76a90455d7344889b0964598e3316e2a79ede8e36f16bdcf2228b8"
 dependencies = [
@@ -1817,17 +1829,17 @@
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "pest"
-version = "2.7.9"
+version = "2.7.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "311fb059dee1a7b802f036316d790138c613a4e8b180c822e3925a662e9f0c95"
+checksum = "560131c633294438da9f7c4b08189194b20946c8274c6b9e38881a7874dc8ee8"
 dependencies = [
  "memchr",
  "thiserror",
  "ucd-trie",
 ]
 
 [[package]]
@@ -1853,15 +1865,15 @@
 name = "pin-project-internal"
 version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
@@ -1918,38 +1930,19 @@
  "impl-serde",
  "scale-info",
  "uint",
 ]
 
 [[package]]
 name = "proc-macro-crate"
-version = "1.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f4c021e1093a56626774e81216a4ce732a735e5bad4868a03f3ed65ca0c3919"
-dependencies = [
- "once_cell",
- "toml_edit 0.19.15",
-]
-
-[[package]]
-name = "proc-macro-crate"
-version = "2.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e8366a6159044a37876a2b9817124296703c586a5c92e2c53751fa06d8d43e8"
-dependencies = [
- "toml_edit 0.20.7",
-]
-
-[[package]]
-name = "proc-macro-crate"
 version = "3.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d37c51ca738a55da99dc0c4a34860fd675453b8b36209178c2249bb13651284"
 dependencies = [
- "toml_edit 0.21.1",
+ "toml_edit",
 ]
 
 [[package]]
 name = "proc-macro-error"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
@@ -1970,17 +1963,17 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "ec96c6a92621310b51366f1e28d05ef11489516e93be030060e5fc12024a49d6"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "proptest"
 version = "1.4.0"
@@ -2057,41 +2050,41 @@
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck 0.4.1",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "quick-error"
 version = "1.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a1d01941d82fa2ab50be1e79e6714289dd7cde78eba4c074bc5a4374f650dfe0"
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "radium"
 version = "0.7.0"
@@ -2135,19 +2128,19 @@
 checksum = "d25bf25ec5ae4a3f1b92f929810509a2f53d7dca2f50b794ff57e3face536c8f"
 dependencies = [
  "rand_core",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "regex"
 version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
@@ -2376,17 +2369,17 @@
 name = "ruint-macro"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f86854cf50259291520509879a5c294c3c9a4c334e9ff65071c51e42ef1e2343"
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+checksum = "719b953e2095829ee67db738b3bfa9fa368c94900df327b3f07fe6e794d2fe1f"
 
 [[package]]
 name = "rustc-hex"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3e75f6a532d0fd9f7f13144f392b6ad56a32696bfcd9c78f797f16bbb6f072d6"
 
@@ -2401,35 +2394,35 @@
 
 [[package]]
 name = "rustc_version"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
- "semver 1.0.22",
+ "semver 1.0.23",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.32"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
  "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.21.10"
+version = "0.21.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9d5a6813c0759e4609cd494e8e725babae6a2ca7b62a5536a13daaec6fcb7ba"
+checksum = "3f56a14d1f48b391359b22f731fd4bd7e43c97f3c50eee276f3aa09c94784d3e"
 dependencies = [
  "log",
  "ring 0.17.8",
  "rustls-webpki",
  "sct",
 ]
 
@@ -2450,17 +2443,17 @@
 dependencies = [
  "ring 0.17.8",
  "untrusted 0.9.0",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.14"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
+checksum = "955d28af4278de8121b7ebeb796b6a45735dc01436d898801014aced2773a3d6"
 
 [[package]]
 name = "rusty-fork"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cb3dcc6e454c328bb824492db107ab7c0ae8fcffe4ad210136ef014458c1bc4f"
 dependencies = [
@@ -2468,37 +2461,37 @@
  "quick-error",
  "tempfile",
  "wait-timeout",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
+checksum = "f3cb5ba0dc43242ce17de99c180e96db90b235b8a9fdc9543c96d2209116bd9f"
 
 [[package]]
 name = "scale-info"
-version = "2.11.1"
+version = "2.11.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "788745a868b0e751750388f4e6546eb921ef714a4317fa6954f7cde114eb2eb7"
+checksum = "eca070c12893629e2cc820a9761bedf6ce1dcddc9852984d1dc734b8bd9bd024"
 dependencies = [
  "cfg-if",
  "derive_more",
  "parity-scale-codec",
  "scale-info-derive",
 ]
 
 [[package]]
 name = "scale-info-derive"
-version = "2.11.1"
+version = "2.11.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dc2f4e8bc344b9fc3d5f74f72c2e55bfc38d28dc2ebc69c194a3df424e4d9ac"
+checksum = "2d35494501194174bda522a32605929eefc9ecf7e0a326c26db1fdd85881eb62"
 dependencies = [
- "proc-macro-crate 1.3.1",
+ "proc-macro-crate",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "schannel"
@@ -2537,30 +2530,30 @@
  "pkcs8",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "security-framework"
-version = "2.10.0"
+version = "2.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "770452e37cad93e0a50d5abc3990d2bc351c36d0328f86cefec2f2fb206eaef6"
+checksum = "c627723fd09706bacdb5cf41499e95098555af3c3c29d014dc3c458ef6be11c0"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.5.0",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
 name = "security-framework-sys"
-version = "2.10.0"
+version = "2.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41f3cc463c0ef97e11c3461a9d3787412d30e8e7eb907c79180c4a57bf7c04ef"
+checksum = "317936bbbd05227752583946b9e66d7ce3b489f84e11a94a510b4437fef407d7"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "semver"
@@ -2569,17 +2562,17 @@
 checksum = "f301af10236f6df4160f7c3f04eec6dbc70ace82d23326abad5edee88801c6b6"
 dependencies = [
  "semver-parser",
 ]
 
 [[package]]
 name = "semver"
-version = "1.0.22"
+version = "1.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
+checksum = "61697e0a1c7e512e84a621326239844a24d8207b4669b41bc18b32ea5cbf988b"
 
 [[package]]
 name = "semver-parser"
 version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "00b0bef5b7f9e0df16536d3961cfb6e84331c065b4066afb39768d0e319411f7"
 dependencies = [
@@ -2596,37 +2589,37 @@
 name = "send_wrapper"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cd0b0ec5f1c1ca621c432a25813d8d60c88abe6d3e08a3eb9cf37d97a0fe3d73"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "7253ab4de971e72fb7be983802300c30b5a7f0c2e56fab8abfc6a214307c0094"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "500cbc0ebeb6f46627f50f3f5811ccf6bf00643be300b4c3eabc0ef55dc5b5ba"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.115"
+version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -2671,17 +2664,17 @@
 dependencies = [
  "digest 0.10.7",
  "keccak",
 ]
 
 [[package]]
 name = "sha3-asm"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bac61da6b35ad76b195eb4771210f947734321a8d81d7738e1580d953bc7a15e"
+checksum = "a9b57fd861253bff08bb1919e995f90ba8f4889de2726091c8876f3a4e823b40"
 dependencies = [
  "cc",
  "cfg-if",
 ]
 
 [[package]]
 name = "signature"
@@ -2703,31 +2696,31 @@
  "num-traits",
  "thiserror",
  "time",
 ]
 
 [[package]]
 name = "simular"
-version = "0.2.2"
+version = "0.2.3"
 dependencies = [
  "alloy-dyn-abi",
  "alloy-primitives",
  "anyhow",
  "hex",
  "pyo3",
  "serde",
  "serde_json",
  "simular-core",
 ]
 
 [[package]]
 name = "simular-core"
-version = "0.2.3"
+version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0bd839cfebd76e663b021d026a55cf201bf61579f4cc3ce79b6aa87b1a853f5"
+checksum = "7de90fd13a45e6e0609f663d1339b4837c0352dfc227a6b19214798d280a106d"
 dependencies = [
  "alloy-dyn-abi",
  "alloy-json-abi",
  "alloy-primitives",
  "alloy-sol-types",
  "anyhow",
  "ethers-core",
@@ -2755,17 +2748,17 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "socket2"
-version = "0.5.6"
+version = "0.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
+checksum = "ce305eb0b4296696835b71df73eb912e0f1ffd2556a501fcede6e0c50349191c"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "spin"
@@ -2810,15 +2803,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6cf59daf282c0a494ba14fd21610a0325f9f90ec9d1231dea26bcb1d696c946"
 dependencies = [
  "heck 0.4.1",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.58",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "substrate-bn"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b5bbfa79abbae15dd642ea8176a21a635ff3c00059961d1ea27ad04e5b441c"
@@ -2845,33 +2838,33 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.58"
+version = "2.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
+checksum = "c42f3f41a2de00b01c0aaad383c5a45241efc8b2d1eda5661812fda5f3cdcff5"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn-solidity"
-version = "0.7.0"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4497156948bd342b52038035a6fa514a89626e37af9d2c52a5e8d8ebcc7ee479"
+checksum = "b8db114c44cf843a8bacd37a146e37987a0b823a0e8bc4fdc610c9c72ab397a5"
 dependencies = [
  "paste",
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "sync_wrapper"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2047c6ded9c721764247e62cd3b03c09ffc529b2ba5b10ec482ae507a4a70160"
@@ -2919,37 +2912,37 @@
  "fastrand",
  "rustix",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "c546c80d6be4bc6a00c0f01730c08df82eaa7a7a61f11d656526506112cc1709"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "46c3384250002a6d5af4d114f2845d37b57521033f30d5c3f46c4d70e1197533"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.34"
+version = "0.3.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8248b6521bb14bc45b4067159b9b6ad792e2d6d754d6c41fb50e29fefe38749"
+checksum = "5dfd88e563464686c916c7e46e623e520ddc6d79fa6641390f2e3fa86e83e885"
 dependencies = [
  "deranged",
  "itoa",
  "num-conv",
  "powerfmt",
  "serde",
  "time-core",
@@ -2960,17 +2953,17 @@
 name = "time-core"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef927ca75afb808a4d64dd374f00a2adf8d0fcff8e7b184af886c3c87ec4a3f3"
 
 [[package]]
 name = "time-macros"
-version = "0.2.17"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ba3a3ef41e6672a2f0f001392bb5dcd3ff0a9992d618ca761a11c3121547774"
+checksum = "3f252a68540fde3a3877aeea552b832b40ab9a69e318efd078774a01ddee1ccf"
 dependencies = [
  "num-conv",
  "time-core",
 ]
 
 [[package]]
 name = "tiny-keccak"
@@ -3017,15 +3010,15 @@
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
@@ -3057,53 +3050,30 @@
  "tokio-rustls",
  "tungstenite",
  "webpki-roots",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.10"
+version = "0.7.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5419f34732d9eb6ee4c3578b7989078579b7f039cbbb9ca2c4da015749371e15"
+checksum = "9cf6b47b3771c49ac75ad09a6162f53ad4b8088b76ac60e8ec1455b31a189fe1"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
- "tracing",
 ]
 
 [[package]]
 name = "toml_datetime"
-version = "0.6.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
-
-[[package]]
-name = "toml_edit"
-version = "0.19.15"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b5bb770da30e5cbfde35a2d7b9b8a2c4b8ef89548a7a6aeab5c9a576e3e7421"
-dependencies = [
- "indexmap",
- "toml_datetime",
- "winnow 0.5.40",
-]
-
-[[package]]
-name = "toml_edit"
-version = "0.20.7"
+version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "70f427fce4d84c72b5b732388bf4a9f4531b53f74e2887e3ecb2481f68f66d81"
-dependencies = [
- "indexmap",
- "toml_datetime",
- "winnow 0.5.40",
-]
+checksum = "4badfd56924ae69bcc9039335b2e017639ce3f9b001c393c1b2d1ef846ce2cbf"
 
 [[package]]
 name = "toml_edit"
 version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a8534fd7f78b5405e860340ad6575217ce99f38d4d5c8f2442cb5ecb50090e1"
 dependencies = [
@@ -3133,15 +3103,15 @@
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
@@ -3337,15 +3307,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.66",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -3371,15 +3341,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.66",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -3435,15 +3405,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -3455,125 +3425,132 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winnow"
 version = "0.5.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f593a95398737aeed53e489c785df13f3618e41dbcd6718c6addbf1395aa6876"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winnow"
-version = "0.6.5"
+version = "0.6.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dffa400e67ed5a4dd237983829e66475f0a4a26938c4b04c21baede6262215b8"
+checksum = "c3c52e9c97a68071b23e836c9380edae937f17b9c4667bd021973efc689f618d"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winreg"
 version = "0.50.0"
@@ -3610,44 +3587,44 @@
 checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
 dependencies = [
  "tap",
 ]
 
 [[package]]
 name = "zerocopy"
-version = "0.7.32"
+version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74d4d3961e53fa4c9a25a8637fc2bfaf2595b3d3ae34875568a5cf64787716be"
+checksum = "ae87e3fcd617500e5d106f0380cf7b77f3c6092aae37191433159dda23cfb087"
 dependencies = [
  "zerocopy-derive",
 ]
 
 [[package]]
 name = "zerocopy-derive"
-version = "0.7.32"
+version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
+checksum = "15e934569e47891f7d9411f1a451d947a60e000ab3bd24fbb970f000387d1b3b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "zeroize"
-version = "1.7.0"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
+checksum = "ced3678a2879b30306d323f4542626697a464a97c0a07c9aebf7ebca65cd4dde"
 dependencies = [
  "zeroize_derive",
 ]
 
 [[package]]
 name = "zeroize_derive"
 version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ce36e65b0d2999d2aafac989fb249189a141aee1f53c612c1f37d72631959f69"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.66",
 ]
```

### Comparing `simular_evm-0.2.2/pyproject.toml` & `simular_evm-0.2.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 [tool.maturin]
 features = ["pyo3/extension-module"]
 sdist-include = ["LICENSE", "README.md"]
 
 
 [project]
 name = "simular-evm"
-version = "0.2.2"
+version = "0.2.3"
 requires-python = ">=3.11"
 authors = [
     { name = "Dave Bryson", email = "davebryson@users.noreply.github.com" },
 ]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/simular-fi/simular"
 repository = "https://github.com/simular-fi/simular"
-documentation = "https://github.com/simular-fi/simular/docs/"
+documentation = "https://simular.readthedocs.io/en/latest/"
 keywords = ["agent-based modeling", "ethereum", "solidity", "simulation"]
 description = "smart-contract api and embedded ethereum virtual machine"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
@@ -41,9 +41,9 @@
 ]
 
 [tool.hatch.envs.dev.scripts]
 docs = "sphinx-build -M html docs docs/build"
 
 [project.urls]
 Source = "https://github.com/simular-fi/simular"
-Documentation = "https://simular-fi.github.io/simular"
+Documentation = "https://simular.readthedocs.io/en/latest/"
 Issues = "https://github.com/simular-fi/simular/issues"
```

### Comparing `simular_evm-0.2.2/PKG-INFO` & `simular_evm-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: simular-evm
-Version: 0.2.2
+Version: 0.2.3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: eth-abi >=4.1.0
 Requires-Dist: eth-utils >=2.2.0
@@ -14,15 +14,15 @@
 Home-Page: https://github.com/simular-fi/simular
 Author: Dave Bryson
 Author-email: Dave Bryson <davebryson@users.noreply.github.com>
 License: Apache-2.0
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source, https://github.com/simular-fi/simular
-Project-URL: Documentation, https://simular-fi.github.io/simular
+Project-URL: Documentation, https://simular.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/simular-fi/simular/issues
 
 
 # Simular
 
 [![pypi](https://img.shields.io/pypi/v/simular-evm.svg)](https://pypi.python.org/pypi/simular-evm)
```

