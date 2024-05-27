# Comparing `tmp/langflow_base-0.0.48.tar.gz` & `tmp/langflow_base-0.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langflow_base-0.0.48.tar", max compression
+gzip compressed data, was "langflow_base-0.0.49.tar", max compression
```

## Comparing `langflow_base-0.0.48.tar` & `langflow_base-0.0.49.tar`

### file list

```diff
@@ -1,1788 +1,1732 @@
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.320054 langflow_base-0.0.48/README.md
--rw-r--r--   0        0        0    18450 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/__main__.py
--rw-r--r--   0        0        0       38 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/README
--rw-r--r--   0        0        0     3111 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/env.py
--rw-r--r--   0        0        0      964 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/script.py.mako
--rw-r--r--   0        0        0     2826 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/versions/006b3990db50_add_unique_constraints.py
--rw-r--r--   0        0        0     3053 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/versions/012fb73ac359_add_folder_table.py
--rw-r--r--   0        0        0      648 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/versions/0b8757876a7c_.py
--rw-r--r--   0        0        0     2630 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/versions/1a110b568907_replace_credential_table_with_variable.py
--rw-r--r--   0        0        0     1101 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/versions/1ef9c4f3765d_.py
--rw-r--r--   0        0        0     1447 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/versions/1f4d6df60295_add_default_fields_column.py
--rw-r--r--   0        0        0     7221 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/versions/260dbcc8b680_adds_tables.py
--rw-r--r--   0        0        0     1439 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/versions/29fe8f1f806b_add_missing_index.py
--rw-r--r--   0        0        0     1774 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/versions/2ac71eb9c3ae_adds_credential_table.py
--rw-r--r--   0        0        0     6127 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/versions/4e5980a44eaa_fix_date_times_again.py
--rw-r--r--   0        0        0     2339 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/versions/58b28437a398_modify_nullable.py
--rw-r--r--   0        0        0     1802 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/versions/63b9c451fd30_add_icon_and_icon_bg_color_to_flow.py
--rw-r--r--   0        0        0     1809 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/versions/67cc006d50bf_add_profile_image_column.py
--rw-r--r--   0        0        0     2191 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/versions/6e7b581b5648_fix_nullable.py
--rw-r--r--   0        0        0     1811 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/versions/7843803a87b5_store_updates.py
--rw-r--r--   0        0        0     6127 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/versions/79e675cb6752_change_datetime_type.py
--rw-r--r--   0        0        0     2157 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/versions/7d2162acc8b2_adds_updated_at_and_folder_cols.py
--rw-r--r--   0        0        0     4281 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/versions/b2fa308044b5_add_unique_constraints.py
--rw-r--r--   0        0        0     2705 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/versions/bc2f01c40e4a_new_fixes.py
--rw-r--r--   0        0        0     2052 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/versions/c153816fd85f_set_name_and_value_to_not_nullable.py
--rw-r--r--   0        0        0     2551 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/versions/e3bc869fa272_fix_nullable.py
--rw-r--r--   0        0        0      726 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/versions/eb5866d51fd2_change_columns_to_be_nullable.py
--rw-r--r--   0        0        0     1149 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/versions/f5ee9749d1a6_user_id_can_be_null_in_flow.py
--rw-r--r--   0        0        0     2018 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic/versions/fd531f8868b1_fix_credential_table.py
--rw-r--r--   0        0        0     3497 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/alembic.ini
--rw-r--r--   0        0        0       61 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/api/__init__.py
--rw-r--r--   0        0        0      810 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/api/router.py
--rw-r--r--   0        0        0    11575 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/api/utils.py
--rw-r--r--   0        0        0      986 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/api/v1/__init__.py
--rw-r--r--   0        0        0     2988 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/api/v1/api_key.py
--rw-r--r--   0        0        0     5033 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/api/v1/base.py
--rw-r--r--   0        0        0     4772 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/api/v1/callback.py
--rw-r--r--   0        0        0    14132 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/api/v1/chat.py
--rw-r--r--   0        0        0    20162 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/api/v1/endpoints.py
--rw-r--r--   0        0        0     4991 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/api/v1/files.py
--rw-r--r--   0        0        0     8474 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/api/v1/flows.py
--rw-r--r--   0        0        0     8831 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/api/v1/folders.py
--rw-r--r--   0        0        0     5137 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/api/v1/login.py
--rw-r--r--   0        0        0     3007 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/api/v1/monitor.py
--rw-r--r--   0        0        0     8198 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/api/v1/schemas.py
--rw-r--r--   0        0        0     7347 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/api/v1/store.py
--rw-r--r--   0        0        0     5126 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/api/v1/users.py
--rw-r--r--   0        0        0     3257 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/api/v1/validate.py
--rw-r--r--   0        0        0     4399 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/api/v1/variable.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/base/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/base/agents/__init__.py
--rw-r--r--   0        0        0     2947 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/base/agents/agent.py
--rw-r--r--   0        0        0      941 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/base/agents/default_prompts.py
--rw-r--r--   0        0        0     3993 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/base/agents/utils.py
--rw-r--r--   0        0        0      768 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/base/constants.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.320054 langflow_base-0.0.48/langflow/base/data/__init__.py
--rw-r--r--   0        0        0     4922 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/base/data/utils.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/base/io/__init__.py
--rw-r--r--   0        0        0     5160 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/base/io/chat.py
--rw-r--r--   0        0        0     1573 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/base/io/text.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/base/memory/__init__.py
--rw-r--r--   0        0        0     1762 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/base/memory/memory.py
--rw-r--r--   0        0        0       68 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/base/models/__init__.py
--rw-r--r--   0        0        0       89 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/base/models/groq_constants.py
--rw-r--r--   0        0        0     4250 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/base/models/model.py
--rw-r--r--   0        0        0      102 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/base/models/openai_constants.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/base/prompts/__init__.py
--rw-r--r--   0        0        0     3278 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/base/prompts/api_utils.py
--rw-r--r--   0        0        0     1538 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/base/prompts/utils.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/base/tools/__init__.py
--rw-r--r--   0        0        0      751 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/base/tools/base.py
--rw-r--r--   0        0        0      275 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/__init__.py
--rw-r--r--   0        0        0     1860 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/agents/AgentInitializer.py
--rw-r--r--   0        0        0     1448 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/agents/CSVAgent.py
--rw-r--r--   0        0        0      782 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/agents/JsonAgent.py
--rw-r--r--   0        0        0     3625 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/agents/OpenAIConversationalAgent.py
--rw-r--r--   0        0        0     1104 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/agents/SQLAgent.py
--rw-r--r--   0        0        0     2392 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/agents/ToolCallingAgent.py
--rw-r--r--   0        0        0      869 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/agents/VectorStoreAgent.py
--rw-r--r--   0        0        0      875 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/agents/VectorStoreRouterAgent.py
--rw-r--r--   0        0        0     4147 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/agents/XMLAgent.py
--rw-r--r--   0        0        0      649 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/agents/__init__.py
--rw-r--r--   0        0        0     1535 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/chains/ConversationChain.py
--rw-r--r--   0        0        0     1035 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/chains/LLMChain.py
--rw-r--r--   0        0        0      997 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/chains/LLMCheckerChain.py
--rw-r--r--   0        0        0     1593 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/chains/LLMMathChain.py
--rw-r--r--   0        0        0     2753 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/chains/RetrievalQA.py
--rw-r--r--   0        0        0     2536 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/chains/RetrievalQAWithSourcesChain.py
--rw-r--r--   0        0        0     2332 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/chains/SQLGenerator.py
--rw-r--r--   0        0        0      608 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/chains/__init__.py
--rw-r--r--   0        0        0     3811 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/data/APIRequest.py
--rw-r--r--   0        0        0     2409 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/data/Directory.py
--rw-r--r--   0        0        0     1694 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/data/File.py
--rw-r--r--   0        0        0      725 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/data/URL.py
--rw-r--r--   0        0        0      221 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/data/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/documentloaders/__init__.py
--rw-r--r--   0        0        0     1611 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/embeddings/AmazonBedrockEmbeddings.py
--rw-r--r--   0        0        0     2261 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/embeddings/AzureOpenAIEmbeddings.py
--rw-r--r--   0        0        0     1411 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/embeddings/CohereEmbeddings.py
--rw-r--r--   0        0        0     1547 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/embeddings/HuggingFaceEmbeddings.py
--rw-r--r--   0        0        0     1852 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/embeddings/HuggingFaceInferenceAPIEmbeddings.py
--rw-r--r--   0        0        0     2053 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/embeddings/MistalAIEmbeddings.py
--rw-r--r--   0        0        0     1194 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/embeddings/OllamaEmbeddings.py
--rw-r--r--   0        0        0     5585 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/embeddings/OpenAIEmbeddings.py
--rw-r--r--   0        0        0     3107 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/embeddings/VertexAIEmbeddings.py
--rw-r--r--   0        0        0      833 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/embeddings/__init__.py
--rw-r--r--   0        0        0     7855 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/experimental/AgentComponent.py
--rw-r--r--   0        0        0      785 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/experimental/ClearMessageHistory.py
--rw-r--r--   0        0        0     1519 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/experimental/ExtractDataFromRecord.py
--rw-r--r--   0        0        0     3429 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/experimental/FlowTool.py
--rw-r--r--   0        0        0      497 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/experimental/ListFlows.py
--rw-r--r--   0        0        0      593 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/experimental/Listen.py
--rw-r--r--   0        0        0      983 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/experimental/MergeRecords.py
--rw-r--r--   0        0        0     1448 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/experimental/Notify.py
--rw-r--r--   0        0        0     1198 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/experimental/Pass.py
--rw-r--r--   0        0        0      729 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/experimental/PythonFunction.py
--rw-r--r--   0        0        0     2376 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/experimental/RunFlow.py
--rw-r--r--   0        0        0     4719 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/experimental/RunnableExecutor.py
--rw-r--r--   0        0        0     2338 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/experimental/SQLExecutor.py
--rw-r--r--   0        0        0     1540 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/experimental/SplitText.py
--rw-r--r--   0        0        0     1321 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/experimental/StoreMessage.py
--rw-r--r--   0        0        0     5190 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/experimental/SubFlow.py
--rw-r--r--   0        0        0     2777 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/experimental/TextOperator.py
--rw-r--r--   0        0        0     1001 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/experimental/__init__.py
--rw-r--r--   0        0        0     1035 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/helpers/CombineText.py
--rw-r--r--   0        0        0      882 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/helpers/CombineTextsUnsorted.py
--rw-r--r--   0        0        0     3257 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/helpers/CreateRecord.py
--rw-r--r--   0        0        0      553 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/helpers/CustomComponent.py
--rw-r--r--   0        0        0      689 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/helpers/DocumentToRecord.py
--rw-r--r--   0        0        0      840 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/helpers/IDGenerator.py
--rw-r--r--   0        0        0     2996 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/helpers/MemoryComponent.py
--rw-r--r--   0        0        0     1865 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/helpers/MessageHistory.py
--rw-r--r--   0        0        0     1169 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/helpers/RecordsToText.py
--rw-r--r--   0        0        0     1331 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/helpers/ShouldRunNext.py
--rw-r--r--   0        0        0     1116 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/helpers/UpdateRecord.py
--rw-r--r--   0        0        0      555 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/helpers/__init__.py
--rw-r--r--   0        0        0     1063 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/inputs/ChatInput.py
--rw-r--r--   0        0        0     1161 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/inputs/Prompt.py
--rw-r--r--   0        0        0     1032 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/inputs/TextInput.py
--rw-r--r--   0        0        0      159 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/inputs/__init__.py
--rw-r--r--   0        0        0     1279 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/langchain_utilities/BingSearchAPIWrapper.py
--rw-r--r--   0        0        0      813 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/langchain_utilities/GoogleSearchAPIWrapper.py
--rw-r--r--   0        0        0     1706 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/langchain_utilities/GoogleSerperAPIWrapper.py
--rw-r--r--   0        0        0     1599 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/langchain_utilities/JSONDocumentBuilder.py
--rw-r--r--   0        0        0      677 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/langchain_utilities/SQLDatabase.py
--rw-r--r--   0        0        0     1584 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/langchain_utilities/SearchApi.py
--rw-r--r--   0        0        0     1164 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/langchain_utilities/SearxSearchWrapper.py
--rw-r--r--   0        0        0     1039 2024-05-24 01:13:47.324054 langflow_base-0.0.48/langflow/components/langchain_utilities/SerpAPIWrapper.py
--rw-r--r--   0        0        0     1037 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/langchain_utilities/WikipediaAPIWrapper.py
--rw-r--r--   0        0        0      735 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/langchain_utilities/WolframAlphaAPIWrapper.py
--rw-r--r--   0        0        0     3042 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/memories/AstraDBMessageReader.py
--rw-r--r--   0        0        0     3833 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/memories/AstraDBMessageWriter.py
--rw-r--r--   0        0        0     6008 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/memories/ZepMessageReader.py
--rw-r--r--   0        0        0     3956 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/memories/ZepMessageWriter.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/memories/__init__.py
--rw-r--r--   0        0        0     2295 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/model_specs/AmazonBedrockSpecs.py
--rw-r--r--   0        0        0     2627 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/model_specs/AnthropicLLMSpecs.py
--rw-r--r--   0        0        0     3360 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/model_specs/AzureChatOpenAISpecs.py
--rw-r--r--   0        0        0     3653 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/model_specs/BaiduQianfanChatEndpointsSpecs.py
--rw-r--r--   0        0        0     3565 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/model_specs/BaiduQianfanLLMEndpointsSpecs.py
--rw-r--r--   0        0        0     2905 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/model_specs/ChatAnthropicSpecs.py
--rw-r--r--   0        0        0     5878 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/model_specs/ChatLiteLLMSpecs.py
--rw-r--r--   0        0        0     2763 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/model_specs/ChatMistralSpecs.py
--rw-r--r--   0        0        0     9872 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/model_specs/ChatOllamaEndpointSpecs.py
--rw-r--r--   0        0        0     2487 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/model_specs/ChatOpenAISpecs.py
--rw-r--r--   0        0        0     2657 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/model_specs/ChatVertexAISpecs.py
--rw-r--r--   0        0        0     1075 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/model_specs/CohereSpecs.py
--rw-r--r--   0        0        0     2885 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/model_specs/GoogleGenerativeAISpecs.py
--rw-r--r--   0        0        0     2814 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/model_specs/GroqModelSpecs.py
--rw-r--r--   0        0        0     1644 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/model_specs/HuggingFaceEndpointsSpecs.py
--rw-r--r--   0        0        0     5795 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/model_specs/OllamaLLMSpecs.py
--rw-r--r--   0        0        0     4813 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/model_specs/VertexAISpecs.py
--rw-r--r--   0        0        0     1167 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/model_specs/__init__.py
--rw-r--r--   0        0        0     3630 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/models/AmazonBedrockModel.py
--rw-r--r--   0        0        0     3621 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/models/AnthropicModel.py
--rw-r--r--   0        0        0     3891 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/models/AzureOpenAIModel.py
--rw-r--r--   0        0        0     4421 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/models/BaiduQianfanChatModel.py
--rw-r--r--   0        0        0     6512 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/models/ChatLiteLLMModel.py
--rw-r--r--   0        0        0     2219 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/models/CohereModel.py
--rw-r--r--   0        0        0     3695 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/models/GoogleGenerativeAIModel.py
--rw-r--r--   0        0        0     3223 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/models/GroqModel.py
--rw-r--r--   0        0        0     2631 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/models/HuggingFaceModel.py
--rw-r--r--   0        0        0     4501 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/models/MistralModel.py
--rw-r--r--   0        0        0    11131 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/models/OllamaModel.py
--rw-r--r--   0        0        0     3259 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/models/OpenAIModel.py
--rw-r--r--   0        0        0     3762 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/models/VertexAiModel.py
--rw-r--r--   0        0        0      934 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/models/__init__.py
--rw-r--r--   0        0        0      921 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/outputs/ChatOutput.py
--rw-r--r--   0        0        0      282 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/outputs/RecordsOutput.py
--rw-r--r--   0        0        0     1008 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/outputs/TextOutput.py
--rw-r--r--   0        0        0      110 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/outputs/__init__.py
--rw-r--r--   0        0        0     1822 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/retrievers/AmazonKendra.py
--rw-r--r--   0        0        0     1135 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/retrievers/MetalRetriever.py
--rw-r--r--   0        0        0     2260 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/retrievers/MultiQueryRetriever.py
--rw-r--r--   0        0        0     2530 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/retrievers/VectaraSelfQueryRetriver.py
--rw-r--r--   0        0        0      574 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/retrievers/VectorStoreRetriever.py
--rw-r--r--   0        0        0      503 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/retrievers/__init__.py
--rw-r--r--   0        0        0     1550 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/textsplitters/CharacterTextSplitter.py
--rw-r--r--   0        0        0     3074 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/textsplitters/LanguageRecursiveTextSplitter.py
--rw-r--r--   0        0        0     3330 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/textsplitters/RecursiveCharacterTextSplitter.py
--rw-r--r--   0        0        0      378 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/textsplitters/__init__.py
--rw-r--r--   0        0        0      554 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/toolkits/JsonToolkit.py
--rw-r--r--   0        0        0     1813 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/toolkits/Metaphor.py
--rw-r--r--   0        0        0      844 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/toolkits/OpenAPIToolkit.py
--rw-r--r--   0        0        0      812 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/toolkits/VectorStoreInfo.py
--rw-r--r--   0        0        0      884 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/toolkits/VectorStoreRouterToolkit.py
--rw-r--r--   0        0        0      811 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/toolkits/VectorStoreToolkit.py
--rw-r--r--   0        0        0      527 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/toolkits/__init__.py
--rw-r--r--   0        0        0     2706 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/tools/PythonREPLTool.py
--rw-r--r--   0        0        0      996 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/tools/RetrieverTool.py
--rw-r--r--   0        0        0     1132 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/tools/SearchAPITool.py
--rw-r--r--   0        0        0     1584 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/tools/SearchApi.py
--rw-r--r--   0        0        0      290 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/tools/__init__.py
--rw-r--r--   0        0        0     6489 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/vectorsearch/AstraDBSearch.py
--rw-r--r--   0        0        0     4666 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/vectorsearch/ChromaSearch.py
--rw-r--r--   0        0        0     2870 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/vectorsearch/CouchbaseSearch.py
--rw-r--r--   0        0        0     1875 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/vectorsearch/FAISSSearch.py
--rw-r--r--   0        0        0     2307 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/vectorsearch/MongoDBAtlasVectorSearch.py
--rw-r--r--   0        0        0     3551 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/vectorsearch/PineconeSearch.py
--rw-r--r--   0        0        0     4085 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/vectorsearch/QdrantSearch.py
--rw-r--r--   0        0        0     3003 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/vectorsearch/RedisSearch.py
--rw-r--r--   0        0        0     2048 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/vectorsearch/SupabaseVectorStoreSearch.py
--rw-r--r--   0        0        0     2215 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/vectorsearch/VectaraSearch.py
--rw-r--r--   0        0        0     2854 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/vectorsearch/WeaviateSearch.py
--rw-r--r--   0        0        0     1020 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/vectorsearch/__init__.py
--rw-r--r--   0        0        0     2660 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/vectorsearch/pgvectorSearch.py
--rw-r--r--   0        0        0     7031 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/vectorstores/AstraDB.py
--rw-r--r--   0        0        0     5137 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/vectorstores/Chroma.py
--rw-r--r--   0        0        0     3551 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/vectorstores/Couchbase.py
--rw-r--r--   0        0        0     1811 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/vectorstores/FAISS.py
--rw-r--r--   0        0        0     2464 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/vectorstores/MongoDBAtlasVector.py
--rw-r--r--   0        0        0     5572 2024-05-24 01:13:47.328054 langflow_base-0.0.48/langflow/components/vectorstores/Pinecone.py
--rw-r--r--   0        0        0     4409 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/components/vectorstores/Qdrant.py
--rw-r--r--   0        0        0     3100 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/components/vectorstores/Redis.py
--rw-r--r--   0        0        0     1894 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/components/vectorstores/SupabaseVectorStore.py
--rw-r--r--   0        0        0     3025 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/components/vectorstores/Vectara.py
--rw-r--r--   0        0        0     3678 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/components/vectorstores/Weaviate.py
--rw-r--r--   0        0        0      847 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/components/vectorstores/__init__.py
--rw-r--r--   0        0        0       80 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/components/vectorstores/base/__init__.py
--rw-r--r--   0        0        0     1645 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/components/vectorstores/base/model.py
--rw-r--r--   0        0        0     2902 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/components/vectorstores/pgvector.py
--rw-r--r--   0        0        0    10194 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/config.yaml
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/core/__init__.py
--rw-r--r--   0        0        0      351 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/core/celery_app.py
--rw-r--r--   0        0        0      778 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/core/celeryconfig.py
--rw-r--r--   0        0        0       85 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/custom.py
--rw-r--r--   0        0        0     1485 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/field_typing/__init__.py
--rw-r--r--   0        0        0     1821 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/field_typing/constants.py
--rw-r--r--   0        0        0     1060 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/field_typing/range_spec.py
--rw-r--r--   0        0        0      423 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/a-arrow-down-338b684d.js
--rw-r--r--   0        0        0      422 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/a-arrow-up-60532c04.js
--rw-r--r--   0        0        0      444 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/a-large-small-1fd2cf94.js
--rw-r--r--   0        0        0      513 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/accessibility-7deeca04.js
--rw-r--r--   0        0        0      312 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/activity-c184725f.js
--rw-r--r--   0        0        0      384 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/activity-square-88b26d9e.js
--rw-r--r--   0        0        0      541 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/air-vent-f05f65f0.js
--rw-r--r--   0        0        0      419 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/airplay-ecb19158.js
--rw-r--r--   0        0        0      514 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/alarm-clock-b53682c1.js
--rw-r--r--   0        0        0      521 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/alarm-clock-check-d3b32670.js
--rw-r--r--   0        0        0      515 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/alarm-clock-minus-fc96df2e.js
--rw-r--r--   0        0        0      543 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/alarm-clock-off-6a0418e2.js
--rw-r--r--   0        0        0      551 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/alarm-clock-plus-bfb4a090.js
--rw-r--r--   0        0        0      562 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/alarm-smoke-f5027e9e.js
--rw-r--r--   0        0        0      392 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/album-7e1574fb.js
--rw-r--r--   0        0        0      483 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/alert-octagon-d9330aa2.js
--rw-r--r--   0        0        0      440 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/alert-triangle-5cb2282d.js
--rw-r--r--   0        0        0      424 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/align-center-506fc132.js
--rw-r--r--   0        0        0      585 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/align-center-horizontal-e3305b6c.js
--rw-r--r--   0        0        0      583 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/align-center-vertical-6fd65fe5.js
--rw-r--r--   0        0        0      435 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/align-end-horizontal-56dd8854.js
--rw-r--r--   0        0        0      433 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/align-end-vertical-c2761c94.js
--rw-r--r--   0        0        0      558 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/align-horizontal-distribute-center-6966cea5.js
--rw-r--r--   0        0        0      483 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/align-horizontal-distribute-end-e4d8f68b.js
--rw-r--r--   0        0        0      484 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/align-horizontal-distribute-start-deef9a79.js
--rw-r--r--   0        0        0      446 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/align-horizontal-justify-center-54c1ffd6.js
--rw-r--r--   0        0        0      443 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/align-horizontal-justify-end-35555d6d.js
--rw-r--r--   0        0        0      444 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/align-horizontal-justify-start-8c57d718.js
--rw-r--r--   0        0        0      414 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/align-horizontal-space-around-1fc8c174.js
--rw-r--r--   0        0        0      481 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/align-horizontal-space-between-fe30b7bb.js
--rw-r--r--   0        0        0      425 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/align-justify-7430845d.js
--rw-r--r--   0        0        0      422 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/align-left-98f95c28.js
--rw-r--r--   0        0        0      423 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/align-right-4454a958.js
--rw-r--r--   0        0        0      436 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/align-start-horizontal-b9435ff6.js
--rw-r--r--   0        0        0      434 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/align-start-vertical-5f600266.js
--rw-r--r--   0        0        0      556 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/align-vertical-distribute-center-e4878d08.js
--rw-r--r--   0        0        0      481 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/align-vertical-distribute-end-7cd22002.js
--rw-r--r--   0        0        0      482 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/align-vertical-distribute-start-6c0545ec.js
--rw-r--r--   0        0        0      444 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/align-vertical-justify-center-bb10c107.js
--rw-r--r--   0        0        0      441 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/align-vertical-justify-end-3f0569f5.js
--rw-r--r--   0        0        0      442 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/align-vertical-justify-start-865ed5d0.js
--rw-r--r--   0        0        0      412 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/align-vertical-space-around-07b5b726.js
--rw-r--r--   0        0        0      479 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/align-vertical-space-between-a733674f.js
--rw-r--r--   0        0        0      692 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/ambulance-b3609100.js
--rw-r--r--   0        0        0      416 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/ampersand-f5a2e3aa.js
--rw-r--r--   0        0        0      480 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/ampersands-d0253acc.js
--rw-r--r--   0        0        0      391 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/anchor-73a68d00.js
--rw-r--r--   0        0        0      511 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/angry-c69f99c1.js
--rw-r--r--   0        0        0      412 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/annoyed-0943735a.js
--rw-r--r--   0        0        0      489 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/antenna-2235cf56.js
--rw-r--r--   0        0        0      502 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/anvil-fb30cafa.js
--rw-r--r--   0        0        0      581 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/aperture-ae888f7c.js
--rw-r--r--   0        0        0      432 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/app-window-0aa03576.js
--rw-r--r--   0        0        0      491 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/apple-f15b18b1.js
--rw-r--r--   0        0        0      428 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/archive-2683c9a2.js
--rw-r--r--   0        0        0      514 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/archive-restore-34113244.js
--rw-r--r--   0        0        0      472 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/archive-x-66c84c4a.js
--rw-r--r--   0        0        0      349 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/area-chart-16f6cfc6.js
--rw-r--r--   0        0        0      503 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/armchair-a28f314e.js
--rw-r--r--   0        0        0      316 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/arrow-big-down-703869c0.js
--rw-r--r--   0        0        0      354 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/arrow-big-down-dash-d4a5f63d.js
--rw-r--r--   0        0        0      318 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/arrow-big-left-8aeb87df.js
--rw-r--r--   0        0        0      359 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/arrow-big-left-dash-0e9d8ada.js
--rw-r--r--   0        0        0      316 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/arrow-big-right-0d80daa8.js
--rw-r--r--   0        0        0      355 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/arrow-big-right-dash-ad8cf79f.js
--rw-r--r--   0        0        0      355 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/arrow-big-up-dash-bb5022b6.js
--rw-r--r--   0        0        0      482 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/arrow-down-0-1-1849a1e5.js
--rw-r--r--   0        0        0      482 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/arrow-down-1-0-93c1214c.js
--rw-r--r--   0        0        0      339 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-down-15182de4.js
--rw-r--r--   0        0        0      480 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-down-a-z-2f5cf730.js
--rw-r--r--   0        0        0      392 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-down-circle-02d39da3.js
--rw-r--r--   0        0        0      382 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/arrow-down-from-line-79907b98.js
--rw-r--r--   0        0        0      341 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-down-left-72dcddc0.js
--rw-r--r--   0        0        0      404 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-down-left-from-circle-f6565ead.js
--rw-r--r--   0        0        0      435 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-down-left-from-square-c5d61426.js
--rw-r--r--   0        0        0      412 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/arrow-down-left-square-03b5a2e2.js
--rw-r--r--   0        0        0      457 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-down-narrow-wide-b192f668.js
--rw-r--r--   0        0        0      342 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-down-right-f81908eb.js
--rw-r--r--   0        0        0      408 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-down-right-from-circle-54dfc45c.js
--rw-r--r--   0        0        0      439 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-down-right-from-square-eb44ce78.js
--rw-r--r--   0        0        0      411 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-down-right-square-db440ed9.js
--rw-r--r--   0        0        0      409 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-down-square-14d38d87.js
--rw-r--r--   0        0        0      391 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-down-to-dot-97c32166.js
--rw-r--r--   0        0        0      381 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-down-to-line-c854a162.js
--rw-r--r--   0        0        0      418 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-down-up-503d530e.js
--rw-r--r--   0        0        0      457 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-down-wide-narrow-73411b65.js
--rw-r--r--   0        0        0      481 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-down-z-a-0a8f0a5a.js
--rw-r--r--   0        0        0      393 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-left-circle-9e413a44.js
--rw-r--r--   0        0        0      382 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-left-from-line-7e401686.js
--rw-r--r--   0        0        0      421 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-left-right-c015b85a.js
--rw-r--r--   0        0        0      410 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-left-square-76b0c96b.js
--rw-r--r--   0        0        0      380 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-left-to-line-da4690d3.js
--rw-r--r--   0        0        0      339 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/arrow-right-1d0201a6.js
--rw-r--r--   0        0        0      389 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-right-circle-bb3d7c2d.js
--rw-r--r--   0        0        0      384 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-right-from-line-114a0b5c.js
--rw-r--r--   0        0        0      421 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-right-left-c17dbdf5.js
--rw-r--r--   0        0        0      411 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-right-square-e2e3c49c.js
--rw-r--r--   0        0        0      383 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/arrow-right-to-line-eb08b9fd.js
--rw-r--r--   0        0        0      479 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/arrow-up-0-1-82594474.js
--rw-r--r--   0        0        0      336 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/arrow-up-01a00be9.js
--rw-r--r--   0        0        0      479 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/arrow-up-1-0-021af6b1.js
--rw-r--r--   0        0        0      477 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/arrow-up-a-z-b8c69625.js
--rw-r--r--   0        0        0      392 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/arrow-up-circle-99b08177.js
--rw-r--r--   0        0        0      418 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/arrow-up-down-56751fc0.js
--rw-r--r--   0        0        0      390 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/arrow-up-from-dot-0be5e248.js
--rw-r--r--   0        0        0      381 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/arrow-up-from-line-53ee15ad.js
--rw-r--r--   0        0        0      339 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/arrow-up-left-2a24a4d7.js
--rw-r--r--   0        0        0      398 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/arrow-up-left-from-circle-32c439ee.js
--rw-r--r--   0        0        0      431 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrow-up-left-from-square-01fc1e48.js
--rw-r--r--   0        0        0      410 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/arrow-up-left-square-2b91a55f.js
--rw-r--r--   0        0        0      456 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/arrow-up-narrow-wide-17ff0540.js
--rw-r--r--   0        0        0      340 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/arrow-up-right-1a25e20d.js
--rw-r--r--   0        0        0      402 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/arrow-up-right-from-circle-b5869313.js
--rw-r--r--   0        0        0      433 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/arrow-up-right-from-square-a65d79d4.js
--rw-r--r--   0        0        0      409 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/arrow-up-right-square-344bad1c.js
--rw-r--r--   0        0        0      409 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/arrow-up-square-b238a11c.js
--rw-r--r--   0        0        0      456 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/arrow-up-wide-narrow-49508601.js
--rw-r--r--   0        0        0      478 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/arrow-up-z-a-89c31683.js
--rw-r--r--   0        0        0      459 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/arrows-up-from-line-353e8880.js
--rw-r--r--   0        0        0      388 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/asterisk-d519fe8d.js
--rw-r--r--   0        0        0      446 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/asterisk-square-627151cc.js
--rw-r--r--   0        0        0      368 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/at-sign-e494f28f.js
--rw-r--r--   0        0        0      603 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/atom-634b4c72.js
--rw-r--r--   0        0        0      479 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/audio-lines-c710554a.js
--rw-r--r--   0        0        0      394 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/audio-waveform-72cc8864.js
--rw-r--r--   0        0        0      365 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/award-838dab96.js
--rw-r--r--   0        0        0      385 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/axe-c8895529.js
--rw-r--r--   0        0        0      333 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/axis-3d-ed2aa0d7.js
--rw-r--r--   0        0        0      565 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/baby-804d807f.js
--rw-r--r--   0        0        0      564 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/backpack-6bb8f8dc.js
--rw-r--r--   0        0        0      443 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/badge-15f43f3b.js
--rw-r--r--   0        0        0      562 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/badge-alert-2792746a.js
--rw-r--r--   0        0        0      535 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/badge-cent-9c74db33.js
--rw-r--r--   0        0        0      490 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/badge-check-67516e36.js
--rw-r--r--   0        0        0      559 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/badge-dollar-sign-534ee5dd.js
--rw-r--r--   0        0        0      535 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/badge-euro-e86cd8b5.js
--rw-r--r--   0        0        0      571 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/badge-help-a99e4c15.js
--rw-r--r--   0        0        0      580 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/badge-indian-rupee-b932ef23.js
--rw-r--r--   0        0        0      560 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/badge-info-38c2f4b4.js
--rw-r--r--   0        0        0      604 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/badge-japanese-yen-f7736118.js
--rw-r--r--   0        0        0      503 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/badge-minus-2b2d9863.js
--rw-r--r--   0        0        0      564 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/badge-percent-96abe075.js
--rw-r--r--   0        0        0      557 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/badge-plus-ef608fba.js
--rw-r--r--   0        0        0      585 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/badge-pound-sterling-5e65ad38.js
--rw-r--r--   0        0        0      546 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/badge-russian-ruble-b25d9ad9.js
--rw-r--r--   0        0        0      565 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/badge-swiss-franc-3060d493.js
--rw-r--r--   0        0        0      552 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/badge-x-0845dea8.js
--rw-r--r--   0        0        0      560 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/baggage-claim-4b4424f5.js
--rw-r--r--   0        0        0      344 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/ban-2d975df8.js
--rw-r--r--   0        0        0      492 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/banana-a2f8f835.js
--rw-r--r--   0        0        0      420 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/banknote-ef157399.js
--rw-r--r--   0        0        0      423 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/bar-chart-1b02f895.js
--rw-r--r--   0        0        0      424 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/bar-chart-2-8a9cea9c.js
--rw-r--r--   0        0        0      409 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/bar-chart-3-906213ee.js
--rw-r--r--   0        0        0      409 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/bar-chart-4-686d3252.js
--rw-r--r--   0        0        0      431 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/bar-chart-big-b17c6716.js
--rw-r--r--   0        0        0      415 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/bar-chart-horizontal-576570cf.js
--rw-r--r--   0        0        0      440 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/bar-chart-horizontal-big-5ae473e6.js
--rw-r--r--   0        0        0      440 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/barcode-958cbc2c.js
--rw-r--r--   0        0        0      375 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/baseline-c9ed7767.js
--rw-r--r--   0        0        0      591 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/bath-52eb7e8c.js
--rw-r--r--   0        0        0      386 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/battery-49889fb9.js
--rw-r--r--   0        0        0      502 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/battery-charging-a0b81b04.js
--rw-r--r--   0        0        0      556 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/battery-full-67d8a9b3.js
--rw-r--r--   0        0        0      443 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/battery-low-9d9655fb.js
--rw-r--r--   0        0        0      502 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/battery-medium-0eab96f5.js
--rw-r--r--   0        0        0      566 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/battery-warning-62ab1682.js
--rw-r--r--   0        0        0      399 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/beaker-30d946d7.js
--rw-r--r--   0        0        0      476 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/bean-4d702040.js
--rw-r--r--   0        0        0      603 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/bean-off-7b09212a.js
--rw-r--r--   0        0        0      414 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/bed-95c1ff23.js
--rw-r--r--   0        0        0      471 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/bed-double-dc7b8344.js
--rw-r--r--   0        0        0      435 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/bed-single-b69bd325.js
--rw-r--r--   0        0        0      593 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/beef-9bf4ee37.js
--rw-r--r--   0        0        0      642 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/beer-41f73772.js
--rw-r--r--   0        0        0      466 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/bell-dot-973b925e.js
--rw-r--r--   0        0        0      569 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/bell-electric-5dc74521.js
--rw-r--r--   0        0        0      454 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/bell-minus-75b6bb37.js
--rw-r--r--   0        0        0      494 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/bell-off-013dd363.js
--rw-r--r--   0        0        0      492 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/bell-plus-35794ca9.js
--rw-r--r--   0        0        0      489 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/bell-ring-d87fc621.js
--rw-r--r--   0        0        0      444 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/between-horizontal-end-8154d6be.js
--rw-r--r--   0        0        0      444 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/between-horizontal-start-b3ebce6e.js
--rw-r--r--   0        0        0      441 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/between-vertical-end-5e57d29a.js
--rw-r--r--   0        0        0      443 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/between-vertical-start-09c1d3e1.js
--rw-r--r--   0        0        0      458 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/bike-0db4bab8.js
--rw-r--r--   0        0        0      856 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/biohazard-7f870d29.js
--rw-r--r--   0        0        0      548 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/bird-ad099b8b.js
--rw-r--r--   0        0        0      509 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/bitcoin-ed65414a.js
--rw-r--r--   0        0        0      344 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/blend-da79df0d.js
--rw-r--r--   0        0        0      523 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/blinds-9d36e4b5.js
--rw-r--r--   0        0        0      313 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/bluetooth-c725ba5e.js
--rw-r--r--   0        0        0      432 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/bluetooth-connected-4c6854cc.js
--rw-r--r--   0        0        0      400 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/bluetooth-off-c097243a.js
--rw-r--r--   0        0        0      419 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/bluetooth-searching-8a896819.js
--rw-r--r--   0        0        0      361 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/bold-701f2144.js
--rw-r--r--   0        0        0      452 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/bolt-c268ffe9.js
--rw-r--r--   0        0        0      453 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/bomb-cc1a91f7.js
--rw-r--r--   0        0        0      470 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/bone-cc6365d6.js
--rw-r--r--   0        0        0      345 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/book-58172484.js
--rw-r--r--   0        0        0      428 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/book-a-6f4d63ca.js
--rw-r--r--   0        0        0      457 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/book-audio-1fb3edb9.js
--rw-r--r--   0        0        0      393 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/book-check-cadcac19.js
--rw-r--r--   0        0        0      440 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/book-copy-196a2644.js
--rw-r--r--   0        0        0      714 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/book-dashed-86cbe767.js
--rw-r--r--   0        0        0      428 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/book-down-3d1b2c2a.js
--rw-r--r--   0        0        0      503 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/book-headphones-3104e0cd.js
--rw-r--r--   0        0        0      526 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/book-heart-8beae983.js
--rw-r--r--   0        0        0      467 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/book-image-3a884dca.js
--rw-r--r--   0        0        0      509 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/book-key-049e6543.js
--rw-r--r--   0        0        0      500 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/book-lock-2c04fc1c.js
--rw-r--r--   0        0        0      386 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/book-minus-5455678a.js
--rw-r--r--   0        0        0      398 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/book-open-a5fffbd9.js
--rw-r--r--   0        0        0      463 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/book-open-check-614c22a6.js
--rw-r--r--   0        0        0      546 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/book-open-text-0c4694bc.js
--rw-r--r--   0        0        0      421 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/book-plus-72092ac0.js
--rw-r--r--   0        0        0      420 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/book-text-8fc03a16.js
--rw-r--r--   0        0        0      462 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/book-type-9f03d08e.js
--rw-r--r--   0        0        0      501 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/book-up-2-42570482.js
--rw-r--r--   0        0        0      426 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/book-up-8a64d962.js
--rw-r--r--   0        0        0      445 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/book-user-3222d5f5.js
--rw-r--r--   0        0        0      425 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/book-x-fe5f9aa3.js
--rw-r--r--   0        0        0      338 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/bookmark-806c6c55.js
--rw-r--r--   0        0        0      382 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/bookmark-check-56bf6079.js
--rw-r--r--   0        0        0      398 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/bookmark-minus-c8279111.js
--rw-r--r--   0        0        0      419 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/bookmark-x-cb28f311.js
--rw-r--r--   0        0        0      588 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/boom-box-4e291b8b.js
--rw-r--r--   0        0        0      485 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/box-7261d0ef.js
--rw-r--r--   0        0        0      739 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/box-select-b0ef4e91.js
--rw-r--r--   0        0        0      340 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/brackets-fc62ae99.js
--rw-r--r--   0        0        0      958 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/brain-cog-3d4bb4c6.js
--rw-r--r--   0        0        0      637 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/brain-d34d8a4b.js
--rw-r--r--   0        0        0      578 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/brick-wall-b5fb72e9.js
--rw-r--r--   0        0        0      403 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/briefcase-f0c60756.js
--rw-r--r--   0        0        0      488 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/bring-to-front-33a69782.js
--rw-r--r--   0        0        0      495 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/brush-aed7dc33.js
--rw-r--r--   0        0        0      841 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/bug-c0e4b5c7.js
--rw-r--r--   0        0        0      722 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/bug-off-221980ea.js
--rw-r--r--   0        0        0      741 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/bug-play-d73bf6fc.js
--rw-r--r--   0        0        0      613 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/building-2-6f46c282.js
--rw-r--r--   0        0        0      717 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/building-af553e71.js
--rw-r--r--   0        0        0      622 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/bus-5900cfa3.js
--rw-r--r--   0        0        0      623 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/bus-front-7dc8cedb.js
--rw-r--r--   0        0        0      620 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/cable-a48206d9.js
--rw-r--r--   0        0        0      588 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/cable-car-ec551b2e.js
--rw-r--r--   0        0        0      665 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/cake-edd21758.js
--rw-r--r--   0        0        0      472 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/cake-slice-9083d9b8.js
--rw-r--r--   0        0        0      705 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/calculator-9ba50681.js
--rw-r--r--   0        0        0      501 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/calendar-check-2-b5080d83.js
--rw-r--r--   0        0        0      479 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/calendar-check-d1639410.js
--rw-r--r--   0        0        0      557 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/calendar-clock-ea51db8f.js
--rw-r--r--   0        0        0      668 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/calendar-days-ef7e5a38.js
--rw-r--r--   0        0        0      432 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/calendar-e79a04d6.js
--rw-r--r--   0        0        0      512 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/calendar-fold-1da81079.js
--rw-r--r--   0        0        0      632 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/calendar-heart-5677e0b9.js
--rw-r--r--   0        0        0      475 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/calendar-minus-2-10e1944c.js
--rw-r--r--   0        0        0      494 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/calendar-minus-8e18db70.js
--rw-r--r--   0        0        0      560 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/calendar-off-0bd1e591.js
--rw-r--r--   0        0        0      511 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/calendar-plus-2-28f4ce9f.js
--rw-r--r--   0        0        0      530 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/calendar-plus-73dc0684.js
--rw-r--r--   0        0        0      589 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/calendar-range-83746210.js
--rw-r--r--   0        0        0      551 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/calendar-search-02e8602b.js
--rw-r--r--   0        0        0      511 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/calendar-x-1190d7bb.js
--rw-r--r--   0        0        0      532 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/calendar-x-2-b568f6b9.js
--rw-r--r--   0        0        0      423 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/camera-251bf339.js
--rw-r--r--   0        0        0      507 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/camera-off-60b4968e.js
--rw-r--r--   0        0        0      578 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/candlestick-chart-1765be54.js
--rw-r--r--   0        0        0      617 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/candy-7dd2ee96.js
--rw-r--r--   0        0        0      547 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/candy-cane-0be5742f.js
--rw-r--r--   0        0        0      811 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/candy-off-523922e8.js
--rw-r--r--   0        0        0      390 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/captions-41e269e3.js
--rw-r--r--   0        0        0      537 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/captions-off-2f69fa80.js
--rw-r--r--   0        0        0      577 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/car-d4fab838.js
--rw-r--r--   0        0        0      574 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/car-front-a8753e88.js
--rw-r--r--   0        0        0      614 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/car-taxi-front-7222b3f3.js
--rw-r--r--   0        0        0      546 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/caravan-7e780ccf.js
--rw-r--r--   0        0        0      590 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/carrot-1da699eb.js
--rw-r--r--   0        0        0      421 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/case-lower-26d2ce81.js
--rw-r--r--   0        0        0      425 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/case-sensitive-03494efb.js
--rw-r--r--   0        0        0      411 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/case-upper-90d8233f.js
--rw-r--r--   0        0        0      550 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/cassette-tape-11ee7a3e.js
--rw-r--r--   0        0        0      493 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/cast-60db50b8.js
--rw-r--r--   0        0        0      657 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/castle-aa353636.js
--rw-r--r--   0        0        0      634 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/cat-b10af0e4.js
--rw-r--r--   0        0        0      559 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/cctv-c9b74e6f.js
--rw-r--r--   0        0        0      353 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/check-check-3fbd6fcb.js
--rw-r--r--   0        0        0      367 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/check-circle-86d25b90.js
--rw-r--r--   0        0        0      370 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/check-square-2-3fe1db0e.js
--rw-r--r--   0        0        0      390 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/check-square-ca7352fc.js
--rw-r--r--   0        0        0      458 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/chef-hat-9abd6519.js
--rw-r--r--   0        0        0      577 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/cherry-ec8c07da.js
--rw-r--r--   0        0        0      359 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/chevron-down-circle-ef290fe2.js
--rw-r--r--   0        0        0      376 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/chevron-down-square-a70a006b.js
--rw-r--r--   0        0        0      341 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/chevron-first-6730d035.js
--rw-r--r--   0        0        0      340 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/chevron-last-69617516.js
--rw-r--r--   0        0        0      359 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/chevron-left-circle-072df83c.js
--rw-r--r--   0        0        0      376 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/chevron-left-square-88d1452c.js
--rw-r--r--   0        0        0      359 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/chevron-right-circle-50d7679b.js
--rw-r--r--   0        0        0      356 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/chevron-up-circle-50393f96.js
--rw-r--r--   0        0        0      373 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/chevron-up-square-05a06445.js
--rw-r--r--   0        0        0      345 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/chevrons-down-acd0eac0.js
--rw-r--r--   0        0        0      347 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/chevrons-down-up-defb4639.js
--rw-r--r--   0        0        0      350 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/chevrons-left-right-00bef326.js
--rw-r--r--   0        0        0      352 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/chevrons-right-left-d128c9b7.js
--rw-r--r--   0        0        0      346 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/chevrons-up-735bd5ef.js
--rw-r--r--   0        0        0      537 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/chrome-214e9f29.js
--rw-r--r--   0        0        0      523 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/church-82bb793c.js
--rw-r--r--   0        0        0      474 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/cigarette-782cc077.js
--rw-r--r--   0        0        0      570 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/cigarette-off-6e801ae2.js
--rw-r--r--   0        0        0      748 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/circle-dashed-ceb50c6a.js
--rw-r--r--   0        0        0      421 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/circle-dollar-sign-d1e628b4.js
--rw-r--r--   0        0        0      815 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/circle-dot-dashed-0eb51089.js
--rw-r--r--   0        0        0      429 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/circle-ellipsis-e53f5a9e.js
--rw-r--r--   0        0        0      379 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/circle-equal-ed683c0f.js
--rw-r--r--   0        0        0      636 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/circle-fading-plus-f5dbfc16.js
--rw-r--r--   0        0        0      423 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/circle-off-9e5cb236.js
--rw-r--r--   0        0        0      345 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/circle-slash-2-dcd430b1.js
--rw-r--r--   0        0        0      359 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/circle-slash-b9a0b0c5.js
--rw-r--r--   0        0        0      429 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/circle-user-45fedf2a.js
--rw-r--r--   0        0        0      407 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/circle-user-round-6a9cf9c4.js
--rw-r--r--   0        0        0      522 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/circuit-board-7cd682a8.js
--rw-r--r--   0        0        0      517 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/citrus-f0326961.js
--rw-r--r--   0        0        0      521 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/clapperboard-b8e90a42.js
--rw-r--r--   0        0        0      478 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/clipboard-check-e00df14e.js
--rw-r--r--   0        0        0      553 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/clipboard-copy-61b23095.js
--rw-r--r--   0        0        0      585 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/clipboard-list-5426b358.js
--rw-r--r--   0        0        0      472 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/clipboard-minus-a9a93ea5.js
--rw-r--r--   0        0        0      520 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/clipboard-paste-ee5d0d42.js
--rw-r--r--   0        0        0      520 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/clipboard-pen-7403e404.js
--rw-r--r--   0        0        0      574 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/clipboard-pen-line-21803d72.js
--rw-r--r--   0        0        0      509 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/clipboard-plus-7c095619.js
--rw-r--r--   0        0        0      550 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/clipboard-type-f743f70a.js
--rw-r--r--   0        0        0      509 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/clipboard-x-d56d3409.js
--rw-r--r--   0        0        0      355 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/clock-1-b94fcef7.js
--rw-r--r--   0        0        0      354 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/clock-10-b2753250.js
--rw-r--r--   0        0        0      355 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/clock-11-7db4033d.js
--rw-r--r--   0        0        0      349 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/clock-12-07ebbfa6.js
--rw-r--r--   0        0        0      354 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/clock-2-2857fa45.js
--rw-r--r--   0        0        0      356 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/clock-3-d8e33794.js
--rw-r--r--   0        0        0      354 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/clock-4-ca107a0e.js
--rw-r--r--   0        0        0      356 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/clock-5-d3688e5d.js
--rw-r--r--   0        0        0      356 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/clock-6-21971acd.js
--rw-r--r--   0        0        0      355 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/clock-7-8462485f.js
--rw-r--r--   0        0        0      353 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/clock-8-d741e03a.js
--rw-r--r--   0        0        0      355 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/clock-9-9599372b.js
--rw-r--r--   0        0        0      353 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/clock-dc8bdde4.js
--rw-r--r--   0        0        0      335 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/cloud-83e7cbdf.js
--rw-r--r--   0        0        0      740 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/cloud-cog-d9e48864.js
--rw-r--r--   0        0        0      567 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/cloud-drizzle-e9ee8e3d.js
--rw-r--r--   0        0        0      417 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/cloud-fog-377e768a.js
--rw-r--r--   0        0        0      570 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/cloud-hail-551a6ea9.js
--rw-r--r--   0        0        0      394 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/cloud-lightning-c8d1996b.js
--rw-r--r--   0        0        0      416 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/cloud-moon-d7511f0d.js
--rw-r--r--   0        0        0      515 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/cloud-moon-rain-381e8468.js
--rw-r--r--   0        0        0      477 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/cloud-off-063a4c1d.js
--rw-r--r--   0        0        0      454 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/cloud-rain-338791c2.js
--rw-r--r--   0        0        0      465 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/cloud-rain-wind-03e07aa2.js
--rw-r--r--   0        0        0      576 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/cloud-snow-ad1d7740.js
--rw-r--r--   0        0        0      565 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/cloud-sun-630cbe71.js
--rw-r--r--   0        0        0      641 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/cloud-sun-rain-5249c398.js
--rw-r--r--   0        0        0      419 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/cloudy-000fba20.js
--rw-r--r--   0        0        0      594 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/clover-77915ed9.js
--rw-r--r--   0        0        0      407 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/club-6ad5de20.js
--rw-r--r--   0        0        0      412 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/code-square-044e4cc2.js
--rw-r--r--   0        0        0      568 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/codepen-b2e8542d.js
--rw-r--r--   0        0        0      726 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/codesandbox-7efd711a.js
--rw-r--r--   0        0        0      538 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/coffee-05730958.js
--rw-r--r--   0        0        0      885 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/cog-25bd7786.js
--rw-r--r--   0        0        0      454 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/coins-bd1bf521.js
--rw-r--r--   0        0        0      361 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/columns-2-01e62843.js
--rw-r--r--   0        0        0      397 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/columns-3-711daf33.js
--rw-r--r--   0        0        0      438 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/columns-4-224e3e26.js
--rw-r--r--   0        0        0      518 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/component-a81ab53e.js
--rw-r--r--   0        0        0      462 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/computer-71fd4536.js
--rw-r--r--   0        0        0      458 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/concierge-bell-86061895.js
--rw-r--r--   0        0        0      384 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/cone-2d5ac659.js
--rw-r--r--   0        0        0      593 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/construction-fe67f2d9.js
--rw-r--r--   0        0        0      527 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/contact-2-c389498e.js
--rw-r--r--   0        0        0      542 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/contact-b9c1f247.js
--rw-r--r--   0        0        0      622 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/container-8047bd33.js
--rw-r--r--   0        0        0      361 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/contrast-2db415fc.js
--rw-r--r--   0        0        0      534 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/cookie-5ac97459.js
--rw-r--r--   0        0        0      510 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/cooking-pot-60655687.js
--rw-r--r--   0        0        0      459 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/copy-check-0db8f346.js
--rw-r--r--   0        0        0      472 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/copy-minus-f4c2e84a.js
--rw-r--r--   0        0        0      527 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/copy-plus-cfb7c23a.js
--rw-r--r--   0        0        0      472 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/copy-slash-f93a0eba.js
--rw-r--r--   0        0        0      524 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/copy-x-4bc29fe8.js
--rw-r--r--   0        0        0      364 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/copyleft-f7bf8939.js
--rw-r--r--   0        0        0      361 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/copyright-8f6bee9b.js
--rw-r--r--   0        0        0      368 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/corner-down-left-529b9628.js
--rw-r--r--   0        0        0      372 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/corner-down-right-5a00b340.js
--rw-r--r--   0        0        0      370 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/corner-left-down-a945b7bb.js
--rw-r--r--   0        0        0      366 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/corner-left-up-f7b7a6ea.js
--rw-r--r--   0        0        0      372 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/corner-right-down-a24df1a7.js
--rw-r--r--   0        0        0      367 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/corner-right-up-8a587911.js
--rw-r--r--   0        0        0      366 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/corner-up-left-2edcaa13.js
--rw-r--r--   0        0        0      370 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/corner-up-right-bb4d22df.js
--rw-r--r--   0        0        0      506 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/creative-commons-8a08b5bb.js
--rw-r--r--   0        0        0      381 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/credit-card-29c50219.js
--rw-r--r--   0        0        0      745 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/croissant-cf14f255.js
--rw-r--r--   0        0        0      360 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/crop-ec2de7ad.js
--rw-r--r--   0        0        0      430 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/cross-c73155d1.js
--rw-r--r--   0        0        0      528 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/crosshair-797727d3.js
--rw-r--r--   0        0        0      326 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/crown-b10e7ff6.js
--rw-r--r--   0        0        0      551 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/cuboid-e2b6b17f.js
--rw-r--r--   0        0        0      495 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/cup-soda-cd8a0720.js
--rw-r--r--   0        0        0      522 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/currency-2f95ffaa.js
--rw-r--r--   0        0        0      367 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/cylinder-acebbe66.js
--rw-r--r--   0        0        0      607 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/database-backup-7e289bb9.js
--rw-r--r--   0        0        0      513 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/database-zap-b120cb34.js
--rw-r--r--   0        0        0      514 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/dessert-0e61f7af.js
--rw-r--r--   0        0        0      529 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/diameter-29b4aa9b.js
--rw-r--r--   0        0        0      419 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/diamond-a71b67ce.js
--rw-r--r--   0        0        0      367 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/dice-1-1d647002.js
--rw-r--r--   0        0        0      404 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/dice-2-ba43ec95.js
--rw-r--r--   0        0        0      443 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/dice-3-eeb10f84.js
--rw-r--r--   0        0        0      480 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/dice-4-4ab3610f.js
--rw-r--r--   0        0        0      519 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/dice-5-1fa08684.js
--rw-r--r--   0        0        0      557 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/dice-6-40a50ff1.js
--rw-r--r--   0        0        0      581 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/dices-13083691.js
--rw-r--r--   0        0        0      365 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/diff-6d4999f0.js
--rw-r--r--   0        0        0      386 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/disc-2-eeb76b3f.js
--rw-r--r--   0        0        0      457 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/disc-3-b8279770.js
--rw-r--r--   0        0        0      346 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/disc-608769ee.js
--rw-r--r--   0        0        0      407 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/disc-album-dc82f5be.js
--rw-r--r--   0        0        0      401 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/divide-0e9b398c.js
--rw-r--r--   0        0        0      476 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/divide-circle-8fd6d6fb.js
--rw-r--r--   0        0        0      500 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/divide-square-6a5043a0.js
--rw-r--r--   0        0        0      781 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/dna-6fa418fc.js
--rw-r--r--   0        0        0      821 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/dna-off-a86c6e71.js
--rw-r--r--   0        0        0      893 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/dog-0ed15e9a.js
--rw-r--r--   0        0        0      393 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/dollar-sign-b3fb7040.js
--rw-r--r--   0        0        0      419 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/donut-926b37ba.js
--rw-r--r--   0        0        0      406 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/door-closed-f6bdacff.js
--rw-r--r--   0        0        0      543 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/door-open-caf41777.js
--rw-r--r--   0        0        0      373 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/dot-square-5ee42a15.js
--rw-r--r--   0        0        0      508 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/drafting-compass-14926d84.js
--rw-r--r--   0        0        0      733 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/drama-2aa25a7f.js
--rw-r--r--   0        0        0      509 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/dribbble-426e96f1.js
--rw-r--r--   0        0        0      683 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/drill-3ab18849.js
--rw-r--r--   0        0        0      382 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/droplet-cde68b77.js
--rw-r--r--   0        0        0      548 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/droplets-a565eb54.js
--rw-r--r--   0        0        0      557 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/drum-0881aa6e.js
--rw-r--r--   0        0        0      602 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/drumstick-42cc5c3b.js
--rw-r--r--   0        0        0      530 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/dumbbell-d91d8011.js
--rw-r--r--   0        0        0      408 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/ear-8195764e.js
--rw-r--r--   0        0        0      614 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/ear-off-ca41fa4a.js
--rw-r--r--   0        0        0      351 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/eclipse-d34d29e1.js
--rw-r--r--   0        0        0      387 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/egg-355b27ab.js
--rw-r--r--   0        0        0      466 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/egg-fried-1a418806.js
--rw-r--r--   0        0        0      571 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/egg-off-15482582.js
--rw-r--r--   0        0        0      363 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/equal-8d7334c3.js
--rw-r--r--   0        0        0      420 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/equal-not-f15b9cc9.js
--rw-r--r--   0        0        0      401 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/equal-square-baf2c6cd.js
--rw-r--r--   0        0        0      435 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/euro-1ec53874.js
--rw-r--r--   0        0        0      481 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/expand-6c17c5ce.js
--rw-r--r--   0        0        0      352 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/facebook-7dbfefb3.js
--rw-r--r--   0        0        0      479 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/factory-278a980e.js
--rw-r--r--   0        0        0      502 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/fan-57bb5046.js
--rw-r--r--   0        0        0      376 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/fast-forward-f4dd1b1f.js
--rw-r--r--   0        0        0      444 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/feather-10711528.js
--rw-r--r--   0        0        0      617 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/fence-ee593734.js
--rw-r--r--   0        0        0      643 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/ferris-wheel-38cf8098.js
--rw-r--r--   0        0        0      646 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/figma-7ce64fda.js
--rw-r--r--   0        0        0      550 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/file-archive-16a981ce.js
--rw-r--r--   0        0        0      505 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/file-audio-05e886ea.js
--rw-r--r--   0        0        0      535 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/file-audio-2-eba1bafe.js
--rw-r--r--   0        0        0      475 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/file-axis-3d-0081c1ce.js
--rw-r--r--   0        0        0      504 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/file-badge-2-f715aaa5.js
--rw-r--r--   0        0        0      506 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/file-badge-58a2164c.js
--rw-r--r--   0        0        0      515 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/file-bar-chart-2-df4f1ba6.js
--rw-r--r--   0        0        0      514 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/file-bar-chart-7528c81d.js
--rw-r--r--   0        0        0      655 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/file-box-ade74692.js
--rw-r--r--   0        0        0      430 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/file-check-2-51a06c3e.js
--rw-r--r--   0        0        0      440 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/file-check-45bb29d8.js
--rw-r--r--   0        0        0      471 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/file-code-2-da69ff0e.js
--rw-r--r--   0        0        0      483 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/file-code-738bb7e0.js
--rw-r--r--   0        0        0      750 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/file-cog-92ab8d32.js
--rw-r--r--   0        0        0      454 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/file-diff-2674d100.js
--rw-r--r--   0        0        0      528 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/file-digit-d190a761.js
--rw-r--r--   0        0        0      598 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/file-heart-0e4c6049.js
--rw-r--r--   0        0        0      522 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/file-image-ce046320.js
--rw-r--r--   0        0        0      466 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/file-input-f082e6a0.js
--rw-r--r--   0        0        0      577 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/file-json-2-e5f3b51f.js
--rw-r--r--   0        0        0      589 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/file-json-bdae09ef.js
--rw-r--r--   0        0        0      514 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/file-key-2-b0bc49ac.js
--rw-r--r--   0        0        0      474 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/file-key-6c16592b.js
--rw-r--r--   0        0        0      454 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/file-line-chart-289e0070.js
--rw-r--r--   0        0        0      463 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/file-lock-06488db3.js
--rw-r--r--   0        0        0      505 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/file-lock-2-193473d8.js
--rw-r--r--   0        0        0      434 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/file-minus-1944d693.js
--rw-r--r--   0        0        0      424 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/file-minus-2-2b193278.js
--rw-r--r--   0        0        0      480 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/file-music-0cd1a5a5.js
--rw-r--r--   0        0        0      539 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/file-output-ec885816.js
--rw-r--r--   0        0        0      454 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/file-pen-36c525e2.js
--rw-r--r--   0        0        0      453 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/file-pen-line-d43bdcf1.js
--rw-r--r--   0        0        0      504 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/file-pie-chart-2d4ace9b.js
--rw-r--r--   0        0        0      459 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/file-plus-2-adae4d0c.js
--rw-r--r--   0        0        0      471 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/file-plus-43206f76.js
--rw-r--r--   0        0        0      489 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/file-question-b70f12a6.js
--rw-r--r--   0        0        0      583 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/file-scan-6d6f6d71.js
--rw-r--r--   0        0        0      550 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/file-spreadsheet-43a79f96.js
--rw-r--r--   0        0        0      546 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/file-stack-e4b74c5a.js
--rw-r--r--   0        0        0      464 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/file-symlink-21eb812d.js
--rw-r--r--   0        0        0      480 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/file-terminal-19347e68.js
--rw-r--r--   0        0        0      512 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/file-type-c9cab45d.js
--rw-r--r--   0        0        0      506 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/file-video-2-36068464.js
--rw-r--r--   0        0        0      445 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/file-video-844f909b.js
--rw-r--r--   0        0        0      486 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/file-volume-075f703a.js
--rw-r--r--   0        0        0      544 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/file-volume-2-c5616849.js
--rw-r--r--   0        0        0      423 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/file-warning-b060c4bf.js
--rw-r--r--   0        0        0      464 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/file-x-2-89dcea18.js
--rw-r--r--   0        0        0      479 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/file-x-cec4ad05.js
--rw-r--r--   0        0        0      461 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/files-871f2c83.js
--rw-r--r--   0        0        0      582 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/film-d24eb5d6.js
--rw-r--r--   0        0        0      336 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/filter-9fa6eb33.js
--rw-r--r--   0        0        0      402 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/filter-x-f7669990.js
--rw-r--r--   0        0        0      813 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/fingerprint-d9b62aff.js
--rw-r--r--   0        0        0      581 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/fire-extinguisher-5bccd8e3.js
--rw-r--r--   0        0        0      791 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/fish-f12e8325.js
--rw-r--r--   0        0        0      835 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/fish-off-a19b2443.js
--rw-r--r--   0        0        0      318 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/fish-symbol-499225bb.js
--rw-r--r--   0        0        0      394 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/flag-51df24ff.js
--rw-r--r--   0        0        0      453 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/flag-off-5ac8a8ef.js
--rw-r--r--   0        0        0      312 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/flag-triangle-left-861dad2d.js
--rw-r--r--   0        0        0      313 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/flag-triangle-right-43e19b0e.js
--rw-r--r--   0        0        0      453 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/flame-0df71fcf.js
--rw-r--r--   0        0        0      474 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/flame-kindling-c943242a.js
--rw-r--r--   0        0        0      470 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/flashlight-f560f5d8.js
--rw-r--r--   0        0        0      506 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/flashlight-off-7ff00ae2.js
--rw-r--r--   0        0        0      573 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/flask-conical-off-e88dcc6f.js
--rw-r--r--   0        0        0      474 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/flask-round-7fac9eed.js
--rw-r--r--   0        0        0      498 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/flip-horizontal-2-1ec31095.js
--rw-r--r--   0        0        0      548 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/flip-horizontal-40d9ef22.js
--rw-r--r--   0        0        0      503 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/flip-vertical-2-a95edc44.js
--rw-r--r--   0        0        0      549 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/flip-vertical-57017fb6.js
--rw-r--r--   0        0        0      617 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/flower-2-b71a7369.js
--rw-r--r--   0        0        0      657 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/flower-7e27e620.js
--rw-r--r--   0        0        0      513 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/focus-119a2d2c.js
--rw-r--r--   0        0        0      568 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/fold-horizontal-e86e541d.js
--rw-r--r--   0        0        0      570 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/fold-vertical-b2f86633.js
--rw-r--r--   0        0        0      542 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/folder-archive-0867c658.js
--rw-r--r--   0        0        0      450 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/folder-check-327b635b.js
--rw-r--r--   0        0        0      474 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/folder-clock-761d3b7d.js
--rw-r--r--   0        0        0      446 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/folder-closed-675100c8.js
--rw-r--r--   0        0        0      796 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/folder-cog-147353aa.js
--rw-r--r--   0        0        0      453 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/folder-dot-148fa737.js
--rw-r--r--   0        0        0      487 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/folder-down-b77e4f98.js
--rw-r--r--   0        0        0      536 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/folder-git-2-179844c9.js
--rw-r--r--   0        0        0      527 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/folder-git-c020630f.js
--rw-r--r--   0        0        0      556 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/folder-heart-9f9ea4b3.js
--rw-r--r--   0        0        0      488 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/folder-input-d1719b76.js
--rw-r--r--   0        0        0      523 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/folder-kanban-a3dfd68e.js
--rw-r--r--   0        0        0      521 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/folder-key-c4cc0892.js
--rw-r--r--   0        0        0      514 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/folder-lock-9187bd0c.js
--rw-r--r--   0        0        0      444 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/folder-minus-f1a446f6.js
--rw-r--r--   0        0        0      466 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/folder-open-554eb0ff.js
--rw-r--r--   0        0        0      519 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/folder-open-dot-bd887495.js
--rw-r--r--   0        0        0      490 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/folder-output-ce643418.js
--rw-r--r--   0        0        0      461 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/folder-pen-d7c61ca8.js
--rw-r--r--   0        0        0      491 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/folder-root-27e94b32.js
--rw-r--r--   0        0        0      509 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/folder-search-2-eaa41b51.js
--rw-r--r--   0        0        0      488 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/folder-search-52dccfbd.js
--rw-r--r--   0        0        0      469 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/folder-symlink-f5605327.js
--rw-r--r--   0        0        0      598 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/folder-sync-b7d69c14.js
--rw-r--r--   0        0        0      653 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/folder-tree-16c062ce.js
--rw-r--r--   0        0        0      484 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/folder-up-99d5573f.js
--rw-r--r--   0        0        0      489 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/folder-x-34790d57.js
--rw-r--r--   0        0        0      458 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/folders-59e58057.js
--rw-r--r--   0        0        0      624 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/footprints-64b0ead1.js
--rw-r--r--   0        0        0      474 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/forklift-6f97c2a0.js
--rw-r--r--   0        0        0      471 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/frame-cff826dc.js
--rw-r--r--   0        0        0      327 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/framer-19128747.js
--rw-r--r--   0        0        0      470 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/frown-175ce156.js
--rw-r--r--   0        0        0      544 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/fuel-f21d2bfd.js
--rw-r--r--   0        0        0      535 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/fullscreen-7d7817b8.js
--rw-r--r--   0        0        0      448 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/function-square-daa63af8.js
--rw-r--r--   0        0        0      405 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/gallery-horizontal-cfc06fe2.js
--rw-r--r--   0        0        0      409 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/gallery-horizontal-end-17370a66.js
--rw-r--r--   0        0        0      479 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/gallery-thumbnails-a81776ef.js
--rw-r--r--   0        0        0      404 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/gallery-vertical-68378ca2.js
--rw-r--r--   0        0        0      406 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/gallery-vertical-end-2398dac0.js
--rw-r--r--   0        0        0      795 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/gamepad-2-3ae0b330.js
--rw-r--r--   0        0        0      549 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/gamepad-23b3ad90.js
--rw-r--r--   0        0        0      369 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/gantt-chart-532e7888.js
--rw-r--r--   0        0        0      440 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/gantt-chart-square-75cc145f.js
--rw-r--r--   0        0        0      351 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/gauge-46e81e98.js
--rw-r--r--   0        0        0      411 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/gauge-circle-d58f500a.js
--rw-r--r--   0        0        0      476 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/gavel-b589a715.js
--rw-r--r--   0        0        0      392 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/gem-6bb7bddc.js
--rw-r--r--   0        0        0      437 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/ghost-63f26d11.js
--rw-r--r--   0        0        0      449 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/git-branch-de689845.js
--rw-r--r--   0        0        0      427 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/git-commit-horizontal-a44390ce.js
--rw-r--r--   0        0        0      388 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/git-commit-vertical-69c30a57.js
--rw-r--r--   0        0        0      549 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/git-compare-arrows-81eff26e.js
--rw-r--r--   0        0        0      459 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/git-compare-ea80db52.js
--rw-r--r--   0        0        0      517 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/git-graph-7ba52a21.js
--rw-r--r--   0        0        0      397 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/git-merge-f2b8f827.js
--rw-r--r--   0        0        0      462 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/git-pull-request-980e4e95.js
--rw-r--r--   0        0        0      493 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/git-pull-request-arrow-6ca9574a.js
--rw-r--r--   0        0        0      516 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/git-pull-request-closed-a14928c4.js
--rw-r--r--   0        0        0      479 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/git-pull-request-create-6e51ec23.js
--rw-r--r--   0        0        0      526 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/git-pull-request-create-arrow-08b3e525.js
--rw-r--r--   0        0        0      489 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/git-pull-request-draft-a4f3ca06.js
--rw-r--r--   0        0        0      550 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/gitlab-1d3a66c3.js
--rw-r--r--   0        0        0      418 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/glass-water-5a687e2b.js
--rw-r--r--   0        0        0      527 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/glasses-7fe19bf9.js
--rw-r--r--   0        0        0      579 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/globe-2-47d02662.js
--rw-r--r--   0        0        0      410 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/goal-cf06f6c3.js
--rw-r--r--   0        0        0      631 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/grab-70e64ba1.js
--rw-r--r--   0        0        0      506 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/graduation-cap-a0715b8d.js
--rw-r--r--   0        0        0      714 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/grape-332f120a.js
--rw-r--r--   0        0        0      397 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/grid-2x2-38118c1d.js
--rw-r--r--   0        0        0      469 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/grid-3x3-09e797d0.js
--rw-r--r--   0        0        0      675 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/grip-c338a35d.js
--rw-r--r--   0        0        0      542 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/grip-horizontal-c47cb1ba.js
--rw-r--r--   0        0        0      540 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/grip-vertical-da29db8f.js
--rw-r--r--   0        0        0      681 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/guitar-2d10606f.js
--rw-r--r--   0        0        0      584 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/hand-coins-7d87aee4.js
--rw-r--r--   0        0        0      589 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/hand-d08db668.js
--rw-r--r--   0        0        0      622 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/hand-heart-f341c0c6.js
--rw-r--r--   0        0        0      496 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/hand-helping-4102a64b.js
--rw-r--r--   0        0        0      570 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/hand-metal-4c03951f.js
--rw-r--r--   0        0        0      605 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/hand-platter-bda84c9f.js
--rw-r--r--   0        0        0      621 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/handshake-a314c225.js
--rw-r--r--   0        0        0      565 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/hard-drive-2d00eab4.js
--rw-r--r--   0        0        0      486 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/hard-drive-download-773c154d.js
--rw-r--r--   0        0        0      485 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/hard-drive-upload-b3197ca7.js
--rw-r--r--   0        0        0      532 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/hard-hat-4e174197.js
--rw-r--r--   0        0        0      471 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/hash-8bc8412e.js
--rw-r--r--   0        0        0      579 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/haze-b45745fb.js
--rw-r--r--   0        0        0      406 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/hdmi-port-ca77cf7b.js
--rw-r--r--   0        0        0      408 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/heading-1-9cbc51f4.js
--rw-r--r--   0        0        0      433 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/heading-2-66c68aa3.js
--rw-r--r--   0        0        0      508 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/heading-3-f0c7eb2b.js
--rw-r--r--   0        0        0      443 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/heading-4-5badafef.js
--rw-r--r--   0        0        0      500 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/heading-5-a83f7a41.js
--rw-r--r--   0        0        0      465 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/heading-6-a058a407.js
--rw-r--r--   0        0        0      367 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/heading-aa580ea0.js
--rw-r--r--   0        0        0      412 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/headphones-a21f3c90.js
--rw-r--r--   0        0        0      473 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/headset-ff8ed4da.js
--rw-r--r--   0        0        0      471 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/heart-crack-8c09cad2.js
--rw-r--r--   0        0        0      639 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/heart-handshake-bcbba2ba.js
--rw-r--r--   0        0        0      539 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/heart-off-43722eb5.js
--rw-r--r--   0        0        0      494 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/heart-pulse-2080697b.js
--rw-r--r--   0        0        0      712 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/heater-af5de4da.js
--rw-r--r--   0        0        0      407 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/hexagon-3757803a.js
--rw-r--r--   0        0        0      396 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/highlighter-916684f7.js
--rw-r--r--   0        0        0      412 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/history-de3bca16.js
--rw-r--r--   0        0        0      924 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/hop-d889a2a4.js
--rw-r--r--   0        0        0      877 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/hop-off-53ebd056.js
--rw-r--r--   0        0        0      712 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/hotel-397a190d.js
--rw-r--r--   0        0        0      535 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/hourglass-d50bf166.js
--rw-r--r--   0        0        0      485 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/ice-cream-2-71d211f6.js
--rw-r--r--   0        0        0      438 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/ice-cream-b7cf0f87.js
--rw-r--r--   0        0        0      444 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/image-321ba4a1.js
--rw-r--r--   0        0        0      549 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/image-down-f9f50798.js
--rw-r--r--   0        0        0      515 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/image-minus-a2c5accd.js
--rw-r--r--   0        0        0      645 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/image-off-67dff800.js
--rw-r--r--   0        0        0      568 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/image-plus-81549658.js
--rw-r--r--   0        0        0      499 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/images-c4d00c01.js
--rw-r--r--   0        0        0      437 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/import-14f0b3bd.js
--rw-r--r--   0        0        0      461 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/inbox-d74663f7.js
--rw-r--r--   0        0        0      473 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/indent-c40b16d9.js
--rw-r--r--   0        0        0  9622377 2024-05-24 01:15:20.773085 langflow_base-0.0.48/langflow/frontend/assets/index-5d2e85d2.js
--rw-r--r--   0        0        0   550845 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/index-b5c02d80.css
--rw-r--r--   0        0        0      465 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/indian-rupee-344cad03.js
--rw-r--r--   0        0        0      384 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/infinity-dcf96e9e.js
--rw-r--r--   0        0        0      483 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/inspection-panel-fabca1ee.js
--rw-r--r--   0        0        0      471 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/instagram-825f9cb0.js
--rw-r--r--   0        0        0      419 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/italic-83cd5d13.js
--rw-r--r--   0        0        0      391 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/iteration-ccw-8185a0f1.js
--rw-r--r--   0        0        0      385 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/iteration-cw-092806c0.js
--rw-r--r--   0        0        0      396 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/japanese-yen-8363e75d.js
--rw-r--r--   0        0        0      476 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/joystick-92227220.js
--rw-r--r--   0        0        0      365 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/kanban-f40521f4.js
--rw-r--r--   0        0        0      435 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/kanban-square-28d851ef.js
--rw-r--r--   0        0        0      855 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/kanban-square-dashed-011cd9c5.js
--rw-r--r--   0        0        0      413 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/key-round-4eff9d32.js
--rw-r--r--   0        0        0      513 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/key-square-7b7c4744.js
--rw-r--r--   0        0        0      624 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/keyboard-music-216e0129.js
--rw-r--r--   0        0        0      410 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/lamp-03453946.js
--rw-r--r--   0        0        0      398 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/lamp-ceiling-ea75860a.js
--rw-r--r--   0        0        0      478 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/lamp-desk-ca20ffd0.js
--rw-r--r--   0        0        0      378 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/lamp-floor-22ec2b4e.js
--rw-r--r--   0        0        0      433 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/lamp-wall-down-8a7bc680.js
--rw-r--r--   0        0        0      432 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/lamp-wall-up-0f22083b.js
--rw-r--r--   0        0        0      522 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/land-plot-fbcf7d50.js
--rw-r--r--   0        0        0      582 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/landmark-c8fd19f9.js
--rw-r--r--   0        0        0      491 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/languages-7db159c1.js
--rw-r--r--   0        0        0      393 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/laptop-c2115f06.js
--rw-r--r--   0        0        0      477 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/lasso-f1509c13.js
--rw-r--r--   0        0        0      717 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/lasso-select-e5441e2c.js
--rw-r--r--   0        0        0      483 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/laugh-fb84eb9f.js
--rw-r--r--   0        0        0      507 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/layers-2-79243e40.js
--rw-r--r--   0        0        0      645 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/layers-3-fa210f21.js
--rw-r--r--   0        0        0      525 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/layout-dashboard-20091918.js
--rw-r--r--   0        0        0      520 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/layout-grid-a5dbe99b.js
--rw-r--r--   0        0        0      535 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/layout-list-281c03bd.js
--rw-r--r--   0        0        0      460 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/layout-panel-left-7c72ff94.js
--rw-r--r--   0        0        0      460 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/layout-panel-top-2b5e6a8c.js
--rw-r--r--   0        0        0      460 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/layout-template-fc16389d.js
--rw-r--r--   0        0        0      440 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/leaf-a45ed6c5.js
--rw-r--r--   0        0        0      615 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/leafy-green-12a9e7f1.js
--rw-r--r--   0        0        0      405 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/library-b6a25ede.js
--rw-r--r--   0        0        0      495 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/library-big-5e395cde.js
--rw-r--r--   0        0        0      441 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/library-square-2b5951f3.js
--rw-r--r--   0        0        0      555 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/life-buoy-9b302c13.js
--rw-r--r--   0        0        0      476 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/ligature-192d4243.js
--rw-r--r--   0        0        0      461 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/lightbulb-a9367c75.js
--rw-r--r--   0        0        0      531 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/lightbulb-off-a9572065.js
--rw-r--r--   0        0        0      344 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/line-chart-cd1a1275.js
--rw-r--r--   0        0        0      416 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/link-2-dd51ce36.js
--rw-r--r--   0        0        0      467 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/link-2-off-63f7485d.js
--rw-r--r--   0        0        0      469 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/linkedin-55211952.js
--rw-r--r--   0        0        0      586 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/list-6c4583fe.js
--rw-r--r--   0        0        0      453 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/list-checks-fd98d460.js
--rw-r--r--   0        0        0      468 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/list-collapse-2f1fb453.js
--rw-r--r--   0        0        0      464 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/list-end-ffe50314.js
--rw-r--r--   0        0        0      370 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/list-filter-44feb044.js
--rw-r--r--   0        0        0      407 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/list-minus-e3e6e4e8.js
--rw-r--r--   0        0        0      480 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/list-music-66d7a7e0.js
--rw-r--r--   0        0        0      559 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/list-ordered-f67a586a.js
--rw-r--r--   0        0        0      442 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/list-plus-e0555946.js
--rw-r--r--   0        0        0      511 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/list-restart-144e0982.js
--rw-r--r--   0        0        0      465 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/list-start-b96debc3.js
--rw-r--r--   0        0        0      474 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/list-todo-e01d08d1.js
--rw-r--r--   0        0        0      473 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/list-tree-e1447981.js
--rw-r--r--   0        0        0      416 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/list-video-1f29121a.js
--rw-r--r--   0        0        0      443 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/list-x-3bc9ea77.js
--rw-r--r--   0        0        0      740 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/loader-6788a7f7.js
--rw-r--r--   0        0        0      524 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/locate-7eee1a99.js
--rw-r--r--   0        0        0      577 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/locate-fixed-bc0164df.js
--rw-r--r--   0        0        0      741 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/locate-off-6d1017b1.js
--rw-r--r--   0        0        0      429 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/lock-keyhole-f04c19b7.js
--rw-r--r--   0        0        0      433 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/log-out-0039b468.js
--rw-r--r--   0        0        0      427 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/lollipop-df11836a.js
--rw-r--r--   0        0        0      560 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/luggage-5d91149b.js
--rw-r--r--   0        0        0      369 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/m-square-cee2edee.js
--rw-r--r--   0        0        0      448 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/magnet-a7a74a3d.js
--rw-r--r--   0        0        0      390 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/mail-590d97fd.js
--rw-r--r--   0        0        0      458 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/mail-check-52828765.js
--rw-r--r--   0        0        0      452 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/mail-minus-1be29beb.js
--rw-r--r--   0        0        0      463 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/mail-open-7df531dc.js
--rw-r--r--   0        0        0      488 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/mail-plus-07ec6f2e.js
--rw-r--r--   0        0        0      564 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/mail-question-3e638ddf.js
--rw-r--r--   0        0        0      577 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/mail-search-69d0fb92.js
--rw-r--r--   0        0        0      498 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/mail-warning-670b68fc.js
--rw-r--r--   0        0        0      489 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/mail-x-5752ee92.js
--rw-r--r--   0        0        0      539 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/mailbox-476dc431.js
--rw-r--r--   0        0        0      441 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/mails-34626a1b.js
--rw-r--r--   0        0        0    23161 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/male-technologist-d2e7de57.png
--rw-r--r--   0        0        0      437 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/map-ce4788ee.js
--rw-r--r--   0        0        0      374 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/map-pin-56b57fa7.js
--rw-r--r--   0        0        0      667 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/map-pin-off-f46c49f4.js
--rw-r--r--   0        0        0      525 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/map-pinned-b0ef6f9d.js
--rw-r--r--   0        0        0      374 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/martini-a7add61d.js
--rw-r--r--   0        0        0      468 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/maximize-a28fc4f1.js
--rw-r--r--   0        0        0      610 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/medal-ae183bc6.js
--rw-r--r--   0        0        0      367 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/megaphone-97084f20.js
--rw-r--r--   0        0        0      480 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/megaphone-off-6b6f915d.js
--rw-r--r--   0        0        0      469 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/meh-35cd2b47.js
--rw-r--r--   0        0        0      702 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/memory-stick-a95af896.js
--rw-r--r--   0        0        0      436 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/menu-square-31663887.js
--rw-r--r--   0        0        0      401 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/merge-8e297d56.js
--rw-r--r--   0        0        0      412 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/message-circle-code-99a33b12.js
--rw-r--r--   0        0        0      783 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/message-circle-dashed-c3eb173d.js
--rw-r--r--   0        0        0      460 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/message-circle-heart-d79043df.js
--rw-r--r--   0        0        0      442 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/message-circle-more-6ef47832.js
--rw-r--r--   0        0        0      453 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/message-circle-off-4e169269.js
--rw-r--r--   0        0        0      398 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/message-circle-plus-81b3ef29.js
--rw-r--r--   0        0        0      434 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/message-circle-question-38ea5e6e.js
--rw-r--r--   0        0        0      422 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/message-circle-reply-9497c6e7.js
--rw-r--r--   0        0        0      404 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/message-circle-warning-9bb87a42.js
--rw-r--r--   0        0        0      398 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/message-circle-x-7d481ce0.js
--rw-r--r--   0        0        0      441 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/message-square-code-1836bd4c.js
--rw-r--r--   0        0        0      612 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/message-square-dashed-63e862cd.js
--rw-r--r--   0        0        0      463 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/message-square-diff-ca6ae959.js
--rw-r--r--   0        0        0      394 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/message-square-dot-f624eebe.js
--rw-r--r--   0        0        0      486 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/message-square-heart-68e54d86.js
--rw-r--r--   0        0        0      423 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/message-square-off-272fdc98.js
--rw-r--r--   0        0        0      429 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/message-square-plus-45a0e0e9.js
--rw-r--r--   0        0        0      464 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/message-square-quote-7ff17009.js
--rw-r--r--   0        0        0      454 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/message-square-reply-b562c939.js
--rw-r--r--   0        0        0      420 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/message-square-share-0964723f.js
--rw-r--r--   0        0        0      430 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/message-square-text-99a6beef.js
--rw-r--r--   0        0        0      435 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/message-square-warning-25b96994.js
--rw-r--r--   0        0        0      437 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/message-square-x-a221e210.js
--rw-r--r--   0        0        0      372 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/mic-2-861745e6.js
--rw-r--r--   0        0        0      445 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/mic-e53d992d.js
--rw-r--r--   0        0        0      597 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/mic-off-c97851d9.js
--rw-r--r--   0        0        0      559 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/microscope-4c5e2ae8.js
--rw-r--r--   0        0        0      497 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/microwave-f789cec7.js
--rw-r--r--   0        0        0      413 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/milestone-6ad4c0c4.js
--rw-r--r--   0        0        0      547 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/milk-17837e5c.js
--rw-r--r--   0        0        0      607 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/milk-off-c72c2c04.js
--rw-r--r--   0        0        0      468 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/minimize-c8e8ec56.js
--rw-r--r--   0        0        0      341 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/minus-circle-862dbf5a.js
--rw-r--r--   0        0        0      363 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/minus-square-6fd45698.js
--rw-r--r--   0        0        0      434 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/monitor-a2d354bb.js
--rw-r--r--   0        0        0      443 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/monitor-check-162a522c.js
--rw-r--r--   0        0        0      465 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/monitor-dot-85c6e2b2.js
--rw-r--r--   0        0        0      480 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/monitor-down-b8f60ac2.js
--rw-r--r--   0        0        0      492 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/monitor-off-3288386e.js
--rw-r--r--   0        0        0      475 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/monitor-pause-728f3bb5.js
--rw-r--r--   0        0        0      443 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/monitor-play-d1bfa54a.js
--rw-r--r--   0        0        0      500 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/monitor-smartphone-a0dca1ea.js
--rw-r--r--   0        0        0      522 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/monitor-speaker-fbdd7793.js
--rw-r--r--   0        0        0      457 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/monitor-stop-0610c2df.js
--rw-r--r--   0        0        0      477 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/monitor-up-37964c1c.js
--rw-r--r--   0        0        0      482 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/monitor-x-11e18515.js
--rw-r--r--   0        0        0      394 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/moon-star-49802d11.js
--rw-r--r--   0        0        0      400 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/more-vertical-7169056a.js
--rw-r--r--   0        0        0      311 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/mountain-c7b18206.js
--rw-r--r--   0        0        0      408 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/mountain-snow-d3a63c6f.js
--rw-r--r--   0        0        0      357 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/mouse-5a3723fd.js
--rw-r--r--   0        0        0      370 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/mouse-pointer-1d56851e.js
--rw-r--r--   0        0        0      324 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/mouse-pointer-2-0788cd23.js
--rw-r--r--   0        0        0      486 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/mouse-pointer-click-3edb0cdb.js
--rw-r--r--   0        0        0      686 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/mouse-pointer-square-dashed-2d247999.js
--rw-r--r--   0        0        0      409 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/mouse-pointer-square-eb41a313.js
--rw-r--r--   0        0        0      574 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/move-300bf01c.js
--rw-r--r--   0        0        0      417 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/move-3d-1ae965a3.js
--rw-r--r--   0        0        0      423 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/move-diagonal-2-c4423577.js
--rw-r--r--   0        0        0      422 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/move-diagonal-6735637c.js
--rw-r--r--   0        0        0      341 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/move-down-7c02d5ab.js
--rw-r--r--   0        0        0      341 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/move-down-left-ebf3a155.js
--rw-r--r--   0        0        0      343 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/move-down-right-0cc7a6b9.js
--rw-r--r--   0        0        0      424 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/move-horizontal-7a028148.js
--rw-r--r--   0        0        0      338 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/move-left-2136c3cd.js
--rw-r--r--   0        0        0      342 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/move-right-1c98b70f.js
--rw-r--r--   0        0        0      336 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/move-up-e91955fa.js
--rw-r--r--   0        0        0      338 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/move-up-left-bfce2b05.js
--rw-r--r--   0        0        0      340 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/move-up-right-f530e63a.js
--rw-r--r--   0        0        0      422 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/move-vertical-b6e59403.js
--rw-r--r--   0        0        0      389 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/music-0ba88ffb.js
--rw-r--r--   0        0        0      339 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/music-2-c7f1f6f0.js
--rw-r--r--   0        0        0      336 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/music-3-472bf62b.js
--rw-r--r--   0        0        0      428 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/music-4-d77235d5.js
--rw-r--r--   0        0        0      324 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/navigation-2-0fbbbc5b.js
--rw-r--r--   0        0        0      436 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/navigation-2-off-3e75af4c.js
--rw-r--r--   0        0        0      323 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/navigation-37e1a560.js
--rw-r--r--   0        0        0      436 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/navigation-off-8aba9e41.js
--rw-r--r--   0        0        0      517 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/newspaper-c5cbe283.js
--rw-r--r--   0        0        0      503 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/nfc-ba38f74c.js
--rw-r--r--   0        0        0      504 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/notebook-df9ab14b.js
--rw-r--r--   0        0        0      569 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/notebook-pen-2cb4fcf8.js
--rw-r--r--   0        0        0      618 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/notebook-tabs-57108f6c.js
--rw-r--r--   0        0        0      586 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/notebook-text-90d14136.js
--rw-r--r--   0        0        0      542 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/notepad-text-a6008a7b.js
--rw-r--r--   0        0        0      804 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/notepad-text-dashed-c8d9e1e3.js
--rw-r--r--   0        0        0      769 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/nut-302b4fc7.js
--rw-r--r--   0        0        0      880 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/nut-off-416c230b.js
--rw-r--r--   0        0        0      364 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/octagon-3e428e17.js
--rw-r--r--   0        0        0      334 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/option-20d51683.js
--rw-r--r--   0        0        0      519 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/orbit-73963e9d.js
--rw-r--r--   0        0        0      474 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/outdent-865d48e2.js
--rw-r--r--   0        0        0      534 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/package-5282c64c.js
--rw-r--r--   0        0        0      600 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/package-check-f94596d2.js
--rw-r--r--   0        0        0      594 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/package-minus-87f97424.js
--rw-r--r--   0        0        0      791 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/package-open-50313ee6.js
--rw-r--r--   0        0        0      630 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/package-plus-4ec37a35.js
--rw-r--r--   0        0        0      659 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/package-search-1587ffd9.js
--rw-r--r--   0        0        0      601 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/package-x-d81f8c09.js
--rw-r--r--   0        0        0      514 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/paint-bucket-93cba5af.js
--rw-r--r--   0        0        0      478 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/paint-roller-fa4a2150.js
--rw-r--r--   0        0        0      473 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/paintbrush-2-fbc3d15f.js
--rw-r--r--   0        0        0      516 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/paintbrush-c5238598.js
--rw-r--r--   0        0        0      638 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/palmtree-7355f6bb.js
--rw-r--r--   0        0        0      364 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/panel-bottom-6d01fe7b.js
--rw-r--r--   0        0        0      411 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/panel-bottom-close-fa3dda93.js
--rw-r--r--   0        0        0      479 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/panel-bottom-dashed-65f8850c.js
--rw-r--r--   0        0        0      410 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/panel-bottom-open-c8f7d3ef.js
--rw-r--r--   0        0        0      361 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/panel-left-bbd543d0.js
--rw-r--r--   0        0        0      409 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/panel-left-close-95e4a3f1.js
--rw-r--r--   0        0        0      473 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/panel-left-dashed-f8f8ba05.js
--rw-r--r--   0        0        0      407 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/panel-left-open-0e676308.js
--rw-r--r--   0        0        0      363 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/panel-right-b4499943.js
--rw-r--r--   0        0        0      409 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/panel-right-close-f7eb8bf1.js
--rw-r--r--   0        0        0      478 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/panel-right-dashed-742b9247.js
--rw-r--r--   0        0        0      410 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/panel-right-open-ae48eb72.js
--rw-r--r--   0        0        0      407 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/panel-top-close-cfabbad6.js
--rw-r--r--   0        0        0      472 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/panel-top-dashed-a8420167.js
--rw-r--r--   0        0        0      360 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/panel-top-f1784e7f.js
--rw-r--r--   0        0        0      407 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/panel-top-open-95b0eb41.js
--rw-r--r--   0        0        0      405 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/panels-left-bottom-5f188146.js
--rw-r--r--   0        0        0      407 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/panels-right-bottom-05cb76ad.js
--rw-r--r--   0        0        0      401 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/panels-top-left-a1b25954.js
--rw-r--r--   0        0        0      362 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/parentheses-37577a43.js
--rw-r--r--   0        0        0      361 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/parking-circle-860c3779.js
--rw-r--r--   0        0        0      447 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/parking-circle-off-5ae4d1ee.js
--rw-r--r--   0        0        0      528 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/parking-meter-c3c52a07.js
--rw-r--r--   0        0        0      383 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/parking-square-8b953717.js
--rw-r--r--   0        0        0      544 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/parking-square-off-740bd731.js
--rw-r--r--   0        0        0      910 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/party-popper-7f352c5a.js
--rw-r--r--   0        0        0      372 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/pause-a3997290.js
--rw-r--r--   0        0        0      420 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/pause-circle-384a7e9b.js
--rw-r--r--   0        0        0      434 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/pause-octagon-dff2ebfd.js
--rw-r--r--   0        0        0      516 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/paw-print-0e3aa68a.js
--rw-r--r--   0        0        0      432 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/pc-case-61dbb122.js
--rw-r--r--   0        0        0      330 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/pen-140cfa46.js
--rw-r--r--   0        0        0      367 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/pen-line-7acae35e.js
--rw-r--r--   0        0        0      469 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/pen-tool-7441bdca.js
--rw-r--r--   0        0        0      658 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/pencil-ruler-c7daf67c.js
--rw-r--r--   0        0        0      417 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/pentagon-2dbf9f1c.js
--rw-r--r--   0        0        0      412 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/percent-0a1b4c20.js
--rw-r--r--   0        0        0      426 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/percent-circle-6706e13b.js
--rw-r--r--   0        0        0      551 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/percent-diamond-a221c97d.js
--rw-r--r--   0        0        0      443 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/percent-square-9a60c93e.js
--rw-r--r--   0        0        0      431 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/person-standing-12605d7a.js
--rw-r--r--   0        0        0      569 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/phone-bb7af3a3.js
--rw-r--r--   0        0        0      680 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/phone-call-a324d52a.js
--rw-r--r--   0        0        0      685 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/phone-forwarded-7416bc2f.js
--rw-r--r--   0        0        0      683 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/phone-incoming-45414c5f.js
--rw-r--r--   0        0        0      683 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/phone-missed-46ce970c.js
--rw-r--r--   0        0        0      650 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/phone-off-ef820972.js
--rw-r--r--   0        0        0      683 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/phone-outgoing-eb5faee5.js
--rw-r--r--   0        0        0      411 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/pi-0aab49e5.js
--rw-r--r--   0        0        0      448 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/pi-square-bfda5f59.js
--rw-r--r--   0        0        0      575 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/piano-3e58cbd0.js
--rw-r--r--   0        0        0      419 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/picture-in-picture-2-532321a7.js
--rw-r--r--   0        0        0      431 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/picture-in-picture-5275251a.js
--rw-r--r--   0        0        0      374 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/pie-chart-9ae16dd2.js
--rw-r--r--   0        0        0      495 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/piggy-bank-9c3bf720.js
--rw-r--r--   0        0        0      390 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/pilcrow-a1b42cf7.js
--rw-r--r--   0        0        0      463 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/pilcrow-square-d08b2930.js
--rw-r--r--   0        0        0      388 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/pill-b5e5eb65.js
--rw-r--r--   0        0        0      516 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/pin-off-7ff30ecb.js
--rw-r--r--   0        0        0      463 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/pipette-1e962b9f.js
--rw-r--r--   0        0        0      501 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/pizza-f0deed1d.js
--rw-r--r--   0        0        0      476 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/plane-facec1e0.js
--rw-r--r--   0        0        0      583 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/plane-landing-91d10c06.js
--rw-r--r--   0        0        0      574 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/plane-takeoff-e3daa27f.js
--rw-r--r--   0        0        0      362 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/play-circle-0a458909.js
--rw-r--r--   0        0        0      368 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/play-square-d8f3e7a3.js
--rw-r--r--   0        0        0      458 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/plug-2-3aeb006f.js
--rw-r--r--   0        0        0      433 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/plug-4bf1d0a9.js
--rw-r--r--   0        0        0      495 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/plug-zap-2-31808c4f.js
--rw-r--r--   0        0        0      527 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/plug-zap-d1efc20e.js
--rw-r--r--   0        0        0      414 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/pocket-64314cbf.js
--rw-r--r--   0        0        0      504 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/podcast-5ee672fb.js
--rw-r--r--   0        0        0      642 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/pointer-6a99de81.js
--rw-r--r--   0        0        0      663 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/pointer-off-9f315d62.js
--rw-r--r--   0        0        0      552 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/popcorn-e646c986.js
--rw-r--r--   0        0        0      411 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/popsicle-62c081c9.js
--rw-r--r--   0        0        0      428 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/pound-sterling-98b56e6d.js
--rw-r--r--   0        0        0      348 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/power-c0b8eb1b.js
--rw-r--r--   0        0        0      419 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/power-circle-973e2e2e.js
--rw-r--r--   0        0        0      453 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/power-off-60f0489a.js
--rw-r--r--   0        0        0      435 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/power-square-f3b9df9c.js
--rw-r--r--   0        0        0      409 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/presentation-8a30976f.js
--rw-r--r--   0        0        0      474 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/printer-01182271.js
--rw-r--r--   0        0        0      562 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/projector-ea7a2ed4.js
--rw-r--r--   0        0        0     1135 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/puzzle-e8df0c53.js
--rw-r--r--   0        0        0      433 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/pyramid-42f3c2bc.js
--rw-r--r--   0        0        0      824 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/qr-code-92db79b5.js
--rw-r--r--   0        0        0      574 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/quote-ebbe955b.js
--rw-r--r--   0        0        0      616 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/rabbit-ea3ddd8c.js
--rw-r--r--   0        0        0      677 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/radar-74ff71f7.js
--rw-r--r--   0        0        0      722 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/radiation-28ac3311.js
--rw-r--r--   0        0        0      304 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/radical-df83abe8.js
--rw-r--r--   0        0        0      539 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/radio-e0db86d7.js
--rw-r--r--   0        0        0      438 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/radio-receiver-241ac64e.js
--rw-r--r--   0        0        0      628 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/radio-tower-4dcbd4de.js
--rw-r--r--   0        0        0      461 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/radius-4ad64aba.js
--rw-r--r--   0        0        0      380 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/rail-symbol-6a1e3180.js
--rw-r--r--   0        0        0      406 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/rainbow-f431fd74.js
--rw-r--r--   0        0        0      687 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/rat-59bc794f.js
--rw-r--r--   0        0        0      387 2024-05-24 01:15:20.741084 langflow_base-0.0.48/langflow/frontend/assets/ratio-56551707.js
--rw-r--r--   0        0        0      467 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/receipt-04f5c566.js
--rw-r--r--   0        0        0      452 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/receipt-cent-fdbff390.js
--rw-r--r--   0        0        0      449 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/receipt-euro-2ff548fd.js
--rw-r--r--   0        0        0      497 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/receipt-indian-rupee-107c9f2e.js
--rw-r--r--   0        0        0      520 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/receipt-japanese-yen-27196c83.js
--rw-r--r--   0        0        0      499 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/receipt-pound-sterling-6a851018.js
--rw-r--r--   0        0        0      461 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/receipt-russian-ruble-0c3bd056.js
--rw-r--r--   0        0        0      479 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/receipt-swiss-franc-0af66aaf.js
--rw-r--r--   0        0        0      471 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/receipt-text-d52c16dc.js
--rw-r--r--   0        0        0      335 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/rectangle-horizontal-d5e41423.js
--rw-r--r--   0        0        0      333 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/rectangle-vertical-ef76eb26.js
--rw-r--r--   0        0        0      757 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/recycle-cea96532.js
--rw-r--r--   0        0        0      383 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/redo-2-6b57c1db.js
--rw-r--r--   0        0        0      414 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/redo-dot-acc69b3c.js
--rw-r--r--   0        0        0      501 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/refresh-ccw-dot-2abbe1d7.js
--rw-r--r--   0        0        0      495 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/refresh-cw-ded069ad.js
--rw-r--r--   0        0        0      675 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/refresh-cw-off-26c765c7.js
--rw-r--r--   0        0        0      434 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/refrigerator-bbba713d.js
--rw-r--r--   0        0        0      485 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/regex-5f11ac98.js
--rw-r--r--   0        0        0      459 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/remove-formatting-9056e1f7.js
--rw-r--r--   0        0        0      487 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/repeat-1-209d375c.js
--rw-r--r--   0        0        0      447 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/repeat-2-226af233.js
--rw-r--r--   0        0        0      751 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/replace-all-3afafbb1.js
--rw-r--r--   0        0        0      614 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/replace-f610ab8f.js
--rw-r--r--   0        0        0      360 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/reply-04203a0a.js
--rw-r--r--   0        0        0      416 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/reply-all-2f95773e.js
--rw-r--r--   0        0        0      373 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/rewind-0dcda923.js
--rw-r--r--   0        0        0      731 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/ribbon-30f6b81f.js
--rw-r--r--   0        0        0    26806 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/robot-95e1b00d.png
--rw-r--r--   0        0        0      627 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/rocket-dd64364a.js
--rw-r--r--   0        0        0      498 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/rocking-chair-48b0d67c.js
--rw-r--r--   0        0        0      579 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/roller-coaster-07467718.js
--rw-r--r--   0        0        0      575 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/rotate-3d-123855e5.js
--rw-r--r--   0        0        0      374 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/rotate-ccw-fa2e4815.js
--rw-r--r--   0        0        0      375 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/rotate-cw-fb2b4c62.js
--rw-r--r--   0        0        0      424 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/route-51350f1b.js
--rw-r--r--   0        0        0      607 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/route-off-9b0cd50f.js
--rw-r--r--   0        0        0      554 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/router-7d73f15e.js
--rw-r--r--   0        0        0      358 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/rows-2-db495965.js
--rw-r--r--   0        0        0      394 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/rows-3-4bd8ea33.js
--rw-r--r--   0        0        0      435 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/rows-4-d3b56076.js
--rw-r--r--   0        0        0      399 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/rss-a86acff1.js
--rw-r--r--   0        0        0      573 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/ruler-7f425ff8.js
--rw-r--r--   0        0        0      353 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/russian-ruble-4335329e.js
--rw-r--r--   0        0        0      413 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/sailboat-9791d947.js
--rw-r--r--   0        0        0      651 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/salad-d5faeb52.js
--rw-r--r--   0        0        0      585 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/sandwich-6f29208b.js
--rw-r--r--   0        0        0      485 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/satellite-d14d025e.js
--rw-r--r--   0        0        0      459 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/satellite-dish-b270ce57.js
--rw-r--r--   0        0        0      423 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/scale-3d-c328b763.js
--rw-r--r--   0        0        0      543 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/scale-f896884c.js
--rw-r--r--   0        0        0      461 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/scaling-699b61b2.js
--rw-r--r--   0        0        0      464 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/scan-5cd4dfc4.js
--rw-r--r--   0        0        0      581 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/scan-barcode-566f4c1e.js
--rw-r--r--   0        0        0      585 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/scan-eye-2473d111.js
--rw-r--r--   0        0        0      595 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/scan-face-6b16b2e0.js
--rw-r--r--   0        0        0      505 2024-05-24 01:15:20.737084 langflow_base-0.0.48/langflow/frontend/assets/scan-line-43fa2ecd.js
--rw-r--r--   0        0        0      561 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/scan-search-6abfbd41.js
--rw-r--r--   0        0        0      576 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/scan-text-ee620dce.js
--rw-r--r--   0        0        0      657 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/scatter-chart-b0552128.js
--rw-r--r--   0        0        0      615 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/school-2-665376f7.js
--rw-r--r--   0        0        0      544 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/school-3f78e0ab.js
--rw-r--r--   0        0        0      570 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/scissors-line-dashed-aad245e8.js
--rw-r--r--   0        0        0      556 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/scissors-square-75252291.js
--rw-r--r--   0        0        0      680 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/scissors-square-dashed-bottom-1c99d312.js
--rw-r--r--   0        0        0      500 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/screen-share-off-2bb3e9c2.js
--rw-r--r--   0        0        0      402 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/scroll-2b74946d.js
--rw-r--r--   0        0        0      394 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/search-check-29a560b5.js
--rw-r--r--   0        0        0      435 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/search-code-60e5e292.js
--rw-r--r--   0        0        0      394 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/search-slash-e352dd58.js
--rw-r--r--   0        0        0      431 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/search-x-b5e3d1c0.js
--rw-r--r--   0        0        0      348 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/send-horizontal-ded44ff0.js
--rw-r--r--   0        0        0      494 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/send-to-back-c538e5c7.js
--rw-r--r--   0        0        0      429 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/separator-horizontal-22e03055.js
--rw-r--r--   0        0        0      427 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/separator-vertical-fb23f93d.js
--rw-r--r--   0        0        0      513 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/server-22d39749.js
--rw-r--r--   0        0        0      943 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/server-cog-4f664742.js
--rw-r--r--   0        0        0      586 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/server-crash-2de8d911.js
--rw-r--r--   0        0        0      621 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/server-off-e5302d6b.js
--rw-r--r--   0        0        0      900 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/settings-2c5eb85f.js
--rw-r--r--   0        0        0      492 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/shapes-ab5f60f5.js
--rw-r--r--   0        0        0      544 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/sheet-c18d33b2.js
--rw-r--r--   0        0        0      413 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/shell-7041f088.js
--rw-r--r--   0        0        0      407 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/shield-alert-da301322.js
--rw-r--r--   0        0        0      369 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/shield-ban-2f837fc2.js
--rw-r--r--   0        0        0      374 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/shield-check-57d729e9.js
--rw-r--r--   0        0        0      451 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/shield-ellipsis-1e4d47da.js
--rw-r--r--   0        0        0      368 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/shield-half-7f9034e6.js
--rw-r--r--   0        0        0      368 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/shield-minus-746917fc.js
--rw-r--r--   0        0        0      452 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/shield-off-d0097f34.js
--rw-r--r--   0        0        0      403 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/shield-plus-bd844eb0.js
--rw-r--r--   0        0        0      438 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/shield-question-acee1538.js
--rw-r--r--   0        0        0      407 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/shield-x-20fc7c07.js
--rw-r--r--   0        0        0      625 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/ship-34376655.js
--rw-r--r--   0        0        0      693 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/ship-wheel-5f798c44.js
--rw-r--r--   0        0        0      461 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/shirt-40d6c417.js
--rw-r--r--   0        0        0      425 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/shopping-bag-e264cfb5.js
--rw-r--r--   0        0        0      584 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/shopping-basket-c496e3a3.js
--rw-r--r--   0        0        0      461 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/shopping-cart-f7972bbc.js
--rw-r--r--   0        0        0      445 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/shovel-87b6429e.js
--rw-r--r--   0        0        0      671 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/shower-head-9234f682.js
--rw-r--r--   0        0        0      479 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/shrink-a509776b.js
--rw-r--r--   0        0        0      435 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/shrub-d5b1732e.js
--rw-r--r--   0        0        0      559 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/shuffle-5a3cdb9d.js
--rw-r--r--   0        0        0      307 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/sigma-2e2eac32.js
--rw-r--r--   0        0        0      382 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/sigma-square-f9086730.js
--rw-r--r--   0        0        0      443 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/signal-e03f8a6e.js
--rw-r--r--   0        0        0      410 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/signal-high-3b71f87f.js
--rw-r--r--   0        0        0      334 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/signal-low-5b3d6a00.js
--rw-r--r--   0        0        0      375 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/signal-medium-77c8eec6.js
--rw-r--r--   0        0        0      298 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/signal-zero-a696bbd6.js
--rw-r--r--   0        0        0      444 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/signpost-big-d6bb07d1.js
--rw-r--r--   0        0        0      395 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/signpost-c43dd41b.js
--rw-r--r--   0        0        0      638 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/siren-594aae1f.js
--rw-r--r--   0        0        0      368 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/skip-back-3fe1b4df.js
--rw-r--r--   0        0        0      371 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/skip-forward-1242d364.js
--rw-r--r--   0        0        0      524 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/skull-f042a7bf.js
--rw-r--r--   0        0        0      779 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/slack-422f1b25.js
--rw-r--r--   0        0        0      294 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/slash-be35eeb1.js
--rw-r--r--   0        0        0      381 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/slash-square-288167ac.js
--rw-r--r--   0        0        0      379 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/slice-c3dad828.js
--rw-r--r--   0        0        0      372 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/smartphone-868cca7d.js
--rw-r--r--   0        0        0      396 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/smartphone-charging-4f1bc8af.js
--rw-r--r--   0        0        0      520 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/smartphone-nfc-f363c1ef.js
--rw-r--r--   0        0        0      468 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/smile-00a26bc9.js
--rw-r--r--   0        0        0      549 2024-05-24 01:15:20.749085 langflow_base-0.0.48/langflow/frontend/assets/smile-plus-5f6ed569.js
--rw-r--r--   0        0        0      537 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/snail-da9a7766.js
--rw-r--r--   0        0        0      537 2024-05-24 01:15:20.753085 langflow_base-0.0.48/langflow/frontend/assets/sofa-2bfdf61c.js
--rw-r--r--   0        0        0      703 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/soup-f6cf262a.js
--rw-r--r--   0        0        0      321 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/space-798958e5.js
--rw-r--r--   0        0        0      454 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/spade-0bbb1aa1.js
--rw-r--r--   0        0        0      430 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/sparkle-3d5760b9.js
--rw-r--r--   0        0        0      448 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/speaker-f7945326.js
--rw-r--r--   0        0        0      534 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/speech-caef5ead.js
--rw-r--r--   0        0        0      495 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/spell-check-2-e0aa4126.js
--rw-r--r--   0        0        0      383 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/spell-check-f166dc68.js
--rw-r--r--   0        0        0      396 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/spline-694d7ddd.js
--rw-r--r--   0        0        0      434 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/split-94678a76.js
--rw-r--r--   0        0        0      457 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/split-square-horizontal-62846c6f.js
--rw-r--r--   0        0        0      455 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/split-square-vertical-d7b1a293.js
--rw-r--r--   0        0        0      698 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/spray-can-d7810702.js
--rw-r--r--   0        0        0      576 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/sprout-2941b7af.js
--rw-r--r--   0        0        0      439 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/square-dashed-bottom-84130080.js
--rw-r--r--   0        0        0      529 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/square-dashed-bottom-code-778cf01d.js
--rw-r--r--   0        0        0      375 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/square-radical-c6519b19.js
--rw-r--r--   0        0        0      490 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/square-stack-b7c58a9d.js
--rw-r--r--   0        0        0      443 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/square-user-caa0b22f.js
--rw-r--r--   0        0        0      429 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/square-user-round-6041baba.js
--rw-r--r--   0        0        0      334 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/squircle-869daa19.js
--rw-r--r--   0        0        0      583 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/squirrel-1f8d0f35.js
--rw-r--r--   0        0        0      540 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/stamp-59355141.js
--rw-r--r--   0        0        0      385 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/star-5ad6ab78.js
--rw-r--r--   0        0        0      324 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/star-half-dd116c9e.js
--rw-r--r--   0        0        0      473 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/star-off-54f225a7.js
--rw-r--r--   0        0        0      365 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/step-back-96bf0f8a.js
--rw-r--r--   0        0        0      367 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/step-forward-304ebcdc.js
--rw-r--r--   0        0        0      513 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/stethoscope-1fa99fa8.js
--rw-r--r--   0        0        0      538 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/sticker-144df895.js
--rw-r--r--   0        0        0      399 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/sticky-note-2858bd4c.js
--rw-r--r--   0        0        0      361 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/stop-circle-682b4316.js
--rw-r--r--   0        0        0      398 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/stretch-horizontal-deaacaf3.js
--rw-r--r--   0        0        0      396 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/stretch-vertical-d3f10b13.js
--rw-r--r--   0        0        0      422 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/strikethrough-72878769.js
--rw-r--r--   0        0        0      477 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/subscript-91dc6b5f.js
--rw-r--r--   0        0        0      642 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/sun-dim-24f43cd5.js
--rw-r--r--   0        0        0      655 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/sun-medium-820ad250.js
--rw-r--r--   0        0        0      654 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/sun-moon-690f2196.js
--rw-r--r--   0        0        0      699 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/sun-snow-5e3f18c5.js
--rw-r--r--   0        0        0      594 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/sunrise-65a8ae93.js
--rw-r--r--   0        0        0      594 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/sunset-51bf7930.js
--rw-r--r--   0        0        0      491 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/superscript-96f8b76d.js
--rw-r--r--   0        0        0      563 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/swatch-book-217377ae.js
--rw-r--r--   0        0        0      373 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/swiss-franc-f2b395c5.js
--rw-r--r--   0        0        0      533 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/switch-camera-be80e3cf.js
--rw-r--r--   0        0        0      492 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/sword-90806a62.js
--rw-r--r--   0        0        0      725 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/swords-bdda5651.js
--rw-r--r--   0        0        0      536 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/syringe-530e6026.js
--rw-r--r--   0        0        0      390 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/table-2-aa8e71c1.js
--rw-r--r--   0        0        0      431 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/table-963e7daa.js
--rw-r--r--   0        0        0      441 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/table-properties-b2fc3d31.js
--rw-r--r--   0        0        0      388 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/tablet-0916dc26.js
--rw-r--r--   0        0        0      456 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/tablet-smartphone-8833648a.js
--rw-r--r--   0        0        0      439 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/tablets-d1f9646c.js
--rw-r--r--   0        0        0      501 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/tag-5ad49284.js
--rw-r--r--   0        0        0      567 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/tags-be256b31.js
--rw-r--r--   0        0        0      292 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/tally-1-b05cc2f6.js
--rw-r--r--   0        0        0      328 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/tally-2-209b0771.js
--rw-r--r--   0        0        0      365 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/tally-3-f335e9a6.js
--rw-r--r--   0        0        0      402 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/tally-4-5aafa5e8.js
--rw-r--r--   0        0        0      441 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/tally-5-a07599d2.js
--rw-r--r--   0        0        0      463 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/tangent-f5131226.js
--rw-r--r--   0        0        0      396 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/target-bbc4af84.js
--rw-r--r--   0        0        0      791 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/telescope-f24b3ac3.js
--rw-r--r--   0        0        0      424 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/tent-720ee227.js
--rw-r--r--   0        0        0      546 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/tent-tree-48eb1ffa.js
--rw-r--r--   0        0        0      431 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/test-tube-2-e828197b.js
--rw-r--r--   0        0        0      425 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/test-tube-5c9f0b52.js
--rw-r--r--   0        0        0      575 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/test-tubes-e92b4851.js
--rw-r--r--   0        0        0      370 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/text-20bd10b2.js
--rw-r--r--   0        0        0      434 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/text-cursor-d575e4f0.js
--rw-r--r--   0        0        0      405 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/text-quote-114106c0.js
--rw-r--r--   0        0        0      903 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/text-select-4cd99566.js
--rw-r--r--   0        0        0      703 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/theater-a353a219.js
--rw-r--r--   0        0        0      332 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/thermometer-e6c688d9.js
--rw-r--r--   0        0        0      543 2024-05-24 01:15:20.761085 langflow_base-0.0.48/langflow/frontend/assets/thermometer-snowflake-be8d8d4e.js
--rw-r--r--   0        0        0      552 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/thermometer-sun-94d72684.js
--rw-r--r--   0        0        0      478 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/thumbs-down-21e22cbc.js
--rw-r--r--   0        0        0      478 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/thumbs-up-b0327fee.js
--rw-r--r--   0        0        0      496 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/ticket-59ef6fa6.js
--rw-r--r--   0        0        0      433 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/ticket-check-a63070c9.js
--rw-r--r--   0        0        0      427 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/ticket-minus-b5a8f3d3.js
--rw-r--r--   0        0        0      507 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/ticket-percent-d1fb44a4.js
--rw-r--r--   0        0        0      462 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/ticket-plus-0b02434c.js
--rw-r--r--   0        0        0      433 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/ticket-slash-c5c920d6.js
--rw-r--r--   0        0        0      470 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/ticket-x-277ff8f5.js
--rw-r--r--   0        0        0      413 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/timer-63ef82c8.js
--rw-r--r--   0        0        0      515 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/timer-off-ebfa1a04.js
--rw-r--r--   0        0        0      443 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/timer-reset-7ff7158f.js
--rw-r--r--   0        0        0      380 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/toggle-left-23160936.js
--rw-r--r--   0        0        0      382 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/toggle-right-fb2a1fb6.js
--rw-r--r--   0        0        0      441 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/tornado-ecbdd395.js
--rw-r--r--   0        0        0      374 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/torus-959c03a5.js
--rw-r--r--   0        0        0      399 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/touchpad-6c8f5159.js
--rw-r--r--   0        0        0      534 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/touchpad-off-14143303.js
--rw-r--r--   0        0        0      581 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/tower-control-d0da130d.js
--rw-r--r--   0        0        0      662 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/tractor-f0adfa2a.js
--rw-r--r--   0        0        0      661 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/traffic-cone-62187088.js
--rw-r--r--   0        0        0      557 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/train-front-bd9494d4.js
--rw-r--r--   0        0        0      622 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/train-front-tunnel-4cd69150.js
--rw-r--r--   0        0        0      527 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/train-track-5fdf782c.js
--rw-r--r--   0        0        0      548 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/tram-front-b7bd0d07.js
--rw-r--r--   0        0        0      420 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/trash-548efc8e.js
--rw-r--r--   0        0        0      436 2024-05-24 01:15:20.745085 langflow_base-0.0.48/langflow/frontend/assets/tree-deciduous-3f8b1290.js
--rw-r--r--   0        0        0      483 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/tree-pine-2b427a6d.js
--rw-r--r--   0        0        0      546 2024-05-24 01:15:20.757085 langflow_base-0.0.48/langflow/frontend/assets/trees-7698e8a4.js
--rw-r--r--   0        0        0      444 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/trello-3ccdab69.js
--rw-r--r--   0        0        0      382 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/trending-down-c9533d32.js
--rw-r--r--   0        0        0      379 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/trending-up-071757ce.js
--rw-r--r--   0        0        0      354 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/triangle-dc6903e2.js
--rw-r--r--   0        0        0      364 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/triangle-right-023a2364.js
--rw-r--r--   0        0        0      640 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/trophy-2d75b216.js
--rw-r--r--   0        0        0      576 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/truck-c4b0a7fc.js
--rw-r--r--   0        0        0      532 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/turtle-b3106944.js
--rw-r--r--   0        0        0      356 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/tv-2-06e948fb.js
--rw-r--r--   0        0        0      376 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/tv-360b34eb.js
--rw-r--r--   0        0        0      321 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/twitch-7b6d926e.js
--rw-r--r--   0        0        0      421 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/twitter-06b12afe.js
--rw-r--r--   0        0        0      404 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/umbrella-35d823ca.js
--rw-r--r--   0        0        0      488 2024-05-24 01:15:20.717084 langflow_base-0.0.48/langflow/frontend/assets/umbrella-off-4a7736d2.js
--rw-r--r--   0        0        0      366 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/underline-a8d39a72.js
--rw-r--r--   0        0        0      384 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/undo-2-6ba370e2.js
--rw-r--r--   0        0        0      412 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/undo-dot-dfc9e5ce.js
--rw-r--r--   0        0        0     9608 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/undraw_blog_post_re_fy5x-de7369a0.svg
--rw-r--r--   0        0        0    10459 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/undraw_chat_bot_re_e2gj-eceb89b6.svg
--rw-r--r--   0        0        0    12395 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/undraw_cloud_docs_re_xjht-c1ec41f9.svg
--rw-r--r--   0        0        0    40053 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/undraw_real_time_analytics_re_yliv-25632bd9.svg
--rw-r--r--   0        0        0     5612 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/undraw_short_bio_re_fmx0-949a7b7d.svg
--rw-r--r--   0        0        0    11757 2024-05-24 01:15:20.713084 langflow_base-0.0.48/langflow/frontend/assets/undraw_transfer_files_re_a2a9-c499dfcb.svg
--rw-r--r--   0        0        0      569 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/unfold-horizontal-5cdb7854.js
--rw-r--r--   0        0        0      572 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/unfold-vertical-98fd63f5.js
--rw-r--r--   0        0        0      334 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/unlink-2-7b45e48d.js
--rw-r--r--   0        0        0      703 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/unlink-684a02e2.js
--rw-r--r--   0        0        0      382 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/unlock-a770e507.js
--rw-r--r--   0        0        0      433 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/unlock-keyhole-c96563d9.js
--rw-r--r--   0        0        0      426 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/upload-cloud-b724f6cf.js
--rw-r--r--   0        0        0      576 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/usb-4c542cb8.js
--rw-r--r--   0        0        0      428 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/user-check-2b998463.js
--rw-r--r--   0        0        0      757 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/user-cog-042a9c97.js
--rw-r--r--   0        0        0      430 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/user-minus-2b419d96.js
--rw-r--r--   0        0        0      484 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/user-plus-ef296d04.js
--rw-r--r--   0        0        0      351 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/user-round-9678c3f1.js
--rw-r--r--   0        0        0      407 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/user-round-check-333295c7.js
--rw-r--r--   0        0        0      459 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/user-round-search-bf215914.js
--rw-r--r--   0        0        0      438 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/user-round-x-b64b3a0a.js
--rw-r--r--   0        0        0      453 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/user-search-a44398cb.js
--rw-r--r--   0        0        0      480 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/user-x-c3cf35a7.js
--rw-r--r--   0        0        0      479 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/users-02903511.js
--rw-r--r--   0        0        0      439 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/utensils-60a15b68.js
--rw-r--r--   0        0        0      536 2024-05-24 01:15:20.729084 langflow_base-0.0.48/langflow/frontend/assets/utensils-crossed-8fc371ec.js
--rw-r--r--   0        0        0      517 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/utility-pole-9d58dfcf.js
--rw-r--r--   0        0        0      837 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/vault-038eee2a.js
--rw-r--r--   0        0        0      444 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/vegan-05798bd6.js
--rw-r--r--   0        0        0      514 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/venetian-mask-fe3f1aeb.js
--rw-r--r--   0        0        0      420 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/vibrate-667e7072.js
--rw-r--r--   0        0        0      546 2024-05-24 01:15:20.725084 langflow_base-0.0.48/langflow/frontend/assets/vibrate-off-0bdf0a78.js
--rw-r--r--   0        0        0      373 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/video-8f31a003.js
--rw-r--r--   0        0        0      472 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/video-off-b65e7039.js
--rw-r--r--   0        0        0      492 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/videotape-2374e735.js
--rw-r--r--   0        0        0      549 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/view-f9e42cb1.js
--rw-r--r--   0        0        0      404 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/voicemail-03d63f76.js
--rw-r--r--   0        0        0      384 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/volume-1-a8dcab50.js
--rw-r--r--   0        0        0      444 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/volume-2-51a7a1bb.js
--rw-r--r--   0        0        0      326 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/volume-fd2fd766.js
--rw-r--r--   0        0        0      437 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/volume-x-2cd7713a.js
--rw-r--r--   0        0        0      405 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/vote-1ee56c91.js
--rw-r--r--   0        0        0      425 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/wallet-1c10d16f.js
--rw-r--r--   0        0        0      398 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/wallet-2-eb5caf85.js
--rw-r--r--   0        0        0      502 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/wallet-cards-97bf1044.js
--rw-r--r--   0        0        0      510 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/wallpaper-78a97ca2.js
--rw-r--r--   0        0        0      604 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/wand-28efcf56.js
--rw-r--r--   0        0        0      535 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/warehouse-f82177ac.js
--rw-r--r--   0        0        0      522 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/washing-machine-c4d18bcb.js
--rw-r--r--   0        0        0      549 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/watch-4d03e446.js
--rw-r--r--   0        0        0      598 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/waves-c75c9971.js
--rw-r--r--   0        0        0      590 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/waypoints-4f37dfb8.js
--rw-r--r--   0        0        0     4310 2024-05-24 01:15:20.721084 langflow_base-0.0.48/langflow/frontend/assets/web-vitals-60d3425a.js
--rw-r--r--   0        0        0      422 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/webcam-8a307428.js
--rw-r--r--   0        0        0      527 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/webhook-9f58c70e.js
--rw-r--r--   0        0        0      653 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/webhook-off-d5460710.js
--rw-r--r--   0        0        0      435 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/weight-faa2a2c8.js
--rw-r--r--   0        0        0     1055 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/wheat-0b843377.js
--rw-r--r--   0        0        0     1103 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/wheat-off-a706bc18.js
--rw-r--r--   0        0        0      492 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/whole-word-6a795fdb.js
--rw-r--r--   0        0        0      455 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/wifi-46c5237a.js
--rw-r--r--   0        0        0      634 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/wifi-off-a80416b7.js
--rw-r--r--   0        0        0      427 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/wind-a90729e4.js
--rw-r--r--   0        0        0      458 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/wine-7b6ca8a2.js
--rw-r--r--   0        0        0      597 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/wine-off-9c00409f.js
--rw-r--r--   0        0        0      475 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/wrap-text-46766bc2.js
--rw-r--r--   0        0        0      437 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/wrench-e7dc10d8.js
--rw-r--r--   0        0        0      440 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/x-octagon-86f69d07.js
--rw-r--r--   0        0        0      405 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/x-square-174ee91e.js
--rw-r--r--   0        0        0      503 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/youtube-7e2b9bd8.js
--rw-r--r--   0        0        0      502 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/zap-off-10dadbae.js
--rw-r--r--   0        0        0      476 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/zoom-in-3fb13670.js
--rw-r--r--   0        0        0      422 2024-05-24 01:15:20.733085 langflow_base-0.0.48/langflow/frontend/assets/zoom-out-625141d6.js
--rw-r--r--   0        0        0   104187 2024-05-24 01:15:20.709084 langflow_base-0.0.48/langflow/frontend/favicon.ico
--rw-r--r--   0        0        0      660 2024-05-24 01:15:20.773085 langflow_base-0.0.48/langflow/frontend/index.html
--rw-r--r--   0        0        0      820 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/graph/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/graph/edge/__init__.py
--rw-r--r--   0        0        0     7245 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/graph/edge/base.py
--rw-r--r--   0        0        0      989 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/graph/edge/schema.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/graph/edge/utils.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/graph/graph/__init__.py
--rw-r--r--   0        0        0    56620 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/graph/graph/base.py
--rw-r--r--   0        0        0     2628 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/graph/graph/constants.py
--rw-r--r--   0        0        0     4649 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/graph/graph/runnable_vertices_manager.py
--rw-r--r--   0        0        0     1589 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/graph/graph/state_manager.py
--rw-r--r--   0        0        0     7111 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/graph/graph/utils.py
--rw-r--r--   0        0        0     1822 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/graph/schema.py
--rw-r--r--   0        0        0     1265 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/graph/utils.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/graph/vertex/__init__.py
--rw-r--r--   0        0        0    30797 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/graph/vertex/base.py
--rw-r--r--   0        0        0        1 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/graph/vertex/constants.py
--rw-r--r--   0        0        0    22124 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/graph/vertex/types.py
--rw-r--r--   0        0        0     4543 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/graph/vertex/utils.py
--rw-r--r--   0        0        0      103 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/helpers/__init__.py
--rw-r--r--   0        0        0     7078 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/helpers/flow.py
--rw-r--r--   0        0        0     1235 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/helpers/record.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/initial_setup/__init__.py
--rw-r--r--   0        0        0    10009 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/initial_setup/setup.py
--rw-r--r--   0        0        0    35485 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/initial_setup/starter_projects/Basic Prompting (Hello, world!).json
--rw-r--r--   0        0        0    43780 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/initial_setup/starter_projects/Langflow Blog Writter.json
--rw-r--r--   0        0        0    41729 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/initial_setup/starter_projects/Langflow Document QA.json
--rw-r--r--   0        0        0    52220 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/initial_setup/starter_projects/Langflow Memory Conversation.json
--rw-r--r--   0        0        0    74431 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/initial_setup/starter_projects/Langflow Prompt Chaining.json
--rw-r--r--   0        0        0   207599 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/initial_setup/starter_projects/VectorStore-RAG-Flows.json
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/interface/__init__.py
--rw-r--r--   0        0        0       84 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/interface/agents/__init__.py
--rw-r--r--   0        0        0     2483 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/interface/agents/base.py
--rw-r--r--   0        0        0     8875 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/interface/agents/custom.py
--rw-r--r--   0        0        0     1455 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/interface/agents/prebuilt.py
--rw-r--r--   0        0        0     4646 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/interface/base.py
--rw-r--r--   0        0        0       84 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/interface/chains/__init__.py
--rw-r--r--   0        0        0     3039 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/interface/chains/base.py
--rw-r--r--   0        0        0     4822 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/interface/chains/custom.py
--rw-r--r--   0        0        0      194 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/interface/custom/__init__.py
--rw-r--r--   0        0        0     1269 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/interface/custom/attributes.py
--rw-r--r--   0        0        0     1501 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/interface/custom/base.py
--rw-r--r--   0        0        0       62 2024-05-24 01:13:47.332054 langflow_base-0.0.48/langflow/interface/custom/code_parser/__init__.py
--rw-r--r--   0        0        0    13275 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/custom/code_parser/code_parser.py
--rw-r--r--   0        0        0     1394 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/custom/code_parser/utils.py
--rw-r--r--   0        0        0       77 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/custom/custom_component/__init__.py
--rw-r--r--   0        0        0     2908 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/custom/custom_component/component.py
--rw-r--r--   0        0        0    17310 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/custom/custom_component/custom_component.py
--rw-r--r--   0        0        0       77 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/custom/directory_reader/__init__.py
--rw-r--r--   0        0        0    11481 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/custom/directory_reader/directory_reader.py
--rw-r--r--   0        0        0     5587 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/custom/directory_reader/utils.py
--rw-r--r--   0        0        0      385 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/custom/eval.py
--rw-r--r--   0        0        0      723 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/custom/schema.py
--rw-r--r--   0        0        0    16603 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/custom/utils.py
--rw-r--r--   0        0        0     2303 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/custom_lists.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/document_loaders/__init__.py
--rw-r--r--   0        0        0     1571 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/document_loaders/base.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/embeddings/__init__.py
--rw-r--r--   0        0        0     1537 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/embeddings/base.py
--rw-r--r--   0        0        0       94 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/importing/__init__.py
--rw-r--r--   0        0        0     5374 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/importing/utils.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/initialize/__init__.py
--rw-r--r--   0        0        0      363 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/initialize/llm.py
--rw-r--r--   0        0        0    22567 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/initialize/loading.py
--rw-r--r--   0        0        0     4232 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/initialize/utils.py
--rw-r--r--   0        0        0     8548 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/initialize/vector_store.py
--rw-r--r--   0        0        0      747 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/listing.py
--rw-r--r--   0        0        0       78 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/llms/__init__.py
--rw-r--r--   0        0        0     1449 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/llms/base.py
--rw-r--r--   0        0        0       88 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/memories/__init__.py
--rw-r--r--   0        0        0     2290 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/memories/base.py
--rw-r--r--   0        0        0       87 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/prompts/__init__.py
--rw-r--r--   0        0        0     2556 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/prompts/base.py
--rw-r--r--   0        0        0     2448 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/prompts/custom.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/retrievers/__init__.py
--rw-r--r--   0        0        0     2238 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/retrievers/base.py
--rw-r--r--   0        0        0     1742 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/run.py
--rw-r--r--   0        0        0      106 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/text_splitters/__init__.py
--rw-r--r--   0        0        0     1542 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/text_splitters/base.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/toolkits/__init__.py
--rw-r--r--   0        0        0     2743 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/toolkits/base.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/toolkits/custom.py
--rw-r--r--   0        0        0       81 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/tools/__init__.py
--rw-r--r--   0        0        0     5808 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/tools/base.py
--rw-r--r--   0        0        0      849 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/tools/constants.py
--rw-r--r--   0        0        0     1266 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/tools/custom.py
--rw-r--r--   0        0        0     4165 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/tools/util.py
--rw-r--r--   0        0        0     2895 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/types.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/utilities/__init__.py
--rw-r--r--   0        0        0     2538 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/utilities/base.py
--rw-r--r--   0        0        0     6181 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/utils.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/vector_store/__init__.py
--rw-r--r--   0        0        0     1871 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/vector_store/base.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/wrappers/__init__.py
--rw-r--r--   0        0        0     1035 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/interface/wrappers/base.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/legacy_custom/__init__.py
--rw-r--r--   0        0        0     1648 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/legacy_custom/customs.py
--rw-r--r--   0        0        0       91 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/load.py
--rw-r--r--   0        0        0     5344 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/main.py
--rw-r--r--   0        0        0     5205 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/memory.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/processing/__init__.py
--rw-r--r--   0        0        0     3527 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/processing/base.py
--rw-r--r--   0        0        0     5170 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/processing/load.py
--rw-r--r--   0        0        0    11570 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/processing/process.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/py.typed
--rw-r--r--   0        0        0       89 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/schema/__init__.py
--rw-r--r--   0        0        0     2589 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/schema/dotdict.py
--rw-r--r--   0        0        0     1307 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/schema/graph.py
--rw-r--r--   0        0        0     6324 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/schema/schema.py
--rw-r--r--   0        0        0     1978 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/server.py
--rw-r--r--   0        0        0      115 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/services/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/services/auth/__init__.py
--rw-r--r--   0        0        0      327 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/services/auth/factory.py
--rw-r--r--   0        0        0      330 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/services/auth/service.py
--rw-r--r--   0        0        0    12091 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/services/auth/utils.py
--rw-r--r--   0        0        0      790 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/services/base.py
--rw-r--r--   0        0        0      284 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/services/cache/__init__.py
--rw-r--r--   0        0        0     4032 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/services/cache/base.py
--rw-r--r--   0        0        0     1561 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/services/cache/factory.py
--rw-r--r--   0        0        0    12992 2024-05-24 01:13:47.336054 langflow_base-0.0.48/langflow/services/cache/service.py
--rw-r--r--   0        0        0     4752 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/cache/utils.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/chat/__init__.py
--rw-r--r--   0        0        0     4562 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/chat/cache.py
--rw-r--r--   0        0        0       45 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/chat/config.py
--rw-r--r--   0        0        0      340 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/chat/factory.py
--rw-r--r--   0        0        0     1374 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/chat/service.py
--rw-r--r--   0        0        0     1794 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/chat/utils.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/database/__init__.py
--rw-r--r--   0        0        0      672 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/database/factory.py
--rw-r--r--   0        0        0      192 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/database/models/__init__.py
--rw-r--r--   0        0        0      146 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/database/models/api_key/__init__.py
--rw-r--r--   0        0        0     2589 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/database/models/api_key/crud.py
--rw-r--r--   0        0        0     1828 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/database/models/api_key/model.py
--rw-r--r--   0        0        0      760 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/database/models/base.py
--rw-r--r--   0        0        0      118 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/database/models/flow/__init__.py
--rw-r--r--   0        0        0     5306 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/database/models/flow/model.py
--rw-r--r--   0        0        0      134 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/database/models/folder/__init__.py
--rw-r--r--   0        0        0      138 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/database/models/folder/constants.py
--rw-r--r--   0        0        0     1750 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/database/models/folder/model.py
--rw-r--r--   0        0        0     1014 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/database/models/folder/utils.py
--rw-r--r--   0        0        0      137 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/database/models/user/__init__.py
--rw-r--r--   0        0        0     2044 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/database/models/user/crud.py
--rw-r--r--   0        0        0     2259 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/database/models/user/model.py
--rw-r--r--   0        0        0      150 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/database/models/variable/__init__.py
--rw-r--r--   0        0        0     2441 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/database/models/variable/model.py
--rw-r--r--   0        0        0    11304 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/database/service.py
--rw-r--r--   0        0        0     2643 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/database/utils.py
--rw-r--r--   0        0        0     6735 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/deps.py
--rw-r--r--   0        0        0     2955 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/factory.py
--rw-r--r--   0        0        0     5383 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/manager.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/monitor/__init__.py
--rw-r--r--   0        0        0      429 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/monitor/factory.py
--rw-r--r--   0        0        0     6208 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/monitor/schema.py
--rw-r--r--   0        0        0     5965 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/monitor/service.py
--rw-r--r--   0        0        0     5754 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/monitor/utils.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/plugins/__init__.py
--rw-r--r--   0        0        0      247 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/plugins/base.py
--rw-r--r--   0        0        0      476 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/plugins/factory.py
--rw-r--r--   0        0        0     2440 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/plugins/langfuse_plugin.py
--rw-r--r--   0        0        0     2454 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/plugins/service.py
--rw-r--r--   0        0        0      707 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/schema.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/session/__init__.py
--rw-r--r--   0        0        0      439 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/session/factory.py
--rw-r--r--   0        0        0     2124 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/session/service.py
--rw-r--r--   0        0        0      516 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/session/utils.py
--rw-r--r--   0        0        0       65 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/settings/__init__.py
--rw-r--r--   0        0        0     4193 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/settings/auth.py
--rw-r--r--   0        0        0    13759 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/settings/base.py
--rw-r--r--   0        0        0      653 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/settings/constants.py
--rw-r--r--   0        0        0      506 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/settings/factory.py
--rw-r--r--   0        0        0     1503 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/settings/manager.py
--rw-r--r--   0        0        0     1526 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/settings/service.py
--rw-r--r--   0        0        0     1381 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/settings/utils.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/socket/__init__.py
--rw-r--r--   0        0        0      472 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/socket/factory.py
--rw-r--r--   0        0        0     2778 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/socket/service.py
--rw-r--r--   0        0        0     3400 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/socket/utils.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/state/__init__.py
--rw-r--r--   0        0        0      432 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/state/factory.py
--rw-r--r--   0        0        0     2546 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/state/service.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/storage/__init__.py
--rw-r--r--   0        0        0      955 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/storage/constants.py
--rw-r--r--   0        0        0     1118 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/storage/factory.py
--rw-r--r--   0        0        0     3919 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/storage/local.py
--rw-r--r--   0        0        0     3801 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/storage/s3.py
--rw-r--r--   0        0        0     1247 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/storage/service.py
--rw-r--r--   0        0        0      219 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/storage/utils.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/store/__init__.py
--rw-r--r--   0        0        0      720 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/store/exceptions.py
--rw-r--r--   0        0        0      444 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/store/factory.py
--rw-r--r--   0        0        0     2013 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/store/schema.py
--rw-r--r--   0        0        0    23442 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/store/service.py
--rw-r--r--   0        0        0     2020 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/store/utils.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/task/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/task/backends/__init__.py
--rw-r--r--   0        0        0     2373 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/task/backends/anyio.py
--rw-r--r--   0        0        0      307 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/task/backends/base.py
--rw-r--r--   0        0        0      885 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/task/backends/celery.py
--rw-r--r--   0        0        0      340 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/task/factory.py
--rw-r--r--   0        0        0     2819 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/task/service.py
--rw-r--r--   0        0        0      613 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/task/utils.py
--rw-r--r--   0        0        0     6206 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/utils.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/variable/__init__.py
--rw-r--r--   0        0        0      459 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/variable/factory.py
--rw-r--r--   0        0        0     4996 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/services/variable/service.py
--rw-r--r--   0        0        0     6473 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/settings.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/template/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.340055 langflow_base-0.0.48/langflow/template/field/__init__.py
--rw-r--r--   0        0        0     5001 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/template/field/base.py
--rw-r--r--   0        0        0      376 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/template/field/prompt.py
--rw-r--r--   0        0        0      445 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/template/frontend_node/__init__.py
--rw-r--r--   0        0        0     5291 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/template/frontend_node/agents.py
--rw-r--r--   0        0        0    11441 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/template/frontend_node/base.py
--rw-r--r--   0        0        0     8146 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/template/frontend_node/chains.py
--rw-r--r--   0        0        0     1609 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/template/frontend_node/constants.py
--rw-r--r--   0        0        0     1733 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/template/frontend_node/custom_components.py
--rw-r--r--   0        0        0     9188 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/template/frontend_node/documentloaders.py
--rw-r--r--   0        0        0     3702 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/template/frontend_node/embeddings.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/template/frontend_node/formatter/__init__.py
--rw-r--r--   0        0        0      298 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/template/frontend_node/formatter/base.py
--rw-r--r--   0        0        0     5719 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/template/frontend_node/formatter/field_formatters.py
--rw-r--r--   0        0        0     5294 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/template/frontend_node/llms.py
--rw-r--r--   0        0        0     6525 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/template/frontend_node/memories.py
--rw-r--r--   0        0        0     3419 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/template/frontend_node/prompts.py
--rw-r--r--   0        0        0      523 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/template/frontend_node/retrievers.py
--rw-r--r--   0        0        0     2356 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/template/frontend_node/textsplitters.py
--rw-r--r--   0        0        0     3836 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/template/frontend_node/tools.py
--rw-r--r--   0        0        0     1035 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/template/frontend_node/utilities.py
--rw-r--r--   0        0        0    11972 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/template/frontend_node/vectorstores.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/template/template/__init__.py
--rw-r--r--   0        0        0     2424 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/template/template/base.py
--rw-r--r--   0        0        0        0 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/utils/__init__.py
--rw-r--r--   0        0        0     5684 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/utils/constants.py
--rw-r--r--   0        0        0      386 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/utils/lazy_load.py
--rw-r--r--   0        0        0     3581 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/utils/logger.py
--rw-r--r--   0        0        0     3154 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/utils/payload.py
--rw-r--r--   0        0        0     1677 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/utils/schemas.py
--rw-r--r--   0        0        0    13569 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/utils/util.py
--rw-r--r--   0        0        0    10400 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/utils/validate.py
--rw-r--r--   0        0        0     1081 2024-05-24 01:13:47.344055 langflow_base-0.0.48/langflow/worker.py
--rw-r--r--   0        0        0     2375 2024-05-24 01:13:47.344055 langflow_base-0.0.48/pyproject.toml
--rw-r--r--   0        0        0     2296 1970-01-01 00:00:00.000000 langflow_base-0.0.48/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.496194 langflow_base-0.0.49/README.md
+-rw-r--r--   0        0        0    20743 2024-05-27 20:10:52.496194 langflow_base-0.0.49/langflow/__main__.py
+-rw-r--r--   0        0        0       38 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/README
+-rw-r--r--   0        0        0     3111 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/env.py
+-rw-r--r--   0        0        0      964 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/script.py.mako
+-rw-r--r--   0        0        0     2826 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/versions/006b3990db50_add_unique_constraints.py
+-rw-r--r--   0        0        0     3053 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/versions/012fb73ac359_add_folder_table.py
+-rw-r--r--   0        0        0      648 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/versions/0b8757876a7c_.py
+-rw-r--r--   0        0        0     2630 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/versions/1a110b568907_replace_credential_table_with_variable.py
+-rw-r--r--   0        0        0     1101 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/versions/1ef9c4f3765d_.py
+-rw-r--r--   0        0        0     1447 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/versions/1f4d6df60295_add_default_fields_column.py
+-rw-r--r--   0        0        0     7221 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/versions/260dbcc8b680_adds_tables.py
+-rw-r--r--   0        0        0     1439 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/versions/29fe8f1f806b_add_missing_index.py
+-rw-r--r--   0        0        0     1774 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/versions/2ac71eb9c3ae_adds_credential_table.py
+-rw-r--r--   0        0        0     6127 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/versions/4e5980a44eaa_fix_date_times_again.py
+-rw-r--r--   0        0        0     2339 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/versions/58b28437a398_modify_nullable.py
+-rw-r--r--   0        0        0     1802 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/versions/63b9c451fd30_add_icon_and_icon_bg_color_to_flow.py
+-rw-r--r--   0        0        0     1809 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/versions/67cc006d50bf_add_profile_image_column.py
+-rw-r--r--   0        0        0     2191 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/versions/6e7b581b5648_fix_nullable.py
+-rw-r--r--   0        0        0     1811 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/versions/7843803a87b5_store_updates.py
+-rw-r--r--   0        0        0     6127 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/versions/79e675cb6752_change_datetime_type.py
+-rw-r--r--   0        0        0     2157 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/versions/7d2162acc8b2_adds_updated_at_and_folder_cols.py
+-rw-r--r--   0        0        0     4281 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/versions/b2fa308044b5_add_unique_constraints.py
+-rw-r--r--   0        0        0     2705 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/versions/bc2f01c40e4a_new_fixes.py
+-rw-r--r--   0        0        0     2052 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/versions/c153816fd85f_set_name_and_value_to_not_nullable.py
+-rw-r--r--   0        0        0     2551 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/versions/e3bc869fa272_fix_nullable.py
+-rw-r--r--   0        0        0      726 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/versions/eb5866d51fd2_change_columns_to_be_nullable.py
+-rw-r--r--   0        0        0     1149 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/versions/f5ee9749d1a6_user_id_can_be_null_in_flow.py
+-rw-r--r--   0        0        0     2018 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/alembic/versions/fd531f8868b1_fix_credential_table.py
+-rw-r--r--   0        0        0     3497 2024-05-27 20:10:52.496194 langflow_base-0.0.49/langflow/alembic.ini
+-rw-r--r--   0        0        0       61 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/api/__init__.py
+-rw-r--r--   0        0        0      810 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/api/router.py
+-rw-r--r--   0        0        0    11575 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/api/utils.py
+-rw-r--r--   0        0        0      986 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/api/v1/__init__.py
+-rw-r--r--   0        0        0     2988 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/api/v1/api_key.py
+-rw-r--r--   0        0        0     5033 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/api/v1/base.py
+-rw-r--r--   0        0        0     4772 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/api/v1/callback.py
+-rw-r--r--   0        0        0    14132 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/api/v1/chat.py
+-rw-r--r--   0        0        0    20125 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/api/v1/endpoints.py
+-rw-r--r--   0        0        0     4991 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/api/v1/files.py
+-rw-r--r--   0        0        0     8578 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/api/v1/flows.py
+-rw-r--r--   0        0        0     8831 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/api/v1/folders.py
+-rw-r--r--   0        0        0     5137 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/api/v1/login.py
+-rw-r--r--   0        0        0     3007 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/api/v1/monitor.py
+-rw-r--r--   0        0        0     8198 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/api/v1/schemas.py
+-rw-r--r--   0        0        0     7347 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/api/v1/store.py
+-rw-r--r--   0        0        0     5126 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/api/v1/users.py
+-rw-r--r--   0        0        0     3257 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/api/v1/validate.py
+-rw-r--r--   0        0        0     4399 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/api/v1/variable.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/base/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/base/agents/__init__.py
+-rw-r--r--   0        0        0     2947 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/base/agents/agent.py
+-rw-r--r--   0        0        0      941 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/base/agents/default_prompts.py
+-rw-r--r--   0        0        0     3993 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/base/agents/utils.py
+-rw-r--r--   0        0        0      768 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/base/constants.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/base/data/__init__.py
+-rw-r--r--   0        0        0     4922 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/base/data/utils.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/base/io/__init__.py
+-rw-r--r--   0        0        0     5133 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/base/io/chat.py
+-rw-r--r--   0        0        0     1546 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/base/io/text.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/base/memory/__init__.py
+-rw-r--r--   0        0        0     1735 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/base/memory/memory.py
+-rw-r--r--   0        0        0       68 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/base/models/__init__.py
+-rw-r--r--   0        0        0       89 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/base/models/groq_constants.py
+-rw-r--r--   0        0        0     4250 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/base/models/model.py
+-rw-r--r--   0        0        0      102 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/base/models/openai_constants.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/base/prompts/__init__.py
+-rw-r--r--   0        0        0     3278 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/base/prompts/api_utils.py
+-rw-r--r--   0        0        0     1538 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/base/prompts/utils.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/base/tools/__init__.py
+-rw-r--r--   0        0        0      751 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/base/tools/base.py
+-rw-r--r--   0        0        0      275 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/components/__init__.py
+-rw-r--r--   0        0        0     1448 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/components/agents/CSVAgent.py
+-rw-r--r--   0        0        0      746 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/components/agents/JsonAgent.py
+-rw-r--r--   0        0        0     1077 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/components/agents/SQLAgent.py
+-rw-r--r--   0        0        0     2392 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/components/agents/ToolCallingAgent.py
+-rw-r--r--   0        0        0      842 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/components/agents/VectorStoreAgent.py
+-rw-r--r--   0        0        0      848 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/components/agents/VectorStoreRouterAgent.py
+-rw-r--r--   0        0        0     4147 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/components/agents/XMLAgent.py
+-rw-r--r--   0        0        0      474 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/components/agents/__init__.py
+-rw-r--r--   0        0        0     1508 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/components/chains/ConversationChain.py
+-rw-r--r--   0        0        0     1008 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/components/chains/LLMChain.py
+-rw-r--r--   0        0        0      970 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/components/chains/LLMCheckerChain.py
+-rw-r--r--   0        0        0     1566 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/components/chains/LLMMathChain.py
+-rw-r--r--   0        0        0     2726 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/components/chains/RetrievalQA.py
+-rw-r--r--   0        0        0     2509 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/components/chains/RetrievalQAWithSourcesChain.py
+-rw-r--r--   0        0        0     2305 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/components/chains/SQLGenerator.py
+-rw-r--r--   0        0        0      608 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/components/chains/__init__.py
+-rw-r--r--   0        0        0     3785 2024-05-27 20:10:52.500194 langflow_base-0.0.49/langflow/components/data/APIRequest.py
+-rw-r--r--   0        0        0     2382 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/data/Directory.py
+-rw-r--r--   0        0        0     1667 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/data/File.py
+-rw-r--r--   0        0        0      698 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/data/URL.py
+-rw-r--r--   0        0        0      221 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/documentloaders/__init__.py
+-rw-r--r--   0        0        0     1585 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/embeddings/AmazonBedrockEmbeddings.py
+-rw-r--r--   0        0        0     2235 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/embeddings/AzureOpenAIEmbeddings.py
+-rw-r--r--   0        0        0     1411 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/embeddings/CohereEmbeddings.py
+-rw-r--r--   0        0        0     1520 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/embeddings/HuggingFaceEmbeddings.py
+-rw-r--r--   0        0        0     1825 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/embeddings/HuggingFaceInferenceAPIEmbeddings.py
+-rw-r--r--   0        0        0     2026 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/embeddings/MistalAIEmbeddings.py
+-rw-r--r--   0        0        0     1168 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/embeddings/OllamaEmbeddings.py
+-rw-r--r--   0        0        0     5488 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/embeddings/OpenAIEmbeddings.py
+-rw-r--r--   0        0        0     3080 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/embeddings/VertexAIEmbeddings.py
+-rw-r--r--   0        0        0      833 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/embeddings/__init__.py
+-rw-r--r--   0        0        0     7855 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/experimental/AgentComponent.py
+-rw-r--r--   0        0        0      758 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/experimental/ClearMessageHistory.py
+-rw-r--r--   0        0        0     1492 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/experimental/ExtractDataFromRecord.py
+-rw-r--r--   0        0        0     3429 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/experimental/FlowTool.py
+-rw-r--r--   0        0        0      470 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/experimental/ListFlows.py
+-rw-r--r--   0        0        0      566 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/experimental/Listen.py
+-rw-r--r--   0        0        0      956 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/experimental/MergeRecords.py
+-rw-r--r--   0        0        0     1421 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/experimental/Notify.py
+-rw-r--r--   0        0        0     1172 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/experimental/Pass.py
+-rw-r--r--   0        0        0      692 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/experimental/PythonFunction.py
+-rw-r--r--   0        0        0     2376 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/experimental/RunFlow.py
+-rw-r--r--   0        0        0     4692 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/experimental/RunnableExecutor.py
+-rw-r--r--   0        0        0     2311 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/experimental/SQLExecutor.py
+-rw-r--r--   0        0        0     1513 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/experimental/SplitText.py
+-rw-r--r--   0        0        0     1294 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/experimental/StoreMessage.py
+-rw-r--r--   0        0        0     5190 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/experimental/SubFlow.py
+-rw-r--r--   0        0        0     2750 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/experimental/TextOperator.py
+-rw-r--r--   0        0        0     1001 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/experimental/__init__.py
+-rw-r--r--   0        0        0     1008 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/helpers/CombineText.py
+-rw-r--r--   0        0        0      855 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/helpers/CombineTextsUnsorted.py
+-rw-r--r--   0        0        0     3257 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/helpers/CreateRecord.py
+-rw-r--r--   0        0        0      526 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/helpers/CustomComponent.py
+-rw-r--r--   0        0        0      662 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/helpers/DocumentToRecord.py
+-rw-r--r--   0        0        0      813 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/helpers/IDGenerator.py
+-rw-r--r--   0        0        0     2996 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/helpers/MemoryComponent.py
+-rw-r--r--   0        0        0     1838 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/helpers/MessageHistory.py
+-rw-r--r--   0        0        0     1142 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/helpers/RecordsToText.py
+-rw-r--r--   0        0        0     1331 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/helpers/ShouldRunNext.py
+-rw-r--r--   0        0        0     1089 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/helpers/UpdateRecord.py
+-rw-r--r--   0        0        0      555 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/helpers/__init__.py
+-rw-r--r--   0        0        0     1063 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/inputs/ChatInput.py
+-rw-r--r--   0        0        0     1134 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/inputs/Prompt.py
+-rw-r--r--   0        0        0     1032 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/inputs/TextInput.py
+-rw-r--r--   0        0        0      159 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/inputs/__init__.py
+-rw-r--r--   0        0        0     1252 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/langchain_utilities/BingSearchAPIWrapper.py
+-rw-r--r--   0        0        0      786 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/langchain_utilities/GoogleSearchAPIWrapper.py
+-rw-r--r--   0        0        0     1679 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/langchain_utilities/GoogleSerperAPIWrapper.py
+-rw-r--r--   0        0        0     1572 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/langchain_utilities/JSONDocumentBuilder.py
+-rw-r--r--   0        0        0      650 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/langchain_utilities/SQLDatabase.py
+-rw-r--r--   0        0        0     1584 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/langchain_utilities/SearchApi.py
+-rw-r--r--   0        0        0     1137 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/langchain_utilities/SearxSearchWrapper.py
+-rw-r--r--   0        0        0     1012 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/langchain_utilities/SerpAPIWrapper.py
+-rw-r--r--   0        0        0     1010 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/langchain_utilities/WikipediaAPIWrapper.py
+-rw-r--r--   0        0        0      708 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/langchain_utilities/WolframAlphaAPIWrapper.py
+-rw-r--r--   0        0        0     3042 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/memories/AstraDBMessageReader.py
+-rw-r--r--   0        0        0     3833 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/memories/AstraDBMessageWriter.py
+-rw-r--r--   0        0        0     5992 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/memories/ZepMessageReader.py
+-rw-r--r--   0        0        0     3956 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/memories/ZepMessageWriter.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/memories/__init__.py
+-rw-r--r--   0        0        0     2269 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/model_specs/AmazonBedrockSpecs.py
+-rw-r--r--   0        0        0     2668 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/model_specs/AnthropicLLMSpecs.py
+-rw-r--r--   0        0        0     3274 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/model_specs/AzureChatOpenAISpecs.py
+-rw-r--r--   0        0        0     3627 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/model_specs/BaiduQianfanChatEndpointsSpecs.py
+-rw-r--r--   0        0        0     3538 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/model_specs/BaiduQianfanLLMEndpointsSpecs.py
+-rw-r--r--   0        0        0     2938 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/model_specs/ChatAnthropicSpecs.py
+-rw-r--r--   0        0        0     5753 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/model_specs/ChatLiteLLMSpecs.py
+-rw-r--r--   0        0        0     2771 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/model_specs/ChatMistralSpecs.py
+-rw-r--r--   0        0        0     9830 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/model_specs/ChatOllamaEndpointSpecs.py
+-rw-r--r--   0        0        0     2529 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/model_specs/ChatOpenAISpecs.py
+-rw-r--r--   0        0        0     2488 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/model_specs/ChatVertexAISpecs.py
+-rw-r--r--   0        0        0     1351 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/model_specs/CohereSpecs.py
+-rw-r--r--   0        0        0     2858 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/model_specs/GoogleGenerativeAISpecs.py
+-rw-r--r--   0        0        0     2814 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/model_specs/GroqModelSpecs.py
+-rw-r--r--   0        0        0     1617 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/model_specs/HuggingFaceEndpointsSpecs.py
+-rw-r--r--   0        0        0     5768 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/model_specs/OllamaLLMSpecs.py
+-rw-r--r--   0        0        0     4786 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/model_specs/VertexAISpecs.py
+-rw-r--r--   0        0        0     1167 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/model_specs/__init__.py
+-rw-r--r--   0        0        0     3630 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/models/AmazonBedrockModel.py
+-rw-r--r--   0        0        0     3654 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/models/AnthropicModel.py
+-rw-r--r--   0        0        0     3903 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/models/AzureOpenAIModel.py
+-rw-r--r--   0        0        0     4421 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/models/BaiduQianfanChatModel.py
+-rw-r--r--   0        0        0     6440 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/models/ChatLiteLLMModel.py
+-rw-r--r--   0        0        0     2204 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/models/CohereModel.py
+-rw-r--r--   0        0        0     3695 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/models/GoogleGenerativeAIModel.py
+-rw-r--r--   0        0        0     3223 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/models/GroqModel.py
+-rw-r--r--   0        0        0     2631 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/models/HuggingFaceModel.py
+-rw-r--r--   0        0        0     4609 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/models/MistralModel.py
+-rw-r--r--   0        0        0    11116 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/models/OllamaModel.py
+-rw-r--r--   0        0        0     3367 2024-05-27 20:10:52.504194 langflow_base-0.0.49/langflow/components/models/OpenAIModel.py
+-rw-r--r--   0        0        0     3620 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/models/VertexAiModel.py
+-rw-r--r--   0        0        0      934 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/models/__init__.py
+-rw-r--r--   0        0        0      921 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/outputs/ChatOutput.py
+-rw-r--r--   0        0        0      282 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/outputs/RecordsOutput.py
+-rw-r--r--   0        0        0     1008 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/outputs/TextOutput.py
+-rw-r--r--   0        0        0      110 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/outputs/__init__.py
+-rw-r--r--   0        0        0     1796 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/retrievers/AmazonKendra.py
+-rw-r--r--   0        0        0     1109 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/retrievers/MetalRetriever.py
+-rw-r--r--   0        0        0     2335 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/retrievers/MultiQueryRetriever.py
+-rw-r--r--   0        0        0     2504 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/retrievers/VectaraSelfQueryRetriver.py
+-rw-r--r--   0        0        0      547 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/retrievers/VectorStoreRetriever.py
+-rw-r--r--   0        0        0      503 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/retrievers/__init__.py
+-rw-r--r--   0        0        0     1524 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/textsplitters/CharacterTextSplitter.py
+-rw-r--r--   0        0        0     3048 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/textsplitters/LanguageRecursiveTextSplitter.py
+-rw-r--r--   0        0        0     3304 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/textsplitters/RecursiveCharacterTextSplitter.py
+-rw-r--r--   0        0        0      378 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/textsplitters/__init__.py
+-rw-r--r--   0        0        0      908 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/toolkits/JsonToolkit.py
+-rw-r--r--   0        0        0     1787 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/toolkits/Metaphor.py
+-rw-r--r--   0        0        0     1306 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/toolkits/OpenAPIToolkit.py
+-rw-r--r--   0        0        0      785 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/toolkits/VectorStoreInfo.py
+-rw-r--r--   0        0        0      857 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/toolkits/VectorStoreRouterToolkit.py
+-rw-r--r--   0        0        0      784 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/toolkits/VectorStoreToolkit.py
+-rw-r--r--   0        0        0      527 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/toolkits/__init__.py
+-rw-r--r--   0        0        0     2706 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/tools/PythonREPLTool.py
+-rw-r--r--   0        0        0      969 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/tools/RetrieverTool.py
+-rw-r--r--   0        0        0     1132 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/tools/SearchAPITool.py
+-rw-r--r--   0        0        0     1584 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/tools/SearchApi.py
+-rw-r--r--   0        0        0      290 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/tools/__init__.py
+-rw-r--r--   0        0        0     6489 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorsearch/AstraDBSearch.py
+-rw-r--r--   0        0        0     4735 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorsearch/ChromaSearch.py
+-rw-r--r--   0        0        0     2870 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorsearch/CouchbaseSearch.py
+-rw-r--r--   0        0        0     1875 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorsearch/FAISSSearch.py
+-rw-r--r--   0        0        0     2307 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorsearch/MongoDBAtlasVectorSearch.py
+-rw-r--r--   0        0        0     3569 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorsearch/PineconeSearch.py
+-rw-r--r--   0        0        0     4085 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorsearch/QdrantSearch.py
+-rw-r--r--   0        0        0     3003 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorsearch/RedisSearch.py
+-rw-r--r--   0        0        0     2048 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorsearch/SupabaseVectorStoreSearch.py
+-rw-r--r--   0        0        0     2215 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorsearch/VectaraSearch.py
+-rw-r--r--   0        0        0     2854 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorsearch/WeaviateSearch.py
+-rw-r--r--   0        0        0     1021 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorsearch/__init__.py
+-rw-r--r--   0        0        0     2660 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorsearch/pgvectorSearch.py
+-rw-r--r--   0        0        0     7031 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorstores/AstraDB.py
+-rw-r--r--   0        0        0     5094 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorstores/Chroma.py
+-rw-r--r--   0        0        0     3551 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorstores/Couchbase.py
+-rw-r--r--   0        0        0     1785 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorstores/FAISS.py
+-rw-r--r--   0        0        0     2438 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorstores/MongoDBAtlasVector.py
+-rw-r--r--   0        0        0     5546 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorstores/Pinecone.py
+-rw-r--r--   0        0        0     4383 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorstores/Qdrant.py
+-rw-r--r--   0        0        0     3074 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorstores/Redis.py
+-rw-r--r--   0        0        0     1868 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorstores/SupabaseVectorStore.py
+-rw-r--r--   0        0        0     2998 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorstores/Vectara.py
+-rw-r--r--   0        0        0     3651 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorstores/Weaviate.py
+-rw-r--r--   0        0        0      847 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorstores/__init__.py
+-rw-r--r--   0        0        0       80 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorstores/base/__init__.py
+-rw-r--r--   0        0        0     1618 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorstores/base/model.py
+-rw-r--r--   0        0        0     2876 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/components/vectorstores/pgvector.py
+-rw-r--r--   0        0        0    10194 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/config.yaml
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/core/__init__.py
+-rw-r--r--   0        0        0      351 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/core/celery_app.py
+-rw-r--r--   0        0        0      778 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/core/celeryconfig.py
+-rw-r--r--   0        0        0       92 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/custom/__init__.py
+-rw-r--r--   0        0        0     1269 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/custom/attributes.py
+-rw-r--r--   0        0        0       62 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/custom/code_parser/__init__.py
+-rw-r--r--   0        0        0    13255 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/custom/code_parser/code_parser.py
+-rw-r--r--   0        0        0     1394 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/custom/code_parser/utils.py
+-rw-r--r--   0        0        0       77 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/custom/custom_component/__init__.py
+-rw-r--r--   0        0        0     2878 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/custom/custom_component/component.py
+-rw-r--r--   0        0        0    17289 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/custom/custom_component/custom_component.py
+-rw-r--r--   0        0        0       77 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/custom/directory_reader/__init__.py
+-rw-r--r--   0        0        0    11444 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/custom/directory_reader/directory_reader.py
+-rw-r--r--   0        0        0     5577 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/custom/directory_reader/utils.py
+-rw-r--r--   0        0        0      358 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/custom/eval.py
+-rw-r--r--   0        0        0      723 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/custom/schema.py
+-rw-r--r--   0        0        0    16526 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/custom/utils.py
+-rw-r--r--   0        0        0     1485 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/field_typing/__init__.py
+-rw-r--r--   0        0        0     1821 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/field_typing/constants.py
+-rw-r--r--   0        0        0     1060 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/field_typing/range_spec.py
+-rw-r--r--   0        0        0      423 2024-05-27 20:12:20.876251 langflow_base-0.0.49/langflow/frontend/assets/a-arrow-down-338b684d.js
+-rw-r--r--   0        0        0      422 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/a-arrow-up-60532c04.js
+-rw-r--r--   0        0        0      444 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/a-large-small-1fd2cf94.js
+-rw-r--r--   0        0        0      513 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/accessibility-7deeca04.js
+-rw-r--r--   0        0        0      312 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/activity-c184725f.js
+-rw-r--r--   0        0        0      384 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/activity-square-88b26d9e.js
+-rw-r--r--   0        0        0      541 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/air-vent-f05f65f0.js
+-rw-r--r--   0        0        0      419 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/airplay-ecb19158.js
+-rw-r--r--   0        0        0      514 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/alarm-clock-b53682c1.js
+-rw-r--r--   0        0        0      521 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/alarm-clock-check-d3b32670.js
+-rw-r--r--   0        0        0      515 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/alarm-clock-minus-fc96df2e.js
+-rw-r--r--   0        0        0      543 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/alarm-clock-off-6a0418e2.js
+-rw-r--r--   0        0        0      551 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/alarm-clock-plus-bfb4a090.js
+-rw-r--r--   0        0        0      562 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/alarm-smoke-f5027e9e.js
+-rw-r--r--   0        0        0      392 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/album-7e1574fb.js
+-rw-r--r--   0        0        0      483 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/alert-octagon-d9330aa2.js
+-rw-r--r--   0        0        0      440 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/alert-triangle-5cb2282d.js
+-rw-r--r--   0        0        0      424 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/align-center-506fc132.js
+-rw-r--r--   0        0        0      585 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/align-center-horizontal-e3305b6c.js
+-rw-r--r--   0        0        0      583 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/align-center-vertical-6fd65fe5.js
+-rw-r--r--   0        0        0      435 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/align-end-horizontal-56dd8854.js
+-rw-r--r--   0        0        0      433 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/align-end-vertical-c2761c94.js
+-rw-r--r--   0        0        0      558 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/align-horizontal-distribute-center-6966cea5.js
+-rw-r--r--   0        0        0      483 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/align-horizontal-distribute-end-e4d8f68b.js
+-rw-r--r--   0        0        0      484 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/align-horizontal-distribute-start-deef9a79.js
+-rw-r--r--   0        0        0      446 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/align-horizontal-justify-center-54c1ffd6.js
+-rw-r--r--   0        0        0      443 2024-05-27 20:12:20.876251 langflow_base-0.0.49/langflow/frontend/assets/align-horizontal-justify-end-35555d6d.js
+-rw-r--r--   0        0        0      444 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/align-horizontal-justify-start-8c57d718.js
+-rw-r--r--   0        0        0      414 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/align-horizontal-space-around-1fc8c174.js
+-rw-r--r--   0        0        0      481 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/align-horizontal-space-between-fe30b7bb.js
+-rw-r--r--   0        0        0      425 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/align-justify-7430845d.js
+-rw-r--r--   0        0        0      422 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/align-left-98f95c28.js
+-rw-r--r--   0        0        0      423 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/align-right-4454a958.js
+-rw-r--r--   0        0        0      436 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/align-start-horizontal-b9435ff6.js
+-rw-r--r--   0        0        0      434 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/align-start-vertical-5f600266.js
+-rw-r--r--   0        0        0      556 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/align-vertical-distribute-center-e4878d08.js
+-rw-r--r--   0        0        0      481 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/align-vertical-distribute-end-7cd22002.js
+-rw-r--r--   0        0        0      482 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/align-vertical-distribute-start-6c0545ec.js
+-rw-r--r--   0        0        0      444 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/align-vertical-justify-center-bb10c107.js
+-rw-r--r--   0        0        0      441 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/align-vertical-justify-end-3f0569f5.js
+-rw-r--r--   0        0        0      442 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/align-vertical-justify-start-865ed5d0.js
+-rw-r--r--   0        0        0      412 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/align-vertical-space-around-07b5b726.js
+-rw-r--r--   0        0        0      479 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/align-vertical-space-between-a733674f.js
+-rw-r--r--   0        0        0      692 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/ambulance-b3609100.js
+-rw-r--r--   0        0        0      416 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/ampersand-f5a2e3aa.js
+-rw-r--r--   0        0        0      480 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/ampersands-d0253acc.js
+-rw-r--r--   0        0        0      391 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/anchor-73a68d00.js
+-rw-r--r--   0        0        0      511 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/angry-c69f99c1.js
+-rw-r--r--   0        0        0      412 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/annoyed-0943735a.js
+-rw-r--r--   0        0        0      489 2024-05-27 20:12:20.876251 langflow_base-0.0.49/langflow/frontend/assets/antenna-2235cf56.js
+-rw-r--r--   0        0        0      502 2024-05-27 20:12:20.876251 langflow_base-0.0.49/langflow/frontend/assets/anvil-fb30cafa.js
+-rw-r--r--   0        0        0      581 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/aperture-ae888f7c.js
+-rw-r--r--   0        0        0      432 2024-05-27 20:12:20.876251 langflow_base-0.0.49/langflow/frontend/assets/app-window-0aa03576.js
+-rw-r--r--   0        0        0      491 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/apple-f15b18b1.js
+-rw-r--r--   0        0        0      428 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/archive-2683c9a2.js
+-rw-r--r--   0        0        0      514 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/archive-restore-34113244.js
+-rw-r--r--   0        0        0      472 2024-05-27 20:12:20.876251 langflow_base-0.0.49/langflow/frontend/assets/archive-x-66c84c4a.js
+-rw-r--r--   0        0        0      349 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/area-chart-16f6cfc6.js
+-rw-r--r--   0        0        0      503 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/armchair-a28f314e.js
+-rw-r--r--   0        0        0      316 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/arrow-big-down-703869c0.js
+-rw-r--r--   0        0        0      354 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/arrow-big-down-dash-d4a5f63d.js
+-rw-r--r--   0        0        0      318 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/arrow-big-left-8aeb87df.js
+-rw-r--r--   0        0        0      359 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/arrow-big-left-dash-0e9d8ada.js
+-rw-r--r--   0        0        0      316 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/arrow-big-right-0d80daa8.js
+-rw-r--r--   0        0        0      355 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/arrow-big-right-dash-ad8cf79f.js
+-rw-r--r--   0        0        0      355 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/arrow-big-up-dash-bb5022b6.js
+-rw-r--r--   0        0        0      482 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/arrow-down-0-1-1849a1e5.js
+-rw-r--r--   0        0        0      482 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/arrow-down-1-0-93c1214c.js
+-rw-r--r--   0        0        0      339 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/arrow-down-15182de4.js
+-rw-r--r--   0        0        0      480 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/arrow-down-a-z-2f5cf730.js
+-rw-r--r--   0        0        0      392 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/arrow-down-circle-02d39da3.js
+-rw-r--r--   0        0        0      382 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/arrow-down-from-line-79907b98.js
+-rw-r--r--   0        0        0      341 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/arrow-down-left-72dcddc0.js
+-rw-r--r--   0        0        0      404 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/arrow-down-left-from-circle-f6565ead.js
+-rw-r--r--   0        0        0      435 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/arrow-down-left-from-square-c5d61426.js
+-rw-r--r--   0        0        0      412 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/arrow-down-left-square-03b5a2e2.js
+-rw-r--r--   0        0        0      457 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/arrow-down-narrow-wide-b192f668.js
+-rw-r--r--   0        0        0      342 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/arrow-down-right-f81908eb.js
+-rw-r--r--   0        0        0      408 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/arrow-down-right-from-circle-54dfc45c.js
+-rw-r--r--   0        0        0      439 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/arrow-down-right-from-square-eb44ce78.js
+-rw-r--r--   0        0        0      411 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/arrow-down-right-square-db440ed9.js
+-rw-r--r--   0        0        0      409 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/arrow-down-square-14d38d87.js
+-rw-r--r--   0        0        0      391 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/arrow-down-to-dot-97c32166.js
+-rw-r--r--   0        0        0      381 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/arrow-down-to-line-c854a162.js
+-rw-r--r--   0        0        0      418 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/arrow-down-up-503d530e.js
+-rw-r--r--   0        0        0      457 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/arrow-down-wide-narrow-73411b65.js
+-rw-r--r--   0        0        0      481 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/arrow-down-z-a-0a8f0a5a.js
+-rw-r--r--   0        0        0      393 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/arrow-left-circle-9e413a44.js
+-rw-r--r--   0        0        0      382 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/arrow-left-from-line-7e401686.js
+-rw-r--r--   0        0        0      421 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/arrow-left-right-c015b85a.js
+-rw-r--r--   0        0        0      410 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/arrow-left-square-76b0c96b.js
+-rw-r--r--   0        0        0      380 2024-05-27 20:12:20.876251 langflow_base-0.0.49/langflow/frontend/assets/arrow-left-to-line-da4690d3.js
+-rw-r--r--   0        0        0      339 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/arrow-right-1d0201a6.js
+-rw-r--r--   0        0        0      389 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/arrow-right-circle-bb3d7c2d.js
+-rw-r--r--   0        0        0      384 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/arrow-right-from-line-114a0b5c.js
+-rw-r--r--   0        0        0      421 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/arrow-right-left-c17dbdf5.js
+-rw-r--r--   0        0        0      411 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/arrow-right-square-e2e3c49c.js
+-rw-r--r--   0        0        0      383 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/arrow-right-to-line-eb08b9fd.js
+-rw-r--r--   0        0        0      479 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/arrow-up-0-1-82594474.js
+-rw-r--r--   0        0        0      336 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/arrow-up-01a00be9.js
+-rw-r--r--   0        0        0      479 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/arrow-up-1-0-021af6b1.js
+-rw-r--r--   0        0        0      477 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/arrow-up-a-z-b8c69625.js
+-rw-r--r--   0        0        0      392 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/arrow-up-circle-99b08177.js
+-rw-r--r--   0        0        0      418 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/arrow-up-down-56751fc0.js
+-rw-r--r--   0        0        0      390 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/arrow-up-from-dot-0be5e248.js
+-rw-r--r--   0        0        0      381 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/arrow-up-from-line-53ee15ad.js
+-rw-r--r--   0        0        0      339 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/arrow-up-left-2a24a4d7.js
+-rw-r--r--   0        0        0      398 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/arrow-up-left-from-circle-32c439ee.js
+-rw-r--r--   0        0        0      431 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/arrow-up-left-from-square-01fc1e48.js
+-rw-r--r--   0        0        0      410 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/arrow-up-left-square-2b91a55f.js
+-rw-r--r--   0        0        0      456 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/arrow-up-narrow-wide-17ff0540.js
+-rw-r--r--   0        0        0      340 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/arrow-up-right-1a25e20d.js
+-rw-r--r--   0        0        0      402 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/arrow-up-right-from-circle-b5869313.js
+-rw-r--r--   0        0        0      433 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/arrow-up-right-from-square-a65d79d4.js
+-rw-r--r--   0        0        0      409 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/arrow-up-right-square-344bad1c.js
+-rw-r--r--   0        0        0      409 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/arrow-up-square-b238a11c.js
+-rw-r--r--   0        0        0      456 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/arrow-up-wide-narrow-49508601.js
+-rw-r--r--   0        0        0      478 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/arrow-up-z-a-89c31683.js
+-rw-r--r--   0        0        0      459 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/arrows-up-from-line-353e8880.js
+-rw-r--r--   0        0        0      388 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/asterisk-d519fe8d.js
+-rw-r--r--   0        0        0      446 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/asterisk-square-627151cc.js
+-rw-r--r--   0        0        0      368 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/at-sign-e494f28f.js
+-rw-r--r--   0        0        0      603 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/atom-634b4c72.js
+-rw-r--r--   0        0        0      479 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/audio-lines-c710554a.js
+-rw-r--r--   0        0        0      394 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/audio-waveform-72cc8864.js
+-rw-r--r--   0        0        0      365 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/award-838dab96.js
+-rw-r--r--   0        0        0      385 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/axe-c8895529.js
+-rw-r--r--   0        0        0      333 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/axis-3d-ed2aa0d7.js
+-rw-r--r--   0        0        0      565 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/baby-804d807f.js
+-rw-r--r--   0        0        0      564 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/backpack-6bb8f8dc.js
+-rw-r--r--   0        0        0      443 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/badge-15f43f3b.js
+-rw-r--r--   0        0        0      562 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/badge-alert-2792746a.js
+-rw-r--r--   0        0        0      535 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/badge-cent-9c74db33.js
+-rw-r--r--   0        0        0      490 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/badge-check-67516e36.js
+-rw-r--r--   0        0        0      559 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/badge-dollar-sign-534ee5dd.js
+-rw-r--r--   0        0        0      535 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/badge-euro-e86cd8b5.js
+-rw-r--r--   0        0        0      571 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/badge-help-a99e4c15.js
+-rw-r--r--   0        0        0      580 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/badge-indian-rupee-b932ef23.js
+-rw-r--r--   0        0        0      560 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/badge-info-38c2f4b4.js
+-rw-r--r--   0        0        0      604 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/badge-japanese-yen-f7736118.js
+-rw-r--r--   0        0        0      503 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/badge-minus-2b2d9863.js
+-rw-r--r--   0        0        0      564 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/badge-percent-96abe075.js
+-rw-r--r--   0        0        0      557 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/badge-plus-ef608fba.js
+-rw-r--r--   0        0        0      585 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/badge-pound-sterling-5e65ad38.js
+-rw-r--r--   0        0        0      546 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/badge-russian-ruble-b25d9ad9.js
+-rw-r--r--   0        0        0      565 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/badge-swiss-franc-3060d493.js
+-rw-r--r--   0        0        0      552 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/badge-x-0845dea8.js
+-rw-r--r--   0        0        0      560 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/baggage-claim-4b4424f5.js
+-rw-r--r--   0        0        0      344 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/ban-2d975df8.js
+-rw-r--r--   0        0        0      492 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/banana-a2f8f835.js
+-rw-r--r--   0        0        0      420 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/banknote-ef157399.js
+-rw-r--r--   0        0        0      423 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/bar-chart-1b02f895.js
+-rw-r--r--   0        0        0      424 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/bar-chart-2-8a9cea9c.js
+-rw-r--r--   0        0        0      409 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/bar-chart-3-906213ee.js
+-rw-r--r--   0        0        0      409 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/bar-chart-4-686d3252.js
+-rw-r--r--   0        0        0      431 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/bar-chart-big-b17c6716.js
+-rw-r--r--   0        0        0      415 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/bar-chart-horizontal-576570cf.js
+-rw-r--r--   0        0        0      440 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/bar-chart-horizontal-big-5ae473e6.js
+-rw-r--r--   0        0        0      440 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/barcode-958cbc2c.js
+-rw-r--r--   0        0        0      375 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/baseline-c9ed7767.js
+-rw-r--r--   0        0        0      591 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/bath-52eb7e8c.js
+-rw-r--r--   0        0        0      386 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/battery-49889fb9.js
+-rw-r--r--   0        0        0      502 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/battery-charging-a0b81b04.js
+-rw-r--r--   0        0        0      556 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/battery-full-67d8a9b3.js
+-rw-r--r--   0        0        0      443 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/battery-low-9d9655fb.js
+-rw-r--r--   0        0        0      502 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/battery-medium-0eab96f5.js
+-rw-r--r--   0        0        0      566 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/battery-warning-62ab1682.js
+-rw-r--r--   0        0        0      399 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/beaker-30d946d7.js
+-rw-r--r--   0        0        0      476 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/bean-4d702040.js
+-rw-r--r--   0        0        0      603 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/bean-off-7b09212a.js
+-rw-r--r--   0        0        0      414 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/bed-95c1ff23.js
+-rw-r--r--   0        0        0      471 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/bed-double-dc7b8344.js
+-rw-r--r--   0        0        0      435 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/bed-single-b69bd325.js
+-rw-r--r--   0        0        0      593 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/beef-9bf4ee37.js
+-rw-r--r--   0        0        0      642 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/beer-41f73772.js
+-rw-r--r--   0        0        0      466 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/bell-dot-973b925e.js
+-rw-r--r--   0        0        0      569 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/bell-electric-5dc74521.js
+-rw-r--r--   0        0        0      454 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/bell-minus-75b6bb37.js
+-rw-r--r--   0        0        0      494 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/bell-off-013dd363.js
+-rw-r--r--   0        0        0      492 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/bell-plus-35794ca9.js
+-rw-r--r--   0        0        0      489 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/bell-ring-d87fc621.js
+-rw-r--r--   0        0        0      444 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/between-horizontal-end-8154d6be.js
+-rw-r--r--   0        0        0      444 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/between-horizontal-start-b3ebce6e.js
+-rw-r--r--   0        0        0      441 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/between-vertical-end-5e57d29a.js
+-rw-r--r--   0        0        0      443 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/between-vertical-start-09c1d3e1.js
+-rw-r--r--   0        0        0      458 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/bike-0db4bab8.js
+-rw-r--r--   0        0        0      856 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/biohazard-7f870d29.js
+-rw-r--r--   0        0        0      548 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/bird-ad099b8b.js
+-rw-r--r--   0        0        0      509 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/bitcoin-ed65414a.js
+-rw-r--r--   0        0        0      344 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/blend-da79df0d.js
+-rw-r--r--   0        0        0      523 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/blinds-9d36e4b5.js
+-rw-r--r--   0        0        0      313 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/bluetooth-c725ba5e.js
+-rw-r--r--   0        0        0      432 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/bluetooth-connected-4c6854cc.js
+-rw-r--r--   0        0        0      400 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/bluetooth-off-c097243a.js
+-rw-r--r--   0        0        0      419 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/bluetooth-searching-8a896819.js
+-rw-r--r--   0        0        0      361 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/bold-701f2144.js
+-rw-r--r--   0        0        0      452 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/bolt-c268ffe9.js
+-rw-r--r--   0        0        0      453 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/bomb-cc1a91f7.js
+-rw-r--r--   0        0        0      470 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/bone-cc6365d6.js
+-rw-r--r--   0        0        0      345 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/book-58172484.js
+-rw-r--r--   0        0        0      428 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/book-a-6f4d63ca.js
+-rw-r--r--   0        0        0      457 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/book-audio-1fb3edb9.js
+-rw-r--r--   0        0        0      393 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/book-check-cadcac19.js
+-rw-r--r--   0        0        0      440 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/book-copy-196a2644.js
+-rw-r--r--   0        0        0      714 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/book-dashed-86cbe767.js
+-rw-r--r--   0        0        0      428 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/book-down-3d1b2c2a.js
+-rw-r--r--   0        0        0      503 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/book-headphones-3104e0cd.js
+-rw-r--r--   0        0        0      526 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/book-heart-8beae983.js
+-rw-r--r--   0        0        0      467 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/book-image-3a884dca.js
+-rw-r--r--   0        0        0      509 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/book-key-049e6543.js
+-rw-r--r--   0        0        0      500 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/book-lock-2c04fc1c.js
+-rw-r--r--   0        0        0      386 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/book-minus-5455678a.js
+-rw-r--r--   0        0        0      398 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/book-open-a5fffbd9.js
+-rw-r--r--   0        0        0      463 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/book-open-check-614c22a6.js
+-rw-r--r--   0        0        0      546 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/book-open-text-0c4694bc.js
+-rw-r--r--   0        0        0      421 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/book-plus-72092ac0.js
+-rw-r--r--   0        0        0      420 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/book-text-8fc03a16.js
+-rw-r--r--   0        0        0      462 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/book-type-9f03d08e.js
+-rw-r--r--   0        0        0      501 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/book-up-2-42570482.js
+-rw-r--r--   0        0        0      426 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/book-up-8a64d962.js
+-rw-r--r--   0        0        0      445 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/book-user-3222d5f5.js
+-rw-r--r--   0        0        0      425 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/book-x-fe5f9aa3.js
+-rw-r--r--   0        0        0      338 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/bookmark-806c6c55.js
+-rw-r--r--   0        0        0      382 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/bookmark-check-56bf6079.js
+-rw-r--r--   0        0        0      398 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/bookmark-minus-c8279111.js
+-rw-r--r--   0        0        0      419 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/bookmark-x-cb28f311.js
+-rw-r--r--   0        0        0      588 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/boom-box-4e291b8b.js
+-rw-r--r--   0        0        0      485 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/box-7261d0ef.js
+-rw-r--r--   0        0        0      739 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/box-select-b0ef4e91.js
+-rw-r--r--   0        0        0      340 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/brackets-fc62ae99.js
+-rw-r--r--   0        0        0      958 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/brain-cog-3d4bb4c6.js
+-rw-r--r--   0        0        0      637 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/brain-d34d8a4b.js
+-rw-r--r--   0        0        0      578 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/brick-wall-b5fb72e9.js
+-rw-r--r--   0        0        0      403 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/briefcase-f0c60756.js
+-rw-r--r--   0        0        0      488 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/bring-to-front-33a69782.js
+-rw-r--r--   0        0        0      495 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/brush-aed7dc33.js
+-rw-r--r--   0        0        0      841 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/bug-c0e4b5c7.js
+-rw-r--r--   0        0        0      722 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/bug-off-221980ea.js
+-rw-r--r--   0        0        0      741 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/bug-play-d73bf6fc.js
+-rw-r--r--   0        0        0      613 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/building-2-6f46c282.js
+-rw-r--r--   0        0        0      717 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/building-af553e71.js
+-rw-r--r--   0        0        0      622 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/bus-5900cfa3.js
+-rw-r--r--   0        0        0      623 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/bus-front-7dc8cedb.js
+-rw-r--r--   0        0        0      620 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/cable-a48206d9.js
+-rw-r--r--   0        0        0      588 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/cable-car-ec551b2e.js
+-rw-r--r--   0        0        0      665 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/cake-edd21758.js
+-rw-r--r--   0        0        0      472 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/cake-slice-9083d9b8.js
+-rw-r--r--   0        0        0      705 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/calculator-9ba50681.js
+-rw-r--r--   0        0        0      501 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/calendar-check-2-b5080d83.js
+-rw-r--r--   0        0        0      479 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/calendar-check-d1639410.js
+-rw-r--r--   0        0        0      557 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/calendar-clock-ea51db8f.js
+-rw-r--r--   0        0        0      668 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/calendar-days-ef7e5a38.js
+-rw-r--r--   0        0        0      432 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/calendar-e79a04d6.js
+-rw-r--r--   0        0        0      512 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/calendar-fold-1da81079.js
+-rw-r--r--   0        0        0      632 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/calendar-heart-5677e0b9.js
+-rw-r--r--   0        0        0      475 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/calendar-minus-2-10e1944c.js
+-rw-r--r--   0        0        0      494 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/calendar-minus-8e18db70.js
+-rw-r--r--   0        0        0      560 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/calendar-off-0bd1e591.js
+-rw-r--r--   0        0        0      511 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/calendar-plus-2-28f4ce9f.js
+-rw-r--r--   0        0        0      530 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/calendar-plus-73dc0684.js
+-rw-r--r--   0        0        0      589 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/calendar-range-83746210.js
+-rw-r--r--   0        0        0      551 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/calendar-search-02e8602b.js
+-rw-r--r--   0        0        0      511 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/calendar-x-1190d7bb.js
+-rw-r--r--   0        0        0      532 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/calendar-x-2-b568f6b9.js
+-rw-r--r--   0        0        0      423 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/camera-251bf339.js
+-rw-r--r--   0        0        0      507 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/camera-off-60b4968e.js
+-rw-r--r--   0        0        0      578 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/candlestick-chart-1765be54.js
+-rw-r--r--   0        0        0      617 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/candy-7dd2ee96.js
+-rw-r--r--   0        0        0      547 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/candy-cane-0be5742f.js
+-rw-r--r--   0        0        0      811 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/candy-off-523922e8.js
+-rw-r--r--   0        0        0      390 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/captions-41e269e3.js
+-rw-r--r--   0        0        0      537 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/captions-off-2f69fa80.js
+-rw-r--r--   0        0        0      577 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/car-d4fab838.js
+-rw-r--r--   0        0        0      574 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/car-front-a8753e88.js
+-rw-r--r--   0        0        0      614 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/car-taxi-front-7222b3f3.js
+-rw-r--r--   0        0        0      546 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/caravan-7e780ccf.js
+-rw-r--r--   0        0        0      590 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/carrot-1da699eb.js
+-rw-r--r--   0        0        0      421 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/case-lower-26d2ce81.js
+-rw-r--r--   0        0        0      425 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/case-sensitive-03494efb.js
+-rw-r--r--   0        0        0      411 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/case-upper-90d8233f.js
+-rw-r--r--   0        0        0      550 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/cassette-tape-11ee7a3e.js
+-rw-r--r--   0        0        0      493 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/cast-60db50b8.js
+-rw-r--r--   0        0        0      657 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/castle-aa353636.js
+-rw-r--r--   0        0        0      634 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/cat-b10af0e4.js
+-rw-r--r--   0        0        0      559 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/cctv-c9b74e6f.js
+-rw-r--r--   0        0        0      353 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/check-check-3fbd6fcb.js
+-rw-r--r--   0        0        0      367 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/check-circle-86d25b90.js
+-rw-r--r--   0        0        0      370 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/check-square-2-3fe1db0e.js
+-rw-r--r--   0        0        0      390 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/check-square-ca7352fc.js
+-rw-r--r--   0        0        0      458 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/chef-hat-9abd6519.js
+-rw-r--r--   0        0        0      577 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/cherry-ec8c07da.js
+-rw-r--r--   0        0        0      359 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/chevron-down-circle-ef290fe2.js
+-rw-r--r--   0        0        0      376 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/chevron-down-square-a70a006b.js
+-rw-r--r--   0        0        0      341 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/chevron-first-6730d035.js
+-rw-r--r--   0        0        0      340 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/chevron-last-69617516.js
+-rw-r--r--   0        0        0      359 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/chevron-left-circle-072df83c.js
+-rw-r--r--   0        0        0      376 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/chevron-left-square-88d1452c.js
+-rw-r--r--   0        0        0      359 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/chevron-right-circle-50d7679b.js
+-rw-r--r--   0        0        0      356 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/chevron-up-circle-50393f96.js
+-rw-r--r--   0        0        0      373 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/chevron-up-square-05a06445.js
+-rw-r--r--   0        0        0      345 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/chevrons-down-acd0eac0.js
+-rw-r--r--   0        0        0      347 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/chevrons-down-up-defb4639.js
+-rw-r--r--   0        0        0      350 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/chevrons-left-right-00bef326.js
+-rw-r--r--   0        0        0      352 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/chevrons-right-left-d128c9b7.js
+-rw-r--r--   0        0        0      346 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/chevrons-up-735bd5ef.js
+-rw-r--r--   0        0        0      537 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/chrome-214e9f29.js
+-rw-r--r--   0        0        0      523 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/church-82bb793c.js
+-rw-r--r--   0        0        0      474 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/cigarette-782cc077.js
+-rw-r--r--   0        0        0      570 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/cigarette-off-6e801ae2.js
+-rw-r--r--   0        0        0      748 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/circle-dashed-ceb50c6a.js
+-rw-r--r--   0        0        0      421 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/circle-dollar-sign-d1e628b4.js
+-rw-r--r--   0        0        0      815 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/circle-dot-dashed-0eb51089.js
+-rw-r--r--   0        0        0      429 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/circle-ellipsis-e53f5a9e.js
+-rw-r--r--   0        0        0      379 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/circle-equal-ed683c0f.js
+-rw-r--r--   0        0        0      636 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/circle-fading-plus-f5dbfc16.js
+-rw-r--r--   0        0        0      423 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/circle-off-9e5cb236.js
+-rw-r--r--   0        0        0      345 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/circle-slash-2-dcd430b1.js
+-rw-r--r--   0        0        0      359 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/circle-slash-b9a0b0c5.js
+-rw-r--r--   0        0        0      429 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/circle-user-45fedf2a.js
+-rw-r--r--   0        0        0      407 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/circle-user-round-6a9cf9c4.js
+-rw-r--r--   0        0        0      522 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/circuit-board-7cd682a8.js
+-rw-r--r--   0        0        0      517 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/citrus-f0326961.js
+-rw-r--r--   0        0        0      521 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/clapperboard-b8e90a42.js
+-rw-r--r--   0        0        0      478 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/clipboard-check-e00df14e.js
+-rw-r--r--   0        0        0      553 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/clipboard-copy-61b23095.js
+-rw-r--r--   0        0        0      585 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/clipboard-list-5426b358.js
+-rw-r--r--   0        0        0      472 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/clipboard-minus-a9a93ea5.js
+-rw-r--r--   0        0        0      520 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/clipboard-paste-ee5d0d42.js
+-rw-r--r--   0        0        0      520 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/clipboard-pen-7403e404.js
+-rw-r--r--   0        0        0      574 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/clipboard-pen-line-21803d72.js
+-rw-r--r--   0        0        0      509 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/clipboard-plus-7c095619.js
+-rw-r--r--   0        0        0      550 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/clipboard-type-f743f70a.js
+-rw-r--r--   0        0        0      509 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/clipboard-x-d56d3409.js
+-rw-r--r--   0        0        0      355 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/clock-1-b94fcef7.js
+-rw-r--r--   0        0        0      354 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/clock-10-b2753250.js
+-rw-r--r--   0        0        0      355 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/clock-11-7db4033d.js
+-rw-r--r--   0        0        0      349 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/clock-12-07ebbfa6.js
+-rw-r--r--   0        0        0      354 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/clock-2-2857fa45.js
+-rw-r--r--   0        0        0      356 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/clock-3-d8e33794.js
+-rw-r--r--   0        0        0      354 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/clock-4-ca107a0e.js
+-rw-r--r--   0        0        0      356 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/clock-5-d3688e5d.js
+-rw-r--r--   0        0        0      356 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/clock-6-21971acd.js
+-rw-r--r--   0        0        0      355 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/clock-7-8462485f.js
+-rw-r--r--   0        0        0      353 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/clock-8-d741e03a.js
+-rw-r--r--   0        0        0      355 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/clock-9-9599372b.js
+-rw-r--r--   0        0        0      353 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/clock-dc8bdde4.js
+-rw-r--r--   0        0        0      335 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/cloud-83e7cbdf.js
+-rw-r--r--   0        0        0      740 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/cloud-cog-d9e48864.js
+-rw-r--r--   0        0        0      567 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/cloud-drizzle-e9ee8e3d.js
+-rw-r--r--   0        0        0      417 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/cloud-fog-377e768a.js
+-rw-r--r--   0        0        0      570 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/cloud-hail-551a6ea9.js
+-rw-r--r--   0        0        0      394 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/cloud-lightning-c8d1996b.js
+-rw-r--r--   0        0        0      416 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/cloud-moon-d7511f0d.js
+-rw-r--r--   0        0        0      515 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/cloud-moon-rain-381e8468.js
+-rw-r--r--   0        0        0      477 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/cloud-off-063a4c1d.js
+-rw-r--r--   0        0        0      454 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/cloud-rain-338791c2.js
+-rw-r--r--   0        0        0      465 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/cloud-rain-wind-03e07aa2.js
+-rw-r--r--   0        0        0      576 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/cloud-snow-ad1d7740.js
+-rw-r--r--   0        0        0      565 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/cloud-sun-630cbe71.js
+-rw-r--r--   0        0        0      641 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/cloud-sun-rain-5249c398.js
+-rw-r--r--   0        0        0      419 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/cloudy-000fba20.js
+-rw-r--r--   0        0        0      594 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/clover-77915ed9.js
+-rw-r--r--   0        0        0      407 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/club-6ad5de20.js
+-rw-r--r--   0        0        0      412 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/code-square-044e4cc2.js
+-rw-r--r--   0        0        0      568 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/codepen-b2e8542d.js
+-rw-r--r--   0        0        0      726 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/codesandbox-7efd711a.js
+-rw-r--r--   0        0        0      538 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/coffee-05730958.js
+-rw-r--r--   0        0        0      885 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/cog-25bd7786.js
+-rw-r--r--   0        0        0      454 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/coins-bd1bf521.js
+-rw-r--r--   0        0        0      361 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/columns-2-01e62843.js
+-rw-r--r--   0        0        0      397 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/columns-3-711daf33.js
+-rw-r--r--   0        0        0      438 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/columns-4-224e3e26.js
+-rw-r--r--   0        0        0      518 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/component-a81ab53e.js
+-rw-r--r--   0        0        0      462 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/computer-71fd4536.js
+-rw-r--r--   0        0        0      458 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/concierge-bell-86061895.js
+-rw-r--r--   0        0        0      384 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/cone-2d5ac659.js
+-rw-r--r--   0        0        0      593 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/construction-fe67f2d9.js
+-rw-r--r--   0        0        0      527 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/contact-2-c389498e.js
+-rw-r--r--   0        0        0      542 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/contact-b9c1f247.js
+-rw-r--r--   0        0        0      622 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/container-8047bd33.js
+-rw-r--r--   0        0        0      361 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/contrast-2db415fc.js
+-rw-r--r--   0        0        0      534 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/cookie-5ac97459.js
+-rw-r--r--   0        0        0      510 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/cooking-pot-60655687.js
+-rw-r--r--   0        0        0      459 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/copy-check-0db8f346.js
+-rw-r--r--   0        0        0      472 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/copy-minus-f4c2e84a.js
+-rw-r--r--   0        0        0      527 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/copy-plus-cfb7c23a.js
+-rw-r--r--   0        0        0      472 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/copy-slash-f93a0eba.js
+-rw-r--r--   0        0        0      524 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/copy-x-4bc29fe8.js
+-rw-r--r--   0        0        0      364 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/copyleft-f7bf8939.js
+-rw-r--r--   0        0        0      361 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/copyright-8f6bee9b.js
+-rw-r--r--   0        0        0      368 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/corner-down-left-529b9628.js
+-rw-r--r--   0        0        0      372 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/corner-down-right-5a00b340.js
+-rw-r--r--   0        0        0      370 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/corner-left-down-a945b7bb.js
+-rw-r--r--   0        0        0      366 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/corner-left-up-f7b7a6ea.js
+-rw-r--r--   0        0        0      372 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/corner-right-down-a24df1a7.js
+-rw-r--r--   0        0        0      367 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/corner-right-up-8a587911.js
+-rw-r--r--   0        0        0      366 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/corner-up-left-2edcaa13.js
+-rw-r--r--   0        0        0      370 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/corner-up-right-bb4d22df.js
+-rw-r--r--   0        0        0      506 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/creative-commons-8a08b5bb.js
+-rw-r--r--   0        0        0      381 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/credit-card-29c50219.js
+-rw-r--r--   0        0        0      745 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/croissant-cf14f255.js
+-rw-r--r--   0        0        0      360 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/crop-ec2de7ad.js
+-rw-r--r--   0        0        0      430 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/cross-c73155d1.js
+-rw-r--r--   0        0        0      528 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/crosshair-797727d3.js
+-rw-r--r--   0        0        0      326 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/crown-b10e7ff6.js
+-rw-r--r--   0        0        0      551 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/cuboid-e2b6b17f.js
+-rw-r--r--   0        0        0      495 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/cup-soda-cd8a0720.js
+-rw-r--r--   0        0        0      522 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/currency-2f95ffaa.js
+-rw-r--r--   0        0        0      367 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/cylinder-acebbe66.js
+-rw-r--r--   0        0        0      607 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/database-backup-7e289bb9.js
+-rw-r--r--   0        0        0      513 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/database-zap-b120cb34.js
+-rw-r--r--   0        0        0      514 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/dessert-0e61f7af.js
+-rw-r--r--   0        0        0      529 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/diameter-29b4aa9b.js
+-rw-r--r--   0        0        0      419 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/diamond-a71b67ce.js
+-rw-r--r--   0        0        0      367 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/dice-1-1d647002.js
+-rw-r--r--   0        0        0      404 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/dice-2-ba43ec95.js
+-rw-r--r--   0        0        0      443 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/dice-3-eeb10f84.js
+-rw-r--r--   0        0        0      480 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/dice-4-4ab3610f.js
+-rw-r--r--   0        0        0      519 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/dice-5-1fa08684.js
+-rw-r--r--   0        0        0      557 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/dice-6-40a50ff1.js
+-rw-r--r--   0        0        0      581 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/dices-13083691.js
+-rw-r--r--   0        0        0      365 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/diff-6d4999f0.js
+-rw-r--r--   0        0        0      386 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/disc-2-eeb76b3f.js
+-rw-r--r--   0        0        0      457 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/disc-3-b8279770.js
+-rw-r--r--   0        0        0      346 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/disc-608769ee.js
+-rw-r--r--   0        0        0      407 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/disc-album-dc82f5be.js
+-rw-r--r--   0        0        0      401 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/divide-0e9b398c.js
+-rw-r--r--   0        0        0      476 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/divide-circle-8fd6d6fb.js
+-rw-r--r--   0        0        0      500 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/divide-square-6a5043a0.js
+-rw-r--r--   0        0        0      781 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/dna-6fa418fc.js
+-rw-r--r--   0        0        0      821 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/dna-off-a86c6e71.js
+-rw-r--r--   0        0        0      893 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/dog-0ed15e9a.js
+-rw-r--r--   0        0        0      393 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/dollar-sign-b3fb7040.js
+-rw-r--r--   0        0        0      419 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/donut-926b37ba.js
+-rw-r--r--   0        0        0      406 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/door-closed-f6bdacff.js
+-rw-r--r--   0        0        0      543 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/door-open-caf41777.js
+-rw-r--r--   0        0        0      373 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/dot-square-5ee42a15.js
+-rw-r--r--   0        0        0      508 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/drafting-compass-14926d84.js
+-rw-r--r--   0        0        0      733 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/drama-2aa25a7f.js
+-rw-r--r--   0        0        0      509 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/dribbble-426e96f1.js
+-rw-r--r--   0        0        0      683 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/drill-3ab18849.js
+-rw-r--r--   0        0        0      382 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/droplet-cde68b77.js
+-rw-r--r--   0        0        0      548 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/droplets-a565eb54.js
+-rw-r--r--   0        0        0      557 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/drum-0881aa6e.js
+-rw-r--r--   0        0        0      602 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/drumstick-42cc5c3b.js
+-rw-r--r--   0        0        0      530 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/dumbbell-d91d8011.js
+-rw-r--r--   0        0        0      408 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/ear-8195764e.js
+-rw-r--r--   0        0        0      614 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/ear-off-ca41fa4a.js
+-rw-r--r--   0        0        0      351 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/eclipse-d34d29e1.js
+-rw-r--r--   0        0        0      387 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/egg-355b27ab.js
+-rw-r--r--   0        0        0      466 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/egg-fried-1a418806.js
+-rw-r--r--   0        0        0      571 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/egg-off-15482582.js
+-rw-r--r--   0        0        0      363 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/equal-8d7334c3.js
+-rw-r--r--   0        0        0      420 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/equal-not-f15b9cc9.js
+-rw-r--r--   0        0        0      401 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/equal-square-baf2c6cd.js
+-rw-r--r--   0        0        0      435 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/euro-1ec53874.js
+-rw-r--r--   0        0        0      481 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/expand-6c17c5ce.js
+-rw-r--r--   0        0        0      352 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/facebook-7dbfefb3.js
+-rw-r--r--   0        0        0      479 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/factory-278a980e.js
+-rw-r--r--   0        0        0      502 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/fan-57bb5046.js
+-rw-r--r--   0        0        0      376 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/fast-forward-f4dd1b1f.js
+-rw-r--r--   0        0        0      444 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/feather-10711528.js
+-rw-r--r--   0        0        0      617 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/fence-ee593734.js
+-rw-r--r--   0        0        0      643 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/ferris-wheel-38cf8098.js
+-rw-r--r--   0        0        0      646 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/figma-7ce64fda.js
+-rw-r--r--   0        0        0      550 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/file-archive-16a981ce.js
+-rw-r--r--   0        0        0      505 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/file-audio-05e886ea.js
+-rw-r--r--   0        0        0      535 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/file-audio-2-eba1bafe.js
+-rw-r--r--   0        0        0      475 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/file-axis-3d-0081c1ce.js
+-rw-r--r--   0        0        0      504 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/file-badge-2-f715aaa5.js
+-rw-r--r--   0        0        0      506 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/file-badge-58a2164c.js
+-rw-r--r--   0        0        0      515 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/file-bar-chart-2-df4f1ba6.js
+-rw-r--r--   0        0        0      514 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/file-bar-chart-7528c81d.js
+-rw-r--r--   0        0        0      655 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/file-box-ade74692.js
+-rw-r--r--   0        0        0      430 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/file-check-2-51a06c3e.js
+-rw-r--r--   0        0        0      440 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/file-check-45bb29d8.js
+-rw-r--r--   0        0        0      471 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/file-code-2-da69ff0e.js
+-rw-r--r--   0        0        0      483 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/file-code-738bb7e0.js
+-rw-r--r--   0        0        0      750 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/file-cog-92ab8d32.js
+-rw-r--r--   0        0        0      454 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/file-diff-2674d100.js
+-rw-r--r--   0        0        0      528 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/file-digit-d190a761.js
+-rw-r--r--   0        0        0      598 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/file-heart-0e4c6049.js
+-rw-r--r--   0        0        0      522 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/file-image-ce046320.js
+-rw-r--r--   0        0        0      466 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/file-input-f082e6a0.js
+-rw-r--r--   0        0        0      577 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/file-json-2-e5f3b51f.js
+-rw-r--r--   0        0        0      589 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/file-json-bdae09ef.js
+-rw-r--r--   0        0        0      514 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/file-key-2-b0bc49ac.js
+-rw-r--r--   0        0        0      474 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/file-key-6c16592b.js
+-rw-r--r--   0        0        0      454 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/file-line-chart-289e0070.js
+-rw-r--r--   0        0        0      463 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/file-lock-06488db3.js
+-rw-r--r--   0        0        0      505 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/file-lock-2-193473d8.js
+-rw-r--r--   0        0        0      434 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/file-minus-1944d693.js
+-rw-r--r--   0        0        0      424 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/file-minus-2-2b193278.js
+-rw-r--r--   0        0        0      480 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/file-music-0cd1a5a5.js
+-rw-r--r--   0        0        0      539 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/file-output-ec885816.js
+-rw-r--r--   0        0        0      454 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/file-pen-36c525e2.js
+-rw-r--r--   0        0        0      453 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/file-pen-line-d43bdcf1.js
+-rw-r--r--   0        0        0      504 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/file-pie-chart-2d4ace9b.js
+-rw-r--r--   0        0        0      459 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/file-plus-2-adae4d0c.js
+-rw-r--r--   0        0        0      471 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/file-plus-43206f76.js
+-rw-r--r--   0        0        0      489 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/file-question-b70f12a6.js
+-rw-r--r--   0        0        0      583 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/file-scan-6d6f6d71.js
+-rw-r--r--   0        0        0      550 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/file-spreadsheet-43a79f96.js
+-rw-r--r--   0        0        0      546 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/file-stack-e4b74c5a.js
+-rw-r--r--   0        0        0      464 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/file-symlink-21eb812d.js
+-rw-r--r--   0        0        0      480 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/file-terminal-19347e68.js
+-rw-r--r--   0        0        0      512 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/file-type-c9cab45d.js
+-rw-r--r--   0        0        0      506 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/file-video-2-36068464.js
+-rw-r--r--   0        0        0      445 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/file-video-844f909b.js
+-rw-r--r--   0        0        0      486 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/file-volume-075f703a.js
+-rw-r--r--   0        0        0      544 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/file-volume-2-c5616849.js
+-rw-r--r--   0        0        0      423 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/file-warning-b060c4bf.js
+-rw-r--r--   0        0        0      464 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/file-x-2-89dcea18.js
+-rw-r--r--   0        0        0      479 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/file-x-cec4ad05.js
+-rw-r--r--   0        0        0      461 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/files-871f2c83.js
+-rw-r--r--   0        0        0      582 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/film-d24eb5d6.js
+-rw-r--r--   0        0        0      336 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/filter-9fa6eb33.js
+-rw-r--r--   0        0        0      402 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/filter-x-f7669990.js
+-rw-r--r--   0        0        0      813 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/fingerprint-d9b62aff.js
+-rw-r--r--   0        0        0      581 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/fire-extinguisher-5bccd8e3.js
+-rw-r--r--   0        0        0      791 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/fish-f12e8325.js
+-rw-r--r--   0        0        0      835 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/fish-off-a19b2443.js
+-rw-r--r--   0        0        0      318 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/fish-symbol-499225bb.js
+-rw-r--r--   0        0        0      394 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/flag-51df24ff.js
+-rw-r--r--   0        0        0      453 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/flag-off-5ac8a8ef.js
+-rw-r--r--   0        0        0      312 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/flag-triangle-left-861dad2d.js
+-rw-r--r--   0        0        0      313 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/flag-triangle-right-43e19b0e.js
+-rw-r--r--   0        0        0      453 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/flame-0df71fcf.js
+-rw-r--r--   0        0        0      474 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/flame-kindling-c943242a.js
+-rw-r--r--   0        0        0      470 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/flashlight-f560f5d8.js
+-rw-r--r--   0        0        0      506 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/flashlight-off-7ff00ae2.js
+-rw-r--r--   0        0        0      573 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/flask-conical-off-e88dcc6f.js
+-rw-r--r--   0        0        0      474 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/flask-round-7fac9eed.js
+-rw-r--r--   0        0        0      498 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/flip-horizontal-2-1ec31095.js
+-rw-r--r--   0        0        0      548 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/flip-horizontal-40d9ef22.js
+-rw-r--r--   0        0        0      503 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/flip-vertical-2-a95edc44.js
+-rw-r--r--   0        0        0      549 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/flip-vertical-57017fb6.js
+-rw-r--r--   0        0        0      617 2024-05-27 20:12:20.884250 langflow_base-0.0.49/langflow/frontend/assets/flower-2-b71a7369.js
+-rw-r--r--   0        0        0      657 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/flower-7e27e620.js
+-rw-r--r--   0        0        0      513 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/focus-119a2d2c.js
+-rw-r--r--   0        0        0      568 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/fold-horizontal-e86e541d.js
+-rw-r--r--   0        0        0      570 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/fold-vertical-b2f86633.js
+-rw-r--r--   0        0        0      542 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/folder-archive-0867c658.js
+-rw-r--r--   0        0        0      450 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/folder-check-327b635b.js
+-rw-r--r--   0        0        0      474 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/folder-clock-761d3b7d.js
+-rw-r--r--   0        0        0      446 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/folder-closed-675100c8.js
+-rw-r--r--   0        0        0      796 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/folder-cog-147353aa.js
+-rw-r--r--   0        0        0      453 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/folder-dot-148fa737.js
+-rw-r--r--   0        0        0      487 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/folder-down-b77e4f98.js
+-rw-r--r--   0        0        0      536 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/folder-git-2-179844c9.js
+-rw-r--r--   0        0        0      527 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/folder-git-c020630f.js
+-rw-r--r--   0        0        0      556 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/folder-heart-9f9ea4b3.js
+-rw-r--r--   0        0        0      488 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/folder-input-d1719b76.js
+-rw-r--r--   0        0        0      523 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/folder-kanban-a3dfd68e.js
+-rw-r--r--   0        0        0      521 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/folder-key-c4cc0892.js
+-rw-r--r--   0        0        0      514 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/folder-lock-9187bd0c.js
+-rw-r--r--   0        0        0      444 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/folder-minus-f1a446f6.js
+-rw-r--r--   0        0        0      466 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/folder-open-554eb0ff.js
+-rw-r--r--   0        0        0      519 2024-05-27 20:12:20.888251 langflow_base-0.0.49/langflow/frontend/assets/folder-open-dot-bd887495.js
+-rw-r--r--   0        0        0      490 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/folder-output-ce643418.js
+-rw-r--r--   0        0        0      461 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/folder-pen-d7c61ca8.js
+-rw-r--r--   0        0        0      491 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/folder-root-27e94b32.js
+-rw-r--r--   0        0        0      509 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/folder-search-2-eaa41b51.js
+-rw-r--r--   0        0        0      488 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/folder-search-52dccfbd.js
+-rw-r--r--   0        0        0      469 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/folder-symlink-f5605327.js
+-rw-r--r--   0        0        0      598 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/folder-sync-b7d69c14.js
+-rw-r--r--   0        0        0      653 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/folder-tree-16c062ce.js
+-rw-r--r--   0        0        0      484 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/folder-up-99d5573f.js
+-rw-r--r--   0        0        0      489 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/folder-x-34790d57.js
+-rw-r--r--   0        0        0      458 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/folders-59e58057.js
+-rw-r--r--   0        0        0      624 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/footprints-64b0ead1.js
+-rw-r--r--   0        0        0      474 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/forklift-6f97c2a0.js
+-rw-r--r--   0        0        0      471 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/frame-cff826dc.js
+-rw-r--r--   0        0        0      327 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/framer-19128747.js
+-rw-r--r--   0        0        0      470 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/frown-175ce156.js
+-rw-r--r--   0        0        0      544 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/fuel-f21d2bfd.js
+-rw-r--r--   0        0        0      535 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/fullscreen-7d7817b8.js
+-rw-r--r--   0        0        0      448 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/function-square-daa63af8.js
+-rw-r--r--   0        0        0      405 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/gallery-horizontal-cfc06fe2.js
+-rw-r--r--   0        0        0      409 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/gallery-horizontal-end-17370a66.js
+-rw-r--r--   0        0        0      479 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/gallery-thumbnails-a81776ef.js
+-rw-r--r--   0        0        0      404 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/gallery-vertical-68378ca2.js
+-rw-r--r--   0        0        0      406 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/gallery-vertical-end-2398dac0.js
+-rw-r--r--   0        0        0      795 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/gamepad-2-3ae0b330.js
+-rw-r--r--   0        0        0      549 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/gamepad-23b3ad90.js
+-rw-r--r--   0        0        0      369 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/gantt-chart-532e7888.js
+-rw-r--r--   0        0        0      440 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/gantt-chart-square-75cc145f.js
+-rw-r--r--   0        0        0      351 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/gauge-46e81e98.js
+-rw-r--r--   0        0        0      411 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/gauge-circle-d58f500a.js
+-rw-r--r--   0        0        0      476 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/gavel-b589a715.js
+-rw-r--r--   0        0        0      392 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/gem-6bb7bddc.js
+-rw-r--r--   0        0        0      437 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/ghost-63f26d11.js
+-rw-r--r--   0        0        0      449 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/git-branch-de689845.js
+-rw-r--r--   0        0        0      427 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/git-commit-horizontal-a44390ce.js
+-rw-r--r--   0        0        0      388 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/git-commit-vertical-69c30a57.js
+-rw-r--r--   0        0        0      549 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/git-compare-arrows-81eff26e.js
+-rw-r--r--   0        0        0      459 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/git-compare-ea80db52.js
+-rw-r--r--   0        0        0      517 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/git-graph-7ba52a21.js
+-rw-r--r--   0        0        0      397 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/git-merge-f2b8f827.js
+-rw-r--r--   0        0        0      462 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/git-pull-request-980e4e95.js
+-rw-r--r--   0        0        0      493 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/git-pull-request-arrow-6ca9574a.js
+-rw-r--r--   0        0        0      516 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/git-pull-request-closed-a14928c4.js
+-rw-r--r--   0        0        0      479 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/git-pull-request-create-6e51ec23.js
+-rw-r--r--   0        0        0      526 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/git-pull-request-create-arrow-08b3e525.js
+-rw-r--r--   0        0        0      489 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/git-pull-request-draft-a4f3ca06.js
+-rw-r--r--   0        0        0      550 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/gitlab-1d3a66c3.js
+-rw-r--r--   0        0        0      418 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/glass-water-5a687e2b.js
+-rw-r--r--   0        0        0      527 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/glasses-7fe19bf9.js
+-rw-r--r--   0        0        0      579 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/globe-2-47d02662.js
+-rw-r--r--   0        0        0      410 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/goal-cf06f6c3.js
+-rw-r--r--   0        0        0      631 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/grab-70e64ba1.js
+-rw-r--r--   0        0        0      506 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/graduation-cap-a0715b8d.js
+-rw-r--r--   0        0        0      714 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/grape-332f120a.js
+-rw-r--r--   0        0        0      397 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/grid-2x2-38118c1d.js
+-rw-r--r--   0        0        0      469 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/grid-3x3-09e797d0.js
+-rw-r--r--   0        0        0      675 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/grip-c338a35d.js
+-rw-r--r--   0        0        0      542 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/grip-horizontal-c47cb1ba.js
+-rw-r--r--   0        0        0      540 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/grip-vertical-da29db8f.js
+-rw-r--r--   0        0        0      681 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/guitar-2d10606f.js
+-rw-r--r--   0        0        0      584 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/hand-coins-7d87aee4.js
+-rw-r--r--   0        0        0      589 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/hand-d08db668.js
+-rw-r--r--   0        0        0      622 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/hand-heart-f341c0c6.js
+-rw-r--r--   0        0        0      496 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/hand-helping-4102a64b.js
+-rw-r--r--   0        0        0      570 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/hand-metal-4c03951f.js
+-rw-r--r--   0        0        0      605 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/hand-platter-bda84c9f.js
+-rw-r--r--   0        0        0      621 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/handshake-a314c225.js
+-rw-r--r--   0        0        0      565 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/hard-drive-2d00eab4.js
+-rw-r--r--   0        0        0      486 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/hard-drive-download-773c154d.js
+-rw-r--r--   0        0        0      485 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/hard-drive-upload-b3197ca7.js
+-rw-r--r--   0        0        0      532 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/hard-hat-4e174197.js
+-rw-r--r--   0        0        0      471 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/hash-8bc8412e.js
+-rw-r--r--   0        0        0      579 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/haze-b45745fb.js
+-rw-r--r--   0        0        0      406 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/hdmi-port-ca77cf7b.js
+-rw-r--r--   0        0        0      408 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/heading-1-9cbc51f4.js
+-rw-r--r--   0        0        0      433 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/heading-2-66c68aa3.js
+-rw-r--r--   0        0        0      508 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/heading-3-f0c7eb2b.js
+-rw-r--r--   0        0        0      443 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/heading-4-5badafef.js
+-rw-r--r--   0        0        0      500 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/heading-5-a83f7a41.js
+-rw-r--r--   0        0        0      465 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/heading-6-a058a407.js
+-rw-r--r--   0        0        0      367 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/heading-aa580ea0.js
+-rw-r--r--   0        0        0      412 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/headphones-a21f3c90.js
+-rw-r--r--   0        0        0      473 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/headset-ff8ed4da.js
+-rw-r--r--   0        0        0      471 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/heart-crack-8c09cad2.js
+-rw-r--r--   0        0        0      639 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/heart-handshake-bcbba2ba.js
+-rw-r--r--   0        0        0      539 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/heart-off-43722eb5.js
+-rw-r--r--   0        0        0      494 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/heart-pulse-2080697b.js
+-rw-r--r--   0        0        0      712 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/heater-af5de4da.js
+-rw-r--r--   0        0        0      407 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/hexagon-3757803a.js
+-rw-r--r--   0        0        0      396 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/highlighter-916684f7.js
+-rw-r--r--   0        0        0      412 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/history-de3bca16.js
+-rw-r--r--   0        0        0      924 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/hop-d889a2a4.js
+-rw-r--r--   0        0        0      877 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/hop-off-53ebd056.js
+-rw-r--r--   0        0        0      712 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/hotel-397a190d.js
+-rw-r--r--   0        0        0      535 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/hourglass-d50bf166.js
+-rw-r--r--   0        0        0      485 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/ice-cream-2-71d211f6.js
+-rw-r--r--   0        0        0      438 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/ice-cream-b7cf0f87.js
+-rw-r--r--   0        0        0      444 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/image-321ba4a1.js
+-rw-r--r--   0        0        0      549 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/image-down-f9f50798.js
+-rw-r--r--   0        0        0      515 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/image-minus-a2c5accd.js
+-rw-r--r--   0        0        0      645 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/image-off-67dff800.js
+-rw-r--r--   0        0        0      568 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/image-plus-81549658.js
+-rw-r--r--   0        0        0      499 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/images-c4d00c01.js
+-rw-r--r--   0        0        0      437 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/import-14f0b3bd.js
+-rw-r--r--   0        0        0      461 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/inbox-d74663f7.js
+-rw-r--r--   0        0        0      473 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/indent-c40b16d9.js
+-rw-r--r--   0        0        0  9622377 2024-05-27 20:12:20.940251 langflow_base-0.0.49/langflow/frontend/assets/index-5d2e85d2.js
+-rw-r--r--   0        0        0   550845 2024-05-27 20:12:20.876251 langflow_base-0.0.49/langflow/frontend/assets/index-b5c02d80.css
+-rw-r--r--   0        0        0      465 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/indian-rupee-344cad03.js
+-rw-r--r--   0        0        0      384 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/infinity-dcf96e9e.js
+-rw-r--r--   0        0        0      483 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/inspection-panel-fabca1ee.js
+-rw-r--r--   0        0        0      471 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/instagram-825f9cb0.js
+-rw-r--r--   0        0        0      419 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/italic-83cd5d13.js
+-rw-r--r--   0        0        0      391 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/iteration-ccw-8185a0f1.js
+-rw-r--r--   0        0        0      385 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/iteration-cw-092806c0.js
+-rw-r--r--   0        0        0      396 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/japanese-yen-8363e75d.js
+-rw-r--r--   0        0        0      476 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/joystick-92227220.js
+-rw-r--r--   0        0        0      365 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/kanban-f40521f4.js
+-rw-r--r--   0        0        0      435 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/kanban-square-28d851ef.js
+-rw-r--r--   0        0        0      855 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/kanban-square-dashed-011cd9c5.js
+-rw-r--r--   0        0        0      413 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/key-round-4eff9d32.js
+-rw-r--r--   0        0        0      513 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/key-square-7b7c4744.js
+-rw-r--r--   0        0        0      624 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/keyboard-music-216e0129.js
+-rw-r--r--   0        0        0      410 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/lamp-03453946.js
+-rw-r--r--   0        0        0      398 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/lamp-ceiling-ea75860a.js
+-rw-r--r--   0        0        0      478 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/lamp-desk-ca20ffd0.js
+-rw-r--r--   0        0        0      378 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/lamp-floor-22ec2b4e.js
+-rw-r--r--   0        0        0      433 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/lamp-wall-down-8a7bc680.js
+-rw-r--r--   0        0        0      432 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/lamp-wall-up-0f22083b.js
+-rw-r--r--   0        0        0      522 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/land-plot-fbcf7d50.js
+-rw-r--r--   0        0        0      582 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/landmark-c8fd19f9.js
+-rw-r--r--   0        0        0      491 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/languages-7db159c1.js
+-rw-r--r--   0        0        0      393 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/laptop-c2115f06.js
+-rw-r--r--   0        0        0      477 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/lasso-f1509c13.js
+-rw-r--r--   0        0        0      717 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/lasso-select-e5441e2c.js
+-rw-r--r--   0        0        0      483 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/laugh-fb84eb9f.js
+-rw-r--r--   0        0        0      507 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/layers-2-79243e40.js
+-rw-r--r--   0        0        0      645 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/layers-3-fa210f21.js
+-rw-r--r--   0        0        0      525 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/layout-dashboard-20091918.js
+-rw-r--r--   0        0        0      520 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/layout-grid-a5dbe99b.js
+-rw-r--r--   0        0        0      535 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/layout-list-281c03bd.js
+-rw-r--r--   0        0        0      460 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/layout-panel-left-7c72ff94.js
+-rw-r--r--   0        0        0      460 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/layout-panel-top-2b5e6a8c.js
+-rw-r--r--   0        0        0      460 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/layout-template-fc16389d.js
+-rw-r--r--   0        0        0      440 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/leaf-a45ed6c5.js
+-rw-r--r--   0        0        0      615 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/leafy-green-12a9e7f1.js
+-rw-r--r--   0        0        0      405 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/library-b6a25ede.js
+-rw-r--r--   0        0        0      495 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/library-big-5e395cde.js
+-rw-r--r--   0        0        0      441 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/library-square-2b5951f3.js
+-rw-r--r--   0        0        0      555 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/life-buoy-9b302c13.js
+-rw-r--r--   0        0        0      476 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/ligature-192d4243.js
+-rw-r--r--   0        0        0      461 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/lightbulb-a9367c75.js
+-rw-r--r--   0        0        0      531 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/lightbulb-off-a9572065.js
+-rw-r--r--   0        0        0      344 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/line-chart-cd1a1275.js
+-rw-r--r--   0        0        0      416 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/link-2-dd51ce36.js
+-rw-r--r--   0        0        0      467 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/link-2-off-63f7485d.js
+-rw-r--r--   0        0        0      469 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/linkedin-55211952.js
+-rw-r--r--   0        0        0      586 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/list-6c4583fe.js
+-rw-r--r--   0        0        0      453 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/list-checks-fd98d460.js
+-rw-r--r--   0        0        0      468 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/list-collapse-2f1fb453.js
+-rw-r--r--   0        0        0      464 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/list-end-ffe50314.js
+-rw-r--r--   0        0        0      370 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/list-filter-44feb044.js
+-rw-r--r--   0        0        0      407 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/list-minus-e3e6e4e8.js
+-rw-r--r--   0        0        0      480 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/list-music-66d7a7e0.js
+-rw-r--r--   0        0        0      559 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/list-ordered-f67a586a.js
+-rw-r--r--   0        0        0      442 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/list-plus-e0555946.js
+-rw-r--r--   0        0        0      511 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/list-restart-144e0982.js
+-rw-r--r--   0        0        0      465 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/list-start-b96debc3.js
+-rw-r--r--   0        0        0      474 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/list-todo-e01d08d1.js
+-rw-r--r--   0        0        0      473 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/list-tree-e1447981.js
+-rw-r--r--   0        0        0      416 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/list-video-1f29121a.js
+-rw-r--r--   0        0        0      443 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/list-x-3bc9ea77.js
+-rw-r--r--   0        0        0      740 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/loader-6788a7f7.js
+-rw-r--r--   0        0        0      524 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/locate-7eee1a99.js
+-rw-r--r--   0        0        0      577 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/locate-fixed-bc0164df.js
+-rw-r--r--   0        0        0      741 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/locate-off-6d1017b1.js
+-rw-r--r--   0        0        0      429 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/lock-keyhole-f04c19b7.js
+-rw-r--r--   0        0        0      433 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/log-out-0039b468.js
+-rw-r--r--   0        0        0      427 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/lollipop-df11836a.js
+-rw-r--r--   0        0        0      560 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/luggage-5d91149b.js
+-rw-r--r--   0        0        0      369 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/m-square-cee2edee.js
+-rw-r--r--   0        0        0      448 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/magnet-a7a74a3d.js
+-rw-r--r--   0        0        0      390 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/mail-590d97fd.js
+-rw-r--r--   0        0        0      458 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/mail-check-52828765.js
+-rw-r--r--   0        0        0      452 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/mail-minus-1be29beb.js
+-rw-r--r--   0        0        0      463 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/mail-open-7df531dc.js
+-rw-r--r--   0        0        0      488 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/mail-plus-07ec6f2e.js
+-rw-r--r--   0        0        0      564 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/mail-question-3e638ddf.js
+-rw-r--r--   0        0        0      577 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/mail-search-69d0fb92.js
+-rw-r--r--   0        0        0      498 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/mail-warning-670b68fc.js
+-rw-r--r--   0        0        0      489 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/mail-x-5752ee92.js
+-rw-r--r--   0        0        0      539 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/mailbox-476dc431.js
+-rw-r--r--   0        0        0      441 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/mails-34626a1b.js
+-rw-r--r--   0        0        0    23161 2024-05-27 20:12:20.876251 langflow_base-0.0.49/langflow/frontend/assets/male-technologist-d2e7de57.png
+-rw-r--r--   0        0        0      437 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/map-ce4788ee.js
+-rw-r--r--   0        0        0      374 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/map-pin-56b57fa7.js
+-rw-r--r--   0        0        0      667 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/map-pin-off-f46c49f4.js
+-rw-r--r--   0        0        0      525 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/map-pinned-b0ef6f9d.js
+-rw-r--r--   0        0        0      374 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/martini-a7add61d.js
+-rw-r--r--   0        0        0      468 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/maximize-a28fc4f1.js
+-rw-r--r--   0        0        0      610 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/medal-ae183bc6.js
+-rw-r--r--   0        0        0      367 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/megaphone-97084f20.js
+-rw-r--r--   0        0        0      480 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/megaphone-off-6b6f915d.js
+-rw-r--r--   0        0        0      469 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/meh-35cd2b47.js
+-rw-r--r--   0        0        0      702 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/memory-stick-a95af896.js
+-rw-r--r--   0        0        0      436 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/menu-square-31663887.js
+-rw-r--r--   0        0        0      401 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/merge-8e297d56.js
+-rw-r--r--   0        0        0      412 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/message-circle-code-99a33b12.js
+-rw-r--r--   0        0        0      783 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/message-circle-dashed-c3eb173d.js
+-rw-r--r--   0        0        0      460 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/message-circle-heart-d79043df.js
+-rw-r--r--   0        0        0      442 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/message-circle-more-6ef47832.js
+-rw-r--r--   0        0        0      453 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/message-circle-off-4e169269.js
+-rw-r--r--   0        0        0      398 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/message-circle-plus-81b3ef29.js
+-rw-r--r--   0        0        0      434 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/message-circle-question-38ea5e6e.js
+-rw-r--r--   0        0        0      422 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/message-circle-reply-9497c6e7.js
+-rw-r--r--   0        0        0      404 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/message-circle-warning-9bb87a42.js
+-rw-r--r--   0        0        0      398 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/message-circle-x-7d481ce0.js
+-rw-r--r--   0        0        0      441 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/message-square-code-1836bd4c.js
+-rw-r--r--   0        0        0      612 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/message-square-dashed-63e862cd.js
+-rw-r--r--   0        0        0      463 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/message-square-diff-ca6ae959.js
+-rw-r--r--   0        0        0      394 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/message-square-dot-f624eebe.js
+-rw-r--r--   0        0        0      486 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/message-square-heart-68e54d86.js
+-rw-r--r--   0        0        0      423 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/message-square-off-272fdc98.js
+-rw-r--r--   0        0        0      429 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/message-square-plus-45a0e0e9.js
+-rw-r--r--   0        0        0      464 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/message-square-quote-7ff17009.js
+-rw-r--r--   0        0        0      454 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/message-square-reply-b562c939.js
+-rw-r--r--   0        0        0      420 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/message-square-share-0964723f.js
+-rw-r--r--   0        0        0      430 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/message-square-text-99a6beef.js
+-rw-r--r--   0        0        0      435 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/message-square-warning-25b96994.js
+-rw-r--r--   0        0        0      437 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/message-square-x-a221e210.js
+-rw-r--r--   0        0        0      372 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/mic-2-861745e6.js
+-rw-r--r--   0        0        0      445 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/mic-e53d992d.js
+-rw-r--r--   0        0        0      597 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/mic-off-c97851d9.js
+-rw-r--r--   0        0        0      559 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/microscope-4c5e2ae8.js
+-rw-r--r--   0        0        0      497 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/microwave-f789cec7.js
+-rw-r--r--   0        0        0      413 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/milestone-6ad4c0c4.js
+-rw-r--r--   0        0        0      547 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/milk-17837e5c.js
+-rw-r--r--   0        0        0      607 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/milk-off-c72c2c04.js
+-rw-r--r--   0        0        0      468 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/minimize-c8e8ec56.js
+-rw-r--r--   0        0        0      341 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/minus-circle-862dbf5a.js
+-rw-r--r--   0        0        0      363 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/minus-square-6fd45698.js
+-rw-r--r--   0        0        0      434 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/monitor-a2d354bb.js
+-rw-r--r--   0        0        0      443 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/monitor-check-162a522c.js
+-rw-r--r--   0        0        0      465 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/monitor-dot-85c6e2b2.js
+-rw-r--r--   0        0        0      480 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/monitor-down-b8f60ac2.js
+-rw-r--r--   0        0        0      492 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/monitor-off-3288386e.js
+-rw-r--r--   0        0        0      475 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/monitor-pause-728f3bb5.js
+-rw-r--r--   0        0        0      443 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/monitor-play-d1bfa54a.js
+-rw-r--r--   0        0        0      500 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/monitor-smartphone-a0dca1ea.js
+-rw-r--r--   0        0        0      522 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/monitor-speaker-fbdd7793.js
+-rw-r--r--   0        0        0      457 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/monitor-stop-0610c2df.js
+-rw-r--r--   0        0        0      477 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/monitor-up-37964c1c.js
+-rw-r--r--   0        0        0      482 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/monitor-x-11e18515.js
+-rw-r--r--   0        0        0      394 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/moon-star-49802d11.js
+-rw-r--r--   0        0        0      400 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/more-vertical-7169056a.js
+-rw-r--r--   0        0        0      311 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/mountain-c7b18206.js
+-rw-r--r--   0        0        0      408 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/mountain-snow-d3a63c6f.js
+-rw-r--r--   0        0        0      357 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/mouse-5a3723fd.js
+-rw-r--r--   0        0        0      370 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/mouse-pointer-1d56851e.js
+-rw-r--r--   0        0        0      324 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/mouse-pointer-2-0788cd23.js
+-rw-r--r--   0        0        0      486 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/mouse-pointer-click-3edb0cdb.js
+-rw-r--r--   0        0        0      686 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/mouse-pointer-square-dashed-2d247999.js
+-rw-r--r--   0        0        0      409 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/mouse-pointer-square-eb41a313.js
+-rw-r--r--   0        0        0      574 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/move-300bf01c.js
+-rw-r--r--   0        0        0      417 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/move-3d-1ae965a3.js
+-rw-r--r--   0        0        0      423 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/move-diagonal-2-c4423577.js
+-rw-r--r--   0        0        0      422 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/move-diagonal-6735637c.js
+-rw-r--r--   0        0        0      341 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/move-down-7c02d5ab.js
+-rw-r--r--   0        0        0      341 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/move-down-left-ebf3a155.js
+-rw-r--r--   0        0        0      343 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/move-down-right-0cc7a6b9.js
+-rw-r--r--   0        0        0      424 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/move-horizontal-7a028148.js
+-rw-r--r--   0        0        0      338 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/move-left-2136c3cd.js
+-rw-r--r--   0        0        0      342 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/move-right-1c98b70f.js
+-rw-r--r--   0        0        0      336 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/move-up-e91955fa.js
+-rw-r--r--   0        0        0      338 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/move-up-left-bfce2b05.js
+-rw-r--r--   0        0        0      340 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/move-up-right-f530e63a.js
+-rw-r--r--   0        0        0      422 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/move-vertical-b6e59403.js
+-rw-r--r--   0        0        0      389 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/music-0ba88ffb.js
+-rw-r--r--   0        0        0      339 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/music-2-c7f1f6f0.js
+-rw-r--r--   0        0        0      336 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/music-3-472bf62b.js
+-rw-r--r--   0        0        0      428 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/music-4-d77235d5.js
+-rw-r--r--   0        0        0      324 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/navigation-2-0fbbbc5b.js
+-rw-r--r--   0        0        0      436 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/navigation-2-off-3e75af4c.js
+-rw-r--r--   0        0        0      323 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/navigation-37e1a560.js
+-rw-r--r--   0        0        0      436 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/navigation-off-8aba9e41.js
+-rw-r--r--   0        0        0      517 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/newspaper-c5cbe283.js
+-rw-r--r--   0        0        0      503 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/nfc-ba38f74c.js
+-rw-r--r--   0        0        0      504 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/notebook-df9ab14b.js
+-rw-r--r--   0        0        0      569 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/notebook-pen-2cb4fcf8.js
+-rw-r--r--   0        0        0      618 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/notebook-tabs-57108f6c.js
+-rw-r--r--   0        0        0      586 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/notebook-text-90d14136.js
+-rw-r--r--   0        0        0      542 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/notepad-text-a6008a7b.js
+-rw-r--r--   0        0        0      804 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/notepad-text-dashed-c8d9e1e3.js
+-rw-r--r--   0        0        0      769 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/nut-302b4fc7.js
+-rw-r--r--   0        0        0      880 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/nut-off-416c230b.js
+-rw-r--r--   0        0        0      364 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/octagon-3e428e17.js
+-rw-r--r--   0        0        0      334 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/option-20d51683.js
+-rw-r--r--   0        0        0      519 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/orbit-73963e9d.js
+-rw-r--r--   0        0        0      474 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/outdent-865d48e2.js
+-rw-r--r--   0        0        0      534 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/package-5282c64c.js
+-rw-r--r--   0        0        0      600 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/package-check-f94596d2.js
+-rw-r--r--   0        0        0      594 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/package-minus-87f97424.js
+-rw-r--r--   0        0        0      791 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/package-open-50313ee6.js
+-rw-r--r--   0        0        0      630 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/package-plus-4ec37a35.js
+-rw-r--r--   0        0        0      659 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/package-search-1587ffd9.js
+-rw-r--r--   0        0        0      601 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/package-x-d81f8c09.js
+-rw-r--r--   0        0        0      514 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/paint-bucket-93cba5af.js
+-rw-r--r--   0        0        0      478 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/paint-roller-fa4a2150.js
+-rw-r--r--   0        0        0      473 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/paintbrush-2-fbc3d15f.js
+-rw-r--r--   0        0        0      516 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/paintbrush-c5238598.js
+-rw-r--r--   0        0        0      638 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/palmtree-7355f6bb.js
+-rw-r--r--   0        0        0      364 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/panel-bottom-6d01fe7b.js
+-rw-r--r--   0        0        0      411 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/panel-bottom-close-fa3dda93.js
+-rw-r--r--   0        0        0      479 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/panel-bottom-dashed-65f8850c.js
+-rw-r--r--   0        0        0      410 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/panel-bottom-open-c8f7d3ef.js
+-rw-r--r--   0        0        0      361 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/panel-left-bbd543d0.js
+-rw-r--r--   0        0        0      409 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/panel-left-close-95e4a3f1.js
+-rw-r--r--   0        0        0      473 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/panel-left-dashed-f8f8ba05.js
+-rw-r--r--   0        0        0      407 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/panel-left-open-0e676308.js
+-rw-r--r--   0        0        0      363 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/panel-right-b4499943.js
+-rw-r--r--   0        0        0      409 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/panel-right-close-f7eb8bf1.js
+-rw-r--r--   0        0        0      478 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/panel-right-dashed-742b9247.js
+-rw-r--r--   0        0        0      410 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/panel-right-open-ae48eb72.js
+-rw-r--r--   0        0        0      407 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/panel-top-close-cfabbad6.js
+-rw-r--r--   0        0        0      472 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/panel-top-dashed-a8420167.js
+-rw-r--r--   0        0        0      360 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/panel-top-f1784e7f.js
+-rw-r--r--   0        0        0      407 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/panel-top-open-95b0eb41.js
+-rw-r--r--   0        0        0      405 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/panels-left-bottom-5f188146.js
+-rw-r--r--   0        0        0      407 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/panels-right-bottom-05cb76ad.js
+-rw-r--r--   0        0        0      401 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/panels-top-left-a1b25954.js
+-rw-r--r--   0        0        0      362 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/parentheses-37577a43.js
+-rw-r--r--   0        0        0      361 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/parking-circle-860c3779.js
+-rw-r--r--   0        0        0      447 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/parking-circle-off-5ae4d1ee.js
+-rw-r--r--   0        0        0      528 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/parking-meter-c3c52a07.js
+-rw-r--r--   0        0        0      383 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/parking-square-8b953717.js
+-rw-r--r--   0        0        0      544 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/parking-square-off-740bd731.js
+-rw-r--r--   0        0        0      910 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/party-popper-7f352c5a.js
+-rw-r--r--   0        0        0      372 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/pause-a3997290.js
+-rw-r--r--   0        0        0      420 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/pause-circle-384a7e9b.js
+-rw-r--r--   0        0        0      434 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/pause-octagon-dff2ebfd.js
+-rw-r--r--   0        0        0      516 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/paw-print-0e3aa68a.js
+-rw-r--r--   0        0        0      432 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/pc-case-61dbb122.js
+-rw-r--r--   0        0        0      330 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/pen-140cfa46.js
+-rw-r--r--   0        0        0      367 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/pen-line-7acae35e.js
+-rw-r--r--   0        0        0      469 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/pen-tool-7441bdca.js
+-rw-r--r--   0        0        0      658 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/pencil-ruler-c7daf67c.js
+-rw-r--r--   0        0        0      417 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/pentagon-2dbf9f1c.js
+-rw-r--r--   0        0        0      412 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/percent-0a1b4c20.js
+-rw-r--r--   0        0        0      426 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/percent-circle-6706e13b.js
+-rw-r--r--   0        0        0      551 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/percent-diamond-a221c97d.js
+-rw-r--r--   0        0        0      443 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/percent-square-9a60c93e.js
+-rw-r--r--   0        0        0      431 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/person-standing-12605d7a.js
+-rw-r--r--   0        0        0      569 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/phone-bb7af3a3.js
+-rw-r--r--   0        0        0      680 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/phone-call-a324d52a.js
+-rw-r--r--   0        0        0      685 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/phone-forwarded-7416bc2f.js
+-rw-r--r--   0        0        0      683 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/phone-incoming-45414c5f.js
+-rw-r--r--   0        0        0      683 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/phone-missed-46ce970c.js
+-rw-r--r--   0        0        0      650 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/phone-off-ef820972.js
+-rw-r--r--   0        0        0      683 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/phone-outgoing-eb5faee5.js
+-rw-r--r--   0        0        0      411 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/pi-0aab49e5.js
+-rw-r--r--   0        0        0      448 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/pi-square-bfda5f59.js
+-rw-r--r--   0        0        0      575 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/piano-3e58cbd0.js
+-rw-r--r--   0        0        0      419 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/picture-in-picture-2-532321a7.js
+-rw-r--r--   0        0        0      431 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/picture-in-picture-5275251a.js
+-rw-r--r--   0        0        0      374 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/pie-chart-9ae16dd2.js
+-rw-r--r--   0        0        0      495 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/piggy-bank-9c3bf720.js
+-rw-r--r--   0        0        0      390 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/pilcrow-a1b42cf7.js
+-rw-r--r--   0        0        0      463 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/pilcrow-square-d08b2930.js
+-rw-r--r--   0        0        0      388 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/pill-b5e5eb65.js
+-rw-r--r--   0        0        0      516 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/pin-off-7ff30ecb.js
+-rw-r--r--   0        0        0      463 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/pipette-1e962b9f.js
+-rw-r--r--   0        0        0      501 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/pizza-f0deed1d.js
+-rw-r--r--   0        0        0      476 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/plane-facec1e0.js
+-rw-r--r--   0        0        0      583 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/plane-landing-91d10c06.js
+-rw-r--r--   0        0        0      574 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/plane-takeoff-e3daa27f.js
+-rw-r--r--   0        0        0      362 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/play-circle-0a458909.js
+-rw-r--r--   0        0        0      368 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/play-square-d8f3e7a3.js
+-rw-r--r--   0        0        0      458 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/plug-2-3aeb006f.js
+-rw-r--r--   0        0        0      433 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/plug-4bf1d0a9.js
+-rw-r--r--   0        0        0      495 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/plug-zap-2-31808c4f.js
+-rw-r--r--   0        0        0      527 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/plug-zap-d1efc20e.js
+-rw-r--r--   0        0        0      414 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/pocket-64314cbf.js
+-rw-r--r--   0        0        0      504 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/podcast-5ee672fb.js
+-rw-r--r--   0        0        0      642 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/pointer-6a99de81.js
+-rw-r--r--   0        0        0      663 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/pointer-off-9f315d62.js
+-rw-r--r--   0        0        0      552 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/popcorn-e646c986.js
+-rw-r--r--   0        0        0      411 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/popsicle-62c081c9.js
+-rw-r--r--   0        0        0      428 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/pound-sterling-98b56e6d.js
+-rw-r--r--   0        0        0      348 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/power-c0b8eb1b.js
+-rw-r--r--   0        0        0      419 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/power-circle-973e2e2e.js
+-rw-r--r--   0        0        0      453 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/power-off-60f0489a.js
+-rw-r--r--   0        0        0      435 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/power-square-f3b9df9c.js
+-rw-r--r--   0        0        0      409 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/presentation-8a30976f.js
+-rw-r--r--   0        0        0      474 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/printer-01182271.js
+-rw-r--r--   0        0        0      562 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/projector-ea7a2ed4.js
+-rw-r--r--   0        0        0     1135 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/puzzle-e8df0c53.js
+-rw-r--r--   0        0        0      433 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/pyramid-42f3c2bc.js
+-rw-r--r--   0        0        0      824 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/qr-code-92db79b5.js
+-rw-r--r--   0        0        0      574 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/quote-ebbe955b.js
+-rw-r--r--   0        0        0      616 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/rabbit-ea3ddd8c.js
+-rw-r--r--   0        0        0      677 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/radar-74ff71f7.js
+-rw-r--r--   0        0        0      722 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/radiation-28ac3311.js
+-rw-r--r--   0        0        0      304 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/radical-df83abe8.js
+-rw-r--r--   0        0        0      539 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/radio-e0db86d7.js
+-rw-r--r--   0        0        0      438 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/radio-receiver-241ac64e.js
+-rw-r--r--   0        0        0      628 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/radio-tower-4dcbd4de.js
+-rw-r--r--   0        0        0      461 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/radius-4ad64aba.js
+-rw-r--r--   0        0        0      380 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/rail-symbol-6a1e3180.js
+-rw-r--r--   0        0        0      406 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/rainbow-f431fd74.js
+-rw-r--r--   0        0        0      687 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/rat-59bc794f.js
+-rw-r--r--   0        0        0      387 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/ratio-56551707.js
+-rw-r--r--   0        0        0      467 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/receipt-04f5c566.js
+-rw-r--r--   0        0        0      452 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/receipt-cent-fdbff390.js
+-rw-r--r--   0        0        0      449 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/receipt-euro-2ff548fd.js
+-rw-r--r--   0        0        0      497 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/receipt-indian-rupee-107c9f2e.js
+-rw-r--r--   0        0        0      520 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/receipt-japanese-yen-27196c83.js
+-rw-r--r--   0        0        0      499 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/receipt-pound-sterling-6a851018.js
+-rw-r--r--   0        0        0      461 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/receipt-russian-ruble-0c3bd056.js
+-rw-r--r--   0        0        0      479 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/receipt-swiss-franc-0af66aaf.js
+-rw-r--r--   0        0        0      471 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/receipt-text-d52c16dc.js
+-rw-r--r--   0        0        0      335 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/rectangle-horizontal-d5e41423.js
+-rw-r--r--   0        0        0      333 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/rectangle-vertical-ef76eb26.js
+-rw-r--r--   0        0        0      757 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/recycle-cea96532.js
+-rw-r--r--   0        0        0      383 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/redo-2-6b57c1db.js
+-rw-r--r--   0        0        0      414 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/redo-dot-acc69b3c.js
+-rw-r--r--   0        0        0      501 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/refresh-ccw-dot-2abbe1d7.js
+-rw-r--r--   0        0        0      495 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/refresh-cw-ded069ad.js
+-rw-r--r--   0        0        0      675 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/refresh-cw-off-26c765c7.js
+-rw-r--r--   0        0        0      434 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/refrigerator-bbba713d.js
+-rw-r--r--   0        0        0      485 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/regex-5f11ac98.js
+-rw-r--r--   0        0        0      459 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/remove-formatting-9056e1f7.js
+-rw-r--r--   0        0        0      487 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/repeat-1-209d375c.js
+-rw-r--r--   0        0        0      447 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/repeat-2-226af233.js
+-rw-r--r--   0        0        0      751 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/replace-all-3afafbb1.js
+-rw-r--r--   0        0        0      614 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/replace-f610ab8f.js
+-rw-r--r--   0        0        0      360 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/reply-04203a0a.js
+-rw-r--r--   0        0        0      416 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/reply-all-2f95773e.js
+-rw-r--r--   0        0        0      373 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/rewind-0dcda923.js
+-rw-r--r--   0        0        0      731 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/ribbon-30f6b81f.js
+-rw-r--r--   0        0        0    26806 2024-05-27 20:12:20.876251 langflow_base-0.0.49/langflow/frontend/assets/robot-95e1b00d.png
+-rw-r--r--   0        0        0      627 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/rocket-dd64364a.js
+-rw-r--r--   0        0        0      498 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/rocking-chair-48b0d67c.js
+-rw-r--r--   0        0        0      579 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/roller-coaster-07467718.js
+-rw-r--r--   0        0        0      575 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/rotate-3d-123855e5.js
+-rw-r--r--   0        0        0      374 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/rotate-ccw-fa2e4815.js
+-rw-r--r--   0        0        0      375 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/rotate-cw-fb2b4c62.js
+-rw-r--r--   0        0        0      424 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/route-51350f1b.js
+-rw-r--r--   0        0        0      607 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/route-off-9b0cd50f.js
+-rw-r--r--   0        0        0      554 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/router-7d73f15e.js
+-rw-r--r--   0        0        0      358 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/rows-2-db495965.js
+-rw-r--r--   0        0        0      394 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/rows-3-4bd8ea33.js
+-rw-r--r--   0        0        0      435 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/rows-4-d3b56076.js
+-rw-r--r--   0        0        0      399 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/rss-a86acff1.js
+-rw-r--r--   0        0        0      573 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/ruler-7f425ff8.js
+-rw-r--r--   0        0        0      353 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/russian-ruble-4335329e.js
+-rw-r--r--   0        0        0      413 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/sailboat-9791d947.js
+-rw-r--r--   0        0        0      651 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/salad-d5faeb52.js
+-rw-r--r--   0        0        0      585 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/sandwich-6f29208b.js
+-rw-r--r--   0        0        0      485 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/satellite-d14d025e.js
+-rw-r--r--   0        0        0      459 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/satellite-dish-b270ce57.js
+-rw-r--r--   0        0        0      423 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/scale-3d-c328b763.js
+-rw-r--r--   0        0        0      543 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/scale-f896884c.js
+-rw-r--r--   0        0        0      461 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/scaling-699b61b2.js
+-rw-r--r--   0        0        0      464 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/scan-5cd4dfc4.js
+-rw-r--r--   0        0        0      581 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/scan-barcode-566f4c1e.js
+-rw-r--r--   0        0        0      585 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/scan-eye-2473d111.js
+-rw-r--r--   0        0        0      595 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/scan-face-6b16b2e0.js
+-rw-r--r--   0        0        0      505 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/scan-line-43fa2ecd.js
+-rw-r--r--   0        0        0      561 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/scan-search-6abfbd41.js
+-rw-r--r--   0        0        0      576 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/scan-text-ee620dce.js
+-rw-r--r--   0        0        0      657 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/scatter-chart-b0552128.js
+-rw-r--r--   0        0        0      615 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/school-2-665376f7.js
+-rw-r--r--   0        0        0      544 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/school-3f78e0ab.js
+-rw-r--r--   0        0        0      570 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/scissors-line-dashed-aad245e8.js
+-rw-r--r--   0        0        0      556 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/scissors-square-75252291.js
+-rw-r--r--   0        0        0      680 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/scissors-square-dashed-bottom-1c99d312.js
+-rw-r--r--   0        0        0      500 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/screen-share-off-2bb3e9c2.js
+-rw-r--r--   0        0        0      402 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/scroll-2b74946d.js
+-rw-r--r--   0        0        0      394 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/search-check-29a560b5.js
+-rw-r--r--   0        0        0      435 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/search-code-60e5e292.js
+-rw-r--r--   0        0        0      394 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/search-slash-e352dd58.js
+-rw-r--r--   0        0        0      431 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/search-x-b5e3d1c0.js
+-rw-r--r--   0        0        0      348 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/send-horizontal-ded44ff0.js
+-rw-r--r--   0        0        0      494 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/send-to-back-c538e5c7.js
+-rw-r--r--   0        0        0      429 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/separator-horizontal-22e03055.js
+-rw-r--r--   0        0        0      427 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/separator-vertical-fb23f93d.js
+-rw-r--r--   0        0        0      513 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/server-22d39749.js
+-rw-r--r--   0        0        0      943 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/server-cog-4f664742.js
+-rw-r--r--   0        0        0      586 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/server-crash-2de8d911.js
+-rw-r--r--   0        0        0      621 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/server-off-e5302d6b.js
+-rw-r--r--   0        0        0      900 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/settings-2c5eb85f.js
+-rw-r--r--   0        0        0      492 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/shapes-ab5f60f5.js
+-rw-r--r--   0        0        0      544 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/sheet-c18d33b2.js
+-rw-r--r--   0        0        0      413 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/shell-7041f088.js
+-rw-r--r--   0        0        0      407 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/shield-alert-da301322.js
+-rw-r--r--   0        0        0      369 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/shield-ban-2f837fc2.js
+-rw-r--r--   0        0        0      374 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/shield-check-57d729e9.js
+-rw-r--r--   0        0        0      451 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/shield-ellipsis-1e4d47da.js
+-rw-r--r--   0        0        0      368 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/shield-half-7f9034e6.js
+-rw-r--r--   0        0        0      368 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/shield-minus-746917fc.js
+-rw-r--r--   0        0        0      452 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/shield-off-d0097f34.js
+-rw-r--r--   0        0        0      403 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/shield-plus-bd844eb0.js
+-rw-r--r--   0        0        0      438 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/shield-question-acee1538.js
+-rw-r--r--   0        0        0      407 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/shield-x-20fc7c07.js
+-rw-r--r--   0        0        0      625 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/ship-34376655.js
+-rw-r--r--   0        0        0      693 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/ship-wheel-5f798c44.js
+-rw-r--r--   0        0        0      461 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/shirt-40d6c417.js
+-rw-r--r--   0        0        0      425 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/shopping-bag-e264cfb5.js
+-rw-r--r--   0        0        0      584 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/shopping-basket-c496e3a3.js
+-rw-r--r--   0        0        0      461 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/shopping-cart-f7972bbc.js
+-rw-r--r--   0        0        0      445 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/shovel-87b6429e.js
+-rw-r--r--   0        0        0      671 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/shower-head-9234f682.js
+-rw-r--r--   0        0        0      479 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/shrink-a509776b.js
+-rw-r--r--   0        0        0      435 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/shrub-d5b1732e.js
+-rw-r--r--   0        0        0      559 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/shuffle-5a3cdb9d.js
+-rw-r--r--   0        0        0      307 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/sigma-2e2eac32.js
+-rw-r--r--   0        0        0      382 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/sigma-square-f9086730.js
+-rw-r--r--   0        0        0      443 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/signal-e03f8a6e.js
+-rw-r--r--   0        0        0      410 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/signal-high-3b71f87f.js
+-rw-r--r--   0        0        0      334 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/signal-low-5b3d6a00.js
+-rw-r--r--   0        0        0      375 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/signal-medium-77c8eec6.js
+-rw-r--r--   0        0        0      298 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/signal-zero-a696bbd6.js
+-rw-r--r--   0        0        0      444 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/signpost-big-d6bb07d1.js
+-rw-r--r--   0        0        0      395 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/signpost-c43dd41b.js
+-rw-r--r--   0        0        0      638 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/siren-594aae1f.js
+-rw-r--r--   0        0        0      368 2024-05-27 20:12:20.892251 langflow_base-0.0.49/langflow/frontend/assets/skip-back-3fe1b4df.js
+-rw-r--r--   0        0        0      371 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/skip-forward-1242d364.js
+-rw-r--r--   0        0        0      524 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/skull-f042a7bf.js
+-rw-r--r--   0        0        0      779 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/slack-422f1b25.js
+-rw-r--r--   0        0        0      294 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/slash-be35eeb1.js
+-rw-r--r--   0        0        0      381 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/slash-square-288167ac.js
+-rw-r--r--   0        0        0      379 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/slice-c3dad828.js
+-rw-r--r--   0        0        0      372 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/smartphone-868cca7d.js
+-rw-r--r--   0        0        0      396 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/smartphone-charging-4f1bc8af.js
+-rw-r--r--   0        0        0      520 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/smartphone-nfc-f363c1ef.js
+-rw-r--r--   0        0        0      468 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/smile-00a26bc9.js
+-rw-r--r--   0        0        0      549 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/smile-plus-5f6ed569.js
+-rw-r--r--   0        0        0      537 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/snail-da9a7766.js
+-rw-r--r--   0        0        0      537 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/sofa-2bfdf61c.js
+-rw-r--r--   0        0        0      703 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/soup-f6cf262a.js
+-rw-r--r--   0        0        0      321 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/space-798958e5.js
+-rw-r--r--   0        0        0      454 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/spade-0bbb1aa1.js
+-rw-r--r--   0        0        0      430 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/sparkle-3d5760b9.js
+-rw-r--r--   0        0        0      448 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/speaker-f7945326.js
+-rw-r--r--   0        0        0      534 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/speech-caef5ead.js
+-rw-r--r--   0        0        0      495 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/spell-check-2-e0aa4126.js
+-rw-r--r--   0        0        0      383 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/spell-check-f166dc68.js
+-rw-r--r--   0        0        0      396 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/spline-694d7ddd.js
+-rw-r--r--   0        0        0      434 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/split-94678a76.js
+-rw-r--r--   0        0        0      457 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/split-square-horizontal-62846c6f.js
+-rw-r--r--   0        0        0      455 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/split-square-vertical-d7b1a293.js
+-rw-r--r--   0        0        0      698 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/spray-can-d7810702.js
+-rw-r--r--   0        0        0      576 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/sprout-2941b7af.js
+-rw-r--r--   0        0        0      439 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/square-dashed-bottom-84130080.js
+-rw-r--r--   0        0        0      529 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/square-dashed-bottom-code-778cf01d.js
+-rw-r--r--   0        0        0      375 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/square-radical-c6519b19.js
+-rw-r--r--   0        0        0      490 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/square-stack-b7c58a9d.js
+-rw-r--r--   0        0        0      443 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/square-user-caa0b22f.js
+-rw-r--r--   0        0        0      429 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/square-user-round-6041baba.js
+-rw-r--r--   0        0        0      334 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/squircle-869daa19.js
+-rw-r--r--   0        0        0      583 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/squirrel-1f8d0f35.js
+-rw-r--r--   0        0        0      540 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/stamp-59355141.js
+-rw-r--r--   0        0        0      385 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/star-5ad6ab78.js
+-rw-r--r--   0        0        0      324 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/star-half-dd116c9e.js
+-rw-r--r--   0        0        0      473 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/star-off-54f225a7.js
+-rw-r--r--   0        0        0      365 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/step-back-96bf0f8a.js
+-rw-r--r--   0        0        0      367 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/step-forward-304ebcdc.js
+-rw-r--r--   0        0        0      513 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/stethoscope-1fa99fa8.js
+-rw-r--r--   0        0        0      538 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/sticker-144df895.js
+-rw-r--r--   0        0        0      399 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/sticky-note-2858bd4c.js
+-rw-r--r--   0        0        0      361 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/stop-circle-682b4316.js
+-rw-r--r--   0        0        0      398 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/stretch-horizontal-deaacaf3.js
+-rw-r--r--   0        0        0      396 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/stretch-vertical-d3f10b13.js
+-rw-r--r--   0        0        0      422 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/strikethrough-72878769.js
+-rw-r--r--   0        0        0      477 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/subscript-91dc6b5f.js
+-rw-r--r--   0        0        0      642 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/sun-dim-24f43cd5.js
+-rw-r--r--   0        0        0      655 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/sun-medium-820ad250.js
+-rw-r--r--   0        0        0      654 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/sun-moon-690f2196.js
+-rw-r--r--   0        0        0      699 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/sun-snow-5e3f18c5.js
+-rw-r--r--   0        0        0      594 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/sunrise-65a8ae93.js
+-rw-r--r--   0        0        0      594 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/sunset-51bf7930.js
+-rw-r--r--   0        0        0      491 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/superscript-96f8b76d.js
+-rw-r--r--   0        0        0      563 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/swatch-book-217377ae.js
+-rw-r--r--   0        0        0      373 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/swiss-franc-f2b395c5.js
+-rw-r--r--   0        0        0      533 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/switch-camera-be80e3cf.js
+-rw-r--r--   0        0        0      492 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/sword-90806a62.js
+-rw-r--r--   0        0        0      725 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/swords-bdda5651.js
+-rw-r--r--   0        0        0      536 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/syringe-530e6026.js
+-rw-r--r--   0        0        0      390 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/table-2-aa8e71c1.js
+-rw-r--r--   0        0        0      431 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/table-963e7daa.js
+-rw-r--r--   0        0        0      441 2024-05-27 20:12:20.904250 langflow_base-0.0.49/langflow/frontend/assets/table-properties-b2fc3d31.js
+-rw-r--r--   0        0        0      388 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/tablet-0916dc26.js
+-rw-r--r--   0        0        0      456 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/tablet-smartphone-8833648a.js
+-rw-r--r--   0        0        0      439 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/tablets-d1f9646c.js
+-rw-r--r--   0        0        0      501 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/tag-5ad49284.js
+-rw-r--r--   0        0        0      567 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/tags-be256b31.js
+-rw-r--r--   0        0        0      292 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/tally-1-b05cc2f6.js
+-rw-r--r--   0        0        0      328 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/tally-2-209b0771.js
+-rw-r--r--   0        0        0      365 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/tally-3-f335e9a6.js
+-rw-r--r--   0        0        0      402 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/tally-4-5aafa5e8.js
+-rw-r--r--   0        0        0      441 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/tally-5-a07599d2.js
+-rw-r--r--   0        0        0      463 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/tangent-f5131226.js
+-rw-r--r--   0        0        0      396 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/target-bbc4af84.js
+-rw-r--r--   0        0        0      791 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/telescope-f24b3ac3.js
+-rw-r--r--   0        0        0      424 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/tent-720ee227.js
+-rw-r--r--   0        0        0      546 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/tent-tree-48eb1ffa.js
+-rw-r--r--   0        0        0      431 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/test-tube-2-e828197b.js
+-rw-r--r--   0        0        0      425 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/test-tube-5c9f0b52.js
+-rw-r--r--   0        0        0      575 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/test-tubes-e92b4851.js
+-rw-r--r--   0        0        0      370 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/text-20bd10b2.js
+-rw-r--r--   0        0        0      434 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/text-cursor-d575e4f0.js
+-rw-r--r--   0        0        0      405 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/text-quote-114106c0.js
+-rw-r--r--   0        0        0      903 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/text-select-4cd99566.js
+-rw-r--r--   0        0        0      703 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/theater-a353a219.js
+-rw-r--r--   0        0        0      332 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/thermometer-e6c688d9.js
+-rw-r--r--   0        0        0      543 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/thermometer-snowflake-be8d8d4e.js
+-rw-r--r--   0        0        0      552 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/thermometer-sun-94d72684.js
+-rw-r--r--   0        0        0      478 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/thumbs-down-21e22cbc.js
+-rw-r--r--   0        0        0      478 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/thumbs-up-b0327fee.js
+-rw-r--r--   0        0        0      496 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/ticket-59ef6fa6.js
+-rw-r--r--   0        0        0      433 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/ticket-check-a63070c9.js
+-rw-r--r--   0        0        0      427 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/ticket-minus-b5a8f3d3.js
+-rw-r--r--   0        0        0      507 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/ticket-percent-d1fb44a4.js
+-rw-r--r--   0        0        0      462 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/ticket-plus-0b02434c.js
+-rw-r--r--   0        0        0      433 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/ticket-slash-c5c920d6.js
+-rw-r--r--   0        0        0      470 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/ticket-x-277ff8f5.js
+-rw-r--r--   0        0        0      413 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/timer-63ef82c8.js
+-rw-r--r--   0        0        0      515 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/timer-off-ebfa1a04.js
+-rw-r--r--   0        0        0      443 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/timer-reset-7ff7158f.js
+-rw-r--r--   0        0        0      380 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/toggle-left-23160936.js
+-rw-r--r--   0        0        0      382 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/toggle-right-fb2a1fb6.js
+-rw-r--r--   0        0        0      441 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/tornado-ecbdd395.js
+-rw-r--r--   0        0        0      374 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/torus-959c03a5.js
+-rw-r--r--   0        0        0      399 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/touchpad-6c8f5159.js
+-rw-r--r--   0        0        0      534 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/touchpad-off-14143303.js
+-rw-r--r--   0        0        0      581 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/tower-control-d0da130d.js
+-rw-r--r--   0        0        0      662 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/tractor-f0adfa2a.js
+-rw-r--r--   0        0        0      661 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/traffic-cone-62187088.js
+-rw-r--r--   0        0        0      557 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/train-front-bd9494d4.js
+-rw-r--r--   0        0        0      622 2024-05-27 20:12:20.908251 langflow_base-0.0.49/langflow/frontend/assets/train-front-tunnel-4cd69150.js
+-rw-r--r--   0        0        0      527 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/train-track-5fdf782c.js
+-rw-r--r--   0        0        0      548 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/tram-front-b7bd0d07.js
+-rw-r--r--   0        0        0      420 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/trash-548efc8e.js
+-rw-r--r--   0        0        0      436 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/tree-deciduous-3f8b1290.js
+-rw-r--r--   0        0        0      483 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/tree-pine-2b427a6d.js
+-rw-r--r--   0        0        0      546 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/trees-7698e8a4.js
+-rw-r--r--   0        0        0      444 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/trello-3ccdab69.js
+-rw-r--r--   0        0        0      382 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/trending-down-c9533d32.js
+-rw-r--r--   0        0        0      379 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/trending-up-071757ce.js
+-rw-r--r--   0        0        0      354 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/triangle-dc6903e2.js
+-rw-r--r--   0        0        0      364 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/triangle-right-023a2364.js
+-rw-r--r--   0        0        0      640 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/trophy-2d75b216.js
+-rw-r--r--   0        0        0      576 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/truck-c4b0a7fc.js
+-rw-r--r--   0        0        0      532 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/turtle-b3106944.js
+-rw-r--r--   0        0        0      356 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/tv-2-06e948fb.js
+-rw-r--r--   0        0        0      376 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/tv-360b34eb.js
+-rw-r--r--   0        0        0      321 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/twitch-7b6d926e.js
+-rw-r--r--   0        0        0      421 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/twitter-06b12afe.js
+-rw-r--r--   0        0        0      404 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/umbrella-35d823ca.js
+-rw-r--r--   0        0        0      488 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/umbrella-off-4a7736d2.js
+-rw-r--r--   0        0        0      366 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/underline-a8d39a72.js
+-rw-r--r--   0        0        0      384 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/undo-2-6ba370e2.js
+-rw-r--r--   0        0        0      412 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/undo-dot-dfc9e5ce.js
+-rw-r--r--   0        0        0     9608 2024-05-27 20:12:20.876251 langflow_base-0.0.49/langflow/frontend/assets/undraw_blog_post_re_fy5x-de7369a0.svg
+-rw-r--r--   0        0        0    10459 2024-05-27 20:12:20.876251 langflow_base-0.0.49/langflow/frontend/assets/undraw_chat_bot_re_e2gj-eceb89b6.svg
+-rw-r--r--   0        0        0    12395 2024-05-27 20:12:20.876251 langflow_base-0.0.49/langflow/frontend/assets/undraw_cloud_docs_re_xjht-c1ec41f9.svg
+-rw-r--r--   0        0        0    40053 2024-05-27 20:12:20.876251 langflow_base-0.0.49/langflow/frontend/assets/undraw_real_time_analytics_re_yliv-25632bd9.svg
+-rw-r--r--   0        0        0     5612 2024-05-27 20:12:20.876251 langflow_base-0.0.49/langflow/frontend/assets/undraw_short_bio_re_fmx0-949a7b7d.svg
+-rw-r--r--   0        0        0    11757 2024-05-27 20:12:20.876251 langflow_base-0.0.49/langflow/frontend/assets/undraw_transfer_files_re_a2a9-c499dfcb.svg
+-rw-r--r--   0        0        0      569 2024-05-27 20:12:20.916251 langflow_base-0.0.49/langflow/frontend/assets/unfold-horizontal-5cdb7854.js
+-rw-r--r--   0        0        0      572 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/unfold-vertical-98fd63f5.js
+-rw-r--r--   0        0        0      334 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/unlink-2-7b45e48d.js
+-rw-r--r--   0        0        0      703 2024-05-27 20:12:20.912251 langflow_base-0.0.49/langflow/frontend/assets/unlink-684a02e2.js
+-rw-r--r--   0        0        0      382 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/unlock-a770e507.js
+-rw-r--r--   0        0        0      433 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/unlock-keyhole-c96563d9.js
+-rw-r--r--   0        0        0      426 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/upload-cloud-b724f6cf.js
+-rw-r--r--   0        0        0      576 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/usb-4c542cb8.js
+-rw-r--r--   0        0        0      428 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/user-check-2b998463.js
+-rw-r--r--   0        0        0      757 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/user-cog-042a9c97.js
+-rw-r--r--   0        0        0      430 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/user-minus-2b419d96.js
+-rw-r--r--   0        0        0      484 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/user-plus-ef296d04.js
+-rw-r--r--   0        0        0      351 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/user-round-9678c3f1.js
+-rw-r--r--   0        0        0      407 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/user-round-check-333295c7.js
+-rw-r--r--   0        0        0      459 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/user-round-search-bf215914.js
+-rw-r--r--   0        0        0      438 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/user-round-x-b64b3a0a.js
+-rw-r--r--   0        0        0      453 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/user-search-a44398cb.js
+-rw-r--r--   0        0        0      480 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/user-x-c3cf35a7.js
+-rw-r--r--   0        0        0      479 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/users-02903511.js
+-rw-r--r--   0        0        0      439 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/utensils-60a15b68.js
+-rw-r--r--   0        0        0      536 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/utensils-crossed-8fc371ec.js
+-rw-r--r--   0        0        0      517 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/utility-pole-9d58dfcf.js
+-rw-r--r--   0        0        0      837 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/vault-038eee2a.js
+-rw-r--r--   0        0        0      444 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/vegan-05798bd6.js
+-rw-r--r--   0        0        0      514 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/venetian-mask-fe3f1aeb.js
+-rw-r--r--   0        0        0      420 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/vibrate-667e7072.js
+-rw-r--r--   0        0        0      546 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/vibrate-off-0bdf0a78.js
+-rw-r--r--   0        0        0      373 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/video-8f31a003.js
+-rw-r--r--   0        0        0      472 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/video-off-b65e7039.js
+-rw-r--r--   0        0        0      492 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/videotape-2374e735.js
+-rw-r--r--   0        0        0      549 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/view-f9e42cb1.js
+-rw-r--r--   0        0        0      404 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/voicemail-03d63f76.js
+-rw-r--r--   0        0        0      384 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/volume-1-a8dcab50.js
+-rw-r--r--   0        0        0      444 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/volume-2-51a7a1bb.js
+-rw-r--r--   0        0        0      326 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/volume-fd2fd766.js
+-rw-r--r--   0        0        0      437 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/volume-x-2cd7713a.js
+-rw-r--r--   0        0        0      405 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/vote-1ee56c91.js
+-rw-r--r--   0        0        0      425 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/wallet-1c10d16f.js
+-rw-r--r--   0        0        0      398 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/wallet-2-eb5caf85.js
+-rw-r--r--   0        0        0      502 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/wallet-cards-97bf1044.js
+-rw-r--r--   0        0        0      510 2024-05-27 20:12:20.896251 langflow_base-0.0.49/langflow/frontend/assets/wallpaper-78a97ca2.js
+-rw-r--r--   0        0        0      604 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/wand-28efcf56.js
+-rw-r--r--   0        0        0      535 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/warehouse-f82177ac.js
+-rw-r--r--   0        0        0      522 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/washing-machine-c4d18bcb.js
+-rw-r--r--   0        0        0      549 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/watch-4d03e446.js
+-rw-r--r--   0        0        0      598 2024-05-27 20:12:20.920251 langflow_base-0.0.49/langflow/frontend/assets/waves-c75c9971.js
+-rw-r--r--   0        0        0      590 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/waypoints-4f37dfb8.js
+-rw-r--r--   0        0        0     4310 2024-05-27 20:12:20.880251 langflow_base-0.0.49/langflow/frontend/assets/web-vitals-60d3425a.js
+-rw-r--r--   0        0        0      422 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/webcam-8a307428.js
+-rw-r--r--   0        0        0      527 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/webhook-9f58c70e.js
+-rw-r--r--   0        0        0      653 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/webhook-off-d5460710.js
+-rw-r--r--   0        0        0      435 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/weight-faa2a2c8.js
+-rw-r--r--   0        0        0     1055 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/wheat-0b843377.js
+-rw-r--r--   0        0        0     1103 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/wheat-off-a706bc18.js
+-rw-r--r--   0        0        0      492 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/whole-word-6a795fdb.js
+-rw-r--r--   0        0        0      455 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/wifi-46c5237a.js
+-rw-r--r--   0        0        0      634 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/wifi-off-a80416b7.js
+-rw-r--r--   0        0        0      427 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/wind-a90729e4.js
+-rw-r--r--   0        0        0      458 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/wine-7b6ca8a2.js
+-rw-r--r--   0        0        0      597 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/wine-off-9c00409f.js
+-rw-r--r--   0        0        0      475 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/wrap-text-46766bc2.js
+-rw-r--r--   0        0        0      437 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/wrench-e7dc10d8.js
+-rw-r--r--   0        0        0      440 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/x-octagon-86f69d07.js
+-rw-r--r--   0        0        0      405 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/x-square-174ee91e.js
+-rw-r--r--   0        0        0      503 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/youtube-7e2b9bd8.js
+-rw-r--r--   0        0        0      502 2024-05-27 20:12:20.928251 langflow_base-0.0.49/langflow/frontend/assets/zap-off-10dadbae.js
+-rw-r--r--   0        0        0      476 2024-05-27 20:12:20.924251 langflow_base-0.0.49/langflow/frontend/assets/zoom-in-3fb13670.js
+-rw-r--r--   0        0        0      422 2024-05-27 20:12:20.900251 langflow_base-0.0.49/langflow/frontend/assets/zoom-out-625141d6.js
+-rw-r--r--   0        0        0   104187 2024-05-27 20:12:20.876251 langflow_base-0.0.49/langflow/frontend/favicon.ico
+-rw-r--r--   0        0        0      660 2024-05-27 20:12:20.940251 langflow_base-0.0.49/langflow/frontend/index.html
+-rw-r--r--   0        0        0      322 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/graph/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/graph/edge/__init__.py
+-rw-r--r--   0        0        0     7245 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/graph/edge/base.py
+-rw-r--r--   0        0        0      989 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/graph/edge/schema.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/graph/edge/utils.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.508194 langflow_base-0.0.49/langflow/graph/graph/__init__.py
+-rw-r--r--   0        0        0    56169 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/graph/graph/base.py
+-rw-r--r--   0        0        0      866 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/graph/graph/constants.py
+-rw-r--r--   0        0        0     4649 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/graph/graph/runnable_vertices_manager.py
+-rw-r--r--   0        0        0     1589 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/graph/graph/state_manager.py
+-rw-r--r--   0        0        0     7111 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/graph/graph/utils.py
+-rw-r--r--   0        0        0     1822 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/graph/schema.py
+-rw-r--r--   0        0        0     1265 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/graph/utils.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/graph/vertex/__init__.py
+-rw-r--r--   0        0        0    29777 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/graph/vertex/base.py
+-rw-r--r--   0        0        0        1 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/graph/vertex/constants.py
+-rw-r--r--   0        0        0    10506 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/graph/vertex/types.py
+-rw-r--r--   0        0        0     1843 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/graph/vertex/utils.py
+-rw-r--r--   0        0        0      103 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/helpers/__init__.py
+-rw-r--r--   0        0        0     7078 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/helpers/flow.py
+-rw-r--r--   0        0        0     1235 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/helpers/record.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/initial_setup/__init__.py
+-rw-r--r--   0        0        0    10011 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/initial_setup/setup.py
+-rw-r--r--   0        0        0    49285 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/initial_setup/starter_projects/Basic Prompting (Hello, world!).json
+-rw-r--r--   0        0        0    60448 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/initial_setup/starter_projects/Langflow Blog Writter.json
+-rw-r--r--   0        0        0    57573 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/initial_setup/starter_projects/Langflow Document QA.json
+-rw-r--r--   0        0        0    72066 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/initial_setup/starter_projects/Langflow Memory Conversation.json
+-rw-r--r--   0        0        0   101913 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/initial_setup/starter_projects/Langflow Prompt Chaining.json
+-rw-r--r--   0        0        0   207507 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/initial_setup/starter_projects/VectorStore-RAG-Flows.json
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/interface/__init__.py
+-rw-r--r--   0        0        0       94 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/interface/importing/__init__.py
+-rw-r--r--   0        0        0      786 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/interface/importing/utils.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/interface/initialize/__init__.py
+-rw-r--r--   0        0        0      363 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/interface/initialize/llm.py
+-rw-r--r--   0        0        0     4971 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/interface/initialize/loading.py
+-rw-r--r--   0        0        0     4232 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/interface/initialize/utils.py
+-rw-r--r--   0        0        0     8548 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/interface/initialize/vector_store.py
+-rw-r--r--   0        0        0      747 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/interface/listing.py
+-rw-r--r--   0        0        0     1742 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/interface/run.py
+-rw-r--r--   0        0        0      858 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/interface/types.py
+-rw-r--r--   0        0        0     6183 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/interface/utils.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/legacy_custom/__init__.py
+-rw-r--r--   0        0        0      392 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/legacy_custom/customs.py
+-rw-r--r--   0        0        0      129 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/load/__init__.py
+-rw-r--r--   0        0        0     5170 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/load/load.py
+-rw-r--r--   0        0        0     5344 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/main.py
+-rw-r--r--   0        0        0     5205 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/memory.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/processing/__init__.py
+-rw-r--r--   0        0        0     1455 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/processing/base.py
+-rw-r--r--   0        0        0     7789 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/processing/process.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/py.typed
+-rw-r--r--   0        0        0       89 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/schema/__init__.py
+-rw-r--r--   0        0        0     2589 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/schema/dotdict.py
+-rw-r--r--   0        0        0     1307 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/schema/graph.py
+-rw-r--r--   0        0        0     6324 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/schema/schema.py
+-rw-r--r--   0        0        0     1978 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/server.py
+-rw-r--r--   0        0        0      115 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/services/auth/__init__.py
+-rw-r--r--   0        0        0      327 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/services/auth/factory.py
+-rw-r--r--   0        0        0      330 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/services/auth/service.py
+-rw-r--r--   0        0        0    12091 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/services/auth/utils.py
+-rw-r--r--   0        0        0      790 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/services/base.py
+-rw-r--r--   0        0        0      284 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/services/cache/__init__.py
+-rw-r--r--   0        0        0     4032 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/services/cache/base.py
+-rw-r--r--   0        0        0     1561 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/services/cache/factory.py
+-rw-r--r--   0        0        0    12992 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/services/cache/service.py
+-rw-r--r--   0        0        0     4752 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/services/cache/utils.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/services/chat/__init__.py
+-rw-r--r--   0        0        0     4562 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/services/chat/cache.py
+-rw-r--r--   0        0        0       45 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/services/chat/config.py
+-rw-r--r--   0        0        0      340 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/services/chat/factory.py
+-rw-r--r--   0        0        0     1374 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/services/chat/service.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/services/database/__init__.py
+-rw-r--r--   0        0        0      671 2024-05-27 20:10:52.512194 langflow_base-0.0.49/langflow/services/database/factory.py
+-rw-r--r--   0        0        0      192 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/database/models/__init__.py
+-rw-r--r--   0        0        0      146 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/database/models/api_key/__init__.py
+-rw-r--r--   0        0        0     2589 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/database/models/api_key/crud.py
+-rw-r--r--   0        0        0     1883 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/database/models/api_key/model.py
+-rw-r--r--   0        0        0      760 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/database/models/base.py
+-rw-r--r--   0        0        0      118 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/database/models/flow/__init__.py
+-rw-r--r--   0        0        0     5306 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/database/models/flow/model.py
+-rw-r--r--   0        0        0      134 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/database/models/folder/__init__.py
+-rw-r--r--   0        0        0      138 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/database/models/folder/constants.py
+-rw-r--r--   0        0        0     1750 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/database/models/folder/model.py
+-rw-r--r--   0        0        0     1014 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/database/models/folder/utils.py
+-rw-r--r--   0        0        0      137 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/database/models/user/__init__.py
+-rw-r--r--   0        0        0     2044 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/database/models/user/crud.py
+-rw-r--r--   0        0        0     2259 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/database/models/user/model.py
+-rw-r--r--   0        0        0      150 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/database/models/variable/__init__.py
+-rw-r--r--   0        0        0     2441 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/database/models/variable/model.py
+-rw-r--r--   0        0        0    11304 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/database/service.py
+-rw-r--r--   0        0        0     2643 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/database/utils.py
+-rw-r--r--   0        0        0     6735 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/deps.py
+-rw-r--r--   0        0        0     2955 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/factory.py
+-rw-r--r--   0        0        0     5383 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/manager.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/monitor/__init__.py
+-rw-r--r--   0        0        0      429 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/monitor/factory.py
+-rw-r--r--   0        0        0     6208 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/monitor/schema.py
+-rw-r--r--   0        0        0     5965 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/monitor/service.py
+-rw-r--r--   0        0        0     5754 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/monitor/utils.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/plugins/__init__.py
+-rw-r--r--   0        0        0      247 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/plugins/base.py
+-rw-r--r--   0        0        0      476 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/plugins/factory.py
+-rw-r--r--   0        0        0     2440 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/plugins/langfuse_plugin.py
+-rw-r--r--   0        0        0     2454 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/plugins/service.py
+-rw-r--r--   0        0        0      707 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/schema.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/session/__init__.py
+-rw-r--r--   0        0        0      439 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/session/factory.py
+-rw-r--r--   0        0        0     2124 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/session/service.py
+-rw-r--r--   0        0        0      516 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/session/utils.py
+-rw-r--r--   0        0        0       65 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/settings/__init__.py
+-rw-r--r--   0        0        0     4263 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/settings/auth.py
+-rw-r--r--   0        0        0    12454 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/settings/base.py
+-rw-r--r--   0        0        0      653 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/settings/constants.py
+-rw-r--r--   0        0        0      506 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/settings/factory.py
+-rw-r--r--   0        0        0     1503 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/settings/manager.py
+-rw-r--r--   0        0        0     1527 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/settings/service.py
+-rw-r--r--   0        0        0     1381 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/settings/utils.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/socket/__init__.py
+-rw-r--r--   0        0        0      472 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/socket/factory.py
+-rw-r--r--   0        0        0     2778 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/socket/service.py
+-rw-r--r--   0        0        0     3400 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/socket/utils.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/state/__init__.py
+-rw-r--r--   0        0        0      432 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/state/factory.py
+-rw-r--r--   0        0        0     2546 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/state/service.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/storage/__init__.py
+-rw-r--r--   0        0        0      955 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/storage/constants.py
+-rw-r--r--   0        0        0     1118 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/storage/factory.py
+-rw-r--r--   0        0        0     3919 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/storage/local.py
+-rw-r--r--   0        0        0     3801 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/storage/s3.py
+-rw-r--r--   0        0        0     1247 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/storage/service.py
+-rw-r--r--   0        0        0      219 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/storage/utils.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/store/__init__.py
+-rw-r--r--   0        0        0      720 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/store/exceptions.py
+-rw-r--r--   0        0        0      444 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/store/factory.py
+-rw-r--r--   0        0        0     2047 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/store/schema.py
+-rw-r--r--   0        0        0    23442 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/store/service.py
+-rw-r--r--   0        0        0     2020 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/store/utils.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/task/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/task/backends/__init__.py
+-rw-r--r--   0        0        0     2373 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/task/backends/anyio.py
+-rw-r--r--   0        0        0      307 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/task/backends/base.py
+-rw-r--r--   0        0        0      885 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/task/backends/celery.py
+-rw-r--r--   0        0        0      340 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/task/factory.py
+-rw-r--r--   0        0        0     2819 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/task/service.py
+-rw-r--r--   0        0        0      613 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/task/utils.py
+-rw-r--r--   0        0        0     6206 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/utils.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/variable/__init__.py
+-rw-r--r--   0        0        0      459 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/variable/factory.py
+-rw-r--r--   0        0        0     4996 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/services/variable/service.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/template/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/template/field/__init__.py
+-rw-r--r--   0        0        0     5001 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/template/field/base.py
+-rw-r--r--   0        0        0      376 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/template/field/prompt.py
+-rw-r--r--   0        0        0      120 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/template/frontend_node/__init__.py
+-rw-r--r--   0        0        0    11441 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/template/frontend_node/base.py
+-rw-r--r--   0        0        0     1609 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/template/frontend_node/constants.py
+-rw-r--r--   0        0        0     1706 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/template/frontend_node/custom_components.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/template/frontend_node/formatter/__init__.py
+-rw-r--r--   0        0        0      298 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/template/frontend_node/formatter/base.py
+-rw-r--r--   0        0        0     5719 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/template/frontend_node/formatter/field_formatters.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/template/template/__init__.py
+-rw-r--r--   0        0        0     2424 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/template/template/base.py
+-rw-r--r--   0        0        0        0 2024-05-27 20:10:52.516194 langflow_base-0.0.49/langflow/utils/__init__.py
+-rw-r--r--   0        0        0     5684 2024-05-27 20:10:52.520194 langflow_base-0.0.49/langflow/utils/constants.py
+-rw-r--r--   0        0        0      386 2024-05-27 20:10:52.520194 langflow_base-0.0.49/langflow/utils/lazy_load.py
+-rw-r--r--   0        0        0     3581 2024-05-27 20:10:52.520194 langflow_base-0.0.49/langflow/utils/logger.py
+-rw-r--r--   0        0        0     3154 2024-05-27 20:10:52.520194 langflow_base-0.0.49/langflow/utils/payload.py
+-rw-r--r--   0        0        0     1677 2024-05-27 20:10:52.520194 langflow_base-0.0.49/langflow/utils/schemas.py
+-rw-r--r--   0        0        0    13571 2024-05-27 20:10:52.520194 langflow_base-0.0.49/langflow/utils/util.py
+-rw-r--r--   0        0        0    10400 2024-05-27 20:10:52.520194 langflow_base-0.0.49/langflow/utils/validate.py
+-rw-r--r--   0        0        0     1081 2024-05-27 20:10:52.520194 langflow_base-0.0.49/langflow/worker.py
+-rw-r--r--   0        0        0     2396 2024-05-27 20:10:52.520194 langflow_base-0.0.49/pyproject.toml
+-rw-r--r--   0        0        0     2338 1970-01-01 00:00:00.000000 langflow_base-0.0.49/PKG-INFO
```

### Comparing `langflow_base-0.0.48/langflow/__main__.py` & `langflow_base-0.0.49/langflow/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 from rich.panel import Panel
 from rich.table import Table
 from sqlmodel import select
 
 from langflow.main import setup_app
 from langflow.services.database.models.folder.utils import create_default_folder_if_it_doesnt_exist
 from langflow.services.database.utils import session_getter
-from langflow.services.deps import get_db_service
+from langflow.services.deps import get_db_service, get_settings_service, session_scope
+from langflow.services.settings.constants import DEFAULT_SUPERUSER
 from langflow.services.utils import initialize_services
 from langflow.utils.logger import configure, logger
 from langflow.utils.util import update_settings
 
 console = Console()
 
 app = typer.Typer(no_args_is_help=True)
@@ -79,15 +80,14 @@
     timeout: int = typer.Option(300, help="Worker timeout in seconds."),
     port: int = typer.Option(7860, help="Port to listen on.", envvar="LANGFLOW_PORT"),
     components_path: Optional[Path] = typer.Option(
         Path(__file__).parent / "components",
         help="Path to the directory containing custom components.",
         envvar="LANGFLOW_COMPONENTS_PATH",
     ),
-    config: str = typer.Option(Path(__file__).parent / "config.yaml", help="Path to the configuration file."),
     # .env file param
     env_file: Path = typer.Option(None, help="Path to the .env file containing environment variables."),
     log_level: str = typer.Option("critical", help="Logging level.", envvar="LANGFLOW_LOG_LEVEL"),
     log_file: Path = typer.Option("logs/langflow.log", help="Path to the log file.", envvar="LANGFLOW_LOG_FILE"),
     cache: Optional[str] = typer.Option(
         envvar="LANGFLOW_LANGCHAIN_CACHE",
         help="Type of cache to use. (InMemoryCache, SQLiteCache)",
@@ -128,15 +128,14 @@
     set_var_for_macos_issue()
     # override env variables with .env file
 
     if env_file:
         load_dotenv(env_file, override=True)
 
     update_settings(
-        config,
         dev=dev,
         remove_api_keys=remove_api_keys,
         cache=cache,
         components_path=components_path,
         store=store,
     )
     # create path object if path is provided
@@ -506,14 +505,74 @@
     db_service = get_db_service()
     if not test:
         db_service.run_migrations()
     results = db_service.run_migrations_test()
     display_results(results)
 
 
+@app.command()
+def api_key(
+    log_level: str = typer.Option("error", help="Logging level.", envvar="LANGFLOW_LOG_LEVEL"),
+):
+    """
+    Creates an API key for the default superuser if AUTO_LOGIN is enabled.
+
+    Args:
+        log_level (str, optional): Logging level. Defaults to "error".
+
+    Returns:
+        None
+    """
+    configure(log_level=log_level)
+    initialize_services()
+    settings_service = get_settings_service()
+    auth_settings = settings_service.auth_settings
+    if not auth_settings.AUTO_LOGIN:
+        typer.echo("Auto login is disabled. API keys cannot be created through the CLI.")
+        return
+    with session_scope() as session:
+        from langflow.services.database.models.user.model import User
+
+        superuser = session.exec(select(User).where(User.username == DEFAULT_SUPERUSER)).first()
+        if not superuser:
+            typer.echo("Default superuser not found. This command requires a superuser and AUTO_LOGIN to be enabled.")
+            return
+        from langflow.services.database.models.api_key import ApiKey, ApiKeyCreate
+        from langflow.services.database.models.api_key.crud import create_api_key, delete_api_key
+
+        api_key = session.exec(select(ApiKey).where(ApiKey.user_id == superuser.id)).first()
+        if api_key:
+            delete_api_key(session, api_key.id)
+
+        api_key_create = ApiKeyCreate(name="CLI")
+        unmasked_api_key = create_api_key(session, api_key_create, user_id=superuser.id)
+        session.commit()
+        # Create a banner to display the API key and tell the user it won't be shown again
+        api_key_banner(unmasked_api_key)
+
+
+def api_key_banner(unmasked_api_key):
+    is_mac = platform.system() == "Darwin"
+    import pyperclip  # type: ignore
+
+    pyperclip.copy(unmasked_api_key.api_key)
+    panel = Panel(
+        f"[bold]API Key Created Successfully:[/bold]\n\n"
+        f"[bold blue]{unmasked_api_key.api_key}[/bold blue]\n\n"
+        "This is the only time the API key will be displayed. \n"
+        "Make sure to store it in a secure location. \n\n"
+        f"The API key has been copied to your clipboard. [bold]{['Ctrl','Cmd'][is_mac]} + V[/bold] to paste it.",
+        box=box.ROUNDED,
+        border_style="blue",
+        expand=False,
+    )
+    console = Console()
+    console.print(panel)
+
+
 def main():
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         app()
 
 
 if __name__ == "__main__":
```

### Comparing `langflow_base-0.0.48/langflow/alembic/env.py` & `langflow_base-0.0.49/langflow/alembic/env.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/script.py.mako` & `langflow_base-0.0.49/langflow/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/versions/006b3990db50_add_unique_constraints.py` & `langflow_base-0.0.49/langflow/alembic/versions/006b3990db50_add_unique_constraints.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/versions/012fb73ac359_add_folder_table.py` & `langflow_base-0.0.49/langflow/alembic/versions/012fb73ac359_add_folder_table.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/versions/0b8757876a7c_.py` & `langflow_base-0.0.49/langflow/alembic/versions/0b8757876a7c_.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/versions/1a110b568907_replace_credential_table_with_variable.py` & `langflow_base-0.0.49/langflow/alembic/versions/1a110b568907_replace_credential_table_with_variable.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/versions/1ef9c4f3765d_.py` & `langflow_base-0.0.49/langflow/alembic/versions/1ef9c4f3765d_.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/versions/1f4d6df60295_add_default_fields_column.py` & `langflow_base-0.0.49/langflow/alembic/versions/1f4d6df60295_add_default_fields_column.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/versions/260dbcc8b680_adds_tables.py` & `langflow_base-0.0.49/langflow/alembic/versions/260dbcc8b680_adds_tables.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/versions/29fe8f1f806b_add_missing_index.py` & `langflow_base-0.0.49/langflow/alembic/versions/29fe8f1f806b_add_missing_index.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/versions/2ac71eb9c3ae_adds_credential_table.py` & `langflow_base-0.0.49/langflow/alembic/versions/2ac71eb9c3ae_adds_credential_table.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/versions/4e5980a44eaa_fix_date_times_again.py` & `langflow_base-0.0.49/langflow/alembic/versions/4e5980a44eaa_fix_date_times_again.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/versions/58b28437a398_modify_nullable.py` & `langflow_base-0.0.49/langflow/alembic/versions/58b28437a398_modify_nullable.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/versions/63b9c451fd30_add_icon_and_icon_bg_color_to_flow.py` & `langflow_base-0.0.49/langflow/alembic/versions/63b9c451fd30_add_icon_and_icon_bg_color_to_flow.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/versions/67cc006d50bf_add_profile_image_column.py` & `langflow_base-0.0.49/langflow/alembic/versions/67cc006d50bf_add_profile_image_column.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/versions/6e7b581b5648_fix_nullable.py` & `langflow_base-0.0.49/langflow/alembic/versions/6e7b581b5648_fix_nullable.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/versions/7843803a87b5_store_updates.py` & `langflow_base-0.0.49/langflow/alembic/versions/7843803a87b5_store_updates.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/versions/79e675cb6752_change_datetime_type.py` & `langflow_base-0.0.49/langflow/alembic/versions/79e675cb6752_change_datetime_type.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/versions/7d2162acc8b2_adds_updated_at_and_folder_cols.py` & `langflow_base-0.0.49/langflow/alembic/versions/7d2162acc8b2_adds_updated_at_and_folder_cols.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/versions/b2fa308044b5_add_unique_constraints.py` & `langflow_base-0.0.49/langflow/alembic/versions/b2fa308044b5_add_unique_constraints.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/versions/bc2f01c40e4a_new_fixes.py` & `langflow_base-0.0.49/langflow/alembic/versions/bc2f01c40e4a_new_fixes.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/versions/c153816fd85f_set_name_and_value_to_not_nullable.py` & `langflow_base-0.0.49/langflow/alembic/versions/c153816fd85f_set_name_and_value_to_not_nullable.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/versions/e3bc869fa272_fix_nullable.py` & `langflow_base-0.0.49/langflow/alembic/versions/e3bc869fa272_fix_nullable.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/versions/eb5866d51fd2_change_columns_to_be_nullable.py` & `langflow_base-0.0.49/langflow/alembic/versions/eb5866d51fd2_change_columns_to_be_nullable.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/versions/f5ee9749d1a6_user_id_can_be_null_in_flow.py` & `langflow_base-0.0.49/langflow/alembic/versions/f5ee9749d1a6_user_id_can_be_null_in_flow.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic/versions/fd531f8868b1_fix_credential_table.py` & `langflow_base-0.0.49/langflow/alembic/versions/fd531f8868b1_fix_credential_table.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/alembic.ini` & `langflow_base-0.0.49/langflow/alembic.ini`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/api/router.py` & `langflow_base-0.0.49/langflow/api/router.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/api/utils.py` & `langflow_base-0.0.49/langflow/api/utils.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/api/v1/__init__.py` & `langflow_base-0.0.49/langflow/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/api/v1/api_key.py` & `langflow_base-0.0.49/langflow/api/v1/api_key.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/api/v1/base.py` & `langflow_base-0.0.49/langflow/api/v1/base.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/api/v1/callback.py` & `langflow_base-0.0.49/langflow/api/v1/callback.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/api/v1/chat.py` & `langflow_base-0.0.49/langflow/api/v1/chat.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/api/v1/endpoints.py` & `langflow_base-0.0.49/langflow/api/v1/endpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     ProcessResponse,
     RunResponse,
     SimplifiedAPIRequest,
     TaskStatusResponse,
     UpdateCustomComponentRequest,
     UploadFileResponse,
 )
+from langflow.custom import CustomComponent
+from langflow.custom.utils import build_custom_component_template
 from langflow.graph.graph.base import Graph
-from langflow.interface.custom.custom_component import CustomComponent
-from langflow.interface.custom.utils import build_custom_component_template
 from langflow.processing.process import process_tweaks, run_graph_internal
 from langflow.schema.graph import Tweaks
 from langflow.services.auth.utils import api_key_security, get_current_active_user
 from langflow.services.cache.utils import save_uploaded_file
 from langflow.services.database.models.flow import Flow
 from langflow.services.database.models.user.model import User
 from langflow.services.deps import get_session, get_session_service, get_settings_service, get_task_service
@@ -39,15 +39,15 @@
 def get_all(
     settings_service=Depends(get_settings_service),
 ):
     from langflow.interface.types import get_all_types_dict
 
     logger.debug("Building langchain types dict")
     try:
-        all_types_dict = get_all_types_dict(settings_service.settings.COMPONENTS_PATH)
+        all_types_dict = get_all_types_dict(settings_service.settings.components_path)
         return all_types_dict
     except Exception as exc:
         logger.exception(exc)
         raise HTTPException(status_code=500, detail=str(exc)) from exc
 
 
 @router.post("/run/{flow_id}", response_model=RunResponse, response_model_exclude_none=True)
```

### Comparing `langflow_base-0.0.48/langflow/api/v1/files.py` & `langflow_base-0.0.49/langflow/api/v1/files.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/api/v1/flows.py` & `langflow_base-0.0.49/langflow/api/v1/flows.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,18 @@
     if flow.user_id is None:
         flow.user_id = current_user.id
 
     db_flow = Flow.model_validate(flow, from_attributes=True)
     db_flow.updated_at = datetime.now(timezone.utc)
 
     if db_flow.folder_id is None:
-        default_folder = session.exec(select(Folder).where(Folder.name == DEFAULT_FOLDER_NAME)).first()
+        # Make sure flows always have a folder
+        default_folder = session.exec(
+            select(Folder).where(Folder.name == DEFAULT_FOLDER_NAME, Folder.user_id == current_user.id)
+        ).first()
         if default_folder:
             db_flow.folder_id = default_folder.id
 
     session.add(db_flow)
     session.commit()
     session.refresh(db_flow)
     return db_flow
@@ -123,15 +126,15 @@
         flow_id=flow_id,
         current_user=current_user,
         settings_service=settings_service,
     )
     if not db_flow:
         raise HTTPException(status_code=404, detail="Flow not found")
     flow_data = flow.model_dump(exclude_unset=True)
-    if settings_service.settings.REMOVE_API_KEYS:
+    if settings_service.settings.remove_api_keys:
         flow_data = remove_api_keys(flow_data)
     for key, value in flow_data.items():
         if value is not None:
             setattr(db_flow, key, value)
     db_flow.updated_at = datetime.now(timezone.utc)
     if db_flow.folder_id is None:
         default_folder = session.exec(select(Folder).where(Folder.name == DEFAULT_FOLDER_NAME)).first()
```

### Comparing `langflow_base-0.0.48/langflow/api/v1/folders.py` & `langflow_base-0.0.49/langflow/api/v1/folders.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/api/v1/login.py` & `langflow_base-0.0.49/langflow/api/v1/login.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/api/v1/monitor.py` & `langflow_base-0.0.49/langflow/api/v1/monitor.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/api/v1/schemas.py` & `langflow_base-0.0.49/langflow/api/v1/schemas.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/api/v1/store.py` & `langflow_base-0.0.49/langflow/api/v1/store.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 
 @router.get("/check/")
 def check_if_store_is_enabled(
     settings_service=Depends(get_settings_service),
 ):
     return {
-        "enabled": settings_service.settings.STORE,
+        "enabled": settings_service.settings.store,
     }
 
 
 @router.get("/check/api_key")
 async def check_if_store_has_api_key(
     api_key: Optional[str] = Depends(get_optional_user_store_api_key),
     store_service: StoreService = Depends(get_store_service),
```

### Comparing `langflow_base-0.0.48/langflow/api/v1/users.py` & `langflow_base-0.0.49/langflow/api/v1/users.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/api/v1/validate.py` & `langflow_base-0.0.49/langflow/api/v1/validate.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/api/v1/variable.py` & `langflow_base-0.0.49/langflow/api/v1/variable.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/base/agents/agent.py` & `langflow_base-0.0.49/langflow/base/agents/agent.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/base/agents/default_prompts.py` & `langflow_base-0.0.49/langflow/base/agents/default_prompts.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/base/agents/utils.py` & `langflow_base-0.0.49/langflow/base/agents/utils.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/base/constants.py` & `langflow_base-0.0.49/langflow/base/constants.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/base/data/utils.py` & `langflow_base-0.0.49/langflow/base/data/utils.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/base/io/chat.py` & `langflow_base-0.0.49/langflow/base/io/chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional, Union
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import Text
 from langflow.helpers.record import records_to_text
-from langflow.interface.custom.custom_component import CustomComponent
 from langflow.memory import store_message
 from langflow.schema import Record
 
 
 class ChatComponent(CustomComponent):
     display_name = "Chat Component"
     description = "Use as base for chat components."
```

### Comparing `langflow_base-0.0.48/langflow/base/io/text.py` & `langflow_base-0.0.49/langflow/base/io/text.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import Text
 from langflow.helpers.record import records_to_text
-from langflow.interface.custom.custom_component import CustomComponent
 from langflow.schema.schema import Record
 
 
 class TextComponent(CustomComponent):
     display_name = "Text Component"
     description = "Used to pass text to the next component."
```

### Comparing `langflow_base-0.0.48/langflow/base/memory/memory.py` & `langflow_base-0.0.49/langflow/base/memory/memory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 from langflow.schema.schema import Record
 
 
 class BaseMemoryComponent(CustomComponent):
     display_name = "Chat Memory"
     description = "Retrieves stored chat messages given a specific Session ID."
     beta: bool = True
```

### Comparing `langflow_base-0.0.48/langflow/base/models/model.py` & `langflow_base-0.0.49/langflow/base/models/model.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/base/prompts/api_utils.py` & `langflow_base-0.0.49/langflow/base/prompts/api_utils.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/base/prompts/utils.py` & `langflow_base-0.0.49/langflow/base/prompts/utils.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/base/tools/base.py` & `langflow_base-0.0.49/langflow/base/tools/base.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/agents/AgentInitializer.py` & `langflow_base-0.0.49/langflow/components/agents/ToolCallingAgent.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,64 @@
-from typing import Callable, List, Optional, Union
+from typing import List, Optional
 
-from langchain.agents import AgentExecutor, AgentType, initialize_agent, types
+from langchain.agents.tool_calling_agent.base import create_tool_calling_agent
+from langchain_core.prompts import ChatPromptTemplate
 
-from langflow.field_typing import BaseChatMemory, BaseLanguageModel, Tool
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.base.agents.agent import LCAgentComponent
+from langflow.field_typing import BaseLanguageModel, Text, Tool
+from langflow.schema.schema import Record
 
 
-class AgentInitializerComponent(CustomComponent):
-    display_name: str = "Agent Initializer"
-    description: str = "Initialize a Langchain Agent."
-    documentation: str = "https://python.langchain.com/docs/modules/agents/agent_types/"
+class ToolCallingAgentComponent(LCAgentComponent):
+    display_name: str = "Tool Calling Agent"
+    description: str = "Agent that uses tools. Only models that are compatible with function calling are supported."
 
     def build_config(self):
-        agents = list(types.AGENT_TO_CLASS.keys())
-        # field_type and required are optional
         return {
-            "agent": {"options": agents, "value": agents[0], "display_name": "Agent Type"},
-            "max_iterations": {"display_name": "Max Iterations", "value": 10},
-            "memory": {"display_name": "Memory"},
+            "llm": {"display_name": "LLM"},
             "tools": {"display_name": "Tools"},
-            "llm": {"display_name": "Language Model"},
-            "code": {"advanced": True},
+            "user_prompt": {
+                "display_name": "Prompt",
+                "multiline": True,
+                "info": "This prompt must contain 'input' key.",
+            },
+            "handle_parsing_errors": {
+                "display_name": "Handle Parsing Errors",
+                "info": "If True, the agent will handle parsing errors. If False, the agent will raise an error.",
+                "advanced": True,
+            },
+            "memory": {
+                "display_name": "Memory",
+                "info": "Memory to use for the agent.",
+            },
+            "input_value": {
+                "display_name": "Inputs",
+                "info": "Input text to pass to the agent.",
+            },
         }
 
-    def build(
+    async def build(
         self,
-        agent: str,
+        input_value: str,
         llm: BaseLanguageModel,
         tools: List[Tool],
-        max_iterations: int,
-        memory: Optional[BaseChatMemory] = None,
-    ) -> Union[AgentExecutor, Callable]:
-        agent = AgentType(agent)
-        if memory:
-            return initialize_agent(
-                tools=tools,
-                llm=llm,
-                agent=agent,
-                memory=memory,
-                return_intermediate_steps=True,
-                handle_parsing_errors=True,
-                max_iterations=max_iterations,
-            )
-        return initialize_agent(
-            tools=tools,
-            llm=llm,
-            agent=agent,
-            return_intermediate_steps=True,
-            handle_parsing_errors=True,
-            max_iterations=max_iterations,
-        )
+        user_prompt: str = "{input}",
+        message_history: Optional[List[Record]] = None,
+        system_message: str = "You are a helpful assistant",
+        handle_parsing_errors: bool = True,
+    ) -> Text:
+        if "input" not in user_prompt:
+            raise ValueError("Prompt must contain 'input' key.")
+        messages = [
+            ("system", system_message),
+            (
+                "placeholder",
+                "{chat_history}",
+            ),
+            ("human", user_prompt),
+            ("placeholder", "{agent_scratchpad}"),
+        ]
+        prompt = ChatPromptTemplate.from_messages(messages)
+        agent = create_tool_calling_agent(llm, tools, prompt)
+        result = await self.run_agent(agent, input_value, tools, message_history, handle_parsing_errors)
+        self.status = result
+        return result
```

### Comparing `langflow_base-0.0.48/langflow/components/agents/CSVAgent.py` & `langflow_base-0.0.49/langflow/components/agents/CSVAgent.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/agents/JsonAgent.py` & `langflow_base-0.0.49/langflow/components/agents/JsonAgent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from langchain.agents import AgentExecutor
+from langchain_community.agent_toolkits import create_json_agent
 from langchain_community.agent_toolkits.json.toolkit import JsonToolkit
 
-from langflow.field_typing import (
-    BaseLanguageModel,
-)
-from langflow.interface.custom.custom_component import CustomComponent
-from langchain_community.agent_toolkits import create_json_agent
+from langflow.custom import CustomComponent
+from langflow.field_typing import BaseLanguageModel
 
 
 class JsonAgentComponent(CustomComponent):
     display_name = "JsonAgent"
     description = "Construct a json agent from an LLM and tools."
 
     def build_config(self):
```

### Comparing `langflow_base-0.0.48/langflow/components/agents/OpenAIConversationalAgent.py` & `langflow_base-0.0.49/langflow/components/models/OpenAIModel.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,105 @@
-from typing import List, Optional
+from typing import Optional
 
-from langchain.agents.agent import AgentExecutor
-from langchain.agents.agent_toolkits.conversational_retrieval.openai_functions import _get_default_system_message
-from langchain.agents.openai_functions_agent.base import OpenAIFunctionsAgent
-from langchain.memory.token_buffer import ConversationTokenBufferMemory
 from langchain_openai import ChatOpenAI
-
-from langflow.field_typing.range_spec import RangeSpec
-from langflow.interface.custom.custom_component import CustomComponent
 from pydantic.v1 import SecretStr
-from langchain_core.memory import BaseMemory
-from langchain_core.prompts import MessagesPlaceholder, SystemMessagePromptTemplate
-from langchain_core.tools import Tool
+
+from langflow.base.constants import STREAM_INFO_TEXT
+from langflow.base.models.model import LCModelComponent
+from langflow.base.models.openai_constants import MODEL_NAMES
+from langflow.field_typing import NestedDict, Text
 
 
-class ConversationalAgent(CustomComponent):
-    display_name: str = "OpenAI Conversational Agent"
-    description: str = "Conversational Agent that can use OpenAI's function calling API"
+class OpenAIModelComponent(LCModelComponent):
+    display_name = "OpenAI"
+    description = "Generates text using OpenAI LLMs."
     icon = "OpenAI"
 
+    field_order = [
+        "max_tokens",
+        "model_kwargs",
+        "model_name",
+        "openai_api_base",
+        "openai_api_key",
+        "temperature",
+        "input_value",
+        "system_message",
+        "stream",
+    ]
+
     def build_config(self):
-        openai_function_models = [
-            "gpt-4-turbo-preview",
-            "gpt-4-0125-preview",
-            "gpt-4-1106-preview",
-            "gpt-4-vision-preview",
-            "gpt-3.5-turbo-0125",
-            "gpt-3.5-turbo-1106",
-        ]
         return {
-            "tools": {"display_name": "Tools"},
-            "memory": {"display_name": "Memory"},
-            "system_message": {"display_name": "System Message"},
-            "max_token_limit": {"display_name": "Max Token Limit"},
+            "input_value": {"display_name": "Input"},
+            "max_tokens": {
+                "display_name": "Max Tokens",
+                "advanced": True,
+                "info": "The maximum number of tokens to generate. Set to 0 for unlimited tokens.",
+            },
+            "model_kwargs": {
+                "display_name": "Model Kwargs",
+                "advanced": True,
+            },
             "model_name": {
                 "display_name": "Model Name",
-                "options": openai_function_models,
-                "value": openai_function_models[0],
+                "advanced": False,
+                "options": MODEL_NAMES,
+            },
+            "openai_api_base": {
+                "display_name": "OpenAI API Base",
+                "advanced": True,
+                "info": (
+                    "The base URL of the OpenAI API. Defaults to https://api.openai.com/v1.\n\n"
+                    "You can change this to use other APIs like JinaChat, LocalAI and Prem."
+                ),
+            },
+            "openai_api_key": {
+                "display_name": "OpenAI API Key",
+                "info": "The OpenAI API Key to use for the OpenAI model.",
+                "advanced": False,
+                "password": True,
             },
-            "code": {"show": False},
             "temperature": {
                 "display_name": "Temperature",
-                "value": 0.2,
-                "rangeSpec": RangeSpec(min=0, max=2, step=0.1),
+                "advanced": False,
+                "value": 0.1,
+            },
+            "stream": {
+                "display_name": "Stream",
+                "info": STREAM_INFO_TEXT,
+                "advanced": True,
+            },
+            "system_message": {
+                "display_name": "System Message",
+                "info": "System message to pass to the model.",
+                "advanced": True,
             },
         }
 
     def build(
         self,
-        model_name: str,
+        input_value: Text,
         openai_api_key: str,
-        tools: List[Tool],
+        temperature: float,
+        model_name: str = "gpt-4o",
+        max_tokens: Optional[int] = 256,
+        model_kwargs: NestedDict = {},
         openai_api_base: Optional[str] = None,
-        memory: Optional[BaseMemory] = None,
-        system_message: Optional[SystemMessagePromptTemplate] = None,
-        max_token_limit: int = 2000,
-        temperature: float = 0.9,
-    ) -> AgentExecutor:
+        stream: bool = False,
+        system_message: Optional[str] = None,
+    ) -> Text:
+        if not openai_api_base:
+            openai_api_base = "https://api.openai.com/v1"
         if openai_api_key:
             api_key = SecretStr(openai_api_key)
         else:
             api_key = None
 
-        llm = ChatOpenAI(
+        output = ChatOpenAI(
+            max_tokens=max_tokens or None,
+            model_kwargs=model_kwargs,
             model=model_name,
-            api_key=api_key,
             base_url=openai_api_base,
-            max_tokens=max_token_limit,
+            api_key=api_key,
             temperature=temperature,
         )
-        if not memory:
-            memory_key = "chat_history"
-            memory = ConversationTokenBufferMemory(
-                memory_key=memory_key,
-                return_messages=True,
-                output_key="output",
-                llm=llm,
-                max_token_limit=max_token_limit,
-            )
-        else:
-            memory_key = memory.memory_key  # type: ignore
 
-        _system_message = system_message or _get_default_system_message()
-        prompt = OpenAIFunctionsAgent.create_prompt(
-            system_message=_system_message,  # type: ignore
-            extra_prompt_messages=[MessagesPlaceholder(variable_name=memory_key)],
-        )
-        agent = OpenAIFunctionsAgent(
-            llm=llm,
-            tools=tools,
-            prompt=prompt,  # type: ignore
-        )
-        return AgentExecutor(
-            agent=agent,
-            tools=tools,  # type: ignore
-            memory=memory,
-            verbose=True,
-            return_intermediate_steps=True,
-            handle_parsing_errors=True,
-        )
+        return self.get_chat_result(output, stream, input_value, system_message)
```

### Comparing `langflow_base-0.0.48/langflow/components/agents/SQLAgent.py` & `langflow_base-0.0.49/langflow/components/agents/SQLAgent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Callable, Union
 
 from langchain.agents import AgentExecutor
-from langchain_community.utilities import SQLDatabase
 from langchain_community.agent_toolkits import SQLDatabaseToolkit
 from langchain_community.agent_toolkits.sql.base import create_sql_agent
+from langchain_community.utilities import SQLDatabase
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import BaseLanguageModel
-from langflow.interface.custom.custom_component import CustomComponent
 
 
 class SQLAgentComponent(CustomComponent):
     display_name = "SQLAgent"
     description = "Construct an SQL agent from an LLM and tools."
 
     def build_config(self):
```

### Comparing `langflow_base-0.0.48/langflow/components/agents/ToolCallingAgent.py` & `langflow_base-0.0.49/langflow/components/memories/AstraDBMessageReader.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,91 @@
-from typing import List, Optional
+from typing import Optional, cast
 
-from langchain.agents.tool_calling_agent.base import create_tool_calling_agent
-from langchain_core.prompts import ChatPromptTemplate
+from langchain_astradb.chat_message_histories import AstraDBChatMessageHistory
 
-from langflow.base.agents.agent import LCAgentComponent
-from langflow.field_typing import BaseLanguageModel, Text, Tool
+from langflow.base.memory.memory import BaseMemoryComponent
+from langflow.field_typing import Text
 from langflow.schema.schema import Record
 
 
-class ToolCallingAgentComponent(LCAgentComponent):
-    display_name: str = "Tool Calling Agent"
-    description: str = "Agent that uses tools. Only models that are compatible with function calling are supported."
+class AstraDBMessageReaderComponent(BaseMemoryComponent):
+    display_name = "Astra DB Message Reader"
+    description = "Retrieves stored chat messages from Astra DB."
 
     def build_config(self):
         return {
-            "llm": {"display_name": "LLM"},
-            "tools": {"display_name": "Tools"},
-            "user_prompt": {
-                "display_name": "Prompt",
-                "multiline": True,
-                "info": "This prompt must contain 'input' key.",
+            "session_id": {
+                "display_name": "Session ID",
+                "info": "Session ID of the chat history.",
+                "input_types": ["Text"],
             },
-            "handle_parsing_errors": {
-                "display_name": "Handle Parsing Errors",
-                "info": "If True, the agent will handle parsing errors. If False, the agent will raise an error.",
-                "advanced": True,
+            "collection_name": {
+                "display_name": "Collection Name",
+                "info": "Collection name for Astra DB.",
+                "input_types": ["Text"],
+            },
+            "token": {
+                "display_name": "Astra DB Application Token",
+                "info": "Token for the Astra DB instance.",
+                "password": True,
             },
-            "memory": {
-                "display_name": "Memory",
-                "info": "Memory to use for the agent.",
+            "api_endpoint": {
+                "display_name": "Astra DB API Endpoint",
+                "info": "API Endpoint for the Astra DB instance.",
+                "password": True,
             },
-            "input_value": {
-                "display_name": "Inputs",
-                "info": "Input text to pass to the agent.",
+            "namespace": {
+                "display_name": "Namespace",
+                "info": "Namespace for the Astra DB instance.",
+                "input_types": ["Text"],
+                "advanced": True,
             },
         }
 
-    async def build(
+    def get_messages(self, **kwargs) -> list[Record]:
+        """
+        Retrieves messages from the AstraDBChatMessageHistory memory.
+
+        Args:
+            memory (AstraDBChatMessageHistory): The AstraDBChatMessageHistory instance to retrieve messages from.
+
+        Returns:
+            list[Record]: A list of Record objects representing the search results.
+        """
+        memory: AstraDBChatMessageHistory = cast(AstraDBChatMessageHistory, kwargs.get("memory"))
+        if not memory:
+            raise ValueError("AstraDBChatMessageHistory instance is required.")
+
+        # Get messages from the memory
+        messages = memory.messages
+        results = [Record.from_lc_message(message) for message in messages]
+
+        return list(results)
+
+    def build(
         self,
-        input_value: str,
-        llm: BaseLanguageModel,
-        tools: List[Tool],
-        user_prompt: str = "{input}",
-        message_history: Optional[List[Record]] = None,
-        system_message: str = "You are a helpful assistant",
-        handle_parsing_errors: bool = True,
-    ) -> Text:
-        if "input" not in user_prompt:
-            raise ValueError("Prompt must contain 'input' key.")
-        messages = [
-            ("system", system_message),
-            (
-                "placeholder",
-                "{chat_history}",
-            ),
-            ("human", user_prompt),
-            ("placeholder", "{agent_scratchpad}"),
-        ]
-        prompt = ChatPromptTemplate.from_messages(messages)
-        agent = create_tool_calling_agent(llm, tools, prompt)
-        result = await self.run_agent(agent, input_value, tools, message_history, handle_parsing_errors)
-        self.status = result
-        return result
+        session_id: Text,
+        collection_name: str,
+        token: str,
+        api_endpoint: str,
+        namespace: Optional[str] = None,
+    ) -> list[Record]:
+        try:
+            pass
+        except ImportError:
+            raise ImportError(
+                "Could not import langchain Astra DB integration package. "
+                "Please install it with `pip install langchain-astradb`."
+            )
+
+        memory = AstraDBChatMessageHistory(
+            session_id=session_id,
+            collection_name=collection_name,
+            token=token,
+            api_endpoint=api_endpoint,
+            namespace=namespace,
+        )
+
+        records = self.get_messages(memory=memory)
+        self.status = records
+
+        return records
```

### Comparing `langflow_base-0.0.48/langflow/components/agents/VectorStoreAgent.py` & `langflow_base-0.0.49/langflow/components/agents/VectorStoreAgent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Callable, Union
 
 from langchain.agents import AgentExecutor, create_vectorstore_agent
 from langchain.agents.agent_toolkits.vectorstore.toolkit import VectorStoreToolkit
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import BaseLanguageModel
-from langflow.interface.custom.custom_component import CustomComponent
 
 
 class VectorStoreAgentComponent(CustomComponent):
     display_name = "VectorStoreAgent"
     description = "Construct an agent from a Vector Store."
 
     def build_config(self):
```

### Comparing `langflow_base-0.0.48/langflow/components/agents/VectorStoreRouterAgent.py` & `langflow_base-0.0.49/langflow/components/agents/VectorStoreRouterAgent.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Callable
 
 from langchain.agents import create_vectorstore_router_agent
 from langchain.agents.agent_toolkits.vectorstore.toolkit import VectorStoreRouterToolkit
 from langchain_core.language_models.base import BaseLanguageModel
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 
 
 class VectorStoreRouterAgentComponent(CustomComponent):
     display_name = "VectorStoreRouterAgent"
     description = "Construct an agent from a Vector Store Router."
 
     def build_config(self):
```

### Comparing `langflow_base-0.0.48/langflow/components/agents/XMLAgent.py` & `langflow_base-0.0.49/langflow/components/agents/XMLAgent.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/agents/__init__.py` & `langflow_base-0.0.49/langflow/components/toolkits/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-from .AgentInitializer import AgentInitializerComponent
-from .CSVAgent import CSVAgentComponent
-from .JsonAgent import JsonAgentComponent
-from .OpenAIConversationalAgent import ConversationalAgent
-from .SQLAgent import SQLAgentComponent
-from .VectorStoreAgent import VectorStoreAgentComponent
-from .VectorStoreRouterAgent import VectorStoreRouterAgentComponent
-from .XMLAgent import XMLAgentComponent
+from .JsonToolkit import JsonToolkitComponent
+from .Metaphor import MetaphorToolkit
+from .OpenAPIToolkit import OpenAPIToolkitComponent
+from .VectorStoreInfo import VectorStoreInfoComponent
+from .VectorStoreRouterToolkit import VectorStoreRouterToolkitComponent
+from .VectorStoreToolkit import VectorStoreToolkitComponent
 
 __all__ = [
-    "AgentInitializerComponent",
-    "CSVAgentComponent",
-    "JsonAgentComponent",
-    "ConversationalAgent",
-    "SQLAgentComponent",
-    "VectorStoreAgentComponent",
-    "VectorStoreRouterAgentComponent",
-    "XMLAgentComponent",
+    "JsonToolkitComponent",
+    "MetaphorToolkit",
+    "OpenAPIToolkitComponent",
+    "VectorStoreInfoComponent",
+    "VectorStoreRouterToolkitComponent",
+    "VectorStoreToolkitComponent",
 ]
```

### Comparing `langflow_base-0.0.48/langflow/components/chains/ConversationChain.py` & `langflow_base-0.0.49/langflow/components/chains/ConversationChain.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional
 
 from langchain.chains import ConversationChain
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import BaseLanguageModel, BaseMemory, Text
-from langflow.interface.custom.custom_component import CustomComponent
 
 
 class ConversationChainComponent(CustomComponent):
     display_name = "ConversationChain"
     description = "Chain to have a conversation and load context from memory."
 
     def build_config(self):
```

### Comparing `langflow_base-0.0.48/langflow/components/chains/LLMCheckerChain.py` & `langflow_base-0.0.49/langflow/components/chains/LLMCheckerChain.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from langchain.chains import LLMCheckerChain
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import BaseLanguageModel, Text
-from langflow.interface.custom.custom_component import CustomComponent
 
 
 class LLMCheckerChainComponent(CustomComponent):
     display_name = "LLMCheckerChain"
     description = ""
     documentation = "https://python.langchain.com/docs/modules/chains/additional/llm_checker"
```

### Comparing `langflow_base-0.0.48/langflow/components/chains/LLMMathChain.py` & `langflow_base-0.0.49/langflow/components/chains/LLMMathChain.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional
 
 from langchain.chains import LLMChain, LLMMathChain
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import BaseLanguageModel, BaseMemory, Text
-from langflow.interface.custom.custom_component import CustomComponent
 
 
 class LLMMathChainComponent(CustomComponent):
     display_name = "LLMMathChain"
     description = "Chain that interprets a prompt and executes python code to do math."
     documentation = "https://python.langchain.com/docs/modules/chains/additional/llm_math"
```

### Comparing `langflow_base-0.0.48/langflow/components/chains/RetrievalQA.py` & `langflow_base-0.0.49/langflow/components/chains/RetrievalQA.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 
 from langchain.chains.retrieval_qa.base import RetrievalQA
 from langchain_core.documents import Document
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import BaseLanguageModel, BaseMemory, BaseRetriever, Text
-from langflow.interface.custom.custom_component import CustomComponent
 from langflow.schema.schema import Record
 
 
 class RetrievalQAComponent(CustomComponent):
     display_name = "Retrieval QA"
     description = "Chain for question-answering against an index."
```

### Comparing `langflow_base-0.0.48/langflow/components/chains/RetrievalQAWithSourcesChain.py` & `langflow_base-0.0.49/langflow/components/chains/RetrievalQAWithSourcesChain.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 
 from langchain.chains import RetrievalQAWithSourcesChain
 from langchain_core.documents import Document
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import BaseLanguageModel, BaseMemory, BaseRetriever, Text
-from langflow.interface.custom.custom_component import CustomComponent
 
 
 class RetrievalQAWithSourcesChainComponent(CustomComponent):
     display_name = "RetrievalQAWithSourcesChain"
     description = "Question-answering with sources over an index."
 
     def build_config(self):
```

### Comparing `langflow_base-0.0.48/langflow/components/chains/SQLGenerator.py` & `langflow_base-0.0.49/langflow/components/chains/SQLGenerator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Optional
 
 from langchain.chains import create_sql_query_chain
 from langchain_community.utilities.sql_database import SQLDatabase
 from langchain_core.prompts import PromptTemplate
 from langchain_core.runnables import Runnable
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import BaseLanguageModel, Text
-from langflow.interface.custom.custom_component import CustomComponent
 
 
 class SQLGeneratorComponent(CustomComponent):
     display_name = "Natural Language to SQL"
     description = "Generate SQL from natural language."
 
     def build_config(self):
```

### Comparing `langflow_base-0.0.48/langflow/components/chains/__init__.py` & `langflow_base-0.0.49/langflow/components/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/data/APIRequest.py` & `langflow_base-0.0.49/langflow/components/data/APIRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 import json
 from typing import List, Optional
 
 import httpx
-from langflow.interface.custom.custom_component import CustomComponent
+
+from langflow.custom import CustomComponent
 from langflow.schema import Record
 
 
 class APIRequest(CustomComponent):
     display_name: str = "API Request"
     description: str = "Make HTTP requests given one or more URLs."
     output_types: list[str] = ["Record"]
```

### Comparing `langflow_base-0.0.48/langflow/components/data/Directory.py` & `langflow_base-0.0.49/langflow/components/data/Directory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Dict, List, Optional
 
 from langflow.base.data.utils import parallel_load_records, parse_text_file_to_record, retrieve_file_paths
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 from langflow.schema import Record
 
 
 class DirectoryComponent(CustomComponent):
     display_name = "Directory"
     description = "Recursively load files from a directory."
     icon = "folder"
```

### Comparing `langflow_base-0.0.48/langflow/components/data/File.py` & `langflow_base-0.0.49/langflow/components/data/File.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from typing import Any, Dict
 
 from langflow.base.data.utils import TEXT_FILE_TYPES, parse_text_file_to_record
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 from langflow.schema import Record
 
 
 class FileComponent(CustomComponent):
     display_name = "File"
     description = "A generic file loader."
     icon = "file-text"
```

### Comparing `langflow_base-0.0.48/langflow/components/data/URL.py` & `langflow_base-0.0.49/langflow/components/data/URL.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Dict
 
 from langchain_community.document_loaders.web_base import WebBaseLoader
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 from langflow.schema import Record
 
 
 class URLComponent(CustomComponent):
     display_name = "URL"
     description = "Fetch content from one or more URLs."
     icon = "layout-template"
```

### Comparing `langflow_base-0.0.48/langflow/components/embeddings/AmazonBedrockEmbeddings.py` & `langflow_base-0.0.49/langflow/components/embeddings/AmazonBedrockEmbeddings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional
-from langchain_community.embeddings import BedrockEmbeddings
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langchain_community.embeddings import BedrockEmbeddings
 from langchain_core.embeddings import Embeddings
 
+from langflow.custom import CustomComponent
+
 
 class AmazonBedrockEmeddingsComponent(CustomComponent):
     display_name: str = "Amazon Bedrock Embeddings"
     description: str = "Generate embeddings using Amazon Bedrock models."
     documentation = "https://python.langchain.com/docs/modules/data_connection/text_embedding/integrations/bedrock"
 
     def build_config(self):
```

### Comparing `langflow_base-0.0.48/langflow/components/embeddings/AzureOpenAIEmbeddings.py` & `langflow_base-0.0.49/langflow/components/embeddings/AzureOpenAIEmbeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from langflow.interface.custom.custom_component import CustomComponent
 from langchain_core.embeddings import Embeddings
 from langchain_openai import AzureOpenAIEmbeddings
 from pydantic.v1 import SecretStr
 
+from langflow.custom import CustomComponent
+
 
 class AzureOpenAIEmbeddingsComponent(CustomComponent):
     display_name: str = "Azure OpenAI Embeddings"
     description: str = "Generate embeddings using Azure OpenAI models."
     documentation: str = "https://python.langchain.com/docs/integrations/text_embedding/azureopenai"
     beta = False
     icon = "Azure"
```

### Comparing `langflow_base-0.0.48/langflow/components/embeddings/CohereEmbeddings.py` & `langflow_base-0.0.49/langflow/components/embeddings/CohereEmbeddings.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/embeddings/HuggingFaceEmbeddings.py` & `langflow_base-0.0.49/langflow/components/embeddings/HuggingFaceEmbeddings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, Optional
 
 from langchain_community.embeddings.huggingface import HuggingFaceEmbeddings
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 
 
 class HuggingFaceEmbeddingsComponent(CustomComponent):
     display_name = "Hugging Face Embeddings"
     description = "Generate embeddings using HuggingFace models."
     documentation = (
         "https://python.langchain.com/docs/modules/data_connection/text_embedding/integrations/sentence_transformers"
```

### Comparing `langflow_base-0.0.48/langflow/components/embeddings/HuggingFaceInferenceAPIEmbeddings.py` & `langflow_base-0.0.49/langflow/components/embeddings/HuggingFaceInferenceAPIEmbeddings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict, Optional
 
 from langchain_community.embeddings.huggingface import HuggingFaceInferenceAPIEmbeddings
 from pydantic.v1.types import SecretStr
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 
 
 class HuggingFaceInferenceAPIEmbeddingsComponent(CustomComponent):
     display_name = "Hugging Face API Embeddings"
     description = "Generate embeddings using Hugging Face Inference API models."
     documentation = "https://github.com/huggingface/text-embeddings-inference"
     icon = "HuggingFace"
```

### Comparing `langflow_base-0.0.48/langflow/components/embeddings/MistalAIEmbeddings.py` & `langflow_base-0.0.49/langflow/components/embeddings/MistalAIEmbeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from langchain_mistralai.embeddings import MistralAIEmbeddings
 from pydantic.v1 import SecretStr
 
-from langchain_mistralai.embeddings import MistralAIEmbeddings
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 from langflow.field_typing import Embeddings
 
 
 class MistralAIEmbeddingsComponent(CustomComponent):
     display_name = "MistralAI Embeddings"
     description = "Generate embeddings using MistralAI models."
```

### Comparing `langflow_base-0.0.48/langflow/components/embeddings/OllamaEmbeddings.py` & `langflow_base-0.0.49/langflow/components/embeddings/OllamaEmbeddings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional
-from langchain_community.embeddings import OllamaEmbeddings
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langchain_community.embeddings import OllamaEmbeddings
 from langchain_core.embeddings import Embeddings
 
+from langflow.custom import CustomComponent
+
 
 class OllamaEmbeddingsComponent(CustomComponent):
     display_name: str = "Ollama Embeddings"
     description: str = "Generate embeddings using Ollama models."
     documentation = "https://python.langchain.com/docs/integrations/text_embedding/ollama"
 
     def build_config(self):
```

### Comparing `langflow_base-0.0.48/langflow/components/embeddings/OpenAIEmbeddings.py` & `langflow_base-0.0.49/langflow/components/embeddings/OpenAIEmbeddings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Any, Dict, List, Optional
+from typing import Dict, List, Optional
 
 from langchain_openai.embeddings.base import OpenAIEmbeddings
 from pydantic.v1 import SecretStr
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import Embeddings, NestedDict
-from langflow.interface.custom.custom_component import CustomComponent
 
 
 class OpenAIEmbeddingsComponent(CustomComponent):
     display_name = "OpenAI Embeddings"
     description = "Generate embeddings using OpenAI models."
 
     def build_config(self):
@@ -90,15 +90,14 @@
         self,
         openai_api_key: str,
         default_headers: Optional[Dict[str, str]] = None,
         default_query: Optional[NestedDict] = {},
         allowed_special: List[str] = [],
         disallowed_special: List[str] = ["all"],
         chunk_size: int = 1000,
-        client: Optional[Any] = None,
         deployment: str = "text-embedding-ada-002",
         embedding_ctx_length: int = 8191,
         max_retries: int = 6,
         model: str = "text-embedding-ada-002",
         model_kwargs: NestedDict = {},
         openai_api_base: Optional[str] = None,
         openai_api_type: Optional[str] = None,
@@ -122,15 +121,14 @@
         return OpenAIEmbeddings(
             tiktoken_enabled=tiktoken_enable,
             default_headers=default_headers,
             default_query=default_query,
             allowed_special=set(allowed_special),
             disallowed_special="all",
             chunk_size=chunk_size,
-            client=client,
             deployment=deployment,
             embedding_ctx_length=embedding_ctx_length,
             max_retries=max_retries,
             model=model,
             model_kwargs=model_kwargs,
             base_url=openai_api_base,
             api_key=api_key,
```

### Comparing `langflow_base-0.0.48/langflow/components/embeddings/VertexAIEmbeddings.py` & `langflow_base-0.0.49/langflow/components/embeddings/VertexAIEmbeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Optional
 
 from langchain_google_vertexai import VertexAIEmbeddings
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 
 
 class VertexAIEmbeddingsComponent(CustomComponent):
     display_name = "VertexAI Embeddings"
     description = "Generate embeddings using Google Cloud VertexAI models."
 
     def build_config(self):
```

### Comparing `langflow_base-0.0.48/langflow/components/embeddings/__init__.py` & `langflow_base-0.0.49/langflow/components/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/experimental/AgentComponent.py` & `langflow_base-0.0.49/langflow/components/experimental/AgentComponent.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/experimental/ClearMessageHistory.py` & `langflow_base-0.0.49/langflow/components/experimental/ClearMessageHistory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 from langflow.memory import delete_messages, get_messages
 
 
 class ClearMessageHistoryComponent(CustomComponent):
     display_name = "Clear Message History"
     description = "A component to clear the message history."
     icon = "ClearMessageHistory"
```

### Comparing `langflow_base-0.0.48/langflow/components/experimental/ExtractDataFromRecord.py` & `langflow_base-0.0.49/langflow/components/experimental/ExtractDataFromRecord.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 from langflow.schema import Record
 
 
 class ExtractKeyFromRecordComponent(CustomComponent):
     display_name = "Extract Key From Record"
     description = "Extracts a key from a record."
     beta: bool = True
```

### Comparing `langflow_base-0.0.48/langflow/components/experimental/FlowTool.py` & `langflow_base-0.0.49/langflow/components/experimental/FlowTool.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/experimental/Listen.py` & `langflow_base-0.0.49/langflow/components/experimental/Listen.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 from langflow.schema import Record
 
 
 class ListenComponent(CustomComponent):
     display_name = "Listen"
     description = "A component to listen for a notification."
     beta: bool = True
```

### Comparing `langflow_base-0.0.48/langflow/components/experimental/MergeRecords.py` & `langflow_base-0.0.49/langflow/components/experimental/MergeRecords.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 from langflow.schema import Record
 
 
 class MergeRecordsComponent(CustomComponent):
     display_name = "Merge Records"
     description = "Merges records."
     beta: bool = True
```

### Comparing `langflow_base-0.0.48/langflow/components/experimental/Notify.py` & `langflow_base-0.0.49/langflow/components/experimental/Notify.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 from langflow.schema import Record
 
 
 class NotifyComponent(CustomComponent):
     display_name = "Notify"
     description = "A component to generate a notification to Get Notified component."
     icon = "Notify"
```

### Comparing `langflow_base-0.0.48/langflow/components/experimental/Pass.py` & `langflow_base-0.0.49/langflow/components/experimental/Pass.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Union
-from langflow.interface.custom.custom_component import CustomComponent
-from langflow.schema import Record
+
+from langflow.custom import CustomComponent
 from langflow.field_typing import Text
+from langflow.schema import Record
 
 
 class PassComponent(CustomComponent):
     display_name = "Pass"
     description = "A pass-through component that forwards the second input while ignoring the first, used for controlling workflow direction."
     field_order = ["ignored_input", "forwarded_input"]
```

### Comparing `langflow_base-0.0.48/langflow/components/experimental/PythonFunction.py` & `langflow_base-0.0.49/langflow/components/experimental/PythonFunction.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable
 
+from langflow.custom import CustomComponent
+from langflow.custom.utils import get_function
 from langflow.field_typing import Code
-from langflow.interface.custom.custom_component import CustomComponent
-from langflow.interface.custom.utils import get_function
 
 
 class PythonFunctionComponent(CustomComponent):
     display_name = "Python Function"
     description = "Define a Python function."
     icon = "Python"
```

### Comparing `langflow_base-0.0.48/langflow/components/experimental/RunFlow.py` & `langflow_base-0.0.49/langflow/components/experimental/RunFlow.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/experimental/RunnableExecutor.py` & `langflow_base-0.0.49/langflow/components/experimental/RunnableExecutor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from langchain_core.runnables import Runnable
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import Text
-from langflow.interface.custom.custom_component import CustomComponent
 
 
 class RunnableExecComponent(CustomComponent):
     description = "Execute a runnable. It will try to guess the input and output keys."
     display_name = "Runnable Executor"
     beta: bool = True
     field_order = [
```

### Comparing `langflow_base-0.0.48/langflow/components/experimental/SQLExecutor.py` & `langflow_base-0.0.49/langflow/components/experimental/SQLExecutor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from langchain_community.tools.sql_database.tool import QuerySQLDataBaseTool
 from langchain_community.utilities import SQLDatabase
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import Text
-from langflow.interface.custom.custom_component import CustomComponent
 
 
 class SQLExecutorComponent(CustomComponent):
     display_name = "SQL Executor"
     description = "Execute SQL query."
     beta: bool = True
```

### Comparing `langflow_base-0.0.48/langflow/components/experimental/SplitText.py` & `langflow_base-0.0.49/langflow/components/experimental/SplitText.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import Text
-from langflow.interface.custom.custom_component import CustomComponent
 from langflow.schema import Record
 from langflow.utils.util import unescape_string
 
 
 class SplitTextComponent(CustomComponent):
     display_name: str = "Split Text"
     description: str = "Split text into chunks of a specified length."
```

### Comparing `langflow_base-0.0.48/langflow/components/experimental/StoreMessage.py` & `langflow_base-0.0.49/langflow/components/experimental/StoreMessage.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Optional
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 from langflow.memory import get_messages, store_message
 from langflow.schema import Record
 
 
 class StoreMessageComponent(CustomComponent):
     display_name = "Store Message"
     description = "Stores a chat message given a Session ID."
```

### Comparing `langflow_base-0.0.48/langflow/components/experimental/SubFlow.py` & `langflow_base-0.0.49/langflow/components/experimental/SubFlow.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/experimental/TextOperator.py` & `langflow_base-0.0.49/langflow/components/experimental/TextOperator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional, Union
 
-from langflow.interface.custom.custom_component import CustomComponent
-from langflow.schema import Record
+from langflow.custom import CustomComponent
 from langflow.field_typing import Text
+from langflow.schema import Record
 
 
 class TextOperatorComponent(CustomComponent):
     display_name = "Text Operator"
     description = "Compares two text inputs based on a specified condition such as equality or inequality, with optional case sensitivity."
 
     def build_config(self) -> dict:
```

### Comparing `langflow_base-0.0.48/langflow/components/experimental/__init__.py` & `langflow_base-0.0.49/langflow/components/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/helpers/CombineText.py` & `langflow_base-0.0.49/langflow/components/helpers/CombineText.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 from langflow.field_typing import Text
 
 
 class CombineTextComponent(CustomComponent):
     display_name = "Combine Text"
     description = "Concatenate two text sources into a single text chunk using a specified delimiter."
     icon = "merge"
```

### Comparing `langflow_base-0.0.48/langflow/components/helpers/CombineTextsUnsorted.py` & `langflow_base-0.0.49/langflow/components/helpers/CombineTextsUnsorted.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 from langflow.field_typing import Text
 
 
 class CombineTextsUnsortedComponent(CustomComponent):
     display_name = "Combine Texts (Unsorted)"
     description = "Concatenate text sources into a single text chunk using a specified delimiter."
     icon = "merge"
```

### Comparing `langflow_base-0.0.48/langflow/components/helpers/CreateRecord.py` & `langflow_base-0.0.49/langflow/components/helpers/CreateRecord.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/helpers/CustomComponent.py` & `langflow_base-0.0.49/langflow/components/helpers/CustomComponent.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # from langflow.field_typing import Data
+from langflow.custom import CustomComponent
 from langflow.schema import Record
-from langflow.interface.custom.custom_component import CustomComponent
 
 
 class Component(CustomComponent):
     display_name = "Custom Component"
     description = "Use as a template to create your own component."
     documentation: str = "http://docs.langflow.org/components/custom"
     icon = "custom_components"
```

### Comparing `langflow_base-0.0.48/langflow/components/helpers/DocumentToRecord.py` & `langflow_base-0.0.49/langflow/components/helpers/DocumentToRecord.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List
 
 from langchain_core.documents import Document
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 from langflow.schema import Record
 
 
 class DocumentToRecordComponent(CustomComponent):
     display_name = "Documents To Records"
     description = "Convert LangChain Documents into Records."
```

### Comparing `langflow_base-0.0.48/langflow/components/helpers/IDGenerator.py` & `langflow_base-0.0.49/langflow/components/helpers/IDGenerator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import uuid
 from typing import Any, Optional
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 
 
 class UUIDGeneratorComponent(CustomComponent):
     documentation: str = "http://docs.langflow.org/components/custom"
     display_name = "ID Generator"
     description = "Generates a unique ID."
```

### Comparing `langflow_base-0.0.48/langflow/components/helpers/MemoryComponent.py` & `langflow_base-0.0.49/langflow/components/helpers/MemoryComponent.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/helpers/MessageHistory.py` & `langflow_base-0.0.49/langflow/components/helpers/MessageHistory.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Optional
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 from langflow.memory import get_messages
 from langflow.schema import Record
 
 
 class MessageHistoryComponent(CustomComponent):
     display_name = "Message History"
     description = "Retrieves stored chat messages given a specific Session ID."
```

### Comparing `langflow_base-0.0.48/langflow/components/helpers/RecordsToText.py` & `langflow_base-0.0.49/langflow/components/helpers/RecordsToText.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from langflow.custom import CustomComponent
 from langflow.field_typing import Text
 from langflow.helpers.record import records_to_text
-from langflow.interface.custom.custom_component import CustomComponent
 from langflow.schema import Record
 
 
 class RecordsToTextComponent(CustomComponent):
     display_name = "Records To Text"
     description = "Convert Records into plain text following a specified template."
```

### Comparing `langflow_base-0.0.48/langflow/components/helpers/ShouldRunNext.py` & `langflow_base-0.0.49/langflow/components/helpers/ShouldRunNext.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/helpers/UpdateRecord.py` & `langflow_base-0.0.49/langflow/components/helpers/UpdateRecord.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 from langflow.schema import Record
 
 
 class UpdateRecordComponent(CustomComponent):
     display_name = "Update Record"
     description = "Update Record with text-based key/value pairs, similar to updating a Python dictionary."
```

### Comparing `langflow_base-0.0.48/langflow/components/helpers/__init__.py` & `langflow_base-0.0.49/langflow/components/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/inputs/ChatInput.py` & `langflow_base-0.0.49/langflow/components/inputs/ChatInput.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/inputs/Prompt.py` & `langflow_base-0.0.49/langflow/components/inputs/Prompt.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from langchain_core.prompts import PromptTemplate
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import Prompt, TemplateField, Text
-from langflow.interface.custom.custom_component import CustomComponent
 
 
 class PromptComponent(CustomComponent):
     display_name: str = "Prompt"
     description: str = "Create a prompt template with dynamic variables."
     icon = "prompts"
```

### Comparing `langflow_base-0.0.48/langflow/components/inputs/TextInput.py` & `langflow_base-0.0.49/langflow/components/inputs/TextInput.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/langchain_utilities/BingSearchAPIWrapper.py` & `langflow_base-0.0.49/langflow/components/langchain_utilities/BingSearchAPIWrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Assuming `BingSearchAPIWrapper` is a class that exists in the context
 # and has the appropriate methods and attributes.
 # We need to make sure this class is importable from the context where this code will be running.
 from langchain_community.utilities.bing_search import BingSearchAPIWrapper
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 
 
 class BingSearchAPIWrapperComponent(CustomComponent):
     display_name = "BingSearchAPIWrapper"
     description = "Wrapper for Bing Search API."
 
     def build_config(self):
```

### Comparing `langflow_base-0.0.48/langflow/components/langchain_utilities/GoogleSearchAPIWrapper.py` & `langflow_base-0.0.49/langflow/components/langchain_utilities/GoogleSearchAPIWrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable, Union
 
 from langchain_community.utilities.google_search import GoogleSearchAPIWrapper
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 
 
 class GoogleSearchAPIWrapperComponent(CustomComponent):
     display_name = "GoogleSearchAPIWrapper"
     description = "Wrapper for Google Search API."
 
     def build_config(self):
```

### Comparing `langflow_base-0.0.48/langflow/components/langchain_utilities/GoogleSerperAPIWrapper.py` & `langflow_base-0.0.49/langflow/components/langchain_utilities/GoogleSerperAPIWrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict
 
 # Assuming the existence of GoogleSerperAPIWrapper class in the serper module
 # If this class does not exist, you would need to create it or import the appropriate class from another module
 from langchain_community.utilities.google_serper import GoogleSerperAPIWrapper
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 
 
 class GoogleSerperAPIWrapperComponent(CustomComponent):
     display_name = "GoogleSerperAPIWrapper"
     description = "Wrapper around the Serper.dev Google Search API."
 
     def build_config(self) -> Dict[str, Dict]:
```

### Comparing `langflow_base-0.0.48/langflow/components/langchain_utilities/JSONDocumentBuilder.py` & `langflow_base-0.0.49/langflow/components/langchain_utilities/JSONDocumentBuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # **Output**
 
 # - **Document:** The Document containing the JSON object.
 
 from langchain_core.documents import Document
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 from langflow.services.database.models.base import orjson_dumps
 
 
 class JSONDocumentBuilder(CustomComponent):
     display_name: str = "JSON Document Builder"
     description: str = "Build a Document containing a JSON object using a key and another Document page content."
     output_types: list[str] = ["Document"]
```

### Comparing `langflow_base-0.0.48/langflow/components/langchain_utilities/SQLDatabase.py` & `langflow_base-0.0.49/langflow/components/langchain_utilities/SQLDatabase.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from langchain_experimental.sql.base import SQLDatabase
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 
 
 class SQLDatabaseComponent(CustomComponent):
     display_name = "SQLDatabase"
     description = "SQL Database"
 
     def build_config(self):
```

### Comparing `langflow_base-0.0.48/langflow/components/langchain_utilities/SearchApi.py` & `langflow_base-0.0.49/langflow/components/langchain_utilities/SearchApi.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/langchain_utilities/SearxSearchWrapper.py` & `langflow_base-0.0.49/langflow/components/langchain_utilities/SearxSearchWrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, Optional
 
 from langchain_community.utilities.searx_search import SearxSearchWrapper
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 
 
 class SearxSearchWrapperComponent(CustomComponent):
     display_name = "SearxSearchWrapper"
     description = "Wrapper for Searx API."
 
     def build_config(self):
```

### Comparing `langflow_base-0.0.48/langflow/components/langchain_utilities/SerpAPIWrapper.py` & `langflow_base-0.0.49/langflow/components/langchain_utilities/SerpAPIWrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable, Union
 
 from langchain_community.utilities.serpapi import SerpAPIWrapper
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 
 
 class SerpAPIWrapperComponent(CustomComponent):
     display_name = "SerpAPIWrapper"
     description = "Wrapper around SerpAPI"
 
     def build_config(self):
```

### Comparing `langflow_base-0.0.48/langflow/components/langchain_utilities/WikipediaAPIWrapper.py` & `langflow_base-0.0.49/langflow/components/langchain_utilities/WikipediaAPIWrapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable, Union
 
 from langchain_community.utilities.wikipedia import WikipediaAPIWrapper
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 
 # Assuming WikipediaAPIWrapper is a class that needs to be imported.
 # The import statement is not included as it is not provided in the JSON
 # and the actual implementation details are unknown.
 
 
 class WikipediaAPIWrapperComponent(CustomComponent):
```

### Comparing `langflow_base-0.0.48/langflow/components/langchain_utilities/WolframAlphaAPIWrapper.py` & `langflow_base-0.0.49/langflow/components/langchain_utilities/WolframAlphaAPIWrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable, Union
 
 from langchain_community.utilities.wolfram_alpha import WolframAlphaAPIWrapper
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 
 # Since all the fields in the JSON have show=False, we will only create a basic component
 # without any configurable fields.
 
 
 class WolframAlphaAPIWrapperComponent(CustomComponent):
     display_name = "WolframAlphaAPIWrapper"
```

### Comparing `langflow_base-0.0.48/langflow/components/memories/AstraDBMessageReader.py` & `langflow_base-0.0.49/langflow/components/models/GroqModel.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,91 +1,95 @@
-from typing import Optional, cast
+from typing import Optional
 
-from langchain_astradb.chat_message_histories import AstraDBChatMessageHistory
+from langchain_groq import ChatGroq
+from langflow.base.models.groq_constants import MODEL_NAMES
+from pydantic.v1 import SecretStr
 
-from langflow.base.memory.memory import BaseMemoryComponent
+from langflow.base.constants import STREAM_INFO_TEXT
+from langflow.base.models.model import LCModelComponent
 from langflow.field_typing import Text
-from langflow.schema.schema import Record
 
 
-class AstraDBMessageReaderComponent(BaseMemoryComponent):
-    display_name = "Astra DB Message Reader"
-    description = "Retrieves stored chat messages from Astra DB."
+class GroqModel(LCModelComponent):
+    display_name: str = "Groq"
+    description: str = "Generate text using Groq."
+    icon = "Groq"
+
+    field_order = [
+        "groq_api_key",
+        "model",
+        "max_output_tokens",
+        "temperature",
+        "top_k",
+        "top_p",
+        "n",
+        "input_value",
+        "system_message",
+        "stream",
+    ]
 
     def build_config(self):
         return {
-            "session_id": {
-                "display_name": "Session ID",
-                "info": "Session ID of the chat history.",
-                "input_types": ["Text"],
-            },
-            "collection_name": {
-                "display_name": "Collection Name",
-                "info": "Collection name for Astra DB.",
-                "input_types": ["Text"],
-            },
-            "token": {
-                "display_name": "Astra DB Application Token",
-                "info": "Token for the Astra DB instance.",
+            "groq_api_key": {
+                "display_name": "Groq API Key",
+                "info": "API key for the Groq API.",
                 "password": True,
             },
-            "api_endpoint": {
-                "display_name": "Astra DB API Endpoint",
-                "info": "API Endpoint for the Astra DB instance.",
-                "password": True,
+            "groq_api_base": {
+                "display_name": "Groq API Base",
+                "info": "Base URL path for API requests, leave blank if not using a proxy or service emulator.",
+                "advanced": True,
+            },
+            "max_tokens": {
+                "display_name": "Max Output Tokens",
+                "info": "The maximum number of tokens to generate.",
+                "advanced": True,
+            },
+            "temperature": {
+                "display_name": "Temperature",
+                "info": "Run inference with this temperature. Must by in the closed interval [0.0, 1.0].",
+            },
+            "n": {
+                "display_name": "N",
+                "info": "Number of chat completions to generate for each prompt. Note that the API may not return the full n completions if duplicates are generated.",
+                "advanced": True,
             },
-            "namespace": {
-                "display_name": "Namespace",
-                "info": "Namespace for the Astra DB instance.",
-                "input_types": ["Text"],
+            "model_name": {
+                "display_name": "Model",
+                "info": "The name of the model to use. Supported examples: gemini-pro",
+                "options": MODEL_NAMES,
+            },
+            "input_value": {"display_name": "Input", "info": "The input to the model."},
+            "stream": {
+                "display_name": "Stream",
+                "info": STREAM_INFO_TEXT,
+                "advanced": True,
+            },
+            "system_message": {
+                "display_name": "System Message",
+                "info": "System message to pass to the model.",
                 "advanced": True,
             },
         }
 
-    def get_messages(self, **kwargs) -> list[Record]:
-        """
-        Retrieves messages from the AstraDBChatMessageHistory memory.
-
-        Args:
-            memory (AstraDBChatMessageHistory): The AstraDBChatMessageHistory instance to retrieve messages from.
-
-        Returns:
-            list[Record]: A list of Record objects representing the search results.
-        """
-        memory: AstraDBChatMessageHistory = cast(AstraDBChatMessageHistory, kwargs.get("memory"))
-        if not memory:
-            raise ValueError("AstraDBChatMessageHistory instance is required.")
-
-        # Get messages from the memory
-        messages = memory.messages
-        results = [Record.from_lc_message(message) for message in messages]
-
-        return list(results)
-
     def build(
         self,
-        session_id: Text,
-        collection_name: str,
-        token: str,
-        api_endpoint: str,
-        namespace: Optional[str] = None,
-    ) -> list[Record]:
-        try:
-            pass
-        except ImportError:
-            raise ImportError(
-                "Could not import langchain Astra DB integration package. "
-                "Please install it with `pip install langchain-astradb`."
-            )
-
-        memory = AstraDBChatMessageHistory(
-            session_id=session_id,
-            collection_name=collection_name,
-            token=token,
-            api_endpoint=api_endpoint,
-            namespace=namespace,
+        groq_api_key: str,
+        model_name: str,
+        input_value: Text,
+        groq_api_base: Optional[str] = None,
+        max_tokens: Optional[int] = None,
+        temperature: float = 0.1,
+        n: Optional[int] = 1,
+        stream: bool = False,
+        system_message: Optional[str] = None,
+    ) -> Text:
+        output = ChatGroq(
+            model_name=model_name,
+            max_tokens=max_tokens or None,  # type: ignore
+            temperature=temperature,
+            groq_api_base=groq_api_base,
+            n=n or 1,
+            groq_api_key=SecretStr(groq_api_key),
+            streaming=stream,
         )
-
-        records = self.get_messages(memory=memory)
-        self.status = records
-
-        return records
+        return self.get_chat_result(output, stream, input_value, system_message)
```

### Comparing `langflow_base-0.0.48/langflow/components/memories/AstraDBMessageWriter.py` & `langflow_base-0.0.49/langflow/components/memories/AstraDBMessageWriter.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/memories/ZepMessageReader.py` & `langflow_base-0.0.49/langflow/components/memories/ZepMessageReader.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,27 +112,26 @@
     def build(
         self,
         session_id: Text,
         api_base_path: str = "api/v1",
         url: Optional[Text] = None,
         api_key: Optional[Text] = None,
         query: Optional[Text] = None,
-        search_scope: SearchScope = SearchScope.messages,
-        search_type: SearchType = SearchType.similarity,
+        search_scope: str = SearchScope.messages,
+        search_type: str = SearchType.similarity,
         limit: Optional[int] = None,
     ) -> list[Record]:
         try:
-            from zep_python import ZepClient
-            from zep_python.langchain import ZepChatMessageHistory
-
             # Monkeypatch API_BASE_PATH to
             # avoid 404
             # This is a workaround for the local Zep instance
             # cloud Zep works with v2
             import zep_python.zep_client
+            from zep_python import ZepClient
+            from zep_python.langchain import ZepChatMessageHistory
 
             zep_python.zep_client.API_BASE_PATH = api_base_path
         except ImportError:
             raise ImportError(
                 "Could not import zep-python package. " "Please install it with `pip install zep-python`."
             )
         if url == "":
```

### Comparing `langflow_base-0.0.48/langflow/components/memories/ZepMessageWriter.py` & `langflow_base-0.0.49/langflow/components/memories/ZepMessageWriter.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/model_specs/AmazonBedrockSpecs.py` & `langflow_base-0.0.49/langflow/components/model_specs/AmazonBedrockSpecs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Optional
-from langflow.field_typing import BaseLanguageModel
+
 from langchain_community.llms.bedrock import Bedrock
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
+from langflow.field_typing import BaseLanguageModel
 
 
 class AmazonBedrockComponent(CustomComponent):
     display_name: str = "Amazon Bedrock"
     description: str = "LLM model from Amazon Bedrock."
     icon = "Amazon"
```

### Comparing `langflow_base-0.0.48/langflow/components/model_specs/AnthropicLLMSpecs.py` & `langflow_base-0.0.49/langflow/components/model_specs/AnthropicLLMSpecs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional
+
 from langchain_anthropic import ChatAnthropic
+from langchain_core.language_models import BaseLanguageModel
 from pydantic.v1 import SecretStr
 
-from langflow.interface.custom.custom_component import CustomComponent
-from langchain_core.language_models import BaseLanguageModel
+from langflow.custom import CustomComponent
 
 
 class ChatAntropicSpecsComponent(CustomComponent):
     display_name: str = "Anthropic"
     description: str = "Anthropic Chat&Completion large language models."
     icon = "Anthropic"
 
@@ -30,16 +31,16 @@
                 "display_name": "Anthropic API Key",
                 "required": True,
                 "password": True,
                 "info": "Your Anthropic API key.",
             },
             "max_tokens": {
                 "display_name": "Max Tokens",
-                "field_type": "int",
-                "value": 256,
+                "advanced": True,
+                "info": "The maximum number of tokens to generate. Set to 0 for unlimited tokens.",
             },
             "temperature": {
                 "display_name": "Temperature",
                 "field_type": "float",
                 "value": 0.7,
             },
             "api_endpoint": {
```

### Comparing `langflow_base-0.0.48/langflow/components/model_specs/AzureChatOpenAISpecs.py` & `langflow_base-0.0.49/langflow/components/model_specs/AzureChatOpenAISpecs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Optional
 
-from langflow.interface.custom.custom_component import CustomComponent
 from langchain_core.language_models import BaseLanguageModel
 from langchain_openai import AzureChatOpenAI
 from pydantic.v1 import SecretStr
 
+from langflow.custom import CustomComponent
+
 
 class AzureChatOpenAISpecsComponent(CustomComponent):
     display_name: str = "AzureChatOpenAI"
     description: str = "LLM model from Azure OpenAI."
     documentation: str = "https://python.langchain.com/docs/integrations/llms/azure_openai"
     beta = False
     icon = "Azure"
@@ -61,19 +62,16 @@
                 "display_name": "Temperature",
                 "value": 0.7,
                 "field_type": "float",
                 "required": False,
             },
             "max_tokens": {
                 "display_name": "Max Tokens",
-                "value": 1000,
-                "required": False,
-                "field_type": "int",
                 "advanced": True,
-                "info": "Maximum number of tokens to generate.",
+                "info": "The maximum number of tokens to generate. Set to 0 for unlimited tokens.",
             },
             "code": {"show": False},
         }
 
     def build(
         self,
         model: str,
@@ -92,12 +90,12 @@
             llm = AzureChatOpenAI(
                 model=model,
                 azure_endpoint=azure_endpoint,
                 azure_deployment=azure_deployment,
                 api_version=api_version,
                 api_key=azure_api_key,
                 temperature=temperature,
-                max_tokens=max_tokens,
+                max_tokens=max_tokens or None,
             )
         except Exception as e:
             raise ValueError("Could not connect to AzureOpenAI API.") from e
         return llm
```

### Comparing `langflow_base-0.0.48/langflow/components/model_specs/BaiduQianfanChatEndpointsSpecs.py` & `langflow_base-0.0.49/langflow/components/model_specs/BaiduQianfanChatEndpointsSpecs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Optional
 
 from langchain_community.chat_models.baidu_qianfan_endpoint import QianfanChatEndpoint
+
 from pydantic.v1 import SecretStr
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import BaseLanguageModel
-from langflow.interface.custom.custom_component import CustomComponent
 
 
 class QianfanChatEndpointComponent(CustomComponent):
     display_name: str = "QianfanChatEndpoint"
     description: str = (
         "Baidu Qianfan chat models. Get more detail from "
         "https://python.langchain.com/docs/integrations/chat/baidu_qianfan_endpoint."
```

### Comparing `langflow_base-0.0.48/langflow/components/model_specs/BaiduQianfanLLMEndpointsSpecs.py` & `langflow_base-0.0.49/langflow/components/model_specs/BaiduQianfanLLMEndpointsSpecs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
 from langchain_community.llms.baidu_qianfan_endpoint import QianfanLLMEndpoint
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 from langflow.field_typing import BaseLanguageModel
 
 
 class QianfanLLMEndpointComponent(CustomComponent):
     display_name: str = "QianfanLLMEndpoint"
     description: str = (
         "Baidu Qianfan hosted open source or customized models. "
```

### Comparing `langflow_base-0.0.48/langflow/components/model_specs/ChatAnthropicSpecs.py` & `langflow_base-0.0.49/langflow/components/model_specs/ChatAnthropicSpecs.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,17 +42,16 @@
                 "display_name": "Anthropic API Key",
                 "required": True,
                 "password": True,
                 "info": "Your Anthropic API key.",
             },
             "max_tokens": {
                 "display_name": "Max Tokens",
-                "field_type": "int",
                 "advanced": True,
-                "value": 256,
+                "info": "The maximum number of tokens to generate. Set to 0 for unlimited tokens.",
             },
             "temperature": {
                 "display_name": "Temperature",
                 "field_type": "float",
                 "value": 0.1,
             },
             "anthropic_api_url": {
```

### Comparing `langflow_base-0.0.48/langflow/components/model_specs/ChatLiteLLMSpecs.py` & `langflow_base-0.0.49/langflow/components/model_specs/ChatLiteLLMSpecs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Dict, Optional
 
 from langchain_community.chat_models.litellm import ChatLiteLLM, ChatLiteLLMException
+
+from langflow.custom import CustomComponent
 from langflow.field_typing import BaseLanguageModel
-from langflow.interface.custom.custom_component import CustomComponent
 
 
 class ChatLiteLLMComponent(CustomComponent):
     display_name = "ChatLiteLLM"
     description = "`LiteLLM` collection of large language models."
     documentation = "https://python.langchain.com/docs/integrations/chat/litellm"
 
@@ -77,20 +78,17 @@
                 "advanced": True,
                 "required": False,
                 "info": "Number of chat completions to generate for each prompt. "
                 "Note that the API may not return the full n completions if duplicates are generated.",
                 "default": 1,
             },
             "max_tokens": {
-                "display_name": "Max tokens",
-                "field_type": "int",
-                "advanced": False,
-                "required": False,
-                "default": 256,
-                "info": "The maximum number of tokens to generate for each chat completion.",
+                "display_name": "Max Tokens",
+                "advanced": True,
+                "info": "The maximum number of tokens to generate. Set to 0 for unlimited tokens.",
             },
             "max_retries": {
                 "display_name": "Max retries",
                 "field_type": "int",
                 "advanced": True,
                 "required": False,
                 "default": 6,
```

### Comparing `langflow_base-0.0.48/langflow/components/model_specs/ChatMistralSpecs.py` & `langflow_base-0.0.49/langflow/components/model_specs/ChatMistralSpecs.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         if not mistral_api_base:
             mistral_api_base = "https://api.mistral.ai"
 
         try:
             output = ChatMistralAI(
                 model_name=model,
                 api_key=(SecretStr(mistral_api_key) if mistral_api_key else None),
-                max_tokens=max_tokens,
+                max_tokens=max_tokens or None,
                 temperature=temperature,
                 endpoint=mistral_api_base,
             )
         except Exception as e:
             raise ValueError("Could not connect to Mistral API.") from e
 
         return output
```

### Comparing `langflow_base-0.0.48/langflow/components/model_specs/ChatOllamaEndpointSpecs.py` & `langflow_base-0.0.49/langflow/components/model_specs/ChatOllamaEndpointSpecs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import Any, Dict, List, Optional
+from typing import Dict, List, Optional
 
 # from langchain_community.chat_models import ChatOllama
 from langchain_community.chat_models import ChatOllama
 from langchain_core.language_models.chat_models import BaseChatModel
 
 # from langchain.chat_models import ChatOllama
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 
 # from langchain.callbacks.manager import CallbackManager
 
 
 class ChatOllamaComponent(CustomComponent):
     display_name = "ChatOllama"
     description = "Local LLM for chat with Ollama."
@@ -178,15 +178,15 @@
         #######################################################################################
         repeat_last_n: Optional[int] = None,
         verbose: Optional[bool] = None,
         cache: Optional[bool] = None,
         num_ctx: Optional[int] = None,
         num_gpu: Optional[int] = None,
         format: Optional[str] = None,
-        metadata: Optional[Dict[str, Any]] = None,
+        metadata: Optional[Dict] = None,
         num_thread: Optional[int] = None,
         repeat_penalty: Optional[float] = None,
         stop: Optional[List[str]] = None,
         system: Optional[str] = None,
         tags: Optional[List[str]] = None,
         temperature: Optional[float] = None,
         template: Optional[str] = None,
```

### Comparing `langflow_base-0.0.48/langflow/components/model_specs/ChatOpenAISpecs.py` & `langflow_base-0.0.49/langflow/components/model_specs/ChatOpenAISpecs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from typing import Optional
 
 from langchain_openai import ChatOpenAI
 from pydantic.v1 import SecretStr
 
-
 from langflow.base.models.openai_constants import MODEL_NAMES
+from langflow.custom import CustomComponent
 from langflow.field_typing import BaseLanguageModel, NestedDict
-from langflow.interface.custom.custom_component import CustomComponent
 
 
 class ChatOpenAIComponent(CustomComponent):
     display_name = "ChatOpenAI"
     description = "`OpenAI` Chat large language models API."
     icon = "OpenAI"
 
     def build_config(self):
         return {
             "max_tokens": {
                 "display_name": "Max Tokens",
-                "advanced": False,
-                "required": False,
+                "advanced": True,
+                "info": "The maximum number of tokens to generate. Set to 0 for unlimited tokens.",
             },
             "model_kwargs": {
                 "display_name": "Model Kwargs",
                 "advanced": True,
                 "required": False,
             },
             "model_name": {"display_name": "Model Name", "advanced": False, "options": MODEL_NAMES},
@@ -48,28 +47,28 @@
                 "required": False,
                 "value": 0.7,
             },
         }
 
     def build(
         self,
-        max_tokens: Optional[int] = 256,
+        max_tokens: Optional[int] = 0,
         model_kwargs: NestedDict = {},
         model_name: str = "gpt-4o",
         openai_api_base: Optional[str] = None,
         openai_api_key: Optional[str] = None,
         temperature: float = 0.7,
     ) -> BaseLanguageModel:
         if not openai_api_base:
             openai_api_base = "https://api.openai.com/v1"
         if openai_api_key:
             api_key = SecretStr(openai_api_key)
         else:
             api_key = None
         return ChatOpenAI(
-            max_tokens=max_tokens,
+            max_tokens=max_tokens or None,
             model_kwargs=model_kwargs,
             model=model_name,
             base_url=openai_api_base,
             api_key=api_key,
             temperature=temperature,
         )
```

### Comparing `langflow_base-0.0.48/langflow/components/model_specs/ChatVertexAISpecs.py` & `langflow_base-0.0.49/langflow/components/model_specs/ChatVertexAISpecs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from typing import List, Optional
+from typing import Optional
 
 from langchain_community.chat_models.vertexai import ChatVertexAI
-from langchain_core.messages.base import BaseMessage
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import BaseLanguageModel
-from langflow.interface.custom.custom_component import CustomComponent
 
 
 class ChatVertexAIComponent(CustomComponent):
     display_name = "ChatVertexAI"
     description = "`Vertex AI` Chat large language models API."
     icon = "VertexAI"
 
@@ -61,26 +60,24 @@
             },
         }
 
     def build(
         self,
         credentials: Optional[str],
         project: str,
-        examples: Optional[List[BaseMessage]] = [],
         location: str = "us-central1",
         max_output_tokens: int = 128,
         model_name: str = "chat-bison",
         temperature: float = 0.0,
         top_k: int = 40,
         top_p: float = 0.95,
         verbose: bool = False,
     ) -> BaseLanguageModel:
         return ChatVertexAI(
             credentials=credentials,
-            examples=examples,
             location=location,
             max_output_tokens=max_output_tokens,
             model_name=model_name,
             project=project,
             temperature=temperature,
             top_k=top_k,
             top_p=top_p,
```

### Comparing `langflow_base-0.0.48/langflow/components/model_specs/GoogleGenerativeAISpecs.py` & `langflow_base-0.0.49/langflow/components/model_specs/GoogleGenerativeAISpecs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 
 from langchain_google_genai import ChatGoogleGenerativeAI  # type: ignore
 from pydantic.v1.types import SecretStr
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import BaseLanguageModel, RangeSpec
-from langflow.interface.custom.custom_component import CustomComponent
 
 
 class GoogleGenerativeAIComponent(CustomComponent):
     display_name: str = "Google Generative AI"
     description: str = "A component that uses Google Generative AI to generate text."
     documentation: str = "http://docs.langflow.org/components/custom"
     icon = "Google"
```

### Comparing `langflow_base-0.0.48/langflow/components/model_specs/GroqModelSpecs.py` & `langflow_base-0.0.49/langflow/components/model_specs/GroqModelSpecs.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/model_specs/HuggingFaceEndpointsSpecs.py` & `langflow_base-0.0.49/langflow/components/model_specs/HuggingFaceEndpointsSpecs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional
 
-from langflow.field_typing import BaseLanguageModel
 from langchain_community.llms.huggingface_endpoint import HuggingFaceEndpoint
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
+from langflow.field_typing import BaseLanguageModel
 
 
 class HuggingFaceEndpointsComponent(CustomComponent):
     display_name: str = "Hugging Face Inference API"
     description: str = "LLM model from Hugging Face Inference API."
     icon = "HuggingFace"
```

### Comparing `langflow_base-0.0.48/langflow/components/model_specs/OllamaLLMSpecs.py` & `langflow_base-0.0.49/langflow/components/model_specs/OllamaLLMSpecs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Optional
 
-from langflow.field_typing import BaseLanguageModel
 from langchain_community.llms.ollama import Ollama
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
+from langflow.field_typing import BaseLanguageModel
 
 
 class OllamaLLM(CustomComponent):
     display_name = "Ollama"
     description = "Local LLM with Ollama."
 
     def build_config(self) -> dict:
```

### Comparing `langflow_base-0.0.48/langflow/components/model_specs/VertexAISpecs.py` & `langflow_base-0.0.49/langflow/components/model_specs/VertexAISpecs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict, Optional
 
-from langflow.field_typing import BaseLanguageModel
 from langchain_community.llms.vertexai import VertexAI
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
+from langflow.field_typing import BaseLanguageModel
 
 
 class VertexAIComponent(CustomComponent):
     display_name = "VertexAI"
     description = "Google Vertex AI large language models"
     icon = "VertexAI"
```

### Comparing `langflow_base-0.0.48/langflow/components/model_specs/__init__.py` & `langflow_base-0.0.49/langflow/components/model_specs/__init__.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/models/AmazonBedrockModel.py` & `langflow_base-0.0.49/langflow/components/models/AmazonBedrockModel.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/models/AnthropicModel.py` & `langflow_base-0.0.49/langflow/components/models/AnthropicModel.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,17 +45,16 @@
                 "display_name": "Anthropic API Key",
                 "required": True,
                 "password": True,
                 "info": "Your Anthropic API key.",
             },
             "max_tokens": {
                 "display_name": "Max Tokens",
-                "field_type": "int",
                 "advanced": True,
-                "value": 256,
+                "info": "The maximum number of tokens to generate. Set to 0 for unlimited tokens.",
             },
             "temperature": {
                 "display_name": "Temperature",
                 "field_type": "float",
                 "value": 0.1,
             },
             "anthropic_api_url": {
```

### Comparing `langflow_base-0.0.48/langflow/components/models/AzureOpenAIModel.py` & `langflow_base-0.0.49/langflow/components/models/AzureOpenAIModel.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,17 +70,16 @@
             "api_key": {"display_name": "API Key", "password": True},
             "temperature": {
                 "display_name": "Temperature",
                 "value": 0.7,
             },
             "max_tokens": {
                 "display_name": "Max Tokens",
-                "value": 1000,
                 "advanced": True,
-                "info": "Maximum number of tokens to generate.",
+                "info": "The maximum number of tokens to generate. Set to 0 for unlimited tokens.",
             },
             "code": {"show": False},
             "input_value": {"display_name": "Input"},
             "stream": {
                 "display_name": "Stream",
                 "info": STREAM_INFO_TEXT,
                 "advanced": True,
@@ -113,13 +112,13 @@
             output = AzureChatOpenAI(
                 model=model,
                 azure_endpoint=azure_endpoint,
                 azure_deployment=azure_deployment,
                 api_version=api_version,
                 api_key=secret_api_key,
                 temperature=temperature,
-                max_tokens=max_tokens,
+                max_tokens=max_tokens or None,
             )
         except Exception as e:
             raise ValueError("Could not connect to AzureOpenAI API.") from e
 
         return self.get_chat_result(output, stream, input_value, system_message)
```

### Comparing `langflow_base-0.0.48/langflow/components/models/BaiduQianfanChatModel.py` & `langflow_base-0.0.49/langflow/components/models/BaiduQianfanChatModel.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/models/ChatLiteLLMModel.py` & `langflow_base-0.0.49/langflow/components/models/ChatLiteLLMModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,17 +89,15 @@
                 "required": False,
                 "info": "Number of chat completions to generate for each prompt. "
                 "Note that the API may not return the full n completions if duplicates are generated.",
                 "default": 1,
             },
             "max_tokens": {
                 "display_name": "Max tokens",
-                "field_type": "int",
                 "advanced": False,
-                "required": False,
                 "default": 256,
                 "info": "The maximum number of tokens to generate for each chat completion.",
             },
             "max_retries": {
                 "display_name": "Max retries",
                 "field_type": "int",
                 "advanced": True,
```

### Comparing `langflow_base-0.0.48/langflow/components/models/CohereModel.py` & `langflow_base-0.0.49/langflow/components/models/CohereModel.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 
-from langchain_community.chat_models.cohere import ChatCohere
 from pydantic.v1 import SecretStr
 from langflow.field_typing import Text
 from langflow.base.constants import STREAM_INFO_TEXT
 from langflow.base.models.model import LCModelComponent
+from langchain_cohere import ChatCohere
 
 
 class CohereComponent(LCModelComponent):
     display_name = "Cohere"
     description = "Generate text using Cohere LLMs."
     documentation = "https://python.langchain.com/docs/modules/model_io/models/llms/integrations/cohere"
 
@@ -30,17 +30,15 @@
                 "type": "password",
                 "password": True,
                 "required": True,
             },
             "max_tokens": {
                 "display_name": "Max Tokens",
                 "advanced": True,
-                "default": 256,
-                "type": "int",
-                "show": True,
+                "info": "The maximum number of tokens to generate. Set to 0 for unlimited tokens.",
             },
             "temperature": {
                 "display_name": "Temperature",
                 "default": 0.75,
                 "type": "float",
                 "show": True,
             },
```

### Comparing `langflow_base-0.0.48/langflow/components/models/GoogleGenerativeAIModel.py` & `langflow_base-0.0.49/langflow/components/models/GoogleGenerativeAIModel.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/models/GroqModel.py` & `langflow_base-0.0.49/langflow/components/vectorsearch/WeaviateSearch.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,95 +1,85 @@
-from typing import Optional
+from typing import List, Optional
 
-from langchain_groq import ChatGroq
-from langflow.base.models.groq_constants import MODEL_NAMES
-from pydantic.v1 import SecretStr
-
-from langflow.base.constants import STREAM_INFO_TEXT
-from langflow.base.models.model import LCModelComponent
+from langflow.components.vectorstores.base.model import LCVectorStoreComponent
+from langflow.components.vectorstores.Weaviate import WeaviateVectorStoreComponent
 from langflow.field_typing import Text
+from langflow.schema import Record
+from langchain_core.embeddings import Embeddings
 
 
-class GroqModel(LCModelComponent):
-    display_name: str = "Groq"
-    description: str = "Generate text using Groq."
-    icon = "Groq"
-
-    field_order = [
-        "groq_api_key",
-        "model",
-        "max_output_tokens",
-        "temperature",
-        "top_k",
-        "top_p",
-        "n",
-        "input_value",
-        "system_message",
-        "stream",
-    ]
-
-    def build_config(self):
-        return {
-            "groq_api_key": {
-                "display_name": "Groq API Key",
-                "info": "API key for the Groq API.",
-                "password": True,
-            },
-            "groq_api_base": {
-                "display_name": "Groq API Base",
-                "info": "Base URL path for API requests, leave blank if not using a proxy or service emulator.",
-                "advanced": True,
-            },
-            "max_tokens": {
-                "display_name": "Max Output Tokens",
-                "info": "The maximum number of tokens to generate.",
-                "advanced": True,
-            },
-            "temperature": {
-                "display_name": "Temperature",
-                "info": "Run inference with this temperature. Must by in the closed interval [0.0, 1.0].",
-            },
-            "n": {
-                "display_name": "N",
-                "info": "Number of chat completions to generate for each prompt. Note that the API may not return the full n completions if duplicates are generated.",
-                "advanced": True,
-            },
-            "model_name": {
-                "display_name": "Model",
-                "info": "The name of the model to use. Supported examples: gemini-pro",
-                "options": MODEL_NAMES,
-            },
-            "input_value": {"display_name": "Input", "info": "The input to the model."},
-            "stream": {
-                "display_name": "Stream",
-                "info": STREAM_INFO_TEXT,
-                "advanced": True,
-            },
-            "system_message": {
-                "display_name": "System Message",
-                "info": "System message to pass to the model.",
-                "advanced": True,
-            },
-        }
+class WeaviateSearchVectorStore(WeaviateVectorStoreComponent, LCVectorStoreComponent):
+    display_name: str = "Weaviate Search"
+    description: str = "Search a Weaviate Vector Store for similar documents."
+    documentation = "https://python.langchain.com/docs/integrations/vectorstores/weaviate"
+    icon = "Weaviate"
+
+    field_config = {
+        "search_type": {
+            "display_name": "Search Type",
+            "options": ["Similarity", "MMR"],
+        },
+        "input_value": {"display_name": "Input"},
+        "url": {"display_name": "Weaviate URL", "value": "http://localhost:8080"},
+        "api_key": {
+            "display_name": "API Key",
+            "password": True,
+            "required": False,
+        },
+        "index_name": {
+            "display_name": "Index name",
+            "required": False,
+        },
+        "text_key": {
+            "display_name": "Text Key",
+            "required": False,
+            "advanced": True,
+            "value": "text",
+        },
+        "embedding": {"display_name": "Embedding"},
+        "attributes": {
+            "display_name": "Attributes",
+            "required": False,
+            "is_list": True,
+            "field_type": "str",
+            "advanced": True,
+        },
+        "search_by_text": {
+            "display_name": "Search By Text",
+            "field_type": "bool",
+            "advanced": True,
+        },
+        "number_of_results": {
+            "display_name": "Number of Results",
+            "info": "Number of results to return.",
+            "advanced": True,
+        },
+    }
 
-    def build(
+    def build(  # type: ignore[override]
         self,
-        groq_api_key: str,
-        model_name: str,
         input_value: Text,
-        groq_api_base: Optional[str] = None,
-        max_tokens: Optional[int] = None,
-        temperature: float = 0.1,
-        n: Optional[int] = 1,
-        stream: bool = False,
-        system_message: Optional[str] = None,
-    ) -> Text:
-        output = ChatGroq(
-            model_name=model_name,
-            max_tokens=max_tokens or None,  # type: ignore
-            temperature=temperature,
-            groq_api_base=groq_api_base,
-            n=n or 1,
-            groq_api_key=SecretStr(groq_api_key),
-            streaming=stream,
+        search_type: str,
+        url: str,
+        index_name: str,
+        number_of_results: int = 4,
+        search_by_text: bool = False,
+        api_key: Optional[str] = None,
+        text_key: str = "text",
+        embedding: Optional[Embeddings] = None,
+        attributes: Optional[list] = None,
+    ) -> List[Record]:
+        vector_store = super().build(
+            url=url,
+            api_key=api_key,
+            index_name=index_name,
+            text_key=text_key,
+            embedding=embedding,
+            attributes=attributes,
+            search_by_text=search_by_text,
+        )
+        if not vector_store:
+            raise ValueError("Failed to load the Weaviate index.")
+
+        return self.search_with_vector_store(
+            vector_store=vector_store, input_value=input_value, search_type=search_type, k=number_of_results
         )
-        return self.get_chat_result(output, stream, input_value, system_message)
```

### Comparing `langflow_base-0.0.48/langflow/components/models/HuggingFaceModel.py` & `langflow_base-0.0.49/langflow/components/models/HuggingFaceModel.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/models/MistralModel.py` & `langflow_base-0.0.49/langflow/components/models/MistralModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
     def build_config(self):
         return {
             "input_value": {"display_name": "Input"},
             "max_tokens": {
                 "display_name": "Max Tokens",
                 "advanced": True,
+                "info": "The maximum number of tokens to generate. Set to 0 for unlimited tokens.",
             },
             "model_name": {
                 "display_name": "Model Name",
                 "advanced": False,
                 "options": [
                     "open-mistral-7b",
                     "open-mixtral-8x7b",
@@ -121,15 +122,15 @@
             mistral_api_base = "https://api.mistral.ai"
         if mistral_api_key:
             api_key = SecretStr(mistral_api_key)
         else:
             api_key = None
 
         chat_model = ChatMistralAI(
-            max_tokens=max_tokens,
+            max_tokens=max_tokens or None,
             model_name=model_name,
             endpoint=mistral_api_base,
             api_key=api_key,
             temperature=temperature,
             max_retries=max_retries,
             timeout=timeout,
             max_concurrent_requests=max_concurrent_requests,
```

### Comparing `langflow_base-0.0.48/langflow/components/models/OllamaModel.py` & `langflow_base-0.0.49/langflow/components/models/OllamaModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List, Optional
+from typing import Dict, List, Optional
 
 # from langchain_community.chat_models import ChatOllama
 from langchain_community.chat_models import ChatOllama
 
 from langflow.base.constants import STREAM_INFO_TEXT
 from langflow.base.models.model import LCModelComponent
 
@@ -225,15 +225,15 @@
         #######################################################################################
         repeat_last_n: Optional[int] = None,
         verbose: Optional[bool] = None,
         cache: Optional[bool] = None,
         num_ctx: Optional[int] = None,
         num_gpu: Optional[int] = None,
         format: Optional[str] = None,
-        metadata: Optional[Dict[str, Any]] = None,
+        metadata: Optional[Dict] = None,
         num_thread: Optional[int] = None,
         repeat_penalty: Optional[float] = None,
         stop: Optional[List[str]] = None,
         system: Optional[str] = None,
         tags: Optional[List[str]] = None,
         temperature: Optional[float] = None,
         template: Optional[str] = None,
```

### Comparing `langflow_base-0.0.48/langflow/components/models/OpenAIModel.py` & `langflow_base-0.0.49/langflow/components/vectorsearch/QdrantSearch.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,104 +1,103 @@
-from typing import Optional
+from typing import List, Optional
 
-from langchain_openai import ChatOpenAI
-from pydantic.v1 import SecretStr
+from langflow.components.vectorstores.base.model import LCVectorStoreComponent
+from langflow.components.vectorstores.Qdrant import QdrantComponent
+from langflow.field_typing import Embeddings, NestedDict, Text
+from langflow.schema import Record
 
-from langflow.base.constants import STREAM_INFO_TEXT
-from langflow.base.models.model import LCModelComponent
-from langflow.base.models.openai_constants import MODEL_NAMES
-from langflow.field_typing import NestedDict, Text
-
-
-class OpenAIModelComponent(LCModelComponent):
-    display_name = "OpenAI"
-    description = "Generates text using OpenAI LLMs."
-    icon = "OpenAI"
-
-    field_order = [
-        "max_tokens",
-        "model_kwargs",
-        "model_name",
-        "openai_api_base",
-        "openai_api_key",
-        "temperature",
-        "input_value",
-        "system_message",
-        "stream",
-    ]
+
+class QdrantSearchComponent(QdrantComponent, LCVectorStoreComponent):
+    display_name = "Qdrant Search"
+    description = "Construct Qdrant wrapper from a list of texts."
+    icon = "Qdrant"
 
     def build_config(self):
         return {
-            "input_value": {"display_name": "Input"},
-            "max_tokens": {
-                "display_name": "Max Tokens",
-                "advanced": True,
-            },
-            "model_kwargs": {
-                "display_name": "Model Kwargs",
-                "advanced": True,
-            },
-            "model_name": {
-                "display_name": "Model Name",
-                "advanced": False,
-                "options": MODEL_NAMES,
+            "search_type": {
+                "display_name": "Search Type",
+                "options": ["Similarity", "MMR"],
             },
-            "openai_api_base": {
-                "display_name": "OpenAI API Base",
+            "input_value": {"display_name": "Input"},
+            "embedding": {"display_name": "Embedding"},
+            "api_key": {"display_name": "API Key", "password": True, "advanced": True},
+            "collection_name": {"display_name": "Collection Name"},
+            "content_payload_key": {
+                "display_name": "Content Payload Key",
                 "advanced": True,
-                "info": (
-                    "The base URL of the OpenAI API. Defaults to https://api.openai.com/v1.\n\n"
-                    "You can change this to use other APIs like JinaChat, LocalAI and Prem."
-                ),
-            },
-            "openai_api_key": {
-                "display_name": "OpenAI API Key",
-                "info": "The OpenAI API Key to use for the OpenAI model.",
-                "advanced": False,
-                "password": True,
-            },
-            "temperature": {
-                "display_name": "Temperature",
-                "advanced": False,
-                "value": 0.1,
             },
-            "stream": {
-                "display_name": "Stream",
-                "info": STREAM_INFO_TEXT,
+            "distance_func": {"display_name": "Distance Function", "advanced": True},
+            "grpc_port": {"display_name": "gRPC Port", "advanced": True},
+            "host": {"display_name": "Host", "advanced": True},
+            "https": {"display_name": "HTTPS", "advanced": True},
+            "location": {"display_name": "Location", "advanced": True},
+            "metadata_payload_key": {
+                "display_name": "Metadata Payload Key",
                 "advanced": True,
             },
-            "system_message": {
-                "display_name": "System Message",
-                "info": "System message to pass to the model.",
+            "path": {"display_name": "Path", "advanced": True},
+            "port": {"display_name": "Port", "advanced": True},
+            "prefer_grpc": {"display_name": "Prefer gRPC", "advanced": True},
+            "prefix": {"display_name": "Prefix", "advanced": True},
+            "search_kwargs": {"display_name": "Search Kwargs", "advanced": True},
+            "timeout": {"display_name": "Timeout", "advanced": True},
+            "url": {"display_name": "URL", "advanced": True},
+            "number_of_results": {
+                "display_name": "Number of Results",
+                "info": "Number of results to return.",
                 "advanced": True,
             },
         }
 
-    def build(
+    def build(  # type: ignore[override]
         self,
         input_value: Text,
-        openai_api_key: str,
-        temperature: float,
-        model_name: str = "gpt-4o",
-        max_tokens: Optional[int] = 256,
-        model_kwargs: NestedDict = {},
-        openai_api_base: Optional[str] = None,
-        stream: bool = False,
-        system_message: Optional[str] = None,
-    ) -> Text:
-        if not openai_api_base:
-            openai_api_base = "https://api.openai.com/v1"
-        if openai_api_key:
-            api_key = SecretStr(openai_api_key)
-        else:
-            api_key = None
-
-        output = ChatOpenAI(
-            max_tokens=max_tokens,
-            model_kwargs=model_kwargs,
-            model=model_name,
-            base_url=openai_api_base,
+        embedding: Embeddings,
+        collection_name: str,
+        number_of_results: int = 4,
+        search_type: str = "similarity",
+        api_key: Optional[str] = None,
+        content_payload_key: str = "page_content",
+        distance_func: str = "Cosine",
+        grpc_port: int = 6334,
+        https: bool = False,
+        host: Optional[str] = None,
+        location: Optional[str] = None,
+        metadata_payload_key: str = "metadata",
+        path: Optional[str] = None,
+        port: Optional[int] = 6333,
+        prefer_grpc: bool = False,
+        prefix: Optional[str] = None,
+        search_kwargs: Optional[NestedDict] = None,
+        timeout: Optional[int] = None,
+        url: Optional[str] = None,
+    ) -> List[Record]:  # type: ignore[override]
+        vector_store = super().build(
+            embedding=embedding,
+            collection_name=collection_name,
             api_key=api_key,
-            temperature=temperature,
+            content_payload_key=content_payload_key,
+            distance_func=distance_func,
+            grpc_port=grpc_port,
+            https=https,
+            host=host,
+            location=location,
+            metadata_payload_key=metadata_payload_key,
+            path=path,
+            port=port,
+            prefer_grpc=prefer_grpc,
+            prefix=prefix,
+            timeout=timeout,
+            url=url,
+        )
+        if not vector_store:
+            raise ValueError("Failed to load the Qdrant index.")
+        if search_kwargs is None:
+            search_kwargs = {}
+
+        return self.search_with_vector_store(
+            vector_store=vector_store,
+            input_value=input_value,
+            search_type=search_type,
+            k=number_of_results,
+            **search_kwargs,
         )
-
-        return self.get_chat_result(output, stream, input_value, system_message)
```

### Comparing `langflow_base-0.0.48/langflow/components/models/VertexAiModel.py` & `langflow_base-0.0.49/langflow/components/models/VertexAiModel.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from typing import List, Optional
+from typing import Optional
 
-from langchain_core.messages.base import BaseMessage
 
 from langflow.base.constants import STREAM_INFO_TEXT
 from langflow.base.models.model import LCModelComponent
 from langflow.field_typing import Text
 
 
 class ChatVertexAIComponent(LCModelComponent):
@@ -89,15 +88,14 @@
         }
 
     def build(
         self,
         input_value: Text,
         credentials: Optional[str],
         project: str,
-        examples: Optional[List[BaseMessage]] = [],
         location: str = "us-central1",
         max_output_tokens: int = 128,
         model_name: str = "chat-bison",
         temperature: float = 0.0,
         top_k: int = 40,
         top_p: float = 0.95,
         verbose: bool = False,
@@ -108,15 +106,14 @@
             from langchain_google_vertexai import ChatVertexAI  # type: ignore
         except ImportError:
             raise ImportError(
                 "To use the ChatVertexAI model, you need to install the langchain-google-vertexai package."
             )
         output = ChatVertexAI(
             credentials=credentials,
-            examples=examples,
             location=location,
             max_output_tokens=max_output_tokens,
             model_name=model_name,
             project=project,
             temperature=temperature,
             top_k=top_k,
             top_p=top_p,
```

### Comparing `langflow_base-0.0.48/langflow/components/models/__init__.py` & `langflow_base-0.0.49/langflow/components/models/__init__.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/outputs/ChatOutput.py` & `langflow_base-0.0.49/langflow/components/outputs/ChatOutput.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/outputs/TextOutput.py` & `langflow_base-0.0.49/langflow/components/outputs/TextOutput.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/retrievers/AmazonKendra.py` & `langflow_base-0.0.49/langflow/components/retrievers/AmazonKendra.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional
-from langchain_community.retrievers import AmazonKendraRetriever
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langchain_community.retrievers import AmazonKendraRetriever
 from langchain_core.retrievers import BaseRetriever
 
+from langflow.custom import CustomComponent
+
 
 class AmazonKendraRetrieverComponent(CustomComponent):
     display_name: str = "Amazon Kendra Retriever"
     description: str = "Retriever that uses the Amazon Kendra API."
     icon = "Amazon"
 
     def build_config(self):
```

### Comparing `langflow_base-0.0.48/langflow/components/retrievers/MetalRetriever.py` & `langflow_base-0.0.49/langflow/components/retrievers/MetalRetriever.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional
+
 from langchain_community.retrievers import MetalRetriever
+from langchain_core.retrievers import BaseRetriever
 from metal_sdk.metal import Metal  # type: ignore
 
-from langflow.interface.custom.custom_component import CustomComponent
-from langchain_core.retrievers import BaseRetriever
+from langflow.custom import CustomComponent
 
 
 class MetalRetrieverComponent(CustomComponent):
     display_name: str = "Metal Retriever"
     description: str = "Retriever that uses the Metal API."
 
     def build_config(self):
```

### Comparing `langflow_base-0.0.48/langflow/components/retrievers/MultiQueryRetriever.py` & `langflow_base-0.0.49/langflow/components/retrievers/MultiQueryRetriever.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional
 
 from langchain.retrievers import MultiQueryRetriever
 
-from langflow.field_typing import BaseRetriever, PromptTemplate, BaseLanguageModel
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
+from langflow.field_typing import BaseLanguageModel, BaseRetriever, PromptTemplate, Text
 
 
 class MultiQueryRetrieverComponent(CustomComponent):
     display_name = "MultiQueryRetriever"
     description = "Initialize from llm using default template."
     documentation = "https://python.langchain.com/docs/modules/data_connection/retrievers/how_to/MultiQueryRetriever"
 
@@ -37,14 +37,17 @@
             "parser_key": {"display_name": "Parser Key", "default": "lines"},
         }
 
     def build(
         self,
         llm: BaseLanguageModel,
         retriever: BaseRetriever,
-        prompt: Optional[PromptTemplate] = None,
+        prompt: Optional[Text] = None,
         parser_key: str = "lines",
     ) -> MultiQueryRetriever:
         if not prompt:
             return MultiQueryRetriever.from_llm(llm=llm, retriever=retriever, parser_key=parser_key)
         else:
-            return MultiQueryRetriever.from_llm(llm=llm, retriever=retriever, prompt=prompt, parser_key=parser_key)
+            prompt_template = PromptTemplate.from_template(prompt)
+            return MultiQueryRetriever.from_llm(
+                llm=llm, retriever=retriever, prompt=prompt_template, parser_key=parser_key
+            )
```

### Comparing `langflow_base-0.0.48/langflow/components/retrievers/VectaraSelfQueryRetriver.py` & `langflow_base-0.0.49/langflow/components/retrievers/VectaraSelfQueryRetriver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import json
 from typing import List
+
 from langchain.chains.query_constructor.base import AttributeInfo
 from langchain.retrievers.self_query.base import SelfQueryRetriever
-
-from langflow.interface.custom.custom_component import CustomComponent
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.retrievers import BaseRetriever
 from langchain_core.vectorstores import VectorStore
 
+from langflow.custom import CustomComponent
+
 
 class VectaraSelfQueryRetriverComponent(CustomComponent):
     """
     A custom component for implementing Vectara Self Query Retriever using a vector store.
     """
 
     display_name: str = "Vectara Self Query Retriever for Vectara Vector Store"
```

### Comparing `langflow_base-0.0.48/langflow/components/textsplitters/CharacterTextSplitter.py` & `langflow_base-0.0.49/langflow/components/textsplitters/CharacterTextSplitter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langchain_text_splitters import CharacterTextSplitter
+
+from langflow.custom import CustomComponent
 from langflow.schema.schema import Record
 from langflow.utils.util import unescape_string
-from langchain_text_splitters import CharacterTextSplitter
 
 
 class CharacterTextSplitterComponent(CustomComponent):
     display_name = "CharacterTextSplitter"
     description = "Splitting text that looks at characters."
 
     def build_config(self):
```

### Comparing `langflow_base-0.0.48/langflow/components/textsplitters/LanguageRecursiveTextSplitter.py` & `langflow_base-0.0.49/langflow/components/textsplitters/LanguageRecursiveTextSplitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List, Optional
 
-from langflow.interface.custom.custom_component import CustomComponent
-from langflow.schema.schema import Record
 from langchain_text_splitters import Language, RecursiveCharacterTextSplitter
 
+from langflow.custom import CustomComponent
+from langflow.schema.schema import Record
+
 
 class LanguageRecursiveTextSplitterComponent(CustomComponent):
     display_name: str = "Language Recursive Text Splitter"
     description: str = "Split text into chunks of a specified length based on language."
     documentation: str = "https://docs.langflow.org/components/text-splitters#languagerecursivetextsplitter"
 
     def build_config(self):
```

### Comparing `langflow_base-0.0.48/langflow/components/textsplitters/RecursiveCharacterTextSplitter.py` & `langflow_base-0.0.49/langflow/components/textsplitters/RecursiveCharacterTextSplitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Optional
+
 from langchain_core.documents import Document
+from langchain_text_splitters import RecursiveCharacterTextSplitter
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 from langflow.schema import Record
 from langflow.utils.util import build_loader_repr_from_records, unescape_string
-from langchain_text_splitters import RecursiveCharacterTextSplitter
 
 
 class RecursiveCharacterTextSplitterComponent(CustomComponent):
     display_name: str = "Recursive Character Text Splitter"
     description: str = "Split text into chunks of a specified length."
     documentation: str = "https://docs.langflow.org/components/text-splitters#recursivecharactertextsplitter"
```

### Comparing `langflow_base-0.0.48/langflow/components/toolkits/Metaphor.py` & `langflow_base-0.0.49/langflow/components/toolkits/Metaphor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List, Union
-from metaphor_python import Metaphor  # type: ignore
 
-from langflow.interface.custom.custom_component import CustomComponent
 from langchain_community.agent_toolkits.base import BaseToolkit
 from langchain_core.tools import Tool, tool
+from metaphor_python import Metaphor  # type: ignore
+
+from langflow.custom import CustomComponent
 
 
 class MetaphorToolkit(CustomComponent):
     display_name: str = "Metaphor"
     description: str = "Metaphor Toolkit"
     documentation = "https://python.langchain.com/docs/integrations/tools/metaphor_search"
     beta: bool = True
```

### Comparing `langflow_base-0.0.48/langflow/components/toolkits/VectorStoreInfo.py` & `langflow_base-0.0.49/langflow/components/toolkits/VectorStoreInfo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from langchain.agents.agent_toolkits.vectorstore.toolkit import VectorStoreInfo
-
-from langflow.interface.custom.custom_component import CustomComponent
 from langchain_core.vectorstores import VectorStore
 
+from langflow.custom import CustomComponent
+
 
 class VectorStoreInfoComponent(CustomComponent):
     display_name = "VectorStoreInfo"
     description = "Information about a VectorStore"
 
     def build_config(self):
         return {
```

### Comparing `langflow_base-0.0.48/langflow/components/toolkits/VectorStoreRouterToolkit.py` & `langflow_base-0.0.49/langflow/components/toolkits/VectorStoreRouterToolkit.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Union
 
 from langchain.agents.agent_toolkits.vectorstore.toolkit import VectorStoreInfo, VectorStoreRouterToolkit
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import BaseLanguageModel, Tool
-from langflow.interface.custom.custom_component import CustomComponent
 
 
 class VectorStoreRouterToolkitComponent(CustomComponent):
     display_name = "VectorStoreRouterToolkit"
     description = "Toolkit for routing between Vector Stores."
 
     def build_config(self):
```

### Comparing `langflow_base-0.0.48/langflow/components/toolkits/VectorStoreToolkit.py` & `langflow_base-0.0.49/langflow/components/toolkits/VectorStoreToolkit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Union
 
 from langchain.agents.agent_toolkits.vectorstore.toolkit import VectorStoreInfo, VectorStoreToolkit
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import BaseLanguageModel, Tool
-from langflow.interface.custom.custom_component import CustomComponent
 
 
 class VectorStoreToolkitComponent(CustomComponent):
     display_name = "VectorStoreToolkit"
     description = "Toolkit for interacting with a Vector Store."
 
     def build_config(self):
```

### Comparing `langflow_base-0.0.48/langflow/components/tools/PythonREPLTool.py` & `langflow_base-0.0.49/langflow/components/tools/PythonREPLTool.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/tools/SearchAPITool.py` & `langflow_base-0.0.49/langflow/components/tools/SearchAPITool.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/tools/SearchApi.py` & `langflow_base-0.0.49/langflow/components/tools/SearchApi.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/vectorsearch/AstraDBSearch.py` & `langflow_base-0.0.49/langflow/components/vectorsearch/AstraDBSearch.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/vectorsearch/ChromaSearch.py` & `langflow_base-0.0.49/langflow/components/vectorstores/Chroma.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,111 +1,122 @@
-from typing import List, Optional
+from typing import List, Optional, Union
 
-import chromadb  # type: ignore
-from langchain_community.vectorstores.chroma import Chroma
-
-from langflow.components.vectorstores.base.model import LCVectorStoreComponent
-from langflow.field_typing import Embeddings, Text
-from langflow.schema import Record
-
-
-class ChromaSearchComponent(LCVectorStoreComponent):
-    display_name: str = "Chroma Search"
-    description: str = "Search a Chroma collection for similar documents."
+from chromadb.config import Settings
+from langchain_chroma import Chroma
+from langchain_core.embeddings import Embeddings
+from langchain_core.retrievers import BaseRetriever
+from langchain_core.vectorstores import VectorStore
+
+from langflow.custom import CustomComponent
+from langflow.schema.schema import Record
+
+
+class ChromaComponent(CustomComponent):
+    """
+    A custom component for implementing a Vector Store using Chroma.
+    """
+
+    display_name: str = "Chroma"
+    description: str = "Implementation of Vector Store using Chroma"
+    documentation = "https://python.langchain.com/docs/integrations/vectorstores/chroma"
     icon = "Chroma"
 
     def build_config(self):
         """
         Builds the configuration for the component.
 
         Returns:
         - dict: A dictionary containing the configuration options for the component.
         """
         return {
-            "input_value": {"display_name": "Input"},
-            "search_type": {
-                "display_name": "Search Type",
-                "options": ["Similarity", "MMR"],
-            },
             "collection_name": {"display_name": "Collection Name", "value": "langflow"},
-            # "persist": {"display_name": "Persist"},
-            "index_directory": {"display_name": "Index Directory"},
-            "code": {"show": False, "display_name": "Code"},
-            "embedding": {
-                "display_name": "Embedding",
-                "info": "Embedding model to vectorize inputs (make sure to use same as index)",
-            },
+            "index_directory": {"display_name": "Persist Directory"},
+            "code": {"advanced": True, "display_name": "Code"},
+            "inputs": {"display_name": "Input", "input_types": ["Document", "Record"]},
+            "embedding": {"display_name": "Embedding"},
             "chroma_server_cors_allow_origins": {
                 "display_name": "Server CORS Allow Origins",
                 "advanced": True,
             },
             "chroma_server_host": {"display_name": "Server Host", "advanced": True},
-            "chroma_server_port": {"display_name": "Server Port", "advanced": True},
+            "chroma_server_http_port": {"display_name": "Server HTTP Port", "advanced": True},
             "chroma_server_grpc_port": {
                 "display_name": "Server gRPC Port",
                 "advanced": True,
             },
             "chroma_server_ssl_enabled": {
                 "display_name": "Server SSL Enabled",
                 "advanced": True,
             },
-            "number_of_results": {
-                "display_name": "Number of Results",
-                "info": "Number of results to return.",
-                "advanced": True,
-            },
         }
 
     def build(
         self,
-        input_value: Text,
-        search_type: str,
         collection_name: str,
         embedding: Embeddings,
         chroma_server_ssl_enabled: bool,
-        number_of_results: int = 4,
         index_directory: Optional[str] = None,
-        chroma_server_cors_allow_origins: Optional[str] = None,
+        inputs: Optional[List[Record]] = None,
+        chroma_server_cors_allow_origins: List[str] = [],
         chroma_server_host: Optional[str] = None,
-        chroma_server_port: Optional[int] = None,
+        chroma_server_http_port: Optional[int] = None,
         chroma_server_grpc_port: Optional[int] = None,
-    ) -> List[Record]:
+    ) -> Union[VectorStore, BaseRetriever]:
         """
         Builds the Vector Store or BaseRetriever object.
 
         Args:
         - collection_name (str): The name of the collection.
-        - persist_directory (Optional[str]): The directory to persist the Vector Store to.
+        - embedding (Embeddings): The embeddings to use for the Vector Store.
         - chroma_server_ssl_enabled (bool): Whether to enable SSL for the Chroma server.
-        - persist (bool): Whether to persist the Vector Store or not.
-        - embedding (Optional[Embeddings]): The embeddings to use for the Vector Store.
-        - documents (Optional[Document]): The documents to use for the Vector Store.
-        - chroma_server_cors_allow_origins (Optional[str]): The CORS allow origins for the Chroma server.
+        - index_directory (Optional[str]): The directory to persist the Vector Store to.
+        - inputs (Optional[List[Record]]): The input records to use for the Vector Store.
+        - chroma_server_cors_allow_origins (List[str]): The CORS allow origins for the Chroma server.
         - chroma_server_host (Optional[str]): The host for the Chroma server.
-        - chroma_server_port (Optional[int]): The port for the Chroma server.
+        - chroma_server_http_port (Optional[int]): The HTTP port for the Chroma server.
         - chroma_server_grpc_port (Optional[int]): The gRPC port for the Chroma server.
 
         Returns:
         - Union[VectorStore, BaseRetriever]: The Vector Store or BaseRetriever object.
         """
 
         # Chroma settings
         chroma_settings = None
 
         if chroma_server_host is not None:
-            chroma_settings = chromadb.config.Settings(
-                chroma_server_cors_allow_origins=chroma_server_cors_allow_origins or None,
+            chroma_settings = Settings(
+                chroma_server_cors_allow_origins=chroma_server_cors_allow_origins or [],
                 chroma_server_host=chroma_server_host,
-                chroma_server_port=chroma_server_port or None,
+                chroma_server_http_port=chroma_server_http_port or None,
                 chroma_server_grpc_port=chroma_server_grpc_port or None,
                 chroma_server_ssl_enabled=chroma_server_ssl_enabled,
             )
-        if index_directory:
+
+        # If documents, then we need to create a Chroma instance using .from_documents
+
+        # Check index_directory and expand it if it is a relative path
+        if index_directory is not None:
             index_directory = self.resolve_path(index_directory)
-        vector_store = Chroma(
-            embedding_function=embedding,
-            collection_name=collection_name,
-            persist_directory=index_directory,
-            client_settings=chroma_settings,
-        )
 
-        return self.search_with_vector_store(input_value, search_type, vector_store, k=number_of_results)
+        documents = []
+        for _input in inputs or []:
+            if isinstance(_input, Record):
+                documents.append(_input.to_lc_document())
+            else:
+                documents.append(_input)
+        if documents is not None and embedding is not None:
+            if len(documents) == 0:
+                raise ValueError("If documents are provided, there must be at least one document.")
+            chroma = Chroma.from_documents(
+                documents=documents,  # type: ignore
+                persist_directory=index_directory,
+                collection_name=collection_name,
+                embedding=embedding,
+                client_settings=chroma_settings,
+            )
+        else:
+            chroma = Chroma(
+                persist_directory=index_directory,
+                client_settings=chroma_settings,
+                embedding_function=embedding,
+            )
+        return chroma
```

### Comparing `langflow_base-0.0.48/langflow/components/vectorsearch/CouchbaseSearch.py` & `langflow_base-0.0.49/langflow/components/vectorsearch/CouchbaseSearch.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/vectorsearch/FAISSSearch.py` & `langflow_base-0.0.49/langflow/components/vectorsearch/FAISSSearch.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/vectorsearch/MongoDBAtlasVectorSearch.py` & `langflow_base-0.0.49/langflow/components/vectorsearch/MongoDBAtlasVectorSearch.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/vectorsearch/PineconeSearch.py` & `langflow_base-0.0.49/langflow/components/vectorsearch/PineconeSearch.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             "search_type": {
                 "display_name": "Search Type",
                 "options": ["Similarity", "MMR"],
             },
             "input_value": {"display_name": "Input"},
             "embedding": {"display_name": "Embedding"},
             "index_name": {"display_name": "Index Name"},
-            "namespace": {"display_name": "Namespace", "advanced": True},
+            "namespace": {"display_name": "Namespace", "info": "Namespace for the index."},
             "distance_strategy": {
                 "display_name": "Distance Strategy",
                 # get values from enum
                 # and make them title case for display
                 "options": distance_options,
                 "advanced": True,
                 "value": distance_value,
```

### Comparing `langflow_base-0.0.48/langflow/components/vectorsearch/QdrantSearch.py` & `langflow_base-0.0.49/langflow/components/vectorstores/Qdrant.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-from typing import List, Optional
+from typing import Optional, Union
 
-from langflow.components.vectorstores.base.model import LCVectorStoreComponent
-from langflow.components.vectorstores.Qdrant import QdrantComponent
-from langflow.field_typing import Embeddings, NestedDict, Text
-from langflow.schema import Record
+from langchain_community.vectorstores.qdrant import Qdrant
+from langchain_core.retrievers import BaseRetriever
+from langchain_core.vectorstores import VectorStore
 
+from langflow.custom import CustomComponent
+from langflow.field_typing import Embeddings
+from langflow.schema.schema import Record
 
-class QdrantSearchComponent(QdrantComponent, LCVectorStoreComponent):
-    display_name = "Qdrant Search"
+
+class QdrantComponent(CustomComponent):
+    display_name = "Qdrant"
     description = "Construct Qdrant wrapper from a list of texts."
     icon = "Qdrant"
 
     def build_config(self):
         return {
-            "search_type": {
-                "display_name": "Search Type",
-                "options": ["Similarity", "MMR"],
-            },
-            "input_value": {"display_name": "Input"},
+            "inputs": {"display_name": "Input", "input_types": ["Document", "Record"]},
             "embedding": {"display_name": "Embedding"},
             "api_key": {"display_name": "API Key", "password": True, "advanced": True},
             "collection_name": {"display_name": "Collection Name"},
             "content_payload_key": {
                 "display_name": "Content Payload Key",
                 "advanced": True,
             },
@@ -34,70 +33,83 @@
                 "display_name": "Metadata Payload Key",
                 "advanced": True,
             },
             "path": {"display_name": "Path", "advanced": True},
             "port": {"display_name": "Port", "advanced": True},
             "prefer_grpc": {"display_name": "Prefer gRPC", "advanced": True},
             "prefix": {"display_name": "Prefix", "advanced": True},
-            "search_kwargs": {"display_name": "Search Kwargs", "advanced": True},
             "timeout": {"display_name": "Timeout", "advanced": True},
             "url": {"display_name": "URL", "advanced": True},
-            "number_of_results": {
-                "display_name": "Number of Results",
-                "info": "Number of results to return.",
-                "advanced": True,
-            },
         }
 
-    def build(  # type: ignore[override]
+    def build(
         self,
-        input_value: Text,
         embedding: Embeddings,
         collection_name: str,
-        number_of_results: int = 4,
-        search_type: str = "similarity",
+        inputs: Optional[Record] = None,
         api_key: Optional[str] = None,
         content_payload_key: str = "page_content",
         distance_func: str = "Cosine",
         grpc_port: int = 6334,
         https: bool = False,
         host: Optional[str] = None,
         location: Optional[str] = None,
         metadata_payload_key: str = "metadata",
         path: Optional[str] = None,
         port: Optional[int] = 6333,
         prefer_grpc: bool = False,
         prefix: Optional[str] = None,
-        search_kwargs: Optional[NestedDict] = None,
         timeout: Optional[int] = None,
         url: Optional[str] = None,
-    ) -> List[Record]:  # type: ignore[override]
-        vector_store = super().build(
-            embedding=embedding,
-            collection_name=collection_name,
-            api_key=api_key,
-            content_payload_key=content_payload_key,
-            distance_func=distance_func,
-            grpc_port=grpc_port,
-            https=https,
-            host=host,
-            location=location,
-            metadata_payload_key=metadata_payload_key,
-            path=path,
-            port=port,
-            prefer_grpc=prefer_grpc,
-            prefix=prefix,
-            timeout=timeout,
-            url=url,
-        )
-        if not vector_store:
-            raise ValueError("Failed to load the Qdrant index.")
-        if search_kwargs is None:
-            search_kwargs = {}
-
-        return self.search_with_vector_store(
-            vector_store=vector_store,
-            input_value=input_value,
-            search_type=search_type,
-            k=number_of_results,
-            **search_kwargs,
-        )
+    ) -> Union[VectorStore, Qdrant, BaseRetriever]:
+        documents = []
+        for _input in inputs or []:
+            if isinstance(_input, Record):
+                documents.append(_input.to_lc_document())
+            else:
+                documents.append(_input)
+        if documents is None:
+            from qdrant_client import QdrantClient
+
+            client = QdrantClient(
+                location=location,
+                url=host,
+                port=port,
+                grpc_port=grpc_port,
+                https=https,
+                prefix=prefix,
+                timeout=timeout,
+                prefer_grpc=prefer_grpc,
+                metadata_payload_key=metadata_payload_key,
+                content_payload_key=content_payload_key,
+                api_key=api_key,
+                collection_name=collection_name,
+                host=host,
+                path=path,
+            )
+            vs = Qdrant(
+                client=client,
+                collection_name=collection_name,
+                embeddings=embedding,
+            )
+            return vs
+        else:
+            vs = Qdrant.from_documents(
+                documents=documents,  # type: ignore
+                embedding=embedding,
+                api_key=api_key,
+                collection_name=collection_name,
+                content_payload_key=content_payload_key,
+                distance_func=distance_func,
+                grpc_port=grpc_port,
+                host=host,
+                https=https,
+                location=location,
+                metadata_payload_key=metadata_payload_key,
+                path=path,
+                port=port,
+                prefer_grpc=prefer_grpc,
+                prefix=prefix,
+                timeout=timeout,
+                url=url,
+            )
+        return vs
```

### Comparing `langflow_base-0.0.48/langflow/components/vectorsearch/RedisSearch.py` & `langflow_base-0.0.49/langflow/components/vectorsearch/RedisSearch.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/vectorsearch/SupabaseVectorStoreSearch.py` & `langflow_base-0.0.49/langflow/components/vectorsearch/SupabaseVectorStoreSearch.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/vectorsearch/VectaraSearch.py` & `langflow_base-0.0.49/langflow/components/vectorsearch/VectaraSearch.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/vectorsearch/__init__.py` & `langflow_base-0.0.49/langflow/components/vectorsearch/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .PineconeSearch import PineconeSearchComponent
 from .QdrantSearch import QdrantSearchComponent
 from .RedisSearch import RedisSearchComponent
 from .SupabaseVectorStoreSearch import SupabaseSearchComponent
 from .VectaraSearch import VectaraSearchComponent
 from .WeaviateSearch import WeaviateSearchVectorStore
 from .pgvectorSearch import PGVectorSearchComponent
-from .Couchbase import CouchbaseSearchComponent # type: ignore
+from .Couchbase import CouchbaseSearchComponent  # type: ignore
 
 __all__ = [
     "AstraDBSearchComponent",
     "ChromaSearchComponent",
     "CouchbaseSearchComponent",
     "FAISSSearchComponent",
     "MongoDBAtlasSearchComponent",
```

### Comparing `langflow_base-0.0.48/langflow/components/vectorsearch/pgvectorSearch.py` & `langflow_base-0.0.49/langflow/components/vectorsearch/pgvectorSearch.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/vectorstores/AstraDB.py` & `langflow_base-0.0.49/langflow/components/vectorstores/AstraDB.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/vectorstores/Chroma.py` & `langflow_base-0.0.49/langflow/components/vectorsearch/ChromaSearch.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,122 +1,112 @@
-from typing import List, Optional, Union
+from typing import List, Optional
 
-import chromadb  # type: ignore
-from langchain_community.vectorstores.chroma import Chroma
+from chromadb.config import Settings
+from langchain_chroma import Chroma
 
-from langflow.interface.custom.custom_component import CustomComponent
-from langflow.schema.schema import Record
-from langchain_core.embeddings import Embeddings
-from langchain_core.retrievers import BaseRetriever
-from langchain_core.vectorstores import VectorStore
-
-
-class ChromaComponent(CustomComponent):
-    """
-    A custom component for implementing a Vector Store using Chroma.
-    """
-
-    display_name: str = "Chroma"
-    description: str = "Implementation of Vector Store using Chroma"
-    documentation = "https://python.langchain.com/docs/integrations/vectorstores/chroma"
+from langflow.components.vectorstores.base.model import LCVectorStoreComponent
+from langflow.field_typing import Embeddings, Text
+from langflow.schema import Record
+
+
+class ChromaSearchComponent(LCVectorStoreComponent):
+    display_name: str = "Chroma Search"
+    description: str = "Search a Chroma collection for similar documents."
     icon = "Chroma"
 
     def build_config(self):
         """
         Builds the configuration for the component.
 
         Returns:
         - dict: A dictionary containing the configuration options for the component.
         """
         return {
+            "input_value": {"display_name": "Input"},
+            "search_type": {
+                "display_name": "Search Type",
+                "options": ["Similarity", "MMR"],
+            },
             "collection_name": {"display_name": "Collection Name", "value": "langflow"},
-            "index_directory": {"display_name": "Persist Directory"},
-            "code": {"advanced": True, "display_name": "Code"},
-            "inputs": {"display_name": "Input", "input_types": ["Document", "Record"]},
-            "embedding": {"display_name": "Embedding"},
+            # "persist": {"display_name": "Persist"},
+            "index_directory": {"display_name": "Index Directory"},
+            "code": {"show": False, "display_name": "Code"},
+            "embedding": {
+                "display_name": "Embedding",
+                "info": "Embedding model to vectorize inputs (make sure to use same as index)",
+            },
             "chroma_server_cors_allow_origins": {
                 "display_name": "Server CORS Allow Origins",
                 "advanced": True,
             },
             "chroma_server_host": {"display_name": "Server Host", "advanced": True},
-            "chroma_server_port": {"display_name": "Server Port", "advanced": True},
+            "chroma_server_http_port": {"display_name": "Server HTTP Port", "advanced": True},
             "chroma_server_grpc_port": {
                 "display_name": "Server gRPC Port",
                 "advanced": True,
             },
             "chroma_server_ssl_enabled": {
                 "display_name": "Server SSL Enabled",
                 "advanced": True,
             },
+            "number_of_results": {
+                "display_name": "Number of Results",
+                "info": "Number of results to return.",
+                "advanced": True,
+            },
         }
 
     def build(
         self,
+        input_value: Text,
+        search_type: str,
         collection_name: str,
         embedding: Embeddings,
         chroma_server_ssl_enabled: bool,
+        number_of_results: int = 4,
         index_directory: Optional[str] = None,
-        inputs: Optional[List[Record]] = None,
-        chroma_server_cors_allow_origins: Optional[str] = None,
+        chroma_server_cors_allow_origins: List[str] = [],
         chroma_server_host: Optional[str] = None,
-        chroma_server_port: Optional[int] = None,
+        chroma_server_http_port: Optional[int] = None,
         chroma_server_grpc_port: Optional[int] = None,
-    ) -> Union[VectorStore, BaseRetriever]:
+    ) -> List[Record]:
         """
         Builds the Vector Store or BaseRetriever object.
 
         Args:
+        - input_value (Text): The input value.
+        - search_type (str): The type of search.
         - collection_name (str): The name of the collection.
-        - index_directory (Optional[str]): The directory to persist the Vector Store to.
+        - embedding (Embeddings): The embeddings to use for the Vector Store.
         - chroma_server_ssl_enabled (bool): Whether to enable SSL for the Chroma server.
-        - embedding (Optional[Embeddings]): The embeddings to use for the Vector Store.
-        - documents (Optional[Document]): The documents to use for the Vector Store.
-        - chroma_server_cors_allow_origins (Optional[str]): The CORS allow origins for the Chroma server.
-        - chroma_server_host (Optional[str]): The host for the Chroma server.
-        - chroma_server_port (Optional[int]): The port for the Chroma server.
-        - chroma_server_grpc_port (Optional[int]): The gRPC port for the Chroma server.
+        - number_of_results (int, optional): The number of results to retrieve. Defaults to 4.
+        - index_directory (str, optional): The directory to persist the Vector Store to. Defaults to None.
+        - chroma_server_cors_allow_origins (List[str], optional): The CORS allow origins for the Chroma server. Defaults to [].
+        - chroma_server_host (str, optional): The host for the Chroma server. Defaults to None.
+        - chroma_server_http_port (int, optional): The HTTP port for the Chroma server. Defaults to None.
+        - chroma_server_grpc_port (int, optional): The gRPC port for the Chroma server. Defaults to None.
 
         Returns:
-        - Union[VectorStore, BaseRetriever]: The Vector Store or BaseRetriever object.
+        - List[Record]: The list of records.
         """
 
         # Chroma settings
         chroma_settings = None
 
         if chroma_server_host is not None:
-            chroma_settings = chromadb.config.Settings(
-                chroma_server_cors_allow_origins=chroma_server_cors_allow_origins or None,
+            chroma_settings = Settings(
+                chroma_server_cors_allow_origins=chroma_server_cors_allow_origins or [],
                 chroma_server_host=chroma_server_host,
-                chroma_server_port=chroma_server_port or None,
+                chroma_server_http_port=chroma_server_http_port or None,
                 chroma_server_grpc_port=chroma_server_grpc_port or None,
                 chroma_server_ssl_enabled=chroma_server_ssl_enabled,
             )
-
-        # If documents, then we need to create a Chroma instance using .from_documents
-
-        # Check index_directory and expand it if it is a relative path
-        if index_directory is not None:
+        if index_directory:
             index_directory = self.resolve_path(index_directory)
+        vector_store = Chroma(
+            embedding_function=embedding,
+            collection_name=collection_name,
+            persist_directory=index_directory,
+            client_settings=chroma_settings,
+        )
 
-        documents = []
-        for _input in inputs or []:
-            if isinstance(_input, Record):
-                documents.append(_input.to_lc_document())
-            else:
-                documents.append(_input)
-        if documents is not None and embedding is not None:
-            if len(documents) == 0:
-                raise ValueError("If documents are provided, there must be at least one document.")
-            chroma = Chroma.from_documents(
-                documents=documents,  # type: ignore
-                persist_directory=index_directory,
-                collection_name=collection_name,
-                embedding=embedding,
-                client_settings=chroma_settings,
-            )
-        else:
-            chroma = Chroma(
-                persist_directory=index_directory,
-                client_settings=chroma_settings,
-                embedding_function=embedding,
-            )
-        return chroma
+        return self.search_with_vector_store(input_value, search_type, vector_store, k=number_of_results)
```

### Comparing `langflow_base-0.0.48/langflow/components/vectorstores/Couchbase.py` & `langflow_base-0.0.49/langflow/components/vectorstores/Couchbase.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/vectorstores/FAISS.py` & `langflow_base-0.0.49/langflow/components/vectorstores/FAISS.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import List, Text, Union
+
 from langchain_community.vectorstores.faiss import FAISS
+from langchain_core.retrievers import BaseRetriever
+from langchain_core.vectorstores import VectorStore
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import Embeddings
-from langflow.interface.custom.custom_component import CustomComponent
 from langflow.schema.schema import Record
-from langchain_core.retrievers import BaseRetriever
-from langchain_core.vectorstores import VectorStore
 
 
 class FAISSComponent(CustomComponent):
     display_name = "FAISS"
     description = "Ingest documents into FAISS Vector Store."
     documentation = "https://python.langchain.com/docs/modules/data_connection/vectorstores/integrations/faiss"
```

### Comparing `langflow_base-0.0.48/langflow/components/vectorstores/MongoDBAtlasVector.py` & `langflow_base-0.0.49/langflow/components/vectorstores/MongoDBAtlasVector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List, Optional
 
 from langchain_community.vectorstores.mongodb_atlas import MongoDBAtlasVectorSearch
+
+from langflow.custom import CustomComponent
 from langflow.field_typing import Embeddings
-from langflow.interface.custom.custom_component import CustomComponent
 from langflow.schema.schema import Record
 
 
 class MongoDBAtlasComponent(CustomComponent):
     display_name = "MongoDB Atlas"
     description = "Construct a `MongoDB Atlas Vector Search` vector store from raw documents."
     icon = "MongoDB"
```

### Comparing `langflow_base-0.0.48/langflow/components/vectorstores/Pinecone.py` & `langflow_base-0.0.49/langflow/components/vectorstores/Pinecone.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from typing import List, Optional, Union
+
 from langchain_core.documents import Document
+from langchain_core.retrievers import BaseRetriever
+from langchain_core.vectorstores import VectorStore
 from langchain_pinecone._utilities import DistanceStrategy
 from langchain_pinecone.vectorstores import PineconeVectorStore
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import Embeddings
-from langflow.interface.custom.custom_component import CustomComponent
 from langflow.schema.schema import Record
-from langchain_core.retrievers import BaseRetriever
-from langchain_core.vectorstores import VectorStore
 
 
 class PineconeComponent(CustomComponent):
     display_name = "Pinecone"
     description = "Construct Pinecone wrapper from raw documents."
     icon = "Pinecone"
     field_order = ["index_name", "namespace", "distance_strategy", "pinecone_api_key", "documents", "embedding"]
```

### Comparing `langflow_base-0.0.48/langflow/components/vectorstores/Redis.py` & `langflow_base-0.0.49/langflow/components/vectorstores/Redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Optional, Union
+
 from langchain_community.vectorstores.redis import Redis
+from langchain_core.embeddings import Embeddings
 from langchain_core.retrievers import BaseRetriever
+from langchain_core.vectorstores import VectorStore
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 from langflow.schema.schema import Record
-from langchain_core.embeddings import Embeddings
-from langchain_core.vectorstores import VectorStore
 
 
 class RedisComponent(CustomComponent):
     """
     A custom component for implementing a Vector Store using Redis.
     """
```

### Comparing `langflow_base-0.0.48/langflow/components/vectorstores/SupabaseVectorStore.py` & `langflow_base-0.0.49/langflow/components/vectorstores/SupabaseVectorStore.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import List, Optional, Union
+
 from langchain_community.vectorstores.supabase import SupabaseVectorStore
+from langchain_core.retrievers import BaseRetriever
+from langchain_core.vectorstores import VectorStore
 from supabase.client import Client, create_client
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import Embeddings
-from langflow.interface.custom.custom_component import CustomComponent
 from langflow.schema.schema import Record
-from langchain_core.retrievers import BaseRetriever
-from langchain_core.vectorstores import VectorStore
 
 
 class SupabaseComponent(CustomComponent):
     display_name = "Supabase"
     description = "Return VectorStore initialized from texts and embeddings."
 
     def build_config(self):
```

### Comparing `langflow_base-0.0.48/langflow/components/vectorstores/Vectara.py` & `langflow_base-0.0.49/langflow/components/vectorstores/Vectara.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import urllib.request
 from typing import List, Optional, Union
 
 from langchain_community.embeddings import FakeEmbeddings
 from langchain_community.vectorstores.vectara import Vectara
 from langchain_core.vectorstores import VectorStore
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import BaseRetriever
-from langflow.interface.custom.custom_component import CustomComponent
 from langflow.schema.schema import Record
 
 
 class VectaraComponent(CustomComponent):
     display_name: str = "Vectara"
     description: str = "Implementation of Vector Store using Vectara"
     documentation = "https://python.langchain.com/docs/integrations/vectorstores/vectara"
```

### Comparing `langflow_base-0.0.48/langflow/components/vectorstores/Weaviate.py` & `langflow_base-0.0.49/langflow/components/vectorstores/Weaviate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Optional, Union
 
 import weaviate  # type: ignore
 from langchain_community.vectorstores import Weaviate
 from langchain_core.documents import Document
-
-from langflow.interface.custom.custom_component import CustomComponent
-from langflow.schema.schema import Record
 from langchain_core.embeddings import Embeddings
 from langchain_core.retrievers import BaseRetriever
 from langchain_core.vectorstores import VectorStore
 
+from langflow.custom import CustomComponent
+from langflow.schema.schema import Record
+
 
 class WeaviateVectorStoreComponent(CustomComponent):
     display_name: str = "Weaviate"
     description: str = "Implementation of Vector Store using Weaviate"
     documentation = "https://python.langchain.com/docs/integrations/vectorstores/weaviate"
     field_config = {
         "url": {"display_name": "Weaviate URL", "value": "http://localhost:8080"},
```

### Comparing `langflow_base-0.0.48/langflow/components/vectorstores/__init__.py` & `langflow_base-0.0.49/langflow/components/vectorstores/__init__.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/components/vectorstores/base/model.py` & `langflow_base-0.0.49/langflow/components/vectorstores/base/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import List, Union
 
 from langchain_core.documents import Document
 from langchain_core.retrievers import BaseRetriever
 from langchain_core.vectorstores import VectorStore
 
+from langflow.custom import CustomComponent
 from langflow.field_typing import Text
 from langflow.helpers.record import docs_to_records
-from langflow.interface.custom.custom_component import CustomComponent
 from langflow.schema import Record
 
 
 class LCVectorStoreComponent(CustomComponent):
     display_name: str = "LC Vector Store"
     description: str = "Search a LC Vector Store for similar documents."
```

### Comparing `langflow_base-0.0.48/langflow/components/vectorstores/pgvector.py` & `langflow_base-0.0.49/langflow/components/vectorstores/pgvector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Optional, Union
+
 from langchain_community.vectorstores.pgvector import PGVector
+from langchain_core.embeddings import Embeddings
 from langchain_core.retrievers import BaseRetriever
+from langchain_core.vectorstores import VectorStore
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 from langflow.schema.schema import Record
-from langchain_core.embeddings import Embeddings
-from langchain_core.vectorstores import VectorStore
 
 
 class PGVectorComponent(CustomComponent):
     """
     A custom component for implementing a Vector Store using PostgreSQL.
     """
```

### Comparing `langflow_base-0.0.48/langflow/config.yaml` & `langflow_base-0.0.49/langflow/config.yaml`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/core/celeryconfig.py` & `langflow_base-0.0.49/langflow/core/celeryconfig.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/field_typing/__init__.py` & `langflow_base-0.0.49/langflow/field_typing/__init__.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/field_typing/constants.py` & `langflow_base-0.0.49/langflow/field_typing/constants.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/field_typing/range_spec.py` & `langflow_base-0.0.49/langflow/field_typing/range_spec.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/accessibility-7deeca04.js` & `langflow_base-0.0.49/langflow/frontend/assets/accessibility-7deeca04.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/air-vent-f05f65f0.js` & `langflow_base-0.0.49/langflow/frontend/assets/air-vent-f05f65f0.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/alarm-clock-b53682c1.js` & `langflow_base-0.0.49/langflow/frontend/assets/alarm-clock-b53682c1.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/alarm-clock-check-d3b32670.js` & `langflow_base-0.0.49/langflow/frontend/assets/alarm-clock-check-d3b32670.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/alarm-clock-minus-fc96df2e.js` & `langflow_base-0.0.49/langflow/frontend/assets/alarm-clock-minus-fc96df2e.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/alarm-clock-off-6a0418e2.js` & `langflow_base-0.0.49/langflow/frontend/assets/alarm-clock-off-6a0418e2.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/alarm-clock-plus-bfb4a090.js` & `langflow_base-0.0.49/langflow/frontend/assets/alarm-clock-plus-bfb4a090.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/alarm-smoke-f5027e9e.js` & `langflow_base-0.0.49/langflow/frontend/assets/alarm-smoke-f5027e9e.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/align-center-horizontal-e3305b6c.js` & `langflow_base-0.0.49/langflow/frontend/assets/align-center-horizontal-e3305b6c.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/align-center-vertical-6fd65fe5.js` & `langflow_base-0.0.49/langflow/frontend/assets/align-center-vertical-6fd65fe5.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/align-horizontal-distribute-center-6966cea5.js` & `langflow_base-0.0.49/langflow/frontend/assets/align-horizontal-distribute-center-6966cea5.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/align-vertical-distribute-center-e4878d08.js` & `langflow_base-0.0.49/langflow/frontend/assets/align-vertical-distribute-center-e4878d08.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/ambulance-b3609100.js` & `langflow_base-0.0.49/langflow/frontend/assets/ambulance-b3609100.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/aperture-ae888f7c.js` & `langflow_base-0.0.49/langflow/frontend/assets/aperture-ae888f7c.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/archive-restore-34113244.js` & `langflow_base-0.0.49/langflow/frontend/assets/archive-restore-34113244.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/atom-634b4c72.js` & `langflow_base-0.0.49/langflow/frontend/assets/atom-634b4c72.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/baby-804d807f.js` & `langflow_base-0.0.49/langflow/frontend/assets/baby-804d807f.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/backpack-6bb8f8dc.js` & `langflow_base-0.0.49/langflow/frontend/assets/backpack-6bb8f8dc.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/badge-alert-2792746a.js` & `langflow_base-0.0.49/langflow/frontend/assets/badge-alert-2792746a.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/badge-cent-9c74db33.js` & `langflow_base-0.0.49/langflow/frontend/assets/badge-cent-9c74db33.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/badge-dollar-sign-534ee5dd.js` & `langflow_base-0.0.49/langflow/frontend/assets/badge-dollar-sign-534ee5dd.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/badge-euro-e86cd8b5.js` & `langflow_base-0.0.49/langflow/frontend/assets/badge-euro-e86cd8b5.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/badge-help-a99e4c15.js` & `langflow_base-0.0.49/langflow/frontend/assets/badge-help-a99e4c15.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/badge-indian-rupee-b932ef23.js` & `langflow_base-0.0.49/langflow/frontend/assets/badge-indian-rupee-b932ef23.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/badge-info-38c2f4b4.js` & `langflow_base-0.0.49/langflow/frontend/assets/badge-info-38c2f4b4.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/badge-japanese-yen-f7736118.js` & `langflow_base-0.0.49/langflow/frontend/assets/badge-japanese-yen-f7736118.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/badge-percent-96abe075.js` & `langflow_base-0.0.49/langflow/frontend/assets/badge-percent-96abe075.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/badge-plus-ef608fba.js` & `langflow_base-0.0.49/langflow/frontend/assets/badge-plus-ef608fba.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/badge-pound-sterling-5e65ad38.js` & `langflow_base-0.0.49/langflow/frontend/assets/badge-pound-sterling-5e65ad38.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/badge-russian-ruble-b25d9ad9.js` & `langflow_base-0.0.49/langflow/frontend/assets/badge-russian-ruble-b25d9ad9.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/badge-swiss-franc-3060d493.js` & `langflow_base-0.0.49/langflow/frontend/assets/badge-swiss-franc-3060d493.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/badge-x-0845dea8.js` & `langflow_base-0.0.49/langflow/frontend/assets/badge-x-0845dea8.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/baggage-claim-4b4424f5.js` & `langflow_base-0.0.49/langflow/frontend/assets/baggage-claim-4b4424f5.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/bath-52eb7e8c.js` & `langflow_base-0.0.49/langflow/frontend/assets/bath-52eb7e8c.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/battery-full-67d8a9b3.js` & `langflow_base-0.0.49/langflow/frontend/assets/battery-full-67d8a9b3.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/battery-warning-62ab1682.js` & `langflow_base-0.0.49/langflow/frontend/assets/battery-warning-62ab1682.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/bean-off-7b09212a.js` & `langflow_base-0.0.49/langflow/frontend/assets/bean-off-7b09212a.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/beef-9bf4ee37.js` & `langflow_base-0.0.49/langflow/frontend/assets/beef-9bf4ee37.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/beer-41f73772.js` & `langflow_base-0.0.49/langflow/frontend/assets/beer-41f73772.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/bell-electric-5dc74521.js` & `langflow_base-0.0.49/langflow/frontend/assets/bell-electric-5dc74521.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/biohazard-7f870d29.js` & `langflow_base-0.0.49/langflow/frontend/assets/biohazard-7f870d29.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/bird-ad099b8b.js` & `langflow_base-0.0.49/langflow/frontend/assets/bird-ad099b8b.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/blinds-9d36e4b5.js` & `langflow_base-0.0.49/langflow/frontend/assets/blinds-9d36e4b5.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/book-dashed-86cbe767.js` & `langflow_base-0.0.49/langflow/frontend/assets/book-dashed-86cbe767.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/book-heart-8beae983.js` & `langflow_base-0.0.49/langflow/frontend/assets/book-heart-8beae983.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/book-open-text-0c4694bc.js` & `langflow_base-0.0.49/langflow/frontend/assets/book-open-text-0c4694bc.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/boom-box-4e291b8b.js` & `langflow_base-0.0.49/langflow/frontend/assets/boom-box-4e291b8b.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/box-select-b0ef4e91.js` & `langflow_base-0.0.49/langflow/frontend/assets/box-select-b0ef4e91.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/brain-cog-3d4bb4c6.js` & `langflow_base-0.0.49/langflow/frontend/assets/brain-cog-3d4bb4c6.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/brain-d34d8a4b.js` & `langflow_base-0.0.49/langflow/frontend/assets/brain-d34d8a4b.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/brick-wall-b5fb72e9.js` & `langflow_base-0.0.49/langflow/frontend/assets/brick-wall-b5fb72e9.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/bug-c0e4b5c7.js` & `langflow_base-0.0.49/langflow/frontend/assets/bug-c0e4b5c7.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/bug-off-221980ea.js` & `langflow_base-0.0.49/langflow/frontend/assets/bug-off-221980ea.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/bug-play-d73bf6fc.js` & `langflow_base-0.0.49/langflow/frontend/assets/bug-play-d73bf6fc.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/building-2-6f46c282.js` & `langflow_base-0.0.49/langflow/frontend/assets/building-2-6f46c282.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/building-af553e71.js` & `langflow_base-0.0.49/langflow/frontend/assets/building-af553e71.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/bus-5900cfa3.js` & `langflow_base-0.0.49/langflow/frontend/assets/bus-5900cfa3.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/bus-front-7dc8cedb.js` & `langflow_base-0.0.49/langflow/frontend/assets/bus-front-7dc8cedb.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/cable-a48206d9.js` & `langflow_base-0.0.49/langflow/frontend/assets/cable-a48206d9.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/cable-car-ec551b2e.js` & `langflow_base-0.0.49/langflow/frontend/assets/cable-car-ec551b2e.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/cake-edd21758.js` & `langflow_base-0.0.49/langflow/frontend/assets/cake-edd21758.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/calculator-9ba50681.js` & `langflow_base-0.0.49/langflow/frontend/assets/calculator-9ba50681.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/calendar-clock-ea51db8f.js` & `langflow_base-0.0.49/langflow/frontend/assets/calendar-clock-ea51db8f.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/calendar-days-ef7e5a38.js` & `langflow_base-0.0.49/langflow/frontend/assets/calendar-days-ef7e5a38.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/calendar-fold-1da81079.js` & `langflow_base-0.0.49/langflow/frontend/assets/calendar-fold-1da81079.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/calendar-heart-5677e0b9.js` & `langflow_base-0.0.49/langflow/frontend/assets/calendar-heart-5677e0b9.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/calendar-off-0bd1e591.js` & `langflow_base-0.0.49/langflow/frontend/assets/calendar-off-0bd1e591.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/calendar-plus-73dc0684.js` & `langflow_base-0.0.49/langflow/frontend/assets/calendar-plus-73dc0684.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/calendar-range-83746210.js` & `langflow_base-0.0.49/langflow/frontend/assets/calendar-range-83746210.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/calendar-search-02e8602b.js` & `langflow_base-0.0.49/langflow/frontend/assets/calendar-search-02e8602b.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/calendar-x-2-b568f6b9.js` & `langflow_base-0.0.49/langflow/frontend/assets/calendar-x-2-b568f6b9.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/candlestick-chart-1765be54.js` & `langflow_base-0.0.49/langflow/frontend/assets/candlestick-chart-1765be54.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/candy-7dd2ee96.js` & `langflow_base-0.0.49/langflow/frontend/assets/candy-7dd2ee96.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/candy-cane-0be5742f.js` & `langflow_base-0.0.49/langflow/frontend/assets/candy-cane-0be5742f.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/candy-off-523922e8.js` & `langflow_base-0.0.49/langflow/frontend/assets/candy-off-523922e8.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/captions-off-2f69fa80.js` & `langflow_base-0.0.49/langflow/frontend/assets/captions-off-2f69fa80.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/car-d4fab838.js` & `langflow_base-0.0.49/langflow/frontend/assets/car-d4fab838.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/car-front-a8753e88.js` & `langflow_base-0.0.49/langflow/frontend/assets/car-front-a8753e88.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/car-taxi-front-7222b3f3.js` & `langflow_base-0.0.49/langflow/frontend/assets/car-taxi-front-7222b3f3.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/caravan-7e780ccf.js` & `langflow_base-0.0.49/langflow/frontend/assets/caravan-7e780ccf.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/carrot-1da699eb.js` & `langflow_base-0.0.49/langflow/frontend/assets/carrot-1da699eb.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/cassette-tape-11ee7a3e.js` & `langflow_base-0.0.49/langflow/frontend/assets/cassette-tape-11ee7a3e.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/castle-aa353636.js` & `langflow_base-0.0.49/langflow/frontend/assets/castle-aa353636.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/cat-b10af0e4.js` & `langflow_base-0.0.49/langflow/frontend/assets/cat-b10af0e4.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/cctv-c9b74e6f.js` & `langflow_base-0.0.49/langflow/frontend/assets/cctv-c9b74e6f.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/cherry-ec8c07da.js` & `langflow_base-0.0.49/langflow/frontend/assets/cherry-ec8c07da.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/chrome-214e9f29.js` & `langflow_base-0.0.49/langflow/frontend/assets/chrome-214e9f29.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/church-82bb793c.js` & `langflow_base-0.0.49/langflow/frontend/assets/church-82bb793c.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/cigarette-off-6e801ae2.js` & `langflow_base-0.0.49/langflow/frontend/assets/cigarette-off-6e801ae2.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/circle-dashed-ceb50c6a.js` & `langflow_base-0.0.49/langflow/frontend/assets/circle-dashed-ceb50c6a.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/circle-dot-dashed-0eb51089.js` & `langflow_base-0.0.49/langflow/frontend/assets/circle-dot-dashed-0eb51089.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/circle-fading-plus-f5dbfc16.js` & `langflow_base-0.0.49/langflow/frontend/assets/circle-fading-plus-f5dbfc16.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/circuit-board-7cd682a8.js` & `langflow_base-0.0.49/langflow/frontend/assets/circuit-board-7cd682a8.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/citrus-f0326961.js` & `langflow_base-0.0.49/langflow/frontend/assets/citrus-f0326961.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/clapperboard-b8e90a42.js` & `langflow_base-0.0.49/langflow/frontend/assets/clapperboard-b8e90a42.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/clipboard-copy-61b23095.js` & `langflow_base-0.0.49/langflow/frontend/assets/clipboard-copy-61b23095.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/clipboard-list-5426b358.js` & `langflow_base-0.0.49/langflow/frontend/assets/clipboard-list-5426b358.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/clipboard-paste-ee5d0d42.js` & `langflow_base-0.0.49/langflow/frontend/assets/clipboard-paste-ee5d0d42.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/clipboard-pen-7403e404.js` & `langflow_base-0.0.49/langflow/frontend/assets/clipboard-pen-7403e404.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/clipboard-pen-line-21803d72.js` & `langflow_base-0.0.49/langflow/frontend/assets/clipboard-pen-line-21803d72.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/clipboard-type-f743f70a.js` & `langflow_base-0.0.49/langflow/frontend/assets/clipboard-type-f743f70a.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/cloud-cog-d9e48864.js` & `langflow_base-0.0.49/langflow/frontend/assets/cloud-cog-d9e48864.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/cloud-drizzle-e9ee8e3d.js` & `langflow_base-0.0.49/langflow/frontend/assets/cloud-drizzle-e9ee8e3d.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/cloud-hail-551a6ea9.js` & `langflow_base-0.0.49/langflow/frontend/assets/cloud-hail-551a6ea9.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/cloud-moon-rain-381e8468.js` & `langflow_base-0.0.49/langflow/frontend/assets/cloud-moon-rain-381e8468.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/cloud-snow-ad1d7740.js` & `langflow_base-0.0.49/langflow/frontend/assets/cloud-snow-ad1d7740.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/cloud-sun-630cbe71.js` & `langflow_base-0.0.49/langflow/frontend/assets/cloud-sun-630cbe71.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/cloud-sun-rain-5249c398.js` & `langflow_base-0.0.49/langflow/frontend/assets/cloud-sun-rain-5249c398.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/clover-77915ed9.js` & `langflow_base-0.0.49/langflow/frontend/assets/clover-77915ed9.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/codepen-b2e8542d.js` & `langflow_base-0.0.49/langflow/frontend/assets/codepen-b2e8542d.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/codesandbox-7efd711a.js` & `langflow_base-0.0.49/langflow/frontend/assets/codesandbox-7efd711a.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/coffee-05730958.js` & `langflow_base-0.0.49/langflow/frontend/assets/coffee-05730958.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/cog-25bd7786.js` & `langflow_base-0.0.49/langflow/frontend/assets/cog-25bd7786.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/component-a81ab53e.js` & `langflow_base-0.0.49/langflow/frontend/assets/component-a81ab53e.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/construction-fe67f2d9.js` & `langflow_base-0.0.49/langflow/frontend/assets/construction-fe67f2d9.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/contact-2-c389498e.js` & `langflow_base-0.0.49/langflow/frontend/assets/contact-2-c389498e.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/contact-b9c1f247.js` & `langflow_base-0.0.49/langflow/frontend/assets/contact-b9c1f247.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/container-8047bd33.js` & `langflow_base-0.0.49/langflow/frontend/assets/container-8047bd33.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/cookie-5ac97459.js` & `langflow_base-0.0.49/langflow/frontend/assets/cookie-5ac97459.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/copy-plus-cfb7c23a.js` & `langflow_base-0.0.49/langflow/frontend/assets/copy-plus-cfb7c23a.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/copy-x-4bc29fe8.js` & `langflow_base-0.0.49/langflow/frontend/assets/copy-x-4bc29fe8.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/croissant-cf14f255.js` & `langflow_base-0.0.49/langflow/frontend/assets/croissant-cf14f255.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/crosshair-797727d3.js` & `langflow_base-0.0.49/langflow/frontend/assets/crosshair-797727d3.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/cuboid-e2b6b17f.js` & `langflow_base-0.0.49/langflow/frontend/assets/cuboid-e2b6b17f.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/currency-2f95ffaa.js` & `langflow_base-0.0.49/langflow/frontend/assets/currency-2f95ffaa.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/database-backup-7e289bb9.js` & `langflow_base-0.0.49/langflow/frontend/assets/database-backup-7e289bb9.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/database-zap-b120cb34.js` & `langflow_base-0.0.49/langflow/frontend/assets/database-zap-b120cb34.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/dessert-0e61f7af.js` & `langflow_base-0.0.49/langflow/frontend/assets/dessert-0e61f7af.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/diameter-29b4aa9b.js` & `langflow_base-0.0.49/langflow/frontend/assets/diameter-29b4aa9b.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/dice-5-1fa08684.js` & `langflow_base-0.0.49/langflow/frontend/assets/dice-5-1fa08684.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/dice-6-40a50ff1.js` & `langflow_base-0.0.49/langflow/frontend/assets/dice-6-40a50ff1.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/dices-13083691.js` & `langflow_base-0.0.49/langflow/frontend/assets/dices-13083691.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/dna-6fa418fc.js` & `langflow_base-0.0.49/langflow/frontend/assets/dna-6fa418fc.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/dna-off-a86c6e71.js` & `langflow_base-0.0.49/langflow/frontend/assets/dna-off-a86c6e71.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/dog-0ed15e9a.js` & `langflow_base-0.0.49/langflow/frontend/assets/dog-0ed15e9a.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/door-open-caf41777.js` & `langflow_base-0.0.49/langflow/frontend/assets/door-open-caf41777.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/drama-2aa25a7f.js` & `langflow_base-0.0.49/langflow/frontend/assets/drama-2aa25a7f.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/drill-3ab18849.js` & `langflow_base-0.0.49/langflow/frontend/assets/drill-3ab18849.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/droplets-a565eb54.js` & `langflow_base-0.0.49/langflow/frontend/assets/droplets-a565eb54.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/drum-0881aa6e.js` & `langflow_base-0.0.49/langflow/frontend/assets/drum-0881aa6e.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/drumstick-42cc5c3b.js` & `langflow_base-0.0.49/langflow/frontend/assets/drumstick-42cc5c3b.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/dumbbell-d91d8011.js` & `langflow_base-0.0.49/langflow/frontend/assets/dumbbell-d91d8011.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/ear-off-ca41fa4a.js` & `langflow_base-0.0.49/langflow/frontend/assets/ear-off-ca41fa4a.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/egg-off-15482582.js` & `langflow_base-0.0.49/langflow/frontend/assets/egg-off-15482582.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/fence-ee593734.js` & `langflow_base-0.0.49/langflow/frontend/assets/fence-ee593734.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/ferris-wheel-38cf8098.js` & `langflow_base-0.0.49/langflow/frontend/assets/ferris-wheel-38cf8098.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/figma-7ce64fda.js` & `langflow_base-0.0.49/langflow/frontend/assets/figma-7ce64fda.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/file-archive-16a981ce.js` & `langflow_base-0.0.49/langflow/frontend/assets/file-archive-16a981ce.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/file-audio-2-eba1bafe.js` & `langflow_base-0.0.49/langflow/frontend/assets/file-audio-2-eba1bafe.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/file-bar-chart-2-df4f1ba6.js` & `langflow_base-0.0.49/langflow/frontend/assets/file-bar-chart-2-df4f1ba6.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/file-bar-chart-7528c81d.js` & `langflow_base-0.0.49/langflow/frontend/assets/file-bar-chart-7528c81d.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/file-box-ade74692.js` & `langflow_base-0.0.49/langflow/frontend/assets/file-box-ade74692.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/file-cog-92ab8d32.js` & `langflow_base-0.0.49/langflow/frontend/assets/file-cog-92ab8d32.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/file-digit-d190a761.js` & `langflow_base-0.0.49/langflow/frontend/assets/file-digit-d190a761.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/file-heart-0e4c6049.js` & `langflow_base-0.0.49/langflow/frontend/assets/file-heart-0e4c6049.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/file-image-ce046320.js` & `langflow_base-0.0.49/langflow/frontend/assets/file-image-ce046320.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/file-json-2-e5f3b51f.js` & `langflow_base-0.0.49/langflow/frontend/assets/file-json-2-e5f3b51f.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/file-json-bdae09ef.js` & `langflow_base-0.0.49/langflow/frontend/assets/file-json-bdae09ef.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/file-key-2-b0bc49ac.js` & `langflow_base-0.0.49/langflow/frontend/assets/file-key-2-b0bc49ac.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/file-output-ec885816.js` & `langflow_base-0.0.49/langflow/frontend/assets/file-output-ec885816.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/file-scan-6d6f6d71.js` & `langflow_base-0.0.49/langflow/frontend/assets/file-scan-6d6f6d71.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/file-spreadsheet-43a79f96.js` & `langflow_base-0.0.49/langflow/frontend/assets/file-spreadsheet-43a79f96.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/file-stack-e4b74c5a.js` & `langflow_base-0.0.49/langflow/frontend/assets/file-stack-e4b74c5a.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/file-type-c9cab45d.js` & `langflow_base-0.0.49/langflow/frontend/assets/file-type-c9cab45d.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/file-volume-2-c5616849.js` & `langflow_base-0.0.49/langflow/frontend/assets/file-volume-2-c5616849.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/film-d24eb5d6.js` & `langflow_base-0.0.49/langflow/frontend/assets/film-d24eb5d6.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/fingerprint-d9b62aff.js` & `langflow_base-0.0.49/langflow/frontend/assets/fingerprint-d9b62aff.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/fire-extinguisher-5bccd8e3.js` & `langflow_base-0.0.49/langflow/frontend/assets/fire-extinguisher-5bccd8e3.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/fish-f12e8325.js` & `langflow_base-0.0.49/langflow/frontend/assets/fish-f12e8325.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/fish-off-a19b2443.js` & `langflow_base-0.0.49/langflow/frontend/assets/fish-off-a19b2443.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/flask-conical-off-e88dcc6f.js` & `langflow_base-0.0.49/langflow/frontend/assets/flask-conical-off-e88dcc6f.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/flip-horizontal-40d9ef22.js` & `langflow_base-0.0.49/langflow/frontend/assets/flip-horizontal-40d9ef22.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/flip-vertical-57017fb6.js` & `langflow_base-0.0.49/langflow/frontend/assets/flip-vertical-57017fb6.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/flower-2-b71a7369.js` & `langflow_base-0.0.49/langflow/frontend/assets/flower-2-b71a7369.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/flower-7e27e620.js` & `langflow_base-0.0.49/langflow/frontend/assets/flower-7e27e620.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/focus-119a2d2c.js` & `langflow_base-0.0.49/langflow/frontend/assets/focus-119a2d2c.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/fold-horizontal-e86e541d.js` & `langflow_base-0.0.49/langflow/frontend/assets/fold-horizontal-e86e541d.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/fold-vertical-b2f86633.js` & `langflow_base-0.0.49/langflow/frontend/assets/fold-vertical-b2f86633.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/folder-archive-0867c658.js` & `langflow_base-0.0.49/langflow/frontend/assets/folder-archive-0867c658.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/folder-cog-147353aa.js` & `langflow_base-0.0.49/langflow/frontend/assets/folder-cog-147353aa.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/folder-git-2-179844c9.js` & `langflow_base-0.0.49/langflow/frontend/assets/folder-git-2-179844c9.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/folder-git-c020630f.js` & `langflow_base-0.0.49/langflow/frontend/assets/folder-git-c020630f.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/folder-heart-9f9ea4b3.js` & `langflow_base-0.0.49/langflow/frontend/assets/folder-heart-9f9ea4b3.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/folder-kanban-a3dfd68e.js` & `langflow_base-0.0.49/langflow/frontend/assets/folder-kanban-a3dfd68e.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/folder-key-c4cc0892.js` & `langflow_base-0.0.49/langflow/frontend/assets/folder-key-c4cc0892.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/folder-lock-9187bd0c.js` & `langflow_base-0.0.49/langflow/frontend/assets/folder-lock-9187bd0c.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/folder-open-dot-bd887495.js` & `langflow_base-0.0.49/langflow/frontend/assets/folder-open-dot-bd887495.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/folder-sync-b7d69c14.js` & `langflow_base-0.0.49/langflow/frontend/assets/folder-sync-b7d69c14.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/folder-tree-16c062ce.js` & `langflow_base-0.0.49/langflow/frontend/assets/folder-tree-16c062ce.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/footprints-64b0ead1.js` & `langflow_base-0.0.49/langflow/frontend/assets/footprints-64b0ead1.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/fuel-f21d2bfd.js` & `langflow_base-0.0.49/langflow/frontend/assets/fuel-f21d2bfd.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/fullscreen-7d7817b8.js` & `langflow_base-0.0.49/langflow/frontend/assets/fullscreen-7d7817b8.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/gamepad-2-3ae0b330.js` & `langflow_base-0.0.49/langflow/frontend/assets/gamepad-2-3ae0b330.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/gamepad-23b3ad90.js` & `langflow_base-0.0.49/langflow/frontend/assets/gamepad-23b3ad90.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/git-compare-arrows-81eff26e.js` & `langflow_base-0.0.49/langflow/frontend/assets/git-compare-arrows-81eff26e.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/git-graph-7ba52a21.js` & `langflow_base-0.0.49/langflow/frontend/assets/git-graph-7ba52a21.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/git-pull-request-closed-a14928c4.js` & `langflow_base-0.0.49/langflow/frontend/assets/git-pull-request-closed-a14928c4.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/git-pull-request-create-arrow-08b3e525.js` & `langflow_base-0.0.49/langflow/frontend/assets/git-pull-request-create-arrow-08b3e525.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/gitlab-1d3a66c3.js` & `langflow_base-0.0.49/langflow/frontend/assets/gitlab-1d3a66c3.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/glasses-7fe19bf9.js` & `langflow_base-0.0.49/langflow/frontend/assets/glasses-7fe19bf9.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/globe-2-47d02662.js` & `langflow_base-0.0.49/langflow/frontend/assets/globe-2-47d02662.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/grab-70e64ba1.js` & `langflow_base-0.0.49/langflow/frontend/assets/grab-70e64ba1.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/grape-332f120a.js` & `langflow_base-0.0.49/langflow/frontend/assets/grape-332f120a.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/grip-c338a35d.js` & `langflow_base-0.0.49/langflow/frontend/assets/grip-c338a35d.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/grip-horizontal-c47cb1ba.js` & `langflow_base-0.0.49/langflow/frontend/assets/grip-horizontal-c47cb1ba.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/grip-vertical-da29db8f.js` & `langflow_base-0.0.49/langflow/frontend/assets/grip-vertical-da29db8f.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/guitar-2d10606f.js` & `langflow_base-0.0.49/langflow/frontend/assets/guitar-2d10606f.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/hand-coins-7d87aee4.js` & `langflow_base-0.0.49/langflow/frontend/assets/hand-coins-7d87aee4.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/hand-d08db668.js` & `langflow_base-0.0.49/langflow/frontend/assets/hand-d08db668.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/hand-heart-f341c0c6.js` & `langflow_base-0.0.49/langflow/frontend/assets/hand-heart-f341c0c6.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/hand-metal-4c03951f.js` & `langflow_base-0.0.49/langflow/frontend/assets/hand-metal-4c03951f.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/hand-platter-bda84c9f.js` & `langflow_base-0.0.49/langflow/frontend/assets/hand-platter-bda84c9f.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/handshake-a314c225.js` & `langflow_base-0.0.49/langflow/frontend/assets/handshake-a314c225.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/hard-drive-2d00eab4.js` & `langflow_base-0.0.49/langflow/frontend/assets/hard-drive-2d00eab4.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/hard-hat-4e174197.js` & `langflow_base-0.0.49/langflow/frontend/assets/hard-hat-4e174197.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/haze-b45745fb.js` & `langflow_base-0.0.49/langflow/frontend/assets/haze-b45745fb.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/heart-handshake-bcbba2ba.js` & `langflow_base-0.0.49/langflow/frontend/assets/heart-handshake-bcbba2ba.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/heart-off-43722eb5.js` & `langflow_base-0.0.49/langflow/frontend/assets/heart-off-43722eb5.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/heater-af5de4da.js` & `langflow_base-0.0.49/langflow/frontend/assets/heater-af5de4da.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/hop-d889a2a4.js` & `langflow_base-0.0.49/langflow/frontend/assets/hop-d889a2a4.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/hop-off-53ebd056.js` & `langflow_base-0.0.49/langflow/frontend/assets/hop-off-53ebd056.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/hotel-397a190d.js` & `langflow_base-0.0.49/langflow/frontend/assets/hotel-397a190d.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/hourglass-d50bf166.js` & `langflow_base-0.0.49/langflow/frontend/assets/hourglass-d50bf166.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/image-down-f9f50798.js` & `langflow_base-0.0.49/langflow/frontend/assets/image-down-f9f50798.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/image-minus-a2c5accd.js` & `langflow_base-0.0.49/langflow/frontend/assets/image-minus-a2c5accd.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/image-off-67dff800.js` & `langflow_base-0.0.49/langflow/frontend/assets/image-off-67dff800.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/image-plus-81549658.js` & `langflow_base-0.0.49/langflow/frontend/assets/image-plus-81549658.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/index-5d2e85d2.js` & `langflow_base-0.0.49/langflow/frontend/assets/index-5d2e85d2.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/index-b5c02d80.css` & `langflow_base-0.0.49/langflow/frontend/assets/index-b5c02d80.css`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/kanban-square-dashed-011cd9c5.js` & `langflow_base-0.0.49/langflow/frontend/assets/kanban-square-dashed-011cd9c5.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/key-square-7b7c4744.js` & `langflow_base-0.0.49/langflow/frontend/assets/key-square-7b7c4744.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/keyboard-music-216e0129.js` & `langflow_base-0.0.49/langflow/frontend/assets/keyboard-music-216e0129.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/land-plot-fbcf7d50.js` & `langflow_base-0.0.49/langflow/frontend/assets/land-plot-fbcf7d50.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/landmark-c8fd19f9.js` & `langflow_base-0.0.49/langflow/frontend/assets/landmark-c8fd19f9.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/lasso-select-e5441e2c.js` & `langflow_base-0.0.49/langflow/frontend/assets/lasso-select-e5441e2c.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/layers-3-fa210f21.js` & `langflow_base-0.0.49/langflow/frontend/assets/layers-3-fa210f21.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/layout-dashboard-20091918.js` & `langflow_base-0.0.49/langflow/frontend/assets/layout-dashboard-20091918.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/layout-grid-a5dbe99b.js` & `langflow_base-0.0.49/langflow/frontend/assets/layout-grid-a5dbe99b.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/layout-list-281c03bd.js` & `langflow_base-0.0.49/langflow/frontend/assets/layout-list-281c03bd.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/leafy-green-12a9e7f1.js` & `langflow_base-0.0.49/langflow/frontend/assets/leafy-green-12a9e7f1.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/life-buoy-9b302c13.js` & `langflow_base-0.0.49/langflow/frontend/assets/life-buoy-9b302c13.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/lightbulb-off-a9572065.js` & `langflow_base-0.0.49/langflow/frontend/assets/lightbulb-off-a9572065.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/list-6c4583fe.js` & `langflow_base-0.0.49/langflow/frontend/assets/list-6c4583fe.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/list-ordered-f67a586a.js` & `langflow_base-0.0.49/langflow/frontend/assets/list-ordered-f67a586a.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/loader-6788a7f7.js` & `langflow_base-0.0.49/langflow/frontend/assets/loader-6788a7f7.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/locate-7eee1a99.js` & `langflow_base-0.0.49/langflow/frontend/assets/locate-7eee1a99.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/locate-fixed-bc0164df.js` & `langflow_base-0.0.49/langflow/frontend/assets/locate-fixed-bc0164df.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/locate-off-6d1017b1.js` & `langflow_base-0.0.49/langflow/frontend/assets/locate-off-6d1017b1.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/luggage-5d91149b.js` & `langflow_base-0.0.49/langflow/frontend/assets/luggage-5d91149b.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/mail-question-3e638ddf.js` & `langflow_base-0.0.49/langflow/frontend/assets/mail-question-3e638ddf.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/mail-search-69d0fb92.js` & `langflow_base-0.0.49/langflow/frontend/assets/mail-search-69d0fb92.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/mailbox-476dc431.js` & `langflow_base-0.0.49/langflow/frontend/assets/mailbox-476dc431.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/male-technologist-d2e7de57.png` & `langflow_base-0.0.49/langflow/frontend/assets/male-technologist-d2e7de57.png`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/map-pin-off-f46c49f4.js` & `langflow_base-0.0.49/langflow/frontend/assets/map-pin-off-f46c49f4.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/map-pinned-b0ef6f9d.js` & `langflow_base-0.0.49/langflow/frontend/assets/map-pinned-b0ef6f9d.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/medal-ae183bc6.js` & `langflow_base-0.0.49/langflow/frontend/assets/medal-ae183bc6.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/memory-stick-a95af896.js` & `langflow_base-0.0.49/langflow/frontend/assets/memory-stick-a95af896.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/message-circle-dashed-c3eb173d.js` & `langflow_base-0.0.49/langflow/frontend/assets/message-circle-dashed-c3eb173d.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/message-square-dashed-63e862cd.js` & `langflow_base-0.0.49/langflow/frontend/assets/message-square-dashed-63e862cd.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/mic-off-c97851d9.js` & `langflow_base-0.0.49/langflow/frontend/assets/mic-off-c97851d9.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/microscope-4c5e2ae8.js` & `langflow_base-0.0.49/langflow/frontend/assets/microscope-4c5e2ae8.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/milk-17837e5c.js` & `langflow_base-0.0.49/langflow/frontend/assets/milk-17837e5c.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/milk-off-c72c2c04.js` & `langflow_base-0.0.49/langflow/frontend/assets/milk-off-c72c2c04.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/monitor-speaker-fbdd7793.js` & `langflow_base-0.0.49/langflow/frontend/assets/monitor-speaker-fbdd7793.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/mouse-pointer-square-dashed-2d247999.js` & `langflow_base-0.0.49/langflow/frontend/assets/mouse-pointer-square-dashed-2d247999.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/move-300bf01c.js` & `langflow_base-0.0.49/langflow/frontend/assets/move-300bf01c.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/newspaper-c5cbe283.js` & `langflow_base-0.0.49/langflow/frontend/assets/newspaper-c5cbe283.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/notebook-pen-2cb4fcf8.js` & `langflow_base-0.0.49/langflow/frontend/assets/notebook-pen-2cb4fcf8.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/notebook-tabs-57108f6c.js` & `langflow_base-0.0.49/langflow/frontend/assets/notebook-tabs-57108f6c.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/notebook-text-90d14136.js` & `langflow_base-0.0.49/langflow/frontend/assets/notebook-text-90d14136.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/notepad-text-a6008a7b.js` & `langflow_base-0.0.49/langflow/frontend/assets/notepad-text-a6008a7b.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/notepad-text-dashed-c8d9e1e3.js` & `langflow_base-0.0.49/langflow/frontend/assets/notepad-text-dashed-c8d9e1e3.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/nut-302b4fc7.js` & `langflow_base-0.0.49/langflow/frontend/assets/nut-302b4fc7.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/nut-off-416c230b.js` & `langflow_base-0.0.49/langflow/frontend/assets/nut-off-416c230b.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/orbit-73963e9d.js` & `langflow_base-0.0.49/langflow/frontend/assets/orbit-73963e9d.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/package-5282c64c.js` & `langflow_base-0.0.49/langflow/frontend/assets/package-5282c64c.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/package-check-f94596d2.js` & `langflow_base-0.0.49/langflow/frontend/assets/package-check-f94596d2.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/package-minus-87f97424.js` & `langflow_base-0.0.49/langflow/frontend/assets/package-minus-87f97424.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/package-open-50313ee6.js` & `langflow_base-0.0.49/langflow/frontend/assets/package-open-50313ee6.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/package-plus-4ec37a35.js` & `langflow_base-0.0.49/langflow/frontend/assets/package-plus-4ec37a35.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/package-search-1587ffd9.js` & `langflow_base-0.0.49/langflow/frontend/assets/package-search-1587ffd9.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/package-x-d81f8c09.js` & `langflow_base-0.0.49/langflow/frontend/assets/package-x-d81f8c09.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/paint-bucket-93cba5af.js` & `langflow_base-0.0.49/langflow/frontend/assets/paint-bucket-93cba5af.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/paintbrush-c5238598.js` & `langflow_base-0.0.49/langflow/frontend/assets/paintbrush-c5238598.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/palmtree-7355f6bb.js` & `langflow_base-0.0.49/langflow/frontend/assets/palmtree-7355f6bb.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/parking-meter-c3c52a07.js` & `langflow_base-0.0.49/langflow/frontend/assets/parking-meter-c3c52a07.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/parking-square-off-740bd731.js` & `langflow_base-0.0.49/langflow/frontend/assets/parking-square-off-740bd731.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/party-popper-7f352c5a.js` & `langflow_base-0.0.49/langflow/frontend/assets/party-popper-7f352c5a.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/paw-print-0e3aa68a.js` & `langflow_base-0.0.49/langflow/frontend/assets/paw-print-0e3aa68a.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/pencil-ruler-c7daf67c.js` & `langflow_base-0.0.49/langflow/frontend/assets/pencil-ruler-c7daf67c.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/percent-diamond-a221c97d.js` & `langflow_base-0.0.49/langflow/frontend/assets/percent-diamond-a221c97d.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/phone-bb7af3a3.js` & `langflow_base-0.0.49/langflow/frontend/assets/phone-bb7af3a3.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/phone-call-a324d52a.js` & `langflow_base-0.0.49/langflow/frontend/assets/phone-call-a324d52a.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/phone-forwarded-7416bc2f.js` & `langflow_base-0.0.49/langflow/frontend/assets/phone-forwarded-7416bc2f.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/phone-incoming-45414c5f.js` & `langflow_base-0.0.49/langflow/frontend/assets/phone-incoming-45414c5f.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/phone-missed-46ce970c.js` & `langflow_base-0.0.49/langflow/frontend/assets/phone-missed-46ce970c.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/phone-off-ef820972.js` & `langflow_base-0.0.49/langflow/frontend/assets/phone-off-ef820972.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/phone-outgoing-eb5faee5.js` & `langflow_base-0.0.49/langflow/frontend/assets/phone-outgoing-eb5faee5.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/piano-3e58cbd0.js` & `langflow_base-0.0.49/langflow/frontend/assets/piano-3e58cbd0.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/pin-off-7ff30ecb.js` & `langflow_base-0.0.49/langflow/frontend/assets/pin-off-7ff30ecb.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/plane-landing-91d10c06.js` & `langflow_base-0.0.49/langflow/frontend/assets/plane-landing-91d10c06.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/plane-takeoff-e3daa27f.js` & `langflow_base-0.0.49/langflow/frontend/assets/plane-takeoff-e3daa27f.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/plug-zap-d1efc20e.js` & `langflow_base-0.0.49/langflow/frontend/assets/plug-zap-d1efc20e.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/pointer-6a99de81.js` & `langflow_base-0.0.49/langflow/frontend/assets/pointer-6a99de81.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/pointer-off-9f315d62.js` & `langflow_base-0.0.49/langflow/frontend/assets/pointer-off-9f315d62.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/popcorn-e646c986.js` & `langflow_base-0.0.49/langflow/frontend/assets/popcorn-e646c986.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/projector-ea7a2ed4.js` & `langflow_base-0.0.49/langflow/frontend/assets/projector-ea7a2ed4.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/puzzle-e8df0c53.js` & `langflow_base-0.0.49/langflow/frontend/assets/puzzle-e8df0c53.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/qr-code-92db79b5.js` & `langflow_base-0.0.49/langflow/frontend/assets/qr-code-92db79b5.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/quote-ebbe955b.js` & `langflow_base-0.0.49/langflow/frontend/assets/quote-ebbe955b.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/rabbit-ea3ddd8c.js` & `langflow_base-0.0.49/langflow/frontend/assets/rabbit-ea3ddd8c.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/radar-74ff71f7.js` & `langflow_base-0.0.49/langflow/frontend/assets/radar-74ff71f7.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/radiation-28ac3311.js` & `langflow_base-0.0.49/langflow/frontend/assets/radiation-28ac3311.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/radio-e0db86d7.js` & `langflow_base-0.0.49/langflow/frontend/assets/radio-e0db86d7.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/radio-tower-4dcbd4de.js` & `langflow_base-0.0.49/langflow/frontend/assets/radio-tower-4dcbd4de.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/rat-59bc794f.js` & `langflow_base-0.0.49/langflow/frontend/assets/rat-59bc794f.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/receipt-japanese-yen-27196c83.js` & `langflow_base-0.0.49/langflow/frontend/assets/receipt-japanese-yen-27196c83.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/recycle-cea96532.js` & `langflow_base-0.0.49/langflow/frontend/assets/recycle-cea96532.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/refresh-cw-off-26c765c7.js` & `langflow_base-0.0.49/langflow/frontend/assets/refresh-cw-off-26c765c7.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/replace-all-3afafbb1.js` & `langflow_base-0.0.49/langflow/frontend/assets/replace-all-3afafbb1.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/replace-f610ab8f.js` & `langflow_base-0.0.49/langflow/frontend/assets/replace-f610ab8f.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/ribbon-30f6b81f.js` & `langflow_base-0.0.49/langflow/frontend/assets/ribbon-30f6b81f.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/robot-95e1b00d.png` & `langflow_base-0.0.49/langflow/frontend/assets/robot-95e1b00d.png`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/rocket-dd64364a.js` & `langflow_base-0.0.49/langflow/frontend/assets/rocket-dd64364a.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/roller-coaster-07467718.js` & `langflow_base-0.0.49/langflow/frontend/assets/roller-coaster-07467718.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/rotate-3d-123855e5.js` & `langflow_base-0.0.49/langflow/frontend/assets/rotate-3d-123855e5.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/route-off-9b0cd50f.js` & `langflow_base-0.0.49/langflow/frontend/assets/route-off-9b0cd50f.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/router-7d73f15e.js` & `langflow_base-0.0.49/langflow/frontend/assets/router-7d73f15e.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/ruler-7f425ff8.js` & `langflow_base-0.0.49/langflow/frontend/assets/ruler-7f425ff8.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/salad-d5faeb52.js` & `langflow_base-0.0.49/langflow/frontend/assets/salad-d5faeb52.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/sandwich-6f29208b.js` & `langflow_base-0.0.49/langflow/frontend/assets/sandwich-6f29208b.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/scale-f896884c.js` & `langflow_base-0.0.49/langflow/frontend/assets/scale-f896884c.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/scan-barcode-566f4c1e.js` & `langflow_base-0.0.49/langflow/frontend/assets/scan-barcode-566f4c1e.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/scan-eye-2473d111.js` & `langflow_base-0.0.49/langflow/frontend/assets/scan-eye-2473d111.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/scan-face-6b16b2e0.js` & `langflow_base-0.0.49/langflow/frontend/assets/scan-face-6b16b2e0.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/scan-search-6abfbd41.js` & `langflow_base-0.0.49/langflow/frontend/assets/scan-search-6abfbd41.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/scan-text-ee620dce.js` & `langflow_base-0.0.49/langflow/frontend/assets/scan-text-ee620dce.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/scatter-chart-b0552128.js` & `langflow_base-0.0.49/langflow/frontend/assets/scatter-chart-b0552128.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/school-2-665376f7.js` & `langflow_base-0.0.49/langflow/frontend/assets/school-2-665376f7.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/school-3f78e0ab.js` & `langflow_base-0.0.49/langflow/frontend/assets/school-3f78e0ab.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/scissors-line-dashed-aad245e8.js` & `langflow_base-0.0.49/langflow/frontend/assets/scissors-line-dashed-aad245e8.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/scissors-square-75252291.js` & `langflow_base-0.0.49/langflow/frontend/assets/scissors-square-75252291.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/scissors-square-dashed-bottom-1c99d312.js` & `langflow_base-0.0.49/langflow/frontend/assets/scissors-square-dashed-bottom-1c99d312.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/server-22d39749.js` & `langflow_base-0.0.49/langflow/frontend/assets/server-22d39749.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/server-cog-4f664742.js` & `langflow_base-0.0.49/langflow/frontend/assets/server-cog-4f664742.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/server-crash-2de8d911.js` & `langflow_base-0.0.49/langflow/frontend/assets/server-crash-2de8d911.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/server-off-e5302d6b.js` & `langflow_base-0.0.49/langflow/frontend/assets/server-off-e5302d6b.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/settings-2c5eb85f.js` & `langflow_base-0.0.49/langflow/frontend/assets/settings-2c5eb85f.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/sheet-c18d33b2.js` & `langflow_base-0.0.49/langflow/frontend/assets/sheet-c18d33b2.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/ship-34376655.js` & `langflow_base-0.0.49/langflow/frontend/assets/ship-34376655.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/ship-wheel-5f798c44.js` & `langflow_base-0.0.49/langflow/frontend/assets/ship-wheel-5f798c44.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/shopping-basket-c496e3a3.js` & `langflow_base-0.0.49/langflow/frontend/assets/shopping-basket-c496e3a3.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/shower-head-9234f682.js` & `langflow_base-0.0.49/langflow/frontend/assets/shower-head-9234f682.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/shuffle-5a3cdb9d.js` & `langflow_base-0.0.49/langflow/frontend/assets/shuffle-5a3cdb9d.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/siren-594aae1f.js` & `langflow_base-0.0.49/langflow/frontend/assets/siren-594aae1f.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/skull-f042a7bf.js` & `langflow_base-0.0.49/langflow/frontend/assets/skull-f042a7bf.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/slack-422f1b25.js` & `langflow_base-0.0.49/langflow/frontend/assets/slack-422f1b25.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/smartphone-nfc-f363c1ef.js` & `langflow_base-0.0.49/langflow/frontend/assets/smartphone-nfc-f363c1ef.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/smile-plus-5f6ed569.js` & `langflow_base-0.0.49/langflow/frontend/assets/smile-plus-5f6ed569.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/snail-da9a7766.js` & `langflow_base-0.0.49/langflow/frontend/assets/snail-da9a7766.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/sofa-2bfdf61c.js` & `langflow_base-0.0.49/langflow/frontend/assets/sofa-2bfdf61c.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/soup-f6cf262a.js` & `langflow_base-0.0.49/langflow/frontend/assets/soup-f6cf262a.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/speech-caef5ead.js` & `langflow_base-0.0.49/langflow/frontend/assets/speech-caef5ead.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/spray-can-d7810702.js` & `langflow_base-0.0.49/langflow/frontend/assets/spray-can-d7810702.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/sprout-2941b7af.js` & `langflow_base-0.0.49/langflow/frontend/assets/sprout-2941b7af.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/square-dashed-bottom-code-778cf01d.js` & `langflow_base-0.0.49/langflow/frontend/assets/square-dashed-bottom-code-778cf01d.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/squirrel-1f8d0f35.js` & `langflow_base-0.0.49/langflow/frontend/assets/squirrel-1f8d0f35.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/stamp-59355141.js` & `langflow_base-0.0.49/langflow/frontend/assets/stamp-59355141.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/stethoscope-1fa99fa8.js` & `langflow_base-0.0.49/langflow/frontend/assets/stethoscope-1fa99fa8.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/sticker-144df895.js` & `langflow_base-0.0.49/langflow/frontend/assets/sticker-144df895.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/sun-dim-24f43cd5.js` & `langflow_base-0.0.49/langflow/frontend/assets/sun-dim-24f43cd5.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/sun-medium-820ad250.js` & `langflow_base-0.0.49/langflow/frontend/assets/sun-medium-820ad250.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/sun-moon-690f2196.js` & `langflow_base-0.0.49/langflow/frontend/assets/sun-moon-690f2196.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/sun-snow-5e3f18c5.js` & `langflow_base-0.0.49/langflow/frontend/assets/sun-snow-5e3f18c5.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/sunrise-65a8ae93.js` & `langflow_base-0.0.49/langflow/frontend/assets/sunrise-65a8ae93.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/sunset-51bf7930.js` & `langflow_base-0.0.49/langflow/frontend/assets/sunset-51bf7930.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/swatch-book-217377ae.js` & `langflow_base-0.0.49/langflow/frontend/assets/swatch-book-217377ae.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/switch-camera-be80e3cf.js` & `langflow_base-0.0.49/langflow/frontend/assets/switch-camera-be80e3cf.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/swords-bdda5651.js` & `langflow_base-0.0.49/langflow/frontend/assets/swords-bdda5651.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/syringe-530e6026.js` & `langflow_base-0.0.49/langflow/frontend/assets/syringe-530e6026.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/tags-be256b31.js` & `langflow_base-0.0.49/langflow/frontend/assets/tags-be256b31.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/telescope-f24b3ac3.js` & `langflow_base-0.0.49/langflow/frontend/assets/telescope-f24b3ac3.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/tent-tree-48eb1ffa.js` & `langflow_base-0.0.49/langflow/frontend/assets/tent-tree-48eb1ffa.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/test-tubes-e92b4851.js` & `langflow_base-0.0.49/langflow/frontend/assets/test-tubes-e92b4851.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/text-select-4cd99566.js` & `langflow_base-0.0.49/langflow/frontend/assets/text-select-4cd99566.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/theater-a353a219.js` & `langflow_base-0.0.49/langflow/frontend/assets/theater-a353a219.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/thermometer-snowflake-be8d8d4e.js` & `langflow_base-0.0.49/langflow/frontend/assets/thermometer-snowflake-be8d8d4e.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/thermometer-sun-94d72684.js` & `langflow_base-0.0.49/langflow/frontend/assets/thermometer-sun-94d72684.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/timer-off-ebfa1a04.js` & `langflow_base-0.0.49/langflow/frontend/assets/timer-off-ebfa1a04.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/touchpad-off-14143303.js` & `langflow_base-0.0.49/langflow/frontend/assets/touchpad-off-14143303.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/tower-control-d0da130d.js` & `langflow_base-0.0.49/langflow/frontend/assets/tower-control-d0da130d.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/tractor-f0adfa2a.js` & `langflow_base-0.0.49/langflow/frontend/assets/tractor-f0adfa2a.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/traffic-cone-62187088.js` & `langflow_base-0.0.49/langflow/frontend/assets/traffic-cone-62187088.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/train-front-bd9494d4.js` & `langflow_base-0.0.49/langflow/frontend/assets/train-front-bd9494d4.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/train-front-tunnel-4cd69150.js` & `langflow_base-0.0.49/langflow/frontend/assets/train-front-tunnel-4cd69150.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/train-track-5fdf782c.js` & `langflow_base-0.0.49/langflow/frontend/assets/train-track-5fdf782c.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/tram-front-b7bd0d07.js` & `langflow_base-0.0.49/langflow/frontend/assets/tram-front-b7bd0d07.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/trees-7698e8a4.js` & `langflow_base-0.0.49/langflow/frontend/assets/trees-7698e8a4.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/trophy-2d75b216.js` & `langflow_base-0.0.49/langflow/frontend/assets/trophy-2d75b216.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/truck-c4b0a7fc.js` & `langflow_base-0.0.49/langflow/frontend/assets/truck-c4b0a7fc.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/turtle-b3106944.js` & `langflow_base-0.0.49/langflow/frontend/assets/turtle-b3106944.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/undraw_blog_post_re_fy5x-de7369a0.svg` & `langflow_base-0.0.49/langflow/frontend/assets/undraw_blog_post_re_fy5x-de7369a0.svg`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/undraw_chat_bot_re_e2gj-eceb89b6.svg` & `langflow_base-0.0.49/langflow/frontend/assets/undraw_chat_bot_re_e2gj-eceb89b6.svg`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/undraw_cloud_docs_re_xjht-c1ec41f9.svg` & `langflow_base-0.0.49/langflow/frontend/assets/undraw_cloud_docs_re_xjht-c1ec41f9.svg`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/undraw_real_time_analytics_re_yliv-25632bd9.svg` & `langflow_base-0.0.49/langflow/frontend/assets/undraw_real_time_analytics_re_yliv-25632bd9.svg`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/undraw_short_bio_re_fmx0-949a7b7d.svg` & `langflow_base-0.0.49/langflow/frontend/assets/undraw_short_bio_re_fmx0-949a7b7d.svg`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/undraw_transfer_files_re_a2a9-c499dfcb.svg` & `langflow_base-0.0.49/langflow/frontend/assets/undraw_transfer_files_re_a2a9-c499dfcb.svg`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/unfold-horizontal-5cdb7854.js` & `langflow_base-0.0.49/langflow/frontend/assets/unfold-horizontal-5cdb7854.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/unfold-vertical-98fd63f5.js` & `langflow_base-0.0.49/langflow/frontend/assets/unfold-vertical-98fd63f5.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/unlink-684a02e2.js` & `langflow_base-0.0.49/langflow/frontend/assets/unlink-684a02e2.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/usb-4c542cb8.js` & `langflow_base-0.0.49/langflow/frontend/assets/usb-4c542cb8.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/user-cog-042a9c97.js` & `langflow_base-0.0.49/langflow/frontend/assets/user-cog-042a9c97.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/utensils-crossed-8fc371ec.js` & `langflow_base-0.0.49/langflow/frontend/assets/utensils-crossed-8fc371ec.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/utility-pole-9d58dfcf.js` & `langflow_base-0.0.49/langflow/frontend/assets/utility-pole-9d58dfcf.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/vault-038eee2a.js` & `langflow_base-0.0.49/langflow/frontend/assets/vault-038eee2a.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/venetian-mask-fe3f1aeb.js` & `langflow_base-0.0.49/langflow/frontend/assets/venetian-mask-fe3f1aeb.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/vibrate-off-0bdf0a78.js` & `langflow_base-0.0.49/langflow/frontend/assets/vibrate-off-0bdf0a78.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/view-f9e42cb1.js` & `langflow_base-0.0.49/langflow/frontend/assets/view-f9e42cb1.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/wand-28efcf56.js` & `langflow_base-0.0.49/langflow/frontend/assets/wand-28efcf56.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/warehouse-f82177ac.js` & `langflow_base-0.0.49/langflow/frontend/assets/warehouse-f82177ac.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/washing-machine-c4d18bcb.js` & `langflow_base-0.0.49/langflow/frontend/assets/washing-machine-c4d18bcb.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/watch-4d03e446.js` & `langflow_base-0.0.49/langflow/frontend/assets/watch-4d03e446.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/waves-c75c9971.js` & `langflow_base-0.0.49/langflow/frontend/assets/waves-c75c9971.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/waypoints-4f37dfb8.js` & `langflow_base-0.0.49/langflow/frontend/assets/waypoints-4f37dfb8.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/web-vitals-60d3425a.js` & `langflow_base-0.0.49/langflow/frontend/assets/web-vitals-60d3425a.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/webhook-9f58c70e.js` & `langflow_base-0.0.49/langflow/frontend/assets/webhook-9f58c70e.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/webhook-off-d5460710.js` & `langflow_base-0.0.49/langflow/frontend/assets/webhook-off-d5460710.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/wheat-0b843377.js` & `langflow_base-0.0.49/langflow/frontend/assets/wheat-0b843377.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/wheat-off-a706bc18.js` & `langflow_base-0.0.49/langflow/frontend/assets/wheat-off-a706bc18.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/wifi-off-a80416b7.js` & `langflow_base-0.0.49/langflow/frontend/assets/wifi-off-a80416b7.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/assets/wine-off-9c00409f.js` & `langflow_base-0.0.49/langflow/frontend/assets/wine-off-9c00409f.js`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/favicon.ico` & `langflow_base-0.0.49/langflow/frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/frontend/index.html` & `langflow_base-0.0.49/langflow/frontend/index.html`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/graph/edge/base.py` & `langflow_base-0.0.49/langflow/graph/edge/base.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/graph/edge/schema.py` & `langflow_base-0.0.49/langflow/graph/edge/schema.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/graph/graph/base.py` & `langflow_base-0.0.49/langflow/graph/graph/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 from langflow.graph.edge.base import ContractEdge
 from langflow.graph.graph.constants import lazy_load_vertex_dict
 from langflow.graph.graph.runnable_vertices_manager import RunnableVerticesManager
 from langflow.graph.graph.state_manager import GraphStateManager
 from langflow.graph.graph.utils import process_flow
 from langflow.graph.schema import InterfaceComponentTypes, RunOutputs
 from langflow.graph.vertex.base import Vertex
-from langflow.graph.vertex.types import FileToolVertex, InterfaceVertex, LLMVertex, StateVertex, ToolkitVertex
-from langflow.interface.tools.constants import FILE_TOOLS
+from langflow.graph.vertex.types import InterfaceVertex, StateVertex
 from langflow.schema import Record
 from langflow.schema.schema import INPUT_FIELD_NAME, InputType
 from langflow.services.deps import get_chat_service
 
 if TYPE_CHECKING:
     from langflow.graph.schema import ResultData
 
@@ -683,24 +682,16 @@
             return
         self.vertices.remove(vertex)
         self.vertex_map.pop(vertex_id)
         self.edges = [edge for edge in self.edges if edge.source_id != vertex_id and edge.target_id != vertex_id]
 
     def _build_vertex_params(self) -> None:
         """Identifies and handles the LLM vertex within the graph."""
-        llm_vertex = None
         for vertex in self.vertices:
             vertex._build_params()
-            if isinstance(vertex, LLMVertex):
-                llm_vertex = vertex
-
-        if llm_vertex:
-            for vertex in self.vertices:
-                if isinstance(vertex, ToolkitVertex):
-                    vertex.params["llm"] = llm_vertex
 
     def _validate_vertex(self, vertex: Vertex) -> bool:
         """Validates a vertex."""
         # All vertices that do not have edges are invalid
         return len(self.get_vertex_edges(vertex.id)) > 0
 
     def get_vertex(self, vertex_id: str) -> Vertex:
@@ -999,16 +990,14 @@
         elif node_name in ["SharedState", "Notify", "Listen"]:
             return StateVertex
         elif node_base_type in lazy_load_vertex_dict.VERTEX_TYPE_MAP:
             return lazy_load_vertex_dict.VERTEX_TYPE_MAP[node_base_type]
         elif node_name in lazy_load_vertex_dict.VERTEX_TYPE_MAP:
             return lazy_load_vertex_dict.VERTEX_TYPE_MAP[node_name]
 
-        if node_type in FILE_TOOLS:
-            return FileToolVertex
         if node_type in lazy_load_vertex_dict.VERTEX_TYPE_MAP:
             return lazy_load_vertex_dict.VERTEX_TYPE_MAP[node_type]
         return (
             lazy_load_vertex_dict.VERTEX_TYPE_MAP[node_base_type]
             if node_base_type in lazy_load_vertex_dict.VERTEX_TYPE_MAP
             else Vertex
         )
```

### Comparing `langflow_base-0.0.48/langflow/graph/graph/runnable_vertices_manager.py` & `langflow_base-0.0.49/langflow/graph/graph/runnable_vertices_manager.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/graph/graph/state_manager.py` & `langflow_base-0.0.49/langflow/graph/graph/state_manager.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/graph/graph/utils.py` & `langflow_base-0.0.49/langflow/graph/graph/utils.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/graph/schema.py` & `langflow_base-0.0.49/langflow/graph/schema.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/graph/utils.py` & `langflow_base-0.0.49/langflow/graph/utils.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/graph/vertex/base.py` & `langflow_base-0.0.49/langflow/graph/vertex/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from enum import Enum
 from typing import TYPE_CHECKING, Any, AsyncIterator, Callable, Dict, Iterator, List, Optional
 
 from loguru import logger
 
 from langflow.graph.schema import INPUT_COMPONENTS, OUTPUT_COMPONENTS, InterfaceComponentTypes, ResultData
 from langflow.graph.utils import UnbuiltObject, UnbuiltResult
-from langflow.graph.vertex.utils import generate_result, log_transaction
+from langflow.graph.vertex.utils import log_transaction
 from langflow.interface.initialize import loading
 from langflow.interface.listing import lazy_load_dict
 from langflow.schema.schema import INPUT_FIELD_NAME
 from langflow.services.deps import get_storage_service
 from langflow.utils.constants import DIRECT_TYPES
 from langflow.utils.schemas import ChatOutputResponse
 from langflow.utils.util import sync_to_async, unescape_string
@@ -450,37 +450,14 @@
             artifacts=artifacts,
             messages=messages,
             component_display_name=self.display_name,
             component_id=self.id,
         )
         self.set_result(result_dict)
 
-    async def _run(
-        self,
-        user_id: str,
-        inputs: Optional[dict] = None,
-        session_id: Optional[str] = None,
-    ):
-        # user_id is just for compatibility with the other build methods
-        inputs = inputs or {}
-        # inputs = {key: value or "" for key, value in inputs.items()}
-        # if hasattr(self._built_object, "input_keys"):
-        #     # test if all keys are in inputs
-        #     # and if not add them with empty string
-        #     # for key in self._built_object.input_keys:
-        #     #     if key not in inputs:
-        #     #         inputs[key] = ""
-        #     if inputs == {} and hasattr(self._built_object, "prompt"):
-        #         inputs = self._built_object.prompt.partial_variables
-        if isinstance(self._built_object, str):
-            self._built_result = self._built_object
-
-        result = await generate_result(self._built_object, inputs, self.has_external_output, session_id)
-        self._built_result = result
-
     async def _build_each_vertex_in_params_dict(self, user_id=None):
         """
         Iterates over each vertex in the params dictionary and builds it.
         """
         for key, value in self._raw_params.items():
             if self._is_vertex(value):
                 if value == self:
```

### Comparing `langflow_base-0.0.48/langflow/helpers/flow.py` & `langflow_base-0.0.49/langflow/helpers/flow.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/helpers/record.py` & `langflow_base-0.0.49/langflow/helpers/record.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/initial_setup/setup.py` & `langflow_base-0.0.49/langflow/initial_setup/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
     project_name,
     project_description,
     project_is_component,
     updated_at_datetime,
     project_data,
     project_icon,
     project_icon_bg_color,
-    new_folder_id
+    new_folder_id,
 ):
     logger.debug(f"Creating starter project {project_name}")
     new_project = FlowCreate(
         name=project_name,
         description=project_description,
         icon=project_icon,
         icon_bg_color=project_icon_bg_color,
@@ -202,15 +202,15 @@
         session.refresh(db_folder)
         return db_folder
     else:
         return session.exec(select(Folder).where(Folder.name == STARTER_FOLDER_NAME)).first()
 
 
 def create_or_update_starter_projects():
-    components_paths = get_settings_service().settings.COMPONENTS_PATH
+    components_paths = get_settings_service().settings.components_path
     try:
         all_types_dict = get_all_components(components_paths, as_dict=True)
     except Exception as e:
         logger.exception(f"Error loading components: {e}")
         raise e
     with session_scope() as session:
         new_folder = create_starter_folder(session)
@@ -243,9 +243,9 @@
                     project_name,
                     project_description,
                     project_is_component,
                     updated_at_datetime,
                     project_data,
                     project_icon,
                     project_icon_bg_color,
-                    new_folder.id
+                    new_folder.id,
                 )
```

### Comparing `langflow_base-0.0.48/langflow/initial_setup/starter_projects/Basic Prompting (Hello, world!).json` & `langflow_base-0.0.49/langflow/initial_setup/starter_projects/Basic Prompting (Hello, world!).json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999999995690651%*

 * *Differences: {"'data'": "{'nodes': {0: {'data': {'node': {'template': {'code': {'value': 'from "*

 * *           'langchain_core.prompts import PromptTemplate\\n\\nfrom langflow.custom import '*

 * *           'CustomComponent\\nfrom langflow.field_typing import Prompt, TemplateField, '*

 * *           'Text\\n\\n\\nclass PromptComponent(CustomComponent):\\n    display_name: str = '*

 * *           '"Prompt"\\n    description: str = "Create a prompt template with dynamic '*

 * *           'variables."\\n    icon = "prompts"\\n\\n    def build_c […]*

```diff
@@ -144,15 +144,15 @@
                                 "name": "code",
                                 "password": false,
                                 "placeholder": "",
                                 "required": true,
                                 "show": true,
                                 "title_case": false,
                                 "type": "code",
-                                "value": "from langchain_core.prompts import PromptTemplate\n\nfrom langflow.field_typing import Prompt, TemplateField, Text\nfrom langflow.interface.custom.custom_component import CustomComponent\n\n\nclass PromptComponent(CustomComponent):\n    display_name: str = \"Prompt\"\n    description: str = \"Create a prompt template with dynamic variables.\"\n    icon = \"prompts\"\n\n    def build_config(self):\n        return {\n            \"template\": TemplateField(display_name=\"Template\"),\n            \"code\": TemplateField(advanced=True),\n        }\n\n    def build(\n        self,\n        template: Prompt,\n        **kwargs,\n    ) -> Text:\n        from langflow.base.prompts.utils import dict_values_to_string\n\n        prompt_template = PromptTemplate.from_template(Text(template))\n        kwargs = dict_values_to_string(kwargs)\n        kwargs = {k: \"\\n\".join(v) if isinstance(v, list) else v for k, v in kwargs.items()}\n        try:\n            formated_prompt = prompt_template.format(**kwargs)\n        except Exception as exc:\n            raise ValueError(f\"Error formatting prompt: {exc}\") from exc\n        self.status = f'Prompt:\\n\"{formated_prompt}\"'\n        return formated_prompt\n"
+                                "value": "from langchain_core.prompts import PromptTemplate\n\nfrom langflow.custom import CustomComponent\nfrom langflow.field_typing import Prompt, TemplateField, Text\n\n\nclass PromptComponent(CustomComponent):\n    display_name: str = \"Prompt\"\n    description: str = \"Create a prompt template with dynamic variables.\"\n    icon = \"prompts\"\n\n    def build_config(self):\n        return {\n            \"template\": TemplateField(display_name=\"Template\"),\n            \"code\": TemplateField(advanced=True),\n        }\n\n    def build(\n        self,\n        template: Prompt,\n        **kwargs,\n    ) -> Text:\n        from langflow.base.prompts.utils import dict_values_to_string\n\n        prompt_template = PromptTemplate.from_template(Text(template))\n        kwargs = dict_values_to_string(kwargs)\n        kwargs = {k: \"\\n\".join(v) if isinstance(v, list) else v for k, v in kwargs.items()}\n        try:\n            formated_prompt = prompt_template.format(**kwargs)\n        except Exception as exc:\n            raise ValueError(f\"Error formatting prompt: {exc}\") from exc\n        self.status = f'Prompt:\\n\"{formated_prompt}\"'\n        return formated_prompt\n"
                             },
                             "template": {
                                 "advanced": false,
                                 "display_name": "Template",
                                 "dynamic": false,
                                 "fileTypes": [],
                                 "file_path": "",
@@ -274,15 +274,15 @@
                                 "name": "code",
                                 "password": false,
                                 "placeholder": "",
                                 "required": true,
                                 "show": true,
                                 "title_case": false,
                                 "type": "code",
-                                "value": "from typing import Optional\n\nfrom langchain_openai import ChatOpenAI\nfrom pydantic.v1 import SecretStr\n\nfrom langflow.base.constants import STREAM_INFO_TEXT\nfrom langflow.base.models.model import LCModelComponent\nfrom langflow.base.models.openai_constants import MODEL_NAMES\nfrom langflow.field_typing import NestedDict, Text\n\n\nclass OpenAIModelComponent(LCModelComponent):\n    display_name = \"OpenAI\"\n    description = \"Generates text using OpenAI LLMs.\"\n    icon = \"OpenAI\"\n\n    field_order = [\n        \"max_tokens\",\n        \"model_kwargs\",\n        \"model_name\",\n        \"openai_api_base\",\n        \"openai_api_key\",\n        \"temperature\",\n        \"input_value\",\n        \"system_message\",\n        \"stream\",\n    ]\n\n    def build_config(self):\n        return {\n            \"input_value\": {\"display_name\": \"Input\"},\n            \"max_tokens\": {\n                \"display_name\": \"Max Tokens\",\n                \"advanced\": True,\n            },\n            \"model_kwargs\": {\n                \"display_name\": \"Model Kwargs\",\n                \"advanced\": True,\n            },\n            \"model_name\": {\n                \"display_name\": \"Model Name\",\n                \"advanced\": False,\n                \"options\": MODEL_NAMES,\n            },\n            \"openai_api_base\": {\n                \"display_name\": \"OpenAI API Base\",\n                \"advanced\": True,\n                \"info\": (\n                    \"The base URL of the OpenAI API. Defaults to https://api.openai.com/v1.\\n\\n\"\n                    \"You can change this to use other APIs like JinaChat, LocalAI and Prem.\"\n                ),\n            },\n            \"openai_api_key\": {\n                \"display_name\": \"OpenAI API Key\",\n                \"info\": \"The OpenAI API Key to use for the OpenAI model.\",\n                \"advanced\": False,\n                \"password\": True,\n            },\n            \"temperature\": {\n                \"display_name\": \"Temperature\",\n                \"advanced\": False,\n                \"value\": 0.1,\n            },\n            \"stream\": {\n                \"display_name\": \"Stream\",\n                \"info\": STREAM_INFO_TEXT,\n                \"advanced\": True,\n            },\n            \"system_message\": {\n                \"display_name\": \"System Message\",\n                \"info\": \"System message to pass to the model.\",\n                \"advanced\": True,\n            },\n        }\n\n    def build(\n        self,\n        input_value: Text,\n        openai_api_key: str,\n        temperature: float,\n        model_name: str = \"gpt-4o\",\n        max_tokens: Optional[int] = 256,\n        model_kwargs: NestedDict = {},\n        openai_api_base: Optional[str] = None,\n        stream: bool = False,\n        system_message: Optional[str] = None,\n    ) -> Text:\n        if not openai_api_base:\n            openai_api_base = \"https://api.openai.com/v1\"\n        if openai_api_key:\n            api_key = SecretStr(openai_api_key)\n        else:\n            api_key = None\n\n        output = ChatOpenAI(\n            max_tokens=max_tokens,\n            model_kwargs=model_kwargs,\n            model=model_name,\n            base_url=openai_api_base,\n            api_key=api_key,\n            temperature=temperature,\n        )\n\n        return self.get_chat_result(output, stream, input_value, system_message)\n"
+                                "value": "from typing import Optional\n\nfrom langchain_openai import ChatOpenAI\nfrom pydantic.v1 import SecretStr\n\nfrom langflow.base.constants import STREAM_INFO_TEXT\nfrom langflow.base.models.model import LCModelComponent\nfrom langflow.base.models.openai_constants import MODEL_NAMES\nfrom langflow.field_typing import NestedDict, Text\n\n\nclass OpenAIModelComponent(LCModelComponent):\n    display_name = \"OpenAI\"\n    description = \"Generates text using OpenAI LLMs.\"\n    icon = \"OpenAI\"\n\n    field_order = [\n        \"max_tokens\",\n        \"model_kwargs\",\n        \"model_name\",\n        \"openai_api_base\",\n        \"openai_api_key\",\n        \"temperature\",\n        \"input_value\",\n        \"system_message\",\n        \"stream\",\n    ]\n\n    def build_config(self):\n        return {\n            \"input_value\": {\"display_name\": \"Input\"},\n            \"max_tokens\": {\n                \"display_name\": \"Max Tokens\",\n                \"advanced\": True,\n                \"info\": \"The maximum number of tokens to generate. Set to 0 for unlimited tokens.\",\n            },\n            \"model_kwargs\": {\n                \"display_name\": \"Model Kwargs\",\n                \"advanced\": True,\n            },\n            \"model_name\": {\n                \"display_name\": \"Model Name\",\n                \"advanced\": False,\n                \"options\": MODEL_NAMES,\n            },\n            \"openai_api_base\": {\n                \"display_name\": \"OpenAI API Base\",\n                \"advanced\": True,\n                \"info\": (\n                    \"The base URL of the OpenAI API. Defaults to https://api.openai.com/v1.\\n\\n\"\n                    \"You can change this to use other APIs like JinaChat, LocalAI and Prem.\"\n                ),\n            },\n            \"openai_api_key\": {\n                \"display_name\": \"OpenAI API Key\",\n                \"info\": \"The OpenAI API Key to use for the OpenAI model.\",\n                \"advanced\": False,\n                \"password\": True,\n            },\n            \"temperature\": {\n                \"display_name\": \"Temperature\",\n                \"advanced\": False,\n                \"value\": 0.1,\n            },\n            \"stream\": {\n                \"display_name\": \"Stream\",\n                \"info\": STREAM_INFO_TEXT,\n                \"advanced\": True,\n            },\n            \"system_message\": {\n                \"display_name\": \"System Message\",\n                \"info\": \"System message to pass to the model.\",\n                \"advanced\": True,\n            },\n        }\n\n    def build(\n        self,\n        input_value: Text,\n        openai_api_key: str,\n        temperature: float,\n        model_name: str = \"gpt-4o\",\n        max_tokens: Optional[int] = 256,\n        model_kwargs: NestedDict = {},\n        openai_api_base: Optional[str] = None,\n        stream: bool = False,\n        system_message: Optional[str] = None,\n    ) -> Text:\n        if not openai_api_base:\n            openai_api_base = \"https://api.openai.com/v1\"\n        if openai_api_key:\n            api_key = SecretStr(openai_api_key)\n        else:\n            api_key = None\n\n        output = ChatOpenAI(\n            max_tokens=max_tokens or None,\n            model_kwargs=model_kwargs,\n            model=model_name,\n            base_url=openai_api_base,\n            api_key=api_key,\n            temperature=temperature,\n        )\n\n        return self.get_chat_result(output, stream, input_value, system_message)\n"
                             },
                             "input_value": {
                                 "advanced": false,
                                 "display_name": "Input",
                                 "dynamic": false,
                                 "fileTypes": [],
                                 "file_path": "",
@@ -303,15 +303,15 @@
                             },
                             "max_tokens": {
                                 "advanced": true,
                                 "display_name": "Max Tokens",
                                 "dynamic": false,
                                 "fileTypes": [],
                                 "file_path": "",
-                                "info": "",
+                                "info": "The maximum number of tokens to generate. Set to 0 for unlimited tokens.",
                                 "list": false,
                                 "load_from_db": false,
                                 "multiline": false,
                                 "name": "max_tokens",
                                 "password": false,
                                 "placeholder": "",
                                 "required": false,
```

### Comparing `langflow_base-0.0.48/langflow/initial_setup/starter_projects/Langflow Blog Writter.json` & `langflow_base-0.0.49/langflow/initial_setup/starter_projects/Langflow Blog Writter.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999999873045211%*

 * *Differences: {"'data'": "{'nodes': {0: {'data': {'node': {'template': {'code': {'value': 'from "*

 * *           'langchain_core.prompts import PromptTemplate\\n\\nfrom langflow.custom import '*

 * *           'CustomComponent\\nfrom langflow.field_typing import Prompt, TemplateField, '*

 * *           'Text\\n\\n\\nclass PromptComponent(CustomComponent):\\n    display_name: str = '*

 * *           '"Prompt"\\n    description: str = "Create a prompt template with dynamic '*

 * *           'variables."\\n    icon = "prompts"\\n\\n    def build_c […]*

```diff
@@ -209,15 +209,15 @@
                                 "name": "code",
                                 "password": false,
                                 "placeholder": "",
                                 "required": true,
                                 "show": true,
                                 "title_case": false,
                                 "type": "code",
-                                "value": "from langchain_core.prompts import PromptTemplate\n\nfrom langflow.field_typing import Prompt, TemplateField, Text\nfrom langflow.interface.custom.custom_component import CustomComponent\n\n\nclass PromptComponent(CustomComponent):\n    display_name: str = \"Prompt\"\n    description: str = \"Create a prompt template with dynamic variables.\"\n    icon = \"prompts\"\n\n    def build_config(self):\n        return {\n            \"template\": TemplateField(display_name=\"Template\"),\n            \"code\": TemplateField(advanced=True),\n        }\n\n    def build(\n        self,\n        template: Prompt,\n        **kwargs,\n    ) -> Text:\n        from langflow.base.prompts.utils import dict_values_to_string\n\n        prompt_template = PromptTemplate.from_template(Text(template))\n        kwargs = dict_values_to_string(kwargs)\n        kwargs = {k: \"\\n\".join(v) if isinstance(v, list) else v for k, v in kwargs.items()}\n        try:\n            formated_prompt = prompt_template.format(**kwargs)\n        except Exception as exc:\n            raise ValueError(f\"Error formatting prompt: {exc}\") from exc\n        self.status = f'Prompt:\\n\"{formated_prompt}\"'\n        return formated_prompt\n"
+                                "value": "from langchain_core.prompts import PromptTemplate\n\nfrom langflow.custom import CustomComponent\nfrom langflow.field_typing import Prompt, TemplateField, Text\n\n\nclass PromptComponent(CustomComponent):\n    display_name: str = \"Prompt\"\n    description: str = \"Create a prompt template with dynamic variables.\"\n    icon = \"prompts\"\n\n    def build_config(self):\n        return {\n            \"template\": TemplateField(display_name=\"Template\"),\n            \"code\": TemplateField(advanced=True),\n        }\n\n    def build(\n        self,\n        template: Prompt,\n        **kwargs,\n    ) -> Text:\n        from langflow.base.prompts.utils import dict_values_to_string\n\n        prompt_template = PromptTemplate.from_template(Text(template))\n        kwargs = dict_values_to_string(kwargs)\n        kwargs = {k: \"\\n\".join(v) if isinstance(v, list) else v for k, v in kwargs.items()}\n        try:\n            formated_prompt = prompt_template.format(**kwargs)\n        except Exception as exc:\n            raise ValueError(f\"Error formatting prompt: {exc}\") from exc\n        self.status = f'Prompt:\\n\"{formated_prompt}\"'\n        return formated_prompt\n"
                             },
                             "instructions": {
                                 "advanced": false,
                                 "display_name": "instructions",
                                 "dynamic": false,
                                 "field_type": "str",
                                 "fileTypes": [],
@@ -369,15 +369,15 @@
                                 "name": "code",
                                 "password": false,
                                 "placeholder": "",
                                 "required": true,
                                 "show": true,
                                 "title_case": false,
                                 "type": "code",
-                                "value": "from typing import Any, Dict\n\nfrom langchain_community.document_loaders.web_base import WebBaseLoader\n\nfrom langflow.interface.custom.custom_component import CustomComponent\nfrom langflow.schema import Record\n\n\nclass URLComponent(CustomComponent):\n    display_name = \"URL\"\n    description = \"Fetch content from one or more URLs.\"\n    icon = \"layout-template\"\n\n    def build_config(self) -> Dict[str, Any]:\n        return {\n            \"urls\": {\"display_name\": \"URL\"},\n        }\n\n    def build(\n        self,\n        urls: list[str],\n    ) -> list[Record]:\n        loader = WebBaseLoader(web_paths=urls)\n        docs = loader.load()\n        records = self.to_records(docs)\n        self.status = records\n        return records\n"
+                                "value": "from typing import Any, Dict\n\nfrom langchain_community.document_loaders.web_base import WebBaseLoader\n\nfrom langflow.custom import CustomComponent\nfrom langflow.schema import Record\n\n\nclass URLComponent(CustomComponent):\n    display_name = \"URL\"\n    description = \"Fetch content from one or more URLs.\"\n    icon = \"layout-template\"\n\n    def build_config(self) -> Dict[str, Any]:\n        return {\n            \"urls\": {\"display_name\": \"URL\"},\n        }\n\n    def build(\n        self,\n        urls: list[str],\n    ) -> list[Record]:\n        loader = WebBaseLoader(web_paths=urls)\n        docs = loader.load()\n        records = self.to_records(docs)\n        self.status = records\n        return records\n"
                             },
                             "urls": {
                                 "advanced": false,
                                 "display_name": "URL",
                                 "dynamic": false,
                                 "fileTypes": [],
                                 "file_path": "",
@@ -668,15 +668,15 @@
                                 "name": "code",
                                 "password": false,
                                 "placeholder": "",
                                 "required": true,
                                 "show": true,
                                 "title_case": false,
                                 "type": "code",
-                                "value": "from typing import Optional\n\nfrom langchain_openai import ChatOpenAI\nfrom pydantic.v1 import SecretStr\n\nfrom langflow.base.constants import STREAM_INFO_TEXT\nfrom langflow.base.models.model import LCModelComponent\nfrom langflow.base.models.openai_constants import MODEL_NAMES\nfrom langflow.field_typing import NestedDict, Text\n\n\nclass OpenAIModelComponent(LCModelComponent):\n    display_name = \"OpenAI\"\n    description = \"Generates text using OpenAI LLMs.\"\n    icon = \"OpenAI\"\n\n    field_order = [\n        \"max_tokens\",\n        \"model_kwargs\",\n        \"model_name\",\n        \"openai_api_base\",\n        \"openai_api_key\",\n        \"temperature\",\n        \"input_value\",\n        \"system_message\",\n        \"stream\",\n    ]\n\n    def build_config(self):\n        return {\n            \"input_value\": {\"display_name\": \"Input\"},\n            \"max_tokens\": {\n                \"display_name\": \"Max Tokens\",\n                \"advanced\": True,\n            },\n            \"model_kwargs\": {\n                \"display_name\": \"Model Kwargs\",\n                \"advanced\": True,\n            },\n            \"model_name\": {\n                \"display_name\": \"Model Name\",\n                \"advanced\": False,\n                \"options\": MODEL_NAMES,\n            },\n            \"openai_api_base\": {\n                \"display_name\": \"OpenAI API Base\",\n                \"advanced\": True,\n                \"info\": (\n                    \"The base URL of the OpenAI API. Defaults to https://api.openai.com/v1.\\n\\n\"\n                    \"You can change this to use other APIs like JinaChat, LocalAI and Prem.\"\n                ),\n            },\n            \"openai_api_key\": {\n                \"display_name\": \"OpenAI API Key\",\n                \"info\": \"The OpenAI API Key to use for the OpenAI model.\",\n                \"advanced\": False,\n                \"password\": True,\n            },\n            \"temperature\": {\n                \"display_name\": \"Temperature\",\n                \"advanced\": False,\n                \"value\": 0.1,\n            },\n            \"stream\": {\n                \"display_name\": \"Stream\",\n                \"info\": STREAM_INFO_TEXT,\n                \"advanced\": True,\n            },\n            \"system_message\": {\n                \"display_name\": \"System Message\",\n                \"info\": \"System message to pass to the model.\",\n                \"advanced\": True,\n            },\n        }\n\n    def build(\n        self,\n        input_value: Text,\n        openai_api_key: str,\n        temperature: float,\n        model_name: str = \"gpt-4o\",\n        max_tokens: Optional[int] = 256,\n        model_kwargs: NestedDict = {},\n        openai_api_base: Optional[str] = None,\n        stream: bool = False,\n        system_message: Optional[str] = None,\n    ) -> Text:\n        if not openai_api_base:\n            openai_api_base = \"https://api.openai.com/v1\"\n        if openai_api_key:\n            api_key = SecretStr(openai_api_key)\n        else:\n            api_key = None\n\n        output = ChatOpenAI(\n            max_tokens=max_tokens,\n            model_kwargs=model_kwargs,\n            model=model_name,\n            base_url=openai_api_base,\n            api_key=api_key,\n            temperature=temperature,\n        )\n\n        return self.get_chat_result(output, stream, input_value, system_message)\n"
+                                "value": "from typing import Optional\n\nfrom langchain_openai import ChatOpenAI\nfrom pydantic.v1 import SecretStr\n\nfrom langflow.base.constants import STREAM_INFO_TEXT\nfrom langflow.base.models.model import LCModelComponent\nfrom langflow.base.models.openai_constants import MODEL_NAMES\nfrom langflow.field_typing import NestedDict, Text\n\n\nclass OpenAIModelComponent(LCModelComponent):\n    display_name = \"OpenAI\"\n    description = \"Generates text using OpenAI LLMs.\"\n    icon = \"OpenAI\"\n\n    field_order = [\n        \"max_tokens\",\n        \"model_kwargs\",\n        \"model_name\",\n        \"openai_api_base\",\n        \"openai_api_key\",\n        \"temperature\",\n        \"input_value\",\n        \"system_message\",\n        \"stream\",\n    ]\n\n    def build_config(self):\n        return {\n            \"input_value\": {\"display_name\": \"Input\"},\n            \"max_tokens\": {\n                \"display_name\": \"Max Tokens\",\n                \"advanced\": True,\n                \"info\": \"The maximum number of tokens to generate. Set to 0 for unlimited tokens.\",\n            },\n            \"model_kwargs\": {\n                \"display_name\": \"Model Kwargs\",\n                \"advanced\": True,\n            },\n            \"model_name\": {\n                \"display_name\": \"Model Name\",\n                \"advanced\": False,\n                \"options\": MODEL_NAMES,\n            },\n            \"openai_api_base\": {\n                \"display_name\": \"OpenAI API Base\",\n                \"advanced\": True,\n                \"info\": (\n                    \"The base URL of the OpenAI API. Defaults to https://api.openai.com/v1.\\n\\n\"\n                    \"You can change this to use other APIs like JinaChat, LocalAI and Prem.\"\n                ),\n            },\n            \"openai_api_key\": {\n                \"display_name\": \"OpenAI API Key\",\n                \"info\": \"The OpenAI API Key to use for the OpenAI model.\",\n                \"advanced\": False,\n                \"password\": True,\n            },\n            \"temperature\": {\n                \"display_name\": \"Temperature\",\n                \"advanced\": False,\n                \"value\": 0.1,\n            },\n            \"stream\": {\n                \"display_name\": \"Stream\",\n                \"info\": STREAM_INFO_TEXT,\n                \"advanced\": True,\n            },\n            \"system_message\": {\n                \"display_name\": \"System Message\",\n                \"info\": \"System message to pass to the model.\",\n                \"advanced\": True,\n            },\n        }\n\n    def build(\n        self,\n        input_value: Text,\n        openai_api_key: str,\n        temperature: float,\n        model_name: str = \"gpt-4o\",\n        max_tokens: Optional[int] = 256,\n        model_kwargs: NestedDict = {},\n        openai_api_base: Optional[str] = None,\n        stream: bool = False,\n        system_message: Optional[str] = None,\n    ) -> Text:\n        if not openai_api_base:\n            openai_api_base = \"https://api.openai.com/v1\"\n        if openai_api_key:\n            api_key = SecretStr(openai_api_key)\n        else:\n            api_key = None\n\n        output = ChatOpenAI(\n            max_tokens=max_tokens or None,\n            model_kwargs=model_kwargs,\n            model=model_name,\n            base_url=openai_api_base,\n            api_key=api_key,\n            temperature=temperature,\n        )\n\n        return self.get_chat_result(output, stream, input_value, system_message)\n"
                             },
                             "input_value": {
                                 "advanced": false,
                                 "display_name": "Input",
                                 "dynamic": false,
                                 "fileTypes": [],
                                 "file_path": "",
@@ -697,15 +697,15 @@
                             },
                             "max_tokens": {
                                 "advanced": true,
                                 "display_name": "Max Tokens",
                                 "dynamic": false,
                                 "fileTypes": [],
                                 "file_path": "",
-                                "info": "",
+                                "info": "The maximum number of tokens to generate. Set to 0 for unlimited tokens.",
                                 "list": false,
                                 "load_from_db": false,
                                 "multiline": false,
                                 "name": "max_tokens",
                                 "password": false,
                                 "placeholder": "",
                                 "required": false,
@@ -924,15 +924,15 @@
                                 "name": "code",
                                 "password": false,
                                 "placeholder": "",
                                 "required": true,
                                 "show": true,
                                 "title_case": false,
                                 "type": "code",
-                                "value": "from typing import Any, Dict\n\nfrom langchain_community.document_loaders.web_base import WebBaseLoader\n\nfrom langflow.interface.custom.custom_component import CustomComponent\nfrom langflow.schema import Record\n\n\nclass URLComponent(CustomComponent):\n    display_name = \"URL\"\n    description = \"Fetch content from one or more URLs.\"\n    icon = \"layout-template\"\n\n    def build_config(self) -> Dict[str, Any]:\n        return {\n            \"urls\": {\"display_name\": \"URL\"},\n        }\n\n    def build(\n        self,\n        urls: list[str],\n    ) -> list[Record]:\n        loader = WebBaseLoader(web_paths=urls)\n        docs = loader.load()\n        records = self.to_records(docs)\n        self.status = records\n        return records\n"
+                                "value": "from typing import Any, Dict\n\nfrom langchain_community.document_loaders.web_base import WebBaseLoader\n\nfrom langflow.custom import CustomComponent\nfrom langflow.schema import Record\n\n\nclass URLComponent(CustomComponent):\n    display_name = \"URL\"\n    description = \"Fetch content from one or more URLs.\"\n    icon = \"layout-template\"\n\n    def build_config(self) -> Dict[str, Any]:\n        return {\n            \"urls\": {\"display_name\": \"URL\"},\n        }\n\n    def build(\n        self,\n        urls: list[str],\n    ) -> list[Record]:\n        loader = WebBaseLoader(web_paths=urls)\n        docs = loader.load()\n        records = self.to_records(docs)\n        self.status = records\n        return records\n"
                             },
                             "urls": {
                                 "advanced": false,
                                 "display_name": "URL",
                                 "dynamic": false,
                                 "fileTypes": [],
                                 "file_path": "",
```

### Comparing `langflow_base-0.0.48/langflow/initial_setup/starter_projects/Langflow Document QA.json` & `langflow_base-0.0.49/langflow/initial_setup/starter_projects/Langflow Document QA.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999999995705426%*

 * *Differences: {"'data'": "{'nodes': {0: {'data': {'node': {'template': {'code': {'value': 'from "*

 * *           'langchain_core.prompts import PromptTemplate\\n\\nfrom langflow.custom import '*

 * *           'CustomComponent\\nfrom langflow.field_typing import Prompt, TemplateField, '*

 * *           'Text\\n\\n\\nclass PromptComponent(CustomComponent):\\n    display_name: str = '*

 * *           '"Prompt"\\n    description: str = "Create a prompt template with dynamic '*

 * *           'variables."\\n    icon = "prompts"\\n\\n    def build_c […]*

```diff
@@ -228,15 +228,15 @@
                                 "name": "code",
                                 "password": false,
                                 "placeholder": "",
                                 "required": true,
                                 "show": true,
                                 "title_case": false,
                                 "type": "code",
-                                "value": "from langchain_core.prompts import PromptTemplate\n\nfrom langflow.field_typing import Prompt, TemplateField, Text\nfrom langflow.interface.custom.custom_component import CustomComponent\n\n\nclass PromptComponent(CustomComponent):\n    display_name: str = \"Prompt\"\n    description: str = \"Create a prompt template with dynamic variables.\"\n    icon = \"prompts\"\n\n    def build_config(self):\n        return {\n            \"template\": TemplateField(display_name=\"Template\"),\n            \"code\": TemplateField(advanced=True),\n        }\n\n    def build(\n        self,\n        template: Prompt,\n        **kwargs,\n    ) -> Text:\n        from langflow.base.prompts.utils import dict_values_to_string\n\n        prompt_template = PromptTemplate.from_template(Text(template))\n        kwargs = dict_values_to_string(kwargs)\n        kwargs = {k: \"\\n\".join(v) if isinstance(v, list) else v for k, v in kwargs.items()}\n        try:\n            formated_prompt = prompt_template.format(**kwargs)\n        except Exception as exc:\n            raise ValueError(f\"Error formatting prompt: {exc}\") from exc\n        self.status = f'Prompt:\\n\"{formated_prompt}\"'\n        return formated_prompt\n"
+                                "value": "from langchain_core.prompts import PromptTemplate\n\nfrom langflow.custom import CustomComponent\nfrom langflow.field_typing import Prompt, TemplateField, Text\n\n\nclass PromptComponent(CustomComponent):\n    display_name: str = \"Prompt\"\n    description: str = \"Create a prompt template with dynamic variables.\"\n    icon = \"prompts\"\n\n    def build_config(self):\n        return {\n            \"template\": TemplateField(display_name=\"Template\"),\n            \"code\": TemplateField(advanced=True),\n        }\n\n    def build(\n        self,\n        template: Prompt,\n        **kwargs,\n    ) -> Text:\n        from langflow.base.prompts.utils import dict_values_to_string\n\n        prompt_template = PromptTemplate.from_template(Text(template))\n        kwargs = dict_values_to_string(kwargs)\n        kwargs = {k: \"\\n\".join(v) if isinstance(v, list) else v for k, v in kwargs.items()}\n        try:\n            formated_prompt = prompt_template.format(**kwargs)\n        except Exception as exc:\n            raise ValueError(f\"Error formatting prompt: {exc}\") from exc\n        self.status = f'Prompt:\\n\"{formated_prompt}\"'\n        return formated_prompt\n"
                             },
                             "template": {
                                 "advanced": false,
                                 "display_name": "Template",
                                 "dynamic": false,
                                 "fileTypes": [],
                                 "file_path": "",
@@ -793,15 +793,15 @@
                                 "name": "code",
                                 "password": false,
                                 "placeholder": "",
                                 "required": true,
                                 "show": true,
                                 "title_case": false,
                                 "type": "code",
-                                "value": "from typing import Optional\n\nfrom langchain_openai import ChatOpenAI\nfrom pydantic.v1 import SecretStr\n\nfrom langflow.base.constants import STREAM_INFO_TEXT\nfrom langflow.base.models.model import LCModelComponent\nfrom langflow.base.models.openai_constants import MODEL_NAMES\nfrom langflow.field_typing import NestedDict, Text\n\n\nclass OpenAIModelComponent(LCModelComponent):\n    display_name = \"OpenAI\"\n    description = \"Generates text using OpenAI LLMs.\"\n    icon = \"OpenAI\"\n\n    field_order = [\n        \"max_tokens\",\n        \"model_kwargs\",\n        \"model_name\",\n        \"openai_api_base\",\n        \"openai_api_key\",\n        \"temperature\",\n        \"input_value\",\n        \"system_message\",\n        \"stream\",\n    ]\n\n    def build_config(self):\n        return {\n            \"input_value\": {\"display_name\": \"Input\"},\n            \"max_tokens\": {\n                \"display_name\": \"Max Tokens\",\n                \"advanced\": True,\n            },\n            \"model_kwargs\": {\n                \"display_name\": \"Model Kwargs\",\n                \"advanced\": True,\n            },\n            \"model_name\": {\n                \"display_name\": \"Model Name\",\n                \"advanced\": False,\n                \"options\": MODEL_NAMES,\n            },\n            \"openai_api_base\": {\n                \"display_name\": \"OpenAI API Base\",\n                \"advanced\": True,\n                \"info\": (\n                    \"The base URL of the OpenAI API. Defaults to https://api.openai.com/v1.\\n\\n\"\n                    \"You can change this to use other APIs like JinaChat, LocalAI and Prem.\"\n                ),\n            },\n            \"openai_api_key\": {\n                \"display_name\": \"OpenAI API Key\",\n                \"info\": \"The OpenAI API Key to use for the OpenAI model.\",\n                \"advanced\": False,\n                \"password\": True,\n            },\n            \"temperature\": {\n                \"display_name\": \"Temperature\",\n                \"advanced\": False,\n                \"value\": 0.1,\n            },\n            \"stream\": {\n                \"display_name\": \"Stream\",\n                \"info\": STREAM_INFO_TEXT,\n                \"advanced\": True,\n            },\n            \"system_message\": {\n                \"display_name\": \"System Message\",\n                \"info\": \"System message to pass to the model.\",\n                \"advanced\": True,\n            },\n        }\n\n    def build(\n        self,\n        input_value: Text,\n        openai_api_key: str,\n        temperature: float,\n        model_name: str = \"gpt-4o\",\n        max_tokens: Optional[int] = 256,\n        model_kwargs: NestedDict = {},\n        openai_api_base: Optional[str] = None,\n        stream: bool = False,\n        system_message: Optional[str] = None,\n    ) -> Text:\n        if not openai_api_base:\n            openai_api_base = \"https://api.openai.com/v1\"\n        if openai_api_key:\n            api_key = SecretStr(openai_api_key)\n        else:\n            api_key = None\n\n        output = ChatOpenAI(\n            max_tokens=max_tokens,\n            model_kwargs=model_kwargs,\n            model=model_name,\n            base_url=openai_api_base,\n            api_key=api_key,\n            temperature=temperature,\n        )\n\n        return self.get_chat_result(output, stream, input_value, system_message)\n"
+                                "value": "from typing import Optional\n\nfrom langchain_openai import ChatOpenAI\nfrom pydantic.v1 import SecretStr\n\nfrom langflow.base.constants import STREAM_INFO_TEXT\nfrom langflow.base.models.model import LCModelComponent\nfrom langflow.base.models.openai_constants import MODEL_NAMES\nfrom langflow.field_typing import NestedDict, Text\n\n\nclass OpenAIModelComponent(LCModelComponent):\n    display_name = \"OpenAI\"\n    description = \"Generates text using OpenAI LLMs.\"\n    icon = \"OpenAI\"\n\n    field_order = [\n        \"max_tokens\",\n        \"model_kwargs\",\n        \"model_name\",\n        \"openai_api_base\",\n        \"openai_api_key\",\n        \"temperature\",\n        \"input_value\",\n        \"system_message\",\n        \"stream\",\n    ]\n\n    def build_config(self):\n        return {\n            \"input_value\": {\"display_name\": \"Input\"},\n            \"max_tokens\": {\n                \"display_name\": \"Max Tokens\",\n                \"advanced\": True,\n                \"info\": \"The maximum number of tokens to generate. Set to 0 for unlimited tokens.\",\n            },\n            \"model_kwargs\": {\n                \"display_name\": \"Model Kwargs\",\n                \"advanced\": True,\n            },\n            \"model_name\": {\n                \"display_name\": \"Model Name\",\n                \"advanced\": False,\n                \"options\": MODEL_NAMES,\n            },\n            \"openai_api_base\": {\n                \"display_name\": \"OpenAI API Base\",\n                \"advanced\": True,\n                \"info\": (\n                    \"The base URL of the OpenAI API. Defaults to https://api.openai.com/v1.\\n\\n\"\n                    \"You can change this to use other APIs like JinaChat, LocalAI and Prem.\"\n                ),\n            },\n            \"openai_api_key\": {\n                \"display_name\": \"OpenAI API Key\",\n                \"info\": \"The OpenAI API Key to use for the OpenAI model.\",\n                \"advanced\": False,\n                \"password\": True,\n            },\n            \"temperature\": {\n                \"display_name\": \"Temperature\",\n                \"advanced\": False,\n                \"value\": 0.1,\n            },\n            \"stream\": {\n                \"display_name\": \"Stream\",\n                \"info\": STREAM_INFO_TEXT,\n                \"advanced\": True,\n            },\n            \"system_message\": {\n                \"display_name\": \"System Message\",\n                \"info\": \"System message to pass to the model.\",\n                \"advanced\": True,\n            },\n        }\n\n    def build(\n        self,\n        input_value: Text,\n        openai_api_key: str,\n        temperature: float,\n        model_name: str = \"gpt-4o\",\n        max_tokens: Optional[int] = 256,\n        model_kwargs: NestedDict = {},\n        openai_api_base: Optional[str] = None,\n        stream: bool = False,\n        system_message: Optional[str] = None,\n    ) -> Text:\n        if not openai_api_base:\n            openai_api_base = \"https://api.openai.com/v1\"\n        if openai_api_key:\n            api_key = SecretStr(openai_api_key)\n        else:\n            api_key = None\n\n        output = ChatOpenAI(\n            max_tokens=max_tokens or None,\n            model_kwargs=model_kwargs,\n            model=model_name,\n            base_url=openai_api_base,\n            api_key=api_key,\n            temperature=temperature,\n        )\n\n        return self.get_chat_result(output, stream, input_value, system_message)\n"
                             },
                             "input_value": {
                                 "advanced": false,
                                 "display_name": "Input",
                                 "dynamic": false,
                                 "fileTypes": [],
                                 "file_path": "",
@@ -822,15 +822,15 @@
                             },
                             "max_tokens": {
                                 "advanced": true,
                                 "display_name": "Max Tokens",
                                 "dynamic": false,
                                 "fileTypes": [],
                                 "file_path": "",
-                                "info": "",
+                                "info": "The maximum number of tokens to generate. Set to 0 for unlimited tokens.",
                                 "list": false,
                                 "load_from_db": false,
                                 "multiline": false,
                                 "name": "max_tokens",
                                 "password": false,
                                 "placeholder": "",
                                 "required": false,
```

### Comparing `langflow_base-0.0.48/langflow/initial_setup/starter_projects/Langflow Memory Conversation.json` & `langflow_base-0.0.49/langflow/initial_setup/starter_projects/Langflow Memory Conversation.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999999973158912%*

 * *Differences: {"'data'": "{'nodes': {3: {'data': {'node': {'template': {'code': {'value': 'from "*

 * *           'langchain_core.prompts import PromptTemplate\\n\\nfrom langflow.custom import '*

 * *           'CustomComponent\\nfrom langflow.field_typing import Prompt, TemplateField, '*

 * *           'Text\\n\\n\\nclass PromptComponent(CustomComponent):\\n    display_name: str = '*

 * *           '"Prompt"\\n    description: str = "Create a prompt template with dynamic '*

 * *           'variables."\\n    icon = "prompts"\\n\\n    def build_c […]*

```diff
@@ -772,15 +772,15 @@
                                 "name": "code",
                                 "password": false,
                                 "placeholder": "",
                                 "required": true,
                                 "show": true,
                                 "title_case": false,
                                 "type": "code",
-                                "value": "from langchain_core.prompts import PromptTemplate\n\nfrom langflow.field_typing import Prompt, TemplateField, Text\nfrom langflow.interface.custom.custom_component import CustomComponent\n\n\nclass PromptComponent(CustomComponent):\n    display_name: str = \"Prompt\"\n    description: str = \"Create a prompt template with dynamic variables.\"\n    icon = \"prompts\"\n\n    def build_config(self):\n        return {\n            \"template\": TemplateField(display_name=\"Template\"),\n            \"code\": TemplateField(advanced=True),\n        }\n\n    def build(\n        self,\n        template: Prompt,\n        **kwargs,\n    ) -> Text:\n        from langflow.base.prompts.utils import dict_values_to_string\n\n        prompt_template = PromptTemplate.from_template(Text(template))\n        kwargs = dict_values_to_string(kwargs)\n        kwargs = {k: \"\\n\".join(v) if isinstance(v, list) else v for k, v in kwargs.items()}\n        try:\n            formated_prompt = prompt_template.format(**kwargs)\n        except Exception as exc:\n            raise ValueError(f\"Error formatting prompt: {exc}\") from exc\n        self.status = f'Prompt:\\n\"{formated_prompt}\"'\n        return formated_prompt\n"
+                                "value": "from langchain_core.prompts import PromptTemplate\n\nfrom langflow.custom import CustomComponent\nfrom langflow.field_typing import Prompt, TemplateField, Text\n\n\nclass PromptComponent(CustomComponent):\n    display_name: str = \"Prompt\"\n    description: str = \"Create a prompt template with dynamic variables.\"\n    icon = \"prompts\"\n\n    def build_config(self):\n        return {\n            \"template\": TemplateField(display_name=\"Template\"),\n            \"code\": TemplateField(advanced=True),\n        }\n\n    def build(\n        self,\n        template: Prompt,\n        **kwargs,\n    ) -> Text:\n        from langflow.base.prompts.utils import dict_values_to_string\n\n        prompt_template = PromptTemplate.from_template(Text(template))\n        kwargs = dict_values_to_string(kwargs)\n        kwargs = {k: \"\\n\".join(v) if isinstance(v, list) else v for k, v in kwargs.items()}\n        try:\n            formated_prompt = prompt_template.format(**kwargs)\n        except Exception as exc:\n            raise ValueError(f\"Error formatting prompt: {exc}\") from exc\n        self.status = f'Prompt:\\n\"{formated_prompt}\"'\n        return formated_prompt\n"
                             },
                             "context": {
                                 "advanced": false,
                                 "display_name": "context",
                                 "dynamic": false,
                                 "field_type": "str",
                                 "fileTypes": [],
@@ -926,15 +926,15 @@
                                 "name": "code",
                                 "password": false,
                                 "placeholder": "",
                                 "required": true,
                                 "show": true,
                                 "title_case": false,
                                 "type": "code",
-                                "value": "from typing import Optional\n\nfrom langchain_openai import ChatOpenAI\nfrom pydantic.v1 import SecretStr\n\nfrom langflow.base.constants import STREAM_INFO_TEXT\nfrom langflow.base.models.model import LCModelComponent\nfrom langflow.base.models.openai_constants import MODEL_NAMES\nfrom langflow.field_typing import NestedDict, Text\n\n\nclass OpenAIModelComponent(LCModelComponent):\n    display_name = \"OpenAI\"\n    description = \"Generates text using OpenAI LLMs.\"\n    icon = \"OpenAI\"\n\n    field_order = [\n        \"max_tokens\",\n        \"model_kwargs\",\n        \"model_name\",\n        \"openai_api_base\",\n        \"openai_api_key\",\n        \"temperature\",\n        \"input_value\",\n        \"system_message\",\n        \"stream\",\n    ]\n\n    def build_config(self):\n        return {\n            \"input_value\": {\"display_name\": \"Input\"},\n            \"max_tokens\": {\n                \"display_name\": \"Max Tokens\",\n                \"advanced\": True,\n            },\n            \"model_kwargs\": {\n                \"display_name\": \"Model Kwargs\",\n                \"advanced\": True,\n            },\n            \"model_name\": {\n                \"display_name\": \"Model Name\",\n                \"advanced\": False,\n                \"options\": MODEL_NAMES,\n            },\n            \"openai_api_base\": {\n                \"display_name\": \"OpenAI API Base\",\n                \"advanced\": True,\n                \"info\": (\n                    \"The base URL of the OpenAI API. Defaults to https://api.openai.com/v1.\\n\\n\"\n                    \"You can change this to use other APIs like JinaChat, LocalAI and Prem.\"\n                ),\n            },\n            \"openai_api_key\": {\n                \"display_name\": \"OpenAI API Key\",\n                \"info\": \"The OpenAI API Key to use for the OpenAI model.\",\n                \"advanced\": False,\n                \"password\": True,\n            },\n            \"temperature\": {\n                \"display_name\": \"Temperature\",\n                \"advanced\": False,\n                \"value\": 0.1,\n            },\n            \"stream\": {\n                \"display_name\": \"Stream\",\n                \"info\": STREAM_INFO_TEXT,\n                \"advanced\": True,\n            },\n            \"system_message\": {\n                \"display_name\": \"System Message\",\n                \"info\": \"System message to pass to the model.\",\n                \"advanced\": True,\n            },\n        }\n\n    def build(\n        self,\n        input_value: Text,\n        openai_api_key: str,\n        temperature: float,\n        model_name: str = \"gpt-4o\",\n        max_tokens: Optional[int] = 256,\n        model_kwargs: NestedDict = {},\n        openai_api_base: Optional[str] = None,\n        stream: bool = False,\n        system_message: Optional[str] = None,\n    ) -> Text:\n        if not openai_api_base:\n            openai_api_base = \"https://api.openai.com/v1\"\n        if openai_api_key:\n            api_key = SecretStr(openai_api_key)\n        else:\n            api_key = None\n\n        output = ChatOpenAI(\n            max_tokens=max_tokens,\n            model_kwargs=model_kwargs,\n            model=model_name,\n            base_url=openai_api_base,\n            api_key=api_key,\n            temperature=temperature,\n        )\n\n        return self.get_chat_result(output, stream, input_value, system_message)\n"
+                                "value": "from typing import Optional\n\nfrom langchain_openai import ChatOpenAI\nfrom pydantic.v1 import SecretStr\n\nfrom langflow.base.constants import STREAM_INFO_TEXT\nfrom langflow.base.models.model import LCModelComponent\nfrom langflow.base.models.openai_constants import MODEL_NAMES\nfrom langflow.field_typing import NestedDict, Text\n\n\nclass OpenAIModelComponent(LCModelComponent):\n    display_name = \"OpenAI\"\n    description = \"Generates text using OpenAI LLMs.\"\n    icon = \"OpenAI\"\n\n    field_order = [\n        \"max_tokens\",\n        \"model_kwargs\",\n        \"model_name\",\n        \"openai_api_base\",\n        \"openai_api_key\",\n        \"temperature\",\n        \"input_value\",\n        \"system_message\",\n        \"stream\",\n    ]\n\n    def build_config(self):\n        return {\n            \"input_value\": {\"display_name\": \"Input\"},\n            \"max_tokens\": {\n                \"display_name\": \"Max Tokens\",\n                \"advanced\": True,\n                \"info\": \"The maximum number of tokens to generate. Set to 0 for unlimited tokens.\",\n            },\n            \"model_kwargs\": {\n                \"display_name\": \"Model Kwargs\",\n                \"advanced\": True,\n            },\n            \"model_name\": {\n                \"display_name\": \"Model Name\",\n                \"advanced\": False,\n                \"options\": MODEL_NAMES,\n            },\n            \"openai_api_base\": {\n                \"display_name\": \"OpenAI API Base\",\n                \"advanced\": True,\n                \"info\": (\n                    \"The base URL of the OpenAI API. Defaults to https://api.openai.com/v1.\\n\\n\"\n                    \"You can change this to use other APIs like JinaChat, LocalAI and Prem.\"\n                ),\n            },\n            \"openai_api_key\": {\n                \"display_name\": \"OpenAI API Key\",\n                \"info\": \"The OpenAI API Key to use for the OpenAI model.\",\n                \"advanced\": False,\n                \"password\": True,\n            },\n            \"temperature\": {\n                \"display_name\": \"Temperature\",\n                \"advanced\": False,\n                \"value\": 0.1,\n            },\n            \"stream\": {\n                \"display_name\": \"Stream\",\n                \"info\": STREAM_INFO_TEXT,\n                \"advanced\": True,\n            },\n            \"system_message\": {\n                \"display_name\": \"System Message\",\n                \"info\": \"System message to pass to the model.\",\n                \"advanced\": True,\n            },\n        }\n\n    def build(\n        self,\n        input_value: Text,\n        openai_api_key: str,\n        temperature: float,\n        model_name: str = \"gpt-4o\",\n        max_tokens: Optional[int] = 256,\n        model_kwargs: NestedDict = {},\n        openai_api_base: Optional[str] = None,\n        stream: bool = False,\n        system_message: Optional[str] = None,\n    ) -> Text:\n        if not openai_api_base:\n            openai_api_base = \"https://api.openai.com/v1\"\n        if openai_api_key:\n            api_key = SecretStr(openai_api_key)\n        else:\n            api_key = None\n\n        output = ChatOpenAI(\n            max_tokens=max_tokens or None,\n            model_kwargs=model_kwargs,\n            model=model_name,\n            base_url=openai_api_base,\n            api_key=api_key,\n            temperature=temperature,\n        )\n\n        return self.get_chat_result(output, stream, input_value, system_message)\n"
                             },
                             "input_value": {
                                 "advanced": false,
                                 "display_name": "Input",
                                 "dynamic": false,
                                 "fileTypes": [],
                                 "file_path": "",
@@ -955,15 +955,15 @@
                             },
                             "max_tokens": {
                                 "advanced": true,
                                 "display_name": "Max Tokens",
                                 "dynamic": false,
                                 "fileTypes": [],
                                 "file_path": "",
-                                "info": "",
+                                "info": "The maximum number of tokens to generate. Set to 0 for unlimited tokens.",
                                 "list": false,
                                 "load_from_db": false,
                                 "multiline": false,
                                 "name": "max_tokens",
                                 "password": false,
                                 "placeholder": "",
                                 "required": false,
```

### Comparing `langflow_base-0.0.48/langflow/initial_setup/starter_projects/Langflow Prompt Chaining.json` & `langflow_base-0.0.49/langflow/initial_setup/starter_projects/Langflow Prompt Chaining.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999999947398582%*

 * *Differences: {"'data'": "{'nodes': {0: {'data': {'node': {'template': {'code': {'value': 'from "*

 * *           'langchain_core.prompts import PromptTemplate\\n\\nfrom langflow.custom import '*

 * *           'CustomComponent\\nfrom langflow.field_typing import Prompt, TemplateField, '*

 * *           'Text\\n\\n\\nclass PromptComponent(CustomComponent):\\n    display_name: str = '*

 * *           '"Prompt"\\n    description: str = "Create a prompt template with dynamic '*

 * *           'variables."\\n    icon = "prompts"\\n\\n    def build_c […]*

```diff
@@ -298,15 +298,15 @@
                                 "name": "code",
                                 "password": false,
                                 "placeholder": "",
                                 "required": true,
                                 "show": true,
                                 "title_case": false,
                                 "type": "code",
-                                "value": "from langchain_core.prompts import PromptTemplate\n\nfrom langflow.field_typing import Prompt, TemplateField, Text\nfrom langflow.interface.custom.custom_component import CustomComponent\n\n\nclass PromptComponent(CustomComponent):\n    display_name: str = \"Prompt\"\n    description: str = \"Create a prompt template with dynamic variables.\"\n    icon = \"prompts\"\n\n    def build_config(self):\n        return {\n            \"template\": TemplateField(display_name=\"Template\"),\n            \"code\": TemplateField(advanced=True),\n        }\n\n    def build(\n        self,\n        template: Prompt,\n        **kwargs,\n    ) -> Text:\n        from langflow.base.prompts.utils import dict_values_to_string\n\n        prompt_template = PromptTemplate.from_template(Text(template))\n        kwargs = dict_values_to_string(kwargs)\n        kwargs = {k: \"\\n\".join(v) if isinstance(v, list) else v for k, v in kwargs.items()}\n        try:\n            formated_prompt = prompt_template.format(**kwargs)\n        except Exception as exc:\n            raise ValueError(f\"Error formatting prompt: {exc}\") from exc\n        self.status = f'Prompt:\\n\"{formated_prompt}\"'\n        return formated_prompt\n"
+                                "value": "from langchain_core.prompts import PromptTemplate\n\nfrom langflow.custom import CustomComponent\nfrom langflow.field_typing import Prompt, TemplateField, Text\n\n\nclass PromptComponent(CustomComponent):\n    display_name: str = \"Prompt\"\n    description: str = \"Create a prompt template with dynamic variables.\"\n    icon = \"prompts\"\n\n    def build_config(self):\n        return {\n            \"template\": TemplateField(display_name=\"Template\"),\n            \"code\": TemplateField(advanced=True),\n        }\n\n    def build(\n        self,\n        template: Prompt,\n        **kwargs,\n    ) -> Text:\n        from langflow.base.prompts.utils import dict_values_to_string\n\n        prompt_template = PromptTemplate.from_template(Text(template))\n        kwargs = dict_values_to_string(kwargs)\n        kwargs = {k: \"\\n\".join(v) if isinstance(v, list) else v for k, v in kwargs.items()}\n        try:\n            formated_prompt = prompt_template.format(**kwargs)\n        except Exception as exc:\n            raise ValueError(f\"Error formatting prompt: {exc}\") from exc\n        self.status = f'Prompt:\\n\"{formated_prompt}\"'\n        return formated_prompt\n"
                             },
                             "document": {
                                 "advanced": false,
                                 "display_name": "document",
                                 "dynamic": false,
                                 "field_type": "str",
                                 "fileTypes": [],
@@ -418,15 +418,15 @@
                                 "name": "code",
                                 "password": false,
                                 "placeholder": "",
                                 "required": true,
                                 "show": true,
                                 "title_case": false,
                                 "type": "code",
-                                "value": "from langchain_core.prompts import PromptTemplate\n\nfrom langflow.field_typing import Prompt, TemplateField, Text\nfrom langflow.interface.custom.custom_component import CustomComponent\n\n\nclass PromptComponent(CustomComponent):\n    display_name: str = \"Prompt\"\n    description: str = \"Create a prompt template with dynamic variables.\"\n    icon = \"prompts\"\n\n    def build_config(self):\n        return {\n            \"template\": TemplateField(display_name=\"Template\"),\n            \"code\": TemplateField(advanced=True),\n        }\n\n    def build(\n        self,\n        template: Prompt,\n        **kwargs,\n    ) -> Text:\n        from langflow.base.prompts.utils import dict_values_to_string\n\n        prompt_template = PromptTemplate.from_template(Text(template))\n        kwargs = dict_values_to_string(kwargs)\n        kwargs = {k: \"\\n\".join(v) if isinstance(v, list) else v for k, v in kwargs.items()}\n        try:\n            formated_prompt = prompt_template.format(**kwargs)\n        except Exception as exc:\n            raise ValueError(f\"Error formatting prompt: {exc}\") from exc\n        self.status = f'Prompt:\\n\"{formated_prompt}\"'\n        return formated_prompt\n"
+                                "value": "from langchain_core.prompts import PromptTemplate\n\nfrom langflow.custom import CustomComponent\nfrom langflow.field_typing import Prompt, TemplateField, Text\n\n\nclass PromptComponent(CustomComponent):\n    display_name: str = \"Prompt\"\n    description: str = \"Create a prompt template with dynamic variables.\"\n    icon = \"prompts\"\n\n    def build_config(self):\n        return {\n            \"template\": TemplateField(display_name=\"Template\"),\n            \"code\": TemplateField(advanced=True),\n        }\n\n    def build(\n        self,\n        template: Prompt,\n        **kwargs,\n    ) -> Text:\n        from langflow.base.prompts.utils import dict_values_to_string\n\n        prompt_template = PromptTemplate.from_template(Text(template))\n        kwargs = dict_values_to_string(kwargs)\n        kwargs = {k: \"\\n\".join(v) if isinstance(v, list) else v for k, v in kwargs.items()}\n        try:\n            formated_prompt = prompt_template.format(**kwargs)\n        except Exception as exc:\n            raise ValueError(f\"Error formatting prompt: {exc}\") from exc\n        self.status = f'Prompt:\\n\"{formated_prompt}\"'\n        return formated_prompt\n"
                             },
                             "summary": {
                                 "advanced": false,
                                 "display_name": "summary",
                                 "dynamic": false,
                                 "field_type": "str",
                                 "fileTypes": [],
@@ -1149,15 +1149,15 @@
                                 "name": "code",
                                 "password": false,
                                 "placeholder": "",
                                 "required": true,
                                 "show": true,
                                 "title_case": false,
                                 "type": "code",
-                                "value": "from typing import Optional\n\nfrom langchain_openai import ChatOpenAI\nfrom pydantic.v1 import SecretStr\n\nfrom langflow.base.constants import STREAM_INFO_TEXT\nfrom langflow.base.models.model import LCModelComponent\nfrom langflow.base.models.openai_constants import MODEL_NAMES\nfrom langflow.field_typing import NestedDict, Text\n\n\nclass OpenAIModelComponent(LCModelComponent):\n    display_name = \"OpenAI\"\n    description = \"Generates text using OpenAI LLMs.\"\n    icon = \"OpenAI\"\n\n    field_order = [\n        \"max_tokens\",\n        \"model_kwargs\",\n        \"model_name\",\n        \"openai_api_base\",\n        \"openai_api_key\",\n        \"temperature\",\n        \"input_value\",\n        \"system_message\",\n        \"stream\",\n    ]\n\n    def build_config(self):\n        return {\n            \"input_value\": {\"display_name\": \"Input\"},\n            \"max_tokens\": {\n                \"display_name\": \"Max Tokens\",\n                \"advanced\": True,\n            },\n            \"model_kwargs\": {\n                \"display_name\": \"Model Kwargs\",\n                \"advanced\": True,\n            },\n            \"model_name\": {\n                \"display_name\": \"Model Name\",\n                \"advanced\": False,\n                \"options\": MODEL_NAMES,\n            },\n            \"openai_api_base\": {\n                \"display_name\": \"OpenAI API Base\",\n                \"advanced\": True,\n                \"info\": (\n                    \"The base URL of the OpenAI API. Defaults to https://api.openai.com/v1.\\n\\n\"\n                    \"You can change this to use other APIs like JinaChat, LocalAI and Prem.\"\n                ),\n            },\n            \"openai_api_key\": {\n                \"display_name\": \"OpenAI API Key\",\n                \"info\": \"The OpenAI API Key to use for the OpenAI model.\",\n                \"advanced\": False,\n                \"password\": True,\n            },\n            \"temperature\": {\n                \"display_name\": \"Temperature\",\n                \"advanced\": False,\n                \"value\": 0.1,\n            },\n            \"stream\": {\n                \"display_name\": \"Stream\",\n                \"info\": STREAM_INFO_TEXT,\n                \"advanced\": True,\n            },\n            \"system_message\": {\n                \"display_name\": \"System Message\",\n                \"info\": \"System message to pass to the model.\",\n                \"advanced\": True,\n            },\n        }\n\n    def build(\n        self,\n        input_value: Text,\n        openai_api_key: str,\n        temperature: float,\n        model_name: str = \"gpt-4o\",\n        max_tokens: Optional[int] = 256,\n        model_kwargs: NestedDict = {},\n        openai_api_base: Optional[str] = None,\n        stream: bool = False,\n        system_message: Optional[str] = None,\n    ) -> Text:\n        if not openai_api_base:\n            openai_api_base = \"https://api.openai.com/v1\"\n        if openai_api_key:\n            api_key = SecretStr(openai_api_key)\n        else:\n            api_key = None\n\n        output = ChatOpenAI(\n            max_tokens=max_tokens,\n            model_kwargs=model_kwargs,\n            model=model_name,\n            base_url=openai_api_base,\n            api_key=api_key,\n            temperature=temperature,\n        )\n\n        return self.get_chat_result(output, stream, input_value, system_message)\n"
+                                "value": "from typing import Optional\n\nfrom langchain_openai import ChatOpenAI\nfrom pydantic.v1 import SecretStr\n\nfrom langflow.base.constants import STREAM_INFO_TEXT\nfrom langflow.base.models.model import LCModelComponent\nfrom langflow.base.models.openai_constants import MODEL_NAMES\nfrom langflow.field_typing import NestedDict, Text\n\n\nclass OpenAIModelComponent(LCModelComponent):\n    display_name = \"OpenAI\"\n    description = \"Generates text using OpenAI LLMs.\"\n    icon = \"OpenAI\"\n\n    field_order = [\n        \"max_tokens\",\n        \"model_kwargs\",\n        \"model_name\",\n        \"openai_api_base\",\n        \"openai_api_key\",\n        \"temperature\",\n        \"input_value\",\n        \"system_message\",\n        \"stream\",\n    ]\n\n    def build_config(self):\n        return {\n            \"input_value\": {\"display_name\": \"Input\"},\n            \"max_tokens\": {\n                \"display_name\": \"Max Tokens\",\n                \"advanced\": True,\n                \"info\": \"The maximum number of tokens to generate. Set to 0 for unlimited tokens.\",\n            },\n            \"model_kwargs\": {\n                \"display_name\": \"Model Kwargs\",\n                \"advanced\": True,\n            },\n            \"model_name\": {\n                \"display_name\": \"Model Name\",\n                \"advanced\": False,\n                \"options\": MODEL_NAMES,\n            },\n            \"openai_api_base\": {\n                \"display_name\": \"OpenAI API Base\",\n                \"advanced\": True,\n                \"info\": (\n                    \"The base URL of the OpenAI API. Defaults to https://api.openai.com/v1.\\n\\n\"\n                    \"You can change this to use other APIs like JinaChat, LocalAI and Prem.\"\n                ),\n            },\n            \"openai_api_key\": {\n                \"display_name\": \"OpenAI API Key\",\n                \"info\": \"The OpenAI API Key to use for the OpenAI model.\",\n                \"advanced\": False,\n                \"password\": True,\n            },\n            \"temperature\": {\n                \"display_name\": \"Temperature\",\n                \"advanced\": False,\n                \"value\": 0.1,\n            },\n            \"stream\": {\n                \"display_name\": \"Stream\",\n                \"info\": STREAM_INFO_TEXT,\n                \"advanced\": True,\n            },\n            \"system_message\": {\n                \"display_name\": \"System Message\",\n                \"info\": \"System message to pass to the model.\",\n                \"advanced\": True,\n            },\n        }\n\n    def build(\n        self,\n        input_value: Text,\n        openai_api_key: str,\n        temperature: float,\n        model_name: str = \"gpt-4o\",\n        max_tokens: Optional[int] = 256,\n        model_kwargs: NestedDict = {},\n        openai_api_base: Optional[str] = None,\n        stream: bool = False,\n        system_message: Optional[str] = None,\n    ) -> Text:\n        if not openai_api_base:\n            openai_api_base = \"https://api.openai.com/v1\"\n        if openai_api_key:\n            api_key = SecretStr(openai_api_key)\n        else:\n            api_key = None\n\n        output = ChatOpenAI(\n            max_tokens=max_tokens or None,\n            model_kwargs=model_kwargs,\n            model=model_name,\n            base_url=openai_api_base,\n            api_key=api_key,\n            temperature=temperature,\n        )\n\n        return self.get_chat_result(output, stream, input_value, system_message)\n"
                             },
                             "input_value": {
                                 "advanced": false,
                                 "display_name": "Input",
                                 "dynamic": false,
                                 "fileTypes": [],
                                 "file_path": "",
@@ -1178,15 +1178,15 @@
                             },
                             "max_tokens": {
                                 "advanced": true,
                                 "display_name": "Max Tokens",
                                 "dynamic": false,
                                 "fileTypes": [],
                                 "file_path": "",
-                                "info": "",
+                                "info": "The maximum number of tokens to generate. Set to 0 for unlimited tokens.",
                                 "list": false,
                                 "load_from_db": false,
                                 "multiline": false,
                                 "name": "max_tokens",
                                 "password": false,
                                 "placeholder": "",
                                 "required": false,
@@ -1533,15 +1533,15 @@
                                 "name": "code",
                                 "password": false,
                                 "placeholder": "",
                                 "required": true,
                                 "show": true,
                                 "title_case": false,
                                 "type": "code",
-                                "value": "from typing import Optional\n\nfrom langchain_openai import ChatOpenAI\nfrom pydantic.v1 import SecretStr\n\nfrom langflow.base.constants import STREAM_INFO_TEXT\nfrom langflow.base.models.model import LCModelComponent\nfrom langflow.base.models.openai_constants import MODEL_NAMES\nfrom langflow.field_typing import NestedDict, Text\n\n\nclass OpenAIModelComponent(LCModelComponent):\n    display_name = \"OpenAI\"\n    description = \"Generates text using OpenAI LLMs.\"\n    icon = \"OpenAI\"\n\n    field_order = [\n        \"max_tokens\",\n        \"model_kwargs\",\n        \"model_name\",\n        \"openai_api_base\",\n        \"openai_api_key\",\n        \"temperature\",\n        \"input_value\",\n        \"system_message\",\n        \"stream\",\n    ]\n\n    def build_config(self):\n        return {\n            \"input_value\": {\"display_name\": \"Input\"},\n            \"max_tokens\": {\n                \"display_name\": \"Max Tokens\",\n                \"advanced\": True,\n            },\n            \"model_kwargs\": {\n                \"display_name\": \"Model Kwargs\",\n                \"advanced\": True,\n            },\n            \"model_name\": {\n                \"display_name\": \"Model Name\",\n                \"advanced\": False,\n                \"options\": MODEL_NAMES,\n            },\n            \"openai_api_base\": {\n                \"display_name\": \"OpenAI API Base\",\n                \"advanced\": True,\n                \"info\": (\n                    \"The base URL of the OpenAI API. Defaults to https://api.openai.com/v1.\\n\\n\"\n                    \"You can change this to use other APIs like JinaChat, LocalAI and Prem.\"\n                ),\n            },\n            \"openai_api_key\": {\n                \"display_name\": \"OpenAI API Key\",\n                \"info\": \"The OpenAI API Key to use for the OpenAI model.\",\n                \"advanced\": False,\n                \"password\": True,\n            },\n            \"temperature\": {\n                \"display_name\": \"Temperature\",\n                \"advanced\": False,\n                \"value\": 0.1,\n            },\n            \"stream\": {\n                \"display_name\": \"Stream\",\n                \"info\": STREAM_INFO_TEXT,\n                \"advanced\": True,\n            },\n            \"system_message\": {\n                \"display_name\": \"System Message\",\n                \"info\": \"System message to pass to the model.\",\n                \"advanced\": True,\n            },\n        }\n\n    def build(\n        self,\n        input_value: Text,\n        openai_api_key: str,\n        temperature: float,\n        model_name: str = \"gpt-4o\",\n        max_tokens: Optional[int] = 256,\n        model_kwargs: NestedDict = {},\n        openai_api_base: Optional[str] = None,\n        stream: bool = False,\n        system_message: Optional[str] = None,\n    ) -> Text:\n        if not openai_api_base:\n            openai_api_base = \"https://api.openai.com/v1\"\n        if openai_api_key:\n            api_key = SecretStr(openai_api_key)\n        else:\n            api_key = None\n\n        output = ChatOpenAI(\n            max_tokens=max_tokens,\n            model_kwargs=model_kwargs,\n            model=model_name,\n            base_url=openai_api_base,\n            api_key=api_key,\n            temperature=temperature,\n        )\n\n        return self.get_chat_result(output, stream, input_value, system_message)\n"
+                                "value": "from typing import Optional\n\nfrom langchain_openai import ChatOpenAI\nfrom pydantic.v1 import SecretStr\n\nfrom langflow.base.constants import STREAM_INFO_TEXT\nfrom langflow.base.models.model import LCModelComponent\nfrom langflow.base.models.openai_constants import MODEL_NAMES\nfrom langflow.field_typing import NestedDict, Text\n\n\nclass OpenAIModelComponent(LCModelComponent):\n    display_name = \"OpenAI\"\n    description = \"Generates text using OpenAI LLMs.\"\n    icon = \"OpenAI\"\n\n    field_order = [\n        \"max_tokens\",\n        \"model_kwargs\",\n        \"model_name\",\n        \"openai_api_base\",\n        \"openai_api_key\",\n        \"temperature\",\n        \"input_value\",\n        \"system_message\",\n        \"stream\",\n    ]\n\n    def build_config(self):\n        return {\n            \"input_value\": {\"display_name\": \"Input\"},\n            \"max_tokens\": {\n                \"display_name\": \"Max Tokens\",\n                \"advanced\": True,\n                \"info\": \"The maximum number of tokens to generate. Set to 0 for unlimited tokens.\",\n            },\n            \"model_kwargs\": {\n                \"display_name\": \"Model Kwargs\",\n                \"advanced\": True,\n            },\n            \"model_name\": {\n                \"display_name\": \"Model Name\",\n                \"advanced\": False,\n                \"options\": MODEL_NAMES,\n            },\n            \"openai_api_base\": {\n                \"display_name\": \"OpenAI API Base\",\n                \"advanced\": True,\n                \"info\": (\n                    \"The base URL of the OpenAI API. Defaults to https://api.openai.com/v1.\\n\\n\"\n                    \"You can change this to use other APIs like JinaChat, LocalAI and Prem.\"\n                ),\n            },\n            \"openai_api_key\": {\n                \"display_name\": \"OpenAI API Key\",\n                \"info\": \"The OpenAI API Key to use for the OpenAI model.\",\n                \"advanced\": False,\n                \"password\": True,\n            },\n            \"temperature\": {\n                \"display_name\": \"Temperature\",\n                \"advanced\": False,\n                \"value\": 0.1,\n            },\n            \"stream\": {\n                \"display_name\": \"Stream\",\n                \"info\": STREAM_INFO_TEXT,\n                \"advanced\": True,\n            },\n            \"system_message\": {\n                \"display_name\": \"System Message\",\n                \"info\": \"System message to pass to the model.\",\n                \"advanced\": True,\n            },\n        }\n\n    def build(\n        self,\n        input_value: Text,\n        openai_api_key: str,\n        temperature: float,\n        model_name: str = \"gpt-4o\",\n        max_tokens: Optional[int] = 256,\n        model_kwargs: NestedDict = {},\n        openai_api_base: Optional[str] = None,\n        stream: bool = False,\n        system_message: Optional[str] = None,\n    ) -> Text:\n        if not openai_api_base:\n            openai_api_base = \"https://api.openai.com/v1\"\n        if openai_api_key:\n            api_key = SecretStr(openai_api_key)\n        else:\n            api_key = None\n\n        output = ChatOpenAI(\n            max_tokens=max_tokens or None,\n            model_kwargs=model_kwargs,\n            model=model_name,\n            base_url=openai_api_base,\n            api_key=api_key,\n            temperature=temperature,\n        )\n\n        return self.get_chat_result(output, stream, input_value, system_message)\n"
                             },
                             "input_value": {
                                 "advanced": false,
                                 "display_name": "Input",
                                 "dynamic": false,
                                 "fileTypes": [],
                                 "file_path": "",
@@ -1562,15 +1562,15 @@
                             },
                             "max_tokens": {
                                 "advanced": true,
                                 "display_name": "Max Tokens",
                                 "dynamic": false,
                                 "fileTypes": [],
                                 "file_path": "",
-                                "info": "",
+                                "info": "The maximum number of tokens to generate. Set to 0 for unlimited tokens.",
                                 "list": false,
                                 "load_from_db": false,
                                 "multiline": false,
                                 "name": "max_tokens",
                                 "password": false,
                                 "placeholder": "",
                                 "required": false,
```

### Comparing `langflow_base-0.0.48/langflow/initial_setup/starter_projects/VectorStore-RAG-Flows.json` & `langflow_base-0.0.49/langflow/initial_setup/starter_projects/VectorStore-RAG-Flows.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999999940260315%*

 * *Differences: {"'data'": "{'nodes': {2: {'data': {'node': {'template': {'code': {'value': 'from typing import "*

 * *           'Dict, List, Optional\\n\\nfrom langchain_openai.embeddings.base import '*

 * *           'OpenAIEmbeddings\\nfrom pydantic.v1 import SecretStr\\n\\nfrom langflow.custom import '*

 * *           'CustomComponent\\nfrom langflow.field_typing import Embeddings, '*

 * *           'NestedDict\\n\\n\\nclass OpenAIEmbeddingsComponent(CustomComponent):\\n    '*

 * *           'display_name = "OpenAI Embeddings"\\n    descripti […]*

```diff
@@ -697,15 +697,15 @@
                                 "name": "code",
                                 "password": false,
                                 "placeholder": "",
                                 "required": true,
                                 "show": true,
                                 "title_case": false,
                                 "type": "code",
-                                "value": "from typing import Any, Dict, List, Optional\n\nfrom langchain_openai.embeddings.base import OpenAIEmbeddings\nfrom pydantic.v1 import SecretStr\n\nfrom langflow.field_typing import Embeddings, NestedDict\nfrom langflow.interface.custom.custom_component import CustomComponent\n\n\nclass OpenAIEmbeddingsComponent(CustomComponent):\n    display_name = \"OpenAI Embeddings\"\n    description = \"Generate embeddings using OpenAI models.\"\n\n    def build_config(self):\n        return {\n            \"allowed_special\": {\n                \"display_name\": \"Allowed Special\",\n                \"advanced\": True,\n                \"field_type\": \"str\",\n                \"is_list\": True,\n            },\n            \"default_headers\": {\n                \"display_name\": \"Default Headers\",\n                \"advanced\": True,\n                \"field_type\": \"dict\",\n            },\n            \"default_query\": {\n                \"display_name\": \"Default Query\",\n                \"advanced\": True,\n                \"field_type\": \"NestedDict\",\n            },\n            \"disallowed_special\": {\n                \"display_name\": \"Disallowed Special\",\n                \"advanced\": True,\n                \"field_type\": \"str\",\n                \"is_list\": True,\n            },\n            \"chunk_size\": {\"display_name\": \"Chunk Size\", \"advanced\": True},\n            \"client\": {\"display_name\": \"Client\", \"advanced\": True},\n            \"deployment\": {\"display_name\": \"Deployment\", \"advanced\": True},\n            \"embedding_ctx_length\": {\n                \"display_name\": \"Embedding Context Length\",\n                \"advanced\": True,\n            },\n            \"max_retries\": {\"display_name\": \"Max Retries\", \"advanced\": True},\n            \"model\": {\n                \"display_name\": \"Model\",\n                \"advanced\": False,\n                \"options\": [\n                    \"text-embedding-3-small\",\n                    \"text-embedding-3-large\",\n                    \"text-embedding-ada-002\",\n                ],\n            },\n            \"model_kwargs\": {\"display_name\": \"Model Kwargs\", \"advanced\": True},\n            \"openai_api_base\": {\n                \"display_name\": \"OpenAI API Base\",\n                \"password\": True,\n                \"advanced\": True,\n            },\n            \"openai_api_key\": {\"display_name\": \"OpenAI API Key\", \"password\": True},\n            \"openai_api_type\": {\n                \"display_name\": \"OpenAI API Type\",\n                \"advanced\": True,\n                \"password\": True,\n            },\n            \"openai_api_version\": {\n                \"display_name\": \"OpenAI API Version\",\n                \"advanced\": True,\n            },\n            \"openai_organization\": {\n                \"display_name\": \"OpenAI Organization\",\n                \"advanced\": True,\n            },\n            \"openai_proxy\": {\"display_name\": \"OpenAI Proxy\", \"advanced\": True},\n            \"request_timeout\": {\"display_name\": \"Request Timeout\", \"advanced\": True},\n            \"show_progress_bar\": {\n                \"display_name\": \"Show Progress Bar\",\n                \"advanced\": True,\n            },\n            \"skip_empty\": {\"display_name\": \"Skip Empty\", \"advanced\": True},\n            \"tiktoken_model_name\": {\n                \"display_name\": \"TikToken Model Name\",\n                \"advanced\": True,\n            },\n            \"tiktoken_enable\": {\"display_name\": \"TikToken Enable\", \"advanced\": True},\n        }\n\n    def build(\n        self,\n        openai_api_key: str,\n        default_headers: Optional[Dict[str, str]] = None,\n        default_query: Optional[NestedDict] = {},\n        allowed_special: List[str] = [],\n        disallowed_special: List[str] = [\"all\"],\n        chunk_size: int = 1000,\n        client: Optional[Any] = None,\n        deployment: str = \"text-embedding-ada-002\",\n        embedding_ctx_length: int = 8191,\n        max_retries: int = 6,\n        model: str = \"text-embedding-ada-002\",\n        model_kwargs: NestedDict = {},\n        openai_api_base: Optional[str] = None,\n        openai_api_type: Optional[str] = None,\n        openai_api_version: Optional[str] = None,\n        openai_organization: Optional[str] = None,\n        openai_proxy: Optional[str] = None,\n        request_timeout: Optional[float] = None,\n        show_progress_bar: bool = False,\n        skip_empty: bool = False,\n        tiktoken_enable: bool = True,\n        tiktoken_model_name: Optional[str] = None,\n    ) -> Embeddings:\n        # This is to avoid errors with Vector Stores (e.g Chroma)\n        if disallowed_special == [\"all\"]:\n            disallowed_special = \"all\"  # type: ignore\n        if openai_api_key:\n            api_key = SecretStr(openai_api_key)\n        else:\n            api_key = None\n\n        return OpenAIEmbeddings(\n            tiktoken_enabled=tiktoken_enable,\n            default_headers=default_headers,\n            default_query=default_query,\n            allowed_special=set(allowed_special),\n            disallowed_special=\"all\",\n            chunk_size=chunk_size,\n            client=client,\n            deployment=deployment,\n            embedding_ctx_length=embedding_ctx_length,\n            max_retries=max_retries,\n            model=model,\n            model_kwargs=model_kwargs,\n            base_url=openai_api_base,\n            api_key=api_key,\n            openai_api_type=openai_api_type,\n            api_version=openai_api_version,\n            organization=openai_organization,\n            openai_proxy=openai_proxy,\n            timeout=request_timeout,\n            show_progress_bar=show_progress_bar,\n            skip_empty=skip_empty,\n            tiktoken_model_name=tiktoken_model_name,\n        )\n"
+                                "value": "from typing import Dict, List, Optional\n\nfrom langchain_openai.embeddings.base import OpenAIEmbeddings\nfrom pydantic.v1 import SecretStr\n\nfrom langflow.custom import CustomComponent\nfrom langflow.field_typing import Embeddings, NestedDict\n\n\nclass OpenAIEmbeddingsComponent(CustomComponent):\n    display_name = \"OpenAI Embeddings\"\n    description = \"Generate embeddings using OpenAI models.\"\n\n    def build_config(self):\n        return {\n            \"allowed_special\": {\n                \"display_name\": \"Allowed Special\",\n                \"advanced\": True,\n                \"field_type\": \"str\",\n                \"is_list\": True,\n            },\n            \"default_headers\": {\n                \"display_name\": \"Default Headers\",\n                \"advanced\": True,\n                \"field_type\": \"dict\",\n            },\n            \"default_query\": {\n                \"display_name\": \"Default Query\",\n                \"advanced\": True,\n                \"field_type\": \"NestedDict\",\n            },\n            \"disallowed_special\": {\n                \"display_name\": \"Disallowed Special\",\n                \"advanced\": True,\n                \"field_type\": \"str\",\n                \"is_list\": True,\n            },\n            \"chunk_size\": {\"display_name\": \"Chunk Size\", \"advanced\": True},\n            \"client\": {\"display_name\": \"Client\", \"advanced\": True},\n            \"deployment\": {\"display_name\": \"Deployment\", \"advanced\": True},\n            \"embedding_ctx_length\": {\n                \"display_name\": \"Embedding Context Length\",\n                \"advanced\": True,\n            },\n            \"max_retries\": {\"display_name\": \"Max Retries\", \"advanced\": True},\n            \"model\": {\n                \"display_name\": \"Model\",\n                \"advanced\": False,\n                \"options\": [\n                    \"text-embedding-3-small\",\n                    \"text-embedding-3-large\",\n                    \"text-embedding-ada-002\",\n                ],\n            },\n            \"model_kwargs\": {\"display_name\": \"Model Kwargs\", \"advanced\": True},\n            \"openai_api_base\": {\n                \"display_name\": \"OpenAI API Base\",\n                \"password\": True,\n                \"advanced\": True,\n            },\n            \"openai_api_key\": {\"display_name\": \"OpenAI API Key\", \"password\": True},\n            \"openai_api_type\": {\n                \"display_name\": \"OpenAI API Type\",\n                \"advanced\": True,\n                \"password\": True,\n            },\n            \"openai_api_version\": {\n                \"display_name\": \"OpenAI API Version\",\n                \"advanced\": True,\n            },\n            \"openai_organization\": {\n                \"display_name\": \"OpenAI Organization\",\n                \"advanced\": True,\n            },\n            \"openai_proxy\": {\"display_name\": \"OpenAI Proxy\", \"advanced\": True},\n            \"request_timeout\": {\"display_name\": \"Request Timeout\", \"advanced\": True},\n            \"show_progress_bar\": {\n                \"display_name\": \"Show Progress Bar\",\n                \"advanced\": True,\n            },\n            \"skip_empty\": {\"display_name\": \"Skip Empty\", \"advanced\": True},\n            \"tiktoken_model_name\": {\n                \"display_name\": \"TikToken Model Name\",\n                \"advanced\": True,\n            },\n            \"tiktoken_enable\": {\"display_name\": \"TikToken Enable\", \"advanced\": True},\n        }\n\n    def build(\n        self,\n        openai_api_key: str,\n        default_headers: Optional[Dict[str, str]] = None,\n        default_query: Optional[NestedDict] = {},\n        allowed_special: List[str] = [],\n        disallowed_special: List[str] = [\"all\"],\n        chunk_size: int = 1000,\n        deployment: str = \"text-embedding-ada-002\",\n        embedding_ctx_length: int = 8191,\n        max_retries: int = 6,\n        model: str = \"text-embedding-ada-002\",\n        model_kwargs: NestedDict = {},\n        openai_api_base: Optional[str] = None,\n        openai_api_type: Optional[str] = None,\n        openai_api_version: Optional[str] = None,\n        openai_organization: Optional[str] = None,\n        openai_proxy: Optional[str] = None,\n        request_timeout: Optional[float] = None,\n        show_progress_bar: bool = False,\n        skip_empty: bool = False,\n        tiktoken_enable: bool = True,\n        tiktoken_model_name: Optional[str] = None,\n    ) -> Embeddings:\n        # This is to avoid errors with Vector Stores (e.g Chroma)\n        if disallowed_special == [\"all\"]:\n            disallowed_special = \"all\"  # type: ignore\n        if openai_api_key:\n            api_key = SecretStr(openai_api_key)\n        else:\n            api_key = None\n\n        return OpenAIEmbeddings(\n            tiktoken_enabled=tiktoken_enable,\n            default_headers=default_headers,\n            default_query=default_query,\n            allowed_special=set(allowed_special),\n            disallowed_special=\"all\",\n            chunk_size=chunk_size,\n            deployment=deployment,\n            embedding_ctx_length=embedding_ctx_length,\n            max_retries=max_retries,\n            model=model,\n            model_kwargs=model_kwargs,\n            base_url=openai_api_base,\n            api_key=api_key,\n            openai_api_type=openai_api_type,\n            api_version=openai_api_version,\n            organization=openai_organization,\n            openai_proxy=openai_proxy,\n            timeout=request_timeout,\n            show_progress_bar=show_progress_bar,\n            skip_empty=skip_empty,\n            tiktoken_model_name=tiktoken_model_name,\n        )\n"
                             },
                             "default_headers": {
                                 "advanced": true,
                                 "display_name": "Default Headers",
                                 "dynamic": false,
                                 "fileTypes": [],
                                 "file_path": "",
@@ -1169,15 +1169,15 @@
                                 "name": "code",
                                 "password": false,
                                 "placeholder": "",
                                 "required": true,
                                 "show": true,
                                 "title_case": false,
                                 "type": "code",
-                                "value": "from typing import Optional\n\nfrom langchain_openai import ChatOpenAI\nfrom pydantic.v1 import SecretStr\n\nfrom langflow.base.constants import STREAM_INFO_TEXT\nfrom langflow.base.models.model import LCModelComponent\nfrom langflow.base.models.openai_constants import MODEL_NAMES\nfrom langflow.field_typing import NestedDict, Text\n\n\nclass OpenAIModelComponent(LCModelComponent):\n    display_name = \"OpenAI\"\n    description = \"Generates text using OpenAI LLMs.\"\n    icon = \"OpenAI\"\n\n    field_order = [\n        \"max_tokens\",\n        \"model_kwargs\",\n        \"model_name\",\n        \"openai_api_base\",\n        \"openai_api_key\",\n        \"temperature\",\n        \"input_value\",\n        \"system_message\",\n        \"stream\",\n    ]\n\n    def build_config(self):\n        return {\n            \"input_value\": {\"display_name\": \"Input\"},\n            \"max_tokens\": {\n                \"display_name\": \"Max Tokens\",\n                \"advanced\": True,\n            },\n            \"model_kwargs\": {\n                \"display_name\": \"Model Kwargs\",\n                \"advanced\": True,\n            },\n            \"model_name\": {\n                \"display_name\": \"Model Name\",\n                \"advanced\": False,\n                \"options\": MODEL_NAMES,\n            },\n            \"openai_api_base\": {\n                \"display_name\": \"OpenAI API Base\",\n                \"advanced\": True,\n                \"info\": (\n                    \"The base URL of the OpenAI API. Defaults to https://api.openai.com/v1.\\n\\n\"\n                    \"You can change this to use other APIs like JinaChat, LocalAI and Prem.\"\n                ),\n            },\n            \"openai_api_key\": {\n                \"display_name\": \"OpenAI API Key\",\n                \"info\": \"The OpenAI API Key to use for the OpenAI model.\",\n                \"advanced\": False,\n                \"password\": True,\n            },\n            \"temperature\": {\n                \"display_name\": \"Temperature\",\n                \"advanced\": False,\n                \"value\": 0.1,\n            },\n            \"stream\": {\n                \"display_name\": \"Stream\",\n                \"info\": STREAM_INFO_TEXT,\n                \"advanced\": True,\n            },\n            \"system_message\": {\n                \"display_name\": \"System Message\",\n                \"info\": \"System message to pass to the model.\",\n                \"advanced\": True,\n            },\n        }\n\n    def build(\n        self,\n        input_value: Text,\n        openai_api_key: str,\n        temperature: float,\n        model_name: str = \"gpt-4o\",\n        max_tokens: Optional[int] = 256,\n        model_kwargs: NestedDict = {},\n        openai_api_base: Optional[str] = None,\n        stream: bool = False,\n        system_message: Optional[str] = None,\n    ) -> Text:\n        if not openai_api_base:\n            openai_api_base = \"https://api.openai.com/v1\"\n        if openai_api_key:\n            api_key = SecretStr(openai_api_key)\n        else:\n            api_key = None\n\n        output = ChatOpenAI(\n            max_tokens=max_tokens,\n            model_kwargs=model_kwargs,\n            model=model_name,\n            base_url=openai_api_base,\n            api_key=api_key,\n            temperature=temperature,\n        )\n\n        return self.get_chat_result(output, stream, input_value, system_message)\n"
+                                "value": "from typing import Optional\n\nfrom langchain_openai import ChatOpenAI\nfrom pydantic.v1 import SecretStr\n\nfrom langflow.base.constants import STREAM_INFO_TEXT\nfrom langflow.base.models.model import LCModelComponent\nfrom langflow.base.models.openai_constants import MODEL_NAMES\nfrom langflow.field_typing import NestedDict, Text\n\n\nclass OpenAIModelComponent(LCModelComponent):\n    display_name = \"OpenAI\"\n    description = \"Generates text using OpenAI LLMs.\"\n    icon = \"OpenAI\"\n\n    field_order = [\n        \"max_tokens\",\n        \"model_kwargs\",\n        \"model_name\",\n        \"openai_api_base\",\n        \"openai_api_key\",\n        \"temperature\",\n        \"input_value\",\n        \"system_message\",\n        \"stream\",\n    ]\n\n    def build_config(self):\n        return {\n            \"input_value\": {\"display_name\": \"Input\"},\n            \"max_tokens\": {\n                \"display_name\": \"Max Tokens\",\n                \"advanced\": True,\n                \"info\": \"The maximum number of tokens to generate. Set to 0 for unlimited tokens.\",\n            },\n            \"model_kwargs\": {\n                \"display_name\": \"Model Kwargs\",\n                \"advanced\": True,\n            },\n            \"model_name\": {\n                \"display_name\": \"Model Name\",\n                \"advanced\": False,\n                \"options\": MODEL_NAMES,\n            },\n            \"openai_api_base\": {\n                \"display_name\": \"OpenAI API Base\",\n                \"advanced\": True,\n                \"info\": (\n                    \"The base URL of the OpenAI API. Defaults to https://api.openai.com/v1.\\n\\n\"\n                    \"You can change this to use other APIs like JinaChat, LocalAI and Prem.\"\n                ),\n            },\n            \"openai_api_key\": {\n                \"display_name\": \"OpenAI API Key\",\n                \"info\": \"The OpenAI API Key to use for the OpenAI model.\",\n                \"advanced\": False,\n                \"password\": True,\n            },\n            \"temperature\": {\n                \"display_name\": \"Temperature\",\n                \"advanced\": False,\n                \"value\": 0.1,\n            },\n            \"stream\": {\n                \"display_name\": \"Stream\",\n                \"info\": STREAM_INFO_TEXT,\n                \"advanced\": True,\n            },\n            \"system_message\": {\n                \"display_name\": \"System Message\",\n                \"info\": \"System message to pass to the model.\",\n                \"advanced\": True,\n            },\n        }\n\n    def build(\n        self,\n        input_value: Text,\n        openai_api_key: str,\n        temperature: float,\n        model_name: str = \"gpt-4o\",\n        max_tokens: Optional[int] = 256,\n        model_kwargs: NestedDict = {},\n        openai_api_base: Optional[str] = None,\n        stream: bool = False,\n        system_message: Optional[str] = None,\n    ) -> Text:\n        if not openai_api_base:\n            openai_api_base = \"https://api.openai.com/v1\"\n        if openai_api_key:\n            api_key = SecretStr(openai_api_key)\n        else:\n            api_key = None\n\n        output = ChatOpenAI(\n            max_tokens=max_tokens or None,\n            model_kwargs=model_kwargs,\n            model=model_name,\n            base_url=openai_api_base,\n            api_key=api_key,\n            temperature=temperature,\n        )\n\n        return self.get_chat_result(output, stream, input_value, system_message)\n"
                             },
                             "input_value": {
                                 "advanced": false,
                                 "display_name": "Input",
                                 "dynamic": false,
                                 "fileTypes": [],
                                 "file_path": "",
@@ -1198,15 +1198,15 @@
                             },
                             "max_tokens": {
                                 "advanced": true,
                                 "display_name": "Max Tokens",
                                 "dynamic": false,
                                 "fileTypes": [],
                                 "file_path": "",
-                                "info": "",
+                                "info": "The maximum number of tokens to generate. Set to 0 for unlimited tokens.",
                                 "list": false,
                                 "load_from_db": false,
                                 "multiline": false,
                                 "name": "max_tokens",
                                 "password": false,
                                 "placeholder": "",
                                 "required": false,
@@ -1438,15 +1438,15 @@
                                 "name": "code",
                                 "password": false,
                                 "placeholder": "",
                                 "required": true,
                                 "show": true,
                                 "title_case": false,
                                 "type": "code",
-                                "value": "from langchain_core.prompts import PromptTemplate\n\nfrom langflow.field_typing import Prompt, TemplateField, Text\nfrom langflow.interface.custom.custom_component import CustomComponent\n\n\nclass PromptComponent(CustomComponent):\n    display_name: str = \"Prompt\"\n    description: str = \"Create a prompt template with dynamic variables.\"\n    icon = \"prompts\"\n\n    def build_config(self):\n        return {\n            \"template\": TemplateField(display_name=\"Template\"),\n            \"code\": TemplateField(advanced=True),\n        }\n\n    def build(\n        self,\n        template: Prompt,\n        **kwargs,\n    ) -> Text:\n        from langflow.base.prompts.utils import dict_values_to_string\n\n        prompt_template = PromptTemplate.from_template(Text(template))\n        kwargs = dict_values_to_string(kwargs)\n        kwargs = {k: \"\\n\".join(v) if isinstance(v, list) else v for k, v in kwargs.items()}\n        try:\n            formated_prompt = prompt_template.format(**kwargs)\n        except Exception as exc:\n            raise ValueError(f\"Error formatting prompt: {exc}\") from exc\n        self.status = f'Prompt:\\n\"{formated_prompt}\"'\n        return formated_prompt\n"
+                                "value": "from langchain_core.prompts import PromptTemplate\n\nfrom langflow.custom import CustomComponent\nfrom langflow.field_typing import Prompt, TemplateField, Text\n\n\nclass PromptComponent(CustomComponent):\n    display_name: str = \"Prompt\"\n    description: str = \"Create a prompt template with dynamic variables.\"\n    icon = \"prompts\"\n\n    def build_config(self):\n        return {\n            \"template\": TemplateField(display_name=\"Template\"),\n            \"code\": TemplateField(advanced=True),\n        }\n\n    def build(\n        self,\n        template: Prompt,\n        **kwargs,\n    ) -> Text:\n        from langflow.base.prompts.utils import dict_values_to_string\n\n        prompt_template = PromptTemplate.from_template(Text(template))\n        kwargs = dict_values_to_string(kwargs)\n        kwargs = {k: \"\\n\".join(v) if isinstance(v, list) else v for k, v in kwargs.items()}\n        try:\n            formated_prompt = prompt_template.format(**kwargs)\n        except Exception as exc:\n            raise ValueError(f\"Error formatting prompt: {exc}\") from exc\n        self.status = f'Prompt:\\n\"{formated_prompt}\"'\n        return formated_prompt\n"
                             },
                             "context": {
                                 "advanced": false,
                                 "display_name": "context",
                                 "dynamic": false,
                                 "field_type": "str",
                                 "fileTypes": [],
@@ -1773,15 +1773,15 @@
                                 "name": "code",
                                 "password": false,
                                 "placeholder": "",
                                 "required": true,
                                 "show": true,
                                 "title_case": false,
                                 "type": "code",
-                                "value": "from pathlib import Path\nfrom typing import Any, Dict\n\nfrom langflow.base.data.utils import TEXT_FILE_TYPES, parse_text_file_to_record\nfrom langflow.interface.custom.custom_component import CustomComponent\nfrom langflow.schema import Record\n\n\nclass FileComponent(CustomComponent):\n    display_name = \"File\"\n    description = \"A generic file loader.\"\n    icon = \"file-text\"\n\n    def build_config(self) -> Dict[str, Any]:\n        return {\n            \"path\": {\n                \"display_name\": \"Path\",\n                \"field_type\": \"file\",\n                \"file_types\": TEXT_FILE_TYPES,\n                \"info\": f\"Supported file types: {', '.join(TEXT_FILE_TYPES)}\",\n            },\n            \"silent_errors\": {\n                \"display_name\": \"Silent Errors\",\n                \"advanced\": True,\n                \"info\": \"If true, errors will not raise an exception.\",\n            },\n        }\n\n    def load_file(self, path: str, silent_errors: bool = False) -> Record:\n        resolved_path = self.resolve_path(path)\n        path_obj = Path(resolved_path)\n        extension = path_obj.suffix[1:].lower()\n        if extension == \"doc\":\n            raise ValueError(\"doc files are not supported. Please save as .docx\")\n        if extension not in TEXT_FILE_TYPES:\n            raise ValueError(f\"Unsupported file type: {extension}\")\n        record = parse_text_file_to_record(resolved_path, silent_errors)\n        self.status = record if record else \"No data\"\n        return record or Record()\n\n    def build(\n        self,\n        path: str,\n        silent_errors: bool = False,\n    ) -> Record:\n        record = self.load_file(path, silent_errors)\n        self.status = record\n        return record\n"
+                                "value": "from pathlib import Path\nfrom typing import Any, Dict\n\nfrom langflow.base.data.utils import TEXT_FILE_TYPES, parse_text_file_to_record\nfrom langflow.custom import CustomComponent\nfrom langflow.schema import Record\n\n\nclass FileComponent(CustomComponent):\n    display_name = \"File\"\n    description = \"A generic file loader.\"\n    icon = \"file-text\"\n\n    def build_config(self) -> Dict[str, Any]:\n        return {\n            \"path\": {\n                \"display_name\": \"Path\",\n                \"field_type\": \"file\",\n                \"file_types\": TEXT_FILE_TYPES,\n                \"info\": f\"Supported file types: {', '.join(TEXT_FILE_TYPES)}\",\n            },\n            \"silent_errors\": {\n                \"display_name\": \"Silent Errors\",\n                \"advanced\": True,\n                \"info\": \"If true, errors will not raise an exception.\",\n            },\n        }\n\n    def load_file(self, path: str, silent_errors: bool = False) -> Record:\n        resolved_path = self.resolve_path(path)\n        path_obj = Path(resolved_path)\n        extension = path_obj.suffix[1:].lower()\n        if extension == \"doc\":\n            raise ValueError(\"doc files are not supported. Please save as .docx\")\n        if extension not in TEXT_FILE_TYPES:\n            raise ValueError(f\"Unsupported file type: {extension}\")\n        record = parse_text_file_to_record(resolved_path, silent_errors)\n        self.status = record if record else \"No data\"\n        return record or Record()\n\n    def build(\n        self,\n        path: str,\n        silent_errors: bool = False,\n    ) -> Record:\n        record = self.load_file(path, silent_errors)\n        self.status = record\n        return record\n"
                             },
                             "path": {
                                 "advanced": false,
                                 "display_name": "Path",
                                 "dynamic": false,
                                 "fileTypes": [
                                     ".txt",
@@ -1930,15 +1930,15 @@
                                 "name": "code",
                                 "password": false,
                                 "placeholder": "",
                                 "required": true,
                                 "show": true,
                                 "title_case": false,
                                 "type": "code",
-                                "value": "from typing import Optional\nfrom langchain_core.documents import Document\n\nfrom langflow.interface.custom.custom_component import CustomComponent\nfrom langflow.schema import Record\nfrom langflow.utils.util import build_loader_repr_from_records, unescape_string\nfrom langchain_text_splitters import RecursiveCharacterTextSplitter\n\n\nclass RecursiveCharacterTextSplitterComponent(CustomComponent):\n    display_name: str = \"Recursive Character Text Splitter\"\n    description: str = \"Split text into chunks of a specified length.\"\n    documentation: str = \"https://docs.langflow.org/components/text-splitters#recursivecharactertextsplitter\"\n\n    def build_config(self):\n        return {\n            \"inputs\": {\n                \"display_name\": \"Input\",\n                \"info\": \"The texts to split.\",\n                \"input_types\": [\"Document\", \"Record\"],\n            },\n            \"separators\": {\n                \"display_name\": \"Separators\",\n                \"info\": 'The characters to split on.\\nIf left empty defaults to [\"\\\\n\\\\n\", \"\\\\n\", \" \", \"\"].',\n                \"is_list\": True,\n            },\n            \"chunk_size\": {\n                \"display_name\": \"Chunk Size\",\n                \"info\": \"The maximum length of each chunk.\",\n                \"field_type\": \"int\",\n                \"value\": 1000,\n            },\n            \"chunk_overlap\": {\n                \"display_name\": \"Chunk Overlap\",\n                \"info\": \"The amount of overlap between chunks.\",\n                \"field_type\": \"int\",\n                \"value\": 200,\n            },\n            \"code\": {\"show\": False},\n        }\n\n    def build(\n        self,\n        inputs: list[Document],\n        separators: Optional[list[str]] = None,\n        chunk_size: Optional[int] = 1000,\n        chunk_overlap: Optional[int] = 200,\n    ) -> list[Record]:\n        \"\"\"\n        Split text into chunks of a specified length.\n\n        Args:\n            separators (list[str]): The characters to split on.\n            chunk_size (int): The maximum length of each chunk.\n            chunk_overlap (int): The amount of overlap between chunks.\n            length_function (function): The function to use to calculate the length of the text.\n\n        Returns:\n            list[str]: The chunks of text.\n        \"\"\"\n\n        if separators == \"\":\n            separators = None\n        elif separators:\n            # check if the separators list has escaped characters\n            # if there are escaped characters, unescape them\n            separators = [unescape_string(x) for x in separators]\n\n        # Make sure chunk_size and chunk_overlap are ints\n        if isinstance(chunk_size, str):\n            chunk_size = int(chunk_size)\n        if isinstance(chunk_overlap, str):\n            chunk_overlap = int(chunk_overlap)\n        splitter = RecursiveCharacterTextSplitter(\n            separators=separators,\n            chunk_size=chunk_size,\n            chunk_overlap=chunk_overlap,\n        )\n        documents = []\n        for _input in inputs:\n            if isinstance(_input, Record):\n                documents.append(_input.to_lc_document())\n            else:\n                documents.append(_input)\n        docs = splitter.split_documents(documents)\n        records = self.to_records(docs)\n        self.repr_value = build_loader_repr_from_records(records)\n        return records\n"
+                                "value": "from typing import Optional\n\nfrom langchain_core.documents import Document\nfrom langchain_text_splitters import RecursiveCharacterTextSplitter\n\nfrom langflow.custom import CustomComponent\nfrom langflow.schema import Record\nfrom langflow.utils.util import build_loader_repr_from_records, unescape_string\n\n\nclass RecursiveCharacterTextSplitterComponent(CustomComponent):\n    display_name: str = \"Recursive Character Text Splitter\"\n    description: str = \"Split text into chunks of a specified length.\"\n    documentation: str = \"https://docs.langflow.org/components/text-splitters#recursivecharactertextsplitter\"\n\n    def build_config(self):\n        return {\n            \"inputs\": {\n                \"display_name\": \"Input\",\n                \"info\": \"The texts to split.\",\n                \"input_types\": [\"Document\", \"Record\"],\n            },\n            \"separators\": {\n                \"display_name\": \"Separators\",\n                \"info\": 'The characters to split on.\\nIf left empty defaults to [\"\\\\n\\\\n\", \"\\\\n\", \" \", \"\"].',\n                \"is_list\": True,\n            },\n            \"chunk_size\": {\n                \"display_name\": \"Chunk Size\",\n                \"info\": \"The maximum length of each chunk.\",\n                \"field_type\": \"int\",\n                \"value\": 1000,\n            },\n            \"chunk_overlap\": {\n                \"display_name\": \"Chunk Overlap\",\n                \"info\": \"The amount of overlap between chunks.\",\n                \"field_type\": \"int\",\n                \"value\": 200,\n            },\n            \"code\": {\"show\": False},\n        }\n\n    def build(\n        self,\n        inputs: list[Document],\n        separators: Optional[list[str]] = None,\n        chunk_size: Optional[int] = 1000,\n        chunk_overlap: Optional[int] = 200,\n    ) -> list[Record]:\n        \"\"\"\n        Split text into chunks of a specified length.\n\n        Args:\n            separators (list[str]): The characters to split on.\n            chunk_size (int): The maximum length of each chunk.\n            chunk_overlap (int): The amount of overlap between chunks.\n            length_function (function): The function to use to calculate the length of the text.\n\n        Returns:\n            list[str]: The chunks of text.\n        \"\"\"\n\n        if separators == \"\":\n            separators = None\n        elif separators:\n            # check if the separators list has escaped characters\n            # if there are escaped characters, unescape them\n            separators = [unescape_string(x) for x in separators]\n\n        # Make sure chunk_size and chunk_overlap are ints\n        if isinstance(chunk_size, str):\n            chunk_size = int(chunk_size)\n        if isinstance(chunk_overlap, str):\n            chunk_overlap = int(chunk_overlap)\n        splitter = RecursiveCharacterTextSplitter(\n            separators=separators,\n            chunk_size=chunk_size,\n            chunk_overlap=chunk_overlap,\n        )\n        documents = []\n        for _input in inputs:\n            if isinstance(_input, Record):\n                documents.append(_input.to_lc_document())\n            else:\n                documents.append(_input)\n        docs = splitter.split_documents(documents)\n        records = self.to_records(docs)\n        self.repr_value = build_loader_repr_from_records(records)\n        return records\n"
                             },
                             "inputs": {
                                 "advanced": false,
                                 "display_name": "Input",
                                 "dynamic": false,
                                 "fileTypes": [],
                                 "file_path": "",
@@ -2971,15 +2971,15 @@
                                 "name": "code",
                                 "password": false,
                                 "placeholder": "",
                                 "required": true,
                                 "show": true,
                                 "title_case": false,
                                 "type": "code",
-                                "value": "from typing import Any, Dict, List, Optional\n\nfrom langchain_openai.embeddings.base import OpenAIEmbeddings\nfrom pydantic.v1 import SecretStr\n\nfrom langflow.field_typing import Embeddings, NestedDict\nfrom langflow.interface.custom.custom_component import CustomComponent\n\n\nclass OpenAIEmbeddingsComponent(CustomComponent):\n    display_name = \"OpenAI Embeddings\"\n    description = \"Generate embeddings using OpenAI models.\"\n\n    def build_config(self):\n        return {\n            \"allowed_special\": {\n                \"display_name\": \"Allowed Special\",\n                \"advanced\": True,\n                \"field_type\": \"str\",\n                \"is_list\": True,\n            },\n            \"default_headers\": {\n                \"display_name\": \"Default Headers\",\n                \"advanced\": True,\n                \"field_type\": \"dict\",\n            },\n            \"default_query\": {\n                \"display_name\": \"Default Query\",\n                \"advanced\": True,\n                \"field_type\": \"NestedDict\",\n            },\n            \"disallowed_special\": {\n                \"display_name\": \"Disallowed Special\",\n                \"advanced\": True,\n                \"field_type\": \"str\",\n                \"is_list\": True,\n            },\n            \"chunk_size\": {\"display_name\": \"Chunk Size\", \"advanced\": True},\n            \"client\": {\"display_name\": \"Client\", \"advanced\": True},\n            \"deployment\": {\"display_name\": \"Deployment\", \"advanced\": True},\n            \"embedding_ctx_length\": {\n                \"display_name\": \"Embedding Context Length\",\n                \"advanced\": True,\n            },\n            \"max_retries\": {\"display_name\": \"Max Retries\", \"advanced\": True},\n            \"model\": {\n                \"display_name\": \"Model\",\n                \"advanced\": False,\n                \"options\": [\n                    \"text-embedding-3-small\",\n                    \"text-embedding-3-large\",\n                    \"text-embedding-ada-002\",\n                ],\n            },\n            \"model_kwargs\": {\"display_name\": \"Model Kwargs\", \"advanced\": True},\n            \"openai_api_base\": {\n                \"display_name\": \"OpenAI API Base\",\n                \"password\": True,\n                \"advanced\": True,\n            },\n            \"openai_api_key\": {\"display_name\": \"OpenAI API Key\", \"password\": True},\n            \"openai_api_type\": {\n                \"display_name\": \"OpenAI API Type\",\n                \"advanced\": True,\n                \"password\": True,\n            },\n            \"openai_api_version\": {\n                \"display_name\": \"OpenAI API Version\",\n                \"advanced\": True,\n            },\n            \"openai_organization\": {\n                \"display_name\": \"OpenAI Organization\",\n                \"advanced\": True,\n            },\n            \"openai_proxy\": {\"display_name\": \"OpenAI Proxy\", \"advanced\": True},\n            \"request_timeout\": {\"display_name\": \"Request Timeout\", \"advanced\": True},\n            \"show_progress_bar\": {\n                \"display_name\": \"Show Progress Bar\",\n                \"advanced\": True,\n            },\n            \"skip_empty\": {\"display_name\": \"Skip Empty\", \"advanced\": True},\n            \"tiktoken_model_name\": {\n                \"display_name\": \"TikToken Model Name\",\n                \"advanced\": True,\n            },\n            \"tiktoken_enable\": {\"display_name\": \"TikToken Enable\", \"advanced\": True},\n        }\n\n    def build(\n        self,\n        openai_api_key: str,\n        default_headers: Optional[Dict[str, str]] = None,\n        default_query: Optional[NestedDict] = {},\n        allowed_special: List[str] = [],\n        disallowed_special: List[str] = [\"all\"],\n        chunk_size: int = 1000,\n        client: Optional[Any] = None,\n        deployment: str = \"text-embedding-ada-002\",\n        embedding_ctx_length: int = 8191,\n        max_retries: int = 6,\n        model: str = \"text-embedding-ada-002\",\n        model_kwargs: NestedDict = {},\n        openai_api_base: Optional[str] = None,\n        openai_api_type: Optional[str] = None,\n        openai_api_version: Optional[str] = None,\n        openai_organization: Optional[str] = None,\n        openai_proxy: Optional[str] = None,\n        request_timeout: Optional[float] = None,\n        show_progress_bar: bool = False,\n        skip_empty: bool = False,\n        tiktoken_enable: bool = True,\n        tiktoken_model_name: Optional[str] = None,\n    ) -> Embeddings:\n        # This is to avoid errors with Vector Stores (e.g Chroma)\n        if disallowed_special == [\"all\"]:\n            disallowed_special = \"all\"  # type: ignore\n        if openai_api_key:\n            api_key = SecretStr(openai_api_key)\n        else:\n            api_key = None\n\n        return OpenAIEmbeddings(\n            tiktoken_enabled=tiktoken_enable,\n            default_headers=default_headers,\n            default_query=default_query,\n            allowed_special=set(allowed_special),\n            disallowed_special=\"all\",\n            chunk_size=chunk_size,\n            client=client,\n            deployment=deployment,\n            embedding_ctx_length=embedding_ctx_length,\n            max_retries=max_retries,\n            model=model,\n            model_kwargs=model_kwargs,\n            base_url=openai_api_base,\n            api_key=api_key,\n            openai_api_type=openai_api_type,\n            api_version=openai_api_version,\n            organization=openai_organization,\n            openai_proxy=openai_proxy,\n            timeout=request_timeout,\n            show_progress_bar=show_progress_bar,\n            skip_empty=skip_empty,\n            tiktoken_model_name=tiktoken_model_name,\n        )\n"
+                                "value": "from typing import Dict, List, Optional\n\nfrom langchain_openai.embeddings.base import OpenAIEmbeddings\nfrom pydantic.v1 import SecretStr\n\nfrom langflow.custom import CustomComponent\nfrom langflow.field_typing import Embeddings, NestedDict\n\n\nclass OpenAIEmbeddingsComponent(CustomComponent):\n    display_name = \"OpenAI Embeddings\"\n    description = \"Generate embeddings using OpenAI models.\"\n\n    def build_config(self):\n        return {\n            \"allowed_special\": {\n                \"display_name\": \"Allowed Special\",\n                \"advanced\": True,\n                \"field_type\": \"str\",\n                \"is_list\": True,\n            },\n            \"default_headers\": {\n                \"display_name\": \"Default Headers\",\n                \"advanced\": True,\n                \"field_type\": \"dict\",\n            },\n            \"default_query\": {\n                \"display_name\": \"Default Query\",\n                \"advanced\": True,\n                \"field_type\": \"NestedDict\",\n            },\n            \"disallowed_special\": {\n                \"display_name\": \"Disallowed Special\",\n                \"advanced\": True,\n                \"field_type\": \"str\",\n                \"is_list\": True,\n            },\n            \"chunk_size\": {\"display_name\": \"Chunk Size\", \"advanced\": True},\n            \"client\": {\"display_name\": \"Client\", \"advanced\": True},\n            \"deployment\": {\"display_name\": \"Deployment\", \"advanced\": True},\n            \"embedding_ctx_length\": {\n                \"display_name\": \"Embedding Context Length\",\n                \"advanced\": True,\n            },\n            \"max_retries\": {\"display_name\": \"Max Retries\", \"advanced\": True},\n            \"model\": {\n                \"display_name\": \"Model\",\n                \"advanced\": False,\n                \"options\": [\n                    \"text-embedding-3-small\",\n                    \"text-embedding-3-large\",\n                    \"text-embedding-ada-002\",\n                ],\n            },\n            \"model_kwargs\": {\"display_name\": \"Model Kwargs\", \"advanced\": True},\n            \"openai_api_base\": {\n                \"display_name\": \"OpenAI API Base\",\n                \"password\": True,\n                \"advanced\": True,\n            },\n            \"openai_api_key\": {\"display_name\": \"OpenAI API Key\", \"password\": True},\n            \"openai_api_type\": {\n                \"display_name\": \"OpenAI API Type\",\n                \"advanced\": True,\n                \"password\": True,\n            },\n            \"openai_api_version\": {\n                \"display_name\": \"OpenAI API Version\",\n                \"advanced\": True,\n            },\n            \"openai_organization\": {\n                \"display_name\": \"OpenAI Organization\",\n                \"advanced\": True,\n            },\n            \"openai_proxy\": {\"display_name\": \"OpenAI Proxy\", \"advanced\": True},\n            \"request_timeout\": {\"display_name\": \"Request Timeout\", \"advanced\": True},\n            \"show_progress_bar\": {\n                \"display_name\": \"Show Progress Bar\",\n                \"advanced\": True,\n            },\n            \"skip_empty\": {\"display_name\": \"Skip Empty\", \"advanced\": True},\n            \"tiktoken_model_name\": {\n                \"display_name\": \"TikToken Model Name\",\n                \"advanced\": True,\n            },\n            \"tiktoken_enable\": {\"display_name\": \"TikToken Enable\", \"advanced\": True},\n        }\n\n    def build(\n        self,\n        openai_api_key: str,\n        default_headers: Optional[Dict[str, str]] = None,\n        default_query: Optional[NestedDict] = {},\n        allowed_special: List[str] = [],\n        disallowed_special: List[str] = [\"all\"],\n        chunk_size: int = 1000,\n        deployment: str = \"text-embedding-ada-002\",\n        embedding_ctx_length: int = 8191,\n        max_retries: int = 6,\n        model: str = \"text-embedding-ada-002\",\n        model_kwargs: NestedDict = {},\n        openai_api_base: Optional[str] = None,\n        openai_api_type: Optional[str] = None,\n        openai_api_version: Optional[str] = None,\n        openai_organization: Optional[str] = None,\n        openai_proxy: Optional[str] = None,\n        request_timeout: Optional[float] = None,\n        show_progress_bar: bool = False,\n        skip_empty: bool = False,\n        tiktoken_enable: bool = True,\n        tiktoken_model_name: Optional[str] = None,\n    ) -> Embeddings:\n        # This is to avoid errors with Vector Stores (e.g Chroma)\n        if disallowed_special == [\"all\"]:\n            disallowed_special = \"all\"  # type: ignore\n        if openai_api_key:\n            api_key = SecretStr(openai_api_key)\n        else:\n            api_key = None\n\n        return OpenAIEmbeddings(\n            tiktoken_enabled=tiktoken_enable,\n            default_headers=default_headers,\n            default_query=default_query,\n            allowed_special=set(allowed_special),\n            disallowed_special=\"all\",\n            chunk_size=chunk_size,\n            deployment=deployment,\n            embedding_ctx_length=embedding_ctx_length,\n            max_retries=max_retries,\n            model=model,\n            model_kwargs=model_kwargs,\n            base_url=openai_api_base,\n            api_key=api_key,\n            openai_api_type=openai_api_type,\n            api_version=openai_api_version,\n            organization=openai_organization,\n            openai_proxy=openai_proxy,\n            timeout=request_timeout,\n            show_progress_bar=show_progress_bar,\n            skip_empty=skip_empty,\n            tiktoken_model_name=tiktoken_model_name,\n        )\n"
                             },
                             "default_headers": {
                                 "advanced": true,
                                 "display_name": "Default Headers",
                                 "dynamic": false,
                                 "fileTypes": [],
                                 "file_path": "",
```

### Comparing `langflow_base-0.0.48/langflow/interface/custom/attributes.py` & `langflow_base-0.0.49/langflow/custom/attributes.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/interface/custom/code_parser/code_parser.py` & `langflow_base-0.0.49/langflow/custom/code_parser/code_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import traceback
 from typing import Any, Dict, List, Type, Union
 
 from cachetools import TTLCache, cachedmethod, keys
 from fastapi import HTTPException
 from loguru import logger
 
-from langflow.interface.custom.eval import eval_custom_component_code
-from langflow.interface.custom.schema import CallableCodeDetails, ClassCodeDetails, MissingDefault
+from langflow.custom.eval import eval_custom_component_code
+from langflow.custom.schema import CallableCodeDetails, ClassCodeDetails, MissingDefault
 
 
 class CodeSyntaxError(HTTPException):
     pass
 
 
 def get_data_type():
```

### Comparing `langflow_base-0.0.48/langflow/interface/custom/code_parser/utils.py` & `langflow_base-0.0.49/langflow/custom/code_parser/utils.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/interface/custom/custom_component/component.py` & `langflow_base-0.0.49/langflow/custom/custom_component/component.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import operator
 import warnings
 from typing import Any, ClassVar, Optional
 
 from cachetools import TTLCache, cachedmethod
 from fastapi import HTTPException
 
-from langflow.interface.custom.attributes import ATTR_FUNC_MAPPING
-from langflow.interface.custom.code_parser import CodeParser
-from langflow.interface.custom.eval import eval_custom_component_code
+from langflow.custom.attributes import ATTR_FUNC_MAPPING
+from langflow.custom.code_parser import CodeParser
+from langflow.custom.eval import eval_custom_component_code
 from langflow.utils import validate
 
 
 class ComponentCodeNullError(HTTPException):
     pass
```

### Comparing `langflow_base-0.0.48/langflow/interface/custom/custom_component/custom_component.py` & `langflow_base-0.0.49/langflow/custom/custom_component/custom_component.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 from typing import TYPE_CHECKING, Any, Callable, ClassVar, List, Optional, Sequence, Union
 from uuid import UUID
 
 import yaml
 from cachetools import TTLCache, cachedmethod
 from langchain_core.documents import Document
 from pydantic import BaseModel
-
-from langflow.helpers.flow import list_flows, load_flow, run_flow
-from langflow.interface.custom.code_parser.utils import (
+from langflow.custom.code_parser.utils import (
     extract_inner_type_from_generic_alias,
     extract_union_types_from_generic_alias,
 )
-from langflow.interface.custom.custom_component.component import Component
+from langflow.custom.custom_component.component import Component
+from langflow.helpers.flow import list_flows, load_flow, run_flow
 from langflow.schema import Record
 from langflow.schema.dotdict import dotdict
 from langflow.services.deps import get_storage_service, get_variable_service, session_scope
 from langflow.services.storage.service import StorageService
 from langflow.utils import validate
 
 if TYPE_CHECKING:
```

### Comparing `langflow_base-0.0.48/langflow/interface/custom/directory_reader/directory_reader.py` & `langflow_base-0.0.49/langflow/custom/directory_reader/directory_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import ast
 import os
 import zlib
 from pathlib import Path
 
 from loguru import logger
 
-from langflow.interface.custom.custom_component import CustomComponent
+from langflow.custom import CustomComponent
 
 
 class CustomComponentPathValueError(ValueError):
     pass
 
 
 class StringCompressor:
@@ -63,15 +63,15 @@
     def is_empty_file(self, file_content):
         """
         Check if the file content is empty.
         """
         return len(file_content.strip()) == 0
 
     def filter_loaded_components(self, data: dict, with_errors: bool) -> dict:
-        from langflow.interface.custom.utils import build_component
+        from langflow.custom.utils import build_component
 
         items = []
         for menu in data["menu"]:
             components = []
             for component in menu["components"]:
                 try:
                     if component["error"] if with_errors else not component["error"]:
```

### Comparing `langflow_base-0.0.48/langflow/interface/custom/directory_reader/utils.py` & `langflow_base-0.0.49/langflow/custom/directory_reader/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from loguru import logger
 
-from langflow.interface.custom.directory_reader import DirectoryReader
+from langflow.custom.directory_reader import DirectoryReader
 from langflow.template.frontend_node.custom_components import CustomComponentFrontendNode
 
 
 def merge_nested_dicts_with_renaming(dict1, dict2):
     for key, value in dict2.items():
         if key in dict1 and isinstance(value, dict) and isinstance(dict1.get(key), dict):
             for sub_key, sub_value in value.items():
```

### Comparing `langflow_base-0.0.48/langflow/interface/custom/schema.py` & `langflow_base-0.0.49/langflow/custom/schema.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/interface/custom/utils.py` & `langflow_base-0.0.49/langflow/custom/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 from uuid import UUID
 
 from fastapi import HTTPException
 from loguru import logger
 from pydantic import BaseModel
 
-from langflow.field_typing.range_spec import RangeSpec
-from langflow.interface.custom.attributes import ATTR_FUNC_MAPPING
-from langflow.interface.custom.code_parser.utils import extract_inner_type
-from langflow.interface.custom.custom_component import CustomComponent
-from langflow.interface.custom.directory_reader.utils import (
+from langflow.custom import CustomComponent
+from langflow.custom.attributes import ATTR_FUNC_MAPPING
+from langflow.custom.code_parser.utils import extract_inner_type
+from langflow.custom.directory_reader.utils import (
     build_custom_component_list_from_path,
     determine_component_name,
     merge_nested_dicts_with_renaming,
 )
-from langflow.interface.custom.eval import eval_custom_component_code
-from langflow.interface.custom.schema import MissingDefault
+from langflow.custom.eval import eval_custom_component_code
+from langflow.custom.schema import MissingDefault
+from langflow.field_typing.range_spec import RangeSpec
 from langflow.schema import dotdict
 from langflow.template.field.base import TemplateField
 from langflow.template.frontend_node.custom_components import CustomComponentFrontendNode
 from langflow.utils import validate
 from langflow.utils.util import get_base_classes
```

### Comparing `langflow_base-0.0.48/langflow/interface/initialize/utils.py` & `langflow_base-0.0.49/langflow/interface/initialize/utils.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/interface/initialize/vector_store.py` & `langflow_base-0.0.49/langflow/interface/initialize/vector_store.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/interface/listing.py` & `langflow_base-0.0.49/langflow/interface/listing.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,11 +17,11 @@
             "Custom": ["Custom Tool", "Python Function"],
         }
 
     def get_type_dict(self):
         from langflow.interface.types import get_all_types_dict
 
         settings_service = get_settings_service()
-        return get_all_types_dict(settings_service.settings.COMPONENTS_PATH)
+        return get_all_types_dict(settings_service.settings.components_path)
 
 
 lazy_load_dict = AllTypesDict()
```

### Comparing `langflow_base-0.0.48/langflow/interface/run.py` & `langflow_base-0.0.49/langflow/interface/run.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/interface/utils.py` & `langflow_base-0.0.49/langflow/interface/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 import os
 import re
 from io import BytesIO
 from typing import Dict
 
 import yaml
 from docstring_parser import parse
+from langchain_core.language_models import BaseLanguageModel
+from loguru import logger
+from PIL.Image import Image
+
 from langflow.services.chat.config import ChatConfig
 from langflow.services.deps import get_settings_service
 from langflow.utils.util import format_dict, get_base_classes, get_default_factory
-from loguru import logger
-from PIL.Image import Image
-from langchain_core.language_models import BaseLanguageModel
 
 
 def load_file_into_dict(file_path: str) -> dict:
     if not os.path.exists(file_path):
         raise FileNotFoundError(f"File not found: {file_path}")
 
     # Files names are UUID, so we can't find the extension
@@ -91,21 +92,22 @@
 
 def setup_llm_caching():
     """Setup LLM caching."""
     settings_service = get_settings_service()
     try:
         set_langchain_cache(settings_service.settings)
     except ImportError:
-        logger.warning(f"Could not import {settings_service.settings.CACHE_TYPE}. ")
+        logger.warning(f"Could not import {settings_service.settings.cache_type}. ")
     except Exception as exc:
         logger.warning(f"Could not setup LLM caching. Error: {exc}")
 
 
 def set_langchain_cache(settings):
     from langchain.globals import set_llm_cache
+
     from langflow.interface.importing.utils import import_class
 
     if cache_type := os.getenv("LANGFLOW_LANGCHAIN_CACHE"):
         try:
             cache_class = import_class(f"langchain_community.cache.{cache_type or settings.LANGCHAIN_CACHE}")
 
             logger.debug(f"Setting up LLM caching with {cache_class.__name__}")
```

### Comparing `langflow_base-0.0.48/langflow/main.py` & `langflow_base-0.0.49/langflow/main.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/memory.py` & `langflow_base-0.0.49/langflow/memory.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/processing/load.py` & `langflow_base-0.0.49/langflow/load/load.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/processing/process.py` & `langflow_base-0.0.49/langflow/utils/util.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,312 +1,452 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
+import importlib
+import inspect
+import re
+from functools import wraps
+from pathlib import Path
+from typing import Any, Dict, List, Optional, Union
+
+from docstring_parser import parse
+
+
+from langflow.schema.schema import Record
+from langflow.services.deps import get_settings_service
+from langflow.template.frontend_node.constants import FORCE_SHOW_FIELDS
+from langflow.utils import constants
+from langflow.utils.logger import logger
+
+
+def unescape_string(s: str):
+    # Replace escaped new line characters with actual new line characters
+    return s.replace("\\n", "\n")
+
+
+def remove_ansi_escape_codes(text):
+    return re.sub(r"\x1b\[[0-9;]*[a-zA-Z]", "", text)
+
+
+def build_template_from_function(name: str, type_to_loader_dict: Dict, add_function: bool = False):
+    classes = [item.__annotations__["return"].__name__ for item in type_to_loader_dict.values()]
+
+    # Raise error if name is not in chains
+    if name not in classes:
+        raise ValueError(f"{name} not found")
+
+    for _type, v in type_to_loader_dict.items():
+        if v.__annotations__["return"].__name__ == name:
+            _class = v.__annotations__["return"]
+
+            # Get the docstring
+            docs = parse(_class.__doc__)
+
+            variables = {"_type": _type}
+            for class_field_items, value in _class.model_fields.items():
+                if class_field_items in ["callback_manager"]:
+                    continue
+                variables[class_field_items] = {}
+                for name_, value_ in value.__repr_args__():
+                    if name_ == "default_factory":
+                        try:
+                            variables[class_field_items]["default"] = get_default_factory(
+                                module=_class.__base__.__module__, function=value_
+                            )
+                        except Exception:
+                            variables[class_field_items]["default"] = None
+                    elif name_ not in ["name"]:
+                        variables[class_field_items][name_] = value_
+
+                variables[class_field_items]["placeholder"] = (
+                    docs.params[class_field_items] if class_field_items in docs.params else ""
+                )
+            # Adding function to base classes to allow
+            # the output to be a function
+            base_classes = get_base_classes(_class)
+            if add_function:
+                base_classes.append("Callable")
+
+            return {
+                "template": format_dict(variables, name),
+                "description": docs.short_description or "",
+                "base_classes": base_classes,
+            }
+
+
+def build_template_from_method(
+    class_name: str,
+    method_name: str,
+    type_to_cls_dict: Dict,
+    add_function: bool = False,
+):
+    classes = [item.__name__ for item in type_to_cls_dict.values()]
+
+    # Raise error if class_name is not in classes
+    if class_name not in classes:
+        raise ValueError(f"{class_name} not found.")
+
+    for _type, v in type_to_cls_dict.items():
+        if v.__name__ == class_name:
+            _class = v
+
+            # Check if the method exists in this class
+            if not hasattr(_class, method_name):
+                raise ValueError(f"Method {method_name} not found in class {class_name}")
+
+            # Get the method
+            method = getattr(_class, method_name)
+
+            # Get the docstring
+            docs = parse(method.__doc__)
+
+            # Get the signature of the method
+            sig = inspect.signature(method)
+
+            # Get the parameters of the method
+            params = sig.parameters
+
+            # Initialize the variables dictionary with method parameters
+            variables = {
+                "_type": _type,
+                **{
+                    name: {
+                        "default": (param.default if param.default != param.empty else None),
+                        "type": (param.annotation if param.annotation != param.empty else None),
+                        "required": param.default == param.empty,
+                    }
+                    for name, param in params.items()
+                    if name not in ["self", "kwargs", "args"]
+                },
+            }
+
+            base_classes = get_base_classes(_class)
+
+            # Adding function to base classes to allow the output to be a function
+            if add_function:
+                base_classes.append("Callable")
+
+            return {
+                "template": format_dict(variables, class_name),
+                "description": docs.short_description or "",
+                "base_classes": base_classes,
+            }
+
+
+def get_base_classes(cls):
+    """Get the base classes of a class.
+    These are used to determine the output of the nodes.
+    """
+
+    if hasattr(cls, "__bases__") and cls.__bases__:
+        bases = cls.__bases__
+        result = []
+        for base in bases:
+            if any(type in base.__module__ for type in ["pydantic", "abc"]):
+                continue
+            result.append(base.__name__)
+            base_classes = get_base_classes(base)
+            # check if the base_classes are in the result
+            # if not, add them
+            for base_class in base_classes:
+                if base_class not in result:
+                    result.append(base_class)
+    else:
+        result = [cls.__name__]
+    if not result:
+        result = [cls.__name__]
+    return list(set(result + [cls.__name__]))
+
+
+def get_default_factory(module: str, function: str):
+    pattern = r"<function (\w+)>"
+
+    if match := re.search(pattern, function):
+        imported_module = importlib.import_module(module)
+        return getattr(imported_module, match[1])()
+    return None
+
+
+def update_verbose(d: dict, new_value: bool) -> dict:
+    """
+    Recursively updates the value of the 'verbose' key in a dictionary.
+
+    Args:
+        d: the dictionary to update
+        new_value: the new value to set
+
+    Returns:
+        The updated dictionary.
+    """
+
+    for k, v in d.items():
+        if isinstance(v, dict):
+            update_verbose(v, new_value)
+        elif k == "verbose":
+            d[k] = new_value
+    return d
+
+
+def sync_to_async(func):
+    """
+    Decorator to convert a sync function to an async function.
+    """
+
+    @wraps(func)
+    async def async_wrapper(*args, **kwargs):
+        return func(*args, **kwargs)
 
+    return async_wrapper
+
+
+def format_dict(dictionary: Dict[str, Any], class_name: Optional[str] = None) -> Dict[str, Any]:
+    """
+    Formats a dictionary by removing certain keys and modifying the
+    values of other keys.
+
+    Returns:
+        A new dictionary with the desired modifications applied.
+    """
 
-from langchain.agents import AgentExecutor
-from loguru import logger
-from pydantic import BaseModel
-
-from langflow.graph.graph.base import Graph
-from langflow.graph.schema import RunOutputs
-from langflow.graph.vertex.base import Vertex
-from langflow.interface.run import get_memory_key, update_memory_keys
-from langflow.schema.graph import InputValue, Tweaks
-from langflow.schema.schema import INPUT_FIELD_NAME
-from langflow.services.session.service import SessionService
-from langchain_core.agents import AgentAction
-
-
-if TYPE_CHECKING:
-    from langflow.api.v1.schemas import InputValueRequest
-
-
-def fix_memory_inputs(langchain_object):
-    """
-    Given a LangChain object, this function checks if it has a memory attribute and if that memory key exists in the
-    object's input variables. If so, it does nothing. Otherwise, it gets a possible new memory key using the
-    get_memory_key function and updates the memory keys using the update_memory_keys function.
-    """
-    if not hasattr(langchain_object, "memory") or langchain_object.memory is None:
-        return
-    try:
-        if (
-            hasattr(langchain_object.memory, "memory_key")
-            and langchain_object.memory.memory_key in langchain_object.input_variables
-        ):
-            return
-    except AttributeError:
-        input_variables = (
-            langchain_object.prompt.input_variables
-            if hasattr(langchain_object, "prompt")
-            else langchain_object.input_keys
-        )
-        if langchain_object.memory.memory_key in input_variables:
-            return
-
-    possible_new_mem_key = get_memory_key(langchain_object)
-    if possible_new_mem_key is not None:
-        update_memory_keys(langchain_object, possible_new_mem_key)
-
-
-def format_actions(actions: List[Tuple[AgentAction, str]]) -> str:
-    """Format a list of (AgentAction, answer) tuples into a string."""
-    output = []
-    for action, answer in actions:
-        log = action.log
-        tool = action.tool
-        tool_input = action.tool_input
-        output.append(f"Log: {log}")
-        if "Action" not in log and "Action Input" not in log:
-            output.append(f"Tool: {tool}")
-            output.append(f"Tool Input: {tool_input}")
-        output.append(f"Answer: {answer}")
-        output.append("")  # Add a blank line
-    return "\n".join(output)
-
-
-def get_result_and_thought(langchain_object: Any, inputs: dict):
-    """Get result and thought from extracted json"""
-    try:
-        if hasattr(langchain_object, "verbose"):
-            langchain_object.verbose = True
-
-        if hasattr(langchain_object, "return_intermediate_steps"):
-            langchain_object.return_intermediate_steps = False
-
-        try:
-            if not isinstance(langchain_object, AgentExecutor):
-                fix_memory_inputs(langchain_object)
-        except Exception as exc:
-            logger.error(f"Error fixing memory inputs: {exc}")
-
-        try:
-            output = langchain_object(inputs, return_only_outputs=True)
-        except ValueError as exc:
-            # make the error message more informative
-            logger.debug(f"Error: {str(exc)}")
-            output = langchain_object.run(inputs)
-
-    except Exception as exc:
-        raise ValueError(f"Error: {str(exc)}") from exc
-    return output
-
-
-def get_input_str_if_only_one_input(inputs: dict) -> Optional[str]:
-    """Get input string if only one input is provided"""
-    return list(inputs.values())[0] if len(inputs) == 1 else None
-
-
-def process_inputs(
-    inputs: Optional[Union[dict, List[dict]]] = None,
-    artifacts: Optional[Dict[str, Any]] = None,
-) -> Union[dict, List[dict]]:
-    if inputs is None:
-        inputs = {}
-    if artifacts is None:
-        artifacts = {}
-
-    if isinstance(inputs, dict):
-        inputs = update_inputs_dict(inputs, artifacts)
-    elif isinstance(inputs, List):
-        inputs = [update_inputs_dict(inp, artifacts) for inp in inputs]
-
-    return inputs
-
-
-def update_inputs_dict(inputs: dict, artifacts: Dict[str, Any]) -> dict:
-    for key, value in artifacts.items():
-        if key == "repr":
+    for key, value in dictionary.items():
+        if key in ["_type"]:
             continue
-        elif key not in inputs or not inputs[key]:
-            inputs[key] = value
 
-    return inputs
+        _type: Union[str, type] = get_type(value)
 
+        if "BaseModel" in str(_type):
+            continue
 
-class Result(BaseModel):
-    result: Any
-    session_id: str
-
-
-async def run_graph_internal(
-    graph: "Graph",
-    flow_id: str,
-    stream: bool = False,
-    session_id: Optional[str] = None,
-    inputs: Optional[List["InputValueRequest"]] = None,
-    outputs: Optional[List[str]] = None,
-    artifacts: Optional[Dict[str, Any]] = None,
-    session_service: Optional[SessionService] = None,
-) -> tuple[List[RunOutputs], str]:
-    """Run the graph and generate the result"""
-    inputs = inputs or []
-    graph_data = graph._graph_data
-    if session_id is None and session_service is not None:
-        session_id_str = session_service.generate_key(session_id=flow_id, data_graph=graph_data)
-    elif session_id is not None:
-        session_id_str = session_id
-    else:
-        raise ValueError("session_id or session_service must be provided")
-    components = []
-    inputs_list = []
-    types = []
-    for input_value_request in inputs:
-        if input_value_request.input_value is None:
-            logger.warning("InputValueRequest input_value cannot be None, defaulting to an empty string.")
-            input_value_request.input_value = ""
-        components.append(input_value_request.components or [])
-        inputs_list.append({INPUT_FIELD_NAME: input_value_request.input_value})
-        types.append(input_value_request.type)
-
-    run_outputs = await graph.arun(
-        inputs_list,
-        components,
-        types,
-        outputs or [],
-        stream=stream,
-        session_id=session_id_str or "",
-    )
-    if session_id_str and session_service:
-        await session_service.update_session(session_id_str, (graph, artifacts))
-    return run_outputs, session_id_str
+        _type = remove_optional_wrapper(_type)
+        _type = check_list_type(_type, value)
+        _type = replace_mapping_with_dict(_type)
+        _type = get_type_from_union_literal(_type)
+
+        value["type"] = get_formatted_type(key, _type)
+        value["show"] = should_show_field(value, key)
+        value["password"] = is_password_field(key)
+        value["multiline"] = is_multiline_field(key)
+
+        if key == "dict_":
+            set_dict_file_attributes(value)
+
+        replace_default_value_with_actual(value)
+
+        if key == "headers":
+            set_headers_value(value)
 
+        add_options_to_field(value, class_name, key)
 
-def run_graph(
-    graph: "Graph",
-    input_value: str,
-    input_type: str,
-    output_type: str,
-    fallback_to_env_vars: bool = False,
-    output_component: Optional[str] = None,
-) -> List[RunOutputs]:
+    return dictionary
+
+
+# "Union[Literal['f-string'], Literal['jinja2']]" -> "str"
+def get_type_from_union_literal(union_literal: str) -> str:
+    # if types are literal strings
+    # the type is a string
+    if "Literal" in union_literal:
+        return "str"
+    return union_literal
+
+
+def get_type(value: Any) -> Union[str, type]:
     """
-    Runs the given Langflow Graph with the specified input and returns the outputs.
+    Retrieves the type value from the dictionary.
+
+    Returns:
+        The type value.
+    """
+    # get "type" or "annotation" from the value
+    _type = value.get("type") or value.get("annotation")
+
+    return _type if isinstance(_type, str) else _type.__name__
 
-    Args:
-        graph (Graph): The graph to be executed.
-        input_value (str): The input value to be passed to the graph.
-        input_type (str): The type of the input value.
-        output_type (str): The type of the desired output.
-        output_component (Optional[str], optional): The specific output component to retrieve. Defaults to None.
+
+def remove_optional_wrapper(_type: Union[str, type]) -> str:
+    """
+    Removes the 'Optional' wrapper from the type string.
 
     Returns:
-        List[RunOutputs]: A list of RunOutputs objects representing the outputs of the graph.
+        The type string with the 'Optional' wrapper removed.
+    """
+    if isinstance(_type, type):
+        _type = str(_type)
+    if "Optional" in _type:
+        _type = _type.replace("Optional[", "")[:-1]
 
+    return _type
+
+
+def check_list_type(_type: str, value: Dict[str, Any]) -> str:
+    """
+    Checks if the type is a list type and modifies the value accordingly.
+
+    Returns:
+        The modified type string.
     """
-    inputs = [InputValue(components=[], input_value=input_value, type=input_type)]
-    if output_component:
-        outputs = [output_component]
+    if any(list_type in _type for list_type in ["List", "Sequence", "Set"]):
+        _type = _type.replace("List[", "").replace("Sequence[", "").replace("Set[", "")[:-1]
+        value["list"] = True
     else:
-        outputs = [
-            vertex.id
-            for vertex in graph.vertices
-            if output_type == "debug"
-            or (vertex.is_output and (output_type == "any" or output_type in vertex.id.lower()))
-        ]
-    components = []
-    inputs_list = []
-    types = []
-    for input_value_request in inputs:
-        if input_value_request.input_value is None:
-            logger.warning("InputValueRequest input_value cannot be None, defaulting to an empty string.")
-            input_value_request.input_value = ""
-        components.append(input_value_request.components or [])
-        inputs_list.append({INPUT_FIELD_NAME: input_value_request.input_value})
-        types.append(input_value_request.type)
-    run_outputs = graph.run(
-        inputs_list,
-        components,
-        types,
-        outputs or [],
-        stream=False,
-        session_id="",
-        fallback_to_env_vars=fallback_to_env_vars,
+        value["list"] = False
+
+    return _type
+
+
+def replace_mapping_with_dict(_type: str) -> str:
+    """
+    Replaces 'Mapping' with 'dict' in the type string.
+
+    Returns:
+        The modified type string.
+    """
+    if "Mapping" in _type:
+        _type = _type.replace("Mapping", "dict")
+
+    return _type
+
+
+def get_formatted_type(key: str, _type: str) -> str:
+    """
+    Formats the type value based on the given key.
+
+    Returns:
+        The formatted type value.
+    """
+    if key == "allowed_tools":
+        return "Tool"
+
+    elif key == "max_value_length":
+        return "int"
+
+    return _type
+
+
+def should_show_field(value: Dict[str, Any], key: str) -> bool:
+    """
+    Determines if the field should be shown or not.
+
+    Returns:
+        True if the field should be shown, False otherwise.
+    """
+    return (
+        (value["required"] and key != "input_variables")
+        or key in FORCE_SHOW_FIELDS
+        or any(text in key.lower() for text in ["password", "token", "api", "key"])
     )
-    return run_outputs
 
 
-def validate_input(
-    graph_data: Dict[str, Any], tweaks: Union["Tweaks", Dict[str, Dict[str, Any]]]
-) -> List[Dict[str, Any]]:
-    if not isinstance(graph_data, dict) or not isinstance(tweaks, dict):
-        raise ValueError("graph_data and tweaks should be dictionaries")
+def is_password_field(key: str) -> bool:
+    """
+    Determines if the field is a password field.
+
+    Returns:
+        True if the field is a password field, False otherwise.
+    """
+    return any(text in key.lower() for text in ["password", "token", "api", "key"])
+
+
+def is_multiline_field(key: str) -> bool:
+    """
+    Determines if the field is a multiline field.
 
-    nodes = graph_data.get("data", {}).get("nodes") or graph_data.get("nodes")
+    Returns:
+        True if the field is a multiline field, False otherwise.
+    """
+    return key in {
+        "suffix",
+        "prefix",
+        "template",
+        "examples",
+        "code",
+        "headers",
+        "format_instructions",
+    }
 
-    if not isinstance(nodes, list):
-        raise ValueError("graph_data should contain a list of nodes under 'data' key or directly under 'nodes' key")
 
-    return nodes
+def set_dict_file_attributes(value: Dict[str, Any]) -> None:
+    """
+    Sets the file attributes for the 'dict_' key.
+    """
+    value["type"] = "file"
+    value["fileTypes"] = [".json", ".yaml", ".yml"]
 
 
-def apply_tweaks(node: Dict[str, Any], node_tweaks: Dict[str, Any]) -> None:
-    template_data = node.get("data", {}).get("node", {}).get("template")
+def replace_default_value_with_actual(value: Dict[str, Any]) -> None:
+    """
+    Replaces the default value with the actual value.
+    """
+    if "default" in value:
+        value["value"] = value["default"]
+        value.pop("default")
 
-    if not isinstance(template_data, dict):
-        logger.warning(f"Template data for node {node.get('id')} should be a dictionary")
-        return
 
-    for tweak_name, tweak_value in node_tweaks.items():
-        if tweak_name not in template_data:
-            continue
-        if tweak_name in template_data:
-            key = "file_path" if template_data[tweak_name]["type"] == "file" else "value"
-            template_data[tweak_name][key] = tweak_value
-
-
-def apply_tweaks_on_vertex(vertex: Vertex, node_tweaks: Dict[str, Any]) -> None:
-    for tweak_name, tweak_value in node_tweaks.items():
-        if tweak_name and tweak_value and tweak_name in vertex.params:
-            vertex.params[tweak_name] = tweak_value
-
-
-def process_tweaks(
-    graph_data: Dict[str, Any], tweaks: Union["Tweaks", Dict[str, Dict[str, Any]]], stream: bool = False
-) -> Dict[str, Any]:
-    """
-    This function is used to tweak the graph data using the node id and the tweaks dict.
-
-    :param graph_data: The dictionary containing the graph data. It must contain a 'data' key with
-                       'nodes' as its child or directly contain 'nodes' key. Each node should have an 'id' and 'data'.
-    :param tweaks: The dictionary containing the tweaks. The keys can be the node id or the name of the tweak.
-                   The values can be a dictionary containing the tweaks for the node or the value of the tweak.
-    :param stream: A boolean flag indicating whether streaming should be deactivated across all components or not. Default is False.
-    :return: The modified graph_data dictionary.
-    :raises ValueError: If the input is not in the expected format.
-    """
-    tweaks_dict = {}
-    if not isinstance(tweaks, dict):
-        tweaks_dict = tweaks.model_dump()
-    else:
-        tweaks_dict = tweaks
-    if "stream" not in tweaks_dict:
-        tweaks_dict["stream"] = stream
-    nodes = validate_input(graph_data, tweaks_dict)
-    nodes_map = {node.get("id"): node for node in nodes}
-    nodes_display_name_map = {node.get("data", {}).get("node", {}).get("display_name"): node for node in nodes}
-
-    all_nodes_tweaks = {}
-    for key, value in tweaks_dict.items():
-        if isinstance(value, dict):
-            if node := nodes_map.get(key):
-                apply_tweaks(node, value)
-            elif node := nodes_display_name_map.get(key):
-                apply_tweaks(node, value)
-        else:
-            all_nodes_tweaks[key] = value
-    if all_nodes_tweaks:
-        for node in nodes:
-            apply_tweaks(node, all_nodes_tweaks)
-
-    return graph_data
-
-
-def process_tweaks_on_graph(graph: Graph, tweaks: Dict[str, Dict[str, Any]]):
-    for vertex in graph.vertices:
-        if isinstance(vertex, Vertex) and isinstance(vertex.id, str):
-            node_id = vertex.id
-            if node_tweaks := tweaks.get(node_id):
-                apply_tweaks_on_vertex(vertex, node_tweaks)
-        else:
-            logger.warning("Each node should be a Vertex with an 'id' attribute of type str")
+def set_headers_value(value: Dict[str, Any]) -> None:
+    """
+    Sets the value for the 'headers' key.
+    """
+    value["value"] = """{"Authorization": "Bearer <token>"}"""
 
-    return graph
+
+def add_options_to_field(value: Dict[str, Any], class_name: Optional[str], key: str) -> None:
+    """
+    Adds options to the field based on the class name and key.
+    """
+    options_map = {
+        "OpenAI": constants.OPENAI_MODELS,
+        "ChatOpenAI": constants.CHAT_OPENAI_MODELS,
+        "Anthropic": constants.ANTHROPIC_MODELS,
+        "ChatAnthropic": constants.ANTHROPIC_MODELS,
+    }
+
+    if class_name in options_map and key == "model_name":
+        value["options"] = options_map[class_name]
+        value["list"] = True
+        value["value"] = options_map[class_name][0]
+
+
+def build_loader_repr_from_records(records: List[Record]) -> str:
+    """
+    Builds a string representation of the loader based on the given records.
+
+    Args:
+        records (List[Record]): A list of records.
+
+    Returns:
+        str: A string representation of the loader.
+
+    """
+    if records:
+        avg_length = sum(len(doc.text) for doc in records) / len(records)
+        return f"""{len(records)} records
+        \nAvg. Record Length (characters): {int(avg_length)}
+        Records: {records[:3]}..."""
+    return "0 records"
+
+
+def update_settings(
+    config: Optional[str] = None,
+    cache: Optional[str] = None,
+    dev: bool = False,
+    remove_api_keys: bool = False,
+    components_path: Optional[Path] = None,
+    store: bool = True,
+):
+    """Update the settings from a config file."""
+    from langflow.services.utils import initialize_settings_service
+
+    # Check for database_url in the environment variables
+
+    initialize_settings_service()
+    settings_service = get_settings_service()
+    if config:
+        logger.debug(f"Loading settings from {config}")
+        settings_service.settings.update_from_yaml(config, dev=dev)
+    if remove_api_keys:
+        logger.debug(f"Setting remove_api_keys to {remove_api_keys}")
+        settings_service.settings.update_settings(remove_api_keys=remove_api_keys)
+    if cache:
+        logger.debug(f"Setting cache to {cache}")
+        settings_service.settings.update_settings(cache=cache)
+    if components_path:
+        logger.debug(f"Adding component path {components_path}")
+        settings_service.settings.update_settings(components_path=components_path)
+    if not store:
+        logger.debug("Setting store to False")
+        settings_service.settings.update_settings(store=False)
```

### Comparing `langflow_base-0.0.48/langflow/schema/dotdict.py` & `langflow_base-0.0.49/langflow/schema/dotdict.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/schema/graph.py` & `langflow_base-0.0.49/langflow/schema/graph.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/schema/schema.py` & `langflow_base-0.0.49/langflow/schema/schema.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/server.py` & `langflow_base-0.0.49/langflow/server.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/auth/utils.py` & `langflow_base-0.0.49/langflow/services/auth/utils.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/base.py` & `langflow_base-0.0.49/langflow/services/base.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/cache/base.py` & `langflow_base-0.0.49/langflow/services/cache/base.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/cache/factory.py` & `langflow_base-0.0.49/langflow/services/cache/factory.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,26 +12,26 @@
     def __init__(self):
         super().__init__(CacheService)
 
     def create(self, settings_service: "SettingsService"):
         # Here you would have logic to create and configure a CacheService
         # based on the settings_service
 
-        if settings_service.settings.CACHE_TYPE == "redis":
+        if settings_service.settings.cache_type == "redis":
             logger.debug("Creating Redis cache")
             redis_cache = RedisCache(
-                host=settings_service.settings.REDIS_HOST,
-                port=settings_service.settings.REDIS_PORT,
-                db=settings_service.settings.REDIS_DB,
-                url=settings_service.settings.REDIS_URL,
-                expiration_time=settings_service.settings.REDIS_CACHE_EXPIRE,
+                host=settings_service.settings.redis_host,
+                port=settings_service.settings.redis_port,
+                db=settings_service.settings.redis_db,
+                url=settings_service.settings.redis_url,
+                expiration_time=settings_service.settings.redis_cache_expire,
             )
             if redis_cache.is_connected():
                 logger.debug("Redis cache is connected")
                 return redis_cache
             logger.warning("Redis cache is not connected, falling back to in-memory cache")
             return ThreadingInMemoryCache()
 
-        elif settings_service.settings.CACHE_TYPE == "memory":
+        elif settings_service.settings.cache_type == "memory":
             return ThreadingInMemoryCache()
-        elif settings_service.settings.CACHE_TYPE == "async":
+        elif settings_service.settings.cache_type == "async":
             return AsyncInMemoryCache()
```

### Comparing `langflow_base-0.0.48/langflow/services/cache/service.py` & `langflow_base-0.0.49/langflow/services/cache/service.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/cache/utils.py` & `langflow_base-0.0.49/langflow/services/cache/utils.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/chat/cache.py` & `langflow_base-0.0.49/langflow/services/chat/cache.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/chat/service.py` & `langflow_base-0.0.49/langflow/services/chat/service.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/database/factory.py` & `langflow_base-0.0.49/langflow/services/database/factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from typing import TYPE_CHECKING
 
-
 from langflow.services.database.service import DatabaseService
 from langflow.services.factory import ServiceFactory
 
 if TYPE_CHECKING:
     from langflow.services.settings.service import SettingsService
 
 
 class DatabaseServiceFactory(ServiceFactory):
     def __init__(self):
         super().__init__(DatabaseService)
 
     def create(self, settings_service: "SettingsService"):
         # Here you would have logic to create and configure a DatabaseService
-        if not settings_service.settings.DATABASE_URL:
+        if not settings_service.settings.database_url:
             raise ValueError("No database URL provided")
-        return DatabaseService(settings_service.settings.DATABASE_URL)
+        return DatabaseService(settings_service.settings.database_url)
```

### Comparing `langflow_base-0.0.48/langflow/services/database/models/api_key/crud.py` & `langflow_base-0.0.49/langflow/services/database/models/api_key/crud.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/database/models/api_key/model.py` & `langflow_base-0.0.49/langflow/services/database/models/api_key/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime, timezone
 from typing import TYPE_CHECKING, Optional
 from uuid import UUID, uuid4
 
-from pydantic import field_validator, validator
+from pydantic import field_validator
 from sqlmodel import Column, DateTime, Field, Relationship, SQLModel, func
 
 if TYPE_CHECKING:
     from langflow.services.database.models.user import User
 
 
 def utc_now():
@@ -36,26 +36,28 @@
 
 class ApiKeyCreate(ApiKeyBase):
     api_key: Optional[str] = None
     user_id: Optional[UUID] = None
     created_at: Optional[datetime] = Field(default_factory=utc_now)
 
     @field_validator("created_at", mode="before")
+    @classmethod
     def set_created_at(cls, v):
         return v or utc_now()
 
 
 class UnmaskedApiKeyRead(ApiKeyBase):
     id: UUID
     api_key: str = Field()
     user_id: UUID = Field()
 
 
 class ApiKeyRead(ApiKeyBase):
     id: UUID
-    api_key: str = Field()
+    api_key: str = Field(schema_extra={"validate_default": True})
     user_id: UUID = Field()
 
-    @validator("api_key", always=True)
+    @field_validator("api_key")
+    @classmethod
     def mask_api_key(cls, v):
         # This validator will always run, and will mask the API key
         return f"{v[:8]}{'*' * (len(v) - 8)}"
```

### Comparing `langflow_base-0.0.48/langflow/services/database/models/base.py` & `langflow_base-0.0.49/langflow/services/database/models/base.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/database/models/flow/model.py` & `langflow_base-0.0.49/langflow/services/database/models/flow/model.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/database/models/folder/model.py` & `langflow_base-0.0.49/langflow/services/database/models/folder/model.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/database/models/folder/utils.py` & `langflow_base-0.0.49/langflow/services/database/models/folder/utils.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/database/models/user/crud.py` & `langflow_base-0.0.49/langflow/services/database/models/user/crud.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/database/models/user/model.py` & `langflow_base-0.0.49/langflow/services/database/models/user/model.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/database/models/variable/model.py` & `langflow_base-0.0.49/langflow/services/database/models/variable/model.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/database/service.py` & `langflow_base-0.0.49/langflow/services/database/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         self.script_location = langflow_dir / "alembic"
         self.alembic_cfg_path = langflow_dir / "alembic.ini"
         self.engine = self._create_engine()
 
     def _create_engine(self) -> "Engine":
         """Create the engine for the database."""
         settings_service = get_settings_service()
-        if settings_service.settings.DATABASE_URL and settings_service.settings.DATABASE_URL.startswith("sqlite"):
+        if settings_service.settings.database_url and settings_service.settings.database_url.startswith("sqlite"):
             connect_args = {"check_same_thread": False}
         else:
             connect_args = {}
         return create_engine(self.database_url, connect_args=connect_args)
 
     def __enter__(self):
         self._session = Session(self.engine)
```

### Comparing `langflow_base-0.0.48/langflow/services/database/utils.py` & `langflow_base-0.0.49/langflow/services/database/utils.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/deps.py` & `langflow_base-0.0.49/langflow/services/deps.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/factory.py` & `langflow_base-0.0.49/langflow/services/factory.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/manager.py` & `langflow_base-0.0.49/langflow/services/manager.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/monitor/schema.py` & `langflow_base-0.0.49/langflow/services/monitor/schema.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/monitor/service.py` & `langflow_base-0.0.49/langflow/services/monitor/service.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/monitor/utils.py` & `langflow_base-0.0.49/langflow/services/monitor/utils.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/plugins/service.py` & `langflow_base-0.0.49/langflow/services/plugins/service.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/schema.py` & `langflow_base-0.0.49/langflow/services/schema.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/session/service.py` & `langflow_base-0.0.49/langflow/services/session/service.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/session/utils.py` & `langflow_base-0.0.49/langflow/services/session/utils.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/settings/auth.py` & `langflow_base-0.0.49/langflow/services/settings/auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import secrets
 from pathlib import Path
 from typing import Literal
 
 from loguru import logger
 from passlib.context import CryptContext
-from pydantic import Field, SecretStr, validator
+from pydantic import Field, SecretStr, field_validator
 from pydantic_settings import BaseSettings
 
 from langflow.services.settings.constants import DEFAULT_SUPERUSER, DEFAULT_SUPERUSER_PASSWORD
 from langflow.services.settings.utils import read_secret_from_file, write_secret_to_file
 
 
 class AuthSettings(BaseSettings):
@@ -58,31 +58,33 @@
         self.SUPERUSER = DEFAULT_SUPERUSER
         self.SUPERUSER_PASSWORD = DEFAULT_SUPERUSER_PASSWORD
 
     # If autologin is true, then we need to set the credentials to
     # the default values
     # so we need to validate the superuser and superuser_password
     # fields
-    @validator("SUPERUSER", "SUPERUSER_PASSWORD", pre=True)
-    def validate_superuser(cls, value, values):
-        if values.get("AUTO_LOGIN"):
+    @field_validator("SUPERUSER", "SUPERUSER_PASSWORD", mode="before")
+    @classmethod
+    def validate_superuser(cls, value, info):
+        if info.data.get("AUTO_LOGIN"):
             if value != DEFAULT_SUPERUSER:
                 value = DEFAULT_SUPERUSER
                 logger.debug("Resetting superuser to default value")
-            if values.get("SUPERUSER_PASSWORD") != DEFAULT_SUPERUSER_PASSWORD:
-                values["SUPERUSER_PASSWORD"] = DEFAULT_SUPERUSER_PASSWORD
+            if info.data.get("SUPERUSER_PASSWORD") != DEFAULT_SUPERUSER_PASSWORD:
+                info.data["SUPERUSER_PASSWORD"] = DEFAULT_SUPERUSER_PASSWORD
                 logger.debug("Resetting superuser password to default value")
 
             return value
 
         return value
 
-    @validator("SECRET_KEY", pre=True)
-    def get_secret_key(cls, value, values):
-        config_dir = values.get("CONFIG_DIR")
+    @field_validator("SECRET_KEY", mode="before")
+    @classmethod
+    def get_secret_key(cls, value, info):
+        config_dir = info.data.get("CONFIG_DIR")
 
         if not config_dir:
             logger.debug("No CONFIG_DIR provided, not saving secret key")
             return value or secrets.token_urlsafe(32)
 
         secret_key_path = Path(config_dir) / "secret_key"
```

### Comparing `langflow_base-0.0.48/langflow/services/settings/base.py` & `langflow_base-0.0.49/langflow/services/settings/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 import os
 from pathlib import Path
 from shutil import copy2
 from typing import Any, List, Optional, Tuple, Type
 
 import orjson
 import yaml
-from langflow.services.settings.constants import VARIABLES_TO_GET_FROM_ENVIRONMENT
 from loguru import logger
 from pydantic import field_validator
 from pydantic.fields import FieldInfo
 from pydantic_settings import BaseSettings, EnvSettingsSource, PydanticBaseSettingsSource, SettingsConfigDict
 
+from langflow.services.settings.constants import VARIABLES_TO_GET_FROM_ENVIRONMENT
+
 # BASE_COMPONENTS_PATH = str(Path(__file__).parent / "components")
 BASE_COMPONENTS_PATH = str(Path(__file__).parent.parent.parent / "components")
 
 
 def is_list_of_any(field: FieldInfo) -> bool:
     """
     Check if the given field is a list or an optional list of any type.
@@ -53,78 +54,62 @@
             if isinstance(value, list):
                 return value
 
         return super().prepare_field_value(field_name, field, value, value_is_complex)
 
 
 class Settings(BaseSettings):
-    CHAINS: dict = {}
-    AGENTS: dict = {}
-    PROMPTS: dict = {}
-    LLMS: dict = {}
-    TOOLS: dict = {}
-    MEMORIES: dict = {}
-    EMBEDDINGS: dict = {}
-    VECTORSTORES: dict = {}
-    DOCUMENTLOADERS: dict = {}
-    WRAPPERS: dict = {}
-    RETRIEVERS: dict = {}
-    TOOLKITS: dict = {}
-    TEXTSPLITTERS: dict = {}
-    UTILITIES: dict = {}
-    CUSTOM_COMPONENTS: dict = {}
-
     # Define the default LANGFLOW_DIR
-    CONFIG_DIR: Optional[str] = None
+    config_dir: Optional[str] = None
     # Define if langflow db should be saved in config dir or
     # in the langflow directory
-    SAVE_DB_IN_CONFIG_DIR: bool = False
+    save_db_in_config_dir: bool = False
     """Define if langflow database should be saved in LANGFLOW_CONFIG_DIR or in the langflow directory (i.e. in the package directory)."""
 
-    DEV: bool = False
-    DATABASE_URL: Optional[str] = None
-    CACHE_TYPE: str = "async"
-    REMOVE_API_KEYS: bool = False
-    COMPONENTS_PATH: List[str] = []
-    LANGCHAIN_CACHE: str = "InMemoryCache"
+    dev: bool = False
+    database_url: Optional[str] = None
+    cache_type: str = "async"
+    remove_api_keys: bool = False
+    components_path: List[str] = []
+    langchain_cache: str = "InMemoryCache"
 
     # Redis
-    REDIS_HOST: str = "localhost"
-    REDIS_PORT: int = 6379
-    REDIS_DB: int = 0
-    REDIS_URL: Optional[str] = None
-    REDIS_CACHE_EXPIRE: int = 3600
+    redis_host: str = "localhost"
+    redis_port: int = 6379
+    redis_db: int = 0
+    redis_url: Optional[str] = None
+    redis_cache_expire: int = 3600
 
     # PLUGIN_DIR: Optional[str] = None
 
-    LANGFUSE_SECRET_KEY: Optional[str] = None
-    LANGFUSE_PUBLIC_KEY: Optional[str] = None
-    LANGFUSE_HOST: Optional[str] = None
-
-    STORE: Optional[bool] = True
-    STORE_URL: Optional[str] = "https://api.langflow.store"
-    DOWNLOAD_WEBHOOK_URL: Optional[str] = (
+    langfuse_secret_key: Optional[str] = None
+    langfuse_public_key: Optional[str] = None
+    langfuse_host: Optional[str] = None
+
+    store: Optional[bool] = True
+    store_url: Optional[str] = "https://api.langflow.store"
+    download_webhook_url: Optional[str] = (
         "https://api.langflow.store/flows/trigger/ec611a61-8460-4438-b187-a4f65e5559d4"
     )
-    LIKE_WEBHOOK_URL: Optional[str] = "https://api.langflow.store/flows/trigger/64275852-ec00-45c1-984e-3bff814732da"
+    like_webhook_url: Optional[str] = "https://api.langflow.store/flows/trigger/64275852-ec00-45c1-984e-3bff814732da"
 
-    STORAGE_TYPE: str = "local"
+    storage_type: str = "local"
 
-    CELERY_ENABLED: bool = False
+    celery_enabled: bool = False
 
     fallback_to_env_var: bool = True
     """If set to True, Global Variables set in the UI will fallback to a environment variable
     with the same name in case Langflow fails to retrieve the variable value."""
 
     store_environment_variables: bool = True
     """Whether to store environment variables as Global Variables in the database."""
     variables_to_get_from_environment: list[str] = VARIABLES_TO_GET_FROM_ENVIRONMENT
     """List of environment variables to get from the environment and store in the database."""
 
-    @field_validator("CONFIG_DIR", mode="before")
+    @field_validator("config_dir", mode="before")
     def set_langflow_dir(cls, value):
         if not value:
             from platformdirs import user_cache_dir
 
             # Define the app name and author
             app_name = "langflow"
             app_author = "langflow"
@@ -139,51 +124,51 @@
         if isinstance(value, str):
             value = Path(value)
         if not value.exists():
             value.mkdir(parents=True, exist_ok=True)
 
         return str(value)
 
-    @field_validator("DATABASE_URL", mode="before")
+    @field_validator("database_url", mode="before")
     def set_database_url(cls, value, info):
         if not value:
             logger.debug("No database_url provided, trying LANGFLOW_DATABASE_URL env variable")
             if langflow_database_url := os.getenv("LANGFLOW_DATABASE_URL"):
                 value = langflow_database_url
                 logger.debug("Using LANGFLOW_DATABASE_URL env variable.")
             else:
-                logger.debug("No DATABASE_URL env variable, using sqlite database")
+                logger.debug("No database_url env variable, using sqlite database")
                 # Originally, we used sqlite:///./langflow.db
                 # so we need to migrate to the new format
                 # if there is a database in that location
-                if not info.data["CONFIG_DIR"]:
-                    raise ValueError("CONFIG_DIR not set, please set it or provide a DATABASE_URL")
+                if not info.data["config_dir"]:
+                    raise ValueError("config_dir not set, please set it or provide a database_url")
                 from langflow.version import is_pre_release  # type: ignore
 
-                if info.data["SAVE_DB_IN_CONFIG_DIR"]:
-                    database_dir = info.data["CONFIG_DIR"]
-                    logger.debug(f"Saving database to CONFIG_DIR: {database_dir}")
+                if info.data["save_db_in_config_dir"]:
+                    database_dir = info.data["config_dir"]
+                    logger.debug(f"Saving database to config_dir: {database_dir}")
                 else:
                     database_dir = Path(__file__).parent.parent.parent.resolve()
                     logger.debug(f"Saving database to langflow directory: {database_dir}")
 
                 pre_db_file_name = "langflow-pre.db"
                 db_file_name = "langflow.db"
                 new_pre_path = f"{database_dir}/{pre_db_file_name}"
                 new_path = f"{database_dir}/{db_file_name}"
                 final_path = None
                 if is_pre_release:
                     if Path(new_pre_path).exists():
                         final_path = new_pre_path
-                    elif Path(new_path).exists() and info.data["SAVE_DB_IN_CONFIG_DIR"]:
+                    elif Path(new_path).exists() and info.data["save_db_in_config_dir"]:
                         # We need to copy the current db to the new location
                         logger.debug("Copying existing database to new location")
                         copy2(new_path, new_pre_path)
                         logger.debug(f"Copied existing database to {new_pre_path}")
-                    elif Path(f"./{db_file_name}").exists() and info.data["SAVE_DB_IN_CONFIG_DIR"]:
+                    elif Path(f"./{db_file_name}").exists() and info.data["save_db_in_config_dir"]:
                         logger.debug("Copying existing database to new location")
                         copy2(f"./{db_file_name}", new_pre_path)
                         logger.debug(f"Copied existing database to {new_pre_path}")
                     else:
                         logger.debug(f"Creating new database at {new_pre_path}")
                         final_path = new_pre_path
                 else:
@@ -207,15 +192,15 @@
                     else:
                         final_path = new_path
 
                 value = f"sqlite:///{final_path}"
 
         return value
 
-    @field_validator("COMPONENTS_PATH", mode="before")
+    @field_validator("components_path", mode="before")
     def set_components_path(cls, value):
         if os.getenv("LANGFLOW_COMPONENTS_PATH"):
             logger.debug("Adding LANGFLOW_COMPONENTS_PATH to components_path")
             langflow_component_path = os.getenv("LANGFLOW_COMPONENTS_PATH")
             if Path(langflow_component_path).exists() and langflow_component_path not in value:
                 if isinstance(langflow_component_path, list):
                     for path in langflow_component_path:
@@ -236,31 +221,16 @@
         logger.debug(f"Components path: {value}")
         return value
 
     model_config = SettingsConfigDict(validate_assignment=True, extra="ignore", env_prefix="LANGFLOW_")
 
     def update_from_yaml(self, file_path: str, dev: bool = False):
         new_settings = load_settings_from_yaml(file_path)
-        self.CHAINS = new_settings.CHAINS or {}
-        self.AGENTS = new_settings.AGENTS or {}
-        self.PROMPTS = new_settings.PROMPTS or {}
-        self.LLMS = new_settings.LLMS or {}
-        self.TOOLS = new_settings.TOOLS or {}
-        self.MEMORIES = new_settings.MEMORIES or {}
-        self.WRAPPERS = new_settings.WRAPPERS or {}
-        self.TOOLKITS = new_settings.TOOLKITS or {}
-        self.TEXTSPLITTERS = new_settings.TEXTSPLITTERS or {}
-        self.UTILITIES = new_settings.UTILITIES or {}
-        self.EMBEDDINGS = new_settings.EMBEDDINGS or {}
-        self.VECTORSTORES = new_settings.VECTORSTORES or {}
-        self.DOCUMENTLOADERS = new_settings.DOCUMENTLOADERS or {}
-        self.RETRIEVERS = new_settings.RETRIEVERS or {}
-        self.CUSTOM_COMPONENTS = new_settings.CUSTOM_COMPONENTS or {}
-        self.COMPONENTS_PATH = new_settings.COMPONENTS_PATH or []
-        self.DEV = dev
+        self.components_path = new_settings.components_path or []
+        self.dev = dev
 
     def update_settings(self, **kwargs):
         logger.debug("Updating settings")
         for key, value in kwargs.items():
             # value may contain sensitive information, so we don't want to log it
             if not hasattr(self, key):
                 logger.debug(f"Key {key} not found in settings")
@@ -321,10 +291,7 @@
 
         for key in settings_dict:
             if key not in Settings.model_fields.keys():
                 raise KeyError(f"Key {key} not found in settings")
             logger.debug(f"Loading {len(settings_dict[key])} {key} from {file_path}")
 
     return Settings(**settings_dict)
-    return Settings(**settings_dict)
-    return Settings(**settings_dict)
-    return Settings(**settings_dict)
```

### Comparing `langflow_base-0.0.48/langflow/services/settings/constants.py` & `langflow_base-0.0.49/langflow/services/settings/constants.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/settings/manager.py` & `langflow_base-0.0.49/langflow/services/settings/manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,14 +31,14 @@
 
             for key in settings_dict:
                 if key not in Settings.model_fields.keys():
                     raise KeyError(f"Key {key} not found in settings")
                 logger.debug(f"Loading {len(settings_dict[key])} {key} from {file_path}")
 
         settings = Settings(**settings_dict)
-        if not settings.CONFIG_DIR:
+        if not settings.config_dir:
             raise ValueError("CONFIG_DIR must be set in settings")
 
         auth_settings = AuthSettings(
-            CONFIG_DIR=settings.CONFIG_DIR,
+            CONFIG_DIR=settings.config_dir,
         )
         return cls(settings, auth_settings)
```

### Comparing `langflow_base-0.0.48/langflow/services/settings/service.py` & `langflow_base-0.0.49/langflow/services/settings/service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 
 import yaml
+from loguru import logger
+
 from langflow.services.base import Service
 from langflow.services.settings.auth import AuthSettings
 from langflow.services.settings.base import Settings
-from loguru import logger
 
 
 class SettingsService(Service):
     name = "settings_service"
 
     def __init__(self, settings: Settings, auth_settings: AuthSettings):
         super().__init__()
@@ -30,14 +31,14 @@
 
             for key in settings_dict:
                 if key not in Settings.model_fields.keys():
                     logger.warning(f"Key {key} not found in settings")
                 logger.debug(f"Loading {len(settings_dict[key])} {key} from {file_path}")
 
         settings = Settings(**settings_dict)
-        if not settings.CONFIG_DIR:
+        if not settings.config_dir:
             raise ValueError("CONFIG_DIR must be set in settings")
 
         auth_settings = AuthSettings(
-            CONFIG_DIR=settings.CONFIG_DIR,
+            CONFIG_DIR=settings.config_dir,
         )
         return cls(settings, auth_settings)
```

### Comparing `langflow_base-0.0.48/langflow/services/settings/utils.py` & `langflow_base-0.0.49/langflow/services/settings/utils.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/socket/service.py` & `langflow_base-0.0.49/langflow/services/socket/service.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/socket/utils.py` & `langflow_base-0.0.49/langflow/services/socket/utils.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/state/service.py` & `langflow_base-0.0.49/langflow/services/state/service.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/storage/constants.py` & `langflow_base-0.0.49/langflow/services/storage/constants.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/storage/factory.py` & `langflow_base-0.0.49/langflow/services/storage/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class StorageServiceFactory(ServiceFactory):
     def __init__(self):
         super().__init__(
             StorageService,
         )
 
     def create(self, session_service: SessionService, settings_service: SettingsService):
-        storage_type = settings_service.settings.STORAGE_TYPE
+        storage_type = settings_service.settings.storage_type
         if storage_type.lower() == "local":
             from .local import LocalStorageService
 
             return LocalStorageService(session_service, settings_service)
         elif storage_type.lower() == "s3":
             from .s3 import S3StorageService
```

### Comparing `langflow_base-0.0.48/langflow/services/storage/local.py` & `langflow_base-0.0.49/langflow/services/storage/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class LocalStorageService(StorageService):
     """A service class for handling local storage operations without aiofiles."""
 
     def __init__(self, session_service, settings_service):
         """Initialize the local storage service with session and settings services."""
         super().__init__(session_service, settings_service)
-        self.data_dir = Path(settings_service.settings.CONFIG_DIR)
+        self.data_dir = Path(settings_service.settings.config_dir)
         self.set_ready()
 
     def build_full_path(self, flow_id: str, file_name: str) -> str:
         """Build the full path of a file in the local storage."""
         return str(self.data_dir / flow_id / file_name)
 
     async def save_file(self, flow_id: str, file_name: str, data: bytes):
```

### Comparing `langflow_base-0.0.48/langflow/services/storage/s3.py` & `langflow_base-0.0.49/langflow/services/storage/s3.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/storage/service.py` & `langflow_base-0.0.49/langflow/services/storage/service.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/store/exceptions.py` & `langflow_base-0.0.49/langflow/services/store/exceptions.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/store/schema.py` & `langflow_base-0.0.49/langflow/services/store/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Optional
 from uuid import UUID
 
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, field_validator
 
 
 class TagResponse(BaseModel):
     id: UUID
     name: Optional[str]
 
 
@@ -33,15 +33,16 @@
     user_created: Optional[dict] = {}
     tags: Optional[List[TagResponse]] = None
     downloads_count: Optional[int] = None
     last_tested_version: Optional[str] = None
     private: Optional[bool] = None
 
     # tags comes as a TagsIdResponse but we want to return a list of TagResponse
-    @validator("tags", pre=True)
+    @field_validator("tags", mode="before")
+    @classmethod
     def tags_to_list(cls, v):
         # Check if all values are have id and name
         # if so, return v else transform to TagResponse
         if not v:
             return v
         if all(["id" in tag and "name" in tag for tag in v]):
             return v
```

### Comparing `langflow_base-0.0.48/langflow/services/store/service.py` & `langflow_base-0.0.49/langflow/services/store/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,17 +75,17 @@
     is a Directus instance. It allows to search, get and post components to
     the store."""
 
     name = "store_service"
 
     def __init__(self, settings_service: "SettingsService"):
         self.settings_service = settings_service
-        self.base_url = self.settings_service.settings.STORE_URL
-        self.download_webhook_url = self.settings_service.settings.DOWNLOAD_WEBHOOK_URL
-        self.like_webhook_url = self.settings_service.settings.LIKE_WEBHOOK_URL
+        self.base_url = self.settings_service.settings.store_url
+        self.download_webhook_url = self.settings_service.settings.download_webhook_url
+        self.like_webhook_url = self.settings_service.settings.like_webhook_url
         self.components_url = f"{self.base_url}/items/components"
         self.default_fields = [
             "id",
             "name",
             "description",
             "user_created.username",
             "is_component",
```

### Comparing `langflow_base-0.0.48/langflow/services/store/utils.py` & `langflow_base-0.0.49/langflow/services/store/utils.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/task/backends/anyio.py` & `langflow_base-0.0.49/langflow/services/task/backends/anyio.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/task/backends/celery.py` & `langflow_base-0.0.49/langflow/services/task/backends/celery.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/task/service.py` & `langflow_base-0.0.49/langflow/services/task/service.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 class TaskService(Service):
     name = "task_service"
 
     def __init__(self, settings_service: "SettingsService"):
         self.settings_service = settings_service
         try:
-            if self.settings_service.settings.CELERY_ENABLED:
+            if self.settings_service.settings.celery_enabled:
                 USE_CELERY = True
                 status = check_celery_availability()
 
                 USE_CELERY = status.get("availability") is not None
             else:
                 USE_CELERY = False
         except ImportError:
```

### Comparing `langflow_base-0.0.48/langflow/services/task/utils.py` & `langflow_base-0.0.49/langflow/services/task/utils.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/utils.py` & `langflow_base-0.0.49/langflow/services/utils.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/services/variable/service.py` & `langflow_base-0.0.49/langflow/services/variable/service.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/template/field/base.py` & `langflow_base-0.0.49/langflow/template/field/base.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/template/frontend_node/base.py` & `langflow_base-0.0.49/langflow/template/frontend_node/base.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/template/frontend_node/constants.py` & `langflow_base-0.0.49/langflow/template/frontend_node/constants.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/template/frontend_node/custom_components.py` & `langflow_base-0.0.49/langflow/template/frontend_node/custom_components.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 
 from langflow.template.field.base import TemplateField
 from langflow.template.frontend_node.base import FrontendNode
 from langflow.template.template.base import Template
 
-DEFAULT_CUSTOM_COMPONENT_CODE = """from langflow.interface.custom.custom_component import CustomComponent
+DEFAULT_CUSTOM_COMPONENT_CODE = """from langflow.custom import CustomComponent
 
 from typing import Optional, List, Dict, Union
 from langflow.field_typing import (
     AgentExecutor,
     BaseChatMemory,
     BaseLanguageModel,
     BaseLLM,
```

### Comparing `langflow_base-0.0.48/langflow/template/frontend_node/formatter/field_formatters.py` & `langflow_base-0.0.49/langflow/template/frontend_node/formatter/field_formatters.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/template/template/base.py` & `langflow_base-0.0.49/langflow/template/template/base.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/utils/constants.py` & `langflow_base-0.0.49/langflow/utils/constants.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/utils/logger.py` & `langflow_base-0.0.49/langflow/utils/logger.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/utils/payload.py` & `langflow_base-0.0.49/langflow/utils/payload.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/utils/schemas.py` & `langflow_base-0.0.49/langflow/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/utils/validate.py` & `langflow_base-0.0.49/langflow/utils/validate.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/langflow/worker.py` & `langflow_base-0.0.49/langflow/worker.py`

 * *Files identical despite different names*

### Comparing `langflow_base-0.0.48/pyproject.toml` & `langflow_base-0.0.49/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langflow-base"
-version = "0.0.48"
+version = "0.0.49"
 description = "A Python package with a built-in web application"
 authors = ["Langflow <contact@langflow.org>"]
 maintainers = [
     "Carlos Coelho <carlos@langflow.org>",
     "Cristhian Zanforlin <cristhian.lousa@gmail.com>",
     "Gabriel Almeida <gabriel@langflow.org>",
     "Igor Carvalho <igorr.ackerman@gmail.com>",
@@ -57,14 +57,15 @@
 python-docx = "^1.1.0"
 jq = { version = "^1.7.0", markers = "sys_platform != 'win32'" }
 pypdf = "^4.2.0"
 nest-asyncio = "^1.6.0"
 emoji = "^2.12.0"
 cryptography = "^42.0.5"
 asyncer = "^0.0.5"
+pyperclip = "^1.8.2"
 
 
 [tool.poetry.extras]
 deploy = ["celery", "redis", "flower"]
 local = ["llama-cpp-python", "sentence-transformers", "ctransformers"]
 all = ["deploy", "local"]
```

### Comparing `langflow_base-0.0.48/PKG-INFO` & `langflow_base-0.0.49/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langflow-base
-Version: 0.0.48
+Version: 0.0.49
 Summary: A Python package with a built-in web application
 Home-page: https://github.com/langflow-ai/langflow
 License: MIT
 Keywords: nlp,langchain,openai,gpt,gui
 Author: Langflow
 Author-email: contact@langflow.org
 Maintainer: Carlos Coelho
@@ -40,14 +40,15 @@
 Requires-Dist: pandas (==2.2.0)
 Requires-Dist: passlib (>=1.7.4,<2.0.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: platformdirs (>=4.2.0,<5.0.0)
 Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.2.0,<3.0.0)
 Requires-Dist: pypdf (>=4.2.0,<5.0.0)
+Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: python-docx (>=1.1.0,<2.0.0)
 Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Requires-Dist: python-multipart (>=0.0.7,<0.0.8)
 Requires-Dist: python-socketio (>=5.11.0,<6.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: sqlmodel (>=0.0.18,<0.0.19)
 Requires-Dist: typer (>=0.12.0,<0.13.0)
```

