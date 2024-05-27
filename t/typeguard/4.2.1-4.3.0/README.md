# Comparing `tmp/typeguard-4.2.1.tar.gz` & `tmp/typeguard-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typeguard-4.2.1.tar", last modified: Sun Mar 24 08:05:33 2024, max compression
+gzip compressed data, was "typeguard-4.3.0.tar", last modified: Mon May 27 09:45:22 2024, max compression
```

## Comparing `typeguard-4.2.1.tar` & `typeguard-4.3.0.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 08:05:33.637175 typeguard-4.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 08:05:33.629175 typeguard-4.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 08:05:33.629175 typeguard-4.2.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-03-24 08:05:26.000000 typeguard-4.2.1/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-24 08:05:26.000000 typeguard-4.2.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-24 08:05:26.000000 typeguard-4.2.1/.github/ISSUE_TEMPLATE/features_request.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 08:05:33.629175 typeguard-4.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-03-24 08:05:26.000000 typeguard-4.2.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-24 08:05:26.000000 typeguard-4.2.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-24 08:05:26.000000 typeguard-4.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-03-24 08:05:26.000000 typeguard-4.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-24 08:05:26.000000 typeguard-4.2.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-24 08:05:26.000000 typeguard-4.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-03-24 08:05:33.637175 typeguard-4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-03-24 08:05:26.000000 typeguard-4.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 08:05:33.629175 typeguard-4.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-03-24 08:05:26.000000 typeguard-4.2.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-24 08:05:26.000000 typeguard-4.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-03-24 08:05:26.000000 typeguard-4.2.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-03-24 08:05:26.000000 typeguard-4.2.1/docs/extending.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8131 2024-03-24 08:05:26.000000 typeguard-4.2.1/docs/features.rst
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-24 08:05:26.000000 typeguard-4.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10754 2024-03-24 08:05:26.000000 typeguard-4.2.1/docs/userguide.rst
--rw-r--r--   0 runner    (1001) docker     (127)    23810 2024-03-24 08:05:26.000000 typeguard-4.2.1/docs/versionhistory.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-03-24 08:05:26.000000 typeguard-4.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 08:05:33.637175 typeguard-4.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 08:05:33.629175 typeguard-4.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 08:05:33.633175 typeguard-4.2.1/src/typeguard/
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-03-24 08:05:26.000000 typeguard-4.2.1/src/typeguard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27836 2024-03-24 08:05:26.000000 typeguard-4.2.1/src/typeguard/_checkers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-03-24 08:05:26.000000 typeguard-4.2.1/src/typeguard/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-03-24 08:05:26.000000 typeguard-4.2.1/src/typeguard/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-03-24 08:05:26.000000 typeguard-4.2.1/src/typeguard/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-03-24 08:05:26.000000 typeguard-4.2.1/src/typeguard/_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-03-24 08:05:26.000000 typeguard-4.2.1/src/typeguard/_importhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-03-24 08:05:26.000000 typeguard-4.2.1/src/typeguard/_memo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-03-24 08:05:26.000000 typeguard-4.2.1/src/typeguard/_pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-03-24 08:05:26.000000 typeguard-4.2.1/src/typeguard/_suppression.py
--rw-r--r--   0 runner    (1001) docker     (127)    44937 2024-03-24 08:05:26.000000 typeguard-4.2.1/src/typeguard/_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-24 08:05:26.000000 typeguard-4.2.1/src/typeguard/_union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-03-24 08:05:26.000000 typeguard-4.2.1/src/typeguard/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 08:05:26.000000 typeguard-4.2.1/src/typeguard/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 08:05:33.637175 typeguard-4.2.1/src/typeguard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-03-24 08:05:33.000000 typeguard-4.2.1/src/typeguard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-03-24 08:05:33.000000 typeguard-4.2.1/src/typeguard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 08:05:33.000000 typeguard-4.2.1/src/typeguard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-24 08:05:33.000000 typeguard-4.2.1/src/typeguard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-24 08:05:33.000000 typeguard-4.2.1/src/typeguard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-24 08:05:33.000000 typeguard-4.2.1/src/typeguard.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 08:05:33.637175 typeguard-4.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-24 08:05:26.000000 typeguard-4.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-24 08:05:26.000000 typeguard-4.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6600 2024-03-24 08:05:26.000000 typeguard-4.2.1/tests/dummymodule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 08:05:33.637175 typeguard-4.2.1/tests/mypy/
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-03-24 08:05:26.000000 typeguard-4.2.1/tests/mypy/negative.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-24 08:05:26.000000 typeguard-4.2.1/tests/mypy/positive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-03-24 08:05:26.000000 typeguard-4.2.1/tests/mypy/test_type_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)    35540 2024-03-24 08:05:26.000000 typeguard-4.2.1/tests/test_checkers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-03-24 08:05:26.000000 typeguard-4.2.1/tests/test_importhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-03-24 08:05:26.000000 typeguard-4.2.1/tests/test_instrumentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-24 08:05:26.000000 typeguard-4.2.1/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-03-24 08:05:26.000000 typeguard-4.2.1/tests/test_pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-03-24 08:05:26.000000 typeguard-4.2.1/tests/test_suppression.py
--rw-r--r--   0 runner    (1001) docker     (127)    52530 2024-03-24 08:05:26.000000 typeguard-4.2.1/tests/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17587 2024-03-24 08:05:26.000000 typeguard-4.2.1/tests/test_typechecked.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-03-24 08:05:26.000000 typeguard-4.2.1/tests/test_union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-24 08:05:26.000000 typeguard-4.2.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-24 08:05:26.000000 typeguard-4.2.1/tests/test_warn_on_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:22.585251 typeguard-4.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:22.577251 typeguard-4.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:22.577251 typeguard-4.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-27 09:45:16.000000 typeguard-4.3.0/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-27 09:45:16.000000 typeguard-4.3.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-27 09:45:16.000000 typeguard-4.3.0/.github/ISSUE_TEMPLATE/features_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-27 09:45:16.000000 typeguard-4.3.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:22.577251 typeguard-4.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-27 09:45:16.000000 typeguard-4.3.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-27 09:45:16.000000 typeguard-4.3.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-27 09:45:16.000000 typeguard-4.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-27 09:45:16.000000 typeguard-4.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-27 09:45:16.000000 typeguard-4.3.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-27 09:45:16.000000 typeguard-4.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-27 09:45:22.585251 typeguard-4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-27 09:45:16.000000 typeguard-4.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:22.577251 typeguard-4.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-27 09:45:16.000000 typeguard-4.3.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-27 09:45:16.000000 typeguard-4.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-27 09:45:16.000000 typeguard-4.3.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-27 09:45:16.000000 typeguard-4.3.0/docs/extending.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8731 2024-05-27 09:45:16.000000 typeguard-4.3.0/docs/features.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-27 09:45:16.000000 typeguard-4.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10774 2024-05-27 09:45:16.000000 typeguard-4.3.0/docs/userguide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    24313 2024-05-27 09:45:16.000000 typeguard-4.3.0/docs/versionhistory.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-27 09:45:16.000000 typeguard-4.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 09:45:22.585251 typeguard-4.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:22.573251 typeguard-4.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:22.581251 typeguard-4.3.0/src/typeguard/
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-27 09:45:16.000000 typeguard-4.3.0/src/typeguard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31360 2024-05-27 09:45:16.000000 typeguard-4.3.0/src/typeguard/_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-27 09:45:16.000000 typeguard-4.3.0/src/typeguard/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-05-27 09:45:16.000000 typeguard-4.3.0/src/typeguard/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-27 09:45:16.000000 typeguard-4.3.0/src/typeguard/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-05-27 09:45:16.000000 typeguard-4.3.0/src/typeguard/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-05-27 09:45:16.000000 typeguard-4.3.0/src/typeguard/_importhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-27 09:45:16.000000 typeguard-4.3.0/src/typeguard/_memo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-27 09:45:16.000000 typeguard-4.3.0/src/typeguard/_pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-27 09:45:16.000000 typeguard-4.3.0/src/typeguard/_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44937 2024-05-27 09:45:16.000000 typeguard-4.3.0/src/typeguard/_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-27 09:45:16.000000 typeguard-4.3.0/src/typeguard/_union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-27 09:45:16.000000 typeguard-4.3.0/src/typeguard/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:16.000000 typeguard-4.3.0/src/typeguard/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:22.585251 typeguard-4.3.0/src/typeguard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-27 09:45:22.000000 typeguard-4.3.0/src/typeguard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-27 09:45:22.000000 typeguard-4.3.0/src/typeguard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 09:45:22.000000 typeguard-4.3.0/src/typeguard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-27 09:45:22.000000 typeguard-4.3.0/src/typeguard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-27 09:45:22.000000 typeguard-4.3.0/src/typeguard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 09:45:22.000000 typeguard-4.3.0/src/typeguard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:22.581251 typeguard-4.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-27 09:45:16.000000 typeguard-4.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-27 09:45:16.000000 typeguard-4.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6600 2024-05-27 09:45:16.000000 typeguard-4.3.0/tests/dummymodule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:22.585251 typeguard-4.3.0/tests/mypy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-27 09:45:16.000000 typeguard-4.3.0/tests/mypy/negative.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-27 09:45:16.000000 typeguard-4.3.0/tests/mypy/positive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-27 09:45:16.000000 typeguard-4.3.0/tests/mypy/test_type_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38033 2024-05-27 09:45:16.000000 typeguard-4.3.0/tests/test_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-27 09:45:16.000000 typeguard-4.3.0/tests/test_importhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-05-27 09:45:16.000000 typeguard-4.3.0/tests/test_instrumentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-27 09:45:16.000000 typeguard-4.3.0/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-27 09:45:16.000000 typeguard-4.3.0/tests/test_pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-27 09:45:16.000000 typeguard-4.3.0/tests/test_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52530 2024-05-27 09:45:16.000000 typeguard-4.3.0/tests/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17587 2024-05-27 09:45:16.000000 typeguard-4.3.0/tests/test_typechecked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-27 09:45:16.000000 typeguard-4.3.0/tests/test_union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-27 09:45:16.000000 typeguard-4.3.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-27 09:45:16.000000 typeguard-4.3.0/tests/test_warn_on_error.py
```

### Comparing `typeguard-4.2.1/.github/ISSUE_TEMPLATE/bug_report.yaml` & `typeguard-4.3.0/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/.github/ISSUE_TEMPLATE/features_request.yaml` & `typeguard-4.3.0/.github/ISSUE_TEMPLATE/features_request.yaml`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/.github/workflows/publish.yml` & `typeguard-4.3.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/.github/workflows/test.yml` & `typeguard-4.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/.pre-commit-config.yaml` & `typeguard-4.3.0/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-toml
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [ "--fix=lf" ]
       - id: trailing-whitespace
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.3
+    rev: v0.4.5
     hooks:
       - id: ruff
         args: [--fix, --show-fixes]
-
-  - repo: https://github.com/psf/black
-    rev: 24.3.0
-    hooks:
-      - id: black
-        exclude: "^tests/mypy/negative.py"
+      - id: ruff-format
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
       - id: mypy
         additional_dependencies: [ "typing_extensions" ]
         exclude: "^tests/"
 
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
```

### Comparing `typeguard-4.2.1/LICENSE` & `typeguard-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/PKG-INFO` & `typeguard-4.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeguard
-Version: 4.2.1
+Version: 4.3.0
 Summary: Run-time type checker for Python
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://typeguard.readthedocs.io/en/latest/
 Project-URL: Change log, https://typeguard.readthedocs.io/en/latest/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/typeguard
 Project-URL: Issue tracker, https://github.com/agronholm/typeguard/issues
@@ -18,23 +18,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: importlib_metadata>=3.6; python_version < "3.10"
-Requires-Dist: typing_extensions>=4.10.0; python_version < "3.13"
+Requires-Dist: typing_extensions>=4.10.0
 Provides-Extra: test
 Requires-Dist: coverage[toml]>=7; extra == "test"
 Requires-Dist: pytest>=7; extra == "test"
 Requires-Dist: mypy>=1.2.0; platform_python_implementation != "PyPy" and extra == "test"
 Provides-Extra: doc
 Requires-Dist: packaging; extra == "doc"
 Requires-Dist: Sphinx>=7; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints>=1.2.0; extra == "doc"
+Requires-Dist: sphinx-rtd-theme>=1.3.0; extra == "doc"
 
 .. image:: https://github.com/agronholm/typeguard/actions/workflows/test.yml/badge.svg
   :target: https://github.com/agronholm/typeguard/actions/workflows/test.yml
   :alt: Build Status
 .. image:: https://coveralls.io/repos/agronholm/typeguard/badge.svg?branch=master&service=github
   :target: https://coveralls.io/github/agronholm/typeguard?branch=master
   :alt: Code Coverage
```

### Comparing `typeguard-4.2.1/README.rst` & `typeguard-4.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/docs/api.rst` & `typeguard-4.3.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/docs/conf.py` & `typeguard-4.3.0/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,11 +28,11 @@
 autodoc_type_aliases = {
     "TypeCheckerCallable": "typeguard.TypeCheckerCallable",
     "TypeCheckFailCallback": "typeguard.TypeCheckFailCallback",
     "TypeCheckLookupCallback": "typeguard.TypeCheckLookupCallback",
 }
 todo_include_todos = False
 
-html_theme = "nature"
+html_theme = "sphinx_rtd_theme"
 htmlhelp_basename = "typeguarddoc"
 
 intersphinx_mapping = {"python": ("https://docs.python.org/3/", None)}
```

### Comparing `typeguard-4.2.1/docs/contributing.rst` & `typeguard-4.3.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/docs/extending.rst` & `typeguard-4.3.0/docs/extending.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/docs/features.rst` & `typeguard-4.3.0/docs/features.rst`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 The following type checks are not yet supported in Typeguard:
 
 * Types of values assigned to class or instance variables
 * Types of values assigned to global or nonlocal variables
 * Stubs defined with :func:`@overload <typing.overload>` (the implementation is checked
   if instrumented)
-* ``yield_from`` statements in generator functions
+* ``yield from`` statements in generator functions
 * ``ParamSpec`` and ``Concatenate`` are currently ignored
 * Types where they are shadowed by arguments with the same name (e.g.
   ``def foo(x: type, type: str): ...``)
 
 Other limitations
 -----------------
 
@@ -54,14 +54,28 @@
 instrumentation added, it needs to replace all the references to the original function
 with the new one. This could be impossible when it's placed on top of another decorator
 that wraps the original function. It has no way of telling that other decorator that the
 target function should be switched to a new one. To work around this limitation, either
 place :func:`@typechecked <typechecked>` at the bottom of the decorator stack, or use
 the import hook instead.
 
+Protocol checking
++++++++++++++++++
+
+As of version 4.3.0, Typeguard can check instances and classes against Protocols,
+regardless of whether they were annotated with :decorator:`typing.runtime_checkable`.
+
+There are several limitations on the checks performed, however:
+
+* For non-callable members, only presence is checked for; no type compatibility checks
+  are performed
+* For methods, only the number of positional arguments are checked against, so any added
+  keyword-only arguments without defaults don't currently trip the checker
+* Likewise, argument types are not checked for compatibility
+
 Special considerations for ``if TYPE_CHECKING:``
 ------------------------------------------------
 
 Both the import hook and :func:`@typechecked <typechecked>` avoid checking against
 anything imported in a module-level ``if TYPE_CHECKING:`` (or
 ``if typing.TYPE_CHECKING:``) block, since those types will not be available at run
 time. Therefore, no errors or warnings are emitted for such annotations, even when they
```

### Comparing `typeguard-4.2.1/docs/userguide.rst` & `typeguard-4.3.0/docs/userguide.rst`

 * *Files 1% similar despite different names*

```diff
@@ -144,16 +144,16 @@
 ``if TYPE_CHECKING:`` (add the appropriate :mod:`typing` imports). Imports made within
 such blocks on the module level will be replaced in calls to internal type checking
 functions with :data:`~typing.Any`.
 
 Using the pytest plugin
 -----------------------
 
-Typeguard comes with a pytest plugin that installs the import hook (explained in the
-previous section). To use it, run ``pytest`` with the appropriate
+Typeguard comes with a plugin for pytest (v7.0 or newer) that installs the import hook
+(explained in the previous section). To use it, run ``pytest`` with the appropriate
 ``--typeguard-packages`` option. For example, if you wanted to instrument the
 ``foo.bar`` and ``xyz`` packages for type checking, you can do the following:
 
 .. code-block:: bash
 
     pytest --typeguard-packages=foo.bar,xyz
```

### Comparing `typeguard-4.2.1/docs/versionhistory.rst` & `typeguard-4.3.0/docs/versionhistory.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 Version history
 ===============
 
 This library adheres to
 `Semantic Versioning 2.0 <https://semver.org/#semantic-versioning-200>`_.
 
+**4.3.0** (2024-05-27)
+
+- Added support for checking against static protocols
+- Fixed some compatibility problems when running on Python 3.13
+  (`#460 <https://github.com/agronholm/typeguard/issues/460>`_; PR by @JelleZijlstra)
+- Fixed test suite incompatibility with pytest 8.2
+  (`#461 <https://github.com/agronholm/typeguard/issues/461>`_)
+- Fixed pytest plugin crashing on pytest version older than v7.0.0 (even if it's just
+  present) (`#343 <https://github.com/agronholm/typeguard/issues/343>`_)
+
 **4.2.1** (2023-03-24)
 
 - Fixed missing ``typing_extensions`` dependency for Python 3.12
   (`#444 <https://github.com/agronholm/typeguard/issues/444>`_)
 - Fixed deprecation warning in the test suite on Python 3.13
   (`#444 <https://github.com/agronholm/typeguard/issues/444>`_)
```

### Comparing `typeguard-4.2.1/pyproject.toml` & `typeguard-4.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 requires-python = ">= 3.8"
 dependencies = [
     "importlib_metadata >= 3.6; python_version < '3.10'",
-    "typing_extensions >= 4.10.0; python_version < '3.13'",
+    "typing_extensions >= 4.10.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://typeguard.readthedocs.io/en/latest/"
 "Change log" = "https://typeguard.readthedocs.io/en/latest/versionhistory.html"
 "Source code" = "https://github.com/agronholm/typeguard"
@@ -42,28 +42,29 @@
     "pytest >= 7",
     'mypy >= 1.2.0; python_implementation != "PyPy"',
 ]
 doc = [
     "packaging",
     "Sphinx >= 7",
     "sphinx-autodoc-typehints >= 1.2.0",
+    "sphinx-rtd-theme >= 1.3.0",
 ]
 
 [project.entry-points]
 pytest11 = {typeguard = "typeguard._pytest_plugin"}
 
 [tool.setuptools.package-data]
 typeguard = ["py.typed"]
 
 [tool.setuptools_scm]
 version_scheme = "post-release"
 local_scheme = "dirty-tag"
 
 [tool.pytest.ini_options]
-addopts = "-rsx --tb=short"
+addopts = "--tb=short"
 testpaths = "tests"
 xfail_strict = true
 filterwarnings = ["error"]
 
 [tool.coverage.run]
 source = ["typeguard"]
 
@@ -82,15 +83,15 @@
     "W",            # pycodestyle warnings
     "I",            # isort
     "PGH",          # pygrep-hooks
     "UP",           # pyupgrade
     "B0",           # flake8-bugbear
 ]
 ignore = [
-    "PGH001",
+    "S307",
     "B008",
 ]
 
 [tool.mypy]
 python_version = "3.9"
 strict = true
 pretty = true
```

### Comparing `typeguard-4.2.1/src/typeguard/__init__.py` & `typeguard-4.3.0/src/typeguard/__init__.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/src/typeguard/_checkers.py` & `typeguard-4.3.0/src/typeguard/_checkers.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,30 +28,32 @@
     TextIO,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 from unittest.mock import Mock
+from weakref import WeakKeyDictionary
 
 try:
     import typing_extensions
 except ImportError:
     typing_extensions = None  # type: ignore[assignment]
 
+# Must use this because typing.is_typeddict does not recognize
+# TypedDict from typing_extensions, and as of version 4.12.0
+# typing_extensions.TypedDict is different from typing.TypedDict
+# on all versions.
+from typing_extensions import is_typeddict
+
 from ._config import ForwardRefPolicy
 from ._exceptions import TypeCheckError, TypeHintWarning
 from ._memo import TypeCheckMemo
 from ._utils import evaluate_forwardref, get_stacklevel, get_type_name, qualified_name
 
-if sys.version_info >= (3, 13):
-    from typing import is_typeddict
-else:
-    from typing_extensions import is_typeddict
-
 if sys.version_info >= (3, 11):
     from typing import (
         Annotated,
         NotRequired,
         TypeAlias,
         get_args,
         get_origin,
@@ -83,14 +85,17 @@
 ]
 
 checker_lookup_functions: list[TypeCheckLookupCallback] = []
 generic_alias_types: tuple[type, ...] = (type(List), type(List[Any]))
 if sys.version_info >= (3, 9):
     generic_alias_types += (types.GenericAlias,)
 
+protocol_check_cache: WeakKeyDictionary[
+    type[Any], dict[type[Any], TypeCheckError | None]
+] = WeakKeyDictionary()
 
 # Sentinel
 _missing = object()
 
 # Lifted from mypy.sharedparse
 BINARY_MAGIC_METHODS = {
     "__add__",
@@ -645,27 +650,104 @@
 
 def check_protocol(
     value: Any,
     origin_type: Any,
     args: tuple[Any, ...],
     memo: TypeCheckMemo,
 ) -> None:
-    # TODO: implement proper compatibility checking and support non-runtime protocols
-    if getattr(origin_type, "_is_runtime_protocol", False):
-        if not isinstance(value, origin_type):
-            raise TypeCheckError(
-                f"is not compatible with the {origin_type.__qualname__} protocol"
+    subject: type[Any] = value if isclass(value) else type(value)
+
+    if subject in protocol_check_cache:
+        result_map = protocol_check_cache[subject]
+        if origin_type in result_map:
+            if exc := result_map[origin_type]:
+                raise exc
+            else:
+                return
+
+    # Collect a set of methods and non-method attributes present in the protocol
+    ignored_attrs = set(dir(typing.Protocol)) | {
+        "__annotations__",
+        "__non_callable_proto_members__",
+    }
+    expected_methods: dict[str, tuple[Any, Any]] = {}
+    expected_noncallable_members: dict[str, Any] = {}
+    for attrname in dir(origin_type):
+        # Skip attributes present in typing.Protocol
+        if attrname in ignored_attrs:
+            continue
+
+        member = getattr(origin_type, attrname)
+        if callable(member):
+            signature = inspect.signature(member)
+            argtypes = [
+                (p.annotation if p.annotation is not Parameter.empty else Any)
+                for p in signature.parameters.values()
+                if p.kind is not Parameter.KEYWORD_ONLY
+            ] or Ellipsis
+            return_annotation = (
+                signature.return_annotation
+                if signature.return_annotation is not Parameter.empty
+                else Any
             )
+            expected_methods[attrname] = argtypes, return_annotation
+        else:
+            expected_noncallable_members[attrname] = member
+
+    for attrname, annotation in typing.get_type_hints(origin_type).items():
+        expected_noncallable_members[attrname] = annotation
+
+    subject_annotations = typing.get_type_hints(subject)
+
+    # Check that all required methods are present and their signatures are compatible
+    result_map = protocol_check_cache.setdefault(subject, {})
+    try:
+        for attrname, callable_args in expected_methods.items():
+            try:
+                method = getattr(subject, attrname)
+            except AttributeError:
+                if attrname in subject_annotations:
+                    raise TypeCheckError(
+                        f"is not compatible with the {origin_type.__qualname__} protocol "
+                        f"because its {attrname!r} attribute is not a method"
+                    ) from None
+                else:
+                    raise TypeCheckError(
+                        f"is not compatible with the {origin_type.__qualname__} protocol "
+                        f"because it has no method named {attrname!r}"
+                    ) from None
+
+            if not callable(method):
+                raise TypeCheckError(
+                    f"is not compatible with the {origin_type.__qualname__} protocol "
+                    f"because its {attrname!r} attribute is not a callable"
+                )
+
+            # TODO: raise exception on added keyword-only arguments without defaults
+            try:
+                check_callable(method, Callable, callable_args, memo)
+            except TypeCheckError as exc:
+                raise TypeCheckError(
+                    f"is not compatible with the {origin_type.__qualname__} protocol "
+                    f"because its {attrname!r} method {exc}"
+                ) from None
+
+        # Check that all required non-callable members are present
+        for attrname in expected_noncallable_members:
+            # TODO: implement assignability checks for non-callable members
+            if attrname not in subject_annotations and not hasattr(subject, attrname):
+                raise TypeCheckError(
+                    f"is not compatible with the {origin_type.__qualname__} protocol "
+                    f"because it has no attribute named {attrname!r}"
+                )
+    except TypeCheckError as exc:
+        result_map[origin_type] = exc
+        raise
     else:
-        warnings.warn(
-            f"Typeguard cannot check the {origin_type.__qualname__} protocol because "
-            f"it is a non-runtime protocol. If you would like to type check this "
-            f"protocol, please use @typing.runtime_checkable",
-            stacklevel=get_stacklevel(),
-        )
+        result_map[origin_type] = None
 
 
 def check_byteslike(
     value: Any,
     origin_type: Any,
     args: tuple[Any, ...],
     memo: TypeCheckMemo,
@@ -848,15 +930,16 @@
 ) -> TypeCheckerCallable | None:
     checker = origin_type_checkers.get(origin_type)
     if checker is not None:
         return checker
     elif is_typeddict(origin_type):
         return check_typed_dict
     elif isclass(origin_type) and issubclass(
-        origin_type, Tuple  # type: ignore[arg-type]
+        origin_type,
+        Tuple,  # type: ignore[arg-type]
     ):
         # NamedTuple
         return check_tuple
     elif getattr(origin_type, "_is_protocol", False):
         return check_protocol
     elif isinstance(origin_type, ParamSpec):
         return check_paramspec
```

### Comparing `typeguard-4.2.1/src/typeguard/_config.py` & `typeguard-4.3.0/src/typeguard/_config.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/src/typeguard/_decorators.py` & `typeguard-4.3.0/src/typeguard/_decorators.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/src/typeguard/_exceptions.py` & `typeguard-4.3.0/src/typeguard/_exceptions.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/src/typeguard/_functions.py` & `typeguard-4.3.0/src/typeguard/_functions.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/src/typeguard/_importhook.py` & `typeguard-4.3.0/src/typeguard/_importhook.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/src/typeguard/_memo.py` & `typeguard-4.3.0/src/typeguard/_memo.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/src/typeguard/_pytest_plugin.py` & `typeguard-4.3.0/src/typeguard/_pytest_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from __future__ import annotations
 
 import sys
 import warnings
-from typing import Any, Literal
-
-from pytest import Config, Parser
+from typing import TYPE_CHECKING, Any, Literal
 
 from typeguard._config import CollectionCheckStrategy, ForwardRefPolicy, global_config
 from typeguard._exceptions import InstrumentationWarning
 from typeguard._importhook import install_import_hook
 from typeguard._utils import qualified_name, resolve_reference
 
+if TYPE_CHECKING:
+    from pytest import Config, Parser
+
 
 def pytest_addoption(parser: Parser) -> None:
     def add_ini_option(
         opt_type: (
             Literal["string", "paths", "pathlist", "args", "linelist", "bool"] | None
-        )
+        ),
     ) -> None:
         parser.addini(
             group.options[-1].names()[0][2:],
             group.options[-1].attrs()["help"],
             opt_type,
         )
```

### Comparing `typeguard-4.2.1/src/typeguard/_suppression.py` & `typeguard-4.3.0/src/typeguard/_suppression.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 @overload
 def suppress_type_checks() -> ContextManager[None]: ...
 
 
 def suppress_type_checks(
-    func: Callable[P, T] | None = None
+    func: Callable[P, T] | None = None,
 ) -> Callable[P, T] | ContextManager[None]:
     """
     Temporarily suppress all type checking.
 
     This function has two operating modes, based on how it's used:
 
     #. as a context manager (``with suppress_type_checks(): ...``)
```

### Comparing `typeguard-4.2.1/src/typeguard/_transformer.py` & `typeguard-4.3.0/src/typeguard/_transformer.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/src/typeguard/_union_transformer.py` & `typeguard-4.3.0/src/typeguard/_union_transformer.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/src/typeguard/_utils.py` & `typeguard-4.3.0/src/typeguard/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,19 +7,29 @@
 from types import CodeType, FrameType, FunctionType
 from typing import TYPE_CHECKING, Any, Callable, ForwardRef, Union, cast, final
 from weakref import WeakValueDictionary
 
 if TYPE_CHECKING:
     from ._memo import TypeCheckMemo
 
-if sys.version_info >= (3, 10):
+if sys.version_info >= (3, 13):
     from typing import get_args, get_origin
 
     def evaluate_forwardref(forwardref: ForwardRef, memo: TypeCheckMemo) -> Any:
-        return forwardref._evaluate(memo.globals, memo.locals, frozenset())
+        return forwardref._evaluate(
+            memo.globals, memo.locals, type_params=(), recursive_guard=frozenset()
+        )
+
+elif sys.version_info >= (3, 10):
+    from typing import get_args, get_origin
+
+    def evaluate_forwardref(forwardref: ForwardRef, memo: TypeCheckMemo) -> Any:
+        return forwardref._evaluate(
+            memo.globals, memo.locals, recursive_guard=frozenset()
+        )
 
 else:
     from typing_extensions import get_args, get_origin
 
     evaluate_extra_args: tuple[frozenset[Any], ...] = (
         (frozenset(),) if sys.version_info >= (3, 9) else ()
     )
```

### Comparing `typeguard-4.2.1/src/typeguard.egg-info/PKG-INFO` & `typeguard-4.3.0/src/typeguard.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeguard
-Version: 4.2.1
+Version: 4.3.0
 Summary: Run-time type checker for Python
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://typeguard.readthedocs.io/en/latest/
 Project-URL: Change log, https://typeguard.readthedocs.io/en/latest/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/typeguard
 Project-URL: Issue tracker, https://github.com/agronholm/typeguard/issues
@@ -18,23 +18,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: importlib_metadata>=3.6; python_version < "3.10"
-Requires-Dist: typing_extensions>=4.10.0; python_version < "3.13"
+Requires-Dist: typing_extensions>=4.10.0
 Provides-Extra: test
 Requires-Dist: coverage[toml]>=7; extra == "test"
 Requires-Dist: pytest>=7; extra == "test"
 Requires-Dist: mypy>=1.2.0; platform_python_implementation != "PyPy" and extra == "test"
 Provides-Extra: doc
 Requires-Dist: packaging; extra == "doc"
 Requires-Dist: Sphinx>=7; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints>=1.2.0; extra == "doc"
+Requires-Dist: sphinx-rtd-theme>=1.3.0; extra == "doc"
 
 .. image:: https://github.com/agronholm/typeguard/actions/workflows/test.yml/badge.svg
   :target: https://github.com/agronholm/typeguard/actions/workflows/test.yml
   :alt: Build Status
 .. image:: https://coveralls.io/repos/agronholm/typeguard/badge.svg?branch=master&service=github
   :target: https://coveralls.io/github/agronholm/typeguard?branch=master
   :alt: Code Coverage
```

### Comparing `typeguard-4.2.1/src/typeguard.egg-info/SOURCES.txt` & `typeguard-4.3.0/src/typeguard.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
 LICENSE
 README.rst
 pyproject.toml
+.github/pull_request_template.md
 .github/ISSUE_TEMPLATE/bug_report.yaml
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/features_request.yaml
 .github/workflows/publish.yml
 .github/workflows/test.yml
 docs/api.rst
 docs/conf.py
```

### Comparing `typeguard-4.2.1/tests/__init__.py` & `typeguard-4.3.0/tests/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -43,15 +43,17 @@
 
 class Child(Parent):
     def method(self, a: int) -> None:
         pass
 
 
 class StaticProtocol(Protocol):
-    def meth(self) -> None: ...
+    member: int
+
+    def meth(self, x: str) -> None: ...
 
 
 @runtime_checkable
 class RuntimeProtocol(Protocol):
     member: int
 
-    def meth(self) -> None: ...
+    def meth(self, x: str) -> None: ...
```

### Comparing `typeguard-4.2.1/tests/conftest.py` & `typeguard-4.3.0/tests/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import random
 import re
 import string
 import sys
 import typing
 from itertools import count
+from pathlib import Path
 
 import pytest
 import typing_extensions
 
 version_re = re.compile(r"_py(\d)(\d)\.py$")
 pytest_plugins = ["pytester"]
 
 
-def pytest_ignore_collect(path, config):
-    match = version_re.search(path.basename)
+def pytest_ignore_collect(collection_path: Path, config: pytest.Config) -> bool:
+    match = version_re.search(collection_path.name)
     if match:
         version = tuple(int(x) for x in match.groups())
         if sys.version_info < version:
             return True
 
+    return False
+
 
 @pytest.fixture
 def sample_set() -> set:
     # Create a set which, when iterated, returns "bb" as the first item
     for num in count():
         letter = random.choice(string.ascii_lowercase)
         dummy_set = {letter, num}
```

### Comparing `typeguard-4.2.1/tests/dummymodule.py` & `typeguard-4.3.0/tests/dummymodule.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/tests/mypy/negative.py` & `typeguard-4.3.0/tests/mypy/negative.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/tests/mypy/positive.py` & `typeguard-4.3.0/tests/mypy/positive.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/tests/mypy/test_type_annotations.py` & `typeguard-4.3.0/tests/mypy/test_type_annotations.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/tests/test_checkers.py` & `typeguard-4.3.0/tests/test_checkers.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     TypeCheckError,
     TypeCheckMemo,
     TypeHintWarning,
     check_type,
     check_type_internal,
     suppress_type_checks,
 )
+from typeguard._checkers import is_typeddict
 from typeguard._utils import qualified_name
 
 from . import (
     Child,
     Employee,
     JSONType,
     Parent,
@@ -526,14 +527,22 @@
             y: "NotRequired[int]"
 
         with pytest.raises(
             TypeCheckError, match=r"value of key 'y' of dict is not an instance of int"
         ):
             check_type({"x": 1, "y": "foo"}, DummyDict)
 
+    def test_is_typeddict(self, typing_provider):
+        # Ensure both typing.TypedDict and typing_extensions.TypedDict are recognized
+        class DummyDict(typing_provider.TypedDict):
+            x: int
+
+        assert is_typeddict(DummyDict)
+        assert not is_typeddict(dict)
+
 
 class TestList:
     def test_bad_type(self):
         pytest.raises(TypeCheckError, check_type, 5, List[int]).match(
             "int is not a list"
         )
 
@@ -982,74 +991,127 @@
         )
 
     def test_text_real_file(self, tmp_path: Path):
         with tmp_path.joinpath("testfile").open("w") as f:
             check_type(f, TextIO)
 
 
+@pytest.mark.parametrize(
+    "instantiate, annotation",
+    [
+        pytest.param(True, RuntimeProtocol, id="instance_runtime"),
+        pytest.param(False, Type[RuntimeProtocol], id="class_runtime"),
+        pytest.param(True, StaticProtocol, id="instance_static"),
+        pytest.param(False, Type[StaticProtocol], id="class_static"),
+    ],
+)
 class TestProtocol:
-    def test_protocol(self):
+    def test_member_defaultval(self, instantiate, annotation):
         class Foo:
             member = 1
 
-            def meth(self) -> None:
+            def meth(self, x: str) -> None:
                 pass
 
-        check_type(Foo(), RuntimeProtocol)
-        check_type(Foo, Type[RuntimeProtocol])
+        subject = Foo() if instantiate else Foo
+        for _ in range(2):  # Makes sure that the cache is also exercised
+            check_type(subject, annotation)
 
-    def test_protocol_warns_on_static(self):
+    def test_member_annotation(self, instantiate, annotation):
         class Foo:
-            member = 1
+            member: int
 
-            def meth(self) -> None:
+            def meth(self, x: str) -> None:
                 pass
 
-        with pytest.warns(
-            UserWarning, match=r"Typeguard cannot check the StaticProtocol protocol.*"
-        ) as warning:
-            check_type(Foo(), StaticProtocol)
+        subject = Foo() if instantiate else Foo
+        for _ in range(2):
+            check_type(subject, annotation)
 
-        assert warning.list[0].filename == __file__
+    def test_attribute_missing(self, instantiate, annotation):
+        class Foo:
+            val = 1
 
-        with pytest.warns(
-            UserWarning, match=r"Typeguard cannot check the StaticProtocol protocol.*"
-        ) as warning:
-            check_type(Foo, Type[StaticProtocol])
+            def meth(self, x: str) -> None:
+                pass
 
-        assert warning.list[0].filename == __file__
+        clsname = f"{__name__}.TestProtocol.test_attribute_missing.<locals>.Foo"
+        subject = Foo() if instantiate else Foo
+        for _ in range(2):
+            pytest.raises(TypeCheckError, check_type, subject, annotation).match(
+                f"{clsname} is not compatible with the (Runtime|Static)Protocol "
+                f"protocol because it has no attribute named 'member'"
+            )
 
-    def test_fail_non_method_members(self):
+    def test_method_missing(self, instantiate, annotation):
         class Foo:
-            val = 1
+            member: int
 
-            def meth(self) -> None:
-                pass
+        pattern = (
+            f"{__name__}.TestProtocol.test_method_missing.<locals>.Foo is not "
+            f"compatible with the (Runtime|Static)Protocol protocol because it has no "
+            f"method named 'meth'"
+        )
+        subject = Foo() if instantiate else Foo
+        for _ in range(2):
+            pytest.raises(TypeCheckError, check_type, subject, annotation).match(
+                pattern
+            )
 
-        clsname = f"{__name__}.TestProtocol.test_fail_non_method_members.<locals>.Foo"
-        pytest.raises(TypeCheckError, check_type, Foo(), RuntimeProtocol).match(
-            f"{clsname} is not compatible with the RuntimeProtocol protocol"
-        )
-        pytest.raises(TypeCheckError, check_type, Foo, Type[RuntimeProtocol]).match(
-            f"class {clsname} is not compatible with the RuntimeProtocol protocol"
-        )
+    def test_attribute_is_not_method_1(self, instantiate, annotation):
+        class Foo:
+            member: int
+            meth: str
 
-    def test_fail(self):
+        pattern = (
+            f"{__name__}.TestProtocol.test_attribute_is_not_method_1.<locals>.Foo is "
+            f"not compatible with the (Runtime|Static)Protocol protocol because its "
+            f"'meth' attribute is not a method"
+        )
+        subject = Foo() if instantiate else Foo
+        for _ in range(2):
+            pytest.raises(TypeCheckError, check_type, subject, annotation).match(
+                pattern
+            )
+
+    def test_attribute_is_not_method_2(self, instantiate, annotation):
         class Foo:
-            def meth2(self) -> None:
+            member: int
+            meth = "foo"
+
+        pattern = (
+            f"{__name__}.TestProtocol.test_attribute_is_not_method_2.<locals>.Foo is "
+            f"not compatible with the (Runtime|Static)Protocol protocol because its "
+            f"'meth' attribute is not a callable"
+        )
+        subject = Foo() if instantiate else Foo
+        for _ in range(2):
+            pytest.raises(TypeCheckError, check_type, subject, annotation).match(
+                pattern
+            )
+
+    def test_method_signature_mismatch(self, instantiate, annotation):
+        class Foo:
+            member: int
+
+            def meth(self, x: str, y: int) -> None:
                 pass
 
         pattern = (
-            f"{__name__}.TestProtocol.test_fail.<locals>.Foo is not compatible with "
-            f"the RuntimeProtocol protocol"
-        )
-        pytest.raises(TypeCheckError, check_type, Foo(), RuntimeProtocol).match(pattern)
-        pytest.raises(TypeCheckError, check_type, Foo, Type[RuntimeProtocol]).match(
-            pattern
-        )
+            rf"(class )?{__name__}.TestProtocol.test_method_signature_mismatch."
+            rf"<locals>.Foo is not compatible with the (Runtime|Static)Protocol "
+            rf"protocol because its 'meth' method has too many mandatory positional "
+            rf"arguments in its declaration; expected 2 but 3 mandatory positional "
+            rf"argument\(s\) declared"
+        )
+        subject = Foo() if instantiate else Foo
+        for _ in range(2):
+            pytest.raises(TypeCheckError, check_type, subject, annotation).match(
+                pattern
+            )
 
 
 class TestRecursiveType:
     def test_valid(self):
         check_type({"a": [1, 2, 3]}, JSONType)
 
     def test_fail(self):
```

### Comparing `typeguard-4.2.1/tests/test_importhook.py` & `typeguard-4.3.0/tests/test_importhook.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/tests/test_instrumentation.py` & `typeguard-4.3.0/tests/test_instrumentation.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/tests/test_plugins.py` & `typeguard-4.3.0/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/tests/test_pytest_plugin.py` & `typeguard-4.3.0/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/tests/test_suppression.py` & `typeguard-4.3.0/tests/test_suppression.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/tests/test_transformer.py` & `typeguard-4.3.0/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/tests/test_typechecked.py` & `typeguard-4.3.0/tests/test_typechecked.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/tests/test_union_transformer.py` & `typeguard-4.3.0/tests/test_union_transformer.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/tests/test_utils.py` & `typeguard-4.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.2.1/tests/test_warn_on_error.py` & `typeguard-4.3.0/tests/test_warn_on_error.py`

 * *Files identical despite different names*

