# Comparing `tmp/django-simple-history-3.5.0.tar.gz` & `tmp/django_simple_history-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-simple-history-3.5.0.tar", last modified: Mon Feb 19 21:09:07 2024, max compression
+gzip compressed data, was "django_simple_history-3.6.0.tar", last modified: Sun May 26 23:26:53 2024, max compression
```

## Comparing `django-simple-history-3.5.0.tar` & `django_simple_history-3.6.0.tar`

### file list

```diff
@@ -1,189 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.562512 django-simple-history-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/.codeclimate.yml
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.538512 django-simple-history-3.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.542512 django-simple-history-3.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.542512 django-simple-history-3.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    18060 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    21820 2024-02-19 21:09:07.562512 django-simple-history-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.558512 django-simple-history-3.5.0/django_simple_history.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21820 2024-02-19 21:09:07.000000 django-simple-history-3.5.0/django_simple_history.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-02-19 21:09:07.000000 django-simple-history-3.5.0/django_simple_history.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 21:09:07.000000 django-simple-history-3.5.0/django_simple_history.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-19 21:09:07.000000 django-simple-history-3.5.0/django_simple_history.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-19 21:09:07.000000 django-simple-history-3.5.0/django_simple_history.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/doc-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.542512 django-simple-history-3.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.542512 django-simple-history-3.5.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/docs/_static/.keep
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/docs/admin.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/docs/common_issues.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/docs/historical_model.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/docs/history_diffing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/docs/multiple_dbs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/docs/querying_history.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/docs/quick_start.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.546512 django-simple-history-3.5.0/docs/screens/
--rw-r--r--   0 runner    (1001) docker     (127)    88377 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/docs/screens/10_revert_disabled.png
--rw-r--r--   0 runner    (1001) docker     (127)   101284 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/docs/screens/1_poll_history.png
--rw-r--r--   0 runner    (1001) docker     (127)   111293 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/docs/screens/2_revert.png
--rw-r--r--   0 runner    (1001) docker     (127)    90104 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/docs/screens/3_poll_reverted.png
--rw-r--r--   0 runner    (1001) docker     (127)   110264 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/docs/screens/4_history_after_poll_reverted.png
--rw-r--r--   0 runner    (1001) docker     (127)    38025 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/docs/screens/5_history_list_display.png
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/docs/signals.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/docs/user_tracking.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.546512 django-simple-history-3.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/requirements/coverage.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/requirements/lint.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/requirements/mysql.txt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/requirements/postgres.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/requirements/tox.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     5529 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/runtests.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 21:09:07.562512 django-simple-history-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.546512 django-simple-history-3.5.0/simple_history/
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11906 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.534512 django-simple-history-3.5.0/simple_history/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.534512 django-simple-history-3.5.0/simple_history/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.546512 django-simple-history-3.5.0/simple_history/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.534512 django-simple-history-3.5.0/simple_history/locale/cs_CZ/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.546512 django-simple-history-3.5.0/simple_history/locale/cs_CZ/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/locale/cs_CZ/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/locale/cs_CZ/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.534512 django-simple-history-3.5.0/simple_history/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.550512 django-simple-history-3.5.0/simple_history/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.534512 django-simple-history-3.5.0/simple_history/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.550512 django-simple-history-3.5.0/simple_history/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.534512 django-simple-history-3.5.0/simple_history/locale/id/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.550512 django-simple-history-3.5.0/simple_history/locale/id/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/locale/id/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/locale/id/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.534512 django-simple-history-3.5.0/simple_history/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.550512 django-simple-history-3.5.0/simple_history/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.534512 django-simple-history-3.5.0/simple_history/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.550512 django-simple-history-3.5.0/simple_history/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.534512 django-simple-history-3.5.0/simple_history/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.550512 django-simple-history-3.5.0/simple_history/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.534512 django-simple-history-3.5.0/simple_history/locale/ru_RU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.550512 django-simple-history-3.5.0/simple_history/locale/ru_RU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/locale/ru_RU/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/locale/ru_RU/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.534512 django-simple-history-3.5.0/simple_history/locale/ur/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.550512 django-simple-history-3.5.0/simple_history/locale/ur/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/locale/ur/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/locale/ur/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.534512 django-simple-history-3.5.0/simple_history/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.550512 django-simple-history-3.5.0/simple_history/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.550512 django-simple-history-3.5.0/simple_history/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.550512 django-simple-history-3.5.0/simple_history/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/management/commands/clean_duplicate_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/management/commands/clean_old_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/management/commands/populate_history.py
--rw-r--r--   0 runner    (1001) docker     (127)    10053 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    38041 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.554512 django-simple-history-3.5.0/simple_history/registry_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/registry_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.554512 django-simple-history-3.5.0/simple_history/registry_tests/migration_test_app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/registry_tests/migration_test_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.554512 django-simple-history-3.5.0/simple_history/registry_tests/migration_test_app/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/registry_tests/migration_test_app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/registry_tests/migration_test_app/migrations/0002_historicalmodelwithcustomattrforeignkey_modelwithcustomattrforeignkey.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/registry_tests/migration_test_app/migrations/0003_alter_historicalmodelwithcustomattrforeignkey_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/registry_tests/migration_test_app/migrations/0004_history_date_indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/registry_tests/migration_test_app/migrations/0005_historicalmodelwithcustomattronetoonefield_modelwithcustomattronetoonefield.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/registry_tests/migration_test_app/migrations/0006_alter_historicalmodelwithcustomattronetoonefield_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/registry_tests/migration_test_app/migrations/0007_alter_historicalmodelwithcustomattrforeignkey_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/registry_tests/migration_test_app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/registry_tests/migration_test_app/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/registry_tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/registry_tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.534512 django-simple-history-3.5.0/simple_history/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.554512 django-simple-history-3.5.0/simple_history/templates/simple_history/
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/templates/simple_history/_object_history_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/templates/simple_history/object_history.html
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/templates/simple_history/object_history_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/templates/simple_history/submit_line.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.554512 django-simple-history-3.5.0/simple_history/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/templatetags/getattributes.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/templatetags/simple_history_admin_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/templatetags/simple_history_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.558512 django-simple-history-3.5.0/simple_history/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/tests/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.558512 django-simple-history-3.5.0/simple_history/tests/custom_user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/tests/custom_user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/tests/custom_user/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/tests/custom_user/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.558512 django-simple-history-3.5.0/simple_history/tests/external/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/tests/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/tests/external/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.558512 django-simple-history-3.5.0/simple_history/tests/generated_file_checks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/tests/generated_file_checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/tests/generated_file_checks/check_translations.py
--rw-r--r--   0 runner    (1001) docker     (127)    26018 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/tests/other_admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:09:07.558512 django-simple-history-3.5.0/simple_history/tests/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/tests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37384 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/tests/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    23446 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/tests/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/tests/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    13709 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/tests/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10246 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/tests/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    98325 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/tests/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/tests/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/tests/tests/test_templatetags.py
--rw-r--r--   0 runner    (1001) docker     (127)    21030 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/tests/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/tests/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/tests/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     8667 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/simple_history/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-02-19 21:08:56.000000 django-simple-history-3.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.313086 django_simple_history-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.codeclimate.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.289086 django_simple_history-3.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.289086 django_simple_history-3.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.289086 django_simple_history-3.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    20025 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    23785 2024-05-26 23:26:53.313086 django_simple_history-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.313086 django_simple_history-3.6.0/django_simple_history.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23785 2024-05-26 23:26:53.000000 django_simple_history-3.6.0/django_simple_history.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-26 23:26:53.000000 django_simple_history-3.6.0/django_simple_history.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 23:26:53.000000 django_simple_history-3.6.0/django_simple_history.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-26 23:26:53.000000 django_simple_history-3.6.0/django_simple_history.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-26 23:26:53.000000 django_simple_history-3.6.0/django_simple_history.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/doc-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.293086 django_simple_history-3.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.293086 django_simple_history-3.6.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/_static/.keep
+-rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/admin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/common_issues.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19603 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/historical_model.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/history_diffing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/multiple_dbs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/querying_history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/quick_start.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.293086 django_simple_history-3.6.0/docs/screens/
+-rw-r--r--   0 runner    (1001) docker     (127)    15881 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/screens/10_revert_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19753 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/screens/1_poll_history.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17844 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/screens/2_revert.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16449 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/screens/3_poll_reverted.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21966 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/screens/4_history_after_poll_reverted.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/screens/5_history_list_display.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/signals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/user_tracking.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.297086 django_simple_history-3.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/requirements/coverage.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/requirements/lint.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/requirements/mysql.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/requirements/postgres.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/requirements/tox.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5529 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 23:26:53.313086 django_simple_history-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.297086 django_simple_history-3.6.0/simple_history/
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15067 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.281086 django_simple_history-3.6.0/simple_history/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.281086 django_simple_history-3.6.0/simple_history/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.297086 django_simple_history-3.6.0/simple_history/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.281086 django_simple_history-3.6.0/simple_history/locale/cs_CZ/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.297086 django_simple_history-3.6.0/simple_history/locale/cs_CZ/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/cs_CZ/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/cs_CZ/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.281086 django_simple_history-3.6.0/simple_history/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.297086 django_simple_history-3.6.0/simple_history/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.281086 django_simple_history-3.6.0/simple_history/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.297086 django_simple_history-3.6.0/simple_history/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.281086 django_simple_history-3.6.0/simple_history/locale/id/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.301086 django_simple_history-3.6.0/simple_history/locale/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.281086 django_simple_history-3.6.0/simple_history/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.301086 django_simple_history-3.6.0/simple_history/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.281086 django_simple_history-3.6.0/simple_history/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.301086 django_simple_history-3.6.0/simple_history/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.281086 django_simple_history-3.6.0/simple_history/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.301086 django_simple_history-3.6.0/simple_history/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.281086 django_simple_history-3.6.0/simple_history/locale/ru_RU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.301086 django_simple_history-3.6.0/simple_history/locale/ru_RU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/ru_RU/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/ru_RU/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.281086 django_simple_history-3.6.0/simple_history/locale/ur/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.301086 django_simple_history-3.6.0/simple_history/locale/ur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/ur/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/ur/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.281086 django_simple_history-3.6.0/simple_history/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.301086 django_simple_history-3.6.0/simple_history/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.301086 django_simple_history-3.6.0/simple_history/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.301086 django_simple_history-3.6.0/simple_history/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/management/commands/clean_duplicate_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/management/commands/clean_old_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/management/commands/populate_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44885 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.301086 django_simple_history-3.6.0/simple_history/registry_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.301086 django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.305086 django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0002_historicalmodelwithcustomattrforeignkey_modelwithcustomattrforeignkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0003_alter_historicalmodelwithcustomattrforeignkey_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0004_history_date_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0005_historicalmodelwithcustomattronetoonefield_modelwithcustomattronetoonefield.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0006_alter_historicalmodelwithcustomattronetoonefield_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0007_alter_historicalmodelwithcustomattrforeignkey_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/registry_tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/template_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.285086 django_simple_history-3.6.0/simple_history/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.305086 django_simple_history-3.6.0/simple_history/templates/simple_history/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/templates/simple_history/object_history.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/templates/simple_history/object_history_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/templates/simple_history/object_history_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/templates/simple_history/submit_line.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.305086 django_simple_history-3.6.0/simple_history/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/templatetags/getattributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/templatetags/simple_history_admin_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/templatetags/simple_history_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.309086 django_simple_history-3.6.0/simple_history/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.309086 django_simple_history-3.6.0/simple_history/tests/custom_user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/custom_user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/custom_user/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/custom_user/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.309086 django_simple_history-3.6.0/simple_history/tests/external/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/external/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.309086 django_simple_history-3.6.0/simple_history/tests/generated_file_checks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/generated_file_checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/generated_file_checks/check_translations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26580 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/other_admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:26:53.313086 django_simple_history-3.6.0/simple_history/tests/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44355 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23446 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15129 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10246 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107885 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13486 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/test_template_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23823 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/tests/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9612 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/simple_history/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-26 23:26:43.000000 django_simple_history-3.6.0/tox.ini
```

### Comparing `django-simple-history-3.5.0/.codeclimate.yml` & `django_simple_history-3.6.0/.codeclimate.yml`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/.github/ISSUE_TEMPLATE/bug_report.md` & `django_simple_history-3.6.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/.github/ISSUE_TEMPLATE/feature_request.md` & `django_simple_history-3.6.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/.github/workflows/release.yml` & `django_simple_history-3.6.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/.github/workflows/test.yml` & `django_simple_history-3.6.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/.pre-commit-config.yaml` & `django_simple_history-3.6.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 ---
 repos:
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.7.7
+    rev: 1.7.8
     hooks:
       - id: bandit
-        args:
-          - "-x *test*.py"
+        exclude: /.*tests/
 
   - repo: https://github.com/psf/black-pre-commit-mirror
-    rev: 24.2.0
+    rev: 24.4.2
     hooks:
       - id: black
         language_version: python3.8
 
   - repo: https://github.com/pycqa/flake8
     rev: 7.0.0
     hooks:
@@ -22,15 +21,15 @@
 
   - repo: https://github.com/PyCQA/isort
     rev: 5.13.2
     hooks:
       - id: isort
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: requirements-txt-fixer
         files: requirements/.*\.txt$
       - id: trailing-whitespace
       - id: check-added-large-files
       - id: fix-byte-order-marker
       - id: check-docstring-first
@@ -43,11 +42,11 @@
     rev: v1.35.1
     hooks:
       - id: yamllint
         args:
           - "--strict"
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.15.1
+    rev: v3.15.2
     hooks:
       - id: pyupgrade
         args: [--py38-plus]
```

### Comparing `django-simple-history-3.5.0/.readthedocs.yaml` & `django_simple_history-3.6.0/.readthedocs.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -17,7 +17,10 @@
 
 # Optional but recommended, declare the Python requirements required
 # to build your documentation
 # See https://docs.readthedocs.io/en/stable/guides/reproducible-builds.html
 python:
   install:
     - requirements: requirements/docs.txt
+    # Install this project locally, so that its package metadata can be queried
+    - method: pip
+      path: .
```

### Comparing `django-simple-history-3.5.0/AUTHORS.rst` & `django_simple_history-3.6.0/AUTHORS.rst`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,15 @@
 - `Paulo Peres <https://github.com/PauloPeres>`_
 - `Alex Todorov <https://github.com/atodorov>`_
 - David Smith (`smithdc1 <https://github.com/smithdc1>`_)
 - Shi Han Ng (`shihanng <https://github.com/shihanng>`_)
 - `ddusi <https://github.com/ddusi>`_
 - `DanialErfanian <https://github.com/DanialErfanian>`_
 - `Sridhar Marella <https://github.com/sridhar562345>`_
+- `Mattia Fantoni <https://github.com/MattFanto>`_
 
 Background
 ==========
 
 This code originally comes from Pro Django, published by Apress, Inc.
 in December 2008. The author of the book and primary author
 of the code is Marty Alchin <marty@martyalchin.com>, who
```

### Comparing `django-simple-history-3.5.0/CHANGES.rst` & `django_simple_history-3.6.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,44 @@
 Changes
 =======
 
 Unreleased
 ----------
 
 
+3.6.0 (2024-05-26)
+------------------
+
+- Support custom History ``Manager`` and ``QuerySet`` classes (gh-1280)
+- Renamed the (previously internal) admin template
+  ``simple_history/_object_history_list.html`` to
+  ``simple_history/object_history_list.html``, and added the field
+  ``SimpleHistoryAdmin.object_history_list_template`` for overriding it (gh-1128)
+- Deprecated the undocumented template tag ``simple_history_admin_list.display_list()``;
+  it will be removed in version 3.8 (gh-1128)
+- Added ``SimpleHistoryAdmin.get_history_queryset()`` for overriding which ``QuerySet``
+  is used to list the historical records (gh-1128)
+- Added ``SimpleHistoryAdmin.get_history_list_display()`` which returns
+  ``history_list_display`` by default, and made the latter into an actual field (gh-1128)
+- ``ModelDelta`` and ``ModelChange`` (in ``simple_history.models``) are now immutable
+  dataclasses; their signatures remain unchanged (gh-1128)
+- ``ModelDelta``'s ``changes`` and ``changed_fields`` are now sorted alphabetically by
+  field name. Also, if ``ModelChange`` is for an M2M field, its ``old`` and ``new``
+  lists are sorted by the related object. This should help prevent flaky tests. (gh-1128)
+- ``diff_against()`` has a new keyword argument, ``foreign_keys_are_objs``;
+  see usage in the docs under "History Diffing" (gh-1128)
+- Added a "Changes" column to ``SimpleHistoryAdmin``'s object history table, listing
+  the changes between each historical record of the object; see the docs under
+  "Customizing the History Admin Templates" for overriding its template context (gh-1128)
+- Fixed the setting ``SIMPLE_HISTORY_ENABLED = False`` not preventing M2M historical
+  records from being created (gh-1328)
+- For history-tracked M2M fields, adding M2M objects (using ``add()`` or ``set()``)
+  used to cause a number of database queries that scaled linearly with the number of
+  objects; this has been fixed to now be a constant number of queries (gh-1333)
+
 3.5.0 (2024-02-19)
 ------------------
 
 - Fixed ``FieldError`` when creating historical records for many-to-many fields with
   ``to="self"`` (gh-1218)
 - Allow ``HistoricalRecords.m2m_fields`` as str (gh-1243)
 - Fixed ``HistoryRequestMiddleware`` deleting non-existent
```

### Comparing `django-simple-history-3.5.0/CODE_OF_CONDUCT.md` & `django_simple_history-3.6.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/CONTRIBUTING.rst` & `django_simple_history-3.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/LICENSE.txt` & `django_simple_history-3.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/Makefile` & `django_simple_history-3.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/PKG-INFO` & `django_simple_history-3.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-history
-Version: 3.5.0
+Version: 3.6.0
 Summary: Store model history and view/revert changes from admin site.
 Home-page: https://github.com/jazzband/django-simple-history
 Author: Corey Bertram
 Author-email: corey@qr7.com
 Maintainer: Trey Hunner
 Project-URL: Documentation, https://django-simple-history.readthedocs.io/
 Project-URL: Changelog, https://github.com/jazzband/django-simple-history/blob/master/CHANGES.rst
@@ -101,14 +101,44 @@
 Changes
 =======
 
 Unreleased
 ----------
 
 
+3.6.0 (2024-05-26)
+------------------
+
+- Support custom History ``Manager`` and ``QuerySet`` classes (gh-1280)
+- Renamed the (previously internal) admin template
+  ``simple_history/_object_history_list.html`` to
+  ``simple_history/object_history_list.html``, and added the field
+  ``SimpleHistoryAdmin.object_history_list_template`` for overriding it (gh-1128)
+- Deprecated the undocumented template tag ``simple_history_admin_list.display_list()``;
+  it will be removed in version 3.8 (gh-1128)
+- Added ``SimpleHistoryAdmin.get_history_queryset()`` for overriding which ``QuerySet``
+  is used to list the historical records (gh-1128)
+- Added ``SimpleHistoryAdmin.get_history_list_display()`` which returns
+  ``history_list_display`` by default, and made the latter into an actual field (gh-1128)
+- ``ModelDelta`` and ``ModelChange`` (in ``simple_history.models``) are now immutable
+  dataclasses; their signatures remain unchanged (gh-1128)
+- ``ModelDelta``'s ``changes`` and ``changed_fields`` are now sorted alphabetically by
+  field name. Also, if ``ModelChange`` is for an M2M field, its ``old`` and ``new``
+  lists are sorted by the related object. This should help prevent flaky tests. (gh-1128)
+- ``diff_against()`` has a new keyword argument, ``foreign_keys_are_objs``;
+  see usage in the docs under "History Diffing" (gh-1128)
+- Added a "Changes" column to ``SimpleHistoryAdmin``'s object history table, listing
+  the changes between each historical record of the object; see the docs under
+  "Customizing the History Admin Templates" for overriding its template context (gh-1128)
+- Fixed the setting ``SIMPLE_HISTORY_ENABLED = False`` not preventing M2M historical
+  records from being created (gh-1328)
+- For history-tracked M2M fields, adding M2M objects (using ``add()`` or ``set()``)
+  used to cause a number of database queries that scaled linearly with the number of
+  objects; this has been fixed to now be a constant number of queries (gh-1333)
+
 3.5.0 (2024-02-19)
 ------------------
 
 - Fixed ``FieldError`` when creating historical records for many-to-many fields with
   ``to="self"`` (gh-1218)
 - Allow ``HistoricalRecords.m2m_fields`` as str (gh-1243)
 - Fixed ``HistoryRequestMiddleware`` deleting non-existent
```

### Comparing `django-simple-history-3.5.0/PULL_REQUEST_TEMPLATE.md` & `django_simple_history-3.6.0/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/README.rst` & `django_simple_history-3.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/django_simple_history.egg-info/PKG-INFO` & `django_simple_history-3.6.0/django_simple_history.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-history
-Version: 3.5.0
+Version: 3.6.0
 Summary: Store model history and view/revert changes from admin site.
 Home-page: https://github.com/jazzband/django-simple-history
 Author: Corey Bertram
 Author-email: corey@qr7.com
 Maintainer: Trey Hunner
 Project-URL: Documentation, https://django-simple-history.readthedocs.io/
 Project-URL: Changelog, https://github.com/jazzband/django-simple-history/blob/master/CHANGES.rst
@@ -101,14 +101,44 @@
 Changes
 =======
 
 Unreleased
 ----------
 
 
+3.6.0 (2024-05-26)
+------------------
+
+- Support custom History ``Manager`` and ``QuerySet`` classes (gh-1280)
+- Renamed the (previously internal) admin template
+  ``simple_history/_object_history_list.html`` to
+  ``simple_history/object_history_list.html``, and added the field
+  ``SimpleHistoryAdmin.object_history_list_template`` for overriding it (gh-1128)
+- Deprecated the undocumented template tag ``simple_history_admin_list.display_list()``;
+  it will be removed in version 3.8 (gh-1128)
+- Added ``SimpleHistoryAdmin.get_history_queryset()`` for overriding which ``QuerySet``
+  is used to list the historical records (gh-1128)
+- Added ``SimpleHistoryAdmin.get_history_list_display()`` which returns
+  ``history_list_display`` by default, and made the latter into an actual field (gh-1128)
+- ``ModelDelta`` and ``ModelChange`` (in ``simple_history.models``) are now immutable
+  dataclasses; their signatures remain unchanged (gh-1128)
+- ``ModelDelta``'s ``changes`` and ``changed_fields`` are now sorted alphabetically by
+  field name. Also, if ``ModelChange`` is for an M2M field, its ``old`` and ``new``
+  lists are sorted by the related object. This should help prevent flaky tests. (gh-1128)
+- ``diff_against()`` has a new keyword argument, ``foreign_keys_are_objs``;
+  see usage in the docs under "History Diffing" (gh-1128)
+- Added a "Changes" column to ``SimpleHistoryAdmin``'s object history table, listing
+  the changes between each historical record of the object; see the docs under
+  "Customizing the History Admin Templates" for overriding its template context (gh-1128)
+- Fixed the setting ``SIMPLE_HISTORY_ENABLED = False`` not preventing M2M historical
+  records from being created (gh-1328)
+- For history-tracked M2M fields, adding M2M objects (using ``add()`` or ``set()``)
+  used to cause a number of database queries that scaled linearly with the number of
+  objects; this has been fixed to now be a constant number of queries (gh-1333)
+
 3.5.0 (2024-02-19)
 ------------------
 
 - Fixed ``FieldError`` when creating historical records for many-to-many fields with
   ``to="self"`` (gh-1218)
 - Allow ``HistoricalRecords.m2m_fields`` as str (gh-1243)
 - Fixed ``HistoryRequestMiddleware`` deleting non-existent
```

### Comparing `django-simple-history-3.5.0/django_simple_history.egg-info/SOURCES.txt` & `django_simple_history-3.6.0/django_simple_history.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 simple_history/__init__.py
 simple_history/admin.py
 simple_history/exceptions.py
 simple_history/manager.py
 simple_history/middleware.py
 simple_history/models.py
 simple_history/signals.py
+simple_history/template_utils.py
 simple_history/utils.py
 simple_history/locale/ar/LC_MESSAGES/django.mo
 simple_history/locale/ar/LC_MESSAGES/django.po
 simple_history/locale/cs_CZ/LC_MESSAGES/django.mo
 simple_history/locale/cs_CZ/LC_MESSAGES/django.po
 simple_history/locale/de/LC_MESSAGES/django.mo
 simple_history/locale/de/LC_MESSAGES/django.po
@@ -103,17 +104,17 @@
 simple_history/registry_tests/migration_test_app/migrations/0002_historicalmodelwithcustomattrforeignkey_modelwithcustomattrforeignkey.py
 simple_history/registry_tests/migration_test_app/migrations/0003_alter_historicalmodelwithcustomattrforeignkey_options_and_more.py
 simple_history/registry_tests/migration_test_app/migrations/0004_history_date_indexing.py
 simple_history/registry_tests/migration_test_app/migrations/0005_historicalmodelwithcustomattronetoonefield_modelwithcustomattronetoonefield.py
 simple_history/registry_tests/migration_test_app/migrations/0006_alter_historicalmodelwithcustomattronetoonefield_options_and_more.py
 simple_history/registry_tests/migration_test_app/migrations/0007_alter_historicalmodelwithcustomattrforeignkey_options_and_more.py
 simple_history/registry_tests/migration_test_app/migrations/__init__.py
-simple_history/templates/simple_history/_object_history_list.html
 simple_history/templates/simple_history/object_history.html
 simple_history/templates/simple_history/object_history_form.html
+simple_history/templates/simple_history/object_history_list.html
 simple_history/templates/simple_history/submit_line.html
 simple_history/templatetags/__init__.py
 simple_history/templatetags/getattributes.py
 simple_history/templatetags/simple_history_admin_list.py
 simple_history/templatetags/simple_history_compat.py
 simple_history/tests/__init__.py
 simple_history/tests/admin.py
@@ -127,15 +128,17 @@
 simple_history/tests/external/__init__.py
 simple_history/tests/external/models.py
 simple_history/tests/generated_file_checks/__init__.py
 simple_history/tests/generated_file_checks/check_translations.py
 simple_history/tests/tests/__init__.py
 simple_history/tests/tests/test_admin.py
 simple_history/tests/tests/test_commands.py
+simple_history/tests/tests/test_deprecation.py
 simple_history/tests/tests/test_index.py
 simple_history/tests/tests/test_manager.py
 simple_history/tests/tests/test_middleware.py
 simple_history/tests/tests/test_models.py
 simple_history/tests/tests/test_signals.py
+simple_history/tests/tests/test_template_utils.py
 simple_history/tests/tests/test_templatetags.py
 simple_history/tests/tests/test_utils.py
 simple_history/tests/tests/utils.py
```

### Comparing `django-simple-history-3.5.0/docs/Makefile` & `django_simple_history-3.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/docs/common_issues.rst` & `django_simple_history-3.6.0/docs/common_issues.rst`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/docs/conf.py` & `django_simple_history-3.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/docs/historical_model.rst` & `django_simple_history-3.6.0/docs/historical_model.rst`

 * *Files 10% similar despite different names*

```diff
@@ -175,14 +175,85 @@
 The resulting history class names would be `AuditPoll` and `AuditOpinion`.
 If the app the models are defined in is `yoda` then the corresponding history table names would be `yoda_auditpoll` and `yoda_auditopinion`
 
 IMPORTANT: Setting `custom_model_name` to `lambda x:f'{x}'` is not permitted.
            An error will be generated and no history model created if they are the same.
 
 
+Custom History Manager and Historical QuerySets
+-----------------------------------------------
+
+To manipulate the history ``Manager`` or the historical ``QuerySet`` of
+``HistoricalRecords``, you can specify the ``history_manager`` and
+``historical_queryset`` options. The values must be subclasses
+of ``simple_history.manager.HistoryManager`` and
+``simple_history.manager.HistoricalQuerySet``, respectively.
+
+Keep in mind, you can use either or both of these options. To understand the
+difference between a ``Manager`` and a ``QuerySet``,
+see `Django's Manager documentation`_.
+
+.. code-block:: python
+
+    from datetime import timedelta
+    from django.db import models
+    from django.utils import timezone
+    from simple_history.manager import HistoryManager, HistoricalQuerySet
+    from simple_history.models import HistoricalRecords
+
+
+    class HistoryQuestionManager(HistoryManager):
+        def published(self):
+            return self.filter(pub_date__lte=timezone.now())
+
+
+    class HistoryQuestionQuerySet(HistoricalQuerySet):
+        def question_prefixed(self):
+            return self.filter(question__startswith="Question: ")
+
+
+    class Question(models.Model):
+        pub_date = models.DateTimeField("date published")
+        history = HistoricalRecords(
+            history_manager=HistoryQuestionManager,
+            historical_queryset=HistoryQuestionQuerySet,
+        )
+
+    # This is now possible:
+    queryset = Question.history.published().question_prefixed()
+
+
+To reuse a ``QuerySet`` from the model, see the following code example:
+
+.. code-block:: python
+
+    from datetime import timedelta
+    from django.db import models
+    from django.utils import timezone
+    from simple_history.models import HistoricalRecords
+    from simple_history.manager import HistoryManager, HistoricalQuerySet
+
+
+    class QuestionQuerySet(models.QuerySet):
+        def question_prefixed(self):
+            return self.filter(question__startswith="Question: ")
+
+
+    class HistoryQuestionQuerySet(QuestionQuerySet, HistoricalQuerySet):
+        """Redefine ``QuerySet`` with base class ``HistoricalQuerySet``."""
+
+
+    class Question(models.Model):
+        pub_date = models.DateTimeField("date published")
+        history = HistoricalRecords(historical_queryset=HistoryQuestionQuerySet)
+        manager = QuestionQuerySet.as_manager()
+
+.. _Django's Manager documentation: https://docs.djangoproject.com/en/stable/topics/db/managers/
+
+
 TextField as `history_change_reason`
 ------------------------------------
 
 The ``HistoricalRecords`` object can be customized to accept a
 ``TextField`` model field for saving the
 `history_change_reason` either through settings or via the constructor on the
 model. The common use case for this is for supporting larger model change
@@ -479,15 +550,14 @@
 You will see the many to many changes when diffing between two historical records:
 
 .. code-block:: python
 
     informal = Category.objects.create(name="informal questions")
     official = Category.objects.create(name="official questions")
     p = Poll.objects.create(question="what's up?")
-    p.save()
     p.categories.add(informal, official)
     p.categories.remove(informal)
 
     last_record = p.history.latest()
     previous_record = last_record.prev_record
     delta = last_record.diff_against(previous_record)
```

### Comparing `django-simple-history-3.5.0/docs/index.rst` & `django_simple_history-3.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/docs/make.bat` & `django_simple_history-3.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/docs/multiple_dbs.rst` & `django_simple_history-3.6.0/docs/multiple_dbs.rst`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/docs/querying_history.rst` & `django_simple_history-3.6.0/docs/querying_history.rst`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/docs/quick_start.rst` & `django_simple_history-3.6.0/docs/quick_start.rst`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/docs/signals.rst` & `django_simple_history-3.6.0/docs/signals.rst`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/docs/user_tracking.rst` & `django_simple_history-3.6.0/docs/user_tracking.rst`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/docs/utils.rst` & `django_simple_history-3.6.0/docs/utils.rst`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/runtests.py` & `django_simple_history-3.6.0/runtests.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/setup.py` & `django_simple_history-3.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/__init__.py` & `django_simple_history-3.6.0/simple_history/__init__.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/admin.py` & `django_simple_history-3.6.0/simple_history/admin.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,38 @@
+from typing import Any, Sequence
+
 from django import http
 from django.apps import apps as django_apps
 from django.conf import settings
 from django.contrib import admin
 from django.contrib.admin import helpers
 from django.contrib.admin.utils import unquote
 from django.contrib.auth import get_permission_codename, get_user_model
 from django.core.exceptions import PermissionDenied
+from django.db.models import QuerySet
 from django.shortcuts import get_object_or_404, render
 from django.urls import re_path, reverse
 from django.utils.encoding import force_str
 from django.utils.html import mark_safe
 from django.utils.text import capfirst
 from django.utils.translation import gettext as _
 
+from .manager import HistoricalQuerySet, HistoryManager
+from .models import HistoricalChanges
+from .template_utils import HistoricalRecordContextHelper
 from .utils import get_history_manager_for_model, get_history_model_for_model
 
 SIMPLE_HISTORY_EDIT = getattr(settings, "SIMPLE_HISTORY_EDIT", False)
 
 
 class SimpleHistoryAdmin(admin.ModelAdmin):
+    history_list_display = []
+
     object_history_template = "simple_history/object_history.html"
+    object_history_list_template = "simple_history/object_history_list.html"
     object_history_form_template = "simple_history/object_history_form.html"
 
     def get_urls(self):
         """Returns the additional urls used by the Reversion admin."""
         urls = super().get_urls()
         admin_site = self.admin_site
         opts = self.model._meta
@@ -42,49 +51,51 @@
         request.current_app = self.admin_site.name
         model = self.model
         opts = model._meta
         app_label = opts.app_label
         pk_name = opts.pk.attname
         history = getattr(model, model._meta.simple_history_manager_attribute)
         object_id = unquote(object_id)
-        action_list = history.filter(**{pk_name: object_id})
-        if not isinstance(history.model.history_user, property):
-            # Only select_related when history_user is a ForeignKey (not a property)
-            action_list = action_list.select_related("history_user")
-        history_list_display = getattr(self, "history_list_display", [])
+        historical_records = self.get_history_queryset(
+            request, history, pk_name, object_id
+        )
+        history_list_display = self.get_history_list_display(request)
         # If no history was found, see whether this object even exists.
         try:
             obj = self.get_queryset(request).get(**{pk_name: object_id})
         except model.DoesNotExist:
             try:
-                obj = action_list.latest("history_date").instance
-            except action_list.model.DoesNotExist:
+                obj = historical_records.latest("history_date").instance
+            except historical_records.model.DoesNotExist:
                 raise http.Http404
 
         if not self.has_view_history_or_change_history_permission(request, obj):
             raise PermissionDenied
 
-        # Set attribute on each action_list entry from admin methods
+        # Set attribute on each historical record from admin methods
         for history_list_entry in history_list_display:
             value_for_entry = getattr(self, history_list_entry, None)
             if value_for_entry and callable(value_for_entry):
-                for list_entry in action_list:
-                    setattr(list_entry, history_list_entry, value_for_entry(list_entry))
+                for record in historical_records:
+                    setattr(record, history_list_entry, value_for_entry(record))
+
+        self.set_history_delta_changes(request, historical_records)
 
         content_type = self.content_type_model_cls.objects.get_for_model(
             get_user_model()
         )
-
         admin_user_view = "admin:{}_{}_change".format(
             content_type.app_label,
             content_type.model,
         )
+
         context = {
             "title": self.history_view_title(request, obj),
-            "action_list": action_list,
+            "object_history_list_template": self.object_history_list_template,
+            "historical_records": historical_records,
             "module_name": capfirst(force_str(opts.verbose_name_plural)),
             "object": obj,
             "root_path": getattr(self.admin_site, "root_path", None),
             "app_label": app_label,
             "opts": opts,
             "admin_user_view": admin_user_view,
             "history_list_display": history_list_display,
@@ -93,14 +104,81 @@
         context.update(self.admin_site.each_context(request))
         context.update(extra_context or {})
         extra_kwargs = {}
         return self.render_history_view(
             request, self.object_history_template, context, **extra_kwargs
         )
 
+    def get_history_queryset(
+        self, request, history_manager: HistoryManager, pk_name: str, object_id: Any
+    ) -> QuerySet:
+        """
+        Return a ``QuerySet`` of all historical records that should be listed in the
+        ``object_history_list_template`` template.
+        This is used by ``history_view()``.
+
+        :param request:
+        :param history_manager:
+        :param pk_name: The name of the original model's primary key field.
+        :param object_id: The primary key of the object whose history is listed.
+        """
+        qs: HistoricalQuerySet = history_manager.filter(**{pk_name: object_id})
+        if not isinstance(history_manager.model.history_user, property):
+            # Only select_related when history_user is a ForeignKey (not a property)
+            qs = qs.select_related("history_user")
+        # Prefetch related objects to reduce the number of DB queries when diffing
+        qs = qs._select_related_history_tracked_objs()
+        return qs
+
+    def get_history_list_display(self, request) -> Sequence[str]:
+        """
+        Return a sequence containing the names of additional fields to be displayed on
+        the object history page. These can either be fields or properties on the model
+        or the history model, or methods on the admin class.
+        """
+        return self.history_list_display
+
+    def get_historical_record_context_helper(
+        self, request, historical_record: HistoricalChanges
+    ) -> HistoricalRecordContextHelper:
+        """
+        Return an instance of ``HistoricalRecordContextHelper`` for formatting
+        the template context for ``historical_record``.
+        """
+        return HistoricalRecordContextHelper(self.model, historical_record)
+
+    def set_history_delta_changes(
+        self,
+        request,
+        historical_records: Sequence[HistoricalChanges],
+        foreign_keys_are_objs=True,
+    ):
+        """
+        Add a ``history_delta_changes`` attribute to all historical records
+        except the first (oldest) one.
+
+        :param request:
+        :param historical_records:
+        :param foreign_keys_are_objs: Passed to ``diff_against()`` when calculating
+               the deltas; see its docstring for details.
+        """
+        previous = None
+        for current in historical_records:
+            if previous is None:
+                previous = current
+                continue
+            # Related objects should have been prefetched in `get_history_queryset()`
+            delta = previous.diff_against(
+                current, foreign_keys_are_objs=foreign_keys_are_objs
+            )
+            helper = self.get_historical_record_context_helper(request, previous)
+            previous.history_delta_changes = helper.context_for_delta_changes(delta)
+
+            previous = current
+
     def history_view_title(self, request, obj):
         if self.revert_disabled(request, obj) and not SIMPLE_HISTORY_EDIT:
             return _("View history: %s") % force_str(obj)
         else:
             return _("Change history: %s") % force_str(obj)
 
     def response_change(self, request, obj):
```

### Comparing `django-simple-history-3.5.0/simple_history/locale/ar/LC_MESSAGES/django.mo` & `django_simple_history-3.6.0/simple_history/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/locale/ar/LC_MESSAGES/django.po` & `django_simple_history-3.6.0/simple_history/locale/ar/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -56,38 +56,14 @@
 msgid "Changed"
 msgstr "تغيير"
 
 #: simple_history/models.py:552
 msgid "Deleted"
 msgstr "تمت إزالته"
 
-#: simple_history/templates/simple_history/_object_history_list.html:9
-msgid "Object"
-msgstr "عنصر"
-
-#: simple_history/templates/simple_history/_object_history_list.html:13
-msgid "Date/time"
-msgstr "التاريخ/الوقت"
-
-#: simple_history/templates/simple_history/_object_history_list.html:14
-msgid "Comment"
-msgstr "تعليق"
-
-#: simple_history/templates/simple_history/_object_history_list.html:15
-msgid "Changed by"
-msgstr "تغير من قبل"
-
-#: simple_history/templates/simple_history/_object_history_list.html:16
-msgid "Change reason"
-msgstr "سبب التغير"
-
-#: simple_history/templates/simple_history/_object_history_list.html:37
-msgid "None"
-msgstr "فارغ"
-
 #: simple_history/templates/simple_history/object_history.html:11
 msgid ""
 "Choose a date from the list below to revert to a previous version of this "
 "object."
 msgstr "إختر تاريخ من القائمة ادناه."
 
 #: simple_history/templates/simple_history/object_history.html:16
@@ -117,14 +93,38 @@
 "Press the 'Revert' button below to revert to this version of the object."
 msgstr "اضغط على زر 'استرجاع' ادناه للاسترجاع لهذه النسخة من العنصر."
 
 #: simple_history/templates/simple_history/object_history_form.html:25
 msgid "Press the 'Change History' button below to edit the history."
 msgstr "اضغط على زر 'تعديل سجل التغيرات' ادناه لتعديل التاريخ."
 
+#: simple_history/templates/simple_history/object_history_list.html:9
+msgid "Object"
+msgstr "عنصر"
+
+#: simple_history/templates/simple_history/object_history_list.html:13
+msgid "Date/time"
+msgstr "التاريخ/الوقت"
+
+#: simple_history/templates/simple_history/object_history_list.html:14
+msgid "Comment"
+msgstr "تعليق"
+
+#: simple_history/templates/simple_history/object_history_list.html:15
+msgid "Changed by"
+msgstr "تغير من قبل"
+
+#: simple_history/templates/simple_history/object_history_list.html:16
+msgid "Change reason"
+msgstr "سبب التغير"
+
+#: simple_history/templates/simple_history/object_history_list.html:42
+msgid "None"
+msgstr "فارغ"
+
 #: simple_history/templates/simple_history/submit_line.html:4
 msgid "Revert"
 msgstr "استرجاع"
 
 #: simple_history/templates/simple_history/submit_line.html:6
 msgid "Change History"
 msgstr "تعديل سجل التغيرات"
```

### Comparing `django-simple-history-3.5.0/simple_history/locale/cs_CZ/LC_MESSAGES/django.mo` & `django_simple_history-3.6.0/simple_history/locale/cs_CZ/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/locale/cs_CZ/LC_MESSAGES/django.po` & `django_simple_history-3.6.0/simple_history/locale/cs_CZ/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -55,38 +55,14 @@
 msgid "Changed"
 msgstr "Změněno"
 
 #: simple_history/models.py:433
 msgid "Deleted"
 msgstr "Smazáno"
 
-#: simple_history/templates/simple_history/_object_history_list.html:9
-msgid "Object"
-msgstr "Objekt"
-
-#: simple_history/templates/simple_history/_object_history_list.html:13
-msgid "Date/time"
-msgstr "Datum/čas"
-
-#: simple_history/templates/simple_history/_object_history_list.html:14
-msgid "Comment"
-msgstr "Komentář"
-
-#: simple_history/templates/simple_history/_object_history_list.html:15
-msgid "Changed by"
-msgstr "Změnil"
-
-#: simple_history/templates/simple_history/_object_history_list.html:16
-msgid "Change reason"
-msgstr "Důvod změny"
-
-#: simple_history/templates/simple_history/_object_history_list.html:37
-msgid "None"
-msgstr "Žádné"
-
 #: simple_history/templates/simple_history/object_history.html:11
 msgid ""
 "Choose a date from the list below to revert to a previous version of this "
 "object."
 msgstr ""
 "Vyberte datum ze seznamu níže a vraťte se k předchozí verzi tohoto objektu."
 
@@ -117,14 +93,38 @@
 "Press the 'Revert' button below to revert to this version of the object."
 msgstr "Stisknutím tlačítka 'Vrátit změny' se vrátíte k této verzi objektu."
 
 #: simple_history/templates/simple_history/object_history_form.html:25
 msgid "Press the 'Change History' button below to edit the history."
 msgstr "Chcete-li historii upravit, stiskněte tlačítko 'Změnit historii'"
 
+#: simple_history/templates/simple_history/object_history_list.html:9
+msgid "Object"
+msgstr "Objekt"
+
+#: simple_history/templates/simple_history/object_history_list.html:13
+msgid "Date/time"
+msgstr "Datum/čas"
+
+#: simple_history/templates/simple_history/object_history_list.html:14
+msgid "Comment"
+msgstr "Komentář"
+
+#: simple_history/templates/simple_history/object_history_list.html:15
+msgid "Changed by"
+msgstr "Změnil"
+
+#: simple_history/templates/simple_history/object_history_list.html:16
+msgid "Change reason"
+msgstr "Důvod změny"
+
+#: simple_history/templates/simple_history/object_history_list.html:42
+msgid "None"
+msgstr "Žádné"
+
 #: simple_history/templates/simple_history/submit_line.html:4
 msgid "Revert"
 msgstr "Vrátit změny"
 
 #: simple_history/templates/simple_history/submit_line.html:6
 msgid "Change History"
 msgstr "Historie změn"
```

### Comparing `django-simple-history-3.5.0/simple_history/locale/de/LC_MESSAGES/django.mo` & `django_simple_history-3.6.0/simple_history/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/locale/de/LC_MESSAGES/django.po` & `django_simple_history-3.6.0/simple_history/locale/de/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -44,38 +44,14 @@
 msgid "Changed"
 msgstr "Geändert"
 
 #: simple_history/models.py:314
 msgid "Deleted"
 msgstr "Gelöscht"
 
-#: simple_history/templates/simple_history/_object_history_list.html:9
-msgid "Object"
-msgstr "Objekt"
-
-#: simple_history/templates/simple_history/_object_history_list.html:13
-msgid "Date/time"
-msgstr "Datum/Uhrzeit"
-
-#: simple_history/templates/simple_history/_object_history_list.html:14
-msgid "Comment"
-msgstr "Kommentar"
-
-#: simple_history/templates/simple_history/_object_history_list.html:15
-msgid "Changed by"
-msgstr "Geändert von"
-
-#: simple_history/templates/simple_history/_object_history_list.html:16
-msgid "Change reason"
-msgstr "Änderungsgrund"
-
-#: simple_history/templates/simple_history/_object_history_list.html:37
-msgid "None"
-msgstr "Keine/r"
-
 #: simple_history/templates/simple_history/object_history.html:11
 msgid ""
 "Choose a date from the list below to revert to a previous version of this "
 "object."
 msgstr ""
 "Wählen Sie eine Version des Objektes aus der untenstehenden Liste, um diese "
 "wiederherzustellen."
@@ -104,14 +80,38 @@
 "Klicken Sie unten auf 'Wiederherstellen', um diese Version des Objektes "
 "wiederherzustellen."
 
 #: simple_history/templates/simple_history/object_history_form.html:21
 msgid "Or press the 'Change History' button to edit the history."
 msgstr "Oder wählen Sie 'Historie ändern', um diese zu bearbeiten."
 
+#: simple_history/templates/simple_history/object_history_list.html:9
+msgid "Object"
+msgstr "Objekt"
+
+#: simple_history/templates/simple_history/object_history_list.html:13
+msgid "Date/time"
+msgstr "Datum/Uhrzeit"
+
+#: simple_history/templates/simple_history/object_history_list.html:14
+msgid "Comment"
+msgstr "Kommentar"
+
+#: simple_history/templates/simple_history/object_history_list.html:15
+msgid "Changed by"
+msgstr "Geändert von"
+
+#: simple_history/templates/simple_history/object_history_list.html:16
+msgid "Change reason"
+msgstr "Änderungsgrund"
+
+#: simple_history/templates/simple_history/object_history_list.html:42
+msgid "None"
+msgstr "Keine/r"
+
 #: simple_history/templates/simple_history/submit_line.html:3
 msgid "Revert"
 msgstr "Wiederherstellen"
 
 #: simple_history/templates/simple_history/submit_line.html:4
 msgid "Change History"
 msgstr "Historie ändern"
```

### Comparing `django-simple-history-3.5.0/simple_history/locale/fr/LC_MESSAGES/django.mo` & `django_simple_history-3.6.0/simple_history/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/locale/fr/LC_MESSAGES/django.po` & `django_simple_history-3.6.0/simple_history/locale/fr/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -55,38 +55,14 @@
 msgid "Changed"
 msgstr "Modifié"
 
 #: .\simple_history\models.py:433
 msgid "Deleted"
 msgstr "Effacé"
 
-#: .\simple_history\templates\simple_history\_object_history_list.html:9
-msgid "Object"
-msgstr "Objet"
-
-#: .\simple_history\templates\simple_history\_object_history_list.html:13
-msgid "Date/time"
-msgstr "Date/heure"
-
-#: .\simple_history\templates\simple_history\_object_history_list.html:14
-msgid "Comment"
-msgstr "Commentaire"
-
-#: .\simple_history\templates\simple_history\_object_history_list.html:15
-msgid "Changed by"
-msgstr "Modifié par"
-
-#: .\simple_history\templates\simple_history\_object_history_list.html:16
-msgid "Change reason"
-msgstr "Raison de la modification"
-
-#: .\simple_history\templates\simple_history\_object_history_list.html:37
-msgid "None"
-msgstr "Aucun"
-
 #: .\simple_history\templates\simple_history\object_history.html:11
 msgid ""
 "Choose a date from the list below to revert to a previous version of this "
 "object."
 msgstr ""
 "Choisissez une date dans la liste ci-dessous pour revenir à une version "
 "précédente de cet objet."
@@ -121,14 +97,38 @@
 "l' objet."
 
 #: .\simple_history\templates\simple_history\object_history_form.html:25
 msgid "Press the 'Change History' button below to edit the history."
 msgstr ""
 "Cliquez sur le bouton 'Historique' ci-dessous pour modifier l'historique."
 
+#: .\simple_history\templates\simple_history\object_history_list.html:9
+msgid "Object"
+msgstr "Objet"
+
+#: .\simple_history\templates\simple_history\object_history_list.html:13
+msgid "Date/time"
+msgstr "Date/heure"
+
+#: .\simple_history\templates\simple_history\object_history_list.html:14
+msgid "Comment"
+msgstr "Commentaire"
+
+#: .\simple_history\templates\simple_history\object_history_list.html:15
+msgid "Changed by"
+msgstr "Modifié par"
+
+#: .\simple_history\templates\simple_history\object_history_list.html:16
+msgid "Change reason"
+msgstr "Raison de la modification"
+
+#: .\simple_history\templates\simple_history\object_history_list.html:42
+msgid "None"
+msgstr "Aucun"
+
 #: .\simple_history\templates\simple_history\submit_line.html:4
 msgid "Revert"
 msgstr "Rétablir"
 
 #: .\simple_history\templates\simple_history\submit_line.html:6
 msgid "Change History"
 msgstr "Historique des changements"
```

### Comparing `django-simple-history-3.5.0/simple_history/locale/id/LC_MESSAGES/django.mo` & `django_simple_history-3.6.0/simple_history/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/locale/id/LC_MESSAGES/django.po` & `django_simple_history-3.6.0/simple_history/locale/id/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -54,38 +54,14 @@
 msgid "Changed"
 msgstr "Diubah"
 
 #: .\simple_history\models.py:552
 msgid "Deleted"
 msgstr "Dihapus"
 
-#: .\simple_history\templates\simple_history\_object_history_list.html:9
-msgid "Object"
-msgstr "Objek"
-
-#: .\simple_history\templates\simple_history\_object_history_list.html:13
-msgid "Date/time"
-msgstr "Tanggal/waktu"
-
-#: .\simple_history\templates\simple_history\_object_history_list.html:14
-msgid "Comment"
-msgstr "Komentar"
-
-#: .\simple_history\templates\simple_history\_object_history_list.html:15
-msgid "Changed by"
-msgstr "Diubah oleh"
-
-#: .\simple_history\templates\simple_history\_object_history_list.html:16
-msgid "Change reason"
-msgstr "Alasan perubahan"
-
-#: .\simple_history\templates\simple_history\_object_history_list.html:37
-msgid "None"
-msgstr "Tidak ada"
-
 #: .\simple_history\templates\simple_history\object_history.html:11
 msgid ""
 "Choose a date from the list below to revert to a previous version of this "
 "object."
 msgstr ""
 "Pilih tanggal dari daftar di bawah ini untuk kembali ke versi sebelumnya "
 "dari objek ini."
@@ -118,14 +94,38 @@
 msgstr ""
 "Tekan tombol 'Kembalikan' di bawah ini untuk kembali ke versi objek ini."
 
 #: .\simple_history\templates\simple_history\object_history_form.html:25
 msgid "Press the 'Change History' button below to edit the history."
 msgstr "Tekan tombol 'Ubah Riwayat' di bawah ini untuk mengubah riwayat."
 
+#: .\simple_history\templates\simple_history\object_history_list.html:9
+msgid "Object"
+msgstr "Objek"
+
+#: .\simple_history\templates\simple_history\object_history_list.html:13
+msgid "Date/time"
+msgstr "Tanggal/waktu"
+
+#: .\simple_history\templates\simple_history\object_history_list.html:14
+msgid "Comment"
+msgstr "Komentar"
+
+#: .\simple_history\templates\simple_history\object_history_list.html:15
+msgid "Changed by"
+msgstr "Diubah oleh"
+
+#: .\simple_history\templates\simple_history\object_history_list.html:16
+msgid "Change reason"
+msgstr "Alasan perubahan"
+
+#: .\simple_history\templates\simple_history\object_history_list.html:42
+msgid "None"
+msgstr "Tidak ada"
+
 #: .\simple_history\templates\simple_history\submit_line.html:4
 msgid "Revert"
 msgstr "Kembalikan"
 
 #: .\simple_history\templates\simple_history\submit_line.html:6
 msgid "Change History"
 msgstr "Ubah Riwayat"
```

### Comparing `django-simple-history-3.5.0/simple_history/locale/nb/LC_MESSAGES/django.mo` & `django_simple_history-3.6.0/simple_history/locale/nb/LC_MESSAGES/django.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-simple-history\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2023-07-09 12:31+0200\n"
+"PO-Revision-Date: 2024-04-11 19:34+0200\n"
 "Last-Translator: Anders <ddabble@github.com>\n"
 "Language-Team: Norwegian Bokmål <placeholder@example.com>\n"
 "Language: nb\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -22,14 +22,17 @@
 
 msgid "Changed"
 msgstr "Endret"
 
 msgid "Changed by"
 msgstr "Endret av"
 
+msgid "Changes"
+msgstr "Endringer"
+
 msgid ""
 "Choose a date from the list below to revert to a previous version of this "
 "object."
 msgstr ""
 "Velg en dato fra listen nedenfor for å tilbakestille til en tidligere "
 "versjon av dette objektet."
 
@@ -44,14 +47,17 @@
 
 msgid "Date/time"
 msgstr "Dato/tid"
 
 msgid "Deleted"
 msgstr "Slettet"
 
+msgid "Deleted %(type_name)s"
+msgstr "Slettet %(type_name)s"
+
 msgid "History"
 msgstr "Historikk"
 
 msgid "Home"
 msgstr "Hjem"
 
 msgid "None"
```

### Comparing `django-simple-history-3.5.0/simple_history/locale/nb/LC_MESSAGES/django.po` & `django_simple_history-3.6.0/simple_history/locale/nb/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,50 +4,50 @@
 # Anders <ddabble@github.com>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: django-simple-history\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-07-09 13:55+0200\n"
-"PO-Revision-Date: 2023-07-09 12:31+0200\n"
+"PO-Revision-Date: 2024-04-11 19:34+0200\n"
 "Last-Translator: Anders <ddabble@github.com>\n"
 "Language-Team: Norwegian Bokmål <placeholder@example.com>\n"
 "Language: nb\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 # Dette er en tittel, ikke en handlingsbeskrivelse, så f.eks.
 # "Se/Vis (endrings)historikk" hadde ikke fungert så bra
-#: simple_history/admin.py:102
+#: simple_history/admin.py:109
 #, python-format
 msgid "View history: %s"
 msgstr "Endringshistorikk: %s"
 
-#: simple_history/admin.py:104
+#: simple_history/admin.py:111
 #, python-format
 msgid "Change history: %s"
 msgstr "Endringshistorikk: %s"
 
-#: simple_history/admin.py:110
+#: simple_history/admin.py:117
 #, python-format
 msgid "The %(name)s \"%(obj)s\" was changed successfully."
 msgstr "%(name)s «%(obj)s» ble endret."
 
-#: simple_history/admin.py:116
+#: simple_history/admin.py:123
 msgid "You may edit it again below"
 msgstr "Du kan redigere videre nedenfor"
 
-#: simple_history/admin.py:217
+#: simple_history/admin.py:224
 #, python-format
 msgid "View %s"
 msgstr "Se %s"
 
-#: simple_history/admin.py:219
+#: simple_history/admin.py:226
 #, python-format
 msgid "Revert %s"
 msgstr "Tilbakestill %s"
 
 #: simple_history/models.py:552
 msgid "Created"
 msgstr "Opprettet"
@@ -56,37 +56,18 @@
 msgid "Changed"
 msgstr "Endret"
 
 #: simple_history/models.py:552
 msgid "Deleted"
 msgstr "Slettet"
 
-#: simple_history/templates/simple_history/_object_history_list.html:9
-msgid "Object"
-msgstr "Objekt"
-
-#: simple_history/templates/simple_history/_object_history_list.html:13
-msgid "Date/time"
-msgstr "Dato/tid"
-
-#: simple_history/templates/simple_history/_object_history_list.html:14
-msgid "Comment"
-msgstr "Kommentar"
-
-#: simple_history/templates/simple_history/_object_history_list.html:15
-msgid "Changed by"
-msgstr "Endret av"
-
-#: simple_history/templates/simple_history/_object_history_list.html:16
-msgid "Change reason"
-msgstr "Endringsårsak"
-
-#: simple_history/templates/simple_history/_object_history_list.html:37
-msgid "None"
-msgstr "Ingen"
+#: simple_history/models.py:1124
+#, python-format
+msgid "Deleted %(type_name)s"
+msgstr "Slettet %(type_name)s"
 
 #: simple_history/templates/simple_history/object_history.html:11
 msgid ""
 "Choose a date from the list below to revert to a previous version of this "
 "object."
 msgstr ""
 "Velg en dato fra listen nedenfor for å tilbakestille til en tidligere "
@@ -121,14 +102,42 @@
 "Trykk på 'Tilbakestill'-knappen under for å tilbakestille til denne "
 "versjonen av objektet."
 
 #: simple_history/templates/simple_history/object_history_form.html:25
 msgid "Press the 'Change History' button below to edit the history."
 msgstr "Trykk på 'Endre historikk'-knappen under for å endre historikken."
 
+#: simple_history/templates/simple_history/object_history_list.html:9
+msgid "Object"
+msgstr "Objekt"
+
+#: simple_history/templates/simple_history/object_history_list.html:13
+msgid "Date/time"
+msgstr "Dato/tid"
+
+#: simple_history/templates/simple_history/object_history_list.html:14
+msgid "Comment"
+msgstr "Kommentar"
+
+#: simple_history/templates/simple_history/object_history_list.html:15
+msgid "Changed by"
+msgstr "Endret av"
+
+#: simple_history/templates/simple_history/object_history_list.html:16
+msgid "Change reason"
+msgstr "Endringsårsak"
+
+#: simple_history/templates/simple_history/object_history_list.html:17
+msgid "Changes"
+msgstr "Endringer"
+
+#: simple_history/templates/simple_history/object_history_list.html:42
+msgid "None"
+msgstr "Ingen"
+
 #: simple_history/templates/simple_history/submit_line.html:4
 msgid "Revert"
 msgstr "Tilbakestill"
 
 #: simple_history/templates/simple_history/submit_line.html:6
 msgid "Change History"
 msgstr "Endre historikk"
```

### Comparing `django-simple-history-3.5.0/simple_history/locale/pl/LC_MESSAGES/django.mo` & `django_simple_history-3.6.0/simple_history/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/locale/pl/LC_MESSAGES/django.po` & `django_simple_history-3.6.0/simple_history/locale/pl/LC_MESSAGES/django.po`

 * *Files 20% similar despite different names*

```diff
@@ -53,34 +53,14 @@
 #: templates/simple_history/object_history.html:10
 msgid ""
 "Choose a date from the list below to revert to a previous version of this "
 "object."
 msgstr ""
 "Wybierz datę z poniższej listy aby przywrócić poprzednią wersję tego obiektu."
 
-#: templates/simple_history/object_history.html:17
-msgid "Object"
-msgstr "Obiekt"
-
-#: templates/simple_history/object_history.html:18
-msgid "Date/time"
-msgstr "Data/czas"
-
-#: templates/simple_history/object_history.html:19
-msgid "Comment"
-msgstr "Komentarz"
-
-#: templates/simple_history/object_history.html:20
-msgid "Changed by"
-msgstr "Zmodyfikowane przez"
-
-#: templates/simple_history/object_history.html:38
-msgid "None"
-msgstr "Brak"
-
 #: templates/simple_history/object_history.html:46
 msgid "This object doesn't have a change history."
 msgstr "Ten obiekt nie ma historii zmian."
 
 #: templates/simple_history/object_history_form.html:7
 msgid "Home"
 msgstr "Strona główna"
@@ -99,14 +79,34 @@
 "Press the 'Revert' button below to revert to this version of the object."
 msgstr "Naciśnij przycisk „Przywróć” aby przywrócić tę wersję obiektu."
 
 #: templates/simple_history/object_history_form.html:21
 msgid "Or press the 'Change History' button to edit the history."
 msgstr "Lub naciśnij przycisk „Historia zmian” aby edytować historię."
 
+#: templates/simple_history/object_history_list.html:9
+msgid "Object"
+msgstr "Obiekt"
+
+#: templates/simple_history/object_history_list.html:13
+msgid "Date/time"
+msgstr "Data/czas"
+
+#: templates/simple_history/object_history_list.html:14
+msgid "Comment"
+msgstr "Komentarz"
+
+#: templates/simple_history/object_history_list.html:15
+msgid "Changed by"
+msgstr "Zmodyfikowane przez"
+
+#: templates/simple_history/object_history_list.html:42
+msgid "None"
+msgstr "Brak"
+
 #: templates/simple_history/submit_line.html:3
 msgid "Revert"
 msgstr "Przywróć"
 
 #: templates/simple_history/submit_line.html:4
 msgid "Change History"
 msgstr "Historia zmian"
```

### Comparing `django-simple-history-3.5.0/simple_history/locale/pt_BR/LC_MESSAGES/django.mo` & `django_simple_history-3.6.0/simple_history/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/locale/pt_BR/LC_MESSAGES/django.po` & `django_simple_history-3.6.0/simple_history/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -53,34 +53,14 @@
 msgid ""
 "Choose a date from the list below to revert to a previous version of this "
 "object."
 msgstr ""
 "Escolha a data desejada na lista a seguir para reverter as modificações "
 "feitas nesse objeto."
 
-#: simple_history/templates/simple_history/object_history.html:17
-msgid "Object"
-msgstr "Objeto"
-
-#: simple_history/templates/simple_history/object_history.html:18
-msgid "Date/time"
-msgstr "Data/hora"
-
-#: simple_history/templates/simple_history/object_history.html:19
-msgid "Comment"
-msgstr "Comentário"
-
-#: simple_history/templates/simple_history/object_history.html:20
-msgid "Changed by"
-msgstr "Modificado por"
-
-#: simple_history/templates/simple_history/object_history.html:38
-msgid "None"
-msgstr "-"
-
 #: simple_history/templates/simple_history/object_history.html:46
 msgid "This object doesn't have a change history."
 msgstr "Esse objeto não tem um histórico de modificações."
 
 #: simple_history/templates/simple_history/object_history_form.html:7
 msgid "Home"
 msgstr "Início"
@@ -100,14 +80,34 @@
 msgstr ""
 "Clique em 'Reverter' para reverter as modificações feitas nesse objeto."
 
 #: simple_history/templates/simple_history/object_history_form.html:21
 msgid "Or press the 'Change History' button to edit the history."
 msgstr "Ou clique em 'Histórico de Modificações' para modificar o histórico."
 
+#: simple_history/templates/simple_history/object_history_list.html:9
+msgid "Object"
+msgstr "Objeto"
+
+#: simple_history/templates/simple_history/object_history_list.html:13
+msgid "Date/time"
+msgstr "Data/hora"
+
+#: simple_history/templates/simple_history/object_history_list.html:14
+msgid "Comment"
+msgstr "Comentário"
+
+#: simple_history/templates/simple_history/object_history_list.html:15
+msgid "Changed by"
+msgstr "Modificado por"
+
+#: simple_history/templates/simple_history/object_history_list.html:42
+msgid "None"
+msgstr "-"
+
 #: simple_history/templates/simple_history/submit_line.html:3
 msgid "Revert"
 msgstr "Reverter"
 
 #: simple_history/templates/simple_history/submit_line.html:4
 msgid "Change History"
 msgstr "Histórico de Modificações"
```

### Comparing `django-simple-history-3.5.0/simple_history/locale/ru_RU/LC_MESSAGES/django.mo` & `django_simple_history-3.6.0/simple_history/locale/ru_RU/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/locale/ru_RU/LC_MESSAGES/django.po` & `django_simple_history-3.6.0/simple_history/locale/ru_RU/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -46,34 +46,14 @@
 msgid "Changed"
 msgstr "Изменено"
 
 #: models.py:306
 msgid "Deleted"
 msgstr "Удалено"
 
-#: templates/simple_history/_object_history_list.html:9
-msgid "Object"
-msgstr "Объект"
-
-#: templates/simple_history/_object_history_list.html:13
-msgid "Date/time"
-msgstr "Дата/время"
-
-#: templates/simple_history/_object_history_list.html:14
-msgid "Comment"
-msgstr "Комментарий"
-
-#: templates/simple_history/_object_history_list.html:15
-msgid "Changed by"
-msgstr "Изменено"
-
-#: templates/simple_history/_object_history_list.html:36
-msgid "None"
-msgstr "None"
-
 #: templates/simple_history/object_history.html:11
 msgid ""
 "Choose a date from the list below to revert to a previous version of this "
 "object."
 msgstr ""
 "Выберите дату из списка ниже, чтобы вернуться к предыдущей версии этого "
 "объекта."
@@ -101,18 +81,38 @@
 msgstr ""
 "Нажмите кнопку 'Восстановить' ниже, чтобы вернуться к этой версии объекта."
 
 #: templates/simple_history/object_history_form.html:21
 msgid "Or press the 'Change History' button to edit the history."
 msgstr "Или нажмите кнопку 'Изменить запись', чтобы изменить историю."
 
+#: templates/simple_history/object_history_list.html:9
+msgid "Object"
+msgstr "Объект"
+
+#: templates/simple_history/object_history_list.html:13
+msgid "Date/time"
+msgstr "Дата/время"
+
+#: templates/simple_history/object_history_list.html:14
+msgid "Comment"
+msgstr "Комментарий"
+
+#: templates/simple_history/object_history_list.html:15
+msgid "Changed by"
+msgstr "Изменено"
+
+#: templates/simple_history/object_history_list.html:16
+msgid "Change reason"
+msgstr "Причина изменения"
+
+#: templates/simple_history/object_history_list.html:42
+msgid "None"
+msgstr "None"
+
 #: templates/simple_history/submit_line.html:3
 msgid "Revert"
 msgstr "Восстановить"
 
 #: templates/simple_history/submit_line.html:4
 msgid "Change History"
 msgstr "Изменить запись"
-
-#: templates/simple_history/_object_history_list.html:16
-msgid "Change reason"
-msgstr "Причина изменения"
```

### Comparing `django-simple-history-3.5.0/simple_history/locale/ur/LC_MESSAGES/django.mo` & `django_simple_history-3.6.0/simple_history/locale/ur/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/locale/ur/LC_MESSAGES/django.po` & `django_simple_history-3.6.0/simple_history/locale/ur/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -54,38 +54,14 @@
 msgid "Changed"
 msgstr "بدل گیا"
 
 #: .\simple_history\models.py:552
 msgid "Deleted"
 msgstr "حذف کر دیا گیا"
 
-#: .\simple_history\templates\simple_history\_object_history_list.html:9
-msgid "Object"
-msgstr "آبجیکٹ"
-
-#: .\simple_history\templates\simple_history\_object_history_list.html:13
-msgid "Date/time"
-msgstr "تاریخ/وقت"
-
-#: .\simple_history\templates\simple_history\_object_history_list.html:14
-msgid "Comment"
-msgstr "تبصرہ"
-
-#: .\simple_history\templates\simple_history\_object_history_list.html:15
-msgid "Changed by"
-msgstr "کی طرف سے تبدیل"
-
-#: .\simple_history\templates\simple_history\_object_history_list.html:16
-msgid "Change reason"
-msgstr "تبدیلی کا سبب"
-
-#: .\simple_history\templates\simple_history\_object_history_list.html:37
-msgid "None"
-msgstr "کوئی نہیں"
-
 #: .\simple_history\templates\simple_history\object_history.html:11
 msgid ""
 "Choose a date from the list below to revert to a previous version of this "
 "object."
 msgstr ""
 "اس آبجیکٹ کے پچھلے ورژن پر واپس جانے کے لیے نیچے دی گئی فہرست میں سے ایک تاریخ کا انتخاب کریں۔"
 
@@ -117,14 +93,38 @@
 msgstr ""
 "آبجیکٹ کے اس ورژن پر واپس جانے کے لیے نیچے 'تبدیلی واپس کریں' کے بٹن کو دبائیں."
 
 #: .\simple_history\templates\simple_history\object_history_form.html:25
 msgid "Press the 'Change History' button below to edit the history."
 msgstr "تاریخ میں ترمیم کرنے کے لیے نیچے دیے گئے 'تاریخ کو تبدیل کریں' کے بٹن کو دبائیں."
 
+#: .\simple_history\templates\simple_history\object_history_list.html:9
+msgid "Object"
+msgstr "آبجیکٹ"
+
+#: .\simple_history\templates\simple_history\object_history_list.html:13
+msgid "Date/time"
+msgstr "تاریخ/وقت"
+
+#: .\simple_history\templates\simple_history\object_history_list.html:14
+msgid "Comment"
+msgstr "تبصرہ"
+
+#: .\simple_history\templates\simple_history\object_history_list.html:15
+msgid "Changed by"
+msgstr "کی طرف سے تبدیل"
+
+#: .\simple_history\templates\simple_history\object_history_list.html:16
+msgid "Change reason"
+msgstr "تبدیلی کا سبب"
+
+#: .\simple_history\templates\simple_history\object_history_list.html:42
+msgid "None"
+msgstr "کوئی نہیں"
+
 #: .\simple_history\templates\simple_history\submit_line.html:4
 msgid "Revert"
 msgstr "تبدیلی واپس کریں"
 
 #: .\simple_history\templates\simple_history\submit_line.html:6
 msgid "Change History"
 msgstr "تاریخ کو تبدیل کریں"
```

### Comparing `django-simple-history-3.5.0/simple_history/locale/zh_Hans/LC_MESSAGES/django.mo` & `django_simple_history-3.6.0/simple_history/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/locale/zh_Hans/LC_MESSAGES/django.po` & `django_simple_history-3.6.0/simple_history/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -54,38 +54,14 @@
 msgid "Changed"
 msgstr "已修改"
 
 #: simple_history/models.py:552
 msgid "Deleted"
 msgstr "已删除"
 
-#: simple_history/templates/simple_history/_object_history_list.html:9
-msgid "Object"
-msgstr "记录对象"
-
-#: simple_history/templates/simple_history/_object_history_list.html:13
-msgid "Date/time"
-msgstr "日期/时间"
-
-#: simple_history/templates/simple_history/_object_history_list.html:14
-msgid "Comment"
-msgstr "备注"
-
-#: simple_history/templates/simple_history/_object_history_list.html:15
-msgid "Changed by"
-msgstr "修改人"
-
-#: simple_history/templates/simple_history/_object_history_list.html:16
-msgid "Change reason"
-msgstr "修改原因"
-
-#: simple_history/templates/simple_history/_object_history_list.html:37
-msgid "None"
-msgstr "无"
-
 #: simple_history/templates/simple_history/object_history.html:11
 msgid ""
 "Choose a date from the list below to revert to a previous version of this "
 "object."
 msgstr "从下面的列表中选择一个日期以还原到该记录对象的先前版本"
 
 #: simple_history/templates/simple_history/object_history.html:16
@@ -115,14 +91,38 @@
 "Press the 'Revert' button below to revert to this version of the object."
 msgstr "按下面的“还原”按钮还原记录到当前版本。"
 
 #: simple_history/templates/simple_history/object_history_form.html:25
 msgid "Press the 'Change History' button below to edit the history."
 msgstr "按下面的“修改历史记录”按钮编辑历史记录。"
 
+#: simple_history/templates/simple_history/object_history_list.html:9
+msgid "Object"
+msgstr "记录对象"
+
+#: simple_history/templates/simple_history/object_history_list.html:13
+msgid "Date/time"
+msgstr "日期/时间"
+
+#: simple_history/templates/simple_history/object_history_list.html:14
+msgid "Comment"
+msgstr "备注"
+
+#: simple_history/templates/simple_history/object_history_list.html:15
+msgid "Changed by"
+msgstr "修改人"
+
+#: simple_history/templates/simple_history/object_history_list.html:16
+msgid "Change reason"
+msgstr "修改原因"
+
+#: simple_history/templates/simple_history/object_history_list.html:42
+msgid "None"
+msgstr "无"
+
 #: simple_history/templates/simple_history/submit_line.html:4
 msgid "Revert"
 msgstr "还原"
 
 #: simple_history/templates/simple_history/submit_line.html:6
 msgid "Change History"
 msgstr "修改历史记录"
```

### Comparing `django-simple-history-3.5.0/simple_history/management/commands/clean_duplicate_history.py` & `django_simple_history-3.6.0/simple_history/management/commands/clean_duplicate_history.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/management/commands/clean_old_history.py` & `django_simple_history-3.6.0/simple_history/management/commands/clean_old_history.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/management/commands/populate_history.py` & `django_simple_history-3.6.0/simple_history/management/commands/populate_history.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/manager.py` & `django_simple_history-3.6.0/simple_history/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,14 +87,26 @@
                 .values("pk")[:1]
             )
             latest_historics = self.filter(
                 history_id__in=Subquery(latest_pk_attr_historic_ids)
             )
         return latest_historics
 
+    def _select_related_history_tracked_objs(self):
+        """
+        A convenience method that calls ``select_related()`` with all the names of
+        the model's history-tracked ``ForeignKey`` fields.
+        """
+        field_names = [
+            field.name
+            for field in self.model.tracked_fields
+            if isinstance(field, models.ForeignKey)
+        ]
+        return self.select_related(*field_names)
+
     def _clone(self):
         c = super()._clone()
         c._as_instances = self._as_instances
         c._as_of = self._as_of
         c._pk_attr = self._pk_attr
         return c
 
@@ -115,22 +127,14 @@
         ):
             self._result_cache = [item.instance for item in self._result_cache]
             for item in self._result_cache:
                 historic = getattr(item, SIMPLE_HISTORY_REVERSE_ATTR_NAME)
                 setattr(historic, "_as_of", self._as_of)
 
 
-class HistoryDescriptor:
-    def __init__(self, model):
-        self.model = model
-
-    def __get__(self, instance, owner):
-        return HistoryManager.from_queryset(HistoricalQuerySet)(self.model, instance)
-
-
 class HistoryManager(models.Manager):
     def __init__(self, model, instance=None):
         super().__init__()
         self.model = model
         self.instance = instance
 
     def get_super_queryset(self):
@@ -268,7 +272,19 @@
             if hasattr(self.model, "history_relation"):
                 row.history_relation_id = instance.pk
             historical_instances.append(row)
 
         return self.model.objects.bulk_create(
             historical_instances, batch_size=batch_size
         )
+
+
+class HistoryDescriptor:
+    def __init__(self, model, manager=HistoryManager, queryset=HistoricalQuerySet):
+        self.model = model
+        self.queryset_class = queryset
+        self.manager_class = manager
+
+    def __get__(self, instance, owner):
+        return self.manager_class.from_queryset(self.queryset_class)(
+            self.model, instance
+        )
```

### Comparing `django-simple-history-3.5.0/simple_history/middleware.py` & `django_simple_history-3.6.0/simple_history/middleware.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/models.py` & `django_simple_history-3.6.0/simple_history/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import copy
 import importlib
 import uuid
 import warnings
+from dataclasses import dataclass
 from functools import partial
+from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Sequence, Type, Union
 
+import django
 from django.apps import apps
 from django.conf import settings
 from django.contrib import admin
 from django.contrib.auth import get_user_model
 from django.core.exceptions import ImproperlyConfigured, ObjectDoesNotExist
 from django.db import models
 from django.db.models import ManyToManyField
@@ -24,31 +27,38 @@
 from django.urls import reverse
 from django.utils import timezone
 from django.utils.encoding import smart_str
 from django.utils.functional import cached_property
 from django.utils.text import format_lazy
 from django.utils.translation import gettext_lazy as _
 
-from simple_history import utils
-
-from . import exceptions
-from .manager import SIMPLE_HISTORY_REVERSE_ATTR_NAME, HistoryDescriptor
+from . import exceptions, utils
+from .manager import (
+    SIMPLE_HISTORY_REVERSE_ATTR_NAME,
+    HistoricalQuerySet,
+    HistoryDescriptor,
+    HistoryManager,
+)
 from .signals import (
     post_create_historical_m2m_records,
     post_create_historical_record,
     pre_create_historical_m2m_records,
     pre_create_historical_record,
 )
-from .utils import get_change_reason_from_object
 
 try:
     from asgiref.local import Local as LocalContext
 except ImportError:
     from threading import local as LocalContext
 
+if TYPE_CHECKING:
+    ModelTypeHint = models.Model
+else:
+    ModelTypeHint = object
+
 registered_models = {}
 
 
 def _default_get_user(request, **kwargs):
     try:
         return request.user
     except AttributeError:
@@ -96,14 +106,16 @@
         history_user_getter=_history_user_getter,
         history_user_setter=_history_user_setter,
         related_name=None,
         use_base_model_db=False,
         user_db_constraint=True,
         no_db_index=list(),
         excluded_field_kwargs=None,
+        history_manager=HistoryManager,
+        historical_queryset=HistoricalQuerySet,
         m2m_fields=(),
         m2m_fields_model_field_name="_history_m2m_fields",
         m2m_bases=(models.Model,),
     ):
         self.user_set_verbose_name = verbose_name
         self.user_set_verbose_name_plural = verbose_name_plural
         self.user_related_name = user_related_name
@@ -118,14 +130,16 @@
         self.custom_model_name = custom_model_name
         self.app = app
         self.user_id_field = history_user_id_field
         self.user_getter = history_user_getter
         self.user_setter = history_user_setter
         self.related_name = related_name
         self.use_base_model_db = use_base_model_db
+        self.history_manager = history_manager
+        self.historical_queryset = historical_queryset
         self.m2m_fields = m2m_fields
         self.m2m_fields_model_field_name = m2m_fields_model_field_name
 
         if isinstance(no_db_index, str):
             no_db_index = [no_db_index]
         self.no_db_index = no_db_index
 
@@ -211,15 +225,19 @@
         for field in m2m_fields:
             m2m_changed.connect(
                 partial(self.m2m_changed, attr=field.name),
                 sender=field.remote_field.through,
                 weak=False,
             )
 
-        descriptor = HistoryDescriptor(history_model)
+        descriptor = HistoryDescriptor(
+            history_model,
+            manager=self.history_manager,
+            queryset=self.historical_queryset,
+        )
         setattr(sender, self.manager_name, descriptor)
         sender._meta.simple_history_manager_attribute = self.manager_name
 
         for field in m2m_fields:
             m2m_model = self.create_history_m2m_model(
                 history_model, field.remote_field.through
             )
@@ -648,44 +666,46 @@
             self.create_historical_record(instance, "-", using=using)
 
     def get_change_reason_for_object(self, instance, history_type, using):
         """
         Get change reason for object.
         Customize this method to automatically fill change reason from context.
         """
-        return get_change_reason_from_object(instance)
+        return utils.get_change_reason_from_object(instance)
 
     def m2m_changed(self, instance, action, attr, pk_set, reverse, **_):
+        if not getattr(settings, "SIMPLE_HISTORY_ENABLED", True):
+            return
         if hasattr(instance, "skip_history_when_saving"):
             return
 
         if action in ("post_add", "post_remove", "post_clear"):
             # It should be safe to ~ this since the row must exist to modify m2m on it
             self.create_historical_record(instance, "~")
 
     def create_historical_record_m2ms(self, history_instance, instance):
         for field in history_instance._history_m2m_fields:
             m2m_history_model = self.m2m_models[field]
             original_instance = history_instance.instance
             through_model = getattr(original_instance, field.name).through
+            through_model_field_names = [f.name for f in through_model._meta.fields]
+            through_model_fk_field_names = [
+                f.name for f in through_model._meta.fields if isinstance(f, ForeignKey)
+            ]
 
             insert_rows = []
 
-            # `m2m_field_name()` is part of Django's internal API
-            through_field_name = field.m2m_field_name()
-
+            through_field_name = utils.get_m2m_field_name(field)
             rows = through_model.objects.filter(**{through_field_name: instance})
-
+            rows = rows.select_related(*through_model_fk_field_names)
             for row in rows:
                 insert_row = {"history": history_instance}
 
-                for through_model_field in through_model._meta.fields:
-                    insert_row[through_model_field.name] = getattr(
-                        row, through_model_field.name
-                    )
+                for field_name in through_model_field_names:
+                    insert_row[field_name] = getattr(row, field_name)
                 insert_rows.append(m2m_history_model(**insert_row))
 
             pre_create_historical_m2m_records.send(
                 sender=m2m_history_model,
                 rows=insert_rows,
                 history_instance=history_instance,
                 instance=instance,
@@ -796,14 +816,21 @@
     # field.deconstruct() here
     field.db_collation = None
 
     if field.primary_key or field.unique:
         # Unique fields can no longer be guaranteed unique,
         # but they should still be indexed for faster lookups.
         field.primary_key = False
+        # DEV: Remove this check (but keep the contents) when the minimum required
+        #      Django version is 5.1
+        if django.VERSION >= (5, 1):
+            field.unique = False
+        # (Django < 5.1) Can't set `unique` as it's a property, so set the backing field
+        # (Django >= 5.1) Set the backing field in addition to the cached property
+        #                 above, to cover all bases
         field._unique = False
         field.db_index = True
         field.serialize = True
 
 
 class HistoricForwardManyToOneDescriptor(ForwardManyToOneDescriptor):
     """
@@ -917,21 +944,42 @@
     def __get__(self, instance, owner):
         if instance is None:
             return self
         values = {f.attname: getattr(instance, f.attname) for f in self.fields_included}
         return self.model(**values)
 
 
-class HistoricalChanges:
-    def diff_against(self, old_history, excluded_fields=None, included_fields=None):
+class HistoricalChanges(ModelTypeHint):
+    def diff_against(
+        self,
+        old_history: "HistoricalChanges",
+        excluded_fields: Iterable[str] = None,
+        included_fields: Iterable[str] = None,
+        *,
+        foreign_keys_are_objs=False,
+    ) -> "ModelDelta":
+        """
+        :param old_history:
+        :param excluded_fields: The names of fields to exclude from diffing.
+               This takes precedence over ``included_fields``.
+        :param included_fields: The names of the only fields to include when diffing.
+               If not provided, all history-tracked fields will be included.
+        :param foreign_keys_are_objs: If ``False``, the returned diff will only contain
+               the raw PKs of any ``ForeignKey`` fields.
+               If ``True``, the diff will contain the actual related model objects
+               instead of just the PKs; deleted related objects will be instances of
+               ``DeletedObject``.
+               Note that passing ``True`` will necessarily query the database if the
+               related objects have not been prefetched (using e.g.
+               ``select_related()``).
+        """
         if not isinstance(old_history, type(self)):
             raise TypeError(
-                ("unsupported type(s) for diffing: " "'{}' and '{}'").format(
-                    type(self), type(old_history)
-                )
+                "unsupported type(s) for diffing:"
+                f" '{type(self)}' and '{type(old_history)}'"
             )
         if excluded_fields is None:
             excluded_fields = set()
 
         included_m2m_fields = {field.name for field in old_history._history_m2m_fields}
         if included_fields is None:
             included_fields = {f.name for f in old_history.tracked_fields if f.editable}
@@ -941,63 +989,176 @@
         fields = (
             set(included_fields)
             .difference(included_m2m_fields)
             .difference(excluded_fields)
         )
         m2m_fields = set(included_m2m_fields).difference(excluded_fields)
 
+        changes = [
+            *self._get_field_changes_for_diff(
+                old_history, fields, foreign_keys_are_objs
+            ),
+            *self._get_m2m_field_changes_for_diff(
+                old_history, m2m_fields, foreign_keys_are_objs
+            ),
+        ]
+        # Sort by field (attribute) name, to ensure a consistent order
+        changes.sort(key=lambda change: change.field)
+        changed_fields = [change.field for change in changes]
+        return ModelDelta(changes, changed_fields, old_history, self)
+
+    def _get_field_changes_for_diff(
+        self,
+        old_history: "HistoricalChanges",
+        fields: Iterable[str],
+        foreign_keys_are_objs: bool,
+    ) -> List["ModelChange"]:
+        """Helper method for ``diff_against()``."""
         changes = []
-        changed_fields = []
 
         old_values = model_to_dict(old_history, fields=fields)
-        current_values = model_to_dict(self, fields=fields)
+        new_values = model_to_dict(self, fields=fields)
 
         for field in fields:
             old_value = old_values[field]
-            current_value = current_values[field]
+            new_value = new_values[field]
 
-            if old_value != current_value:
-                changes.append(ModelChange(field, old_value, current_value))
-                changed_fields.append(field)
+            if old_value != new_value:
+                field_meta = self._meta.get_field(field)
+                if foreign_keys_are_objs and isinstance(field_meta, ForeignKey):
+                    # Set the fields to their related model objects instead of
+                    # the raw PKs from `model_to_dict()`
+                    def get_value(record, foreign_key):
+                        try:
+                            value = getattr(record, field)
+                        # `value` seems to be None (without raising this exception)
+                        # if the object has not been refreshed from the database
+                        except ObjectDoesNotExist:
+                            value = None
+
+                        if value is None:
+                            value = DeletedObject(field_meta.related_model, foreign_key)
+                        return value
 
-        # Separately compare m2m fields:
-        for field in m2m_fields:
-            # First retrieve a single item to get the field names from:
-            reference_history_m2m_item = (
-                getattr(old_history, field).first() or getattr(self, field).first()
-            )
-            history_field_names = []
-            if reference_history_m2m_item:
-                # Create a list of field names to compare against.
-                # The list is generated without the primary key of the intermediate
-                # table, the foreign key to the history record, and the actual 'history'
-                # field, to avoid false positives while diffing.
-                history_field_names = [
-                    f.name
-                    for f in reference_history_m2m_item._meta.fields
-                    if f.editable and f.name not in ["id", "m2m_history_id", "history"]
-                ]
+                    old_value = get_value(old_history, old_value)
+                    new_value = get_value(self, new_value)
+
+                change = ModelChange(field, old_value, new_value)
+                changes.append(change)
+
+        return changes
+
+    def _get_m2m_field_changes_for_diff(
+        self,
+        old_history: "HistoricalChanges",
+        m2m_fields: Iterable[str],
+        foreign_keys_are_objs: bool,
+    ) -> List["ModelChange"]:
+        """Helper method for ``diff_against()``."""
+        changes = []
 
-            old_rows = list(getattr(old_history, field).values(*history_field_names))
-            new_rows = list(getattr(self, field).values(*history_field_names))
+        for field in m2m_fields:
+            original_field_meta = self.instance_type._meta.get_field(field)
+            reverse_field_name = utils.get_m2m_reverse_field_name(original_field_meta)
+            # Sort the M2M rows by the related object, to ensure a consistent order
+            old_m2m_qs = getattr(old_history, field).order_by(reverse_field_name)
+            new_m2m_qs = getattr(self, field).order_by(reverse_field_name)
+            m2m_through_model_opts = new_m2m_qs.model._meta
+
+            # Create a list of field names to compare against.
+            # The list is generated without the PK of the intermediate (through)
+            # table, the foreign key to the history record, and the actual `history`
+            # field, to avoid false positives while diffing.
+            through_model_fields = [
+                f.name
+                for f in m2m_through_model_opts.fields
+                if f.editable and f.name not in ["id", "m2m_history_id", "history"]
+            ]
+            old_rows = list(old_m2m_qs.values(*through_model_fields))
+            new_rows = list(new_m2m_qs.values(*through_model_fields))
 
             if old_rows != new_rows:
+                if foreign_keys_are_objs:
+                    fk_fields = [
+                        f
+                        for f in through_model_fields
+                        if isinstance(m2m_through_model_opts.get_field(f), ForeignKey)
+                    ]
+
+                    # Set the through fields to their related model objects instead of
+                    # the raw PKs from `values()`
+                    def rows_with_foreign_key_objs(m2m_qs):
+                        def get_value(obj, through_field):
+                            try:
+                                value = getattr(obj, through_field)
+                            # If the related object has been deleted, `value` seems to
+                            # usually already be None instead of raising this exception
+                            except ObjectDoesNotExist:
+                                value = None
+
+                            if value is None:
+                                meta = m2m_through_model_opts.get_field(through_field)
+                                foreign_key = getattr(obj, meta.attname)
+                                value = DeletedObject(meta.related_model, foreign_key)
+                            return value
+
+                        # Replicate the format of the return value of QuerySet.values()
+                        return [
+                            {
+                                through_field: get_value(through_obj, through_field)
+                                for through_field in through_model_fields
+                            }
+                            for through_obj in m2m_qs.select_related(*fk_fields)
+                        ]
+
+                    old_rows = rows_with_foreign_key_objs(old_m2m_qs)
+                    new_rows = rows_with_foreign_key_objs(new_m2m_qs)
+
                 change = ModelChange(field, old_rows, new_rows)
                 changes.append(change)
-                changed_fields.append(field)
 
-        return ModelDelta(changes, changed_fields, old_history, self)
+        return changes
+
+
+@dataclass(frozen=True)
+class DeletedObject:
+    model: Type[models.Model]
+    pk: Any
+
+    def __str__(self):
+        deleted_model_str = _("Deleted %(type_name)s") % {
+            "type_name": self.model._meta.verbose_name,
+        }
+        return f"{deleted_model_str} (pk={self.pk})"
+
+
+# Either:
+# - The value of a foreign key field:
+#   - If ``foreign_keys_are_objs=True`` is passed to ``diff_against()``:
+#     Either the related object or ``DeletedObject``.
+#   - Otherwise:
+#     The PK of the related object.
+#
+# - The value of a many-to-many field:
+#   A list of dicts from the through model field names to either:
+#   - If ``foreign_keys_are_objs=True`` is passed to ``diff_against()``:
+#     Either the through model's related objects or ``DeletedObject``.
+#   - Otherwise:
+#     The PK of the through model's related objects.
+#
+# - Any of the other possible values of a model field.
+ModelChangeValue = Union[Any, DeletedObject, List[Dict[str, Union[Any, DeletedObject]]]]
 
 
+@dataclass(frozen=True)
 class ModelChange:
-    def __init__(self, field_name, old_value, new_value):
-        self.field = field_name
-        self.old = old_value
-        self.new = new_value
+    field: str
+    old: ModelChangeValue
+    new: ModelChangeValue
 
 
+@dataclass(frozen=True)
 class ModelDelta:
-    def __init__(self, changes, changed_fields, old_record, new_record):
-        self.changes = changes
-        self.changed_fields = changed_fields
-        self.old_record = old_record
-        self.new_record = new_record
+    changes: Sequence[ModelChange]
+    changed_fields: Sequence[str]
+    old_record: HistoricalChanges
+    new_record: HistoricalChanges
```

### Comparing `django-simple-history-3.5.0/simple_history/registry_tests/migration_test_app/migrations/0001_initial.py` & `django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/registry_tests/migration_test_app/migrations/0002_historicalmodelwithcustomattrforeignkey_modelwithcustomattrforeignkey.py` & `django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0002_historicalmodelwithcustomattrforeignkey_modelwithcustomattrforeignkey.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/registry_tests/migration_test_app/migrations/0003_alter_historicalmodelwithcustomattrforeignkey_options_and_more.py` & `django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0003_alter_historicalmodelwithcustomattrforeignkey_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/registry_tests/migration_test_app/migrations/0004_history_date_indexing.py` & `django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0004_history_date_indexing.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/registry_tests/migration_test_app/migrations/0005_historicalmodelwithcustomattronetoonefield_modelwithcustomattronetoonefield.py` & `django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0005_historicalmodelwithcustomattronetoonefield_modelwithcustomattronetoonefield.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/registry_tests/migration_test_app/migrations/0006_alter_historicalmodelwithcustomattronetoonefield_options_and_more.py` & `django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0006_alter_historicalmodelwithcustomattronetoonefield_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/registry_tests/migration_test_app/migrations/0007_alter_historicalmodelwithcustomattrforeignkey_options_and_more.py` & `django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/migrations/0007_alter_historicalmodelwithcustomattrforeignkey_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/registry_tests/migration_test_app/models.py` & `django_simple_history-3.6.0/simple_history/registry_tests/migration_test_app/models.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/registry_tests/tests.py` & `django_simple_history-3.6.0/simple_history/registry_tests/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     def test_register_separate_app(self):
         def get_history(model):
             return model.history
 
         self.assertRaises(AttributeError, get_history, User)
         self.assertEqual(len(User.histories.all()), 0)
-        user = User.objects.create(username="bob", password="pass")  # nosec
+        user = User.objects.create(username="bob", password="pass")
         self.assertEqual(len(User.histories.all()), 1)
         self.assertEqual(len(user.histories.all()), 1)
 
     def test_reregister(self):
         with self.assertRaises(exceptions.MultipleRegistrationsError):
             register(Restaurant, manager_name="again")
```

### Comparing `django-simple-history-3.5.0/simple_history/signals.py` & `django_simple_history-3.6.0/simple_history/signals.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/templates/simple_history/object_history_form.html` & `django_simple_history-3.6.0/simple_history/templates/simple_history/object_history_form.html`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/tests/admin.py` & `django_simple_history-3.6.0/simple_history/tests/admin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from django.contrib import admin
+from django.utils.safestring import SafeString, mark_safe
 
 from simple_history.admin import SimpleHistoryAdmin
+from simple_history.template_utils import HistoricalRecordContextHelper
 from simple_history.tests.external.models import ExternalModelWithCustomUserIdField
 
 from .models import (
     Book,
     Choice,
     ConcreteExternal,
     Document,
     Employee,
     FileModel,
     Paper,
     Person,
+    Place,
     Planet,
     Poll,
+    PollWithManyToMany,
 )
 
 
 class PersonAdmin(SimpleHistoryAdmin):
     def has_change_permission(self, request, obj=None):
         return False
 
@@ -39,18 +43,40 @@
 class PlanetAdmin(SimpleHistoryAdmin):
     def test_method(self, obj):
         return "test_method_value"
 
     history_list_display = ["title", "test_method"]
 
 
-admin.site.register(Poll, SimpleHistoryAdmin)
-admin.site.register(Choice, ChoiceAdmin)
-admin.site.register(Person, PersonAdmin)
+class HistoricalPollWithManyToManyContextHelper(HistoricalRecordContextHelper):
+    def prepare_delta_change_value(self, change, value):
+        display_value = super().prepare_delta_change_value(change, value)
+        if change.field == "places":
+            assert isinstance(display_value, list)
+            assert all(isinstance(place, Place) for place in display_value)
+
+            places = sorted(display_value, key=lambda place: place.name)
+            display_value = list(map(self.place_display, places))
+        return display_value
+
+    @staticmethod
+    def place_display(place: Place) -> SafeString:
+        return mark_safe(f"<b>{place.name}</b>")
+
+
+class PollWithManyToManyAdmin(SimpleHistoryAdmin):
+    def get_historical_record_context_helper(self, request, historical_record):
+        return HistoricalPollWithManyToManyContextHelper(self.model, historical_record)
+
+
 admin.site.register(Book, SimpleHistoryAdmin)
+admin.site.register(Choice, ChoiceAdmin)
+admin.site.register(ConcreteExternal, SimpleHistoryAdmin)
 admin.site.register(Document, SimpleHistoryAdmin)
-admin.site.register(Paper, SimpleHistoryAdmin)
 admin.site.register(Employee, SimpleHistoryAdmin)
-admin.site.register(ConcreteExternal, SimpleHistoryAdmin)
 admin.site.register(ExternalModelWithCustomUserIdField, SimpleHistoryAdmin)
 admin.site.register(FileModel, FileModelAdmin)
+admin.site.register(Paper, SimpleHistoryAdmin)
+admin.site.register(Person, PersonAdmin)
 admin.site.register(Planet, PlanetAdmin)
+admin.site.register(Poll, SimpleHistoryAdmin)
+admin.site.register(PollWithManyToMany, PollWithManyToManyAdmin)
```

### Comparing `django-simple-history-3.5.0/simple_history/tests/external/models.py` & `django_simple_history-3.6.0/simple_history/tests/external/models.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/tests/generated_file_checks/check_translations.py` & `django_simple_history-3.6.0/simple_history/tests/generated_file_checks/check_translations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import subprocess  # nosec
+import subprocess
 import sys
 from glob import glob
 from pathlib import Path
 
 import django
 from django.conf import settings
 from django.core.management import call_command
@@ -40,32 +40,32 @@
     # Delete the .mo files before regenerating them below
     delete_mo_files()
 
     log("Running 'compilemessages'...")
     call_command("compilemessages")
 
     log("\nRunning 'git status'...")
-    result = subprocess.run(  # nosec
+    result = subprocess.run(
         ["git", "status", "--porcelain"],
         check=True,
         stdout=subprocess.PIPE,
     )
-    assert result.stderr is None  # nosec
+    assert result.stderr is None
     stdout = result.stdout.decode()
     if stdout:
         log_err(f"Unexpected changes found in the workspace:\n\n{stdout}")
         if ".mo" in stdout:
             log_err(
                 "To properly update any '.mo' files,"
                 " try deleting them before running 'compilemessages'."
             )
         sys.exit(1)
     else:
         # Print the human-readable status to the console
-        subprocess.run(["git", "status"])  # nosec
+        subprocess.run(["git", "status"])
 
 
 if __name__ == "__main__":
     if not settings.configured:
         settings.configure(**get_default_settings())
     django.setup()
     main()
```

### Comparing `django-simple-history-3.5.0/simple_history/tests/models.py` & `django_simple_history-3.6.0/simple_history/tests/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from django.conf import settings
 from django.db import models
 from django.db.models.deletion import CASCADE
 from django.db.models.fields.related import ForeignKey
 from django.urls import reverse
 
 from simple_history import register
+from simple_history.manager import HistoricalQuerySet, HistoryManager
 from simple_history.models import HistoricalRecords, HistoricForeignKey
 
 from .custom_user.models import CustomUser as User
 from .external.models import AbstractExternal, AbstractExternal2, AbstractExternal3
 
 get_model = apps.get_model
 
@@ -151,14 +152,33 @@
     places = models.ManyToManyField("Place")
 
     history = HistoricalRecords(
         m2m_fields=[places], history_id_field=models.UUIDField(default=uuid.uuid4)
     )
 
 
+class PollQuerySet(HistoricalQuerySet):
+    def questions(self):
+        return self.filter(question__startswith="Question ")
+
+
+class PollManager(HistoryManager):
+    def low_ids(self):
+        return self.filter(id__lte=3)
+
+
+class PollWithQuerySetCustomizations(models.Model):
+    question = models.CharField(max_length=200)
+    pub_date = models.DateTimeField("date published")
+
+    history = HistoricalRecords(
+        history_manager=PollManager, historical_queryset=PollQuerySet
+    )
+
+
 class HistoricalRecordsWithExtraFieldM2M(HistoricalRecords):
     def get_extra_fields_m2m(self, model, through_model, fields):
         extra_fields = super().get_extra_fields_m2m(model, through_model, fields)
 
         def get_class_name(self):
             return self.__class__.__name__
```

### Comparing `django-simple-history-3.5.0/simple_history/tests/tests/test_admin.py` & `django_simple_history-3.6.0/simple_history/tests/tests/test_admin.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import Permission
 from django.contrib.messages.storage.fallback import FallbackStorage
 from django.test import TestCase
 from django.test.client import RequestFactory
 from django.test.utils import override_settings
 from django.urls import reverse
+from django.utils.dateparse import parse_datetime
 from django.utils.encoding import force_str
 
 from simple_history.admin import SimpleHistoryAdmin
 from simple_history.models import HistoricalRecords
+from simple_history.template_utils import HistoricalRecordContextHelper
 from simple_history.tests.external.models import ExternalModelWithCustomUserIdField
 from simple_history.tests.tests.utils import (
     PermissionAction,
     middleware_override_settings,
 )
 
 from ..models import (
@@ -25,16 +27,18 @@
     BucketData,
     BucketMember,
     Choice,
     ConcreteExternal,
     Employee,
     FileModel,
     Person,
+    Place,
     Planet,
     Poll,
+    PollWithManyToMany,
     State,
 )
 
 User = get_user_model()
 today = datetime(2021, 1, 1, 10, 0)
 tomorrow = today + timedelta(days=1)
 
@@ -82,14 +86,177 @@
         self.assertContains(response, "Poll object")
         self.assertContains(response, "Created")
         self.assertContains(response, "Changed by")
         self.assertContains(response, "Change reason")
         self.assertContains(response, "A random test reason")
         self.assertContains(response, self.user.username)
 
+    def test_history_list_contains_diff_changes(self):
+        self.login()
+        poll = Poll(question="why?", pub_date=today)
+        poll._history_user = self.user
+        poll.save()
+
+        poll_history_url = get_history_url(poll)
+        response = self.client.get(poll_history_url)
+        self.assertContains(response, "Changes")
+        # The poll hasn't had any of its fields changed after creation,
+        # so these values should not be present
+        self.assertNotContains(response, "Question:")
+        self.assertNotContains(response, "why?")
+        self.assertNotContains(response, "Date published:")
+
+        poll.question = "how?"
+        poll.save()
+        response = self.client.get(poll_history_url)
+        self.assertContains(response, "Question:")
+        self.assertContains(response, "why?")
+        self.assertContains(response, "how?")
+        self.assertNotContains(response, "Date published:")
+
+        poll.question = "when?"
+        poll.pub_date = parse_datetime("2024-04-04 04:04:04")
+        poll.save()
+        response = self.client.get(poll_history_url)
+        self.assertContains(response, "Question:")
+        self.assertContains(response, "why?")
+        self.assertContains(response, "how?")
+        self.assertContains(response, "when?")
+        self.assertContains(response, "Date published:")
+        self.assertContains(response, "2021-01-01 10:00:00")
+        self.assertContains(response, "2024-04-04 04:04:04")
+
+    def test_history_list_contains_diff_changes_for_foreign_key_fields(self):
+        self.login()
+        poll1 = Poll.objects.create(question="why?", pub_date=today)
+        poll1_pk = poll1.pk
+        poll2 = Poll.objects.create(question="how?", pub_date=today)
+        poll2_pk = poll2.pk
+        choice = Choice(poll=poll1, votes=1)
+        choice._history_user = self.user
+        choice.save()
+        choice_history_url = get_history_url(choice)
+
+        # Before changing the poll:
+        response = self.client.get(choice_history_url)
+        self.assertNotContains(response, "Poll:")
+        expected_old_poll = f"Poll object ({poll1_pk})"
+        self.assertNotContains(response, expected_old_poll)
+        expected_new_poll = f"Poll object ({poll2_pk})"
+        self.assertNotContains(response, expected_new_poll)
+
+        # After changing the poll:
+        choice.poll = poll2
+        choice.save()
+        response = self.client.get(choice_history_url)
+        self.assertContains(response, "Poll:")
+        self.assertContains(response, expected_old_poll)
+        self.assertContains(response, expected_new_poll)
+
+        # After deleting all polls:
+        Poll.objects.all().delete()
+        response = self.client.get(choice_history_url)
+        self.assertContains(response, "Poll:")
+        self.assertContains(response, f"Deleted poll (pk={poll1_pk})")
+        self.assertContains(response, f"Deleted poll (pk={poll2_pk})")
+
+    @patch(
+        # Test without the customization in PollWithManyToMany's admin class
+        "simple_history.tests.admin.HistoricalPollWithManyToManyContextHelper",
+        HistoricalRecordContextHelper,
+    )
+    def test_history_list_contains_diff_changes_for_m2m_fields(self):
+        self.login()
+        poll = PollWithManyToMany(question="why?", pub_date=today)
+        poll._history_user = self.user
+        poll.save()
+        place1 = Place.objects.create(name="Here")
+        place1_pk = place1.pk
+        place2 = Place.objects.create(name="There")
+        place2_pk = place2.pk
+        poll_history_url = get_history_url(poll)
+
+        # Before adding places:
+        response = self.client.get(poll_history_url)
+        self.assertNotContains(response, "Places:")
+        expected_old_places = "[]"
+        self.assertNotContains(response, expected_old_places)
+        expected_new_places = (
+            f"[Place object ({place1_pk}), Place object ({place2_pk})]"
+        )
+        self.assertNotContains(response, expected_new_places)
+
+        # After adding places:
+        poll.places.add(place1, place2)
+        response = self.client.get(poll_history_url)
+        self.assertContains(response, "Places:")
+        self.assertContains(response, expected_old_places)
+        self.assertContains(response, expected_new_places)
+
+        # After deleting all places:
+        Place.objects.all().delete()
+        response = self.client.get(poll_history_url)
+        self.assertContains(response, "Places:")
+        self.assertContains(response, expected_old_places)
+        expected_new_places = (
+            f"[Deleted place (pk={place1_pk}), Deleted place (pk={place2_pk})]"
+        )
+        self.assertContains(response, expected_new_places)
+
+    def test_history_list_doesnt_contain_too_long_diff_changes(self):
+        self.login()
+
+        def create_and_change_poll(*, initial_question, changed_question) -> Poll:
+            poll = Poll(question=initial_question, pub_date=today)
+            poll._history_user = self.user
+            poll.save()
+            poll.question = changed_question
+            poll.save()
+            return poll
+
+        repeated_chars = (
+            HistoricalRecordContextHelper.DEFAULT_MAX_DISPLAYED_DELTA_CHANGE_CHARS
+        )
+
+        # Number of characters right on the limit
+        poll1 = create_and_change_poll(
+            initial_question="A" * repeated_chars,
+            changed_question="B" * repeated_chars,
+        )
+        response = self.client.get(get_history_url(poll1))
+        self.assertContains(response, "Question:")
+        self.assertContains(response, "A" * repeated_chars)
+        self.assertContains(response, "B" * repeated_chars)
+
+        # Number of characters just over the limit
+        poll2 = create_and_change_poll(
+            initial_question="A" * (repeated_chars + 1),
+            changed_question="B" * (repeated_chars + 1),
+        )
+        response = self.client.get(get_history_url(poll2))
+        self.assertContains(response, "Question:")
+        self.assertContains(response, f"{'A' * 61}[35 chars]AAAAA")
+        self.assertContains(response, f"{'B' * 61}[35 chars]BBBBB")
+
+    def test_overriding__historical_record_context_helper__with_custom_m2m_string(self):
+        self.login()
+
+        place1 = Place.objects.create(name="Place 1")
+        place2 = Place.objects.create(name="Place 2")
+        place3 = Place.objects.create(name="Place 3")
+        poll = PollWithManyToMany.objects.create(question="why?", pub_date=today)
+        poll.places.add(place1, place2)
+        poll.places.set([place3])
+
+        response = self.client.get(get_history_url(poll))
+        self.assertContains(response, "Places:")
+        self.assertContains(response, "[]")
+        self.assertContains(response, "[<b>Place 1</b>, <b>Place 2</b>]")
+        self.assertContains(response, "[<b>Place 3</b>]")
+
     def test_history_list_custom_fields(self):
         model_name = self.user._meta.model_name
         self.assertEqual(model_name, "customuser")
         self.login()
         poll = Poll(question="why?", pub_date=today)
         poll._history_user = self.user
         poll.save()
```

### Comparing `django-simple-history-3.5.0/simple_history/tests/tests/test_commands.py` & `django_simple_history-3.6.0/simple_history/tests/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/tests/tests/test_index.py` & `django_simple_history-3.6.0/simple_history/tests/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/tests/tests/test_manager.py` & `django_simple_history-3.6.0/simple_history/tests/tests/test_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import django
 from django.contrib.auth import get_user_model
 from django.db import IntegrityError
 from django.test import TestCase, override_settings, skipUnlessDBFeature
 
 from simple_history.manager import SIMPLE_HISTORY_REVERSE_ATTR_NAME
 
-from ..models import Document, Poll, RankedDocument
+from ..models import Choice, Document, Poll, RankedDocument
 
 User = get_user_model()
 
 
 class AsOfTest(TestCase):
     model = Document
 
@@ -367,7 +367,41 @@
             all(
                 [
                     history.history_change_reason == "reason"
                     for history in Poll.history.all()
                 ]
             )
         )
+
+
+class PrefetchingMethodsTestCase(TestCase):
+    def setUp(self):
+        d = datetime(3021, 1, 1, 10, 0)
+        self.poll1 = Poll.objects.create(question="why?", pub_date=d)
+        self.poll2 = Poll.objects.create(question="how?", pub_date=d)
+        self.choice1 = Choice.objects.create(poll=self.poll1, votes=1)
+        self.choice2 = Choice.objects.create(poll=self.poll1, votes=2)
+        self.choice3 = Choice.objects.create(poll=self.poll2, votes=3)
+
+    def test__select_related_history_tracked_objs__prefetches_expected_objects(self):
+        num_choices = Choice.objects.count()
+        self.assertEqual(num_choices, 3)
+
+        def access_related_objs(records):
+            for record in records:
+                self.assertIsInstance(record.poll, Poll)
+
+        # Without prefetching:
+        with self.assertNumQueries(1):
+            historical_records = Choice.history.all()
+            self.assertEqual(len(historical_records), num_choices)
+        with self.assertNumQueries(num_choices):
+            access_related_objs(historical_records)
+
+        # With prefetching:
+        with self.assertNumQueries(1):
+            historical_records = (
+                Choice.history.all()._select_related_history_tracked_objs()
+            )
+            self.assertEqual(len(historical_records), num_choices)
+        with self.assertNumQueries(0):
+            access_related_objs(historical_records)
```

### Comparing `django-simple-history-3.5.0/simple_history/tests/tests/test_middleware.py` & `django_simple_history-3.6.0/simple_history/tests/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/tests/tests/test_models.py` & `django_simple_history-3.6.0/simple_history/tests/tests/test_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+import dataclasses
 import unittest
 import uuid
 import warnings
 from datetime import datetime, timedelta
 
-import django
 from django.apps import apps
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.core.exceptions import ImproperlyConfigured, ObjectDoesNotExist
 from django.core.files.base import ContentFile
 from django.db import IntegrityError, models
 from django.db.models.fields.proxy import OrderWrt
@@ -15,24 +15,25 @@
 from django.urls import reverse
 from django.utils import timezone
 
 from simple_history import register
 from simple_history.exceptions import RelatedNameConflictError
 from simple_history.models import (
     SIMPLE_HISTORY_REVERSE_ATTR_NAME,
+    DeletedObject,
     HistoricalRecords,
     ModelChange,
+    ModelDelta,
     is_historic,
     to_historic,
 )
 from simple_history.signals import (
     pre_create_historical_m2m_records,
     pre_create_historical_record,
 )
-from simple_history.tests.custom_user.models import CustomUser
 from simple_history.tests.tests.utils import (
     database_router_override_settings,
     database_router_override_settings_history_in_diff_db,
     middleware_override_settings,
 )
 from simple_history.utils import get_history_model_for_model, update_change_reason
 
@@ -82,15 +83,14 @@
     ModelWithFkToModelWithHistoryUsingBaseModelDb,
     ModelWithHistoryInDifferentDb,
     ModelWithHistoryUsingBaseModelDb,
     ModelWithMultipleNoDBIndex,
     ModelWithSingleNoDBIndexUnique,
     MultiOneToOne,
     MyOverrideModelNameRegisterMethod1,
-    OverrideModelNameAsCallable,
     OverrideModelNameUsingBaseModel1,
     Person,
     Place,
     Poll,
     PollChildBookWithManyToMany,
     PollChildRestaurantWithManyToMany,
     PollInfo,
@@ -99,14 +99,15 @@
     PollWithExcludedFKField,
     PollWithExcludeFields,
     PollWithHistoricalIPAddress,
     PollWithManyToMany,
     PollWithManyToManyCustomHistoryID,
     PollWithManyToManyWithIPAddress,
     PollWithNonEditableField,
+    PollWithQuerySetCustomizations,
     PollWithSelfManyToMany,
     PollWithSeveralManyToMany,
     Province,
     Restaurant,
     SelfFK,
     Series,
     SeriesWork,
@@ -692,19 +693,21 @@
     def test_history_diff_includes_changed_fields(self):
         p = Poll.objects.create(question="what's up?", pub_date=today)
         p.question = "what's up, man?"
         p.save()
         new_record, old_record = p.history.all()
         with self.assertNumQueries(0):
             delta = new_record.diff_against(old_record)
-        expected_change = ModelChange("question", "what's up?", "what's up, man")
-        self.assertEqual(delta.changed_fields, ["question"])
-        self.assertEqual(delta.old_record, old_record)
-        self.assertEqual(delta.new_record, new_record)
-        self.assertEqual(expected_change.field, delta.changes[0].field)
+        expected_delta = ModelDelta(
+            [ModelChange("question", "what's up?", "what's up, man?")],
+            ["question"],
+            old_record,
+            new_record,
+        )
+        self.assertEqual(delta, expected_delta)
 
     def test_history_diff_does_not_include_unchanged_fields(self):
         p = Poll.objects.create(question="what's up?", pub_date=today)
         p.question = "what's up, man?"
         p.save()
         new_record, old_record = p.history.all()
         with self.assertNumQueries(0):
@@ -715,19 +718,156 @@
         r = InheritedRestaurant.objects.create(name="McDonna", serves_hot_dogs=False)
         # change base model field
         r.name = "DonnutsKing"
         r.save()
         new_record, old_record = r.history.all()
         with self.assertNumQueries(0):
             delta = new_record.diff_against(old_record)
-        expected_change = ModelChange("name", "McDonna", "DonnutsKing")
-        self.assertEqual(delta.changed_fields, ["name"])
-        self.assertEqual(delta.old_record, old_record)
-        self.assertEqual(delta.new_record, new_record)
-        self.assertEqual(expected_change.field, delta.changes[0].field)
+        expected_delta = ModelDelta(
+            [ModelChange("name", "McDonna", "DonnutsKing")],
+            ["name"],
+            old_record,
+            new_record,
+        )
+        self.assertEqual(delta, expected_delta)
+
+    def test_history_diff_arg__foreign_keys_are_objs__returns_expected_fk_values(self):
+        poll1 = Poll.objects.create(question="why?", pub_date=today)
+        poll1_pk = poll1.pk
+        poll2 = Poll.objects.create(question="how?", pub_date=tomorrow)
+        poll2_pk = poll2.pk
+        choice = Choice.objects.create(poll=poll1, choice="hmm", votes=3)
+        choice.poll = poll2
+        choice.choice = "idk"
+        choice.votes = 0
+        choice.save()
+        new_record, old_record = choice.history.all()
+
+        # Test with the default value of `foreign_keys_are_objs`
+        with self.assertNumQueries(0):
+            delta = new_record.diff_against(old_record)
+        expected_pk_changes = [
+            ModelChange("choice", "hmm", "idk"),
+            ModelChange("poll", poll1_pk, poll2_pk),
+            ModelChange("votes", 3, 0),
+        ]
+        expected_pk_delta = ModelDelta(
+            expected_pk_changes, ["choice", "poll", "votes"], old_record, new_record
+        )
+        self.assertEqual(delta, expected_pk_delta)
+
+        # Test with `foreign_keys_are_objs=True`
+        with self.assertNumQueries(2):  # Once for each poll in the new record
+            delta = new_record.diff_against(old_record, foreign_keys_are_objs=True)
+        choice_changes, _poll_changes, votes_changes = expected_pk_changes
+        # The PKs should now instead be their corresponding model objects
+        expected_obj_changes = [
+            choice_changes,
+            ModelChange("poll", poll1, poll2),
+            votes_changes,
+        ]
+        expected_obj_delta = dataclasses.replace(
+            expected_pk_delta, changes=expected_obj_changes
+        )
+        self.assertEqual(delta, expected_obj_delta)
+
+        # --- Delete the polls and do the same tests again ---
+
+        Poll.objects.all().delete()
+        old_record.refresh_from_db()
+        new_record.refresh_from_db()
+
+        # Test with the default value of `foreign_keys_are_objs`
+        with self.assertNumQueries(0):
+            delta = new_record.diff_against(old_record)
+        self.assertEqual(delta, expected_pk_delta)
+
+        # Test with `foreign_keys_are_objs=True`
+        with self.assertNumQueries(2):  # Once for each poll in the new record
+            delta = new_record.diff_against(old_record, foreign_keys_are_objs=True)
+        # The model objects should now instead be instances of `DeletedObject`
+        expected_obj_changes = [
+            choice_changes,
+            ModelChange(
+                "poll", DeletedObject(Poll, poll1_pk), DeletedObject(Poll, poll2_pk)
+            ),
+            votes_changes,
+        ]
+        expected_obj_delta = dataclasses.replace(
+            expected_pk_delta, changes=expected_obj_changes
+        )
+        self.assertEqual(delta, expected_obj_delta)
+
+    def test_history_diff_arg__foreign_keys_are_objs__returns_expected_m2m_values(self):
+        poll = PollWithManyToMany.objects.create(question="why?", pub_date=today)
+        place1 = Place.objects.create(name="Here")
+        place1_pk = place1.pk
+        place2 = Place.objects.create(name="There")
+        place2_pk = place2.pk
+        poll.places.add(place1, place2)
+        new_record, old_record = poll.history.all()
+
+        # Test with the default value of `foreign_keys_are_objs`
+        with self.assertNumQueries(2):  # Once for each record
+            delta = new_record.diff_against(old_record)
+        expected_pk_change = ModelChange(
+            "places",
+            [],
+            [
+                {"pollwithmanytomany": poll.pk, "place": place1_pk},
+                {"pollwithmanytomany": poll.pk, "place": place2_pk},
+            ],
+        )
+        expected_pk_delta = ModelDelta(
+            [expected_pk_change], ["places"], old_record, new_record
+        )
+        self.assertEqual(delta, expected_pk_delta)
+
+        # Test with `foreign_keys_are_objs=True`
+        with self.assertNumQueries(2 * 2):  # Twice for each record
+            delta = new_record.diff_against(old_record, foreign_keys_are_objs=True)
+        # The PKs should now instead be their corresponding model objects
+        expected_obj_change = dataclasses.replace(
+            expected_pk_change,
+            new=[
+                {"pollwithmanytomany": poll, "place": place1},
+                {"pollwithmanytomany": poll, "place": place2},
+            ],
+        )
+        expected_obj_delta = dataclasses.replace(
+            expected_pk_delta, changes=[expected_obj_change]
+        )
+        self.assertEqual(delta, expected_obj_delta)
+
+        # --- Delete the places and do the same tests again ---
+
+        Place.objects.all().delete()
+        old_record.refresh_from_db()
+        new_record.refresh_from_db()
+
+        # Test with the default value of `foreign_keys_are_objs`
+        with self.assertNumQueries(2):  # Once for each record
+            delta = new_record.diff_against(old_record)
+        self.assertEqual(delta, expected_pk_delta)
+
+        # Test with `foreign_keys_are_objs=True`
+        with self.assertNumQueries(2 * 2):  # Twice for each record
+            delta = new_record.diff_against(old_record, foreign_keys_are_objs=True)
+        # The model objects should now instead be instances of `DeletedObject`
+        expected_obj_change = dataclasses.replace(
+            expected_obj_change,
+            new=[
+                {"pollwithmanytomany": poll, "place": DeletedObject(Place, place1_pk)},
+                {"pollwithmanytomany": poll, "place": DeletedObject(Place, place2_pk)},
+            ],
+        )
+        expected_obj_delta = dataclasses.replace(
+            expected_obj_delta, changes=[expected_obj_change]
+        )
+        self.assertEqual(delta, expected_obj_delta)
 
     def test_history_table_name_is_not_inherited(self):
         def assert_table_name(obj, expected_table_name):
             history_model = obj.history.model
             self.assertEqual(
                 history_model.__name__, f"Historical{obj._meta.model.__name__}"
             )
@@ -754,56 +894,101 @@
     def test_history_diff_with_excluded_fields(self):
         p = Poll.objects.create(question="what's up?", pub_date=today)
         p.question = "what's up, man?"
         p.save()
         new_record, old_record = p.history.all()
         with self.assertNumQueries(0):
             delta = new_record.diff_against(old_record, excluded_fields=("question",))
-        self.assertEqual(delta.changed_fields, [])
-        self.assertEqual(delta.changes, [])
+        expected_delta = ModelDelta([], [], old_record, new_record)
+        self.assertEqual(delta, expected_delta)
 
     def test_history_diff_with_included_fields(self):
         p = Poll.objects.create(question="what's up?", pub_date=today)
         p.question = "what's up, man?"
         p.save()
         new_record, old_record = p.history.all()
         with self.assertNumQueries(0):
             delta = new_record.diff_against(old_record, included_fields=[])
-        self.assertEqual(delta.changed_fields, [])
-        self.assertEqual(delta.changes, [])
+        expected_delta = ModelDelta([], [], old_record, new_record)
+        self.assertEqual(delta, expected_delta)
 
         with self.assertNumQueries(0):
             delta = new_record.diff_against(old_record, included_fields=["question"])
-        self.assertEqual(delta.changed_fields, ["question"])
-        self.assertEqual(len(delta.changes), 1)
+        expected_delta = dataclasses.replace(
+            expected_delta,
+            changes=[ModelChange("question", "what's up?", "what's up, man?")],
+            changed_fields=["question"],
+        )
+        self.assertEqual(delta, expected_delta)
 
     def test_history_diff_with_non_editable_field(self):
         p = PollWithNonEditableField.objects.create(
             question="what's up?", pub_date=today
         )
         p.question = "what's up, man?"
         p.save()
         new_record, old_record = p.history.all()
         with self.assertNumQueries(0):
             delta = new_record.diff_against(old_record)
-        self.assertEqual(delta.changed_fields, ["question"])
-        self.assertEqual(len(delta.changes), 1)
+        expected_delta = ModelDelta(
+            [ModelChange("question", "what's up?", "what's up, man?")],
+            ["question"],
+            old_record,
+            new_record,
+        )
+        self.assertEqual(delta, expected_delta)
 
     def test_history_with_unknown_field(self):
         p = Poll.objects.create(question="what's up?", pub_date=today)
         p.question = "what's up, man?"
         p.save()
         new_record, old_record = p.history.all()
         with self.assertRaises(KeyError):
             with self.assertNumQueries(0):
                 new_record.diff_against(old_record, included_fields=["unknown_field"])
 
         with self.assertNumQueries(0):
             new_record.diff_against(old_record, excluded_fields=["unknown_field"])
 
+    def test_history_with_custom_queryset(self):
+        PollWithQuerySetCustomizations.objects.create(
+            id=1, pub_date=today, question="Question 1"
+        )
+        PollWithQuerySetCustomizations.objects.create(
+            id=2, pub_date=today, question="Low Id"
+        )
+        PollWithQuerySetCustomizations.objects.create(
+            id=10, pub_date=today, question="Random"
+        )
+
+        self.assertEqual(
+            set(
+                PollWithQuerySetCustomizations.history.low_ids().values_list(
+                    "question", flat=True
+                )
+            ),
+            {"Question 1", "Low Id"},
+        )
+        self.assertEqual(
+            set(
+                PollWithQuerySetCustomizations.history.questions().values_list(
+                    "question", flat=True
+                )
+            ),
+            {"Question 1"},
+        )
+        self.assertEqual(
+            set(
+                PollWithQuerySetCustomizations.history.low_ids()
+                .questions()
+                .values_list("question", flat=True)
+            ),
+            {"Question 1"},
+        )
+
 
 class GetPrevRecordAndNextRecordTestCase(TestCase):
     def assertRecordsMatch(self, record_a, record_b):
         self.assertEqual(record_a, record_b)
         self.assertEqual(record_a.question, record_b.question)
 
     def setUp(self):
@@ -963,14 +1148,22 @@
             ["id", "question", "pub_date"],
         )
         assert_tracked_fields_equal(
             PollWithHistoricalIPAddress,
             ["id", "question", "pub_date"],
         )
         assert_tracked_fields_equal(
+            PollWithManyToMany,
+            ["id", "question", "pub_date"],
+        )
+        assert_tracked_fields_equal(
+            Choice,
+            ["id", "poll", "choice", "votes"],
+        )
+        assert_tracked_fields_equal(
             ModelWithCustomAttrOneToOneField,
             ["id", "poll"],
         )
 
     def test_create_history_model_with_one_to_one_field_to_integer_field(self):
         try:
             self.create_history_model(AdminProfile, False)
@@ -1881,15 +2074,14 @@
 
         self.assertEqual(poll1.history.all().count(), 2)
 
 
 class ManyToManyWithSignalsTest(TestCase):
     def setUp(self):
         self.model = PollWithManyToManyWithIPAddress
-        # self.historical_through_model = self.model.history.
         self.places = (
             Place.objects.create(name="London"),
             Place.objects.create(name="Paris"),
         )
         self.poll = self.model.objects.create(question="what's up?", pub_date=today)
         pre_create_historical_m2m_records.connect(
             add_static_history_ip_address_on_m2m,
@@ -1921,18 +2113,36 @@
     def test_diff(self):
         self.poll.places.clear()
         self.poll.places.add(*self.places)
 
         new = self.poll.history.first()
         old = new.prev_record
 
-        delta = new.diff_against(old)
-
-        self.assertEqual("places", delta.changes[0].field)
-        self.assertEqual(2, len(delta.changes[0].new))
+        with self.assertNumQueries(2):  # Once for each record
+            delta = new.diff_against(old)
+        expected_delta = ModelDelta(
+            [
+                ModelChange(
+                    "places",
+                    [],
+                    [
+                        {
+                            "pollwithmanytomanywithipaddress": self.poll.pk,
+                            "place": place.pk,
+                            "ip_address": "192.168.0.1",
+                        }
+                        for place in self.places
+                    ],
+                )
+            ],
+            ["places"],
+            old,
+            new,
+        )
+        self.assertEqual(delta, expected_delta)
 
 
 class ManyToManyCustomIDTest(TestCase):
     def setUp(self):
         self.model = PollWithManyToManyCustomHistoryID
         self.history_model = self.model.history.model
         self.place = Place.objects.create(name="Home")
@@ -2162,14 +2372,51 @@
         # Most recent should only have the first Place remaining
         m2m_record = self.poll.history.all()[0]
         self.assertEqual(m2m_record.places.all().count(), 1)
 
         historical_place = m2m_record.places.first()
         self.assertEqual(historical_place.place, self.place)
 
+    def test_add_remove_set_and_clear_methods_make_expected_num_queries(self):
+        for num_places in (1, 2, 4):
+            with self.subTest(num_places=num_places):
+                start_pk = 100 + num_places
+                places = Place.objects.bulk_create(
+                    Place(pk=pk, name=f"Place {pk}")
+                    for pk in range(start_pk, start_pk + num_places)
+                )
+                self.assertEqual(len(places), num_places)
+                self.assertEqual(self.poll.places.count(), 0)
+
+                # The number of queries should stay the same, regardless of
+                # the number of places added or removed
+                with self.assertNumQueries(5):
+                    self.poll.places.add(*places)
+                self.assertEqual(self.poll.places.count(), num_places)
+
+                with self.assertNumQueries(3):
+                    self.poll.places.remove(*places)
+                self.assertEqual(self.poll.places.count(), 0)
+
+                with self.assertNumQueries(6):
+                    self.poll.places.set(places)
+                self.assertEqual(self.poll.places.count(), num_places)
+
+                with self.assertNumQueries(4):
+                    self.poll.places.set([])
+                self.assertEqual(self.poll.places.count(), 0)
+
+                with self.assertNumQueries(5):
+                    self.poll.places.add(*places)
+                self.assertEqual(self.poll.places.count(), num_places)
+
+                with self.assertNumQueries(3):
+                    self.poll.places.clear()
+                self.assertEqual(self.poll.places.count(), 0)
+
     def test_m2m_relation(self):
         # Ensure only the correct M2Ms are saved and returned for history objects
         poll_2 = PollWithManyToMany.objects.create(question="Why", pub_date=today)
         place_2 = Place.objects.create(name="Place 2")
 
         poll_2.places.add(self.place)
         poll_2.places.add(place_2)
@@ -2197,68 +2444,82 @@
         place_2 = Place.objects.create(name="Place 2")
 
         skip_poll.places.add(place_2)
 
         self.assertEqual(skip_poll.history.all().count(), 2)
         self.assertEqual(skip_poll.history.all()[0].places.count(), 2)
 
+    @override_settings(SIMPLE_HISTORY_ENABLED=False)
+    def test_saving_with_disabled_history_doesnt_create_records(self):
+        # 1 from `setUp()`
+        self.assertEqual(PollWithManyToMany.history.count(), 1)
+
+        poll = PollWithManyToMany.objects.create(
+            question="skip history?", pub_date=today
+        )
+        poll.question = "huh?"
+        poll.save()
+        poll.places.add(self.place)
+
+        self.assertEqual(poll.history.count(), 0)
+        # The count should not have changed
+        self.assertEqual(PollWithManyToMany.history.count(), 1)
+
     def test_diff_against(self):
         self.poll.places.add(self.place)
         add_record, create_record = self.poll.history.all()
 
-        delta = add_record.diff_against(create_record)
+        with self.assertNumQueries(2):  # Once for each record
+            delta = add_record.diff_against(create_record)
         expected_change = ModelChange(
             "places", [], [{"pollwithmanytomany": self.poll.pk, "place": self.place.pk}]
         )
-        self.assertEqual(delta.changed_fields, ["places"])
-        self.assertEqual(delta.old_record, create_record)
-        self.assertEqual(delta.new_record, add_record)
-        self.assertEqual(expected_change.field, delta.changes[0].field)
-
-        self.assertListEqual(expected_change.new, delta.changes[0].new)
-        self.assertListEqual(expected_change.old, delta.changes[0].old)
-
-        delta = add_record.diff_against(create_record, included_fields=["places"])
-        self.assertEqual(delta.changed_fields, ["places"])
-        self.assertEqual(delta.old_record, create_record)
-        self.assertEqual(delta.new_record, add_record)
-        self.assertEqual(expected_change.field, delta.changes[0].field)
-
-        delta = add_record.diff_against(create_record, excluded_fields=["places"])
-        self.assertEqual(delta.changed_fields, [])
-        self.assertEqual(delta.old_record, create_record)
-        self.assertEqual(delta.new_record, add_record)
+        expected_delta = ModelDelta(
+            [expected_change], ["places"], create_record, add_record
+        )
+        self.assertEqual(delta, expected_delta)
+
+        with self.assertNumQueries(2):  # Once for each record
+            delta = add_record.diff_against(create_record, included_fields=["places"])
+        self.assertEqual(delta, expected_delta)
+
+        with self.assertNumQueries(0):
+            delta = add_record.diff_against(create_record, excluded_fields=["places"])
+        expected_delta = dataclasses.replace(
+            expected_delta, changes=[], changed_fields=[]
+        )
+        self.assertEqual(delta, expected_delta)
 
         self.poll.places.clear()
 
         # First and third records are effectively the same.
         del_record, add_record, create_record = self.poll.history.all()
-        delta = del_record.diff_against(create_record)
+        with self.assertNumQueries(2):  # Once for each record
+            delta = del_record.diff_against(create_record)
         self.assertNotIn("places", delta.changed_fields)
 
+        with self.assertNumQueries(2):  # Once for each record
+            delta = del_record.diff_against(add_record)
         # Second and third should have the same diffs as first and second, but with
         # old and new reversed
         expected_change = ModelChange(
             "places", [{"place": self.place.pk, "pollwithmanytomany": self.poll.pk}], []
         )
-        delta = del_record.diff_against(add_record)
-        self.assertEqual(delta.changed_fields, ["places"])
-        self.assertEqual(delta.old_record, add_record)
-        self.assertEqual(delta.new_record, del_record)
-        self.assertEqual(expected_change.field, delta.changes[0].field)
-        self.assertListEqual(expected_change.new, delta.changes[0].new)
-        self.assertListEqual(expected_change.old, delta.changes[0].old)
+        expected_delta = ModelDelta(
+            [expected_change], ["places"], add_record, del_record
+        )
+        self.assertEqual(delta, expected_delta)
 
 
 @override_settings(**database_router_override_settings)
 class MultiDBExplicitHistoryUserIDTest(TestCase):
     databases = {"default", "other"}
 
     def setUp(self):
-        self.user = get_user_model().objects.create(  # nosec
+        self.user = get_user_model().objects.create(
             username="username", email="username@test.com", password="top_secret"
         )
 
     def test_history_user_with_fk_in_different_db_raises_value_error(self):
         instance = ExternalModel(name="random_name")
         instance._history_user = self.user
         with self.assertRaises(ValueError):
@@ -2291,18 +2552,18 @@
 
         self.assertEqual(user_id, instance.history.first().history_user_id)
         self.assertIsNone(instance.history.first().history_user)
 
 
 class RelatedNameTest(TestCase):
     def setUp(self):
-        self.user_one = get_user_model().objects.create(  # nosec
+        self.user_one = get_user_model().objects.create(
             username="username_one", email="first@user.com", password="top_secret"
         )
-        self.user_two = get_user_model().objects.create(  # nosec
+        self.user_two = get_user_model().objects.create(
             username="username_two", email="second@user.com", password="top_secret"
         )
 
         self.one = Street(name="Test Street")
         self.one._history_user = self.user_one
         self.one.save()
```

### Comparing `django-simple-history-3.5.0/simple_history/tests/tests/test_signals.py` & `django_simple_history-3.6.0/simple_history/tests/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/tests/tests/test_utils.py` & `django_simple_history-3.6.0/simple_history/tests/tests/test_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import unittest
 from datetime import datetime
 from unittest import skipUnless
 from unittest.mock import Mock, patch
 
 import django
 from django.contrib.auth import get_user_model
 from django.db import IntegrityError, transaction
@@ -10,30 +11,96 @@
 
 from simple_history.exceptions import AlternativeManagerError, NotHistoricalModelError
 from simple_history.tests.models import (
     BulkCreateManyToManyModel,
     Document,
     Place,
     Poll,
+    PollChildBookWithManyToMany,
+    PollChildRestaurantWithManyToMany,
     PollWithAlternativeManager,
     PollWithExcludeFields,
     PollWithHistoricalSessionAttr,
+    PollWithManyToMany,
+    PollWithManyToManyCustomHistoryID,
+    PollWithManyToManyWithIPAddress,
+    PollWithSelfManyToMany,
+    PollWithSeveralManyToMany,
     PollWithUniqueQuestion,
     Street,
 )
 from simple_history.utils import (
     bulk_create_with_history,
     bulk_update_with_history,
     get_history_manager_for_model,
+    get_history_model_for_model,
+    get_m2m_field_name,
+    get_m2m_reverse_field_name,
     update_change_reason,
 )
 
 User = get_user_model()
 
 
+class GetM2MFieldNamesTestCase(unittest.TestCase):
+    def test__get_m2m_field_name__returns_expected_value(self):
+        def field_names(model):
+            history_model = get_history_model_for_model(model)
+            # Sort the fields, to prevent flaky tests
+            fields = sorted(history_model._history_m2m_fields, key=lambda f: f.name)
+            return [get_m2m_field_name(field) for field in fields]
+
+        self.assertListEqual(field_names(PollWithManyToMany), ["pollwithmanytomany"])
+        self.assertListEqual(
+            field_names(PollWithManyToManyCustomHistoryID),
+            ["pollwithmanytomanycustomhistoryid"],
+        )
+        self.assertListEqual(
+            field_names(PollWithManyToManyWithIPAddress),
+            ["pollwithmanytomanywithipaddress"],
+        )
+        self.assertListEqual(
+            field_names(PollWithSeveralManyToMany), ["pollwithseveralmanytomany"] * 3
+        )
+        self.assertListEqual(
+            field_names(PollChildBookWithManyToMany),
+            ["pollchildbookwithmanytomany"] * 2,
+        )
+        self.assertListEqual(
+            field_names(PollChildRestaurantWithManyToMany),
+            ["pollchildrestaurantwithmanytomany"] * 2,
+        )
+        self.assertListEqual(
+            field_names(PollWithSelfManyToMany), ["from_pollwithselfmanytomany"]
+        )
+
+    def test__get_m2m_reverse_field_name__returns_expected_value(self):
+        def field_names(model):
+            history_model = get_history_model_for_model(model)
+            # Sort the fields, to prevent flaky tests
+            fields = sorted(history_model._history_m2m_fields, key=lambda f: f.name)
+            return [get_m2m_reverse_field_name(field) for field in fields]
+
+        self.assertListEqual(field_names(PollWithManyToMany), ["place"])
+        self.assertListEqual(field_names(PollWithManyToManyCustomHistoryID), ["place"])
+        self.assertListEqual(field_names(PollWithManyToManyWithIPAddress), ["place"])
+        self.assertListEqual(
+            field_names(PollWithSeveralManyToMany), ["book", "place", "restaurant"]
+        )
+        self.assertListEqual(
+            field_names(PollChildBookWithManyToMany), ["book", "place"]
+        )
+        self.assertListEqual(
+            field_names(PollChildRestaurantWithManyToMany), ["place", "restaurant"]
+        )
+        self.assertListEqual(
+            field_names(PollWithSelfManyToMany), ["to_pollwithselfmanytomany"]
+        )
+
+
 class BulkCreateWithHistoryTestCase(TestCase):
     def setUp(self):
         self.data = [
             Poll(id=1, question="Question 1", pub_date=timezone.now()),
             Poll(id=2, question="Question 2", pub_date=timezone.now()),
             Poll(id=3, question="Question 3", pub_date=timezone.now()),
             Poll(id=4, question="Question 4", pub_date=timezone.now()),
```

### Comparing `django-simple-history-3.5.0/simple_history/tests/tests/utils.py` & `django_simple_history-3.6.0/simple_history/tests/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/tests/urls.py` & `django_simple_history-3.6.0/simple_history/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/tests/view.py` & `django_simple_history-3.6.0/simple_history/tests/view.py`

 * *Files identical despite different names*

### Comparing `django-simple-history-3.5.0/simple_history/utils.py` & `django_simple_history-3.6.0/simple_history/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,38 @@
 def get_app_model_primary_key_name(model):
     """Return the primary key name for a given app model."""
     if isinstance(model._meta.pk, ForeignKey):
         return model._meta.pk.name + "_id"
     return model._meta.pk.name
 
 
+def get_m2m_field_name(m2m_field: ManyToManyField) -> str:
+    """
+    Returns the field name of an M2M field's through model that corresponds to the model
+    the M2M field is defined on.
+
+    E.g. for a ``votes`` M2M field on a ``Poll`` model that references a ``Vote`` model
+    (and with a default-generated through model), this function would return ``"poll"``.
+    """
+    # This method is part of Django's internal API
+    return m2m_field.m2m_field_name()
+
+
+def get_m2m_reverse_field_name(m2m_field: ManyToManyField) -> str:
+    """
+    Returns the field name of an M2M field's through model that corresponds to the model
+    the M2M field references.
+
+    E.g. for a ``votes`` M2M field on a ``Poll`` model that references a ``Vote`` model
+    (and with a default-generated through model), this function would return ``"vote"``.
+    """
+    # This method is part of Django's internal API
+    return m2m_field.m2m_reverse_field_name()
+
+
 def bulk_create_with_history(
     objs,
     model,
     batch_size=None,
     ignore_conflicts=False,
     default_user=None,
     default_change_reason=None,
```

### Comparing `django-simple-history-3.5.0/tox.ini` & `django_simple_history-3.6.0/tox.ini`

 * *Files identical despite different names*

