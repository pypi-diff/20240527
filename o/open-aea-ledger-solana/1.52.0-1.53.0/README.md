# Comparing `tmp/open_aea_ledger_solana-1.52.0.tar.gz` & `tmp/open_aea_ledger_solana-1.53.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_aea_ledger_solana-1.52.0.tar", last modified: Mon May  6 07:25:18 2024, max compression
+gzip compressed data, was "open_aea_ledger_solana-1.53.0.tar", last modified: Mon May 27 09:29:41 2024, max compression
```

## Comparing `open_aea_ledger_solana-1.52.0.tar` & `open_aea_ledger_solana-1.53.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:25:18.121408 open_aea_ledger_solana-1.52.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-06 07:25:18.121408 open_aea_ledger_solana-1.52.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:25:18.117408 open_aea_ledger_solana-1.52.0/aea_ledger_solana/
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/aea_ledger_solana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/aea_ledger_solana/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/aea_ledger_solana/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8599 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/aea_ledger_solana/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/aea_ledger_solana/faucet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/aea_ledger_solana/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/aea_ledger_solana/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    32925 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/aea_ledger_solana/solana.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/aea_ledger_solana/solana_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/aea_ledger_solana/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/aea_ledger_solana/transaction_instruction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/aea_ledger_solana/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:25:18.121408 open_aea_ledger_solana-1.52.0/open_aea_ledger_solana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-06 07:25:18.000000 open_aea_ledger_solana-1.52.0/open_aea_ledger_solana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-06 07:25:18.000000 open_aea_ledger_solana-1.52.0/open_aea_ledger_solana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 07:25:18.000000 open_aea_ledger_solana-1.52.0/open_aea_ledger_solana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-06 07:25:18.000000 open_aea_ledger_solana-1.52.0/open_aea_ledger_solana.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-06 07:25:18.000000 open_aea_ledger_solana-1.52.0/open_aea_ledger_solana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-06 07:25:18.000000 open_aea_ledger_solana-1.52.0/open_aea_ledger_solana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 07:25:18.121408 open_aea_ledger_solana-1.52.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:25:18.121408 open_aea_ledger_solana-1.52.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:25:18.121408 open_aea_ledger_solana-1.52.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/tests/data/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:25:18.113408 open_aea_ledger_solana-1.52.0/tests/data/dummy_contract/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:25:18.121408 open_aea_ledger_solana-1.52.0/tests/data/dummy_contract/build/
--rw-r--r--   0 runner    (1001) docker     (127)    84952 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/tests/data/dummy_contract/build/idl.json
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/tests/data/solana_private_key0.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/tests/data/solana_private_key1.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/tests/data/solana_private_key2.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/tests/data/solana_private_key_program.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:25:18.113408 open_aea_ledger_solana-1.52.0/tests/data/spl-token-faucet/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:25:18.113408 open_aea_ledger_solana-1.52.0/tests/data/spl-token-faucet/target/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:25:18.121408 open_aea_ledger_solana-1.52.0/tests/data/spl-token-faucet/target/deploy/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/tests/data/spl-token-faucet/target/deploy/spl_token_faucet-keypair.json
--rwxr-xr-x   0 runner    (1001) docker     (127)   175592 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/tests/data/spl-token-faucet/target/deploy/spl_token_faucet.so
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:25:18.121408 open_aea_ledger_solana-1.52.0/tests/data/spl-token-faucet/target/idl/
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/tests/data/spl-token-faucet/target/idl/spl_token_faucet.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:25:18.113408 open_aea_ledger_solana-1.52.0/tests/data/tic-tac-toe/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:25:18.113408 open_aea_ledger_solana-1.52.0/tests/data/tic-tac-toe/target/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:25:18.121408 open_aea_ledger_solana-1.52.0/tests/data/tic-tac-toe/target/deploy/
--rwxr-xr-x   0 runner    (1001) docker     (127)   208064 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/tests/data/tic-tac-toe/target/deploy/tic_tac_toe.so
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:25:18.121408 open_aea_ledger_solana-1.52.0/tests/data/tic-tac-toe/target/idl/
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/tests/data/tic-tac-toe/target/idl/tic_tac_toe.json
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/tests/test_contracts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/tests/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/tests/test_faucet.py
--rw-r--r--   0 runner    (1001) docker     (127)    20438 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/tests/test_solana.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/tests/test_solana_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-05-06 07:24:46.000000 open_aea_ledger_solana-1.52.0/tests/test_underlying_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:29:41.670307 open_aea_ledger_solana-1.53.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-27 09:29:41.670307 open_aea_ledger_solana-1.53.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:29:41.666307 open_aea_ledger_solana-1.53.0/aea_ledger_solana/
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/aea_ledger_solana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/aea_ledger_solana/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/aea_ledger_solana/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8599 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/aea_ledger_solana/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/aea_ledger_solana/faucet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/aea_ledger_solana/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/aea_ledger_solana/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    32925 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/aea_ledger_solana/solana.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/aea_ledger_solana/solana_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/aea_ledger_solana/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/aea_ledger_solana/transaction_instruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/aea_ledger_solana/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:29:41.670307 open_aea_ledger_solana-1.53.0/open_aea_ledger_solana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-27 09:29:41.000000 open_aea_ledger_solana-1.53.0/open_aea_ledger_solana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-27 09:29:41.000000 open_aea_ledger_solana-1.53.0/open_aea_ledger_solana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 09:29:41.000000 open_aea_ledger_solana-1.53.0/open_aea_ledger_solana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-27 09:29:41.000000 open_aea_ledger_solana-1.53.0/open_aea_ledger_solana.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-27 09:29:41.000000 open_aea_ledger_solana-1.53.0/open_aea_ledger_solana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 09:29:41.000000 open_aea_ledger_solana-1.53.0/open_aea_ledger_solana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 09:29:41.670307 open_aea_ledger_solana-1.53.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:29:41.666307 open_aea_ledger_solana-1.53.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:29:41.666307 open_aea_ledger_solana-1.53.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/tests/data/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:29:41.662306 open_aea_ledger_solana-1.53.0/tests/data/dummy_contract/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:29:41.666307 open_aea_ledger_solana-1.53.0/tests/data/dummy_contract/build/
+-rw-r--r--   0 runner    (1001) docker     (127)    84952 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/tests/data/dummy_contract/build/idl.json
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/tests/data/solana_private_key0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/tests/data/solana_private_key1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/tests/data/solana_private_key2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/tests/data/solana_private_key_program.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:29:41.662306 open_aea_ledger_solana-1.53.0/tests/data/spl-token-faucet/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:29:41.662306 open_aea_ledger_solana-1.53.0/tests/data/spl-token-faucet/target/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:29:41.666307 open_aea_ledger_solana-1.53.0/tests/data/spl-token-faucet/target/deploy/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/tests/data/spl-token-faucet/target/deploy/spl_token_faucet-keypair.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)   175592 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/tests/data/spl-token-faucet/target/deploy/spl_token_faucet.so
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:29:41.670307 open_aea_ledger_solana-1.53.0/tests/data/spl-token-faucet/target/idl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/tests/data/spl-token-faucet/target/idl/spl_token_faucet.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:29:41.662306 open_aea_ledger_solana-1.53.0/tests/data/tic-tac-toe/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:29:41.662306 open_aea_ledger_solana-1.53.0/tests/data/tic-tac-toe/target/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:29:41.670307 open_aea_ledger_solana-1.53.0/tests/data/tic-tac-toe/target/deploy/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   208064 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/tests/data/tic-tac-toe/target/deploy/tic_tac_toe.so
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:29:41.670307 open_aea_ledger_solana-1.53.0/tests/data/tic-tac-toe/target/idl/
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/tests/data/tic-tac-toe/target/idl/tic_tac_toe.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/tests/test_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/tests/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/tests/test_faucet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20438 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/tests/test_solana.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/tests/test_solana_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-05-27 09:29:07.000000 open_aea_ledger_solana-1.53.0/tests/test_underlying_lib.py
```

### Comparing `open_aea_ledger_solana-1.52.0/LICENSE` & `open_aea_ledger_solana-1.53.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/PKG-INFO` & `open_aea_ledger_solana-1.53.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-solana
-Version: 1.52.0
+Version: 1.53.0
 Summary: Python package wrapping the public and private key cryptography and ledger api of solana.
 Author: dassy23
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `open_aea_ledger_solana-1.52.0/aea_ledger_solana/__init__.py` & `open_aea_ledger_solana-1.53.0/aea_ledger_solana/__init__.py`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/aea_ledger_solana/account.py` & `open_aea_ledger_solana-1.53.0/aea_ledger_solana/account.py`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/aea_ledger_solana/constants.py` & `open_aea_ledger_solana-1.53.0/aea_ledger_solana/constants.py`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/aea_ledger_solana/crypto.py` & `open_aea_ledger_solana-1.53.0/aea_ledger_solana/crypto.py`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/aea_ledger_solana/faucet.py` & `open_aea_ledger_solana-1.53.0/aea_ledger_solana/faucet.py`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/aea_ledger_solana/helper.py` & `open_aea_ledger_solana-1.53.0/aea_ledger_solana/helper.py`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/aea_ledger_solana/solana.py` & `open_aea_ledger_solana-1.53.0/aea_ledger_solana/solana.py`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/aea_ledger_solana/solana_api.py` & `open_aea_ledger_solana-1.53.0/aea_ledger_solana/solana_api.py`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/aea_ledger_solana/transaction.py` & `open_aea_ledger_solana-1.53.0/aea_ledger_solana/transaction.py`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/aea_ledger_solana/transaction_instruction.py` & `open_aea_ledger_solana-1.53.0/aea_ledger_solana/transaction_instruction.py`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/aea_ledger_solana/utils.py` & `open_aea_ledger_solana-1.53.0/aea_ledger_solana/utils.py`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/open_aea_ledger_solana.egg-info/PKG-INFO` & `open_aea_ledger_solana-1.53.0/open_aea_ledger_solana.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-solana
-Version: 1.52.0
+Version: 1.53.0
 Summary: Python package wrapping the public and private key cryptography and ledger api of solana.
 Author: dassy23
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `open_aea_ledger_solana-1.52.0/open_aea_ledger_solana.egg-info/SOURCES.txt` & `open_aea_ledger_solana-1.53.0/open_aea_ledger_solana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/setup.py` & `open_aea_ledger_solana-1.53.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 """Setup script for "aea_ledger_solana" package."""
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="open-aea-ledger-solana",
-    version="1.52.0",
+    version="1.53.0",
     author="dassy23",
     license="Apache-2.0",
     description="Python package wrapping the public and private key cryptography and ledger api of solana.",
     long_description="Python package wrapping the public and private key cryptography and ledger api of solana.",
     long_description_content_type="text/markdown",
     packages=find_packages(include=["aea_ledger_solana*"]),
     package_data={"aea_ledger_solana": ["py.typed"]},
```

### Comparing `open_aea_ledger_solana-1.52.0/tests/__init__.py` & `open_aea_ledger_solana-1.53.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/tests/conftest.py` & `open_aea_ledger_solana-1.53.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/tests/data/Dockerfile` & `open_aea_ledger_solana-1.53.0/tests/data/Dockerfile`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/tests/data/dummy_contract/build/idl.json` & `open_aea_ledger_solana-1.53.0/tests/data/dummy_contract/build/idl.json`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/tests/data/spl-token-faucet/target/deploy/spl_token_faucet.so` & `open_aea_ledger_solana-1.53.0/tests/data/spl-token-faucet/target/deploy/spl_token_faucet.so`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/tests/data/spl-token-faucet/target/idl/spl_token_faucet.json` & `open_aea_ledger_solana-1.53.0/tests/data/spl-token-faucet/target/idl/spl_token_faucet.json`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/tests/data/tic-tac-toe/target/deploy/tic_tac_toe.so` & `open_aea_ledger_solana-1.53.0/tests/data/tic-tac-toe/target/deploy/tic_tac_toe.so`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/tests/data/tic-tac-toe/target/idl/tic_tac_toe.json` & `open_aea_ledger_solana-1.53.0/tests/data/tic-tac-toe/target/idl/tic_tac_toe.json`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/tests/test_contracts.py` & `open_aea_ledger_solana-1.53.0/tests/test_contracts.py`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/tests/test_crypto.py` & `open_aea_ledger_solana-1.53.0/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/tests/test_faucet.py` & `open_aea_ledger_solana-1.53.0/tests/test_faucet.py`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/tests/test_solana.py` & `open_aea_ledger_solana-1.53.0/tests/test_solana.py`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/tests/test_solana_transaction.py` & `open_aea_ledger_solana-1.53.0/tests/test_solana_transaction.py`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_solana-1.52.0/tests/test_underlying_lib.py` & `open_aea_ledger_solana-1.53.0/tests/test_underlying_lib.py`

 * *Files identical despite different names*

