# Comparing `tmp/ledgerwallet-0.4.0.tar.gz` & `tmp/ledgerwallet-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ledgerwallet-0.4.0.tar", last modified: Wed Dec  6 13:54:50 2023, max compression
+gzip compressed data, was "ledgerwallet-0.5.0.tar", last modified: Mon May 27 11:07:58 2024, max compression
```

## Comparing `ledgerwallet-0.4.0.tar` & `ledgerwallet-0.5.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:54:50.248223 ledgerwallet-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:54:50.236223 ledgerwallet-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:54:50.240223 ledgerwallet-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      260 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7658 2023-12-06 13:54:50.248223 ledgerwallet-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:54:50.240223 ledgerwallet-0.4.0/ledgerwallet/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-06 13:54:50.000000 ledgerwallet-0.4.0/ledgerwallet/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15487 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:54:50.244223 ledgerwallet-0.4.0/ledgerwallet/crypto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/crypto/ecc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/crypto/scp.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/hsmscript.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/hsmserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    13247 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/ledgerctl.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/ledgerserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/manifest_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/manifest_toml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:54:50.244223 ledgerwallet-0.4.0/ledgerwallet/proto/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/proto/LedgerHSMServer.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/proto/LedgerHSMServer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/proto/LedgerHSMServer_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/proto/listApps.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/proto/listApps_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/proto/listApps_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/simpleserver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:54:50.244223 ledgerwallet-0.4.0/ledgerwallet/transport/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/transport/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/transport/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/transport/hid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/transport/tcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/ledgerwallet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:54:50.248223 ledgerwallet-0.4.0/ledgerwallet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7658 2023-12-06 13:54:50.000000 ledgerwallet-0.4.0/ledgerwallet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2023-12-06 13:54:50.000000 ledgerwallet-0.4.0/ledgerwallet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 13:54:50.000000 ledgerwallet-0.4.0/ledgerwallet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-06 13:54:50.000000 ledgerwallet-0.4.0/ledgerwallet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-12-06 13:54:50.000000 ledgerwallet-0.4.0/ledgerwallet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-06 13:54:50.000000 ledgerwallet-0.4.0/ledgerwallet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-12-06 13:54:50.248223 ledgerwallet-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:54:50.236223 ledgerwallet-0.4.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:54:50.244223 ledgerwallet-0.4.0/tests/app/
--rw-r--r--   0 runner    (1001) docker     (127)    53376 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/tests/app/app.hex
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/tests/app/app.json
--rw-r--r--   0 runner    (1001) docker     (127)      194 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/tests/app/app.toml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/tests/app/nanos_app_ssh.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:54:50.248223 ledgerwallet-0.4.0/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:54:50.248223 ledgerwallet-0.4.0/tests/unit/crypto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/tests/unit/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/tests/unit/crypto/test_ecc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:54:50.248223 ledgerwallet-0.4.0/tests/unit/data/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/tests/unit/data/empty_manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/tests/unit/data/empty_manifest.toml
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/tests/unit/data/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)      233 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/tests/unit/data/manifest.toml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/tests/unit/data/minimal_manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/tests/unit/data/minimal_manifest.toml
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/tests/unit/data/missing_binary_manifest.toml
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/tests/unit/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      742 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/tests/unit/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/tests/unit/test_manifest_ManifestJSON.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/tests/unit/test_manifest_ManifestTOML.py
--rw-r--r--   0 runner    (1001) docker     (127)     6288 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/tests/unit/test_params.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2023-12-06 13:54:37.000000 ledgerwallet-0.4.0/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:07:58.727129 ledgerwallet-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:07:58.715129 ledgerwallet-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:07:58.719128 ledgerwallet-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7658 2024-05-27 11:07:58.727129 ledgerwallet-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:07:58.719128 ledgerwallet-0.5.0/ledgerwallet/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-27 11:07:58.000000 ledgerwallet-0.5.0/ledgerwallet/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:07:58.723129 ledgerwallet-0.5.0/ledgerwallet/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/crypto/ecc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/crypto/scp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/hsmscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/hsmserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13247 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/ledgerctl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/ledgerserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7563 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/manifest_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/manifest_toml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:07:58.723129 ledgerwallet-0.5.0/ledgerwallet/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/proto/LedgerHSMServer.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/proto/LedgerHSMServer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/proto/LedgerHSMServer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/proto/listApps.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/proto/listApps_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/proto/listApps_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/simpleserver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:07:58.723129 ledgerwallet-0.5.0/ledgerwallet/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/transport/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/transport/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/transport/hid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/transport/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/ledgerwallet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:07:58.727129 ledgerwallet-0.5.0/ledgerwallet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7658 2024-05-27 11:07:58.000000 ledgerwallet-0.5.0/ledgerwallet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-27 11:07:58.000000 ledgerwallet-0.5.0/ledgerwallet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 11:07:58.000000 ledgerwallet-0.5.0/ledgerwallet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-27 11:07:58.000000 ledgerwallet-0.5.0/ledgerwallet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-27 11:07:58.000000 ledgerwallet-0.5.0/ledgerwallet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 11:07:58.000000 ledgerwallet-0.5.0/ledgerwallet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-27 11:07:58.727129 ledgerwallet-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:07:58.715129 ledgerwallet-0.5.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:07:58.723129 ledgerwallet-0.5.0/tests/app/
+-rw-r--r--   0 runner    (1001) docker     (127)    53376 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/tests/app/app.hex
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/tests/app/app.json
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/tests/app/app.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/tests/app/nanos_app_ssh.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:07:58.723129 ledgerwallet-0.5.0/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:07:58.723129 ledgerwallet-0.5.0/tests/unit/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/tests/unit/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/tests/unit/crypto/test_ecc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:07:58.727129 ledgerwallet-0.5.0/tests/unit/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/tests/unit/data/empty_manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/tests/unit/data/empty_manifest.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/tests/unit/data/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/tests/unit/data/manifest.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/tests/unit/data/minimal_manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/tests/unit/data/minimal_manifest.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/tests/unit/data/missing_binary_manifest.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/tests/unit/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/tests/unit/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/tests/unit/test_manifest_ManifestJSON.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/tests/unit/test_manifest_ManifestTOML.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6288 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/tests/unit/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-27 11:07:47.000000 ledgerwallet-0.5.0/tests/unit/test_utils.py
```

### Comparing `ledgerwallet-0.4.0/.github/workflows/ci.yml` & `ledgerwallet-0.5.0/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             echo "- Not triggered from tag, will be deployed on test.pypi.org"; \
         fi
         echo "- Tag version: ${{ env.TAG_VERSION }}"
 
     - name: Check version against CHANGELOG
       if: startsWith(github.ref, 'refs/tags/')
       run: |
-        CHANGELOG_VERSION=$(grep -Po '(?<=## \[)(\d\.)+[^\]]' CHANGELOG.md | head -n 1)
+        CHANGELOG_VERSION=$(grep -Po '(?<=## \[)(\d+\.)+[^\]]' CHANGELOG.md | head -n 1)
         if [ "${{ env.TAG_VERSION }}" == "${CHANGELOG_VERSION}" ]; \
         then \
             exit 0; \
         else \
             echo "Tag '${{ env.TAG_VERSION }}' and CHANGELOG '${CHANGELOG_VERSION}' versions mismatch!"; \
             exit 1; \
         fi
```

### Comparing `ledgerwallet-0.4.0/.github/workflows/codeql-analysis.yml` & `ledgerwallet-0.5.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/.gitignore` & `ledgerwallet-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/.pre-commit-config.yaml` & `ledgerwallet-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/CHANGELOG.md` & `ledgerwallet-0.5.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.5.0] - 2024-05-22
+
+### Add
+
+- Support for Stax and Flex dashboard icon generation when installing apps.
+
 ## [0.4.0] - 2023-12-06
 
 ### Add
 
 - offline mode : Add an option to allow dumping the APDU installation / delete file instead of trying to send it to a device.
 
 ## [0.3.0] - 2023-05-29
```

### Comparing `ledgerwallet-0.4.0/LICENSE` & `ledgerwallet-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/PKG-INFO` & `ledgerwallet-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledgerwallet
-Version: 0.4.0
+Version: 0.5.0
 Summary: Library to communicate with Ledger Nano S/X and Speculos
 Author-email: Ledger <hello@ledger.fr>
 License: MIT License
         
         Copyright (c) 2019 Ledger
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ledgerwallet-0.4.0/README.md` & `ledgerwallet-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/ledgerwallet/client.py` & `ledgerwallet-0.5.0/ledgerwallet/client.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/ledgerwallet/crypto/ecc.py` & `ledgerwallet-0.5.0/ledgerwallet/crypto/ecc.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/ledgerwallet/crypto/scp.py` & `ledgerwallet-0.5.0/ledgerwallet/crypto/scp.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/ledgerwallet/hsmserver.py` & `ledgerwallet-0.5.0/ledgerwallet/hsmserver.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/ledgerwallet/ledgerctl.py` & `ledgerwallet-0.5.0/ledgerwallet/ledgerctl.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/ledgerwallet/manifest_json.py` & `ledgerwallet-0.5.0/ledgerwallet/manifest_json.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         for entry, value in self.dic.items():
             if entry == "name":
                 parameters.append({"type_": "BOLOS_TAG_APPNAME", "value": value})
             elif entry == "version":
                 parameters.append({"type_": "BOLOS_TAG_APPVERSION", "value": value})
             elif entry == "icon":
                 parameters.append(
-                    {"type_": "BOLOS_TAG_ICON", "value": icon_from_file(value)}
+                    {"type_": "BOLOS_TAG_ICON", "value": icon_from_file(value, device)}
                 )
             elif entry == "derivationPath":
                 derivation_paths = self.serialize_derivation_path(value)
                 parameters.append(
                     {"type_": "BOLOS_TAG_DERIVEPATH", "value": derivation_paths}
                 )
         return params.AppParams.build(parameters)
```

### Comparing `ledgerwallet-0.4.0/ledgerwallet/manifest_toml.py` & `ledgerwallet-0.5.0/ledgerwallet/manifest_toml.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                 parameters.append({"type_": "BOLOS_TAG_APPVERSION", "value": value})
             elif entry == device:
                 for device_entry, device_value in self.dic[entry].items():
                     if device_entry == "icon":
                         parameters.append(
                             {
                                 "type_": "BOLOS_TAG_ICON",
-                                "value": icon_from_file(device_value),
+                                "value": icon_from_file(device_value, device),
                             }
                         )
                     elif device_entry == "derivationPath":
                         derivation_paths = self.serialize_derivation_path(device_value)
                         parameters.append(
                             {"type_": "BOLOS_TAG_DERIVEPATH", "value": derivation_paths}
                         )
```

### Comparing `ledgerwallet-0.4.0/ledgerwallet/params.py` & `ledgerwallet-0.5.0/ledgerwallet/params.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/ledgerwallet/proto/LedgerHSMServer_pb2.py` & `ledgerwallet-0.5.0/ledgerwallet/proto/LedgerHSMServer_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,23 +7,21 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-
-
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15LedgerHSMServer.proto\x12\rbluehsmserver\"7\n\tParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x61lias\x18\x02 \x01(\t\x12\r\n\x05local\x18\x03 \x01(\x08\"\xa1\x01\n\x07Request\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nparameters\x18\x02 \x01(\x0c\x12\x11\n\treference\x18\x03 \x01(\t\x12\x0b\n\x03\x65lf\x18\x04 \x01(\x0c\x12\r\n\x05\x63lose\x18\x05 \x01(\x08\x12\x12\n\nlargeStack\x18\x06 \x01(\x08\x12\x33\n\x11remote_parameters\x18\x07 \x03(\x0b\x32\x18.bluehsmserver.Parameter\"L\n\x08Response\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08response\x18\x02 \x01(\x0c\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\x11\n\texception\x18\x04 \x01(\tb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'LedgerHSMServer_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
-  DESCRIPTOR._options = None
-  _PARAMETER._serialized_start=40
-  _PARAMETER._serialized_end=95
-  _REQUEST._serialized_start=98
-  _REQUEST._serialized_end=259
-  _RESPONSE._serialized_start=261
-  _RESPONSE._serialized_end=337
+    DESCRIPTOR._options = None
+    _PARAMETER._serialized_start = 40
+    _PARAMETER._serialized_end = 95
+    _REQUEST._serialized_start = 98
+    _REQUEST._serialized_end = 259
+    _RESPONSE._serialized_start = 261
+    _RESPONSE._serialized_end = 337
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ledgerwallet-0.4.0/ledgerwallet/proto/LedgerHSMServer_pb2.pyi` & `ledgerwallet-0.5.0/ledgerwallet/proto/LedgerHSMServer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/ledgerwallet/proto/listApps_pb2.py` & `ledgerwallet-0.5.0/ledgerwallet/proto/listApps_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,21 +7,20 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0elistApps.proto\x12\x08listapps\"F\n\x03\x41pp\x12\r\n\x05\x66lags\x18\x01 \x01(\r\x12\x0c\n\x04hash\x18\x02 \x01(\x0c\x12\x14\n\x0chashCodeData\x18\x03 \x01(\x0c\x12\x0c\n\x04name\x18\x04 \x01(\t\"&\n\x07\x41ppList\x12\x1b\n\x04list\x18\x01 \x03(\x0b\x32\r.listapps.Appb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
+    b'\n\x0elistApps.proto\x12\x08listapps\"F\n\x03\x41pp\x12\r\n\x05\x66lags\x18\x01 \x01(\r\x12\x0c\n\x04hash\x18\x02 \x01(\x0c\x12\x14\n\x0chashCodeData\x18\x03 \x01(\x0c\x12\x0c\n\x04name\x18\x04 \x01(\t\"&\n\x07\x41ppList\x12\x1b\n\x04list\x18\x01 \x03(\x0b\x32\r.listapps.Appb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'listApps_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
-  DESCRIPTOR._options = None
-  _APP._serialized_start=28
-  _APP._serialized_end=98
-  _APPLIST._serialized_start=100
-  _APPLIST._serialized_end=138
+    DESCRIPTOR._options = None
+    _APP._serialized_start = 28
+    _APP._serialized_end = 98
+    _APPLIST._serialized_start = 100
+    _APPLIST._serialized_end = 138
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ledgerwallet-0.4.0/ledgerwallet/proto/listApps_pb2.pyi` & `ledgerwallet-0.5.0/ledgerwallet/proto/listApps_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/ledgerwallet/simpleserver.py` & `ledgerwallet-0.5.0/ledgerwallet/simpleserver.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/ledgerwallet/transport/__init__.py` & `ledgerwallet-0.5.0/ledgerwallet/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/ledgerwallet/transport/device.py` & `ledgerwallet-0.5.0/ledgerwallet/transport/device.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/ledgerwallet/transport/file.py` & `ledgerwallet-0.5.0/ledgerwallet/transport/file.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/ledgerwallet/transport/hid.py` & `ledgerwallet-0.5.0/ledgerwallet/transport/hid.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/ledgerwallet/transport/tcp.py` & `ledgerwallet-0.5.0/ledgerwallet/transport/tcp.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/ledgerwallet/utils.py` & `ledgerwallet-0.5.0/ledgerwallet/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 
 class DeviceNames(Enum):
     LEDGER_NANO_S = "Ledger Nano S"
     LEDGER_NANO_X = "Ledger Nano X"
     LEDGER_NANO_SP = "Ledger Nano S+"
     LEDGER_BLUE = "Ledger Blue"
+    LEDGER_STAX = "Ledger Stax"
+    LEDGER_FLEX = "Ledger Flex"
 
 
 class LedgerIns(IntEnum):
     SECUINS = 0
     GET_VERSION = 1
     VALIDATE_TARGET_ID = 4
     INITIALIZE_AUTHENTICATION = 0x50
@@ -95,14 +97,16 @@
         0x31100002: DeviceNames.LEDGER_NANO_S.value,  # firmware version <= 1.3.1
         0x31100003: DeviceNames.LEDGER_NANO_S.value,  # firmware version > 1.3.1
         0x31100004: DeviceNames.LEDGER_NANO_S.value,  # firmware version >= 1.5
         0x31000002: DeviceNames.LEDGER_BLUE.value,  # firmware version <= 2.0
         0x31010004: DeviceNames.LEDGER_BLUE.value,  # firmware version > 2.0
         0x33000004: DeviceNames.LEDGER_NANO_X.value,
         0x33100004: DeviceNames.LEDGER_NANO_SP.value,
+        0x33200004: DeviceNames.LEDGER_STAX.value,
+        0x33300004: DeviceNames.LEDGER_FLEX.value,
     }
     return target_ids.get(target_id, "Unknown device")
 
 
 def decode_flags(flags: int):
     flag_values = {
         1: "issuer",
```

### Comparing `ledgerwallet-0.4.0/ledgerwallet.egg-info/PKG-INFO` & `ledgerwallet-0.5.0/ledgerwallet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledgerwallet
-Version: 0.4.0
+Version: 0.5.0
 Summary: Library to communicate with Ledger Nano S/X and Speculos
 Author-email: Ledger <hello@ledger.fr>
 License: MIT License
         
         Copyright (c) 2019 Ledger
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ledgerwallet-0.4.0/ledgerwallet.egg-info/SOURCES.txt` & `ledgerwallet-0.5.0/ledgerwallet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/pyproject.toml` & `ledgerwallet-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/tests/app/app.hex` & `ledgerwallet-0.5.0/tests/app/app.hex`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/tests/unit/crypto/test_ecc.py` & `ledgerwallet-0.5.0/tests/unit/crypto/test_ecc.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/tests/unit/test_device.py` & `ledgerwallet-0.5.0/tests/unit/test_device.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/tests/unit/test_manifest_ManifestJSON.py` & `ledgerwallet-0.5.0/tests/unit/test_manifest_ManifestJSON.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,11 +62,12 @@
             "23" +  # 35: following size
             "05" +  # secp256k1 (1) + ed25519 (4)
             "03" + "8000002c80000000000000ff" +                # "44'/0'/255"
             "05" + "8000002c80000000800000000000000100000190"  # "44'/0'/0'/1/400"
         )
         # fmt: on
         with patch(
-            "ledgerwallet.manifest_json.icon_from_file", lambda x: b"\x01\x02\x03\x04"
+            "ledgerwallet.manifest_json.icon_from_file",
+            lambda x, y: b"\x01\x02\x03\x04",
         ):
             result_json = self.json_manifest.serialize_parameters("1234")
         self.assertEqual(result_json, expected)
```

### Comparing `ledgerwallet-0.4.0/tests/unit/test_manifest_ManifestTOML.py` & `ledgerwallet-0.5.0/tests/unit/test_manifest_ManifestTOML.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,11 +72,12 @@
             "23" +  # 35: following size
             "05" +  # secp256k1 (1) + ed25519 (4)
             "03" + "8000002c80000000000000ff" +                # "44'/0'/255"
             "05" + "8000002c80000000800000000000000100000190"  # "44'/0'/0'/1/400"
         )
         # fmt: on
         with patch(
-            "ledgerwallet.manifest_toml.icon_from_file", lambda x: b"\x01\x02\x03\x04"
+            "ledgerwallet.manifest_toml.icon_from_file",
+            lambda x, y: b"\x01\x02\x03\x04",
         ):
             result_toml = self.toml_manifest.serialize_parameters("1234")
         self.assertEqual(result_toml, expected)
```

### Comparing `ledgerwallet-0.4.0/tests/unit/test_params.py` & `ledgerwallet-0.5.0/tests/unit/test_params.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.4.0/tests/unit/test_utils.py` & `ledgerwallet-0.5.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

