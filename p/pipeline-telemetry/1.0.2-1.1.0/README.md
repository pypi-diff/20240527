# Comparing `tmp/pipeline_telemetry-1.0.2.tar.gz` & `tmp/pipeline_telemetry-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline_telemetry-1.0.2.tar", last modified: Wed May  8 14:29:29 2024, max compression
+gzip compressed data, was "pipeline_telemetry-1.1.0.tar", last modified: Mon May 27 16:19:39 2024, max compression
```

## Comparing `pipeline_telemetry-1.0.2.tar` & `pipeline_telemetry-1.1.0.tar`

### file list

```diff
@@ -1,112 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:29.638623 pipeline_telemetry-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    43679 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-08 14:29:29.638623 pipeline_telemetry-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:29.626623 pipeline_telemetry-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/docs/adding telemetry.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/docs/decorators.rst
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/docs/process_type.rst
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:29.626623 pipeline_telemetry-1.0.2/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/docs/reference/pipeline_telemetry.rst
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/docs/storage class.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/docs/telemetry aggregation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/docs/telemetry counters.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/docs/telemetry mixin.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/docs/telemetry object.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-08 14:29:29.638623 pipeline_telemetry-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:29.618623 pipeline_telemetry-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:29.626623 pipeline_telemetry-1.0.2/src/pipeline_telemetry/
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:29.630623 pipeline_telemetry-1.0.2/src/pipeline_telemetry/aggregator/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/aggregator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/aggregator/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/aggregator/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/aggregator/mongo_aggregator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:29.630623 pipeline_telemetry-1.0.2/src/pipeline_telemetry/data_classes/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/data_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/data_classes/telemetry_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    14116 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:29.630623 pipeline_telemetry-1.0.2/src/pipeline_telemetry/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/settings/data_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/settings/date_ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/settings/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/settings/process_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/settings/telemetry_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:29.630623 pipeline_telemetry-1.0.2/src/pipeline_telemetry/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/storage/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/storage/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/storage/mongo.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/storage/mongo_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:29.630623 pipeline_telemetry-1.0.2/src/pipeline_telemetry/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/validators/abstract_validator_instruction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/validators/dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/validators/entries_have_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/validators/has_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry/validators/validate_entries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:29.638623 pipeline_telemetry-1.0.2/src/pipeline_telemetry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-08 14:29:29.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-08 14:29:29.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:29:29.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-08 14:29:29.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 14:29:29.000000 pipeline_telemetry-1.0.2/src/pipeline_telemetry.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:29.634623 pipeline_telemetry-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_add_telemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:29.634623 pipeline_telemetry-1.0.2/tests/test_aggregator/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_aggregator/test_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_aggregator/test_aggregator_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_aggregator/test_daily_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_aggregator/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_aggregator/test_mongo_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_aggregator/test_partial_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:29.634623 pipeline_telemetry-1.0.2/tests/test_integration/
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_integration/test_int_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_integration/test_integration_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_process_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:29.634623 pipeline_telemetry-1.0.2/tests/test_settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_settings/test_date_time_ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_settings/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_settings_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:29.638623 pipeline_telemetry-1.0.2/tests/test_storage/
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_storage/test_mongo_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    14409 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_storage/test_sqllite_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_storage/test_storage_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_telemetry_class_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_telemetry_counter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:29.638623 pipeline_telemetry-1.0.2/tests/test_telemetry_models/
--rw-r--r--   0 runner    (1001) docker     (127)    16966 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_telemetry_models/test_telemetry_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_telemetry_models/test_telemetry_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_telemetry_models/test_telemetry_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:29.638623 pipeline_telemetry-1.0.2/tests/test_validators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_validators/test_dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_validators/test_entries_have_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_validators/test_has_key_instruction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-05-08 14:29:25.000000 pipeline_telemetry-1.0.2/tests/test_validators/test_validate_entries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:39.801494 pipeline_telemetry-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    43679 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-27 16:19:39.801494 pipeline_telemetry-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:39.789494 pipeline_telemetry-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/docs/adding telemetry.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/docs/decorators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/docs/process_type.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:39.789494 pipeline_telemetry-1.1.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/docs/reference/pipeline_telemetry.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/docs/storage class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/docs/telemetry aggregation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/docs/telemetry counters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/docs/telemetry mixin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/docs/telemetry object.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-27 16:19:39.801494 pipeline_telemetry-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:39.785493 pipeline_telemetry-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:39.789494 pipeline_telemetry-1.1.0/src/pipeline_telemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:39.793494 pipeline_telemetry-1.1.0/src/pipeline_telemetry/aggregator/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/aggregator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/aggregator/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/aggregator/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/aggregator/mongo_aggregator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:39.793494 pipeline_telemetry-1.1.0/src/pipeline_telemetry/data_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/data_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/data_classes/telemetry_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14081 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:39.793494 pipeline_telemetry-1.1.0/src/pipeline_telemetry/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/settings/data_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/settings/date_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/settings/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/settings/process_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/settings/telemetry_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:39.793494 pipeline_telemetry-1.1.0/src/pipeline_telemetry/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/storage/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/storage/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/storage/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/storage/mongo_bunnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/storage/mongo_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:39.797494 pipeline_telemetry-1.1.0/src/pipeline_telemetry/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/validators/abstract_validator_instruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/validators/dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/validators/entries_have_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/validators/has_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry/validators/validate_entries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:39.801494 pipeline_telemetry-1.1.0/src/pipeline_telemetry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-27 16:19:39.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-27 16:19:39.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:19:39.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-27 16:19:39.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-27 16:19:39.000000 pipeline_telemetry-1.1.0/src/pipeline_telemetry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:39.797494 pipeline_telemetry-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_add_telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:39.797494 pipeline_telemetry-1.1.0/tests/test_aggregator/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_aggregator/test_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_aggregator/test_aggregator_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_aggregator/test_daily_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_aggregator/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_aggregator/test_mongo_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_aggregator/test_partial_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:39.797494 pipeline_telemetry-1.1.0/tests/test_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_integration/test_int_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_integration/test_integration_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_process_type_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_process_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:39.797494 pipeline_telemetry-1.1.0/tests/test_settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_settings/test_date_time_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_settings/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_settings_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:39.797494 pipeline_telemetry-1.1.0/tests/test_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_storage/test_mongo_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14409 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_storage/test_sqllite_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_storage/test_storage_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_telemetry_class_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9318 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_telemetry_counter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:39.801494 pipeline_telemetry-1.1.0/tests/test_telemetry_models/
+-rw-r--r--   0 runner    (1001) docker     (127)    16965 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_telemetry_models/test_telemetry_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_telemetry_models/test_telemetry_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_telemetry_models/test_telemetry_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:39.801494 pipeline_telemetry-1.1.0/tests/test_validators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_validators/test_dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_validators/test_entries_have_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_validators/test_has_key_instruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-05-27 16:19:36.000000 pipeline_telemetry-1.1.0/tests/test_validators/test_validate_entries.py
```

### Comparing `pipeline_telemetry-1.0.2/CHANGELOG.rst` & `pipeline_telemetry-1.1.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 
 Changelog
 =========
+1.1.0 (2024-05-27)
+-------------------
+* Added support for Bunnet with pydantic and mongo storage.
+* Added ProcessTypesMeta class to allow for ProcessTypes definition that are recognized by typechecking and linting.
+
+
 1.0.0 (2024-05-08)
 -------------------
 * Added python 3.12 support
 
 0.9.4 (2022-11-03)
 -------------------
 * Added ``PartialToSingleMongoAggregator`` and ``PartialToSingleAggregator``
```

### Comparing `pipeline_telemetry-1.0.2/CONTRIBUTING.rst` & `pipeline_telemetry-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/LICENSE` & `pipeline_telemetry-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/PKG-INFO` & `pipeline_telemetry-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline-telemetry
-Version: 1.0.2
+Version: 1.1.0
 Summary: Measure your data pipelines with easy to use telemetry logic
 Home-page: https://github.com/MaartendeRuyter/pipeline-telemetry
 Author: Maarten de Ruyter
 Author-email: "Maarten de Ruyter" <maarten@geodatagarden.com>
 License: GNU
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: error-manager
 Requires-Dist: mongoengine
 Requires-Dist: jmespath
+Requires-Dist: bunnet
 
 ========
 Overview
 ========
 
 .. start-badges
```

### Comparing `pipeline_telemetry-1.0.2/README.rst` & `pipeline_telemetry-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/docs/adding telemetry.rst` & `pipeline_telemetry-1.1.0/docs/adding telemetry.rst`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/docs/conf.py` & `pipeline_telemetry-1.1.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "Pipeline Telemetry"
 year = "2024"
 author = "Maarten de Ruyter"
 copyright = "{0}, {1}".format(year, author)
-version = release = "1.0.2"
+version = release = "1.1.0"
 
 extensions = []
 
 templates_path = ['_templates']
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 html_theme = "sphinx_rtd_theme"
```

### Comparing `pipeline_telemetry-1.0.2/docs/decorators.rst` & `pipeline_telemetry-1.1.0/docs/decorators.rst`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/docs/process_type.rst` & `pipeline_telemetry-1.1.0/docs/process_type.rst`

 * *Files 11% similar despite different names*

```diff
@@ -150,7 +150,49 @@
         'telemetry_rules': {}
         }
     
     telemetry_obj = Telemetry(**TELEMETRY_LOAD_CLIMATE_DATA)
 
 You can now add telemetry to this telemetry object using subprocess, 'RETRIEVE_CLIMATE_OBJECT_FROM_API', 'CONVERT_TO_YEARLY_CLIMATE_OBJECT' and 
 'STORE_YEARLY_CLIMATE'.
+
+
+Registering process types using a meta class
+--------------------------------------------
+ProcessTypes register methods are dynamically evaluated. Therefore linters, codecompletion and typechecker will not recognize your custom process types and::
+
+    ProcessTypes.YOUR_PROCESS_TYPE
+
+will not pass you're type checker and linter. 
+You can solve this by defining you custom ProcessTypes class based upon the ``ProcessTypesMeta`` class and mixing in any class with ``ProcessType`` class attributes::
+
+    from pipeline_telemetry import ProcessTypesMeta
+
+    class ProcessTypesSet1():
+        CUSTOM_PROCESS = ProcessType(
+            process_type = 'CUSTOM_PROCESS',
+            subtypes = [
+                'SUB_PROCESS_1',
+                'SUB_PROCESS_2']
+        )
+
+    class ProcessTypesSet2():
+        OTHER_CUSTOM_PROCESS = ProcessType(
+            process_type = 'OTHER_CUSTOM_PROCESS',
+            subtypes = [
+                'SUB_PROCESS_1',
+                'SUB_PROCESS_2']
+        )
+
+    cls MyProcessTypes(ProcessTypesSet1, ProcessTypesSet2, metaclass=ProcessTypesMeta): ...
+
+The ``MyProcessTypes`` class now acts as a ProcessTypes class (it is actually a subclass of ProcessTypes) with CUSTOM_PROCESS and OTHER_CUSTOM_PROCESS as ProcessType attributes.::
+
+    MyProcessTypes.CUSTOM_PROCESS
+    MyProcessTypes.OTHER_CUSTOM_PROCESS
+
+Now pass your linting and type checker and will autocomplete in your IDE.
+
+
+
+
+
```

### Comparing `pipeline_telemetry-1.0.2/docs/telemetry aggregation.rst` & `pipeline_telemetry-1.1.0/docs/telemetry aggregation.rst`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/docs/telemetry counters.rst` & `pipeline_telemetry-1.1.0/docs/telemetry counters.rst`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         telemetry.save_and_close()
 
 In this example two telemetry_counters define in a counters module are added to the telemetry object. In case of successful processing of data object the number of processed data points is added to the counter defined in PROCESSED_DATA_POINTS telemetry_counter
 
 set_increment
 -------------
 
-When a telemetry counter is added to a result in a different class from where the telementry object is stored you will not be able to overide the increment when adding the counter to the telemetry object (See previous example). As ``TelementryCounter`` object is non mutable is not possible to update the increment in the predefined counter object. The ``set_increment`` method was created to bypass this. Calling the method with the new increment as argument on an existing counter will return a copy of that counter with an updated increment.::
+When a telemetry counter is added to a result in a different class from where the telemetry object is stored you will not be able to overide the increment when adding the counter to the telemetry object (See previous example). As ``TelemetryCounter`` object is non mutable is not possible to update the increment in the predefined counter object. The ``set_increment`` method was created to bypass this. Calling the method with the new increment as argument on an existing counter will return a copy of that counter with an updated increment.::
 
     >>> form settings import PREDEFINED_COUNTER
     >>> PREDEFINED_COUNTER.increment
     1
     >>> new_counter = PREDEFINED_COUNTER.set_increment(increment=10)
     >>> new_counter.increment
     10
```

### Comparing `pipeline_telemetry-1.0.2/docs/telemetry mixin.rst` & `pipeline_telemetry-1.1.0/docs/telemetry mixin.rst`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/docs/telemetry object.rst` & `pipeline_telemetry-1.1.0/docs/telemetry object.rst`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/docs/usage.rst` & `pipeline_telemetry-1.1.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/setup.cfg` & `pipeline_telemetry-1.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pipeline-telemetry
-version = 1.0.2
+version = 1.1.0
 description = Measure your data pipelines with easy to use telemetry logic
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/MaartendeRuyter/pipeline-telemetry
 author = Maarten de Ruyter
 author_email = "Maarten de Ruyter" <maarten@geodatagarden.com>
 license = GNU
@@ -24,14 +24,15 @@
 	=src
 packages = find:
 include_package_data = True
 install_requires = 
 	error-manager
 	mongoengine
 	jmespath
+	bunnet
 
 [options.packages.find]
 where = src
 exclude = 
 	test*
 
 [mypy]
@@ -67,14 +68,15 @@
 envlist = py310, py311, py312
 isolated_build = True
 
 [testenv]
 deps = 
 	error-manager
 	mongoengine
+	bunnet
 	freezegun
 	jmespath
 	pymongo>=4.7
 	pytest
 	pytest-cov
 	pytest-mock
 commands =
```

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry/__init__.py` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     >>> telemetry = Telemetry(
             source_name, process_type, telemetry_rules, storage_class)
     >>> pipeline_telemetry.add(sub_process_type, data, errors)
     >>> pipeline_telemetry.save_and_close()
 
 In this example a telemetry object is created, the result of a sub_process is
 then added with either the data resulting from this sub process or the error
-that the sub process returned. In the final step the telementry is saved and
+that the sub process returned. In the final step the telemetry is saved and
 closed
 
 Arguments
     - source_name (str):
         Process name for the pipeline process that this telemetry is reporting
         on. Name is free to choose but make sure it is a unique name for each
         unique process as it will otherwise be difficult to use the telemetry
@@ -60,17 +60,22 @@
     increase_fail_count,
     is_telemetry_counter,
     process_return_value,
 )
 from .main import Telemetry
 from .mixin import TelemetryMixin
 from .settings.data_class import ProcessType, TelemetryCounter
-from .settings.process_type import ProcessTypes
+from .settings.process_type import ProcessTypes, ProcessTypesMeta
 from .settings.settings import BaseEnumerator, DefaultProcessTypes
 from .settings.telemetry_errors import ValidationErrors
+from .storage.mongo_bunnet import (
+    TelemetryBunnetModel,
+    TelemetryBunnetStorage,
+    init_database,
+)
 from .validators import DictValidator, EntriesHaveKey, HasKey, ValidateEntries
 
 __all__ = [
     "DailyAggregator",
     "DailyMongoAggregator",
     "PartialToSingleAggregator",
     "PartialToSingleMongoAggregator",
@@ -85,16 +90,20 @@
     "increase_base_count",
     "increase_fail_count",
     "is_telemetry_counter",
     "process_return_value",
     "Telemetry",
     "TelemetryMixin",
     "ProcessType",
+    "ProcessTypesMeta",
     "TelemetryCounter",
     "BaseEnumerator",
+    "init_database",
+    "TelemetryBunnetModel",
+    "TelemetryBunnetStorage",
 ]
 
 ProcessTypes.register_process_types(DefaultProcessTypes)
 ListErrors.register_errors(ValidationErrors)
 
 DictValidator.register_instruction(ValidateEntries)
 DictValidator.register_instruction(HasKey)
```

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry/aggregator/aggregator.py` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry/aggregator/aggregator.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         """
         # gather the database instances to be aggregated
         telemetry_list_params = self._telememtry_list_params(date_time_range)._asdict()
         telemetry_objects = self.__telemetry_storage.telemetry_list(
             **telemetry_list_params
         )
 
-        initial_telemetry_obj = self.__target_telemetry.copy()
+        initial_telemetry_obj = self.__target_telemetry.telemetry_copy()
         aggregator = self.__aggregator(initial_telemetry_obj)
         aggregated_telemetry = aggregator.aggregate(telemetry_objects)
 
         return self._set_start_date_time_for_aggregated_telemetry(
             aggregated_telemetry, date_time_range
         )
```

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry/aggregator/helper.py` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry/aggregator/helper.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry/aggregator/mongo_aggregator.py` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry/aggregator/mongo_aggregator.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry/data_classes/telemetry_models.py` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry/data_classes/telemetry_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,25 @@
 
 - TelemetryModel: Data class to define the Telemetry object category, type,
                   source etc. Holds the reference to the actual counters defined
                   in TelemetryData dataclass.
 """
 
 from collections import defaultdict
-from dataclasses import dataclass, field
 from datetime import datetime
-from typing import DefaultDict, Dict, Optional
+from typing import DefaultDict, Dict
 
 from errors import ErrorCode
+from pydantic import BaseModel, Field, field_validator
 
 from pipeline_telemetry.settings import exceptions
 from pipeline_telemetry.settings import settings as st
 
 
-@dataclass
-class TelemetryData:
+class TelemetryData(BaseModel):
     """
     Class to define the telemetry (error)counters.
 
     attributes:
     - base_counter (int): counter for the TelemetryData object.
     - fail_counter (int): fail counter for the TelemetryData object.
     - counters (dict): dict of sub (custom) counters [str: int]
@@ -42,16 +41,16 @@
     counters can be added in which case base, fail, custom and error counters
     will be summed up seperately. Add method will return self with added
     TelemetryData object.
     """
 
     base_counter: int = 0
     fail_counter: int = 0
-    counters: DefaultDict[str, int] = field(default_factory=lambda: defaultdict(int))
-    errors: DefaultDict[str, int] = field(default_factory=lambda: defaultdict(int))
+    counters: DefaultDict[str, int] = Field(default_factory=lambda: defaultdict(int))
+    errors: DefaultDict[str, int] = Field(default_factory=lambda: defaultdict(int))
 
     def increase_base_count(self, increment: int) -> None:
         """Increase the base counter with a given increment."""
         self.base_counter += increment
 
     def increase_fail_count(self, increment: int) -> None:
         """Increase the fail counter with a given increment."""
@@ -81,69 +80,67 @@
                 increment=increment, error_code_key=error_code_key
             )
         for counter, increment in telemetry_data.counters.items():
             self.increase_custom_count(increment=increment, counter=counter)
         return self
 
 
-@dataclass
-class TelemetryModel:
+class TelemetryModel(BaseModel):
     telemetry_type: str
     category: str
     sub_category: str
     source_name: str
     process_type: str
     start_date_time: datetime = datetime.now()
-    run_time_in_seconds: Optional[float] = None
+    run_time_in_seconds: float = 0
     io_time_in_seconds: float = 0
     traffic_light: str = st.DEFAULT_TRAFIC_LIGHT_COLOR
-    telemetry: Dict[str, TelemetryData] = field(default_factory=dict)
+    telemetry: Dict[str, TelemetryData] = Field(default_factory=dict)
 
-    def validate(self) -> None:
-        self._check_telemetry_type()
-
-    def copy(self) -> "TelemetryModel":
+    def telemetry_copy(self) -> "TelemetryModel":
         """
         Method to return a copy of the telemetry model. In a telemetry copy
         only the attributes telemetry_type, categroy, sub_category, source_name
         and process_type are copied.
         """
         return TelemetryModel(
             telemetry_type=self.telemetry_type,
             category=self.category,
             sub_category=self.sub_category,
             source_name=self.source_name,
             process_type=self.process_type,
         )
 
-    def _check_telemetry_type(self) -> None:
+    @field_validator("telemetry_type")
+    def _check_telemetry_type(cls, value) -> None:
         """Check validaty of provided telemetry type.
 
         Raises exception if not valid. Returns non if telemetry type is valid.
 
         Args:
             telemetry_type (str): [description]
 
         Raises:
             exceptions.InvalidTelemetryType: When telemetry type is not valid.
         """
-        if self.telemetry_type not in st.TELEMETRY_TYPES:
+        if value not in st.TELEMETRY_TYPES:
             raise exceptions.InvalidTelemetryType(st.TELEMETRY_TYPES)
+        return value
 
     def set_orange_traffic_light(self) -> None:
         """Sets traffic light attribute to orange."""
         self.traffic_light = st.TRAFIC_LIGHT_COLOR_ORANGE
 
     def set_red_traffic_light(self) -> None:
         """Sets traffic light attribute to red."""
         self.traffic_light = st.TRAFIC_LIGHT_COLOR_RED
 
     def __add__(self, telemetry_model_to_add: "TelemetryModel") -> "TelemetryModel":
         """
-        Method to add to telementry model instances.
+        Method to add to telemetry model instances.
         Adding a 2 telemetry model instances implies adding all telemetry data
         objects and adding iotime, run time and traffic light attributes to a
         specific counter.
         """
         self.__add_base_count()
         self.__add_sub_process(telemetry_model_to_add=telemetry_model_to_add)
         self.__add_traffic_light(telemetry_model_to_add=telemetry_model_to_add)
```

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry/decorator.py` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry/decorator.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry/helper.py` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry/helper.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry/main.py` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
         self._telemetry = TelemetryModel(
             telemetry_type=telemetry_type,
             category=category,
             sub_category=sub_category,
             source_name=source_name,
             process_type=process_type.name,
         )
-        self._telemetry.validate()
 
     @classmethod
     def add_process_type(cls, process_type_key: str, process_type: ProcessType) -> None:
         """
         Add a custom process type to the available process types to the
         already registered process types.
```

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry/mixin.py` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry/mixin.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry/settings/__init__.py` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry/settings/data_class.py` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry/settings/data_class.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry/settings/date_ranges.py` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry/settings/date_ranges.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry/settings/exceptions.py` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry/settings/exceptions.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry/settings/settings.py` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry/settings/settings.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry/settings/telemetry_errors.py` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry/settings/telemetry_errors.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry/storage/generic.py` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry/storage/generic.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry/storage/memory.py` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry/storage/memory.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry/storage/mongo.py` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry/storage/mongo.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry/storage/mongo_connection.py` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry/storage/mongo_connection.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry/validators/abstract_validator_instruction.py` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry/validators/abstract_validator_instruction.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry/validators/dict_validator.py` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry/validators/dict_validator.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry/validators/entries_have_key.py` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry/validators/entries_have_key.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry/validators/has_key.py` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry/validators/has_key.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry/validators/validate_entries.py` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry/validators/validate_entries.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry.egg-info/PKG-INFO` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline-telemetry
-Version: 1.0.2
+Version: 1.1.0
 Summary: Measure your data pipelines with easy to use telemetry logic
 Home-page: https://github.com/MaartendeRuyter/pipeline-telemetry
 Author: Maarten de Ruyter
 Author-email: "Maarten de Ruyter" <maarten@geodatagarden.com>
 License: GNU
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: error-manager
 Requires-Dist: mongoengine
 Requires-Dist: jmespath
+Requires-Dist: bunnet
 
 ========
 Overview
 ========
 
 .. start-badges
```

### Comparing `pipeline_telemetry-1.0.2/src/pipeline_telemetry.egg-info/SOURCES.txt` & `pipeline_telemetry-1.1.0/src/pipeline_telemetry.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -49,26 +49,28 @@
 src/pipeline_telemetry/settings/process_type.py
 src/pipeline_telemetry/settings/settings.py
 src/pipeline_telemetry/settings/telemetry_errors.py
 src/pipeline_telemetry/storage/__init__.py
 src/pipeline_telemetry/storage/generic.py
 src/pipeline_telemetry/storage/memory.py
 src/pipeline_telemetry/storage/mongo.py
+src/pipeline_telemetry/storage/mongo_bunnet.py
 src/pipeline_telemetry/storage/mongo_connection.py
 src/pipeline_telemetry/validators/__init__.py
 src/pipeline_telemetry/validators/abstract_validator_instruction.py
 src/pipeline_telemetry/validators/dict_validator.py
 src/pipeline_telemetry/validators/entries_have_key.py
 src/pipeline_telemetry/validators/has_key.py
 src/pipeline_telemetry/validators/validate_entries.py
 tests/test_add_telemetry.py
 tests/test_data.py
 tests/test_decorator.py
 tests/test_helpers.py
 tests/test_mixin.py
+tests/test_process_type_meta.py
 tests/test_process_types.py
 tests/test_settings_module.py
 tests/test_telemetry_class_methods.py
 tests/test_telemetry_counter.py
 tests/test_aggregator/test_aggregator.py
 tests/test_aggregator/test_aggregator_data.py
 tests/test_aggregator/test_daily_aggregator.py
```

### Comparing `pipeline_telemetry-1.0.2/tests/test_add_telemetry.py` & `pipeline_telemetry-1.1.0/tests/test_add_telemetry.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/tests/test_aggregator/test_aggregator.py` & `pipeline_telemetry-1.1.0/tests/test_aggregator/test_aggregator.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/tests/test_aggregator/test_aggregator_data.py` & `pipeline_telemetry-1.1.0/tests/test_aggregator/test_aggregator_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from datetime import date, datetime, timedelta
 from typing import Iterator, List
 
-from test_data import DEFAULT_TELEMETRY_MODEL_PARAMS, DEFAULT_TELEMETRY_PARAMS
+from test_data import DEFAULT_TELEMETRY_MODEL_PARAMS, DEFAULT_TELEMETRY_SELECTOR_PARAMS
 
 from pipeline_telemetry import TelemetrySelector
 from pipeline_telemetry.data_classes import TelemetryData, TelemetryModel
 
-TEST_TELEMETRY_SELECTOR = TelemetrySelector(**DEFAULT_TELEMETRY_PARAMS)
+TEST_TELEMETRY_SELECTOR = TelemetrySelector(**DEFAULT_TELEMETRY_SELECTOR_PARAMS)
 
 TODAY = date.today()
 YESTERDAY = date.today() - timedelta(days=1)
 DAY_BEFORE_YESTERDAY = date.today() - timedelta(days=2)
 
 TELEMETRY_MODEL_1 = TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS)
```

### Comparing `pipeline_telemetry-1.0.2/tests/test_aggregator/test_daily_aggregator.py` & `pipeline_telemetry-1.1.0/tests/test_aggregator/test_daily_aggregator.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/tests/test_aggregator/test_helper.py` & `pipeline_telemetry-1.1.0/tests/test_aggregator/test_helper.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/tests/test_aggregator/test_mongo_aggregator.py` & `pipeline_telemetry-1.1.0/tests/test_aggregator/test_mongo_aggregator.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/tests/test_aggregator/test_partial_aggregator.py` & `pipeline_telemetry-1.1.0/tests/test_aggregator/test_partial_aggregator.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/tests/test_data.py` & `pipeline_telemetry-1.1.0/tests/test_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,21 @@
 DEFAULT_TELEMETRY_PARAMS = {
     "category": "WEATHER",
     "sub_category": "DAILY_PREDICTIONS",
     "source_name": "load_weather_data",
     "process_type": ProcessTypes.CREATE_DATA_FROM_URL,
 }
 
+DEFAULT_TELEMETRY_SELECTOR_PARAMS = {
+    "category": "WEATHER",
+    "sub_category": "DAILY_PREDICTIONS",
+    "source_name": "load_weather_data",
+    "process_type": ProcessTypes.CREATE_DATA_FROM_URL.name,
+}
+
 DEFAULT_TELEMETRY_MODEL_PARAMS = {
     "telemetry_type": "SINGLE TELEMETRY",
     "category": "WEATHER",
     "sub_category": "DAILY_PREDICTIONS",
     "source_name": "load_weather_data",
     "process_type": ProcessTypes.CREATE_DATA_FROM_URL.name,
 }
```

### Comparing `pipeline_telemetry-1.0.2/tests/test_decorator.py` & `pipeline_telemetry-1.1.0/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/tests/test_helpers.py` & `pipeline_telemetry-1.1.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/tests/test_integration/test_int_telemetry.py` & `pipeline_telemetry-1.1.0/tests/test_integration/test_int_telemetry.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/tests/test_integration/test_integration_data.py` & `pipeline_telemetry-1.1.0/tests/test_integration/test_integration_data.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/tests/test_mixin.py` & `pipeline_telemetry-1.1.0/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/tests/test_process_types.py` & `pipeline_telemetry-1.1.0/tests/test_process_types.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/tests/test_settings/test_date_time_ranges.py` & `pipeline_telemetry-1.1.0/tests/test_settings/test_date_time_ranges.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/tests/test_settings/test_exceptions.py` & `pipeline_telemetry-1.1.0/tests/test_settings/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/tests/test_storage/test_mongo_storage.py` & `pipeline_telemetry-1.1.0/tests/test_storage/test_mongo_storage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """Module to test storage module."""
 
 from datetime import datetime, timedelta
 
 from test_data import DEFAULT_TELEMETRY_MODEL_PARAMS
 
 from pipeline_telemetry.data_classes import TelemetryModel
-from pipeline_telemetry.settings.settings import DEFAULT_TRAFIC_LIGHT_COLOR, RUN_TIME
+from pipeline_telemetry.settings.settings import (
+    DEFAULT_TRAFIC_LIGHT_COLOR,
+    RUN_TIME,
+    SINGLE_TELEMETRY_TYPE,
+)
 from pipeline_telemetry.storage.mongo import TelemetryMongoModel, TelemetryMongoStorage
 from pipeline_telemetry.storage.mongo_connection import get_mongo_db_port
 
 
 def telemetry_query_params():
     """Returns a default set of query params"""
     return DEFAULT_TELEMETRY_MODEL_PARAMS | {
@@ -40,45 +44,47 @@
         return_value={},
     )
     _telemetry_model_kwargs_spy = mocker.spy(
         TelemetryMongoStorage, "_telemetry_model_kwargs"
     )
     _telemetry_mongo_model_new_spy = mocker.spy(TelemetryMongoModel, "__new__")
     _telemetry_mongo_model_save_spy = mocker.spy(TelemetryMongoModel, "save")
-    TelemetryMongoStorage().store_telemetry(telemetry={"source_name": "test"})
+    TelemetryMongoStorage().store_telemetry(telemetry={
+        "source_name": "test"})  # type: ignore
     assert _telemetry_model_kwargs_spy.called
     assert _telemetry_mongo_model_new_spy.called
     assert _telemetry_mongo_model_save_spy.called
 
 
 def test_telemetry_model_kwargs_method():
     """Test _telemetry_model_kwargs method returns correct kwargs."""
+    current_time = datetime.now()
     result = TelemetryMongoStorage()._telemetry_model_kwargs(
         TelemetryModel(
             **{
-                "telemetry_type": "test telemetry type",
+                "telemetry_type": SINGLE_TELEMETRY_TYPE,
                 "category": "test",
                 "sub_category": "sub_test",
                 "source_name": "tst_source_name",
                 "process_type": "tst_process_type",
-                "start_date_time": "tst_start_date_time",
+                "start_date_time": current_time,
                 "run_time_in_seconds": 1.123,
                 "io_time_in_seconds": 1.1,
                 "traffic_light": DEFAULT_TRAFIC_LIGHT_COLOR,
             }
         )
     )
 
     assert result == {
-        "telemetry_type": "test telemetry type",
+        "telemetry_type": SINGLE_TELEMETRY_TYPE,
         "category": "test",
         "sub_category": "sub_test",
         "source_name": "tst_source_name",
         "process_type": "tst_process_type",
-        "start_date_time": "tst_start_date_time",
+        "start_date_time": current_time,
         "run_time_in_seconds": "1.12",
         "io_time_in_seconds": 1.1,
         "telemetry": {},
         "traffic_light": DEFAULT_TRAFIC_LIGHT_COLOR,
     }
```

### Comparing `pipeline_telemetry-1.0.2/tests/test_storage/test_sqllite_storage.py` & `pipeline_telemetry-1.1.0/tests/test_storage/test_sqllite_storage.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/tests/test_telemetry_class_methods.py` & `pipeline_telemetry-1.1.0/tests/test_telemetry_class_methods.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/tests/test_telemetry_counter.py` & `pipeline_telemetry-1.1.0/tests/test_telemetry_counter.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,62 +218,62 @@
         counter_name=TD.TEST_TELEMETRY_COUNTER.counter_name,
     )
     assert counter.increment == 1
     new_counter = counter.set_increment(increment=10)
     assert new_counter.increment == 10
 
 
-def test_telementry_counter_hash():
+def test_telemetry_counter_hash():
     """Test that a TelemetryCounter object can be hashed."""
     assert TD.TEST_TELEMETRY_COUNTER.__hash__()
 
 
 def test_tc_hash_does_include_the_increment():
     """Test that increment value changes the hash."""
     assert (
         not TD.TEST_TELEMETRY_COUNTER.__hash__()
         == TD.TEST_TELEMETRY_COUNTER_INC_2.__hash__()
     )
 
 
 def test_tc_hash_works_with_errors():
     """
-    Test that a telementry counters with different errors return a different
+    Test that a telemetry counters with different errors return a different
     hash.
     """
     assert (
         not TD.TEST_ERROR_TELEMETRY_COUNTER.__hash__()
         == TD.TEST_ERROR_TELEMETRY_COUNTER_2.__hash__()
     )
 
 
 def test_tc_hash_works_with_counters():
     """
-    Test that a telementry counters with different counters return a different
+    Test that a telemetry counters with different counters return a different
     hash.
     """
     assert (
         not TD.TEST_TELEMETRY_COUNTER.__hash__()
         == TD.TEST_TELEMETRY_COUNTER_2.__hash__()
     )
 
 
 def test_tc_hash_does_include_process_types_field():
     """
-    Test that a telementry counters with a different list of process types
+    Test that a telemetry counters with a different list of process types
     return a different hash.
     """
     assert (
         not TD.TEST_TC_MULT_PROCESS_TYPES.__hash__()
         == TD.TEST_TC_MULT_PROCESS_TYPES_2.__hash__()
     )
 
 
 def test_tc_hash_does_include_sub_process_field():
     """
-    Test that a telementry counters with a different sub_process
+    Test that a telemetry counters with a different sub_process
     return a different hash.
     """
     assert (
         not TD.TEST_TELEMETRY_COUNTER.__hash__()
         == TD.TEST_TELEMETRY_COUNTER_3.__hash__()
     )
```

### Comparing `pipeline_telemetry-1.0.2/tests/test_telemetry_models/test_telemetry_class.py` & `pipeline_telemetry-1.1.0/tests/test_telemetry_models/test_telemetry_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
     with pytest.raises(exceptions.TelemetryObjectAlreadyClosed):
         telemetry_inst.increase_sub_process_fail_count("RETRIEVE_RAW_DATA")
 
 
 def test_sub_process_custom_count_not_allowed_with_closed_telemetry():
     """
     check that a sub process custom count method raises an excpetion
-    when telementry object has been closed
+    when telemetry object has been closed
     """
     telemetry_inst = Telemetry(**DEFAULT_TELEMETRY_PARAMS)
     telemetry_inst.increase_sub_process_base_count("RETRIEVE_RAW_DATA")
     telemetry_inst.save_and_close()
     with pytest.raises(exceptions.TelemetryObjectAlreadyClosed):
         telemetry_inst.increase_sub_process_custom_count(
             sub_process="RETRIEVE_RAW_DATA", custom_counter="test_counter"
```

### Comparing `pipeline_telemetry-1.0.2/tests/test_telemetry_models/test_telemetry_data.py` & `pipeline_telemetry-1.1.0/tests/test_telemetry_models/test_telemetry_data.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/tests/test_telemetry_models/test_telemetry_model.py` & `pipeline_telemetry-1.1.0/tests/test_telemetry_models/test_telemetry_model.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/tests/test_validators/test_dict_validator.py` & `pipeline_telemetry-1.1.0/tests/test_validators/test_dict_validator.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/tests/test_validators/test_entries_have_key.py` & `pipeline_telemetry-1.1.0/tests/test_validators/test_entries_have_key.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/tests/test_validators/test_has_key_instruction.py` & `pipeline_telemetry-1.1.0/tests/test_validators/test_has_key_instruction.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.2/tests/test_validators/test_validate_entries.py` & `pipeline_telemetry-1.1.0/tests/test_validators/test_validate_entries.py`

 * *Files identical despite different names*

