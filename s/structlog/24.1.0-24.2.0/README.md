# Comparing `tmp/structlog-24.1.0.tar.gz` & `tmp/structlog-24.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Jan  8 09:45:50 2024, max compression
+gzip compressed data, last modified: Mon May 27 21:35:45 2024, max compression
```

## Comparing `structlog-24.1.0.tar` & `structlog-24.2.0.tar`

### file list

```diff
@@ -1,110 +1,113 @@
--rw-r--r--   0        0        0      125 2024-01-08 09:45:50.000000 structlog-24.1.0/.git_archival.txt
--rw-r--r--   0        0        0      143 2024-01-08 09:45:50.000000 structlog-24.1.0/.gitattributes
--rw-r--r--   0        0        0      758 2024-01-08 09:45:50.000000 structlog-24.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        5 2024-01-08 09:45:50.000000 structlog-24.1.0/.python-version-default
--rw-r--r--   0        0        0      224 2024-01-08 09:45:50.000000 structlog-24.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0    41788 2024-01-08 09:45:50.000000 structlog-24.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      407 2024-01-08 09:45:50.000000 structlog-24.1.0/COPYRIGHT
--rw-r--r--   0        0        0     6374 2024-01-08 09:45:50.000000 structlog-24.1.0/README.md
--rw-r--r--   0        0        0      882 2024-01-08 09:45:50.000000 structlog-24.1.0/show_off.py
--rw-r--r--   0        0        0     2942 2024-01-08 09:45:50.000000 structlog-24.1.0/tox.ini
--rw-r--r--   0        0        0     5483 2024-01-08 09:45:50.000000 structlog-24.1.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     9107 2024-01-08 09:45:50.000000 structlog-24.1.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0       43 2024-01-08 09:45:50.000000 structlog-24.1.0/.github/FUNDING.yml
--rw-r--r--   0        0        0     2474 2024-01-08 09:45:50.000000 structlog-24.1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      910 2024-01-08 09:45:50.000000 structlog-24.1.0/.github/SECURITY.md
--rw-r--r--   0        0        0      123 2024-01-08 09:45:50.000000 structlog-24.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0     5189 2024-01-08 09:45:50.000000 structlog-24.1.0/.github/sponsors/FilePreviews.svg
--rw-r--r--   0        0        0     1901 2024-01-08 09:45:50.000000 structlog-24.1.0/.github/sponsors/Sentry.svg
--rw-r--r--   0        0        0     2082 2024-01-08 09:45:50.000000 structlog-24.1.0/.github/sponsors/Tidelift.svg
--rw-r--r--   0        0        0     1932 2024-01-08 09:45:50.000000 structlog-24.1.0/.github/sponsors/Variomedia.svg
--rw-r--r--   0        0        0      659 2024-01-08 09:45:50.000000 structlog-24.1.0/.github/workflows/build-docset.yml
--rw-r--r--   0        0        0     5432 2024-01-08 09:45:50.000000 structlog-24.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      691 2024-01-08 09:45:50.000000 structlog-24.1.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1577 2024-01-08 09:45:50.000000 structlog-24.1.0/.github/workflows/pypi-package.yml
--rw-r--r--   0        0        0     5579 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/Makefile
--rw-r--r--   0        0        0    10879 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/api.rst
--rw-r--r--   0        0        0     8613 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/bound-loggers.md
--rw-r--r--   0        0        0     4332 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/conf.py
--rw-r--r--   0        0        0     4918 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/configuration.md
--rw-r--r--   0        0        0     5306 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/console-output.md
--rw-r--r--   0        0        0     6777 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/contextvars.md
--rw-r--r--   0        0        0     2295 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/exceptions.md
--rw-r--r--   0        0        0     4481 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/frameworks.md
--rw-r--r--   0        0        0    10472 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/getting-started.md
--rw-r--r--   0        0        0     2641 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/glossary.md
--rw-r--r--   0        0        0     2275 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/index.md
--rw-r--r--   0        0        0     1038 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/license.md
--rw-r--r--   0        0        0     4898 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/logging-best-practices.md
--rw-r--r--   0        0        0     5102 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/make.bat
--rw-r--r--   0        0        0     4462 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/performance.md
--rw-r--r--   0        0        0     6006 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/processors.md
--rw-r--r--   0        0        0     7325 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/recipes.md
--rw-r--r--   0        0        0    21452 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/standard-library.md
--rw-r--r--   0        0        0     2375 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/testing.md
--rw-r--r--   0        0        0     6782 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/thread-local.md
--rw-r--r--   0        0        0     4306 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/twisted.md
--rw-r--r--   0        0        0     1901 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/typing.md
--rw-r--r--   0        0        0     4603 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/why.md
--rw-r--r--   0        0        0    55792 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/_static/BoundLogger.svg
--rw-r--r--   0        0        0      355 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/_static/Justfile
--rw-r--r--   0        0        0   253716 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/_static/console_renderer.png
--rw-r--r--   0        0        0      277 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/_static/custom.css
--rw-r--r--   0        0        0      677 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/_static/docset-icon.png
--rw-r--r--   0        0        0     1810 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/_static/docset-icon@2x.png
--rw-r--r--   0        0        0   577103 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/_static/social card.afdesign
--rw-r--r--   0        0        0   112021 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/_static/structlog_logo.afdesign
--rw-r--r--   0        0        0   152510 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/_static/structlog_logo.png
--rw-r--r--   0        0        0    25175 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/_static/structlog_logo.svg
--rw-r--r--   0        0        0    58175 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/_static/structlog_logo_horizontal.afdesign
--rw-r--r--   0        0        0    28032 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/_static/structlog_logo_horizontal.svg
--rw-r--r--   0        0        0    22682 2024-01-08 09:45:50.000000 structlog-24.1.0/docs/_static/structlog_logo_small.png
--rw-r--r--   0        0        0     2911 2024-01-08 09:45:50.000000 structlog-24.1.0/src/structlog/__init__.py
--rw-r--r--   0        0        0     7297 2024-01-08 09:45:50.000000 structlog-24.1.0/src/structlog/_base.py
--rw-r--r--   0        0        0    13866 2024-01-08 09:45:50.000000 structlog-24.1.0/src/structlog/_config.py
--rw-r--r--   0        0        0     2177 2024-01-08 09:45:50.000000 structlog-24.1.0/src/structlog/_frames.py
--rw-r--r--   0        0        0     1636 2024-01-08 09:45:50.000000 structlog-24.1.0/src/structlog/_generic.py
--rw-r--r--   0        0        0     1206 2024-01-08 09:45:50.000000 structlog-24.1.0/src/structlog/_greenlets.py
--rw-r--r--   0        0        0     1886 2024-01-08 09:45:50.000000 structlog-24.1.0/src/structlog/_log_levels.py
--rw-r--r--   0        0        0     7645 2024-01-08 09:45:50.000000 structlog-24.1.0/src/structlog/_native.py
--rw-r--r--   0        0        0     9276 2024-01-08 09:45:50.000000 structlog-24.1.0/src/structlog/_output.py
--rw-r--r--   0        0        0     1545 2024-01-08 09:45:50.000000 structlog-24.1.0/src/structlog/_utils.py
--rw-r--r--   0        0        0     5369 2024-01-08 09:45:50.000000 structlog-24.1.0/src/structlog/contextvars.py
--rw-r--r--   0        0        0    23428 2024-01-08 09:45:50.000000 structlog-24.1.0/src/structlog/dev.py
--rw-r--r--   0        0        0      503 2024-01-08 09:45:50.000000 structlog-24.1.0/src/structlog/exceptions.py
--rw-r--r--   0        0        0    27945 2024-01-08 09:45:50.000000 structlog-24.1.0/src/structlog/processors.py
--rw-r--r--   0        0        0        0 2024-01-08 09:45:50.000000 structlog-24.1.0/src/structlog/py.typed
--rw-r--r--   0        0        0    37507 2024-01-08 09:45:50.000000 structlog-24.1.0/src/structlog/stdlib.py
--rw-r--r--   0        0        0     5228 2024-01-08 09:45:50.000000 structlog-24.1.0/src/structlog/testing.py
--rw-r--r--   0        0        0     9185 2024-01-08 09:45:50.000000 structlog-24.1.0/src/structlog/threadlocal.py
--rw-r--r--   0        0        0     7739 2024-01-08 09:45:50.000000 structlog-24.1.0/src/structlog/tracebacks.py
--rw-r--r--   0        0        0    10173 2024-01-08 09:45:50.000000 structlog-24.1.0/src/structlog/twisted.py
--rw-r--r--   0        0        0      764 2024-01-08 09:45:50.000000 structlog-24.1.0/src/structlog/types.py
--rw-r--r--   0        0        0     8019 2024-01-08 09:45:50.000000 structlog-24.1.0/src/structlog/typing.py
--rw-r--r--   0        0        0      226 2024-01-08 09:45:50.000000 structlog-24.1.0/tests/__init__.py
--rw-r--r--   0        0        0      488 2024-01-08 09:45:50.000000 structlog-24.1.0/tests/additional_frame.py
--rw-r--r--   0        0        0     1465 2024-01-08 09:45:50.000000 structlog-24.1.0/tests/conftest.py
--rw-r--r--   0        0        0     7298 2024-01-08 09:45:50.000000 structlog-24.1.0/tests/test_base.py
--rw-r--r--   0        0        0    13226 2024-01-08 09:45:50.000000 structlog-24.1.0/tests/test_config.py
--rw-r--r--   0        0        0     9087 2024-01-08 09:45:50.000000 structlog-24.1.0/tests/test_contextvars.py
--rw-r--r--   0        0        0    19708 2024-01-08 09:45:50.000000 structlog-24.1.0/tests/test_dev.py
--rw-r--r--   0        0        0     4419 2024-01-08 09:45:50.000000 structlog-24.1.0/tests/test_frames.py
--rw-r--r--   0        0        0     1671 2024-01-08 09:45:50.000000 structlog-24.1.0/tests/test_generic.py
--rw-r--r--   0        0        0     9066 2024-01-08 09:45:50.000000 structlog-24.1.0/tests/test_log_levels.py
--rw-r--r--   0        0        0     9325 2024-01-08 09:45:50.000000 structlog-24.1.0/tests/test_output.py
--rw-r--r--   0        0        0     1499 2024-01-08 09:45:50.000000 structlog-24.1.0/tests/test_packaging.py
--rw-r--r--   0        0        0    34415 2024-01-08 09:45:50.000000 structlog-24.1.0/tests/test_processors.py
--rw-r--r--   0        0        0    40780 2024-01-08 09:45:50.000000 structlog-24.1.0/tests/test_stdlib.py
--rw-r--r--   0        0        0     4773 2024-01-08 09:45:50.000000 structlog-24.1.0/tests/test_testing.py
--rw-r--r--   0        0        0    13796 2024-01-08 09:45:50.000000 structlog-24.1.0/tests/test_threadlocal.py
--rw-r--r--   0        0        0    16614 2024-01-08 09:45:50.000000 structlog-24.1.0/tests/test_tracebacks.py
--rw-r--r--   0        0        0    10263 2024-01-08 09:45:50.000000 structlog-24.1.0/tests/test_twisted.py
--rw-r--r--   0        0        0     3304 2024-01-08 09:45:50.000000 structlog-24.1.0/tests/test_utils.py
--rw-r--r--   0        0        0      465 2024-01-08 09:45:50.000000 structlog-24.1.0/tests/utils.py
--rw-r--r--   0        0        0    10990 2024-01-08 09:45:50.000000 structlog-24.1.0/tests/typing/api.py
--rw-r--r--   0        0        0      171 2024-01-08 09:45:50.000000 structlog-24.1.0/.gitignore
--rw-r--r--   0        0        0    10174 2024-01-08 09:45:50.000000 structlog-24.1.0/LICENSE-APACHE
--rw-r--r--   0        0        0     1113 2024-01-08 09:45:50.000000 structlog-24.1.0/LICENSE-MIT
--rw-r--r--   0        0        0       72 2024-01-08 09:45:50.000000 structlog-24.1.0/NOTICE
--rw-r--r--   0        0        0     6344 2024-01-08 09:45:50.000000 structlog-24.1.0/pyproject.toml
--rw-r--r--   0        0        0     6941 2024-01-08 09:45:50.000000 structlog-24.1.0/PKG-INFO
+-rw-r--r--   0        0        0      125 2024-05-27 21:35:45.000000 structlog-24.2.0/.git_archival.txt
+-rw-r--r--   0        0        0      143 2024-05-27 21:35:45.000000 structlog-24.2.0/.gitattributes
+-rw-r--r--   0        0        0      756 2024-05-27 21:35:45.000000 structlog-24.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        5 2024-05-27 21:35:45.000000 structlog-24.2.0/.python-version-default
+-rw-r--r--   0        0        0      224 2024-05-27 21:35:45.000000 structlog-24.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0    42993 2024-05-27 21:35:45.000000 structlog-24.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      407 2024-05-27 21:35:45.000000 structlog-24.2.0/COPYRIGHT
+-rw-r--r--   0        0        0     6533 2024-05-27 21:35:45.000000 structlog-24.2.0/README.md
+-rw-r--r--   0        0        0      882 2024-05-27 21:35:45.000000 structlog-24.2.0/show_off.py
+-rw-r--r--   0        0        0     2901 2024-05-27 21:35:45.000000 structlog-24.2.0/tox.ini
+-rw-r--r--   0        0        0     5482 2024-05-27 21:35:45.000000 structlog-24.2.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     9411 2024-05-27 21:35:45.000000 structlog-24.2.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0       43 2024-05-27 21:35:45.000000 structlog-24.2.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0     2474 2024-05-27 21:35:45.000000 structlog-24.2.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      910 2024-05-27 21:35:45.000000 structlog-24.2.0/.github/SECURITY.md
+-rw-r--r--   0        0        0      123 2024-05-27 21:35:45.000000 structlog-24.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     5189 2024-05-27 21:35:45.000000 structlog-24.2.0/.github/sponsors/FilePreviews.svg
+-rw-r--r--   0        0        0     5490 2024-05-27 21:35:45.000000 structlog-24.2.0/.github/sponsors/Klaviyo.svg
+-rw-r--r--   0        0        0     1901 2024-05-27 21:35:45.000000 structlog-24.2.0/.github/sponsors/Sentry.svg
+-rw-r--r--   0        0        0     2082 2024-05-27 21:35:45.000000 structlog-24.2.0/.github/sponsors/Tidelift.svg
+-rw-r--r--   0        0        0     1932 2024-05-27 21:35:45.000000 structlog-24.2.0/.github/sponsors/Variomedia.svg
+-rw-r--r--   0        0        0      649 2024-05-27 21:35:45.000000 structlog-24.2.0/.github/workflows/build-docset.yml
+-rw-r--r--   0        0        0     5848 2024-05-27 21:35:45.000000 structlog-24.2.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      691 2024-05-27 21:35:45.000000 structlog-24.2.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1662 2024-05-27 21:35:45.000000 structlog-24.2.0/.github/workflows/pypi-package.yml
+-rw-r--r--   0        0        0     5579 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/Makefile
+-rw-r--r--   0        0        0    10879 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/api.rst
+-rw-r--r--   0        0        0     8613 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/bound-loggers.md
+-rw-r--r--   0        0        0     4331 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/conf.py
+-rw-r--r--   0        0        0     4920 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/configuration.md
+-rw-r--r--   0        0        0     5306 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/console-output.md
+-rw-r--r--   0        0        0     6777 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/contextvars.md
+-rw-r--r--   0        0        0     2295 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/exceptions.md
+-rw-r--r--   0        0        0     4481 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/frameworks.md
+-rw-r--r--   0        0        0    10469 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/getting-started.md
+-rw-r--r--   0        0        0     2641 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/glossary.md
+-rw-r--r--   0        0        0     2275 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/index.md
+-rw-r--r--   0        0        0     1038 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/license.md
+-rw-r--r--   0        0        0     4898 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/logging-best-practices.md
+-rw-r--r--   0        0        0     5102 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/make.bat
+-rw-r--r--   0        0        0     4462 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/performance.md
+-rw-r--r--   0        0        0     6006 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/processors.md
+-rw-r--r--   0        0        0     7325 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/recipes.md
+-rw-r--r--   0        0        0    22284 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/standard-library.md
+-rw-r--r--   0        0        0     2375 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/testing.md
+-rw-r--r--   0        0        0     6782 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/thread-local.md
+-rw-r--r--   0        0        0     4306 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/twisted.md
+-rw-r--r--   0        0        0     1901 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/typing.md
+-rw-r--r--   0        0        0     4603 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/why.md
+-rw-r--r--   0        0        0    55792 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/_static/BoundLogger.svg
+-rw-r--r--   0        0        0      355 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/_static/Justfile
+-rw-r--r--   0        0        0   253716 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/_static/console_renderer.png
+-rw-r--r--   0        0        0      277 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/_static/custom.css
+-rw-r--r--   0        0        0     1145 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/_static/docset-icon.png
+-rw-r--r--   0        0        0     2172 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/_static/docset-icon@2x.png
+-rw-r--r--   0        0        0   577103 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/_static/social card.afdesign
+-rw-r--r--   0        0        0   112021 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/_static/structlog_logo.afdesign
+-rw-r--r--   0        0        0   152510 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/_static/structlog_logo.png
+-rw-r--r--   0        0        0    25175 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/_static/structlog_logo.svg
+-rw-r--r--   0        0        0    58175 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/_static/structlog_logo_horizontal.afdesign
+-rw-r--r--   0        0        0    28032 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/_static/structlog_logo_horizontal.svg
+-rw-r--r--   0        0        0    22682 2024-05-27 21:35:45.000000 structlog-24.2.0/docs/_static/structlog_logo_small.png
+-rw-r--r--   0        0        0     2911 2024-05-27 21:35:45.000000 structlog-24.2.0/src/structlog/__init__.py
+-rw-r--r--   0        0        0     7263 2024-05-27 21:35:45.000000 structlog-24.2.0/src/structlog/_base.py
+-rw-r--r--   0        0        0    13868 2024-05-27 21:35:45.000000 structlog-24.2.0/src/structlog/_config.py
+-rw-r--r--   0        0        0     2161 2024-05-27 21:35:45.000000 structlog-24.2.0/src/structlog/_frames.py
+-rw-r--r--   0        0        0     1636 2024-05-27 21:35:45.000000 structlog-24.2.0/src/structlog/_generic.py
+-rw-r--r--   0        0        0     1206 2024-05-27 21:35:45.000000 structlog-24.2.0/src/structlog/_greenlets.py
+-rw-r--r--   0        0        0     1886 2024-05-27 21:35:45.000000 structlog-24.2.0/src/structlog/_log_levels.py
+-rw-r--r--   0        0        0     7633 2024-05-27 21:35:45.000000 structlog-24.2.0/src/structlog/_native.py
+-rw-r--r--   0        0        0     9115 2024-05-27 21:35:45.000000 structlog-24.2.0/src/structlog/_output.py
+-rw-r--r--   0        0        0      933 2024-05-27 21:35:45.000000 structlog-24.2.0/src/structlog/_utils.py
+-rw-r--r--   0        0        0     5371 2024-05-27 21:35:45.000000 structlog-24.2.0/src/structlog/contextvars.py
+-rw-r--r--   0        0        0    23950 2024-05-27 21:35:45.000000 structlog-24.2.0/src/structlog/dev.py
+-rw-r--r--   0        0        0      503 2024-05-27 21:35:45.000000 structlog-24.2.0/src/structlog/exceptions.py
+-rw-r--r--   0        0        0    28629 2024-05-27 21:35:45.000000 structlog-24.2.0/src/structlog/processors.py
+-rw-r--r--   0        0        0        0 2024-05-27 21:35:45.000000 structlog-24.2.0/src/structlog/py.typed
+-rw-r--r--   0        0        0    38043 2024-05-27 21:35:45.000000 structlog-24.2.0/src/structlog/stdlib.py
+-rw-r--r--   0        0        0     5229 2024-05-27 21:35:45.000000 structlog-24.2.0/src/structlog/testing.py
+-rw-r--r--   0        0        0     9185 2024-05-27 21:35:45.000000 structlog-24.2.0/src/structlog/threadlocal.py
+-rw-r--r--   0        0        0     7799 2024-05-27 21:35:45.000000 structlog-24.2.0/src/structlog/tracebacks.py
+-rw-r--r--   0        0        0    10091 2024-05-27 21:35:45.000000 structlog-24.2.0/src/structlog/twisted.py
+-rw-r--r--   0        0        0      764 2024-05-27 21:35:45.000000 structlog-24.2.0/src/structlog/types.py
+-rw-r--r--   0        0        0     7979 2024-05-27 21:35:45.000000 structlog-24.2.0/src/structlog/typing.py
+-rw-r--r--   0        0        0      226 2024-05-27 21:35:45.000000 structlog-24.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      488 2024-05-27 21:35:45.000000 structlog-24.2.0/tests/additional_frame.py
+-rw-r--r--   0        0        0     1465 2024-05-27 21:35:45.000000 structlog-24.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     7298 2024-05-27 21:35:45.000000 structlog-24.2.0/tests/test_base.py
+-rw-r--r--   0        0        0    13240 2024-05-27 21:35:45.000000 structlog-24.2.0/tests/test_config.py
+-rw-r--r--   0        0        0     9087 2024-05-27 21:35:45.000000 structlog-24.2.0/tests/test_contextvars.py
+-rw-r--r--   0        0        0    19708 2024-05-27 21:35:45.000000 structlog-24.2.0/tests/test_dev.py
+-rw-r--r--   0        0        0     4419 2024-05-27 21:35:45.000000 structlog-24.2.0/tests/test_frames.py
+-rw-r--r--   0        0        0     1671 2024-05-27 21:35:45.000000 structlog-24.2.0/tests/test_generic.py
+-rw-r--r--   0        0        0     9066 2024-05-27 21:35:45.000000 structlog-24.2.0/tests/test_log_levels.py
+-rw-r--r--   0        0        0     9325 2024-05-27 21:35:45.000000 structlog-24.2.0/tests/test_output.py
+-rw-r--r--   0        0        0     1499 2024-05-27 21:35:45.000000 structlog-24.2.0/tests/test_packaging.py
+-rw-r--r--   0        0        0    43074 2024-05-27 21:35:45.000000 structlog-24.2.0/tests/test_stdlib.py
+-rw-r--r--   0        0        0     4773 2024-05-27 21:35:45.000000 structlog-24.2.0/tests/test_testing.py
+-rw-r--r--   0        0        0    13796 2024-05-27 21:35:45.000000 structlog-24.2.0/tests/test_threadlocal.py
+-rw-r--r--   0        0        0    16598 2024-05-27 21:35:45.000000 structlog-24.2.0/tests/test_tracebacks.py
+-rw-r--r--   0        0        0    10263 2024-05-27 21:35:45.000000 structlog-24.2.0/tests/test_twisted.py
+-rw-r--r--   0        0        0     2170 2024-05-27 21:35:45.000000 structlog-24.2.0/tests/test_utils.py
+-rw-r--r--   0        0        0      465 2024-05-27 21:35:45.000000 structlog-24.2.0/tests/utils.py
+-rw-r--r--   0        0        0        0 2024-05-27 21:35:45.000000 structlog-24.2.0/tests/processors/__init__.py
+-rw-r--r--   0        0        0    19631 2024-05-27 21:35:45.000000 structlog-24.2.0/tests/processors/test_processors.py
+-rw-r--r--   0        0        0    16918 2024-05-27 21:35:45.000000 structlog-24.2.0/tests/processors/test_renderers.py
+-rw-r--r--   0        0        0    10990 2024-05-27 21:35:45.000000 structlog-24.2.0/tests/typing/api.py
+-rw-r--r--   0        0        0      171 2024-05-27 21:35:45.000000 structlog-24.2.0/.gitignore
+-rw-r--r--   0        0        0    10174 2024-05-27 21:35:45.000000 structlog-24.2.0/LICENSE-APACHE
+-rw-r--r--   0        0        0     1113 2024-05-27 21:35:45.000000 structlog-24.2.0/LICENSE-MIT
+-rw-r--r--   0        0        0       72 2024-05-27 21:35:45.000000 structlog-24.2.0/NOTICE
+-rw-r--r--   0        0        0     6488 2024-05-27 21:35:45.000000 structlog-24.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7943 2024-05-27 21:35:45.000000 structlog-24.2.0/PKG-INFO
```

### Comparing `structlog-24.1.0/CHANGELOG.md` & `structlog-24.2.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,47 @@
 The **third number** is for emergencies when we need to start branches for older releases.
 
 You can find our backwards-compatibility policy [here](https://github.com/hynek/structlog/blob/main/.github/SECURITY.md).
 
 <!-- changelog follows -->
 
 
+## [24.2.0](https://github.com/hynek/structlog/compare/24.1.0...24.2.0) - 2024-05-27
+
+### Added
+
+- It is now possible to disable log level-padding in `structlog.dev.LogLevelColumnFormatter` and `structlog.dev.ConsoleRenderer`.
+  [#599](https://github.com/hynek/structlog/pull/599)
+
+- The `structlog.processors.CallsiteParameterAdder` can now be pickled.
+  [#603](https://github.com/hynek/structlog/pull/603)
+
+- `structlog.processors.CallsiteParameterAdder` now also works with `structlog.stdlib.BoundLogger`'s non-standard async methods (`ainfo()`, and so forth)
+  [#618](https://github.com/hynek/structlog/pull/618)
+
+
+### Changed
+
+- `structlog.processors.LogfmtRenderer` now escapes newlines.
+  [#592](https://github.com/hynek/structlog/pull/592)
+
+- `structlog.processors.LogfmtRenderer` now escapes backslashes and double quotes.
+  [#594](https://github.com/hynek/structlog/pull/594)
+
+- `structlog.processors.CallsiteParameterAdder` has been optimized to be about 2x faster.
+  [#606](https://github.com/hynek/structlog/pull/606)
+
+
+### Fixed
+
+- `structlog.stdlib.render_to_log_kwargs` now correctly passes stacklevel as a kwarg to stdlib logging.
+  [#619](https://github.com/hynek/structlog/pull/620)
+
+
+
 ## [24.1.0](https://github.com/hynek/structlog/compare/23.3.0...24.1.0) - 2024-01-08
 
 ### Fixed
 
 - The lazy logger proxy returned by `structlog.get_logger()` now returns its initial values when asked for context.
   When asked for context before binding for the first time, it returned an empty dictionary in 23.3.0.
```

### Comparing `structlog-24.1.0/README.md` & `structlog-24.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
 *structlog* would not be possible without our [amazing sponsors](https://github.com/sponsors/hynek).
 Especially those generously supporting us at the *The Organization* tier and higher:
 
 <p align="center">
    <a href="https://www.variomedia.de/"><img src="https://raw.githubusercontent.com/hynek/structlog/main/.github/sponsors/Variomedia.svg" width="200" height="60" /></a>
    <a href="https://tidelift.com/?utm_source=lifter&utm_medium=referral&utm_campaign=hynek"><img src="https://raw.githubusercontent.com/hynek/structlog/main/.github/sponsors/Tidelift.svg" width="200" height="60" /></a>
+   <a href="https://klaviyo.com/"><img src="https://raw.githubusercontent.com/hynek/structlog/main/.github/sponsors/Klaviyo.svg" width="200" height="60"/></a>
    <a href="https://filepreviews.io/"><img src="https://raw.githubusercontent.com/hynek/structlog/main/.github/sponsors/FilePreviews.svg" width="200" height="60" /></a>
 </p>
 
 <p align="center">
    <strong>Please consider <a href="https://github.com/sponsors/hynek">joining them</a> to help make <em>structlog</em>’s maintenance more sustainable!</strong>
 </p>
```

#### html2text {}

```diff
@@ -20,15 +20,16 @@
 blob/main/docs/_static/console_renderer.png?raw=true) ## Sponsors *structlog*
 would not be possible without our [amazing sponsors](https://github.com/
 sponsors/hynek). Especially those generously supporting us at the *The
 Organization* tier and higher:
    _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_h_y_n_e_k_/_s_t_r_u_c_t_l_o_g_/_m_a_i_n_/_._g_i_t_h_u_b_/_s_p_o_n_s_o_r_s_/
 _V_a_r_i_o_m_e_d_i_a_._s_v_g_]_[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_h_y_n_e_k_/_s_t_r_u_c_t_l_o_g_/_m_a_i_n_/_._g_i_t_h_u_b_/
    _s_p_o_n_s_o_r_s_/_T_i_d_e_l_i_f_t_._s_v_g_]_[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_h_y_n_e_k_/_s_t_r_u_c_t_l_o_g_/
-                    _m_a_i_n_/_._g_i_t_h_u_b_/_s_p_o_n_s_o_r_s_/_F_i_l_e_P_r_e_v_i_e_w_s_._s_v_g_]
+  _m_a_i_n_/_._g_i_t_h_u_b_/_s_p_o_n_s_o_r_s_/_K_l_a_v_i_y_o_._s_v_g_]_[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_h_y_n_e_k_/
+               _s_t_r_u_c_t_l_o_g_/_m_a_i_n_/_._g_i_t_h_u_b_/_s_p_o_n_s_o_r_s_/_F_i_l_e_P_r_e_v_i_e_w_s_._s_v_g_]
    PPlleeaassee ccoonnssiiddeerr _jj_oo_ii_nn_ii_nn_gg_ _tt_hh_ee_mm ttoo hheellpp mmaakkee ssttrruuccttlloogg?â??ss mmaaiinntteennaannccee mmoorree
                                  ssuussttaaiinnaabbllee!!
 --- *structlog* has been successfully used in production at every scale since
 **2013**, while embracing cutting-edge technologies like *asyncio*, context
 variables, or type hints as they emerged. Its paradigms proved influential
 enough to [help design](https://twitter.com/sirupsen/status/638330548361019392)
 structured logging [packages across ecosystems](https://github.com/sirupsen/
```

### Comparing `structlog-24.1.0/show_off.py` & `structlog-24.2.0/show_off.py`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/tox.ini` & `structlog-24.2.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,14 @@
 
 [testenv]
 package = wheel
 wheel_build_env = .pkg
 extras =
     tests: tests
     mypy: typing
-pass_env =
-    FORCE_COLOR
-    NO_COLOR
 commands =
     tests: pytest {posargs}
     mypy: mypy tests/typing
 
 
 # Run oldest and latest under Coverage.
 # Keep in-sync with coverage `depends below.
@@ -66,15 +63,14 @@
 commands =
     watchfiles \
         --ignore-paths docs/_build/ \
         'sphinx-build -W -n --jobs auto -b html -d {envtmpdir}/doctrees docs docs/_build/html' \
         src \
         docs
 
-
 [testenv:docs-linkcheck]
 base_python = {[testenv:docs]base_python}
 extras = {[testenv:docs]extras}
 commands = sphinx-build -W -b linkcheck -d {envtmpdir}/doctrees docs docs/_build/html
 
 
 [testenv:pre-commit]
```

### Comparing `structlog-24.1.0/.github/CODE_OF_CONDUCT.md` & `structlog-24.2.0/.github/CODE_OF_CONDUCT.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Contributor Covenant Code of Conduct
 
 ## Our Pledge
 
 We as members, contributors, and leaders pledge to make participation in our
 community a harassment-free experience for everyone, regardless of age, body
 size, visible or invisible disability, ethnicity, sex characteristics, gender
-identity and expression, level of experience, education, socio-economic status,
+identity and expression, level of experience, education, socioeconomic status,
 nationality, personal appearance, race, caste, color, religion, or sexual
 identity and orientation.
 
 We pledge to act and interact in ways that contribute to an open, welcoming,
 diverse, inclusive, and healthy community.
 
 ## Our Standards
```

### Comparing `structlog-24.1.0/.github/CONTRIBUTING.md` & `structlog-24.2.0/.github/CONTRIBUTING.md`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,23 @@
 
 If you're using [*direnv*](https://direnv.net), you can automate the creation of a virtual environment with the correct Python version by adding the following `.envrc` to the project root:
 
 ```bash
 layout python python$(cat .python-version-default)
 ```
 
+or, if you like [*uv*](https://github.com/astral-sh/uv):
+
+```bash
+test -d .venv || uv venv --python python$(cat .python-version-default)
+. .venv/bin/activate
+```
+
+---
+
 [Create a fork](https://github.com/hynek/structlog/fork) of the *structlog* repository and clone it:
 
 ```console
 $ git clone git@github.com:YOU/structlog.git
 ```
 
 Or if you prefer to use Git via HTTPS:
@@ -65,15 +74,15 @@
 
 > [!WARNING]
 > - **Before** you start working on a new pull request, use the "*Sync fork*" button in GitHub's web UI to ensure your fork is up to date.
 > - **Always create a new branch off `main` for each new pull request.**
 >   Yes, you can work on `main` in your fork and submit pull requests.
 >   But this will *inevitably* lead to you not being able to synchronize your fork with upstream and having to start over.
 
-Change into the newly created directory and after activating a virtual environment, install an editable version of *structlog* along with its tests and docs requirements:
+Change into the newly created directory and after activating a virtual environment, install an editable version of *structlog* along with its tests requirements:
 
 ```console
 $ cd structlog
 $ python -Im pip install --upgrade pip wheel  # PLEASE don't skip this step
 $ python -Im pip install -e '.[dev]'
 ```
 
@@ -81,22 +90,22 @@
 
 ```console
 $ python -m pytest
 ```
 
 When working on the documentation, use:
 
-```bash
+```console
 $ tox run -e docs-watch
 ```
 
 ... to watch your files and automatically rebuild when a file changes.
 And use:
 
-```bash
+```console
 $ tox run -e docs
 ```
 
 ... to build it once and run our doctests.
 
 The built documentation can then be found in `docs/_build/html/`.
 
@@ -127,14 +136,18 @@
   def func(x: str) -> str:
       """
       Do something.
 
       Args:
           x: A very important parameter.
 
+          y:
+              Another important parameter but one that doesn't fit a line so
+              it already starts on the next one.
+
       Returns:
           A very important return value.
       """
   ```
 - If you add or change public APIs, tag the docstring using `..  versionadded:: 16.0.0 WHAT` or `..  versionchanged:: 16.2.0 WHAT`.
 - We use [Ruff](https://ruff.rs/) to sort our imports, and we use [Black](https://github.com/psf/black) with line length of 79 characters to format our code.
   As long as you run our full [*tox*] suite before committing, or install our [*pre-commit*] hooks (ideally you'll do both – see [*Local Development Environment*](#local-development-environment) above), you won't have to spend any time on formatting your code at all.
@@ -176,15 +189,15 @@
 
   ```markdown
   Last line of previous section.
 
 
   ## Header of New Top Section
 
-  ###  Header of New Section
+  ### Header of New Section
 
   First line of new section.
   ```
 
 
 ### Changelog
```

### Comparing `structlog-24.1.0/.github/PULL_REQUEST_TEMPLATE.md` & `structlog-24.2.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/.github/SECURITY.md` & `structlog-24.2.0/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/.github/sponsors/FilePreviews.svg` & `structlog-24.2.0/.github/sponsors/FilePreviews.svg`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/.github/sponsors/Sentry.svg` & `structlog-24.2.0/.github/sponsors/Sentry.svg`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/.github/sponsors/Tidelift.svg` & `structlog-24.2.0/.github/sponsors/Tidelift.svg`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/.github/sponsors/Variomedia.svg` & `structlog-24.2.0/.github/sponsors/Variomedia.svg`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/.github/workflows/build-docset.yml` & `structlog-24.2.0/.github/workflows/build-docset.yml`

 * *Files 5% similar despite different names*

```diff
@@ -6,30 +6,29 @@
     tags: ["*"]
   workflow_dispatch:
 
 env:
   PIP_DISABLE_PIP_VERSION_CHECK: 1
   PIP_NO_PYTHON_VERSION_WARNING: 1
 
-permissions:
-  contents: read
+permissions: {}
 
 jobs:
   docset:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0  # get correct version
       - uses: actions/setup-python@v5
         with:
           python-version: "3.12"
 
       - run: pip install tox
 
-      - run: tox -e docset
+      - run: tox run -e docset
       - run: tar --exclude='.DS_Store' -cvzf structlog.tgz structlog.docset
 
       - uses: actions/upload-artifact@v4
         with:
           name: docset
           path: structlog.tgz
```

### Comparing `structlog-24.1.0/.github/workflows/ci.yml` & `structlog-24.2.0/.github/workflows/ci.yml`

 * *Files 9% similar despite different names*

```diff
@@ -21,42 +21,41 @@
 
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - uses: hynek/build-and-inspect-python-package@v2
+        id: baipp
+
+    outputs:
+      python-versions: ${{ steps.baipp.outputs.supported_python_classifiers_json_array }}
 
   tests:
     name: Tests & API Mypy on ${{ matrix.python-version }}
     needs: build-package
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version:
-          - "3.8"
-          - "3.9"
-          - "3.10"
-          - "3.11"
-          - "3.12"
+        python-version: ${{ fromJson(needs.build-package.outputs.python-versions) }}
 
     steps:
       - name: Download pre-built packages
         uses: actions/download-artifact@v4
         with:
           name: Packages
           path: dist
       - run: tar xf dist/*.tar.gz --strip-components=1
       - uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
           allow-prereleases: true
           cache: pip
-      - run: python -Im pip install tox
+      - run: python -Im pip install tox-uv
 
       - run: python -Im tox run --installpkg dist/*.whl -f py$(echo ${{ matrix.python-version }} | tr -d .)
 
       - name: Upload coverage data
         uses: actions/upload-artifact@v4
         with:
           name: coverage-data-${{ matrix.python-version }}
@@ -111,15 +110,15 @@
           path: dist
       - run: tar xf dist/*.tar.gz --strip-components=1
       - uses: actions/setup-python@v5
         with:
           python-version-file: .python-version-default
           allow-prereleases: true
           cache: pip
-      - run: python -Im pip install tox
+      - run: python -Im pip install tox-uv
 
       - run: python -Im tox run --installpkg dist/*.whl -e mypy-pkg
 
   pyright:
     name: Pyright
     runs-on: ubuntu-latest
     needs: build-package
@@ -132,15 +131,15 @@
           path: dist
       - run: tar xf dist/*.tar.gz --strip-components=1
       - uses: actions/setup-python@v5
         with:
           python-version-file: .python-version-default
           allow-prereleases: true
           cache: pip
-      - run: python -Im pip install tox
+      - run: python -Im pip install tox-uv
 
       - run: python -Im tox run --installpkg dist/*.whl -e pyright
 
   docs:
     name: Build docs & run doctests
     needs: build-package
     runs-on: ubuntu-latest
@@ -152,15 +151,15 @@
           path: dist
       - run: tar xf dist/*.tar.gz --strip-components=1
       - uses: actions/setup-python@v5
         with:
           # Keep in sync with tox.ini/docs & .readthedocs.yaml
           python-version: "3.12"
           cache: pip
-      - run: python -Im pip install tox
+      - run: python -Im pip install tox-uv
 
       - run: python -Im tox run -e docs
 
   install-dev:
     name: Verify dev env
     runs-on: ${{ matrix.os }}
     strategy:
@@ -170,16 +169,22 @@
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
           python-version-file: .python-version-default
           cache: pip
 
-      - run: python -Im pip install -e .[dev]
-      - run: python -Ic 'import structlog; print(structlog.__version__)'
+      - run: python -Im pip install uv
+      - run: uv venv
+      - run: uv pip install -e .[dev]
+
+      - run: .venv/bin/python -Ic 'import structlog; print(structlog.__version__)'
+        if: runner.os != 'Windows'
+      - run: .\.venv\Scripts\python.exe -Ic 'import structlog; print(structlog.__version__)'
+        if: runner.os == 'Windows'
 
   required-checks-pass:
     name: Ensure everything required is passing for branch protection
     if: always()
 
     needs:
       - coverage
@@ -192,22 +197,22 @@
 
     steps:
       - name: Decide whether the needed jobs succeeded or failed
         uses: re-actors/alls-green@release/v1
         with:
           jobs: ${{ toJSON(needs) }}
 
-
   colors:
     name: Visual check for color settings using env variables
     needs: build-package
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
           python-version-file: .python-version-default
           cache: pip
-      - run: python -Im pip install tox
+      # tox 4.12.0 started passing FORCE_COLOR and NO_COLOR by default.
+      - run: python -Im pip install 'tox>=4.12.0' tox-uv
 
       - run: python -Im tox run -f color
```

### Comparing `structlog-24.1.0/.github/workflows/codeql-analysis.yml` & `structlog-24.2.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/.github/workflows/pypi-package.yml` & `structlog-24.2.0/.github/workflows/pypi-package.yml`

 * *Files 17% similar despite different names*

```diff
@@ -7,28 +7,31 @@
     tags: ["*"]
   release:
     types:
       - published
   workflow_dispatch:
 
 permissions:
+  attestations: write
   contents: read
   id-token: write
 
 jobs:
   build-package:
     name: Build & verify package
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - uses: hynek/build-and-inspect-python-package@v2
+        with:
+          attest-build-provenance-github: 'true'
 
   # Upload to Test PyPI on every commit on main.
   release-test-pypi:
     name: Publish in-dev package to test.pypi.org
     environment: release-test-pypi
     if: github.event_name == 'push' && github.ref == 'refs/heads/main'
     runs-on: ubuntu-latest
```

### Comparing `structlog-24.1.0/docs/Makefile` & `structlog-24.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/api.rst` & `structlog-24.2.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/bound-loggers.md` & `structlog-24.2.0/docs/bound-loggers.md`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/conf.py` & `structlog-24.2.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 autodoc_typehints = "description"
 autodoc_typehints_description_target = "documented"
 
 # -- Options for HTML output --------------------------------------------------
 
 html_theme = "furo"
 html_theme_options = {
-    "top_of_page_button": None,
+    "top_of_page_buttons": [],
     "light_css_variables": {
         "font-stack": "Inter, sans-serif",
         "font-stack--monospace": "BerkeleyMono, MonoLisa, ui-monospace, "
         "SFMono-Regular, Menlo, Consolas, Liberation Mono, monospace",
     },
 }
 html_logo = "_static/structlog_logo.svg"
```

### Comparing `structlog-24.1.0/docs/configuration.md` & `structlog-24.2.0/docs/configuration.md`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 That can be handy in tests.
 
 At any time, you can check whether and how *structlog* is configured using {func}`structlog.is_configured` and {func}`structlog.get_config`}:
 
 ```pycon
 >>> structlog.is_configured()
 False
->>> structlog.configure(logger_factory=structlog.stdlib.LoggerFactory)
+>>> structlog.configure(logger_factory=structlog.stdlib.LoggerFactory())
 >>> structlog.is_configured()
 True
 >>> cfg = structlog.get_config()
 >>> cfg["logger_factory"]
 <class 'structlog.stdlib.LoggerFactory'>
 ```
```

### Comparing `structlog-24.1.0/docs/console-output.md` & `structlog-24.2.0/docs/console-output.md`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/contextvars.md` & `structlog-24.2.0/docs/contextvars.md`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/exceptions.md` & `structlog-24.2.0/docs/exceptions.md`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/frameworks.md` & `structlog-24.2.0/docs/frameworks.md`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/getting-started.md` & `structlog-24.2.0/docs/getting-started.md`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 What if the parameters are introduced step by step?
 And do you really want to have a logging closure in each of your views?
 
 Let's have a look at a better approach:
 
 ```python
 def view(request):
-    log = logger.bind(
+    log = log.bind(
         user_agent=request.get("HTTP_USER_AGENT", "UNKNOWN"),
         peer_ip=request.client_addr,
     )
 
     if foo := request.get("foo"):
         log = log.bind(foo=foo)
```

### Comparing `structlog-24.1.0/docs/glossary.md` & `structlog-24.2.0/docs/glossary.md`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/index.md` & `structlog-24.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/license.md` & `structlog-24.2.0/docs/license.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 *structlog* is licensed both under the [Apache License, Version 2](https://choosealicense.com/licenses/apache/) and the [MIT license](https://choosealicense.com/licenses/mit/).
 
 Any contribution intentionally submitted for inclusion in the work by you, as defined in the Apache-2.0 license, shall be dual licensed as above, without any additional terms or conditions.
 
 ---
 
-The reason for that is to be both protected against patent claims by own contributors and still allow the usage within GPLv2 software. For more legal details, see [this issue](https://github.com/pyca/cryptography/issues/1209) on the bug tracker of PyCA's `cryptography` project.
+The reason for that is to be both protected against patent claims by own contributors and still allow the usage within GPLv2 software. For more legal details, see [this issue](https://github.com/pyca/cryptography/issues/1209) on the bug tracker of PyCA's *cryptography* project.
 
 The full license texts can be also found in the source code repository:
 
 - [Apache License 2.0](https://github.com/hynek/structlog/blob/main/LICENSE-APACHE)
 - [MIT](https://github.com/hynek/structlog/blob/main/LICENSE-MIT)
```

### Comparing `structlog-24.1.0/docs/logging-best-practices.md` & `structlog-24.2.0/docs/logging-best-practices.md`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/make.bat` & `structlog-24.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/performance.md` & `structlog-24.2.0/docs/performance.md`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/processors.md` & `structlog-24.2.0/docs/processors.md`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/recipes.md` & `structlog-24.2.0/docs/recipes.md`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/standard-library.md` & `structlog-24.2.0/docs/standard-library.md`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,23 @@
 ### Don't Integrate
 
 The most straight-forward option is to configure standard library `logging` close enough to what *structlog* is logging and leaving it at that.
 
 Since these are usually log entries from third parties that don't take advantage of *structlog*'s features, this is surprisingly often a perfectly adequate approach.
 
 For instance, if you log JSON in production, configure `logging` to use [*python-json-logger*] to make it print JSON too, and then tweak the configuration to match their outputs.
+You can also use {class}`~structlog.stdlib.ProcessorFormatter` as a formatter for `logging` to get the same output for both *structlog* and `logging` log entries -- see [below](processor-formatter) for an example.
+
+:::{note}
+If you want to use same file (for example, `sys.stdout` or `sys.stderr`) for both *structlog* and `logging.StreamHandler` output, you must use {class}`~structlog.WriteLogger` instead of {class}`~structlog.PrintLogger`.
+
+This is because {class}`~structlog.PrintLogger` uses `print(log, file=file, flush=True)` to write log, and `print` writes the `log` message and a newline ("\n") to the stream separately.
+This can cause interleaving of log entries from *structlog* and `logging` loggers.
+{class}`~structlog.WriteLogger` writes log entries atomically to the file (for example, `file.write(log+"\n")`).
+:::
 
 
 ### Rendering Within *structlog*
 
 This is the simplest approach where *structlog* does all the heavy lifting and passes a fully-formatted string to `logging`.
 Chances are, this is all you need.
```

### Comparing `structlog-24.1.0/docs/testing.md` & `structlog-24.2.0/docs/testing.md`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/thread-local.md` & `structlog-24.2.0/docs/thread-local.md`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/twisted.md` & `structlog-24.2.0/docs/twisted.md`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/typing.md` & `structlog-24.2.0/docs/typing.md`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/why.md` & `structlog-24.2.0/docs/why.md`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/_static/BoundLogger.svg` & `structlog-24.2.0/docs/_static/BoundLogger.svg`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/_static/console_renderer.png` & `structlog-24.2.0/docs/_static/console_renderer.png`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/_static/social card.afdesign` & `structlog-24.2.0/docs/_static/social card.afdesign`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/_static/structlog_logo.afdesign` & `structlog-24.2.0/docs/_static/structlog_logo.afdesign`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/_static/structlog_logo.png` & `structlog-24.2.0/docs/_static/structlog_logo.png`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/_static/structlog_logo.svg` & `structlog-24.2.0/docs/_static/structlog_logo.svg`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/_static/structlog_logo_horizontal.afdesign` & `structlog-24.2.0/docs/_static/structlog_logo_horizontal.afdesign`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/_static/structlog_logo_horizontal.svg` & `structlog-24.2.0/docs/_static/structlog_logo_horizontal.svg`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/docs/_static/structlog_logo_small.png` & `structlog-24.2.0/docs/_static/structlog_logo_small.png`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/src/structlog/__init__.py` & `structlog-24.2.0/src/structlog/__init__.py`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/src/structlog/_base.py` & `structlog-24.2.0/src/structlog/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,15 @@
         context: Context,
     ):
         self._logger = logger
         self._processors = processors
         self._context = context
 
     def __repr__(self) -> str:
-        return "<{}(context={!r}, processors={!r})>".format(
-            self.__class__.__name__, self._context, self._processors
-        )
+        return f"<{self.__class__.__name__}(context={self._context!r}, processors={self._processors!r})>"
 
     def __eq__(self, other: object) -> bool:
         try:
             return self._context == other._context  # type: ignore[attr-defined]
         except AttributeError:
             return False
```

### Comparing `structlog-24.1.0/src/structlog/_config.py` & `structlog-24.2.0/src/structlog/_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,17 +59,17 @@
     Global defaults.
     """
 
     is_configured: bool = False
     default_processors: Iterable[Processor] = _BUILTIN_DEFAULT_PROCESSORS[:]
     default_context_class: type[Context] = _BUILTIN_DEFAULT_CONTEXT_CLASS
     default_wrapper_class: Any = _BUILTIN_DEFAULT_WRAPPER_CLASS
-    logger_factory: Callable[
-        ..., WrappedLogger
-    ] = _BUILTIN_DEFAULT_LOGGER_FACTORY
+    logger_factory: Callable[..., WrappedLogger] = (
+        _BUILTIN_DEFAULT_LOGGER_FACTORY
+    )
     cache_logger_on_first_use: bool = _BUILTIN_CACHE_LOGGER_ON_FIRST_USE
 
 
 _CONFIG = _Configuration()
 """
 Global defaults used when arguments to `wrap_logger` are omitted.
 """
```

### Comparing `structlog-24.1.0/src/structlog/_frames.py` & `structlog-24.2.0/src/structlog/_frames.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,18 +51,18 @@
         _getframe:
             Callable to find current frame. Only for testing to avoid
             monkeypatching of sys._getframe.
 
     Returns:
         tuple of (frame, name)
     """
-    ignores = ["structlog"] + (additional_ignores or [])
+    ignores = tuple(["structlog"] + (additional_ignores or []))
     f = _ASYNC_CALLING_STACK.get(_getframe())
     name = f.f_globals.get("__name__") or "?"
-    while any(tuple(name.startswith(i) for i in ignores)):
+    while name.startswith(ignores):
         if f.f_back is None:
             name = "?"
             break
         f = f.f_back
         name = f.f_globals.get("__name__") or "?"
     return f, name
```

### Comparing `structlog-24.1.0/src/structlog/_generic.py` & `structlog-24.2.0/src/structlog/_generic.py`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/src/structlog/_greenlets.py` & `structlog-24.2.0/src/structlog/_greenlets.py`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/src/structlog/_log_levels.py` & `structlog-24.2.0/src/structlog/_log_levels.py`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/src/structlog/_native.py` & `structlog-24.2.0/src/structlog/_native.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,16 +206,15 @@
     meths["afatal"] = meths["aerror"]
     meths["warn"] = meths["warning"]
     meths["awarn"] = meths["awarning"]
     meths["msg"] = meths["info"]
     meths["amsg"] = meths["ainfo"]
 
     return type(
-        "BoundLoggerFilteringAt%s"
-        % (LEVEL_TO_NAME.get(min_level, "Notset").capitalize()),
+        f"BoundLoggerFilteringAt{LEVEL_TO_NAME.get(min_level, 'Notset').capitalize()}",
         (BoundLoggerBase,),
         meths,
     )
 
 
 # Pre-create all possible filters to make them pickleable.
 BoundLoggerFilteringAtNotset = _make_filtering_bound_logger(NOTSET)
```

### Comparing `structlog-24.1.0/src/structlog/_output.py` & `structlog-24.2.0/src/structlog/_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 import sys
 import threading
 
 from pickle import PicklingError
 from sys import stderr, stdout
 from typing import IO, Any, BinaryIO, TextIO
 
-from structlog._utils import until_not_interrupted
-
 
 WRITE_LOCKS: dict[IO[Any], threading.Lock] = {}
 
 
 def _get_lock_for_file(file: IO[Any]) -> threading.Lock:
     lock = WRITE_LOCKS.get(file)
     if lock is None:
@@ -105,15 +103,15 @@
 
     def msg(self, message: str) -> None:
         """
         Print *message*.
         """
         f = self._file if self._file is not stdout else None
         with self._lock:
-            until_not_interrupted(print, message, file=f, flush=True)
+            print(message, file=f, flush=True)
 
     log = debug = info = warn = warning = msg
     fatal = failure = err = error = critical = exception = msg
 
 
 class PrintLoggerFactory:
     r"""
@@ -212,16 +210,16 @@
         return f"<WriteLogger(file={self._file!r})>"
 
     def msg(self, message: str) -> None:
         """
         Write and flush *message*.
         """
         with self._lock:
-            until_not_interrupted(self._write, message + "\n")
-            until_not_interrupted(self._flush)
+            self._write(message + "\n")
+            self._flush()
 
     log = debug = info = warn = warning = msg
     fatal = failure = err = error = critical = exception = msg
 
 
 class WriteLoggerFactory:
     r"""
@@ -253,14 +251,15 @@
 
     Useful if you follow `current logging best practices
     <logging-best-practices>` together with a formatter that returns bytes
     (e.g. `orjson <https://github.com/ijl/orjson>`_).
 
     .. versionadded:: 20.2.0
     """
+
     __slots__ = ("_file", "_write", "_flush", "_lock")
 
     def __init__(self, file: BinaryIO | None = None):
         self._file = file or sys.stdout.buffer
         self._write = self._file.write
         self._flush = self._file.flush
 
@@ -315,16 +314,16 @@
         return f"<BytesLogger(file={self._file!r})>"
 
     def msg(self, message: bytes) -> None:
         """
         Write *message*.
         """
         with self._lock:
-            until_not_interrupted(self._write, message + b"\n")
-            until_not_interrupted(self._flush)
+            self._write(message + b"\n")
+            self._flush()
 
     log = debug = info = warn = warning = msg
     fatal = failure = err = error = critical = exception = msg
 
 
 class BytesLoggerFactory:
     r"""
@@ -335,14 +334,15 @@
     Args:
         file: File to print to. (default: `sys.stdout`\ ``.buffer``)
 
     Positional arguments are silently ignored.
 
     .. versionadded:: 20.2.0
     """
+
     __slots__ = ("_file",)
 
     def __init__(self, file: BinaryIO | None = None):
         self._file = file
 
     def __call__(self, *args: Any) -> BytesLogger:
         return BytesLogger(self._file)
```

### Comparing `structlog-24.1.0/src/structlog/contextvars.py` & `structlog-24.2.0/src/structlog/contextvars.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 
 from .typing import BindableLogger, EventDict, WrappedLogger
 
 
 STRUCTLOG_KEY_PREFIX = "structlog_"
 STRUCTLOG_KEY_PREFIX_LEN = len(STRUCTLOG_KEY_PREFIX)
 
-_ASYNC_CALLING_STACK: contextvars.ContextVar[
-    FrameType
-] = contextvars.ContextVar("_ASYNC_CALLING_STACK")
+_ASYNC_CALLING_STACK: contextvars.ContextVar[FrameType] = (
+    contextvars.ContextVar("_ASYNC_CALLING_STACK")
+)
 
 # For proper isolation, we have to use a dict of ContextVars instead of a
 # single ContextVar with a dict.
 # See https://github.com/hynek/structlog/pull/302 for details.
 _CONTEXT_VARS: dict[str, contextvars.ContextVar[Any]] = {}
```

### Comparing `structlog-24.1.0/src/structlog/dev.py` & `structlog-24.2.0/src/structlog/dev.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the MIT License.  See the LICENSE file in the root of this
 # repository for complete details.
 
 """
 Helpers that make development with *structlog* more pleasant.
 
-See also the narrative documentation in `development`.
+See also the narrative documentation in `console-output`.
 """
 
 from __future__ import annotations
 
 import shutil
 import sys
 import warnings
@@ -279,26 +279,37 @@
             A dictionary of level names to styles that are applied to it. If
             None, the level is formatted as a plain ``[level]``.
 
         reset_style:
             What to use to reset the style after the level name. Ignored if
             if *level_styles* is None.
 
+        width:
+            The width to pad the level to. If 0, no padding is done.
+
     .. versionadded:: 23.3.0
+    .. versionadded:: 24.2.0 *width*
     """
 
     level_styles: dict[str, str] | None
     reset_style: str
     width: int
 
-    def __init__(self, level_styles: dict[str, str], reset_style: str) -> None:
+    def __init__(
+        self,
+        level_styles: dict[str, str],
+        reset_style: str,
+        width: int | None = None,
+    ) -> None:
         self.level_styles = level_styles
         if level_styles:
-            self.width = len(
-                max(self.level_styles.keys(), key=lambda e: len(e))
+            self.width = (
+                0
+                if width == 0
+                else len(max(self.level_styles.keys(), key=lambda e: len(e)))
             )
             self.reset_style = reset_style
         else:
             self.width = 0
             self.reset_style = ""
 
     def __call__(self, key: str, value: object) -> str:
@@ -417,15 +428,15 @@
 elif better_exceptions is not None:
     default_exception_formatter = better_traceback
 else:
     default_exception_formatter = plain_traceback
 
 
 class ConsoleRenderer:
-    """
+    r"""
     Render ``event_dict`` nicely aligned, possibly in colors, and ordered.
 
     If ``event_dict`` contains a true-ish ``exc_info`` key, it will be rendered
     *after* the log line. If Rich_ or better-exceptions_ are present, in colors
     and with extra context.
 
     Args:
@@ -450,16 +461,16 @@
         force_colors:
             Force colors even for non-tty destinations. Use this option if your
             logs are stored in a file that is meant to be streamed to the
             console. Only meaningful on Windows. Ignored if *columns* are
             passed.
 
         repr_native_str:
-            When `True`, `repr` is also applied to ``str``s. The ``event`` key
-            is *never* `repr` -ed. Ignored if *columns* are passed.
+            When `True`, `repr` is also applied to ``str``\ s. The ``event``
+            key is *never* `repr` -ed. Ignored if *columns* are passed.
 
         level_styles:
             When present, use these styles for colors. This must be a dict from
             level names (strings) to Colorama styles. The default can be
             obtained by calling `ConsoleRenderer.get_default_level_styles`.
             Ignored when *columns* are passed.
 
@@ -481,14 +492,18 @@
             *columns* are passed.
 
         timestamp_key:
             The key to look for timestamp of the log message. Needed when you
             rename it e.g. using `structlog.processors.EventRenamer`. Ignored
             if *columns* are passed.
 
+        pad_level:
+            Whether to pad log level with blanks to the longest amongst all
+            level label.
+
     Requires the Colorama_ package if *colors* is `True` **on Windows**.
 
     Raises:
         ValueError: If there's not exactly one default column formatter.
 
     .. _Colorama: https://pypi.org/project/colorama/
     .. _better-exceptions: https://pypi.org/project/better-exceptions/
@@ -520,28 +535,30 @@
        The colors keyword now defaults to True on non-Windows systems, and
        either True or False in Windows depending on whether Colorama is
        installed.
     .. versionadded:: 21.3.0 *sort_keys*
     .. versionadded:: 22.1.0 *event_key*
     .. versionadded:: 23.2.0 *timestamp_key*
     .. versionadded:: 23.3.0 *columns*
+    .. versionadded:: 24.2.0 *pad_level*
     """
 
-    def __init__(  # noqa: PLR0912
+    def __init__(  # noqa: PLR0912, PLR0915
         self,
         pad_event: int = _EVENT_WIDTH,
         colors: bool = _has_colors,
         force_colors: bool = False,
         repr_native_str: bool = False,
         level_styles: Styles | None = None,
         exception_formatter: ExceptionRenderer = default_exception_formatter,
         sort_keys: bool = True,
         event_key: str = "event",
         timestamp_key: str = "timestamp",
         columns: list[Column] | None = None,
+        pad_level: bool = True,
     ):
         self._exception_formatter = exception_formatter
         self._sort_keys = sort_keys
 
         if columns is not None:
             to_warn = []
 
@@ -641,28 +658,30 @@
             value_style=styles.bright + styles.logger_name,
             reset_style=styles.reset,
             value_repr=str,
             prefix="[",
             postfix="]",
         )
 
+        level_width = 0 if not pad_level else None
+
         self._columns = [
             Column(
                 timestamp_key,
                 KeyValueColumnFormatter(
                     key_style=None,
                     value_style=styles.timestamp,
                     reset_style=styles.reset,
                     value_repr=str,
                 ),
             ),
             Column(
                 "level",
                 LogLevelColumnFormatter(
-                    level_to_color, reset_style=styles.reset
+                    level_to_color, reset_style=styles.reset, width=level_width
                 ),
             ),
             Column(
                 event_key,
                 KeyValueColumnFormatter(
                     key_style=None,
                     value_style=styles.bright,
```

### Comparing `structlog-24.1.0/src/structlog/processors.py` & `structlog-24.2.0/src/structlog/processors.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 Processors useful regardless of the logging framework.
 """
 
 from __future__ import annotations
 
 import datetime
 import enum
-import inspect
 import json
 import logging
 import operator
 import os
 import sys
 import threading
 import time
 
+from types import FrameType
 from typing import (
     Any,
     Callable,
     ClassVar,
     Collection,
     NamedTuple,
     Sequence,
@@ -132,15 +132,15 @@
 
         bool_as_flag:
             When ``True``, render ``{"flag": True}`` as ``flag``, instead of
             ``flag=true``. ``{"flag": False}`` is always rendered as
             ``flag=false``.
 
     Raises:
-        ValueError: If a key contains non printable or space characters.
+        ValueError: If a key contains non-printable or whitespace characters.
 
     .. versionadded:: 21.5.0
     """
 
     def __init__(
         self,
         sort_keys: bool = False,
@@ -166,17 +166,24 @@
 
             if isinstance(value, bool):
                 if self.bool_as_flag and value:
                     elements.append(f"{key}")
                     continue
                 value = "true" if value else "false"
 
-            value = f"{value}".replace('"', '\\"')
+            value = str(value)
+            backslashes_need_escaping = (
+                " " in value or "=" in value or '"' in value
+            )
+            if backslashes_need_escaping and "\\" in value:
+                value = value.replace("\\", "\\\\")
+
+            value = value.replace('"', '\\"').replace("\n", "\\n")
 
-            if " " in value or "=" in value:
+            if backslashes_need_escaping:
                 value = f'"{value}"'
 
             elements.append(f"{key}={value}")
 
         return " ".join(elements)
 
 
@@ -713,14 +720,50 @@
     THREAD_NAME = "thread_name"
     #: The ID of the process the callsite was executed in.
     PROCESS = "process"
     #: The name of the process the callsite was executed in.
     PROCESS_NAME = "process_name"
 
 
+def _get_callsite_pathname(module: str, frame: FrameType) -> Any:
+    return frame.f_code.co_filename
+
+
+def _get_callsite_filename(module: str, frame: FrameType) -> Any:
+    return os.path.basename(frame.f_code.co_filename)
+
+
+def _get_callsite_module(module: str, frame: FrameType) -> Any:
+    return os.path.splitext(os.path.basename(frame.f_code.co_filename))[0]
+
+
+def _get_callsite_func_name(module: str, frame: FrameType) -> Any:
+    return frame.f_code.co_name
+
+
+def _get_callsite_lineno(module: str, frame: FrameType) -> Any:
+    return frame.f_lineno
+
+
+def _get_callsite_thread(module: str, frame: FrameType) -> Any:
+    return threading.get_ident()
+
+
+def _get_callsite_thread_name(module: str, frame: FrameType) -> Any:
+    return threading.current_thread().name
+
+
+def _get_callsite_process(module: str, frame: FrameType) -> Any:
+    return os.getpid()
+
+
+def _get_callsite_process_name(module: str, frame: FrameType) -> Any:
+    return get_processname()
+
+
 class CallsiteParameterAdder:
     """
     Adds parameters of the callsite that an event dictionary originated from to
     the event dictionary. This processor can be used to enrich events
     dictionaries with information such as the function name, line number and
     filename that an event dictionary originated from.
 
@@ -754,43 +797,25 @@
         ``processors`` of `structlog.configure` and ``foreign_pre_chain`` of
         `structlog.stdlib.ProcessorFormatter`.
 
     .. versionadded:: 21.5.0
     """
 
     _handlers: ClassVar[
-        dict[CallsiteParameter, Callable[[str, inspect.Traceback], Any]]
+        dict[CallsiteParameter, Callable[[str, FrameType], Any]]
     ] = {
-        CallsiteParameter.PATHNAME: (
-            lambda module, frame_info: frame_info.filename
-        ),
-        CallsiteParameter.FILENAME: (
-            lambda module, frame_info: os.path.basename(frame_info.filename)
-        ),
-        CallsiteParameter.MODULE: (
-            lambda module, frame_info: os.path.splitext(
-                os.path.basename(frame_info.filename)
-            )[0]
-        ),
-        CallsiteParameter.FUNC_NAME: (
-            lambda module, frame_info: frame_info.function
-        ),
-        CallsiteParameter.LINENO: (
-            lambda module, frame_info: frame_info.lineno
-        ),
-        CallsiteParameter.THREAD: (
-            lambda module, frame_info: threading.get_ident()
-        ),
-        CallsiteParameter.THREAD_NAME: (
-            lambda module, frame_info: threading.current_thread().name
-        ),
-        CallsiteParameter.PROCESS: (lambda module, frame_info: os.getpid()),
-        CallsiteParameter.PROCESS_NAME: (
-            lambda module, frame_info: get_processname()
-        ),
+        CallsiteParameter.PATHNAME: _get_callsite_pathname,
+        CallsiteParameter.FILENAME: _get_callsite_filename,
+        CallsiteParameter.MODULE: _get_callsite_module,
+        CallsiteParameter.FUNC_NAME: _get_callsite_func_name,
+        CallsiteParameter.LINENO: _get_callsite_lineno,
+        CallsiteParameter.THREAD: _get_callsite_thread,
+        CallsiteParameter.THREAD_NAME: _get_callsite_thread_name,
+        CallsiteParameter.PROCESS: _get_callsite_process,
+        CallsiteParameter.PROCESS_NAME: _get_callsite_process_name,
     }
     _record_attribute_map: ClassVar[dict[CallsiteParameter, str]] = {
         CallsiteParameter.PATHNAME: "pathname",
         CallsiteParameter.FILENAME: "filename",
         CallsiteParameter.MODULE: "module",
         CallsiteParameter.FUNC_NAME: "funcName",
         CallsiteParameter.LINENO: "lineno",
@@ -816,15 +841,15 @@
         if additional_ignores is None:
             additional_ignores = []
         # Ignore stack frames from the logging module. They will occur if this
         # processor is used in ProcessorFormatter, and additionally the logging
         # module should not be logging using structlog.
         self._additional_ignores = ["logging", *additional_ignores]
         self._active_handlers: list[
-            tuple[CallsiteParameter, Callable[[str, inspect.Traceback], Any]]
+            tuple[CallsiteParameter, Callable[[str, FrameType], Any]]
         ] = []
         self._record_mappings: list[CallsiteParameterAdder._RecordMapping] = []
         for parameter in parameters:
             self._active_handlers.append(
                 (parameter, self._handlers[parameter])
             )
             self._record_mappings.append(
@@ -846,17 +871,16 @@
                 event_dict[mapping.event_dict_key] = record.__dict__[
                     mapping.record_attribute
                 ]
         else:
             frame, module = _find_first_app_frame_and_name(
                 additional_ignores=self._additional_ignores
             )
-            frame_info = inspect.getframeinfo(frame)
             for parameter, handler in self._active_handlers:
-                event_dict[parameter.value] = handler(module, frame_info)
+                event_dict[parameter.value] = handler(module, frame)
         return event_dict
 
 
 class EventRenamer:
     r"""
     Rename the ``event`` key in event dicts.
```

### Comparing `structlog-24.1.0/src/structlog/stdlib.py` & `structlog-24.2.0/src/structlog/stdlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,18 @@
         )
 
     It also contains a bunch of properties that pass-through to the wrapped
     `logging.Logger` which should make it work as a drop-in replacement.
 
     .. versionadded:: 23.1.0
        Async variants `alog()`, `adebug()`, `ainfo()`, and so forth.
+
+    .. versionchanged:: 24.2.0
+        Callsite parameters are now also collected by
+        `structlog.processors.CallsiteParameterAdder` for async log methods.
     """
 
     _logger: logging.Logger
 
     def bind(self, **new_values: Any) -> BoundLogger:
         """
         Return a new logger with *new_values* added to the existing ones.
@@ -389,20 +393,24 @@
         event: str,
         args: tuple[Any, ...],
         kw: dict[str, Any],
     ) -> None:
         """
         Merge contextvars and log using the sync logger in a thread pool.
         """
+        scs_token = _ASYNC_CALLING_STACK.set(sys._getframe().f_back.f_back)  # type: ignore[union-attr, arg-type, unused-ignore]
         ctx = contextvars.copy_context()
 
-        await asyncio.get_running_loop().run_in_executor(
-            None,
-            lambda: ctx.run(lambda: meth(event, *args, **kw)),
-        )
+        try:
+            await asyncio.get_running_loop().run_in_executor(
+                None,
+                lambda: ctx.run(lambda: meth(event, *args, **kw)),
+            )
+        finally:
+            _ASYNC_CALLING_STACK.reset(scs_token)
 
     async def adebug(self, event: str, *args: Any, **kw: Any) -> None:
         """
         Log using `debug()`, but asynchronously in a separate thread.
 
         .. versionadded:: 23.1.0
         """
@@ -495,14 +503,16 @@
 
     Only available for Python 3.7 and later.
 
     .. versionadded:: 20.2.0
     .. versionchanged:: 20.2.0 fix _dispatch_to_sync contextvars usage
     .. deprecated:: 23.1.0
        Use the regular `BoundLogger` with its a-prefixed methods instead.
+    .. versionchanged:: 23.3.0
+        Callsite parameters are now also collected for async log methods.
     """
 
     __slots__ = ("sync_bl", "_loop")
 
     #: The wrapped synchronous logger. It is useful to be able to log
     #: synchronously occasionally.
     sync_bl: BoundLogger
@@ -590,16 +600,14 @@
         meth: Callable[..., Any],
         event: str,
         args: tuple[Any, ...],
         kw: dict[str, Any],
     ) -> None:
         """
         Merge contextvars and log using the sync logger in a thread pool.
-        .. versionchanged:: 23.3.0
-           Callsite parameters are now also collected under asyncio.
         """
         scs_token = _ASYNC_CALLING_STACK.set(sys._getframe().f_back.f_back)  # type: ignore[union-attr, arg-type, unused-ignore]
         ctx = contextvars.copy_context()
 
         try:
             await asyncio.get_running_loop().run_in_executor(
                 self._executor,
@@ -866,31 +874,34 @@
 
 
 def render_to_log_kwargs(
     _: logging.Logger, __: str, event_dict: EventDict
 ) -> EventDict:
     """
     Render ``event_dict`` into keyword arguments for `logging.log`.
+    See `logging.Logger`'s ``_log`` method for kwargs reference.
 
     The ``event`` field is translated into ``msg`` and the rest of the
     *event_dict* is added as ``extra``.
 
     This allows you to defer formatting to `logging`.
 
     .. versionadded:: 17.1.0
     .. versionchanged:: 22.1.0
-       ``exc_info``, ``stack_info``, and ``stackLevel`` are passed as proper
+       ``exc_info``, ``stack_info``, and ``stacklevel`` are passed as proper
        kwargs and not put into ``extra``.
+    .. versionchanged:: 24.2.0
+       ``stackLevel`` corrected to ``stacklevel``.
     """
     return {
         "msg": event_dict.pop("event"),
         "extra": event_dict,
         **{
             kw: event_dict.pop(kw)
-            for kw in ("exc_info", "stack_info", "stackLevel")
+            for kw in ("exc_info", "stack_info", "stacklevel")
             if kw in event_dict
         },
     }
 
 
 class ProcessorFormatter(logging.Formatter):
     r"""
```

### Comparing `structlog-24.1.0/src/structlog/testing.py` & `structlog-24.2.0/src/structlog/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,14 +195,15 @@
 
     To be used with `structlog.configure`\ 's *logger_factory*.
 
     Positional arguments are silently ignored.
 
     .. versionadded:: 20.2.0
     """
+
     logger: CapturingLogger
 
     def __init__(self) -> None:
         self.logger = CapturingLogger()
 
     def __call__(self, *args: Any) -> CapturingLogger:
         return self.logger
```

### Comparing `structlog-24.1.0/src/structlog/threadlocal.py` & `structlog-24.2.0/src/structlog/threadlocal.py`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/src/structlog/tracebacks.py` & `structlog-24.2.0/src/structlog/tracebacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     Container for a list of stack traces.
     """
 
     stacks: list[Stack]
 
 
 def safe_str(_object: Any) -> str:
-    """Don't allow exceptions from __str__ to propegate."""
+    """Don't allow exceptions from __str__ to propagate."""
     try:
         return str(_object)
     except Exception as error:  # noqa: BLE001
         return f"<str-error {str(error)!r}>"
 
 
 def to_repr(obj: Any, max_string: int | None = None) -> str:
@@ -173,20 +173,22 @@
             filename = frame_summary.f_code.co_filename
             if filename and not filename.startswith("<"):
                 filename = os.path.abspath(filename)
             frame = Frame(
                 filename=filename or "?",
                 lineno=line_no,
                 name=frame_summary.f_code.co_name,
-                locals={
-                    key: to_repr(value, max_string=locals_max_string)
-                    for key, value in frame_summary.f_locals.items()
-                }
-                if show_locals
-                else None,
+                locals=(
+                    {
+                        key: to_repr(value, max_string=locals_max_string)
+                        for key, value in frame_summary.f_locals.items()
+                    }
+                    if show_locals
+                    else None
+                ),
             )
             append(frame)
 
         cause = getattr(exc_value, "__cause__", None)
         if cause and cause.__traceback__:
             exc_type = cause.__class__
             exc_value = cause
```

### Comparing `structlog-24.1.0/src/structlog/twisted.py` & `structlog-24.2.0/src/structlog/twisted.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from twisted.python import log
 from twisted.python.failure import Failure
 from twisted.python.log import ILogObserver, textFromEventDict
 from zope.interface import implementer
 
 from ._base import BoundLoggerBase
 from ._config import _BUILTIN_DEFAULT_PROCESSORS
-from ._utils import until_not_interrupted
 from .processors import JSONRenderer as GenericJSONRenderer
 from .typing import EventDict, WrappedLogger
 
 
 class BoundLogger(BoundLoggerBase):
     """
     Twisted-specific version of `structlog.BoundLogger`.
@@ -211,20 +210,19 @@
     """
 
     def __init__(self, file: TextIO) -> None:
         self._write = file.write
         self._flush = file.flush
 
     def __call__(self, eventDict: EventDict) -> None:
-        until_not_interrupted(
-            self._write,
+        self._write(
             textFromEventDict(eventDict)  # type: ignore[arg-type, operator]
             + "\n",
         )
-        until_not_interrupted(self._flush)
+        self._flush()
 
 
 @implementer(ILogObserver)
 class JSONLogObserverWrapper:
     """
     Wrap a log *observer* and render non-`JSONRenderer` entries to JSON.
 
@@ -299,16 +297,17 @@
     **Must** be the last processor in the chain and requires a *dictRenderer*
     for the actual formatting as an constructor argument in order to be able to
     fully support the original behaviors of ``log.msg()`` and ``log.err()``.
     """
 
     def __init__(
         self,
-        dictRenderer: Callable[[WrappedLogger, str, EventDict], str]
-        | None = None,
+        dictRenderer: (
+            Callable[[WrappedLogger, str, EventDict], str] | None
+        ) = None,
     ) -> None:
         self._dictRenderer = dictRenderer or _BUILTIN_DEFAULT_PROCESSORS[-1]
 
     def __call__(
         self, logger: WrappedLogger, name: str, eventDict: EventDict
     ) -> Any:
         if name == "err":
```

### Comparing `structlog-24.1.0/src/structlog/types.py` & `structlog-24.2.0/src/structlog/types.py`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/src/structlog/typing.py` & `structlog-24.2.0/src/structlog/typing.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,40 +112,35 @@
     Returns:
         Anything that can be rendered by the last processor in your chain, for
         example, a string or a JSON-serializable structure.
 
     .. versionadded:: 22.1.0
     """
 
-    def __call__(self, exc_info: ExcInfo) -> Any:
-        ...
+    def __call__(self, exc_info: ExcInfo) -> Any: ...
 
 
 @runtime_checkable
 class BindableLogger(Protocol):
     """
     **Protocol**: Methods shared among all bound loggers and that are relied on
     by *structlog*.
 
     .. versionadded:: 20.2.0
     """
 
     _context: Context
 
-    def bind(self, **new_values: Any) -> BindableLogger:
-        ...
+    def bind(self, **new_values: Any) -> BindableLogger: ...
 
-    def unbind(self, *keys: str) -> BindableLogger:
-        ...
+    def unbind(self, *keys: str) -> BindableLogger: ...
 
-    def try_unbind(self, *keys: str) -> BindableLogger:
-        ...
+    def try_unbind(self, *keys: str) -> BindableLogger: ...
 
-    def new(self, **new_values: Any) -> BindableLogger:
-        ...
+    def new(self, **new_values: Any) -> BindableLogger: ...
 
 
 class FilteringBoundLogger(BindableLogger, Protocol):
     """
     **Protocol**: A `BindableLogger` that filters by a level.
 
     The only way to instantiate one is using `make_filtering_bound_logger`.
```

### Comparing `structlog-24.1.0/tests/conftest.py` & `structlog-24.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/tests/test_base.py` & `structlog-24.2.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/tests/test_config.py` & `structlog-24.2.0/tests/test_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     """
     If someone defines an attribute on an ABC with a logger, that logger is not
     detected as an abstract method.
 
     See https://github.com/hynek/structlog/issues/229
     """
 
-    class Foo(metaclass=abc.ABCMeta):
+    class Foo(metaclass=abc.ABCMeta):  # noqa: B024
         log = structlog.get_logger()
 
     Foo()
 
 
 def test_lazy_logger_is_an_instance_of_bindable_logger():
     """
```

### Comparing `structlog-24.1.0/tests/test_contextvars.py` & `structlog-24.2.0/tests/test_contextvars.py`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/tests/test_dev.py` & `structlog-24.2.0/tests/test_dev.py`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/tests/test_frames.py` & `structlog-24.2.0/tests/test_frames.py`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/tests/test_generic.py` & `structlog-24.2.0/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/tests/test_log_levels.py` & `structlog-24.2.0/tests/test_log_levels.py`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/tests/test_output.py` & `structlog-24.2.0/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/tests/test_packaging.py` & `structlog-24.2.0/tests/test_packaging.py`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/tests/test_processors.py` & `structlog-24.2.0/tests/test_stdlib.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,1151 +1,1451 @@
 # SPDX-License-Identifier: MIT OR Apache-2.0
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the MIT License.  See the LICENSE file in the root of this
 # repository for complete details.
 
 from __future__ import annotations
 
-import datetime
-import functools
-import inspect
-import itertools
 import json
 import logging
+import logging.config
 import os
-import pickle
 import sys
-import threading
 
 from io import StringIO
+from typing import Any, Callable, Collection, Dict
+from unittest.mock import patch
 
 import pytest
+import pytest_asyncio
 
-from freezegun import freeze_time
+from pretend import call_recorder, stub
 
-import structlog
-
-from structlog import BoundLogger
-from structlog._utils import get_processname
-from structlog.processors import (
-    CallsiteParameter,
-    CallsiteParameterAdder,
-    EventRenamer,
-    ExceptionPrettyPrinter,
-    ExceptionRenderer,
-    JSONRenderer,
-    KeyValueRenderer,
-    LogfmtRenderer,
-    MaybeTimeStamper,
-    StackInfoRenderer,
-    TimeStamper,
-    UnicodeDecoder,
-    UnicodeEncoder,
-    _figure_out_exc_info,
-    _json_fallback_handler,
-    format_exc_info,
+from structlog import (
+    PrintLogger,
+    ReturnLogger,
+    configure,
+    get_context,
+    wrap_logger,
+)
+from structlog._config import _CONFIG
+from structlog._log_levels import CRITICAL, NAME_TO_LEVEL, WARN
+from structlog.dev import ConsoleRenderer
+from structlog.exceptions import DropEvent
+from structlog.processors import JSONRenderer, KeyValueRenderer
+from structlog.stdlib import (
+    AsyncBoundLogger,
+    BoundLogger,
+    ExtraAdder,
+    LoggerFactory,
+    PositionalArgumentsFormatter,
+    ProcessorFormatter,
+    _FixedFindCallerLogger,
+    add_log_level,
+    add_log_level_number,
+    add_logger_name,
+    filter_by_level,
+    get_logger,
+    recreate_defaults,
+    render_to_log_kwargs,
 )
-from structlog.stdlib import ProcessorFormatter
-from structlog.threadlocal import wrap_dict
-from structlog.typing import EventDict
-from tests.additional_frame import additional_frame
-from tests.utils import CustomError
+from structlog.testing import CapturedCall
+from structlog.typing import BindableLogger, EventDict
 
+from .additional_frame import additional_frame
 
-try:
-    import simplejson
-except ImportError:
-    simplejson = None
 
+def build_bl(logger=None, processors=None, context=None):
+    """
+    Convenience function to build BoundLogger with sane defaults.
+    """
+    return BoundLogger(logger or ReturnLogger(), processors, {})
 
-class TestKeyValueRenderer:
-    def test_sort_keys(self, event_dict):
-        """
-        Keys are sorted if sort_keys is set.
-        """
-        rv = KeyValueRenderer(sort_keys=True)(None, None, event_dict)
 
-        assert r"a=<A(\o/)> b=[3, 4] x=7 y='test' z=(1, 2)" == rv
+def return_method_name(_, method_name, __):
+    """
+    A final renderer that returns the name of the logging method.
+    """
+    return method_name
+
 
-    def test_order_complete(self, event_dict):
+class TestLoggerFactory:
+    def setup_method(self, method):
         """
-        Orders keys according to key_order.
+        The stdlib logger factory modifies global state to fix caller
+        identification.
         """
-        rv = KeyValueRenderer(key_order=["y", "b", "a", "z", "x"])(
-            None, None, event_dict
-        )
+        self.original_logger = logging.getLoggerClass()
 
-        assert r"y='test' b=[3, 4] a=<A(\o/)> z=(1, 2) x=7" == rv
+    def teardown_method(self, method):
+        logging.setLoggerClass(self.original_logger)
 
-    def test_order_missing(self, event_dict):
+    def test_deduces_correct_name(self):
         """
-        Missing keys get rendered as None.
+        The factory isn't called directly but from structlog._config so
+        deducing has to be slightly smarter.
         """
-        rv = KeyValueRenderer(key_order=["c", "y", "b", "a", "z", "x"])(
-            None, None, event_dict
+        assert "tests.additional_frame" == (
+            additional_frame(LoggerFactory()).name
         )
+        assert "tests.test_stdlib" == LoggerFactory()().name
 
-        assert r"c=None y='test' b=[3, 4] a=<A(\o/)> z=(1, 2) x=7" == rv
-
-    def test_order_missing_dropped(self, event_dict):
+    def test_ignores_frames(self):
         """
-        Missing keys get dropped
+        The name guesser walks up the frames until it reaches a frame whose
+        name is not from structlog or one of the configurable other names.
         """
-        rv = KeyValueRenderer(
-            key_order=["c", "y", "b", "a", "z", "x"], drop_missing=True
-        )(None, None, event_dict)
 
-        assert r"y='test' b=[3, 4] a=<A(\o/)> z=(1, 2) x=7" == rv
+        # Compute the names to __main__ so it doesn't get thrown off if people
+        # install plugins that alter the frames. E.g. #370
+        names = set()
+        f = sys._getframe()
+        while f.f_globals["__name__"] != "__main__":
+            names.add(f.f_globals["__name__"].split(".", 1)[0])
+            f = f.f_back
+
+        assert (
+            "__main__"
+            == additional_frame(
+                LoggerFactory(ignore_frame_names=list(names))
+            ).name
+        )
 
-    def test_order_extra(self, event_dict):
+    def test_deduces_correct_caller(self):
         """
-        Extra keys get sorted if sort_keys=True.
+        It will find the correct caller.
         """
-        event_dict["B"] = "B"
-        event_dict["A"] = "A"
+        logger = _FixedFindCallerLogger("test")
 
-        rv = KeyValueRenderer(
-            key_order=["c", "y", "b", "a", "z", "x"], sort_keys=True
-        )(None, None, event_dict)
+        file_name, line_number, func_name = logger.findCaller()[:3]
 
-        assert (
-            r"c=None y='test' b=[3, 4] a=<A(\o/)> z=(1, 2) x=7 A='A' B='B'"
-        ) == rv
+        assert file_name == os.path.realpath(__file__)
+        assert func_name == "test_deduces_correct_caller"
 
-    def test_order_sorted_missing_dropped(self, event_dict):
+    def test_stack_info(self):
         """
-        Keys get sorted if sort_keys=True and extras get dropped.
+        If we ask for stack_info, it will returned.
         """
-        event_dict["B"] = "B"
-        event_dict["A"] = "A"
-
-        rv = KeyValueRenderer(
-            key_order=["c", "y", "b", "a", "z", "x"],
-            sort_keys=True,
-            drop_missing=True,
-        )(None, None, event_dict)
+        logger = _FixedFindCallerLogger("test")
+        testing, is_, fun, stack_info = logger.findCaller(stack_info=True)
 
-        assert r"y='test' b=[3, 4] a=<A(\o/)> z=(1, 2) x=7 A='A' B='B'" == rv
+        assert "testing, is_, fun" in stack_info
 
-    def test_random_order(self, event_dict):
+    def test_no_stack_info_by_default(self):
         """
-        No special ordering doesn't blow up.
+        If we don't ask for stack_info, it won't be returned.
         """
-        rv = KeyValueRenderer()(None, None, event_dict)
+        logger = _FixedFindCallerLogger("test")
+        testing, is_, fun, stack_info = logger.findCaller()
 
-        assert isinstance(rv, str)
+        assert None is stack_info
 
-    @pytest.mark.parametrize("rns", [True, False])
-    def test_repr_native_str(self, rns):
+    def test_find_caller(self, caplog):
         """
-        repr_native_str=False doesn't repr on native strings.
+        The caller is found.
         """
-        rv = KeyValueRenderer(repr_native_str=rns)(
-            None, None, {"event": "哈", "key": 42, "key2": "哈"}
-        )
+        logger = LoggerFactory()()
 
-        cnt = rv.count("哈")
-        assert 2 == cnt
+        logger.error("Test")
 
+        assert caplog.text.startswith(
+            "ERROR    tests.test_stdlib:test_stdlib.py"
+        )
 
-class TestLogfmtRenderer:
-    def test_sort_keys(self, event_dict):
+    def test_sets_correct_logger(self):
         """
-        Keys are sorted if sort_keys is set.
+        Calling LoggerFactory ensures that Logger.findCaller gets patched.
         """
-        rv = LogfmtRenderer(sort_keys=True)(None, None, event_dict)
+        LoggerFactory()
 
-        assert r'a=<A(\o/)> b="[3, 4]" x=7 y=test z="(1, 2)"' == rv
+        assert logging.getLoggerClass() is _FixedFindCallerLogger
 
-    def test_order_complete(self, event_dict):
+    def test_positional_argument_avoids_guessing(self):
         """
-        Orders keys according to key_order.
+        If a positional argument is passed to the factory, it's used as the
+        name instead of guessing.
         """
-        rv = LogfmtRenderer(key_order=["y", "b", "a", "z", "x"])(
-            None, None, event_dict
-        )
+        lf = LoggerFactory()("foo")
 
-        assert r'y=test b="[3, 4]" a=<A(\o/)> z="(1, 2)" x=7' == rv
+        assert "foo" == lf.name
 
-    def test_order_missing(self, event_dict):
+
+class TestFilterByLevel:
+    def test_filters_lower_levels(self):
         """
-        Missing keys get rendered as None.
+        Log entries below the current level raise a DropEvent.
         """
-        rv = LogfmtRenderer(key_order=["c", "y", "b", "a", "z", "x"])(
-            None, None, event_dict
-        )
+        logger = logging.Logger(__name__)
+        logger.setLevel(CRITICAL)
 
-        assert r'c= y=test b="[3, 4]" a=<A(\o/)> z="(1, 2)" x=7' == rv
+        with pytest.raises(DropEvent):
+            filter_by_level(logger, "warn", {})
 
-    def test_order_missing_dropped(self, event_dict):
+    def test_passes_higher_levels(self):
         """
-        Missing keys get dropped
+        Log entries with higher levels are passed through unchanged.
         """
-        rv = LogfmtRenderer(
-            key_order=["c", "y", "b", "a", "z", "x"], drop_missing=True
-        )(None, None, event_dict)
+        logger = logging.Logger(__name__)
+        logger.setLevel(WARN)
+        event_dict = {"event": "test"}
+
+        assert event_dict is filter_by_level(logger, "warn", event_dict)
+        assert event_dict is filter_by_level(logger, "error", event_dict)
+        assert event_dict is filter_by_level(logger, "exception", event_dict)
 
-        assert r'y=test b="[3, 4]" a=<A(\o/)> z="(1, 2)" x=7' == rv
 
-    def test_order_extra(self, event_dict):
+class TestBoundLogger:
+    @pytest.mark.parametrize(
+        ("method_name"),
+        ["debug", "info", "warning", "error", "exception", "critical"],
+    )
+    def test_proxies_to_correct_method(self, method_name):
         """
-        Extra keys get sorted if sort_keys=True.
+        The basic proxied methods are proxied to the correct counterparts.
         """
-        event_dict["B"] = "B"
-        event_dict["A"] = "A"
+        bl = BoundLogger(ReturnLogger(), [return_method_name], {})
 
-        rv = LogfmtRenderer(
-            key_order=["c", "y", "b", "a", "z", "x"], sort_keys=True
-        )(None, None, event_dict)
+        assert method_name == getattr(bl, method_name)("event")
 
-        assert (
-            r'c= y=test b="[3, 4]" a=<A(\o/)> z="(1, 2)" x=7 A=A B=B'
-        ) == rv
-
-    def test_order_sorted_missing_dropped(self, event_dict):
+    def test_proxies_log(self):
         """
-        Keys get sorted if sort_keys=True and extras get dropped.
+        BoundLogger.exception.log() is proxied to the appropriate method.
         """
-        event_dict["B"] = "B"
-        event_dict["A"] = "A"
-
-        rv = LogfmtRenderer(
-            key_order=["c", "y", "b", "a", "z", "x"],
-            sort_keys=True,
-            drop_missing=True,
-        )(None, None, event_dict)
+        bl = BoundLogger(ReturnLogger(), [return_method_name], {})
 
-        assert r'y=test b="[3, 4]" a=<A(\o/)> z="(1, 2)" x=7 A=A B=B' == rv
+        assert "critical" == bl.log(50, "event")
+        assert "debug" == bl.log(10, "event")
 
-    def test_random_order(self, event_dict):
+    def test_positional_args_proxied(self):
         """
-        No special ordering doesn't blow up.
+        Positional arguments supplied are proxied as kwarg.
         """
-        rv = LogfmtRenderer()(None, None, event_dict)
+        bl = BoundLogger(ReturnLogger(), [], {})
+        args, kwargs = bl.debug("event", "foo", bar="baz")
 
-        assert isinstance(rv, str)
+        assert "baz" == kwargs.get("bar")
+        assert ("foo",) == kwargs.get("positional_args")
 
-    def test_empty_event_dict(self):
+    @pytest.mark.parametrize(
+        "attribute_name",
+        ["name", "level", "parent", "propagate", "handlers", "disabled"],
+    )
+    def test_stdlib_passthrough_attributes(self, attribute_name):
         """
-        Empty event dict renders as empty string.
+        stdlib logger attributes are also available in stdlib BoundLogger.
         """
-        rv = LogfmtRenderer()(None, None, {})
+        stdlib_logger = logging.getLogger("Test")
+        stdlib_logger_attribute = getattr(stdlib_logger, attribute_name)
+        bl = BoundLogger(stdlib_logger, [], {})
+        bound_logger_attribute = getattr(bl, attribute_name)
 
-        assert "" == rv
+        assert bound_logger_attribute == stdlib_logger_attribute
 
-    def test_bool_as_flag(self):
+    @pytest.mark.parametrize(
+        ("method_name", "method_args"),
+        [
+            ("addHandler", [None]),
+            ("removeHandler", [None]),
+            ("hasHandlers", None),
+            ("callHandlers", [None]),
+            ("handle", [None]),
+            ("setLevel", [None]),
+            ("getEffectiveLevel", None),
+            ("isEnabledFor", [None]),
+            ("findCaller", None),
+            (
+                "makeRecord",
+                [
+                    "name",
+                    "debug",
+                    "test_func",
+                    "1",
+                    "test msg",
+                    ["foo"],
+                    False,
+                ],
+            ),
+            ("getChild", [None]),
+        ],
+    )
+    def test_stdlib_passthrough_methods(self, method_name, method_args):
         """
-        If activated, render ``{"a": True}`` as ``a`` instead of ``a=true``.
+        stdlib logger methods are also available in stdlib BoundLogger.
         """
-        event_dict = {"a": True, "b": False}
+        called_stdlib_method = [False]
 
-        rv_abbrev = LogfmtRenderer(bool_as_flag=True)(None, None, event_dict)
-        assert r"a b=false" == rv_abbrev
+        def validate(*args, **kw):
+            called_stdlib_method[0] = True
 
-        rv_no_abbrev = LogfmtRenderer(bool_as_flag=False)(
-            None, None, event_dict
-        )
-        assert r"a=true b=false" == rv_no_abbrev
+        stdlib_logger = logging.getLogger("Test")
+        stdlib_logger_method = getattr(stdlib_logger, method_name, None)
+        if stdlib_logger_method:
+            setattr(stdlib_logger, method_name, validate)
+            bl = BoundLogger(stdlib_logger, [], {})
+            bound_logger_method = getattr(bl, method_name)
 
-    def test_reference_format(self):
-        """
-        Test rendering according to example at
-        https://pkg.go.dev/github.com/kr/logfmt
-        """
-        event_dict = {
-            "foo": "bar",
-            "a": 14,
-            "baz": "hello kitty",
-            "cool%story": "bro",
-            "f": True,
-            "%^asdf": True,
-        }
+            assert bound_logger_method is not None
+
+            if method_args:
+                bound_logger_method(*method_args)
+            else:
+                bound_logger_method()
 
-        rv = LogfmtRenderer()(None, None, event_dict)
-        assert 'foo=bar a=14 baz="hello kitty" cool%story=bro f %^asdf' == rv
+            assert called_stdlib_method[0] is True
 
-    def test_equal_sign_or_space_in_value(self):
+    def test_exception_exc_info(self):
         """
-        Values with equal signs are always quoted.
+        BoundLogger.exception sets exc_info=True.
         """
-        event_dict = {
-            "without": "somevalue",
-            "withequal": "some=value",
-            "withspace": "some value",
-        }
+        bl = BoundLogger(ReturnLogger(), [], {})
 
-        rv = LogfmtRenderer()(None, None, event_dict)
-        assert (
-            r'without=somevalue withequal="some=value" withspace="some value"'
-            == rv
+        assert ((), {"exc_info": True, "event": "event"}) == bl.exception(
+            "event"
         )
 
-    def test_invalid_key(self):
+    def test_exception_exc_info_override(self):
         """
-        Keys cannot contain space characters.
+        If *exc_info* is password to exception, it's used.
         """
-        event_dict = {
-            "invalid key": "somevalue",
-        }
-
-        with pytest.raises(ValueError, match='Invalid key: "invalid key"'):
-            LogfmtRenderer()(None, None, event_dict)
+        bl = BoundLogger(ReturnLogger(), [], {})
 
+        assert ((), {"exc_info": 42, "event": "event"}) == bl.exception(
+            "event", exc_info=42
+        )
 
-class TestJSONRenderer:
-    def test_renders_json(self, event_dict):
+    def test_proxies_bind(self):
         """
-        Renders a predictable JSON string.
+        Bind calls the correct bind.
         """
-        rv = JSONRenderer(sort_keys=True)(None, None, event_dict)
+        bl = build_bl().bind(a=42)
 
-        assert (
-            r'{"a": "<A(\\o/)>", "b": [3, 4], "x": 7, '
-            r'"y": "test", "z": '
-            r"[1, 2]}"
-        ) == rv
+        assert {"a": 42} == get_context(bl)
 
-    def test_FallbackEncoder_handles_ThreadLocalDictWrapped_dicts(self):
+    def test_proxies_new(self):
         """
-        Our fallback handling handles properly ThreadLocalDictWrapper values.
+        Newcalls the correct new.
         """
-        with pytest.deprecated_call():
-            d = wrap_dict(dict)
-
-        s = json.dumps(d({"a": 42}), default=_json_fallback_handler)
+        bl = build_bl().bind(a=42).new(b=23)
 
-        assert '{"a": 42}' == s
+        assert {"b": 23} == get_context(bl)
 
-    def test_FallbackEncoder_falls_back(self):
+    def test_proxies_unbind(self):
         """
-        The fallback handler uses repr if it doesn't know the type.
+        Unbind calls the correct unbind.
         """
-        s = json.dumps(
-            {"date": datetime.date(1980, 3, 25)},
-            default=_json_fallback_handler,
-        )
+        bl = build_bl().bind(a=42).unbind("a")
 
-        assert '{"date": "datetime.date(1980, 3, 25)"}' == s
+        assert {} == get_context(bl)
 
-    def test_serializer(self):
+    def test_proxies_try_unbind(self):
         """
-        A custom serializer is used if specified.
+        try_unbind calls the correct try_unbind.
         """
-        jr = JSONRenderer(serializer=lambda obj, **kw: {"a": 42})
-        obj = object()
+        bl = build_bl().bind(a=42).try_unbind("a", "b")
 
-        assert {"a": 42} == jr(None, None, obj)
+        assert {} == get_context(bl)
 
-    def test_custom_fallback(self):
+    @pytest.mark.parametrize(
+        "meth", ["debug", "info", "warning", "error", "critical"]
+    )
+    async def test_async_log_methods(self, meth, cl):
         """
-        A custom fallback handler can be used.
+        Async methods log async.
         """
-        jr = JSONRenderer(default=lambda x: repr(x)[::-1])
-        d = {"date": datetime.date(1980, 3, 25)}
+        bl = build_bl(cl, processors=[])
+
+        await getattr(bl, f"a{meth}")("Async!")
 
-        assert '{"date": ")52 ,3 ,0891(etad.emitetad"}' == jr(None, None, d)
+        assert [
+            CapturedCall(method_name=meth, args=(), kwargs={"event": "Async!"})
+        ] == cl.calls
 
-    @pytest.mark.skipif(simplejson is None, reason="simplejson is missing.")
-    def test_simplejson(self, event_dict):
+    async def test_alog(self, cl):
         """
-        Integration test with simplejson.
+        Alog logs async at the correct level.
         """
-        jr = JSONRenderer(serializer=simplejson.dumps)
+        bl = build_bl(cl, processors=[])
 
-        assert {
-            "a": "<A(\\o/)>",
-            "b": [3, 4],
-            "x": 7,
-            "y": "test",
-            "z": [1, 2],
-        } == json.loads(jr(None, None, event_dict))
+        await bl.alog(logging.INFO, "foo %s", "bar")
 
+        assert [
+            CapturedCall(
+                method_name="info",
+                args=(),
+                kwargs={"positional_args": ("bar",), "event": "foo %s"},
+            )
+        ] == cl.calls
 
-class TestTimeStamper:
-    def test_disallows_non_utc_unix_timestamps(self):
+    async def test_aexception_exc_info_true(self, cl):
         """
-        A asking for a UNIX timestamp with a timezone that's not UTC raises a
-        ValueError.
+        aexception passes current exc_info into dispatch.
         """
-        with pytest.raises(
-            ValueError, match="UNIX timestamps are always UTC."
-        ):
-            TimeStamper(utc=False)
+        bl = build_bl(cl, processors=[])
+
+        try:
+            raise ValueError(42)
+        except ValueError as e:
+            await bl.aexception("oops")
+            exc = e
+
+        (cc,) = cl.calls
 
-    def test_inserts_utc_unix_timestamp_by_default(self):
+        assert isinstance(cc[2]["exc_info"], tuple)
+        assert exc == cc[2]["exc_info"][1]
+
+    async def test_aexception_exc_info_explicit(self, cl):
         """
-        Per default a float UNIX timestamp is used.
+        In aexception, if exc_info isn't missing or True, leave it be.
         """
-        ts = TimeStamper()
-        d = ts(None, None, {})
+        bl = build_bl(cl, processors=[])
+
+        obj = object()
+
+        await bl.aexception("ooops", exc_info=obj)
+
+        assert obj is cl.calls[0].kwargs["exc_info"]
 
-        # freezegun doesn't work with time.time. :(
-        assert isinstance(d["timestamp"], float)
 
-    @freeze_time("1980-03-25 16:00:00")
-    def test_local(self):
+class TestPositionalArgumentsFormatter:
+    def test_formats_tuple(self):
         """
-        Timestamp in local timezone work.  We can't add a timezone to the
-        string without additional libraries.
+        Positional arguments as simple types are rendered.
         """
-        ts = TimeStamper(fmt="iso", utc=False)
-        d = ts(None, None, {})
+        formatter = PositionalArgumentsFormatter()
+        event_dict = formatter(
+            None,
+            None,
+            {"event": "%d %d %s", "positional_args": (1, 2, "test")},
+        )
 
-        assert "1980-03-25T16:00:00" == d["timestamp"]
+        assert "1 2 test" == event_dict["event"]
+        assert "positional_args" not in event_dict
 
-    @freeze_time("1980-03-25 16:00:00")
-    def test_formats(self):
+    def test_formats_dict(self):
         """
-        The fmt string is respected.
+        Positional arguments as dict are rendered.
         """
-        ts = TimeStamper(fmt="%Y")
-        d = ts(None, None, {})
+        formatter = PositionalArgumentsFormatter()
+        event_dict = formatter(
+            None,
+            None,
+            {"event": "%(foo)s bar", "positional_args": ({"foo": "bar"},)},
+        )
 
-        assert "1980" == d["timestamp"]
+        assert "bar bar" == event_dict["event"]
+        assert "positional_args" not in event_dict
 
-    @freeze_time("1980-03-25 16:00:00")
-    def test_adds_Z_to_iso(self):
+    def test_positional_args_retained(self):
         """
-        stdlib's isoformat is buggy, so we fix it.
+        Positional arguments are retained if remove_positional_args
+        argument is set to False.
         """
-        ts = TimeStamper(fmt="iso", utc=True)
-        d = ts(None, None, {})
+        formatter = PositionalArgumentsFormatter(remove_positional_args=False)
+        positional_args = (1, 2, "test")
+        event_dict = formatter(
+            None,
+            None,
+            {"event": "%d %d %s", "positional_args": positional_args},
+        )
 
-        assert "1980-03-25T16:00:00Z" == d["timestamp"]
+        assert "positional_args" in event_dict
+        assert positional_args == event_dict["positional_args"]
 
-    @freeze_time("1980-03-25 16:00:00")
-    def test_key_can_be_specified(self):
+    def test_nop_no_args(self):
         """
-        Timestamp is stored with the specified key.
+        If no positional args are passed, nothing happens.
         """
-        ts = TimeStamper(fmt="%m", key="month")
-        d = ts(None, None, {})
+        formatter = PositionalArgumentsFormatter()
 
-        assert "03" == d["month"]
+        assert {} == formatter(None, None, {})
 
-    @freeze_time("1980-03-25 16:00:00")
-    @pytest.mark.parametrize("fmt", [None, "%Y"])
-    @pytest.mark.parametrize("utc", [True, False])
-    @pytest.mark.parametrize("key", [None, "other-key"])
-    @pytest.mark.parametrize("proto", range(pickle.HIGHEST_PROTOCOL + 1))
-    def test_pickle(self, fmt, utc, key, proto):
+    def test_args_removed_if_empty(self):
         """
-        TimeStamper is serializable.
+        If remove_positional_args is True and positional_args is (), still
+        remove them.
+
+        Regression test for https://github.com/hynek/structlog/issues/82.
         """
-        # UNIX timestamps must be UTC.
-        if fmt is None and not utc:
-            pytest.skip()
+        formatter = PositionalArgumentsFormatter()
 
-        ts = TimeStamper()
+        assert {} == formatter(None, None, {"positional_args": ()})
 
-        assert ts(None, None, {}) == pickle.loads(pickle.dumps(ts, proto))(
-            None, None, {}
-        )
 
-    def test_apply_freezegun_after_instantiation(self):
+class TestAddLogLevelNumber:
+    @pytest.mark.parametrize(("level", "number"), NAME_TO_LEVEL.items())
+    def test_log_level_number_added(self, level, number):
         """
-        Freezing time after instantiation of TimeStamper works.
+        The log level number is added to the event dict.
         """
-        ts = TimeStamper(fmt="iso", utc=False)
-
-        with freeze_time("1980-03-25 16:00:00", tz_offset=1):
-            d = ts(None, None, {})
+        event_dict = add_log_level_number(None, level, {})
 
-            assert "1980-03-25T17:00:00" == d["timestamp"]
+        assert number == event_dict["level_number"]
 
 
-class TestMaybeTimeStamper:
-    def test_overwrite(self):
+class TestAddLogLevel:
+    def test_log_level_added(self):
         """
-        If there is a timestamp, leave it.
+        The log level is added to the event dict.
         """
-        mts = MaybeTimeStamper()
+        event_dict = add_log_level(None, "error", {})
 
-        assert {"timestamp": 42} == mts(None, None, {"timestamp": 42})
+        assert "error" == event_dict["level"]
 
-    def test_none(self):
+    @pytest.mark.parametrize(
+        ("alias", "normalized"), [("warn", "warning"), ("exception", "error")]
+    )
+    def test_log_level_alias_normalized(self, alias, normalized):
         """
-        If there is no timestamp, add one.
+        The normalized name of the log level is added to the event dict.
         """
-        mts = MaybeTimeStamper()
+        event_dict = add_log_level(None, alias, {})
+
+        assert normalized == event_dict["level"]
+
+
+@pytest.fixture(name="make_log_record")
+def _make_log_record():
+    """
+    A LogRecord factory.
+    """
+
+    def create_log_record(**kwargs):
+        defaults = {
+            "name": "sample-name",
+            "level": logging.INFO,
+            "pathname": None,
+            "lineno": None,
+            "msg": "sample-message",
+            "args": [],
+            "exc_info": None,
+        }
+        defaults.update(kwargs)
+        return logging.LogRecord(**defaults)
 
-        assert "timestamp" in mts(None, None, {})
+    return create_log_record
 
 
-class TestFormatExcInfo:
-    def test_custom_formatter(self):
+class TestAddLoggerName:
+    def test_logger_name_added(self):
         """
-        The exception formatter can be changed.
+        The logger name is added to the event dict.
         """
-        formatter = ExceptionRenderer(lambda _: "There is no exception!")
+        name = "sample-name"
+        logger = logging.getLogger(name)
+        event_dict = add_logger_name(logger, None, {})
 
-        try:
-            raise CustomError("test")
-        except CustomError as e:
-            exc = e
-
-        assert formatter(None, None, {"exc_info": exc}) == {
-            "exception": "There is no exception!"
-        }
+        assert name == event_dict["logger"]
 
-    @pytest.mark.parametrize("ei", [False, None, ""])
-    def test_nop(self, ei):
+    def test_logger_name_added_with_record(self, make_log_record):
         """
-        If exc_info is falsey, only remove the key.
+        The logger name is deduced from the LogRecord if provided.
         """
-        assert {} == ExceptionRenderer()(None, None, {"exc_info": ei})
+        name = "sample-name"
+        record = make_log_record(name=name)
+        event_dict = add_logger_name(None, None, {"_record": record})
+
+        assert name == event_dict["logger"]
+
+
+def extra_dict() -> dict[str, Any]:
+    """
+    A dict to be passed in the `extra` parameter of the `logging` module's log
+    methods.
+    """
+    return {
+        "this": "is",
+        "some": "extra values",
+        "x_int": 4,
+        "x_bool": True,
+    }
+
 
-    def test_nop_missing(self):
+@pytest.fixture(name="extra_dict")
+def extra_dict_fixture():
+    return extra_dict()
+
+
+class TestExtraAdder:
+    @pytest.mark.parametrize(
+        ("allow", "misses"),
+        [
+            (None, None),
+            ({}, None),
+            *[({key}, None) for key in extra_dict()],
+            ({"missing"}, {"missing"}),
+            ({"missing", "keys"}, {"missing"}),
+            ({"this", "x_int"}, None),
+        ],
+    )
+    def test_add_extra(
+        self,
+        make_log_record: Callable[[], logging.LogRecord],
+        extra_dict: dict[str, Any],
+        allow: Collection[str] | None,
+        misses: set[str] | None,
+    ):
         """
-        If event dict doesn't contain exc_info, do nothing.
+        Extra attributes of a LogRecord object are added to the event dict.
         """
-        assert {} == ExceptionRenderer()(None, None, {})
+        record: logging.LogRecord = make_log_record()
+        record.__dict__.update(extra_dict)
+        event_dict = {"_record": record, "ed_key": "ed_value"}
+        expected = self._copy_allowed(event_dict, extra_dict, allow)
+
+        if allow is None:
+            actual = ExtraAdder()(None, None, event_dict)
+            assert expected == actual
+        actual = ExtraAdder(allow)(None, None, event_dict)
+        assert expected == actual
+        if misses:
+            assert misses.isdisjoint(expected.keys())
 
-    def test_formats_tuple(self):
+    def test_no_record(self):
         """
-        If exc_info is a tuple, it is used.
+        If the event_dict has no LogRecord, do nothing.
         """
-        formatter = ExceptionRenderer(lambda exc_info: exc_info)
-        d = formatter(None, None, {"exc_info": (None, None, 42)})
+        actual = ExtraAdder()(None, None, {})
 
-        assert {"exception": (None, None, 42)} == d
+        assert {} == actual
 
-    def test_gets_exc_info_on_bool(self):
+    @pytest.mark.parametrize(
+        ("allow", "misses"),
+        [
+            (None, None),
+            ({}, None),
+            *[({key}, None) for key in extra_dict()],
+            ({"missing"}, {"missing"}),
+            ({"missing", "keys"}, {"missing"}),
+            ({"this", "x_int"}, None),
+        ],
+    )
+    def test_add_extra_e2e(
+        self,
+        extra_dict: dict[str, Any],
+        allow: Collection[str] | None,
+        misses: set[str] | None,
+    ):
         """
-        If exc_info is True, it is obtained using sys.exc_info().
+        Values passed in the `extra` parameter of the `logging` module's log
+        methods pass through to log output.
         """
-        # monkeypatching sys.exc_info makes currently pytest return 1 on
-        # success.
-        try:
-            raise ValueError("test")
-        except ValueError:
-            d = ExceptionRenderer()(None, None, {"exc_info": True})
+        logger = logging.Logger(sys._getframe().f_code.co_name)
+        string_io = StringIO()
+        handler = logging.StreamHandler(string_io)
+        formatter = ProcessorFormatter(
+            foreign_pre_chain=[ExtraAdder(allow)],
+            processors=[JSONRenderer()],
+        )
+        handler.setFormatter(formatter)
+        handler.setLevel(0)
+        logger.addHandler(handler)
+        logger.setLevel(0)
+        logging.warning("allow = %s", allow)
+
+        event_dict = {"event": "Some text"}
+        expected = self._copy_allowed(event_dict, extra_dict, allow)
+
+        logger.info("Some %s", "text", extra=extra_dict)
+        actual = {
+            key: value
+            for key, value in json.loads(string_io.getvalue()).items()
+            if not key.startswith("_")
+        }
+
+        assert expected == actual
+        if misses:
+            assert misses.isdisjoint(expected.keys())
+
+    @classmethod
+    def _copy_allowed(
+        cls,
+        event_dict: EventDict,
+        extra_dict: dict[str, Any],
+        allow: Collection[str] | None,
+    ) -> EventDict:
+        if allow is None:
+            return {**event_dict, **extra_dict}
+
+        return {
+            **event_dict,
+            **{
+                key: value for key, value in extra_dict.items() if key in allow
+            },
+        }
+
+
+@pytest.fixture(name="stdlib_logger")
+def _stdlib_logger():
+    logger = logging.getLogger("test_logger")
+    logger.setLevel(logging.DEBUG)
+
+    yield logger
 
-        assert "exc_info" not in d
-        assert 'raise ValueError("test")' in d["exception"]
-        assert "ValueError: test" in d["exception"]
+    logging.basicConfig()
 
-    def test_exception(self):
+
+class TestRenderToLogKW:
+    def test_default(self, stdlib_logger):
         """
-        Passing exceptions as exc_info is valid.
+        Translates `event` to `msg` and handles otherwise empty `event_dict`s.
         """
-        formatter = ExceptionRenderer(lambda exc_info: exc_info)
+        d = render_to_log_kwargs(None, None, {"event": "message"})
 
-        try:
-            raise ValueError("test")
-        except ValueError as e:
-            exc = e
-        else:
-            pytest.fail("Exception not raised.")
+        assert {"msg": "message", "extra": {}} == d
 
-        assert {
-            "exception": (ValueError, exc, exc.__traceback__)
-        } == formatter(None, None, {"exc_info": exc})
+        # now check stdlib logger likes those kwargs
+        with patch.object(stdlib_logger, "_log") as mock_log:
+            stdlib_logger.info(**d)
+
+        mock_log.assert_called_once_with(logging.INFO, "message", (), extra={})
 
-    def test_exception_without_traceback(self):
+    def test_add_extra_event_dict(self, event_dict, stdlib_logger):
         """
-        If an Exception is missing a traceback, render it anyway.
+        Adds all remaining data from `event_dict` into `extra`.
         """
-        rv = ExceptionRenderer()(
-            None, None, {"exc_info": Exception("no traceback!")}
-        )
+        event_dict["event"] = "message"
+        d = render_to_log_kwargs(None, None, event_dict)
+
+        assert {"msg": "message", "extra": event_dict} == d
+
+        # now check stdlib logger likes those kwargs
+        with patch.object(stdlib_logger, "_log") as mock_log:
+            stdlib_logger.info(**d)
 
-        assert {"exception": "Exception: no traceback!"} == rv
+        mock_log.assert_called_once_with(
+            logging.INFO, "message", (), extra=event_dict
+        )
 
-    def test_format_exception(self):
+    def test_handles_special_kw(self, event_dict, stdlib_logger):
         """
-        "format_exception" is the "ExceptionRenderer" with default settings.
+        "exc_info", "stack_info", and "stacklevel" aren't passed as extras.
+
+        Cf. https://github.com/hynek/structlog/issues/424
         """
-        try:
-            raise ValueError("test")
-        except ValueError as e:
-            a = format_exc_info(None, None, {"exc_info": e})
-            b = ExceptionRenderer()(None, None, {"exc_info": e})
+        del event_dict["a"]  # needs a repr
+        event_dict["event"] = "message"
+
+        event_dict["exc_info"] = True
+        event_dict["stack_info"] = False
+        event_dict["stacklevel"] = 1
+        event_dict["stackLevel"] = 1  # not a reserved kw
+
+        d = render_to_log_kwargs(None, None, event_dict)
+        expected = {
+            "msg": "message",
+            "exc_info": True,
+            "stack_info": False,
+            "stacklevel": 1,
+            "extra": {
+                "b": [3, 4],
+                "x": 7,
+                "y": "test",
+                "z": (1, 2),
+                "stackLevel": 1,
+            },
+        }
+
+        assert expected == d
 
-        assert a == b
+        # now check stdlib logger likes those kwargs
+        with patch.object(stdlib_logger, "_log") as mock_log:
+            stdlib_logger.info(**d)
+
+        expected.pop("msg")
+        mock_log.assert_called_once_with(
+            logging.INFO, "message", (), **expected
+        )
 
-    @pytest.mark.parametrize("ei", [True, (None, None, None)])
-    def test_no_exception(self, ei):
+    def test_integration_special_kw(self, event_dict, stdlib_logger):
         """
-        A missing exception does not blow up.
+        render_to_log_kwargs with a wrapped logger calls the stdlib logger
+        correctly
+
+        reserved stdlib keywords are in logging.Logger._log
+        https://github.com/python/cpython/blob/ae7b17673f29efe17b416cbcfbf43b5b3ff5977c/Lib/logging/__init__.py#L1632
         """
-        assert {"exception": "MISSING"} == format_exc_info(
-            None, None, {"exc_info": ei}
+        expected = {
+            "msg": "message",
+            "exc_info": True,
+            "stack_info": False,
+            "stacklevel": 1,
+            "extra": {**event_dict},
+        }
+
+        event_dict["exc_info"] = True
+        event_dict["stack_info"] = False
+        event_dict["stacklevel"] = 1
+
+        struct_logger = wrap_logger(
+            stdlib_logger,
+            processors=[render_to_log_kwargs],
+        )
+
+        # now check struct logger passes those kwargs to stdlib
+        with patch.object(stdlib_logger, "_log") as mock_log:
+            struct_logger.info("message", **event_dict)
+
+        expected.pop("msg")
+        mock_log.assert_called_once_with(
+            logging.INFO, "message", (), **expected
         )
 
 
-class TestUnicodeEncoder:
-    def test_encodes(self):
+@pytest.fixture(name="configure_for_processor_formatter")
+def _configure_for_processor_formatter():
+    """
+    Configure structlog to use ProcessorFormatter.
+
+    Reset logging setting after the test (structlog is reset automatically
+    before all tests).
+    """
+    configure(
+        processors=[add_log_level, ProcessorFormatter.wrap_for_formatter],
+        logger_factory=LoggerFactory(),
+        wrapper_class=BoundLogger,
+    )
+
+    yield
+
+    logging.basicConfig()
+
+
+def configure_logging(
+    pre_chain,
+    logger=None,
+    pass_foreign_args=False,
+    renderer=ConsoleRenderer(colors=False),  # noqa: B008
+):
+    """
+    Configure logging to use ProcessorFormatter.
+
+    Return a list that is filled with event dicts form calls.
+    """
+    event_dicts = []
+
+    def capture(_, __, ed):
+        event_dicts.append(ed.copy())
+
+        return ed
+
+    logging.config.dictConfig(
+        {
+            "version": 1,
+            "disable_existing_loggers": False,
+            "formatters": {
+                "plain": {
+                    "()": ProcessorFormatter,
+                    "processors": [
+                        capture,
+                        ProcessorFormatter.remove_processors_meta,
+                        renderer,
+                    ],
+                    "foreign_pre_chain": pre_chain,
+                    "format": "%(message)s [in %(funcName)s]",
+                    "logger": logger,
+                    "pass_foreign_args": pass_foreign_args,
+                }
+            },
+            "handlers": {
+                "default": {
+                    "level": "DEBUG",
+                    "class": "logging.StreamHandler",
+                    "formatter": "plain",
+                }
+            },
+            "loggers": {
+                "": {
+                    "handlers": ["default"],
+                    "level": "DEBUG",
+                    "propagate": True,
+                }
+            },
+        }
+    )
+
+    return event_dicts
+
+
+@pytest.mark.usefixtures("configure_for_processor_formatter")
+class TestProcessorFormatter:
+    """
+    These are all integration tests because they're all about integration.
+    """
+
+    def test_foreign_delegate(self, capsys):
         """
-        Unicode strings get encoded (as UTF-8 by default).
+        If foreign_pre_chain is None, non-structlog log entries are delegated
+        to logging. The processor chain's event dict is invoked with
+        `_from_structlog=False`
         """
-        e = UnicodeEncoder()
+        calls = configure_logging(None)
+
+        logging.getLogger().warning("foo")
 
-        assert {"foo": b"b\xc3\xa4r"} == e(None, None, {"foo": "b\xe4r"})
+        assert ("", "foo [in test_foreign_delegate]\n") == capsys.readouterr()
+        assert calls[0]["_from_structlog"] is False
+        assert isinstance(calls[0]["_record"], logging.LogRecord)
 
-    def test_passes_arguments(self):
+    def test_clears_args(self, capsys):
         """
-        Encoding options are passed into the encoding call.
+        We render our log records before sending it back to logging.  Therefore
+        we must clear `LogRecord.args` otherwise the user gets an
+        `TypeError: not all arguments converted during string formatting.` if
+        they use positional formatting in stdlib logging.
         """
-        e = UnicodeEncoder("latin1", "xmlcharrefreplace")
+        configure_logging(None)
 
-        assert {"foo": b"&#8211;"} == e(None, None, {"foo": "\u2013"})
+        logging.getLogger().warning("hello %s.", "world")
 
-    def test_bytes_nop(self):
+        assert (
+            "",
+            "hello world. [in test_clears_args]\n",
+        ) == capsys.readouterr()
+
+    def test_pass_foreign_args_true_sets_positional_args_key(self):
         """
-        If the string is already bytes, don't do anything.
+        If `pass_foreign_args` is `True` we set the `positional_args` key in
+        the `event_dict` before clearing args.
         """
-        e = UnicodeEncoder()
+        test_processor = call_recorder(lambda _, __, event_dict: event_dict)
+        configure_logging((test_processor,), pass_foreign_args=True)
+
+        positional_args = {"foo": "bar"}
+        logging.getLogger().info("okay %(foo)s", positional_args)
 
-        assert {"foo": b"b\xc3\xa4r"} == e(None, None, {"foo": b"b\xc3\xa4r"})
+        event_dict = test_processor.calls[0].args[2]
 
+        assert "positional_args" in event_dict
+        assert positional_args == event_dict["positional_args"]
 
-class TestUnicodeDecoder:
-    def test_decodes(self):
+    def test_log_dict(self, capsys):
         """
-        Byte strings get decoded (as UTF-8 by default).
+        dicts can be logged with std library loggers.
         """
-        ud = UnicodeDecoder()
+        configure_logging(None)
 
-        assert {"foo": "b\xe4r"} == ud(None, None, {"foo": b"b\xc3\xa4r"})
+        logging.getLogger().warning({"foo": "bar"})
+
+        assert (
+            "",
+            "{'foo': 'bar'} [in test_log_dict]\n",
+        ) == capsys.readouterr()
 
-    def test_passes_arguments(self):
+    def test_foreign_pre_chain(self, capsys):
         """
-        Encoding options are passed into the encoding call.
+        If foreign_pre_chain is an iterable, it's used to pre-process
+        non-structlog log entries.
         """
-        ud = UnicodeDecoder("utf-8", "ignore")
+        configure_logging([add_log_level])
 
-        assert {"foo": ""} == ud(None, None, {"foo": b"\xa1\xa4"})
+        logging.getLogger().warning("foo")
 
-    def test_bytes_nop(self):
+        assert (
+            "",
+            "[warning  ] foo [in test_foreign_pre_chain]\n",
+        ) == capsys.readouterr()
+
+    def test_foreign_pre_chain_add_logger_name(self, capsys):
         """
-        If the value is already unicode, don't do anything.
+        foreign_pre_chain works with add_logger_name processor.
         """
-        ud = UnicodeDecoder()
+        configure_logging((add_logger_name,))
 
-        assert {"foo": "b\u2013r"} == ud(None, None, {"foo": "b\u2013r"})
+        logging.getLogger("sample-name").warning("foo")
 
+        assert (
+            "",
+            "foo                            [sample-name] [in test_foreign_pr"
+            "e_chain_add_logger_name]\n",
+        ) == capsys.readouterr()
 
-class TestExceptionPrettyPrinter:
-    def test_stdout_by_default(self):
+    def test_foreign_chain_can_pass_dictionaries_without_excepting(
+        self, capsys
+    ):
         """
-        If no file is supplied, use stdout.
+        If a foreign logger passes a dictionary to a logging function,
+        check we correctly identify that it did not come from structlog.
         """
-        epp = ExceptionPrettyPrinter()
+        configure_logging(None)
+        configure(
+            processors=[ProcessorFormatter.wrap_for_formatter],
+            logger_factory=LoggerFactory(),
+            wrapper_class=BoundLogger,
+        )
 
-        assert sys.stdout is epp._file
+        logging.getLogger().warning({"foo": "bar"})
 
-    def test_prints_exception(self, sio):
+        assert (
+            "",
+            "{'foo': 'bar'} [in "
+            "test_foreign_chain_can_pass_dictionaries_without_excepting]\n",
+        ) == capsys.readouterr()
+
+    def test_foreign_pre_chain_gets_exc_info(self):
         """
-        If there's an `exception` key in the event_dict, just print it out.
-        This happens if `format_exc_info` was run before us in the chain.
+        If non-structlog record contains exc_info, foreign_pre_chain functions
+        have access to it.
         """
-        epp = ExceptionPrettyPrinter(file=sio)
+        test_processor = call_recorder(lambda _, __, event_dict: event_dict)
+        configure_logging((test_processor,), renderer=KeyValueRenderer())
+
         try:
-            raise ValueError
-        except ValueError:
-            ed = format_exc_info(None, None, {"exc_info": True})
-        epp(None, None, ed)
+            raise RuntimeError("oh no")
+        except Exception:
+            logging.getLogger().exception("okay")
 
-        out = sio.getvalue()
+        event_dict = test_processor.calls[0].args[2]
 
-        assert "test_prints_exception" in out
-        assert "raise ValueError" in out
+        assert "exc_info" in event_dict
+        assert isinstance(event_dict["exc_info"], tuple)
 
-    def test_removes_exception_after_printing(self, sio):
+    def test_foreign_pre_chain_sys_exc_info(self):
         """
-        After pretty printing `exception` is removed from the event_dict.
+        If a foreign_pre_chain function accesses sys.exc_info(),
+        ProcessorFormatter should not have changed it.
         """
-        epp = ExceptionPrettyPrinter(sio)
-        try:
-            raise ValueError
-        except ValueError:
-            ed = format_exc_info(None, None, {"exc_info": True})
 
-        assert "exception" in ed
+        class MyError(Exception):
+            pass
 
-        new_ed = epp(None, None, ed)
+        def add_excinfo(logger, log_method, event_dict):
+            event_dict["exc_info"] = sys.exc_info()
+            return event_dict
 
-        assert "exception" not in new_ed
+        test_processor = call_recorder(lambda _, __, event_dict: event_dict)
+        configure_logging(
+            (add_excinfo, test_processor), renderer=KeyValueRenderer()
+        )
 
-    def test_handles_exc_info(self, sio):
-        """
-        If `exc_info` is passed in, it behaves like `format_exc_info`.
-        """
-        epp = ExceptionPrettyPrinter(sio)
         try:
-            raise ValueError
-        except ValueError:
-            epp(None, None, {"exc_info": True})
+            raise MyError("oh no")
+        except Exception:
+            logging.getLogger().error("okay")
 
-        out = sio.getvalue()
+        event_dict = test_processor.calls[0].args[2]
 
-        assert "test_handles_exc_info" in out
-        assert "raise ValueError" in out
+        assert MyError is event_dict["exc_info"][0]
 
-    def test_removes_exc_info_after_printing(self, sio):
+    def test_other_handlers_get_original_record(self):
         """
-        After pretty printing `exception` is removed from the event_dict.
+        Logging handlers that come after the handler with ProcessorFormatter
+        should receive original, unmodified record.
         """
-        epp = ExceptionPrettyPrinter(sio)
-        try:
-            raise ValueError
-        except ValueError:
-            ed = epp(None, None, {"exc_info": True})
+        configure_logging(None)
+
+        handler1 = logging.StreamHandler()
+        handler1.setFormatter(ProcessorFormatter(JSONRenderer()))
+        handler2 = stub(
+            handle=call_recorder(lambda record: None),
+            level=logging.INFO,
+        )
+        logger = logging.getLogger()
+        logger.addHandler(handler1)
+        logger.addHandler(handler2)
 
-        assert "exc_info" not in ed
+        logger.info("meh")
 
-    def test_nop_if_no_exception(self, sio):
-        """
-        If there is no exception, don't print anything.
-        """
-        epp = ExceptionPrettyPrinter(sio)
-        epp(None, None, {})
+        assert 1 == len(handler2.handle.calls)
 
-        assert "" == sio.getvalue()
+        handler2_record = handler2.handle.calls[0].args[0]
 
-    def test_own_exc_info(self, sio):
+        assert "meh" == handler2_record.msg
+
+    @pytest.mark.parametrize("keep", [True, False])
+    def test_formatter_unsets_exc_info(self, capsys, keep):
         """
-        If exc_info is a tuple, use it.
+        Stack traces doesn't get printed outside of the json document when
+        keep_exc_info are set to False but preserved if set to True.
         """
-        epp = ExceptionPrettyPrinter(sio)
+        configure_logging(None)
+        logger = logging.getLogger()
+
+        def format_exc_info_fake(logger, name, event_dict):
+            del event_dict["exc_info"]
+            event_dict["exception"] = "Exception!"
+            return event_dict
+
+        formatter = ProcessorFormatter(
+            processor=JSONRenderer(),
+            keep_stack_info=keep,
+            keep_exc_info=keep,
+            foreign_pre_chain=[format_exc_info_fake],
+        )
+        logger.handlers[0].setFormatter(formatter)
+
         try:
-            raise ValueError("XXX")
-        except ValueError:
-            ei = sys.exc_info()
+            raise RuntimeError("oh no")
+        except Exception:
+            logging.getLogger().exception("seen worse")
 
-        epp(None, None, {"exc_info": ei})
+        out, err = capsys.readouterr()
 
-        assert "XXX" in sio.getvalue()
+        assert "" == out
 
-    def test_exception_on_py3(self, sio):
+        if keep is False:
+            assert (
+                '{"event": "seen worse", "exception": "Exception!"}\n'
+            ) == err
+        else:
+            assert "Traceback (most recent call last):" in err
+
+    @pytest.mark.parametrize("keep", [True, False])
+    def test_formatter_unsets_stack_info(self, capsys, keep):
         """
-        On Python 3, it's also legal to pass an Exception.
+        Stack traces doesn't get printed outside of the json document when
+        keep_stack_info are set to False but preserved if set to True.
         """
-        epp = ExceptionPrettyPrinter(sio)
-        try:
-            raise ValueError("XXX")
-        except ValueError as e:
-            epp(None, None, {"exc_info": e})
+        configure_logging(None)
+        logger = logging.getLogger()
+
+        formatter = ProcessorFormatter(
+            processor=JSONRenderer(),
+            keep_stack_info=keep,
+            keep_exc_info=keep,
+            foreign_pre_chain=[],
+        )
+        logger.handlers[0].setFormatter(formatter)
 
-        assert "XXX" in sio.getvalue()
+        logging.getLogger().warning("have a stack trace", stack_info=True)
 
+        out, err = capsys.readouterr()
 
-@pytest.fixture()
-def sir():
-    return StackInfoRenderer()
+        assert "" == out
 
+        if keep is False:
+            assert 1 == err.count("Stack (most recent call last):")
+        else:
+            assert 2 == err.count("Stack (most recent call last):")
 
-class TestStackInfoRenderer:
-    def test_removes_stack_info(self, sir):
+    def test_native(self, capsys):
         """
-        The `stack_info` key is removed from `event_dict`.
+        If the log entry comes from structlog, it's unpackaged and processed.
         """
-        ed = sir(None, None, {"stack_info": True})
+        eds = configure_logging(None)
+
+        get_logger().warning("foo")
 
-        assert "stack_info" not in ed
+        assert (
+            "",
+            "[warning  ] foo [in test_native]\n",
+        ) == capsys.readouterr()
+        assert eds[0]["_from_structlog"] is True
+        assert isinstance(eds[0]["_record"], logging.LogRecord)
 
-    def test_adds_stack_if_asked(self, sir):
+    def test_native_logger(self, capsys):
         """
-        If `stack_info` is true, `stack` is added.
+        If the log entry comes from structlog, it's unpackaged and processed.
         """
-        ed = sir(None, None, {"stack_info": True})
+        logger = logging.getLogger()
+        eds = configure_logging(None, logger=logger)
+
+        get_logger().warning("foo")
+
+        assert (
+            "",
+            "[warning  ] foo [in test_native_logger]\n",
+        ) == capsys.readouterr()
+        assert eds[0]["_from_structlog"] is True
+        assert isinstance(eds[0]["_record"], logging.LogRecord)
+
+    def test_foreign_pre_chain_filter_by_level(self, capsys):
+        """
+        foreign_pre_chain works with filter_by_level processor.
+        """
+        logger = logging.getLogger()
+        configure_logging([filter_by_level], logger=logger)
+        configure(
+            processors=[ProcessorFormatter.wrap_for_formatter],
+            logger_factory=LoggerFactory(),
+            wrapper_class=BoundLogger,
+        )
 
-        assert "stack" in ed
+        logger.warning("foo")
 
-    def test_renders_correct_stack(self, sir):
+        assert (
+            "",
+            "foo [in test_foreign_pre_chain_filter_by_level]\n",
+        ) == capsys.readouterr()
+
+    def test_processor_and_processors(self):
         """
-        The rendered stack is correct.
+        Passing both processor and processors raises a TypeError.
         """
-        ed = sir(None, None, {"stack_info": True})
-
-        assert 'ed = sir(None, None, {"stack_info": True})' in ed["stack"]
+        with pytest.raises(TypeError, match="mutually exclusive"):
+            ProcessorFormatter(processor=1, processors=[1])
 
-    def test_additional_ignores(self):
+    def test_no_renderer(self):
         """
-        Filtering of names works.
+        Passing neither processor nor processors raises a TypeError.
         """
-        sir = StackInfoRenderer(["tests.additional_frame"])
+        with pytest.raises(TypeError, match="must be passed"):
+            ProcessorFormatter()
 
-        ed = additional_frame(
-            functools.partial(sir, None, None, {"stack_info": True})
+    def test_remove_processors_meta(self):
+        """
+        remove_processors_meta removes _record and _from_structlog. And only
+        them.
+        """
+        assert {"foo": "bar"} == ProcessorFormatter.remove_processors_meta(
+            None,
+            None,
+            {"foo": "bar", "_record": "foo", "_from_structlog": True},
         )
 
-        assert "additional_frame.py" not in ed["stack"]
+    def test_non_string_message_warning(self):
+        """
+        A warning is raised if the last processor in
+        ProcessorFormatter.processors doesn't return a string.
+        """
+        configure_logging(None)
+        logger = logging.getLogger()
+
+        formatter = ProcessorFormatter(
+            processors=[lambda *args, **kwargs: {"foo": "bar"}],
+        )
+        logger.handlers[0].setFormatter(formatter)
 
+        with pytest.warns(
+            RuntimeWarning,
+            match="The last processor in ProcessorFormatter.processors must return a string",
+        ):
+            logger.info("baz")
 
-class TestFigureOutExcInfo:
-    @pytest.mark.parametrize("true_value", [True, 1, 1.1])
-    def test_obtains_exc_info_on_True(self, true_value):
+    def test_logrecord_exc_info(self):
         """
-        If the passed argument evaluates to True obtain exc_info ourselves.
+        LogRecord.exc_info is set consistently for structlog and non-structlog
+        log records.
         """
+        configure_logging(None)
+
+        # This doesn't test ProcessorFormatter itself directly, but it's
+        # relevant to setups where ProcessorFormatter is used, i.e. where
+        # handlers will receive LogRecord objects that come from both structlog
+        # and non-structlog loggers.
+
+        records: Dict[  # noqa: UP006 - dict isn't generic until Python 3.9
+            str, logging.LogRecord
+        ] = {}
+
+        class DummyHandler(logging.Handler):
+            def emit(self, record):
+                # Don't do anything; just store the record in the records dict
+                # by its message, so we can assert things about it.
+                if isinstance(record.msg, dict):
+                    records[record.msg["event"]] = record
+                else:
+                    records[record.msg] = record
+
+        stdlib_logger = logging.getLogger()
+        structlog_logger = get_logger()
+
+        # It doesn't matter which logger we add the handler to here.
+        stdlib_logger.addHandler(DummyHandler())
+
         try:
-            0 / 0
+            raise Exception("foo")
         except Exception:
-            assert sys.exc_info() == _figure_out_exc_info(true_value)
-        else:
-            pytest.fail("Exception not raised.")
+            stdlib_logger.exception("bar")
+            structlog_logger.exception("baz")
 
-    def test_py3_exception_no_traceback(self):
-        """
-        Exceptions without tracebacks are simply returned with None for
-        traceback.
-        """
-        e = ValueError()
+        stdlib_record = records.pop("bar")
 
-        assert (e.__class__, e, None) == _figure_out_exc_info(e)
+        assert "bar" == stdlib_record.msg
+        assert stdlib_record.exc_info
+        assert Exception is stdlib_record.exc_info[0]
+        assert ("foo",) == stdlib_record.exc_info[1].args
 
+        structlog_record = records.pop("baz")
 
-class TestCallsiteParameterAdder:
-    parameter_strings = {
-        "pathname",
-        "filename",
-        "module",
-        "func_name",
-        "lineno",
-        "thread",
-        "thread_name",
-        "process",
-        "process_name",
-    }
+        assert "baz" == structlog_record.msg["event"]
+        assert True is structlog_record.msg["exc_info"]
+        assert structlog_record.exc_info
+        assert Exception is structlog_record.exc_info[0]
+        assert ("foo",) == structlog_record.exc_info[1].args
 
-    _all_parameters = set(CallsiteParameter)
+        assert not records
 
-    def test_all_parameters(self) -> None:
+    def test_use_get_message_false(self):
         """
-        All callsite parameters are included in ``self.parameter_strings`` and
-        the dictionary returned by ``self.get_callsite_parameters`` contains
-        keys for all callsite parameters.
+        If use_get_message_is False, the event is obtained using
+        str(record.msg) instead of calling record.getMessage. That means
+        positional formatting is not performed.
         """
+        event_dicts = []
 
-        assert self.parameter_strings == {
-            member.value for member in self._all_parameters
-        }
-        assert self.parameter_strings == self.get_callsite_parameters().keys()
+        def capture(_, __, ed):
+            event_dicts.append(ed.copy())
 
-    @pytest.mark.asyncio()
-    async def test_async(self) -> None:
-        """
-        Callsite information for async invocations are correct.
-        """
-        string_io = StringIO()
+            return str(ed)
 
-        class StingIOLogger(structlog.PrintLogger):
-            def __init__(self):
-                super().__init__(file=string_io)
-
-        processor = self.make_processor(None, ["concurrent", "threading"])
-        structlog.configure(
-            processors=[processor, JSONRenderer()],
-            logger_factory=StingIOLogger,
-            wrapper_class=structlog.stdlib.AsyncBoundLogger,
-            cache_logger_on_first_use=True,
+        proc = ProcessorFormatter(processors=[capture], use_get_message=False)
+
+        record = logging.LogRecord(
+            "foo",
+            logging.INFO,
+            "path.py",
+            42,
+            "le msg: %s",
+            ("keep separate",),
+            None,
         )
 
-        logger = structlog.stdlib.get_logger()
+        assert proc.format(record)
+        assert "le msg: %s" == event_dicts[0]["event"]
+
 
-        callsite_params = self.get_callsite_parameters()
-        await logger.info("baz")
-        logger_params = json.loads(string_io.getvalue())
+@pytest_asyncio.fixture(name="abl")
+async def _abl(cl):
+    return AsyncBoundLogger(cl, context={}, processors=[])
 
-        # These are different when running under async
-        for key in ["thread", "thread_name"]:
-            callsite_params.pop(key)
-            logger_params.pop(key)
 
-        assert {"event": "baz", **callsite_params} == logger_params
+class TestAsyncBoundLogger:
+    def test_sync_bl(self, abl, cl):
+        """
+        AsyncBoungLogger.sync_bl works outside of loops.
+        """
+        abl.sync_bl.info("test")
+
+        assert [
+            CapturedCall(method_name="info", args=(), kwargs={"event": "test"})
+        ] == cl.calls
 
-    def test_additional_ignores(self, monkeypatch: pytest.MonkeyPatch) -> None:
+    @pytest.mark.asyncio()
+    async def test_protocol(self, abl):
         """
-        Stack frames from modules with names that start with values in
-        `additional_ignores` are ignored when determining the callsite.
+        AsyncBoundLogger is a proper BindableLogger.
         """
-        test_message = "test message"
-        additional_ignores = ["tests.additional_frame"]
-        processor = self.make_processor(None, additional_ignores)
-        event_dict: EventDict = {"event": test_message}
+        assert isinstance(abl, BindableLogger)
 
-        # Warning: the next two lines must appear exactly like this to make
-        # line numbers match.
-        callsite_params = self.get_callsite_parameters(1)
-        actual = processor(None, None, event_dict)
+    @pytest.mark.asyncio()
+    async def test_correct_levels(self, abl, cl, stdlib_log_method):
+        """
+        The proxy methods call the correct upstream methods.
+        """
+        await getattr(abl.bind(foo="bar"), stdlib_log_method)("42")
 
-        expected = {"event": test_message, **callsite_params}
+        aliases = {"warn": "warning"}
 
-        assert expected == actual
+        alias = aliases.get(stdlib_log_method)
+        expect = alias if alias else stdlib_log_method
 
-    @pytest.mark.parametrize(
-        ("origin", "parameter_strings"),
-        itertools.product(
-            ["logging", "structlog"],
-            [
-                None,
-                *[{parameter} for parameter in parameter_strings],
-                set(),
-                parameter_strings,
-                {"pathname", "filename"},
-                {"module", "func_name"},
-            ],
-        ),
-    )
-    def test_processor(
-        self,
-        origin: str,
-        parameter_strings: set[str] | None,
-    ):
+        assert expect == cl.calls[0].method_name
+
+    @pytest.mark.asyncio()
+    async def test_log_method(self, abl, cl):
         """
-        The correct callsite parameters are added to event dictionaries.
+        The `log` method is proxied too.
         """
-        test_message = "test message"
-        processor = self.make_processor(parameter_strings)
-        if origin == "structlog":
-            event_dict: EventDict = {"event": test_message}
-            callsite_params = self.get_callsite_parameters()
-            actual = processor(None, None, event_dict)
-        elif origin == "logging":
-            callsite_params = self.get_callsite_parameters()
-            record = logging.LogRecord(
-                "name",
-                logging.INFO,
-                callsite_params["pathname"],
-                callsite_params["lineno"],
-                test_message,
-                None,
-                None,
-                callsite_params["func_name"],
-            )
-            event_dict: EventDict = {
-                "event": test_message,
-                "_record": record,
-                "_from_structlog": False,
-            }
-            actual = processor(None, None, event_dict)
-        else:
-            pytest.fail(f"invalid origin {origin}")
-        actual = {
-            key: value
-            for key, value in actual.items()
-            if not key.startswith("_")
-        }
-        callsite_params = self.filter_parameter_dict(
-            callsite_params, parameter_strings
-        )
-        expected = {"event": test_message, **callsite_params}
+        await abl.bind(foo="bar").log(logging.ERROR, "42")
 
-        assert expected == actual
+        assert "error" == cl.calls[0].method_name
 
-    @pytest.mark.parametrize(
-        ("setup", "origin", "parameter_strings"),
-        itertools.product(
-            ["common-without-pre", "common-with-pre", "shared", "everywhere"],
-            ["logging", "structlog"],
-            [
-                None,
-                *[{parameter} for parameter in parameter_strings],
-                set(),
-                parameter_strings,
-                {"pathname", "filename"},
-                {"module", "func_name"},
-            ],
-        ),
-    )
-    def test_e2e(
-        self,
-        setup: str,
-        origin: str,
-        parameter_strings: set[str] | None,
-    ) -> None:
+    @pytest.mark.asyncio()
+    async def test_exception(self, abl, cl):
         """
-        Logging output contains the correct callsite parameters.
+        `exception` makes sure 'exc_info" is set, if it's not set already.
         """
-        logger = logging.Logger(sys._getframe().f_code.co_name)
-        string_io = StringIO()
-        handler = logging.StreamHandler(string_io)
-        processors = [self.make_processor(parameter_strings)]
-        if setup == "common-without-pre":
-            common_processors = processors
-            formatter = ProcessorFormatter(
-                processors=[*processors, JSONRenderer()]
-            )
-        elif setup == "common-with-pre":
-            common_processors = processors
-            formatter = ProcessorFormatter(
-                foreign_pre_chain=processors,
-                processors=[JSONRenderer()],
-            )
-        elif setup == "shared":
-            common_processors = []
-            formatter = ProcessorFormatter(
-                processors=[*processors, JSONRenderer()],
-            )
-        elif setup == "everywhere":
-            common_processors = processors
-            formatter = ProcessorFormatter(
-                foreign_pre_chain=processors,
-                processors=[*processors, JSONRenderer()],
-            )
-        else:
-            pytest.fail(f"invalid setup {setup}")
-        handler.setFormatter(formatter)
-        handler.setLevel(0)
-        logger.addHandler(handler)
-        logger.setLevel(0)
+        try:
+            raise ValueError("omg")
+        except ValueError:
+            await abl.exception("oops")
 
-        test_message = "test message"
-        if origin == "logging":
-            callsite_params = self.get_callsite_parameters()
-            logger.info(test_message)
-        elif origin == "structlog":
-            ctx = {}
-            bound_logger = BoundLogger(
-                logger,
-                [*common_processors, ProcessorFormatter.wrap_for_formatter],
-                ctx,
-            )
-            callsite_params = self.get_callsite_parameters()
-            bound_logger.info(test_message)
-        else:
-            pytest.fail(f"invalid origin {origin}")
+        ei = cl.calls[0].kwargs["exc_info"]
 
-        callsite_params = self.filter_parameter_dict(
-            callsite_params, parameter_strings
-        )
-        actual = {
-            key: value
-            for key, value in json.loads(string_io.getvalue()).items()
-            if not key.startswith("_")
-        }
-        expected = {"event": test_message, **callsite_params}
+        assert ValueError is ei[0]
+        assert ("omg",) == ei[1].args
 
-        assert expected == actual
+    @pytest.mark.asyncio()
+    async def test_exception_do_not_overwrite(self, abl, cl):
+        """
+        `exception` leaves exc_info be, if it's set.
+        """
+        o1 = object()
+        o2 = object()
+        o3 = object()
 
-    @classmethod
-    def make_processor(
-        cls,
-        parameter_strings: set[str] | None,
-        additional_ignores: list[str] | None = None,
-    ) -> CallsiteParameterAdder:
-        """
-        Creates a ``CallsiteParameterAdder`` with parameters matching the
-        supplied *parameter_strings* values and with the supplied
-        *additional_ignores* values.
-
-        Args:
-            parameter_strings:
-                Strings for which corresponding ``CallsiteParameters`` should
-                be included in the resulting ``CallsiteParameterAdded``.
-
-            additional_ignores:
-                Used as *additional_ignores* for the resulting
-                ``CallsiteParameterAdded``.
-        """
-        if parameter_strings is None:
-            return CallsiteParameterAdder(
-                additional_ignores=additional_ignores
-            )
+        try:
+            raise ValueError("omg")
+        except ValueError:
+            await abl.exception("oops", exc_info=(o1, o2, o3))
 
-        parameters = cls.filter_parameters(parameter_strings)
-        return CallsiteParameterAdder(
-            parameters=parameters,
-            additional_ignores=additional_ignores,
-        )
+        ei = cl.calls[0].kwargs["exc_info"]
+        assert (o1, o2, o3) == ei
 
-    @classmethod
-    def filter_parameters(
-        cls, parameter_strings: set[str] | None
-    ) -> set[CallsiteParameter]:
-        """
-        Returns a set containing all ``CallsiteParameter`` members with values
-        that are in ``parameter_strings``.
-
-        Args:
-            parameter_strings:
-                The parameters strings for which corresponding
-                ``CallsiteParameter`` members should be returned. If this value
-                is `None` then all ``CallsiteParameter`` will be returned.
+    @pytest.mark.asyncio()
+    async def test_bind_unbind(self, cl):
         """
-        if parameter_strings is None:
-            return cls._all_parameters
-        return {
-            parameter
-            for parameter in cls._all_parameters
-            if parameter.value in parameter_strings
-        }
-
-    @classmethod
-    def filter_parameter_dict(
-        cls, input: dict[str, object], parameter_strings: set[str] | None
-    ) -> dict[str, object]:
-        """
-        Returns a dictionary that is equivalent to *input* but with all keys
-        not in *parameter_strings* removed.
-
-        Args:
-            parameter_strings:
-                The keys to keep in the dictionary, if this value is ``None``
-                then all keys matching ``cls.parameter_strings`` are kept.
+        new/bind/unbind/try_unbind are correctly propagated.
         """
-        if parameter_strings is None:
-            parameter_strings = cls.parameter_strings
-        return {
-            key: value
-            for key, value in input.items()
-            if key in parameter_strings
-        }
+        l1 = AsyncBoundLogger(cl, context={}, processors=[])
 
-    @classmethod
-    def get_callsite_parameters(cls, offset: int = 1) -> dict[str, object]:
-        """
-        This function creates dictionary of callsite parameters for the line
-        that is ``offset`` lines after the invocation of this function.
+        l2 = l1.bind(x=42)
 
-        Args:
-            offset:
-                The amount of lines after the invocation of this function that
-                callsite parameters should be generated for.
-        """
-        frame_info = inspect.stack()[1]
-        frame_traceback = inspect.getframeinfo(frame_info[0])
-        return {
-            "pathname": frame_traceback.filename,
-            "filename": os.path.basename(frame_traceback.filename),
-            "module": os.path.splitext(
-                os.path.basename(frame_traceback.filename)
-            )[0],
-            "func_name": frame_info.function,
-            "lineno": frame_info.lineno + offset,
-            "thread": threading.get_ident(),
-            "thread_name": threading.current_thread().name,
-            "process": os.getpid(),
-            "process_name": get_processname(),
-        }
+        assert l1 is not l2
+        assert l1.sync_bl is not l2.sync_bl
+        assert {} == l1._context
+        assert {"x": 42} == l2._context
 
+        l3 = l2.new(y=23)
 
-class TestRenameKey:
-    def test_rename_once(self):
+        assert l2 is not l3
+        assert l2.sync_bl is not l3.sync_bl
+        assert {"y": 23} == l3._context
+
+        l4 = l3.unbind("y")
+
+        assert {} == l4._context
+        assert l3 is not l4
+
+        # N.B. x isn't bound anymore.
+        l5 = l4.try_unbind("x")
+
+        assert {} == l5._context
+        assert l4 is not l5
+
+    @pytest.mark.asyncio()
+    async def test_integration(self, capsys):
         """
-        Renaming event to something else works.
+        Configure and log an actual entry.
         """
-        assert {"msg": "hi", "foo": "bar"} == EventRenamer("msg")(
-            None, None, {"event": "hi", "foo": "bar"}
+
+        configure(
+            processors=[add_log_level, JSONRenderer()],
+            logger_factory=PrintLogger,
+            wrapper_class=AsyncBoundLogger,
+            cache_logger_on_first_use=True,
         )
 
-    def test_rename_twice(self):
-        """
-        Renaming both from and to `event` works.
-        """
+        logger = get_logger()
+
+        await logger.bind(foo="bar").info("baz", x="42")
+
         assert {
-            "msg": "hi",
-            "event": "fabulous",
             "foo": "bar",
-        } == EventRenamer("msg", "_event")(
-            None, None, {"event": "hi", "foo": "bar", "_event": "fabulous"}
-        )
+            "x": "42",
+            "event": "baz",
+            "level": "info",
+        } == json.loads(capsys.readouterr().out)
 
-    def test_replace_by_key_is_optional(self):
-        """
-        The key that is renamed to `event` doesn't have to exist.
-        """
-        assert {"msg": "hi", "foo": "bar"} == EventRenamer("msg", "missing")(
-            None, None, {"event": "hi", "foo": "bar"}
-        )
+
+@pytest.mark.parametrize("log_level", [None, 45])
+def test_recreate_defaults(log_level):
+    """
+    Recreate defaults configures structlog and -- if asked -- logging.
+    """
+    logging.basicConfig(
+        stream=sys.stderr,
+        level=1,
+        force=True,
+    )
+
+    recreate_defaults(log_level=log_level)
+
+    assert BoundLogger is _CONFIG.default_wrapper_class
+    assert dict is _CONFIG.default_context_class
+    assert isinstance(_CONFIG.logger_factory, LoggerFactory)
+
+    log = get_logger().bind()
+    if log_level is not None:
+        assert log_level == log.getEffectiveLevel()
+    else:
+        assert 1 == log.getEffectiveLevel()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `structlog-24.1.0/tests/test_testing.py` & `structlog-24.2.0/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/tests/test_threadlocal.py` & `structlog-24.2.0/tests/test_threadlocal.py`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/tests/test_tracebacks.py` & `structlog-24.2.0/tests/test_tracebacks.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,15 +298,15 @@
 def test_syntax_error():
     """
     For SyntaxError, extra info about that error is added to the trace.
     """
     try:
         # raises SyntaxError: invalid syntax
         lineno = get_next_lineno()
-        eval("2 +* 2")  # noqa: PGH001
+        eval("2 +* 2")
     except SyntaxError as e:
         trace = tracebacks.extract(type(e), e, e.__traceback__)
 
     assert [
         tracebacks.Stack(
             exc_type="SyntaxError",
             exc_value="invalid syntax (<string>, line 1)",
```

### Comparing `structlog-24.1.0/tests/test_twisted.py` & `structlog-24.2.0/tests/test_twisted.py`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/tests/typing/api.py` & `structlog-24.2.0/tests/typing/api.py`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/LICENSE-APACHE` & `structlog-24.2.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/LICENSE-MIT` & `structlog-24.2.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `structlog-24.1.0/pyproject.toml` & `structlog-24.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,16 @@
 
 [tool.black]
 line-length = 79
 
 
 [tool.ruff]
 src = ["src", "tests"]
+
+[tool.ruff.lint]
 select = ["ALL"]
 ignore = [
     "A",       # shadowing is fine
     "ANN",     # Mypy is better at this
     "ARG",     # unused arguments are common w/ interfaces
     "C901",    # sometimes you trade complexity for performance
     "COM",     # Black takes care of our commas
@@ -139,40 +141,43 @@
     "PLW2901", # overwriting a loop var can be useful
     "RUF001",  # leave my smart characters alone
     "RUF001",  # leave my smart characters alone
     "SLF001",  # private members are accessed by friendly functions
     "T201",    # prints are fine
     "TCH",     # TYPE_CHECKING blocks break autodocs
     "TD",      # we don't follow other people's todo style
+    "TID252",  # Relative imports are fine
     "TRY003",  # simple strings are fine
     "TRY004",  # too many false negatives
     "TRY300",  # else blocks are nice, but code-locality is nicer
     "PTH",     # pathlib can be slow, so no point to rewrite
 ]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/*" = [
     "B018",    # "useless" expressions can be useful in tests
     "BLE",     # tests have different rules around exceptions
     "EM",      # tests have different rules around exceptions
+    "LOG001",  # need to instantiate log messages in tests
     "PLC1901", # empty strings are falsey, but are less specific in tests
     "PT005",   # we always add underscores and explicit name
     "RUF012",  # no type hints in tests
     "S",       # it's test; chill out security
     "SIM300",  # Yoda rocks in tests
     "TRY",     # tests have different rules around exceptions
 ]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 lines-between-types = 1
 lines-after-imports = 2
 
 
 [tool.mypy]
 strict = true
+pretty = true
 
 show_error_codes = true
 enable_error_code = ["ignore-without-code"]
 ignore_missing_imports = true
 
 warn_return_any = false
```

### Comparing `structlog-24.1.0/PKG-INFO` & `structlog-24.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: structlog
-Version: 24.1.0
+Version: 24.2.0
 Summary: Structured Logging for Python
 Project-URL: Documentation, https://www.structlog.org/
 Project-URL: Changelog, https://github.com/hynek/structlog/blob/main/CHANGELOG.md
 Project-URL: GitHub, https://github.com/hynek/structlog
 Project-URL: Funding, https://github.com/sponsors/hynek
 Project-URL: Tidelift, https://tidelift.com?utm_source=lifter&utm_medium=referral&utm_campaign=hynek
 Project-URL: Mastodon, https://mastodon.social/@hynek
@@ -23,15 +23,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Logging
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Provides-Extra: dev
-Requires-Dist: structlog[tests,typing]; extra == 'dev'
+Requires-Dist: freezegun>=0.2.8; extra == 'dev'
+Requires-Dist: mypy>=1.4; extra == 'dev'
+Requires-Dist: pretend; extra == 'dev'
+Requires-Dist: pytest-asyncio>=0.17; extra == 'dev'
+Requires-Dist: pytest>=6.0; extra == 'dev'
+Requires-Dist: rich; extra == 'dev'
+Requires-Dist: simplejson; extra == 'dev'
+Requires-Dist: twisted; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: furo; extra == 'docs'
 Requires-Dist: myst-parser; extra == 'docs'
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx-notfound-page; extra == 'docs'
 Requires-Dist: sphinxcontrib-mermaid; extra == 'docs'
 Requires-Dist: sphinxext-opengraph; extra == 'docs'
@@ -74,14 +81,15 @@
 
 *structlog* would not be possible without our [amazing sponsors](https://github.com/sponsors/hynek).
 Especially those generously supporting us at the *The Organization* tier and higher:
 
 <p align="center">
    <a href="https://www.variomedia.de/"><img src="https://raw.githubusercontent.com/hynek/structlog/main/.github/sponsors/Variomedia.svg" width="200" height="60" /></a>
    <a href="https://tidelift.com/?utm_source=lifter&utm_medium=referral&utm_campaign=hynek"><img src="https://raw.githubusercontent.com/hynek/structlog/main/.github/sponsors/Tidelift.svg" width="200" height="60" /></a>
+   <a href="https://klaviyo.com/"><img src="https://raw.githubusercontent.com/hynek/structlog/main/.github/sponsors/Klaviyo.svg" width="200" height="60"/></a>
    <a href="https://filepreviews.io/"><img src="https://raw.githubusercontent.com/hynek/structlog/main/.github/sponsors/FilePreviews.svg" width="200" height="60" /></a>
 </p>
 
 <p align="center">
    <strong>Please consider <a href="https://github.com/sponsors/hynek">joining them</a> to help make <em>structlog</em>’s maintenance more sustainable!</strong>
 </p>
 
@@ -107,25 +115,43 @@
 Available as part of the Tidelift Subscription.
 
 The maintainers of *structlog* and thousands of other packages are working with Tidelift to deliver commercial support and maintenance for the open source packages you use to build your applications. Save time, reduce risk, and improve code health, while paying the maintainers of the exact packages you use. [Learn more.](https://tidelift.com/?utm_source=lifter&utm_medium=referral&utm_campaign=hynek)
 
 
 ## Release Information
 
-### Fixed
+### Added
+
+- It is now possible to disable log level-padding in `structlog.dev.LogLevelColumnFormatter` and `structlog.dev.ConsoleRenderer`.
+  [#599](https://github.com/hynek/structlog/pull/599)
+
+- The `structlog.processors.CallsiteParameterAdder` can now be pickled.
+  [#603](https://github.com/hynek/structlog/pull/603)
+
+- `structlog.processors.CallsiteParameterAdder` now also works with `structlog.stdlib.BoundLogger`'s non-standard async methods (`ainfo()`, and so forth)
+  [#618](https://github.com/hynek/structlog/pull/618)
+
+
+### Changed
 
-- The lazy logger proxy returned by `structlog.get_logger()` now returns its initial values when asked for context.
-  When asked for context before binding for the first time, it returned an empty dictionary in 23.3.0.
+- `structlog.processors.LogfmtRenderer` now escapes newlines.
+  [#592](https://github.com/hynek/structlog/pull/592)
+
+- `structlog.processors.LogfmtRenderer` now escapes backslashes and double quotes.
+  [#594](https://github.com/hynek/structlog/pull/594)
+
+- `structlog.processors.CallsiteParameterAdder` has been optimized to be about 2x faster.
+  [#606](https://github.com/hynek/structlog/pull/606)
+
+
+### Fixed
 
-- The displayed level name when using `structlog.stdlib.BoundLogger.exception()` is `"error"` instead of `"exception"`.
-  Fixes regression in 23.3.0.
-  [#584](https://github.com/hynek/structlog/issues/584)
+- `structlog.stdlib.render_to_log_kwargs` now correctly passes stacklevel as a kwarg to stdlib logging.
+  [#619](https://github.com/hynek/structlog/pull/620)
 
-- Don't ignore the `width` argument of `RichTracebackFormatter`.
-  [#587](https://github.com/hynek/structlog/issues/587)
 
 
 ---
 
 [Full Changelog →](https://www.structlog.org/en/stable/changelog.html)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: structlog Version: 24.1.0 Summary: Structured
+Metadata-Version: 2.3 Name: structlog Version: 24.2.0 Summary: Structured
 Logging for Python Project-URL: Documentation, https://www.structlog.org/
 Project-URL: Changelog, https://github.com/hynek/structlog/blob/main/
 CHANGELOG.md Project-URL: GitHub, https://github.com/hynek/structlog Project-
 URL: Funding, https://github.com/sponsors/hynek Project-URL: Tidelift, https://
 tidelift.com?utm_source=lifter&utm_medium=referral&utm_campaign=hynek Project-
 URL: Mastodon, https://mastodon.social/@hynek Project-URL: Twitter, https://
 twitter.com/hynek Author-email: Hynek Schlawack
@@ -11,26 +11,30 @@
 log,logging,structure,structured Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: System :: Logging Classifier: Typing ::
-Typed Requires-Python: >=3.8 Provides-Extra: dev Requires-Dist: structlog
-[tests,typing]; extra == 'dev' Provides-Extra: docs Requires-Dist: furo; extra
-== 'docs' Requires-Dist: myst-parser; extra == 'docs' Requires-Dist: sphinx;
-extra == 'docs' Requires-Dist: sphinx-notfound-page; extra == 'docs' Requires-
-Dist: sphinxcontrib-mermaid; extra == 'docs' Requires-Dist: sphinxext-
-opengraph; extra == 'docs' Requires-Dist: twisted; extra == 'docs' Provides-
-Extra: tests Requires-Dist: freezegun>=0.2.8; extra == 'tests' Requires-Dist:
-pretend; extra == 'tests' Requires-Dist: pytest-asyncio>=0.17; extra == 'tests'
-Requires-Dist: pytest>=6.0; extra == 'tests' Requires-Dist: simplejson; extra
-== 'tests' Provides-Extra: typing Requires-Dist: mypy>=1.4; extra == 'typing'
-Requires-Dist: rich; extra == 'typing' Requires-Dist: twisted; extra ==
-'typing' Description-Content-Type: text/markdown
+Typed Requires-Python: >=3.8 Provides-Extra: dev Requires-Dist:
+freezegun>=0.2.8; extra == 'dev' Requires-Dist: mypy>=1.4; extra == 'dev'
+Requires-Dist: pretend; extra == 'dev' Requires-Dist: pytest-asyncio>=0.17;
+extra == 'dev' Requires-Dist: pytest>=6.0; extra == 'dev' Requires-Dist: rich;
+extra == 'dev' Requires-Dist: simplejson; extra == 'dev' Requires-Dist:
+twisted; extra == 'dev' Provides-Extra: docs Requires-Dist: furo; extra ==
+'docs' Requires-Dist: myst-parser; extra == 'docs' Requires-Dist: sphinx; extra
+== 'docs' Requires-Dist: sphinx-notfound-page; extra == 'docs' Requires-Dist:
+sphinxcontrib-mermaid; extra == 'docs' Requires-Dist: sphinxext-opengraph;
+extra == 'docs' Requires-Dist: twisted; extra == 'docs' Provides-Extra: tests
+Requires-Dist: freezegun>=0.2.8; extra == 'tests' Requires-Dist: pretend; extra
+== 'tests' Requires-Dist: pytest-asyncio>=0.17; extra == 'tests' Requires-Dist:
+pytest>=6.0; extra == 'tests' Requires-Dist: simplejson; extra == 'tests'
+Provides-Extra: typing Requires-Dist: mypy>=1.4; extra == 'typing' Requires-
+Dist: rich; extra == 'typing' Requires-Dist: twisted; extra == 'typing'
+Description-Content-Type: text/markdown
                               [structlog mascot]
 *structlog* is *the* production-ready logging solution for Python: -
 **Simple**: Everything is about **functions** that take and return
 **dictionaries** â all hidden behind **familiar APIs**. - **Powerful**:
 Functions and dictionaries arenât just simple but also powerful. *structlog*
 leaves *you* in control. - **Fast**: *structlog* is not hamstrung by designs of
 yore. Its flexibility comes not at the price of performance. Thanks to its
@@ -44,15 +48,16 @@
 blob/main/docs/_static/console_renderer.png?raw=true) ## Sponsors *structlog*
 would not be possible without our [amazing sponsors](https://github.com/
 sponsors/hynek). Especially those generously supporting us at the *The
 Organization* tier and higher:
    _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_h_y_n_e_k_/_s_t_r_u_c_t_l_o_g_/_m_a_i_n_/_._g_i_t_h_u_b_/_s_p_o_n_s_o_r_s_/
 _V_a_r_i_o_m_e_d_i_a_._s_v_g_]_[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_h_y_n_e_k_/_s_t_r_u_c_t_l_o_g_/_m_a_i_n_/_._g_i_t_h_u_b_/
    _s_p_o_n_s_o_r_s_/_T_i_d_e_l_i_f_t_._s_v_g_]_[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_h_y_n_e_k_/_s_t_r_u_c_t_l_o_g_/
-                    _m_a_i_n_/_._g_i_t_h_u_b_/_s_p_o_n_s_o_r_s_/_F_i_l_e_P_r_e_v_i_e_w_s_._s_v_g_]
+  _m_a_i_n_/_._g_i_t_h_u_b_/_s_p_o_n_s_o_r_s_/_K_l_a_v_i_y_o_._s_v_g_]_[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_h_y_n_e_k_/
+               _s_t_r_u_c_t_l_o_g_/_m_a_i_n_/_._g_i_t_h_u_b_/_s_p_o_n_s_o_r_s_/_F_i_l_e_P_r_e_v_i_e_w_s_._s_v_g_]
    PPlleeaassee ccoonnssiiddeerr _jj_oo_ii_nn_ii_nn_gg_ _tt_hh_ee_mm ttoo hheellpp mmaakkee ssttrruuccttlloogg?â??ss mmaaiinntteennaannccee mmoorree
                                  ssuussttaaiinnaabbllee!!
 --- *structlog* has been successfully used in production at every scale since
 **2013**, while embracing cutting-edge technologies like *asyncio*, context
 variables, or type hints as they emerged. Its paradigms proved influential
 enough to [help design](https://twitter.com/sirupsen/status/638330548361019392)
 structured logging [packages across ecosystems](https://github.com/sirupsen/
@@ -65,25 +70,32 @@
 ## *structlog* for Enterprise Available as part of the Tidelift Subscription.
 The maintainers of *structlog* and thousands of other packages are working with
 Tidelift to deliver commercial support and maintenance for the open source
 packages you use to build your applications. Save time, reduce risk, and
 improve code health, while paying the maintainers of the exact packages you
 use. [Learn more.](https://tidelift.com/
 ?utm_source=lifter&utm_medium=referral&utm_campaign=hynek) ## Release
-Information ### Fixed - The lazy logger proxy returned by `structlog.get_logger
-()` now returns its initial values when asked for context. When asked for
-context before binding for the first time, it returned an empty dictionary in
-23.3.0. - The displayed level name when using
-`structlog.stdlib.BoundLogger.exception()` is `"error"` instead of
-`"exception"`. Fixes regression in 23.3.0. [#584](https://github.com/hynek/
-structlog/issues/584) - Don't ignore the `width` argument of
-`RichTracebackFormatter`. [#587](https://github.com/hynek/structlog/issues/587)
---- [Full Changelog â](https://www.structlog.org/en/stable/changelog.html) ##
-Credits *structlog* is written and maintained by [Hynek Schlawack](https://
-hynek.me/). The idea of bound loggers is inspired by previous work by [Jean-
-Paul Calderone](https://github.com/exarkun) and [David Reid](https://
-github.com/dreid). The development is kindly supported by my employer
-[Variomedia AG](https://www.variomedia.de/), *structlog*âs [Tidelift
+Information ### Added - It is now possible to disable log level-padding in
+`structlog.dev.LogLevelColumnFormatter` and `structlog.dev.ConsoleRenderer`.
+[#599](https://github.com/hynek/structlog/pull/599) - The
+`structlog.processors.CallsiteParameterAdder` can now be pickled. [#603](https:
+//github.com/hynek/structlog/pull/603) -
+`structlog.processors.CallsiteParameterAdder` now also works with
+`structlog.stdlib.BoundLogger`'s non-standard async methods (`ainfo()`, and so
+forth) [#618](https://github.com/hynek/structlog/pull/618) ### Changed -
+`structlog.processors.LogfmtRenderer` now escapes newlines. [#592](https://
+github.com/hynek/structlog/pull/592) - `structlog.processors.LogfmtRenderer`
+now escapes backslashes and double quotes. [#594](https://github.com/hynek/
+structlog/pull/594) - `structlog.processors.CallsiteParameterAdder` has been
+optimized to be about 2x faster. [#606](https://github.com/hynek/structlog/
+pull/606) ### Fixed - `structlog.stdlib.render_to_log_kwargs` now correctly
+passes stacklevel as a kwarg to stdlib logging. [#619](https://github.com/
+hynek/structlog/pull/620) --- [Full Changelog â](https://www.structlog.org/
+en/stable/changelog.html) ## Credits *structlog* is written and maintained by
+[Hynek Schlawack](https://hynek.me/). The idea of bound loggers is inspired by
+previous work by [Jean-Paul Calderone](https://github.com/exarkun) and [David
+Reid](https://github.com/dreid). The development is kindly supported by my
+employer [Variomedia AG](https://www.variomedia.de/), *structlog*âs [Tidelift
 subscribers](https://tidelift.com/
 ?utm_source=lifter&utm_medium=referral&utm_campaign=hynek), and all my amazing
 [GitHub Sponsors](https://github.com/sponsors/hynek). The logs-loving beaver
 logo has been contributed by [Lynn Root](https://www.roguelynn.com).
```

