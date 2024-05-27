# Comparing `tmp/pantos_service_node-1.6.0-py3-none-any.whl.zip` & `tmp/pantos_service_node-1.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,103 +1,52 @@
-Zip file size: 128420 bytes, number of entries: 101
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 10:20 pantos/__init__.py
--rw-r--r--  2.0 unx     3251 b- defN 24-Apr-23 10:21 pantos/alembic.ini
--rw-r--r--  2.0 unx     7809 b- defN 24-Apr-23 10:21 pantos/bids.yml
--rw-r--r--  2.0 unx     5415 b- defN 24-Apr-23 10:21 pantos/service-node-config.env
--rw-r--r--  2.0 unx    14841 b- defN 24-Apr-23 10:21 pantos/service-node-config.yml
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 10:20 pantos/common/__init__.py
--rw-r--r--  2.0 unx     6041 b- defN 24-Apr-23 10:20 pantos/common/configuration.py
--rw-r--r--  2.0 unx     4739 b- defN 24-Apr-23 10:20 pantos/common/entities.py
--rw-r--r--  2.0 unx     3311 b- defN 24-Apr-23 10:20 pantos/common/exceptions.py
--rw-r--r--  2.0 unx     7012 b- defN 24-Apr-23 10:20 pantos/common/logging.py
--rw-r--r--  2.0 unx     2969 b- defN 24-Apr-23 10:20 pantos/common/restapi.py
--rw-r--r--  2.0 unx    12286 b- defN 24-Apr-23 10:20 pantos/common/servicenodes.py
--rw-r--r--  2.0 unx     5043 b- defN 24-Apr-23 10:20 pantos/common/signer.py
--rw-r--r--  2.0 unx      509 b- defN 24-Apr-23 10:20 pantos/common/types.py
--rw-r--r--  2.0 unx       55 b- defN 24-Apr-23 10:20 pantos/common/blockchains/__init__.py
--rw-r--r--  2.0 unx      974 b- defN 24-Apr-23 10:20 pantos/common/blockchains/avalanche.py
--rw-r--r--  2.0 unx    41291 b- defN 24-Apr-23 10:20 pantos/common/blockchains/base.py
--rw-r--r--  2.0 unx      969 b- defN 24-Apr-23 10:20 pantos/common/blockchains/bnbchain.py
--rw-r--r--  2.0 unx      922 b- defN 24-Apr-23 10:20 pantos/common/blockchains/celo.py
--rw-r--r--  2.0 unx      938 b- defN 24-Apr-23 10:20 pantos/common/blockchains/cronos.py
--rw-r--r--  2.0 unx     1695 b- defN 24-Apr-23 10:20 pantos/common/blockchains/enums.py
--rw-r--r--  2.0 unx    19287 b- defN 24-Apr-23 10:20 pantos/common/blockchains/ethereum.py
--rw-r--r--  2.0 unx     3642 b- defN 24-Apr-23 10:20 pantos/common/blockchains/factory.py
--rw-r--r--  2.0 unx      938 b- defN 24-Apr-23 10:20 pantos/common/blockchains/fantom.py
--rw-r--r--  2.0 unx      946 b- defN 24-Apr-23 10:20 pantos/common/blockchains/polygon.py
--rw-r--r--  2.0 unx     3596 b- defN 24-Apr-23 10:20 pantos/common/blockchains/solana.py
--rw-r--r--  2.0 unx     6505 b- defN 24-Apr-23 10:20 pantos/common/blockchains/tasks.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/__init__.py
--rw-r--r--  2.0 unx     7229 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/avalanche_pantos_forwarder.abi
--rw-r--r--  2.0 unx    42156 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/avalanche_pantos_hub.abi
--rw-r--r--  2.0 unx     4069 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/avalanche_pantos_token.abi
--rw-r--r--  2.0 unx     4840 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/avalanche_standard_token.abi
--rw-r--r--  2.0 unx     7229 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/bnb_chain_pantos_forwarder.abi
--rw-r--r--  2.0 unx    42156 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/bnb_chain_pantos_hub.abi
--rw-r--r--  2.0 unx     4069 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/bnb_chain_pantos_token.abi
--rw-r--r--  2.0 unx     4840 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/bnb_chain_standard_token.abi
--rw-r--r--  2.0 unx     7229 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/celo_pantos_forwarder.abi
--rw-r--r--  2.0 unx    42156 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/celo_pantos_hub.abi
--rw-r--r--  2.0 unx     4069 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/celo_pantos_token.abi
--rw-r--r--  2.0 unx     4840 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/celo_standard_token.abi
--rw-r--r--  2.0 unx     7229 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/cronos_pantos_forwarder.abi
--rw-r--r--  2.0 unx    42156 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/cronos_pantos_hub.abi
--rw-r--r--  2.0 unx     4069 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/cronos_pantos_token.abi
--rw-r--r--  2.0 unx     4840 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/cronos_standard_token.abi
--rw-r--r--  2.0 unx     7229 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/ethereum_pantos_forwarder.abi
--rw-r--r--  2.0 unx    42156 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/ethereum_pantos_hub.abi
--rw-r--r--  2.0 unx     4069 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/ethereum_pantos_token.abi
--rw-r--r--  2.0 unx     4840 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/ethereum_standard_token.abi
--rw-r--r--  2.0 unx     7229 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/fantom_pantos_forwarder.abi
--rw-r--r--  2.0 unx    42156 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/fantom_pantos_hub.abi
--rw-r--r--  2.0 unx     4069 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/fantom_pantos_token.abi
--rw-r--r--  2.0 unx     4840 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/fantom_standard_token.abi
--rw-r--r--  2.0 unx     7229 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/polygon_pantos_forwarder.abi
--rw-r--r--  2.0 unx    42156 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/polygon_pantos_hub.abi
--rw-r--r--  2.0 unx     4069 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/polygon_pantos_token.abi
--rw-r--r--  2.0 unx     4840 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/polygon_standard_token.abi
--rw-r--r--  2.0 unx       79 b- defN 24-Apr-23 10:20 pantos/servicenode/__init__.py
--rw-r--r--  2.0 unx      806 b- defN 24-Apr-23 10:20 pantos/servicenode/__main__.py
--rw-r--r--  2.0 unx     3257 b- defN 24-Apr-23 10:20 pantos/servicenode/application.py
--rw-r--r--  2.0 unx     2641 b- defN 24-Apr-23 10:20 pantos/servicenode/celery.py
--rw-r--r--  2.0 unx     9432 b- defN 24-Apr-23 10:20 pantos/servicenode/configuration.py
--rw-r--r--  2.0 unx      221 b- defN 24-Apr-23 10:20 pantos/servicenode/exceptions.py
--rw-r--r--  2.0 unx    13968 b- defN 24-Apr-23 10:20 pantos/servicenode/restapi.py
--rw-r--r--  2.0 unx      198 b- defN 24-Apr-23 10:20 pantos/servicenode/wsgi.py
--rw-r--r--  2.0 unx       53 b- defN 24-Apr-23 10:20 pantos/servicenode/blockchains/__init__.py
--rw-r--r--  2.0 unx      957 b- defN 24-Apr-23 10:20 pantos/servicenode/blockchains/avalanche.py
--rw-r--r--  2.0 unx    22379 b- defN 24-Apr-23 10:20 pantos/servicenode/blockchains/base.py
--rw-r--r--  2.0 unx      952 b- defN 24-Apr-23 10:20 pantos/servicenode/blockchains/bnbchain.py
--rw-r--r--  2.0 unx      905 b- defN 24-Apr-23 10:20 pantos/servicenode/blockchains/celo.py
--rw-r--r--  2.0 unx      921 b- defN 24-Apr-23 10:20 pantos/servicenode/blockchains/cronos.py
--rw-r--r--  2.0 unx    16807 b- defN 24-Apr-23 10:20 pantos/servicenode/blockchains/ethereum.py
--rw-r--r--  2.0 unx     1101 b- defN 24-Apr-23 10:20 pantos/servicenode/blockchains/factory.py
--rw-r--r--  2.0 unx      921 b- defN 24-Apr-23 10:20 pantos/servicenode/blockchains/fantom.py
--rw-r--r--  2.0 unx      929 b- defN 24-Apr-23 10:20 pantos/servicenode/blockchains/polygon.py
--rw-r--r--  2.0 unx     2846 b- defN 24-Apr-23 10:20 pantos/servicenode/blockchains/solana.py
--rw-r--r--  2.0 unx       40 b- defN 24-Apr-23 10:20 pantos/servicenode/business/__init__.py
--rw-r--r--  2.0 unx      341 b- defN 24-Apr-23 10:20 pantos/servicenode/business/base.py
--rw-r--r--  2.0 unx     3574 b- defN 24-Apr-23 10:20 pantos/servicenode/business/bids.py
--rw-r--r--  2.0 unx     3341 b- defN 24-Apr-23 10:20 pantos/servicenode/business/node.py
--rw-r--r--  2.0 unx     4446 b- defN 24-Apr-23 10:20 pantos/servicenode/business/plugins.py
--rw-r--r--  2.0 unx    37731 b- defN 24-Apr-23 10:20 pantos/servicenode/business/transfers.py
--rw-r--r--  2.0 unx     3477 b- defN 24-Apr-23 10:20 pantos/servicenode/database/__init__.py
--rw-r--r--  2.0 unx    20036 b- defN 24-Apr-23 10:20 pantos/servicenode/database/access.py
--rw-r--r--  2.0 unx     1166 b- defN 24-Apr-23 10:20 pantos/servicenode/database/enums.py
--rw-r--r--  2.0 unx     1234 b- defN 24-Apr-23 10:20 pantos/servicenode/database/exceptions.py
--rw-r--r--  2.0 unx    13701 b- defN 24-Apr-23 10:20 pantos/servicenode/database/models.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 10:20 pantos/servicenode/database/migrations/__init__.py
--rw-r--r--  2.0 unx     2080 b- defN 24-Apr-23 10:20 pantos/servicenode/database/migrations/env.py
--rw-r--r--  2.0 unx      817 b- defN 24-Apr-23 10:20 pantos/servicenode/database/migrations/versions/5e552e0ec844_remove_id_from_bids_table.py
--rw-r--r--  2.0 unx     1520 b- defN 24-Apr-23 10:20 pantos/servicenode/database/migrations/versions/85982c1f3b95_create_deferrable_constraint.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 10:20 pantos/servicenode/database/migrations/versions/__init__.py
--rw-r--r--  2.0 unx     4152 b- defN 24-Apr-23 10:20 pantos/servicenode/database/migrations/versions/bd913c5bfdfb_off_chain_bids.py
--rw-r--r--  2.0 unx     7067 b- defN 24-Apr-23 10:20 pantos/servicenode/database/migrations/versions/c4c46d14ca6a_initial_database_schema.py
--rw-r--r--  2.0 unx     1675 b- defN 24-Apr-23 10:20 pantos/servicenode/plugins/__init__.py
--rw-r--r--  2.0 unx     2476 b- defN 24-Apr-23 10:20 pantos/servicenode/plugins/base.py
--rw-r--r--  2.0 unx     3368 b- defN 24-Apr-23 10:20 pantos/servicenode/plugins/bids.py
--rw-r--r--  2.0 unx    35148 b- defN 24-Apr-23 10:21 pantos_service_node-1.6.0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx      856 b- defN 24-Apr-23 10:21 pantos_service_node-1.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-23 10:21 pantos_service_node-1.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-23 10:21 pantos_service_node-1.6.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    10159 b- defN 24-Apr-23 10:21 pantos_service_node-1.6.0.dist-info/RECORD
-101 files, 800919 bytes uncompressed, 111752 bytes compressed:  86.0%
+Zip file size: 72123 bytes, number of entries: 50
+-rw-r--r--  2.0 unx     3251 b- defN 80-Jan-01 00:00 pantos/alembic.ini
+-rw-r--r--  2.0 unx     7809 b- defN 80-Jan-01 00:00 pantos/bids.yml
+-rw-r--r--  2.0 unx     5587 b- defN 80-Jan-01 00:00 pantos/service-node-config.env
+-rw-r--r--  2.0 unx    15434 b- defN 80-Jan-01 00:00 pantos/service-node-config.yml
+-rw-r--r--  2.0 unx       79 b- defN 80-Jan-01 00:00 pantos/servicenode/__init__.py
+-rw-r--r--  2.0 unx      866 b- defN 80-Jan-01 00:00 pantos/servicenode/__main__.py
+-rw-r--r--  2.0 unx     3257 b- defN 80-Jan-01 00:00 pantos/servicenode/application.py
+-rw-r--r--  2.0 unx       53 b- defN 80-Jan-01 00:00 pantos/servicenode/blockchains/__init__.py
+-rw-r--r--  2.0 unx      959 b- defN 80-Jan-01 00:00 pantos/servicenode/blockchains/avalanche.py
+-rw-r--r--  2.0 unx    22433 b- defN 80-Jan-01 00:00 pantos/servicenode/blockchains/base.py
+-rw-r--r--  2.0 unx      954 b- defN 80-Jan-01 00:00 pantos/servicenode/blockchains/bnbchain.py
+-rw-r--r--  2.0 unx      907 b- defN 80-Jan-01 00:00 pantos/servicenode/blockchains/celo.py
+-rw-r--r--  2.0 unx      923 b- defN 80-Jan-01 00:00 pantos/servicenode/blockchains/cronos.py
+-rw-r--r--  2.0 unx    16877 b- defN 80-Jan-01 00:00 pantos/servicenode/blockchains/ethereum.py
+-rw-r--r--  2.0 unx     1295 b- defN 80-Jan-01 00:00 pantos/servicenode/blockchains/factory.py
+-rw-r--r--  2.0 unx      923 b- defN 80-Jan-01 00:00 pantos/servicenode/blockchains/fantom.py
+-rw-r--r--  2.0 unx      931 b- defN 80-Jan-01 00:00 pantos/servicenode/blockchains/polygon.py
+-rw-r--r--  2.0 unx     2848 b- defN 80-Jan-01 00:00 pantos/servicenode/blockchains/solana.py
+-rw-r--r--  2.0 unx       40 b- defN 80-Jan-01 00:00 pantos/servicenode/business/__init__.py
+-rw-r--r--  2.0 unx      341 b- defN 80-Jan-01 00:00 pantos/servicenode/business/base.py
+-rw-r--r--  2.0 unx     3576 b- defN 80-Jan-01 00:00 pantos/servicenode/business/bids.py
+-rw-r--r--  2.0 unx     3035 b- defN 80-Jan-01 00:00 pantos/servicenode/business/node.py
+-rw-r--r--  2.0 unx     4452 b- defN 80-Jan-01 00:00 pantos/servicenode/business/plugins.py
+-rw-r--r--  2.0 unx    38424 b- defN 80-Jan-01 00:00 pantos/servicenode/business/transfers.py
+-rw-r--r--  2.0 unx     3227 b- defN 80-Jan-01 00:00 pantos/servicenode/celery.py
+-rw-r--r--  2.0 unx     9542 b- defN 80-Jan-01 00:00 pantos/servicenode/configuration.py
+-rw-r--r--  2.0 unx     3493 b- defN 80-Jan-01 00:00 pantos/servicenode/database/__init__.py
+-rw-r--r--  2.0 unx    20295 b- defN 80-Jan-01 00:00 pantos/servicenode/database/access.py
+-rw-r--r--  2.0 unx     1166 b- defN 80-Jan-01 00:00 pantos/servicenode/database/enums.py
+-rw-r--r--  2.0 unx     1286 b- defN 80-Jan-01 00:00 pantos/servicenode/database/exceptions.py
+-rw-r--r--  2.0 unx     2322 b- defN 80-Jan-01 00:00 pantos/servicenode/database/migrations/README
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 pantos/servicenode/database/migrations/__init__.py
+-rw-r--r--  2.0 unx     2096 b- defN 80-Jan-01 00:00 pantos/servicenode/database/migrations/env.py
+-rw-r--r--  2.0 unx      510 b- defN 80-Jan-01 00:00 pantos/servicenode/database/migrations/script.py.mako
+-rw-r--r--  2.0 unx      853 b- defN 80-Jan-01 00:00 pantos/servicenode/database/migrations/versions/5e552e0ec844_remove_id_from_bids_table.py
+-rw-r--r--  2.0 unx     1560 b- defN 80-Jan-01 00:00 pantos/servicenode/database/migrations/versions/85982c1f3b95_create_deferrable_constraint.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 pantos/servicenode/database/migrations/versions/__init__.py
+-rw-r--r--  2.0 unx     4392 b- defN 80-Jan-01 00:00 pantos/servicenode/database/migrations/versions/bd913c5bfdfb_off_chain_bids.py
+-rw-r--r--  2.0 unx     7193 b- defN 80-Jan-01 00:00 pantos/servicenode/database/migrations/versions/c4c46d14ca6a_initial_database_schema.py
+-rw-r--r--  2.0 unx    13940 b- defN 80-Jan-01 00:00 pantos/servicenode/database/models.py
+-rw-r--r--  2.0 unx      221 b- defN 80-Jan-01 00:00 pantos/servicenode/exceptions.py
+-rw-r--r--  2.0 unx     1871 b- defN 80-Jan-01 00:00 pantos/servicenode/plugins/__init__.py
+-rw-r--r--  2.0 unx     2477 b- defN 80-Jan-01 00:00 pantos/servicenode/plugins/base.py
+-rw-r--r--  2.0 unx     3370 b- defN 80-Jan-01 00:00 pantos/servicenode/plugins/bids.py
+-rw-r--r--  2.0 unx    14323 b- defN 80-Jan-01 00:00 pantos/servicenode/restapi.py
+-rw-r--r--  2.0 unx      198 b- defN 80-Jan-01 00:00 pantos/servicenode/wsgi.py
+-rw-r--r--  2.0 unx    35148 b- defN 80-Jan-01 00:00 pantos_service_node-1.7.0.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     7206 b- defN 80-Jan-01 00:00 pantos_service_node-1.7.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 pantos_service_node-1.7.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     4850 b- defN 16-Jan-01 00:00 pantos_service_node-1.7.0.dist-info/RECORD
+50 files, 276881 bytes uncompressed, 64157 bytes compressed:  76.8%
```

## zipnote {}

```diff
@@ -1,199 +1,28 @@
-Filename: pantos/__init__.py
-Comment: 
-
 Filename: pantos/alembic.ini
 Comment: 
 
 Filename: pantos/bids.yml
 Comment: 
 
 Filename: pantos/service-node-config.env
 Comment: 
 
 Filename: pantos/service-node-config.yml
 Comment: 
 
-Filename: pantos/common/__init__.py
-Comment: 
-
-Filename: pantos/common/configuration.py
-Comment: 
-
-Filename: pantos/common/entities.py
-Comment: 
-
-Filename: pantos/common/exceptions.py
-Comment: 
-
-Filename: pantos/common/logging.py
-Comment: 
-
-Filename: pantos/common/restapi.py
-Comment: 
-
-Filename: pantos/common/servicenodes.py
-Comment: 
-
-Filename: pantos/common/signer.py
-Comment: 
-
-Filename: pantos/common/types.py
-Comment: 
-
-Filename: pantos/common/blockchains/__init__.py
-Comment: 
-
-Filename: pantos/common/blockchains/avalanche.py
-Comment: 
-
-Filename: pantos/common/blockchains/base.py
-Comment: 
-
-Filename: pantos/common/blockchains/bnbchain.py
-Comment: 
-
-Filename: pantos/common/blockchains/celo.py
-Comment: 
-
-Filename: pantos/common/blockchains/cronos.py
-Comment: 
-
-Filename: pantos/common/blockchains/enums.py
-Comment: 
-
-Filename: pantos/common/blockchains/ethereum.py
-Comment: 
-
-Filename: pantos/common/blockchains/factory.py
-Comment: 
-
-Filename: pantos/common/blockchains/fantom.py
-Comment: 
-
-Filename: pantos/common/blockchains/polygon.py
-Comment: 
-
-Filename: pantos/common/blockchains/solana.py
-Comment: 
-
-Filename: pantos/common/blockchains/tasks.py
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/__init__.py
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/avalanche_pantos_forwarder.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/avalanche_pantos_hub.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/avalanche_pantos_token.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/avalanche_standard_token.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/bnb_chain_pantos_forwarder.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/bnb_chain_pantos_hub.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/bnb_chain_pantos_token.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/bnb_chain_standard_token.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/celo_pantos_forwarder.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/celo_pantos_hub.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/celo_pantos_token.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/celo_standard_token.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/cronos_pantos_forwarder.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/cronos_pantos_hub.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/cronos_pantos_token.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/cronos_standard_token.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/ethereum_pantos_forwarder.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/ethereum_pantos_hub.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/ethereum_pantos_token.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/ethereum_standard_token.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/fantom_pantos_forwarder.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/fantom_pantos_hub.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/fantom_pantos_token.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/fantom_standard_token.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/polygon_pantos_forwarder.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/polygon_pantos_hub.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/polygon_pantos_token.abi
-Comment: 
-
-Filename: pantos/common/blockchains/contracts/polygon_standard_token.abi
-Comment: 
-
 Filename: pantos/servicenode/__init__.py
 Comment: 
 
 Filename: pantos/servicenode/__main__.py
 Comment: 
 
 Filename: pantos/servicenode/application.py
 Comment: 
 
-Filename: pantos/servicenode/celery.py
-Comment: 
-
-Filename: pantos/servicenode/configuration.py
-Comment: 
-
-Filename: pantos/servicenode/exceptions.py
-Comment: 
-
-Filename: pantos/servicenode/restapi.py
-Comment: 
-
-Filename: pantos/servicenode/wsgi.py
-Comment: 
-
 Filename: pantos/servicenode/blockchains/__init__.py
 Comment: 
 
 Filename: pantos/servicenode/blockchains/avalanche.py
 Comment: 
 
 Filename: pantos/servicenode/blockchains/base.py
@@ -237,35 +66,44 @@
 
 Filename: pantos/servicenode/business/plugins.py
 Comment: 
 
 Filename: pantos/servicenode/business/transfers.py
 Comment: 
 
+Filename: pantos/servicenode/celery.py
+Comment: 
+
+Filename: pantos/servicenode/configuration.py
+Comment: 
+
 Filename: pantos/servicenode/database/__init__.py
 Comment: 
 
 Filename: pantos/servicenode/database/access.py
 Comment: 
 
 Filename: pantos/servicenode/database/enums.py
 Comment: 
 
 Filename: pantos/servicenode/database/exceptions.py
 Comment: 
 
-Filename: pantos/servicenode/database/models.py
+Filename: pantos/servicenode/database/migrations/README
 Comment: 
 
 Filename: pantos/servicenode/database/migrations/__init__.py
 Comment: 
 
 Filename: pantos/servicenode/database/migrations/env.py
 Comment: 
 
+Filename: pantos/servicenode/database/migrations/script.py.mako
+Comment: 
+
 Filename: pantos/servicenode/database/migrations/versions/5e552e0ec844_remove_id_from_bids_table.py
 Comment: 
 
 Filename: pantos/servicenode/database/migrations/versions/85982c1f3b95_create_deferrable_constraint.py
 Comment: 
 
 Filename: pantos/servicenode/database/migrations/versions/__init__.py
@@ -273,32 +111,41 @@
 
 Filename: pantos/servicenode/database/migrations/versions/bd913c5bfdfb_off_chain_bids.py
 Comment: 
 
 Filename: pantos/servicenode/database/migrations/versions/c4c46d14ca6a_initial_database_schema.py
 Comment: 
 
+Filename: pantos/servicenode/database/models.py
+Comment: 
+
+Filename: pantos/servicenode/exceptions.py
+Comment: 
+
 Filename: pantos/servicenode/plugins/__init__.py
 Comment: 
 
 Filename: pantos/servicenode/plugins/base.py
 Comment: 
 
 Filename: pantos/servicenode/plugins/bids.py
 Comment: 
 
-Filename: pantos_service_node-1.6.0.dist-info/LICENSE.md
+Filename: pantos/servicenode/restapi.py
+Comment: 
+
+Filename: pantos/servicenode/wsgi.py
 Comment: 
 
-Filename: pantos_service_node-1.6.0.dist-info/METADATA
+Filename: pantos_service_node-1.7.0.dist-info/LICENSE.md
 Comment: 
 
-Filename: pantos_service_node-1.6.0.dist-info/WHEEL
+Filename: pantos_service_node-1.7.0.dist-info/METADATA
 Comment: 
 
-Filename: pantos_service_node-1.6.0.dist-info/top_level.txt
+Filename: pantos_service_node-1.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: pantos_service_node-1.6.0.dist-info/RECORD
+Filename: pantos_service_node-1.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pantos/service-node-config.env

```diff
@@ -47,14 +47,15 @@
 ##### Section: signer #####
 # SIGNER_PEM=
 SIGNER_PEM_PASSWORD='<fill me>'
 
 ##### Section: blockchains #####
 ##### Section: avalanche #####
 # AVALANCHE_ACTIVE=
+# AVALANCHE_REGISTERED=
 AVALANCHE_UNSTAKING_ADDRESS='<fill me>'
 # AVALANCHE_PRIVATE_KEY=
 AVALANCHE_PRIVATE_KEY_PASSWORD='<fill me>'
 # AVALANCHE_PROVIDER=
 # AVALANCHE_FALLBACK_PROVIDER=
 # AVALANCHE_AVERAGE_BLOCK_TIME=
 # AVALANCHE_PROVIDER_TIMEOUT=
@@ -66,14 +67,15 @@
 # AVALANCHE_MIN_ADAPTABLE_FEE_PER_GAS=
 # AVALANCHE_MAX_TOTAL_FEE_PER_GAS=
 # AVALANCHE_ADAPTABLE_FEE_INCREASE_FACTOR=
 # AVALANCHE_BLOCKS_UNTIL_RESUBMISSION=
 # AVALANCHE_STAKE=
 ##### Section: bnb_chain #####
 # BNB_ACTIVE=
+# BNB_REGISTERED=
 BNB_UNSTAKING_ADDRESS='<fill me>'
 # BNB_PRIVATE_KEY=
 BNB_PRIVATE_KEY_PASSWORD='<fill me>'
 # BNB_PROVIDER=
 # BNB_FALLBACK_PROVIDER=
 # BNB_AVERAGE_BLOCK_TIME=
 # BNB_PROVIDER_TIMEOUT=
@@ -85,14 +87,15 @@
 # BNB_MIN_ADAPTABLE_FEE_PER_GAS=
 # BNB_MAX_TOTAL_FEE_PER_GAS=
 # BNB_ADAPTABLE_FEE_INCREASE_FACTOR=
 # BNB_BLOCKS_UNTIL_RESUBMISSION=
 # BNB_STAKE=
 ##### Section: celo #####
 # CELO_ACTIVE=
+# CELO_REGISTERED=
 CELO_UNSTAKING_ADDRESS='<fill me>'
 # CELO_PRIVATE_KEY=
 CELO_PRIVATE_KEY_PASSWORD='<fill me>'
 # CELO_PROVIDER=
 # CELO_FALLBACK_PROVIDER=
 # CELO_AVERAGE_BLOCK_TIME=
 # CELO_PROVIDER_TIMEOUT=
@@ -104,14 +107,15 @@
 # CELO_MIN_ADAPTABLE_FEE_PER_GAS=
 # CELO_MAX_TOTAL_FEE_PER_GAS=
 # CELO_ADAPTABLE_FEE_INCREASE_FACTOR=
 # CELO_BLOCKS_UNTIL_RESUBMISSION=
 # CELO_STAKE=
 ##### Section: cronos #####
 # CRONOS_ACTIVE=
+# CRONOS_REGISTERED=
 CRONOS_UNSTAKING_ADDRESS='<fill me>'
 # CRONOS_PRIVATE_KEY=
 CRONOS_PRIVATE_KEY_PASSWORD='<fill me>'
 # CRONOS_PROVIDER=
 # CRONOS_FALLBACK_PROVIDER=
 # CRONOS_AVERAGE_BLOCK_TIME=
 # CRONOS_PROVIDER_TIMEOUT=
@@ -123,14 +127,15 @@
 # CRONOS_MIN_ADAPTABLE_FEE_PER_GAS=
 # CRONOS_MAX_TOTAL_FEE_PER_GAS=
 # CRONOS_ADAPTABLE_FEE_INCREASE_FACTOR=
 # CRONOS_BLOCKS_UNTIL_RESUBMISSION=
 # CRONOS_STAKE=
 ##### Section: ethereum #####
 # ETHEREUM_ACTIVE=
+# ETHEREUM_REGISTERED=
 ETHEREUM_UNSTAKING_ADDRESS='<fill me>'
 # ETHEREUM_PRIVATE_KEY=
 ETHEREUM_PRIVATE_KEY_PASSWORD='<fill me>'
 # ETHEREUM_PROVIDER=
 # ETHEREUM_FALLBACK_PROVIDER=
 # ETHEREUM_AVERAGE_BLOCK_TIME=
 # ETHEREUM_PROVIDER_TIMEOUT=
@@ -142,14 +147,15 @@
 # ETHEREUM_MIN_ADAPTABLE_FEE_PER_GAS=
 # ETHEREUM_MAX_TOTAL_FEE_PER_GAS=
 # ETHEREUM_ADAPTABLE_FEE_INCREASE_FACTOR=
 # ETHEREUM_BLOCKS_UNTIL_RESUBMISSION=
 # ETHEREUM_STAKE=
 ##### Section: fantom #####
 # FANTOM_ACTIVE=
+# FANTOM_REGISTERED=
 FANTOM_UNSTAKING_ADDRESS='<fill me>'
 # FANTOM_PRIVATE_KEY=
 FANTOM_PRIVATE_KEY_PASSWORD='<fill me>'
 # FANTOM_PROVIDER=
 # FANTOM_FALLBACK_PROVIDER=
 # FANTOM_AVERAGE_BLOCK_TIME=
 # FANTOM_PROVIDER_TIMEOUT=
@@ -160,15 +166,16 @@
 # FANTOM_CONFIRMATIONS=
 # FANTOM_MIN_ADAPTABLE_FEE_PER_GAS=
 # FANTOM_MAX_TOTAL_FEE_PER_GAS=
 # FANTOM_ADAPTABLE_FEE_INCREASE_FACTOR=
 # FANTOM_BLOCKS_UNTIL_RESUBMISSION=
 # FANTOM_STAKE=
 ##### Section: polygon #####
-# POLYGON_ACTIVE=
+POLYGON_ACTIVE=false
+# POLYGON_REGISTERED=
 POLYGON_UNSTAKING_ADDRESS='<fill me>'
 # POLYGON_PRIVATE_KEY=
 POLYGON_PRIVATE_KEY_PASSWORD='<fill me>'
 # POLYGON_PROVIDER=
 # POLYGON_FALLBACK_PROVIDER=
 # POLYGON_AVERAGE_BLOCK_TIME=
 # POLYGON_PROVIDER_TIMEOUT=
@@ -180,14 +187,15 @@
 # POLYGON_MIN_ADAPTABLE_FEE_PER_GAS=
 # POLYGON_MAX_TOTAL_FEE_PER_GAS=
 # POLYGON_ADAPTABLE_FEE_INCREASE_FACTOR=
 # POLYGON_BLOCKS_UNTIL_RESUBMISSION=
 # POLYGON_STAKE=
 ##### Section: solana #####
 # SOLANA_ACTIVE=
+# SOLANA_REGISTERED=
 # SOLANA_UNSTAKING_ADDRESS=
 # SOLANA_PRIVATE_KEY=
 # SOLANA_PRIVATE_KEY_PASSWORD=
 # SOLANA_PROVIDER=
 # SOLANA_AVERAGE_BLOCK_TIME=
 # SOLANA_CHAIN_ID=
 # SOLANA_HUB=
```

## pantos/service-node-config.yml

```diff
@@ -50,14 +50,15 @@
 signer:
     pem: !ENV ${SIGNER_PEM:/etc/pantos/service-node-signer.pem}
     pem_password: !ENV ${SIGNER_PEM_PASSWORD}
 
 blockchains:
     avalanche:
         active: !ENV tag:yaml.org,2002:bool ${AVALANCHE_ACTIVE:true}
+        registered: !ENV tag:yaml.org,2002:bool ${AVALANCHE_REGISTERED:true}
         unstaking_address: !ENV ${AVALANCHE_UNSTAKING_ADDRESS:0x726265A9e352F2e9f15F255957840992803cED7d}
         private_key: !ENV ${AVALANCHE_PRIVATE_KEY:/etc/pantos/service-node.keystore}
         private_key_password: !ENV ${AVALANCHE_PRIVATE_KEY_PASSWORD:<fill me>}
         provider: !ENV ${AVALANCHE_PROVIDER:https://api.avax-test.network/ext/bc/C/rpc}
         fallback_providers:
             - !ENV ${AVALANCHE_FALLBACK_PROVIDER:https://api.avax-test.network/ext/bc/C/rpc}
         average_block_time: !ENV tag:yaml.org,2002:int ${AVALANCHE_AVERAGE_BLOCK_TIME:3}
@@ -70,14 +71,15 @@
         min_adaptable_fee_per_gas: !ENV tag:yaml.org,2002:int ${AVALANCHE_MIN_ADAPTABLE_FEE_PER_GAS:1000000000}
         #max_total_fee_per_gas: !ENV tag:yaml.org,2002:int ${AVALANCHE_MAX_TOTAL_FEE_PER_GAS: }
         adaptable_fee_increase_factor: !ENV tag:yaml.org,2002:float ${AVALANCHE_ADAPTABLE_FEE_INCREASE_FACTOR:1.101}
         blocks_until_resubmission: !ENV tag:yaml.org,2002:int ${AVALANCHE_BLOCKS_UNTIL_RESUBMISSION:20}
         stake: !ENV tag:yaml.org,2002:int ${AVALANCHE_STAKE:10000000000000}
     bnb_chain:
         active: !ENV tag:yaml.org,2002:bool ${BNB_ACTIVE:true}
+        registered: !ENV tag:yaml.org,2002:bool ${BNB_REGISTERED:true}
         unstaking_address: !ENV ${BNB_UNSTAKING_ADDRESS:0x726265A9e352F2e9f15F255957840992803cED7d}
         private_key: !ENV ${BNB_PRIVATE_KEY:/etc/pantos/service-node.keystore}
         private_key_password: !ENV ${BNB_PRIVATE_KEY_PASSWORD:<fill me>}
         provider: !ENV ${BNB_PROVIDER:https://data-seed-prebsc-1-s1.binance.org:8545/}
         fallback_providers:
             - !ENV ${BNB_FALLBACK_PROVIDER:https://data-seed-prebsc-1-s1.binance.org:8545/}
         average_block_time: !ENV tag:yaml.org,2002:int ${BNB_AVERAGE_BLOCK_TIME:3}
@@ -90,14 +92,15 @@
         min_adaptable_fee_per_gas: !ENV tag:yaml.org,2002:int ${BNB_MIN_ADAPTABLE_FEE_PER_GAS:5000000000}
         #max_total_fee_per_gas: !ENV tag:yaml.org,2002:int ${BNB_MAX_TOTAL_FEE_PER_GAS: }
         adaptable_fee_increase_factor: !ENV tag:yaml.org,2002:float ${BNB_ADAPTABLE_FEE_INCREASE_FACTOR:1.101}
         blocks_until_resubmission: !ENV tag:yaml.org,2002:int ${BNB_BLOCKS_UNTIL_RESUBMISSION:20}
         stake: !ENV tag:yaml.org,2002:int ${BNB_STAKE:10000000000000}
     celo:
         active: !ENV tag:yaml.org,2002:bool ${CELO_ACTIVE:true}
+        registered: !ENV tag:yaml.org,2002:bool ${CELO_REGISTERED:true}
         unstaking_address: !ENV ${CELO_UNSTAKING_ADDRESS:0x726265A9e352F2e9f15F255957840992803cED7d}
         private_key: !ENV ${CELO_PRIVATE_KEY:/etc/pantos/service-node.keystore}
         private_key_password: !ENV ${CELO_PRIVATE_KEY_PASSWORD:<fill me>}
         provider: !ENV ${CELO_PROVIDER:https://alfajores-forno.celo-testnet.org}
         fallback_providers:
             - !ENV ${CELO_FALLBACK_PROVIDER:https://alfajores-forno.celo-testnet.org}
         average_block_time: !ENV tag:yaml.org,2002:int ${CELO_AVERAGE_BLOCK_TIME:5}
@@ -110,14 +113,15 @@
         min_adaptable_fee_per_gas: !ENV tag:yaml.org,2002:int ${CELO_MIN_ADAPTABLE_FEE_PER_GAS:1000000000}
         #max_total_fee_per_gas: !ENV tag:yaml.org,2002:int ${CELO_MAX_TOTAL_FEE_PER_GAS: }
         adaptable_fee_increase_factor: !ENV tag:yaml.org,2002:float ${CELO_ADAPTABLE_FEE_INCREASE_FACTOR:1.101}
         blocks_until_resubmission: !ENV tag:yaml.org,2002:int ${CELO_BLOCKS_UNTIL_RESUBMISSION:20}
         stake: !ENV tag:yaml.org,2002:int ${CELO_STAKE:10000000000000}
     cronos:
         active: !ENV tag:yaml.org,2002:bool ${CRONOS_ACTIVE:true}
+        registered: !ENV tag:yaml.org,2002:bool ${CRONOS_REGISTERED:true}
         unstaking_address: !ENV ${CRONOS_UNSTAKING_ADDRESS:0x726265A9e352F2e9f15F255957840992803cED7d}
         private_key: !ENV ${CRONOS_PRIVATE_KEY:/etc/pantos/service-node.keystore}
         private_key_password: !ENV ${CRONOS_PRIVATE_KEY_PASSWORD:<fill me>}
         provider: !ENV ${CRONOS_PROVIDER:https://evm-t3.cronos.org}
         fallback_providers:
             - !ENV ${CRONOS_FALLBACK_PROVIDER:https://cronos-testnet.crypto.org:8545/}
         average_block_time: !ENV tag:yaml.org,2002:int ${CRONOS_AVERAGE_BLOCK_TIME:5}
@@ -130,14 +134,15 @@
         min_adaptable_fee_per_gas: !ENV tag:yaml.org,2002:int ${CRONOS_MIN_ADAPTABLE_FEE_PER_GAS:1000000000}
         #max_total_fee_per_gas: !ENV tag:yaml.org,2002:int ${CRONOS_MAX_TOTAL_FEE_PER_GAS: }
         adaptable_fee_increase_factor: !ENV tag:yaml.org,2002:float ${CRONOS_ADAPTABLE_FEE_INCREASE_FACTOR:1.101}
         blocks_until_resubmission: !ENV tag:yaml.org,2002:int ${CRONOS_BLOCKS_UNTIL_RESUBMISSION:20}
         stake: !ENV tag:yaml.org,2002:int ${CRONOS_STAKE:10000000000000}
     ethereum:
         active: !ENV tag:yaml.org,2002:bool ${ETHEREUM_ACTIVE:true}
+        registered: !ENV tag:yaml.org,2002:bool ${ETHEREUM_REGISTERED:true}
         unstaking_address: !ENV ${ETHEREUM_UNSTAKING_ADDRESS:0x726265A9e352F2e9f15F255957840992803cED7d}
         private_key: !ENV ${ETHEREUM_PRIVATE_KEY:/etc/pantos/service-node.keystore}
         private_key_password: !ENV ${ETHEREUM_PRIVATE_KEY_PASSWORD:<fill me>}
         provider: !ENV ${ETHEREUM_PROVIDER:https://ethereum-holesky.publicnode.com}
         fallback_providers:
             - !ENV ${ETHEREUM_FALLBACK_PROVIDER:https://ethereum-holesky.publicnode.com}
         average_block_time: !ENV tag:yaml.org,2002:int ${ETHEREUM_AVERAGE_BLOCK_TIME:14}
@@ -150,14 +155,15 @@
         min_adaptable_fee_per_gas: !ENV tag:yaml.org,2002:int ${ETHEREUM_MIN_ADAPTABLE_FEE_PER_GAS:1000000000}
         #max_total_fee_per_gas: !ENV tag:yaml.org,2002:int ${ETHEREUM_MAX_TOTAL_FEE_PER_GAS: }
         adaptable_fee_increase_factor: !ENV tag:yaml.org,2002:float ${ETHEREUM_ADAPTABLE_FEE_INCREASE_FACTOR:1.101}
         blocks_until_resubmission: !ENV tag:yaml.org,2002:int ${ETHEREUM_BLOCKS_UNTIL_RESUBMISSION:20}
         stake: !ENV tag:yaml.org,2002:int ${ETHEREUM_STAKE:10000000000000}
     fantom:
         active: !ENV tag:yaml.org,2002:bool ${FANTOM_ACTIVE:true}
+        registered: !ENV tag:yaml.org,2002:bool ${FANTOM_REGISTERED:true}
         unstaking_address: !ENV ${FANTOM_UNSTAKING_ADDRESS:0x726265A9e352F2e9f15F255957840992803cED7d}
         private_key: !ENV ${FANTOM_PRIVATE_KEY:/etc/pantos/service-node.keystore}
         private_key_password: !ENV ${FANTOM_PRIVATE_KEY_PASSWORD:<fill me>}
         provider: !ENV ${FANTOM_PROVIDER:https://rpc.ankr.com/fantom_testnet}
         fallback_providers:
             - !ENV ${FANTOM_FALLBACK_PROVIDER:https://rpc.ankr.com/fantom_testnet}
         average_block_time: !ENV tag:yaml.org,2002:int ${FANTOM_AVERAGE_BLOCK_TIME:1}
@@ -170,14 +176,15 @@
         min_adaptable_fee_per_gas: !ENV tag:yaml.org,2002:int ${FANTOM_MIN_ADAPTABLE_FEE_PER_GAS:1000000000}
         #max_total_fee_per_gas: !ENV tag:yaml.org,2002:int ${FANTOM_MAX_TOTAL_FEE_PER_GAS: }
         adaptable_fee_increase_factor: !ENV tag:yaml.org,2002:float ${FANTOM_ADAPTABLE_FEE_INCREASE_FACTOR:1.101}
         blocks_until_resubmission: !ENV tag:yaml.org,2002:int ${FANTOM_BLOCKS_UNTIL_RESUBMISSION:20}
         stake: !ENV tag:yaml.org,2002:int ${FANTOM_STAKE:10000000000000}
     polygon:
         active: !ENV tag:yaml.org,2002:bool ${POLYGON_ACTIVE:true}
+        registered: !ENV tag:yaml.org,2002:bool ${POLYGON_REGISTERED:true}
         unstaking_address: !ENV ${POLYGON_UNSTAKING_ADDRESS:0x726265A9e352F2e9f15F255957840992803cED7d}
         private_key: !ENV ${POLYGON_PRIVATE_KEY:/etc/pantos/service-node.keystore}
         private_key_password: !ENV ${POLYGON_PRIVATE_KEY_PASSWORD:<fill me>}
         provider: !ENV ${POLYGON_PROVIDER:https://rpc.ankr.com/polygon_mumbai}
         fallback_providers:
             - !ENV ${POLYGON_FALLBACK_PROVIDER:https://rpc.ankr.com/polygon_mumbai}
         average_block_time: !ENV tag:yaml.org,2002:int ${POLYGON_AVERAGE_BLOCK_TIME:3}
@@ -190,14 +197,15 @@
         min_adaptable_fee_per_gas: !ENV tag:yaml.org,2002:int ${POLYGON_MIN_ADAPTABLE_FEE_PER_GAS:1000000000}
         #max_total_fee_per_gas: !ENV tag:yaml.org,2002:int ${POLYGON_MAX_TOTAL_FEE_PER_GAS: }
         adaptable_fee_increase_factor: !ENV tag:yaml.org,2002:float ${POLYGON_ADAPTABLE_FEE_INCREASE_FACTOR:1.101}
         blocks_until_resubmission: !ENV tag:yaml.org,2002:int ${POLYGON_BLOCKS_UNTIL_RESUBMISSION:20}
         stake: !ENV tag:yaml.org,2002:int ${POLYGON_STAKE:10000000000000}
     solana:
         active: !ENV tag:yaml.org,2002:bool ${SOLANA_ACTIVE:false}
+        registered: !ENV tag:yaml.org,2002:bool ${SOLANA_REGISTERED:true}
         unstaking_address: !ENV ${SOLANA_UNSTAKING_ADDRESS:0x726265A9e352F2e9f15F255957840992803cED7d:' '}
         private_key: !ENV ${SOLANA_PRIVATE_KEY:' '}
         private_key_password: !ENV ${SOLANA_PRIVATE_KEY_PASSWORD:<fill me>}
         provider: !ENV ${SOLANA_PROVIDER:<fill me>}
         fallback_providers:
             - !ENV ${SOLANA_FALLBACK_PROVIDER:<fill me>}
         average_block_time: !ENV tag:yaml.org,2002:int ${SOLANA_AVERAGE_BLOCK_TIME:1}
```

## pantos/servicenode/__main__.py

```diff
@@ -10,9 +10,12 @@
     host = config['application'].get('host')
     port = config['application'].get('port')
     ssl_certificate = config['application'].get('ssl_certificate')
     ssl_private_key = config['application'].get('ssl_private_key')
     ssl_context = (None if ssl_certificate is None or ssl_private_key is None
                    else (ssl_certificate, ssl_private_key))
     debug = config['application']['debug']
-    application.run(host=host, port=port, ssl_context=ssl_context, debug=debug,
+    application.run(host=host,
+                    port=port,
+                    ssl_context=ssl_context,
+                    debug=debug,
                     use_reloader=False)
```

## pantos/servicenode/application.py

 * *Ordering differences only*

```diff
@@ -2,18 +2,18 @@
 
 """
 import logging
 import pathlib
 import sys
 
 import flask
-
 from pantos.common.logging import LogFile
 from pantos.common.logging import LogFormat
 from pantos.common.logging import initialize_logger
+
 from pantos.servicenode.blockchains.factory import \
     initialize_blockchain_clients
 from pantos.servicenode.business.node import NodeInteractor
 from pantos.servicenode.configuration import config
 from pantos.servicenode.configuration import load_config
 from pantos.servicenode.database import \
     initialize_package as initialize_database_package
```

## pantos/servicenode/celery.py

```diff
@@ -2,42 +2,68 @@
 
 """
 import logging
 import pathlib
 import sys
 
 import celery  # type: ignore
-
 from pantos.common.logging import LogFile
 from pantos.common.logging import LogFormat
 from pantos.common.logging import initialize_logger
+
 from pantos.servicenode.application import initialize_application
 from pantos.servicenode.configuration import config
 from pantos.servicenode.plugins import initialize_plugins
 
+_TRANSFERS_QUEUE_NAME = 'transfers'
+_BIDS_QUEUE_NAME = 'bids'
+
 
 def is_celery_worker_process() -> bool:
     return (len(sys.argv) > 0 and sys.argv[0].endswith('celery')
             and 'worker' in sys.argv)
 
 
 if is_celery_worker_process():
     initialize_application(False)  # pragma: no cover
 
-celery_app = celery.Celery(
-    'pantos.servicenode', broker=config['celery']['broker'],
-    backend=config['celery']['backend'], include=[
-        'pantos.common.blockchains.tasks',
-        'pantos.servicenode.business.transfers',
-        'pantos.servicenode.business.plugins'
-    ])
+celery_app = celery.Celery('pantos.servicenode',
+                           broker=config['celery']['broker'],
+                           backend=config['celery']['backend'],
+                           include=[
+                               'pantos.common.blockchains.tasks',
+                               'pantos.servicenode.business.transfers',
+                               'pantos.servicenode.business.plugins'
+                           ])
 """Celery application instance."""
 
-if is_celery_worker_process():
-    initialize_plugins(start_worker=True)  # pragma: no cover
+# Additional Celery configuration
+celery_app.conf.update(
+    result_expires=None,
+    task_default_exchange='pantos.servicenode',
+    task_default_queue='transfers',
+    task_routes={
+        'pantos.servicenode.business.plugins.execute_bid_plugin': {
+            'queue': _BIDS_QUEUE_NAME
+        },
+        'pantos.servicenode.business.transfers.*': {
+            'queue': _TRANSFERS_QUEUE_NAME
+        },
+        'pantos.common.blockchains.tasks.*': {
+            'queue': _TRANSFERS_QUEUE_NAME
+        }
+    },
+    task_track_started=True,
+    worker_enable_remote_control=False)
+
+if is_celery_worker_process():  # pragma: no cover
+    # purge the bids queue at startup
+    with celery_app.connection_for_write() as connection:
+        connection.default_channel.queue_purge(_BIDS_QUEUE_NAME)
+    initialize_plugins(start_worker=True)
 
 
 @celery.signals.after_setup_task_logger.connect  # Celery task logger
 @celery.signals.after_setup_logger.connect  # Celery logger
 def setup_logger(logger: logging.Logger, *args, **kwargs):
     """Sent after the setup of every single task and Celery logger.
     Used to augment logging configuration.
@@ -59,16 +85,7 @@
         log_file = LogFile(file_path, max_bytes, backup_count)
     debug = config['application']['debug']
     try:
         initialize_logger(logger, log_format, standard_output, log_file, debug)
     except Exception:
         logger.critical('unable to initialize logging', exc_info=True)
         sys.exit(1)
-
-
-# Additional Celery configuration
-celery_app.conf.update(result_expires=None,
-                       task_default_exchange='pantos.servicenode',
-                       task_default_queue='pantos.servicenode',
-                       task_default_routing_key='pantos.servicenode',
-                       task_track_started=True,
-                       worker_enable_remote_control=False)
```

## pantos/servicenode/configuration.py

```diff
@@ -19,14 +19,18 @@
 _VALIDATION_SCHEMA_BLOCKCHAIN = {
     'type': 'dict',
     'schema': {
         'active': {
             'type': 'boolean',
             'default': True
         },
+        'registered': {
+            'type': 'boolean',
+            'default': True
+        },
         'unstaking_address': {
             'type': 'string',
             'required': True,
             'empty': False
         },
         'private_key': {
             'type': 'string',
@@ -283,16 +287,18 @@
                         'required': True
                     }
                 }
             }
         }
     },
     'blockchains': {
-        'type': 'dict',
-        'schema': dict(
+        'type':
+        'dict',
+        'schema':
+        dict(
             zip([b.name.lower() for b in Blockchain],
                 itertools.repeat(_VALIDATION_SCHEMA_BLOCKCHAIN)))
     }
 }
 """Schema for validating the configuration file."""
```

## pantos/servicenode/restapi.py

```diff
@@ -8,24 +8,24 @@
 
 import flask
 import flask_cors  # type: ignore
 import flask_restful  # type: ignore
 import flask_restful.reqparse  # type: ignore
 import marshmallow
 import marshmallow.validate
-
 from pantos.common.blockchains.enums import Blockchain
 from pantos.common.entities import ServiceNodeBid
 from pantos.common.restapi import Live
 from pantos.common.restapi import bad_request
 from pantos.common.restapi import conflict
 from pantos.common.restapi import internal_server_error
 from pantos.common.restapi import not_acceptable
 from pantos.common.restapi import ok_response
 from pantos.common.restapi import resource_not_found
+
 from pantos.servicenode.blockchains.factory import get_blockchain_client
 from pantos.servicenode.business.bids import BidInteractor
 from pantos.servicenode.business.transfers import SenderNonceNotUniqueError
 from pantos.servicenode.business.transfers import TransferInteractor
 from pantos.servicenode.business.transfers import \
     TransferInteractorBidNotAcceptedError
 from pantos.servicenode.business.transfers import \
@@ -52,18 +52,18 @@
     signature = marshmallow.fields.String(required=True)
 
 
 class _TransferSchema(marshmallow.Schema):
     """Validation schema for the transfer endpoint parameters.
 
     """
-
     source_blockchain_id = marshmallow.fields.Integer(required=True)
     destination_blockchain_id = marshmallow.fields.Integer(
-        required=True, validate=marshmallow.validate.OneOf(
+        required=True,
+        validate=marshmallow.validate.OneOf(
             [blockchain.value for blockchain in Blockchain]))
     sender_address = marshmallow.fields.String(required=True)
     recipient_address = marshmallow.fields.String(required=True)
     source_token_address = marshmallow.fields.String(required=True)
     destination_token_address = marshmallow.fields.String(required=True)
     valid_until = marshmallow.fields.Integer(required=True)
     amount = marshmallow.fields.Integer(required=True)
@@ -78,15 +78,18 @@
             blockchain.value for blockchain in Blockchain
         ]
         if blockchain_id not in supported_blockchains_ids:
             raise marshmallow.ValidationError(
                 message='This is not a supported blockchain. '
                 f'Must be one of: {supported_blockchains_ids}.',
                 field_name='source_blockchain_id')
-        elif not get_blockchain_config(Blockchain(blockchain_id))['active']:
+        blockchain_config = get_blockchain_config(Blockchain(blockchain_id))
+        active = blockchain_config['active']
+        registered = blockchain_config['registered']
+        if not active or not registered:
             raise marshmallow.ValidationError(
                 message='This is not an active blockchain.',
                 field_name='source_blockchain_id')
 
     @marshmallow.validates_schema
     def __validate_schema(self, data: typing.Dict[str, typing.Any],
                           **kwargs) -> None:
@@ -119,19 +122,21 @@
 
     def __check_valid_recipient_address(self,
                                         destination_blockchain: Blockchain,
                                         recipient_address: str) -> None:
         if not get_blockchain_client(
                 destination_blockchain).is_valid_recipient_address(
                     recipient_address):
-            _logger.warning(
-                'new transfer request: invalid recipient address', extra={
-                    'recipient_address': recipient_address,
-                    'destination_blockchain': destination_blockchain.name
-                })
+            _logger.warning('new transfer request: invalid recipient address',
+                            extra={
+                                'recipient_address':
+                                recipient_address,
+                                'destination_blockchain':
+                                destination_blockchain.name
+                            })
             raise marshmallow.ValidationError(
                 'recipient address must be a valid blockchain '
                 'address, different from the 0 address on '
                 f'{destination_blockchain.name}',
                 field_name='recipient_address')
 
     def __check_valid_source_token_address(self, source_blockchain: Blockchain,
@@ -196,25 +201,28 @@
 
 
 class _BidsSchema(marshmallow.Schema):
     """Validation schema for the bids endpoint parameters.
 
     """
     source_blockchain = marshmallow.fields.Integer(
-        required=True, validate=marshmallow.validate.OneOf(
+        required=True,
+        validate=marshmallow.validate.OneOf(
             [blockchain.value for blockchain in Blockchain]))
     destination_blockchain = marshmallow.fields.Integer(
-        required=True, validate=marshmallow.validate.OneOf(
+        required=True,
+        validate=marshmallow.validate.OneOf(
             [blockchain.value for blockchain in Blockchain]))
 
 
 class _Transfer(flask_restful.Resource):
     """RESTful resource for token transfer requests.
 
     """
+
     def post(self) -> flask.Response:
         try:
             time_received = time.time()
             arguments = flask_restful.request.json
             initiate_transfer_request = _TransferSchema().load(
                 arguments | {'time_received': time_received})
             _logger.info('new transfer request', extra=arguments)
@@ -236,14 +244,15 @@
         return ok_response({'task_id': str(task_id)})
 
 
 class _TransferStatus(flask_restful.Resource):
     """RESTful resource for token transfer status requests.
 
     """
+
     def get(self, task_id: str) -> flask.Response:
         try:
             task_id_uuid = _TransferStatusSchema().load({'task_id': task_id})
             _logger.info(f'new transfer status request: {task_id}')
             find_transfer_response = TransferInteractor().find_transfer(
                 task_id_uuid)
         except marshmallow.ValidationError:
@@ -255,40 +264,48 @@
                             f'"{task_id}"')
             resource_not_found(f'task ID {task_id} is unknown')
         except Exception:
             _logger.critical('unable to process a transfer status request',
                              exc_info=True)
             internal_server_error()
         return ok_response({
-            'task_id': str(task_id_uuid),
-            'source_blockchain_id': find_transfer_response.source_blockchain.
-            value,
-            'destination_blockchain_id': find_transfer_response.
-            destination_blockchain.value,
-            'sender_address': find_transfer_response.sender_address,
-            'recipient_address': find_transfer_response.recipient_address,
-            'source_token_address': find_transfer_response.
-            source_token_address,
-            'destination_token_address': find_transfer_response.
-            destination_token_address,
-            'amount': find_transfer_response.amount,
-            'fee': find_transfer_response.fee,
-            'status': find_transfer_response.status.to_public_status().name.
-            lower(),
-            'transfer_id': '' if find_transfer_response.transfer_id is None
-            else find_transfer_response.transfer_id,
-            'transaction_id': '' if find_transfer_response.transaction_id
-            is None else find_transfer_response.transaction_id
+            'task_id':
+            str(task_id_uuid),
+            'source_blockchain_id':
+            find_transfer_response.source_blockchain.value,
+            'destination_blockchain_id':
+            find_transfer_response.destination_blockchain.value,
+            'sender_address':
+            find_transfer_response.sender_address,
+            'recipient_address':
+            find_transfer_response.recipient_address,
+            'source_token_address':
+            find_transfer_response.source_token_address,
+            'destination_token_address':
+            find_transfer_response.destination_token_address,
+            'amount':
+            find_transfer_response.amount,
+            'fee':
+            find_transfer_response.fee,
+            'status':
+            find_transfer_response.status.to_public_status().name.lower(),
+            'transfer_id':
+            '' if find_transfer_response.transfer_id is None else
+            find_transfer_response.transfer_id,
+            'transaction_id':
+            '' if find_transfer_response.transaction_id is None else
+            find_transfer_response.transaction_id
         })
 
 
 class _Bids(flask_restful.Resource):
     """RESTful resource for token transfer bids.
 
     """
+
     def get(self) -> flask.Response:
         try:
             query_arguments = flask_restful.request.args
             bids_parameter = _BidsSchema().load(query_arguments)
             _logger.info('new bids request', extra=bids_parameter)
             bids = BidInteractor().get_cross_blockchain_bids(
                 bids_parameter['source_blockchain'],
```

## pantos/servicenode/blockchains/avalanche.py

```diff
@@ -1,13 +1,14 @@
 """Module for Avalanche-specific clients and errors. Since the
 Avalanche C-Chain is Ethereum-compatible, the client implementation
 inherits from the pantos.servicenode.blockchains.ethereum module.
 
 """
 from pantos.common.blockchains.enums import Blockchain
+
 from pantos.servicenode.blockchains.base import BlockchainClientError
 from pantos.servicenode.blockchains.ethereum import EthereumClient
 from pantos.servicenode.blockchains.ethereum import EthereumClientError
 
 
 class AvalancheClientError(EthereumClientError):
     """Exception class for all Avalanche client errors.
@@ -16,14 +17,15 @@
     pass
 
 
 class AvalancheClient(EthereumClient):
     """Avalanche-specific blockchain client.
 
     """
+
     @classmethod
     def get_blockchain(cls) -> Blockchain:
         # Docstring inherited
         return Blockchain.AVALANCHE
 
     @classmethod
     def get_error_class(cls) -> type[BlockchainClientError]:
```

## pantos/servicenode/blockchains/base.py

```diff
@@ -15,14 +15,15 @@
 from pantos.common.blockchains.enums import ContractAbi
 from pantos.common.blockchains.factory import get_blockchain_utilities
 from pantos.common.blockchains.factory import initialize_blockchain_utilities
 from pantos.common.entities import TransactionStatus
 from pantos.common.exceptions import ErrorCreator
 from pantos.common.types import BlockchainAddress
 from pantos.common.types import ContractFunctionArgs
+
 from pantos.servicenode.configuration import get_blockchain_config
 from pantos.servicenode.exceptions import ServiceNodeError
 
 _logger = logging.getLogger(__name__)
 
 
 class BlockchainClientError(ServiceNodeError):
@@ -33,45 +34,49 @@
 
 
 class InsufficientBalanceError(BlockchainClientError):
     """Exception class for all blockchain client errors caused by an
     insufficient balance.
 
     """
+
     def __init__(self, **kwargs: typing.Any):
         # Docstring inherited
         super().__init__('insufficient balance', **kwargs)
 
 
 class InvalidSignatureError(BlockchainClientError):
     """Exception class for all blockchain client errors caused by an
     invalid signature.
 
     """
+
     def __init__(self, **kwargs: typing.Any):
         # Docstring inherited
         super().__init__('invalid signature', **kwargs)
 
 
 class UnresolvableTransferSubmissionError(BlockchainClientError):
     """Exception to be raised if there has been an unresolvable error
     during a single-chain transfer or cross-chain transferFrom
     submission.
 
     """
+
     def __init__(self, **kwargs: typing.Any):
         # Docstring inherited
         super().__init__('unresolvable transfer/transferFrom submission error',
                          **kwargs)
 
 
 class BlockchainClient(BlockchainHandler, ErrorCreator[BlockchainClientError]):
     """Base class for all blockchain clients.
 
     """
+
     def __init__(self):
         """Construct a blockchain client instance.
 
         Raises
         ------
         BlockchainClientError
             If the corresponding blockchain utilities cannot be
@@ -86,16 +91,18 @@
             self._get_config()['confirmations']
         transaction_network_id = self._get_config().get('chain_id')
         private_key = self._get_config()['private_key']
         private_key_password = self._get_config()['private_key_password']
         try:
             initialize_blockchain_utilities(
                 self.get_blockchain(), [blockchain_node_url],
-                fallback_blockchain_nodes_urls, average_block_time,
-                required_transaction_confirmations, transaction_network_id,
+                fallback_blockchain_nodes_urls,
+                average_block_time,
+                required_transaction_confirmations,
+                transaction_network_id,
                 default_private_key=(private_key, private_key_password),
                 celery_tasks_enabled=True)
         except BlockchainUtilitiesError:
             raise self._create_error(
                 f'unable to initialize the {self.get_blockchain_name()} '
                 'utilities')
 
@@ -406,32 +413,32 @@
         try:
             status_response = \
                 self._get_utilities().get_transaction_submission_status(
                     internal_transaction_id)
         except BlockchainUtilitiesError:
             raise self._create_unresolvable_transfer_submission_error(
                 internal_transaction_id=internal_transaction_id)
-        _logger.info(
-            'transfer/transferFrom transaction submission status',
-            extra=vars(status_response)
-            | {'internal_transaction_id': internal_transaction_id})
+        _logger.info('transfer/transferFrom transaction submission status',
+                     extra=vars(status_response)
+                     | {'internal_transaction_id': internal_transaction_id})
         if not status_response.transaction_submission_completed:
             return BlockchainClient.TransferSubmissionStatusResponse(False)
         transaction_status = status_response.transaction_status
         assert transaction_status in [
             TransactionStatus.CONFIRMED, TransactionStatus.REVERTED
         ]
         transaction_id = status_response.transaction_id
         assert transaction_id is not None
         on_chain_transfer_id = (None if transaction_status
                                 is not TransactionStatus.CONFIRMED else
                                 self._read_on_chain_transfer_id(
                                     transaction_id, destination_blockchain))
         return BlockchainClient.TransferSubmissionStatusResponse(
-            True, transaction_status=transaction_status,
+            True,
+            transaction_status=transaction_status,
             transaction_id=transaction_id,
             on_chain_transfer_id=on_chain_transfer_id)
 
     @abc.abstractmethod
     def unregister_node(self) -> None:
         """Unregister the service node at the Pantos Hub on the
         blockchain.
```

## pantos/servicenode/blockchains/bnbchain.py

```diff
@@ -1,13 +1,14 @@
 """Module for BNB-Chain-specific clients and errors. Since the BNB
 Smart Chain is Ethereum-compatible, the client implementation inherits
 from the pantos.servicenode.blockchains.ethereum module.
 
 """
 from pantos.common.blockchains.enums import Blockchain
+
 from pantos.servicenode.blockchains.base import BlockchainClientError
 from pantos.servicenode.blockchains.ethereum import EthereumClient
 from pantos.servicenode.blockchains.ethereum import EthereumClientError
 
 
 class BnbChainClientError(EthereumClientError):
     """Exception class for all BNB Chain client errors.
@@ -16,14 +17,15 @@
     pass
 
 
 class BnbChainClient(EthereumClient):
     """BNB-Chain-specific blockchain client.
 
     """
+
     @classmethod
     def get_blockchain(cls) -> Blockchain:
         # Docstring inherited
         return Blockchain.BNB_CHAIN
 
     @classmethod
     def get_error_class(cls) -> type[BlockchainClientError]:
```

## pantos/servicenode/blockchains/celo.py

```diff
@@ -1,13 +1,14 @@
 """Module for Celo-specific clients and errors. Since Celo is
 Ethereum-compatible, the client implementation inherits from the
 pantos.servicenode.blockchains.ethereum module.
 
 """
 from pantos.common.blockchains.enums import Blockchain
+
 from pantos.servicenode.blockchains.base import BlockchainClientError
 from pantos.servicenode.blockchains.ethereum import EthereumClient
 from pantos.servicenode.blockchains.ethereum import EthereumClientError
 
 
 class CeloClientError(EthereumClientError):
     """Exception class for all Celo client errors.
@@ -16,14 +17,15 @@
     pass
 
 
 class CeloClient(EthereumClient):
     """Celo-specific blockchain client.
 
     """
+
     @classmethod
     def get_blockchain(cls) -> Blockchain:
         # Docstring inherited
         return Blockchain.CELO
 
     @classmethod
     def get_error_class(cls) -> type[BlockchainClientError]:
```

## pantos/servicenode/blockchains/cronos.py

```diff
@@ -1,13 +1,14 @@
 """Module for Cronos-specific clients and errors. Since Cronos is
 Ethereum-compatible, the client implementation inherits from the
 pantos.servicenode.blockchains.ethereum module.
 
 """
 from pantos.common.blockchains.enums import Blockchain
+
 from pantos.servicenode.blockchains.base import BlockchainClientError
 from pantos.servicenode.blockchains.ethereum import EthereumClient
 from pantos.servicenode.blockchains.ethereum import EthereumClientError
 
 
 class CronosClientError(EthereumClientError):
     """Exception class for all Cronos client errors.
@@ -16,14 +17,15 @@
     pass
 
 
 class CronosClient(EthereumClient):
     """Cronos-specific blockchain client.
 
     """
+
     @classmethod
     def get_blockchain(cls) -> Blockchain:
         # Docstring inherited
         return Blockchain.CRONOS
 
     @classmethod
     def get_error_class(cls) -> type[BlockchainClientError]:
```

## pantos/servicenode/blockchains/ethereum.py

```diff
@@ -6,22 +6,22 @@
 import time
 import typing
 import uuid
 
 import web3
 import web3.contract.contract
 import web3.exceptions
-
 from pantos.common.blockchains.base import NodeConnections
 from pantos.common.blockchains.base import TransactionNonceTooLowError
 from pantos.common.blockchains.base import TransactionUnderpricedError
 from pantos.common.blockchains.enums import Blockchain
 from pantos.common.blockchains.enums import ContractAbi
 from pantos.common.blockchains.ethereum import EthereumUtilities
 from pantos.common.types import BlockchainAddress
+
 from pantos.servicenode.blockchains.base import BlockchainClient
 from pantos.servicenode.blockchains.base import BlockchainClientError
 from pantos.servicenode.database import access as database_access
 
 _HUB_REGISTER_SERVICE_NODE_FUNCTION_SELECTOR = '0x901428b0'
 _HUB_REGISTER_SERVICE_NODE_GAS = 300000
 
@@ -58,14 +58,15 @@
     pass
 
 
 class EthereumClient(BlockchainClient):
     """Ethereum-specific blockchain client.
 
     """
+
     def __init__(self):
         # Docstring inherited
         super().__init__()
         private_key = self._get_config()['private_key']
         private_key_password = self._get_config()['private_key_password']
         private_key = self._get_utilities().decrypt_private_key(
             private_key, private_key_password)
@@ -154,15 +155,16 @@
                 _HUB_REGISTER_SERVICE_NODE_GAS, None, nonce)
             internal_transaction_id = self._start_transaction_submission(
                 request, node_connections)
             extra_info |= {'internal_transaction_id': internal_transaction_id}
             _logger.info('node registration submitted', extra=extra_info)
         except Exception:
             raise self._create_error('unable to register the service node',
-                                     node_url=node_url, node_stake=node_stake)
+                                     node_url=node_url,
+                                     node_stake=node_stake)
 
     def start_transfer_submission(
             self, request: BlockchainClient.TransferSubmissionStartRequest) \
             -> uuid.UUID:
         # Docstring inherited
         on_chain_request = (request.sender_address, request.recipient_address,
                             request.token_address, request.amount,
@@ -312,30 +314,32 @@
         try:
             node_connections = self.__create_node_connections()
             transaction_receipt = node_connections.eth.get_transaction_receipt(
                 typing.cast(web3.types.HexStr, transaction_id)).get()
             assert (
                 transaction_receipt['transactionHash'].hex() == transaction_id)
             _logger.info(
-                'transfer/transferFrom transaction receipt', extra=json.loads(
+                'transfer/transferFrom transaction receipt',
+                extra=json.loads(
                     web3.Web3.to_json(transaction_receipt)))  # type: ignore
             hub_contract = self._create_hub_contract(node_connections)
             if self.get_blockchain() is destination_blockchain:
                 event_log = hub_contract.events.Transfer().process_receipt(
                     transaction_receipt, errors=web3.logs.DISCARD)[0].get()
                 on_chain_transfer_id = event_log['args']['transferId']
             else:
                 event_log = hub_contract.events.TransferFrom().process_receipt(
                     transaction_receipt, errors=web3.logs.DISCARD)[0].get()
                 on_chain_transfer_id = event_log['args']['sourceTransferId']
             return on_chain_transfer_id
         except Exception:
             raise self._create_error(
                 'unable to read the Pantos transfer ID on the source '
-                'blockchain', transaction_id=transaction_id,
+                'blockchain',
+                transaction_id=transaction_id,
                 destination_blockchain=destination_blockchain)
 
     def __create_node_connections(self) -> NodeConnections:
         provider_timeout = self._get_config()['provider_timeout']
         return self._get_utilities().create_node_connections(provider_timeout)
 
     def __start_transfer_submission(self, internal_transfer_id: int,
```

## pantos/servicenode/blockchains/factory.py

```diff
@@ -1,30 +1,33 @@
 """Factory for blockchain clients.
 
 """
 import typing
 
 from pantos.common.blockchains.enums import Blockchain
+
 from pantos.servicenode.blockchains.base import BlockchainClient
+from pantos.servicenode.configuration import get_blockchain_config
 
 _blockchain_clients: typing.Dict[Blockchain, BlockchainClient] = {}
 """Blockchain-specific client objects."""
 
 _blockchain_client_classes = BlockchainClient.find_subclasses()
 """Blockchain-specific client classes."""
 
 
 def initialize_blockchain_clients() -> None:
-    """Initialize the blockchain-specific client objects for all
+    """Initialize the blockchain-specific client objects for all active
     blockchains.
 
     """
     for blockchain in Blockchain:
-        blockchain_client = _blockchain_client_classes[blockchain]()
-        _blockchain_clients[blockchain] = blockchain_client
+        if get_blockchain_config(blockchain)['active']:
+            blockchain_client = _blockchain_client_classes[blockchain]()
+            _blockchain_clients[blockchain] = blockchain_client
 
 
 def get_blockchain_client(blockchain: Blockchain) -> BlockchainClient:
     """Factory for blockchain-specific client objects.
 
     Parameters
     ----------
@@ -33,8 +36,9 @@
 
     Returns
     -------
     BlockchainClient
         A blockchain client instance for the specified blockchain.
 
     """
+    assert get_blockchain_config(blockchain)['active']
     return _blockchain_clients[blockchain]
```

## pantos/servicenode/blockchains/fantom.py

```diff
@@ -1,13 +1,14 @@
 """Module for Fantom-specific clients and errors. Since Fantom is
 Ethereum-compatible, the client implementation inherits from the
 pantos.servicenode.blockchains.ethereum module.
 
 """
 from pantos.common.blockchains.enums import Blockchain
+
 from pantos.servicenode.blockchains.base import BlockchainClientError
 from pantos.servicenode.blockchains.ethereum import EthereumClient
 from pantos.servicenode.blockchains.ethereum import EthereumClientError
 
 
 class FantomClientError(EthereumClientError):
     """Exception class for all Fantom client errors.
@@ -16,14 +17,15 @@
     pass
 
 
 class FantomClient(EthereumClient):
     """Fantom-specific blockchain client.
 
     """
+
     @classmethod
     def get_blockchain(cls) -> Blockchain:
         # Docstring inherited
         return Blockchain.FANTOM
 
     @classmethod
     def get_error_class(cls) -> type[BlockchainClientError]:
```

## pantos/servicenode/blockchains/polygon.py

```diff
@@ -1,13 +1,14 @@
 """Module for Polygon-specific clients and errors. Since Polygon is
 Ethereum-compatible, the client implementation inherits from the
 pantos.servicenode.blockchains.ethereum module.
 
 """
 from pantos.common.blockchains.enums import Blockchain
+
 from pantos.servicenode.blockchains.base import BlockchainClientError
 from pantos.servicenode.blockchains.ethereum import EthereumClient
 from pantos.servicenode.blockchains.ethereum import EthereumClientError
 
 
 class PolygonClientError(EthereumClientError):
     """Exception class for all Polygon client errors.
@@ -16,14 +17,15 @@
     pass
 
 
 class PolygonClient(EthereumClient):
     """Polygon-specific blockchain client.
 
     """
+
     @classmethod
     def get_blockchain(cls) -> Blockchain:
         # Docstring inherited
         return Blockchain.POLYGON
 
     @classmethod
     def get_error_class(cls) -> type[BlockchainClientError]:
```

## pantos/servicenode/blockchains/solana.py

```diff
@@ -1,14 +1,15 @@
 """Module for Solana-specific clients and errors.
 
 """
 import uuid
 
 from pantos.common.blockchains.enums import Blockchain
 from pantos.common.types import BlockchainAddress
+
 from pantos.servicenode.blockchains.base import BlockchainClient
 from pantos.servicenode.blockchains.base import BlockchainClientError
 
 
 class SolanaClientError(BlockchainClientError):
     """Exception class for all Solana client errors.
 
@@ -16,14 +17,15 @@
     pass
 
 
 class SolanaClient(BlockchainClient):
     """Solana-specific blockchain client.
 
     """
+
     def __init__(self):
         # Docstring inherited
         pass  # pragma: no cover
 
     @classmethod
     def get_blockchain(cls) -> Blockchain:
         # Docstring inherited
```

## pantos/servicenode/business/bids.py

```diff
@@ -3,14 +3,15 @@
 """
 import dataclasses
 import logging
 import typing
 
 from pantos.common.blockchains.enums import Blockchain
 from pantos.common.signer import get_signer
+
 from pantos.servicenode.business.base import Interactor
 from pantos.servicenode.business.base import InteractorError
 from pantos.servicenode.configuration import get_signer_config
 from pantos.servicenode.database import access as database_access
 
 _logger = logging.getLogger(__name__)
 """Logger for this module."""
@@ -23,14 +24,15 @@
     pass
 
 
 class BidInteractor(Interactor):
     """Interactor for managing service node bids.
 
     """
+
     @dataclasses.dataclass
     class Bid:
         """Data for a transfer bid.
 
         Attributes
         ----------
         execution_time : int
```

## pantos/servicenode/business/node.py

```diff
@@ -1,14 +1,14 @@
 """Business logic for managing the service node itself.
 
 """
 import logging
 
 from pantos.common.blockchains.enums import Blockchain
-from pantos.servicenode.blockchains.base import BlockchainClientError
+
 from pantos.servicenode.blockchains.factory import get_blockchain_client
 from pantos.servicenode.business.base import Interactor
 from pantos.servicenode.business.base import InteractorError
 from pantos.servicenode.configuration import config
 from pantos.servicenode.configuration import get_blockchain_config
 
 _logger = logging.getLogger(__name__)
@@ -22,14 +22,15 @@
     pass
 
 
 class NodeInteractor(Interactor):
     """Interactor for managing the service node itself.
 
     """
+
     def update_node_registrations(self) -> None:
         """Update the service node registrations on all supported
         blockchains.
 
         Raises
         ------
         NodeInteractorError
@@ -37,46 +38,39 @@
 
         """
         for blockchain in Blockchain:
             _logger.info('updating the service node registration on '
                          '{}'.format(blockchain.name))
             try:
                 blockchain_config = get_blockchain_config(blockchain)
-                active = blockchain_config['active']
-                try:
-                    blockchain_client = get_blockchain_client(blockchain)
-                    registered = blockchain_client.is_node_registered()
-                except BlockchainClientError:
-                    if active:
-                        raise
-                    else:
-                        # It is fine if we cannot interact with an
-                        # inactive blockchain (e.g. because of a
-                        # non-working blockchain node)
-                        continue
-                if active and registered:
+                if not blockchain_config['active']:
+                    continue
+                to_be_registered = blockchain_config['registered']
+                blockchain_client = get_blockchain_client(blockchain)
+                is_registered = blockchain_client.is_node_registered()
+                if to_be_registered and is_registered:
                     old_node_url = blockchain_client.read_node_url()
                     new_node_url = config['application']['url']
                     if old_node_url != new_node_url:
                         blockchain_client.update_node_url(new_node_url)
-                elif active:
+                elif to_be_registered:
                     is_unbonding = blockchain_client.is_unbonding()
                     if is_unbonding:
                         # Service node was unregistered but the stake
                         # has not been withdrawn yet
                         blockchain_client.cancel_unregistration()
                     else:
                         # Not yet registered
                         unstaking_address = blockchain_config[
                             'unstaking_address']
                         node_url = config['application']['url']
                         node_stake = blockchain_config['stake']
                         blockchain_client.register_node(
                             node_url, node_stake, unstaking_address)
-                elif registered:
-                    # Not active anymore
+                elif is_registered:
+                    # Not to be registered anymore
                     blockchain_client.unregister_node()
-                # Do nothing if not active and not registered
+                # Do nothing if neither registered nor to be registered
             except Exception:
                 raise NodeInteractorError(
                     'unable to update the service node registration on '
                     '{}'.format(blockchain.name))
```

## pantos/servicenode/business/plugins.py

```diff
@@ -1,16 +1,17 @@
 import collections.abc
 import dataclasses
 import logging
 
+import celery  # type: ignore
 from pantos.common.blockchains.enums import Blockchain
+
 from pantos.servicenode.blockchains.factory import get_blockchain_client
 from pantos.servicenode.business.base import Interactor
 from pantos.servicenode.business.base import InteractorError
-from pantos.servicenode.celery import celery_app as celery_app
 from pantos.servicenode.configuration import get_plugin_config
 from pantos.servicenode.database.access import replace_bids
 from pantos.servicenode.plugins import get_bid_plugin
 from pantos.servicenode.plugins.base import Bid
 from pantos.servicenode.plugins.base import BidPluginError
 
 _logger = logging.getLogger(__name__)
@@ -26,14 +27,15 @@
     pass
 
 
 class BidPluginInteractor(Interactor):
     """Interactor for handling the bid plugin operations.
 
     """
+
     def replace_bids(self, source_blockchain: Blockchain) -> int:
         """Replace the old bids with new bids given by the bid plugin.
         Additionally, the Validator fee is added to the bid fee.
 
         Returns
         -------
         int
@@ -93,27 +95,27 @@
         """
         total_factor = source_blockchain_factor + destination_blockchain_factor
         for bid in bids:
             bid.fee = round(
                 (bid.fee * total_factor) / source_blockchain_factor)
 
 
-@celery_app.task
+@celery.current_app.task
 def execute_bid_plugin(source_blockchain_id: int):
     """Celery task for executing the bid plugin.
 
     Parameters
     ----------
     source_blockchain_id : int
         The source blockchain for which the plugin is executed.
 
     """
+    source_blockchain = Blockchain(source_blockchain_id)
     bid_plugin_interactor = BidPluginInteractor()
     delay = _DEFAULT_DELAY
     try:
-        delay = bid_plugin_interactor.replace_bids(
-            Blockchain(source_blockchain_id))
+        delay = bid_plugin_interactor.replace_bids(source_blockchain)
     except Exception:
         _logger.critical('unable to replace the bids', exc_info=True)
     finally:
         execute_bid_plugin.apply_async(args=[source_blockchain_id],
                                        countdown=delay)
```

## pantos/servicenode/business/transfers.py

```diff
@@ -4,28 +4,29 @@
 import dataclasses
 import logging
 import math
 import time
 import typing
 import uuid
 
+import celery  # type: ignore
 from pantos.common.blockchains.enums import Blockchain
 from pantos.common.entities import ServiceNodeBid
 from pantos.common.entities import TransactionStatus
 from pantos.common.signer import get_signer
+
 from pantos.servicenode.blockchains.base import BlockchainClient
 from pantos.servicenode.blockchains.base import InsufficientBalanceError
 from pantos.servicenode.blockchains.base import InvalidSignatureError
 from pantos.servicenode.blockchains.base import \
     UnresolvableTransferSubmissionError
 from pantos.servicenode.blockchains.factory import get_blockchain_client
 from pantos.servicenode.business.base import Interactor
 from pantos.servicenode.business.base import InteractorError
 from pantos.servicenode.business.bids import BidInteractorError
-from pantos.servicenode.celery import celery_app
 from pantos.servicenode.configuration import config
 from pantos.servicenode.configuration import get_blockchain_config
 from pantos.servicenode.configuration import get_signer_config
 from pantos.servicenode.database import access as database_access
 from pantos.servicenode.database.enums import TransferStatus
 from pantos.servicenode.database.exceptions import SenderNonceNotUniqueError
 from pantos.servicenode.plugins import get_bid_plugin
@@ -64,14 +65,15 @@
     pass
 
 
 class TransferInteractor(Interactor):
     """Interactor for handling token transfers.
 
     """
+
     @dataclasses.dataclass
     class ConfirmTransferRequest:
         """Request data for confirming the inclusion of a token transfer
         on the source blockchain.
 
         Attributes
         ----------
@@ -120,15 +122,16 @@
                 request.source_blockchain)
             try:
                 status_response = \
                     source_blockchain_client.get_transfer_submission_status(
                         request.internal_transaction_id,
                         request.destination_blockchain)
             except UnresolvableTransferSubmissionError:
-                _logger.error('token transfer failed', extra=extra_info,
+                _logger.error('token transfer failed',
+                              extra=extra_info,
                               exc_info=True)
                 database_access.reset_transfer_nonce(
                     request.internal_transfer_id)
                 database_access.update_transfer_status(
                     request.internal_transfer_id, TransferStatus.FAILED)
                 return True
             if not status_response.transaction_submission_completed:
@@ -255,15 +258,16 @@
     def __single_chain_transfer(self,
                                 request: ExecuteTransferRequest) -> uuid.UUID:
         if request.source_token_address != request.destination_token_address:
             database_access.update_transfer_status(
                 request.internal_transfer_id, TransferStatus.FAILED)
             raise TransferInteractorUnrecoverableError(
                 'source and destination token addresses must be equal for '
-                'a single-chain token transfer', request=request)
+                'a single-chain token transfer',
+                request=request)
         transfer_request = BlockchainClient.TransferSubmissionStartRequest(
             request.internal_transfer_id, request.sender_address,
             request.recipient_address, request.source_token_address,
             request.amount, request.fee, request.sender_nonce,
             request.valid_until, request.signature)
         source_blockchain_client = get_blockchain_client(
             request.source_blockchain)
@@ -344,22 +348,25 @@
                 _logger.warning(
                     'new transfer request: invalid "valid until" timestamp '
                     f'{valid_until} for bid on '
                     f'{source_blockchain.name}')
                 raise TransferInteractorBidNotAcceptedError(
                     message='"valid until" timestamp must be at least '
                     'the current timestamp plus the service '
-                    'node bid\'s execution time', field_name='valid_until')
+                    'node bid\'s execution time',
+                    field_name='valid_until')
         except TransferInteractorBidNotAcceptedError:
             _logger.critical('unable to check the "valid until" timestamp',
                              exc_info=True)
             raise
 
     def __is_valid_execution_time_limit(
-            self, blockchain: Blockchain, execution_time_limit: int,
+            self,
+            blockchain: Blockchain,
+            execution_time_limit: int,
             bid_execution_time: int,
             start_time: typing.Optional[float] = None) -> bool:
         """Check if a given execution time limit matches the execution
         time specified by a service node bid. The execution time limit
         must be at least the start time plus the service node bid's
         execution time.
 
@@ -432,62 +439,66 @@
             If the given bid is not valid.
 
         """
         _logger.debug(
             'Checking if given bid is for source/destination blockchain')
         if (bid.source_blockchain != source_blockchain_id
                 or bid.destination_blockchain != destination_blockchain_id):
-            _logger.info(
-                'new transfer request: invalid bid', extra={
-                    'bid.fee': bid.fee,
-                    'bid.valid_until': bid.valid_until,
-                    'bid.execution_time': bid.execution_time,
-                    'bid.source_blockchain': bid.source_blockchain,
-                    'bid.destination_blockchain': bid.destination_blockchain,
-                    'source_blockchain_id': source_blockchain_id,
-                    'destination_blockchain_id': destination_blockchain_id,
-                    'bid.signature': bid.signature
-                })
+            _logger.info('new transfer request: invalid bid',
+                         extra={
+                             'bid.fee': bid.fee,
+                             'bid.valid_until': bid.valid_until,
+                             'bid.execution_time': bid.execution_time,
+                             'bid.source_blockchain': bid.source_blockchain,
+                             'bid.destination_blockchain':
+                             bid.destination_blockchain,
+                             'source_blockchain_id': source_blockchain_id,
+                             'destination_blockchain_id':
+                             destination_blockchain_id,
+                             'bid.signature': bid.signature
+                         })
             raise TransferInteractorBidNotAcceptedError(
                 message='bid not valid for blockchain pair',
                 field_name='bid.source_blockchain/bid.destination_blockchain')
         _logger.debug(
             'Bid is for correct blockchain pair. Checking if expired')
 
         bid_expired = self.__has_bid_expired(bid.valid_until)
 
         if bid_expired:
-            _logger.info(
-                'new transfer request: bid expired', extra={
-                    'bid.fee': bid.fee,
-                    'bid.valid_until': bid.valid_until,
-                    'bid.execution_time': bid.execution_time,
-                    'bid.source_blockchain': bid.source_blockchain,
-                    'bid.destination_blockchain': bid.destination_blockchain,
-                    'bid.signature': bid.signature
-                })
+            _logger.info('new transfer request: bid expired',
+                         extra={
+                             'bid.fee': bid.fee,
+                             'bid.valid_until': bid.valid_until,
+                             'bid.execution_time': bid.execution_time,
+                             'bid.source_blockchain': bid.source_blockchain,
+                             'bid.destination_blockchain':
+                             bid.destination_blockchain,
+                             'bid.signature': bid.signature
+                         })
             raise TransferInteractorBidNotAcceptedError(
                 message='bid has expired', field_name='bid.valid_until')
 
         _logger.info('Bid has not expired. Verifying bids signature')
         valid_bid = self.__verify_bids_signature(int(bid.fee), bid.valid_until,
                                                  bid.execution_time,
                                                  source_blockchain_id,
                                                  destination_blockchain_id,
                                                  bid.signature)
         if not valid_bid:
-            _logger.info(
-                'new transfer request: invalid bid', extra={
-                    'bid.fee': bid.fee,
-                    'bid.valid_until': bid.valid_until,
-                    'bid.execution_time': bid.execution_time,
-                    'source_blockchain_id': source_blockchain_id,
-                    'destination_blockchain_id': destination_blockchain_id,
-                    'bid.signature': bid.signature
-                })
+            _logger.info('new transfer request: invalid bid',
+                         extra={
+                             'bid.fee': bid.fee,
+                             'bid.valid_until': bid.valid_until,
+                             'bid.execution_time': bid.execution_time,
+                             'source_blockchain_id': source_blockchain_id,
+                             'destination_blockchain_id':
+                             destination_blockchain_id,
+                             'bid.signature': bid.signature
+                         })
             raise TransferInteractorBidNotAcceptedError(
                 message='bid\'s signature is invalid',
                 field_name='bid.signature')
         return valid_bid
 
     def __verify_bids_signature(self, fee: int, bid_valid_until: int,
                                 execution_time: int, source_blockchain_id: int,
@@ -718,14 +729,15 @@
             source_blockchain_config = get_blockchain_config(
                 request.source_blockchain)
             source_blockchain_client = get_blockchain_client(
                 request.source_blockchain)
             destination_blockchain_client = get_blockchain_client(
                 request.destination_blockchain)
             assert source_blockchain_config['active']
+            assert source_blockchain_config['registered']
             assert source_blockchain_client.is_valid_address(
                 request.sender_address)
             assert destination_blockchain_client.is_valid_address(
                 request.recipient_address)
             assert source_blockchain_client.is_valid_address(
                 request.source_token_address)
             assert destination_blockchain_client.is_valid_address(
@@ -770,15 +782,15 @@
         except TransferInteractorBidNotAcceptedError:
             raise
         except Exception:
             raise TransferInteractorError(
                 'unable to initiate a new token transfer', request=request)
 
 
-@celery_app.task(bind=True, max_retries=100)
+@celery.current_app.task(bind=True, max_retries=100)
 def confirm_transfer_task(self, internal_transfer_id: int,
                           source_blockchain_id: int,
                           destination_blockchain_id: int,
                           internal_transaction_id: str) -> bool:
     """Celery task for confirming the inclusion of a token transfer on
     the source blockchain.
 
@@ -809,25 +821,26 @@
         internal_transfer_id, source_blockchain, destination_blockchain,
         uuid.UUID(internal_transaction_id))
     try:
         confirmation_completed = TransferInteractor().confirm_transfer(
             confirm_transfer_request)
     except Exception as error:
         _logger.error('unable to confirm a token transfer',
-                      extra=vars(confirm_transfer_request), exc_info=True)
+                      extra=vars(confirm_transfer_request),
+                      exc_info=True)
         retry_interval = config['tasks']['confirm_transfer'][
             'retry_interval_after_error']
         raise self.retry(countdown=retry_interval, exc=error)
     if not confirmation_completed:
         retry_interval = config['tasks']['confirm_transfer']['interval']
         raise self.retry(countdown=retry_interval)
     return True
 
 
-@celery_app.task(bind=True, max_retries=None)
+@celery.current_app.task(bind=True, max_retries=None)
 def execute_transfer_task(self, internal_transfer_id: int,
                           source_blockchain_id: int,
                           destination_blockchain_id: int, sender_address: str,
                           recipient_address: str, source_token_address: str,
                           destination_token_address: str, amount: int,
                           fee: int, sender_nonce: int, valid_until: int,
                           signature: str) -> bool:
@@ -882,23 +895,26 @@
         destination_token_address, amount, fee, sender_nonce, valid_until,
         signature)
     try:
         internal_transaction_id = TransferInteractor().execute_transfer(
             execute_transfer_request)
         confirm_transfer_interval = config['tasks']['confirm_transfer'][
             'interval']
-        confirm_transfer_task.apply_async(
-            args=(internal_transfer_id, source_blockchain_id,
-                  destination_blockchain_id, str(internal_transaction_id)),
-            countdown=confirm_transfer_interval)
+        confirm_transfer_task.apply_async(args=(internal_transfer_id,
+                                                source_blockchain_id,
+                                                destination_blockchain_id,
+                                                str(internal_transaction_id)),
+                                          countdown=confirm_transfer_interval)
         return True
     except TransferInteractorUnrecoverableError as error:
         _logger.error(
             'unable to execute a token transfer - unrecoverable error',
-            extra=error.details, exc_info=True)
+            extra=error.details,
+            exc_info=True)
         return False
     except TransferInteractorError as error:
         _logger.error('unable to execute a token transfer - retrying',
-                      extra=error.details, exc_info=True)
+                      extra=error.details,
+                      exc_info=True)
         retry_interval = config['tasks']['execute_transfer'][
             'retry_interval_after_error']
         raise self.retry(countdown=retry_interval, exc=error)
```

## pantos/servicenode/database/__init__.py

```diff
@@ -5,16 +5,16 @@
 import typing
 
 import sqlalchemy  # type: ignore
 import sqlalchemy.exc  # type: ignore
 import sqlalchemy.orm  # type: ignore
 from alembic import command
 from alembic.config import Config
-
 from pantos.common.blockchains.enums import Blockchain
+
 from pantos.servicenode.configuration import config
 from pantos.servicenode.database.enums import TransferStatus
 from pantos.servicenode.database.exceptions import DatabaseError
 from pantos.servicenode.database.models import Blockchain as Blockchain_
 from pantos.servicenode.database.models import \
     TransferStatus as TransferStatus_
 
@@ -72,16 +72,18 @@
     # Before connecting, run alembic to ensure
     # the database schema is up to date
     if is_flask_app and config['database']['apply_migrations']:
         run_migrations(config['database']['alembic_config'],
                        config['database']['url'])
 
     sql_engine = sqlalchemy.create_engine(
-        config['database']['url'], pool_size=config['database']['pool_size'],
-        max_overflow=config['database']['max_overflow'], pool_pre_ping=True,
+        config['database']['url'],
+        pool_size=config['database']['pool_size'],
+        max_overflow=config['database']['max_overflow'],
+        pool_pre_ping=True,
         echo=config['database']['echo'])
     global _session_maker
     _session_maker = sqlalchemy.orm.sessionmaker(bind=sql_engine)
     # Initialize the tables
     with _session_maker.begin() as session:
         # Blockchain table
         max_blockchain_id = \
```

## pantos/servicenode/database/access.py

```diff
@@ -6,16 +6,16 @@
 import threading
 import typing
 import uuid
 
 import sqlalchemy  # type: ignore
 import sqlalchemy.exc  # type: ignore
 import sqlalchemy.orm  # type: ignore
-
 from pantos.common.blockchains.enums import Blockchain
+
 from pantos.servicenode.database import get_session
 from pantos.servicenode.database import get_session_maker
 from pantos.servicenode.database.enums import TransferStatus
 from pantos.servicenode.database.exceptions import DatabaseError
 from pantos.servicenode.database.exceptions import SenderNonceNotUniqueError
 from pantos.servicenode.database.models import UNIQUE_SENDER_NONCE_CONSTRAINT
 from pantos.servicenode.database.models import Base
@@ -53,15 +53,17 @@
 
     """
     assert execution_time > 0
     assert valid_until > 0
     assert fee > 0
     bid = Bid(source_blockchain_id=source_blockchain.value,
               destination_blockchain_id=destination_blockchain.value,
-              execution_time=execution_time, valid_until=valid_until, fee=fee)
+              execution_time=execution_time,
+              valid_until=valid_until,
+              fee=fee)
     with get_session_maker().begin() as session:
         session.add(bid)
         session.flush()
 
 
 def replace_bids(source_blockchain_id: int, destination_blockchain_id: int,
                  bids: typing.List[typing.Dict[typing.Any, typing.Any]]):
@@ -141,56 +143,63 @@
 
     """
     try:
         with get_session_maker().begin() as session:
             # Create the source and destination token contract instances if
             # they do not exist yet
             source_token_contract = _read_token_contract(
-                session, blockchain_id=source_blockchain.value,
+                session,
+                blockchain_id=source_blockchain.value,
                 address=source_token_address)
             source_token_contract_id = (
-                source_token_contract.id if source_token_contract is not None
-                else _create_token_contract(
-                    blockchain_id=source_blockchain.value,
-                    address=source_token_address))
+                source_token_contract.id
+                if source_token_contract is not None else
+                _create_token_contract(blockchain_id=source_blockchain.value,
+                                       address=source_token_address))
             destination_token_contract = _read_token_contract(
-                session, blockchain_id=destination_blockchain.value,
+                session,
+                blockchain_id=destination_blockchain.value,
                 address=destination_token_address)
             destination_token_contract_id = (
                 destination_token_contract.id if destination_token_contract
                 is not None else _create_token_contract(
                     blockchain_id=destination_blockchain.value,
                     address=destination_token_address))
             # Create the hub and forwarder contract instances if they do not
             # exist yet
             hub_contract = _read_hub_contract(
-                session, blockchain_id=source_blockchain.value,
+                session,
+                blockchain_id=source_blockchain.value,
                 address=hub_address)
             hub_contract_id = (hub_contract.id if hub_contract is not None else
                                _create_hub_contract(
                                    blockchain_id=source_blockchain.value,
                                    address=hub_address))
             forwarder_contract = _read_forwarder_contract(
-                session, blockchain_id=source_blockchain.value,
+                session,
+                blockchain_id=source_blockchain.value,
                 address=forwarder_address)
             forwarder_contract_id = (forwarder_contract.id
                                      if forwarder_contract is not None else
                                      _create_forwarder_contract(
                                          blockchain_id=source_blockchain.value,
                                          address=forwarder_address))
 
             transfer = Transfer(
                 source_blockchain_id=source_blockchain.value,
                 destination_blockchain_id=destination_blockchain.value,
                 sender_address=sender_address,
                 recipient_address=recipient_address,
                 source_token_contract_id=source_token_contract_id,
                 destination_token_contract_id=destination_token_contract_id,
-                amount=amount, fee=fee, sender_nonce=sender_nonce,
-                signature=signature, hub_contract_id=hub_contract_id,
+                amount=amount,
+                fee=fee,
+                sender_nonce=sender_nonce,
+                signature=signature,
+                hub_contract_id=hub_contract_id,
                 forwarder_contract_id=forwarder_contract_id,
                 status_id=TransferStatus.ACCEPTED.value)
             session.add(transfer)
             session.flush()
             return int(transfer.id)
     except sqlalchemy.exc.IntegrityError as e:
         session.rollback()
@@ -350,24 +359,26 @@
 
     statement = sqlalchemy.update(Transfer).where(
         sqlalchemy.or_(
             Transfer.id == internal_transfer_id,
             sqlalchemy.and_(
                 Transfer.source_blockchain_id == blockchain.value,
                 Transfer.nonce == minimum_failed_nonce_cte.c.min))).values({
-                    Transfer.nonce: sqlalchemy.case(
-                        (count_failed_nonces_subquery == 0,
-                         sqlalchemy.case((maximum_transfer_nonce_subquery
+                    Transfer.nonce:
+                    sqlalchemy.case((count_failed_nonces_subquery == 0,
+                                     sqlalchemy.case(
+                                         (maximum_transfer_nonce_subquery
                                           >= latest_blockchain_nonce,
                                           maximum_transfer_nonce_subquery + 1),
                                          else_=latest_blockchain_nonce)),
-                        (Transfer.id == internal_transfer_id,
-                         minimum_failed_nonce_cte.c.min),
-                        else_=sqlalchemy.null()),
-                    Transfer.status_id: sqlalchemy.case(
+                                    (Transfer.id == internal_transfer_id,
+                                     minimum_failed_nonce_cte.c.min),
+                                    else_=sqlalchemy.null()),
+                    Transfer.status_id:
+                    sqlalchemy.case(
                         (Transfer.id == internal_transfer_id,
                          TransferStatus.ACCEPTED_NEW_NONCE_ASSIGNED.value),
                         else_=sqlalchemy.case(
                             (Transfer.status_id == TransferStatus.FAILED.value,
                              TransferStatus.FAILED.value),
                             else_=TransferStatus.ACCEPTED.value))
                 })
```

## pantos/servicenode/database/exceptions.py

```diff
@@ -1,13 +1,14 @@
 """Module that defines database-specific exceptions.
 
 """
 import typing
 
 from pantos.common.blockchains.enums import Blockchain
+
 from pantos.servicenode.exceptions import ServiceNodeError
 
 
 class DatabaseError(ServiceNodeError):
     """Base exception class for all database errors.
 
     """
@@ -16,14 +17,15 @@
 
 class SenderNonceNotUniqueError(DatabaseError):
     """Error that is raised when an already existing sender nonce is
     requested to be added again for a specific blockchain and sender
     address.
 
     """
+
     def __init__(self, blockchain: Blockchain, sender_address: str,
                  sender_nonce: int, **kwargs: typing.Any):
         """Construct an error instance.
 
         Parameters
         ----------
         blockchain : Blockchain
@@ -32,10 +34,12 @@
             The blockchain address of the sender.
         sender_nonce : int
             The non-unique sender nonce.
         **kwargs : dict
             Additional information about the error as keyword arguments.
 
         """
-        super().__init__('sender nonce not unique', blockchain=blockchain,
+        super().__init__('sender nonce not unique',
+                         blockchain=blockchain,
                          sender_address=sender_address,
-                         sender_nonce=sender_nonce, **kwargs)
+                         sender_nonce=sender_nonce,
+                         **kwargs)
```

## pantos/servicenode/database/models.py

```diff
@@ -112,15 +112,17 @@
     blockchain_id = sqlalchemy.Column(sqlalchemy.Integer,
                                       sqlalchemy.ForeignKey('blockchains.id'),
                                       nullable=False)
     address = sqlalchemy.Column(sqlalchemy.Text, nullable=False)
     blockchain = sqlalchemy.orm.relationship('Blockchain',
                                              back_populates='token_contracts')
     __table_args__ = (sqlalchemy.schema.Index(
-        'ux_token_contracts_blockchain_id_address', blockchain_id, address,
+        'ux_token_contracts_blockchain_id_address',
+        blockchain_id,
+        address,
         unique=True), )
 
 
 class Bid(Base):
     """Model class for the "bids" database table. Each instance
     represents a service node bid registered at the Pantos Hub of a
     supported source blockchain.
@@ -141,20 +143,25 @@
         service node (in seconds).
     fee : sqlalchemy.Column
         The fee for a transfer (in PAN).
 
     """
     __tablename__ = 'bids'
     source_blockchain_id = sqlalchemy.Column(
-        sqlalchemy.Integer, sqlalchemy.ForeignKey('blockchains.id'),
-        nullable=False, primary_key=True)
+        sqlalchemy.Integer,
+        sqlalchemy.ForeignKey('blockchains.id'),
+        nullable=False,
+        primary_key=True)
     destination_blockchain_id = sqlalchemy.Column(
-        sqlalchemy.Integer, sqlalchemy.ForeignKey('blockchains.id'),
-        nullable=False, primary_key=True)
-    execution_time = sqlalchemy.Column(sqlalchemy.Integer, nullable=False,
+        sqlalchemy.Integer,
+        sqlalchemy.ForeignKey('blockchains.id'),
+        nullable=False,
+        primary_key=True)
+    execution_time = sqlalchemy.Column(sqlalchemy.Integer,
+                                       nullable=False,
                                        primary_key=True)
     valid_until = sqlalchemy.Column(sqlalchemy.Integer, nullable=False)
     fee = sqlalchemy.Column(
         # Large enough for a 256-bit unsigned integer
         sqlalchemy.Numeric(precision=78, scale=0),
         nullable=False)
 
@@ -240,55 +247,62 @@
     updated : sqlalchemy.Column
         The timestamp when the transfer was last updated.
 
     """
     __tablename__ = 'transfers'
     id = sqlalchemy.Column(sqlalchemy.Integer, primary_key=True)
     source_blockchain_id = sqlalchemy.Column(
-        sqlalchemy.Integer, sqlalchemy.ForeignKey('blockchains.id'),
+        sqlalchemy.Integer,
+        sqlalchemy.ForeignKey('blockchains.id'),
         nullable=False)
     destination_blockchain_id = sqlalchemy.Column(
-        sqlalchemy.Integer, sqlalchemy.ForeignKey('blockchains.id'),
+        sqlalchemy.Integer,
+        sqlalchemy.ForeignKey('blockchains.id'),
         nullable=False)
     sender_address = sqlalchemy.Column(sqlalchemy.Text, nullable=False)
     recipient_address = sqlalchemy.Column(sqlalchemy.Text, nullable=False)
     source_token_contract_id = sqlalchemy.Column(
-        sqlalchemy.Integer, sqlalchemy.ForeignKey('token_contracts.id'),
+        sqlalchemy.Integer,
+        sqlalchemy.ForeignKey('token_contracts.id'),
         nullable=False)
     destination_token_contract_id = sqlalchemy.Column(
-        sqlalchemy.Integer, sqlalchemy.ForeignKey('token_contracts.id'),
+        sqlalchemy.Integer,
+        sqlalchemy.ForeignKey('token_contracts.id'),
         nullable=False)
     amount = sqlalchemy.Column(
         # Large enough for a 256-bit unsigned integer
         sqlalchemy.Numeric(precision=78, scale=0),
         nullable=False)
     fee = sqlalchemy.Column(
         # Large enough for a 256-bit unsigned integer
         sqlalchemy.Numeric(precision=78, scale=0),
         nullable=False)
     sender_nonce = sqlalchemy.Column(
         # Large enough for a 256-bit unsigned integer
         sqlalchemy.Numeric(precision=78, scale=0))
     signature = sqlalchemy.Column(sqlalchemy.Text, nullable=False)
     hub_contract_id = sqlalchemy.Column(
-        sqlalchemy.Integer, sqlalchemy.ForeignKey('hub_contracts.id'),
+        sqlalchemy.Integer,
+        sqlalchemy.ForeignKey('hub_contracts.id'),
         nullable=False)
     forwarder_contract_id = sqlalchemy.Column(
-        sqlalchemy.Integer, sqlalchemy.ForeignKey('forwarder_contracts.id'),
+        sqlalchemy.Integer,
+        sqlalchemy.ForeignKey('forwarder_contracts.id'),
         nullable=False)
     task_id = sqlalchemy.Column(sqlalchemy.Text, unique=True)
     on_chain_transfer_id = sqlalchemy.Column(
         # Large enough for a 256-bit unsigned integer
         sqlalchemy.Numeric(precision=78, scale=0))
     transaction_id = sqlalchemy.Column(sqlalchemy.Text)
     nonce = sqlalchemy.Column(sqlalchemy.BigInteger)
     status_id = sqlalchemy.Column(sqlalchemy.Integer,
                                   sqlalchemy.ForeignKey('transfer_status.id'),
                                   nullable=False)
-    created = sqlalchemy.Column(sqlalchemy.DateTime, nullable=False,
+    created = sqlalchemy.Column(sqlalchemy.DateTime,
+                                nullable=False,
                                 default=datetime.datetime.utcnow)
     updated = sqlalchemy.Column(sqlalchemy.DateTime)
     source_blockchain = sqlalchemy.orm.relationship(
         'Blockchain',
         primaryjoin='Transfer.source_blockchain_id==Blockchain.id')
     destination_blockchain = sqlalchemy.orm.relationship(
         'Blockchain',
@@ -301,19 +315,23 @@
         'TokenContract',
         primaryjoin='Transfer.destination_token_contract_id==TokenContract.id',
         lazy='joined')
     hub_contract = sqlalchemy.orm.relationship('HubContract')
     forwarder_contract = sqlalchemy.orm.relationship('ForwarderContract')
     status = sqlalchemy.orm.relationship('TransferStatus')
     __table_args__ = (
-        sqlalchemy.UniqueConstraint(forwarder_contract_id, sender_address,
+        sqlalchemy.UniqueConstraint(forwarder_contract_id,
+                                    sender_address,
                                     sender_nonce,
                                     name=UNIQUE_SENDER_NONCE_CONSTRAINT),
         sqlalchemy.UniqueConstraint(hub_contract_id, on_chain_transfer_id),
         sqlalchemy.UniqueConstraint(source_blockchain_id, transaction_id),
         sqlalchemy.UniqueConstraint(
-            source_blockchain_id, nonce, status_id, deferrable=True,
+            source_blockchain_id,
+            nonce,
+            status_id,
+            deferrable=True,
             name='uq_transfers_source_blockchain_id_nonce_status_id'),
         sqlalchemy.schema.Index(
             'ix_transfers_source_blockchain_id_nonce_status_id',
             source_blockchain_id, nonce.desc(), status_id),
     )
```

## pantos/servicenode/database/migrations/env.py

```diff
@@ -43,16 +43,18 @@
     """
     alembic_ini_config: typing.Dict[str, str] = typing.cast(
         typing.Dict[str, str],
         alembic_config.get_section(
             alembic_config.config_ini_section)) if alembic_config.get_section(
                 alembic_config.config_ini_section) is not None else {}
     connectable = sqlalchemy.engine_from_config(
-        alembic_ini_config, url=config['database']['url'],
-        prefix="sqlalchemy.", poolclass=sqlalchemy.pool.NullPool)
+        alembic_ini_config,
+        url=config['database']['url'],
+        prefix="sqlalchemy.",
+        poolclass=sqlalchemy.pool.NullPool)
 
     with connectable.connect() as connection:
         alembic.context.configure(connection=connection,
                                   target_metadata=target_metadata)
 
         with alembic.context.begin_transaction():
             alembic.context.run_migrations()
```

## pantos/servicenode/database/migrations/versions/5e552e0ec844_remove_id_from_bids_table.py

```diff
@@ -21,11 +21,13 @@
     # ### end Alembic commands ###
 
 
 def downgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
     op.add_column(
         'bids',
-        sa.Column('id', sa.INTEGER(),
+        sa.Column('id',
+                  sa.INTEGER(),
                   server_default=sa.text("nextval('bids_id_seq'::regclass)"),
-                  autoincrement=True, nullable=False))
+                  autoincrement=True,
+                  nullable=False))
     # ### end Alembic commands ###
```

## pantos/servicenode/database/migrations/versions/85982c1f3b95_create_deferrable_constraint.py

```diff
@@ -16,27 +16,32 @@
 
 
 def upgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
     alembic.op.drop_index('ux_transfers_source_blockchain_id_nonce_status_id',
                           table_name='transfers')
     alembic.op.create_index(
-        'ix_transfers_source_blockchain_id_nonce_status_id', 'transfers',
+        'ix_transfers_source_blockchain_id_nonce_status_id',
+        'transfers',
         ['source_blockchain_id',
-         sa.text('nonce DESC'), 'status_id'], unique=False)
+         sa.text('nonce DESC'), 'status_id'],
+        unique=False)
     alembic.op.create_unique_constraint(
-        'uq_transfers_source_blockchain_id_nonce_status_id', 'transfers',
-        ['source_blockchain_id', 'nonce', 'status_id'], deferrable='True')
+        'uq_transfers_source_blockchain_id_nonce_status_id',
+        'transfers', ['source_blockchain_id', 'nonce', 'status_id'],
+        deferrable='True')
     # ### end Alembic commands ###
 
 
 def downgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
     alembic.op.drop_constraint(
-        'uq_transfers_source_blockchain_id_nonce_status_id', 'transfers',
+        'uq_transfers_source_blockchain_id_nonce_status_id',
+        'transfers',
         type_='unique')
     alembic.op.drop_index('ix_transfers_source_blockchain_id_nonce_status_id',
                           table_name='transfers')
     alembic.op.create_index(
-        'ux_transfers_source_blockchain_id_nonce_status_id', 'transfers',
-        ['source_blockchain_id', 'nonce', 'status_id'], unique=False)
+        'ux_transfers_source_blockchain_id_nonce_status_id',
+        'transfers', ['source_blockchain_id', 'nonce', 'status_id'],
+        unique=False)
     # ### end Alembic commands ###
```

## pantos/servicenode/database/migrations/versions/bd913c5bfdfb_off_chain_bids.py

```diff
@@ -27,30 +27,33 @@
     TransferTable = sa.Table('transfers', metadata, autoload_with=connection)
     transfer_fee_subquery = sa.select(BidTable.columns.fee).where(
         TransferTable.columns.bid_id == BidTable.columns.id).as_scalar()
     transfer_fee_update_statement = sa.update(TransferTable).where(
         TransferTable.columns.fee == sqlalchemy.null()).values(
             fee=transfer_fee_subquery)
     connection.execute(transfer_fee_update_statement)
-    alembic.op.alter_column('transfers', 'fee',
-                            existing_type=sa.NUMERIC(precision=78,
-                                                     scale=0), nullable=False)
-    alembic.op.drop_constraint('transfers_bid_id_fkey', 'transfers',
+    alembic.op.alter_column('transfers',
+                            'fee',
+                            existing_type=sa.NUMERIC(precision=78, scale=0),
+                            nullable=False)
+    alembic.op.drop_constraint('transfers_bid_id_fkey',
+                               'transfers',
                                type_='foreignkey')
     alembic.op.drop_column('transfers', 'bid_id')
     delete_bids_table_statement = sa.delete(BidTable)
     connection.execute(delete_bids_table_statement)
     alembic.op.add_column(
         'bids', sa.Column('valid_until', sa.Integer(), nullable=False))
     alembic.op.add_column(
         'bids', sa.Column('source_blockchain_id', sa.Integer(),
                           nullable=False))
     alembic.op.drop_index('ux_bids_hub_contract_id_on_chain_bid_id',
                           table_name='bids')
-    alembic.op.drop_constraint('bids_hub_contract_id_fkey', 'bids',
+    alembic.op.drop_constraint('bids_hub_contract_id_fkey',
+                               'bids',
                                type_='foreignkey')
     alembic.op.create_foreign_key('bids_source_blockchain_id', 'bids',
                                   'blockchains', ['source_blockchain_id'],
                                   ['id'])
     alembic.op.drop_column('bids', 'unregistered')
     alembic.op.drop_column('bids', 'on_chain_bid_id')
     alembic.op.drop_column('bids', 'registered')
@@ -58,36 +61,45 @@
     # ### end Alembic commands ###
 
 
 def downgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
     alembic.op.add_column(
         'bids',
-        sa.Column('hub_contract_id', sa.INTEGER(), autoincrement=False,
+        sa.Column('hub_contract_id',
+                  sa.INTEGER(),
+                  autoincrement=False,
                   nullable=False))
     alembic.op.add_column('transfers',
                           sa.Column('bid_id', sa.Integer(), nullable=False))
     alembic.op.create_foreign_key('bids_hub_contract_id_fkey', 'bids',
                                   'hub_contracts', ['hub_contract_id'], ['id'])
     alembic.op.create_foreign_key('transfers_bid_id_fkey', 'transfers', 'bids',
                                   ['bid_id'], ['id'])
     alembic.op.add_column(
         'bids',
-        sa.Column('registered', sqlalchemy.dialects.postgresql.TIMESTAMP(),
-                  autoincrement=False, nullable=True))
+        sa.Column('registered',
+                  sqlalchemy.dialects.postgresql.TIMESTAMP(),
+                  autoincrement=False,
+                  nullable=True))
     alembic.op.add_column(
         'bids',
-        sa.Column('on_chain_bid_id', sa.BIGINT(), autoincrement=False,
+        sa.Column('on_chain_bid_id',
+                  sa.BIGINT(),
+                  autoincrement=False,
                   nullable=True))
     alembic.op.add_column(
         'bids',
-        sa.Column('unregistered', sqlalchemy.dialects.postgresql.TIMESTAMP(),
-                  autoincrement=False, nullable=True))
-    alembic.op.create_index('ux_bids_hub_contract_id_on_chain_bid_id', 'bids',
-                            ['hub_contract_id', 'on_chain_bid_id'],
+        sa.Column('unregistered',
+                  sqlalchemy.dialects.postgresql.TIMESTAMP(),
+                  autoincrement=False,
+                  nullable=True))
+    alembic.op.create_index('ux_bids_hub_contract_id_on_chain_bid_id',
+                            'bids', ['hub_contract_id', 'on_chain_bid_id'],
                             unique=False)
-    alembic.op.drop_constraint('bids_source_blockchain_id', 'bids',
+    alembic.op.drop_constraint('bids_source_blockchain_id',
+                               'bids',
                                type_='foreignkey')
     alembic.op.drop_column('transfers', 'fee')
     alembic.op.drop_column('bids', 'valid_until')
     alembic.op.drop_column('bids', 'source_blockchain_id')
     # ### end Alembic commands ###
```

## pantos/servicenode/database/migrations/versions/c4c46d14ca6a_initial_database_schema.py

```diff
@@ -66,35 +66,38 @@
         sa.ForeignKeyConstraint(
             ['destination_blockchain_id'],
             ['blockchains.id'],
         ), sa.ForeignKeyConstraint(
             ['hub_contract_id'],
             ['hub_contracts.id'],
         ), sa.PrimaryKeyConstraint('id'))
-    alembic.op.create_index('ux_bids_hub_contract_id_on_chain_bid_id', 'bids',
-                            ['hub_contract_id', 'on_chain_bid_id'],
+    alembic.op.create_index('ux_bids_hub_contract_id_on_chain_bid_id',
+                            'bids', ['hub_contract_id', 'on_chain_bid_id'],
                             unique=True)
     alembic.op.create_table(
         'transfers', sa.Column('id', sa.Integer(), nullable=False),
         sa.Column('source_blockchain_id', sa.Integer(), nullable=False),
         sa.Column('destination_blockchain_id', sa.Integer(), nullable=False),
         sa.Column('sender_address', sa.Text(), nullable=False),
         sa.Column('recipient_address', sa.Text(), nullable=False),
         sa.Column('source_token_contract_id', sa.Integer(), nullable=False),
-        sa.Column('destination_token_contract_id', sa.Integer(),
+        sa.Column('destination_token_contract_id',
+                  sa.Integer(),
                   nullable=False),
         sa.Column('amount', sa.Numeric(precision=78, scale=0), nullable=False),
         sa.Column('bid_id', sa.Integer(), nullable=False),
-        sa.Column('sender_nonce', sa.Numeric(precision=78, scale=0),
+        sa.Column('sender_nonce',
+                  sa.Numeric(precision=78, scale=0),
                   nullable=True),
         sa.Column('signature', sa.Text(), nullable=False),
         sa.Column('hub_contract_id', sa.Integer(), nullable=False),
         sa.Column('forwarder_contract_id', sa.Integer(), nullable=False),
         sa.Column('task_id', sa.Text(), nullable=True),
-        sa.Column('on_chain_transfer_id', sa.Numeric(precision=78, scale=0),
+        sa.Column('on_chain_transfer_id',
+                  sa.Numeric(precision=78, scale=0),
                   nullable=True),
         sa.Column('transaction_id', sa.Text(), nullable=True),
         sa.Column('nonce', sa.BigInteger(), nullable=True),
         sa.Column('status_id', sa.Integer(), nullable=False),
         sa.Column('created', sa.DateTime(), nullable=False),
         sa.Column('updated', sa.DateTime(), nullable=True),
         sa.ForeignKeyConstraint(
@@ -123,23 +126,27 @@
         sa.ForeignKeyConstraint(
             ['source_token_contract_id'],
             ['token_contracts.id'],
         ), sa.ForeignKeyConstraint(
             ['status_id'],
             ['transfer_status.id'],
         ), sa.PrimaryKeyConstraint('id'),
-        sa.UniqueConstraint('forwarder_contract_id', 'sender_address',
-                            'sender_nonce', name='unique_sender_nonce'),
+        sa.UniqueConstraint('forwarder_contract_id',
+                            'sender_address',
+                            'sender_nonce',
+                            name='unique_sender_nonce'),
         sa.UniqueConstraint('hub_contract_id', 'on_chain_transfer_id'),
         sa.UniqueConstraint('source_blockchain_id', 'transaction_id'),
         sa.UniqueConstraint('task_id'))
     alembic.op.create_index(
-        'ux_transfers_source_blockchain_id_nonce_status_id', 'transfers',
+        'ux_transfers_source_blockchain_id_nonce_status_id',
+        'transfers',
         ['source_blockchain_id',
-         sa.text('nonce DESC'), 'status_id'], unique=True)
+         sa.text('nonce DESC'), 'status_id'],
+        unique=True)
     # ### end Alembic commands ###
 
 
 def downgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
     alembic.op.drop_index('ux_transfers_source_blockchain_id_nonce_status_id',
                           table_name='transfers')
```

## pantos/servicenode/plugins/__init__.py

```diff
@@ -1,22 +1,30 @@
 import importlib
-import typing
 
 from pantos.common.blockchains.enums import Blockchain
+
 from pantos.servicenode.configuration import get_blockchain_config
 from pantos.servicenode.configuration import get_plugin_config
 from pantos.servicenode.plugins.base import BidPlugin
 
 _DEFAULT_PLUGIN = 'pantos.servicenode.plugins.bids.ConfigFileBidPlugin'
 """Default plugin to use if no plugin is configured."""
 
-_bid_plugin: typing.Optional[BidPlugin] = None
+_bid_plugin: BidPlugin | None = None
 
 
 def get_bid_plugin():
+    """Get the bid plugin.
+
+    Returns
+    -------
+    BidPlugin
+        The initialized bid plugin.
+
+    """
     return _bid_plugin
 
 
 def initialize_plugins(start_worker: bool):
     """Initialize the plugins by loading the code from the specified location
     in the configuration.
 
@@ -30,18 +38,18 @@
     from pantos.servicenode.business.plugins import execute_bid_plugin
     global _bid_plugin
 
     _bid_plugin = _import_bid_plugin()
     if start_worker:
         for source_blockchain in Blockchain:
             source_blockchain_config = get_blockchain_config(source_blockchain)
-
-            if not source_blockchain_config['active']:
+            active = source_blockchain_config['active']
+            registered = source_blockchain_config['registered']
+            if not active or not registered:
                 continue
-
             execute_bid_plugin.delay(source_blockchain)
 
 
 def _import_bid_plugin() -> BidPlugin:
     plugin_config = get_plugin_config()
     if plugin_config['bids']['class']:
         class_config = plugin_config['bids']['class'].split('.')
```

## pantos/servicenode/plugins/base.py

```diff
@@ -34,14 +34,15 @@
     destination_blockchain_id: int
     fee: int
     execution_time: int
     valid_until: int
 
 
 class BidPlugin(abc.ABC):
+
     @abc.abstractmethod
     def get_bids(
             self, source_blockchain_id: int, destination_blockchain_id: int,
             **kwargs: typing.Any) \
             -> typing.Tuple[collections.abc.Iterable[Bid], int]:
         """Calculates bid fees for a token transfer from a source blockchain
         to a destination blockchain.
```

## pantos/servicenode/plugins/bids.py

```diff
@@ -1,13 +1,14 @@
 import collections.abc
 import time
 import typing
 
 from pantos.common.blockchains.enums import Blockchain
 from pantos.common.configuration import Config
+
 from pantos.servicenode.plugins.base import Bid
 from pantos.servicenode.plugins.base import BidPlugin
 from pantos.servicenode.plugins.base import BidPluginError
 
 _BLOCKCHAIN_NAME_REGEX = "|".join([b.name.lower() for b in Blockchain])
 
 _BIDS_SCHEMA = {
@@ -56,14 +57,15 @@
     Attributes
     ----------
     config : Config
         The configuration object.
     delay : int
         The delay in seconds until the next bid calculation.
     """
+
     def __init__(self):
         """Initializes the plugin.
         """
         self.config = None
         self.delay = 60
 
     def get_bids(
```

## Comparing `pantos_service_node-1.6.0.dist-info/LICENSE.md` & `pantos_service_node-1.7.0.dist-info/LICENSE.md`

 * *Files identical despite different names*

