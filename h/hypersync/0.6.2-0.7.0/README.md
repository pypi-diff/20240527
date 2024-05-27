# Comparing `tmp/hypersync-0.6.2.tar.gz` & `tmp/hypersync-0.7.0.tar.gz`

## Comparing `hypersync-0.6.2.tar` & `hypersync-0.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      787 1970-01-01 00:00:00.000000 hypersync-0.6.2/Cargo.toml
--rw-r--r--   0     1001      127     2988 2024-05-05 00:04:33.000000 hypersync-0.6.2/.github/workflows/publish.yml
--rw-r--r--   0     1001      127      699 2024-05-05 00:04:33.000000 hypersync-0.6.2/.gitignore
--rw-r--r--   0     1001      127    16725 2024-05-05 00:04:33.000000 hypersync-0.6.2/LICENSE
--rw-r--r--   0     1001      127      137 2024-05-05 00:04:33.000000 hypersync-0.6.2/README.md
--rw-r--r--   0     1001      127     4840 2024-05-05 00:04:33.000000 hypersync-0.6.2/erc20.abi.json
--rw-r--r--   0     1001      127     3232 2024-05-05 00:04:33.000000 hypersync-0.6.2/examples/all-erc20.py
--rw-r--r--   0     1001      127      959 2024-05-05 00:04:33.000000 hypersync-0.6.2/examples/simple-blocks-and-transaction-hashes.py
--rw-r--r--   0     1001      127      902 2024-05-05 00:04:33.000000 hypersync-0.6.2/examples/simple-blocks-and-transactions.py
--rw-r--r--   0     1001      127     1201 2024-05-05 00:04:33.000000 hypersync-0.6.2/examples/simple-logs-of-event.py
--rw-r--r--   0     1001      127      935 2024-05-05 00:04:33.000000 hypersync-0.6.2/examples/simple-logs.py
--rw-r--r--   0     1001      127     2694 2024-05-05 00:04:33.000000 hypersync-0.6.2/examples/top-usdt.py
--rw-r--r--   0     1001      127     5558 2024-05-05 00:04:33.000000 hypersync-0.6.2/examples/wallet.py
--rw-r--r--   0     1001      127     1906 2024-05-05 00:04:33.000000 hypersync-0.6.2/examples/watch.py
--rw-r--r--   0     1001      127     9132 2024-05-05 00:04:33.000000 hypersync-0.6.2/hypersync/__init__.py
--rw-r--r--   0     1001      127     2752 2024-05-05 00:04:33.000000 hypersync-0.6.2/src/config.rs
--rw-r--r--   0     1001      127     4241 2024-05-05 00:04:33.000000 hypersync-0.6.2/src/decode.rs
--rw-r--r--   0     1001      127    13235 2024-05-05 00:04:33.000000 hypersync-0.6.2/src/from_arrow.rs
--rw-r--r--   0     1001      127    20356 2024-05-05 00:04:33.000000 hypersync-0.6.2/src/lib.rs
--rw-r--r--   0     1001      127     7062 2024-05-05 00:04:33.000000 hypersync-0.6.2/src/query.rs
--rw-r--r--   0     1001      127     6949 2024-05-05 00:04:33.000000 hypersync-0.6.2/src/types.rs
--rw-r--r--   0     1001      127     9152 2024-05-05 00:04:33.000000 hypersync-0.6.2/test.py
--rw-r--r--   0     1001      127    84516 2024-05-05 00:04:33.000000 hypersync-0.6.2/Cargo.lock
--rw-r--r--   0     1001      127      604 2024-05-05 00:04:33.000000 hypersync-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      671 1970-01-01 00:00:00.000000 hypersync-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 hypersync-0.7.0/Cargo.toml
+-rw-r--r--   0     1001      127     2988 2024-05-27 17:56:39.000000 hypersync-0.7.0/.github/workflows/publish.yml
+-rw-r--r--   0     1001      127      699 2024-05-27 17:56:39.000000 hypersync-0.7.0/.gitignore
+-rw-r--r--   0     1001      127    16725 2024-05-27 17:56:39.000000 hypersync-0.7.0/LICENSE
+-rw-r--r--   0     1001      127      137 2024-05-27 17:56:39.000000 hypersync-0.7.0/README.md
+-rw-r--r--   0     1001      127     2951 2024-05-27 17:56:39.000000 hypersync-0.7.0/examples/all-erc20.py
+-rw-r--r--   0     1001      127      981 2024-05-27 17:56:39.000000 hypersync-0.7.0/examples/simple-blocks-and-transaction-hashes.py
+-rw-r--r--   0     1001      127      924 2024-05-27 17:56:39.000000 hypersync-0.7.0/examples/simple-blocks-and-transactions.py
+-rw-r--r--   0     1001      127     1223 2024-05-27 17:56:39.000000 hypersync-0.7.0/examples/simple-logs-of-event.py
+-rw-r--r--   0     1001      127      957 2024-05-27 17:56:39.000000 hypersync-0.7.0/examples/simple-logs.py
+-rw-r--r--   0     1001      127     2722 2024-05-27 17:56:39.000000 hypersync-0.7.0/examples/top-usdt.py
+-rw-r--r--   0     1001      127     4980 2024-05-27 17:56:39.000000 hypersync-0.7.0/examples/wallet.py
+-rw-r--r--   0     1001      127     2013 2024-05-27 17:56:39.000000 hypersync-0.7.0/examples/watch.py
+-rw-r--r--   0     1001      127     9811 2024-05-27 17:56:39.000000 hypersync-0.7.0/hypersync/__init__.py
+-rw-r--r--   0     1001      127     2410 2024-05-27 17:56:39.000000 hypersync-0.7.0/src/arrow_ffi.rs
+-rw-r--r--   0     1001      127     2989 2024-05-27 17:56:39.000000 hypersync-0.7.0/src/config.rs
+-rw-r--r--   0     1001      127     3628 2024-05-27 17:56:39.000000 hypersync-0.7.0/src/decode.rs
+-rw-r--r--   0     1001      127     7054 2024-05-27 17:56:39.000000 hypersync-0.7.0/src/lib.rs
+-rw-r--r--   0     1001      127     6251 2024-05-27 17:56:39.000000 hypersync-0.7.0/src/query.rs
+-rw-r--r--   0     1001      127     8746 2024-05-27 17:56:39.000000 hypersync-0.7.0/src/response.rs
+-rw-r--r--   0     1001      127    15992 2024-05-27 17:56:39.000000 hypersync-0.7.0/src/types.rs
+-rw-r--r--   0     1001      127     8784 2024-05-27 17:56:39.000000 hypersync-0.7.0/test.py
+-rw-r--r--   0     1001      127    85048 2024-05-27 17:56:39.000000 hypersync-0.7.0/Cargo.lock
+-rw-r--r--   0     1001      127      561 2024-05-27 17:56:39.000000 hypersync-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      671 1970-01-01 00:00:00.000000 hypersync-0.7.0/PKG-INFO
```

### Comparing `hypersync-0.6.2/.github/workflows/publish.yml` & `hypersync-0.7.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `hypersync-0.6.2/.gitignore` & `hypersync-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hypersync-0.6.2/LICENSE` & `hypersync-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hypersync-0.6.2/examples/all-erc20.py` & `hypersync-0.7.0/examples/all-erc20.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import hypersync
 import asyncio
-from hypersync import BlockField, TransactionField, LogField
+from hypersync import BlockField, TransactionField, LogField, ClientConfig
 
 async def main():
     # Create hypersync client using the arbitrum hypersync endpoint
-    client = hypersync.HypersyncClient("https://arbitrum.hypersync.xyz")
+    client = hypersync.HypersyncClient(ClientConfig())
 
     # The query to run
     query = hypersync.Query(
 		# start from block 0 and go to the end of the chain (we don't specify a toBlock).
 		from_block=0,
         # The logs we want. We will also automatically get transactions and blocks relating to these logs (the query implicitly joins them).
 		logs=[hypersync.LogSelection(
@@ -34,49 +34,42 @@
                 TransactionField.TRANSACTION_INDEX,
                 TransactionField.HASH,
                 TransactionField.FROM,
                 TransactionField.TO,
                 TransactionField.VALUE,
                 TransactionField.INPUT,
 			]
-		)
+		),
     )
 
     print("Running the query...")
 
     # Run the query once, the query is automatically paginated so it will return when it reaches some limit (time, response size etc.)
     # there is a next_block field on the response object so we can set the from_block of our query to this value and continue our query until
     # res.next_block is equal to res.archive_height or query.to_block in case we specified an end block.
-    res = await client.send_req(query)
+    res = await client.get(query)
 
     print(f"Ran the query once.  Next block to query is {res.next_block}")
 
-    # read json abi file for erc20
-    with open('./erc20.abi.json', 'r') as json_file:
-        abi = json_file.read()
-
-    # Map of contract_address -> abi
-    abis = {}
-
-    # every log we get should be decodable by this abi but we don't know
-    # the specific contract addresses since we are indexing all erc20 transfers.
-    for log in res.data.logs:
-        abis[log.address] = abi
-
-    # Create a decoder with our mapping
-    decoder = hypersync.Decoder(abis)
+    decoder = hypersync.Decoder([
+        "Transfer(address indexed from, address indexed to, uint256 value)"
+    ])
 
     # Decode the log on a background thread so we don't block the event loop.
     # Can also use decoder.decode_logs_sync if it is more convenient.
     decoded_logs = await decoder.decode_logs(res.data.logs)
 
     # Let's count total volume, it is meaningless because of currency differences but good as an example.
     total_volume = 0
     for log in decoded_logs:
-        total_volume += log.body[0]
+        #skip invalid logs
+        if log is None:
+            continue
+
+        total_volume += log.body[0].val
     
     total_blocks = res.next_block - query.from_block
 
     print(f"total volume was {total_volume} in {total_blocks} blocks")
 
 
 asyncio.run(main())
```

### Comparing `hypersync-0.6.2/examples/simple-blocks-and-transaction-hashes.py` & `hypersync-0.7.0/examples/simple-blocks-and-transaction-hashes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import hypersync
 import asyncio
 
 # returns all blocks and the hashes of the transactions (not entire transaction objects) within a block range
 
 async def main():
     # Create hypersync client using the mainnet hypersync endpoint (default)
-    client = hypersync.HypersyncClient()
+    client = hypersync.HypersyncClient(hypersync.ClientConfig())
 
-    query = client.preset_query_blocks_and_transaction_hashes(17_000_000, 17_000_050)
+    query = hypersync.preset_query_blocks_and_transaction_hashes(17_000_000, 17_000_050)
 
     print("Running the query...")
 
     # Run the query once, the query is automatically paginated so it will return when it reaches some limit (time, response size etc.)
     # there is a next_block field on the response object so we can set the from_block of our query to this value and continue our query until
     # res.next_block is equal to res.archive_height or query.to_block in case we specified an end block.
-    res = await client.send_req(query)
+    res = await client.get(query)
 
     print(f"Query returned {len(res.data.blocks)} blocks and {len(res.data.transactions)} transaction hashes")
 
 
 
 asyncio.run(main())
```

### Comparing `hypersync-0.6.2/examples/simple-blocks-and-transactions.py` & `hypersync-0.7.0/examples/simple-logs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import hypersync
 import asyncio
 
-# returns all block and transaction objects within a block range
+# returns all logs from a contract within a block range
 
 async def main():
     # Create hypersync client using the mainnet hypersync endpoint (default)
-    client = hypersync.HypersyncClient()
+    client = hypersync.HypersyncClient(hypersync.ClientConfig())
 
-    query = client.preset_query_blocks_and_transactions(17_000_000, 17_000_050)
+    usdt_contract = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
+
+    query = hypersync.preset_query_logs(usdt_contract, 17_000_000, 17_000_050)
 
     print("Running the query...")
 
     # Run the query once, the query is automatically paginated so it will return when it reaches some limit (time, response size etc.)
     # there is a next_block field on the response object so we can set the from_block of our query to this value and continue our query until
     # res.next_block is equal to res.archive_height or query.to_block in case we specified an end block.
-    res = await client.send_req(query)
+    res = await client.get(query)
 
-    print(f"Query returned {len(res.data.blocks)} blocks and {len(res.data.transactions)} transactions")
+    print(f"Query returned {len(res.data.logs)} logs from contract {usdt_contract}")
 
 
 
 asyncio.run(main())
```

### Comparing `hypersync-0.6.2/examples/simple-logs-of-event.py` & `hypersync-0.7.0/examples/simple-logs-of-event.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import hypersync
 import asyncio
 
 # returns all logs of a specific event from a contract within a block range
 
 async def main():
     # Create hypersync client using the mainnet hypersync endpoint (default)
-    client = hypersync.HypersyncClient()
+    client = hypersync.HypersyncClient(hypersync.ClientConfig())
 
     usdt_contract = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
 
     # topic0 of transaction event signature (hash of event signature)
     # query will return logs of this event
     event_topic_0 = "0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef"
 
-    query = client.preset_query_logs_of_event(usdt_contract, event_topic_0, 17_000_000, 17_000_050)
+    query = hypersync.preset_query_logs_of_event(usdt_contract, event_topic_0, 17_000_000, 17_000_050)
 
     print("Running the query...")
 
     # Run the query once, the query is automatically paginated so it will return when it reaches some limit (time, response size etc.)
     # there is a next_block field on the response object so we can set the from_block of our query to this value and continue our query until
     # res.next_block is equal to res.archive_height or query.to_block in case we specified an end block.
-    res = await client.send_req(query)
+    res = await client.get(query)
 
     print(f"Query returned {len(res.data.logs)} logs of transfer events from contract {usdt_contract}")
 
 
 
 asyncio.run(main())
```

### Comparing `hypersync-0.6.2/examples/top-usdt.py` & `hypersync-0.7.0/examples/top-usdt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import hypersync
 from hypersync import LogSelection, LogField, DataType, FieldSelection, ColumnMapping, TransactionField
 import asyncio
 import polars
 
 async def collect_events():
-    client = hypersync.HypersyncClient()
+    client = hypersync.HypersyncClient(hypersync.ClientConfig())
 
     height = await client.get_height()
 
     query = hypersync.Query(
         # start from 10k blocks back
         from_block=height-int(1e4),
         # Select the logs we want
@@ -28,31 +28,30 @@
             transaction=[
                 TransactionField.HASH,
                 TransactionField.GAS_USED,
             ]
         ),
     )
 
-    config = hypersync.ParquetConfig(
-        path="data",
-        hex_output=True,
+    config = hypersync.StreamConfig(
+        hex_output=hypersync.HexOutput.PREFIXED,
         column_mapping=ColumnMapping(
             # map value columns to float so we can do calculations with them
             decoded_log={
                 "value": DataType.FLOAT64,
             },
             transaction={
                 TransactionField.GAS_USED: DataType.FLOAT64,
             },
         ),
         # give event signature so client can decode logs into decoded_logs.parquet file
         event_signature="Transfer(address indexed from, address indexed to, uint256 value)",
     )
 
-    await client.create_parquet_folder(query, config)
+    await client.collect_parquet("data", query, config)
 
 def analyze_events():
     # read raw logs
     logs = polars.read_parquet(
         "data/logs.parquet",
     )
```

### Comparing `hypersync-0.6.2/examples/wallet.py` & `hypersync-0.7.0/examples/wallet.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Convert address to topic for filtering. Padds the address with zeroes.
 def address_to_topic(address):
     return "0x000000000000000000000000" + address[2:]
 
 
 async def main():
     # Create hypersync client using the mainnet hypersync endpoint (default)
-    client = hypersync.HypersyncClient()
+    client = hypersync.HypersyncClient(hypersync.ClientConfig())
 
     address_topic_filter = list(map(address_to_topic, addresses))
 
     # The query to run
     query = hypersync.Query(
         from_block=0,
         # The logs we want. We will also automatically get transactions and blocks relating to these logs (the query implicitly joins them).
@@ -84,52 +84,42 @@
                 TransactionField.INPUT,
             ]
 		)
     )
 
     print("Running the query...")
 
-    # Run the query once, the query is automatically paginated so it will return when it reaches some limit (time, response size etc.)
-    # there is a next_block field on the response object so we can set the from_block of our query to this value and continue our query until
-    # res.next_block is equal to res.archive_height or query.to_block in case we specified an end block.
-    res = await client.send_req(query)
+    res = await client.collect(query, hypersync.StreamConfig())
 
     print(f"Ran the query once.  Next block to query is {res.next_block}")
 
-    # read json abi file for erc20
-    with open("./erc20.abi.json", "r") as json_file:
-        abi = json_file.read()
-
-    # Map of contract_address -> abi
-    abis = {}
-
-    # every log we get should be decodable by this abi but we don't know
-    # the specific contract addresses since we are indexing all erc20 transfers.
-    for log in res.data.logs:
-        abis[log.address] = abi
-
-    # Create a decoder with out mapping
-    decoder = hypersync.Decoder(abis)
+    decoder = hypersync.Decoder([
+        "Transfer(address indexed from, address indexed to, uint256 value)"
+    ])
 
     # Decode the log on a background thread so we don't block the event loop.
     # Can also use decoder.decode_logs_sync if it is more convenient.
     decoded_logs = await decoder.decode_logs(res.data.logs)
 
     # Let's count total volume for each address, it is meaningless because of currency differences but good as an example.
     total_erc20_volume = {}
 
     for log in decoded_logs:
+        #skip invalid logs
+        if log is None:
+            continue
+
         # Check if the keys exist in the dictionary, if not, initialize them with 0
-        total_erc20_volume[log.indexed[0]] = total_erc20_volume.get(log.indexed[0], 0)
-        total_erc20_volume[log.indexed[1]] = total_erc20_volume.get(log.indexed[1], 0)
+        total_erc20_volume[log.indexed[0].val] = total_erc20_volume.get(log.indexed[0].val, 0)
+        total_erc20_volume[log.indexed[1].val] = total_erc20_volume.get(log.indexed[1].val, 0)
 
         # We count for both sides but we will filter by our addresses later
         # so we will ignore unnecessary addresses.
-        total_erc20_volume[log.indexed[0]] += log.body[0]
-        total_erc20_volume[log.indexed[1]] += log.body[0]
+        total_erc20_volume[log.indexed[0].val] += log.body[0].val
+        total_erc20_volume[log.indexed[1].val] += log.body[0].val
 
     for address in addresses:
         erc20_volume = total_erc20_volume.get(address, 0)
         print(f"total erc20 transfer voume for address {address} is {erc20_volume}")
 
     total_wei_volume = {}
     for tx in res.data.transactions:
```

### Comparing `hypersync-0.6.2/hypersync/__init__.py` & `hypersync-0.7.0/hypersync/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 from .hypersync import HypersyncClient as _HypersyncClient
 from .hypersync import Decoder as _Decoder
 from typing import Optional, Dict
 from dataclasses import dataclass, asdict
 from strenum import StrEnum
 
 class Decoder:
-    def __init__(self, json_abis: Dict[str, str]):
-        self.inner = _Decoder(json_abis)
+    def __init__(self, signatures: list[str]):
+        self.inner = _Decoder(signatures)
     
+    def enable_checksummed_addresses(self):
+        self.inner.enable_checksummed_addresses()
+
+    def disable_checksummed_addresses(self):
+        self.inner.disable_checksummed_addresses()
+
     async def decode_logs(self, logs: any) -> any:
         return await self.inner.decode_logs(logs)
 
     def decode_logs_sync(self, logs: any) -> any:
         return self.inner.decode_logs_sync(logs)
     
     async def decode_events(self, events: any) -> any:
@@ -72,32 +78,31 @@
     VALUE = 'value'
     V = 'v'
     R = 'r'
     S = 's'
     MAX_PRIORITY_FEE_PER_GAS = 'max_priority_fee_per_gas'
     MAX_FEE_PER_GAS = 'max_fee_per_gas'
     CHAIN_ID = 'chain_id'
+    ACCESS_LIST = 'access_list'
+    MAX_FEE_PER_BLOB_GAS = 'max_fee_per_blob_gas'
+    BLOB_VERSIONED_HASHES = 'blob_versioned_hashes'
     CUMULATIVE_GAS_USED = 'cumulative_gas_used'
     EFFECTIVE_GAS_PRICE = 'effective_gas_price'
     GAS_USED = 'gas_used'
     CONTRACT_ADDRESS = 'contract_address'
     LOGS_BLOOM = 'logs_bloom'
-    TYPE = 'type'
+    KIND = 'type'
     ROOT = 'root'
     STATUS = 'status'
-    SIGHASH = 'sighash'
-    TX_Y_PARITY = 'tx_y_parity'
-    TX_ACCESS_LIST = 'tx_access_list'
-    TX_L1_FEE = 'tx_l1_fee'
-    TX_L1_GAS_PRICE = 'tx_l1_gas_price'
-    TX_L1_GAS_USED = 'tx_l1_gas_used'
-    TX_L1_FEE_SCALAR = 'tx_l1_fee_scalar'
-    TX_GAS_USED_FOR_L1 = 'tx_gas_used_for_l1'
-    MAX_FEE_PER_BLOB_GAS = 'max_fee_per_blob_gas'
-    BLOB_VERSIONED_HASHES = 'blob_versioned_hashes'
+    Y_PARITY = 'y_parity'
+    L1_FEE = 'l1_fee'
+    L1_GAS_PRICE = 'l1_gas_price'
+    L1_GAS_USED = 'l1_gas_used'
+    L1_FEE_SCALAR = 'l1_fee_scalar'
+    GAS_USED_FOR_L1 = 'gas_used_for_l1'
 
 class LogField(StrEnum):
     REMOVED = 'removed'
     LOG_INDEX = 'log_index'
     TRANSACTION_INDEX = 'transaction_index'
     TRANSACTION_HASH = 'transaction_hash'
     BLOCK_HASH = 'block_hash'
@@ -111,47 +116,57 @@
 
 class TraceField(StrEnum):
     FROM = 'from'
     TO = 'to'
     CALL_TYPE = 'call_type'
     GAS = 'gas'
     INPUT = 'input'
+    INIT = 'init'
     VALUE = 'value'
+    AUTHOR = 'author'
     REWARD_TYPE = 'reward_type'
     BLOCK_HASH = 'block_hash'
     BLOCK_NUMBER = 'block_number'
+    ADDRESS = 'address'
+    CODE = 'code'
     GAS_USED = 'gas_used'
     OUTPUT = 'output'
     SUBTRACES = 'subtraces'
     TRACE_ADDRESS = 'trace_address'
     TRANSACTION_HASH = 'transaction_hash'
     TRANSACTION_POSITION = 'transaction_position'
     TYPE = 'type'
     ERROR = 'error'
-    SIGHASH = 'sighash'
+
+class HexOutput(StrEnum):
+    NO_ENCODE = 'NoEncode'
+    PREFIXED = 'Prefixed'
+    NON_PREFIXED = 'NonPrefixed'
 
 @dataclass
 class LogSelection:
     address: Optional[list[str]] = None
     topics: Optional[list[list[str]]] = None
 
 @dataclass
 class TransactionSelection:
     from_: Optional[list[str]] = None
     to: Optional[list[str]] = None
     sighash: Optional[list[str]] = None
     status: Optional[int] = None
+    kind: Optional[list[str]] = None
+    contract_address: Optional[list[str]] = None
 
 @dataclass
 class TraceSelection:
     from_: Optional[list[str]] = None
     to: Optional[list[str]] = None
     call_type: Optional[list[str]] = None
     reward_type: Optional[list[str]] = None
-    type_: Optional[list[str]] = None
+    kind: Optional[list[str]] = None
     sighash: Optional[list[str]] = None
 
 @dataclass
 class FieldSelection:
     block: Optional[list[BlockField]] = None
     transaction: Optional[list[TransactionField]] = None
     log: Optional[list[LogField]] = None
@@ -176,82 +191,115 @@
     block: Optional[Dict[BlockField, DataType]] = None
     transaction: Optional[Dict[TransactionField, DataType]] = None
     log: Optional[Dict[LogField, DataType]] = None
     trace: Optional[Dict[TraceField, DataType]] = None
     decoded_log: Optional[Dict[str, DataType]] = None
 
 @dataclass
-class ParquetConfig:
-    path: str
-    hex_output: Optional[bool] = None
-    batch_size: Optional[int] = None
-    concurrency: Optional[int] = None
-    retry: Optional[bool] = None
+class StreamConfig:
     column_mapping: Optional[ColumnMapping] = None
     event_signature: Optional[str] = None
+    hex_output: Optional[HexOutput] = None
+    batch_size: Optional[int] = None
+    concurrency: Optional[int] = None
+    max_num_blocks: Optional[int] = None
+    max_num_transactions: Optional[int] = None
+    max_num_logs: Optional[int] = None
+    max_num_traces: Optional[int] = None
+
+@dataclass
+class ClientConfig:
+    url: Optional[str] = None
+    bearer_token: Optional[str] = None
+    http_req_timeout_millis: Optional[int] = None
+    max_num_retries: Optional[int] = None
+    retry_backoff_ms: Optional[int] = None
+    retry_base_ms: Optional[int] = None
+    retry_ceiling_ms: Optional[int] = None
 
 class HypersyncClient:
-    def __init__(self, url="https://eth.hypersync.xyz", bearer_token=None, http_req_timeout_millis=None):
-        self.inner = _HypersyncClient({
-            "url": url,
-            "bearer_token": bearer_token,
-            "http_req_timeout_millis": http_req_timeout_millis
-        })
+    def __init__(self, config: ClientConfig):
+        self.inner = _HypersyncClient(asdict(config))
 
     async def get_height(self) -> int:
         return await self.inner.get_height()
+    
+    async def collect(self, query: Query, config: StreamConfig) -> any:
+        return await self.inner.collect(asdict(query), asdict(config))
+    
+    async def collect_events(self, query: Query, config: StreamConfig) -> any:
+        return await self.inner.collect_events(asdict(query), asdict(config))
+    
+    async def collect_arrow(self, query: Query, config: StreamConfig) -> any:
+        return await self.inner.collect_arrow(asdict(query), asdict(config))
+    
+    async def collect_parquet(self, path: str, query: Query, config: StreamConfig) -> None:
+        return await self.inner.collect_parquet(path, asdict(query), asdict(config))
 
-    async def create_parquet_folder(self, query: Query, config: ParquetConfig) -> None:
-        return await self.inner.create_parquet_folder(asdict(query), asdict(config))
+    async def get(self, query: Query) -> any:
+        return await self.inner.get(asdict(query))
+    
+    async def get_events(self, query: Query) -> any:
+        return await self.inner.get_events(asdict(query))
+    
+    async def get_arrow(self, query: Query) -> any:
+        return await self.inner.get_arrow(asdict(query))
+    
+    async def stream(self, query: Query, config: StreamConfig) -> any:
+        return await self.inner.stream(asdict(query), asdict(config))
+    
+    async def stream_events(self, query: Query, config: StreamConfig) -> any:
+        return await self.inner.stream_events(asdict(query), asdict(config))
+    
+    async def stream_arrow(self, query: Query, config: StreamConfig) -> any:
+        return await self.inner.stream_arrow(asdict(query), asdict(config))
 
-    async def send_req(self, query: Query) -> any:
-        return await self.inner.send_req(asdict(query))
+def preset_query_blocks_and_transactions(from_block: int, to_block: Optional[int] = None) -> Query:
+    return Query(
+        from_block=from_block,
+        to_block=to_block,
+        include_all_blocks=True,
+        transactions=[TransactionSelection()],
+        field_selection=FieldSelection(
+            block=[e.value for e in BlockField],
+            transaction=[e.value for e in TransactionField],
+        )
+    )
 
-    async def send_events_req(self, query: Query) -> any:
-        return await self.inner.send_events_req(asdict(query))
+def preset_query_blocks_and_transaction_hashes(from_block: int, to_block: Optional[int] = None) -> Query:
+    return Query(
+        from_block=from_block,
+        to_block=to_block,
+        include_all_blocks=True,
+        transactions=[TransactionSelection()],
+        field_selection=FieldSelection(
+            block=[e.value for e in BlockField],
+            transaction=[
+                TransactionField.BLOCK_HASH,
+                TransactionField.BLOCK_NUMBER,
+                TransactionField.HASH,
+            ],
+        )
+    )
 
-    async def send_req_arrow(self, query: Query) -> any:
-        return await self.inner.send_req_arrow(asdict(query))
-    
-    def preset_query_blocks_and_transactions(self, from_block: int, to_block: Optional[int]) -> Query:
-        query = self.inner.preset_query_blocks_and_transactions(from_block, to_block)
-        return dict_to_query(query)
-    
-    def preset_query_blocks_and_transaction_hashes(self, from_block: int, to_block: Optional[int]) -> Query:
-        query = self.inner.preset_query_blocks_and_transaction_hashes(from_block, to_block)
-        return dict_to_query(query)
-    
-    def preset_query_logs(self, contract_address: str, from_block: int, to_block: Optional[int]) -> Query:
-        query = self.inner.preset_query_logs(contract_address, from_block, to_block)
-        return dict_to_query(query)
-    
-    def preset_query_logs_of_event(self, contract_address: str, topic0: str, from_block: int, to_block: Optional[int]) -> Query:
-        query = self.inner.preset_query_logs_of_event(contract_address, topic0, from_block, to_block)
-        return dict_to_query(query)
-
-# helper function for converting a Query object from the rust side interpreted as a dict into a 
-# dataclass Query
-def dict_to_query(data: dict) -> Query:
-    logs = [LogSelection(**log) for log in data.get('logs', [])] if 'logs' in data else None
-    transactions = [TransactionSelection(**txn) for txn in data.get('transactions', [])] if 'transactions' in data else None
-    traces = [TraceSelection(**trace) for trace in data.get('traces', [])] if 'traces' in data else None
-    
-    field_selection = FieldSelection(
-        block=[BlockField(block) for block in data['field_selection'].get('block', [])] if 'block' in data['field_selection'] else None,
-        transaction=[TransactionField(txn) for txn in data['field_selection'].get('transaction', [])] if 'transaction' in data['field_selection'] else None,
-        log=[LogField(log) for log in data['field_selection'].get('log', [])] if 'log' in data['field_selection'] else None,
-        trace=[TraceField(trace) for trace in data['field_selection'].get('trace', [])] if 'trace' in data['field_selection'] else None,
+def preset_query_logs(address: str, from_block: int, to_block: Optional[int] = None) -> Query:
+    return Query(
+        from_block=from_block,
+        to_block=to_block,
+        logs=[LogSelection(address=[address])],
+        field_selection=FieldSelection(
+            log=[e.value for e in LogField]
+        )
     )
-    
+
+def preset_query_logs_of_event(address: str, topic0: str, from_block: int, to_block: Optional[int] = None) -> Query:
     return Query(
-        from_block=data['from_block'],
-        to_block=data.get('to_block'),
-        logs=logs,
-        transactions=transactions,
-        traces=traces,
-        include_all_blocks=data.get('include_all_blocks'),
-        max_num_blocks=data.get('max_num_blocks'),
-        max_num_transactions=data.get('max_num_transactions'),
-        max_num_logs=data.get('max_num_logs'),
-        max_num_traces=data.get('max_num_traces'),
-        field_selection=field_selection,
-    )
+        from_block=from_block,
+        to_block=to_block,
+        logs=[LogSelection(
+            address=[address],
+            topics=[[topic0]]
+        )],
+        field_selection=FieldSelection(
+            log=[e.value for e in LogField]
+        )
+    )
```

### Comparing `hypersync-0.6.2/src/config.rs` & `hypersync-0.7.0/src/config.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,78 @@
-use std::collections::BTreeMap;
+use std::collections::HashMap;
 
 use anyhow::{Context, Result};
-use serde::Serialize;
+use serde::{Deserialize, Serialize};
 
-#[derive(Default, Clone, Serialize, dict_derive::FromPyObject)]
-pub struct ParquetConfig {
-    /// Path to write parquet files to
-    pub path: String,
+#[derive(
+    Default, Clone, Serialize, Deserialize, dict_derive::FromPyObject, dict_derive::IntoPyObject,
+)]
+pub struct StreamConfig {
     #[serde(skip_serializing_if = "Option::is_none")]
-    /// Convert binary output columns to hex
-    pub hex_output: Option<bool>,
+    pub column_mapping: Option<ColumnMapping>,
+    #[serde(skip_serializing_if = "Option::is_none")]
+    pub event_signature: Option<String>,
+    #[serde(skip_serializing_if = "Option::is_none")]
+    pub hex_output: Option<String>,
     #[serde(skip_serializing_if = "Option::is_none")]
-    /// Block range size to use when making individual requests.
     pub batch_size: Option<i64>,
     #[serde(skip_serializing_if = "Option::is_none")]
-    /// Controls the number of concurrent requests made to hypersync server.
     pub concurrency: Option<i64>,
     #[serde(skip_serializing_if = "Option::is_none")]
-    /// Requests are retried forever internally if this param is set to true.
-    pub retry: Option<bool>,
+    pub max_num_blocks: Option<i64>,
     #[serde(skip_serializing_if = "Option::is_none")]
-    /// Define type mapping for output columns
-    pub column_mapping: Option<ColumnMapping>,
+    pub max_num_transactions: Option<i64>,
     #[serde(skip_serializing_if = "Option::is_none")]
-    /// Define type mapping for output columns
-    pub event_signature: Option<String>,
+    pub max_num_logs: Option<i64>,
+    #[serde(skip_serializing_if = "Option::is_none")]
+    pub max_num_traces: Option<i64>,
 }
 
-#[derive(Default, Clone, Serialize, dict_derive::FromPyObject)]
+#[derive(
+    Default, Clone, Serialize, Deserialize, dict_derive::FromPyObject, dict_derive::IntoPyObject,
+)]
 pub struct ColumnMapping {
     #[serde(skip_serializing_if = "Option::is_none")]
-    pub block: Option<BTreeMap<String, String>>,
+    pub block: Option<HashMap<String, String>>,
     #[serde(skip_serializing_if = "Option::is_none")]
-    pub transaction: Option<BTreeMap<String, String>>,
+    pub transaction: Option<HashMap<String, String>>,
     #[serde(skip_serializing_if = "Option::is_none")]
-    pub log: Option<BTreeMap<String, String>>,
+    pub log: Option<HashMap<String, String>>,
     #[serde(skip_serializing_if = "Option::is_none")]
-    pub trace: Option<BTreeMap<String, String>>,
+    pub trace: Option<HashMap<String, String>>,
     #[serde(skip_serializing_if = "Option::is_none")]
-    pub decoded_log: Option<BTreeMap<String, String>>,
+    pub decoded_log: Option<HashMap<String, String>>,
 }
 
-impl ParquetConfig {
-    pub fn try_convert(&self) -> Result<skar_client::ParquetConfig> {
+impl StreamConfig {
+    pub fn try_convert(&self) -> Result<hypersync_client::StreamConfig> {
         let json = serde_json::to_vec(self).context("serialize to json")?;
         serde_json::from_slice(&json).context("parse json")
     }
 }
 
-#[derive(Default, Clone, Serialize, dict_derive::FromPyObject)]
-pub struct Config {
-    /// Url of the source hypersync instance
-    pub url: String,
-    /// Optional bearer_token to put into http requests made to source hypersync instance
+#[derive(
+    Default, Clone, Serialize, Deserialize, dict_derive::FromPyObject, dict_derive::IntoPyObject,
+)]
+pub struct ClientConfig {
+    #[serde(skip_serializing_if = "Option::is_none")]
+    pub url: Option<String>,
     #[serde(skip_serializing_if = "Option::is_none")]
     pub bearer_token: Option<String>,
-    /// Timout treshold for a single http request in milliseconds, default is 30 seconds (30_000ms)
     #[serde(skip_serializing_if = "Option::is_none")]
     pub http_req_timeout_millis: Option<i64>,
+    #[serde(skip_serializing_if = "Option::is_none")]
+    pub max_num_retries: Option<i64>,
+    #[serde(skip_serializing_if = "Option::is_none")]
+    pub retry_backoff_ms: Option<i64>,
+    #[serde(skip_serializing_if = "Option::is_none")]
+    pub retry_base_ms: Option<i64>,
+    #[serde(skip_serializing_if = "Option::is_none")]
+    pub retry_ceiling_ms: Option<i64>,
 }
 
-impl Config {
-    pub fn try_convert(&self) -> Result<skar_client::Config> {
+impl ClientConfig {
+    pub fn try_convert(&self) -> Result<hypersync_client::ClientConfig> {
         let json = serde_json::to_vec(self).context("serialize to json")?;
         serde_json::from_slice(&json).context("parse json")
     }
 }
```

### Comparing `hypersync-0.6.2/src/query.rs` & `hypersync-0.7.0/src/query.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 use anyhow::{Context, Result};
+use hypersync_client::net_types;
 use serde::{Deserialize, Serialize};
 
 #[derive(
     Default, Clone, Serialize, Deserialize, dict_derive::FromPyObject, dict_derive::IntoPyObject,
 )]
 pub struct TraceSelection {
     #[serde(skip_serializing_if = "Option::is_none")]
@@ -12,54 +13,47 @@
     pub to: Option<Vec<String>>,
     #[serde(skip_serializing_if = "Option::is_none")]
     pub call_type: Option<Vec<String>>,
     #[serde(skip_serializing_if = "Option::is_none")]
     pub reward_type: Option<Vec<String>>,
     #[serde(skip_serializing_if = "Option::is_none")]
     #[serde(rename = "type")]
-    pub type_: Option<Vec<String>>,
+    pub kind: Option<Vec<String>>,
     #[serde(skip_serializing_if = "Option::is_none")]
     pub sighash: Option<Vec<String>>,
 }
 
 #[derive(
     Default, Clone, Serialize, Deserialize, dict_derive::FromPyObject, dict_derive::IntoPyObject,
 )]
 pub struct LogSelection {
-    /// Address of the contract, any logs that has any of these addresses will be returned.
-    /// Empty means match all.
     #[serde(skip_serializing_if = "Option::is_none")]
     pub address: Option<Vec<String>>,
-    /// Topics to match, each member of the top level array is another array, if the nth topic matches any
-    ///  topic specified in topics[n] the log will be returned. Empty means match all.
     #[serde(skip_serializing_if = "Option::is_none")]
     pub topics: Option<Vec<Vec<String>>>,
 }
 
 #[derive(
     Default, Clone, Serialize, Deserialize, dict_derive::FromPyObject, dict_derive::IntoPyObject,
 )]
 pub struct TransactionSelection {
-    /// Address the transaction should originate from. If transaction.from matches any of these, the transaction
-    ///  will be returned. Keep in mind that this has an and relationship with to filter, so each transaction should
-    ///  match both of them. Empty means match all.
     #[serde(skip_serializing_if = "Option::is_none")]
     #[serde(rename = "from")]
     pub from_: Option<Vec<String>>,
-    /// Address the transaction should go to. If transaction.to matches any of these, the transaction will
-    ///  be returned. Keep in mind that this has an and relationship with from filter, so each transaction should
-    ///  match both of them. Empty means match all.
     #[serde(skip_serializing_if = "Option::is_none")]
     pub to: Option<Vec<String>>,
-    /// If first 4 bytes of transaction input matches any of these, transaction will be returned. Empty means match all.
     #[serde(skip_serializing_if = "Option::is_none")]
     pub sighash: Option<Vec<String>>,
-    /// If tx.status matches this it will be returned.
     #[serde(skip_serializing_if = "Option::is_none")]
-    pub status: Option<i64>,
+    pub status: Option<u64>,
+    #[serde(skip_serializing_if = "Option::is_none")]
+    #[serde(rename = "type")]
+    pub kind: Option<Vec<String>>,
+    #[serde(skip_serializing_if = "Option::is_none")]
+    pub contract_address: Option<Vec<String>>,
 }
 
 #[derive(
     Default, Clone, Serialize, Deserialize, dict_derive::FromPyObject, dict_derive::IntoPyObject,
 )]
 pub struct FieldSelection {
     #[serde(skip_serializing_if = "Option::is_none")]
@@ -73,24 +67,24 @@
 }
 
 #[derive(
     Default, Clone, Serialize, Deserialize, dict_derive::FromPyObject, dict_derive::IntoPyObject,
 )]
 pub struct Query {
     /// The block to start the query from
-    pub from_block: i64,
+    pub from_block: u64,
     /// The block to end the query at. If not specified, the query will go until the
     ///  end of data. Exclusive, the returned range will be [from_block..to_block).
     ///
     /// The query will return before it reaches this target block if it hits the time limit
     ///  configured on the server. The user should continue their query by putting the
     ///  next_block field in the response into from_block field of their next query. This implements
     ///  pagination.
     #[serde(skip_serializing_if = "Option::is_none")]
-    pub to_block: Option<i64>,
+    pub to_block: Option<u64>,
     /// List of log selections, these have an or relationship between them, so the query will return logs
     /// that match any of these selections.
     #[serde(skip_serializing_if = "Option::is_none")]
     pub logs: Option<Vec<LogSelection>>,
     /// List of transaction selections, the query will return transactions that match any of these selections and
     ///  it will return transactions that are related to the returned logs.
     #[serde(skip_serializing_if = "Option::is_none")]
@@ -106,37 +100,37 @@
     pub include_all_blocks: Option<bool>,
     /// Field selection. The user can select which fields they are interested in, requesting less fields will improve
     ///  query execution time and reduce the payload size so the user should always use a minimal number of fields.
     pub field_selection: FieldSelection,
     /// Maximum number of blocks that should be returned, the server might return more blocks than this number but
     ///  it won't overshoot by too much.
     #[serde(skip_serializing_if = "Option::is_none")]
-    pub max_num_blocks: Option<i64>,
+    pub max_num_blocks: Option<u64>,
     /// Maximum number of transactions that should be returned, the server might return more transactions than this number but
     ///  it won't overshoot by too much.
     #[serde(skip_serializing_if = "Option::is_none")]
-    pub max_num_transactions: Option<i64>,
+    pub max_num_transactions: Option<u64>,
     /// Maximum number of logs that should be returned, the server might return more logs than this number but
     ///  it won't overshoot by too much.
     #[serde(skip_serializing_if = "Option::is_none")]
-    pub max_num_logs: Option<i64>,
+    pub max_num_logs: Option<u64>,
     /// Maximum number of traces that should be returned, the server might return more traces than this number but
     ///  it won't overshoot by too much.
     #[serde(skip_serializing_if = "Option::is_none")]
-    pub max_num_traces: Option<i64>,
+    pub max_num_traces: Option<u64>,
 }
 
 impl Query {
-    pub fn try_convert(&self) -> Result<skar_net_types::Query> {
+    pub fn try_convert(&self) -> Result<net_types::Query> {
         let json = serde_json::to_vec(self).context("serialize to json")?;
         serde_json::from_slice(&json).context("parse json")
     }
 }
 
-impl TryFrom<skar_net_types::Query> for Query {
+impl TryFrom<net_types::Query> for Query {
     type Error = anyhow::Error;
 
-    fn try_from(skar_query: skar_net_types::Query) -> Result<Self> {
+    fn try_from(skar_query: net_types::Query) -> Result<Self> {
         let json = serde_json::to_vec(&skar_query).context("serialize query to json")?;
         serde_json::from_slice(&json).context("parse json")
     }
 }
```

### Comparing `hypersync-0.6.2/test.py` & `hypersync-0.7.0/test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import hypersync
 import asyncio
 import time
-from hypersync import DataType, BlockField, TransactionField, LogField, TraceField
+from hypersync import DataType, BlockField, TransactionField, LogField, TraceField, HexOutput
 
 # for benchmarking times.  Will run the function this many times and take the
 # average
 NUM_BENCHMARK_RUNS = 1
 
 # The address we want to get all ERC20 transfers and transactions for
 ADDR = "1e037f97d730Cc881e77F01E409D828b0bb14de0"
@@ -67,24 +67,22 @@
             TraceField.CALL_TYPE,
             TraceField.TRANSACTION_POSITION,
         ],
     )
 )
 
 async def test_create_parquet_folder():
-    client = hypersync.HypersyncClient()
+    client = hypersync.HypersyncClient(hypersync.ClientConfig())
     total_time = 0
     for _ in range(NUM_BENCHMARK_RUNS):
         start_time = time.time()
 
-        await client.create_parquet_folder(
-            QUERY, hypersync.ParquetConfig(
-                path="data",
-                retry=True,
-                hex_output=True,
+        await client.collect_parquet(
+            "data", QUERY, hypersync.StreamConfig(
+                hex_output=HexOutput.PREFIXED,
                 column_mapping=hypersync.ColumnMapping(
                     trace={
                         TraceField.TRANSACTION_POSITION: DataType.INT32,
                     },
                     transaction={
                         TransactionField.BLOCK_NUMBER: DataType.INT64,
                         TransactionField.VALUE: DataType.FLOAT32,
@@ -94,146 +92,130 @@
                     },
                 ),
                 event_signature="Transfer(address indexed from, address indexed to, uint256 value)",
             )
         )
         execution_time = (time.time() - start_time) * 1000
         total_time += execution_time
-    avg_time = total_time / NUM_BENCHMARK_RUNS
     print(f"create_parquet_folder time: {format(execution_time, '.9f')}ms")
 
 async def test_send_req():
-    client = hypersync.HypersyncClient()
+    client = hypersync.HypersyncClient(hypersync.ClientConfig())
     total_time = 0
     for _ in range(NUM_BENCHMARK_RUNS):
         start_time = time.time()
-        res = await client.send_req(QUERY)
+        await client.get(QUERY)
         execution_time = (time.time() - start_time) * 1000
         total_time += execution_time
-    avg_time = total_time / NUM_BENCHMARK_RUNS
     print(f"send_req time: {format(execution_time, '.9f')}ms")
 
-
 async def test_send_req_arrow():
-    client = hypersync.HypersyncClient()
+    client = hypersync.HypersyncClient(hypersync.ClientConfig())
     import pyarrow
     total_time = 0
     for _ in range(NUM_BENCHMARK_RUNS):
         start_time = time.time()
-        res = await client.send_req_arrow(QUERY)
+        res = await client.get_arrow(QUERY)
         execution_time = (time.time() - start_time) * 1000
         assert(type(res.data.blocks) == pyarrow.lib.Table)
         assert(res.data.blocks._is_initialized())
         assert(type(res.data.transactions) == pyarrow.lib.Table)
         assert(res.data.transactions._is_initialized())
         assert(type(res.data.logs) == pyarrow.lib.Table)
         assert(res.data.logs._is_initialized())
         total_time += execution_time
-    avg_time = total_time / NUM_BENCHMARK_RUNS
     print(f"send_req_arrow time: {format(execution_time, '.9f')}ms")
 
 
 async def test_send_events_req():
-    client = hypersync.HypersyncClient()
+    client = hypersync.HypersyncClient(hypersync.ClientConfig())
     total_time = 0
     for _ in range(NUM_BENCHMARK_RUNS):
         start_time = time.time()
-        res = await client.send_events_req(QUERY)
+        await client.get_events(QUERY)
         execution_time = (time.time() - start_time) * 1000
         total_time += execution_time
-    avg_time = total_time / NUM_BENCHMARK_RUNS
     print(f"send_events_req time: {format(execution_time, '.9f')}ms")
 
-
 async def test_get_height():
-    client = hypersync.HypersyncClient()
+    client = hypersync.HypersyncClient(hypersync.ClientConfig())
     total_time = 0
     for _ in range(NUM_BENCHMARK_RUNS):
         start_time = time.time()
-        height = await client.get_height()
+        await client.get_height()
         execution_time = (time.time() - start_time) * 1000
         total_time += execution_time
-    avg_time = total_time / NUM_BENCHMARK_RUNS
     print(f"get_height time: {format(execution_time, '.9f')}ms")
 
 
 async def test_decode_logs():
-    client = hypersync.HypersyncClient()
-    res = await client.send_req(QUERY)
-    with open("./erc20.abi.json", "r") as json_file:
-        json = json_file.read()
-    abis = {}
-    for log in res.data.logs:
-        abis[log.address] = json
-    decoder = hypersync.Decoder(json_abis=abis)
+    client = hypersync.HypersyncClient(hypersync.ClientConfig())
+    res = await client.get(QUERY)
+    decoder = hypersync.Decoder([
+        "Transfer(address indexed from, address indexed to, uint256 value)"
+    ])
     total_time = 0
     for _ in range(NUM_BENCHMARK_RUNS):
         start_time = time.time()
-        decoded_logs = decoder.decode_logs_sync(res.data.logs)
+        decoder.decode_logs_sync(res.data.logs)
         execution_time = (time.time() - start_time) * 1000
         total_time += execution_time
-    avg_time = total_time / NUM_BENCHMARK_RUNS
     print(f"decode_logs time: {format(execution_time, '.9f')}ms")
 
-
 async def test_decode_events():
-    client = hypersync.HypersyncClient()
-    res = await client.send_events_req(QUERY)
-    with open("./erc20.abi.json", "r") as json_file:
-        json = json_file.read()
-    abis = {}
-    for event in res.events:
-        abis[event.log.address] = json
-    decoder = hypersync.Decoder(abis)
+    client = hypersync.HypersyncClient(hypersync.ClientConfig())
+    res = await client.get_events(QUERY)
+    decoder = hypersync.Decoder([
+        "Transfer(address indexed from, address indexed to, uint256 value)"
+    ])
     total_time = 0
     for _ in range(NUM_BENCHMARK_RUNS):
         start_time = time.time()
-        decoded_events = decoder.decode_events_sync(res.events)
+        decoder.decode_events_sync(res.data)
         execution_time = (time.time() - start_time) * 1000
         total_time += execution_time
-    avg_time = total_time / NUM_BENCHMARK_RUNS
     print(f"decode_events time: {format(execution_time, '.9f')}ms")
 
 async def test_preset_query_blocks_and_transactions():
     start_time = time.time()
-    client = hypersync.HypersyncClient()
-    query = client.preset_query_blocks_and_transactions(17_000_000, 17_000_010)
-    res = await client.send_req(query)
+    client = hypersync.HypersyncClient(hypersync.ClientConfig())
+    query = hypersync.preset_query_blocks_and_transactions(17_000_000, 17_000_010)
+    res = await client.get(query)
     execution_time = (time.time() - start_time) * 1000
     assert(len(res.data.blocks) == 10)
     assert(len(res.data.transactions) > 1)
     print(f"preset_query_blocks_and_transactions time: {format(execution_time, '.9f')}ms")
 
 async def test_preset_query_blocks_and_transaction_hashes():
     start_time = time.time()
-    client = hypersync.HypersyncClient()
-    query = client.preset_query_blocks_and_transaction_hashes(17_000_000, 17_000_010)
-    res = await client.send_req(query)
+    client = hypersync.HypersyncClient(hypersync.ClientConfig())
+    query = hypersync.preset_query_blocks_and_transaction_hashes(17_000_000, 17_000_010)
+    res = await client.get(query)
     execution_time = (time.time() - start_time) * 1000
     assert(len(res.data.blocks) == 10)
     assert(len(res.data.transactions) > 1)
     print(f"preset_query_blocks_and_transaction_hashes time: {format(execution_time, '.9f')}ms")
 
 async def test_preset_query_logs():
     start_time = time.time()
-    client = hypersync.HypersyncClient()
+    client = hypersync.HypersyncClient(hypersync.ClientConfig())
     contract_address = "0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48"
-    query = client.preset_query_logs(contract_address, 17_000_000, 17_000_010)
-    res = await client.send_req(query)
+    query = hypersync.preset_query_logs(contract_address, 17_000_000, 17_000_010)
+    res = await client.get(query)
     execution_time = (time.time() - start_time) * 1000
     assert(len(res.data.logs) > 1)
     print(f"preset_query_logs time: {format(execution_time, '.9f')}ms")
 
 async def test_preset_query_logs_of_event():
     start_time = time.time()
-    client = hypersync.HypersyncClient()
+    client = hypersync.HypersyncClient(hypersync.ClientConfig())
     contract_address = "0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48"
     topic0 = "0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef"
-    query = client.preset_query_logs_of_event(contract_address, topic0, 17_000_000, 17_000_010)
-    res = await client.send_req(query)
+    query = hypersync.preset_query_logs_of_event(contract_address, topic0, 17_000_000, 17_000_010)
+    res = await client.get(query)
     execution_time = (time.time() - start_time) * 1000
     assert(len(res.data.logs) > 1)
     print(f"preset_query_logs_of_event time: {format(execution_time, '.9f')}ms")
 
 
 async def main():
     print("hypersync-client-python")
```

### Comparing `hypersync-0.6.2/Cargo.lock` & `hypersync-0.7.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -58,46 +58,46 @@
 name = "allocator-api2"
 version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c6cb57a04249c6480766f7f7cef5467412af1490f8d1e243141daddada3264f"
 
 [[package]]
 name = "alloy-dyn-abi"
-version = "0.7.2"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "545885d9b0b2c30fd344ae291439b4bfe59e48dd62fbc862f8503d98088967dc"
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
- "winnow 0.6.7",
+ "winnow 0.6.8",
 ]
 
 [[package]]
 name = "alloy-json-abi"
-version = "0.7.2"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "786689872ec4e7d354810ab0dffd48bb40b838c047522eb031cbd47d15634849"
+checksum = "7e30946aa6173020259055a44971f5cf40a7d76c931d209caeb51b333263df4f"
 dependencies = [
  "alloy-primitives",
  "alloy-sol-type-parser",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "alloy-primitives"
-version = "0.7.2"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "525448f6afc1b70dd0f9d0a8145631bf2f5e434678ab23ab18409ca264cae6b3"
+checksum = "db8aa973e647ec336810a9356af8aea787249c9d00b1525359f3db29a68d231b"
 dependencies = [
  "alloy-rlp",
  "bytes",
  "cfg-if",
  "const-hex",
  "derive_more",
  "hex-literal",
@@ -109,69 +109,83 @@
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
-version = "0.7.2"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89c80a2cb97e7aa48611cbb63950336f9824a174cdf670527cc6465078a26ea1"
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
  "alloy-sol-macro-input",
  "const-hex",
  "heck 0.4.1",
  "indexmap",
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.66",
  "syn-solidity",
  "tiny-keccak",
 ]
 
 [[package]]
 name = "alloy-sol-macro-input"
-version = "0.7.2"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c58894b58ac50979eeac6249661991ac40b9d541830d9a725f7714cc9ef08c23"
+checksum = "32c8da04c1343871fb6ce5a489218f9c85323c8340a36e9106b5fc98d4dd59d5"
 dependencies = [
  "const-hex",
  "dunce",
  "heck 0.5.0",
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.66",
  "syn-solidity",
 ]
 
 [[package]]
 name = "alloy-sol-type-parser"
-version = "0.7.2"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7da8e71ea68e780cc203919e03f69f59e7afe92d2696fb1dcb6662f61e4031b6"
+checksum = "368cae4dc052cad1d8f72eb2ae0c38027116933eeb49213c200a9e9875f208d7"
 dependencies = [
- "winnow 0.6.7",
+ "winnow 0.6.8",
 ]
 
 [[package]]
 name = "alloy-sol-types"
-version = "0.7.2"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "399287f68d1081ed8b1f4903c49687658b95b142207d7cb4ae2f4813915343ef"
+checksum = "40a64d2d2395c1ac636b62419a7b17ec39031d6b2367e66e9acbf566e6055e9c"
 dependencies = [
  "alloy-primitives",
  "alloy-sol-macro",
  "const-hex",
  "serde",
 ]
 
@@ -222,17 +236,17 @@
 dependencies = [
  "anstyle",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.82"
+version = "1.0.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
+checksum = "b3d1d046238990b9cf5bcde22a3fb3584ee5cf65fb2765f454ed428c7a0063da"
 
 [[package]]
 name = "ark-ff"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6b3235cc41ee7a12aaaf2c575a2ad7b46713a8a50bda2fc3b003a04845c05dd6"
 dependencies = [
@@ -256,15 +270,15 @@
 dependencies = [
  "ark-ff-asm 0.4.2",
  "ark-ff-macros 0.4.2",
  "ark-serialize 0.4.2",
  "ark-std 0.4.0",
  "derivative",
  "digest 0.10.7",
- "itertools 0.10.5",
+ "itertools",
  "num-bigint",
  "num-traits",
  "paste",
  "rustc_version 0.4.0",
  "zeroize",
 ]
 
@@ -384,26 +398,26 @@
 name = "async-stream-impl"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "16e62a023e7c117e27523144c5d2459f4397fcc3cab0085af8e2224f643a0193"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "async-trait"
 version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "atoi_simd"
 version = "0.15.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ae037714f313c1353189ead58ef9eec30a8e8dc101b2622d461418fd59e28a9"
@@ -412,15 +426,15 @@
 name = "auto_impl"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c87f3f15e7794432337fc718554eaa4dc8f04c9677a950ffe366f20a162ae42"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
@@ -461,14 +475,23 @@
 [[package]]
 name = "base64ct"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8c3c1a368f70d6cf7302d78f8f7093da241fb8e8807c05cc9e51a125895a6d5b"
 
 [[package]]
+name = "bincode"
+version = "1.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
+dependencies = [
+ "serde",
+]
+
+[[package]]
 name = "bit-set"
 version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0700ddab506f33b20a03b13996eccd309a48e5ff77d0d95926aa0210fb4e95f1"
 dependencies = [
  "bit-vec",
 ]
@@ -537,30 +560,30 @@
 name = "byte-slice-cast"
 version = "1.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c3ac9f8b63eca6fd385229b3675f6cc0dc5c8a5c8a54a59d4f52ffd670d87b0c"
 
 [[package]]
 name = "bytemuck"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d6d68c57235a3a081186990eca2867354726650f42f7516ca50c28d6281fd15"
+checksum = "78834c15cb5d5efe3452d58b1e8ba890dd62d21907f867f383358198e56ebca5"
 dependencies = [
  "bytemuck_derive",
 ]
 
 [[package]]
 name = "bytemuck_derive"
-version = "1.6.0"
+version = "1.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4da9a32f3fed317401fa3c862968128267c3106685286e15d5aaa3d7389c2f60"
+checksum = "369cfaf2a5bed5d8f8202073b2e093c9f508251de1551a0deb4253e4c7d80909"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
@@ -572,17 +595,17 @@
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "capnp"
-version = "0.19.3"
+version = "0.19.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b11832e6fb7a695c4a63cc42bd97bd2cda7165cd850caf5aff9a3d0e617720ed"
+checksum = "3aed85272154b3c0bfda873c40395f13adcfbc89696bf639a512291077f8cd17"
 dependencies = [
  "embedded-io",
 ]
 
 [[package]]
 name = "capnpc"
 version = "0.19.0"
@@ -590,17 +613,17 @@
 checksum = "c75ba30e0f08582d53c2f3710cf4bb65ff562614b1ba86906d7391adffe189ec"
 dependencies = [
  "capnp",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.96"
+version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "065a29261d53ba54260972629f9ca6bffa69bac13cd1fed61420f7fa68b9f8bd"
+checksum = "41c270e7540d725e65ac7f1b212ac8ce349719624d7bcff99f8e2e488e8cf03f"
 dependencies = [
  "jobserver",
  "libc",
  "once_cell",
 ]
 
 [[package]]
@@ -622,17 +645,17 @@
 name = "colorchoice"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b6a852b24ab71dffc585bcb46eaf7959d175cb865a7152e35b348d1b2960422"
 
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
@@ -656,17 +679,17 @@
 checksum = "53fe5e26ff1b7aef8bca9c6080520cfb8d9333c7568e1829cef191a9723e5504"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
-version = "1.4.0"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
+checksum = "a97769d94ddab943e4510d138150169a2758b5ef3eb191a9ee688de3e23ef7b3"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crossbeam-deque"
 version = "0.8.5"
@@ -684,17 +707,17 @@
 checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.19"
+version = "0.8.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+checksum = "22ec99545bb0ed0ea7bb9b8e1e9122ea386ff8a48c0922e43f36d45ab09e0e80"
 
 [[package]]
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
@@ -810,17 +833,17 @@
  "rfc6979",
  "signature",
  "spki",
 ]
 
 [[package]]
 name = "either"
-version = "1.11.0"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
+checksum = "3dca9240753cf90908d7e4aac30f630662b02aebaa1b58a3cadabdb23385b58b"
 
 [[package]]
 name = "elliptic-curve"
 version = "0.13.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b5e6043086bf7973472e0c7dff2142ea0b680d30e18d9cc40f267efbf222bd47"
 dependencies = [
@@ -870,17 +893,17 @@
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
 name = "ethnum"
@@ -1043,15 +1066,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -1089,17 +1112,17 @@
  "typenum",
  "version_check",
  "zeroize",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.14"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
@@ -1254,17 +1277,17 @@
  "tokio",
  "tokio-rustls",
  "tower-service",
 ]
 
 [[package]]
 name = "hyper-util"
-version = "0.1.3"
+version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca38ef113da30126bbff9cd1705f9273e15d45498615d138b0c20279ac7a76aa"
+checksum = "3d8d52be92d09acc2e01dddb7fde3ad983fc6489c7db4837e605bc3fca4cb63e"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-util",
  "http",
  "http-body",
  "hyper",
@@ -1274,37 +1297,107 @@
  "tower",
  "tower-service",
  "tracing",
 ]
 
 [[package]]
 name = "hypersync"
-version = "0.6.2"
+version = "0.7.0"
 dependencies = [
  "alloy-dyn-abi",
  "alloy-json-abi",
  "alloy-primitives",
  "anyhow",
  "dict_derive",
  "env_logger",
  "faster-hex",
- "itertools 0.12.1",
+ "hypersync-client",
  "polars-arrow",
  "prefix-hex",
  "pyo3",
  "pyo3-asyncio",
+ "ruint",
  "serde",
  "serde_json",
- "skar-client",
- "skar-format",
- "skar-net-types",
  "tokio",
 ]
 
 [[package]]
+name = "hypersync-client"
+version = "0.6.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5425c4365cd25e4ab38fb7bd1934b412a7ab0cbab9aa0b9d6843978ee0dad2d3"
+dependencies = [
+ "alloy-dyn-abi",
+ "alloy-json-abi",
+ "anyhow",
+ "arrayvec",
+ "bincode",
+ "capnp",
+ "faster-hex",
+ "fastrange-rs",
+ "futures",
+ "hypersync-format",
+ "hypersync-net-types",
+ "hypersync-schema",
+ "log",
+ "nohash-hasher",
+ "num_cpus",
+ "polars-arrow",
+ "polars-parquet",
+ "rand",
+ "rayon",
+ "reqwest",
+ "ruint",
+ "serde",
+ "serde_json",
+ "tokio",
+ "tokio-util",
+ "url",
+ "xxhash-rust",
+]
+
+[[package]]
+name = "hypersync-format"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f6adfb41a077e57a9f90b351479cdb3cf6baff41cb58662a781eaee755dd4176"
+dependencies = [
+ "alloy-primitives",
+ "arrayvec",
+ "derive_more",
+ "faster-hex",
+ "serde",
+ "thiserror",
+]
+
+[[package]]
+name = "hypersync-net-types"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fb637eda1279334f02f330d4d32bcd243f51d6463b8dd12e23c4e489926c9dcb"
+dependencies = [
+ "arrayvec",
+ "capnp",
+ "capnpc",
+ "hypersync-format",
+ "serde",
+]
+
+[[package]]
+name = "hypersync-schema"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5d6f4349ba69d61a80349f5aa16844abd2accdaa6002ec78f14e77f052988b6f"
+dependencies = [
+ "anyhow",
+ "polars-arrow",
+]
+
+[[package]]
 name = "idna"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "634d9b1461af396cad843f47fdba5597a4f9e6ddd4bfb6ff5d85028c25cb12f6"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
@@ -1364,23 +1457,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
-name = "itertools"
-version = "0.12.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
-dependencies = [
- "either",
-]
-
-[[package]]
 name = "itoa"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jobserver"
@@ -1411,45 +1495,45 @@
  "elliptic-curve",
  "once_cell",
  "sha2",
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
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.154"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
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
 version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
@@ -1502,17 +1586,17 @@
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
@@ -1543,20 +1627,25 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
  "target-features",
 ]
 
 [[package]]
+name = "nohash-hasher"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2bf50223579dc7cdcfb3bfcacf7069ff68243f8c363f62ffa99cf000a6b9c451"
+
+[[package]]
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
 name = "num-integer"
 version = "0.1.46"
@@ -1599,43 +1688,43 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
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
  "proc-macro-crate",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "parking_lot"
-version = "0.12.2"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
+checksum = "f1bf18183cf54e8d6059647fc3063646a1801cf30896933ec2311622cc4b9a27"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
@@ -1658,17 +1747,17 @@
 dependencies = [
  "async-trait",
  "futures",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.14"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
+checksum = "57c0d7b74b563b49d38dae00a0c37d4d6de9b432382b2892f0574ddcae73fd0a"
 
 [[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
@@ -1696,15 +1785,15 @@
 name = "pin-project-internal"
 version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
@@ -1869,19 +1958,18 @@
  "fixed-hash",
  "impl-codec",
  "uint",
 ]
 
 [[package]]
 name = "proc-macro-crate"
-version = "2.0.2"
+version = "3.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b00f26d3400549137f92511a46ac1cd8ce37cb5598a96d382381458b992a5d24"
+checksum = "6d37c51ca738a55da99dc0c4a34860fd675453b8b36209178c2249bb13651284"
 dependencies = [
- "toml_datetime",
  "toml_edit",
 ]
 
 [[package]]
 name = "proc-macro-error"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1903,17 +1991,17 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.81"
+version = "1.0.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
+checksum = "ec96c6a92621310b51366f1e28d05ef11489516e93be030060e5fc12024a49d6"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "proptest"
 version = "1.4.0"
@@ -1945,24 +2033,24 @@
 
 [[package]]
 name = "pyo3"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
 dependencies = [
+ "anyhow",
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
- "serde",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-asyncio"
 version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2000,28 +2088,28 @@
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.60",
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
- "syn 2.0.60",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "quick-error"
 version = "1.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a1d01941d82fa2ab50be1e79e6714289dd7cde78eba4c074bc5a4374f650dfe0"
@@ -2251,17 +2339,17 @@
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
 
@@ -2276,15 +2364,15 @@
 
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
 version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
@@ -2318,23 +2406,23 @@
 dependencies = [
  "base64 0.22.1",
  "rustls-pki-types",
 ]
 
 [[package]]
 name = "rustls-pki-types"
-version = "1.5.0"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "beb461507cee2c2ff151784c52762cf4d9ff6a61f3e80968600ed24fa837fa54"
+checksum = "976295e77ce332211c0d24d92c0e83e50f5c5f046d11082cea19f3df13a3562d"
 
 [[package]]
 name = "rustls-webpki"
-version = "0.102.3"
+version = "0.102.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f3bce581c0dd41bce533ce695a1437fa16a7ab5ac3ccfa99fe1a620a7885eabf"
+checksum = "ff448f7e92e913c4b7d4c6d8e4540a1724b319b4152b8aef6d4cf8339712b33e"
 dependencies = [
  "ring",
  "rustls-pki-types",
  "untrusted",
 ]
 
 [[package]]
@@ -2347,17 +2435,17 @@
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
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
@@ -2382,17 +2470,17 @@
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
@@ -2403,37 +2491,37 @@
 name = "seq-macro"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
 
 [[package]]
 name = "serde"
-version = "1.0.200"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ddc6f9cc94d67c0e21aaf7eda3a010fd3af78ebf6e096aa6e2e13c79749cce4f"
+checksum = "7253ab4de971e72fb7be983802300c30b5a7f0c2e56fab8abfc6a214307c0094"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.200"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "856f046b9400cee3c8c94ed572ecdb752444c24528c035cd35882aad6f492bcb"
+checksum = "500cbc0ebeb6f46627f50f3f5811ccf6bf00643be300b4c3eabc0ef55dc5b5ba"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.116"
+version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -2457,17 +2545,17 @@
  "cfg-if",
  "cpufeatures",
  "digest 0.10.7",
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
@@ -2482,83 +2570,14 @@
 [[package]]
 name = "simdutf8"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
 
 [[package]]
-name = "skar-client"
-version = "0.18.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "afc01e61a814dffca760b3364ab03d75e6c63bd8322945f7796722436741c7c3"
-dependencies = [
- "alloy-dyn-abi",
- "alloy-json-abi",
- "anyhow",
- "arrayvec",
- "capnp",
- "faster-hex",
- "fastrange-rs",
- "futures",
- "log",
- "num_cpus",
- "polars-arrow",
- "polars-parquet",
- "rand",
- "rayon",
- "reqwest",
- "ruint",
- "serde",
- "serde_json",
- "skar-format",
- "skar-net-types",
- "skar-schema",
- "tokio",
- "tokio-util",
- "url",
- "xxhash-rust",
-]
-
-[[package]]
-name = "skar-format"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "276a8fafebc7737dfc7d9ce303fc1deee7c6bbaa53a6620aa2218855409bdb4b"
-dependencies = [
- "arrayvec",
- "derive_more",
- "faster-hex",
- "serde",
- "thiserror",
-]
-
-[[package]]
-name = "skar-net-types"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4be4bb45cbce53cb2072e90a1d03026270cbeabee0b9631410ff1133fcab2c83"
-dependencies = [
- "arrayvec",
- "capnp",
- "capnpc",
- "serde",
- "skar-format",
-]
-
-[[package]]
-name = "skar-schema"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c300d21f258c87b58ef60b56421ac82b219ae465f95466c9b1d3e9c8ef8cb09"
-dependencies = [
- "anyhow",
- "polars-arrow",
-]
-
-[[package]]
 name = "slab"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
@@ -2667,33 +2686,33 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.60"
+version = "2.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
+checksum = "c42f3f41a2de00b01c0aaad383c5a45241efc8b2d1eda5661812fda5f3cdcff5"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn-solidity"
-version = "0.7.2"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aa0cefd02f532035d83cfec82647c6eb53140b0485220760e669f4bad489e36"
+checksum = "b8db114c44cf843a8bacd37a146e37987a0b823a0e8bc4fdc610c9c72ab397a5"
 dependencies = [
  "paste",
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "sync_wrapper"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2047c6ded9c721764247e62cd3b03c09ffc529b2ba5b10ec482ae507a4a70160"
@@ -2726,30 +2745,30 @@
  "fastrand",
  "rustix",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.59"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
+checksum = "c546c80d6be4bc6a00c0f01730c08df82eaa7a7a61f11d656526506112cc1709"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.59"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
+checksum = "46c3384250002a6d5af4d114f2845d37b57521033f30d5c3f46c4d70e1197533"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "tiny-keccak"
 version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c9d3793400a45f954c52e73d068316d76b6f4e36977e3fcebb13a2721e80237"
@@ -2793,15 +2812,15 @@
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "tokio-rustls"
 version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "775e0c0f0adb3a2f22a00c4745d728b479985fc15ee7ca6a2608388c5569860f"
@@ -2823,23 +2842,23 @@
  "futures-sink",
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
 name = "toml_datetime"
-version = "0.6.3"
+version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7cda73e2f1397b1262d6dfdcef8aafae14d1de7748d66822d3bfeeb6d03e5e4b"
+checksum = "4badfd56924ae69bcc9039335b2e017639ce3f9b001c393c1b2d1ef846ce2cbf"
 
 [[package]]
 name = "toml_edit"
-version = "0.20.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "396e4d48bbb2b7554c944bde63101b5ae446cff6ec4a24227428f15eb72ef338"
+checksum = "6a8534fd7f78b5405e860340ad6575217ce99f38d4d5c8f2442cb5ecb50090e1"
 dependencies = [
  "indexmap",
  "toml_datetime",
  "winnow 0.5.40",
 ]
 
 [[package]]
@@ -2851,15 +2870,14 @@
  "futures-core",
  "futures-util",
  "pin-project",
  "pin-project-lite",
  "tokio",
  "tower-layer",
  "tower-service",
- "tracing",
 ]
 
 [[package]]
 name = "tower-layer"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c20c8dbed6283a09604c3e69b4b7eeb54e298b8a600d4d5ecb5ad39de609f1d0"
@@ -2872,15 +2890,14 @@
 
 [[package]]
 name = "tracing"
 version = "0.1.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
 dependencies = [
- "log",
  "pin-project-lite",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
@@ -3030,15 +3047,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.66",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -3064,15 +3081,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.66",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -3266,17 +3283,17 @@
 checksum = "f593a95398737aeed53e489c785df13f3618e41dbcd6718c6addbf1395aa6876"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winnow"
-version = "0.6.7"
+version = "0.6.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14b9415ee827af173ebb3f15f9083df5a122eb93572ec28741fb153356ea2578"
+checksum = "c3c52e9c97a68071b23e836c9380edae937f17b9c4667bd021973efc689f618d"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winreg"
 version = "0.52.0"
@@ -3300,50 +3317,50 @@
 name = "xxhash-rust"
 version = "0.8.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "927da81e25be1e1a2901d59b81b37dd2efd1fc9c9345a55007f09bf5a2d3ee03"
 
 [[package]]
 name = "zerocopy"
-version = "0.7.33"
+version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "087eca3c1eaf8c47b94d02790dd086cd594b912d2043d4de4bfdd466b3befb7c"
+checksum = "ae87e3fcd617500e5d106f0380cf7b77f3c6092aae37191433159dda23cfb087"
 dependencies = [
  "zerocopy-derive",
 ]
 
 [[package]]
 name = "zerocopy-derive"
-version = "0.7.33"
+version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f4b6c273f496d8fd4eaf18853e6b448760225dc030ff2c485a786859aea6393"
+checksum = "15e934569e47891f7d9411f1a451d947a60e000ab3bd24fbb970f000387d1b3b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
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
- "syn 2.0.60",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "zstd"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2d789b1514203a1120ad2429eae43a7bd32b90976a7bb8a05f7ec02fa88cc23a"
```

### Comparing `hypersync-0.6.2/pyproject.toml` & `hypersync-0.7.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -14,9 +14,7 @@
     "Topic :: Database :: Front-Ends",
     "Topic :: Software Development :: Libraries",
 ]
 dynamic = ["version"]
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
-profile = "no_lto"
-skip-auditwheel = false
```

### Comparing `hypersync-0.6.2/PKG-INFO` & `hypersync-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hypersync
-Version: 0.6.2
+Version: 0.7.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: strenum >=0.4.15, <0.4.16
```

