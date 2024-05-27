# Comparing `tmp/foundationallm-0.7.6.tar.gz` & `tmp/foundationallm-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundationallm-0.7.6.tar", last modified: Mon May 27 10:08:46 2024, max compression
+gzip compressed data, was "foundationallm-0.7.7.tar", last modified: Mon May 27 11:09:33 2024, max compression
```

## Comparing `foundationallm-0.7.6.tar` & `foundationallm-0.7.7.tar`

### file list

```diff
@@ -1,39 +1,132 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 10:08:46.986018 foundationallm-0.7.6/
--rw-rw-rw-   0        0        0      201 2024-05-07 13:15:07.000000 foundationallm-0.7.6/LICENSE
--rw-rw-rw-   0        0        0      892 2024-05-27 10:08:46.985017 foundationallm-0.7.6/PKG-INFO
--rw-rw-rw-   0        0        0      347 2024-05-23 14:45:46.000000 foundationallm-0.7.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 10:08:46.926317 foundationallm-0.7.6/foundationallm/
-drwxrwxrwx   0        0        0        0 2024-05-27 10:08:46.947341 foundationallm-0.7.6/foundationallm/config/
--rw-rw-rw-   0        0        0      177 2023-12-14 16:50:30.000000 foundationallm-0.7.6/foundationallm/config/__init__.py
--rw-rw-rw-   0        0        0     4874 2024-05-23 11:10:06.000000 foundationallm-0.7.6/foundationallm/config/configuration.py
--rw-rw-rw-   0        0        0      605 2023-12-14 16:50:30.000000 foundationallm-0.7.6/foundationallm/config/context.py
--rw-rw-rw-   0        0        0      378 2024-03-15 16:01:06.000000 foundationallm-0.7.6/foundationallm/config/environment_variables.py
--rw-rw-rw-   0        0        0      556 2023-12-14 16:50:30.000000 foundationallm-0.7.6/foundationallm/config/user_identity.py
-drwxrwxrwx   0        0        0        0 2024-05-27 10:08:46.927318 foundationallm-0.7.6/foundationallm/models/
-drwxrwxrwx   0        0        0        0 2024-05-27 10:08:46.968997 foundationallm-0.7.6/foundationallm/models/agents/
--rw-rw-rw-   0        0        0      409 2024-05-23 14:45:46.000000 foundationallm-0.7.6/foundationallm/models/agents/__init__.py
--rw-rw-rw-   0        0        0      815 2024-05-07 13:15:07.000000 foundationallm-0.7.6/foundationallm/models/agents/agent_base.py
--rw-rw-rw-   0        0        0      316 2024-04-24 17:34:13.000000 foundationallm-0.7.6/foundationallm/models/agents/agent_conversation_history_settings.py
--rw-rw-rw-   0        0        0      274 2024-04-24 17:34:13.000000 foundationallm-0.7.6/foundationallm/models/agents/agent_gatekeeper_settings.py
--rw-rw-rw-   0        0        0      594 2024-05-07 13:15:07.000000 foundationallm-0.7.6/foundationallm/models/agents/agent_vectorization_settings.py
--rw-rw-rw-   0        0        0      361 2024-04-24 17:34:13.000000 foundationallm-0.7.6/foundationallm/models/agents/knowledge_management_agent.py
--rw-rw-rw-   0        0        0      518 2024-05-07 13:15:07.000000 foundationallm-0.7.6/foundationallm/models/agents/knowledge_management_completion_request.py
-drwxrwxrwx   0        0        0        0 2024-05-27 10:08:46.971500 foundationallm-0.7.6/foundationallm/models/authentication/
--rw-rw-rw-   0        0        0       55 2024-05-07 13:15:07.000000 foundationallm-0.7.6/foundationallm/models/authentication/__init__.py
--rw-rw-rw-   0        0        0      157 2024-05-07 13:15:07.000000 foundationallm-0.7.6/foundationallm/models/authentication/authentication_types.py
-drwxrwxrwx   0        0        0        0 2024-05-27 10:08:46.982013 foundationallm-0.7.6/foundationallm/models/orchestration/
--rw-rw-rw-   0        0        0      402 2024-05-23 14:45:46.000000 foundationallm-0.7.6/foundationallm/models/orchestration/__init__.py
--rw-rw-rw-   0        0        0      272 2024-04-24 17:34:13.000000 foundationallm-0.7.6/foundationallm/models/orchestration/citation.py
--rw-rw-rw-   0        0        0      502 2024-05-07 13:15:07.000000 foundationallm-0.7.6/foundationallm/models/orchestration/completion_request_base.py
--rw-rw-rw-   0        0        0      523 2024-04-24 17:34:13.000000 foundationallm-0.7.6/foundationallm/models/orchestration/completion_response.py
--rw-rw-rw-   0        0        0      469 2024-05-23 14:45:46.000000 foundationallm-0.7.6/foundationallm/models/orchestration/endpoint_settings.py
--rw-rw-rw-   0        0        0      370 2023-12-14 16:50:30.000000 foundationallm-0.7.6/foundationallm/models/orchestration/message_history_item.py
--rw-rw-rw-   0        0        0      154 2024-05-23 14:45:46.000000 foundationallm-0.7.6/foundationallm/models/orchestration/operation_types.py
--rw-rw-rw-   0        0        0      939 2024-05-07 13:15:07.000000 foundationallm-0.7.6/foundationallm/models/orchestration/orchestration_settings.py
-drwxrwxrwx   0        0        0        0 2024-05-27 10:08:46.984019 foundationallm-0.7.6/foundationallm.egg-info/
--rw-rw-rw-   0        0        0      892 2024-05-27 10:08:46.000000 foundationallm-0.7.6/foundationallm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1340 2024-05-27 10:08:46.000000 foundationallm-0.7.6/foundationallm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 10:08:46.000000 foundationallm-0.7.6/foundationallm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-27 10:08:46.000000 foundationallm-0.7.6/foundationallm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      651 2024-05-27 10:06:29.000000 foundationallm-0.7.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-27 10:08:46.987018 foundationallm-0.7.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:33.590997 foundationallm-0.7.7/
+-rw-rw-rw-   0        0        0      201 2024-05-07 13:15:07.000000 foundationallm-0.7.7/LICENSE
+-rw-rw-rw-   0        0        0      892 2024-05-27 11:09:33.589999 foundationallm-0.7.7/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-05-23 14:45:46.000000 foundationallm-0.7.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:32.848576 foundationallm-0.7.7/foundationallm/
+-rw-rw-rw-   0        0        0       71 2023-12-14 16:50:30.000000 foundationallm-0.7.7/foundationallm/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-12-14 16:50:30.000000 foundationallm-0.7.7/foundationallm/_version.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:32.903598 foundationallm-0.7.7/foundationallm/config/
+-rw-rw-rw-   0        0        0      177 2023-12-14 16:50:30.000000 foundationallm-0.7.7/foundationallm/config/__init__.py
+-rw-rw-rw-   0        0        0     4874 2024-05-23 11:10:06.000000 foundationallm-0.7.7/foundationallm/config/configuration.py
+-rw-rw-rw-   0        0        0      605 2023-12-14 16:50:30.000000 foundationallm-0.7.7/foundationallm/config/context.py
+-rw-rw-rw-   0        0        0      378 2024-03-15 16:01:06.000000 foundationallm-0.7.7/foundationallm/config/environment_variables.py
+-rw-rw-rw-   0        0        0      556 2023-12-14 16:50:30.000000 foundationallm-0.7.7/foundationallm/config/user_identity.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:32.911598 foundationallm-0.7.7/foundationallm/langchain/
+-rw-rw-rw-   0        0        0       39 2023-10-19 14:24:41.000000 foundationallm-0.7.7/foundationallm/langchain/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:32.951597 foundationallm-0.7.7/foundationallm/langchain/agents/
+-rw-rw-rw-   0        0        0      211 2024-05-07 13:15:07.000000 foundationallm-0.7.7/foundationallm/langchain/agents/__init__.py
+-rw-rw-rw-   0        0        0     1903 2024-05-07 13:15:07.000000 foundationallm-0.7.7/foundationallm/langchain/agents/agent_factory.py
+-rw-rw-rw-   0        0        0    16960 2024-05-23 14:45:46.000000 foundationallm-0.7.7/foundationallm/langchain/agents/langchain_agent_base.py
+-rw-rw-rw-   0        0        0     5475 2024-05-08 09:51:28.000000 foundationallm-0.7.7/foundationallm/langchain/agents/langchain_knowledge_management_agent.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:32.966628 foundationallm-0.7.7/foundationallm/langchain/data_sources/
+-rw-rw-rw-   0        0        0       64 2023-12-14 16:50:30.000000 foundationallm-0.7.7/foundationallm/langchain/data_sources/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:32.982278 foundationallm-0.7.7/foundationallm/langchain/data_sources/blob/
+-rw-rw-rw-   0        0        0       66 2023-12-14 16:50:30.000000 foundationallm-0.7.7/foundationallm/langchain/data_sources/blob/__init__.py
+-rw-rw-rw-   0        0        0      485 2024-01-24 21:43:50.000000 foundationallm-0.7.7/foundationallm/langchain/data_sources/blob/blob_storage_configuration.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:32.997840 foundationallm-0.7.7/foundationallm/langchain/data_sources/cxo/
+-rw-rw-rw-   0        0        0       49 2024-01-24 21:43:50.000000 foundationallm-0.7.7/foundationallm/langchain/data_sources/cxo/__init__.py
+-rw-rw-rw-   0        0        0      421 2024-01-24 21:43:50.000000 foundationallm-0.7.7/foundationallm/langchain/data_sources/cxo/cxo_configuration.py
+-rw-rw-rw-   0        0        0      125 2023-12-14 16:50:30.000000 foundationallm-0.7.7/foundationallm/langchain/data_sources/data_source_configuration.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:33.016530 foundationallm-0.7.7/foundationallm/langchain/data_sources/search_service/
+-rw-rw-rw-   0        0        0      103 2024-01-09 18:22:07.000000 foundationallm-0.7.7/foundationallm/langchain/data_sources/search_service/__init__.py
+-rw-rw-rw-   0        0        0      655 2024-01-24 21:43:50.000000 foundationallm-0.7.7/foundationallm/langchain/data_sources/search_service/search_service_configuration.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:33.091802 foundationallm-0.7.7/foundationallm/langchain/data_sources/sql/
+-rw-rw-rw-   0        0        0      351 2023-12-14 16:50:30.000000 foundationallm-0.7.7/foundationallm/langchain/data_sources/sql/__init__.py
+-rw-rw-rw-   0        0        0     1162 2023-12-14 16:50:30.000000 foundationallm-0.7.7/foundationallm/langchain/data_sources/sql/mariadb.py
+-rw-rw-rw-   0        0        0     1304 2023-12-14 16:50:30.000000 foundationallm-0.7.7/foundationallm/langchain/data_sources/sql/mssql.py
+-rw-rw-rw-   0        0        0     1158 2023-12-14 16:50:30.000000 foundationallm-0.7.7/foundationallm/langchain/data_sources/sql/mysql.py
+-rw-rw-rw-   0        0        0     1153 2023-12-14 16:50:30.000000 foundationallm-0.7.7/foundationallm/langchain/data_sources/sql/postgresql.py
+-rw-rw-rw-   0        0        0      632 2024-01-24 21:43:50.000000 foundationallm-0.7.7/foundationallm/langchain/data_sources/sql/sql_database_configuration.py
+-rw-rw-rw-   0        0        0     2516 2024-01-29 10:28:21.000000 foundationallm-0.7.7/foundationallm/langchain/data_sources/sql/sql_database_datasource.py
+-rw-rw-rw-   0        0        0      208 2024-04-24 17:34:13.000000 foundationallm-0.7.7/foundationallm/langchain/data_sources/sql/sql_database_dialects.py
+-rw-rw-rw-   0        0        0     1919 2024-04-24 17:34:13.000000 foundationallm-0.7.7/foundationallm/langchain/data_sources/sql/sql_database_factory.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:33.106133 foundationallm-0.7.7/foundationallm/langchain/exceptions/
+-rw-rw-rw-   0        0        0       53 2024-05-07 13:15:07.000000 foundationallm-0.7.7/foundationallm/langchain/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      195 2024-05-07 13:15:07.000000 foundationallm-0.7.7/foundationallm/langchain/exceptions/langchain_exception.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:33.130052 foundationallm-0.7.7/foundationallm/langchain/language_models/
+-rw-rw-rw-   0        0        0      139 2023-12-14 16:50:30.000000 foundationallm-0.7.7/foundationallm/langchain/language_models/__init__.py
+-rw-rw-rw-   0        0        0      943 2024-04-24 17:34:13.000000 foundationallm-0.7.7/foundationallm/langchain/language_models/language_model_base.py
+-rw-rw-rw-   0        0        0      856 2024-04-24 17:34:13.000000 foundationallm-0.7.7/foundationallm/langchain/language_models/language_model_factory.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:33.148420 foundationallm-0.7.7/foundationallm/langchain/language_models/openai/
+-rw-rw-rw-   0        0        0       75 2023-12-14 16:50:30.000000 foundationallm-0.7.7/foundationallm/langchain/language_models/openai/__init__.py
+-rw-rw-rw-   0        0        0     4760 2024-04-24 17:34:13.000000 foundationallm-0.7.7/foundationallm/langchain/language_models/openai/openai_model.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:33.165968 foundationallm-0.7.7/foundationallm/langchain/orchestration/
+-rw-rw-rw-   0        0        0       57 2023-12-14 16:50:30.000000 foundationallm-0.7.7/foundationallm/langchain/orchestration/__init__.py
+-rw-rw-rw-   0        0        0     2242 2024-05-07 13:15:07.000000 foundationallm-0.7.7/foundationallm/langchain/orchestration/orchestration_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:33.215679 foundationallm-0.7.7/foundationallm/langchain/retrievers/
+-rw-rw-rw-   0        0        0      262 2024-04-24 17:34:13.000000 foundationallm-0.7.7/foundationallm/langchain/retrievers/__init__.py
+-rw-rw-rw-   0        0        0      265 2024-03-15 16:01:06.000000 foundationallm-0.7.7/foundationallm/langchain/retrievers/agent_parameter_retriever_keys.py
+-rw-rw-rw-   0        0        0     6011 2024-05-07 13:15:07.000000 foundationallm-0.7.7/foundationallm/langchain/retrievers/azure_ai_search_service_retriever.py
+-rw-rw-rw-   0        0        0      522 2024-04-24 17:34:13.000000 foundationallm-0.7.7/foundationallm/langchain/retrievers/citation_retrieval_base.py
+-rw-rw-rw-   0        0        0     4779 2024-05-07 13:15:07.000000 foundationallm-0.7.7/foundationallm/langchain/retrievers/retriever_factory.py
+-rw-rw-rw-   0        0        0     4738 2024-01-29 10:28:21.000000 foundationallm-0.7.7/foundationallm/langchain/retrievers/search_service_filter_retriever.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:33.241677 foundationallm-0.7.7/foundationallm/langchain/toolkits/
+-rw-rw-rw-   0        0        0      131 2023-12-14 16:50:30.000000 foundationallm-0.7.7/foundationallm/langchain/toolkits/__init__.py
+-rw-rw-rw-   0        0        0     1777 2024-01-29 10:28:21.000000 foundationallm-0.7.7/foundationallm/langchain/toolkits/anomaly_detection_toolkit.py
+-rw-rw-rw-   0        0        0     3245 2024-01-29 10:28:21.000000 foundationallm-0.7.7/foundationallm/langchain/toolkits/secure_sql_database_toolkit.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:33.267220 foundationallm-0.7.7/foundationallm/langchain/tools/
+-rw-rw-rw-   0        0        0      200 2023-12-14 16:50:30.000000 foundationallm-0.7.7/foundationallm/langchain/tools/__init__.py
+-rw-rw-rw-   0        0        0     2450 2024-01-29 10:28:21.000000 foundationallm-0.7.7/foundationallm/langchain/tools/query_pandas_dataframe_tool.py
+-rw-rw-rw-   0        0        0     1656 2024-01-29 10:28:21.000000 foundationallm-0.7.7/foundationallm/langchain/tools/secure_sql_database_query_tool.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:33.283224 foundationallm-0.7.7/foundationallm/models/
+-rw-rw-rw-   0        0        0       73 2024-03-15 16:01:06.000000 foundationallm-0.7.7/foundationallm/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:33.339734 foundationallm-0.7.7/foundationallm/models/agents/
+-rw-rw-rw-   0        0        0      409 2024-05-23 14:45:46.000000 foundationallm-0.7.7/foundationallm/models/agents/__init__.py
+-rw-rw-rw-   0        0        0      815 2024-05-07 13:15:07.000000 foundationallm-0.7.7/foundationallm/models/agents/agent_base.py
+-rw-rw-rw-   0        0        0      316 2024-04-24 17:34:13.000000 foundationallm-0.7.7/foundationallm/models/agents/agent_conversation_history_settings.py
+-rw-rw-rw-   0        0        0      274 2024-04-24 17:34:13.000000 foundationallm-0.7.7/foundationallm/models/agents/agent_gatekeeper_settings.py
+-rw-rw-rw-   0        0        0      594 2024-05-07 13:15:07.000000 foundationallm-0.7.7/foundationallm/models/agents/agent_vectorization_settings.py
+-rw-rw-rw-   0        0        0      361 2024-04-24 17:34:13.000000 foundationallm-0.7.7/foundationallm/models/agents/knowledge_management_agent.py
+-rw-rw-rw-   0        0        0      518 2024-05-07 13:15:07.000000 foundationallm-0.7.7/foundationallm/models/agents/knowledge_management_completion_request.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:33.354733 foundationallm-0.7.7/foundationallm/models/authentication/
+-rw-rw-rw-   0        0        0       55 2024-05-07 13:15:07.000000 foundationallm-0.7.7/foundationallm/models/authentication/__init__.py
+-rw-rw-rw-   0        0        0      157 2024-05-07 13:15:07.000000 foundationallm-0.7.7/foundationallm/models/authentication/authentication_types.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:33.389247 foundationallm-0.7.7/foundationallm/models/language_models/
+-rw-rw-rw-   0        0        0      187 2024-04-24 17:34:13.000000 foundationallm-0.7.7/foundationallm/models/language_models/__init__.py
+-rw-rw-rw-   0        0        0      690 2024-03-11 14:31:54.000000 foundationallm-0.7.7/foundationallm/models/language_models/embedding_model.py
+-rw-rw-rw-   0        0        0      175 2023-12-14 16:50:30.000000 foundationallm-0.7.7/foundationallm/models/language_models/language_model_provider.py
+-rw-rw-rw-   0        0        0      138 2023-12-14 16:50:30.000000 foundationallm-0.7.7/foundationallm/models/language_models/language_model_type.py
+-rw-rw-rw-   0        0        0      101 2023-12-14 16:50:30.000000 foundationallm-0.7.7/foundationallm/models/list_option.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:33.451246 foundationallm-0.7.7/foundationallm/models/orchestration/
+-rw-rw-rw-   0        0        0      402 2024-05-23 14:45:46.000000 foundationallm-0.7.7/foundationallm/models/orchestration/__init__.py
+-rw-rw-rw-   0        0        0      272 2024-04-24 17:34:13.000000 foundationallm-0.7.7/foundationallm/models/orchestration/citation.py
+-rw-rw-rw-   0        0        0      502 2024-05-07 13:15:07.000000 foundationallm-0.7.7/foundationallm/models/orchestration/completion_request_base.py
+-rw-rw-rw-   0        0        0      523 2024-04-24 17:34:13.000000 foundationallm-0.7.7/foundationallm/models/orchestration/completion_response.py
+-rw-rw-rw-   0        0        0      469 2024-05-23 14:45:46.000000 foundationallm-0.7.7/foundationallm/models/orchestration/endpoint_settings.py
+-rw-rw-rw-   0        0        0      370 2023-12-14 16:50:30.000000 foundationallm-0.7.7/foundationallm/models/orchestration/message_history_item.py
+-rw-rw-rw-   0        0        0      154 2024-05-23 14:45:46.000000 foundationallm-0.7.7/foundationallm/models/orchestration/operation_types.py
+-rw-rw-rw-   0        0        0      939 2024-05-07 13:15:07.000000 foundationallm-0.7.7/foundationallm/models/orchestration/orchestration_settings.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:32.818955 foundationallm-0.7.7/foundationallm/models/resource_providers/
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:33.465246 foundationallm-0.7.7/foundationallm/models/resource_providers/prompts/
+-rw-rw-rw-   0        0        0       98 2024-05-07 13:15:07.000000 foundationallm-0.7.7/foundationallm/models/resource_providers/prompts/__init__.py
+-rw-rw-rw-   0        0        0      422 2024-05-07 13:15:07.000000 foundationallm-0.7.7/foundationallm/models/resource_providers/prompts/multipart_prompt.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:33.494913 foundationallm-0.7.7/foundationallm/models/resource_providers/vectorization/
+-rw-rw-rw-   0        0        0      862 2024-03-11 14:31:54.000000 foundationallm-0.7.7/foundationallm/models/resource_providers/vectorization/__init__.py
+-rw-rw-rw-   0        0        0      320 2024-03-11 14:31:54.000000 foundationallm-0.7.7/foundationallm/models/resource_providers/vectorization/configuration_references_base.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:33.502910 foundationallm-0.7.7/foundationallm/models/resource_providers/vectorization/embedding_profiles/
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:33.518911 foundationallm-0.7.7/foundationallm/models/resource_providers/vectorization/embedding_profiles/azure_openai/
+-rw-rw-rw-   0        0        0      998 2024-03-11 14:31:54.000000 foundationallm-0.7.7/foundationallm/models/resource_providers/vectorization/embedding_profiles/azure_openai/azure_openai_configuration_references.py
+-rw-rw-rw-   0        0        0      613 2024-03-11 14:31:54.000000 foundationallm-0.7.7/foundationallm/models/resource_providers/vectorization/embedding_profiles/azure_openai/azure_openai_embedding_profile.py
+-rw-rw-rw-   0        0        0      324 2024-03-11 14:31:54.000000 foundationallm-0.7.7/foundationallm/models/resource_providers/vectorization/embedding_profiles/embedding_profile_base.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:33.525909 foundationallm-0.7.7/foundationallm/models/resource_providers/vectorization/indexing_profiles/
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:33.546910 foundationallm-0.7.7/foundationallm/models/resource_providers/vectorization/indexing_profiles/azure_ai_search/
+-rw-rw-rw-   0        0        0      653 2024-04-03 14:03:09.000000 foundationallm-0.7.7/foundationallm/models/resource_providers/vectorization/indexing_profiles/azure_ai_search/azure_ai_search_configuration_references.py
+-rw-rw-rw-   0        0        0      813 2024-03-11 14:31:54.000000 foundationallm-0.7.7/foundationallm/models/resource_providers/vectorization/indexing_profiles/azure_ai_search/azure_ai_search_indexing_profile.py
+-rw-rw-rw-   0        0        0      649 2024-04-24 17:34:13.000000 foundationallm-0.7.7/foundationallm/models/resource_providers/vectorization/indexing_profiles/azure_ai_search/azure_ai_search_settings.py
+-rw-rw-rw-   0        0        0      310 2024-03-11 14:31:54.000000 foundationallm-0.7.7/foundationallm/models/resource_providers/vectorization/indexing_profiles/indexing_profile_base.py
+-rw-rw-rw-   0        0        0      754 2024-03-11 14:31:54.000000 foundationallm-0.7.7/foundationallm/models/resource_providers/vectorization/profile_base.py
+-rw-rw-rw-   0        0        0      229 2024-03-11 14:31:54.000000 foundationallm-0.7.7/foundationallm/models/resource_providers/vectorization/settings_base.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:33.570910 foundationallm-0.7.7/foundationallm/storage/
+-rw-rw-rw-   0        0        0      108 2023-12-14 16:50:30.000000 foundationallm-0.7.7/foundationallm/storage/__init__.py
+-rw-rw-rw-   0        0        0     6092 2024-04-30 12:19:06.000000 foundationallm-0.7.7/foundationallm/storage/blob_storage_manager.py
+-rw-rw-rw-   0        0        0     2063 2024-03-15 16:01:06.000000 foundationallm-0.7.7/foundationallm/storage/storage_manager_base.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:33.585914 foundationallm-0.7.7/foundationallm/telemetry/
+-rw-rw-rw-   0        0        0       34 2024-03-11 14:31:54.000000 foundationallm-0.7.7/foundationallm/telemetry/__init__.py
+-rw-rw-rw-   0        0        0     2558 2024-03-11 14:31:54.000000 foundationallm-0.7.7/foundationallm/telemetry/telemetry.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:09:33.588996 foundationallm-0.7.7/foundationallm.egg-info/
+-rw-rw-rw-   0        0        0      892 2024-05-27 11:09:32.000000 foundationallm-0.7.7/foundationallm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5717 2024-05-27 11:09:32.000000 foundationallm-0.7.7/foundationallm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 11:09:32.000000 foundationallm-0.7.7/foundationallm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-27 11:09:32.000000 foundationallm-0.7.7/foundationallm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      583 2024-05-27 11:09:13.000000 foundationallm-0.7.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-27 11:09:33.590997 foundationallm-0.7.7/setup.cfg
```

### Comparing `foundationallm-0.7.6/PKG-INFO` & `foundationallm-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundationallm
-Version: 0.7.6
+Version: 0.7.7
 Summary: Enables integration with the FoundationaLLM platform.
 Author-email: FoundationaLLM <dev@foundationallm.ai>
 Project-URL: Homepage, https://foundationallm.ai
 Project-URL: Issues, https://github.com/solliancenet/foundationallm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `foundationallm-0.7.6/foundationallm/config/configuration.py` & `foundationallm-0.7.7/foundationallm/config/configuration.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.6/foundationallm/config/context.py` & `foundationallm-0.7.7/foundationallm/config/context.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.6/foundationallm/config/user_identity.py` & `foundationallm-0.7.7/foundationallm/config/user_identity.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.6/foundationallm/models/agents/agent_base.py` & `foundationallm-0.7.7/foundationallm/models/agents/agent_base.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.6/foundationallm/models/agents/agent_vectorization_settings.py` & `foundationallm-0.7.7/foundationallm/models/agents/agent_vectorization_settings.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.6/foundationallm/models/agents/knowledge_management_completion_request.py` & `foundationallm-0.7.7/foundationallm/models/agents/knowledge_management_completion_request.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.6/foundationallm/models/orchestration/completion_response.py` & `foundationallm-0.7.7/foundationallm/models/orchestration/completion_response.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.6/foundationallm/models/orchestration/orchestration_settings.py` & `foundationallm-0.7.7/foundationallm/models/orchestration/orchestration_settings.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.6/foundationallm.egg-info/PKG-INFO` & `foundationallm-0.7.7/foundationallm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundationallm
-Version: 0.7.6
+Version: 0.7.7
 Summary: Enables integration with the FoundationaLLM platform.
 Author-email: FoundationaLLM <dev@foundationallm.ai>
 Project-URL: Homepage, https://foundationallm.ai
 Project-URL: Issues, https://github.com/solliancenet/foundationallm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

