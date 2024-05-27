# Comparing `tmp/flake8_async-24.5.3.tar.gz` & `tmp/flake8_async-24.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_async-24.5.3.tar", last modified: Wed May 22 10:54:56 2024, max compression
+gzip compressed data, was "flake8_async-24.5.4.tar", last modified: Mon May 27 11:34:37 2024, max compression
```

## Comparing `flake8_async-24.5.3.tar` & `flake8_async-24.5.4.tar`

### file list

```diff
@@ -1,129 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:54:56.600402 flake8_async-24.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-22 10:54:47.000000 flake8_async-24.5.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-22 10:54:47.000000 flake8_async-24.5.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-22 10:54:47.000000 flake8_async-24.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-22 10:54:47.000000 flake8_async-24.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-22 10:54:56.600402 flake8_async-24.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-22 10:54:47.000000 flake8_async-24.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:54:56.580402 flake8_async-24.5.3/flake8_async/
--rw-r--r--   0 runner    (1001) docker     (127)    15327 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:54:56.584402 flake8_async-24.5.3/flake8_async/visitors/
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/flake8asyncvisitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15294 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/visitor101.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/visitor102.py
--rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/visitor103_104.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/visitor105.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/visitor111.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/visitor118.py
--rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/visitor2xx.py
--rw-r--r--   0 runner    (1001) docker     (127)    36306 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/visitor91x.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/visitor_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)    12683 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:54:56.600402 flake8_async-24.5.3/flake8_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-22 10:54:56.000000 flake8_async-24.5.3/flake8_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-22 10:54:56.000000 flake8_async-24.5.3/flake8_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:54:56.000000 flake8_async-24.5.3/flake8_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-22 10:54:56.000000 flake8_async-24.5.3/flake8_async.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:54:56.000000 flake8_async-24.5.3/flake8_async.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 10:54:56.000000 flake8_async-24.5.3/flake8_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 10:54:56.000000 flake8_async-24.5.3/flake8_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-22 10:54:47.000000 flake8_async-24.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 10:54:56.600402 flake8_async-24.5.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2204 2024-05-22 10:54:47.000000 flake8_async-24.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:54:56.588402 flake8_async-24.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:54:56.588402 flake8_async-24.5.3/tests/autofix_files/
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/autofix_files/async100.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/autofix_files/async100_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/autofix_files/async100_simple_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)    12002 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/autofix_files/async910.py
--rw-r--r--   0 runner    (1001) docker     (127)    28741 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/autofix_files/async911.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/autofix_files/async91x_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/autofix_files/noqa.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/autofix_files/noqa_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:54:56.600402 flake8_async-24.5.3/tests/eval_files/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/anyio_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async100.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async100_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async100_noautofix.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async100_simple_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async101.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async101_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async101_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async101_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     7082 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async102.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async102_aclose.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async102_aclose_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async102_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async102_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async102_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async103.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async103_all_imported.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async103_both_imported.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async103_no_104.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async103_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async104.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async104_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async104_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async105.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async105_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async106.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async109.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async110.py
--rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async111.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async111_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async111_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async112.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async112_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async112_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async113.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async113_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async113_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async114.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async115.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async116.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async118.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async119.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async200.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async210.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async211.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async212.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async22x.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async22x_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async232.py
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async232_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async23x.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async23x_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async240.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async250.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async250_multi_library.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async251.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async251_multi_library.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async900.py
--rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async910.py
--rw-r--r--   0 runner    (1001) docker     (127)    24009 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async911.py
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async912.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async912_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async91x_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async91x_noautofix.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/no_library.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/noqa.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/noqa_no_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/noqa_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/trio_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/test_all_visitors_imported.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3807 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/test_changelog_and_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12695 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/test_config_and_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/test_exception_on_invalid_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    29840 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/test_flake8_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/test_formatting.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3425 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/test_messages_documented.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/trio_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:34:37.646502 flake8_async-24.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-27 11:34:29.000000 flake8_async-24.5.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-27 11:34:29.000000 flake8_async-24.5.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-27 11:34:29.000000 flake8_async-24.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-27 11:34:29.000000 flake8_async-24.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-27 11:34:37.646502 flake8_async-24.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-27 11:34:29.000000 flake8_async-24.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:34:37.626502 flake8_async-24.5.4/flake8_async/
+-rw-r--r--   0 runner    (1001) docker     (127)    15959 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:34:37.630502 flake8_async-24.5.4/flake8_async/visitors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/flake8asyncvisitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15337 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/visitor101.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/visitor102.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/visitor103_104.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/visitor105.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/visitor111.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/visitor118.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/visitor2xx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40658 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/visitor91x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/visitor_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12683 2024-05-27 11:34:29.000000 flake8_async-24.5.4/flake8_async/visitors/visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:34:37.646502 flake8_async-24.5.4/flake8_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-27 11:34:37.000000 flake8_async-24.5.4/flake8_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-27 11:34:37.000000 flake8_async-24.5.4/flake8_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 11:34:37.000000 flake8_async-24.5.4/flake8_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-27 11:34:37.000000 flake8_async-24.5.4/flake8_async.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 11:34:37.000000 flake8_async-24.5.4/flake8_async.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-27 11:34:37.000000 flake8_async-24.5.4/flake8_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 11:34:37.000000 flake8_async-24.5.4/flake8_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-27 11:34:29.000000 flake8_async-24.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 11:34:37.646502 flake8_async-24.5.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2204 2024-05-27 11:34:29.000000 flake8_async-24.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:34:37.634503 flake8_async-24.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:34:37.634503 flake8_async-24.5.4/tests/autofix_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/async100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/async100_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/async100_simple_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12020 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/async910.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/async910_insert_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28741 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/async911.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/async911_insert_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/async913.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/async91x_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/exception_suppress_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/exception_suppress_context_manager_import_star.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/noqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/autofix_files/noqa_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:34:37.646502 flake8_async-24.5.4/tests/eval_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/anyio_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async100_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async100_noautofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async100_simple_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async101.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async101_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async101_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async101_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7082 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async102.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async102_aclose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async102_aclose_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async102_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async102_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async102_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async103.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async103_all_imported.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async103_both_imported.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async103_no_104.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async103_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async104.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async104_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async104_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async105.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async105_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async106.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async109.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async111.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async111_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async111_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async112.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async112_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async112_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async113.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async113_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async113_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async114.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async115.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async116.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async118.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async119.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async210.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async211.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async212.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async22x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async22x_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async232.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async232_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async23x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async23x_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async240.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async250.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async250_multi_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async251.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async251_multi_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async900.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async910.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async910_insert_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24009 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async911.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async911_insert_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async912.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async912_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async913.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async91x_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/async91x_noautofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/exception_suppress_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/exception_suppress_context_manager_import_star.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/no_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/noqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/noqa_no_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/noqa_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/eval_files/trio_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/test_all_visitors_imported.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3807 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/test_changelog_and_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12695 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/test_config_and_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/test_exception_on_invalid_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29839 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/test_flake8_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/test_formatting.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3425 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/test_messages_documented.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tests/trio_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-27 11:34:29.000000 flake8_async-24.5.4/tox.ini
```

### Comparing `flake8_async-24.5.3/LICENSE` & `flake8_async-24.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/PKG-INFO` & `flake8_async-24.5.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-async
-Version: 24.5.3
+Version: 24.5.4
 Summary: A highly opinionated flake8 plugin for Trio-related problems.
 Author: Zac Hatfield-Dodds, John Litborn, and Contributors
 Author-email: zac@zhd.dev
 License: MIT
 Project-URL: Homepage, https://github.com/python-trio/flake8-async
 Project-URL: Documentation, https://flake8-async.readthedocs.io/
 Project-URL: Changelog, https://flake8-async.readthedocs.io/en/latest/changelog.html
@@ -41,7 +41,10 @@
 It may well be too noisy for anyone with different opinions, that's OK.
 
 Pairs well with flake8-bugbear.
 
 Some checks are incorporated into [ruff](https://github.com/astral-sh/ruff).
 
 This plugin was previously known as flake8-trio, and there was a separate small plugin known as flake8-async for asyncio. But this plugin was a superset of the checks in flake8-async, and support for anyio was added, so it's now named flake8-async to more properly convey its usage. At the same time all error codes were renamed from TRIOxxx to ASYNCxxx, as was previously used by the old flake8-async.
+
+## Rules
+https://flake8-async.readthedocs.io/en/latest/rules.html
```

### Comparing `flake8_async-24.5.3/README.md` & `flake8_async-24.5.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,7 +14,10 @@
 It may well be too noisy for anyone with different opinions, that's OK.
 
 Pairs well with flake8-bugbear.
 
 Some checks are incorporated into [ruff](https://github.com/astral-sh/ruff).
 
 This plugin was previously known as flake8-trio, and there was a separate small plugin known as flake8-async for asyncio. But this plugin was a superset of the checks in flake8-async, and support for anyio was added, so it's now named flake8-async to more properly convey its usage. At the same time all error codes were renamed from TRIOxxx to ASYNCxxx, as was previously used by the old flake8-async.
+
+## Rules
+https://flake8-async.readthedocs.io/en/latest/rules.html
```

### Comparing `flake8_async-24.5.3/flake8_async/__init__.py` & `flake8_async-24.5.4/flake8_async/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     from flake8.options.manager import OptionManager
 
     from .base import Error
 
 
 # CalVer: YY.month.patch, e.g. first release of July 2022 == "22.7.1"
-__version__ = "24.5.3"
+__version__ = "24.5.4"
 
 
 # taken from https://github.com/Zac-HD/shed
 @functools.lru_cache
 def _get_git_repo_root(cwd: str | None = None) -> str:
     return subprocess.run(
         ["git", "rev-parse", "--show-toplevel"],
@@ -258,14 +258,26 @@
                 "checkpoint warnings for. "
                 "Decorators can be dotted or not, as well as support * as a wildcard. "
                 "For example, ``--no-checkpoint-warning-decorators=app.route,"
                 "mydecorator,mypackage.mydecorators.*``"
             ),
         )
         add_argument(
+            "--exception-suppress-context-managers",
+            default="",
+            required=False,
+            type=comma_separated_list,
+            help=(
+                "Comma-separated list of contextmanagers which may suppress exceptions "
+                "without reraising, breaking checkpoint guarantees of ASYNC91x. "
+                "``contextlib.suppress`` will be added to the list. "
+                "Decorators can be dotted or not, as well as support * as a wildcard. "
+            ),
+        )
+        add_argument(
             "--startable-in-context-manager",
             type=parse_async114_identifiers,
             default="",
             required=False,
             help=(
                 "Comma-separated list of method calls to additionally enable ASYNC113 "
                 "warnings for. Will also check for the pattern inside function calls. "
@@ -375,14 +387,15 @@
             options.async200_blocking_calls = options.trio200_blocking_calls
 
         Plugin._options = Options(
             enabled_codes=enabled_codes,
             autofix_codes=autofix_codes,
             error_on_autofix=options.error_on_autofix,
             no_checkpoint_warning_decorators=options.no_checkpoint_warning_decorators,
+            exception_suppress_context_managers=options.exception_suppress_context_managers,
             startable_in_context_manager=options.startable_in_context_manager,
             async200_blocking_calls=options.async200_blocking_calls,
             anyio=options.anyio,
             asyncio=options.asyncio,
             disable_noqa=options.disable_noqa,
         )
```

### Comparing `flake8_async-24.5.3/flake8_async/base.py` & `flake8_async-24.5.4/flake8_async/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     # error codes to give errors for
     enabled_codes: set[str]
     # error codes to autofix
     autofix_codes: set[str]
     # whether to print an error message even when autofixed
     error_on_autofix: bool
     no_checkpoint_warning_decorators: Collection[str]
+    exception_suppress_context_managers: Collection[str]
     startable_in_context_manager: Collection[str]
     async200_blocking_calls: dict[str, str]
     anyio: bool
     asyncio: bool
     disable_noqa: bool
```

### Comparing `flake8_async-24.5.3/flake8_async/runner.py` & `flake8_async-24.5.4/flake8_async/runner.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/flake8_async/visitors/__init__.py` & `flake8_async-24.5.4/flake8_async/visitors/__init__.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/flake8_async/visitors/flake8asyncvisitor.py` & `flake8_async-24.5.4/flake8_async/visitors/flake8asyncvisitor.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/flake8_async/visitors/helpers.py` & `flake8_async-24.5.4/flake8_async/visitors/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,16 @@
             # strip leading "@"s for when we're working with decorators
             if fnmatch(qualified_name, pattern.lstrip("@")):
                 return pattern
     return None
 
 
 def fnmatch_qualified_name_cst(
-    name_list: Iterable[cst.Decorator], *patterns: str
+    name_list: Iterable[cst.Decorator | cst.Call | cst.Attribute | cst.Name],
+    *patterns: str,
 ) -> str | None:
     for name in name_list:
         qualified_name = get_full_name_for_node_or_raise(name)
 
         for pattern in patterns:
             # strip leading "@"s for when we're working with decorators
             if fnmatch(qualified_name, pattern.lstrip("@")):
```

### Comparing `flake8_async-24.5.3/flake8_async/visitors/visitor101.py` & `flake8_async-24.5.4/flake8_async/visitors/visitor101.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/flake8_async/visitors/visitor102.py` & `flake8_async-24.5.4/flake8_async/visitors/visitor102.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/flake8_async/visitors/visitor103_104.py` & `flake8_async-24.5.4/flake8_async/visitors/visitor103_104.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/flake8_async/visitors/visitor105.py` & `flake8_async-24.5.4/flake8_async/visitors/visitor105.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/flake8_async/visitors/visitor111.py` & `flake8_async-24.5.4/flake8_async/visitors/visitor111.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/flake8_async/visitors/visitor118.py` & `flake8_async-24.5.4/flake8_async/visitors/visitor118.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/flake8_async/visitors/visitor2xx.py` & `flake8_async-24.5.4/flake8_async/visitors/visitor2xx.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/flake8_async/visitors/visitor91x.py` & `flake8_async-24.5.4/flake8_async/visitors/visitor91x.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 each yield.
 """
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, cast
 
 import libcst as cst
 import libcst.matchers as m
 from libcst.metadata import PositionProvider
 
 from ..base import Statement
 from .flake8asyncvisitor import Flake8AsyncVisitor_cst
@@ -69,16 +69,16 @@
     body_guaranteed_once: bool = False
     has_break: bool = False
 
     uncheckpointed_before_continue: set[Statement] = field(default_factory=set)
     uncheckpointed_before_break: set[Statement] = field(default_factory=set)
 
     artificial_errors: set[cst.Return | cst.Yield] = field(default_factory=set)
-    nodes_needing_checkpoints: list[cst.Return | cst.Yield] = field(
-        default_factory=list
+    nodes_needing_checkpoints: list[cst.Return | cst.Yield | ArtificialStatement] = (
+        field(default_factory=list)
     )
 
     def copy(self):
         return LoopState(
             infinite_loop=self.infinite_loop,
             body_guaranteed_once=self.body_guaranteed_once,
             has_break=self.has_break,
@@ -211,16 +211,18 @@
     Called from `leave_While` and `leave_For` in Visitor91X.
     """
 
     def __init__(
         self,
         nodes_needing_checkpoint: Sequence[cst.Yield | cst.Return],
         library: tuple[str, ...],
+        explicitly_imported: dict[str, bool],
     ):
         super().__init__()
+        self.explicitly_imported_library = explicitly_imported
         self.nodes_needing_checkpoint = nodes_needing_checkpoint
         self.__library = library
 
     @property
     def library(self) -> tuple[str, ...]:
         return self.__library if self.__library else ("trio",)
 
@@ -258,14 +260,15 @@
             "{0} from async iterable with no guaranteed checkpoint since {1.name} "
             "on line {1.lineno}."
         ),
         "ASYNC912": (
             "CancelScope with no guaranteed checkpoint. This makes it potentially "
             "impossible to cancel."
         ),
+        "ASYNC913": ("Indefinite loop with no guaranteed checkpoint."),
         "ASYNC100": (
             "{0}.{1} context contains no checkpoints, remove the context or add"
             " `await {0}.lowlevel.checkpoint()`."
         ),
     }
 
     def __init__(self, *args: Any, **kwargs: Any):
@@ -279,14 +282,17 @@
         self.loop_state = LoopState()
         self.try_state = TryState()
 
         # ASYNC100
         self.has_checkpoint_stack: list[bool] = []
         self.node_dict: dict[cst.With, list[AttributeCall]] = {}
 
+        # --exception-suppress-context-manager
+        self.suppress_imported_as: list[str] = []
+
     def should_autofix(self, node: cst.CSTNode, code: str | None = None) -> bool:
         if code is None:  # pragma: no branch
             code = "ASYNC911" if self.has_yield else "ASYNC910"
 
         return (
             not self.noautofix
             and super().should_autofix(node, code)
@@ -296,14 +302,36 @@
     def checkpoint(self) -> None:
         self.uncheckpointed_statements = set()
         self.has_checkpoint_stack = [True] * len(self.has_checkpoint_stack)
 
     def checkpoint_statement(self) -> cst.SimpleStatementLine:
         return checkpoint_statement(self.library[0])
 
+    def visit_ImportFrom(self, node: cst.ImportFrom) -> None:
+        # Semi-crude approach to handle `from contextlib import suppress`.
+        # It does not handle the identifier being overridden, or assigned
+        # to other idefintifers. Function scoping is handled though.
+        # The "proper" way would be to add a cst version of
+        # visitor_utility.VisitorTypeTracker, and expand that to handle imports.
+        if isinstance(node.module, cst.Name) and node.module.value == "contextlib":
+            # handle `from contextlib import *`
+            if isinstance(node.names, cst.ImportStar):
+                self.suppress_imported_as.append("suppress")
+                return
+            for alias in node.names:
+                if alias.name.value == "suppress":
+                    if alias.asname is not None:
+                        # `libcst.AsName` is incorrectly typed
+                        # https://github.com/Instagram/LibCST/issues/503
+                        assert isinstance(alias.asname.name, cst.Name)
+                        self.suppress_imported_as.append(alias.asname.name.value)
+                    else:
+                        self.suppress_imported_as.append("suppress")
+                    return
+
     def visit_FunctionDef(self, node: cst.FunctionDef) -> bool:
         # don't lint functions whose bodies solely consist of pass or ellipsis
         # @overload functions are also guaranteed to be empty
         # we also ignore pytest fixtures
         if func_has_decorator(node, "overload", "fixture") or func_empty_body(node):
             return False  # subnodes can be ignored
 
@@ -312,14 +340,15 @@
             "has_yield",
             "safe_decorator",
             "async_function",
             "uncheckpointed_statements",
             "loop_state",
             "try_state",
             "has_checkpoint_stack",
+            "suppress_imported_as",
             copy=True,
         )
         self.uncheckpointed_statements = set()
         self.has_checkpoint_stack = []
         self.has_yield = self.safe_decorator = False
         self.loop_state = LoopState()
 
@@ -352,14 +381,16 @@
         ):
             # insert checkpoint at the end of body
             new_body = list(updated_node.body.body)
             new_body.append(self.checkpoint_statement())
             indentedblock = updated_node.body.with_changes(body=new_body)
             updated_node = updated_node.with_changes(body=indentedblock)
 
+            self.ensure_imported_library()
+
         self.restore_state(original_node)
         return updated_node
 
     # error if function exit/return/yields with uncheckpointed statements
     # returns a bool indicating if any real (i.e. not artificial) errors were raised
     # so caller can insert checkpoint before statement (if yield/return) or at end
     # of body (functiondef)
@@ -445,20 +476,37 @@
         self.checkpoint()
         return updated_node
 
     # raising exception means we don't need to checkpoint so we can treat it as one
     # can't use TypeVar due to libcst's built-in type checking not supporting it
     leave_Raise = leave_Await  # type: ignore
 
+    def _is_exception_suppressing_context_manager(self, node: cst.With) -> bool:
+        return (
+            fnmatch_qualified_name_cst(
+                (x.item for x in node.items if isinstance(x.item, cst.Call)),
+                "contextlib.suppress",
+                *self.suppress_imported_as,
+                *self.options.exception_suppress_context_managers,
+            )
+            is not None
+        )
+
     # Async context managers can reasonably checkpoint on either or both of entry and
     # exit.  Given that we can't tell which, we assume "both" to avoid raising a
     # missing-checkpoint warning when there might in fact be one (i.e. a false alarm).
     def visit_With_body(self, node: cst.With):
         if getattr(node, "asynchronous", None):
             self.checkpoint()
+
+        # if this might suppress exceptions, we cannot treat anything inside it as
+        # checkpointing.
+        if self._is_exception_suppressing_context_manager(node):
+            self.save_state(node, "uncheckpointed_statements", copy=True)
+
         if res := (
             with_has_call(node, *cancel_scope_names)
             or with_has_call(
                 node, "timeout", "timeout_at", base=("asyncio", "asyncio.timeouts")
             )
         ):
             pos = self.get_metadata(PositionProvider, node).start  # pyright: ignore
@@ -495,14 +543,22 @@
             line: int = pos.line  # pyright: ignore
             column: int = pos.column  # pyright: ignore
             s = ArtificialStatement("with", line, column)
             if s in self.uncheckpointed_statements:
                 self.uncheckpointed_statements.remove(s)
                 for res in self.node_dict[original_node]:
                     self.error(res.node, error_code="ASYNC912")
+
+        # if exception-suppressing, restore all uncheckpointed statements from
+        # before the `with`.
+        if self._is_exception_suppressing_context_manager(original_node):
+            prev_checkpoints = self.uncheckpointed_statements
+            self.restore_state(original_node)
+            self.uncheckpointed_statements.update(prev_checkpoints)
+
         if getattr(original_node, "asynchronous", None):
             self.checkpoint()
         return updated_node
 
     # error if no checkpoint since earlier yield or function entry
     def leave_Yield(
         self, original_node: cst.Yield, updated_node: cst.Yield
@@ -717,14 +773,26 @@
                 any_error |= self.error_91x(err_node, stmt)
 
         # if there's no errors from artificial statements, we don't need to insert
         # the potential checkpoints
         if not any_error:
             self.loop_state.nodes_needing_checkpoints = []
 
+        if (
+            self.loop_state.infinite_loop
+            and not self.loop_state.has_break
+            and ARTIFICIAL_STATEMENT in self.uncheckpointed_statements
+            and self.error(node, error_code="ASYNC913")
+        ):
+            # We can override nodes_needing_checkpoints, as that's solely for checkpoints
+            # that error because of the artificial statement injected at the start of
+            # the loop. When inserting a checkpoint at the start of the loop, those
+            # will be remedied
+            self.loop_state.nodes_needing_checkpoints = [ARTIFICIAL_STATEMENT]
+
         # replace artificial statements in else with prebody uncheckpointed statements
         # non-artificial stmts before continue/break/at body end will already be in them
         for stmts in (
             self.loop_state.uncheckpointed_before_continue,
             self.loop_state.uncheckpointed_before_break,
             self.uncheckpointed_statements,
         ):
@@ -777,23 +845,46 @@
         self, original_node: cst.For | cst.While, updated_node: cst.For | cst.While
     ) -> (
         cst.While
         | cst.For
         | cst.FlattenSentinel[cst.For | cst.While]
         | cst.RemovalSentinel
     ):
-        if self.loop_state.nodes_needing_checkpoints:
+        # don't bother autofixing same-line loops
+        if isinstance(updated_node.body, cst.SimpleStatementSuite):
+            self.restore_state(original_node)
+            return updated_node
+
+        # ASYNC913, indefinite loop with no guaranteed checkpoint
+        if self.loop_state.nodes_needing_checkpoints == [ARTIFICIAL_STATEMENT]:
+            if self.should_autofix(original_node, code="ASYNC913"):
+                # insert checkpoint at start of body
+                new_body = list(updated_node.body.body)
+                new_body.insert(0, self.checkpoint_statement())
+                indentedblock = updated_node.body.with_changes(body=new_body)
+                updated_node = updated_node.with_changes(body=indentedblock)
+
+                self.ensure_imported_library()
+        elif self.loop_state.nodes_needing_checkpoints:
+            assert ARTIFICIAL_STATEMENT not in self.loop_state.nodes_needing_checkpoints
             transformer = InsertCheckpointsInLoopBody(
-                self.loop_state.nodes_needing_checkpoints, self.library
+                cast(
+                    "list[cst.Yield | cst.Return]",
+                    self.loop_state.nodes_needing_checkpoints,
+                ),
+                self.library,
+                self.explicitly_imported_library,
             )
             # type of updated_node expanded to the return type
             updated_node = updated_node.visit(transformer)  # type: ignore
 
+            # include any necessary import added
+            self.add_import.update(transformer.add_import)
+
         self.restore_state(original_node)
-        # https://github.com/afonasev/flake8-return/issues/133
         return updated_node
 
     leave_For = leave_While
 
     # save state in case of continue/break at a point not guaranteed to checkpoint
     def visit_Continue(self, node: cst.Continue):
         if not self.async_function:
```

### Comparing `flake8_async-24.5.3/flake8_async/visitors/visitor_utility.py` & `flake8_async-24.5.4/flake8_async/visitors/visitor_utility.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/flake8_async/visitors/visitors.py` & `flake8_async-24.5.4/flake8_async/visitors/visitors.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/flake8_async.egg-info/PKG-INFO` & `flake8_async-24.5.4/flake8_async.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-async
-Version: 24.5.3
+Version: 24.5.4
 Summary: A highly opinionated flake8 plugin for Trio-related problems.
 Author: Zac Hatfield-Dodds, John Litborn, and Contributors
 Author-email: zac@zhd.dev
 License: MIT
 Project-URL: Homepage, https://github.com/python-trio/flake8-async
 Project-URL: Documentation, https://flake8-async.readthedocs.io/
 Project-URL: Changelog, https://flake8-async.readthedocs.io/en/latest/changelog.html
@@ -41,7 +41,10 @@
 It may well be too noisy for anyone with different opinions, that's OK.
 
 Pairs well with flake8-bugbear.
 
 Some checks are incorporated into [ruff](https://github.com/astral-sh/ruff).
 
 This plugin was previously known as flake8-trio, and there was a separate small plugin known as flake8-async for asyncio. But this plugin was a superset of the checks in flake8-async, and support for anyio was added, so it's now named flake8-async to more properly convey its usage. At the same time all error codes were renamed from TRIOxxx to ASYNCxxx, as was previously used by the old flake8-async.
+
+## Rules
+https://flake8-async.readthedocs.io/en/latest/rules.html
```

### Comparing `flake8_async-24.5.3/flake8_async.egg-info/SOURCES.txt` & `flake8_async-24.5.4/flake8_async.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -41,16 +41,21 @@
 tests/test_formatting.py
 tests/test_messages_documented.py
 tests/trio_options.py
 tests/autofix_files/async100.py
 tests/autofix_files/async100_asyncio.py
 tests/autofix_files/async100_simple_autofix.py
 tests/autofix_files/async910.py
+tests/autofix_files/async910_insert_library.py
 tests/autofix_files/async911.py
+tests/autofix_files/async911_insert_library.py
+tests/autofix_files/async913.py
 tests/autofix_files/async91x_autofix.py
+tests/autofix_files/exception_suppress_context_manager.py
+tests/autofix_files/exception_suppress_context_manager_import_star.py
 tests/autofix_files/noqa.py
 tests/autofix_files/noqa_testing.py
 tests/eval_files/anyio_trio.py
 tests/eval_files/async100.py
 tests/eval_files/async100_asyncio.py
 tests/eval_files/async100_noautofix.py
 tests/eval_files/async100_simple_autofix.py
@@ -104,17 +109,22 @@
 tests/eval_files/async240.py
 tests/eval_files/async250.py
 tests/eval_files/async250_multi_library.py
 tests/eval_files/async251.py
 tests/eval_files/async251_multi_library.py
 tests/eval_files/async900.py
 tests/eval_files/async910.py
+tests/eval_files/async910_insert_library.py
 tests/eval_files/async911.py
+tests/eval_files/async911_insert_library.py
 tests/eval_files/async912.py
 tests/eval_files/async912_asyncio.py
+tests/eval_files/async913.py
 tests/eval_files/async91x_autofix.py
 tests/eval_files/async91x_noautofix.py
+tests/eval_files/exception_suppress_context_manager.py
+tests/eval_files/exception_suppress_context_manager_import_star.py
 tests/eval_files/no_library.py
 tests/eval_files/noqa.py
 tests/eval_files/noqa_no_autofix.py
 tests/eval_files/noqa_testing.py
 tests/eval_files/trio_anyio.py
```

### Comparing `flake8_async-24.5.3/pyproject.toml` & `flake8_async-24.5.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,28 @@
 ignore-init-module-imports = true
 in-place = true
 quiet = true
 remove-all-unused-imports = true
 remove-duplicate-keys = true
 remove-unused-variables = true
 
+[tool.black]
+# need to use force-exclude since pre-commit directly specifies files
+force-exclude = "tests/autofix_files/.*.py"
+
 [tool.codespell]
 ignore-words-list = 'spawnve'
 
 [tool.isort]
 only_modified = true
 profile = "black"
 py_version = "311"
 quiet = true
 skip_gitignore = true
-skip_glob = "tests/eval_files/*"
+skip_glob = "tests/*_files/*"
 
 [tool.mypy]
 check_untyped_defs = true
 disable_error_code = ["no-untyped-def", "misc", "no-untyped-call", "no-any-return"]
 python_version = "3.9"
 strict = true
 warn_unreachable = true
```

### Comparing `flake8_async-24.5.3/setup.py` & `flake8_async-24.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/autofix_files/async100.py` & `flake8_async-24.5.4/tests/autofix_files/async100.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/autofix_files/async100_simple_autofix.py` & `flake8_async-24.5.4/tests/autofix_files/async100_simple_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/autofix_files/async910.py` & `flake8_async-24.5.4/tests/autofix_files/async910.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # AUTOFIX
 # ASYNCIO_NO_AUTOFIX
 # mypy: disable-error-code="unreachable"
 from __future__ import annotations
 
+import contextlib
 import typing
 from typing import Any, overload
 
 import pytest
 import trio
 
 _ = ""
```

### Comparing `flake8_async-24.5.3/tests/autofix_files/async911.py` & `flake8_async-24.5.4/tests/autofix_files/async911.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/autofix_files/async91x_autofix.py` & `flake8_async-24.5.4/tests/autofix_files/async91x_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/autofix_files/noqa.py` & `flake8_async-24.5.4/tests/autofix_files/noqa.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/conftest.py` & `flake8_async-24.5.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async100.py` & `flake8_async-24.5.4/tests/eval_files/async100.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async100_asyncio.py` & `flake8_async-24.5.4/tests/eval_files/async100_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async100_noautofix.py` & `flake8_async-24.5.4/tests/eval_files/async100_noautofix.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async100_simple_autofix.py` & `flake8_async-24.5.4/tests/eval_files/async100_simple_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async101.py` & `flake8_async-24.5.4/tests/eval_files/async101.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async101_asyncio.py` & `flake8_async-24.5.4/tests/eval_files/async101_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async102.py` & `flake8_async-24.5.4/tests/eval_files/async102.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async102_aclose.py` & `flake8_async-24.5.4/tests/eval_files/async102_aclose.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async102_aclose_args.py` & `flake8_async-24.5.4/tests/eval_files/async102_aclose_args.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async102_anyio.py` & `flake8_async-24.5.4/tests/eval_files/async102_anyio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async102_asyncio.py` & `flake8_async-24.5.4/tests/eval_files/async102_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async102_trio.py` & `flake8_async-24.5.4/tests/eval_files/async102_trio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async103.py` & `flake8_async-24.5.4/tests/eval_files/async103.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async103_all_imported.py` & `flake8_async-24.5.4/tests/eval_files/async103_all_imported.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async103_both_imported.py` & `flake8_async-24.5.4/tests/eval_files/async103_both_imported.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async103_trio.py` & `flake8_async-24.5.4/tests/eval_files/async103_trio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async104.py` & `flake8_async-24.5.4/tests/eval_files/async104.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async104_anyio.py` & `flake8_async-24.5.4/tests/eval_files/async104_anyio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async105.py` & `flake8_async-24.5.4/tests/eval_files/async105.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async106.py` & `flake8_async-24.5.4/tests/eval_files/async106.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async109.py` & `flake8_async-24.5.4/tests/eval_files/async109.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async110.py` & `flake8_async-24.5.4/tests/eval_files/async110.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async111.py` & `flake8_async-24.5.4/tests/eval_files/async111.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async111_anyio.py` & `flake8_async-24.5.4/tests/eval_files/async111_anyio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async111_asyncio.py` & `flake8_async-24.5.4/tests/eval_files/async111_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async112.py` & `flake8_async-24.5.4/tests/eval_files/async112.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async112_anyio.py` & `flake8_async-24.5.4/tests/eval_files/async112_anyio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async112_asyncio.py` & `flake8_async-24.5.4/tests/eval_files/async112_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async113.py` & `flake8_async-24.5.4/tests/eval_files/async113.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async113_trio.py` & `flake8_async-24.5.4/tests/eval_files/async113_trio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async114.py` & `flake8_async-24.5.4/tests/eval_files/async114.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async115.py` & `flake8_async-24.5.4/tests/eval_files/async115.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async116.py` & `flake8_async-24.5.4/tests/eval_files/async116.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async118.py` & `flake8_async-24.5.4/tests/eval_files/async118.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async119.py` & `flake8_async-24.5.4/tests/eval_files/async119.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async200.py` & `flake8_async-24.5.4/tests/eval_files/async200.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async210.py` & `flake8_async-24.5.4/tests/eval_files/async210.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async211.py` & `flake8_async-24.5.4/tests/eval_files/async211.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async212.py` & `flake8_async-24.5.4/tests/eval_files/async212.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async22x.py` & `flake8_async-24.5.4/tests/eval_files/async22x.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async22x_asyncio.py` & `flake8_async-24.5.4/tests/eval_files/async22x_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async232.py` & `flake8_async-24.5.4/tests/eval_files/async232.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async232_asyncio.py` & `flake8_async-24.5.4/tests/eval_files/async232_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async23x.py` & `flake8_async-24.5.4/tests/eval_files/async23x.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async23x_asyncio.py` & `flake8_async-24.5.4/tests/eval_files/async23x_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async240.py` & `flake8_async-24.5.4/tests/eval_files/async240.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async900.py` & `flake8_async-24.5.4/tests/eval_files/async900.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async910.py` & `flake8_async-24.5.4/tests/eval_files/async910.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # AUTOFIX
 # ASYNCIO_NO_AUTOFIX
 # mypy: disable-error-code="unreachable"
 from __future__ import annotations
 
+import contextlib
 import typing
 from typing import Any, overload
 
 import pytest
 import trio
 
 _ = ""
```

### Comparing `flake8_async-24.5.3/tests/eval_files/async911.py` & `flake8_async-24.5.4/tests/eval_files/async911.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async912.py` & `flake8_async-24.5.4/tests/eval_files/async912.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # asyncio is tested in async912_asyncio. Cancelscopes in anyio are named the same
 # as in trio, so they're also tested with this file.
 
 # ASYNC100 has autofixes, but ASYNC912 does not. This leaves us with the option
 # of not testing both in the same file, or running with NOAUTOFIX.
 # NOAUTOFIX
 
+import contextlib
 from typing import TypeVar
 
 import trio
 
 
 def bar() -> bool:
     return False
@@ -125,15 +126,15 @@
         ...
     # but saving with `as` does
     with trio.fail_at(10) as res:  # ASYNC912: 9
         if bar():
             await trio.lowlevel.checkpoint()
 
 
-# TODO: issue #240
+# This is handled by ASYNC913, which will raise an error about the loop.
 async def livelocks():
     with trio.move_on_after(0.1):  # should error
         while True:
             try:
                 await trio.sleep("1")  # type: ignore
             except TypeError:
                 pass
@@ -148,24 +149,30 @@
         while condition():
             try:
                 await trio.sleep("1")  # type: ignore
             except TypeError:
                 pass
 
 
-# TODO: add --async912-context-managers=
+# TODO: no-guaranteed-checkpoint-in-infinite-loop
+# https://github.com/python-trio/flake8-async/issues/240
 async def livelocks_3():
-    import contextlib
-
     with trio.move_on_after(0.1):  # should error
         while True:
             with contextlib.suppress(TypeError):
                 await trio.sleep("1")  # type: ignore
 
 
+async def livelocks_4():
+    with trio.move_on_after(0.1):  # ASYNC912: 9
+        while condition():
+            with contextlib.suppress(TypeError):
+                await trio.sleep("1")  # type: ignore
+
+
 # raises an error...?
 with trio.move_on_after(10):  # ASYNC100: 5, "trio", "move_on_after"
     ...
 
 
 # completely sync function ... is this something we care about?
 def sync_func():
```

### Comparing `flake8_async-24.5.3/tests/eval_files/async912_asyncio.py` & `flake8_async-24.5.4/tests/eval_files/async912_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async91x_autofix.py` & `flake8_async-24.5.4/tests/eval_files/async91x_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/eval_files/async91x_noautofix.py` & `flake8_async-24.5.4/tests/eval_files/async91x_noautofix.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ARG --enable=ASYNC910,ASYNC911
+# ARG --enable=ASYNC910,ASYNC911,ASYNC913
 from typing import Any
 
 
 def condition() -> Any: ...
 
 
 async def foo() -> Any:
@@ -68,7 +68,27 @@
     _ = (
         await foo()
         and (yield)
         and await foo()
         and (yield)  # ASYNC911: 13, "yield", Stmt("yield", line-2, 13)
     )
     await foo()
+
+
+async def foo_sameline_913():
+    # fmt: off
+    while True: ...  # ASYNC913: 4
+    # fmt: on
+
+
+# this previously caused a crash
+async def foo_sameline_911():
+    await foo()
+    # fmt: off
+    while True: yield  # ASYNC911: 16, "yield", Stmt("yield", lineno)
+    # fmt: on
+
+
+# this was guarded by an isinstance check though
+# fmt: off
+async def foo_sameline_910(): print()  # ASYNC910: 0, "exit", Stmt("function definition", line)
+# fmt: on
```

### Comparing `flake8_async-24.5.3/tests/eval_files/noqa.py` & `flake8_async-24.5.4/tests/eval_files/noqa.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/test_all_visitors_imported.py` & `flake8_async-24.5.4/tests/test_all_visitors_imported.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/test_changelog_and_version.py` & `flake8_async-24.5.4/tests/test_changelog_and_version.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/test_config_and_args.py` & `flake8_async-24.5.4/tests/test_config_and_args.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/test_decorator.py` & `flake8_async-24.5.4/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/test_exception_on_invalid_code.py` & `flake8_async-24.5.4/tests/test_exception_on_invalid_code.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tests/test_flake8_async.py` & `flake8_async-24.5.4/tests/test_flake8_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,15 +436,15 @@
             message = error_class.error_codes[err_code + alt_code]
             try:
                 expected.append(Error(err_code, lineno, int(col), message, *args))
             except AttributeError as e:
                 msg = f"Line {lineno}: Failed to format\n {message!r}\nwith\n{args}"
                 raise ParseError(msg) from e
 
-    assert enabled_codes, "no codes enabled. Fix file name or add `# ARGS --enable=...`"
+    assert enabled_codes, "no codes enabled. Fix file name or add `# ARG --enable=...`"
     enabled_codes_list = enabled_codes.split(",")
     for code in enabled_codes_list:
         assert re.fullmatch(
             r"ASYNC\d\d\d", code
         ), f"invalid code {code} in list {enabled_codes_list}"
 
     for error in expected:
```

### Comparing `flake8_async-24.5.3/tests/test_messages_documented.py` & `flake8_async-24.5.4/tests/test_messages_documented.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.3/tox.ini` & `flake8_async-24.5.4/tox.ini`

 * *Files identical despite different names*

