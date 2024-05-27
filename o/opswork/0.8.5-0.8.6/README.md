# Comparing `tmp/opswork-0.8.5.tar.gz` & `tmp/opswork-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opswork-0.8.5.tar", last modified: Thu May 16 21:55:50 2024, max compression
+gzip compressed data, was "opswork-0.8.6.tar", last modified: Mon May 27 20:35:58 2024, max compression
```

## Comparing `opswork-0.8.5.tar` & `opswork-0.8.6.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:55:50.240687 opswork-0.8.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:55:50.232687 opswork-0.8.5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-16 21:55:17.000000 opswork-0.8.5/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-16 21:55:17.000000 opswork-0.8.5/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:55:50.232687 opswork-0.8.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-16 21:55:17.000000 opswork-0.8.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-16 21:55:17.000000 opswork-0.8.5/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:55:50.232687 opswork-0.8.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-16 21:55:17.000000 opswork-0.8.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-16 21:55:17.000000 opswork-0.8.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-16 21:55:17.000000 opswork-0.8.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-16 21:55:17.000000 opswork-0.8.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-16 21:55:17.000000 opswork-0.8.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-16 21:55:17.000000 opswork-0.8.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-16 21:55:17.000000 opswork-0.8.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-16 21:55:17.000000 opswork-0.8.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-16 21:55:17.000000 opswork-0.8.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-16 21:55:50.240687 opswork-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-16 21:55:17.000000 opswork-0.8.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-16 21:55:17.000000 opswork-0.8.5/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:55:50.236687 opswork-0.8.5/cache/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 21:55:17.000000 opswork-0.8.5/cache/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-16 21:55:17.000000 opswork-0.8.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:55:50.228687 opswork-0.8.5/recipe/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:55:50.236687 opswork-0.8.5/recipe/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-16 21:55:17.000000 opswork-0.8.5/recipe/cmd/recipe.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:55:50.236687 opswork-0.8.5/recipe/motd/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-16 21:55:17.000000 opswork-0.8.5/recipe/motd/motd.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-16 21:55:17.000000 opswork-0.8.5/recipe/motd/recipe.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:55:50.236687 opswork-0.8.5/recipe/nginx/
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-16 21:55:17.000000 opswork-0.8.5/recipe/nginx/recipe.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:55:50.236687 opswork-0.8.5/recipe/ping/
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-16 21:55:17.000000 opswork-0.8.5/recipe/ping/recipe.yml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-16 21:55:17.000000 opswork-0.8.5/renovate.json
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-16 21:55:50.240687 opswork-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-16 21:55:17.000000 opswork-0.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:55:50.228687 opswork-0.8.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:55:50.236687 opswork-0.8.5/src/opswork/
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-16 21:55:17.000000 opswork-0.8.5/src/opswork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8384 2024-05-16 21:55:17.000000 opswork-0.8.5/src/opswork/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:55:50.236687 opswork-0.8.5/src/opswork/command/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-16 21:55:17.000000 opswork-0.8.5/src/opswork/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-05-16 21:55:17.000000 opswork-0.8.5/src/opswork/command/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-05-16 21:55:17.000000 opswork-0.8.5/src/opswork/command/hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-16 21:55:17.000000 opswork-0.8.5/src/opswork/command/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-05-16 21:55:17.000000 opswork-0.8.5/src/opswork/command/recipes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-16 21:55:17.000000 opswork-0.8.5/src/opswork/command/secret.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:55:50.236687 opswork-0.8.5/src/opswork/exception/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-16 21:55:17.000000 opswork-0.8.5/src/opswork/exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:55:50.240687 opswork-0.8.5/src/opswork/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-16 21:55:17.000000 opswork-0.8.5/src/opswork/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-16 21:55:17.000000 opswork-0.8.5/src/opswork/model/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-16 21:55:17.000000 opswork-0.8.5/src/opswork/model/recipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-16 21:55:17.000000 opswork-0.8.5/src/opswork/model/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-16 21:55:17.000000 opswork-0.8.5/src/opswork/model/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:55:50.240687 opswork-0.8.5/src/opswork/module/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-16 21:55:17.000000 opswork-0.8.5/src/opswork/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-16 21:55:17.000000 opswork-0.8.5/src/opswork/module/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9239 2024-05-16 21:55:17.000000 opswork-0.8.5/src/opswork/module/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-16 21:55:17.000000 opswork-0.8.5/src/opswork/module/encrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-16 21:55:17.000000 opswork-0.8.5/src/opswork/module/file_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-16 21:55:17.000000 opswork-0.8.5/src/opswork/module/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-16 21:55:17.000000 opswork-0.8.5/src/opswork/module/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-05-16 21:55:17.000000 opswork-0.8.5/src/opswork/module/playbook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:55:50.240687 opswork-0.8.5/src/opswork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-16 21:55:50.000000 opswork-0.8.5/src/opswork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-16 21:55:50.000000 opswork-0.8.5/src/opswork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 21:55:50.000000 opswork-0.8.5/src/opswork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-16 21:55:50.000000 opswork-0.8.5/src/opswork.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 21:55:50.000000 opswork-0.8.5/src/opswork.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-16 21:55:50.000000 opswork-0.8.5/src/opswork.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 21:55:50.000000 opswork-0.8.5/src/opswork.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:55:50.240687 opswork-0.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-16 21:55:17.000000 opswork-0.8.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:55:50.240687 opswork-0.8.5/tests/module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:55:17.000000 opswork-0.8.5/tests/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-16 21:55:17.000000 opswork-0.8.5/tests/module/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-16 21:55:17.000000 opswork-0.8.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:58.823549 opswork-0.8.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:58.815549 opswork-0.8.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-27 20:35:44.000000 opswork-0.8.6/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-27 20:35:44.000000 opswork-0.8.6/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:58.815549 opswork-0.8.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-27 20:35:44.000000 opswork-0.8.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-27 20:35:44.000000 opswork-0.8.6/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:58.819549 opswork-0.8.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-27 20:35:44.000000 opswork-0.8.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-27 20:35:44.000000 opswork-0.8.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-27 20:35:44.000000 opswork-0.8.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-27 20:35:44.000000 opswork-0.8.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-27 20:35:44.000000 opswork-0.8.6/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-27 20:35:44.000000 opswork-0.8.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-27 20:35:44.000000 opswork-0.8.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-27 20:35:44.000000 opswork-0.8.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-27 20:35:44.000000 opswork-0.8.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-27 20:35:58.823549 opswork-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-27 20:35:44.000000 opswork-0.8.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-27 20:35:44.000000 opswork-0.8.6/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:58.819549 opswork-0.8.6/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 20:35:44.000000 opswork-0.8.6/cache/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-27 20:35:44.000000 opswork-0.8.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:58.811549 opswork-0.8.6/recipe/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:58.819549 opswork-0.8.6/recipe/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-27 20:35:44.000000 opswork-0.8.6/recipe/cmd/recipe.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:58.819549 opswork-0.8.6/recipe/motd/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-27 20:35:44.000000 opswork-0.8.6/recipe/motd/motd.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-27 20:35:44.000000 opswork-0.8.6/recipe/motd/recipe.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:58.819549 opswork-0.8.6/recipe/nginx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-27 20:35:44.000000 opswork-0.8.6/recipe/nginx/recipe.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:58.819549 opswork-0.8.6/recipe/ping/
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-27 20:35:44.000000 opswork-0.8.6/recipe/ping/recipe.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-27 20:35:44.000000 opswork-0.8.6/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-27 20:35:58.823549 opswork-0.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-27 20:35:44.000000 opswork-0.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:58.811549 opswork-0.8.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:58.819549 opswork-0.8.6/src/opswork/
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-27 20:35:44.000000 opswork-0.8.6/src/opswork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8384 2024-05-27 20:35:44.000000 opswork-0.8.6/src/opswork/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:58.819549 opswork-0.8.6/src/opswork/command/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-27 20:35:44.000000 opswork-0.8.6/src/opswork/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-05-27 20:35:44.000000 opswork-0.8.6/src/opswork/command/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-05-27 20:35:44.000000 opswork-0.8.6/src/opswork/command/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-27 20:35:44.000000 opswork-0.8.6/src/opswork/command/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-05-27 20:35:44.000000 opswork-0.8.6/src/opswork/command/recipes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-27 20:35:44.000000 opswork-0.8.6/src/opswork/command/secret.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:58.819549 opswork-0.8.6/src/opswork/exception/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-27 20:35:44.000000 opswork-0.8.6/src/opswork/exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:58.823549 opswork-0.8.6/src/opswork/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-27 20:35:44.000000 opswork-0.8.6/src/opswork/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-27 20:35:44.000000 opswork-0.8.6/src/opswork/model/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-27 20:35:44.000000 opswork-0.8.6/src/opswork/model/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-27 20:35:44.000000 opswork-0.8.6/src/opswork/model/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-27 20:35:44.000000 opswork-0.8.6/src/opswork/model/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:58.823549 opswork-0.8.6/src/opswork/module/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-27 20:35:44.000000 opswork-0.8.6/src/opswork/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-27 20:35:44.000000 opswork-0.8.6/src/opswork/module/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9239 2024-05-27 20:35:44.000000 opswork-0.8.6/src/opswork/module/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-27 20:35:44.000000 opswork-0.8.6/src/opswork/module/encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-27 20:35:44.000000 opswork-0.8.6/src/opswork/module/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-27 20:35:44.000000 opswork-0.8.6/src/opswork/module/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-27 20:35:44.000000 opswork-0.8.6/src/opswork/module/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-05-27 20:35:44.000000 opswork-0.8.6/src/opswork/module/playbook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:58.823549 opswork-0.8.6/src/opswork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-27 20:35:58.000000 opswork-0.8.6/src/opswork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-27 20:35:58.000000 opswork-0.8.6/src/opswork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:35:58.000000 opswork-0.8.6/src/opswork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-27 20:35:58.000000 opswork-0.8.6/src/opswork.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:35:58.000000 opswork-0.8.6/src/opswork.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-27 20:35:58.000000 opswork-0.8.6/src/opswork.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 20:35:58.000000 opswork-0.8.6/src/opswork.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:58.823549 opswork-0.8.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-27 20:35:44.000000 opswork-0.8.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:58.823549 opswork-0.8.6/tests/module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:44.000000 opswork-0.8.6/tests/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-27 20:35:44.000000 opswork-0.8.6/tests/module/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-27 20:35:44.000000 opswork-0.8.6/tox.ini
```

### Comparing `opswork-0.8.5/.github/workflows/release.yml` & `opswork-0.8.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/.gitignore` & `opswork-0.8.6/.gitignore`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/CHANGELOG.rst` & `opswork-0.8.6/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/CODE_OF_CONDUCT.md` & `opswork-0.8.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/CONTRIBUTING.rst` & `opswork-0.8.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/LICENSE.txt` & `opswork-0.8.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/Makefile` & `opswork-0.8.6/Makefile`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/PKG-INFO` & `opswork-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opswork
-Version: 0.8.5
+Version: 0.8.6
 Summary: OpsWork Swiss Knife.
 Home-page: https://github.com/Clivern/OpsWork/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/Clivern/OpsWork/
 Project-URL: Source, https://github.com/Clivern/OpsWork/
@@ -19,15 +19,15 @@
 License-File: LICENSE.txt
 Requires-Dist: click<=8.1.7
 Requires-Dist: ansible-runner<=2.4.0
 Requires-Dist: prettytable<=3.10.0
 Requires-Dist: PyYAML<=6.0.1
 Requires-Dist: cryptography<=42.0.7
 Requires-Dist: GitPython<=3.1.43
-Requires-Dist: requests<=2.31.0
+Requires-Dist: requests<=2.32.2
 Requires-Dist: importlib-metadata<=7.1.0; python_version < "3.8"
 
 .. image:: https://img.shields.io/pypi/v/opswork.svg
     :alt: PyPI-Server
     :target: https://pypi.org/project/opswork/
 .. image:: https://github.com/clivern/opswork/actions/workflows/ci.yml/badge.svg
     :alt: Build Status
```

### Comparing `opswork-0.8.5/README.rst` & `opswork-0.8.6/README.rst`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/SECURITY.md` & `opswork-0.8.6/SECURITY.md`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/recipe/cmd/recipe.yml` & `opswork-0.8.6/recipe/cmd/recipe.yml`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/recipe/motd/recipe.yml` & `opswork-0.8.6/recipe/motd/recipe.yml`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/recipe/nginx/recipe.yml` & `opswork-0.8.6/recipe/nginx/recipe.yml`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/recipe/ping/recipe.yml` & `opswork-0.8.6/recipe/ping/recipe.yml`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/setup.cfg` & `opswork-0.8.6/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 install_requires = 
 	click<=8.1.7
 	ansible-runner<=2.4.0
 	prettytable<=3.10.0
 	PyYAML<=6.0.1
 	cryptography<=42.0.7
 	GitPython<=3.1.43
-	requests<=2.31.0
+	requests<=2.32.2
 	importlib-metadata<=7.1.0; python_version<"3.8"
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 	recipe
```

### Comparing `opswork-0.8.5/setup.py` & `opswork-0.8.6/setup.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/src/opswork/__init__.py` & `opswork-0.8.6/src/opswork/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/src/opswork/cli.py` & `opswork-0.8.6/src/opswork/cli.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/src/opswork/command/__init__.py` & `opswork-0.8.6/src/opswork/command/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/src/opswork/command/configs.py` & `opswork-0.8.6/src/opswork/command/configs.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/src/opswork/command/hosts.py` & `opswork-0.8.6/src/opswork/command/hosts.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/src/opswork/command/random.py` & `opswork-0.8.6/src/opswork/command/random.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/src/opswork/command/recipes.py` & `opswork-0.8.6/src/opswork/command/recipes.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/src/opswork/command/secret.py` & `opswork-0.8.6/src/opswork/command/secret.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/src/opswork/exception/__init__.py` & `opswork-0.8.6/src/opswork/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/src/opswork/model/__init__.py` & `opswork-0.8.6/src/opswork/model/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/src/opswork/model/host.py` & `opswork-0.8.6/src/opswork/model/host.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/src/opswork/model/recipe.py` & `opswork-0.8.6/src/opswork/model/recipe.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/src/opswork/model/secret.py` & `opswork-0.8.6/src/opswork/model/secret.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/src/opswork/model/task.py` & `opswork-0.8.6/src/opswork/model/task.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/src/opswork/module/__init__.py` & `opswork-0.8.6/src/opswork/module/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/src/opswork/module/config.py` & `opswork-0.8.6/src/opswork/module/config.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/src/opswork/module/database.py` & `opswork-0.8.6/src/opswork/module/database.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/src/opswork/module/encrypt.py` & `opswork-0.8.6/src/opswork/module/encrypt.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/src/opswork/module/file_system.py` & `opswork-0.8.6/src/opswork/module/file_system.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/src/opswork/module/logger.py` & `opswork-0.8.6/src/opswork/module/logger.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/src/opswork/module/output.py` & `opswork-0.8.6/src/opswork/module/output.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/src/opswork/module/playbook.py` & `opswork-0.8.6/src/opswork/module/playbook.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/src/opswork.egg-info/PKG-INFO` & `opswork-0.8.6/src/opswork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opswork
-Version: 0.8.5
+Version: 0.8.6
 Summary: OpsWork Swiss Knife.
 Home-page: https://github.com/Clivern/OpsWork/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/Clivern/OpsWork/
 Project-URL: Source, https://github.com/Clivern/OpsWork/
@@ -19,15 +19,15 @@
 License-File: LICENSE.txt
 Requires-Dist: click<=8.1.7
 Requires-Dist: ansible-runner<=2.4.0
 Requires-Dist: prettytable<=3.10.0
 Requires-Dist: PyYAML<=6.0.1
 Requires-Dist: cryptography<=42.0.7
 Requires-Dist: GitPython<=3.1.43
-Requires-Dist: requests<=2.31.0
+Requires-Dist: requests<=2.32.2
 Requires-Dist: importlib-metadata<=7.1.0; python_version < "3.8"
 
 .. image:: https://img.shields.io/pypi/v/opswork.svg
     :alt: PyPI-Server
     :target: https://pypi.org/project/opswork/
 .. image:: https://github.com/clivern/opswork/actions/workflows/ci.yml/badge.svg
     :alt: Build Status
```

### Comparing `opswork-0.8.5/src/opswork.egg-info/SOURCES.txt` & `opswork-0.8.6/src/opswork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/tests/__init__.py` & `opswork-0.8.6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/tests/module/test_logger.py` & `opswork-0.8.6/tests/module/test_logger.py`

 * *Files identical despite different names*

### Comparing `opswork-0.8.5/tox.ini` & `opswork-0.8.6/tox.ini`

 * *Files identical despite different names*

