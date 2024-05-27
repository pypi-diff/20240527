# Comparing `tmp/skale.py-7.dev11.tar.gz` & `tmp/skale.py-7.dev12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skale.py-7.dev11.tar", last modified: Wed Apr 24 15:12:16 2024, max compression
+gzip compressed data, was "skale.py-7.dev12.tar", last modified: Mon May 27 12:45:31 2024, max compression
```

## Comparing `skale.py-7.dev11.tar` & `skale.py-7.dev12.tar`

### file list

```diff
@@ -1,105 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.186797 skale.py-7.dev11/
--rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-04-24 15:11:04.000000 skale.py-7.dev11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-24 15:11:04.000000 skale.py-7.dev11/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-24 15:12:16.182796 skale.py-7.dev11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-24 15:11:04.000000 skale.py-7.dev11/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:12:16.186797 skale.py-7.dev11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-24 15:12:15.000000 skale.py-7.dev11/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.174796 skale.py-7.dev11/skale/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.174796 skale.py-7.dev11/skale/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.174796 skale.py-7.dev11/skale/contracts/allocator/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/allocator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/allocator/allocator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/allocator/escrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/base_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/contract_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.174796 skale.py-7.dev11/skale/contracts/ima/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/ima/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/ima/linker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.178796 skale.py-7.dev11/skale/contracts/manager/
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/bounty_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/constants_holder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.178796 skale.py-7.dev11/skale/contracts/manager/delegation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/delegation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/delegation/delegation_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/delegation/delegation_period_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/delegation/distributor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/delegation/slashing_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/delegation/token_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/delegation/validator_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/dkg.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/key_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/node_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/punisher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/schains.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/schains_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/sync_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.178796 skale.py-7.dev11/skale/contracts/manager/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/test/time_helpers_with_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/wallets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.178796 skale.py-7.dev11/skale/dataclasses/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/dataclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/dataclasses/delegation_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/dataclasses/node_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/dataclasses/schain_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/dataclasses/skaled_ports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.178796 skale.py-7.dev11/skale/schain_config/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/schain_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/schain_config/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/schain_config/ports_allocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/schain_config/rotation_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/skale_allocator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/skale_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/skale_ima.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/skale_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.182796 skale.py-7.dev11/skale/transactions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/transactions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/transactions/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/transactions/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.182796 skale.py-7.dev11/skale/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/account_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/contract_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/contract_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.182796 skale.py-7.dev11/skale/utils/contracts_provision/
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/contracts_provision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/contracts_provision/allocator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/contracts_provision/fake_multisig_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/contracts_provision/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/contracts_provision/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.182796 skale.py-7.dev11/skale/utils/random_names/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/random_names/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/random_names/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/random_names/vocabulary.py
--rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/web3_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.182796 skale.py-7.dev11/skale/wallets/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/wallets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/wallets/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/wallets/ledger_wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/wallets/redis_wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/wallets/sgx_wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/wallets/web3_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.174796 skale.py-7.dev11/skale.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-24 15:12:16.000000 skale.py-7.dev11/skale.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-24 15:12:16.000000 skale.py-7.dev11/skale.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:12:16.000000 skale.py-7.dev11/skale.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-24 15:12:16.000000 skale.py-7.dev11/skale.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 15:12:16.000000 skale.py-7.dev11/skale.py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.170796 skale.py-7.dev11/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.182796 skale.py-7.dev11/tests/schain_config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:11:04.000000 skale.py-7.dev11/tests/schain_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-24 15:11:04.000000 skale.py-7.dev11/tests/schain_config/generator_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-24 15:11:04.000000 skale.py-7.dev11/tests/schain_config/ports_allocation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:45:31.897572 skale.py-7.dev12/
+-rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-05-27 12:44:18.000000 skale.py-7.dev12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-27 12:44:18.000000 skale.py-7.dev12/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-27 12:45:31.897572 skale.py-7.dev12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-27 12:44:18.000000 skale.py-7.dev12/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 12:45:31.897572 skale.py-7.dev12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-27 12:45:31.000000 skale.py-7.dev12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:45:31.889572 skale.py-7.dev12/skale/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:45:31.893572 skale.py-7.dev12/skale/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:45:31.893572 skale.py-7.dev12/skale/contracts/allocator/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/allocator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/allocator/allocator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/allocator/escrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/allocator_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/base_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:45:31.893572 skale.py-7.dev12/skale/contracts/ima/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/ima/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/ima/linker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/ima_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:45:31.893572 skale.py-7.dev12/skale/contracts/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/bounty_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/constants_holder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/contract_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:45:31.893572 skale.py-7.dev12/skale/contracts/manager/delegation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/delegation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9697 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/delegation/delegation_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/delegation/delegation_period_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/delegation/distributor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/delegation/slashing_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/delegation/token_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/delegation/validator_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/dkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/key_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/node_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/punisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/schains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/schains_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/sync_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:45:31.893572 skale.py-7.dev12/skale/contracts/manager/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/test/time_helpers_with_debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/manager/wallets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/contracts/skale_manager_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:45:31.893572 skale.py-7.dev12/skale/dataclasses/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/dataclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/dataclasses/node_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/dataclasses/schain_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/dataclasses/skaled_ports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:45:31.897572 skale.py-7.dev12/skale/schain_config/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/schain_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/schain_config/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/schain_config/ports_allocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/schain_config/rotation_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/skale_allocator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/skale_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/skale_ima.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8024 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/skale_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:45:31.897572 skale.py-7.dev12/skale/transactions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/transactions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/transactions/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/transactions/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:45:31.897572 skale.py-7.dev12/skale/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/utils/account_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/utils/contract_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/utils/contract_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:45:31.897572 skale.py-7.dev12/skale/utils/contracts_provision/
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/utils/contracts_provision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/utils/contracts_provision/allocator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/utils/contracts_provision/fake_multisig_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13231 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/utils/contracts_provision/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/utils/contracts_provision/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/utils/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:45:31.897572 skale.py-7.dev12/skale/utils/random_names/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/utils/random_names/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/utils/random_names/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/utils/random_names/vocabulary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10030 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/utils/web3_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:45:31.897572 skale.py-7.dev12/skale/wallets/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/wallets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/wallets/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8849 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/wallets/ledger_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/wallets/redis_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/wallets/sgx_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-27 12:44:18.000000 skale.py-7.dev12/skale/wallets/web3_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:45:31.889572 skale.py-7.dev12/skale.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-27 12:45:31.000000 skale.py-7.dev12/skale.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-27 12:45:31.000000 skale.py-7.dev12/skale.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:45:31.000000 skale.py-7.dev12/skale.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-27 12:45:31.000000 skale.py-7.dev12/skale.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 12:45:31.000000 skale.py-7.dev12/skale.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:45:31.889572 skale.py-7.dev12/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:45:31.897572 skale.py-7.dev12/tests/schain_config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:44:18.000000 skale.py-7.dev12/tests/schain_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-27 12:44:18.000000 skale.py-7.dev12/tests/schain_config/generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-27 12:44:18.000000 skale.py-7.dev12/tests/schain_config/ports_allocation_test.py
```

### Comparing `skale.py-7.dev11/LICENSE` & `skale.py-7.dev12/LICENSE`

 * *Files identical despite different names*

### Comparing `skale.py-7.dev11/PKG-INFO` & `skale.py-7.dev12/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skale.py
-Version: 7.dev11
+Version: 7.dev12
 Summary: SKALE client tools
 Home-page: https://github.com/skalenetwork/skale.py
 Author: SKALE Labs
 Author-email: support@skalelabs.com
 Keywords: skale
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `skale.py-7.dev11/README.md` & `skale.py-7.dev12/README.md`

 * *Files identical despite different names*

### Comparing `skale.py-7.dev11/setup.py` & `skale.py-7.dev12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,25 +29,25 @@
 
 extras_require['dev'] = (
     extras_require['linter'] + extras_require['dev'] + extras_require['hw-wallet']
 )
 
 setup(
     name='skale.py',
-    version='7dev11',
+    version='7dev12',
     description='SKALE client tools',
     long_description_markdown_filename='README.md',
     author='SKALE Labs',
     author_email='support@skalelabs.com',
     url='https://github.com/skalenetwork/skale.py',
     include_package_data=True,
     install_requires=[
         "asyncio==3.4.3",
         "pyyaml==6.0",
-        "redis==4.4.4",
+        "redis==5.0.3",
         "sgx.py==0.9dev2",
         "skale-contracts==1.0.1a5",
         "typing-extensions==4.9.0",
         "web3==6.13.0"
     ],
 
     python_requires='>=3.7,<4',
```

### Comparing `skale.py-7.dev11/skale/config.py` & `skale.py-7.dev12/skale/config.py`

 * *Files identical despite different names*

### Comparing `skale.py-7.dev11/skale/contracts/allocator/allocator.py` & `skale.py-7.dev12/skale/contracts/allocator/allocator.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,19 +14,32 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 """ SKALE Allocator Core Escrow methods """
 
-from enum import IntEnum
+from typing import Any, Dict, List
 
-from skale.contracts.base_contract import BaseContract, transaction_method
-from skale.transactions.exceptions import ContractLogicError
-from skale.transactions.result import TxRes
+from eth_typing import ChecksumAddress
+from web3 import Web3
+from web3.contract.contract import ContractFunction
+from web3.exceptions import ContractLogicError
+from web3.types import Wei
+
+from skale.contracts.allocator_contract import AllocatorContract
+from skale.contracts.base_contract import transaction_method
+from skale.types.allocation import (
+    BeneficiaryStatus,
+    BeneficiaryPlan,
+    Plan,
+    PlanId,
+    PlanWithId,
+    TimeUnit
+)
 from skale.utils.helper import format_fields
 
 
 PLAN_FIELDS = [
     'totalVestingDuration',
     'vestingCliff',
     'vestingIntervalTimeUnit',
@@ -43,133 +56,163 @@
     'amountAfterLockup'
 ]
 
 MAX_NUM_OF_PLANS = 9999
 MAX_NUM_OF_BENEFICIARIES = 9999
 
 
-class TimeUnit(IntEnum):
-    DAY = 0
-    MONTH = 1
-    YEAR = 2
-
-
-class BeneficiaryStatus(IntEnum):
-    UNKNOWN = 0
-    CONFIRMED = 1
-    ACTIVE = 2
-    TERMINATED = 3
-
-
-class Allocator(BaseContract):
-    def is_beneficiary_registered(self, beneficiary_address: str) -> bool:
+class Allocator(AllocatorContract):
+    def is_beneficiary_registered(self, beneficiary_address: ChecksumAddress) -> bool:
         """Confirms whether the beneficiary is registered in a Plan.
 
         :returns: Boolean value
         :rtype: bool
         """
-        return self.contract.functions.isBeneficiaryRegistered(beneficiary_address).call()
+        return bool(self.contract.functions.isBeneficiaryRegistered(beneficiary_address).call())
 
-    def is_delegation_allowed(self, beneficiary_address: str) -> bool:
-        return self.contract.functions.isDelegationAllowed(beneficiary_address).call()
+    def is_delegation_allowed(self, beneficiary_address: ChecksumAddress) -> bool:
+        return bool(self.contract.functions.isDelegationAllowed(beneficiary_address).call())
 
-    def is_vesting_active(self, beneficiary_address: str) -> bool:
-        return self.contract.functions.isVestingActive(beneficiary_address).call()
+    def is_vesting_active(self, beneficiary_address: ChecksumAddress) -> bool:
+        return bool(self.contract.functions.isVestingActive(beneficiary_address).call())
 
-    def get_escrow_address(self, beneficiary_address: str) -> str:
-        return self.contract.functions.getEscrowAddress(beneficiary_address).call()
+    def get_escrow_address(self, beneficiary_address: ChecksumAddress) -> ChecksumAddress:
+        return Web3.to_checksum_address(
+            self.contract.functions.getEscrowAddress(beneficiary_address).call()
+        )
 
     @transaction_method
     def add_plan(
             self,
             vesting_cliff: int,
             total_vesting_duration: int,
             vesting_interval_time_unit: TimeUnit,
             vesting_interval: int,
             can_delegate: bool,
             is_terminatable: bool
-    ) -> TxRes:
+    ) -> ContractFunction:
         return self.contract.functions.addPlan(
             vestingCliff=vesting_cliff,
             totalVestingDuration=total_vesting_duration,
             vestingIntervalTimeUnit=vesting_interval_time_unit.value,
             vestingInterval=vesting_interval,
             canDelegate=can_delegate,
             isTerminatable=is_terminatable
         )
 
     @transaction_method
     def connect_beneficiary_to_plan(
             self,
-            beneficiary_address: str,
+            beneficiary_address: ChecksumAddress,
             plan_id: int,
             start_month: int,
             full_amount: int,
             lockup_amount: int,
-    ) -> TxRes:
+    ) -> ContractFunction:
         return self.contract.functions.connectBeneficiaryToPlan(
             beneficiary=beneficiary_address,
             planId=plan_id,
             startMonth=start_month,
             fullAmount=full_amount,
             lockupAmount=lockup_amount
         )
 
     @transaction_method
-    def start_vesting(self, beneficiary_address: str) -> TxRes:
+    def start_vesting(self, beneficiary_address: ChecksumAddress) -> ContractFunction:
         return self.contract.functions.startVesting(beneficiary_address)
 
     @transaction_method
-    def stop_vesting(self, beneficiary_address: str) -> TxRes:
+    def stop_vesting(self, beneficiary_address: ChecksumAddress) -> ContractFunction:
         return self.contract.functions.stopVesting(beneficiary_address)
 
     @transaction_method
-    def grant_role(self, role: bytes, address: str) -> TxRes:
+    def grant_role(self, role: bytes, address: ChecksumAddress) -> ContractFunction:
         return self.contract.functions.grantRole(role, address)
 
     def vesting_manager_role(self) -> bytes:
-        return self.contract.functions.VESTING_MANAGER_ROLE().call()
+        return bytes(self.contract.functions.VESTING_MANAGER_ROLE().call())
 
-    def has_role(self, role: bytes, address: str) -> bool:
-        return self.contract.functions.hasRole(role, address).call()
+    def has_role(self, role: bytes, address: ChecksumAddress) -> bool:
+        return bool(self.contract.functions.hasRole(role, address).call())
 
-    def __get_beneficiary_plan_params_raw(self, beneficiary_address: str):
-        return self.contract.functions.getBeneficiaryPlanParams(beneficiary_address).call()
+    def __get_beneficiary_plan_params_raw(self, beneficiary_address: ChecksumAddress) -> List[Any]:
+        return list(self.contract.functions.getBeneficiaryPlanParams(beneficiary_address).call())
 
     @format_fields(BENEFICIARY_FIELDS)
-    def get_beneficiary_plan_params_dict(self, beneficiary_address: str) -> dict:
+    def get_beneficiary_plan_params_dict(self, beneficiary_address: ChecksumAddress) -> List[Any]:
         return self.__get_beneficiary_plan_params_raw(beneficiary_address)
 
-    def get_beneficiary_plan_params(self, beneficiary_address: str) -> dict:
+    def get_beneficiary_plan_params(self, beneficiary_address: ChecksumAddress) -> BeneficiaryPlan:
         plan_params = self.get_beneficiary_plan_params_dict(beneficiary_address)
-        plan_params['statusName'] = BeneficiaryStatus(plan_params['status']).name
-        return plan_params
+        if plan_params is None:
+            raise ValueError('Plan for ', beneficiary_address, ' is missing')
+        if isinstance(plan_params, list):
+            return self._to_beneficiary_plan({
+                **plan_params[0],
+                'statusName': BeneficiaryStatus(plan_params[0]['status']).name
+            })
+        if isinstance(plan_params, dict):
+            return self._to_beneficiary_plan({
+                **plan_params,
+                'statusName': BeneficiaryStatus(plan_params.get('status', 0)).name
+            })
+        raise TypeError(f'Internal error on getting plan params for ${beneficiary_address}')
 
-    def __get_plan_raw(self, plan_id: int):
-        return self.contract.functions.getPlan(plan_id).call()
+    def __get_plan_raw(self, plan_id: PlanId) -> List[Any]:
+        return list(self.contract.functions.getPlan(plan_id).call())
 
     @format_fields(PLAN_FIELDS)
-    def get_plan(self, plan_id: int) -> dict:
+    def get_untyped_plan(self, plan_id: PlanId) -> List[Any]:
         return self.__get_plan_raw(plan_id)
 
-    def get_all_plans(self) -> dict:
+    def get_plan(self, plan_id: PlanId) -> Plan:
+        untyped_plan = self.get_untyped_plan(plan_id)
+        if untyped_plan is None:
+            raise ValueError('Plan ', plan_id, ' is missing')
+        if isinstance(untyped_plan, list):
+            return self._to_plan(untyped_plan[0])
+        if isinstance(untyped_plan, dict):
+            return self._to_plan(untyped_plan)
+        raise TypeError(plan_id)
+
+    def get_all_plans(self) -> List[PlanWithId]:
         plans = []
         for i in range(1, MAX_NUM_OF_PLANS):
             try:
-                plan = self.get_plan(i)
-                plan['planId'] = i
+                plan_id = PlanId(i)
+                plan = PlanWithId({**self.get_plan(plan_id), 'planId': plan_id})
                 plans.append(plan)
             except (ContractLogicError, ValueError):
                 break
         return plans
 
-    def calculate_vested_amount(self, address: str) -> int:
-        return self.contract.functions.calculateVestedAmount(address).call()
+    def calculate_vested_amount(self, address: ChecksumAddress) -> Wei:
+        return Wei(self.contract.functions.calculateVestedAmount(address).call())
 
-    def get_finish_vesting_time(self, address: str) -> int:
-        return self.contract.functions.getFinishVestingTime(address).call()
+    def get_finish_vesting_time(self, address: ChecksumAddress) -> int:
+        return int(self.contract.functions.getFinishVestingTime(address).call())
 
-    def get_lockup_period_end_timestamp(self, address: str) -> int:
-        return self.contract.functions.getLockupPeriodEndTimestamp(address).call()
+    def get_lockup_period_end_timestamp(self, address: ChecksumAddress) -> int:
+        return int(self.contract.functions.getLockupPeriodEndTimestamp(address).call())
 
-    def get_time_of_next_vest(self, address: str) -> int:
-        return self.contract.functions.getTimeOfNextVest(address).call()
+    def get_time_of_next_vest(self, address: ChecksumAddress) -> int:
+        return int(self.contract.functions.getTimeOfNextVest(address).call())
+
+    def _to_plan(self, untyped_plan: Dict[str, Any]) -> Plan:
+        return Plan({
+            'totalVestingDuration': int(untyped_plan['totalVestingDuration']),
+            'vestingCliff': int(untyped_plan['vestingCliff']),
+            'vestingIntervalTimeUnit': TimeUnit(untyped_plan['vestingIntervalTimeUnit']),
+            'vestingInterval': int(untyped_plan['vestingInterval']),
+            'isDelegationAllowed': bool(untyped_plan['isDelegationAllowed']),
+            'isTerminatable': bool(untyped_plan['isTerminatable'])
+        })
+
+    def _to_beneficiary_plan(self, untyped_beneficiary_plan: Dict[str, Any]) -> BeneficiaryPlan:
+        return BeneficiaryPlan({
+            'status': BeneficiaryStatus(untyped_beneficiary_plan['status']),
+            'statusName': str(untyped_beneficiary_plan['statusName']),
+            'planId': PlanId(untyped_beneficiary_plan['planId']),
+            'startMonth': int(untyped_beneficiary_plan['startMonth']),
+            'fullAmount': Wei(untyped_beneficiary_plan['fullAmount']),
+            'amountAfterLockup': Wei(untyped_beneficiary_plan['amountAfterLockup'])
+        })
```

### Comparing `skale.py-7.dev11/skale/contracts/allocator/escrow.py` & `skale.py-7.dev12/skale/contracts/allocator/escrow.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,61 +14,84 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 """ SKALE Allocator Core Escrow methods """
 
+from __future__ import annotations
 import functools
+from typing import Any, Callable, TYPE_CHECKING
 
-from skale.contracts.base_contract import BaseContract, transaction_method
+from eth_typing import ChecksumAddress
+from web3.contract.contract import ContractFunction
+from web3.types import Wei
+
+from skale.contracts.allocator_contract import AllocatorContract
+from skale.contracts.base_contract import transaction_method
 from skale.transactions.result import TxRes
+from skale.types.delegation import DelegationId
+from skale.types.validator import ValidatorId
+
+if TYPE_CHECKING:
+    from skale.contracts.allocator.allocator import Allocator
 
 
-def beneficiary_escrow(transaction):
+def beneficiary_escrow(transaction: Callable[..., TxRes]) -> Callable[..., TxRes]:
     @functools.wraps(transaction)
-    def wrapper(self, *args, beneficiary_address, **kwargs):
+    def wrapper(
+            self: AllocatorContract,
+            *args: Any,
+            beneficiary_address: ChecksumAddress,
+            **kwargs: Any
+    ) -> TxRes:
         self.contract = self.skale.instance.get_contract('Escrow', beneficiary_address)
         return transaction(self, *args, **kwargs)
     return wrapper
 
 
-class Escrow(BaseContract):
+class Escrow(AllocatorContract):
     @property
     @functools.lru_cache()
-    def allocator(self):
+    def allocator(self) -> Allocator:
         return self.skale.allocator
 
-    def init_contract(self, skale, address, abi) -> None:
-        self.contract = None
+    def init_contract(self, *args: Any) -> None:
+        self.contract = self.allocator.contract
 
     @beneficiary_escrow
     @transaction_method
-    def retrieve(self) -> TxRes:
+    def retrieve(self) -> ContractFunction:
         """Allows Holder to retrieve vested tokens from the Escrow contract
 
         :returns: Transaction results
         :rtype: TxRes
         """
         return self.contract.functions.retrieve()
 
     @beneficiary_escrow
     @transaction_method
-    def retrieve_after_termination(self, address: str) -> TxRes:
+    def retrieve_after_termination(self, address: ChecksumAddress) -> ContractFunction:
         """Allows Core Owner to retrieve remaining transferrable escrow balance
         after Core holder termination. Slashed tokens are non-transferable
 
         :returns: Transaction results
         :rtype: TxRes
         """
         return self.contract.functions.retrieveAfterTermination(address)
 
     @beneficiary_escrow
     @transaction_method
-    def delegate(self, validator_id: int, amount: int, delegation_period: int, info: str) -> TxRes:
+    def delegate(
+            self,
+            validator_id: ValidatorId,
+            amount: Wei,
+            delegation_period: int,
+            info: str
+    ) -> ContractFunction:
         """Allows Core holder to propose a delegation to a validator
 
         :param validator_id: ID of the validator to delegate tokens
         :type validator_id: int
         :param amount: Amount of tokens to delegate
         :type amount: int
         :param delegation_period: Period of delegation
@@ -78,42 +101,42 @@
         :returns: Transaction results
         :rtype: TxRes
         """
         return self.contract.functions.delegate(validator_id, amount, delegation_period, info)
 
     @beneficiary_escrow
     @transaction_method
-    def request_undelegation(self, delegation_id: int) -> TxRes:
+    def request_undelegation(self, delegation_id: DelegationId) -> ContractFunction:
         """Allows Holder and Owner to request undelegation. Only Owner can
         request undelegation after Core holder is deactivated (upon holder termination)
 
         :param delegation_id: ID of the delegation
         :type delegation_id: int
         :returns: Transaction results
         :rtype: TxRes
         """
         return self.contract.functions.requestUndelegation(delegation_id)
 
     @beneficiary_escrow
     @transaction_method
-    def withdraw_bounty(self, validator_id: int, to: str) -> TxRes:
+    def withdraw_bounty(self, validator_id: ValidatorId, to: ChecksumAddress) -> ContractFunction:
         """Allows Beneficiary and Vesting Owner to withdraw earned bounty.
 
         :param validator_id: ID of the validator
         :type validator_id: int
         :param to: Recipient address
         :type to: str
         :returns: Transaction results
         :rtype: TxRes
         """
         return self.contract.functions.withdrawBounty(validator_id, to)
 
     @beneficiary_escrow
     @transaction_method
-    def cancel_pending_delegation(self, delegation_id: int) -> TxRes:
+    def cancel_pending_delegation(self, delegation_id: DelegationId) -> ContractFunction:
         """Cancel pending delegation request.
 
         :param delegation_id: ID of the delegation to cancel
         :type delegation_id: int
         :returns: Transaction results
         :rtype: TxRes
         """
```

### Comparing `skale.py-7.dev11/skale/contracts/base_contract.py` & `skale.py-7.dev12/skale/contracts/base_contract.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,74 +13,118 @@
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 """ SKALE base contract class """
-
+from __future__ import annotations
 import logging
 from functools import wraps
-from typing import Dict, Optional
+from typing import Any, Callable, TYPE_CHECKING, Generic, TypeVar
 
+from eth_typing import ChecksumAddress
 from web3 import Web3
+from web3.contract.contract import ContractFunction
+from web3.types import ABI, Nonce, Wei
 
 import skale.config as config
-from skale.transactions.result import TxRes
-from skale.transactions.tools import make_dry_run_call, transaction_from_method, TxStatus
+from skale.transactions.result import TxRes, TxStatus
+from skale.transactions.tools import make_dry_run_call, transaction_from_method
 from skale.utils.web3_utils import (
     DEFAULT_BLOCKS_TO_WAIT,
     get_eth_nonce,
     MAX_WAITING_TIME,
     wait_for_confirmation_blocks
 )
 
+from skale.skale_base import SkaleBase
 from skale.utils.helper import to_camel_case
 
+if TYPE_CHECKING:
+    pass
+
 
 logger = logging.getLogger(__name__)
 
 
-def transaction_method(transaction):
+SkaleType = TypeVar('SkaleType', bound=SkaleBase)
+
+
+class BaseContract(Generic[SkaleType]):
+    def __init__(
+            self,
+            skale: SkaleType,
+            name: str,
+            address: ChecksumAddress | str | bytes,
+            abi: ABI
+    ):
+        self.skale = skale
+        self.name = name
+        self.address = Web3.to_checksum_address(address)
+        self.init_contract(skale, self.address, abi)
+
+    def init_contract(self, skale: SkaleBase, address: ChecksumAddress, abi: ABI) -> None:
+        self.contract = skale.web3.eth.contract(address=address, abi=abi)
+
+    def __getattr__(self, attr: str) -> Callable[..., Any]:
+        """Fallback for contract calls"""
+        logger.debug("Calling contract function: %s", attr)
+
+        def wrapper(*args: Any, **kw: Any) -> Any:
+            logger.debug('called with %r and %r' % (args, kw))
+            camel_case_fn_name = to_camel_case(attr)
+            if hasattr(self.contract.functions, camel_case_fn_name):
+                return getattr(self.contract.functions,
+                               camel_case_fn_name)(*args, **kw).call()
+            if hasattr(self.contract.functions, attr):
+                return getattr(self.contract.functions,
+                               attr)(*args, **kw).call()
+            raise AttributeError(attr)
+        return wrapper
+
+
+def transaction_method(transaction: Callable[..., ContractFunction]) -> Callable[..., TxRes]:
     @wraps(transaction)
     def wrapper(
-        self,
-        *args,
-        wait_for=True,
-        blocks_to_wait=DEFAULT_BLOCKS_TO_WAIT,
-        timeout=MAX_WAITING_TIME,
-        gas_limit=None,
-        gas_price=None,
-        nonce=None,
-        max_fee_per_gas=None,
-        max_priority_fee_per_gas=None,
-        value=0,
-        dry_run_only=False,
-        skip_dry_run=False,
-        raise_for_status=True,
-        multiplier=None,
-        priority=None,
-        confirmation_blocks=0,
-        meta: Optional[Dict] = None,
-        **kwargs
-    ):
+        self: BaseContract[SkaleType],
+        *args: Any,
+        wait_for: bool = True,
+        blocks_to_wait: int = DEFAULT_BLOCKS_TO_WAIT,
+        timeout: int = MAX_WAITING_TIME,
+        gas_limit: int | None = None,
+        gas_price: int | None = None,
+        nonce: Nonce | None = None,
+        max_fee_per_gas: int | None = None,
+        max_priority_fee_per_gas: int | None = None,
+        value: Wei = Wei(0),
+        dry_run_only: bool = False,
+        skip_dry_run: bool = False,
+        raise_for_status: bool = True,
+        multiplier: float | None = None,
+        priority: int | None = None,
+        confirmation_blocks: int = 0,
+        **kwargs: Any
+    ) -> TxRes:
         method = transaction(self, *args, **kwargs)
 
         nonce = get_eth_nonce(self.skale.web3, self.skale.wallet.address)
 
         call_result, tx_hash, receipt = None, None, None
         should_dry_run = not skip_dry_run and not config.DISABLE_DRY_RUN
 
+        dry_run_success = False
         if should_dry_run:
             call_result = make_dry_run_call(self.skale, method, gas_limit, value)
             if call_result.status == TxStatus.SUCCESS:
-                gas_limit = gas_limit or call_result.data['gas']
+                gas_limit = gas_limit or int(call_result.data['gas'])
+                dry_run_success = True
 
         should_send = not dry_run_only and \
-            (not should_dry_run or call_result.status == TxStatus.SUCCESS)
+            (not should_dry_run or dry_run_success)
 
         if should_send:
             gas_limit = gas_limit or config.DEFAULT_GAS_LIMIT
             gas_price = gas_price or config.DEFAULT_GAS_PRICE_WEI or self.skale.gas_price
             tx = transaction_from_method(
                 method=method,
                 gas_limit=gas_limit,
@@ -91,53 +135,24 @@
                 value=value
             )
             method_name = f'{self.name}.{method.abi.get("name")}'
             tx_hash = self.skale.wallet.sign_and_send(
                 tx,
                 multiplier=multiplier,
                 priority=priority,
-                method=method_name,
-                meta=meta
+                method=method_name
             )
 
-        should_wait = tx_hash is not None and wait_for
-        if should_wait:
+        if tx_hash is not None and wait_for:
             receipt = self.skale.wallet.wait(tx_hash)
 
         should_confirm = receipt is not None and confirmation_blocks > 0
         if should_confirm:
             wait_for_confirmation_blocks(self.skale.web3, confirmation_blocks)
 
         tx_res = TxRes(call_result, tx_hash, receipt)
 
         if raise_for_status:
             tx_res.raise_for_status()
         return tx_res
 
     return wrapper
-
-
-class BaseContract:
-    def __init__(self, skale, name, address, abi):
-        self.skale = skale
-        self.name = name
-        self.address = Web3.to_checksum_address(address)
-        self.init_contract(skale, address, abi)
-
-    def init_contract(self, skale, address, abi) -> None:
-        self.contract = skale.web3.eth.contract(address=address, abi=abi)
-
-    def __getattr__(self, attr):
-        """Fallback for contract calls"""
-        logger.debug("Calling contract function: %s", attr)
-
-        def wrapper(*args, **kw):
-            logger.debug('called with %r and %r' % (args, kw))
-            camel_case_fn_name = to_camel_case(attr)
-            if hasattr(self.contract.functions, camel_case_fn_name):
-                return getattr(self.contract.functions,
-                               camel_case_fn_name)(*args, **kw).call()
-            if hasattr(self.contract.functions, attr):
-                return getattr(self.contract.functions,
-                               attr)(*args, **kw).call()
-            raise AttributeError(attr)
-        return wrapper
```

### Comparing `skale.py-7.dev11/skale/contracts/contract_manager.py` & `skale.py-7.dev12/skale/contracts/manager/contract_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,20 +15,22 @@
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 """ SKALE Contract manager class """
 
 from Crypto.Hash import keccak
+from eth_typing import ChecksumAddress
+from web3 import Web3
 
-from skale.contracts.base_contract import BaseContract
+from skale.contracts.skale_manager_contract import SkaleManagerContract
 from skale.utils.helper import add_0x_prefix
 
 
-class ContractManager(BaseContract):
-    def get_contract_address(self, name):
+class ContractManager(SkaleManagerContract):
+    def get_contract_address(self, name: str) -> ChecksumAddress:
         contract_hash = add_0x_prefix(self.get_contract_hash_by_name(name))
-        return self.contract.functions.contracts(contract_hash).call()
+        return Web3.to_checksum_address(self.contract.functions.contracts(contract_hash).call())
 
-    def get_contract_hash_by_name(self, name):
+    def get_contract_hash_by_name(self, name: str) -> str:
         keccak_hash = keccak.new(data=name.encode("utf8"), digest_bits=256)
         return keccak_hash.hexdigest()
```

### Comparing `skale.py-7.dev11/skale/contracts/ima/linker.py` & `skale.py-7.dev12/skale/contracts/skale_manager_contract.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,22 +12,13 @@
 #   SKALE.py is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
+from skale.contracts.base_contract import BaseContract
+from skale.skale_manager import SkaleManager
 
-from skale.contracts.base_contract import BaseContract, transaction_method
 
-
-class Linker(BaseContract):
-    @transaction_method
-    def connect_schain(
-            self,
-            schain_name: str,
-            mainnet_contracts: list
-    ):
-        return self.contract.functions.connectSchain(
-            schain_name,
-            mainnet_contracts
-        )
+class SkaleManagerContract(BaseContract[SkaleManager]):
+    pass
```

### Comparing `skale.py-7.dev11/skale/contracts/manager/bounty_v2.py` & `skale.py-7.dev12/skale/utils/contract_info.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 #   -*- coding: utf-8 -*-
 #
 #   This file is part of SKALE.py
 #
-#   Copyright (C) 2021 SKALE Labs
+#   Copyright (C) 2019-Present SKALE Labs
 #
 #   SKALE.py is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU Affero General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   SKALE.py is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
+""" Contract info utilities """
 
-from skale.contracts.base_contract import BaseContract, transaction_method
-from skale.transactions.result import TxRes
+from __future__ import annotations
+from typing import Generic, NamedTuple, Type, TYPE_CHECKING
 
+from skale.contracts.base_contract import SkaleType
 
-class BountyV2(BaseContract):
-    @transaction_method
-    def grant_role(self, role: bytes, owner: str) -> TxRes:
-        return self.contract.functions.grantRole(role, owner)
+if TYPE_CHECKING:
+    from skale.contracts.base_contract import BaseContract
+    from skale.utils.contract_types import ContractTypes
 
-    def has_role(self, role: bytes, address: str) -> bool:
-        return self.contract.functions.hasRole(role, address).call()
 
-    def bounty_reduction_manager_role(self):
-        return self.contract.functions.BOUNTY_REDUCTION_MANAGER_ROLE().call()
+class ContractInfo(NamedTuple, Generic[SkaleType]):
+    name: str
+    contract_name: str
+    contract_class: Type[BaseContract[SkaleType]]
+    type: ContractTypes
+    upgradeable: bool
```

### Comparing `skale.py-7.dev11/skale/contracts/manager/constants_holder.py` & `skale.py-7.dev12/skale/contracts/manager/constants_holder.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,86 +13,89 @@
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
-from skale.contracts.base_contract import BaseContract, transaction_method
-from skale.transactions.result import TxRes
+from eth_typing import ChecksumAddress
+from web3.contract.contract import ContractFunction
 
+from skale.contracts.base_contract import transaction_method
+from skale.contracts.skale_manager_contract import SkaleManagerContract
 
-class ConstantsHolder(BaseContract):
+
+class ConstantsHolder(SkaleManagerContract):
     @transaction_method
-    def set_periods(self, new_reward_period, new_delta_period):
+    def set_periods(self, new_reward_period: int, new_delta_period: int) -> ContractFunction:
         return self.contract.functions.setPeriods(
             new_reward_period,
             new_delta_period
         )
 
-    def get_reward_period(self):
-        return self.contract.functions.rewardPeriod().call()
+    def get_reward_period(self) -> int:
+        return int(self.contract.functions.rewardPeriod().call())
 
-    def get_delta_period(self):
-        return self.contract.functions.deltaPeriod().call()
+    def get_delta_period(self) -> int:
+        return int(self.contract.functions.deltaPeriod().call())
 
     @transaction_method
-    def set_check_time(self, new_check_time):
+    def set_check_time(self, new_check_time: int) -> ContractFunction:
         return self.contract.functions.setCheckTime(new_check_time)
 
-    def get_check_time(self):
-        return self.contract.functions.checkTime().call()
+    def get_check_time(self) -> int:
+        return int(self.contract.functions.checkTime().call())
 
     @transaction_method
-    def set_latency(self, new_allowable_latency):
+    def set_latency(self, new_allowable_latency: int) -> ContractFunction:
         return self.contract.functions.setLatency(new_allowable_latency)
 
-    def get_latency(self):
-        return self.contract.functions.allowableLatency().call()
+    def get_latency(self) -> int:
+        return int(self.contract.functions.allowableLatency().call())
 
-    def get_first_delegation_month(self):
-        return self.contract.functions.firstDelegationsMonth().call()
+    def get_first_delegation_month(self) -> int:
+        return int(self.contract.functions.firstDelegationsMonth().call())
 
     def msr(self) -> int:
         """Minimum staking requirement to create a node.
 
         :returns: MSR (in wei)
         :rtype: int
         """
-        return self.contract.functions.msr().call()
+        return int(self.contract.functions.msr().call())
 
     @transaction_method
-    def _set_msr(self, new_msr: int) -> None:
+    def _set_msr(self, new_msr: int) -> ContractFunction:
         """For internal usage only"""
         return self.contract.functions.setMSR(new_msr)
 
     def get_launch_timestamp(self) -> int:
-        return self.contract.functions.launchTimestamp().call()
+        return int(self.contract.functions.launchTimestamp().call())
 
     @transaction_method
-    def set_launch_timestamp(self, launch_timestamp: int):
+    def set_launch_timestamp(self, launch_timestamp: int) -> ContractFunction:
         return self.contract.functions.setLaunchTimestamp(launch_timestamp)
 
     @transaction_method
-    def set_rotation_delay(self, rotation_delay: int) -> None:
+    def set_rotation_delay(self, rotation_delay: int) -> ContractFunction:
         """For internal usage only"""
         return self.contract.functions.setRotationDelay(rotation_delay)
 
     def get_rotation_delay(self) -> int:
-        return self.contract.functions.rotationDelay().call()
+        return int(self.contract.functions.rotationDelay().call())
 
     def get_dkg_timeout(self) -> int:
-        return self.contract.functions.complaintTimeLimit().call()
+        return int(self.contract.functions.complaintTimeLimit().call())
 
     @transaction_method
-    def set_complaint_timelimit(self, complaint_timelimit: int):
+    def set_complaint_timelimit(self, complaint_timelimit: int) -> ContractFunction:
         return self.contract.functions.setComplaintTimeLimit(complaint_timelimit)
 
     @transaction_method
-    def grant_role(self, role: bytes, address: str) -> TxRes:
+    def grant_role(self, role: bytes, address: ChecksumAddress) -> ContractFunction:
         return self.contract.functions.grantRole(role, address)
 
     def constants_holder_role(self) -> bytes:
-        return self.contract.functions.CONSTANTS_HOLDER_MANAGER_ROLE().call()
+        return bytes(self.contract.functions.CONSTANTS_HOLDER_MANAGER_ROLE().call())
 
-    def has_role(self, role: bytes, address: str) -> bool:
-        return self.contract.functions.hasRole(role, address).call()
+    def has_role(self, role: bytes, address: ChecksumAddress) -> bool:
+        return bool(self.contract.functions.hasRole(role, address).call())
```

### Comparing `skale.py-7.dev11/skale/contracts/manager/delegation/delegation_controller.py` & `skale.py-7.dev12/skale/contracts/manager/delegation/delegation_controller.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,124 +13,151 @@
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
-from skale.contracts.base_contract import BaseContract, transaction_method
+from typing import Any, Dict, List
+
+from eth_typing import ChecksumAddress
+from web3.contract.contract import ContractFunction
+from web3.types import Wei
+
+from skale.contracts.base_contract import transaction_method
+from skale.contracts.skale_manager_contract import SkaleManagerContract
+from skale.types.delegation import Delegation, DelegationId, DelegationStatus, FullDelegation
+from skale.types.validator import ValidatorId
 from skale.utils.helper import format_fields
-from skale.transactions.result import TxRes
-from skale.dataclasses.delegation_status import DelegationStatus
 
 
 FIELDS = [
     'address', 'validator_id', 'amount', 'delegation_period', 'created',
     'started', 'finished', 'info'
 ]
 
 
-class DelegationController(BaseContract):
+class DelegationController(SkaleManagerContract):
     """Wrapper for DelegationController.sol functions"""
 
     @format_fields(FIELDS)
-    def get_delegation(self, delegation_id: int) -> dict:
+    def get_untyped_delegation(self, delegation_id: DelegationId) -> List[Any]:
         """Returns delegation structure.
 
         :returns: Info about delegation request
-        :rtype: dict
+        :rtype: list
         """
         return self.__raw_get_delegation(delegation_id)
 
-    def get_delegation_full(self, delegation_id: int) -> dict:
+    def get_delegation(self, delegation_id: DelegationId) -> Delegation:
+        delegation = self.get_untyped_delegation(delegation_id)
+        if delegation is None:
+            raise ValueError("Can't get delegation with id ", delegation_id)
+        if isinstance(delegation, dict):
+            return self._to_delegation(delegation)
+        if isinstance(delegation, list):
+            return self._to_delegation(delegation[0])
+        raise TypeError(delegation_id)
+
+    def get_delegation_full(self, delegation_id: DelegationId) -> FullDelegation:
         """Returns delegation structure with ID and status fields.
 
         :returns: Info about delegation request
         :rtype: dict
         """
         delegation = self.get_delegation(delegation_id)
-        delegation['id'] = delegation_id
-        delegation['status'] = self._get_delegation_status(delegation_id)
-        return delegation
+        return FullDelegation({
+            'id': delegation_id,
+            'status': self._get_delegation_status(delegation_id),
+            **delegation
+        })
 
-    def __raw_get_delegation(self, delegation_id: int) -> list:
+    def __raw_get_delegation(self, delegation_id: DelegationId) -> List[Any]:
         """Returns raw delegation fields.
 
         :returns: Info about delegation request
         :rtype: list
         """
-        return self.contract.functions.getDelegation(delegation_id).call()
+        return list(self.contract.functions.getDelegation(delegation_id).call())
 
-    def _get_delegation_ids_by_validator(self, validator_id: int) -> list:
+    def _get_delegation_ids_by_validator(self, validator_id: ValidatorId) -> List[DelegationId]:
         delegation_ids_len = self._get_delegation_ids_len_by_validator(
             validator_id)
         return [
-            self.contract.functions.delegationsByValidator(
-                validator_id, _id).call()
+            DelegationId(
+                self.contract.functions.delegationsByValidator(validator_id, _id).call()
+            )
             for _id in range(delegation_ids_len)
         ]
 
-    def _get_delegation_ids_by_holder(self, address: str) -> list:
+    def _get_delegation_ids_by_holder(self, address: ChecksumAddress) -> List[DelegationId]:
         delegation_ids_len = self._get_delegation_ids_len_by_holder(address)
         return [
-            self.contract.functions.delegationsByHolder(address, _id).call()
+            DelegationId(
+                self.contract.functions.delegationsByHolder(address, _id).call()
+            )
             for _id in range(delegation_ids_len)
         ]
 
-    def _get_delegation_ids_len_by_validator(self, validator_id: int) -> list:
-        return self.contract.functions.getDelegationsByValidatorLength(validator_id).call()
+    def _get_delegation_ids_len_by_validator(self, validator_id: ValidatorId) -> int:
+        return int(self.contract.functions.getDelegationsByValidatorLength(validator_id).call())
 
-    def _get_delegation_ids_len_by_holder(self, address: str) -> list:
-        return self.contract.functions.getDelegationsByHolderLength(address).call()
+    def _get_delegation_ids_len_by_holder(self, address: ChecksumAddress) -> int:
+        return int(self.contract.functions.getDelegationsByHolderLength(address).call())
 
-    def _get_delegation_state_index(self, delegation_id: int) -> str:
-        return self.contract.functions.getState(delegation_id).call()
+    def _get_delegation_state_index(self, delegation_id: DelegationId) -> int:
+        return int(self.contract.functions.getState(delegation_id).call())
 
-    def _get_delegation_status(self, delegation_id: int) -> str:
+    def _get_delegation_status(self, delegation_id: DelegationId) -> DelegationStatus:
         index = self._get_delegation_state_index(delegation_id)
-        return DelegationStatus(index).name
+        return DelegationStatus(index)
 
-    def get_all_delegations(self, delegation_ids: list) -> list:
+    def get_all_delegations(self, delegation_ids: List[DelegationId]) -> List[FullDelegation]:
         """Returns list of formatted delegations with particular status.
 
         :param delegation_ids: List of delegation IDs
         :type address: list
         :returns: List of formatted delegations
         :rtype: list
         """
         return [
             self.skale.delegation_controller.get_delegation_full(_id)
             for _id in delegation_ids
         ]
 
-    def get_all_delegations_by_holder(self, address: str) -> list:
+    def get_all_delegations_by_holder(self, address: ChecksumAddress) -> List[FullDelegation]:
         """Returns list of formatted delegations for token holder.
 
         :param address: Ethereum address
         :type address: str
         :returns: List of formatted delegation requests
         :rtype: list
         """
         delegation_ids = self._get_delegation_ids_by_holder(address)
         return self.get_all_delegations(delegation_ids)
 
-    def get_all_delegations_by_validator(self, validator_id: int) -> list:
+    def get_all_delegations_by_validator(self, validator_id: ValidatorId) -> List[FullDelegation]:
         """Returns list of formatted delegations for validator.
 
         :param validator_id: ID of the validator
         :type address: int
         :returns: List of formatted delegations
         :rtype: list
         """
-        validator_id = int(validator_id)
         delegation_ids = self._get_delegation_ids_by_validator(validator_id)
         return self.get_all_delegations(delegation_ids)
 
     @transaction_method
-    def delegate(self, validator_id: int, amount: int, delegation_period: int, info: str) -> TxRes:
+    def delegate(
+            self,
+            validator_id: ValidatorId,
+            amount: Wei,
+            delegation_period: int,
+            info: str
+    ) -> ContractFunction:
         """Creates request to delegate amount of tokens to validator_id.
 
         :param validator_id: ID of the validator to delegate tokens
         :type validator_id: int
         :param amount: Amount of tokens to delegate
         :type amount: int
         :param delegation_period: Period of delegation
@@ -139,72 +166,84 @@
         :type info: str
         :returns: Transaction results
         :rtype: TxRes
         """
         return self.contract.functions.delegate(validator_id, amount, delegation_period, info)
 
     @transaction_method
-    def accept_pending_delegation(self, delegation_id: int) -> TxRes:
+    def accept_pending_delegation(self, delegation_id: DelegationId) -> ContractFunction:
         """Accepts a pending delegation by delegation ID.
 
         :param delegation_id: Delegation ID to accept
         :type delegation_id: int
         :returns: Transaction results
         :rtype: TxRes
         """
         return self.contract.functions.acceptPendingDelegation(delegation_id)
 
     @transaction_method
-    def cancel_pending_delegation(self, delegation_id: int) -> TxRes:
+    def cancel_pending_delegation(self, delegation_id: DelegationId) -> ContractFunction:
         """Cancel pending delegation request.
 
         :param delegation_id: ID of the delegation to cancel
         :type delegation_id: int
         :returns: Transaction results
         :rtype: TxRes
         """
         return self.contract.functions.cancelPendingDelegation(delegation_id)
 
     @transaction_method
-    def request_undelegation(self, delegation_id: int) -> TxRes:
+    def request_undelegation(self, delegation_id: DelegationId) -> ContractFunction:
         """ This method is  for undelegating request in the end of
             delegation period (3/6/12 months)
 
         :param delegation_id: ID of the delegation to undelegate
         :type delegation_id: int
         :returns: Transaction results
         :rtype: TxRes
         """
         return self.contract.functions.requestUndelegation(delegation_id)
 
-    def get_delegated_to_validator_now(self, validator_id: int) -> int:
+    def get_delegated_to_validator_now(self, validator_id: ValidatorId) -> Wei:
         """Amount of delegated tokens to the validator
 
         :param validator_id: ID of the validator
         :type validator_id: int
         :returns: Amount of delegated tokens
         :rtype: int
         """
-        return self.contract.functions.getAndUpdateDelegatedToValidatorNow(validator_id).call()
+        return Wei(self.contract.functions.getAndUpdateDelegatedToValidatorNow(validator_id).call())
 
-    def get_delegated_to_validator(self, validator_id: int, month: int) -> int:
+    def get_delegated_to_validator(self, validator_id: ValidatorId, month: int) -> Wei:
         """Amount of delegated tokens to the validator unil month
 
         :param validator_id: ID of the validator
         :type validator_id: int
         :param month: last requested month
         :type month: int
         :returns: Amount of delegated tokens
         :rtype: int
         """
 
-        return self.contract.functions.getDelegatedToValidator(validator_id, month).call()
+        return Wei(self.contract.functions.getDelegatedToValidator(validator_id, month).call())
 
-    def get_delegated_amount(self, address: str) -> int:
+    def get_delegated_amount(self, address: ChecksumAddress) -> Wei:
         """Amount of delegated tokens by token holder
 
         :param address: Token holder address
         :type address: str
         :returns: Amount of delegated tokens
         :rtype: int
         """
-        return self.contract.functions.getAndUpdateDelegatedAmount(address).call()
+        return Wei(self.contract.functions.getAndUpdateDelegatedAmount(address).call())
+
+    def _to_delegation(self, delegation: Dict[str, Any]) -> Delegation:
+        return Delegation({
+            'address': ChecksumAddress(delegation['address']),
+            'validator_id': ValidatorId(delegation['validator_id']),
+            'amount': Wei(delegation['amount']),
+            'delegation_period': int(delegation['delegation_period']),
+            'created': int(delegation['created']),
+            'started': int(delegation['started']),
+            'finished': int(delegation['finished']),
+            'info': str(delegation['info'])
+        })
```

### Comparing `skale.py-7.dev11/skale/contracts/manager/delegation/delegation_period_manager.py` & `skale.py-7.dev12/skale/contracts/manager/delegation/delegation_period_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,36 +13,39 @@
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
-from skale.contracts.base_contract import BaseContract, transaction_method
-from skale.transactions.result import TxRes
+from eth_typing import ChecksumAddress
+from web3.contract.contract import ContractFunction
 
+from skale.contracts.base_contract import transaction_method
+from skale.contracts.skale_manager_contract import SkaleManagerContract
 
-class DelegationPeriodManager(BaseContract):
+
+class DelegationPeriodManager(SkaleManagerContract):
     """Wrapper for DelegationPeriodManager.sol functions"""
 
     @transaction_method
     def set_delegation_period(self, months_count: int,
-                              stake_multiplier: int) -> None:
+                              stake_multiplier: int) -> ContractFunction:
         return self.contract.functions.setDelegationPeriod(
             monthsCount=months_count,
             stakeMultiplier=stake_multiplier
         )
 
     def is_delegation_period_allowed(self, months_count: int) -> bool:
-        return self.contract.functions.isDelegationPeriodAllowed(
+        return bool(self.contract.functions.isDelegationPeriodAllowed(
             monthsCount=months_count
-        ).call()
+        ).call())
 
     @transaction_method
-    def grant_role(self, role: bytes, address: str) -> TxRes:
+    def grant_role(self, role: bytes, address: ChecksumAddress) -> ContractFunction:
         return self.contract.functions.grantRole(role, address)
 
     def delegation_period_setter_role(self) -> bytes:
-        return self.contract.functions.DELEGATION_PERIOD_SETTER_ROLE().call()
+        return bytes(self.contract.functions.DELEGATION_PERIOD_SETTER_ROLE().call())
 
-    def has_role(self, role: bytes, address: str) -> bool:
-        return self.contract.functions.hasRole(role, address).call()
+    def has_role(self, role: bytes, address: ChecksumAddress) -> bool:
+        return bool(self.contract.functions.hasRole(role, address).call())
```

### Comparing `skale.py-7.dev11/skale/contracts/manager/delegation/distributor.py` & `skale.py-7.dev12/skale/contracts/manager/delegation/distributor.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,74 +14,89 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
 from functools import wraps
+from typing import Any, Callable, Tuple, TypedDict
 
-from skale.contracts.base_contract import BaseContract, transaction_method
-from skale.transactions.result import TxRes
+from eth_typing import ChecksumAddress
+from web3.contract.contract import ContractFunction
+from web3.types import Wei
 
+from skale.contracts.base_contract import transaction_method
+from skale.contracts.skale_manager_contract import SkaleManagerContract
+from skale.types.validator import ValidatorId
 
-def formatter(method):
+
+class EarnedData(TypedDict):
+    earned: Wei
+    end_month: int
+
+
+def formatter(method: Callable[..., Tuple[Wei, int]]) -> Callable[..., EarnedData]:
     @wraps(method)
-    def wrapper(self, *args, **kwargs):
+    def wrapper(self: SkaleManagerContract, *args: Any, **kwargs: Any) -> EarnedData:
         res = method(self, *args, **kwargs)
-        return {
+        return EarnedData({
             'earned': res[0],
             'end_month': res[1],
-        }
+        })
     return wrapper
 
 
-class Distributor(BaseContract):
+class Distributor(SkaleManagerContract):
     """Wrapper for Distributor.sol functions"""
 
     @formatter
-    def get_earned_bounty_amount(self, validator_id: int, address: str) -> dict:
+    def get_earned_bounty_amount(
+            self,
+            validator_id: ValidatorId,
+            address: ChecksumAddress
+    ) -> Tuple[Wei, int]:
         """Get earned bounty amount for the validator
 
         :param validator_id: ID of the validator
         :type validator_id: int
         :returns: Earned bounty amount and end month
         :rtype: dict
         """
-        return self.contract.functions.getAndUpdateEarnedBountyAmount(validator_id).call({
+        return tuple(self.contract.functions.getAndUpdateEarnedBountyAmount(validator_id).call({
             'from': address
-        })
+        }))
 
     @formatter
-    def get_earned_fee_amount(self, address: str) -> dict:
+    def get_earned_fee_amount(self, address: str) -> Tuple[Wei, int]:
         """Get earned fee amount for the address
 
         :param address: Address of the validator
         :type address: str
         :returns: Earned bounty amount and end month
         :rtype: dict
         """
-        return self.contract.functions.getEarnedFeeAmount().call({
+        return tuple(self.contract.functions.getEarnedFeeAmount().call({
             'from': address
-        })
+        }))
 
     @transaction_method
-    def withdraw_bounty(self, validator_id: int, to: str) -> TxRes:
+    def withdraw_bounty(self, validator_id: ValidatorId, to: ChecksumAddress) -> ContractFunction:
         """Withdraw earned bounty to specified address
 
         :param validator_id: ID of the validator
         :type validator_id: int
         :param to: Address to transfer bounty
         :type to: str
         :returns: Transaction results
         :rtype: TxRes
         """
         return self.contract.functions.withdrawBounty(validator_id, to)
 
     @transaction_method
-    def withdraw_fee(self, to: str) -> TxRes:
+    def withdraw_fee(self, to: ChecksumAddress) -> ContractFunction:
         """Withdraw earned fee to specified address
 
         :param to: Address to transfer bounty
         :type to: str
         :returns: Transaction results
         :rtype: TxRes
         """
```

### Comparing `skale.py-7.dev11/skale/contracts/manager/delegation/slashing_table.py` & `skale.py-7.dev12/skale/contracts/manager/delegation/slashing_table.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,39 @@
-from skale.contracts.base_contract import BaseContract, transaction_method
-from skale.transactions.result import TxRes
+from eth_typing import ChecksumAddress
+from web3.contract.contract import ContractFunction
+from web3.types import Wei
 
+from skale.contracts.base_contract import transaction_method
+from skale.contracts.skale_manager_contract import SkaleManagerContract
 
-class SlashingTable(BaseContract):
+
+class SlashingTable(SkaleManagerContract):
     """ Wrapper for SlashingTable.sol functions """
 
     @transaction_method
-    def set_penalty(self, offense, penalty) -> TxRes:
+    def set_penalty(self, offense: str, penalty: Wei) -> ContractFunction:
         """ Set slashing penalty
         :param offense: reason of slashing
         :type offense: str
         :param penalty: penalty value to set
         :type penalty: int
         :rtype: TxRes
         """
         return self.contract.functions.setPenalty(offense, penalty)
 
-    def get_penalty(self, offense) -> int:
+    def get_penalty(self, offense: str) -> Wei:
         """ Get slashing penalty value
         :param offense: reason of slashing
         :type offense: str
         :rtype: int
         """
-        return self.contract.functions.getPenalty(offense).call()
+        return Wei(self.contract.functions.getPenalty(offense).call())
 
     @transaction_method
-    def grant_role(self, role: bytes, address: str) -> TxRes:
+    def grant_role(self, role: bytes, address: ChecksumAddress) -> ContractFunction:
         return self.contract.functions.grantRole(role, address)
 
     def penalty_setter_role(self) -> bytes:
-        return self.contract.functions.PENALTY_SETTER_ROLE().call()
+        return bytes(self.contract.functions.PENALTY_SETTER_ROLE().call())
 
-    def has_role(self, role: bytes, address: str) -> bool:
-        return self.contract.functions.hasRole(role, address).call()
+    def has_role(self, role: bytes, address: ChecksumAddress) -> bool:
+        return bool(self.contract.functions.hasRole(role, address).call())
```

### Comparing `skale.py-7.dev11/skale/contracts/manager/delegation/token_state.py` & `skale.py-7.dev12/skale/contracts/manager/wallets.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 #   -*- coding: utf-8 -*-
 #
 #   This file is part of SKALE.py
 #
-#   Copyright (C) 2019-Present SKALE Labs
+#   Copyright (C) 2021-Present SKALE Labs
 #
 #   SKALE.py is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU Affero General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   SKALE.py is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
-from skale.contracts.base_contract import BaseContract, transaction_method
-from skale.transactions.result import TxRes
+from web3.contract.contract import ContractFunction
 
+from skale.contracts.base_contract import transaction_method
+from skale.contracts.skale_manager_contract import SkaleManagerContract
 
-class TokenState(BaseContract):
-    """Wrapper for TokenState.sol functions"""
 
-    def get_and_update_locked_amount(self, holder_address: str) -> int:
-        """This method is for check quantity of `freezed` tokens
-           :param holder_address: Address of the holder
-           :type holder_address: str
-           :returns:
-           :rtype: int
+class Wallets(SkaleManagerContract):
+    def get_validator_balance(self, validator_id: int) -> int:
+        """Returns SRW balance by validator id (in wei).
+
+        :returns: SRW balance (wei)
+        :rtype: int
         """
-        return self.contract.functions.getAndUpdateLockedAmount(holder_address).call()
+        return int(self.contract.functions.getValidatorBalance(validator_id).call())
 
     @transaction_method
-    def grant_role(self, role: bytes, owner: str) -> TxRes:
-        return self.contract.functions.grantRole(role, owner)
-
-    def has_role(self, role: bytes, address: str) -> bool:
-        return self.contract.functions.hasRole(role, address).call()
+    def recharge_validator_wallet(self, validator_id: int) -> ContractFunction:
+        """Pass value kwarg (in wei) to the function when calling it"""
+        return self.contract.functions.rechargeValidatorWallet(validator_id)
 
-    def locker_manager_role(self):
-        return self.contract.functions.LOCKER_MANAGER_ROLE().call()
+    @transaction_method
+    def withdraw_funds_from_validator_wallet(self, amount: int) -> ContractFunction:
+        return self.contract.functions.withdrawFundsFromValidatorWallet(amount)
```

### Comparing `skale.py-7.dev11/skale/contracts/manager/delegation/validator_service.py` & `skale.py-7.dev12/skale/contracts/manager/delegation/validator_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,105 +13,130 @@
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
+from typing import Any, Dict, List
+from eth_typing import ChecksumAddress
 from web3 import Web3
+from web3.contract.contract import ContractFunction
+from web3.types import Wei
 
-from skale.contracts.base_contract import BaseContract, transaction_method
+from skale.contracts.base_contract import transaction_method
+from skale.contracts.skale_manager_contract import SkaleManagerContract
+from skale.types.validator import Validator, ValidatorId, ValidatorWithId
 from skale.utils.helper import format_fields
 
-from skale.transactions.result import TxRes
-
 
 FIELDS = [
     'name', 'validator_address', 'requested_address', 'description', 'fee_rate',
     'registration_time', 'minimum_delegation_amount', 'accept_new_requests',
     'trusted'
 ]
 
 
-class ValidatorService(BaseContract):
+class ValidatorService(SkaleManagerContract):
     """Wrapper for ValidatorService.sol functions"""
 
-    def __get_raw(self, _id) -> list:
+    def __get_raw(self, _id: ValidatorId) -> List[Any]:
         """Returns raw validator info.
 
         :returns: Raw validator info
         :rtype: list
         """
-        return self.contract.functions.validators(_id).call()
+        return list(self.contract.functions.validators(_id).call())
 
     @format_fields(FIELDS)
-    def get(self, _id) -> dict:
+    def untyped_get(self, _id: ValidatorId) -> List[Any]:
         """Returns validator info.
 
         :returns: Validator info
         :rtype: dict
         """
         validator = self.__get_raw(_id)
         trusted = self._is_authorized_validator(_id)
         validator.append(trusted)
         return validator
 
-    def get_with_id(self, _id) -> dict:
+    def get(self, _id: ValidatorId) -> Validator:
+        untyped_validator = self.untyped_get(_id)
+        if untyped_validator is None:
+            raise ValueError('Validator with id ', _id, ' is missing')
+        if isinstance(untyped_validator, dict):
+            return self._to_validator(untyped_validator)
+        if isinstance(untyped_validator, list):
+            return self._to_validator(untyped_validator[0])
+        raise TypeError(_id)
+
+    def get_with_id(self, _id: ValidatorId) -> ValidatorWithId:
         """Returns validator info with ID.
 
         :returns: Validator info with ID
         :rtype: dict
         """
         validator = self.get(_id)
-        validator['id'] = _id
-        return validator
+        return ValidatorWithId({'id': _id, **validator})
 
-    def number_of_validators(self):
+    def number_of_validators(self) -> int:
         """Returns number of registered validators.
 
         :returns: List of validators
         :rtype: int
         """
-        return self.contract.functions.numberOfValidators().call()
+        return int(self.contract.functions.numberOfValidators().call())
 
-    def ls(self, trusted_only=False):
+    def ls(self, trusted_only: bool = False) -> List[ValidatorWithId]:
         """Returns list of registered validators.
 
         :returns: List of validators
         :rtype: list
         """
         number_of_validators = self.number_of_validators()
         validators = [
             self.get_with_id(val_id)
             for val_id in self.get_trusted_validator_ids()
         ] if trusted_only else [
-            self.get_with_id(val_id)
+            self.get_with_id(ValidatorId(val_id))
             for val_id in range(1, number_of_validators + 1)
         ]
         return validators
 
-    def get_linked_addresses_by_validator_address(self, address: str) -> list:
+    def get_linked_addresses_by_validator_address(
+            self,
+            address: ChecksumAddress
+    ) -> List[ChecksumAddress]:
         """Returns list of node addresses linked to the validator address.
 
         :returns: List of node addresses
         :rtype: list
         """
-        return self.contract.functions.getMyNodesAddresses().call({
-            'from': address
-        })
+        return [
+            Web3.to_checksum_address(address)
+            for address
+            in self.contract.functions.getMyNodesAddresses().call({'from': address})
+        ]
 
-    def get_linked_addresses_by_validator_id(self, validator_id: int) -> list:
+    def get_linked_addresses_by_validator_id(
+            self,
+            validator_id: ValidatorId
+    ) -> List[ChecksumAddress]:
         """Returns list of node addresses linked to the validator ID.
 
         :returns: List of node addresses
         :rtype: list
         """
-        return self.contract.functions.getNodeAddresses(validator_id).call()
+        return [
+            Web3.to_checksum_address(address)
+            for address
+            in self.contract.functions.getNodeAddresses(validator_id).call()
+        ]
 
-    def is_main_address(self, validator_address: str) -> bool:
+    def is_main_address(self, validator_address: ChecksumAddress) -> bool:
         """Checks if provided address is the main validator address
 
         :returns: True if provided address is the main validator address, otherwise False
         :rtype: bool
         """
         if not self.validator_address_exists(validator_address):
             return False
@@ -121,67 +146,71 @@
             validator_id = self.validator_id_by_address(validator_address)
             validator = self.get(validator_id)
         except Exception:
             return False
 
         return validator_address == validator['validator_address']
 
-    def validator_address_exists(self, validator_address: str) -> bool:
+    def validator_address_exists(self, validator_address: ChecksumAddress) -> bool:
         """Checks if there is a validator with provided address
 
         :returns: True if validator exists, otherwise False
         :rtype: bool
         """
-        return self.contract.functions.validatorAddressExists(validator_address).call()
+        return bool(self.contract.functions.validatorAddressExists(validator_address).call())
 
-    def validator_exists(self, validator_id: str) -> bool:
+    def validator_exists(self, validator_id: ValidatorId) -> bool:
         """Checks if there is a validator with provided ID
 
         :returns: True if validator exists, otherwise False
         :rtype: bool
         """
-        return self.contract.functions.validatorExists(validator_id).call()
+        return bool(self.contract.functions.validatorExists(validator_id).call())
 
-    def validator_id_by_address(self, validator_address: str) -> int:
+    def validator_id_by_address(self, validator_address: ChecksumAddress) -> ValidatorId:
         """Returns validator ID by validator address
 
         :returns: Validator ID
         :rtype: int
         """
-        return self.contract.functions.getValidatorId(validator_address).call()
+        return ValidatorId(self.contract.functions.getValidatorId(validator_address).call())
 
-    def get_trusted_validator_ids(self) -> list:
+    def get_trusted_validator_ids(self) -> List[ValidatorId]:
         """Returns list of trusted validators id.
 
         :returns: List of trusted validators id
         :rtype: list
         """
-        return self.contract.functions.getTrustedValidators().call()
+        return [
+            ValidatorId(id)
+            for id
+            in self.contract.functions.getTrustedValidators().call()
+        ]
 
     @transaction_method
-    def _enable_validator(self, validator_id: int) -> TxRes:
+    def _enable_validator(self, validator_id: ValidatorId) -> ContractFunction:
         """For internal usage only"""
         return self.contract.functions.enableValidator(validator_id)
 
     @transaction_method
-    def _disable_validator(self, validator_id: int) -> TxRes:
+    def _disable_validator(self, validator_id: ValidatorId) -> ContractFunction:
         """For internal usage only"""
         return self.contract.functions.disableValidator(validator_id)
 
-    def _is_authorized_validator(self, validator_id: int) -> bool:
+    def _is_authorized_validator(self, validator_id: ValidatorId) -> bool:
         """For internal usage only"""
-        return self.contract.functions.isAuthorizedValidator(validator_id).call()
+        return bool(self.contract.functions.isAuthorizedValidator(validator_id).call())
 
-    def is_accepting_new_requests(self, validator_id: int) -> bool:
+    def is_accepting_new_requests(self, validator_id: ValidatorId) -> bool:
         """For internal usage only"""
-        return self.contract.functions.isAcceptingNewRequests(validator_id).call()
+        return bool(self.contract.functions.isAcceptingNewRequests(validator_id).call())
 
     @transaction_method
     def register_validator(self, name: str, description: str, fee_rate: int,
-                           min_delegation_amount: int) -> TxRes:
+                           min_delegation_amount: int) -> ContractFunction:
         """Registers a new validator in the SKALE Manager contracts.
 
         :param name: Validator name
         :type name: str
         :param description: Validator description
         :type description: str
         :param fee_rate: Validator fee rate
@@ -190,123 +219,136 @@
         :type min_delegation_amount: int
         :returns: Transaction results
         :rtype: TxRes
         """
         return self.contract.functions.registerValidator(
             name, description, fee_rate, min_delegation_amount)
 
-    def get_link_node_signature(self, validator_id: int) -> str:
+    def get_link_node_signature(self, validator_id: ValidatorId) -> str:
         unsigned_hash = Web3.solidity_keccak(['uint256'], [validator_id])
         signed_hash = self.skale.wallet.sign_hash(unsigned_hash.hex())
         return signed_hash.signature.hex()
 
     @transaction_method
-    def link_node_address(self, node_address: str, signature: str) -> TxRes:
+    def link_node_address(self, node_address: ChecksumAddress, signature: str) -> ContractFunction:
         """Link node address to your validator account.
 
         :param node_address: Address of the node to link
         :type node_address: str
         :param signature: Signature - reuslt of the get_link_node_signature function
         :type signature: str
         :returns: Transaction results
         :rtype: TxRes
         """
         return self.contract.functions.linkNodeAddress(node_address, signature)
 
     @transaction_method
-    def unlink_node_address(self, node_address: str) -> TxRes:
+    def unlink_node_address(self, node_address: ChecksumAddress) -> ContractFunction:
         """Unlink node address from your validator account.
 
         :param node_address: Address of the node to unlink
         :type node_address: str
         :returns: Transaction results
         :rtype: TxRes
         """
         return self.contract.functions.unlinkNodeAddress(node_address)
 
     @transaction_method
-    def disable_whitelist(self) -> TxRes:
+    def disable_whitelist(self) -> ContractFunction:
         """ Disable validator whitelist. Master key only transaction.
         :returns: Transaction results
         :rtype: TxRes
         """
         return self.contract.functions.disableWhitelist()
 
     def get_use_whitelist(self) -> bool:
         """ Return useWhitelist contract variable
         :returns: useWhitelist value
         :rtype: bool
         """
-        return self.contract.functions.useWhitelist().call()
+        return bool(self.contract.functions.useWhitelist().call())
 
-    def get_and_update_bond_amount(self, validator_id: int) -> int:
+    def get_and_update_bond_amount(self, validator_id: ValidatorId) -> int:
         """Return amount of token that validator delegated to himself
            :param validator_id: id of the validator
            :returns:
            :rtype: int
         """
-        return self.contract.functions.getAndUpdateBondAmount(validator_id).call()
+        return int(self.contract.functions.getAndUpdateBondAmount(validator_id).call())
 
     @transaction_method
-    def set_validator_mda(self, minimum_delegation_amount: int) -> TxRes:
+    def set_validator_mda(self, minimum_delegation_amount: Wei) -> ContractFunction:
         """ Allows a validator to set the minimum delegation amount.
 
         :param new_minimum_delegation_amount: Minimum delegation amount
         :type new_minimum_delegation_amount: int
         :returns: Transaction results
         :rtype: TxRes
         """
         return self.contract.functions.setValidatorMDA(minimum_delegation_amount)
 
     @transaction_method
-    def request_for_new_address(self, new_validator_address: str) -> TxRes:
+    def request_for_new_address(self, new_validator_address: ChecksumAddress) -> ContractFunction:
         """ Allows a validator to request a new address.
 
         :param new_validator_address: New validator address
         :type new_validator_address: str
         :returns: Transaction results
         :rtype: TxRes
         """
         return self.contract.functions.requestForNewAddress(new_validator_address)
 
     @transaction_method
-    def confirm_new_address(self, validator_id: int) -> TxRes:
+    def confirm_new_address(self, validator_id: ValidatorId) -> ContractFunction:
         """  Confirm change of the address.
 
         :param validator_id: ID of the validator
         :type validator_id: int
         :returns: Transaction results
         :rtype: TxRes
         """
         return self.contract.functions.confirmNewAddress(validator_id)
 
     @transaction_method
-    def set_validator_name(self, new_name: str) -> TxRes:
+    def set_validator_name(self, new_name: str) -> ContractFunction:
         """ Allows a validator to change the name.
 
         :param new_name: New validator name
         :type new_name: str
         :returns: Transaction results
         :rtype: TxRes
         """
         return self.contract.functions.setValidatorName(new_name)
 
     @transaction_method
-    def set_validator_description(self, new_description: str) -> TxRes:
+    def set_validator_description(self, new_description: str) -> ContractFunction:
         """ Allows a validator to change the name.
 
         :param new_description: New validator description
         :type new_name: str
         :returns: Transaction results
         :rtype: TxRes
         """
         return self.contract.functions.setValidatorDescription(new_description)
 
     @transaction_method
-    def grant_role(self, role: bytes, address: str) -> TxRes:
+    def grant_role(self, role: bytes, address: ChecksumAddress) -> ContractFunction:
         return self.contract.functions.grantRole(role, address)
 
     def validator_manager_role(self) -> bytes:
-        return self.contract.functions.VALIDATOR_MANAGER_ROLE().call()
+        return bytes(self.contract.functions.VALIDATOR_MANAGER_ROLE().call())
 
-    def has_role(self, role: bytes, address: str) -> bool:
-        return self.contract.functions.hasRole(role, address).call()
+    def has_role(self, role: bytes, address: ChecksumAddress) -> bool:
+        return bool(self.contract.functions.hasRole(role, address).call())
+
+    def _to_validator(self, untyped_validator: Dict[str, Any]) -> Validator:
+        return Validator({
+            'name': str(untyped_validator['name']),
+            'validator_address': ChecksumAddress(untyped_validator['validator_address']),
+            'requested_address': ChecksumAddress(untyped_validator['requested_address']),
+            'description': str(untyped_validator['description']),
+            'fee_rate': int(untyped_validator['fee_rate']),
+            'registration_time': int(untyped_validator['registration_time']),
+            'minimum_delegation_amount': Wei(untyped_validator['minimum_delegation_amount']),
+            'accept_new_requests': bool(untyped_validator['accept_new_requests']),
+            'trusted': bool(untyped_validator['trusted'])
+        })
```

### Comparing `skale.py-7.dev11/skale/contracts/manager/groups.py` & `skale.py-7.dev12/skale/contracts/allocator_contract.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,13 @@
 #   SKALE.py is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
-""" SKALE group class """
-
 from skale.contracts.base_contract import BaseContract
+from skale.skale_allocator import SkaleAllocator
 
 
-class Groups(BaseContract):
+class AllocatorContract(BaseContract[SkaleAllocator]):
     pass
```

### Comparing `skale.py-7.dev11/skale/contracts/manager/key_storage.py` & `skale.py-7.dev12/skale/contracts/ima/linker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 #   -*- coding: utf-8 -*-
 #
 #   This file is part of SKALE.py
 #
-#   Copyright (C) 2020-Present SKALE Labs
+#   Copyright (C) 2019-Present SKALE Labs
 #
 #   SKALE.py is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU Affero General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   SKALE.py is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
-from skale.contracts.base_contract import BaseContract
+from typing import List
+from eth_typing import ChecksumAddress
+from web3.contract.contract import ContractFunction
 
+from skale.contracts.base_contract import transaction_method
+from skale.contracts.ima_contract import ImaContract
+from skale.types.schain import SchainName
 
-class KeyStorage(BaseContract):
-    def get_common_public_key(self, group_index):
-        return self.contract.functions.getCommonPublicKey(group_index).call()
 
-    def get_previous_public_key(self, group_index):
-        return self.contract.functions.getPreviousPublicKey(group_index).call()
-
-    def get_all_previous_public_keys(self, group_index):
-        return self.contract.functions.getAllPreviousPublicKeys(group_index).call()
+class Linker(ImaContract):
+    @transaction_method
+    def connect_schain(
+            self,
+            schain_name: SchainName,
+            mainnet_contracts: List[ChecksumAddress]
+    ) -> ContractFunction:
+        return self.contract.functions.connectSchain(
+            schain_name,
+            mainnet_contracts
+        )
```

### Comparing `skale.py-7.dev11/skale/contracts/manager/manager.py` & `skale.py-7.dev12/skale/contracts/manager/manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,30 +18,42 @@
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 """ SKALE manager operations """
 
 
 import logging
 import socket
 
-from eth_abi import encode
-
-from skale.contracts.base_contract import BaseContract, transaction_method
+from eth_abi.abi import encode
+from eth_typing import ChecksumAddress
+from web3.contract.contract import ContractFunction
+
+from skale.contracts.base_contract import transaction_method
+from skale.contracts.skale_manager_contract import SkaleManagerContract
+from skale.types.node import NodeId, Port
+from skale.types.schain import SchainName
 from skale.utils import helper
 from skale.transactions.result import TxRes
 from skale.dataclasses.schain_options import (
     SchainOptions, get_default_schain_options
 )
 
 logger = logging.getLogger(__name__)
 
 
-class Manager(BaseContract):
+class Manager(SkaleManagerContract):
 
     @transaction_method
-    def create_node(self, ip, port, name, domain_name, public_ip=None):
+    def create_node(
+            self,
+            ip: str,
+            port: Port,
+            name: str,
+            domain_name: str,
+            public_ip: str | None = None
+    ) -> ContractFunction:
         logger.info(
             f'create_node: {ip}:{port}, name: {name}, domain_name: {domain_name}')
         skale_nonce = helper.generate_nonce()
         if not public_ip:
             public_ip = ip
         ip_bytes = socket.inet_aton(ip)
         public_ip_bytes = socket.inet_aton(public_ip)
@@ -52,32 +64,32 @@
             ip_bytes,
             public_ip_bytes,
             pk_parts_bytes,
             name,
             domain_name
         )
 
-    def create_default_schain(self, name):
+    def create_default_schain(self, name: SchainName) -> TxRes:
         lifetime = 3600
         nodes_type = self.skale.schains_internal.number_of_schain_types()
         price_in_wei = self.skale.schains.get_schain_price(
             nodes_type, lifetime)
         return self.create_schain(lifetime, nodes_type, price_in_wei, name,
                                   wait_for=True)
 
     @transaction_method
     def create_schain(
         self,
         lifetime: int,
         type_of_nodes: int,
         deposit: str,
-        name: str,
-        schain_originator: str = None,
-        options: SchainOptions = None
-    ):
+        name: SchainName,
+        schain_originator: ChecksumAddress | None = None,
+        options: SchainOptions | None = None
+    ) -> ContractFunction:
         logger.info(
             f'create_schain: type_of_nodes: {type_of_nodes}, name: {name}')
         skale_nonce = helper.generate_nonce()
 
         if schain_originator is None:
             schain_originator = self.skale.wallet.address
         if not options:
@@ -91,37 +103,37 @@
         return self.skale.token.contract.functions.send(
             self.address,
             deposit,
             tx_data
         )
 
     @transaction_method
-    def get_bounty(self, node_id):
+    def get_bounty(self, node_id: NodeId) -> ContractFunction:
         return self.contract.functions.getBounty(node_id)
 
     @transaction_method
-    def delete_schain(self, schain_name):
+    def delete_schain(self, schain_name: SchainName) -> ContractFunction:
         return self.contract.functions.deleteSchain(schain_name)
 
     @transaction_method
-    def delete_schain_by_root(self, schain_name):
+    def delete_schain_by_root(self, schain_name: SchainName) -> ContractFunction:
         return self.contract.functions.deleteSchainByRoot(schain_name)
 
     @transaction_method
-    def node_exit(self, node_id):
+    def node_exit(self, node_id: NodeId) -> ContractFunction:
         return self.contract.functions.nodeExit(node_id)
 
     @transaction_method
-    def grant_role(self, role: bytes, address: str) -> TxRes:
+    def grant_role(self, role: bytes, address: ChecksumAddress) -> ContractFunction:
         return self.contract.functions.grantRole(role, address)
 
     def default_admin_role(self) -> bytes:
-        return self.contract.functions.DEFAULT_ADMIN_ROLE().call()
+        return bytes(self.contract.functions.DEFAULT_ADMIN_ROLE().call())
 
     def admin_role(self) -> bytes:
-        return self.contract.functions.ADMIN_ROLE().call()
+        return bytes(self.contract.functions.ADMIN_ROLE().call())
 
     def schain_removal_role(self) -> bytes:
-        return self.contract.functions.SCHAIN_REMOVAL_ROLE().call()
+        return bytes(self.contract.functions.SCHAIN_REMOVAL_ROLE().call())
 
-    def has_role(self, role: bytes, address: str) -> bool:
-        return self.contract.functions.hasRole(role, address).call()
+    def has_role(self, role: bytes, address: ChecksumAddress) -> bool:
+        return bool(self.contract.functions.hasRole(role, address).call())
```

### Comparing `skale.py-7.dev11/skale/contracts/manager/node_rotation.py` & `skale.py-7.dev12/skale/contracts/manager/node_rotation.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,126 +14,119 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 """ NodeRotation.sol functions """
 
+from __future__ import annotations
 import logging
 import functools
-import warnings
-from dataclasses import dataclass
+from typing import TYPE_CHECKING, List
 
-from skale.contracts.base_contract import BaseContract, transaction_method
-from skale.transactions.result import TxRes
+from eth_typing import ChecksumAddress
+
+from skale.contracts.base_contract import transaction_method
+from web3.contract.contract import ContractFunction
 from web3.exceptions import ContractLogicError
 
+from skale.contracts.skale_manager_contract import SkaleManagerContract
+from skale.types.node import NodeId
+from skale.types.rotation import Rotation, RotationSwap
+from skale.types.schain import SchainHash, SchainName
 
-logger = logging.getLogger(__name__)
+if TYPE_CHECKING:
+    from skale.contracts.manager.schains import SChains
 
 
-NO_PREVIOUS_NODE_EXCEPTION_TEXT = 'No previous node'
+logger = logging.getLogger(__name__)
 
 
-@dataclass
-class Rotation:
-    leaving_node_id: int
-    new_node_id: int
-    freeze_until: int
-    rotation_counter: int
+NO_PREVIOUS_NODE_EXCEPTION_TEXT = 'No previous node'
 
 
-class NodeRotation(BaseContract):
+class NodeRotation(SkaleManagerContract):
     """Wrapper for NodeRotation.sol functions"""
 
     @property
     @functools.lru_cache()
-    def schains(self):
+    def schains(self) -> SChains:
         return self.skale.schains
 
-    def get_rotation_obj(self, schain_name) -> Rotation:
+    def get_rotation(self, schain_name: SchainName) -> Rotation:
         schain_id = self.schains.name_to_id(schain_name)
         rotation_data = self.contract.functions.getRotation(schain_id).call()
         return Rotation(*rotation_data)
 
-    def get_rotation(self, schain_name):
-        warnings.warn('Deprecated, will be removed in v6', DeprecationWarning)
-        schain_id = self.schains.name_to_id(schain_name)
-        rotation_data = self.contract.functions.getRotation(schain_id).call()
-        return {
-            'leaving_node': rotation_data[0],
-            'new_node': rotation_data[1],
-            'freeze_until': rotation_data[2],
-            'rotation_id': rotation_data[3]
-        }
-
-    def get_leaving_history(self, node_id):
+    def get_leaving_history(self, node_id: NodeId) -> List[RotationSwap]:
         raw_history = self.contract.functions.getLeavingHistory(node_id).call()
         history = [
-            {
-                'schain_id': schain[0],
-                'finished_rotation': schain[1]
-            }
+            RotationSwap({
+                'schain_id': SchainHash(schain[0]),
+                'finished_rotation': int(schain[1])
+            })
             for schain in raw_history
         ]
         return history
 
-    def get_schain_finish_ts(self, node_id: int, schain_name: str) -> int:
-        raw_history = self.contract.functions.getLeavingHistory(node_id).call()
+    def get_schain_finish_ts(self, node_id: NodeId, schain_name: SchainName) -> int | None:
+        history = self.get_leaving_history(node_id)
         schain_id = self.skale.schains.name_to_id(schain_name)
         finish_ts = next(
-            (schain[1] for schain in raw_history if '0x' + schain[0].hex() == schain_id), None)
+            (swap['finished_rotation'] for swap in history if swap['schain_id'] == schain_id),
+            None
+        )
         if not finish_ts:
             return None
-        return finish_ts
+        return int(finish_ts)
 
-    def is_rotation_in_progress(self, schain_name) -> bool:
+    def is_rotation_in_progress(self, schain_name: SchainName) -> bool:
         schain_id = self.schains.name_to_id(schain_name)
-        return self.contract.functions.isRotationInProgress(schain_id).call()
+        return bool(self.contract.functions.isRotationInProgress(schain_id).call())
 
-    def is_new_node_found(self, schain_name) -> bool:
+    def is_new_node_found(self, schain_name: SchainName) -> bool:
         schain_id = self.schains.name_to_id(schain_name)
-        return self.contract.functions.isNewNodeFound(schain_id).call()
+        return bool(self.contract.functions.isNewNodeFound(schain_id).call())
 
-    def is_rotation_active(self, schain_name) -> bool:
+    def is_rotation_active(self, schain_name: SchainName) -> bool:
         """
         The public function that tells whether rotation is in the active phase - the new group is
         already generated
         """
         finish_ts_reached = self.is_finish_ts_reached(schain_name)
         return self.is_rotation_in_progress(schain_name) and not finish_ts_reached
 
-    def is_finish_ts_reached(self, schain_name) -> bool:
-        rotation = self.skale.node_rotation.get_rotation_obj(schain_name)
+    def is_finish_ts_reached(self, schain_name: SchainName) -> bool:
+        rotation = self.skale.node_rotation.get_rotation(schain_name)
         schain_finish_ts = self.get_schain_finish_ts(rotation.leaving_node_id, schain_name)
 
         if not schain_finish_ts:
             schain_finish_ts = 0
 
         latest_block = self.skale.web3.eth.get_block('latest')
         current_ts = latest_block['timestamp']
 
         logger.info(f'current_ts: {current_ts}, schain_finish_ts: {schain_finish_ts}')
         return current_ts > schain_finish_ts
 
-    def wait_for_new_node(self, schain_name):
+    def wait_for_new_node(self, schain_name: SchainName) -> bool:
         schain_id = self.schains.name_to_id(schain_name)
-        return self.contract.functions.waitForNewNode(schain_id).call()
+        return bool(self.contract.functions.waitForNewNode(schain_id).call())
 
     @transaction_method
-    def grant_role(self, role: bytes, owner: str) -> TxRes:
+    def grant_role(self, role: bytes, owner: str) -> ContractFunction:
         return self.contract.functions.grantRole(role, owner)
 
-    def has_role(self, role: bytes, address: str) -> bool:
-        return self.contract.functions.hasRole(role, address).call()
+    def has_role(self, role: bytes, address: ChecksumAddress) -> bool:
+        return bool(self.contract.functions.hasRole(role, address).call())
 
-    def debugger_role(self):
-        return self.contract.functions.DEBUGGER_ROLE().call()
+    def debugger_role(self) -> bytes:
+        return bytes(self.contract.functions.DEBUGGER_ROLE().call())
 
-    def get_previous_node(self, schain_name: str, node_id: int) -> int:
+    def get_previous_node(self, schain_name: SchainName, node_id: NodeId) -> NodeId | None:
         schain_id = self.schains.name_to_id(schain_name)
         try:
-            return self.contract.functions.getPreviousNode(schain_id, node_id).call()
+            return NodeId(self.contract.functions.getPreviousNode(schain_id, node_id).call())
         except (ContractLogicError, ValueError) as e:
             if NO_PREVIOUS_NODE_EXCEPTION_TEXT in str(e):
                 return None
             raise e
```

### Comparing `skale.py-7.dev11/skale/contracts/manager/punisher.py` & `skale.py-7.dev12/skale/contracts/manager/bounty_v2.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,21 +13,24 @@
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
-from skale.contracts.base_contract import BaseContract, transaction_method
-from skale.transactions.result import TxRes
+from eth_typing import ChecksumAddress
+from web3.contract.contract import ContractFunction
 
+from skale.contracts.base_contract import transaction_method
+from skale.contracts.skale_manager_contract import SkaleManagerContract
 
-class Punisher(BaseContract):
+
+class BountyV2(SkaleManagerContract):
     @transaction_method
-    def grant_role(self, role: bytes, owner: str) -> TxRes:
+    def grant_role(self, role: bytes, owner: ChecksumAddress) -> ContractFunction:
         return self.contract.functions.grantRole(role, owner)
 
-    def has_role(self, role: bytes, address: str) -> bool:
-        return self.contract.functions.hasRole(role, address).call()
+    def has_role(self, role: bytes, address: ChecksumAddress) -> bool:
+        return bool(self.contract.functions.hasRole(role, address).call())
 
-    def forgiver_role(self):
-        return self.contract.functions.FORGIVER_ROLE().call()
+    def bounty_reduction_manager_role(self) -> bytes:
+        return bytes(self.contract.functions.BOUNTY_REDUCTION_MANAGER_ROLE().call())
```

### Comparing `skale.py-7.dev11/skale/contracts/manager/schains.py` & `skale.py-7.dev12/skale/contracts/manager/schains.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,140 +15,130 @@
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 """ Schains.sol functions """
 
 import functools
-from dataclasses import dataclass, asdict
+from dataclasses import asdict
+from typing import Any, List
 
 from Crypto.Hash import keccak
-
-from skale.contracts.base_contract import BaseContract, transaction_method
-from skale.transactions.result import TxRes
-from skale.utils.helper import format_fields
+from eth_typing import ChecksumAddress, HexStr
+from hexbytes import HexBytes
+from web3 import Web3
+from web3.contract.contract import ContractFunction
+from web3.types import Wei
+
+from skale.contracts.base_contract import transaction_method
+from skale.contracts.manager.node_rotation import NodeRotation
+from skale.contracts.manager.schains_internal import SChainsInternal
+from skale.contracts.skale_manager_contract import SkaleManagerContract
+from skale.types.node import NodeId
+from skale.types.schain import SchainHash, SchainName, SchainStructure, SchainStructureWithStatus
 from skale.dataclasses.schain_options import (
     SchainOptions, get_default_schain_options, parse_schain_options
 )
 
 
 FIELDS = [
     'name', 'mainnetOwner', 'indexInOwnerList', 'partOfNode', 'lifetime', 'startDate', 'startBlock',
-    'deposit', 'index', 'generation', 'originator', 'chainId', 'multitransactionMode',
-    'thresholdEncryption'
+    'deposit', 'index', 'generation', 'originator', 'chainId', 'options'
 ]
 
 
-@dataclass
-class SchainStructure:
-    name: str
-    mainnet_owner: str
-    index_in_owner_list: int
-    part_of_node: int
-    lifetime: int
-    start_date: int
-    start_block: int
-    deposit: int
-    index: int
-    generation: int
-    originator: str
-    chain_id: int
-    options: SchainOptions
-
-
-class SChains(BaseContract):
+class SChains(SkaleManagerContract):
     """Wrapper for some of the Schains.sol functions"""
 
-    def name_to_group_id(self, name):
+    def name_to_group_id(self, name: SchainName) -> HexBytes:
         return self.skale.web3.keccak(text=name)
 
     @property
     @functools.lru_cache()
-    def schains_internal(self):
+    def schains_internal(self) -> SChainsInternal:
         return self.skale.schains_internal
 
     @property
     @functools.lru_cache()
-    def node_rotation(self):
+    def node_rotation(self) -> NodeRotation:
         return self.skale.node_rotation
 
-    @format_fields(FIELDS)
-    def get(self, id_, obj=False):
+    def get(self, id_: SchainHash) -> SchainStructure:
         res = self.schains_internal.get_raw(id_)
-        hash_obj = keccak.new(data=res[0].encode("utf8"), digest_bits=256)
-        hash_str = "0x" + hash_obj.hexdigest()[:13]
-        res.append(hash_str)
         options = self.get_options(id_)
-        if obj:  # TODO: temporary solution for backwards compatibility
-            return SchainStructure(*res, options=options)
-        else:
-            res += asdict(options).values()
-        return res
+        return SchainStructure(**asdict(res), chainId=self.name_to_id(res.name), options=options)
 
-    @format_fields(FIELDS)
-    def get_by_name(self, name, obj=False):
+    def get_by_name(self, name: SchainName) -> SchainStructure:
         id_ = self.name_to_id(name)
-        return self.get(id_, obj=obj)
+        return self.get(id_)
 
-    def get_schains_for_owner(self, account):
+    def get_schains_for_owner(self, account: ChecksumAddress) -> List[SchainStructure]:
         schains = []
         list_size = self.schains_internal.get_schain_list_size(account)
 
         for i in range(0, list_size):
             id_ = self.schains_internal.get_schain_id_by_index_for_owner(account, i)
             schain = self.get(id_)
             schains.append(schain)
         return schains
 
-    def get_schains_for_node(self, node_id):
+    def get_schains_for_node(self, node_id: NodeId) -> list[SchainStructureWithStatus]:
         schains = []
         schain_ids = self.schains_internal.get_schain_ids_for_node(node_id)
         for schain_id in schain_ids:
-            schain = self.get(schain_id)
-            schain['active'] = True if self.schain_active(schain) else False
+            simple_schain = self.get(schain_id)
+            schain = SchainStructureWithStatus(
+                **asdict(simple_schain),
+                active=self.schain_active(simple_schain)
+            )
             schains.append(schain)
         return schains
 
-    def get_active_schains_for_node(self, node_id):
+    def get_active_schains_for_node(self, node_id: NodeId) -> List[SchainStructureWithStatus]:
         schains = []
         schain_ids = self.schains_internal.get_active_schain_ids_for_node(node_id)
         for schain_id in schain_ids:
-            schain = self.get(schain_id)
-            schain['active'] = True
+            simple_schain = self.get(schain_id)
+            schain = SchainStructureWithStatus(
+                **asdict(simple_schain),
+                active=True
+            )
             schains.append(schain)
         return schains
 
-    def name_to_id(self, name):
+    def name_to_id(self, name: SchainName) -> SchainHash:
         keccak_hash = keccak.new(data=name.encode("utf8"), digest_bits=256)
-        return '0x' + keccak_hash.hexdigest()
+        return SchainHash(Web3.to_bytes(hexstr=Web3.to_hex(hexstr=HexStr(keccak_hash.hexdigest()))))
 
-    def get_last_rotation_id(self, schain_name):
+    def get_last_rotation_id(self, schain_name: SchainName) -> int:
         rotation_data = self.node_rotation.get_rotation(schain_name)
-        return rotation_data['rotation_id']
+        return rotation_data.rotation_counter
 
-    def schain_active(self, schain):
-        if schain['name'] != '' and \
-                schain['mainnetOwner'] != '0x0000000000000000000000000000000000000000':
+    def schain_active(self, schain: SchainStructure) -> bool:
+        if schain.name != '' and \
+                schain.mainnetOwner != '0x0000000000000000000000000000000000000000':
             return True
+        return False
 
-    def get_schain_price(self, index_of_type, lifetime):
-        return self.contract.functions.getSchainPrice(index_of_type,
-                                                      lifetime).call()
+    def get_schain_price(self, index_of_type: int, lifetime: int) -> Wei:
+        return Wei(
+            self.contract.functions.getSchainPrice(index_of_type, lifetime).call()
+        )
 
     @transaction_method
     def add_schain_by_foundation(
         self,
         lifetime: int,
         type_of_nodes: int,
         nonce: int,
-        name: str,
-        options: SchainOptions = None,
-        schain_owner=None,
-        schain_originator=None
-    ) -> TxRes:
+        name: SchainName,
+        options: SchainOptions | None = None,
+        schain_owner: ChecksumAddress | None = None,
+        schain_originator: ChecksumAddress | None = None
+    ) -> ContractFunction:
         if schain_owner is None:
             schain_owner = self.skale.wallet.address
         if schain_originator is None:
             schain_originator = self.skale.wallet.address
         if not options:
             options = get_default_schain_options()
 
@@ -159,27 +149,27 @@
             name,
             schain_owner,
             schain_originator,
             options.to_tuples()
         )
 
     @transaction_method
-    def grant_role(self, role: bytes, owner: str) -> TxRes:
+    def grant_role(self, role: bytes, owner: ChecksumAddress) -> ContractFunction:
         return self.contract.functions.grantRole(role, owner)
 
-    def schain_creator_role(self):
-        return self.contract.functions.SCHAIN_CREATOR_ROLE().call()
+    def schain_creator_role(self) -> bytes:
+        return bytes(self.contract.functions.SCHAIN_CREATOR_ROLE().call())
 
-    def __raw_get_options(self, schain_id: str) -> list:
-        return self.contract.functions.getOptions(schain_id).call()
+    def __raw_get_options(self, schain_id: SchainHash) -> List[Any]:
+        return list(self.contract.functions.getOptions(schain_id).call())
 
-    def get_options(self, schain_id: str) -> SchainOptions:
+    def get_options(self, schain_id: SchainHash) -> SchainOptions:
         return parse_schain_options(
             raw_options=self.__raw_get_options(schain_id)
         )
 
-    def get_options_by_name(self, name: str) -> SchainOptions:
+    def get_options_by_name(self, name: SchainName) -> SchainOptions:
         id_ = self.name_to_id(name)
         return self.get_options(id_)
 
-    def restart_schain_creation(self, name: str) -> TxRes:
+    def restart_schain_creation(self, name: SchainName) -> ContractFunction:
         return self.contract.functions.restartSchainCreation(name)
```

### Comparing `skale.py-7.dev11/skale/contracts/manager/sync_manager.py` & `skale.py-7.dev12/skale/contracts/manager/sync_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,57 +17,59 @@
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
 from collections import namedtuple
 from typing import List
+from web3.contract.contract import ContractFunction
 
-from skale.contracts.base_contract import BaseContract, transaction_method
+from skale.contracts.base_contract import transaction_method
+from skale.contracts.skale_manager_contract import SkaleManagerContract
 from skale.transactions.result import TxRes
 from skale.utils.helper import ip_from_bytes, ip_to_bytes
 
 
 class IpRange(namedtuple('IpRange', ['start_ip', 'end_ip'])):
     @classmethod
     def from_packed(cls, packed_ips: List[bytes]) -> IpRange:
         return cls(
             ip_from_bytes(packed_ips[0]),
             ip_from_bytes(packed_ips[1])
         )
 
 
-class SyncManager(BaseContract):
+class SyncManager(SkaleManagerContract):
     """Wrapper for SyncManager.sol functions"""
 
     @transaction_method
-    def add_ip_range(self, name, start_ip: str, end_ip: str) -> TxRes:
+    def add_ip_range(self, name: str, start_ip: str, end_ip: str) -> ContractFunction:
         return self.contract.functions.addIPRange(
             name,
             ip_to_bytes(start_ip),
             ip_to_bytes(end_ip)
         )
 
     @transaction_method
-    def remove_ip_range(self, name: str) -> TxRes:
+    def remove_ip_range(self, name: str) -> ContractFunction:
         return self.contract.functions.removeIPRange(name)
 
     def get_ip_ranges_number(self) -> int:
-        return self.contract.functions.getIPRangesNumber().call()
+        return int(self.contract.functions.getIPRangesNumber().call())
 
     def get_ip_range_by_index(self, index: int) -> IpRange:
         packed = self.contract.functions.getIPRangeByIndex(index).call()
         return IpRange.from_packed(packed)
 
     def get_ip_range_by_name(self, name: str) -> IpRange:
         packed = self.contract.functions.getIPRangeByName(name).call()
         return IpRange.from_packed(packed)
 
     def grant_sync_manager_role(self, address: str) -> TxRes:
         return self.grant_role(self.sync_manager_role(), address)
 
     def sync_manager_role(self) -> bytes:
-        return self.contract.functions.SYNC_MANAGER_ROLE().call()
+        return bytes(self.contract.functions.SYNC_MANAGER_ROLE().call())
 
     @transaction_method
-    def grant_role(self, role: bytes, owner: str) -> TxRes:
+    def grant_role(self, role: bytes, owner: str) -> ContractFunction:
         return self.contract.functions.grantRole(role, owner)
```

### Comparing `skale.py-7.dev11/skale/contracts/manager/test/time_helpers_with_debug.py` & `skale.py-7.dev12/skale/contracts/manager/test/time_helpers_with_debug.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,23 +13,25 @@
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
-from skale.contracts.base_contract import BaseContract, transaction_method
-from skale.transactions.result import TxRes
+from web3.contract.contract import ContractFunction
 
+from skale.contracts.base_contract import transaction_method
+from skale.contracts.skale_manager_contract import SkaleManagerContract
 
-class TimeHelpersWithDebug(BaseContract):
+
+class TimeHelpersWithDebug(SkaleManagerContract):
     """Wrapper for TimeHelpersWithDebug.sol functions (internal usage only)"""
 
     @transaction_method
-    def skip_time(self, sec: int) -> TxRes:
+    def skip_time(self, sec: int) -> ContractFunction:
         """Skip time on contracts
 
         :param sec: Time to skip in seconds
         :type sec: int
         :returns: Transaction results
         :rtype: TxRes
         """
@@ -37,8 +39,8 @@
 
     def get_current_month(self) -> int:
         """Get current month from contract
 
         :returns: Month index
         :rtype: int
         """
-        return self.contract.functions.getCurrentMonth().call()
+        return int(self.contract.functions.getCurrentMonth().call())
```

### Comparing `skale.py-7.dev11/skale/contracts/manager/token.py` & `skale.py-7.dev12/skale/skale_ima.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,30 +12,40 @@
 #   SKALE.py is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
-""" SKALE token operations """
 
-from skale.contracts.base_contract import BaseContract, transaction_method
+from __future__ import annotations
+import logging
+from typing import List
 
+from skale.skale_base import SkaleBase
+from skale.utils.contract_info import ContractInfo
+from skale.utils.contract_types import ContractTypes
+from skale.utils.helper import get_contracts_info
 
-class Token(BaseContract):
-    @transaction_method
-    def transfer(self, address, value):
-        return self.contract.functions.send(address, value, b'')
 
-    def get_balance(self, address):
-        return self.contract.functions.balanceOf(address).call()
+logger = logging.getLogger(__name__)
 
-    @transaction_method
-    def add_authorized(self, address, wallet):  # pragma: no cover
-        return self.contract.functions.addAuthorized(address)
 
-    def get_and_update_slashed_amount(self, address: str) -> int:
-        return self.contract.functions.getAndUpdateSlashedAmount(address).call()
+class SkaleIma(SkaleBase):
+    @property
+    def project_name(self) -> str:
+        return 'mainnet-ima'
 
-    @transaction_method
-    def mint(self, address, amount, user_data=b'', operator_data=b''):
-        return self.contract.functions.mint(address, amount, user_data, operator_data)
+    def contracts_info(self) -> List[ContractInfo[SkaleIma]]:
+        import skale.contracts.ima as contracts
+        return [
+            ContractInfo('linker', 'Linker',
+                         contracts.Linker, ContractTypes.API, False)
+        ]
+
+    def set_contracts_info(self) -> None:
+        self._SkaleBase__contracts_info = get_contracts_info(self.contracts_info())
+
+
+def spawn_skale_ima_lib(skale_ima: SkaleIma) -> SkaleIma:
+    """ Clone skale ima object with the same wallet """
+    return SkaleIma(skale_ima._endpoint, skale_ima.instance.address, skale_ima.wallet)
```

### Comparing `skale.py-7.dev11/skale/contracts/manager/wallets.py` & `skale.py-7.dev12/skale/skale_allocator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,67 @@
 #   -*- coding: utf-8 -*-
 #
 #   This file is part of SKALE.py
 #
-#   Copyright (C) 2021-Present SKALE Labs
+#   Copyright (C) 2019-Present SKALE Labs
 #
 #   SKALE.py is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU Affero General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   SKALE.py is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
+from __future__ import annotations
 
-from skale.contracts.base_contract import BaseContract, transaction_method
-from skale.transactions.result import TxRes
+import logging
+from typing import TYPE_CHECKING, List, cast
+from web3.constants import CHECKSUM_ADDRESSS_ZERO
 
+from skale.skale_base import SkaleBase
+from skale.utils.contract_info import ContractInfo
+from skale.utils.contract_types import ContractTypes
+from skale.utils.helper import get_contracts_info
 
-class Wallets(BaseContract):
-    def get_validator_balance(self, validator_id: int) -> int:
-        """Returns SRW balance by validator id (in wei).
-
-        :returns: SRW balance (wei)
-        :rtype: int
-        """
-        return self.contract.functions.getValidatorBalance(validator_id).call()
-
-    @transaction_method
-    def recharge_validator_wallet(self, validator_id: int) -> TxRes:
-        """Pass value kwarg (in wei) to the function when calling it"""
-        return self.contract.functions.rechargeValidatorWallet(validator_id)
-
-    @transaction_method
-    def withdraw_funds_from_validator_wallet(self, amount: int) -> TxRes:
-        return self.contract.functions.withdrawFundsFromValidatorWallet(amount)
+if TYPE_CHECKING:
+    from eth_typing import ChecksumAddress
+    from skale.contracts.allocator.allocator import Allocator
+
+
+logger = logging.getLogger(__name__)
+
+
+def spawn_skale_allocator_lib(skale: SkaleAllocator) -> SkaleAllocator:
+    return SkaleAllocator(skale._endpoint, skale.instance.address, skale.wallet)
+
+
+class SkaleAllocator(SkaleBase):
+    """Represents skale-allocator smart contracts"""
+    @property
+    def project_name(self) -> str:
+        return 'skale-allocator'
+
+    @property
+    def allocator(self) -> Allocator:
+        return cast('Allocator', super()._get_contract('allocator'))
+
+    def contracts_info(self) -> List[ContractInfo[SkaleAllocator]]:
+        import skale.contracts.allocator as contracts
+        return [
+            ContractInfo('escrow', 'Escrow', contracts.Escrow,
+                         ContractTypes.API, True),
+            ContractInfo('allocator', 'Allocator', contracts.Allocator,
+                         ContractTypes.API, True)
+        ]
+
+    def get_contract_address(self, name: str) -> ChecksumAddress:
+        if name == 'Escrow':
+            return CHECKSUM_ADDRESSS_ZERO
+        return super().get_contract_address(name)
+
+    def set_contracts_info(self) -> None:
+        self._SkaleBase__contracts_info = get_contracts_info(self.contracts_info())
```

### Comparing `skale.py-7.dev11/skale/dataclasses/__init__.py` & `skale.py-7.dev12/skale/dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `skale.py-7.dev11/skale/dataclasses/delegation_status.py` & `skale.py-7.dev12/skale/contracts/manager/groups.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,19 +12,14 @@
 #   SKALE.py is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
+""" SKALE group class """
 
-from enum import Enum
+from skale.contracts.skale_manager_contract import SkaleManagerContract
 
 
-class DelegationStatus(Enum):
-    PROPOSED = 0
-    ACCEPTED = 1
-    CANCELED = 2
-    REJECTED = 3
-    DELEGATED = 4
-    UNDELEGATION_REQUESTED = 5
-    COMPLETED = 6
+class Groups(SkaleManagerContract):
+    pass
```

### Comparing `skale.py-7.dev11/skale/dataclasses/node_info.py` & `skale.py-7.dev12/skale/dataclasses/node_info.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,32 +15,33 @@
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
 from dataclasses import dataclass
 from skale.dataclasses.skaled_ports import SkaledPorts
+from skale.types.node import NodeId, Port
 
 
 @dataclass
 class NodeInfo():
     """Dataclass that represents base info about the node"""
-    node_id: int
+    node_id: NodeId
     name: str
-    base_port: int
+    base_port: Port
 
-    def calc_ports(self):
+    def calc_ports(self) -> dict[str, Port]:
         return {
-            'httpRpcPort': self.base_port + SkaledPorts.HTTP_JSON.value,
-            'httpsRpcPort': self.base_port + SkaledPorts.HTTPS_JSON.value,
-            'wsRpcPort': self.base_port + SkaledPorts.WS_JSON.value,
-            'wssRpcPort': self.base_port + SkaledPorts.WSS_JSON.value,
-            'infoHttpRpcPort': self.base_port + SkaledPorts.INFO_HTTP_JSON.value
+            'httpRpcPort': Port(self.base_port + SkaledPorts.HTTP_JSON.value),
+            'httpsRpcPort': Port(self.base_port + SkaledPorts.HTTPS_JSON.value),
+            'wsRpcPort': Port(self.base_port + SkaledPorts.WS_JSON.value),
+            'wssRpcPort': Port(self.base_port + SkaledPorts.WSS_JSON.value),
+            'infoHttpRpcPort': Port(self.base_port + SkaledPorts.INFO_HTTP_JSON.value)
         }
 
-    def to_dict(self):
+    def to_dict(self) -> dict[str, NodeId | str | Port]:
         return {
             'nodeID': self.node_id,
             'nodeName': self.name,
             'basePort': self.base_port,
             **self.calc_ports()
         }
```

### Comparing `skale.py-7.dev11/skale/dataclasses/schain_options.py` & `skale.py-7.dev12/skale/dataclasses/schain_options.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,31 +12,35 @@
 #   SKALE.py is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
-
+from __future__ import annotations
 from dataclasses import dataclass
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from skale.types.schain import SchainOption
 
 
 @dataclass
 class SchainOptions:
     multitransaction_mode: bool
     threshold_encryption: bool
 
-    def to_tuples(self) -> list:
+    def to_tuples(self) -> list[SchainOption]:
         return [
             ('multitr', bool_to_bytes(self.multitransaction_mode)),
             ('encrypt', bool_to_bytes(self.threshold_encryption))
         ]
 
 
-def parse_schain_options(raw_options: list) -> SchainOptions:
+def parse_schain_options(raw_options: list[SchainOption]) -> SchainOptions:
     """
     Parses raw sChain options from smart contracts (list of tuples).
     Returns default values if nothing is set on contracts.
     """
     if len(raw_options) == 0:
         return get_default_schain_options()
     return SchainOptions(
```

### Comparing `skale.py-7.dev11/skale/dataclasses/skaled_ports.py` & `skale.py-7.dev12/skale/dataclasses/skaled_ports.py`

 * *Files identical despite different names*

### Comparing `skale.py-7.dev11/skale/schain_config/__init__.py` & `skale.py-7.dev12/skale/schain_config/__init__.py`

 * *Files identical despite different names*

### Comparing `skale.py-7.dev11/skale/schain_config/rotation_history.py` & `skale.py-7.dev12/skale/schain_config/rotation_history.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,43 +13,52 @@
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
+from __future__ import annotations
 import logging
-from collections import namedtuple
+from typing import TYPE_CHECKING, Dict, List, TypedDict
+from skale.types.rotation import RotationNodeData
 
-from skale import Skale
-from skale.contracts.manager.node_rotation import Rotation
+if TYPE_CHECKING:
+    from skale.skale_manager import SkaleManager
+    from skale.types.dkg import G2Point
+    from skale.types.node import NodeId
+    from skale.types.rotation import BlsPublicKey, NodesGroup, Rotation
+    from skale.types.schain import SchainName
 
 logger = logging.getLogger(__name__)
 
-RotationNodeData = namedtuple('RotationNodeData', ['index', 'node_id', 'public_key'])
+
+class PreviousNodeData(TypedDict):
+    finish_ts: int
+    previous_node_id: NodeId
 
 
 def get_previous_schain_groups(
-    skale: Skale,
-    schain_name: str,
-    leaving_node_id=None,
-) -> dict:
+    skale: SkaleManager,
+    schain_name: SchainName,
+    leaving_node_id: NodeId | None = None,
+) -> Dict[int, NodesGroup]:
     """
     Returns all previous node groups with public keys and finish timestamps.
     In case of no rotations returns the current state.
     """
     logger.info(f'Collecting rotation history for {schain_name}...')
-    node_groups = {}
+    node_groups: dict[int, NodesGroup] = {}
 
-    group_id = skale.schains.name_to_group_id(schain_name)
+    group_id = skale.schains.name_to_id(schain_name)
 
     previous_public_keys = skale.key_storage.get_all_previous_public_keys(group_id)
     current_public_key = skale.key_storage.get_common_public_key(group_id)
 
-    rotation = skale.node_rotation.get_rotation_obj(schain_name)
+    rotation = skale.node_rotation.get_rotation(schain_name)
 
     logger.info(f'Rotation data for {schain_name}: {rotation}')
 
     _add_current_schain_state(skale, node_groups, rotation, schain_name, current_public_key)
     if rotation.rotation_counter == 0:
         return node_groups
 
@@ -62,20 +71,20 @@
         leaving_node_id=leaving_node_id
     )
 
     return node_groups
 
 
 def _add_current_schain_state(
-    skale: Skale,
-    node_groups: dict,
+    skale: SkaleManager,
+    node_groups: dict[int, NodesGroup],
     rotation: Rotation,
-    schain_name: str,
-    current_public_key: list
-) -> dict:
+    schain_name: SchainName,
+    current_public_key: G2Point
+) -> None:
     """
     Internal function, composes the initial info about the current sChain state and adds it to the
     node_groups dictionary
     """
     current_nodes = {}
     ids = skale.schains_internal.get_node_ids_for_schain(schain_name)
     for (index, node_id) in enumerate(ids):
@@ -87,36 +96,37 @@
         'nodes': current_nodes,
         'finish_ts': None,
         'bls_public_key': _compose_bls_public_key_info(current_public_key)
     }
 
 
 def _add_previous_schain_rotations_state(
-    skale: Skale,
-    node_groups: dict,
+    skale: SkaleManager,
+    node_groups: dict[int, NodesGroup],
     rotation: Rotation,
-    schain_name: str,
-    previous_public_keys: list,
-    leaving_node_id=None
-) -> dict:
+    schain_name: SchainName,
+    previous_public_keys: list[G2Point],
+    leaving_node_id: NodeId | None = None
+) -> None:
     """
     Internal function, handles rotations from (rotation_counter - 2) to 0 and adds them to the
     node_groups dictionary
     """
-    previous_nodes = {}
+
+    previous_nodes: Dict[NodeId, PreviousNodeData] = {}
 
     for rotation_id in range(rotation.rotation_counter - 1, -1, -1):
         nodes = node_groups[rotation_id + 1]['nodes'].copy()
         for node_id in nodes:
             if node_id not in previous_nodes:
                 previous_node = skale.node_rotation.get_previous_node(schain_name, node_id)
                 if previous_node is not None:
                     finish_ts = skale.node_rotation.get_schain_finish_ts(previous_node, schain_name)
                     previous_nodes[node_id] = {
-                        'finish_ts': finish_ts,
+                        'finish_ts': finish_ts or 0,
                         'previous_node_id': previous_node
                     }
 
         new_node_id = max(previous_nodes.items(), key=lambda x: x[1]['finish_ts'])[0]
         previous_node_id = previous_nodes[new_node_id]['previous_node_id']
         public_key = skale.nodes.get_node_public_key(previous_node_id)
 
@@ -154,39 +164,44 @@
         del previous_nodes[new_node_id]
 
         if leaving_node_id and previous_node_id == leaving_node_id:
             logger.info(f'Finishing rotation history parsing: {leaving_node_id} found')
             break
 
 
-def _pop_previous_bls_public_key(previous_public_keys):
+def _pop_previous_bls_public_key(previous_public_keys: List[G2Point]) -> BlsPublicKey | None:
     """
     Returns BLS public key for the group and removes it from the list, returns None if node
     with provided node_id was kicked out of the chain because of failed DKG.
     """
     raw_bls_keys = previous_public_keys[-1]
     bls_keys = _compose_bls_public_key_info(raw_bls_keys)
     del previous_public_keys[-1]
     return bls_keys
 
 
-def _compose_bls_public_key_info(bls_public_key: str) -> dict:
+def _compose_bls_public_key_info(bls_public_key: G2Point) -> BlsPublicKey | None:
     if bls_public_key:
         return {
             'blsPublicKey0': str(bls_public_key[0][0]),
             'blsPublicKey1': str(bls_public_key[0][1]),
             'blsPublicKey2': str(bls_public_key[1][0]),
             'blsPublicKey3': str(bls_public_key[1][1])
         }
+    return None
 
 
-def get_new_nodes_list(skale: Skale, name: str, node_groups) -> list:
+def get_new_nodes_list(
+        skale: SkaleManager,
+        name: SchainName,
+        node_groups: Dict[int, NodesGroup]
+) -> list[NodeId]:
     """Returns list of new nodes in for the latest rotation"""
     logger.info(f'Getting new nodes list for chain {name}')
-    rotation = skale.node_rotation.get_rotation_obj(name)
+    rotation = skale.node_rotation.get_rotation(name)
     current_group_ids = node_groups[rotation.rotation_counter]['nodes'].keys()
     new_nodes = []
     for index in node_groups:
         past_rotation = node_groups[index]['rotation']
         if not past_rotation:
             continue
         if past_rotation['new_node_id'] in current_group_ids:
```

### Comparing `skale.py-7.dev11/skale/skale_base.py` & `skale.py-7.dev12/skale/skale_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,130 +17,137 @@
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
 import abc
 import logging
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Dict, Self, Type
 
 from skale_contracts import skale_contracts
 
-from skale.wallets import BaseWallet
 from skale.utils.exceptions import InvalidWalletError, EmptyWalletError
 from skale.utils.web3_utils import default_gas_price, init_web3
-
-from skale.contracts.contract_manager import ContractManager
+from skale.wallets import BaseWallet
 
 if TYPE_CHECKING:
-    from eth_typing import Address, ChecksumAddress
+    from eth_typing import ChecksumAddress
+    from skale.contracts.base_contract import BaseContract
+    from skale.utils.contract_info import ContractInfo
 
 
 logger = logging.getLogger(__name__)
 
 
 class EmptyPrivateKey(Exception):
     pass
 
 
 class SkaleBase:
     __metaclass__ = abc.ABCMeta
 
-    def __init__(self, endpoint, alias_or_address: str,
-                 wallet=None, state_path=None,
-                 ts_diff=None, provider_timeout=30):
+    def __init__(
+            self,
+            endpoint: str,
+            alias_or_address: str,
+            wallet: BaseWallet | None = None,
+            state_path: str | None = None,
+            ts_diff: int | None = None,
+            provider_timeout: int = 30):
         logger.info('Initializing skale.py, endpoint: %s, wallet: %s',
                     endpoint, type(wallet).__name__)
         self._endpoint = endpoint
         self.web3 = init_web3(endpoint,
                               state_path=state_path,
                               ts_diff=ts_diff,
                               provider_timeout=provider_timeout)
         self.network = skale_contracts.get_network_by_provider(self.web3.provider)
         self.project = self.network.get_project(self.project_name)
         self.instance = self.project.get_instance(alias_or_address)
-        self.__contracts = {}
-        self.__contracts_info = {}
+        self.__contracts: Dict[str, BaseContract[Self]] = {}
+        self.__contracts_info: Dict[str, ContractInfo[Self]] = {}
         self.set_contracts_info()
         if wallet:
             self.wallet = wallet
 
     @property
     @abc.abstractmethod
     def project_name(self) -> str:
         """Name of smart contracts project"""
 
     @property
-    def gas_price(self):
+    def gas_price(self) -> int:
         return default_gas_price(self.web3)
 
     @property
-    def wallet(self):
+    def wallet(self) -> BaseWallet:
         if not self._wallet:
             raise EmptyWalletError('No wallet provided')
         return self._wallet
 
     @wallet.setter
-    def wallet(self, wallet):
+    def wallet(self, wallet: BaseWallet) -> None:
         if issubclass(type(wallet), BaseWallet):
             self._wallet = wallet
         else:
             raise InvalidWalletError(f'Wrong wallet class: {type(wallet).__name__}. \
                                        Must be one of the BaseWallet subclasses')
 
-    def __is_debug_contracts(self, abi):
-        return abi.get('time_helpers_with_debug_address', None)
-
     @abc.abstractmethod
-    def set_contracts_info(self):
-        return
-
-    def init_contract_manager(self):
-        self.add_lib_contract('contract_manager', ContractManager, 'ContractManager')
+    def set_contracts_info(self) -> None:
+        pass
 
-    def __init_contract_from_info(self, contract_info):
+    def __init_contract_from_info(self, contract_info: ContractInfo[Self]) -> None:
         if contract_info.upgradeable:
             self.init_upgradeable_contract(contract_info)
         else:
             self.add_lib_contract(
                 contract_info.name,
                 contract_info.contract_class,
                 contract_info.contract_name
             )
 
-    def init_upgradeable_contract(self, contract_info):
+    def init_upgradeable_contract(self, contract_info: ContractInfo[Self]) -> None:
         address = self.get_contract_address(contract_info.contract_name)
         self.add_lib_contract(
             contract_info.name,
             contract_info.contract_class,
             contract_info.contract_name,
             address
         )
 
-    def add_lib_contract(self, name: str, contract_class,
-                         contract_name: str, contract_address: Address = None):
+    def add_lib_contract(
+            self,
+            name: str,
+            contract_class: Type[BaseContract[Self]],
+            contract_name: str,
+            contract_address: ChecksumAddress | None = None
+    ) -> None:
         address = contract_address or self.instance.get_contract_address(contract_name)
         logger.debug('Fetching abi for %s, address %s', name, address)
         contract_abi = self.instance.abi[contract_name]
         self.add_contract(name, contract_class(
             self, name, address, contract_abi))
 
-    def add_contract(self, name, contract):
+    def add_contract(self, name: str, contract: BaseContract[Self]) -> None:
         self.__contracts[name] = contract
 
-    def get_contract_address(self, name) -> ChecksumAddress:
+    def get_contract_address(self, name: str) -> ChecksumAddress:
         return self.web3.to_checksum_address(
             self.instance.get_contract_address(name)
         )
 
-    def __get_contract_by_name(self, name):
-        return self.__contracts[name]
-
-    def __getattr__(self, name):
+    def _get_contract(self, name: str) -> BaseContract[Self]:
         if name not in self.__contracts:
             if not self.__contracts_info.get(name):
                 logger.warning("%s method/contract wasn't found", name)
-                return None
+                raise ValueError(name, ' is an unknown contract')
             logger.debug("Contract %s wasn't inited, creating now", name)
             contract_info = self.__contracts_info[name]
             self.__init_contract_from_info(contract_info)
         return self.__get_contract_by_name(name)
+
+    def __get_contract_by_name(self, name: str) -> BaseContract[Self]:
+        return self.__contracts[name]
+
+    def __getattr__(self, name: str) -> BaseContract[Self]:
+        return self._get_contract(name)
```

### Comparing `skale.py-7.dev11/skale/skale_ima.py` & `skale.py-7.dev12/skale/contracts/manager/delegation/token_state.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,33 +13,36 @@
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
-import logging
+from eth_typing import ChecksumAddress
+from web3.contract.contract import ContractFunction
+from web3.types import Wei
+
+from skale.contracts.base_contract import transaction_method
+from skale.contracts.skale_manager_contract import SkaleManagerContract
+
+
+class TokenState(SkaleManagerContract):
+    """Wrapper for TokenState.sol functions"""
+
+    def get_and_update_locked_amount(self, holder_address: ChecksumAddress) -> Wei:
+        """This method is for check quantity of `freezed` tokens
+           :param holder_address: Address of the holder
+           :type holder_address: str
+           :returns:
+           :rtype: int
+        """
+        return Wei(self.contract.functions.getAndUpdateLockedAmount(holder_address).call())
+
+    @transaction_method
+    def grant_role(self, role: bytes, owner: ChecksumAddress) -> ContractFunction:
+        return self.contract.functions.grantRole(role, owner)
 
-from skale.skale_base import SkaleBase
-import skale.contracts.ima as contracts
-from skale.utils.contract_info import ContractInfo
-from skale.utils.contract_types import ContractTypes
-from skale.utils.helper import get_contracts_info
+    def has_role(self, role: bytes, address: ChecksumAddress) -> bool:
+        return bool(self.contract.functions.hasRole(role, address).call())
 
-
-logger = logging.getLogger(__name__)
-
-
-CONTRACTS_INFO = [
-    ContractInfo('linker', 'Linker',
-                 contracts.Linker, ContractTypes.API, False)
-]
-
-
-def spawn_skale_ima_lib(skale_ima):
-    """ Clone skale ima object with the same wallet """
-    return SkaleIma(skale_ima._endpoint, skale_ima._abi_filepath, skale_ima.wallet)
-
-
-class SkaleIma(SkaleBase):
-    def set_contracts_info(self):
-        self._SkaleBase__contracts_info = get_contracts_info(CONTRACTS_INFO)
+    def locker_manager_role(self) -> bytes:
+        return bytes(self.contract.functions.LOCKER_MANAGER_ROLE().call())
```

### Comparing `skale.py-7.dev11/skale/transactions/exceptions.py` & `skale.py-7.dev12/skale/transactions/exceptions.py`

 * *Files identical despite different names*

### Comparing `skale.py-7.dev11/skale/transactions/result.py` & `skale.py-7.dev12/skale/transactions/result.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,15 +14,18 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
 import enum
-from typing import NamedTuple
+from typing import Mapping, NamedTuple
+
+from web3.types import TxReceipt
+from eth_typing import HexStr
 
 from skale.transactions.exceptions import (
     DryRunFailedError,
     DryRunRevertError,
     TransactionFailedError
 )
 
@@ -32,19 +35,24 @@
     SUCCESS = 1
 
 
 class TxCallResult(NamedTuple):
     status: TxStatus
     error: str
     message: str
-    data: dict
+    data: Mapping[str, str | int]
 
 
 class TxRes:
-    def __init__(self, tx_call_result=None, tx_hash=None, receipt=None, revert=None):
+    def __init__(
+            self,
+            tx_call_result: TxCallResult | None = None,
+            tx_hash: HexStr | None = None,
+            receipt: TxReceipt | None = None
+    ):
         self.tx_call_result = tx_call_result
         self.tx_hash = tx_hash
         self.receipt = receipt
         self.attempts = 0
 
     def __str__(self) -> str:
         return (
@@ -57,13 +65,16 @@
             f'TxRes hash: {self.tx_hash}, tx_call_result {self.tx_call_result}, '
             f'receipt {self.receipt}'
         )
 
     def raise_for_status(self) -> None:
         if self.receipt is not None:
             if self.receipt['status'] == TxStatus.FAILED:
-                raise TransactionFailedError(self.receipt)
+                raise TransactionFailedError(
+                    "Tx status is failed",
+                    {key: str(value) for key, value in self.receipt.items()}
+                )
         elif self.tx_call_result is not None and self.tx_call_result.status == TxStatus.FAILED:
             if self.tx_call_result.error == 'revert':
                 raise DryRunRevertError(self.tx_call_result.message)
             else:
                 raise DryRunFailedError(self.tx_call_result.message)
```

### Comparing `skale.py-7.dev11/skale/transactions/tools.py` & `skale.py-7.dev12/skale/transactions/tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,40 +13,52 @@
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
+from __future__ import annotations
 import logging
 import time
 from functools import partial, wraps
-from typing import Dict, Optional
+from typing import Any, Callable, Optional, TYPE_CHECKING
 
+from eth_typing import ChecksumAddress
 from web3 import Web3
+from web3.contract.contract import ContractFunction
 from web3.exceptions import ContractLogicError, Web3Exception
 from web3._utils.transactions import get_block_gas_limit
+from web3.types import Nonce, TxParams, Wei
 
 import skale.config as config
 from skale.transactions.exceptions import TransactionError
 from skale.transactions.result import TxCallResult, TxRes, TxStatus
 from skale.utils.web3_utils import get_eth_nonce
 
+if TYPE_CHECKING:
+    from skale.skale_base import SkaleBase
+
 
 logger = logging.getLogger(__name__)
 
 
 DEFAULT_ETH_SEND_GAS_LIMIT = 22000
 
 
-def make_dry_run_call(skale, method, gas_limit=None, value=0) -> TxCallResult:
-    opts = {
+def make_dry_run_call(
+        skale: SkaleBase,
+        method: ContractFunction,
+        gas_limit: int | None = None,
+        value: Wei = Wei(0)
+) -> TxCallResult:
+    opts = TxParams({
         'from': skale.wallet.address,
         'value': value
-    }
+    })
     logger.info(
         f'Dry run tx: {method.fn_name}, '
         f'sender: {skale.wallet.address}, '
         f'wallet: {skale.wallet.__class__.__name__}, '
         f'value: {value}, '
     )
     estimated_gas = 0
@@ -56,25 +68,36 @@
             estimated_gas = gas_limit
             opts.update({'gas': gas_limit})
             method.call(opts)
         else:
             estimated_gas = estimate_gas(skale.web3, method, opts)
         logger.info(f'Estimated gas for {method.fn_name}: {estimated_gas}')
     except ContractLogicError as e:
-        return TxCallResult(status=TxStatus.FAILED,
-                            error='revert', message=e.message, data=e.data)
+        message = e.message or 'Contract logic error'
+        error_data = e.data or {}
+        data = {'data': error_data} if isinstance(error_data, str) else error_data
+        return TxCallResult(
+            status=TxStatus.FAILED,
+            error='revert',
+            message=message,
+            data=data
+        )
     except (Web3Exception, ValueError) as e:
         logger.exception('Dry run for %s failed', method)
         return TxCallResult(status=TxStatus.FAILED, error='exception', message=str(e), data={})
 
-    return TxCallResult(status=TxStatus.SUCCESS, error='',
-                        message='success', data={'gas': estimated_gas})
+    return TxCallResult(
+        status=TxStatus.SUCCESS,
+        error='',
+        message='success',
+        data={'gas': estimated_gas}
+    )
 
 
-def estimate_gas(web3, method, opts):
+def estimate_gas(web3: Web3, method: ContractFunction, opts: TxParams) -> int:
     try:
         block_gas_limit = get_block_gas_limit(web3)
     except AttributeError:
         block_gas_limit = get_block_gas_limit(web3)
 
     estimated_gas = method.estimate_gas(
         opts,
@@ -86,99 +109,108 @@
     if normalized_estimated_gas > block_gas_limit:
         logger.warning(f'Estimate gas for {method.fn_name} - {normalized_estimated_gas} exceeds \
 block gas limit, going to use block_gas_limit ({block_gas_limit}) for this transaction')
         return block_gas_limit
     return normalized_estimated_gas
 
 
-def build_tx_dict(method, *args, **kwargs):
+def build_tx_dict(method: ContractFunction, *args: Any, **kwargs: Any) -> TxParams:
     base_fields = compose_base_fields(*args, **kwargs)
     return method.build_transaction(base_fields)
 
 
 def compose_base_fields(
-    nonce: int,
+    nonce: Nonce,
     gas_limit: int,
-    gas_price: Optional[int] = None,
-    max_fee_per_gas: Optional[int] = None,
-    max_priority_fee_per_gas: Optional[int] = None,
-    value: Optional[int] = 0,
-) -> Dict:
-    fee_fields = {
+    gas_price: Wei | None = None,
+    max_fee_per_gas: Wei | None = None,
+    max_priority_fee_per_gas: Wei | None = None,
+    value: Wei = Wei(0),
+) -> TxParams:
+    fee_fields = TxParams({
         'gas': gas_limit,
         'nonce': nonce,
         'value': value
-    }
-    if max_priority_fee_per_gas is not None:
+    })
+    if max_priority_fee_per_gas is not None and max_fee_per_gas is not None:
         fee_fields.update({
             'maxPriorityFeePerGas': max_priority_fee_per_gas,
             'maxFeePerGas': max_fee_per_gas
         })
         fee_fields.update({'type': 2})
     elif gas_price is not None:
         fee_fields.update({'gasPrice': gas_price})
         fee_fields.update({'type': 1})
     return fee_fields
 
 
 def transaction_from_method(
-    method,
+    method: ContractFunction,
     *,
     multiplier: Optional[float] = None,
     priority: Optional[int] = None,
-    **kwargs
-) -> str:
+    **kwargs: Any
+) -> TxParams:
     tx = build_tx_dict(method, **kwargs)
     logger.info(
         f'Tx: {method.fn_name}, '
         f'Fields: {tx}, '
     )
     return tx
 
 
 def compose_eth_transfer_tx(
     web3: Web3,
-    from_address: str,
-    to_address: str,
-    value: int,
-    **kwargs
-) -> Dict:
+    from_address: ChecksumAddress,
+    to_address: ChecksumAddress,
+    value: Wei,
+    **kwargs: Any
+) -> TxParams:
     nonce = get_eth_nonce(web3, from_address)
     base_fields = compose_base_fields(
         nonce=nonce,
         gas_limit=DEFAULT_ETH_SEND_GAS_LIMIT,
         value=value,
         **kwargs
     )
-    tx = {
+    tx = TxParams({
         'from': from_address,
         'to': to_address,
         **base_fields
-    }
+    })
     return tx
 
 
-def retry_tx(tx=None, *, max_retries=3, timeout=-1):
+def retry_tx(
+        tx: Callable[..., TxRes] | None = None,
+        *,
+        max_retries: int = 3,
+        timeout: int = -1
+) -> Callable[..., TxRes | None] | partial[Any]:
     if tx is None:
         return partial(retry_tx, max_retries=3, timeout=timeout)
 
     @wraps(tx)
-    def wrapper(*args, **kwargs):
+    def wrapper(*args: Any, **kwargs: Any) -> TxRes | None:
         return run_tx_with_retry(
             tx, *args,
             max_retries=max_retries,
             retry_timeout=timeout, **kwargs
         )
     return wrapper
 
 
-def run_tx_with_retry(transaction, *args, max_retries=3,
-                      retry_timeout=-1,
-                      raise_for_status=True,
-                      **kwargs) -> TxRes:
+def run_tx_with_retry(
+        transaction: Callable[..., TxRes],
+        *args: Any,
+        max_retries: int = 3,
+        retry_timeout: int = -1,
+        raise_for_status: bool = True,
+        **kwargs: Any
+) -> TxRes | None:
     attempt = 0
     tx_res = None
     exp_timeout = 1
     error = None
     while attempt < max_retries:
         try:
             tx_res = transaction(
```

### Comparing `skale.py-7.dev11/skale/utils/account_tools.py` & `skale.py-7.dev12/skale/utils/account_tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,48 +14,67 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 """ Account utilities """
 
+from __future__ import annotations
+from decimal import Decimal
 import logging
-from typing import Optional
+from typing import Any, Dict, List, Literal, Optional, TYPE_CHECKING, Type, TypedDict
 
+from eth_typing import ChecksumAddress
 from web3 import Web3
+from web3.types import TxReceipt, Wei
 
+from skale.transactions.result import TxRes
 from skale.transactions.tools import compose_eth_transfer_tx
 from skale.utils.constants import LONG_LINE
 from skale.wallets import LedgerWallet, Web3Wallet
 from skale.utils.web3_utils import (
     check_receipt,
     default_gas_price,
     wait_for_confirmation_blocks
 )
 
+if TYPE_CHECKING:
+    from skale.skale_manager import SkaleManager
+    from skale.wallets.common import BaseWallet
+
+
 logger = logging.getLogger(__name__)
 
 
-WALLET_TYPE_TO_CLASS = {
+class AccountData(TypedDict):
+    address: ChecksumAddress
+    private_key: str
+
+
+WALLET_TYPE_TO_CLASS: Dict[str, Type[LedgerWallet] | Type[Web3Wallet]] = {
     'ledger': LedgerWallet,
     'web3': Web3Wallet
 }
 
 
-def create_wallet(wallet_type='web3', *args, **kwargs):
+def create_wallet(
+        wallet_type: Literal['web3'] | Literal['ledger'] = 'web3',
+        *args: Any,
+        **kwargs: Any
+) -> LedgerWallet | Web3Wallet:
     return WALLET_TYPE_TO_CLASS[wallet_type](*args, **kwargs)
 
 
 def send_tokens(
-    skale,
-    receiver_address,
-    amount,
-    *args,
-    **kwargs
-):
+    skale: SkaleManager,
+    receiver_address: ChecksumAddress,
+    amount: Wei,
+    *args: Any,
+    **kwargs: Any
+) -> TxRes:
     logger.info(
         f'Sending {amount} SKALE tokens from {skale.wallet.address} => '
         f'{receiver_address}'
     )
 
     wei_amount = skale.web3.to_wei(amount, 'ether')
     return skale.token.transfer(
@@ -64,38 +83,38 @@
         *args,
         **kwargs
     )
 
 
 def send_eth(
     web3: Web3,
-    wallet,
-    receiver_address,
-    amount,
-    *args,
+    wallet: BaseWallet,
+    receiver_address: ChecksumAddress,
+    amount: Wei,
+    *args: Any,
     gas_price: Optional[int] = None,
     wait_for: bool = True,
     confirmation_blocks: int = 0,
     multiplier: Optional[int] = None,
     priority: Optional[int] = None,
-    **kwargs
-):
+    **kwargs: Any
+) -> TxReceipt:
     logger.info(
         f'Sending {amount} ETH from {wallet.address} => '
         f'{receiver_address}'
     )
     wei_amount = web3.to_wei(amount, 'ether')
     gas_price = gas_price or default_gas_price(web3)
     tx = compose_eth_transfer_tx(
-        web3=web3,
-        *args,
+        web3,
+        wallet.address,
+        receiver_address,
+        wei_amount,
         gas_price=gas_price,
-        from_address=wallet.address,
-        to_address=receiver_address,
-        value=wei_amount,
+        *args,
         **kwargs
     )
     tx_hash = wallet.sign_and_send(
         tx,
         multiplier=multiplier,
         priority=priority
     )
@@ -106,46 +125,48 @@
             web3,
             confirmation_blocks
         )
     check_receipt(receipt)
     return receipt
 
 
-def account_eth_balance_wei(web3, address):
+def account_eth_balance_wei(web3: Web3, address: ChecksumAddress) -> Wei:
     return web3.eth.get_balance(address)
 
 
-def check_ether_balance(web3, address):
+def check_ether_balance(web3: Web3, address: ChecksumAddress) -> int | Decimal:
     balance_wei = account_eth_balance_wei(web3, address)
     balance = web3.from_wei(balance_wei, 'ether')
 
     logger.info(f'{address} balance: {balance} ETH')
     return balance
 
 
-def check_skale_balance(skale, address):
+def check_skale_balance(skale: SkaleManager, address: ChecksumAddress) -> int | Decimal:
     balance_wei = skale.token.get_balance(address)
     balance = skale.web3.from_wei(balance_wei, 'ether')
     logger.info(f'{address} balance: {balance} SKALE')
     return balance
 
 
-def generate_account(web3):
+def generate_account(web3: Web3) -> AccountData:
     account = web3.eth.account.create()
     private_key = account.key.hex()
     logger.info(f'Generated account: {account.address}')
-    return {'address': account.address, 'private_key': private_key}
+    return AccountData({'address': account.address, 'private_key': private_key})
 
 
-def generate_accounts(skale,
-                      base_wallet,
-                      n_wallets,
-                      skale_amount,
-                      eth_amount,
-                      debug=False):
+def generate_accounts(
+        skale: SkaleManager,
+        base_wallet: BaseWallet,
+        n_wallets: int,
+        skale_amount: Wei,
+        eth_amount: Wei,
+        debug: bool = False
+) -> List[AccountData]:
     n_wallets = int(n_wallets)
     results = []
 
     for _ in range(0, n_wallets):
         wallet = generate_account(skale.web3)
 
         send_tokens(skale, wallet['address'], skale_amount)
```

### Comparing `skale.py-7.dev11/skale/utils/constants.py` & `skale.py-7.dev12/skale/utils/constants.py`

 * *Files identical despite different names*

### Comparing `skale.py-7.dev11/skale/utils/contract_info.py` & `skale.py-7.dev12/skale/utils/contract_types.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,21 +12,16 @@
 #   SKALE.py is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
-""" Contract info utilities """
+""" Contract type utilities """
 
-from typing import NamedTuple
+from enum import Enum
 
-from skale.contracts.base_contract import BaseContract
-from skale.utils.contract_types import ContractTypes
 
-
-class ContractInfo(NamedTuple):
-    name: str
-    contract_name: str
-    contract_class: BaseContract
-    type: ContractTypes
-    upgradeable: bool
+class ContractTypes(Enum):
+    API = 0
+    DATA = 1
+    INTERNAL = 2
```

### Comparing `skale.py-7.dev11/skale/utils/contracts_provision/__init__.py` & `skale.py-7.dev12/skale/utils/contracts_provision/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,27 +13,30 @@
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
-from skale.contracts.allocator.allocator import TimeUnit
+from web3.types import Wei
+
+from skale.types.allocation import TimeUnit
+from skale.types.validator import ValidatorId
 
 # manager test constants
 
 DEFAULT_NODE_NAME = 'test_node'
 SECOND_NODE_NAME = 'test_node_2'
 
 DEFAULT_SCHAIN_NAME = 'test_schain_1'
 
 DEFAULT_DOMAIN_NAME = 'skale.test'
 
 INITIAL_DELEGATION_PERIOD = 2
-D_VALIDATOR_ID = 1
+D_VALIDATOR_ID = ValidatorId(1)
 D_VALIDATOR_NAME = 'test'
 D_VALIDATOR_DESC = 'test'
 D_VALIDATOR_FEE = 10
 D_VALIDATOR_MIN_DEL = 1000000
 
 D_DELEGATION_PERIOD = 2
 D_STAKE_MULTIPLIER = 100
@@ -56,10 +59,10 @@
 WEI_MULTIPLIER = 10 ** 18
 
 TEST_FULL_AMOUNT = 5000 * WEI_MULTIPLIER
 TEST_LOCKUP_AMOUNT = 1000 * WEI_MULTIPLIER
 
 POLL_INTERVAL = 2
 
-TEST_SKALE_AMOUNT = 100000
+TEST_SKALE_AMOUNT = Wei(100000)
 
 D_PLAN_ID = 1
```

### Comparing `skale.py-7.dev11/skale/utils/contracts_provision/allocator.py` & `skale.py-7.dev12/skale/utils/contracts_provision/allocator.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,54 +15,69 @@
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
 from time import sleep
 
+from web3.contract.contract import ContractEvent
+from web3.types import LogReceipt, Wei
+from web3._utils.filters import LogFilter
+
+from skale.skale_allocator import SkaleAllocator
+from skale.skale_manager import SkaleManager
 from skale.utils.account_tools import send_tokens
 from skale.utils.contracts_provision import (
     TEST_SKALE_AMOUNT, TEST_VESTING_CLIFF, TEST_TOTAL_VESTING_DURATION,
     TEST_VESTING_INTERVAL_TIME_UNIT, TEST_VESTING_INTERVAL, TEST_CAN_DELEGATE,
     TEST_IS_TERMINATABLE, POLL_INTERVAL, TEST_START_MONTH, TEST_FULL_AMOUNT, TEST_LOCKUP_AMOUNT
 )
+from skale.wallets.common import BaseWallet
 
 
-def _catch_event(event_obj):
-    event_filter = event_obj.createFilter(
+def _catch_event(event_obj: ContractEvent) -> LogReceipt:
+    event_filter: LogFilter = event_obj.create_filter(
         fromBlock=0,
         toBlock='latest'
     )
     while True:
         for event in event_filter.get_all_entries():
             return event
         sleep(POLL_INTERVAL)
 
 
-def transfer_tokens_to_allocator(skale_manager, skale_allocator, amount=TEST_SKALE_AMOUNT):
+def transfer_tokens_to_allocator(
+        skale_manager: SkaleManager,
+        skale_allocator: SkaleAllocator,
+        amount: Wei = TEST_SKALE_AMOUNT
+) -> None:
     send_tokens(skale_manager, skale_allocator.allocator.address, amount)
 
 
 # def transfer_tokens_to_token_launch_manager(skale, amount=TEST_SKALE_AMOUNT):
 #     send_tokens(skale, skale.wallet, skale.token_launch_manager.address, amount)
 
 
-def add_test_plan(skale_allocator):
+def add_test_plan(skale_allocator: SkaleAllocator) -> int:
     skale_allocator.allocator.add_plan(
         vesting_cliff=TEST_VESTING_CLIFF,
         total_vesting_duration=TEST_TOTAL_VESTING_DURATION,
         vesting_interval_time_unit=TEST_VESTING_INTERVAL_TIME_UNIT,
         vesting_interval=TEST_VESTING_INTERVAL,
         can_delegate=TEST_CAN_DELEGATE,
         is_terminatable=TEST_IS_TERMINATABLE
     )
     return len(skale_allocator.allocator.get_all_plans())
 
 
-def connect_test_beneficiary(skale_allocator, plan_id, wallet):
+def connect_test_beneficiary(
+        skale_allocator: SkaleAllocator,
+        plan_id: int,
+        wallet: BaseWallet
+) -> None:
     skale_allocator.allocator.connect_beneficiary_to_plan(
         beneficiary_address=wallet.address,
         plan_id=plan_id,
         start_month=TEST_START_MONTH,
         full_amount=TEST_FULL_AMOUNT,
         lockup_amount=TEST_LOCKUP_AMOUNT
     )
```

### Comparing `skale.py-7.dev11/skale/utils/contracts_provision/fake_multisig_contract.py` & `skale.py-7.dev12/skale/utils/contracts_provision/fake_multisig_contract.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,19 +16,21 @@
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
 import os
 import json
 
-from skale.transactions.tools import transaction_from_method
+from web3 import Web3
+
 from skale.utils.web3_utils import (
     get_eth_nonce,
     wait_for_receipt_by_blocks
 )
+from skale.wallets.common import BaseWallet
 
 # Usage note: to change this contract update the code, compile it and put the new bytecode and
 # new ABI below
 
 FAKE_MULTISIG_CONTRACT = """
 pragma solidity ^0.8.0;
 
@@ -72,28 +74,26 @@
 DIR_PATH = os.path.dirname(os.path.realpath(__file__))
 FAKE_MULTISIG_DATA_DEFAULT_PATH = os.path.join(DIR_PATH, 'fake_multisig_data.json')
 FAKE_MULTISIG_DATA_PATH = os.getenv('FAKE_MULTISIG_DATA_PATH') or FAKE_MULTISIG_DATA_DEFAULT_PATH
 
 FAKE_MULTISIG_CONSTRUCTOR_GAS = 1000000
 
 
-def deploy_fake_multisig_contract(web3, wallet):
+def deploy_fake_multisig_contract(web3: Web3, wallet: BaseWallet) -> None:
     print('Going to deploy simple payable contract')
     FakeMultisigContract = web3.eth.contract(abi=FAKE_MULTISIG_ABI, bytecode=FAKE_MULTISIG_BYTECODE)
     constructor = FakeMultisigContract.constructor()
-    constructor.fn_name = 'fake_multisig_constructor'
-    tx = transaction_from_method(
-        constructor,
-        nonce=get_eth_nonce(web3, wallet.address),
-        gas_price=3 * 10 ** 9,
-        gas_limit=FAKE_MULTISIG_CONSTRUCTOR_GAS
-    )
+    tx = constructor.build_transaction({
+        'nonce': get_eth_nonce(web3, wallet.address),
+        'gasPrice': 3 * 10 ** 9,
+        'gas': FAKE_MULTISIG_CONSTRUCTOR_GAS
+    })
     tx_hash = wallet.sign_and_send(tx)
     receipt = wait_for_receipt_by_blocks(web3, tx_hash)
-    print(f'Sample contract successfully deployed: {receipt.contractAddress}')
+    print(f"Sample contract successfully deployed: {receipt['contractAddress']}")
     content = {
-        'address': receipt.contractAddress,
+        'address': receipt['contractAddress'],
         'abi': FAKE_MULTISIG_ABI
     }
     with open(FAKE_MULTISIG_DATA_PATH, 'w') as outfile:
         json.dump(content, outfile, indent=4)
     print(f'Sample contract data successfully saved to {FAKE_MULTISIG_DATA_PATH}')
```

### Comparing `skale.py-7.dev11/skale/utils/contracts_provision/main.py` & `skale.py-7.dev12/skale/utils/contracts_provision/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,24 @@
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
+from typing import List, Tuple
+from eth_typing import ChecksumAddress
 from web3 import Web3
+from web3.types import RPCEndpoint
 
-from skale.contracts.manager.nodes import NodeStatus
+from skale.dataclasses.schain_options import SchainOptions
+from skale.skale_manager import SkaleManager
 from skale.transactions.result import TxRes
+from skale.types.node import NodeId, NodeStatus
+from skale.types.validator import ValidatorId
 from skale.utils.contracts_provision import (
     D_VALIDATOR_ID,
     D_VALIDATOR_MIN_DEL,
     D_DELEGATION_PERIOD,
     D_DELEGATION_INFO,
     D_VALIDATOR_NAME,
     D_VALIDATOR_DESC,
@@ -44,38 +50,39 @@
 
 DEFAULT_MINING_INTERVAL = 1000
 TEST_SRW_FUND_VALUE = 3000000000000000000
 
 
 def _skip_evm_time(web3: Web3, seconds: int, mine: bool = True) -> int:
     """For test purposes only, works only with hardhat node"""
-    res = web3.provider.make_request('evm_increaseTime', [seconds])
-    web3.provider.make_request("evm_mine", [])
+    res = web3.provider.make_request(RPCEndpoint('evm_increaseTime'), [seconds])
+    if mine:
+        web3.provider.make_request(RPCEndpoint('evm_mine'), [])
     return int(res['result'])
 
 
 def set_automining(web3: Web3, value: bool) -> int:
-    res = web3.provider.make_request('evm_setAutomine', [value])
+    res = web3.provider.make_request(RPCEndpoint('evm_setAutomine'), [value])
     return int(res['result'])
 
 
 def set_mining_interval(web3: Web3, ms: int) -> int:
-    res = web3.provider.make_request('evm_setIntervalMining', [ms])
+    res = web3.provider.make_request(RPCEndpoint('evm_setIntervalMining'), [ms])
     return int(res['result'])
 
 
-def set_default_mining_interval(web3) -> int:
+def set_default_mining_interval(web3: Web3) -> int:
     return set_mining_interval(web3, DEFAULT_MINING_INTERVAL)
 
 
-def add_test_permissions(skale):
+def add_test_permissions(skale: SkaleManager) -> None:
     add_all_permissions(skale, skale.wallet.address)
 
 
-def add_all_permissions(skale, address):
+def add_all_permissions(skale: SkaleManager, address: ChecksumAddress) -> None:
     default_admin_role = skale.manager.default_admin_role()
     if not skale.manager.has_role(default_admin_role, address):
         skale.manager.grant_role(default_admin_role, address)
 
     schain_creator_role = skale.schains.schain_creator_role()
     if not skale.schains.has_role(schain_creator_role, address):
         skale.schains.grant_role(schain_creator_role, address)
@@ -133,92 +140,92 @@
         skale.delegation_period_manager.grant_role(delegation_period_setter_role, address)
 
     penalty_setter_role = skale.slashing_table.penalty_setter_role()
     if not skale.slashing_table.has_role(penalty_setter_role, address):
         skale.slashing_table.grant_role(penalty_setter_role, address)
 
 
-def add_test2_schain_type(skale) -> TxRes:
+def add_test2_schain_type(skale: SkaleManager) -> TxRes:
     part_of_node = 1
     number_of_nodes = 2
     return skale.schains_internal.add_schain_type(
         part_of_node, number_of_nodes
     )
 
 
-def add_test4_schain_type(skale) -> TxRes:
+def add_test4_schain_type(skale: SkaleManager) -> TxRes:
     part_of_node = 1
     number_of_nodes = 4
     return skale.schains_internal.add_schain_type(
         part_of_node, number_of_nodes
     )
 
 
-def cleanup_nodes(skale, ids=()):
+def cleanup_nodes(skale: SkaleManager, ids: list[NodeId] | None = None) -> None:
     active_ids = filter(
         lambda i: skale.nodes.get_node_status(i) == NodeStatus.ACTIVE,
         ids or skale.nodes.get_active_node_ids()
     )
     for node_id in active_ids:
         if skale.nodes.get(node_id):
             skale.nodes.init_exit(node_id)
             skale.manager.node_exit(node_id)
 
 
-def cleanup_schains(skale):
+def cleanup_schains(skale: SkaleManager) -> None:
     for schain_id in skale.schains_internal.get_all_schains_ids():
         schain_data = skale.schains.get(schain_id)
-        schain_name = schain_data.get('name', None)
+        schain_name = schain_data.name
         if schain_name is not None:
             skale.manager.delete_schain_by_root(schain_name, wait_for=True)
 
 
-def cleanup_nodes_schains(skale):
+def cleanup_nodes_schains(skale: SkaleManager) -> None:
     print('Cleanup nodes and schains')
     cleanup_schains(skale)
     cleanup_nodes(skale)
 
 
-def create_clean_schain(skale):
+def create_clean_schain(skale: SkaleManager) -> str:
     cleanup_nodes_schains(skale)
-    create_nodes(skale)
+    create_nodes([skale])
     return create_schain(skale, random_name=True)
 
 
-def create_node(skale) -> str:
+def create_node(skale: SkaleManager) -> str:
     cleanup_nodes_schains(skale)
     ip, public_ip, port, name = generate_random_node_data()
     skale.manager.create_node(
         ip=ip,
         port=port,
         name=name,
         domain_name=DEFAULT_DOMAIN_NAME,
         public_ip=public_ip,
         wait_for=True
     )
     return name
 
 
-def validator_exist(skale):
+def validator_exist(skale: SkaleManager) -> bool:
     return skale.validator_service.validator_address_exists(
         skale.wallet.address
     )
 
 
-def add_delegation_period(skale):
+def add_delegation_period(skale: SkaleManager) -> None:
     is_added = skale.delegation_period_manager.is_delegation_period_allowed(D_DELEGATION_PERIOD)
     if not is_added:
         skale.delegation_period_manager.set_delegation_period(
             months_count=D_DELEGATION_PERIOD,
             stake_multiplier=D_STAKE_MULTIPLIER,
             wait_for=True
         )
 
 
-def setup_validator(skale):
+def setup_validator(skale: SkaleManager) -> int:
     """Create and activate a validator"""
     set_test_msr(skale)
     print('Address', skale.wallet.address)
     if not validator_exist(skale):
         create_validator(skale)
     else:
         print('Skipping default validator creation')
@@ -230,126 +237,130 @@
         validator_id
     )
     accept_pending_delegation(skale, delegations[-1]['id'])
     _skip_evm_time(skale.web3, MONTH_IN_SECONDS)
     return validator_id
 
 
-def link_address_to_validator(skale):
+def link_address_to_validator(skale: SkaleManager) -> None:
     print('Linking address to validator')
     signature = skale.validator_service.get_link_node_signature(D_VALIDATOR_ID)
     tx_res = skale.validator_service.link_node_address(
         node_address=skale.wallet.address,
         signature=signature,
         wait_for=True
     )
     tx_res.raise_for_status()
 
 
-def link_nodes_to_validator(skale, validator_id, node_skale_objs=()):
+def link_nodes_to_validator(
+        skale: SkaleManager,
+        validator_id: ValidatorId,
+        node_skale_objs: Tuple[SkaleManager] | None = None
+) -> None:
     print('Linking address to validator')
     node_skale_objs = node_skale_objs or (skale,)
     validator_id = validator_id or D_VALIDATOR_ID
     for node_skale in node_skale_objs:
         signature = node_skale.validator_service.get_link_node_signature(
             validator_id
         )
         skale.validator_service.link_node_address(
             node_address=node_skale.wallet.address,
             signature=signature
         )
 
 
-def skip_delegation_delay(skale, delegation_id):
+def skip_delegation_delay(skale: SkaleManager, delegation_id: int) -> None:
     print(f'Activating delegation with ID {delegation_id}')
     skale.token_state._skip_transition_delay(
         delegation_id,
         wait_for=True
     )
 
 
-def accept_pending_delegation(skale, delegation_id):
+def accept_pending_delegation(skale: SkaleManager, delegation_id: int) -> None:
     print(f'Accepting delegation with ID: {delegation_id}')
     skale.delegation_controller.accept_pending_delegation(
         delegation_id=delegation_id,
         wait_for=True
     )
 
 
-def get_test_delegation_amount(skale):
+def get_test_delegation_amount(skale: SkaleManager) -> int:
     msr = skale.constants_holder.msr()
     return msr * 30
 
 
-def set_test_msr(skale, msr=D_VALIDATOR_MIN_DEL):
+def set_test_msr(skale: SkaleManager, msr: int = D_VALIDATOR_MIN_DEL) -> None:
     skale.constants_holder._set_msr(
         new_msr=msr,
         wait_for=True
     )
 
 
-def set_test_mda(skale):
+def set_test_mda(skale: SkaleManager) -> None:
     skale.validator_service.set_validator_mda(0, wait_for=True)
 
 
-def delegate_to_validator(skale, validator_id=D_VALIDATOR_ID):
+def delegate_to_validator(skale: SkaleManager, validator_id: int = D_VALIDATOR_ID) -> None:
     print(f'Delegating tokens to validator ID: {validator_id}')
     skale.delegation_controller.delegate(
         validator_id=validator_id,
         amount=get_test_delegation_amount(skale),
         delegation_period=INITIAL_DELEGATION_PERIOD,
         info=D_DELEGATION_INFO,
         wait_for=True
     )
 
 
-def enable_validator(skale, validator_id=D_VALIDATOR_ID):
+def enable_validator(skale: SkaleManager, validator_id: int = D_VALIDATOR_ID) -> None:
     print(f'Enabling validator ID: {D_VALIDATOR_ID}')
     skale.validator_service._enable_validator(validator_id, wait_for=True)
 
 
-def create_validator(skale):
+def create_validator(skale: SkaleManager) -> None:
     print('Creating default validator')
     skale.validator_service.register_validator(
         name=D_VALIDATOR_NAME,
         description=D_VALIDATOR_DESC,
         fee_rate=D_VALIDATOR_FEE,
         min_delegation_amount=D_VALIDATOR_MIN_DEL,
         wait_for=True
     )
 
 
-def create_nodes(skales, names=()):
+def create_nodes(skales: List[SkaleManager], names: List[str] | None = None) -> list[int]:
     # create couple of nodes
     print('Creating two nodes')
     node_names = names or (DEFAULT_NODE_NAME, SECOND_NODE_NAME)
     for skale, name in zip(skales, node_names):
         ip, public_ip, port, _ = generate_random_node_data()
         skale.manager.create_node(
             ip=ip,
             port=port,
             name=name,
             domain_name=DEFAULT_DOMAIN_NAME,
             public_ip=public_ip,
             wait_for=True
         )
     ids = [
-        skale.nodes.node_name_to_index(name)
+        skales[0].nodes.node_name_to_index(name)
         for name in node_names
     ]
     return ids
 
 
 def create_schain(
-    skale,
-    schain_name=DEFAULT_SCHAIN_NAME,
-    schain_type=1,
-    random_name=False,
-    schain_options=None
-):
+    skale: SkaleManager,
+    schain_name: str = DEFAULT_SCHAIN_NAME,
+    schain_type: int = 1,
+    random_name: bool = False,
+    schain_options: SchainOptions | None = None
+) -> str:
     print('Creating schain')
     # create 1 s-chain
     type_of_nodes, lifetime_seconds, name = generate_random_schain_data(skale)
 
     if random_name:
         schain_name = name
```

### Comparing `skale.py-7.dev11/skale/utils/contracts_provision/utils.py` & `skale.py-7.dev12/skale/utils/contracts_provision/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,31 +16,34 @@
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
 import random
 import string
 
+from skale.skale_manager import SkaleManager
+from skale.types.node import Port
 
-def generate_random_ip():
+
+def generate_random_ip() -> str:
     return '.'.join('%s' % random.randint(0, 255) for i in range(4))
 
 
-def generate_random_name(len=8):
+def generate_random_name(length: int = 8) -> str:
     return ''.join(
-        random.choices(string.ascii_uppercase + string.digits, k=len)
+        random.choices(string.ascii_uppercase + string.digits, k=length)
     )
 
 
-def generate_random_port():
-    return random.randint(0, 60000)
+def generate_random_port() -> Port:
+    return Port(random.randint(0, 60000))
 
 
-def generate_random_node_data():
+def generate_random_node_data() -> tuple[str, str, int, str]:
     return generate_random_ip(), generate_random_ip(), \
         generate_random_port(), generate_random_name()
 
 
-def generate_random_schain_data(skale):
+def generate_random_schain_data(skale: SkaleManager) -> tuple[int, int, str]:
     schain_type = skale.schains_internal.number_of_schain_types()
     lifetime_seconds = 3600  # 1 hour
     return schain_type, lifetime_seconds, generate_random_name()
```

### Comparing `skale.py-7.dev11/skale/utils/exceptions.py` & `skale.py-7.dev12/skale/utils/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,10 +32,10 @@
 
 class SChainNotFoundException(Exception):
     """Raised when requested sChain is not found"""
 
 
 class InvalidNodeIdError(Exception):
     """Raised when wrong node id passed"""
-    def __init__(self, node_id):
+    def __init__(self, node_id: int):
         message = f'Node with ID = {node_id} doesn\'t exist!'
         super().__init__(message)
```

### Comparing `skale.py-7.dev11/skale/utils/helper.py` & `skale.py-7.dev12/skale/utils/helper.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,47 +14,77 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 """ SKALE helper utilities """
 
+from __future__ import annotations
+
 import ipaddress
 import json
 import logging
 import random
 import socket
 import string
 import sys
 from logging import Formatter, StreamHandler
 from random import randint
+from typing import TYPE_CHECKING, Any, Callable, Dict, Generator, List, cast
 
 from skale.config import ENV
+from skale.types.node import Port
+
+if TYPE_CHECKING:
+    from skale.contracts.base_contract import SkaleType
+    from skale.utils.contract_info import ContractInfo
 
 
 logger = logging.getLogger(__name__)
 
 
-def decapitalize(s):
+def decapitalize(s: str) -> str:
     return s[:1].lower() + s[1:] if s else ''
 
 
-def format_fields(fields, flist=False):
+WrapperReturnType = Dict[str, Any] | List[Dict[str, Any]] | None
+
+
+def format_fields(
+        fields: list[str],
+        flist: bool = False
+) -> Callable[
+    [
+        Callable[
+            ...,
+            List[Any]
+        ]
+    ],
+    Callable[..., WrapperReturnType]
+]:
     """
         Transform array to object with passed fields
         Usage:
         @format(['field_name1', 'field_name2'])
         def my_method()
             return [0, 'Test']
 
         => {'field_name1': 0, 'field_name2': 'Test'}
     """
 
-    def real_decorator(function):
-        def wrapper(*args, **kwargs):
+    def real_decorator(
+            function: Callable[
+                ...,
+                List[Any]
+            ]
+    ) -> Callable[..., WrapperReturnType]:
+        def wrapper(
+                *args: Any,
+                **kwargs: Any
+        ) -> WrapperReturnType:
             result = function(*args, **kwargs)
 
             if result is None:
                 return None
 
             if not isinstance(result, list) and not isinstance(result, tuple):
                 return result
@@ -82,120 +112,122 @@
     return socket.inet_ntoa(packed)
 
 
 def ip_to_bytes(ip: str) -> bytes:  # pragma: no cover
     return socket.inet_aton(ip)
 
 
-def is_valid_ipv4_address(address):
+def is_valid_ipv4_address(address: str) -> bool:
     try:
         ipaddress.IPv4Address(address)
     except ValueError:
         return False
     return True
 
 
-def get_abi(abi_filepath: string = None):
+def get_abi(abi_filepath: str | None = None) -> dict[str, Any]:
     if abi_filepath:
         with open(abi_filepath, encoding='utf-8') as data_file:
-            return json.load(data_file)
+            return cast(dict[str, Any], json.load(data_file))
     return {}
 
 
-def get_skale_manager_address(abi_filepath: string = None) -> str:
-    return get_abi(abi_filepath)['skale_manager_address']
+def get_skale_manager_address(abi_filepath: str | None = None) -> str:
+    return cast(str, get_abi(abi_filepath)['skale_manager_address'])
 
 
-def get_allocator_address(abi_filepath: string = None) -> str:
-    return get_abi(abi_filepath)['allocator_address']
+def get_allocator_address(abi_filepath: str | None = None) -> str:
+    return cast(str, get_abi(abi_filepath)['allocator_address'])
 
 
-def generate_nonce():  # pragma: no cover
+def generate_nonce() -> int:  # pragma: no cover
     return randint(0, 65534)
 
 
-def random_string(size=6, chars=string.ascii_lowercase):  # pragma: no cover
+def random_string(size: int = 6, chars: str = string.ascii_lowercase) -> str:  # pragma: no cover
     return ''.join(random.choice(chars) for x in range(size))
 
 
-def generate_random_ip():  # pragma: no cover
+def generate_random_ip() -> str:  # pragma: no cover
     return '.'.join('%s' % random.randint(0, 255) for i in range(4))
 
 
-def generate_random_name(len=8):  # pragma: no cover
+def generate_random_name(length: int = 8) -> str:  # pragma: no cover
     return ''.join(
-        random.choices(string.ascii_uppercase + string.digits, k=len))
+        random.choices(string.ascii_uppercase + string.digits, k=length))
 
 
-def generate_random_port():  # pragma: no cover
-    return random.randint(0, 60000)
+def generate_random_port() -> Port:  # pragma: no cover
+    return Port(random.randint(0, 60000))
 
 
-def generate_custom_config(ip, ws_port):
+def generate_custom_config(ip: str, ws_port: Port) -> dict[str, str | Port]:
     if not ip or not ws_port:
         raise ValueError(
             f'For custom init you should provide ip and ws_port: {ip}, {ws_port}'
         )
     return {
         'ip': ip,
         'ws_port': ws_port,
     }
 
 
-def add_0x_prefix(bytes_string):  # pragma: no cover
+def add_0x_prefix(bytes_string: str) -> str:  # pragma: no cover
     return '0x' + bytes_string
 
 
-def rm_0x_prefix(bytes_string):
+def rm_0x_prefix(bytes_string: str) -> str:
     if bytes_string.startswith('0x'):
         return bytes_string[2:]
     return bytes_string
 
 
-def init_default_logger():  # pragma: no cover
+def init_default_logger() -> None:  # pragma: no cover
     handlers = []
     formatter = Formatter(
         '%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 
     stream_handler = StreamHandler(sys.stderr)
     stream_handler.setFormatter(formatter)
     stream_handler.setLevel(logging.INFO)
     handlers.append(stream_handler)
 
     logging.basicConfig(level=logging.DEBUG, handlers=handlers)
 
 
-def chunk(in_string, num_chunks):  # pragma: no cover
+def chunk(in_string: str, num_chunks: int) -> Generator[str, None, None]:  # pragma: no cover
     chunk_size = len(in_string) // num_chunks
     if len(in_string) % num_chunks:
         chunk_size += 1
     iterator = iter(in_string)
     for _ in range(num_chunks):
         accumulator = []
         for _ in range(chunk_size):
             try:
                 accumulator.append(next(iterator))
             except StopIteration:
                 break
         yield ''.join(accumulator)
 
 
-def split_public_key(public_key: str) -> list:
+def split_public_key(public_key: str) -> list[bytes]:
     public_key = rm_0x_prefix(public_key)
     pk_parts = list(chunk(public_key, 2))
     return list(map(bytes.fromhex, pk_parts))
 
 
-def get_contracts_info(contracts_data):
+def get_contracts_info(
+        contracts_data: list[ContractInfo[SkaleType]]
+) -> dict[str, ContractInfo[SkaleType]]:
     contracts_info = {}
     for contract_info in contracts_data:
         contracts_info[contract_info.name] = contract_info
     return contracts_info
 
 
-def to_camel_case(snake_str):
+def to_camel_case(snake_str: str) -> str:
     components = snake_str.split('_')
     return components[0] + ''.join(x.title() for x in components[1:])
 
 
-def is_test_env():
+def is_test_env() -> bool:
     return "pytest" in sys.modules or ENV == 'test'
```

### Comparing `skale.py-7.dev11/skale/utils/random_names/generator.py` & `skale.py-7.dev12/skale/utils/random_names/generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,29 +18,29 @@
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
 import random
 from skale.utils.random_names.vocabulary import CONSTELLATIONS, STARS, \
     SOUND_AND_APPEARANCE_ADJECTIVES, POSITIVE_AND_TIME_ADJECTIVES
 
 
-def generate_random_node_name():
+def generate_random_node_name() -> str:
     return generate_name(CONSTELLATIONS, POSITIVE_AND_TIME_ADJECTIVES)
 
 
-def generate_random_schain_name():
+def generate_random_schain_name() -> str:
     return generate_name(STARS, SOUND_AND_APPEARANCE_ADJECTIVES)
 
 
-def generate_name(noun_dict, adjective_dict):
+def generate_name(noun_dict: list[str], adjective_dict: list[str]) -> str:
     noun = get_random_word_from_dict(noun_dict)
     adjective = get_random_word_from_dict(adjective_dict)
     return f'{adjective}-{noun}'
 
 
-def get_random_word_from_dict(vocabulary_dict):
+def get_random_word_from_dict(vocabulary_dict: list[str]) -> str:
     return random.choice(vocabulary_dict).lower().replace(" ", "-")
 
 
 if __name__ == "__main__":
     node_name = generate_random_node_name()
     schain_name = generate_random_schain_name()
     print(f'Node name: {node_name}, sChain name: {schain_name}')
```

### Comparing `skale.py-7.dev11/skale/utils/random_names/vocabulary.py` & `skale.py-7.dev12/skale/utils/random_names/vocabulary.py`

 * *Files identical despite different names*

### Comparing `skale.py-7.dev11/skale/utils/web3_utils.py` & `skale.py-7.dev12/skale/utils/web3_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,24 +17,34 @@
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 """ SKALE web3 utilities """
 
 import logging
 import os
 import time
-from typing import Iterable
+from typing import Any, Callable, Dict, Iterable
 from urllib.parse import urlparse
 
-from eth_keys import keys
+from eth_keys.main import lazy_key_api as keys
+from eth_typing import Address, AnyAddress, BlockNumber, ChecksumAddress, HexStr
 from web3 import Web3, WebsocketProvider, HTTPProvider
 from web3.exceptions import TransactionNotFound
-from web3.middleware import (
-    attrdict_middleware,
-    geth_poa_middleware,
-    http_retry_request_middleware
+from web3.middleware.attrdict import attrdict_middleware
+from web3.middleware.exception_retry_request import http_retry_request_middleware
+from web3.middleware.geth_poa import geth_poa_middleware
+from web3.providers.base import JSONBaseProvider
+from web3.types import (
+    _Hash32,
+    ENS,
+    Middleware,
+    Nonce,
+    RPCEndpoint,
+    RPCResponse,
+    Timestamp,
+    TxReceipt
 )
 
 import skale.config as config
 from skale.transactions.exceptions import TransactionFailedError
 from skale.utils.constants import GAS_PRICE_COEFFICIENT
 from skale.utils.helper import is_test_env
 from skale.transactions.exceptions import TransactionNotMinedError
@@ -46,23 +56,27 @@
 WS_MAX_MESSAGE_DATA_BYTES = 5 * 1024 * 1024
 MAX_WAITING_TIME = 3 * 60 * 60  # 3 hours
 BLOCK_WAITING_TIMEOUT = 1
 DEFAULT_HTTP_TIMEOUT = 120
 DEFAULT_BLOCKS_TO_WAIT = 50
 
 
-def get_provider(endpoint, timeout=DEFAULT_HTTP_TIMEOUT, request_kwargs={}):
+def get_provider(
+        endpoint: str,
+        timeout: int = DEFAULT_HTTP_TIMEOUT,
+        request_kwargs: Dict[str, Any] | None = None
+) -> JSONBaseProvider:
     scheme = urlparse(endpoint).scheme
     if scheme == 'ws' or scheme == 'wss':
         kwargs = request_kwargs or {'max_size': WS_MAX_MESSAGE_DATA_BYTES}
         return WebsocketProvider(endpoint, websocket_timeout=timeout,
                                  websocket_kwargs=kwargs)
 
     if scheme == 'http' or scheme == 'https':
-        kwargs = {'timeout': timeout, **request_kwargs}
+        kwargs = {'timeout': timeout, **(request_kwargs or {})}
         return HTTPProvider(endpoint, request_kwargs=kwargs)
 
     raise Exception(
         'Wrong endpoint option.'
         'Supported endpoint schemes: http/https/ws/wss'
     )
 
@@ -83,29 +97,47 @@
 
 
 def save_last_known_block_number(state_path: str, block_number: int) -> None:
     with open(state_path, 'w') as last_block_file:
         last_block_file.write(str(block_number))
 
 
-def outdated_client_time_msg(method, current_time, latest_block_timestamp, allowed_ts_diff):
+def outdated_client_time_msg(
+        method: RPCEndpoint,
+        current_time: float,
+        latest_block_timestamp: Timestamp,
+        allowed_ts_diff: int
+) -> str:
     return f'{method} failed; \
 current_time: {current_time}, latest_block_timestamp: {latest_block_timestamp}, \
 allowed_ts_diff: {allowed_ts_diff}'
 
 
-def outdated_client_file_msg(method, latest_block_number, saved_number, state_path):
+def outdated_client_file_msg(
+        method: RPCEndpoint,
+        latest_block_number: BlockNumber,
+        saved_number: int,
+        state_path: str
+) -> str:
     return f'{method} failed: latest_block_number: {latest_block_number}, \
         saved_number: {saved_number}, state_path: {state_path}'
 
 
-def make_client_checking_middleware(allowed_ts_diff: int,
-                                    state_path: str = None):
-    def eth_client_checking_middleware(make_request, web3):
-        def middleware(method, params):
+def make_client_checking_middleware(
+        allowed_ts_diff: int,
+        state_path: str | None = None
+) -> Callable[
+    [Callable[[RPCEndpoint, Any], RPCResponse], Web3],
+    Callable[[RPCEndpoint, Any], RPCResponse]
+]:
+    def eth_client_checking_middleware(
+            make_request: Callable[[RPCEndpoint, Any], RPCResponse],
+            web3: Web3
+    ) -> Callable[[RPCEndpoint, Any], RPCResponse]:
+        def middleware(method: RPCEndpoint, params: Any) -> RPCResponse:
             if method in ('eth_block_number', 'eth_getBlockByNumber'):
                 response = make_request(method, params)
             else:
                 latest_block = web3.eth.get_block('latest')
                 current_time = time.time()
 
                 ts_diff = current_time - latest_block['timestamp']
@@ -135,55 +167,55 @@
             return response
         return middleware
     return eth_client_checking_middleware
 
 
 def init_web3(endpoint: str,
               provider_timeout: int = DEFAULT_HTTP_TIMEOUT,
-              middlewares: Iterable = None,
-              state_path: str = None, ts_diff: int = None):
+              middlewares: Iterable[Middleware] | None = None,
+              state_path: str | None = None, ts_diff: int | None = None) -> Web3:
     if not middlewares:
         ts_diff = ts_diff or config.ALLOWED_TS_DIFF
         state_path = state_path or config.LAST_BLOCK_FILE
         if not ts_diff == config.NO_SYNC_TS_DIFF:
             sync_middleware = make_client_checking_middleware(ts_diff, state_path)
-            middewares = (
+            middewares = [
                 http_retry_request_middleware,
                 sync_middleware,
                 attrdict_middleware
-            )
+            ]
         else:
-            middewares = (
+            middewares = [
                 http_retry_request_middleware,
                 attrdict_middleware
-            )
+            ]
 
     provider = get_provider(endpoint, timeout=provider_timeout)
     web3 = Web3(provider)
     # required for rinkeby
     web3.middleware_onion.inject(geth_poa_middleware, layer=0)
     for middleware in middewares:
         web3.middleware_onion.add(middleware)  # todo: may cause issues
     return web3
 
 
-def get_receipt(web3, tx):
+def get_receipt(web3: Web3, tx: _Hash32) -> TxReceipt:
     return web3.eth.get_transaction_receipt(tx)
 
 
-def get_eth_nonce(web3, address):
+def get_eth_nonce(web3: Web3, address: Address | ChecksumAddress | ENS) -> Nonce:
     return web3.eth.get_transaction_count(address)
 
 
 def wait_for_receipt_by_blocks(
-    web3,
-    tx,
-    blocks_to_wait=DEFAULT_BLOCKS_TO_WAIT,
-    timeout=MAX_WAITING_TIME
-):
+    web3: Web3,
+    tx: _Hash32,
+    blocks_to_wait: int = DEFAULT_BLOCKS_TO_WAIT,
+    timeout: int = MAX_WAITING_TIME
+) -> TxReceipt:
     blocks_to_wait = blocks_to_wait or DEFAULT_BLOCKS_TO_WAIT
     timeout = timeout or MAX_WAITING_TIME
     previous_block = web3.eth.block_number
     current_block = previous_block
     wait_start_time = time.time()
     while time.time() - wait_start_time < timeout and \
             current_block <= previous_block + blocks_to_wait:
@@ -192,83 +224,77 @@
         except TransactionNotFound:
             receipt = None
         if receipt is not None:
             return receipt
         current_block = web3.eth.block_number
         time.sleep(3)
     raise TransactionNotMinedError(
-        f'Transaction with hash: {tx} not found in {blocks_to_wait} blocks.'
+        f'Transaction with hash: {str(tx)} not found in {blocks_to_wait} blocks.'
     )
 
 
-def wait_receipt(web3, tx, retries=30, timeout=5):
+def wait_receipt(web3: Web3, tx: _Hash32, retries: int = 30, timeout: int = 5) -> TxReceipt:
     for _ in range(0, retries):
         try:
             receipt = get_receipt(web3, tx)
         except TransactionNotFound:
             receipt = None
         if receipt is not None:
             return receipt
         time.sleep(timeout)  # pragma: no cover
     raise TransactionNotMinedError(
-        f'Transaction with hash: {tx} not mined after {retries} retries.'
+        f'Transaction with hash: {str(tx)} not mined after {retries} retries.'
     )
 
 
-def check_receipt(receipt, raise_error=True):
+def check_receipt(receipt: TxReceipt, raise_error: bool = True) -> bool:
     if receipt['status'] != 1:  # pragma: no cover
         if raise_error:
             raise TransactionFailedError(
                 f'Transaction failed, see receipt {receipt}'
             )
         else:
             return False
     return True
 
 
 def wait_for_confirmation_blocks(
-    web3,
-    blocks_to_wait,
-    timeout=MAX_WAITING_TIME,
-    request_timeout=5
-):
+    web3: Web3,
+    blocks_to_wait: int,
+    timeout: int = MAX_WAITING_TIME,
+    request_timeout: int = 5
+) -> None:
     current_block = start_block = web3.eth.block_number
     logger.info(
         f'Current block number is {current_block}, '
         f'waiting for {blocks_to_wait} confimration blocks to be mined'
     )
     wait_start_time = time.time()
     while time.time() - wait_start_time < timeout and \
             current_block <= start_block + blocks_to_wait:
         current_block = web3.eth.block_number
         time.sleep(request_timeout)
 
 
-def private_key_to_public(pr):
+def private_key_to_public(pr: HexStr) -> HexStr:
     pr_bytes = Web3.to_bytes(hexstr=pr)
-    pk = keys.PrivateKey(pr_bytes)
-    return pk.public_key
+    prk = keys.PrivateKey(pr_bytes)
+    pk = prk.public_key
+    return HexStr(pk.to_hex())
 
 
-def public_key_to_address(pk):
+def public_key_to_address(pk: HexStr) -> HexStr:
     hash = Web3.keccak(hexstr=str(pk))
     return Web3.to_hex(hash[-20:])
 
 
-def private_key_to_address(pr):
+def private_key_to_address(pr: HexStr) -> HexStr:
     pk = private_key_to_public(pr)
     return public_key_to_address(pk)
 
 
-def to_checksum_address(address):
+def to_checksum_address(address: AnyAddress | str | bytes) -> ChecksumAddress:
     return Web3.to_checksum_address(address)
 
 
-def wallet_to_public_key(wallet):
-    if isinstance(wallet, dict):
-        return private_key_to_public(wallet['private_key'])
-    else:
-        return wallet['public_key']
-
-
 def default_gas_price(web3: Web3) -> int:
     return web3.eth.gas_price * GAS_PRICE_COEFFICIENT
```

### Comparing `skale.py-7.dev11/skale/wallets/common.py` & `skale.py-7.dev12/skale/wallets/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,20 +14,26 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
 from abc import ABC, abstractmethod
-from typing import Dict, Optional
+from typing import Optional
+
+from eth_account.datastructures import SignedMessage, SignedTransaction
+from eth_typing import ChecksumAddress, HexStr
+from web3 import Web3
+from web3.types import _Hash32, TxParams, TxReceipt
 
 from skale.transactions.exceptions import ChainIdError
+from skale.utils.web3_utils import DEFAULT_BLOCKS_TO_WAIT
 
 
-def ensure_chain_id(tx_dict, web3):
+def ensure_chain_id(tx_dict: TxParams, web3: Web3) -> None:
     if not tx_dict.get('chainId'):
         tx_dict['chainId'] = web3.eth.chain_id
     if not tx_dict.get('chainId'):
         raise ChainIdError('chainId must be in tx_dict (see EIP-155)')
 
 
 class MessageNotSignedError(Exception):
@@ -35,37 +41,37 @@
     Raised when signing message failed
     """
     pass
 
 
 class BaseWallet(ABC):
     @abstractmethod
-    def sign(self, tx):
+    def sign(self, tx_dict: TxParams) -> SignedTransaction:
         pass
 
     @abstractmethod
     def sign_and_send(
         self,
-        tx_dict: Dict,
-        multiplier: Optional[int] = None,
+        tx_dict: TxParams,
+        multiplier: Optional[float] = None,
         priority: Optional[int] = None,
         method: Optional[str] = None
-    ) -> str:
+    ) -> HexStr:
         pass
 
     @abstractmethod
-    def sign_hash(self, unsigned_hash: str) -> str:
+    def sign_hash(self, unsigned_hash: str) -> SignedMessage:
         pass
 
     @property
     @abstractmethod
-    def address(self) -> str:
+    def address(self) -> ChecksumAddress:
         pass
 
     @property
     @abstractmethod
     def public_key(self) -> str:
         pass
 
     @abstractmethod
-    def wait(self, tx: str, confirmation_blocks: int = None):
+    def wait(self, tx: _Hash32, confirmation_blocks: int = DEFAULT_BLOCKS_TO_WAIT) -> TxReceipt:
         pass
```

### Comparing `skale.py-7.dev11/skale/wallets/ledger_wallet.py` & `skale.py-7.dev12/skale/wallets/ledger_wallet.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,87 +15,97 @@
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
 import logging
 import struct
-from typing import Dict, Optional
+from typing import Generator, Tuple, cast
 
+from eth_typing import ChecksumAddress, HexStr
 from hexbytes import HexBytes
-from eth_account.datastructures import SignedTransaction
-from eth_account._utils.legacy_transactions import encode_transaction
-from eth_account._utils.legacy_transactions import \
-    serializable_unsigned_transaction_from_dict as tx_from_dict
+from eth_account.datastructures import SignedMessage, SignedTransaction
+from eth_account._utils.legacy_transactions import (
+    encode_transaction,
+    serializable_unsigned_transaction_from_dict as tx_from_dict,
+    Transaction,
+    UnsignedTransaction
+)
+from eth_account._utils.typed_transactions import TypedTransaction
 
 from eth_utils.crypto import keccak
 from rlp import encode
+from web3 import Web3
+from web3.contract.contract import ContractFunction
 from web3.exceptions import Web3Exception
+from web3.types import _Hash32, TxParams, TxReceipt
 
 import skale.config as config
 from skale.transactions.exceptions import TransactionNotSentError, TransactionNotSignedError
 from skale.utils.web3_utils import (
+    DEFAULT_BLOCKS_TO_WAIT,
+    MAX_WAITING_TIME,
     get_eth_nonce,
     public_key_to_address,
     to_checksum_address,
     wait_for_receipt_by_blocks
 )
 from skale.wallets.common import BaseWallet, ensure_chain_id
 
 logger = logging.getLogger(__name__)
 
 
 class LedgerCommunicationError(Exception):
     pass
 
 
-def encode_bip32_path(path):
+def encode_bip32_path(path: str) -> bytes:
     if len(path) == 0:
         return b''
     encoded_chunks = []
     for bip32_chunk in path.split('/'):
         chunk = bip32_chunk.split('\'')
         if len(chunk) == 1:
             encoded_chunk = struct.pack('>I', int(chunk[0]))
         else:
             encoded_chunk = struct.pack('>I', 0x80000000 | int(chunk[0]))
         encoded_chunks.append(encoded_chunk)
 
     return b''.join(encoded_chunks)
 
 
-def derivation_path_prefix(bin32_path):
+def derivation_path_prefix(bin32_path: str) -> bytes:
     encoded_path = encode_bip32_path(bin32_path)
     encoded_path_len_bytes = (len(encoded_path) // 4).to_bytes(1, 'big')
     return encoded_path_len_bytes + encoded_path
 
 
-def chunks(sequence, size):
+def chunks(sequence: bytes, size: int) -> Generator[bytes, None, None]:
     return (sequence[pos:pos + size] for pos in range(0, len(sequence), size))
 
 
-def get_derivation_path(address_index, legacy) -> str:
+def get_derivation_path(address_index: int, legacy: bool) -> str:
     if legacy:
         return get_legacy_derivation_path(address_index)
     return get_live_derivation_path(address_index)
 
 
-def get_live_derivation_path(address_index) -> str:
+def get_live_derivation_path(address_index: int) -> str:
     return f'44\'/60\'/{address_index}\'/0/0'
 
 
-def get_legacy_derivation_path(address_index) -> str:
+def get_legacy_derivation_path(address_index: int) -> str:
     return f'44\'/60\'/0\'/{address_index}'
 
 
 class LedgerWallet(BaseWallet):
     CHUNK_SIZE = 255
     CLA = b'\xe0'
 
-    def __init__(self, web3, address_index, legacy=False, debug=False):
+    def __init__(self, web3: Web3, address_index: int, legacy: bool = False, debug: bool = False):
         from ledgerblue.comm import getDongle
         from ledgerblue.commException import CommException
 
         self._address_index = address_index
         self._bip32_path = get_derivation_path(address_index, legacy)
         try:
             self.dongle = getDongle(debug)
@@ -104,136 +114,149 @@
                 self.get_address_with_public_key()
         except (OSError, CommException):
             raise LedgerCommunicationError(
                 'Error occured during the interaction with Ledger device'
             )
 
     @property
-    def address(self):
+    def address(self) -> ChecksumAddress:
         return self._address
 
     @property
-    def public_key(self):
+    def public_key(self) -> str:
         return self._public_key
 
     # todo: remove this method after making software wallet as class
-    def __getitem__(self, key):
+    def __getitem__(self, key: str) -> str:
         items = {'address': self.address, 'public_key': self.public_key}
         return items[key]
 
-    def make_payload(self, data=''):
-        encoded_data = encode(data)
+    def make_payload(self, data: str = '') -> bytes:
+        encoded_data = cast(bytes, encode(data))
         path_prefix = derivation_path_prefix(self._bip32_path)
         return path_prefix + encoded_data
 
     @classmethod
-    def parse_sign_result(cls, tx, exchange_result):
+    def parse_sign_result(
+            cls,
+            tx: TypedTransaction | Transaction | UnsignedTransaction,
+            exchange_result: bytearray | bytes
+    ) -> SignedTransaction:
         sign_v = exchange_result[0]
         sign_r = int((exchange_result[1:1 + 32]).hex(), 16)
         sign_s = int((exchange_result[1 + 32: 1 + 32 + 32]).hex(), 16)
         enctx = encode_transaction(tx, (sign_v, sign_r, sign_s))
         transaction_hash = keccak(enctx)
 
         return SignedTransaction(
             rawTransaction=HexBytes(enctx),
             hash=HexBytes(transaction_hash),
             v=sign_v,
             r=sign_r,
             s=sign_s
         )
 
-    def exchange_sign_payload_by_chunks(self, payload):
+    def exchange_sign_payload_by_chunks(self, payload: bytes) -> bytearray:
         INS = b'\x04'
         P1_FIRST = b'\x00'
         P1_SUBSEQUENT = b'\x80'
         P2 = b'\x00'
 
         p1 = P1_FIRST
         for chunk in chunks(payload, LedgerWallet.CHUNK_SIZE):
             chunk_size_bytes = len(chunk).to_bytes(1, 'big')
             apdu = b''.join([
                 LedgerWallet.CLA, INS, p1, P2, chunk_size_bytes, chunk
             ])
             exchange_result = self.dongle.exchange(apdu)
             p1 = P1_SUBSEQUENT
-        return exchange_result
+        return cast(bytearray, exchange_result)
 
-    def sign(self, tx_dict):
+    def sign(self, tx_dict: TxParams) -> SignedTransaction:
         ensure_chain_id(tx_dict, self._web3)
         if tx_dict.get('nonce') is None:
             tx_dict['nonce'] = self._web3.eth.get_transaction_count(self.address)
 
         tx = tx_from_dict(tx_dict)
         try:
             payload = self.make_payload(tx)
             exchange_result = self.exchange_sign_payload_by_chunks(payload)
             return LedgerWallet.parse_sign_result(tx, exchange_result)
         except Exception as e:
             raise TransactionNotSignedError(e)
 
     def sign_and_send(
         self,
-        tx: Dict,
-        multiplier: int = config.DEFAULT_GAS_MULTIPLIER,
-        priority: int = config.DEFAULT_PRIORITY,
-        method: Optional[str] = None,
-        meta: Optional[Dict] = None
-    ) -> str:
+        tx: TxParams,
+        multiplier: float | None = config.DEFAULT_GAS_MULTIPLIER,
+        priority: int | None = config.DEFAULT_PRIORITY,
+        method: str | None = None
+    ) -> HexStr:
         signed_tx = self.sign(tx)
         try:
-            return self._web3.eth.send_raw_transaction(
+            return Web3.to_hex(self._web3.eth.send_raw_transaction(
                 signed_tx.rawTransaction
-            ).hex()
+            ))
         except (ValueError, Web3Exception) as e:
             raise TransactionNotSentError(e)
 
-    def sign_hash(self, unsigned_hash: str):
+    def sign_hash(self, unsigned_hash: str) -> SignedMessage:
         raise NotImplementedError(
             'sign_hash is not implemented for hardware wallet'
         )
 
     @classmethod
-    def parse_derive_result(cls, exchange_result):
+    def parse_derive_result(cls, exchange_result: bytearray) -> Tuple[ChecksumAddress, str]:
         pk_len = exchange_result[0]
-        pk = exchange_result[1: pk_len + 1].hex()[2:]
+        pk = HexStr(exchange_result[1: pk_len + 1].hex()[2:])
         address = public_key_to_address(pk)
         checksum_address = to_checksum_address(address)
         return checksum_address, pk
 
-    def exchange_derive_payload(self, payload):
+    def exchange_derive_payload(self, payload: bytes) -> bytearray:
         INS = b'\x02'
         P1 = b'\x00'
         P2 = b'\x00'
         payload_size_in_bytes = len(payload).to_bytes(1, 'big')
         apdu = b''.join([
             LedgerWallet.CLA, INS, P1, P2,
             payload_size_in_bytes, payload
         ])
-        return self.dongle.exchange(apdu)
+        return cast(bytearray, self.dongle.exchange(apdu))
 
-    def get_address_with_public_key(self):
+    def get_address_with_public_key(self) -> tuple[ChecksumAddress, str]:
         payload = self.make_payload()
         exchange_result = self.exchange_derive_payload(payload)
         return LedgerWallet.parse_derive_result(exchange_result)
 
-    def wait(self, tx_hash: str, blocks_to_wait=None, timeout=None):
+    def wait(
+            self,
+            tx_hash: _Hash32,
+            blocks_to_wait: int = DEFAULT_BLOCKS_TO_WAIT,
+            timeout: int = MAX_WAITING_TIME
+    ) -> TxReceipt:
         return wait_for_receipt_by_blocks(
             self._web3,
             tx_hash,
             blocks_to_wait=blocks_to_wait,
             timeout=timeout
         )
 
 
-def hardware_sign_and_send(web3, method, gas_amount, wallet) -> str:
-    address_from = wallet['address']
+def hardware_sign_and_send(
+        web3: Web3,
+        method: ContractFunction,
+        gas_amount: int,
+        wallet: LedgerWallet
+) -> str:
+    address_from = wallet.address
     eth_nonce = get_eth_nonce(web3, address_from)
     tx_dict = method.build_transaction({
         'gas': gas_amount,
         'nonce': eth_nonce
     })
     signed_txn = wallet.sign(tx_dict)
     tx = web3.eth.send_raw_transaction(signed_txn.rawTransaction).hex()
     logger.info(
-        f'{method.__class__.__name__} - transaction_hash: {web3.to_hex(tx)}'
+        f'{method.__class__.__name__} - transaction_hash: {tx}'
     )
     return tx
```

### Comparing `skale.py-7.dev11/skale/wallets/redis_wallet.py` & `skale.py-7.dev12/skale/wallets/redis_wallet.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,27 +19,32 @@
 
 import binascii
 import json
 import logging
 import os
 import time
 from enum import Enum
-from typing import Dict, Optional, Tuple
+from typing import Optional, Tuple, TypedDict
 
+from eth_account.datastructures import SignedMessage, SignedTransaction
+from eth_typing import ChecksumAddress, HexStr
 from redis import Redis
+from web3 import Web3
+from web3.types import _Hash32, TxParams, TxReceipt
 
 import skale.config as config
 from skale.transactions.exceptions import (
     TransactionError,
     TransactionNotMinedError,
     TransactionNotSentError,
     TransactionWaitError
 )
-from skale.utils.web3_utils import get_receipt, MAX_WAITING_TIME
+from skale.utils.web3_utils import DEFAULT_BLOCKS_TO_WAIT, get_receipt, MAX_WAITING_TIME
 from skale.wallets import BaseWallet
+from skale.wallets.web3_wallet import Web3Wallet
 
 logger = logging.getLogger(__name__)
 
 
 class RedisWalletError(Exception):
     pass
 
@@ -65,35 +70,44 @@
     SUCCESS = 'SUCCESS'
     FAILED = 'FAILED'
 
     def __str__(self) -> str:
         return str.__str__(self)
 
 
+TxRecord = TypedDict(
+    'TxRecord',
+    {
+        'status': TxRecordStatus,
+        'tx_hash': HexStr
+    },
+)
+
+
 class RedisWalletAdapter(BaseWallet):
     ID_SIZE = 16
 
     def __init__(
         self,
         rs: Redis,
         pool: str,
-        base_wallet: BaseWallet,
+        web3_wallet: Web3Wallet,
     ) -> None:
         self.rs = rs
         self.pool = pool
-        self.wallet = base_wallet
+        self.wallet = web3_wallet
 
-    def sign(self, tx: Dict) -> Dict:
+    def sign(self, tx: TxParams) -> SignedTransaction:
         return self.wallet.sign(tx)
 
-    def sign_hash(self, unsigned_hash: str) -> str:
+    def sign_hash(self, unsigned_hash: str) -> SignedMessage:
         return self.wallet.sign_hash(unsigned_hash)
 
     @property
-    def address(self) -> str:
+    def address(self) -> ChecksumAddress:
         return self.wallet.address
 
     @property
     def public_key(self) -> str:
         return self.wallet.public_key
 
     @classmethod
@@ -101,90 +115,96 @@
         prefix = b'tx-'
         unique = binascii.b2a_hex(os.urandom(cls.ID_SIZE // 2))
         return prefix + unique
 
     @classmethod
     def _make_score(cls, priority: int) -> int:
         ts = int(time.time())
-        return priority * 10 ** len(str(ts)) + ts
+        return priority * int(10 ** len(str(ts))) + ts
 
     @classmethod
     def _make_record(
         cls,
-        tx: Dict,
+        tx: TxParams,
         score: int,
-        multiplier: int = config.DEFAULT_GAS_MULTIPLIER,
-        method: Optional[str] = None,
-        meta: Optional[Dict] = None
+        multiplier: float = config.DEFAULT_GAS_MULTIPLIER,
+        method: Optional[str] = None
     ) -> Tuple[bytes, bytes]:
         tx_id = cls._make_raw_id()
         params = {
             'status': 'PROPOSED',
             'score': score,
             'multiplier': multiplier,
             'tx_hash': None,
             'method': method,
-            'meta': meta,
             **tx
         }
         # Ensure gas will be restimated in TM
         params['gas'] = None
         record = json.dumps(params).encode('utf-8')
         return tx_id, record
 
     @classmethod
-    def _to_raw_id(cls, tx_id: str) -> bytes:
-        return tx_id.encode('utf-8')
+    def _to_raw_id(cls, tx_id: _Hash32) -> bytes:
+        if isinstance(tx_id, str):
+            return Web3.to_bytes(hexstr=tx_id)
+        return Web3.to_bytes(tx_id)
 
-    def _to_id(cls, raw_id: str) -> str:
-        return raw_id.decode('utf-8')
+    @classmethod
+    def _to_id(cls, raw_id: bytes) -> HexStr:
+        return Web3.to_hex(raw_id)
 
     def sign_and_send(
         self,
-        tx: Dict,
+        tx: TxParams,
         multiplier: Optional[float] = None,
         priority: Optional[int] = None,
-        method: Optional[str] = None,
-        meta: Optional[Dict] = None
-    ) -> str:
+        method: Optional[str] = None
+    ) -> HexStr:
         priority = priority or config.DEFAULT_PRIORITY
         try:
             logger.info('Sending %s to redis pool, method: %s', tx, method)
             score = self._make_score(priority)
             raw_id, tx_record = self._make_record(
                 tx,
                 score,
-                multiplier=multiplier,
-                method=method,
-                meta=meta
+                multiplier=multiplier or config.DEFAULT_GAS_MULTIPLIER,
+                method=method
             )
             pipe = self.rs.pipeline()
             logger.info('Adding tx %s to the pool', raw_id)
             pipe.zadd(self.pool, {raw_id: score})
             logger.info('Saving tx %s record: %s', raw_id, tx_record)
             pipe.set(raw_id, tx_record, ex=config.TXRECORD_EXPIRATION)
             pipe.execute()
             return self._to_id(raw_id)
         except Exception as err:
             logger.exception(f'Sending {tx} with redis wallet errored')
             raise RedisWalletNotSentError(err)
 
-    def get_status(self, tx_id: str) -> str:
+    def get_status(self, tx_id: _Hash32) -> str:
         return self.get_record(tx_id)['status']
 
-    def get_record(self, tx_id: str) -> Dict:
+    def get_record(self, tx_id: _Hash32) -> TxRecord:
         rid = self._to_raw_id(tx_id)
-        return json.loads(self.rs.get(rid).decode('utf-8'))
+        response = self.rs.get(rid)
+        if isinstance(response, bytes):
+            parsed_json = json.loads(response.decode('utf-8'))
+            return TxRecord({
+                'status': parsed_json['status'],
+                'tx_hash': parsed_json['tx_hash']
+            })
+        raise ValueError('Unknown value was returned from get() call', response)
 
     def wait(
         self,
-        tx_id: str,
-        blocks_to_wait: Optional[int] = None,
+        tx_id: _Hash32,
+        blocks_to_wait: int = DEFAULT_BLOCKS_TO_WAIT,
         timeout: int = MAX_WAITING_TIME
-    ) -> Dict:
+    ) -> TxReceipt:
         start_ts = time.time()
         status, result = None, None
         while status not in [
             TxRecordStatus.DROPPED,
             TxRecordStatus.SUCCESS,
             TxRecordStatus.FAILED
         ] and time.time() - start_ts < timeout:
```

### Comparing `skale.py-7.dev11/skale/wallets/sgx_wallet.py` & `skale.py-7.dev12/skale/wallets/sgx_wallet.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,102 +14,123 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
 import logging
-from typing import Dict, Optional
+from typing import Tuple, cast
 
+from eth_account.datastructures import SignedMessage, SignedTransaction
+from eth_typing import ChecksumAddress, HexStr
 from sgx import SgxClient
 from web3 import Web3
 from web3.exceptions import Web3Exception
+from web3.types import _Hash32, TxParams, TxReceipt
 
 import skale.config as config
 from skale.transactions.exceptions import TransactionNotSentError, TransactionNotSignedError
-from skale.utils.web3_utils import get_eth_nonce, wait_for_receipt_by_blocks
+from skale.utils.web3_utils import (
+    DEFAULT_BLOCKS_TO_WAIT,
+    MAX_WAITING_TIME,
+    get_eth_nonce,
+    wait_for_receipt_by_blocks
+)
 from skale.wallets.common import BaseWallet, ensure_chain_id, MessageNotSignedError
 
 
 logger = logging.getLogger(__name__)
 
 
 class SgxWallet(BaseWallet):
-    def __init__(self, sgx_endpoint, web3, key_name=None, path_to_cert=None):
+    def __init__(
+            self,
+            sgx_endpoint: str,
+            web3: Web3,
+            key_name: str | None = None,
+            path_to_cert: str | None = None
+    ):
         self.sgx_client = SgxClient(sgx_endpoint, path_to_cert=path_to_cert)
         self._web3 = web3
         if key_name is None:
             self._key_name, self._address, self._public_key = self._generate()
         else:
             self._key_name = key_name
             self._address, self._public_key = self._get_account(key_name)
 
-    def sign(self, tx_dict):
+    def sign(self, tx_dict: TxParams) -> SignedTransaction:
         if tx_dict.get('nonce') is None:
             tx_dict['nonce'] = get_eth_nonce(self._web3, self._address)
         ensure_chain_id(tx_dict, self._web3)
         try:
-            return self.sgx_client.sign(tx_dict, self.key_name)
+            return cast(SignedTransaction, self.sgx_client.sign(tx_dict, self.key_name))
         except Exception as e:
             raise TransactionNotSignedError(e)
 
     def sign_and_send(
         self,
-        tx_dict: Dict,
-        multiplier: int = config.DEFAULT_GAS_MULTIPLIER,
-        priority: int = config.DEFAULT_PRIORITY,
-        method: Optional[str] = None,
-        meta: Optional[Dict] = None
-    ) -> str:
+        tx_dict: TxParams,
+        multiplier: float | None = config.DEFAULT_GAS_MULTIPLIER,
+        priority: int | None = config.DEFAULT_PRIORITY,
+        method: str | None = None
+    ) -> HexStr:
         signed_tx = self.sign(tx_dict)
         try:
-            return self._web3.eth.send_raw_transaction(
+            return Web3.to_hex(self._web3.eth.send_raw_transaction(
                 signed_tx.rawTransaction
-            ).hex()
+            ))
         except (ValueError, Web3Exception) as e:
             raise TransactionNotSentError(e)
 
-    def sign_hash(self, unsigned_hash: str):
+    def sign_hash(self, unsigned_hash: str) -> SignedMessage:
         if unsigned_hash.startswith('0x'):
             unsigned_hash = unsigned_hash[2:]
 
         body = bytes.fromhex(unsigned_hash)
         header = b'\x19Ethereum Signed Message:\n32'
         normalized_hash = header + body
         hash_to_sign = Web3.keccak(hexstr='0x' + normalized_hash.hex())
         chain_id = None
         try:
-            return self.sgx_client.sign_hash(
-                hash_to_sign,
-                self._key_name,
-                chain_id
+            return cast(
+                SignedMessage,
+                self.sgx_client.sign_hash(
+                    hash_to_sign,
+                    self._key_name,
+                    chain_id
+                )
             )
         except Exception as e:
             raise MessageNotSignedError(e)
 
     @property
-    def address(self):
+    def address(self) -> ChecksumAddress:
         return self._address
 
     @property
-    def public_key(self):
+    def public_key(self) -> str:
         return self._public_key
 
     @property
-    def key_name(self):
+    def key_name(self) -> str:
         return self._key_name
 
-    def _generate(self):
+    def _generate(self) -> Tuple[str, ChecksumAddress, str]:
         key = self.sgx_client.generate_key()
-        return key.name, key.address, key.public_key
+        return key.name, Web3.to_checksum_address(key.address), key.public_key
 
-    def _get_account(self, key_name):
+    def _get_account(self, key_name: str) -> Tuple[ChecksumAddress, str]:
         account = self.sgx_client.get_account(key_name)
-        return account.address, account.public_key
+        return Web3.to_checksum_address(account.address), account.public_key
 
-    def wait(self, tx_hash: str, blocks_to_wait=None, timeout=None):
+    def wait(
+            self,
+            tx_hash: _Hash32,
+            blocks_to_wait: int = DEFAULT_BLOCKS_TO_WAIT,
+            timeout: int = MAX_WAITING_TIME
+    ) -> TxReceipt:
         return wait_for_receipt_by_blocks(
             self._web3,
             tx_hash,
             blocks_to_wait=blocks_to_wait,
             timeout=timeout
         )
```

### Comparing `skale.py-7.dev11/skale/wallets/web3_wallet.py` & `skale.py-7.dev12/skale/wallets/web3_wallet.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,109 +13,128 @@
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
-from typing import Dict, Optional
-from eth_keys import keys
+from typing import cast
+from eth_keys.main import lazy_key_api as keys
+from eth_keys.datatypes import PublicKey
 from web3 import Web3
+from web3.types import _Hash32, TxParams, TxReceipt
 from eth_account import messages
+from eth_account.datastructures import SignedMessage, SignedTransaction
+from eth_typing import AnyAddress, ChecksumAddress, HexStr
 from web3.exceptions import Web3Exception
 
 import skale.config as config
 from skale.transactions.exceptions import (
     TransactionNotSignedError,
     TransactionNotSentError
 )
-from skale.utils.web3_utils import get_eth_nonce, wait_for_receipt_by_blocks
+from skale.utils.web3_utils import (
+    DEFAULT_BLOCKS_TO_WAIT,
+    MAX_WAITING_TIME,
+    get_eth_nonce,
+    wait_for_receipt_by_blocks
+)
 from skale.wallets.common import BaseWallet, ensure_chain_id, MessageNotSignedError
 
 
-def private_key_to_public(pr):
+def private_key_to_public(pr: HexStr) -> PublicKey:
     pr_bytes = Web3.to_bytes(hexstr=pr)
     pk = keys.PrivateKey(pr_bytes)
     return pk.public_key
 
 
-def public_key_to_address(pk):
+def public_key_to_address(pk: PublicKey) -> ChecksumAddress:
     hash = Web3.keccak(hexstr=str(pk))
     return to_checksum_address(Web3.to_hex(hash[-20:]))
 
 
-def private_key_to_address(pr):
+def private_key_to_address(pr: HexStr) -> ChecksumAddress:
     pk = private_key_to_public(pr)
     return public_key_to_address(pk)
 
 
-def to_checksum_address(address):
+def to_checksum_address(address: AnyAddress | str | bytes) -> ChecksumAddress:
     return Web3.to_checksum_address(address)
 
 
-def generate_wallet(web3):
-    account = web3.eth.account.create()
-    private_key = account.key.hex()
-    return Web3Wallet(private_key, web3)
-
-
 class Web3Wallet(BaseWallet):
-    def __init__(self, private_key, web3):
+    def __init__(self, private_key: HexStr, web3: Web3):
         self._private_key = private_key
         self._public_key = private_key_to_public(self._private_key)
         self._address = public_key_to_address(self._public_key)
 
         self._web3 = web3
 
-    def sign(self, tx_dict):
+    def sign(self, tx_dict: TxParams) -> SignedTransaction:
         if not tx_dict.get('nonce'):
             tx_dict['nonce'] = get_eth_nonce(self._web3, self._address)
         ensure_chain_id(tx_dict, self._web3)
         try:
-            return self._web3.eth.account.sign_transaction(
-                tx_dict,
-                private_key=self._private_key
+            return cast(
+                SignedTransaction,
+                self._web3.eth.account.sign_transaction(
+                    tx_dict,
+                    private_key=self._private_key
+                )
             )
         except (TypeError, ValueError, Web3Exception) as e:
             raise TransactionNotSignedError(e)
 
-    def sign_hash(self, unsigned_hash: str):
+    def sign_hash(self, unsigned_hash: str) -> SignedMessage:
         try:
             unsigned_message = messages.encode_defunct(hexstr=unsigned_hash)
-            return self._web3.eth.account.sign_message(
-                unsigned_message,
-                private_key=self._private_key
+            return cast(
+                SignedMessage,
+                self._web3.eth.account.sign_message(
+                    unsigned_message,
+                    private_key=self._private_key
+                )
             )
         except (TypeError, ValueError, Web3Exception) as e:
             raise MessageNotSignedError(e)
 
     def sign_and_send(
         self,
-        tx_dict: Dict,
-        multiplier: int = config.DEFAULT_GAS_MULTIPLIER,
-        priority: int = config.DEFAULT_PRIORITY,
-        method: Optional[str] = None,
-        meta: Optional[Dict] = None
-    ) -> str:
+        tx_dict: TxParams,
+        multiplier: float | None = config.DEFAULT_GAS_MULTIPLIER,
+        priority: int | None = config.DEFAULT_PRIORITY,
+        method: str | None = None
+    ) -> HexStr:
         signed_tx = self.sign(tx_dict)
         try:
-            return self._web3.eth.send_raw_transaction(
+            return Web3.to_hex(self._web3.eth.send_raw_transaction(
                 signed_tx.rawTransaction
-            ).hex()
+            ))
         except (ValueError, Web3Exception) as e:
             raise TransactionNotSentError(e)
 
     @property
-    def address(self):
+    def address(self) -> ChecksumAddress:
         return self._address
 
     @property
-    def public_key(self):
+    def public_key(self) -> str:
         return str(self._public_key)
 
-    def wait(self, tx_hash: str, blocks_to_wait=None, timeout=None):
+    def wait(
+            self,
+            tx_hash: _Hash32,
+            blocks_to_wait: int = DEFAULT_BLOCKS_TO_WAIT,
+            timeout: int = MAX_WAITING_TIME
+    ) -> TxReceipt:
         return wait_for_receipt_by_blocks(
             self._web3,
             tx_hash,
             blocks_to_wait=blocks_to_wait,
             timeout=timeout
         )
+
+
+def generate_wallet(web3: Web3) -> Web3Wallet:
+    account = web3.eth.account.create()
+    private_key = account.key.hex()
+    return Web3Wallet(private_key, web3)
```

### Comparing `skale.py-7.dev11/skale.py.egg-info/PKG-INFO` & `skale.py-7.dev12/skale.py.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skale.py
-Version: 7.dev11
+Version: 7.dev12
 Summary: SKALE client tools
 Home-page: https://github.com/skalenetwork/skale.py
 Author: SKALE Labs
 Author-email: support@skalelabs.com
 Keywords: skale
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `skale.py-7.dev11/skale.py.egg-info/SOURCES.txt` & `skale.py-7.dev12/skale.py.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,24 +10,27 @@
 skale/skale_manager.py
 skale.py.egg-info/PKG-INFO
 skale.py.egg-info/SOURCES.txt
 skale.py.egg-info/dependency_links.txt
 skale.py.egg-info/requires.txt
 skale.py.egg-info/top_level.txt
 skale/contracts/__init__.py
+skale/contracts/allocator_contract.py
 skale/contracts/base_contract.py
-skale/contracts/contract_manager.py
+skale/contracts/ima_contract.py
+skale/contracts/skale_manager_contract.py
 skale/contracts/allocator/__init__.py
 skale/contracts/allocator/allocator.py
 skale/contracts/allocator/escrow.py
 skale/contracts/ima/__init__.py
 skale/contracts/ima/linker.py
 skale/contracts/manager/__init__.py
 skale/contracts/manager/bounty_v2.py
 skale/contracts/manager/constants_holder.py
+skale/contracts/manager/contract_manager.py
 skale/contracts/manager/dkg.py
 skale/contracts/manager/groups.py
 skale/contracts/manager/key_storage.py
 skale/contracts/manager/manager.py
 skale/contracts/manager/node_rotation.py
 skale/contracts/manager/nodes.py
 skale/contracts/manager/punisher.py
@@ -42,15 +45,14 @@
 skale/contracts/manager/delegation/distributor.py
 skale/contracts/manager/delegation/slashing_table.py
 skale/contracts/manager/delegation/token_state.py
 skale/contracts/manager/delegation/validator_service.py
 skale/contracts/manager/test/__init__.py
 skale/contracts/manager/test/time_helpers_with_debug.py
 skale/dataclasses/__init__.py
-skale/dataclasses/delegation_status.py
 skale/dataclasses/node_info.py
 skale/dataclasses/schain_options.py
 skale/dataclasses/skaled_ports.py
 skale/schain_config/__init__.py
 skale/schain_config/generator.py
 skale/schain_config/ports_allocation.py
 skale/schain_config/rotation_history.py
```

### Comparing `skale.py-7.dev11/tests/schain_config/generator_test.py` & `skale.py-7.dev12/tests/schain_config/generator_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def test_get_nodes_for_schain(skale, schain):
     schain_name = schain
     schain_nodes = get_nodes_for_schain(skale, schain_name)
     fields_with_id = nodes.FIELDS.copy()
     fields_with_id.append('id')
 
     assert len(schain_nodes) >= MIN_NODES_IN_SCHAIN
-    assert list(schain_nodes[0].keys()) == fields_with_id
+    assert set(schain_nodes[0].keys()) == set(fields_with_id)
 
 
 def test_get_schain_nodes_with_schains(skale, schain):
     schain_name = schain
     nodes_with_schains = get_schain_nodes_with_schains(skale, schain_name)
     assert isinstance(nodes_with_schains[0]['schains'], list)
-    assert isinstance(nodes_with_schains[0]['schains'][0]['mainnetOwner'], str)
+    assert isinstance(nodes_with_schains[0]['schains'][0].mainnetOwner, str)
```

### Comparing `skale.py-7.dev11/tests/schain_config/ports_allocation_test.py` & `skale.py-7.dev12/tests/schain_config/ports_allocation_test.py`

 * *Files identical despite different names*

