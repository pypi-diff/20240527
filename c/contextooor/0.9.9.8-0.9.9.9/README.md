# Comparing `tmp/contextooor-0.9.9.8.tar.gz` & `tmp/contextooor-0.9.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contextooor-0.9.9.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "contextooor-0.9.9.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `contextooor-0.9.9.8.tar` & `contextooor-0.9.9.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0       54 2024-03-14 14:32:01.088125 contextooor-0.9.9.8/.gitignore
--rw-r--r--   0        0        0    71515 2024-03-14 15:04:16.974143 contextooor-0.9.9.8/Cargo.lock
--rw-r--r--   0        0        0      334 2024-03-14 15:07:01.741088 contextooor-0.9.9.8/Cargo.toml
--rw-r--r--   0        0        0    10457 2024-01-31 18:27:21.928630 contextooor-0.9.9.8/btc_sanctioned_addresses.parquet
--rw-r--r--   0        0        0    51376 2024-05-06 20:31:27.436460 contextooor-0.9.9.8/coingecko.parquet
-drwxr-xr-x   0        0        0        0 2024-05-13 23:21:23.117782 contextooor-0.9.9.8/contextooor/
--rw-r--r--   0        0        0     4552 2024-03-12 15:15:26.385216 contextooor-0.9.9.8/contextooor/README.md
--rw-r--r--   0        0        0       95 2024-05-13 23:46:36.455951 contextooor-0.9.9.8/contextooor/__init__.py
--rw-r--r--   0        0        0     6285 2024-02-15 15:30:15.619991 contextooor-0.9.9.8/contextooor/btc.py
--rw-r--r--   0        0        0    29738 2023-12-23 03:26:26.687369 contextooor-0.9.9.8/contextooor/core/V2_router/V2_router.py
--rw-r--r--   0        0        0    28278 2023-12-23 03:26:26.691166 contextooor-0.9.9.8/contextooor/core/V3_router/V3_router.py
--rw-r--r--   0        0        0     1497 2023-12-23 03:26:26.694388 contextooor-0.9.9.8/contextooor/core/safe_math.py
--rw-r--r--   0        0        0    13969 2023-12-23 03:26:26.695305 contextooor-0.9.9.8/contextooor/core/universal_router/V2_universal_router.py
--rw-r--r--   0        0        0    17995 2023-12-23 03:26:26.696171 contextooor-0.9.9.8/contextooor/core/universal_router/V3_universal_router.py
--rw-r--r--   0        0        0     7534 2023-12-23 03:26:26.699278 contextooor-0.9.9.8/contextooor/core/universal_router/data.py
--rw-r--r--   0        0        0     5400 2023-12-23 03:26:26.699936 contextooor-0.9.9.8/contextooor/core/universal_router/policies.py
--rw-r--r--   0        0        0    19785 2024-05-13 20:49:45.591671 contextooor-0.9.9.8/contextooor/eth.py
--rw-r--r--   0        0        0    24125 2024-02-15 15:31:50.362363 contextooor-0.9.9.8/contextooor/eth_uniswap.py
--rw-r--r--   0        0        0     2302 2024-02-15 15:32:16.690084 contextooor-0.9.9.8/contextooor/etherscan_testing.py
--rw-r--r--   0        0        0      476 2024-03-12 16:19:03.385043 contextooor-0.9.9.8/contextooor/near.py
--rw-r--r--   0        0        0     2030 2024-01-31 18:53:43.352487 contextooor-0.9.9.8/contextooor/ofac_btc_cronjob.py
--rw-r--r--   0        0        0     1460 2024-03-12 15:29:50.972039 contextooor-0.9.9.8/contextooor/sol.py
-drwxr-xr-x   0        0        0        0 2024-05-13 23:16:59.065773 contextooor-0.9.9.8/cryo/
--rw-r--r--   0        0        0      629 2024-03-14 15:36:17.343067 contextooor-0.9.9.8/decode_near.js
--rw-r--r--   0        0        0        0 2024-03-14 14:44:04.200505 contextooor-0.9.9.8/decode_near.rs
--rw-r--r--   0        0        0     2446 2024-03-13 18:45:11.465827 contextooor-0.9.9.8/encode_near.js
-lrwxr-xr-x   0        0        0        0 2024-03-13 13:55:58.946196 contextooor-0.9.9.8/node_modules/.bin/mustache -> ../mustache/bin/mustache
--rw-r--r--   0        0        0    20111 2024-03-14 15:31:21.934951 contextooor-0.9.9.8/node_modules/.package-lock.json
--rw-r--r--   0        0        0    20279 2024-03-14 15:31:21.931456 contextooor-0.9.9.8/package-lock.json
--rw-r--r--   0        0        0      131 2024-03-14 15:31:21.924015 contextooor-0.9.9.8/package.json
--rw-r--r--   0        0        0      600 2024-05-13 23:45:38.948684 contextooor-0.9.9.8/pyproject.toml
--rw-r--r--   0        0        0     2313 2024-02-15 15:31:40.253535 contextooor-0.9.9.8/test.py
--rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 contextooor-0.9.9.8/PKG-INFO
+-rw-r--r--   0        0        0       72 2024-05-27 17:04:45.134848 contextooor-0.9.9.9/.gitignore
+-rw-r--r--   0        0        0    71515 2024-03-14 15:04:16.974143 contextooor-0.9.9.9/Cargo.lock
+-rw-r--r--   0        0        0      334 2024-03-14 15:07:01.741088 contextooor-0.9.9.9/Cargo.toml
+-rw-r--r--   0        0        0    10457 2024-01-31 18:27:21.928630 contextooor-0.9.9.9/btc_sanctioned_addresses.parquet
+-rw-r--r--   0        0        0    51376 2024-05-06 20:31:27.436460 contextooor-0.9.9.9/coingecko.parquet
+drwxr-xr-x   0        0        0        0 2024-05-27 17:07:21.907443 contextooor-0.9.9.9/contextooor/
+-rw-r--r--   0        0        0     4552 2024-03-12 15:15:26.385216 contextooor-0.9.9.9/contextooor/README.md
+-rw-r--r--   0        0        0       95 2024-05-27 16:52:39.962528 contextooor-0.9.9.9/contextooor/__init__.py
+-rw-r--r--   0        0        0     6285 2024-02-15 15:30:15.619991 contextooor-0.9.9.9/contextooor/btc.py
+-rw-r--r--   0        0        0     2055 2024-05-27 17:07:21.906738 contextooor-0.9.9.9/contextooor/core/Chainalysis/chainalysis_ofac_api.py
+-rw-r--r--   0        0        0    29738 2023-12-23 03:26:26.687369 contextooor-0.9.9.9/contextooor/core/V2_router/V2_router.py
+-rw-r--r--   0        0        0    28278 2023-12-23 03:26:26.691166 contextooor-0.9.9.9/contextooor/core/V3_router/V3_router.py
+-rw-r--r--   0        0        0     1497 2023-12-23 03:26:26.694388 contextooor-0.9.9.9/contextooor/core/safe_math.py
+-rw-r--r--   0        0        0    13969 2023-12-23 03:26:26.695305 contextooor-0.9.9.9/contextooor/core/universal_router/V2_universal_router.py
+-rw-r--r--   0        0        0    17995 2023-12-23 03:26:26.696171 contextooor-0.9.9.9/contextooor/core/universal_router/V3_universal_router.py
+-rw-r--r--   0        0        0     7534 2023-12-23 03:26:26.699278 contextooor-0.9.9.9/contextooor/core/universal_router/data.py
+-rw-r--r--   0        0        0     5400 2023-12-23 03:26:26.699936 contextooor-0.9.9.9/contextooor/core/universal_router/policies.py
+-rw-r--r--   0        0        0    21057 2024-05-27 17:07:21.907599 contextooor-0.9.9.9/contextooor/eth.py
+-rw-r--r--   0        0        0    24125 2024-02-15 15:31:50.362363 contextooor-0.9.9.9/contextooor/eth_uniswap.py
+-rw-r--r--   0        0        0     2302 2024-02-15 15:32:16.690084 contextooor-0.9.9.9/contextooor/etherscan_testing.py
+-rw-r--r--   0        0        0      476 2024-03-12 16:19:03.385043 contextooor-0.9.9.9/contextooor/near.py
+-rw-r--r--   0        0        0     2030 2024-01-31 18:53:43.352487 contextooor-0.9.9.9/contextooor/ofac_btc_cronjob.py
+-rw-r--r--   0        0        0     1460 2024-03-12 15:29:50.972039 contextooor-0.9.9.9/contextooor/sol.py
+-rw-r--r--   0        0        0      629 2024-03-14 15:36:17.343067 contextooor-0.9.9.9/decode_near.js
+-rw-r--r--   0        0        0        0 2024-03-14 14:44:04.200505 contextooor-0.9.9.9/decode_near.rs
+-rw-r--r--   0        0        0     2446 2024-03-13 18:45:11.465827 contextooor-0.9.9.9/encode_near.js
+lrwxr-xr-x   0        0        0        0 2024-03-13 13:55:58.946196 contextooor-0.9.9.9/node_modules/.bin/mustache -> ../mustache/bin/mustache
+-rw-r--r--   0        0        0    20111 2024-03-14 15:31:21.934951 contextooor-0.9.9.9/node_modules/.package-lock.json
+-rw-r--r--   0        0        0    20279 2024-03-14 15:31:21.931456 contextooor-0.9.9.9/package-lock.json
+-rw-r--r--   0        0        0      131 2024-03-14 15:31:21.924015 contextooor-0.9.9.9/package.json
+-rw-r--r--   0        0        0      600 2024-05-13 23:45:38.948684 contextooor-0.9.9.9/pyproject.toml
+-rw-r--r--   0        0        0     2313 2024-02-15 15:31:40.253535 contextooor-0.9.9.9/test.py
+-rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 contextooor-0.9.9.9/PKG-INFO
```

### Comparing `contextooor-0.9.9.8/Cargo.lock` & `contextooor-0.9.9.9/Cargo.lock`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.8/btc_sanctioned_addresses.parquet` & `contextooor-0.9.9.9/btc_sanctioned_addresses.parquet`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.8/coingecko.parquet` & `contextooor-0.9.9.9/coingecko.parquet`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.8/contextooor/README.md` & `contextooor-0.9.9.9/contextooor/README.md`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.8/contextooor/btc.py` & `contextooor-0.9.9.9/contextooor/btc.py`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.8/contextooor/core/V2_router/V2_router.py` & `contextooor-0.9.9.9/contextooor/core/V2_router/V2_router.py`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.8/contextooor/core/V3_router/V3_router.py` & `contextooor-0.9.9.9/contextooor/core/V3_router/V3_router.py`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.8/contextooor/core/safe_math.py` & `contextooor-0.9.9.9/contextooor/core/safe_math.py`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.8/contextooor/core/universal_router/V2_universal_router.py` & `contextooor-0.9.9.9/contextooor/core/universal_router/V2_universal_router.py`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.8/contextooor/core/universal_router/V3_universal_router.py` & `contextooor-0.9.9.9/contextooor/core/universal_router/V3_universal_router.py`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.8/contextooor/core/universal_router/data.py` & `contextooor-0.9.9.9/contextooor/core/universal_router/data.py`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.8/contextooor/core/universal_router/policies.py` & `contextooor-0.9.9.9/contextooor/core/universal_router/policies.py`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.8/contextooor/eth.py` & `contextooor-0.9.9.9/contextooor/eth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from web3 import Web3
 import requests
 import json
 import subprocess
 import os
 import polars as pl
+from contextooor.core.Chainalysis.chainalysis_ofac_api import Chainalysis
+
+DEMO_SANCTIONED_ADDRESSES=["1JHdQHkBZiim1cb4hyUh2PbzEbbg6z2Trf", "0x01e2919679362dFBC9ee1644Ba9C6da6D6245BB1"]
+
+DEMO_NON_SANCTIONED_ADDRESSES=["bc1p7pztjz9qyupr8ztwqy2y3yl7u6y2nvfna3g54rq3s3d7d0k5ee4syceevj", "0x01B2f8877f3e8F366eF4D4F48230949123733897"]
 
 class Snippets:
 
     def __init__(self,w3=Web3(Web3.HTTPProvider("https://eth.public-rpc.com")),etherscan_api_key="PGJ5AYE9WGD77YPS4F3NGQ33MB5YI7JYS8"):
         self.etherscan_api_key=etherscan_api_key
         self.web3=w3
         try:
@@ -23,14 +28,19 @@
             'Authorization': f'bearer {forta_api_key}'}
         data = """{"query":"query Labels($input: LabelsInput) {\\n  labels(input: $input) {\\n    labels {\\n      id\\n      label {\\n        entity\\n        entityType\\n        label\\n      }\\n      source {\\n        id\\n      }\\n    }\\n  }\\n}","variables":{"input":{"entities":"""+'"'+address+'"'+""","labels":["attacker-contract","attacker-eoa"],"sourceIds":"0x80ed808b586aeebe9cdd4088ea4dea0a8e322909c0e4493c993e060e89c09ed1"}}}"""
         response = requests.post('https://api.forta.network/graphql', headers=headers, data=data)
         response=response.json()
         if response['data']['labels']['labels']!=[]:
             return True
         return False
+        
+    def is_sanctioned(self,chainalysis_api_key,address):
+        chainalysis = Chainalysis(chainalysis_api_key)
+        is_sanctioned = chainalysis.is_sanctioned(address)
+        return is_sanctioned
 
     def get_usd_value(self,token):
         formatted_address="ethereum:"+token
         value=requests.get(f"https://coins.llama.fi/prices/current/{formatted_address}".format(formatted_address)).json()
         return int(value["coins"][formatted_address]['price'])
 
     def decode_approval(self,etherscan_txn):
@@ -252,8 +262,28 @@
 
     def is_poisonned_address(self,from_address,to_address, first_n=4, last_n=4, current_block_number=99999999):
         from_address=from_address.lower()
         to_address=to_address.lower()
         df=self.get_tx_history(from_address,current_block_number)
         matchbook=self.find_matches(df,from_address,to_address,first_n,last_n)
         return self.parse_results(matchbook,to_address)
-    
+    
+def test_snippets():
+    api_key = os.getenv('CHAINALYSIS_API_KEY')
+    if api_key is None:
+        raise ValueError("CHAINALYSIS_API_KEY is not set")
+
+    chainalysis = Chainalysis(api_key)
+    for address in DEMO_SANCTIONED_ADDRESSES:
+      is_sanctioned = chainalysis.is_sanctioned(address)
+      assert is_sanctioned == True
+      
+      sanction_data = chainalysis.get_sanctioned_address_data(address)
+      assert sanction_data[0]["category"] == "sanctioned entity"
+      
+    for address in DEMO_NON_SANCTIONED_ADDRESSES:
+      is_sanctioned = chainalysis.is_sanctioned(address)
+      assert is_sanctioned == False
+
+      sanction_data = chainalysis.get_sanctioned_address_data(address)
+      assert len(sanction_data) == 0
+
```

### Comparing `contextooor-0.9.9.8/contextooor/eth_uniswap.py` & `contextooor-0.9.9.9/contextooor/eth_uniswap.py`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.8/contextooor/etherscan_testing.py` & `contextooor-0.9.9.9/contextooor/etherscan_testing.py`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.8/contextooor/ofac_btc_cronjob.py` & `contextooor-0.9.9.9/contextooor/ofac_btc_cronjob.py`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.8/contextooor/sol.py` & `contextooor-0.9.9.9/contextooor/sol.py`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.8/decode_near.js` & `contextooor-0.9.9.9/decode_near.js`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.8/encode_near.js` & `contextooor-0.9.9.9/encode_near.js`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.8/node_modules/.package-lock.json` & `contextooor-0.9.9.9/node_modules/.package-lock.json`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.8/package-lock.json` & `contextooor-0.9.9.9/package-lock.json`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.8/pyproject.toml` & `contextooor-0.9.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `contextooor-0.9.9.8/test.py` & `contextooor-0.9.9.9/test.py`

 * *Files identical despite different names*

