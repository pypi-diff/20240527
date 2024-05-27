# Comparing `tmp/w3tools-0.1.1.tar.gz` & `tmp/w3tools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w3tools-0.1.1.tar", max compression
+gzip compressed data, was "w3tools-0.1.2.tar", max compression
```

## Comparing `w3tools-0.1.1.tar` & `w3tools-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      870 2024-05-20 12:01:09.709086 w3tools-0.1.1/README.md
--rw-r--r--   0        0        0      443 2024-05-20 12:01:09.709086 w3tools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-20 12:01:09.709086 w3tools-0.1.1/w3tools/__init__.py
--rw-r--r--   0        0        0     2836 2024-05-20 12:01:09.709086 w3tools-0.1.1/w3tools/chain.py
--rw-r--r--   0        0        0      960 2024-05-20 12:01:09.709086 w3tools-0.1.1/w3tools/rpc.py
--rw-r--r--   0        0        0     4161 2024-05-20 12:01:09.709086 w3tools-0.1.1/w3tools/w3.py
--rw-r--r--   0        0        0     1545 1970-01-01 00:00:00.000000 w3tools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-27 11:21:49.786446 w3tools-0.1.2/README.md
+-rw-r--r--   0        0        0      442 2024-05-27 11:21:49.786446 w3tools-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-27 11:21:49.786446 w3tools-0.1.2/w3tools/__init__.py
+-rw-r--r--   0        0        0     2879 2024-05-27 11:21:49.786446 w3tools-0.1.2/w3tools/chain.py
+-rw-r--r--   0        0        0     2384 2024-05-27 11:21:49.786446 w3tools-0.1.2/w3tools/rpc.py
+-rw-r--r--   0        0        0     6106 2024-05-27 11:21:49.786446 w3tools-0.1.2/w3tools/w3.py
+-rw-r--r--   0        0        0     1740 1970-01-01 00:00:00.000000 w3tools-0.1.2/PKG-INFO
```

### Comparing `w3tools-0.1.1/README.md` & `w3tools-0.1.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # w3tools: Enhanced Web3 Development Toolkit for Python
 
 w3tools is a Python library that provides a set of tools to enhance the development of Web3 applications, including:
 
 1. Web3 RPC client for popular EVM-based blockchains supporting:
    - popular RPC providers, like Infura, Alchemy, etc.
    - multiple EVM-based blockchains, like Ethereum, Binance Smart Chain, etc.
+   - Websocket and HTTP RPC
    - rate limiting and retrying
    - skip validation of RPC method parameters
    - debug mode
    - cache
    - custom RPC method
 2. Get token price from Uniswap and other DEXs
 3. Get Uniswap liquidity pool information
@@ -19,15 +20,24 @@
 ```bash
 pip install w3tools
 ```
 
 ## Usage
 
 ```python
+from w3tools.chain import ChainId
+from w3tools.w3 import make_w3
 
+w3 = make_w3(
+    ChainId.ETH,
+    "quicknode",
+    api_key="your key",
+)
+
+print(w3.eth.block_number)
 ```
 
 ## Credits
 
 - [Web3.py](https://github.com/ethereum/web3.py)
 
 ## Development
```

### Comparing `w3tools-0.1.1/w3tools/chain.py` & `w3tools-0.1.2/w3tools/chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,17 @@
     VISION = 888888
     NEON = 245022934
     AURORA = 1313161554
     HARMONY = 1666600000
     PALM = 11297108109
     CURIO = 836542336838601
 
+    # testnets
+    ETH_SEPOLIA = 11155111
+
     @classmethod
     def _missing_(cls, key):
         if isinstance(key, str):
             return ChainId[key.upper()]
 
 
 @dataclass
```

### Comparing `w3tools-0.1.1/PKG-INFO` & `w3tools-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: w3tools
-Version: 0.1.1
+Version: 0.1.2
 Summary: w3tools is a Python library that provides a set of tools to enhance the development of Web3 applications
 License: MIT
 Author: wanger
 Author-email: wangereth@icloud.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,14 +19,15 @@
 # w3tools: Enhanced Web3 Development Toolkit for Python
 
 w3tools is a Python library that provides a set of tools to enhance the development of Web3 applications, including:
 
 1. Web3 RPC client for popular EVM-based blockchains supporting:
    - popular RPC providers, like Infura, Alchemy, etc.
    - multiple EVM-based blockchains, like Ethereum, Binance Smart Chain, etc.
+   - Websocket and HTTP RPC
    - rate limiting and retrying
    - skip validation of RPC method parameters
    - debug mode
    - cache
    - custom RPC method
 2. Get token price from Uniswap and other DEXs
 3. Get Uniswap liquidity pool information
@@ -37,15 +38,24 @@
 ```bash
 pip install w3tools
 ```
 
 ## Usage
 
 ```python
+from w3tools.chain import ChainId
+from w3tools.w3 import make_w3
 
+w3 = make_w3(
+    ChainId.ETH,
+    "quicknode",
+    api_key="your key",
+)
+
+print(w3.eth.block_number)
 ```
 
 ## Credits
 
 - [Web3.py](https://github.com/ethereum/web3.py)
 
 ## Development
```

