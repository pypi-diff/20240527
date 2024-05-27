# Comparing `tmp/ape-etherscan-0.7.3.tar.gz` & `tmp/ape-etherscan-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-etherscan-0.7.3.tar", last modified: Thu May  9 01:59:02 2024, max compression
+gzip compressed data, was "ape-etherscan-0.7.4.tar", last modified: Mon May 27 16:07:41 2024, max compression
```

## Comparing `ape-etherscan-0.7.3.tar` & `ape-etherscan-0.7.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:59:02.611034 ape-etherscan-0.7.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:59:02.603034 ape-etherscan-0.7.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:59:02.603034 ape-etherscan-0.7.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:59:02.607034 ape-etherscan-0.7.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-09 01:59:02.611034 ape-etherscan-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:59:02.607034 ape-etherscan-0.7.3/ape_etherscan/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/ape_etherscan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/ape_etherscan/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/ape_etherscan/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/ape_etherscan/dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/ape_etherscan/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/ape_etherscan/explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/ape_etherscan/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/ape_etherscan/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/ape_etherscan/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/ape_etherscan/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16537 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/ape_etherscan/verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 01:59:02.000000 ape-etherscan-0.7.3/ape_etherscan/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:59:02.607034 ape-etherscan-0.7.3/ape_etherscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-09 01:59:02.000000 ape-etherscan-0.7.3/ape_etherscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-09 01:59:02.000000 ape-etherscan-0.7.3/ape_etherscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 01:59:02.000000 ape-etherscan-0.7.3/ape_etherscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 01:59:02.000000 ape-etherscan-0.7.3/ape_etherscan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-09 01:59:02.000000 ape-etherscan-0.7.3/ape_etherscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-09 01:59:02.000000 ape-etherscan-0.7.3/ape_etherscan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-09 01:59:02.611034 ape-etherscan-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:59:02.607034 ape-etherscan-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21852 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:59:02.611034 ape-etherscan-0.7.3/tests/mock_responses/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/mock_responses/get_account_transactions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/mock_responses/get_account_transactions_with_ctor_args.json
--rw-r--r--   0 runner    (1001) docker     (127)    85182 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/mock_responses/get_contract_response_flattened.json
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/mock_responses/get_contract_response_json.json
--rw-r--r--   0 runner    (1001) docker     (127)    21603 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/mock_responses/get_contract_response_json_source_code.json
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/mock_responses/get_contract_response_not_verified.json
--rw-r--r--   0 runner    (1001) docker     (127)    93453 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/mock_responses/get_proxy_contract_response.json
--rw-r--r--   0 runner    (1001) docker     (127)    93483 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/mock_responses/get_vyper_contract_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/test_dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/test_etherscan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:07:41.404014 ape-etherscan-0.7.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:07:41.396014 ape-etherscan-0.7.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:07:41.396014 ape-etherscan-0.7.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:07:41.400014 ape-etherscan-0.7.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-27 16:07:41.404014 ape-etherscan-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:07:41.400014 ape-etherscan-0.7.4/ape_etherscan/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/ape_etherscan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/ape_etherscan/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/ape_etherscan/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/ape_etherscan/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/ape_etherscan/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/ape_etherscan/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/ape_etherscan/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/ape_etherscan/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/ape_etherscan/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/ape_etherscan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18535 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/ape_etherscan/verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-27 16:07:41.000000 ape-etherscan-0.7.4/ape_etherscan/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:07:41.400014 ape-etherscan-0.7.4/ape_etherscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-27 16:07:41.000000 ape-etherscan-0.7.4/ape_etherscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-27 16:07:41.000000 ape-etherscan-0.7.4/ape_etherscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:07:41.000000 ape-etherscan-0.7.4/ape_etherscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:07:41.000000 ape-etherscan-0.7.4/ape_etherscan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-27 16:07:41.000000 ape-etherscan-0.7.4/ape_etherscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-27 16:07:41.000000 ape-etherscan-0.7.4/ape_etherscan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-27 16:07:41.404014 ape-etherscan-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:07:41.400014 ape-etherscan-0.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21852 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:07:41.404014 ape-etherscan-0.7.4/tests/mock_responses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/mock_responses/get_account_transactions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/mock_responses/get_account_transactions_with_ctor_args.json
+-rw-r--r--   0 runner    (1001) docker     (127)    85182 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/mock_responses/get_contract_response_flattened.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/mock_responses/get_contract_response_json.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21603 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/mock_responses/get_contract_response_json_source_code.json
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/mock_responses/get_contract_response_not_verified.json
+-rw-r--r--   0 runner    (1001) docker     (127)    93453 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/mock_responses/get_proxy_contract_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)    93483 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/mock_responses/get_vyper_contract_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/test_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/test_etherscan.py
```

### Comparing `ape-etherscan-0.7.3/.github/ISSUE_TEMPLATE/bug.md` & `ape-etherscan-0.7.4/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/.github/ISSUE_TEMPLATE/feature.md` & `ape-etherscan-0.7.4/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/.github/ISSUE_TEMPLATE/work-item.md` & `ape-etherscan-0.7.4/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/.github/release-drafter.yml` & `ape-etherscan-0.7.4/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/.github/workflows/codeql.yml` & `ape-etherscan-0.7.4/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/.github/workflows/commit.yaml` & `ape-etherscan-0.7.4/.github/workflows/commit.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/.github/workflows/prtitle.yaml` & `ape-etherscan-0.7.4/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/.github/workflows/publish.yaml` & `ape-etherscan-0.7.4/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/.github/workflows/stale-prs.yml` & `ape-etherscan-0.7.4/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/.github/workflows/test.yaml` & `ape-etherscan-0.7.4/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/.gitignore` & `ape-etherscan-0.7.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/.pre-commit-config.yaml` & `ape-etherscan-0.7.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/CONTRIBUTING.md` & `ape-etherscan-0.7.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/LICENSE` & `ape-etherscan-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/PKG-INFO` & `ape-etherscan-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-etherscan
-Version: 0.7.3
+Version: 0.7.4
 Summary: ape-etherscan: Etherscan Explorer Plugin for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-etherscan
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ape-etherscan-0.7.3/README.md` & `ape-etherscan-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/ape_etherscan/__init__.py` & `ape-etherscan-0.7.4/ape_etherscan/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/ape_etherscan/client.py` & `ape-etherscan-0.7.4/ape_etherscan/client.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/ape_etherscan/config.py` & `ape-etherscan-0.7.4/ape_etherscan/config.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/ape_etherscan/dependency.py` & `ape-etherscan-0.7.4/ape_etherscan/dependency.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/ape_etherscan/exceptions.py` & `ape-etherscan-0.7.4/ape_etherscan/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/ape_etherscan/explorer.py` & `ape-etherscan-0.7.4/ape_etherscan/explorer.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/ape_etherscan/query.py` & `ape-etherscan-0.7.4/ape_etherscan/query.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/ape_etherscan/types.py` & `ape-etherscan-0.7.4/ape_etherscan/types.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/ape_etherscan/utils.py` & `ape-etherscan-0.7.4/ape_etherscan/utils.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/ape_etherscan/verify.py` & `ape-etherscan-0.7.4/ape_etherscan/verify.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 from ethpm_types import Compiler, ContractType
 
 from ape_etherscan.client import AccountClient, ClientFactory, ContractClient
 from ape_etherscan.exceptions import ContractVerificationError, EtherscanResponseError
 
 DEFAULT_OPTIMIZATION_RUNS = 200
 _SPDX_ID_TO_API_CODE = {
+    "none": 1,
+    "no-license": 1,
+    "no-permission": 1,
+    "unlicensed": 1,
     "unlicense": 2,
     "mit": 3,
     "gpl-2.0": 4,
     "gpl-3.0": 5,
     "lgpl-2.1": 6,
     "lgpl-3.0": 7,
     "bsd-2-clause": 8,
@@ -40,84 +44,109 @@
 class LicenseType(Enum):
     """
     https://etherscan.io/contract-license-types
     """
 
     NO_LICENSE = 1
     """
-    Nobody else can copy, distribute, or modify your work without being at risk of
+    Nobody else can copy, distribute, or modify your work without risk of
     take-downs, shake-downs, or litigation.
+    https://github.com/github/choosealicense.com/blob/gh-pages/no-permission.md
     """
 
-    UNLICENSED = 2
+    UNLICENSE = 2
     """
-    A license with no conditions whatsoever which dedicates works to the public domain.
+    Unlicensed works, modifications, and larger works may be distributed
+    under different terms and without source code.
+    https://github.com/github/choosealicense.com/blob/gh-pages/_licenses/unlicense.txt
     """
 
     MIT = 3
     """
-    Licensed works, modifications, and larger works may be distributed under different
-    terms and without source code.
+    Licensed works, modifications, and larger works may be distributed
+    under different terms and without source code.
+    https://github.com/github/choosealicense.com/blob/gh-pages/_licenses/mit.txt
     """
 
     GPL_2 = 4
     """
+    The source code of derived works must be made available under the same license.
     https://github.com/github/choosealicense.com/blob/gh-pages/_licenses/gpl-2.0.txt
     """
 
     GPL_3 = 5
     """
+    When distributing derived works, the source code of the work must be made available
+    under the same license and contributors provide an express grant of patent rights.
     https://github.com/github/choosealicense.com/blob/gh-pages/_licenses/gpl-3.0.txt
     """
 
     LGLP_2_1 = 6
     """
+    Derived works must be licensed under the same license, but works that only link
+    to it do not fall under this restriction.
     https://github.com/github/choosealicense.com/blob/gh-pages/_licenses/lgpl-3.0.txt
     """
 
     LGLP_3 = 7
     """
+    When distributing derived works, the source code of the work must be made available
+    under the same license and contributors provide an express grant of patent rights
+    with exceptions for a larger works using provided interfaces.
     https://github.com/github/choosealicense.com/blob/gh-pages/_licenses/lgpl-3.0.txt
     """
 
     BSD_2_CLAUSE = 8
     """
+    Licensed works, modifications, and larger works may be distributed under different
+    terms and without source code.
     https://github.com/github/choosealicense.com/blob/gh-pages/_licenses/bsd-2-clause.txt
     """
 
     BSD_3_CLAUSE = 9
     """
+    Licensed works, modifications, and larger works may be distributed under different
+    terms and without source code. The name of the project or its contributors may not
+    be used to promote derived products without written consent.
     https://github.com/github/choosealicense.com/blob/gh-pages/_licenses/bsd-3-clause.txt
     """
 
     MPL_2 = 10
     """
+    Source code must be made available of licensed/modified files, but not additional files.
+    Copyright and license notices must be preserved. Contributors grant patent rights.
     https://github.com/github/choosealicense.com/blob/gh-pages/_licenses/mpl-2.0.txt
     """
 
     OSL_3 = 11
     """
+    Does not require reciprocal licensing on linked works.
     https://github.com/github/choosealicense.com/blob/gh-pages/_licenses/osl-3.0.txt
     """
 
     APACHE = 2
     """
+    Requires preservation of copyright and license notices.  Licensed works, modifications,
+    and larger works may be distributed under different terms and without source code.
     https://github.com/github/choosealicense.com/blob/gh-pages/_licenses/apache-2.0.txt
     """
 
     AGLP_3 = 13
     """
+    When a modified version is used to provide a service over a network, the complete
+    source code of the modified version must be made available.
     https://github.com/github/choosealicense.com/blob/gh-pages/_licenses/agpl-3.0.txt
     """
 
     BUSL_1_1 = 14
     """
     The BSL is structured to allow free and open usage for many use cases, and only requires
     a commercial license by those who make production use of the software, which is typically
     indicative of an environment that is delivering significant value to a business.
+    https://github.com/github/choosealicense.com/blob/gh-pages/_licenses/bsl-1.0.txt
     """
 
     @classmethod
     def from_spdx_id(cls, spdx_id: str) -> "LicenseType":
         """
         Create an instance using the SPDX Identifier.
```

### Comparing `ape-etherscan-0.7.3/ape_etherscan.egg-info/PKG-INFO` & `ape-etherscan-0.7.4/ape_etherscan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-etherscan
-Version: 0.7.3
+Version: 0.7.4
 Summary: ape-etherscan: Etherscan Explorer Plugin for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-etherscan
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ape-etherscan-0.7.3/ape_etherscan.egg-info/SOURCES.txt` & `ape-etherscan-0.7.4/ape_etherscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/ape_etherscan.egg-info/requires.txt` & `ape-etherscan-0.7.4/ape_etherscan.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/pyproject.toml` & `ape-etherscan-0.7.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/setup.py` & `ape-etherscan-0.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/tests/conftest.py` & `ape-etherscan-0.7.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/tests/mock_responses/get_account_transactions.json` & `ape-etherscan-0.7.4/tests/mock_responses/get_account_transactions.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/tests/mock_responses/get_account_transactions_with_ctor_args.json` & `ape-etherscan-0.7.4/tests/mock_responses/get_account_transactions_with_ctor_args.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/tests/mock_responses/get_contract_response_flattened.json` & `ape-etherscan-0.7.4/tests/mock_responses/get_contract_response_flattened.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/tests/mock_responses/get_contract_response_json.json` & `ape-etherscan-0.7.4/tests/mock_responses/get_contract_response_json.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/tests/mock_responses/get_contract_response_json_source_code.json` & `ape-etherscan-0.7.4/tests/mock_responses/get_contract_response_json_source_code.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/tests/mock_responses/get_proxy_contract_response.json` & `ape-etherscan-0.7.4/tests/mock_responses/get_proxy_contract_response.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/tests/mock_responses/get_vyper_contract_response.json` & `ape-etherscan-0.7.4/tests/mock_responses/get_vyper_contract_response.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/tests/test_config.py` & `ape-etherscan-0.7.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/tests/test_dependency.py` & `ape-etherscan-0.7.4/tests/test_dependency.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.3/tests/test_etherscan.py` & `ape-etherscan-0.7.4/tests/test_etherscan.py`

 * *Files identical despite different names*

