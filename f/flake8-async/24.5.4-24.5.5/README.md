# Comparing `tmp/flake8_async-24.5.4.tar.gz` & `tmp/flake8_async-24.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_async-24.5.4.tar", last modified: Mon May 27 11:34:37 2024, max compression
+gzip compressed data, was "flake8_async-24.5.5.tar", last modified: Mon May 27 18:27:22 2024, max compression
```

## Comparing `flake8_async-24.5.4.tar` & `flake8_async-24.5.5.tar`

### file list

```diff
@@ -1,139 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:34:37.646502 flake8_async-24.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-27 11:34:29.000000 flake8_async-24.5.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-27 11:34:29.000000 flake8_async-24.5.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-27 11:34:29.000000 flake8_async-24.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-27 11:34:29.000000 flake8_async-24.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-27 11:34:37.646502 flake8_async-24.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-27 11:34:29.000000 flake8_async-24.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:34:37.626502 flake8_async-24.5.4/flake8_async/
--rw-r--r--   0 runner    (1001) docker     (127)    15959 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:34:37.630502 flake8_async-24.5.4/flake8_async/visitors/
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/flake8asyncvisitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15337 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/visitor101.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/visitor102.py
--rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/visitor103_104.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/visitor105.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/visitor111.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/visitor118.py
--rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/visitor2xx.py
--rw-r--r--   0 runner    (1001) docker     (127)    40658 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/visitor91x.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/visitor_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)    12683 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:34:37.646502 flake8_async-24.5.4/flake8_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-27 11:34:37.000000 flake8_async-24.5.4/flake8_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-27 11:34:37.000000 flake8_async-24.5.4/flake8_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 11:34:37.000000 flake8_async-24.5.4/flake8_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-27 11:34:37.000000 flake8_async-24.5.4/flake8_async.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 11:34:37.000000 flake8_async-24.5.4/flake8_async.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-27 11:34:37.000000 flake8_async-24.5.4/flake8_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 11:34:37.000000 flake8_async-24.5.4/flake8_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-27 11:34:29.000000 flake8_async-24.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 11:34:37.646502 flake8_async-24.5.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2204 2024-05-27 11:34:29.000000 flake8_async-24.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:34:37.634503 flake8_async-24.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:34:37.634503 flake8_async-24.5.4/tests/autofix_files/
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/async100.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/async100_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/async100_simple_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)    12020 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/async910.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/async910_insert_library.py
--rw-r--r--   0 runner    (1001) docker     (127)    28741 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/async911.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/async911_insert_library.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/async913.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/async91x_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/exception_suppress_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/exception_suppress_context_manager_import_star.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/noqa.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/noqa_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:34:37.646502 flake8_async-24.5.4/tests/eval_files/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/anyio_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async100.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async100_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async100_noautofix.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async100_simple_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async101.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async101_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async101_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async101_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     7082 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async102.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async102_aclose.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async102_aclose_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async102_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async102_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async102_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async103.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async103_all_imported.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async103_both_imported.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async103_no_104.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async103_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async104.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async104_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async104_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async105.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async105_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async106.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async109.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async110.py
--rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async111.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async111_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async111_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async112.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async112_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async112_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async113.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async113_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async113_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async114.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async115.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async116.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async118.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async119.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async200.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async210.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async211.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async212.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async22x.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async22x_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async232.py
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async232_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async23x.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async23x_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async240.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async250.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async250_multi_library.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async251.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async251_multi_library.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async900.py
--rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async910.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async910_insert_library.py
--rw-r--r--   0 runner    (1001) docker     (127)    24009 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async911.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async911_insert_library.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async912.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async912_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async913.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async91x_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async91x_noautofix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/exception_suppress_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/exception_suppress_context_manager_import_star.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/no_library.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/noqa.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/noqa_no_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/noqa_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/trio_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/test_all_visitors_imported.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3807 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/test_changelog_and_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12695 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/test_config_and_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/test_exception_on_invalid_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    29839 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/test_flake8_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/test_formatting.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3425 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/test_messages_documented.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/trio_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:27:22.966097 flake8_async-24.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-27 18:27:15.000000 flake8_async-24.5.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-27 18:27:15.000000 flake8_async-24.5.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-27 18:27:15.000000 flake8_async-24.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-27 18:27:15.000000 flake8_async-24.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-27 18:27:22.966097 flake8_async-24.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-27 18:27:15.000000 flake8_async-24.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:27:22.950097 flake8_async-24.5.5/flake8_async/
+-rw-r--r--   0 runner    (1001) docker     (127)    15959 2024-05-27 18:27:15.000000 flake8_async-24.5.5/flake8_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-27 18:27:15.000000 flake8_async-24.5.5/flake8_async/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-27 18:27:15.000000 flake8_async-24.5.5/flake8_async/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-05-27 18:27:15.000000 flake8_async-24.5.5/flake8_async/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:27:22.950097 flake8_async-24.5.5/flake8_async/visitors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-27 18:27:15.000000 flake8_async-24.5.5/flake8_async/visitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-05-27 18:27:15.000000 flake8_async-24.5.5/flake8_async/visitors/flake8asyncvisitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15501 2024-05-27 18:27:15.000000 flake8_async-24.5.5/flake8_async/visitors/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-27 18:27:15.000000 flake8_async-24.5.5/flake8_async/visitors/visitor101.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-27 18:27:15.000000 flake8_async-24.5.5/flake8_async/visitors/visitor102.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-05-27 18:27:15.000000 flake8_async-24.5.5/flake8_async/visitors/visitor103_104.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-27 18:27:15.000000 flake8_async-24.5.5/flake8_async/visitors/visitor105.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-27 18:27:15.000000 flake8_async-24.5.5/flake8_async/visitors/visitor111.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-27 18:27:15.000000 flake8_async-24.5.5/flake8_async/visitors/visitor118.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-05-27 18:27:15.000000 flake8_async-24.5.5/flake8_async/visitors/visitor2xx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40658 2024-05-27 18:27:15.000000 flake8_async-24.5.5/flake8_async/visitors/visitor91x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-27 18:27:15.000000 flake8_async-24.5.5/flake8_async/visitors/visitor_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14296 2024-05-27 18:27:15.000000 flake8_async-24.5.5/flake8_async/visitors/visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:27:22.966097 flake8_async-24.5.5/flake8_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-27 18:27:22.000000 flake8_async-24.5.5/flake8_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-27 18:27:22.000000 flake8_async-24.5.5/flake8_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 18:27:22.000000 flake8_async-24.5.5/flake8_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-27 18:27:22.000000 flake8_async-24.5.5/flake8_async.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 18:27:22.000000 flake8_async-24.5.5/flake8_async.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-27 18:27:22.000000 flake8_async-24.5.5/flake8_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 18:27:22.000000 flake8_async-24.5.5/flake8_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-27 18:27:15.000000 flake8_async-24.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 18:27:22.966097 flake8_async-24.5.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2204 2024-05-27 18:27:15.000000 flake8_async-24.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:27:22.954097 flake8_async-24.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:27:22.954097 flake8_async-24.5.5/tests/autofix_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/autofix_files/async100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/autofix_files/async100_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/autofix_files/async100_simple_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12020 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/autofix_files/async910.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/autofix_files/async910_insert_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28741 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/autofix_files/async911.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/autofix_files/async911_insert_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/autofix_files/async913.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/autofix_files/async91x_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/autofix_files/exception_suppress_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/autofix_files/exception_suppress_context_manager_import_star.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/autofix_files/noqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/autofix_files/noqa_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:27:22.966097 flake8_async-24.5.5/tests/eval_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/anyio_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async100_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async100_noautofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async100_simple_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async101.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async101_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async101_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async101_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7082 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async102.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async102_aclose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async102_aclose_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async102_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async102_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async102_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async103.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async103_all_imported.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async103_both_imported.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async103_no_104.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async103_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async104.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async104_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async104_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async105.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async105_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async106.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async109.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async111.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async111_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async111_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async112.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async112_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async112_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async113.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async113_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async113_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async114.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async115.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async116.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async118.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async119.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async210.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async211.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async212.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async22x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async22x_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async232.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async232_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async23x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async23x_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async240.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async250.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async250_multi_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async251.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async251_multi_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async300.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async900.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async910.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async910_insert_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24009 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async911.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async911_insert_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async912.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async912_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async913.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async91x_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/async91x_noautofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/exception_suppress_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/exception_suppress_context_manager_import_star.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/no_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/noqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/noqa_no_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/noqa_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/eval_files/trio_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/test_all_visitors_imported.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3807 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/test_changelog_and_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12695 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/test_config_and_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/test_exception_on_invalid_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29855 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/test_flake8_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/test_formatting.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3425 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/test_messages_documented.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tests/trio_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-27 18:27:15.000000 flake8_async-24.5.5/tox.ini
```

### Comparing `flake8_async-24.5.4/LICENSE` & `flake8_async-24.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/PKG-INFO` & `flake8_async-24.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-async
-Version: 24.5.4
+Version: 24.5.5
 Summary: A highly opinionated flake8 plugin for Trio-related problems.
 Author: Zac Hatfield-Dodds, John Litborn, and Contributors
 Author-email: zac@zhd.dev
 License: MIT
 Project-URL: Homepage, https://github.com/python-trio/flake8-async
 Project-URL: Documentation, https://flake8-async.readthedocs.io/
 Project-URL: Changelog, https://flake8-async.readthedocs.io/en/latest/changelog.html
```

### Comparing `flake8_async-24.5.4/README.md` & `flake8_async-24.5.5/README.md`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/flake8_async/__init__.py` & `flake8_async-24.5.5/flake8_async/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     from flake8.options.manager import OptionManager
 
     from .base import Error
 
 
 # CalVer: YY.month.patch, e.g. first release of July 2022 == "22.7.1"
-__version__ = "24.5.4"
+__version__ = "24.5.5"
 
 
 # taken from https://github.com/Zac-HD/shed
 @functools.lru_cache
 def _get_git_repo_root(cwd: str | None = None) -> str:
     return subprocess.run(
         ["git", "rev-parse", "--show-toplevel"],
```

### Comparing `flake8_async-24.5.4/flake8_async/base.py` & `flake8_async-24.5.5/flake8_async/base.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/flake8_async/runner.py` & `flake8_async-24.5.5/flake8_async/runner.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/flake8_async/visitors/__init__.py` & `flake8_async-24.5.5/flake8_async/visitors/__init__.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/flake8_async/visitors/flake8asyncvisitor.py` & `flake8_async-24.5.5/flake8_async/visitors/flake8asyncvisitor.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/flake8_async/visitors/helpers.py` & `flake8_async-24.5.5/flake8_async/visitors/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,19 +333,23 @@
     """Build a cst matcher structure with attributes&names matching a string `a.b.c`."""
     if "." not in attr:
         return m.Name(value=attr)
     body, tail = attr.rsplit(".")
     return m.Attribute(value=build_cst_matcher(body), attr=m.Name(value=tail))
 
 
-def identifier_to_string(attr: cst.Name | cst.Attribute) -> str:
+def identifier_to_string(attr: cst.Name | cst.Attribute) -> str | None:
     if isinstance(attr, cst.Name):
         return attr.value
-    assert isinstance(attr.value, (cst.Attribute, cst.Name))
-    return identifier_to_string(attr.value) + "." + attr.attr.value
+    if not isinstance(attr.value, (cst.Attribute, cst.Name)):
+        return None
+    lhs = identifier_to_string(attr.value)
+    if lhs is None:
+        return None
+    return lhs + "." + attr.attr.value
 
 
 def with_has_call(
     node: cst.With, *names: str, base: Iterable[str] | str = ("trio", "anyio")
 ) -> list[AttributeCall]:
     """Check if a with statement has a matching call, returning a list with matches.
 
@@ -379,18 +383,18 @@
 
     res_list: list[AttributeCall] = []
     for item in node.items:
         if res := m.extract(item.item, matcher):
             assert isinstance(item.item, cst.Call)
             assert isinstance(res["base"], (cst.Name, cst.Attribute))
             assert isinstance(res["function"], cst.Name)
+            base_string = identifier_to_string(res["base"])
+            assert base_string is not None, "subscripts should never get matched"
             res_list.append(
-                AttributeCall(
-                    item.item, identifier_to_string(res["base"]), res["function"].value
-                )
+                AttributeCall(item.item, base_string, res["function"].value)
             )
     return res_list
 
 
 def func_has_decorator(func: cst.FunctionDef, *names: str) -> bool:
     return any(
         list_contains(
```

### Comparing `flake8_async-24.5.4/flake8_async/visitors/visitor101.py` & `flake8_async-24.5.5/flake8_async/visitors/visitor101.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/flake8_async/visitors/visitor102.py` & `flake8_async-24.5.5/flake8_async/visitors/visitor102.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/flake8_async/visitors/visitor103_104.py` & `flake8_async-24.5.5/flake8_async/visitors/visitor103_104.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/flake8_async/visitors/visitor105.py` & `flake8_async-24.5.5/flake8_async/visitors/visitor105.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/flake8_async/visitors/visitor111.py` & `flake8_async-24.5.5/flake8_async/visitors/visitor111.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/flake8_async/visitors/visitor118.py` & `flake8_async-24.5.5/flake8_async/visitors/visitor118.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/flake8_async/visitors/visitor2xx.py` & `flake8_async-24.5.5/flake8_async/visitors/visitor2xx.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/flake8_async/visitors/visitor91x.py` & `flake8_async-24.5.5/flake8_async/visitors/visitor91x.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/flake8_async/visitors/visitor_utility.py` & `flake8_async-24.5.5/flake8_async/visitors/visitor_utility.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/flake8_async/visitors/visitors.py` & `flake8_async-24.5.5/flake8_async/visitors/visitors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 """Various visitors/error classes that are too small to warrant getting their own file."""
 
 from __future__ import annotations
 
 import ast
 from typing import TYPE_CHECKING, Any, cast
 
-from .flake8asyncvisitor import Flake8AsyncVisitor
-from .helpers import disabled_by_default, error_class, get_matching_call, has_decorator
+import libcst as cst
+
+from .flake8asyncvisitor import Flake8AsyncVisitor, Flake8AsyncVisitor_cst
+from .helpers import (
+    disabled_by_default,
+    error_class,
+    error_class_cst,
+    get_matching_call,
+    has_decorator,
+    identifier_to_string,
+)
 
 if TYPE_CHECKING:
     from collections.abc import Mapping
 
 LIBRARIES = ("trio", "anyio", "asyncio")
 
 
@@ -328,14 +337,61 @@
     visit_AsyncWith = visit_With
     visit_FunctionDef = visit_AsyncFunctionDef
     # it's not possible to yield or open context managers in lambda's, so this
     # one isn't strictly needed afaik.
     visit_Lambda = visit_AsyncFunctionDef
 
 
+@error_class_cst
+class Visitor300(Flake8AsyncVisitor_cst):
+    error_codes: Mapping[str, str] = {
+        "ASYNC300": "asyncio.create_task() called without saving the result"
+    }
+
+    def __init__(self, *args: Any, **kwargs: Any):
+        super().__init__(*args, **kwargs)
+        self.safe_to_create_task: bool = False
+
+    def visit_Assign(self, node: cst.CSTNode):
+        self.save_state(node, "safe_to_create_task")
+        self.safe_to_create_task = True
+
+    def visit_CompIf(self, node: cst.CSTNode):
+        self.save_state(node, "safe_to_create_task")
+        self.safe_to_create_task = False
+
+    def visit_Call(self, node: cst.Call):
+        if (
+            isinstance(node.func, (cst.Name, cst.Attribute))
+            and identifier_to_string(node.func) == "asyncio.create_task"
+            and not self.safe_to_create_task
+        ):
+            self.error(node)
+        self.visit_Assign(node)
+
+    visit_NamedExpr = visit_Assign
+    visit_AugAssign = visit_Assign
+    visit_IfExp_test = visit_CompIf
+
+    # because this is a Flake8AsyncVisitor_cst, we need to manually call restore_state
+    def leave_Assign(
+        self, original_node: cst.CSTNode, updated_node: cst.CSTNode
+    ) -> Any:
+        self.restore_state(original_node)
+        return updated_node
+
+    leave_Call = leave_Assign
+    leave_CompIf = leave_Assign
+    leave_NamedExpr = leave_Assign
+    leave_AugAssign = leave_Assign
+
+    def leave_IfExp_test(self, node: cst.IfExp):
+        self.restore_state(node)
+
+
 @error_class
 @disabled_by_default
 class Visitor900(Flake8AsyncVisitor):
     error_codes: Mapping[str, str] = {
         "ASYNC900": "Async generator without `@asynccontextmanager` not allowed."
     }
```

### Comparing `flake8_async-24.5.4/flake8_async.egg-info/PKG-INFO` & `flake8_async-24.5.5/flake8_async.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-async
-Version: 24.5.4
+Version: 24.5.5
 Summary: A highly opinionated flake8 plugin for Trio-related problems.
 Author: Zac Hatfield-Dodds, John Litborn, and Contributors
 Author-email: zac@zhd.dev
 License: MIT
 Project-URL: Homepage, https://github.com/python-trio/flake8-async
 Project-URL: Documentation, https://flake8-async.readthedocs.io/
 Project-URL: Changelog, https://flake8-async.readthedocs.io/en/latest/changelog.html
```

### Comparing `flake8_async-24.5.4/flake8_async.egg-info/SOURCES.txt` & `flake8_async-24.5.5/flake8_async.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 tests/eval_files/async23x.py
 tests/eval_files/async23x_asyncio.py
 tests/eval_files/async240.py
 tests/eval_files/async250.py
 tests/eval_files/async250_multi_library.py
 tests/eval_files/async251.py
 tests/eval_files/async251_multi_library.py
+tests/eval_files/async300.py
 tests/eval_files/async900.py
 tests/eval_files/async910.py
 tests/eval_files/async910_insert_library.py
 tests/eval_files/async911.py
 tests/eval_files/async911_insert_library.py
 tests/eval_files/async912.py
 tests/eval_files/async912_asyncio.py
```

### Comparing `flake8_async-24.5.4/pyproject.toml` & `flake8_async-24.5.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/setup.py` & `flake8_async-24.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/autofix_files/async100.py` & `flake8_async-24.5.5/tests/autofix_files/async100.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/autofix_files/async100_simple_autofix.py` & `flake8_async-24.5.5/tests/autofix_files/async100_simple_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/autofix_files/async910.py` & `flake8_async-24.5.5/tests/autofix_files/async910.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/autofix_files/async911.py` & `flake8_async-24.5.5/tests/autofix_files/async911.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/autofix_files/async913.py` & `flake8_async-24.5.5/tests/autofix_files/async913.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/autofix_files/async91x_autofix.py` & `flake8_async-24.5.5/tests/autofix_files/async91x_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/autofix_files/exception_suppress_context_manager.py` & `flake8_async-24.5.5/tests/autofix_files/exception_suppress_context_manager.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/autofix_files/noqa.py` & `flake8_async-24.5.5/tests/autofix_files/noqa.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/conftest.py` & `flake8_async-24.5.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async100.py` & `flake8_async-24.5.5/tests/eval_files/async100.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async100_asyncio.py` & `flake8_async-24.5.5/tests/eval_files/async100_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async100_noautofix.py` & `flake8_async-24.5.5/tests/eval_files/async100_noautofix.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async100_simple_autofix.py` & `flake8_async-24.5.5/tests/eval_files/async100_simple_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async101.py` & `flake8_async-24.5.5/tests/eval_files/async101.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async101_asyncio.py` & `flake8_async-24.5.5/tests/eval_files/async101_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async102.py` & `flake8_async-24.5.5/tests/eval_files/async102.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async102_aclose.py` & `flake8_async-24.5.5/tests/eval_files/async102_aclose.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async102_aclose_args.py` & `flake8_async-24.5.5/tests/eval_files/async102_aclose_args.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async102_anyio.py` & `flake8_async-24.5.5/tests/eval_files/async102_anyio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async102_asyncio.py` & `flake8_async-24.5.5/tests/eval_files/async102_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async102_trio.py` & `flake8_async-24.5.5/tests/eval_files/async102_trio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async103.py` & `flake8_async-24.5.5/tests/eval_files/async103.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async103_all_imported.py` & `flake8_async-24.5.5/tests/eval_files/async103_all_imported.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async103_both_imported.py` & `flake8_async-24.5.5/tests/eval_files/async103_both_imported.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async103_trio.py` & `flake8_async-24.5.5/tests/eval_files/async103_trio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async104.py` & `flake8_async-24.5.5/tests/eval_files/async104.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async104_anyio.py` & `flake8_async-24.5.5/tests/eval_files/async104_anyio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async105.py` & `flake8_async-24.5.5/tests/eval_files/async105.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async106.py` & `flake8_async-24.5.5/tests/eval_files/async106.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async109.py` & `flake8_async-24.5.5/tests/eval_files/async109.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async110.py` & `flake8_async-24.5.5/tests/eval_files/async110.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async111.py` & `flake8_async-24.5.5/tests/eval_files/async111.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async111_anyio.py` & `flake8_async-24.5.5/tests/eval_files/async111_anyio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async111_asyncio.py` & `flake8_async-24.5.5/tests/eval_files/async111_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async112.py` & `flake8_async-24.5.5/tests/eval_files/async112.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async112_anyio.py` & `flake8_async-24.5.5/tests/eval_files/async112_anyio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async112_asyncio.py` & `flake8_async-24.5.5/tests/eval_files/async112_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async113.py` & `flake8_async-24.5.5/tests/eval_files/async113.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async113_trio.py` & `flake8_async-24.5.5/tests/eval_files/async113_trio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async114.py` & `flake8_async-24.5.5/tests/eval_files/async114.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async115.py` & `flake8_async-24.5.5/tests/eval_files/async115.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async116.py` & `flake8_async-24.5.5/tests/eval_files/async116.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async118.py` & `flake8_async-24.5.5/tests/eval_files/async118.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async119.py` & `flake8_async-24.5.5/tests/eval_files/async119.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async200.py` & `flake8_async-24.5.5/tests/eval_files/async200.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async210.py` & `flake8_async-24.5.5/tests/eval_files/async210.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async211.py` & `flake8_async-24.5.5/tests/eval_files/async211.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async212.py` & `flake8_async-24.5.5/tests/eval_files/async212.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async22x.py` & `flake8_async-24.5.5/tests/eval_files/async22x.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async22x_asyncio.py` & `flake8_async-24.5.5/tests/eval_files/async22x_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async232.py` & `flake8_async-24.5.5/tests/eval_files/async232.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async232_asyncio.py` & `flake8_async-24.5.5/tests/eval_files/async232_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async23x.py` & `flake8_async-24.5.5/tests/eval_files/async23x.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async23x_asyncio.py` & `flake8_async-24.5.5/tests/eval_files/async23x_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async240.py` & `flake8_async-24.5.5/tests/eval_files/async240.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async900.py` & `flake8_async-24.5.5/tests/eval_files/async900.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async910.py` & `flake8_async-24.5.5/tests/eval_files/async910.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async911.py` & `flake8_async-24.5.5/tests/eval_files/async911.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async912.py` & `flake8_async-24.5.5/tests/eval_files/async912.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async912_asyncio.py` & `flake8_async-24.5.5/tests/eval_files/async912_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async913.py` & `flake8_async-24.5.5/tests/eval_files/async913.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async91x_autofix.py` & `flake8_async-24.5.5/tests/eval_files/async91x_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/async91x_noautofix.py` & `flake8_async-24.5.5/tests/eval_files/async91x_noautofix.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/exception_suppress_context_manager.py` & `flake8_async-24.5.5/tests/eval_files/exception_suppress_context_manager.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/eval_files/noqa.py` & `flake8_async-24.5.5/tests/eval_files/noqa.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/test_all_visitors_imported.py` & `flake8_async-24.5.5/tests/test_all_visitors_imported.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/test_changelog_and_version.py` & `flake8_async-24.5.5/tests/test_changelog_and_version.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/test_config_and_args.py` & `flake8_async-24.5.5/tests/test_config_and_args.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/test_decorator.py` & `flake8_async-24.5.5/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/test_exception_on_invalid_code.py` & `flake8_async-24.5.5/tests/test_exception_on_invalid_code.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tests/test_flake8_async.py` & `flake8_async-24.5.5/tests/test_flake8_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -472,14 +472,15 @@
     "ASYNC106",
     "ASYNC111",
     "ASYNC112",
     "ASYNC115",
     "ASYNC116",
     "ASYNC117",
     "ASYNC118",
+    "ASYNC300",
     "ASYNC912",
 }
 
 
 class SyncTransformer(ast.NodeTransformer):
     def visit_Await(self, node: ast.Await):
         return self.generic_visit(node.value)
```

### Comparing `flake8_async-24.5.4/tests/test_messages_documented.py` & `flake8_async-24.5.5/tests/test_messages_documented.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.4/tox.ini` & `flake8_async-24.5.5/tox.ini`

 * *Files identical despite different names*

