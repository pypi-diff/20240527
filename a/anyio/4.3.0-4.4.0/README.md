# Comparing `tmp/anyio-4.3.0.tar.gz` & `tmp/anyio-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyio-4.3.0.tar", last modified: Mon Feb 19 08:35:45 2024, max compression
+gzip compressed data, was "anyio-4.4.0.tar", last modified: Sun May 26 22:01:39 2024, max compression
```

## Comparing `anyio-4.3.0.tar` & `anyio-4.4.0.tar`

### file list

```diff
@@ -1,114 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:35:45.028421 anyio-4.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:35:45.008421 anyio-4.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:35:45.008421 anyio-4.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-02-19 08:35:33.000000 anyio-4.3.0/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-19 08:35:33.000000 anyio-4.3.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-02-19 08:35:33.000000 anyio-4.3.0/.github/ISSUE_TEMPLATE/features_request.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:35:45.008421 anyio-4.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-02-19 08:35:33.000000 anyio-4.3.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-02-19 08:35:33.000000 anyio-4.3.0/.github/workflows/test-downstream.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-02-19 08:35:33.000000 anyio-4.3.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-19 08:35:33.000000 anyio-4.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-02-19 08:35:33.000000 anyio-4.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-19 08:35:33.000000 anyio-4.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-02-19 08:35:33.000000 anyio-4.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-02-19 08:35:45.028421 anyio-4.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-02-19 08:35:33.000000 anyio-4.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:35:45.012421 anyio-4.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-02-19 08:35:33.000000 anyio-4.3.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-02-19 08:35:33.000000 anyio-4.3.0/docs/basics.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-02-19 08:35:33.000000 anyio-4.3.0/docs/cancellation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-02-19 08:35:33.000000 anyio-4.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-02-19 08:35:33.000000 anyio-4.3.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-02-19 08:35:33.000000 anyio-4.3.0/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-02-19 08:35:33.000000 anyio-4.3.0/docs/fileio.rst
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-02-19 08:35:33.000000 anyio-4.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10688 2024-02-19 08:35:33.000000 anyio-4.3.0/docs/migration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-02-19 08:35:33.000000 anyio-4.3.0/docs/networking.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-02-19 08:35:33.000000 anyio-4.3.0/docs/signals.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12714 2024-02-19 08:35:33.000000 anyio-4.3.0/docs/streams.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-02-19 08:35:33.000000 anyio-4.3.0/docs/subprocesses.rst
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-02-19 08:35:33.000000 anyio-4.3.0/docs/support.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-02-19 08:35:33.000000 anyio-4.3.0/docs/synchronization.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-02-19 08:35:33.000000 anyio-4.3.0/docs/tasks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-02-19 08:35:33.000000 anyio-4.3.0/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-02-19 08:35:33.000000 anyio-4.3.0/docs/threads.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-02-19 08:35:33.000000 anyio-4.3.0/docs/typedattrs.rst
--rw-r--r--   0 runner    (1001) docker     (127)    43911 2024-02-19 08:35:33.000000 anyio-4.3.0/docs/versionhistory.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-02-19 08:35:33.000000 anyio-4.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 08:35:45.028421 anyio-4.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:35:45.008421 anyio-4.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:35:45.016421 anyio-4.3.0/src/anyio/
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:35:45.016421 anyio-4.3.0/src/anyio/_backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    81968 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/_backends/_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)    35642 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/_backends/_trio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:35:45.020421 anyio-4.3.0/src/anyio/_core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/_core/_eventloop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/_core/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19512 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/_core/_fileio.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/_core/_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/_core/_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)    24048 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/_core/_sockets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/_core/_streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/_core/_subprocesses.py
--rw-r--r--   0 runner    (1001) docker     (127)    18444 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/_core/_synchronization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/_core/_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/_core/_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/_core/_typedattr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:35:45.020421 anyio-4.3.0/src/anyio/abc/
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/abc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10097 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/abc/_eventloop.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/abc/_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/abc/_sockets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/abc/_streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/abc/_subprocesses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/abc/_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/abc/_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)    15749 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/from_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/lowlevel.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/pytest_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:35:45.024421 anyio-4.3.0/src/anyio/streams/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/streams/buffered.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/streams/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/streams/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/streams/stapled.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/streams/text.py
--rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/streams/tls.py
--rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/to_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-02-19 08:35:33.000000 anyio-4.3.0/src/anyio/to_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:35:45.028421 anyio-4.3.0/src/anyio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-02-19 08:35:44.000000 anyio-4.3.0/src/anyio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-02-19 08:35:45.000000 anyio-4.3.0/src/anyio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 08:35:44.000000 anyio-4.3.0/src/anyio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-19 08:35:44.000000 anyio-4.3.0/src/anyio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-02-19 08:35:44.000000 anyio-4.3.0/src/anyio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-19 08:35:44.000000 anyio-4.3.0/src/anyio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:35:45.024421 anyio-4.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 08:35:33.000000 anyio-4.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-02-19 08:35:33.000000 anyio-4.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:35:45.028421 anyio-4.3.0/tests/streams/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 08:35:33.000000 anyio-4.3.0/tests/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-02-19 08:35:33.000000 anyio-4.3.0/tests/streams/test_buffered.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-02-19 08:35:33.000000 anyio-4.3.0/tests/streams/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-02-19 08:35:33.000000 anyio-4.3.0/tests/streams/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-02-19 08:35:33.000000 anyio-4.3.0/tests/streams/test_stapled.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-02-19 08:35:33.000000 anyio-4.3.0/tests/streams/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)    18742 2024-02-19 08:35:33.000000 anyio-4.3.0/tests/streams/test_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-02-19 08:35:33.000000 anyio-4.3.0/tests/test_debugging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-02-19 08:35:33.000000 anyio-4.3.0/tests/test_eventloop.py
--rw-r--r--   0 runner    (1001) docker     (127)    20553 2024-02-19 08:35:33.000000 anyio-4.3.0/tests/test_fileio.py
--rw-r--r--   0 runner    (1001) docker     (127)    23046 2024-02-19 08:35:33.000000 anyio-4.3.0/tests/test_from_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-02-19 08:35:33.000000 anyio-4.3.0/tests/test_lowlevel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11168 2024-02-19 08:35:33.000000 anyio-4.3.0/tests/test_pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-02-19 08:35:33.000000 anyio-4.3.0/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)    65645 2024-02-19 08:35:33.000000 anyio-4.3.0/tests/test_sockets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-02-19 08:35:33.000000 anyio-4.3.0/tests/test_subprocesses.py
--rw-r--r--   0 runner    (1001) docker     (127)    22197 2024-02-19 08:35:33.000000 anyio-4.3.0/tests/test_synchronization.py
--rw-r--r--   0 runner    (1001) docker     (127)    40288 2024-02-19 08:35:33.000000 anyio-4.3.0/tests/test_taskgroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-02-19 08:35:33.000000 anyio-4.3.0/tests/test_to_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-02-19 08:35:33.000000 anyio-4.3.0/tests/test_to_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:01:39.344221 anyio-4.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:01:39.324221 anyio-4.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:01:39.328221 anyio-4.4.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-26 22:01:34.000000 anyio-4.4.0/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-26 22:01:34.000000 anyio-4.4.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-26 22:01:34.000000 anyio-4.4.0/.github/ISSUE_TEMPLATE/features_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-26 22:01:34.000000 anyio-4.4.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:01:39.328221 anyio-4.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-26 22:01:34.000000 anyio-4.4.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-26 22:01:34.000000 anyio-4.4.0/.github/workflows/test-downstream.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-26 22:01:34.000000 anyio-4.4.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-26 22:01:34.000000 anyio-4.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-26 22:01:34.000000 anyio-4.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-26 22:01:34.000000 anyio-4.4.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-26 22:01:34.000000 anyio-4.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-26 22:01:39.344221 anyio-4.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-26 22:01:34.000000 anyio-4.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:01:39.332221 anyio-4.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-05-26 22:01:34.000000 anyio-4.4.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-26 22:01:34.000000 anyio-4.4.0/docs/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-05-26 22:01:34.000000 anyio-4.4.0/docs/cancellation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-26 22:01:34.000000 anyio-4.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-26 22:01:34.000000 anyio-4.4.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-26 22:01:34.000000 anyio-4.4.0/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-26 22:01:34.000000 anyio-4.4.0/docs/fileio.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-26 22:01:34.000000 anyio-4.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10688 2024-05-26 22:01:34.000000 anyio-4.4.0/docs/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-05-26 22:01:34.000000 anyio-4.4.0/docs/networking.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-26 22:01:34.000000 anyio-4.4.0/docs/signals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12710 2024-05-26 22:01:34.000000 anyio-4.4.0/docs/streams.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-26 22:01:34.000000 anyio-4.4.0/docs/subprocesses.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-26 22:01:34.000000 anyio-4.4.0/docs/support.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-26 22:01:34.000000 anyio-4.4.0/docs/synchronization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-05-26 22:01:34.000000 anyio-4.4.0/docs/tasks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-05-26 22:01:34.000000 anyio-4.4.0/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-05-26 22:01:34.000000 anyio-4.4.0/docs/threads.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-26 22:01:34.000000 anyio-4.4.0/docs/typedattrs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    46865 2024-05-26 22:01:34.000000 anyio-4.4.0/docs/versionhistory.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-26 22:01:34.000000 anyio-4.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 22:01:39.344221 anyio-4.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:01:39.324221 anyio-4.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:01:39.332221 anyio-4.4.0/src/anyio/
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:01:39.336221 anyio-4.4.0/src/anyio/_backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83244 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/_backends/_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35909 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/_backends/_trio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:01:39.336221 anyio-4.4.0/src/anyio/_core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/_core/_eventloop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/_core/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19456 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/_core/_fileio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/_core/_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/_core/_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24028 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/_core/_sockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/_core/_streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/_core/_subprocesses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18444 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/_core/_synchronization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/_core/_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/_core/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/_core/_typedattr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:01:39.336221 anyio-4.4.0/src/anyio/abc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10085 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/abc/_eventloop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/abc/_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/abc/_sockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/abc/_streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/abc/_subprocesses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/abc/_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/abc/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17700 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/from_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/lowlevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/pytest_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:01:39.340221 anyio-4.4.0/src/anyio/streams/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/streams/buffered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/streams/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/streams/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/streams/stapled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/streams/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/streams/tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/to_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-26 22:01:34.000000 anyio-4.4.0/src/anyio/to_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:01:39.344221 anyio-4.4.0/src/anyio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-26 22:01:39.000000 anyio-4.4.0/src/anyio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-26 22:01:39.000000 anyio-4.4.0/src/anyio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 22:01:39.000000 anyio-4.4.0/src/anyio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-26 22:01:39.000000 anyio-4.4.0/src/anyio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-26 22:01:39.000000 anyio-4.4.0/src/anyio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-26 22:01:39.000000 anyio-4.4.0/src/anyio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:01:39.340221 anyio-4.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 22:01:34.000000 anyio-4.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-26 22:01:34.000000 anyio-4.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:01:39.344221 anyio-4.4.0/tests/streams/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 22:01:34.000000 anyio-4.4.0/tests/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-26 22:01:34.000000 anyio-4.4.0/tests/streams/test_buffered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-26 22:01:34.000000 anyio-4.4.0/tests/streams/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15346 2024-05-26 22:01:34.000000 anyio-4.4.0/tests/streams/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-05-26 22:01:34.000000 anyio-4.4.0/tests/streams/test_stapled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-26 22:01:34.000000 anyio-4.4.0/tests/streams/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18790 2024-05-26 22:01:34.000000 anyio-4.4.0/tests/streams/test_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-26 22:01:34.000000 anyio-4.4.0/tests/test_debugging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-26 22:01:34.000000 anyio-4.4.0/tests/test_eventloop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20553 2024-05-26 22:01:34.000000 anyio-4.4.0/tests/test_fileio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23046 2024-05-26 22:01:34.000000 anyio-4.4.0/tests/test_from_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-26 22:01:34.000000 anyio-4.4.0/tests/test_lowlevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11168 2024-05-26 22:01:34.000000 anyio-4.4.0/tests/test_pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-26 22:01:34.000000 anyio-4.4.0/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66565 2024-05-26 22:01:34.000000 anyio-4.4.0/tests/test_sockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-05-26 22:01:34.000000 anyio-4.4.0/tests/test_subprocesses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22197 2024-05-26 22:01:34.000000 anyio-4.4.0/tests/test_synchronization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41395 2024-05-26 22:01:34.000000 anyio-4.4.0/tests/test_taskgroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-05-26 22:01:34.000000 anyio-4.4.0/tests/test_to_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-05-26 22:01:34.000000 anyio-4.4.0/tests/test_to_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-26 22:01:34.000000 anyio-4.4.0/tests/test_typedattr.py
```

### Comparing `anyio-4.3.0/.github/ISSUE_TEMPLATE/bug_report.yaml` & `anyio-4.4.0/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/.github/ISSUE_TEMPLATE/features_request.yaml` & `anyio-4.4.0/.github/ISSUE_TEMPLATE/features_request.yaml`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/.github/workflows/publish.yml` & `anyio-4.4.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/.github/workflows/test-downstream.yml` & `anyio-4.4.0/.github/workflows/test-downstream.yml`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/.github/workflows/test.yml` & `anyio-4.4.0/.github/workflows/test.yml`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
       }}
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
       uses: actions/setup-python@v5
       with:
         python-version: 3.x
-    - uses: actions/cache@v3
+    - uses: actions/cache@v4
       with:
         path: ~/.cache/pip
         key: pip-pyright
     - name: Install dependencies
       run: pip install -e . pyright pytest
     - name: Run pyright
       run: pyright --verifytypes anyio
```

### Comparing `anyio-4.3.0/.pre-commit-config.yaml` & `anyio-4.4.0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # This is the configuration file for pre-commit (https://pre-commit.com/).
 # To use:
 # * Install pre-commit (https://pre-commit.com/#installation)
 # * Copy this file as ".pre-commit-config.yaml"
 # * Run "pre-commit install".
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-toml
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [ "--fix=lf" ]
       - id: trailing-whitespace
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.2.1
+    rev: v0.4.4
     hooks:
       - id: ruff
         args: [--fix, --show-fixes]
       - id: ruff-format
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.8.0
+    rev: v1.10.0
     hooks:
       - id: mypy
         additional_dependencies:
           - pytest
           - trio >= 0.23
           - packaging
```

### Comparing `anyio-4.3.0/LICENSE` & `anyio-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/PKG-INFO` & `anyio-4.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyio
-Version: 4.3.0
+Version: 4.4.0
 Summary: High level compatibility layer for multiple asynchronous event loop implementations
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://anyio.readthedocs.io/en/latest/
 Project-URL: Changelog, https://anyio.readthedocs.io/en/stable/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/anyio
 Project-URL: Issue tracker, https://github.com/agronholm/anyio/issues
```

### Comparing `anyio-4.3.0/README.rst` & `anyio-4.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/docs/api.rst` & `anyio-4.4.0/docs/api.rst`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 
 .. autofunction:: anyio.from_thread.run
 .. autofunction:: anyio.from_thread.run_sync
 .. autofunction:: anyio.from_thread.check_cancelled
 .. autofunction:: anyio.from_thread.start_blocking_portal
 
 .. autoclass:: anyio.from_thread.BlockingPortal
+.. autoclass:: anyio.from_thread.BlockingPortalProvider
 
 Async file I/O
 --------------
 
 .. autofunction:: anyio.open_file
 .. autofunction:: anyio.wrap_file
```

### Comparing `anyio-4.3.0/docs/basics.rst` & `anyio-4.4.0/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/docs/cancellation.rst` & `anyio-4.4.0/docs/cancellation.rst`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/docs/conf.py` & `anyio-4.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/docs/contributing.rst` & `anyio-4.4.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/docs/faq.rst` & `anyio-4.4.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/docs/fileio.rst` & `anyio-4.4.0/docs/fileio.rst`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/docs/migration.rst` & `anyio-4.4.0/docs/migration.rst`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/docs/networking.rst` & `anyio-4.4.0/docs/networking.rst`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/docs/signals.rst` & `anyio-4.4.0/docs/signals.rst`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/docs/streams.rst` & `anyio-4.4.0/docs/streams.rst`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,15 @@
 There are three principal ways you can get an X.509 certificate for your server:
 
 #. Create a self signed certificate
 #. Use certbot_ or a similar software to automatically obtain certificates from
    `Let's Encrypt`_
 #. Buy one from a certificate vendor
 
-The first option is probably the easiest, but this requires that the any client
+The first option is probably the easiest, but this requires that any client
 connecting to your server adds the self signed certificate to their list of trusted
 certificates. This is of course impractical outside of local development and is strongly
 discouraged in production use.
 
 The second option is nowadays the recommended method, as long as you have an environment
 where running certbot_ or similar software can automatically replace the certificate
 with a newer one when necessary, and that you don't need any extra features like class 2
```

### Comparing `anyio-4.3.0/docs/subprocesses.rst` & `anyio-4.4.0/docs/subprocesses.rst`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/docs/support.rst` & `anyio-4.4.0/docs/support.rst`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/docs/synchronization.rst` & `anyio-4.4.0/docs/synchronization.rst`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/docs/tasks.rst` & `anyio-4.4.0/docs/tasks.rst`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/docs/testing.rst` & `anyio-4.4.0/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/docs/threads.rst` & `anyio-4.4.0/docs/threads.rst`

 * *Files 4% similar despite different names*

```diff
@@ -221,7 +221,31 @@
             from_thread.check_cancelled()
             print("Not cancelled yet")
             sleep(1)
 
     async def foo():
         with move_on_after(3):
             await to_thread.run_sync(sync_function)
+
+
+Sharing a blocking portal on demand
+-----------------------------------
+
+If you're building a synchronous API that needs to start a blocking portal on demand,
+you might need a more efficient solution than just starting a blocking portal for each
+call. To that end, you can use :class:`BlockingPortalProvider`::
+
+    from anyio.to_thread import BlockingPortalProvider
+
+    class MyAPI:
+        def __init__(self, async_obj) -> None:
+            self._async_obj = async_obj
+            self._portal_provider = BlockingPortalProvider()
+
+        def do_stuff(self) -> None:
+            with self._portal_provider as portal:
+                portal.call(async_obj.do_async_stuff)
+
+Now, no matter how many threads call the ``do_stuff()`` method on a ``MyAPI`` instance
+at the same time, the same blocking portal will be used to handle the async calls
+inside. It's easy to see that this is much more efficient than having each call spawn
+its own blocking portal.
```

### Comparing `anyio-4.3.0/docs/typedattrs.rst` & `anyio-4.4.0/docs/typedattrs.rst`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/docs/versionhistory.rst` & `anyio-4.4.0/docs/versionhistory.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,57 @@
 Version history
 ===============
 
 This library adheres to `Semantic Versioning 2.0 <http://semver.org/>`_.
 
+**4.4.0**
+
+- Added the ``BlockingPortalProvider`` class to aid with constructing synchronous
+  counterparts to asynchronous interfaces that would otherwise require multiple blocking
+  portals
+- Added ``__slots__`` to ``AsyncResource`` so that child classes can use ``__slots__``
+  (`#733 <https://github.com/agronholm/anyio/pull/733>`_; PR by Justin Su)
+- Added the ``TaskInfo.has_pending_cancellation()`` method
+- Fixed erroneous ``RuntimeError: called 'started' twice on the same task status``
+  when cancelling a task in a TaskGroup created with the ``start()`` method before
+  the first checkpoint is reached after calling ``task_status.started()``
+  (`#706 <https://github.com/agronholm/anyio/issues/706>`_; PR by Dominik Schwabe)
+- Fixed two bugs with ``TaskGroup.start()`` on asyncio:
+
+  * Fixed erroneous ``RuntimeError: called 'started' twice on the same task status``
+    when cancelling a task in a TaskGroup created with the ``start()`` method before
+    the first checkpoint is reached after calling ``task_status.started()``
+    (`#706 <https://github.com/agronholm/anyio/issues/706>`_; PR by Dominik Schwabe)
+  * Fixed the entire task group being cancelled if a ``TaskGroup.start()`` call gets
+    cancelled (`#685 <https://github.com/agronholm/anyio/issues/685>`_,
+    `#710 <https://github.com/agronholm/anyio/issues/710>`_)
+- Fixed a race condition that caused crashes when multiple event loops of the same
+  backend were running in separate threads and simultaneously attempted to use AnyIO for
+  their first time (`#425 <https://github.com/agronholm/anyio/issues/425>`_; PR by David
+  Jiricek and Ganden Schaffner)
+- Fixed cancellation delivery on asyncio incrementing the wrong cancel scope's
+  cancellation counter when cascading a cancel operation to a child scope, thus failing
+  to uncancel the host task (`#716 <https://github.com/agronholm/anyio/issues/716>`_)
+- Fixed erroneous ``TypedAttributeLookupError`` if a typed attribute getter raises
+  ``KeyError``
+- Fixed the asyncio backend not respecting the ``PYTHONASYNCIODEBUG`` environment
+  variable when setting the ``debug`` flag in ``anyio.run()``
+- Fixed ``SocketStream.receive()`` not detecting EOF on asyncio if there is also data in
+  the read buffer (`#701 <https://github.com/agronholm/anyio/issues/701>`_)
+- Fixed ``MemoryObjectStream`` dropping an item if the item is delivered to a recipient
+  that is waiting to receive an item but has a cancellation pending
+  (`#728 <https://github.com/agronholm/anyio/issues/728>`_)
+- Emit a ``ResourceWarning`` for ``MemoryObjectReceiveStream`` and
+  ``MemoryObjectSendStream`` that were garbage collected without being closed (PR by
+  Andrey Kazantcev)
+- Fixed ``MemoryObjectSendStream.send()`` not raising ``BrokenResourceError`` when the
+  last corresponding ``MemoryObjectReceiveStream`` is closed while waiting to send a
+  falsey item (`#731 <https://github.com/agronholm/anyio/issues/731>`_; PR by Ganden
+  Schaffner)
+
 **4.3.0**
 
 - Added support for the Python 3.12 ``walk_up`` keyword argument in
   ``anyio.Path.relative_to()`` (PR by Colin Taylor)
 - Fixed passing ``total_tokens`` to ``anyio.CapacityLimiter()`` as a keyword argument
   not working on the ``trio`` backend
   (`#515 <https://github.com/agronholm/anyio/issues/515>`_)
```

### Comparing `anyio-4.3.0/pyproject.toml` & `anyio-4.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -64,23 +64,30 @@
 pytest11 = {anyio = "anyio.pytest_plugin"}
 
 [tool.setuptools_scm]
 version_scheme = "post-release"
 local_scheme = "dirty-tag"
 
 [tool.ruff]
-select = [
-    "E", "F", "W",  # default flake-8
+src = ["src"]
+
+[tool.ruff.lint]
+extend-select = [
+    "ASYNC",        # flake8-async
+    "W",            # pycodestyle warnings
+    "G",            # flake8-logging-format
     "I",            # isort
+    "ISC",          # flake8-implicit-str-concat
     "PGH",          # pygrep-hooks
+    "RUF100",       # unused noqa (yesqa)
+    "T201",         # print
     "UP",           # pyupgrade
 ]
-src = ["src"]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 "required-imports" = ["from __future__ import annotations"]
 
 [tool.mypy]
 python_version = "3.12"
 strict = true
 ignore_missing_imports = true
 disallow_any_generics = false
@@ -124,14 +131,17 @@
 
 [testenv]
 depends = pre-commit
 package = editable
 commands = coverage run -m pytest {posargs}
 extras = test
 
+[testenv:pypy3]
+commands = pytest {posargs}
+
 [testenv:pre-commit]
 depends =
 basepython = python3
 package = skip
 deps = pre-commit
 commands = pre-commit run --all-files
```

### Comparing `anyio-4.3.0/src/anyio/__init__.py` & `anyio-4.4.0/src/anyio/__init__.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/src/anyio/_backends/_asyncio.py` & `anyio-4.4.0/src/anyio/_backends/_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import array
 import asyncio
 import concurrent.futures
 import math
 import socket
 import sys
 import threading
+import weakref
 from asyncio import (
     AbstractEventLoop,
     CancelledError,
     all_tasks,
     create_task,
     current_task,
     get_running_loop,
@@ -484,15 +485,15 @@
                 continue
 
             # The task is eligible for cancellation if it has started
             should_retry = True
             if task is not current and (task is self._host_task or _task_started(task)):
                 waiter = task._fut_waiter  # type: ignore[attr-defined]
                 if not isinstance(waiter, asyncio.Future) or not waiter.done():
-                    self._cancel_calls += 1
+                    origin._cancel_calls += 1
                     if sys.version_info >= (3, 9):
                         task.cancel(f"Cancelled by cancel scope {id(origin):x}")
                     else:
                         task.cancel()
 
         # Deliver cancellation to child scopes that aren't shielded or running their own
         # cancellation callbacks
@@ -592,22 +593,22 @@
 
 class TaskState:
     """
     Encapsulates auxiliary task information that cannot be added to the Task instance
     itself because there are no guarantees about its implementation.
     """
 
-    __slots__ = "parent_id", "cancel_scope"
+    __slots__ = "parent_id", "cancel_scope", "__weakref__"
 
     def __init__(self, parent_id: int | None, cancel_scope: CancelScope | None):
         self.parent_id = parent_id
         self.cancel_scope = cancel_scope
 
 
-_task_states = WeakKeyDictionary()  # type: WeakKeyDictionary[asyncio.Task, TaskState]
+_task_states: WeakKeyDictionary[asyncio.Task, TaskState] = WeakKeyDictionary()
 
 
 #
 # Task groups
 #
 
 
@@ -616,17 +617,18 @@
         self._future = future
         self._parent_id = parent_id
 
     def started(self, value: T_contra | None = None) -> None:
         try:
             self._future.set_result(value)
         except asyncio.InvalidStateError:
-            raise RuntimeError(
-                "called 'started' twice on the same task status"
-            ) from None
+            if not self._future.cancelled():
+                raise RuntimeError(
+                    "called 'started' twice on the same task status"
+                ) from None
 
         task = cast(asyncio.Task, current_task())
         _task_states[task].parent_id = self._parent_id
 
 
 def iterate_exceptions(
     exception: BaseException,
@@ -709,14 +711,20 @@
             except CancelledError as e:
                 while isinstance(e.__context__, CancelledError):
                     e = e.__context__
 
                 exc = e
 
             if exc is not None:
+                # The future can only be in the cancelled state if the host task was
+                # cancelled, so return immediately instead of adding one more
+                # CancelledError to the exceptions list
+                if task_status_future is not None and task_status_future.cancelled():
+                    return
+
                 if task_status_future is None or task_status_future.done():
                     if not isinstance(exc, CancelledError):
                         self._exceptions.append(exc)
 
                     if not self.cancel_scope._parent_cancelled():
                         self.cancel_scope.cancel()
                 else:
@@ -1043,14 +1051,15 @@
 
 
 class StreamProtocol(asyncio.Protocol):
     read_queue: deque[bytes]
     read_event: asyncio.Event
     write_event: asyncio.Event
     exception: Exception | None = None
+    is_at_eof: bool = False
 
     def connection_made(self, transport: asyncio.BaseTransport) -> None:
         self.read_queue = deque()
         self.read_event = asyncio.Event()
         self.write_event = asyncio.Event()
         self.write_event.set()
         cast(asyncio.Transport, transport).set_write_buffer_limits(0)
@@ -1064,14 +1073,15 @@
         self.write_event.set()
 
     def data_received(self, data: bytes) -> None:
         self.read_queue.append(data)
         self.read_event.set()
 
     def eof_received(self) -> bool | None:
+        self.is_at_eof = True
         self.read_event.set()
         return True
 
     def pause_writing(self) -> None:
         self.write_event = asyncio.Event()
 
     def resume_writing(self) -> None:
@@ -1119,23 +1129,24 @@
 
     @property
     def _raw_socket(self) -> socket.socket:
         return self._transport.get_extra_info("socket")
 
     async def receive(self, max_bytes: int = 65536) -> bytes:
         with self._receive_guard:
-            await AsyncIOBackend.checkpoint()
-
             if (
                 not self._protocol.read_event.is_set()
                 and not self._transport.is_closing()
+                and not self._protocol.is_at_eof
             ):
                 self._transport.resume_reading()
                 await self._protocol.read_event.wait()
                 self._transport.pause_reading()
+            else:
+                await AsyncIOBackend.checkpoint()
 
             try:
                 chunk = self._protocol.read_queue.popleft()
             except IndexError:
                 if self._closed:
                     raise ClosedResourceError from None
                 elif self._protocol.exception:
@@ -1647,15 +1658,15 @@
     async def wait(self) -> None:
         if self.is_set():
             await AsyncIOBackend.checkpoint()
         else:
             await self._event.wait()
 
     def statistics(self) -> EventStatistics:
-        return EventStatistics(len(self._event._waiters))  # type: ignore[attr-defined]
+        return EventStatistics(len(self._event._waiters))
 
 
 class CapacityLimiter(BaseCapacityLimiter):
     _total_tokens: float = 0
 
     def __new__(cls, total_tokens: float) -> CapacityLimiter:
         return object.__new__(cls)
@@ -1747,15 +1758,15 @@
         self.release_on_behalf_of(current_task())
 
     def release_on_behalf_of(self, borrower: object) -> None:
         try:
             self._borrowers.remove(borrower)
         except KeyError:
             raise RuntimeError(
-                "this borrower isn't holding any of this CapacityLimiter's " "tokens"
+                "this borrower isn't holding any of this CapacityLimiter's tokens"
             ) from None
 
         # Notify the next task in line if this limiter has free capacity now
         if self._wait_queue and len(self._borrowers) < self._total_tokens:
             event = self._wait_queue.popitem(last=False)[1]
             event.set()
 
@@ -1819,22 +1830,44 @@
 
 
 #
 # Testing and debugging
 #
 
 
-def _create_task_info(task: asyncio.Task) -> TaskInfo:
-    task_state = _task_states.get(task)
-    if task_state is None:
-        parent_id = None
-    else:
-        parent_id = task_state.parent_id
+class AsyncIOTaskInfo(TaskInfo):
+    def __init__(self, task: asyncio.Task):
+        task_state = _task_states.get(task)
+        if task_state is None:
+            parent_id = None
+        else:
+            parent_id = task_state.parent_id
 
-    return TaskInfo(id(task), parent_id, task.get_name(), task.get_coro())
+        super().__init__(id(task), parent_id, task.get_name(), task.get_coro())
+        self._task = weakref.ref(task)
+
+    def has_pending_cancellation(self) -> bool:
+        if not (task := self._task()):
+            # If the task isn't around anymore, it won't have a pending cancellation
+            return False
+
+        if sys.version_info >= (3, 11):
+            if task.cancelling():
+                return True
+        elif (
+            isinstance(task._fut_waiter, asyncio.Future)
+            and task._fut_waiter.cancelled()
+        ):
+            return True
+
+        if task_state := _task_states.get(task):
+            if cancel_scope := task_state.cancel_scope:
+                return cancel_scope.cancel_called or cancel_scope._parent_cancelled()
+
+        return False
 
 
 class TestRunner(abc.TestRunner):
     _send_stream: MemoryObjectSendStream[tuple[Awaitable[Any], asyncio.Future[Any]]]
 
     def __init__(
         self,
@@ -1883,21 +1916,21 @@
             if len(exceptions) == 1:
                 raise exceptions[0]
             elif exceptions:
                 raise BaseExceptionGroup(
                     "Multiple exceptions occurred in asynchronous callbacks", exceptions
                 )
 
-    @staticmethod
     async def _run_tests_and_fixtures(
+        self,
         receive_stream: MemoryObjectReceiveStream[
             tuple[Awaitable[T_Retval], asyncio.Future[T_Retval]]
         ],
     ) -> None:
-        with receive_stream:
+        with receive_stream, self._send_stream:
             async for coro, future in receive_stream:
                 try:
                     retval = await coro
                 except BaseException as exc:
                     if not future.cancelled():
                         future.set_exception(exc)
                 else:
@@ -1986,15 +2019,15 @@
             _task_states[task] = TaskState(None, None)
 
             try:
                 return await func(*args)
             finally:
                 del _task_states[task]
 
-        debug = options.get("debug", False)
+        debug = options.get("debug", None)
         loop_factory = options.get("loop_factory", None)
         if loop_factory is None and options.get("use_uvloop", False):
             import uvloop
 
             loop_factory = uvloop.new_event_loop
 
         with Runner(debug=debug, loop_factory=loop_factory) as runner:
@@ -2444,19 +2477,19 @@
     def open_signal_receiver(
         cls, *signals: Signals
     ) -> ContextManager[AsyncIterator[Signals]]:
         return _SignalReceiver(signals)
 
     @classmethod
     def get_current_task(cls) -> TaskInfo:
-        return _create_task_info(current_task())  # type: ignore[arg-type]
+        return AsyncIOTaskInfo(current_task())  # type: ignore[arg-type]
 
     @classmethod
-    def get_running_tasks(cls) -> list[TaskInfo]:
-        return [_create_task_info(task) for task in all_tasks() if not task.done()]
+    def get_running_tasks(cls) -> Sequence[TaskInfo]:
+        return [AsyncIOTaskInfo(task) for task in all_tasks() if not task.done()]
 
     @classmethod
     async def wait_all_tasks_blocked(cls) -> None:
         await cls.checkpoint()
         this_task = current_task()
         while True:
             for task in all_tasks():
```

### Comparing `anyio-4.3.0/src/anyio/_backends/_trio.py` & `anyio-4.4.0/src/anyio/_backends/_trio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import array
 import math
 import socket
 import sys
 import types
+import weakref
 from collections.abc import AsyncIterator, Iterable
 from concurrent.futures import Future
 from dataclasses import dataclass
 from functools import partial
 from io import IOBase
 from os import PathLike
 from signal import Signals
@@ -835,14 +836,32 @@
 
     def run_test(
         self, test_func: Callable[..., Coroutine[Any, Any, Any]], kwargs: dict[str, Any]
     ) -> None:
         self._call_in_runner_task(test_func, **kwargs)
 
 
+class TrioTaskInfo(TaskInfo):
+    def __init__(self, task: trio.lowlevel.Task):
+        parent_id = None
+        if task.parent_nursery and task.parent_nursery.parent_task:
+            parent_id = id(task.parent_nursery.parent_task)
+
+        super().__init__(id(task), parent_id, task.name, task.coro)
+        self._task = weakref.proxy(task)
+
+    def has_pending_cancellation(self) -> bool:
+        try:
+            return self._task._cancel_status.effectively_cancelled
+        except ReferenceError:
+            # If the task is no longer around, it surely doesn't have a cancellation
+            # pending
+            return False
+
+
 class TrioBackend(AsyncBackend):
     @classmethod
     def run(
         cls,
         func: Callable[[Unpack[PosArgsT]], Awaitable[T_Retval]],
         args: tuple[Unpack[PosArgsT]],
         kwargs: dict[str, Any],
@@ -1036,23 +1055,21 @@
         else:
             return UDPSocket(trio_socket)
 
     @classmethod
     @overload
     async def create_unix_datagram_socket(
         cls, raw_socket: socket.socket, remote_path: None
-    ) -> abc.UNIXDatagramSocket:
-        ...
+    ) -> abc.UNIXDatagramSocket: ...
 
     @classmethod
     @overload
     async def create_unix_datagram_socket(
         cls, raw_socket: socket.socket, remote_path: str | bytes
-    ) -> abc.ConnectedUNIXDatagramSocket:
-        ...
+    ) -> abc.ConnectedUNIXDatagramSocket: ...
 
     @classmethod
     async def create_unix_datagram_socket(
         cls, raw_socket: socket.socket, remote_path: str | bytes | None
     ) -> abc.UNIXDatagramSocket | abc.ConnectedUNIXDatagramSocket:
         trio_socket = trio.socket.from_stdlib_socket(raw_socket)
 
@@ -1123,36 +1140,27 @@
         cls, *signals: Signals
     ) -> ContextManager[AsyncIterator[Signals]]:
         return _SignalReceiver(signals)
 
     @classmethod
     def get_current_task(cls) -> TaskInfo:
         task = current_task()
-
-        parent_id = None
-        if task.parent_nursery and task.parent_nursery.parent_task:
-            parent_id = id(task.parent_nursery.parent_task)
-
-        return TaskInfo(id(task), parent_id, task.name, task.coro)
+        return TrioTaskInfo(task)
 
     @classmethod
-    def get_running_tasks(cls) -> list[TaskInfo]:
+    def get_running_tasks(cls) -> Sequence[TaskInfo]:
         root_task = current_root_task()
         assert root_task
-        task_infos = [TaskInfo(id(root_task), None, root_task.name, root_task.coro)]
+        task_infos = [TrioTaskInfo(root_task)]
         nurseries = root_task.child_nurseries
         while nurseries:
             new_nurseries: list[trio.Nursery] = []
             for nursery in nurseries:
                 for task in nursery.child_tasks:
-                    task_infos.append(
-                        TaskInfo(
-                            id(task), id(nursery.parent_task), task.name, task.coro
-                        )
-                    )
+                    task_infos.append(TrioTaskInfo(task))
                     new_nurseries.extend(task.child_nurseries)
 
             nurseries = new_nurseries
 
         return task_infos
 
     @classmethod
```

### Comparing `anyio-4.3.0/src/anyio/_core/_eventloop.py` & `anyio-4.4.0/src/anyio/_core/_eventloop.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # This must be updated when new backends are introduced
 BACKENDS = "asyncio", "trio"
 
 T_Retval = TypeVar("T_Retval")
 PosArgsT = TypeVarTuple("PosArgsT")
 
 threadlocals = threading.local()
+loaded_backends: dict[str, type[AsyncBackend]] = {}
 
 
 def run(
     func: Callable[[Unpack[PosArgsT]], Awaitable[T_Retval]],
     *args: Unpack[PosArgsT],
     backend: str = "asyncio",
     backend_options: dict[str, Any] | None = None,
@@ -146,18 +147,20 @@
     try:
         yield
     finally:
         del threadlocals.current_async_backend
         del threadlocals.current_token
 
 
-def get_async_backend(asynclib_name: str | None = None) -> AsyncBackend:
+def get_async_backend(asynclib_name: str | None = None) -> type[AsyncBackend]:
     if asynclib_name is None:
         asynclib_name = sniffio.current_async_library()
 
-    modulename = "anyio._backends._" + asynclib_name
+    # We use our own dict instead of sys.modules to get the already imported back-end
+    # class because the appropriate modules in sys.modules could potentially be only
+    # partially initialized
     try:
-        module = sys.modules[modulename]
+        return loaded_backends[asynclib_name]
     except KeyError:
-        module = import_module(modulename)
-
-    return getattr(module, "backend_class")
+        module = import_module(f"anyio._backends._{asynclib_name}")
+        loaded_backends[asynclib_name] = module.backend_class
+        return module.backend_class
```

### Comparing `anyio-4.3.0/src/anyio/_core/_exceptions.py` & `anyio-4.4.0/src/anyio/_core/_exceptions.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/src/anyio/_core/_fileio.py` & `anyio-4.4.0/src/anyio/_core/_fileio.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,33 +96,29 @@
     async def readinto(self: AsyncFile[bytes], b: WriteableBuffer) -> bytes:
         return await to_thread.run_sync(self._fp.readinto, b)
 
     async def readinto1(self: AsyncFile[bytes], b: WriteableBuffer) -> bytes:
         return await to_thread.run_sync(self._fp.readinto1, b)
 
     @overload
-    async def write(self: AsyncFile[bytes], b: ReadableBuffer) -> int:
-        ...
+    async def write(self: AsyncFile[bytes], b: ReadableBuffer) -> int: ...
 
     @overload
-    async def write(self: AsyncFile[str], b: str) -> int:
-        ...
+    async def write(self: AsyncFile[str], b: str) -> int: ...
 
     async def write(self, b: ReadableBuffer | str) -> int:
         return await to_thread.run_sync(self._fp.write, b)
 
     @overload
     async def writelines(
         self: AsyncFile[bytes], lines: Iterable[ReadableBuffer]
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @overload
-    async def writelines(self: AsyncFile[str], lines: Iterable[str]) -> None:
-        ...
+    async def writelines(self: AsyncFile[str], lines: Iterable[str]) -> None: ...
 
     async def writelines(self, lines: Iterable[ReadableBuffer] | Iterable[str]) -> None:
         return await to_thread.run_sync(self._fp.writelines, lines)
 
     async def truncate(self, size: int | None = None) -> int:
         return await to_thread.run_sync(self._fp.truncate, size)
 
@@ -142,30 +138,28 @@
     mode: OpenBinaryMode,
     buffering: int = ...,
     encoding: str | None = ...,
     errors: str | None = ...,
     newline: str | None = ...,
     closefd: bool = ...,
     opener: Callable[[str, int], int] | None = ...,
-) -> AsyncFile[bytes]:
-    ...
+) -> AsyncFile[bytes]: ...
 
 
 @overload
 async def open_file(
     file: str | PathLike[str] | int,
     mode: OpenTextMode = ...,
     buffering: int = ...,
     encoding: str | None = ...,
     errors: str | None = ...,
     newline: str | None = ...,
     closefd: bool = ...,
     opener: Callable[[str, int], int] | None = ...,
-) -> AsyncFile[str]:
-    ...
+) -> AsyncFile[str]: ...
 
 
 async def open_file(
     file: str | PathLike[str] | int,
     mode: str = "r",
     buffering: int = -1,
     encoding: str | None = None,
@@ -472,27 +466,25 @@
     async def open(
         self,
         mode: OpenBinaryMode,
         buffering: int = ...,
         encoding: str | None = ...,
         errors: str | None = ...,
         newline: str | None = ...,
-    ) -> AsyncFile[bytes]:
-        ...
+    ) -> AsyncFile[bytes]: ...
 
     @overload
     async def open(
         self,
         mode: OpenTextMode = ...,
         buffering: int = ...,
         encoding: str | None = ...,
         errors: str | None = ...,
         newline: str | None = ...,
-    ) -> AsyncFile[str]:
-        ...
+    ) -> AsyncFile[str]: ...
 
     async def open(
         self,
         mode: str = "r",
         buffering: int = -1,
         encoding: str | None = None,
         errors: str | None = None,
```

### Comparing `anyio-4.3.0/src/anyio/_core/_signals.py` & `anyio-4.4.0/src/anyio/_core/_signals.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/src/anyio/_core/_sockets.py` & `anyio-4.4.0/src/anyio/_core/_sockets.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,75 +49,70 @@
     remote_port: int,
     *,
     local_host: IPAddressType | None = ...,
     ssl_context: ssl.SSLContext | None = ...,
     tls_standard_compatible: bool = ...,
     tls_hostname: str,
     happy_eyeballs_delay: float = ...,
-) -> TLSStream:
-    ...
+) -> TLSStream: ...
 
 
 # ssl_context given
 @overload
 async def connect_tcp(
     remote_host: IPAddressType,
     remote_port: int,
     *,
     local_host: IPAddressType | None = ...,
     ssl_context: ssl.SSLContext,
     tls_standard_compatible: bool = ...,
     tls_hostname: str | None = ...,
     happy_eyeballs_delay: float = ...,
-) -> TLSStream:
-    ...
+) -> TLSStream: ...
 
 
 # tls=True
 @overload
 async def connect_tcp(
     remote_host: IPAddressType,
     remote_port: int,
     *,
     local_host: IPAddressType | None = ...,
     tls: Literal[True],
     ssl_context: ssl.SSLContext | None = ...,
     tls_standard_compatible: bool = ...,
     tls_hostname: str | None = ...,
     happy_eyeballs_delay: float = ...,
-) -> TLSStream:
-    ...
+) -> TLSStream: ...
 
 
 # tls=False
 @overload
 async def connect_tcp(
     remote_host: IPAddressType,
     remote_port: int,
     *,
     local_host: IPAddressType | None = ...,
     tls: Literal[False],
     ssl_context: ssl.SSLContext | None = ...,
     tls_standard_compatible: bool = ...,
     tls_hostname: str | None = ...,
     happy_eyeballs_delay: float = ...,
-) -> SocketStream:
-    ...
+) -> SocketStream: ...
 
 
 # No TLS arguments
 @overload
 async def connect_tcp(
     remote_host: IPAddressType,
     remote_port: int,
     *,
     local_host: IPAddressType | None = ...,
     happy_eyeballs_delay: float = ...,
-) -> SocketStream:
-    ...
+) -> SocketStream: ...
 
 
 async def connect_tcp(
     remote_host: IPAddressType,
     remote_port: int,
     *,
     local_host: IPAddressType | None = None,
```

### Comparing `anyio-4.3.0/src/anyio/_core/_streams.py` & `anyio-4.4.0/src/anyio/_core/_streams.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/src/anyio/_core/_subprocesses.py` & `anyio-4.4.0/src/anyio/_core/_subprocesses.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/src/anyio/_core/_synchronization.py` & `anyio-4.4.0/src/anyio/_core/_synchronization.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/src/anyio/_core/_tasks.py` & `anyio-4.4.0/src/anyio/_core/_tasks.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/src/anyio/_core/_testing.py` & `anyio-4.4.0/src/anyio/_core/_testing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from collections.abc import Awaitable, Generator
-from typing import Any
+from typing import Any, cast
 
 from ._eventloop import get_async_backend
 
 
 class TaskInfo:
     """
     Represents an asynchronous task.
@@ -41,16 +41,20 @@
 
     def __hash__(self) -> int:
         return hash(self.id)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(id={self.id!r}, name={self.name!r})"
 
-    def _unwrap(self) -> TaskInfo:
-        return self
+    def has_pending_cancellation(self) -> bool:
+        """
+        Return ``True`` if the task has a cancellation pending, ``False`` otherwise.
+
+        """
+        return False
 
 
 def get_current_task() -> TaskInfo:
     """
     Return the current task.
 
     :return: a representation of the current task
@@ -62,13 +66,13 @@
 def get_running_tasks() -> list[TaskInfo]:
     """
     Return a list of running tasks in the current event loop.
 
     :return: a list of task info objects
 
     """
-    return get_async_backend().get_running_tasks()
+    return cast("list[TaskInfo]", get_async_backend().get_running_tasks())
 
 
 async def wait_all_tasks_blocked() -> None:
     """Wait until all other tasks are waiting for something."""
     await get_async_backend().wait_all_tasks_blocked()
```

### Comparing `anyio-4.3.0/src/anyio/_core/_typedattr.py` & `anyio-4.4.0/src/anyio/_core/_typedattr.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,20 +46,18 @@
         also be included in the returned mapping (but the wrapper may override the
         callables from the wrapped instance).
 
         """
         return {}
 
     @overload
-    def extra(self, attribute: T_Attr) -> T_Attr:
-        ...
+    def extra(self, attribute: T_Attr) -> T_Attr: ...
 
     @overload
-    def extra(self, attribute: T_Attr, default: T_Default) -> T_Attr | T_Default:
-        ...
+    def extra(self, attribute: T_Attr, default: T_Default) -> T_Attr | T_Default: ...
 
     @final
     def extra(self, attribute: Any, default: object = undefined) -> object:
         """
         extra(attribute, default=undefined)
 
         Return the value of the given typed extra attribute.
@@ -69,13 +67,15 @@
         :param default: the value that should be returned if no value is found for the
             attribute
         :raises ~anyio.TypedAttributeLookupError: if the search failed and no default
             value was given
 
         """
         try:
-            return self.extra_attributes[attribute]()
+            getter = self.extra_attributes[attribute]
         except KeyError:
             if default is undefined:
                 raise TypedAttributeLookupError("Attribute not found") from None
             else:
                 return default
+
+        return getter()
```

### Comparing `anyio-4.3.0/src/anyio/abc/__init__.py` & `anyio-4.4.0/src/anyio/abc/__init__.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/src/anyio/abc/_eventloop.py` & `anyio-4.4.0/src/anyio/abc/_eventloop.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,23 +299,21 @@
     ) -> UDPSocket | ConnectedUDPSocket:
         pass
 
     @classmethod
     @overload
     async def create_unix_datagram_socket(
         cls, raw_socket: socket, remote_path: None
-    ) -> UNIXDatagramSocket:
-        ...
+    ) -> UNIXDatagramSocket: ...
 
     @classmethod
     @overload
     async def create_unix_datagram_socket(
         cls, raw_socket: socket, remote_path: str | bytes
-    ) -> ConnectedUNIXDatagramSocket:
-        ...
+    ) -> ConnectedUNIXDatagramSocket: ...
 
     @classmethod
     @abstractmethod
     async def create_unix_datagram_socket(
         cls, raw_socket: socket, remote_path: str | bytes | None
     ) -> UNIXDatagramSocket | ConnectedUNIXDatagramSocket:
         pass
@@ -374,15 +372,15 @@
     @classmethod
     @abstractmethod
     def get_current_task(cls) -> TaskInfo:
         pass
 
     @classmethod
     @abstractmethod
-    def get_running_tasks(cls) -> list[TaskInfo]:
+    def get_running_tasks(cls) -> Sequence[TaskInfo]:
         pass
 
     @classmethod
     @abstractmethod
     async def wait_all_tasks_blocked(cls) -> None:
         pass
```

### Comparing `anyio-4.3.0/src/anyio/abc/_resources.py` & `anyio-4.4.0/src/anyio/abc/_resources.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     """
     Abstract base class for all closeable asynchronous resources.
 
     Works as an asynchronous context manager which returns the instance itself on enter,
     and calls :meth:`aclose` on exit.
     """
 
+    __slots__ = ()
+
     async def __aenter__(self: T) -> T:
         return self
 
     async def __aexit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
```

### Comparing `anyio-4.3.0/src/anyio/abc/_sockets.py` & `anyio-4.4.0/src/anyio/abc/_sockets.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/src/anyio/abc/_streams.py` & `anyio-4.4.0/src/anyio/abc/_streams.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/src/anyio/abc/_subprocesses.py` & `anyio-4.4.0/src/anyio/abc/_subprocesses.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/src/anyio/abc/_tasks.py` & `anyio-4.4.0/src/anyio/abc/_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,18 @@
 T_Retval = TypeVar("T_Retval")
 T_contra = TypeVar("T_contra", contravariant=True)
 PosArgsT = TypeVarTuple("PosArgsT")
 
 
 class TaskStatus(Protocol[T_contra]):
     @overload
-    def started(self: TaskStatus[None]) -> None:
-        ...
+    def started(self: TaskStatus[None]) -> None: ...
 
     @overload
-    def started(self, value: T_contra) -> None:
-        ...
+    def started(self, value: T_contra) -> None: ...
 
     def started(self, value: T_contra | None = None) -> None:
         """
         Signal that the task has started.
 
         :param value: object passed back to the starter of the task
         """
```

### Comparing `anyio-4.3.0/src/anyio/abc/_testing.py` & `anyio-4.4.0/src/anyio/abc/_testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 
     @abstractmethod
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: types.TracebackType | None,
-    ) -> bool | None:
-        ...
+    ) -> bool | None: ...
 
     @abstractmethod
     def run_asyncgen_fixture(
         self,
         fixture_func: Callable[..., AsyncGenerator[_T, Any]],
         kwargs: dict[str, Any],
     ) -> Iterable[_T]:
```

### Comparing `anyio-4.3.0/src/anyio/from_thread.py` & `anyio-4.4.0/src/anyio/from_thread.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import sys
 import threading
 from collections.abc import Awaitable, Callable, Generator
 from concurrent.futures import FIRST_COMPLETED, Future, ThreadPoolExecutor, wait
 from contextlib import AbstractContextManager, contextmanager
+from dataclasses import dataclass, field
 from inspect import isawaitable
 from types import TracebackType
 from typing import (
     Any,
     AsyncContextManager,
     ContextManager,
     Generic,
@@ -257,22 +258,20 @@
         raise NotImplementedError
 
     @overload
     def call(
         self,
         func: Callable[[Unpack[PosArgsT]], Awaitable[T_Retval]],
         *args: Unpack[PosArgsT],
-    ) -> T_Retval:
-        ...
+    ) -> T_Retval: ...
 
     @overload
     def call(
         self, func: Callable[[Unpack[PosArgsT]], T_Retval], *args: Unpack[PosArgsT]
-    ) -> T_Retval:
-        ...
+    ) -> T_Retval: ...
 
     def call(
         self,
         func: Callable[[Unpack[PosArgsT]], Awaitable[T_Retval] | T_Retval],
         *args: Unpack[PosArgsT],
     ) -> T_Retval:
         """
@@ -289,25 +288,23 @@
 
     @overload
     def start_task_soon(
         self,
         func: Callable[[Unpack[PosArgsT]], Awaitable[T_Retval]],
         *args: Unpack[PosArgsT],
         name: object = None,
-    ) -> Future[T_Retval]:
-        ...
+    ) -> Future[T_Retval]: ...
 
     @overload
     def start_task_soon(
         self,
         func: Callable[[Unpack[PosArgsT]], T_Retval],
         *args: Unpack[PosArgsT],
         name: object = None,
-    ) -> Future[T_Retval]:
-        ...
+    ) -> Future[T_Retval]: ...
 
     def start_task_soon(
         self,
         func: Callable[[Unpack[PosArgsT]], Awaitable[T_Retval] | T_Retval],
         *args: Unpack[PosArgsT],
         name: object = None,
     ) -> Future[T_Retval]:
@@ -391,14 +388,71 @@
 
         .. versionadded:: 2.1
 
         """
         return _BlockingAsyncContextManager(cm, self)
 
 
+@dataclass
+class BlockingPortalProvider:
+    """
+    A manager for a blocking portal. Used as a context manager. The first thread to
+    enter this context manager causes a blocking portal to be started with the specific
+    parameters, and the last thread to exit causes the portal to be shut down. Thus,
+    there will be exactly one blocking portal running in this context as long as at
+    least one thread has entered this context manager.
+
+    The parameters are the same as for :func:`~anyio.run`.
+
+    :param backend: name of the backend
+    :param backend_options: backend options
+
+    .. versionadded:: 4.4
+    """
+
+    backend: str = "asyncio"
+    backend_options: dict[str, Any] | None = None
+    _lock: threading.Lock = field(init=False, default_factory=threading.Lock)
+    _leases: int = field(init=False, default=0)
+    _portal: BlockingPortal = field(init=False)
+    _portal_cm: AbstractContextManager[BlockingPortal] | None = field(
+        init=False, default=None
+    )
+
+    def __enter__(self) -> BlockingPortal:
+        with self._lock:
+            if self._portal_cm is None:
+                self._portal_cm = start_blocking_portal(
+                    self.backend, self.backend_options
+                )
+                self._portal = self._portal_cm.__enter__()
+
+            self._leases += 1
+            return self._portal
+
+    def __exit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> None:
+        portal_cm: AbstractContextManager[BlockingPortal] | None = None
+        with self._lock:
+            assert self._portal_cm
+            assert self._leases > 0
+            self._leases -= 1
+            if not self._leases:
+                portal_cm = self._portal_cm
+                self._portal_cm = None
+                del self._portal
+
+        if portal_cm:
+            portal_cm.__exit__(None, None, None)
+
+
 @contextmanager
 def start_blocking_portal(
     backend: str = "asyncio", backend_options: dict[str, Any] | None = None
 ) -> Generator[BlockingPortal, Any, None]:
     """
     Start a new event loop in a new thread and run a blocking portal in its main task.
```

### Comparing `anyio-4.3.0/src/anyio/lowlevel.py` & `anyio-4.4.0/src/anyio/lowlevel.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,20 +110,18 @@
         try:
             return _run_vars[token]
         except KeyError:
             run_vars = _run_vars[token] = {}
             return run_vars
 
     @overload
-    def get(self, default: D) -> T | D:
-        ...
+    def get(self, default: D) -> T | D: ...
 
     @overload
-    def get(self) -> T:
-        ...
+    def get(self) -> T: ...
 
     def get(
         self, default: D | Literal[_NoValueSet.NO_VALUE_SET] = NO_VALUE_SET
     ) -> T | D:
         try:
             return self._current_vars[self._name]
         except KeyError:
```

### Comparing `anyio-4.3.0/src/anyio/pytest_plugin.py` & `anyio-4.4.0/src/anyio/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/src/anyio/streams/buffered.py` & `anyio-4.4.0/src/anyio/streams/buffered.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/src/anyio/streams/file.py` & `anyio-4.4.0/src/anyio/streams/file.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/src/anyio/streams/memory.py` & `anyio-4.4.0/src/anyio/streams/memory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
+import warnings
 from collections import OrderedDict, deque
 from dataclasses import dataclass, field
 from types import TracebackType
 from typing import Generic, NamedTuple, TypeVar
 
 from .. import (
     BrokenResourceError,
     ClosedResourceError,
     EndOfStream,
     WouldBlock,
 )
+from .._core._testing import TaskInfo, get_current_task
 from ..abc import Event, ObjectReceiveStream, ObjectSendStream
 from ..lowlevel import checkpoint
 
 T_Item = TypeVar("T_Item")
 T_co = TypeVar("T_co", covariant=True)
 T_contra = TypeVar("T_contra", contravariant=True)
 
@@ -28,20 +30,26 @@
     #: number of tasks blocked on :meth:`MemoryObjectSendStream.send`
     tasks_waiting_send: int
     #: number of tasks blocked on :meth:`MemoryObjectReceiveStream.receive`
     tasks_waiting_receive: int
 
 
 @dataclass(eq=False)
+class MemoryObjectItemReceiver(Generic[T_Item]):
+    task_info: TaskInfo = field(init=False, default_factory=get_current_task)
+    item: T_Item = field(init=False)
+
+
+@dataclass(eq=False)
 class MemoryObjectStreamState(Generic[T_Item]):
     max_buffer_size: float = field()
     buffer: deque[T_Item] = field(init=False, default_factory=deque)
     open_send_channels: int = field(init=False, default=0)
     open_receive_channels: int = field(init=False, default=0)
-    waiting_receivers: OrderedDict[Event, list[T_Item]] = field(
+    waiting_receivers: OrderedDict[Event, MemoryObjectItemReceiver[T_Item]] = field(
         init=False, default_factory=OrderedDict
     )
     waiting_senders: OrderedDict[Event, T_Item] = field(
         init=False, default_factory=OrderedDict
     )
 
     def statistics(self) -> MemoryObjectStreamStatistics:
@@ -94,25 +102,25 @@
     async def receive(self) -> T_co:
         await checkpoint()
         try:
             return self.receive_nowait()
         except WouldBlock:
             # Add ourselves in the queue
             receive_event = Event()
-            container: list[T_co] = []
-            self._state.waiting_receivers[receive_event] = container
+            receiver = MemoryObjectItemReceiver[T_co]()
+            self._state.waiting_receivers[receive_event] = receiver
 
             try:
                 await receive_event.wait()
             finally:
                 self._state.waiting_receivers.pop(receive_event, None)
 
-            if container:
-                return container[0]
-            else:
+            try:
+                return receiver.item
+            except AttributeError:
                 raise EndOfStream
 
     def clone(self) -> MemoryObjectReceiveStream[T_co]:
         """
         Create a clone of this receive stream.
 
         Each clone can be closed separately. Only when all clones have been closed will
@@ -160,14 +168,22 @@
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
         self.close()
 
+    def __del__(self) -> None:
+        if not self._closed:
+            warnings.warn(
+                f"Unclosed <{self.__class__.__name__}>",
+                ResourceWarning,
+                source=self,
+            )
+
 
 @dataclass(eq=False)
 class MemoryObjectSendStream(Generic[T_contra], ObjectSendStream[T_contra]):
     _state: MemoryObjectStreamState[T_contra]
     _closed: bool = field(init=False, default=False)
 
     def __post_init__(self) -> None:
@@ -186,19 +202,22 @@
 
         """
         if self._closed:
             raise ClosedResourceError
         if not self._state.open_receive_channels:
             raise BrokenResourceError
 
-        if self._state.waiting_receivers:
-            receive_event, container = self._state.waiting_receivers.popitem(last=False)
-            container.append(item)
-            receive_event.set()
-        elif len(self._state.buffer) < self._state.max_buffer_size:
+        while self._state.waiting_receivers:
+            receive_event, receiver = self._state.waiting_receivers.popitem(last=False)
+            if not receiver.task_info.has_pending_cancellation():
+                receiver.item = item
+                receive_event.set()
+                return
+
+        if len(self._state.buffer) < self._state.max_buffer_size:
             self._state.buffer.append(item)
         else:
             raise WouldBlock
 
     async def send(self, item: T_contra) -> None:
         """
         Send an item to the stream.
@@ -221,15 +240,16 @@
             self._state.waiting_senders[send_event] = item
             try:
                 await send_event.wait()
             except BaseException:
                 self._state.waiting_senders.pop(send_event, None)
                 raise
 
-            if self._state.waiting_senders.pop(send_event, None):
+            if send_event in self._state.waiting_senders:
+                del self._state.waiting_senders[send_event]
                 raise BrokenResourceError from None
 
     def clone(self) -> MemoryObjectSendStream[T_contra]:
         """
         Create a clone of this send stream.
 
         Each clone can be closed separately. Only when all clones have been closed will
@@ -277,7 +297,15 @@
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
         self.close()
+
+    def __del__(self) -> None:
+        if not self._closed:
+            warnings.warn(
+                f"Unclosed <{self.__class__.__name__}>",
+                ResourceWarning,
+                source=self,
+            )
```

### Comparing `anyio-4.3.0/src/anyio/streams/stapled.py` & `anyio-4.4.0/src/anyio/streams/stapled.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/src/anyio/streams/text.py` & `anyio-4.4.0/src/anyio/streams/text.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/src/anyio/streams/tls.py` & `anyio-4.4.0/src/anyio/streams/tls.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/src/anyio/to_process.py` & `anyio-4.4.0/src/anyio/to_process.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/src/anyio/to_thread.py` & `anyio-4.4.0/src/anyio/to_thread.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/src/anyio.egg-info/PKG-INFO` & `anyio-4.4.0/src/anyio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyio
-Version: 4.3.0
+Version: 4.4.0
 Summary: High level compatibility layer for multiple asynchronous event loop implementations
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://anyio.readthedocs.io/en/latest/
 Project-URL: Changelog, https://anyio.readthedocs.io/en/stable/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/anyio
 Project-URL: Issue tracker, https://github.com/agronholm/anyio/issues
```

### Comparing `anyio-4.3.0/src/anyio.egg-info/SOURCES.txt` & `anyio-4.4.0/src/anyio.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

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
 .github/workflows/test-downstream.yml
 .github/workflows/test.yml
 docs/api.rst
@@ -85,14 +86,15 @@
 tests/test_signals.py
 tests/test_sockets.py
 tests/test_subprocesses.py
 tests/test_synchronization.py
 tests/test_taskgroups.py
 tests/test_to_process.py
 tests/test_to_thread.py
+tests/test_typedattr.py
 tests/streams/__init__.py
 tests/streams/test_buffered.py
 tests/streams/test_file.py
 tests/streams/test_memory.py
 tests/streams/test_stapled.py
 tests/streams/test_text.py
 tests/streams/test_tls.py
```

### Comparing `anyio-4.3.0/tests/conftest.py` & `anyio-4.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/tests/streams/test_buffered.py` & `anyio-4.4.0/tests/streams/test_buffered.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,23 +13,29 @@
     buffered_stream = BufferedByteReceiveStream(receive_stream)
     await send_stream.send(b"abcd")
     await send_stream.send(b"efgh")
     result = await buffered_stream.receive_exactly(8)
     assert result == b"abcdefgh"
     assert isinstance(result, bytes)
 
+    send_stream.close()
+    receive_stream.close()
+
 
 async def test_receive_exactly_incomplete() -> None:
     send_stream, receive_stream = create_memory_object_stream[bytes](1)
     buffered_stream = BufferedByteReceiveStream(receive_stream)
     await send_stream.send(b"abcd")
     await send_stream.aclose()
     with pytest.raises(IncompleteRead):
         await buffered_stream.receive_exactly(8)
 
+    send_stream.close()
+    receive_stream.close()
+
 
 async def test_receive_until() -> None:
     send_stream, receive_stream = create_memory_object_stream[bytes](2)
     buffered_stream = BufferedByteReceiveStream(receive_stream)
     await send_stream.send(b"abcd")
     await send_stream.send(b"efgh")
 
@@ -37,17 +43,23 @@
     assert result == b"abc"
     assert isinstance(result, bytes)
 
     result = await buffered_stream.receive_until(b"h", 10)
     assert result == b"fg"
     assert isinstance(result, bytes)
 
+    send_stream.close()
+    receive_stream.close()
+
 
 async def test_receive_until_incomplete() -> None:
     send_stream, receive_stream = create_memory_object_stream[bytes](1)
     buffered_stream = BufferedByteReceiveStream(receive_stream)
     await send_stream.send(b"abcd")
     await send_stream.aclose()
     with pytest.raises(IncompleteRead):
         assert await buffered_stream.receive_until(b"de", 10)
 
     assert buffered_stream.buffer == b"abcd"
+
+    send_stream.close()
+    receive_stream.close()
```

### Comparing `anyio-4.3.0/tests/streams/test_file.py` & `anyio-4.4.0/tests/streams/test_file.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/tests/streams/test_memory.py` & `anyio-4.4.0/tests/streams/test_memory.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import gc
 import sys
 from typing import NoReturn
 
 import pytest
 
 from anyio import (
     BrokenResourceError,
@@ -12,15 +13,15 @@
     EndOfStream,
     WouldBlock,
     create_memory_object_stream,
     create_task_group,
     fail_after,
     wait_all_tasks_blocked,
 )
-from anyio.abc import ObjectReceiveStream, ObjectSendStream
+from anyio.abc import ObjectReceiveStream, ObjectSendStream, TaskStatus
 from anyio.streams.memory import MemoryObjectReceiveStream, MemoryObjectSendStream
 
 if sys.version_info < (3, 11):
     from exceptiongroup import ExceptionGroup
 
 pytestmark = pytest.mark.anyio
 
@@ -48,14 +49,17 @@
         tg.start_soon(receiver)
         await wait_all_tasks_blocked()
         await send.send("hello")
         await send.send("anyio")
 
     assert received_objects == ["hello", "anyio"]
 
+    send.close()
+    receive.close()
+
 
 async def test_receive_then_send_nowait() -> None:
     async def receiver() -> None:
         received_objects.append(await receive.receive())
 
     send, receive = create_memory_object_stream[str](0)
     received_objects: list[str] = []
@@ -64,43 +68,55 @@
         tg.start_soon(receiver)
         await wait_all_tasks_blocked()
         send.send_nowait("hello")
         send.send_nowait("anyio")
 
     assert sorted(received_objects, reverse=True) == ["hello", "anyio"]
 
+    send.close()
+    receive.close()
+
 
 async def test_send_then_receive_nowait() -> None:
     send, receive = create_memory_object_stream[str](0)
     async with create_task_group() as tg:
         tg.start_soon(send.send, "hello")
         await wait_all_tasks_blocked()
         assert receive.receive_nowait() == "hello"
 
+    send.close()
+    receive.close()
+
 
 async def test_send_is_unblocked_after_receive_nowait() -> None:
     send, receive = create_memory_object_stream[str](1)
     send.send_nowait("hello")
 
     with fail_after(1):
         async with create_task_group() as tg:
             tg.start_soon(send.send, "anyio")
             await wait_all_tasks_blocked()
             assert receive.receive_nowait() == "hello"
 
     assert receive.receive_nowait() == "anyio"
 
+    send.close()
+    receive.close()
+
 
 async def test_send_nowait_then_receive_nowait() -> None:
     send, receive = create_memory_object_stream[str](2)
     send.send_nowait("hello")
     send.send_nowait("anyio")
     assert receive.receive_nowait() == "hello"
     assert receive.receive_nowait() == "anyio"
 
+    send.close()
+    receive.close()
+
 
 async def test_iterate() -> None:
     async def receiver() -> None:
         async for item in receive:
             received_objects.append(item)
 
     send, receive = create_memory_object_stream[str]()
@@ -109,66 +125,84 @@
         tg.start_soon(receiver)
         await send.send("hello")
         await send.send("anyio")
         await send.aclose()
 
     assert received_objects == ["hello", "anyio"]
 
+    send.close()
+    receive.close()
+
 
 async def test_receive_send_closed_send_stream() -> None:
     send, receive = create_memory_object_stream[None]()
     await send.aclose()
     with pytest.raises(EndOfStream):
         receive.receive_nowait()
 
     with pytest.raises(ClosedResourceError):
         await send.send(None)
 
+    receive.close()
+
 
 async def test_receive_send_closed_receive_stream() -> None:
     send, receive = create_memory_object_stream[None]()
     await receive.aclose()
     with pytest.raises(ClosedResourceError):
         receive.receive_nowait()
 
     with pytest.raises(BrokenResourceError):
         await send.send(None)
 
+    send.close()
+
 
 async def test_cancel_receive() -> None:
     send, receive = create_memory_object_stream[str]()
     async with create_task_group() as tg:
         tg.start_soon(receive.receive)
         await wait_all_tasks_blocked()
         tg.cancel_scope.cancel()
 
     with pytest.raises(WouldBlock):
         send.send_nowait("hello")
 
+    send.close()
+    receive.close()
+
 
 async def test_cancel_send() -> None:
     send, receive = create_memory_object_stream[str]()
     async with create_task_group() as tg:
         tg.start_soon(send.send, "hello")
         await wait_all_tasks_blocked()
         tg.cancel_scope.cancel()
 
     with pytest.raises(WouldBlock):
         receive.receive_nowait()
 
+    send.close()
+    receive.close()
+
 
 async def test_clone() -> None:
     send1, receive1 = create_memory_object_stream[str](1)
     send2 = send1.clone()
     receive2 = receive1.clone()
     await send1.aclose()
     await receive1.aclose()
     send2.send_nowait("hello")
     assert receive2.receive_nowait() == "hello"
 
+    send1.close()
+    receive1.close()
+    send2.close()
+    receive2.close()
+
 
 async def test_clone_closed() -> None:
     send, receive = create_memory_object_stream[NoReturn](1)
     await send.aclose()
     await receive.aclose()
     pytest.raises(ClosedResourceError, send.clone)
     pytest.raises(ClosedResourceError, receive.clone)
@@ -181,33 +215,43 @@
             tg.start_soon(receive.receive)
             await wait_all_tasks_blocked()
             await send.aclose()
 
     assert len(exc.value.exceptions) == 1
     assert isinstance(exc.value.exceptions[0], EndOfStream)
 
+    send.close()
+    receive.close()
+
 
 async def test_close_receive_while_sending() -> None:
-    send, receive = create_memory_object_stream[str](0)
+    # We send None here as a regression test for #731
+    send, receive = create_memory_object_stream[None](0)
     with pytest.raises(ExceptionGroup) as exc:
         async with create_task_group() as tg:
-            tg.start_soon(send.send, "hello")
+            tg.start_soon(send.send, None)
             await wait_all_tasks_blocked()
             await receive.aclose()
 
     assert len(exc.value.exceptions) == 1
     assert isinstance(exc.value.exceptions[0], BrokenResourceError)
 
+    send.close()
+    receive.close()
+
 
 async def test_receive_after_send_closed() -> None:
     send, receive = create_memory_object_stream[str](1)
     await send.send("hello")
     await send.aclose()
     assert await receive.receive() == "hello"
 
+    send.close()
+    receive.close()
+
 
 async def test_receive_when_cancelled() -> None:
     """
     Test that calling receive() in a cancelled scope prevents it from going through with
     the operation.
 
     """
@@ -221,14 +265,17 @@
         with CancelScope() as scope:
             scope.cancel()
             await receive.receive()
 
         assert await receive.receive() == "hello"
         assert await receive.receive() == "world"
 
+    send.close()
+    receive.close()
+
 
 async def test_send_when_cancelled() -> None:
     """
     Test that calling send() in a cancelled scope prevents it from going through with
     the operation.
 
     """
@@ -244,56 +291,86 @@
             scope.cancel()
             await send.send("hello")
 
         await send.send("world")
 
     assert received == ["world"]
 
+    send.close()
+    receive.close()
+
 
 async def test_cancel_during_receive() -> None:
     """
     Test that cancelling a pending receive() operation does not cause an item in the
     stream to be lost.
 
     """
-    receiver_scope = None
 
-    async def scoped_receiver() -> None:
-        nonlocal receiver_scope
-        with CancelScope() as receiver_scope:
+    async def scoped_receiver(task_status: TaskStatus[CancelScope]) -> None:
+        with CancelScope() as cancel_scope:
+            task_status.started(cancel_scope)
             received.append(await receive.receive())
 
-        assert receiver_scope.cancel_called
+        assert cancel_scope.cancel_called
 
     received: list[str] = []
     send, receive = create_memory_object_stream[str]()
-    async with create_task_group() as tg:
-        tg.start_soon(scoped_receiver)
-        await wait_all_tasks_blocked()
-        send.send_nowait("hello")
-        assert receiver_scope is not None
-        receiver_scope.cancel()
+    with send, receive:
+        async with create_task_group() as tg:
+            receiver_scope = await tg.start(scoped_receiver)
+            await wait_all_tasks_blocked()
+            send.send_nowait("hello")
+            receiver_scope.cancel()
 
     assert received == ["hello"]
 
 
+async def test_cancel_during_receive_buffered() -> None:
+    """
+    Test that sending an item to a memory object stream when the receiver that is next
+    in line has been cancelled will not result in the item being lost.
+    """
+
+    async def scoped_receiver(
+        receive: MemoryObjectReceiveStream[str], task_status: TaskStatus[CancelScope]
+    ) -> None:
+        with CancelScope() as cancel_scope:
+            task_status.started(cancel_scope)
+            await receive.receive()
+
+    send, receive = create_memory_object_stream[str](1)
+    with send, receive:
+        async with create_task_group() as tg:
+            cancel_scope = await tg.start(scoped_receiver, receive)
+            await wait_all_tasks_blocked()
+            cancel_scope.cancel()
+            send.send_nowait("item")
+
+        # Since the item was not sent to the cancelled task, it should be available here
+        assert receive.receive_nowait() == "item"
+
+
 async def test_close_receive_after_send() -> None:
     async def send() -> None:
         async with send_stream:
             await send_stream.send("test")
 
     async def receive() -> None:
         async with receive_stream:
             assert await receive_stream.receive() == "test"
 
     send_stream, receive_stream = create_memory_object_stream[str]()
     async with create_task_group() as tg:
         tg.start_soon(send)
         tg.start_soon(receive)
 
+    send_stream.close()
+    receive_stream.close()
+
 
 async def test_statistics() -> None:
     send_stream, receive_stream = create_memory_object_stream[None](1)
     streams: list[MemoryObjectReceiveStream[None] | MemoryObjectSendStream[None]] = [
         send_stream,
         receive_stream,
     ]
@@ -343,14 +420,17 @@
 
             receive_stream.receive_nowait()
 
         assert stream.statistics().current_buffer_used == 0
         assert stream.statistics().tasks_waiting_send == 0
         assert stream.statistics().tasks_waiting_receive == 0
 
+    send_stream.close()
+    receive_stream.close()
+
 
 async def test_sync_close() -> None:
     send_stream, receive_stream = create_memory_object_stream[None](1)
     with send_stream, receive_stream:
         pass
 
     with pytest.raises(ClosedResourceError):
@@ -370,11 +450,51 @@
     """
     send, receive = create_memory_object_stream[float]()
     receive1: MemoryObjectReceiveStream[complex] = receive  # noqa: F841
     receive2: ObjectReceiveStream[complex] = receive  # noqa: F841
     send1: MemoryObjectSendStream[int] = send  # noqa: F841
     send2: ObjectSendStream[int] = send  # noqa: F841
 
+    send.close()
+    receive.close()
+
 
 async def test_deprecated_item_type_parameter() -> None:
     with pytest.warns(DeprecationWarning, match="item_type argument has been "):
-        create_memory_object_stream(item_type=int)
+        send, receive = create_memory_object_stream(item_type=int)  # type: ignore[var-annotated]
+
+        send.close()
+        receive.close()
+
+
+async def test_not_closed_warning() -> None:
+    send, receive = create_memory_object_stream[int]()
+
+    with pytest.warns(ResourceWarning, match="Unclosed <MemoryObjectSendStream>"):
+        del send
+        gc.collect()
+
+    with pytest.warns(ResourceWarning, match="Unclosed <MemoryObjectReceiveStream>"):
+        del receive
+        gc.collect()
+
+
+@pytest.mark.parametrize("anyio_backend", ["asyncio"], indirect=True)
+async def test_send_to_natively_cancelled_receiver() -> None:
+    """
+    Test that if a task waiting on receive.receive() is cancelled and then another
+    task sends an item, said item is not delivered to the task with a pending
+    cancellation, but rather to the next one in line.
+
+    """
+    from asyncio import CancelledError, create_task
+
+    send, receive = create_memory_object_stream[str](1)
+    with send, receive:
+        receive_task = create_task(receive.receive())
+        await wait_all_tasks_blocked()  # ensure that the task is waiting to receive
+        receive_task.cancel()
+        send.send_nowait("hello")
+        with pytest.raises(CancelledError):
+            await receive_task
+
+        assert receive.receive_nowait() == "hello"
```

### Comparing `anyio-4.3.0/tests/streams/test_stapled.py` & `anyio-4.4.0/tests/streams/test_stapled.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/tests/streams/test_text.py` & `anyio-4.4.0/tests/streams/test_text.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,44 +18,59 @@
     await send_stream.send(b"\xc3\xa5\xc3\xa4\xc3")  # ends with half of the "ö" letter
     assert await text_stream.receive() == "åä"
 
     # Send the missing byte for "ö"
     await send_stream.send(b"\xb6")
     assert await text_stream.receive() == "ö"
 
+    send_stream.close()
+    receive_stream.close()
+
 
 async def test_send() -> None:
     send_stream, receive_stream = create_memory_object_stream[bytes](1)
     text_stream = TextSendStream(send_stream)
     await text_stream.send("åäö")
     assert await receive_stream.receive() == b"\xc3\xa5\xc3\xa4\xc3\xb6"
 
+    send_stream.close()
+    receive_stream.close()
+
 
 @pytest.mark.xfail(
     platform.python_implementation() == "PyPy" and sys.pypy_version_info < (7, 3, 2),  # type: ignore[attr-defined]
     reason="PyPy has a bug in its incremental UTF-8 decoder (#3274)",
 )
 async def test_receive_encoding_error() -> None:
     send_stream, receive_stream = create_memory_object_stream[bytes](1)
     text_stream = TextReceiveStream(receive_stream, errors="replace")
     await send_stream.send(b"\xe5\xe4\xf6")  # "åäö" in latin-1
     assert await text_stream.receive() == "���"
 
+    send_stream.close()
+    receive_stream.close()
+
 
 async def test_send_encoding_error() -> None:
     send_stream, receive_stream = create_memory_object_stream[bytes](1)
     text_stream = TextSendStream(send_stream, encoding="iso-8859-1", errors="replace")
     await text_stream.send("€")
     assert await receive_stream.receive() == b"?"
 
+    send_stream.close()
+    receive_stream.close()
+
 
 async def test_bidirectional_stream() -> None:
     send_stream, receive_stream = create_memory_object_stream[bytes](1)
     stapled_stream = StapledObjectStream(send_stream, receive_stream)
     text_stream = TextStream(stapled_stream)
 
     await text_stream.send("åäö")
     assert await receive_stream.receive() == b"\xc3\xa5\xc3\xa4\xc3\xb6"
 
     await send_stream.send(b"\xc3\xa6\xc3\xb8")
     assert await text_stream.receive() == "æø"
     assert text_stream.extra_attributes == {}
+
+    send_stream.close()
+    receive_stream.close()
```

### Comparing `anyio-4.3.0/tests/streams/test_tls.py` & `anyio-4.4.0/tests/streams/test_tls.py`

 * *Files 0% similar despite different names*

```diff
@@ -381,14 +381,17 @@
         send1, receive1 = create_memory_object_stream[bytes]()
         client_stream = StapledObjectStream(send1, receive1)
         mocker.patch.object(TLSStream, "_call_sslobject_method")
         tls_stream = await TLSStream.wrap(client_stream)
         ssl_context = tls_stream.extra(TLSAttribute.ssl_object).context
         assert not ssl_context.options & ssl.OP_IGNORE_UNEXPECTED_EOF
 
+        send1.close()
+        receive1.close()
+
 
 class TestTLSListener:
     async def test_handshake_fail(
         self, server_context: ssl.SSLContext, caplog: pytest.LogCaptureFixture
     ) -> None:
         def handler(stream: object) -> NoReturn:
             pytest.fail("This function should never be called in this scenario")
```

### Comparing `anyio-4.3.0/tests/test_debugging.py` & `anyio-4.4.0/tests/test_debugging.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         "task1",
         "task2",
         "tests.test_debugging.test_get_running_tasks.<locals>.inspect",
     ]
     for task, expected_name in zip(task_infos, expected_names):
         assert task.parent_id == host_task.id
         assert task.name == expected_name
-        assert repr(task) == f"TaskInfo(id={task.id}, name={expected_name!r})"
+        assert repr(task).endswith(f"TaskInfo(id={task.id}, name={expected_name!r})")
 
 
 @pytest.mark.skipif(
     sys.version_info >= (3, 11),
     reason="Generator based coroutines have been removed in Python 3.11",
 )
 @pytest.mark.filterwarnings(
```

### Comparing `anyio-4.3.0/tests/test_eventloop.py` & `anyio-4.4.0/tests/test_eventloop.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import asyncio
 import math
 from asyncio import get_running_loop
 from unittest.mock import AsyncMock
 
 import pytest
+from pytest import MonkeyPatch
 from pytest_mock.plugin import MockerFixture
 
 from anyio import run, sleep_forever, sleep_until
 
 pytestmark = pytest.mark.anyio
 fake_current_time = 1620581544.0
 
@@ -51,14 +52,22 @@
     def test_debug(self) -> None:
         async def main() -> bool:
             return get_running_loop().get_debug()
 
         debug = run(main, backend="asyncio", backend_options={"debug": True})
         assert debug is True
 
+    def test_debug_via_env(self, monkeypatch: MonkeyPatch) -> None:
+        async def main() -> bool:
+            return get_running_loop().get_debug()
+
+        monkeypatch.setenv("PYTHONASYNCIODEBUG", "1")
+        debug = run(main, backend="asyncio")
+        assert debug is True
+
     def test_loop_factory(self) -> None:
         async def main() -> type:
             return type(get_running_loop())
 
         uvloop = pytest.importorskip("uvloop", reason="uvloop not installed")
         loop_class = run(
             main,
```

### Comparing `anyio-4.3.0/tests/test_fileio.py` & `anyio-4.4.0/tests/test_fileio.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/tests/test_from_thread.py` & `anyio-4.4.0/tests/test_from_thread.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/tests/test_lowlevel.py` & `anyio-4.4.0/tests/test_lowlevel.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/tests/test_pytest_plugin.py` & `anyio-4.4.0/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/tests/test_signals.py` & `anyio-4.4.0/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/tests/test_sockets.py` & `anyio-4.4.0/tests/test_sockets.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,4067 +37,4125 @@
 00000240: 6972 2069 6d70 6f72 7420 5465 6d70 5061  ir import TempPa
 00000250: 7468 4661 6374 6f72 790a 0a66 726f 6d20  thFactory..from 
 00000260: 616e 7969 6f20 696d 706f 7274 2028 0a20  anyio import (. 
 00000270: 2020 2042 726f 6b65 6e52 6573 6f75 7263     BrokenResourc
 00000280: 6545 7272 6f72 2c0a 2020 2020 4275 7379  eError,.    Busy
 00000290: 5265 736f 7572 6365 4572 726f 722c 0a20  ResourceError,. 
 000002a0: 2020 2043 6c6f 7365 6452 6573 6f75 7263     ClosedResourc
-000002b0: 6545 7272 6f72 2c0a 2020 2020 4576 656e  eError,.    Even
-000002c0: 742c 0a20 2020 2054 7970 6564 4174 7472  t,.    TypedAttr
-000002d0: 6962 7574 654c 6f6f 6b75 7045 7272 6f72  ibuteLookupError
-000002e0: 2c0a 2020 2020 636f 6e6e 6563 745f 7463  ,.    connect_tc
-000002f0: 702c 0a20 2020 2063 6f6e 6e65 6374 5f75  p,.    connect_u
-00000300: 6e69 782c 0a20 2020 2063 7265 6174 655f  nix,.    create_
-00000310: 636f 6e6e 6563 7465 645f 7564 705f 736f  connected_udp_so
-00000320: 636b 6574 2c0a 2020 2020 6372 6561 7465  cket,.    create
-00000330: 5f63 6f6e 6e65 6374 6564 5f75 6e69 785f  _connected_unix_
-00000340: 6461 7461 6772 616d 5f73 6f63 6b65 742c  datagram_socket,
-00000350: 0a20 2020 2063 7265 6174 655f 7461 736b  .    create_task
-00000360: 5f67 726f 7570 2c0a 2020 2020 6372 6561  _group,.    crea
-00000370: 7465 5f74 6370 5f6c 6973 7465 6e65 722c  te_tcp_listener,
-00000380: 0a20 2020 2063 7265 6174 655f 7564 705f  .    create_udp_
-00000390: 736f 636b 6574 2c0a 2020 2020 6372 6561  socket,.    crea
-000003a0: 7465 5f75 6e69 785f 6461 7461 6772 616d  te_unix_datagram
-000003b0: 5f73 6f63 6b65 742c 0a20 2020 2063 7265  _socket,.    cre
-000003c0: 6174 655f 756e 6978 5f6c 6973 7465 6e65  ate_unix_listene
-000003d0: 722c 0a20 2020 2066 6169 6c5f 6166 7465  r,.    fail_afte
-000003e0: 722c 0a20 2020 2067 6574 6164 6472 696e  r,.    getaddrin
-000003f0: 666f 2c0a 2020 2020 6765 746e 616d 6569  fo,.    getnamei
-00000400: 6e66 6f2c 0a20 2020 206d 6f76 655f 6f6e  nfo,.    move_on
-00000410: 5f61 6674 6572 2c0a 2020 2020 736c 6565  _after,.    slee
-00000420: 702c 0a20 2020 2077 6169 745f 616c 6c5f  p,.    wait_all_
-00000430: 7461 736b 735f 626c 6f63 6b65 642c 0a29  tasks_blocked,.)
-00000440: 0a66 726f 6d20 616e 7969 6f2e 6162 6320  .from anyio.abc 
-00000450: 696d 706f 7274 2028 0a20 2020 2049 5053  import (.    IPS
-00000460: 6f63 6b41 6464 7254 7970 652c 0a20 2020  ockAddrType,.   
-00000470: 204c 6973 7465 6e65 722c 0a20 2020 2053   Listener,.    S
-00000480: 6f63 6b65 7441 7474 7269 6275 7465 2c0a  ocketAttribute,.
-00000490: 2020 2020 536f 636b 6574 4c69 7374 656e      SocketListen
-000004a0: 6572 2c0a 2020 2020 536f 636b 6574 5374  er,.    SocketSt
-000004b0: 7265 616d 2c0a 290a 6672 6f6d 2061 6e79  ream,.).from any
-000004c0: 696f 2e73 7472 6561 6d73 2e73 7461 706c  io.streams.stapl
-000004d0: 6564 2069 6d70 6f72 7420 4d75 6c74 694c  ed import MultiL
-000004e0: 6973 7465 6e65 720a 0a69 6620 7379 732e  istener..if sys.
-000004f0: 7665 7273 696f 6e5f 696e 666f 203c 2028  version_info < (
-00000500: 332c 2031 3129 3a0a 2020 2020 6672 6f6d  3, 11):.    from
-00000510: 2065 7863 6570 7469 6f6e 6772 6f75 7020   exceptiongroup 
-00000520: 696d 706f 7274 2045 7863 6570 7469 6f6e  import Exception
-00000530: 4772 6f75 700a 0a66 726f 6d20 7479 7069  Group..from typi
-00000540: 6e67 2069 6d70 6f72 7420 4c69 7465 7261  ng import Litera
-00000550: 6c0a 0a41 6e79 4950 4164 6472 6573 7346  l..AnyIPAddressF
-00000560: 616d 696c 7920 3d20 4c69 7465 7261 6c5b  amily = Literal[
-00000570: 0a20 2020 2041 6464 7265 7373 4661 6d69  .    AddressFami
-00000580: 6c79 2e41 465f 554e 5350 4543 2c20 4164  ly.AF_UNSPEC, Ad
-00000590: 6472 6573 7346 616d 696c 792e 4146 5f49  dressFamily.AF_I
-000005a0: 4e45 542c 2041 6464 7265 7373 4661 6d69  NET, AddressFami
-000005b0: 6c79 2e41 465f 494e 4554 360a 5d0a 0a70  ly.AF_INET6.]..p
-000005c0: 7974 6573 746d 6172 6b20 3d20 7079 7465  ytestmark = pyte
-000005d0: 7374 2e6d 6172 6b2e 616e 7969 6f0a 0a23  st.mark.anyio..#
-000005e0: 2049 6620 6120 736f 636b 6574 2063 616e   If a socket can
-000005f0: 2062 696e 6420 746f 203a 3a31 2c20 7468   bind to ::1, th
-00000600: 6520 6375 7272 656e 7420 656e 7669 726f  e current enviro
-00000610: 6e6d 656e 7420 6861 7320 4950 7636 2070  nment has IPv6 p
-00000620: 726f 7065 726c 7920 636f 6e66 6967 7572  roperly configur
-00000630: 6564 0a68 6173 5f69 7076 3620 3d20 4661  ed.has_ipv6 = Fa
-00000640: 6c73 650a 6966 2073 6f63 6b65 742e 6861  lse.if socket.ha
-00000650: 735f 6970 7636 3a0a 2020 2020 7472 793a  s_ipv6:.    try:
-00000660: 0a20 2020 2020 2020 2073 203d 2073 6f63  .        s = soc
-00000670: 6b65 742e 736f 636b 6574 2841 6464 7265  ket.socket(Addre
-00000680: 7373 4661 6d69 6c79 2e41 465f 494e 4554  ssFamily.AF_INET
-00000690: 3629 0a20 2020 2020 2020 2074 7279 3a0a  6).        try:.
-000006a0: 2020 2020 2020 2020 2020 2020 732e 6269              s.bi
-000006b0: 6e64 2828 223a 3a31 222c 2030 2929 0a20  nd(("::1", 0)). 
-000006c0: 2020 2020 2020 2066 696e 616c 6c79 3a0a         finally:.
-000006d0: 2020 2020 2020 2020 2020 2020 732e 636c              s.cl
-000006e0: 6f73 6528 290a 2020 2020 2020 2020 2020  ose().          
-000006f0: 2020 6465 6c20 730a 2020 2020 6578 6365    del s.    exce
-00000700: 7074 204f 5345 7272 6f72 3a0a 2020 2020  pt OSError:.    
-00000710: 2020 2020 7061 7373 0a20 2020 2065 6c73      pass.    els
-00000720: 653a 0a20 2020 2020 2020 2068 6173 5f69  e:.        has_i
-00000730: 7076 3620 3d20 5472 7565 0a0a 736b 6970  pv6 = True..skip
-00000740: 5f69 7076 365f 6d61 726b 203d 2070 7974  _ipv6_mark = pyt
-00000750: 6573 742e 6d61 726b 2e73 6b69 7069 6628  est.mark.skipif(
-00000760: 6e6f 7420 6861 735f 6970 7636 2c20 7265  not has_ipv6, re
-00000770: 6173 6f6e 3d22 4950 7636 2069 7320 6e6f  ason="IPv6 is no
-00000780: 7420 6176 6169 6c61 626c 6522 290a 0a0a  t available")...
-00000790: 4070 7974 6573 742e 6669 7874 7572 650a  @pytest.fixture.
-000007a0: 6465 6620 6661 6b65 5f6c 6f63 616c 686f  def fake_localho
-000007b0: 7374 5f64 6e73 286d 6f6e 6b65 7970 6174  st_dns(monkeypat
-000007c0: 6368 3a20 4d6f 6e6b 6579 5061 7463 6829  ch: MonkeyPatch)
-000007d0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 6465   -> None:.    de
-000007e0: 6620 6661 6b65 5f67 6574 6164 6472 696e  f fake_getaddrin
-000007f0: 666f 282a 6172 6773 3a20 416e 792c 202a  fo(*args: Any, *
-00000800: 2a6b 7761 7267 733a 2041 6e79 2920 2d3e  *kwargs: Any) ->
-00000810: 206f 626a 6563 743a 0a20 2020 2020 2020   object:.       
-00000820: 2023 204d 616b 6520 6974 2072 6574 7572   # Make it retur
-00000830: 6e20 4950 7634 2061 6464 7265 7373 6573  n IPv4 addresses
-00000840: 2066 6972 7374 2073 6f20 7765 2063 616e   first so we can
-00000850: 2074 6573 7420 7468 6520 4950 7636 2070   test the IPv6 p
-00000860: 7265 6665 7265 6e63 650a 2020 2020 2020  reference.      
-00000870: 2020 7265 7375 6c74 7320 3d20 7265 616c    results = real
-00000880: 5f67 6574 6164 6472 696e 666f 282a 6172  _getaddrinfo(*ar
-00000890: 6773 2c20 2a2a 6b77 6172 6773 290a 2020  gs, **kwargs).  
-000008a0: 2020 2020 2020 7265 7475 726e 2073 6f72        return sor
-000008b0: 7465 6428 7265 7375 6c74 732c 206b 6579  ted(results, key
-000008c0: 3d6c 616d 6264 6120 6974 656d 3a20 6974  =lambda item: it
-000008d0: 656d 5b30 5d29 0a0a 2020 2020 7265 616c  em[0])..    real
-000008e0: 5f67 6574 6164 6472 696e 666f 203d 2073  _getaddrinfo = s
-000008f0: 6f63 6b65 742e 6765 7461 6464 7269 6e66  ocket.getaddrinf
-00000900: 6f0a 2020 2020 6d6f 6e6b 6579 7061 7463  o.    monkeypatc
-00000910: 682e 7365 7461 7474 7228 2273 6f63 6b65  h.setattr("socke
-00000920: 742e 6765 7461 6464 7269 6e66 6f22 2c20  t.getaddrinfo", 
-00000930: 6661 6b65 5f67 6574 6164 6472 696e 666f  fake_getaddrinfo
-00000940: 290a 0a0a 4070 7974 6573 742e 6669 7874  )...@pytest.fixt
-00000950: 7572 6528 0a20 2020 2070 6172 616d 733d  ure(.    params=
-00000960: 5b0a 2020 2020 2020 2020 7079 7465 7374  [.        pytest
-00000970: 2e70 6172 616d 2841 6464 7265 7373 4661  .param(AddressFa
-00000980: 6d69 6c79 2e41 465f 494e 4554 2c20 6964  mily.AF_INET, id
-00000990: 3d22 6970 7634 2229 2c0a 2020 2020 2020  ="ipv4"),.      
-000009a0: 2020 7079 7465 7374 2e70 6172 616d 2841    pytest.param(A
-000009b0: 6464 7265 7373 4661 6d69 6c79 2e41 465f  ddressFamily.AF_
-000009c0: 494e 4554 362c 2069 643d 2269 7076 3622  INET6, id="ipv6"
-000009d0: 2c20 6d61 726b 733d 5b73 6b69 705f 6970  , marks=[skip_ip
-000009e0: 7636 5f6d 6172 6b5d 292c 0a20 2020 205d  v6_mark]),.    ]
-000009f0: 0a29 0a64 6566 2066 616d 696c 7928 7265  .).def family(re
-00000a00: 7175 6573 743a 2053 7562 5265 7175 6573  quest: SubReques
-00000a10: 7429 202d 3e20 416e 7949 5041 6464 7265  t) -> AnyIPAddre
-00000a20: 7373 4661 6d69 6c79 3a0a 2020 2020 7265  ssFamily:.    re
-00000a30: 7475 726e 2072 6571 7565 7374 2e70 6172  turn request.par
-00000a40: 616d 0a0a 0a40 7079 7465 7374 2e66 6978  am...@pytest.fix
-00000a50: 7475 7265 0a64 6566 2063 6865 636b 5f61  ture.def check_a
-00000a60: 7379 6e63 696f 5f62 7567 2861 6e79 696f  syncio_bug(anyio
-00000a70: 5f62 6163 6b65 6e64 5f6e 616d 653a 2073  _backend_name: s
-00000a80: 7472 2c20 6661 6d69 6c79 3a20 416e 7949  tr, family: AnyI
-00000a90: 5041 6464 7265 7373 4661 6d69 6c79 2920  PAddressFamily) 
-00000aa0: 2d3e 204e 6f6e 653a 0a20 2020 2069 6620  -> None:.    if 
-00000ab0: 280a 2020 2020 2020 2020 616e 7969 6f5f  (.        anyio_
-00000ac0: 6261 636b 656e 645f 6e61 6d65 203d 3d20  backend_name == 
-00000ad0: 2261 7379 6e63 696f 220a 2020 2020 2020  "asyncio".      
-00000ae0: 2020 616e 6420 7379 732e 706c 6174 666f    and sys.platfo
-00000af0: 726d 203d 3d20 2277 696e 3332 220a 2020  rm == "win32".  
-00000b00: 2020 2020 2020 616e 6420 6661 6d69 6c79        and family
-00000b10: 203d 3d20 4164 6472 6573 7346 616d 696c   == AddressFamil
-00000b20: 792e 4146 5f49 4e45 5436 0a20 2020 2029  y.AF_INET6.    )
-00000b30: 3a0a 2020 2020 2020 2020 696d 706f 7274  :.        import
-00000b40: 2061 7379 6e63 696f 0a0a 2020 2020 2020   asyncio..      
-00000b50: 2020 706f 6c69 6379 203d 2061 7379 6e63    policy = async
-00000b60: 696f 2e67 6574 5f65 7665 6e74 5f6c 6f6f  io.get_event_loo
-00000b70: 705f 706f 6c69 6379 2829 0a20 2020 2020  p_policy().     
-00000b80: 2020 2069 6620 706f 6c69 6379 2e5f 5f63     if policy.__c
-00000b90: 6c61 7373 5f5f 2e5f 5f6e 616d 655f 5f20  lass__.__name__ 
-00000ba0: 3d3d 2022 5769 6e64 6f77 7350 726f 6163  == "WindowsProac
-00000bb0: 746f 7245 7665 6e74 4c6f 6f70 506f 6c69  torEventLoopPoli
-00000bc0: 6379 223a 0a20 2020 2020 2020 2020 2020  cy":.           
-00000bd0: 2070 7974 6573 742e 736b 6970 2822 446f   pytest.skip("Do
-00000be0: 6573 206e 6f74 2077 6f72 6b20 6475 6520  es not work due 
-00000bf0: 746f 2061 206b 6e6f 776e 2062 7567 2028  to a known bug (
-00000c00: 3339 3134 3829 2229 0a0a 0a5f 5420 3d20  39148)")..._T = 
-00000c10: 5479 7065 5661 7228 225f 5422 290a 0a0a  TypeVar("_T")...
-00000c20: 6465 6620 5f69 6465 6e74 6974 7928 763a  def _identity(v:
-00000c30: 205f 5429 202d 3e20 5f54 3a0a 2020 2020   _T) -> _T:.    
-00000c40: 7265 7475 726e 2076 0a0a 0a23 2020 5f50  return v...#  _P
-00000c50: 726f 6163 746f 7242 6173 6550 6970 6554  roactorBasePipeT
-00000c60: 7261 6e73 706f 7274 2e61 626f 7274 2829  ransport.abort()
-00000c70: 2061 6674 6572 205f 5072 6f61 6374 6f72   after _Proactor
-00000c80: 4261 7365 5069 7065 5472 616e 7370 6f72  BasePipeTranspor
-00000c90: 742e 636c 6f73 6528 290a 2320 646f 6573  t.close().# does
-00000ca0: 206e 6f74 2063 616e 6365 6c20 7772 6974   not cancel writ
-00000cb0: 6573 3a20 6874 7470 733a 2f2f 6275 6773  es: https://bugs
-00000cc0: 2e70 7974 686f 6e2e 6f72 672f 6973 7375  .python.org/issu
-00000cd0: 6534 3434 3238 0a5f 6967 6e6f 7265 5f77  e44428._ignore_w
-00000ce0: 696e 3332 5f72 6573 6f75 7263 655f 7761  in32_resource_wa
-00000cf0: 726e 696e 6773 203d 2028 0a20 2020 2070  rnings = (.    p
-00000d00: 7974 6573 742e 6d61 726b 2e66 696c 7465  ytest.mark.filte
-00000d10: 7277 6172 6e69 6e67 7328 0a20 2020 2020  rwarnings(.     
-00000d20: 2020 2022 6967 6e6f 7265 3a75 6e63 6c6f     "ignore:unclo
-00000d30: 7365 6420 3c73 6f63 6b65 742e 736f 636b  sed <socket.sock
-00000d40: 6574 3a52 6573 6f75 7263 6557 6172 6e69  et:ResourceWarni
-00000d50: 6e67 222c 0a20 2020 2020 2020 2022 6967  ng",.        "ig
-00000d60: 6e6f 7265 3a75 6e63 6c6f 7365 6420 7472  nore:unclosed tr
-00000d70: 616e 7370 6f72 7420 3c5f 5072 6f61 6374  ansport <_Proact
-00000d80: 6f72 536f 636b 6574 5472 616e 7370 6f72  orSocketTranspor
-00000d90: 7420 636c 6f73 696e 673a 5265 736f 7572  t closing:Resour
-00000da0: 6365 5761 726e 696e 6722 2c0a 2020 2020  ceWarning",.    
-00000db0: 290a 2020 2020 6966 2073 7973 2e70 6c61  ).    if sys.pla
-00000dc0: 7466 6f72 6d20 3d3d 2022 7769 6e33 3222  tform == "win32"
-00000dd0: 0a20 2020 2065 6c73 6520 5f69 6465 6e74  .    else _ident
-00000de0: 6974 790a 290a 0a0a 405f 6967 6e6f 7265  ity.)...@_ignore
-00000df0: 5f77 696e 3332 5f72 6573 6f75 7263 655f  _win32_resource_
-00000e00: 7761 726e 696e 6773 2020 2320 7479 7065  warnings  # type
-00000e10: 3a20 6967 6e6f 7265 5b6f 7065 7261 746f  : ignore[operato
-00000e20: 725d 0a63 6c61 7373 2054 6573 7454 4350  r].class TestTCP
-00000e30: 5374 7265 616d 3a0a 2020 2020 4070 7974  Stream:.    @pyt
-00000e40: 6573 742e 6669 7874 7572 650a 2020 2020  est.fixture.    
-00000e50: 6465 6620 7365 7276 6572 5f73 6f63 6b28  def server_sock(
-00000e60: 7365 6c66 2c20 6661 6d69 6c79 3a20 416e  self, family: An
-00000e70: 7949 5041 6464 7265 7373 4661 6d69 6c79  yIPAddressFamily
-00000e80: 2920 2d3e 2049 7465 7261 746f 725b 736f  ) -> Iterator[so
-00000e90: 636b 6574 2e73 6f63 6b65 745d 3a0a 2020  cket.socket]:.  
-00000ea0: 2020 2020 2020 736f 636b 203d 2073 6f63        sock = soc
-00000eb0: 6b65 742e 736f 636b 6574 2866 616d 696c  ket.socket(famil
-00000ec0: 792c 2073 6f63 6b65 742e 534f 434b 5f53  y, socket.SOCK_S
-00000ed0: 5452 4541 4d29 0a20 2020 2020 2020 2073  TREAM).        s
-00000ee0: 6f63 6b2e 7365 7474 696d 656f 7574 2831  ock.settimeout(1
-00000ef0: 290a 2020 2020 2020 2020 736f 636b 2e62  ).        sock.b
-00000f00: 696e 6428 2822 6c6f 6361 6c68 6f73 7422  ind(("localhost"
-00000f10: 2c20 3029 290a 2020 2020 2020 2020 736f  , 0)).        so
-00000f20: 636b 2e6c 6973 7465 6e28 290a 2020 2020  ck.listen().    
-00000f30: 2020 2020 7969 656c 6420 736f 636b 0a20      yield sock. 
-00000f40: 2020 2020 2020 2073 6f63 6b2e 636c 6f73         sock.clos
-00000f50: 6528 290a 0a20 2020 2040 7079 7465 7374  e()..    @pytest
-00000f60: 2e66 6978 7475 7265 0a20 2020 2064 6566  .fixture.    def
-00000f70: 2073 6572 7665 725f 6164 6472 2873 656c   server_addr(sel
-00000f80: 662c 2073 6572 7665 725f 736f 636b 3a20  f, server_sock: 
-00000f90: 736f 636b 6574 2e73 6f63 6b65 7429 202d  socket.socket) -
-00000fa0: 3e20 7475 706c 655b 7374 722c 2069 6e74  > tuple[str, int
-00000fb0: 5d3a 0a20 2020 2020 2020 2072 6574 7572  ]:.        retur
-00000fc0: 6e20 7365 7276 6572 5f73 6f63 6b2e 6765  n server_sock.ge
-00000fd0: 7473 6f63 6b6e 616d 6528 295b 3a32 5d0a  tsockname()[:2].
-00000fe0: 0a20 2020 2061 7379 6e63 2064 6566 2074  .    async def t
-00000ff0: 6573 745f 6578 7472 615f 6174 7472 6962  est_extra_attrib
-00001000: 7574 6573 280a 2020 2020 2020 2020 7365  utes(.        se
-00001010: 6c66 2c0a 2020 2020 2020 2020 7365 7276  lf,.        serv
-00001020: 6572 5f73 6f63 6b3a 2073 6f63 6b65 742e  er_sock: socket.
-00001030: 736f 636b 6574 2c0a 2020 2020 2020 2020  socket,.        
-00001040: 7365 7276 6572 5f61 6464 723a 2074 7570  server_addr: tup
-00001050: 6c65 5b73 7472 2c20 696e 745d 2c0a 2020  le[str, int],.  
-00001060: 2020 2020 2020 6661 6d69 6c79 3a20 416e        family: An
-00001070: 7949 5041 6464 7265 7373 4661 6d69 6c79  yIPAddressFamily
-00001080: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
-00001090: 0a20 2020 2020 2020 2061 7379 6e63 2077  .        async w
-000010a0: 6974 6820 6177 6169 7420 636f 6e6e 6563  ith await connec
-000010b0: 745f 7463 7028 2a73 6572 7665 725f 6164  t_tcp(*server_ad
-000010c0: 6472 2920 6173 2073 7472 6561 6d3a 0a20  dr) as stream:. 
-000010d0: 2020 2020 2020 2020 2020 2072 6177 5f73             raw_s
-000010e0: 6f63 6b65 7420 3d20 7374 7265 616d 2e65  ocket = stream.e
-000010f0: 7874 7261 2853 6f63 6b65 7441 7474 7269  xtra(SocketAttri
-00001100: 6275 7465 2e72 6177 5f73 6f63 6b65 7429  bute.raw_socket)
-00001110: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-00001120: 6572 7420 7374 7265 616d 2e65 7874 7261  ert stream.extra
-00001130: 2853 6f63 6b65 7441 7474 7269 6275 7465  (SocketAttribute
-00001140: 2e66 616d 696c 7929 203d 3d20 6661 6d69  .family) == fami
-00001150: 6c79 0a20 2020 2020 2020 2020 2020 2061  ly.            a
-00001160: 7373 6572 7420 280a 2020 2020 2020 2020  ssert (.        
-00001170: 2020 2020 2020 2020 7374 7265 616d 2e65          stream.e
-00001180: 7874 7261 2853 6f63 6b65 7441 7474 7269  xtra(SocketAttri
-00001190: 6275 7465 2e6c 6f63 616c 5f61 6464 7265  bute.local_addre
-000011a0: 7373 290a 2020 2020 2020 2020 2020 2020  ss).            
-000011b0: 2020 2020 3d3d 2072 6177 5f73 6f63 6b65      == raw_socke
-000011c0: 742e 6765 7473 6f63 6b6e 616d 6528 295b  t.getsockname()[
-000011d0: 3a32 5d0a 2020 2020 2020 2020 2020 2020  :2].            
-000011e0: 290a 2020 2020 2020 2020 2020 2020 6173  ).            as
-000011f0: 7365 7274 2028 0a20 2020 2020 2020 2020  sert (.         
-00001200: 2020 2020 2020 2073 7472 6561 6d2e 6578         stream.ex
-00001210: 7472 6128 536f 636b 6574 4174 7472 6962  tra(SocketAttrib
-00001220: 7574 652e 6c6f 6361 6c5f 706f 7274 2920  ute.local_port) 
-00001230: 3d3d 2072 6177 5f73 6f63 6b65 742e 6765  == raw_socket.ge
-00001240: 7473 6f63 6b6e 616d 6528 295b 315d 0a20  tsockname()[1]. 
-00001250: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00001260: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-00001270: 7374 7265 616d 2e65 7874 7261 2853 6f63  stream.extra(Soc
-00001280: 6b65 7441 7474 7269 6275 7465 2e72 656d  ketAttribute.rem
-00001290: 6f74 655f 6164 6472 6573 7329 203d 3d20  ote_address) == 
-000012a0: 7365 7276 6572 5f61 6464 720a 2020 2020  server_addr.    
-000012b0: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-000012c0: 7472 6561 6d2e 6578 7472 6128 536f 636b  tream.extra(Sock
-000012d0: 6574 4174 7472 6962 7574 652e 7265 6d6f  etAttribute.remo
-000012e0: 7465 5f70 6f72 7429 203d 3d20 7365 7276  te_port) == serv
-000012f0: 6572 5f61 6464 725b 315d 0a0a 2020 2020  er_addr[1]..    
-00001300: 6173 796e 6320 6465 6620 7465 7374 5f73  async def test_s
-00001310: 656e 645f 7265 6365 6976 6528 0a20 2020  end_receive(.   
-00001320: 2020 2020 2073 656c 662c 2073 6572 7665       self, serve
-00001330: 725f 736f 636b 3a20 736f 636b 6574 2e73  r_sock: socket.s
-00001340: 6f63 6b65 742c 2073 6572 7665 725f 6164  ocket, server_ad
-00001350: 6472 3a20 7475 706c 655b 7374 722c 2069  dr: tuple[str, i
-00001360: 6e74 5d0a 2020 2020 2920 2d3e 204e 6f6e  nt].    ) -> Non
-00001370: 653a 0a20 2020 2020 2020 2061 7379 6e63  e:.        async
-00001380: 2077 6974 6820 6177 6169 7420 636f 6e6e   with await conn
-00001390: 6563 745f 7463 7028 2a73 6572 7665 725f  ect_tcp(*server_
-000013a0: 6164 6472 2920 6173 2073 7472 6561 6d3a  addr) as stream:
-000013b0: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
-000013c0: 656e 742c 205f 203d 2073 6572 7665 725f  ent, _ = server_
-000013d0: 736f 636b 2e61 6363 6570 7428 290a 2020  sock.accept().  
-000013e0: 2020 2020 2020 2020 2020 6177 6169 7420            await 
-000013f0: 7374 7265 616d 2e73 656e 6428 6222 626c  stream.send(b"bl
-00001400: 6168 2229 0a20 2020 2020 2020 2020 2020  ah").           
-00001410: 2072 6571 7565 7374 203d 2063 6c69 656e   request = clien
-00001420: 742e 7265 6376 2831 3030 290a 2020 2020  t.recv(100).    
-00001430: 2020 2020 2020 2020 636c 6965 6e74 2e73          client.s
-00001440: 656e 6461 6c6c 2872 6571 7565 7374 5b3a  endall(request[:
-00001450: 3a2d 315d 290a 2020 2020 2020 2020 2020  :-1]).          
-00001460: 2020 7265 7370 6f6e 7365 203d 2061 7761    response = awa
-00001470: 6974 2073 7472 6561 6d2e 7265 6365 6976  it stream.receiv
-00001480: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-00001490: 636c 6965 6e74 2e63 6c6f 7365 2829 0a0a  client.close()..
-000014a0: 2020 2020 2020 2020 6173 7365 7274 2072          assert r
-000014b0: 6573 706f 6e73 6520 3d3d 2062 2268 616c  esponse == b"hal
-000014c0: 6222 0a0a 2020 2020 6173 796e 6320 6465  b"..    async de
-000014d0: 6620 7465 7374 5f73 656e 645f 6c61 7267  f test_send_larg
-000014e0: 655f 6275 6666 6572 280a 2020 2020 2020  e_buffer(.      
-000014f0: 2020 7365 6c66 2c20 7365 7276 6572 5f73    self, server_s
-00001500: 6f63 6b3a 2073 6f63 6b65 742e 736f 636b  ock: socket.sock
-00001510: 6574 2c20 7365 7276 6572 5f61 6464 723a  et, server_addr:
-00001520: 2074 7570 6c65 5b73 7472 2c20 696e 745d   tuple[str, int]
-00001530: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a0a  .    ) -> None:.
-00001540: 2020 2020 2020 2020 6465 6620 7365 7276          def serv
-00001550: 6528 2920 2d3e 204e 6f6e 653a 0a20 2020  e() -> None:.   
-00001560: 2020 2020 2020 2020 2063 6c69 656e 742c           client,
-00001570: 205f 203d 2073 6572 7665 725f 736f 636b   _ = server_sock
-00001580: 2e61 6363 6570 7428 290a 2020 2020 2020  .accept().      
-00001590: 2020 2020 2020 636c 6965 6e74 2e73 656e        client.sen
-000015a0: 6461 6c6c 2862 7566 6665 7229 0a20 2020  dall(buffer).   
-000015b0: 2020 2020 2020 2020 2063 6c69 656e 742e           client.
-000015c0: 636c 6f73 6528 290a 0a20 2020 2020 2020  close()..       
-000015d0: 2062 7566 6665 7220 3d20 280a 2020 2020   buffer = (.    
-000015e0: 2020 2020 2020 2020 6222 5c78 6666 2220          b"\xff" 
-000015f0: 2a20 3130 3234 202a 2031 3032 340a 2020  * 1024 * 1024.  
-00001600: 2020 2020 2020 2920 2023 2073 686f 756c        )  # shoul
-00001610: 6420 6578 6365 6564 2074 6865 206d 6178  d exceed the max
-00001620: 696d 756d 206b 6572 6e65 6c20 7365 6e64  imum kernel send
-00001630: 2062 7566 6665 7220 7369 7a65 0a20 2020   buffer size.   
-00001640: 2020 2020 2061 7379 6e63 2077 6974 6820       async with 
-00001650: 6177 6169 7420 636f 6e6e 6563 745f 7463  await connect_tc
-00001660: 7028 2a73 6572 7665 725f 6164 6472 2920  p(*server_addr) 
-00001670: 6173 2073 7472 6561 6d3a 0a20 2020 2020  as stream:.     
-00001680: 2020 2020 2020 2074 6872 6561 6420 3d20         thread = 
-00001690: 5468 7265 6164 2874 6172 6765 743d 7365  Thread(target=se
-000016a0: 7276 652c 2064 6165 6d6f 6e3d 5472 7565  rve, daemon=True
-000016b0: 290a 2020 2020 2020 2020 2020 2020 7468  ).            th
-000016c0: 7265 6164 2e73 7461 7274 2829 0a20 2020  read.start().   
-000016d0: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
-000016e0: 6520 3d20 6222 220a 2020 2020 2020 2020  e = b"".        
-000016f0: 2020 2020 7768 696c 6520 6c65 6e28 7265      while len(re
-00001700: 7370 6f6e 7365 2920 3c20 6c65 6e28 6275  sponse) < len(bu
-00001710: 6666 6572 293a 0a20 2020 2020 2020 2020  ffer):.         
-00001720: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-00001730: 2b3d 2061 7761 6974 2073 7472 6561 6d2e  += await stream.
-00001740: 7265 6365 6976 6528 290a 0a20 2020 2020  receive()..     
-00001750: 2020 2074 6872 6561 642e 6a6f 696e 2829     thread.join()
-00001760: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00001770: 7265 7370 6f6e 7365 203d 3d20 6275 6666  response == buff
-00001780: 6572 0a0a 2020 2020 6173 796e 6320 6465  er..    async de
-00001790: 6620 7465 7374 5f73 656e 645f 656f 6628  f test_send_eof(
-000017a0: 0a20 2020 2020 2020 2073 656c 662c 2073  .        self, s
-000017b0: 6572 7665 725f 736f 636b 3a20 736f 636b  erver_sock: sock
-000017c0: 6574 2e73 6f63 6b65 742c 2073 6572 7665  et.socket, serve
-000017d0: 725f 6164 6472 3a20 7475 706c 655b 7374  r_addr: tuple[st
-000017e0: 722c 2069 6e74 5d0a 2020 2020 2920 2d3e  r, int].    ) ->
-000017f0: 204e 6f6e 653a 0a20 2020 2020 2020 2064   None:.        d
-00001800: 6566 2073 6572 7665 2829 202d 3e20 4e6f  ef serve() -> No
-00001810: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00001820: 636c 6965 6e74 2c20 5f20 3d20 7365 7276  client, _ = serv
-00001830: 6572 5f73 6f63 6b2e 6163 6365 7074 2829  er_sock.accept()
-00001840: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
-00001850: 7565 7374 203d 2062 2222 0a20 2020 2020  uest = b"".     
-00001860: 2020 2020 2020 2077 6869 6c65 2054 7275         while Tru
-00001870: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00001880: 2020 2064 6174 6120 3d20 636c 6965 6e74     data = client
-00001890: 2e72 6563 7628 3130 3029 0a20 2020 2020  .recv(100).     
-000018a0: 2020 2020 2020 2020 2020 2072 6571 7565             reque
-000018b0: 7374 202b 3d20 6461 7461 0a20 2020 2020  st += data.     
-000018c0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-000018d0: 7420 6461 7461 3a0a 2020 2020 2020 2020  t data:.        
-000018e0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-000018f0: 6b0a 0a20 2020 2020 2020 2020 2020 2063  k..            c
-00001900: 6c69 656e 742e 7365 6e64 616c 6c28 7265  lient.sendall(re
-00001910: 7175 6573 745b 3a3a 2d31 5d29 0a20 2020  quest[::-1]).   
-00001920: 2020 2020 2020 2020 2063 6c69 656e 742e           client.
-00001930: 636c 6f73 6528 290a 0a20 2020 2020 2020  close()..       
-00001940: 2061 7379 6e63 2077 6974 6820 6177 6169   async with awai
-00001950: 7420 636f 6e6e 6563 745f 7463 7028 2a73  t connect_tcp(*s
-00001960: 6572 7665 725f 6164 6472 2920 6173 2073  erver_addr) as s
-00001970: 7472 6561 6d3a 0a20 2020 2020 2020 2020  tream:.         
-00001980: 2020 2074 6872 6561 6420 3d20 5468 7265     thread = Thre
-00001990: 6164 2874 6172 6765 743d 7365 7276 652c  ad(target=serve,
-000019a0: 2064 6165 6d6f 6e3d 5472 7565 290a 2020   daemon=True).  
-000019b0: 2020 2020 2020 2020 2020 7468 7265 6164            thread
-000019c0: 2e73 7461 7274 2829 0a20 2020 2020 2020  .start().       
-000019d0: 2020 2020 2061 7761 6974 2073 7472 6561       await strea
-000019e0: 6d2e 7365 6e64 2862 2268 656c 6c6f 2c20  m.send(b"hello, 
-000019f0: 2229 0a20 2020 2020 2020 2020 2020 2061  ").            a
-00001a00: 7761 6974 2073 7472 6561 6d2e 7365 6e64  wait stream.send
-00001a10: 2862 2277 6f72 6c64 5c6e 2229 0a20 2020  (b"world\n").   
-00001a20: 2020 2020 2020 2020 2061 7761 6974 2073           await s
-00001a30: 7472 6561 6d2e 7365 6e64 5f65 6f66 2829  tream.send_eof()
-00001a40: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00001a50: 706f 6e73 6520 3d20 6177 6169 7420 7374  ponse = await st
-00001a60: 7265 616d 2e72 6563 6569 7665 2829 0a0a  ream.receive()..
-00001a70: 2020 2020 2020 2020 7468 7265 6164 2e6a          thread.j
-00001a80: 6f69 6e28 290a 2020 2020 2020 2020 6173  oin().        as
-00001a90: 7365 7274 2072 6573 706f 6e73 6520 3d3d  sert response ==
-00001aa0: 2062 225c 6e64 6c72 6f77 202c 6f6c 6c65   b"\ndlrow ,olle
-00001ab0: 6822 0a0a 2020 2020 6173 796e 6320 6465  h"..    async de
-00001ac0: 6620 7465 7374 5f69 7465 7261 7465 280a  f test_iterate(.
-00001ad0: 2020 2020 2020 2020 7365 6c66 2c20 7365          self, se
-00001ae0: 7276 6572 5f73 6f63 6b3a 2073 6f63 6b65  rver_sock: socke
-00001af0: 742e 736f 636b 6574 2c20 7365 7276 6572  t.socket, server
-00001b00: 5f61 6464 723a 2074 7570 6c65 5b73 7472  _addr: tuple[str
-00001b10: 2c20 696e 745d 0a20 2020 2029 202d 3e20  , int].    ) -> 
-00001b20: 4e6f 6e65 3a0a 2020 2020 2020 2020 6465  None:.        de
-00001b30: 6620 7365 7276 6528 2920 2d3e 204e 6f6e  f serve() -> Non
-00001b40: 653a 0a20 2020 2020 2020 2020 2020 2063  e:.            c
-00001b50: 6c69 656e 742c 205f 203d 2073 6572 7665  lient, _ = serve
-00001b60: 725f 736f 636b 2e61 6363 6570 7428 290a  r_sock.accept().
-00001b70: 2020 2020 2020 2020 2020 2020 636c 6965              clie
-00001b80: 6e74 2e73 656e 6461 6c6c 2862 2262 6c22  nt.sendall(b"bl"
-00001b90: 290a 2020 2020 2020 2020 2020 2020 6576  ).            ev
-00001ba0: 656e 742e 7761 6974 2831 290a 2020 2020  ent.wait(1).    
-00001bb0: 2020 2020 2020 2020 636c 6965 6e74 2e73          client.s
-00001bc0: 656e 6461 6c6c 2862 2261 6822 290a 2020  endall(b"ah").  
-00001bd0: 2020 2020 2020 2020 2020 636c 6965 6e74            client
-00001be0: 2e63 6c6f 7365 2829 0a0a 2020 2020 2020  .close()..      
-00001bf0: 2020 6576 656e 7420 3d20 7468 7265 6164    event = thread
-00001c00: 696e 672e 4576 656e 7428 290a 2020 2020  ing.Event().    
-00001c10: 2020 2020 7468 7265 6164 203d 2054 6872      thread = Thr
-00001c20: 6561 6428 7461 7267 6574 3d73 6572 7665  ead(target=serve
-00001c30: 2c20 6461 656d 6f6e 3d54 7275 6529 0a20  , daemon=True). 
-00001c40: 2020 2020 2020 2074 6872 6561 642e 7374         thread.st
-00001c50: 6172 7428 290a 2020 2020 2020 2020 6368  art().        ch
-00001c60: 756e 6b73 203d 205b 5d0a 2020 2020 2020  unks = [].      
-00001c70: 2020 6173 796e 6320 7769 7468 2061 7761    async with awa
-00001c80: 6974 2063 6f6e 6e65 6374 5f74 6370 282a  it connect_tcp(*
-00001c90: 7365 7276 6572 5f61 6464 7229 2061 7320  server_addr) as 
-00001ca0: 7374 7265 616d 3a0a 2020 2020 2020 2020  stream:.        
-00001cb0: 2020 2020 6173 796e 6320 666f 7220 6368      async for ch
-00001cc0: 756e 6b20 696e 2073 7472 6561 6d3a 0a20  unk in stream:. 
-00001cd0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00001ce0: 6875 6e6b 732e 6170 7065 6e64 2863 6875  hunks.append(chu
-00001cf0: 6e6b 290a 2020 2020 2020 2020 2020 2020  nk).            
-00001d00: 2020 2020 6576 656e 742e 7365 7428 290a      event.set().
-00001d10: 0a20 2020 2020 2020 2074 6872 6561 642e  .        thread.
-00001d20: 6a6f 696e 2829 0a20 2020 2020 2020 2061  join().        a
-00001d30: 7373 6572 7420 6368 756e 6b73 203d 3d20  ssert chunks == 
-00001d40: 5b62 2262 6c22 2c20 6222 6168 225d 0a0a  [b"bl", b"ah"]..
-00001d50: 2020 2020 6173 796e 6320 6465 6620 7465      async def te
-00001d60: 7374 5f73 6f63 6b65 745f 6f70 7469 6f6e  st_socket_option
-00001d70: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
-00001d80: 2066 616d 696c 793a 2041 6e79 4950 4164   family: AnyIPAd
-00001d90: 6472 6573 7346 616d 696c 792c 2073 6572  dressFamily, ser
-00001da0: 7665 725f 6164 6472 3a20 7475 706c 655b  ver_addr: tuple[
-00001db0: 7374 722c 2069 6e74 5d0a 2020 2020 2920  str, int].    ) 
-00001dc0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00001dd0: 2061 7379 6e63 2077 6974 6820 6177 6169   async with awai
-00001de0: 7420 636f 6e6e 6563 745f 7463 7028 2a73  t connect_tcp(*s
-00001df0: 6572 7665 725f 6164 6472 2920 6173 2073  erver_addr) as s
-00001e00: 7472 6561 6d3a 0a20 2020 2020 2020 2020  tream:.         
-00001e10: 2020 2072 6177 5f73 6f63 6b65 7420 3d20     raw_socket = 
-00001e20: 7374 7265 616d 2e65 7874 7261 2853 6f63  stream.extra(Soc
-00001e30: 6b65 7441 7474 7269 6275 7465 2e72 6177  ketAttribute.raw
-00001e40: 5f73 6f63 6b65 7429 0a20 2020 2020 2020  _socket).       
-00001e50: 2020 2020 2061 7373 6572 7420 7261 775f       assert raw_
-00001e60: 736f 636b 6574 2e67 6574 736f 636b 6f70  socket.getsockop
-00001e70: 7428 736f 636b 6574 2e49 5050 524f 544f  t(socket.IPPROTO
-00001e80: 5f54 4350 2c20 736f 636b 6574 2e54 4350  _TCP, socket.TCP
-00001e90: 5f4e 4f44 454c 4159 2920 213d 2030 0a0a  _NODELAY) != 0..
-00001ea0: 2020 2020 4073 6b69 705f 6970 7636 5f6d      @skip_ipv6_m
-00001eb0: 6172 6b0a 2020 2020 4070 7974 6573 742e  ark.    @pytest.
-00001ec0: 6d61 726b 2e70 6172 616d 6574 7269 7a65  mark.parametrize
-00001ed0: 280a 2020 2020 2020 2020 226c 6f63 616c  (.        "local
-00001ee0: 5f61 6464 722c 2065 7870 6563 7465 645f  _addr, expected_
-00001ef0: 636c 6965 6e74 5f61 6464 7222 2c0a 2020  client_addr",.  
-00001f00: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
-00001f10: 2020 2020 7079 7465 7374 2e70 6172 616d      pytest.param
-00001f20: 2822 222c 2022 3a3a 3122 2c20 6964 3d22  ("", "::1", id="
-00001f30: 6475 616c 7374 6163 6b22 292c 0a20 2020  dualstack"),.   
-00001f40: 2020 2020 2020 2020 2070 7974 6573 742e           pytest.
-00001f50: 7061 7261 6d28 2231 3237 2e30 2e30 2e31  param("127.0.0.1
-00001f60: 222c 2022 3132 372e 302e 302e 3122 2c20  ", "127.0.0.1", 
-00001f70: 6964 3d22 6970 7634 2229 2c0a 2020 2020  id="ipv4"),.    
-00001f80: 2020 2020 2020 2020 7079 7465 7374 2e70          pytest.p
-00001f90: 6172 616d 2822 3a3a 3122 2c20 223a 3a31  aram("::1", "::1
-00001fa0: 222c 2069 643d 2269 7076 3622 292c 0a20  ", id="ipv6"),. 
-00001fb0: 2020 2020 2020 205d 2c0a 2020 2020 290a         ],.    ).
-00001fc0: 2020 2020 6173 796e 6320 6465 6620 7465      async def te
-00001fd0: 7374 5f68 6170 7079 5f65 7965 6261 6c6c  st_happy_eyeball
-00001fe0: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
-00001ff0: 206c 6f63 616c 5f61 6464 723a 2073 7472   local_addr: str
-00002000: 2c20 6578 7065 6374 6564 5f63 6c69 656e  , expected_clien
-00002010: 745f 6164 6472 3a20 7374 722c 2066 616b  t_addr: str, fak
-00002020: 655f 6c6f 6361 6c68 6f73 745f 646e 733a  e_localhost_dns:
-00002030: 204e 6f6e 650a 2020 2020 2920 2d3e 204e   None.    ) -> N
-00002040: 6f6e 653a 0a20 2020 2020 2020 2063 6c69  one:.        cli
-00002050: 656e 745f 6164 6472 203d 204e 6f6e 652c  ent_addr = None,
-00002060: 204e 6f6e 650a 0a20 2020 2020 2020 2064   None..        d
-00002070: 6566 2073 6572 7665 2829 202d 3e20 4e6f  ef serve() -> No
-00002080: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00002090: 6e6f 6e6c 6f63 616c 2063 6c69 656e 745f  nonlocal client_
-000020a0: 6164 6472 0a20 2020 2020 2020 2020 2020  addr.           
-000020b0: 2063 6c69 656e 742c 2063 6c69 656e 745f   client, client_
-000020c0: 6164 6472 203d 2073 6572 7665 725f 736f  addr = server_so
-000020d0: 636b 2e61 6363 6570 7428 290a 2020 2020  ck.accept().    
-000020e0: 2020 2020 2020 2020 636c 6965 6e74 2e63          client.c
-000020f0: 6c6f 7365 2829 0a0a 2020 2020 2020 2020  lose()..        
-00002100: 6661 6d69 6c79 203d 2028 0a20 2020 2020  family = (.     
-00002110: 2020 2020 2020 2041 6464 7265 7373 4661         AddressFa
-00002120: 6d69 6c79 2e41 465f 494e 4554 0a20 2020  mily.AF_INET.   
-00002130: 2020 2020 2020 2020 2069 6620 6c6f 6361           if loca
-00002140: 6c5f 6164 6472 203d 3d20 2231 3237 2e30  l_addr == "127.0
-00002150: 2e30 2e31 220a 2020 2020 2020 2020 2020  .0.1".          
-00002160: 2020 656c 7365 2041 6464 7265 7373 4661    else AddressFa
-00002170: 6d69 6c79 2e41 465f 494e 4554 360a 2020  mily.AF_INET6.  
-00002180: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00002190: 7365 7276 6572 5f73 6f63 6b20 3d20 736f  server_sock = so
-000021a0: 636b 6574 2e73 6f63 6b65 7428 6661 6d69  cket.socket(fami
-000021b0: 6c79 290a 2020 2020 2020 2020 7365 7276  ly).        serv
-000021c0: 6572 5f73 6f63 6b2e 6269 6e64 2828 6c6f  er_sock.bind((lo
-000021d0: 6361 6c5f 6164 6472 2c20 3029 290a 2020  cal_addr, 0)).  
-000021e0: 2020 2020 2020 7365 7276 6572 5f73 6f63        server_soc
-000021f0: 6b2e 6c69 7374 656e 2829 0a20 2020 2020  k.listen().     
-00002200: 2020 2070 6f72 7420 3d20 7365 7276 6572     port = server
-00002210: 5f73 6f63 6b2e 6765 7473 6f63 6b6e 616d  _sock.getsocknam
-00002220: 6528 295b 315d 0a20 2020 2020 2020 2074  e()[1].        t
-00002230: 6872 6561 6420 3d20 5468 7265 6164 2874  hread = Thread(t
-00002240: 6172 6765 743d 7365 7276 652c 2064 6165  arget=serve, dae
-00002250: 6d6f 6e3d 5472 7565 290a 2020 2020 2020  mon=True).      
-00002260: 2020 7468 7265 6164 2e73 7461 7274 2829    thread.start()
-00002270: 0a0a 2020 2020 2020 2020 6173 796e 6320  ..        async 
-00002280: 7769 7468 2061 7761 6974 2063 6f6e 6e65  with await conne
-00002290: 6374 5f74 6370 2822 6c6f 6361 6c68 6f73  ct_tcp("localhos
-000022a0: 7422 2c20 706f 7274 293a 0a20 2020 2020  t", port):.     
-000022b0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-000022c0: 2020 2020 2074 6872 6561 642e 6a6f 696e       thread.join
-000022d0: 2829 0a20 2020 2020 2020 2073 6572 7665  ().        serve
-000022e0: 725f 736f 636b 2e63 6c6f 7365 2829 0a20  r_sock.close(). 
-000022f0: 2020 2020 2020 2061 7373 6572 7420 636c         assert cl
-00002300: 6965 6e74 5f61 6464 725b 305d 203d 3d20  ient_addr[0] == 
-00002310: 6578 7065 6374 6564 5f63 6c69 656e 745f  expected_client_
-00002320: 6164 6472 0a0a 2020 2020 4070 7974 6573  addr..    @pytes
-00002330: 742e 6d61 726b 2e70 6172 616d 6574 7269  t.mark.parametri
-00002340: 7a65 280a 2020 2020 2020 2020 2274 6172  ze(.        "tar
-00002350: 6765 742c 2065 7863 6570 7469 6f6e 5f63  get, exception_c
-00002360: 6c61 7373 222c 0a20 2020 2020 2020 205b  lass",.        [
-00002370: 0a20 2020 2020 2020 2020 2020 2070 7974  .            pyt
-00002380: 6573 742e 7061 7261 6d28 0a20 2020 2020  est.param(.     
-00002390: 2020 2020 2020 2020 2020 2022 6c6f 6361             "loca
-000023a0: 6c68 6f73 7422 2c20 4578 6365 7074 696f  lhost", Exceptio
-000023b0: 6e47 726f 7570 2c20 6964 3d22 6d75 6c74  nGroup, id="mult
-000023c0: 6922 2c20 6d61 726b 733d 5b73 6b69 705f  i", marks=[skip_
-000023d0: 6970 7636 5f6d 6172 6b5d 0a20 2020 2020  ipv6_mark].     
-000023e0: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
-000023f0: 2020 2020 2020 7079 7465 7374 2e70 6172        pytest.par
-00002400: 616d 2822 3132 372e 302e 302e 3122 2c20  am("127.0.0.1", 
-00002410: 436f 6e6e 6563 7469 6f6e 5265 6675 7365  ConnectionRefuse
-00002420: 6445 7272 6f72 2c20 6964 3d22 7369 6e67  dError, id="sing
-00002430: 6c65 2229 2c0a 2020 2020 2020 2020 5d2c  le"),.        ],
-00002440: 0a20 2020 2029 0a20 2020 2061 7379 6e63  .    ).    async
-00002450: 2064 6566 2074 6573 745f 636f 6e6e 6563   def test_connec
-00002460: 7469 6f6e 5f72 6566 7573 6564 280a 2020  tion_refused(.  
-00002470: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00002480: 2020 2020 7461 7267 6574 3a20 7374 722c      target: str,
-00002490: 0a20 2020 2020 2020 2065 7863 6570 7469  .        excepti
-000024a0: 6f6e 5f63 6c61 7373 3a20 7479 7065 5b45  on_class: type[E
-000024b0: 7863 6570 7469 6f6e 4772 6f75 705d 207c  xceptionGroup] |
-000024c0: 2074 7970 655b 436f 6e6e 6563 7469 6f6e   type[Connection
-000024d0: 5265 6675 7365 6445 7272 6f72 5d2c 0a20  RefusedError],. 
-000024e0: 2020 2020 2020 2066 616b 655f 6c6f 6361         fake_loca
-000024f0: 6c68 6f73 745f 646e 733a 204e 6f6e 652c  lhost_dns: None,
-00002500: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a0a  .    ) -> None:.
-00002510: 2020 2020 2020 2020 6475 6d6d 795f 736f          dummy_so
-00002520: 636b 6574 203d 2073 6f63 6b65 742e 736f  cket = socket.so
-00002530: 636b 6574 2841 6464 7265 7373 4661 6d69  cket(AddressFami
-00002540: 6c79 2e41 465f 494e 4554 3629 0a20 2020  ly.AF_INET6).   
-00002550: 2020 2020 2064 756d 6d79 5f73 6f63 6b65       dummy_socke
-00002560: 742e 6269 6e64 2828 223a 3a22 2c20 3029  t.bind(("::", 0)
-00002570: 290a 2020 2020 2020 2020 6672 6565 5f70  ).        free_p
-00002580: 6f72 7420 3d20 6475 6d6d 795f 736f 636b  ort = dummy_sock
-00002590: 6574 2e67 6574 736f 636b 6e61 6d65 2829  et.getsockname()
-000025a0: 5b31 5d0a 2020 2020 2020 2020 6475 6d6d  [1].        dumm
-000025b0: 795f 736f 636b 6574 2e63 6c6f 7365 2829  y_socket.close()
-000025c0: 0a0a 2020 2020 2020 2020 7769 7468 2070  ..        with p
-000025d0: 7974 6573 742e 7261 6973 6573 284f 5345  ytest.raises(OSE
-000025e0: 7272 6f72 2920 6173 2065 7863 3a0a 2020  rror) as exc:.  
-000025f0: 2020 2020 2020 2020 2020 6177 6169 7420            await 
-00002600: 636f 6e6e 6563 745f 7463 7028 7461 7267  connect_tcp(targ
-00002610: 6574 2c20 6672 6565 5f70 6f72 7429 0a0a  et, free_port)..
-00002620: 2020 2020 2020 2020 6173 7365 7274 2065          assert e
-00002630: 7863 2e6d 6174 6368 2822 416c 6c20 636f  xc.match("All co
-00002640: 6e6e 6563 7469 6f6e 2061 7474 656d 7074  nnection attempt
-00002650: 7320 6661 696c 6564 2229 0a20 2020 2020  s failed").     
-00002660: 2020 2061 7373 6572 7420 6973 696e 7374     assert isinst
-00002670: 616e 6365 2865 7863 2e76 616c 7565 2e5f  ance(exc.value._
-00002680: 5f63 6175 7365 5f5f 2c20 6578 6365 7074  _cause__, except
-00002690: 696f 6e5f 636c 6173 7329 0a20 2020 2020  ion_class).     
-000026a0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-000026b0: 2865 7863 2e76 616c 7565 2e5f 5f63 6175  (exc.value.__cau
-000026c0: 7365 5f5f 2c20 4578 6365 7074 696f 6e47  se__, ExceptionG
-000026d0: 726f 7570 293a 0a20 2020 2020 2020 2020  roup):.         
-000026e0: 2020 2066 6f72 2065 7863 6570 7469 6f6e     for exception
-000026f0: 2069 6e20 6578 632e 7661 6c75 652e 5f5f   in exc.value.__
-00002700: 6361 7573 655f 5f2e 6578 6365 7074 696f  cause__.exceptio
-00002710: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00002720: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
-00002730: 7461 6e63 6528 6578 6365 7074 696f 6e2c  tance(exception,
-00002740: 2043 6f6e 6e65 6374 696f 6e52 6566 7573   ConnectionRefus
-00002750: 6564 4572 726f 7229 0a0a 2020 2020 6173  edError)..    as
-00002760: 796e 6320 6465 6620 7465 7374 5f72 6563  ync def test_rec
-00002770: 6569 7665 5f74 696d 656f 7574 280a 2020  eive_timeout(.  
-00002780: 2020 2020 2020 7365 6c66 2c20 7365 7276        self, serv
-00002790: 6572 5f73 6f63 6b3a 2073 6f63 6b65 742e  er_sock: socket.
-000027a0: 736f 636b 6574 2c20 7365 7276 6572 5f61  socket, server_a
-000027b0: 6464 723a 2074 7570 6c65 5b73 7472 2c20  ddr: tuple[str, 
-000027c0: 696e 745d 0a20 2020 2029 202d 3e20 4e6f  int].    ) -> No
-000027d0: 6e65 3a0a 2020 2020 2020 2020 6465 6620  ne:.        def 
-000027e0: 7365 7276 6528 2920 2d3e 204e 6f6e 653a  serve() -> None:
-000027f0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-00002800: 6e2c 205f 203d 2073 6572 7665 725f 736f  n, _ = server_so
-00002810: 636b 2e61 6363 6570 7428 290a 2020 2020  ck.accept().    
-00002820: 2020 2020 2020 2020 7469 6d65 2e73 6c65          time.sle
-00002830: 6570 2831 290a 2020 2020 2020 2020 2020  ep(1).          
-00002840: 2020 636f 6e6e 2e63 6c6f 7365 2829 0a0a    conn.close()..
-00002850: 2020 2020 2020 2020 7468 7265 6164 203d          thread =
-00002860: 2054 6872 6561 6428 7461 7267 6574 3d73   Thread(target=s
-00002870: 6572 7665 2c20 6461 656d 6f6e 3d54 7275  erve, daemon=Tru
-00002880: 6529 0a20 2020 2020 2020 2074 6872 6561  e).        threa
-00002890: 642e 7374 6172 7428 290a 2020 2020 2020  d.start().      
-000028a0: 2020 6173 796e 6320 7769 7468 2061 7761    async with awa
-000028b0: 6974 2063 6f6e 6e65 6374 5f74 6370 282a  it connect_tcp(*
-000028c0: 7365 7276 6572 5f61 6464 7229 2061 7320  server_addr) as 
-000028d0: 7374 7265 616d 3a0a 2020 2020 2020 2020  stream:.        
-000028e0: 2020 2020 7374 6172 745f 7469 6d65 203d      start_time =
-000028f0: 2074 696d 652e 6d6f 6e6f 746f 6e69 6328   time.monotonic(
-00002900: 290a 2020 2020 2020 2020 2020 2020 7769  ).            wi
-00002910: 7468 206d 6f76 655f 6f6e 5f61 6674 6572  th move_on_after
-00002920: 2830 2e31 293a 0a20 2020 2020 2020 2020  (0.1):.         
-00002930: 2020 2020 2020 2077 6869 6c65 2074 696d         while tim
-00002940: 652e 6d6f 6e6f 746f 6e69 6328 2920 2d20  e.monotonic() - 
-00002950: 7374 6172 745f 7469 6d65 203c 2030 2e33  start_time < 0.3
-00002960: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002970: 2020 2020 2020 6177 6169 7420 7374 7265        await stre
-00002980: 616d 2e72 6563 6569 7665 2831 290a 0a20  am.receive(1).. 
-00002990: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000029a0: 7974 6573 742e 6661 696c 2822 5468 6520  ytest.fail("The 
-000029b0: 7469 6d65 6f75 7420 7761 7320 6e6f 7420  timeout was not 
-000029c0: 7265 7370 6563 7465 6422 290a 0a20 2020  respected")..   
-000029d0: 2061 7379 6e63 2064 6566 2074 6573 745f   async def test_
-000029e0: 636f 6e63 7572 7265 6e74 5f73 656e 6428  concurrent_send(
-000029f0: 7365 6c66 2c20 7365 7276 6572 5f61 6464  self, server_add
-00002a00: 723a 2074 7570 6c65 5b73 7472 2c20 696e  r: tuple[str, in
-00002a10: 745d 2920 2d3e 204e 6f6e 653a 0a20 2020  t]) -> None:.   
-00002a20: 2020 2020 2061 7379 6e63 2064 6566 2073       async def s
-00002a30: 656e 645f 6461 7461 2829 202d 3e20 4e6f  end_data() -> No
-00002a40: 5265 7475 726e 3a0a 2020 2020 2020 2020  Return:.        
-00002a50: 2020 2020 7768 696c 6520 5472 7565 3a0a      while True:.
-00002a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a70: 6177 6169 7420 7374 7265 616d 2e73 656e  await stream.sen
-00002a80: 6428 6222 5c78 3030 2220 2a20 3430 3936  d(b"\x00" * 4096
-00002a90: 290a 0a20 2020 2020 2020 2061 7379 6e63  )..        async
-00002aa0: 2077 6974 6820 6177 6169 7420 636f 6e6e   with await conn
-00002ab0: 6563 745f 7463 7028 2a73 6572 7665 725f  ect_tcp(*server_
-00002ac0: 6164 6472 2920 6173 2073 7472 6561 6d3a  addr) as stream:
-00002ad0: 0a20 2020 2020 2020 2020 2020 2061 7379  .            asy
-00002ae0: 6e63 2077 6974 6820 6372 6561 7465 5f74  nc with create_t
-00002af0: 6173 6b5f 6772 6f75 7028 2920 6173 2074  ask_group() as t
-00002b00: 673a 0a20 2020 2020 2020 2020 2020 2020  g:.             
-00002b10: 2020 2074 672e 7374 6172 745f 736f 6f6e     tg.start_soon
-00002b20: 2873 656e 645f 6461 7461 290a 2020 2020  (send_data).    
-00002b30: 2020 2020 2020 2020 2020 2020 6177 6169              awai
-00002b40: 7420 7761 6974 5f61 6c6c 5f74 6173 6b73  t wait_all_tasks
-00002b50: 5f62 6c6f 636b 6564 2829 0a20 2020 2020  _blocked().     
-00002b60: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00002b70: 7079 7465 7374 2e72 6169 7365 7328 4275  pytest.raises(Bu
-00002b80: 7379 5265 736f 7572 6365 4572 726f 7229  syResourceError)
-00002b90: 2061 7320 6578 633a 0a20 2020 2020 2020   as exc:.       
-00002ba0: 2020 2020 2020 2020 2020 2020 2061 7761               awa
-00002bb0: 6974 2073 7472 6561 6d2e 7365 6e64 2862  it stream.send(b
-00002bc0: 2266 6f6f 2229 0a0a 2020 2020 2020 2020  "foo")..        
-00002bd0: 2020 2020 2020 2020 6578 632e 6d61 7463          exc.matc
-00002be0: 6828 2261 6c72 6561 6479 2077 7269 7469  h("already writi
-00002bf0: 6e67 2074 6f22 290a 2020 2020 2020 2020  ng to").        
-00002c00: 2020 2020 2020 2020 7467 2e63 616e 6365          tg.cance
-00002c10: 6c5f 7363 6f70 652e 6361 6e63 656c 2829  l_scope.cancel()
-00002c20: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-00002c30: 7465 7374 5f63 6f6e 6375 7272 656e 745f  test_concurrent_
-00002c40: 7265 6365 6976 6528 7365 6c66 2c20 7365  receive(self, se
-00002c50: 7276 6572 5f61 6464 723a 2074 7570 6c65  rver_addr: tuple
-00002c60: 5b73 7472 2c20 696e 745d 2920 2d3e 204e  [str, int]) -> N
-00002c70: 6f6e 653a 0a20 2020 2020 2020 2061 7379  one:.        asy
-00002c80: 6e63 2077 6974 6820 6177 6169 7420 636f  nc with await co
-00002c90: 6e6e 6563 745f 7463 7028 2a73 6572 7665  nnect_tcp(*serve
-00002ca0: 725f 6164 6472 2920 6173 2063 6c69 656e  r_addr) as clien
-00002cb0: 743a 0a20 2020 2020 2020 2020 2020 2061  t:.            a
-00002cc0: 7379 6e63 2077 6974 6820 6372 6561 7465  sync with create
-00002cd0: 5f74 6173 6b5f 6772 6f75 7028 2920 6173  _task_group() as
-00002ce0: 2074 673a 0a20 2020 2020 2020 2020 2020   tg:.           
-00002cf0: 2020 2020 2074 672e 7374 6172 745f 736f       tg.start_so
-00002d00: 6f6e 2863 6c69 656e 742e 7265 6365 6976  on(client.receiv
-00002d10: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00002d20: 2020 2061 7761 6974 2077 6169 745f 616c     await wait_al
-00002d30: 6c5f 7461 736b 735f 626c 6f63 6b65 6428  l_tasks_blocked(
-00002d40: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00002d50: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00002d60: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00002d70: 7079 7465 7374 2e72 6169 7365 7328 4275  pytest.raises(Bu
-00002d80: 7379 5265 736f 7572 6365 4572 726f 7229  syResourceError)
-00002d90: 2061 7320 6578 633a 0a20 2020 2020 2020   as exc:.       
-00002da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002db0: 2061 7761 6974 2063 6c69 656e 742e 7265   await client.re
-00002dc0: 6365 6976 6528 290a 0a20 2020 2020 2020  ceive()..       
-00002dd0: 2020 2020 2020 2020 2020 2020 2065 7863               exc
-00002de0: 2e6d 6174 6368 2822 616c 7265 6164 7920  .match("already 
-00002df0: 7265 6164 696e 6720 6672 6f6d 2229 0a20  reading from"). 
-00002e00: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00002e10: 696e 616c 6c79 3a0a 2020 2020 2020 2020  inally:.        
-00002e20: 2020 2020 2020 2020 2020 2020 7467 2e63              tg.c
-00002e30: 616e 6365 6c5f 7363 6f70 652e 6361 6e63  ancel_scope.canc
-00002e40: 656c 2829 0a0a 2020 2020 6173 796e 6320  el()..    async 
-00002e50: 6465 6620 7465 7374 5f63 6c6f 7365 5f64  def test_close_d
-00002e60: 7572 696e 675f 7265 6365 6976 6528 7365  uring_receive(se
-00002e70: 6c66 2c20 7365 7276 6572 5f61 6464 723a  lf, server_addr:
-00002e80: 2074 7570 6c65 5b73 7472 2c20 696e 745d   tuple[str, int]
-00002e90: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00002ea0: 2020 2061 7379 6e63 2064 6566 2069 6e74     async def int
-00002eb0: 6572 7275 7074 2829 202d 3e20 4e6f 6e65  errupt() -> None
-00002ec0: 3a0a 2020 2020 2020 2020 2020 2020 6177  :.            aw
-00002ed0: 6169 7420 7761 6974 5f61 6c6c 5f74 6173  ait wait_all_tas
-00002ee0: 6b73 5f62 6c6f 636b 6564 2829 0a20 2020  ks_blocked().   
-00002ef0: 2020 2020 2020 2020 2061 7761 6974 2073           await s
-00002f00: 7472 6561 6d2e 6163 6c6f 7365 2829 0a0a  tream.aclose()..
-00002f10: 2020 2020 2020 2020 6173 796e 6320 7769          async wi
-00002f20: 7468 2061 7761 6974 2063 6f6e 6e65 6374  th await connect
-00002f30: 5f74 6370 282a 7365 7276 6572 5f61 6464  _tcp(*server_add
-00002f40: 7229 2061 7320 7374 7265 616d 3a0a 2020  r) as stream:.  
-00002f50: 2020 2020 2020 2020 2020 6173 796e 6320            async 
-00002f60: 7769 7468 2063 7265 6174 655f 7461 736b  with create_task
-00002f70: 5f67 726f 7570 2829 2061 7320 7467 3a0a  _group() as tg:.
-00002f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f90: 7467 2e73 7461 7274 5f73 6f6f 6e28 696e  tg.start_soon(in
-00002fa0: 7465 7272 7570 7429 0a20 2020 2020 2020  terrupt).       
-00002fb0: 2020 2020 2020 2020 2077 6974 6820 7079           with py
-00002fc0: 7465 7374 2e72 6169 7365 7328 436c 6f73  test.raises(Clos
-00002fd0: 6564 5265 736f 7572 6365 4572 726f 7229  edResourceError)
-00002fe0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002ff0: 2020 2020 2020 6177 6169 7420 7374 7265        await stre
-00003000: 616d 2e72 6563 6569 7665 2829 0a0a 2020  am.receive()..  
-00003010: 2020 6173 796e 6320 6465 6620 7465 7374    async def test
-00003020: 5f72 6563 6569 7665 5f61 6674 6572 5f63  _receive_after_c
-00003030: 6c6f 7365 2873 656c 662c 2073 6572 7665  lose(self, serve
-00003040: 725f 6164 6472 3a20 7475 706c 655b 7374  r_addr: tuple[st
-00003050: 722c 2069 6e74 5d29 202d 3e20 4e6f 6e65  r, int]) -> None
-00003060: 3a0a 2020 2020 2020 2020 7374 7265 616d  :.        stream
-00003070: 203d 2061 7761 6974 2063 6f6e 6e65 6374   = await connect
-00003080: 5f74 6370 282a 7365 7276 6572 5f61 6464  _tcp(*server_add
-00003090: 7229 0a20 2020 2020 2020 2061 7761 6974  r).        await
-000030a0: 2073 7472 6561 6d2e 6163 6c6f 7365 2829   stream.aclose()
-000030b0: 0a20 2020 2020 2020 2077 6974 6820 7079  .        with py
-000030c0: 7465 7374 2e72 6169 7365 7328 436c 6f73  test.raises(Clos
-000030d0: 6564 5265 736f 7572 6365 4572 726f 7229  edResourceError)
-000030e0: 3a0a 2020 2020 2020 2020 2020 2020 6177  :.            aw
-000030f0: 6169 7420 7374 7265 616d 2e72 6563 6569  ait stream.recei
-00003100: 7665 2829 0a0a 2020 2020 6173 796e 6320  ve()..    async 
-00003110: 6465 6620 7465 7374 5f73 656e 645f 6166  def test_send_af
-00003120: 7465 725f 636c 6f73 6528 7365 6c66 2c20  ter_close(self, 
-00003130: 7365 7276 6572 5f61 6464 723a 2074 7570  server_addr: tup
-00003140: 6c65 5b73 7472 2c20 696e 745d 2920 2d3e  le[str, int]) ->
-00003150: 204e 6f6e 653a 0a20 2020 2020 2020 2073   None:.        s
-00003160: 7472 6561 6d20 3d20 6177 6169 7420 636f  tream = await co
-00003170: 6e6e 6563 745f 7463 7028 2a73 6572 7665  nnect_tcp(*serve
-00003180: 725f 6164 6472 290a 2020 2020 2020 2020  r_addr).        
-00003190: 6177 6169 7420 7374 7265 616d 2e61 636c  await stream.acl
-000031a0: 6f73 6528 290a 2020 2020 2020 2020 7769  ose().        wi
-000031b0: 7468 2070 7974 6573 742e 7261 6973 6573  th pytest.raises
-000031c0: 2843 6c6f 7365 6452 6573 6f75 7263 6545  (ClosedResourceE
-000031d0: 7272 6f72 293a 0a20 2020 2020 2020 2020  rror):.         
-000031e0: 2020 2061 7761 6974 2073 7472 6561 6d2e     await stream.
-000031f0: 7365 6e64 2862 2266 6f6f 2229 0a0a 2020  send(b"foo")..  
-00003200: 2020 6173 796e 6320 6465 6620 7465 7374    async def test
-00003210: 5f73 656e 645f 6166 7465 725f 7065 6572  _send_after_peer
-00003220: 5f63 6c6f 7365 6428 7365 6c66 2c20 6661  _closed(self, fa
-00003230: 6d69 6c79 3a20 416e 7949 5041 6464 7265  mily: AnyIPAddre
-00003240: 7373 4661 6d69 6c79 2920 2d3e 204e 6f6e  ssFamily) -> Non
-00003250: 653a 0a20 2020 2020 2020 2064 6566 2073  e:.        def s
-00003260: 6572 7665 5f6f 6e63 6528 2920 2d3e 204e  erve_once() -> N
-00003270: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00003280: 2063 6c69 656e 745f 736f 636b 2c20 5f20   client_sock, _ 
-00003290: 3d20 7365 7276 6572 5f73 6f63 6b2e 6163  = server_sock.ac
-000032a0: 6365 7074 2829 0a20 2020 2020 2020 2020  cept().         
-000032b0: 2020 2063 6c69 656e 745f 736f 636b 2e63     client_sock.c
-000032c0: 6c6f 7365 2829 0a20 2020 2020 2020 2020  lose().         
-000032d0: 2020 2073 6572 7665 725f 736f 636b 2e63     server_sock.c
-000032e0: 6c6f 7365 2829 0a0a 2020 2020 2020 2020  lose()..        
-000032f0: 7365 7276 6572 5f73 6f63 6b20 3d20 736f  server_sock = so
-00003300: 636b 6574 2e73 6f63 6b65 7428 6661 6d69  cket.socket(fami
-00003310: 6c79 2c20 736f 636b 6574 2e53 4f43 4b5f  ly, socket.SOCK_
-00003320: 5354 5245 414d 290a 2020 2020 2020 2020  STREAM).        
-00003330: 7365 7276 6572 5f73 6f63 6b2e 7365 7474  server_sock.sett
-00003340: 696d 656f 7574 2831 290a 2020 2020 2020  imeout(1).      
-00003350: 2020 7365 7276 6572 5f73 6f63 6b2e 6269    server_sock.bi
-00003360: 6e64 2828 226c 6f63 616c 686f 7374 222c  nd(("localhost",
-00003370: 2030 2929 0a20 2020 2020 2020 2073 6572   0)).        ser
-00003380: 7665 725f 6164 6472 203d 2073 6572 7665  ver_addr = serve
-00003390: 725f 736f 636b 2e67 6574 736f 636b 6e61  r_sock.getsockna
-000033a0: 6d65 2829 5b3a 325d 0a20 2020 2020 2020  me()[:2].       
-000033b0: 2073 6572 7665 725f 736f 636b 2e6c 6973   server_sock.lis
-000033c0: 7465 6e28 290a 2020 2020 2020 2020 7468  ten().        th
-000033d0: 7265 6164 203d 2054 6872 6561 6428 7461  read = Thread(ta
-000033e0: 7267 6574 3d73 6572 7665 5f6f 6e63 652c  rget=serve_once,
-000033f0: 2064 6165 6d6f 6e3d 5472 7565 290a 2020   daemon=True).  
-00003400: 2020 2020 2020 7468 7265 6164 2e73 7461        thread.sta
-00003410: 7274 2829 0a0a 2020 2020 2020 2020 7769  rt()..        wi
-00003420: 7468 2070 7974 6573 742e 7261 6973 6573  th pytest.raises
-00003430: 2842 726f 6b65 6e52 6573 6f75 7263 6545  (BrokenResourceE
-00003440: 7272 6f72 293a 0a20 2020 2020 2020 2020  rror):.         
-00003450: 2020 2061 7379 6e63 2077 6974 6820 6177     async with aw
-00003460: 6169 7420 636f 6e6e 6563 745f 7463 7028  ait connect_tcp(
-00003470: 2a73 6572 7665 725f 6164 6472 2920 6173  *server_addr) as
-00003480: 2073 7472 6561 6d3a 0a20 2020 2020 2020   stream:.       
-00003490: 2020 2020 2020 2020 2066 6f72 205f 2069           for _ i
-000034a0: 6e20 7261 6e67 6528 3130 3030 293a 0a20  n range(1000):. 
-000034b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034c0: 2020 2061 7761 6974 2073 7472 6561 6d2e     await stream.
-000034d0: 7365 6e64 2862 2266 6f6f 2229 0a0a 2020  send(b"foo")..  
-000034e0: 2020 2020 2020 7468 7265 6164 2e6a 6f69        thread.joi
-000034f0: 6e28 290a 0a20 2020 2061 7379 6e63 2064  n()..    async d
-00003500: 6566 2074 6573 745f 636f 6e6e 6563 745f  ef test_connect_
-00003510: 7463 705f 7769 7468 5f74 6c73 280a 2020  tcp_with_tls(.  
-00003520: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00003530: 2020 2020 7365 7276 6572 5f63 6f6e 7465      server_conte
-00003540: 7874 3a20 5353 4c43 6f6e 7465 7874 2c0a  xt: SSLContext,.
-00003550: 2020 2020 2020 2020 636c 6965 6e74 5f63          client_c
-00003560: 6f6e 7465 7874 3a20 5353 4c43 6f6e 7465  ontext: SSLConte
-00003570: 7874 2c0a 2020 2020 2020 2020 7365 7276  xt,.        serv
-00003580: 6572 5f73 6f63 6b3a 2073 6f63 6b65 742e  er_sock: socket.
-00003590: 736f 636b 6574 2c0a 2020 2020 2020 2020  socket,.        
-000035a0: 7365 7276 6572 5f61 6464 723a 2074 7570  server_addr: tup
-000035b0: 6c65 5b73 7472 2c20 696e 745d 2c0a 2020  le[str, int],.  
-000035c0: 2020 2920 2d3e 204e 6f6e 653a 0a20 2020    ) -> None:.   
-000035d0: 2020 2020 2064 6566 2073 6572 7665 2829       def serve()
-000035e0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-000035f0: 2020 2020 2020 7769 7468 2073 7570 7072        with suppr
-00003600: 6573 7328 736f 636b 6574 2e74 696d 656f  ess(socket.timeo
-00003610: 7574 293a 0a20 2020 2020 2020 2020 2020  ut):.           
-00003620: 2020 2020 2063 6c69 656e 742c 2061 6464       client, add
-00003630: 7220 3d20 7365 7276 6572 5f73 6f63 6b2e  r = server_sock.
-00003640: 6163 6365 7074 2829 0a20 2020 2020 2020  accept().       
-00003650: 2020 2020 2020 2020 2063 6c69 656e 742e           client.
-00003660: 7365 7474 696d 656f 7574 2831 290a 2020  settimeout(1).  
-00003670: 2020 2020 2020 2020 2020 2020 2020 636c                cl
-00003680: 6965 6e74 203d 2073 6572 7665 725f 636f  ient = server_co
-00003690: 6e74 6578 742e 7772 6170 5f73 6f63 6b65  ntext.wrap_socke
-000036a0: 7428 636c 6965 6e74 2c20 7365 7276 6572  t(client, server
-000036b0: 5f73 6964 653d 5472 7565 290a 2020 2020  _side=True).    
-000036c0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-000036d0: 203d 2063 6c69 656e 742e 7265 6376 2831   = client.recv(1
-000036e0: 3030 290a 2020 2020 2020 2020 2020 2020  00).            
-000036f0: 2020 2020 636c 6965 6e74 2e73 656e 6461      client.senda
-00003700: 6c6c 2864 6174 615b 3a3a 2d31 5d29 0a20  ll(data[::-1]). 
-00003710: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00003720: 6c69 656e 742e 756e 7772 6170 2829 0a20  lient.unwrap(). 
-00003730: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00003740: 6c69 656e 742e 636c 6f73 6528 290a 0a20  lient.close().. 
-00003750: 2020 2020 2020 2023 2054 6865 2054 4c53         # The TLS
-00003760: 5374 7265 616d 2074 6573 7473 2061 7265  Stream tests are
-00003770: 206d 6f72 6520 636f 6d70 7265 6865 6e73   more comprehens
-00003780: 6976 6520 7468 616e 2074 6869 7320 6f6e  ive than this on
-00003790: 6521 0a20 2020 2020 2020 2074 6872 6561  e!.        threa
-000037a0: 6420 3d20 5468 7265 6164 2874 6172 6765  d = Thread(targe
-000037b0: 743d 7365 7276 652c 2064 6165 6d6f 6e3d  t=serve, daemon=
-000037c0: 5472 7565 290a 2020 2020 2020 2020 7468  True).        th
-000037d0: 7265 6164 2e73 7461 7274 2829 0a20 2020  read.start().   
-000037e0: 2020 2020 2061 7379 6e63 2077 6974 6820       async with 
-000037f0: 6177 6169 7420 636f 6e6e 6563 745f 7463  await connect_tc
-00003800: 7028 0a20 2020 2020 2020 2020 2020 202a  p(.            *
-00003810: 7365 7276 6572 5f61 6464 722c 2074 6c73  server_addr, tls
-00003820: 5f68 6f73 746e 616d 653d 226c 6f63 616c  _hostname="local
-00003830: 686f 7374 222c 2073 736c 5f63 6f6e 7465  host", ssl_conte
-00003840: 7874 3d63 6c69 656e 745f 636f 6e74 6578  xt=client_contex
-00003850: 740a 2020 2020 2020 2020 2920 6173 2073  t.        ) as s
-00003860: 7472 6561 6d3a 0a20 2020 2020 2020 2020  tream:.         
-00003870: 2020 2061 7761 6974 2073 7472 6561 6d2e     await stream.
-00003880: 7365 6e64 2862 2268 656c 6c6f 2229 0a20  send(b"hello"). 
-00003890: 2020 2020 2020 2020 2020 2072 6573 706f             respo
-000038a0: 6e73 6520 3d20 6177 6169 7420 7374 7265  nse = await stre
-000038b0: 616d 2e72 6563 6569 7665 2829 0a0a 2020  am.receive()..  
-000038c0: 2020 2020 2020 6173 7365 7274 2072 6573        assert res
-000038d0: 706f 6e73 6520 3d3d 2062 226f 6c6c 6568  ponse == b"olleh
-000038e0: 220a 2020 2020 2020 2020 7468 7265 6164  ".        thread
-000038f0: 2e6a 6f69 6e28 290a 0a20 2020 2061 7379  .join()..    asy
-00003900: 6e63 2064 6566 2074 6573 745f 636f 6e6e  nc def test_conn
-00003910: 6563 745f 7463 705f 7769 7468 5f74 6c73  ect_tcp_with_tls
-00003920: 5f63 6572 745f 6368 6563 6b5f 6661 696c  _cert_check_fail
-00003930: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00003940: 2020 2020 2020 2020 7365 7276 6572 5f63          server_c
-00003950: 6f6e 7465 7874 3a20 5353 4c43 6f6e 7465  ontext: SSLConte
-00003960: 7874 2c0a 2020 2020 2020 2020 7365 7276  xt,.        serv
-00003970: 6572 5f73 6f63 6b3a 2073 6f63 6b65 742e  er_sock: socket.
-00003980: 736f 636b 6574 2c0a 2020 2020 2020 2020  socket,.        
-00003990: 7365 7276 6572 5f61 6464 723a 2074 7570  server_addr: tup
-000039a0: 6c65 5b73 7472 2c20 696e 745d 2c0a 2020  le[str, int],.  
-000039b0: 2020 2920 2d3e 204e 6f6e 653a 0a20 2020    ) -> None:.   
-000039c0: 2020 2020 2074 6872 6561 645f 6578 6365       thread_exce
-000039d0: 7074 696f 6e20 3d20 4e6f 6e65 0a0a 2020  ption = None..  
-000039e0: 2020 2020 2020 6465 6620 7365 7276 6528        def serve(
-000039f0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00003a00: 2020 2020 2020 206e 6f6e 6c6f 6361 6c20         nonlocal 
-00003a10: 7468 7265 6164 5f65 7863 6570 7469 6f6e  thread_exception
-00003a20: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
-00003a30: 656e 742c 2061 6464 7220 3d20 7365 7276  ent, addr = serv
-00003a40: 6572 5f73 6f63 6b2e 6163 6365 7074 2829  er_sock.accept()
-00003a50: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-00003a60: 6820 636c 6965 6e74 3a0a 2020 2020 2020  h client:.      
-00003a70: 2020 2020 2020 2020 2020 636c 6965 6e74            client
-00003a80: 2e73 6574 7469 6d65 6f75 7428 3129 0a20  .settimeout(1). 
-00003a90: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00003aa0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00003ab0: 2020 2020 2020 2020 7365 7276 6572 5f63          server_c
-00003ac0: 6f6e 7465 7874 2e77 7261 705f 736f 636b  ontext.wrap_sock
-00003ad0: 6574 2863 6c69 656e 742c 2073 6572 7665  et(client, serve
-00003ae0: 725f 7369 6465 3d54 7275 6529 0a20 2020  r_side=True).   
-00003af0: 2020 2020 2020 2020 2020 2020 2065 7863               exc
-00003b00: 6570 7420 4f53 4572 726f 723a 0a20 2020  ept OSError:.   
-00003b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b20: 2070 6173 730a 2020 2020 2020 2020 2020   pass.          
-00003b30: 2020 2020 2020 6578 6365 7074 2042 6173        except Bas
-00003b40: 6545 7863 6570 7469 6f6e 2061 7320 6578  eException as ex
-00003b50: 633a 0a20 2020 2020 2020 2020 2020 2020  c:.             
-00003b60: 2020 2020 2020 2074 6872 6561 645f 6578         thread_ex
-00003b70: 6365 7074 696f 6e20 3d20 6578 630a 0a20  ception = exc.. 
-00003b80: 2020 2020 2020 2074 6872 6561 6420 3d20         thread = 
-00003b90: 5468 7265 6164 2874 6172 6765 743d 7365  Thread(target=se
-00003ba0: 7276 652c 2064 6165 6d6f 6e3d 5472 7565  rve, daemon=True
-00003bb0: 290a 2020 2020 2020 2020 7468 7265 6164  ).        thread
-00003bc0: 2e73 7461 7274 2829 0a20 2020 2020 2020  .start().       
-00003bd0: 2077 6974 6820 7079 7465 7374 2e72 6169   with pytest.rai
-00003be0: 7365 7328 5353 4c45 7272 6f72 293a 0a20  ses(SSLError):. 
-00003bf0: 2020 2020 2020 2020 2020 2061 7761 6974             await
-00003c00: 2063 6f6e 6e65 6374 5f74 6370 282a 7365   connect_tcp(*se
-00003c10: 7276 6572 5f61 6464 722c 2074 6c73 5f68  rver_addr, tls_h
-00003c20: 6f73 746e 616d 653d 226c 6f63 616c 686f  ostname="localho
-00003c30: 7374 2229 0a0a 2020 2020 2020 2020 7468  st")..        th
-00003c40: 7265 6164 2e6a 6f69 6e28 290a 2020 2020  read.join().    
-00003c50: 2020 2020 6173 7365 7274 2074 6872 6561      assert threa
-00003c60: 645f 6578 6365 7074 696f 6e20 6973 204e  d_exception is N
-00003c70: 6f6e 650a 0a20 2020 2040 7079 7465 7374  one..    @pytest
-00003c80: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
-00003c90: 6528 2261 6e79 696f 5f62 6163 6b65 6e64  e("anyio_backend
-00003ca0: 222c 205b 2261 7379 6e63 696f 225d 290a  ", ["asyncio"]).
-00003cb0: 2020 2020 6173 796e 6320 6465 6620 7465      async def te
-00003cc0: 7374 5f75 6e72 6574 7269 6576 6564 5f66  st_unretrieved_f
-00003cd0: 7574 7572 655f 6578 6365 7074 696f 6e5f  uture_exception_
-00003ce0: 7365 7276 6572 5f63 7261 7368 280a 2020  server_crash(.  
-00003cf0: 2020 2020 2020 7365 6c66 2c20 6661 6d69        self, fami
-00003d00: 6c79 3a20 416e 7949 5041 6464 7265 7373  ly: AnyIPAddress
-00003d10: 4661 6d69 6c79 2c20 6361 706c 6f67 3a20  Family, caplog: 
-00003d20: 4c6f 6743 6170 7475 7265 4669 7874 7572  LogCaptureFixtur
-00003d30: 650a 2020 2020 2920 2d3e 204e 6f6e 653a  e.    ) -> None:
-00003d40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00003d50: 2020 2020 2054 6573 7420 7468 6174 2074       Test that t
-00003d60: 6865 7265 2077 6f6e 2774 2062 6520 616e  here won't be an
-00003d70: 7920 6c65 6674 6f76 6572 2046 7574 7572  y leftover Futur
-00003d80: 6573 2074 6861 7420 646f 6e27 7420 6765  es that don't ge
-00003d90: 7420 7468 6569 7220 6578 6365 7074 696f  t their exceptio
-00003da0: 6e73 0a20 2020 2020 2020 2072 6574 7269  ns.        retri
-00003db0: 6576 6564 2e0a 0a20 2020 2020 2020 2053  eved...        S
-00003dc0: 6565 2068 7474 7073 3a2f 2f67 6974 6875  ee https://githu
-00003dd0: 622e 636f 6d2f 656e 636f 6465 2f68 7474  b.com/encode/htt
-00003de0: 7063 6f72 652f 6973 7375 6573 2f33 3832  pcore/issues/382
-00003df0: 2066 6f72 2064 6574 6169 6c73 2e0a 0a20   for details... 
-00003e00: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-00003e10: 2020 2020 6465 6620 7365 7276 6528 2920      def serve() 
-00003e20: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00003e30: 2020 2020 2073 6f63 6b2c 2061 6464 7220       sock, addr 
-00003e40: 3d20 7365 7276 6572 5f73 6f63 6b2e 6163  = server_sock.ac
-00003e50: 6365 7074 2829 0a20 2020 2020 2020 2020  cept().         
-00003e60: 2020 2065 7665 6e74 2e77 6169 7428 3329     event.wait(3)
-00003e70: 0a20 2020 2020 2020 2020 2020 2064 656c  .            del
-00003e80: 2073 6f63 6b0a 2020 2020 2020 2020 2020   sock.          
-00003e90: 2020 6763 2e63 6f6c 6c65 6374 2829 0a0a    gc.collect()..
-00003ea0: 2020 2020 2020 2020 7365 7276 6572 5f73          server_s
-00003eb0: 6f63 6b20 3d20 736f 636b 6574 2e73 6f63  ock = socket.soc
-00003ec0: 6b65 7428 6661 6d69 6c79 2c20 736f 636b  ket(family, sock
-00003ed0: 6574 2e53 4f43 4b5f 5354 5245 414d 290a  et.SOCK_STREAM).
-00003ee0: 2020 2020 2020 2020 7365 7276 6572 5f73          server_s
-00003ef0: 6f63 6b2e 7365 7474 696d 656f 7574 2831  ock.settimeout(1
-00003f00: 290a 2020 2020 2020 2020 7365 7276 6572  ).        server
-00003f10: 5f73 6f63 6b2e 6269 6e64 2828 226c 6f63  _sock.bind(("loc
-00003f20: 616c 686f 7374 222c 2030 2929 0a20 2020  alhost", 0)).   
-00003f30: 2020 2020 2073 6572 7665 725f 736f 636b       server_sock
-00003f40: 2e6c 6973 7465 6e28 290a 2020 2020 2020  .listen().      
-00003f50: 2020 7365 7276 6572 5f61 6464 7220 3d20    server_addr = 
-00003f60: 7365 7276 6572 5f73 6f63 6b2e 6765 7473  server_sock.gets
-00003f70: 6f63 6b6e 616d 6528 295b 3a32 5d0a 2020  ockname()[:2].  
-00003f80: 2020 2020 2020 6576 656e 7420 3d20 7468        event = th
-00003f90: 7265 6164 696e 672e 4576 656e 7428 290a  reading.Event().
-00003fa0: 2020 2020 2020 2020 7468 7265 6164 203d          thread =
-00003fb0: 2054 6872 6561 6428 7461 7267 6574 3d73   Thread(target=s
-00003fc0: 6572 7665 290a 2020 2020 2020 2020 7468  erve).        th
-00003fd0: 7265 6164 2e73 7461 7274 2829 0a20 2020  read.start().   
-00003fe0: 2020 2020 2061 7379 6e63 2077 6974 6820       async with 
-00003ff0: 6177 6169 7420 636f 6e6e 6563 745f 7463  await connect_tc
-00004000: 7028 2a73 6572 7665 725f 6164 6472 2920  p(*server_addr) 
-00004010: 6173 2073 7472 6561 6d3a 0a20 2020 2020  as stream:.     
-00004020: 2020 2020 2020 2061 7761 6974 2073 7472         await str
-00004030: 6561 6d2e 7365 6e64 2862 2247 4554 2229  eam.send(b"GET")
-00004040: 0a20 2020 2020 2020 2020 2020 2065 7665  .            eve
-00004050: 6e74 2e73 6574 2829 0a20 2020 2020 2020  nt.set().       
-00004060: 2020 2020 2077 6974 6820 7079 7465 7374       with pytest
-00004070: 2e72 6169 7365 7328 4272 6f6b 656e 5265  .raises(BrokenRe
-00004080: 736f 7572 6365 4572 726f 7229 3a0a 2020  sourceError):.  
-00004090: 2020 2020 2020 2020 2020 2020 2020 6177                aw
-000040a0: 6169 7420 7374 7265 616d 2e72 6563 6569  ait stream.recei
-000040b0: 7665 2829 0a0a 2020 2020 2020 2020 7468  ve()..        th
-000040c0: 7265 6164 2e6a 6f69 6e28 290a 2020 2020  read.join().    
-000040d0: 2020 2020 6763 2e63 6f6c 6c65 6374 2829      gc.collect()
-000040e0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-000040f0: 6e6f 7420 6361 706c 6f67 2e74 6578 740a  not caplog.text.
-00004100: 0a0a 4070 7974 6573 742e 6d61 726b 2e6e  ..@pytest.mark.n
-00004110: 6574 776f 726b 0a63 6c61 7373 2054 6573  etwork.class Tes
-00004120: 7454 4350 4c69 7374 656e 6572 3a0a 2020  tTCPListener:.  
-00004130: 2020 6173 796e 6320 6465 6620 7465 7374    async def test
-00004140: 5f65 7874 7261 5f61 7474 7269 6275 7465  _extra_attribute
-00004150: 7328 7365 6c66 2c20 6661 6d69 6c79 3a20  s(self, family: 
-00004160: 416e 7949 5041 6464 7265 7373 4661 6d69  AnyIPAddressFami
-00004170: 6c79 2920 2d3e 204e 6f6e 653a 0a20 2020  ly) -> None:.   
-00004180: 2020 2020 2061 7379 6e63 2077 6974 6820       async with 
-00004190: 6177 6169 7420 6372 6561 7465 5f74 6370  await create_tcp
-000041a0: 5f6c 6973 7465 6e65 7228 0a20 2020 2020  _listener(.     
-000041b0: 2020 2020 2020 206c 6f63 616c 5f68 6f73         local_hos
-000041c0: 743d 226c 6f63 616c 686f 7374 222c 2066  t="localhost", f
-000041d0: 616d 696c 793d 6661 6d69 6c79 0a20 2020  amily=family.   
-000041e0: 2020 2020 2029 2061 7320 6d75 6c74 693a       ) as multi:
-000041f0: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-00004200: 6572 7420 6d75 6c74 692e 6578 7472 6128  ert multi.extra(
-00004210: 536f 636b 6574 4174 7472 6962 7574 652e  SocketAttribute.
-00004220: 6661 6d69 6c79 2920 3d3d 2066 616d 696c  family) == famil
-00004230: 790a 2020 2020 2020 2020 2020 2020 666f  y.            fo
-00004240: 7220 6c69 7374 656e 6572 2069 6e20 6d75  r listener in mu
-00004250: 6c74 692e 6c69 7374 656e 6572 733a 0a20  lti.listeners:. 
-00004260: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00004270: 6177 5f73 6f63 6b65 7420 3d20 6c69 7374  aw_socket = list
-00004280: 656e 6572 2e65 7874 7261 2853 6f63 6b65  ener.extra(Socke
-00004290: 7441 7474 7269 6275 7465 2e72 6177 5f73  tAttribute.raw_s
-000042a0: 6f63 6b65 7429 0a20 2020 2020 2020 2020  ocket).         
-000042b0: 2020 2020 2020 2061 7373 6572 7420 6c69         assert li
-000042c0: 7374 656e 6572 2e65 7874 7261 2853 6f63  stener.extra(Soc
-000042d0: 6b65 7441 7474 7269 6275 7465 2e66 616d  ketAttribute.fam
-000042e0: 696c 7929 203d 3d20 6661 6d69 6c79 0a20  ily) == family. 
-000042f0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00004300: 7373 6572 7420 280a 2020 2020 2020 2020  ssert (.        
-00004310: 2020 2020 2020 2020 2020 2020 6c69 7374              list
-00004320: 656e 6572 2e65 7874 7261 2853 6f63 6b65  ener.extra(Socke
-00004330: 7441 7474 7269 6275 7465 2e6c 6f63 616c  tAttribute.local
-00004340: 5f61 6464 7265 7373 290a 2020 2020 2020  _address).      
-00004350: 2020 2020 2020 2020 2020 2020 2020 3d3d                ==
-00004360: 2072 6177 5f73 6f63 6b65 742e 6765 7473   raw_socket.gets
-00004370: 6f63 6b6e 616d 6528 295b 3a32 5d0a 2020  ockname()[:2].  
-00004380: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00004390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043a0: 6173 7365 7274 2028 0a20 2020 2020 2020  assert (.       
-000043b0: 2020 2020 2020 2020 2020 2020 206c 6973               lis
-000043c0: 7465 6e65 722e 6578 7472 6128 536f 636b  tener.extra(Sock
-000043d0: 6574 4174 7472 6962 7574 652e 6c6f 6361  etAttribute.loca
-000043e0: 6c5f 706f 7274 290a 2020 2020 2020 2020  l_port).        
-000043f0: 2020 2020 2020 2020 2020 2020 3d3d 2072              == r
-00004400: 6177 5f73 6f63 6b65 742e 6765 7473 6f63  aw_socket.getsoc
-00004410: 6b6e 616d 6528 295b 315d 0a20 2020 2020  kname()[1].     
-00004420: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00004430: 2020 2020 2020 2020 2020 2020 2070 7974               pyt
-00004440: 6573 742e 7261 6973 6573 280a 2020 2020  est.raises(.    
-00004450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004460: 5479 7065 6441 7474 7269 6275 7465 4c6f  TypedAttributeLo
-00004470: 6f6b 7570 4572 726f 722c 0a20 2020 2020  okupError,.     
-00004480: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00004490: 6973 7465 6e65 722e 6578 7472 612c 0a20  istener.extra,. 
-000044a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044b0: 2020 2053 6f63 6b65 7441 7474 7269 6275     SocketAttribu
-000044c0: 7465 2e72 656d 6f74 655f 6164 6472 6573  te.remote_addres
-000044d0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-000044e0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-000044f0: 2020 2020 2070 7974 6573 742e 7261 6973       pytest.rais
-00004500: 6573 280a 2020 2020 2020 2020 2020 2020  es(.            
-00004510: 2020 2020 2020 2020 5479 7065 6441 7474          TypedAtt
-00004520: 7269 6275 7465 4c6f 6f6b 7570 4572 726f  ributeLookupErro
-00004530: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-00004540: 2020 2020 2020 206c 6973 7465 6e65 722e         listener.
-00004550: 6578 7472 612c 0a20 2020 2020 2020 2020  extra,.         
-00004560: 2020 2020 2020 2020 2020 2053 6f63 6b65             Socke
-00004570: 7441 7474 7269 6275 7465 2e72 656d 6f74  tAttribute.remot
-00004580: 655f 706f 7274 2c0a 2020 2020 2020 2020  e_port,.        
-00004590: 2020 2020 2020 2020 290a 0a20 2020 2040          )..    @
-000045a0: 7079 7465 7374 2e6d 6172 6b2e 7061 7261  pytest.mark.para
-000045b0: 6d65 7472 697a 6528 0a20 2020 2020 2020  metrize(.       
-000045c0: 2022 6661 6d69 6c79 222c 0a20 2020 2020   "family",.     
-000045d0: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
-000045e0: 2070 7974 6573 742e 7061 7261 6d28 4164   pytest.param(Ad
-000045f0: 6472 6573 7346 616d 696c 792e 4146 5f49  dressFamily.AF_I
-00004600: 4e45 542c 2069 643d 2269 7076 3422 292c  NET, id="ipv4"),
-00004610: 0a20 2020 2020 2020 2020 2020 2070 7974  .            pyt
-00004620: 6573 742e 7061 7261 6d28 4164 6472 6573  est.param(Addres
-00004630: 7346 616d 696c 792e 4146 5f49 4e45 5436  sFamily.AF_INET6
-00004640: 2c20 6964 3d22 6970 7636 222c 206d 6172  , id="ipv6", mar
-00004650: 6b73 3d5b 736b 6970 5f69 7076 365f 6d61  ks=[skip_ipv6_ma
-00004660: 726b 5d29 2c0a 2020 2020 2020 2020 2020  rk]),.          
-00004670: 2020 7079 7465 7374 2e70 6172 616d 2873    pytest.param(s
-00004680: 6f63 6b65 742e 4146 5f55 4e53 5045 432c  ocket.AF_UNSPEC,
-00004690: 2069 643d 2262 6f74 6822 2c20 6d61 726b   id="both", mark
-000046a0: 733d 5b73 6b69 705f 6970 7636 5f6d 6172  s=[skip_ipv6_mar
-000046b0: 6b5d 292c 0a20 2020 2020 2020 205d 2c0a  k]),.        ],.
-000046c0: 2020 2020 290a 2020 2020 6173 796e 6320      ).    async 
-000046d0: 6465 6620 7465 7374 5f61 6363 6570 7428  def test_accept(
-000046e0: 7365 6c66 2c20 6661 6d69 6c79 3a20 416e  self, family: An
-000046f0: 7949 5041 6464 7265 7373 4661 6d69 6c79  yIPAddressFamily
-00004700: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00004710: 2020 2061 7379 6e63 2077 6974 6820 6177     async with aw
-00004720: 6169 7420 6372 6561 7465 5f74 6370 5f6c  ait create_tcp_l
-00004730: 6973 7465 6e65 7228 0a20 2020 2020 2020  istener(.       
-00004740: 2020 2020 206c 6f63 616c 5f68 6f73 743d       local_host=
-00004750: 226c 6f63 616c 686f 7374 222c 2066 616d  "localhost", fam
-00004760: 696c 793d 6661 6d69 6c79 0a20 2020 2020  ily=family.     
-00004770: 2020 2029 2061 7320 6d75 6c74 693a 0a20     ) as multi:. 
-00004780: 2020 2020 2020 2020 2020 2066 6f72 206c             for l
-00004790: 6973 7465 6e65 7220 696e 206d 756c 7469  istener in multi
-000047a0: 2e6c 6973 7465 6e65 7273 3a0a 2020 2020  .listeners:.    
-000047b0: 2020 2020 2020 2020 2020 2020 636c 6965              clie
-000047c0: 6e74 203d 2073 6f63 6b65 742e 736f 636b  nt = socket.sock
-000047d0: 6574 286c 6973 7465 6e65 722e 6578 7472  et(listener.extr
-000047e0: 6128 536f 636b 6574 4174 7472 6962 7574  a(SocketAttribut
-000047f0: 652e 6661 6d69 6c79 2929 0a20 2020 2020  e.family)).     
-00004800: 2020 2020 2020 2020 2020 2063 6c69 656e             clien
-00004810: 742e 7365 7474 696d 656f 7574 2831 290a  t.settimeout(1).
-00004820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004830: 636c 6965 6e74 2e63 6f6e 6e65 6374 286c  client.connect(l
-00004840: 6973 7465 6e65 722e 6578 7472 6128 536f  istener.extra(So
-00004850: 636b 6574 4174 7472 6962 7574 652e 6c6f  cketAttribute.lo
-00004860: 6361 6c5f 6164 6472 6573 7329 290a 2020  cal_address)).  
-00004870: 2020 2020 2020 2020 2020 2020 2020 6173                as
-00004880: 7365 7274 2069 7369 6e73 7461 6e63 6528  sert isinstance(
-00004890: 6c69 7374 656e 6572 2c20 536f 636b 6574  listener, Socket
-000048a0: 4c69 7374 656e 6572 290a 2020 2020 2020  Listener).      
-000048b0: 2020 2020 2020 2020 2020 7374 7265 616d            stream
-000048c0: 203d 2061 7761 6974 206c 6973 7465 6e65   = await listene
-000048d0: 722e 6163 6365 7074 2829 0a20 2020 2020  r.accept().     
-000048e0: 2020 2020 2020 2020 2020 2063 6c69 656e             clien
-000048f0: 742e 7365 6e64 616c 6c28 6222 626c 6168  t.sendall(b"blah
-00004900: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00004910: 2020 2072 6571 7565 7374 203d 2061 7761     request = awa
-00004920: 6974 2073 7472 6561 6d2e 7265 6365 6976  it stream.receiv
-00004930: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-00004940: 2020 2020 6177 6169 7420 7374 7265 616d      await stream
-00004950: 2e73 656e 6428 7265 7175 6573 745b 3a3a  .send(request[::
-00004960: 2d31 5d29 0a20 2020 2020 2020 2020 2020  -1]).           
-00004970: 2020 2020 2061 7373 6572 7420 636c 6965       assert clie
-00004980: 6e74 2e72 6563 7628 3130 3029 203d 3d20  nt.recv(100) == 
-00004990: 6222 6861 6c62 220a 2020 2020 2020 2020  b"halb".        
-000049a0: 2020 2020 2020 2020 636c 6965 6e74 2e63          client.c
-000049b0: 6c6f 7365 2829 0a20 2020 2020 2020 2020  lose().         
-000049c0: 2020 2020 2020 2061 7761 6974 2073 7472         await str
-000049d0: 6561 6d2e 6163 6c6f 7365 2829 0a0a 2020  eam.aclose()..  
-000049e0: 2020 6173 796e 6320 6465 6620 7465 7374    async def test
-000049f0: 5f61 6363 6570 745f 6166 7465 725f 636c  _accept_after_cl
-00004a00: 6f73 6528 7365 6c66 2c20 6661 6d69 6c79  ose(self, family
-00004a10: 3a20 416e 7949 5041 6464 7265 7373 4661  : AnyIPAddressFa
-00004a20: 6d69 6c79 2920 2d3e 204e 6f6e 653a 0a20  mily) -> None:. 
-00004a30: 2020 2020 2020 2061 7379 6e63 2077 6974         async wit
-00004a40: 6820 6177 6169 7420 6372 6561 7465 5f74  h await create_t
-00004a50: 6370 5f6c 6973 7465 6e65 7228 0a20 2020  cp_listener(.   
-00004a60: 2020 2020 2020 2020 206c 6f63 616c 5f68           local_h
-00004a70: 6f73 743d 226c 6f63 616c 686f 7374 222c  ost="localhost",
-00004a80: 2066 616d 696c 793d 6661 6d69 6c79 0a20   family=family. 
-00004a90: 2020 2020 2020 2029 2061 7320 6d75 6c74         ) as mult
-00004aa0: 693a 0a20 2020 2020 2020 2020 2020 2066  i:.            f
-00004ab0: 6f72 206c 6973 7465 6e65 7220 696e 206d  or listener in m
-00004ac0: 756c 7469 2e6c 6973 7465 6e65 7273 3a0a  ulti.listeners:.
-00004ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ae0: 6177 6169 7420 6c69 7374 656e 6572 2e61  await listener.a
-00004af0: 636c 6f73 6528 290a 2020 2020 2020 2020  close().        
-00004b00: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
-00004b10: 7369 6e73 7461 6e63 6528 6c69 7374 656e  sinstance(listen
-00004b20: 6572 2c20 536f 636b 6574 4c69 7374 656e  er, SocketListen
-00004b30: 6572 290a 2020 2020 2020 2020 2020 2020  er).            
-00004b40: 2020 2020 7769 7468 2070 7974 6573 742e      with pytest.
-00004b50: 7261 6973 6573 2843 6c6f 7365 6452 6573  raises(ClosedRes
-00004b60: 6f75 7263 6545 7272 6f72 293a 0a20 2020  ourceError):.   
-00004b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b80: 2061 7761 6974 206c 6973 7465 6e65 722e   await listener.
-00004b90: 6163 6365 7074 2829 0a0a 2020 2020 6173  accept()..    as
-00004ba0: 796e 6320 6465 6620 7465 7374 5f73 6f63  ync def test_soc
-00004bb0: 6b65 745f 6f70 7469 6f6e 7328 7365 6c66  ket_options(self
-00004bc0: 2c20 6661 6d69 6c79 3a20 416e 7949 5041  , family: AnyIPA
-00004bd0: 6464 7265 7373 4661 6d69 6c79 2920 2d3e  ddressFamily) ->
-00004be0: 204e 6f6e 653a 0a20 2020 2020 2020 2061   None:.        a
-00004bf0: 7379 6e63 2077 6974 6820 6177 6169 7420  sync with await 
-00004c00: 6372 6561 7465 5f74 6370 5f6c 6973 7465  create_tcp_liste
-00004c10: 6e65 7228 0a20 2020 2020 2020 2020 2020  ner(.           
-00004c20: 206c 6f63 616c 5f68 6f73 743d 226c 6f63   local_host="loc
-00004c30: 616c 686f 7374 222c 2066 616d 696c 793d  alhost", family=
-00004c40: 6661 6d69 6c79 0a20 2020 2020 2020 2029  family.        )
-00004c50: 2061 7320 6d75 6c74 693a 0a20 2020 2020   as multi:.     
-00004c60: 2020 2020 2020 2066 6f72 206c 6973 7465         for liste
-00004c70: 6e65 7220 696e 206d 756c 7469 2e6c 6973  ner in multi.lis
-00004c80: 7465 6e65 7273 3a0a 2020 2020 2020 2020  teners:.        
-00004c90: 2020 2020 2020 2020 7261 775f 736f 636b          raw_sock
-00004ca0: 6574 203d 206c 6973 7465 6e65 722e 6578  et = listener.ex
-00004cb0: 7472 6128 536f 636b 6574 4174 7472 6962  tra(SocketAttrib
-00004cc0: 7574 652e 7261 775f 736f 636b 6574 290a  ute.raw_socket).
-00004cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ce0: 6966 2073 7973 2e70 6c61 7466 6f72 6d20  if sys.platform 
-00004cf0: 3d3d 2022 7769 6e33 3222 3a0a 2020 2020  == "win32":.    
-00004d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d10: 6173 7365 7274 2028 0a20 2020 2020 2020  assert (.       
-00004d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d30: 2072 6177 5f73 6f63 6b65 742e 6765 7473   raw_socket.gets
-00004d40: 6f63 6b6f 7074 280a 2020 2020 2020 2020  ockopt(.        
-00004d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d60: 2020 2020 736f 636b 6574 2e53 4f4c 5f53      socket.SOL_S
-00004d70: 4f43 4b45 542c 2073 6f63 6b65 742e 534f  OCKET, socket.SO
-00004d80: 5f45 5843 4c55 5349 5645 4144 4452 5553  _EXCLUSIVEADDRUS
-00004d90: 450a 2020 2020 2020 2020 2020 2020 2020  E.              
-00004da0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00004db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004dc0: 2020 2020 213d 2030 0a20 2020 2020 2020      != 0.       
-00004dd0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00004de0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00004df0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00004e00: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-00004e10: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00004e20: 2020 2020 2020 2020 2020 7261 775f 736f            raw_so
-00004e30: 636b 6574 2e67 6574 736f 636b 6f70 7428  cket.getsockopt(
-00004e40: 736f 636b 6574 2e53 4f4c 5f53 4f43 4b45  socket.SOL_SOCKE
-00004e50: 542c 2073 6f63 6b65 742e 534f 5f52 4555  T, socket.SO_REU
-00004e60: 5345 4144 4452 290a 2020 2020 2020 2020  SEADDR).        
-00004e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e80: 213d 2030 0a20 2020 2020 2020 2020 2020  != 0.           
-00004e90: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00004ea0: 2020 2020 2020 2020 2020 2020 7261 775f              raw_
-00004eb0: 736f 636b 6574 2e73 6574 736f 636b 6f70  socket.setsockop
-00004ec0: 7428 736f 636b 6574 2e53 4f4c 5f53 4f43  t(socket.SOL_SOC
-00004ed0: 4b45 542c 2073 6f63 6b65 742e 534f 5f52  KET, socket.SO_R
-00004ee0: 4356 4255 462c 2038 3030 3030 290a 2020  CVBUF, 80000).  
-00004ef0: 2020 2020 2020 2020 2020 2020 2020 6173                as
-00004f00: 7365 7274 2072 6177 5f73 6f63 6b65 742e  sert raw_socket.
-00004f10: 6765 7473 6f63 6b6f 7074 2873 6f63 6b65  getsockopt(socke
-00004f20: 742e 534f 4c5f 534f 434b 4554 2c20 736f  t.SOL_SOCKET, so
-00004f30: 636b 6574 2e53 4f5f 5243 5642 5546 2920  cket.SO_RCVBUF) 
-00004f40: 696e 2028 0a20 2020 2020 2020 2020 2020  in (.           
-00004f50: 2020 2020 2020 2020 2038 3030 3030 2c0a           80000,.
-00004f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f70: 2020 2020 3136 3030 3030 2c0a 2020 2020      160000,.    
-00004f80: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00004f90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00004fa0: 6c69 656e 7420 3d20 736f 636b 6574 2e73  lient = socket.s
-00004fb0: 6f63 6b65 7428 7261 775f 736f 636b 6574  ocket(raw_socket
-00004fc0: 2e66 616d 696c 7929 0a20 2020 2020 2020  .family).       
-00004fd0: 2020 2020 2020 2020 2063 6c69 656e 742e           client.
-00004fe0: 7365 7474 696d 656f 7574 2831 290a 2020  settimeout(1).  
-00004ff0: 2020 2020 2020 2020 2020 2020 2020 636c                cl
-00005000: 6965 6e74 2e63 6f6e 6e65 6374 2872 6177  ient.connect(raw
-00005010: 5f73 6f63 6b65 742e 6765 7473 6f63 6b6e  _socket.getsockn
-00005020: 616d 6528 2929 0a0a 2020 2020 2020 2020  ame())..        
-00005030: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
-00005040: 7369 6e73 7461 6e63 6528 6c69 7374 656e  sinstance(listen
-00005050: 6572 2c20 536f 636b 6574 4c69 7374 656e  er, SocketListen
-00005060: 6572 290a 2020 2020 2020 2020 2020 2020  er).            
-00005070: 2020 2020 6173 796e 6320 7769 7468 2061      async with a
-00005080: 7761 6974 206c 6973 7465 6e65 722e 6163  wait listener.ac
-00005090: 6365 7074 2829 2061 7320 7374 7265 616d  cept() as stream
-000050a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000050b0: 2020 2020 2020 7261 775f 736f 636b 6574        raw_socket
-000050c0: 203d 2073 7472 6561 6d2e 6578 7472 6128   = stream.extra(
-000050d0: 536f 636b 6574 4174 7472 6962 7574 652e  SocketAttribute.
-000050e0: 7261 775f 736f 636b 6574 290a 2020 2020  raw_socket).    
-000050f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005100: 6173 7365 7274 2072 6177 5f73 6f63 6b65  assert raw_socke
-00005110: 742e 6765 7474 696d 656f 7574 2829 203d  t.gettimeout() =
-00005120: 3d20 300a 2020 2020 2020 2020 2020 2020  = 0.            
-00005130: 2020 2020 2020 2020 6173 7365 7274 2072          assert r
-00005140: 6177 5f73 6f63 6b65 742e 6661 6d69 6c79  aw_socket.family
-00005150: 203d 3d20 6c69 7374 656e 6572 2e65 7874   == listener.ext
-00005160: 7261 2853 6f63 6b65 7441 7474 7269 6275  ra(SocketAttribu
-00005170: 7465 2e66 616d 696c 7929 0a20 2020 2020  te.family).     
-00005180: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00005190: 7373 6572 7420 280a 2020 2020 2020 2020  ssert (.        
-000051a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051b0: 7261 775f 736f 636b 6574 2e67 6574 736f  raw_socket.getso
-000051c0: 636b 6f70 7428 736f 636b 6574 2e49 5050  ckopt(socket.IPP
-000051d0: 524f 544f 5f54 4350 2c20 736f 636b 6574  ROTO_TCP, socket
-000051e0: 2e54 4350 5f4e 4f44 454c 4159 290a 2020  .TCP_NODELAY).  
-000051f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005200: 2020 2020 2020 213d 2030 0a20 2020 2020        != 0.     
-00005210: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00005220: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005230: 2020 636c 6965 6e74 2e63 6c6f 7365 2829    client.close()
-00005240: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
-00005250: 726b 2e73 6b69 7069 6628 0a20 2020 2020  rk.skipif(.     
-00005260: 2020 206e 6f74 2068 6173 6174 7472 2873     not hasattr(s
-00005270: 6f63 6b65 742c 2022 534f 5f52 4555 5345  ocket, "SO_REUSE
-00005280: 504f 5254 2229 2c20 7265 6173 6f6e 3d22  PORT"), reason="
-00005290: 534f 5f52 4555 5345 504f 5254 206f 7074  SO_REUSEPORT opt
-000052a0: 696f 6e20 6e6f 7420 7375 7070 6f72 7465  ion not supporte
-000052b0: 6422 0a20 2020 2029 0a20 2020 2061 7379  d".    ).    asy
-000052c0: 6e63 2064 6566 2074 6573 745f 7265 7573  nc def test_reus
-000052d0: 655f 706f 7274 2873 656c 662c 2066 616d  e_port(self, fam
-000052e0: 696c 793a 2041 6e79 4950 4164 6472 6573  ily: AnyIPAddres
-000052f0: 7346 616d 696c 7929 202d 3e20 4e6f 6e65  sFamily) -> None
-00005300: 3a0a 2020 2020 2020 2020 6d75 6c74 6931  :.        multi1
-00005310: 203d 2061 7761 6974 2063 7265 6174 655f   = await create_
-00005320: 7463 705f 6c69 7374 656e 6572 280a 2020  tcp_listener(.  
-00005330: 2020 2020 2020 2020 2020 6c6f 6361 6c5f            local_
-00005340: 686f 7374 3d22 6c6f 6361 6c68 6f73 7422  host="localhost"
-00005350: 2c20 6661 6d69 6c79 3d66 616d 696c 792c  , family=family,
-00005360: 2072 6575 7365 5f70 6f72 743d 5472 7565   reuse_port=True
-00005370: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00005380: 2020 2061 7373 6572 7420 6c65 6e28 6d75     assert len(mu
-00005390: 6c74 6931 2e6c 6973 7465 6e65 7273 2920  lti1.listeners) 
-000053a0: 3d3d 2031 0a0a 2020 2020 2020 2020 6d75  == 1..        mu
-000053b0: 6c74 6932 203d 2061 7761 6974 2063 7265  lti2 = await cre
-000053c0: 6174 655f 7463 705f 6c69 7374 656e 6572  ate_tcp_listener
-000053d0: 280a 2020 2020 2020 2020 2020 2020 6c6f  (.            lo
-000053e0: 6361 6c5f 686f 7374 3d22 6c6f 6361 6c68  cal_host="localh
-000053f0: 6f73 7422 2c0a 2020 2020 2020 2020 2020  ost",.          
-00005400: 2020 6c6f 6361 6c5f 706f 7274 3d6d 756c    local_port=mul
-00005410: 7469 312e 6c69 7374 656e 6572 735b 305d  ti1.listeners[0]
-00005420: 2e65 7874 7261 2853 6f63 6b65 7441 7474  .extra(SocketAtt
-00005430: 7269 6275 7465 2e6c 6f63 616c 5f70 6f72  ribute.local_por
-00005440: 7429 2c0a 2020 2020 2020 2020 2020 2020  t),.            
-00005450: 6661 6d69 6c79 3d66 616d 696c 792c 0a20  family=family,. 
-00005460: 2020 2020 2020 2020 2020 2072 6575 7365             reuse
-00005470: 5f70 6f72 743d 5472 7565 2c0a 2020 2020  _port=True,.    
-00005480: 2020 2020 290a 2020 2020 2020 2020 6173      ).        as
-00005490: 7365 7274 206c 656e 286d 756c 7469 322e  sert len(multi2.
-000054a0: 6c69 7374 656e 6572 7329 203d 3d20 310a  listeners) == 1.
-000054b0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-000054c0: 6d75 6c74 6931 2e6c 6973 7465 6e65 7273  multi1.listeners
-000054d0: 5b30 5d2e 6578 7472 6128 0a20 2020 2020  [0].extra(.     
-000054e0: 2020 2020 2020 2053 6f63 6b65 7441 7474         SocketAtt
-000054f0: 7269 6275 7465 2e6c 6f63 616c 5f61 6464  ribute.local_add
-00005500: 7265 7373 0a20 2020 2020 2020 2029 203d  ress.        ) =
-00005510: 3d20 6d75 6c74 6932 2e6c 6973 7465 6e65  = multi2.listene
-00005520: 7273 5b30 5d2e 6578 7472 6128 536f 636b  rs[0].extra(Sock
-00005530: 6574 4174 7472 6962 7574 652e 6c6f 6361  etAttribute.loca
-00005540: 6c5f 6164 6472 6573 7329 0a20 2020 2020  l_address).     
-00005550: 2020 2061 7761 6974 206d 756c 7469 312e     await multi1.
-00005560: 6163 6c6f 7365 2829 0a20 2020 2020 2020  aclose().       
-00005570: 2061 7761 6974 206d 756c 7469 322e 6163   await multi2.ac
-00005580: 6c6f 7365 2829 0a0a 2020 2020 6173 796e  lose()..    asyn
-00005590: 6320 6465 6620 7465 7374 5f63 6c6f 7365  c def test_close
-000055a0: 5f66 726f 6d5f 6f74 6865 725f 7461 736b  _from_other_task
-000055b0: 2873 656c 662c 2066 616d 696c 793a 2041  (self, family: A
-000055c0: 6e79 4950 4164 6472 6573 7346 616d 696c  nyIPAddressFamil
-000055d0: 7929 202d 3e20 4e6f 6e65 3a0a 2020 2020  y) -> None:.    
-000055e0: 2020 2020 6c69 7374 656e 6572 203d 2061      listener = a
-000055f0: 7761 6974 2063 7265 6174 655f 7463 705f  wait create_tcp_
-00005600: 6c69 7374 656e 6572 286c 6f63 616c 5f68  listener(local_h
-00005610: 6f73 743d 226c 6f63 616c 686f 7374 222c  ost="localhost",
-00005620: 2066 616d 696c 793d 6661 6d69 6c79 290a   family=family).
-00005630: 2020 2020 2020 2020 7769 7468 2070 7974          with pyt
-00005640: 6573 742e 7261 6973 6573 2845 7863 6570  est.raises(Excep
-00005650: 7469 6f6e 4772 6f75 7029 2061 7320 6578  tionGroup) as ex
-00005660: 633a 0a20 2020 2020 2020 2020 2020 2061  c:.            a
-00005670: 7379 6e63 2077 6974 6820 6372 6561 7465  sync with create
-00005680: 5f74 6173 6b5f 6772 6f75 7028 2920 6173  _task_group() as
-00005690: 2074 673a 0a20 2020 2020 2020 2020 2020   tg:.           
-000056a0: 2020 2020 2074 672e 7374 6172 745f 736f       tg.start_so
-000056b0: 6f6e 286c 6973 7465 6e65 722e 7365 7276  on(listener.serv
-000056c0: 652c 206c 616d 6264 6120 7374 7265 616d  e, lambda stream
-000056d0: 3a20 4e6f 6e65 290a 2020 2020 2020 2020  : None).        
-000056e0: 2020 2020 2020 2020 6177 6169 7420 7761          await wa
-000056f0: 6974 5f61 6c6c 5f74 6173 6b73 5f62 6c6f  it_all_tasks_blo
-00005700: 636b 6564 2829 0a20 2020 2020 2020 2020  cked().         
-00005710: 2020 2020 2020 2061 7761 6974 206c 6973         await lis
-00005720: 7465 6e65 722e 6163 6c6f 7365 2829 0a20  tener.aclose(). 
-00005730: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00005740: 672e 6361 6e63 656c 5f73 636f 7065 2e63  g.cancel_scope.c
-00005750: 616e 6365 6c28 290a 0a20 2020 2020 2020  ancel()..       
-00005760: 2061 7373 6572 7420 6c65 6e28 6578 632e   assert len(exc.
-00005770: 7661 6c75 652e 6578 6365 7074 696f 6e73  value.exceptions
-00005780: 2920 3d3d 2031 0a20 2020 2020 2020 2061  ) == 1.        a
-00005790: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
-000057a0: 2865 7863 2e76 616c 7565 2e65 7863 6570  (exc.value.excep
-000057b0: 7469 6f6e 735b 305d 2c20 4578 6365 7074  tions[0], Except
-000057c0: 696f 6e47 726f 7570 290a 2020 2020 2020  ionGroup).      
-000057d0: 2020 6e65 7374 6564 5f67 7270 203d 2065    nested_grp = e
-000057e0: 7863 2e76 616c 7565 2e65 7863 6570 7469  xc.value.excepti
-000057f0: 6f6e 735b 305d 0a20 2020 2020 2020 2061  ons[0].        a
-00005800: 7373 6572 7420 6c65 6e28 6e65 7374 6564  ssert len(nested
-00005810: 5f67 7270 2e65 7863 6570 7469 6f6e 7329  _grp.exceptions)
-00005820: 203d 3d20 310a 2020 2020 2020 2020 6173   == 1.        as
-00005830: 7365 7274 2069 7369 6e73 7461 6e63 6528  sert isinstance(
-00005840: 6e65 7374 6564 5f67 7270 2e65 7863 6570  nested_grp.excep
-00005850: 7469 6f6e 735b 305d 2c20 4578 6365 7074  tions[0], Except
-00005860: 696f 6e47 726f 7570 290a 0a20 2020 2061  ionGroup)..    a
-00005870: 7379 6e63 2064 6566 2074 6573 745f 7365  sync def test_se
-00005880: 6e64 5f61 6674 6572 5f65 6f66 2873 656c  nd_after_eof(sel
-00005890: 662c 2066 616d 696c 793a 2041 6e79 4950  f, family: AnyIP
-000058a0: 4164 6472 6573 7346 616d 696c 7929 202d  AddressFamily) -
-000058b0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-000058c0: 6173 796e 6320 6465 6620 6861 6e64 6c65  async def handle
-000058d0: 2873 7472 6561 6d3a 2053 6f63 6b65 7453  (stream: SocketS
-000058e0: 7472 6561 6d29 202d 3e20 4e6f 6e65 3a0a  tream) -> None:.
-000058f0: 2020 2020 2020 2020 2020 2020 6173 796e              asyn
-00005900: 6320 7769 7468 2073 7472 6561 6d3a 0a20  c with stream:. 
-00005910: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00005920: 7761 6974 2073 7472 6561 6d2e 7365 6e64  wait stream.send
-00005930: 2862 2248 656c 6c6f 5c6e 2229 0a0a 2020  (b"Hello\n")..  
-00005940: 2020 2020 2020 6d75 6c74 6920 3d20 6177        multi = aw
-00005950: 6169 7420 6372 6561 7465 5f74 6370 5f6c  ait create_tcp_l
-00005960: 6973 7465 6e65 7228 6661 6d69 6c79 3d66  istener(family=f
-00005970: 616d 696c 792c 206c 6f63 616c 5f68 6f73  amily, local_hos
-00005980: 743d 226c 6f63 616c 686f 7374 2229 0a20  t="localhost"). 
-00005990: 2020 2020 2020 2061 7379 6e63 2077 6974         async wit
-000059a0: 6820 6d75 6c74 692c 2063 7265 6174 655f  h multi, create_
-000059b0: 7461 736b 5f67 726f 7570 2829 2061 7320  task_group() as 
-000059c0: 7467 3a0a 2020 2020 2020 2020 2020 2020  tg:.            
-000059d0: 7467 2e73 7461 7274 5f73 6f6f 6e28 6d75  tg.start_soon(mu
-000059e0: 6c74 692e 7365 7276 652c 2068 616e 646c  lti.serve, handl
-000059f0: 6529 0a20 2020 2020 2020 2020 2020 2061  e).            a
-00005a00: 7761 6974 2077 6169 745f 616c 6c5f 7461  wait wait_all_ta
-00005a10: 736b 735f 626c 6f63 6b65 6428 290a 0a20  sks_blocked().. 
-00005a20: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00005a30: 736f 636b 6574 2e73 6f63 6b65 7428 6661  socket.socket(fa
-00005a40: 6d69 6c79 2920 6173 2063 6c69 656e 743a  mily) as client:
-00005a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005a60: 2063 6c69 656e 742e 636f 6e6e 6563 7428   client.connect(
-00005a70: 6d75 6c74 692e 6578 7472 6128 536f 636b  multi.extra(Sock
-00005a80: 6574 4174 7472 6962 7574 652e 6c6f 6361  etAttribute.loca
-00005a90: 6c5f 6164 6472 6573 7329 290a 2020 2020  l_address)).    
-00005aa0: 2020 2020 2020 2020 2020 2020 636c 6965              clie
-00005ab0: 6e74 2e73 6875 7464 6f77 6e28 736f 636b  nt.shutdown(sock
-00005ac0: 6574 2e53 4855 545f 5752 290a 2020 2020  et.SHUT_WR).    
-00005ad0: 2020 2020 2020 2020 2020 2020 636c 6965              clie
-00005ae0: 6e74 2e73 6574 626c 6f63 6b69 6e67 2846  nt.setblocking(F
-00005af0: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
-00005b00: 2020 2020 2020 7769 7468 2066 6169 6c5f        with fail_
-00005b10: 6166 7465 7228 3129 3a0a 2020 2020 2020  after(1):.      
-00005b20: 2020 2020 2020 2020 2020 2020 2020 7768                wh
-00005b30: 696c 6520 5472 7565 3a0a 2020 2020 2020  ile True:.      
-00005b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b50: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00005b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b70: 2020 206d 6573 7361 6765 203d 2063 6c69     message = cli
-00005b80: 656e 742e 7265 6376 2831 3029 0a20 2020  ent.recv(10).   
-00005b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ba0: 2020 2020 2065 7863 6570 7420 426c 6f63       except Bloc
-00005bb0: 6b69 6e67 494f 4572 726f 723a 0a20 2020  kingIOError:.   
-00005bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bd0: 2020 2020 2020 2020 2061 7761 6974 2073           await s
-00005be0: 6c65 6570 2830 290a 2020 2020 2020 2020  leep(0).        
-00005bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c00: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00005c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c20: 2020 6173 7365 7274 206d 6573 7361 6765    assert message
-00005c30: 203d 3d20 6222 4865 6c6c 6f5c 6e22 0a20   == b"Hello\n". 
-00005c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c50: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00005c60: 0a0a 2020 2020 2020 2020 2020 2020 7467  ..            tg
-00005c70: 2e63 616e 6365 6c5f 7363 6f70 652e 6361  .cancel_scope.ca
-00005c80: 6e63 656c 2829 0a0a 2020 2020 4073 6b69  ncel()..    @ski
-00005c90: 705f 6970 7636 5f6d 6172 6b0a 2020 2020  p_ipv6_mark.    
-00005ca0: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
-00005cb0: 7069 6628 0a20 2020 2020 2020 2073 7973  pif(.        sys
-00005cc0: 2e70 6c61 7466 6f72 6d20 3d3d 2022 7769  .platform == "wi
-00005cd0: 6e33 3222 2c0a 2020 2020 2020 2020 7265  n32",.        re
-00005ce0: 6173 6f6e 3d22 5769 6e64 6f77 7320 646f  ason="Windows do
-00005cf0: 6573 206e 6f74 2073 7570 706f 7274 2069  es not support i
-00005d00: 6e74 6572 6661 6365 206e 616d 6520 7375  nterface name su
-00005d10: 6666 6978 6573 222c 0a20 2020 2029 0a20  ffixes",.    ). 
-00005d20: 2020 2061 7379 6e63 2064 6566 2074 6573     async def tes
-00005d30: 745f 6269 6e64 5f6c 696e 6b5f 6c6f 6361  t_bind_link_loca
-00005d40: 6c28 7365 6c66 2920 2d3e 204e 6f6e 653a  l(self) -> None:
-00005d50: 0a20 2020 2020 2020 2023 2052 6567 7265  .        # Regre
-00005d60: 7373 696f 6e20 7465 7374 2066 6f72 2023  ssion test for #
-00005d70: 3535 340a 2020 2020 2020 2020 6c69 6e6b  554.        link
-00005d80: 5f6c 6f63 616c 5f69 7076 365f 6164 6472  _local_ipv6_addr
-00005d90: 6573 7320 3d20 6e65 7874 280a 2020 2020  ess = next(.    
-00005da0: 2020 2020 2020 2020 280a 2020 2020 2020          (.      
-00005db0: 2020 2020 2020 2020 2020 6164 6472 2e61            addr.a
-00005dc0: 6464 7265 7373 0a20 2020 2020 2020 2020  ddress.         
-00005dd0: 2020 2020 2020 2066 6f72 2061 6464 7265         for addre
-00005de0: 7373 6573 2069 6e20 7073 7574 696c 2e6e  sses in psutil.n
-00005df0: 6574 5f69 665f 6164 6472 7328 292e 7661  et_if_addrs().va
-00005e00: 6c75 6573 2829 0a20 2020 2020 2020 2020  lues().         
-00005e10: 2020 2020 2020 2066 6f72 2061 6464 7220         for addr 
-00005e20: 696e 2061 6464 7265 7373 6573 0a20 2020  in addresses.   
-00005e30: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00005e40: 6164 6472 2e61 6464 7265 7373 2e73 7461  addr.address.sta
-00005e50: 7274 7377 6974 6828 2266 6538 303a 3a22  rtswith("fe80::"
-00005e60: 2920 616e 6420 2225 2220 696e 2061 6464  ) and "%" in add
-00005e70: 722e 6164 6472 6573 730a 2020 2020 2020  r.address.      
-00005e80: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
-00005e90: 2020 2020 204e 6f6e 652c 0a20 2020 2020       None,.     
-00005ea0: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
-00005eb0: 6c69 6e6b 5f6c 6f63 616c 5f69 7076 365f  link_local_ipv6_
-00005ec0: 6164 6472 6573 7320 6973 204e 6f6e 653a  address is None:
-00005ed0: 0a20 2020 2020 2020 2020 2020 2070 7974  .            pyt
-00005ee0: 6573 742e 6661 696c 2822 436f 756c 6420  est.fail("Could 
-00005ef0: 6e6f 7420 6669 6e64 2061 206c 696e 6b2d  not find a link-
-00005f00: 6c6f 6361 6c20 4950 7636 2069 6e74 6572  local IPv6 inter
-00005f10: 6661 6365 2229 0a0a 2020 2020 2020 2020  face")..        
-00005f20: 6173 796e 6320 7769 7468 2061 7761 6974  async with await
-00005f30: 2063 7265 6174 655f 7463 705f 6c69 7374   create_tcp_list
-00005f40: 656e 6572 286c 6f63 616c 5f68 6f73 743d  ener(local_host=
-00005f50: 6c69 6e6b 5f6c 6f63 616c 5f69 7076 365f  link_local_ipv6_
-00005f60: 6164 6472 6573 7329 3a0a 2020 2020 2020  address):.      
-00005f70: 2020 2020 2020 7061 7373 0a0a 0a40 7079        pass...@py
-00005f80: 7465 7374 2e6d 6172 6b2e 736b 6970 6966  test.mark.skipif
-00005f90: 280a 2020 2020 7379 732e 706c 6174 666f  (.    sys.platfo
-00005fa0: 726d 203d 3d20 2277 696e 3332 222c 2072  rm == "win32", r
-00005fb0: 6561 736f 6e3d 2255 4e49 5820 736f 636b  eason="UNIX sock
-00005fc0: 6574 7320 6172 6520 6e6f 7420 6176 6169  ets are not avai
-00005fd0: 6c61 626c 6520 6f6e 2057 696e 646f 7773  lable on Windows
-00005fe0: 220a 290a 636c 6173 7320 5465 7374 554e  ".).class TestUN
-00005ff0: 4958 5374 7265 616d 3a0a 2020 2020 4070  IXStream:.    @p
-00006000: 7974 6573 742e 6669 7874 7572 650a 2020  ytest.fixture.  
-00006010: 2020 6465 6620 736f 636b 6574 5f70 6174    def socket_pat
-00006020: 6828 7365 6c66 2920 2d3e 2047 656e 6572  h(self) -> Gener
-00006030: 6174 6f72 5b50 6174 682c 204e 6f6e 652c  ator[Path, None,
-00006040: 204e 6f6e 655d 3a0a 2020 2020 2020 2020   None]:.        
-00006050: 2320 5573 6520 7374 646c 6962 2074 656d  # Use stdlib tem
-00006060: 7064 6972 2067 656e 6572 6174 696f 6e0a  pdir generation.
-00006070: 2020 2020 2020 2020 2320 4669 7865 7320          # Fixes 
-00006080: 604f 5345 7272 6f72 3a20 4146 5f55 4e49  `OSError: AF_UNI
-00006090: 5820 7061 7468 2074 6f6f 206c 6f6e 6760  X path too long`
-000060a0: 2066 726f 6d20 7079 7465 7374 2067 656e   from pytest gen
-000060b0: 6572 6174 6564 2074 656d 705f 7061 7468  erated temp_path
-000060c0: 0a20 2020 2020 2020 2077 6974 6820 7465  .        with te
-000060d0: 6d70 6669 6c65 2e54 656d 706f 7261 7279  mpfile.Temporary
-000060e0: 4469 7265 6374 6f72 7928 2920 6173 2070  Directory() as p
-000060f0: 6174 683a 0a20 2020 2020 2020 2020 2020  ath:.           
-00006100: 2079 6965 6c64 2050 6174 6828 7061 7468   yield Path(path
-00006110: 2920 2f20 2273 6f63 6b65 7422 0a0a 2020  ) / "socket"..  
-00006120: 2020 4070 7974 6573 742e 6669 7874 7572    @pytest.fixtur
-00006130: 6528 7061 7261 6d73 3d5b 4661 6c73 652c  e(params=[False,
-00006140: 2054 7275 655d 2c20 6964 733d 5b22 7374   True], ids=["st
-00006150: 7222 2c20 2270 6174 6822 5d29 0a20 2020  r", "path"]).   
-00006160: 2064 6566 2073 6f63 6b65 745f 7061 7468   def socket_path
-00006170: 5f6f 725f 7374 7228 7365 6c66 2c20 7265  _or_str(self, re
-00006180: 7175 6573 743a 2053 7562 5265 7175 6573  quest: SubReques
-00006190: 742c 2073 6f63 6b65 745f 7061 7468 3a20  t, socket_path: 
-000061a0: 5061 7468 2920 2d3e 2050 6174 6820 7c20  Path) -> Path | 
-000061b0: 7374 723a 0a20 2020 2020 2020 2072 6574  str:.        ret
-000061c0: 7572 6e20 736f 636b 6574 5f70 6174 6820  urn socket_path 
-000061d0: 6966 2072 6571 7565 7374 2e70 6172 616d  if request.param
-000061e0: 2065 6c73 6520 7374 7228 736f 636b 6574   else str(socket
-000061f0: 5f70 6174 6829 0a0a 2020 2020 4070 7974  _path)..    @pyt
-00006200: 6573 742e 6669 7874 7572 650a 2020 2020  est.fixture.    
-00006210: 6465 6620 7365 7276 6572 5f73 6f63 6b28  def server_sock(
-00006220: 7365 6c66 2c20 736f 636b 6574 5f70 6174  self, socket_pat
-00006230: 683a 2050 6174 6829 202d 3e20 4974 6572  h: Path) -> Iter
-00006240: 6162 6c65 5b73 6f63 6b65 742e 736f 636b  able[socket.sock
-00006250: 6574 5d3a 0a20 2020 2020 2020 2073 6f63  et]:.        soc
-00006260: 6b20 3d20 736f 636b 6574 2e73 6f63 6b65  k = socket.socke
-00006270: 7428 736f 636b 6574 2e41 465f 554e 4958  t(socket.AF_UNIX
-00006280: 2c20 736f 636b 6574 2e53 4f43 4b5f 5354  , socket.SOCK_ST
-00006290: 5245 414d 290a 2020 2020 2020 2020 736f  REAM).        so
-000062a0: 636b 2e73 6574 7469 6d65 6f75 7428 3129  ck.settimeout(1)
-000062b0: 0a20 2020 2020 2020 2073 6f63 6b2e 6269  .        sock.bi
-000062c0: 6e64 2873 7472 2873 6f63 6b65 745f 7061  nd(str(socket_pa
-000062d0: 7468 2929 0a20 2020 2020 2020 2073 6f63  th)).        soc
-000062e0: 6b2e 6c69 7374 656e 2829 0a20 2020 2020  k.listen().     
-000062f0: 2020 2079 6965 6c64 2073 6f63 6b0a 2020     yield sock.  
-00006300: 2020 2020 2020 736f 636b 2e63 6c6f 7365        sock.close
-00006310: 2829 0a0a 2020 2020 6173 796e 6320 6465  ()..    async de
-00006320: 6620 7465 7374 5f65 7874 7261 5f61 7474  f test_extra_att
-00006330: 7269 6275 7465 7328 0a20 2020 2020 2020  ributes(.       
-00006340: 2073 656c 662c 2073 6572 7665 725f 736f   self, server_so
-00006350: 636b 3a20 736f 636b 6574 2e73 6f63 6b65  ck: socket.socke
-00006360: 742c 2073 6f63 6b65 745f 7061 7468 3a20  t, socket_path: 
-00006370: 5061 7468 0a20 2020 2029 202d 3e20 4e6f  Path.    ) -> No
-00006380: 6e65 3a0a 2020 2020 2020 2020 6173 796e  ne:.        asyn
-00006390: 6320 7769 7468 2061 7761 6974 2063 6f6e  c with await con
-000063a0: 6e65 6374 5f75 6e69 7828 736f 636b 6574  nect_unix(socket
-000063b0: 5f70 6174 6829 2061 7320 7374 7265 616d  _path) as stream
-000063c0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-000063d0: 775f 736f 636b 6574 203d 2073 7472 6561  w_socket = strea
-000063e0: 6d2e 6578 7472 6128 536f 636b 6574 4174  m.extra(SocketAt
-000063f0: 7472 6962 7574 652e 7261 775f 736f 636b  tribute.raw_sock
-00006400: 6574 290a 2020 2020 2020 2020 2020 2020  et).            
-00006410: 6173 7365 7274 2073 7472 6561 6d2e 6578  assert stream.ex
-00006420: 7472 6128 536f 636b 6574 4174 7472 6962  tra(SocketAttrib
-00006430: 7574 652e 6661 6d69 6c79 2920 3d3d 2073  ute.family) == s
-00006440: 6f63 6b65 742e 4146 5f55 4e49 580a 2020  ocket.AF_UNIX.  
-00006450: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-00006460: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-00006470: 2020 2073 7472 6561 6d2e 6578 7472 6128     stream.extra(
-00006480: 536f 636b 6574 4174 7472 6962 7574 652e  SocketAttribute.
-00006490: 6c6f 6361 6c5f 6164 6472 6573 7329 203d  local_address) =
-000064a0: 3d20 7261 775f 736f 636b 6574 2e67 6574  = raw_socket.get
-000064b0: 736f 636b 6e61 6d65 2829 0a20 2020 2020  sockname().     
-000064c0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000064d0: 2020 2020 2061 7373 6572 7420 7374 7265       assert stre
-000064e0: 616d 2e65 7874 7261 2853 6f63 6b65 7441  am.extra(SocketA
-000064f0: 7474 7269 6275 7465 2e72 656d 6f74 655f  ttribute.remote_
-00006500: 6164 6472 6573 7329 203d 3d20 7374 7228  address) == str(
-00006510: 736f 636b 6574 5f70 6174 6829 0a20 2020  socket_path).   
-00006520: 2020 2020 2020 2020 2070 7974 6573 742e           pytest.
-00006530: 7261 6973 6573 280a 2020 2020 2020 2020  raises(.        
-00006540: 2020 2020 2020 2020 5479 7065 6441 7474          TypedAtt
-00006550: 7269 6275 7465 4c6f 6f6b 7570 4572 726f  ributeLookupErro
-00006560: 722c 2073 7472 6561 6d2e 6578 7472 612c  r, stream.extra,
-00006570: 2053 6f63 6b65 7441 7474 7269 6275 7465   SocketAttribute
-00006580: 2e6c 6f63 616c 5f70 6f72 740a 2020 2020  .local_port.    
-00006590: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000065a0: 2020 2020 2020 7079 7465 7374 2e72 6169        pytest.rai
-000065b0: 7365 7328 0a20 2020 2020 2020 2020 2020  ses(.           
-000065c0: 2020 2020 2054 7970 6564 4174 7472 6962       TypedAttrib
-000065d0: 7574 654c 6f6f 6b75 7045 7272 6f72 2c20  uteLookupError, 
-000065e0: 7374 7265 616d 2e65 7874 7261 2c20 536f  stream.extra, So
-000065f0: 636b 6574 4174 7472 6962 7574 652e 7265  cketAttribute.re
-00006600: 6d6f 7465 5f70 6f72 740a 2020 2020 2020  mote_port.      
-00006610: 2020 2020 2020 290a 0a20 2020 2061 7379        )..    asy
-00006620: 6e63 2064 6566 2074 6573 745f 7365 6e64  nc def test_send
-00006630: 5f72 6563 6569 7665 280a 2020 2020 2020  _receive(.      
-00006640: 2020 7365 6c66 2c20 7365 7276 6572 5f73    self, server_s
-00006650: 6f63 6b3a 2073 6f63 6b65 742e 736f 636b  ock: socket.sock
-00006660: 6574 2c20 736f 636b 6574 5f70 6174 685f  et, socket_path_
-00006670: 6f72 5f73 7472 3a20 5061 7468 207c 2073  or_str: Path | s
-00006680: 7472 0a20 2020 2029 202d 3e20 4e6f 6e65  tr.    ) -> None
-00006690: 3a0a 2020 2020 2020 2020 6173 796e 6320  :.        async 
-000066a0: 7769 7468 2061 7761 6974 2063 6f6e 6e65  with await conne
-000066b0: 6374 5f75 6e69 7828 736f 636b 6574 5f70  ct_unix(socket_p
-000066c0: 6174 685f 6f72 5f73 7472 2920 6173 2073  ath_or_str) as s
-000066d0: 7472 6561 6d3a 0a20 2020 2020 2020 2020  tream:.         
-000066e0: 2020 2063 6c69 656e 742c 205f 203d 2073     client, _ = s
-000066f0: 6572 7665 725f 736f 636b 2e61 6363 6570  erver_sock.accep
-00006700: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-00006710: 6177 6169 7420 7374 7265 616d 2e73 656e  await stream.sen
-00006720: 6428 6222 626c 6168 2229 0a20 2020 2020  d(b"blah").     
-00006730: 2020 2020 2020 2072 6571 7565 7374 203d         request =
-00006740: 2063 6c69 656e 742e 7265 6376 2831 3030   client.recv(100
-00006750: 290a 2020 2020 2020 2020 2020 2020 636c  ).            cl
-00006760: 6965 6e74 2e73 656e 6461 6c6c 2872 6571  ient.sendall(req
-00006770: 7565 7374 5b3a 3a2d 315d 290a 2020 2020  uest[::-1]).    
-00006780: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-00006790: 203d 2061 7761 6974 2073 7472 6561 6d2e   = await stream.
-000067a0: 7265 6365 6976 6528 290a 2020 2020 2020  receive().      
-000067b0: 2020 2020 2020 636c 6965 6e74 2e63 6c6f        client.clo
-000067c0: 7365 2829 0a0a 2020 2020 2020 2020 6173  se()..        as
-000067d0: 7365 7274 2072 6573 706f 6e73 6520 3d3d  sert response ==
-000067e0: 2062 2268 616c 6222 0a0a 2020 2020 6173   b"halb"..    as
-000067f0: 796e 6320 6465 6620 7465 7374 5f72 6563  ync def test_rec
-00006800: 6569 7665 5f6c 6172 6765 5f62 7566 6665  eive_large_buffe
-00006810: 7228 0a20 2020 2020 2020 2073 656c 662c  r(.        self,
-00006820: 2073 6572 7665 725f 736f 636b 3a20 736f   server_sock: so
-00006830: 636b 6574 2e73 6f63 6b65 742c 2073 6f63  cket.socket, soc
-00006840: 6b65 745f 7061 7468 3a20 5061 7468 0a20  ket_path: Path. 
-00006850: 2020 2029 202d 3e20 4e6f 6e65 3a0a 2020     ) -> None:.  
-00006860: 2020 2020 2020 6465 6620 7365 7276 6528        def serve(
-00006870: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00006880: 2020 2020 2020 2063 6c69 656e 742c 205f         client, _
-00006890: 203d 2073 6572 7665 725f 736f 636b 2e61   = server_sock.a
-000068a0: 6363 6570 7428 290a 2020 2020 2020 2020  ccept().        
-000068b0: 2020 2020 636c 6965 6e74 2e73 656e 6461      client.senda
-000068c0: 6c6c 2862 7566 6665 7229 0a20 2020 2020  ll(buffer).     
-000068d0: 2020 2020 2020 2063 6c69 656e 742e 636c         client.cl
-000068e0: 6f73 6528 290a 0a20 2020 2020 2020 2062  ose()..        b
-000068f0: 7566 6665 7220 3d20 280a 2020 2020 2020  uffer = (.      
-00006900: 2020 2020 2020 6222 5c78 6666 2220 2a20        b"\xff" * 
-00006910: 3130 3234 202a 2035 3132 202b 2062 225c  1024 * 512 + b"\
-00006920: 7830 3022 202a 2031 3032 3420 2a20 3531  x00" * 1024 * 51
-00006930: 320a 2020 2020 2020 2020 2920 2023 2073  2.        )  # s
-00006940: 686f 756c 6420 6578 6365 6564 2074 6865  hould exceed the
-00006950: 206d 6178 696d 756d 206b 6572 6e65 6c20   maximum kernel 
-00006960: 7365 6e64 2062 7566 6665 7220 7369 7a65  send buffer size
-00006970: 0a20 2020 2020 2020 2061 7379 6e63 2077  .        async w
-00006980: 6974 6820 6177 6169 7420 636f 6e6e 6563  ith await connec
-00006990: 745f 756e 6978 2873 6f63 6b65 745f 7061  t_unix(socket_pa
-000069a0: 7468 2920 6173 2073 7472 6561 6d3a 0a20  th) as stream:. 
-000069b0: 2020 2020 2020 2020 2020 2074 6872 6561             threa
-000069c0: 6420 3d20 5468 7265 6164 2874 6172 6765  d = Thread(targe
-000069d0: 743d 7365 7276 652c 2064 6165 6d6f 6e3d  t=serve, daemon=
-000069e0: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-000069f0: 2020 7468 7265 6164 2e73 7461 7274 2829    thread.start()
-00006a00: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00006a10: 706f 6e73 6520 3d20 6222 220a 2020 2020  ponse = b"".    
-00006a20: 2020 2020 2020 2020 7768 696c 6520 6c65          while le
-00006a30: 6e28 7265 7370 6f6e 7365 2920 3c20 6c65  n(response) < le
-00006a40: 6e28 6275 6666 6572 293a 0a20 2020 2020  n(buffer):.     
-00006a50: 2020 2020 2020 2020 2020 2072 6573 706f             respo
-00006a60: 6e73 6520 2b3d 2061 7761 6974 2073 7472  nse += await str
-00006a70: 6561 6d2e 7265 6365 6976 6528 290a 0a20  eam.receive().. 
-00006a80: 2020 2020 2020 2074 6872 6561 642e 6a6f         thread.jo
-00006a90: 696e 2829 0a20 2020 2020 2020 2061 7373  in().        ass
-00006aa0: 6572 7420 7265 7370 6f6e 7365 203d 3d20  ert response == 
-00006ab0: 6275 6666 6572 0a0a 2020 2020 6173 796e  buffer..    asyn
-00006ac0: 6320 6465 6620 7465 7374 5f73 656e 645f  c def test_send_
-00006ad0: 6c61 7267 655f 6275 6666 6572 280a 2020  large_buffer(.  
-00006ae0: 2020 2020 2020 7365 6c66 2c20 7365 7276        self, serv
-00006af0: 6572 5f73 6f63 6b3a 2073 6f63 6b65 742e  er_sock: socket.
-00006b00: 736f 636b 6574 2c20 736f 636b 6574 5f70  socket, socket_p
-00006b10: 6174 683a 2050 6174 680a 2020 2020 2920  ath: Path.    ) 
-00006b20: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00006b30: 2072 6573 706f 6e73 6520 3d20 6222 220a   response = b"".
-00006b40: 0a20 2020 2020 2020 2064 6566 2073 6572  .        def ser
-00006b50: 7665 2829 202d 3e20 4e6f 6e65 3a0a 2020  ve() -> None:.  
-00006b60: 2020 2020 2020 2020 2020 6e6f 6e6c 6f63            nonloc
-00006b70: 616c 2072 6573 706f 6e73 650a 2020 2020  al response.    
-00006b80: 2020 2020 2020 2020 636c 6965 6e74 2c20          client, 
-00006b90: 5f20 3d20 7365 7276 6572 5f73 6f63 6b2e  _ = server_sock.
-00006ba0: 6163 6365 7074 2829 0a20 2020 2020 2020  accept().       
-00006bb0: 2020 2020 2077 6869 6c65 2054 7275 653a       while True:
-00006bc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006bd0: 2064 6174 6120 3d20 636c 6965 6e74 2e72   data = client.r
-00006be0: 6563 7628 3130 3234 290a 2020 2020 2020  ecv(1024).      
-00006bf0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00006c00: 2064 6174 613a 0a20 2020 2020 2020 2020   data:.         
-00006c10: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00006c20: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006c30: 2020 7265 7370 6f6e 7365 202b 3d20 6461    response += da
-00006c40: 7461 0a0a 2020 2020 2020 2020 2020 2020  ta..            
-00006c50: 636c 6965 6e74 2e63 6c6f 7365 2829 0a0a  client.close()..
-00006c60: 2020 2020 2020 2020 6275 6666 6572 203d          buffer =
-00006c70: 2028 0a20 2020 2020 2020 2020 2020 2062   (.            b
-00006c80: 225c 7866 6622 202a 2031 3032 3420 2a20  "\xff" * 1024 * 
-00006c90: 3531 3220 2b20 6222 5c78 3030 2220 2a20  512 + b"\x00" * 
-00006ca0: 3130 3234 202a 2035 3132 0a20 2020 2020  1024 * 512.     
-00006cb0: 2020 2029 2020 2320 7368 6f75 6c64 2065     )  # should e
-00006cc0: 7863 6565 6420 7468 6520 6d61 7869 6d75  xceed the maximu
-00006cd0: 6d20 6b65 726e 656c 2073 656e 6420 6275  m kernel send bu
-00006ce0: 6666 6572 2073 697a 650a 2020 2020 2020  ffer size.      
-00006cf0: 2020 6173 796e 6320 7769 7468 2061 7761    async with awa
-00006d00: 6974 2063 6f6e 6e65 6374 5f75 6e69 7828  it connect_unix(
-00006d10: 736f 636b 6574 5f70 6174 6829 2061 7320  socket_path) as 
-00006d20: 7374 7265 616d 3a0a 2020 2020 2020 2020  stream:.        
-00006d30: 2020 2020 7468 7265 6164 203d 2054 6872      thread = Thr
-00006d40: 6561 6428 7461 7267 6574 3d73 6572 7665  ead(target=serve
-00006d50: 2c20 6461 656d 6f6e 3d54 7275 6529 0a20  , daemon=True). 
-00006d60: 2020 2020 2020 2020 2020 2074 6872 6561             threa
-00006d70: 642e 7374 6172 7428 290a 2020 2020 2020  d.start().      
-00006d80: 2020 2020 2020 6177 6169 7420 7374 7265        await stre
-00006d90: 616d 2e73 656e 6428 6275 6666 6572 290a  am.send(buffer).
-00006da0: 0a20 2020 2020 2020 2074 6872 6561 642e  .        thread.
-00006db0: 6a6f 696e 2829 0a20 2020 2020 2020 2061  join().        a
-00006dc0: 7373 6572 7420 7265 7370 6f6e 7365 203d  ssert response =
-00006dd0: 3d20 6275 6666 6572 0a0a 2020 2020 6173  = buffer..    as
-00006de0: 796e 6320 6465 6620 7465 7374 5f72 6563  ync def test_rec
-00006df0: 6569 7665 5f66 6473 280a 2020 2020 2020  eive_fds(.      
-00006e00: 2020 7365 6c66 2c20 7365 7276 6572 5f73    self, server_s
-00006e10: 6f63 6b3a 2073 6f63 6b65 742e 736f 636b  ock: socket.sock
-00006e20: 6574 2c20 736f 636b 6574 5f70 6174 683a  et, socket_path:
-00006e30: 2050 6174 682c 2074 6d70 5f70 6174 683a   Path, tmp_path:
-00006e40: 2050 6174 680a 2020 2020 2920 2d3e 204e   Path.    ) -> N
-00006e50: 6f6e 653a 0a20 2020 2020 2020 2064 6566  one:.        def
-00006e60: 2073 6572 7665 2829 202d 3e20 4e6f 6e65   serve() -> None
-00006e70: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
-00006e80: 7468 3120 3d20 746d 705f 7061 7468 202f  th1 = tmp_path /
-00006e90: 2022 6669 6c65 3122 0a20 2020 2020 2020   "file1".       
-00006ea0: 2020 2020 2070 6174 6832 203d 2074 6d70       path2 = tmp
-00006eb0: 5f70 6174 6820 2f20 2266 696c 6532 220a  _path / "file2".
-00006ec0: 2020 2020 2020 2020 2020 2020 7061 7468              path
-00006ed0: 312e 7772 6974 655f 7465 7874 2822 4865  1.write_text("He
-00006ee0: 6c6c 6f2c 2022 290a 2020 2020 2020 2020  llo, ").        
-00006ef0: 2020 2020 7061 7468 322e 7772 6974 655f      path2.write_
-00006f00: 7465 7874 2822 576f 726c 6421 2229 0a20  text("World!"). 
-00006f10: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00006f20: 7061 7468 312e 6f70 656e 2829 2061 7320  path1.open() as 
-00006f30: 6669 6c65 312c 2070 6174 6832 2e6f 7065  file1, path2.ope
-00006f40: 6e28 2920 6173 2066 696c 6532 3a0a 2020  n() as file2:.  
-00006f50: 2020 2020 2020 2020 2020 2020 2020 6664                fd
-00006f60: 6172 7261 7920 3d20 6172 7261 792e 6172  array = array.ar
-00006f70: 7261 7928 2269 222c 205b 6669 6c65 312e  ray("i", [file1.
-00006f80: 6669 6c65 6e6f 2829 2c20 6669 6c65 322e  fileno(), file2.
-00006f90: 6669 6c65 6e6f 2829 5d29 0a20 2020 2020  fileno()]).     
-00006fa0: 2020 2020 2020 2020 2020 2063 6c69 656e             clien
-00006fb0: 742c 205f 203d 2073 6572 7665 725f 736f  t, _ = server_so
-00006fc0: 636b 2e61 6363 6570 7428 290a 2020 2020  ck.accept().    
-00006fd0: 2020 2020 2020 2020 2020 2020 636d 7367              cmsg
-00006fe0: 203d 2028 736f 636b 6574 2e53 4f4c 5f53   = (socket.SOL_S
-00006ff0: 4f43 4b45 542c 2073 6f63 6b65 742e 5343  OCKET, socket.SC
-00007000: 4d5f 5249 4748 5453 2c20 6664 6172 7261  M_RIGHTS, fdarra
-00007010: 7929 0a20 2020 2020 2020 2020 2020 2020  y).             
-00007020: 2020 2077 6974 6820 636c 6965 6e74 3a0a     with client:.
-00007030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007040: 2020 2020 636c 6965 6e74 2e73 656e 646d      client.sendm
-00007050: 7367 285b 6222 7465 7374 225d 2c20 5b63  sg([b"test"], [c
-00007060: 6d73 675d 290a 0a20 2020 2020 2020 2061  msg])..        a
-00007070: 7379 6e63 2077 6974 6820 6177 6169 7420  sync with await 
-00007080: 636f 6e6e 6563 745f 756e 6978 2873 6f63  connect_unix(soc
-00007090: 6b65 745f 7061 7468 2920 6173 2073 7472  ket_path) as str
-000070a0: 6561 6d3a 0a20 2020 2020 2020 2020 2020  eam:.           
-000070b0: 2074 6872 6561 6420 3d20 5468 7265 6164   thread = Thread
-000070c0: 2874 6172 6765 743d 7365 7276 652c 2064  (target=serve, d
-000070d0: 6165 6d6f 6e3d 5472 7565 290a 2020 2020  aemon=True).    
-000070e0: 2020 2020 2020 2020 7468 7265 6164 2e73          thread.s
-000070f0: 7461 7274 2829 0a20 2020 2020 2020 2020  tart().         
-00007100: 2020 206d 6573 7361 6765 2c20 6664 7320     message, fds 
-00007110: 3d20 6177 6169 7420 7374 7265 616d 2e72  = await stream.r
-00007120: 6563 6569 7665 5f66 6473 2831 302c 2032  eceive_fds(10, 2
-00007130: 290a 2020 2020 2020 2020 2020 2020 7468  ).            th
-00007140: 7265 6164 2e6a 6f69 6e28 290a 0a20 2020  read.join()..   
-00007150: 2020 2020 2074 6578 7420 3d20 2222 0a20       text = "". 
-00007160: 2020 2020 2020 2066 6f72 2066 6420 696e         for fd in
-00007170: 2066 6473 3a0a 2020 2020 2020 2020 2020   fds:.          
-00007180: 2020 7769 7468 206f 732e 6664 6f70 656e    with os.fdopen
-00007190: 2866 6429 2061 7320 6669 6c65 3a0a 2020  (fd) as file:.  
-000071a0: 2020 2020 2020 2020 2020 2020 2020 7465                te
-000071b0: 7874 202b 3d20 6669 6c65 2e72 6561 6428  xt += file.read(
-000071c0: 290a 0a20 2020 2020 2020 2061 7373 6572  )..        asser
-000071d0: 7420 6d65 7373 6167 6520 3d3d 2062 2274  t message == b"t
-000071e0: 6573 7422 0a20 2020 2020 2020 2061 7373  est".        ass
-000071f0: 6572 7420 7465 7874 203d 3d20 2248 656c  ert text == "Hel
-00007200: 6c6f 2c20 576f 726c 6421 220a 0a20 2020  lo, World!"..   
-00007210: 2061 7379 6e63 2064 6566 2074 6573 745f   async def test_
-00007220: 7265 6365 6976 655f 6664 735f 6261 645f  receive_fds_bad_
-00007230: 6172 6773 280a 2020 2020 2020 2020 7365  args(.        se
-00007240: 6c66 2c20 7365 7276 6572 5f73 6f63 6b3a  lf, server_sock:
-00007250: 2073 6f63 6b65 742e 736f 636b 6574 2c20   socket.socket, 
-00007260: 736f 636b 6574 5f70 6174 683a 2050 6174  socket_path: Pat
-00007270: 680a 2020 2020 2920 2d3e 204e 6f6e 653a  h.    ) -> None:
-00007280: 0a20 2020 2020 2020 2061 7379 6e63 2077  .        async w
-00007290: 6974 6820 6177 6169 7420 636f 6e6e 6563  ith await connec
-000072a0: 745f 756e 6978 2873 6f63 6b65 745f 7061  t_unix(socket_pa
-000072b0: 7468 2920 6173 2073 7472 6561 6d3a 0a20  th) as stream:. 
-000072c0: 2020 2020 2020 2020 2020 2066 6f72 206d             for m
-000072d0: 7367 6c65 6e20 696e 2028 2d31 2c20 2266  sglen in (-1, "f
-000072e0: 6f6f 2229 3a0a 2020 2020 2020 2020 2020  oo"):.          
-000072f0: 2020 2020 2020 7769 7468 2070 7974 6573        with pytes
-00007300: 742e 7261 6973 6573 280a 2020 2020 2020  t.raises(.      
-00007310: 2020 2020 2020 2020 2020 2020 2020 5661                Va
-00007320: 6c75 6545 7272 6f72 2c20 6d61 7463 683d  lueError, match=
-00007330: 226d 7367 6c65 6e20 6d75 7374 2062 6520  "msglen must be 
-00007340: 6120 6e6f 6e2d 6e65 6761 7469 7665 2069  a non-negative i
-00007350: 6e74 6567 6572 220a 2020 2020 2020 2020  nteger".        
-00007360: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-00007370: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00007380: 7761 6974 2073 7472 6561 6d2e 7265 6365  wait stream.rece
-00007390: 6976 655f 6664 7328 6d73 676c 656e 2c20  ive_fds(msglen, 
-000073a0: 3029 2020 2320 7479 7065 3a20 6967 6e6f  0)  # type: igno
-000073b0: 7265 5b61 7267 2d74 7970 655d 0a0a 2020  re[arg-type]..  
-000073c0: 2020 2020 2020 2020 2020 666f 7220 6d61            for ma
-000073d0: 7866 6473 2069 6e20 2830 2c20 2266 6f6f  xfds in (0, "foo
-000073e0: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-000073f0: 2020 2020 7769 7468 2070 7974 6573 742e      with pytest.
-00007400: 7261 6973 6573 280a 2020 2020 2020 2020  raises(.        
-00007410: 2020 2020 2020 2020 2020 2020 5661 6c75              Valu
-00007420: 6545 7272 6f72 2c20 6d61 7463 683d 226d  eError, match="m
-00007430: 6178 6664 7320 6d75 7374 2062 6520 6120  axfds must be a 
-00007440: 706f 7369 7469 7665 2069 6e74 6567 6572  positive integer
-00007450: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00007460: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
-00007470: 2020 2020 2020 2020 2061 7761 6974 2073           await s
-00007480: 7472 6561 6d2e 7265 6365 6976 655f 6664  tream.receive_fd
-00007490: 7328 302c 206d 6178 6664 7329 2020 2320  s(0, maxfds)  # 
-000074a0: 7479 7065 3a20 6967 6e6f 7265 5b61 7267  type: ignore[arg
-000074b0: 2d74 7970 655d 0a0a 2020 2020 6173 796e  -type]..    asyn
-000074c0: 6320 6465 6620 7465 7374 5f73 656e 645f  c def test_send_
-000074d0: 6664 7328 0a20 2020 2020 2020 2073 656c  fds(.        sel
-000074e0: 662c 2073 6572 7665 725f 736f 636b 3a20  f, server_sock: 
-000074f0: 736f 636b 6574 2e73 6f63 6b65 742c 2073  socket.socket, s
-00007500: 6f63 6b65 745f 7061 7468 3a20 5061 7468  ocket_path: Path
-00007510: 2c20 746d 705f 7061 7468 3a20 5061 7468  , tmp_path: Path
-00007520: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a0a  .    ) -> None:.
-00007530: 2020 2020 2020 2020 6465 6620 7365 7276          def serv
-00007540: 6528 2920 2d3e 204e 6f6e 653a 0a20 2020  e() -> None:.   
-00007550: 2020 2020 2020 2020 2066 6473 203d 2061           fds = a
-00007560: 7272 6179 2e61 7272 6179 2822 6922 290a  rray.array("i").
-00007570: 2020 2020 2020 2020 2020 2020 636c 6965              clie
-00007580: 6e74 2c20 5f20 3d20 7365 7276 6572 5f73  nt, _ = server_s
-00007590: 6f63 6b2e 6163 6365 7074 2829 0a20 2020  ock.accept().   
-000075a0: 2020 2020 2020 2020 206d 7367 2c20 616e           msg, an
-000075b0: 6364 6174 612c 202a 5f20 3d20 636c 6965  cdata, *_ = clie
-000075c0: 6e74 2e72 6563 766d 7367 2831 302c 2073  nt.recvmsg(10, s
-000075d0: 6f63 6b65 742e 434d 5347 5f4c 454e 2832  ocket.CMSG_LEN(2
-000075e0: 202a 2066 6473 2e69 7465 6d73 697a 6529   * fds.itemsize)
-000075f0: 290a 2020 2020 2020 2020 2020 2020 636c  ).            cl
-00007600: 6965 6e74 2e63 6c6f 7365 2829 0a20 2020  ient.close().   
-00007610: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-00007620: 6d73 6720 3d3d 2062 2274 6573 7422 0a20  msg == b"test". 
-00007630: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
-00007640: 6d73 675f 6c65 7665 6c2c 2063 6d73 675f  msg_level, cmsg_
-00007650: 7479 7065 2c20 636d 7367 5f64 6174 6120  type, cmsg_data 
-00007660: 696e 2061 6e63 6461 7461 3a0a 2020 2020  in ancdata:.    
-00007670: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-00007680: 7274 2063 6d73 675f 6c65 7665 6c20 3d3d  rt cmsg_level ==
-00007690: 2073 6f63 6b65 742e 534f 4c5f 534f 434b   socket.SOL_SOCK
-000076a0: 4554 0a20 2020 2020 2020 2020 2020 2020  ET.             
-000076b0: 2020 2061 7373 6572 7420 636d 7367 5f74     assert cmsg_t
-000076c0: 7970 6520 3d3d 2073 6f63 6b65 742e 5343  ype == socket.SC
-000076d0: 4d5f 5249 4748 5453 0a20 2020 2020 2020  M_RIGHTS.       
-000076e0: 2020 2020 2020 2020 2066 6473 2e66 726f           fds.fro
-000076f0: 6d62 7974 6573 280a 2020 2020 2020 2020  mbytes(.        
-00007700: 2020 2020 2020 2020 2020 2020 636d 7367              cmsg
-00007710: 5f64 6174 615b 3a20 6c65 6e28 636d 7367  _data[: len(cmsg
-00007720: 5f64 6174 6129 202d 2028 6c65 6e28 636d  _data) - (len(cm
-00007730: 7367 5f64 6174 6129 2025 2066 6473 2e69  sg_data) % fds.i
-00007740: 7465 6d73 697a 6529 5d0a 2020 2020 2020  temsize)].      
-00007750: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00007760: 2020 2020 2020 2020 2074 6578 7420 3d20           text = 
-00007770: 2222 0a20 2020 2020 2020 2020 2020 2066  "".            f
-00007780: 6f72 2066 6420 696e 2066 6473 3a0a 2020  or fd in fds:.  
-00007790: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-000077a0: 7468 206f 732e 6664 6f70 656e 2866 6429  th os.fdopen(fd)
-000077b0: 2061 7320 6669 6c65 3a0a 2020 2020 2020   as file:.      
-000077c0: 2020 2020 2020 2020 2020 2020 2020 7465                te
-000077d0: 7874 202b 3d20 6669 6c65 2e72 6561 6428  xt += file.read(
-000077e0: 290a 0a20 2020 2020 2020 2020 2020 2061  )..            a
-000077f0: 7373 6572 7420 7465 7874 203d 3d20 2248  ssert text == "H
-00007800: 656c 6c6f 2c20 576f 726c 6421 220a 0a20  ello, World!".. 
-00007810: 2020 2020 2020 2070 6174 6831 203d 2074         path1 = t
-00007820: 6d70 5f70 6174 6820 2f20 2266 696c 6531  mp_path / "file1
-00007830: 220a 2020 2020 2020 2020 7061 7468 3220  ".        path2 
-00007840: 3d20 746d 705f 7061 7468 202f 2022 6669  = tmp_path / "fi
-00007850: 6c65 3222 0a20 2020 2020 2020 2070 6174  le2".        pat
-00007860: 6831 2e77 7269 7465 5f74 6578 7428 2248  h1.write_text("H
-00007870: 656c 6c6f 2c20 2229 0a20 2020 2020 2020  ello, ").       
-00007880: 2070 6174 6832 2e77 7269 7465 5f74 6578   path2.write_tex
-00007890: 7428 2257 6f72 6c64 2122 290a 2020 2020  t("World!").    
-000078a0: 2020 2020 7769 7468 2070 6174 6831 2e6f      with path1.o
-000078b0: 7065 6e28 2920 6173 2066 696c 6531 2c20  pen() as file1, 
-000078c0: 7061 7468 322e 6f70 656e 2829 2061 7320  path2.open() as 
-000078d0: 6669 6c65 322c 2066 6169 6c5f 6166 7465  file2, fail_afte
-000078e0: 7228 3229 3a0a 2020 2020 2020 2020 2020  r(2):.          
-000078f0: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
-00007900: 6e63 6528 6669 6c65 312c 2069 6f2e 5465  nce(file1, io.Te
-00007910: 7874 494f 5772 6170 7065 7229 0a20 2020  xtIOWrapper).   
-00007920: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-00007930: 6973 696e 7374 616e 6365 2866 696c 6532  isinstance(file2
-00007940: 2c20 696f 2e54 6578 7449 4f57 7261 7070  , io.TextIOWrapp
-00007950: 6572 290a 2020 2020 2020 2020 2020 2020  er).            
-00007960: 6173 796e 6320 7769 7468 2061 7761 6974  async with await
-00007970: 2063 6f6e 6e65 6374 5f75 6e69 7828 736f   connect_unix(so
-00007980: 636b 6574 5f70 6174 6829 2061 7320 7374  cket_path) as st
-00007990: 7265 616d 3a0a 2020 2020 2020 2020 2020  ream:.          
-000079a0: 2020 2020 2020 7468 7265 6164 203d 2054        thread = T
-000079b0: 6872 6561 6428 7461 7267 6574 3d73 6572  hread(target=ser
-000079c0: 7665 2c20 6461 656d 6f6e 3d54 7275 6529  ve, daemon=True)
-000079d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000079e0: 2074 6872 6561 642e 7374 6172 7428 290a   thread.start().
-000079f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a00: 6177 6169 7420 7374 7265 616d 2e73 656e  await stream.sen
-00007a10: 645f 6664 7328 6222 7465 7374 222c 205b  d_fds(b"test", [
-00007a20: 6669 6c65 312c 2066 696c 6532 5d29 0a20  file1, file2]). 
-00007a30: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00007a40: 6872 6561 642e 6a6f 696e 2829 0a0a 2020  hread.join()..  
-00007a50: 2020 6173 796e 6320 6465 6620 7465 7374    async def test
-00007a60: 5f73 656e 645f 656f 6628 0a20 2020 2020  _send_eof(.     
-00007a70: 2020 2073 656c 662c 2073 6572 7665 725f     self, server_
-00007a80: 736f 636b 3a20 736f 636b 6574 2e73 6f63  sock: socket.soc
-00007a90: 6b65 742c 2073 6f63 6b65 745f 7061 7468  ket, socket_path
-00007aa0: 3a20 5061 7468 0a20 2020 2029 202d 3e20  : Path.    ) -> 
-00007ab0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6465  None:.        de
-00007ac0: 6620 7365 7276 6528 2920 2d3e 204e 6f6e  f serve() -> Non
-00007ad0: 653a 0a20 2020 2020 2020 2020 2020 2063  e:.            c
-00007ae0: 6c69 656e 742c 205f 203d 2073 6572 7665  lient, _ = serve
-00007af0: 725f 736f 636b 2e61 6363 6570 7428 290a  r_sock.accept().
-00007b00: 2020 2020 2020 2020 2020 2020 7265 7175              requ
-00007b10: 6573 7420 3d20 6222 220a 2020 2020 2020  est = b"".      
-00007b20: 2020 2020 2020 7768 696c 6520 5472 7565        while True
-00007b30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00007b40: 2020 6461 7461 203d 2063 6c69 656e 742e    data = client.
-00007b50: 7265 6376 2831 3030 290a 2020 2020 2020  recv(100).      
-00007b60: 2020 2020 2020 2020 2020 7265 7175 6573            reques
-00007b70: 7420 2b3d 2064 6174 610a 2020 2020 2020  t += data.      
-00007b80: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00007b90: 2064 6174 613a 0a20 2020 2020 2020 2020   data:.         
-00007ba0: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00007bb0: 0a0a 2020 2020 2020 2020 2020 2020 636c  ..            cl
-00007bc0: 6965 6e74 2e73 656e 6461 6c6c 2872 6571  ient.sendall(req
-00007bd0: 7565 7374 5b3a 3a2d 315d 290a 2020 2020  uest[::-1]).    
-00007be0: 2020 2020 2020 2020 636c 6965 6e74 2e63          client.c
-00007bf0: 6c6f 7365 2829 0a0a 2020 2020 2020 2020  lose()..        
-00007c00: 6173 796e 6320 7769 7468 2061 7761 6974  async with await
-00007c10: 2063 6f6e 6e65 6374 5f75 6e69 7828 736f   connect_unix(so
-00007c20: 636b 6574 5f70 6174 6829 2061 7320 7374  cket_path) as st
-00007c30: 7265 616d 3a0a 2020 2020 2020 2020 2020  ream:.          
-00007c40: 2020 7468 7265 6164 203d 2054 6872 6561    thread = Threa
-00007c50: 6428 7461 7267 6574 3d73 6572 7665 2c20  d(target=serve, 
-00007c60: 6461 656d 6f6e 3d54 7275 6529 0a20 2020  daemon=True).   
-00007c70: 2020 2020 2020 2020 2074 6872 6561 642e           thread.
-00007c80: 7374 6172 7428 290a 2020 2020 2020 2020  start().        
-00007c90: 2020 2020 6177 6169 7420 7374 7265 616d      await stream
-00007ca0: 2e73 656e 6428 6222 6865 6c6c 6f2c 2022  .send(b"hello, "
-00007cb0: 290a 2020 2020 2020 2020 2020 2020 6177  ).            aw
-00007cc0: 6169 7420 7374 7265 616d 2e73 656e 6428  ait stream.send(
-00007cd0: 6222 776f 726c 645c 6e22 290a 2020 2020  b"world\n").    
-00007ce0: 2020 2020 2020 2020 6177 6169 7420 7374          await st
-00007cf0: 7265 616d 2e73 656e 645f 656f 6628 290a  ream.send_eof().
-00007d00: 2020 2020 2020 2020 2020 2020 7265 7370              resp
-00007d10: 6f6e 7365 203d 2061 7761 6974 2073 7472  onse = await str
-00007d20: 6561 6d2e 7265 6365 6976 6528 290a 0a20  eam.receive().. 
-00007d30: 2020 2020 2020 2074 6872 6561 642e 6a6f         thread.jo
-00007d40: 696e 2829 0a20 2020 2020 2020 2061 7373  in().        ass
-00007d50: 6572 7420 7265 7370 6f6e 7365 203d 3d20  ert response == 
-00007d60: 6222 5c6e 646c 726f 7720 2c6f 6c6c 6568  b"\ndlrow ,olleh
-00007d70: 220a 0a20 2020 2061 7379 6e63 2064 6566  "..    async def
-00007d80: 2074 6573 745f 6974 6572 6174 6528 7365   test_iterate(se
-00007d90: 6c66 2c20 7365 7276 6572 5f73 6f63 6b3a  lf, server_sock:
-00007da0: 2073 6f63 6b65 742e 736f 636b 6574 2c20   socket.socket, 
-00007db0: 736f 636b 6574 5f70 6174 683a 2050 6174  socket_path: Pat
-00007dc0: 6829 202d 3e20 4e6f 6e65 3a0a 2020 2020  h) -> None:.    
-00007dd0: 2020 2020 6465 6620 7365 7276 6528 2920      def serve() 
-00007de0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00007df0: 2020 2020 2063 6c69 656e 742c 205f 203d       client, _ =
-00007e00: 2073 6572 7665 725f 736f 636b 2e61 6363   server_sock.acc
-00007e10: 6570 7428 290a 2020 2020 2020 2020 2020  ept().          
-00007e20: 2020 636c 6965 6e74 2e73 656e 6461 6c6c    client.sendall
-00007e30: 2862 2262 6c22 290a 2020 2020 2020 2020  (b"bl").        
-00007e40: 2020 2020 7469 6d65 2e73 6c65 6570 2830      time.sleep(0
-00007e50: 2e30 3529 0a20 2020 2020 2020 2020 2020  .05).           
-00007e60: 2063 6c69 656e 742e 7365 6e64 616c 6c28   client.sendall(
-00007e70: 6222 6168 2229 0a20 2020 2020 2020 2020  b"ah").         
-00007e80: 2020 2063 6c69 656e 742e 636c 6f73 6528     client.close(
-00007e90: 290a 0a20 2020 2020 2020 2074 6872 6561  )..        threa
-00007ea0: 6420 3d20 5468 7265 6164 2874 6172 6765  d = Thread(targe
-00007eb0: 743d 7365 7276 652c 2064 6165 6d6f 6e3d  t=serve, daemon=
-00007ec0: 5472 7565 290a 2020 2020 2020 2020 7468  True).        th
-00007ed0: 7265 6164 2e73 7461 7274 2829 0a20 2020  read.start().   
-00007ee0: 2020 2020 2063 6875 6e6b 7320 3d20 5b5d       chunks = []
-00007ef0: 0a20 2020 2020 2020 2061 7379 6e63 2077  .        async w
-00007f00: 6974 6820 6177 6169 7420 636f 6e6e 6563  ith await connec
-00007f10: 745f 756e 6978 2873 6f63 6b65 745f 7061  t_unix(socket_pa
-00007f20: 7468 2920 6173 2073 7472 6561 6d3a 0a20  th) as stream:. 
-00007f30: 2020 2020 2020 2020 2020 2061 7379 6e63             async
-00007f40: 2066 6f72 2063 6875 6e6b 2069 6e20 7374   for chunk in st
-00007f50: 7265 616d 3a0a 2020 2020 2020 2020 2020  ream:.          
-00007f60: 2020 2020 2020 6368 756e 6b73 2e61 7070        chunks.app
-00007f70: 656e 6428 6368 756e 6b29 0a0a 2020 2020  end(chunk)..    
-00007f80: 2020 2020 7468 7265 6164 2e6a 6f69 6e28      thread.join(
-00007f90: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
-00007fa0: 2063 6875 6e6b 7320 3d3d 205b 6222 626c   chunks == [b"bl
-00007fb0: 222c 2062 2261 6822 5d0a 0a20 2020 2061  ", b"ah"]..    a
-00007fc0: 7379 6e63 2064 6566 2074 6573 745f 7365  sync def test_se
-00007fd0: 6e64 5f66 6473 5f62 6164 5f61 7267 7328  nd_fds_bad_args(
-00007fe0: 0a20 2020 2020 2020 2073 656c 662c 2073  .        self, s
-00007ff0: 6572 7665 725f 736f 636b 3a20 736f 636b  erver_sock: sock
-00008000: 6574 2e73 6f63 6b65 742c 2073 6f63 6b65  et.socket, socke
-00008010: 745f 7061 7468 3a20 5061 7468 0a20 2020  t_path: Path.   
-00008020: 2029 202d 3e20 4e6f 6e65 3a0a 2020 2020   ) -> None:.    
-00008030: 2020 2020 6173 796e 6320 7769 7468 2061      async with a
-00008040: 7761 6974 2063 6f6e 6e65 6374 5f75 6e69  wait connect_uni
-00008050: 7828 736f 636b 6574 5f70 6174 6829 2061  x(socket_path) a
-00008060: 7320 7374 7265 616d 3a0a 2020 2020 2020  s stream:.      
-00008070: 2020 2020 2020 7769 7468 2070 7974 6573        with pytes
-00008080: 742e 7261 6973 6573 2856 616c 7565 4572  t.raises(ValueEr
-00008090: 726f 722c 206d 6174 6368 3d22 6d65 7373  ror, match="mess
-000080a0: 6167 6520 6d75 7374 206e 6f74 2062 6520  age must not be 
-000080b0: 656d 7074 7922 293a 0a20 2020 2020 2020  empty"):.       
-000080c0: 2020 2020 2020 2020 2061 7761 6974 2073           await s
-000080d0: 7472 6561 6d2e 7365 6e64 5f66 6473 2862  tream.send_fds(b
-000080e0: 2222 2c20 5b30 5d29 0a0a 2020 2020 2020  "", [0])..      
-000080f0: 2020 2020 2020 7769 7468 2070 7974 6573        with pytes
-00008100: 742e 7261 6973 6573 2856 616c 7565 4572  t.raises(ValueEr
-00008110: 726f 722c 206d 6174 6368 3d22 6664 7320  ror, match="fds 
-00008120: 6d75 7374 206e 6f74 2062 6520 656d 7074  must not be empt
-00008130: 7922 293a 0a20 2020 2020 2020 2020 2020  y"):.           
-00008140: 2020 2020 2061 7761 6974 2073 7472 6561       await strea
-00008150: 6d2e 7365 6e64 5f66 6473 2862 2274 6573  m.send_fds(b"tes
-00008160: 7422 2c20 5b5d 290a 0a20 2020 2061 7379  t", [])..    asy
-00008170: 6e63 2064 6566 2074 6573 745f 636f 6e63  nc def test_conc
-00008180: 7572 7265 6e74 5f73 656e 6428 0a20 2020  urrent_send(.   
-00008190: 2020 2020 2073 656c 662c 2073 6572 7665       self, serve
-000081a0: 725f 736f 636b 3a20 736f 636b 6574 2e73  r_sock: socket.s
-000081b0: 6f63 6b65 742c 2073 6f63 6b65 745f 7061  ocket, socket_pa
-000081c0: 7468 3a20 5061 7468 0a20 2020 2029 202d  th: Path.    ) -
-000081d0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-000081e0: 6173 796e 6320 6465 6620 7365 6e64 5f64  async def send_d
-000081f0: 6174 6128 2920 2d3e 204e 6f52 6574 7572  ata() -> NoRetur
-00008200: 6e3a 0a20 2020 2020 2020 2020 2020 2077  n:.            w
-00008210: 6869 6c65 2054 7275 653a 0a20 2020 2020  hile True:.     
-00008220: 2020 2020 2020 2020 2020 2061 7761 6974             await
-00008230: 2063 6c69 656e 742e 7365 6e64 2862 225c   client.send(b"\
-00008240: 7830 3022 202a 2034 3039 3629 0a0a 2020  x00" * 4096)..  
-00008250: 2020 2020 2020 6173 796e 6320 7769 7468        async with
-00008260: 2061 7761 6974 2063 6f6e 6e65 6374 5f75   await connect_u
-00008270: 6e69 7828 736f 636b 6574 5f70 6174 6829  nix(socket_path)
-00008280: 2061 7320 636c 6965 6e74 3a0a 2020 2020   as client:.    
-00008290: 2020 2020 2020 2020 6173 796e 6320 7769          async wi
-000082a0: 7468 2063 7265 6174 655f 7461 736b 5f67  th create_task_g
-000082b0: 726f 7570 2829 2061 7320 7467 3a0a 2020  roup() as tg:.  
-000082c0: 2020 2020 2020 2020 2020 2020 2020 7467                tg
-000082d0: 2e73 7461 7274 5f73 6f6f 6e28 7365 6e64  .start_soon(send
-000082e0: 5f64 6174 6129 0a20 2020 2020 2020 2020  _data).         
-000082f0: 2020 2020 2020 2061 7761 6974 2077 6169         await wai
-00008300: 745f 616c 6c5f 7461 736b 735f 626c 6f63  t_all_tasks_bloc
-00008310: 6b65 6428 290a 2020 2020 2020 2020 2020  ked().          
-00008320: 2020 2020 2020 7769 7468 2070 7974 6573        with pytes
-00008330: 742e 7261 6973 6573 2842 7573 7952 6573  t.raises(BusyRes
-00008340: 6f75 7263 6545 7272 6f72 2920 6173 2065  ourceError) as e
-00008350: 7863 3a0a 2020 2020 2020 2020 2020 2020  xc:.            
-00008360: 2020 2020 2020 2020 6177 6169 7420 636c          await cl
-00008370: 6965 6e74 2e73 656e 6428 6222 666f 6f22  ient.send(b"foo"
-00008380: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-00008390: 2020 2065 7863 2e6d 6174 6368 2822 616c     exc.match("al
-000083a0: 7265 6164 7920 7772 6974 696e 6720 746f  ready writing to
-000083b0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-000083c0: 2020 2074 672e 6361 6e63 656c 5f73 636f     tg.cancel_sco
-000083d0: 7065 2e63 616e 6365 6c28 290a 0a20 2020  pe.cancel()..   
-000083e0: 2061 7379 6e63 2064 6566 2074 6573 745f   async def test_
-000083f0: 636f 6e63 7572 7265 6e74 5f72 6563 6569  concurrent_recei
-00008400: 7665 280a 2020 2020 2020 2020 7365 6c66  ve(.        self
-00008410: 2c20 7365 7276 6572 5f73 6f63 6b3a 2073  , server_sock: s
-00008420: 6f63 6b65 742e 736f 636b 6574 2c20 736f  ocket.socket, so
-00008430: 636b 6574 5f70 6174 683a 2050 6174 680a  cket_path: Path.
-00008440: 2020 2020 2920 2d3e 204e 6f6e 653a 0a20      ) -> None:. 
-00008450: 2020 2020 2020 2061 7379 6e63 2077 6974         async wit
-00008460: 6820 6177 6169 7420 636f 6e6e 6563 745f  h await connect_
-00008470: 756e 6978 2873 6f63 6b65 745f 7061 7468  unix(socket_path
-00008480: 2920 6173 2063 6c69 656e 743a 0a20 2020  ) as client:.   
-00008490: 2020 2020 2020 2020 2061 7379 6e63 2077           async w
-000084a0: 6974 6820 6372 6561 7465 5f74 6173 6b5f  ith create_task_
-000084b0: 6772 6f75 7028 2920 6173 2074 673a 0a20  group() as tg:. 
-000084c0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000084d0: 672e 7374 6172 745f 736f 6f6e 2863 6c69  g.start_soon(cli
-000084e0: 656e 742e 7265 6365 6976 6529 0a20 2020  ent.receive).   
-000084f0: 2020 2020 2020 2020 2020 2020 2061 7761               awa
-00008500: 6974 2077 6169 745f 616c 6c5f 7461 736b  it wait_all_task
-00008510: 735f 626c 6f63 6b65 6428 290a 2020 2020  s_blocked().    
-00008520: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00008530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008540: 2020 2020 2077 6974 6820 7079 7465 7374       with pytest
-00008550: 2e72 6169 7365 7328 4275 7379 5265 736f  .raises(BusyReso
-00008560: 7572 6365 4572 726f 7229 2061 7320 6578  urceError) as ex
-00008570: 633a 0a20 2020 2020 2020 2020 2020 2020  c:.             
-00008580: 2020 2020 2020 2020 2020 2061 7761 6974             await
-00008590: 2063 6c69 656e 742e 7265 6365 6976 6528   client.receive(
-000085a0: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-000085b0: 2020 2020 2020 2065 7863 2e6d 6174 6368         exc.match
-000085c0: 2822 616c 7265 6164 7920 7265 6164 696e  ("already readin
-000085d0: 6720 6672 6f6d 2229 0a20 2020 2020 2020  g from").       
-000085e0: 2020 2020 2020 2020 2066 696e 616c 6c79           finally
-000085f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008600: 2020 2020 2020 7467 2e63 616e 6365 6c5f        tg.cancel_
-00008610: 7363 6f70 652e 6361 6e63 656c 2829 0a0a  scope.cancel()..
-00008620: 2020 2020 6173 796e 6320 6465 6620 7465      async def te
-00008630: 7374 5f63 6c6f 7365 5f64 7572 696e 675f  st_close_during_
-00008640: 7265 6365 6976 6528 0a20 2020 2020 2020  receive(.       
-00008650: 2073 656c 662c 2073 6572 7665 725f 736f   self, server_so
-00008660: 636b 3a20 736f 636b 6574 2e73 6f63 6b65  ck: socket.socke
-00008670: 742c 2073 6f63 6b65 745f 7061 7468 3a20  t, socket_path: 
-00008680: 5061 7468 0a20 2020 2029 202d 3e20 4e6f  Path.    ) -> No
-00008690: 6e65 3a0a 2020 2020 2020 2020 6173 796e  ne:.        asyn
-000086a0: 6320 6465 6620 696e 7465 7272 7570 7428  c def interrupt(
-000086b0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-000086c0: 2020 2020 2020 2061 7761 6974 2077 6169         await wai
-000086d0: 745f 616c 6c5f 7461 736b 735f 626c 6f63  t_all_tasks_bloc
-000086e0: 6b65 6428 290a 2020 2020 2020 2020 2020  ked().          
-000086f0: 2020 6177 6169 7420 7374 7265 616d 2e61    await stream.a
-00008700: 636c 6f73 6528 290a 0a20 2020 2020 2020  close()..       
-00008710: 2061 7379 6e63 2077 6974 6820 6177 6169   async with awai
-00008720: 7420 636f 6e6e 6563 745f 756e 6978 2873  t connect_unix(s
-00008730: 6f63 6b65 745f 7061 7468 2920 6173 2073  ocket_path) as s
-00008740: 7472 6561 6d3a 0a20 2020 2020 2020 2020  tream:.         
-00008750: 2020 2061 7379 6e63 2077 6974 6820 6372     async with cr
-00008760: 6561 7465 5f74 6173 6b5f 6772 6f75 7028  eate_task_group(
-00008770: 2920 6173 2074 673a 0a20 2020 2020 2020  ) as tg:.       
-00008780: 2020 2020 2020 2020 2074 672e 7374 6172           tg.star
-00008790: 745f 736f 6f6e 2869 6e74 6572 7275 7074  t_soon(interrupt
-000087a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000087b0: 2020 7769 7468 2070 7974 6573 742e 7261    with pytest.ra
-000087c0: 6973 6573 2843 6c6f 7365 6452 6573 6f75  ises(ClosedResou
-000087d0: 7263 6545 7272 6f72 293a 0a20 2020 2020  rceError):.     
-000087e0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000087f0: 7761 6974 2073 7472 6561 6d2e 7265 6365  wait stream.rece
-00008800: 6976 6528 290a 0a20 2020 2061 7379 6e63  ive()..    async
-00008810: 2064 6566 2074 6573 745f 7265 6365 6976   def test_receiv
-00008820: 655f 6166 7465 725f 636c 6f73 6528 0a20  e_after_close(. 
-00008830: 2020 2020 2020 2073 656c 662c 2073 6572         self, ser
-00008840: 7665 725f 736f 636b 3a20 736f 636b 6574  ver_sock: socket
-00008850: 2e73 6f63 6b65 742c 2073 6f63 6b65 745f  .socket, socket_
-00008860: 7061 7468 3a20 5061 7468 0a20 2020 2029  path: Path.    )
-00008870: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00008880: 2020 7374 7265 616d 203d 2061 7761 6974    stream = await
-00008890: 2063 6f6e 6e65 6374 5f75 6e69 7828 736f   connect_unix(so
-000088a0: 636b 6574 5f70 6174 6829 0a20 2020 2020  cket_path).     
-000088b0: 2020 2061 7761 6974 2073 7472 6561 6d2e     await stream.
-000088c0: 6163 6c6f 7365 2829 0a20 2020 2020 2020  aclose().       
-000088d0: 2077 6974 6820 7079 7465 7374 2e72 6169   with pytest.rai
-000088e0: 7365 7328 436c 6f73 6564 5265 736f 7572  ses(ClosedResour
-000088f0: 6365 4572 726f 7229 3a0a 2020 2020 2020  ceError):.      
-00008900: 2020 2020 2020 6177 6169 7420 7374 7265        await stre
-00008910: 616d 2e72 6563 6569 7665 2829 0a0a 2020  am.receive()..  
-00008920: 2020 6173 796e 6320 6465 6620 7465 7374    async def test
-00008930: 5f73 656e 645f 6166 7465 725f 636c 6f73  _send_after_clos
-00008940: 6528 0a20 2020 2020 2020 2073 656c 662c  e(.        self,
-00008950: 2073 6572 7665 725f 736f 636b 3a20 736f   server_sock: so
-00008960: 636b 6574 2e73 6f63 6b65 742c 2073 6f63  cket.socket, soc
-00008970: 6b65 745f 7061 7468 3a20 5061 7468 0a20  ket_path: Path. 
-00008980: 2020 2029 202d 3e20 4e6f 6e65 3a0a 2020     ) -> None:.  
-00008990: 2020 2020 2020 7374 7265 616d 203d 2061        stream = a
-000089a0: 7761 6974 2063 6f6e 6e65 6374 5f75 6e69  wait connect_uni
-000089b0: 7828 736f 636b 6574 5f70 6174 6829 0a20  x(socket_path). 
-000089c0: 2020 2020 2020 2061 7761 6974 2073 7472         await str
-000089d0: 6561 6d2e 6163 6c6f 7365 2829 0a20 2020  eam.aclose().   
-000089e0: 2020 2020 2077 6974 6820 7079 7465 7374       with pytest
-000089f0: 2e72 6169 7365 7328 436c 6f73 6564 5265  .raises(ClosedRe
-00008a00: 736f 7572 6365 4572 726f 7229 3a0a 2020  sourceError):.  
-00008a10: 2020 2020 2020 2020 2020 6177 6169 7420            await 
-00008a20: 7374 7265 616d 2e73 656e 6428 6222 666f  stream.send(b"fo
-00008a30: 6f22 290a 0a20 2020 2061 7379 6e63 2064  o")..    async d
-00008a40: 6566 2074 6573 745f 6361 6e6e 6f74 5f63  ef test_cannot_c
-00008a50: 6f6e 6e65 6374 2873 656c 662c 2073 6f63  onnect(self, soc
-00008a60: 6b65 745f 7061 7468 3a20 5061 7468 2920  ket_path: Path) 
-00008a70: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00008a80: 2077 6974 6820 7079 7465 7374 2e72 6169   with pytest.rai
-00008a90: 7365 7328 4669 6c65 4e6f 7446 6f75 6e64  ses(FileNotFound
-00008aa0: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
-00008ab0: 2020 2020 6177 6169 7420 636f 6e6e 6563      await connec
+000002b0: 6545 7272 6f72 2c0a 2020 2020 456e 644f  eError,.    EndO
+000002c0: 6653 7472 6561 6d2c 0a20 2020 2045 7665  fStream,.    Eve
+000002d0: 6e74 2c0a 2020 2020 5479 7065 6441 7474  nt,.    TypedAtt
+000002e0: 7269 6275 7465 4c6f 6f6b 7570 4572 726f  ributeLookupErro
+000002f0: 722c 0a20 2020 2063 6f6e 6e65 6374 5f74  r,.    connect_t
+00000300: 6370 2c0a 2020 2020 636f 6e6e 6563 745f  cp,.    connect_
+00000310: 756e 6978 2c0a 2020 2020 6372 6561 7465  unix,.    create
+00000320: 5f63 6f6e 6e65 6374 6564 5f75 6470 5f73  _connected_udp_s
+00000330: 6f63 6b65 742c 0a20 2020 2063 7265 6174  ocket,.    creat
+00000340: 655f 636f 6e6e 6563 7465 645f 756e 6978  e_connected_unix
+00000350: 5f64 6174 6167 7261 6d5f 736f 636b 6574  _datagram_socket
+00000360: 2c0a 2020 2020 6372 6561 7465 5f74 6173  ,.    create_tas
+00000370: 6b5f 6772 6f75 702c 0a20 2020 2063 7265  k_group,.    cre
+00000380: 6174 655f 7463 705f 6c69 7374 656e 6572  ate_tcp_listener
+00000390: 2c0a 2020 2020 6372 6561 7465 5f75 6470  ,.    create_udp
+000003a0: 5f73 6f63 6b65 742c 0a20 2020 2063 7265  _socket,.    cre
+000003b0: 6174 655f 756e 6978 5f64 6174 6167 7261  ate_unix_datagra
+000003c0: 6d5f 736f 636b 6574 2c0a 2020 2020 6372  m_socket,.    cr
+000003d0: 6561 7465 5f75 6e69 785f 6c69 7374 656e  eate_unix_listen
+000003e0: 6572 2c0a 2020 2020 6661 696c 5f61 6674  er,.    fail_aft
+000003f0: 6572 2c0a 2020 2020 6765 7461 6464 7269  er,.    getaddri
+00000400: 6e66 6f2c 0a20 2020 2067 6574 6e61 6d65  nfo,.    getname
+00000410: 696e 666f 2c0a 2020 2020 6d6f 7665 5f6f  info,.    move_o
+00000420: 6e5f 6166 7465 722c 0a20 2020 2073 6c65  n_after,.    sle
+00000430: 6570 2c0a 2020 2020 7761 6974 5f61 6c6c  ep,.    wait_all
+00000440: 5f74 6173 6b73 5f62 6c6f 636b 6564 2c0a  _tasks_blocked,.
+00000450: 290a 6672 6f6d 2061 6e79 696f 2e61 6263  ).from anyio.abc
+00000460: 2069 6d70 6f72 7420 280a 2020 2020 4950   import (.    IP
+00000470: 536f 636b 4164 6472 5479 7065 2c0a 2020  SockAddrType,.  
+00000480: 2020 4c69 7374 656e 6572 2c0a 2020 2020    Listener,.    
+00000490: 536f 636b 6574 4174 7472 6962 7574 652c  SocketAttribute,
+000004a0: 0a20 2020 2053 6f63 6b65 744c 6973 7465  .    SocketListe
+000004b0: 6e65 722c 0a20 2020 2053 6f63 6b65 7453  ner,.    SocketS
+000004c0: 7472 6561 6d2c 0a29 0a66 726f 6d20 616e  tream,.).from an
+000004d0: 7969 6f2e 7374 7265 616d 732e 7374 6170  yio.streams.stap
+000004e0: 6c65 6420 696d 706f 7274 204d 756c 7469  led import Multi
+000004f0: 4c69 7374 656e 6572 0a0a 6966 2073 7973  Listener..if sys
+00000500: 2e76 6572 7369 6f6e 5f69 6e66 6f20 3c20  .version_info < 
+00000510: 2833 2c20 3131 293a 0a20 2020 2066 726f  (3, 11):.    fro
+00000520: 6d20 6578 6365 7074 696f 6e67 726f 7570  m exceptiongroup
+00000530: 2069 6d70 6f72 7420 4578 6365 7074 696f   import Exceptio
+00000540: 6e47 726f 7570 0a0a 6672 6f6d 2074 7970  nGroup..from typ
+00000550: 696e 6720 696d 706f 7274 204c 6974 6572  ing import Liter
+00000560: 616c 0a0a 416e 7949 5041 6464 7265 7373  al..AnyIPAddress
+00000570: 4661 6d69 6c79 203d 204c 6974 6572 616c  Family = Literal
+00000580: 5b0a 2020 2020 4164 6472 6573 7346 616d  [.    AddressFam
+00000590: 696c 792e 4146 5f55 4e53 5045 432c 2041  ily.AF_UNSPEC, A
+000005a0: 6464 7265 7373 4661 6d69 6c79 2e41 465f  ddressFamily.AF_
+000005b0: 494e 4554 2c20 4164 6472 6573 7346 616d  INET, AddressFam
+000005c0: 696c 792e 4146 5f49 4e45 5436 0a5d 0a0a  ily.AF_INET6.]..
+000005d0: 7079 7465 7374 6d61 726b 203d 2070 7974  pytestmark = pyt
+000005e0: 6573 742e 6d61 726b 2e61 6e79 696f 0a0a  est.mark.anyio..
+000005f0: 2320 4966 2061 2073 6f63 6b65 7420 6361  # If a socket ca
+00000600: 6e20 6269 6e64 2074 6f20 3a3a 312c 2074  n bind to ::1, t
+00000610: 6865 2063 7572 7265 6e74 2065 6e76 6972  he current envir
+00000620: 6f6e 6d65 6e74 2068 6173 2049 5076 3620  onment has IPv6 
+00000630: 7072 6f70 6572 6c79 2063 6f6e 6669 6775  properly configu
+00000640: 7265 640a 6861 735f 6970 7636 203d 2046  red.has_ipv6 = F
+00000650: 616c 7365 0a69 6620 736f 636b 6574 2e68  alse.if socket.h
+00000660: 6173 5f69 7076 363a 0a20 2020 2074 7279  as_ipv6:.    try
+00000670: 3a0a 2020 2020 2020 2020 7320 3d20 736f  :.        s = so
+00000680: 636b 6574 2e73 6f63 6b65 7428 4164 6472  cket.socket(Addr
+00000690: 6573 7346 616d 696c 792e 4146 5f49 4e45  essFamily.AF_INE
+000006a0: 5436 290a 2020 2020 2020 2020 7472 793a  T6).        try:
+000006b0: 0a20 2020 2020 2020 2020 2020 2073 2e62  .            s.b
+000006c0: 696e 6428 2822 3a3a 3122 2c20 3029 290a  ind(("::1", 0)).
+000006d0: 2020 2020 2020 2020 6669 6e61 6c6c 793a          finally:
+000006e0: 0a20 2020 2020 2020 2020 2020 2073 2e63  .            s.c
+000006f0: 6c6f 7365 2829 0a20 2020 2020 2020 2020  lose().         
+00000700: 2020 2064 656c 2073 0a20 2020 2065 7863     del s.    exc
+00000710: 6570 7420 4f53 4572 726f 723a 0a20 2020  ept OSError:.   
+00000720: 2020 2020 2070 6173 730a 2020 2020 656c       pass.    el
+00000730: 7365 3a0a 2020 2020 2020 2020 6861 735f  se:.        has_
+00000740: 6970 7636 203d 2054 7275 650a 0a73 6b69  ipv6 = True..ski
+00000750: 705f 6970 7636 5f6d 6172 6b20 3d20 7079  p_ipv6_mark = py
+00000760: 7465 7374 2e6d 6172 6b2e 736b 6970 6966  test.mark.skipif
+00000770: 286e 6f74 2068 6173 5f69 7076 362c 2072  (not has_ipv6, r
+00000780: 6561 736f 6e3d 2249 5076 3620 6973 206e  eason="IPv6 is n
+00000790: 6f74 2061 7661 696c 6162 6c65 2229 0a0a  ot available")..
+000007a0: 0a40 7079 7465 7374 2e66 6978 7475 7265  .@pytest.fixture
+000007b0: 0a64 6566 2066 616b 655f 6c6f 6361 6c68  .def fake_localh
+000007c0: 6f73 745f 646e 7328 6d6f 6e6b 6579 7061  ost_dns(monkeypa
+000007d0: 7463 683a 204d 6f6e 6b65 7950 6174 6368  tch: MonkeyPatch
+000007e0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2064  ) -> None:.    d
+000007f0: 6566 2066 616b 655f 6765 7461 6464 7269  ef fake_getaddri
+00000800: 6e66 6f28 2a61 7267 733a 2041 6e79 2c20  nfo(*args: Any, 
+00000810: 2a2a 6b77 6172 6773 3a20 416e 7929 202d  **kwargs: Any) -
+00000820: 3e20 6f62 6a65 6374 3a0a 2020 2020 2020  > object:.      
+00000830: 2020 2320 4d61 6b65 2069 7420 7265 7475    # Make it retu
+00000840: 726e 2049 5076 3420 6164 6472 6573 7365  rn IPv4 addresse
+00000850: 7320 6669 7273 7420 736f 2077 6520 6361  s first so we ca
+00000860: 6e20 7465 7374 2074 6865 2049 5076 3620  n test the IPv6 
+00000870: 7072 6566 6572 656e 6365 0a20 2020 2020  preference.     
+00000880: 2020 2072 6573 756c 7473 203d 2072 6561     results = rea
+00000890: 6c5f 6765 7461 6464 7269 6e66 6f28 2a61  l_getaddrinfo(*a
+000008a0: 7267 732c 202a 2a6b 7761 7267 7329 0a20  rgs, **kwargs). 
+000008b0: 2020 2020 2020 2072 6574 7572 6e20 736f         return so
+000008c0: 7274 6564 2872 6573 756c 7473 2c20 6b65  rted(results, ke
+000008d0: 793d 6c61 6d62 6461 2069 7465 6d3a 2069  y=lambda item: i
+000008e0: 7465 6d5b 305d 290a 0a20 2020 2072 6561  tem[0])..    rea
+000008f0: 6c5f 6765 7461 6464 7269 6e66 6f20 3d20  l_getaddrinfo = 
+00000900: 736f 636b 6574 2e67 6574 6164 6472 696e  socket.getaddrin
+00000910: 666f 0a20 2020 206d 6f6e 6b65 7970 6174  fo.    monkeypat
+00000920: 6368 2e73 6574 6174 7472 2822 736f 636b  ch.setattr("sock
+00000930: 6574 2e67 6574 6164 6472 696e 666f 222c  et.getaddrinfo",
+00000940: 2066 616b 655f 6765 7461 6464 7269 6e66   fake_getaddrinf
+00000950: 6f29 0a0a 0a40 7079 7465 7374 2e66 6978  o)...@pytest.fix
+00000960: 7475 7265 280a 2020 2020 7061 7261 6d73  ture(.    params
+00000970: 3d5b 0a20 2020 2020 2020 2070 7974 6573  =[.        pytes
+00000980: 742e 7061 7261 6d28 4164 6472 6573 7346  t.param(AddressF
+00000990: 616d 696c 792e 4146 5f49 4e45 542c 2069  amily.AF_INET, i
+000009a0: 643d 2269 7076 3422 292c 0a20 2020 2020  d="ipv4"),.     
+000009b0: 2020 2070 7974 6573 742e 7061 7261 6d28     pytest.param(
+000009c0: 4164 6472 6573 7346 616d 696c 792e 4146  AddressFamily.AF
+000009d0: 5f49 4e45 5436 2c20 6964 3d22 6970 7636  _INET6, id="ipv6
+000009e0: 222c 206d 6172 6b73 3d5b 736b 6970 5f69  ", marks=[skip_i
+000009f0: 7076 365f 6d61 726b 5d29 2c0a 2020 2020  pv6_mark]),.    
+00000a00: 5d0a 290a 6465 6620 6661 6d69 6c79 2872  ].).def family(r
+00000a10: 6571 7565 7374 3a20 5375 6252 6571 7565  equest: SubReque
+00000a20: 7374 2920 2d3e 2041 6e79 4950 4164 6472  st) -> AnyIPAddr
+00000a30: 6573 7346 616d 696c 793a 0a20 2020 2072  essFamily:.    r
+00000a40: 6574 7572 6e20 7265 7175 6573 742e 7061  eturn request.pa
+00000a50: 7261 6d0a 0a0a 4070 7974 6573 742e 6669  ram...@pytest.fi
+00000a60: 7874 7572 650a 6465 6620 6368 6563 6b5f  xture.def check_
+00000a70: 6173 796e 6369 6f5f 6275 6728 616e 7969  asyncio_bug(anyi
+00000a80: 6f5f 6261 636b 656e 645f 6e61 6d65 3a20  o_backend_name: 
+00000a90: 7374 722c 2066 616d 696c 793a 2041 6e79  str, family: Any
+00000aa0: 4950 4164 6472 6573 7346 616d 696c 7929  IPAddressFamily)
+00000ab0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 6966   -> None:.    if
+00000ac0: 2028 0a20 2020 2020 2020 2061 6e79 696f   (.        anyio
+00000ad0: 5f62 6163 6b65 6e64 5f6e 616d 6520 3d3d  _backend_name ==
+00000ae0: 2022 6173 796e 6369 6f22 0a20 2020 2020   "asyncio".     
+00000af0: 2020 2061 6e64 2073 7973 2e70 6c61 7466     and sys.platf
+00000b00: 6f72 6d20 3d3d 2022 7769 6e33 3222 0a20  orm == "win32". 
+00000b10: 2020 2020 2020 2061 6e64 2066 616d 696c         and famil
+00000b20: 7920 3d3d 2041 6464 7265 7373 4661 6d69  y == AddressFami
+00000b30: 6c79 2e41 465f 494e 4554 360a 2020 2020  ly.AF_INET6.    
+00000b40: 293a 0a20 2020 2020 2020 2069 6d70 6f72  ):.        impor
+00000b50: 7420 6173 796e 6369 6f0a 0a20 2020 2020  t asyncio..     
+00000b60: 2020 2070 6f6c 6963 7920 3d20 6173 796e     policy = asyn
+00000b70: 6369 6f2e 6765 745f 6576 656e 745f 6c6f  cio.get_event_lo
+00000b80: 6f70 5f70 6f6c 6963 7928 290a 2020 2020  op_policy().    
+00000b90: 2020 2020 6966 2070 6f6c 6963 792e 5f5f      if policy.__
+00000ba0: 636c 6173 735f 5f2e 5f5f 6e61 6d65 5f5f  class__.__name__
+00000bb0: 203d 3d20 2257 696e 646f 7773 5072 6f61   == "WindowsProa
+00000bc0: 6374 6f72 4576 656e 744c 6f6f 7050 6f6c  ctorEventLoopPol
+00000bd0: 6963 7922 3a0a 2020 2020 2020 2020 2020  icy":.          
+00000be0: 2020 7079 7465 7374 2e73 6b69 7028 2244    pytest.skip("D
+00000bf0: 6f65 7320 6e6f 7420 776f 726b 2064 7565  oes not work due
+00000c00: 2074 6f20 6120 6b6e 6f77 6e20 6275 6720   to a known bug 
+00000c10: 2833 3931 3438 2922 290a 0a0a 5f54 203d  (39148)")..._T =
+00000c20: 2054 7970 6556 6172 2822 5f54 2229 0a0a   TypeVar("_T")..
+00000c30: 0a64 6566 205f 6964 656e 7469 7479 2876  .def _identity(v
+00000c40: 3a20 5f54 2920 2d3e 205f 543a 0a20 2020  : _T) -> _T:.   
+00000c50: 2072 6574 7572 6e20 760a 0a0a 2320 205f   return v...#  _
+00000c60: 5072 6f61 6374 6f72 4261 7365 5069 7065  ProactorBasePipe
+00000c70: 5472 616e 7370 6f72 742e 6162 6f72 7428  Transport.abort(
+00000c80: 2920 6166 7465 7220 5f50 726f 6163 746f  ) after _Proacto
+00000c90: 7242 6173 6550 6970 6554 7261 6e73 706f  rBasePipeTranspo
+00000ca0: 7274 2e63 6c6f 7365 2829 0a23 2064 6f65  rt.close().# doe
+00000cb0: 7320 6e6f 7420 6361 6e63 656c 2077 7269  s not cancel wri
+00000cc0: 7465 733a 2068 7474 7073 3a2f 2f62 7567  tes: https://bug
+00000cd0: 732e 7079 7468 6f6e 2e6f 7267 2f69 7373  s.python.org/iss
+00000ce0: 7565 3434 3432 380a 5f69 676e 6f72 655f  ue44428._ignore_
+00000cf0: 7769 6e33 325f 7265 736f 7572 6365 5f77  win32_resource_w
+00000d00: 6172 6e69 6e67 7320 3d20 280a 2020 2020  arnings = (.    
+00000d10: 7079 7465 7374 2e6d 6172 6b2e 6669 6c74  pytest.mark.filt
+00000d20: 6572 7761 726e 696e 6773 280a 2020 2020  erwarnings(.    
+00000d30: 2020 2020 2269 676e 6f72 653a 756e 636c      "ignore:uncl
+00000d40: 6f73 6564 203c 736f 636b 6574 2e73 6f63  osed <socket.soc
+00000d50: 6b65 743a 5265 736f 7572 6365 5761 726e  ket:ResourceWarn
+00000d60: 696e 6722 2c0a 2020 2020 2020 2020 2269  ing",.        "i
+00000d70: 676e 6f72 653a 756e 636c 6f73 6564 2074  gnore:unclosed t
+00000d80: 7261 6e73 706f 7274 203c 5f50 726f 6163  ransport <_Proac
+00000d90: 746f 7253 6f63 6b65 7454 7261 6e73 706f  torSocketTranspo
+00000da0: 7274 2063 6c6f 7369 6e67 3a52 6573 6f75  rt closing:Resou
+00000db0: 7263 6557 6172 6e69 6e67 222c 0a20 2020  rceWarning",.   
+00000dc0: 2029 0a20 2020 2069 6620 7379 732e 706c   ).    if sys.pl
+00000dd0: 6174 666f 726d 203d 3d20 2277 696e 3332  atform == "win32
+00000de0: 220a 2020 2020 656c 7365 205f 6964 656e  ".    else _iden
+00000df0: 7469 7479 0a29 0a0a 0a40 5f69 676e 6f72  tity.)...@_ignor
+00000e00: 655f 7769 6e33 325f 7265 736f 7572 6365  e_win32_resource
+00000e10: 5f77 6172 6e69 6e67 7320 2023 2074 7970  _warnings  # typ
+00000e20: 653a 2069 676e 6f72 655b 6f70 6572 6174  e: ignore[operat
+00000e30: 6f72 5d0a 636c 6173 7320 5465 7374 5443  or].class TestTC
+00000e40: 5053 7472 6561 6d3a 0a20 2020 2040 7079  PStream:.    @py
+00000e50: 7465 7374 2e66 6978 7475 7265 0a20 2020  test.fixture.   
+00000e60: 2064 6566 2073 6572 7665 725f 736f 636b   def server_sock
+00000e70: 2873 656c 662c 2066 616d 696c 793a 2041  (self, family: A
+00000e80: 6e79 4950 4164 6472 6573 7346 616d 696c  nyIPAddressFamil
+00000e90: 7929 202d 3e20 4974 6572 6174 6f72 5b73  y) -> Iterator[s
+00000ea0: 6f63 6b65 742e 736f 636b 6574 5d3a 0a20  ocket.socket]:. 
+00000eb0: 2020 2020 2020 2073 6f63 6b20 3d20 736f         sock = so
+00000ec0: 636b 6574 2e73 6f63 6b65 7428 6661 6d69  cket.socket(fami
+00000ed0: 6c79 2c20 736f 636b 6574 2e53 4f43 4b5f  ly, socket.SOCK_
+00000ee0: 5354 5245 414d 290a 2020 2020 2020 2020  STREAM).        
+00000ef0: 736f 636b 2e73 6574 7469 6d65 6f75 7428  sock.settimeout(
+00000f00: 3129 0a20 2020 2020 2020 2073 6f63 6b2e  1).        sock.
+00000f10: 6269 6e64 2828 226c 6f63 616c 686f 7374  bind(("localhost
+00000f20: 222c 2030 2929 0a20 2020 2020 2020 2073  ", 0)).        s
+00000f30: 6f63 6b2e 6c69 7374 656e 2829 0a20 2020  ock.listen().   
+00000f40: 2020 2020 2079 6965 6c64 2073 6f63 6b0a       yield sock.
+00000f50: 2020 2020 2020 2020 736f 636b 2e63 6c6f          sock.clo
+00000f60: 7365 2829 0a0a 2020 2020 4070 7974 6573  se()..    @pytes
+00000f70: 742e 6669 7874 7572 650a 2020 2020 6465  t.fixture.    de
+00000f80: 6620 7365 7276 6572 5f61 6464 7228 7365  f server_addr(se
+00000f90: 6c66 2c20 7365 7276 6572 5f73 6f63 6b3a  lf, server_sock:
+00000fa0: 2073 6f63 6b65 742e 736f 636b 6574 2920   socket.socket) 
+00000fb0: 2d3e 2074 7570 6c65 5b73 7472 2c20 696e  -> tuple[str, in
+00000fc0: 745d 3a0a 2020 2020 2020 2020 7265 7475  t]:.        retu
+00000fd0: 726e 2073 6572 7665 725f 736f 636b 2e67  rn server_sock.g
+00000fe0: 6574 736f 636b 6e61 6d65 2829 5b3a 325d  etsockname()[:2]
+00000ff0: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+00001000: 7465 7374 5f65 7874 7261 5f61 7474 7269  test_extra_attri
+00001010: 6275 7465 7328 0a20 2020 2020 2020 2073  butes(.        s
+00001020: 656c 662c 0a20 2020 2020 2020 2073 6572  elf,.        ser
+00001030: 7665 725f 736f 636b 3a20 736f 636b 6574  ver_sock: socket
+00001040: 2e73 6f63 6b65 742c 0a20 2020 2020 2020  .socket,.       
+00001050: 2073 6572 7665 725f 6164 6472 3a20 7475   server_addr: tu
+00001060: 706c 655b 7374 722c 2069 6e74 5d2c 0a20  ple[str, int],. 
+00001070: 2020 2020 2020 2066 616d 696c 793a 2041         family: A
+00001080: 6e79 4950 4164 6472 6573 7346 616d 696c  nyIPAddressFamil
+00001090: 792c 0a20 2020 2029 202d 3e20 4e6f 6e65  y,.    ) -> None
+000010a0: 3a0a 2020 2020 2020 2020 6173 796e 6320  :.        async 
+000010b0: 7769 7468 2061 7761 6974 2063 6f6e 6e65  with await conne
+000010c0: 6374 5f74 6370 282a 7365 7276 6572 5f61  ct_tcp(*server_a
+000010d0: 6464 7229 2061 7320 7374 7265 616d 3a0a  ddr) as stream:.
+000010e0: 2020 2020 2020 2020 2020 2020 7261 775f              raw_
+000010f0: 736f 636b 6574 203d 2073 7472 6561 6d2e  socket = stream.
+00001100: 6578 7472 6128 536f 636b 6574 4174 7472  extra(SocketAttr
+00001110: 6962 7574 652e 7261 775f 736f 636b 6574  ibute.raw_socket
+00001120: 290a 2020 2020 2020 2020 2020 2020 6173  ).            as
+00001130: 7365 7274 2073 7472 6561 6d2e 6578 7472  sert stream.extr
+00001140: 6128 536f 636b 6574 4174 7472 6962 7574  a(SocketAttribut
+00001150: 652e 6661 6d69 6c79 2920 3d3d 2066 616d  e.family) == fam
+00001160: 696c 790a 2020 2020 2020 2020 2020 2020  ily.            
+00001170: 6173 7365 7274 2028 0a20 2020 2020 2020  assert (.       
+00001180: 2020 2020 2020 2020 2073 7472 6561 6d2e           stream.
+00001190: 6578 7472 6128 536f 636b 6574 4174 7472  extra(SocketAttr
+000011a0: 6962 7574 652e 6c6f 6361 6c5f 6164 6472  ibute.local_addr
+000011b0: 6573 7329 0a20 2020 2020 2020 2020 2020  ess).           
+000011c0: 2020 2020 203d 3d20 7261 775f 736f 636b       == raw_sock
+000011d0: 6574 2e67 6574 736f 636b 6e61 6d65 2829  et.getsockname()
+000011e0: 5b3a 325d 0a20 2020 2020 2020 2020 2020  [:2].           
+000011f0: 2029 0a20 2020 2020 2020 2020 2020 2061   ).            a
+00001200: 7373 6572 7420 280a 2020 2020 2020 2020  ssert (.        
+00001210: 2020 2020 2020 2020 7374 7265 616d 2e65          stream.e
+00001220: 7874 7261 2853 6f63 6b65 7441 7474 7269  xtra(SocketAttri
+00001230: 6275 7465 2e6c 6f63 616c 5f70 6f72 7429  bute.local_port)
+00001240: 203d 3d20 7261 775f 736f 636b 6574 2e67   == raw_socket.g
+00001250: 6574 736f 636b 6e61 6d65 2829 5b31 5d0a  etsockname()[1].
+00001260: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00001270: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+00001280: 2073 7472 6561 6d2e 6578 7472 6128 536f   stream.extra(So
+00001290: 636b 6574 4174 7472 6962 7574 652e 7265  cketAttribute.re
+000012a0: 6d6f 7465 5f61 6464 7265 7373 2920 3d3d  mote_address) ==
+000012b0: 2073 6572 7665 725f 6164 6472 0a20 2020   server_addr.   
+000012c0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+000012d0: 7374 7265 616d 2e65 7874 7261 2853 6f63  stream.extra(Soc
+000012e0: 6b65 7441 7474 7269 6275 7465 2e72 656d  ketAttribute.rem
+000012f0: 6f74 655f 706f 7274 2920 3d3d 2073 6572  ote_port) == ser
+00001300: 7665 725f 6164 6472 5b31 5d0a 0a20 2020  ver_addr[1]..   
+00001310: 2061 7379 6e63 2064 6566 2074 6573 745f   async def test_
+00001320: 7365 6e64 5f72 6563 6569 7665 280a 2020  send_receive(.  
+00001330: 2020 2020 2020 7365 6c66 2c20 7365 7276        self, serv
+00001340: 6572 5f73 6f63 6b3a 2073 6f63 6b65 742e  er_sock: socket.
+00001350: 736f 636b 6574 2c20 7365 7276 6572 5f61  socket, server_a
+00001360: 6464 723a 2074 7570 6c65 5b73 7472 2c20  ddr: tuple[str, 
+00001370: 696e 745d 0a20 2020 2029 202d 3e20 4e6f  int].    ) -> No
+00001380: 6e65 3a0a 2020 2020 2020 2020 6173 796e  ne:.        asyn
+00001390: 6320 7769 7468 2061 7761 6974 2063 6f6e  c with await con
+000013a0: 6e65 6374 5f74 6370 282a 7365 7276 6572  nect_tcp(*server
+000013b0: 5f61 6464 7229 2061 7320 7374 7265 616d  _addr) as stream
+000013c0: 3a0a 2020 2020 2020 2020 2020 2020 636c  :.            cl
+000013d0: 6965 6e74 2c20 5f20 3d20 7365 7276 6572  ient, _ = server
+000013e0: 5f73 6f63 6b2e 6163 6365 7074 2829 0a20  _sock.accept(). 
+000013f0: 2020 2020 2020 2020 2020 2061 7761 6974             await
+00001400: 2073 7472 6561 6d2e 7365 6e64 2862 2262   stream.send(b"b
+00001410: 6c61 6822 290a 2020 2020 2020 2020 2020  lah").          
+00001420: 2020 7265 7175 6573 7420 3d20 636c 6965    request = clie
+00001430: 6e74 2e72 6563 7628 3130 3029 0a20 2020  nt.recv(100).   
+00001440: 2020 2020 2020 2020 2063 6c69 656e 742e           client.
+00001450: 7365 6e64 616c 6c28 7265 7175 6573 745b  sendall(request[
+00001460: 3a3a 2d31 5d29 0a20 2020 2020 2020 2020  ::-1]).         
+00001470: 2020 2072 6573 706f 6e73 6520 3d20 6177     response = aw
+00001480: 6169 7420 7374 7265 616d 2e72 6563 6569  ait stream.recei
+00001490: 7665 2829 0a20 2020 2020 2020 2020 2020  ve().           
+000014a0: 2063 6c69 656e 742e 636c 6f73 6528 290a   client.close().
+000014b0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+000014c0: 7265 7370 6f6e 7365 203d 3d20 6222 6861  response == b"ha
+000014d0: 6c62 220a 0a20 2020 2061 7379 6e63 2064  lb"..    async d
+000014e0: 6566 2074 6573 745f 7365 6e64 5f6c 6172  ef test_send_lar
+000014f0: 6765 5f62 7566 6665 7228 0a20 2020 2020  ge_buffer(.     
+00001500: 2020 2073 656c 662c 2073 6572 7665 725f     self, server_
+00001510: 736f 636b 3a20 736f 636b 6574 2e73 6f63  sock: socket.soc
+00001520: 6b65 742c 2073 6572 7665 725f 6164 6472  ket, server_addr
+00001530: 3a20 7475 706c 655b 7374 722c 2069 6e74  : tuple[str, int
+00001540: 5d0a 2020 2020 2920 2d3e 204e 6f6e 653a  ].    ) -> None:
+00001550: 0a20 2020 2020 2020 2064 6566 2073 6572  .        def ser
+00001560: 7665 2829 202d 3e20 4e6f 6e65 3a0a 2020  ve() -> None:.  
+00001570: 2020 2020 2020 2020 2020 636c 6965 6e74            client
+00001580: 2c20 5f20 3d20 7365 7276 6572 5f73 6f63  , _ = server_soc
+00001590: 6b2e 6163 6365 7074 2829 0a20 2020 2020  k.accept().     
+000015a0: 2020 2020 2020 2063 6c69 656e 742e 7365         client.se
+000015b0: 6e64 616c 6c28 6275 6666 6572 290a 2020  ndall(buffer).  
+000015c0: 2020 2020 2020 2020 2020 636c 6965 6e74            client
+000015d0: 2e63 6c6f 7365 2829 0a0a 2020 2020 2020  .close()..      
+000015e0: 2020 6275 6666 6572 203d 2028 0a20 2020    buffer = (.   
+000015f0: 2020 2020 2020 2020 2062 225c 7866 6622           b"\xff"
+00001600: 202a 2031 3032 3420 2a20 3130 3234 0a20   * 1024 * 1024. 
+00001610: 2020 2020 2020 2029 2020 2320 7368 6f75         )  # shou
+00001620: 6c64 2065 7863 6565 6420 7468 6520 6d61  ld exceed the ma
+00001630: 7869 6d75 6d20 6b65 726e 656c 2073 656e  ximum kernel sen
+00001640: 6420 6275 6666 6572 2073 697a 650a 2020  d buffer size.  
+00001650: 2020 2020 2020 6173 796e 6320 7769 7468        async with
+00001660: 2061 7761 6974 2063 6f6e 6e65 6374 5f74   await connect_t
+00001670: 6370 282a 7365 7276 6572 5f61 6464 7229  cp(*server_addr)
+00001680: 2061 7320 7374 7265 616d 3a0a 2020 2020   as stream:.    
+00001690: 2020 2020 2020 2020 7468 7265 6164 203d          thread =
+000016a0: 2054 6872 6561 6428 7461 7267 6574 3d73   Thread(target=s
+000016b0: 6572 7665 2c20 6461 656d 6f6e 3d54 7275  erve, daemon=Tru
+000016c0: 6529 0a20 2020 2020 2020 2020 2020 2074  e).            t
+000016d0: 6872 6561 642e 7374 6172 7428 290a 2020  hread.start().  
+000016e0: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
+000016f0: 7365 203d 2062 2222 0a20 2020 2020 2020  se = b"".       
+00001700: 2020 2020 2077 6869 6c65 206c 656e 2872       while len(r
+00001710: 6573 706f 6e73 6529 203c 206c 656e 2862  esponse) < len(b
+00001720: 7566 6665 7229 3a0a 2020 2020 2020 2020  uffer):.        
+00001730: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+00001740: 202b 3d20 6177 6169 7420 7374 7265 616d   += await stream
+00001750: 2e72 6563 6569 7665 2829 0a0a 2020 2020  .receive()..    
+00001760: 2020 2020 7468 7265 6164 2e6a 6f69 6e28      thread.join(
+00001770: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
+00001780: 2072 6573 706f 6e73 6520 3d3d 2062 7566   response == buf
+00001790: 6665 720a 0a20 2020 2061 7379 6e63 2064  fer..    async d
+000017a0: 6566 2074 6573 745f 7365 6e64 5f65 6f66  ef test_send_eof
+000017b0: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
+000017c0: 7365 7276 6572 5f73 6f63 6b3a 2073 6f63  server_sock: soc
+000017d0: 6b65 742e 736f 636b 6574 2c20 7365 7276  ket.socket, serv
+000017e0: 6572 5f61 6464 723a 2074 7570 6c65 5b73  er_addr: tuple[s
+000017f0: 7472 2c20 696e 745d 0a20 2020 2029 202d  tr, int].    ) -
+00001800: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00001810: 6465 6620 7365 7276 6528 2920 2d3e 204e  def serve() -> N
+00001820: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00001830: 2063 6c69 656e 742c 205f 203d 2073 6572   client, _ = ser
+00001840: 7665 725f 736f 636b 2e61 6363 6570 7428  ver_sock.accept(
+00001850: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00001860: 7175 6573 7420 3d20 6222 220a 2020 2020  quest = b"".    
+00001870: 2020 2020 2020 2020 7768 696c 6520 5472          while Tr
+00001880: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
+00001890: 2020 2020 6461 7461 203d 2063 6c69 656e      data = clien
+000018a0: 742e 7265 6376 2831 3030 290a 2020 2020  t.recv(100).    
+000018b0: 2020 2020 2020 2020 2020 2020 7265 7175              requ
+000018c0: 6573 7420 2b3d 2064 6174 610a 2020 2020  est += data.    
+000018d0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+000018e0: 6f74 2064 6174 613a 0a20 2020 2020 2020  ot data:.       
+000018f0: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+00001900: 616b 0a0a 2020 2020 2020 2020 2020 2020  ak..            
+00001910: 636c 6965 6e74 2e73 656e 6461 6c6c 2872  client.sendall(r
+00001920: 6571 7565 7374 5b3a 3a2d 315d 290a 2020  equest[::-1]).  
+00001930: 2020 2020 2020 2020 2020 636c 6965 6e74            client
+00001940: 2e63 6c6f 7365 2829 0a0a 2020 2020 2020  .close()..      
+00001950: 2020 6173 796e 6320 7769 7468 2061 7761    async with awa
+00001960: 6974 2063 6f6e 6e65 6374 5f74 6370 282a  it connect_tcp(*
+00001970: 7365 7276 6572 5f61 6464 7229 2061 7320  server_addr) as 
+00001980: 7374 7265 616d 3a0a 2020 2020 2020 2020  stream:.        
+00001990: 2020 2020 7468 7265 6164 203d 2054 6872      thread = Thr
+000019a0: 6561 6428 7461 7267 6574 3d73 6572 7665  ead(target=serve
+000019b0: 2c20 6461 656d 6f6e 3d54 7275 6529 0a20  , daemon=True). 
+000019c0: 2020 2020 2020 2020 2020 2074 6872 6561             threa
+000019d0: 642e 7374 6172 7428 290a 2020 2020 2020  d.start().      
+000019e0: 2020 2020 2020 6177 6169 7420 7374 7265        await stre
+000019f0: 616d 2e73 656e 6428 6222 6865 6c6c 6f2c  am.send(b"hello,
+00001a00: 2022 290a 2020 2020 2020 2020 2020 2020   ").            
+00001a10: 6177 6169 7420 7374 7265 616d 2e73 656e  await stream.sen
+00001a20: 6428 6222 776f 726c 645c 6e22 290a 2020  d(b"world\n").  
+00001a30: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+00001a40: 7374 7265 616d 2e73 656e 645f 656f 6628  stream.send_eof(
+00001a50: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00001a60: 7370 6f6e 7365 203d 2061 7761 6974 2073  sponse = await s
+00001a70: 7472 6561 6d2e 7265 6365 6976 6528 290a  tream.receive().
+00001a80: 0a20 2020 2020 2020 2074 6872 6561 642e  .        thread.
+00001a90: 6a6f 696e 2829 0a20 2020 2020 2020 2061  join().        a
+00001aa0: 7373 6572 7420 7265 7370 6f6e 7365 203d  ssert response =
+00001ab0: 3d20 6222 5c6e 646c 726f 7720 2c6f 6c6c  = b"\ndlrow ,oll
+00001ac0: 6568 220a 0a20 2020 2061 7379 6e63 2064  eh"..    async d
+00001ad0: 6566 2074 6573 745f 6974 6572 6174 6528  ef test_iterate(
+00001ae0: 0a20 2020 2020 2020 2073 656c 662c 2073  .        self, s
+00001af0: 6572 7665 725f 736f 636b 3a20 736f 636b  erver_sock: sock
+00001b00: 6574 2e73 6f63 6b65 742c 2073 6572 7665  et.socket, serve
+00001b10: 725f 6164 6472 3a20 7475 706c 655b 7374  r_addr: tuple[st
+00001b20: 722c 2069 6e74 5d0a 2020 2020 2920 2d3e  r, int].    ) ->
+00001b30: 204e 6f6e 653a 0a20 2020 2020 2020 2064   None:.        d
+00001b40: 6566 2073 6572 7665 2829 202d 3e20 4e6f  ef serve() -> No
+00001b50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00001b60: 636c 6965 6e74 2c20 5f20 3d20 7365 7276  client, _ = serv
+00001b70: 6572 5f73 6f63 6b2e 6163 6365 7074 2829  er_sock.accept()
+00001b80: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
+00001b90: 656e 742e 7365 6e64 616c 6c28 6222 626c  ent.sendall(b"bl
+00001ba0: 2229 0a20 2020 2020 2020 2020 2020 2065  ").            e
+00001bb0: 7665 6e74 2e77 6169 7428 3129 0a20 2020  vent.wait(1).   
+00001bc0: 2020 2020 2020 2020 2063 6c69 656e 742e           client.
+00001bd0: 7365 6e64 616c 6c28 6222 6168 2229 0a20  sendall(b"ah"). 
+00001be0: 2020 2020 2020 2020 2020 2063 6c69 656e             clien
+00001bf0: 742e 636c 6f73 6528 290a 0a20 2020 2020  t.close()..     
+00001c00: 2020 2065 7665 6e74 203d 2074 6872 6561     event = threa
+00001c10: 6469 6e67 2e45 7665 6e74 2829 0a20 2020  ding.Event().   
+00001c20: 2020 2020 2074 6872 6561 6420 3d20 5468       thread = Th
+00001c30: 7265 6164 2874 6172 6765 743d 7365 7276  read(target=serv
+00001c40: 652c 2064 6165 6d6f 6e3d 5472 7565 290a  e, daemon=True).
+00001c50: 2020 2020 2020 2020 7468 7265 6164 2e73          thread.s
+00001c60: 7461 7274 2829 0a20 2020 2020 2020 2063  tart().        c
+00001c70: 6875 6e6b 7320 3d20 5b5d 0a20 2020 2020  hunks = [].     
+00001c80: 2020 2061 7379 6e63 2077 6974 6820 6177     async with aw
+00001c90: 6169 7420 636f 6e6e 6563 745f 7463 7028  ait connect_tcp(
+00001ca0: 2a73 6572 7665 725f 6164 6472 2920 6173  *server_addr) as
+00001cb0: 2073 7472 6561 6d3a 0a20 2020 2020 2020   stream:.       
+00001cc0: 2020 2020 2061 7379 6e63 2066 6f72 2063       async for c
+00001cd0: 6875 6e6b 2069 6e20 7374 7265 616d 3a0a  hunk in stream:.
+00001ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cf0: 6368 756e 6b73 2e61 7070 656e 6428 6368  chunks.append(ch
+00001d00: 756e 6b29 0a20 2020 2020 2020 2020 2020  unk).           
+00001d10: 2020 2020 2065 7665 6e74 2e73 6574 2829       event.set()
+00001d20: 0a0a 2020 2020 2020 2020 7468 7265 6164  ..        thread
+00001d30: 2e6a 6f69 6e28 290a 2020 2020 2020 2020  .join().        
+00001d40: 6173 7365 7274 2063 6875 6e6b 7320 3d3d  assert chunks ==
+00001d50: 205b 6222 626c 222c 2062 2261 6822 5d0a   [b"bl", b"ah"].
+00001d60: 0a20 2020 2061 7379 6e63 2064 6566 2074  .    async def t
+00001d70: 6573 745f 736f 636b 6574 5f6f 7074 696f  est_socket_optio
+00001d80: 6e73 280a 2020 2020 2020 2020 7365 6c66  ns(.        self
+00001d90: 2c20 6661 6d69 6c79 3a20 416e 7949 5041  , family: AnyIPA
+00001da0: 6464 7265 7373 4661 6d69 6c79 2c20 7365  ddressFamily, se
+00001db0: 7276 6572 5f61 6464 723a 2074 7570 6c65  rver_addr: tuple
+00001dc0: 5b73 7472 2c20 696e 745d 0a20 2020 2029  [str, int].    )
+00001dd0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00001de0: 2020 6173 796e 6320 7769 7468 2061 7761    async with awa
+00001df0: 6974 2063 6f6e 6e65 6374 5f74 6370 282a  it connect_tcp(*
+00001e00: 7365 7276 6572 5f61 6464 7229 2061 7320  server_addr) as 
+00001e10: 7374 7265 616d 3a0a 2020 2020 2020 2020  stream:.        
+00001e20: 2020 2020 7261 775f 736f 636b 6574 203d      raw_socket =
+00001e30: 2073 7472 6561 6d2e 6578 7472 6128 536f   stream.extra(So
+00001e40: 636b 6574 4174 7472 6962 7574 652e 7261  cketAttribute.ra
+00001e50: 775f 736f 636b 6574 290a 2020 2020 2020  w_socket).      
+00001e60: 2020 2020 2020 6173 7365 7274 2072 6177        assert raw
+00001e70: 5f73 6f63 6b65 742e 6765 7473 6f63 6b6f  _socket.getsocko
+00001e80: 7074 2873 6f63 6b65 742e 4950 5052 4f54  pt(socket.IPPROT
+00001e90: 4f5f 5443 502c 2073 6f63 6b65 742e 5443  O_TCP, socket.TC
+00001ea0: 505f 4e4f 4445 4c41 5929 2021 3d20 300a  P_NODELAY) != 0.
+00001eb0: 0a20 2020 2040 736b 6970 5f69 7076 365f  .    @skip_ipv6_
+00001ec0: 6d61 726b 0a20 2020 2040 7079 7465 7374  mark.    @pytest
+00001ed0: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
+00001ee0: 6528 0a20 2020 2020 2020 2022 6c6f 6361  e(.        "loca
+00001ef0: 6c5f 6164 6472 2c20 6578 7065 6374 6564  l_addr, expected
+00001f00: 5f63 6c69 656e 745f 6164 6472 222c 0a20  _client_addr",. 
+00001f10: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+00001f20: 2020 2020 2070 7974 6573 742e 7061 7261       pytest.para
+00001f30: 6d28 2222 2c20 223a 3a31 222c 2069 643d  m("", "::1", id=
+00001f40: 2264 7561 6c73 7461 636b 2229 2c0a 2020  "dualstack"),.  
+00001f50: 2020 2020 2020 2020 2020 7079 7465 7374            pytest
+00001f60: 2e70 6172 616d 2822 3132 372e 302e 302e  .param("127.0.0.
+00001f70: 3122 2c20 2231 3237 2e30 2e30 2e31 222c  1", "127.0.0.1",
+00001f80: 2069 643d 2269 7076 3422 292c 0a20 2020   id="ipv4"),.   
+00001f90: 2020 2020 2020 2020 2070 7974 6573 742e           pytest.
+00001fa0: 7061 7261 6d28 223a 3a31 222c 2022 3a3a  param("::1", "::
+00001fb0: 3122 2c20 6964 3d22 6970 7636 2229 2c0a  1", id="ipv6"),.
+00001fc0: 2020 2020 2020 2020 5d2c 0a20 2020 2029          ],.    )
+00001fd0: 0a20 2020 2061 7379 6e63 2064 6566 2074  .    async def t
+00001fe0: 6573 745f 6861 7070 795f 6579 6562 616c  est_happy_eyebal
+00001ff0: 6c73 280a 2020 2020 2020 2020 7365 6c66  ls(.        self
+00002000: 2c20 6c6f 6361 6c5f 6164 6472 3a20 7374  , local_addr: st
+00002010: 722c 2065 7870 6563 7465 645f 636c 6965  r, expected_clie
+00002020: 6e74 5f61 6464 723a 2073 7472 2c20 6661  nt_addr: str, fa
+00002030: 6b65 5f6c 6f63 616c 686f 7374 5f64 6e73  ke_localhost_dns
+00002040: 3a20 4e6f 6e65 0a20 2020 2029 202d 3e20  : None.    ) -> 
+00002050: 4e6f 6e65 3a0a 2020 2020 2020 2020 636c  None:.        cl
+00002060: 6965 6e74 5f61 6464 7220 3d20 4e6f 6e65  ient_addr = None
+00002070: 2c20 4e6f 6e65 0a0a 2020 2020 2020 2020  , None..        
+00002080: 6465 6620 7365 7276 6528 2920 2d3e 204e  def serve() -> N
+00002090: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000020a0: 206e 6f6e 6c6f 6361 6c20 636c 6965 6e74   nonlocal client
+000020b0: 5f61 6464 720a 2020 2020 2020 2020 2020  _addr.          
+000020c0: 2020 636c 6965 6e74 2c20 636c 6965 6e74    client, client
+000020d0: 5f61 6464 7220 3d20 7365 7276 6572 5f73  _addr = server_s
+000020e0: 6f63 6b2e 6163 6365 7074 2829 0a20 2020  ock.accept().   
+000020f0: 2020 2020 2020 2020 2063 6c69 656e 742e           client.
+00002100: 636c 6f73 6528 290a 0a20 2020 2020 2020  close()..       
+00002110: 2066 616d 696c 7920 3d20 280a 2020 2020   family = (.    
+00002120: 2020 2020 2020 2020 4164 6472 6573 7346          AddressF
+00002130: 616d 696c 792e 4146 5f49 4e45 540a 2020  amily.AF_INET.  
+00002140: 2020 2020 2020 2020 2020 6966 206c 6f63            if loc
+00002150: 616c 5f61 6464 7220 3d3d 2022 3132 372e  al_addr == "127.
+00002160: 302e 302e 3122 0a20 2020 2020 2020 2020  0.0.1".         
+00002170: 2020 2065 6c73 6520 4164 6472 6573 7346     else AddressF
+00002180: 616d 696c 792e 4146 5f49 4e45 5436 0a20  amily.AF_INET6. 
+00002190: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000021a0: 2073 6572 7665 725f 736f 636b 203d 2073   server_sock = s
+000021b0: 6f63 6b65 742e 736f 636b 6574 2866 616d  ocket.socket(fam
+000021c0: 696c 7929 0a20 2020 2020 2020 2073 6572  ily).        ser
+000021d0: 7665 725f 736f 636b 2e62 696e 6428 286c  ver_sock.bind((l
+000021e0: 6f63 616c 5f61 6464 722c 2030 2929 0a20  ocal_addr, 0)). 
+000021f0: 2020 2020 2020 2073 6572 7665 725f 736f         server_so
+00002200: 636b 2e6c 6973 7465 6e28 290a 2020 2020  ck.listen().    
+00002210: 2020 2020 706f 7274 203d 2073 6572 7665      port = serve
+00002220: 725f 736f 636b 2e67 6574 736f 636b 6e61  r_sock.getsockna
+00002230: 6d65 2829 5b31 5d0a 2020 2020 2020 2020  me()[1].        
+00002240: 7468 7265 6164 203d 2054 6872 6561 6428  thread = Thread(
+00002250: 7461 7267 6574 3d73 6572 7665 2c20 6461  target=serve, da
+00002260: 656d 6f6e 3d54 7275 6529 0a20 2020 2020  emon=True).     
+00002270: 2020 2074 6872 6561 642e 7374 6172 7428     thread.start(
+00002280: 290a 0a20 2020 2020 2020 2061 7379 6e63  )..        async
+00002290: 2077 6974 6820 6177 6169 7420 636f 6e6e   with await conn
+000022a0: 6563 745f 7463 7028 226c 6f63 616c 686f  ect_tcp("localho
+000022b0: 7374 222c 2070 6f72 7429 3a0a 2020 2020  st", port):.    
+000022c0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+000022d0: 2020 2020 2020 7468 7265 6164 2e6a 6f69        thread.joi
+000022e0: 6e28 290a 2020 2020 2020 2020 7365 7276  n().        serv
+000022f0: 6572 5f73 6f63 6b2e 636c 6f73 6528 290a  er_sock.close().
+00002300: 2020 2020 2020 2020 6173 7365 7274 2063          assert c
+00002310: 6c69 656e 745f 6164 6472 5b30 5d20 3d3d  lient_addr[0] ==
+00002320: 2065 7870 6563 7465 645f 636c 6965 6e74   expected_client
+00002330: 5f61 6464 720a 0a20 2020 2040 7079 7465  _addr..    @pyte
+00002340: 7374 2e6d 6172 6b2e 7061 7261 6d65 7472  st.mark.parametr
+00002350: 697a 6528 0a20 2020 2020 2020 2022 7461  ize(.        "ta
+00002360: 7267 6574 2c20 6578 6365 7074 696f 6e5f  rget, exception_
+00002370: 636c 6173 7322 2c0a 2020 2020 2020 2020  class",.        
+00002380: 5b0a 2020 2020 2020 2020 2020 2020 7079  [.            py
+00002390: 7465 7374 2e70 6172 616d 280a 2020 2020  test.param(.    
+000023a0: 2020 2020 2020 2020 2020 2020 226c 6f63              "loc
+000023b0: 616c 686f 7374 222c 2045 7863 6570 7469  alhost", Excepti
+000023c0: 6f6e 4772 6f75 702c 2069 643d 226d 756c  onGroup, id="mul
+000023d0: 7469 222c 206d 6172 6b73 3d5b 736b 6970  ti", marks=[skip
+000023e0: 5f69 7076 365f 6d61 726b 5d0a 2020 2020  _ipv6_mark].    
+000023f0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+00002400: 2020 2020 2020 2070 7974 6573 742e 7061         pytest.pa
+00002410: 7261 6d28 2231 3237 2e30 2e30 2e31 222c  ram("127.0.0.1",
+00002420: 2043 6f6e 6e65 6374 696f 6e52 6566 7573   ConnectionRefus
+00002430: 6564 4572 726f 722c 2069 643d 2273 696e  edError, id="sin
+00002440: 676c 6522 292c 0a20 2020 2020 2020 205d  gle"),.        ]
+00002450: 2c0a 2020 2020 290a 2020 2020 6173 796e  ,.    ).    asyn
+00002460: 6320 6465 6620 7465 7374 5f63 6f6e 6e65  c def test_conne
+00002470: 6374 696f 6e5f 7265 6675 7365 6428 0a20  ction_refused(. 
+00002480: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00002490: 2020 2020 2074 6172 6765 743a 2073 7472       target: str
+000024a0: 2c0a 2020 2020 2020 2020 6578 6365 7074  ,.        except
+000024b0: 696f 6e5f 636c 6173 733a 2074 7970 655b  ion_class: type[
+000024c0: 4578 6365 7074 696f 6e47 726f 7570 5d20  ExceptionGroup] 
+000024d0: 7c20 7479 7065 5b43 6f6e 6e65 6374 696f  | type[Connectio
+000024e0: 6e52 6566 7573 6564 4572 726f 725d 2c0a  nRefusedError],.
+000024f0: 2020 2020 2020 2020 6661 6b65 5f6c 6f63          fake_loc
+00002500: 616c 686f 7374 5f64 6e73 3a20 4e6f 6e65  alhost_dns: None
+00002510: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
+00002520: 0a20 2020 2020 2020 2064 756d 6d79 5f73  .        dummy_s
+00002530: 6f63 6b65 7420 3d20 736f 636b 6574 2e73  ocket = socket.s
+00002540: 6f63 6b65 7428 4164 6472 6573 7346 616d  ocket(AddressFam
+00002550: 696c 792e 4146 5f49 4e45 5436 290a 2020  ily.AF_INET6).  
+00002560: 2020 2020 2020 6475 6d6d 795f 736f 636b        dummy_sock
+00002570: 6574 2e62 696e 6428 2822 3a3a 222c 2030  et.bind(("::", 0
+00002580: 2929 0a20 2020 2020 2020 2066 7265 655f  )).        free_
+00002590: 706f 7274 203d 2064 756d 6d79 5f73 6f63  port = dummy_soc
+000025a0: 6b65 742e 6765 7473 6f63 6b6e 616d 6528  ket.getsockname(
+000025b0: 295b 315d 0a20 2020 2020 2020 2064 756d  )[1].        dum
+000025c0: 6d79 5f73 6f63 6b65 742e 636c 6f73 6528  my_socket.close(
+000025d0: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
+000025e0: 7079 7465 7374 2e72 6169 7365 7328 4f53  pytest.raises(OS
+000025f0: 4572 726f 7229 2061 7320 6578 633a 0a20  Error) as exc:. 
+00002600: 2020 2020 2020 2020 2020 2061 7761 6974             await
+00002610: 2063 6f6e 6e65 6374 5f74 6370 2874 6172   connect_tcp(tar
+00002620: 6765 742c 2066 7265 655f 706f 7274 290a  get, free_port).
+00002630: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00002640: 6578 632e 6d61 7463 6828 2241 6c6c 2063  exc.match("All c
+00002650: 6f6e 6e65 6374 696f 6e20 6174 7465 6d70  onnection attemp
+00002660: 7473 2066 6169 6c65 6422 290a 2020 2020  ts failed").    
+00002670: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
+00002680: 7461 6e63 6528 6578 632e 7661 6c75 652e  tance(exc.value.
+00002690: 5f5f 6361 7573 655f 5f2c 2065 7863 6570  __cause__, excep
+000026a0: 7469 6f6e 5f63 6c61 7373 290a 2020 2020  tion_class).    
+000026b0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+000026c0: 6528 6578 632e 7661 6c75 652e 5f5f 6361  e(exc.value.__ca
+000026d0: 7573 655f 5f2c 2045 7863 6570 7469 6f6e  use__, Exception
+000026e0: 4772 6f75 7029 3a0a 2020 2020 2020 2020  Group):.        
+000026f0: 2020 2020 666f 7220 6578 6365 7074 696f      for exceptio
+00002700: 6e20 696e 2065 7863 2e76 616c 7565 2e5f  n in exc.value._
+00002710: 5f63 6175 7365 5f5f 2e65 7863 6570 7469  _cause__.excepti
+00002720: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
+00002730: 2020 2020 2061 7373 6572 7420 6973 696e       assert isin
+00002740: 7374 616e 6365 2865 7863 6570 7469 6f6e  stance(exception
+00002750: 2c20 436f 6e6e 6563 7469 6f6e 5265 6675  , ConnectionRefu
+00002760: 7365 6445 7272 6f72 290a 0a20 2020 2061  sedError)..    a
+00002770: 7379 6e63 2064 6566 2074 6573 745f 7265  sync def test_re
+00002780: 6365 6976 655f 7469 6d65 6f75 7428 0a20  ceive_timeout(. 
+00002790: 2020 2020 2020 2073 656c 662c 2073 6572         self, ser
+000027a0: 7665 725f 736f 636b 3a20 736f 636b 6574  ver_sock: socket
+000027b0: 2e73 6f63 6b65 742c 2073 6572 7665 725f  .socket, server_
+000027c0: 6164 6472 3a20 7475 706c 655b 7374 722c  addr: tuple[str,
+000027d0: 2069 6e74 5d0a 2020 2020 2920 2d3e 204e   int].    ) -> N
+000027e0: 6f6e 653a 0a20 2020 2020 2020 2064 6566  one:.        def
+000027f0: 2073 6572 7665 2829 202d 3e20 4e6f 6e65   serve() -> None
+00002800: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
+00002810: 6e6e 2c20 5f20 3d20 7365 7276 6572 5f73  nn, _ = server_s
+00002820: 6f63 6b2e 6163 6365 7074 2829 0a20 2020  ock.accept().   
+00002830: 2020 2020 2020 2020 2074 696d 652e 736c           time.sl
+00002840: 6565 7028 3129 0a20 2020 2020 2020 2020  eep(1).         
+00002850: 2020 2063 6f6e 6e2e 636c 6f73 6528 290a     conn.close().
+00002860: 0a20 2020 2020 2020 2074 6872 6561 6420  .        thread 
+00002870: 3d20 5468 7265 6164 2874 6172 6765 743d  = Thread(target=
+00002880: 7365 7276 652c 2064 6165 6d6f 6e3d 5472  serve, daemon=Tr
+00002890: 7565 290a 2020 2020 2020 2020 7468 7265  ue).        thre
+000028a0: 6164 2e73 7461 7274 2829 0a20 2020 2020  ad.start().     
+000028b0: 2020 2061 7379 6e63 2077 6974 6820 6177     async with aw
+000028c0: 6169 7420 636f 6e6e 6563 745f 7463 7028  ait connect_tcp(
+000028d0: 2a73 6572 7665 725f 6164 6472 2920 6173  *server_addr) as
+000028e0: 2073 7472 6561 6d3a 0a20 2020 2020 2020   stream:.       
+000028f0: 2020 2020 2073 7461 7274 5f74 696d 6520       start_time 
+00002900: 3d20 7469 6d65 2e6d 6f6e 6f74 6f6e 6963  = time.monotonic
+00002910: 2829 0a20 2020 2020 2020 2020 2020 2077  ().            w
+00002920: 6974 6820 6d6f 7665 5f6f 6e5f 6166 7465  ith move_on_afte
+00002930: 7228 302e 3129 3a0a 2020 2020 2020 2020  r(0.1):.        
+00002940: 2020 2020 2020 2020 7768 696c 6520 7469          while ti
+00002950: 6d65 2e6d 6f6e 6f74 6f6e 6963 2829 202d  me.monotonic() -
+00002960: 2073 7461 7274 5f74 696d 6520 3c20 302e   start_time < 0.
+00002970: 333a 0a20 2020 2020 2020 2020 2020 2020  3:.             
+00002980: 2020 2020 2020 2061 7761 6974 2073 7472         await str
+00002990: 6561 6d2e 7265 6365 6976 6528 3129 0a0a  eam.receive(1)..
+000029a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029b0: 7079 7465 7374 2e66 6169 6c28 2254 6865  pytest.fail("The
+000029c0: 2074 696d 656f 7574 2077 6173 206e 6f74   timeout was not
+000029d0: 2072 6573 7065 6374 6564 2229 0a0a 2020   respected")..  
+000029e0: 2020 6173 796e 6320 6465 6620 7465 7374    async def test
+000029f0: 5f63 6f6e 6375 7272 656e 745f 7365 6e64  _concurrent_send
+00002a00: 2873 656c 662c 2073 6572 7665 725f 6164  (self, server_ad
+00002a10: 6472 3a20 7475 706c 655b 7374 722c 2069  dr: tuple[str, i
+00002a20: 6e74 5d29 202d 3e20 4e6f 6e65 3a0a 2020  nt]) -> None:.  
+00002a30: 2020 2020 2020 6173 796e 6320 6465 6620        async def 
+00002a40: 7365 6e64 5f64 6174 6128 2920 2d3e 204e  send_data() -> N
+00002a50: 6f52 6574 7572 6e3a 0a20 2020 2020 2020  oReturn:.       
+00002a60: 2020 2020 2077 6869 6c65 2054 7275 653a       while True:
+00002a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002a80: 2061 7761 6974 2073 7472 6561 6d2e 7365   await stream.se
+00002a90: 6e64 2862 225c 7830 3022 202a 2034 3039  nd(b"\x00" * 409
+00002aa0: 3629 0a0a 2020 2020 2020 2020 6173 796e  6)..        asyn
+00002ab0: 6320 7769 7468 2061 7761 6974 2063 6f6e  c with await con
+00002ac0: 6e65 6374 5f74 6370 282a 7365 7276 6572  nect_tcp(*server
+00002ad0: 5f61 6464 7229 2061 7320 7374 7265 616d  _addr) as stream
+00002ae0: 3a0a 2020 2020 2020 2020 2020 2020 6173  :.            as
+00002af0: 796e 6320 7769 7468 2063 7265 6174 655f  ync with create_
+00002b00: 7461 736b 5f67 726f 7570 2829 2061 7320  task_group() as 
+00002b10: 7467 3a0a 2020 2020 2020 2020 2020 2020  tg:.            
+00002b20: 2020 2020 7467 2e73 7461 7274 5f73 6f6f      tg.start_soo
+00002b30: 6e28 7365 6e64 5f64 6174 6129 0a20 2020  n(send_data).   
+00002b40: 2020 2020 2020 2020 2020 2020 2061 7761               awa
+00002b50: 6974 2077 6169 745f 616c 6c5f 7461 736b  it wait_all_task
+00002b60: 735f 626c 6f63 6b65 6428 290a 2020 2020  s_blocked().    
+00002b70: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00002b80: 2070 7974 6573 742e 7261 6973 6573 2842   pytest.raises(B
+00002b90: 7573 7952 6573 6f75 7263 6545 7272 6f72  usyResourceError
+00002ba0: 2920 6173 2065 7863 3a0a 2020 2020 2020  ) as exc:.      
+00002bb0: 2020 2020 2020 2020 2020 2020 2020 6177                aw
+00002bc0: 6169 7420 7374 7265 616d 2e73 656e 6428  ait stream.send(
+00002bd0: 6222 666f 6f22 290a 0a20 2020 2020 2020  b"foo")..       
+00002be0: 2020 2020 2020 2020 2065 7863 2e6d 6174           exc.mat
+00002bf0: 6368 2822 616c 7265 6164 7920 7772 6974  ch("already writ
+00002c00: 696e 6720 746f 2229 0a20 2020 2020 2020  ing to").       
+00002c10: 2020 2020 2020 2020 2074 672e 6361 6e63           tg.canc
+00002c20: 656c 5f73 636f 7065 2e63 616e 6365 6c28  el_scope.cancel(
+00002c30: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
+00002c40: 2074 6573 745f 636f 6e63 7572 7265 6e74   test_concurrent
+00002c50: 5f72 6563 6569 7665 2873 656c 662c 2073  _receive(self, s
+00002c60: 6572 7665 725f 6164 6472 3a20 7475 706c  erver_addr: tupl
+00002c70: 655b 7374 722c 2069 6e74 5d29 202d 3e20  e[str, int]) -> 
+00002c80: 4e6f 6e65 3a0a 2020 2020 2020 2020 6173  None:.        as
+00002c90: 796e 6320 7769 7468 2061 7761 6974 2063  ync with await c
+00002ca0: 6f6e 6e65 6374 5f74 6370 282a 7365 7276  onnect_tcp(*serv
+00002cb0: 6572 5f61 6464 7229 2061 7320 636c 6965  er_addr) as clie
+00002cc0: 6e74 3a0a 2020 2020 2020 2020 2020 2020  nt:.            
+00002cd0: 6173 796e 6320 7769 7468 2063 7265 6174  async with creat
+00002ce0: 655f 7461 736b 5f67 726f 7570 2829 2061  e_task_group() a
+00002cf0: 7320 7467 3a0a 2020 2020 2020 2020 2020  s tg:.          
+00002d00: 2020 2020 2020 7467 2e73 7461 7274 5f73        tg.start_s
+00002d10: 6f6f 6e28 636c 6965 6e74 2e72 6563 6569  oon(client.recei
+00002d20: 7665 290a 2020 2020 2020 2020 2020 2020  ve).            
+00002d30: 2020 2020 6177 6169 7420 7761 6974 5f61      await wait_a
+00002d40: 6c6c 5f74 6173 6b73 5f62 6c6f 636b 6564  ll_tasks_blocked
+00002d50: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00002d60: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00002d70: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00002d80: 2070 7974 6573 742e 7261 6973 6573 2842   pytest.raises(B
+00002d90: 7573 7952 6573 6f75 7263 6545 7272 6f72  usyResourceError
+00002da0: 2920 6173 2065 7863 3a0a 2020 2020 2020  ) as exc:.      
+00002db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002dc0: 2020 6177 6169 7420 636c 6965 6e74 2e72    await client.r
+00002dd0: 6563 6569 7665 2829 0a0a 2020 2020 2020  eceive()..      
+00002de0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+00002df0: 632e 6d61 7463 6828 2261 6c72 6561 6479  c.match("already
+00002e00: 2072 6561 6469 6e67 2066 726f 6d22 290a   reading from").
+00002e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e20: 6669 6e61 6c6c 793a 0a20 2020 2020 2020  finally:.       
+00002e30: 2020 2020 2020 2020 2020 2020 2074 672e               tg.
+00002e40: 6361 6e63 656c 5f73 636f 7065 2e63 616e  cancel_scope.can
+00002e50: 6365 6c28 290a 0a20 2020 2061 7379 6e63  cel()..    async
+00002e60: 2064 6566 2074 6573 745f 636c 6f73 655f   def test_close_
+00002e70: 6475 7269 6e67 5f72 6563 6569 7665 2873  during_receive(s
+00002e80: 656c 662c 2073 6572 7665 725f 6164 6472  elf, server_addr
+00002e90: 3a20 7475 706c 655b 7374 722c 2069 6e74  : tuple[str, int
+00002ea0: 5d29 202d 3e20 4e6f 6e65 3a0a 2020 2020  ]) -> None:.    
+00002eb0: 2020 2020 6173 796e 6320 6465 6620 696e      async def in
+00002ec0: 7465 7272 7570 7428 2920 2d3e 204e 6f6e  terrupt() -> Non
+00002ed0: 653a 0a20 2020 2020 2020 2020 2020 2061  e:.            a
+00002ee0: 7761 6974 2077 6169 745f 616c 6c5f 7461  wait wait_all_ta
+00002ef0: 736b 735f 626c 6f63 6b65 6428 290a 2020  sks_blocked().  
+00002f00: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+00002f10: 7374 7265 616d 2e61 636c 6f73 6528 290a  stream.aclose().
+00002f20: 0a20 2020 2020 2020 2061 7379 6e63 2077  .        async w
+00002f30: 6974 6820 6177 6169 7420 636f 6e6e 6563  ith await connec
+00002f40: 745f 7463 7028 2a73 6572 7665 725f 6164  t_tcp(*server_ad
+00002f50: 6472 2920 6173 2073 7472 6561 6d3a 0a20  dr) as stream:. 
+00002f60: 2020 2020 2020 2020 2020 2061 7379 6e63             async
+00002f70: 2077 6974 6820 6372 6561 7465 5f74 6173   with create_tas
+00002f80: 6b5f 6772 6f75 7028 2920 6173 2074 673a  k_group() as tg:
+00002f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002fa0: 2074 672e 7374 6172 745f 736f 6f6e 2869   tg.start_soon(i
+00002fb0: 6e74 6572 7275 7074 290a 2020 2020 2020  nterrupt).      
+00002fc0: 2020 2020 2020 2020 2020 7769 7468 2070            with p
+00002fd0: 7974 6573 742e 7261 6973 6573 2843 6c6f  ytest.raises(Clo
+00002fe0: 7365 6452 6573 6f75 7263 6545 7272 6f72  sedResourceError
+00002ff0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00003000: 2020 2020 2020 2061 7761 6974 2073 7472         await str
+00003010: 6561 6d2e 7265 6365 6976 6528 290a 0a20  eam.receive().. 
+00003020: 2020 2061 7379 6e63 2064 6566 2074 6573     async def tes
+00003030: 745f 7265 6365 6976 655f 6166 7465 725f  t_receive_after_
+00003040: 636c 6f73 6528 7365 6c66 2c20 7365 7276  close(self, serv
+00003050: 6572 5f61 6464 723a 2074 7570 6c65 5b73  er_addr: tuple[s
+00003060: 7472 2c20 696e 745d 2920 2d3e 204e 6f6e  tr, int]) -> Non
+00003070: 653a 0a20 2020 2020 2020 2073 7472 6561  e:.        strea
+00003080: 6d20 3d20 6177 6169 7420 636f 6e6e 6563  m = await connec
+00003090: 745f 7463 7028 2a73 6572 7665 725f 6164  t_tcp(*server_ad
+000030a0: 6472 290a 2020 2020 2020 2020 6177 6169  dr).        awai
+000030b0: 7420 7374 7265 616d 2e61 636c 6f73 6528  t stream.aclose(
+000030c0: 290a 2020 2020 2020 2020 7769 7468 2070  ).        with p
+000030d0: 7974 6573 742e 7261 6973 6573 2843 6c6f  ytest.raises(Clo
+000030e0: 7365 6452 6573 6f75 7263 6545 7272 6f72  sedResourceError
+000030f0: 293a 0a20 2020 2020 2020 2020 2020 2061  ):.            a
+00003100: 7761 6974 2073 7472 6561 6d2e 7265 6365  wait stream.rece
+00003110: 6976 6528 290a 0a20 2020 2061 7379 6e63  ive()..    async
+00003120: 2064 6566 2074 6573 745f 7365 6e64 5f61   def test_send_a
+00003130: 6674 6572 5f63 6c6f 7365 2873 656c 662c  fter_close(self,
+00003140: 2073 6572 7665 725f 6164 6472 3a20 7475   server_addr: tu
+00003150: 706c 655b 7374 722c 2069 6e74 5d29 202d  ple[str, int]) -
+00003160: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00003170: 7374 7265 616d 203d 2061 7761 6974 2063  stream = await c
+00003180: 6f6e 6e65 6374 5f74 6370 282a 7365 7276  onnect_tcp(*serv
+00003190: 6572 5f61 6464 7229 0a20 2020 2020 2020  er_addr).       
+000031a0: 2061 7761 6974 2073 7472 6561 6d2e 6163   await stream.ac
+000031b0: 6c6f 7365 2829 0a20 2020 2020 2020 2077  lose().        w
+000031c0: 6974 6820 7079 7465 7374 2e72 6169 7365  ith pytest.raise
+000031d0: 7328 436c 6f73 6564 5265 736f 7572 6365  s(ClosedResource
+000031e0: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
+000031f0: 2020 2020 6177 6169 7420 7374 7265 616d      await stream
+00003200: 2e73 656e 6428 6222 666f 6f22 290a 0a20  .send(b"foo").. 
+00003210: 2020 2061 7379 6e63 2064 6566 2074 6573     async def tes
+00003220: 745f 7365 6e64 5f61 6674 6572 5f70 6565  t_send_after_pee
+00003230: 725f 636c 6f73 6564 2873 656c 662c 2066  r_closed(self, f
+00003240: 616d 696c 793a 2041 6e79 4950 4164 6472  amily: AnyIPAddr
+00003250: 6573 7346 616d 696c 7929 202d 3e20 4e6f  essFamily) -> No
+00003260: 6e65 3a0a 2020 2020 2020 2020 6465 6620  ne:.        def 
+00003270: 7365 7276 655f 6f6e 6365 2829 202d 3e20  serve_once() -> 
+00003280: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00003290: 2020 636c 6965 6e74 5f73 6f63 6b2c 205f    client_sock, _
+000032a0: 203d 2073 6572 7665 725f 736f 636b 2e61   = server_sock.a
+000032b0: 6363 6570 7428 290a 2020 2020 2020 2020  ccept().        
+000032c0: 2020 2020 636c 6965 6e74 5f73 6f63 6b2e      client_sock.
+000032d0: 636c 6f73 6528 290a 2020 2020 2020 2020  close().        
+000032e0: 2020 2020 7365 7276 6572 5f73 6f63 6b2e      server_sock.
+000032f0: 636c 6f73 6528 290a 0a20 2020 2020 2020  close()..       
+00003300: 2073 6572 7665 725f 736f 636b 203d 2073   server_sock = s
+00003310: 6f63 6b65 742e 736f 636b 6574 2866 616d  ocket.socket(fam
+00003320: 696c 792c 2073 6f63 6b65 742e 534f 434b  ily, socket.SOCK
+00003330: 5f53 5452 4541 4d29 0a20 2020 2020 2020  _STREAM).       
+00003340: 2073 6572 7665 725f 736f 636b 2e73 6574   server_sock.set
+00003350: 7469 6d65 6f75 7428 3129 0a20 2020 2020  timeout(1).     
+00003360: 2020 2073 6572 7665 725f 736f 636b 2e62     server_sock.b
+00003370: 696e 6428 2822 6c6f 6361 6c68 6f73 7422  ind(("localhost"
+00003380: 2c20 3029 290a 2020 2020 2020 2020 7365  , 0)).        se
+00003390: 7276 6572 5f61 6464 7220 3d20 7365 7276  rver_addr = serv
+000033a0: 6572 5f73 6f63 6b2e 6765 7473 6f63 6b6e  er_sock.getsockn
+000033b0: 616d 6528 295b 3a32 5d0a 2020 2020 2020  ame()[:2].      
+000033c0: 2020 7365 7276 6572 5f73 6f63 6b2e 6c69    server_sock.li
+000033d0: 7374 656e 2829 0a20 2020 2020 2020 2074  sten().        t
+000033e0: 6872 6561 6420 3d20 5468 7265 6164 2874  hread = Thread(t
+000033f0: 6172 6765 743d 7365 7276 655f 6f6e 6365  arget=serve_once
+00003400: 2c20 6461 656d 6f6e 3d54 7275 6529 0a20  , daemon=True). 
+00003410: 2020 2020 2020 2074 6872 6561 642e 7374         thread.st
+00003420: 6172 7428 290a 0a20 2020 2020 2020 2077  art()..        w
+00003430: 6974 6820 7079 7465 7374 2e72 6169 7365  ith pytest.raise
+00003440: 7328 4272 6f6b 656e 5265 736f 7572 6365  s(BrokenResource
+00003450: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
+00003460: 2020 2020 6173 796e 6320 7769 7468 2061      async with a
+00003470: 7761 6974 2063 6f6e 6e65 6374 5f74 6370  wait connect_tcp
+00003480: 282a 7365 7276 6572 5f61 6464 7229 2061  (*server_addr) a
+00003490: 7320 7374 7265 616d 3a0a 2020 2020 2020  s stream:.      
+000034a0: 2020 2020 2020 2020 2020 666f 7220 5f20            for _ 
+000034b0: 696e 2072 616e 6765 2831 3030 3029 3a0a  in range(1000):.
+000034c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034d0: 2020 2020 6177 6169 7420 7374 7265 616d      await stream
+000034e0: 2e73 656e 6428 6222 666f 6f22 290a 0a20  .send(b"foo").. 
+000034f0: 2020 2020 2020 2074 6872 6561 642e 6a6f         thread.jo
+00003500: 696e 2829 0a0a 2020 2020 6173 796e 6320  in()..    async 
+00003510: 6465 6620 7465 7374 5f63 6f6e 6e65 6374  def test_connect
+00003520: 5f74 6370 5f77 6974 685f 746c 7328 0a20  _tcp_with_tls(. 
+00003530: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00003540: 2020 2020 2073 6572 7665 725f 636f 6e74       server_cont
+00003550: 6578 743a 2053 534c 436f 6e74 6578 742c  ext: SSLContext,
+00003560: 0a20 2020 2020 2020 2063 6c69 656e 745f  .        client_
+00003570: 636f 6e74 6578 743a 2053 534c 436f 6e74  context: SSLCont
+00003580: 6578 742c 0a20 2020 2020 2020 2073 6572  ext,.        ser
+00003590: 7665 725f 736f 636b 3a20 736f 636b 6574  ver_sock: socket
+000035a0: 2e73 6f63 6b65 742c 0a20 2020 2020 2020  .socket,.       
+000035b0: 2073 6572 7665 725f 6164 6472 3a20 7475   server_addr: tu
+000035c0: 706c 655b 7374 722c 2069 6e74 5d2c 0a20  ple[str, int],. 
+000035d0: 2020 2029 202d 3e20 4e6f 6e65 3a0a 2020     ) -> None:.  
+000035e0: 2020 2020 2020 6465 6620 7365 7276 6528        def serve(
+000035f0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00003600: 2020 2020 2020 2077 6974 6820 7375 7070         with supp
+00003610: 7265 7373 2873 6f63 6b65 742e 7469 6d65  ress(socket.time
+00003620: 6f75 7429 3a0a 2020 2020 2020 2020 2020  out):.          
+00003630: 2020 2020 2020 636c 6965 6e74 2c20 6164        client, ad
+00003640: 6472 203d 2073 6572 7665 725f 736f 636b  dr = server_sock
+00003650: 2e61 6363 6570 7428 290a 2020 2020 2020  .accept().      
+00003660: 2020 2020 2020 2020 2020 636c 6965 6e74            client
+00003670: 2e73 6574 7469 6d65 6f75 7428 3129 0a20  .settimeout(1). 
+00003680: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00003690: 6c69 656e 7420 3d20 7365 7276 6572 5f63  lient = server_c
+000036a0: 6f6e 7465 7874 2e77 7261 705f 736f 636b  ontext.wrap_sock
+000036b0: 6574 2863 6c69 656e 742c 2073 6572 7665  et(client, serve
+000036c0: 725f 7369 6465 3d54 7275 6529 0a20 2020  r_side=True).   
+000036d0: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+000036e0: 6120 3d20 636c 6965 6e74 2e72 6563 7628  a = client.recv(
+000036f0: 3130 3029 0a20 2020 2020 2020 2020 2020  100).           
+00003700: 2020 2020 2063 6c69 656e 742e 7365 6e64       client.send
+00003710: 616c 6c28 6461 7461 5b3a 3a2d 315d 290a  all(data[::-1]).
+00003720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003730: 636c 6965 6e74 2e75 6e77 7261 7028 290a  client.unwrap().
+00003740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003750: 636c 6965 6e74 2e63 6c6f 7365 2829 0a0a  client.close()..
+00003760: 2020 2020 2020 2020 2320 5468 6520 544c          # The TL
+00003770: 5353 7472 6561 6d20 7465 7374 7320 6172  SStream tests ar
+00003780: 6520 6d6f 7265 2063 6f6d 7072 6568 656e  e more comprehen
+00003790: 7369 7665 2074 6861 6e20 7468 6973 206f  sive than this o
+000037a0: 6e65 210a 2020 2020 2020 2020 7468 7265  ne!.        thre
+000037b0: 6164 203d 2054 6872 6561 6428 7461 7267  ad = Thread(targ
+000037c0: 6574 3d73 6572 7665 2c20 6461 656d 6f6e  et=serve, daemon
+000037d0: 3d54 7275 6529 0a20 2020 2020 2020 2074  =True).        t
+000037e0: 6872 6561 642e 7374 6172 7428 290a 2020  hread.start().  
+000037f0: 2020 2020 2020 6173 796e 6320 7769 7468        async with
+00003800: 2061 7761 6974 2063 6f6e 6e65 6374 5f74   await connect_t
+00003810: 6370 280a 2020 2020 2020 2020 2020 2020  cp(.            
+00003820: 2a73 6572 7665 725f 6164 6472 2c20 746c  *server_addr, tl
+00003830: 735f 686f 7374 6e61 6d65 3d22 6c6f 6361  s_hostname="loca
+00003840: 6c68 6f73 7422 2c20 7373 6c5f 636f 6e74  lhost", ssl_cont
+00003850: 6578 743d 636c 6965 6e74 5f63 6f6e 7465  ext=client_conte
+00003860: 7874 0a20 2020 2020 2020 2029 2061 7320  xt.        ) as 
+00003870: 7374 7265 616d 3a0a 2020 2020 2020 2020  stream:.        
+00003880: 2020 2020 6177 6169 7420 7374 7265 616d      await stream
+00003890: 2e73 656e 6428 6222 6865 6c6c 6f22 290a  .send(b"hello").
+000038a0: 2020 2020 2020 2020 2020 2020 7265 7370              resp
+000038b0: 6f6e 7365 203d 2061 7761 6974 2073 7472  onse = await str
+000038c0: 6561 6d2e 7265 6365 6976 6528 290a 0a20  eam.receive().. 
+000038d0: 2020 2020 2020 2061 7373 6572 7420 7265         assert re
+000038e0: 7370 6f6e 7365 203d 3d20 6222 6f6c 6c65  sponse == b"olle
+000038f0: 6822 0a20 2020 2020 2020 2074 6872 6561  h".        threa
+00003900: 642e 6a6f 696e 2829 0a0a 2020 2020 6173  d.join()..    as
+00003910: 796e 6320 6465 6620 7465 7374 5f63 6f6e  ync def test_con
+00003920: 6e65 6374 5f74 6370 5f77 6974 685f 746c  nect_tcp_with_tl
+00003930: 735f 6365 7274 5f63 6865 636b 5f66 6169  s_cert_check_fai
+00003940: 6c28 0a20 2020 2020 2020 2073 656c 662c  l(.        self,
+00003950: 0a20 2020 2020 2020 2073 6572 7665 725f  .        server_
+00003960: 636f 6e74 6578 743a 2053 534c 436f 6e74  context: SSLCont
+00003970: 6578 742c 0a20 2020 2020 2020 2073 6572  ext,.        ser
+00003980: 7665 725f 736f 636b 3a20 736f 636b 6574  ver_sock: socket
+00003990: 2e73 6f63 6b65 742c 0a20 2020 2020 2020  .socket,.       
+000039a0: 2073 6572 7665 725f 6164 6472 3a20 7475   server_addr: tu
+000039b0: 706c 655b 7374 722c 2069 6e74 5d2c 0a20  ple[str, int],. 
+000039c0: 2020 2029 202d 3e20 4e6f 6e65 3a0a 2020     ) -> None:.  
+000039d0: 2020 2020 2020 7468 7265 6164 5f65 7863        thread_exc
+000039e0: 6570 7469 6f6e 203d 204e 6f6e 650a 0a20  eption = None.. 
+000039f0: 2020 2020 2020 2064 6566 2073 6572 7665         def serve
+00003a00: 2829 202d 3e20 4e6f 6e65 3a0a 2020 2020  () -> None:.    
+00003a10: 2020 2020 2020 2020 6e6f 6e6c 6f63 616c          nonlocal
+00003a20: 2074 6872 6561 645f 6578 6365 7074 696f   thread_exceptio
+00003a30: 6e0a 2020 2020 2020 2020 2020 2020 636c  n.            cl
+00003a40: 6965 6e74 2c20 6164 6472 203d 2073 6572  ient, addr = ser
+00003a50: 7665 725f 736f 636b 2e61 6363 6570 7428  ver_sock.accept(
+00003a60: 290a 2020 2020 2020 2020 2020 2020 7769  ).            wi
+00003a70: 7468 2063 6c69 656e 743a 0a20 2020 2020  th client:.     
+00003a80: 2020 2020 2020 2020 2020 2063 6c69 656e             clien
+00003a90: 742e 7365 7474 696d 656f 7574 2831 290a  t.settimeout(1).
+00003aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ab0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00003ac0: 2020 2020 2020 2020 2073 6572 7665 725f           server_
+00003ad0: 636f 6e74 6578 742e 7772 6170 5f73 6f63  context.wrap_soc
+00003ae0: 6b65 7428 636c 6965 6e74 2c20 7365 7276  ket(client, serv
+00003af0: 6572 5f73 6964 653d 5472 7565 290a 2020  er_side=True).  
+00003b00: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+00003b10: 6365 7074 204f 5345 7272 6f72 3a0a 2020  cept OSError:.  
+00003b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b30: 2020 7061 7373 0a20 2020 2020 2020 2020    pass.         
+00003b40: 2020 2020 2020 2065 7863 6570 7420 4261         except Ba
+00003b50: 7365 4578 6365 7074 696f 6e20 6173 2065  seException as e
+00003b60: 7863 3a0a 2020 2020 2020 2020 2020 2020  xc:.            
+00003b70: 2020 2020 2020 2020 7468 7265 6164 5f65          thread_e
+00003b80: 7863 6570 7469 6f6e 203d 2065 7863 0a0a  xception = exc..
+00003b90: 2020 2020 2020 2020 7468 7265 6164 203d          thread =
+00003ba0: 2054 6872 6561 6428 7461 7267 6574 3d73   Thread(target=s
+00003bb0: 6572 7665 2c20 6461 656d 6f6e 3d54 7275  erve, daemon=Tru
+00003bc0: 6529 0a20 2020 2020 2020 2074 6872 6561  e).        threa
+00003bd0: 642e 7374 6172 7428 290a 2020 2020 2020  d.start().      
+00003be0: 2020 7769 7468 2070 7974 6573 742e 7261    with pytest.ra
+00003bf0: 6973 6573 2853 534c 4572 726f 7229 3a0a  ises(SSLError):.
+00003c00: 2020 2020 2020 2020 2020 2020 6177 6169              awai
+00003c10: 7420 636f 6e6e 6563 745f 7463 7028 2a73  t connect_tcp(*s
+00003c20: 6572 7665 725f 6164 6472 2c20 746c 735f  erver_addr, tls_
+00003c30: 686f 7374 6e61 6d65 3d22 6c6f 6361 6c68  hostname="localh
+00003c40: 6f73 7422 290a 0a20 2020 2020 2020 2074  ost")..        t
+00003c50: 6872 6561 642e 6a6f 696e 2829 0a20 2020  hread.join().   
+00003c60: 2020 2020 2061 7373 6572 7420 7468 7265       assert thre
+00003c70: 6164 5f65 7863 6570 7469 6f6e 2069 7320  ad_exception is 
+00003c80: 4e6f 6e65 0a0a 2020 2020 4070 7974 6573  None..    @pytes
+00003c90: 742e 6d61 726b 2e70 6172 616d 6574 7269  t.mark.parametri
+00003ca0: 7a65 2822 616e 7969 6f5f 6261 636b 656e  ze("anyio_backen
+00003cb0: 6422 2c20 5b22 6173 796e 6369 6f22 5d29  d", ["asyncio"])
+00003cc0: 0a20 2020 2061 7379 6e63 2064 6566 2074  .    async def t
+00003cd0: 6573 745f 756e 7265 7472 6965 7665 645f  est_unretrieved_
+00003ce0: 6675 7475 7265 5f65 7863 6570 7469 6f6e  future_exception
+00003cf0: 5f73 6572 7665 725f 6372 6173 6828 0a20  _server_crash(. 
+00003d00: 2020 2020 2020 2073 656c 662c 2066 616d         self, fam
+00003d10: 696c 793a 2041 6e79 4950 4164 6472 6573  ily: AnyIPAddres
+00003d20: 7346 616d 696c 792c 2063 6170 6c6f 673a  sFamily, caplog:
+00003d30: 204c 6f67 4361 7074 7572 6546 6978 7475   LogCaptureFixtu
+00003d40: 7265 0a20 2020 2029 202d 3e20 4e6f 6e65  re.    ) -> None
+00003d50: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00003d60: 2020 2020 2020 5465 7374 2074 6861 7420        Test that 
+00003d70: 7468 6572 6520 776f 6e27 7420 6265 2061  there won't be a
+00003d80: 6e79 206c 6566 746f 7665 7220 4675 7475  ny leftover Futu
+00003d90: 7265 7320 7468 6174 2064 6f6e 2774 2067  res that don't g
+00003da0: 6574 2074 6865 6972 2065 7863 6570 7469  et their excepti
+00003db0: 6f6e 730a 2020 2020 2020 2020 7265 7472  ons.        retr
+00003dc0: 6965 7665 642e 0a0a 2020 2020 2020 2020  ieved...        
+00003dd0: 5365 6520 6874 7470 733a 2f2f 6769 7468  See https://gith
+00003de0: 7562 2e63 6f6d 2f65 6e63 6f64 652f 6874  ub.com/encode/ht
+00003df0: 7470 636f 7265 2f69 7373 7565 732f 3338  tpcore/issues/38
+00003e00: 3220 666f 7220 6465 7461 696c 732e 0a0a  2 for details...
+00003e10: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+00003e20: 2020 2020 2064 6566 2073 6572 7665 2829       def serve()
+00003e30: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00003e40: 2020 2020 2020 736f 636b 2c20 6164 6472        sock, addr
+00003e50: 203d 2073 6572 7665 725f 736f 636b 2e61   = server_sock.a
+00003e60: 6363 6570 7428 290a 2020 2020 2020 2020  ccept().        
+00003e70: 2020 2020 6576 656e 742e 7761 6974 2833      event.wait(3
+00003e80: 290a 2020 2020 2020 2020 2020 2020 6465  ).            de
+00003e90: 6c20 736f 636b 0a20 2020 2020 2020 2020  l sock.         
+00003ea0: 2020 2067 632e 636f 6c6c 6563 7428 290a     gc.collect().
+00003eb0: 0a20 2020 2020 2020 2073 6572 7665 725f  .        server_
+00003ec0: 736f 636b 203d 2073 6f63 6b65 742e 736f  sock = socket.so
+00003ed0: 636b 6574 2866 616d 696c 792c 2073 6f63  cket(family, soc
+00003ee0: 6b65 742e 534f 434b 5f53 5452 4541 4d29  ket.SOCK_STREAM)
+00003ef0: 0a20 2020 2020 2020 2073 6572 7665 725f  .        server_
+00003f00: 736f 636b 2e73 6574 7469 6d65 6f75 7428  sock.settimeout(
+00003f10: 3129 0a20 2020 2020 2020 2073 6572 7665  1).        serve
+00003f20: 725f 736f 636b 2e62 696e 6428 2822 6c6f  r_sock.bind(("lo
+00003f30: 6361 6c68 6f73 7422 2c20 3029 290a 2020  calhost", 0)).  
+00003f40: 2020 2020 2020 7365 7276 6572 5f73 6f63        server_soc
+00003f50: 6b2e 6c69 7374 656e 2829 0a20 2020 2020  k.listen().     
+00003f60: 2020 2073 6572 7665 725f 6164 6472 203d     server_addr =
+00003f70: 2073 6572 7665 725f 736f 636b 2e67 6574   server_sock.get
+00003f80: 736f 636b 6e61 6d65 2829 5b3a 325d 0a20  sockname()[:2]. 
+00003f90: 2020 2020 2020 2065 7665 6e74 203d 2074         event = t
+00003fa0: 6872 6561 6469 6e67 2e45 7665 6e74 2829  hreading.Event()
+00003fb0: 0a20 2020 2020 2020 2074 6872 6561 6420  .        thread 
+00003fc0: 3d20 5468 7265 6164 2874 6172 6765 743d  = Thread(target=
+00003fd0: 7365 7276 6529 0a20 2020 2020 2020 2074  serve).        t
+00003fe0: 6872 6561 642e 7374 6172 7428 290a 2020  hread.start().  
+00003ff0: 2020 2020 2020 6173 796e 6320 7769 7468        async with
+00004000: 2061 7761 6974 2063 6f6e 6e65 6374 5f74   await connect_t
+00004010: 6370 282a 7365 7276 6572 5f61 6464 7229  cp(*server_addr)
+00004020: 2061 7320 7374 7265 616d 3a0a 2020 2020   as stream:.    
+00004030: 2020 2020 2020 2020 6177 6169 7420 7374          await st
+00004040: 7265 616d 2e73 656e 6428 6222 4745 5422  ream.send(b"GET"
+00004050: 290a 2020 2020 2020 2020 2020 2020 6576  ).            ev
+00004060: 656e 742e 7365 7428 290a 2020 2020 2020  ent.set().      
+00004070: 2020 2020 2020 7769 7468 2070 7974 6573        with pytes
+00004080: 742e 7261 6973 6573 2842 726f 6b65 6e52  t.raises(BrokenR
+00004090: 6573 6f75 7263 6545 7272 6f72 293a 0a20  esourceError):. 
+000040a0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000040b0: 7761 6974 2073 7472 6561 6d2e 7265 6365  wait stream.rece
+000040c0: 6976 6528 290a 0a20 2020 2020 2020 2074  ive()..        t
+000040d0: 6872 6561 642e 6a6f 696e 2829 0a20 2020  hread.join().   
+000040e0: 2020 2020 2067 632e 636f 6c6c 6563 7428       gc.collect(
+000040f0: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
+00004100: 206e 6f74 2063 6170 6c6f 672e 7465 7874   not caplog.text
+00004110: 0a0a 0a40 7079 7465 7374 2e6d 6172 6b2e  ...@pytest.mark.
+00004120: 6e65 7477 6f72 6b0a 636c 6173 7320 5465  network.class Te
+00004130: 7374 5443 504c 6973 7465 6e65 723a 0a20  stTCPListener:. 
+00004140: 2020 2061 7379 6e63 2064 6566 2074 6573     async def tes
+00004150: 745f 6578 7472 615f 6174 7472 6962 7574  t_extra_attribut
+00004160: 6573 2873 656c 662c 2066 616d 696c 793a  es(self, family:
+00004170: 2041 6e79 4950 4164 6472 6573 7346 616d   AnyIPAddressFam
+00004180: 696c 7929 202d 3e20 4e6f 6e65 3a0a 2020  ily) -> None:.  
+00004190: 2020 2020 2020 6173 796e 6320 7769 7468        async with
+000041a0: 2061 7761 6974 2063 7265 6174 655f 7463   await create_tc
+000041b0: 705f 6c69 7374 656e 6572 280a 2020 2020  p_listener(.    
+000041c0: 2020 2020 2020 2020 6c6f 6361 6c5f 686f          local_ho
+000041d0: 7374 3d22 6c6f 6361 6c68 6f73 7422 2c20  st="localhost", 
+000041e0: 6661 6d69 6c79 3d66 616d 696c 790a 2020  family=family.  
+000041f0: 2020 2020 2020 2920 6173 206d 756c 7469        ) as multi
+00004200: 3a0a 2020 2020 2020 2020 2020 2020 6173  :.            as
+00004210: 7365 7274 206d 756c 7469 2e65 7874 7261  sert multi.extra
+00004220: 2853 6f63 6b65 7441 7474 7269 6275 7465  (SocketAttribute
+00004230: 2e66 616d 696c 7929 203d 3d20 6661 6d69  .family) == fami
+00004240: 6c79 0a20 2020 2020 2020 2020 2020 2066  ly.            f
+00004250: 6f72 206c 6973 7465 6e65 7220 696e 206d  or listener in m
+00004260: 756c 7469 2e6c 6973 7465 6e65 7273 3a0a  ulti.listeners:.
+00004270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004280: 7261 775f 736f 636b 6574 203d 206c 6973  raw_socket = lis
+00004290: 7465 6e65 722e 6578 7472 6128 536f 636b  tener.extra(Sock
+000042a0: 6574 4174 7472 6962 7574 652e 7261 775f  etAttribute.raw_
+000042b0: 736f 636b 6574 290a 2020 2020 2020 2020  socket).        
+000042c0: 2020 2020 2020 2020 6173 7365 7274 206c          assert l
+000042d0: 6973 7465 6e65 722e 6578 7472 6128 536f  istener.extra(So
+000042e0: 636b 6574 4174 7472 6962 7574 652e 6661  cketAttribute.fa
+000042f0: 6d69 6c79 2920 3d3d 2066 616d 696c 790a  mily) == family.
+00004300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004310: 6173 7365 7274 2028 0a20 2020 2020 2020  assert (.       
+00004320: 2020 2020 2020 2020 2020 2020 206c 6973               lis
+00004330: 7465 6e65 722e 6578 7472 6128 536f 636b  tener.extra(Sock
+00004340: 6574 4174 7472 6962 7574 652e 6c6f 6361  etAttribute.loca
+00004350: 6c5f 6164 6472 6573 7329 0a20 2020 2020  l_address).     
+00004360: 2020 2020 2020 2020 2020 2020 2020 203d                 =
+00004370: 3d20 7261 775f 736f 636b 6574 2e67 6574  = raw_socket.get
+00004380: 736f 636b 6e61 6d65 2829 5b3a 325d 0a20  sockname()[:2]. 
+00004390: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+000043a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000043b0: 2061 7373 6572 7420 280a 2020 2020 2020   assert (.      
+000043c0: 2020 2020 2020 2020 2020 2020 2020 6c69                li
+000043d0: 7374 656e 6572 2e65 7874 7261 2853 6f63  stener.extra(Soc
+000043e0: 6b65 7441 7474 7269 6275 7465 2e6c 6f63  ketAttribute.loc
+000043f0: 616c 5f70 6f72 7429 0a20 2020 2020 2020  al_port).       
+00004400: 2020 2020 2020 2020 2020 2020 203d 3d20               == 
+00004410: 7261 775f 736f 636b 6574 2e67 6574 736f  raw_socket.getso
+00004420: 636b 6e61 6d65 2829 5b31 5d0a 2020 2020  ckname()[1].    
+00004430: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00004440: 2020 2020 2020 2020 2020 2020 2020 7079                py
+00004450: 7465 7374 2e72 6169 7365 7328 0a20 2020  test.raises(.   
+00004460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004470: 2054 7970 6564 4174 7472 6962 7574 654c   TypedAttributeL
+00004480: 6f6f 6b75 7045 7272 6f72 2c0a 2020 2020  ookupError,.    
+00004490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044a0: 6c69 7374 656e 6572 2e65 7874 7261 2c0a  listener.extra,.
+000044b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044c0: 2020 2020 536f 636b 6574 4174 7472 6962      SocketAttrib
+000044d0: 7574 652e 7265 6d6f 7465 5f61 6464 7265  ute.remote_addre
+000044e0: 7373 2c0a 2020 2020 2020 2020 2020 2020  ss,.            
+000044f0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00004500: 2020 2020 2020 7079 7465 7374 2e72 6169        pytest.rai
+00004510: 7365 7328 0a20 2020 2020 2020 2020 2020  ses(.           
+00004520: 2020 2020 2020 2020 2054 7970 6564 4174           TypedAt
+00004530: 7472 6962 7574 654c 6f6f 6b75 7045 7272  tributeLookupErr
+00004540: 6f72 2c0a 2020 2020 2020 2020 2020 2020  or,.            
+00004550: 2020 2020 2020 2020 6c69 7374 656e 6572          listener
+00004560: 2e65 7874 7261 2c0a 2020 2020 2020 2020  .extra,.        
+00004570: 2020 2020 2020 2020 2020 2020 536f 636b              Sock
+00004580: 6574 4174 7472 6962 7574 652e 7265 6d6f  etAttribute.remo
+00004590: 7465 5f70 6f72 742c 0a20 2020 2020 2020  te_port,.       
+000045a0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+000045b0: 4070 7974 6573 742e 6d61 726b 2e70 6172  @pytest.mark.par
+000045c0: 616d 6574 7269 7a65 280a 2020 2020 2020  ametrize(.      
+000045d0: 2020 2266 616d 696c 7922 2c0a 2020 2020    "family",.    
+000045e0: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
+000045f0: 2020 7079 7465 7374 2e70 6172 616d 2841    pytest.param(A
+00004600: 6464 7265 7373 4661 6d69 6c79 2e41 465f  ddressFamily.AF_
+00004610: 494e 4554 2c20 6964 3d22 6970 7634 2229  INET, id="ipv4")
+00004620: 2c0a 2020 2020 2020 2020 2020 2020 7079  ,.            py
+00004630: 7465 7374 2e70 6172 616d 2841 6464 7265  test.param(Addre
+00004640: 7373 4661 6d69 6c79 2e41 465f 494e 4554  ssFamily.AF_INET
+00004650: 362c 2069 643d 2269 7076 3622 2c20 6d61  6, id="ipv6", ma
+00004660: 726b 733d 5b73 6b69 705f 6970 7636 5f6d  rks=[skip_ipv6_m
+00004670: 6172 6b5d 292c 0a20 2020 2020 2020 2020  ark]),.         
+00004680: 2020 2070 7974 6573 742e 7061 7261 6d28     pytest.param(
+00004690: 736f 636b 6574 2e41 465f 554e 5350 4543  socket.AF_UNSPEC
+000046a0: 2c20 6964 3d22 626f 7468 222c 206d 6172  , id="both", mar
+000046b0: 6b73 3d5b 736b 6970 5f69 7076 365f 6d61  ks=[skip_ipv6_ma
+000046c0: 726b 5d29 2c0a 2020 2020 2020 2020 5d2c  rk]),.        ],
+000046d0: 0a20 2020 2029 0a20 2020 2061 7379 6e63  .    ).    async
+000046e0: 2064 6566 2074 6573 745f 6163 6365 7074   def test_accept
+000046f0: 2873 656c 662c 2066 616d 696c 793a 2041  (self, family: A
+00004700: 6e79 4950 4164 6472 6573 7346 616d 696c  nyIPAddressFamil
+00004710: 7929 202d 3e20 4e6f 6e65 3a0a 2020 2020  y) -> None:.    
+00004720: 2020 2020 6173 796e 6320 7769 7468 2061      async with a
+00004730: 7761 6974 2063 7265 6174 655f 7463 705f  wait create_tcp_
+00004740: 6c69 7374 656e 6572 280a 2020 2020 2020  listener(.      
+00004750: 2020 2020 2020 6c6f 6361 6c5f 686f 7374        local_host
+00004760: 3d22 6c6f 6361 6c68 6f73 7422 2c20 6661  ="localhost", fa
+00004770: 6d69 6c79 3d66 616d 696c 790a 2020 2020  mily=family.    
+00004780: 2020 2020 2920 6173 206d 756c 7469 3a0a      ) as multi:.
+00004790: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000047a0: 6c69 7374 656e 6572 2069 6e20 6d75 6c74  listener in mult
+000047b0: 692e 6c69 7374 656e 6572 733a 0a20 2020  i.listeners:.   
+000047c0: 2020 2020 2020 2020 2020 2020 2063 6c69               cli
+000047d0: 656e 7420 3d20 736f 636b 6574 2e73 6f63  ent = socket.soc
+000047e0: 6b65 7428 6c69 7374 656e 6572 2e65 7874  ket(listener.ext
+000047f0: 7261 2853 6f63 6b65 7441 7474 7269 6275  ra(SocketAttribu
+00004800: 7465 2e66 616d 696c 7929 290a 2020 2020  te.family)).    
+00004810: 2020 2020 2020 2020 2020 2020 636c 6965              clie
+00004820: 6e74 2e73 6574 7469 6d65 6f75 7428 3129  nt.settimeout(1)
+00004830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004840: 2063 6c69 656e 742e 636f 6e6e 6563 7428   client.connect(
+00004850: 6c69 7374 656e 6572 2e65 7874 7261 2853  listener.extra(S
+00004860: 6f63 6b65 7441 7474 7269 6275 7465 2e6c  ocketAttribute.l
+00004870: 6f63 616c 5f61 6464 7265 7373 2929 0a20  ocal_address)). 
+00004880: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00004890: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
+000048a0: 286c 6973 7465 6e65 722c 2053 6f63 6b65  (listener, Socke
+000048b0: 744c 6973 7465 6e65 7229 0a20 2020 2020  tListener).     
+000048c0: 2020 2020 2020 2020 2020 2073 7472 6561             strea
+000048d0: 6d20 3d20 6177 6169 7420 6c69 7374 656e  m = await listen
+000048e0: 6572 2e61 6363 6570 7428 290a 2020 2020  er.accept().    
+000048f0: 2020 2020 2020 2020 2020 2020 636c 6965              clie
+00004900: 6e74 2e73 656e 6461 6c6c 2862 2262 6c61  nt.sendall(b"bla
+00004910: 6822 290a 2020 2020 2020 2020 2020 2020  h").            
+00004920: 2020 2020 7265 7175 6573 7420 3d20 6177      request = aw
+00004930: 6169 7420 7374 7265 616d 2e72 6563 6569  ait stream.recei
+00004940: 7665 2829 0a20 2020 2020 2020 2020 2020  ve().           
+00004950: 2020 2020 2061 7761 6974 2073 7472 6561       await strea
+00004960: 6d2e 7365 6e64 2872 6571 7565 7374 5b3a  m.send(request[:
+00004970: 3a2d 315d 290a 2020 2020 2020 2020 2020  :-1]).          
+00004980: 2020 2020 2020 6173 7365 7274 2063 6c69        assert cli
+00004990: 656e 742e 7265 6376 2831 3030 2920 3d3d  ent.recv(100) ==
+000049a0: 2062 2268 616c 6222 0a20 2020 2020 2020   b"halb".       
+000049b0: 2020 2020 2020 2020 2063 6c69 656e 742e           client.
+000049c0: 636c 6f73 6528 290a 2020 2020 2020 2020  close().        
+000049d0: 2020 2020 2020 2020 6177 6169 7420 7374          await st
+000049e0: 7265 616d 2e61 636c 6f73 6528 290a 0a20  ream.aclose().. 
+000049f0: 2020 2061 7379 6e63 2064 6566 2074 6573     async def tes
+00004a00: 745f 6163 6365 7074 5f61 6674 6572 5f63  t_accept_after_c
+00004a10: 6c6f 7365 2873 656c 662c 2066 616d 696c  lose(self, famil
+00004a20: 793a 2041 6e79 4950 4164 6472 6573 7346  y: AnyIPAddressF
+00004a30: 616d 696c 7929 202d 3e20 4e6f 6e65 3a0a  amily) -> None:.
+00004a40: 2020 2020 2020 2020 6173 796e 6320 7769          async wi
+00004a50: 7468 2061 7761 6974 2063 7265 6174 655f  th await create_
+00004a60: 7463 705f 6c69 7374 656e 6572 280a 2020  tcp_listener(.  
+00004a70: 2020 2020 2020 2020 2020 6c6f 6361 6c5f            local_
+00004a80: 686f 7374 3d22 6c6f 6361 6c68 6f73 7422  host="localhost"
+00004a90: 2c20 6661 6d69 6c79 3d66 616d 696c 790a  , family=family.
+00004aa0: 2020 2020 2020 2020 2920 6173 206d 756c          ) as mul
+00004ab0: 7469 3a0a 2020 2020 2020 2020 2020 2020  ti:.            
+00004ac0: 666f 7220 6c69 7374 656e 6572 2069 6e20  for listener in 
+00004ad0: 6d75 6c74 692e 6c69 7374 656e 6572 733a  multi.listeners:
+00004ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004af0: 2061 7761 6974 206c 6973 7465 6e65 722e   await listener.
+00004b00: 6163 6c6f 7365 2829 0a20 2020 2020 2020  aclose().       
+00004b10: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+00004b20: 6973 696e 7374 616e 6365 286c 6973 7465  isinstance(liste
+00004b30: 6e65 722c 2053 6f63 6b65 744c 6973 7465  ner, SocketListe
+00004b40: 6e65 7229 0a20 2020 2020 2020 2020 2020  ner).           
+00004b50: 2020 2020 2077 6974 6820 7079 7465 7374       with pytest
+00004b60: 2e72 6169 7365 7328 436c 6f73 6564 5265  .raises(ClosedRe
+00004b70: 736f 7572 6365 4572 726f 7229 3a0a 2020  sourceError):.  
+00004b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b90: 2020 6177 6169 7420 6c69 7374 656e 6572    await listener
+00004ba0: 2e61 6363 6570 7428 290a 0a20 2020 2061  .accept()..    a
+00004bb0: 7379 6e63 2064 6566 2074 6573 745f 736f  sync def test_so
+00004bc0: 636b 6574 5f6f 7074 696f 6e73 2873 656c  cket_options(sel
+00004bd0: 662c 2066 616d 696c 793a 2041 6e79 4950  f, family: AnyIP
+00004be0: 4164 6472 6573 7346 616d 696c 7929 202d  AddressFamily) -
+00004bf0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00004c00: 6173 796e 6320 7769 7468 2061 7761 6974  async with await
+00004c10: 2063 7265 6174 655f 7463 705f 6c69 7374   create_tcp_list
+00004c20: 656e 6572 280a 2020 2020 2020 2020 2020  ener(.          
+00004c30: 2020 6c6f 6361 6c5f 686f 7374 3d22 6c6f    local_host="lo
+00004c40: 6361 6c68 6f73 7422 2c20 6661 6d69 6c79  calhost", family
+00004c50: 3d66 616d 696c 790a 2020 2020 2020 2020  =family.        
+00004c60: 2920 6173 206d 756c 7469 3a0a 2020 2020  ) as multi:.    
+00004c70: 2020 2020 2020 2020 666f 7220 6c69 7374          for list
+00004c80: 656e 6572 2069 6e20 6d75 6c74 692e 6c69  ener in multi.li
+00004c90: 7374 656e 6572 733a 0a20 2020 2020 2020  steners:.       
+00004ca0: 2020 2020 2020 2020 2072 6177 5f73 6f63           raw_soc
+00004cb0: 6b65 7420 3d20 6c69 7374 656e 6572 2e65  ket = listener.e
+00004cc0: 7874 7261 2853 6f63 6b65 7441 7474 7269  xtra(SocketAttri
+00004cd0: 6275 7465 2e72 6177 5f73 6f63 6b65 7429  bute.raw_socket)
+00004ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004cf0: 2069 6620 7379 732e 706c 6174 666f 726d   if sys.platform
+00004d00: 203d 3d20 2277 696e 3332 223a 0a20 2020   == "win32":.   
+00004d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d20: 2061 7373 6572 7420 280a 2020 2020 2020   assert (.      
+00004d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d40: 2020 7261 775f 736f 636b 6574 2e67 6574    raw_socket.get
+00004d50: 736f 636b 6f70 7428 0a20 2020 2020 2020  sockopt(.       
+00004d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d70: 2020 2020 2073 6f63 6b65 742e 534f 4c5f       socket.SOL_
+00004d80: 534f 434b 4554 2c20 736f 636b 6574 2e53  SOCKET, socket.S
+00004d90: 4f5f 4558 434c 5553 4956 4541 4444 5255  O_EXCLUSIVEADDRU
+00004da0: 5345 0a20 2020 2020 2020 2020 2020 2020  SE.             
+00004db0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00004dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004dd0: 2020 2020 2021 3d20 300a 2020 2020 2020       != 0.      
+00004de0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00004df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e00: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00004e10: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+00004e20: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00004e30: 2020 2020 2020 2020 2020 2072 6177 5f73             raw_s
+00004e40: 6f63 6b65 742e 6765 7473 6f63 6b6f 7074  ocket.getsockopt
+00004e50: 2873 6f63 6b65 742e 534f 4c5f 534f 434b  (socket.SOL_SOCK
+00004e60: 4554 2c20 736f 636b 6574 2e53 4f5f 5245  ET, socket.SO_RE
+00004e70: 5553 4541 4444 5229 0a20 2020 2020 2020  USEADDR).       
+00004e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e90: 2021 3d20 300a 2020 2020 2020 2020 2020   != 0.          
+00004ea0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+00004eb0: 2020 2020 2020 2020 2020 2020 2072 6177               raw
+00004ec0: 5f73 6f63 6b65 742e 7365 7473 6f63 6b6f  _socket.setsocko
+00004ed0: 7074 2873 6f63 6b65 742e 534f 4c5f 534f  pt(socket.SOL_SO
+00004ee0: 434b 4554 2c20 736f 636b 6574 2e53 4f5f  CKET, socket.SO_
+00004ef0: 5243 5642 5546 2c20 3830 3030 3029 0a20  RCVBUF, 80000). 
+00004f00: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00004f10: 7373 6572 7420 7261 775f 736f 636b 6574  ssert raw_socket
+00004f20: 2e67 6574 736f 636b 6f70 7428 736f 636b  .getsockopt(sock
+00004f30: 6574 2e53 4f4c 5f53 4f43 4b45 542c 2073  et.SOL_SOCKET, s
+00004f40: 6f63 6b65 742e 534f 5f52 4356 4255 4629  ocket.SO_RCVBUF)
+00004f50: 2069 6e20 280a 2020 2020 2020 2020 2020   in (.          
+00004f60: 2020 2020 2020 2020 2020 3830 3030 302c            80000,
+00004f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004f80: 2020 2020 2031 3630 3030 302c 0a20 2020       160000,.   
+00004f90: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
+00004fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fb0: 636c 6965 6e74 203d 2073 6f63 6b65 742e  client = socket.
+00004fc0: 736f 636b 6574 2872 6177 5f73 6f63 6b65  socket(raw_socke
+00004fd0: 742e 6661 6d69 6c79 290a 2020 2020 2020  t.family).      
+00004fe0: 2020 2020 2020 2020 2020 636c 6965 6e74            client
+00004ff0: 2e73 6574 7469 6d65 6f75 7428 3129 0a20  .settimeout(1). 
+00005000: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00005010: 6c69 656e 742e 636f 6e6e 6563 7428 7261  lient.connect(ra
+00005020: 775f 736f 636b 6574 2e67 6574 736f 636b  w_socket.getsock
+00005030: 6e61 6d65 2829 290a 0a20 2020 2020 2020  name())..       
+00005040: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+00005050: 6973 696e 7374 616e 6365 286c 6973 7465  isinstance(liste
+00005060: 6e65 722c 2053 6f63 6b65 744c 6973 7465  ner, SocketListe
+00005070: 6e65 7229 0a20 2020 2020 2020 2020 2020  ner).           
+00005080: 2020 2020 2061 7379 6e63 2077 6974 6820       async with 
+00005090: 6177 6169 7420 6c69 7374 656e 6572 2e61  await listener.a
+000050a0: 6363 6570 7428 2920 6173 2073 7472 6561  ccept() as strea
+000050b0: 6d3a 0a20 2020 2020 2020 2020 2020 2020  m:.             
+000050c0: 2020 2020 2020 2072 6177 5f73 6f63 6b65         raw_socke
+000050d0: 7420 3d20 7374 7265 616d 2e65 7874 7261  t = stream.extra
+000050e0: 2853 6f63 6b65 7441 7474 7269 6275 7465  (SocketAttribute
+000050f0: 2e72 6177 5f73 6f63 6b65 7429 0a20 2020  .raw_socket).   
+00005100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005110: 2061 7373 6572 7420 7261 775f 736f 636b   assert raw_sock
+00005120: 6574 2e67 6574 7469 6d65 6f75 7428 2920  et.gettimeout() 
+00005130: 3d3d 2030 0a20 2020 2020 2020 2020 2020  == 0.           
+00005140: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+00005150: 7261 775f 736f 636b 6574 2e66 616d 696c  raw_socket.famil
+00005160: 7920 3d3d 206c 6973 7465 6e65 722e 6578  y == listener.ex
+00005170: 7472 6128 536f 636b 6574 4174 7472 6962  tra(SocketAttrib
+00005180: 7574 652e 6661 6d69 6c79 290a 2020 2020  ute.family).    
+00005190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051a0: 6173 7365 7274 2028 0a20 2020 2020 2020  assert (.       
+000051b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051c0: 2072 6177 5f73 6f63 6b65 742e 6765 7473   raw_socket.gets
+000051d0: 6f63 6b6f 7074 2873 6f63 6b65 742e 4950  ockopt(socket.IP
+000051e0: 5052 4f54 4f5f 5443 502c 2073 6f63 6b65  PROTO_TCP, socke
+000051f0: 742e 5443 505f 4e4f 4445 4c41 5929 0a20  t.TCP_NODELAY). 
+00005200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005210: 2020 2020 2020 2021 3d20 300a 2020 2020         != 0.    
+00005220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005230: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+00005240: 2020 2063 6c69 656e 742e 636c 6f73 6528     client.close(
+00005250: 290a 0a20 2020 2040 7079 7465 7374 2e6d  )..    @pytest.m
+00005260: 6172 6b2e 736b 6970 6966 280a 2020 2020  ark.skipif(.    
+00005270: 2020 2020 6e6f 7420 6861 7361 7474 7228      not hasattr(
+00005280: 736f 636b 6574 2c20 2253 4f5f 5245 5553  socket, "SO_REUS
+00005290: 4550 4f52 5422 292c 2072 6561 736f 6e3d  EPORT"), reason=
+000052a0: 2253 4f5f 5245 5553 4550 4f52 5420 6f70  "SO_REUSEPORT op
+000052b0: 7469 6f6e 206e 6f74 2073 7570 706f 7274  tion not support
+000052c0: 6564 220a 2020 2020 290a 2020 2020 6173  ed".    ).    as
+000052d0: 796e 6320 6465 6620 7465 7374 5f72 6575  ync def test_reu
+000052e0: 7365 5f70 6f72 7428 7365 6c66 2c20 6661  se_port(self, fa
+000052f0: 6d69 6c79 3a20 416e 7949 5041 6464 7265  mily: AnyIPAddre
+00005300: 7373 4661 6d69 6c79 2920 2d3e 204e 6f6e  ssFamily) -> Non
+00005310: 653a 0a20 2020 2020 2020 206d 756c 7469  e:.        multi
+00005320: 3120 3d20 6177 6169 7420 6372 6561 7465  1 = await create
+00005330: 5f74 6370 5f6c 6973 7465 6e65 7228 0a20  _tcp_listener(. 
+00005340: 2020 2020 2020 2020 2020 206c 6f63 616c             local
+00005350: 5f68 6f73 743d 226c 6f63 616c 686f 7374  _host="localhost
+00005360: 222c 2066 616d 696c 793d 6661 6d69 6c79  ", family=family
+00005370: 2c20 7265 7573 655f 706f 7274 3d54 7275  , reuse_port=Tru
+00005380: 650a 2020 2020 2020 2020 290a 2020 2020  e.        ).    
+00005390: 2020 2020 6173 7365 7274 206c 656e 286d      assert len(m
+000053a0: 756c 7469 312e 6c69 7374 656e 6572 7329  ulti1.listeners)
+000053b0: 203d 3d20 310a 0a20 2020 2020 2020 206d   == 1..        m
+000053c0: 756c 7469 3220 3d20 6177 6169 7420 6372  ulti2 = await cr
+000053d0: 6561 7465 5f74 6370 5f6c 6973 7465 6e65  eate_tcp_listene
+000053e0: 7228 0a20 2020 2020 2020 2020 2020 206c  r(.            l
+000053f0: 6f63 616c 5f68 6f73 743d 226c 6f63 616c  ocal_host="local
+00005400: 686f 7374 222c 0a20 2020 2020 2020 2020  host",.         
+00005410: 2020 206c 6f63 616c 5f70 6f72 743d 6d75     local_port=mu
+00005420: 6c74 6931 2e6c 6973 7465 6e65 7273 5b30  lti1.listeners[0
+00005430: 5d2e 6578 7472 6128 536f 636b 6574 4174  ].extra(SocketAt
+00005440: 7472 6962 7574 652e 6c6f 6361 6c5f 706f  tribute.local_po
+00005450: 7274 292c 0a20 2020 2020 2020 2020 2020  rt),.           
+00005460: 2066 616d 696c 793d 6661 6d69 6c79 2c0a   family=family,.
+00005470: 2020 2020 2020 2020 2020 2020 7265 7573              reus
+00005480: 655f 706f 7274 3d54 7275 652c 0a20 2020  e_port=True,.   
+00005490: 2020 2020 2029 0a20 2020 2020 2020 2061       ).        a
+000054a0: 7373 6572 7420 6c65 6e28 6d75 6c74 6932  ssert len(multi2
+000054b0: 2e6c 6973 7465 6e65 7273 2920 3d3d 2031  .listeners) == 1
+000054c0: 0a0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
+000054d0: 206d 756c 7469 312e 6c69 7374 656e 6572   multi1.listener
+000054e0: 735b 305d 2e65 7874 7261 280a 2020 2020  s[0].extra(.    
+000054f0: 2020 2020 2020 2020 536f 636b 6574 4174          SocketAt
+00005500: 7472 6962 7574 652e 6c6f 6361 6c5f 6164  tribute.local_ad
+00005510: 6472 6573 730a 2020 2020 2020 2020 2920  dress.        ) 
+00005520: 3d3d 206d 756c 7469 322e 6c69 7374 656e  == multi2.listen
+00005530: 6572 735b 305d 2e65 7874 7261 2853 6f63  ers[0].extra(Soc
+00005540: 6b65 7441 7474 7269 6275 7465 2e6c 6f63  ketAttribute.loc
+00005550: 616c 5f61 6464 7265 7373 290a 2020 2020  al_address).    
+00005560: 2020 2020 6177 6169 7420 6d75 6c74 6931      await multi1
+00005570: 2e61 636c 6f73 6528 290a 2020 2020 2020  .aclose().      
+00005580: 2020 6177 6169 7420 6d75 6c74 6932 2e61    await multi2.a
+00005590: 636c 6f73 6528 290a 0a20 2020 2061 7379  close()..    asy
+000055a0: 6e63 2064 6566 2074 6573 745f 636c 6f73  nc def test_clos
+000055b0: 655f 6672 6f6d 5f6f 7468 6572 5f74 6173  e_from_other_tas
+000055c0: 6b28 7365 6c66 2c20 6661 6d69 6c79 3a20  k(self, family: 
+000055d0: 416e 7949 5041 6464 7265 7373 4661 6d69  AnyIPAddressFami
+000055e0: 6c79 2920 2d3e 204e 6f6e 653a 0a20 2020  ly) -> None:.   
+000055f0: 2020 2020 206c 6973 7465 6e65 7220 3d20       listener = 
+00005600: 6177 6169 7420 6372 6561 7465 5f74 6370  await create_tcp
+00005610: 5f6c 6973 7465 6e65 7228 6c6f 6361 6c5f  _listener(local_
+00005620: 686f 7374 3d22 6c6f 6361 6c68 6f73 7422  host="localhost"
+00005630: 2c20 6661 6d69 6c79 3d66 616d 696c 7929  , family=family)
+00005640: 0a20 2020 2020 2020 2077 6974 6820 7079  .        with py
+00005650: 7465 7374 2e72 6169 7365 7328 4578 6365  test.raises(Exce
+00005660: 7074 696f 6e47 726f 7570 2920 6173 2065  ptionGroup) as e
+00005670: 7863 3a0a 2020 2020 2020 2020 2020 2020  xc:.            
+00005680: 6173 796e 6320 7769 7468 2063 7265 6174  async with creat
+00005690: 655f 7461 736b 5f67 726f 7570 2829 2061  e_task_group() a
+000056a0: 7320 7467 3a0a 2020 2020 2020 2020 2020  s tg:.          
+000056b0: 2020 2020 2020 7467 2e73 7461 7274 5f73        tg.start_s
+000056c0: 6f6f 6e28 6c69 7374 656e 6572 2e73 6572  oon(listener.ser
+000056d0: 7665 2c20 6c61 6d62 6461 2073 7472 6561  ve, lambda strea
+000056e0: 6d3a 204e 6f6e 6529 0a20 2020 2020 2020  m: None).       
+000056f0: 2020 2020 2020 2020 2061 7761 6974 2077           await w
+00005700: 6169 745f 616c 6c5f 7461 736b 735f 626c  ait_all_tasks_bl
+00005710: 6f63 6b65 6428 290a 2020 2020 2020 2020  ocked().        
+00005720: 2020 2020 2020 2020 6177 6169 7420 6c69          await li
+00005730: 7374 656e 6572 2e61 636c 6f73 6528 290a  stener.aclose().
+00005740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005750: 7467 2e63 616e 6365 6c5f 7363 6f70 652e  tg.cancel_scope.
+00005760: 6361 6e63 656c 2829 0a0a 2020 2020 2020  cancel()..      
+00005770: 2020 6173 7365 7274 206c 656e 2865 7863    assert len(exc
+00005780: 2e76 616c 7565 2e65 7863 6570 7469 6f6e  .value.exception
+00005790: 7329 203d 3d20 310a 2020 2020 2020 2020  s) == 1.        
+000057a0: 6173 7365 7274 2069 7369 6e73 7461 6e63  assert isinstanc
+000057b0: 6528 6578 632e 7661 6c75 652e 6578 6365  e(exc.value.exce
+000057c0: 7074 696f 6e73 5b30 5d2c 2045 7863 6570  ptions[0], Excep
+000057d0: 7469 6f6e 4772 6f75 7029 0a20 2020 2020  tionGroup).     
+000057e0: 2020 206e 6573 7465 645f 6772 7020 3d20     nested_grp = 
+000057f0: 6578 632e 7661 6c75 652e 6578 6365 7074  exc.value.except
+00005800: 696f 6e73 5b30 5d0a 2020 2020 2020 2020  ions[0].        
+00005810: 6173 7365 7274 206c 656e 286e 6573 7465  assert len(neste
+00005820: 645f 6772 702e 6578 6365 7074 696f 6e73  d_grp.exceptions
+00005830: 2920 3d3d 2031 0a20 2020 2020 2020 2061  ) == 1.        a
+00005840: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
+00005850: 286e 6573 7465 645f 6772 702e 6578 6365  (nested_grp.exce
+00005860: 7074 696f 6e73 5b30 5d2c 2045 7863 6570  ptions[0], Excep
+00005870: 7469 6f6e 4772 6f75 7029 0a0a 2020 2020  tionGroup)..    
+00005880: 6173 796e 6320 6465 6620 7465 7374 5f73  async def test_s
+00005890: 656e 645f 6166 7465 725f 656f 6628 7365  end_after_eof(se
+000058a0: 6c66 2c20 6661 6d69 6c79 3a20 416e 7949  lf, family: AnyI
+000058b0: 5041 6464 7265 7373 4661 6d69 6c79 2920  PAddressFamily) 
+000058c0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+000058d0: 2061 7379 6e63 2064 6566 2068 616e 646c   async def handl
+000058e0: 6528 7374 7265 616d 3a20 536f 636b 6574  e(stream: Socket
+000058f0: 5374 7265 616d 2920 2d3e 204e 6f6e 653a  Stream) -> None:
+00005900: 0a20 2020 2020 2020 2020 2020 2061 7379  .            asy
+00005910: 6e63 2077 6974 6820 7374 7265 616d 3a0a  nc with stream:.
+00005920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005930: 6177 6169 7420 7374 7265 616d 2e73 656e  await stream.sen
+00005940: 6428 6222 4865 6c6c 6f5c 6e22 290a 0a20  d(b"Hello\n").. 
+00005950: 2020 2020 2020 206d 756c 7469 203d 2061         multi = a
+00005960: 7761 6974 2063 7265 6174 655f 7463 705f  wait create_tcp_
+00005970: 6c69 7374 656e 6572 2866 616d 696c 793d  listener(family=
+00005980: 6661 6d69 6c79 2c20 6c6f 6361 6c5f 686f  family, local_ho
+00005990: 7374 3d22 6c6f 6361 6c68 6f73 7422 290a  st="localhost").
+000059a0: 2020 2020 2020 2020 6173 796e 6320 7769          async wi
+000059b0: 7468 206d 756c 7469 2c20 6372 6561 7465  th multi, create
+000059c0: 5f74 6173 6b5f 6772 6f75 7028 2920 6173  _task_group() as
+000059d0: 2074 673a 0a20 2020 2020 2020 2020 2020   tg:.           
+000059e0: 2074 672e 7374 6172 745f 736f 6f6e 286d   tg.start_soon(m
+000059f0: 756c 7469 2e73 6572 7665 2c20 6861 6e64  ulti.serve, hand
+00005a00: 6c65 290a 2020 2020 2020 2020 2020 2020  le).            
+00005a10: 6177 6169 7420 7761 6974 5f61 6c6c 5f74  await wait_all_t
+00005a20: 6173 6b73 5f62 6c6f 636b 6564 2829 0a0a  asks_blocked()..
+00005a30: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00005a40: 2073 6f63 6b65 742e 736f 636b 6574 2866   socket.socket(f
+00005a50: 616d 696c 7929 2061 7320 636c 6965 6e74  amily) as client
+00005a60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00005a70: 2020 636c 6965 6e74 2e63 6f6e 6e65 6374    client.connect
+00005a80: 286d 756c 7469 2e65 7874 7261 2853 6f63  (multi.extra(Soc
+00005a90: 6b65 7441 7474 7269 6275 7465 2e6c 6f63  ketAttribute.loc
+00005aa0: 616c 5f61 6464 7265 7373 2929 0a20 2020  al_address)).   
+00005ab0: 2020 2020 2020 2020 2020 2020 2063 6c69               cli
+00005ac0: 656e 742e 7368 7574 646f 776e 2873 6f63  ent.shutdown(soc
+00005ad0: 6b65 742e 5348 5554 5f57 5229 0a20 2020  ket.SHUT_WR).   
+00005ae0: 2020 2020 2020 2020 2020 2020 2063 6c69               cli
+00005af0: 656e 742e 7365 7462 6c6f 636b 696e 6728  ent.setblocking(
+00005b00: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
+00005b10: 2020 2020 2020 2077 6974 6820 6661 696c         with fail
+00005b20: 5f61 6674 6572 2831 293a 0a20 2020 2020  _after(1):.     
+00005b30: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00005b40: 6869 6c65 2054 7275 653a 0a20 2020 2020  hile True:.     
+00005b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b60: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00005b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b80: 2020 2020 6d65 7373 6167 6520 3d20 636c      message = cl
+00005b90: 6965 6e74 2e72 6563 7628 3130 290a 2020  ient.recv(10).  
+00005ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005bb0: 2020 2020 2020 6578 6365 7074 2042 6c6f        except Blo
+00005bc0: 636b 696e 6749 4f45 7272 6f72 3a0a 2020  ckingIOError:.  
+00005bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005be0: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+00005bf0: 736c 6565 7028 3029 0a20 2020 2020 2020  sleep(0).       
+00005c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c10: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00005c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c30: 2020 2061 7373 6572 7420 6d65 7373 6167     assert messag
+00005c40: 6520 3d3d 2062 2248 656c 6c6f 5c6e 220a  e == b"Hello\n".
+00005c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c60: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+00005c70: 6b0a 0a20 2020 2020 2020 2020 2020 2074  k..            t
+00005c80: 672e 6361 6e63 656c 5f73 636f 7065 2e63  g.cancel_scope.c
+00005c90: 616e 6365 6c28 290a 0a20 2020 2061 7379  ancel()..    asy
+00005ca0: 6e63 2064 6566 2074 6573 745f 656f 665f  nc def test_eof_
+00005cb0: 6166 7465 725f 7365 6e64 2873 656c 662c  after_send(self,
+00005cc0: 2066 616d 696c 793a 2041 6e79 4950 4164   family: AnyIPAd
+00005cd0: 6472 6573 7346 616d 696c 7929 202d 3e20  dressFamily) -> 
+00005ce0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00005cf0: 2252 6567 7265 7373 696f 6e20 7465 7374  "Regression test
+00005d00: 2066 6f72 2023 3730 312e 2222 220a 2020   for #701.""".  
+00005d10: 2020 2020 2020 7265 6365 6976 6564 5f62        received_b
+00005d20: 7974 6573 203d 2062 2222 0a0a 2020 2020  ytes = b""..    
+00005d30: 2020 2020 6173 796e 6320 6465 6620 6861      async def ha
+00005d40: 6e64 6c65 2873 7472 6561 6d3a 2053 6f63  ndle(stream: Soc
+00005d50: 6b65 7453 7472 6561 6d29 202d 3e20 4e6f  ketStream) -> No
+00005d60: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00005d70: 6e6f 6e6c 6f63 616c 2072 6563 6569 7665  nonlocal receive
+00005d80: 645f 6279 7465 730a 2020 2020 2020 2020  d_bytes.        
+00005d90: 2020 2020 6173 796e 6320 7769 7468 2073      async with s
+00005da0: 7472 6561 6d3a 0a20 2020 2020 2020 2020  tream:.         
+00005db0: 2020 2020 2020 2072 6563 6569 7665 645f         received_
+00005dc0: 6279 7465 7320 3d20 6177 6169 7420 7374  bytes = await st
+00005dd0: 7265 616d 2e72 6563 6569 7665 2829 0a20  ream.receive(). 
+00005de0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00005df0: 6974 6820 7079 7465 7374 2e72 6169 7365  ith pytest.raise
+00005e00: 7328 456e 644f 6653 7472 6561 6d29 2c20  s(EndOfStream), 
+00005e10: 6661 696c 5f61 6674 6572 2831 293a 0a20  fail_after(1):. 
+00005e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e30: 2020 2061 7761 6974 2073 7472 6561 6d2e     await stream.
+00005e40: 7265 6365 6976 6528 290a 0a20 2020 2020  receive()..     
+00005e50: 2020 2020 2020 2074 672e 6361 6e63 656c         tg.cancel
+00005e60: 5f73 636f 7065 2e63 616e 6365 6c28 290a  _scope.cancel().
+00005e70: 0a20 2020 2020 2020 206d 756c 7469 203d  .        multi =
+00005e80: 2061 7761 6974 2063 7265 6174 655f 7463   await create_tc
+00005e90: 705f 6c69 7374 656e 6572 2866 616d 696c  p_listener(famil
+00005ea0: 793d 6661 6d69 6c79 2c20 6c6f 6361 6c5f  y=family, local_
+00005eb0: 686f 7374 3d22 6c6f 6361 6c68 6f73 7422  host="localhost"
+00005ec0: 290a 2020 2020 2020 2020 6173 796e 6320  ).        async 
+00005ed0: 7769 7468 206d 756c 7469 2c20 6372 6561  with multi, crea
+00005ee0: 7465 5f74 6173 6b5f 6772 6f75 7028 2920  te_task_group() 
+00005ef0: 6173 2074 673a 0a20 2020 2020 2020 2020  as tg:.         
+00005f00: 2020 2077 6974 6820 736f 636b 6574 2e73     with socket.s
+00005f10: 6f63 6b65 7428 6661 6d69 6c79 2920 6173  ocket(family) as
+00005f20: 2063 6c69 656e 743a 0a20 2020 2020 2020   client:.       
+00005f30: 2020 2020 2020 2020 2063 6c69 656e 742e           client.
+00005f40: 636f 6e6e 6563 7428 6d75 6c74 692e 6578  connect(multi.ex
+00005f50: 7472 6128 536f 636b 6574 4174 7472 6962  tra(SocketAttrib
+00005f60: 7574 652e 6c6f 6361 6c5f 6164 6472 6573  ute.local_addres
+00005f70: 7329 290a 2020 2020 2020 2020 2020 2020  s)).            
+00005f80: 2020 2020 636c 6965 6e74 2e73 656e 6428      client.send(
+00005f90: 6222 4865 6c6c 6f22 290a 2020 2020 2020  b"Hello").      
+00005fa0: 2020 2020 2020 2020 2020 636c 6965 6e74            client
+00005fb0: 2e73 6875 7464 6f77 6e28 736f 636b 6574  .shutdown(socket
+00005fc0: 2e53 4855 545f 5752 290a 2020 2020 2020  .SHUT_WR).      
+00005fd0: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+00005fe0: 6d75 6c74 692e 7365 7276 6528 6861 6e64  multi.serve(hand
+00005ff0: 6c65 290a 0a20 2020 2020 2020 2061 7373  le)..        ass
+00006000: 6572 7420 7265 6365 6976 6564 5f62 7974  ert received_byt
+00006010: 6573 203d 3d20 6222 4865 6c6c 6f22 0a0a  es == b"Hello"..
+00006020: 2020 2020 4073 6b69 705f 6970 7636 5f6d      @skip_ipv6_m
+00006030: 6172 6b0a 2020 2020 4070 7974 6573 742e  ark.    @pytest.
+00006040: 6d61 726b 2e73 6b69 7069 6628 0a20 2020  mark.skipif(.   
+00006050: 2020 2020 2073 7973 2e70 6c61 7466 6f72       sys.platfor
+00006060: 6d20 3d3d 2022 7769 6e33 3222 2c0a 2020  m == "win32",.  
+00006070: 2020 2020 2020 7265 6173 6f6e 3d22 5769        reason="Wi
+00006080: 6e64 6f77 7320 646f 6573 206e 6f74 2073  ndows does not s
+00006090: 7570 706f 7274 2069 6e74 6572 6661 6365  upport interface
+000060a0: 206e 616d 6520 7375 6666 6978 6573 222c   name suffixes",
+000060b0: 0a20 2020 2029 0a20 2020 2061 7379 6e63  .    ).    async
+000060c0: 2064 6566 2074 6573 745f 6269 6e64 5f6c   def test_bind_l
+000060d0: 696e 6b5f 6c6f 6361 6c28 7365 6c66 2920  ink_local(self) 
+000060e0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+000060f0: 2023 2052 6567 7265 7373 696f 6e20 7465   # Regression te
+00006100: 7374 2066 6f72 2023 3535 340a 2020 2020  st for #554.    
+00006110: 2020 2020 6c69 6e6b 5f6c 6f63 616c 5f69      link_local_i
+00006120: 7076 365f 6164 6472 6573 7320 3d20 6e65  pv6_address = ne
+00006130: 7874 280a 2020 2020 2020 2020 2020 2020  xt(.            
+00006140: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00006150: 2020 6164 6472 2e61 6464 7265 7373 0a20    addr.address. 
+00006160: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00006170: 6f72 2061 6464 7265 7373 6573 2069 6e20  or addresses in 
+00006180: 7073 7574 696c 2e6e 6574 5f69 665f 6164  psutil.net_if_ad
+00006190: 6472 7328 292e 7661 6c75 6573 2829 0a20  drs().values(). 
+000061a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000061b0: 6f72 2061 6464 7220 696e 2061 6464 7265  or addr in addre
+000061c0: 7373 6573 0a20 2020 2020 2020 2020 2020  sses.           
+000061d0: 2020 2020 2069 6620 6164 6472 2e61 6464       if addr.add
+000061e0: 7265 7373 2e73 7461 7274 7377 6974 6828  ress.startswith(
+000061f0: 2266 6538 303a 3a22 2920 616e 6420 2225  "fe80::") and "%
+00006200: 2220 696e 2061 6464 722e 6164 6472 6573  " in addr.addres
+00006210: 730a 2020 2020 2020 2020 2020 2020 292c  s.            ),
+00006220: 0a20 2020 2020 2020 2020 2020 204e 6f6e  .            Non
+00006230: 652c 0a20 2020 2020 2020 2029 0a20 2020  e,.        ).   
+00006240: 2020 2020 2069 6620 6c69 6e6b 5f6c 6f63       if link_loc
+00006250: 616c 5f69 7076 365f 6164 6472 6573 7320  al_ipv6_address 
+00006260: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00006270: 2020 2020 2070 7974 6573 742e 6661 696c       pytest.fail
+00006280: 2822 436f 756c 6420 6e6f 7420 6669 6e64  ("Could not find
+00006290: 2061 206c 696e 6b2d 6c6f 6361 6c20 4950   a link-local IP
+000062a0: 7636 2069 6e74 6572 6661 6365 2229 0a0a  v6 interface")..
+000062b0: 2020 2020 2020 2020 6173 796e 6320 7769          async wi
+000062c0: 7468 2061 7761 6974 2063 7265 6174 655f  th await create_
+000062d0: 7463 705f 6c69 7374 656e 6572 286c 6f63  tcp_listener(loc
+000062e0: 616c 5f68 6f73 743d 6c69 6e6b 5f6c 6f63  al_host=link_loc
+000062f0: 616c 5f69 7076 365f 6164 6472 6573 7329  al_ipv6_address)
+00006300: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
+00006310: 7373 0a0a 0a40 7079 7465 7374 2e6d 6172  ss...@pytest.mar
+00006320: 6b2e 736b 6970 6966 280a 2020 2020 7379  k.skipif(.    sy
+00006330: 732e 706c 6174 666f 726d 203d 3d20 2277  s.platform == "w
+00006340: 696e 3332 222c 2072 6561 736f 6e3d 2255  in32", reason="U
+00006350: 4e49 5820 736f 636b 6574 7320 6172 6520  NIX sockets are 
+00006360: 6e6f 7420 6176 6169 6c61 626c 6520 6f6e  not available on
+00006370: 2057 696e 646f 7773 220a 290a 636c 6173   Windows".).clas
+00006380: 7320 5465 7374 554e 4958 5374 7265 616d  s TestUNIXStream
+00006390: 3a0a 2020 2020 4070 7974 6573 742e 6669  :.    @pytest.fi
+000063a0: 7874 7572 650a 2020 2020 6465 6620 736f  xture.    def so
+000063b0: 636b 6574 5f70 6174 6828 7365 6c66 2920  cket_path(self) 
+000063c0: 2d3e 2047 656e 6572 6174 6f72 5b50 6174  -> Generator[Pat
+000063d0: 682c 204e 6f6e 652c 204e 6f6e 655d 3a0a  h, None, None]:.
+000063e0: 2020 2020 2020 2020 2320 5573 6520 7374          # Use st
+000063f0: 646c 6962 2074 656d 7064 6972 2067 656e  dlib tempdir gen
+00006400: 6572 6174 696f 6e0a 2020 2020 2020 2020  eration.        
+00006410: 2320 4669 7865 7320 604f 5345 7272 6f72  # Fixes `OSError
+00006420: 3a20 4146 5f55 4e49 5820 7061 7468 2074  : AF_UNIX path t
+00006430: 6f6f 206c 6f6e 6760 2066 726f 6d20 7079  oo long` from py
+00006440: 7465 7374 2067 656e 6572 6174 6564 2074  test generated t
+00006450: 656d 705f 7061 7468 0a20 2020 2020 2020  emp_path.       
+00006460: 2077 6974 6820 7465 6d70 6669 6c65 2e54   with tempfile.T
+00006470: 656d 706f 7261 7279 4469 7265 6374 6f72  emporaryDirector
+00006480: 7928 2920 6173 2070 6174 683a 0a20 2020  y() as path:.   
+00006490: 2020 2020 2020 2020 2079 6965 6c64 2050           yield P
+000064a0: 6174 6828 7061 7468 2920 2f20 2273 6f63  ath(path) / "soc
+000064b0: 6b65 7422 0a0a 2020 2020 4070 7974 6573  ket"..    @pytes
+000064c0: 742e 6669 7874 7572 6528 7061 7261 6d73  t.fixture(params
+000064d0: 3d5b 4661 6c73 652c 2054 7275 655d 2c20  =[False, True], 
+000064e0: 6964 733d 5b22 7374 7222 2c20 2270 6174  ids=["str", "pat
+000064f0: 6822 5d29 0a20 2020 2064 6566 2073 6f63  h"]).    def soc
+00006500: 6b65 745f 7061 7468 5f6f 725f 7374 7228  ket_path_or_str(
+00006510: 7365 6c66 2c20 7265 7175 6573 743a 2053  self, request: S
+00006520: 7562 5265 7175 6573 742c 2073 6f63 6b65  ubRequest, socke
+00006530: 745f 7061 7468 3a20 5061 7468 2920 2d3e  t_path: Path) ->
+00006540: 2050 6174 6820 7c20 7374 723a 0a20 2020   Path | str:.   
+00006550: 2020 2020 2072 6574 7572 6e20 736f 636b       return sock
+00006560: 6574 5f70 6174 6820 6966 2072 6571 7565  et_path if reque
+00006570: 7374 2e70 6172 616d 2065 6c73 6520 7374  st.param else st
+00006580: 7228 736f 636b 6574 5f70 6174 6829 0a0a  r(socket_path)..
+00006590: 2020 2020 4070 7974 6573 742e 6669 7874      @pytest.fixt
+000065a0: 7572 650a 2020 2020 6465 6620 7365 7276  ure.    def serv
+000065b0: 6572 5f73 6f63 6b28 7365 6c66 2c20 736f  er_sock(self, so
+000065c0: 636b 6574 5f70 6174 683a 2050 6174 6829  cket_path: Path)
+000065d0: 202d 3e20 4974 6572 6162 6c65 5b73 6f63   -> Iterable[soc
+000065e0: 6b65 742e 736f 636b 6574 5d3a 0a20 2020  ket.socket]:.   
+000065f0: 2020 2020 2073 6f63 6b20 3d20 736f 636b       sock = sock
+00006600: 6574 2e73 6f63 6b65 7428 736f 636b 6574  et.socket(socket
+00006610: 2e41 465f 554e 4958 2c20 736f 636b 6574  .AF_UNIX, socket
+00006620: 2e53 4f43 4b5f 5354 5245 414d 290a 2020  .SOCK_STREAM).  
+00006630: 2020 2020 2020 736f 636b 2e73 6574 7469        sock.setti
+00006640: 6d65 6f75 7428 3129 0a20 2020 2020 2020  meout(1).       
+00006650: 2073 6f63 6b2e 6269 6e64 2873 7472 2873   sock.bind(str(s
+00006660: 6f63 6b65 745f 7061 7468 2929 0a20 2020  ocket_path)).   
+00006670: 2020 2020 2073 6f63 6b2e 6c69 7374 656e       sock.listen
+00006680: 2829 0a20 2020 2020 2020 2079 6965 6c64  ().        yield
+00006690: 2073 6f63 6b0a 2020 2020 2020 2020 736f   sock.        so
+000066a0: 636b 2e63 6c6f 7365 2829 0a0a 2020 2020  ck.close()..    
+000066b0: 6173 796e 6320 6465 6620 7465 7374 5f65  async def test_e
+000066c0: 7874 7261 5f61 7474 7269 6275 7465 7328  xtra_attributes(
+000066d0: 0a20 2020 2020 2020 2073 656c 662c 2073  .        self, s
+000066e0: 6572 7665 725f 736f 636b 3a20 736f 636b  erver_sock: sock
+000066f0: 6574 2e73 6f63 6b65 742c 2073 6f63 6b65  et.socket, socke
+00006700: 745f 7061 7468 3a20 5061 7468 0a20 2020  t_path: Path.   
+00006710: 2029 202d 3e20 4e6f 6e65 3a0a 2020 2020   ) -> None:.    
+00006720: 2020 2020 6173 796e 6320 7769 7468 2061      async with a
+00006730: 7761 6974 2063 6f6e 6e65 6374 5f75 6e69  wait connect_uni
+00006740: 7828 736f 636b 6574 5f70 6174 6829 2061  x(socket_path) a
+00006750: 7320 7374 7265 616d 3a0a 2020 2020 2020  s stream:.      
+00006760: 2020 2020 2020 7261 775f 736f 636b 6574        raw_socket
+00006770: 203d 2073 7472 6561 6d2e 6578 7472 6128   = stream.extra(
+00006780: 536f 636b 6574 4174 7472 6962 7574 652e  SocketAttribute.
+00006790: 7261 775f 736f 636b 6574 290a 2020 2020  raw_socket).    
+000067a0: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
+000067b0: 7472 6561 6d2e 6578 7472 6128 536f 636b  tream.extra(Sock
+000067c0: 6574 4174 7472 6962 7574 652e 6661 6d69  etAttribute.fami
+000067d0: 6c79 2920 3d3d 2073 6f63 6b65 742e 4146  ly) == socket.AF
+000067e0: 5f55 4e49 580a 2020 2020 2020 2020 2020  _UNIX.          
+000067f0: 2020 6173 7365 7274 2028 0a20 2020 2020    assert (.     
+00006800: 2020 2020 2020 2020 2020 2073 7472 6561             strea
+00006810: 6d2e 6578 7472 6128 536f 636b 6574 4174  m.extra(SocketAt
+00006820: 7472 6962 7574 652e 6c6f 6361 6c5f 6164  tribute.local_ad
+00006830: 6472 6573 7329 203d 3d20 7261 775f 736f  dress) == raw_so
+00006840: 636b 6574 2e67 6574 736f 636b 6e61 6d65  cket.getsockname
+00006850: 2829 0a20 2020 2020 2020 2020 2020 2029  ().            )
+00006860: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
+00006870: 6572 7420 7374 7265 616d 2e65 7874 7261  ert stream.extra
+00006880: 2853 6f63 6b65 7441 7474 7269 6275 7465  (SocketAttribute
+00006890: 2e72 656d 6f74 655f 6164 6472 6573 7329  .remote_address)
+000068a0: 203d 3d20 7374 7228 736f 636b 6574 5f70   == str(socket_p
+000068b0: 6174 6829 0a20 2020 2020 2020 2020 2020  ath).           
+000068c0: 2070 7974 6573 742e 7261 6973 6573 280a   pytest.raises(.
+000068d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068e0: 5479 7065 6441 7474 7269 6275 7465 4c6f  TypedAttributeLo
+000068f0: 6f6b 7570 4572 726f 722c 2073 7472 6561  okupError, strea
+00006900: 6d2e 6578 7472 612c 2053 6f63 6b65 7441  m.extra, SocketA
+00006910: 7474 7269 6275 7465 2e6c 6f63 616c 5f70  ttribute.local_p
+00006920: 6f72 740a 2020 2020 2020 2020 2020 2020  ort.            
+00006930: 290a 2020 2020 2020 2020 2020 2020 7079  ).            py
+00006940: 7465 7374 2e72 6169 7365 7328 0a20 2020  test.raises(.   
+00006950: 2020 2020 2020 2020 2020 2020 2054 7970               Typ
+00006960: 6564 4174 7472 6962 7574 654c 6f6f 6b75  edAttributeLooku
+00006970: 7045 7272 6f72 2c20 7374 7265 616d 2e65  pError, stream.e
+00006980: 7874 7261 2c20 536f 636b 6574 4174 7472  xtra, SocketAttr
+00006990: 6962 7574 652e 7265 6d6f 7465 5f70 6f72  ibute.remote_por
+000069a0: 740a 2020 2020 2020 2020 2020 2020 290a  t.            ).
+000069b0: 0a20 2020 2061 7379 6e63 2064 6566 2074  .    async def t
+000069c0: 6573 745f 7365 6e64 5f72 6563 6569 7665  est_send_receive
+000069d0: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
+000069e0: 7365 7276 6572 5f73 6f63 6b3a 2073 6f63  server_sock: soc
+000069f0: 6b65 742e 736f 636b 6574 2c20 736f 636b  ket.socket, sock
+00006a00: 6574 5f70 6174 685f 6f72 5f73 7472 3a20  et_path_or_str: 
+00006a10: 5061 7468 207c 2073 7472 0a20 2020 2029  Path | str.    )
+00006a20: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00006a30: 2020 6173 796e 6320 7769 7468 2061 7761    async with awa
+00006a40: 6974 2063 6f6e 6e65 6374 5f75 6e69 7828  it connect_unix(
+00006a50: 736f 636b 6574 5f70 6174 685f 6f72 5f73  socket_path_or_s
+00006a60: 7472 2920 6173 2073 7472 6561 6d3a 0a20  tr) as stream:. 
+00006a70: 2020 2020 2020 2020 2020 2063 6c69 656e             clien
+00006a80: 742c 205f 203d 2073 6572 7665 725f 736f  t, _ = server_so
+00006a90: 636b 2e61 6363 6570 7428 290a 2020 2020  ck.accept().    
+00006aa0: 2020 2020 2020 2020 6177 6169 7420 7374          await st
+00006ab0: 7265 616d 2e73 656e 6428 6222 626c 6168  ream.send(b"blah
+00006ac0: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
+00006ad0: 6571 7565 7374 203d 2063 6c69 656e 742e  equest = client.
+00006ae0: 7265 6376 2831 3030 290a 2020 2020 2020  recv(100).      
+00006af0: 2020 2020 2020 636c 6965 6e74 2e73 656e        client.sen
+00006b00: 6461 6c6c 2872 6571 7565 7374 5b3a 3a2d  dall(request[::-
+00006b10: 315d 290a 2020 2020 2020 2020 2020 2020  1]).            
+00006b20: 7265 7370 6f6e 7365 203d 2061 7761 6974  response = await
+00006b30: 2073 7472 6561 6d2e 7265 6365 6976 6528   stream.receive(
+00006b40: 290a 2020 2020 2020 2020 2020 2020 636c  ).            cl
+00006b50: 6965 6e74 2e63 6c6f 7365 2829 0a0a 2020  ient.close()..  
+00006b60: 2020 2020 2020 6173 7365 7274 2072 6573        assert res
+00006b70: 706f 6e73 6520 3d3d 2062 2268 616c 6222  ponse == b"halb"
+00006b80: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+00006b90: 7465 7374 5f72 6563 6569 7665 5f6c 6172  test_receive_lar
+00006ba0: 6765 5f62 7566 6665 7228 0a20 2020 2020  ge_buffer(.     
+00006bb0: 2020 2073 656c 662c 2073 6572 7665 725f     self, server_
+00006bc0: 736f 636b 3a20 736f 636b 6574 2e73 6f63  sock: socket.soc
+00006bd0: 6b65 742c 2073 6f63 6b65 745f 7061 7468  ket, socket_path
+00006be0: 3a20 5061 7468 0a20 2020 2029 202d 3e20  : Path.    ) -> 
+00006bf0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6465  None:.        de
+00006c00: 6620 7365 7276 6528 2920 2d3e 204e 6f6e  f serve() -> Non
+00006c10: 653a 0a20 2020 2020 2020 2020 2020 2063  e:.            c
+00006c20: 6c69 656e 742c 205f 203d 2073 6572 7665  lient, _ = serve
+00006c30: 725f 736f 636b 2e61 6363 6570 7428 290a  r_sock.accept().
+00006c40: 2020 2020 2020 2020 2020 2020 636c 6965              clie
+00006c50: 6e74 2e73 656e 6461 6c6c 2862 7566 6665  nt.sendall(buffe
+00006c60: 7229 0a20 2020 2020 2020 2020 2020 2063  r).            c
+00006c70: 6c69 656e 742e 636c 6f73 6528 290a 0a20  lient.close().. 
+00006c80: 2020 2020 2020 2062 7566 6665 7220 3d20         buffer = 
+00006c90: 280a 2020 2020 2020 2020 2020 2020 6222  (.            b"
+00006ca0: 5c78 6666 2220 2a20 3130 3234 202a 2035  \xff" * 1024 * 5
+00006cb0: 3132 202b 2062 225c 7830 3022 202a 2031  12 + b"\x00" * 1
+00006cc0: 3032 3420 2a20 3531 320a 2020 2020 2020  024 * 512.      
+00006cd0: 2020 2920 2023 2073 686f 756c 6420 6578    )  # should ex
+00006ce0: 6365 6564 2074 6865 206d 6178 696d 756d  ceed the maximum
+00006cf0: 206b 6572 6e65 6c20 7365 6e64 2062 7566   kernel send buf
+00006d00: 6665 7220 7369 7a65 0a20 2020 2020 2020  fer size.       
+00006d10: 2061 7379 6e63 2077 6974 6820 6177 6169   async with awai
+00006d20: 7420 636f 6e6e 6563 745f 756e 6978 2873  t connect_unix(s
+00006d30: 6f63 6b65 745f 7061 7468 2920 6173 2073  ocket_path) as s
+00006d40: 7472 6561 6d3a 0a20 2020 2020 2020 2020  tream:.         
+00006d50: 2020 2074 6872 6561 6420 3d20 5468 7265     thread = Thre
+00006d60: 6164 2874 6172 6765 743d 7365 7276 652c  ad(target=serve,
+00006d70: 2064 6165 6d6f 6e3d 5472 7565 290a 2020   daemon=True).  
+00006d80: 2020 2020 2020 2020 2020 7468 7265 6164            thread
+00006d90: 2e73 7461 7274 2829 0a20 2020 2020 2020  .start().       
+00006da0: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+00006db0: 6222 220a 2020 2020 2020 2020 2020 2020  b"".            
+00006dc0: 7768 696c 6520 6c65 6e28 7265 7370 6f6e  while len(respon
+00006dd0: 7365 2920 3c20 6c65 6e28 6275 6666 6572  se) < len(buffer
+00006de0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00006df0: 2020 2072 6573 706f 6e73 6520 2b3d 2061     response += a
+00006e00: 7761 6974 2073 7472 6561 6d2e 7265 6365  wait stream.rece
+00006e10: 6976 6528 290a 0a20 2020 2020 2020 2074  ive()..        t
+00006e20: 6872 6561 642e 6a6f 696e 2829 0a20 2020  hread.join().   
+00006e30: 2020 2020 2061 7373 6572 7420 7265 7370       assert resp
+00006e40: 6f6e 7365 203d 3d20 6275 6666 6572 0a0a  onse == buffer..
+00006e50: 2020 2020 6173 796e 6320 6465 6620 7465      async def te
+00006e60: 7374 5f73 656e 645f 6c61 7267 655f 6275  st_send_large_bu
+00006e70: 6666 6572 280a 2020 2020 2020 2020 7365  ffer(.        se
+00006e80: 6c66 2c20 7365 7276 6572 5f73 6f63 6b3a  lf, server_sock:
+00006e90: 2073 6f63 6b65 742e 736f 636b 6574 2c20   socket.socket, 
+00006ea0: 736f 636b 6574 5f70 6174 683a 2050 6174  socket_path: Pat
+00006eb0: 680a 2020 2020 2920 2d3e 204e 6f6e 653a  h.    ) -> None:
+00006ec0: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+00006ed0: 6520 3d20 6222 220a 0a20 2020 2020 2020  e = b""..       
+00006ee0: 2064 6566 2073 6572 7665 2829 202d 3e20   def serve() -> 
+00006ef0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00006f00: 2020 6e6f 6e6c 6f63 616c 2072 6573 706f    nonlocal respo
+00006f10: 6e73 650a 2020 2020 2020 2020 2020 2020  nse.            
+00006f20: 636c 6965 6e74 2c20 5f20 3d20 7365 7276  client, _ = serv
+00006f30: 6572 5f73 6f63 6b2e 6163 6365 7074 2829  er_sock.accept()
+00006f40: 0a20 2020 2020 2020 2020 2020 2077 6869  .            whi
+00006f50: 6c65 2054 7275 653a 0a20 2020 2020 2020  le True:.       
+00006f60: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
+00006f70: 636c 6965 6e74 2e72 6563 7628 3130 3234  client.recv(1024
+00006f80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00006f90: 2020 6966 206e 6f74 2064 6174 613a 0a20    if not data:. 
+00006fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fb0: 2020 2062 7265 616b 0a0a 2020 2020 2020     break..      
+00006fc0: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
+00006fd0: 7365 202b 3d20 6461 7461 0a0a 2020 2020  se += data..    
+00006fe0: 2020 2020 2020 2020 636c 6965 6e74 2e63          client.c
+00006ff0: 6c6f 7365 2829 0a0a 2020 2020 2020 2020  lose()..        
+00007000: 6275 6666 6572 203d 2028 0a20 2020 2020  buffer = (.     
+00007010: 2020 2020 2020 2062 225c 7866 6622 202a         b"\xff" *
+00007020: 2031 3032 3420 2a20 3531 3220 2b20 6222   1024 * 512 + b"
+00007030: 5c78 3030 2220 2a20 3130 3234 202a 2035  \x00" * 1024 * 5
+00007040: 3132 0a20 2020 2020 2020 2029 2020 2320  12.        )  # 
+00007050: 7368 6f75 6c64 2065 7863 6565 6420 7468  should exceed th
+00007060: 6520 6d61 7869 6d75 6d20 6b65 726e 656c  e maximum kernel
+00007070: 2073 656e 6420 6275 6666 6572 2073 697a   send buffer siz
+00007080: 650a 2020 2020 2020 2020 6173 796e 6320  e.        async 
+00007090: 7769 7468 2061 7761 6974 2063 6f6e 6e65  with await conne
+000070a0: 6374 5f75 6e69 7828 736f 636b 6574 5f70  ct_unix(socket_p
+000070b0: 6174 6829 2061 7320 7374 7265 616d 3a0a  ath) as stream:.
+000070c0: 2020 2020 2020 2020 2020 2020 7468 7265              thre
+000070d0: 6164 203d 2054 6872 6561 6428 7461 7267  ad = Thread(targ
+000070e0: 6574 3d73 6572 7665 2c20 6461 656d 6f6e  et=serve, daemon
+000070f0: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
+00007100: 2020 2074 6872 6561 642e 7374 6172 7428     thread.start(
+00007110: 290a 2020 2020 2020 2020 2020 2020 6177  ).            aw
+00007120: 6169 7420 7374 7265 616d 2e73 656e 6428  ait stream.send(
+00007130: 6275 6666 6572 290a 0a20 2020 2020 2020  buffer)..       
+00007140: 2074 6872 6561 642e 6a6f 696e 2829 0a20   thread.join(). 
+00007150: 2020 2020 2020 2061 7373 6572 7420 7265         assert re
+00007160: 7370 6f6e 7365 203d 3d20 6275 6666 6572  sponse == buffer
+00007170: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+00007180: 7465 7374 5f72 6563 6569 7665 5f66 6473  test_receive_fds
+00007190: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
+000071a0: 7365 7276 6572 5f73 6f63 6b3a 2073 6f63  server_sock: soc
+000071b0: 6b65 742e 736f 636b 6574 2c20 736f 636b  ket.socket, sock
+000071c0: 6574 5f70 6174 683a 2050 6174 682c 2074  et_path: Path, t
+000071d0: 6d70 5f70 6174 683a 2050 6174 680a 2020  mp_path: Path.  
+000071e0: 2020 2920 2d3e 204e 6f6e 653a 0a20 2020    ) -> None:.   
+000071f0: 2020 2020 2064 6566 2073 6572 7665 2829       def serve()
+00007200: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00007210: 2020 2020 2020 7061 7468 3120 3d20 746d        path1 = tm
+00007220: 705f 7061 7468 202f 2022 6669 6c65 3122  p_path / "file1"
+00007230: 0a20 2020 2020 2020 2020 2020 2070 6174  .            pat
+00007240: 6832 203d 2074 6d70 5f70 6174 6820 2f20  h2 = tmp_path / 
+00007250: 2266 696c 6532 220a 2020 2020 2020 2020  "file2".        
+00007260: 2020 2020 7061 7468 312e 7772 6974 655f      path1.write_
+00007270: 7465 7874 2822 4865 6c6c 6f2c 2022 290a  text("Hello, ").
+00007280: 2020 2020 2020 2020 2020 2020 7061 7468              path
+00007290: 322e 7772 6974 655f 7465 7874 2822 576f  2.write_text("Wo
+000072a0: 726c 6421 2229 0a20 2020 2020 2020 2020  rld!").         
+000072b0: 2020 2077 6974 6820 7061 7468 312e 6f70     with path1.op
+000072c0: 656e 2829 2061 7320 6669 6c65 312c 2070  en() as file1, p
+000072d0: 6174 6832 2e6f 7065 6e28 2920 6173 2066  ath2.open() as f
+000072e0: 696c 6532 3a0a 2020 2020 2020 2020 2020  ile2:.          
+000072f0: 2020 2020 2020 6664 6172 7261 7920 3d20        fdarray = 
+00007300: 6172 7261 792e 6172 7261 7928 2269 222c  array.array("i",
+00007310: 205b 6669 6c65 312e 6669 6c65 6e6f 2829   [file1.fileno()
+00007320: 2c20 6669 6c65 322e 6669 6c65 6e6f 2829  , file2.fileno()
+00007330: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+00007340: 2020 2063 6c69 656e 742c 205f 203d 2073     client, _ = s
+00007350: 6572 7665 725f 736f 636b 2e61 6363 6570  erver_sock.accep
+00007360: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+00007370: 2020 2020 636d 7367 203d 2028 736f 636b      cmsg = (sock
+00007380: 6574 2e53 4f4c 5f53 4f43 4b45 542c 2073  et.SOL_SOCKET, s
+00007390: 6f63 6b65 742e 5343 4d5f 5249 4748 5453  ocket.SCM_RIGHTS
+000073a0: 2c20 6664 6172 7261 7929 0a20 2020 2020  , fdarray).     
+000073b0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+000073c0: 636c 6965 6e74 3a0a 2020 2020 2020 2020  client:.        
+000073d0: 2020 2020 2020 2020 2020 2020 636c 6965              clie
+000073e0: 6e74 2e73 656e 646d 7367 285b 6222 7465  nt.sendmsg([b"te
+000073f0: 7374 225d 2c20 5b63 6d73 675d 290a 0a20  st"], [cmsg]).. 
+00007400: 2020 2020 2020 2061 7379 6e63 2077 6974         async wit
+00007410: 6820 6177 6169 7420 636f 6e6e 6563 745f  h await connect_
+00007420: 756e 6978 2873 6f63 6b65 745f 7061 7468  unix(socket_path
+00007430: 2920 6173 2073 7472 6561 6d3a 0a20 2020  ) as stream:.   
+00007440: 2020 2020 2020 2020 2074 6872 6561 6420           thread 
+00007450: 3d20 5468 7265 6164 2874 6172 6765 743d  = Thread(target=
+00007460: 7365 7276 652c 2064 6165 6d6f 6e3d 5472  serve, daemon=Tr
+00007470: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+00007480: 7468 7265 6164 2e73 7461 7274 2829 0a20  thread.start(). 
+00007490: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+000074a0: 6765 2c20 6664 7320 3d20 6177 6169 7420  ge, fds = await 
+000074b0: 7374 7265 616d 2e72 6563 6569 7665 5f66  stream.receive_f
+000074c0: 6473 2831 302c 2032 290a 2020 2020 2020  ds(10, 2).      
+000074d0: 2020 2020 2020 7468 7265 6164 2e6a 6f69        thread.joi
+000074e0: 6e28 290a 0a20 2020 2020 2020 2074 6578  n()..        tex
+000074f0: 7420 3d20 2222 0a20 2020 2020 2020 2066  t = "".        f
+00007500: 6f72 2066 6420 696e 2066 6473 3a0a 2020  or fd in fds:.  
+00007510: 2020 2020 2020 2020 2020 7769 7468 206f            with o
+00007520: 732e 6664 6f70 656e 2866 6429 2061 7320  s.fdopen(fd) as 
+00007530: 6669 6c65 3a0a 2020 2020 2020 2020 2020  file:.          
+00007540: 2020 2020 2020 7465 7874 202b 3d20 6669        text += fi
+00007550: 6c65 2e72 6561 6428 290a 0a20 2020 2020  le.read()..     
+00007560: 2020 2061 7373 6572 7420 6d65 7373 6167     assert messag
+00007570: 6520 3d3d 2062 2274 6573 7422 0a20 2020  e == b"test".   
+00007580: 2020 2020 2061 7373 6572 7420 7465 7874       assert text
+00007590: 203d 3d20 2248 656c 6c6f 2c20 576f 726c   == "Hello, Worl
+000075a0: 6421 220a 0a20 2020 2061 7379 6e63 2064  d!"..    async d
+000075b0: 6566 2074 6573 745f 7265 6365 6976 655f  ef test_receive_
+000075c0: 6664 735f 6261 645f 6172 6773 280a 2020  fds_bad_args(.  
+000075d0: 2020 2020 2020 7365 6c66 2c20 7365 7276        self, serv
+000075e0: 6572 5f73 6f63 6b3a 2073 6f63 6b65 742e  er_sock: socket.
+000075f0: 736f 636b 6574 2c20 736f 636b 6574 5f70  socket, socket_p
+00007600: 6174 683a 2050 6174 680a 2020 2020 2920  ath: Path.    ) 
+00007610: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00007620: 2061 7379 6e63 2077 6974 6820 6177 6169   async with awai
+00007630: 7420 636f 6e6e 6563 745f 756e 6978 2873  t connect_unix(s
+00007640: 6f63 6b65 745f 7061 7468 2920 6173 2073  ocket_path) as s
+00007650: 7472 6561 6d3a 0a20 2020 2020 2020 2020  tream:.         
+00007660: 2020 2066 6f72 206d 7367 6c65 6e20 696e     for msglen in
+00007670: 2028 2d31 2c20 2266 6f6f 2229 3a0a 2020   (-1, "foo"):.  
+00007680: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+00007690: 7468 2070 7974 6573 742e 7261 6973 6573  th pytest.raises
+000076a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000076b0: 2020 2020 2020 5661 6c75 6545 7272 6f72        ValueError
+000076c0: 2c20 6d61 7463 683d 226d 7367 6c65 6e20  , match="msglen 
+000076d0: 6d75 7374 2062 6520 6120 6e6f 6e2d 6e65  must be a non-ne
+000076e0: 6761 7469 7665 2069 6e74 6567 6572 220a  gative integer".
+000076f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007700: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00007710: 2020 2020 2020 2061 7761 6974 2073 7472         await str
+00007720: 6561 6d2e 7265 6365 6976 655f 6664 7328  eam.receive_fds(
+00007730: 6d73 676c 656e 2c20 3029 2020 2320 7479  msglen, 0)  # ty
+00007740: 7065 3a20 6967 6e6f 7265 5b61 7267 2d74  pe: ignore[arg-t
+00007750: 7970 655d 0a0a 2020 2020 2020 2020 2020  ype]..          
+00007760: 2020 666f 7220 6d61 7866 6473 2069 6e20    for maxfds in 
+00007770: 2830 2c20 2266 6f6f 2229 3a0a 2020 2020  (0, "foo"):.    
+00007780: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00007790: 2070 7974 6573 742e 7261 6973 6573 280a   pytest.raises(.
+000077a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077b0: 2020 2020 5661 6c75 6545 7272 6f72 2c20      ValueError, 
+000077c0: 6d61 7463 683d 226d 6178 6664 7320 6d75  match="maxfds mu
+000077d0: 7374 2062 6520 6120 706f 7369 7469 7665  st be a positive
+000077e0: 2069 6e74 6567 6572 220a 2020 2020 2020   integer".      
+000077f0: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
+00007800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007810: 2061 7761 6974 2073 7472 6561 6d2e 7265   await stream.re
+00007820: 6365 6976 655f 6664 7328 302c 206d 6178  ceive_fds(0, max
+00007830: 6664 7329 2020 2320 7479 7065 3a20 6967  fds)  # type: ig
+00007840: 6e6f 7265 5b61 7267 2d74 7970 655d 0a0a  nore[arg-type]..
+00007850: 2020 2020 6173 796e 6320 6465 6620 7465      async def te
+00007860: 7374 5f73 656e 645f 6664 7328 0a20 2020  st_send_fds(.   
+00007870: 2020 2020 2073 656c 662c 2073 6572 7665       self, serve
+00007880: 725f 736f 636b 3a20 736f 636b 6574 2e73  r_sock: socket.s
+00007890: 6f63 6b65 742c 2073 6f63 6b65 745f 7061  ocket, socket_pa
+000078a0: 7468 3a20 5061 7468 2c20 746d 705f 7061  th: Path, tmp_pa
+000078b0: 7468 3a20 5061 7468 0a20 2020 2029 202d  th: Path.    ) -
+000078c0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+000078d0: 6465 6620 7365 7276 6528 2920 2d3e 204e  def serve() -> N
+000078e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000078f0: 2066 6473 203d 2061 7272 6179 2e61 7272   fds = array.arr
+00007900: 6179 2822 6922 290a 2020 2020 2020 2020  ay("i").        
+00007910: 2020 2020 636c 6965 6e74 2c20 5f20 3d20      client, _ = 
+00007920: 7365 7276 6572 5f73 6f63 6b2e 6163 6365  server_sock.acce
+00007930: 7074 2829 0a20 2020 2020 2020 2020 2020  pt().           
+00007940: 206d 7367 2c20 616e 6364 6174 612c 202a   msg, ancdata, *
+00007950: 5f20 3d20 636c 6965 6e74 2e72 6563 766d  _ = client.recvm
+00007960: 7367 2831 302c 2073 6f63 6b65 742e 434d  sg(10, socket.CM
+00007970: 5347 5f4c 454e 2832 202a 2066 6473 2e69  SG_LEN(2 * fds.i
+00007980: 7465 6d73 697a 6529 290a 2020 2020 2020  temsize)).      
+00007990: 2020 2020 2020 636c 6965 6e74 2e63 6c6f        client.clo
+000079a0: 7365 2829 0a20 2020 2020 2020 2020 2020  se().           
+000079b0: 2061 7373 6572 7420 6d73 6720 3d3d 2062   assert msg == b
+000079c0: 2274 6573 7422 0a20 2020 2020 2020 2020  "test".         
+000079d0: 2020 2066 6f72 2063 6d73 675f 6c65 7665     for cmsg_leve
+000079e0: 6c2c 2063 6d73 675f 7479 7065 2c20 636d  l, cmsg_type, cm
+000079f0: 7367 5f64 6174 6120 696e 2061 6e63 6461  sg_data in ancda
+00007a00: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
+00007a10: 2020 2020 6173 7365 7274 2063 6d73 675f      assert cmsg_
+00007a20: 6c65 7665 6c20 3d3d 2073 6f63 6b65 742e  level == socket.
+00007a30: 534f 4c5f 534f 434b 4554 0a20 2020 2020  SOL_SOCKET.     
+00007a40: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+00007a50: 7420 636d 7367 5f74 7970 6520 3d3d 2073  t cmsg_type == s
+00007a60: 6f63 6b65 742e 5343 4d5f 5249 4748 5453  ocket.SCM_RIGHTS
+00007a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007a80: 2066 6473 2e66 726f 6d62 7974 6573 280a   fds.frombytes(.
+00007a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007aa0: 2020 2020 636d 7367 5f64 6174 615b 3a20      cmsg_data[: 
+00007ab0: 6c65 6e28 636d 7367 5f64 6174 6129 202d  len(cmsg_data) -
+00007ac0: 2028 6c65 6e28 636d 7367 5f64 6174 6129   (len(cmsg_data)
+00007ad0: 2025 2066 6473 2e69 7465 6d73 697a 6529   % fds.itemsize)
+00007ae0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00007af0: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+00007b00: 2074 6578 7420 3d20 2222 0a20 2020 2020   text = "".     
+00007b10: 2020 2020 2020 2066 6f72 2066 6420 696e         for fd in
+00007b20: 2066 6473 3a0a 2020 2020 2020 2020 2020   fds:.          
+00007b30: 2020 2020 2020 7769 7468 206f 732e 6664        with os.fd
+00007b40: 6f70 656e 2866 6429 2061 7320 6669 6c65  open(fd) as file
+00007b50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007b60: 2020 2020 2020 7465 7874 202b 3d20 6669        text += fi
+00007b70: 6c65 2e72 6561 6428 290a 0a20 2020 2020  le.read()..     
+00007b80: 2020 2020 2020 2061 7373 6572 7420 7465         assert te
+00007b90: 7874 203d 3d20 2248 656c 6c6f 2c20 576f  xt == "Hello, Wo
+00007ba0: 726c 6421 220a 0a20 2020 2020 2020 2070  rld!"..        p
+00007bb0: 6174 6831 203d 2074 6d70 5f70 6174 6820  ath1 = tmp_path 
+00007bc0: 2f20 2266 696c 6531 220a 2020 2020 2020  / "file1".      
+00007bd0: 2020 7061 7468 3220 3d20 746d 705f 7061    path2 = tmp_pa
+00007be0: 7468 202f 2022 6669 6c65 3222 0a20 2020  th / "file2".   
+00007bf0: 2020 2020 2070 6174 6831 2e77 7269 7465       path1.write
+00007c00: 5f74 6578 7428 2248 656c 6c6f 2c20 2229  _text("Hello, ")
+00007c10: 0a20 2020 2020 2020 2070 6174 6832 2e77  .        path2.w
+00007c20: 7269 7465 5f74 6578 7428 2257 6f72 6c64  rite_text("World
+00007c30: 2122 290a 2020 2020 2020 2020 7769 7468  !").        with
+00007c40: 2070 6174 6831 2e6f 7065 6e28 2920 6173   path1.open() as
+00007c50: 2066 696c 6531 2c20 7061 7468 322e 6f70   file1, path2.op
+00007c60: 656e 2829 2061 7320 6669 6c65 322c 2066  en() as file2, f
+00007c70: 6169 6c5f 6166 7465 7228 3229 3a0a 2020  ail_after(2):.  
+00007c80: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+00007c90: 2069 7369 6e73 7461 6e63 6528 6669 6c65   isinstance(file
+00007ca0: 312c 2069 6f2e 5465 7874 494f 5772 6170  1, io.TextIOWrap
+00007cb0: 7065 7229 0a20 2020 2020 2020 2020 2020  per).           
+00007cc0: 2061 7373 6572 7420 6973 696e 7374 616e   assert isinstan
+00007cd0: 6365 2866 696c 6532 2c20 696f 2e54 6578  ce(file2, io.Tex
+00007ce0: 7449 4f57 7261 7070 6572 290a 2020 2020  tIOWrapper).    
+00007cf0: 2020 2020 2020 2020 6173 796e 6320 7769          async wi
+00007d00: 7468 2061 7761 6974 2063 6f6e 6e65 6374  th await connect
+00007d10: 5f75 6e69 7828 736f 636b 6574 5f70 6174  _unix(socket_pat
+00007d20: 6829 2061 7320 7374 7265 616d 3a0a 2020  h) as stream:.  
+00007d30: 2020 2020 2020 2020 2020 2020 2020 7468                th
+00007d40: 7265 6164 203d 2054 6872 6561 6428 7461  read = Thread(ta
+00007d50: 7267 6574 3d73 6572 7665 2c20 6461 656d  rget=serve, daem
+00007d60: 6f6e 3d54 7275 6529 0a20 2020 2020 2020  on=True).       
+00007d70: 2020 2020 2020 2020 2074 6872 6561 642e           thread.
+00007d80: 7374 6172 7428 290a 2020 2020 2020 2020  start().        
+00007d90: 2020 2020 2020 2020 6177 6169 7420 7374          await st
+00007da0: 7265 616d 2e73 656e 645f 6664 7328 6222  ream.send_fds(b"
+00007db0: 7465 7374 222c 205b 6669 6c65 312c 2066  test", [file1, f
+00007dc0: 696c 6532 5d29 0a20 2020 2020 2020 2020  ile2]).         
+00007dd0: 2020 2020 2020 2074 6872 6561 642e 6a6f         thread.jo
+00007de0: 696e 2829 0a0a 2020 2020 6173 796e 6320  in()..    async 
+00007df0: 6465 6620 7465 7374 5f73 656e 645f 656f  def test_send_eo
+00007e00: 6628 0a20 2020 2020 2020 2073 656c 662c  f(.        self,
+00007e10: 2073 6572 7665 725f 736f 636b 3a20 736f   server_sock: so
+00007e20: 636b 6574 2e73 6f63 6b65 742c 2073 6f63  cket.socket, soc
+00007e30: 6b65 745f 7061 7468 3a20 5061 7468 0a20  ket_path: Path. 
+00007e40: 2020 2029 202d 3e20 4e6f 6e65 3a0a 2020     ) -> None:.  
+00007e50: 2020 2020 2020 6465 6620 7365 7276 6528        def serve(
+00007e60: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00007e70: 2020 2020 2020 2063 6c69 656e 742c 205f         client, _
+00007e80: 203d 2073 6572 7665 725f 736f 636b 2e61   = server_sock.a
+00007e90: 6363 6570 7428 290a 2020 2020 2020 2020  ccept().        
+00007ea0: 2020 2020 7265 7175 6573 7420 3d20 6222      request = b"
+00007eb0: 220a 2020 2020 2020 2020 2020 2020 7768  ".            wh
+00007ec0: 696c 6520 5472 7565 3a0a 2020 2020 2020  ile True:.      
+00007ed0: 2020 2020 2020 2020 2020 6461 7461 203d            data =
+00007ee0: 2063 6c69 656e 742e 7265 6376 2831 3030   client.recv(100
+00007ef0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00007f00: 2020 7265 7175 6573 7420 2b3d 2064 6174    request += dat
+00007f10: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
+00007f20: 2020 6966 206e 6f74 2064 6174 613a 0a20    if not data:. 
+00007f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f40: 2020 2062 7265 616b 0a0a 2020 2020 2020     break..      
+00007f50: 2020 2020 2020 636c 6965 6e74 2e73 656e        client.sen
+00007f60: 6461 6c6c 2872 6571 7565 7374 5b3a 3a2d  dall(request[::-
+00007f70: 315d 290a 2020 2020 2020 2020 2020 2020  1]).            
+00007f80: 636c 6965 6e74 2e63 6c6f 7365 2829 0a0a  client.close()..
+00007f90: 2020 2020 2020 2020 6173 796e 6320 7769          async wi
+00007fa0: 7468 2061 7761 6974 2063 6f6e 6e65 6374  th await connect
+00007fb0: 5f75 6e69 7828 736f 636b 6574 5f70 6174  _unix(socket_pat
+00007fc0: 6829 2061 7320 7374 7265 616d 3a0a 2020  h) as stream:.  
+00007fd0: 2020 2020 2020 2020 2020 7468 7265 6164            thread
+00007fe0: 203d 2054 6872 6561 6428 7461 7267 6574   = Thread(target
+00007ff0: 3d73 6572 7665 2c20 6461 656d 6f6e 3d54  =serve, daemon=T
+00008000: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+00008010: 2074 6872 6561 642e 7374 6172 7428 290a   thread.start().
+00008020: 2020 2020 2020 2020 2020 2020 6177 6169              awai
+00008030: 7420 7374 7265 616d 2e73 656e 6428 6222  t stream.send(b"
+00008040: 6865 6c6c 6f2c 2022 290a 2020 2020 2020  hello, ").      
+00008050: 2020 2020 2020 6177 6169 7420 7374 7265        await stre
+00008060: 616d 2e73 656e 6428 6222 776f 726c 645c  am.send(b"world\
+00008070: 6e22 290a 2020 2020 2020 2020 2020 2020  n").            
+00008080: 6177 6169 7420 7374 7265 616d 2e73 656e  await stream.sen
+00008090: 645f 656f 6628 290a 2020 2020 2020 2020  d_eof().        
+000080a0: 2020 2020 7265 7370 6f6e 7365 203d 2061      response = a
+000080b0: 7761 6974 2073 7472 6561 6d2e 7265 6365  wait stream.rece
+000080c0: 6976 6528 290a 0a20 2020 2020 2020 2074  ive()..        t
+000080d0: 6872 6561 642e 6a6f 696e 2829 0a20 2020  hread.join().   
+000080e0: 2020 2020 2061 7373 6572 7420 7265 7370       assert resp
+000080f0: 6f6e 7365 203d 3d20 6222 5c6e 646c 726f  onse == b"\ndlro
+00008100: 7720 2c6f 6c6c 6568 220a 0a20 2020 2061  w ,olleh"..    a
+00008110: 7379 6e63 2064 6566 2074 6573 745f 6974  sync def test_it
+00008120: 6572 6174 6528 7365 6c66 2c20 7365 7276  erate(self, serv
+00008130: 6572 5f73 6f63 6b3a 2073 6f63 6b65 742e  er_sock: socket.
+00008140: 736f 636b 6574 2c20 736f 636b 6574 5f70  socket, socket_p
+00008150: 6174 683a 2050 6174 6829 202d 3e20 4e6f  ath: Path) -> No
+00008160: 6e65 3a0a 2020 2020 2020 2020 6465 6620  ne:.        def 
+00008170: 7365 7276 6528 2920 2d3e 204e 6f6e 653a  serve() -> None:
+00008180: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
+00008190: 656e 742c 205f 203d 2073 6572 7665 725f  ent, _ = server_
+000081a0: 736f 636b 2e61 6363 6570 7428 290a 2020  sock.accept().  
+000081b0: 2020 2020 2020 2020 2020 636c 6965 6e74            client
+000081c0: 2e73 656e 6461 6c6c 2862 2262 6c22 290a  .sendall(b"bl").
+000081d0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+000081e0: 2e73 6c65 6570 2830 2e30 3529 0a20 2020  .sleep(0.05).   
+000081f0: 2020 2020 2020 2020 2063 6c69 656e 742e           client.
+00008200: 7365 6e64 616c 6c28 6222 6168 2229 0a20  sendall(b"ah"). 
+00008210: 2020 2020 2020 2020 2020 2063 6c69 656e             clien
+00008220: 742e 636c 6f73 6528 290a 0a20 2020 2020  t.close()..     
+00008230: 2020 2074 6872 6561 6420 3d20 5468 7265     thread = Thre
+00008240: 6164 2874 6172 6765 743d 7365 7276 652c  ad(target=serve,
+00008250: 2064 6165 6d6f 6e3d 5472 7565 290a 2020   daemon=True).  
+00008260: 2020 2020 2020 7468 7265 6164 2e73 7461        thread.sta
+00008270: 7274 2829 0a20 2020 2020 2020 2063 6875  rt().        chu
+00008280: 6e6b 7320 3d20 5b5d 0a20 2020 2020 2020  nks = [].       
+00008290: 2061 7379 6e63 2077 6974 6820 6177 6169   async with awai
+000082a0: 7420 636f 6e6e 6563 745f 756e 6978 2873  t connect_unix(s
+000082b0: 6f63 6b65 745f 7061 7468 2920 6173 2073  ocket_path) as s
+000082c0: 7472 6561 6d3a 0a20 2020 2020 2020 2020  tream:.         
+000082d0: 2020 2061 7379 6e63 2066 6f72 2063 6875     async for chu
+000082e0: 6e6b 2069 6e20 7374 7265 616d 3a0a 2020  nk in stream:.  
+000082f0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
+00008300: 756e 6b73 2e61 7070 656e 6428 6368 756e  unks.append(chun
+00008310: 6b29 0a0a 2020 2020 2020 2020 7468 7265  k)..        thre
+00008320: 6164 2e6a 6f69 6e28 290a 2020 2020 2020  ad.join().      
+00008330: 2020 6173 7365 7274 2063 6875 6e6b 7320    assert chunks 
+00008340: 3d3d 205b 6222 626c 222c 2062 2261 6822  == [b"bl", b"ah"
+00008350: 5d0a 0a20 2020 2061 7379 6e63 2064 6566  ]..    async def
+00008360: 2074 6573 745f 7365 6e64 5f66 6473 5f62   test_send_fds_b
+00008370: 6164 5f61 7267 7328 0a20 2020 2020 2020  ad_args(.       
+00008380: 2073 656c 662c 2073 6572 7665 725f 736f   self, server_so
+00008390: 636b 3a20 736f 636b 6574 2e73 6f63 6b65  ck: socket.socke
+000083a0: 742c 2073 6f63 6b65 745f 7061 7468 3a20  t, socket_path: 
+000083b0: 5061 7468 0a20 2020 2029 202d 3e20 4e6f  Path.    ) -> No
+000083c0: 6e65 3a0a 2020 2020 2020 2020 6173 796e  ne:.        asyn
+000083d0: 6320 7769 7468 2061 7761 6974 2063 6f6e  c with await con
+000083e0: 6e65 6374 5f75 6e69 7828 736f 636b 6574  nect_unix(socket
+000083f0: 5f70 6174 6829 2061 7320 7374 7265 616d  _path) as stream
+00008400: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
+00008410: 7468 2070 7974 6573 742e 7261 6973 6573  th pytest.raises
+00008420: 2856 616c 7565 4572 726f 722c 206d 6174  (ValueError, mat
+00008430: 6368 3d22 6d65 7373 6167 6520 6d75 7374  ch="message must
+00008440: 206e 6f74 2062 6520 656d 7074 7922 293a   not be empty"):
+00008450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008460: 2061 7761 6974 2073 7472 6561 6d2e 7365   await stream.se
+00008470: 6e64 5f66 6473 2862 2222 2c20 5b30 5d29  nd_fds(b"", [0])
+00008480: 0a0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
+00008490: 7468 2070 7974 6573 742e 7261 6973 6573  th pytest.raises
+000084a0: 2856 616c 7565 4572 726f 722c 206d 6174  (ValueError, mat
+000084b0: 6368 3d22 6664 7320 6d75 7374 206e 6f74  ch="fds must not
+000084c0: 2062 6520 656d 7074 7922 293a 0a20 2020   be empty"):.   
+000084d0: 2020 2020 2020 2020 2020 2020 2061 7761               awa
+000084e0: 6974 2073 7472 6561 6d2e 7365 6e64 5f66  it stream.send_f
+000084f0: 6473 2862 2274 6573 7422 2c20 5b5d 290a  ds(b"test", []).
+00008500: 0a20 2020 2061 7379 6e63 2064 6566 2074  .    async def t
+00008510: 6573 745f 636f 6e63 7572 7265 6e74 5f73  est_concurrent_s
+00008520: 656e 6428 0a20 2020 2020 2020 2073 656c  end(.        sel
+00008530: 662c 2073 6572 7665 725f 736f 636b 3a20  f, server_sock: 
+00008540: 736f 636b 6574 2e73 6f63 6b65 742c 2073  socket.socket, s
+00008550: 6f63 6b65 745f 7061 7468 3a20 5061 7468  ocket_path: Path
+00008560: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a0a  .    ) -> None:.
+00008570: 2020 2020 2020 2020 6173 796e 6320 6465          async de
+00008580: 6620 7365 6e64 5f64 6174 6128 2920 2d3e  f send_data() ->
+00008590: 204e 6f52 6574 7572 6e3a 0a20 2020 2020   NoReturn:.     
+000085a0: 2020 2020 2020 2077 6869 6c65 2054 7275         while Tru
+000085b0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000085c0: 2020 2061 7761 6974 2063 6c69 656e 742e     await client.
+000085d0: 7365 6e64 2862 225c 7830 3022 202a 2034  send(b"\x00" * 4
+000085e0: 3039 3629 0a0a 2020 2020 2020 2020 6173  096)..        as
+000085f0: 796e 6320 7769 7468 2061 7761 6974 2063  ync with await c
+00008600: 6f6e 6e65 6374 5f75 6e69 7828 736f 636b  onnect_unix(sock
+00008610: 6574 5f70 6174 6829 2061 7320 636c 6965  et_path) as clie
+00008620: 6e74 3a0a 2020 2020 2020 2020 2020 2020  nt:.            
+00008630: 6173 796e 6320 7769 7468 2063 7265 6174  async with creat
+00008640: 655f 7461 736b 5f67 726f 7570 2829 2061  e_task_group() a
+00008650: 7320 7467 3a0a 2020 2020 2020 2020 2020  s tg:.          
+00008660: 2020 2020 2020 7467 2e73 7461 7274 5f73        tg.start_s
+00008670: 6f6f 6e28 7365 6e64 5f64 6174 6129 0a20  oon(send_data). 
+00008680: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00008690: 7761 6974 2077 6169 745f 616c 6c5f 7461  wait wait_all_ta
+000086a0: 736b 735f 626c 6f63 6b65 6428 290a 2020  sks_blocked().  
+000086b0: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+000086c0: 7468 2070 7974 6573 742e 7261 6973 6573  th pytest.raises
+000086d0: 2842 7573 7952 6573 6f75 7263 6545 7272  (BusyResourceErr
+000086e0: 6f72 2920 6173 2065 7863 3a0a 2020 2020  or) as exc:.    
+000086f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008700: 6177 6169 7420 636c 6965 6e74 2e73 656e  await client.sen
+00008710: 6428 6222 666f 6f22 290a 0a20 2020 2020  d(b"foo")..     
+00008720: 2020 2020 2020 2020 2020 2065 7863 2e6d             exc.m
+00008730: 6174 6368 2822 616c 7265 6164 7920 7772  atch("already wr
+00008740: 6974 696e 6720 746f 2229 0a20 2020 2020  iting to").     
+00008750: 2020 2020 2020 2020 2020 2074 672e 6361             tg.ca
+00008760: 6e63 656c 5f73 636f 7065 2e63 616e 6365  ncel_scope.cance
+00008770: 6c28 290a 0a20 2020 2061 7379 6e63 2064  l()..    async d
+00008780: 6566 2074 6573 745f 636f 6e63 7572 7265  ef test_concurre
+00008790: 6e74 5f72 6563 6569 7665 280a 2020 2020  nt_receive(.    
+000087a0: 2020 2020 7365 6c66 2c20 7365 7276 6572      self, server
+000087b0: 5f73 6f63 6b3a 2073 6f63 6b65 742e 736f  _sock: socket.so
+000087c0: 636b 6574 2c20 736f 636b 6574 5f70 6174  cket, socket_pat
+000087d0: 683a 2050 6174 680a 2020 2020 2920 2d3e  h: Path.    ) ->
+000087e0: 204e 6f6e 653a 0a20 2020 2020 2020 2061   None:.        a
+000087f0: 7379 6e63 2077 6974 6820 6177 6169 7420  sync with await 
+00008800: 636f 6e6e 6563 745f 756e 6978 2873 6f63  connect_unix(soc
+00008810: 6b65 745f 7061 7468 2920 6173 2063 6c69  ket_path) as cli
+00008820: 656e 743a 0a20 2020 2020 2020 2020 2020  ent:.           
+00008830: 2061 7379 6e63 2077 6974 6820 6372 6561   async with crea
+00008840: 7465 5f74 6173 6b5f 6772 6f75 7028 2920  te_task_group() 
+00008850: 6173 2074 673a 0a20 2020 2020 2020 2020  as tg:.         
+00008860: 2020 2020 2020 2074 672e 7374 6172 745f         tg.start_
+00008870: 736f 6f6e 2863 6c69 656e 742e 7265 6365  soon(client.rece
+00008880: 6976 6529 0a20 2020 2020 2020 2020 2020  ive).           
+00008890: 2020 2020 2061 7761 6974 2077 6169 745f       await wait_
+000088a0: 616c 6c5f 7461 736b 735f 626c 6f63 6b65  all_tasks_blocke
+000088b0: 6428 290a 2020 2020 2020 2020 2020 2020  d().            
+000088c0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+000088d0: 2020 2020 2020 2020 2020 2020 2077 6974               wit
+000088e0: 6820 7079 7465 7374 2e72 6169 7365 7328  h pytest.raises(
+000088f0: 4275 7379 5265 736f 7572 6365 4572 726f  BusyResourceErro
+00008900: 7229 2061 7320 6578 633a 0a20 2020 2020  r) as exc:.     
+00008910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008920: 2020 2061 7761 6974 2063 6c69 656e 742e     await client.
+00008930: 7265 6365 6976 6528 290a 0a20 2020 2020  receive()..     
+00008940: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00008950: 7863 2e6d 6174 6368 2822 616c 7265 6164  xc.match("alread
+00008960: 7920 7265 6164 696e 6720 6672 6f6d 2229  y reading from")
+00008970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008980: 2066 696e 616c 6c79 3a0a 2020 2020 2020   finally:.      
+00008990: 2020 2020 2020 2020 2020 2020 2020 7467                tg
+000089a0: 2e63 616e 6365 6c5f 7363 6f70 652e 6361  .cancel_scope.ca
+000089b0: 6e63 656c 2829 0a0a 2020 2020 6173 796e  ncel()..    asyn
+000089c0: 6320 6465 6620 7465 7374 5f63 6c6f 7365  c def test_close
+000089d0: 5f64 7572 696e 675f 7265 6365 6976 6528  _during_receive(
+000089e0: 0a20 2020 2020 2020 2073 656c 662c 2073  .        self, s
+000089f0: 6572 7665 725f 736f 636b 3a20 736f 636b  erver_sock: sock
+00008a00: 6574 2e73 6f63 6b65 742c 2073 6f63 6b65  et.socket, socke
+00008a10: 745f 7061 7468 3a20 5061 7468 0a20 2020  t_path: Path.   
+00008a20: 2029 202d 3e20 4e6f 6e65 3a0a 2020 2020   ) -> None:.    
+00008a30: 2020 2020 6173 796e 6320 6465 6620 696e      async def in
+00008a40: 7465 7272 7570 7428 2920 2d3e 204e 6f6e  terrupt() -> Non
+00008a50: 653a 0a20 2020 2020 2020 2020 2020 2061  e:.            a
+00008a60: 7761 6974 2077 6169 745f 616c 6c5f 7461  wait wait_all_ta
+00008a70: 736b 735f 626c 6f63 6b65 6428 290a 2020  sks_blocked().  
+00008a80: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+00008a90: 7374 7265 616d 2e61 636c 6f73 6528 290a  stream.aclose().
+00008aa0: 0a20 2020 2020 2020 2061 7379 6e63 2077  .        async w
+00008ab0: 6974 6820 6177 6169 7420 636f 6e6e 6563  ith await connec
 00008ac0: 745f 756e 6978 2873 6f63 6b65 745f 7061  t_unix(socket_pa
-00008ad0: 7468 290a 0a20 2020 2061 7379 6e63 2064  th)..    async d
-00008ae0: 6566 2074 6573 745f 636f 6e6e 6563 7469  ef test_connecti
-00008af0: 6e67 5f75 7369 6e67 5f62 7974 6573 280a  ng_using_bytes(.
-00008b00: 2020 2020 2020 2020 7365 6c66 2c20 7365          self, se
-00008b10: 7276 6572 5f73 6f63 6b3a 2073 6f63 6b65  rver_sock: socke
-00008b20: 742e 736f 636b 6574 2c20 736f 636b 6574  t.socket, socket
-00008b30: 5f70 6174 683a 2050 6174 680a 2020 2020  _path: Path.    
-00008b40: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00008b50: 2020 2061 7379 6e63 2077 6974 6820 6177     async with aw
-00008b60: 6169 7420 636f 6e6e 6563 745f 756e 6978  ait connect_unix
-00008b70: 2873 7472 2873 6f63 6b65 745f 7061 7468  (str(socket_path
-00008b80: 292e 656e 636f 6465 2829 293a 0a20 2020  ).encode()):.   
-00008b90: 2020 2020 2020 2020 2070 6173 730a 0a20           pass.. 
-00008ba0: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
-00008bb0: 736b 6970 6966 280a 2020 2020 2020 2020  skipif(.        
-00008bc0: 706c 6174 666f 726d 2e73 7973 7465 6d28  platform.system(
-00008bd0: 2920 3d3d 2022 4461 7277 696e 222c 2072  ) == "Darwin", r
-00008be0: 6561 736f 6e3d 226d 6163 4f53 2072 6571  eason="macOS req
-00008bf0: 7569 7265 7320 7661 6c69 6420 5554 462d  uires valid UTF-
-00008c00: 3820 7061 7468 7322 0a20 2020 2029 0a20  8 paths".    ). 
-00008c10: 2020 2061 7379 6e63 2064 6566 2074 6573     async def tes
-00008c20: 745f 636f 6e6e 6563 7469 6e67 5f77 6974  t_connecting_wit
-00008c30: 685f 6e6f 6e5f 7574 6638 2873 656c 662c  h_non_utf8(self,
-00008c40: 2073 6f63 6b65 745f 7061 7468 3a20 5061   socket_path: Pa
-00008c50: 7468 2920 2d3e 204e 6f6e 653a 0a20 2020  th) -> None:.   
-00008c60: 2020 2020 2061 6374 7561 6c5f 7061 7468       actual_path
-00008c70: 203d 2073 7472 2873 6f63 6b65 745f 7061   = str(socket_pa
-00008c80: 7468 292e 656e 636f 6465 2829 202b 2062  th).encode() + b
-00008c90: 225c 7846 3022 0a20 2020 2020 2020 2073  "\xF0".        s
-00008ca0: 6572 7665 7220 3d20 736f 636b 6574 2e73  erver = socket.s
-00008cb0: 6f63 6b65 7428 736f 636b 6574 2e41 465f  ocket(socket.AF_
-00008cc0: 554e 4958 290a 2020 2020 2020 2020 7365  UNIX).        se
-00008cd0: 7276 6572 2e62 696e 6428 6163 7475 616c  rver.bind(actual
-00008ce0: 5f70 6174 6829 0a20 2020 2020 2020 2073  _path).        s
-00008cf0: 6572 7665 722e 6c69 7374 656e 2831 290a  erver.listen(1).
-00008d00: 0a20 2020 2020 2020 2061 7379 6e63 2077  .        async w
-00008d10: 6974 6820 6177 6169 7420 636f 6e6e 6563  ith await connec
-00008d20: 745f 756e 6978 2861 6374 7561 6c5f 7061  t_unix(actual_pa
-00008d30: 7468 293a 0a20 2020 2020 2020 2020 2020  th):.           
-00008d40: 2070 6173 730a 0a0a 4070 7974 6573 742e   pass...@pytest.
-00008d50: 6d61 726b 2e73 6b69 7069 6628 0a20 2020  mark.skipif(.   
-00008d60: 2073 7973 2e70 6c61 7466 6f72 6d20 3d3d   sys.platform ==
-00008d70: 2022 7769 6e33 3222 2c20 7265 6173 6f6e   "win32", reason
-00008d80: 3d22 554e 4958 2073 6f63 6b65 7473 2061  ="UNIX sockets a
-00008d90: 7265 206e 6f74 2061 7661 696c 6162 6c65  re not available
-00008da0: 206f 6e20 5769 6e64 6f77 7322 0a29 0a63   on Windows".).c
-00008db0: 6c61 7373 2054 6573 7455 4e49 584c 6973  lass TestUNIXLis
-00008dc0: 7465 6e65 723a 0a20 2020 2040 7079 7465  tener:.    @pyte
-00008dd0: 7374 2e66 6978 7475 7265 0a20 2020 2064  st.fixture.    d
-00008de0: 6566 2073 6f63 6b65 745f 7061 7468 2873  ef socket_path(s
-00008df0: 656c 6629 202d 3e20 4765 6e65 7261 746f  elf) -> Generato
-00008e00: 725b 5061 7468 2c20 4e6f 6e65 2c20 4e6f  r[Path, None, No
-00008e10: 6e65 5d3a 0a20 2020 2020 2020 2023 2055  ne]:.        # U
-00008e20: 7365 2073 7464 6c69 6220 7465 6d70 6469  se stdlib tempdi
-00008e30: 7220 6765 6e65 7261 7469 6f6e 0a20 2020  r generation.   
-00008e40: 2020 2020 2023 2046 6978 6573 2060 4f53       # Fixes `OS
-00008e50: 4572 726f 723a 2041 465f 554e 4958 2070  Error: AF_UNIX p
-00008e60: 6174 6820 746f 6f20 6c6f 6e67 6020 6672  ath too long` fr
-00008e70: 6f6d 2070 7974 6573 7420 6765 6e65 7261  om pytest genera
-00008e80: 7465 6420 7465 6d70 5f70 6174 680a 2020  ted temp_path.  
-00008e90: 2020 2020 2020 7769 7468 2074 656d 7066        with tempf
-00008ea0: 696c 652e 5465 6d70 6f72 6172 7944 6972  ile.TemporaryDir
-00008eb0: 6563 746f 7279 2829 2061 7320 7061 7468  ectory() as path
-00008ec0: 3a0a 2020 2020 2020 2020 2020 2020 7969  :.            yi
-00008ed0: 656c 6420 5061 7468 2870 6174 6829 202f  eld Path(path) /
-00008ee0: 2022 736f 636b 6574 220a 0a20 2020 2040   "socket"..    @
-00008ef0: 7079 7465 7374 2e66 6978 7475 7265 2870  pytest.fixture(p
-00008f00: 6172 616d 733d 5b46 616c 7365 2c20 5472  arams=[False, Tr
-00008f10: 7565 5d2c 2069 6473 3d5b 2273 7472 222c  ue], ids=["str",
-00008f20: 2022 7061 7468 225d 290a 2020 2020 6465   "path"]).    de
-00008f30: 6620 736f 636b 6574 5f70 6174 685f 6f72  f socket_path_or
-00008f40: 5f73 7472 2873 656c 662c 2072 6571 7565  _str(self, reque
-00008f50: 7374 3a20 5375 6252 6571 7565 7374 2c20  st: SubRequest, 
-00008f60: 736f 636b 6574 5f70 6174 683a 2050 6174  socket_path: Pat
-00008f70: 6829 202d 3e20 5061 7468 207c 2073 7472  h) -> Path | str
-00008f80: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00008f90: 2073 6f63 6b65 745f 7061 7468 2069 6620   socket_path if 
-00008fa0: 7265 7175 6573 742e 7061 7261 6d20 656c  request.param el
-00008fb0: 7365 2073 7472 2873 6f63 6b65 745f 7061  se str(socket_pa
-00008fc0: 7468 290a 0a20 2020 2061 7379 6e63 2064  th)..    async d
-00008fd0: 6566 2074 6573 745f 6578 7472 615f 6174  ef test_extra_at
-00008fe0: 7472 6962 7574 6573 2873 656c 662c 2073  tributes(self, s
-00008ff0: 6f63 6b65 745f 7061 7468 3a20 5061 7468  ocket_path: Path
-00009000: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00009010: 2020 2061 7379 6e63 2077 6974 6820 6177     async with aw
-00009020: 6169 7420 6372 6561 7465 5f75 6e69 785f  ait create_unix_
-00009030: 6c69 7374 656e 6572 2873 6f63 6b65 745f  listener(socket_
-00009040: 7061 7468 2920 6173 206c 6973 7465 6e65  path) as listene
-00009050: 723a 0a20 2020 2020 2020 2020 2020 2072  r:.            r
-00009060: 6177 5f73 6f63 6b65 7420 3d20 6c69 7374  aw_socket = list
-00009070: 656e 6572 2e65 7874 7261 2853 6f63 6b65  ener.extra(Socke
-00009080: 7441 7474 7269 6275 7465 2e72 6177 5f73  tAttribute.raw_s
-00009090: 6f63 6b65 7429 0a20 2020 2020 2020 2020  ocket).         
-000090a0: 2020 2061 7373 6572 7420 6c69 7374 656e     assert listen
-000090b0: 6572 2e65 7874 7261 2853 6f63 6b65 7441  er.extra(SocketA
-000090c0: 7474 7269 6275 7465 2e66 616d 696c 7929  ttribute.family)
-000090d0: 203d 3d20 736f 636b 6574 2e41 465f 554e   == socket.AF_UN
-000090e0: 4958 0a20 2020 2020 2020 2020 2020 2061  IX.            a
-000090f0: 7373 6572 7420 280a 2020 2020 2020 2020  ssert (.        
-00009100: 2020 2020 2020 2020 6c69 7374 656e 6572          listener
-00009110: 2e65 7874 7261 2853 6f63 6b65 7441 7474  .extra(SocketAtt
-00009120: 7269 6275 7465 2e6c 6f63 616c 5f61 6464  ribute.local_add
-00009130: 7265 7373 290a 2020 2020 2020 2020 2020  ress).          
-00009140: 2020 2020 2020 3d3d 2072 6177 5f73 6f63        == raw_soc
-00009150: 6b65 742e 6765 7473 6f63 6b6e 616d 6528  ket.getsockname(
-00009160: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
-00009170: 2020 2020 2020 2020 2020 2020 7079 7465              pyte
-00009180: 7374 2e72 6169 7365 7328 0a20 2020 2020  st.raises(.     
-00009190: 2020 2020 2020 2020 2020 2054 7970 6564             Typed
-000091a0: 4174 7472 6962 7574 654c 6f6f 6b75 7045  AttributeLookupE
-000091b0: 7272 6f72 2c20 6c69 7374 656e 6572 2e65  rror, listener.e
-000091c0: 7874 7261 2c20 536f 636b 6574 4174 7472  xtra, SocketAttr
-000091d0: 6962 7574 652e 6c6f 6361 6c5f 706f 7274  ibute.local_port
-000091e0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-000091f0: 2020 2020 2020 2020 2020 2070 7974 6573             pytes
-00009200: 742e 7261 6973 6573 280a 2020 2020 2020  t.raises(.      
-00009210: 2020 2020 2020 2020 2020 5479 7065 6441            TypedA
-00009220: 7474 7269 6275 7465 4c6f 6f6b 7570 4572  ttributeLookupEr
-00009230: 726f 722c 0a20 2020 2020 2020 2020 2020  ror,.           
-00009240: 2020 2020 206c 6973 7465 6e65 722e 6578       listener.ex
-00009250: 7472 612c 0a20 2020 2020 2020 2020 2020  tra,.           
-00009260: 2020 2020 2053 6f63 6b65 7441 7474 7269       SocketAttri
-00009270: 6275 7465 2e72 656d 6f74 655f 6164 6472  bute.remote_addr
-00009280: 6573 732c 0a20 2020 2020 2020 2020 2020  ess,.           
-00009290: 2029 0a20 2020 2020 2020 2020 2020 2070   ).            p
-000092a0: 7974 6573 742e 7261 6973 6573 280a 2020  ytest.raises(.  
-000092b0: 2020 2020 2020 2020 2020 2020 2020 5479                Ty
-000092c0: 7065 6441 7474 7269 6275 7465 4c6f 6f6b  pedAttributeLook
-000092d0: 7570 4572 726f 722c 206c 6973 7465 6e65  upError, listene
-000092e0: 722e 6578 7472 612c 2053 6f63 6b65 7441  r.extra, SocketA
-000092f0: 7474 7269 6275 7465 2e72 656d 6f74 655f  ttribute.remote_
-00009300: 706f 7274 0a20 2020 2020 2020 2020 2020  port.           
-00009310: 2029 0a0a 2020 2020 6173 796e 6320 6465   )..    async de
-00009320: 6620 7465 7374 5f61 6363 6570 7428 7365  f test_accept(se
-00009330: 6c66 2c20 736f 636b 6574 5f70 6174 685f  lf, socket_path_
-00009340: 6f72 5f73 7472 3a20 5061 7468 207c 2073  or_str: Path | s
-00009350: 7472 2920 2d3e 204e 6f6e 653a 0a20 2020  tr) -> None:.   
-00009360: 2020 2020 2061 7379 6e63 2077 6974 6820       async with 
-00009370: 6177 6169 7420 6372 6561 7465 5f75 6e69  await create_uni
-00009380: 785f 6c69 7374 656e 6572 2873 6f63 6b65  x_listener(socke
-00009390: 745f 7061 7468 5f6f 725f 7374 7229 2061  t_path_or_str) a
-000093a0: 7320 6c69 7374 656e 6572 3a0a 2020 2020  s listener:.    
-000093b0: 2020 2020 2020 2020 636c 6965 6e74 203d          client =
-000093c0: 2073 6f63 6b65 742e 736f 636b 6574 2873   socket.socket(s
-000093d0: 6f63 6b65 742e 4146 5f55 4e49 5829 0a20  ocket.AF_UNIX). 
-000093e0: 2020 2020 2020 2020 2020 2063 6c69 656e             clien
-000093f0: 742e 7365 7474 696d 656f 7574 2831 290a  t.settimeout(1).
-00009400: 2020 2020 2020 2020 2020 2020 636c 6965              clie
-00009410: 6e74 2e63 6f6e 6e65 6374 2873 7472 2873  nt.connect(str(s
-00009420: 6f63 6b65 745f 7061 7468 5f6f 725f 7374  ocket_path_or_st
-00009430: 7229 290a 2020 2020 2020 2020 2020 2020  r)).            
-00009440: 7374 7265 616d 203d 2061 7761 6974 206c  stream = await l
-00009450: 6973 7465 6e65 722e 6163 6365 7074 2829  istener.accept()
-00009460: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
-00009470: 656e 742e 7365 6e64 616c 6c28 6222 626c  ent.sendall(b"bl
-00009480: 6168 2229 0a20 2020 2020 2020 2020 2020  ah").           
-00009490: 2072 6571 7565 7374 203d 2061 7761 6974   request = await
-000094a0: 2073 7472 6561 6d2e 7265 6365 6976 6528   stream.receive(
-000094b0: 290a 2020 2020 2020 2020 2020 2020 6177  ).            aw
-000094c0: 6169 7420 7374 7265 616d 2e73 656e 6428  ait stream.send(
-000094d0: 7265 7175 6573 745b 3a3a 2d31 5d29 0a20  request[::-1]). 
-000094e0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-000094f0: 7420 636c 6965 6e74 2e72 6563 7628 3130  t client.recv(10
-00009500: 3029 203d 3d20 6222 6861 6c62 220a 2020  0) == b"halb".  
-00009510: 2020 2020 2020 2020 2020 636c 6965 6e74            client
-00009520: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
-00009530: 2020 2020 2061 7761 6974 2073 7472 6561       await strea
-00009540: 6d2e 6163 6c6f 7365 2829 0a0a 2020 2020  m.aclose()..    
-00009550: 6173 796e 6320 6465 6620 7465 7374 5f73  async def test_s
-00009560: 6f63 6b65 745f 6f70 7469 6f6e 7328 7365  ocket_options(se
-00009570: 6c66 2c20 736f 636b 6574 5f70 6174 683a  lf, socket_path:
-00009580: 2050 6174 6829 202d 3e20 4e6f 6e65 3a0a   Path) -> None:.
-00009590: 2020 2020 2020 2020 6173 796e 6320 7769          async wi
-000095a0: 7468 2061 7761 6974 2063 7265 6174 655f  th await create_
-000095b0: 756e 6978 5f6c 6973 7465 6e65 7228 736f  unix_listener(so
-000095c0: 636b 6574 5f70 6174 6829 2061 7320 6c69  cket_path) as li
-000095d0: 7374 656e 6572 3a0a 2020 2020 2020 2020  stener:.        
-000095e0: 2020 2020 6c69 7374 656e 6572 5f73 6f63      listener_soc
-000095f0: 6b65 7420 3d20 6c69 7374 656e 6572 2e65  ket = listener.e
-00009600: 7874 7261 2853 6f63 6b65 7441 7474 7269  xtra(SocketAttri
-00009610: 6275 7465 2e72 6177 5f73 6f63 6b65 7429  bute.raw_socket)
-00009620: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-00009630: 6572 7420 6c69 7374 656e 6572 5f73 6f63  ert listener_soc
-00009640: 6b65 742e 6661 6d69 6c79 203d 3d20 736f  ket.family == so
-00009650: 636b 6574 2e41 6464 7265 7373 4661 6d69  cket.AddressFami
-00009660: 6c79 2e41 465f 554e 4958 0a20 2020 2020  ly.AF_UNIX.     
-00009670: 2020 2020 2020 206c 6973 7465 6e65 725f         listener_
-00009680: 736f 636b 6574 2e73 6574 736f 636b 6f70  socket.setsockop
-00009690: 7428 736f 636b 6574 2e53 4f4c 5f53 4f43  t(socket.SOL_SOC
-000096a0: 4b45 542c 2073 6f63 6b65 742e 534f 5f52  KET, socket.SO_R
-000096b0: 4356 4255 462c 2038 3030 3030 290a 2020  CVBUF, 80000).  
-000096c0: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-000096d0: 206c 6973 7465 6e65 725f 736f 636b 6574   listener_socket
-000096e0: 2e67 6574 736f 636b 6f70 7428 736f 636b  .getsockopt(sock
-000096f0: 6574 2e53 4f4c 5f53 4f43 4b45 542c 2073  et.SOL_SOCKET, s
-00009700: 6f63 6b65 742e 534f 5f52 4356 4255 4629  ocket.SO_RCVBUF)
-00009710: 2069 6e20 280a 2020 2020 2020 2020 2020   in (.          
-00009720: 2020 2020 2020 3830 3030 302c 0a20 2020        80000,.   
-00009730: 2020 2020 2020 2020 2020 2020 2031 3630               160
-00009740: 3030 302c 0a20 2020 2020 2020 2020 2020  000,.           
-00009750: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
-00009760: 636c 6965 6e74 203d 2073 6f63 6b65 742e  client = socket.
-00009770: 736f 636b 6574 286c 6973 7465 6e65 725f  socket(listener_
-00009780: 736f 636b 6574 2e66 616d 696c 7929 0a20  socket.family). 
-00009790: 2020 2020 2020 2020 2020 2063 6c69 656e             clien
-000097a0: 742e 7365 7474 696d 656f 7574 2831 290a  t.settimeout(1).
-000097b0: 2020 2020 2020 2020 2020 2020 636c 6965              clie
-000097c0: 6e74 2e63 6f6e 6e65 6374 286c 6973 7465  nt.connect(liste
-000097d0: 6e65 725f 736f 636b 6574 2e67 6574 736f  ner_socket.getso
-000097e0: 636b 6e61 6d65 2829 290a 0a20 2020 2020  ckname())..     
-000097f0: 2020 2020 2020 2061 7379 6e63 2077 6974         async wit
-00009800: 6820 6177 6169 7420 6c69 7374 656e 6572  h await listener
-00009810: 2e61 6363 6570 7428 2920 6173 2073 7472  .accept() as str
-00009820: 6561 6d3a 0a20 2020 2020 2020 2020 2020  eam:.           
-00009830: 2020 2020 2061 7373 6572 7420 7374 7265       assert stre
-00009840: 616d 2e65 7874 7261 2853 6f63 6b65 7441  am.extra(SocketA
-00009850: 7474 7269 6275 7465 2e72 6177 5f73 6f63  ttribute.raw_soc
-00009860: 6b65 7429 2e67 6574 7469 6d65 6f75 7428  ket).gettimeout(
-00009870: 2920 3d3d 2030 0a20 2020 2020 2020 2020  ) == 0.         
-00009880: 2020 2020 2020 2061 7373 6572 7420 7374         assert st
-00009890: 7265 616d 2e65 7874 7261 2853 6f63 6b65  ream.extra(Socke
-000098a0: 7441 7474 7269 6275 7465 2e66 616d 696c  tAttribute.famil
-000098b0: 7929 203d 3d20 6c69 7374 656e 6572 5f73  y) == listener_s
-000098c0: 6f63 6b65 742e 6661 6d69 6c79 0a0a 2020  ocket.family..  
-000098d0: 2020 2020 2020 2020 2020 636c 6965 6e74            client
-000098e0: 2e63 6c6f 7365 2829 0a0a 2020 2020 6173  .close()..    as
-000098f0: 796e 6320 6465 6620 7465 7374 5f73 656e  ync def test_sen
-00009900: 645f 6166 7465 725f 656f 6628 7365 6c66  d_after_eof(self
-00009910: 2c20 736f 636b 6574 5f70 6174 683a 2050  , socket_path: P
-00009920: 6174 6829 202d 3e20 4e6f 6e65 3a0a 2020  ath) -> None:.  
-00009930: 2020 2020 2020 6173 796e 6320 6465 6620        async def 
-00009940: 6861 6e64 6c65 2873 7472 6561 6d3a 2053  handle(stream: S
-00009950: 6f63 6b65 7453 7472 6561 6d29 202d 3e20  ocketStream) -> 
-00009960: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00009970: 2020 6173 796e 6320 7769 7468 2073 7472    async with str
-00009980: 6561 6d3a 0a20 2020 2020 2020 2020 2020  eam:.           
-00009990: 2020 2020 2061 7761 6974 2073 7472 6561       await strea
-000099a0: 6d2e 7365 6e64 2862 2248 656c 6c6f 5c6e  m.send(b"Hello\n
-000099b0: 2229 0a0a 2020 2020 2020 2020 6173 796e  ")..        asyn
-000099c0: 6320 7769 7468 2061 7761 6974 2063 7265  c with await cre
-000099d0: 6174 655f 756e 6978 5f6c 6973 7465 6e65  ate_unix_listene
-000099e0: 7228 0a20 2020 2020 2020 2020 2020 2073  r(.            s
-000099f0: 6f63 6b65 745f 7061 7468 0a20 2020 2020  ocket_path.     
-00009a00: 2020 2029 2061 7320 6c69 7374 656e 6572     ) as listener
-00009a10: 2c20 6372 6561 7465 5f74 6173 6b5f 6772  , create_task_gr
-00009a20: 6f75 7028 2920 6173 2074 673a 0a20 2020  oup() as tg:.   
-00009a30: 2020 2020 2020 2020 2074 672e 7374 6172           tg.star
-00009a40: 745f 736f 6f6e 286c 6973 7465 6e65 722e  t_soon(listener.
-00009a50: 7365 7276 652c 2068 616e 646c 6529 0a20  serve, handle). 
-00009a60: 2020 2020 2020 2020 2020 2061 7761 6974             await
-00009a70: 2077 6169 745f 616c 6c5f 7461 736b 735f   wait_all_tasks_
-00009a80: 626c 6f63 6b65 6428 290a 0a20 2020 2020  blocked()..     
-00009a90: 2020 2020 2020 2077 6974 6820 736f 636b         with sock
-00009aa0: 6574 2e73 6f63 6b65 7428 736f 636b 6574  et.socket(socket
-00009ab0: 2e41 465f 554e 4958 2920 6173 2063 6c69  .AF_UNIX) as cli
-00009ac0: 656e 743a 0a20 2020 2020 2020 2020 2020  ent:.           
-00009ad0: 2020 2020 2063 6c69 656e 742e 636f 6e6e       client.conn
-00009ae0: 6563 7428 7374 7228 736f 636b 6574 5f70  ect(str(socket_p
-00009af0: 6174 6829 290a 2020 2020 2020 2020 2020  ath)).          
-00009b00: 2020 2020 2020 636c 6965 6e74 2e73 6875        client.shu
-00009b10: 7464 6f77 6e28 736f 636b 6574 2e53 4855  tdown(socket.SHU
-00009b20: 545f 5752 290a 2020 2020 2020 2020 2020  T_WR).          
-00009b30: 2020 2020 2020 636c 6965 6e74 2e73 6574        client.set
-00009b40: 626c 6f63 6b69 6e67 2846 616c 7365 290a  blocking(False).
-00009b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b60: 7769 7468 2066 6169 6c5f 6166 7465 7228  with fail_after(
-00009b70: 3129 3a0a 2020 2020 2020 2020 2020 2020  1):.            
-00009b80: 2020 2020 2020 2020 7768 696c 6520 5472          while Tr
-00009b90: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
-00009ba0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00009bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009bc0: 2020 2020 2020 2020 2020 2020 206d 6573               mes
-00009bd0: 7361 6765 203d 2063 6c69 656e 742e 7265  sage = client.re
-00009be0: 6376 2831 3029 0a20 2020 2020 2020 2020  cv(10).         
-00009bf0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00009c00: 7863 6570 7420 426c 6f63 6b69 6e67 494f  xcept BlockingIO
-00009c10: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
-00009c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c30: 2020 2061 7761 6974 2073 6c65 6570 2830     await sleep(0
-00009c40: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00009c50: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00009c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c70: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-00009c80: 7274 206d 6573 7361 6765 203d 3d20 6222  rt message == b"
-00009c90: 4865 6c6c 6f5c 6e22 0a20 2020 2020 2020  Hello\n".       
-00009ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cb0: 2020 2020 2062 7265 616b 0a0a 2020 2020       break..    
-00009cc0: 2020 2020 2020 2020 7467 2e63 616e 6365          tg.cance
-00009cd0: 6c5f 7363 6f70 652e 6361 6e63 656c 2829  l_scope.cancel()
-00009ce0: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-00009cf0: 7465 7374 5f62 696e 645f 7477 6963 6528  test_bind_twice(
-00009d00: 7365 6c66 2c20 736f 636b 6574 5f70 6174  self, socket_pat
-00009d10: 683a 2050 6174 6829 202d 3e20 4e6f 6e65  h: Path) -> None
-00009d20: 3a0a 2020 2020 2020 2020 2222 2254 6573  :.        """Tes
-00009d30: 7420 7468 6174 2074 6865 2070 7265 7669  t that the previ
-00009d40: 6f75 7320 736f 636b 6574 2069 7320 7265  ous socket is re
-00009d50: 6d6f 7665 6420 6265 666f 7265 2062 696e  moved before bin
-00009d60: 6469 6e67 2074 6f20 7468 6520 7061 7468  ding to the path
-00009d70: 2e22 2222 0a20 2020 2020 2020 2066 6f72  .""".        for
-00009d80: 205f 2069 6e20 7261 6e67 6528 3229 3a0a   _ in range(2):.
-00009d90: 2020 2020 2020 2020 2020 2020 6173 796e              asyn
-00009da0: 6320 7769 7468 2061 7761 6974 2063 7265  c with await cre
-00009db0: 6174 655f 756e 6978 5f6c 6973 7465 6e65  ate_unix_listene
-00009dc0: 7228 736f 636b 6574 5f70 6174 6829 3a0a  r(socket_path):.
-00009dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009de0: 7061 7373 0a0a 2020 2020 6173 796e 6320  pass..    async 
-00009df0: 6465 6620 7465 7374 5f6c 6973 7465 6e69  def test_listeni
-00009e00: 6e67 5f62 7974 6573 5f70 6174 6828 7365  ng_bytes_path(se
-00009e10: 6c66 2c20 736f 636b 6574 5f70 6174 683a  lf, socket_path:
-00009e20: 2050 6174 6829 202d 3e20 4e6f 6e65 3a0a   Path) -> None:.
-00009e30: 2020 2020 2020 2020 6173 796e 6320 7769          async wi
-00009e40: 7468 2061 7761 6974 2063 7265 6174 655f  th await create_
-00009e50: 756e 6978 5f6c 6973 7465 6e65 7228 7374  unix_listener(st
-00009e60: 7228 736f 636b 6574 5f70 6174 6829 2e65  r(socket_path).e
-00009e70: 6e63 6f64 6528 2929 3a0a 2020 2020 2020  ncode()):.      
-00009e80: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00009e90: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
-00009ea0: 7069 6628 0a20 2020 2020 2020 2070 6c61  pif(.        pla
-00009eb0: 7466 6f72 6d2e 7379 7374 656d 2829 203d  tform.system() =
-00009ec0: 3d20 2244 6172 7769 6e22 2c20 7265 6173  = "Darwin", reas
-00009ed0: 6f6e 3d22 6d61 634f 5320 7265 7175 6972  on="macOS requir
-00009ee0: 6573 2076 616c 6964 2055 5446 2d38 2070  es valid UTF-8 p
-00009ef0: 6174 6873 220a 2020 2020 290a 2020 2020  aths".    ).    
-00009f00: 6173 796e 6320 6465 6620 7465 7374 5f6c  async def test_l
-00009f10: 6973 7465 6e69 6e67 5f69 6e76 616c 6964  istening_invalid
-00009f20: 5f61 7363 6969 2873 656c 662c 2073 6f63  _ascii(self, soc
-00009f30: 6b65 745f 7061 7468 3a20 5061 7468 2920  ket_path: Path) 
-00009f40: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00009f50: 2072 6561 6c5f 7061 7468 203d 2073 7472   real_path = str
-00009f60: 2873 6f63 6b65 745f 7061 7468 292e 656e  (socket_path).en
-00009f70: 636f 6465 2829 202b 2062 225c 7846 3022  code() + b"\xF0"
-00009f80: 0a20 2020 2020 2020 2061 7379 6e63 2077  .        async w
-00009f90: 6974 6820 6177 6169 7420 6372 6561 7465  ith await create
-00009fa0: 5f75 6e69 785f 6c69 7374 656e 6572 2872  _unix_listener(r
-00009fb0: 6561 6c5f 7061 7468 293a 0a20 2020 2020  eal_path):.     
-00009fc0: 2020 2020 2020 2070 6173 730a 0a0a 6173         pass...as
-00009fd0: 796e 6320 6465 6620 7465 7374 5f6d 756c  ync def test_mul
-00009fe0: 7469 5f6c 6973 7465 6e65 7228 746d 705f  ti_listener(tmp_
-00009ff0: 7061 7468 5f66 6163 746f 7279 3a20 5465  path_factory: Te
-0000a000: 6d70 5061 7468 4661 6374 6f72 7929 202d  mpPathFactory) -
-0000a010: 3e20 4e6f 6e65 3a0a 2020 2020 6173 796e  > None:.    asyn
-0000a020: 6320 6465 6620 6861 6e64 6c65 2873 7472  c def handle(str
-0000a030: 6561 6d3a 2053 6f63 6b65 7453 7472 6561  eam: SocketStrea
-0000a040: 6d29 202d 3e20 4e6f 6e65 3a0a 2020 2020  m) -> None:.    
-0000a050: 2020 2020 636c 6965 6e74 5f61 6464 7265      client_addre
-0000a060: 7373 6573 2e61 7070 656e 6428 7374 7265  sses.append(stre
-0000a070: 616d 2e65 7874 7261 2853 6f63 6b65 7441  am.extra(SocketA
-0000a080: 7474 7269 6275 7465 2e72 656d 6f74 655f  ttribute.remote_
-0000a090: 6164 6472 6573 7329 290a 2020 2020 2020  address)).      
-0000a0a0: 2020 6576 656e 742e 7365 7428 290a 2020    event.set().  
-0000a0b0: 2020 2020 2020 6177 6169 7420 7374 7265        await stre
-0000a0c0: 616d 2e61 636c 6f73 6528 290a 0a20 2020  am.aclose()..   
-0000a0d0: 2063 6c69 656e 745f 6164 6472 6573 7365   client_addresse
-0000a0e0: 733a 206c 6973 745b 7374 7220 7c20 4950  s: list[str | IP
-0000a0f0: 536f 636b 4164 6472 5479 7065 5d20 3d20  SockAddrType] = 
-0000a100: 5b5d 0a20 2020 206c 6973 7465 6e65 7273  [].    listeners
-0000a110: 3a20 6c69 7374 5b4c 6973 7465 6e65 725d  : list[Listener]
-0000a120: 203d 205b 6177 6169 7420 6372 6561 7465   = [await create
-0000a130: 5f74 6370 5f6c 6973 7465 6e65 7228 6c6f  _tcp_listener(lo
-0000a140: 6361 6c5f 686f 7374 3d22 6c6f 6361 6c68  cal_host="localh
-0000a150: 6f73 7422 295d 0a20 2020 2077 6974 6820  ost")].    with 
-0000a160: 7465 6d70 6669 6c65 2e54 656d 706f 7261  tempfile.Tempora
-0000a170: 7279 4469 7265 6374 6f72 7928 2920 6173  ryDirectory() as
-0000a180: 2070 6174 683a 0a20 2020 2020 2020 2069   path:.        i
-0000a190: 6620 7379 732e 706c 6174 666f 726d 2021  f sys.platform !
-0000a1a0: 3d20 2277 696e 3332 223a 0a20 2020 2020  = "win32":.     
-0000a1b0: 2020 2020 2020 206c 6973 7465 6e65 7273         listeners
-0000a1c0: 2e61 7070 656e 6428 6177 6169 7420 6372  .append(await cr
-0000a1d0: 6561 7465 5f75 6e69 785f 6c69 7374 656e  eate_unix_listen
-0000a1e0: 6572 2850 6174 6828 7061 7468 2920 2f20  er(Path(path) / 
-0000a1f0: 2273 6f63 6b65 7422 2929 0a0a 2020 2020  "socket"))..    
-0000a200: 2020 2020 6578 7065 6374 6564 5f61 6464      expected_add
-0000a210: 7265 7373 6573 3a20 6c69 7374 5b73 7472  resses: list[str
-0000a220: 207c 2049 5053 6f63 6b41 6464 7254 7970   | IPSockAddrTyp
-0000a230: 655d 203d 205b 5d0a 2020 2020 2020 2020  e] = [].        
-0000a240: 6173 796e 6320 7769 7468 204d 756c 7469  async with Multi
-0000a250: 4c69 7374 656e 6572 286c 6973 7465 6e65  Listener(listene
-0000a260: 7273 2920 6173 206d 756c 7469 5f6c 6973  rs) as multi_lis
-0000a270: 7465 6e65 723a 0a20 2020 2020 2020 2020  tener:.         
-0000a280: 2020 2061 7379 6e63 2077 6974 6820 6372     async with cr
-0000a290: 6561 7465 5f74 6173 6b5f 6772 6f75 7028  eate_task_group(
-0000a2a0: 2920 6173 2074 673a 0a20 2020 2020 2020  ) as tg:.       
-0000a2b0: 2020 2020 2020 2020 2074 672e 7374 6172           tg.star
-0000a2c0: 745f 736f 6f6e 286d 756c 7469 5f6c 6973  t_soon(multi_lis
-0000a2d0: 7465 6e65 722e 7365 7276 652c 2068 616e  tener.serve, han
-0000a2e0: 646c 6529 0a20 2020 2020 2020 2020 2020  dle).           
-0000a2f0: 2020 2020 2066 6f72 206c 6973 7465 6e65       for listene
-0000a300: 7220 696e 206d 756c 7469 5f6c 6973 7465  r in multi_liste
-0000a310: 6e65 722e 6c69 7374 656e 6572 733a 0a20  ner.listeners:. 
-0000a320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a330: 2020 2065 7665 6e74 203d 2045 7665 6e74     event = Event
-0000a340: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-0000a350: 2020 2020 2020 206c 6f63 616c 5f61 6464         local_add
-0000a360: 7265 7373 203d 206c 6973 7465 6e65 722e  ress = listener.
-0000a370: 6578 7472 6128 536f 636b 6574 4174 7472  extra(SocketAttr
-0000a380: 6962 7574 652e 6c6f 6361 6c5f 6164 6472  ibute.local_addr
-0000a390: 6573 7329 0a20 2020 2020 2020 2020 2020  ess).           
-0000a3a0: 2020 2020 2020 2020 2069 6620 280a 2020           if (.  
-0000a3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3c0: 2020 2020 2020 7379 732e 706c 6174 666f        sys.platfo
-0000a3d0: 726d 2021 3d20 2277 696e 3332 220a 2020  rm != "win32".  
-0000a3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3f0: 2020 2020 2020 616e 6420 6c69 7374 656e        and listen
-0000a400: 6572 2e65 7874 7261 2853 6f63 6b65 7441  er.extra(SocketA
-0000a410: 7474 7269 6275 7465 2e66 616d 696c 7929  ttribute.family)
-0000a420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a430: 2020 2020 2020 2020 203d 3d20 736f 636b           == sock
-0000a440: 6574 2e41 6464 7265 7373 4661 6d69 6c79  et.AddressFamily
-0000a450: 2e41 465f 554e 4958 0a20 2020 2020 2020  .AF_UNIX.       
-0000a460: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
-0000a470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a480: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
-0000a490: 7369 6e73 7461 6e63 6528 6c6f 6361 6c5f  sinstance(local_
-0000a4a0: 6164 6472 6573 732c 2073 7472 290a 2020  address, str).  
-0000a4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4c0: 2020 2020 2020 7374 7265 616d 3a20 536f        stream: So
-0000a4d0: 636b 6574 5374 7265 616d 203d 2061 7761  cketStream = awa
-0000a4e0: 6974 2063 6f6e 6e65 6374 5f75 6e69 7828  it connect_unix(
-0000a4f0: 6c6f 6361 6c5f 6164 6472 6573 7329 0a20  local_address). 
-0000a500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a510: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000a520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a530: 2061 7373 6572 7420 6973 696e 7374 616e   assert isinstan
-0000a540: 6365 286c 6f63 616c 5f61 6464 7265 7373  ce(local_address
-0000a550: 2c20 7475 706c 6529 0a20 2020 2020 2020  , tuple).       
-0000a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a570: 2073 7472 6561 6d20 3d20 6177 6169 7420   stream = await 
-0000a580: 636f 6e6e 6563 745f 7463 7028 2a6c 6f63  connect_tcp(*loc
-0000a590: 616c 5f61 6464 7265 7373 290a 0a20 2020  al_address)..   
-0000a5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5b0: 2065 7870 6563 7465 645f 6164 6472 6573   expected_addres
-0000a5c0: 7365 732e 6170 7065 6e64 280a 2020 2020  ses.append(.    
-0000a5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5e0: 2020 2020 7374 7265 616d 2e65 7874 7261      stream.extra
-0000a5f0: 2853 6f63 6b65 7441 7474 7269 6275 7465  (SocketAttribute
-0000a600: 2e6c 6f63 616c 5f61 6464 7265 7373 290a  .local_address).
-0000a610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a620: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000a630: 2020 2020 2020 2020 2020 6177 6169 7420            await 
-0000a640: 6576 656e 742e 7761 6974 2829 0a20 2020  event.wait().   
-0000a650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a660: 2061 7761 6974 2073 7472 6561 6d2e 6163   await stream.ac
-0000a670: 6c6f 7365 2829 0a0a 2020 2020 2020 2020  lose()..        
-0000a680: 2020 2020 2020 2020 7467 2e63 616e 6365          tg.cance
-0000a690: 6c5f 7363 6f70 652e 6361 6e63 656c 2829  l_scope.cancel()
-0000a6a0: 0a0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
-0000a6b0: 2063 6c69 656e 745f 6164 6472 6573 7365   client_addresse
-0000a6c0: 7320 3d3d 2065 7870 6563 7465 645f 6164  s == expected_ad
-0000a6d0: 6472 6573 7365 730a 0a0a 4070 7974 6573  dresses...@pytes
-0000a6e0: 742e 6d61 726b 2e6e 6574 776f 726b 0a40  t.mark.network.@
-0000a6f0: 7079 7465 7374 2e6d 6172 6b2e 7573 6566  pytest.mark.usef
-0000a700: 6978 7475 7265 7328 2263 6865 636b 5f61  ixtures("check_a
-0000a710: 7379 6e63 696f 5f62 7567 2229 0a63 6c61  syncio_bug").cla
-0000a720: 7373 2054 6573 7455 4450 536f 636b 6574  ss TestUDPSocket
-0000a730: 3a0a 2020 2020 6173 796e 6320 6465 6620  :.    async def 
-0000a740: 7465 7374 5f65 7874 7261 5f61 7474 7269  test_extra_attri
-0000a750: 6275 7465 7328 7365 6c66 2c20 6661 6d69  butes(self, fami
-0000a760: 6c79 3a20 416e 7949 5041 6464 7265 7373  ly: AnyIPAddress
-0000a770: 4661 6d69 6c79 2920 2d3e 204e 6f6e 653a  Family) -> None:
-0000a780: 0a20 2020 2020 2020 2061 7379 6e63 2077  .        async w
-0000a790: 6974 6820 6177 6169 7420 6372 6561 7465  ith await create
-0000a7a0: 5f75 6470 5f73 6f63 6b65 7428 0a20 2020  _udp_socket(.   
-0000a7b0: 2020 2020 2020 2020 2066 616d 696c 793d           family=
-0000a7c0: 6661 6d69 6c79 2c20 6c6f 6361 6c5f 686f  family, local_ho
-0000a7d0: 7374 3d22 6c6f 6361 6c68 6f73 7422 0a20  st="localhost". 
-0000a7e0: 2020 2020 2020 2029 2061 7320 7564 703a         ) as udp:
-0000a7f0: 0a20 2020 2020 2020 2020 2020 2072 6177  .            raw
-0000a800: 5f73 6f63 6b65 7420 3d20 7564 702e 6578  _socket = udp.ex
-0000a810: 7472 6128 536f 636b 6574 4174 7472 6962  tra(SocketAttrib
-0000a820: 7574 652e 7261 775f 736f 636b 6574 290a  ute.raw_socket).
-0000a830: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-0000a840: 7274 2072 6177 5f73 6f63 6b65 742e 6765  rt raw_socket.ge
-0000a850: 7474 696d 656f 7574 2829 203d 3d20 300a  ttimeout() == 0.
-0000a860: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-0000a870: 7274 2075 6470 2e65 7874 7261 2853 6f63  rt udp.extra(Soc
-0000a880: 6b65 7441 7474 7269 6275 7465 2e66 616d  ketAttribute.fam
-0000a890: 696c 7929 203d 3d20 6661 6d69 6c79 0a20  ily) == family. 
-0000a8a0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-0000a8b0: 7420 280a 2020 2020 2020 2020 2020 2020  t (.            
-0000a8c0: 2020 2020 7564 702e 6578 7472 6128 536f      udp.extra(So
-0000a8d0: 636b 6574 4174 7472 6962 7574 652e 6c6f  cketAttribute.lo
-0000a8e0: 6361 6c5f 6164 6472 6573 7329 203d 3d20  cal_address) == 
-0000a8f0: 7261 775f 736f 636b 6574 2e67 6574 736f  raw_socket.getso
-0000a900: 636b 6e61 6d65 2829 5b3a 325d 0a20 2020  ckname()[:2].   
-0000a910: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000a920: 2020 2020 2020 2061 7373 6572 7420 7564         assert ud
-0000a930: 702e 6578 7472 6128 536f 636b 6574 4174  p.extra(SocketAt
-0000a940: 7472 6962 7574 652e 6c6f 6361 6c5f 706f  tribute.local_po
-0000a950: 7274 2920 3d3d 2072 6177 5f73 6f63 6b65  rt) == raw_socke
-0000a960: 742e 6765 7473 6f63 6b6e 616d 6528 295b  t.getsockname()[
-0000a970: 315d 0a20 2020 2020 2020 2020 2020 2070  1].            p
-0000a980: 7974 6573 742e 7261 6973 6573 280a 2020  ytest.raises(.  
-0000a990: 2020 2020 2020 2020 2020 2020 2020 5479                Ty
-0000a9a0: 7065 6441 7474 7269 6275 7465 4c6f 6f6b  pedAttributeLook
-0000a9b0: 7570 4572 726f 722c 2075 6470 2e65 7874  upError, udp.ext
-0000a9c0: 7261 2c20 536f 636b 6574 4174 7472 6962  ra, SocketAttrib
-0000a9d0: 7574 652e 7265 6d6f 7465 5f61 6464 7265  ute.remote_addre
-0000a9e0: 7373 0a20 2020 2020 2020 2020 2020 2029  ss.            )
-0000a9f0: 0a20 2020 2020 2020 2020 2020 2070 7974  .            pyt
-0000aa00: 6573 742e 7261 6973 6573 280a 2020 2020  est.raises(.    
-0000aa10: 2020 2020 2020 2020 2020 2020 5479 7065              Type
-0000aa20: 6441 7474 7269 6275 7465 4c6f 6f6b 7570  dAttributeLookup
-0000aa30: 4572 726f 722c 2075 6470 2e65 7874 7261  Error, udp.extra
-0000aa40: 2c20 536f 636b 6574 4174 7472 6962 7574  , SocketAttribut
-0000aa50: 652e 7265 6d6f 7465 5f70 6f72 740a 2020  e.remote_port.  
-0000aa60: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-0000aa70: 2061 7379 6e63 2064 6566 2074 6573 745f   async def test_
-0000aa80: 7365 6e64 5f72 6563 6569 7665 2873 656c  send_receive(sel
-0000aa90: 662c 2066 616d 696c 793a 2041 6e79 4950  f, family: AnyIP
-0000aaa0: 4164 6472 6573 7346 616d 696c 7929 202d  AddressFamily) -
-0000aab0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0000aac0: 6173 796e 6320 7769 7468 2061 7761 6974  async with await
-0000aad0: 2063 7265 6174 655f 7564 705f 736f 636b   create_udp_sock
-0000aae0: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
-0000aaf0: 6c6f 6361 6c5f 686f 7374 3d22 6c6f 6361  local_host="loca
-0000ab00: 6c68 6f73 7422 2c20 6661 6d69 6c79 3d66  lhost", family=f
-0000ab10: 616d 696c 790a 2020 2020 2020 2020 2920  amily.        ) 
-0000ab20: 6173 2073 6f63 6b3a 0a20 2020 2020 2020  as sock:.       
-0000ab30: 2020 2020 2068 6f73 742c 2070 6f72 7420       host, port 
-0000ab40: 3d20 736f 636b 2e65 7874 7261 2853 6f63  = sock.extra(Soc
-0000ab50: 6b65 7441 7474 7269 6275 7465 2e6c 6f63  ketAttribute.loc
-0000ab60: 616c 5f61 6464 7265 7373 2920 2023 2074  al_address)  # t
-0000ab70: 7970 653a 2069 676e 6f72 655b 6d69 7363  ype: ignore[misc
-0000ab80: 5d0a 2020 2020 2020 2020 2020 2020 6177  ].            aw
-0000ab90: 6169 7420 736f 636b 2e73 656e 6474 6f28  ait sock.sendto(
-0000aba0: 6222 626c 6168 222c 2068 6f73 742c 2070  b"blah", host, p
-0000abb0: 6f72 7429 0a20 2020 2020 2020 2020 2020  ort).           
-0000abc0: 2072 6571 7565 7374 2c20 6164 6472 203d   request, addr =
-0000abd0: 2061 7761 6974 2073 6f63 6b2e 7265 6365   await sock.rece
-0000abe0: 6976 6528 290a 2020 2020 2020 2020 2020  ive().          
-0000abf0: 2020 6173 7365 7274 2072 6571 7565 7374    assert request
-0000ac00: 203d 3d20 6222 626c 6168 220a 2020 2020   == b"blah".    
-0000ac10: 2020 2020 2020 2020 6173 7365 7274 2061          assert a
-0000ac20: 6464 7220 3d3d 2073 6f63 6b2e 6578 7472  ddr == sock.extr
-0000ac30: 6128 536f 636b 6574 4174 7472 6962 7574  a(SocketAttribut
-0000ac40: 652e 6c6f 6361 6c5f 6164 6472 6573 7329  e.local_address)
-0000ac50: 0a0a 2020 2020 2020 2020 2020 2020 6177  ..            aw
-0000ac60: 6169 7420 736f 636b 2e73 656e 6474 6f28  ait sock.sendto(
-0000ac70: 6222 6861 6c62 222c 2068 6f73 742c 2070  b"halb", host, p
-0000ac80: 6f72 7429 0a20 2020 2020 2020 2020 2020  ort).           
-0000ac90: 2072 6573 706f 6e73 652c 2061 6464 7220   response, addr 
-0000aca0: 3d20 6177 6169 7420 736f 636b 2e72 6563  = await sock.rec
-0000acb0: 6569 7665 2829 0a20 2020 2020 2020 2020  eive().         
-0000acc0: 2020 2061 7373 6572 7420 7265 7370 6f6e     assert respon
-0000acd0: 7365 203d 3d20 6222 6861 6c62 220a 2020  se == b"halb".  
-0000ace0: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-0000acf0: 2061 6464 7220 3d3d 2028 686f 7374 2c20   addr == (host, 
-0000ad00: 706f 7274 290a 0a20 2020 2061 7379 6e63  port)..    async
-0000ad10: 2064 6566 2074 6573 745f 6974 6572 6174   def test_iterat
-0000ad20: 6528 7365 6c66 2c20 6661 6d69 6c79 3a20  e(self, family: 
-0000ad30: 416e 7949 5041 6464 7265 7373 4661 6d69  AnyIPAddressFami
-0000ad40: 6c79 2920 2d3e 204e 6f6e 653a 0a20 2020  ly) -> None:.   
-0000ad50: 2020 2020 2061 7379 6e63 2064 6566 2073       async def s
-0000ad60: 6572 7665 2829 202d 3e20 4e6f 6e65 3a0a  erve() -> None:.
-0000ad70: 2020 2020 2020 2020 2020 2020 6173 796e              asyn
-0000ad80: 6320 666f 7220 7061 636b 6574 2c20 6164  c for packet, ad
-0000ad90: 6472 2069 6e20 7365 7276 6572 3a0a 2020  dr in server:.  
-0000ada0: 2020 2020 2020 2020 2020 2020 2020 6177                aw
-0000adb0: 6169 7420 7365 7276 6572 2e73 656e 6428  ait server.send(
-0000adc0: 2870 6163 6b65 745b 3a3a 2d31 5d2c 2061  (packet[::-1], a
-0000add0: 6464 7229 290a 0a20 2020 2020 2020 2061  ddr))..        a
-0000ade0: 7379 6e63 2077 6974 6820 6177 6169 7420  sync with await 
-0000adf0: 6372 6561 7465 5f75 6470 5f73 6f63 6b65  create_udp_socke
-0000ae00: 7428 0a20 2020 2020 2020 2020 2020 2066  t(.            f
-0000ae10: 616d 696c 793d 6661 6d69 6c79 2c20 6c6f  amily=family, lo
-0000ae20: 6361 6c5f 686f 7374 3d22 6c6f 6361 6c68  cal_host="localh
-0000ae30: 6f73 7422 0a20 2020 2020 2020 2029 2061  ost".        ) a
-0000ae40: 7320 7365 7276 6572 3a0a 2020 2020 2020  s server:.      
-0000ae50: 2020 2020 2020 686f 7374 2c20 706f 7274        host, port
-0000ae60: 203d 2073 6572 7665 722e 6578 7472 6128   = server.extra(
-0000ae70: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
-0000ae80: 5b6d 6973 635d 0a20 2020 2020 2020 2020  [misc].         
-0000ae90: 2020 2020 2020 2053 6f63 6b65 7441 7474         SocketAtt
-0000aea0: 7269 6275 7465 2e6c 6f63 616c 5f61 6464  ribute.local_add
-0000aeb0: 7265 7373 0a20 2020 2020 2020 2020 2020  ress.           
-0000aec0: 2029 0a20 2020 2020 2020 2020 2020 2061   ).            a
-0000aed0: 7379 6e63 2077 6974 6820 6177 6169 7420  sync with await 
-0000aee0: 6372 6561 7465 5f75 6470 5f73 6f63 6b65  create_udp_socke
-0000aef0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-0000af00: 2020 2066 616d 696c 793d 6661 6d69 6c79     family=family
-0000af10: 2c20 6c6f 6361 6c5f 686f 7374 3d22 6c6f  , local_host="lo
-0000af20: 6361 6c68 6f73 7422 0a20 2020 2020 2020  calhost".       
-0000af30: 2020 2020 2029 2061 7320 636c 6965 6e74       ) as client
-0000af40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000af50: 2020 6173 796e 6320 7769 7468 2063 7265    async with cre
-0000af60: 6174 655f 7461 736b 5f67 726f 7570 2829  ate_task_group()
-0000af70: 2061 7320 7467 3a0a 2020 2020 2020 2020   as tg:.        
-0000af80: 2020 2020 2020 2020 2020 2020 7467 2e73              tg.s
-0000af90: 7461 7274 5f73 6f6f 6e28 7365 7276 6529  tart_soon(serve)
-0000afa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000afb0: 2020 2020 2061 7761 6974 2063 6c69 656e       await clien
-0000afc0: 742e 7365 6e64 746f 2862 2246 4f4f 4241  t.sendto(b"FOOBA
-0000afd0: 5222 2c20 686f 7374 2c20 706f 7274 290a  R", host, port).
-0000afe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aff0: 2020 2020 6173 7365 7274 2061 7761 6974      assert await
-0000b000: 2063 6c69 656e 742e 7265 6365 6976 6528   client.receive(
-0000b010: 2920 3d3d 2028 6222 5241 424f 4f46 222c  ) == (b"RABOOF",
-0000b020: 2028 686f 7374 2c20 706f 7274 2929 0a20   (host, port)). 
-0000b030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b040: 2020 2061 7761 6974 2063 6c69 656e 742e     await client.
-0000b050: 7365 6e64 746f 2862 2231 3233 3435 3622  sendto(b"123456"
-0000b060: 2c20 686f 7374 2c20 706f 7274 290a 2020  , host, port).  
-0000b070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b080: 2020 6173 7365 7274 2061 7761 6974 2063    assert await c
-0000b090: 6c69 656e 742e 7265 6365 6976 6528 2920  lient.receive() 
-0000b0a0: 3d3d 2028 6222 3635 3433 3231 222c 2028  == (b"654321", (
-0000b0b0: 686f 7374 2c20 706f 7274 2929 0a20 2020  host, port)).   
-0000b0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0d0: 2074 672e 6361 6e63 656c 5f73 636f 7065   tg.cancel_scope
-0000b0e0: 2e63 616e 6365 6c28 290a 0a20 2020 2040  .cancel()..    @
-0000b0f0: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
-0000b100: 6966 280a 2020 2020 2020 2020 6e6f 7420  if(.        not 
-0000b110: 6861 7361 7474 7228 736f 636b 6574 2c20  hasattr(socket, 
-0000b120: 2253 4f5f 5245 5553 4550 4f52 5422 292c  "SO_REUSEPORT"),
-0000b130: 2072 6561 736f 6e3d 2253 4f5f 5245 5553   reason="SO_REUS
-0000b140: 4550 4f52 5420 6f70 7469 6f6e 206e 6f74  EPORT option not
-0000b150: 2073 7570 706f 7274 6564 220a 2020 2020   supported".    
-0000b160: 290a 2020 2020 6173 796e 6320 6465 6620  ).    async def 
-0000b170: 7465 7374 5f72 6575 7365 5f70 6f72 7428  test_reuse_port(
-0000b180: 7365 6c66 2c20 6661 6d69 6c79 3a20 416e  self, family: An
-0000b190: 7949 5041 6464 7265 7373 4661 6d69 6c79  yIPAddressFamily
-0000b1a0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-0000b1b0: 2020 2061 7379 6e63 2077 6974 6820 6177     async with aw
-0000b1c0: 6169 7420 6372 6561 7465 5f75 6470 5f73  ait create_udp_s
-0000b1d0: 6f63 6b65 7428 0a20 2020 2020 2020 2020  ocket(.         
-0000b1e0: 2020 2066 616d 696c 793d 6661 6d69 6c79     family=family
-0000b1f0: 2c20 6c6f 6361 6c5f 686f 7374 3d22 6c6f  , local_host="lo
-0000b200: 6361 6c68 6f73 7422 2c20 7265 7573 655f  calhost", reuse_
-0000b210: 706f 7274 3d54 7275 650a 2020 2020 2020  port=True.      
-0000b220: 2020 2920 6173 2075 6470 3a0a 2020 2020    ) as udp:.    
-0000b230: 2020 2020 2020 2020 706f 7274 203d 2075          port = u
-0000b240: 6470 2e65 7874 7261 2853 6f63 6b65 7441  dp.extra(SocketA
-0000b250: 7474 7269 6275 7465 2e6c 6f63 616c 5f70  ttribute.local_p
-0000b260: 6f72 7429 0a20 2020 2020 2020 2020 2020  ort).           
-0000b270: 2061 7373 6572 7420 706f 7274 2021 3d20   assert port != 
-0000b280: 300a 2020 2020 2020 2020 2020 2020 6173  0.            as
-0000b290: 796e 6320 7769 7468 2061 7761 6974 2063  ync with await c
-0000b2a0: 7265 6174 655f 7564 705f 736f 636b 6574  reate_udp_socket
-0000b2b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000b2c0: 2020 6661 6d69 6c79 3d66 616d 696c 792c    family=family,
-0000b2d0: 206c 6f63 616c 5f68 6f73 743d 226c 6f63   local_host="loc
-0000b2e0: 616c 686f 7374 222c 206c 6f63 616c 5f70  alhost", local_p
-0000b2f0: 6f72 743d 706f 7274 2c20 7265 7573 655f  ort=port, reuse_
-0000b300: 706f 7274 3d54 7275 650a 2020 2020 2020  port=True.      
-0000b310: 2020 2020 2020 2920 6173 2075 6470 323a        ) as udp2:
-0000b320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b330: 2061 7373 6572 7420 706f 7274 203d 3d20   assert port == 
-0000b340: 7564 7032 2e65 7874 7261 2853 6f63 6b65  udp2.extra(Socke
-0000b350: 7441 7474 7269 6275 7465 2e6c 6f63 616c  tAttribute.local
-0000b360: 5f70 6f72 7429 0a0a 2020 2020 6173 796e  _port)..    asyn
-0000b370: 6320 6465 6620 7465 7374 5f63 6f6e 6375  c def test_concu
-0000b380: 7272 656e 745f 7265 6365 6976 6528 7365  rrent_receive(se
-0000b390: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-0000b3a0: 2020 2020 2061 7379 6e63 2077 6974 6820       async with 
-0000b3b0: 6177 6169 7420 6372 6561 7465 5f75 6470  await create_udp
-0000b3c0: 5f73 6f63 6b65 7428 0a20 2020 2020 2020  _socket(.       
-0000b3d0: 2020 2020 2066 616d 696c 793d 4164 6472       family=Addr
-0000b3e0: 6573 7346 616d 696c 792e 4146 5f49 4e45  essFamily.AF_INE
-0000b3f0: 542c 206c 6f63 616c 5f68 6f73 743d 226c  T, local_host="l
-0000b400: 6f63 616c 686f 7374 220a 2020 2020 2020  ocalhost".      
-0000b410: 2020 2920 6173 2075 6470 3a0a 2020 2020    ) as udp:.    
-0000b420: 2020 2020 2020 2020 6173 796e 6320 7769          async wi
-0000b430: 7468 2063 7265 6174 655f 7461 736b 5f67  th create_task_g
-0000b440: 726f 7570 2829 2061 7320 7467 3a0a 2020  roup() as tg:.  
-0000b450: 2020 2020 2020 2020 2020 2020 2020 7467                tg
-0000b460: 2e73 7461 7274 5f73 6f6f 6e28 7564 702e  .start_soon(udp.
-0000b470: 7265 6365 6976 6529 0a20 2020 2020 2020  receive).       
-0000b480: 2020 2020 2020 2020 2061 7761 6974 2077           await w
-0000b490: 6169 745f 616c 6c5f 7461 736b 735f 626c  ait_all_tasks_bl
-0000b4a0: 6f63 6b65 6428 290a 2020 2020 2020 2020  ocked().        
-0000b4b0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-0000b4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4d0: 2077 6974 6820 7079 7465 7374 2e72 6169   with pytest.rai
-0000b4e0: 7365 7328 4275 7379 5265 736f 7572 6365  ses(BusyResource
-0000b4f0: 4572 726f 7229 2061 7320 6578 633a 0a20  Error) as exc:. 
-0000b500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b510: 2020 2020 2020 2061 7761 6974 2075 6470         await udp
-0000b520: 2e72 6563 6569 7665 2829 0a0a 2020 2020  .receive()..    
-0000b530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b540: 6578 632e 6d61 7463 6828 2261 6c72 6561  exc.match("alrea
-0000b550: 6479 2072 6561 6469 6e67 2066 726f 6d22  dy reading from"
-0000b560: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000b570: 2020 6669 6e61 6c6c 793a 0a20 2020 2020    finally:.     
-0000b580: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000b590: 672e 6361 6e63 656c 5f73 636f 7065 2e63  g.cancel_scope.c
-0000b5a0: 616e 6365 6c28 290a 0a20 2020 2061 7379  ancel()..    asy
-0000b5b0: 6e63 2064 6566 2074 6573 745f 636c 6f73  nc def test_clos
-0000b5c0: 655f 6475 7269 6e67 5f72 6563 6569 7665  e_during_receive
-0000b5d0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-0000b5e0: 2020 2020 2020 2020 6173 796e 6320 6465          async de
-0000b5f0: 6620 636c 6f73 655f 7768 656e 5f62 6c6f  f close_when_blo
-0000b600: 636b 6564 2829 202d 3e20 4e6f 6e65 3a0a  cked() -> None:.
-0000b610: 2020 2020 2020 2020 2020 2020 6177 6169              awai
-0000b620: 7420 7761 6974 5f61 6c6c 5f74 6173 6b73  t wait_all_tasks
-0000b630: 5f62 6c6f 636b 6564 2829 0a20 2020 2020  _blocked().     
-0000b640: 2020 2020 2020 2061 7761 6974 2075 6470         await udp
-0000b650: 2e61 636c 6f73 6528 290a 0a20 2020 2020  .aclose()..     
-0000b660: 2020 2061 7379 6e63 2077 6974 6820 6177     async with aw
-0000b670: 6169 7420 6372 6561 7465 5f75 6470 5f73  ait create_udp_s
-0000b680: 6f63 6b65 7428 0a20 2020 2020 2020 2020  ocket(.         
-0000b690: 2020 2066 616d 696c 793d 4164 6472 6573     family=Addres
-0000b6a0: 7346 616d 696c 792e 4146 5f49 4e45 542c  sFamily.AF_INET,
-0000b6b0: 206c 6f63 616c 5f68 6f73 743d 226c 6f63   local_host="loc
-0000b6c0: 616c 686f 7374 220a 2020 2020 2020 2020  alhost".        
-0000b6d0: 2920 6173 2075 6470 3a0a 2020 2020 2020  ) as udp:.      
-0000b6e0: 2020 2020 2020 6173 796e 6320 7769 7468        async with
-0000b6f0: 2063 7265 6174 655f 7461 736b 5f67 726f   create_task_gro
-0000b700: 7570 2829 2061 7320 7467 3a0a 2020 2020  up() as tg:.    
-0000b710: 2020 2020 2020 2020 2020 2020 7467 2e73              tg.s
-0000b720: 7461 7274 5f73 6f6f 6e28 636c 6f73 655f  tart_soon(close_
-0000b730: 7768 656e 5f62 6c6f 636b 6564 290a 2020  when_blocked).  
-0000b740: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-0000b750: 7468 2070 7974 6573 742e 7261 6973 6573  th pytest.raises
-0000b760: 2843 6c6f 7365 6452 6573 6f75 7263 6545  (ClosedResourceE
-0000b770: 7272 6f72 293a 0a20 2020 2020 2020 2020  rror):.         
-0000b780: 2020 2020 2020 2020 2020 2061 7761 6974             await
-0000b790: 2075 6470 2e72 6563 6569 7665 2829 0a0a   udp.receive()..
-0000b7a0: 2020 2020 6173 796e 6320 6465 6620 7465      async def te
-0000b7b0: 7374 5f72 6563 6569 7665 5f61 6674 6572  st_receive_after
-0000b7c0: 5f63 6c6f 7365 2873 656c 6629 202d 3e20  _close(self) -> 
-0000b7d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7564  None:.        ud
-0000b7e0: 7020 3d20 6177 6169 7420 6372 6561 7465  p = await create
-0000b7f0: 5f75 6470 5f73 6f63 6b65 7428 0a20 2020  _udp_socket(.   
-0000b800: 2020 2020 2020 2020 2066 616d 696c 793d           family=
-0000b810: 4164 6472 6573 7346 616d 696c 792e 4146  AddressFamily.AF
-0000b820: 5f49 4e45 542c 206c 6f63 616c 5f68 6f73  _INET, local_hos
-0000b830: 743d 226c 6f63 616c 686f 7374 220a 2020  t="localhost".  
-0000b840: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000b850: 6177 6169 7420 7564 702e 6163 6c6f 7365  await udp.aclose
-0000b860: 2829 0a20 2020 2020 2020 2077 6974 6820  ().        with 
-0000b870: 7079 7465 7374 2e72 6169 7365 7328 436c  pytest.raises(Cl
-0000b880: 6f73 6564 5265 736f 7572 6365 4572 726f  osedResourceErro
-0000b890: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-0000b8a0: 6177 6169 7420 7564 702e 7265 6365 6976  await udp.receiv
-0000b8b0: 6528 290a 0a20 2020 2061 7379 6e63 2064  e()..    async d
-0000b8c0: 6566 2074 6573 745f 7365 6e64 5f61 6674  ef test_send_aft
-0000b8d0: 6572 5f63 6c6f 7365 2873 656c 6629 202d  er_close(self) -
-0000b8e0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0000b8f0: 7564 7020 3d20 6177 6169 7420 6372 6561  udp = await crea
-0000b900: 7465 5f75 6470 5f73 6f63 6b65 7428 0a20  te_udp_socket(. 
-0000b910: 2020 2020 2020 2020 2020 2066 616d 696c             famil
-0000b920: 793d 4164 6472 6573 7346 616d 696c 792e  y=AddressFamily.
-0000b930: 4146 5f49 4e45 542c 206c 6f63 616c 5f68  AF_INET, local_h
-0000b940: 6f73 743d 226c 6f63 616c 686f 7374 220a  ost="localhost".
-0000b950: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000b960: 2020 686f 7374 2c20 706f 7274 203d 2075    host, port = u
-0000b970: 6470 2e65 7874 7261 2853 6f63 6b65 7441  dp.extra(SocketA
-0000b980: 7474 7269 6275 7465 2e6c 6f63 616c 5f61  ttribute.local_a
-0000b990: 6464 7265 7373 2920 2023 2074 7970 653a  ddress)  # type:
-0000b9a0: 2069 676e 6f72 655b 6d69 7363 5d0a 2020   ignore[misc].  
-0000b9b0: 2020 2020 2020 6177 6169 7420 7564 702e        await udp.
-0000b9c0: 6163 6c6f 7365 2829 0a20 2020 2020 2020  aclose().       
-0000b9d0: 2077 6974 6820 7079 7465 7374 2e72 6169   with pytest.rai
-0000b9e0: 7365 7328 436c 6f73 6564 5265 736f 7572  ses(ClosedResour
-0000b9f0: 6365 4572 726f 7229 3a0a 2020 2020 2020  ceError):.      
-0000ba00: 2020 2020 2020 6177 6169 7420 7564 702e        await udp.
-0000ba10: 7365 6e64 746f 2862 2266 6f6f 222c 2068  sendto(b"foo", h
-0000ba20: 6f73 742c 2070 6f72 7429 0a0a 2020 2020  ost, port)..    
-0000ba30: 6173 796e 6320 6465 6620 7465 7374 5f63  async def test_c
-0000ba40: 7265 6174 655f 756e 626f 756e 645f 736f  reate_unbound_so
-0000ba50: 636b 6574 2873 656c 662c 2066 616d 696c  cket(self, famil
-0000ba60: 793a 2041 6e79 4950 4164 6472 6573 7346  y: AnyIPAddressF
-0000ba70: 616d 696c 7929 202d 3e20 4e6f 6e65 3a0a  amily) -> None:.
-0000ba80: 2020 2020 2020 2020 2222 2252 6567 7265          """Regre
-0000ba90: 7373 696f 6e20 7465 7374 2066 6f72 2023  ssion test for #
-0000baa0: 3336 302e 2222 220a 2020 2020 2020 2020  360.""".        
-0000bab0: 6173 796e 6320 7769 7468 2061 7761 6974  async with await
-0000bac0: 2063 7265 6174 655f 7564 705f 736f 636b   create_udp_sock
-0000bad0: 6574 2866 616d 696c 793d 6661 6d69 6c79  et(family=family
-0000bae0: 2920 6173 2075 6470 3a0a 2020 2020 2020  ) as udp:.      
-0000baf0: 2020 2020 2020 6c6f 6361 6c5f 6164 6472        local_addr
-0000bb00: 6573 7320 3d20 6361 7374 280a 2020 2020  ess = cast(.    
-0000bb10: 2020 2020 2020 2020 2020 2020 4950 536f              IPSo
-0000bb20: 636b 4164 6472 5479 7065 2c20 7564 702e  ckAddrType, udp.
-0000bb30: 6578 7472 6128 536f 636b 6574 4174 7472  extra(SocketAttr
-0000bb40: 6962 7574 652e 6c6f 6361 6c5f 6164 6472  ibute.local_addr
-0000bb50: 6573 7329 0a20 2020 2020 2020 2020 2020  ess).           
-0000bb60: 2029 0a20 2020 2020 2020 2020 2020 2061   ).            a
-0000bb70: 7373 6572 7420 6c6f 6361 6c5f 6164 6472  ssert local_addr
-0000bb80: 6573 735b 315d 203e 2030 0a0a 0a40 7079  ess[1] > 0...@py
-0000bb90: 7465 7374 2e6d 6172 6b2e 6e65 7477 6f72  test.mark.networ
-0000bba0: 6b0a 4070 7974 6573 742e 6d61 726b 2e75  k.@pytest.mark.u
-0000bbb0: 7365 6669 7874 7572 6573 2822 6368 6563  sefixtures("chec
-0000bbc0: 6b5f 6173 796e 6369 6f5f 6275 6722 290a  k_asyncio_bug").
-0000bbd0: 636c 6173 7320 5465 7374 436f 6e6e 6563  class TestConnec
-0000bbe0: 7465 6455 4450 536f 636b 6574 3a0a 2020  tedUDPSocket:.  
-0000bbf0: 2020 6173 796e 6320 6465 6620 7465 7374    async def test
-0000bc00: 5f65 7874 7261 5f61 7474 7269 6275 7465  _extra_attribute
-0000bc10: 7328 7365 6c66 2c20 6661 6d69 6c79 3a20  s(self, family: 
-0000bc20: 416e 7949 5041 6464 7265 7373 4661 6d69  AnyIPAddressFami
-0000bc30: 6c79 2920 2d3e 204e 6f6e 653a 0a20 2020  ly) -> None:.   
-0000bc40: 2020 2020 2061 7379 6e63 2077 6974 6820       async with 
-0000bc50: 6177 6169 7420 6372 6561 7465 5f63 6f6e  await create_con
-0000bc60: 6e65 6374 6564 5f75 6470 5f73 6f63 6b65  nected_udp_socke
-0000bc70: 7428 0a20 2020 2020 2020 2020 2020 2022  t(.            "
-0000bc80: 6c6f 6361 6c68 6f73 7422 2c20 3530 3030  localhost", 5000
-0000bc90: 2c20 6661 6d69 6c79 3d66 616d 696c 790a  , family=family.
-0000bca0: 2020 2020 2020 2020 2920 6173 2075 6470          ) as udp
-0000bcb0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-0000bcc0: 775f 736f 636b 6574 203d 2075 6470 2e65  w_socket = udp.e
-0000bcd0: 7874 7261 2853 6f63 6b65 7441 7474 7269  xtra(SocketAttri
-0000bce0: 6275 7465 2e72 6177 5f73 6f63 6b65 7429  bute.raw_socket)
-0000bcf0: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-0000bd00: 6572 7420 7564 702e 6578 7472 6128 536f  ert udp.extra(So
-0000bd10: 636b 6574 4174 7472 6962 7574 652e 6661  cketAttribute.fa
-0000bd20: 6d69 6c79 2920 3d3d 2066 616d 696c 790a  mily) == family.
-0000bd30: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-0000bd40: 7274 2028 0a20 2020 2020 2020 2020 2020  rt (.           
-0000bd50: 2020 2020 2075 6470 2e65 7874 7261 2853       udp.extra(S
-0000bd60: 6f63 6b65 7441 7474 7269 6275 7465 2e6c  ocketAttribute.l
-0000bd70: 6f63 616c 5f61 6464 7265 7373 2920 3d3d  ocal_address) ==
-0000bd80: 2072 6177 5f73 6f63 6b65 742e 6765 7473   raw_socket.gets
-0000bd90: 6f63 6b6e 616d 6528 295b 3a32 5d0a 2020  ockname()[:2].  
-0000bda0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000bdb0: 2020 2020 2020 2020 6173 7365 7274 2075          assert u
-0000bdc0: 6470 2e65 7874 7261 2853 6f63 6b65 7441  dp.extra(SocketA
-0000bdd0: 7474 7269 6275 7465 2e6c 6f63 616c 5f70  ttribute.local_p
-0000bde0: 6f72 7429 203d 3d20 7261 775f 736f 636b  ort) == raw_sock
-0000bdf0: 6574 2e67 6574 736f 636b 6e61 6d65 2829  et.getsockname()
-0000be00: 5b31 5d0a 2020 2020 2020 2020 2020 2020  [1].            
-0000be10: 6173 7365 7274 2028 0a20 2020 2020 2020  assert (.       
-0000be20: 2020 2020 2020 2020 2075 6470 2e65 7874           udp.ext
-0000be30: 7261 2853 6f63 6b65 7441 7474 7269 6275  ra(SocketAttribu
-0000be40: 7465 2e72 656d 6f74 655f 6164 6472 6573  te.remote_addres
-0000be50: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
-0000be60: 2020 203d 3d20 7261 775f 736f 636b 6574     == raw_socket
-0000be70: 2e67 6574 7065 6572 6e61 6d65 2829 5b3a  .getpeername()[:
-0000be80: 325d 0a20 2020 2020 2020 2020 2020 2029  2].            )
-0000be90: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-0000bea0: 6572 7420 7564 702e 6578 7472 6128 536f  ert udp.extra(So
-0000beb0: 636b 6574 4174 7472 6962 7574 652e 7265  cketAttribute.re
-0000bec0: 6d6f 7465 5f70 6f72 7429 203d 3d20 3530  mote_port) == 50
-0000bed0: 3030 0a0a 2020 2020 6173 796e 6320 6465  00..    async de
-0000bee0: 6620 7465 7374 5f73 656e 645f 7265 6365  f test_send_rece
-0000bef0: 6976 6528 7365 6c66 2c20 6661 6d69 6c79  ive(self, family
-0000bf00: 3a20 416e 7949 5041 6464 7265 7373 4661  : AnyIPAddressFa
-0000bf10: 6d69 6c79 2920 2d3e 204e 6f6e 653a 0a20  mily) -> None:. 
-0000bf20: 2020 2020 2020 2061 7379 6e63 2077 6974         async wit
-0000bf30: 6820 6177 6169 7420 6372 6561 7465 5f75  h await create_u
-0000bf40: 6470 5f73 6f63 6b65 7428 0a20 2020 2020  dp_socket(.     
-0000bf50: 2020 2020 2020 2066 616d 696c 793d 6661         family=fa
-0000bf60: 6d69 6c79 2c20 6c6f 6361 6c5f 686f 7374  mily, local_host
-0000bf70: 3d22 6c6f 6361 6c68 6f73 7422 0a20 2020  ="localhost".   
-0000bf80: 2020 2020 2029 2061 7320 7564 7031 3a0a       ) as udp1:.
-0000bf90: 2020 2020 2020 2020 2020 2020 686f 7374              host
-0000bfa0: 2c20 706f 7274 203d 2075 6470 312e 6578  , port = udp1.ex
-0000bfb0: 7472 6128 536f 636b 6574 4174 7472 6962  tra(SocketAttrib
-0000bfc0: 7574 652e 6c6f 6361 6c5f 6164 6472 6573  ute.local_addres
-0000bfd0: 7329 2020 2320 7479 7065 3a20 6967 6e6f  s)  # type: igno
-0000bfe0: 7265 5b6d 6973 635d 0a20 2020 2020 2020  re[misc].       
-0000bff0: 2020 2020 2061 7379 6e63 2077 6974 6820       async with 
-0000c000: 6177 6169 7420 6372 6561 7465 5f63 6f6e  await create_con
-0000c010: 6e65 6374 6564 5f75 6470 5f73 6f63 6b65  nected_udp_socke
-0000c020: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-0000c030: 2020 2068 6f73 742c 2070 6f72 742c 206c     host, port, l
-0000c040: 6f63 616c 5f68 6f73 743d 226c 6f63 616c  ocal_host="local
-0000c050: 686f 7374 222c 2066 616d 696c 793d 6661  host", family=fa
-0000c060: 6d69 6c79 0a20 2020 2020 2020 2020 2020  mily.           
-0000c070: 2029 2061 7320 7564 7032 3a0a 2020 2020   ) as udp2:.    
-0000c080: 2020 2020 2020 2020 2020 2020 686f 7374              host
-0000c090: 2c20 706f 7274 203d 2075 6470 322e 6578  , port = udp2.ex
-0000c0a0: 7472 6128 0a20 2020 2020 2020 2020 2020  tra(.           
-0000c0b0: 2020 2020 2020 2020 2053 6f63 6b65 7441           SocketA
-0000c0c0: 7474 7269 6275 7465 2e6c 6f63 616c 5f61  ttribute.local_a
-0000c0d0: 6464 7265 7373 2020 2320 7479 7065 3a20  ddress  # type: 
-0000c0e0: 6967 6e6f 7265 5b6d 6973 635d 0a20 2020  ignore[misc].   
-0000c0f0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0000c100: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000c110: 7761 6974 2075 6470 322e 7365 6e64 2862  wait udp2.send(b
-0000c120: 2262 6c61 6822 290a 2020 2020 2020 2020  "blah").        
-0000c130: 2020 2020 2020 2020 7265 7175 6573 7420          request 
-0000c140: 3d20 6177 6169 7420 7564 7031 2e72 6563  = await udp1.rec
-0000c150: 6569 7665 2829 0a20 2020 2020 2020 2020  eive().         
-0000c160: 2020 2020 2020 2061 7373 6572 7420 7265         assert re
-0000c170: 7175 6573 7420 3d3d 2028 6222 626c 6168  quest == (b"blah
-0000c180: 222c 2028 686f 7374 2c20 706f 7274 2929  ", (host, port))
-0000c190: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c1a0: 2020 6177 6169 7420 7564 7031 2e73 656e    await udp1.sen
-0000c1b0: 6474 6f28 6222 6861 6c62 222c 2068 6f73  dto(b"halb", hos
-0000c1c0: 742c 2070 6f72 7429 0a20 2020 2020 2020  t, port).       
-0000c1d0: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
-0000c1e0: 6520 3d20 6177 6169 7420 7564 7032 2e72  e = await udp2.r
-0000c1f0: 6563 6569 7665 2829 0a20 2020 2020 2020  eceive().       
-0000c200: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-0000c210: 7265 7370 6f6e 7365 203d 3d20 6222 6861  response == b"ha
-0000c220: 6c62 220a 0a20 2020 2061 7379 6e63 2064  lb"..    async d
-0000c230: 6566 2074 6573 745f 6974 6572 6174 6528  ef test_iterate(
-0000c240: 7365 6c66 2c20 6661 6d69 6c79 3a20 416e  self, family: An
-0000c250: 7949 5041 6464 7265 7373 4661 6d69 6c79  yIPAddressFamily
-0000c260: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-0000c270: 2020 2061 7379 6e63 2064 6566 2073 6572     async def ser
-0000c280: 7665 2829 202d 3e20 4e6f 6e65 3a0a 2020  ve() -> None:.  
-0000c290: 2020 2020 2020 2020 2020 6173 796e 6320            async 
-0000c2a0: 666f 7220 7061 636b 6574 2069 6e20 7564  for packet in ud
-0000c2b0: 7032 3a0a 2020 2020 2020 2020 2020 2020  p2:.            
-0000c2c0: 2020 2020 6177 6169 7420 7564 7032 2e73      await udp2.s
-0000c2d0: 656e 6428 7061 636b 6574 5b3a 3a2d 315d  end(packet[::-1]
-0000c2e0: 290a 0a20 2020 2020 2020 2061 7379 6e63  )..        async
-0000c2f0: 2077 6974 6820 6177 6169 7420 6372 6561   with await crea
-0000c300: 7465 5f75 6470 5f73 6f63 6b65 7428 0a20  te_udp_socket(. 
-0000c310: 2020 2020 2020 2020 2020 2066 616d 696c             famil
-0000c320: 793d 6661 6d69 6c79 2c20 6c6f 6361 6c5f  y=family, local_
-0000c330: 686f 7374 3d22 6c6f 6361 6c68 6f73 7422  host="localhost"
-0000c340: 0a20 2020 2020 2020 2029 2061 7320 7564  .        ) as ud
-0000c350: 7031 3a0a 2020 2020 2020 2020 2020 2020  p1:.            
-0000c360: 686f 7374 2c20 706f 7274 203d 2075 6470  host, port = udp
-0000c370: 312e 6578 7472 6128 536f 636b 6574 4174  1.extra(SocketAt
-0000c380: 7472 6962 7574 652e 6c6f 6361 6c5f 6164  tribute.local_ad
-0000c390: 6472 6573 7329 2020 2320 7479 7065 3a20  dress)  # type: 
-0000c3a0: 6967 6e6f 7265 5b6d 6973 635d 0a20 2020  ignore[misc].   
-0000c3b0: 2020 2020 2020 2020 2061 7379 6e63 2077           async w
-0000c3c0: 6974 6820 6177 6169 7420 6372 6561 7465  ith await create
-0000c3d0: 5f63 6f6e 6e65 6374 6564 5f75 6470 5f73  _connected_udp_s
-0000c3e0: 6f63 6b65 7428 686f 7374 2c20 706f 7274  ocket(host, port
-0000c3f0: 2920 6173 2075 6470 323a 0a20 2020 2020  ) as udp2:.     
-0000c400: 2020 2020 2020 2020 2020 2068 6f73 742c             host,
-0000c410: 2070 6f72 7420 3d20 7564 7032 2e65 7874   port = udp2.ext
-0000c420: 7261 2820 2023 2074 7970 653a 2069 676e  ra(  # type: ign
-0000c430: 6f72 655b 6d69 7363 5d0a 2020 2020 2020  ore[misc].      
-0000c440: 2020 2020 2020 2020 2020 2020 2020 536f                So
-0000c450: 636b 6574 4174 7472 6962 7574 652e 6c6f  cketAttribute.lo
-0000c460: 6361 6c5f 6164 6472 6573 730a 2020 2020  cal_address.    
-0000c470: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000c480: 2020 2020 2020 2020 2020 2020 2020 6173                as
-0000c490: 796e 6320 7769 7468 2063 7265 6174 655f  ync with create_
-0000c4a0: 7461 736b 5f67 726f 7570 2829 2061 7320  task_group() as 
-0000c4b0: 7467 3a0a 2020 2020 2020 2020 2020 2020  tg:.            
-0000c4c0: 2020 2020 2020 2020 7467 2e73 7461 7274          tg.start
-0000c4d0: 5f73 6f6f 6e28 7365 7276 6529 0a20 2020  _soon(serve).   
-0000c4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4f0: 2061 7761 6974 2075 6470 312e 7365 6e64   await udp1.send
-0000c500: 746f 2862 2246 4f4f 4241 5222 2c20 686f  to(b"FOOBAR", ho
-0000c510: 7374 2c20 706f 7274 290a 2020 2020 2020  st, port).      
-0000c520: 2020 2020 2020 2020 2020 2020 2020 6173                as
-0000c530: 7365 7274 2061 7761 6974 2075 6470 312e  sert await udp1.
-0000c540: 7265 6365 6976 6528 2920 3d3d 2028 6222  receive() == (b"
-0000c550: 5241 424f 4f46 222c 2028 686f 7374 2c20  RABOOF", (host, 
-0000c560: 706f 7274 2929 0a20 2020 2020 2020 2020  port)).         
-0000c570: 2020 2020 2020 2020 2020 2061 7761 6974             await
-0000c580: 2075 6470 312e 7365 6e64 746f 2862 2231   udp1.sendto(b"1
-0000c590: 3233 3435 3622 2c20 686f 7374 2c20 706f  23456", host, po
-0000c5a0: 7274 290a 2020 2020 2020 2020 2020 2020  rt).            
-0000c5b0: 2020 2020 2020 2020 6173 7365 7274 2061          assert a
-0000c5c0: 7761 6974 2075 6470 312e 7265 6365 6976  wait udp1.receiv
-0000c5d0: 6528 2920 3d3d 2028 6222 3635 3433 3231  e() == (b"654321
-0000c5e0: 222c 2028 686f 7374 2c20 706f 7274 2929  ", (host, port))
-0000c5f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c600: 2020 2020 2074 672e 6361 6e63 656c 5f73       tg.cancel_s
-0000c610: 636f 7065 2e63 616e 6365 6c28 290a 0a20  cope.cancel().. 
-0000c620: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
-0000c630: 736b 6970 6966 280a 2020 2020 2020 2020  skipif(.        
-0000c640: 6e6f 7420 6861 7361 7474 7228 736f 636b  not hasattr(sock
-0000c650: 6574 2c20 2253 4f5f 5245 5553 4550 4f52  et, "SO_REUSEPOR
-0000c660: 5422 292c 2072 6561 736f 6e3d 2253 4f5f  T"), reason="SO_
-0000c670: 5245 5553 4550 4f52 5420 6f70 7469 6f6e  REUSEPORT option
-0000c680: 206e 6f74 2073 7570 706f 7274 6564 220a   not supported".
-0000c690: 2020 2020 290a 2020 2020 6173 796e 6320      ).    async 
-0000c6a0: 6465 6620 7465 7374 5f72 6575 7365 5f70  def test_reuse_p
-0000c6b0: 6f72 7428 7365 6c66 2c20 6661 6d69 6c79  ort(self, family
-0000c6c0: 3a20 416e 7949 5041 6464 7265 7373 4661  : AnyIPAddressFa
-0000c6d0: 6d69 6c79 2920 2d3e 204e 6f6e 653a 0a20  mily) -> None:. 
-0000c6e0: 2020 2020 2020 2061 7379 6e63 2077 6974         async wit
-0000c6f0: 6820 6177 6169 7420 6372 6561 7465 5f63  h await create_c
-0000c700: 6f6e 6e65 6374 6564 5f75 6470 5f73 6f63  onnected_udp_soc
-0000c710: 6b65 7428 0a20 2020 2020 2020 2020 2020  ket(.           
-0000c720: 2022 6c6f 6361 6c68 6f73 7422 2c20 3630   "localhost", 60
-0000c730: 3030 2c20 6661 6d69 6c79 3d66 616d 696c  00, family=famil
-0000c740: 792c 206c 6f63 616c 5f68 6f73 743d 226c  y, local_host="l
-0000c750: 6f63 616c 686f 7374 222c 2072 6575 7365  ocalhost", reuse
-0000c760: 5f70 6f72 743d 5472 7565 0a20 2020 2020  _port=True.     
-0000c770: 2020 2029 2061 7320 7564 703a 0a20 2020     ) as udp:.   
-0000c780: 2020 2020 2020 2020 2070 6f72 7420 3d20           port = 
-0000c790: 7564 702e 6578 7472 6128 536f 636b 6574  udp.extra(Socket
-0000c7a0: 4174 7472 6962 7574 652e 6c6f 6361 6c5f  Attribute.local_
-0000c7b0: 706f 7274 290a 2020 2020 2020 2020 2020  port).          
-0000c7c0: 2020 6173 7365 7274 2070 6f72 7420 213d    assert port !=
-0000c7d0: 2030 0a20 2020 2020 2020 2020 2020 2061   0.            a
-0000c7e0: 7379 6e63 2077 6974 6820 6177 6169 7420  sync with await 
-0000c7f0: 6372 6561 7465 5f63 6f6e 6e65 6374 6564  create_connected
-0000c800: 5f75 6470 5f73 6f63 6b65 7428 0a20 2020  _udp_socket(.   
-0000c810: 2020 2020 2020 2020 2020 2020 2022 6c6f               "lo
-0000c820: 6361 6c68 6f73 7422 2c0a 2020 2020 2020  calhost",.      
-0000c830: 2020 2020 2020 2020 2020 3630 3031 2c0a            6001,.
-0000c840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c850: 6661 6d69 6c79 3d66 616d 696c 792c 0a20  family=family,. 
-0000c860: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000c870: 6f63 616c 5f68 6f73 743d 226c 6f63 616c  ocal_host="local
-0000c880: 686f 7374 222c 0a20 2020 2020 2020 2020  host",.         
-0000c890: 2020 2020 2020 206c 6f63 616c 5f70 6f72         local_por
-0000c8a0: 743d 706f 7274 2c0a 2020 2020 2020 2020  t=port,.        
-0000c8b0: 2020 2020 2020 2020 7265 7573 655f 706f          reuse_po
-0000c8c0: 7274 3d54 7275 652c 0a20 2020 2020 2020  rt=True,.       
-0000c8d0: 2020 2020 2029 2061 7320 7564 7032 3a0a       ) as udp2:.
-0000c8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c8f0: 6173 7365 7274 2070 6f72 7420 3d3d 2075  assert port == u
-0000c900: 6470 322e 6578 7472 6128 536f 636b 6574  dp2.extra(Socket
-0000c910: 4174 7472 6962 7574 652e 6c6f 6361 6c5f  Attribute.local_
-0000c920: 706f 7274 290a 0a20 2020 2061 7379 6e63  port)..    async
-0000c930: 2064 6566 2074 6573 745f 636f 6e63 7572   def test_concur
-0000c940: 7265 6e74 5f72 6563 6569 7665 2873 656c  rent_receive(sel
-0000c950: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-0000c960: 2020 2020 6173 796e 6320 7769 7468 2061      async with a
-0000c970: 7761 6974 2063 7265 6174 655f 636f 6e6e  wait create_conn
-0000c980: 6563 7465 645f 7564 705f 736f 636b 6574  ected_udp_socket
-0000c990: 280a 2020 2020 2020 2020 2020 2020 226c  (.            "l
-0000c9a0: 6f63 616c 686f 7374 222c 2035 3030 302c  ocalhost", 5000,
-0000c9b0: 206c 6f63 616c 5f68 6f73 743d 226c 6f63   local_host="loc
-0000c9c0: 616c 686f 7374 222c 2066 616d 696c 793d  alhost", family=
-0000c9d0: 4164 6472 6573 7346 616d 696c 792e 4146  AddressFamily.AF
-0000c9e0: 5f49 4e45 540a 2020 2020 2020 2020 2920  _INET.        ) 
-0000c9f0: 6173 2075 6470 3a0a 2020 2020 2020 2020  as udp:.        
-0000ca00: 2020 2020 6173 796e 6320 7769 7468 2063      async with c
-0000ca10: 7265 6174 655f 7461 736b 5f67 726f 7570  reate_task_group
-0000ca20: 2829 2061 7320 7467 3a0a 2020 2020 2020  () as tg:.      
-0000ca30: 2020 2020 2020 2020 2020 7467 2e73 7461            tg.sta
-0000ca40: 7274 5f73 6f6f 6e28 7564 702e 7265 6365  rt_soon(udp.rece
-0000ca50: 6976 6529 0a20 2020 2020 2020 2020 2020  ive).           
-0000ca60: 2020 2020 2061 7761 6974 2077 6169 745f       await wait_
-0000ca70: 616c 6c5f 7461 736b 735f 626c 6f63 6b65  all_tasks_blocke
-0000ca80: 6428 290a 2020 2020 2020 2020 2020 2020  d().            
-0000ca90: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-0000caa0: 2020 2020 2020 2020 2020 2020 2077 6974               wit
-0000cab0: 6820 7079 7465 7374 2e72 6169 7365 7328  h pytest.raises(
-0000cac0: 4275 7379 5265 736f 7572 6365 4572 726f  BusyResourceErro
-0000cad0: 7229 2061 7320 6578 633a 0a20 2020 2020  r) as exc:.     
-0000cae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000caf0: 2020 2061 7761 6974 2075 6470 2e72 6563     await udp.rec
-0000cb00: 6569 7665 2829 0a0a 2020 2020 2020 2020  eive()..        
-0000cb10: 2020 2020 2020 2020 2020 2020 6578 632e              exc.
-0000cb20: 6d61 7463 6828 2261 6c72 6561 6479 2072  match("already r
-0000cb30: 6561 6469 6e67 2066 726f 6d22 290a 2020  eading from").  
-0000cb40: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-0000cb50: 6e61 6c6c 793a 0a20 2020 2020 2020 2020  nally:.         
-0000cb60: 2020 2020 2020 2020 2020 2074 672e 6361             tg.ca
-0000cb70: 6e63 656c 5f73 636f 7065 2e63 616e 6365  ncel_scope.cance
-0000cb80: 6c28 290a 0a20 2020 2061 7379 6e63 2064  l()..    async d
-0000cb90: 6566 2074 6573 745f 636c 6f73 655f 6475  ef test_close_du
-0000cba0: 7269 6e67 5f72 6563 6569 7665 2873 656c  ring_receive(sel
-0000cbb0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-0000cbc0: 2020 2020 6173 796e 6320 6465 6620 636c      async def cl
-0000cbd0: 6f73 655f 7768 656e 5f62 6c6f 636b 6564  ose_when_blocked
-0000cbe0: 2829 202d 3e20 4e6f 6e65 3a0a 2020 2020  () -> None:.    
-0000cbf0: 2020 2020 2020 2020 6177 6169 7420 7761          await wa
-0000cc00: 6974 5f61 6c6c 5f74 6173 6b73 5f62 6c6f  it_all_tasks_blo
-0000cc10: 636b 6564 2829 0a20 2020 2020 2020 2020  cked().         
-0000cc20: 2020 2061 7761 6974 2075 6470 2e61 636c     await udp.acl
-0000cc30: 6f73 6528 290a 0a20 2020 2020 2020 2061  ose()..        a
-0000cc40: 7379 6e63 2077 6974 6820 6177 6169 7420  sync with await 
-0000cc50: 6372 6561 7465 5f63 6f6e 6e65 6374 6564  create_connected
-0000cc60: 5f75 6470 5f73 6f63 6b65 7428 0a20 2020  _udp_socket(.   
-0000cc70: 2020 2020 2020 2020 2022 6c6f 6361 6c68           "localh
-0000cc80: 6f73 7422 2c20 3530 3030 2c20 6c6f 6361  ost", 5000, loca
-0000cc90: 6c5f 686f 7374 3d22 6c6f 6361 6c68 6f73  l_host="localhos
-0000cca0: 7422 2c20 6661 6d69 6c79 3d41 6464 7265  t", family=Addre
-0000ccb0: 7373 4661 6d69 6c79 2e41 465f 494e 4554  ssFamily.AF_INET
-0000ccc0: 0a20 2020 2020 2020 2029 2061 7320 7564  .        ) as ud
-0000ccd0: 703a 0a20 2020 2020 2020 2020 2020 2061  p:.            a
-0000cce0: 7379 6e63 2077 6974 6820 6372 6561 7465  sync with create
-0000ccf0: 5f74 6173 6b5f 6772 6f75 7028 2920 6173  _task_group() as
-0000cd00: 2074 673a 0a20 2020 2020 2020 2020 2020   tg:.           
-0000cd10: 2020 2020 2074 672e 7374 6172 745f 736f       tg.start_so
-0000cd20: 6f6e 2863 6c6f 7365 5f77 6865 6e5f 626c  on(close_when_bl
-0000cd30: 6f63 6b65 6429 0a20 2020 2020 2020 2020  ocked).         
-0000cd40: 2020 2020 2020 2077 6974 6820 7079 7465         with pyte
-0000cd50: 7374 2e72 6169 7365 7328 436c 6f73 6564  st.raises(Closed
-0000cd60: 5265 736f 7572 6365 4572 726f 7229 3a0a  ResourceError):.
-0000cd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd80: 2020 2020 6177 6169 7420 7564 702e 7265      await udp.re
-0000cd90: 6365 6976 6528 290a 0a20 2020 2061 7379  ceive()..    asy
-0000cda0: 6e63 2064 6566 2074 6573 745f 7265 6365  nc def test_rece
-0000cdb0: 6976 655f 6166 7465 725f 636c 6f73 6528  ive_after_close(
-0000cdc0: 7365 6c66 2c20 6661 6d69 6c79 3a20 416e  self, family: An
-0000cdd0: 7949 5041 6464 7265 7373 4661 6d69 6c79  yIPAddressFamily
-0000cde0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-0000cdf0: 2020 2075 6470 203d 2061 7761 6974 2063     udp = await c
-0000ce00: 7265 6174 655f 636f 6e6e 6563 7465 645f  reate_connected_
-0000ce10: 7564 705f 736f 636b 6574 280a 2020 2020  udp_socket(.    
-0000ce20: 2020 2020 2020 2020 226c 6f63 616c 686f          "localho
-0000ce30: 7374 222c 2035 3030 302c 206c 6f63 616c  st", 5000, local
-0000ce40: 5f68 6f73 743d 226c 6f63 616c 686f 7374  _host="localhost
-0000ce50: 222c 2066 616d 696c 793d 6661 6d69 6c79  ", family=family
-0000ce60: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0000ce70: 2020 2061 7761 6974 2075 6470 2e61 636c     await udp.acl
-0000ce80: 6f73 6528 290a 2020 2020 2020 2020 7769  ose().        wi
-0000ce90: 7468 2070 7974 6573 742e 7261 6973 6573  th pytest.raises
-0000cea0: 2843 6c6f 7365 6452 6573 6f75 7263 6545  (ClosedResourceE
-0000ceb0: 7272 6f72 293a 0a20 2020 2020 2020 2020  rror):.         
-0000cec0: 2020 2061 7761 6974 2075 6470 2e72 6563     await udp.rec
-0000ced0: 6569 7665 2829 0a0a 2020 2020 6173 796e  eive()..    asyn
-0000cee0: 6320 6465 6620 7465 7374 5f73 656e 645f  c def test_send_
-0000cef0: 6166 7465 725f 636c 6f73 6528 7365 6c66  after_close(self
-0000cf00: 2c20 6661 6d69 6c79 3a20 416e 7949 5041  , family: AnyIPA
-0000cf10: 6464 7265 7373 4661 6d69 6c79 2920 2d3e  ddressFamily) ->
-0000cf20: 204e 6f6e 653a 0a20 2020 2020 2020 2075   None:.        u
-0000cf30: 6470 203d 2061 7761 6974 2063 7265 6174  dp = await creat
-0000cf40: 655f 636f 6e6e 6563 7465 645f 7564 705f  e_connected_udp_
-0000cf50: 736f 636b 6574 280a 2020 2020 2020 2020  socket(.        
-0000cf60: 2020 2020 226c 6f63 616c 686f 7374 222c      "localhost",
-0000cf70: 2035 3030 302c 206c 6f63 616c 5f68 6f73   5000, local_hos
-0000cf80: 743d 226c 6f63 616c 686f 7374 222c 2066  t="localhost", f
-0000cf90: 616d 696c 793d 6661 6d69 6c79 0a20 2020  amily=family.   
-0000cfa0: 2020 2020 2029 0a20 2020 2020 2020 2061       ).        a
-0000cfb0: 7761 6974 2075 6470 2e61 636c 6f73 6528  wait udp.aclose(
-0000cfc0: 290a 2020 2020 2020 2020 7769 7468 2070  ).        with p
-0000cfd0: 7974 6573 742e 7261 6973 6573 2843 6c6f  ytest.raises(Clo
-0000cfe0: 7365 6452 6573 6f75 7263 6545 7272 6f72  sedResourceError
-0000cff0: 293a 0a20 2020 2020 2020 2020 2020 2061  ):.            a
-0000d000: 7761 6974 2075 6470 2e73 656e 6428 6222  wait udp.send(b"
-0000d010: 666f 6f22 290a 0a0a 4070 7974 6573 742e  foo")...@pytest.
-0000d020: 6d61 726b 2e73 6b69 7069 6628 0a20 2020  mark.skipif(.   
-0000d030: 2073 7973 2e70 6c61 7466 6f72 6d20 3d3d   sys.platform ==
-0000d040: 2022 7769 6e33 3222 2c20 7265 6173 6f6e   "win32", reason
-0000d050: 3d22 554e 4958 2073 6f63 6b65 7473 2061  ="UNIX sockets a
-0000d060: 7265 206e 6f74 2061 7661 696c 6162 6c65  re not available
-0000d070: 206f 6e20 5769 6e64 6f77 7322 0a29 0a63   on Windows".).c
-0000d080: 6c61 7373 2054 6573 7455 4e49 5844 6174  lass TestUNIXDat
-0000d090: 6167 7261 6d53 6f63 6b65 743a 0a20 2020  agramSocket:.   
-0000d0a0: 2040 7079 7465 7374 2e66 6978 7475 7265   @pytest.fixture
-0000d0b0: 0a20 2020 2064 6566 2073 6f63 6b65 745f  .    def socket_
-0000d0c0: 7061 7468 2873 656c 6629 202d 3e20 4765  path(self) -> Ge
-0000d0d0: 6e65 7261 746f 725b 5061 7468 2c20 4e6f  nerator[Path, No
-0000d0e0: 6e65 2c20 4e6f 6e65 5d3a 0a20 2020 2020  ne, None]:.     
-0000d0f0: 2020 2023 2055 7365 2073 7464 6c69 6220     # Use stdlib 
-0000d100: 7465 6d70 6469 7220 6765 6e65 7261 7469  tempdir generati
-0000d110: 6f6e 0a20 2020 2020 2020 2023 2046 6978  on.        # Fix
-0000d120: 6573 2060 4f53 4572 726f 723a 2041 465f  es `OSError: AF_
-0000d130: 554e 4958 2070 6174 6820 746f 6f20 6c6f  UNIX path too lo
-0000d140: 6e67 6020 6672 6f6d 2070 7974 6573 7420  ng` from pytest 
-0000d150: 6765 6e65 7261 7465 6420 7465 6d70 5f70  generated temp_p
-0000d160: 6174 680a 2020 2020 2020 2020 7769 7468  ath.        with
-0000d170: 2074 656d 7066 696c 652e 5465 6d70 6f72   tempfile.Tempor
-0000d180: 6172 7944 6972 6563 746f 7279 2829 2061  aryDirectory() a
-0000d190: 7320 7061 7468 3a0a 2020 2020 2020 2020  s path:.        
-0000d1a0: 2020 2020 7969 656c 6420 5061 7468 2870      yield Path(p
-0000d1b0: 6174 6829 202f 2022 736f 636b 6574 220a  ath) / "socket".
-0000d1c0: 0a20 2020 2040 7079 7465 7374 2e66 6978  .    @pytest.fix
-0000d1d0: 7475 7265 2870 6172 616d 733d 5b46 616c  ture(params=[Fal
-0000d1e0: 7365 2c20 5472 7565 5d2c 2069 6473 3d5b  se, True], ids=[
-0000d1f0: 2273 7472 222c 2022 7061 7468 225d 290a  "str", "path"]).
-0000d200: 2020 2020 6465 6620 736f 636b 6574 5f70      def socket_p
-0000d210: 6174 685f 6f72 5f73 7472 2873 656c 662c  ath_or_str(self,
-0000d220: 2072 6571 7565 7374 3a20 5375 6252 6571   request: SubReq
-0000d230: 7565 7374 2c20 736f 636b 6574 5f70 6174  uest, socket_pat
-0000d240: 683a 2050 6174 6829 202d 3e20 5061 7468  h: Path) -> Path
-0000d250: 207c 2073 7472 3a0a 2020 2020 2020 2020   | str:.        
-0000d260: 7265 7475 726e 2073 6f63 6b65 745f 7061  return socket_pa
-0000d270: 7468 2069 6620 7265 7175 6573 742e 7061  th if request.pa
-0000d280: 7261 6d20 656c 7365 2073 7472 2873 6f63  ram else str(soc
-0000d290: 6b65 745f 7061 7468 290a 0a20 2020 2040  ket_path)..    @
-0000d2a0: 7079 7465 7374 2e66 6978 7475 7265 0a20  pytest.fixture. 
-0000d2b0: 2020 2064 6566 2070 6565 725f 736f 636b     def peer_sock
-0000d2c0: 6574 5f70 6174 6828 7365 6c66 2920 2d3e  et_path(self) ->
-0000d2d0: 2047 656e 6572 6174 6f72 5b50 6174 682c   Generator[Path,
-0000d2e0: 204e 6f6e 652c 204e 6f6e 655d 3a0a 2020   None, None]:.  
-0000d2f0: 2020 2020 2020 2320 5573 6520 7374 646c        # Use stdl
-0000d300: 6962 2074 656d 7064 6972 2067 656e 6572  ib tempdir gener
-0000d310: 6174 696f 6e0a 2020 2020 2020 2020 2320  ation.        # 
-0000d320: 4669 7865 7320 604f 5345 7272 6f72 3a20  Fixes `OSError: 
-0000d330: 4146 5f55 4e49 5820 7061 7468 2074 6f6f  AF_UNIX path too
-0000d340: 206c 6f6e 6760 2066 726f 6d20 7079 7465   long` from pyte
-0000d350: 7374 2067 656e 6572 6174 6564 2074 656d  st generated tem
-0000d360: 705f 7061 7468 0a20 2020 2020 2020 2077  p_path.        w
-0000d370: 6974 6820 7465 6d70 6669 6c65 2e54 656d  ith tempfile.Tem
-0000d380: 706f 7261 7279 4469 7265 6374 6f72 7928  poraryDirectory(
-0000d390: 2920 6173 2070 6174 683a 0a20 2020 2020  ) as path:.     
-0000d3a0: 2020 2020 2020 2079 6965 6c64 2050 6174         yield Pat
-0000d3b0: 6828 7061 7468 2920 2f20 2270 6565 725f  h(path) / "peer_
-0000d3c0: 736f 636b 6574 220a 0a20 2020 2061 7379  socket"..    asy
-0000d3d0: 6e63 2064 6566 2074 6573 745f 6578 7472  nc def test_extr
-0000d3e0: 615f 6174 7472 6962 7574 6573 2873 656c  a_attributes(sel
-0000d3f0: 662c 2073 6f63 6b65 745f 7061 7468 3a20  f, socket_path: 
-0000d400: 5061 7468 2920 2d3e 204e 6f6e 653a 0a20  Path) -> None:. 
-0000d410: 2020 2020 2020 2061 7379 6e63 2077 6974         async wit
-0000d420: 6820 6177 6169 7420 6372 6561 7465 5f75  h await create_u
-0000d430: 6e69 785f 6461 7461 6772 616d 5f73 6f63  nix_datagram_soc
-0000d440: 6b65 7428 6c6f 6361 6c5f 7061 7468 3d73  ket(local_path=s
-0000d450: 6f63 6b65 745f 7061 7468 2920 6173 2075  ocket_path) as u
-0000d460: 6e69 785f 6467 3a0a 2020 2020 2020 2020  nix_dg:.        
-0000d470: 2020 2020 7261 775f 736f 636b 6574 203d      raw_socket =
-0000d480: 2075 6e69 785f 6467 2e65 7874 7261 2853   unix_dg.extra(S
-0000d490: 6f63 6b65 7441 7474 7269 6275 7465 2e72  ocketAttribute.r
-0000d4a0: 6177 5f73 6f63 6b65 7429 0a20 2020 2020  aw_socket).     
-0000d4b0: 2020 2020 2020 2061 7373 6572 7420 7261         assert ra
-0000d4c0: 775f 736f 636b 6574 2e67 6574 7469 6d65  w_socket.gettime
-0000d4d0: 6f75 7428 2920 3d3d 2030 0a20 2020 2020  out() == 0.     
-0000d4e0: 2020 2020 2020 2061 7373 6572 7420 756e         assert un
-0000d4f0: 6978 5f64 672e 6578 7472 6128 536f 636b  ix_dg.extra(Sock
-0000d500: 6574 4174 7472 6962 7574 652e 6661 6d69  etAttribute.fami
-0000d510: 6c79 2920 3d3d 2073 6f63 6b65 742e 4146  ly) == socket.AF
-0000d520: 5f55 4e49 580a 2020 2020 2020 2020 2020  _UNIX.          
-0000d530: 2020 6173 7365 7274 2028 0a20 2020 2020    assert (.     
-0000d540: 2020 2020 2020 2020 2020 2075 6e69 785f             unix_
-0000d550: 6467 2e65 7874 7261 2853 6f63 6b65 7441  dg.extra(SocketA
-0000d560: 7474 7269 6275 7465 2e6c 6f63 616c 5f61  ttribute.local_a
-0000d570: 6464 7265 7373 2920 3d3d 2072 6177 5f73  ddress) == raw_s
-0000d580: 6f63 6b65 742e 6765 7473 6f63 6b6e 616d  ocket.getsocknam
-0000d590: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-0000d5a0: 290a 2020 2020 2020 2020 2020 2020 7079  ).            py
-0000d5b0: 7465 7374 2e72 6169 7365 7328 0a20 2020  test.raises(.   
-0000d5c0: 2020 2020 2020 2020 2020 2020 2054 7970               Typ
-0000d5d0: 6564 4174 7472 6962 7574 654c 6f6f 6b75  edAttributeLooku
-0000d5e0: 7045 7272 6f72 2c20 756e 6978 5f64 672e  pError, unix_dg.
-0000d5f0: 6578 7472 612c 2053 6f63 6b65 7441 7474  extra, SocketAtt
-0000d600: 7269 6275 7465 2e6c 6f63 616c 5f70 6f72  ribute.local_por
-0000d610: 740a 2020 2020 2020 2020 2020 2020 290a  t.            ).
-0000d620: 2020 2020 2020 2020 2020 2020 7079 7465              pyte
-0000d630: 7374 2e72 6169 7365 7328 0a20 2020 2020  st.raises(.     
-0000d640: 2020 2020 2020 2020 2020 2054 7970 6564             Typed
-0000d650: 4174 7472 6962 7574 654c 6f6f 6b75 7045  AttributeLookupE
-0000d660: 7272 6f72 2c20 756e 6978 5f64 672e 6578  rror, unix_dg.ex
-0000d670: 7472 612c 2053 6f63 6b65 7441 7474 7269  tra, SocketAttri
-0000d680: 6275 7465 2e72 656d 6f74 655f 6164 6472  bute.remote_addr
-0000d690: 6573 730a 2020 2020 2020 2020 2020 2020  ess.            
-0000d6a0: 290a 2020 2020 2020 2020 2020 2020 7079  ).            py
-0000d6b0: 7465 7374 2e72 6169 7365 7328 0a20 2020  test.raises(.   
-0000d6c0: 2020 2020 2020 2020 2020 2020 2054 7970               Typ
-0000d6d0: 6564 4174 7472 6962 7574 654c 6f6f 6b75  edAttributeLooku
-0000d6e0: 7045 7272 6f72 2c20 756e 6978 5f64 672e  pError, unix_dg.
-0000d6f0: 6578 7472 612c 2053 6f63 6b65 7441 7474  extra, SocketAtt
-0000d700: 7269 6275 7465 2e72 656d 6f74 655f 706f  ribute.remote_po
-0000d710: 7274 0a20 2020 2020 2020 2020 2020 2029  rt.            )
-0000d720: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-0000d730: 7465 7374 5f73 656e 645f 7265 6365 6976  test_send_receiv
-0000d740: 6528 7365 6c66 2c20 736f 636b 6574 5f70  e(self, socket_p
-0000d750: 6174 685f 6f72 5f73 7472 3a20 5061 7468  ath_or_str: Path
-0000d760: 207c 2073 7472 2920 2d3e 204e 6f6e 653a   | str) -> None:
-0000d770: 0a20 2020 2020 2020 2061 7379 6e63 2077  .        async w
-0000d780: 6974 6820 6177 6169 7420 6372 6561 7465  ith await create
-0000d790: 5f75 6e69 785f 6461 7461 6772 616d 5f73  _unix_datagram_s
-0000d7a0: 6f63 6b65 7428 0a20 2020 2020 2020 2020  ocket(.         
-0000d7b0: 2020 206c 6f63 616c 5f70 6174 683d 736f     local_path=so
-0000d7c0: 636b 6574 5f70 6174 685f 6f72 5f73 7472  cket_path_or_str
-0000d7d0: 2c0a 2020 2020 2020 2020 2920 6173 2073  ,.        ) as s
-0000d7e0: 6f63 6b3a 0a20 2020 2020 2020 2020 2020  ock:.           
-0000d7f0: 2070 6174 6820 3d20 7374 7228 736f 636b   path = str(sock
-0000d800: 6574 5f70 6174 685f 6f72 5f73 7472 290a  et_path_or_str).
-0000d810: 0a20 2020 2020 2020 2020 2020 2061 7761  .            awa
-0000d820: 6974 2073 6f63 6b2e 7365 6e64 746f 2862  it sock.sendto(b
-0000d830: 2262 6c61 6822 2c20 7061 7468 290a 2020  "blah", path).  
-0000d840: 2020 2020 2020 2020 2020 7265 7175 6573            reques
-0000d850: 742c 2061 6464 7220 3d20 6177 6169 7420  t, addr = await 
-0000d860: 736f 636b 2e72 6563 6569 7665 2829 0a20  sock.receive(). 
-0000d870: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-0000d880: 7420 7265 7175 6573 7420 3d3d 2062 2262  t request == b"b
-0000d890: 6c61 6822 0a20 2020 2020 2020 2020 2020  lah".           
-0000d8a0: 2061 7373 6572 7420 6164 6472 203d 3d20   assert addr == 
-0000d8b0: 7061 7468 0a0a 2020 2020 2020 2020 2020  path..          
-0000d8c0: 2020 6177 6169 7420 736f 636b 2e73 656e    await sock.sen
-0000d8d0: 6474 6f28 6222 6861 6c62 222c 2070 6174  dto(b"halb", pat
-0000d8e0: 6829 0a20 2020 2020 2020 2020 2020 2072  h).            r
-0000d8f0: 6573 706f 6e73 652c 2061 6464 7220 3d20  esponse, addr = 
-0000d900: 6177 6169 7420 736f 636b 2e72 6563 6569  await sock.recei
-0000d910: 7665 2829 0a20 2020 2020 2020 2020 2020  ve().           
-0000d920: 2061 7373 6572 7420 7265 7370 6f6e 7365   assert response
-0000d930: 203d 3d20 6222 6861 6c62 220a 2020 2020   == b"halb".    
-0000d940: 2020 2020 2020 2020 6173 7365 7274 2061          assert a
-0000d950: 6464 7220 3d3d 2070 6174 680a 0a20 2020  ddr == path..   
-0000d960: 2061 7379 6e63 2064 6566 2074 6573 745f   async def test_
-0000d970: 6974 6572 6174 6528 7365 6c66 2c20 7065  iterate(self, pe
-0000d980: 6572 5f73 6f63 6b65 745f 7061 7468 3a20  er_socket_path: 
-0000d990: 5061 7468 2c20 736f 636b 6574 5f70 6174  Path, socket_pat
-0000d9a0: 683a 2050 6174 6829 202d 3e20 4e6f 6e65  h: Path) -> None
-0000d9b0: 3a0a 2020 2020 2020 2020 6173 796e 6320  :.        async 
-0000d9c0: 6465 6620 7365 7276 6528 2920 2d3e 204e  def serve() -> N
-0000d9d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000d9e0: 2061 7379 6e63 2066 6f72 2070 6163 6b65   async for packe
-0000d9f0: 742c 2061 6464 7220 696e 2073 6572 7665  t, addr in serve
-0000da00: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-0000da10: 2020 2061 7761 6974 2073 6572 7665 722e     await server.
-0000da20: 7365 6e64 2828 7061 636b 6574 5b3a 3a2d  send((packet[::-
-0000da30: 315d 2c20 6164 6472 2929 0a0a 2020 2020  1], addr))..    
-0000da40: 2020 2020 6173 796e 6320 7769 7468 2061      async with a
-0000da50: 7761 6974 2063 7265 6174 655f 756e 6978  wait create_unix
-0000da60: 5f64 6174 6167 7261 6d5f 736f 636b 6574  _datagram_socket
-0000da70: 280a 2020 2020 2020 2020 2020 2020 6c6f  (.            lo
-0000da80: 6361 6c5f 7061 7468 3d70 6565 725f 736f  cal_path=peer_so
-0000da90: 636b 6574 5f70 6174 682c 0a20 2020 2020  cket_path,.     
-0000daa0: 2020 2029 2061 7320 7365 7276 6572 3a0a     ) as server:.
-0000dab0: 2020 2020 2020 2020 2020 2020 7065 6572              peer
-0000dac0: 5f70 6174 6820 3d20 7374 7228 7065 6572  _path = str(peer
-0000dad0: 5f73 6f63 6b65 745f 7061 7468 290a 2020  _socket_path).  
-0000dae0: 2020 2020 2020 2020 2020 6173 796e 6320            async 
-0000daf0: 7769 7468 2061 7761 6974 2063 7265 6174  with await creat
-0000db00: 655f 756e 6978 5f64 6174 6167 7261 6d5f  e_unix_datagram_
-0000db10: 736f 636b 6574 280a 2020 2020 2020 2020  socket(.        
-0000db20: 2020 2020 2020 2020 6c6f 6361 6c5f 7061          local_pa
-0000db30: 7468 3d73 6f63 6b65 745f 7061 7468 0a20  th=socket_path. 
-0000db40: 2020 2020 2020 2020 2020 2029 2061 7320             ) as 
-0000db50: 636c 6965 6e74 3a0a 2020 2020 2020 2020  client:.        
-0000db60: 2020 2020 2020 2020 6173 796e 6320 7769          async wi
-0000db70: 7468 2063 7265 6174 655f 7461 736b 5f67  th create_task_g
-0000db80: 726f 7570 2829 2061 7320 7467 3a0a 2020  roup() as tg:.  
-0000db90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dba0: 2020 7467 2e73 7461 7274 5f73 6f6f 6e28    tg.start_soon(
-0000dbb0: 7365 7276 6529 0a20 2020 2020 2020 2020  serve).         
-0000dbc0: 2020 2020 2020 2020 2020 2061 7761 6974             await
-0000dbd0: 2063 6c69 656e 742e 7365 6e64 746f 2862   client.sendto(b
-0000dbe0: 2246 4f4f 4241 5222 2c20 7065 6572 5f70  "FOOBAR", peer_p
-0000dbf0: 6174 6829 0a20 2020 2020 2020 2020 2020  ath).           
-0000dc00: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-0000dc10: 6177 6169 7420 636c 6965 6e74 2e72 6563  await client.rec
-0000dc20: 6569 7665 2829 203d 3d20 2862 2252 4142  eive() == (b"RAB
-0000dc30: 4f4f 4622 2c20 7065 6572 5f70 6174 6829  OOF", peer_path)
-0000dc40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dc50: 2020 2020 2061 7761 6974 2063 6c69 656e       await clien
-0000dc60: 742e 7365 6e64 746f 2862 2231 3233 3435  t.sendto(b"12345
-0000dc70: 3622 2c20 7065 6572 5f70 6174 6829 0a20  6", peer_path). 
-0000dc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc90: 2020 2061 7373 6572 7420 6177 6169 7420     assert await 
-0000dca0: 636c 6965 6e74 2e72 6563 6569 7665 2829  client.receive()
-0000dcb0: 203d 3d20 2862 2236 3534 3332 3122 2c20   == (b"654321", 
-0000dcc0: 7065 6572 5f70 6174 6829 0a20 2020 2020  peer_path).     
-0000dcd0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000dce0: 672e 6361 6e63 656c 5f73 636f 7065 2e63  g.cancel_scope.c
-0000dcf0: 616e 6365 6c28 290a 0a20 2020 2061 7379  ancel()..    asy
-0000dd00: 6e63 2064 6566 2074 6573 745f 636f 6e63  nc def test_conc
-0000dd10: 7572 7265 6e74 5f72 6563 6569 7665 2873  urrent_receive(s
-0000dd20: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-0000dd30: 2020 2020 2020 6173 796e 6320 7769 7468        async with
-0000dd40: 2061 7761 6974 2063 7265 6174 655f 756e   await create_un
-0000dd50: 6978 5f64 6174 6167 7261 6d5f 736f 636b  ix_datagram_sock
-0000dd60: 6574 2829 2061 7320 756e 6978 5f64 673a  et() as unix_dg:
-0000dd70: 0a20 2020 2020 2020 2020 2020 2061 7379  .            asy
-0000dd80: 6e63 2077 6974 6820 6372 6561 7465 5f74  nc with create_t
-0000dd90: 6173 6b5f 6772 6f75 7028 2920 6173 2074  ask_group() as t
-0000dda0: 673a 0a20 2020 2020 2020 2020 2020 2020  g:.             
-0000ddb0: 2020 2074 672e 7374 6172 745f 736f 6f6e     tg.start_soon
-0000ddc0: 2875 6e69 785f 6467 2e72 6563 6569 7665  (unix_dg.receive
-0000ddd0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000dde0: 2020 6177 6169 7420 7761 6974 5f61 6c6c    await wait_all
-0000ddf0: 5f74 6173 6b73 5f62 6c6f 636b 6564 2829  _tasks_blocked()
-0000de00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000de10: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-0000de20: 2020 2020 2020 2020 2020 7769 7468 2070            with p
-0000de30: 7974 6573 742e 7261 6973 6573 2842 7573  ytest.raises(Bus
-0000de40: 7952 6573 6f75 7263 6545 7272 6f72 2920  yResourceError) 
-0000de50: 6173 2065 7863 3a0a 2020 2020 2020 2020  as exc:.        
-0000de60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de70: 6177 6169 7420 756e 6978 5f64 672e 7265  await unix_dg.re
-0000de80: 6365 6976 6528 290a 0a20 2020 2020 2020  ceive()..       
-0000de90: 2020 2020 2020 2020 2020 2020 2065 7863               exc
-0000dea0: 2e6d 6174 6368 2822 616c 7265 6164 7920  .match("already 
-0000deb0: 7265 6164 696e 6720 6672 6f6d 2229 0a20  reading from"). 
-0000dec0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000ded0: 696e 616c 6c79 3a0a 2020 2020 2020 2020  inally:.        
-0000dee0: 2020 2020 2020 2020 2020 2020 7467 2e63              tg.c
-0000def0: 616e 6365 6c5f 7363 6f70 652e 6361 6e63  ancel_scope.canc
-0000df00: 656c 2829 0a0a 2020 2020 6173 796e 6320  el()..    async 
-0000df10: 6465 6620 7465 7374 5f63 6c6f 7365 5f64  def test_close_d
-0000df20: 7572 696e 675f 7265 6365 6976 6528 7365  uring_receive(se
-0000df30: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-0000df40: 2020 2020 2061 7379 6e63 2064 6566 2063       async def c
-0000df50: 6c6f 7365 5f77 6865 6e5f 626c 6f63 6b65  lose_when_blocke
-0000df60: 6428 2920 2d3e 204e 6f6e 653a 0a20 2020  d() -> None:.   
-0000df70: 2020 2020 2020 2020 2061 7761 6974 2077           await w
-0000df80: 6169 745f 616c 6c5f 7461 736b 735f 626c  ait_all_tasks_bl
-0000df90: 6f63 6b65 6428 290a 2020 2020 2020 2020  ocked().        
-0000dfa0: 2020 2020 6177 6169 7420 756e 6978 5f64      await unix_d
-0000dfb0: 672e 6163 6c6f 7365 2829 0a0a 2020 2020  g.aclose()..    
-0000dfc0: 2020 2020 6173 796e 6320 7769 7468 2061      async with a
-0000dfd0: 7761 6974 2063 7265 6174 655f 756e 6978  wait create_unix
-0000dfe0: 5f64 6174 6167 7261 6d5f 736f 636b 6574  _datagram_socket
-0000dff0: 2829 2061 7320 756e 6978 5f64 673a 0a20  () as unix_dg:. 
-0000e000: 2020 2020 2020 2020 2020 2061 7379 6e63             async
-0000e010: 2077 6974 6820 6372 6561 7465 5f74 6173   with create_tas
-0000e020: 6b5f 6772 6f75 7028 2920 6173 2074 673a  k_group() as tg:
-0000e030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e040: 2074 672e 7374 6172 745f 736f 6f6e 2863   tg.start_soon(c
-0000e050: 6c6f 7365 5f77 6865 6e5f 626c 6f63 6b65  lose_when_blocke
-0000e060: 6429 0a20 2020 2020 2020 2020 2020 2020  d).             
-0000e070: 2020 2077 6974 6820 7079 7465 7374 2e72     with pytest.r
-0000e080: 6169 7365 7328 436c 6f73 6564 5265 736f  aises(ClosedReso
-0000e090: 7572 6365 4572 726f 7229 3a0a 2020 2020  urceError):.    
-0000e0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0b0: 6177 6169 7420 756e 6978 5f64 672e 7265  await unix_dg.re
-0000e0c0: 6365 6976 6528 290a 0a20 2020 2061 7379  ceive()..    asy
-0000e0d0: 6e63 2064 6566 2074 6573 745f 7265 6365  nc def test_rece
-0000e0e0: 6976 655f 6166 7465 725f 636c 6f73 6528  ive_after_close(
-0000e0f0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-0000e100: 2020 2020 2020 2075 6e69 785f 6467 203d         unix_dg =
-0000e110: 2061 7761 6974 2063 7265 6174 655f 756e   await create_un
-0000e120: 6978 5f64 6174 6167 7261 6d5f 736f 636b  ix_datagram_sock
-0000e130: 6574 2829 0a20 2020 2020 2020 2061 7761  et().        awa
-0000e140: 6974 2075 6e69 785f 6467 2e61 636c 6f73  it unix_dg.aclos
-0000e150: 6528 290a 2020 2020 2020 2020 7769 7468  e().        with
-0000e160: 2070 7974 6573 742e 7261 6973 6573 2843   pytest.raises(C
-0000e170: 6c6f 7365 6452 6573 6f75 7263 6545 7272  losedResourceErr
-0000e180: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
-0000e190: 2061 7761 6974 2075 6e69 785f 6467 2e72   await unix_dg.r
-0000e1a0: 6563 6569 7665 2829 0a0a 2020 2020 6173  eceive()..    as
-0000e1b0: 796e 6320 6465 6620 7465 7374 5f73 656e  ync def test_sen
-0000e1c0: 645f 6166 7465 725f 636c 6f73 6528 7365  d_after_close(se
-0000e1d0: 6c66 2c20 736f 636b 6574 5f70 6174 683a  lf, socket_path:
-0000e1e0: 2050 6174 6829 202d 3e20 4e6f 6e65 3a0a   Path) -> None:.
-0000e1f0: 2020 2020 2020 2020 756e 6978 5f64 6720          unix_dg 
-0000e200: 3d20 6177 6169 7420 6372 6561 7465 5f75  = await create_u
-0000e210: 6e69 785f 6461 7461 6772 616d 5f73 6f63  nix_datagram_soc
-0000e220: 6b65 7428 6c6f 6361 6c5f 7061 7468 3d73  ket(local_path=s
-0000e230: 6f63 6b65 745f 7061 7468 290a 2020 2020  ocket_path).    
-0000e240: 2020 2020 7061 7468 203d 2073 7472 2873      path = str(s
-0000e250: 6f63 6b65 745f 7061 7468 290a 2020 2020  ocket_path).    
-0000e260: 2020 2020 6177 6169 7420 756e 6978 5f64      await unix_d
-0000e270: 672e 6163 6c6f 7365 2829 0a20 2020 2020  g.aclose().     
-0000e280: 2020 2077 6974 6820 7079 7465 7374 2e72     with pytest.r
-0000e290: 6169 7365 7328 436c 6f73 6564 5265 736f  aises(ClosedReso
-0000e2a0: 7572 6365 4572 726f 7229 3a0a 2020 2020  urceError):.    
-0000e2b0: 2020 2020 2020 2020 6177 6169 7420 756e          await un
-0000e2c0: 6978 5f64 672e 7365 6e64 746f 2862 2266  ix_dg.sendto(b"f
-0000e2d0: 6f6f 222c 2070 6174 6829 0a0a 2020 2020  oo", path)..    
-0000e2e0: 6173 796e 6320 6465 6620 7465 7374 5f6c  async def test_l
-0000e2f0: 6f63 616c 5f70 6174 685f 6279 7465 7328  ocal_path_bytes(
-0000e300: 7365 6c66 2c20 736f 636b 6574 5f70 6174  self, socket_pat
-0000e310: 683a 2050 6174 6829 202d 3e20 4e6f 6e65  h: Path) -> None
-0000e320: 3a0a 2020 2020 2020 2020 6173 796e 6320  :.        async 
-0000e330: 7769 7468 2061 7761 6974 2063 7265 6174  with await creat
-0000e340: 655f 756e 6978 5f64 6174 6167 7261 6d5f  e_unix_datagram_
-0000e350: 736f 636b 6574 280a 2020 2020 2020 2020  socket(.        
-0000e360: 2020 2020 6c6f 6361 6c5f 7061 7468 3d73      local_path=s
-0000e370: 7472 2873 6f63 6b65 745f 7061 7468 292e  tr(socket_path).
-0000e380: 656e 636f 6465 2829 0a20 2020 2020 2020  encode().       
-0000e390: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-0000e3a0: 7061 7373 0a0a 2020 2020 4070 7974 6573  pass..    @pytes
-0000e3b0: 742e 6d61 726b 2e73 6b69 7069 6628 0a20  t.mark.skipif(. 
-0000e3c0: 2020 2020 2020 2070 6c61 7466 6f72 6d2e         platform.
-0000e3d0: 7379 7374 656d 2829 203d 3d20 2244 6172  system() == "Dar
-0000e3e0: 7769 6e22 2c20 7265 6173 6f6e 3d22 6d61  win", reason="ma
-0000e3f0: 634f 5320 7265 7175 6972 6573 2076 616c  cOS requires val
-0000e400: 6964 2055 5446 2d38 2070 6174 6873 220a  id UTF-8 paths".
-0000e410: 2020 2020 290a 2020 2020 6173 796e 6320      ).    async 
-0000e420: 6465 6620 7465 7374 5f6c 6f63 616c 5f70  def test_local_p
-0000e430: 6174 685f 696e 7661 6c69 645f 6173 6369  ath_invalid_asci
-0000e440: 6928 7365 6c66 2c20 736f 636b 6574 5f70  i(self, socket_p
-0000e450: 6174 683a 2050 6174 6829 202d 3e20 4e6f  ath: Path) -> No
-0000e460: 6e65 3a0a 2020 2020 2020 2020 7265 616c  ne:.        real
-0000e470: 5f70 6174 6820 3d20 7374 7228 736f 636b  _path = str(sock
-0000e480: 6574 5f70 6174 6829 2e65 6e63 6f64 6528  et_path).encode(
-0000e490: 2920 2b20 6222 5c78 4630 220a 2020 2020  ) + b"\xF0".    
-0000e4a0: 2020 2020 6173 796e 6320 7769 7468 2061      async with a
-0000e4b0: 7761 6974 2063 7265 6174 655f 756e 6978  wait create_unix
-0000e4c0: 5f64 6174 6167 7261 6d5f 736f 636b 6574  _datagram_socket
-0000e4d0: 286c 6f63 616c 5f70 6174 683d 7265 616c  (local_path=real
-0000e4e0: 5f70 6174 6829 3a0a 2020 2020 2020 2020  _path):.        
-0000e4f0: 2020 2020 7061 7373 0a0a 0a40 7079 7465      pass...@pyte
-0000e500: 7374 2e6d 6172 6b2e 736b 6970 6966 280a  st.mark.skipif(.
-0000e510: 2020 2020 7379 732e 706c 6174 666f 726d      sys.platform
-0000e520: 203d 3d20 2277 696e 3332 222c 2072 6561   == "win32", rea
-0000e530: 736f 6e3d 2255 4e49 5820 736f 636b 6574  son="UNIX socket
-0000e540: 7320 6172 6520 6e6f 7420 6176 6169 6c61  s are not availa
-0000e550: 626c 6520 6f6e 2057 696e 646f 7773 220a  ble on Windows".
-0000e560: 290a 636c 6173 7320 5465 7374 436f 6e6e  ).class TestConn
-0000e570: 6563 7465 6455 4e49 5844 6174 6167 7261  ectedUNIXDatagra
-0000e580: 6d53 6f63 6b65 743a 0a20 2020 2040 7079  mSocket:.    @py
-0000e590: 7465 7374 2e66 6978 7475 7265 0a20 2020  test.fixture.   
-0000e5a0: 2064 6566 2073 6f63 6b65 745f 7061 7468   def socket_path
-0000e5b0: 2873 656c 6629 202d 3e20 4765 6e65 7261  (self) -> Genera
-0000e5c0: 746f 725b 5061 7468 2c20 4e6f 6e65 2c20  tor[Path, None, 
-0000e5d0: 4e6f 6e65 5d3a 0a20 2020 2020 2020 2023  None]:.        #
-0000e5e0: 2055 7365 2073 7464 6c69 6220 7465 6d70   Use stdlib temp
-0000e5f0: 6469 7220 6765 6e65 7261 7469 6f6e 0a20  dir generation. 
-0000e600: 2020 2020 2020 2023 2046 6978 6573 2060         # Fixes `
-0000e610: 4f53 4572 726f 723a 2041 465f 554e 4958  OSError: AF_UNIX
-0000e620: 2070 6174 6820 746f 6f20 6c6f 6e67 6020   path too long` 
-0000e630: 6672 6f6d 2070 7974 6573 7420 6765 6e65  from pytest gene
-0000e640: 7261 7465 6420 7465 6d70 5f70 6174 680a  rated temp_path.
-0000e650: 2020 2020 2020 2020 7769 7468 2074 656d          with tem
-0000e660: 7066 696c 652e 5465 6d70 6f72 6172 7944  pfile.TemporaryD
-0000e670: 6972 6563 746f 7279 2829 2061 7320 7061  irectory() as pa
-0000e680: 7468 3a0a 2020 2020 2020 2020 2020 2020  th:.            
-0000e690: 7969 656c 6420 5061 7468 2870 6174 6829  yield Path(path)
-0000e6a0: 202f 2022 736f 636b 6574 220a 0a20 2020   / "socket"..   
-0000e6b0: 2040 7079 7465 7374 2e66 6978 7475 7265   @pytest.fixture
-0000e6c0: 2870 6172 616d 733d 5b46 616c 7365 2c20  (params=[False, 
-0000e6d0: 5472 7565 5d2c 2069 6473 3d5b 2273 7472  True], ids=["str
-0000e6e0: 222c 2022 7061 7468 225d 290a 2020 2020  ", "path"]).    
-0000e6f0: 6465 6620 736f 636b 6574 5f70 6174 685f  def socket_path_
-0000e700: 6f72 5f73 7472 2873 656c 662c 2072 6571  or_str(self, req
-0000e710: 7565 7374 3a20 5375 6252 6571 7565 7374  uest: SubRequest
-0000e720: 2c20 736f 636b 6574 5f70 6174 683a 2050  , socket_path: P
-0000e730: 6174 6829 202d 3e20 5061 7468 207c 2073  ath) -> Path | s
-0000e740: 7472 3a0a 2020 2020 2020 2020 7265 7475  tr:.        retu
-0000e750: 726e 2073 6f63 6b65 745f 7061 7468 2069  rn socket_path i
-0000e760: 6620 7265 7175 6573 742e 7061 7261 6d20  f request.param 
-0000e770: 656c 7365 2073 7472 2873 6f63 6b65 745f  else str(socket_
-0000e780: 7061 7468 290a 0a20 2020 2040 7079 7465  path)..    @pyte
-0000e790: 7374 2e66 6978 7475 7265 0a20 2020 2064  st.fixture.    d
-0000e7a0: 6566 2070 6565 725f 736f 636b 6574 5f70  ef peer_socket_p
-0000e7b0: 6174 6828 7365 6c66 2920 2d3e 2047 656e  ath(self) -> Gen
-0000e7c0: 6572 6174 6f72 5b50 6174 682c 204e 6f6e  erator[Path, Non
-0000e7d0: 652c 204e 6f6e 655d 3a0a 2020 2020 2020  e, None]:.      
-0000e7e0: 2020 2320 5573 6520 7374 646c 6962 2074    # Use stdlib t
-0000e7f0: 656d 7064 6972 2067 656e 6572 6174 696f  empdir generatio
-0000e800: 6e0a 2020 2020 2020 2020 2320 4669 7865  n.        # Fixe
-0000e810: 7320 604f 5345 7272 6f72 3a20 4146 5f55  s `OSError: AF_U
-0000e820: 4e49 5820 7061 7468 2074 6f6f 206c 6f6e  NIX path too lon
-0000e830: 6760 2066 726f 6d20 7079 7465 7374 2067  g` from pytest g
-0000e840: 656e 6572 6174 6564 2074 656d 705f 7061  enerated temp_pa
-0000e850: 7468 0a20 2020 2020 2020 2077 6974 6820  th.        with 
-0000e860: 7465 6d70 6669 6c65 2e54 656d 706f 7261  tempfile.Tempora
-0000e870: 7279 4469 7265 6374 6f72 7928 2920 6173  ryDirectory() as
-0000e880: 2070 6174 683a 0a20 2020 2020 2020 2020   path:.         
-0000e890: 2020 2079 6965 6c64 2050 6174 6828 7061     yield Path(pa
-0000e8a0: 7468 2920 2f20 2270 6565 725f 736f 636b  th) / "peer_sock
-0000e8b0: 6574 220a 0a20 2020 2040 7079 7465 7374  et"..    @pytest
-0000e8c0: 2e66 6978 7475 7265 2870 6172 616d 733d  .fixture(params=
-0000e8d0: 5b46 616c 7365 2c20 5472 7565 5d2c 2069  [False, True], i
-0000e8e0: 6473 3d5b 2270 6565 725f 7374 7222 2c20  ds=["peer_str", 
-0000e8f0: 2270 6565 725f 7061 7468 225d 290a 2020  "peer_path"]).  
-0000e900: 2020 6465 6620 7065 6572 5f73 6f63 6b65    def peer_socke
-0000e910: 745f 7061 7468 5f6f 725f 7374 7228 0a20  t_path_or_str(. 
-0000e920: 2020 2020 2020 2073 656c 662c 2072 6571         self, req
-0000e930: 7565 7374 3a20 5375 6252 6571 7565 7374  uest: SubRequest
-0000e940: 2c20 7065 6572 5f73 6f63 6b65 745f 7061  , peer_socket_pa
-0000e950: 7468 3a20 5061 7468 0a20 2020 2029 202d  th: Path.    ) -
-0000e960: 3e20 5061 7468 207c 2073 7472 3a0a 2020  > Path | str:.  
-0000e970: 2020 2020 2020 7265 7475 726e 2070 6565        return pee
-0000e980: 725f 736f 636b 6574 5f70 6174 6820 6966  r_socket_path if
-0000e990: 2072 6571 7565 7374 2e70 6172 616d 2065   request.param e
-0000e9a0: 6c73 6520 7374 7228 7065 6572 5f73 6f63  lse str(peer_soc
-0000e9b0: 6b65 745f 7061 7468 290a 0a20 2020 2040  ket_path)..    @
-0000e9c0: 7079 7465 7374 2e66 6978 7475 7265 0a20  pytest.fixture. 
-0000e9d0: 2020 2064 6566 2070 6565 725f 736f 636b     def peer_sock
-0000e9e0: 2873 656c 662c 2070 6565 725f 736f 636b  (self, peer_sock
-0000e9f0: 6574 5f70 6174 683a 2050 6174 6829 202d  et_path: Path) -
-0000ea00: 3e20 4974 6572 6162 6c65 5b73 6f63 6b65  > Iterable[socke
-0000ea10: 742e 736f 636b 6574 5d3a 0a20 2020 2020  t.socket]:.     
-0000ea20: 2020 2073 6f63 6b20 3d20 736f 636b 6574     sock = socket
-0000ea30: 2e73 6f63 6b65 7428 736f 636b 6574 2e41  .socket(socket.A
-0000ea40: 465f 554e 4958 2c20 736f 636b 6574 2e53  F_UNIX, socket.S
-0000ea50: 4f43 4b5f 4447 5241 4d29 0a20 2020 2020  OCK_DGRAM).     
-0000ea60: 2020 2073 6f63 6b2e 7365 7474 696d 656f     sock.settimeo
-0000ea70: 7574 2831 290a 2020 2020 2020 2020 736f  ut(1).        so
-0000ea80: 636b 2e62 696e 6428 7374 7228 7065 6572  ck.bind(str(peer
-0000ea90: 5f73 6f63 6b65 745f 7061 7468 2929 0a20  _socket_path)). 
-0000eaa0: 2020 2020 2020 2079 6965 6c64 2073 6f63         yield soc
-0000eab0: 6b0a 2020 2020 2020 2020 736f 636b 2e63  k.        sock.c
-0000eac0: 6c6f 7365 2829 0a0a 2020 2020 6173 796e  lose()..    asyn
-0000ead0: 6320 6465 6620 7465 7374 5f65 7874 7261  c def test_extra
-0000eae0: 5f61 7474 7269 6275 7465 7328 0a20 2020  _attributes(.   
-0000eaf0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000eb00: 2020 2073 6f63 6b65 745f 7061 7468 3a20     socket_path: 
-0000eb10: 5061 7468 2c0a 2020 2020 2020 2020 7065  Path,.        pe
-0000eb20: 6572 5f73 6f63 6b65 745f 7061 7468 3a20  er_socket_path: 
-0000eb30: 5061 7468 2c0a 2020 2020 2020 2020 7065  Path,.        pe
-0000eb40: 6572 5f73 6f63 6b3a 2073 6f63 6b65 742e  er_sock: socket.
-0000eb50: 736f 636b 6574 2c0a 2020 2020 2920 2d3e  socket,.    ) ->
-0000eb60: 204e 6f6e 653a 0a20 2020 2020 2020 2061   None:.        a
-0000eb70: 7379 6e63 2077 6974 6820 6177 6169 7420  sync with await 
-0000eb80: 6372 6561 7465 5f63 6f6e 6e65 6374 6564  create_connected
-0000eb90: 5f75 6e69 785f 6461 7461 6772 616d 5f73  _unix_datagram_s
-0000eba0: 6f63 6b65 7428 0a20 2020 2020 2020 2020  ocket(.         
-0000ebb0: 2020 2072 656d 6f74 655f 7061 7468 3d70     remote_path=p
-0000ebc0: 6565 725f 736f 636b 6574 5f70 6174 682c  eer_socket_path,
-0000ebd0: 0a20 2020 2020 2020 2020 2020 206c 6f63  .            loc
-0000ebe0: 616c 5f70 6174 683d 736f 636b 6574 5f70  al_path=socket_p
-0000ebf0: 6174 682c 0a20 2020 2020 2020 2029 2061  ath,.        ) a
-0000ec00: 7320 756e 6978 5f64 673a 0a20 2020 2020  s unix_dg:.     
-0000ec10: 2020 2020 2020 2072 6177 5f73 6f63 6b65         raw_socke
-0000ec20: 7420 3d20 756e 6978 5f64 672e 6578 7472  t = unix_dg.extr
-0000ec30: 6128 536f 636b 6574 4174 7472 6962 7574  a(SocketAttribut
-0000ec40: 652e 7261 775f 736f 636b 6574 290a 2020  e.raw_socket).  
-0000ec50: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-0000ec60: 2072 6177 5f73 6f63 6b65 7420 6973 206e   raw_socket is n
-0000ec70: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
-0000ec80: 2020 2020 6173 7365 7274 2075 6e69 785f      assert unix_
-0000ec90: 6467 2e65 7874 7261 2853 6f63 6b65 7441  dg.extra(SocketA
-0000eca0: 7474 7269 6275 7465 2e66 616d 696c 7929  ttribute.family)
-0000ecb0: 203d 3d20 4164 6472 6573 7346 616d 696c   == AddressFamil
-0000ecc0: 792e 4146 5f55 4e49 580a 2020 2020 2020  y.AF_UNIX.      
-0000ecd0: 2020 2020 2020 6173 7365 7274 2075 6e69        assert uni
-0000ece0: 785f 6467 2e65 7874 7261 2853 6f63 6b65  x_dg.extra(Socke
-0000ecf0: 7441 7474 7269 6275 7465 2e6c 6f63 616c  tAttribute.local
-0000ed00: 5f61 6464 7265 7373 2920 3d3d 2073 7472  _address) == str
-0000ed10: 2873 6f63 6b65 745f 7061 7468 290a 2020  (socket_path).  
-0000ed20: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-0000ed30: 2075 6e69 785f 6467 2e65 7874 7261 2853   unix_dg.extra(S
-0000ed40: 6f63 6b65 7441 7474 7269 6275 7465 2e72  ocketAttribute.r
-0000ed50: 656d 6f74 655f 6164 6472 6573 7329 203d  emote_address) =
-0000ed60: 3d20 7374 7228 0a20 2020 2020 2020 2020  = str(.         
-0000ed70: 2020 2020 2020 2070 6565 725f 736f 636b         peer_sock
-0000ed80: 6574 5f70 6174 680a 2020 2020 2020 2020  et_path.        
-0000ed90: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000eda0: 2020 7079 7465 7374 2e72 6169 7365 7328    pytest.raises(
-0000edb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000edc0: 2054 7970 6564 4174 7472 6962 7574 654c   TypedAttributeL
-0000edd0: 6f6f 6b75 7045 7272 6f72 2c20 756e 6978  ookupError, unix
-0000ede0: 5f64 672e 6578 7472 612c 2053 6f63 6b65  _dg.extra, Socke
-0000edf0: 7441 7474 7269 6275 7465 2e6c 6f63 616c  tAttribute.local
-0000ee00: 5f70 6f72 740a 2020 2020 2020 2020 2020  _port.          
-0000ee10: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0000ee20: 7079 7465 7374 2e72 6169 7365 7328 0a20  pytest.raises(. 
-0000ee30: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-0000ee40: 7970 6564 4174 7472 6962 7574 654c 6f6f  ypedAttributeLoo
-0000ee50: 6b75 7045 7272 6f72 2c20 756e 6978 5f64  kupError, unix_d
-0000ee60: 672e 6578 7472 612c 2053 6f63 6b65 7441  g.extra, SocketA
-0000ee70: 7474 7269 6275 7465 2e72 656d 6f74 655f  ttribute.remote_
-0000ee80: 706f 7274 0a20 2020 2020 2020 2020 2020  port.           
-0000ee90: 2029 0a0a 2020 2020 6173 796e 6320 6465   )..    async de
-0000eea0: 6620 7465 7374 5f73 656e 645f 7265 6365  f test_send_rece
-0000eeb0: 6976 6528 0a20 2020 2020 2020 2073 656c  ive(.        sel
-0000eec0: 662c 0a20 2020 2020 2020 2073 6f63 6b65  f,.        socke
-0000eed0: 745f 7061 7468 5f6f 725f 7374 723a 2050  t_path_or_str: P
-0000eee0: 6174 6820 7c20 7374 722c 0a20 2020 2020  ath | str,.     
-0000eef0: 2020 2070 6565 725f 736f 636b 6574 5f70     peer_socket_p
-0000ef00: 6174 685f 6f72 5f73 7472 3a20 5061 7468  ath_or_str: Path
-0000ef10: 207c 2073 7472 2c0a 2020 2020 2920 2d3e   | str,.    ) ->
-0000ef20: 204e 6f6e 653a 0a20 2020 2020 2020 2061   None:.        a
-0000ef30: 7379 6e63 2077 6974 6820 6177 6169 7420  sync with await 
-0000ef40: 6372 6561 7465 5f75 6e69 785f 6461 7461  create_unix_data
-0000ef50: 6772 616d 5f73 6f63 6b65 7428 0a20 2020  gram_socket(.   
-0000ef60: 2020 2020 2020 2020 206c 6f63 616c 5f70           local_p
-0000ef70: 6174 683d 7065 6572 5f73 6f63 6b65 745f  ath=peer_socket_
-0000ef80: 7061 7468 5f6f 725f 7374 722c 0a20 2020  path_or_str,.   
+00008ad0: 7468 2920 6173 2073 7472 6561 6d3a 0a20  th) as stream:. 
+00008ae0: 2020 2020 2020 2020 2020 2061 7379 6e63             async
+00008af0: 2077 6974 6820 6372 6561 7465 5f74 6173   with create_tas
+00008b00: 6b5f 6772 6f75 7028 2920 6173 2074 673a  k_group() as tg:
+00008b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008b20: 2074 672e 7374 6172 745f 736f 6f6e 2869   tg.start_soon(i
+00008b30: 6e74 6572 7275 7074 290a 2020 2020 2020  nterrupt).      
+00008b40: 2020 2020 2020 2020 2020 7769 7468 2070            with p
+00008b50: 7974 6573 742e 7261 6973 6573 2843 6c6f  ytest.raises(Clo
+00008b60: 7365 6452 6573 6f75 7263 6545 7272 6f72  sedResourceError
+00008b70: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00008b80: 2020 2020 2020 2061 7761 6974 2073 7472         await str
+00008b90: 6561 6d2e 7265 6365 6976 6528 290a 0a20  eam.receive().. 
+00008ba0: 2020 2061 7379 6e63 2064 6566 2074 6573     async def tes
+00008bb0: 745f 7265 6365 6976 655f 6166 7465 725f  t_receive_after_
+00008bc0: 636c 6f73 6528 0a20 2020 2020 2020 2073  close(.        s
+00008bd0: 656c 662c 2073 6572 7665 725f 736f 636b  elf, server_sock
+00008be0: 3a20 736f 636b 6574 2e73 6f63 6b65 742c  : socket.socket,
+00008bf0: 2073 6f63 6b65 745f 7061 7468 3a20 5061   socket_path: Pa
+00008c00: 7468 0a20 2020 2029 202d 3e20 4e6f 6e65  th.    ) -> None
+00008c10: 3a0a 2020 2020 2020 2020 7374 7265 616d  :.        stream
+00008c20: 203d 2061 7761 6974 2063 6f6e 6e65 6374   = await connect
+00008c30: 5f75 6e69 7828 736f 636b 6574 5f70 6174  _unix(socket_pat
+00008c40: 6829 0a20 2020 2020 2020 2061 7761 6974  h).        await
+00008c50: 2073 7472 6561 6d2e 6163 6c6f 7365 2829   stream.aclose()
+00008c60: 0a20 2020 2020 2020 2077 6974 6820 7079  .        with py
+00008c70: 7465 7374 2e72 6169 7365 7328 436c 6f73  test.raises(Clos
+00008c80: 6564 5265 736f 7572 6365 4572 726f 7229  edResourceError)
+00008c90: 3a0a 2020 2020 2020 2020 2020 2020 6177  :.            aw
+00008ca0: 6169 7420 7374 7265 616d 2e72 6563 6569  ait stream.recei
+00008cb0: 7665 2829 0a0a 2020 2020 6173 796e 6320  ve()..    async 
+00008cc0: 6465 6620 7465 7374 5f73 656e 645f 6166  def test_send_af
+00008cd0: 7465 725f 636c 6f73 6528 0a20 2020 2020  ter_close(.     
+00008ce0: 2020 2073 656c 662c 2073 6572 7665 725f     self, server_
+00008cf0: 736f 636b 3a20 736f 636b 6574 2e73 6f63  sock: socket.soc
+00008d00: 6b65 742c 2073 6f63 6b65 745f 7061 7468  ket, socket_path
+00008d10: 3a20 5061 7468 0a20 2020 2029 202d 3e20  : Path.    ) -> 
+00008d20: 4e6f 6e65 3a0a 2020 2020 2020 2020 7374  None:.        st
+00008d30: 7265 616d 203d 2061 7761 6974 2063 6f6e  ream = await con
+00008d40: 6e65 6374 5f75 6e69 7828 736f 636b 6574  nect_unix(socket
+00008d50: 5f70 6174 6829 0a20 2020 2020 2020 2061  _path).        a
+00008d60: 7761 6974 2073 7472 6561 6d2e 6163 6c6f  wait stream.aclo
+00008d70: 7365 2829 0a20 2020 2020 2020 2077 6974  se().        wit
+00008d80: 6820 7079 7465 7374 2e72 6169 7365 7328  h pytest.raises(
+00008d90: 436c 6f73 6564 5265 736f 7572 6365 4572  ClosedResourceEr
+00008da0: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
+00008db0: 2020 6177 6169 7420 7374 7265 616d 2e73    await stream.s
+00008dc0: 656e 6428 6222 666f 6f22 290a 0a20 2020  end(b"foo")..   
+00008dd0: 2061 7379 6e63 2064 6566 2074 6573 745f   async def test_
+00008de0: 6361 6e6e 6f74 5f63 6f6e 6e65 6374 2873  cannot_connect(s
+00008df0: 656c 662c 2073 6f63 6b65 745f 7061 7468  elf, socket_path
+00008e00: 3a20 5061 7468 2920 2d3e 204e 6f6e 653a  : Path) -> None:
+00008e10: 0a20 2020 2020 2020 2077 6974 6820 7079  .        with py
+00008e20: 7465 7374 2e72 6169 7365 7328 4669 6c65  test.raises(File
+00008e30: 4e6f 7446 6f75 6e64 4572 726f 7229 3a0a  NotFoundError):.
+00008e40: 2020 2020 2020 2020 2020 2020 6177 6169              awai
+00008e50: 7420 636f 6e6e 6563 745f 756e 6978 2873  t connect_unix(s
+00008e60: 6f63 6b65 745f 7061 7468 290a 0a20 2020  ocket_path)..   
+00008e70: 2061 7379 6e63 2064 6566 2074 6573 745f   async def test_
+00008e80: 636f 6e6e 6563 7469 6e67 5f75 7369 6e67  connecting_using
+00008e90: 5f62 7974 6573 280a 2020 2020 2020 2020  _bytes(.        
+00008ea0: 7365 6c66 2c20 7365 7276 6572 5f73 6f63  self, server_soc
+00008eb0: 6b3a 2073 6f63 6b65 742e 736f 636b 6574  k: socket.socket
+00008ec0: 2c20 736f 636b 6574 5f70 6174 683a 2050  , socket_path: P
+00008ed0: 6174 680a 2020 2020 2920 2d3e 204e 6f6e  ath.    ) -> Non
+00008ee0: 653a 0a20 2020 2020 2020 2061 7379 6e63  e:.        async
+00008ef0: 2077 6974 6820 6177 6169 7420 636f 6e6e   with await conn
+00008f00: 6563 745f 756e 6978 2873 7472 2873 6f63  ect_unix(str(soc
+00008f10: 6b65 745f 7061 7468 292e 656e 636f 6465  ket_path).encode
+00008f20: 2829 293a 0a20 2020 2020 2020 2020 2020  ()):.           
+00008f30: 2070 6173 730a 0a20 2020 2040 7079 7465   pass..    @pyte
+00008f40: 7374 2e6d 6172 6b2e 736b 6970 6966 280a  st.mark.skipif(.
+00008f50: 2020 2020 2020 2020 706c 6174 666f 726d          platform
+00008f60: 2e73 7973 7465 6d28 2920 3d3d 2022 4461  .system() == "Da
+00008f70: 7277 696e 222c 2072 6561 736f 6e3d 226d  rwin", reason="m
+00008f80: 6163 4f53 2072 6571 7569 7265 7320 7661  acOS requires va
+00008f90: 6c69 6420 5554 462d 3820 7061 7468 7322  lid UTF-8 paths"
+00008fa0: 0a20 2020 2029 0a20 2020 2061 7379 6e63  .    ).    async
+00008fb0: 2064 6566 2074 6573 745f 636f 6e6e 6563   def test_connec
+00008fc0: 7469 6e67 5f77 6974 685f 6e6f 6e5f 7574  ting_with_non_ut
+00008fd0: 6638 2873 656c 662c 2073 6f63 6b65 745f  f8(self, socket_
+00008fe0: 7061 7468 3a20 5061 7468 2920 2d3e 204e  path: Path) -> N
+00008ff0: 6f6e 653a 0a20 2020 2020 2020 2061 6374  one:.        act
+00009000: 7561 6c5f 7061 7468 203d 2073 7472 2873  ual_path = str(s
+00009010: 6f63 6b65 745f 7061 7468 292e 656e 636f  ocket_path).enco
+00009020: 6465 2829 202b 2062 225c 7866 3022 0a20  de() + b"\xf0". 
+00009030: 2020 2020 2020 2073 6572 7665 7220 3d20         server = 
+00009040: 736f 636b 6574 2e73 6f63 6b65 7428 736f  socket.socket(so
+00009050: 636b 6574 2e41 465f 554e 4958 290a 2020  cket.AF_UNIX).  
+00009060: 2020 2020 2020 7365 7276 6572 2e62 696e        server.bin
+00009070: 6428 6163 7475 616c 5f70 6174 6829 0a20  d(actual_path). 
+00009080: 2020 2020 2020 2073 6572 7665 722e 6c69         server.li
+00009090: 7374 656e 2831 290a 0a20 2020 2020 2020  sten(1)..       
+000090a0: 2061 7379 6e63 2077 6974 6820 6177 6169   async with awai
+000090b0: 7420 636f 6e6e 6563 745f 756e 6978 2861  t connect_unix(a
+000090c0: 6374 7561 6c5f 7061 7468 293a 0a20 2020  ctual_path):.   
+000090d0: 2020 2020 2020 2020 2070 6173 730a 0a0a           pass...
+000090e0: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
+000090f0: 7069 6628 0a20 2020 2073 7973 2e70 6c61  pif(.    sys.pla
+00009100: 7466 6f72 6d20 3d3d 2022 7769 6e33 3222  tform == "win32"
+00009110: 2c20 7265 6173 6f6e 3d22 554e 4958 2073  , reason="UNIX s
+00009120: 6f63 6b65 7473 2061 7265 206e 6f74 2061  ockets are not a
+00009130: 7661 696c 6162 6c65 206f 6e20 5769 6e64  vailable on Wind
+00009140: 6f77 7322 0a29 0a63 6c61 7373 2054 6573  ows".).class Tes
+00009150: 7455 4e49 584c 6973 7465 6e65 723a 0a20  tUNIXListener:. 
+00009160: 2020 2040 7079 7465 7374 2e66 6978 7475     @pytest.fixtu
+00009170: 7265 0a20 2020 2064 6566 2073 6f63 6b65  re.    def socke
+00009180: 745f 7061 7468 2873 656c 6629 202d 3e20  t_path(self) -> 
+00009190: 4765 6e65 7261 746f 725b 5061 7468 2c20  Generator[Path, 
+000091a0: 4e6f 6e65 2c20 4e6f 6e65 5d3a 0a20 2020  None, None]:.   
+000091b0: 2020 2020 2023 2055 7365 2073 7464 6c69       # Use stdli
+000091c0: 6220 7465 6d70 6469 7220 6765 6e65 7261  b tempdir genera
+000091d0: 7469 6f6e 0a20 2020 2020 2020 2023 2046  tion.        # F
+000091e0: 6978 6573 2060 4f53 4572 726f 723a 2041  ixes `OSError: A
+000091f0: 465f 554e 4958 2070 6174 6820 746f 6f20  F_UNIX path too 
+00009200: 6c6f 6e67 6020 6672 6f6d 2070 7974 6573  long` from pytes
+00009210: 7420 6765 6e65 7261 7465 6420 7465 6d70  t generated temp
+00009220: 5f70 6174 680a 2020 2020 2020 2020 7769  _path.        wi
+00009230: 7468 2074 656d 7066 696c 652e 5465 6d70  th tempfile.Temp
+00009240: 6f72 6172 7944 6972 6563 746f 7279 2829  oraryDirectory()
+00009250: 2061 7320 7061 7468 3a0a 2020 2020 2020   as path:.      
+00009260: 2020 2020 2020 7969 656c 6420 5061 7468        yield Path
+00009270: 2870 6174 6829 202f 2022 736f 636b 6574  (path) / "socket
+00009280: 220a 0a20 2020 2040 7079 7465 7374 2e66  "..    @pytest.f
+00009290: 6978 7475 7265 2870 6172 616d 733d 5b46  ixture(params=[F
+000092a0: 616c 7365 2c20 5472 7565 5d2c 2069 6473  alse, True], ids
+000092b0: 3d5b 2273 7472 222c 2022 7061 7468 225d  =["str", "path"]
+000092c0: 290a 2020 2020 6465 6620 736f 636b 6574  ).    def socket
+000092d0: 5f70 6174 685f 6f72 5f73 7472 2873 656c  _path_or_str(sel
+000092e0: 662c 2072 6571 7565 7374 3a20 5375 6252  f, request: SubR
+000092f0: 6571 7565 7374 2c20 736f 636b 6574 5f70  equest, socket_p
+00009300: 6174 683a 2050 6174 6829 202d 3e20 5061  ath: Path) -> Pa
+00009310: 7468 207c 2073 7472 3a0a 2020 2020 2020  th | str:.      
+00009320: 2020 7265 7475 726e 2073 6f63 6b65 745f    return socket_
+00009330: 7061 7468 2069 6620 7265 7175 6573 742e  path if request.
+00009340: 7061 7261 6d20 656c 7365 2073 7472 2873  param else str(s
+00009350: 6f63 6b65 745f 7061 7468 290a 0a20 2020  ocket_path)..   
+00009360: 2061 7379 6e63 2064 6566 2074 6573 745f   async def test_
+00009370: 6578 7472 615f 6174 7472 6962 7574 6573  extra_attributes
+00009380: 2873 656c 662c 2073 6f63 6b65 745f 7061  (self, socket_pa
+00009390: 7468 3a20 5061 7468 2920 2d3e 204e 6f6e  th: Path) -> Non
+000093a0: 653a 0a20 2020 2020 2020 2061 7379 6e63  e:.        async
+000093b0: 2077 6974 6820 6177 6169 7420 6372 6561   with await crea
+000093c0: 7465 5f75 6e69 785f 6c69 7374 656e 6572  te_unix_listener
+000093d0: 2873 6f63 6b65 745f 7061 7468 2920 6173  (socket_path) as
+000093e0: 206c 6973 7465 6e65 723a 0a20 2020 2020   listener:.     
+000093f0: 2020 2020 2020 2072 6177 5f73 6f63 6b65         raw_socke
+00009400: 7420 3d20 6c69 7374 656e 6572 2e65 7874  t = listener.ext
+00009410: 7261 2853 6f63 6b65 7441 7474 7269 6275  ra(SocketAttribu
+00009420: 7465 2e72 6177 5f73 6f63 6b65 7429 0a20  te.raw_socket). 
+00009430: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+00009440: 7420 6c69 7374 656e 6572 2e65 7874 7261  t listener.extra
+00009450: 2853 6f63 6b65 7441 7474 7269 6275 7465  (SocketAttribute
+00009460: 2e66 616d 696c 7929 203d 3d20 736f 636b  .family) == sock
+00009470: 6574 2e41 465f 554e 4958 0a20 2020 2020  et.AF_UNIX.     
+00009480: 2020 2020 2020 2061 7373 6572 7420 280a         assert (.
+00009490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094a0: 6c69 7374 656e 6572 2e65 7874 7261 2853  listener.extra(S
+000094b0: 6f63 6b65 7441 7474 7269 6275 7465 2e6c  ocketAttribute.l
+000094c0: 6f63 616c 5f61 6464 7265 7373 290a 2020  ocal_address).  
+000094d0: 2020 2020 2020 2020 2020 2020 2020 3d3d                ==
+000094e0: 2072 6177 5f73 6f63 6b65 742e 6765 7473   raw_socket.gets
+000094f0: 6f63 6b6e 616d 6528 290a 2020 2020 2020  ockname().      
+00009500: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00009510: 2020 2020 7079 7465 7374 2e72 6169 7365      pytest.raise
+00009520: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
+00009530: 2020 2054 7970 6564 4174 7472 6962 7574     TypedAttribut
+00009540: 654c 6f6f 6b75 7045 7272 6f72 2c20 6c69  eLookupError, li
+00009550: 7374 656e 6572 2e65 7874 7261 2c20 536f  stener.extra, So
+00009560: 636b 6574 4174 7472 6962 7574 652e 6c6f  cketAttribute.lo
+00009570: 6361 6c5f 706f 7274 0a20 2020 2020 2020  cal_port.       
+00009580: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00009590: 2020 2070 7974 6573 742e 7261 6973 6573     pytest.raises
+000095a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000095b0: 2020 5479 7065 6441 7474 7269 6275 7465    TypedAttribute
+000095c0: 4c6f 6f6b 7570 4572 726f 722c 0a20 2020  LookupError,.   
+000095d0: 2020 2020 2020 2020 2020 2020 206c 6973               lis
+000095e0: 7465 6e65 722e 6578 7472 612c 0a20 2020  tener.extra,.   
+000095f0: 2020 2020 2020 2020 2020 2020 2053 6f63               Soc
+00009600: 6b65 7441 7474 7269 6275 7465 2e72 656d  ketAttribute.rem
+00009610: 6f74 655f 6164 6472 6573 732c 0a20 2020  ote_address,.   
+00009620: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00009630: 2020 2020 2020 2070 7974 6573 742e 7261         pytest.ra
+00009640: 6973 6573 280a 2020 2020 2020 2020 2020  ises(.          
+00009650: 2020 2020 2020 5479 7065 6441 7474 7269        TypedAttri
+00009660: 6275 7465 4c6f 6f6b 7570 4572 726f 722c  buteLookupError,
+00009670: 206c 6973 7465 6e65 722e 6578 7472 612c   listener.extra,
+00009680: 2053 6f63 6b65 7441 7474 7269 6275 7465   SocketAttribute
+00009690: 2e72 656d 6f74 655f 706f 7274 0a20 2020  .remote_port.   
+000096a0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+000096b0: 6173 796e 6320 6465 6620 7465 7374 5f61  async def test_a
+000096c0: 6363 6570 7428 7365 6c66 2c20 736f 636b  ccept(self, sock
+000096d0: 6574 5f70 6174 685f 6f72 5f73 7472 3a20  et_path_or_str: 
+000096e0: 5061 7468 207c 2073 7472 2920 2d3e 204e  Path | str) -> N
+000096f0: 6f6e 653a 0a20 2020 2020 2020 2061 7379  one:.        asy
+00009700: 6e63 2077 6974 6820 6177 6169 7420 6372  nc with await cr
+00009710: 6561 7465 5f75 6e69 785f 6c69 7374 656e  eate_unix_listen
+00009720: 6572 2873 6f63 6b65 745f 7061 7468 5f6f  er(socket_path_o
+00009730: 725f 7374 7229 2061 7320 6c69 7374 656e  r_str) as listen
+00009740: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
+00009750: 636c 6965 6e74 203d 2073 6f63 6b65 742e  client = socket.
+00009760: 736f 636b 6574 2873 6f63 6b65 742e 4146  socket(socket.AF
+00009770: 5f55 4e49 5829 0a20 2020 2020 2020 2020  _UNIX).         
+00009780: 2020 2063 6c69 656e 742e 7365 7474 696d     client.settim
+00009790: 656f 7574 2831 290a 2020 2020 2020 2020  eout(1).        
+000097a0: 2020 2020 636c 6965 6e74 2e63 6f6e 6e65      client.conne
+000097b0: 6374 2873 7472 2873 6f63 6b65 745f 7061  ct(str(socket_pa
+000097c0: 7468 5f6f 725f 7374 7229 290a 2020 2020  th_or_str)).    
+000097d0: 2020 2020 2020 2020 7374 7265 616d 203d          stream =
+000097e0: 2061 7761 6974 206c 6973 7465 6e65 722e   await listener.
+000097f0: 6163 6365 7074 2829 0a20 2020 2020 2020  accept().       
+00009800: 2020 2020 2063 6c69 656e 742e 7365 6e64       client.send
+00009810: 616c 6c28 6222 626c 6168 2229 0a20 2020  all(b"blah").   
+00009820: 2020 2020 2020 2020 2072 6571 7565 7374           request
+00009830: 203d 2061 7761 6974 2073 7472 6561 6d2e   = await stream.
+00009840: 7265 6365 6976 6528 290a 2020 2020 2020  receive().      
+00009850: 2020 2020 2020 6177 6169 7420 7374 7265        await stre
+00009860: 616d 2e73 656e 6428 7265 7175 6573 745b  am.send(request[
+00009870: 3a3a 2d31 5d29 0a20 2020 2020 2020 2020  ::-1]).         
+00009880: 2020 2061 7373 6572 7420 636c 6965 6e74     assert client
+00009890: 2e72 6563 7628 3130 3029 203d 3d20 6222  .recv(100) == b"
+000098a0: 6861 6c62 220a 2020 2020 2020 2020 2020  halb".          
+000098b0: 2020 636c 6965 6e74 2e63 6c6f 7365 2829    client.close()
+000098c0: 0a20 2020 2020 2020 2020 2020 2061 7761  .            awa
+000098d0: 6974 2073 7472 6561 6d2e 6163 6c6f 7365  it stream.aclose
+000098e0: 2829 0a0a 2020 2020 6173 796e 6320 6465  ()..    async de
+000098f0: 6620 7465 7374 5f73 6f63 6b65 745f 6f70  f test_socket_op
+00009900: 7469 6f6e 7328 7365 6c66 2c20 736f 636b  tions(self, sock
+00009910: 6574 5f70 6174 683a 2050 6174 6829 202d  et_path: Path) -
+00009920: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00009930: 6173 796e 6320 7769 7468 2061 7761 6974  async with await
+00009940: 2063 7265 6174 655f 756e 6978 5f6c 6973   create_unix_lis
+00009950: 7465 6e65 7228 736f 636b 6574 5f70 6174  tener(socket_pat
+00009960: 6829 2061 7320 6c69 7374 656e 6572 3a0a  h) as listener:.
+00009970: 2020 2020 2020 2020 2020 2020 6c69 7374              list
+00009980: 656e 6572 5f73 6f63 6b65 7420 3d20 6c69  ener_socket = li
+00009990: 7374 656e 6572 2e65 7874 7261 2853 6f63  stener.extra(Soc
+000099a0: 6b65 7441 7474 7269 6275 7465 2e72 6177  ketAttribute.raw
+000099b0: 5f73 6f63 6b65 7429 0a20 2020 2020 2020  _socket).       
+000099c0: 2020 2020 2061 7373 6572 7420 6c69 7374       assert list
+000099d0: 656e 6572 5f73 6f63 6b65 742e 6661 6d69  ener_socket.fami
+000099e0: 6c79 203d 3d20 736f 636b 6574 2e41 6464  ly == socket.Add
+000099f0: 7265 7373 4661 6d69 6c79 2e41 465f 554e  ressFamily.AF_UN
+00009a00: 4958 0a20 2020 2020 2020 2020 2020 206c  IX.            l
+00009a10: 6973 7465 6e65 725f 736f 636b 6574 2e73  istener_socket.s
+00009a20: 6574 736f 636b 6f70 7428 736f 636b 6574  etsockopt(socket
+00009a30: 2e53 4f4c 5f53 4f43 4b45 542c 2073 6f63  .SOL_SOCKET, soc
+00009a40: 6b65 742e 534f 5f52 4356 4255 462c 2038  ket.SO_RCVBUF, 8
+00009a50: 3030 3030 290a 2020 2020 2020 2020 2020  0000).          
+00009a60: 2020 6173 7365 7274 206c 6973 7465 6e65    assert listene
+00009a70: 725f 736f 636b 6574 2e67 6574 736f 636b  r_socket.getsock
+00009a80: 6f70 7428 736f 636b 6574 2e53 4f4c 5f53  opt(socket.SOL_S
+00009a90: 4f43 4b45 542c 2073 6f63 6b65 742e 534f  OCKET, socket.SO
+00009aa0: 5f52 4356 4255 4629 2069 6e20 280a 2020  _RCVBUF) in (.  
+00009ab0: 2020 2020 2020 2020 2020 2020 2020 3830                80
+00009ac0: 3030 302c 0a20 2020 2020 2020 2020 2020  000,.           
+00009ad0: 2020 2020 2031 3630 3030 302c 0a20 2020       160000,.   
+00009ae0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00009af0: 2020 2020 2020 2020 636c 6965 6e74 203d          client =
+00009b00: 2073 6f63 6b65 742e 736f 636b 6574 286c   socket.socket(l
+00009b10: 6973 7465 6e65 725f 736f 636b 6574 2e66  istener_socket.f
+00009b20: 616d 696c 7929 0a20 2020 2020 2020 2020  amily).         
+00009b30: 2020 2063 6c69 656e 742e 7365 7474 696d     client.settim
+00009b40: 656f 7574 2831 290a 2020 2020 2020 2020  eout(1).        
+00009b50: 2020 2020 636c 6965 6e74 2e63 6f6e 6e65      client.conne
+00009b60: 6374 286c 6973 7465 6e65 725f 736f 636b  ct(listener_sock
+00009b70: 6574 2e67 6574 736f 636b 6e61 6d65 2829  et.getsockname()
+00009b80: 290a 0a20 2020 2020 2020 2020 2020 2061  )..            a
+00009b90: 7379 6e63 2077 6974 6820 6177 6169 7420  sync with await 
+00009ba0: 6c69 7374 656e 6572 2e61 6363 6570 7428  listener.accept(
+00009bb0: 2920 6173 2073 7472 6561 6d3a 0a20 2020  ) as stream:.   
+00009bc0: 2020 2020 2020 2020 2020 2020 2061 7373               ass
+00009bd0: 6572 7420 7374 7265 616d 2e65 7874 7261  ert stream.extra
+00009be0: 2853 6f63 6b65 7441 7474 7269 6275 7465  (SocketAttribute
+00009bf0: 2e72 6177 5f73 6f63 6b65 7429 2e67 6574  .raw_socket).get
+00009c00: 7469 6d65 6f75 7428 2920 3d3d 2030 0a20  timeout() == 0. 
+00009c10: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00009c20: 7373 6572 7420 7374 7265 616d 2e65 7874  ssert stream.ext
+00009c30: 7261 2853 6f63 6b65 7441 7474 7269 6275  ra(SocketAttribu
+00009c40: 7465 2e66 616d 696c 7929 203d 3d20 6c69  te.family) == li
+00009c50: 7374 656e 6572 5f73 6f63 6b65 742e 6661  stener_socket.fa
+00009c60: 6d69 6c79 0a0a 2020 2020 2020 2020 2020  mily..          
+00009c70: 2020 636c 6965 6e74 2e63 6c6f 7365 2829    client.close()
+00009c80: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+00009c90: 7465 7374 5f73 656e 645f 6166 7465 725f  test_send_after_
+00009ca0: 656f 6628 7365 6c66 2c20 736f 636b 6574  eof(self, socket
+00009cb0: 5f70 6174 683a 2050 6174 6829 202d 3e20  _path: Path) -> 
+00009cc0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6173  None:.        as
+00009cd0: 796e 6320 6465 6620 6861 6e64 6c65 2873  ync def handle(s
+00009ce0: 7472 6561 6d3a 2053 6f63 6b65 7453 7472  tream: SocketStr
+00009cf0: 6561 6d29 202d 3e20 4e6f 6e65 3a0a 2020  eam) -> None:.  
+00009d00: 2020 2020 2020 2020 2020 6173 796e 6320            async 
+00009d10: 7769 7468 2073 7472 6561 6d3a 0a20 2020  with stream:.   
+00009d20: 2020 2020 2020 2020 2020 2020 2061 7761               awa
+00009d30: 6974 2073 7472 6561 6d2e 7365 6e64 2862  it stream.send(b
+00009d40: 2248 656c 6c6f 5c6e 2229 0a0a 2020 2020  "Hello\n")..    
+00009d50: 2020 2020 6173 796e 6320 7769 7468 2061      async with a
+00009d60: 7761 6974 2063 7265 6174 655f 756e 6978  wait create_unix
+00009d70: 5f6c 6973 7465 6e65 7228 0a20 2020 2020  _listener(.     
+00009d80: 2020 2020 2020 2073 6f63 6b65 745f 7061         socket_pa
+00009d90: 7468 0a20 2020 2020 2020 2029 2061 7320  th.        ) as 
+00009da0: 6c69 7374 656e 6572 2c20 6372 6561 7465  listener, create
+00009db0: 5f74 6173 6b5f 6772 6f75 7028 2920 6173  _task_group() as
+00009dc0: 2074 673a 0a20 2020 2020 2020 2020 2020   tg:.           
+00009dd0: 2074 672e 7374 6172 745f 736f 6f6e 286c   tg.start_soon(l
+00009de0: 6973 7465 6e65 722e 7365 7276 652c 2068  istener.serve, h
+00009df0: 616e 646c 6529 0a20 2020 2020 2020 2020  andle).         
+00009e00: 2020 2061 7761 6974 2077 6169 745f 616c     await wait_al
+00009e10: 6c5f 7461 736b 735f 626c 6f63 6b65 6428  l_tasks_blocked(
+00009e20: 290a 0a20 2020 2020 2020 2020 2020 2077  )..            w
+00009e30: 6974 6820 736f 636b 6574 2e73 6f63 6b65  ith socket.socke
+00009e40: 7428 736f 636b 6574 2e41 465f 554e 4958  t(socket.AF_UNIX
+00009e50: 2920 6173 2063 6c69 656e 743a 0a20 2020  ) as client:.   
+00009e60: 2020 2020 2020 2020 2020 2020 2063 6c69               cli
+00009e70: 656e 742e 636f 6e6e 6563 7428 7374 7228  ent.connect(str(
+00009e80: 736f 636b 6574 5f70 6174 6829 290a 2020  socket_path)).  
+00009e90: 2020 2020 2020 2020 2020 2020 2020 636c                cl
+00009ea0: 6965 6e74 2e73 6875 7464 6f77 6e28 736f  ient.shutdown(so
+00009eb0: 636b 6574 2e53 4855 545f 5752 290a 2020  cket.SHUT_WR).  
+00009ec0: 2020 2020 2020 2020 2020 2020 2020 636c                cl
+00009ed0: 6965 6e74 2e73 6574 626c 6f63 6b69 6e67  ient.setblocking
+00009ee0: 2846 616c 7365 290a 2020 2020 2020 2020  (False).        
+00009ef0: 2020 2020 2020 2020 7769 7468 2066 6169          with fai
+00009f00: 6c5f 6166 7465 7228 3129 3a0a 2020 2020  l_after(1):.    
+00009f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f20: 7768 696c 6520 5472 7565 3a0a 2020 2020  while True:.    
+00009f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f40: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00009f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f60: 2020 2020 206d 6573 7361 6765 203d 2063       message = c
+00009f70: 6c69 656e 742e 7265 6376 2831 3029 0a20  lient.recv(10). 
+00009f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f90: 2020 2020 2020 2065 7863 6570 7420 426c         except Bl
+00009fa0: 6f63 6b69 6e67 494f 4572 726f 723a 0a20  ockingIOError:. 
+00009fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fc0: 2020 2020 2020 2020 2020 2061 7761 6974             await
+00009fd0: 2073 6c65 6570 2830 290a 2020 2020 2020   sleep(0).      
+00009fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ff0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000a000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a010: 2020 2020 6173 7365 7274 206d 6573 7361      assert messa
+0000a020: 6765 203d 3d20 6222 4865 6c6c 6f5c 6e22  ge == b"Hello\n"
+0000a030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a040: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+0000a050: 616b 0a0a 2020 2020 2020 2020 2020 2020  ak..            
+0000a060: 7467 2e63 616e 6365 6c5f 7363 6f70 652e  tg.cancel_scope.
+0000a070: 6361 6e63 656c 2829 0a0a 2020 2020 6173  cancel()..    as
+0000a080: 796e 6320 6465 6620 7465 7374 5f62 696e  ync def test_bin
+0000a090: 645f 7477 6963 6528 7365 6c66 2c20 736f  d_twice(self, so
+0000a0a0: 636b 6574 5f70 6174 683a 2050 6174 6829  cket_path: Path)
+0000a0b0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+0000a0c0: 2020 2222 2254 6573 7420 7468 6174 2074    """Test that t
+0000a0d0: 6865 2070 7265 7669 6f75 7320 736f 636b  he previous sock
+0000a0e0: 6574 2069 7320 7265 6d6f 7665 6420 6265  et is removed be
+0000a0f0: 666f 7265 2062 696e 6469 6e67 2074 6f20  fore binding to 
+0000a100: 7468 6520 7061 7468 2e22 2222 0a20 2020  the path.""".   
+0000a110: 2020 2020 2066 6f72 205f 2069 6e20 7261       for _ in ra
+0000a120: 6e67 6528 3229 3a0a 2020 2020 2020 2020  nge(2):.        
+0000a130: 2020 2020 6173 796e 6320 7769 7468 2061      async with a
+0000a140: 7761 6974 2063 7265 6174 655f 756e 6978  wait create_unix
+0000a150: 5f6c 6973 7465 6e65 7228 736f 636b 6574  _listener(socket
+0000a160: 5f70 6174 6829 3a0a 2020 2020 2020 2020  _path):.        
+0000a170: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+0000a180: 2020 6173 796e 6320 6465 6620 7465 7374    async def test
+0000a190: 5f6c 6973 7465 6e69 6e67 5f62 7974 6573  _listening_bytes
+0000a1a0: 5f70 6174 6828 7365 6c66 2c20 736f 636b  _path(self, sock
+0000a1b0: 6574 5f70 6174 683a 2050 6174 6829 202d  et_path: Path) -
+0000a1c0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000a1d0: 6173 796e 6320 7769 7468 2061 7761 6974  async with await
+0000a1e0: 2063 7265 6174 655f 756e 6978 5f6c 6973   create_unix_lis
+0000a1f0: 7465 6e65 7228 7374 7228 736f 636b 6574  tener(str(socket
+0000a200: 5f70 6174 6829 2e65 6e63 6f64 6528 2929  _path).encode())
+0000a210: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
+0000a220: 7373 0a0a 2020 2020 4070 7974 6573 742e  ss..    @pytest.
+0000a230: 6d61 726b 2e73 6b69 7069 6628 0a20 2020  mark.skipif(.   
+0000a240: 2020 2020 2070 6c61 7466 6f72 6d2e 7379       platform.sy
+0000a250: 7374 656d 2829 203d 3d20 2244 6172 7769  stem() == "Darwi
+0000a260: 6e22 2c20 7265 6173 6f6e 3d22 6d61 634f  n", reason="macO
+0000a270: 5320 7265 7175 6972 6573 2076 616c 6964  S requires valid
+0000a280: 2055 5446 2d38 2070 6174 6873 220a 2020   UTF-8 paths".  
+0000a290: 2020 290a 2020 2020 6173 796e 6320 6465    ).    async de
+0000a2a0: 6620 7465 7374 5f6c 6973 7465 6e69 6e67  f test_listening
+0000a2b0: 5f69 6e76 616c 6964 5f61 7363 6969 2873  _invalid_ascii(s
+0000a2c0: 656c 662c 2073 6f63 6b65 745f 7061 7468  elf, socket_path
+0000a2d0: 3a20 5061 7468 2920 2d3e 204e 6f6e 653a  : Path) -> None:
+0000a2e0: 0a20 2020 2020 2020 2072 6561 6c5f 7061  .        real_pa
+0000a2f0: 7468 203d 2073 7472 2873 6f63 6b65 745f  th = str(socket_
+0000a300: 7061 7468 292e 656e 636f 6465 2829 202b  path).encode() +
+0000a310: 2062 225c 7866 3022 0a20 2020 2020 2020   b"\xf0".       
+0000a320: 2061 7379 6e63 2077 6974 6820 6177 6169   async with awai
+0000a330: 7420 6372 6561 7465 5f75 6e69 785f 6c69  t create_unix_li
+0000a340: 7374 656e 6572 2872 6561 6c5f 7061 7468  stener(real_path
+0000a350: 293a 0a20 2020 2020 2020 2020 2020 2070  ):.            p
+0000a360: 6173 730a 0a0a 6173 796e 6320 6465 6620  ass...async def 
+0000a370: 7465 7374 5f6d 756c 7469 5f6c 6973 7465  test_multi_liste
+0000a380: 6e65 7228 746d 705f 7061 7468 5f66 6163  ner(tmp_path_fac
+0000a390: 746f 7279 3a20 5465 6d70 5061 7468 4661  tory: TempPathFa
+0000a3a0: 6374 6f72 7929 202d 3e20 4e6f 6e65 3a0a  ctory) -> None:.
+0000a3b0: 2020 2020 6173 796e 6320 6465 6620 6861      async def ha
+0000a3c0: 6e64 6c65 2873 7472 6561 6d3a 2053 6f63  ndle(stream: Soc
+0000a3d0: 6b65 7453 7472 6561 6d29 202d 3e20 4e6f  ketStream) -> No
+0000a3e0: 6e65 3a0a 2020 2020 2020 2020 636c 6965  ne:.        clie
+0000a3f0: 6e74 5f61 6464 7265 7373 6573 2e61 7070  nt_addresses.app
+0000a400: 656e 6428 7374 7265 616d 2e65 7874 7261  end(stream.extra
+0000a410: 2853 6f63 6b65 7441 7474 7269 6275 7465  (SocketAttribute
+0000a420: 2e72 656d 6f74 655f 6164 6472 6573 7329  .remote_address)
+0000a430: 290a 2020 2020 2020 2020 6576 656e 742e  ).        event.
+0000a440: 7365 7428 290a 2020 2020 2020 2020 6177  set().        aw
+0000a450: 6169 7420 7374 7265 616d 2e61 636c 6f73  ait stream.aclos
+0000a460: 6528 290a 0a20 2020 2063 6c69 656e 745f  e()..    client_
+0000a470: 6164 6472 6573 7365 733a 206c 6973 745b  addresses: list[
+0000a480: 7374 7220 7c20 4950 536f 636b 4164 6472  str | IPSockAddr
+0000a490: 5479 7065 5d20 3d20 5b5d 0a20 2020 206c  Type] = [].    l
+0000a4a0: 6973 7465 6e65 7273 3a20 6c69 7374 5b4c  isteners: list[L
+0000a4b0: 6973 7465 6e65 725d 203d 205b 6177 6169  istener] = [awai
+0000a4c0: 7420 6372 6561 7465 5f74 6370 5f6c 6973  t create_tcp_lis
+0000a4d0: 7465 6e65 7228 6c6f 6361 6c5f 686f 7374  tener(local_host
+0000a4e0: 3d22 6c6f 6361 6c68 6f73 7422 295d 0a20  ="localhost")]. 
+0000a4f0: 2020 2077 6974 6820 7465 6d70 6669 6c65     with tempfile
+0000a500: 2e54 656d 706f 7261 7279 4469 7265 6374  .TemporaryDirect
+0000a510: 6f72 7928 2920 6173 2070 6174 683a 0a20  ory() as path:. 
+0000a520: 2020 2020 2020 2069 6620 7379 732e 706c         if sys.pl
+0000a530: 6174 666f 726d 2021 3d20 2277 696e 3332  atform != "win32
+0000a540: 223a 0a20 2020 2020 2020 2020 2020 206c  ":.            l
+0000a550: 6973 7465 6e65 7273 2e61 7070 656e 6428  isteners.append(
+0000a560: 6177 6169 7420 6372 6561 7465 5f75 6e69  await create_uni
+0000a570: 785f 6c69 7374 656e 6572 2850 6174 6828  x_listener(Path(
+0000a580: 7061 7468 2920 2f20 2273 6f63 6b65 7422  path) / "socket"
+0000a590: 2929 0a0a 2020 2020 2020 2020 6578 7065  ))..        expe
+0000a5a0: 6374 6564 5f61 6464 7265 7373 6573 3a20  cted_addresses: 
+0000a5b0: 6c69 7374 5b73 7472 207c 2049 5053 6f63  list[str | IPSoc
+0000a5c0: 6b41 6464 7254 7970 655d 203d 205b 5d0a  kAddrType] = [].
+0000a5d0: 2020 2020 2020 2020 6173 796e 6320 7769          async wi
+0000a5e0: 7468 204d 756c 7469 4c69 7374 656e 6572  th MultiListener
+0000a5f0: 286c 6973 7465 6e65 7273 2920 6173 206d  (listeners) as m
+0000a600: 756c 7469 5f6c 6973 7465 6e65 723a 0a20  ulti_listener:. 
+0000a610: 2020 2020 2020 2020 2020 2061 7379 6e63             async
+0000a620: 2077 6974 6820 6372 6561 7465 5f74 6173   with create_tas
+0000a630: 6b5f 6772 6f75 7028 2920 6173 2074 673a  k_group() as tg:
+0000a640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a650: 2074 672e 7374 6172 745f 736f 6f6e 286d   tg.start_soon(m
+0000a660: 756c 7469 5f6c 6973 7465 6e65 722e 7365  ulti_listener.se
+0000a670: 7276 652c 2068 616e 646c 6529 0a20 2020  rve, handle).   
+0000a680: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000a690: 206c 6973 7465 6e65 7220 696e 206d 756c   listener in mul
+0000a6a0: 7469 5f6c 6973 7465 6e65 722e 6c69 7374  ti_listener.list
+0000a6b0: 656e 6572 733a 0a20 2020 2020 2020 2020  eners:.         
+0000a6c0: 2020 2020 2020 2020 2020 2065 7665 6e74             event
+0000a6d0: 203d 2045 7665 6e74 2829 0a20 2020 2020   = Event().     
+0000a6e0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000a6f0: 6f63 616c 5f61 6464 7265 7373 203d 206c  ocal_address = l
+0000a700: 6973 7465 6e65 722e 6578 7472 6128 536f  istener.extra(So
+0000a710: 636b 6574 4174 7472 6962 7574 652e 6c6f  cketAttribute.lo
+0000a720: 6361 6c5f 6164 6472 6573 7329 0a20 2020  cal_address).   
+0000a730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a740: 2069 6620 280a 2020 2020 2020 2020 2020   if (.          
+0000a750: 2020 2020 2020 2020 2020 2020 2020 7379                sy
+0000a760: 732e 706c 6174 666f 726d 2021 3d20 2277  s.platform != "w
+0000a770: 696e 3332 220a 2020 2020 2020 2020 2020  in32".          
+0000a780: 2020 2020 2020 2020 2020 2020 2020 616e                an
+0000a790: 6420 6c69 7374 656e 6572 2e65 7874 7261  d listener.extra
+0000a7a0: 2853 6f63 6b65 7441 7474 7269 6275 7465  (SocketAttribute
+0000a7b0: 2e66 616d 696c 7929 0a20 2020 2020 2020  .family).       
+0000a7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7d0: 203d 3d20 736f 636b 6574 2e41 6464 7265   == socket.Addre
+0000a7e0: 7373 4661 6d69 6c79 2e41 465f 554e 4958  ssFamily.AF_UNIX
+0000a7f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a800: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
+0000a810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a820: 6173 7365 7274 2069 7369 6e73 7461 6e63  assert isinstanc
+0000a830: 6528 6c6f 6361 6c5f 6164 6472 6573 732c  e(local_address,
+0000a840: 2073 7472 290a 2020 2020 2020 2020 2020   str).          
+0000a850: 2020 2020 2020 2020 2020 2020 2020 7374                st
+0000a860: 7265 616d 3a20 536f 636b 6574 5374 7265  ream: SocketStre
+0000a870: 616d 203d 2061 7761 6974 2063 6f6e 6e65  am = await conne
+0000a880: 6374 5f75 6e69 7828 6c6f 6361 6c5f 6164  ct_unix(local_ad
+0000a890: 6472 6573 7329 0a20 2020 2020 2020 2020  dress).         
+0000a8a0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000a8b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a8c0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+0000a8d0: 6973 696e 7374 616e 6365 286c 6f63 616c  isinstance(local
+0000a8e0: 5f61 6464 7265 7373 2c20 7475 706c 6529  _address, tuple)
+0000a8f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a900: 2020 2020 2020 2020 2073 7472 6561 6d20           stream 
+0000a910: 3d20 6177 6169 7420 636f 6e6e 6563 745f  = await connect_
+0000a920: 7463 7028 2a6c 6f63 616c 5f61 6464 7265  tcp(*local_addre
+0000a930: 7373 290a 0a20 2020 2020 2020 2020 2020  ss)..           
+0000a940: 2020 2020 2020 2020 2065 7870 6563 7465           expecte
+0000a950: 645f 6164 6472 6573 7365 732e 6170 7065  d_addresses.appe
+0000a960: 6e64 280a 2020 2020 2020 2020 2020 2020  nd(.            
+0000a970: 2020 2020 2020 2020 2020 2020 7374 7265              stre
+0000a980: 616d 2e65 7874 7261 2853 6f63 6b65 7441  am.extra(SocketA
+0000a990: 7474 7269 6275 7465 2e6c 6f63 616c 5f61  ttribute.local_a
+0000a9a0: 6464 7265 7373 290a 2020 2020 2020 2020  ddress).        
+0000a9b0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000a9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a9d0: 2020 6177 6169 7420 6576 656e 742e 7761    await event.wa
+0000a9e0: 6974 2829 0a20 2020 2020 2020 2020 2020  it().           
+0000a9f0: 2020 2020 2020 2020 2061 7761 6974 2073           await s
+0000aa00: 7472 6561 6d2e 6163 6c6f 7365 2829 0a0a  tream.aclose()..
+0000aa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa20: 7467 2e63 616e 6365 6c5f 7363 6f70 652e  tg.cancel_scope.
+0000aa30: 6361 6e63 656c 2829 0a0a 2020 2020 2020  cancel()..      
+0000aa40: 2020 6173 7365 7274 2063 6c69 656e 745f    assert client_
+0000aa50: 6164 6472 6573 7365 7320 3d3d 2065 7870  addresses == exp
+0000aa60: 6563 7465 645f 6164 6472 6573 7365 730a  ected_addresses.
+0000aa70: 0a0a 4070 7974 6573 742e 6d61 726b 2e6e  ..@pytest.mark.n
+0000aa80: 6574 776f 726b 0a40 7079 7465 7374 2e6d  etwork.@pytest.m
+0000aa90: 6172 6b2e 7573 6566 6978 7475 7265 7328  ark.usefixtures(
+0000aaa0: 2263 6865 636b 5f61 7379 6e63 696f 5f62  "check_asyncio_b
+0000aab0: 7567 2229 0a63 6c61 7373 2054 6573 7455  ug").class TestU
+0000aac0: 4450 536f 636b 6574 3a0a 2020 2020 6173  DPSocket:.    as
+0000aad0: 796e 6320 6465 6620 7465 7374 5f65 7874  ync def test_ext
+0000aae0: 7261 5f61 7474 7269 6275 7465 7328 7365  ra_attributes(se
+0000aaf0: 6c66 2c20 6661 6d69 6c79 3a20 416e 7949  lf, family: AnyI
+0000ab00: 5041 6464 7265 7373 4661 6d69 6c79 2920  PAddressFamily) 
+0000ab10: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0000ab20: 2061 7379 6e63 2077 6974 6820 6177 6169   async with awai
+0000ab30: 7420 6372 6561 7465 5f75 6470 5f73 6f63  t create_udp_soc
+0000ab40: 6b65 7428 0a20 2020 2020 2020 2020 2020  ket(.           
+0000ab50: 2066 616d 696c 793d 6661 6d69 6c79 2c20   family=family, 
+0000ab60: 6c6f 6361 6c5f 686f 7374 3d22 6c6f 6361  local_host="loca
+0000ab70: 6c68 6f73 7422 0a20 2020 2020 2020 2029  lhost".        )
+0000ab80: 2061 7320 7564 703a 0a20 2020 2020 2020   as udp:.       
+0000ab90: 2020 2020 2072 6177 5f73 6f63 6b65 7420       raw_socket 
+0000aba0: 3d20 7564 702e 6578 7472 6128 536f 636b  = udp.extra(Sock
+0000abb0: 6574 4174 7472 6962 7574 652e 7261 775f  etAttribute.raw_
+0000abc0: 736f 636b 6574 290a 2020 2020 2020 2020  socket).        
+0000abd0: 2020 2020 6173 7365 7274 2072 6177 5f73      assert raw_s
+0000abe0: 6f63 6b65 742e 6765 7474 696d 656f 7574  ocket.gettimeout
+0000abf0: 2829 203d 3d20 300a 2020 2020 2020 2020  () == 0.        
+0000ac00: 2020 2020 6173 7365 7274 2075 6470 2e65      assert udp.e
+0000ac10: 7874 7261 2853 6f63 6b65 7441 7474 7269  xtra(SocketAttri
+0000ac20: 6275 7465 2e66 616d 696c 7929 203d 3d20  bute.family) == 
+0000ac30: 6661 6d69 6c79 0a20 2020 2020 2020 2020  family.         
+0000ac40: 2020 2061 7373 6572 7420 280a 2020 2020     assert (.    
+0000ac50: 2020 2020 2020 2020 2020 2020 7564 702e              udp.
+0000ac60: 6578 7472 6128 536f 636b 6574 4174 7472  extra(SocketAttr
+0000ac70: 6962 7574 652e 6c6f 6361 6c5f 6164 6472  ibute.local_addr
+0000ac80: 6573 7329 203d 3d20 7261 775f 736f 636b  ess) == raw_sock
+0000ac90: 6574 2e67 6574 736f 636b 6e61 6d65 2829  et.getsockname()
+0000aca0: 5b3a 325d 0a20 2020 2020 2020 2020 2020  [:2].           
+0000acb0: 2029 0a20 2020 2020 2020 2020 2020 2061   ).            a
+0000acc0: 7373 6572 7420 7564 702e 6578 7472 6128  ssert udp.extra(
+0000acd0: 536f 636b 6574 4174 7472 6962 7574 652e  SocketAttribute.
+0000ace0: 6c6f 6361 6c5f 706f 7274 2920 3d3d 2072  local_port) == r
+0000acf0: 6177 5f73 6f63 6b65 742e 6765 7473 6f63  aw_socket.getsoc
+0000ad00: 6b6e 616d 6528 295b 315d 0a20 2020 2020  kname()[1].     
+0000ad10: 2020 2020 2020 2070 7974 6573 742e 7261         pytest.ra
+0000ad20: 6973 6573 280a 2020 2020 2020 2020 2020  ises(.          
+0000ad30: 2020 2020 2020 5479 7065 6441 7474 7269        TypedAttri
+0000ad40: 6275 7465 4c6f 6f6b 7570 4572 726f 722c  buteLookupError,
+0000ad50: 2075 6470 2e65 7874 7261 2c20 536f 636b   udp.extra, Sock
+0000ad60: 6574 4174 7472 6962 7574 652e 7265 6d6f  etAttribute.remo
+0000ad70: 7465 5f61 6464 7265 7373 0a20 2020 2020  te_address.     
+0000ad80: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000ad90: 2020 2020 2070 7974 6573 742e 7261 6973       pytest.rais
+0000ada0: 6573 280a 2020 2020 2020 2020 2020 2020  es(.            
+0000adb0: 2020 2020 5479 7065 6441 7474 7269 6275      TypedAttribu
+0000adc0: 7465 4c6f 6f6b 7570 4572 726f 722c 2075  teLookupError, u
+0000add0: 6470 2e65 7874 7261 2c20 536f 636b 6574  dp.extra, Socket
+0000ade0: 4174 7472 6962 7574 652e 7265 6d6f 7465  Attribute.remote
+0000adf0: 5f70 6f72 740a 2020 2020 2020 2020 2020  _port.          
+0000ae00: 2020 290a 0a20 2020 2061 7379 6e63 2064    )..    async d
+0000ae10: 6566 2074 6573 745f 7365 6e64 5f72 6563  ef test_send_rec
+0000ae20: 6569 7665 2873 656c 662c 2066 616d 696c  eive(self, famil
+0000ae30: 793a 2041 6e79 4950 4164 6472 6573 7346  y: AnyIPAddressF
+0000ae40: 616d 696c 7929 202d 3e20 4e6f 6e65 3a0a  amily) -> None:.
+0000ae50: 2020 2020 2020 2020 6173 796e 6320 7769          async wi
+0000ae60: 7468 2061 7761 6974 2063 7265 6174 655f  th await create_
+0000ae70: 7564 705f 736f 636b 6574 280a 2020 2020  udp_socket(.    
+0000ae80: 2020 2020 2020 2020 6c6f 6361 6c5f 686f          local_ho
+0000ae90: 7374 3d22 6c6f 6361 6c68 6f73 7422 2c20  st="localhost", 
+0000aea0: 6661 6d69 6c79 3d66 616d 696c 790a 2020  family=family.  
+0000aeb0: 2020 2020 2020 2920 6173 2073 6f63 6b3a        ) as sock:
+0000aec0: 0a20 2020 2020 2020 2020 2020 2068 6f73  .            hos
+0000aed0: 742c 2070 6f72 7420 3d20 736f 636b 2e65  t, port = sock.e
+0000aee0: 7874 7261 2853 6f63 6b65 7441 7474 7269  xtra(SocketAttri
+0000aef0: 6275 7465 2e6c 6f63 616c 5f61 6464 7265  bute.local_addre
+0000af00: 7373 2920 2023 2074 7970 653a 2069 676e  ss)  # type: ign
+0000af10: 6f72 655b 6d69 7363 5d0a 2020 2020 2020  ore[misc].      
+0000af20: 2020 2020 2020 6177 6169 7420 736f 636b        await sock
+0000af30: 2e73 656e 6474 6f28 6222 626c 6168 222c  .sendto(b"blah",
+0000af40: 2068 6f73 742c 2070 6f72 7429 0a20 2020   host, port).   
+0000af50: 2020 2020 2020 2020 2072 6571 7565 7374           request
+0000af60: 2c20 6164 6472 203d 2061 7761 6974 2073  , addr = await s
+0000af70: 6f63 6b2e 7265 6365 6976 6528 290a 2020  ock.receive().  
+0000af80: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+0000af90: 2072 6571 7565 7374 203d 3d20 6222 626c   request == b"bl
+0000afa0: 6168 220a 2020 2020 2020 2020 2020 2020  ah".            
+0000afb0: 6173 7365 7274 2061 6464 7220 3d3d 2073  assert addr == s
+0000afc0: 6f63 6b2e 6578 7472 6128 536f 636b 6574  ock.extra(Socket
+0000afd0: 4174 7472 6962 7574 652e 6c6f 6361 6c5f  Attribute.local_
+0000afe0: 6164 6472 6573 7329 0a0a 2020 2020 2020  address)..      
+0000aff0: 2020 2020 2020 6177 6169 7420 736f 636b        await sock
+0000b000: 2e73 656e 6474 6f28 6222 6861 6c62 222c  .sendto(b"halb",
+0000b010: 2068 6f73 742c 2070 6f72 7429 0a20 2020   host, port).   
+0000b020: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
+0000b030: 652c 2061 6464 7220 3d20 6177 6169 7420  e, addr = await 
+0000b040: 736f 636b 2e72 6563 6569 7665 2829 0a20  sock.receive(). 
+0000b050: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+0000b060: 7420 7265 7370 6f6e 7365 203d 3d20 6222  t response == b"
+0000b070: 6861 6c62 220a 2020 2020 2020 2020 2020  halb".          
+0000b080: 2020 6173 7365 7274 2061 6464 7220 3d3d    assert addr ==
+0000b090: 2028 686f 7374 2c20 706f 7274 290a 0a20   (host, port).. 
+0000b0a0: 2020 2061 7379 6e63 2064 6566 2074 6573     async def tes
+0000b0b0: 745f 6974 6572 6174 6528 7365 6c66 2c20  t_iterate(self, 
+0000b0c0: 6661 6d69 6c79 3a20 416e 7949 5041 6464  family: AnyIPAdd
+0000b0d0: 7265 7373 4661 6d69 6c79 2920 2d3e 204e  ressFamily) -> N
+0000b0e0: 6f6e 653a 0a20 2020 2020 2020 2061 7379  one:.        asy
+0000b0f0: 6e63 2064 6566 2073 6572 7665 2829 202d  nc def serve() -
+0000b100: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000b110: 2020 2020 6173 796e 6320 666f 7220 7061      async for pa
+0000b120: 636b 6574 2c20 6164 6472 2069 6e20 7365  cket, addr in se
+0000b130: 7276 6572 3a0a 2020 2020 2020 2020 2020  rver:.          
+0000b140: 2020 2020 2020 6177 6169 7420 7365 7276        await serv
+0000b150: 6572 2e73 656e 6428 2870 6163 6b65 745b  er.send((packet[
+0000b160: 3a3a 2d31 5d2c 2061 6464 7229 290a 0a20  ::-1], addr)).. 
+0000b170: 2020 2020 2020 2061 7379 6e63 2077 6974         async wit
+0000b180: 6820 6177 6169 7420 6372 6561 7465 5f75  h await create_u
+0000b190: 6470 5f73 6f63 6b65 7428 0a20 2020 2020  dp_socket(.     
+0000b1a0: 2020 2020 2020 2066 616d 696c 793d 6661         family=fa
+0000b1b0: 6d69 6c79 2c20 6c6f 6361 6c5f 686f 7374  mily, local_host
+0000b1c0: 3d22 6c6f 6361 6c68 6f73 7422 0a20 2020  ="localhost".   
+0000b1d0: 2020 2020 2029 2061 7320 7365 7276 6572       ) as server
+0000b1e0: 3a0a 2020 2020 2020 2020 2020 2020 686f  :.            ho
+0000b1f0: 7374 2c20 706f 7274 203d 2073 6572 7665  st, port = serve
+0000b200: 722e 6578 7472 6128 2020 2320 7479 7065  r.extra(  # type
+0000b210: 3a20 6967 6e6f 7265 5b6d 6973 635d 0a20  : ignore[misc]. 
+0000b220: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+0000b230: 6f63 6b65 7441 7474 7269 6275 7465 2e6c  ocketAttribute.l
+0000b240: 6f63 616c 5f61 6464 7265 7373 0a20 2020  ocal_address.   
+0000b250: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000b260: 2020 2020 2020 2061 7379 6e63 2077 6974         async wit
+0000b270: 6820 6177 6169 7420 6372 6561 7465 5f75  h await create_u
+0000b280: 6470 5f73 6f63 6b65 7428 0a20 2020 2020  dp_socket(.     
+0000b290: 2020 2020 2020 2020 2020 2066 616d 696c             famil
+0000b2a0: 793d 6661 6d69 6c79 2c20 6c6f 6361 6c5f  y=family, local_
+0000b2b0: 686f 7374 3d22 6c6f 6361 6c68 6f73 7422  host="localhost"
+0000b2c0: 0a20 2020 2020 2020 2020 2020 2029 2061  .            ) a
+0000b2d0: 7320 636c 6965 6e74 3a0a 2020 2020 2020  s client:.      
+0000b2e0: 2020 2020 2020 2020 2020 6173 796e 6320            async 
+0000b2f0: 7769 7468 2063 7265 6174 655f 7461 736b  with create_task
+0000b300: 5f67 726f 7570 2829 2061 7320 7467 3a0a  _group() as tg:.
+0000b310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b320: 2020 2020 7467 2e73 7461 7274 5f73 6f6f      tg.start_soo
+0000b330: 6e28 7365 7276 6529 0a20 2020 2020 2020  n(serve).       
+0000b340: 2020 2020 2020 2020 2020 2020 2061 7761               awa
+0000b350: 6974 2063 6c69 656e 742e 7365 6e64 746f  it client.sendto
+0000b360: 2862 2246 4f4f 4241 5222 2c20 686f 7374  (b"FOOBAR", host
+0000b370: 2c20 706f 7274 290a 2020 2020 2020 2020  , port).        
+0000b380: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+0000b390: 7274 2061 7761 6974 2063 6c69 656e 742e  rt await client.
+0000b3a0: 7265 6365 6976 6528 2920 3d3d 2028 6222  receive() == (b"
+0000b3b0: 5241 424f 4f46 222c 2028 686f 7374 2c20  RABOOF", (host, 
+0000b3c0: 706f 7274 2929 0a20 2020 2020 2020 2020  port)).         
+0000b3d0: 2020 2020 2020 2020 2020 2061 7761 6974             await
+0000b3e0: 2063 6c69 656e 742e 7365 6e64 746f 2862   client.sendto(b
+0000b3f0: 2231 3233 3435 3622 2c20 686f 7374 2c20  "123456", host, 
+0000b400: 706f 7274 290a 2020 2020 2020 2020 2020  port).          
+0000b410: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+0000b420: 2061 7761 6974 2063 6c69 656e 742e 7265   await client.re
+0000b430: 6365 6976 6528 2920 3d3d 2028 6222 3635  ceive() == (b"65
+0000b440: 3433 3231 222c 2028 686f 7374 2c20 706f  4321", (host, po
+0000b450: 7274 2929 0a20 2020 2020 2020 2020 2020  rt)).           
+0000b460: 2020 2020 2020 2020 2074 672e 6361 6e63           tg.canc
+0000b470: 656c 5f73 636f 7065 2e63 616e 6365 6c28  el_scope.cancel(
+0000b480: 290a 0a20 2020 2040 7079 7465 7374 2e6d  )..    @pytest.m
+0000b490: 6172 6b2e 736b 6970 6966 280a 2020 2020  ark.skipif(.    
+0000b4a0: 2020 2020 6e6f 7420 6861 7361 7474 7228      not hasattr(
+0000b4b0: 736f 636b 6574 2c20 2253 4f5f 5245 5553  socket, "SO_REUS
+0000b4c0: 4550 4f52 5422 292c 2072 6561 736f 6e3d  EPORT"), reason=
+0000b4d0: 2253 4f5f 5245 5553 4550 4f52 5420 6f70  "SO_REUSEPORT op
+0000b4e0: 7469 6f6e 206e 6f74 2073 7570 706f 7274  tion not support
+0000b4f0: 6564 220a 2020 2020 290a 2020 2020 6173  ed".    ).    as
+0000b500: 796e 6320 6465 6620 7465 7374 5f72 6575  ync def test_reu
+0000b510: 7365 5f70 6f72 7428 7365 6c66 2c20 6661  se_port(self, fa
+0000b520: 6d69 6c79 3a20 416e 7949 5041 6464 7265  mily: AnyIPAddre
+0000b530: 7373 4661 6d69 6c79 2920 2d3e 204e 6f6e  ssFamily) -> Non
+0000b540: 653a 0a20 2020 2020 2020 2061 7379 6e63  e:.        async
+0000b550: 2077 6974 6820 6177 6169 7420 6372 6561   with await crea
+0000b560: 7465 5f75 6470 5f73 6f63 6b65 7428 0a20  te_udp_socket(. 
+0000b570: 2020 2020 2020 2020 2020 2066 616d 696c             famil
+0000b580: 793d 6661 6d69 6c79 2c20 6c6f 6361 6c5f  y=family, local_
+0000b590: 686f 7374 3d22 6c6f 6361 6c68 6f73 7422  host="localhost"
+0000b5a0: 2c20 7265 7573 655f 706f 7274 3d54 7275  , reuse_port=Tru
+0000b5b0: 650a 2020 2020 2020 2020 2920 6173 2075  e.        ) as u
+0000b5c0: 6470 3a0a 2020 2020 2020 2020 2020 2020  dp:.            
+0000b5d0: 706f 7274 203d 2075 6470 2e65 7874 7261  port = udp.extra
+0000b5e0: 2853 6f63 6b65 7441 7474 7269 6275 7465  (SocketAttribute
+0000b5f0: 2e6c 6f63 616c 5f70 6f72 7429 0a20 2020  .local_port).   
+0000b600: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+0000b610: 706f 7274 2021 3d20 300a 2020 2020 2020  port != 0.      
+0000b620: 2020 2020 2020 6173 796e 6320 7769 7468        async with
+0000b630: 2061 7761 6974 2063 7265 6174 655f 7564   await create_ud
+0000b640: 705f 736f 636b 6574 280a 2020 2020 2020  p_socket(.      
+0000b650: 2020 2020 2020 2020 2020 6661 6d69 6c79            family
+0000b660: 3d66 616d 696c 792c 206c 6f63 616c 5f68  =family, local_h
+0000b670: 6f73 743d 226c 6f63 616c 686f 7374 222c  ost="localhost",
+0000b680: 206c 6f63 616c 5f70 6f72 743d 706f 7274   local_port=port
+0000b690: 2c20 7265 7573 655f 706f 7274 3d54 7275  , reuse_port=Tru
+0000b6a0: 650a 2020 2020 2020 2020 2020 2020 2920  e.            ) 
+0000b6b0: 6173 2075 6470 323a 0a20 2020 2020 2020  as udp2:.       
+0000b6c0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+0000b6d0: 706f 7274 203d 3d20 7564 7032 2e65 7874  port == udp2.ext
+0000b6e0: 7261 2853 6f63 6b65 7441 7474 7269 6275  ra(SocketAttribu
+0000b6f0: 7465 2e6c 6f63 616c 5f70 6f72 7429 0a0a  te.local_port)..
+0000b700: 2020 2020 6173 796e 6320 6465 6620 7465      async def te
+0000b710: 7374 5f63 6f6e 6375 7272 656e 745f 7265  st_concurrent_re
+0000b720: 6365 6976 6528 7365 6c66 2920 2d3e 204e  ceive(self) -> N
+0000b730: 6f6e 653a 0a20 2020 2020 2020 2061 7379  one:.        asy
+0000b740: 6e63 2077 6974 6820 6177 6169 7420 6372  nc with await cr
+0000b750: 6561 7465 5f75 6470 5f73 6f63 6b65 7428  eate_udp_socket(
+0000b760: 0a20 2020 2020 2020 2020 2020 2066 616d  .            fam
+0000b770: 696c 793d 4164 6472 6573 7346 616d 696c  ily=AddressFamil
+0000b780: 792e 4146 5f49 4e45 542c 206c 6f63 616c  y.AF_INET, local
+0000b790: 5f68 6f73 743d 226c 6f63 616c 686f 7374  _host="localhost
+0000b7a0: 220a 2020 2020 2020 2020 2920 6173 2075  ".        ) as u
+0000b7b0: 6470 3a0a 2020 2020 2020 2020 2020 2020  dp:.            
+0000b7c0: 6173 796e 6320 7769 7468 2063 7265 6174  async with creat
+0000b7d0: 655f 7461 736b 5f67 726f 7570 2829 2061  e_task_group() a
+0000b7e0: 7320 7467 3a0a 2020 2020 2020 2020 2020  s tg:.          
+0000b7f0: 2020 2020 2020 7467 2e73 7461 7274 5f73        tg.start_s
+0000b800: 6f6f 6e28 7564 702e 7265 6365 6976 6529  oon(udp.receive)
+0000b810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b820: 2061 7761 6974 2077 6169 745f 616c 6c5f   await wait_all_
+0000b830: 7461 736b 735f 626c 6f63 6b65 6428 290a  tasks_blocked().
+0000b840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b850: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+0000b860: 2020 2020 2020 2020 2077 6974 6820 7079           with py
+0000b870: 7465 7374 2e72 6169 7365 7328 4275 7379  test.raises(Busy
+0000b880: 5265 736f 7572 6365 4572 726f 7229 2061  ResourceError) a
+0000b890: 7320 6578 633a 0a20 2020 2020 2020 2020  s exc:.         
+0000b8a0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000b8b0: 7761 6974 2075 6470 2e72 6563 6569 7665  wait udp.receive
+0000b8c0: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
+0000b8d0: 2020 2020 2020 2020 6578 632e 6d61 7463          exc.matc
+0000b8e0: 6828 2261 6c72 6561 6479 2072 6561 6469  h("already readi
+0000b8f0: 6e67 2066 726f 6d22 290a 2020 2020 2020  ng from").      
+0000b900: 2020 2020 2020 2020 2020 6669 6e61 6c6c            finall
+0000b910: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+0000b920: 2020 2020 2020 2074 672e 6361 6e63 656c         tg.cancel
+0000b930: 5f73 636f 7065 2e63 616e 6365 6c28 290a  _scope.cancel().
+0000b940: 0a20 2020 2061 7379 6e63 2064 6566 2074  .    async def t
+0000b950: 6573 745f 636c 6f73 655f 6475 7269 6e67  est_close_during
+0000b960: 5f72 6563 6569 7665 2873 656c 6629 202d  _receive(self) -
+0000b970: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000b980: 6173 796e 6320 6465 6620 636c 6f73 655f  async def close_
+0000b990: 7768 656e 5f62 6c6f 636b 6564 2829 202d  when_blocked() -
+0000b9a0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000b9b0: 2020 2020 6177 6169 7420 7761 6974 5f61      await wait_a
+0000b9c0: 6c6c 5f74 6173 6b73 5f62 6c6f 636b 6564  ll_tasks_blocked
+0000b9d0: 2829 0a20 2020 2020 2020 2020 2020 2061  ().            a
+0000b9e0: 7761 6974 2075 6470 2e61 636c 6f73 6528  wait udp.aclose(
+0000b9f0: 290a 0a20 2020 2020 2020 2061 7379 6e63  )..        async
+0000ba00: 2077 6974 6820 6177 6169 7420 6372 6561   with await crea
+0000ba10: 7465 5f75 6470 5f73 6f63 6b65 7428 0a20  te_udp_socket(. 
+0000ba20: 2020 2020 2020 2020 2020 2066 616d 696c             famil
+0000ba30: 793d 4164 6472 6573 7346 616d 696c 792e  y=AddressFamily.
+0000ba40: 4146 5f49 4e45 542c 206c 6f63 616c 5f68  AF_INET, local_h
+0000ba50: 6f73 743d 226c 6f63 616c 686f 7374 220a  ost="localhost".
+0000ba60: 2020 2020 2020 2020 2920 6173 2075 6470          ) as udp
+0000ba70: 3a0a 2020 2020 2020 2020 2020 2020 6173  :.            as
+0000ba80: 796e 6320 7769 7468 2063 7265 6174 655f  ync with create_
+0000ba90: 7461 736b 5f67 726f 7570 2829 2061 7320  task_group() as 
+0000baa0: 7467 3a0a 2020 2020 2020 2020 2020 2020  tg:.            
+0000bab0: 2020 2020 7467 2e73 7461 7274 5f73 6f6f      tg.start_soo
+0000bac0: 6e28 636c 6f73 655f 7768 656e 5f62 6c6f  n(close_when_blo
+0000bad0: 636b 6564 290a 2020 2020 2020 2020 2020  cked).          
+0000bae0: 2020 2020 2020 7769 7468 2070 7974 6573        with pytes
+0000baf0: 742e 7261 6973 6573 2843 6c6f 7365 6452  t.raises(ClosedR
+0000bb00: 6573 6f75 7263 6545 7272 6f72 293a 0a20  esourceError):. 
+0000bb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb20: 2020 2061 7761 6974 2075 6470 2e72 6563     await udp.rec
+0000bb30: 6569 7665 2829 0a0a 2020 2020 6173 796e  eive()..    asyn
+0000bb40: 6320 6465 6620 7465 7374 5f72 6563 6569  c def test_recei
+0000bb50: 7665 5f61 6674 6572 5f63 6c6f 7365 2873  ve_after_close(s
+0000bb60: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+0000bb70: 2020 2020 2020 7564 7020 3d20 6177 6169        udp = awai
+0000bb80: 7420 6372 6561 7465 5f75 6470 5f73 6f63  t create_udp_soc
+0000bb90: 6b65 7428 0a20 2020 2020 2020 2020 2020  ket(.           
+0000bba0: 2066 616d 696c 793d 4164 6472 6573 7346   family=AddressF
+0000bbb0: 616d 696c 792e 4146 5f49 4e45 542c 206c  amily.AF_INET, l
+0000bbc0: 6f63 616c 5f68 6f73 743d 226c 6f63 616c  ocal_host="local
+0000bbd0: 686f 7374 220a 2020 2020 2020 2020 290a  host".        ).
+0000bbe0: 2020 2020 2020 2020 6177 6169 7420 7564          await ud
+0000bbf0: 702e 6163 6c6f 7365 2829 0a20 2020 2020  p.aclose().     
+0000bc00: 2020 2077 6974 6820 7079 7465 7374 2e72     with pytest.r
+0000bc10: 6169 7365 7328 436c 6f73 6564 5265 736f  aises(ClosedReso
+0000bc20: 7572 6365 4572 726f 7229 3a0a 2020 2020  urceError):.    
+0000bc30: 2020 2020 2020 2020 6177 6169 7420 7564          await ud
+0000bc40: 702e 7265 6365 6976 6528 290a 0a20 2020  p.receive()..   
+0000bc50: 2061 7379 6e63 2064 6566 2074 6573 745f   async def test_
+0000bc60: 7365 6e64 5f61 6674 6572 5f63 6c6f 7365  send_after_close
+0000bc70: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+0000bc80: 2020 2020 2020 2020 7564 7020 3d20 6177          udp = aw
+0000bc90: 6169 7420 6372 6561 7465 5f75 6470 5f73  ait create_udp_s
+0000bca0: 6f63 6b65 7428 0a20 2020 2020 2020 2020  ocket(.         
+0000bcb0: 2020 2066 616d 696c 793d 4164 6472 6573     family=Addres
+0000bcc0: 7346 616d 696c 792e 4146 5f49 4e45 542c  sFamily.AF_INET,
+0000bcd0: 206c 6f63 616c 5f68 6f73 743d 226c 6f63   local_host="loc
+0000bce0: 616c 686f 7374 220a 2020 2020 2020 2020  alhost".        
+0000bcf0: 290a 2020 2020 2020 2020 686f 7374 2c20  ).        host, 
+0000bd00: 706f 7274 203d 2075 6470 2e65 7874 7261  port = udp.extra
+0000bd10: 2853 6f63 6b65 7441 7474 7269 6275 7465  (SocketAttribute
+0000bd20: 2e6c 6f63 616c 5f61 6464 7265 7373 2920  .local_address) 
+0000bd30: 2023 2074 7970 653a 2069 676e 6f72 655b   # type: ignore[
+0000bd40: 6d69 7363 5d0a 2020 2020 2020 2020 6177  misc].        aw
+0000bd50: 6169 7420 7564 702e 6163 6c6f 7365 2829  ait udp.aclose()
+0000bd60: 0a20 2020 2020 2020 2077 6974 6820 7079  .        with py
+0000bd70: 7465 7374 2e72 6169 7365 7328 436c 6f73  test.raises(Clos
+0000bd80: 6564 5265 736f 7572 6365 4572 726f 7229  edResourceError)
+0000bd90: 3a0a 2020 2020 2020 2020 2020 2020 6177  :.            aw
+0000bda0: 6169 7420 7564 702e 7365 6e64 746f 2862  ait udp.sendto(b
+0000bdb0: 2266 6f6f 222c 2068 6f73 742c 2070 6f72  "foo", host, por
+0000bdc0: 7429 0a0a 2020 2020 6173 796e 6320 6465  t)..    async de
+0000bdd0: 6620 7465 7374 5f63 7265 6174 655f 756e  f test_create_un
+0000bde0: 626f 756e 645f 736f 636b 6574 2873 656c  bound_socket(sel
+0000bdf0: 662c 2066 616d 696c 793a 2041 6e79 4950  f, family: AnyIP
+0000be00: 4164 6472 6573 7346 616d 696c 7929 202d  AddressFamily) -
+0000be10: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000be20: 2222 2252 6567 7265 7373 696f 6e20 7465  """Regression te
+0000be30: 7374 2066 6f72 2023 3336 302e 2222 220a  st for #360.""".
+0000be40: 2020 2020 2020 2020 6173 796e 6320 7769          async wi
+0000be50: 7468 2061 7761 6974 2063 7265 6174 655f  th await create_
+0000be60: 7564 705f 736f 636b 6574 2866 616d 696c  udp_socket(famil
+0000be70: 793d 6661 6d69 6c79 2920 6173 2075 6470  y=family) as udp
+0000be80: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+0000be90: 6361 6c5f 6164 6472 6573 7320 3d20 6361  cal_address = ca
+0000bea0: 7374 280a 2020 2020 2020 2020 2020 2020  st(.            
+0000beb0: 2020 2020 4950 536f 636b 4164 6472 5479      IPSockAddrTy
+0000bec0: 7065 2c20 7564 702e 6578 7472 6128 536f  pe, udp.extra(So
+0000bed0: 636b 6574 4174 7472 6962 7574 652e 6c6f  cketAttribute.lo
+0000bee0: 6361 6c5f 6164 6472 6573 7329 0a20 2020  cal_address).   
+0000bef0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000bf00: 2020 2020 2020 2061 7373 6572 7420 6c6f         assert lo
+0000bf10: 6361 6c5f 6164 6472 6573 735b 315d 203e  cal_address[1] >
+0000bf20: 2030 0a0a 0a40 7079 7465 7374 2e6d 6172   0...@pytest.mar
+0000bf30: 6b2e 6e65 7477 6f72 6b0a 4070 7974 6573  k.network.@pytes
+0000bf40: 742e 6d61 726b 2e75 7365 6669 7874 7572  t.mark.usefixtur
+0000bf50: 6573 2822 6368 6563 6b5f 6173 796e 6369  es("check_asynci
+0000bf60: 6f5f 6275 6722 290a 636c 6173 7320 5465  o_bug").class Te
+0000bf70: 7374 436f 6e6e 6563 7465 6455 4450 536f  stConnectedUDPSo
+0000bf80: 636b 6574 3a0a 2020 2020 6173 796e 6320  cket:.    async 
+0000bf90: 6465 6620 7465 7374 5f65 7874 7261 5f61  def test_extra_a
+0000bfa0: 7474 7269 6275 7465 7328 7365 6c66 2c20  ttributes(self, 
+0000bfb0: 6661 6d69 6c79 3a20 416e 7949 5041 6464  family: AnyIPAdd
+0000bfc0: 7265 7373 4661 6d69 6c79 2920 2d3e 204e  ressFamily) -> N
+0000bfd0: 6f6e 653a 0a20 2020 2020 2020 2061 7379  one:.        asy
+0000bfe0: 6e63 2077 6974 6820 6177 6169 7420 6372  nc with await cr
+0000bff0: 6561 7465 5f63 6f6e 6e65 6374 6564 5f75  eate_connected_u
+0000c000: 6470 5f73 6f63 6b65 7428 0a20 2020 2020  dp_socket(.     
+0000c010: 2020 2020 2020 2022 6c6f 6361 6c68 6f73         "localhos
+0000c020: 7422 2c20 3530 3030 2c20 6661 6d69 6c79  t", 5000, family
+0000c030: 3d66 616d 696c 790a 2020 2020 2020 2020  =family.        
+0000c040: 2920 6173 2075 6470 3a0a 2020 2020 2020  ) as udp:.      
+0000c050: 2020 2020 2020 7261 775f 736f 636b 6574        raw_socket
+0000c060: 203d 2075 6470 2e65 7874 7261 2853 6f63   = udp.extra(Soc
+0000c070: 6b65 7441 7474 7269 6275 7465 2e72 6177  ketAttribute.raw
+0000c080: 5f73 6f63 6b65 7429 0a20 2020 2020 2020  _socket).       
+0000c090: 2020 2020 2061 7373 6572 7420 7564 702e       assert udp.
+0000c0a0: 6578 7472 6128 536f 636b 6574 4174 7472  extra(SocketAttr
+0000c0b0: 6962 7574 652e 6661 6d69 6c79 2920 3d3d  ibute.family) ==
+0000c0c0: 2066 616d 696c 790a 2020 2020 2020 2020   family.        
+0000c0d0: 2020 2020 6173 7365 7274 2028 0a20 2020      assert (.   
+0000c0e0: 2020 2020 2020 2020 2020 2020 2075 6470               udp
+0000c0f0: 2e65 7874 7261 2853 6f63 6b65 7441 7474  .extra(SocketAtt
+0000c100: 7269 6275 7465 2e6c 6f63 616c 5f61 6464  ribute.local_add
+0000c110: 7265 7373 2920 3d3d 2072 6177 5f73 6f63  ress) == raw_soc
+0000c120: 6b65 742e 6765 7473 6f63 6b6e 616d 6528  ket.getsockname(
+0000c130: 295b 3a32 5d0a 2020 2020 2020 2020 2020  )[:2].          
+0000c140: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000c150: 6173 7365 7274 2075 6470 2e65 7874 7261  assert udp.extra
+0000c160: 2853 6f63 6b65 7441 7474 7269 6275 7465  (SocketAttribute
+0000c170: 2e6c 6f63 616c 5f70 6f72 7429 203d 3d20  .local_port) == 
+0000c180: 7261 775f 736f 636b 6574 2e67 6574 736f  raw_socket.getso
+0000c190: 636b 6e61 6d65 2829 5b31 5d0a 2020 2020  ckname()[1].    
+0000c1a0: 2020 2020 2020 2020 6173 7365 7274 2028          assert (
+0000c1b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c1c0: 2075 6470 2e65 7874 7261 2853 6f63 6b65   udp.extra(Socke
+0000c1d0: 7441 7474 7269 6275 7465 2e72 656d 6f74  tAttribute.remot
+0000c1e0: 655f 6164 6472 6573 7329 0a20 2020 2020  e_address).     
+0000c1f0: 2020 2020 2020 2020 2020 203d 3d20 7261             == ra
+0000c200: 775f 736f 636b 6574 2e67 6574 7065 6572  w_socket.getpeer
+0000c210: 6e61 6d65 2829 5b3a 325d 0a20 2020 2020  name()[:2].     
+0000c220: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000c230: 2020 2020 2061 7373 6572 7420 7564 702e       assert udp.
+0000c240: 6578 7472 6128 536f 636b 6574 4174 7472  extra(SocketAttr
+0000c250: 6962 7574 652e 7265 6d6f 7465 5f70 6f72  ibute.remote_por
+0000c260: 7429 203d 3d20 3530 3030 0a0a 2020 2020  t) == 5000..    
+0000c270: 6173 796e 6320 6465 6620 7465 7374 5f73  async def test_s
+0000c280: 656e 645f 7265 6365 6976 6528 7365 6c66  end_receive(self
+0000c290: 2c20 6661 6d69 6c79 3a20 416e 7949 5041  , family: AnyIPA
+0000c2a0: 6464 7265 7373 4661 6d69 6c79 2920 2d3e  ddressFamily) ->
+0000c2b0: 204e 6f6e 653a 0a20 2020 2020 2020 2061   None:.        a
+0000c2c0: 7379 6e63 2077 6974 6820 6177 6169 7420  sync with await 
+0000c2d0: 6372 6561 7465 5f75 6470 5f73 6f63 6b65  create_udp_socke
+0000c2e0: 7428 0a20 2020 2020 2020 2020 2020 2066  t(.            f
+0000c2f0: 616d 696c 793d 6661 6d69 6c79 2c20 6c6f  amily=family, lo
+0000c300: 6361 6c5f 686f 7374 3d22 6c6f 6361 6c68  cal_host="localh
+0000c310: 6f73 7422 0a20 2020 2020 2020 2029 2061  ost".        ) a
+0000c320: 7320 7564 7031 3a0a 2020 2020 2020 2020  s udp1:.        
+0000c330: 2020 2020 686f 7374 2c20 706f 7274 203d      host, port =
+0000c340: 2075 6470 312e 6578 7472 6128 536f 636b   udp1.extra(Sock
+0000c350: 6574 4174 7472 6962 7574 652e 6c6f 6361  etAttribute.loca
+0000c360: 6c5f 6164 6472 6573 7329 2020 2320 7479  l_address)  # ty
+0000c370: 7065 3a20 6967 6e6f 7265 5b6d 6973 635d  pe: ignore[misc]
+0000c380: 0a20 2020 2020 2020 2020 2020 2061 7379  .            asy
+0000c390: 6e63 2077 6974 6820 6177 6169 7420 6372  nc with await cr
+0000c3a0: 6561 7465 5f63 6f6e 6e65 6374 6564 5f75  eate_connected_u
+0000c3b0: 6470 5f73 6f63 6b65 7428 0a20 2020 2020  dp_socket(.     
+0000c3c0: 2020 2020 2020 2020 2020 2068 6f73 742c             host,
+0000c3d0: 2070 6f72 742c 206c 6f63 616c 5f68 6f73   port, local_hos
+0000c3e0: 743d 226c 6f63 616c 686f 7374 222c 2066  t="localhost", f
+0000c3f0: 616d 696c 793d 6661 6d69 6c79 0a20 2020  amily=family.   
+0000c400: 2020 2020 2020 2020 2029 2061 7320 7564           ) as ud
+0000c410: 7032 3a0a 2020 2020 2020 2020 2020 2020  p2:.            
+0000c420: 2020 2020 686f 7374 2c20 706f 7274 203d      host, port =
+0000c430: 2075 6470 322e 6578 7472 6128 0a20 2020   udp2.extra(.   
+0000c440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c450: 2053 6f63 6b65 7441 7474 7269 6275 7465   SocketAttribute
+0000c460: 2e6c 6f63 616c 5f61 6464 7265 7373 2020  .local_address  
+0000c470: 2320 7479 7065 3a20 6967 6e6f 7265 5b6d  # type: ignore[m
+0000c480: 6973 635d 0a20 2020 2020 2020 2020 2020  isc].           
+0000c490: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000c4a0: 2020 2020 2020 2061 7761 6974 2075 6470         await udp
+0000c4b0: 322e 7365 6e64 2862 2262 6c61 6822 290a  2.send(b"blah").
+0000c4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c4d0: 7265 7175 6573 7420 3d20 6177 6169 7420  request = await 
+0000c4e0: 7564 7031 2e72 6563 6569 7665 2829 0a20  udp1.receive(). 
+0000c4f0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000c500: 7373 6572 7420 7265 7175 6573 7420 3d3d  ssert request ==
+0000c510: 2028 6222 626c 6168 222c 2028 686f 7374   (b"blah", (host
+0000c520: 2c20 706f 7274 2929 0a0a 2020 2020 2020  , port))..      
+0000c530: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+0000c540: 7564 7031 2e73 656e 6474 6f28 6222 6861  udp1.sendto(b"ha
+0000c550: 6c62 222c 2068 6f73 742c 2070 6f72 7429  lb", host, port)
+0000c560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c570: 2072 6573 706f 6e73 6520 3d20 6177 6169   response = awai
+0000c580: 7420 7564 7032 2e72 6563 6569 7665 2829  t udp2.receive()
+0000c590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c5a0: 2061 7373 6572 7420 7265 7370 6f6e 7365   assert response
+0000c5b0: 203d 3d20 6222 6861 6c62 220a 0a20 2020   == b"halb"..   
+0000c5c0: 2061 7379 6e63 2064 6566 2074 6573 745f   async def test_
+0000c5d0: 6974 6572 6174 6528 7365 6c66 2c20 6661  iterate(self, fa
+0000c5e0: 6d69 6c79 3a20 416e 7949 5041 6464 7265  mily: AnyIPAddre
+0000c5f0: 7373 4661 6d69 6c79 2920 2d3e 204e 6f6e  ssFamily) -> Non
+0000c600: 653a 0a20 2020 2020 2020 2061 7379 6e63  e:.        async
+0000c610: 2064 6566 2073 6572 7665 2829 202d 3e20   def serve() -> 
+0000c620: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000c630: 2020 6173 796e 6320 666f 7220 7061 636b    async for pack
+0000c640: 6574 2069 6e20 7564 7032 3a0a 2020 2020  et in udp2:.    
+0000c650: 2020 2020 2020 2020 2020 2020 6177 6169              awai
+0000c660: 7420 7564 7032 2e73 656e 6428 7061 636b  t udp2.send(pack
+0000c670: 6574 5b3a 3a2d 315d 290a 0a20 2020 2020  et[::-1])..     
+0000c680: 2020 2061 7379 6e63 2077 6974 6820 6177     async with aw
+0000c690: 6169 7420 6372 6561 7465 5f75 6470 5f73  ait create_udp_s
+0000c6a0: 6f63 6b65 7428 0a20 2020 2020 2020 2020  ocket(.         
+0000c6b0: 2020 2066 616d 696c 793d 6661 6d69 6c79     family=family
+0000c6c0: 2c20 6c6f 6361 6c5f 686f 7374 3d22 6c6f  , local_host="lo
+0000c6d0: 6361 6c68 6f73 7422 0a20 2020 2020 2020  calhost".       
+0000c6e0: 2029 2061 7320 7564 7031 3a0a 2020 2020   ) as udp1:.    
+0000c6f0: 2020 2020 2020 2020 686f 7374 2c20 706f          host, po
+0000c700: 7274 203d 2075 6470 312e 6578 7472 6128  rt = udp1.extra(
+0000c710: 536f 636b 6574 4174 7472 6962 7574 652e  SocketAttribute.
+0000c720: 6c6f 6361 6c5f 6164 6472 6573 7329 2020  local_address)  
+0000c730: 2320 7479 7065 3a20 6967 6e6f 7265 5b6d  # type: ignore[m
+0000c740: 6973 635d 0a20 2020 2020 2020 2020 2020  isc].           
+0000c750: 2061 7379 6e63 2077 6974 6820 6177 6169   async with awai
+0000c760: 7420 6372 6561 7465 5f63 6f6e 6e65 6374  t create_connect
+0000c770: 6564 5f75 6470 5f73 6f63 6b65 7428 686f  ed_udp_socket(ho
+0000c780: 7374 2c20 706f 7274 2920 6173 2075 6470  st, port) as udp
+0000c790: 323a 0a20 2020 2020 2020 2020 2020 2020  2:.             
+0000c7a0: 2020 2068 6f73 742c 2070 6f72 7420 3d20     host, port = 
+0000c7b0: 7564 7032 2e65 7874 7261 2820 2023 2074  udp2.extra(  # t
+0000c7c0: 7970 653a 2069 676e 6f72 655b 6d69 7363  ype: ignore[misc
+0000c7d0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000c7e0: 2020 2020 2020 536f 636b 6574 4174 7472        SocketAttr
+0000c7f0: 6962 7574 652e 6c6f 6361 6c5f 6164 6472  ibute.local_addr
+0000c800: 6573 730a 2020 2020 2020 2020 2020 2020  ess.            
+0000c810: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000c820: 2020 2020 2020 6173 796e 6320 7769 7468        async with
+0000c830: 2063 7265 6174 655f 7461 736b 5f67 726f   create_task_gro
+0000c840: 7570 2829 2061 7320 7467 3a0a 2020 2020  up() as tg:.    
+0000c850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c860: 7467 2e73 7461 7274 5f73 6f6f 6e28 7365  tg.start_soon(se
+0000c870: 7276 6529 0a20 2020 2020 2020 2020 2020  rve).           
+0000c880: 2020 2020 2020 2020 2061 7761 6974 2075           await u
+0000c890: 6470 312e 7365 6e64 746f 2862 2246 4f4f  dp1.sendto(b"FOO
+0000c8a0: 4241 5222 2c20 686f 7374 2c20 706f 7274  BAR", host, port
+0000c8b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000c8c0: 2020 2020 2020 6173 7365 7274 2061 7761        assert awa
+0000c8d0: 6974 2075 6470 312e 7265 6365 6976 6528  it udp1.receive(
+0000c8e0: 2920 3d3d 2028 6222 5241 424f 4f46 222c  ) == (b"RABOOF",
+0000c8f0: 2028 686f 7374 2c20 706f 7274 2929 0a20   (host, port)). 
+0000c900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c910: 2020 2061 7761 6974 2075 6470 312e 7365     await udp1.se
+0000c920: 6e64 746f 2862 2231 3233 3435 3622 2c20  ndto(b"123456", 
+0000c930: 686f 7374 2c20 706f 7274 290a 2020 2020  host, port).    
+0000c940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c950: 6173 7365 7274 2061 7761 6974 2075 6470  assert await udp
+0000c960: 312e 7265 6365 6976 6528 2920 3d3d 2028  1.receive() == (
+0000c970: 6222 3635 3433 3231 222c 2028 686f 7374  b"654321", (host
+0000c980: 2c20 706f 7274 2929 0a20 2020 2020 2020  , port)).       
+0000c990: 2020 2020 2020 2020 2020 2020 2074 672e               tg.
+0000c9a0: 6361 6e63 656c 5f73 636f 7065 2e63 616e  cancel_scope.can
+0000c9b0: 6365 6c28 290a 0a20 2020 2040 7079 7465  cel()..    @pyte
+0000c9c0: 7374 2e6d 6172 6b2e 736b 6970 6966 280a  st.mark.skipif(.
+0000c9d0: 2020 2020 2020 2020 6e6f 7420 6861 7361          not hasa
+0000c9e0: 7474 7228 736f 636b 6574 2c20 2253 4f5f  ttr(socket, "SO_
+0000c9f0: 5245 5553 4550 4f52 5422 292c 2072 6561  REUSEPORT"), rea
+0000ca00: 736f 6e3d 2253 4f5f 5245 5553 4550 4f52  son="SO_REUSEPOR
+0000ca10: 5420 6f70 7469 6f6e 206e 6f74 2073 7570  T option not sup
+0000ca20: 706f 7274 6564 220a 2020 2020 290a 2020  ported".    ).  
+0000ca30: 2020 6173 796e 6320 6465 6620 7465 7374    async def test
+0000ca40: 5f72 6575 7365 5f70 6f72 7428 7365 6c66  _reuse_port(self
+0000ca50: 2c20 6661 6d69 6c79 3a20 416e 7949 5041  , family: AnyIPA
+0000ca60: 6464 7265 7373 4661 6d69 6c79 2920 2d3e  ddressFamily) ->
+0000ca70: 204e 6f6e 653a 0a20 2020 2020 2020 2061   None:.        a
+0000ca80: 7379 6e63 2077 6974 6820 6177 6169 7420  sync with await 
+0000ca90: 6372 6561 7465 5f63 6f6e 6e65 6374 6564  create_connected
+0000caa0: 5f75 6470 5f73 6f63 6b65 7428 0a20 2020  _udp_socket(.   
+0000cab0: 2020 2020 2020 2020 2022 6c6f 6361 6c68           "localh
+0000cac0: 6f73 7422 2c20 3630 3030 2c20 6661 6d69  ost", 6000, fami
+0000cad0: 6c79 3d66 616d 696c 792c 206c 6f63 616c  ly=family, local
+0000cae0: 5f68 6f73 743d 226c 6f63 616c 686f 7374  _host="localhost
+0000caf0: 222c 2072 6575 7365 5f70 6f72 743d 5472  ", reuse_port=Tr
+0000cb00: 7565 0a20 2020 2020 2020 2029 2061 7320  ue.        ) as 
+0000cb10: 7564 703a 0a20 2020 2020 2020 2020 2020  udp:.           
+0000cb20: 2070 6f72 7420 3d20 7564 702e 6578 7472   port = udp.extr
+0000cb30: 6128 536f 636b 6574 4174 7472 6962 7574  a(SocketAttribut
+0000cb40: 652e 6c6f 6361 6c5f 706f 7274 290a 2020  e.local_port).  
+0000cb50: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+0000cb60: 2070 6f72 7420 213d 2030 0a20 2020 2020   port != 0.     
+0000cb70: 2020 2020 2020 2061 7379 6e63 2077 6974         async wit
+0000cb80: 6820 6177 6169 7420 6372 6561 7465 5f63  h await create_c
+0000cb90: 6f6e 6e65 6374 6564 5f75 6470 5f73 6f63  onnected_udp_soc
+0000cba0: 6b65 7428 0a20 2020 2020 2020 2020 2020  ket(.           
+0000cbb0: 2020 2020 2022 6c6f 6361 6c68 6f73 7422       "localhost"
+0000cbc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000cbd0: 2020 3630 3031 2c0a 2020 2020 2020 2020    6001,.        
+0000cbe0: 2020 2020 2020 2020 6661 6d69 6c79 3d66          family=f
+0000cbf0: 616d 696c 792c 0a20 2020 2020 2020 2020  amily,.         
+0000cc00: 2020 2020 2020 206c 6f63 616c 5f68 6f73         local_hos
+0000cc10: 743d 226c 6f63 616c 686f 7374 222c 0a20  t="localhost",. 
+0000cc20: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000cc30: 6f63 616c 5f70 6f72 743d 706f 7274 2c0a  ocal_port=port,.
+0000cc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc50: 7265 7573 655f 706f 7274 3d54 7275 652c  reuse_port=True,
+0000cc60: 0a20 2020 2020 2020 2020 2020 2029 2061  .            ) a
+0000cc70: 7320 7564 7032 3a0a 2020 2020 2020 2020  s udp2:.        
+0000cc80: 2020 2020 2020 2020 6173 7365 7274 2070          assert p
+0000cc90: 6f72 7420 3d3d 2075 6470 322e 6578 7472  ort == udp2.extr
+0000cca0: 6128 536f 636b 6574 4174 7472 6962 7574  a(SocketAttribut
+0000ccb0: 652e 6c6f 6361 6c5f 706f 7274 290a 0a20  e.local_port).. 
+0000ccc0: 2020 2061 7379 6e63 2064 6566 2074 6573     async def tes
+0000ccd0: 745f 636f 6e63 7572 7265 6e74 5f72 6563  t_concurrent_rec
+0000cce0: 6569 7665 2873 656c 6629 202d 3e20 4e6f  eive(self) -> No
+0000ccf0: 6e65 3a0a 2020 2020 2020 2020 6173 796e  ne:.        asyn
+0000cd00: 6320 7769 7468 2061 7761 6974 2063 7265  c with await cre
+0000cd10: 6174 655f 636f 6e6e 6563 7465 645f 7564  ate_connected_ud
+0000cd20: 705f 736f 636b 6574 280a 2020 2020 2020  p_socket(.      
+0000cd30: 2020 2020 2020 226c 6f63 616c 686f 7374        "localhost
+0000cd40: 222c 2035 3030 302c 206c 6f63 616c 5f68  ", 5000, local_h
+0000cd50: 6f73 743d 226c 6f63 616c 686f 7374 222c  ost="localhost",
+0000cd60: 2066 616d 696c 793d 4164 6472 6573 7346   family=AddressF
+0000cd70: 616d 696c 792e 4146 5f49 4e45 540a 2020  amily.AF_INET.  
+0000cd80: 2020 2020 2020 2920 6173 2075 6470 3a0a        ) as udp:.
+0000cd90: 2020 2020 2020 2020 2020 2020 6173 796e              asyn
+0000cda0: 6320 7769 7468 2063 7265 6174 655f 7461  c with create_ta
+0000cdb0: 736b 5f67 726f 7570 2829 2061 7320 7467  sk_group() as tg
+0000cdc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000cdd0: 2020 7467 2e73 7461 7274 5f73 6f6f 6e28    tg.start_soon(
+0000cde0: 7564 702e 7265 6365 6976 6529 0a20 2020  udp.receive).   
+0000cdf0: 2020 2020 2020 2020 2020 2020 2061 7761               awa
+0000ce00: 6974 2077 6169 745f 616c 6c5f 7461 736b  it wait_all_task
+0000ce10: 735f 626c 6f63 6b65 6428 290a 2020 2020  s_blocked().    
+0000ce20: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+0000ce30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ce40: 2020 2020 2077 6974 6820 7079 7465 7374       with pytest
+0000ce50: 2e72 6169 7365 7328 4275 7379 5265 736f  .raises(BusyReso
+0000ce60: 7572 6365 4572 726f 7229 2061 7320 6578  urceError) as ex
+0000ce70: 633a 0a20 2020 2020 2020 2020 2020 2020  c:.             
+0000ce80: 2020 2020 2020 2020 2020 2061 7761 6974             await
+0000ce90: 2075 6470 2e72 6563 6569 7665 2829 0a0a   udp.receive()..
+0000cea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ceb0: 2020 2020 6578 632e 6d61 7463 6828 2261      exc.match("a
+0000cec0: 6c72 6561 6479 2072 6561 6469 6e67 2066  lready reading f
+0000ced0: 726f 6d22 290a 2020 2020 2020 2020 2020  rom").          
+0000cee0: 2020 2020 2020 6669 6e61 6c6c 793a 0a20        finally:. 
+0000cef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf00: 2020 2074 672e 6361 6e63 656c 5f73 636f     tg.cancel_sco
+0000cf10: 7065 2e63 616e 6365 6c28 290a 0a20 2020  pe.cancel()..   
+0000cf20: 2061 7379 6e63 2064 6566 2074 6573 745f   async def test_
+0000cf30: 636c 6f73 655f 6475 7269 6e67 5f72 6563  close_during_rec
+0000cf40: 6569 7665 2873 656c 6629 202d 3e20 4e6f  eive(self) -> No
+0000cf50: 6e65 3a0a 2020 2020 2020 2020 6173 796e  ne:.        asyn
+0000cf60: 6320 6465 6620 636c 6f73 655f 7768 656e  c def close_when
+0000cf70: 5f62 6c6f 636b 6564 2829 202d 3e20 4e6f  _blocked() -> No
+0000cf80: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000cf90: 6177 6169 7420 7761 6974 5f61 6c6c 5f74  await wait_all_t
+0000cfa0: 6173 6b73 5f62 6c6f 636b 6564 2829 0a20  asks_blocked(). 
+0000cfb0: 2020 2020 2020 2020 2020 2061 7761 6974             await
+0000cfc0: 2075 6470 2e61 636c 6f73 6528 290a 0a20   udp.aclose().. 
+0000cfd0: 2020 2020 2020 2061 7379 6e63 2077 6974         async wit
+0000cfe0: 6820 6177 6169 7420 6372 6561 7465 5f63  h await create_c
+0000cff0: 6f6e 6e65 6374 6564 5f75 6470 5f73 6f63  onnected_udp_soc
+0000d000: 6b65 7428 0a20 2020 2020 2020 2020 2020  ket(.           
+0000d010: 2022 6c6f 6361 6c68 6f73 7422 2c20 3530   "localhost", 50
+0000d020: 3030 2c20 6c6f 6361 6c5f 686f 7374 3d22  00, local_host="
+0000d030: 6c6f 6361 6c68 6f73 7422 2c20 6661 6d69  localhost", fami
+0000d040: 6c79 3d41 6464 7265 7373 4661 6d69 6c79  ly=AddressFamily
+0000d050: 2e41 465f 494e 4554 0a20 2020 2020 2020  .AF_INET.       
+0000d060: 2029 2061 7320 7564 703a 0a20 2020 2020   ) as udp:.     
+0000d070: 2020 2020 2020 2061 7379 6e63 2077 6974         async wit
+0000d080: 6820 6372 6561 7465 5f74 6173 6b5f 6772  h create_task_gr
+0000d090: 6f75 7028 2920 6173 2074 673a 0a20 2020  oup() as tg:.   
+0000d0a0: 2020 2020 2020 2020 2020 2020 2074 672e               tg.
+0000d0b0: 7374 6172 745f 736f 6f6e 2863 6c6f 7365  start_soon(close
+0000d0c0: 5f77 6865 6e5f 626c 6f63 6b65 6429 0a20  _when_blocked). 
+0000d0d0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+0000d0e0: 6974 6820 7079 7465 7374 2e72 6169 7365  ith pytest.raise
+0000d0f0: 7328 436c 6f73 6564 5265 736f 7572 6365  s(ClosedResource
+0000d100: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
+0000d110: 2020 2020 2020 2020 2020 2020 6177 6169              awai
+0000d120: 7420 7564 702e 7265 6365 6976 6528 290a  t udp.receive().
+0000d130: 0a20 2020 2061 7379 6e63 2064 6566 2074  .    async def t
+0000d140: 6573 745f 7265 6365 6976 655f 6166 7465  est_receive_afte
+0000d150: 725f 636c 6f73 6528 7365 6c66 2c20 6661  r_close(self, fa
+0000d160: 6d69 6c79 3a20 416e 7949 5041 6464 7265  mily: AnyIPAddre
+0000d170: 7373 4661 6d69 6c79 2920 2d3e 204e 6f6e  ssFamily) -> Non
+0000d180: 653a 0a20 2020 2020 2020 2075 6470 203d  e:.        udp =
+0000d190: 2061 7761 6974 2063 7265 6174 655f 636f   await create_co
+0000d1a0: 6e6e 6563 7465 645f 7564 705f 736f 636b  nnected_udp_sock
+0000d1b0: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
+0000d1c0: 226c 6f63 616c 686f 7374 222c 2035 3030  "localhost", 500
+0000d1d0: 302c 206c 6f63 616c 5f68 6f73 743d 226c  0, local_host="l
+0000d1e0: 6f63 616c 686f 7374 222c 2066 616d 696c  ocalhost", famil
+0000d1f0: 793d 6661 6d69 6c79 0a20 2020 2020 2020  y=family.       
+0000d200: 2029 0a20 2020 2020 2020 2061 7761 6974   ).        await
+0000d210: 2075 6470 2e61 636c 6f73 6528 290a 2020   udp.aclose().  
+0000d220: 2020 2020 2020 7769 7468 2070 7974 6573        with pytes
+0000d230: 742e 7261 6973 6573 2843 6c6f 7365 6452  t.raises(ClosedR
+0000d240: 6573 6f75 7263 6545 7272 6f72 293a 0a20  esourceError):. 
+0000d250: 2020 2020 2020 2020 2020 2061 7761 6974             await
+0000d260: 2075 6470 2e72 6563 6569 7665 2829 0a0a   udp.receive()..
+0000d270: 2020 2020 6173 796e 6320 6465 6620 7465      async def te
+0000d280: 7374 5f73 656e 645f 6166 7465 725f 636c  st_send_after_cl
+0000d290: 6f73 6528 7365 6c66 2c20 6661 6d69 6c79  ose(self, family
+0000d2a0: 3a20 416e 7949 5041 6464 7265 7373 4661  : AnyIPAddressFa
+0000d2b0: 6d69 6c79 2920 2d3e 204e 6f6e 653a 0a20  mily) -> None:. 
+0000d2c0: 2020 2020 2020 2075 6470 203d 2061 7761         udp = awa
+0000d2d0: 6974 2063 7265 6174 655f 636f 6e6e 6563  it create_connec
+0000d2e0: 7465 645f 7564 705f 736f 636b 6574 280a  ted_udp_socket(.
+0000d2f0: 2020 2020 2020 2020 2020 2020 226c 6f63              "loc
+0000d300: 616c 686f 7374 222c 2035 3030 302c 206c  alhost", 5000, l
+0000d310: 6f63 616c 5f68 6f73 743d 226c 6f63 616c  ocal_host="local
+0000d320: 686f 7374 222c 2066 616d 696c 793d 6661  host", family=fa
+0000d330: 6d69 6c79 0a20 2020 2020 2020 2029 0a20  mily.        ). 
+0000d340: 2020 2020 2020 2061 7761 6974 2075 6470         await udp
+0000d350: 2e61 636c 6f73 6528 290a 2020 2020 2020  .aclose().      
+0000d360: 2020 7769 7468 2070 7974 6573 742e 7261    with pytest.ra
+0000d370: 6973 6573 2843 6c6f 7365 6452 6573 6f75  ises(ClosedResou
+0000d380: 7263 6545 7272 6f72 293a 0a20 2020 2020  rceError):.     
+0000d390: 2020 2020 2020 2061 7761 6974 2075 6470         await udp
+0000d3a0: 2e73 656e 6428 6222 666f 6f22 290a 0a0a  .send(b"foo")...
+0000d3b0: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
+0000d3c0: 7069 6628 0a20 2020 2073 7973 2e70 6c61  pif(.    sys.pla
+0000d3d0: 7466 6f72 6d20 3d3d 2022 7769 6e33 3222  tform == "win32"
+0000d3e0: 2c20 7265 6173 6f6e 3d22 554e 4958 2073  , reason="UNIX s
+0000d3f0: 6f63 6b65 7473 2061 7265 206e 6f74 2061  ockets are not a
+0000d400: 7661 696c 6162 6c65 206f 6e20 5769 6e64  vailable on Wind
+0000d410: 6f77 7322 0a29 0a63 6c61 7373 2054 6573  ows".).class Tes
+0000d420: 7455 4e49 5844 6174 6167 7261 6d53 6f63  tUNIXDatagramSoc
+0000d430: 6b65 743a 0a20 2020 2040 7079 7465 7374  ket:.    @pytest
+0000d440: 2e66 6978 7475 7265 0a20 2020 2064 6566  .fixture.    def
+0000d450: 2073 6f63 6b65 745f 7061 7468 2873 656c   socket_path(sel
+0000d460: 6629 202d 3e20 4765 6e65 7261 746f 725b  f) -> Generator[
+0000d470: 5061 7468 2c20 4e6f 6e65 2c20 4e6f 6e65  Path, None, None
+0000d480: 5d3a 0a20 2020 2020 2020 2023 2055 7365  ]:.        # Use
+0000d490: 2073 7464 6c69 6220 7465 6d70 6469 7220   stdlib tempdir 
+0000d4a0: 6765 6e65 7261 7469 6f6e 0a20 2020 2020  generation.     
+0000d4b0: 2020 2023 2046 6978 6573 2060 4f53 4572     # Fixes `OSEr
+0000d4c0: 726f 723a 2041 465f 554e 4958 2070 6174  ror: AF_UNIX pat
+0000d4d0: 6820 746f 6f20 6c6f 6e67 6020 6672 6f6d  h too long` from
+0000d4e0: 2070 7974 6573 7420 6765 6e65 7261 7465   pytest generate
+0000d4f0: 6420 7465 6d70 5f70 6174 680a 2020 2020  d temp_path.    
+0000d500: 2020 2020 7769 7468 2074 656d 7066 696c      with tempfil
+0000d510: 652e 5465 6d70 6f72 6172 7944 6972 6563  e.TemporaryDirec
+0000d520: 746f 7279 2829 2061 7320 7061 7468 3a0a  tory() as path:.
+0000d530: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
+0000d540: 6420 5061 7468 2870 6174 6829 202f 2022  d Path(path) / "
+0000d550: 736f 636b 6574 220a 0a20 2020 2040 7079  socket"..    @py
+0000d560: 7465 7374 2e66 6978 7475 7265 2870 6172  test.fixture(par
+0000d570: 616d 733d 5b46 616c 7365 2c20 5472 7565  ams=[False, True
+0000d580: 5d2c 2069 6473 3d5b 2273 7472 222c 2022  ], ids=["str", "
+0000d590: 7061 7468 225d 290a 2020 2020 6465 6620  path"]).    def 
+0000d5a0: 736f 636b 6574 5f70 6174 685f 6f72 5f73  socket_path_or_s
+0000d5b0: 7472 2873 656c 662c 2072 6571 7565 7374  tr(self, request
+0000d5c0: 3a20 5375 6252 6571 7565 7374 2c20 736f  : SubRequest, so
+0000d5d0: 636b 6574 5f70 6174 683a 2050 6174 6829  cket_path: Path)
+0000d5e0: 202d 3e20 5061 7468 207c 2073 7472 3a0a   -> Path | str:.
+0000d5f0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000d600: 6f63 6b65 745f 7061 7468 2069 6620 7265  ocket_path if re
+0000d610: 7175 6573 742e 7061 7261 6d20 656c 7365  quest.param else
+0000d620: 2073 7472 2873 6f63 6b65 745f 7061 7468   str(socket_path
+0000d630: 290a 0a20 2020 2040 7079 7465 7374 2e66  )..    @pytest.f
+0000d640: 6978 7475 7265 0a20 2020 2064 6566 2070  ixture.    def p
+0000d650: 6565 725f 736f 636b 6574 5f70 6174 6828  eer_socket_path(
+0000d660: 7365 6c66 2920 2d3e 2047 656e 6572 6174  self) -> Generat
+0000d670: 6f72 5b50 6174 682c 204e 6f6e 652c 204e  or[Path, None, N
+0000d680: 6f6e 655d 3a0a 2020 2020 2020 2020 2320  one]:.        # 
+0000d690: 5573 6520 7374 646c 6962 2074 656d 7064  Use stdlib tempd
+0000d6a0: 6972 2067 656e 6572 6174 696f 6e0a 2020  ir generation.  
+0000d6b0: 2020 2020 2020 2320 4669 7865 7320 604f        # Fixes `O
+0000d6c0: 5345 7272 6f72 3a20 4146 5f55 4e49 5820  SError: AF_UNIX 
+0000d6d0: 7061 7468 2074 6f6f 206c 6f6e 6760 2066  path too long` f
+0000d6e0: 726f 6d20 7079 7465 7374 2067 656e 6572  rom pytest gener
+0000d6f0: 6174 6564 2074 656d 705f 7061 7468 0a20  ated temp_path. 
+0000d700: 2020 2020 2020 2077 6974 6820 7465 6d70         with temp
+0000d710: 6669 6c65 2e54 656d 706f 7261 7279 4469  file.TemporaryDi
+0000d720: 7265 6374 6f72 7928 2920 6173 2070 6174  rectory() as pat
+0000d730: 683a 0a20 2020 2020 2020 2020 2020 2079  h:.            y
+0000d740: 6965 6c64 2050 6174 6828 7061 7468 2920  ield Path(path) 
+0000d750: 2f20 2270 6565 725f 736f 636b 6574 220a  / "peer_socket".
+0000d760: 0a20 2020 2061 7379 6e63 2064 6566 2074  .    async def t
+0000d770: 6573 745f 6578 7472 615f 6174 7472 6962  est_extra_attrib
+0000d780: 7574 6573 2873 656c 662c 2073 6f63 6b65  utes(self, socke
+0000d790: 745f 7061 7468 3a20 5061 7468 2920 2d3e  t_path: Path) ->
+0000d7a0: 204e 6f6e 653a 0a20 2020 2020 2020 2061   None:.        a
+0000d7b0: 7379 6e63 2077 6974 6820 6177 6169 7420  sync with await 
+0000d7c0: 6372 6561 7465 5f75 6e69 785f 6461 7461  create_unix_data
+0000d7d0: 6772 616d 5f73 6f63 6b65 7428 6c6f 6361  gram_socket(loca
+0000d7e0: 6c5f 7061 7468 3d73 6f63 6b65 745f 7061  l_path=socket_pa
+0000d7f0: 7468 2920 6173 2075 6e69 785f 6467 3a0a  th) as unix_dg:.
+0000d800: 2020 2020 2020 2020 2020 2020 7261 775f              raw_
+0000d810: 736f 636b 6574 203d 2075 6e69 785f 6467  socket = unix_dg
+0000d820: 2e65 7874 7261 2853 6f63 6b65 7441 7474  .extra(SocketAtt
+0000d830: 7269 6275 7465 2e72 6177 5f73 6f63 6b65  ribute.raw_socke
+0000d840: 7429 0a20 2020 2020 2020 2020 2020 2061  t).            a
+0000d850: 7373 6572 7420 7261 775f 736f 636b 6574  ssert raw_socket
+0000d860: 2e67 6574 7469 6d65 6f75 7428 2920 3d3d  .gettimeout() ==
+0000d870: 2030 0a20 2020 2020 2020 2020 2020 2061   0.            a
+0000d880: 7373 6572 7420 756e 6978 5f64 672e 6578  ssert unix_dg.ex
+0000d890: 7472 6128 536f 636b 6574 4174 7472 6962  tra(SocketAttrib
+0000d8a0: 7574 652e 6661 6d69 6c79 2920 3d3d 2073  ute.family) == s
+0000d8b0: 6f63 6b65 742e 4146 5f55 4e49 580a 2020  ocket.AF_UNIX.  
+0000d8c0: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+0000d8d0: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+0000d8e0: 2020 2075 6e69 785f 6467 2e65 7874 7261     unix_dg.extra
+0000d8f0: 2853 6f63 6b65 7441 7474 7269 6275 7465  (SocketAttribute
+0000d900: 2e6c 6f63 616c 5f61 6464 7265 7373 2920  .local_address) 
+0000d910: 3d3d 2072 6177 5f73 6f63 6b65 742e 6765  == raw_socket.ge
+0000d920: 7473 6f63 6b6e 616d 6528 290a 2020 2020  tsockname().    
+0000d930: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000d940: 2020 2020 2020 7079 7465 7374 2e72 6169        pytest.rai
+0000d950: 7365 7328 0a20 2020 2020 2020 2020 2020  ses(.           
+0000d960: 2020 2020 2054 7970 6564 4174 7472 6962       TypedAttrib
+0000d970: 7574 654c 6f6f 6b75 7045 7272 6f72 2c20  uteLookupError, 
+0000d980: 756e 6978 5f64 672e 6578 7472 612c 2053  unix_dg.extra, S
+0000d990: 6f63 6b65 7441 7474 7269 6275 7465 2e6c  ocketAttribute.l
+0000d9a0: 6f63 616c 5f70 6f72 740a 2020 2020 2020  ocal_port.      
+0000d9b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000d9c0: 2020 2020 7079 7465 7374 2e72 6169 7365      pytest.raise
+0000d9d0: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
+0000d9e0: 2020 2054 7970 6564 4174 7472 6962 7574     TypedAttribut
+0000d9f0: 654c 6f6f 6b75 7045 7272 6f72 2c20 756e  eLookupError, un
+0000da00: 6978 5f64 672e 6578 7472 612c 2053 6f63  ix_dg.extra, Soc
+0000da10: 6b65 7441 7474 7269 6275 7465 2e72 656d  ketAttribute.rem
+0000da20: 6f74 655f 6164 6472 6573 730a 2020 2020  ote_address.    
+0000da30: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000da40: 2020 2020 2020 7079 7465 7374 2e72 6169        pytest.rai
+0000da50: 7365 7328 0a20 2020 2020 2020 2020 2020  ses(.           
+0000da60: 2020 2020 2054 7970 6564 4174 7472 6962       TypedAttrib
+0000da70: 7574 654c 6f6f 6b75 7045 7272 6f72 2c20  uteLookupError, 
+0000da80: 756e 6978 5f64 672e 6578 7472 612c 2053  unix_dg.extra, S
+0000da90: 6f63 6b65 7441 7474 7269 6275 7465 2e72  ocketAttribute.r
+0000daa0: 656d 6f74 655f 706f 7274 0a20 2020 2020  emote_port.     
+0000dab0: 2020 2020 2020 2029 0a0a 2020 2020 6173         )..    as
+0000dac0: 796e 6320 6465 6620 7465 7374 5f73 656e  ync def test_sen
+0000dad0: 645f 7265 6365 6976 6528 7365 6c66 2c20  d_receive(self, 
+0000dae0: 736f 636b 6574 5f70 6174 685f 6f72 5f73  socket_path_or_s
+0000daf0: 7472 3a20 5061 7468 207c 2073 7472 2920  tr: Path | str) 
+0000db00: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0000db10: 2061 7379 6e63 2077 6974 6820 6177 6169   async with awai
+0000db20: 7420 6372 6561 7465 5f75 6e69 785f 6461  t create_unix_da
+0000db30: 7461 6772 616d 5f73 6f63 6b65 7428 0a20  tagram_socket(. 
+0000db40: 2020 2020 2020 2020 2020 206c 6f63 616c             local
+0000db50: 5f70 6174 683d 736f 636b 6574 5f70 6174  _path=socket_pat
+0000db60: 685f 6f72 5f73 7472 2c0a 2020 2020 2020  h_or_str,.      
+0000db70: 2020 2920 6173 2073 6f63 6b3a 0a20 2020    ) as sock:.   
+0000db80: 2020 2020 2020 2020 2070 6174 6820 3d20           path = 
+0000db90: 7374 7228 736f 636b 6574 5f70 6174 685f  str(socket_path_
+0000dba0: 6f72 5f73 7472 290a 0a20 2020 2020 2020  or_str)..       
+0000dbb0: 2020 2020 2061 7761 6974 2073 6f63 6b2e       await sock.
+0000dbc0: 7365 6e64 746f 2862 2262 6c61 6822 2c20  sendto(b"blah", 
+0000dbd0: 7061 7468 290a 2020 2020 2020 2020 2020  path).          
+0000dbe0: 2020 7265 7175 6573 742c 2061 6464 7220    request, addr 
+0000dbf0: 3d20 6177 6169 7420 736f 636b 2e72 6563  = await sock.rec
+0000dc00: 6569 7665 2829 0a20 2020 2020 2020 2020  eive().         
+0000dc10: 2020 2061 7373 6572 7420 7265 7175 6573     assert reques
+0000dc20: 7420 3d3d 2062 2262 6c61 6822 0a20 2020  t == b"blah".   
+0000dc30: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+0000dc40: 6164 6472 203d 3d20 7061 7468 0a0a 2020  addr == path..  
+0000dc50: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+0000dc60: 736f 636b 2e73 656e 6474 6f28 6222 6861  sock.sendto(b"ha
+0000dc70: 6c62 222c 2070 6174 6829 0a20 2020 2020  lb", path).     
+0000dc80: 2020 2020 2020 2072 6573 706f 6e73 652c         response,
+0000dc90: 2061 6464 7220 3d20 6177 6169 7420 736f   addr = await so
+0000dca0: 636b 2e72 6563 6569 7665 2829 0a20 2020  ck.receive().   
+0000dcb0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+0000dcc0: 7265 7370 6f6e 7365 203d 3d20 6222 6861  response == b"ha
+0000dcd0: 6c62 220a 2020 2020 2020 2020 2020 2020  lb".            
+0000dce0: 6173 7365 7274 2061 6464 7220 3d3d 2070  assert addr == p
+0000dcf0: 6174 680a 0a20 2020 2061 7379 6e63 2064  ath..    async d
+0000dd00: 6566 2074 6573 745f 6974 6572 6174 6528  ef test_iterate(
+0000dd10: 7365 6c66 2c20 7065 6572 5f73 6f63 6b65  self, peer_socke
+0000dd20: 745f 7061 7468 3a20 5061 7468 2c20 736f  t_path: Path, so
+0000dd30: 636b 6574 5f70 6174 683a 2050 6174 6829  cket_path: Path)
+0000dd40: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+0000dd50: 2020 6173 796e 6320 6465 6620 7365 7276    async def serv
+0000dd60: 6528 2920 2d3e 204e 6f6e 653a 0a20 2020  e() -> None:.   
+0000dd70: 2020 2020 2020 2020 2061 7379 6e63 2066           async f
+0000dd80: 6f72 2070 6163 6b65 742c 2061 6464 7220  or packet, addr 
+0000dd90: 696e 2073 6572 7665 723a 0a20 2020 2020  in server:.     
+0000dda0: 2020 2020 2020 2020 2020 2061 7761 6974             await
+0000ddb0: 2073 6572 7665 722e 7365 6e64 2828 7061   server.send((pa
+0000ddc0: 636b 6574 5b3a 3a2d 315d 2c20 6164 6472  cket[::-1], addr
+0000ddd0: 2929 0a0a 2020 2020 2020 2020 6173 796e  ))..        asyn
+0000dde0: 6320 7769 7468 2061 7761 6974 2063 7265  c with await cre
+0000ddf0: 6174 655f 756e 6978 5f64 6174 6167 7261  ate_unix_datagra
+0000de00: 6d5f 736f 636b 6574 280a 2020 2020 2020  m_socket(.      
+0000de10: 2020 2020 2020 6c6f 6361 6c5f 7061 7468        local_path
+0000de20: 3d70 6565 725f 736f 636b 6574 5f70 6174  =peer_socket_pat
+0000de30: 682c 0a20 2020 2020 2020 2029 2061 7320  h,.        ) as 
+0000de40: 7365 7276 6572 3a0a 2020 2020 2020 2020  server:.        
+0000de50: 2020 2020 7065 6572 5f70 6174 6820 3d20      peer_path = 
+0000de60: 7374 7228 7065 6572 5f73 6f63 6b65 745f  str(peer_socket_
+0000de70: 7061 7468 290a 2020 2020 2020 2020 2020  path).          
+0000de80: 2020 6173 796e 6320 7769 7468 2061 7761    async with awa
+0000de90: 6974 2063 7265 6174 655f 756e 6978 5f64  it create_unix_d
+0000dea0: 6174 6167 7261 6d5f 736f 636b 6574 280a  atagram_socket(.
+0000deb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dec0: 6c6f 6361 6c5f 7061 7468 3d73 6f63 6b65  local_path=socke
+0000ded0: 745f 7061 7468 0a20 2020 2020 2020 2020  t_path.         
+0000dee0: 2020 2029 2061 7320 636c 6965 6e74 3a0a     ) as client:.
+0000def0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df00: 6173 796e 6320 7769 7468 2063 7265 6174  async with creat
+0000df10: 655f 7461 736b 5f67 726f 7570 2829 2061  e_task_group() a
+0000df20: 7320 7467 3a0a 2020 2020 2020 2020 2020  s tg:.          
+0000df30: 2020 2020 2020 2020 2020 7467 2e73 7461            tg.sta
+0000df40: 7274 5f73 6f6f 6e28 7365 7276 6529 0a20  rt_soon(serve). 
+0000df50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df60: 2020 2061 7761 6974 2063 6c69 656e 742e     await client.
+0000df70: 7365 6e64 746f 2862 2246 4f4f 4241 5222  sendto(b"FOOBAR"
+0000df80: 2c20 7065 6572 5f70 6174 6829 0a20 2020  , peer_path).   
+0000df90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dfa0: 2061 7373 6572 7420 6177 6169 7420 636c   assert await cl
+0000dfb0: 6965 6e74 2e72 6563 6569 7665 2829 203d  ient.receive() =
+0000dfc0: 3d20 2862 2252 4142 4f4f 4622 2c20 7065  = (b"RABOOF", pe
+0000dfd0: 6572 5f70 6174 6829 0a20 2020 2020 2020  er_path).       
+0000dfe0: 2020 2020 2020 2020 2020 2020 2061 7761               awa
+0000dff0: 6974 2063 6c69 656e 742e 7365 6e64 746f  it client.sendto
+0000e000: 2862 2231 3233 3435 3622 2c20 7065 6572  (b"123456", peer
+0000e010: 5f70 6174 6829 0a20 2020 2020 2020 2020  _path).         
+0000e020: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+0000e030: 7420 6177 6169 7420 636c 6965 6e74 2e72  t await client.r
+0000e040: 6563 6569 7665 2829 203d 3d20 2862 2236  eceive() == (b"6
+0000e050: 3534 3332 3122 2c20 7065 6572 5f70 6174  54321", peer_pat
+0000e060: 6829 0a20 2020 2020 2020 2020 2020 2020  h).             
+0000e070: 2020 2020 2020 2074 672e 6361 6e63 656c         tg.cancel
+0000e080: 5f73 636f 7065 2e63 616e 6365 6c28 290a  _scope.cancel().
+0000e090: 0a20 2020 2061 7379 6e63 2064 6566 2074  .    async def t
+0000e0a0: 6573 745f 636f 6e63 7572 7265 6e74 5f72  est_concurrent_r
+0000e0b0: 6563 6569 7665 2873 656c 6629 202d 3e20  eceive(self) -> 
+0000e0c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6173  None:.        as
+0000e0d0: 796e 6320 7769 7468 2061 7761 6974 2063  ync with await c
+0000e0e0: 7265 6174 655f 756e 6978 5f64 6174 6167  reate_unix_datag
+0000e0f0: 7261 6d5f 736f 636b 6574 2829 2061 7320  ram_socket() as 
+0000e100: 756e 6978 5f64 673a 0a20 2020 2020 2020  unix_dg:.       
+0000e110: 2020 2020 2061 7379 6e63 2077 6974 6820       async with 
+0000e120: 6372 6561 7465 5f74 6173 6b5f 6772 6f75  create_task_grou
+0000e130: 7028 2920 6173 2074 673a 0a20 2020 2020  p() as tg:.     
+0000e140: 2020 2020 2020 2020 2020 2074 672e 7374             tg.st
+0000e150: 6172 745f 736f 6f6e 2875 6e69 785f 6467  art_soon(unix_dg
+0000e160: 2e72 6563 6569 7665 290a 2020 2020 2020  .receive).      
+0000e170: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+0000e180: 7761 6974 5f61 6c6c 5f74 6173 6b73 5f62  wait_all_tasks_b
+0000e190: 6c6f 636b 6564 2829 0a20 2020 2020 2020  locked().       
+0000e1a0: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+0000e1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1c0: 2020 7769 7468 2070 7974 6573 742e 7261    with pytest.ra
+0000e1d0: 6973 6573 2842 7573 7952 6573 6f75 7263  ises(BusyResourc
+0000e1e0: 6545 7272 6f72 2920 6173 2065 7863 3a0a  eError) as exc:.
+0000e1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e200: 2020 2020 2020 2020 6177 6169 7420 756e          await un
+0000e210: 6978 5f64 672e 7265 6365 6976 6528 290a  ix_dg.receive().
+0000e220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e230: 2020 2020 2065 7863 2e6d 6174 6368 2822       exc.match("
+0000e240: 616c 7265 6164 7920 7265 6164 696e 6720  already reading 
+0000e250: 6672 6f6d 2229 0a20 2020 2020 2020 2020  from").         
+0000e260: 2020 2020 2020 2066 696e 616c 6c79 3a0a         finally:.
+0000e270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e280: 2020 2020 7467 2e63 616e 6365 6c5f 7363      tg.cancel_sc
+0000e290: 6f70 652e 6361 6e63 656c 2829 0a0a 2020  ope.cancel()..  
+0000e2a0: 2020 6173 796e 6320 6465 6620 7465 7374    async def test
+0000e2b0: 5f63 6c6f 7365 5f64 7572 696e 675f 7265  _close_during_re
+0000e2c0: 6365 6976 6528 7365 6c66 2920 2d3e 204e  ceive(self) -> N
+0000e2d0: 6f6e 653a 0a20 2020 2020 2020 2061 7379  one:.        asy
+0000e2e0: 6e63 2064 6566 2063 6c6f 7365 5f77 6865  nc def close_whe
+0000e2f0: 6e5f 626c 6f63 6b65 6428 2920 2d3e 204e  n_blocked() -> N
+0000e300: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000e310: 2061 7761 6974 2077 6169 745f 616c 6c5f   await wait_all_
+0000e320: 7461 736b 735f 626c 6f63 6b65 6428 290a  tasks_blocked().
+0000e330: 2020 2020 2020 2020 2020 2020 6177 6169              awai
+0000e340: 7420 756e 6978 5f64 672e 6163 6c6f 7365  t unix_dg.aclose
+0000e350: 2829 0a0a 2020 2020 2020 2020 6173 796e  ()..        asyn
+0000e360: 6320 7769 7468 2061 7761 6974 2063 7265  c with await cre
+0000e370: 6174 655f 756e 6978 5f64 6174 6167 7261  ate_unix_datagra
+0000e380: 6d5f 736f 636b 6574 2829 2061 7320 756e  m_socket() as un
+0000e390: 6978 5f64 673a 0a20 2020 2020 2020 2020  ix_dg:.         
+0000e3a0: 2020 2061 7379 6e63 2077 6974 6820 6372     async with cr
+0000e3b0: 6561 7465 5f74 6173 6b5f 6772 6f75 7028  eate_task_group(
+0000e3c0: 2920 6173 2074 673a 0a20 2020 2020 2020  ) as tg:.       
+0000e3d0: 2020 2020 2020 2020 2074 672e 7374 6172           tg.star
+0000e3e0: 745f 736f 6f6e 2863 6c6f 7365 5f77 6865  t_soon(close_whe
+0000e3f0: 6e5f 626c 6f63 6b65 6429 0a20 2020 2020  n_blocked).     
+0000e400: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+0000e410: 7079 7465 7374 2e72 6169 7365 7328 436c  pytest.raises(Cl
+0000e420: 6f73 6564 5265 736f 7572 6365 4572 726f  osedResourceErro
+0000e430: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+0000e440: 2020 2020 2020 2020 6177 6169 7420 756e          await un
+0000e450: 6978 5f64 672e 7265 6365 6976 6528 290a  ix_dg.receive().
+0000e460: 0a20 2020 2061 7379 6e63 2064 6566 2074  .    async def t
+0000e470: 6573 745f 7265 6365 6976 655f 6166 7465  est_receive_afte
+0000e480: 725f 636c 6f73 6528 7365 6c66 2920 2d3e  r_close(self) ->
+0000e490: 204e 6f6e 653a 0a20 2020 2020 2020 2075   None:.        u
+0000e4a0: 6e69 785f 6467 203d 2061 7761 6974 2063  nix_dg = await c
+0000e4b0: 7265 6174 655f 756e 6978 5f64 6174 6167  reate_unix_datag
+0000e4c0: 7261 6d5f 736f 636b 6574 2829 0a20 2020  ram_socket().   
+0000e4d0: 2020 2020 2061 7761 6974 2075 6e69 785f       await unix_
+0000e4e0: 6467 2e61 636c 6f73 6528 290a 2020 2020  dg.aclose().    
+0000e4f0: 2020 2020 7769 7468 2070 7974 6573 742e      with pytest.
+0000e500: 7261 6973 6573 2843 6c6f 7365 6452 6573  raises(ClosedRes
+0000e510: 6f75 7263 6545 7272 6f72 293a 0a20 2020  ourceError):.   
+0000e520: 2020 2020 2020 2020 2061 7761 6974 2075           await u
+0000e530: 6e69 785f 6467 2e72 6563 6569 7665 2829  nix_dg.receive()
+0000e540: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+0000e550: 7465 7374 5f73 656e 645f 6166 7465 725f  test_send_after_
+0000e560: 636c 6f73 6528 7365 6c66 2c20 736f 636b  close(self, sock
+0000e570: 6574 5f70 6174 683a 2050 6174 6829 202d  et_path: Path) -
+0000e580: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000e590: 756e 6978 5f64 6720 3d20 6177 6169 7420  unix_dg = await 
+0000e5a0: 6372 6561 7465 5f75 6e69 785f 6461 7461  create_unix_data
+0000e5b0: 6772 616d 5f73 6f63 6b65 7428 6c6f 6361  gram_socket(loca
+0000e5c0: 6c5f 7061 7468 3d73 6f63 6b65 745f 7061  l_path=socket_pa
+0000e5d0: 7468 290a 2020 2020 2020 2020 7061 7468  th).        path
+0000e5e0: 203d 2073 7472 2873 6f63 6b65 745f 7061   = str(socket_pa
+0000e5f0: 7468 290a 2020 2020 2020 2020 6177 6169  th).        awai
+0000e600: 7420 756e 6978 5f64 672e 6163 6c6f 7365  t unix_dg.aclose
+0000e610: 2829 0a20 2020 2020 2020 2077 6974 6820  ().        with 
+0000e620: 7079 7465 7374 2e72 6169 7365 7328 436c  pytest.raises(Cl
+0000e630: 6f73 6564 5265 736f 7572 6365 4572 726f  osedResourceErro
+0000e640: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+0000e650: 6177 6169 7420 756e 6978 5f64 672e 7365  await unix_dg.se
+0000e660: 6e64 746f 2862 2266 6f6f 222c 2070 6174  ndto(b"foo", pat
+0000e670: 6829 0a0a 2020 2020 6173 796e 6320 6465  h)..    async de
+0000e680: 6620 7465 7374 5f6c 6f63 616c 5f70 6174  f test_local_pat
+0000e690: 685f 6279 7465 7328 7365 6c66 2c20 736f  h_bytes(self, so
+0000e6a0: 636b 6574 5f70 6174 683a 2050 6174 6829  cket_path: Path)
+0000e6b0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+0000e6c0: 2020 6173 796e 6320 7769 7468 2061 7761    async with awa
+0000e6d0: 6974 2063 7265 6174 655f 756e 6978 5f64  it create_unix_d
+0000e6e0: 6174 6167 7261 6d5f 736f 636b 6574 280a  atagram_socket(.
+0000e6f0: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
+0000e700: 6c5f 7061 7468 3d73 7472 2873 6f63 6b65  l_path=str(socke
+0000e710: 745f 7061 7468 292e 656e 636f 6465 2829  t_path).encode()
+0000e720: 0a20 2020 2020 2020 2029 3a0a 2020 2020  .        ):.    
+0000e730: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+0000e740: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
+0000e750: 6b69 7069 6628 0a20 2020 2020 2020 2070  kipif(.        p
+0000e760: 6c61 7466 6f72 6d2e 7379 7374 656d 2829  latform.system()
+0000e770: 203d 3d20 2244 6172 7769 6e22 2c20 7265   == "Darwin", re
+0000e780: 6173 6f6e 3d22 6d61 634f 5320 7265 7175  ason="macOS requ
+0000e790: 6972 6573 2076 616c 6964 2055 5446 2d38  ires valid UTF-8
+0000e7a0: 2070 6174 6873 220a 2020 2020 290a 2020   paths".    ).  
+0000e7b0: 2020 6173 796e 6320 6465 6620 7465 7374    async def test
+0000e7c0: 5f6c 6f63 616c 5f70 6174 685f 696e 7661  _local_path_inva
+0000e7d0: 6c69 645f 6173 6369 6928 7365 6c66 2c20  lid_ascii(self, 
+0000e7e0: 736f 636b 6574 5f70 6174 683a 2050 6174  socket_path: Pat
+0000e7f0: 6829 202d 3e20 4e6f 6e65 3a0a 2020 2020  h) -> None:.    
+0000e800: 2020 2020 7265 616c 5f70 6174 6820 3d20      real_path = 
+0000e810: 7374 7228 736f 636b 6574 5f70 6174 6829  str(socket_path)
+0000e820: 2e65 6e63 6f64 6528 2920 2b20 6222 5c78  .encode() + b"\x
+0000e830: 6630 220a 2020 2020 2020 2020 6173 796e  f0".        asyn
+0000e840: 6320 7769 7468 2061 7761 6974 2063 7265  c with await cre
+0000e850: 6174 655f 756e 6978 5f64 6174 6167 7261  ate_unix_datagra
+0000e860: 6d5f 736f 636b 6574 286c 6f63 616c 5f70  m_socket(local_p
+0000e870: 6174 683d 7265 616c 5f70 6174 6829 3a0a  ath=real_path):.
+0000e880: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+0000e890: 0a0a 0a40 7079 7465 7374 2e6d 6172 6b2e  ...@pytest.mark.
+0000e8a0: 736b 6970 6966 280a 2020 2020 7379 732e  skipif(.    sys.
+0000e8b0: 706c 6174 666f 726d 203d 3d20 2277 696e  platform == "win
+0000e8c0: 3332 222c 2072 6561 736f 6e3d 2255 4e49  32", reason="UNI
+0000e8d0: 5820 736f 636b 6574 7320 6172 6520 6e6f  X sockets are no
+0000e8e0: 7420 6176 6169 6c61 626c 6520 6f6e 2057  t available on W
+0000e8f0: 696e 646f 7773 220a 290a 636c 6173 7320  indows".).class 
+0000e900: 5465 7374 436f 6e6e 6563 7465 6455 4e49  TestConnectedUNI
+0000e910: 5844 6174 6167 7261 6d53 6f63 6b65 743a  XDatagramSocket:
+0000e920: 0a20 2020 2040 7079 7465 7374 2e66 6978  .    @pytest.fix
+0000e930: 7475 7265 0a20 2020 2064 6566 2073 6f63  ture.    def soc
+0000e940: 6b65 745f 7061 7468 2873 656c 6629 202d  ket_path(self) -
+0000e950: 3e20 4765 6e65 7261 746f 725b 5061 7468  > Generator[Path
+0000e960: 2c20 4e6f 6e65 2c20 4e6f 6e65 5d3a 0a20  , None, None]:. 
+0000e970: 2020 2020 2020 2023 2055 7365 2073 7464         # Use std
+0000e980: 6c69 6220 7465 6d70 6469 7220 6765 6e65  lib tempdir gene
+0000e990: 7261 7469 6f6e 0a20 2020 2020 2020 2023  ration.        #
+0000e9a0: 2046 6978 6573 2060 4f53 4572 726f 723a   Fixes `OSError:
+0000e9b0: 2041 465f 554e 4958 2070 6174 6820 746f   AF_UNIX path to
+0000e9c0: 6f20 6c6f 6e67 6020 6672 6f6d 2070 7974  o long` from pyt
+0000e9d0: 6573 7420 6765 6e65 7261 7465 6420 7465  est generated te
+0000e9e0: 6d70 5f70 6174 680a 2020 2020 2020 2020  mp_path.        
+0000e9f0: 7769 7468 2074 656d 7066 696c 652e 5465  with tempfile.Te
+0000ea00: 6d70 6f72 6172 7944 6972 6563 746f 7279  mporaryDirectory
+0000ea10: 2829 2061 7320 7061 7468 3a0a 2020 2020  () as path:.    
+0000ea20: 2020 2020 2020 2020 7969 656c 6420 5061          yield Pa
+0000ea30: 7468 2870 6174 6829 202f 2022 736f 636b  th(path) / "sock
+0000ea40: 6574 220a 0a20 2020 2040 7079 7465 7374  et"..    @pytest
+0000ea50: 2e66 6978 7475 7265 2870 6172 616d 733d  .fixture(params=
+0000ea60: 5b46 616c 7365 2c20 5472 7565 5d2c 2069  [False, True], i
+0000ea70: 6473 3d5b 2273 7472 222c 2022 7061 7468  ds=["str", "path
+0000ea80: 225d 290a 2020 2020 6465 6620 736f 636b  "]).    def sock
+0000ea90: 6574 5f70 6174 685f 6f72 5f73 7472 2873  et_path_or_str(s
+0000eaa0: 656c 662c 2072 6571 7565 7374 3a20 5375  elf, request: Su
+0000eab0: 6252 6571 7565 7374 2c20 736f 636b 6574  bRequest, socket
+0000eac0: 5f70 6174 683a 2050 6174 6829 202d 3e20  _path: Path) -> 
+0000ead0: 5061 7468 207c 2073 7472 3a0a 2020 2020  Path | str:.    
+0000eae0: 2020 2020 7265 7475 726e 2073 6f63 6b65      return socke
+0000eaf0: 745f 7061 7468 2069 6620 7265 7175 6573  t_path if reques
+0000eb00: 742e 7061 7261 6d20 656c 7365 2073 7472  t.param else str
+0000eb10: 2873 6f63 6b65 745f 7061 7468 290a 0a20  (socket_path).. 
+0000eb20: 2020 2040 7079 7465 7374 2e66 6978 7475     @pytest.fixtu
+0000eb30: 7265 0a20 2020 2064 6566 2070 6565 725f  re.    def peer_
+0000eb40: 736f 636b 6574 5f70 6174 6828 7365 6c66  socket_path(self
+0000eb50: 2920 2d3e 2047 656e 6572 6174 6f72 5b50  ) -> Generator[P
+0000eb60: 6174 682c 204e 6f6e 652c 204e 6f6e 655d  ath, None, None]
+0000eb70: 3a0a 2020 2020 2020 2020 2320 5573 6520  :.        # Use 
+0000eb80: 7374 646c 6962 2074 656d 7064 6972 2067  stdlib tempdir g
+0000eb90: 656e 6572 6174 696f 6e0a 2020 2020 2020  eneration.      
+0000eba0: 2020 2320 4669 7865 7320 604f 5345 7272    # Fixes `OSErr
+0000ebb0: 6f72 3a20 4146 5f55 4e49 5820 7061 7468  or: AF_UNIX path
+0000ebc0: 2074 6f6f 206c 6f6e 6760 2066 726f 6d20   too long` from 
+0000ebd0: 7079 7465 7374 2067 656e 6572 6174 6564  pytest generated
+0000ebe0: 2074 656d 705f 7061 7468 0a20 2020 2020   temp_path.     
+0000ebf0: 2020 2077 6974 6820 7465 6d70 6669 6c65     with tempfile
+0000ec00: 2e54 656d 706f 7261 7279 4469 7265 6374  .TemporaryDirect
+0000ec10: 6f72 7928 2920 6173 2070 6174 683a 0a20  ory() as path:. 
+0000ec20: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
+0000ec30: 2050 6174 6828 7061 7468 2920 2f20 2270   Path(path) / "p
+0000ec40: 6565 725f 736f 636b 6574 220a 0a20 2020  eer_socket"..   
+0000ec50: 2040 7079 7465 7374 2e66 6978 7475 7265   @pytest.fixture
+0000ec60: 2870 6172 616d 733d 5b46 616c 7365 2c20  (params=[False, 
+0000ec70: 5472 7565 5d2c 2069 6473 3d5b 2270 6565  True], ids=["pee
+0000ec80: 725f 7374 7222 2c20 2270 6565 725f 7061  r_str", "peer_pa
+0000ec90: 7468 225d 290a 2020 2020 6465 6620 7065  th"]).    def pe
+0000eca0: 6572 5f73 6f63 6b65 745f 7061 7468 5f6f  er_socket_path_o
+0000ecb0: 725f 7374 7228 0a20 2020 2020 2020 2073  r_str(.        s
+0000ecc0: 656c 662c 2072 6571 7565 7374 3a20 5375  elf, request: Su
+0000ecd0: 6252 6571 7565 7374 2c20 7065 6572 5f73  bRequest, peer_s
+0000ece0: 6f63 6b65 745f 7061 7468 3a20 5061 7468  ocket_path: Path
+0000ecf0: 0a20 2020 2029 202d 3e20 5061 7468 207c  .    ) -> Path |
+0000ed00: 2073 7472 3a0a 2020 2020 2020 2020 7265   str:.        re
+0000ed10: 7475 726e 2070 6565 725f 736f 636b 6574  turn peer_socket
+0000ed20: 5f70 6174 6820 6966 2072 6571 7565 7374  _path if request
+0000ed30: 2e70 6172 616d 2065 6c73 6520 7374 7228  .param else str(
+0000ed40: 7065 6572 5f73 6f63 6b65 745f 7061 7468  peer_socket_path
+0000ed50: 290a 0a20 2020 2040 7079 7465 7374 2e66  )..    @pytest.f
+0000ed60: 6978 7475 7265 0a20 2020 2064 6566 2070  ixture.    def p
+0000ed70: 6565 725f 736f 636b 2873 656c 662c 2070  eer_sock(self, p
+0000ed80: 6565 725f 736f 636b 6574 5f70 6174 683a  eer_socket_path:
+0000ed90: 2050 6174 6829 202d 3e20 4974 6572 6162   Path) -> Iterab
+0000eda0: 6c65 5b73 6f63 6b65 742e 736f 636b 6574  le[socket.socket
+0000edb0: 5d3a 0a20 2020 2020 2020 2073 6f63 6b20  ]:.        sock 
+0000edc0: 3d20 736f 636b 6574 2e73 6f63 6b65 7428  = socket.socket(
+0000edd0: 736f 636b 6574 2e41 465f 554e 4958 2c20  socket.AF_UNIX, 
+0000ede0: 736f 636b 6574 2e53 4f43 4b5f 4447 5241  socket.SOCK_DGRA
+0000edf0: 4d29 0a20 2020 2020 2020 2073 6f63 6b2e  M).        sock.
+0000ee00: 7365 7474 696d 656f 7574 2831 290a 2020  settimeout(1).  
+0000ee10: 2020 2020 2020 736f 636b 2e62 696e 6428        sock.bind(
+0000ee20: 7374 7228 7065 6572 5f73 6f63 6b65 745f  str(peer_socket_
+0000ee30: 7061 7468 2929 0a20 2020 2020 2020 2079  path)).        y
+0000ee40: 6965 6c64 2073 6f63 6b0a 2020 2020 2020  ield sock.      
+0000ee50: 2020 736f 636b 2e63 6c6f 7365 2829 0a0a    sock.close()..
+0000ee60: 2020 2020 6173 796e 6320 6465 6620 7465      async def te
+0000ee70: 7374 5f65 7874 7261 5f61 7474 7269 6275  st_extra_attribu
+0000ee80: 7465 7328 0a20 2020 2020 2020 2073 656c  tes(.        sel
+0000ee90: 662c 0a20 2020 2020 2020 2073 6f63 6b65  f,.        socke
+0000eea0: 745f 7061 7468 3a20 5061 7468 2c0a 2020  t_path: Path,.  
+0000eeb0: 2020 2020 2020 7065 6572 5f73 6f63 6b65        peer_socke
+0000eec0: 745f 7061 7468 3a20 5061 7468 2c0a 2020  t_path: Path,.  
+0000eed0: 2020 2020 2020 7065 6572 5f73 6f63 6b3a        peer_sock:
+0000eee0: 2073 6f63 6b65 742e 736f 636b 6574 2c0a   socket.socket,.
+0000eef0: 2020 2020 2920 2d3e 204e 6f6e 653a 0a20      ) -> None:. 
+0000ef00: 2020 2020 2020 2061 7379 6e63 2077 6974         async wit
+0000ef10: 6820 6177 6169 7420 6372 6561 7465 5f63  h await create_c
+0000ef20: 6f6e 6e65 6374 6564 5f75 6e69 785f 6461  onnected_unix_da
+0000ef30: 7461 6772 616d 5f73 6f63 6b65 7428 0a20  tagram_socket(. 
+0000ef40: 2020 2020 2020 2020 2020 2072 656d 6f74             remot
+0000ef50: 655f 7061 7468 3d70 6565 725f 736f 636b  e_path=peer_sock
+0000ef60: 6574 5f70 6174 682c 0a20 2020 2020 2020  et_path,.       
+0000ef70: 2020 2020 206c 6f63 616c 5f70 6174 683d       local_path=
+0000ef80: 736f 636b 6574 5f70 6174 682c 0a20 2020  socket_path,.   
 0000ef90: 2020 2020 2029 2061 7320 756e 6978 5f64       ) as unix_d
-0000efa0: 6731 3a0a 2020 2020 2020 2020 2020 2020  g1:.            
-0000efb0: 6173 796e 6320 7769 7468 2061 7761 6974  async with await
-0000efc0: 2063 7265 6174 655f 636f 6e6e 6563 7465   create_connecte
-0000efd0: 645f 756e 6978 5f64 6174 6167 7261 6d5f  d_unix_datagram_
-0000efe0: 736f 636b 6574 280a 2020 2020 2020 2020  socket(.        
-0000eff0: 2020 2020 2020 2020 7065 6572 5f73 6f63          peer_soc
-0000f000: 6b65 745f 7061 7468 5f6f 725f 7374 722c  ket_path_or_str,
-0000f010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f020: 206c 6f63 616c 5f70 6174 683d 736f 636b   local_path=sock
-0000f030: 6574 5f70 6174 685f 6f72 5f73 7472 2c0a  et_path_or_str,.
-0000f040: 2020 2020 2020 2020 2020 2020 2920 6173              ) as
-0000f050: 2075 6e69 785f 6467 323a 0a20 2020 2020   unix_dg2:.     
-0000f060: 2020 2020 2020 2020 2020 2073 6f63 6b65             socke
-0000f070: 745f 7061 7468 203d 2073 7472 2873 6f63  t_path = str(soc
-0000f080: 6b65 745f 7061 7468 5f6f 725f 7374 7229  ket_path_or_str)
-0000f090: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f0a0: 2020 6177 6169 7420 756e 6978 5f64 6732    await unix_dg2
-0000f0b0: 2e73 656e 6428 6222 626c 6168 2229 0a20  .send(b"blah"). 
-0000f0c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000f0d0: 6571 7565 7374 203d 2061 7761 6974 2075  equest = await u
-0000f0e0: 6e69 785f 6467 312e 7265 6365 6976 6528  nix_dg1.receive(
-0000f0f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000f100: 2020 6173 7365 7274 2072 6571 7565 7374    assert request
-0000f110: 203d 3d20 2862 2262 6c61 6822 2c20 736f   == (b"blah", so
-0000f120: 636b 6574 5f70 6174 6829 0a0a 2020 2020  cket_path)..    
-0000f130: 2020 2020 2020 2020 2020 2020 6177 6169              awai
-0000f140: 7420 756e 6978 5f64 6731 2e73 656e 6474  t unix_dg1.sendt
-0000f150: 6f28 6222 6861 6c62 222c 2073 6f63 6b65  o(b"halb", socke
-0000f160: 745f 7061 7468 290a 2020 2020 2020 2020  t_path).        
-0000f170: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-0000f180: 203d 2061 7761 6974 2075 6e69 785f 6467   = await unix_dg
-0000f190: 322e 7265 6365 6976 6528 290a 2020 2020  2.receive().    
-0000f1a0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-0000f1b0: 7274 2072 6573 706f 6e73 6520 3d3d 2062  rt response == b
-0000f1c0: 2268 616c 6222 0a0a 2020 2020 6173 796e  "halb"..    asyn
-0000f1d0: 6320 6465 6620 7465 7374 5f69 7465 7261  c def test_itera
-0000f1e0: 7465 280a 2020 2020 2020 2020 7365 6c66  te(.        self
-0000f1f0: 2c0a 2020 2020 2020 2020 736f 636b 6574  ,.        socket
-0000f200: 5f70 6174 683a 2050 6174 682c 0a20 2020  _path: Path,.   
-0000f210: 2020 2020 2070 6565 725f 736f 636b 6574       peer_socket
-0000f220: 5f70 6174 683a 2050 6174 682c 0a20 2020  _path: Path,.   
-0000f230: 2029 202d 3e20 4e6f 6e65 3a0a 2020 2020   ) -> None:.    
-0000f240: 2020 2020 6173 796e 6320 6465 6620 7365      async def se
-0000f250: 7276 6528 2920 2d3e 204e 6f6e 653a 0a20  rve() -> None:. 
-0000f260: 2020 2020 2020 2020 2020 2061 7379 6e63             async
-0000f270: 2066 6f72 2070 6163 6b65 7420 696e 2075   for packet in u
-0000f280: 6e69 785f 6467 323a 0a20 2020 2020 2020  nix_dg2:.       
-0000f290: 2020 2020 2020 2020 2061 7761 6974 2075           await u
-0000f2a0: 6e69 785f 6467 322e 7365 6e64 2870 6163  nix_dg2.send(pac
-0000f2b0: 6b65 745b 3a3a 2d31 5d29 0a0a 2020 2020  ket[::-1])..    
-0000f2c0: 2020 2020 6173 796e 6320 7769 7468 2061      async with a
-0000f2d0: 7761 6974 2063 7265 6174 655f 756e 6978  wait create_unix
-0000f2e0: 5f64 6174 6167 7261 6d5f 736f 636b 6574  _datagram_socket
-0000f2f0: 280a 2020 2020 2020 2020 2020 2020 6c6f  (.            lo
-0000f300: 6361 6c5f 7061 7468 3d70 6565 725f 736f  cal_path=peer_so
-0000f310: 636b 6574 5f70 6174 682c 0a20 2020 2020  cket_path,.     
-0000f320: 2020 2029 2061 7320 756e 6978 5f64 6731     ) as unix_dg1
-0000f330: 3a0a 2020 2020 2020 2020 2020 2020 6173  :.            as
-0000f340: 796e 6320 7769 7468 2061 7761 6974 2063  ync with await c
-0000f350: 7265 6174 655f 636f 6e6e 6563 7465 645f  reate_connected_
-0000f360: 756e 6978 5f64 6174 6167 7261 6d5f 736f  unix_datagram_so
-0000f370: 636b 6574 280a 2020 2020 2020 2020 2020  cket(.          
-0000f380: 2020 2020 2020 7065 6572 5f73 6f63 6b65        peer_socke
-0000f390: 745f 7061 7468 2c20 6c6f 6361 6c5f 7061  t_path, local_pa
-0000f3a0: 7468 3d73 6f63 6b65 745f 7061 7468 0a20  th=socket_path. 
-0000f3b0: 2020 2020 2020 2020 2020 2029 2061 7320             ) as 
-0000f3c0: 756e 6978 5f64 6732 3a0a 2020 2020 2020  unix_dg2:.      
-0000f3d0: 2020 2020 2020 2020 2020 7061 7468 203d            path =
-0000f3e0: 2073 7472 2873 6f63 6b65 745f 7061 7468   str(socket_path
-0000f3f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000f400: 2020 6173 796e 6320 7769 7468 2063 7265    async with cre
-0000f410: 6174 655f 7461 736b 5f67 726f 7570 2829  ate_task_group()
-0000f420: 2061 7320 7467 3a0a 2020 2020 2020 2020   as tg:.        
-0000f430: 2020 2020 2020 2020 2020 2020 7467 2e73              tg.s
-0000f440: 7461 7274 5f73 6f6f 6e28 7365 7276 6529  tart_soon(serve)
-0000f450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f460: 2020 2020 2061 7761 6974 2075 6e69 785f       await unix_
-0000f470: 6467 312e 7365 6e64 746f 2862 2246 4f4f  dg1.sendto(b"FOO
-0000f480: 4241 5222 2c20 7061 7468 290a 2020 2020  BAR", path).    
-0000f490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f4a0: 6173 7365 7274 2061 7761 6974 2075 6e69  assert await uni
-0000f4b0: 785f 6467 312e 7265 6365 6976 6528 2920  x_dg1.receive() 
-0000f4c0: 3d3d 2028 6222 5241 424f 4f46 222c 2070  == (b"RABOOF", p
-0000f4d0: 6174 6829 0a20 2020 2020 2020 2020 2020  ath).           
-0000f4e0: 2020 2020 2020 2020 2061 7761 6974 2075           await u
-0000f4f0: 6e69 785f 6467 312e 7365 6e64 746f 2862  nix_dg1.sendto(b
-0000f500: 2231 3233 3435 3622 2c20 7061 7468 290a  "123456", path).
-0000f510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f520: 2020 2020 6173 7365 7274 2061 7761 6974      assert await
-0000f530: 2075 6e69 785f 6467 312e 7265 6365 6976   unix_dg1.receiv
-0000f540: 6528 2920 3d3d 2028 6222 3635 3433 3231  e() == (b"654321
-0000f550: 222c 2070 6174 6829 0a20 2020 2020 2020  ", path).       
-0000f560: 2020 2020 2020 2020 2020 2020 2074 672e               tg.
-0000f570: 6361 6e63 656c 5f73 636f 7065 2e63 616e  cancel_scope.can
-0000f580: 6365 6c28 290a 0a20 2020 2061 7379 6e63  cel()..    async
-0000f590: 2064 6566 2074 6573 745f 636f 6e63 7572   def test_concur
-0000f5a0: 7265 6e74 5f72 6563 6569 7665 280a 2020  rent_receive(.  
-0000f5b0: 2020 2020 2020 7365 6c66 2c20 7065 6572        self, peer
-0000f5c0: 5f73 6f63 6b65 745f 7061 7468 3a20 5061  _socket_path: Pa
-0000f5d0: 7468 2c20 7065 6572 5f73 6f63 6b3a 2073  th, peer_sock: s
-0000f5e0: 6f63 6b65 742e 736f 636b 6574 0a20 2020  ocket.socket.   
-0000f5f0: 2029 202d 3e20 4e6f 6e65 3a0a 2020 2020   ) -> None:.    
-0000f600: 2020 2020 6173 796e 6320 7769 7468 2061      async with a
-0000f610: 7761 6974 2063 7265 6174 655f 636f 6e6e  wait create_conn
-0000f620: 6563 7465 645f 756e 6978 5f64 6174 6167  ected_unix_datag
-0000f630: 7261 6d5f 736f 636b 6574 280a 2020 2020  ram_socket(.    
-0000f640: 2020 2020 2020 2020 7065 6572 5f73 6f63          peer_soc
-0000f650: 6b65 745f 7061 7468 0a20 2020 2020 2020  ket_path.       
-0000f660: 2029 2061 7320 756e 6978 5f64 673a 0a20   ) as unix_dg:. 
-0000f670: 2020 2020 2020 2020 2020 2061 7379 6e63             async
-0000f680: 2077 6974 6820 6372 6561 7465 5f74 6173   with create_tas
-0000f690: 6b5f 6772 6f75 7028 2920 6173 2074 673a  k_group() as tg:
-0000f6a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f6b0: 2074 672e 7374 6172 745f 736f 6f6e 2875   tg.start_soon(u
-0000f6c0: 6e69 785f 6467 2e72 6563 6569 7665 290a  nix_dg.receive).
-0000f6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6e0: 6177 6169 7420 7761 6974 5f61 6c6c 5f74  await wait_all_t
-0000f6f0: 6173 6b73 5f62 6c6f 636b 6564 2829 0a20  asks_blocked(). 
-0000f700: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000f710: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-0000f720: 2020 2020 2020 2020 7769 7468 2070 7974          with pyt
-0000f730: 6573 742e 7261 6973 6573 2842 7573 7952  est.raises(BusyR
-0000f740: 6573 6f75 7263 6545 7272 6f72 2920 6173  esourceError) as
-0000f750: 2065 7863 3a0a 2020 2020 2020 2020 2020   exc:.          
-0000f760: 2020 2020 2020 2020 2020 2020 2020 6177                aw
-0000f770: 6169 7420 756e 6978 5f64 672e 7265 6365  ait unix_dg.rece
-0000f780: 6976 6528 290a 0a20 2020 2020 2020 2020  ive()..         
-0000f790: 2020 2020 2020 2020 2020 2065 7863 2e6d             exc.m
-0000f7a0: 6174 6368 2822 616c 7265 6164 7920 7265  atch("already re
-0000f7b0: 6164 696e 6720 6672 6f6d 2229 0a20 2020  ading from").   
-0000f7c0: 2020 2020 2020 2020 2020 2020 2066 696e               fin
-0000f7d0: 616c 6c79 3a0a 2020 2020 2020 2020 2020  ally:.          
-0000f7e0: 2020 2020 2020 2020 2020 7467 2e63 616e            tg.can
-0000f7f0: 6365 6c5f 7363 6f70 652e 6361 6e63 656c  cel_scope.cancel
-0000f800: 2829 0a0a 2020 2020 6173 796e 6320 6465  ()..    async de
-0000f810: 6620 7465 7374 5f63 6c6f 7365 5f64 7572  f test_close_dur
-0000f820: 696e 675f 7265 6365 6976 6528 0a20 2020  ing_receive(.   
-0000f830: 2020 2020 2073 656c 662c 2070 6565 725f       self, peer_
-0000f840: 736f 636b 6574 5f70 6174 685f 6f72 5f73  socket_path_or_s
-0000f850: 7472 3a20 5061 7468 207c 2073 7472 2c20  tr: Path | str, 
-0000f860: 7065 6572 5f73 6f63 6b3a 2073 6f63 6b65  peer_sock: socke
-0000f870: 742e 736f 636b 6574 0a20 2020 2029 202d  t.socket.    ) -
-0000f880: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0000f890: 6173 796e 6320 6465 6620 636c 6f73 655f  async def close_
-0000f8a0: 7768 656e 5f62 6c6f 636b 6564 2829 202d  when_blocked() -
-0000f8b0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0000f8c0: 2020 2020 6177 6169 7420 7761 6974 5f61      await wait_a
-0000f8d0: 6c6c 5f74 6173 6b73 5f62 6c6f 636b 6564  ll_tasks_blocked
-0000f8e0: 2829 0a20 2020 2020 2020 2020 2020 2061  ().            a
-0000f8f0: 7761 6974 2075 6470 2e61 636c 6f73 6528  wait udp.aclose(
-0000f900: 290a 0a20 2020 2020 2020 2061 7379 6e63  )..        async
-0000f910: 2077 6974 6820 6177 6169 7420 6372 6561   with await crea
-0000f920: 7465 5f63 6f6e 6e65 6374 6564 5f75 6e69  te_connected_uni
-0000f930: 785f 6461 7461 6772 616d 5f73 6f63 6b65  x_datagram_socke
-0000f940: 7428 0a20 2020 2020 2020 2020 2020 2070  t(.            p
-0000f950: 6565 725f 736f 636b 6574 5f70 6174 685f  eer_socket_path_
-0000f960: 6f72 5f73 7472 0a20 2020 2020 2020 2029  or_str.        )
-0000f970: 2061 7320 7564 703a 0a20 2020 2020 2020   as udp:.       
-0000f980: 2020 2020 2061 7379 6e63 2077 6974 6820       async with 
-0000f990: 6372 6561 7465 5f74 6173 6b5f 6772 6f75  create_task_grou
-0000f9a0: 7028 2920 6173 2074 673a 0a20 2020 2020  p() as tg:.     
-0000f9b0: 2020 2020 2020 2020 2020 2074 672e 7374             tg.st
-0000f9c0: 6172 745f 736f 6f6e 2863 6c6f 7365 5f77  art_soon(close_w
-0000f9d0: 6865 6e5f 626c 6f63 6b65 6429 0a20 2020  hen_blocked).   
-0000f9e0: 2020 2020 2020 2020 2020 2020 2077 6974               wit
-0000f9f0: 6820 7079 7465 7374 2e72 6169 7365 7328  h pytest.raises(
-0000fa00: 436c 6f73 6564 5265 736f 7572 6365 4572  ClosedResourceEr
-0000fa10: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
-0000fa20: 2020 2020 2020 2020 2020 6177 6169 7420            await 
-0000fa30: 7564 702e 7265 6365 6976 6528 290a 0a20  udp.receive().. 
-0000fa40: 2020 2061 7379 6e63 2064 6566 2074 6573     async def tes
-0000fa50: 745f 7265 6365 6976 655f 6166 7465 725f  t_receive_after_
-0000fa60: 636c 6f73 6528 0a20 2020 2020 2020 2073  close(.        s
-0000fa70: 656c 662c 2070 6565 725f 736f 636b 6574  elf, peer_socket
-0000fa80: 5f70 6174 685f 6f72 5f73 7472 3a20 5061  _path_or_str: Pa
-0000fa90: 7468 207c 2073 7472 2c20 7065 6572 5f73  th | str, peer_s
-0000faa0: 6f63 6b3a 2073 6f63 6b65 742e 736f 636b  ock: socket.sock
-0000fab0: 6574 0a20 2020 2029 202d 3e20 4e6f 6e65  et.    ) -> None
-0000fac0: 3a0a 2020 2020 2020 2020 7564 7020 3d20  :.        udp = 
-0000fad0: 6177 6169 7420 6372 6561 7465 5f63 6f6e  await create_con
-0000fae0: 6e65 6374 6564 5f75 6e69 785f 6461 7461  nected_unix_data
-0000faf0: 6772 616d 5f73 6f63 6b65 7428 7065 6572  gram_socket(peer
-0000fb00: 5f73 6f63 6b65 745f 7061 7468 5f6f 725f  _socket_path_or_
-0000fb10: 7374 7229 0a20 2020 2020 2020 2061 7761  str).        awa
-0000fb20: 6974 2075 6470 2e61 636c 6f73 6528 290a  it udp.aclose().
-0000fb30: 2020 2020 2020 2020 7769 7468 2070 7974          with pyt
-0000fb40: 6573 742e 7261 6973 6573 2843 6c6f 7365  est.raises(Close
-0000fb50: 6452 6573 6f75 7263 6545 7272 6f72 293a  dResourceError):
-0000fb60: 0a20 2020 2020 2020 2020 2020 2061 7761  .            awa
-0000fb70: 6974 2075 6470 2e72 6563 6569 7665 2829  it udp.receive()
-0000fb80: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-0000fb90: 7465 7374 5f73 656e 645f 6166 7465 725f  test_send_after_
-0000fba0: 636c 6f73 6528 0a20 2020 2020 2020 2073  close(.        s
-0000fbb0: 656c 662c 2070 6565 725f 736f 636b 6574  elf, peer_socket
-0000fbc0: 5f70 6174 685f 6f72 5f73 7472 3a20 5061  _path_or_str: Pa
-0000fbd0: 7468 207c 2073 7472 2c20 7065 6572 5f73  th | str, peer_s
-0000fbe0: 6f63 6b3a 2073 6f63 6b65 742e 736f 636b  ock: socket.sock
-0000fbf0: 6574 0a20 2020 2029 202d 3e20 4e6f 6e65  et.    ) -> None
-0000fc00: 3a0a 2020 2020 2020 2020 7564 7020 3d20  :.        udp = 
-0000fc10: 6177 6169 7420 6372 6561 7465 5f63 6f6e  await create_con
-0000fc20: 6e65 6374 6564 5f75 6e69 785f 6461 7461  nected_unix_data
-0000fc30: 6772 616d 5f73 6f63 6b65 7428 7065 6572  gram_socket(peer
-0000fc40: 5f73 6f63 6b65 745f 7061 7468 5f6f 725f  _socket_path_or_
-0000fc50: 7374 7229 0a20 2020 2020 2020 2061 7761  str).        awa
-0000fc60: 6974 2075 6470 2e61 636c 6f73 6528 290a  it udp.aclose().
-0000fc70: 2020 2020 2020 2020 7769 7468 2070 7974          with pyt
-0000fc80: 6573 742e 7261 6973 6573 2843 6c6f 7365  est.raises(Close
-0000fc90: 6452 6573 6f75 7263 6545 7272 6f72 293a  dResourceError):
-0000fca0: 0a20 2020 2020 2020 2020 2020 2061 7761  .            awa
-0000fcb0: 6974 2075 6470 2e73 656e 6428 6222 666f  it udp.send(b"fo
-0000fcc0: 6f22 290a 0a0a 4070 7974 6573 742e 6d61  o")...@pytest.ma
-0000fcd0: 726b 2e6e 6574 776f 726b 0a61 7379 6e63  rk.network.async
-0000fce0: 2064 6566 2074 6573 745f 6765 7461 6464   def test_getadd
-0000fcf0: 7269 6e66 6f28 2920 2d3e 204e 6f6e 653a  rinfo() -> None:
-0000fd00: 0a20 2020 2023 2049 444e 4120 3230 3033  .    # IDNA 2003
-0000fd10: 2067 6574 7320 7468 6973 2077 726f 6e67   gets this wrong
-0000fd20: 0a20 2020 2063 6f72 7265 6374 203d 2061  .    correct = a
-0000fd30: 7761 6974 2067 6574 6164 6472 696e 666f  wait getaddrinfo
-0000fd40: 2822 6661 c39f 2e64 6522 2c20 3029 0a20  ("fa...de", 0). 
-0000fd50: 2020 2077 726f 6e67 203d 2061 7761 6974     wrong = await
-0000fd60: 2067 6574 6164 6472 696e 666f 2822 6661   getaddrinfo("fa
-0000fd70: 7373 2e64 6522 2c20 3029 0a20 2020 2061  ss.de", 0).    a
-0000fd80: 7373 6572 7420 636f 7272 6563 7420 213d  ssert correct !=
-0000fd90: 2077 726f 6e67 0a0a 0a40 7079 7465 7374   wrong...@pytest
-0000fda0: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
-0000fdb0: 6528 0a20 2020 2022 736f 636b 5f74 7970  e(.    "sock_typ
-0000fdc0: 6522 2c20 5b73 6f63 6b65 742e 534f 434b  e", [socket.SOCK
-0000fdd0: 5f53 5452 4541 4d2c 2073 6f63 6b65 742e  _STREAM, socket.
-0000fde0: 536f 636b 6574 4b69 6e64 2e53 4f43 4b5f  SocketKind.SOCK_
-0000fdf0: 5354 5245 414d 5d0a 290a 6173 796e 6320  STREAM].).async 
-0000fe00: 6465 6620 7465 7374 5f67 6574 6164 6472  def test_getaddr
-0000fe10: 696e 666f 5f69 7076 3661 6464 7228 0a20  info_ipv6addr(. 
-0000fe20: 2020 2073 6f63 6b5f 7479 7065 3a20 4c69     sock_type: Li
-0000fe30: 7465 7261 6c5b 736f 636b 6574 2e53 6f63  teral[socket.Soc
-0000fe40: 6b65 744b 696e 642e 534f 434b 5f53 5452  ketKind.SOCK_STR
-0000fe50: 4541 4d5d 2c0a 2920 2d3e 204e 6f6e 653a  EAM],.) -> None:
-0000fe60: 0a20 2020 2023 2049 444e 4120 7472 6970  .    # IDNA trip
-0000fe70: 7320 7570 206f 7665 7220 7261 7720 4950  s up over raw IP
-0000fe80: 7636 2061 6464 7265 7373 6573 0a20 2020  v6 addresses.   
-0000fe90: 2070 726f 746f 203d 2030 2069 6620 706c   proto = 0 if pl
-0000fea0: 6174 666f 726d 2e73 7973 7465 6d28 2920  atform.system() 
-0000feb0: 3d3d 2022 5769 6e64 6f77 7322 2065 6c73  == "Windows" els
-0000fec0: 6520 360a 2020 2020 6173 7365 7274 2061  e 6.    assert a
-0000fed0: 7761 6974 2067 6574 6164 6472 696e 666f  wait getaddrinfo
-0000fee0: 2822 3a3a 3122 2c20 302c 2074 7970 653d  ("::1", 0, type=
-0000fef0: 736f 636b 5f74 7970 6529 203d 3d20 5b0a  sock_type) == [.
-0000ff00: 2020 2020 2020 2020 280a 2020 2020 2020          (.      
-0000ff10: 2020 2020 2020 736f 636b 6574 2e41 6464        socket.Add
-0000ff20: 7265 7373 4661 6d69 6c79 2e41 465f 494e  ressFamily.AF_IN
-0000ff30: 4554 362c 0a20 2020 2020 2020 2020 2020  ET6,.           
-0000ff40: 2073 6f63 6b65 742e 536f 636b 6574 4b69   socket.SocketKi
-0000ff50: 6e64 2e53 4f43 4b5f 5354 5245 414d 2c0a  nd.SOCK_STREAM,.
-0000ff60: 2020 2020 2020 2020 2020 2020 7072 6f74              prot
-0000ff70: 6f2c 0a20 2020 2020 2020 2020 2020 2022  o,.            "
-0000ff80: 222c 0a20 2020 2020 2020 2020 2020 2028  ",.            (
-0000ff90: 223a 3a31 222c 2030 292c 0a20 2020 2020  "::1", 0),.     
-0000ffa0: 2020 2029 0a20 2020 205d 0a0a 0a61 7379     ).    ]...asy
-0000ffb0: 6e63 2064 6566 2074 6573 745f 6765 746e  nc def test_getn
-0000ffc0: 616d 6569 6e66 6f28 2920 2d3e 204e 6f6e  ameinfo() -> Non
-0000ffd0: 653a 0a20 2020 2065 7870 6563 7465 645f  e:.    expected_
-0000ffe0: 7265 7375 6c74 203d 2073 6f63 6b65 742e  result = socket.
-0000fff0: 6765 746e 616d 6569 6e66 6f28 2822 3132  getnameinfo(("12
-00010000: 372e 302e 302e 3122 2c20 3636 3636 292c  7.0.0.1", 6666),
-00010010: 2030 290a 2020 2020 7265 7375 6c74 203d   0).    result =
-00010020: 2061 7761 6974 2067 6574 6e61 6d65 696e   await getnamein
-00010030: 666f 2828 2231 3237 2e30 2e30 2e31 222c  fo(("127.0.0.1",
-00010040: 2036 3636 3629 290a 2020 2020 6173 7365   6666)).    asse
-00010050: 7274 2072 6573 756c 7420 3d3d 2065 7870  rt result == exp
-00010060: 6563 7465 645f 7265 7375 6c74 0a         ected_result.
+0000efa0: 673a 0a20 2020 2020 2020 2020 2020 2072  g:.            r
+0000efb0: 6177 5f73 6f63 6b65 7420 3d20 756e 6978  aw_socket = unix
+0000efc0: 5f64 672e 6578 7472 6128 536f 636b 6574  _dg.extra(Socket
+0000efd0: 4174 7472 6962 7574 652e 7261 775f 736f  Attribute.raw_so
+0000efe0: 636b 6574 290a 2020 2020 2020 2020 2020  cket).          
+0000eff0: 2020 6173 7365 7274 2072 6177 5f73 6f63    assert raw_soc
+0000f000: 6b65 7420 6973 206e 6f74 204e 6f6e 650a  ket is not None.
+0000f010: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+0000f020: 7274 2075 6e69 785f 6467 2e65 7874 7261  rt unix_dg.extra
+0000f030: 2853 6f63 6b65 7441 7474 7269 6275 7465  (SocketAttribute
+0000f040: 2e66 616d 696c 7929 203d 3d20 4164 6472  .family) == Addr
+0000f050: 6573 7346 616d 696c 792e 4146 5f55 4e49  essFamily.AF_UNI
+0000f060: 580a 2020 2020 2020 2020 2020 2020 6173  X.            as
+0000f070: 7365 7274 2075 6e69 785f 6467 2e65 7874  sert unix_dg.ext
+0000f080: 7261 2853 6f63 6b65 7441 7474 7269 6275  ra(SocketAttribu
+0000f090: 7465 2e6c 6f63 616c 5f61 6464 7265 7373  te.local_address
+0000f0a0: 2920 3d3d 2073 7472 2873 6f63 6b65 745f  ) == str(socket_
+0000f0b0: 7061 7468 290a 2020 2020 2020 2020 2020  path).          
+0000f0c0: 2020 6173 7365 7274 2075 6e69 785f 6467    assert unix_dg
+0000f0d0: 2e65 7874 7261 2853 6f63 6b65 7441 7474  .extra(SocketAtt
+0000f0e0: 7269 6275 7465 2e72 656d 6f74 655f 6164  ribute.remote_ad
+0000f0f0: 6472 6573 7329 203d 3d20 7374 7228 0a20  dress) == str(. 
+0000f100: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000f110: 6565 725f 736f 636b 6574 5f70 6174 680a  eer_socket_path.
+0000f120: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000f130: 2020 2020 2020 2020 2020 7079 7465 7374            pytest
+0000f140: 2e72 6169 7365 7328 0a20 2020 2020 2020  .raises(.       
+0000f150: 2020 2020 2020 2020 2054 7970 6564 4174           TypedAt
+0000f160: 7472 6962 7574 654c 6f6f 6b75 7045 7272  tributeLookupErr
+0000f170: 6f72 2c20 756e 6978 5f64 672e 6578 7472  or, unix_dg.extr
+0000f180: 612c 2053 6f63 6b65 7441 7474 7269 6275  a, SocketAttribu
+0000f190: 7465 2e6c 6f63 616c 5f70 6f72 740a 2020  te.local_port.  
+0000f1a0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000f1b0: 2020 2020 2020 2020 7079 7465 7374 2e72          pytest.r
+0000f1c0: 6169 7365 7328 0a20 2020 2020 2020 2020  aises(.         
+0000f1d0: 2020 2020 2020 2054 7970 6564 4174 7472         TypedAttr
+0000f1e0: 6962 7574 654c 6f6f 6b75 7045 7272 6f72  ibuteLookupError
+0000f1f0: 2c20 756e 6978 5f64 672e 6578 7472 612c  , unix_dg.extra,
+0000f200: 2053 6f63 6b65 7441 7474 7269 6275 7465   SocketAttribute
+0000f210: 2e72 656d 6f74 655f 706f 7274 0a20 2020  .remote_port.   
+0000f220: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+0000f230: 6173 796e 6320 6465 6620 7465 7374 5f73  async def test_s
+0000f240: 656e 645f 7265 6365 6976 6528 0a20 2020  end_receive(.   
+0000f250: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0000f260: 2020 2073 6f63 6b65 745f 7061 7468 5f6f     socket_path_o
+0000f270: 725f 7374 723a 2050 6174 6820 7c20 7374  r_str: Path | st
+0000f280: 722c 0a20 2020 2020 2020 2070 6565 725f  r,.        peer_
+0000f290: 736f 636b 6574 5f70 6174 685f 6f72 5f73  socket_path_or_s
+0000f2a0: 7472 3a20 5061 7468 207c 2073 7472 2c0a  tr: Path | str,.
+0000f2b0: 2020 2020 2920 2d3e 204e 6f6e 653a 0a20      ) -> None:. 
+0000f2c0: 2020 2020 2020 2061 7379 6e63 2077 6974         async wit
+0000f2d0: 6820 6177 6169 7420 6372 6561 7465 5f75  h await create_u
+0000f2e0: 6e69 785f 6461 7461 6772 616d 5f73 6f63  nix_datagram_soc
+0000f2f0: 6b65 7428 0a20 2020 2020 2020 2020 2020  ket(.           
+0000f300: 206c 6f63 616c 5f70 6174 683d 7065 6572   local_path=peer
+0000f310: 5f73 6f63 6b65 745f 7061 7468 5f6f 725f  _socket_path_or_
+0000f320: 7374 722c 0a20 2020 2020 2020 2029 2061  str,.        ) a
+0000f330: 7320 756e 6978 5f64 6731 3a0a 2020 2020  s unix_dg1:.    
+0000f340: 2020 2020 2020 2020 6173 796e 6320 7769          async wi
+0000f350: 7468 2061 7761 6974 2063 7265 6174 655f  th await create_
+0000f360: 636f 6e6e 6563 7465 645f 756e 6978 5f64  connected_unix_d
+0000f370: 6174 6167 7261 6d5f 736f 636b 6574 280a  atagram_socket(.
+0000f380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f390: 7065 6572 5f73 6f63 6b65 745f 7061 7468  peer_socket_path
+0000f3a0: 5f6f 725f 7374 722c 0a20 2020 2020 2020  _or_str,.       
+0000f3b0: 2020 2020 2020 2020 206c 6f63 616c 5f70           local_p
+0000f3c0: 6174 683d 736f 636b 6574 5f70 6174 685f  ath=socket_path_
+0000f3d0: 6f72 5f73 7472 2c0a 2020 2020 2020 2020  or_str,.        
+0000f3e0: 2020 2020 2920 6173 2075 6e69 785f 6467      ) as unix_dg
+0000f3f0: 323a 0a20 2020 2020 2020 2020 2020 2020  2:.             
+0000f400: 2020 2073 6f63 6b65 745f 7061 7468 203d     socket_path =
+0000f410: 2073 7472 2873 6f63 6b65 745f 7061 7468   str(socket_path
+0000f420: 5f6f 725f 7374 7229 0a0a 2020 2020 2020  _or_str)..      
+0000f430: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+0000f440: 756e 6978 5f64 6732 2e73 656e 6428 6222  unix_dg2.send(b"
+0000f450: 626c 6168 2229 0a20 2020 2020 2020 2020  blah").         
+0000f460: 2020 2020 2020 2072 6571 7565 7374 203d         request =
+0000f470: 2061 7761 6974 2075 6e69 785f 6467 312e   await unix_dg1.
+0000f480: 7265 6365 6976 6528 290a 2020 2020 2020  receive().      
+0000f490: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+0000f4a0: 2072 6571 7565 7374 203d 3d20 2862 2262   request == (b"b
+0000f4b0: 6c61 6822 2c20 736f 636b 6574 5f70 6174  lah", socket_pat
+0000f4c0: 6829 0a0a 2020 2020 2020 2020 2020 2020  h)..            
+0000f4d0: 2020 2020 6177 6169 7420 756e 6978 5f64      await unix_d
+0000f4e0: 6731 2e73 656e 6474 6f28 6222 6861 6c62  g1.sendto(b"halb
+0000f4f0: 222c 2073 6f63 6b65 745f 7061 7468 290a  ", socket_path).
+0000f500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f510: 7265 7370 6f6e 7365 203d 2061 7761 6974  response = await
+0000f520: 2075 6e69 785f 6467 322e 7265 6365 6976   unix_dg2.receiv
+0000f530: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+0000f540: 2020 2020 6173 7365 7274 2072 6573 706f      assert respo
+0000f550: 6e73 6520 3d3d 2062 2268 616c 6222 0a0a  nse == b"halb"..
+0000f560: 2020 2020 6173 796e 6320 6465 6620 7465      async def te
+0000f570: 7374 5f69 7465 7261 7465 280a 2020 2020  st_iterate(.    
+0000f580: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0000f590: 2020 736f 636b 6574 5f70 6174 683a 2050    socket_path: P
+0000f5a0: 6174 682c 0a20 2020 2020 2020 2070 6565  ath,.        pee
+0000f5b0: 725f 736f 636b 6574 5f70 6174 683a 2050  r_socket_path: P
+0000f5c0: 6174 682c 0a20 2020 2029 202d 3e20 4e6f  ath,.    ) -> No
+0000f5d0: 6e65 3a0a 2020 2020 2020 2020 6173 796e  ne:.        asyn
+0000f5e0: 6320 6465 6620 7365 7276 6528 2920 2d3e  c def serve() ->
+0000f5f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000f600: 2020 2061 7379 6e63 2066 6f72 2070 6163     async for pac
+0000f610: 6b65 7420 696e 2075 6e69 785f 6467 323a  ket in unix_dg2:
+0000f620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f630: 2061 7761 6974 2075 6e69 785f 6467 322e   await unix_dg2.
+0000f640: 7365 6e64 2870 6163 6b65 745b 3a3a 2d31  send(packet[::-1
+0000f650: 5d29 0a0a 2020 2020 2020 2020 6173 796e  ])..        asyn
+0000f660: 6320 7769 7468 2061 7761 6974 2063 7265  c with await cre
+0000f670: 6174 655f 756e 6978 5f64 6174 6167 7261  ate_unix_datagra
+0000f680: 6d5f 736f 636b 6574 280a 2020 2020 2020  m_socket(.      
+0000f690: 2020 2020 2020 6c6f 6361 6c5f 7061 7468        local_path
+0000f6a0: 3d70 6565 725f 736f 636b 6574 5f70 6174  =peer_socket_pat
+0000f6b0: 682c 0a20 2020 2020 2020 2029 2061 7320  h,.        ) as 
+0000f6c0: 756e 6978 5f64 6731 3a0a 2020 2020 2020  unix_dg1:.      
+0000f6d0: 2020 2020 2020 6173 796e 6320 7769 7468        async with
+0000f6e0: 2061 7761 6974 2063 7265 6174 655f 636f   await create_co
+0000f6f0: 6e6e 6563 7465 645f 756e 6978 5f64 6174  nnected_unix_dat
+0000f700: 6167 7261 6d5f 736f 636b 6574 280a 2020  agram_socket(.  
+0000f710: 2020 2020 2020 2020 2020 2020 2020 7065                pe
+0000f720: 6572 5f73 6f63 6b65 745f 7061 7468 2c20  er_socket_path, 
+0000f730: 6c6f 6361 6c5f 7061 7468 3d73 6f63 6b65  local_path=socke
+0000f740: 745f 7061 7468 0a20 2020 2020 2020 2020  t_path.         
+0000f750: 2020 2029 2061 7320 756e 6978 5f64 6732     ) as unix_dg2
+0000f760: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000f770: 2020 7061 7468 203d 2073 7472 2873 6f63    path = str(soc
+0000f780: 6b65 745f 7061 7468 290a 2020 2020 2020  ket_path).      
+0000f790: 2020 2020 2020 2020 2020 6173 796e 6320            async 
+0000f7a0: 7769 7468 2063 7265 6174 655f 7461 736b  with create_task
+0000f7b0: 5f67 726f 7570 2829 2061 7320 7467 3a0a  _group() as tg:.
+0000f7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f7d0: 2020 2020 7467 2e73 7461 7274 5f73 6f6f      tg.start_soo
+0000f7e0: 6e28 7365 7276 6529 0a20 2020 2020 2020  n(serve).       
+0000f7f0: 2020 2020 2020 2020 2020 2020 2061 7761               awa
+0000f800: 6974 2075 6e69 785f 6467 312e 7365 6e64  it unix_dg1.send
+0000f810: 746f 2862 2246 4f4f 4241 5222 2c20 7061  to(b"FOOBAR", pa
+0000f820: 7468 290a 2020 2020 2020 2020 2020 2020  th).            
+0000f830: 2020 2020 2020 2020 6173 7365 7274 2061          assert a
+0000f840: 7761 6974 2075 6e69 785f 6467 312e 7265  wait unix_dg1.re
+0000f850: 6365 6976 6528 2920 3d3d 2028 6222 5241  ceive() == (b"RA
+0000f860: 424f 4f46 222c 2070 6174 6829 0a20 2020  BOOF", path).   
+0000f870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f880: 2061 7761 6974 2075 6e69 785f 6467 312e   await unix_dg1.
+0000f890: 7365 6e64 746f 2862 2231 3233 3435 3622  sendto(b"123456"
+0000f8a0: 2c20 7061 7468 290a 2020 2020 2020 2020  , path).        
+0000f8b0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+0000f8c0: 7274 2061 7761 6974 2075 6e69 785f 6467  rt await unix_dg
+0000f8d0: 312e 7265 6365 6976 6528 2920 3d3d 2028  1.receive() == (
+0000f8e0: 6222 3635 3433 3231 222c 2070 6174 6829  b"654321", path)
+0000f8f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f900: 2020 2020 2074 672e 6361 6e63 656c 5f73       tg.cancel_s
+0000f910: 636f 7065 2e63 616e 6365 6c28 290a 0a20  cope.cancel().. 
+0000f920: 2020 2061 7379 6e63 2064 6566 2074 6573     async def tes
+0000f930: 745f 636f 6e63 7572 7265 6e74 5f72 6563  t_concurrent_rec
+0000f940: 6569 7665 280a 2020 2020 2020 2020 7365  eive(.        se
+0000f950: 6c66 2c20 7065 6572 5f73 6f63 6b65 745f  lf, peer_socket_
+0000f960: 7061 7468 3a20 5061 7468 2c20 7065 6572  path: Path, peer
+0000f970: 5f73 6f63 6b3a 2073 6f63 6b65 742e 736f  _sock: socket.so
+0000f980: 636b 6574 0a20 2020 2029 202d 3e20 4e6f  cket.    ) -> No
+0000f990: 6e65 3a0a 2020 2020 2020 2020 6173 796e  ne:.        asyn
+0000f9a0: 6320 7769 7468 2061 7761 6974 2063 7265  c with await cre
+0000f9b0: 6174 655f 636f 6e6e 6563 7465 645f 756e  ate_connected_un
+0000f9c0: 6978 5f64 6174 6167 7261 6d5f 736f 636b  ix_datagram_sock
+0000f9d0: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
+0000f9e0: 7065 6572 5f73 6f63 6b65 745f 7061 7468  peer_socket_path
+0000f9f0: 0a20 2020 2020 2020 2029 2061 7320 756e  .        ) as un
+0000fa00: 6978 5f64 673a 0a20 2020 2020 2020 2020  ix_dg:.         
+0000fa10: 2020 2061 7379 6e63 2077 6974 6820 6372     async with cr
+0000fa20: 6561 7465 5f74 6173 6b5f 6772 6f75 7028  eate_task_group(
+0000fa30: 2920 6173 2074 673a 0a20 2020 2020 2020  ) as tg:.       
+0000fa40: 2020 2020 2020 2020 2074 672e 7374 6172           tg.star
+0000fa50: 745f 736f 6f6e 2875 6e69 785f 6467 2e72  t_soon(unix_dg.r
+0000fa60: 6563 6569 7665 290a 2020 2020 2020 2020  eceive).        
+0000fa70: 2020 2020 2020 2020 6177 6169 7420 7761          await wa
+0000fa80: 6974 5f61 6c6c 5f74 6173 6b73 5f62 6c6f  it_all_tasks_blo
+0000fa90: 636b 6564 2829 0a20 2020 2020 2020 2020  cked().         
+0000faa0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+0000fab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fac0: 7769 7468 2070 7974 6573 742e 7261 6973  with pytest.rais
+0000fad0: 6573 2842 7573 7952 6573 6f75 7263 6545  es(BusyResourceE
+0000fae0: 7272 6f72 2920 6173 2065 7863 3a0a 2020  rror) as exc:.  
+0000faf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb00: 2020 2020 2020 6177 6169 7420 756e 6978        await unix
+0000fb10: 5f64 672e 7265 6365 6976 6528 290a 0a20  _dg.receive().. 
+0000fb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb30: 2020 2065 7863 2e6d 6174 6368 2822 616c     exc.match("al
+0000fb40: 7265 6164 7920 7265 6164 696e 6720 6672  ready reading fr
+0000fb50: 6f6d 2229 0a20 2020 2020 2020 2020 2020  om").           
+0000fb60: 2020 2020 2066 696e 616c 6c79 3a0a 2020       finally:.  
+0000fb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb80: 2020 7467 2e63 616e 6365 6c5f 7363 6f70    tg.cancel_scop
+0000fb90: 652e 6361 6e63 656c 2829 0a0a 2020 2020  e.cancel()..    
+0000fba0: 6173 796e 6320 6465 6620 7465 7374 5f63  async def test_c
+0000fbb0: 6c6f 7365 5f64 7572 696e 675f 7265 6365  lose_during_rece
+0000fbc0: 6976 6528 0a20 2020 2020 2020 2073 656c  ive(.        sel
+0000fbd0: 662c 2070 6565 725f 736f 636b 6574 5f70  f, peer_socket_p
+0000fbe0: 6174 685f 6f72 5f73 7472 3a20 5061 7468  ath_or_str: Path
+0000fbf0: 207c 2073 7472 2c20 7065 6572 5f73 6f63   | str, peer_soc
+0000fc00: 6b3a 2073 6f63 6b65 742e 736f 636b 6574  k: socket.socket
+0000fc10: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a0a  .    ) -> None:.
+0000fc20: 2020 2020 2020 2020 6173 796e 6320 6465          async de
+0000fc30: 6620 636c 6f73 655f 7768 656e 5f62 6c6f  f close_when_blo
+0000fc40: 636b 6564 2829 202d 3e20 4e6f 6e65 3a0a  cked() -> None:.
+0000fc50: 2020 2020 2020 2020 2020 2020 6177 6169              awai
+0000fc60: 7420 7761 6974 5f61 6c6c 5f74 6173 6b73  t wait_all_tasks
+0000fc70: 5f62 6c6f 636b 6564 2829 0a20 2020 2020  _blocked().     
+0000fc80: 2020 2020 2020 2061 7761 6974 2075 6470         await udp
+0000fc90: 2e61 636c 6f73 6528 290a 0a20 2020 2020  .aclose()..     
+0000fca0: 2020 2061 7379 6e63 2077 6974 6820 6177     async with aw
+0000fcb0: 6169 7420 6372 6561 7465 5f63 6f6e 6e65  ait create_conne
+0000fcc0: 6374 6564 5f75 6e69 785f 6461 7461 6772  cted_unix_datagr
+0000fcd0: 616d 5f73 6f63 6b65 7428 0a20 2020 2020  am_socket(.     
+0000fce0: 2020 2020 2020 2070 6565 725f 736f 636b         peer_sock
+0000fcf0: 6574 5f70 6174 685f 6f72 5f73 7472 0a20  et_path_or_str. 
+0000fd00: 2020 2020 2020 2029 2061 7320 7564 703a         ) as udp:
+0000fd10: 0a20 2020 2020 2020 2020 2020 2061 7379  .            asy
+0000fd20: 6e63 2077 6974 6820 6372 6561 7465 5f74  nc with create_t
+0000fd30: 6173 6b5f 6772 6f75 7028 2920 6173 2074  ask_group() as t
+0000fd40: 673a 0a20 2020 2020 2020 2020 2020 2020  g:.             
+0000fd50: 2020 2074 672e 7374 6172 745f 736f 6f6e     tg.start_soon
+0000fd60: 2863 6c6f 7365 5f77 6865 6e5f 626c 6f63  (close_when_bloc
+0000fd70: 6b65 6429 0a20 2020 2020 2020 2020 2020  ked).           
+0000fd80: 2020 2020 2077 6974 6820 7079 7465 7374       with pytest
+0000fd90: 2e72 6169 7365 7328 436c 6f73 6564 5265  .raises(ClosedRe
+0000fda0: 736f 7572 6365 4572 726f 7229 3a0a 2020  sourceError):.  
+0000fdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fdc0: 2020 6177 6169 7420 7564 702e 7265 6365    await udp.rece
+0000fdd0: 6976 6528 290a 0a20 2020 2061 7379 6e63  ive()..    async
+0000fde0: 2064 6566 2074 6573 745f 7265 6365 6976   def test_receiv
+0000fdf0: 655f 6166 7465 725f 636c 6f73 6528 0a20  e_after_close(. 
+0000fe00: 2020 2020 2020 2073 656c 662c 2070 6565         self, pee
+0000fe10: 725f 736f 636b 6574 5f70 6174 685f 6f72  r_socket_path_or
+0000fe20: 5f73 7472 3a20 5061 7468 207c 2073 7472  _str: Path | str
+0000fe30: 2c20 7065 6572 5f73 6f63 6b3a 2073 6f63  , peer_sock: soc
+0000fe40: 6b65 742e 736f 636b 6574 0a20 2020 2029  ket.socket.    )
+0000fe50: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+0000fe60: 2020 7564 7020 3d20 6177 6169 7420 6372    udp = await cr
+0000fe70: 6561 7465 5f63 6f6e 6e65 6374 6564 5f75  eate_connected_u
+0000fe80: 6e69 785f 6461 7461 6772 616d 5f73 6f63  nix_datagram_soc
+0000fe90: 6b65 7428 7065 6572 5f73 6f63 6b65 745f  ket(peer_socket_
+0000fea0: 7061 7468 5f6f 725f 7374 7229 0a20 2020  path_or_str).   
+0000feb0: 2020 2020 2061 7761 6974 2075 6470 2e61       await udp.a
+0000fec0: 636c 6f73 6528 290a 2020 2020 2020 2020  close().        
+0000fed0: 7769 7468 2070 7974 6573 742e 7261 6973  with pytest.rais
+0000fee0: 6573 2843 6c6f 7365 6452 6573 6f75 7263  es(ClosedResourc
+0000fef0: 6545 7272 6f72 293a 0a20 2020 2020 2020  eError):.       
+0000ff00: 2020 2020 2061 7761 6974 2075 6470 2e72       await udp.r
+0000ff10: 6563 6569 7665 2829 0a0a 2020 2020 6173  eceive()..    as
+0000ff20: 796e 6320 6465 6620 7465 7374 5f73 656e  ync def test_sen
+0000ff30: 645f 6166 7465 725f 636c 6f73 6528 0a20  d_after_close(. 
+0000ff40: 2020 2020 2020 2073 656c 662c 2070 6565         self, pee
+0000ff50: 725f 736f 636b 6574 5f70 6174 685f 6f72  r_socket_path_or
+0000ff60: 5f73 7472 3a20 5061 7468 207c 2073 7472  _str: Path | str
+0000ff70: 2c20 7065 6572 5f73 6f63 6b3a 2073 6f63  , peer_sock: soc
+0000ff80: 6b65 742e 736f 636b 6574 0a20 2020 2029  ket.socket.    )
+0000ff90: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+0000ffa0: 2020 7564 7020 3d20 6177 6169 7420 6372    udp = await cr
+0000ffb0: 6561 7465 5f63 6f6e 6e65 6374 6564 5f75  eate_connected_u
+0000ffc0: 6e69 785f 6461 7461 6772 616d 5f73 6f63  nix_datagram_soc
+0000ffd0: 6b65 7428 7065 6572 5f73 6f63 6b65 745f  ket(peer_socket_
+0000ffe0: 7061 7468 5f6f 725f 7374 7229 0a20 2020  path_or_str).   
+0000fff0: 2020 2020 2061 7761 6974 2075 6470 2e61       await udp.a
+00010000: 636c 6f73 6528 290a 2020 2020 2020 2020  close().        
+00010010: 7769 7468 2070 7974 6573 742e 7261 6973  with pytest.rais
+00010020: 6573 2843 6c6f 7365 6452 6573 6f75 7263  es(ClosedResourc
+00010030: 6545 7272 6f72 293a 0a20 2020 2020 2020  eError):.       
+00010040: 2020 2020 2061 7761 6974 2075 6470 2e73       await udp.s
+00010050: 656e 6428 6222 666f 6f22 290a 0a0a 4070  end(b"foo")...@p
+00010060: 7974 6573 742e 6d61 726b 2e6e 6574 776f  ytest.mark.netwo
+00010070: 726b 0a61 7379 6e63 2064 6566 2074 6573  rk.async def tes
+00010080: 745f 6765 7461 6464 7269 6e66 6f28 2920  t_getaddrinfo() 
+00010090: 2d3e 204e 6f6e 653a 0a20 2020 2023 2049  -> None:.    # I
+000100a0: 444e 4120 3230 3033 2067 6574 7320 7468  DNA 2003 gets th
+000100b0: 6973 2077 726f 6e67 0a20 2020 2063 6f72  is wrong.    cor
+000100c0: 7265 6374 203d 2061 7761 6974 2067 6574  rect = await get
+000100d0: 6164 6472 696e 666f 2822 6661 c39f 2e64  addrinfo("fa...d
+000100e0: 6522 2c20 3029 0a20 2020 2077 726f 6e67  e", 0).    wrong
+000100f0: 203d 2061 7761 6974 2067 6574 6164 6472   = await getaddr
+00010100: 696e 666f 2822 6661 7373 2e64 6522 2c20  info("fass.de", 
+00010110: 3029 0a20 2020 2061 7373 6572 7420 636f  0).    assert co
+00010120: 7272 6563 7420 213d 2077 726f 6e67 0a0a  rrect != wrong..
+00010130: 0a40 7079 7465 7374 2e6d 6172 6b2e 7061  .@pytest.mark.pa
+00010140: 7261 6d65 7472 697a 6528 0a20 2020 2022  rametrize(.    "
+00010150: 736f 636b 5f74 7970 6522 2c20 5b73 6f63  sock_type", [soc
+00010160: 6b65 742e 534f 434b 5f53 5452 4541 4d2c  ket.SOCK_STREAM,
+00010170: 2073 6f63 6b65 742e 536f 636b 6574 4b69   socket.SocketKi
+00010180: 6e64 2e53 4f43 4b5f 5354 5245 414d 5d0a  nd.SOCK_STREAM].
+00010190: 290a 6173 796e 6320 6465 6620 7465 7374  ).async def test
+000101a0: 5f67 6574 6164 6472 696e 666f 5f69 7076  _getaddrinfo_ipv
+000101b0: 3661 6464 7228 0a20 2020 2073 6f63 6b5f  6addr(.    sock_
+000101c0: 7479 7065 3a20 4c69 7465 7261 6c5b 736f  type: Literal[so
+000101d0: 636b 6574 2e53 6f63 6b65 744b 696e 642e  cket.SocketKind.
+000101e0: 534f 434b 5f53 5452 4541 4d5d 2c0a 2920  SOCK_STREAM],.) 
+000101f0: 2d3e 204e 6f6e 653a 0a20 2020 2023 2049  -> None:.    # I
+00010200: 444e 4120 7472 6970 7320 7570 206f 7665  DNA trips up ove
+00010210: 7220 7261 7720 4950 7636 2061 6464 7265  r raw IPv6 addre
+00010220: 7373 6573 0a20 2020 2070 726f 746f 203d  sses.    proto =
+00010230: 2030 2069 6620 706c 6174 666f 726d 2e73   0 if platform.s
+00010240: 7973 7465 6d28 2920 3d3d 2022 5769 6e64  ystem() == "Wind
+00010250: 6f77 7322 2065 6c73 6520 360a 2020 2020  ows" else 6.    
+00010260: 6173 7365 7274 2061 7761 6974 2067 6574  assert await get
+00010270: 6164 6472 696e 666f 2822 3a3a 3122 2c20  addrinfo("::1", 
+00010280: 302c 2074 7970 653d 736f 636b 5f74 7970  0, type=sock_typ
+00010290: 6529 203d 3d20 5b0a 2020 2020 2020 2020  e) == [.        
+000102a0: 280a 2020 2020 2020 2020 2020 2020 736f  (.            so
+000102b0: 636b 6574 2e41 6464 7265 7373 4661 6d69  cket.AddressFami
+000102c0: 6c79 2e41 465f 494e 4554 362c 0a20 2020  ly.AF_INET6,.   
+000102d0: 2020 2020 2020 2020 2073 6f63 6b65 742e           socket.
+000102e0: 536f 636b 6574 4b69 6e64 2e53 4f43 4b5f  SocketKind.SOCK_
+000102f0: 5354 5245 414d 2c0a 2020 2020 2020 2020  STREAM,.        
+00010300: 2020 2020 7072 6f74 6f2c 0a20 2020 2020      proto,.     
+00010310: 2020 2020 2020 2022 222c 0a20 2020 2020         "",.     
+00010320: 2020 2020 2020 2028 223a 3a31 222c 2030         ("::1", 0
+00010330: 292c 0a20 2020 2020 2020 2029 0a20 2020  ),.        ).   
+00010340: 205d 0a0a 0a61 7379 6e63 2064 6566 2074   ]...async def t
+00010350: 6573 745f 6765 746e 616d 6569 6e66 6f28  est_getnameinfo(
+00010360: 2920 2d3e 204e 6f6e 653a 0a20 2020 2065  ) -> None:.    e
+00010370: 7870 6563 7465 645f 7265 7375 6c74 203d  xpected_result =
+00010380: 2073 6f63 6b65 742e 6765 746e 616d 6569   socket.getnamei
+00010390: 6e66 6f28 2822 3132 372e 302e 302e 3122  nfo(("127.0.0.1"
+000103a0: 2c20 3636 3636 292c 2030 290a 2020 2020  , 6666), 0).    
+000103b0: 7265 7375 6c74 203d 2061 7761 6974 2067  result = await g
+000103c0: 6574 6e61 6d65 696e 666f 2828 2231 3237  etnameinfo(("127
+000103d0: 2e30 2e30 2e31 222c 2036 3636 3629 290a  .0.0.1", 6666)).
+000103e0: 2020 2020 6173 7365 7274 2072 6573 756c      assert resul
+000103f0: 7420 3d3d 2065 7870 6563 7465 645f 7265  t == expected_re
+00010400: 7375 6c74 0a                             sult.
```

### Comparing `anyio-4.3.0/tests/test_subprocesses.py` & `anyio-4.4.0/tests/test_subprocesses.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/tests/test_synchronization.py` & `anyio-4.4.0/tests/test_synchronization.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/tests/test_taskgroups.py` & `anyio-4.4.0/tests/test_taskgroups.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     current_effective_deadline,
     current_time,
     fail_after,
     get_cancelled_exc_class,
     get_current_task,
     move_on_after,
     sleep,
+    sleep_forever,
     wait_all_tasks_blocked,
 )
 from anyio.abc import TaskGroup, TaskStatus
 from anyio.lowlevel import checkpoint
 
 if sys.version_info < (3, 11):
     from exceptiongroup import BaseExceptionGroup, ExceptionGroup
@@ -119,14 +120,24 @@
             task_status.started()
 
     async with create_task_group() as tg:
         value = await tg.start(taskfunc)
         assert value is None
 
 
+async def test_no_called_started_twice() -> None:
+    async def taskfunc(*, task_status: TaskStatus) -> None:
+        task_status.started()
+
+    async with create_task_group() as tg:
+        coro = tg.start(taskfunc)
+        tg.cancel_scope.cancel()
+        await coro
+
+
 async def test_start_with_value() -> None:
     async def taskfunc(*, task_status: TaskStatus) -> None:
         task_status.started("foo")
 
     async with create_task_group() as tg:
         value = await tg.start(taskfunc)
         assert value == "foo"
@@ -181,17 +192,14 @@
         tg.cancel_scope.cancel()
         await tg.start(taskfunc)
 
     assert started
     assert not finished
 
 
-@pytest.mark.xfail(
-    sys.version_info < (3, 9), reason="Requires a way to detect cancellation source"
-)
 @pytest.mark.parametrize("anyio_backend", ["asyncio"])
 async def test_start_native_host_cancelled() -> None:
     started = finished = False
 
     async def taskfunc(*, task_status: TaskStatus) -> None:
         nonlocal started, finished
         started = True
@@ -443,14 +451,27 @@
     cancel_scope = anyio.CancelScope()
     cancel_scope.cancel()
     with cancel_scope:
         await anyio.sleep(1)  # Checkpoint to allow anyio to check for cancellation
         pytest.fail("execution should not reach this point")
 
 
+@pytest.mark.xfail(
+    sys.version_info < (3, 11), reason="Requires asyncio.Task.cancelling()"
+)
+@pytest.mark.parametrize("anyio_backend", ["asyncio"])
+async def test_cancel_counter_nested_scopes() -> None:
+    with CancelScope() as root_scope:
+        with CancelScope():
+            root_scope.cancel()
+            await sleep(0.5)
+
+    assert not cast(asyncio.Task, asyncio.current_task()).cancelling()
+
+
 async def test_exception_group_children() -> None:
     with pytest.raises(BaseExceptionGroup) as exc:
         async with create_task_group() as tg:
             tg.start_soon(async_error, "task1")
             tg.start_soon(async_error, "task2", 0.15)
 
     assert len(exc.value.exceptions) == 2
@@ -529,15 +550,15 @@
 @pytest.mark.xfail(
     reason="There is currently no way to tell if cancellation happened due to timeout "
     "explicitly if the deadline has been exceeded"
 )
 async def test_fail_after_scope_cancelled_before_timeout() -> None:
     with fail_after(0.1) as scope:
         scope.cancel()
-        time.sleep(0.11)
+        time.sleep(0.11)  # noqa: ASYNC101
         await sleep(0)
 
 
 @pytest.mark.parametrize("delay", [0, 0.1], ids=["instant", "delayed"])
 async def test_move_on_after(delay: float) -> None:
     result = False
     with move_on_after(delay) as scope:
@@ -1332,14 +1353,32 @@
             await wait_all_tasks_blocked()
 
             with CancelScope(shield=True), fail_after(1):
                 parent_scope.cancel()
                 await cancelled.wait()
 
 
+async def test_start_cancels_parent_scope() -> None:
+    """Regression test for #685 / #710."""
+    started: bool = False
+
+    async def in_task_group(task_status: TaskStatus[None]) -> None:
+        nonlocal started
+        started = True
+        await sleep_forever()
+
+    async with create_task_group() as tg:
+        with CancelScope() as inner_scope:
+            inner_scope.cancel()
+            await tg.start(in_task_group)
+
+    assert started
+    assert not tg.cancel_scope.cancel_called
+
+
 class TestTaskStatusTyping:
     """
     These tests do not do anything at run time, but since the test suite is also checked
     with a static type checker, it ensures that the `TaskStatus` typing works as
     intended.
     """
```

### Comparing `anyio-4.3.0/tests/test_to_process.py` & `anyio-4.4.0/tests/test_to_process.py`

 * *Files identical despite different names*

### Comparing `anyio-4.3.0/tests/test_to_thread.py` & `anyio-4.4.0/tests/test_to_thread.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import asyncio
 import threading
 import time
-from concurrent.futures import Future
+from concurrent.futures import Future, ThreadPoolExecutor
 from contextvars import ContextVar
 from functools import partial
 from typing import Any, NoReturn
 
 import pytest
 import sniffio
 
@@ -17,14 +17,15 @@
     Event,
     create_task_group,
     from_thread,
     sleep,
     to_thread,
     wait_all_tasks_blocked,
 )
+from anyio.from_thread import BlockingPortalProvider
 
 pytestmark = pytest.mark.anyio
 
 
 async def test_run_in_thread_cancelled() -> None:
     state = 0
 
@@ -283,7 +284,77 @@
     """
 
     def raise_stopiteration() -> NoReturn:
         raise StopIteration
 
     with pytest.raises(RuntimeError, match="coroutine raised StopIteration"):
         await to_thread.run_sync(raise_stopiteration)
+
+
+class TestBlockingPortalProvider:
+    @pytest.fixture
+    def provider(
+        self, anyio_backend_name: str, anyio_backend_options: dict[str, Any]
+    ) -> BlockingPortalProvider:
+        return BlockingPortalProvider(
+            backend=anyio_backend_name, backend_options=anyio_backend_options
+        )
+
+    def test_single_thread(
+        self, provider: BlockingPortalProvider, anyio_backend_name: str
+    ) -> None:
+        threads: set[threading.Thread] = set()
+
+        async def check_thread() -> None:
+            assert sniffio.current_async_library() == anyio_backend_name
+            threads.add(threading.current_thread())
+
+        active_threads_before = threading.active_count()
+        for _ in range(3):
+            with provider as portal:
+                portal.call(check_thread)
+
+        assert len(threads) == 3
+        assert threading.active_count() == active_threads_before
+
+    def test_single_thread_overlapping(
+        self, provider: BlockingPortalProvider, anyio_backend_name: str
+    ) -> None:
+        threads: set[threading.Thread] = set()
+
+        async def check_thread() -> None:
+            assert sniffio.current_async_library() == anyio_backend_name
+            threads.add(threading.current_thread())
+
+        with provider as portal1:
+            with provider as portal2:
+                assert portal1 is portal2
+                portal2.call(check_thread)
+
+            portal1.call(check_thread)
+
+        assert len(threads) == 1
+
+    def test_multiple_threads(
+        self, provider: BlockingPortalProvider, anyio_backend_name: str
+    ) -> None:
+        threads: set[threading.Thread] = set()
+        event = Event()
+
+        async def check_thread() -> None:
+            assert sniffio.current_async_library() == anyio_backend_name
+            await event.wait()
+            threads.add(threading.current_thread())
+
+        def dummy() -> None:
+            with provider as portal:
+                portal.call(check_thread)
+
+        with ThreadPoolExecutor(max_workers=3) as pool:
+            for _ in range(3):
+                pool.submit(dummy)
+
+            with provider as portal:
+                portal.call(wait_all_tasks_blocked)
+                portal.call(event.set)
+
+        assert len(threads) == 1
```

