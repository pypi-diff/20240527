# Comparing `tmp/whiffle_client-0.4.3.tar.gz` & `tmp/whiffle_client-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whiffle_client-0.4.3.tar", last modified: Thu May 23 13:20:06 2024, max compression
+gzip compressed data, was "whiffle_client-0.4.4.tar", last modified: Mon May 27 13:02:42 2024, max compression
```

## Comparing `whiffle_client-0.4.3.tar` & `whiffle_client-0.4.4.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:20:06.081550 whiffle_client-0.4.3/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/LICENCE.txt
--rw-r--r--   0 root         (0) root         (0)    11095 2024-05-23 13:20:06.080551 whiffle_client-0.4.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      980 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)    10139 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/USER_README.md
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 13:20:06.081550 whiffle_client-0.4.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:20:06.071550 whiffle_client-0.4.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2506 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2096 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/tests/test_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:20:06.072550 whiffle_client-0.4.3/whiffle_client/
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:20:06.075550 whiffle_client-0.4.3/whiffle_client/analysis/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/analysis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7628 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/analysis/io.py
--rw-rw-rw-   0 root         (0) root         (0)    16433 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/analysis/plot.py
--rw-rw-rw-   0 root         (0) root         (0)     4854 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/analysis/scatter.py
--rw-rw-rw-   0 root         (0) root         (0)     4957 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/analysis/skill.py
--rw-rw-rw-   0 root         (0) root         (0)     3231 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/analysis/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3995 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/base_client.py
--rw-rw-rw-   0 root         (0) root         (0)     6260 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/client.py
--rw-rw-rw-   0 root         (0) root         (0)     1400 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     3218 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/entrypoints.py
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:20:06.075550 whiffle_client-0.4.3/whiffle_client/loaders/
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/loaders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1183 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/loaders/csv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:20:06.076550 whiffle_client-0.4.3/whiffle_client/resources/
--rw-rw-rw-   0 root         (0) root         (0)     2624 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/resources/example_generic_params.json
--rw-rw-rw-   0 root         (0) root         (0)     1015 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/resources/example_yaml_include.yaml
--rw-rw-rw-   0 root         (0) root         (0)      154 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/resources/example_yaml_include_metmasts.yaml
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/resources/whiffle_config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:20:06.076550 whiffle_client-0.4.3/whiffle_client/snippets/
--rw-rw-rw-   0 root         (0) root         (0)     2401 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/snippets/create_mock_powercurve.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:20:06.076550 whiffle_client-0.4.3/whiffle_client/wind/
--rw-rw-rw-   0 root         (0) root         (0)       96 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/wind/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1802 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/wind/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:20:06.078550 whiffle_client-0.4.3/whiffle_client/wind/components/
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/wind/components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      183 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/wind/components/dates.py
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/wind/components/domain.py
--rw-rw-rw-   0 root         (0) root         (0)      212 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/wind/components/geometries.py
--rw-rw-rw-   0 root         (0) root         (0)      188 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/wind/components/metmast.py
--rw-rw-rw-   0 root         (0) root         (0)      190 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/wind/components/turbine.py
--rw-rw-rw-   0 root         (0) root         (0)     1166 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/wind/components/turbine_model_specs.py
--rw-rw-rw-   0 root         (0) root         (0)     5252 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/wind/components/wind_simulation_task.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/wind/components/windfarm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:20:06.079550 whiffle_client-0.4.3/whiffle_client/wind/mapping/
--rw-rw-rw-   0 root         (0) root         (0)      243 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/wind/mapping/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      667 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/wind/mapping/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4808 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/wind/mapping/turbine_model_specs.py
--rw-rw-rw-   0 root         (0) root         (0)     6023 2024-05-23 13:20:03.000000 whiffle_client-0.4.3/whiffle_client/wind/mapping/wind_simulation_tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:20:06.079550 whiffle_client-0.4.3/whiffle_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11095 2024-05-23 13:20:06.000000 whiffle_client-0.4.3/whiffle_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1652 2024-05-23 13:20:06.000000 whiffle_client-0.4.3/whiffle_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 13:20:06.000000 whiffle_client-0.4.3/whiffle_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2024-05-23 13:20:06.000000 whiffle_client-0.4.3/whiffle_client.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      189 2024-05-23 13:20:06.000000 whiffle_client-0.4.3/whiffle_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-23 13:20:06.000000 whiffle_client-0.4.3/whiffle_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 13:02:42.809380 whiffle_client-0.4.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/LICENCE.txt
+-rw-r--r--   0 root         (0) root         (0)    11079 2024-05-27 13:02:42.809380 whiffle_client-0.4.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      980 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    10125 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/USER_README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1260 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 13:02:42.809380 whiffle_client-0.4.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 13:02:42.797380 whiffle_client-0.4.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2506 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2096 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/tests/test_client.py
+-rw-rw-rw-   0 root         (0) root         (0)      560 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/tests/test_io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 13:02:42.799380 whiffle_client-0.4.4/whiffle_client/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 13:02:42.803380 whiffle_client-0.4.4/whiffle_client/analysis/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/analysis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7628 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/analysis/io.py
+-rw-rw-rw-   0 root         (0) root         (0)    16433 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/analysis/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     4854 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/analysis/scatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4957 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/analysis/skill.py
+-rw-rw-rw-   0 root         (0) root         (0)     3231 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/analysis/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3995 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/base_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     6154 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1162 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     3218 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/entrypoints.py
+-rw-rw-rw-   0 root         (0) root         (0)     1671 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 13:02:42.803380 whiffle_client-0.4.4/whiffle_client/loaders/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/loaders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1394 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/loaders/csv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 13:02:42.804380 whiffle_client-0.4.4/whiffle_client/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     2624 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/resources/example_generic_params.json
+-rw-rw-rw-   0 root         (0) root         (0)     1015 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/resources/example_yaml_include.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/resources/example_yaml_include_metmasts.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/resources/whiffle_config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 13:02:42.804380 whiffle_client-0.4.4/whiffle_client/snippets/
+-rw-rw-rw-   0 root         (0) root         (0)     2401 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/snippets/create_mock_powercurve.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 13:02:42.805380 whiffle_client-0.4.4/whiffle_client/wind/
+-rw-rw-rw-   0 root         (0) root         (0)       96 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/wind/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/wind/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 13:02:42.806380 whiffle_client-0.4.4/whiffle_client/wind/components/
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/wind/components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      183 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/wind/components/dates.py
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/wind/components/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)      212 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/wind/components/geometries.py
+-rw-rw-rw-   0 root         (0) root         (0)      190 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/wind/components/metmast.py
+-rw-rw-rw-   0 root         (0) root         (0)      190 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/wind/components/turbine.py
+-rw-rw-rw-   0 root         (0) root         (0)     1166 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/wind/components/turbine_model_specs.py
+-rw-rw-rw-   0 root         (0) root         (0)     5005 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/wind/components/wind_simulation_task.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/wind/components/windfarm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 13:02:42.807380 whiffle_client-0.4.4/whiffle_client/wind/mapping/
+-rw-rw-rw-   0 root         (0) root         (0)      243 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/wind/mapping/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      624 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/wind/mapping/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4802 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/wind/mapping/turbine_model_specs.py
+-rw-rw-rw-   0 root         (0) root         (0)     6023 2024-05-27 13:02:39.000000 whiffle_client-0.4.4/whiffle_client/wind/mapping/wind_simulation_tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 13:02:42.808380 whiffle_client-0.4.4/whiffle_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11079 2024-05-27 13:02:42.000000 whiffle_client-0.4.4/whiffle_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1669 2024-05-27 13:02:42.000000 whiffle_client-0.4.4/whiffle_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 13:02:42.000000 whiffle_client-0.4.4/whiffle_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2024-05-27 13:02:42.000000 whiffle_client-0.4.4/whiffle_client.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      187 2024-05-27 13:02:42.000000 whiffle_client-0.4.4/whiffle_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-27 13:02:42.000000 whiffle_client-0.4.4/whiffle_client.egg-info/top_level.txt
```

### Comparing `whiffle_client-0.4.3/LICENCE.txt` & `whiffle_client-0.4.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.3/PKG-INFO` & `whiffle_client-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: whiffle_client
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python based web client to interact with Whiffle services
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 Requires-Dist: click~=8.0.4
 Requires-Dist: PyYAML~=6.0
-Requires-Dist: pyyaml-include~=1.3.1
+Requires-Dist: pyyaml-include~=2.1
 Requires-Dist: platformdirs~=4.0.0
 Requires-Dist: requests
 Requires-Dist: pandas>=2
 Requires-Dist: jupyter
 Provides-Extra: analysis
 Requires-Dist: numpy; extra == "analysis"
 Requires-Dist: scipy; extra == "analysis"
@@ -115,22 +115,22 @@
 reference_code: "Test simulations"
 
 dates: 
   start: "2023-01-01"
   end: "2023-01-07"
 
 windfarms:
-  windfarm_a: !include ./inputs/windfarm_A.yaml
+  windfarm_a: !include ./windfarm_A.yaml
   windfarm_b:
     name: [turbine_1B, turbine_2B, turbine_3B, turbine_4B]
     location: [[4.25, 51.92], [4.21, 52.035], [4.31, 51.952], [4.22, 52.014]]  
     turbine_model_name: my_turbine_model_1
     thrust: True
     include_in_les: True
-  windfarm_c: !include-csv ./inputs/windfarm_C.csv
+  windfarm_c: !include-csv ./windfarm_C.csv
 
 metmasts:
   name: [metA, metB, metC]
   location: [[4.05, 52], [4.1, 52.05], [4.15, 52.15]]  
 metmasts_heights: [20, 40, 60, 80, 100, 2500, 3000] # unlimited
 
 wind_resource_grid_heights: [100]
```

### Comparing `whiffle_client-0.4.3/README.md` & `whiffle_client-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.3/USER_README.md` & `whiffle_client-0.4.4/USER_README.md`

 * *Files 1% similar despite different names*

```diff
@@ -88,22 +88,22 @@
 reference_code: "Test simulations"
 
 dates: 
   start: "2023-01-01"
   end: "2023-01-07"
 
 windfarms:
-  windfarm_a: !include ./inputs/windfarm_A.yaml
+  windfarm_a: !include ./windfarm_A.yaml
   windfarm_b:
     name: [turbine_1B, turbine_2B, turbine_3B, turbine_4B]
     location: [[4.25, 51.92], [4.21, 52.035], [4.31, 51.952], [4.22, 52.014]]  
     turbine_model_name: my_turbine_model_1
     thrust: True
     include_in_les: True
-  windfarm_c: !include-csv ./inputs/windfarm_C.csv
+  windfarm_c: !include-csv ./windfarm_C.csv
 
 metmasts:
   name: [metA, metB, metC]
   location: [[4.05, 52], [4.1, 52.05], [4.15, 52.15]]  
 metmasts_heights: [20, 40, 60, 80, 100, 2500, 3000] # unlimited
 
 wind_resource_grid_heights: [100]
```

### Comparing `whiffle_client-0.4.3/pyproject.toml` & `whiffle_client-0.4.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ]
 
 requires-python = ">=3.8"
 
 dependencies = [
     "click~=8.0.4",
     "PyYAML~=6.0",
-    "pyyaml-include~=1.3.1",
+    "pyyaml-include~=2.1",
     "platformdirs~=4.0.0",
     "requests",
     "pandas>=2",
     "jupyter"
 ]
 
 dynamic = ["version"]
```

### Comparing `whiffle_client-0.4.3/tests/test_cli.py` & `whiffle_client-0.4.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.3/tests/test_client.py` & `whiffle_client-0.4.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.3/whiffle_client/analysis/io.py` & `whiffle_client-0.4.4/whiffle_client/analysis/io.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.3/whiffle_client/analysis/plot.py` & `whiffle_client-0.4.4/whiffle_client/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.3/whiffle_client/analysis/scatter.py` & `whiffle_client-0.4.4/whiffle_client/analysis/scatter.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.3/whiffle_client/analysis/skill.py` & `whiffle_client-0.4.4/whiffle_client/analysis/skill.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.3/whiffle_client/analysis/utils.py` & `whiffle_client-0.4.4/whiffle_client/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.3/whiffle_client/base_client.py` & `whiffle_client-0.4.4/whiffle_client/base_client.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.3/whiffle_client/client.py` & `whiffle_client-0.4.4/whiffle_client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,31 +3,28 @@
 import json
 import os
 import time
 
 import pkg_resources
 import platformdirs
 import yaml
-from yamlinclude import YamlIncludeConstructor
 
 from whiffle_client.base_client import BaseClient
-from whiffle_client.io import download_write_chunks
+from whiffle_client.io import download_write_chunks, load_yaml_with_include
 
 CHUNK_SIZE = 1024 * 1024
 CONFIG_FILE_NAME = "whiffle_config.yaml"
 CONFIG_FILE_PATH_LOCATIONS = [
     f"{platformdirs.user_config_dir('whiffle')}/{CONFIG_FILE_NAME}",  # app path
     f"{CONFIG_FILE_NAME}",  # workdir path
     pkg_resources.resource_filename(
         "whiffle_client", f"resources/{CONFIG_FILE_NAME}"
     ),  # package resource
 ]
 
-YamlIncludeConstructor.add_to_loader_class(loader_class=yaml.FullLoader)
-
 
 class ServerError(BaseException):
     pass
 
 
 class NoTokenError(Exception):
     pass
@@ -68,20 +65,20 @@
         # Reqular Python dictionary, convert to json
         if type(input_params_io) == dict:
             data = json.dumps(input_params_io).encode("ascii")
         # Either a filename or already json
         elif type(input_params_io) == str:
             _, extension = os.path.splitext(input_params_io)
             if extension.lower() in {".json", ".yaml", ".yml"}:
-                with open(input_params_io) as f:
-                    if extension == ".json":
+                if extension == ".json":
+                    with open(input_params_io) as f:
                         data = f.read()
-                    else:
-                        yaml_data = yaml.load(f, Loader=yaml.FullLoader)
-                        data = json.dumps(yaml_data)
+                else:
+                    yaml_data = load_yaml_with_include(input_params_io)
+                    data = json.dumps(yaml_data)
             else:
                 # Assume the data is json
                 json.loads(input_params_io)  # will raise an exception if not
                 data = input_params_io
         else:
             raise TypeError("Only dictionary or a filename are allowed")
         return data
```

### Comparing `whiffle_client-0.4.3/whiffle_client/entrypoints.py` & `whiffle_client-0.4.4/whiffle_client/entrypoints.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.3/whiffle_client/loaders/csv.py` & `whiffle_client-0.4.4/whiffle_client/loaders/csv.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,22 @@
-from dataclasses import InitVar, dataclass, field
 import json
+from dataclasses import InitVar, asdict, dataclass, field
+from pathlib import Path
+
 import pandas as pd
 
 
-def csv_loader_constructor(loader, node):
-    return CSVLoader(path_to_csv=loader.construct_yaml_str(node))
+def csv_loader_constructor(base_dir=None):
+    def csv_loader(loader, node):
+        path = loader.construct_scalar(node)
+        if base_dir is not None:
+            path = f"{Path(base_dir).resolve()}/{path}"
+        return asdict(CSVLoader(path_to_csv=path))
+
+    return csv_loader
 
 
 @dataclass
 class CSVLoader:
     # Init attributes
     path_to_csv: InitVar[str] = ""
```

### Comparing `whiffle_client-0.4.3/whiffle_client/resources/example_generic_params.json` & `whiffle_client-0.4.4/whiffle_client/resources/example_generic_params.json`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.3/whiffle_client/resources/example_yaml_include.yaml` & `whiffle_client-0.4.4/whiffle_client/resources/example_yaml_include.yaml`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.3/whiffle_client/snippets/create_mock_powercurve.py` & `whiffle_client-0.4.4/whiffle_client/snippets/create_mock_powercurve.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.3/whiffle_client/wind/client.py` & `whiffle_client-0.4.4/whiffle_client/wind/client.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.3/whiffle_client/wind/components/__init__.py` & `whiffle_client-0.4.4/whiffle_client/wind/components/__init__.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.3/whiffle_client/wind/components/turbine_model_specs.py` & `whiffle_client-0.4.4/whiffle_client/wind/components/turbine_model_specs.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.3/whiffle_client/wind/components/wind_simulation_task.py` & `whiffle_client-0.4.4/whiffle_client/wind/components/wind_simulation_task.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,15 @@
 import datetime
 import inspect
 import json
 from dataclasses import asdict, dataclass, field
 
-import yaml
-from yamlinclude import YamlIncludeConstructor
-
-from whiffle_client.loaders import csv_loader_constructor
 from whiffle_client.wind.components import Domain, Geometries, Metmast, Windfarm
 from whiffle_client.wind.components.dates import Dates
 
-YamlIncludeConstructor.add_to_loader_class(loader_class=yaml.FullLoader)
-yaml.add_constructor("!include-csv", csv_loader_constructor)
-
 READ_ONLY_FIELDS = set(
     [
         "id",
         "status",
         "messages",
         "creator",
         "created",
@@ -78,23 +71,23 @@
         )
 
     def __post_init__(self):
 
         if isinstance(self.metmasts, list):
             self.metmasts = [
                 Metmast(
-                    id=metmast["name"],
+                    name=metmast["name"],
                     longitude=metmast["longitude"],
                     latitude=metmast["latitude"],
                 )
                 for metmast in self.metmasts
             ]
         elif isinstance(self.metmasts, dict):
             self.metmasts = [
-                Metmast(id=name, latitude=latitude, longitude=longitude)
+                Metmast(name=name, latitude=latitude, longitude=longitude)
                 for name, (longitude, latitude) in zip(
                     self.metmasts["name"], self.metmasts["location"]
                 )
             ]
 
         if isinstance(self.windfarms, list):
             self.windfarms = [Windfarm(**windfarm) for windfarm in self.windfarms]
@@ -122,15 +115,15 @@
     def _get_api_params(self):
         params = asdict(self)
         _ = [params.pop(key, None) for key in READ_ONLY_FIELDS]
 
         if self.metmasts:
             params["metmasts"] = [
                 {
-                    "name": metmast.id,
+                    "name": metmast.name,
                     "longitude": metmast.longitude,
                     "latitude": metmast.latitude,
                 }
                 for metmast in self.metmasts
             ]
 
         if self.windfarms:
```

### Comparing `whiffle_client-0.4.3/whiffle_client/wind/mapping/base.py` & `whiffle_client-0.4.4/whiffle_client/wind/mapping/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from abc import ABC, abstractmethod
-from dataclasses import asdict
-import json
 
 
 class BaseMapping(ABC):
     URL = None
     RESOURCE_TYPE = None
 
     def __init__(self, session):
```

### Comparing `whiffle_client-0.4.3/whiffle_client/wind/mapping/turbine_model_specs.py` & `whiffle_client-0.4.4/whiffle_client/wind/mapping/turbine_model_specs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from whiffle_client.wind.components.turbine_model_specs import TurbineModelSpecs
 from whiffle_client.decorators import load_data
 from whiffle_client.wind.mapping.base import BaseMapping
 
 
 class TurbineModelSpecsEndpoints(BaseMapping):
 
-    URL = "/api/aspforge/turbine-models"
+    URL = "/api/v1/turbine-models"
     RESOURCE_TYPE = "TurbineModelSpecs"
 
     # Turbine models commands
     @load_data(TurbineModelSpecs)
     def add(
         self,
         data: Union[str, dict, Path, TurbineModelSpecs] = None,
```

### Comparing `whiffle_client-0.4.3/whiffle_client/wind/mapping/wind_simulation_tasks.py` & `whiffle_client-0.4.4/whiffle_client/wind/mapping/wind_simulation_tasks.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.3/whiffle_client.egg-info/PKG-INFO` & `whiffle_client-0.4.4/whiffle_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: whiffle_client
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python based web client to interact with Whiffle services
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 Requires-Dist: click~=8.0.4
 Requires-Dist: PyYAML~=6.0
-Requires-Dist: pyyaml-include~=1.3.1
+Requires-Dist: pyyaml-include~=2.1
 Requires-Dist: platformdirs~=4.0.0
 Requires-Dist: requests
 Requires-Dist: pandas>=2
 Requires-Dist: jupyter
 Provides-Extra: analysis
 Requires-Dist: numpy; extra == "analysis"
 Requires-Dist: scipy; extra == "analysis"
@@ -115,22 +115,22 @@
 reference_code: "Test simulations"
 
 dates: 
   start: "2023-01-01"
   end: "2023-01-07"
 
 windfarms:
-  windfarm_a: !include ./inputs/windfarm_A.yaml
+  windfarm_a: !include ./windfarm_A.yaml
   windfarm_b:
     name: [turbine_1B, turbine_2B, turbine_3B, turbine_4B]
     location: [[4.25, 51.92], [4.21, 52.035], [4.31, 51.952], [4.22, 52.014]]  
     turbine_model_name: my_turbine_model_1
     thrust: True
     include_in_les: True
-  windfarm_c: !include-csv ./inputs/windfarm_C.csv
+  windfarm_c: !include-csv ./windfarm_C.csv
 
 metmasts:
   name: [metA, metB, metC]
   location: [[4.05, 52], [4.1, 52.05], [4.15, 52.15]]  
 metmasts_heights: [20, 40, 60, 80, 100, 2500, 3000] # unlimited
 
 wind_resource_grid_heights: [100]
```

### Comparing `whiffle_client-0.4.3/whiffle_client.egg-info/SOURCES.txt` & `whiffle_client-0.4.4/whiffle_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENCE.txt
 README.md
 USER_README.md
 pyproject.toml
 tests/test_cli.py
 tests/test_client.py
+tests/test_io.py
 whiffle_client/__init__.py
 whiffle_client/base_client.py
 whiffle_client/client.py
 whiffle_client/decorators.py
 whiffle_client/entrypoints.py
 whiffle_client/io.py
 whiffle_client.egg-info/PKG-INFO
```

