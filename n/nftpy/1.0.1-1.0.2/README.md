# Comparing `tmp/nftpy-1.0.1.tar.gz` & `tmp/nftpy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nftpy-1.0.1.tar", max compression
+gzip compressed data, was "nftpy-1.0.2.tar", max compression
```

## Comparing `nftpy-1.0.1.tar` & `nftpy-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,11 @@
--rw-r--r--   0        0        0     1091 2024-05-26 15:17:47.475262 nftpy-1.0.1/LICENSE
--rw-r--r--   0        0        0      192 2024-05-27 00:06:47.340203 nftpy-1.0.1/nftpy/__init__.py
--rw-r--r--   0        0        0     1361 2024-05-27 00:23:21.883841 nftpy-1.0.1/nftpy/errors.py
--rw-r--r--   0        0        0      108 2024-05-26 23:26:30.765898 nftpy-1.0.1/nftpy/EVM/__init__.py
--rw-r--r--   0        0        0      299 2024-05-26 23:26:31.229002 nftpy-1.0.1/nftpy/EVM/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     3304 2024-05-26 23:26:31.233003 nftpy-1.0.1/nftpy/EVM/__pycache__/abi.cpython-312.pyc
--rw-r--r--   0        0        0     3655 2024-05-26 23:17:54.447994 nftpy-1.0.1/nftpy/EVM/__pycache__/chains.cpython-312.pyc
--rw-r--r--   0        0        0     7436 2024-05-26 23:39:14.392610 nftpy-1.0.1/nftpy/EVM/__pycache__/nft.cpython-312.pyc
--rw-r--r--   0        0        0     9518 2024-05-26 23:26:30.769899 nftpy-1.0.1/nftpy/EVM/abi.py
--rw-r--r--   0        0        0     4346 2024-05-26 23:11:38.342594 nftpy-1.0.1/nftpy/EVM/chains.py
--rw-r--r--   0        0        0     6241 2024-05-27 00:25:39.520889 nftpy-1.0.1/nftpy/EVM/nft.py
--rw-r--r--   0        0        0     8490 2024-05-27 00:24:28.197791 nftpy-1.0.1/nftpy/opensea.py
--rw-r--r--   0        0        0      512 2024-05-27 01:20:58.029872 nftpy-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     8489 2024-05-27 01:10:51.882679 nftpy-1.0.1/README.md
--rw-r--r--   0        0        0     8934 1970-01-01 00:00:00.000000 nftpy-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-05-27 01:41:06.348086 nftpy-1.0.2/LICENSE
+-rw-r--r--   0        0        0      228 2024-05-27 01:42:48.914058 nftpy-1.0.2/nftpy/__init__.py
+-rw-r--r--   0        0        0     1361 2024-05-27 01:41:06.351086 nftpy-1.0.2/nftpy/errors.py
+-rw-r--r--   0        0        0      108 2024-05-27 01:41:06.349086 nftpy-1.0.2/nftpy/EVM/__init__.py
+-rw-r--r--   0        0        0     9518 2024-05-27 01:41:06.350086 nftpy-1.0.2/nftpy/EVM/abi.py
+-rw-r--r--   0        0        0     4346 2024-05-27 01:41:06.350086 nftpy-1.0.2/nftpy/EVM/chains.py
+-rw-r--r--   0        0        0     6241 2024-05-27 01:41:06.350086 nftpy-1.0.2/nftpy/EVM/nft.py
+-rw-r--r--   0        0        0     8490 2024-05-27 01:41:06.351086 nftpy-1.0.2/nftpy/opensea.py
+-rw-r--r--   0        0        0      570 2024-05-27 01:57:09.605403 nftpy-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8483 2024-05-27 01:41:06.349086 nftpy-1.0.2/README.md
+-rw-r--r--   0        0        0     8931 1970-01-01 00:00:00.000000 nftpy-1.0.2/PKG-INFO
```

### Comparing `nftpy-1.0.1/LICENSE` & `nftpy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nftpy-1.0.1/nftpy/errors.py` & `nftpy-1.0.2/nftpy/errors.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.0.1/nftpy/EVM/abi.py` & `nftpy-1.0.2/nftpy/EVM/abi.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.0.1/nftpy/EVM/chains.py` & `nftpy-1.0.2/nftpy/EVM/chains.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.0.1/nftpy/EVM/nft.py` & `nftpy-1.0.2/nftpy/EVM/nft.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.0.1/nftpy/opensea.py` & `nftpy-1.0.2/nftpy/opensea.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.0.1/pyproject.toml` & `nftpy-1.0.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 [tool.poetry]
 name = "nftpy"
-version = "1.0.1"
+version = "1.0.2"
 description = "A NFT specific Python library for easy NFT integration in Python"
 authors = ["CoulterStutz <coultercash@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/coulterstutz/nftpy"
 repository = "https://github.com/coulterstutz/nftpy"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 web3 = "^6.2.0"
 requests = "^2.28.1"
 
+[tool.poetry.group.dev.dependencies]
+twine = "^5.1.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nftpy-1.0.1/README.md` & `nftpy-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,15 @@
 We will first start off by creating our class. We are going to define our class with three arguments:
 - contract_address: The address of the contract you are trying to query.
 - abi: The ABI of the contract you are trying to query. The EVM.ABI class provides presets for our ABI. You can also paste an ABI into the field.
 - network: This dictates what RPC URL to use and sets a preset that works best with the network.
 - rpc_url: If you do not want to use a preset and instead want to use a custom RPC, define it using this field.
 
 ```python
-import nftpy.EVM as EVM
-
+import NFTPy.EVM as EVM
 Pixelmon = EVM.NFT("0x32973908FaeE0Bf825A343000fE412ebE56F802A", abi=EVM.ABI.ERC721, network=EVM.Chains.ETH)
 #                   Contract Address                                ABI              Network To Query (Ethereum)
 ```
 Now that we have created our NFT object, we can query it. We will start with getting the metadata of a token. I am just putting a random token as the argument.
 ```python
 print(Pixelmon.get_token_metadata(5580))
 ```
@@ -107,18 +106,16 @@
 ### Interacting with OpenSea API | NFTPy.OpenSea
 We will first start by creating our class with the following arguments:
 - api_key: Your OpenSea API key.
 - chain: The blockchain network (e.g., Ethereum, Polygon).
 - collection_slug: The slug of the collection you want to query (the last part of the url when browsing the collection on opensea) This assigns the interface to a specific collection. If you are using the interface to view multiple collections then you should leave this blank
 
 **Please Note**: When defining the chain, it should be done with NFTPy.OpenSea.Chain as the api requires a special format for chain definition
-
 ```python
-from nftpy import OpenSea, OpenSeaChain
-
+from NFTPy import OpenSea, OpenSeaChain
 opensea = OpenSea(api_key='your-opensea-api-key', chain=OpenSeaChain.POLYGON, collection_slug='your-collection-slug')
 ```
 If we want to query the stats of the NFT collection we can run the following command. If you did not define a collection slug when initializing the interface you will need to define it inside this function
 ```python
 opensea.get_collection_stats()
 ```
 After running that, we should see an output resembling this:
```

### Comparing `nftpy-1.0.1/PKG-INFO` & `nftpy-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nftpy
-Version: 1.0.1
+Version: 1.0.2
 Summary: A NFT specific Python library for easy NFT integration in Python
 Home-page: https://github.com/coulterstutz/nftpy
 License: MIT
 Author: CoulterStutz
 Author-email: coultercash@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -58,16 +58,15 @@
 We will first start off by creating our class. We are going to define our class with three arguments:
 - contract_address: The address of the contract you are trying to query.
 - abi: The ABI of the contract you are trying to query. The EVM.ABI class provides presets for our ABI. You can also paste an ABI into the field.
 - network: This dictates what RPC URL to use and sets a preset that works best with the network.
 - rpc_url: If you do not want to use a preset and instead want to use a custom RPC, define it using this field.
 
 ```python
-import nftpy.EVM as EVM
-
+import NFTPy.EVM as EVM
 Pixelmon = EVM.NFT("0x32973908FaeE0Bf825A343000fE412ebE56F802A", abi=EVM.ABI.ERC721, network=EVM.Chains.ETH)
 #                   Contract Address                                ABI              Network To Query (Ethereum)
 ```
 Now that we have created our NFT object, we can query it. We will start with getting the metadata of a token. I am just putting a random token as the argument.
 ```python
 print(Pixelmon.get_token_metadata(5580))
 ```
@@ -124,18 +123,16 @@
 ### Interacting with OpenSea API | NFTPy.OpenSea
 We will first start by creating our class with the following arguments:
 - api_key: Your OpenSea API key.
 - chain: The blockchain network (e.g., Ethereum, Polygon).
 - collection_slug: The slug of the collection you want to query (the last part of the url when browsing the collection on opensea) This assigns the interface to a specific collection. If you are using the interface to view multiple collections then you should leave this blank
 
 **Please Note**: When defining the chain, it should be done with NFTPy.OpenSea.Chain as the api requires a special format for chain definition
-
 ```python
-from nftpy import OpenSea, OpenSeaChain
-
+from NFTPy import OpenSea, OpenSeaChain
 opensea = OpenSea(api_key='your-opensea-api-key', chain=OpenSeaChain.POLYGON, collection_slug='your-collection-slug')
 ```
 If we want to query the stats of the NFT collection we can run the following command. If you did not define a collection slug when initializing the interface you will need to define it inside this function
 ```python
 opensea.get_collection_stats()
 ```
 After running that, we should see an output resembling this:
```

