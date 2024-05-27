# Comparing `tmp/alfasim_sdk-0.9.0.tar.gz` & `tmp/alfasim_sdk-2024.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alfasim_sdk-0.9.0.tar", last modified: Tue May  4 12:34:56 2021, max compression
+gzip compressed data, was "alfasim_sdk-2024.1.tar", last modified: Mon May 27 14:28:18 2024, max compression
```

## Comparing `alfasim_sdk-0.9.0.tar` & `alfasim_sdk-2024.1.tar`

### file list

```diff
@@ -1,58 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     4153 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      308 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      952 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      103 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      102 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/
--rw-r--r--   0 runner    (1001) docker     (121)      352 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/alfasim_sdk.h
--rw-r--r--   0 runner    (1001) docker     (121)    32763 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/api.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/detail/
--rw-r--r--   0 runner    (1001) docker     (121)     6072 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/detail/bootstrap_linux.h
--rw-r--r--   0 runner    (1001) docker     (121)     6176 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/detail/api_pointers.h
--rw-r--r--   0 runner    (1001) docker     (121)     7326 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/detail/bootstrap_win.h
--rw-r--r--   0 runner    (1001) docker     (121)     3677 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/common.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/
--rw-r--r--   0 runner    (1001) docker     (121)    11651 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/generate_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     8573 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/case_description_attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)    62558 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/alfacase_to_case.py
--rw-r--r--   0 runner    (1001) docker     (121)    14730 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/generate_case_description_docstring.py
--rw-r--r--   0 runner    (1001) docker     (121)     2370 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/alfatable.py
--rw-r--r--   0 runner    (1001) docker     (121)    32796 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     2819 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/alfacase.py
--rw-r--r--   0 runner    (1001) docker     (121)    87465 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/case_description.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5410 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/case_to_alfacase.py
--rw-r--r--   0 runner    (1001) docker     (121)    32221 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     2711 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfasim_sdk_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5188 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/units.py
--rw-r--r--   0 runner    (1001) docker     (121)    13372 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/context.py
--rw-r--r--   0 runner    (1001) docker     (121)    16747 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/hook_specs_gui.py
--rw-r--r--   0 runner    (1001) docker     (121)     3910 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/layout.py
--rw-r--r--   0 runner    (1001) docker     (121)     5594 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/models.py
--rw-r--r--   0 runner    (1001) docker     (121)    10611 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     4203 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/variables.py
--rw-r--r--   0 runner    (1001) docker     (121)     1361 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/status.py
--rw-r--r--   0 runner    (1001) docker     (121)     7521 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    77964 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/hook_specs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1290 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/validators.py
--rw-r--r--   0 runner    (1001) docker     (121)      135 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/version.py
--rw-r--r--   0 runner    (1001) docker     (121)    17717 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1830 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     2114 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       89 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1159 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)      796 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/RELEASING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2114 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2653 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/HISTORY.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:28:18.338202 alfasim_sdk-2024.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    12501 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-27 14:28:18.338202 alfasim_sdk-2024.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/RELEASING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-27 14:28:18.338202 alfasim_sdk-2024.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:28:18.326202 alfasim_sdk-2024.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:28:18.330201 alfasim_sdk-2024.1/src/alfasim_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)    21992 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:28:18.330201 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:28:18.334201 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/alfacase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/alfacase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/alfacase/alfacase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73724 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/alfacase/alfacase_to_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/alfacase/alfatable.py
+-rw-r--r--   0 runner    (1001) docker     (127)   138751 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/alfacase/case_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17260 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/alfacase/case_description_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7947 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/alfacase/case_to_alfacase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/alfacase/generate_case_description_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/alfacase/generate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15399 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/alfacase/plugin_alfacase_to_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/alfacase/plugin_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56041 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/alfacase/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/alfasim_sdk_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15350 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14040 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84105 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/hook_specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16442 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/hook_specs_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32201 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/_internal/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:28:18.334201 alfasim_sdk-2024.1/src/alfasim_sdk/alfasim_sdk_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/alfasim_sdk_api/alfasim_sdk.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38362 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/alfasim_sdk_api/api.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/alfasim_sdk_api/common.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:28:18.334201 alfasim_sdk-2024.1/src/alfasim_sdk/alfasim_sdk_api/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)     7530 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/alfasim_sdk_api/detail/api_pointers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/alfasim_sdk_api/detail/bootstrap_linux.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/alfasim_sdk_api/detail/bootstrap_win.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17146 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/default_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:28:18.334201 alfasim_sdk-2024.1/src/alfasim_sdk/result_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/result_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66746 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/result_reader/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/result_reader/aggregator_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9871 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/result_reader/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:28:18.338202 alfasim_sdk-2024.1/src/alfasim_sdk/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk/testing/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:28:18.338202 alfasim_sdk-2024.1/src/alfasim_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-27 14:28:18.000000 alfasim_sdk-2024.1/src/alfasim_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-27 14:28:18.000000 alfasim_sdk-2024.1/src/alfasim_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:28:18.000000 alfasim_sdk-2024.1/src/alfasim_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-27 14:28:18.000000 alfasim_sdk-2024.1/src/alfasim_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:28:18.000000 alfasim_sdk-2024.1/src/alfasim_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-27 14:28:18.000000 alfasim_sdk-2024.1/src/alfasim_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-27 14:28:18.000000 alfasim_sdk-2024.1/src/alfasim_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:28:18.338202 alfasim_sdk-2024.1/src/alfasim_sdk_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/src/alfasim_sdk_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:28:18.338202 alfasim_sdk-2024.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/tests/test_alfasim_sdk_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/tests/test_case_builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/tests/test_hook_specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-05-27 14:28:13.000000 alfasim_sdk-2024.1/tests/test_invoke.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `alfasim_sdk-0.9.0/CONTRIBUTING.rst` & `alfasim_sdk-2024.1/CONTRIBUTING.rst`

 * *Files 6% similar despite different names*

```diff
@@ -116,15 +116,8 @@
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated.
 
 Building the Docs
 -----------------
 
-Inside the folder docs, there is a makefile with all instructions necessary to build the documentation locally. In order to execute this instruction type `make html` inside the `docs` folder, and an HTML file will be generated under `_build\html`
-
-```bash
-cd docs
-make html
-cd  _build\html\
-start index.html
-```
+See `README.rst` in /docs for instructions and tips about building the docs.
```

### Comparing `alfasim_sdk-0.9.0/LICENSE` & `alfasim_sdk-2024.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.9.0/setup.cfg` & `alfasim_sdk-2024.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -6,18 +6,17 @@
 author_email = foss@esss.co
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 classifiers = 
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 
 [options.entry_points]
 console_scripts = 
 	alfasim-sdk=alfasim_sdk:console_main
 
 [options.packages.find]
 where = src
@@ -26,24 +25,25 @@
 * = *.h
 
 [options]
 packages = find:
 package_dir = 
 	=src
 include_package_data = True
-python_requires = >=3.6
+python_requires = >=3.8
 zip_safe = no
 setup_requires = 
 	setuptools>=40.0
 install_requires = 
 	python-hookman
 	typing_inspect
-	strictyaml
+	strictyaml>=1.4.3
 	boltons
 	Click>=7.0
-	barril>=1.9.0
+	barril>=1.13,<2.0
 	pluggy>=0.13.0
+	h5py
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/api.h` & `alfasim_sdk-2024.1/src/alfasim_sdk/alfasim_sdk_api/api.h`

 * *Files 10% similar despite different names*

```diff
@@ -258,71 +258,171 @@
     @param[out] size Size of `out` array of values. It can be the number of volumes or number of faces
                      depending in which #GridScope the secondary variable was registered.
     @return An #error_code value.
 */
 DLL_EXPORT int get_plugin_variable(void* ctx, void** out, const char* variable_name, int line_index, enum TimestepScope ts_scope, int* size);
 
 /*!
-    Gets the field ID of the given name. Althought this depends on the hydrodynamic model being
+    Gets the field ID of the given name. Although this depends on the hydrodynamic model being
     solved, common values include "gas", "oil", "droplet" and "bubble". This functions supports
     retrieve ID of field added by plugin.
 
     @param[in] ctx ALFAsim's plugins context.
     @param[out] out Field ID.
     @param[in] name Name of the field to retrieve the ID.
     @return An #error_code value.
 */
 DLL_EXPORT int get_field_id(void* ctx, int* out, const char* name);
 
 /*!
+    Gets the phase ID of the given name. Although this depends on the hydrodynamic model
+    being solved, common values include "gas", "oil" and "water". This functions supports
+    retrieve ID of phase added by plugin.
+
+    @param[in] ctx ALFAsim's plugins context.
+    @param[out] out Phase ID.
+    @param[in] name Name of the phase to retrieve the ID.
+    @return An #error_code value.
+*/
+DLL_EXPORT int get_phase_id(void* ctx, int* out, const char* name);
+
+/*!
+    Gets the layer ID of the given name. Although this depends on the hydrodynamic model
+    being solved, common values include "gas", "oil" and "water". This functions supports
+    retrieve ID of layer added by plugin.
+
+    @param[in] ctx ALFAsim's plugins context.
+    @param[out] out Layer ID.
+    @param[in] name Name of the layer to retrieve the ID.
+    @return An #error_code value.
+*/
+DLL_EXPORT int get_layer_id(void* ctx, int* out, const char* name);
+
+/*!
+    Gives the number of fields in the hydrodynamic model being solved including dispersed
+    and continuous fields. This information may be important when new fields are added by
+    plugins.
+
+    @param[in] ctx ALFAsim's plugins context.
+    @param[out] out Number of Fields.
+    @return An #error_code value.
+*/
+DLL_EXPORT int get_number_of_fields(void* ctx, int* out);
+
+/*!
+    Gives the number of phases in the hydrodynamic model being solved. This information
+    may be important when new phases are added by plugins.
+
+    @param[in] ctx ALFAsim's plugins context.
+    @param[out] out Number of Phases.
+    @return An #error_code value.
+*/
+DLL_EXPORT int get_number_of_phases(void* ctx, int* out);
+
+/*!
+    Gives the number of layers in the hydrodynamic model being solved. This information
+    may be important when new layers are added by plugins.
+
+    @param[in] ctx ALFAsim's plugins context.
+    @param[out] out Number of layers.
+    @return An #error_code value.
+*/
+DLL_EXPORT int get_number_of_layers(void* ctx, int* out);
+
+/*!
+    Gives the number of phase pairs in the hydrodynamic model being solved. It depends
+    on number of phases and may be important to calculate the phase pair state variables.
+
+    @param[in] ctx ALFAsim's plugins context.
+    @param[out] out Number of phase pairs.
+    @return An #error_code value.
+*/
+DLL_EXPORT int get_number_of_phase_pairs(void* ctx, int* out);
+
+/*!
     Gets the primary field ID of the phase with given name. For example, the "oil" phase has
     primary field "oil". Different phases may have different primary fields. Use this function
     when you need a variable from a field, but you aren't sure about the field name, but you know
     the phase name.
 
     @param[in] ctx ALFAsim's plugins context.
     @param[out] out Field ID.
     @param[in] name Name of the phase to retrieve the primary field ID.
     @return An #error_code value.
 */
 DLL_EXPORT int get_primary_field_id_of_phase(void* ctx, int* out, const char* name);
 
 /*!
-    Gets the phase ID of the given name. Althought this depends on the hydrodynamic model
-    being solved, common values include "gas", "oil" and "water". This functions supports
-    retrieve ID of phase added by plugin.
+    Gets an array of phase IDs, in which each element is related to the fields in the hydrodynamic
+    model. This function is usefull when is necessary to get information from a phase of a specific
+    field (for example "oil in water" field is a "oil" phase).
+
+    Example of usage:
+    ~~~~~{.cpp}
+    errcode = get_phase_id_of_fields(ctx, &phase_of_field, &size);
+    int oil_in_water_phase_id = phase_of_field[oil_in_water_field_id];
+    ~~~~~
 
     @param[in] ctx ALFAsim's plugins context.
-    @param[out] out Phase ID.
-    @param[in] name Name of the phase to retrieve the ID.
+    @param[out] out Phase IDs array.
+    @param[out] size Size of the `out` array of IDs.
     @return An #error_code value.
 */
-DLL_EXPORT int get_phase_id(void* ctx, int* out, const char* name);
+DLL_EXPORT int get_phase_id_of_fields(void* ctx, int** out, int* size);
 
 /*!
-    Gets the layer ID of the given name. Althought this depends on the hydrodynamic model
-    being solved, common values include "gas", "oil" and "water". This functions supports
-    retrieve ID of layer added by plugin.
+    Gets an array of field IDs which are contained in a layer. For example: the "oil" layer could
+    be formed by continuous "oil" field with dispersed "bubble"(gas) and dispersed "water in oil"
+    fields (and also other dispersed fields added by plugins).
+
+    Example of usage:
+    ~~~~~{.cpp}
+    errcode = get_field_ids_in_layer(ctx, &fields_in_Layer, layer_id, &size);
+    ~~~~~
 
     @param[in] ctx ALFAsim's plugins context.
-    @param[out] out Layer ID.
-    @param[in] name Name of the layer to retrieve the ID.
+    @param[out] out Field IDs array.
+    @param[in] layer_id Layer ID in which the field IDs are required.
+    @param[out] size Size of the `out` array of IDs.
     @return An #error_code value.
 */
-DLL_EXPORT int get_layer_id(void* ctx, int* out, const char* name);
+DLL_EXPORT int get_field_ids_in_layer(void* ctx, int** out, int layer_id, int* size);
+
+/*!
+    Gets the phase pair ID given a pair of phase ID's. It is important to calculate a phase pair
+    properties (like surface tension) for more that one phase pair (For example: Gas-Oil,
+    Gas-Water and Oil-Water).
+
+    Since this function has phase ID's in parameters, it MUST be used in conjunction with
+    #get_phase_id function.
+
+    Example of usage:
+    ~~~~~{.cpp}
+    errcode = get_phase_id(ctx, &oil_phase_id, "oil");
+    errcode = get_phase_id(ctx, &water_phase_id, "water");
+    errcode = get_phase_pair_id(ctx, &oil_water_id, oil_phase_id, water_phase_id);
+    ~~~~~
+
+    @param[in] ctx ALFAsim's plugins context.
+    @param[out] out Phase pair ID.
+    @param[in] phase_0_id First phase ID of the pair.
+    @param[in] phase_1_id Second phase ID of the pair.
+    @return An #error_code value.
+*/
+DLL_EXPORT int get_phase_pair_id(void* ctx, int* out, int phase_0_id, int phase_1_id);
 
 /*!
     Gets the current contents of a given state variable (For an array data pointer).
     A state variable is any variable calculated from pressure and temperature,
     as any thermodynamic variable.
 
     Example of usage:
     ~~~~~{.cpp}
     errcode = get_state_variable_array(
-        ctx, enthalpy, StateVariable::H, FIELD_GAS, size);
+        ctx, &enthalpy, StateVariable::H, FIELD_GAS, &size);
     ~~~~~
 
     @param[in] ctx ALFAsim's plugins context.
     @param[out] out State Variable values array.
     @param[in] state_var A #StateVariable value. It indicates which variable to be retrieved.
     @param[in] field_index Index of the field in which the state variable is retrieved.
     @param[out] size Size of the `out` array of values.
@@ -359,19 +459,21 @@
     - `"RSW"`: Water vapour mass fraction in gas phase [kg/kg]
     - `"S_w"`: Wetted Perimeter of a layer [m]
     - `"ff_S_wall"`: Wall friction factor times wall perimeter [-]
     - `"ff_S_interface"`: Interface Friction factor times interface perimeter [-]
     - `"D"`: Pipe Inner Diameter [m]
     - `"A"`: Cross-sectional Area in each control volume [m2]
     - `"theta"`: Inclination of each control volume [rad]
+    - `"ks"`: Pipe roughness. Only available for FACE GridScope  [m]
     - `"dx"`: Control Volume Length along the Pipe Axis [m]
     - `"dv"`: Volume of the control volume [m3]
     - `"D_eff"`: Effective Pipe Inner Diameter, considering the internal deposit layers [m]
     - `"A_eff"`: Cross-sectional Area Effective in each control volume, considering the internal deposit layers [m2]
     - `"dv_eff"`: Effective Volume of the control volume, considering the internal deposit layers [m3]
+    - `"volumetric_flow_rate"` : Volumetric flow rate [m3/s]
 
     It is important to know that the listed `variable_name`s are no available in all #MultiFieldDescriptionScope
     and #GridScope. Because of that, the #error_code must be checked.
 
     @param[in] ctx ALFAsim's plugins context.
     @param[out] out Variable values array.
     @param[in] variable_name String with the variable name. See the list of possible values above.
@@ -501,14 +603,28 @@
     int** out,
     enum GridScope grid_scope,
     enum TimestepScope ts_scope,
     int* size
 );
 
 /*!
+    Returns the thickness of the deposition of phase on pipe inner wall.
+
+    @param[in] ctx ALFAsim's plugins context.
+    @param[out] out Thickness of phase deposited on inner wall.
+    @param[in] phase_id Phase index.
+    @param[in] ts_scope A #TimestepScope value.
+    @param[in] size Size of out array of values.
+    @return An #error_code value.
+*/
+DLL_EXPORT int get_deposition_thickness(
+   void* ctx, double** out, int phase_id, enum TimestepScope ts_scope, int* size
+);
+
+/*!
     Retrieves the tracer ID given a tracer reference. A tracer reference may be obtained from the
     user input data (See #get_plugin_input_data_reference API function for an example).
 
     @param[in] ctx ALFAsim's plugins context.
     @param[out] tracer_id Tracer ID.
     @param[in] reference Tracer reference.
     @return An #error_code value.
@@ -774,8 +890,38 @@
                             to a phase any value can be passed.
     @return An #error_code value.
 */
 DLL_EXPORT int get_liq_liq_shear_force_per_volume_input_variable(
     void* ctx, double* out, const char* var_name, int phase_id
 );
 
+/*!
+    Gets the relative emulsion viscosity for liquid-liquid calculations.
+
+    During the implementation of any HOOK related to the Liquid-Liquid Mechanistic model, this
+    function provides the relative emulsion viscosity from Emulsion Model (selected through GUI).
+
+    It allows the plugin HOOKs to use the same emulsion model used internally by ALFAsim.
+
+    The definition of relative viscosity is given by the ratio between the apparent viscosity
+    (dispersed field + continuous field) and the continuous field.
+
+    @param[in] ctx ALFAsim's plugins context.
+    @param[out] out Relative Emulsion Viscosity [-].
+    @param[in] mu_disp Dispersed Field Viscosity [Pa.s].
+    @param[in] mu_cont Continuous Field Viscosity [Pa.s].
+    @param[in] alpha_disp_in_layer Dispersed Field Volume Fraction in the layer (emulsion) [m3 of dispersed field /m3 of layer].
+    @param[in] T Fluid temperature [K].
+    @param[in] water_in_oil True when water is dispersed in oil, otherwise it is a dispersion of oil in water.
+    @return An #error_code value.
+*/
+DLL_EXPORT int get_relative_emulsion_viscosity(
+    void* ctx,
+    double* out,
+    double mu_disp,
+    double mu_cont,
+    double alpha_disp_in_layer,
+    double T,
+    bool water_in_oil
+);
+
 #endif
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/detail/bootstrap_linux.h` & `alfasim_sdk-2024.1/src/alfasim_sdk/alfasim_sdk_api/detail/bootstrap_linux.h`

 * *Files 13% similar despite different names*

```diff
@@ -58,37 +58,46 @@
     api->get_plugin_input_data_string = (get_plugin_input_data_string_func)dlsym(api->handle, "get_plugin_input_data_string");
     api->get_plugin_input_data_string_size = (get_plugin_input_data_string_size_func)dlsym(api->handle, "get_plugin_input_data_string_size");
     api->get_plugin_input_data_file_content = (get_plugin_input_data_file_content_func)dlsym(api->handle, "get_plugin_input_data_file_content");
     api->get_plugin_input_data_file_content_size = (get_plugin_input_data_file_content_size_func)dlsym(api->handle, "get_plugin_input_data_file_content_size");
     api->get_plugin_input_data_reference = (get_plugin_input_data_reference_func)dlsym(api->handle, "get_plugin_input_data_reference");
     api->get_plugin_variable = (get_plugin_variable_func)dlsym(api->handle, "get_plugin_variable");
     api->get_field_id = (get_field_id_func)dlsym(api->handle, "get_field_id");
-    api->get_primary_field_id_of_phase = (get_field_id_func)dlsym(api->handle, "get_primary_field_id_of_phase");
     api->get_phase_id = (get_phase_id_func)dlsym(api->handle, "get_phase_id");
     api->get_layer_id = (get_layer_id_func)dlsym(api->handle, "get_layer_id");
+    api->get_number_of_fields = (get_number_of_fields_func)dlsym(api->handle, "get_number_of_fields");
+    api->get_number_of_phases = (get_number_of_phases_func)dlsym(api->handle, "get_number_of_phases");
+    api->get_number_of_layers = (get_number_of_layers_func)dlsym(api->handle, "get_number_of_layers");
+    api->get_number_of_phase_pairs = (get_number_of_phase_pairs_func)dlsym(api->handle, "get_number_of_phase_pairs");
+    api->get_primary_field_id_of_phase = (get_field_id_func)dlsym(api->handle, "get_primary_field_id_of_phase");
+    api->get_phase_id_of_fields = (get_phase_id_of_fields_func)dlsym(api->handle, "get_phase_id_of_fields");
+    api->get_field_ids_in_layer = (get_field_ids_in_layer_func)dlsym(api->handle, "get_field_ids_in_layer");
+    api->get_phase_pair_id = (get_phase_pair_id_func)dlsym(api->handle, "get_phase_pair_id");
     api->get_state_variable_array = (get_state_variable_array_func)dlsym(api->handle, "get_state_variable_array");
     api->get_simulation_array = (get_simulation_array_func)dlsym(api->handle, "get_simulation_array");
     api->get_simulation_tracer_array = (get_simulation_tracer_array_func)dlsym(api->handle, "get_simulation_tracer_array");
     api->get_simulation_quantity = (get_simulation_quantity_func)dlsym(api->handle, "get_simulation_quantity");
     api->get_wall_interfaces_temperature = (get_wall_interfaces_temperature_func)dlsym(api->handle, "get_wall_interfaces_temperature");
     api->get_flow_pattern = (get_flow_pattern_func)dlsym(api->handle, "get_flow_pattern");
     api->get_liqliq_flow_pattern = (get_flow_pattern_func)dlsym(api->handle, "get_liqliq_flow_pattern");
+    api->get_deposition_thickness = (get_deposition_thickness_func)dlsym(api->handle, "get_deposition_thickness");
     api->get_plugin_input_data_table_quantity = (get_plugin_input_data_table_quantity_func)dlsym(api->handle, "get_plugin_input_data_table_quantity");
     api->get_tracer_id = (get_tracer_id_func)dlsym(api->handle, "get_tracer_id");
     api->get_tracer_name_size = (get_tracer_name_size_func)dlsym(api->handle, "get_tracer_name_size");
     api->get_tracer_name = (get_tracer_name_func)dlsym(api->handle, "get_tracer_name");
     api->get_tracer_ref_by_name = (get_tracer_ref_by_name_func)dlsym(api->handle, "get_tracer_ref_by_name");
     api->get_tracer_partition_coefficient = (get_tracer_partition_coefficient_func)dlsym(api->handle, "get_tracer_partition_coefficient");
     api->get_plugin_input_data_multiplereference_selected_size = (get_plugin_input_data_multiplereference_selected_size_func)dlsym(api->handle, "get_plugin_input_data_multiplereference_selected_size");
     api->get_ucm_friction_factor_input_variable = (get_input_variable_func)dlsym(api->handle, "get_ucm_friction_factor_input_variable");
     api->get_ucm_fluid_geometrical_properties = (get_ucm_fluid_geometrical_properties_func)dlsym(api->handle, "get_ucm_fluid_geometrical_properties");
     api->get_liq_liq_flow_pattern_input_variable = (get_input_variable_func)dlsym(api->handle, "get_liq_liq_flow_pattern_input_variable");
     api->get_liquid_effective_viscosity_input_variable = (get_input_variable_func)dlsym(api->handle, "get_liquid_effective_viscosity_input_variable");
     api->get_gas_liq_surface_tension_input_variable = (get_input_variable_func)dlsym(api->handle, "get_gas_liq_surface_tension_input_variable");
     api->get_liq_liq_shear_force_per_volume_input_variable = (get_input_variable_func)dlsym(api->handle, "get_liq_liq_shear_force_per_volume_input_variable");
+    api->get_relative_emulsion_viscosity = (get_relative_emulsion_viscosity_func)dlsym(api->handle, "get_relative_emulsion_viscosity");
 
     return SDK_OK;
 }
 
 inline void alfasim_sdk_close(ALFAsimSDK_API* api)
 {
     if (api->handle != nullptr){
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/detail/bootstrap_win.h` & `alfasim_sdk-2024.1/src/alfasim_sdk/alfasim_sdk_api/detail/bootstrap_win.h`

 * *Files 16% similar despite different names*

```diff
@@ -82,37 +82,46 @@
     api->get_plugin_input_data_string = (get_plugin_input_data_string_func)GetProcAddress(api->handle, "get_plugin_input_data_string");
     api->get_plugin_input_data_string_size = (get_plugin_input_data_string_size_func)GetProcAddress(api->handle, "get_plugin_input_data_string_size");
     api->get_plugin_input_data_file_content = (get_plugin_input_data_file_content_func)GetProcAddress(api->handle, "get_plugin_input_data_file_content");
     api->get_plugin_input_data_file_content_size = (get_plugin_input_data_file_content_size_func)GetProcAddress(api->handle, "get_plugin_input_data_file_content_size");
     api->get_plugin_input_data_reference = (get_plugin_input_data_reference_func)GetProcAddress(api->handle, "get_plugin_input_data_reference");
     api->get_plugin_variable = (get_plugin_variable_func)GetProcAddress(api->handle, "get_plugin_variable");
     api->get_field_id = (get_field_id_func)GetProcAddress(api->handle, "get_field_id");
-    api->get_primary_field_id_of_phase = (get_primary_field_id_of_phase_func)GetProcAddress(api->handle, "get_primary_field_id_of_phase");
     api->get_phase_id = (get_phase_id_func)GetProcAddress(api->handle, "get_phase_id");
     api->get_layer_id = (get_layer_id_func)GetProcAddress(api->handle, "get_layer_id");
+    api->get_number_of_fields = (get_number_of_fields_func)GetProcAddress(api->handle, "get_number_of_fields");
+    api->get_number_of_phases = (get_number_of_phases_func)GetProcAddress(api->handle, "get_number_of_phases");
+    api->get_number_of_layers = (get_number_of_layers_func)GetProcAddress(api->handle, "get_number_of_layers");
+    api->get_number_of_phase_pairs = (get_number_of_phase_pairs_func)GetProcAddress(api->handle, "get_number_of_phase_pairs");
+    api->get_primary_field_id_of_phase = (get_primary_field_id_of_phase_func)GetProcAddress(api->handle, "get_primary_field_id_of_phase");
+    api->get_phase_id_of_fields = (get_phase_id_of_fields_func)GetProcAddress(api->handle, "get_phase_id_of_fields");
+    api->get_field_ids_in_layer = (get_field_ids_in_layer_func)GetProcAddress(api->handle, "get_field_ids_in_layer");
+    api->get_phase_pair_id = (get_phase_pair_id_func)GetProcAddress(api->handle, "get_phase_pair_id");
     api->get_state_variable_array = (get_state_variable_array_func)GetProcAddress(api->handle, "get_state_variable_array");
     api->get_simulation_array = (get_simulation_array_func)GetProcAddress(api->handle, "get_simulation_array");
     api->get_simulation_tracer_array = (get_simulation_tracer_array_func)GetProcAddress(api->handle, "get_simulation_tracer_array");
     api->get_simulation_quantity = (get_simulation_quantity_func)GetProcAddress(api->handle, "get_simulation_quantity");
     api->get_wall_interfaces_temperature = (get_wall_interfaces_temperature_func)GetProcAddress(api->handle, "get_wall_interfaces_temperature");
     api->get_flow_pattern = (get_flow_pattern_func)GetProcAddress(api->handle, "get_flow_pattern");
     api->get_liqliq_flow_pattern = (get_flow_pattern_func)GetProcAddress(api->handle, "get_liqliq_flow_pattern");
+    api->get_deposition_thickness = (get_deposition_thickness_func)GetProcAddress(api->handle, "get_deposition_thickness");
     api->get_plugin_input_data_table_quantity = (get_plugin_input_data_table_quantity_func)GetProcAddress(api->handle, "get_plugin_input_data_table_quantity");
     api->get_tracer_id = (get_tracer_id_func)GetProcAddress(api->handle, "get_tracer_id");
     api->get_tracer_name_size = (get_tracer_name_size_func)GetProcAddress(api->handle, "get_tracer_name_size");
     api->get_tracer_name = (get_tracer_name_func)GetProcAddress(api->handle, "get_tracer_name");
     api->get_tracer_ref_by_name = (get_tracer_ref_by_name_func)GetProcAddress(api->handle, "get_tracer_ref_by_name");
     api->get_tracer_partition_coefficient = (get_tracer_partition_coefficient_func)GetProcAddress(api->handle, "get_tracer_partition_coefficient");
     api->get_plugin_input_data_multiplereference_selected_size = (get_plugin_input_data_multiplereference_selected_size_func)GetProcAddress(api->handle, "get_plugin_input_data_multiplereference_selected_size");
     api->get_ucm_friction_factor_input_variable = (get_input_variable_func)GetProcAddress(api->handle, "get_ucm_friction_factor_input_variable");
     api->get_ucm_fluid_geometrical_properties = (get_ucm_fluid_geometrical_properties_func)GetProcAddress(api->handle, "get_ucm_fluid_geometrical_properties");
     api->get_liq_liq_flow_pattern_input_variable = (get_input_variable_func)GetProcAddress(api->handle, "get_liq_liq_flow_pattern_input_variable");
     api->get_liquid_effective_viscosity_input_variable = (get_input_variable_func)GetProcAddress(api->handle, "get_liquid_effective_viscosity_input_variable");
     api->get_gas_liq_surface_tension_input_variable = (get_input_variable_func)GetProcAddress(api->handle, "get_gas_liq_surface_tension_input_variable");
     api->get_liq_liq_shear_force_per_volume_input_variable = (get_input_variable_func)GetProcAddress(api->handle, "get_liq_liq_shear_force_per_volume_input_variable");
+    api->get_relative_emulsion_viscosity = (get_relative_emulsion_viscosity_func)GetProcAddress(api->handle, "get_relative_emulsion_viscosity");
 
     return SDK_OK;
 }
 
 /*!
     Unload ALFAsim-SDK API dll.
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/common.h` & `alfasim_sdk-2024.1/src/alfasim_sdk/alfasim_sdk_api/common.h`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,17 @@
     RHO, /*!< Density*/
     MU, /*!< Viscosity*/
     CP, /*!< Heat Capacity*/
     DRHO_DP, /*!< Partial derivative of density in relation to pressure*/
     DRHO_DT, /*!< Partial derivative of density in relation to temperature*/
     H, /*!< Enthalpy*/
     K, /*!< Thermal Conductivity*/
-    SIGMA /*!< Interfacial tension*/
+    SIGMA, /*!< Interfacial tension*/
+    RS, /*!< gas mass fraction w.r.t. to hydrocarbon system*/
+    RSW /*!< vapor mass fraction w.r.t. to gas system*/
 };
 
 /*!
     It holds all variable scopes (grid, multifield and timestep)
 */
 struct VariableScope
 {
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/generate_schema.py` & `alfasim_sdk-2024.1/src/alfasim_sdk/_internal/alfacase/generate_schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,109 +7,121 @@
 from enum import EnumMeta
 from pathlib import Path
 from typing import List
 from typing import Set
 
 import attr
 import typing_inspect
+from barril.curve.curve import Curve
 from barril.units import Array
 from barril.units import Scalar
 from strictyaml.utils import flatten
 from typing_inspect import is_optional_type
 
 from alfasim_sdk import CaseDescription
 
-
 INDENTANTION = "    "
 
 
-def is_enum(value):
+def is_enum(value: typing.Any):
     return isinstance(value, EnumMeta)
 
 
-def enum_to_alfacase_schema(type_, block_indentation):
+def enum_to_alfacase_schema(type_: type, indent: int) -> str:
     return f"Enum({[i.value for i in type_]})"
 
 
-def is_numpy_1_darray(type_):
+def is_numpy_1_darray(type_: type) -> bool:
     return typing_inspect.is_new_type(type_) and type_.__name__ == "Numpy1DArray"
 
 
-def numpy_1_darray_to_alfacase_schema(type_, block_indentation):
+def numpy_1_darray_to_alfacase_schema(type_: type, indent: int) -> str:
     return "Seq(Float())"
 
 
-def is_list(type_):
+def is_list(type_: type) -> bool:
     return typing_inspect.get_origin(type_) in (typing.List, list)
 
 
-def list_to_alfacase_schema(type_, block_indentation):
+def list_to_alfacase_schema(type_: type, indent: int) -> str:
     list_value = typing_inspect.get_args(type_)[0]
-    return f"Seq({_get_attr_value(list_value, block_indentation=block_indentation[:-len(INDENTANTION)])})"
+    return f"Seq({_get_attr_value(list_value, indent=indent+1)})"
 
 
-def is_float(type_):
+def is_float(type_: type) -> bool:
     return inspect.isclass(type_) and issubclass(type_, float)
 
 
-def float_to_alfacase_schema(type_, block_indentation):
+def float_to_alfacase_schema(type_: type, indent: int) -> str:
     return "Float()"
 
 
-def is_boolean(type_):
+def is_boolean(type_: type) -> bool:
     return inspect.isclass(type_) and issubclass(type_, bool)
 
 
-def boolean_to_alfacase_schema(type_, block_indentation):
+def boolean_to_alfacase_schema(type_: type, indent: int) -> str:
     return "Bool()"
 
 
-def is_str(type_):
+def is_str(type_: type) -> bool:
     return inspect.isclass(type_) and issubclass(type_, str)
 
 
-def str_to_alfacase_schema(type_, block_indentation):
+def str_to_alfacase_schema(type_: type, indent: int) -> str:
     return "Str()"
 
 
-def is_attrs(type_):
-    return any((hasattr(i, "__attrs_attrs__") for i in flatten([type_])))
+def is_attrs(type_: type) -> bool:
+    return any(hasattr(i, "__attrs_attrs__") for i in flatten([type_]))
 
 
-def attrs_to_alfacase_schema(type_, block_indentation):
+def attrs_to_alfacase_schema(type_: type, indent: int) -> str:
     return obtain_schema_name(type_)
 
 
-def is_dict(type_):
+def is_dict(type_: type) -> bool:
     return typing_inspect.get_origin(type_) in (typing.Dict, dict)
 
 
-def dict_to_alfacase_schema(type_, block_indentation):
+def dict_to_alfacase_schema(type_: type, indent: int) -> str:
     key_type, value_type = (
         typing_inspect.get_last_args(type_)
         if sys.version_info.minor == 6
         else typing_inspect.get_args(type_)
     )
-    return f"MapPattern(Str(), {_get_attr_value(value_type)})"
+    body_indent = indent + 1
+    value_schema = _get_attr_value(value_type, indent=body_indent)
+    if "\n" in value_schema:
+        lines = [
+            "MapPattern(",
+            f"{INDENTANTION * body_indent}Str(),",
+            f"{INDENTANTION * body_indent}{value_schema},",
+            f"{INDENTANTION * indent})",
+        ]
+        return "\n".join(lines)
+    else:
+        return f"MapPattern(Str(), {value_schema})"
 
 
-def is_union(type_):
+def is_union(type_: type) -> bool:
     return typing_inspect.is_union_type(type_)
 
 
 @contextmanager
-def _map_section(lines, block_indentation=INDENTANTION):
+def _map_section(lines: List[str], indent=0) -> List[str]:
+    body_indent = indent + 1
     lines.append("Map(")
-    lines.append(block_indentation + "{")
+    lines.append(f"{INDENTANTION * body_indent}{{")
     yield lines
-    lines.append(block_indentation + "}")
-    lines.append(block_indentation[: -len(INDENTANTION)] + ")")
+    lines.append(f"{INDENTANTION * body_indent}}}")
+    lines.append(f"{INDENTANTION * indent})")
 
 
-def union_to_alfacase_schema(type_, *, block_indentation=INDENTANTION):
+def union_to_alfacase_schema(type_: type, *, indent=0) -> str:
     """
     Creates a structure that allows multiples types for the same key.
 
     There is a validator for this kind of situation within strictyaml but does not work
     with Maps/Seqs as discussed in https://github.com/crdoconnor/strictyaml/issues/51
     The alternative presented from the maintainer was to use the `revalidate` method after the load.
 
@@ -124,90 +136,107 @@
     """
     # PvtModel Tables
     if set(type_.__args__) == {str, Path}:
         return "Str()"
 
     # Attrs classes
     lines = []
-    with _map_section(lines, block_indentation=block_indentation):
+    map_items_indent = indent + 2
+    with _map_section(lines, indent=indent):
         for arg in type_.__args__:
             key = convert_to_snake_case(arg.__name__.replace("Description", ""))
             value = obtain_schema_name(arg)
             lines.append(
-                block_indentation + INDENTANTION + f'Optional("{key}"): Seq({value}),'
+                f'{INDENTANTION * map_items_indent}Optional("{key}"): Seq({value}),'
             )
 
     return "\n".join(lines)
 
 
-def is_scalar(type_):
+def is_scalar(type_: type) -> bool:
     return inspect.isclass(type_) and issubclass(type_, Scalar)
 
 
-def scalar_to_alfacase_schema(type_, block_indentation):
+def scalar_to_alfacase_schema(type_: type, indent: int) -> str:
     return 'Map({"value": Float(), "unit": Str()})'
 
 
-def is_array(type_):
+def is_array(type_: type) -> bool:
     return inspect.isclass(type_) and issubclass(type_, Array)
 
 
-def array_to_alfacase_schema(type_, block_indentation):
+def array_to_alfacase_schema(type_: type, indent: int) -> str:
     return 'Map({"values": Seq(Float()), "unit": Str()})'
 
 
-def is_int(type_):
-    return inspect.isclass(type_) and issubclass(type_, int)
+def is_curve(type_: type) -> bool:
+    return inspect.isclass(type_) and issubclass(type_, Curve)
+
+
+def curve_to_alfacase_schema(type_: type, indent: int) -> str:
+    map_items_indent = indent + 2
+    array_schema = array_to_alfacase_schema(float, indent=map_items_indent)
+
+    with _map_section([], indent=indent) as lines:
+        lines.append(f'{INDENTANTION * map_items_indent}"image": {array_schema},')
+        lines.append(f'{INDENTANTION * map_items_indent}"domain": {array_schema},')
+
+    return "\n".join(lines)
 
 
-def int_to_alfacase_schema(type_, block_indentation):
+def is_int(type_: type) -> bool:
+    # bool is a subclass of int, but we are not intersted in matching that here.
+    return inspect.isclass(type_) and issubclass(type_, int) and not is_boolean(type_)
+
+
+def int_to_alfacase_schema(type_: type, indent: int) -> str:
     return "Int()"
 
 
-def is_path(type_):
+def is_path(type_: type) -> bool:
     return inspect.isclass(type_) and issubclass(type_, Path)
 
 
-def path_to_alfacase_schema(type_, block_indentation):
+def path_to_alfacase_schema(type_: type, indent: int) -> str:
     return "Str()"
 
 
-LIST_OF_IMPLEMENTATIONS = [
+LIST_OF_IMPLEMENTATIONS: List[typing.Tuple[type, typing.Callable]] = [
     (is_enum, enum_to_alfacase_schema),
     (is_attrs, attrs_to_alfacase_schema),
     (is_list, list_to_alfacase_schema),
     (is_float, float_to_alfacase_schema),
     (is_str, str_to_alfacase_schema),
     (is_boolean, boolean_to_alfacase_schema),
     (is_numpy_1_darray, numpy_1_darray_to_alfacase_schema),
     (is_dict, dict_to_alfacase_schema),
     (is_union, union_to_alfacase_schema),
     (is_scalar, scalar_to_alfacase_schema),
     (is_array, array_to_alfacase_schema),
+    (is_curve, curve_to_alfacase_schema),
     (is_int, int_to_alfacase_schema),
     (is_path, path_to_alfacase_schema),
 ]
 
 
-def _get_attr_value(
-    type_: type, block_indentation: str = INDENTANTION, key: str = "<Unknown>"
-) -> str:
+def _get_attr_value(type_: type, indent: int, key: str = "<Unknown>") -> str:
     """
     Indentation is a parameter used for Union and Dict.
     If the type parameter is a "Optional" type, only the args are used (without the NoneType)
     """
     if is_optional_type(type_):
         referred_type = typing_inspect.get_args(type_, evaluate=True)[0]
         type_ = referred_type
 
     for predicate_function, handle_function in LIST_OF_IMPLEMENTATIONS:
         if predicate_function(type_):
-            return handle_function(
-                type_, block_indentation=block_indentation + INDENTANTION
-            )
+            return handle_function(type_, indent=indent)
+
+    if type_ is typing.Any:
+        return "Any()"
 
     raise RuntimeError(
         f"Alfacase Schema does not know how to handle {type_}.\n"
         f"Perhaps you forgot to add the type hint to attribute named '{key}'?"
     )
 
 
@@ -239,41 +268,37 @@
     return f'"{key}"' if value.default is attr.NOTHING else f'Optional("{key}")'
 
 
 # plugins:
 #   For now, Plugins inputs (GUI) will not be able to be customizable by YAML
 
 IGNORED_PROPERTIES = (
-    "plugins",
-    "table_parameters",
+    "pt_table_parameters",
+    "ph_table_parameters",
     "emulsion_model_plugin_id",
 )
 
 
-def _get_attribute_schema(
-    key: str, value: attr.ib, indentation=INDENTANTION * 2
-) -> str:
+def _get_attribute_schema(key: str, value: attr.ib, indent: int = 2) -> str:
     """
     Helper method that return the equivalent schema for the given key and value.
 
     Keep in mind that for stricyyaml schema, an Optional type means that the user don't need
     to inform a value. While for type hint, an Optional type means that the attribute accepts None.
     """
     if value.default is attr.NOTHING and is_optional_type(value.type):
         msg = (
             "StrictYAML doesn't support None value (only missing keys denote a value), "
             "therefore Optional type are only allowed when the case has a default value."
         )
         raise TypeError(msg)
     attribute_name = _get_attr_name(key, value)
-    attribute_value = _get_attr_value(
-        value.type, block_indentation=indentation, key=key
-    )
+    attribute_value = _get_attr_value(value.type, indent=indent, key=key)
 
-    return indentation + f"{attribute_name}: {attribute_value}" + ","
+    return f"{INDENTANTION * indent}{attribute_name}: {attribute_value}" + ","
 
 
 def generate_alfacase_schema(class_: type) -> str:
     """
     Return a schema for the given `class_` that is decorated with @attr and has type hints.
     """
     lines = [f"{obtain_schema_name(class_)} = Map(", f"{INDENTANTION}{{"]
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/alfacase_to_case.py` & `alfasim_sdk-2024.1/src/alfasim_sdk/_internal/alfacase/alfacase_to_case.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,26 +6,30 @@
 from pathlib import Path
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Type
+from typing import TypeVar
 from typing import Union
 
 import attr
 from attr.validators import instance_of
+from barril.curve.curve import Curve
 from barril.units import Array
 from barril.units import Scalar
 from barril.units import UnitDatabase
 from strictyaml import YAML
 
 from alfasim_sdk._internal import constants
 from alfasim_sdk._internal.alfacase import case_description
 
+T = TypeVar("T")
+
 
 @attr.s
 class DescriptionDocument:
     """
     A class to hold information from the Alfacase file loaded.
 
     :ivar strictyaml.YAML content:
@@ -47,18 +51,19 @@
     @classmethod
     def from_file(cls, file_path: Path) -> "DescriptionDocument":
         """
         Load the values from the given file_path validating against the Schema defined on
         alfacase.schema.case_schema
         """
         import strictyaml
-        from alfasim_sdk._internal.alfacase.schema import case_description_schema
+
         from alfasim_sdk._internal.alfacase.case_description_attributes import (
             DescriptionError,
         )
+        from alfasim_sdk._internal.alfacase.schema import case_description_schema
 
         try:
             content = strictyaml.dirty_load(
                 yaml_string=Path(file_path).read_text(encoding="UTF-8"),
                 schema=case_description_schema,
                 allow_flow_style=True,
             )
@@ -73,15 +78,141 @@
     """
     Return the default category for the given unit
     """
     if unit:
         return UnitDatabase.GetSingleton().GetDefaultCategory(unit)
 
 
-def load_scalar(key: str, alfacase_content: DescriptionDocument, category) -> Scalar:
+def update_multi_input_flags(document: DescriptionDocument, item_description: T) -> T:
+    """
+    Update the multi input flags in `item_description` if not present in `alfacase_content` and
+    can be unambiguously deduced from the presence of constant and transient inputs. If deduction
+    is ambiguous or value is already correct, nothing is changed (no-op).
+
+    :returns: The updated `item_description` (can return `item_description` unchanged).
+    """
+    item_attr_dict = attr.asdict(item_description, recurse=False)
+    fields_to_update: Dict[str, constants.MultiInputType] = {}
+    for key, value in item_attr_dict.items():
+        is_set_in_alfacase = key in document
+        if (not is_set_in_alfacase) and isinstance(value, constants.MultiInputType):
+            assert key.endswith(constants.MULTI_INPUT_TYPE_SUFFIX)
+
+            constant_key = key[: -len(constants.MULTI_INPUT_TYPE_SUFFIX)]
+            has_constant_data = constant_key in document
+
+            curve_key = f"{constant_key}_curve"
+            has_curve_data = curve_key in document
+
+            new_value: Optional[constants.MultiInputType] = None
+            if has_constant_data and not has_curve_data:
+                new_value = constants.MultiInputType.Constant
+            elif has_curve_data and not has_constant_data:
+                new_value = constants.MultiInputType.Curve
+
+            if (new_value is not None) and (
+                getattr(item_description, key) != new_value
+            ):
+                fields_to_update[key] = new_value
+
+    if fields_to_update:
+        item_description = attr.evolve(item_description, **fields_to_update)
+    return item_description
+
+
+@lru_cache(maxsize=None)
+def get_instance_list_loader(*, class_: type) -> Callable:
+    return partial(load_list_of_instance, class_=class_)
+
+
+def load_list_of_instance(
+    alfacase_content: DescriptionDocument, class_: Type[T]
+) -> List[T]:
+    return [
+        load_instance(
+            DescriptionDocument(value, alfacase_content.file_path), class_=class_
+        )
+        for value in alfacase_content.content
+    ]
+
+
+def load_instance(
+    alfacase_content: DescriptionDocument,
+    class_: Type[T],
+    explicit_loaders: Optional[Dict[str, Callable]] = None,
+) -> T:
+    """
+    Create an instance of class_ with the attributes found in alfacase_content.
+    """
+    alfacase_to_case_description = get_case_description_attribute_loader_dict(
+        class_, explicit_loaders=explicit_loaders
+    )
+    case_values = to_case_values(alfacase_content, alfacase_to_case_description)
+    item_description = class_(**case_values)
+    return update_multi_input_flags(alfacase_content, item_description)
+
+
+@lru_cache(maxsize=None)
+def get_instance_loader(*, class_: type) -> Callable:
+    """
+    Return a load instance function pre-populate with the class_.
+    """
+    return partial(load_instance, class_=class_)
+
+
+def load_dict_of_instance(alfacase_content: DescriptionDocument, class_: Type[T]) -> T:
+    return {
+        key.data: load_instance(
+            DescriptionDocument(value, alfacase_content.file_path), class_=class_
+        )
+        for key, value in alfacase_content.content.items()
+    }
+
+
+@lru_cache(maxsize=None)
+def get_dict_of_instance_loader(*, class_: type) -> Callable:
+    return partial(load_dict_of_instance, class_=class_)
+
+
+def get_case_description_attribute_loader_dict(
+    class_: Any, explicit_loaders: Optional[Dict[str, Callable]] = None
+) -> Dict[str, Callable]:
+    """
+    Create a dict of loaders to be used with `to_case_values`.
+
+    Loaders are created for all attributes (``attr.id``) in ``class_``.
+    If ``explicit_loaders`` are supplied those loaders are used instead of the
+    automatically generated ones.
+    """
+    loaders: Dict[str, Callable] = (
+        {} if explicit_loaders is None else explicit_loaders.copy()
+    )
+
+    for attr_instance in attr.fields(class_):
+        name = attr_instance.name
+        if name in loaders:
+            continue
+
+        metadata = attr_instance.metadata
+        if "type" in metadata:
+            kwargs = metadata.copy()
+            type_ = kwargs.pop("type")
+            loader_getter_name = f"get_{type_}_loader"
+            loader = globals()[loader_getter_name]
+            loaders[name] = loader(**kwargs)
+            continue
+
+        loaders[name] = load_value
+
+    return loaders
+
+
+def load_scalar(
+    key: str, alfacase_content: DescriptionDocument, category: str
+) -> Scalar:
     """
     Create a barril.units.Scalar instance from the given alfacase_content.
     # TODO: ASIM-3556: All atributes from this module should get the category from the CaseDescription
     """
     return Scalar(
         category,
         alfacase_content[key]["value"].content.data,
@@ -100,15 +231,15 @@
     the default category for the given unit.
     """
     return partial(
         load_scalar, category=_obtain_category_for_scalar(category, from_unit)
     )
 
 
-def load_array(key: str, alfacase_content: DescriptionDocument, category) -> Array:
+def load_array(key: str, alfacase_content: DescriptionDocument, category: str) -> Array:
     """
     Create a barril.units.Array instance from the given YAML content.
     # TODO: ASIM-3556: All atributes from this module should get the category from the CaseDescription
     """
     return Array(
         category,
         alfacase_content[key]["values"].content.data,
@@ -128,15 +259,17 @@
     """
     return partial(
         load_array, category=_obtain_category_for_scalar(category, from_unit)
     )
 
 
 def load_list_of_arrays(
-    key: str, alfacase_content: DescriptionDocument, category
+    key: str,
+    alfacase_content: DescriptionDocument,
+    category: str,
 ) -> List[Array]:
     """
     Create a barril.units.Array instance from the given YAML content.
     # TODO: ASIM-3556: All atributes from this module should get the category from the CaseDescription
     """
     return [
         Array(category, entry.content.data["values"], entry.content.data["unit"])
@@ -156,16 +289,18 @@
     """
     return partial(
         load_list_of_arrays, category=_obtain_category_for_scalar(category, from_unit)
     )
 
 
 def load_dict_of_arrays(
-    key: str, alfacase_content: DescriptionDocument, category
-) -> Array:
+    key: str,
+    alfacase_content: DescriptionDocument,
+    category: str,
+) -> Dict[str, Array]:
     """
     Create a Dict of str to barril.units.Array instances from the given YAML content.
     # TODO: ASIM-3556: All atributes from this module should get the category from the CaseDescription
     """
     return {
         k: Array(category, v["values"], v["unit"])
         for k, v in alfacase_content[key].content.data.items()
@@ -183,14 +318,82 @@
     the default category for the given unit.
     """
     return partial(
         load_dict_of_arrays, category=_obtain_category_for_scalar(category, from_unit)
     )
 
 
+def load_curve(
+    key: str,
+    alfacase_content: DescriptionDocument,
+    category: str,
+    domain_category: str = "time",
+) -> Curve:
+    """
+    Create a barril.curve.curve.Curve instance from the given YAML content.
+    # TODO: ASIM-3556: All atributes from this module should get the category from the CaseDescription
+    """
+    curve_in_alfacase = alfacase_content[key]
+    return Curve(
+        load_array("image", curve_in_alfacase, category),
+        load_array("domain", curve_in_alfacase, domain_category),
+    )
+
+
+@lru_cache(maxsize=None)
+def get_curve_loader(
+    *,
+    category: Optional[str] = None,
+    from_unit: Optional[str] = None,
+    domain_category: Optional[str] = None,
+    from_domain_unit: Optional[str] = None,
+) -> Callable:
+    """
+    Return a load_curve function pre-populated with the category
+
+    If ``from_unit`` is provided, the category parameter will be filled with
+    the default category for the given unit.
+    """
+    args = dict(category=_obtain_category_for_scalar(category, from_unit))
+    if domain_category is not None or from_domain_unit is not None:
+        args["domain_category"] = _obtain_category_for_scalar(
+            domain_category, from_domain_unit
+        )
+    return partial(load_curve, **args)
+
+
+def load_dict_of_curves(
+    key: str, alfacase_content: DescriptionDocument, category: str
+) -> Dict[str, Curve]:
+    """
+    Create a Dict of str to barril.curve.curve.Curve instances from the given YAML content.
+    # TODO: ASIM-3556: All atributes from this module should get the category from the CaseDescription
+    """
+    curve_dict_in_alfacase = alfacase_content[key]
+    return {
+        k: load_curve(k, curve_dict_in_alfacase, category)
+        for k in curve_dict_in_alfacase.content.data.keys()
+    }
+
+
+@lru_cache(maxsize=None)
+def get_curve_dict_loader(
+    *, category: Optional[str] = None, from_unit: Optional[str] = None
+) -> Callable:
+    """
+    Return a load_dict_of_curves function pre-populated with the category
+
+    If ``from_unit`` is provided, the category parameter will be filled with
+    the default category for the given unit.
+    """
+    return partial(
+        load_dict_of_curves, category=_obtain_category_for_scalar(category, from_unit)
+    )
+
+
 def _obtain_category_for_scalar(category: str, from_unit: str) -> str:
     """
     Obtain the category to be used for GetArrayLoader and GetScalarLoader.
 
     Raises ValueError with either category and from_unit are defined, and also raises ValueError if
     neither category or from_unit are defined.
     """
@@ -201,23 +404,25 @@
     if category is None and from_unit is None:
         raise ValueError("Either 'category' or 'from_unit' parameter must be defined")
 
     return category or get_category_for(from_unit)
 
 
 def load_dict_with_scalar(
-    key: str, alfacase_content: DescriptionDocument, category
+    key: str,
+    alfacase_content: DescriptionDocument,
+    category: str,
 ) -> Dict[str, Scalar]:
     return {
         key: Scalar(category, value["value"], value["unit"])
         for key, value in alfacase_content[key].content.data.items()
     }
 
 
-def get_dict_with_scalar_loader(*, category: str) -> Callable:
+def get_scalar_dict_loader(*, category: str) -> Callable:
     """
     Return a LoadDictWithScalar function pre-populate with the category
     """
     return partial(load_dict_with_scalar, category=category)
 
 
 def load_enum(
@@ -256,14 +461,15 @@
     )
 
 
 PvtModelTable = str
 PvtModels = Union[
     PvtModelTable,
     case_description.PvtModelCompositionalDescription,
+    case_description.PvtModelCombinedDescription,
     case_description.PvtModelCorrelationDescription,
 ]
 
 
 def load_pvt_tables(alfacase_content: DescriptionDocument) -> Dict[str, Path]:
     def get_table_file(value):
         """
@@ -313,17 +519,22 @@
         "gas_density_std": get_scalar_loader(from_unit="kg/m3"),
         "rs_sat": get_scalar_loader(from_unit="sm3/sm3"),
         "pvt_correlation_package": get_enum_loader(
             enum_class=constants.CorrelationPackage
         ),
     }
 
-    def generate_pvt_model_correlation(value: DescriptionDocument):
+    def generate_pvt_model_correlation(
+        value: DescriptionDocument,
+    ) -> case_description.PvtModelCorrelationDescription:
         case_values = to_case_values(value, alfacase_to_case_description)
-        return case_description.PvtModelCorrelationDescription(**case_values)
+        item_description = case_description.PvtModelCorrelationDescription(
+            **case_values
+        )
+        return update_multi_input_flags(document, item_description)
 
     return {
         key.data: generate_pvt_model_correlation(
             DescriptionDocument(value, document.file_path)
         )
         for key, value in document.content.items()
     }
@@ -337,15 +548,16 @@
         "scn": load_value,
         "MW": get_scalar_loader(from_unit="kg/mol"),
         "rho": get_scalar_loader(from_unit="kg/m3"),
     }
 
     def generate_heavy_components_description(document: DescriptionDocument):
         case_values = to_case_values(document, alfacase_to_case_description)
-        return case_description.HeavyComponentDescription(**case_values)
+        item_description = case_description.HeavyComponentDescription(**case_values)
+        return update_multi_input_flags(document, item_description)
 
     return [
         generate_heavy_components_description(alfacase_document)
         for alfacase_document in document
     ]
 
 
@@ -366,15 +578,16 @@
         "Cp_2": get_scalar_loader(from_unit="-"),
         "Cp_3": get_scalar_loader(from_unit="-"),
         "Cp_4": get_scalar_loader(from_unit="-"),
     }
 
     def generate_light_components_description(document: DescriptionDocument):
         case_values = to_case_values(document, alfacase_to_case_description)
-        return case_description.LightComponentDescription(**case_values)
+        item_description = case_description.LightComponentDescription(**case_values)
+        return update_multi_input_flags(document, item_description)
 
     return [
         generate_light_components_description(alfacase_document)
         for alfacase_document in document
     ]
 
 
@@ -385,15 +598,16 @@
         "component_1": load_value,
         "component_2": load_value,
         "value": load_value,
     }
 
     def generate_bip_description(alfacase_document: DescriptionDocument):
         case_values = to_case_values(alfacase_document, alfacase_to_case_description)
-        return case_description.BipDescription(**case_values)
+        item_description = case_description.BipDescription(**case_values)
+        return update_multi_input_flags(document, item_description)
 
     return [
         generate_bip_description(alfacase_document) for alfacase_document in document
     ]
 
 
 def load_composition_description(
@@ -403,35 +617,37 @@
         "component": load_value,
         "molar_fraction": get_scalar_loader(from_unit="mol/mol"),
         "reference_enthalpy": get_scalar_loader(from_unit="J/mol"),
     }
 
     def generate_composition_description(document: DescriptionDocument):
         case_values = to_case_values(document, alfacase_to_case_description)
-        return case_description.CompositionDescription(**case_values)
+        item_description = case_description.CompositionDescription(**case_values)
+        return update_multi_input_flags(document, item_description)
 
     return [
         generate_composition_description(alfacase_document)
         for alfacase_document in document
     ]
 
 
-def load_fluid_description(
+def load_compositional_fluid_description(
     document: DescriptionDocument,
-) -> Dict[str, case_description.FluidDescription]:
+) -> Dict[str, case_description.CompositionalFluidDescription]:
     alfacase_to_case_description = {
         "composition": load_composition_description,
         "fraction_pairs": load_bip_description,
     }
 
     def generate_fluid_description(
         value: DescriptionDocument,
-    ) -> case_description.FluidDescription:
+    ) -> case_description.CompositionalFluidDescription:
         case_values = to_case_values(value, alfacase_to_case_description)
-        return case_description.FluidDescription(**case_values)
+        item_description = case_description.CompositionalFluidDescription(**case_values)
+        return update_multi_input_flags(document, item_description)
 
     return {
         key.data: generate_fluid_description(
             DescriptionDocument(value, document.file_path)
         )
         for key, value in document.content.items()
     }
@@ -448,40 +664,52 @@
             enum_class=constants.SurfaceTensionType
         ),
         "viscosity_model": get_enum_loader(
             enum_class=constants.PVTCompositionalViscosityModel
         ),
         "heavy_components": load_heavy_component_description,
         "light_components": load_light_component_description,
-        "fluids": load_fluid_description,
+        "fluids": load_compositional_fluid_description,
     }
 
     def generate_pvt_model_compositional(value: DescriptionDocument):
         case_values = to_case_values(value, alfacase_to_case_description)
-        return case_description.PvtModelCompositionalDescription(**case_values)
+        item_description = case_description.PvtModelCompositionalDescription(
+            **case_values
+        )
+        return update_multi_input_flags(document, item_description)
 
     return {
         key.data: generate_pvt_model_compositional(
             DescriptionDocument(value, document.file_path)
         )
         for key, value in document.content.items()
     }
 
 
+def load_combined_fluid_description(
+    document: DescriptionDocument,
+) -> Dict[str, case_description.CombinedFluidDescription]:
+    return load_dict_of_instance(document, case_description.CombinedFluidDescription)
+
+
+def load_pvt_model_combined_description(
+    document: DescriptionDocument,
+) -> Dict[str, case_description.PvtModelCombinedDescription]:
+    return load_dict_of_instance(document, case_description.PvtModelCombinedDescription)
+
+
 def load_pvt_models_description(
     document: DescriptionDocument,
 ) -> case_description.PvtModelsDescription:
-    alfacase_to_case_description = {
-        "default_model": load_value,
-        "tables": load_pvt_tables,
-        "correlations": load_pvt_model_correlation_description,
-        "compositions": load_pvt_model_compositional_description,
-    }
-    case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.PvtModelsDescription(**case_values)
+    return load_instance(
+        document,
+        case_description.PvtModelsDescription,
+        explicit_loaders={"tables": load_pvt_tables},
+    )
 
 
 # Used for testing - Will be ignored on the document contents
 IGNORE_KEY = "IgnoreKey"
 
 
 def to_case_values(
@@ -524,17 +752,17 @@
 def load_casing_section_description(
     document: DescriptionDocument,
 ) -> List[case_description.CasingSectionDescription]:
     alfacase_to_case_description = {
         "name": load_value,
         "hanger_depth": get_scalar_loader(from_unit="m"),
         "settings_depth": get_scalar_loader(from_unit="m"),
-        "hole_diameter": get_scalar_loader(from_unit="m"),
-        "outer_diameter": get_scalar_loader(from_unit="m"),
-        "inner_diameter": get_scalar_loader(from_unit="m"),
+        "hole_diameter": get_scalar_loader(category="diameter"),
+        "outer_diameter": get_scalar_loader(category="diameter"),
+        "inner_diameter": get_scalar_loader(category="diameter"),
         "inner_roughness": get_scalar_loader(from_unit="m"),
         "material": load_value,
         "top_of_filler": get_scalar_loader(from_unit="m"),
         "filler_material": load_value,
         "material_above_filler": load_value,
     }
 
@@ -544,41 +772,34 @@
 
     return [
         generate_casing_section_description(alfacase_document)
         for alfacase_document in document
     ]
 
 
-def load_cv_table_description(
-    document: DescriptionDocument,
-) -> case_description.CvTableDescription:
-    alfacase_to_case_description = {
-        "opening": get_array_loader(from_unit="-"),
-        "flow_coefficient": get_array_loader(from_unit="(galUS/min)/(psi^0.5)"),
-    }
-    case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.CvTableDescription(**case_values)
-
-
 def load_environment_property_description(
     document: DescriptionDocument,
 ) -> List[case_description.EnvironmentPropertyDescription]:
     # fmt: off
     alfacase_to_case_description = {
         'type': get_enum_loader(enum_class=constants.PipeEnvironmentHeatTransferCoefficientModelType),
         'position': get_scalar_loader(from_unit='m'),
         'temperature': get_scalar_loader(from_unit='degC'),
         'heat_transfer_coefficient': get_scalar_loader(from_unit='W/m2.K'),
         'overall_heat_transfer_coefficient': get_scalar_loader(from_unit='W/m2.K'),
         'fluid_velocity': get_scalar_loader(from_unit='m/s'),
     }
+
     # fmt: on
     def generate_environment_property_description(document: DescriptionDocument):
         case_values = to_case_values(document, alfacase_to_case_description)
-        return case_description.EnvironmentPropertyDescription(**case_values)
+        item_description = case_description.EnvironmentPropertyDescription(
+            **case_values
+        )
+        return update_multi_input_flags(document, item_description)
 
     return [
         generate_environment_property_description(alfacase_document)
         for alfacase_document in document
     ]
 
 
@@ -589,59 +810,63 @@
         "name": load_value,
         "start": get_scalar_loader(from_unit="m"),
         "material": load_value,
     }
 
     def generate_formation_layer_description(document: DescriptionDocument):
         case_values = to_case_values(document, alfacase_to_case_description)
-        return case_description.FormationLayerDescription(**case_values)
+        item_description = case_description.FormationLayerDescription(**case_values)
+        return update_multi_input_flags(document, item_description)
 
     return [
         generate_formation_layer_description(alfacase_document)
         for alfacase_document in document
     ]
 
 
 def load_gas_lift_valve_equipment_description(
     document: DescriptionDocument,
 ) -> Dict[str, case_description.GasLiftValveEquipmentDescription]:
     alfacase_to_case_description = {
         "name": load_value,
         "position": get_scalar_loader(from_unit="m"),
-        "diameter": get_scalar_loader(from_unit="m"),
+        "diameter": get_scalar_loader(category="diameter"),
         "valve_type": get_enum_loader(enum_class=constants.ValveType),
         "delta_p_min": get_scalar_loader(from_unit="Pa"),
-        "discharge_coeff": get_scalar_loader(from_unit="-"),
+        "discharge_coefficient": get_scalar_loader(from_unit="-"),
     }
 
     def generate_gas_lift_description(document: DescriptionDocument):
         case_values = to_case_values(document, alfacase_to_case_description)
-        return case_description.GasLiftValveEquipmentDescription(**case_values)
+        item_description = case_description.GasLiftValveEquipmentDescription(
+            **case_values
+        )
+        return update_multi_input_flags(document, item_description)
 
     return {
         key.data: generate_gas_lift_description(
             DescriptionDocument(value, document.file_path)
         )
         for key, value in document.content.items()
     }
 
 
 def load_heat_source_equipment_description(
     document: DescriptionDocument,
 ) -> Dict[str, case_description.HeatSourceEquipmentDescription]:
-    alfacase_to_case_description = {
-        "name": load_value,
-        "start": get_scalar_loader(from_unit="m"),
-        "length": get_scalar_loader(from_unit="m"),
-        "power": get_scalar_loader(from_unit="W"),
-    }
+    alfacase_to_case_description = get_case_description_attribute_loader_dict(
+        case_description.HeatSourceEquipmentDescription
+    )
 
     def generate_heat_source_description(document: DescriptionDocument):
         case_values = to_case_values(document, alfacase_to_case_description)
-        return case_description.HeatSourceEquipmentDescription(**case_values)
+        item_description = case_description.HeatSourceEquipmentDescription(
+            **case_values
+        )
+        return update_multi_input_flags(document, item_description)
 
     return {
         key.data: generate_heat_source_description(
             DescriptionDocument(value, document.file_path)
         )
         for key, value in document.content.items()
     }
@@ -712,15 +937,16 @@
     alfacase_to_case_description = {
         "position_input_type": get_enum_loader(enum_class=constants.TableInputType),
         "table_x": load_referenced_velocities_container_description,
         "table_y": load_referenced_velocities_container_description,
         "table_length": load_velocities_container_description,
     }
     case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.InitialVelocitiesDescription(**case_values)
+    item_description = case_description.InitialVelocitiesDescription(**case_values)
+    return update_multi_input_flags(document, item_description)
 
 
 load_referenced_temperatures_container_description = (
     get_initial_conditions_table_loader(
         case_description.ReferencedTemperaturesContainerDescription,
         "temperatures",
         "K",
@@ -743,15 +969,16 @@
     alfacase_to_case_description = {
         "position_input_type": get_enum_loader(enum_class=constants.TableInputType),
         "table_x": load_referenced_temperatures_container_description,
         "table_y": load_referenced_temperatures_container_description,
         "table_length": load_temperatures_container_description,
     }
     case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.InitialTemperaturesDescription(**case_values)
+    item_description = case_description.InitialTemperaturesDescription(**case_values)
+    return update_multi_input_flags(document, item_description)
 
 
 load_referenced_volume_fractions_container_description = (
     get_initial_conditions_table_loader(
         case_description.ReferencedVolumeFractionsContainerDescription,
         "fractions",
         "-",
@@ -774,15 +1001,16 @@
     alfacase_to_case_description = {
         "position_input_type": get_enum_loader(enum_class=constants.TableInputType),
         "table_x": load_referenced_volume_fractions_container_description,
         "table_y": load_referenced_volume_fractions_container_description,
         "table_length": load_volume_fractions_container_description,
     }
     case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.InitialVolumeFractionsDescription(**case_values)
+    item_description = case_description.InitialVolumeFractionsDescription(**case_values)
+    return update_multi_input_flags(document, item_description)
 
 
 load_referenced_pressure_container_description = get_initial_conditions_table_loader(
     case_description.ReferencedPressureContainerDescription,
     "pressures",
     "Pa",
     is_referenced=True,
@@ -803,15 +1031,16 @@
     alfacase_to_case_description = {
         "position_input_type": get_enum_loader(enum_class=constants.TableInputType),
         "table_x": load_referenced_pressure_container_description,
         "table_y": load_referenced_pressure_container_description,
         "table_length": load_pressure_container_description,
     }
     case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.InitialPressuresDescription(**case_values)
+    item_description = case_description.InitialPressuresDescription(**case_values)
+    return update_multi_input_flags(document, item_description)
 
 
 load_referenced_tracers_mass_fractions_container_description = (
     get_tracers_initial_conditions_table_loader(
         case_description.ReferencedTracersMassFractionsContainerDescription,
         "tracers_mass_fractions",
         "-",
@@ -834,61 +1063,58 @@
     alfacase_to_case_description = {
         "position_input_type": get_enum_loader(enum_class=constants.TableInputType),
         "table_x": load_referenced_tracers_mass_fractions_container_description,
         "table_y": load_referenced_tracers_mass_fractions_container_description,
         "table_length": load_tracers_mass_fractions_container_description,
     }
     case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.InitialTracersMassFractionsDescription(**case_values)
+    item_description = case_description.InitialTracersMassFractionsDescription(
+        **case_values
+    )
+    return update_multi_input_flags(document, item_description)
 
 
 def load_initial_conditions_description(
     document: DescriptionDocument,
 ) -> case_description.InitialConditionsDescription:
     alfacase_to_case_description = {
         "velocities": load_initial_velocities_description,
         "temperatures": load_initial_temperatures_description,
         "volume_fractions": load_initial_volume_fractions_description,
         "pressures": load_initial_pressures_description,
         "tracers_mass_fractions": load_initial_tracers_mass_fractions_description,
         "fluid": load_value,
     }
     case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.InitialConditionsDescription(**case_values)
+    item_description = case_description.InitialConditionsDescription(**case_values)
+    return update_multi_input_flags(document, item_description)
 
 
 def _load_mass_source_common() -> Dict[str, Callable]:
-    return {
-        "fluid": load_value,
-        "temperature": get_scalar_loader(from_unit="K"),
-        "tracer_mass_fraction": get_array_loader(category="mass fraction"),
-        "water_cut": get_scalar_loader(category="volume fraction"),
-        "gas_oil_ratio": get_scalar_loader(from_unit="sm3/sm3"),
-        "source_type": get_enum_loader(enum_class=constants.MassSourceType),
-        "volumetric_flow_rates_std": get_dict_with_scalar_loader(
-            category="standard volume per time"
-        ),
-        "mass_flow_rates": get_dict_with_scalar_loader(category="mass flow rate"),
-        "total_mass_flow_rate": get_scalar_loader(from_unit="kg/s"),
-    }
+    return get_case_description_attribute_loader_dict(
+        case_description._MassSourceCommon
+    )
 
 
 def load_mass_source_equipment_description(
     document: DescriptionDocument,
 ) -> Dict[str, case_description.MassSourceEquipmentDescription]:
     alfacase_to_case_description = {
         "name": load_value,
         "position": get_scalar_loader(from_unit="m"),
         "material_above_filler": load_value,
     }
     alfacase_to_case_description.update(**_load_mass_source_common())
 
     def generate_mass_source_description(document: DescriptionDocument):
         case_values = to_case_values(document, alfacase_to_case_description)
-        return case_description.MassSourceEquipmentDescription(**case_values)
+        item_description = case_description.MassSourceEquipmentDescription(
+            **case_values
+        )
+        return update_multi_input_flags(document, item_description)
 
     return {
         key.data: generate_mass_source_description(
             DescriptionDocument(value, document.file_path)
         )
         for key, value in document.content.items()
     }
@@ -907,111 +1133,114 @@
         "outer_emissivity": get_scalar_loader(category="emissivity"),
         "expansion": get_scalar_loader(from_unit="1/K"),
         "viscosity": get_scalar_loader(from_unit="cP"),
     }
 
     def generate_materials_description(document: DescriptionDocument):
         case_values = to_case_values(document, alfacase_to_case_description)
-        return case_description.MaterialDescription(**case_values)
+        item_description = case_description.MaterialDescription(**case_values)
+        return update_multi_input_flags(document, item_description)
 
     return [
         generate_materials_description(alfacase_document)
         for alfacase_document in document
     ]
 
 
 def load_internal_node_properties_description(
     document: DescriptionDocument,
 ) -> case_description.InternalNodePropertiesDescription:
     alfacase_to_case_description = {"fluid": load_value}
     case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.InternalNodePropertiesDescription(**case_values)
+    item_description = case_description.InternalNodePropertiesDescription(**case_values)
+    return update_multi_input_flags(document, item_description)
 
 
 def load_mass_source_node_properties_description(
     document: DescriptionDocument,
 ) -> case_description.MassSourceNodePropertiesDescription:
     case_values = to_case_values(document, _load_mass_source_common())
-    return case_description.MassSourceNodePropertiesDescription(**case_values)
+    item_description = case_description.MassSourceNodePropertiesDescription(
+        **case_values
+    )
+    return update_multi_input_flags(document, item_description)
 
 
 def load_pressure_node_properties_description(
     document: DescriptionDocument,
 ) -> case_description.PressureNodePropertiesDescription:
     case_values = to_case_values(document, _load_pressure_source_common())
-    return case_description.PressureNodePropertiesDescription(**case_values)
+    item_description = case_description.PressureNodePropertiesDescription(**case_values)
+    return update_multi_input_flags(document, item_description)
 
 
 def load_separator_node_properties_description(
     document: DescriptionDocument,
 ) -> case_description.SeparatorNodePropertiesDescription:
     alfacase_to_case_description = {
         "environment_temperature": get_scalar_loader(from_unit="K"),
         "geometry": get_enum_loader(enum_class=constants.SeparatorGeometryType),
         "length": get_scalar_loader(from_unit="m"),
         "overall_heat_transfer_coefficient": get_scalar_loader(from_unit="W/m2.K"),
-        "diameter": get_scalar_loader(from_unit="m"),
-        "nozzles": get_dict_with_scalar_loader(category=get_category_for("m")),
-        "initial_phase_volume_fractions": get_dict_with_scalar_loader(
+        "diameter": get_scalar_loader(category="diameter"),
+        "nozzles": get_scalar_dict_loader(category=get_category_for("m")),
+        "initial_phase_volume_fractions": get_scalar_dict_loader(
             category="volume fraction"
         ),
         "gas_separation_efficiency": get_scalar_loader(from_unit="%"),
         "liquid_separation_efficiency": get_scalar_loader(from_unit="%"),
     }
     case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.SeparatorNodePropertiesDescription(**case_values)
+    item_description = case_description.SeparatorNodePropertiesDescription(
+        **case_values
+    )
+    return update_multi_input_flags(document, item_description)
 
 
 def load_node_description(
     document: DescriptionDocument,
 ) -> List[case_description.NodeDescription]:
     alfacase_to_case_description = {
         "name": load_value,
         "node_type": get_enum_loader(enum_class=constants.NodeCellType),
         "pvt_model": load_value,
         "pressure_properties": load_pressure_node_properties_description,
         "mass_source_properties": load_mass_source_node_properties_description,
         "internal_properties": load_internal_node_properties_description,
         "separator_properties": load_separator_node_properties_description,
+        "controller_properties": get_instance_loader(
+            class_=case_description.ControllerNodePropertiesDescription
+        ),
     }
 
     def generate_node_description(
         document: DescriptionDocument,
     ) -> case_description.NodeDescription:
         case_values = to_case_values(document, alfacase_to_case_description)
-        return case_description.NodeDescription(**case_values)
+        item_description = case_description.NodeDescription(**case_values)
+        return update_multi_input_flags(document, item_description)
 
     return [
         generate_node_description(alfacase_document) for alfacase_document in document
     ]
 
 
-def load_opening_curve_description(
-    document: DescriptionDocument,
-) -> case_description.OpeningCurveDescription:
-    alfacase_to_case_description = {
-        "time": get_array_loader(from_unit="s"),
-        "opening": get_array_loader(from_unit="-"),
-    }
-    case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.OpeningCurveDescription(**case_values)
-
-
 def load_packer_description(
     document: DescriptionDocument,
 ) -> List[case_description.PackerDescription]:
     alfacase_to_case_description = {
         "name": load_value,
         "position": get_scalar_loader(from_unit="m"),
         "material_above": load_value,
     }
 
     def generate_packer_description(document: DescriptionDocument):
         case_values = to_case_values(document, alfacase_to_case_description)
-        return case_description.PackerDescription(**case_values)
+        item_description = case_description.PackerDescription(**case_values)
+        return update_multi_input_flags(document, item_description)
 
     return [
         generate_packer_description(alfacase_document) for alfacase_document in document
     ]
 
 
 def load_pipe_segments_description(
@@ -1020,15 +1249,16 @@
     alfacase_to_case_description = {
         "start_positions": get_array_loader(from_unit="m"),
         "diameters": get_array_loader(from_unit="m"),
         "roughnesses": get_array_loader(from_unit="m"),
         "wall_names": load_value,
     }
     case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.PipeSegmentsDescription(**case_values)
+    item_description = case_description.PipeSegmentsDescription(**case_values)
+    return update_multi_input_flags(document, item_description)
 
 
 def load_profile_output_description(
     document: DescriptionDocument,
 ) -> List[case_description.ProfileOutputDescription]:
     alfacase_to_case_description = {
         "curve_names": load_value,
@@ -1036,65 +1266,89 @@
         "location": get_enum_loader(enum_class=constants.OutputAttachmentLocation),
     }
 
     def generate_profile_definitions(
         document: DescriptionDocument,
     ) -> case_description.ProfileOutputDescription:
         case_values = to_case_values(document, alfacase_to_case_description)
-        return case_description.ProfileOutputDescription(**case_values)
+        item_description = case_description.ProfileOutputDescription(**case_values)
+        return update_multi_input_flags(document, item_description)
 
     return [
         generate_profile_definitions(alfacase_document)
         for alfacase_document in document
     ]
 
 
 def load_linear_ipr_description(
     document: DescriptionDocument,
 ) -> Dict[str, case_description.LinearIPRDescription]:
-    alfacase_to_case_description = {
-        "well_index_phase": get_enum_loader(enum_class=constants.WellIndexPhaseType),
-        "min_pressure_difference": get_scalar_loader(from_unit="Pa"),
-        "well_index": get_scalar_loader(from_unit="m3/bar.d"),
-    }
+    alfacase_to_case_description = get_case_description_attribute_loader_dict(
+        case_description.LinearIPRDescription
+    )
 
     def generate_linear_ipr_correlation(value: DescriptionDocument):
         case_values = to_case_values(value, alfacase_to_case_description)
-        return case_description.LinearIPRDescription(**case_values)
+        item_description = case_description.LinearIPRDescription(**case_values)
+        return update_multi_input_flags(document, item_description)
 
     return {
         key.data: generate_linear_ipr_correlation(
             DescriptionDocument(value, document.file_path)
         )
         for key, value in document.content.items()
     }
 
 
+def load_vogel_ipr_description(
+    document: DescriptionDocument,
+) -> Dict[str, case_description.VogelIPRDescription]:
+    return load_dict_of_instance(document, class_=case_description.VogelIPRDescription)
+
+
+def load_fetkovich_ipr_description(
+    document: DescriptionDocument,
+) -> Dict[str, case_description.FetkovichIPRDescription]:
+    return load_dict_of_instance(
+        document, class_=case_description.FetkovichIPRDescription
+    )
+
+
+def load_forchheimer_ipr_description(
+    document: DescriptionDocument,
+) -> Dict[str, case_description.ForchheimerIPRDescription]:
+    return load_dict_of_instance(
+        document, class_=case_description.ForchheimerIPRDescription
+    )
+
+
 def load_ipr_curve_description(
     document: DescriptionDocument,
 ) -> case_description.IPRCurveDescription:
     alfacase_to_case_description = {
         "pressure_difference": get_array_loader(from_unit="Pa"),
         "flow_rate": get_array_loader(from_unit="sm3/d"),
     }
     case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.IPRCurveDescription(**case_values)
+    item_description = case_description.IPRCurveDescription(**case_values)
+    return update_multi_input_flags(document, item_description)
 
 
 def load_table_ipr_description(
     document: DescriptionDocument,
 ) -> Dict[str, case_description.LinearIPRDescription]:
     alfacase_to_case_description = {
         "well_index_phase": get_enum_loader(enum_class=constants.WellIndexPhaseType),
         "table": load_ipr_curve_description,
     }
 
     def generate_table_ipr_correlation(value: DescriptionDocument):
         case_values = to_case_values(value, alfacase_to_case_description)
-        return case_description.TableIPRDescription(**case_values)
+        item_description = case_description.TableIPRDescription(**case_values)
+        return update_multi_input_flags(document, item_description)
 
     return {
         key.data: generate_table_ipr_correlation(
             DescriptionDocument(value, document.file_path)
         )
         for key, value in document.content.items()
     }
@@ -1102,32 +1356,27 @@
 
 def load_ipr_models_description(
     document: DescriptionDocument,
 ) -> case_description.IPRModelsDescription:
     alfacase_to_case_description = {
         "linear_models": load_linear_ipr_description,
         "table_models": load_table_ipr_description,
+        "vogel_models": load_vogel_ipr_description,
+        "fetkovich_models": load_fetkovich_ipr_description,
+        "forchheimer_models": load_forchheimer_ipr_description,
     }
     case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.IPRModelsDescription(**case_values)
+    item_description = case_description.IPRModelsDescription(**case_values)
+    return update_multi_input_flags(document, item_description)
 
 
 def _load_pressure_source_common() -> Dict[str, Callable]:
-    return {
-        "fluid": load_value,
-        "tracer_mass_fraction": get_array_loader(category="mass fraction"),
-        "split_type": get_enum_loader(enum_class=constants.MassInflowSplitType),
-        "mass_fractions": get_dict_with_scalar_loader(category="mass fraction"),
-        "volume_fractions": get_dict_with_scalar_loader(category="volume fraction"),
-        "water_cut": get_scalar_loader(category="volume fraction"),
-        "gas_oil_ratio": get_scalar_loader(from_unit="sm3/sm3"),
-        "gas_liquid_ratio": get_scalar_loader(from_unit="sm3/sm3"),
-        "pressure": get_scalar_loader(from_unit="bar"),
-        "temperature": get_scalar_loader(from_unit="K"),
-    }
+    return get_case_description_attribute_loader_dict(
+        case_description._PressureSourceCommon
+    )
 
 
 def load_reservoir_inflow_equipment_description(
     document: DescriptionDocument,
 ) -> Dict[str, case_description.ReservoirInflowEquipmentDescription]:
     alfacase_to_case_description = {
         "name": load_value,
@@ -1140,15 +1389,18 @@
         "injectivity_ipr": load_value,
         "tracer_mass_fraction": get_array_loader(category="mass fraction"),
     }
     alfacase_to_case_description.update(**_load_pressure_source_common())
 
     def generate_reservoir_inflow_description(document: DescriptionDocument):
         case_values = to_case_values(document, alfacase_to_case_description)
-        return case_description.ReservoirInflowEquipmentDescription(**case_values)
+        item_description = case_description.ReservoirInflowEquipmentDescription(
+            **case_values
+        )
+        return update_multi_input_flags(document, item_description)
 
     return {
         key.data: generate_reservoir_inflow_description(
             DescriptionDocument(value, document.file_path)
         )
         for key, value in document.content.items()
     }
@@ -1158,66 +1410,162 @@
     document: DescriptionDocument,
 ) -> case_description.SpeedCurveDescription:
     alfacase_to_case_description = {
         "time": get_array_loader(from_unit="s"),
         "speed": get_array_loader(from_unit="rpm"),
     }
     case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.SpeedCurveDescription(**case_values)
+    item_description = case_description.SpeedCurveDescription(**case_values)
+    return update_multi_input_flags(document, item_description)
 
 
 def load_table_pump_description(
     document: DescriptionDocument,
 ) -> case_description.TablePumpDescription:
     alfacase_to_case_description = {
         "speeds": get_array_loader(from_unit="rpm"),
         "void_fractions": get_array_loader(category="volume fraction"),
         "flow_rates": get_array_loader(category="volume flow rate"),
         "pressure_boosts": get_array_loader(from_unit="bar"),
+        "heads": get_array_loader(from_unit="m"),
+        "efficiencies": get_array_loader(from_unit="%"),
+        "powers": get_array_loader(from_unit="W"),
     }
     case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.TablePumpDescription(**case_values)
+    item_description = case_description.TablePumpDescription(**case_values)
+    return update_multi_input_flags(document, item_description)
+
+
+def generate_trend_description(
+    document: DescriptionDocument,
+    alfacase_to_case_description: Dict[str, Callable],
+    description_type: [T],
+) -> [T]:
+    case_values = to_case_values(document, alfacase_to_case_description)
+    item_description = description_type(**case_values)
+    return update_multi_input_flags(document, item_description)
 
 
-def load_trend_output_description(
+def load_positional_pipe_trend_description(
     document: DescriptionDocument,
-) -> List[case_description.TrendOutputDescription]:
+) -> List[case_description.PositionalPipeTrendDescription]:
+    alfacase_to_case_description = get_case_description_attribute_loader_dict(
+        case_description.PositionalPipeTrendDescription
+    )
+    return [
+        generate_trend_description(
+            alfacase_document,
+            alfacase_to_case_description,
+            case_description.PositionalPipeTrendDescription,
+        )
+        for alfacase_document in document
+    ]
+
+
+def load_equipment_trend_description(
+    document: DescriptionDocument,
+) -> List[case_description.EquipmentTrendDescription]:
     alfacase_to_case_description = {
         "curve_names": load_value,
-        "location": get_enum_loader(enum_class=constants.OutputAttachmentLocation),
         "element_name": load_value,
-        "position": get_scalar_loader(from_unit="m"),
     }
+    return [
+        generate_trend_description(
+            alfacase_document,
+            alfacase_to_case_description,
+            case_description.EquipmentTrendDescription,
+        )
+        for alfacase_document in document
+    ]
 
-    def generate_trend_description(
-        document: DescriptionDocument,
-    ) -> case_description.TrendOutputDescription:
-        case_values = to_case_values(document, alfacase_to_case_description)
-        return case_description.TrendOutputDescription(**case_values)
 
+def load_separator_trend_description(
+    document: DescriptionDocument,
+) -> List[case_description.SeparatorTrendDescription]:
+    alfacase_to_case_description = {
+        "curve_names": load_value,
+        "element_name": load_value,
+    }
+    return [
+        generate_trend_description(
+            alfacase_document,
+            alfacase_to_case_description,
+            case_description.SeparatorTrendDescription,
+        )
+        for alfacase_document in document
+    ]
+
+
+def load_controller_trend_description(
+    document: DescriptionDocument,
+) -> List[case_description.ControllerTrendDescription]:
+    alfacase_to_case_description = {
+        "curve_names": load_value,
+        "element_name": load_value,
+    }
+    return [
+        generate_trend_description(
+            alfacase_document,
+            alfacase_to_case_description,
+            case_description.ControllerTrendDescription,
+        )
+        for alfacase_document in document
+    ]
+
+
+def load_global_trend_description(
+    document: DescriptionDocument,
+) -> List[case_description.GlobalTrendDescription]:
+    alfacase_to_case_description = {
+        "curve_names": load_value,
+    }
     return [
-        generate_trend_description(alfacase_document) for alfacase_document in document
+        generate_trend_description(
+            alfacase_document,
+            alfacase_to_case_description,
+            case_description.GlobalTrendDescription,
+        )
+        for alfacase_document in document
+    ]
+
+
+def load_overall_pipe_trend_description(
+    document: DescriptionDocument,
+) -> List[case_description.OverallPipeTrendDescription]:
+    alfacase_to_case_description = {
+        "curve_names": load_value,
+        "element_name": load_value,
+        "location": get_enum_loader(enum_class=constants.OutputAttachmentLocation),
+    }
+    return [
+        generate_trend_description(
+            alfacase_document,
+            alfacase_to_case_description,
+            case_description.OverallPipeTrendDescription,
+        )
+        for alfacase_document in document
     ]
 
 
 def load_tubing_description(
     document: DescriptionDocument,
 ) -> List[case_description.TubingDescription]:
     alfacase_to_case_description = {
         "name": load_value,
         "length": get_scalar_loader(from_unit="m"),
-        "outer_diameter": get_scalar_loader(from_unit="m"),
-        "inner_diameter": get_scalar_loader(from_unit="m"),
+        "outer_diameter": get_scalar_loader(category="diameter"),
+        "inner_diameter": get_scalar_loader(category="diameter"),
         "inner_roughness": get_scalar_loader(from_unit="m"),
         "material": load_value,
     }
 
     def generate_tubings_description(document: DescriptionDocument):
         case_values = to_case_values(document, alfacase_to_case_description)
-        return case_description.TubingDescription(**case_values)
+        item_description = case_description.TubingDescription(**case_values)
+        return update_multi_input_flags(document, item_description)
 
     return [
         generate_tubings_description(alfacase_document)
         for alfacase_document in document
     ]
 
 
@@ -1228,15 +1576,16 @@
         "thickness": get_scalar_loader(from_unit="m"),
         "material_name": load_value,
         "has_annulus_flow": load_value,
     }
 
     def generate_wall_layer_container_description(document: DescriptionDocument):
         case_values = to_case_values(document, alfacase_to_case_description)
-        return case_description.WallLayerDescription(**case_values)
+        item_description = case_description.WallLayerDescription(**case_values)
+        return update_multi_input_flags(document, item_description)
 
     return [
         generate_wall_layer_container_description(alfacase_document)
         for alfacase_document in document
     ]
 
 
@@ -1244,46 +1593,59 @@
     document: DescriptionDocument,
 ) -> case_description.AnnulusDescription:
     alfacase_to_case_description = {
         "has_annulus_flow": load_value,
         "pvt_model": load_value,
         "top_node": load_value,
         "initial_conditions": load_initial_conditions_description,
-        "gas_lift_valve_equipment": load_gas_lift_valve_equipment_description,
+        "equipment": get_instance_loader(
+            class_=case_description.AnnulusEquipmentDescription
+        ),
     }
     case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.AnnulusDescription(**case_values)
+    item_description = case_description.AnnulusDescription(**case_values)
+    return update_multi_input_flags(document, item_description)
+
+
+def load_trends_output_description(
+    document: DescriptionDocument,
+) -> case_description.TrendsOutputDescription:
+    return load_instance(document, case_description.TrendsOutputDescription)
 
 
 def load_case_output_description(
     document: DescriptionDocument,
 ) -> case_description.CaseOutputDescription:
     alfacase_to_case_description = {
         "profiles": load_profile_output_description,
-        "trends": load_trend_output_description,
+        "automatic_profile_frequency": load_value,
         "profile_frequency": get_scalar_loader(from_unit="s"),
+        "trends": load_trends_output_description,
+        "automatic_trend_frequency": load_value,
         "trend_frequency": get_scalar_loader(from_unit="s"),
     }
     case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.CaseOutputDescription(**case_values)
+    item_description = case_description.CaseOutputDescription(**case_values)
+    return update_multi_input_flags(document, item_description)
 
 
 def load_open_hole_description(
     document: DescriptionDocument,
 ) -> List[case_description.OpenHoleDescription]:
     alfacase_to_case_description = {
         "name": load_value,
         "length": get_scalar_loader(from_unit="m"),
-        "diameter": get_scalar_loader(from_unit="m"),
+        "diameter": get_scalar_loader(category="diameter"),
         "inner_roughness": get_scalar_loader(from_unit="m"),
     }
 
     def generate_open_hole_description(document: DescriptionDocument):
         case_values = to_case_values(document, alfacase_to_case_description)
-        return case_description.OpenHoleDescription(**case_values)
+        item_description = case_description.OpenHoleDescription(**case_values)
+        return update_multi_input_flags(document, item_description)
 
     return [
         generate_open_hole_description(alfacase_document)
         for alfacase_document in document
     ]
 
 
@@ -1293,28 +1655,32 @@
     alfacase_to_case_description = {
         "casing_sections": load_casing_section_description,
         "tubings": load_tubing_description,
         "packers": load_packer_description,
         "open_holes": load_open_hole_description,
     }
     case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.CasingDescription(**case_values)
+    item_description = case_description.CasingDescription(**case_values)
+    return update_multi_input_flags(document, item_description)
 
 
 def load_compressor_pressure_table_description(
     document: DescriptionDocument,
 ) -> case_description.CompressorPressureTableDescription:
     alfacase_to_case_description = {
         "speed_entries": get_array_loader(from_unit="rpm"),
         "corrected_mass_flow_rate_entries": get_array_loader(from_unit="kg/s"),
         "pressure_ratio_table": get_array_loader(from_unit="-"),
         "isentropic_efficiency_table": get_array_loader(from_unit="-"),
     }
     case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.CompressorPressureTableDescription(**case_values)
+    item_description = case_description.CompressorPressureTableDescription(
+        **case_values
+    )
+    return update_multi_input_flags(document, item_description)
 
 
 def load_compressor_equipment_description(
     document: DescriptionDocument,
 ) -> Dict[str, case_description.CompressorEquipmentDescription]:
     alfacase_to_case_description = {
         "name": load_value,
@@ -1329,15 +1695,18 @@
             enum_class=constants.InterpolationType
         ),
         "flow_direction": get_enum_loader(enum_class=constants.FlowDirection),
     }
 
     def generate_compressor_description(document: DescriptionDocument):
         case_values = to_case_values(document, alfacase_to_case_description)
-        return case_description.CompressorEquipmentDescription(**case_values)
+        item_description = case_description.CompressorEquipmentDescription(
+            **case_values
+        )
+        return update_multi_input_flags(document, item_description)
 
     return {
         key.data: generate_compressor_description(
             DescriptionDocument(value, document.file_path)
         )
         for key, value in document.content.items()
     }
@@ -1352,152 +1721,137 @@
             enum_class=constants.PipeThermalPositionInput
         ),
         "reference_y_coordinate": get_scalar_loader(from_unit="m"),
         "md_properties_table": load_environment_property_description,
         "tvd_properties_table": load_environment_property_description,
     }
     case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.EnvironmentDescription(**case_values)
+    item_description = case_description.EnvironmentDescription(**case_values)
+    return update_multi_input_flags(document, item_description)
 
 
 def load_formation_description(
     document: DescriptionDocument,
 ) -> case_description.FormationDescription:
     alfacase_to_case_description = {
         "reference_y_coordinate": get_scalar_loader(from_unit="m"),
         "layers": load_formation_layer_description,
     }
     case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.FormationDescription(**case_values)
+    item_description = case_description.FormationDescription(**case_values)
+    return update_multi_input_flags(document, item_description)
 
 
-def load_pump_equipment_description(
+def _generate_description(
     document: DescriptionDocument,
-) -> Dict[str, case_description.PumpEquipmentDescription]:
-    alfacase_to_case_description = {
-        "name": load_value,
-        "position": get_scalar_loader(from_unit="m"),
-        "type": get_enum_loader(enum_class=constants.PumpType),
-        "pressure_boost": get_scalar_loader(from_unit="Pa"),
-        "thermal_efficiency": get_scalar_loader(from_unit="-"),
-        "table": load_table_pump_description,
-        "speed_curve": load_speed_curve_description,
-        "speed_curve_interpolation_type": get_enum_loader(
-            enum_class=constants.InterpolationType
-        ),
-        "flow_direction": get_enum_loader(enum_class=constants.FlowDirection),
-    }
+    alfacase_to_case_description: Dict[str, Callable],
+    description_type: Type[T],
+) -> T:
+    case_values = to_case_values(document, alfacase_to_case_description)
+    item_description = description_type(**case_values)
+    return update_multi_input_flags(document, item_description)
 
-    def generate_pump_description(document: DescriptionDocument):
-        case_values = to_case_values(document, alfacase_to_case_description)
-        return case_description.PumpEquipmentDescription(**case_values)
+
+def load_valve_equipment_description(
+    document: DescriptionDocument,
+) -> Dict[str, case_description.ValveEquipmentDescription]:
+    alfacase_to_case_description = get_case_description_attribute_loader_dict(
+        case_description.ValveEquipmentDescription
+    )
 
     return {
-        key.data: generate_pump_description(
-            DescriptionDocument(value, document.file_path)
+        key.data: _generate_description(
+            DescriptionDocument(value, document.file_path),
+            alfacase_to_case_description,
+            case_description.ValveEquipmentDescription,
         )
         for key, value in document.content.items()
     }
 
 
-def load_valve_equipment_description(
+def load_pig_equipment_description(
     document: DescriptionDocument,
-) -> Dict[str, case_description.ValveEquipmentDescription]:
-    alfacase_to_case_description = {
-        "name": load_value,
-        "position": get_scalar_loader(from_unit="m"),
-        "type": get_enum_loader(enum_class=constants.ValveType),
-        "diameter": get_scalar_loader(from_unit="m"),
-        "opening_type": get_enum_loader(enum_class=constants.ValveOpeningType),
-        "opening": get_scalar_loader(from_unit="-"),
-        "opening_curve_interpolation_type": get_enum_loader(
-            enum_class=constants.InterpolationType
-        ),
-        "opening_curve": load_opening_curve_description,
-        "cv_table": load_cv_table_description,
-        "flow_direction": get_enum_loader(enum_class=constants.FlowDirection),
-    }
-
-    def generate_valve_description(document: DescriptionDocument):
-
-        case_values = to_case_values(document, alfacase_to_case_description)
-        return case_description.ValveEquipmentDescription(**case_values)
+) -> Dict[str, case_description.PigEquipmentDescription]:
+    alfacase_to_case_description = get_case_description_attribute_loader_dict(
+        case_description.PigEquipmentDescription
+    )
 
     return {
-        key.data: generate_valve_description(
-            DescriptionDocument(value, document.file_path)
+        key.data: _generate_description(
+            DescriptionDocument(value, document.file_path),
+            alfacase_to_case_description,
+            case_description.PigEquipmentDescription,
         )
         for key, value in document.content.items()
     }
 
 
 def load_wall_description(
     document: DescriptionDocument,
 ) -> List[case_description.WallDescription]:
     alfacase_to_case_description = {
         "name": load_value,
         "inner_roughness": get_scalar_loader(from_unit="m"),
         "wall_layer_container": load_wall_layer_description,
     }
 
-    def generate_walls_description(document: DescriptionDocument):
-        case_values = to_case_values(document, alfacase_to_case_description)
-        return case_description.WallDescription(**case_values)
-
     return [
-        generate_walls_description(alfacase_document) for alfacase_document in document
+        _generate_description(
+            alfacase_document,
+            alfacase_to_case_description,
+            case_description.WallDescription,
+        )
+        for alfacase_document in document
     ]
 
 
 def load_equipment_description(
     document: DescriptionDocument,
 ) -> case_description.EquipmentDescription:
-    alfacase_to_case_description = {
-        "mass_sources": load_mass_source_equipment_description,
-        "pumps": load_pump_equipment_description,
-        "valves": load_valve_equipment_description,
-        "reservoir_inflows": load_reservoir_inflow_equipment_description,
-        "heat_sources": load_heat_source_equipment_description,
-        "compressors": load_compressor_equipment_description,
-    }
-    case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.EquipmentDescription(**case_values)
+    return load_instance(document, case_description.EquipmentDescription)
 
 
 def load_x_and_y_description(
     document: DescriptionDocument,
 ) -> case_description.XAndYDescription:
     alfacase_to_case_description = {
         "x": get_array_loader(from_unit="m"),
         "y": get_array_loader(from_unit="m"),
     }
-    case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.XAndYDescription(**case_values)
+    return _generate_description(
+        document,
+        alfacase_to_case_description,
+        case_description.XAndYDescription,
+    )
 
 
 def load_length_and_elevation_description(
     document: DescriptionDocument,
 ) -> case_description.LengthAndElevationDescription:
     alfacase_to_case_description = {
         "length": get_array_loader(from_unit="m"),
         "elevation": get_array_loader(from_unit="m"),
     }
-    case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.LengthAndElevationDescription(**case_values)
+    return _generate_description(
+        document,
+        alfacase_to_case_description,
+        case_description.LengthAndElevationDescription,
+    )
 
 
 def load_profile_description(
     document: DescriptionDocument,
 ) -> case_description.ProfileDescription:
     alfacase_to_case_description = {
         "x_and_y": load_x_and_y_description,
         "length_and_elevation": load_length_and_elevation_description,
     }
     case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.ProfileDescription(**case_values)
+    item_description = case_description.ProfileDescription(**case_values)
+    return update_multi_input_flags(document, item_description)
 
 
 def load_pipe_description(
     document: DescriptionDocument,
 ) -> List[case_description.PipeDescription]:
     # fmt: off
     alfacase_to_case_description = {
@@ -1509,18 +1863,20 @@
         "pvt_model": load_value,
         "segments": load_pipe_segments_description,
         "source": load_value,
         "target": load_value,
         "source_port": get_enum_loader(enum_class=constants.WellConnectionPort),
         "target_port": get_enum_loader(enum_class=constants.WellConnectionPort),
     }
+
     # fmt: on
     def generate_pipes_description(document: DescriptionDocument):
         case_values = to_case_values(document, alfacase_to_case_description)
-        return case_description.PipeDescription(**case_values)
+        item_description = case_description.PipeDescription(**case_values)
+        return update_multi_input_flags(document, item_description)
 
     return [
         generate_pipes_description(alfacase_document) for alfacase_document in document
     ]
 
 
 def load_well_description(
@@ -1539,41 +1895,30 @@
         "environment": load_environment_description,
         "equipment": load_equipment_description,
         "formation": load_formation_description,
     }
 
     def generate_wells_description(document: DescriptionDocument):
         case_values = to_case_values(document, alfacase_to_case_description)
-        return case_description.WellDescription(**case_values)
+        item_description = case_description.WellDescription(**case_values)
+        return update_multi_input_flags(document, item_description)
 
     return [
         generate_wells_description(alfacase_document) for alfacase_document in document
     ]
 
 
 def load_physics_description(
     document: DescriptionDocument,
 ) -> case_description.PhysicsDescription:
-    # fmt: off
-    alfacase_to_case_description = {
-        'hydrodynamic_model': get_enum_loader(enum_class=constants.HydrodynamicModelType),
-        'simulation_regime': get_enum_loader(enum_class=constants.SimulationRegimeType),
-        'energy_model': get_enum_loader(enum_class=constants.EnergyModel),
-        'solids_model': get_enum_loader(enum_class=constants.SolidsModelType),
-        'initial_condition_strategy': get_enum_loader(enum_class=constants.InitialConditionStrategyType),
-        'restart_filepath': load_path,
-        'keep_former_results': load_value,
-        'emulsion_model': get_enum_loader(enum_class=constants.EmulsionModelType),
-        'emulsion_model_plugin_id': load_value,
-        'flash_model': get_enum_loader(enum_class=constants.FlashModel),
-        'correlations_package': get_enum_loader(enum_class=constants.CorrelationPackageType),
-    }
-    # fmt: on
-    case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.PhysicsDescription(**case_values)
+    return load_instance(
+        document,
+        case_description.PhysicsDescription,
+        explicit_loaders=dict(restart_filepath=load_path),
+    )
 
 
 # fmt: off
 def load_numerical_options_description(document: DescriptionDocument) -> case_description.NumericalOptionsDescription:
     alfacase_to_case_description = {
         'tolerance': load_value,
         'maximum_iterations': load_value,
@@ -1584,19 +1929,22 @@
         'divergence_tolerance': load_value,
         'friction_factor_evaluation_strategy': get_enum_loader(enum_class=constants.EvaluationStrategyType),
         'simulation_mode': get_enum_loader(enum_class=constants.SimulationModeType),
         'enable_solver_caching': load_value,
         'caching_rtol': load_value,
         'caching_atol': load_value,
         'always_repeat_timestep': load_value,
+        'enable_fast_compositional': load_value
     }
     case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.NumericalOptionsDescription(**case_values)
+    item_description = case_description.NumericalOptionsDescription(**case_values)
+    return update_multi_input_flags(document, item_description)
 # fmt: on
 
+
 # fmt: off
 def load_time_options_description(
     document: DescriptionDocument
 ) -> case_description.TimeOptionsDescription:
     alfacase_to_case_description = {
         "stop_on_steady_state": load_value,
         "initial_time": get_scalar_loader(from_unit="h"),
@@ -1604,25 +1952,25 @@
         "initial_timestep": get_scalar_loader(from_unit="s"),
         "minimum_timestep": get_scalar_loader(from_unit="s"),
         "maximum_timestep": get_scalar_loader(from_unit="s"),
         "restart_autosave_frequency": get_scalar_loader(from_unit="h"),
         "minimum_time_for_steady_state_stop": get_scalar_loader(from_unit="s"),
     }
     case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.TimeOptionsDescription(**case_values)
-
+    item_description = case_description.TimeOptionsDescription(**case_values)
+    return update_multi_input_flags(document, item_description)
 
 # fmt: on
 
 
 def load_tracer_model_constant_coefficients_description(
     document: DescriptionDocument,
 ) -> Dict[str, case_description.TracerModelConstantCoefficientsDescription]:
     alfacase_to_case_description = {
-        "partition_coefficients": get_dict_with_scalar_loader(category="mass fraction")
+        "partition_coefficients": get_scalar_dict_loader(category="mass fraction")
     }
 
     def generate_tracer_model_constant_coefficients_description(
         value: DescriptionDocument,
     ):
         case_values = to_case_values(value, alfacase_to_case_description)
         return case_description.TracerModelConstantCoefficientsDescription(
@@ -1640,36 +1988,44 @@
 def load_tracers_description(
     document: DescriptionDocument,
 ) -> case_description.TracersDescription:
     alfacase_to_case_description = {
         "constant_coefficients": load_tracer_model_constant_coefficients_description
     }
     case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.TracersDescription(**case_values)
+    item_description = case_description.TracersDescription(**case_values)
+    return update_multi_input_flags(document, item_description)
 
 
 def load_case_description(
     document: DescriptionDocument,
 ) -> case_description.CaseDescription:
+    from alfasim_sdk._internal.alfacase.plugin_alfacase_to_case import (
+        load_list_of_plugin,
+    )
+
     # fmt: off
     alfacase_to_case_description = {
         'physics': load_physics_description,
         'numerical_options': load_numerical_options_description,
         'time_options': load_time_options_description,
         'max_timestep_change_factor': load_value,
         'max_cfl_value': load_value,
         'friction_factor_evaluation_strategy': get_enum_loader(enum_class=constants.EvaluationStrategyType),
         'name': load_value,
+        'comment': load_value,
+        'plugins': load_list_of_plugin,
         'positions': load_value,
         'tracers': load_tracers_description,
         'ipr_models': load_ipr_models_description,
         'pvt_models': load_pvt_models_description,
         'materials': load_material_description,
         'nodes': load_node_description,
         'outputs': load_case_output_description,
         'pipes': load_pipe_description,
         'walls': load_wall_description,
         'wells': load_well_description,
     }
     # fmt: on
     case_values = to_case_values(document, alfacase_to_case_description)
-    return case_description.CaseDescription(**case_values)
+    item_description = case_description.CaseDescription(**case_values)
+    return update_multi_input_flags(document, item_description)
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/generate_case_description_docstring.py` & `alfasim_sdk-2024.1/src/alfasim_sdk/_internal/alfacase/generate_case_description_docstring.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 from typing import List
 from typing import Sequence
 from typing import Tuple
 from typing import Type
 
 import attr
 from attr._make import Attribute
+from barril.curve.curve import Curve
 from barril.units import Array
 from barril.units._scalar import Scalar
 
 from alfasim_sdk._internal.alfacase.generate_schema import IGNORED_PROPERTIES
 from alfasim_sdk._internal.alfacase.generate_schema import is_array
 from alfasim_sdk._internal.alfacase.generate_schema import is_attrs
 from alfasim_sdk._internal.alfacase.generate_schema import is_boolean
+from alfasim_sdk._internal.alfacase.generate_schema import is_curve
 from alfasim_sdk._internal.alfacase.generate_schema import is_dict
 from alfasim_sdk._internal.alfacase.generate_schema import is_enum
 from alfasim_sdk._internal.alfacase.generate_schema import is_float
 from alfasim_sdk._internal.alfacase.generate_schema import is_int
 from alfasim_sdk._internal.alfacase.generate_schema import is_list
 from alfasim_sdk._internal.alfacase.generate_schema import is_path
 from alfasim_sdk._internal.alfacase.generate_schema import is_scalar
@@ -38,22 +40,30 @@
     [
         "angle per time",
         "density",
         "dimensionless",
         "dynamic viscosity",
         "emissivity",
         "flow coefficient",
+        "force",
+        "force per velocity",
+        "force per velocity squared",
+        "forchheimer linear productivity index",
+        "forchheimer quadratic productivity index",
         "heat transfer coefficient",
         "length",
+        "mass",
         "mass flow rate",
         "mass fraction",
         "mass per mol",
         "molar thermodynamic energy",
         "molar volume",
         "mole per mole",
+        "nonDarcy flow coefficient",
+        "permeability rock",
         "power",
         "pressure",
         "productivity index",
         "specific heat capacity",
         "standard volume per standard volume",
         "standard volume per standard volume",
         "standard volume per time",
@@ -76,15 +86,15 @@
     units = unit_database.GetCategoryInfo(category).valid_units_set
     info = unit_database.unit_to_unit_info
     body = [f'    :"{unit}": {info[unit].name}' for unit in units]
     lines = [
         f".. admonition:: Available units for category '{category}'",
         "    :class: dropdown",
         "",
-        *sorted(body, key=str.casefold),
+        *sorted(body, key=lambda x: (x.casefold(), x.swapcase())),
         "",
     ]
     return "\n".join(lines)
 
 
 def generate_definition(class_name: str) -> str:
     """
@@ -137,18 +147,18 @@
             f"{value.default.__class__.__name__}.{value.default.name}"
         )
     elif isinstance(value.default, attr.Factory):
         if value.default.factory is dict:
             default_value_string += "{}"
         elif value.default.factory is list:
             default_value_string += "[]"
-        elif is_attrs(value.default):
+        elif is_attrs(value.default.factory):
             default_value_string += f"{value.default.factory.__name__}()"
         else:
-            default_value_string += "UNKNOWN FACTORY"
+            assert False, "Unknown factory"  # pragma: no cover
     elif is_attrs(value.default):
         default_value_string += f"{value.default.__class__.__name__}()"
     else:
         default_value_string += f"{repr(value.default)}"
 
     return default_value_string
 
@@ -165,15 +175,18 @@
             for predicate_function, handle_function in list_of_predicate_and_handles:
                 if predicate_function(value.type):
                     attribute_value = handle_function(value.type)
                     default_value = _get_case_attr_default_value(value)
 
                     # For Schema: if the attributes have a default value the entry is optional.
                     if default_value and is_schema:
-                        attribute_value += " # optional"
+                        if attribute_value.lstrip(" \t").startswith("\n"):
+                            attribute_value = " # optional" + attribute_value
+                        else:
+                            attribute_value += "  # optional"
                         default_value = ""
 
                     # If attribute_value ends with backslash (because of the cross-reference), add extra space
                     # for a default value.
                     # Otherwise, the equal symbol will be sticky with the link.
                     if default_value and attribute_value[-1] == "\\":
                         default_value = f" {default_value}"
@@ -181,14 +194,15 @@
                     line_content = f"{BASE_INDENT}{attribute_name}: {attribute_value}{default_value}"
 
                     # Remove the last character if it's a backslash otherwise the line break will be avoided.
                     if line_content.endswith("\\"):
                         line_content = line_content[:-1]
 
                     lines.append(line_content)
+                    break  # Match found, break inner loop
     return lines
 
 
 def _get_class_with_reference(visible_name: str, ref: str) -> str:
     """
     Return the name of the class with a valid reference to be used by sphinx.
     """
@@ -201,14 +215,21 @@
 
 
 def _get_array_reference() -> str:
     """Return a string with a cross-reference to Array documentation."""
     return _get_class_with_reference(visible_name="Array", ref="barril.units.Array")
 
 
+def _get_curve_reference() -> str:
+    """Return a string with a cross-reference to Curve documentation."""
+    return _get_class_with_reference(
+        visible_name="Curve", ref="barril.curve.curve.Curve"
+    )
+
+
 def _get_list_reference() -> str:
     """Return a string with a cross-reference to List documentation."""
     return _get_class_with_reference(visible_name="List", ref="typing.List")
 
 
 def _get_dict_reference() -> str:
     """Return a string with a cross-reference to Dict documentation."""
@@ -264,14 +285,16 @@
     Note that all usages of union on CaseDescription are from the Optional module.
     """
     optional_with_reference = _get_optional_reference()
     ref_value = value.__args__[0]
 
     if isinstance(ref_value, enum.EnumMeta):
         name = enum_formatted(ref_value)
+    elif is_attrs(ref_value):
+        name = attrs_formatted(ref_value)
     elif is_array(ref_value):
         name = _get_array_reference()
     elif is_list(ref_value):
         name = f"{_get_list_reference()}[{ref_value.__args__[0].__name__}]"
     else:
         name = ref_value.__name__
 
@@ -326,31 +349,34 @@
         lines += attrs_formatted_for_schema(argument)
     elif is_union(argument):
         lines += f"{' | '.join(i.__name__.replace('str', 'string') for i in argument.__args__)}"
     elif is_scalar(argument):
         lines += scalar_formatted_for_schema(argument, number_of_indent=2)
     elif is_array(argument):
         lines += array_formatted_for_schema(argument, number_of_indent=2)
+    elif argument is Any:
+        lines += "Any"
     else:
         lines += argument.__name__
     return lines
 
 
 def union_formatted_for_schema(value: Any) -> str:
     """
     All usages of union on CaseDescription are from the Optional module, so this function will
     return a string showing parameters with a label '# optional' indicating that this field could be
     is not mandatory.
     """
     parameter = value.__args__[0]
     if value.__args__ in ((str, type(None)), (Path, type(None))):
         name = "string"
+    elif value.__args__ == (Scalar, type(None)):
+        name = scalar_formatted_for_schema(value)
     elif value.__args__ == (Array, type(None)):
-        name = f"{INDENT}"
-        name += array_formatted_for_schema(value)
+        name = array_formatted_for_schema(value)
     elif isinstance(parameter, enum.EnumMeta):
         name = f"{enum_formatted_for_schema(parameter)}"
     elif is_attrs(parameter):
         name = f"{attrs_formatted_for_schema(parameter)}"
     elif is_list(parameter):
         name = f"{INDENT}"
         name += list_formatted_for_schema(parameter)
@@ -379,25 +405,41 @@
         How many indentations beyond the base should this schema have,
         useful for when used with other schema such as Dict.
     """
     block_indentation = BASE_INDENT + INDENT * number_of_indent
     return f"\n{block_indentation}values: [number]\n{block_indentation}unit: string"
 
 
+def curve_formatted_for_schema(value: Type[Curve], *, number_of_indent=1) -> str:
+    """
+    Return a string showing how to configure a Array.
+
+    :param int number_of_indent:
+        How many indentations beyond the base should this schema have,
+        useful for when used with other schema such as Dict.
+    """
+    block_indentation = BASE_INDENT + INDENT * number_of_indent
+    array_schema = array_formatted_for_schema(
+        Array, number_of_indent=number_of_indent + 1
+    )
+    return f"\n{block_indentation}image:{array_schema}\n{block_indentation}domain:{array_schema}"
+
+
 LIST_OF_CASE_ATTRIBUTES = [
     (is_enum, enum_formatted),
     (is_attrs, attrs_formatted),
     (is_list, list_formatted),
     (is_float, lambda value: value.__name__),
     (is_str, lambda value: value.__name__),
     (is_boolean, lambda value: value.__name__),
     (is_dict, dict_formatted),
     (is_union, union_formatted),
     (is_scalar, lambda value: _get_scalar_reference()),
     (is_array, lambda value: _get_array_reference()),
+    (is_curve, lambda value: _get_curve_reference()),
     (is_int, lambda value: value.__name__),
     (is_path, lambda value: value.__name__),
 ]
 
 
 LIST_OF_CASE_SCHEMAS = [
     (is_enum, enum_formatted),
@@ -406,10 +448,11 @@
     (is_float, lambda value: "number"),
     (is_str, lambda value: "string"),
     (is_boolean, lambda value: "boolean"),
     (is_dict, dict_formatted_for_schema),
     (is_union, union_formatted_for_schema),
     (is_scalar, scalar_formatted_for_schema),
     (is_array, array_formatted_for_schema),
+    (is_curve, curve_formatted_for_schema),
     (is_int, lambda value: "number"),
     (is_path, lambda value: value.__name__),
 ]
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/alfatable.py` & `alfasim_sdk-2024.1/src/alfasim_sdk/_internal/alfacase/alfatable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from pathlib import Path
 
 from alfasim_sdk._internal.alfacase import case_description
 from alfasim_sdk._internal.alfacase.alfacase_to_case import get_category_for
 
 
-def generate_alfatable_file(alfacase_file, alfatable_filename, description):
+def generate_alfatable_file(
+    alfacase_file: Path,
+    alfatable_filename: str,
+    description: case_description.CaseDescription,
+) -> Path:
     """
     Create `.alfatable` file for the given description.
     """
     from boltons.strutils import slugify
 
     from alfasim_sdk import convert_description_to_alfacase
 
@@ -20,24 +24,25 @@
         / f"{alfacase_file.stem}.{slugify(alfatable_filename)}.alfatable"
     )
     alfatable_file.write_text(alfatable_content, encoding="utf-8")
     return alfatable_file
 
 
 def load_pvt_model_table_parameters_description_from_alfatable(
-    file_path,
-) -> case_description.PvtModelTableParametersDescription:
+    file_path: Path,
+) -> case_description.PvtModelPtTableParametersDescription:
     """
     Load the content from the alfatable in the given file_path. The validation is turned off due to performance issues.
     """
-    from ruamel import yaml as ruamelyaml
+    from strictyaml.ruamel.main import YAML
     from barril.units import Scalar
     import numpy as np
 
-    content = ruamelyaml.safe_load(Path(file_path).read_text(encoding="UTF-8"))
+    yaml = YAML(typ="safe", pure=True)
+    content = yaml.load(Path(file_path))
 
     table_parameter_keys_and_values = {
         "pressure_values": np.array(content["pressure_values"]),
         "temperature_values": np.array(content["temperature_values"]),
         "table_variables": [np.array(value) for value in content["table_variables"]],
         "variable_names": content["variable_names"],
         "label": content.get("label", None),
@@ -56,10 +61,10 @@
         "total_water_fraction": "-",
     }
 
     table_parameter_keys_and_scalars = {
         key: Scalar(get_category_for(unit), content[key]["value"], content[key]["unit"])
         for key, unit in key_and_unit.items()
     }
-    return case_description.PvtModelTableParametersDescription(
+    return case_description.PvtModelPtTableParametersDescription(
         **table_parameter_keys_and_values, **table_parameter_keys_and_scalars
     )
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/schema.py` & `alfasim_sdk-2024.1/src/alfasim_sdk/_internal/alfacase/schema.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 # fmt: off
 # #[[[cog
 # import cog
 # from alfasim_sdk import CaseDescription
 # from alfasim_sdk._internal.alfacase.generate_schema import get_all_classes_that_needs_schema, generate_alfacase_schema
-# cog.out("from strictyaml import Bool, Enum, Int, Map, MapPattern, Optional, Seq, Str, Float # noreorder")
+# cog.out("from strictyaml import Any, Bool, Enum, Int, Map, MapPattern, Optional, Seq, Str, Float # noreorder")
 # cog.out("\n\n")
 # cog.out("\n\n")
 # list_of_classes_that_needs_schema = get_all_classes_that_needs_schema(CaseDescription)
 # for class_ in list_of_classes_that_needs_schema:
 #    cog.out(generate_alfacase_schema(class_))
 # ]]]
-from strictyaml import Bool, Enum, Int, Map, MapPattern, Optional, Seq, Str, Float # noreorder
+from strictyaml import Any, Bool, Enum, Int, Map, MapPattern, Optional, Seq, Str, Float # noreorder
 
 
 
+alfasim_version_info_schema = Map(
+    {
+        "platform": Str(),
+        "version": Str(),
+        "revision": Str(),
+        "date": Str(),
+    }
+)
 bip_description_schema = Map(
     {
         "component_1": Str(),
         "component_2": Str(),
         "value": Float(),
     }
 )
@@ -32,14 +40,19 @@
         "inner_roughness": Map({"value": Float(), "unit": Str()}),
         Optional("material"): Str(),
         "top_of_filler": Map({"value": Float(), "unit": Str()}),
         Optional("filler_material"): Str(),
         Optional("material_above_filler"): Str(),
     }
 )
+combined_fluid_description_schema = Map(
+    {
+        Optional("pvt_model"): Str(),
+    }
+)
 composition_description_schema = Map(
     {
         "component": Str(),
         Optional("molar_fraction"): Map({"value": Float(), "unit": Str()}),
         Optional("reference_enthalpy"): Map({"value": Float(), "unit": Str()}),
     }
 )
@@ -47,14 +60,38 @@
     {
         Optional("speed_entries"): Map({"values": Seq(Float()), "unit": Str()}),
         Optional("corrected_mass_flow_rate_entries"): Map({"values": Seq(Float()), "unit": Str()}),
         Optional("pressure_ratio_table"): Map({"values": Seq(Float()), "unit": Str()}),
         Optional("isentropic_efficiency_table"): Map({"values": Seq(Float()), "unit": Str()}),
     }
 )
+controller_input_signal_properties_description_schema = Map(
+    {
+        Optional("target_variable"): Str(),
+        Optional("input_trend_name"): Str(),
+        Optional("unit"): Str(),
+    }
+)
+controller_output_signal_properties_description_schema = Map(
+    {
+        Optional("controlled_property"): Str(),
+        Optional("unit"): Str(),
+        Optional("network_element_name"): Str(),
+        Optional("min_value"): Float(),
+        Optional("max_value"): Float(),
+        Optional("max_rate_of_change"): Float(),
+    }
+)
+controller_trend_description_schema = Map(
+    {
+        Optional("name"): Str(),
+        "curve_names": Seq(Str()),
+        "element_name": Str(),
+    }
+)
 cv_table_description_schema = Map(
     {
         Optional("opening"): Map({"values": Seq(Float()), "unit": Str()}),
         Optional("flow_coefficient"): Map({"values": Seq(Float()), "unit": Str()}),
     }
 )
 environment_property_description_schema = Map(
@@ -63,35 +100,86 @@
         "temperature": Map({"value": Float(), "unit": Str()}),
         "type": Enum(['walls_and_environment_heat_transfer_coefficient', 'walls_and_water_heat_transfer_coefficient_model', 'walls_and_air_heat_transfer_coefficient_model', 'overall_heat_transfer_coefficient_model', 'walls_without_environment_heat_transfer_coefficient']),
         Optional("heat_transfer_coefficient"): Map({"value": Float(), "unit": Str()}),
         Optional("overall_heat_transfer_coefficient"): Map({"value": Float(), "unit": Str()}),
         Optional("fluid_velocity"): Map({"value": Float(), "unit": Str()}),
     }
 )
+equipment_trend_description_schema = Map(
+    {
+        Optional("name"): Str(),
+        "curve_names": Seq(Str()),
+        "element_name": Str(),
+    }
+)
+fetkovich_ipr_description_schema = Map(
+    {
+        Optional("well_index_phase"): Enum(['well_index_phase_gas', 'well_index_phase_oil', 'well_index_phase_water', 'well_index_phase_liquid']),
+        Optional("min_pressure_difference"): Map({"value": Float(), "unit": Str()}),
+        Optional("bubble_point_pressure"): Map({"value": Float(), "unit": Str()}),
+        Optional("well_index_input_type"): Enum(['constant', 'curve']),
+        Optional("well_index"): Map({"value": Float(), "unit": Str()}),
+        Optional("well_index_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
+    }
+)
+forchheimer_ipr_description_schema = Map(
+    {
+        Optional("calculate_coeff_option"): Enum(['reservoir_parameters', 'flow_coefficients']),
+        Optional("well_index_phase"): Enum(['well_index_phase_gas', 'well_index_phase_oil', 'well_index_phase_water', 'well_index_phase_liquid']),
+        Optional("min_pressure_difference"): Map({"value": Float(), "unit": Str()}),
+        Optional("gas_viscosity"): Map({"value": Float(), "unit": Str()}),
+        Optional("gas_z_factor"): Map({"value": Float(), "unit": Str()}),
+        Optional("reservoir_permeability"): Map({"value": Float(), "unit": Str()}),
+        Optional("drainage_radius"): Map({"value": Float(), "unit": Str()}),
+        Optional("well_radius"): Map({"value": Float(), "unit": Str()}),
+        Optional("well_skin_factor"): Map({"value": Float(), "unit": Str()}),
+        Optional("non_darcy_parameter"): Map({"value": Float(), "unit": Str()}),
+        Optional("B_coeff"): Map({"value": Float(), "unit": Str()}),
+        Optional("C_coeff"): Map({"value": Float(), "unit": Str()}),
+    }
+)
 formation_layer_description_schema = Map(
     {
         "name": Str(),
         "start": Map({"value": Float(), "unit": Str()}),
         Optional("material"): Str(),
     }
 )
 gas_lift_valve_equipment_description_schema = Map(
     {
         "position": Map({"value": Float(), "unit": Str()}),
         "diameter": Map({"value": Float(), "unit": Str()}),
         "valve_type": Enum(['perkins_valve', 'choke_valve_with_flow_coefficient', 'check_valve']),
         "delta_p_min": Map({"value": Float(), "unit": Str()}),
-        "discharge_coeff": Map({"value": Float(), "unit": Str()}),
+        "discharge_coefficient": Map({"value": Float(), "unit": Str()}),
+    }
+)
+global_trend_description_schema = Map(
+    {
+        Optional("name"): Str(),
+        "curve_names": Seq(Str()),
     }
 )
 heat_source_equipment_description_schema = Map(
     {
         "start": Map({"value": Float(), "unit": Str()}),
         "length": Map({"value": Float(), "unit": Str()}),
-        "power": Map({"value": Float(), "unit": Str()}),
+        Optional("power_input_type"): Enum(['constant', 'curve']),
+        Optional("power"): Map({"value": Float(), "unit": Str()}),
+        Optional("power_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
     }
 )
 heavy_component_description_schema = Map(
     {
         "name": Str(),
         "scn": Int(),
         Optional("MW"): Map({"value": Float(), "unit": Str()}),
@@ -132,42 +220,145 @@
         Optional("Cp_4"): Map({"value": Float(), "unit": Str()}),
     }
 )
 linear_ipr_description_schema = Map(
     {
         Optional("well_index_phase"): Enum(['well_index_phase_gas', 'well_index_phase_oil', 'well_index_phase_water', 'well_index_phase_liquid']),
         Optional("min_pressure_difference"): Map({"value": Float(), "unit": Str()}),
+        Optional("well_index_input_type"): Enum(['constant', 'curve']),
         Optional("well_index"): Map({"value": Float(), "unit": Str()}),
+        Optional("well_index_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
     }
 )
 mass_source_equipment_description_schema = Map(
     {
         Optional("fluid"): Str(),
         Optional("tracer_mass_fraction"): Map({"values": Seq(Float()), "unit": Str()}),
+        Optional("temperature_input_type"): Enum(['constant', 'curve']),
         Optional("temperature"): Map({"value": Float(), "unit": Str()}),
+        Optional("temperature_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
         Optional("source_type"): Enum(['mass_source_type_mass_flow_rates', 'mass_source_type_all_volumetric_flow_rates', 'mass_source_type_flow_rate_oil_gor_wc', 'mass_source_type_flow_rate_gas_gor_wc', 'mass_source_type_flow_rate_water_gor_wc', 'mass_source_type_total_mass_flow_rate_pvt_split']),
+        Optional("volumetric_flow_rates_std_input_type"): Enum(['constant', 'curve']),
         Optional("volumetric_flow_rates_std"): MapPattern(Str(), Map({"value": Float(), "unit": Str()})),
+        Optional("volumetric_flow_rates_std_curve"): MapPattern(
+            Str(),
+            Map(
+                {
+                    "image": Map({"values": Seq(Float()), "unit": Str()}),
+                    "domain": Map({"values": Seq(Float()), "unit": Str()}),
+                }
+            ),
+        ),
+        Optional("mass_flow_rates_input_type"): Enum(['constant', 'curve']),
         Optional("mass_flow_rates"): MapPattern(Str(), Map({"value": Float(), "unit": Str()})),
+        Optional("mass_flow_rates_curve"): MapPattern(
+            Str(),
+            Map(
+                {
+                    "image": Map({"values": Seq(Float()), "unit": Str()}),
+                    "domain": Map({"values": Seq(Float()), "unit": Str()}),
+                }
+            ),
+        ),
+        Optional("total_mass_flow_rate_input_type"): Enum(['constant', 'curve']),
         Optional("total_mass_flow_rate"): Map({"value": Float(), "unit": Str()}),
+        Optional("total_mass_flow_rate_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
+        Optional("water_cut_input_type"): Enum(['constant', 'curve']),
         Optional("water_cut"): Map({"value": Float(), "unit": Str()}),
+        Optional("water_cut_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
+        Optional("gas_oil_ratio_input_type"): Enum(['constant', 'curve']),
         Optional("gas_oil_ratio"): Map({"value": Float(), "unit": Str()}),
+        Optional("gas_oil_ratio_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
         "position": Map({"value": Float(), "unit": Str()}),
     }
 )
 mass_source_node_properties_description_schema = Map(
     {
         Optional("fluid"): Str(),
         Optional("tracer_mass_fraction"): Map({"values": Seq(Float()), "unit": Str()}),
+        Optional("temperature_input_type"): Enum(['constant', 'curve']),
         Optional("temperature"): Map({"value": Float(), "unit": Str()}),
+        Optional("temperature_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
         Optional("source_type"): Enum(['mass_source_type_mass_flow_rates', 'mass_source_type_all_volumetric_flow_rates', 'mass_source_type_flow_rate_oil_gor_wc', 'mass_source_type_flow_rate_gas_gor_wc', 'mass_source_type_flow_rate_water_gor_wc', 'mass_source_type_total_mass_flow_rate_pvt_split']),
+        Optional("volumetric_flow_rates_std_input_type"): Enum(['constant', 'curve']),
         Optional("volumetric_flow_rates_std"): MapPattern(Str(), Map({"value": Float(), "unit": Str()})),
+        Optional("volumetric_flow_rates_std_curve"): MapPattern(
+            Str(),
+            Map(
+                {
+                    "image": Map({"values": Seq(Float()), "unit": Str()}),
+                    "domain": Map({"values": Seq(Float()), "unit": Str()}),
+                }
+            ),
+        ),
+        Optional("mass_flow_rates_input_type"): Enum(['constant', 'curve']),
         Optional("mass_flow_rates"): MapPattern(Str(), Map({"value": Float(), "unit": Str()})),
+        Optional("mass_flow_rates_curve"): MapPattern(
+            Str(),
+            Map(
+                {
+                    "image": Map({"values": Seq(Float()), "unit": Str()}),
+                    "domain": Map({"values": Seq(Float()), "unit": Str()}),
+                }
+            ),
+        ),
+        Optional("total_mass_flow_rate_input_type"): Enum(['constant', 'curve']),
         Optional("total_mass_flow_rate"): Map({"value": Float(), "unit": Str()}),
+        Optional("total_mass_flow_rate_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
+        Optional("water_cut_input_type"): Enum(['constant', 'curve']),
         Optional("water_cut"): Map({"value": Float(), "unit": Str()}),
+        Optional("water_cut_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
+        Optional("gas_oil_ratio_input_type"): Enum(['constant', 'curve']),
         Optional("gas_oil_ratio"): Map({"value": Float(), "unit": Str()}),
+        Optional("gas_oil_ratio_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
     }
 )
 material_description_schema = Map(
     {
         "name": Str(),
         Optional("material_type"): Enum(['solid', 'fluid']),
         Optional("density"): Map({"value": Float(), "unit": Str()}),
@@ -190,92 +381,234 @@
         Optional("divergence_tolerance"): Float(),
         Optional("friction_factor_evaluation_strategy"): Enum(['time_explicit', 'newton_explicit', 'implicit']),
         Optional("simulation_mode"): Enum(['default', 'robust']),
         Optional("enable_solver_caching"): Bool(),
         Optional("caching_rtol"): Float(),
         Optional("caching_atol"): Float(),
         Optional("always_repeat_timestep"): Bool(),
+        Optional("enable_fast_compositional"): Bool(),
     }
 )
 open_hole_description_schema = Map(
     {
         "name": Str(),
         "length": Map({"value": Float(), "unit": Str()}),
         "diameter": Map({"value": Float(), "unit": Str()}),
         "inner_roughness": Map({"value": Float(), "unit": Str()}),
     }
 )
-opening_curve_description_schema = Map(
+overall_pipe_trend_description_schema = Map(
     {
-        Optional("time"): Map({"values": Seq(Float()), "unit": Str()}),
-        Optional("opening"): Map({"values": Seq(Float()), "unit": Str()}),
+        Optional("name"): Str(),
+        "curve_names": Seq(Str()),
+        "location": Enum(['main', 'annulus', 'not_defined']),
+        "element_name": Str(),
     }
 )
 packer_description_schema = Map(
     {
         "name": Str(),
         "position": Map({"value": Float(), "unit": Str()}),
         Optional("material_above"): Str(),
     }
 )
 physics_description_schema = Map(
     {
         Optional("hydrodynamic_model"): Enum(['hydrodynamic_model_2_fields', 'hydrodynamic_model_4_fields', 'hydrodynamic_model_3_layers_gas_oil_water', 'hydrodynamic_model_5_fields_solid', 'hydrodynamic_model_5_fields_water', 'hydrodynamic_model_5_fields_co2', 'hydrodynamic_model_3_layers_no_bubble_gas_oil_water', 'hydrodynamic_model_3_layers_water_with_co2', 'hydrodynamic_model_3_layers_7_fields_gas_oil_water', 'hydrodynamic_model_3_layers_9_fields_gas_oil_water']),
         Optional("simulation_regime"): Enum(['simulation_regime_transient', 'simulation_regime_steady_state']),
         Optional("energy_model"): Enum(['no_model', 'global_model', 'layers_model']),
-        Optional("solids_model"): Enum(['no_model', 'thomas1965_equilibrium', 'mills1985_equilibrium', 'santamaria2010_equilibrium']),
+        Optional("solids_model"): Enum(['no_model', 'thomas1965_equilibrium', 'mills1985_equilibrium', 'santamaria2010_equilibrium', 'from_plugin']),
+        Optional("solids_model_plugin_id"): Str(),
         Optional("initial_condition_strategy"): Enum(['constant', 'steady_state', 'restart']),
         Optional("restart_filepath"): Str(),
         Optional("keep_former_results"): Bool(),
-        Optional("emulsion_model"): Enum(['no_model', 'model_default', 'taylor1932', 'brinkman1952', 'mooney1951a', 'mooney1951b', 'hinze1955', 'sleicher1962', 'brauner2001', 'boxall2012', 'brinkman1952_and_yeh1964', 'from_plugin']),
+        Optional("emulsion_model_enabled"): Bool(),
+        Optional("emulsion_relative_viscosity_model"): Enum(['model_default', 'taylor1932', 'brinkman1952', 'mooney1951a', 'mooney1951b', 'pal_rhodes1989', 'ronningsen1995', 'volumetric_weight', 'woelflin_1942', 'barnea_mizrahi1976', 'table_based', 'from_plugin']),
+        Optional("emulsion_pal_rhodes_phi_rel_100"): Map({"value": Float(), "unit": Str()}),
+        Optional("emulsion_woelflin_a"): Map({"value": Float(), "unit": Str()}),
+        Optional("emulsion_woelflin_b"): Map({"value": Float(), "unit": Str()}),
+        Optional("emulsion_table_based_rel_visc_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
+        Optional("emulsion_relative_viscosity_tuning_factor"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
+        Optional("emulsion_droplet_size_model"): Enum(['model_default', 'hinze1955', 'sleicher1962', 'brauner2001', 'boxall2012']),
+        Optional("emulsion_inversion_point_model"): Enum(['model_default', 'brauner_and_ullmann_2002', 'brinkman1952_and_yeh1964', 'constant']),
+        Optional("emulsion_inversion_water_cut"): Map({"value": Float(), "unit": Str()}),
         Optional("flash_model"): Enum(['hydrocarbon_only', 'hydrocarbon_and_water']),
         Optional("correlations_package"): Enum(['correlation_package_classical', 'correlation_package_alfasim', 'correlation_package_isdb_tests']),
     }
 )
+pig_equipment_description_schema = Map(
+    {
+        "diameter": Map({"value": Float(), "unit": Str()}),
+        "position": Map({"value": Float(), "unit": Str()}),
+        Optional("launch_times"): Map({"values": Seq(Float()), "unit": Str()}),
+        Optional("mass_input_type"): Enum(['constant', 'curve']),
+        Optional("mass"): Map({"value": Float(), "unit": Str()}),
+        Optional("mass_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
+        Optional("static_force_input_type"): Enum(['constant', 'curve']),
+        Optional("static_force"): Map({"value": Float(), "unit": Str()}),
+        Optional("static_force_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
+        Optional("wall_friction_input_type"): Enum(['constant', 'curve']),
+        Optional("wall_friction"): Map({"value": Float(), "unit": Str()}),
+        Optional("wall_friction_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
+        Optional("linear_friction_input_type"): Enum(['constant', 'curve']),
+        Optional("linear_friction"): Map({"value": Float(), "unit": Str()}),
+        Optional("linear_friction_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
+        Optional("quadratic_friction_input_type"): Enum(['constant', 'curve']),
+        Optional("quadratic_friction"): Map({"value": Float(), "unit": Str()}),
+        Optional("quadratic_friction_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
+        Optional("trap_mode"): Enum(['automatic', 'user_defined']),
+        Optional("trap_position"): Map({"value": Float(), "unit": Str()}),
+        Optional("trap_pipe_name"): Str(),
+        Optional("route_mode"): Enum(['automatic', 'user_defined']),
+        Optional("pipe_route_names"): Seq(Str()),
+    }
+)
 pipe_segments_description_schema = Map(
     {
         "start_positions": Map({"values": Seq(Float()), "unit": Str()}),
         "diameters": Map({"values": Seq(Float()), "unit": Str()}),
         "roughnesses": Map({"values": Seq(Float()), "unit": Str()}),
         Optional("wall_names"): Seq(Str()),
     }
 )
+plugin_description_schema = Map(
+    {
+        Optional("name"): Str(),
+        Optional("gui_models"): MapPattern(Str(), Any()),
+        Optional("is_enabled"): Bool(),
+    }
+)
 pressure_container_description_schema = Map(
     {
         Optional("positions"): Map({"values": Seq(Float()), "unit": Str()}),
         Optional("pressures"): Map({"values": Seq(Float()), "unit": Str()}),
     }
 )
 pressure_node_properties_description_schema = Map(
     {
+        Optional("pressure_input_type"): Enum(['constant', 'curve']),
         Optional("pressure"): Map({"value": Float(), "unit": Str()}),
+        Optional("pressure_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
+        Optional("temperature_input_type"): Enum(['constant', 'curve']),
         Optional("temperature"): Map({"value": Float(), "unit": Str()}),
+        Optional("temperature_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
         Optional("fluid"): Str(),
         Optional("tracer_mass_fraction"): Map({"values": Seq(Float()), "unit": Str()}),
         Optional("split_type"): Enum(['mass_inflow_split_type_constant_volume_fraction', 'mass_inflow_split_type_constant_mass_fraction', 'mass_inflow_split_type_pvt', 'mass_inflow_split_type_pvt_user_gor_wc', 'mass_inflow_split_type_pvt_user_glr_wc']),
+        Optional("mass_fractions_input_type"): Enum(['constant', 'curve']),
         Optional("mass_fractions"): MapPattern(Str(), Map({"value": Float(), "unit": Str()})),
+        Optional("mass_fractions_curve"): MapPattern(
+            Str(),
+            Map(
+                {
+                    "image": Map({"values": Seq(Float()), "unit": Str()}),
+                    "domain": Map({"values": Seq(Float()), "unit": Str()}),
+                }
+            ),
+        ),
+        Optional("volume_fractions_input_type"): Enum(['constant', 'curve']),
         Optional("volume_fractions"): MapPattern(Str(), Map({"value": Float(), "unit": Str()})),
+        Optional("volume_fractions_curve"): MapPattern(
+            Str(),
+            Map(
+                {
+                    "image": Map({"values": Seq(Float()), "unit": Str()}),
+                    "domain": Map({"values": Seq(Float()), "unit": Str()}),
+                }
+            ),
+        ),
+        Optional("gas_liquid_ratio_input_type"): Enum(['constant', 'curve']),
         Optional("gas_liquid_ratio"): Map({"value": Float(), "unit": Str()}),
+        Optional("gas_liquid_ratio_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
+        Optional("gas_oil_ratio_input_type"): Enum(['constant', 'curve']),
         Optional("gas_oil_ratio"): Map({"value": Float(), "unit": Str()}),
+        Optional("gas_oil_ratio_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
+        Optional("water_cut_input_type"): Enum(['constant', 'curve']),
         Optional("water_cut"): Map({"value": Float(), "unit": Str()}),
+        Optional("water_cut_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
     }
 )
 profile_output_description_schema = Map(
     {
         "curve_names": Seq(Str()),
+        "location": Enum(['main', 'annulus', 'not_defined']),
         "element_name": Str(),
-        "location": Enum(['main', 'annulus']),
     }
 )
 pvt_model_correlation_description_schema = Map(
     {
         Optional("oil_density_std"): Map({"value": Float(), "unit": Str()}),
         Optional("gas_density_std"): Map({"value": Float(), "unit": Str()}),
         Optional("rs_sat"): Map({"value": Float(), "unit": Str()}),
         Optional("pvt_correlation_package"): Enum(['pvt_correlation_package_lasater', 'pvt_correlation_package_standing', 'pvt_correlation_package_vazquez_beggs', 'pvt_correlation_package_glaso']),
+        Optional("h2s_mol_frac"): Map({"value": Float(), "unit": Str()}),
+        Optional("co2_mol_frac"): Map({"value": Float(), "unit": Str()}),
+        Optional("oil_viscosity"): Enum(['Egbogah']),
+        Optional("gas_viscosity"): Enum(['Lee Gonzalez Eakin']),
+        Optional("surface_tension"): Enum(['Baker Swerdloff']),
     }
 )
 referenced_pressure_container_description_schema = Map(
     {
         Optional("reference_coordinate"): Map({"value": Float(), "unit": Str()}),
         Optional("positions"): Map({"values": Seq(Float()), "unit": Str()}),
         Optional("pressures"): Map({"values": Seq(Float()), "unit": Str()}),
@@ -307,24 +640,79 @@
         Optional("reference_coordinate"): Map({"value": Float(), "unit": Str()}),
         Optional("positions"): Map({"values": Seq(Float()), "unit": Str()}),
         Optional("fractions"): MapPattern(Str(), Map({"values": Seq(Float()), "unit": Str()})),
     }
 )
 reservoir_inflow_equipment_description_schema = Map(
     {
+        Optional("pressure_input_type"): Enum(['constant', 'curve']),
         Optional("pressure"): Map({"value": Float(), "unit": Str()}),
+        Optional("pressure_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
+        Optional("temperature_input_type"): Enum(['constant', 'curve']),
         Optional("temperature"): Map({"value": Float(), "unit": Str()}),
+        Optional("temperature_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
         Optional("fluid"): Str(),
         Optional("tracer_mass_fraction"): Map({"values": Seq(Float()), "unit": Str()}),
         Optional("split_type"): Enum(['mass_inflow_split_type_constant_volume_fraction', 'mass_inflow_split_type_constant_mass_fraction', 'mass_inflow_split_type_pvt', 'mass_inflow_split_type_pvt_user_gor_wc', 'mass_inflow_split_type_pvt_user_glr_wc']),
+        Optional("mass_fractions_input_type"): Enum(['constant', 'curve']),
         Optional("mass_fractions"): MapPattern(Str(), Map({"value": Float(), "unit": Str()})),
+        Optional("mass_fractions_curve"): MapPattern(
+            Str(),
+            Map(
+                {
+                    "image": Map({"values": Seq(Float()), "unit": Str()}),
+                    "domain": Map({"values": Seq(Float()), "unit": Str()}),
+                }
+            ),
+        ),
+        Optional("volume_fractions_input_type"): Enum(['constant', 'curve']),
         Optional("volume_fractions"): MapPattern(Str(), Map({"value": Float(), "unit": Str()})),
+        Optional("volume_fractions_curve"): MapPattern(
+            Str(),
+            Map(
+                {
+                    "image": Map({"values": Seq(Float()), "unit": Str()}),
+                    "domain": Map({"values": Seq(Float()), "unit": Str()}),
+                }
+            ),
+        ),
+        Optional("gas_liquid_ratio_input_type"): Enum(['constant', 'curve']),
         Optional("gas_liquid_ratio"): Map({"value": Float(), "unit": Str()}),
+        Optional("gas_liquid_ratio_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
+        Optional("gas_oil_ratio_input_type"): Enum(['constant', 'curve']),
         Optional("gas_oil_ratio"): Map({"value": Float(), "unit": Str()}),
+        Optional("gas_oil_ratio_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
+        Optional("water_cut_input_type"): Enum(['constant', 'curve']),
         Optional("water_cut"): Map({"value": Float(), "unit": Str()}),
+        Optional("water_cut_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
         "start": Map({"value": Float(), "unit": Str()}),
         "length": Map({"value": Float(), "unit": Str()}),
         Optional("productivity_ipr"): Str(),
         Optional("injectivity_ipr"): Str(),
     }
 )
 separator_node_properties_description_schema = Map(
@@ -336,26 +724,45 @@
         Optional("diameter"): Map({"value": Float(), "unit": Str()}),
         Optional("nozzles"): MapPattern(Str(), Map({"value": Float(), "unit": Str()})),
         Optional("initial_phase_volume_fractions"): MapPattern(Str(), Map({"value": Float(), "unit": Str()})),
         Optional("gas_separation_efficiency"): Map({"value": Float(), "unit": Str()}),
         Optional("liquid_separation_efficiency"): Map({"value": Float(), "unit": Str()}),
     }
 )
+separator_trend_description_schema = Map(
+    {
+        Optional("name"): Str(),
+        "curve_names": Seq(Str()),
+        "element_name": Str(),
+    }
+)
 speed_curve_description_schema = Map(
     {
         Optional("time"): Map({"values": Seq(Float()), "unit": Str()}),
         Optional("speed"): Map({"values": Seq(Float()), "unit": Str()}),
     }
 )
+surge_volume_options_description_schema = Map(
+    {
+        Optional("time_mode"): Enum(['all_simulation', 'user_defined']),
+        Optional("drainage_mode"): Enum(['automatic', 'user_defined']),
+        Optional("start_time"): Map({"value": Float(), "unit": Str()}),
+        Optional("end_time"): Map({"value": Float(), "unit": Str()}),
+        Optional("maximum_drainage_rate"): Map({"value": Float(), "unit": Str()}),
+    }
+)
 table_pump_description_schema = Map(
     {
         Optional("speeds"): Map({"values": Seq(Float()), "unit": Str()}),
         Optional("void_fractions"): Map({"values": Seq(Float()), "unit": Str()}),
         Optional("flow_rates"): Map({"values": Seq(Float()), "unit": Str()}),
         Optional("pressure_boosts"): Map({"values": Seq(Float()), "unit": Str()}),
+        Optional("heads"): Map({"values": Seq(Float()), "unit": Str()}),
+        Optional("efficiencies"): Map({"values": Seq(Float()), "unit": Str()}),
+        Optional("powers"): Map({"values": Seq(Float()), "unit": Str()}),
     }
 )
 temperatures_container_description_schema = Map(
     {
         Optional("positions"): Map({"values": Seq(Float()), "unit": Str()}),
         Optional("temperatures"): Map({"values": Seq(Float()), "unit": Str()}),
     }
@@ -380,22 +787,14 @@
 )
 tracers_mass_fractions_container_description_schema = Map(
     {
         Optional("positions"): Map({"values": Seq(Float()), "unit": Str()}),
         Optional("tracers_mass_fractions"): Seq(Map({"values": Seq(Float()), "unit": Str()})),
     }
 )
-trend_output_description_schema = Map(
-    {
-        "curve_names": Seq(Str()),
-        "element_name": Str(),
-        "position": Map({"value": Float(), "unit": Str()}),
-        "location": Enum(['main', 'annulus']),
-    }
-)
 tubing_description_schema = Map(
     {
         "name": Str(),
         "length": Map({"value": Float(), "unit": Str()}),
         "outer_diameter": Map({"value": Float(), "unit": Str()}),
         "inner_diameter": Map({"value": Float(), "unit": Str()}),
         "inner_roughness": Map({"value": Float(), "unit": Str()}),
@@ -404,14 +803,28 @@
 )
 velocities_container_description_schema = Map(
     {
         Optional("positions"): Map({"values": Seq(Float()), "unit": Str()}),
         Optional("velocities"): MapPattern(Str(), Map({"values": Seq(Float()), "unit": Str()})),
     }
 )
+vogel_ipr_description_schema = Map(
+    {
+        Optional("well_index_phase"): Enum(['well_index_phase_gas', 'well_index_phase_oil', 'well_index_phase_water', 'well_index_phase_liquid']),
+        Optional("min_pressure_difference"): Map({"value": Float(), "unit": Str()}),
+        Optional("well_max_flow_rate_input_type"): Enum(['constant', 'curve']),
+        Optional("well_max_flow_rate"): Map({"value": Float(), "unit": Str()}),
+        Optional("well_max_flow_rate_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
+    }
+)
 volume_fractions_container_description_schema = Map(
     {
         Optional("positions"): Map({"values": Seq(Float()), "unit": Str()}),
         Optional("fractions"): MapPattern(Str(), Map({"values": Seq(Float()), "unit": Str()})),
     }
 )
 wall_layer_description_schema = Map(
@@ -423,60 +836,61 @@
 )
 x_and_y_description_schema = Map(
     {
         Optional("x"): Map({"values": Seq(Float()), "unit": Str()}),
         Optional("y"): Map({"values": Seq(Float()), "unit": Str()}),
     }
 )
-case_output_description_schema = Map(
-    {
-        Optional("automatic_trend_frequency"): Bool(),
-        Optional("trends"): Seq(trend_output_description_schema),
-        Optional("trend_frequency"): Map({"value": Float(), "unit": Str()}),
-        Optional("automatic_profile_frequency"): Bool(),
-        Optional("profiles"): Seq(profile_output_description_schema),
-        Optional("profile_frequency"): Map({"value": Float(), "unit": Str()}),
-    }
-)
 casing_description_schema = Map(
     {
         Optional("casing_sections"): Seq(casing_section_description_schema),
         Optional("tubings"): Seq(tubing_description_schema),
         Optional("packers"): Seq(packer_description_schema),
         Optional("open_holes"): Seq(open_hole_description_schema),
     }
 )
+compositional_fluid_description_schema = Map(
+    {
+        Optional("composition"): Seq(composition_description_schema),
+        Optional("fraction_pairs"): Seq(bip_description_schema),
+    }
+)
 compressor_equipment_description_schema = Map(
     {
         "position": Map({"value": Float(), "unit": Str()}),
         Optional("speed_curve"): speed_curve_description_schema,
         Optional("reference_pressure"): Map({"value": Float(), "unit": Str()}),
         Optional("reference_temperature"): Map({"value": Float(), "unit": Str()}),
         Optional("constant_speed"): Map({"value": Float(), "unit": Str()}),
         Optional("compressor_type"): Enum(['speed_curve', 'constant_speed']),
         Optional("speed_curve_interpolation_type"): Enum(['constant', 'linear', 'quadratic']),
         Optional("flow_direction"): Enum(['forward', 'backward']),
         Optional("table"): compressor_pressure_table_description_schema,
     }
 )
+controller_node_properties_description_schema = Map(
+    {
+        Optional("type"): Enum(['pid']),
+        Optional("gain"): Float(),
+        Optional("setpoint"): Float(),
+        Optional("integral_time"): Map({"value": Float(), "unit": Str()}),
+        Optional("derivative_time"): Map({"value": Float(), "unit": Str()}),
+        Optional("input_signal_properties"): controller_input_signal_properties_description_schema,
+        Optional("output_signal_properties"): controller_output_signal_properties_description_schema,
+    }
+)
 environment_description_schema = Map(
     {
         Optional("thermal_model"): Enum(['adiabatic_walls', 'steady_state_heat_transfer', 'transient_heat_transfer']),
         Optional("position_input_mode"): Enum(['position_by_tvd', 'position_by_md']),
         Optional("reference_y_coordinate"): Map({"value": Float(), "unit": Str()}),
         Optional("md_properties_table"): Seq(environment_property_description_schema),
         Optional("tvd_properties_table"): Seq(environment_property_description_schema),
     }
 )
-fluid_description_schema = Map(
-    {
-        Optional("composition"): Seq(composition_description_schema),
-        Optional("fraction_pairs"): Seq(bip_description_schema),
-    }
-)
 formation_description_schema = Map(
     {
         "reference_y_coordinate": Map({"value": Float(), "unit": Str()}),
         Optional("layers"): Seq(formation_layer_description_schema),
     }
 )
 initial_pressures_description_schema = Map(
@@ -515,41 +929,91 @@
     {
         Optional("position_input_type"): Enum(['vertical_position', 'horizontal_position', 'length']),
         Optional("table_x"): referenced_volume_fractions_container_description_schema,
         Optional("table_y"): referenced_volume_fractions_container_description_schema,
         Optional("table_length"): volume_fractions_container_description_schema,
     }
 )
-node_description_schema = Map(
+leak_equipment_description_schema = Map(
     {
-        "name": Str(),
-        "node_type": Enum(['internal_node', 'mass_source_boundary', 'pressure_boundary', 'separator_node']),
-        Optional("pvt_model"): Str(),
-        Optional("pressure_properties"): pressure_node_properties_description_schema,
-        Optional("mass_source_properties"): mass_source_node_properties_description_schema,
-        Optional("internal_properties"): internal_node_properties_description_schema,
-        Optional("separator_properties"): separator_node_properties_description_schema,
+        "position": Map({"value": Float(), "unit": Str()}),
+        Optional("location"): Enum(['main', 'annulus', 'not_defined']),
+        Optional("model"): Enum(['orifice', 'flow_coefficient', 'gas_lift_valve']),
+        Optional("type"): Enum(['internal', 'external']),
+        Optional("diameter"): Map({"value": Float(), "unit": Str()}),
+        Optional("discharge_coefficient"): Map({"value": Float(), "unit": Str()}),
+        Optional("cv_table"): cv_table_description_schema,
+        Optional("gas_lift_valve_opening_type"): Enum(['minimum_pressure_difference', 'pressure_operated']),
+        Optional("minimum_pressure_difference"): Map({"value": Float(), "unit": Str()}),
+        Optional("bellows_reference_pressure"): Map({"value": Float(), "unit": Str()}),
+        Optional("bellows_reference_temperature"): Map({"value": Float(), "unit": Str()}),
+        Optional("port_to_bellows_area_ratio"): Map({"value": Float(), "unit": Str()}),
+        Optional("opening_input_type"): Enum(['constant', 'curve']),
+        Optional("opening"): Map({"value": Float(), "unit": Str()}),
+        Optional("opening_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
+        Optional("target_pipe_name"): Str(),
+        Optional("target_position"): Map({"value": Float(), "unit": Str()}),
+        Optional("target_location"): Enum(['main', 'annulus', 'not_defined']),
+        Optional("backflow"): Bool(),
+        Optional("backpressure"): Map({"value": Float(), "unit": Str()}),
+    }
+)
+positional_pipe_trend_description_schema = Map(
+    {
+        Optional("name"): Str(),
+        "curve_names": Seq(Str()),
+        "location": Enum(['main', 'annulus', 'not_defined']),
+        "position": Map({"value": Float(), "unit": Str()}),
+        "element_name": Str(),
+        Optional("surge_volume_options"): surge_volume_options_description_schema,
     }
 )
 profile_description_schema = Map(
     {
         Optional("x_and_y"): x_and_y_description_schema,
         Optional("length_and_elevation"): length_and_elevation_description_schema,
     }
 )
 pump_equipment_description_schema = Map(
     {
         "position": Map({"value": Float(), "unit": Str()}),
-        Optional("type"): Enum(['constant_pressure', 'table_interpolation']),
-        Optional("pressure_boost"): Map({"value": Float(), "unit": Str()}),
+        Optional("flow_direction"): Enum(['forward', 'backward']),
         Optional("thermal_efficiency"): Map({"value": Float(), "unit": Str()}),
+        Optional("thermal_efficiency_model"): Enum(['constant', 'efficiency_curve_based']),
+        Optional("type"): Enum(['constant_pressure', 'table_interpolation', 'electric_submersible_pump']),
+        Optional("pressure_boost"): Map({"value": Float(), "unit": Str()}),
         Optional("table"): table_pump_description_schema,
         Optional("speed_curve"): speed_curve_description_schema,
         Optional("speed_curve_interpolation_type"): Enum(['constant', 'linear', 'quadratic']),
-        Optional("flow_direction"): Enum(['forward', 'backward']),
+        Optional("esp_table"): table_pump_description_schema,
+        Optional("esp_speed_input_type"): Enum(['constant', 'curve']),
+        Optional("esp_speed"): Map({"value": Float(), "unit": Str()}),
+        Optional("esp_speed_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
+        Optional("esp_number_of_stages"): Int(),
+        Optional("esp_reference_density"): Map({"value": Float(), "unit": Str()}),
+        Optional("esp_manufacturer"): Str(),
+        Optional("esp_model"): Str(),
+        Optional("esp_viscosity_model"): Enum(['no_model', 'ansihi_2010']),
+        Optional("density_correction_enabled"): Bool(),
+    }
+)
+pvt_model_combined_description_schema = Map(
+    {
+        Optional("reference_pvt_model"): Str(),
+        Optional("fluids"): MapPattern(Str(), combined_fluid_description_schema),
     }
 )
 table_ipr_description_schema = Map(
     {
         Optional("well_index_phase"): Enum(['well_index_phase_gas', 'well_index_phase_oil', 'well_index_phase_water', 'well_index_phase_liquid']),
         Optional("table"): ipr_curve_description_schema,
     }
@@ -564,91 +1028,142 @@
         "position": Map({"value": Float(), "unit": Str()}),
         Optional("type"): Enum(['perkins_valve', 'choke_valve_with_flow_coefficient', 'check_valve']),
         Optional("diameter"): Map({"value": Float(), "unit": Str()}),
         Optional("flow_direction"): Enum(['forward', 'backward']),
         Optional("opening_type"): Enum(['constant_opening', 'table_interpolation']),
         Optional("opening"): Map({"value": Float(), "unit": Str()}),
         Optional("opening_curve_interpolation_type"): Enum(['constant', 'linear', 'quadratic']),
-        Optional("opening_curve"): opening_curve_description_schema,
+        Optional("opening_curve"): Map(
+            {
+                "image": Map({"values": Seq(Float()), "unit": Str()}),
+                "domain": Map({"values": Seq(Float()), "unit": Str()}),
+            }
+        ),
         Optional("cv_table"): cv_table_description_schema,
     }
 )
 wall_description_schema = Map(
     {
         "name": Str(),
         Optional("inner_roughness"): Map({"value": Float(), "unit": Str()}),
         Optional("wall_layer_container"): Seq(wall_layer_description_schema),
     }
 )
+annulus_equipment_description_schema = Map(
+    {
+        Optional("leaks"): MapPattern(Str(), leak_equipment_description_schema),
+        Optional("gas_lift_valves"): MapPattern(Str(), gas_lift_valve_equipment_description_schema),
+    }
+)
 equipment_description_schema = Map(
     {
         Optional("mass_sources"): MapPattern(Str(), mass_source_equipment_description_schema),
         Optional("pumps"): MapPattern(Str(), pump_equipment_description_schema),
         Optional("valves"): MapPattern(Str(), valve_equipment_description_schema),
         Optional("reservoir_inflows"): MapPattern(Str(), reservoir_inflow_equipment_description_schema),
         Optional("heat_sources"): MapPattern(Str(), heat_source_equipment_description_schema),
         Optional("compressors"): MapPattern(Str(), compressor_equipment_description_schema),
+        Optional("leaks"): MapPattern(Str(), leak_equipment_description_schema),
+        Optional("pigs"): MapPattern(Str(), pig_equipment_description_schema),
     }
 )
 ipr_models_description_schema = Map(
     {
         Optional("linear_models"): MapPattern(Str(), linear_ipr_description_schema),
+        Optional("vogel_models"): MapPattern(Str(), vogel_ipr_description_schema),
+        Optional("fetkovich_models"): MapPattern(Str(), fetkovich_ipr_description_schema),
+        Optional("forchheimer_models"): MapPattern(Str(), forchheimer_ipr_description_schema),
         Optional("table_models"): MapPattern(Str(), table_ipr_description_schema),
     }
 )
 initial_conditions_description_schema = Map(
     {
         Optional("pressures"): initial_pressures_description_schema,
         Optional("volume_fractions"): initial_volume_fractions_description_schema,
         Optional("tracers_mass_fractions"): initial_tracers_mass_fractions_description_schema,
         Optional("velocities"): initial_velocities_description_schema,
         Optional("temperatures"): initial_temperatures_description_schema,
         Optional("fluid"): Str(),
     }
 )
+node_description_schema = Map(
+    {
+        "name": Str(),
+        "node_type": Enum(['internal_node', 'mass_source_boundary', 'pressure_boundary', 'separator_node', 'controller_node']),
+        Optional("pvt_model"): Str(),
+        Optional("pressure_properties"): pressure_node_properties_description_schema,
+        Optional("mass_source_properties"): mass_source_node_properties_description_schema,
+        Optional("internal_properties"): internal_node_properties_description_schema,
+        Optional("separator_properties"): separator_node_properties_description_schema,
+        Optional("controller_properties"): controller_node_properties_description_schema,
+    }
+)
 pvt_model_compositional_description_schema = Map(
     {
         Optional("equation_of_state_type"): Enum(['pvt_compositional_peng_robinson', 'pvt_compositional_soave_redlich_kwong']),
         Optional("surface_tension_model_type"): Enum(['WeinaugKatz', 'LeeChien', 'SchechterGuo']),
         Optional("viscosity_model"): Enum(['corresponding_states_principle', 'lohrenz_bray_clark']),
         Optional("heavy_components"): Seq(heavy_component_description_schema),
         Optional("light_components"): Seq(light_component_description_schema),
-        Optional("fluids"): MapPattern(Str(), fluid_description_schema),
+        Optional("fluids"): MapPattern(Str(), compositional_fluid_description_schema),
+    }
+)
+trends_output_description_schema = Map(
+    {
+        Optional("positional_pipe_trends"): Seq(positional_pipe_trend_description_schema),
+        Optional("overall_pipe_trends"): Seq(overall_pipe_trend_description_schema),
+        Optional("global_trends"): Seq(global_trend_description_schema),
+        Optional("equipment_trends"): Seq(equipment_trend_description_schema),
+        Optional("separator_trends"): Seq(separator_trend_description_schema),
+        Optional("controller_trends"): Seq(controller_trend_description_schema),
     }
 )
 annulus_description_schema = Map(
     {
         "has_annulus_flow": Bool(),
         Optional("pvt_model"): Str(),
         Optional("initial_conditions"): initial_conditions_description_schema,
-        Optional("gas_lift_valve_equipment"): MapPattern(Str(), gas_lift_valve_equipment_description_schema),
+        Optional("equipment"): annulus_equipment_description_schema,
         "top_node": Str(),
     }
 )
+case_output_description_schema = Map(
+    {
+        Optional("automatic_trend_frequency"): Bool(),
+        Optional("trends"): trends_output_description_schema,
+        Optional("trend_frequency"): Map({"value": Float(), "unit": Str()}),
+        Optional("automatic_profile_frequency"): Bool(),
+        Optional("profiles"): Seq(profile_output_description_schema),
+        Optional("profile_frequency"): Map({"value": Float(), "unit": Str()}),
+    }
+)
 pipe_description_schema = Map(
     {
         "name": Str(),
         "source": Str(),
         "target": Str(),
         Optional("source_port"): Enum(['port', 'left_annulus_port', 'right_annulus_port']),
         Optional("target_port"): Enum(['port', 'left_annulus_port', 'right_annulus_port']),
         Optional("pvt_model"): Str(),
         Optional("profile"): profile_description_schema,
         Optional("equipment"): equipment_description_schema,
         Optional("environment"): environment_description_schema,
         Optional("segments"): pipe_segments_description_schema,
         Optional("initial_conditions"): initial_conditions_description_schema,
+        Optional("flow_pattern_model"): Enum(['unit_cell', 'regime_capturing']),
+        Optional("regime_capturing_mesh_threshold"): Map({"value": Float(), "unit": Str()}),
     }
 )
 pvt_models_description_schema = Map(
     {
         Optional("default_model"): Str(),
         Optional("tables"): MapPattern(Str(), Str()),
         Optional("correlations"): MapPattern(Str(), pvt_model_correlation_description_schema),
-        Optional("compositions"): MapPattern(Str(), pvt_model_compositional_description_schema),
+        Optional("compositional"): MapPattern(Str(), pvt_model_compositional_description_schema),
+        Optional("combined"): MapPattern(Str(), pvt_model_combined_description_schema),
     }
 )
 well_description_schema = Map(
     {
         "name": Str(),
         Optional("pvt_model"): Str(),
         Optional("stagnant_fluid"): Str(),
@@ -662,23 +1177,25 @@
         Optional("initial_conditions"): initial_conditions_description_schema,
         Optional("equipment"): equipment_description_schema,
     }
 )
 case_description_schema = Map(
     {
         Optional("name"): Str(),
+        Optional("alfasim_version_info"): alfasim_version_info_schema,
+        Optional("comment"): Str(),
         Optional("physics"): physics_description_schema,
         Optional("time_options"): time_options_description_schema,
         Optional("numerical_options"): numerical_options_description_schema,
+        Optional("plugins"): Seq(plugin_description_schema),
         Optional("ipr_models"): ipr_models_description_schema,
         Optional("pvt_models"): pvt_models_description_schema,
         Optional("tracers"): tracers_description_schema,
         Optional("outputs"): case_output_description_schema,
         Optional("pipes"): Seq(pipe_description_schema),
         Optional("nodes"): Seq(node_description_schema),
         Optional("wells"): Seq(well_description_schema),
         Optional("materials"): Seq(material_description_schema),
         Optional("walls"): Seq(wall_description_schema),
     }
 )
-# [[[end]]] (checksum: 41248460c8164bf2648e6a873c1af78f)
-# fmt: on
+# [[[end]]] (checksum: c3e9dda5b6b211c66aef5f5b6f7ab550)
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/alfacase.py` & `alfasim_sdk-2024.1/src/alfasim_sdk/_internal/alfacase/alfacase.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,67 @@
 from pathlib import Path
 
 from alfasim_sdk._internal.alfacase import case_description
 
 
 def generate_alfacase_file(
     alfacase_description: case_description.CaseDescription, alfacase_file: Path
-):
+) -> None:
     """
     Dump the case_description to the given alfacase_file, using YAML format.
 
     PvtModels that are of mode constants.PVT_MODEL_TABLE will be dumped into a separate file (.alfatable).
     """
+    from alfasim_sdk._internal.alfacase.plugin_alfacase_to_case import (
+        dump_file_contents_and_update_plugins,
+    )
+
     _generate_alfatable_file_for_pvt_models_description(
         alfacase_description.pvt_models, alfacase_file
     )
+    alfacase_description = dump_file_contents_and_update_plugins(
+        alfacase_description, alfacase_file
+    )
+
     alfacase_file_content = convert_description_to_alfacase(alfacase_description)
     alfacase_file.write_text(alfacase_file_content, encoding="utf-8")
 
 
 def _generate_alfatable_file_for_pvt_models_description(
     pvt_models: case_description.PvtModelsDescription, alfacase_file: Path
-):
+) -> None:
     """
     Create `.alfatable` files for each pvt_model which the mode is constants.PVT_MODEL_TABLE.
     """
     from alfasim_sdk import generate_alfatable_file
 
-    for pvt_name, pvt_table_description in pvt_models.table_parameters.items():
+    # TODO: ASIM-4980: generate alfatable files for ph table
+    for pvt_name, pvt_table_description in pvt_models.pt_table_parameters.items():
         alfatable_file = generate_alfatable_file(
             alfacase_file=alfacase_file,
             alfatable_filename=pvt_name,
             description=pvt_table_description,
         )
         pvt_models.tables[pvt_name] = alfatable_file.name
-    pvt_models.table_parameters.clear()
+    pvt_models.pt_table_parameters.clear()
 
 
 def convert_description_to_alfacase(
-    alfacase_description, *, enable_flow_style_on_numpy: bool = False
+    alfacase_description: case_description.CaseDescription,
+    *,
+    enable_flow_style_on_numpy: bool = False,
+    remove_redundant_input_type_data: bool = True,
 ) -> str:
     """
     Convert a given case (decorated with attrs) to YAML representation.
     The strictyaml conversion ("as_yaml") requires that all items from dict are strings.
 
+    :param alfacase_description:
+        Alfasim case description.
+
     :param enable_flow_style_on_numpy:
         Signalize that numpy arrays should dumped with flow style enabled.
 
         enable_flow_style_on_numpy=False
         .. code-block:: python
 
             pressure:
@@ -54,29 +69,34 @@
                 - 2
 
         enable_flow_style_on_numpy=True
        .. code-block:: python
 
             pressure: [1, 2]
 
+    :param remove_redundant_input_type_data:
+        For transient entries remove input type selector, and the unused constant or curve entries.
+
     """
     import attr
     from strictyaml import YAML
     from .case_to_alfacase import convert_dict_to_valid_alfacase_format
 
+    alfacase_description_dict = attr.asdict(alfacase_description, recurse=False)
     case_description_dict = convert_dict_to_valid_alfacase_format(
-        attr.asdict(alfacase_description, recurse=False),
+        alfacase_description_dict,
         enable_flow_style_on_numpy=enable_flow_style_on_numpy,
+        remove_redundant_input_type_data=remove_redundant_input_type_data,
     )
     return YAML(case_description_dict).as_yaml()
 
 
 def convert_alfacase_to_description(
     file_alfacase: Path,
 ) -> case_description.CaseDescription:
     """
-    Return a alfasim_sdk.alfacase.case_description.Case with all information provided on file_yaml.
+    Return a :class:`alfasim_sdk._internal.alfacase.case_description` with all information provided on file_yaml.
     """
     from alfasim_sdk._internal.alfacase.alfacase_to_case import load_case_description
     from alfasim_sdk._internal.alfacase.alfacase_to_case import DescriptionDocument
 
     return load_case_description(DescriptionDocument.from_file(file_alfacase))
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/case_to_alfacase.py` & `alfasim_sdk-2024.1/src/alfasim_sdk/_internal/alfacase/case_to_alfacase.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Union
 
 import attr
 import numpy as np
+from barril.curve.curve import Curve
 from barril.units import Array
 from barril.units import Scalar
 
+from alfasim_sdk import MultiInputType
+from alfasim_sdk._internal import constants
 from alfasim_sdk._internal.alfacase import case_description
 from alfasim_sdk._internal.alfacase.generate_schema import IGNORED_PROPERTIES
 from alfasim_sdk._internal.alfacase.generate_schema import is_attrs
 
-
-ATTRIBUTES = Union[Scalar, Array, Enum, np.ndarray, List, List[Enum]]
-
+ATTRIBUTES = Union[Scalar, Array, Curve, Enum, np.ndarray, List, List[Enum]]
 
 NON_FININTE_VALUES_TO_STRING = [
     (math.isnan, ".nan"),
     (lambda value: math.isinf(value) and value > 0, ".inf"),
     (lambda value: math.isinf(value) and value < 0, "-.inf"),
 ]
 
@@ -33,17 +34,17 @@
 
     This approach was intended to avoid to dump dictionary with curly brackets "{ }"
     and keep a list of strings with block style.
 
     For more details check:
     https://stackoverflow.com/questions/63364894/how-to-dump-only-lists-with-flow-style-with-pyyaml-or-ruamel-yaml
     """
-    import ruamel
+    from strictyaml.ruamel import comments
 
-    retval = ruamel.yaml.comments.CommentedSeq(values)
+    retval = comments.CommentedSeq(values)
 
     if enable_flow_style:
         retval.fa.set_flow_style()
     return retval
 
 
 def _convert_value_to_valid_alfacase_format(
@@ -57,35 +58,45 @@
     """
     if isinstance(value, Scalar):
         return {"value": str(value.value), "unit": value.unit}
 
     if isinstance(value, Array):
         return {"values": [str(i) for i in value.values], "unit": value.unit}
 
+    if isinstance(value, Curve):
+        return {
+            "image": _convert_value_to_valid_alfacase_format(
+                value.image, enable_flow_style_on_numpy
+            ),
+            "domain": _convert_value_to_valid_alfacase_format(
+                value.domain, enable_flow_style_on_numpy
+            ),
+        }
+
     if isinstance(value, Enum):
         return value.value
 
     if isinstance(value, np.ndarray) and value.ndim == 1:
         return format_list(
             values=[str(coefficients) for coefficients in value],
             enable_flow_style=enable_flow_style_on_numpy,
         )
 
     if isinstance(value, list) and all(
-        (isinstance(item, np.ndarray) and item.ndim == 1 for item in value)
+        isinstance(item, np.ndarray) and item.ndim == 1 for item in value
     ):
         return [
             format_list(
                 values=[str(np_value) for np_value in np_array],
                 enable_flow_style=enable_flow_style_on_numpy,
             )
             for np_array in value
         ]
 
-    if isinstance(value, list) and all((isinstance(item, Array) for item in value)):
+    if isinstance(value, list) and all(isinstance(item, Array) for item in value):
         return [
             {"values": [str(i) for i in item.values], "unit": item.unit}
             for item in value
         ]
 
     if isinstance(value, list):
         return [str(i) for i in value]
@@ -101,68 +112,111 @@
 
         return float_formatted_value
 
     return str(value)
 
 
 def convert_dict_to_valid_alfacase_format(
-    case_description_dict: Dict[str, ATTRIBUTES], enable_flow_style_on_numpy: bool
+    case_description_dict: Dict[str, ATTRIBUTES],
+    *,
+    enable_flow_style_on_numpy: bool,
+    remove_redundant_input_type_data: bool = True,
 ) -> Dict[str, Any]:
     """
     Convert all values of the dictionary to string.
 
     Note.: strict_yaml only allows "str" values on all attributes in order to render the YAML content.
 
     :param enable_flow_style_on_numpy:
         Signalize that numpy arrays should dumped with inline list ( pressure: [1, 2] ).
 
+    :param remove_redundant_input_type_data:
+        For transient entries remove input type selector, and the unused constant or curve entries.
     """
+    transient_fields: Dict[str, MultiInputType] = {}
     converted_dict = {}
     for key, value in case_description_dict.items():
         is_empty_dict = isinstance(value, dict) and not value
         ignore = key in IGNORED_PROPERTIES
 
         if is_empty_dict or value is None or ignore:
             continue
 
-        if is_attrs(value):
+        if remove_redundant_input_type_data and isinstance(
+            value, constants.MultiInputType
+        ):
+            assert key.endswith(constants.MULTI_INPUT_TYPE_SUFFIX)
+            transient_fields[key] = value
 
+        if is_attrs(value):
             to_dict = partial(attr.asdict, recurse=False)
 
             if isinstance(value, list):
                 converted_value = [
                     convert_dict_to_valid_alfacase_format(
-                        to_dict(i), enable_flow_style_on_numpy
+                        to_dict(i),
+                        enable_flow_style_on_numpy=enable_flow_style_on_numpy,
+                        remove_redundant_input_type_data=remove_redundant_input_type_data,
                     )
                     for i in value
                 ]
             else:
                 converted_value = convert_dict_to_valid_alfacase_format(
-                    to_dict(value), enable_flow_style_on_numpy
+                    to_dict(value),
+                    enable_flow_style_on_numpy=enable_flow_style_on_numpy,
+                    remove_redundant_input_type_data=remove_redundant_input_type_data,
                 )
 
             if converted_value:
                 converted_dict[key] = converted_value
             continue
 
         if isinstance(value, dict):
             converted_dict[key] = convert_dict_to_valid_alfacase_format(
-                value, enable_flow_style_on_numpy
+                value,
+                enable_flow_style_on_numpy=enable_flow_style_on_numpy,
+                remove_redundant_input_type_data=remove_redundant_input_type_data,
             )
             continue
 
+        if isinstance(value, list) and all(isinstance(item, dict) for item in value):
+            converted_dict[key] = [
+                convert_dict_to_valid_alfacase_format(
+                    item,
+                    enable_flow_style_on_numpy=enable_flow_style_on_numpy,
+                    remove_redundant_input_type_data=remove_redundant_input_type_data,
+                )
+                for item in value
+            ]
+            continue
+
         converted_dict[key] = _convert_value_to_valid_alfacase_format(
             value, enable_flow_style_on_numpy
         )
 
+    if remove_redundant_input_type_data:
+        for key, multi_input_type in transient_fields.items():
+            constant_key = key[: -len(constants.MULTI_INPUT_TYPE_SUFFIX)]
+            curve_key = f"{constant_key}_curve"
+
+            converted_dict.pop(key, None)
+            if multi_input_type == constants.MultiInputType.Constant:
+                converted_dict.pop(curve_key, None)
+            elif multi_input_type == constants.MultiInputType.Curve:
+                converted_dict.pop(constant_key, None)
+            else:  # pragma: no cover
+                raise AssertionError(f"unexpected value {key}: {multi_input_type}")
+
     return converted_dict
 
 
 EquipmentTypes = Union[
     case_description.MassSourceEquipmentDescription,
     case_description.HeatSourceEquipmentDescription,
     case_description.CompressorEquipmentDescription,
     case_description.ReservoirInflowEquipmentDescription,
     case_description.ValveEquipmentDescription,
     case_description.PumpEquipmentDescription,
     case_description.GasLiftValveEquipmentDescription,
+    case_description.LeakEquipmentDescription,
+    case_description.PigEquipmentDescription,
 ]
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/types.py` & `alfasim_sdk-2024.1/src/alfasim_sdk/_internal/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from alfasim_sdk._internal.validators import non_empty_str
 from alfasim_sdk._internal.validators import valid_unit
 
 
 @attr.s(kw_only=True)
 class ALFAsimType:
-    name = attrib(default="ALFAsim")
+    name: str = attrib(default="ALFAsim")
 
 
 @attr.s(kw_only=True)
 class TracerType(ALFAsimType):
     _CONTAINER_TYPE = "TracerModelContainer"
 
 
@@ -48,21 +48,21 @@
 
 
 @attr.s(kw_only=True)
 class BaseField:
     """
     A base field for all types available at ALFAsim.
 
-    :param caption: Label to be displayed on the right side of the component.
+    :ivar caption: Label to be displayed on the right side of the component.
 
-    :param tooltip: Shows a tip, a short piece of text.
+    :ivar tooltip: Shows a tip, a short piece of text.
 
-    :param Callable enable_expr: Function to evaluate if the component will be enabled or not.
+    :ivar enable_expr: Function to evaluate if the component will be enabled or not.
 
-    :param Callable visible_expr: Function to inform if the component will be visible or not.
+    :ivar visible_expr: Function to inform if the component will be visible or not.
 
     .. rubric:: **Caption and Tooltip**:
 
     Caption is the most basic information that all fields must inform, it will display Label over the right side of
     the component on the ``Model Explorer`` window.
 
     Tooltips are short pieces of text to reminder/inform the user about some specificity about the property when they
@@ -104,15 +104,15 @@
 
     .. _enable-expression-section:
 
     .. rubric:: **Enable Expression**:
 
     Accepts a python function that controls either the component will be enabled, or disabled.
     The python function will receive two arguments, an instance of itself (to check local values) and an instance of
-    :func:`alfasim_sdk.context.Context` to retrieve information about the application.
+    :class:`~alfasim_sdk._internal.context.Context` to retrieve information about the application.
 
     This function must return a boolean, informing True (for enabled) or False (for disabled).
 
     .. epigraph:: **enabled**:
         The component will handle keyboard and mouse events.
 
     .. epigraph:: **disabled**:
@@ -149,15 +149,15 @@
 
     .. _visible-expression-section:
 
     .. rubric:: **Visible Expression**:
 
     Accepts a python function that controls either the component will be visible, or not.
     The python function will receive two arguments, an instance of itself (to check local values) and an instance of
-    :func:`alfasim_sdk.context.Context` to retrieve information about the application.
+    :func:`~alfasim_sdk._internal.context.Context` to retrieve information about the application.
 
     This function must return a boolean, informing True (for visible) or False (for invisible).
 
     .. rubric:: Example myplugin.py
 
     .. code-block:: python
         :emphasize-lines: 1-2, 11
@@ -186,15 +186,15 @@
 
     .. image:: /_static/images/api/base_field_visible_expr_1.png
 
     .. image:: /_static/images/api/base_field_visible_expr_2.png
 
     .. Development only
 
-        The BaseField class and all others classes that inheritance from BaseField must use kw_only=True for all attributes.
+        The :class:`~BaseField` class and all others classes that inheritance from it, must use kw_only=True for all attributes.
         This is due to the necessity to make enable_expr and visible_expr an optional value and the only way to have
         properties with default values mixed with required properties is with key-word only arguments.
     """
 
     caption: str = attrib(validator=non_empty_str)
     tooltip: str = attrib(default="", validator=instance_of(str))
     enable_expr: Optional[Callable] = attrib(
@@ -206,17 +206,17 @@
 
 
 @attr.s(kw_only=True)
 class String(BaseField):
     """
     The String field represents an input that allows the user to enter and edit a single line of plain text.
 
-    The String field have all options available from :func:`~alfasim_sdk.types.BaseField`, plus the following ones
+    The String field have all options available from :class:`BaseField`, plus the following ones
 
-    :parameter str value: property to hold the value informed by the user.
+    :ivar value: property to hold the value informed by the user.
 
     .. rubric:: Example myplugin.py
 
     .. code-block:: python
 
         @data_model(icon="", caption="My Plugin")
         class MyModel:
@@ -230,15 +230,15 @@
     .. rubric:: **Accessing String Field from Plugin**:
 
     In order to access this field from inside the plugin implementation, in C/C++  you need to use :cpp:func:`get_plugin_input_data_string_size`
     together with :cpp:func:`get_plugin_input_data_string_size`
 
     .. rubric:: **Accessing String Field from Context**:
 
-    When accessed from the :func:`~alfasim_sdk.context.Context`, the String field will return the currently text as ``str``.
+    When accessed from the :class:`~alfasim_sdk._internal.context.Context`, the String field will return the currently text as ``str``.
 
     .. code-block:: python
 
         >>> ctx.get_model("MyModel").string_field
         'Default Value'
 
         >>> type(ctx.get_model("MyModel").string_field)
@@ -251,18 +251,18 @@
 
 @attr.s(kw_only=True)
 class Enum(BaseField):
     """
     The Enum field provides list of options to the user, showing  only the select item but providing a way to display
     a list of all options through a combo-box.
 
-    The Enum field have all options available from :func:`~alfasim_sdk.types.BaseField`, besides the listed the ones listed above:
+    The Enum field have all options available from :class:`~BaseField`, besides the listed the ones listed above:
 
-    :param values: A list of strings with the available options.
-    :param initial: Indicates which one of the options should be selected per default.
+    :ivar values: A list of strings with the available options.
+    :ivar initial: Indicates which one of the options should be selected per default.
                     If not given, the first item in ``values`` will be used as default.
 
     .. rubric:: Example myplugin.py
 
     .. code-block:: python
 
         @data_model(icon="", caption="My Plugin")
@@ -277,15 +277,15 @@
 
     .. rubric:: **Accessing Enum Field from Plugin**:
 
     In order to access this field from inside the plugin implementation, in C/C++,  you need to use :cpp:func:`get_plugin_input_data_enum`
 
     .. rubric:: **Accessing Enum Field from Context**:
 
-    When accessed from the :func:`~alfasim_sdk.context.Context`, the Enum field will return the currently selected option
+    When accessed from the :class:`~alfasim_sdk._internal.context.Context`, the Enum field will return the currently selected option
     as ``str``.
 
     .. code-block:: python
 
         @data_model(icon="", caption="My Plugin")
         class MyModel:
             enum_field = Enum(
@@ -302,15 +302,15 @@
 
         >>> type(ctx.get_model("MyModel").enum_field)
         <class 'str'>
 
     """
 
     values: List[str] = attrib()
-    initial: str = attrib(validator=optional(instance_of(str)), default=None)
+    initial: Optional[str] = attrib(validator=optional(instance_of(str)), default=None)
 
     @values.validator
     def check(  # pylint: disable=arguments-differ
         self, attr: Attribute, values: List[str]
     ) -> None:
         if not isinstance(values, list):
             raise TypeError(
@@ -329,16 +329,18 @@
                 raise TypeError(
                     "The initial condition must be within the declared values"
                 )
 
 
 @attr.s(kw_only=True)
 class BaseReference(BaseField):
-    ref_type = attrib()
-    container_type = attrib(default=None, validator=optional(non_empty_str))
+    ref_type: type = attrib()
+    container_type: Optional[str] = attrib(
+        default=None, validator=optional(non_empty_str)
+    )
 
     def __attrs_post_init__(self):
         if issubclass(self.ref_type, ALFAsimType):
             self.container_type = self.ref_type._CONTAINER_TYPE
         else:
             if self.container_type is None:
                 raise TypeError(
@@ -371,21 +373,19 @@
 
     :ALFAsimTypes: models from ALFAsim, for example, Tracers.
     :Custom Data: a model defined within the plugin.
 
     .. note::
         In order to reference custom data, the model must be inside a container.
 
-    :param str caption:
-        Property used as a label for the field.
+    :ivar caption: Property used as a label for the field.
 
-    :param ref_type:
-        Property that indicates which type of data the Reference will hold.
+    :ivar ref_type: Property that indicates which type of data the Reference will hold.
 
-    :param container_type:
+    :ivar container_type:
         The name of the class that holds the ref_type, this property must be used when the ``ref_type`` references model from the plugin.
 
     .. rubric:: Example using ``ALFAsimTypes`` on myplugin.py
 
     .. code-block:: python
 
         @data_model(icon="", caption="My Plugin")
@@ -420,15 +420,15 @@
 
     .. rubric:: **Accessing Reference Field from Plugin**:
 
     In order to access this field from inside the plugin implementation, in C/C++,  you need to use :cpp:func:`get_plugin_input_data_reference`
 
     .. rubric:: **Accessing Reference Field from Context**:
 
-    When accessed from the :func:`~alfasim_sdk.context.Context`, the Reference field will return the currently selected option
+    When accessed from the :class:`~alfasim_sdk._internal.context.Context`, the Reference field will return the currently selected option
     object instance.
 
     With the instance, you can access all attributes from the object normally. Check the example below.
 
     .. code-block:: bash
 
         @data_model(caption="My Model")
@@ -463,25 +463,25 @@
 
     """
 
 
 @attr.s(kw_only=True)
 class MultipleReference(BaseReference):
     """
-    The MultipleReference field works similar to :func:`~alfasim_sdk.types.Reference`, providing a list of options
+    The MultipleReference field works similar to :class:`Reference`, providing a list of options
     to the user, but allowing multiple values, of the same type, to be chosen.
 
     There are two types of models supported by this field.
     :ALFAsimTypes: models from ALFAsim, for example, Tracers.
     :Custom Data: a model defined within the plugin.
 
     .. note::
         In order to reference a custom data the model must be inside a container.
 
-    :ivar str caption:
+    :ivar caption:
         Property used as a label for the field.
 
     :ivar ref_type:
         Property that indicates which type of data the Reference will hold.
 
     :ivar container_type:
         The name of the class that holds the ref_type, this property must be used when the ref_type references model from the plugin.
@@ -521,15 +521,15 @@
 
     .. rubric:: **Accessing MultipleReference Field from Plugin**:
 
     In order to access this field from inside the plugin implementation, in C/C++,  you need to use :cpp:func:`get_plugin_input_data_multiplereference_selected_size`
 
     .. rubric:: **Accessing MultipleReference Field from Context**:
 
-    When accessed from the :func:`~alfasim_sdk.context.Context`, the MultipleReference field will return a list with
+    When accessed from the :class:`~alfasim_sdk._internal.context.Context`, the MultipleReference field will return a list with
     the currently selected option objects instances.
 
     With the instance, you can access all attributes from the object. Check the example below.
 
     .. code-block:: bash
 
         @data_model(caption="My Model")
@@ -561,28 +561,28 @@
 
 
 @attr.s(kw_only=True, frozen=True)
 class Quantity(BaseField):
     """
     The Quantity field provides a way to the user provide a scalar value into the application.
 
-    The Quantity field have all options available from :func:`~alfasim_sdk.types.BaseField`, besides the listed the ones listed above:
-    :param values:  A number value.
-    :param unit:    Unit for the given scalar.
+    The Quantity field have all options available from :class:`~BaseField`, besides the listed the ones listed above:
+    :ivar values:  A number value.
+    :ivar unit:    Unit for the given scalar.
 
     All scalar values are created using the `Barril library`_
 
     Checkout the Barril documentation, `to see all available units <https://barril.readthedocs.io/en/latest/units.html>`_
 
     .. note::
 
         If you want to check the input value, is recommended to include a status monitor in your plugin
         to make sure that the provided value is valid.
 
-        For more details about status monitor check :func:`~alfasim_sdk.hooks_specs_gui.alfasim_get_status`
+        For more details about status monitor check :func:`~alfasim_sdk._internal.hook_specs_gui.alfasim_get_status`
 
     .. rubric:: Example myplugin.py
 
     .. code-block:: python
 
         @data_model(icon="", caption="My Plugin")
         class MyModel:
@@ -595,15 +595,15 @@
 
     .. rubric:: **Accessing Quantity Field from Plugin**:
 
     In order to access this field from inside the plugin implementation, in C/C++,  you need to use :cpp:func:`get_plugin_input_data_quantity`
 
     .. rubric:: **Accessing Quantity Field from Context**:
 
-    When accessed from the :func:`~alfasim_sdk.context.Context`, the Quantity field will return a ``Scalar`` object, with
+    When accessed from the :class:`~alfasim_sdk._internal.context.Context`, the Quantity field will return a :class:`barril.units.Scalar` object, with
     the current value and unit.
     Check out the `Scalar documentation from Barril`_ for more details about the usage.
 
     .. code-block:: bash
 
         @data_model(icon="", caption="My Plugin")
         class MyModel:
@@ -633,23 +633,23 @@
     value: numbers.Real = attrib(validator=instance_of(numbers.Real))
     unit: str = attrib(validator=[non_empty_str, valid_unit])
 
 
 @attr.s(kw_only=True, frozen=True)
 class TableColumn(BaseField):
     """
-    The TableColumn component provides columns for a :func:`~alfasim_sdk.type.Table` field.
-    Currently only columns with a :func:`~alfasim_sdk.type.Quantity` fields are available.
+    The TableColumn component provides columns for a :class:`Table` field.
+    Currently only columns with a :class:`Quantity` fields are available.
 
-    Check out the documentation from :func:`~alfasim_sdk.type.Table` to see more details about the usage and how to retrieve values.
+    Check out the documentation from :class:`Table` to see more details about the usage and how to retrieve values.
     """
 
     id: str = attrib(validator=non_empty_str)
     value: Quantity = attrib()
-    caption = attrib(init=False, default="")
+    caption: str = attrib(init=False, default="")
 
     def __attrs_post_init__(self) -> None:
         object.__setattr__(self, "caption", self.value.caption)
 
     @value.validator
     def check(  # pylint: disable=arguments-differ
         self, attr: Attribute, values: Quantity
@@ -707,15 +707,15 @@
 
     .. rubric:: **Accessing Table Field from Plugin**:
 
     In order to access this field from inside the plugin implementation, in C/C++,  you need to use :cpp:func:`get_plugin_input_data_table_quantity`
 
     .. rubric:: **Accessing Table Field from Context**:
 
-    When accessed from the :func:`~alfasim_sdk.context.Context`, the Table field will return a model, with information about
+    When accessed from the :class:`~alfasim_sdk._internal.context.Context`, the Table field will return a model, with information about
     all columns.
 
 
     .. code-block:: bash
         :linenos:
 
         @data_model(icon="", caption="My Model")
@@ -764,16 +764,16 @@
 
 
 @attr.s(kw_only=True)
 class Boolean(BaseField):
     """
     The Boolean field provides a checkbox to select/deselect a property.
 
-    The Boolean fields have all options available from :func:`~alfasim_sdk.types.BaseField`, besides the listed the ones listed above:
-    :param value:  A boolean informing the initial state from the Field
+    The Boolean fields have all options available from :class:`~BaseField`, besides the listed the ones listed above:
+    :ivar value:  A boolean informing the initial state from the Field
 
     .. rubric:: Example myplugin.py
 
     .. code-block:: python
 
         @data_model(icon="", caption="My Plugin")
         class MyModel:
@@ -786,15 +786,15 @@
 
     .. rubric:: **Accessing Boolean Field from Plugin**:
 
     In order to access this field from inside the plugin implementation, in C/C++,  you need to use :cpp:func:`get_plugin_input_data_boolean`
 
     .. rubric:: **Accessing Quantity Field from Context**:
 
-    When accessed from the :func:`~alfasim_sdk.context.Context`, the Boolean field will return a boolean value
+    When accessed from the :class:`~alfasim_sdk._internal.context.Context`, the Boolean field will return a boolean value
 
     .. code-block:: bash
 
         @data_model(icon="", caption="My Plugin")
         class MyModel:
             quantity_field = Boolean(
                 value=False,
@@ -816,17 +816,17 @@
     The name of the selected file will be available over the GUI.
 
     .. note::
 
         If you want to make the file mandatory it is recommended to include a status monitor in your plugin
         to make sure that a file is selected.
 
-        For more details about status monitor check :func:`~alfasim_sdk.hooks_specs_gui.alfasim_get_status`
+        For more details about status monitor check :func:`~alfasim_sdk._internal.hook_specs_gui.alfasim_get_status`
 
-    :param caption: Label to be displayed on the right side of the component.
+    :ivar caption: Label to be displayed on the right side of the component.
 
     .. rubric:: Example myplugin.py
 
     .. code-block:: python
 
         @data_model(icon="", caption="My Plugin")
         class MyModel:
@@ -837,131 +837,136 @@
     .. rubric:: **Accessing FileContent Field from Plugin**:
 
     In order to access this field from inside the plugin implementation, in C/C++,  you need to use :cpp:func:`get_plugin_input_data_file_content`
     together with :cpp:func:`get_plugin_input_data_file_content_size`
 
     .. rubric:: **Accessing Quantity Field from Context**:
 
-    When accessed from the :func:`~alfasim_sdk.context.Context`, the FileContent field will return a FileContent object,
+    When accessed from the :class:`~alfasim_sdk._internal.context.Context`, the FileContent field will return a FileContent object,
     a Model that represent a file from the filesystem.
 
     Class FileContent
 
-    :path:          Return a `Path object`_ of the file.
-    :content:       The content from the file in binary format.
-    :size:          The size of the file in bytes.
-    :modified_data: Return a `Datetime object`_, with the last time the file was modified
+    :ivar path:          Return a `Path object`_ of the file.
+    :ivar content:       The content from the file in binary format.
+    :ivar size:          The size of the file in bytes.
+    :ivar modified_date: Return a `Datetime object`_, with the last time the file was modified
 
     >>> ctx.get_model("MyModel").file_content_field.path
     WindowsPath('C:/ol-wax-1.wax')
 
     >>> ctx.get_model("MyModel").file_content_field.content
     b"!Name of Table  [...] "
 
     >>> ctx.get_model("MyModel").file_content_field.size
     90379
 
-    >>> ctx.get_model("MyModel").file_content_field.modified_data
+    >>> ctx.get_model("MyModel").file_content_field.modified_date
     datetime.datetime(2019, 5, 10, 14, 22, 11, 50795)
 
     .. _Path object: https://docs.python.org/3/library/pathlib.html#pure-paths
     .. _Datetime object: https://docs.python.org/3/library/datetime.html#datetime-objects
     """
 
 
 @attr.s(kw_only=True, frozen=True)
 class AddField:
     """
     Allows the plugin to add new fields to Hydrodynamic model.
 
-    An added field **must** be associated to a phase (Using :class:`~alfasim_sdk.AddPhase` or :class:`~alfasim_sdk.UpdatePhase`)
-    and added to a layer (Using :class:`~alfasim_sdk.AddLayer` or :class:`~alfasim_sdk.UpdateLayer`)
+    An added field **must** be associated to a phase (Using :class:`AddPhase` or :class:`UpdatePhase`)
+    and added to a layer (Using :class:`AddLayer` or :class:`UpdateLayer`)
 
-    :param name: Name of the new field.
+    :ivar name: Name of the new field.
 
     .. note::
         This type is supposed to be used in the :py:func:`~alfasim_sdk._internal.hook_specs_gui.alfasim_configure_fields` `hook`.
 
     """
 
     name: str = attr.ib()
 
 
 @attr.s(kw_only=True, frozen=True)
 class AddLayer:
     """
     Allows the plugin to add new layers to Hydrodynamic model.
 
-    :param name: Name of the new layer.
-    :param fields: List of fields names contained in the added layer.
-    :param continuous_field: Name of the continuous field of the added layer (must be in the `fields` list).
+    :ivar name: Name of the new layer.
+
+    :ivar fields: List of fields names contained in the added layer.
+
+    :ivar continuous_field: Name of the continuous field of the added layer (must be in the `fields` list).
 
     .. note::
-        This type is supposed to be used in the :py:func:`~alfasim_sdk._internal.hook_specs_gui.alfasim_configure_layers` `hook`.
+        This type is supposed to be used in the :func:`~alfasim_sdk._internal.hook_specs_gui.alfasim_configure_layers` `hook`.
     """
 
     name: str = attr.ib()
-    fields: list = attr.ib()
+    fields: List[str] = attr.ib()
     continuous_field: str = attr.ib()
 
 
 @attr.s(kw_only=True, frozen=True)
 class UpdateLayer:
     """
     Allows the plugin to update existing layer of the Hydrodynamic model.
 
     List of possible layers names (see :ref:`api-constants-section` for details):
      - ``GAS_LAYER``
      - ``OIL_LAYER``
      - ``WATER_LAYER`` (If a three phase hydrodynamic model is used)
 
-    :param name: Name of the updated layer.
-    :param additional_fields: List of additional fields names to be appended in the fields list of the layer.
+    :ivar name: Name of the updated layer.
 
+    :ivar additional_fields: List of additional fields names to be appended in the fields list of the layer.
 
     .. note::
-        This type is supposed to be used in the :py:func:`~alfasim_sdk._internal.hook_specs_gui.alfasim_configure_layers` `hook`.
+        This type is supposed to be used in the :func:`~alfasim_sdk._internal.hook_specs_gui.alfasim_configure_layers` `hook`.
     """
 
     name: str = attr.ib()
-    additional_fields: list = attr.ib()
+    additional_fields: List[str] = attr.ib()
 
 
 @attr.s(kw_only=True, frozen=True)
 class AddPhase:
     """
     Allows the plugin to add new phases to Hydrodynamic model.
 
-    :param name: Name of the new phase.
-    :param fields: List of fields names associated to the added phase. It is important to know how to calculate the state variables of fields.
-    :param primary_field: Reference field when a phase property calculation is performed through the fields of the phase.
-    :param is_solid: A boolean variable to identify if the added phase is solid.
+    :ivar name: Name of the new phase.
+    :ivar fields: List of fields names associated to the added phase. It is important to know how to calculate
+        the state variables of fields.
+
+    :ivar primary_field: Reference field when a phase property calculation is performed through the fields of the phase.
+
+    :ivar is_solid: A boolean variable to identify if the added phase is solid.
 
     .. note::
-        This type is supposed to be used in the :py:func:`~alfasim_sdk._internal.hook_specs_gui.alfasim_configure_phases` `hook`.
+        This type is supposed to be used in the :func:`~alfasim_sdk._internal.hook_specs_gui.alfasim_configure_phases` `hook`.
     """
 
     name: str = attr.ib()
-    fields: list = attr.ib()
+    fields: List[str] = attr.ib()
     primary_field: str = attr.ib()
     is_solid: bool = attr.ib(default=False)
 
 
 @attr.s(kw_only=True, frozen=True)
 class UpdatePhase:
     """
     Allows the plugin update existing phases of the Hydrodynamic model.
 
     List of possible phase names (see :ref:`api-constants-section` for details):
      - ``GAS_PHASE``
      - ``OIL_PHASE``
      - ``WATER_PHASE`` (If a three phase hydrodynamic model is used)
 
-    :param name: Name of the new phase.
-    :param additional_fields: List of additional fields names to be appended in the fields list of the phase.
+    :ivar name: Name of the new phase.
+    :ivar additional_fields: List of additional fields names to be appended in the fields list of the phase.
 
     .. note::
-        This type is supposed to be used in the :py:func:`~alfasim_sdk._internal.hook_specs_gui.alfasim_configure_phases` `hook`.
+        This type is supposed to be used in the :func:`~alfasim_sdk._internal.hook_specs_gui.alfasim_configure_phases` `hook`.
     """
 
     name: str = attr.ib()
-    additional_fields: list = attr.ib()
+    additional_fields: List[str] = attr.ib()
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfasim_sdk_utils.py` & `alfasim_sdk-2024.1/src/alfasim_sdk/_internal/alfasim_sdk_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Any
+from typing import Dict
 from typing import Optional
 from typing import Tuple
 
 import attr
 
 from alfasim_sdk._internal.types import BaseField
 from alfasim_sdk._internal.types import Group
@@ -27,15 +29,22 @@
         "model": model,
         "bases": bases,
     }
 
     return attr_class
 
 
-def is_a_valid_field(value) -> bool:
+def get_metadata(obj: Any) -> Dict[str, Any]:
+    """
+    Return the metadata associated with a class created by the SDK.
+    """
+    return obj._alfasim_metadata
+
+
+def is_a_valid_field(value: type) -> bool:
     """
     A utility method to indicate if the given value is BaseField or a Tab layout
     """
     valid_field = False
 
     if isinstance(value, BaseField):
         valid_field = True
@@ -45,15 +54,15 @@
 
     if isinstance(value, type) and issubclass(value, Group):
         valid_field = True
 
     return valid_field
 
 
-def get_all_attributes(class_: type):
+def get_all_attributes(class_: type) -> Dict[str, Any]:
     """
     Return a dictionary with all attributes from the given class_ converted to an attr.Attribute, ignoring all "dunders"
     method and raising a TypeError to avoid attributes with a "_" at the beginning of the name
     """
     attributes = {}
     for key, value in vars(class_).items():
         if key.startswith("__"):
@@ -70,29 +79,25 @@
             )
 
         attributes[key] = attr.ib(default=value)
 
     return attributes
 
 
-def get_current_version():
+def get_current_version() -> str:
     """
     Checks current version of alfasim-sdk. Extracted to be easier to mock in tests.
-    :return:
     """
     import alfasim_sdk
 
     return alfasim_sdk.__version__
 
 
-def get_extras_default_required_version():
+def get_extras_default_required_version() -> str:
     """
-    :rtype str:
     :return:
         Returns a string with default alfasim-sdk version requirement for plugins. Default is
         greater or equal current version and lesser than next major release.
     """
     parts = get_current_version().split(".")
-    current_major = parts[0]
     current_minor = ".".join(parts[:2])
-    next_major = int(current_major) + 1
-    return f">={current_minor}, <{next_major}"
+    return f">={current_minor}"
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/units.py` & `alfasim_sdk-2024.1/src/alfasim_sdk/_internal/units.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from functools import lru_cache
 
 
-@lru_cache()
-def register_units():
+@lru_cache
+def register_units() -> None:
     """
     Register new categories for Barril and limit the number of units shown to users.
 
     Note: we try to add all combinations of units we find useful, but given that POSC doesn't have all
     possible combinations we remove the ones which don't work manually.
     """
 
@@ -112,14 +112,15 @@
     velocity_units.remove("km/d")
     velocity_units.remove("km/min")
     velocity_units.remove("mm/d")
     velocity_units.remove("mm/h")
     velocity_units.remove("mm/min")
     velocity_units.remove("in/d")
     velocity_units.remove("in/h")
+    velocity_units.append("mm/a")
     db.AddCategory(
         "velocity", quantity_type="velocity", valid_units=velocity_units, override=True
     )
 
     # we don't construct volume_per_volume_units using 'volume_units' because the number of units available by
     # the dimensionless quantity type is really small
     volume_per_volume_units = ["m3/m3", "L/m3", "ft3/ft3", "volppm"]
@@ -146,8 +147,23 @@
     # Creating separate categories for some Gas properties, so they are plotted in a separate axis
     std_volume_per_time_units = db.GetValidUnits("standard volume per time")
     db.AddCategory(
         "gas standard volume per time",
         quantity_type="standard volume per time",
         valid_units=std_volume_per_time_units,
     )
-    # "gas volume flow rate" is also required, but it is already registered
+
+    std_volume_units = db.GetValidUnits("standard volume")
+    db.AddCategory(
+        "gas standard volume",
+        quantity_type="standard volume",
+        valid_units=std_volume_units,
+    )
+    # NOTE: "gas volume flow rate" and "gas volume" are also required, but they are already registered
+
+    angle_per_time_units = ["Hz", "rpm", "rad/s"]
+    db.AddCategory(
+        "angle per time",
+        quantity_type="frequency",
+        valid_units=angle_per_time_units,
+        override=True,
+    )
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/context.py` & `alfasim_sdk-2024.1/src/alfasim_sdk/_internal/context.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,80 +4,81 @@
 import attr
 from attr.validators import deep_iterable
 from attr.validators import in_
 from attr.validators import instance_of
 from attr.validators import optional
 from barril.units import Scalar
 
-from alfasim_sdk._internal.constants import EmulsionModelType
+from alfasim_sdk._internal.constants import EmulsionDropletSizeModelType
+from alfasim_sdk._internal.constants import EmulsionInversionPointModelType
+from alfasim_sdk._internal.constants import EmulsionRelativeViscosityModelType
 from alfasim_sdk._internal.constants import HydrodynamicModelType
 from alfasim_sdk._internal.constants import SolidsModelType
 from alfasim_sdk._internal.validators import list_of_strings
 from alfasim_sdk._internal.validators import non_empty_str
 
 
 @attr.s(frozen=True)
 class PluginInfo:
     """
     PluginInfo provides information about the plugin name, its current state (either enabled or not) and all
     models defined from this plugin.
     """
 
-    caption = attr.attrib(validator=non_empty_str)
-    name = attr.attrib(validator=non_empty_str)
-    enabled = attr.attrib(validator=instance_of(bool))
-    models = attr.attrib(validator=list_of_strings)
+    caption: str = attr.attrib(validator=non_empty_str)
+    name: str = attr.attrib(validator=non_empty_str)
+    enabled: bool = attr.attrib(validator=instance_of(bool))
+    models: List[str] = attr.attrib(validator=list_of_strings)
 
 
 @attr.s(frozen=True)
 class PipelineSegmentInfo:
     """
     The PipelineSegmentInfo provides information about segments associated with a pipeline.
 
     PipelineSegmentInfo provides the following attributes:
-        edge_name: name of the edge that the segment is associated with
 
-        start_position: Defines point where this segment starts in MD (measured depth).
+    :ivar start_position: Defines point where this segment starts in MD (measured depth).
 
-        inner_diameter: Inner diameter of pipe annulus.
+    :ivar inner_diameter: Inner diameter of pipe annulus.
 
-        roughness: Absolute roughness of the wall of this segment.
-            When ```is_custom``` is true, the reported roughness is customized for this segment,
-            otherwise, the reported roughness is the original reported by the wall.
+    :ivar roughness: Absolute roughness of the wall of this segment.
+        When ```is_custom``` is true, the reported roughness is customized for this segment,
+        otherwise, the reported roughness is the original reported by the wall.
+
+    :ivar is_custom: Informs either the roughness value is custom or original from the wall
 
-        is_custom: Informs either the roughness value is custom or original from the wall
     """
 
-    inner_diameter = attr.attrib(validator=instance_of(Scalar))
-    start_position = attr.attrib(validator=instance_of(Scalar))
-    is_custom = attr.attrib(validator=instance_of(bool))
-    roughness = attr.attrib(validator=instance_of(Scalar))
+    inner_diameter: Scalar = attr.attrib(validator=instance_of(Scalar))
+    start_position: Scalar = attr.attrib(validator=instance_of(Scalar))
+    is_custom: bool = attr.attrib(validator=instance_of(bool))
+    roughness: Scalar = attr.attrib(validator=instance_of(Scalar))
 
 
 list_of_segments = deep_iterable(
     member_validator=instance_of(PipelineSegmentInfo),
     iterable_validator=instance_of(list),
 )
 
 
 @attr.s(frozen=True)
 class PipelineInfo:
     """
     The PipelineInfo provides information about the geometry of a pipeline.
 
     PipelineSegmentInfo provides the following attributes:
-        name: Name associated with this ``Pipeline`` on ALFAsim
-
-        edge_name: Name of the edge that this ``Pipeline`` is associated with.
+    :ivar name: Name associated with this ``Pipeline`` on ALFAsim
 
-        segments: List of segments associates with this ``Pipeline``
-        For more information check `alfasim_sdk.context.PipelineSegmentInfo`
+    :ivar edge_name: Name of the edge that this ``Pipeline`` is associated with.
 
-        total_length: Total length of the pipeline.
+    :ivar segments: List of segments associates with this ``Pipeline``
+        For more information check :class:`~PipelineSegmentInfo`
 
+    :ivar total_length: Total length of the pipeline.
     """
 
     name = attr.attrib(type=str, validator=non_empty_str)
     edge_name = attr.attrib(type=str, validator=non_empty_str)
     segments = attr.attrib(type=List[PipelineSegmentInfo], validator=list_of_segments)
     total_length = attr.attrib(type=Scalar, validator=instance_of(Scalar))
 
@@ -85,89 +86,112 @@
 @attr.s(frozen=True)
 class NodeInfo:
     """
     The ``NodeInfo`` provides information about a ``Node`` from ``ALFAsim``, it provides the name of the Node and the number of
     phases that the associate PVT model has.
     """
 
-    name = attr.attrib(validator=non_empty_str)
-    number_of_phases_from_associated_pvt = attr.attrib(
+    name: str = attr.attrib(validator=non_empty_str)
+    number_of_phases_from_associated_pvt: Optional[int] = attr.attrib(
         validator=optional(instance_of(int))
     )
 
 
 @attr.s(frozen=True)
 class EdgeInfo:
     """
     The ``EdgeInfo`` provides information about a ``Edge`` from ``ALFAsim``, it provides the name of the Node and the number of
     phases that the associate pvt model has.
     """
 
-    name = attr.attrib(validator=non_empty_str)
-    number_of_phases_from_associated_pvt = attr.attrib(
+    name: str = attr.attrib(validator=non_empty_str)
+    number_of_phases_from_associated_pvt: Optional[int] = attr.attrib(
         validator=optional(instance_of(int))
     )
 
 
 @attr.s(frozen=True)
 class HydrodynamicModelInfo:
     """
     HydrodynamicModelInfo provides information about which layer, fields, and phases the currently Hydrodynamic model is using.
     """
 
-    selected_base_type = attr.attrib(validator=in_(HydrodynamicModelType))
-    phases = attr.attrib(validator=list_of_strings)
-    fields = attr.attrib(validator=list_of_strings)
-    layers = attr.attrib(validator=list_of_strings)
+    selected_base_type: HydrodynamicModelType = attr.attrib(
+        validator=in_(HydrodynamicModelType)
+    )
+    phases: List[str] = attr.attrib(validator=list_of_strings)
+    fields: List[str] = attr.attrib(validator=list_of_strings)
+    layers: List[str] = attr.attrib(validator=list_of_strings)
     has_water_phase = attr.attrib(type=bool, validator=instance_of(bool))
 
 
 @attr.s(frozen=True)
+class EmulsionModelInfo:
+    """
+    EmulsionModelInfo provides information about whether the emulsion model is enabled and the models used for relative
+    viscosity, droplet size, and inversion point.
+    """
+
+    enabled = attr.attrib(type=bool, validator=instance_of(bool))
+    relative_viscosity_model: EmulsionRelativeViscosityModelType = attr.attrib(
+        validator=in_(EmulsionRelativeViscosityModelType)
+    )
+    droplet_size_model: EmulsionDropletSizeModelType = attr.attrib(
+        validator=in_(EmulsionDropletSizeModelType)
+    )
+    inversion_point_model: EmulsionInversionPointModelType = attr.attrib(
+        validator=in_(EmulsionInversionPointModelType)
+    )
+
+
+@attr.s(frozen=True)
 class PhysicsOptionsInfo:
     """
-    PhysicsOptionsInfo provides information about the ``Physics Options`` available at ``ALFAsim``.
+    ``PhysicsOptionsInfo`` provides information about the physics options available at ``ALFAsim``.
 
     The following option can be accessed:
 
-    Emulsion Model: Informs which emulsion model the application is currently using.
-    For more information about all options available check ``alfasim_sdk.context.EmulsionModelType``
+    Emulsion Model: Informs the relative viscosity, droplet size, and inversion point emulsion models
 
     Solids Model: Informs the current solid model being used by the application
-    For more information about all options available check ``alfasim_sdk.context.SolidsModelType``
+    For more information about all options available check :py:class:`~alfasim_sdk._internal.constants.SolidsModelType`
 
-    Hydrodynamic Model: Provides a ``alfasim_sdk.context.HydrodynamicModelInfo`` informing which layers, fields and phases
+    Hydrodynamic Model: Provides a :class:`HydrodynamicModelInfo` informing which layers, fields and phases
     the application is currently using.
-    For more information about all options available check ``alfasim_sdk.context.HydrodynamicModelInfo``
     """
 
-    emulsion_model = attr.attrib(validator=in_(EmulsionModelType))
-    solids_model = attr.attrib(validator=in_(SolidsModelType))
-    hydrodynamic_model = attr.attrib(validator=instance_of(HydrodynamicModelInfo))
+    emulsion_model: EmulsionModelInfo = attr.attrib(
+        validator=instance_of(EmulsionModelInfo)
+    )
+    solids_model: SolidsModelType = attr.attrib(validator=in_(SolidsModelType))
+    hydrodynamic_model: HydrodynamicModelInfo = attr.attrib(
+        validator=instance_of(HydrodynamicModelInfo)
+    )
 
 
 class Context:
     """
     The context class provides information about the current state of the application
     and the models implemented by the user.
 
-    The following methods provide an instance of :func:`~alfasim_sdk.context.Context` to inform the current state
+    The following methods provide an instance of ``Context`` to inform the current state
     of the application:
 
     - :ref:`visible-expression-section` parameter from all fields
     - :ref:`enable-expression-section` parameter from all fields
-    - :func:`~alfasim_sdk.hook_specs_gui.alfasim_get_status` hook
+    - :func:`~alfasim_sdk._internal.hook_specs_gui.alfasim_get_status` hook
     """
 
     def get_model(self, model_name: str) -> Optional[type]:
         """
         Returns an instance of the given ``model_name``.
 
-        The parameter ``model_name`` must be the name of a model defined within the plugin.
+        :param model_name: must be the name of a model defined within the plugin.
 
-        In the example below, the Context is used to access a property from the model ``MyModel``
+        In the example below, the ``Context`` is used to access a property from the model ``MyModel``
 
         ``ctx.GetModel("Acme")`` as exemplified in the code below.
 
         .. rubric:: Setting up the model
 
         .. code-block:: python
 
@@ -187,26 +211,26 @@
 
             >>> ctx.get_model('MyModel')
             MyModel(name='ALFAsim', scalar=Scalar(1.0, 'degC', 'temperature'))
 
             >>> ctx.get_model('MyModel').name
             'ALFAsim'
 
-        At runtime, you can also verify the names of the models defined by a given plugin. For this, you need to
-        For more information check :func:`~alfasim_sdk.context.Context.GetPluginInfoById`
+        At runtime, you can also verify the names of the models defined by a given plugin.
+        For more information check cpp:func:`~alfasim_sdk.context.Context.GetPluginInfoById`
 
         :raises TypeError: When the given ``model_name`` does not exist.
         :raises FrozenInstanceError: When trying to modify a value
 
         """
 
     def get_pipelines(self) -> Optional[List[PipelineInfo]]:
         """
         Return a list with all Pipes available on the Network from the Project.
-        Each Pipe is represented by an instance of :func:`~alfasim_sdk.context.PipelineInfo`.
+        Each Pipe is represented by an instance of :class:`~alfasim_sdk._internal.context.PipelineInfo`.
 
         .. rubric:: Usage Example of GetPipelines
 
         .. image:: /_static/images/api/context_access_network.png
 
         The image above has two Pipelines configured, you can access this information by using the method ``GetPipelines`` as
         demonstrated below.
@@ -226,25 +250,25 @@
             1
 
 
         .. note::
 
             The values from PipelineInfo are read-only, they cannot be modified.
 
-        Checkout the :func:`~alfasim_sdk.context.PipelineInfo` section to know more about the properties available.
+        Checkout the :class:`~alfasim_sdk._internal.context.PipelineInfo` section to know more about the properties available.
         """
 
     def get_plugins_infos(self) -> List[PluginInfo]:
         """
         Return a list of all plugins available on ALFAsim.
-        Each plugin is represented by an instance of :func:`~alfasim_sdk.context.PluginInfo`.
+        Each plugin is represented by an instance of :class:`PluginInfo`.
 
         .. rubric:: Usage Example of GetPluginsInfos
 
-        The example demonstrated how you can access information about the plugin from using the :func:`~alfasim_sdk.context.GetPluginsInfos`
+        The example demonstrated how you can access information about the plugin from using the cpp:func:`~alfasim_sdk.context.Context.GetPluginsInfos`
         method.
 
         .. rubric:: Setting up the model
 
         .. code-block:: python
 
             @data_model(caption="MyPlugin", icon="")
@@ -267,77 +291,77 @@
             >>> ctx.get_plugins_infos()[0].enabled
             True
 
             >>> ctx.get_plugins_infos()[0].models
             ['MyModel']
 
 
-        Checkout the :func:`~alfasim_sdk.context.PluginInfo` section to know more about the properties available.
+        Checkout the :class:`PluginInfo` section to know more about the properties available.
         """
 
     def get_plugin_info_by_id(self, plugin_id: str) -> PluginInfo:
         """
-        Similar to :func:`~alfasim_sdk.context.GetPluginsInfos` but returns a single instance of :func:`~alfasim_sdk.context.PluginInfo`
+        Similar to :func:`get_plugins_infos` but returns a single instance of :class:`PluginInfo`
         from the given ``plugin_id`` parameter.
 
-        Checkout the :func:`~alfasim_sdk.context.PluginInfo` section to know more about the properties available.
+        Checkout the :class:`PluginInfo` section to know more about the properties available.
 
         :raises ValueError: When the plugin informed by ``plugin_id`` it's not available.
         """
 
     def get_edges(self) -> Optional[List[EdgeInfo]]:
         """
         Return a list of all Edges available on ALFAsim.
-        Each Edge is represented by an instance of :func:`~alfasim_sdk.context.EdgeInfo`.
+        Each Edge is represented by an instance of :class:`EdgeInfo`.
 
         .. rubric:: Example of GetEdges
 
         .. image:: /_static/images/api/context_access_network.png
 
-        The image above has two Edges configured, in order to access the available Edges, it's possible to use the method ``GetEdges`` as
+        The image above has two Edges configured, in order to access the available Edges, it's possible to use the method ``get_edges`` as
         demonstrated below.
 
         .. rubric:: Accessing GetEdges from the context
 
         .. code-block:: console
 
             >>> ctx.get_edges()[0]
             EdgeInfo(name='Pipe 1', number_of_phases_from_associated_pvt=2)
 
             >>> ctx.get_pipelines()[0].number_of_phases_from_associated_pvt
             'Pipe 1'
 
-        Checkout the :func:`~alfasim_sdk.context.EdgeInfo` section to know more about the properties available.
+        Checkout the :class:`EdgeInfo` section to know more about the properties available.
         """
 
     def get_nodes(self) -> Optional[List[NodeInfo]]:
         """
         Return a list of all Nodes available on ALFAsim.
-        Each Node is represented by an instance of :func:`alfasim_sdk.context.NodeInfo`.
+        Each Node is represented by an instance of :class:`NodeInfo`.
 
         .. rubric:: Usage Example of GetNodes
 
         .. image:: /_static/images/api/context_access_network.png
 
-        The image above has three nodes configured, you can access this information by using the method ``GetNodes`` as
+        The image above has three nodes configured, you can access this information by using the method ``get_nodes`` as
         demonstrated below.
 
         .. code-block:: console
 
             >>> ctx.get_nodes[0]
             NodeInfo(name='Node 1', number_of_phases_from_associated_pvt=2)
 
             >>> ctx.get_nodes[0].name
             'Node 1'
 
         .. note::
 
             The values from NodeInfo are read-only, they cannot be modified.
 
-        Checkout the :func:`~alfasim_sdk.context.NodeInfo` section to know more about the properties available.
+        Checkout the :class:`NodeInfo` section to know more about the properties available.
         """
 
     def get_physics_options(self) -> PhysicsOptionsInfo:
         """
         Return the physics options from the current project from ALFAsim.
 
         .. rubric:: Example of GetPhysicsOptions
@@ -356,24 +380,24 @@
 
         .. code-block:: python
 
             >>> ctx.get_physics_options()
             PhysicsOptionsInfo( [...] )
 
             >>> ctx.get_physics_options().emulsion_model.value
-            'EmulsionModelType.brinkman1952'
+            EmulsionModelInfo( [ ... ] )
 
             >>> ctx.get_physics_options().hydrodynamic_model
             HydrodynamicModelInfo( [ ... ] )
 
             >>> ctx.get_physics_options().hydrodynamic_model.fields
             ['gas', 'oil', 'droplet', 'bubble']
 
             >>> ctx.get_physics_options().hydrodynamic_model.layers
             ['gas', 'oil']
 
             >>> ctx.get_physics_options().hydrodynamic_model.phases
             ['gas', 'oil']
 
-        Checkout the :func:`~alfasim_sdk.context.PhysicsOptionsInfo` section to know more about the properties available.
+        Checkout the :class:`PhysicsOptionsInfo` section to know more about the properties available.
 
         """
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/hook_specs_gui.py` & `alfasim_sdk-2024.1/src/alfasim_sdk/_internal/hook_specs_gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,10 @@
-from typing import List
-from typing import Union
-
 from pluggy import HookspecMarker
 
-from alfasim_sdk import ErrorMessage
-from alfasim_sdk import WarningMessage
 from alfasim_sdk._internal.context import Context
-from alfasim_sdk._internal.variables import SecondaryVariable
-
 
 hookspec = HookspecMarker("ALFAsim")
 
 
 @hookspec
 def alfasim_get_data_model_type():
     """
@@ -19,16 +12,16 @@
 
     - Customize items on ALFAsim application, by adding new components over the Tree.
     - Hold input data information to be accessed from the solver.
     - Validate input data or configuration made on ALFAsim, to ensure that the plugin has all configuration necessary to be run successfully.
 
     This hook needs to return a class decorated with one of the following options:
 
-    - :func:`alfasim_sdk.models.container_model`
-    - :func:`alfasim_sdk.models.data_model`
+    - :func:`~alfasim_sdk.container_model`
+    - :func:`~alfasim_sdk.data_model`
 
     The image below shows the locations where a custom model can be inserted implementing the hook.
 
     .. image:: /_static/images/hooks/tree_plugin_marker.png
         :scale: 80%
 
     .. image:: /_static/images/hooks/model_explorer_with_marker.png
@@ -36,15 +29,15 @@
 
     .. |m_1| image:: /_static/images/marker_1.png
         :scale: 80%
 
     .. |m_2| image:: /_static/images/marker_2.png
         :scale: 80%
 
-    |m_1| Location to where the models :func:`~alfasim_sdk.models.container_model` or :func:`~alfasim_sdk.models.data_model` will be placed. |br|
+    |m_1| Location to where the models :func:`~alfasim_sdk.container_model` or :func:`~alfasim_sdk.data_model` will be placed. |br|
     |m_2| Location to where the :ref:`inputs fields <api-types-section>` will be placed.
 
     Example 1: The following example shows how to create a new model.
 
     .. code-block:: python
 
         import alfasim_sdk
@@ -63,16 +56,16 @@
 
     .. image:: /_static/images/hooks/alfasim_get_data_model_type_example_1.png
         :scale: 80%
 
 
     Example 2: This second example shows how to create a new container model.
 
-    Notice that when using the :func:`~alfasim_sdk.models.container_model` you only need to inform the container class
-    to the :func:`~alfasim_sdk.hook_specs_gui.alfasim_get_data_model_type` hook
+    Notice that when using the :func:`~alfasim_sdk.container_model` you only need to inform the container class
+    to the :func:`~alfasim_get_data_model_type` hook
 
     .. code-block:: python
 
         import alfasim_sdk
         from alfasim_sdk import data_model, container_model
         from alfasim_sdk import Quantity, String
 
@@ -124,23 +117,23 @@
 
     .. image:: /_static/images/hooks/alfasim_get_data_model_type_example_3.png
         :scale: 80%
     """
 
 
 @hookspec
-def alfasim_get_additional_variables() -> List[SecondaryVariable]:
+def alfasim_get_additional_variables():
     """
     Allows plugins to register new additional variables on ALFAsim.
 
     It can be used to store the internal variable from the plugin (on solver), or it can be used to expose as an
     output to the user in the plot window (on application). To calculate and update the registered variables the Solver
     `hooks` described on :ref:`update_secondary_variables` section must be implemented.
 
-    This method expects to return a list of :func:`alfasim_sdk.variables.SecondaryVariable`, for more details checkout
+    This method expects to return a list of :class:`~alfasim_sdk.SecondaryVariable`, for more details checkout
     the reference section with all details about :ref:`variables <api-variables-section>`
 
     Usage example:
 
     .. code-block:: python
 
         from alfasim_sdk import SecondaryVariable
@@ -162,41 +155,41 @@
                 )]
     """
 
 
 @hookspec
 def alfasim_get_status(
     ctx: Context,
-) -> List[Union[WarningMessage, ErrorMessage]]:
+):
     """
     Allows plugins to execute custom checks on ALFAsim.
     These checks can be used to guarantee the consistency of the data or compatibility with some configuration made on |alfasim|.
 
     The status monitor accepts two types of message:
 
-     - :func:`~alfasim_sdk.status.ErrorMessage`:
+    :class:`~alfasim_sdk.ErrorMessage`:
         Signalize the application to block the simulation until the error is fixed.
 
-     - :func:`~alfasim_sdk.status.WarningMessage`:
+    :class:`~alfasim_sdk.WarningMessage`:
         Signalize the application that the user needs to fix this problem, but does not need to block the simulation.
 
     When no errors are detected, an empty list must be returned.
 
-    The ``alfasim_get_status`` will be called for:
+    The :func:`alfasim_get_status` will be called for:
 
      - Each time a model from the plugin is modified.
      - Each time a ``Physics options`` from |alfasim| are modified. |br|
        Ex.: Hydrodynamic model changed
 
     The ``ctx`` parameter is provided to retrieve information about the current state of the application and the current value
     of the models implemented by the user.
 
-    Check out the full documentation of :class:`alfasim_sdk.context.Context` for more details.
+    Check out the full documentation of :class:`~alfasim_sdk._internal.context.Context` for more details.
 
-    The following example shows how to display an ErrorMessage when a :func:`~alfasim_sdk.types.Quantity` field does not have the desired value.
+    The following example shows how to display an ErrorMessage when a :class:`~alfasim_sdk.Quantity` field does not have the desired value.
 
     .. code-block:: python
 
         import alfasim_sdk
         from alfasim_sdk import data_model
         from alfasim_sdk import Quantity
         from alfasim_sdk import ErrorMessage
@@ -241,21 +234,21 @@
 @hookspec
 def alfasim_configure_fields(ctx: Context):
     """
     Allows plugins to configure new fields to be added in |alfasim|'s hydrodynamic model.
 
     An added ``field`` must be associated with:
 
-     - Phase, defined by :class:`~alfasim_sdk.types.AddPhase` or :class:`~alfasim_sdk.types.UpdatePhase`.
-     - Layer, defined by :class:`~alfasim_sdk.types.AddLayer` or :class:`~alfasim_sdk.types.UpdateLayer`.
+     - Phase, defined by :class:`~alfasim_sdk.AddPhase` or :class:`~alfasim_sdk.UpdatePhase`.
+     - Layer, defined by :class:`~alfasim_sdk.AddLayer` or :class:`~alfasim_sdk.UpdateLayer`.
 
-     The ``ctx`` parameter is provided to retrieve information about the current state of the application and the current value
+    The ``ctx`` parameter is provided to retrieve information about the current state of the application and the current value
     of the models implemented by the user.
 
-    Check out the full documentation of :class:`alfasim_sdk.context.Context` for more details.
+    Check out the full documentation of :class:`~alfasim_sdk._internal.context.Context` for more details.
 
     Example of usage:
 
     .. code-block:: python
 
         @alfasim_sdk.hookimpl
         def alfasim_configure_fields(ctx):
@@ -269,21 +262,21 @@
 
 
 @hookspec
 def alfasim_configure_layers(ctx: Context):
     """
     Allows plugins to configure new layers or associate a new field with a existing layer for |alfasim|'s hydrodynamic model
 
-    In order to configure a new layer, it is necessary to return an :class:`~alfasim_sdk.types.AddLayer` object defining the
+    In order to configure a new layer, it is necessary to return an :class:`~alfasim_sdk.AddLayer` object defining the
     required fields.
 
-     The ``ctx`` parameter is provided to retrieve information about the current state of the application and the current value
+    The ``ctx`` parameter is provided to retrieve information about the current state of the application and the current value
     of the models implemented by the user.
 
-    Check out the full documentation of :class:`alfasim_sdk.context.Context` for more details.
+    Check out the full documentation of :class:`~alfasim_sdk._internal.context.Context` for more details.
 
     Example of usage:
 
     .. code-block:: python
 
         @alfasim_sdk.hookimpl
         def alfasim_configure_layers(ctx):
@@ -307,21 +300,21 @@
     """
 
 
 @hookspec
 def alfasim_configure_phases(ctx: Context):
     """
     Allows plugins to configure new phases or associate a new field with a existing phase from the application.
-    In order to configure a new phase it is necessary to return an :class:`~alfasim_sdk.types.AddPhase` object defining the
+    In order to configure a new phase it is necessary to return an :class:`~alfasim_sdk.AddPhase` object defining the
     required fields.
 
-     The ``ctx`` parameter is provided to retrieve information about the current state of the application and the current value
+    The ``ctx`` parameter is provided to retrieve information about the current state of the application and the current value
     of the models implemented by the user.
 
-    Check out the full documentation of :class:`alfasim_sdk.context.Context` for more details.
+    Check out the full documentation of :class:`~alfasim_sdk._internal.context.Context` for more details.
 
     Example of usage:
 
     .. code-block:: python
 
         @alfasim_sdk.hookimpl
         def alfasim_configure_phases(ctx):
@@ -334,31 +327,31 @@
                     ],
                     primary_field='plugin_continuous_field',
                     is_solid=False,
                 )
             ]
 
     With this new phase, all existing hydrodynamic models from the application will have this additional phase.
-    Notice that the ``fields`` parameter must be a field registered from the hook :func:`~alfasim_sdk.hook_specs_gui.alfasim_configure_fields`.
+    Notice that the ``fields`` parameter must be a field registered from the hook :func:`alfasim_configure_fields`.
 
     .. note::
 
             You can restrict the operation of your plugin in the application to certain settings by using the status monitor.
             For example, if your plugin does not work with the water phase you can block the simulation
             if the user is using a hydrodynamic model with water.
 
-            For more details check out the documentation of :func:`~alfasim_sdk.hook_specs_gui.alfasim_get_status`
+            For more details check out the documentation of :func:`alfasim_get_status`
 
 
     The image below shows the new added phase on the application.
 
     .. image:: /_static/images/hooks/alfasim_configure_phase_example_1.png
         :scale: 80%
 
-    It is also possible to add additional fields to existent phases using the :class:`~alfasim_sdk.types.UpdatePhase`.
+    It is also possible to add additional fields to existent phases using the :class:`~alfasim_sdk.UpdatePhase`.
 
     Example of usage:
 
     .. code-block:: python
 
         @alfasim_sdk.hookimpl
         def alfasim_configure_phases(ctx):
@@ -376,18 +369,18 @@
 def alfasim_get_phase_properties_calculated_from_plugin():
     """
     Allows the plugin to calculate the properties (state variables) of a phase.
 
     Must return a list of phase names in which state variables will be computed for. If the plugin implements this `hook`
     four C/C++ Solver `hooks` also must be implemented. They are:
 
-     - :py:func:`HOOK_INITIALIZE_STATE_VARIABLE_CALCULATOR<alfasim_sdk.hook_specs.initialize_state_variables_calculator>`
-     - :py:func:`HOOK_CALCULATE_STATE_VARIABLE<alfasim_sdk.hook_specs.calculate_state_variable>`
-     - :py:func:`HOOK_CALCULATE_PHASE_PAIR_STATE_VARIABLE<alfasim_sdk.hook_specs.calculate_phase_pair_state_variable>`
-     - :py:func:`HOOK_FINALIZE_STATE_VARIABLE_CALCULATOR<alfasim_sdk.hook_specs.finalize_state_variables_calculator>`
+     - :py:func:`HOOK_INITIALIZE_STATE_VARIABLE_CALCULATOR<alfasim_sdk._internal.hook_specs.initialize_state_variables_calculator>`
+     - :py:func:`HOOK_CALCULATE_STATE_VARIABLE<alfasim_sdk._internal.hook_specs.calculate_state_variable>`
+     - :py:func:`HOOK_CALCULATE_PHASE_PAIR_STATE_VARIABLE<alfasim_sdk._internal.hook_specs.calculate_phase_pair_state_variable>`
+     - :py:func:`HOOK_FINALIZE_STATE_VARIABLE_CALCULATOR<alfasim_sdk._internal.hook_specs.finalize_state_variables_calculator>`
 
     The first and last hooks are called immediately before and after the state variables are calculated, respectively.
 
      Example of usage:
 
     .. code-block:: python
 
@@ -402,15 +395,15 @@
 
 @hookspec
 def alfasim_get_phase_interaction_properties_calculated_from_plugin():
     """
     Allows the plugin to calculate the properties that are related to a pair of phases, like `surface tension`.
 
     Must return a list of tuple of phases in which state variables will be computed for. In order to
-    implement the properties, :py:func:`HOOK_CALCULATE_PHASE_PAIR_STATE_VARIABLE<alfasim_sdk.hook_specs.calculate_phase_pair_state_variable>`
+    implement the properties, :py:func:`HOOK_CALCULATE_PHASE_PAIR_STATE_VARIABLE<alfasim_sdk._internal.hook_specs.calculate_phase_pair_state_variable>`
     must be implemented on the C/C++ part of the plugin.
 
     Example of usage:
 
     .. code-block:: python
 
         from alfasim_sdk import GAS_PHASE, OIL_PHASE, WATER_PHASE
@@ -430,19 +423,19 @@
     """
     Allows the plugin to add new tracers in the |alfasim|'s Tracer Solver, in which the transport equation will be
     modified by Solver `hooks` listed below.
 
     Must return a list of tracers in which the internal tracer model `hooks` will be implemented.
     The following C/C++ Solver `hooks` must be implemented:
 
-     - :py:func:`HOOK_INITIALIZE_MASS_FRACTION_OF_TRACER<alfasim_sdk.hook_specs.initialize_mass_fraction_of_tracer>`
-     - :py:func:`HOOK_COMPUTE_MASS_FRACTION_OF_TRACER_IN_PHASE<alfasim_sdk.hook_specs.calculate_mass_fraction_of_tracer_in_phase>`
-     - :py:func:`HOOK_COMPUTE_MASS_FRACTION_OF_TRACER_IN_FIELD<alfasim_sdk.hook_specs.calculate_mass_fraction_of_tracer_in_field>`
-     - :py:func:`HOOK_SET_BOUNDARY_CONDITION_OF_MASS_FRACTION_OF_TRACER<alfasim_sdk.hook_specs.set_prescribed_boundary_condition_of_mass_fraction_of_tracer>`
-     - :py:func:`HOOK_UPDATE_BOUNDARY_CONDITION_OF_MASS_FRACTION_OF_TRACER<alfasim_sdk.hook_specs.update_boundary_condition_of_mass_fraction_of_tracer>`
+     - :py:func:`HOOK_INITIALIZE_MASS_FRACTION_OF_TRACER<alfasim_sdk._internal.hook_specs.initialize_mass_fraction_of_tracer>`
+     - :py:func:`HOOK_COMPUTE_MASS_FRACTION_OF_TRACER_IN_PHASE<alfasim_sdk._internal.hook_specs.calculate_mass_fraction_of_tracer_in_phase>`
+     - :py:func:`HOOK_COMPUTE_MASS_FRACTION_OF_TRACER_IN_FIELD<alfasim_sdk._internal.hook_specs.calculate_mass_fraction_of_tracer_in_field>`
+     - :py:func:`HOOK_SET_BOUNDARY_CONDITION_OF_MASS_FRACTION_OF_TRACER<alfasim_sdk._internal.hook_specs.set_prescribed_boundary_condition_of_mass_fraction_of_tracer>`
+     - :py:func:`HOOK_UPDATE_BOUNDARY_CONDITION_OF_MASS_FRACTION_OF_TRACER<alfasim_sdk._internal.hook_specs.update_boundary_condition_of_mass_fraction_of_tracer>`
 
     Example of usage:
 
     .. code-block:: python
 
         @alfasim_sdk.hookimpl
         def alfasim_get_user_defined_tracers_from_plugin():
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/layout.py` & `alfasim_sdk-2024.1/src/alfasim_sdk/_internal/layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from alfasim_sdk._internal.types import Group
 from alfasim_sdk._internal.types import Tab
 from alfasim_sdk._internal.types import Tabs
 
 
 def tabs() -> Callable:
     """
-    Create a tab bar layout, to group multiples :func:"~alfasim_sdk.layout.tab" instances.
+    Create a tab bar layout, to group multiples :func:"tab" instances.
 
-    With the ``tabs``, you can split up complex dialog into "pages" using a :func:"~alfasim_sdk.layout.tab" instance.
+    With the ``tabs``, you can split up complex dialog into "pages" using a :func:"tab" instance.
 
-    Notice that only classes decorated with :func:"~alfasim_sdk.layout.tab" can be placed inside a ``tab bar``.
+    Notice that only classes decorated with :func:"tab" can be placed inside a ``tab bar``.
 
     Example of usage:
 
     .. code-block:: python
 
         @data_model(icon="", caption="My Model")
         class MyModel:
@@ -70,15 +70,15 @@
         return wrap_class(class_)
 
     return apply
 
 
 def tab(*, caption: str) -> Callable:
     """
-    The tab represents a single entry, on the :func:`~alfasim_sdk.layout.tabs` layout.
+    The tab represents a single entry, on the :func:`~tabs` layout.
 
     Notice that only components available at the :ref:`types modules <api-types-section>` can be placed inside a tab.
     """
 
     def apply(class_: type):
         @functools.wraps(class_)
         def wrap_class(class_: type, caption: str):
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/models.py` & `alfasim_sdk-2024.1/src/alfasim_sdk/_internal/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import functools
 from typing import Callable
 from typing import Optional
 
 from alfasim_sdk._internal.alfasim_sdk_utils import get_attr_class
 
 
-def container_model(*, model: type, caption: str, icon: Optional[str]) -> Callable:
+def container_model(
+    *, model: type, caption: str, icon: Optional[str] = None
+) -> Callable:
     """
     ``container_model`` is an object that keeps together many different properties defined by the plugin and allows developers
-    to build user interfaces in a declarative way similar to :func:`~alfasim_sdk.models.data_model`.
+    to build user interfaces in a declarative way similar to :func:`data_model`.
 
-    :func:`~alfasim_sdk.models.container_model` can also hold a reference to a :func:`~alfasim_sdk.models.data_model`
-    declared from the plugin, making this object a parent for all new :func:`~alfasim_sdk.models.data_model` created.
+    ``container_model`` can also hold a reference to a :func:`data_model`
+    declared from the plugin, making this object a parent for all new :func:`data_model` created.
 
     .. rubric:: **Application Required**:
 
-    The following options are required when declaring a :func:`~alfasim_sdk.models.container_model`.
+    The following options are required when declaring a ``container_model``.
 
-    :caption:   A text to be displayed over the Tree.
-    :icon:      Name of the icon to be used over the Tree.
-    :model:     A reference to a class decorated with :func:`~alfasim_sdk.models.data_model`.
+    :param caption:   A text to be displayed over the Tree.
+    :param icon:      Name of the icon to be used over the Tree.
+    :param model:     A reference to a class decorated with :func:`data_model`.
 
     .. note::
 
         Even though the icon parameter is required, it's not currently being used.
 
 
     .. rubric:: **Plugin defined**:
@@ -85,36 +87,45 @@
     .. image:: /_static/images/api/container_model_remove_1.png
         :scale: 80%
 
     .. image:: /_static/images/api/container_model_remove_2.png
         :scale: 80%
 
     """
+    is_model_data_model = (
+        hasattr(model, "__attrs_attrs__")
+        and hasattr(model, "_alfasim_metadata")
+        and model._alfasim_metadata["model"] is None
+    )
+    if not is_model_data_model:
+        raise TypeError(
+            "The `model` argument must be a class decorated with `data_model`"
+        )
 
     def apply(class_):
         @functools.wraps(class_)
         def wrap_class(class_, caption, icon):
             return get_attr_class(class_, caption, icon, model)
 
         return wrap_class(class_, caption, icon)
 
     return apply
 
 
 def data_model(*, caption: str, icon: Optional[str] = None) -> Callable:
     """
-    ```data_model``` is an object that keeps together many different properties defined by the plugin and allows developers
+    ``data_model`` is an object that keeps together many different properties defined by the plugin and allows developers
     to build user interfaces in a declarative way.
 
     .. rubric:: **Application Required**:
 
     The following options are required when declaring a data_model and are used into the user interface
 
-        :caption:   A text to be displayed over the Tree.
-        :icon:      Name of the icon to be used over the Tree.
+    :param caption:   A text to be displayed over the Tree.
+    :param icon:      Name of the icon to be used over the Tree.
 
     .. note::
 
         Even though the icon parameter is required, it's not currently being used.
 
 
     .. rubric:: **Plugin Defined**:
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/constants.py` & `alfasim_sdk-2024.1/src/alfasim_sdk/_internal/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -104,14 +104,44 @@
     Sleicher1962 = "sleicher1962"
     Brauner2001 = "brauner2001"
     Boxall2012 = "boxall2012"
     Brinkman1952AndYeh1964 = "brinkman1952_and_yeh1964"
     FromPlugin = "from_plugin"
 
 
+class EmulsionRelativeViscosityModelType(Enum):
+    ModelDefault = "model_default"
+    Taylor1932 = "taylor1932"
+    Brinkman1952 = "brinkman1952"
+    Mooney1951a = "mooney1951a"
+    Mooney1951b = "mooney1951b"
+    PalRhodes1989 = "pal_rhodes1989"
+    Ronningsen1995 = "ronningsen1995"
+    VolumetricWeight = "volumetric_weight"
+    Woelflin1942 = "woelflin_1942"
+    BarneaMizrahi1976 = "barnea_mizrahi1976"
+    TableBased = "table_based"
+    FromPlugin = "from_plugin"
+
+
+class EmulsionDropletSizeModelType(Enum):
+    ModelDefault = "model_default"
+    Hinze1955 = "hinze1955"
+    Sleicher1962 = "sleicher1962"
+    Brauner2001 = "brauner2001"
+    Boxall2012 = "boxall2012"
+
+
+class EmulsionInversionPointModelType(Enum):
+    ModelDefault = "model_default"
+    BraunerUllmann2002 = "brauner_and_ullmann_2002"
+    Brinkman1952AndYeh1964 = "brinkman1952_and_yeh1964"
+    Constant = "constant"
+
+
 class SolidsModelType(Enum):
     """
     Informs which solid model should be used:
 
     - NoModel - None:RR
         Without slip velocity and slurry viscosity
 
@@ -120,27 +150,32 @@
 
     - Santamaria2010Equilibrium - Santamaría-Holek (2010):
         This model is more appropriate to use when the solid phase has properties similar to or equal to hydrate.
         It was fitted by Qin et al. (2018) for hydrates.
 
     - Thomas1965Equilibrium - Thomas (1965):
         Employs the equilibrium slip velocity model and the Thomas (1965) effective dynamic viscosity expression.
+
+    - FromPlugin:
+        Slip velocity and slurry viscosity are calculated from plugin hooks with an external implementation.
     """
 
     NoModel = "no_model"
     Thomas1965Equilibrium = "thomas1965_equilibrium"
     Mills1985Equilibrium = "mills1985_equilibrium"
     Santamaria2010Equilibrium = "santamaria2010_equilibrium"
+    FromPlugin = "from_plugin"
 
 
 class NodeCellType(Enum):
     Internal = "internal_node"
     MassSource = "mass_source_boundary"
     Pressure = "pressure_boundary"
     Separator = "separator_node"
+    Controller = "controller_node"
 
 
 class MassInflowSplitType(Enum):
     """
     PvtUserGorWc is currently only used for GenKey
     """
 
@@ -243,14 +278,36 @@
     Do not rely on the value of this enum, it is used exclusively for backward compatibility
     """
 
     HydrocarbonOnly = "hydrocarbon_only"
     HydrocarbonAndWater = "hydrocarbon_and_water"
 
 
+class DrainageRateMode(Enum):
+    """
+    Drainage Rate mode used by Surge Volume curves calculation.
+    """
+
+    #: Uses a default drain flow rate = (AccLiq(end_time) - AccLiq(start_time))/(end_time - start_time)
+    Automatic = "automatic"
+    #: Allows the user to input a maximum drainage rate
+    UserDefined = "user_defined"
+
+
+class SurgeVolumeTimeMode(Enum):
+    """
+    Time mode used by Surge Volume curves calculation.
+    """
+
+    #: Uses the initial and final time of the whole simulation.
+    AllSimulation = "all_simulation"
+    #: Uses custom initial/final time input by the user.
+    UserDefined = "user_defined"
+
+
 class FlowDirection(Enum):
     Forward = "forward"
     Backward = "backward"
 
 
 class InterpolationType(Enum):
     Constant = "constant"
@@ -292,42 +349,100 @@
     Default = "default"
     Robust = "robust"
 
 
 DEFAULT_TEMPERATURE_IN_K = 288.6
 
 
+class MultiInputType(Enum):
+    Constant = "constant"
+    Curve = "curve"
+
+
 class PumpType(Enum):
     ConstantPressure = "constant_pressure"
     TableInterpolation = "table_interpolation"
+    ElectricSubmersiblePump = "electric_submersible_pump"
 
 
 class ValveOpeningType(Enum):
     ConstantOpening = "constant_opening"
     TableInterpolation = "table_interpolation"
 
 
 class ValveType(Enum):
     PerkinsValve = "perkins_valve"
     ChokeValveWithFlowCoefficient = "choke_valve_with_flow_coefficient"
     CheckValve = "check_valve"
 
 
+class LeakModel(Enum):
+    Orifice = "orifice"
+    FlowCoefficient = "flow_coefficient"
+    GasLiftValve = "gas_lift_valve"
+
+
+class LeakType(Enum):
+    Internal = "internal"
+    External = "external"
+
+
+class GasLiftValveOpeningType(Enum):
+    MinimumPressureDifference = "minimum_pressure_difference"
+    PressureOperated = "pressure_operated"
+
+
 class CompressorSpeedType(Enum):
     SpeedCurve = "speed_curve"
     ConstantSpeed = "constant_speed"
 
 
+class PumpViscosityModel(Enum):
+    """
+    Defines a viscosity model correction to ESP
+        - ``NoModel``: Viscosity model correction is disabled.
+        - ``AnsiHi2010``: Applies the ANSI-HI(2010) viscosity correction.
+    """
+
+    NoModel = "no_model"
+    AnsiHi2010 = "ansihi_2010"
+
+
+class PumpThermalEfficiencyModel(Enum):
+    """
+    Defines the pump thermal efficiency model
+        - ``Constant``: An user-defined constant value is used to define to transform the ESP mechanical energy to heat.
+        - ``PumpEfficiencyCurve``: The ESP efficiency curve is used to transform the ESP mechanical energy to heat.
+    """
+
+    Constant = "constant"
+    PumpEfficiencyCurve = "efficiency_curve_based"
+
+
 class OutputAttachmentLocation(Enum):
     """
     Output Attachment Location will tell the location in which this attachment's data should be retrieved from.
     """
 
     Main = "main"
     Annulus = "annulus"
+    NotDefined = "not_defined"
+
+
+LeakLocation = OutputAttachmentLocation
+
+
+class EquipmentAttachmentLocation(Enum):
+    """
+    Location in which an equipment can be attached.
+    """
+
+    Main = "main"
+    Annulus = "annulus"
+    Both = "both"
 
 
 class CorrelationPackage(Enum):
     Lasater = "pvt_correlation_package_lasater"
     Standing = "pvt_correlation_package_standing"
     VazquezBeggs = "pvt_correlation_package_vazquez_beggs"
     Glaso = "pvt_correlation_package_glaso"
@@ -355,7 +470,72 @@
     """
     Available ports for connecting to a Well node.
     """
 
     Top = "port"  # 'port' is being used for backwards compatibility.
     LeftAnnulus = "left_annulus_port"
     RightAnnulus = "right_annulus_port"
+
+
+class ControllerType(Enum):
+    PID = "pid"
+
+
+class PigTrappingMode(Enum):
+    """
+    Trapping mode of a PIG equipment.
+    """
+
+    #: The PIG is automatically trapped whenever it reaches a boundary node (e.g.,
+    #: pressure or mass boundary).
+    Automatic = "automatic"
+
+    #: The PIG is trapped according to user-defined pipe and position unless it
+    #: reaches a boundary node first.
+    UserDefined = "user_defined"
+
+
+class PigRoutingMode(Enum):
+    """
+    Trapping mode of a PIG equipment.
+    """
+
+    #: When a PIG encounters an internal node, the next pipe in which the PIG goes to
+    #: is selected based on the pipe with greatest total mass flow rate at that point.
+    Automatic = "automatic"
+
+    #: When a PIG encounters an internal node, the next pipe in which the PIG goes
+    #: to is selected based on a user-defined trajectory (edge group).
+    UserDefined = "user_defined"
+
+
+class FlowPatternModel(Enum):
+    """
+    Model used for identify the current flow pattern in a given pipe position.
+    """
+
+    UnitCell = "unit_cell"
+    RegimeCapturing = "regime_capturing"
+
+
+MULTI_INPUT_TYPE_SUFFIX = "_input_type"
+
+
+class CorrelationsOilViscosity(Enum):
+    Egbogah = "Egbogah"
+
+
+class CorrelationsGasViscosity(Enum):
+    LeeGonzalezEakin = "Lee Gonzalez Eakin"
+
+
+class CorrelationsSurfaceTension(Enum):
+    BakerSwerdloff = "Baker Swerdloff"
+
+
+class ForchheimerCoefficientsOption(Enum):
+    """
+    Option for the Forchheimer IPR coefficients definition.
+    """
+
+    ReservoirParameters = "reservoir_parameters"
+    FlowCoefficients = "flow_coefficients"
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/variables.py` & `alfasim_sdk-2024.1/src/alfasim_sdk/_internal/variables.py`

 * *Files 9% similar despite different names*

```diff
@@ -67,23 +67,23 @@
 
 @attr.s(kw_only=True)
 class SecondaryVariable:
     """
     Secondary variables are those variables that are not unknowns from the nonlinear system.
     That is, they are not directly solved in the nonlinear system, but they are calculated based on the nonlinear system results.
 
-    :param name: Plugin secondary variable name. This name will be used to access it in the :ref:`solver_hooks`.
-    :param caption: Caption to be shown in the GUI (For output purpose).
-    :param type: a :class:`~alfasim_sdk.Type` value.
-    :param unit: A string with the unit of the variable.
-    :param visibility: a :class:`~alfasim_sdk.Visibility` value.
-    :param location: a :class:`~alfasim_sdk.Location` value.
-    :param multifield_scope: a :class:`~alfasim_sdk.Scope`.
-    :param default_value: Default value to be set.
-    :param checked_on_gui_default: If the added variable has :class:`~alfasim_sdk.Visibility` equal to ``Output``,
+    :ivar name: Plugin secondary variable name. This name will be used to access it in the :ref:`solver_hooks`.
+    :ivar caption: Caption to be shown in the GUI (For output purpose).
+    :ivar type: a :class:`~Type` value.
+    :ivar unit: A string with the unit of the variable.
+    :ivar visibility: a :class:`~Visibility` value.
+    :ivar location: a :class:`~Location` value.
+    :ivar multifield_scope: a :class:`~Scope`.
+    :ivar default_value: Default value to be set.
+    :ivar checked_on_gui_default: If the added variable has :class:`~Visibility` equal to ``Output``,
         it indicates that this variable will be exported as output by default.
 
     The ``unit`` param accepts all units available on `Barril <https://github.com/ESSS/barril>`_ Unit Manager, for
     more information read its `documentation <https://barril.readthedocs.io/en/latest/>`_.
 
     .. note::
         This type is supposed to be used in the :py:func:`~alfasim_sdk._internal.hook_specs_gui.alfasim_get_additional_variables` `hook`.
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/status.py` & `alfasim_sdk-2024.1/src/alfasim_sdk/_internal/status.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 
 @attr.s(kw_only=True)
 class ErrorMessage:
     """
     ErrorMessage allows the plugin to display a message over the status monitor, and signalize to the application to block
     the simulation until the issue is fixed.
 
-    :param model_name: Name of the model that issues the error.
-    :param message: Message that will be displayed over the status monitor.
+    :ivar model_name: Name of the model that issues the error.
+    :ivar message: Message that will be displayed over the status monitor.
 
-    Checkout the :func:`~alfasim_sdk.hook_specs_gui.alfasim_get_status` for some examples of :func:`~alfasim_sdk.status.ErrorMessage` in action.
+    Checkout the :func:`~alfasim_sdk._internal.hook_specs_gui.alfasim_get_status` for some examples of ```ErrorMessage``` in action.
     """
 
     model_name: str = attrib(validator=non_empty_str)
     message: str = attrib(validator=non_empty_str)
 
 
 @attr.s(kw_only=True)
 class WarningMessage:
     """
     WarningMessage allows the plugin to display a message to the user over the status monitor, and signalizes a minor
     issue that needs to be fixed but doesn't block the simulation.
 
-    :param model_name: Name of the model that issues the warning.
-    :param message: Message that will be displayed over the status monitor.
+    :ivar model_name: Name of the model that issues the warning.
+    :ivar message: Message that will be displayed over the status monitor.
 
-    Checkout the :func:`~alfasim_sdk.hook_specs_gui.alfasim_get_status` for some examples of :func:`~alfasim_sdk.status.WarningMessage` in action.
+    Checkout the :func:`~alfasim_sdk._internal.hook_specs_gui.alfasim_get_status` for some examples of ```WarningMessage``` in action.
     """
 
     model_name: str = attrib(validator=non_empty_str)
     message: str = attrib(validator=non_empty_str)
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/hook_specs.py` & `alfasim_sdk-2024.1/src/alfasim_sdk/_internal/hook_specs.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         :emphasize-lines: 1
 
         HOOK_FINALIZE(ctx)
         {
             // Threads information
             int n_threads = -1;
             int errcode = alfasim_sdk_api.get_number_of_threads(ctx, &n_threads);
-            f (errcode != 0){ // or errcode != OK
+            if (errcode != 0){ // or errcode != OK
                 return errcode;
             }
             const char* plugin_id = get_plugin_id();
             // Plugin internal data
             for (int thread_id = 0; thread_id < n_threads; ++thread_id) {
                 void* data = nullptr;
                 errcode = alfasim_sdk_api.get_plugin_data(
@@ -138,25 +138,25 @@
         :emphasize-lines: 1
 
         HOOK_UPDATE_PLUGINS_SECONDARY_VARIABLES(ctx)
         {
             int errcode = -1;
             int size_U = -1;
             int size_E = -1;
-            int liq_id = -1;
+            int oil_id = -1;
             errcode = alfasim_sdk_api.get_field_id(
                 ctx, &oil_id, "oil");
             double* vel;
             VariableScope Fields_OnFaces = {
                 GridScope::FACE,
                 MultiFieldDescriptionScope::FIELD,
                 TimestepScope::CURRENT
             }
             errcode = alfasim_sdk_api.get_simulation_array(
-                ctx, &vel, (char*) "U", Fields_OnFaces, liq_id, &size_U);
+                ctx, &vel, (char*) "U", Fields_OnFaces, oil_id, &size_U);
             double* kinetic_energy;
             char* name = "kinetic_energy_of_oil";
             int global_idx = 0;
             errcode = alfasim_sdk_api.get_plugin_variable(
                 ctx,
                 (void**) (&kinetic_energy),
                 name,
@@ -174,14 +174,72 @@
 
     In the example above the variable ``kinetic_energy_of_oil`` was registered as a global variable, but its value is
     obtained for `oil field`. If this variable would be calculated to all fields then the ``global_idx`` would be
     substituted by ``field_idx`` and it would be performed to each `field`.
     """
 
 
+def update_plugins_secondary_variables_time_explicit(ctx: "void*") -> "int":
+    """
+    **c++ signature** : ``HOOK_UPDATE_PLUGINS_SECONDARY_VARIABLES_TIME_EXPLICIT(void* ctx)``
+
+    Internal simulator hook to update plugin's secondary variables time explicit.
+    This is called only once at the end of ALFAsim's update internal secondary variables workflow.
+
+    :param ctx: ALFAsim's plugins context
+    :returns: Return OK if successful or anything different if failed
+
+    Example of usage:
+
+    .. code-block:: c++
+        :linenos:
+        :emphasize-lines: 1
+
+        HOOK_UPDATE_PLUGINS_SECONDARY_VARIABLES_TIME_EXPLICIT(ctx)
+        {
+            int errcode = -1;
+            int size_U = -1;
+            int size_E = -1;
+            int liq_id = -1;
+            errcode = alfasim_sdk_api.get_field_id(
+                ctx, &oil_id, "oil");
+            double* vel;
+            VariableScope Fields_OnFaces = {
+                GridScope::FACE,
+                MultiFieldDescriptionScope::FIELD,
+                TimestepScope::CURRENT
+            }
+            errcode = alfasim_sdk_api.get_simulation_array(
+                ctx, &vel, (char*) "U", Fields_OnFaces, liq_id, &size_U);
+            double* kinetic_energy;
+            char* name = "kinetic_energy_of_oil";
+            int global_idx = 0;
+            errcode = alfasim_sdk_api.get_plugin_variable(
+                ctx,
+                (void**) (&kinetic_energy),
+                name,
+                global_idx,
+                TimestepScope::CURRENT,
+                &size_E);
+            if (size_U != size_E){
+                return OUT_OF_BOUNDS;
+            }
+            for (int i =0; i < size_U; ++i){
+                kinetic_energy[i] = vel[i] * vel[i] / 2.;
+            }
+            return OK;
+        }
+
+    In the example above the variable ``kinetic_energy_of_oil`` was registered as a global variable, but its value is
+    obtained for `oil field` and only at the end of the time steps' linear solver (explicit approach). If this
+    variable would be calculated to all fields then the ``global_idx`` would be substituted by ``field_idx`` and it
+    would be performed to each `field`.
+    """
+
+
 def update_plugins_secondary_variables_on_first_timestep(ctx: "void*") -> "int":
     """
     **c++ signature** : ``HOOK_UPDATE_PLUGINS_SECONDARY_VARIABLES_ON_FIRST_TIMESTEP(void* ctx)``
 
     Internal simulator hook to update plugin's secondary variables on the first timestep.
     This is called as the first step on ALFAsim's update internal variables workflow.
     This method is specially important when you have a plugin which the secondary variables depend
@@ -505,46 +563,51 @@
 
 
 def initialize_state_variables_calculator(
     ctx: "void*",
     P: "void*",
     T: "void*",
     T_mix: "void*",
+    phi: "void*",
     n_control_volumes: "int",
     n_layers: "int",
+    n_tracers: "int",
 ) -> "int":
     """
     **c++ signature** : ``HOOK_INITIALIZE_STATE_VARIABLES_CALCULATOR(void* ctx, void* P, void* T, void* T_mix,
-    int n_control_volumes, int n_layers)``
+    void* phi, int n_control_volumes, int n_layers, int n_tracers)``
 
     Hook for the state variables calculator initialization (internal ``ALFAsim`` structure).
 
     At this point, it is possible to pre-calculate and cache any relevant information. Then, for each state variable of
     the phases in the python configuration file, the `hook` :py:func:`HOOK_CALCULATE_STATE_VARIABLE<alfasim_sdk._internal.hook_specs.calculate_state_variable>`
     is called and return the pre-calculated values.
 
     :param ctx: ALFAsim's plugins context
     :param P: Pressure values array
     :param T: Temperature values array
     :param T_mix: Mixture temperature values array
+    :param phi: Tracer mass fraction values array
     :param n_control_volumes: Number of control volumes
     :param n_layers: Number of layers
+    :param n_tracers: Number of tracers in the system
     :returns: Return OK if successful or anything different if failed
 
     The ``P`` and ``T_mix`` have size equal to ``n_control_volumes``. However, ``T`` has values contiguous in memory
-    and its dimensions are given by ``n_layers`` and ``n_control_volumes``
+    and its dimensions are given by ``n_layers`` and ``n_control_volumes``. Finally, ``phi`` dimensions are given by
+    ``n_tracers`` and ``n_control_volumes``.
 
     Example of usage:
 
     .. code-block:: c++
         :linenos:
         :emphasize-lines: 1
 
         HOOK_INITIALIZE_STATE_VARIABLES_CALCULATOR(
-            ctx, P, T, T_mix, n_control_volumes, n_layers)
+            ctx, P, T, T_mix, phi, n_control_volumes, n_layers, n_tracers)
         {
             // getting plugin internal data
             int errcode = -1;
             int thread_id = -1;
             errcode = alfasim_sdk_api.get_thread_id(ctx, &thread_id);
             if (errcode != OK) {
                 return errcode;
@@ -557,15 +620,15 @@
             // MyFunction is a function implemented by
             // plugin developer that computes de density
             data.density = MyFunction(P, T_mix, n_control_volumes);
             return OK;
         }
         // Then, to use the cached value:
         HOOK_CALCULATE_STATE_VARIABLE(
-            ctx, P, T, n_control_volumes, n_layers, phase_id, property_id, output)
+            ctx, P, T, n_control_volumes, phase_id, field_id, property_id, output)
         {
             // getting plugin internal data
             int errcode = -1;
             int thread_id = -1;
             errcode = alfasim_sdk_api.get_thread_id(ctx, &thread_id);
             if (errcode != OK) {
                 return errcode;
@@ -595,20 +658,21 @@
 
 def calculate_state_variable(
     ctx: "void*",
     P: "void*",
     T: "void*",
     n_control_volumes: "int",
     phase_id: "int",
+    field_id: "int",
     property_id: "int",
     output: "void*",
 ) -> "int":
     """
-    **c++ signature** : ``HOOK_CALCULATE_STATE_VARIABLE(void* ctx, void* P, void* T, int n_control_volumes, int n_layers,
-    int phase_id, int property_id, void* output)``
+    **c++ signature** : ``HOOK_CALCULATE_STATE_VARIABLE(void* ctx, void* P, void* T, int n_control_volumes,
+    int phase_id, int field_id, int property_id, void* output)``
 
     Hook to calculate the state variable given by the `property_id` (See :cpp:enum:`StateVariable` values), for the
     phase with `phase_id` (Note that the phase id is the same as the one retrieved from the :cpp:func:`get_phase_id` API
     function - It is not advisable to use hardcoded numbers).
 
     List of affected variables:|br|
     - ``Density`` |br|
@@ -619,34 +683,41 @@
     - ``Enthalpy`` |br|
     - ``Thermal Conductivity`` |br|
 
     :param ctx: ALFAsim's plugins context
     :param P: Pressure values array
     :param T: Temperature values array
     :param n_control_volumes: Number of control volumes
-    :param n_layers: Number of layers
     :param n_phase_id: Id of phase in which the property must be calculated
+    :param n_field_id: Id of field in which the property must be calculated (Associated to the phase)
     :param property_id: A :cpp:enum:`StateVariable` value. It indicates which
                         property must be calculated
     :param output: Output values array
     :returns: Return OK if successful or anything different if failed
 
     The ``output`` parameter must be filled with the calculated property for each control volume. The
     pressure ``P`` and layer or mixture temperature ``T`` (Depending on the energy model being used)
     are given in order to perform the calculation. The number of control volumes is also given for
     convenience.
 
+    In case of calculating all properties and caching them in the :py:func:`HOOK_INITIALIZE_STATE_VARIABLES_CALCULATOR<alfasim_sdk._internal.hook_specs.initialize_state_variables_calculator>`
+    (depending on the model used inside the plugin) the ``field_id`` can be used to retrieve the cached
+    properties for a specific field associated to the phase in which ``phase_id`` is informed. For
+    example, when the energy model for layers is used in a simulation, fields of a phase may be in
+    others layers ("oil in water" is located in the "water" layer) in which the temperature are different.
+
+
     Example of usage:
 
     .. code-block:: c++
         :linenos:
         :emphasize-lines: 1
 
         HOOK_CALCULATE_STATE_VARIABLE(
-            ctx, P, T, n_control_volumes, n_layers, phase_id, property_id, output)
+            ctx, P, T, n_control_volumes, phase_id, field_id, property_id, output)
         {
             // getting plugin internal data
             int errcode = -1;
             int thread_id = -1;
             errcode = alfasim_sdk_api.get_thread_id(ctx, &thread_id);
             if (errcode != OK) {
                 return errcode;
@@ -680,51 +751,58 @@
 def calculate_phase_pair_state_variable(
     ctx: "void*",
     P: "void*",
     T_mix: "void*",
     n_control_volumes: "int",
     phase1_id: "int",
     phase2_id: "int",
+    phase_pair_id: "int",
     property_id: "int",
     output: "void*",
 ) -> "int":
     """
     **c++ signature** : ``HOOK_CALCULATE_PHASE_PAIR_STATE_VARIABLE(void* ctx, void* P, void* T_mix, int n_control_volumes,
-    int phase1_id, int phase2_id, int property_id, void* output)``
+    int phase1_id, int phase2_id, int phase_pair_id, int property_id, void* output)``
 
     Hook to calculate the state variable given by the `property_id` (See :cpp:enum:`StateVariable` values), for the phase
     pair `(phase1_id, phase2_id)` (Note that the phase id is the same as the one retrieved from the :cpp:func:`get_phase_id()`
     API function - It is not advisable to use hardcoded numbers).
 
     List of affected variables:|br|
     - ``Interfacial Tension``
 
     :param ctx: ALFAsim's plugins context
     :param P: Pressure values array
     :param T_mix: Mixture temperature values array
     :param n_control_volumes: Number of control volumes
-    :param n_phase1_id: Id of phase one in which the property must be calculated
-    :param n_phase2_id: Id of phase two in which the property must be calculated
+    :param phase1_id: Id of phase one in which the property must be calculated
+    :param phase2_id: Id of phase two in which the property must be calculated
+    :param phase_pair_id: Id of the phase pair in which the property must be calculated
     :param property_id: A :cpp:enum:`StateVariable` value. It indicates which
                         property must be calculated
     :param output: Output values array
     :returns: Return OK if successful or anything different if failed
 
     The output parameter must be filled with the calculated property for each control volume. The
     pressure ``P`` and mixture temperature ``T_mix`` are given in order to perform the calculation.
     The number of control volumes is also given for convenience.
 
+    Since the state properties calculated by this hook is performed for phase pairs, the information
+    of the phases involved is provided by the ``phase_pair_id`` and also by the single phase IDs called
+    ``phase1_id`` and  ``phase2_id``. To identify which ``phase_pair_id`` are being passed it is possible
+    to retrieve the phase pair IDs by using :cpp:func:`get_phase_pair_id`.
+
     Example of usage:
 
     .. code-block:: c++
         :linenos:
         :emphasize-lines: 1
 
         HOOK_CALCULATE_PHASE_PAIR_STATE_VARIABLE(
-            ctx, P, T_mix, n_control_volumes, phase1_id, phase2_id, property_id, output)
+            ctx, P, T_mix, n_control_volumes, phase1_id, phase2_id, phase_pair_id, property_id, output)
         {
             // getting plugin internal data
             int errcode = -1;
             int thread_id = -1;
             errcode = alfasim_sdk_api.get_thread_id(ctx, &thread_id);
             if (errcode != OK) {
                 return errcode;
@@ -910,58 +988,155 @@
         }
 
     """
 
 
 def calculate_slip_velocity(
     ctx: "void*",
-    U_fields: "void*",
-    alpha_f: "void*",
-    d_disp_fields: "void*",
-    P: "void*",
-    rho_f: "void*",
-    mu_f: "void*",
-    sin_theta_f: "void*",
-    delta_x_f: "void*",
+    U_slip: "double*",
+    solid_field_index: "int",
+    layer_index: "int",
+    n_faces: "int",
 ) -> "int":
     """
-    Internal simulator hook to calculate slip velocity between fluids
-    and solid phase.
+    **c++ signature** : ``HOOK_CALCULATE_SLIP_VELOCITY(void* ctx, double* U_slip, int solid_field_index, int layer_index, int n_faces)``
+
+    Internal `hook` to calculate slip velocity in the Solids Model.
+    This `hook` will be used in the solids model to calculate the slip velocity between
+    fluid and solid phase.
+
+    The output variable ``U_slip`` is the slip velocity with size equal to ``n_faces`` and it
+    is dimensionless.
+    The ``solid_field_index`` is the index of the dispersed solid field.
+    The ``layer_index`` is the index of the layer and continuous field in the layer (in which the solid
+    field is dispersed).
+
+    .. Note::
+        It is important to know that the calculations for velocity is performed over the faces (see
+        ``n_faces`` param). For that, any variable that should be retrieved using :cpp:func:`get_simulation_array`
+        must be use value ``FACE`` in the :cpp:enum:`GridScope` param.
 
     :param ctx: ALFAsim's plugins context
-    :param U_fields: Field velocities,
-    :param alpha_f: Field Volume fractions on faces,
-    :param d_disp_fields: Diameter of dispersed fields,
-    :param P: Pressure,
-    :param rho_f: Field densities on faces,
-    :param mu_f: Field viscosities on faces,
-    :param sin_theta_f: Sin of Theta on faces in which Theta is the angle between the Pipe and the Y-Axis,
-    :param delta_x_f: The control volume lenght related to the faces,
+    :param U_slip: Slip velocity between fluid and solid phase
+    :param solid_field_index: Index of the dispersed solid field
+    :param layer_index: Index of the Layer or Continuous Field
+    :param n_faces: Number of faces.
 
     :returns: Return OK if successful or anything different if failed
 
-    It is expected to be changed the U_fields of solid phase, whose index will be available via API.
+    Example of usage:
+
+    .. code-block:: c++
+        :linenos:
+        :emphasize-lines: 1
+
+        HOOK_CALCULATE_SLIP_VELOCITY(ctx, U_slip, disp_field_index, layer_index, n_faces)
+        {
+            const char* plugin_id = get_plugin_id()
+            errcode = alfasim_sdk_api.get_thread_id(ctx, &thread_id);
+            if (errcode != OK) {
+                return errcode;
+            }
+            // MyStruct is a developer defined struct to hold
+            // all important information for plugin hooks.
+            MyStruct* data = nullptr;
+            errcode = alfasim_sdk_api.get_plugin_data(ctx, (void**) &data, plugin_id, thread_id);
+            if (errcode != OK) {
+                return errcode;
+            }
+
+            // compute the slip velocity using your own correlation
+            for (int i = 0; i < n_faces; ++i){
+                U_slip[i] = slip_velocity[i];
+            }
+
+            return OK;
+        }
     """
 
 
-def calculate_slurry_viscosity(
-    ctx: "void*", alpha_f: "void*", mu_f: "void*", mu_f_layer: "void*"
+def calculate_relative_slurry_viscosity(
+    ctx: "void*",
+    mu_r: "double*",
+    solid_field_index: "int",
+    layer_index: "int",
+    n_faces: "int",
 ) -> "int":
     """
-    Internal simulator hook to calculate slurry viscosity of layer(s).
+    **c++ signature** : ``HOOK_RELATIVE_SLURRY_VISCOSITY(void* ctx, double* mu_r, int solid_field_index, int layer_index, int n_faces)``
 
-    :param ctx: ALFAsim's plugins context
-    :param alpha_f: Fields Volume fractions on faces,
-    :param mu_f: Field viscosities on faces,
-    :param mu_f_layer: Layer Viscosities on faces,
+    Internal `hook` to calculate the relative slurry viscosity in the Solids Model.
+    This `hook` will be used in the Solids model to calculate the effective viscosity of the slurry
+    (solid field + continuous field).
+
+    The relative slurry viscosity is defined by:
+
+    .. math::
 
+        \\begin{equation}
+            \\mu_r = \\frac{\\mu_{eff}}{\\mu_c}
+        \\end{equation}
+
+
+    .. rubric:: Where
+
+    :1: :math:`\\mu_r` is the relative emulsion viscosity
+    :2: :math:`\\mu_{eff}` is the effective viscosity
+    :3: :math:`\\mu_c` is the viscosity of the continuous field
+
+    The output variable ``mu_r`` is the relative slurry viscosity with size equal to ``n_faces`` and it
+    is dimensionless.
+    The ``solid_field_index`` is the index of the dispersed solid field.
+    The ``layer_index`` is the index of the layer and continuous field in the layer (in which the solid
+    field is dispersed).
+
+    .. Note::
+        It is important to know that the calculations for viscosity is performed over the faces (see
+        ``n_faces`` param). For that, any variable that should be retrieved using :cpp:func:`get_simulation_array`
+        must be use value ``FACE`` in the :cpp:enum:`GridScope` param.
+
+    This `hook` allows the implementation of the relative slurry viscosity correlation. Once the plugin
+    installed it is important to be selected in the solids model configuration inside the Physics data
+    tree in the ALFAsim application in order to be used.
+
+    :param ctx: ALFAsim's plugins context
+    :param mu_r: Relative slurry viscosity
+    :param solid_field_index: Index of the dispersed solid field
+    :param layer_index: Index of the Layer or Continuous Field
+    :param n_faces: Number of faces.
     :returns: Return OK if successful or anything different if failed
 
-    It is expected to be changed the mu_f_layer of oil layer(continuous oil and dispersed solid),
-    whose index will be available via API.
+    Example of usage:
+
+    .. code-block:: c++
+        :linenos:
+        :emphasize-lines: 1
+
+        HOOK_RELATIVE_SLURRY_VISCOSITY(ctx, mu_r, solid_field_index, layer_index, n_faces)
+        {
+            const char* plugin_id = get_plugin_id()
+            errcode = alfasim_sdk_api.get_thread_id(ctx, &thread_id);
+            if (errcode != OK) {
+                return errcode;
+            }
+            // MyStruct is a developer defined struct to hold
+            // all important information for plugin hooks.
+            MyStruct* data = nullptr;
+            errcode = alfasim_sdk_api.get_plugin_data(ctx, (void**) &data, plugin_id, thread_id);
+            if (errcode != OK) {
+                return errcode;
+            }
+
+            // compute the relative slurry viscosity using your own correlation
+            for (int i = 0; i < n_faces; ++i){
+                mu_r[i] = relative_slurry_viscosity[i];
+            }
+
+            return OK;
+        }
     """
 
 
 def initialize_mass_fraction_of_tracer(
     ctx: "void*", phi_initial: "void*", tracer_index: "int"
 ) -> "int":
     """
@@ -1401,16 +1576,16 @@
 
     The ``ll_fp`` must be one of the following values: |br|
     - `0 - Unknown`: Unknown Flow Pattern. |br|
     - `1 - Ambivalent`: Ambivalent Flow Pattern between Dispersed Oil and Dispersed Water. |br|
     - `2 - Dispersed Oil`: Dispersed oil in continuous water. |br|
     - `3 - Dispersed Water`: Dispersed water in continuous Oil. |br|
     - `4 - Separated`: Separated continuous oil and continuous water. |br|
-    - `5 - separated Mixed`: Separated with dispersed oil and water droplets. |br|
-    - `6 - separated Wavy`: Separated with waves. |br|
+    - `5 - Separated Wavy`: Separated with waves. |br|
+    - `6 - Separated Mixed`: Separated with dispersed oil and water droplets. |br|
 
     Any value different from these values will be assumed an `Unknown` flow pattern.
 
     :param ctx: ALFAsim's plugins context
     :param ll_fp: Liquid-Liquid Flow Pattern
     :param water_vol_frac: Volume fraction of water in the Liquid-Liquid System
     :returns: Return OK if successful or anything different if failed
@@ -1661,24 +1836,24 @@
         }
     """
 
 
 def calculate_relative_emulsion_viscosity(
     ctx: "void*",
     mu_r: "double*",
-    disp_field_index: "int",
-    layer_index: "int",
-    n_faces: "int",
+    mu_disp: "double",
+    mu_cont: "double",
+    alpha_disp_in_layer: "double",
+    T: "double",
+    water_in_oil: "bool",
 ) -> "int":
     """
-    **c++ signature** : ``HOOK_RELATIVE_EMULSION_VISCOSITY(void* ctx, double* mu_r, int disp_field_index, int layer_index, int n_faces)``
+    **c++ signature** : ``HOOK_RELATIVE_EMULSION_VISCOSITY(void* ctx, double* mu_r, double mu_disp, double mu_cont, double alpha_disp_in_layer, double T, bool water_in_oil)``
 
-    Internal `hook` to calculate the relative emulsion viscosity in the Emulsion Model.
-    This `hook` will be used in the emulsion model to calculate the apparent viscosity of the emulsion
-    (Continuous field + dispersed field).
+    Internal `hook` to calculate the relative emulsion viscosity of an oil-water dispersion (emulsion)
 
     The relative emulsion viscosity is defined by:
 
     .. math::
 
         \\begin{equation}
             \\mu_r = \\frac{\\mu_m}{\\mu_c}
@@ -1687,69 +1862,43 @@
 
     .. rubric:: Where
 
     :1: :math:`\\mu_r` is the relative emulsion viscosity
     :2: :math:`\\mu_m` is the apparent viscosity
     :3: :math:`\\mu_c` is the viscosity of the continuous field
 
-    The output variable ``mu_r`` is the relative emulsion viscosity with size equal to ``n_faces`` and it
-    is dimensionless.
-    The ``disp_field_index`` is the index of the dipersed field. Since it is an emulsion dispersed field,
-    it can have values for ``oil in water`` and ``water in oil`` fields.
-    The ``layer_index`` is the index of the layer and continuous field in the layer. Since it is the index
-    of the main field of the emulsion, it can have values for ``oil``  or ``water`` layers (and/or continuous
-    fields).
-
-    .. Note::
-        It is important to know that the calculations for viscosity is performed over the faces (see
-        ``n_faces`` param). For that, any variable that should be retrieved using :cpp:func:`get_simulation_array`
-        must be use value ``Face`` in the :cpp:enum:`GridScope` param.
+    The output variable ``mu_r`` is the relative emulsion viscosity, ``mu_disp`` is the dispersed field
+    viscosity, ``mu_cont`` is the continuous field viscosity and ``alpha_disp_in_layer`` is the volume
+    fraction of dispersed field in the layer (dispersed field plus continuous field), T is the fluid temperature,
+    and water_in_oil is true when water is the dispersed phase and false otherwise.
 
     This `hook` allows the implementation of the relative emulsion viscosity correlation. Once the plugin
     installed it is important to be selected in the emulsion model configuration inside the Physics data
     tree in the ALFAsim application in order to be used.
 
     :param ctx: ALFAsim's plugins context
     :param mu_r: Relative emulsion viscosity
-    :param disp_field_index: Index of the dispersed field
-    :param layer_index: Index of the Layer or Continuous Field
-    :param n_faces: Number of faces.
+    :param mu_disp: Dispersed field viscosity
+    :param mu_cont: Continuous field viscosity
+    :param alpha_disp_in_layer: Volume fraction of dispersed field in layer.
+    :param T: Fluid temperature
+    :param water_in_oil: True when water is the dispersed phase
+
     :returns: Return OK if successful or anything different if failed
 
     Example of usage:
 
     .. code-block:: c++
         :linenos:
         :emphasize-lines: 1
 
-        HOOK_RELATIVE_EMULSION_VISCOSITY(ctx, mu_r, disp_field_index, layer_index, n_faces)
+        HOOK_RELATIVE_EMULSION_VISCOSITY(ctx, mu_r, mu_disp, mu_cont, alpha_disp_in_layer, T, water_in_oil)
         {
-            const char* plugin_id = get_plugin_id()
-            errcode = alfasim_sdk_api.get_thread_id(ctx, &thread_id);
-            if (errcode != OK) {
-                return errcode;
-            }
-            // MyStruct is a developer defined struct to hold
-            // all important information for plugin hooks.
-            MyStruct* data = nullptr;
-            errcode = alfasim_sdk_api.get_plugin_data(ctx, (void**) &data, plugin_id, thread_id);
-
-            if (disp_field_index == data.oil_in_water_index){
-                // Calculate the relative emulsion viscosity
-                // for water dominated scenario.
-                // ComputeForWaterDominated is a function implemented
-                // by plugin developer
-                ComputeForWaterDominated(mu_r, n_faces);
-            } else if (disp_field_index == data.water_in_oil_index){
-                // Calculate the relative emulsion viscosity
-                // for oil dominated scenario
-                // ComputeForOilDominated is a function implemented
-                // by plugin developer
-                ComputeForOilDominated(mu_r, n_faces);
-            }
+            // Einstein (1906) relative viscosity model
+            mu_r = 1.0 + 2.5 * alpha_disp_in_layer;
 
             return OK;
         }
     """
 
 
 def friction_factor(v1: "int", v2: "int") -> "int":
@@ -1786,99 +1935,93 @@
         Entrainment fraction, defined as the ratio between the droplet mass flow rate and the total liquid
         mass flow rate (dimensionless)
     """
 
 
 def update_internal_deposition_layer(
     ctx: "void*",
-    thickness: "void*",
+    phase_id: "int*",
+    thickness_variation_rate: "void*",
     density: "void*",
     heat_capacity: "void*",
     thermal_conductivity: "void*",
     n_control_volumes: "int",
 ) -> "int":
     """
-    **c++ signature** : ``HOOK_UPDATE_INTERNAL_DEPOSITION_LAYER(void* ctx, void* thickness, void* density, void* heat_capacity, void* thermal_conductivity,
-    int n_control_volumes)``
+    **c++ signature** : ``HOOK_UPDATE_INTERNAL_DEPOSITION_LAYER(void* ctx, int* phase_id, void* thickness_variation_rate,
+    void* density, void* heat_capacity, void* thermal_conductivity, int n_control_volumes)``
 
-    Internal simulator hook to evaluate the thickness and thermal properties of the deposited layer at the inside of the pipeline walls.
-    This is called for accounting the diameter reduction and wall thermal effects.
+    Internal simulator hook to evaluate the deposition volumetric rate and thermal properties of the deposited layer on
+    pipeline walls. This is called for accounting the inner diameter reduction and wall thermal effects.
 
-    The plugin is supposed to change the given ``thickness``, ``density``, ``heat_capacity``, ``thermal_conductivity`` array pointers. Its values are contiguous
-    in memory and the dimension is given by ``n_control_volumes``. It has unit equal to ``[m]``.
+    The plugin is supposed to change ``thickness_variation_rate``, ``density``, ``heat_capacity``,
+    ``thermal_conductivity`` array pointers, as well as the integer value phase_id. The array pointers must be contiguous
+    in memory and their dimension is given by ``n_control_volumes``.
 
     :param ctx: ALFAsim's plugins context
-    :param thickness: Thickness of the internal deposit layer
+    :param phase_id: Id of phase that is being deposited on pipe walls
+    :param thickness_variation_rate: Rate of change of deposition layer thickness
     :param density: Density of the internal deposit layer [kg/m3]
     :param heat_capacity: Heat capacity of the internal deposit layer [J/(kg.K)]
     :param thermal_conductivity: Thermal conductivity of the internal deposit layer [W/(m.K)]
     :param n_control_volumes: Number of control volumes
     :returns: Return OK if successful or anything different if failed
 
     Example of usage:
 
     .. code-block:: c++
         :linenos:
         :emphasize-lines: 1
 
         HOOK_UPDATE_INTERNAL_DEPOSITION_LAYER(
-            ctx, thickness, density, heat_capacity, thermal_conductivity, n_control_volumes)
+            ctx, phase_id, thickness_variation_rate, density, heat_capacity, thermal_conductivity, n_control_volumes)
         {
             auto errcode = -1;
 
             double dt = -1.0;
             errcode = alfasim.get_simulation_quantity(
                 ctx, &dt, TimestepScope::CURRENT, (char*) "dt");
             if (errcode != 0) {
                 return errcode;
             }
 
-            // Handle first time step, because you won't have the previously information
+            int phase_wax_id = -1;
+            errcode = alfasim.get_phase_id(ctx, &phase_wax_id, "wax");
+            if (errcode != 0) {
+                return errcode;
+            }
+            *phase_id = phase_wax_id;
+
+            // Handle first time step. At this point there is no data from previous time step.
             double current_time = -1.0;
             errcode = alfasim.get_simulation_quantity(
                 ctx, &current_time, TimestepScope::CURRENT, (char*) "time");
             if (errcode != 0) {
                 return errcode;
             }
 
             double wax_density = 900.0 // [kg/m3]
             double wax_heat_capacity = 2140.0 // [J/(kg.K)]
             double wax_thermal_conductivity = 0.25 // [W/(m.K)]
 
             if (current_time == 0.0){
                 // Set a value for the deposition layer thickness
                  for (int i = 0; i < n_control_volumes; ++i) {
-                   (double*) thickness[i] = 0.0; // [m]
+                   (double*) thickness_variation_rate[i] = 0.0; // [m]
                    (double*) density[i] = wax_density; // [kg/m3]
                    (double*) heat_capacity[i] = wax_heat_capacity; //  [J/(kg.K)]
                    (double*) thermal_conductivity[i] = wax_thermal_conductivity; // [W/(m.K)]
                 }
             } else{
-                // Get previously deposition layer thickness to obtain the current
-                void* thickness_old_raw_ptr;
-                errcode = alfasim.get_plugin_variable(
-                    ctx,
-                    &thickness_old_raw_ptr,
-                    "thickness",
-                    0,
-                    TimestepScope::PREVIOUS,
-                    &size);
-                if (errcode != 0) {
-                    return errcode;
-                }
-                auto* thickness_old =
-                    (double*) (thickness_old_raw_ptr);
-
                 // Calculate the variation of the deposition layer in one time step
                 double* d_deposit_layer_dt = 0.0001; // [m/s]
 
                 // Sum this variation with the thickness of the older time step
                 for (int i = 0; i < n_control_volumes; ++i) {
-                    (double*) thickness[i] =
-                        thickness_old[i] + d_deposit_layer_dt * dt; // [m]
+                    (double*) thickness_variation_rate[i] = d_deposit_layer_dt; // [m3/s]
                    (double*) density[i] = wax_density; // [kg/m3]
                    (double*) heat_capacity[i] = wax_heat_capacity; //  [J/(kg.K)]
                    (double*) thermal_conductivity[i] = wax_thermal_conductivity; // [W/(m.K)]
                 }
             }
 
             return OK;
@@ -1896,14 +2039,15 @@
     version="1",
     pyd_name="_alfasim_hooks",
     hooks=[
         initialize,
         finalize,
         # Update secondary variables registered by plugin
         update_plugins_secondary_variables_on_first_timestep,
+        update_plugins_secondary_variables_time_explicit,
         update_plugins_secondary_variables,
         update_plugins_secondary_variables_on_tracer_solver,
         # Calculate source terms
         calculate_mass_source_term,
         calculate_momentum_source_term,
         calculate_energy_source_term,
         calculate_tracer_source_term,
@@ -1911,16 +2055,17 @@
         initialize_state_variables_calculator,
         finalize_state_variables_calculator,
         calculate_state_variable,
         calculate_phase_pair_state_variable,
         # Hooks related to solids phases
         initialize_particle_diameter_of_solids_fields,
         update_particle_diameter_of_solids_fields,
+        # Hooks related to Solids Model
         calculate_slip_velocity,
-        calculate_slurry_viscosity,
+        calculate_relative_slurry_viscosity,
         # Hooks related to Tracer added by plugin
         initialize_mass_fraction_of_tracer,
         calculate_mass_fraction_of_tracer_in_phase,
         calculate_mass_fraction_of_tracer_in_field,
         set_prescribed_boundary_condition_of_mass_fraction_of_tracer,
         update_boundary_condition_of_mass_fraction_of_tracer,
         # Hooks related to UCM Friction Factor
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/validators.py` & `alfasim_sdk-2024.1/src/alfasim_sdk/_internal/validators.py`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk/__init__.py` & `alfasim_sdk-2024.1/src/alfasim_sdk/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# -*- coding: utf-8 -*-
 """Top-level package for alfasim-sdk."""
 import pluggy
 
 from alfasim_sdk._internal import version
+from alfasim_sdk._internal.alfasim_sdk_utils import get_metadata
 from alfasim_sdk._internal.units import register_units
 
 # Package information
 __author__ = "ESSS"
 __email__ = "foss@esss.co"
 __version__ = version.__version__
 
@@ -29,14 +29,15 @@
 
 # CLI:
 from alfasim_sdk._internal.cli import console_main
 
 # ALFACase: Descriptions
 from alfasim_sdk._internal.alfacase.case_description import AnnulusDescription
 from alfasim_sdk._internal.alfacase.case_description import BipDescription
+from alfasim_sdk._internal.alfacase.case_description import AlfasimVersionInfo
 from alfasim_sdk._internal.alfacase.case_description import CaseDescription
 from alfasim_sdk._internal.alfacase.case_description import CaseOutputDescription
 from alfasim_sdk._internal.alfacase.case_description import CasingDescription
 from alfasim_sdk._internal.alfacase.case_description import CasingSectionDescription
 from alfasim_sdk._internal.alfacase.case_description import CompositionDescription
 from alfasim_sdk._internal.alfacase.case_description import (
     CompressorEquipmentDescription,
@@ -46,15 +47,19 @@
 )
 from alfasim_sdk._internal.alfacase.case_description import CvTableDescription
 from alfasim_sdk._internal.alfacase.case_description import EnvironmentDescription
 from alfasim_sdk._internal.alfacase.case_description import (
     EnvironmentPropertyDescription,
 )
 from alfasim_sdk._internal.alfacase.case_description import EquipmentDescription
-from alfasim_sdk._internal.alfacase.case_description import FluidDescription
+from alfasim_sdk._internal.alfacase.case_description import AnnulusEquipmentDescription
+from alfasim_sdk._internal.alfacase.case_description import CombinedFluidDescription
+from alfasim_sdk._internal.alfacase.case_description import (
+    CompositionalFluidDescription,
+)
 from alfasim_sdk._internal.alfacase.case_description import FormationDescription
 from alfasim_sdk._internal.alfacase.case_description import FormationLayerDescription
 from alfasim_sdk._internal.alfacase.case_description import (
     GasLiftValveEquipmentDescription,
 )
 from alfasim_sdk._internal.alfacase.case_description import (
     HeatSourceEquipmentDescription,
@@ -79,54 +84,65 @@
 )
 from alfasim_sdk._internal.alfacase.case_description import (
     InitialVolumeFractionsDescription,
 )
 from alfasim_sdk._internal.alfacase.case_description import (
     InternalNodePropertiesDescription,
 )
+from alfasim_sdk._internal.alfacase.case_description import LeakEquipmentDescription
 from alfasim_sdk._internal.alfacase.case_description import (
     LengthAndElevationDescription,
 )
 from alfasim_sdk._internal.alfacase.case_description import LightComponentDescription
 from alfasim_sdk._internal.alfacase.case_description import LinearIPRDescription
+from alfasim_sdk._internal.alfacase.case_description import VogelIPRDescription
+from alfasim_sdk._internal.alfacase.case_description import FetkovichIPRDescription
+from alfasim_sdk._internal.alfacase.case_description import ForchheimerIPRDescription
 from alfasim_sdk._internal.alfacase.case_description import (
     MassSourceEquipmentDescription,
 )
 from alfasim_sdk._internal.alfacase.case_description import (
     MassSourceNodePropertiesDescription,
 )
 from alfasim_sdk._internal.alfacase.case_description import MaterialDescription
 from alfasim_sdk._internal.alfacase.case_description import NodeDescription
 from alfasim_sdk._internal.alfacase.case_description import (
     NumericalOptionsDescription,
 )
 from alfasim_sdk._internal.alfacase.case_description import OpenHoleDescription
-from alfasim_sdk._internal.alfacase.case_description import OpeningCurveDescription
 from alfasim_sdk._internal.alfacase.case_description import PackerDescription
 from alfasim_sdk._internal.alfacase.case_description import PhysicsDescription
+from alfasim_sdk._internal.alfacase.case_description import PigEquipmentDescription
 from alfasim_sdk._internal.alfacase.case_description import PipeDescription
 from alfasim_sdk._internal.alfacase.case_description import PipeSegmentsDescription
+from alfasim_sdk._internal.alfacase.case_description import PluginDescription
 from alfasim_sdk._internal.alfacase.case_description import (
     PressureContainerDescription,
 )
 from alfasim_sdk._internal.alfacase.case_description import (
     PressureNodePropertiesDescription,
 )
 from alfasim_sdk._internal.alfacase.case_description import ProfileDescription
 from alfasim_sdk._internal.alfacase.case_description import ProfileOutputDescription
 from alfasim_sdk._internal.alfacase.case_description import PumpEquipmentDescription
 from alfasim_sdk._internal.alfacase.case_description import (
     PvtModelCompositionalDescription,
 )
 from alfasim_sdk._internal.alfacase.case_description import (
+    PvtModelCombinedDescription,
+)
+from alfasim_sdk._internal.alfacase.case_description import (
     PvtModelCorrelationDescription,
 )
 from alfasim_sdk._internal.alfacase.case_description import PvtModelsDescription
 from alfasim_sdk._internal.alfacase.case_description import (
-    PvtModelTableParametersDescription,
+    PvtModelPtTableParametersDescription,
+)
+from alfasim_sdk._internal.alfacase.case_description import (
+    PvtModelPhTableParametersDescription,
 )
 from alfasim_sdk._internal.alfacase.case_description import (
     ReferencedPressureContainerDescription,
 )
 from alfasim_sdk._internal.alfacase.case_description import (
     ReferencedTemperaturesContainerDescription,
 )
@@ -142,107 +158,148 @@
 from alfasim_sdk._internal.alfacase.case_description import (
     ReservoirInflowEquipmentDescription,
 )
 from alfasim_sdk._internal.alfacase.case_description import (
     SeparatorNodePropertiesDescription,
 )
 from alfasim_sdk._internal.alfacase.case_description import SpeedCurveDescription
+from alfasim_sdk._internal.alfacase.case_description import (
+    SurgeVolumeOptionsDescription,
+)
 from alfasim_sdk._internal.alfacase.case_description import TableIPRDescription
 from alfasim_sdk._internal.alfacase.case_description import TablePumpDescription
 from alfasim_sdk._internal.alfacase.case_description import (
     TemperaturesContainerDescription,
 )
 from alfasim_sdk._internal.alfacase.case_description import TimeOptionsDescription
 from alfasim_sdk._internal.alfacase.case_description import (
     TracerModelConstantCoefficientsDescription,
 )
 from alfasim_sdk._internal.alfacase.case_description import TracersDescription
 from alfasim_sdk._internal.alfacase.case_description import (
     TracersMassFractionsContainerDescription,
 )
-from alfasim_sdk._internal.alfacase.case_description import TrendOutputDescription
+from alfasim_sdk._internal.alfacase.case_description import (
+    TrendsOutputDescription,
+    PositionalPipeTrendDescription,
+    OverallPipeTrendDescription,
+    GlobalTrendDescription,
+    EquipmentTrendDescription,
+    SeparatorTrendDescription,
+    ControllerTrendDescription,
+)
 from alfasim_sdk._internal.alfacase.case_description import TubingDescription
 from alfasim_sdk._internal.alfacase.case_description import ValveEquipmentDescription
 from alfasim_sdk._internal.alfacase.case_description import (
     VelocitiesContainerDescription,
 )
 from alfasim_sdk._internal.alfacase.case_description import (
     VolumeFractionsContainerDescription,
 )
 from alfasim_sdk._internal.alfacase.case_description import WallDescription
 from alfasim_sdk._internal.alfacase.case_description import WallLayerDescription
 from alfasim_sdk._internal.alfacase.case_description import WellDescription
 from alfasim_sdk._internal.alfacase.case_description import XAndYDescription
 
+from alfasim_sdk._internal.alfacase.case_description import (
+    ControllerNodePropertiesDescription,
+)
+from alfasim_sdk._internal.alfacase.case_description import (
+    ControllerInputSignalPropertiesDescription,
+    ControllerOutputSignalPropertiesDescription,
+)
+
 # ALFACase: Utilities
 from alfasim_sdk._internal.alfacase.alfacase import convert_alfacase_to_description
 from alfasim_sdk._internal.alfacase.alfacase import convert_description_to_alfacase
 from alfasim_sdk._internal.alfacase.alfacase import generate_alfacase_file
 from alfasim_sdk._internal.alfacase.alfatable import generate_alfatable_file
 from alfasim_sdk._internal.alfacase.alfatable import (
     load_pvt_model_table_parameters_description_from_alfatable,
 )
 
 # Constants
 from alfasim_sdk._internal.constants import BUBBLE_FIELD
 from alfasim_sdk._internal.constants import CompressorSpeedType
+from alfasim_sdk._internal.constants import ControllerType
+from alfasim_sdk._internal.constants import CorrelationsGasViscosity
+from alfasim_sdk._internal.constants import CorrelationsOilViscosity
 from alfasim_sdk._internal.constants import CorrelationPackage
 from alfasim_sdk._internal.constants import CorrelationPackageType
+from alfasim_sdk._internal.constants import CorrelationsSurfaceTension
 from alfasim_sdk._internal.constants import DEFAULT_TEMPERATURE_IN_K
+from alfasim_sdk._internal.constants import DrainageRateMode
 from alfasim_sdk._internal.constants import DROPLET_FIELD
-from alfasim_sdk._internal.constants import EXTRAS_REQUIRED_VERSION_KEY
 from alfasim_sdk._internal.constants import EmulsionModelType
+from alfasim_sdk._internal.constants import EmulsionRelativeViscosityModelType
+from alfasim_sdk._internal.constants import EmulsionDropletSizeModelType
+from alfasim_sdk._internal.constants import EmulsionInversionPointModelType
 from alfasim_sdk._internal.constants import EnergyModel
 from alfasim_sdk._internal.constants import EnergyModelPrimaryVariable
 from alfasim_sdk._internal.constants import EquationOfStateType
+from alfasim_sdk._internal.constants import EquipmentAttachmentLocation
 from alfasim_sdk._internal.constants import EvaluationStrategyType
+from alfasim_sdk._internal.constants import EXTRAS_REQUIRED_VERSION_KEY
+from alfasim_sdk._internal.constants import FlashModel
+from alfasim_sdk._internal.constants import FlowDirection
+from alfasim_sdk._internal.constants import FlowPatternModel
 from alfasim_sdk._internal.constants import FLUID_GAS
 from alfasim_sdk._internal.constants import FLUID_OIL
 from alfasim_sdk._internal.constants import FLUID_PHASE_NAMES
 from alfasim_sdk._internal.constants import FLUID_WATER
-from alfasim_sdk._internal.constants import FlashModel
-from alfasim_sdk._internal.constants import FlowDirection
 from alfasim_sdk._internal.constants import GAS_FIELD
 from alfasim_sdk._internal.constants import GAS_LAYER
 from alfasim_sdk._internal.constants import GAS_PHASE
+from alfasim_sdk._internal.constants import GasLiftValveOpeningType
 from alfasim_sdk._internal.constants import HydrodynamicModelType
 from alfasim_sdk._internal.constants import InitialConditionStrategyType
 from alfasim_sdk._internal.constants import InterpolationType
+from alfasim_sdk._internal.constants import LeakLocation
+from alfasim_sdk._internal.constants import LeakModel
+from alfasim_sdk._internal.constants import LeakType
 from alfasim_sdk._internal.constants import MassInflowSplitType
 from alfasim_sdk._internal.constants import MassSourceType
 from alfasim_sdk._internal.constants import MaterialType
+from alfasim_sdk._internal.constants import MultiInputType
 from alfasim_sdk._internal.constants import NodeCellType
 from alfasim_sdk._internal.constants import NonlinearSolverType
 from alfasim_sdk._internal.constants import OIL_FIELD
 from alfasim_sdk._internal.constants import OIL_LAYER
 from alfasim_sdk._internal.constants import OIL_PHASE
 from alfasim_sdk._internal.constants import OutputAttachmentLocation
-from alfasim_sdk._internal.constants import PVTCompositionalViscosityModel
+from alfasim_sdk._internal.constants import PigRoutingMode
+from alfasim_sdk._internal.constants import PigTrappingMode
 from alfasim_sdk._internal.constants import (
     PipeEnvironmentHeatTransferCoefficientModelType,
 )
 from alfasim_sdk._internal.constants import PipeThermalModelType
 from alfasim_sdk._internal.constants import PipeThermalPositionInput
 from alfasim_sdk._internal.constants import PumpType
-from alfasim_sdk._internal.constants import SOLID_PHASE
+from alfasim_sdk._internal.constants import PumpViscosityModel
+from alfasim_sdk._internal.constants import PumpThermalEfficiencyModel
+from alfasim_sdk._internal.constants import PVTCompositionalViscosityModel
 from alfasim_sdk._internal.constants import SeparatorGeometryType
 from alfasim_sdk._internal.constants import SimulationModeType
 from alfasim_sdk._internal.constants import SimulationRegimeType
+from alfasim_sdk._internal.constants import SOLID_PHASE
 from alfasim_sdk._internal.constants import SolidsModelType
 from alfasim_sdk._internal.constants import SurfaceTensionType
+from alfasim_sdk._internal.constants import SurgeVolumeTimeMode
 from alfasim_sdk._internal.constants import TableInputType
 from alfasim_sdk._internal.constants import TracerModelType
 from alfasim_sdk._internal.constants import ValveOpeningType
 from alfasim_sdk._internal.constants import ValveType
 from alfasim_sdk._internal.constants import WATER_DROPLET_IN_OIL_FIELD
 from alfasim_sdk._internal.constants import WATER_FIELD
 from alfasim_sdk._internal.constants import WATER_LAYER
 from alfasim_sdk._internal.constants import WATER_PHASE
 from alfasim_sdk._internal.constants import WellConnectionPort
 from alfasim_sdk._internal.constants import WellIndexPhaseType
+from alfasim_sdk._internal.constants import ForchheimerCoefficientsOption
+
 
 # Plugins: Layouts imports
 from alfasim_sdk._internal.layout import tab
 from alfasim_sdk._internal.layout import tabs
 from alfasim_sdk._internal.layout import group
 
 # Plugins: Models imports
@@ -261,14 +318,15 @@
 from alfasim_sdk._internal.types import UpdatePhase
 
 # Plugins: Types for configure_layers hook
 from alfasim_sdk._internal.types import AddLayer
 from alfasim_sdk._internal.types import UpdateLayer
 
 # Plugins: Types  for UI customization
+from alfasim_sdk._internal.types import BaseField
 from alfasim_sdk._internal.types import Boolean
 from alfasim_sdk._internal.types import Enum
 from alfasim_sdk._internal.types import FileContent
 from alfasim_sdk._internal.types import MultipleReference
 from alfasim_sdk._internal.types import Quantity
 from alfasim_sdk._internal.types import Reference
 from alfasim_sdk._internal.types import String
@@ -282,170 +340,213 @@
 # Plugins: Constants used on SecondaryVariable
 from alfasim_sdk._internal.variables import Visibility
 from alfasim_sdk._internal.variables import Scope
 from alfasim_sdk._internal.variables import Type
 from alfasim_sdk._internal.variables import Location
 
 __all__ = [
-    "console_main",
+    "AddField",
+    "AddLayer",
+    "AddPhase",
     "AnnulusDescription",
+    "AnnulusEquipmentDescription",
+    "BUBBLE_FIELD",
+    "BaseField",
     "BipDescription",
+    "Boolean",
+    "AlfasimVersionInfo",
     "CaseDescription",
     "CaseOutputDescription",
     "CasingDescription",
     "CasingSectionDescription",
     "CompositionDescription",
     "CompressorEquipmentDescription",
     "CompressorPressureTableDescription",
+    "CompressorSpeedType",
+    "ControllerInputSignalPropertiesDescription",
+    "ControllerNodePropertiesDescription",
+    "ControllerOutputSignalPropertiesDescription",
+    "ControllerTrendDescription",
+    "ControllerType",
+    "CorrelationPackage",
+    "CorrelationPackageType",
+    "CorrelationsOilViscosity",
+    "CorrelationsGasViscosity",
+    "CorrelationsSurfaceTension",
     "CvTableDescription",
+    "DEFAULT_TEMPERATURE_IN_K",
+    "DROPLET_FIELD",
+    "DrainageRateMode",
+    "EXTRAS_REQUIRED_VERSION_KEY",
+    "EmulsionModelType",
+    "EmulsionRelativeViscosityModelType",
+    "EmulsionDropletSizeModelType",
+    "EmulsionInversionPointModelType",
+    "EnergyModel",
+    "EnergyModelPrimaryVariable",
+    "Enum",
     "EnvironmentDescription",
     "EnvironmentPropertyDescription",
+    "EquationOfStateType",
+    "EquipmentAttachmentLocation",
     "EquipmentDescription",
-    "FluidDescription",
+    "EquipmentTrendDescription",
+    "ErrorMessage",
+    "EvaluationStrategyType",
+    "FLUID_GAS",
+    "FLUID_OIL",
+    "FLUID_PHASE_NAMES",
+    "FLUID_WATER",
+    "FileContent",
+    "FlashModel",
+    "FlowDirection",
+    "FlowPatternModel",
+    "ForchheimerIPRDescription",
+    "ForchheimerCoefficientsOption",
+    "CompositionalFluidDescription",
+    "CombinedFluidDescription",
     "FormationDescription",
     "FormationLayerDescription",
+    "GAS_FIELD",
+    "GAS_LAYER",
+    "GAS_PHASE",
     "GasLiftValveEquipmentDescription",
+    "GasLiftValveOpeningType",
+    "GlobalTrendDescription",
     "HeatSourceEquipmentDescription",
     "HeavyComponentDescription",
+    "HydrodynamicModelType",
     "IPRCurveDescription",
     "IPRModelsDescription",
+    "InitialConditionStrategyType",
     "InitialConditionsDescription",
     "InitialPressuresDescription",
     "InitialTemperaturesDescription",
     "InitialTracersMassFractionsDescription",
     "InitialVelocitiesDescription",
     "InitialVolumeFractionsDescription",
     "InternalNodePropertiesDescription",
+    "InterpolationType",
+    "LeakEquipmentDescription",
+    "LeakLocation",
+    "LeakModel",
+    "LeakType",
     "LengthAndElevationDescription",
     "LightComponentDescription",
     "LinearIPRDescription",
+    "Location",
+    "MassInflowSplitType",
     "MassSourceEquipmentDescription",
     "MassSourceNodePropertiesDescription",
+    "MassSourceType",
     "MaterialDescription",
+    "MaterialType",
+    "MultiInputType",
+    "MultipleReference",
+    "NodeCellType",
     "NodeDescription",
+    "NonlinearSolverType",
     "NumericalOptionsDescription",
+    "OIL_FIELD",
+    "OIL_LAYER",
+    "OIL_PHASE",
     "OpenHoleDescription",
-    "OpeningCurveDescription",
+    "OutputAttachmentLocation",
+    "OverallPipeTrendDescription",
+    "PVTCompositionalViscosityModel",
     "PackerDescription",
     "PhysicsDescription",
+    "PigEquipmentDescription",
+    "PigRoutingMode",
+    "PigTrappingMode",
     "PipeDescription",
+    "PipeEnvironmentHeatTransferCoefficientModelType",
     "PipeSegmentsDescription",
+    "PipeThermalModelType",
+    "PipeThermalPositionInput",
+    "PluginDescription",
+    "PositionalPipeTrendDescription",
     "PressureContainerDescription",
     "PressureNodePropertiesDescription",
     "ProfileDescription",
     "ProfileOutputDescription",
     "PumpEquipmentDescription",
+    "PumpType",
+    "PumpViscosityModel",
+    "PumpThermalEfficiencyModel",
+    "PvtModelCombinedDescription",
     "PvtModelCompositionalDescription",
     "PvtModelCorrelationDescription",
+    "PvtModelPtTableParametersDescription",
+    "PvtModelPhTableParametersDescription",
     "PvtModelsDescription",
-    "PvtModelTableParametersDescription",
+    "Quantity",
+    "Reference",
     "ReferencedPressureContainerDescription",
     "ReferencedTemperaturesContainerDescription",
     "ReferencedTracersMassFractionsContainerDescription",
     "ReferencedVelocitiesContainerDescription",
     "ReferencedVolumeFractionsContainerDescription",
     "ReservoirInflowEquipmentDescription",
+    "SOLID_PHASE",
+    "Scope",
+    "SecondaryVariable",
+    "SeparatorGeometryType",
     "SeparatorNodePropertiesDescription",
+    "SeparatorTrendDescription",
+    "SimulationModeType",
+    "SimulationRegimeType",
+    "SolidsModelType",
     "SpeedCurveDescription",
+    "String",
+    "SurfaceTensionType",
+    "SurgeVolumeOptionsDescription",
+    "SurgeVolumeTimeMode",
+    "Table",
+    "TableColumn",
     "TableIPRDescription",
+    "TableInputType",
     "TablePumpDescription",
     "TemperaturesContainerDescription",
     "TimeOptionsDescription",
     "TracerModelConstantCoefficientsDescription",
+    "TracerModelType",
+    "TracerType",
     "TracersDescription",
     "TracersMassFractionsContainerDescription",
-    "TrendOutputDescription",
+    "TrendsOutputDescription",
     "TubingDescription",
+    "Type",
+    "UpdateLayer",
+    "UpdatePhase",
+    "FetkovichIPRDescription",
     "ValveEquipmentDescription",
+    "ValveOpeningType",
+    "ValveType",
     "VelocitiesContainerDescription",
+    "Visibility",
+    "VogelIPRDescription",
     "VolumeFractionsContainerDescription",
+    "WATER_DROPLET_IN_OIL_FIELD",
+    "WATER_FIELD",
+    "WATER_LAYER",
+    "WATER_PHASE",
     "WallDescription",
     "WallLayerDescription",
+    "WarningMessage",
+    "WellConnectionPort",
     "WellDescription",
+    "WellIndexPhaseType",
     "XAndYDescription",
+    "console_main",
+    "container_model",
     "convert_alfacase_to_description",
     "convert_description_to_alfacase",
+    "data_model",
     "generate_alfacase_file",
     "generate_alfatable_file",
+    "get_metadata",
+    "group",
     "load_pvt_model_table_parameters_description_from_alfatable",
-    "BUBBLE_FIELD",
-    "CompressorSpeedType",
-    "CorrelationPackage",
-    "CorrelationPackageType",
-    "DEFAULT_TEMPERATURE_IN_K",
-    "DROPLET_FIELD",
-    "EXTRAS_REQUIRED_VERSION_KEY",
-    "EmulsionModelType",
-    "EnergyModel",
-    "EnergyModelPrimaryVariable",
-    "EquationOfStateType",
-    "EvaluationStrategyType",
-    "FLUID_GAS",
-    "FLUID_OIL",
-    "FLUID_PHASE_NAMES",
-    "FLUID_WATER",
-    "FlashModel",
-    "FlowDirection",
-    "GAS_FIELD",
-    "GAS_LAYER",
-    "GAS_PHASE",
-    "HydrodynamicModelType",
-    "InitialConditionStrategyType",
-    "InterpolationType",
-    "MassInflowSplitType",
-    "MassSourceType",
-    "MaterialType",
-    "NodeCellType",
-    "NonlinearSolverType",
-    "OIL_FIELD",
-    "OIL_LAYER",
-    "OIL_PHASE",
-    "OutputAttachmentLocation",
-    "PVTCompositionalViscosityModel",
-    "PipeEnvironmentHeatTransferCoefficientModelType",
-    "PipeThermalModelType",
-    "PipeThermalPositionInput",
-    "PumpType",
-    "SOLID_PHASE",
-    "SeparatorGeometryType",
-    "SimulationModeType",
-    "SimulationRegimeType",
-    "SolidsModelType",
-    "SurfaceTensionType",
-    "TableInputType",
-    "TracerModelType",
-    "ValveOpeningType",
-    "ValveType",
-    "WATER_DROPLET_IN_OIL_FIELD",
-    "WATER_FIELD",
-    "WATER_LAYER",
-    "WATER_PHASE",
-    "WellConnectionPort",
-    "WellIndexPhaseType",
     "tab",
     "tabs",
-    "group",
-    "container_model",
-    "data_model",
-    "WarningMessage",
-    "ErrorMessage",
-    "AddField",
-    "AddPhase",
-    "UpdatePhase",
-    "AddLayer",
-    "UpdateLayer",
-    "Boolean",
-    "Enum",
-    "FileContent",
-    "MultipleReference",
-    "Quantity",
-    "Reference",
-    "String",
-    "Table",
-    "TableColumn",
-    "TracerType",
-    "SecondaryVariable",
-    "Visibility",
-    "Scope",
-    "Type",
-    "Location",
 ]
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk.egg-info/SOURCES.txt` & `alfasim_sdk-2024.1/src/alfasim_sdk.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-AUTHORS.rst
+CHANGELOG.rst
 CONTRIBUTING.rst
-HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
 RELEASING.rst
 pyproject.toml
 setup.cfg
 setup.py
 src/alfasim_sdk/__init__.py
+src/alfasim_sdk/default_tasks.py
 src/alfasim_sdk.egg-info/PKG-INFO
 src/alfasim_sdk.egg-info/SOURCES.txt
 src/alfasim_sdk.egg-info/dependency_links.txt
 src/alfasim_sdk.egg-info/entry_points.txt
 src/alfasim_sdk.egg-info/not-zip-safe
 src/alfasim_sdk.egg-info/requires.txt
 src/alfasim_sdk.egg-info/top_level.txt
@@ -36,14 +36,28 @@
 src/alfasim_sdk/_internal/alfacase/alfacase_to_case.py
 src/alfasim_sdk/_internal/alfacase/alfatable.py
 src/alfasim_sdk/_internal/alfacase/case_description.py
 src/alfasim_sdk/_internal/alfacase/case_description_attributes.py
 src/alfasim_sdk/_internal/alfacase/case_to_alfacase.py
 src/alfasim_sdk/_internal/alfacase/generate_case_description_docstring.py
 src/alfasim_sdk/_internal/alfacase/generate_schema.py
+src/alfasim_sdk/_internal/alfacase/plugin_alfacase_to_case.py
+src/alfasim_sdk/_internal/alfacase/plugin_introspection.py
 src/alfasim_sdk/_internal/alfacase/schema.py
 src/alfasim_sdk/alfasim_sdk_api/alfasim_sdk.h
 src/alfasim_sdk/alfasim_sdk_api/api.h
 src/alfasim_sdk/alfasim_sdk_api/common.h
 src/alfasim_sdk/alfasim_sdk_api/detail/api_pointers.h
 src/alfasim_sdk/alfasim_sdk_api/detail/bootstrap_linux.h
-src/alfasim_sdk/alfasim_sdk_api/detail/bootstrap_win.h
+src/alfasim_sdk/alfasim_sdk_api/detail/bootstrap_win.h
+src/alfasim_sdk/result_reader/__init__.py
+src/alfasim_sdk/result_reader/aggregator.py
+src/alfasim_sdk/result_reader/aggregator_constants.py
+src/alfasim_sdk/result_reader/reader.py
+src/alfasim_sdk/testing/__init__.py
+src/alfasim_sdk/testing/fixtures.py
+src/alfasim_sdk_plugins/__init__.py
+tests/test_alfasim_sdk_utils.py
+tests/test_case_builders.py
+tests/test_cli.py
+tests/test_hook_specs.py
+tests/test_invoke.py
```

### Comparing `alfasim_sdk-0.9.0/src/alfasim_sdk.egg-info/PKG-INFO` & `alfasim_sdk-2024.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,70 @@
 Metadata-Version: 2.1
-Name: alfasim-sdk
-Version: 0.9.0
+Name: alfasim_sdk
+Version: 2024.1
 Summary: ALFAsim API/SDK
 Home-page: https://github.com/esss/alfasim-sdk
 Author: ESSS
 Author-email: foss@esss.co
-License: UNKNOWN
-Description: ===========
-        alfasim-sdk
-        ===========
-        
-        
-        .. image:: https://img.shields.io/pypi/v/alfasim-sdk.svg
-                :target: https://pypi.python.org/pypi/alfasim-sdk
-        
-        .. image:: https://github.com/ESSS/alfasim-sdk/workflows/ALFAsim%20SDK/badge.svg
-            :target: https://github.com/ESSS/alfasim-sdk/actions?query=workflow%3A%22ALFAsim+SDK%22
-        
-        .. image:: https://codecov.io/gh/ESSS/alfasim-sdk/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/ESSS/alfasim-sdk
-        
-        .. image:: https://readthedocs.org/projects/alfasim-sdk/badge/?version=latest
-            :target: https://alfasim-sdk.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-            :target: https://github.com/python/black
-        
-        
-        
-        
-        ALFAsim API/SDK
-        
-        
-        * Free software: MIT license
-        * Documentation: https://alfasim-sdk.readthedocs.io.
-        
-        
-        Features
-        --------
-        
-        * TODO
-        
-        Credits
-        -------
-        
-        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: python-hookman
+Requires-Dist: typing_inspect
+Requires-Dist: strictyaml>=1.4.3
+Requires-Dist: boltons
+Requires-Dist: Click>=7.0
+Requires-Dist: barril<2.0,>=1.13
+Requires-Dist: pluggy>=0.13.0
+Requires-Dist: h5py
+
+===========
+alfasim-sdk
+===========
+
+
+.. image:: https://img.shields.io/pypi/v/alfasim-sdk.svg
+        :target: https://pypi.python.org/pypi/alfasim-sdk
+
+.. image:: https://github.com/ESSS/alfasim-sdk/workflows/ALFAsim%20SDK/badge.svg
+    :target: https://github.com/ESSS/alfasim-sdk/actions?query=workflow%3A%22ALFAsim+SDK%22
+
+.. image:: https://codecov.io/gh/ESSS/alfasim-sdk/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/ESSS/alfasim-sdk
+
+.. image:: https://readthedocs.org/projects/alfasim-sdk/badge/?version=latest
+    :target: https://alfasim-sdk.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/python/black
+
+.. image:: https://sonarcloud.io/api/project_badges/measure?project=ESSS_alfasim-sdk&metric=alert_status
+    :target: https://sonarcloud.io/project/overview?id=ESSS_alfasim-sdk
+
+
+
+ALFAsim API/SDK
+
+
+* Free software: MIT license
+* Documentation: https://alfasim-sdk.readthedocs.io.
+
+
+Features
+--------
+
+* TODO
+
+Credits
+-------
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
```

### Comparing `alfasim_sdk-0.9.0/README.rst` & `alfasim_sdk-2024.1/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 .. image:: https://readthedocs.org/projects/alfasim-sdk/badge/?version=latest
     :target: https://alfasim-sdk.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/python/black
 
+.. image:: https://sonarcloud.io/api/project_badges/measure?project=ESSS_alfasim-sdk&metric=alert_status
+    :target: https://sonarcloud.io/project/overview?id=ESSS_alfasim-sdk
 
 
 
 ALFAsim API/SDK
 
 
 * Free software: MIT license
```

### Comparing `alfasim_sdk-0.9.0/RELEASING.rst` & `alfasim_sdk-2024.1/RELEASING.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 =========
 Releasing
 =========
 
-When releasing a new branch should be created to update the release date for the version in ``HISTORY.str``.
+When releasing a new branch should be created to update the release date for the version in ``CHANGELOG.str``.
 
 The version being released is listed in https://github.com/ESSS/alfasim-sdk/blob/master/src/alfasim_sdk/_internal/version.py, if needed this value should be changed to match accordingly.
 
 Any other required changes related to the release should also be included in the same branch.
 
 When all changes are ready the branch should be tagged ``v<release-number>`` and merged.
 
-After released it is advisable to update https://github.com/ESSS/alfasim-sdk/blob/master/src/alfasim_sdk/_internal/version.py with the next release version (increase minor version, for example ``0.6.0`` to ``0.7.0``) and ``HISTORY.rst`` to add a section to next unreleased version.
+After released, update `version.py <src/alfasim_sdk/_internal/version.py>`__ with the next release version planned for ALFAsim and add a new *unreleased* section to the ``CHANGELOG.rst``. Note that this version number appears on ALFAsim's About window, so should be done **before** the next ALFAsim planned release.
```

### Comparing `alfasim_sdk-0.9.0/PKG-INFO` & `alfasim_sdk-2024.1/src/alfasim_sdk.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,70 @@
 Metadata-Version: 2.1
 Name: alfasim_sdk
-Version: 0.9.0
+Version: 2024.1
 Summary: ALFAsim API/SDK
 Home-page: https://github.com/esss/alfasim-sdk
 Author: ESSS
 Author-email: foss@esss.co
-License: UNKNOWN
-Description: ===========
-        alfasim-sdk
-        ===========
-        
-        
-        .. image:: https://img.shields.io/pypi/v/alfasim-sdk.svg
-                :target: https://pypi.python.org/pypi/alfasim-sdk
-        
-        .. image:: https://github.com/ESSS/alfasim-sdk/workflows/ALFAsim%20SDK/badge.svg
-            :target: https://github.com/ESSS/alfasim-sdk/actions?query=workflow%3A%22ALFAsim+SDK%22
-        
-        .. image:: https://codecov.io/gh/ESSS/alfasim-sdk/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/ESSS/alfasim-sdk
-        
-        .. image:: https://readthedocs.org/projects/alfasim-sdk/badge/?version=latest
-            :target: https://alfasim-sdk.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-            :target: https://github.com/python/black
-        
-        
-        
-        
-        ALFAsim API/SDK
-        
-        
-        * Free software: MIT license
-        * Documentation: https://alfasim-sdk.readthedocs.io.
-        
-        
-        Features
-        --------
-        
-        * TODO
-        
-        Credits
-        -------
-        
-        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: python-hookman
+Requires-Dist: typing_inspect
+Requires-Dist: strictyaml>=1.4.3
+Requires-Dist: boltons
+Requires-Dist: Click>=7.0
+Requires-Dist: barril<2.0,>=1.13
+Requires-Dist: pluggy>=0.13.0
+Requires-Dist: h5py
+
+===========
+alfasim-sdk
+===========
+
+
+.. image:: https://img.shields.io/pypi/v/alfasim-sdk.svg
+        :target: https://pypi.python.org/pypi/alfasim-sdk
+
+.. image:: https://github.com/ESSS/alfasim-sdk/workflows/ALFAsim%20SDK/badge.svg
+    :target: https://github.com/ESSS/alfasim-sdk/actions?query=workflow%3A%22ALFAsim+SDK%22
+
+.. image:: https://codecov.io/gh/ESSS/alfasim-sdk/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/ESSS/alfasim-sdk
+
+.. image:: https://readthedocs.org/projects/alfasim-sdk/badge/?version=latest
+    :target: https://alfasim-sdk.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/python/black
+
+.. image:: https://sonarcloud.io/api/project_badges/measure?project=ESSS_alfasim-sdk&metric=alert_status
+    :target: https://sonarcloud.io/project/overview?id=ESSS_alfasim-sdk
+
+
+
+ALFAsim API/SDK
+
+
+* Free software: MIT license
+* Documentation: https://alfasim-sdk.readthedocs.io.
+
+
+Features
+--------
+
+* TODO
+
+Credits
+-------
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
```

