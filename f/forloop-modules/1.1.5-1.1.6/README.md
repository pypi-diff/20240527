# Comparing `tmp/forloop_modules-1.1.5.tar.gz` & `tmp/forloop_modules-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forloop_modules-1.1.5.tar", last modified: Fri May 24 13:02:45 2024, max compression
+gzip compressed data, was "forloop_modules-1.1.6.tar", last modified: Mon May 27 18:10:02 2024, max compression
```

## Comparing `forloop_modules-1.1.5.tar` & `forloop_modules-1.1.6.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 13:02:45.598657 forloop_modules-1.1.5/
--rw-rw-rw-   0        0        0     1525 2024-02-22 17:34:45.000000 forloop_modules-1.1.5/LICENSE
--rw-rw-rw-   0        0        0      658 2024-05-24 13:02:45.597787 forloop_modules-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      155 2024-02-22 17:34:45.000000 forloop_modules-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 13:02:45.127397 forloop_modules-1.1.5/forloop_modules/
--rw-rw-rw-   0        0        0      179 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 13:02:45.148686 forloop_modules-1.1.5/forloop_modules/errors/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/errors/__init__.py
--rw-rw-rw-   0        0        0     1670 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/errors/errors.py
--rw-rw-rw-   0        0        0     9860 2024-03-12 11:46:28.000000 forloop_modules-1.1.5/forloop_modules/flog.py
-drwxrwxrwx   0        0        0        0 2024-05-24 13:02:45.344540 forloop_modules-1.1.5/forloop_modules/function_handlers/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/__init__.py
--rw-rw-rw-   0        0        0     6781 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/api_endpoint_handlers.py
--rw-rw-rw-   0        0        0    22200 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/api_handlers.py
-drwxrwxrwx   0        0        0        0 2024-05-24 13:02:45.386147 forloop_modules-1.1.5/forloop_modules/function_handlers/auxilliary/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/auxilliary/__init__.py
--rw-rw-rw-   0        0        0    17835 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/auxilliary/abstract_function_handler.py
--rw-rw-rw-   0        0        0      807 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/auxilliary/auxiliary_functions.py
--rw-rw-rw-   0        0        0     2061 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/auxilliary/data_types_validation.py
--rw-rw-rw-   0        0        0     1047 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/auxilliary/docs.py
--rw-rw-rw-   0        0        0     1940 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/auxilliary/forloop_code_eval.py
--rw-rw-rw-   0        0        0     7933 2024-05-03 13:07:28.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/auxilliary/form_dict_list.py
--rw-rw-rw-   0        0        0     2169 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/auxilliary/node_type_categories_manager.py
--rw-rw-rw-   0        0        0    25173 2024-05-03 13:07:28.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/browser_handlers.py
--rw-rw-rw-   0        0        0   204411 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/cleaning_handlers.py
--rw-rw-rw-   0        0        0    12333 2024-05-16 23:27:10.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/control_flow_handlers.py
--rw-rw-rw-   0        0        0    46277 2024-03-21 12:02:54.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/data_handlers.py
--rw-rw-rw-   0        0        0    72995 2024-04-08 16:56:40.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/database_handlers.py
--rw-rw-rw-   0        0        0    30031 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/datetime_handlers.py
--rw-rw-rw-   0        0        0    14696 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/file_managment_handlers.py
--rw-rw-rw-   0        0        0    83412 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/integration_handlers.py
--rw-rw-rw-   0        0        0    27439 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/mapping_handlers.py
--rw-rw-rw-   0        0        0    14152 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/model_handlers.py
--rw-rw-rw-   0        0        0     2778 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/orchestration_handlers.py
--rw-rw-rw-   0        0        0    16250 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/rpa_handlers.py
-drwxrwxrwx   0        0        0        0 2024-05-24 13:02:45.413071 forloop_modules-1.1.5/forloop_modules/function_handlers/transformations/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/transformations/__init__.py
--rw-rw-rw-   0        0        0    14097 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/transformations/basic_transforms.py
--rw-rw-rw-   0        0        0    10448 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/transformations/imputation.py
--rw-rw-rw-   0        0        0     4092 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/transformations/outliers.py
--rw-rw-rw-   0        0        0    59084 2024-05-24 13:02:30.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/variable_handlers.py
--rw-rw-rw-   0        0        0   103428 2024-05-24 13:02:30.000000 forloop_modules-1.1.5/forloop_modules/function_handlers/webscraping_handlers.py
-drwxrwxrwx   0        0        0        0 2024-05-24 13:02:45.453635 forloop_modules-1.1.5/forloop_modules/globals/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/globals/__init__.py
--rw-rw-rw-   0        0        0     5162 2024-05-03 13:07:28.000000 forloop_modules-1.1.5/forloop_modules/globals/active_entity_tracker.py
--rw-rw-rw-   0        0        0     1871 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/globals/database_utilities_handler.py
--rw-rw-rw-   0        0        0     8917 2024-05-21 18:30:50.000000 forloop_modules-1.1.5/forloop_modules/globals/db_connection.py
--rw-rw-rw-   0        0        0     8030 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/globals/dbtables_loader_popups.py
--rw-rw-rw-   0        0        0      223 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/globals/docs_categories.py
--rw-rw-rw-   0        0        0    18806 2024-05-16 23:27:10.000000 forloop_modules-1.1.5/forloop_modules/globals/local_variable_handler.py
--rw-rw-rw-   0        0        0    33426 2024-05-24 13:02:30.000000 forloop_modules-1.1.5/forloop_modules/globals/scraping_utilities_handler.py
--rw-rw-rw-   0        0        0     9133 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/globals/variable_handler.py
-drwxrwxrwx   0        0        0        0 2024-05-24 13:02:45.467646 forloop_modules-1.1.5/forloop_modules/integrations/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/integrations/__init__.py
--rw-rw-rw-   0        0        0     2082 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/integrations/slack_integration.py
--rw-rw-rw-   0        0        0     3580 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/integrations/testing_check_slack_notifications.py
--rw-rw-rw-   0        0        0    14244 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/node_detail_form.py
--rw-rw-rw-   0        0        0    10856 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/pipeline_function_handlers.py
-drwxrwxrwx   0        0        0        0 2024-05-24 13:02:45.489644 forloop_modules-1.1.5/forloop_modules/queries/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/queries/__init__.py
--rw-rw-rw-   0        0        0     2888 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/queries/context_request_backend_auxiliary_functions.py
--rw-rw-rw-   0        0        0    21803 2024-05-16 23:27:10.000000 forloop_modules-1.1.5/forloop_modules/queries/db_model_templates.py
--rw-rw-rw-   0        0        0    42315 2024-05-21 18:30:50.000000 forloop_modules-1.1.5/forloop_modules/queries/node_context_requests_backend.py
-drwxrwxrwx   0        0        0        0 2024-05-24 13:02:45.495612 forloop_modules-1.1.5/forloop_modules/redis/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/redis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 13:02:45.508706 forloop_modules-1.1.5/forloop_modules/redis/config/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/redis/config/__init__.py
--rw-rw-rw-   0        0        0     2063 2024-05-17 06:48:31.000000 forloop_modules-1.1.5/forloop_modules/redis/config/config.py
--rw-rw-rw-   0        0        0     6573 2024-05-16 23:27:10.000000 forloop_modules-1.1.5/forloop_modules/redis/redis_connection.py
-drwxrwxrwx   0        0        0        0 2024-05-24 13:02:45.589776 forloop_modules-1.1.5/forloop_modules/utils/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/utils/__init__.py
--rw-rw-rw-   0        0        0     5587 2024-04-08 16:56:40.000000 forloop_modules-1.1.5/forloop_modules/utils/definitions.py
--rw-rw-rw-   0        0        0     1024 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/utils/encryption.py
--rw-rw-rw-   0        0        0     3393 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/utils/pandas_operations.py
--rw-rw-rw-   0        0        0     3545 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/utils/pickle_serializer.py
--rw-rw-rw-   0        0        0     3190 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/utils/script_utils.py
--rw-rw-rw-   0        0        0     2021 2024-05-03 13:07:28.000000 forloop_modules-1.1.5/forloop_modules/utils/sse_parser.py
--rw-rw-rw-   0        0        0     1622 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/utils/str_helpers.py
--rw-rw-rw-   0        0        0      856 2024-04-08 16:56:40.000000 forloop_modules-1.1.5/forloop_modules/utils/synchronization_flags.py
--rw-rw-rw-   0        0        0     4570 2024-04-08 16:56:40.000000 forloop_modules-1.1.5/forloop_modules/utils/url_template_builder.py
--rw-rw-rw-   0        0        0     3558 2024-02-29 13:17:45.000000 forloop_modules-1.1.5/forloop_modules/utils/various.py
-drwxrwxrwx   0        0        0        0 2024-05-24 13:02:45.142380 forloop_modules-1.1.5/forloop_modules.egg-info/
--rw-rw-rw-   0        0        0      658 2024-05-24 13:02:44.000000 forloop_modules-1.1.5/forloop_modules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3529 2024-05-24 13:02:45.000000 forloop_modules-1.1.5/forloop_modules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 13:02:44.000000 forloop_modules-1.1.5/forloop_modules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-05-24 13:02:44.000000 forloop_modules-1.1.5/forloop_modules.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 13:02:45.598657 forloop_modules-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      786 2024-05-24 13:02:19.000000 forloop_modules-1.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-24 13:02:45.597787 forloop_modules-1.1.5/tests/
--rw-rw-rw-   0        0        0        0 2024-02-22 17:34:45.000000 forloop_modules-1.1.5/tests/__init__.py
--rw-rw-rw-   0        0        0     3316 2024-04-08 16:56:40.000000 forloop_modules-1.1.5/tests/test_url_template_builder.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:10:02.309815 forloop_modules-1.1.6/
+-rw-rw-rw-   0        0        0     1525 2024-02-22 17:34:45.000000 forloop_modules-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0      658 2024-05-27 18:10:02.309815 forloop_modules-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      155 2024-02-22 17:34:45.000000 forloop_modules-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 18:10:02.241624 forloop_modules-1.1.6/forloop_modules/
+-rw-rw-rw-   0        0        0      179 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:10:02.256639 forloop_modules-1.1.6/forloop_modules/errors/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/errors/__init__.py
+-rw-rw-rw-   0        0        0     1670 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/errors/errors.py
+-rw-rw-rw-   0        0        0     9860 2024-03-12 11:46:28.000000 forloop_modules-1.1.6/forloop_modules/flog.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:10:02.271296 forloop_modules-1.1.6/forloop_modules/function_handlers/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/__init__.py
+-rw-rw-rw-   0        0        0     6781 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/api_endpoint_handlers.py
+-rw-rw-rw-   0        0        0    22200 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/api_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:10:02.278805 forloop_modules-1.1.6/forloop_modules/function_handlers/auxilliary/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/auxilliary/__init__.py
+-rw-rw-rw-   0        0        0    17835 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/auxilliary/abstract_function_handler.py
+-rw-rw-rw-   0        0        0      807 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/auxilliary/auxiliary_functions.py
+-rw-rw-rw-   0        0        0     2061 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/auxilliary/data_types_validation.py
+-rw-rw-rw-   0        0        0     1047 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/auxilliary/docs.py
+-rw-rw-rw-   0        0        0     1940 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/auxilliary/forloop_code_eval.py
+-rw-rw-rw-   0        0        0     7933 2024-05-03 13:07:28.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/auxilliary/form_dict_list.py
+-rw-rw-rw-   0        0        0     2169 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/auxilliary/node_type_categories_manager.py
+-rw-rw-rw-   0        0        0    26342 2024-05-26 04:09:02.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/browser_handlers.py
+-rw-rw-rw-   0        0        0   204411 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/cleaning_handlers.py
+-rw-rw-rw-   0        0        0    12333 2024-05-16 23:27:10.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/control_flow_handlers.py
+-rw-rw-rw-   0        0        0    46277 2024-03-21 12:02:54.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/data_handlers.py
+-rw-rw-rw-   0        0        0    72995 2024-04-08 16:56:40.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/database_handlers.py
+-rw-rw-rw-   0        0        0    30031 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/datetime_handlers.py
+-rw-rw-rw-   0        0        0    14696 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/file_managment_handlers.py
+-rw-rw-rw-   0        0        0    83412 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/integration_handlers.py
+-rw-rw-rw-   0        0        0    27439 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/mapping_handlers.py
+-rw-rw-rw-   0        0        0    14152 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/model_handlers.py
+-rw-rw-rw-   0        0        0     2778 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/orchestration_handlers.py
+-rw-rw-rw-   0        0        0    16250 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/rpa_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:10:02.282825 forloop_modules-1.1.6/forloop_modules/function_handlers/transformations/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/transformations/__init__.py
+-rw-rw-rw-   0        0        0    14097 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/transformations/basic_transforms.py
+-rw-rw-rw-   0        0        0    10448 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/transformations/imputation.py
+-rw-rw-rw-   0        0        0     4092 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/transformations/outliers.py
+-rw-rw-rw-   0        0        0    59084 2024-05-24 13:02:30.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/variable_handlers.py
+-rw-rw-rw-   0        0        0   103428 2024-05-24 13:02:30.000000 forloop_modules-1.1.6/forloop_modules/function_handlers/webscraping_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:10:02.291024 forloop_modules-1.1.6/forloop_modules/globals/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/globals/__init__.py
+-rw-rw-rw-   0        0        0     5162 2024-05-03 13:07:28.000000 forloop_modules-1.1.6/forloop_modules/globals/active_entity_tracker.py
+-rw-rw-rw-   0        0        0     1871 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/globals/database_utilities_handler.py
+-rw-rw-rw-   0        0        0     8917 2024-05-21 18:30:50.000000 forloop_modules-1.1.6/forloop_modules/globals/db_connection.py
+-rw-rw-rw-   0        0        0     8030 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/globals/dbtables_loader_popups.py
+-rw-rw-rw-   0        0        0      223 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/globals/docs_categories.py
+-rw-rw-rw-   0        0        0    18806 2024-05-16 23:27:10.000000 forloop_modules-1.1.6/forloop_modules/globals/local_variable_handler.py
+-rw-rw-rw-   0        0        0    33426 2024-05-24 13:02:30.000000 forloop_modules-1.1.6/forloop_modules/globals/scraping_utilities_handler.py
+-rw-rw-rw-   0        0        0     9133 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/globals/variable_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:10:02.293271 forloop_modules-1.1.6/forloop_modules/integrations/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/integrations/__init__.py
+-rw-rw-rw-   0        0        0     2082 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/integrations/slack_integration.py
+-rw-rw-rw-   0        0        0     3580 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/integrations/testing_check_slack_notifications.py
+-rw-rw-rw-   0        0        0    14244 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/node_detail_form.py
+-rw-rw-rw-   0        0        0    10856 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/pipeline_function_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:10:02.296369 forloop_modules-1.1.6/forloop_modules/queries/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/queries/__init__.py
+-rw-rw-rw-   0        0        0     2888 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/queries/context_request_backend_auxiliary_functions.py
+-rw-rw-rw-   0        0        0    21803 2024-05-16 23:27:10.000000 forloop_modules-1.1.6/forloop_modules/queries/db_model_templates.py
+-rw-rw-rw-   0        0        0    42315 2024-05-21 18:30:50.000000 forloop_modules-1.1.6/forloop_modules/queries/node_context_requests_backend.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:10:02.297374 forloop_modules-1.1.6/forloop_modules/redis/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/redis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:10:02.299374 forloop_modules-1.1.6/forloop_modules/redis/config/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/redis/config/__init__.py
+-rw-rw-rw-   0        0        0     2063 2024-05-17 06:48:31.000000 forloop_modules-1.1.6/forloop_modules/redis/config/config.py
+-rw-rw-rw-   0        0        0     6573 2024-05-16 23:27:10.000000 forloop_modules-1.1.6/forloop_modules/redis/redis_connection.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:10:02.307300 forloop_modules-1.1.6/forloop_modules/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/utils/__init__.py
+-rw-rw-rw-   0        0        0     5587 2024-04-08 16:56:40.000000 forloop_modules-1.1.6/forloop_modules/utils/definitions.py
+-rw-rw-rw-   0        0        0     1024 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/utils/encryption.py
+-rw-rw-rw-   0        0        0     3393 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/utils/pandas_operations.py
+-rw-rw-rw-   0        0        0     3545 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/utils/pickle_serializer.py
+-rw-rw-rw-   0        0        0     3190 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/utils/script_utils.py
+-rw-rw-rw-   0        0        0     2021 2024-05-03 13:07:28.000000 forloop_modules-1.1.6/forloop_modules/utils/sse_parser.py
+-rw-rw-rw-   0        0        0     1622 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/utils/str_helpers.py
+-rw-rw-rw-   0        0        0      856 2024-04-08 16:56:40.000000 forloop_modules-1.1.6/forloop_modules/utils/synchronization_flags.py
+-rw-rw-rw-   0        0        0     4570 2024-04-08 16:56:40.000000 forloop_modules-1.1.6/forloop_modules/utils/url_template_builder.py
+-rw-rw-rw-   0        0        0     3558 2024-02-29 13:17:45.000000 forloop_modules-1.1.6/forloop_modules/utils/various.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:10:02.254629 forloop_modules-1.1.6/forloop_modules.egg-info/
+-rw-rw-rw-   0        0        0      658 2024-05-27 18:10:02.000000 forloop_modules-1.1.6/forloop_modules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3529 2024-05-27 18:10:02.000000 forloop_modules-1.1.6/forloop_modules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 18:10:02.000000 forloop_modules-1.1.6/forloop_modules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-27 18:10:02.000000 forloop_modules-1.1.6/forloop_modules.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 18:10:02.309815 forloop_modules-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      786 2024-05-27 18:10:00.000000 forloop_modules-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:10:02.308815 forloop_modules-1.1.6/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-22 17:34:45.000000 forloop_modules-1.1.6/tests/__init__.py
+-rw-rw-rw-   0        0        0     3316 2024-04-08 16:56:40.000000 forloop_modules-1.1.6/tests/test_url_template_builder.py
```

### Comparing `forloop_modules-1.1.5/LICENSE` & `forloop_modules-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/PKG-INFO` & `forloop_modules-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forloop_modules
-Version: 1.1.5
+Version: 1.1.6
 Summary: This package contains open source modules and integrations within Forloop.ai platform
 Home-page: https://github.com/ForloopAI/forloop_modules
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `forloop_modules-1.1.5/forloop_modules/errors/errors.py` & `forloop_modules-1.1.6/forloop_modules/errors/errors.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/flog.py` & `forloop_modules-1.1.6/forloop_modules/flog.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/api_endpoint_handlers.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/api_endpoint_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/api_handlers.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/api_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/auxilliary/abstract_function_handler.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/auxilliary/abstract_function_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/auxilliary/auxiliary_functions.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/auxilliary/auxiliary_functions.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/auxilliary/data_types_validation.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/auxilliary/data_types_validation.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/auxilliary/docs.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/auxilliary/docs.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/auxilliary/forloop_code_eval.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/auxilliary/forloop_code_eval.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/auxilliary/form_dict_list.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/auxilliary/form_dict_list.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/auxilliary/node_type_categories_manager.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/auxilliary/node_type_categories_manager.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/browser_handlers.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/browser_handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -205,14 +205,36 @@
             matching_elements = []
             matching_elements_groups = {}
             suh.matching_elements_groups = matching_elements_groups
             # message = "Selected elements XPATHs " + str(
             #     selected_elements_xpaths_new
             # ) + ", Error occured in finding matching elements"
 
+        ##### FIND SIMILAR ITEMS X,Y POSITION ALGORITHMIC CORRECTION #####
+        print("MATCHING GROUPS", matching_elements_groups)
+        
+        for k,v in matching_elements_groups.items():
+            print("K,V", k,v)
+            print(v[0])
+            x_positions=[x["rect"]["x"] for x in v]
+            y_positions=[x["rect"]["y"] for x in v]
+            print("X POSITIONS", x_positions)
+            print("Y POSITIONS", y_positions)
+            print("ELEMENT_GROUP_LEN",len(v))
+            
+            x_positions_differences=[x_positions[i+1]-x_positions[i] for i,item in enumerate(x_positions) if i+1<len(x_positions)]
+            y_positions_differences=[y_positions[i+1]-y_positions[i] for i,item in enumerate(y_positions) if i+1<len(y_positions)]
+            print("X POSITIONS_DIFF", x_positions_differences)
+            print("Y POSITIONS_DIFF", y_positions_differences)
+            
+            most_common_rounded_shift_in_x=[round(x/10)*10 for x in x_positions_differences]
+            most_common_rounded_shift_in_y=[round(y/10)*10 for y in y_positions_differences]
+            ##### TODO: Finish this!
+        
+        
         data = {
             # "message": message,
             # "ok": True,
             "elements_generalized_xpaths": elements_generalized_xpaths,
             "similar_items_xpaths": matching_elements,
             "similar_items_xpath_groups": matching_elements_groups,
         }
@@ -405,15 +427,15 @@
 
         # request_thread=slack_notif.UnblockingFunctionThread(slack_notif.send_slack_notification, api_scan_webpage.url, user_email=api_scan_webpage.email)
         # request_thread.start()
 
         #slack_notif.send_slack_notification(api_scan_webpage.url,user_email=api_scan_webpage.email)  #2 seconds
         # e_time = time.perf_counter() - start_time #12.5s
 
-        suh.webscraping_client.load_website(url, timeout=30)
+        suh.webscraping_client.load_website(url, timeout=50)
         elements, screenshot_base64 = suh.scan_web_page_API(output_folder, scraping_options)  #9 seconds
 
         # # Convert PNG file to WEBP
         # img = Image.open(output_folder / "website.png")
         # img.save(output_folder / "website.webp", quality=85)
         # (output_folder / "website.png").unlink()
         # with open(output_folder / "website.webp", "rb") as file:
```

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/cleaning_handlers.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/cleaning_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/control_flow_handlers.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/control_flow_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/data_handlers.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/data_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/database_handlers.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/database_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/datetime_handlers.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/datetime_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/file_managment_handlers.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/file_managment_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/integration_handlers.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/integration_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/mapping_handlers.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/mapping_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/model_handlers.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/model_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/orchestration_handlers.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/orchestration_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/rpa_handlers.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/rpa_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/transformations/basic_transforms.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/transformations/basic_transforms.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/transformations/imputation.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/transformations/imputation.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/transformations/outliers.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/transformations/outliers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/variable_handlers.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/variable_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/function_handlers/webscraping_handlers.py` & `forloop_modules-1.1.6/forloop_modules/function_handlers/webscraping_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/globals/active_entity_tracker.py` & `forloop_modules-1.1.6/forloop_modules/globals/active_entity_tracker.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/globals/database_utilities_handler.py` & `forloop_modules-1.1.6/forloop_modules/globals/database_utilities_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/globals/db_connection.py` & `forloop_modules-1.1.6/forloop_modules/globals/db_connection.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/globals/dbtables_loader_popups.py` & `forloop_modules-1.1.6/forloop_modules/globals/dbtables_loader_popups.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/globals/local_variable_handler.py` & `forloop_modules-1.1.6/forloop_modules/globals/local_variable_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/globals/scraping_utilities_handler.py` & `forloop_modules-1.1.6/forloop_modules/globals/scraping_utilities_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/globals/variable_handler.py` & `forloop_modules-1.1.6/forloop_modules/globals/variable_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/integrations/slack_integration.py` & `forloop_modules-1.1.6/forloop_modules/integrations/slack_integration.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/integrations/testing_check_slack_notifications.py` & `forloop_modules-1.1.6/forloop_modules/integrations/testing_check_slack_notifications.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/node_detail_form.py` & `forloop_modules-1.1.6/forloop_modules/node_detail_form.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/pipeline_function_handlers.py` & `forloop_modules-1.1.6/forloop_modules/pipeline_function_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/queries/context_request_backend_auxiliary_functions.py` & `forloop_modules-1.1.6/forloop_modules/queries/context_request_backend_auxiliary_functions.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/queries/db_model_templates.py` & `forloop_modules-1.1.6/forloop_modules/queries/db_model_templates.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/queries/node_context_requests_backend.py` & `forloop_modules-1.1.6/forloop_modules/queries/node_context_requests_backend.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/redis/config/config.py` & `forloop_modules-1.1.6/forloop_modules/redis/config/config.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/redis/redis_connection.py` & `forloop_modules-1.1.6/forloop_modules/redis/redis_connection.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/utils/definitions.py` & `forloop_modules-1.1.6/forloop_modules/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/utils/encryption.py` & `forloop_modules-1.1.6/forloop_modules/utils/encryption.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/utils/pandas_operations.py` & `forloop_modules-1.1.6/forloop_modules/utils/pandas_operations.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/utils/pickle_serializer.py` & `forloop_modules-1.1.6/forloop_modules/utils/pickle_serializer.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/utils/script_utils.py` & `forloop_modules-1.1.6/forloop_modules/utils/script_utils.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/utils/sse_parser.py` & `forloop_modules-1.1.6/forloop_modules/utils/sse_parser.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/utils/str_helpers.py` & `forloop_modules-1.1.6/forloop_modules/utils/str_helpers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/utils/synchronization_flags.py` & `forloop_modules-1.1.6/forloop_modules/utils/synchronization_flags.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/utils/url_template_builder.py` & `forloop_modules-1.1.6/forloop_modules/utils/url_template_builder.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules/utils/various.py` & `forloop_modules-1.1.6/forloop_modules/utils/various.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/forloop_modules.egg-info/PKG-INFO` & `forloop_modules-1.1.6/forloop_modules.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forloop-modules
-Version: 1.1.5
+Version: 1.1.6
 Summary: This package contains open source modules and integrations within Forloop.ai platform
 Home-page: https://github.com/ForloopAI/forloop_modules
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `forloop_modules-1.1.5/forloop_modules.egg-info/SOURCES.txt` & `forloop_modules-1.1.6/forloop_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.5/setup.py` & `forloop_modules-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='forloop_modules',
-    version='1.1.5',
+    version='1.1.6',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='This package contains open source modules and integrations within Forloop.ai platform',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/ForloopAI/forloop_modules',
     packages=setuptools.find_packages(),
```

### Comparing `forloop_modules-1.1.5/tests/test_url_template_builder.py` & `forloop_modules-1.1.6/tests/test_url_template_builder.py`

 * *Files identical despite different names*

