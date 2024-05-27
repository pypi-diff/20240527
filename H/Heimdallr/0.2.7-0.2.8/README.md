# Comparing `tmp/Heimdallr-0.2.7.tar.gz` & `tmp/heimdallr-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Heimdallr-0.2.7.tar", last modified: Wed Aug 24 08:05:15 2022, max compression
+gzip compressed data, was "heimdallr-0.2.8.tar", last modified: Mon May 27 09:04:18 2024, max compression
```

## Comparing `Heimdallr-0.2.7.tar` & `heimdallr-0.2.8.tar`

### file list

```diff
@@ -1,70 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 08:05:15.854451 Heimdallr-0.2.7/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 08:05:15.830451 Heimdallr-0.2.7/Heimdallr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2199 2022-08-24 08:05:15.000000 Heimdallr-0.2.7/Heimdallr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1837 2022-08-24 08:05:15.000000 Heimdallr-0.2.7/Heimdallr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-08-24 08:05:15.000000 Heimdallr-0.2.7/Heimdallr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      224 2022-08-24 08:05:15.000000 Heimdallr-0.2.7/Heimdallr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1215 2022-08-24 08:05:15.000000 Heimdallr-0.2.7/Heimdallr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       27 2022-08-24 08:05:15.000000 Heimdallr-0.2.7/Heimdallr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)    10455 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (116)     2199 2022-08-24 08:05:15.854451 Heimdallr-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      903 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 08:05:15.830451 Heimdallr-0.2.7/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (116)       88 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 08:05:15.830451 Heimdallr-0.2.7/heimdallr/
--rw-r--r--   0 runner    (1001) docker     (116)     3699 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 08:05:15.830451 Heimdallr-0.2.7/heimdallr/configuration/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1747 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/configuration/heimdallr_config.py
--rw-r--r--   0 runner    (1001) docker     (116)    14416 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/configuration/heimdallr_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 08:05:15.834451 Heimdallr-0.2.7/heimdallr/entry_points/
--rw-r--r--   0 runner    (1001) docker     (116)      118 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8417 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/entry_points/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 08:05:15.834451 Heimdallr-0.2.7/heimdallr/entry_points/deprecated/
--rw-r--r--   0 runner    (1001) docker     (116)      152 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/entry_points/deprecated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2714 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/entry_points/deprecated/publisher_non_sch.py
--rw-r--r--   0 runner    (1001) docker     (116)     3179 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/entry_points/publisher.py
--rw-r--r--   0 runner    (1001) docker     (116)     1275 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/entry_points/repl.py
--rw-r--r--   0 runner    (1001) docker     (116)    10366 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/entry_points/server.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 08:05:15.838451 Heimdallr-0.2.7/heimdallr/server/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 08:05:15.838451 Heimdallr-0.2.7/heimdallr/server/board_layout/
--rw-r--r--   0 runner    (1001) docker     (116)      213 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/server/board_layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2244 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/server/board_layout/body.py
--rw-r--r--   0 runner    (1001) docker     (116)      817 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/server/board_layout/footer.py
--rw-r--r--   0 runner    (1001) docker     (116)     1895 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/server/board_layout/header.py
--rw-r--r--   0 runner    (1001) docker     (116)     3127 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/server/board_layout/menu.py
--rw-r--r--   0 runner    (1001) docker     (116)      490 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/server/board_layout/root_layout.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 08:05:15.838451 Heimdallr-0.2.7/heimdallr/utilities/
--rw-r--r--   0 runner    (1001) docker     (116)      128 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      522 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/utilities/date_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 08:05:15.842451 Heimdallr-0.2.7/heimdallr/utilities/nvidia/
--rw-r--r--   0 runner    (1001) docker     (116)      152 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/utilities/nvidia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    69780 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/utilities/nvidia/bindings.py
--rw-r--r--   0 runner    (1001) docker     (116)     2956 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/utilities/nvidia/packing.py
--rw-r--r--   0 runner    (1001) docker     (116)   145969 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/utilities/nvidia/smi_parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 08:05:15.846451 Heimdallr-0.2.7/heimdallr/utilities/publisher/
--rw-r--r--   0 runner    (1001) docker     (116)      490 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/utilities/publisher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/utilities/publisher/system_resources.py
--rw-r--r--   0 runner    (1001) docker     (116)      993 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/utilities/publisher/unpacking.py
--rw-r--r--   0 runner    (1001) docker     (116)     1167 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/utilities/publisher/windows_task_scheduler_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 08:05:15.850451 Heimdallr-0.2.7/heimdallr/utilities/server/
--rw-r--r--   0 runner    (1001) docker     (116)      198 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/utilities/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1608 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/utilities/server/du_utilities.py
--rw-r--r--   0 runner    (1001) docker     (116)     5953 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/utilities/server/github_org_generators.py
--rw-r--r--   0 runner    (1001) docker     (116)     3810 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/utilities/server/google_calendar.py
--rw-r--r--   0 runner    (1001) docker     (116)     4273 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/utilities/server/gpu_utilities.py
--rw-r--r--   0 runner    (1001) docker     (116)     2803 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/heimdallr/utilities/server/teams_status.py
--rw-r--r--   0 runner    (1001) docker     (116)      230 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      134 2022-08-24 08:05:15.854451 Heimdallr-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     7721 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 08:05:15.854451 Heimdallr-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (116)       88 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 08:05:15.854451 Heimdallr-0.2.7/tests/lab_board/
--rw-r--r--   0 runner    (1001) docker     (116)      118 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/tests/lab_board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      118 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/tests/lab_board/test_lab_board.py
--rw-r--r--   0 runner    (1001) docker     (116)     1621 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/tests/req_unit_test.py
--rw-r--r--   0 runner    (1001) docker     (116)      172 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (116)    15234 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/tests/test_nvml.py
--rw-r--r--   0 runner    (1001) docker     (116)      493 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/tests/test_sanity.py
--rw-r--r--   0 runner    (1001) docker     (116)     2258 2022-08-24 08:03:28.000000 Heimdallr-0.2.7/tests/test_smi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:04:18.938463 heimdallr-0.2.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:04:18.930463 heimdallr-0.2.8/Heimdallr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-27 09:04:18.000000 heimdallr-0.2.8/Heimdallr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-27 09:04:18.000000 heimdallr-0.2.8/Heimdallr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 09:04:18.000000 heimdallr-0.2.8/Heimdallr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-27 09:04:18.000000 heimdallr-0.2.8/Heimdallr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-27 09:04:18.000000 heimdallr-0.2.8/Heimdallr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 09:04:18.000000 heimdallr-0.2.8/Heimdallr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-05-27 09:01:55.000000 heimdallr-0.2.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-27 09:04:18.938463 heimdallr-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-27 09:01:55.000000 heimdallr-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:04:18.922463 heimdallr-0.2.8/heimdallr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:04:18.922463 heimdallr-0.2.8/heimdallr/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/configuration/heimdallr_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14400 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/configuration/heimdallr_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:04:18.922463 heimdallr-0.2.8/heimdallr/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/entry_points/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:04:18.922463 heimdallr-0.2.8/heimdallr/entry_points/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/entry_points/deprecated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/entry_points/deprecated/publisher_non_sch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/entry_points/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/entry_points/repl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/entry_points/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:04:18.922463 heimdallr-0.2.8/heimdallr/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:04:18.926463 heimdallr-0.2.8/heimdallr/server/board_layout/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/server/board_layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/server/board_layout/body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/server/board_layout/footer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/server/board_layout/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/server/board_layout/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/server/board_layout/root_layout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:04:18.926463 heimdallr-0.2.8/heimdallr/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/utilities/date_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:04:18.926463 heimdallr-0.2.8/heimdallr/utilities/nvidia/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/utilities/nvidia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71186 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/utilities/nvidia/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/utilities/nvidia/packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)   146246 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/utilities/nvidia/smi_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:04:18.926463 heimdallr-0.2.8/heimdallr/utilities/publisher/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/utilities/publisher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/utilities/publisher/system_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/utilities/publisher/unpacking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/utilities/publisher/windows_task_scheduler_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:04:18.930463 heimdallr-0.2.8/heimdallr/utilities/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/utilities/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/utilities/server/du_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/utilities/server/github_org_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/utilities/server/google_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/utilities/server/gpu_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/utilities/server/meet_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/utilities/server/slack_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-27 09:01:55.000000 heimdallr-0.2.8/heimdallr/utilities/server/teams_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-27 09:01:55.000000 heimdallr-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-27 09:04:18.938463 heimdallr-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-05-27 09:01:55.000000 heimdallr-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:04:18.930463 heimdallr-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-27 09:01:55.000000 heimdallr-0.2.8/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16600 2024-05-27 09:01:55.000000 heimdallr-0.2.8/tests/test_nvml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-27 09:01:55.000000 heimdallr-0.2.8/tests/test_sanity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-27 09:01:55.000000 heimdallr-0.2.8/tests/test_smi.py
```

### Comparing `Heimdallr-0.2.7/Heimdallr.egg-info/SOURCES.txt` & `heimdallr-0.2.8/Heimdallr.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 setup.py
 Heimdallr.egg-info/PKG-INFO
 Heimdallr.egg-info/SOURCES.txt
 Heimdallr.egg-info/dependency_links.txt
 Heimdallr.egg-info/entry_points.txt
 Heimdallr.egg-info/requires.txt
 Heimdallr.egg-info/top_level.txt
-benchmarks/__init__.py
 heimdallr/__init__.py
 heimdallr/configuration/__init__.py
 heimdallr/configuration/heimdallr_config.py
 heimdallr/configuration/heimdallr_settings.py
 heimdallr/entry_points/__init__.py
 heimdallr/entry_points/cli.py
 heimdallr/entry_points/publisher.py
@@ -39,16 +38,14 @@
 heimdallr/utilities/publisher/unpacking.py
 heimdallr/utilities/publisher/windows_task_scheduler_utilities.py
 heimdallr/utilities/server/__init__.py
 heimdallr/utilities/server/du_utilities.py
 heimdallr/utilities/server/github_org_generators.py
 heimdallr/utilities/server/google_calendar.py
 heimdallr/utilities/server/gpu_utilities.py
+heimdallr/utilities/server/meet_status.py
+heimdallr/utilities/server/slack_status.py
 heimdallr/utilities/server/teams_status.py
-tests/__init__.py
-tests/req_unit_test.py
 tests/test_import.py
 tests/test_nvml.py
 tests/test_sanity.py
-tests/test_smi.py
-tests/lab_board/__init__.py
-tests/lab_board/test_lab_board.py
+tests/test_smi.py
```

### Comparing `Heimdallr-0.2.7/LICENSE.md` & `heimdallr-0.2.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Heimdallr-0.2.7/README.md` & `heimdallr-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `Heimdallr-0.2.7/heimdallr/configuration/heimdallr_config.py` & `heimdallr-0.2.8/heimdallr/configuration/heimdallr_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 __author__ = "Christian Heider Nielsen"
-__doc__ = ""
+__doc__ = """ description """
 
 import os
 
 from warg import NOD
 
 SERVER_ADDRESS = "localhost"
 SERVER_PORT = int(os.environ.get("PORT", 5555))
```

### Comparing `Heimdallr-0.2.7/heimdallr/configuration/heimdallr_settings.py` & `heimdallr-0.2.8/heimdallr/configuration/heimdallr_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,53 +10,52 @@
 import getpass
 import inspect
 import os
 import shelve
 from enum import Enum
 from typing import Union
 
-from warg.os_platform import is_nix
-
-if is_nix():
-    try:
-        import sh
-    except (ImportError, ModuleNotFoundError) as e:
-        print(e)
-        print("Please install sh and dependencies")
-
 from sorcery import assigned_names
+from warg import PropertySettings, is_windows
+from warg import ensure_existence
+from warg import is_nix
 
-from apppath import ensure_existence
 from heimdallr import PROJECT_APP_PATH
-from warg import PropertySettings, is_windows
 
 __all__ = [
     "HeimdallrSettings",  # Setting Class
     "SettingScopeEnum",  # Setting scope Enum
     "set_all_heimdallr_settings",  # Set settings function
 ]
 
+if is_nix():
+    try:
+        import sh
+    except (ImportError, ModuleNotFoundError) as e:
+        print(e)
+        print("Please install sh and dependencies")
+
 
 # PropertySettings.raise_exception_on_none = False
 
 
 class SettingScopeEnum(Enum):
-    """ """
+    """description"""
 
     user, site, root = assigned_names()
 
 
 class EnvironmentVariablePreference(Enum):
-    """ """
+    """description"""
 
     prefer, if_missing, ignore = assigned_names()
 
 
 class HeimdallrSettings(PropertySettings):
-    """ """
+    """description"""
 
     _setting_scope = None
     _google_settings_path = None
     _mqtt_settings_path = None
     _github_settings_path = None
     _credentials_base_path = None
     _teams_settings_path = None
@@ -108,15 +107,15 @@
         HeimdallrSettings._github_settings_path = ensure_existence(
             p / "github.settings"
         )
         HeimdallrSettings._teams_settings_path = ensure_existence(p / "teams.settings")
 
     @property
     def teams_config(self) -> Union[object, dict, None]:
-        """ """
+        """description"""
         key = inspect.currentframe().f_code.co_name
         if (
             self._look_up_env_on_missing == EnvironmentVariablePreference.prefer
             and key in os.environ
         ):
             return os.environ.get(key)
         with shelve.open(str(HeimdallrSettings._teams_settings_path)) as d:
@@ -143,15 +142,15 @@
         with shelve.open(
             str(HeimdallrSettings._teams_settings_path), writeback=True
         ) as d:
             d[key] = config
 
     @property
     def google_calendar_id(self) -> Union[object, str, None]:
-        """ """
+        """description"""
         key = inspect.currentframe().f_code.co_name
         if (
             self._look_up_env_on_missing == EnvironmentVariablePreference.prefer
             and key in os.environ
         ):
             return os.environ.get(key)
         with shelve.open(str(HeimdallrSettings._google_settings_path)) as d:
@@ -180,29 +179,26 @@
         ) as d:
             d[key] = calendar_id
 
     @google_calendar_id.deleter
     def google_calendar_id(self) -> None:
         """
 
-        Args:
-            calendar_id ():
-
-        Returns:
-
+        :return:
+        :rtype:
         """
         key = inspect.currentframe().f_code.co_name
         with shelve.open(
             str(HeimdallrSettings._github_settings_path), writeback=True
         ) as d:
             del d[key]
 
     @property
     def github_token(self) -> Union[object, str, None]:
-        """ """
+        """description"""
         key = inspect.currentframe().f_code.co_name
         if (
             self._look_up_env_on_missing == EnvironmentVariablePreference.prefer
             and key in os.environ
         ):
             return os.environ.get(key)
         with shelve.open(str(HeimdallrSettings._github_settings_path)) as d:
@@ -231,50 +227,47 @@
         ) as d:
             d[key] = calendar_id
 
     @github_token.deleter
     def github_token(self) -> None:
         """
 
-        Args:
-            calendar_id ():
-
-        Returns:
-
+        :return:
+        :rtype:
         """
         key = inspect.currentframe().f_code.co_name
         with shelve.open(
             str(HeimdallrSettings._github_settings_path), writeback=True
         ) as d:
             del d[key]
 
     '''
 @property
 def mqtt_access_token(self) -> Optional[str]:
-  """ """
-  key = inspect.currentframe().f_code.co_name
-  if self._look_up_env_on_missing == EnvironmentVariablePreference.prefer and key in os.environ:
-          return os.environ.get(key)
-  with shelve.open(str(HeimdallrSettings._mqtt_settings_path)) as d:
-      if key in d:
-          return d[key]
-  if self._look_up_env_on_missing == EnvironmentVariablePreference.if_missing and key in os.environ:
-      return os.environ.get(key)
-  return None
+""" description """
+key = inspect.currentframe().f_code.co_name
+if self._look_up_env_on_missing == EnvironmentVariablePreference.prefer and key in os.environ:
+  return os.environ.get(key)
+with shelve.open(str(HeimdallrSettings._mqtt_settings_path)) as d:
+if key in d:
+  return d[key]
+if self._look_up_env_on_missing == EnvironmentVariablePreference.if_missing and key in os.environ:
+return os.environ.get(key)
+return None
 
 @mqtt_access_token.setter
 def mqtt_access_token(self, token: str) -> None:
-  key = inspect.currentframe().f_code.co_name
-  with shelve.open(str(HeimdallrSettings._mqtt_settings_path), writeback=True) as d:
-      d[key] = token
+key = inspect.currentframe().f_code.co_name
+with shelve.open(str(HeimdallrSettings._mqtt_settings_path), writeback=True) as d:
+d[key] = token
 '''
 
     @property
     def mqtt_username(self) -> Union[object, str, None]:
-        """ """
+        """description"""
         key = inspect.currentframe().f_code.co_name
         if (
             self._look_up_env_on_missing == EnvironmentVariablePreference.prefer
             and key in os.environ
         ):
             return os.environ.get(key)
         with shelve.open(str(HeimdallrSettings._mqtt_settings_path)) as d:
@@ -314,15 +307,15 @@
         with shelve.open(
             str(HeimdallrSettings._mqtt_settings_path), writeback=True
         ) as d:
             del d[key]
 
     @property
     def mqtt_password(self) -> Union[object, str, None]:
-        """ """
+        """description"""
         key = inspect.currentframe().f_code.co_name
         if (
             self._look_up_env_on_missing == EnvironmentVariablePreference.prefer
             and key in os.environ
         ):
             return os.environ.get(key)
         with shelve.open(str(HeimdallrSettings._mqtt_settings_path)) as d:
@@ -362,15 +355,15 @@
         with shelve.open(
             str(HeimdallrSettings._mqtt_settings_path), writeback=True
         ) as d:
             del d[key]
 
     @property
     def mqtt_broker(self) -> Union[object, str, None]:
-        """ """
+        """description"""
         key = inspect.currentframe().f_code.co_name
         if (
             self._look_up_env_on_missing == EnvironmentVariablePreference.prefer
             and key in os.environ
         ):
             return os.environ.get(key)
         with shelve.open(str(HeimdallrSettings._mqtt_settings_path)) as d:
@@ -410,15 +403,15 @@
         with shelve.open(
             str(HeimdallrSettings._mqtt_settings_path), writeback=True
         ) as d:
             del d[key]
 
     @property
     def mqtt_port(self) -> Union[object, str, None]:
-        """ """
+        """description"""
         key = inspect.currentframe().f_code.co_name
         if (
             self._look_up_env_on_missing == EnvironmentVariablePreference.prefer
             and key in os.environ
         ):
             return os.environ.get(key)
         with shelve.open(str(HeimdallrSettings._mqtt_settings_path)) as d:
@@ -463,38 +456,38 @@
 
 def set_all_heimdallr_settings(
     setting_scope: SettingScopeEnum = SettingScopeEnum.user,
     *,
     _lower_keys: bool = True,
     **kwargs,
 ):
-    """ """
-    HEIMDALLR_SETTINGS = HeimdallrSettings(setting_scope)
-    # print(f"current heimdallr settings: {HEIMDALLR_SETTINGS}")
+    """description"""
+    heimdallr_settings = HeimdallrSettings(setting_scope)
+    # print(f"current heimdallr settings: {heimdallr_settings}")
     if _lower_keys:
         kwargs = {k.lower(): v for k, v in kwargs.items()}
 
     # for k in kwargs.keys():
-    #    assert k in HEIMDALLR_SETTINGS, f'"{k}" is not in Heimdallrs settings'
+    #    assert k in heimdallr_settings, f'"{k}" is not in Heimdallrs settings'
 
-    for k in HEIMDALLR_SETTINGS:
+    for k in heimdallr_settings:
         assert k in kwargs.keys(), f'Missing "{k}" from kwargs'
 
-    HEIMDALLR_SETTINGS.__from_dict__(kwargs)
+    heimdallr_settings.__from_dict__(kwargs)
 
     print(f"new heimdallr settings: {HeimdallrSettings()}")
 
 
 if __name__ == "__main__":
     settings = HeimdallrSettings()
 
     for k in settings:
         print(k, settings[k])
 
     """
 set_all_heimdallr_settings(
-  **{
-      k: getattr(settings, k) if getattr(settings, k) else None
-      for k in iter(settings)
-  }
+**{
+k: getattr(settings, k) if getattr(settings, k) else None
+for k in iter(settings)
+}
 )
 """
```

### Comparing `Heimdallr-0.2.7/heimdallr/entry_points/cli.py` & `heimdallr-0.2.8/heimdallr/entry_points/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,35 +9,37 @@
 
 from enum import Enum
 from functools import partial
 from pathlib import Path
 from typing import Any
 
 import fire
-from draugr.python_utilities import get_terminal_size
-from pyfiglet import Figlet
-from sorcery import assigned_names
-
-from heimdallr import get_version
+import warg
 from heimdallr.configuration.heimdallr_settings import (
     HeimdallrSettings,
     SettingScopeEnum,
 )
+from pyfiglet import Figlet
+from sorcery import assigned_names
+
+from heimdallr import get_version
 
 margin_percentage = 0 / 6
-terminal_width = get_terminal_size().columns
+terminal_width = warg.get_terminal_size().columns
 margin = int(margin_percentage * terminal_width)
 width = terminal_width - 2 * margin
 underline = "_" * width
 indent = " " * margin
 sponsors = "Alexandra Institute"
 
+__all__ = []
+
 
 class ServiceOption(Enum):
-    """ """
+    """description"""
 
     (
         install,
         remove,
         uninstall,
         disable,
         enable,
@@ -45,21 +47,21 @@
         stop,
         restart,
         status,
     ) = assigned_names()  # same
 
 
 class HeimdallrMode(Enum):
-    """ """
+    """description"""
 
     server, publisher = assigned_names()
 
 
 class HeimdallrCLI:
-    """ """
+    """description"""
 
     def __init__(self, *, setting_scope: SettingScopeEnum = SettingScopeEnum.user):
         try:
             self.setting_scope = SettingScopeEnum(setting_scope)
         except ValueError as a:
             print(f"Valid options {list(SettingScopeEnum.__iter__())}")
             raise a
@@ -84,15 +86,15 @@
         self,
         setting: str,
         value: Any,
     ) -> None:
         """Setting options: [mqtt_access_token, mqtt_username, mqtt_password, mqtt_broker, mqtt_port]"""
         print(self.setting_scope)
         settings = HeimdallrSettings(setting_scope=self.setting_scope)
-        print(settings._mqtt_settings_path)
+        print(settings._mqtt_settings_path)  # TODO: ACCESS TO protected member
         settings.__setattr__(setting, value)
 
     def multi_set(self, **kw) -> None:
         """prefix kwargs sequence with a '-' eg. 'heimdallr multi_set -mqtt_port=9213' Setting options: [
         mqtt_access_token,
         mqtt_username,
         mqtt_password,
@@ -240,30 +242,31 @@
     @staticmethod
     def sponsors(*, drawer: callable = print) -> None:
         """emits sponsors"""
         drawer(sponsors)
 
     @staticmethod
     def shell():
+        """description"""
         from heimdallr.entry_points import repl
 
         repl.main()
 
 
 def draw_cli_header(
     *, title: str = "Heimdallr", font: str = "big", drawer: callable = print
 ):
-    """ """
+    """description"""
     drawer(
-        f"{Figlet(font=font, justify='center', width=terminal_width).renderText(title)}{underline}\n"
+        f"{Figlet(font = font, justify = 'center', width = terminal_width).renderText(title)}{underline}\n"
     )
 
 
 def main(*, always_draw_header: bool = False):
-    """ """
+    """description"""
     if always_draw_header:
         draw_cli_header()
     fire.Fire(HeimdallrCLI, name="heimdallr")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `Heimdallr-0.2.7/heimdallr/entry_points/deprecated/publisher_non_sch.py` & `heimdallr-0.2.8/heimdallr/entry_points/deprecated/publisher_non_sch.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 import json
 import socket
 import time
 
 import paho.mqtt.client as mqtt
-from apppath import ensure_existence
-from draugr import IgnoreInterruptSignal
-from draugr.python_utilities.business import busy_indicator
 from draugr.writers import LogWriter, MockWriter, Writer
-from warg import NOD
-
-from heimdallr import PROJECT_APP_PATH, PROJECT_NAME
 from heimdallr.configuration.heimdallr_config import ALL_CONSTANTS
 from heimdallr.configuration.heimdallr_settings import HeimdallrSettings
 from heimdallr.utilities.publisher.unpacking import pull_gpu_info
+from warg import IgnoreInterruptSignal
+from warg import NOD
+from warg import busy_indicator
+from warg import ensure_existence
+
+from heimdallr import PROJECT_APP_PATH, PROJECT_NAME
 
 HOSTNAME = socket.gethostname()
 
 __all__ = ["main"]
 
 LOG_WRITER: Writer = MockWriter()
 
 
 def on_publish(client, userdata, result) -> None:
-    """ """
+    """description"""
     global LOG_WRITER
     LOG_WRITER(result)
 
 
 def on_disconnect(client, userdata, rc):
-    """ """
+    """description"""
     if rc != 0:
         print("Unexpected MQTT disconnection. Will auto-reconnect")
         client.reconnect()
 
 
 def main(is_user: bool = False):
-    """ """
+    """description"""
     global LOG_WRITER
     if is_user:
         LOG_WRITER = LogWriter(
             ensure_existence(PROJECT_APP_PATH.user_log)
             / f"{PROJECT_NAME}_publisher.log"
         )
     else:
@@ -48,28 +48,28 @@
             / f"{PROJECT_NAME}_publisher.log"
         )
     LOG_WRITER.open()
     client = mqtt.Client()
     client.on_publish = on_publish
     client.on_disconnect = on_disconnect
 
-    HEIMDALLR_SETTINGS = HeimdallrSettings()  # TODO input scope
+    heimdallr_settings = HeimdallrSettings()  # TODO input scope
 
     client.username_pw_set(
-        HEIMDALLR_SETTINGS.mqtt_username, HEIMDALLR_SETTINGS.mqtt_password
+        heimdallr_settings.mqtt_username, heimdallr_settings.mqtt_password
     )
     try:
         client.connect(
-            HEIMDALLR_SETTINGS.mqtt_broker, HEIMDALLR_SETTINGS.mqtt_port, keepalive=60
+            heimdallr_settings.mqtt_broker, heimdallr_settings.mqtt_port, keepalive=60
         )
     except ValueError as ve:
         raise ValueError(
-            f"{HEIMDALLR_SETTINGS._mqtt_settings_path},"
-            f"{HEIMDALLR_SETTINGS.mqtt_broker},"
-            f"{HEIMDALLR_SETTINGS.mqtt_port},"
+            f"{heimdallr_settings._mqtt_settings_path},"
+            f"{heimdallr_settings.mqtt_broker},"
+            f"{heimdallr_settings.mqtt_port},"
             f"{ve}"
         )
     client.loop_start()
 
     sensor_data = NOD({HOSTNAME: pull_gpu_info()})
     next_reading = time.time()
```

### Comparing `Heimdallr-0.2.7/heimdallr/entry_points/publisher.py` & `heimdallr-0.2.8/heimdallr/entry_points/publisher.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,66 @@
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+__author__ = "Christian Heider Nielsen"
+__doc__ = r"""
+
+           Created on 19/03/2020
+           """
+
 import json
 import socket
 import time
 from typing import Any
 
 import paho.mqtt.client as mqtt
-import schedule
-from apppath import ensure_existence
-from draugr.python_utilities.business import busy_indicator
+import schedule  # TODO: USE PENDULUM INSTEAD
 from draugr.writers import LogWriter, MockWriter, Writer
-from warg import NOD
+from warg import NOD, busy_indicator, ensure_existence
 
 from heimdallr import PROJECT_APP_PATH, PROJECT_NAME
 from heimdallr.configuration.heimdallr_config import ALL_CONSTANTS
 from heimdallr.configuration.heimdallr_settings import (
     HeimdallrSettings,
     SettingScopeEnum,
 )
 from heimdallr.utilities.publisher.unpacking import pull_disk_usage_info, pull_gpu_info
 
-HOSTNAME = socket.gethostname()
-
 __all__ = ["main"]
 
+HOSTNAME = socket.gethostname()
 LOG_WRITER: Writer = MockWriter()
 
 
 def on_publish(client: Any, userdata: Any, result, writer: callable = None) -> None:
-    """ """
+    """
+    publisher callback
+    """
     global LOG_WRITER
     LOG_WRITER(result)
     if writer:
         writer(result)
 
 
 def on_disconnect(client: Any, userdata: Any, rc, writer: callable = print) -> None:
-    """ """
+    """
+    disconnect callback
+    """
     global LOG_WRITER
     if rc != 0:
         client.reconnect()
         result = "Unexpected MQTT disconnection. Will auto-reconnect"
         LOG_WRITER(result)
         writer(result)
 
 
 def main(setting_scope: SettingScopeEnum = SettingScopeEnum.user) -> None:
-    """ """
+    """
+    main entry point
+    """
     global LOG_WRITER
     if setting_scope == SettingScopeEnum.user:
         LOG_WRITER = LogWriter(
             ensure_existence(PROJECT_APP_PATH.user_log)
             / f"{PROJECT_NAME}_publisher.log"
         )
     else:
@@ -57,42 +69,42 @@
             / f"{PROJECT_NAME}_publisher.log"
         )
     LOG_WRITER.open()
     client = mqtt.Client(HOSTNAME)
     client.on_publish = on_publish
     client.on_disconnect = on_disconnect
 
-    HEIMDALLR_SETTINGS = HeimdallrSettings(setting_scope)
+    heimdallr_settings = HeimdallrSettings(setting_scope)
 
     client.username_pw_set(
-        HEIMDALLR_SETTINGS.mqtt_username, HEIMDALLR_SETTINGS.mqtt_password
+        heimdallr_settings.mqtt_username, heimdallr_settings.mqtt_password
     )
     try:
         client.connect(
-            HEIMDALLR_SETTINGS.mqtt_broker, HEIMDALLR_SETTINGS.mqtt_port, keepalive=60
+            heimdallr_settings.mqtt_broker, heimdallr_settings.mqtt_port, keepalive=60
         )
     except ValueError as ve:
         raise ValueError(
-            f"{HEIMDALLR_SETTINGS._mqtt_settings_path},"
-            f"{HEIMDALLR_SETTINGS.mqtt_broker},"
-            f"{HEIMDALLR_SETTINGS.mqtt_port},"
+            f"{heimdallr_settings._mqtt_settings_path},"
+            f"{heimdallr_settings.mqtt_broker},"
+            f"{heimdallr_settings.mqtt_port},"
             f"{ve}"
         )
 
     client.loop_start()
 
     sensor_data = NOD(
         {HOSTNAME: {"gpu_stats": pull_gpu_info(), "du_stats": pull_disk_usage_info()}}
     )
 
     if True:  # with IgnoreInterruptSignal():
         print("Publisher started")
 
         def job():
-            """ """
+            """description"""
             sensor_data[HOSTNAME]["gpu_stats"] = pull_gpu_info()
             sensor_data[HOSTNAME]["du_stats"] = pull_disk_usage_info()
             client.publish(
                 ALL_CONSTANTS.MQTT_TOPIC,
                 json.dumps(sensor_data.as_dict()),
                 ALL_CONSTANTS.MQTT_QOS,
             )
```

### Comparing `Heimdallr-0.2.7/heimdallr/entry_points/repl.py` & `heimdallr-0.2.8/heimdallr/entry_points/repl.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,47 +3,46 @@
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 19/01/2020
            """
 
-from draugr import ConfigShell
-from draugr.python_utilities import get_terminal_size
-from pyfiglet import Figlet
 
 from heimdallr.configuration.heimdallr_settings import (
     HeimdallrSettings,
     SettingScopeEnum,
 )
+from pyfiglet import Figlet
+from warg import ConfigShell, get_terminal_size
 
 margin_percentage = 0 / 6
 terminal_width = get_terminal_size().columns
 margin = int(margin_percentage * terminal_width)
 width = terminal_width - 2 * margin
 underline = "_" * width
 indent = " " * margin
 sponsors = "Alexandra Institute"
 
 
 def draw_cli_header(
     *, title: str = "Heimdallr", font: str = "big", drawer: callable = print
 ) -> None:
-    """ """
+    """description"""
     drawer(
-        f"{Figlet(font=font, justify='center', width=terminal_width).renderText(title)}{underline}\n"
+        f"{Figlet(font = font, justify = 'center', width = terminal_width).renderText(title)}{underline}\n"
     )
 
 
 def main(
     *,
     always_draw_header: bool = False,
     setting_scope: SettingScopeEnum = SettingScopeEnum.user,
 ) -> None:
-    """ """
+    """description"""
     if always_draw_header:
         draw_cli_header()
 
     repl = ConfigShell("heimdallr")
     repl.add_property_options(HeimdallrSettings(setting_scope=setting_scope))
     repl.add_func("sponsor", lambda *e: print(sponsors))
     repl.cmdloop()
```

### Comparing `Heimdallr-0.2.7/heimdallr/entry_points/server.py` & `heimdallr-0.2.8/heimdallr/entry_points/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,51 @@
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+__author__ = "Christian Heider Nielsen"
+__doc__ = r"""
+
+           Created on 19/03/2020
+           """
+
+
 import copy
 import datetime
 import json
 import logging
 import socket
 from typing import Any
 
 import dash
 import flask
-from apppath import ensure_existence
 from dash import Dash
 from dash.dash_table import DataTable
 from dash.dependencies import Input, Output
 from dash.html import Div
-from draugr.python_utilities import default_datetime_repr
 from draugr.writers import LogWriter, MockWriter, Writer
 from flask import Response
-from paho import mqtt
-from paho.mqtt.client import Client
-from pandas import DataFrame
-from waitress import serve
-from warg import NOD
-
-from heimdallr import PROJECT_APP_PATH, PROJECT_NAME
 from heimdallr.configuration.heimdallr_config import ALL_CONSTANTS
 from heimdallr.configuration.heimdallr_settings import (
     HeimdallrSettings,
     SettingScopeEnum,
 )
 from heimdallr.server.board_layout import get_root_layout
 from heimdallr.utilities.server import (
     get_calender_df,
     per_machine_per_device_pie_charts,
     to_overall_gpu_process_df,
 )
+from paho import mqtt
+from paho.mqtt.client import Client
+from pandas import DataFrame
+from waitress import serve
+from warg import NOD, default_datetime_repr
+from warg import ensure_existence
+
+from heimdallr import PROJECT_APP_PATH, PROJECT_NAME
 
 __all__ = ["main"]
 
 from heimdallr.utilities.server.du_utilities import to_overall_du_process_df
 from heimdallr.utilities.server.teams_status import team_members_status
 
 log = logging.getLogger("werkzeug")
@@ -87,77 +96,84 @@
 
 
 @DASH_APP.callback(
     Output(ALL_CONSTANTS.TIME_ID, "children"),
     [Input(ALL_CONSTANTS.TIME_INTERVAL_ID, "n_intervals")],
 )
 def update_time(n: int) -> str:
-    """ """
+    """description"""
     global GPU_STATS
     global KEEP_ALIVE
-    for k, v in KEEP_ALIVE.items():
-        if v > ALL_CONSTANTS.TIMEOUT_MACHINES_SEC:
-            if k in GPU_STATS.keys():
-                GPU_STATS.pop(k)
-                print(f"deleting {k} from stats")
-
-    for key in list(KEEP_ALIVE.keys()):
-        if key in GPU_STATS.keys():
-            KEEP_ALIVE[key] = KEEP_ALIVE[key] + 1
-        else:
-            KEEP_ALIVE.pop(key)
-            print(f"deleting {key} from keep alive")
+    try:
+        for k, v in KEEP_ALIVE.items():
+            if v > ALL_CONSTANTS.TIMEOUT_MACHINES_SEC:
+                if k in GPU_STATS.keys():
+                    GPU_STATS.pop(k)
+                    print(f"deleting {k} from stats")
+
+        for key in list(KEEP_ALIVE.keys()):
+            if key in GPU_STATS.keys():
+                KEEP_ALIVE[key] = KEEP_ALIVE[key] + 1
+            else:
+                KEEP_ALIVE.pop(key)
+                print(f"deleting {key} from keep alive")
+
+    except Exception as e:
+        print(e)
 
     return default_datetime_repr(datetime.datetime.now())
 
 
 @DASH_APP.callback(
     Output(ALL_CONSTANTS.CALENDAR_ID, "children"),
     [Input(ALL_CONSTANTS.CALENDAR_INTERVAL_ID, "n_intervals")],
 )
 def update_calendar_live(n: int) -> DataTable:
-    """ """
-    df = get_calender_df(
-        HeimdallrSettings().google_calendar_id,
-        HeimdallrSettings()._credentials_base_path,
-        num_entries=ALL_CONSTANTS.TABLE_PAGE_SIZE,
-    )
+    """description"""
+    try:
+        df = get_calender_df(
+            HeimdallrSettings().google_calendar_id,
+            HeimdallrSettings()._credentials_base_path,
+            num_entries=ALL_CONSTANTS.TABLE_PAGE_SIZE,
+        )
 
-    return DataTable(
-        id="calender-table-0",
-        columns=[{"name": i, "id": i} for i in df.columns],
-        data=df.to_dict("records"),
-        page_size=ALL_CONSTANTS.TABLE_PAGE_SIZE,
-        style_as_list_view=True,
-        style_data_conditional=[
-            {
-                "if": {"column_id": "start", "filter_query": "{start} > 3.9"},
-                "backgroundColor": "green",
-                "color": "white",
-            },
-        ],  # TODO: MAKE GRADIENT TO ORANGE FOR WHEN NEARING START, and GREEN WHEN IN PROGRESS
-    )
+        return DataTable(
+            id="calender-table-0",
+            columns=[{"name": i, "id": i} for i in df.columns],
+            data=df.to_dict("records"),
+            page_size=ALL_CONSTANTS.TABLE_PAGE_SIZE,
+            style_as_list_view=True,
+            style_data_conditional=[
+                {
+                    "if": {"column_id": "start", "filter_query": "{start} > 3.9"},
+                    "backgroundColor": "green",
+                    "color": "white",
+                },
+            ],  # TODO: MAKE GRADIENT TO ORANGE FOR WHEN NEARING START, and GREEN WHEN IN PROGRESS
+        )
+    except Exception as e:
+        return Div([f"Error: {e}"])
 
 
 @DASH_APP.callback(
     Output(ALL_CONSTANTS.TEAMS_STATUS_ID, "children"),
     [Input(ALL_CONSTANTS.TEAMS_STATUS_INTERVAL_ID, "n_intervals")],
 )
 def update_teams_status_live(n: int) -> Div:
-    """ """
+    """description"""
 
     return Div(team_members_status(None), className="row")
 
 
 @DASH_APP.callback(
     Output(ALL_CONSTANTS.GPU_GRAPHS_ID, "children"),
     [Input(ALL_CONSTANTS.GPU_INTERVAL_ID, "n_intervals")],
 )
 def update_graph(n: int) -> Div:
-    """ """
+    """description"""
     global GPU_STATS
     global KEEP_ALIVE
     compute_machines = []
     if GPU_STATS:
         compute_machines.extend(
             per_machine_per_device_pie_charts(copy.deepcopy(GPU_STATS), KEEP_ALIVE)
         )
@@ -165,15 +181,15 @@
 
 
 @DASH_APP.callback(
     Output(ALL_CONSTANTS.GPU_TABLES_ID, "children"),
     [Input(ALL_CONSTANTS.GPU_INTERVAL_ID, "n_intervals")],
 )
 def update_table(n: int) -> Div:
-    """ """
+    """description"""
     MQTT_CLIENT.loop()
 
     compute_machines = []
 
     if GPU_STATS:
         df = to_overall_gpu_process_df(copy.deepcopy(GPU_STATS))
     else:
@@ -200,15 +216,15 @@
 
 
 @DASH_APP.callback(
     Output(ALL_CONSTANTS.DU_TABLES_ID, "children"),
     [Input(ALL_CONSTANTS.DU_INTERVAL_ID, "n_intervals")],
 )
 def update_table(n: int) -> Div:
-    """ """
+    """description"""
     MQTT_CLIENT.loop()
 
     compute_machines = []
 
     if DU_STATS:
         df = to_overall_du_process_df(copy.deepcopy(DU_STATS))
     else:
@@ -266,15 +282,15 @@
                 setattr(settings, k, v)
     else:
         print("Not in development mode")
     return flask.redirect("/")
 
 
 def on_message(client: Any, userdata: Any, result: mqtt.client.MQTTMessage) -> None:
-    """ """
+    """description"""
     global LOG_WRITER
     global GPU_STATS
     global KEEP_ALIVE
     d = json.loads(result.payload)
     keys = d.keys()
     for key in keys:
         if "gpu_stats" in d[key]:
@@ -286,22 +302,27 @@
         KEEP_ALIVE[key] = 0
     LOG_WRITER(
         f"received payload for {keys}, retain:{result.retain}, timestamp:{result.timestamp}"
     )
 
 
 def on_disconnect(client: Any, userdata: Any, rc: Any) -> None:
-    """ """
+    """description"""
     if rc != 0:
         print("Unexpected MQTT disconnection. Will auto-reconnect")
         client.reconnect()
         client.subscribe(ALL_CONSTANTS.MQTT_TOPIC, ALL_CONSTANTS.MQTT_QOS)
 
 
 def setup_mqtt_connection(settings) -> None:
+    """
+
+    :param settings:
+    :type settings:
+    """
     if (
         False
         # settings.mqtt_access_token and False
     ):  # TODO: not implemented
         pass
         # MQTT_CLIENT.username_pw_set(settings.MQTT_ACCESS_TOKEN)
     else:
@@ -323,15 +344,15 @@
 
 def main(
     *args,
     setting_scope: SettingScopeEnum = SettingScopeEnum.user,
     development=False,
     **kwargs,
 ) -> None:
-    """ """
+    """description"""
     global LOG_WRITER, DEVELOPMENT
 
     if setting_scope == SettingScopeEnum.user:
         LOG_WRITER = LogWriter(
             ensure_existence(PROJECT_APP_PATH.user_log) / f"{PROJECT_NAME}_server.log"
         )
     else:
```

### Comparing `Heimdallr-0.2.7/heimdallr/server/board_layout/body.py` & `heimdallr-0.2.8/heimdallr/server/board_layout/body.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 15/03/2020
            """
 
+__all__ = ["get_body"]
+
 from typing import List
 
 from dash import dcc, html
-
 from heimdallr.configuration.heimdallr_config import (
     CALENDAR_ID,
     CALENDAR_INTERVAL_ID,
     CALENDAR_INTERVAL_MS,
     DU_INTERVAL_ID,
     DU_INTERVAL_MS,
     DU_TABLES_ID,
@@ -23,19 +24,19 @@
     GPU_INTERVAL_MS,
     GPU_TABLES_ID,
     TEAMS_STATUS_ID,
     TEAMS_STATUS_INTERVAL_ID,
     TEAMS_STATUS_INTERVAL_MS,
 )
 
-__all__ = ["get_body"]
-
 
 def get_body() -> List[html.Div]:
-    """ """
+    """
+    body
+    """
     return [
         html.Div(
             [
                 html.Div(
                     [
                         html.Div([], id=CALENDAR_ID),
                         dcc.Interval(
```

### Comparing `Heimdallr-0.2.7/heimdallr/server/board_layout/footer.py` & `heimdallr-0.2.8/heimdallr/server/board_layout/footer.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,15 +14,17 @@
     BUILD_STATUS_MAPPING,
 )
 
 __all__ = ["get_footer"]
 
 
 def get_footer() -> html.Footer:
-    """ """
+    """
+    footer
+    """
     return html.Footer(
         [
             html.Div(
                 [
                     html.P([f"{k}: "]),
                     html.A([html.Img(src=v)], href=v.split(".svg")[0]),
                 ],
```

### Comparing `Heimdallr-0.2.7/heimdallr/server/board_layout/header.py` & `heimdallr-0.2.8/heimdallr/server/board_layout/header.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,27 +7,29 @@
            Created on 15/03/2020
            """
 
 import base64
 from pathlib import Path
 
 from dash import dcc, html
-
-import heimdallr
 from heimdallr.configuration.heimdallr_config import (
     HTML_TITLE,
     TIME_ID,
     TIME_INTERVAL_ID,
 )
 
+import heimdallr
+
 __all__ = ["get_header"]
 
 
 def get_header() -> html.Div:
-    """ """
+    """
+    header
+    """
     svg_p = Path(heimdallr.__file__).parent / "entry_points" / "assets" / "aivclab.svg"
     if svg_p.exists():
         with open(
             svg_p,
             "rb",
         ) as svg:
             encoded = base64.b64encode(svg.read())
```

### Comparing `Heimdallr-0.2.7/heimdallr/server/board_layout/menu.py` & `heimdallr-0.2.8/heimdallr/server/board_layout/menu.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
            Created on 15/03/2020
            """
 
 from itertools import cycle
 
 from dash import dcc, html
-
 from heimdallr.configuration.heimdallr_settings import HeimdallrSettings
 
 # import dash_bootstrap_components #TODO
 
 """
 import dash_bootstrap_components as dbc
 import dash_html_components as html
@@ -73,15 +72,15 @@
                           )
                       for inp_type in ALLOWED_TYPES
                       ]
 """
 
 
 def get_menu() -> html.Div:
-    """ """
+    """description"""
     return html.Div(
         [
             html.Div(
                 [
                     html.Div(
                         [html.Button("Show/Hide Menu", id="menu_toggle_button")],
                         className="row p-1",
```

### Comparing `Heimdallr-0.2.7/heimdallr/utilities/nvidia/bindings.py` & `heimdallr-0.2.8/heimdallr/utilities/nvidia/bindings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+__author__ = "Christian"
+__doc__ = r"""
+
+           Created on 29/03/2020
+           """
+
 # ============================================================================ #
 # Copyright (c) 2011-2015, NVIDIA Corporation.  All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 #    * Redistributions of source code must retain the above copyright notice,
@@ -291,15 +300,15 @@
 
 
 class NVMLError_Uninitialized(Exception):
     pass
 
 
 class NVMLError(Exception):
-    """ """
+    """description"""
 
     _val_mapping = dict()
     # List of currently known error codes
     _errcode_to_string = {
         NVML_ERROR_UNINITIALIZED: "Uninitialized",
         NVML_ERROR_INVALID_ARGUMENT: "Invalid Argument",
         NVML_ERROR_NOT_SUPPORTED: "Not Supported",
@@ -362,18 +371,18 @@
         # e.g. Turn NVML_ERROR_ALREADY_INITIALIZED into NVMLError_AlreadyInitialized
         class_name = "NVMLError_" + string.capwords(
             err_name.replace("NVML_ERROR_", ""), "_"
         ).replace("_", "")
         err_val = getattr(this_module, err_name)
 
         def gen_new(val):
-            """ """
+            """description"""
 
             def new(typ):
-                """ """
+                """description"""
                 obj = NVMLError.__new__(typ, val)
                 return obj
 
             return new
 
         new_error_class = type(class_name, (NVMLError,), {"__new__": gen_new(err_val)})
         new_error_class.__module__ = __name__
@@ -381,15 +390,15 @@
         NVMLError._val_mapping[err_val] = new_error_class
 
 
 _extract_errors_as_classes()
 
 
 def check_return(ret):
-    """ """
+    """description"""
     if ret != NVML_SUCCESS:
         raise NVMLError(ret)
     return ret
 
 
 ## ========================================================================== ##
 ##                                                                            ##
@@ -399,15 +408,15 @@
 
 _func_pointer_cache = (
     dict()
 )  # function pointers are cached to prevent unnecessary lib_load_lock locking
 
 
 def get_func_pointer(name):
-    """ """
+    """description"""
     global nvml_lib
 
     if name in _func_pointer_cache:
         return _func_pointer_cache[name]
 
     lib_load_lock.acquire()
     try:
@@ -425,38 +434,38 @@
 
 
 ## Alternative object
 # Allows the object to be printed
 # Allows mismatched types to be assigned
 #  - like None when the Structure variant requires c_uint
 class FriendlyObject(object):
-    """ """
+    """description"""
 
     def __init__(self, dictionary):
         for x in dictionary:
             setattr(self, x, dictionary[x])
 
     def __str__(self):
         return self.__dict__.__str__()
 
 
 def struct_to_friendly_object(struct):
-    """ """
+    """description"""
     d = {}
     for x in struct._fields_:
         key = x[0]
         value = getattr(struct, key)
         d[key] = value
     obj = FriendlyObject(d)
     return obj
 
 
 # pack the object so it can be passed to the NVML library
 def friendly_object_to_struct(obj, model):
-    """ """
+    """description"""
     for x in model._fields_:
         key = x[0]
         value = obj.__dict__[key]
         setattr(model, key, value)
     return model
 
 
@@ -854,53 +863,53 @@
         nvml_lib_refcount -= 1
     lib_load_lock.release()
     return None
 
 
 # Added in 2.285
 def nvml_error_string(result):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlErrorString")
     fn.restype = c_char_p  # otherwise return is an int
     ret = fn(result)
     return ret
 
 
 # Added in 2.285
 def nvmlSystemGetNVMLVersion():
-    """ """
+    """description"""
     c_version = create_string_buffer(NVML_SYSTEM_NVML_VERSION_BUFFER_SIZE)
     fn = get_func_pointer("nvmlSystemGetNVMLVersion")
     ret = fn(c_version, c_uint(NVML_SYSTEM_NVML_VERSION_BUFFER_SIZE))
     check_return(ret)
     return c_version.value
 
 
 # Added in 2.285
 def nvmlSystemGetProcessName(pid):
-    """ """
+    """description"""
     c_name = create_string_buffer(1024)
     fn = get_func_pointer("nvmlSystemGetProcessName")
     ret = fn(c_uint(pid), c_name, c_uint(1024))
     check_return(ret)
     return c_name.value
 
 
 def nvmlSystemGetDriverVersion():
-    """ """
+    """description"""
     c_version = create_string_buffer(NVML_SYSTEM_DRIVER_VERSION_BUFFER_SIZE)
     fn = get_func_pointer("nvmlSystemGetDriverVersion")
     ret = fn(c_version, c_uint(NVML_SYSTEM_DRIVER_VERSION_BUFFER_SIZE))
     check_return(ret)
     return c_version.value
 
 
 # Added in 2.285
 def nvmlSystemGetHicVersion():
-    """ """
+    """description"""
     c_count = c_uint(0)
     hics = None
     fn = get_func_pointer("nvmlSystemGetHicVersion")
 
     # get the count
     ret = fn(byref(c_count), None)
 
@@ -917,361 +926,361 @@
     ret = fn(byref(c_count), hics)
     check_return(ret)
     return hics
 
 
 ## Unit get functions
 def nvmlUnitGetCount():
-    """ """
+    """description"""
     c_count = c_uint()
     fn = get_func_pointer("nvmlUnitGetCount")
     ret = fn(byref(c_count))
     check_return(ret)
     return c_count.value
 
 
 def nvmlUnitGetHandleByIndex(index):
-    """ """
+    """description"""
     c_index = c_uint(index)
     unit = c_nvmlUnit_t()
     fn = get_func_pointer("nvmlUnitGetHandleByIndex")
     ret = fn(c_index, byref(unit))
     check_return(ret)
     return unit
 
 
 def nvmlUnitGetUnitInfo(unit):
-    """ """
+    """description"""
     c_info = c_nvmlUnitInfo_t()
     fn = get_func_pointer("nvmlUnitGetUnitInfo")
     ret = fn(unit, byref(c_info))
     check_return(ret)
     return c_info
 
 
 def nvmlUnitGetLedState(unit):
-    """ """
+    """description"""
     c_state = c_nvmlLedState_t()
     fn = get_func_pointer("nvmlUnitGetLedState")
     ret = fn(unit, byref(c_state))
     check_return(ret)
     return c_state
 
 
 def nvmlUnitGetPsuInfo(unit):
-    """ """
+    """description"""
     c_info = c_nvmlPSUInfo_t()
     fn = get_func_pointer("nvmlUnitGetPsuInfo")
     ret = fn(unit, byref(c_info))
     check_return(ret)
     return c_info
 
 
 def nvmlUnitGetTemperature(unit, type):
-    """ """
+    """description"""
     c_temp = c_uint()
     fn = get_func_pointer("nvmlUnitGetTemperature")
     ret = fn(unit, c_uint(type), byref(c_temp))
     check_return(ret)
     return c_temp.value
 
 
 def nvmlUnitGetFanSpeedInfo(unit):
-    """ """
+    """description"""
     c_speeds = c_nvmlUnitFanSpeeds_t()
     fn = get_func_pointer("nvmlUnitGetFanSpeedInfo")
     ret = fn(unit, byref(c_speeds))
     check_return(ret)
     return c_speeds
 
 
 # added to API
 def nvmlUnitGetDeviceCount(unit):
-    """ """
+    """description"""
     c_count = c_uint(0)
     # query the unit to determine device count
     fn = get_func_pointer("nvmlUnitGetDevices")
     ret = fn(unit, byref(c_count), None)
     if ret == NVML_ERROR_INSUFFICIENT_SIZE:
         ret = NVML_SUCCESS
     check_return(ret)
     return c_count.value
 
 
 def nvmlUnitGetDevices(unit):
-    """ """
+    """description"""
     c_count = c_uint(nvmlUnitGetDeviceCount(unit))
     device_array = c_nvmlDevice_t * c_count.value
     c_devices = device_array()
     fn = get_func_pointer("nvmlUnitGetDevices")
     ret = fn(unit, byref(c_count), c_devices)
     check_return(ret)
     return c_devices
 
 
 ## Device get functions
 def nvmlDeviceGetCount():
-    """ """
+    """description"""
     c_count = c_uint()
     fn = get_func_pointer("nvmlDeviceGetCount_v2")
     ret = fn(byref(c_count))
     check_return(ret)
     return c_count.value
 
 
 def nvmlDeviceGetHandleByIndex(index):
-    """ """
+    """description"""
     c_index = c_uint(index)
     device = c_nvmlDevice_t()
     fn = get_func_pointer("nvmlDeviceGetHandleByIndex_v2")
     ret = fn(c_index, byref(device))
     check_return(ret)
     return device
 
 
 def nvmlDeviceGetHandleBySerial(serial):
-    """ """
+    """description"""
     c_serial = c_char_p(serial)
     device = c_nvmlDevice_t()
     fn = get_func_pointer("nvmlDeviceGetHandleBySerial")
     ret = fn(c_serial, byref(device))
     check_return(ret)
     return device
 
 
 def nvmlDeviceGetHandleByUUID(uuid):
-    """ """
+    """description"""
     c_uuid = c_char_p(uuid)
     device = c_nvmlDevice_t()
     fn = get_func_pointer("nvmlDeviceGetHandleByUUID")
     ret = fn(c_uuid, byref(device))
     check_return(ret)
     return device
 
 
 def nvmlDeviceGetHandleByPciBusId(pciBusId):
-    """ """
+    """description"""
     c_busId = c_char_p(pciBusId)
     device = c_nvmlDevice_t()
     fn = get_func_pointer("nvmlDeviceGetHandleByPciBusId_v2")
     ret = fn(c_busId, byref(device))
     check_return(ret)
     return device
 
 
 def nvmlDeviceGetName(handle):
-    """ """
+    """description"""
     c_name = create_string_buffer(NVML_DEVICE_NAME_BUFFER_SIZE)
     fn = get_func_pointer("nvmlDeviceGetName")
     ret = fn(handle, c_name, c_uint(NVML_DEVICE_NAME_BUFFER_SIZE))
     check_return(ret)
     return c_name.value
 
 
 def nvmlDeviceGetBoardId(handle):
-    """ """
+    """description"""
     c_id = c_uint()
     fn = get_func_pointer("nvmlDeviceGetBoardId")
     ret = fn(handle, byref(c_id))
     check_return(ret)
     return c_id.value
 
 
 def nvmlDeviceGetMultiGpuBoard(handle):
-    """ """
+    """description"""
     c_multiGpu = c_uint()
     fn = get_func_pointer("nvmlDeviceGetMultiGpuBoard")
     ret = fn(handle, byref(c_multiGpu))
     check_return(ret)
     return c_multiGpu.value
 
 
 def nvmlDeviceGetBrand(handle):
-    """ """
+    """description"""
     c_type = _nvmlBrandType_t()
     fn = get_func_pointer("nvmlDeviceGetBrand")
     ret = fn(handle, byref(c_type))
     check_return(ret)
     return c_type.value
 
 
 def nvmlDeviceGetSerial(handle):
-    """ """
+    """description"""
     c_serial = create_string_buffer(NVML_DEVICE_SERIAL_BUFFER_SIZE)
     fn = get_func_pointer("nvmlDeviceGetSerial")
     ret = fn(handle, c_serial, c_uint(NVML_DEVICE_SERIAL_BUFFER_SIZE))
     check_return(ret)
     return c_serial.value
 
 
 def nvmlDeviceGetCpuAffinity(handle, cpuSetSize):
-    """ """
+    """description"""
     affinity_array = c_ulonglong * cpuSetSize
     c_affinity = affinity_array()
     fn = get_func_pointer("nvmlDeviceGetCpuAffinity")
     ret = fn(handle, cpuSetSize, byref(c_affinity))
     check_return(ret)
     return c_affinity
 
 
 def nvmlDeviceSetCpuAffinity(handle):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlDeviceSetCpuAffinity")
     ret = fn(handle)
     check_return(ret)
     return None
 
 
 def nvmlDeviceClearCpuAffinity(handle):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlDeviceClearCpuAffinity")
     ret = fn(handle)
     check_return(ret)
     return None
 
 
 def nvmlDeviceGetMinorNumber(handle):
-    """ """
+    """description"""
     c_minor_number = c_uint()
     fn = get_func_pointer("nvmlDeviceGetMinorNumber")
     ret = fn(handle, byref(c_minor_number))
     check_return(ret)
     return c_minor_number.value
 
 
 def nvmlDeviceGetUUID(handle):
-    """ """
+    """description"""
     c_uuid = create_string_buffer(NVML_DEVICE_UUID_BUFFER_SIZE)
     fn = get_func_pointer("nvmlDeviceGetUUID")
     ret = fn(handle, c_uuid, c_uint(NVML_DEVICE_UUID_BUFFER_SIZE))
     check_return(ret)
     return c_uuid.value
 
 
 def nvmlDeviceGetInforomVersion(handle, infoRomObject):
-    """ """
+    """description"""
     c_version = create_string_buffer(NVML_DEVICE_INFOROM_VERSION_BUFFER_SIZE)
     fn = get_func_pointer("nvmlDeviceGetInforomVersion")
     ret = fn(
         handle,
         _nvmlInforomObject_t(infoRomObject),
         c_version,
         c_uint(NVML_DEVICE_INFOROM_VERSION_BUFFER_SIZE),
     )
     check_return(ret)
     return c_version.value
 
 
 # Added in 4.304
 def nvmlDeviceGetInforomImageVersion(handle):
-    """ """
+    """description"""
     c_version = create_string_buffer(NVML_DEVICE_INFOROM_VERSION_BUFFER_SIZE)
     fn = get_func_pointer("nvmlDeviceGetInforomImageVersion")
     ret = fn(handle, c_version, c_uint(NVML_DEVICE_INFOROM_VERSION_BUFFER_SIZE))
     check_return(ret)
     return c_version.value
 
 
 # Added in 4.304
 def nvmlDeviceGetInforomConfigurationChecksum(handle):
-    """ """
+    """description"""
     c_checksum = c_uint()
     fn = get_func_pointer("nvmlDeviceGetInforomConfigurationChecksum")
     ret = fn(handle, byref(c_checksum))
     check_return(ret)
     return c_checksum.value
 
 
 # Added in 4.304
 def nvmlDeviceValidateInforom(handle):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlDeviceValidateInforom")
     ret = fn(handle)
     check_return(ret)
     return None
 
 
 def nvmlDeviceGetDisplayMode(handle):
-    """ """
+    """description"""
     c_mode = _nvmlEnableState_t()
     fn = get_func_pointer("nvmlDeviceGetDisplayMode")
     ret = fn(handle, byref(c_mode))
     check_return(ret)
     return c_mode.value
 
 
 def nvmlDeviceGetDisplayActive(handle):
-    """ """
+    """description"""
     c_mode = _nvmlEnableState_t()
     fn = get_func_pointer("nvmlDeviceGetDisplayActive")
     ret = fn(handle, byref(c_mode))
     check_return(ret)
     return c_mode.value
 
 
 def nvmlDeviceGetPersistenceMode(handle):
-    """ """
+    """description"""
     c_state = _nvmlEnableState_t()
     fn = get_func_pointer("nvmlDeviceGetPersistenceMode")
     ret = fn(handle, byref(c_state))
     check_return(ret)
     return c_state.value
 
 
 def nvmlDeviceGetPciInfo(handle):
-    """ """
+    """description"""
     c_info = nvmlPciInfo_t()
     fn = get_func_pointer("nvmlDeviceGetPciInfo_v2")
     ret = fn(handle, byref(c_info))
     check_return(ret)
     return c_info
 
 
 def nvmlDeviceGetClockInfo(handle, type):
-    """ """
+    """description"""
     c_clock = c_uint()
     fn = get_func_pointer("nvmlDeviceGetClockInfo")
     ret = fn(handle, _nvmlClockType_t(type), byref(c_clock))
     check_return(ret)
     return c_clock.value
 
 
 # Added in 2.285
 def nvmlDeviceGetMaxClockInfo(handle, type):
-    """ """
+    """description"""
     c_clock = c_uint()
     fn = get_func_pointer("nvmlDeviceGetMaxClockInfo")
     ret = fn(handle, _nvmlClockType_t(type), byref(c_clock))
     check_return(ret)
     return c_clock.value
 
 
 # Added in 4.304
 def nvmlDeviceGetApplicationsClock(handle, type):
-    """ """
+    """description"""
     c_clock = c_uint()
     fn = get_func_pointer("nvmlDeviceGetApplicationsClock")
     ret = fn(handle, _nvmlClockType_t(type), byref(c_clock))
     check_return(ret)
     return c_clock.value
 
 
 # Added in 5.319
 def nvmlDeviceGetDefaultApplicationsClock(handle, type):
-    """ """
+    """description"""
     c_clock = c_uint()
     fn = get_func_pointer("nvmlDeviceGetDefaultApplicationsClock")
     ret = fn(handle, _nvmlClockType_t(type), byref(c_clock))
     check_return(ret)
     return c_clock.value
 
 
 # Added in 4.304
 def nvmlDeviceGetSupportedMemoryClocks(handle):
-    """ """
+    """description"""
     # first call to get the size
     c_count = c_uint(0)
     fn = get_func_pointer("nvmlDeviceGetSupportedMemoryClocks")
     ret = fn(handle, byref(c_count), None)
 
     if ret == NVML_SUCCESS:
         # special case, no clocks
@@ -1293,15 +1302,15 @@
     else:
         # error case
         raise NVMLError(ret)
 
 
 # Added in 4.304
 def nvmlDeviceGetSupportedGraphicsClocks(handle, memoryClockMHz):
-    """ """
+    """description"""
     # first call to get the size
     c_count = c_uint(0)
     fn = get_func_pointer("nvmlDeviceGetSupportedGraphicsClocks")
     ret = fn(handle, c_uint(memoryClockMHz), byref(c_count), None)
 
     if ret == NVML_SUCCESS:
         # special case, no clocks
@@ -1322,146 +1331,146 @@
         return procs
     else:
         # error case
         raise NVMLError(ret)
 
 
 def nvmlDeviceGetFanSpeed(handle):
-    """ """
+    """description"""
     c_speed = c_uint()
     fn = get_func_pointer("nvmlDeviceGetFanSpeed")
     ret = fn(handle, byref(c_speed))
     check_return(ret)
     return c_speed.value
 
 
 def nvmlDeviceGetTemperature(handle, sensor):
-    """ """
+    """description"""
     c_temp = c_uint()
     fn = get_func_pointer("nvmlDeviceGetTemperature")
     ret = fn(handle, _nvmlTemperatureSensors_t(sensor), byref(c_temp))
     check_return(ret)
     return c_temp.value
 
 
 def nvmlDeviceGetTemperatureThreshold(handle, threshold):
-    """ """
+    """description"""
     c_temp = c_uint()
     fn = get_func_pointer("nvmlDeviceGetTemperatureThreshold")
     ret = fn(handle, _nvmlTemperatureThresholds_t(threshold), byref(c_temp))
     check_return(ret)
     return c_temp.value
 
 
 # DEPRECATED use nvmlDeviceGetPerformanceState
 def nvmlDeviceGetPowerState(handle):
-    """ """
+    """description"""
     c_pstate = _nvmlPstates_t()
     fn = get_func_pointer("nvmlDeviceGetPowerState")
     ret = fn(handle, byref(c_pstate))
     check_return(ret)
     return c_pstate.value
 
 
 def nvmlDeviceGetPerformanceState(handle):
-    """ """
+    """description"""
     c_pstate = _nvmlPstates_t()
     fn = get_func_pointer("nvmlDeviceGetPerformanceState")
     ret = fn(handle, byref(c_pstate))
     check_return(ret)
     return c_pstate.value
 
 
 def nvmlDeviceGetPowerManagementMode(handle):
-    """ """
+    """description"""
     c_pcapMode = _nvmlEnableState_t()
     fn = get_func_pointer("nvmlDeviceGetPowerManagementMode")
     ret = fn(handle, byref(c_pcapMode))
     check_return(ret)
     return c_pcapMode.value
 
 
 def nvmlDeviceGetPowerManagementLimit(handle):
-    """ """
+    """description"""
     c_limit = c_uint()
     fn = get_func_pointer("nvmlDeviceGetPowerManagementLimit")
     ret = fn(handle, byref(c_limit))
     check_return(ret)
     return c_limit.value
 
 
 # Added in 4.304
 def nvmlDeviceGetPowerManagementLimitConstraints(handle):
-    """ """
+    """description"""
     c_minLimit = c_uint()
     c_maxLimit = c_uint()
     fn = get_func_pointer("nvmlDeviceGetPowerManagementLimitConstraints")
     ret = fn(handle, byref(c_minLimit), byref(c_maxLimit))
     check_return(ret)
     return [c_minLimit.value, c_maxLimit.value]
 
 
 # Added in 4.304
 def nvmlDeviceGetPowerManagementDefaultLimit(handle):
-    """ """
+    """description"""
     c_limit = c_uint()
     fn = get_func_pointer("nvmlDeviceGetPowerManagementDefaultLimit")
     ret = fn(handle, byref(c_limit))
     check_return(ret)
     return c_limit.value
 
 
 # Added in 331
 def nvmlDeviceGetEnforcedPowerLimit(handle):
-    """ """
+    """description"""
     c_limit = c_uint()
     fn = get_func_pointer("nvmlDeviceGetEnforcedPowerLimit")
     ret = fn(handle, byref(c_limit))
     check_return(ret)
     return c_limit.value
 
 
 def nvmlDeviceGetPowerUsage(handle):
-    """ """
+    """description"""
     c_mWatts = c_uint()
     fn = get_func_pointer("nvmlDeviceGetPowerUsage")
     ret = fn(handle, byref(c_mWatts))
     check_return(ret)
     return c_mWatts.value
 
 
 def nvmlDeviceGetTotalEnergyConsumption(handle):
-    """ """
+    """description"""
     c_mJoules = c_uint()
     fn = get_func_pointer("nvmlDeviceGetTotalEnergyConsumption")
     ret = fn(handle, byref(c_mJoules))
     check_return(ret)
     return c_mJoules.value
 
 
 # Added in 4.304
 def nvmlDeviceGetGpuOperationMode(handle):
-    """ """
+    """description"""
     c_currState = _nvmlGpuOperationMode_t()
     c_pendingState = _nvmlGpuOperationMode_t()
     fn = get_func_pointer("nvmlDeviceGetGpuOperationMode")
     ret = fn(handle, byref(c_currState), byref(c_pendingState))
     check_return(ret)
     return [c_currState.value, c_pendingState.value]
 
 
 # Added in 4.304
 def nvmlDeviceGetCurrentGpuOperationMode(handle):
-    """ """
+    """description"""
     return nvmlDeviceGetGpuOperationMode(handle)[0]
 
 
 # Added in 4.304
 def nvmlDeviceGetPendingGpuOperationMode(handle):
-    """ """
+    """description"""
     return nvmlDeviceGetGpuOperationMode(handle)[1]
 
 
 def nvmlDeviceGetMemoryInfo(handle):
     """Retrieves memory object.
 
     Return object includes the amount of used, free and total memory available
@@ -1478,171 +1487,171 @@
     fn = get_func_pointer("nvmlDeviceGetMemoryInfo")
     ret = fn(handle, byref(c_memory))
     check_return(ret)
     return c_memory
 
 
 def nvmlDeviceGetBAR1MemoryInfo(handle):
-    """ """
+    """description"""
     c_bar1_memory = c_nvmlBAR1Memory_t()
     fn = get_func_pointer("nvmlDeviceGetBAR1MemoryInfo")
     ret = fn(handle, byref(c_bar1_memory))
     check_return(ret)
     return c_bar1_memory
 
 
 def nvmlDeviceGetComputeMode(handle):
-    """ """
+    """description"""
     c_mode = _nvmlComputeMode_t()
     fn = get_func_pointer("nvmlDeviceGetComputeMode")
     ret = fn(handle, byref(c_mode))
     check_return(ret)
     return c_mode.value
 
 
 def nvmlDeviceGetEccMode(handle):
-    """ """
+    """description"""
     c_currState = _nvmlEnableState_t()
     c_pendingState = _nvmlEnableState_t()
     fn = get_func_pointer("nvmlDeviceGetEccMode")
     ret = fn(handle, byref(c_currState), byref(c_pendingState))
     check_return(ret)
     return [c_currState.value, c_pendingState.value]
 
 
 # added to API
 def nvmlDeviceGetCurrentEccMode(handle):
-    """ """
+    """description"""
     return nvmlDeviceGetEccMode(handle)[0]
 
 
 # added to API
 def nvmlDeviceGetPendingEccMode(handle):
-    """ """
+    """description"""
     return nvmlDeviceGetEccMode(handle)[1]
 
 
 def nvmlDeviceGetTotalEccErrors(handle, errorType, counterType):
-    """ """
+    """description"""
     c_count = c_ulonglong()
     fn = get_func_pointer("nvmlDeviceGetTotalEccErrors")
     ret = fn(
         handle,
         _nvmlMemoryErrorType_t(errorType),
         _nvmlEccCounterType_t(counterType),
         byref(c_count),
     )
     check_return(ret)
     return c_count.value
 
 
 # This is deprecated, instead use nvmlDeviceGetMemoryErrorCounter
 def nvmlDeviceGetDetailedEccErrors(handle, errorType, counterType):
-    """ """
+    """description"""
     c_counts = c_nvmlEccErrorCounts_t()
     fn = get_func_pointer("nvmlDeviceGetDetailedEccErrors")
     ret = fn(
         handle,
         _nvmlMemoryErrorType_t(errorType),
         _nvmlEccCounterType_t(counterType),
         byref(c_counts),
     )
     check_return(ret)
     return c_counts
 
 
 # Added in 4.304
 def nvmlDeviceGetMemoryErrorCounter(handle, errorType, counterType, locationType):
-    """ """
+    """description"""
     c_count = c_ulonglong()
     fn = get_func_pointer("nvmlDeviceGetMemoryErrorCounter")
     ret = fn(
         handle,
         _nvmlMemoryErrorType_t(errorType),
         _nvmlEccCounterType_t(counterType),
         _nvmlMemoryLocation_t(locationType),
         byref(c_count),
     )
     check_return(ret)
     return c_count.value
 
 
 def nvmlDeviceGetUtilizationRates(handle):
-    """ """
+    """description"""
     c_util = c_nvmlUtilization_t()
     fn = get_func_pointer("nvmlDeviceGetUtilizationRates")
     ret = fn(handle, byref(c_util))
     check_return(ret)
     return c_util
 
 
 def nvmlDeviceGetEncoderUtilization(handle):
-    """ """
+    """description"""
     c_util = c_uint()
     c_samplingPeriod = c_uint()
     fn = get_func_pointer("nvmlDeviceGetEncoderUtilization")
     ret = fn(handle, byref(c_util), byref(c_samplingPeriod))
     check_return(ret)
     return [c_util.value, c_samplingPeriod.value]
 
 
 def nvmlDeviceGetDecoderUtilization(handle):
-    """ """
+    """description"""
     c_util = c_uint()
     c_samplingPeriod = c_uint()
     fn = get_func_pointer("nvmlDeviceGetDecoderUtilization")
     ret = fn(handle, byref(c_util), byref(c_samplingPeriod))
     check_return(ret)
     return [c_util.value, c_samplingPeriod.value]
 
 
 def nvmlDeviceGetPcieReplayCounter(handle):
-    """ """
+    """description"""
     c_replay = c_uint()
     fn = get_func_pointer("nvmlDeviceGetPcieReplayCounter")
     ret = fn(handle, byref(c_replay))
     check_return(ret)
     return c_replay.value
 
 
 def nvmlDeviceGetDriverModel(handle):
-    """ """
+    """description"""
     c_currModel = _nvmlDriverModel_t()
     c_pendingModel = _nvmlDriverModel_t()
     fn = get_func_pointer("nvmlDeviceGetDriverModel")
     ret = fn(handle, byref(c_currModel), byref(c_pendingModel))
     check_return(ret)
     return [c_currModel.value, c_pendingModel.value]
 
 
 # added to API
 def nvmlDeviceGetCurrentDriverModel(handle):
-    """ """
+    """description"""
     return nvmlDeviceGetDriverModel(handle)[0]
 
 
 # added to API
 def nvmlDeviceGetPendingDriverModel(handle):
-    """ """
+    """description"""
     return nvmlDeviceGetDriverModel(handle)[1]
 
 
 # Added in 2.285
 def nvmlDeviceGetVbiosVersion(handle):
-    """ """
+    """description"""
     c_version = create_string_buffer(NVML_DEVICE_VBIOS_VERSION_BUFFER_SIZE)
     fn = get_func_pointer("nvmlDeviceGetVbiosVersion")
     ret = fn(handle, c_version, c_uint(NVML_DEVICE_VBIOS_VERSION_BUFFER_SIZE))
     check_return(ret)
     return c_version.value
 
 
 # Added in 2.285
 def nvmlDeviceGetComputeRunningProcesses(handle):
-    """ """
+    """description"""
     # first call to get the size
     c_count = c_uint(0)
     fn = get_func_pointer("nvmlDeviceGetComputeRunningProcesses")
     ret = fn(handle, byref(c_count), None)
 
     if ret == NVML_SUCCESS:
         # special case, no running processes
@@ -1670,15 +1679,15 @@
         return procs
     else:
         # error case
         raise NVMLError(ret)
 
 
 def nvmlDeviceGetGraphicsRunningProcesses(handle):
-    """ """
+    """description"""
     # first call to get the size
     c_count = c_uint(0)
     fn = get_func_pointer("nvmlDeviceGetGraphicsRunningProcesses")
     ret = fn(handle, byref(c_count), None)
 
     if ret == NVML_SUCCESS:
         # special case, no running processes
@@ -1706,315 +1715,315 @@
         return procs
     else:
         # error case
         raise NVMLError(ret)
 
 
 def nvmlDeviceGetAutoBoostedClocksEnabled(handle):
-    """ """
+    """description"""
     c_isEnabled = _nvmlEnableState_t()
     c_defaultIsEnabled = _nvmlEnableState_t()
     fn = get_func_pointer("nvmlDeviceGetAutoBoostedClocksEnabled")
     ret = fn(handle, byref(c_isEnabled), byref(c_defaultIsEnabled))
     check_return(ret)
     return [c_isEnabled.value, c_defaultIsEnabled.value]
     # Throws NVML_ERROR_NOT_SUPPORTED if hardware doesn't support setting auto boosted clocks
 
 
 ## Set functions
 def nvmlUnitSetLedState(unit, color):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlUnitSetLedState")
     ret = fn(unit, _nvmlLedColor_t(color))
     check_return(ret)
     return None
 
 
 def nvmlDeviceSetPersistenceMode(handle, mode):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlDeviceSetPersistenceMode")
     ret = fn(handle, _nvmlEnableState_t(mode))
     check_return(ret)
     return None
 
 
 def nvmlDeviceSetComputeMode(handle, mode):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlDeviceSetComputeMode")
     ret = fn(handle, _nvmlComputeMode_t(mode))
     check_return(ret)
     return None
 
 
 def nvmlDeviceSetEccMode(handle, mode):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlDeviceSetEccMode")
     ret = fn(handle, _nvmlEnableState_t(mode))
     check_return(ret)
     return None
 
 
 def nvmlDeviceClearEccErrorCounts(handle, counterType):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlDeviceClearEccErrorCounts")
     ret = fn(handle, _nvmlEccCounterType_t(counterType))
     check_return(ret)
     return None
 
 
 def nvmlDeviceSetDriverModel(handle, model):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlDeviceSetDriverModel")
     ret = fn(handle, _nvmlDriverModel_t(model))
     check_return(ret)
     return None
 
 
 def nvmlDeviceSetAutoBoostedClocksEnabled(handle, enabled):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlDeviceSetAutoBoostedClocksEnabled")
     ret = fn(handle, _nvmlEnableState_t(enabled))
     check_return(ret)
     return None
     # Throws NVML_ERROR_NOT_SUPPORTED if hardware doesn't support setting auto boosted clocks
 
 
 def nvmlDeviceSetDefaultAutoBoostedClocksEnabled(handle, enabled, flags):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlDeviceSetDefaultAutoBoostedClocksEnabled")
     ret = fn(handle, _nvmlEnableState_t(enabled), c_uint(flags))
     check_return(ret)
     return None
     # Throws NVML_ERROR_NOT_SUPPORTED if hardware doesn't support setting auto boosted clocks
 
 
 # Added in 4.304
 def nvmlDeviceSetApplicationsClocks(handle, maxMemClockMHz, maxGraphicsClockMHz):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlDeviceSetApplicationsClocks")
     ret = fn(handle, c_uint(maxMemClockMHz), c_uint(maxGraphicsClockMHz))
     check_return(ret)
     return None
 
 
 # Added in 4.304
 def nvmlDeviceResetApplicationsClocks(handle):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlDeviceResetApplicationsClocks")
     ret = fn(handle)
     check_return(ret)
     return None
 
 
 # Added in 4.304
 def nvmlDeviceSetPowerManagementLimit(handle, limit):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlDeviceSetPowerManagementLimit")
     ret = fn(handle, c_uint(limit))
     check_return(ret)
     return None
 
 
 # Added in 4.304
 def nvmlDeviceSetGpuOperationMode(handle, mode):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlDeviceSetGpuOperationMode")
     ret = fn(handle, _nvmlGpuOperationMode_t(mode))
     check_return(ret)
     return None
 
 
 # Added in 2.285
 def nvmlEventSetCreate():
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlEventSetCreate")
     eventSet = c_nvmlEventSet_t()
     ret = fn(byref(eventSet))
     check_return(ret)
     return eventSet
 
 
 # Added in 2.285
 def nvmlDeviceRegisterEvents(handle, eventTypes, eventSet):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlDeviceRegisterEvents")
     ret = fn(handle, c_ulonglong(eventTypes), eventSet)
     check_return(ret)
     return None
 
 
 # Added in 2.285
 def nvmlDeviceGetSupportedEventTypes(handle):
-    """ """
+    """description"""
     c_eventTypes = c_ulonglong()
     fn = get_func_pointer("nvmlDeviceGetSupportedEventTypes")
     ret = fn(handle, byref(c_eventTypes))
     check_return(ret)
     return c_eventTypes.value
 
 
 # Added in 2.285
 # raises NVML_ERROR_TIMEOUT exception on timeout
 def nvmlEventSetWait(eventSet, timeoutms):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlEventSetWait")
     data = c_nvmlEventData_t()
     ret = fn(eventSet, byref(data), c_uint(timeoutms))
     check_return(ret)
     return data
 
 
 # Added in 2.285
 def nvmlEventSetFree(eventSet):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlEventSetFree")
     ret = fn(eventSet)
     check_return(ret)
     return None
 
 
 # Added in 3.295
 def nvmlDeviceOnSameBoard(handle1, handle2):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlDeviceOnSameBoard")
     onSameBoard = c_int()
     ret = fn(handle1, handle2, byref(onSameBoard))
     check_return(ret)
     return onSameBoard.value != 0
 
 
 # Added in 3.295
 def nvmlDeviceGetCurrPcieLinkGeneration(handle):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlDeviceGetCurrPcieLinkGeneration")
     gen = c_uint()
     ret = fn(handle, byref(gen))
     check_return(ret)
     return gen.value
 
 
 # Added in 3.295
 def nvmlDeviceGetMaxPcieLinkGeneration(handle):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlDeviceGetMaxPcieLinkGeneration")
     gen = c_uint()
     ret = fn(handle, byref(gen))
     check_return(ret)
     return gen.value
 
 
 # Added in 3.295
 def nvmlDeviceGetCurrPcieLinkWidth(handle):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlDeviceGetCurrPcieLinkWidth")
     width = c_uint()
     ret = fn(handle, byref(width))
     check_return(ret)
     return width.value
 
 
 # Added in 3.295
 def nvmlDeviceGetMaxPcieLinkWidth(handle):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlDeviceGetMaxPcieLinkWidth")
     width = c_uint()
     ret = fn(handle, byref(width))
     check_return(ret)
     return width.value
 
 
 # Added in 4.304
 def nvmlDeviceGetSupportedClocksThrottleReasons(handle):
-    """ """
+    """description"""
     c_reasons = c_ulonglong()
     fn = get_func_pointer("nvmlDeviceGetSupportedClocksThrottleReasons")
     ret = fn(handle, byref(c_reasons))
     check_return(ret)
     return c_reasons.value
 
 
 # Added in 4.304
 def nvmlDeviceGetCurrentClocksThrottleReasons(handle):
-    """ """
+    """description"""
     c_reasons = c_ulonglong()
     fn = get_func_pointer("nvmlDeviceGetCurrentClocksThrottleReasons")
     ret = fn(handle, byref(c_reasons))
     check_return(ret)
     return c_reasons.value
 
 
 # Added in 5.319
 def nvmlDeviceGetIndex(handle):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlDeviceGetIndex")
     c_index = c_uint()
     ret = fn(handle, byref(c_index))
     check_return(ret)
     return c_index.value
 
 
 # Added in 5.319
 def nvmlDeviceGetAccountingMode(handle):
-    """ """
+    """description"""
     c_mode = _nvmlEnableState_t()
     fn = get_func_pointer("nvmlDeviceGetAccountingMode")
     ret = fn(handle, byref(c_mode))
     check_return(ret)
     return c_mode.value
 
 
 def nvmlDeviceSetAccountingMode(handle, mode):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlDeviceSetAccountingMode")
     ret = fn(handle, _nvmlEnableState_t(mode))
     check_return(ret)
     return None
 
 
 def nvmlDeviceClearAccountingPids(handle):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlDeviceClearAccountingPids")
     ret = fn(handle)
     check_return(ret)
     return None
 
 
 def nvmlDeviceGetAccountingStats(handle, pid):
-    """ """
+    """description"""
     stats = c_nvmlAccountingStats_t()
     fn = get_func_pointer("nvmlDeviceGetAccountingStats")
     ret = fn(handle, c_uint(pid), byref(stats))
     check_return(ret)
     if stats.maxMemoryUsage == NVML_VALUE_NOT_AVAILABLE_ulonglong.value:
         # special case for WDDM on Windows, see comment above
         stats.maxMemoryUsage = None
     return stats
 
 
 def nvmlDeviceGetAccountingPids(handle):
-    """ """
+    """description"""
     count = c_uint(nvmlDeviceGetAccountingBufferSize(handle))
     pids = (c_uint * count.value)()
     fn = get_func_pointer("nvmlDeviceGetAccountingPids")
     ret = fn(handle, byref(count), pids)
     check_return(ret)
     return map(int, pids[0 : count.value])
 
 
 def nvmlDeviceGetAccountingBufferSize(handle):
-    """ """
+    """description"""
     bufferSize = c_uint()
     fn = get_func_pointer("nvmlDeviceGetAccountingBufferSize")
     ret = fn(handle, byref(bufferSize))
     check_return(ret)
     return int(bufferSize.value)
 
 
 def nvmlDeviceGetRetiredPages(device, sourceFilter):
-    """ """
+    """description"""
     c_source = _nvmlPageRetirementCause_t(sourceFilter)
     c_count = c_uint(0)
     fn = get_func_pointer("nvmlDeviceGetRetiredPages")
 
     # First call will get the size
     ret = fn(device, c_source, byref(c_count), None)
 
@@ -2030,50 +2039,50 @@
     c_pages = page_array()
     ret = fn(device, c_source, byref(c_count), c_pages)
     check_return(ret)
     return map(int, c_pages[0 : c_count.value])
 
 
 def nvmlDeviceGetRetiredPagesPendingStatus(device):
-    """ """
+    """description"""
     c_pending = _nvmlEnableState_t()
     fn = get_func_pointer("nvmlDeviceGetRetiredPagesPendingStatus")
     ret = fn(device, byref(c_pending))
     check_return(ret)
     return int(c_pending.value)
 
 
 def nvmlDeviceGetAPIRestriction(device, apiType):
-    """ """
+    """description"""
     c_permission = _nvmlEnableState_t()
     fn = get_func_pointer("nvmlDeviceGetAPIRestriction")
     ret = fn(device, _nvmlRestrictedAPI_t(apiType), byref(c_permission))
     check_return(ret)
     return int(c_permission.value)
 
 
 def nvmlDeviceSetAPIRestriction(handle, apiType, isRestricted):
-    """ """
+    """description"""
     fn = get_func_pointer("nvmlDeviceSetAPIRestriction")
     ret = fn(handle, _nvmlRestrictedAPI_t(apiType), _nvmlEnableState_t(isRestricted))
     check_return(ret)
     return None
 
 
 def nvmlDeviceGetBridgeChipInfo(handle):
-    """ """
+    """description"""
     bridgeHierarchy = c_nvmlBridgeChipHierarchy_t()
     fn = get_func_pointer("nvmlDeviceGetBridgeChipInfo")
     ret = fn(handle, byref(bridgeHierarchy))
     check_return(ret)
     return bridgeHierarchy
 
 
 def nvmlDeviceGetSamples(device, sampling_type, timeStamp):
-    """ """
+    """description"""
     c_sampling_type = _nvmlSamplingType_t(sampling_type)
     c_time_stamp = c_ulonglong(timeStamp)
     c_sample_count = c_uint(0)
     c_sample_value_type = _nvmlValueType_t()
     fn = get_func_pointer("nvmlDeviceGetSamples")
 
     ## First Call gets the size
@@ -2097,40 +2106,40 @@
         c_sampling_type,
         c_time_stamp,
         byref(c_sample_value_type),
         byref(c_sample_count),
         c_samples,
     )
     check_return(ret)
-    return (c_sample_value_type.value, c_samples[0 : c_sample_count.value])
+    return c_sample_value_type.value, c_samples[0 : c_sample_count.value]
 
 
 def nvmlDeviceGetViolationStatus(device, perfPolicyType):
-    """ """
+    """description"""
     c_perfPolicy_type = _nvmlPerfPolicyType_t(perfPolicyType)
     c_violTime = c_nvmlViolationTime_t()
     fn = get_func_pointer("nvmlDeviceGetViolationStatus")
 
     ## Invoke the method to get violation time
     ret = fn(device, c_perfPolicy_type, byref(c_violTime))
     check_return(ret)
     return c_violTime
 
 
 def nvmlDeviceGetPcieThroughput(device, counter):
-    """ """
+    """description"""
     c_util = c_uint()
     fn = get_func_pointer("nvmlDeviceGetPcieThroughput")
     ret = fn(device, _nvmlPcieUtilCounter_t(counter), byref(c_util))
     check_return(ret)
     return c_util.value
 
 
 def nvmlSystemGetTopologyGpuSet(cpuNumber):
-    """ """
+    """description"""
     c_count = c_uint(0)
     fn = get_func_pointer("nvmlSystemGetTopologyGpuSet")
 
     # First call will get the size
     ret = fn(cpuNumber, byref(c_count), None)
 
     if ret != NVML_SUCCESS:
@@ -2141,15 +2150,15 @@
     c_devices = device_array()
     ret = fn(cpuNumber, byref(c_count), c_devices)
     check_return(ret)
     return map(None, c_devices[0 : c_count.value])
 
 
 def nvmlDeviceGetTopologyNearestGpus(device, level):
-    """ """
+    """description"""
     c_count = c_uint(0)
     fn = get_func_pointer("nvmlDeviceGetTopologyNearestGpus")
 
     # First call will get the size
     ret = fn(device, level, byref(c_count), None)
 
     if ret != NVML_SUCCESS:
@@ -2160,15 +2169,15 @@
     c_devices = device_array()
     ret = fn(device, level, byref(c_count), c_devices)
     check_return(ret)
     return map(None, c_devices[0 : c_count.value])
 
 
 def nvmlDeviceGetTopologyCommonAncestor(device1, device2):
-    """ """
+    """description"""
     c_level = _nvmlGpuTopologyLevel_t()
     fn = get_func_pointer("nvmlDeviceGetTopologyCommonAncestor")
     ret = fn(device1, device2, byref(c_level))
     check_return(ret)
     return c_level.value
```

### Comparing `Heimdallr-0.2.7/heimdallr/utilities/nvidia/packing.py` & `heimdallr-0.2.8/heimdallr/utilities/nvidia/packing.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,26 +7,27 @@
            Created on 19/03/2020
            """
 
 import time
 from typing import List, Tuple
 
 import psutil
-from warg import NOD
-
 from heimdallr.utilities.nvidia import bindings
+from warg import NOD
 
 try:
     bindings.nvmlInit()
 except Exception as e:
     print(e)
 
 
 def get_nv_info(include_graphics_processes: bool = True) -> Tuple[str, List]:
-    """ """
+    """
+    Get NVidia GPU information
+    """
     devices = []
     try:
         driver_version = bindings.nvmlSystemGetDriverVersion().decode()
         device_count = bindings.nvmlDeviceGetCount()
 
         for device_i in range(device_count):
             handle = bindings.nvmlDeviceGetHandleByIndex(device_i)
```

### Comparing `Heimdallr-0.2.7/heimdallr/utilities/nvidia/smi_parsing.py` & `heimdallr-0.2.8/heimdallr/utilities/nvidia/smi_parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+__author__ = "Christian"
+__doc__ = r"""
+
+           Created on 29/03/2020
+           """
+
 # ============================================================================ #
 # Copyright (c) 2011-2019, NVIDIA Corporation.  All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 #    * Redistributions of source code must retain the above copyright notice,
@@ -337,21 +346,23 @@
 
 
 class NVMLError_NotSupported(Exception):
     pass
 
 
 class NvidiaSMI:
-    """ """
+    """
+    NvidiaSMI is a class for querying the NVIDIA SMI (System Management Interface)
+    """
 
     __instance = None
     __handles = None
 
     class loop_async:
-        """ """
+        """description"""
 
         __last_result = None
         __task = None
         __abort = False
         __callback_chain = None
 
         def __init__(self, time_in_milliseconds=1, filter=None, callback=None):
@@ -390,37 +401,37 @@
 
         def __callback(self, result):
             self.__last_result = result
             if self.__callback_chain is not None:
                 self.__callback_chain(self, result)
 
         def cancel(self):
-            """ """
+            """description"""
             self.__abort = True
             if self.__task is not None:
                 self.__task.join()
 
         def is_aborted(self):
-            """ """
+            """description"""
             return self.__abort
 
         def result(self):
-            """ """
+            """description"""
             return self.__last_result
 
     @staticmethod
     def getInstance():
         """Static access method."""
         if NvidiaSMI.__instance == None:
             NvidiaSMI()
         return NvidiaSMI.__instance
 
     @staticmethod
     def loop(time_in_milliseconds=1, filter=None, callback=None):
-        """ """
+        """description"""
         return NvidiaSMI.loop_async(time_in_milliseconds, filter, callback)
 
     def __init__(self):
         """Virtually private constructor."""
         if NvidiaSMI.__instance != None:
             raise Exception("This class is a singleton, use getInstance()")
         else:
@@ -944,15 +955,15 @@
 
         try:
             supportedClocksThrottleReasons = (
                 nvmlDeviceGetSupportedClocksThrottleReasons(handle)
             )
             clocksThrottleReasons = nvmlDeviceGetCurrentClocksThrottleReasons(handle)
             strResult += "    <clocks_throttle_reasons>\n"
-            for (mask, name) in throttleReasons:
+            for mask, name in throttleReasons:
                 if name != "clocks_throttle_reason_user_defined_clocks":
                     if mask & supportedClocksThrottleReasons:
                         val = "Active" if mask & clocksThrottleReasons else "Not Active"
                     else:
                         val = (
                             "N/A"  # nvidia_smi.__handleError(NVML_ERROR_NOT_SUPPORTED);
                         )
@@ -986,15 +997,15 @@
         clockThrottleReasons = {}
 
         try:
             supportedClocksThrottleReasons = (
                 nvmlDeviceGetSupportedClocksThrottleReasons(handle)
             )
             clocksThrottleReasons = nvmlDeviceGetCurrentClocksThrottleReasons(handle)
-            for (mask, name) in throttleReasons:
+            for mask, name in throttleReasons:
                 if name != "clocks_throttle_reason_user_defined_clocks":
                     if mask & supportedClocksThrottleReasons:
                         val = "Active" if mask & clocksThrottleReasons else "Not Active"
                     else:
                         val = (
                             "N/A"  # nvidia_smi.__handleError(NVML_ERROR_NOT_SUPPORTED);
                         )
@@ -1517,15 +1528,15 @@
                             strFwVersion = "N/A"
                         else:
                             strFwVersion = "%08X" % (
                                 bridgeHierarchy.bridgeChipInfo[0].fwVersion
                             )
                         pciBridgeChip += (
                             "        <bridge_chip_fw>%s</bridge_chip_fw>\n"
-                            % (strFwVersion)
+                            % strFwVersion
                         )
                     except NVMLError as err:
                         pciBridgeChip += (
                             "        <bridge_chip_type>"
                             + NvidiaSMI.__handleError(err)
                             + "</bridge_chip_type>\n"
                         )
@@ -1639,15 +1650,14 @@
                 includeMemoryUsage = False
                 if (
                     NVSMI_ALL in filter
                     or NVSMI_MEMORY_TOTAL in filter
                     or NVSMI_MEMORY_USED in filter
                     or NVSMI_MEMORY_FREE in filter
                 ):
-
                     includeMemoryUsage = True
                     try:
                         memInfo = nvmlDeviceGetMemoryInfo(handle)
                         mem_total = (
                             NvidiaSMI.__toString(memInfo.total / 1024 / 1024) + " MiB"
                         )
                         mem_used = (
@@ -2642,23 +2652,23 @@
                     includePci = True
 
                 if NVSMI_ALL in filter or NVSMI_PCI_DOMAIN in filter:
                     pci["pci_domain"] = "%04X" % pciInfo.domain
                     includePci = True
 
                 if NVSMI_ALL in filter or NVSMI_PCI_DEVICE_ID in filter:
-                    pci["pci_device_id"] = "%08X" % (pciInfo.pciDeviceId)
+                    pci["pci_device_id"] = "%08X" % pciInfo.pciDeviceId
                     includePci = True
 
                 if NVSMI_ALL in filter or NVSMI_PCI_BUS_ID in filter:
                     pci["pci_bus_id"] = NvidiaSMI.__toString(pciInfo.busId)
                     includePci = True
 
                 if NVSMI_ALL in filter or NVSMI_PCI_SUBDEVICE_ID in filter:
-                    pci["pci_sub_system_id"] = "%08X" % (pciInfo.pciSubSystemId)
+                    pci["pci_sub_system_id"] = "%08X" % pciInfo.pciSubSystemId
                     includePci = True
 
                 pciGpuLinkInfo = {}
                 includeLinkInfo = False
                 pciGen = {}
                 includeGen = False
 
@@ -2813,27 +2823,26 @@
                     or NVSMI_CLOCK_THROTTLE_REASONS_SW_PWR_CAP in filter
                     or NVSMI_CLOCK_THROTTLE_REASONS_HW_SLOWDOWN in filter
                     or NVSMI_CLOCK_THROTTLE_REASONS_HW_THERMAL_SLOWDOWN in filter
                     or NVSMI_CLOCK_THROTTLE_REASONS_HW_PWR_BRAKE_SLOWDOWN in filter
                     or NVSMI_CLOCK_THROTTLE_REASONS_SW_THERMAL_SLOWDOWN in filter
                     or NVSMI_CLOCK_THROTTLE_REASONS_SYNC_BOOST in filter
                 ):
-                    gpuResults[
-                        "clocks_throttle"
-                    ] = NvidiaSMI.__GetClocksThrottleReasons(handle)
+                    gpuResults["clocks_throttle"] = (
+                        NvidiaSMI.__GetClocksThrottleReasons(handle)
+                    )
 
                 fbMemoryUsage = {}
                 includeMemoryUsage = False
                 if (
                     NVSMI_ALL in filter
                     or NVSMI_MEMORY_TOTAL in filter
                     or NVSMI_MEMORY_USED in filter
                     or NVSMI_MEMORY_FREE in filter
                 ):
-
                     includeMemoryUsage = True
                     try:
                         memInfo = nvmlDeviceGetMemoryInfo(handle)
                         mem_total = memInfo.total / 1024 / 1024
                         mem_used = memInfo.used / 1024 / 1024
                         mem_free = (
                             memInfo.total / 1024 / 1024 - memInfo.used / 1024 / 1024
@@ -2900,15 +2909,14 @@
                 utilization = {}
                 includeUtilization = False
                 if (
                     NVSMI_ALL in filter
                     or NVSMI_UTILIZATION_GPU in filter
                     or NVSMI_UTILIZATION_MEM in filter
                 ):
-
                     try:
                         util = nvmlDeviceGetUtilizationRates(handle)
                         gpu_util = util.gpu
                         mem_util = util.memory
                     except NVMLError as err:
                         error = NvidiaSMI.__handleError(err)
                         gpu_util = error
@@ -3256,17 +3264,17 @@
                             try:
                                 clocks = nvmlDeviceGetSupportedGraphicsClocks(handle, m)
                                 for c in clocks:
                                     supportedGraphicsClocks.append(c)
                             except NVMLError as err:
                                 supportedGraphicsClocks = NvidiaSMI.__handleError(err)
 
-                            supportMemClock[
-                                "supported_graphics_clock"
-                            ] = supportedGraphicsClocks
+                            supportMemClock["supported_graphics_clock"] = (
+                                supportedGraphicsClocks
+                            )
 
                             supportedClocks.append(supportMemClock)
                     #                         jj+=1
 
                     except NVMLError as err:
                         supportedClocks["Error"] = NvidiaSMI.__handleError(err)
 
@@ -3369,66 +3377,66 @@
 
     def __to_str_dictionary(self, value, indent):
         strResults = ""
         try:
             for key, val in value.items():
                 if isinstance(val, collections.Mapping):
                     if len(val.values()) > 0:
-                        strResults += ("%s%s:\n") % (indent, key)
+                        strResults += "%s%s:\n" % (indent, key)
                         strResults += self.__to_str_dictionary(val, "  " + indent)
                     else:
-                        strResults += ("%s%s: %s\n") % (indent, key, "None")
+                        strResults += "%s%s: %s\n" % (indent, key, "None")
                 elif (type(val) is list) and (isinstance(val[0], collections.Mapping)):
                     for i in range(0, len(val)):
-                        strResults += ("%s%s: [%d of %d]\n") % (
+                        strResults += "%s%s: [%d of %d]\n" % (
                             indent,
                             key,
                             i + 1,
                             len(val),
                         )
                         strResults += self.__to_str_dictionary(val[i], "  " + indent)
                 else:
-                    strResults += ("%s%s: %s\n") % (indent, key, str(val))
+                    strResults += "%s%s: %s\n" % (indent, key, str(val))
 
         except Exception as e:
             strResults += "\n[Error] " + str(e)
 
         return strResults
 
     def __to_str(self, results):
         strResults = ""
         indent = "  "
         for key, val in results.items():
             if type(val) is list:
                 for i in range(0, len(val)):
-                    strResults += ("%s%s: [%d of %d]\n") % (
+                    strResults += "%s%s: [%d of %d]\n" % (
                         indent,
                         key,
                         i + 1,
                         len(val),
                     )
                     strResults += self.__to_str_dictionary(val[i], "  " + indent)
             else:
-                strResults += ("%s%s: %s\n") % (indent, key, str(val))
+                strResults += "%s%s: %s\n" % (indent, key, str(val))
 
         return strResults
 
     def format(self, results):
-        """ """
+        """description"""
         if type(results) is str:
             return results
 
         return self.__to_str(results)
 
 
 # this is not exectued when module is imported
 if __name__ == "__main__":
 
     def main():
-        """ """
+        """description"""
         # evaluate arguments
         as_xml = False
         query_gpu_args = None
         for i in range(1, len(sys.argv)):
             v = sys.argv[i]
             if v.lower() == "xml":
                 as_xml = True
@@ -3437,11 +3445,10 @@
 
         # execute device query
         nvsmi = NvidiaSMI.getInstance()
         if as_xml:
             results = nvsmi.XmlDeviceQuery(query_gpu_args)
         else:
             results = nvsmi.DeviceQuery(query_gpu_args)
-
-        print(nvsmi.format(results))
+            print(nvsmi.format(results))
 
     main()
```

### Comparing `Heimdallr-0.2.7/heimdallr/utilities/publisher/system_resources.py` & `heimdallr-0.2.8/heimdallr/utilities/publisher/system_resources.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,32 +3,21 @@
 
 __author__ = "Christian"
 __doc__ = r"""
 
            Created on 29/03/2020
            """
 
-from typing import Dict, Mapping, Tuple
+from typing import Dict, Tuple
 
 import psutil
 
 __all__ = ["get_list_of_process_sorted_by_memory"]
 
-
-def select(mapping: Mapping, *a) -> Mapping:
-    """
-
-    Args:
-      mapping:
-      *a:
-
-    Returns:
-
-    """
-    return {k: v for k, v in mapping.items() if k in a}
+from warg.generators.mapping_generator import select_dict
 
 
 def get_list_of_process_sorted_by_memory(
     attrs: Tuple = ("name", "username"), scaling: float = (1024**2), top_k: int = 10
 ) -> Dict:
     """
     Get list of running process sorted by Memory Usage
@@ -42,33 +31,33 @@
         except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
             pass
     sorted_entries = sorted(
         list_of_proc_objects, key=lambda proc_obj: proc_obj["vms"], reverse=True
     )
     if top_k:
         sorted_entries = sorted_entries[:top_k]
-    return {v["pid"]: select(v, "vms", *attrs) for v in sorted_entries}
+    return {v["pid"]: select_dict(v, "vms", *attrs) for v in sorted_entries}
 
 
 if __name__ == "__main__":
 
     def main():
-        """ """
+        """description"""
         print("*** Iterate over all running process and print process ID & Name ***")
         for proc in psutil.process_iter():
             try:
                 process_name = proc.name()
                 process_id = proc.pid
                 print(process_name, " ::: ", process_id)
             except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
                 pass
         print("*** Create a list of all running processes ***")
 
     def all_info_procs():
-        """ """
+        """description"""
         list_of_process_names = list()
         for proc in psutil.process_iter():
             p_info_dict = proc.as_dict()
             list_of_process_names.append(p_info_dict)
         for elem in list_of_process_names:
             print(elem)
```

### Comparing `Heimdallr-0.2.7/heimdallr/utilities/publisher/unpacking.py` & `heimdallr-0.2.8/heimdallr/utilities/publisher/unpacking.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,42 @@
-from warg import NOD
+# !/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+__author__ = "Christian"
+__doc__ = r"""
+
+           Created on 29/03/2020
+           """
 
 from heimdallr.utilities.nvidia.packing import get_nv_info
+from warg import NOD
 
 
 def pull_gpu_info(include_graphics_processes: bool = True) -> dict:
     """Get all information about all your graphics cards.
 
     Returns:
       dict: The returned result is a dict with 3 keys: count, driver_version and devices:
           count: Number of gpus found
           driver_version: The version of the system’s graphics driver
           devices: It's a list and every item is a namedtuple Device which has 10 fields, for exzample id,
           name and fan_speed etc.
-                   It should be noted that the Process field is also a namedtuple which has 11 fields."""
+                   It should be noted that the Process field is also a namedtuple which has 11 fields.
+    """
 
     driver_version, devices = get_nv_info(include_graphics_processes)
 
     info = NOD()
 
     info["count"] = len(devices)
     info["driver_version"] = driver_version
     info["devices"] = devices
     return info.as_dict()
 
 
 def pull_disk_usage_info() -> dict:
+    """
+
+    :return:
+    :rtype:
+    """
     return {"disk_usage": {"total": 0, "used": 0, "free": 0}}
```

### Comparing `Heimdallr-0.2.7/heimdallr/utilities/publisher/windows_task_scheduler_utilities.py` & `heimdallr-0.2.8/heimdallr/utilities/publisher/windows_task_scheduler_utilities.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,64 @@
-__all__ = ["disable_service", "remove_service", "install_service", "enable_service"]
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+__author__ = "Christian"
+__doc__ = r"""
 
-from pathlib import Path
+           Created on 29/03/2020
+           """
+
+__all__ = ["disable_service", "remove_service", "install_service", "enable_service"]
 
 from draugr.os_utilities.windows_utilities import (
     delete_task,
     new_user_logon_execute_task,
     set_task_activity,
 )
 
 
 def disable_service(service_name: str) -> None:
     """
+    disable service
 
     Args:
       service_name:
     """
     set_task_activity(service_name, False)
 
 
 def enable_service(service_name: str) -> None:
     """
+    enable service
 
     Args:
       service_name:
     """
     set_task_activity(service_name, True)
 
 
-def install_service(service_entry_point_path: Path, service_name: str) -> None:
+def install_service(service_name: str) -> None:
     """
+    install service
 
     Args:
-      service_entry_point_path:
       service_name:
     """
+
     new_user_logon_execute_task(
         service_name,
         service_name,
         "python.exe",  # cmd.exe python.exe .....
         "-m heimdallr publish",
     )
 
 
 def remove_service(service_name) -> None:
     """
+    remove service
 
     Args:
       service_name:
     """
     delete_task(service_name)
```

### Comparing `Heimdallr-0.2.7/heimdallr/utilities/server/du_utilities.py` & `heimdallr-0.2.8/heimdallr/utilities/server/du_utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,40 @@
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+__author__ = "Christian"
+__doc__ = r"""
+
+           Created on 29/03/2020
+           """
+
 from typing import Mapping
 
 import numpy
 import pandas
-from pandas import DataFrame
-
 from heimdallr.configuration.heimdallr_config import (
     DROP_COLUMNS,
     INT_COLUMNS,
     MB_COLUMNS,
     PERCENT_COLUMNS,
 )
 from heimdallr.utilities.date_tools import timestamp_to_datetime
+from pandas import DataFrame
 
 MB_DIVISOR = int(1024**2)
 
 __all__ = [
     "to_overall_du_process_df",
 ]
 
 
 def to_overall_du_process_df(gpu_stats: Mapping) -> DataFrame:
-    """ """
+    """
+    to overall disk usage process df
+    """
     resulta = []
     columns = []
     if len(gpu_stats):
         for k2, v2 in gpu_stats.items():
             if "partitions" in v2:
                 for part_i in v2["partitions"]:
                     df = pandas.DataFrame(data=part_i)
```

### Comparing `Heimdallr-0.2.7/heimdallr/utilities/server/github_org_generators.py` & `heimdallr-0.2.8/heimdallr/utilities/server/github_org_generators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,26 @@
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+__author__ = "Christian"
+__doc__ = r"""
+
+           Created on 29/03/2020
+           """
+
+import calendar
+
 # https://github.com/pulls?q=is%3Aopen+is%3Apr+user%3Aaivclab+archived%3Afalse+
 # https://github.com/pulls?user=aivclab
 from datetime import datetime, timedelta
 from enum import Enum
 from typing import Generator, Iterable, List, Union
 
 from github import Github  # pip install PyGithub
-from github.GithubObject import NotSet
+from github.GithubObject import _NotSetType
 from github.Issue import Issue
 from github.Label import Label
 from github.Milestone import Milestone
 from github.NamedUser import NamedUser
 from github.PullRequest import PullRequest
 from github.Repository import Repository
 from sorcery import assigned_names
@@ -92,23 +103,23 @@
     :param org_name:
     """
     yield from yield_prs(yield_org_repos(g, org_name))
 
 
 def yield_issues(
     iterable: Iterable[Repository],
-    milestone: Union[Milestone, str] = NotSet,
+    milestone: Union[Milestone, str] = _NotSetType,
     state: Union[str, StateEnum] = StateEnum.open,
-    assignee: Union[NamedUser, str] = NotSet,
-    mentioned: NamedUser = NotSet,
-    labels: Union[List[str], List[Label]] = NotSet,
+    assignee: Union[NamedUser, str] = _NotSetType,
+    mentioned: NamedUser = _NotSetType,
+    labels: Union[List[str], List[Label]] = _NotSetType,
     sort: Union[str, IssueSortEnum] = IssueSortEnum.updated,
     direction: Union[str, DirectionEnum] = DirectionEnum.desc,
-    since: datetime = NotSet,  # datetime.now(),
-    creator: Union[str, NamedUser] = NotSet,
+    since: datetime = _NotSetType,  # datetime.now(),
+    creator: Union[str, NamedUser] = _NotSetType,
 ) -> Generator[Issue, None, None]:
     """
 
     Read more: https://docs.github.com/en/rest/reference/issues#list-issues-assigned-to-the-authenticated-user--parameters
 
     Args:
       iterable:
@@ -143,16 +154,16 @@
 
 
 def yield_prs(
     iterable: Iterable[Repository],
     state: Union[str, StateEnum] = StateEnum.open,
     sort: Union[str, PullRequestSortEnum] = PullRequestSortEnum.updated,
     direction: Union[str, DirectionEnum] = DirectionEnum.desc,
-    base: str = NotSet,
-    head: str = NotSet,
+    base: str = _NotSetType,
+    head: str = _NotSetType,
 ) -> Generator[PullRequest, None, None]:
     """
 
     Read more: https://docs.github.com/en/rest/reference/pulls#list-pull-requests--parameters
 
     Args:
       iterable:
@@ -189,17 +200,14 @@
     :return:
     """
     return (
         g.get_organization(org_name).get_repo(repo_name).get_pull(pull_request_number)
     )
 
 
-import calendar
-
-
 def utc_to_epoch(timestamp):  # Timestamp is a datetime object in UTC time
     """
 
     :param timestamp:
     :return:
     """
     return calendar.timegm(timestamp.utctimetuple())
```

### Comparing `Heimdallr-0.2.7/heimdallr/utilities/server/google_calendar.py` & `heimdallr-0.2.8/heimdallr/utilities/server/google_calendar.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,30 @@
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+__author__ = "Christian"
+__doc__ = r"""
+
+           Created on 29/03/2020
+           """
+
 import datetime
 import pickle
 from pathlib import Path
 
 import pandas
 from google.auth.transport.requests import Request
 from google_auth_oauthlib.flow import InstalledAppFlow
 
 try:
     from googleapiclient.discovery import build
 except:
-    print("try upgrade googleapiclient")
+    print("try upgrade google-api-python-client")
 
-from apppath import ensure_existence
+from warg import ensure_existence
 from heimdallr.configuration.heimdallr_settings import HeimdallrSettings
 from heimdallr.utilities.date_tools import iso_dt_to_datetime
 
 __all__ = ["get_calender_df"]
 
 SCOPES = ["https://www.googleapis.com/auth/calendar.readonly"]
```

### Comparing `Heimdallr-0.2.7/heimdallr/utilities/server/gpu_utilities.py` & `heimdallr-0.2.8/heimdallr/utilities/server/gpu_utilities.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,50 @@
-"""Function to get GPU information.
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+__author__ = "Christian"
+__doc__ = r"""
+
+           Created on 29/03/2020
+           Function to get GPU information.
 """
 
 from typing import List, Mapping, Sequence
 
 import numpy
 import pandas
 from dash import html
 from dash.dcc import Graph
 from dash.html import Div, H3
-from pandas import DataFrame
-from plotly import graph_objs
-from warg import Number
-
 from heimdallr.configuration.heimdallr_config import (
     DROP_COLUMNS,
     INT_COLUMNS,
     MB_COLUMNS,
     PERCENT_COLUMNS,
 )
 from heimdallr.utilities.date_tools import timestamp_to_datetime
 from heimdallr.utilities.publisher.unpacking import pull_gpu_info
+from pandas import DataFrame
+from plotly import graph_objs
+from warg import Number
 
 MB_DIVISOR = int(1024**2)
 
 __all__ = [
     "to_overall_gpu_process_df",
     "per_machine_per_device_pie_charts",
 ]
 
 
 def to_overall_gpu_process_df(
     gpu_stats: Mapping, sort_by_key="used_gpu_mem"
 ) -> DataFrame:
-    """ """
+    """
+    to overall gpu usage process df
+    """
     resulta = []
     columns = []
     if len(gpu_stats):
         for k2, v2 in gpu_stats.items():
             device_info = v2["devices"]
             for device_i in device_info:
                 processes = device_i["processes"]
@@ -68,15 +76,17 @@
 
     return out_df
 
 
 def per_machine_per_device_pie_charts(
     gpu_stats: Mapping, keep_alive: Sequence[Number]
 ) -> List[html.Div]:
-    """ """
+    """
+    per machine per device pie charts
+    """
     compute_machines = []
     for machine_name, machine in gpu_stats.items():
         machine_devices = []
         devices = machine["devices"]
 
         for i, d in enumerate(devices):
             used = d["used"] // MB_DIVISOR
```

### Comparing `Heimdallr-0.2.7/heimdallr/utilities/server/teams_status.py` & `heimdallr-0.2.8/heimdallr/utilities/server/slack_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,30 @@
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+__author__ = "Christian"
+__doc__ = r"""
+
+           Created on 29/03/2020
+           """
+
 import json
 import logging
 import random
 from typing import List
 
-import msal
 import requests
 
-__all__ = ["team_members_status"]
+__all__ = ["slack_members_status"]
 
 from dash import html
 from dash.html import Div, H3, H4, H2
 
 
-def team_members_status(access_token) -> List[html.Div]:
+def slack_members_status(access_token) -> List[html.Div]:
     """
     Get the status of all teams in the tenant
     """
     members = []
     for i in range(4):
         members.append(
             Div(
@@ -44,17 +52,18 @@
                 className="col p-1",
             )
         )
     return members
 
 
 if __name__ == "__main__":
-
     from exclude.calendar_app.tutorial.set_teams_config import s
 
+    import msal
+
     app = msal.ConfidentialClientApplication(
         s.teams_client_id,
         authority=s.teams_authority,
         client_credential=s.teams_secret,
         # token_cache=...  # Default cache is in memory only.
         # You can learn how to use SerializableTokenCache from
         # https://msal-python.rtfd.io/en/latest/#msal.SerializableTokenCache
```

### Comparing `Heimdallr-0.2.7/setup.py` & `heimdallr-0.2.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,51 +2,51 @@
 # -*- coding: utf-8 -*-
 import re
 from typing import List, Sequence, Union
 
 from setuptools import find_packages, setup
 
 
-def python_version_check(major: int = 3, minor: int = 7) -> None:
-    """ """
+def python_version_check(major: int = 3, minor: int = 8) -> None:
+    """description"""
     import sys
 
     assert sys.version_info.major == major and sys.version_info.minor >= minor, (
         f"This project is utilises language features only present Python {major}.{minor} and greater. "
         f"You are running {sys.version_info}."
     )
 
 
 python_version_check()
 
 from pathlib import Path
 
 
 def read_reqs(file: str, path: Path) -> List[str]:
-    """ """
+    """description"""
 
     def readlines_ignore_comments(f):
-        """ """
+        """description"""
         return [a_ for a_ in f.readlines() if "#" not in a_ and a_]
 
     def recursive_flatten_ignore_str(seq: Sequence) -> Sequence:
-        """ """
+        """description"""
         if not seq:  # is empty Sequence
             return seq
         if isinstance(seq[0], str):
             return seq
         if isinstance(seq[0], Sequence):
             return (
                 *recursive_flatten_ignore_str(seq[0]),
                 *recursive_flatten_ignore_str(seq[1:]),
             )
-        return (*seq[:1], *recursive_flatten_ignore_str(seq[1:]))
+        return *seq[:1], *recursive_flatten_ignore_str(seq[1:])
 
     def unroll_nested_reqs(req_str: str, base_path: Path):
-        """ """
+        """description"""
         if req_str.startswith("-r"):
             with open(base_path / req_str.strip("-r").strip()) as f:
                 return [
                     unroll_nested_reqs(req.strip(), base_path)
                     for req in readlines_ignore_comments(f)
                 ]
         else:
@@ -75,89 +75,89 @@
     version = re.search(rf"__version__ = {str_reg_exp}", content, re.M).group(1)
     project_name = re.search(rf"__project__ = {str_reg_exp}", content, re.M).group(1)
     author = re.search(rf"__author__ = {str_reg_exp}", content, re.M).group(1)
 __author__ = author
 
 
 class HeimdallrPackage:
-    """ """
+    """description"""
 
     @property
     def test_dependencies(self) -> list:
         return read_reqs(
             "requirements_tests.txt", Path(__file__).parent / "requirements"
         )
 
     @property
     def setup_dependencies(self) -> list:
-        """ """
+        """description"""
         return read_reqs("requirements_dev.txt", Path(__file__).parent / "requirements")
 
     @property
     def package_name(self) -> str:
-        """ """
+        """description"""
         return project_name
 
     @property
     def url(self) -> str:
-        """ """
+        """description"""
         return "https://github.com/aivclab/heimdallr"
 
     @property
     def download_url(self) -> str:
-        """ """
+        """description"""
         return self.url + "/releases"
 
     @property
     def readme_type(self) -> str:
-        """ """
+        """description"""
         return "text/markdown"
 
     @property
     def packages(self) -> List[Union[str, bytes]]:
-        """ """
+        """description"""
         return find_packages(
             exclude=[
                 # 'Path/To/Exclude'
             ]
         )
 
     @property
     def author_name(self) -> str:
-        """ """
+        """description"""
         return author
 
     @property
     def author_email(self) -> str:
-        """ """
+        """description"""
         return "christian.heider@alexandra.dk"
 
     @property
     def maintainer_name(self) -> str:
-        """ """
+        """description"""
         return self.author_name
 
     @property
     def maintainer_email(self) -> str:
-        """ """
+        """description"""
         return self.author_email
 
     @property
     def package_data(self) -> dict:
-        """ """
+        """description"""
         # data = glob.glob('data/', recursive=True)
         return {
             # 'PackageName':[
             # *data
             #  ]
         }
 
     @property
     def entry_points(self) -> dict:
-        """ """
+        """description"""
         return {
             "console_scripts": [
                 # "name_of_executable = module.with:function_to_execute"
                 "heimdallr = heimdallr.entry_points.cli:main",
                 "heimdallr-repl = heimdallr.entry_points.repl:main",
                 "heimdallr-publish = heimdallr.entry_points.publisher:main",
                 "heimdallr-server = heimdallr.entry_points.server:main",
@@ -188,42 +188,42 @@
             all_dependencies += these_extras[group_name]
         these_extras["all"] = list(set(all_dependencies))
 
         return these_extras
 
     @property
     def requirements(self) -> List[str]:
-        """ """
+        """description"""
         return read_reqs("requirements.txt", Path(__file__).parent)
 
     @property
     def description(self) -> str:
-        """ """
+        """description"""
         return "A package for hosting and connecting to a live dashboard"
 
     @property
     def readme(self) -> str:
-        """ """
+        """description"""
         with open("README.md", encoding="utf8") as f:
             return f.read()
 
     @property
     def keyword(self) -> str:
-        """ """
+        """description"""
         with open("KEYWORDS.md") as f:
             return f.read()
 
     @property
     def license(self) -> str:
-        """ """
+        """description"""
         return "Apache License, Version 2.0"
 
     @property
     def classifiers(self) -> List[str]:
-        """ """
+        """description"""
         return [
             "Development Status :: 4 - Beta",
             "Environment :: Console",
             "Intended Audience :: End Users/Desktop",
             "Intended Audience :: Developers",
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: MacOS :: MacOS X",
@@ -234,15 +234,15 @@
             "Natural Language :: English",
             # 'Topic :: Scientific/Engineering :: Artificial Intelligence'
             # 'Topic :: Software Development :: Bug Tracking',
         ]
 
     @property
     def version(self) -> str:
-        """ """
+        """description"""
         return version
 
 
 if __name__ == "__main__":
     pkg = HeimdallrPackage()
 
     setup(
```

### Comparing `Heimdallr-0.2.7/tests/test_nvml.py` & `heimdallr-0.2.8/tests/test_nvml.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 import sys
 import time
 from distutils.version import LooseVersion
 
 import pytest
 
-if sys.platform == "linux":
+SKIP_TEST = True
+
+if sys.platform == "linux" and not SKIP_TEST:
     print("Linux system detected")
     import pynvml
 
     NVML_PCIE_UTIL_TX_BYTES = pynvml.NVML_PCIE_UTIL_TX_BYTES
     NVML_PCIE_UTIL_RX_BYTES = pynvml.NVML_PCIE_UTIL_RX_BYTES
     NVML_PCIE_UTIL_COUNT = pynvml.NVML_PCIE_UTIL_COUNT
 
@@ -53,335 +55,323 @@
                     == pynvml.NVML_SUCCESS
                 )
                 error_count = pynvml.nvmlDeviceGetNvLinkErrorCounter(
                     handles[i], j, error_type
                 )
                 assert error_count >= 0
 
+    # Fixture to initialize and finalize nvml
+    @pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
+    @pytest.fixture(scope="module")
+    def nvml(request):
+        """description"""
+        pynvml.nvmlInit()
+
+        def nvml_close():
+            """description"""
+            pynvml.nvmlShutdown()
+
+        request.addfinalizer(nvml_close)
+
+    # Get GPU count
+    @pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
+    @pytest.fixture
+    def ngpus(nvml):
+        """description"""
+        result = pynvml.nvmlDeviceGetCount()
+        assert result > 0
+        print("[" + str(result) + " GPUs]", end=" ")
+        return result
+
+    # Get handles using pynvml.nvmlDeviceGetHandleByIndex
+    @pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
+    @pytest.fixture
+    def handles(ngpus):
+        """description"""
+        handles = [pynvml.nvmlDeviceGetHandleByIndex(i) for i in range(ngpus)]
+        assert len(handles) == ngpus
+        return handles
+
+    @pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
+    @pytest.fixture
+    def serials(ngpus, handles):
+        """description"""
+        serials = [pynvml.nvmlDeviceGetSerial(handles[i]) for i in range(ngpus)]
+        assert len(serials) == ngpus
+        return serials
+
+    @pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
+    @pytest.fixture
+    def uuids(ngpus, handles):
+        """description"""
+        uuids = [pynvml.nvmlDeviceGetUUID(handles[i]) for i in range(ngpus)]
+        assert len(uuids) == ngpus
+        return uuids
+
+    @pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
+    @pytest.fixture
+    def pci_info(ngpus, handles):
+        """description"""
+        pci_info = [pynvml.nvmlDeviceGetPciInfo(handles[i]) for i in range(ngpus)]
+        assert len(pci_info) == ngpus
+        return pci_info
+
+    ## ---------------------------- ##
+    ## Start Fucntion-pointer Tests ##
+    ## ---------------------------- ##
+
+    # Test pynvml.nvmlSystemGetNVMLVersion
+    @pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
+    def test_nvml_system_get_nvml_version(nvml):
+        vsn = 0.0
+        vsn = pynvml.nvmlSystemGetNVMLVersion().decode()
+        print("[NVML Version: " + vsn + "]", end=" ")
+        assert vsn > LooseVersion("0.0")
 
-# Fixture to initialize and finalize nvml
-@pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
-@pytest.fixture(scope="module")
-def nvml(request):
-    """ """
-    pynvml.nvmlInit()
-
-    def nvml_close():
-        """ """
-        pynvml.nvmlShutdown()
-
-    request.addfinalizer(nvml_close)
-
-
-# Get GPU count
-@pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
-@pytest.fixture
-def ngpus(nvml):
-    """ """
-    result = pynvml.nvmlDeviceGetCount()
-    assert result > 0
-    print("[" + str(result) + " GPUs]", end=" ")
-    return result
-
-
-# Get handles using pynvml.nvmlDeviceGetHandleByIndex
-@pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
-@pytest.fixture
-def handles(ngpus):
-    """ """
-    handles = [pynvml.nvmlDeviceGetHandleByIndex(i) for i in range(ngpus)]
-    assert len(handles) == ngpus
-    return handles
-
-
-@pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
-@pytest.fixture
-def serials(ngpus, handles):
-    """ """
-    serials = [pynvml.nvmlDeviceGetSerial(handles[i]) for i in range(ngpus)]
-    assert len(serials) == ngpus
-    return serials
-
-
-@pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
-@pytest.fixture
-def uuids(ngpus, handles):
-    """ """
-    uuids = [pynvml.nvmlDeviceGetUUID(handles[i]) for i in range(ngpus)]
-    assert len(uuids) == ngpus
-    return uuids
-
-
-@pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
-@pytest.fixture
-def pci_info(ngpus, handles):
-    """ """
-    pci_info = [pynvml.nvmlDeviceGetPciInfo(handles[i]) for i in range(ngpus)]
-    assert len(pci_info) == ngpus
-    return pci_info
-
-
-## ---------------------------- ##
-## Start Fucntion-pointer Tests ##
-## ---------------------------- ##
-
-# Test pynvml.nvmlSystemGetNVMLVersion
-@pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
-def test_nvmlSystemGetNVMLVersion(nvml):
-    vsn = 0.0
-    vsn = pynvml.nvmlSystemGetNVMLVersion().decode()
-    print("[NVML Version: " + vsn + "]", end=" ")
-    assert vsn > LooseVersion("0.0")
-
-
-# Test pynvml.nvmlSystemGetProcessName
-@pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
-def test_nvmlSystemGetProcessName(nvml):
-    procname = None
-    procname = pynvml.nvmlSystemGetProcessName(os.getpid())
-    print("[Process: " + str(procname.decode()) + "]", end=" ")
-    assert procname != None
-
-
-# Test pynvml.nvmlSystemGetDriverVersion
-@pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
-def test_nvmlSystemGetDriverVersion(nvml):
-    vsn = 0.0
-    vsn = pynvml.nvmlSystemGetDriverVersion().decode()
-    print("[Driver Version: " + vsn + "]", end=" ")
-    assert vsn > LooseVersion("0.0")  # Developing with 396.44
-
-
-## Unit "Get" Functions (Skipping for now) ##
-
-## Device "Get" Functions (Note: Some functions are fixtures, above) ##
-
-# Test pynvml.nvmlDeviceGetHandleBySerial
-@pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
-def test_nvmlDeviceGetHandleBySerial(ngpus, serials):
-    handles = [pynvml.nvmlDeviceGetHandleBySerial(serials[i]) for i in range(ngpus)]
-    assert len(handles) == ngpus
-
-
-# Test pynvml.nvmlDeviceGetHandleByUUID
-@pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
-def test_nvmlDeviceGetHandleByUUID(ngpus, uuids):
-    handles = [pynvml.nvmlDeviceGetHandleByUUID(uuids[i]) for i in range(ngpus)]
-    assert len(handles) == ngpus
-
-
-# Test pynvml.nvmlDeviceGetHandleByPciBusId
-@pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
-def test_nvmlDeviceGetHandleByPciBusId(ngpus, pci_info):
-    handles = [
-        pynvml.nvmlDeviceGetHandleByPciBusId(pci_info[i].busId) for i in range(ngpus)
-    ]
-    assert len(handles) == ngpus
-
-
-# [Skipping] pynvml.nvmlDeviceGetName
-# [Skipping] pynvml.nvmlDeviceGetBoardId
-# [Skipping] pynvml.nvmlDeviceGetMultiGpuBoard
-# [Skipping] pynvml.nvmlDeviceGetBrand
-# [Skipping] pynvml.nvmlDeviceGetCpuAffinity
-# [Skipping] pynvml.nvmlDeviceSetCpuAffinity
-# [Skipping] pynvml.nvmlDeviceClearCpuAffinity
-# [Skipping] pynvml.nvmlDeviceGetMinorNumber
-# [Skipping] pynvml.nvmlDeviceGetUUID
-# [Skipping] pynvml.nvmlDeviceGetInforomVersion
-# [Skipping] pynvml.nvmlDeviceGetInforomImageVersion
-# [Skipping] pynvml.nvmlDeviceGetInforomConfigurationChecksum
-# [Skipping] pynvml.nvmlDeviceValidateInforom
-# [Skipping] pynvml.nvmlDeviceGetDisplayMode
-# [Skipping] pynvml.nvmlDeviceGetPersistenceMode
-# [Skipping] pynvml.nvmlDeviceGetClockInfo
-# [Skipping] pynvml.nvmlDeviceGetMaxClockInfo
-# [Skipping] pynvml.nvmlDeviceGetApplicationsCloc
-# [Skipping] pynvml.nvmlDeviceGetDefaultApplicationsClock
-# [Skipping] pynvml.nvmlDeviceGetSupportedMemoryClocks
-# [Skipping] pynvml.nvmlDeviceGetSupportedGraphicsClocks
-# [Skipping] pynvml.nvmlDeviceGetFanSpeed
-# [Skipping] pynvml.nvmlDeviceGetTemperature
-# [Skipping] pynvml.nvmlDeviceGetTemperatureThreshold
-# [Skipping] pynvml.nvmlDeviceGetPowerState
-# [Skipping] pynvml.nvmlDeviceGetPerformanceState
-# [Skipping] pynvml.nvmlDeviceGetPowerManagementMode
-# [Skipping] pynvml.nvmlDeviceGetPowerManagementLimit
-# [Skipping] pynvml.nvmlDeviceGetPowerManagementLimitConstraints
-# [Skipping] pynvml.nvmlDeviceGetPowerManagementDefaultLimit
-# [Skipping] pynvml.nvmlDeviceGetEnforcedPowerLimit
-
-# Test pynvml.nvmlDeviceGetPowerUsage
-@pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
-def test_nvmlDeviceGetPowerUsage(ngpus, handles):
-    for i in range(ngpus):
-        power_mWatts = pynvml.nvmlDeviceGetPowerUsage(handles[i])
-        assert power_mWatts >= 0.0
-
-
-# Test pynvml.nvmlDeviceGetTotalEnergyConsumption
-@pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
-def test_nvmlDeviceGetTotalEnergyConsumption(ngpus, handles):
-    for i in range(ngpus):
-        energy_mJoules1 = pynvml.nvmlDeviceGetTotalEnergyConsumption(handles[i])
-        for j in range(10):  # idle for 150 ms
-            time.sleep(0.015)  # and check for increase every 15 ms
-            energy_mJoules2 = pynvml.nvmlDeviceGetTotalEnergyConsumption(handles[i])
-            assert energy_mJoules2 >= energy_mJoules1
-            if energy_mJoules2 > energy_mJoules1:
-                break
-        else:
-            assert False, "energy did not increase across 150 ms interval"
-
-
-# [Skipping] pynvml.nvmlDeviceGetGpuOperationMode
-# [Skipping] pynvml.nvmlDeviceGetCurrentGpuOperationMode
-# [Skipping] pynvml.nvmlDeviceGetPendingGpuOperationMode
-
-# Test pynvml.nvmlDeviceGetMemoryInfo
-@pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
-def test_nvmlDeviceGetMemoryInfo(ngpus, handles):
-    for i in range(ngpus):
-        meminfo = pynvml.nvmlDeviceGetMemoryInfo(handles[i])
-        assert (meminfo.used <= meminfo.total) and (meminfo.free <= meminfo.total)
-
-
-# [Skipping] pynvml.nvmlDeviceGetBAR1MemoryInfo
-# [Skipping] pynvml.nvmlDeviceGetComputeMode
-# [Skipping] pynvml.nvmlDeviceGetEccMode
-# [Skipping] pynvml.nvmlDeviceGetCurrentEccMode (Python API Addition)
-# [Skipping] pynvml.nvmlDeviceGetPendingEccMode (Python API Addition)
-# [Skipping] pynvml.nvmlDeviceGetTotalEccErrors
-# [Skipping] pynvml.nvmlDeviceGetDetailedEccErrors
-# [Skipping] pynvml.nvmlDeviceGetMemoryErrorCounter
-
-# Test pynvml.nvmlDeviceGetUtilizationRates
-@pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
-def test_nvmlDeviceGetUtilizationRates(ngpus, handles):
-    for i in range(ngpus):
-        urate = pynvml.nvmlDeviceGetUtilizationRates(handles[i])
-        assert urate.gpu >= 0
-        assert urate.memory >= 0
-
-
-# [Skipping] pynvml.nvmlDeviceGetEncoderUtilization
-# [Skipping] pynvml.nvmlDeviceGetDecoderUtilization
-# [Skipping] pynvml.nvmlDeviceGetPcieReplayCounter
-# [Skipping] pynvml.nvmlDeviceGetDriverModel
-# [Skipping] pynvml.nvmlDeviceGetCurrentDriverModel
-# [Skipping] pynvml.nvmlDeviceGetPendingDriverModel
-# [Skipping] pynvml.nvmlDeviceGetVbiosVersion
-# [Skipping] pynvml.nvmlDeviceGetComputeRunningProcesses
-# [Skipping] pynvml.nvmlDeviceGetGraphicsRunningProcesses
-# [Skipping] pynvml.nvmlDeviceGetAutoBoostedClocksEnabled
-# [Skipping] nvmlUnitSetLedState
-# [Skipping] pynvml.nvmlDeviceSetPersistenceMode
-# [Skipping] pynvml.nvmlDeviceSetComputeMode
-# [Skipping] pynvml.nvmlDeviceSetEccMode
-# [Skipping] pynvml.nvmlDeviceClearEccErrorCounts
-# [Skipping] pynvml.nvmlDeviceSetDriverModel
-# [Skipping] pynvml.nvmlDeviceSetAutoBoostedClocksEnabled
-# [Skipping] pynvml.nvmlDeviceSetDefaultAutoBoostedClocksEnabled
-# [Skipping] pynvml.nvmlDeviceSetApplicationsClocks
-# [Skipping] pynvml.nvmlDeviceResetApplicationsClocks
-# [Skipping] pynvml.nvmlDeviceSetPowerManagementLimit
-# [Skipping] pynvml.nvmlDeviceSetGpuOperationMode
-# [Skipping] nvmlEventSetCreate
-# [Skipping] pynvml.nvmlDeviceRegisterEvents
-# [Skipping] pynvml.nvmlDeviceGetSupportedEventTypes
-# [Skipping] nvmlEventSetWait
-# [Skipping] nvmlEventSetFree
-# [Skipping] pynvml.nvmlDeviceOnSameBoard
-# [Skipping] pynvml.nvmlDeviceGetCurrPcieLinkGeneration
-# [Skipping] pynvml.nvmlDeviceGetMaxPcieLinkGeneration
-# [Skipping] pynvml.nvmlDeviceGetCurrPcieLinkWidth
-# [Skipping] pynvml.nvmlDeviceGetMaxPcieLinkWidth
-# [Skipping] pynvml.nvmlDeviceGetSupportedClocksThrottleReasons
-# [Skipping] pynvml.nvmlDeviceGetCurrentClocksThrottleReasons
-# [Skipping] pynvml.nvmlDeviceGetIndex
-# [Skipping] pynvml.nvmlDeviceGetAccountingMode
-# [Skipping] pynvml.nvmlDeviceSetAccountingMode
-# [Skipping] pynvml.nvmlDeviceClearAccountingPids
-# [Skipping] pynvml.nvmlDeviceGetAccountingStats
-# [Skipping] pynvml.nvmlDeviceGetAccountingPids
-# [Skipping] pynvml.nvmlDeviceGetAccountingBufferSize
-# [Skipping] pynvml.nvmlDeviceGetRetiredPages
-# [Skipping] pynvml.nvmlDeviceGetRetiredPagesPendingStatus
-# [Skipping] pynvml.nvmlDeviceGetAPIRestriction
-# [Skipping] pynvml.nvmlDeviceSetAPIRestriction
-# [Skipping] pynvml.nvmlDeviceGetBridgeChipInfo
-# [Skipping] pynvml.nvmlDeviceGetSamples
-# [Skipping] pynvml.nvmlDeviceGetViolationStatus
-
-# Test pynvml.nvmlDeviceGetPcieThroughput
-@pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
-def test_nvmlDeviceGetPcieThroughput(ngpus, handles):
-    for i in range(ngpus):
-        tx_bytes_tp = pynvml.nvmlDeviceGetPcieThroughput(
-            handles[i], NVML_PCIE_UTIL_TX_BYTES
-        )
-        assert tx_bytes_tp >= 0
-        rx_bytes_tp = pynvml.nvmlDeviceGetPcieThroughput(
-            handles[i], NVML_PCIE_UTIL_RX_BYTES
-        )
-        assert rx_bytes_tp >= 0
-        count_tp = pynvml.nvmlDeviceGetPcieThroughput(handles[i], NVML_PCIE_UTIL_COUNT)
-        assert count_tp >= 0
-
-
-# [Skipping] pynvml.nvmlSystemGetTopologyGpuSet
-# [Skipping] pynvml.nvmlDeviceGetTopologyNearestGpus
-# [Skipping] pynvml.nvmlDeviceGetTopologyCommonAncestor
-
-# Test pynvml.nvmlDeviceGetNvLinkVersion
-# Test pynvml.nvmlDeviceGetNvLinkState
-# Test pynvml.nvmlDeviceGetNvLinkRemotePciInfo
-@pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
-def test_nvml_nvlink_properties(ngpus, handles):
-    for i in range(ngpus):
-        for j in range(pynvml.NVML_NVLINK_MAX_LINKS):
-            version = pynvml.nvmlDeviceGetNvLinkVersion(handles[i], j)
-            assert version >= 1
-            state = pynvml.nvmlDeviceGetNvLinkState(handles[i], j)
-            assert state >= 0
-            pci_info = pynvml.nvmlDeviceGetNvLinkRemotePciInfo(handles[i], j)
-            assert isinstance(pci_info, pynvml.c_nvmlPciInfo_t)
-
-
-# Test pynvml.nvmlDeviceResetNvLinkUtilizationCounter
-# Test pynvml.nvmlDeviceSetNvLinkUtilizationControl
-# Test pynvml.nvmlDeviceGetNvLinkUtilizationCounter
-# Test pynvml.nvmlDeviceGetNvLinkUtilizationControl
-# Test pynvml.nvmlDeviceFreezeNvLinkUtilizationCounter
-@pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
-@pytest.mark.parametrize("counter", [0, 1])
-@pytest.mark.parametrize("control", [0, 1, 2])
-def test_nvml_nvlink_counters(ngpus, handles, counter, control):
-    reset = 0
-    for i in range(ngpus):
-        for j in range(pynvml.NVML_NVLINK_MAX_LINKS):
-            assert (
-                pynvml.nvmlDeviceResetNvLinkUtilizationCounter(handles[i], j, counter)
-                == pynvml.NVML_SUCCESS
+    # Test pynvml.nvmlSystemGetProcessName
+    @pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
+    def test_nvml_system_get_process_name(nvml):
+        procname = None
+        procname = pynvml.nvmlSystemGetProcessName(os.getpid())
+        print("[Process: " + str(procname.decode()) + "]", end=" ")
+        assert procname != None
+
+    # Test pynvml.nvmlSystemGetDriverVersion
+    @pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
+    def test_nvml_system_get_driver_version(nvml):
+        vsn = 0.0
+        vsn = pynvml.nvmlSystemGetDriverVersion().decode()
+        print("[Driver Version: " + vsn + "]", end=" ")
+        assert vsn > LooseVersion("0.0")  # Developing with 396.44
+
+    ## Unit "Get" Functions (Skipping for now) ##
+
+    ## Device "Get" Functions (Note: Some functions are fixtures, above) ##
+
+    # Test pynvml.nvmlDeviceGetHandleBySerial
+    @pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
+    def test_nvml_device_get_handle_by_serial(ngpus, serials):
+        handles = [pynvml.nvmlDeviceGetHandleBySerial(serials[i]) for i in range(ngpus)]
+        assert len(handles) == ngpus
+
+    # Test pynvml.nvmlDeviceGetHandleByUUID
+    @pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
+    def test_nvml_device_get_handle_by_uuid(ngpus, uuids):
+        handles = [pynvml.nvmlDeviceGetHandleByUUID(uuids[i]) for i in range(ngpus)]
+        assert len(handles) == ngpus
+
+    # Test pynvml.nvmlDeviceGetHandleByPciBusId
+    @pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
+    def test_nvml_device_get_handle_by_pci_bus_id(ngpus, pci_info):
+        handles = [
+            pynvml.nvmlDeviceGetHandleByPciBusId(pci_info[i].busId)
+            for i in range(ngpus)
+        ]
+        assert len(handles) == ngpus
+
+    # [Skipping] pynvml.nvmlDeviceGetName
+    # [Skipping] pynvml.nvmlDeviceGetBoardId
+    # [Skipping] pynvml.nvmlDeviceGetMultiGpuBoard
+    # [Skipping] pynvml.nvmlDeviceGetBrand
+    # [Skipping] pynvml.nvmlDeviceGetCpuAffinity
+    # [Skipping] pynvml.nvmlDeviceSetCpuAffinity
+    # [Skipping] pynvml.nvmlDeviceClearCpuAffinity
+    # [Skipping] pynvml.nvmlDeviceGetMinorNumber
+    # [Skipping] pynvml.nvmlDeviceGetUUID
+    # [Skipping] pynvml.nvmlDeviceGetInforomVersion
+    # [Skipping] pynvml.nvmlDeviceGetInforomImageVersion
+    # [Skipping] pynvml.nvmlDeviceGetInforomConfigurationChecksum
+    # [Skipping] pynvml.nvmlDeviceValidateInforom
+    # [Skipping] pynvml.nvmlDeviceGetDisplayMode
+    # [Skipping] pynvml.nvmlDeviceGetPersistenceMode
+    # [Skipping] pynvml.nvmlDeviceGetClockInfo
+    # [Skipping] pynvml.nvmlDeviceGetMaxClockInfo
+    # [Skipping] pynvml.nvmlDeviceGetApplicationsCloc
+    # [Skipping] pynvml.nvmlDeviceGetDefaultApplicationsClock
+    # [Skipping] pynvml.nvmlDeviceGetSupportedMemoryClocks
+    # [Skipping] pynvml.nvmlDeviceGetSupportedGraphicsClocks
+    # [Skipping] pynvml.nvmlDeviceGetFanSpeed
+    # [Skipping] pynvml.nvmlDeviceGetTemperature
+    # [Skipping] pynvml.nvmlDeviceGetTemperatureThreshold
+    # [Skipping] pynvml.nvmlDeviceGetPowerState
+    # [Skipping] pynvml.nvmlDeviceGetPerformanceState
+    # [Skipping] pynvml.nvmlDeviceGetPowerManagementMode
+    # [Skipping] pynvml.nvmlDeviceGetPowerManagementLimit
+    # [Skipping] pynvml.nvmlDeviceGetPowerManagementLimitConstraints
+    # [Skipping] pynvml.nvmlDeviceGetPowerManagementDefaultLimit
+    # [Skipping] pynvml.nvmlDeviceGetEnforcedPowerLimit
+
+    # Test pynvml.nvmlDeviceGetPowerUsage
+    @pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
+    def test_nvmlDeviceGetPowerUsage(ngpus, handles):
+        for i in range(ngpus):
+            power_mWatts = pynvml.nvmlDeviceGetPowerUsage(handles[i])
+            assert power_mWatts >= 0.0
+
+    # Test pynvml.nvmlDeviceGetTotalEnergyConsumption
+    @pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
+    def test_nvmlDeviceGetTotalEnergyConsumption(ngpus, handles):
+        for i in range(ngpus):
+            energy_mJoules1 = pynvml.nvmlDeviceGetTotalEnergyConsumption(handles[i])
+            for j in range(10):  # idle for 150 ms
+                time.sleep(0.015)  # and check for increase every 15 ms
+                energy_mJoules2 = pynvml.nvmlDeviceGetTotalEnergyConsumption(handles[i])
+                assert energy_mJoules2 >= energy_mJoules1
+                if energy_mJoules2 > energy_mJoules1:
+                    break
+            else:
+                assert False, "energy did not increase across 150 ms interval"
+
+    # [Skipping] pynvml.nvmlDeviceGetGpuOperationMode
+    # [Skipping] pynvml.nvmlDeviceGetCurrentGpuOperationMode
+    # [Skipping] pynvml.nvmlDeviceGetPendingGpuOperationMode
+
+    # Test pynvml.nvmlDeviceGetMemoryInfo
+    @pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
+    def test_nvmlDeviceGetMemoryInfo(ngpus, handles):
+        for i in range(ngpus):
+            meminfo = pynvml.nvmlDeviceGetMemoryInfo(handles[i])
+            assert (meminfo.used <= meminfo.total) and (meminfo.free <= meminfo.total)
+
+    # [Skipping] pynvml.nvmlDeviceGetBAR1MemoryInfo
+    # [Skipping] pynvml.nvmlDeviceGetComputeMode
+    # [Skipping] pynvml.nvmlDeviceGetEccMode
+    # [Skipping] pynvml.nvmlDeviceGetCurrentEccMode (Python API Addition)
+    # [Skipping] pynvml.nvmlDeviceGetPendingEccMode (Python API Addition)
+    # [Skipping] pynvml.nvmlDeviceGetTotalEccErrors
+    # [Skipping] pynvml.nvmlDeviceGetDetailedEccErrors
+    # [Skipping] pynvml.nvmlDeviceGetMemoryErrorCounter
+
+    # Test pynvml.nvmlDeviceGetUtilizationRates
+    @pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
+    def test_nvmlDeviceGetUtilizationRates(ngpus, handles):
+        for i in range(ngpus):
+            urate = pynvml.nvmlDeviceGetUtilizationRates(handles[i])
+            assert urate.gpu >= 0
+            assert urate.memory >= 0
+
+    # [Skipping] pynvml.nvmlDeviceGetEncoderUtilization
+    # [Skipping] pynvml.nvmlDeviceGetDecoderUtilization
+    # [Skipping] pynvml.nvmlDeviceGetPcieReplayCounter
+    # [Skipping] pynvml.nvmlDeviceGetDriverModel
+    # [Skipping] pynvml.nvmlDeviceGetCurrentDriverModel
+    # [Skipping] pynvml.nvmlDeviceGetPendingDriverModel
+    # [Skipping] pynvml.nvmlDeviceGetVbiosVersion
+    # [Skipping] pynvml.nvmlDeviceGetComputeRunningProcesses
+    # [Skipping] pynvml.nvmlDeviceGetGraphicsRunningProcesses
+    # [Skipping] pynvml.nvmlDeviceGetAutoBoostedClocksEnabled
+    # [Skipping] nvmlUnitSetLedState
+    # [Skipping] pynvml.nvmlDeviceSetPersistenceMode
+    # [Skipping] pynvml.nvmlDeviceSetComputeMode
+    # [Skipping] pynvml.nvmlDeviceSetEccMode
+    # [Skipping] pynvml.nvmlDeviceClearEccErrorCounts
+    # [Skipping] pynvml.nvmlDeviceSetDriverModel
+    # [Skipping] pynvml.nvmlDeviceSetAutoBoostedClocksEnabled
+    # [Skipping] pynvml.nvmlDeviceSetDefaultAutoBoostedClocksEnabled
+    # [Skipping] pynvml.nvmlDeviceSetApplicationsClocks
+    # [Skipping] pynvml.nvmlDeviceResetApplicationsClocks
+    # [Skipping] pynvml.nvmlDeviceSetPowerManagementLimit
+    # [Skipping] pynvml.nvmlDeviceSetGpuOperationMode
+    # [Skipping] nvmlEventSetCreate
+    # [Skipping] pynvml.nvmlDeviceRegisterEvents
+    # [Skipping] pynvml.nvmlDeviceGetSupportedEventTypes
+    # [Skipping] nvmlEventSetWait
+    # [Skipping] nvmlEventSetFree
+    # [Skipping] pynvml.nvmlDeviceOnSameBoard
+    # [Skipping] pynvml.nvmlDeviceGetCurrPcieLinkGeneration
+    # [Skipping] pynvml.nvmlDeviceGetMaxPcieLinkGeneration
+    # [Skipping] pynvml.nvmlDeviceGetCurrPcieLinkWidth
+    # [Skipping] pynvml.nvmlDeviceGetMaxPcieLinkWidth
+    # [Skipping] pynvml.nvmlDeviceGetSupportedClocksThrottleReasons
+    # [Skipping] pynvml.nvmlDeviceGetCurrentClocksThrottleReasons
+    # [Skipping] pynvml.nvmlDeviceGetIndex
+    # [Skipping] pynvml.nvmlDeviceGetAccountingMode
+    # [Skipping] pynvml.nvmlDeviceSetAccountingMode
+    # [Skipping] pynvml.nvmlDeviceClearAccountingPids
+    # [Skipping] pynvml.nvmlDeviceGetAccountingStats
+    # [Skipping] pynvml.nvmlDeviceGetAccountingPids
+    # [Skipping] pynvml.nvmlDeviceGetAccountingBufferSize
+    # [Skipping] pynvml.nvmlDeviceGetRetiredPages
+    # [Skipping] pynvml.nvmlDeviceGetRetiredPagesPendingStatus
+    # [Skipping] pynvml.nvmlDeviceGetAPIRestriction
+    # [Skipping] pynvml.nvmlDeviceSetAPIRestriction
+    # [Skipping] pynvml.nvmlDeviceGetBridgeChipInfo
+    # [Skipping] pynvml.nvmlDeviceGetSamples
+    # [Skipping] pynvml.nvmlDeviceGetViolationStatus
+
+    # Test pynvml.nvmlDeviceGetPcieThroughput
+    @pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
+    def test_nvmlDeviceGetPcieThroughput(ngpus, handles):
+        for i in range(ngpus):
+            tx_bytes_tp = pynvml.nvmlDeviceGetPcieThroughput(
+                handles[i], NVML_PCIE_UTIL_TX_BYTES
             )
-            pynvml.nvmlDeviceSetNvLinkUtilizationControl(
-                handles[i], j, counter, control, reset
+            assert tx_bytes_tp >= 0
+            rx_bytes_tp = pynvml.nvmlDeviceGetPcieThroughput(
+                handles[i], NVML_PCIE_UTIL_RX_BYTES
             )
-            countdict = pynvml.nvmlDeviceGetNvLinkUtilizationCounter(
-                handles[i], j, counter
+            assert rx_bytes_tp >= 0
+            count_tp = pynvml.nvmlDeviceGetPcieThroughput(
+                handles[i], NVML_PCIE_UTIL_COUNT
             )
-            ctl = pynvml.nvmlDeviceGetNvLinkUtilizationControl(handles[i], j, counter)
-            assert countdict["rx"] >= 0
-            assert countdict["tx"] >= 0
-            assert ctl == control
-            assert (
-                pynvml.nvmlDeviceFreezeNvLinkUtilizationCounter(
-                    handles[i], j, counter, 1
+            assert count_tp >= 0
+
+    # [Skipping] pynvml.nvmlSystemGetTopologyGpuSet
+    # [Skipping] pynvml.nvmlDeviceGetTopologyNearestGpus
+    # [Skipping] pynvml.nvmlDeviceGetTopologyCommonAncestor
+
+    # Test pynvml.nvmlDeviceGetNvLinkVersion
+    # Test pynvml.nvmlDeviceGetNvLinkState
+    # Test pynvml.nvmlDeviceGetNvLinkRemotePciInfo
+    @pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
+    def test_nvml_nvlink_properties(ngpus, handles):
+        for i in range(ngpus):
+            for j in range(pynvml.NVML_NVLINK_MAX_LINKS):
+                version = pynvml.nvmlDeviceGetNvLinkVersion(handles[i], j)
+                assert version >= 1
+                state = pynvml.nvmlDeviceGetNvLinkState(handles[i], j)
+                assert state >= 0
+                pci_info = pynvml.nvmlDeviceGetNvLinkRemotePciInfo(handles[i], j)
+                assert isinstance(pci_info, pynvml.c_nvmlPciInfo_t)
+
+    # Test pynvml.nvmlDeviceResetNvLinkUtilizationCounter
+    # Test pynvml.nvmlDeviceSetNvLinkUtilizationControl
+    # Test pynvml.nvmlDeviceGetNvLinkUtilizationCounter
+    # Test pynvml.nvmlDeviceGetNvLinkUtilizationControl
+    # Test pynvml.nvmlDeviceFreezeNvLinkUtilizationCounter
+    @pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
+    @pytest.mark.parametrize("counter", [0, 1])
+    @pytest.mark.parametrize("control", [0, 1, 2])
+    def test_nvml_nvlink_counters(ngpus, handles, counter, control):
+        reset = 0
+        for i in range(ngpus):
+            for j in range(pynvml.NVML_NVLINK_MAX_LINKS):
+                assert (
+                    pynvml.nvmlDeviceResetNvLinkUtilizationCounter(
+                        handles[i], j, counter
+                    )
+                    == pynvml.NVML_SUCCESS
                 )
-                == pynvml.NVML_SUCCESS
-            )
-            assert (
-                pynvml.nvmlDeviceFreezeNvLinkUtilizationCounter(
-                    handles[i], j, counter, 0
+                pynvml.nvmlDeviceSetNvLinkUtilizationControl(
+                    handles[i], j, counter, control, reset
+                )
+                countdict = pynvml.nvmlDeviceGetNvLinkUtilizationCounter(
+                    handles[i], j, counter
+                )
+                ctl = pynvml.nvmlDeviceGetNvLinkUtilizationControl(
+                    handles[i], j, counter
+                )
+                assert countdict["rx"] >= 0
+                assert countdict["tx"] >= 0
+                assert ctl == control
+                assert (
+                    pynvml.nvmlDeviceFreezeNvLinkUtilizationCounter(
+                        handles[i], j, counter, 1
+                    )
+                    == pynvml.NVML_SUCCESS
+                )
+                assert (
+                    pynvml.nvmlDeviceFreezeNvLinkUtilizationCounter(
+                        handles[i], j, counter, 0
+                    )
+                    == pynvml.NVML_SUCCESS
                 )
-                == pynvml.NVML_SUCCESS
-            )
```

### Comparing `Heimdallr-0.2.7/tests/test_smi.py` & `heimdallr-0.2.8/tests/test_smi.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 if sys.platform == "linux":
     from heimdallr.utilities.nvidia.smi_parsing import NvidiaSMI
 
 
 @pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
 @pytest.fixture(scope="module")
 def smi(request):
-    """ """
+    """description"""
     return NvidiaSMI.getInstance()
 
 
 @pytest.mark.skipif(sys.platform != "linux", reason="Test only on linux")
 @pytest.fixture
 def ngpus(smi):
-    """ """
+    """description"""
     result = smi.DeviceQuery("count")["count"]
     assert result > 0
     print("[" + str(result) + " GPUs]", end=" ")
     return result
 
 
 ## ---------------------------- ##
```

