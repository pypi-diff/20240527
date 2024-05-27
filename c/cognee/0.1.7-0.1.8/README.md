# Comparing `tmp/cognee-0.1.7.tar.gz` & `tmp/cognee-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognee-0.1.7.tar", max compression
+gzip compressed data, was "cognee-0.1.8.tar", max compression
```

## Comparing `cognee-0.1.7.tar` & `cognee-0.1.8.tar`

### file list

```diff
@@ -1,168 +1,570 @@
--rw-r--r--   0        0        0    11344 2024-03-30 14:25:45.849829 cognee-0.1.7/LICENSE
--rw-r--r--   0        0        0     3795 2024-05-03 08:46:46.343235 cognee-0.1.7/README.md
--rw-r--r--   0        0        0      249 2024-03-30 11:45:01.187785 cognee-0.1.7/cognee/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.333367 cognee-0.1.7/cognee/api/__init__.py
--rw-r--r--   0        0        0     4370 2024-04-25 22:16:19.632624 cognee-0.1.7/cognee/api/client.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.333421 cognee-0.1.7/cognee/api/v1/__init__.py
--rw-r--r--   0        0        0       21 2024-03-13 17:10:40.333706 cognee-0.1.7/cognee/api/v1/add/__init__.py
--rw-r--r--   0        0        0     4716 2024-04-25 22:16:19.633201 cognee-0.1.7/cognee/api/v1/add/add.py
--rw-r--r--   0        0        0     1517 2024-03-29 12:58:54.562218 cognee-0.1.7/cognee/api/v1/add/add_standalone.py
--rw-r--r--   0        0        0      626 2024-03-29 12:58:54.562387 cognee-0.1.7/cognee/api/v1/add/remember.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.633260 cognee-0.1.7/cognee/api/v1/cognify/__init__.py
--rw-r--r--   0        0        0     7358 2024-05-03 08:36:42.745390 cognee-0.1.7/cognee/api/v1/cognify/cognify.py
--rw-r--r--   0        0        0       27 2024-03-29 12:58:54.562770 cognee-0.1.7/cognee/api/v1/config/__init__.py
--rw-r--r--   0        0        0     2296 2024-04-24 17:34:59.319404 cognee-0.1.7/cognee/api/v1/config/config.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.633793 cognee-0.1.7/cognee/api/v1/datasets/__init__.py
--rw-r--r--   0        0        0      594 2024-04-20 17:06:04.933300 cognee-0.1.7/cognee/api/v1/datasets/datasets.py
--rw-r--r--   0        0        0       25 2024-03-29 16:33:26.552588 cognee-0.1.7/cognee/api/v1/prune/__init__.py
--rw-r--r--   0        0        0      965 2024-04-30 16:56:32.066819 cognee-0.1.7/cognee/api/v1/prune/prune.py
--rw-r--r--   0        0        0       39 2024-03-22 15:50:27.356555 cognee-0.1.7/cognee/api/v1/search/__init__.py
--rw-r--r--   0        0        0     3611 2024-04-25 22:16:19.634363 cognee-0.1.7/cognee/api/v1/search/search.py
--rw-r--r--   0        0        0     6489 2024-04-25 22:16:19.634966 cognee-0.1.7/cognee/config.py
--rw-r--r--   0        0        0     1778 2024-03-13 17:10:40.342297 cognee-0.1.7/cognee/fetch_secret.py
--rw-r--r--   0        0        0     8308 2024-05-03 08:36:42.745874 cognee-0.1.7/cognee/infrastructure/InfrastructureConfig.py
--rw-r--r--   0        0        0       56 2024-03-13 17:10:40.343200 cognee-0.1.7/cognee/infrastructure/__init__.py
--rw-r--r--   0        0        0      110 2024-03-29 12:58:54.563482 cognee-0.1.7/cognee/infrastructure/data/__init__.py
--rw-r--r--   0        0        0     4456 2024-04-24 17:34:59.321526 cognee-0.1.7/cognee/infrastructure/data/chunking/DefaultChunkEngine.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.635699 cognee-0.1.7/cognee/infrastructure/data/chunking/__init__.py
--rw-r--r--   0        0        0      889 2024-03-13 17:10:40.343833 cognee-0.1.7/cognee/infrastructure/data/models/Data.py
--rw-r--r--   0        0        0      721 2024-03-13 17:10:40.344000 cognee-0.1.7/cognee/infrastructure/data/models/Dataset.py
--rw-r--r--   0        0        0      553 2024-03-13 17:10:40.344153 cognee-0.1.7/cognee/infrastructure/data/models/DatasetData.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344189 cognee-0.1.7/cognee/infrastructure/data/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.635851 cognee-0.1.7/cognee/infrastructure/data/utils/__init__.py
--rw-r--r--   0        0        0      756 2024-04-21 19:51:39.681809 cognee-0.1.7/cognee/infrastructure/data/utils/extract_keywords.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344241 cognee-0.1.7/cognee/infrastructure/databases/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344307 cognee-0.1.7/cognee/infrastructure/databases/graph/__init__.py
--rw-r--r--   0        0        0     1291 2024-04-29 10:09:13.468512 cognee-0.1.7/cognee/infrastructure/databases/graph/get_graph_client.py
--rw-r--r--   0        0        0     1162 2024-04-20 17:06:04.935830 cognee-0.1.7/cognee/infrastructure/databases/graph/graph_db_interface.py
--rw-r--r--   0        0        0        0 2024-04-20 17:06:04.935887 cognee-0.1.7/cognee/infrastructure/databases/graph/neo4j_driver/__init__.py
--rw-r--r--   0        0        0     8109 2024-04-20 17:06:04.936346 cognee-0.1.7/cognee/infrastructure/databases/graph/neo4j_driver/adapter.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.344904 cognee-0.1.7/cognee/infrastructure/databases/graph/networkx/__init__.py
--rw-r--r--   0        0        0     5302 2024-04-29 10:11:05.964933 cognee-0.1.7/cognee/infrastructure/databases/graph/networkx/adapter.py
--rw-r--r--   0        0        0      462 2024-03-13 17:10:40.345204 cognee-0.1.7/cognee/infrastructure/databases/relational/DatabaseEngine.py
--rw-r--r--   0        0        0       76 2024-03-13 17:10:40.345343 cognee-0.1.7/cognee/infrastructure/databases/relational/ModelBase.py
--rw-r--r--   0        0        0      170 2024-03-13 17:10:40.345690 cognee-0.1.7/cognee/infrastructure/databases/relational/__init__.py
--rw-r--r--   0        0        0     4539 2024-04-20 17:06:04.937151 cognee-0.1.7/cognee/infrastructure/databases/relational/duckdb/DuckDBAdapter.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.637021 cognee-0.1.7/cognee/infrastructure/databases/relational/duckdb/__init__.py
--rw-r--r--   0        0        0     1006 2024-03-13 17:10:40.346527 cognee-0.1.7/cognee/infrastructure/databases/relational/relational_db_interface.py
--rw-r--r--   0        0        0     2847 2024-03-13 17:10:40.346830 cognee-0.1.7/cognee/infrastructure/databases/relational/sqlite/SqliteEngine.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.346864 cognee-0.1.7/cognee/infrastructure/databases/relational/sqlite/__init__.py
--rw-r--r--   0        0        0       41 2024-03-13 17:10:40.347026 cognee-0.1.7/cognee/infrastructure/databases/relational/utils/__init__.py
--rw-r--r--   0        0        0      595 2024-03-13 17:10:40.347281 cognee-0.1.7/cognee/infrastructure/databases/relational/utils/with_rollback.py
--rw-r--r--   0        0        0      191 2024-03-29 14:26:49.588629 cognee-0.1.7/cognee/infrastructure/databases/vector/__init__.py
--rw-r--r--   0        0        0     1343 2024-05-03 08:36:42.746430 cognee-0.1.7/cognee/infrastructure/databases/vector/embeddings/DefaultEmbeddingEngine.py
--rw-r--r--   0        0        0      243 2024-05-03 08:36:42.746729 cognee-0.1.7/cognee/infrastructure/databases/vector/embeddings/EmbeddingEngine.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.637164 cognee-0.1.7/cognee/infrastructure/databases/vector/embeddings/__init__.py
--rw-r--r--   0        0        0     5264 2024-05-03 08:36:42.747158 cognee-0.1.7/cognee/infrastructure/databases/vector/lancedb/LanceDBAdapter.py
--rw-r--r--   0        0        0      138 2024-03-22 15:50:27.357923 cognee-0.1.7/cognee/infrastructure/databases/vector/models/CollectionConfig.py
--rw-r--r--   0        0        0      398 2024-05-03 08:36:42.747541 cognee-0.1.7/cognee/infrastructure/databases/vector/models/DataPoint.py
--rw-r--r--   0        0        0       69 2024-05-03 08:36:42.747946 cognee-0.1.7/cognee/infrastructure/databases/vector/models/PayloadSchema.py
--rw-r--r--   0        0        0      171 2024-03-22 15:50:27.358192 cognee-0.1.7/cognee/infrastructure/databases/vector/models/ScoredResult.py
--rw-r--r--   0        0        0      143 2024-03-22 15:50:27.358320 cognee-0.1.7/cognee/infrastructure/databases/vector/models/VectorConfig.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.637726 cognee-0.1.7/cognee/infrastructure/databases/vector/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.637873 cognee-0.1.7/cognee/infrastructure/databases/vector/pinecone/__init__.py
--rw-r--r--   0        0        0      256 2024-03-13 17:10:40.348493 cognee-0.1.7/cognee/infrastructure/databases/vector/pinecone/adapter.py
--rw-r--r--   0        0        0     6706 2024-05-03 08:36:42.748385 cognee-0.1.7/cognee/infrastructure/databases/vector/qdrant/QDrantAdapter.py
--rw-r--r--   0        0        0       96 2024-04-20 17:06:04.938909 cognee-0.1.7/cognee/infrastructure/databases/vector/qdrant/__init__.py
--rw-r--r--   0        0        0     1362 2024-05-03 08:36:42.748791 cognee-0.1.7/cognee/infrastructure/databases/vector/vector_db_interface.py
--rw-r--r--   0        0        0     4500 2024-05-03 08:36:42.749289 cognee-0.1.7/cognee/infrastructure/databases/vector/weaviate_db/WeaviateAdapter.py
--rw-r--r--   0        0        0       45 2024-03-22 15:50:27.359256 cognee-0.1.7/cognee/infrastructure/databases/vector/weaviate_db/__init__.py
--rw-r--r--   0        0        0      185 2024-03-13 17:10:40.349945 cognee-0.1.7/cognee/infrastructure/files/__init__.py
--rw-r--r--   0        0        0      364 2024-03-13 17:10:40.350194 cognee-0.1.7/cognee/infrastructure/files/add_file_to_storage.py
--rw-r--r--   0        0        0      320 2024-03-13 17:10:40.350437 cognee-0.1.7/cognee/infrastructure/files/remove_file_from_storage.py
--rw-r--r--   0        0        0     1443 2024-04-20 17:06:04.939689 cognee-0.1.7/cognee/infrastructure/files/storage/LocalStorage.py
--rw-r--r--   0        0        0      640 2024-03-13 17:10:40.350788 cognee-0.1.7/cognee/infrastructure/files/storage/StorageManager.py
--rw-r--r--   0        0        0       39 2024-03-13 17:10:40.351087 cognee-0.1.7/cognee/infrastructure/files/storage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.351134 cognee-0.1.7/cognee/infrastructure/files/utils/__init__.py
--rw-r--r--   0        0        0      392 2024-04-23 10:42:22.654946 cognee-0.1.7/cognee/infrastructure/files/utils/extract_text_from_file.py
--rw-r--r--   0        0        0      835 2024-04-23 10:42:22.655413 cognee-0.1.7/cognee/infrastructure/files/utils/get_file_metadata.py
--rw-r--r--   0        0        0       84 2024-03-13 17:10:40.351628 cognee-0.1.7/cognee/infrastructure/files/utils/get_file_size.py
--rw-r--r--   0        0        0      748 2024-03-29 12:58:54.566841 cognee-0.1.7/cognee/infrastructure/files/utils/guess_file_type.py
--rw-r--r--   0        0        0      825 2024-03-29 12:58:54.567011 cognee-0.1.7/cognee/infrastructure/files/utils/is_text_content.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.351679 cognee-0.1.7/cognee/infrastructure/llm/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 12:58:54.567125 cognee-0.1.7/cognee/infrastructure/llm/anthropic/__init__.py
--rw-r--r--   0        0        0     1768 2024-04-20 17:06:04.940078 cognee-0.1.7/cognee/infrastructure/llm/anthropic/adapter.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.639301 cognee-0.1.7/cognee/infrastructure/llm/generic_llm_api/__init__.py
--rw-r--r--   0        0        0     4308 2024-04-20 17:06:04.940411 cognee-0.1.7/cognee/infrastructure/llm/generic_llm_api/adapter.py
--rw-r--r--   0        0        0     1112 2024-04-20 17:06:04.940688 cognee-0.1.7/cognee/infrastructure/llm/get_llm_client.py
--rw-r--r--   0        0        0     1593 2024-04-20 17:06:04.941068 cognee-0.1.7/cognee/infrastructure/llm/llm_interface.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.352341 cognee-0.1.7/cognee/infrastructure/llm/openai/__init__.py
--rw-r--r--   0        0        0     4885 2024-04-20 17:06:04.941424 cognee-0.1.7/cognee/infrastructure/llm/openai/adapter.py
--rw-r--r--   0        0        0       90 2024-03-22 15:50:27.360221 cognee-0.1.7/cognee/infrastructure/llm/prompts/__init__.py
--rw-r--r--   0        0        0     5614 2024-03-13 17:10:40.353367 cognee-0.1.7/cognee/infrastructure/llm/prompts/classify_content.txt
--rw-r--r--   0        0        0     1323 2024-04-20 17:06:04.941763 cognee-0.1.7/cognee/infrastructure/llm/prompts/generate_cog_layers.txt
--rw-r--r--   0        0        0     2192 2024-04-20 17:06:04.942070 cognee-0.1.7/cognee/infrastructure/llm/prompts/generate_graph_prompt.txt
--rw-r--r--   0        0        0      613 2024-03-22 15:50:27.360715 cognee-0.1.7/cognee/infrastructure/llm/prompts/read_query_prompt.py
--rw-r--r--   0        0        0      962 2024-03-22 15:50:27.360888 cognee-0.1.7/cognee/infrastructure/llm/prompts/render_prompt.py
--rw-r--r--   0        0        0       86 2024-03-22 15:50:27.361017 cognee-0.1.7/cognee/infrastructure/llm/prompts/summarize_content.txt
--rw-r--r--   0        0        0      889 2024-03-13 17:10:40.353850 cognee-0.1.7/cognee/infrastructure/pipeline/models/Operation.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.639465 cognee-0.1.7/cognee/infrastructure/pipeline/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.353968 cognee-0.1.7/cognee/modules/__init__.py
--rw-r--r--   0        0        0        0 2024-04-21 08:53:16.821314 cognee-0.1.7/cognee/modules/cognify/__init__.py
--rw-r--r--   0        0        0     3298 2024-04-21 08:39:11.814707 cognee-0.1.7/cognee/modules/cognify/dataset.py
--rw-r--r--   0        0        0     2622 2024-04-21 08:53:49.473271 cognee-0.1.7/cognee/modules/cognify/evaluate.py
--rw-r--r--   0        0        0        1 2024-03-13 17:10:40.354160 cognee-0.1.7/cognee/modules/cognify/graph/__init__.py
--rw-r--r--   0        0        0     1186 2024-04-25 22:16:19.640140 cognee-0.1.7/cognee/modules/cognify/graph/add_classification_nodes.py
--rw-r--r--   0        0        0     5201 2024-05-03 08:36:42.749768 cognee-0.1.7/cognee/modules/cognify/graph/add_cognitive_layer_graphs.py
--rw-r--r--   0        0        0     1138 2024-04-25 22:16:19.640702 cognee-0.1.7/cognee/modules/cognify/graph/add_cognitive_layers.py
--rw-r--r--   0        0        0     1483 2024-05-03 08:36:42.750160 cognee-0.1.7/cognee/modules/cognify/graph/add_data_chunks.py
--rw-r--r--   0        0        0     1005 2024-05-03 08:36:42.750569 cognee-0.1.7/cognee/modules/cognify/graph/add_document_node.py
--rw-r--r--   0        0        0     2145 2024-05-03 08:36:42.750991 cognee-0.1.7/cognee/modules/cognify/graph/add_label_nodes.py
--rw-r--r--   0        0        0     6969 2024-04-20 17:06:04.945151 cognee-0.1.7/cognee/modules/cognify/graph/add_node_connections.py
--rw-r--r--   0        0        0      798 2024-04-25 09:42:30.766937 cognee-0.1.7/cognee/modules/cognify/graph/add_summary_nodes.py
--rw-r--r--   0        0        0    10961 2024-04-20 17:06:04.945725 cognee-0.1.7/cognee/modules/cognify/graph/create.py
--rw-r--r--   0        0        0     1673 2024-04-20 17:06:04.946033 cognee-0.1.7/cognee/modules/cognify/graph/initialize_graph.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.355565 cognee-0.1.7/cognee/modules/cognify/llm/__init__.py
--rw-r--r--   0        0        0     1216 2024-04-20 17:06:04.946434 cognee-0.1.7/cognee/modules/cognify/llm/resolve_cross_graph_references.py
--rw-r--r--   0        0        0     7187 2024-04-21 13:31:24.978503 cognee-0.1.7/cognee/modules/cognify/test.py
--rw-r--r--   0        0        0     2669 2024-04-21 08:53:43.386066 cognee-0.1.7/cognee/modules/cognify/train.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.641213 cognee-0.1.7/cognee/modules/data/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.641372 cognee-0.1.7/cognee/modules/data/extraction/__init__.py
--rw-r--r--   0        0        0      960 2024-04-20 17:06:04.947116 cognee-0.1.7/cognee/modules/data/extraction/extract_categories.py
--rw-r--r--   0        0        0      490 2024-04-20 17:06:04.947749 cognee-0.1.7/cognee/modules/data/extraction/extract_cognitive_layers.py
--rw-r--r--   0        0        0      497 2024-04-20 17:06:04.948077 cognee-0.1.7/cognee/modules/data/extraction/extract_summary.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.641459 cognee-0.1.7/cognee/modules/data/extraction/knowledge_graph/__init__.py
--rw-r--r--   0        0        0      542 2024-04-20 17:06:04.948548 cognee-0.1.7/cognee/modules/data/extraction/knowledge_graph/extract_content_graph.py
--rw-r--r--   0        0        0     1042 2024-05-03 08:36:42.751386 cognee-0.1.7/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph.py
--rw-r--r--   0        0        0     4740 2024-04-25 22:16:19.641944 cognee-0.1.7/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph_module.py
--rw-r--r--   0        0        0      638 2024-04-20 17:06:04.949628 cognee-0.1.7/cognee/modules/data/get_cognitive_layers.py
--rw-r--r--   0        0        0      516 2024-04-20 17:06:04.949924 cognee-0.1.7/cognee/modules/data/get_content_categories.py
--rw-r--r--   0        0        0      499 2024-04-20 17:06:04.950170 cognee-0.1.7/cognee/modules/data/get_content_summary.py
--rw-r--r--   0        0        0      895 2024-04-20 17:06:04.950394 cognee-0.1.7/cognee/modules/data/get_layer_graphs.py
--rw-r--r--   0        0        0       69 2024-03-30 11:42:14.111069 cognee-0.1.7/cognee/modules/discovery/__init__.py
--rw-r--r--   0        0        0      756 2024-03-30 11:49:14.418639 cognee-0.1.7/cognee/modules/discovery/discover_directory_datasets.py
--rw-r--r--   0        0        0       62 2024-03-29 12:58:54.570027 cognee-0.1.7/cognee/modules/ingestion/__init__.py
--rw-r--r--   0        0        0     1763 2024-03-29 12:58:54.570193 cognee-0.1.7/cognee/modules/ingestion/add_data_to_dataset.py
--rw-r--r--   0        0        0      490 2024-03-29 12:58:54.570428 cognee-0.1.7/cognee/modules/ingestion/classify.py
--rw-r--r--   0        0        0      780 2024-04-21 19:39:20.100717 cognee-0.1.7/cognee/modules/ingestion/data_types/BinaryData.py
--rw-r--r--   0        0        0      295 2024-04-21 19:33:23.824343 cognee-0.1.7/cognee/modules/ingestion/data_types/IngestionData.py
--rw-r--r--   0        0        0      764 2024-04-21 19:38:38.394049 cognee-0.1.7/cognee/modules/ingestion/data_types/TextData.py
--rw-r--r--   0        0        0      145 2024-03-13 17:10:40.359643 cognee-0.1.7/cognee/modules/ingestion/data_types/__init__.py
--rw-r--r--   0        0        0      125 2024-03-13 17:10:40.359841 cognee-0.1.7/cognee/modules/ingestion/exceptions.py
--rw-r--r--   0        0        0      275 2024-04-20 17:06:04.950837 cognee-0.1.7/cognee/modules/ingestion/identify.py
--rw-r--r--   0        0        0      796 2024-03-29 12:58:54.571415 cognee-0.1.7/cognee/modules/ingestion/save.py
--rw-r--r--   0        0        0     1109 2024-04-20 17:06:04.951176 cognee-0.1.7/cognee/modules/search/CogneeSearch.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361325 cognee-0.1.7/cognee/modules/search/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361372 cognee-0.1.7/cognee/modules/search/graph/__init__.py
--rw-r--r--   0        0        0     2083 2024-04-20 17:23:41.887212 cognee-0.1.7/cognee/modules/search/graph/search_adjacent.py
--rw-r--r--   0        0        0     1869 2024-04-20 17:23:55.244065 cognee-0.1.7/cognee/modules/search/graph/search_categories.py
--rw-r--r--   0        0        0     2976 2024-04-20 17:23:50.632849 cognee-0.1.7/cognee/modules/search/graph/search_neighbour.py
--rw-r--r--   0        0        0     1747 2024-04-20 17:24:00.829943 cognee-0.1.7/cognee/modules/search/graph/search_summary.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.361762 cognee-0.1.7/cognee/modules/search/vector/__init__.py
--rw-r--r--   0        0        0     1614 2024-05-03 08:36:42.751852 cognee-0.1.7/cognee/modules/search/vector/search_similarity.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.362031 cognee-0.1.7/cognee/modules/users/__init__.py
--rw-r--r--   0        0        0      179 2024-03-13 17:10:40.362758 cognee-0.1.7/cognee/modules/users/memory/__init__.py
--rw-r--r--   0        0        0      802 2024-03-13 17:10:40.362950 cognee-0.1.7/cognee/modules/users/memory/create_information_points.py
--rw-r--r--   0        0        0      229 2024-03-13 17:10:40.363108 cognee-0.1.7/cognee/modules/users/memory/is_existing_memory.py
--rw-r--r--   0        0        0      203 2024-03-13 17:10:40.363292 cognee-0.1.7/cognee/modules/users/memory/register_memory_for_user.py
--rw-r--r--   0        0        0   124245 2024-04-21 08:54:54.214070 cognee-0.1.7/cognee/programs/extract_knowledge_graph/extract_knowledge_graph.json
--rw-r--r--   0        0        0      182 2024-03-13 17:10:40.363716 cognee-0.1.7/cognee/root_dir.py
--rw-r--r--   0        0        0        0 2024-03-13 17:10:40.364048 cognee-0.1.7/cognee/shared/__init__.py
--rw-r--r--   0        0        0     8633 2024-04-25 09:42:30.768854 cognee-0.1.7/cognee/shared/data_models.py
--rw-r--r--   0        0        0      365 2024-03-22 15:50:27.366234 cognee-0.1.7/cognee/shared/encode_uuid.py
--rw-r--r--   0        0        0        0 2024-04-25 22:16:19.642031 cognee-0.1.7/cognee/tests/__init__.py
--rw-r--r--   0        0        0      985 2024-04-25 22:16:19.642354 cognee-0.1.7/cognee/tests/test_data/Natural_language_processing.txt
--rwxr-xr-x   0        0        0     5982 2024-04-25 22:16:19.642833 cognee-0.1.7/cognee/tests/test_library.py
--rw-r--r--   0        0        0     9487 2024-04-25 22:16:19.643423 cognee-0.1.7/cognee/utils.py
--rw-r--r--   0        0        0     2775 2024-05-03 08:43:06.425402 cognee-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     6856 1970-01-01 00:00:00.000000 cognee-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11344 2024-04-23 05:20:06.866180 cognee-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3943 2024-05-27 05:37:00.853829 cognee-0.1.8/README.md
+-rw-r--r--   0        0        0      186 2024-05-10 20:47:32.390494 cognee-0.1.8/cognee/.data/code/e6ac18788c6a51dfaaf9b963d5bc094b.txt
+-rw-r--r--   0        0        0     1257 2024-05-09 09:29:57.011777 cognee-0.1.8/cognee/.data/example/.craft.txt
+-rw-r--r--   0        0        0      716 2024-05-09 09:29:57.009663 cognee-0.1.8/cognee/.data/example/.flake8.txt
+-rw-r--r--   0        0        0      269 2024-05-09 09:29:57.011322 cognee-0.1.8/cognee/.data/example/.gitignore.txt
+-rw-r--r--   0        0        0      124 2024-05-09 09:29:57.010913 cognee-0.1.8/cognee/.data/example/.gitmodules.txt
+-rw-r--r--   0        0        0      636 2024-05-09 09:29:57.010239 cognee-0.1.8/cognee/.data/example/.pre-commit-config.txt
+-rw-r--r--   0        0        0       14 2024-05-09 09:29:57.010581 cognee-0.1.8/cognee/.data/example/.tool-versions.txt
+-rw-r--r--   0        0        0    97420 2024-05-09 09:29:57.010128 cognee-0.1.8/cognee/.data/example/CHANGELOG.txt
+-rw-r--r--   0        0        0     1169 2024-05-09 09:29:57.010808 cognee-0.1.8/cognee/.data/example/CONTRIBUTING-aws-lambda.txt
+-rw-r--r--   0        0        0     9702 2024-05-09 09:29:57.011552 cognee-0.1.8/cognee/.data/example/CONTRIBUTING.txt
+-rw-r--r--   0        0        0     1093 2024-05-09 09:29:57.009989 cognee-0.1.8/cognee/.data/example/LICENSE.txt
+-rw-r--r--   0        0        0       44 2024-05-09 09:29:57.010692 cognee-0.1.8/cognee/.data/example/MANIFEST.txt
+-rw-r--r--   0        0        0     1751 2024-05-09 09:29:57.010349 cognee-0.1.8/cognee/.data/example/Makefile.txt
+-rw-r--r--   0        0        0     4974 2024-05-09 09:29:57.011021 cognee-0.1.8/cognee/.data/example/README.txt
+-rw-r--r--   0        0        0      222 2024-05-09 09:29:56.911149 cognee-0.1.8/cognee/.data/example/aws-lambda-layer-requirements.txt
+-rw-r--r--   0        0        0      336 2024-05-09 09:29:57.009783 cognee-0.1.8/cognee/.data/example/codecov.txt
+-rw-r--r--   0        0        0      304 2024-05-09 09:29:56.911335 cognee-0.1.8/cognee/.data/example/devenv-requirements.txt
+-rw-r--r--   0        0        0        7 2024-05-09 09:29:57.053281 cognee-0.1.8/cognee/.data/example/docs/.gitignore.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.053711 cognee-0.1.8/cognee/.data/example/docs/_static/.gitkeep.txt
+-rw-r--r--   0        0        0     1314 2024-05-09 09:29:57.053508 cognee-0.1.8/cognee/.data/example/docs/api.txt
+-rw-r--r--   0        0        0      849 2024-05-09 09:29:57.053402 cognee-0.1.8/cognee/.data/example/docs/apidocs.txt
+-rw-r--r--   0        0        0     5638 2024-05-09 09:29:57.053152 cognee-0.1.8/cognee/.data/example/docs/conf.txt
+-rw-r--r--   0        0        0      376 2024-05-09 09:29:57.053022 cognee-0.1.8/cognee/.data/example/docs/index.txt
+-rw-r--r--   0        0        0      202 2024-05-09 09:29:57.053615 cognee-0.1.8/cognee/.data/example/docs/integrations.txt
+-rw-r--r--   0        0        0       87 2024-05-09 09:29:56.911395 cognee-0.1.8/cognee/.data/example/docs-requirements.txt
+-rw-r--r--   0        0        0      381 2024-05-09 09:29:56.980677 cognee-0.1.8/cognee/.data/example/linter-requirements.txt
+-rw-r--r--   0        0        0     1900 2024-05-09 09:29:57.011115 cognee-0.1.8/cognee/.data/example/mypy.txt
+-rw-r--r--   0        0        0      394 2024-05-09 09:29:57.010472 cognee-0.1.8/cognee/.data/example/pyproject.txt
+-rw-r--r--   0        0        0      519 2024-05-09 09:29:57.009890 cognee-0.1.8/cognee/.data/example/pytest.txt
+-rw-r--r--   0        0        0     1002 2024-05-09 09:29:57.053856 cognee-0.1.8/cognee/.data/example/scripts/aws-attach-layer-to-lambda-function.txt
+-rw-r--r--   0        0        0      641 2024-05-09 09:29:57.054177 cognee-0.1.8/cognee/.data/example/scripts/aws-cleanup.txt
+-rw-r--r--   0        0        0      464 2024-05-09 09:29:57.054550 cognee-0.1.8/cognee/.data/example/scripts/aws-delete-lamba-layer-versions.txt
+-rw-r--r--   0        0        0     1065 2024-05-09 09:29:57.054071 cognee-0.1.8/cognee/.data/example/scripts/aws-deploy-local-layer.txt
+-rw-r--r--   0        0        0     4709 2024-05-09 09:29:57.054423 cognee-0.1.8/cognee/.data/example/scripts/build_aws_lambda_layer.txt
+-rw-r--r--   0        0        0      641 2024-05-09 09:29:57.053957 cognee-0.1.8/cognee/.data/example/scripts/bump-version.txt
+-rw-r--r--   0        0        0     2975 2024-05-09 09:29:57.054281 cognee-0.1.8/cognee/.data/example/scripts/init_serverless_sdk.txt
+-rw-r--r--   0        0        0      846 2024-05-09 09:29:57.054658 cognee-0.1.8/cognee/.data/example/scripts/runtox.txt
+-rw-r--r--   0        0        0     9179 2024-05-09 09:29:57.054884 cognee-0.1.8/cognee/.data/example/scripts/split-tox-gh-actions/split-tox-gh-actions.txt
+-rw-r--r--   0        0        0     1623 2024-05-09 09:29:57.055265 cognee-0.1.8/cognee/.data/example/scripts/split-tox-gh-actions/templates/base.txt
+-rw-r--r--   0        0        0     1065 2024-05-09 09:29:57.055380 cognee-0.1.8/cognee/.data/example/scripts/split-tox-gh-actions/templates/check_permissions.txt
+-rw-r--r--   0        0        0     1101 2024-05-09 09:29:57.055148 cognee-0.1.8/cognee/.data/example/scripts/split-tox-gh-actions/templates/check_required.txt
+-rw-r--r--   0        0        0     3966 2024-05-09 09:29:57.055041 cognee-0.1.8/cognee/.data/example/scripts/split-tox-gh-actions/templates/test_group.txt
+-rw-r--r--   0        0        0     1069 2024-05-09 09:29:57.038396 cognee-0.1.8/cognee/.data/example/sentry_sdk/__init__.txt
+-rw-r--r--   0        0        0     6936 2024-05-09 09:29:57.040081 cognee-0.1.8/cognee/.data/example/sentry_sdk/_compat.txt
+-rw-r--r--   0        0        0     4957 2024-05-09 09:29:57.038744 cognee-0.1.8/cognee/.data/example/sentry_sdk/_functools.txt
+-rw-r--r--   0        0        0     5390 2024-05-09 09:29:57.038165 cognee-0.1.8/cognee/.data/example/sentry_sdk/_lru_cache.txt
+-rw-r--r--   0        0        0    11267 2024-05-09 09:29:57.038619 cognee-0.1.8/cognee/.data/example/sentry_sdk/_queue.txt
+-rw-r--r--   0        0        0     5652 2024-05-09 09:29:57.037298 cognee-0.1.8/cognee/.data/example/sentry_sdk/_types.txt
+-rw-r--r--   0        0        0     3790 2024-05-09 09:29:57.037832 cognee-0.1.8/cognee/.data/example/sentry_sdk/_werkzeug.txt
+-rw-r--r--   0        0        0     6242 2024-05-09 09:29:57.039448 cognee-0.1.8/cognee/.data/example/sentry_sdk/api.txt
+-rw-r--r--   0        0        0     1811 2024-05-09 09:29:57.039335 cognee-0.1.8/cognee/.data/example/sentry_sdk/attachments.txt
+-rw-r--r--   0        0        0    28495 2024-05-09 09:29:57.038042 cognee-0.1.8/cognee/.data/example/sentry_sdk/client.txt
+-rw-r--r--   0        0        0    11598 2024-05-09 09:29:57.039201 cognee-0.1.8/cognee/.data/example/sentry_sdk/consts.txt
+-rw-r--r--   0        0        0      170 2024-05-09 09:29:57.052548 cognee-0.1.8/cognee/.data/example/sentry_sdk/crons/__init__.txt
+-rw-r--r--   0        0        0      953 2024-05-09 09:29:57.052320 cognee-0.1.8/cognee/.data/example/sentry_sdk/crons/_decorator.txt
+-rw-r--r--   0        0        0      506 2024-05-09 09:29:57.052872 cognee-0.1.8/cognee/.data/example/sentry_sdk/crons/_decorator_py2.txt
+-rw-r--r--   0        0        0     1527 2024-05-09 09:29:57.052775 cognee-0.1.8/cognee/.data/example/sentry_sdk/crons/api.txt
+-rw-r--r--   0        0        0       87 2024-05-09 09:29:57.052670 cognee-0.1.8/cognee/.data/example/sentry_sdk/crons/consts.txt
+-rw-r--r--   0        0        0     2401 2024-05-09 09:29:57.052446 cognee-0.1.8/cognee/.data/example/sentry_sdk/crons/decorator.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.051812 cognee-0.1.8/cognee/.data/example/sentry_sdk/db/__init__.txt
+-rw-r--r--   0        0        0     1534 2024-05-09 09:29:57.052073 cognee-0.1.8/cognee/.data/example/sentry_sdk/db/explain_plan/__init__.txt
+-rw-r--r--   0        0        0     1597 2024-05-09 09:29:57.051960 cognee-0.1.8/cognee/.data/example/sentry_sdk/db/explain_plan/django.txt
+-rw-r--r--   0        0        0     1656 2024-05-09 09:29:57.052172 cognee-0.1.8/cognee/.data/example/sentry_sdk/db/explain_plan/sqlalchemy.txt
+-rw-r--r--   0        0        0     1132 2024-05-09 09:29:57.039702 cognee-0.1.8/cognee/.data/example/sentry_sdk/debug.txt
+-rw-r--r--   0        0        0     9708 2024-05-09 09:29:57.040585 cognee-0.1.8/cognee/.data/example/sentry_sdk/envelope.txt
+-rw-r--r--   0        0        0    22723 2024-05-09 09:29:57.038984 cognee-0.1.8/cognee/.data/example/sentry_sdk/hub.txt
+-rw-r--r--   0        0        0     7298 2024-05-09 09:29:57.043701 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/__init__.txt
+-rw-r--r--   0        0        0     3096 2024-05-09 09:29:57.047520 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/_asgi_common.txt
+-rw-r--r--   0        0        0     5286 2024-05-09 09:29:57.042096 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/_wsgi_common.txt
+-rw-r--r--   0        0        0    11591 2024-05-09 09:29:57.041477 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/aiohttp.txt
+-rw-r--r--   0        0        0      963 2024-05-09 09:29:57.045018 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/argv.txt
+-rw-r--r--   0        0        0     6228 2024-05-09 09:29:57.046006 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/ariadne.txt
+-rw-r--r--   0        0        0     7180 2024-05-09 09:29:57.045165 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/arq.txt
+-rw-r--r--   0        0        0    11873 2024-05-09 09:29:57.043130 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/asgi.txt
+-rw-r--r--   0        0        0     3201 2024-05-09 09:29:57.043267 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/asyncio.txt
+-rw-r--r--   0        0        0     6297 2024-05-09 09:29:57.041724 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/asyncpg.txt
+-rw-r--r--   0        0        0     1846 2024-05-09 09:29:57.043827 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/atexit.txt
+-rw-r--r--   0        0        0    15922 2024-05-09 09:29:57.041855 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/aws_lambda.txt
+-rw-r--r--   0        0        0     5689 2024-05-09 09:29:57.046865 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/beam.txt
+-rw-r--r--   0        0        0     4542 2024-05-09 09:29:57.046387 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/boto3.txt
+-rw-r--r--   0        0        0     6453 2024-05-09 09:29:57.046735 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/bottle.txt
+-rw-r--r--   0        0        0    21973 2024-05-09 09:29:57.045547 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/celery.txt
+-rw-r--r--   0        0        0     4769 2024-05-09 09:29:57.045835 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/chalice.txt
+-rw-r--r--   0        0        0     5107 2024-05-09 09:29:57.044217 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/clickhouse_driver.txt
+-rw-r--r--   0        0        0     6755 2024-05-09 09:29:57.043423 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/cloud_resource_context.txt
+-rw-r--r--   0        0        0     1184 2024-05-09 09:29:57.042549 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/dedupe.txt
+-rw-r--r--   0        0        0    24135 2024-05-09 09:29:57.050785 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/django/__init__.txt
+-rw-r--r--   0        0        0     7056 2024-05-09 09:29:57.050660 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/django/asgi.txt
+-rw-r--r--   0        0        0     3692 2024-05-09 09:29:57.050997 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/django/caching.txt
+-rw-r--r--   0        0        0     5967 2024-05-09 09:29:57.051109 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/django/middleware.txt
+-rw-r--r--   0        0        0     3054 2024-05-09 09:29:57.050414 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/django/signals_handlers.txt
+-rw-r--r--   0        0        0     5697 2024-05-09 09:29:57.050891 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/django/templates.txt
+-rw-r--r--   0        0        0     5005 2024-05-09 09:29:57.050536 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/django/transactions.txt
+-rw-r--r--   0        0        0     2909 2024-05-09 09:29:57.051222 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/django/views.txt
+-rw-r--r--   0        0        0     2260 2024-05-09 09:29:57.047930 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/excepthook.txt
+-rw-r--r--   0        0        0     2041 2024-05-09 09:29:57.044635 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/executing.txt
+-rw-r--r--   0        0        0     9496 2024-05-09 09:29:57.047081 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/falcon.txt
+-rw-r--r--   0        0        0     4685 2024-05-09 09:29:57.042209 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/fastapi.txt
+-rw-r--r--   0        0        0     7808 2024-05-09 09:29:57.042659 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/flask.txt
+-rw-r--r--   0        0        0     8273 2024-05-09 09:29:57.047406 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/gcp.txt
+-rw-r--r--   0        0        0     2906 2024-05-09 09:29:57.045682 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/gnu_backtrace.txt
+-rw-r--r--   0        0        0     4435 2024-05-09 09:29:57.048081 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/gql.txt
+-rw-r--r--   0        0        0     3746 2024-05-09 09:29:57.046155 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/graphene.txt
+-rw-r--r--   0        0        0     4979 2024-05-09 09:29:57.048716 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/grpc/__init__.txt
+-rw-r--r--   0        0        0      104 2024-05-09 09:29:57.049054 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/grpc/aio/__init__.txt
+-rw-r--r--   0        0        0     3078 2024-05-09 09:29:57.048946 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/grpc/aio/client.txt
+-rw-r--r--   0        0        0     3901 2024-05-09 09:29:57.048847 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/grpc/aio/server.txt
+-rw-r--r--   0        0        0     3235 2024-05-09 09:29:57.048587 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/grpc/client.txt
+-rw-r--r--   0        0        0     2321 2024-05-09 09:29:57.048479 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/grpc/server.txt
+-rw-r--r--   0        0        0     5005 2024-05-09 09:29:57.042430 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/httpx.txt
+-rw-r--r--   0        0        0     5489 2024-05-09 09:29:57.041167 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/huey.txt
+-rw-r--r--   0        0        0     9573 2024-05-09 09:29:57.041050 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/logging.txt
+-rw-r--r--   0        0        0     3051 2024-05-09 09:29:57.047807 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/loguru.txt
+-rw-r--r--   0        0        0      872 2024-05-09 09:29:57.046271 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/modules.txt
+-rw-r--r--   0        0        0    11253 2024-05-09 09:29:57.044872 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/openai.txt
+-rw-r--r--   0        0        0      210 2024-05-09 09:29:57.049551 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/opentelemetry/__init__.txt
+-rw-r--r--   0        0        0      167 2024-05-09 09:29:57.049669 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/opentelemetry/consts.txt
+-rw-r--r--   0        0        0     5830 2024-05-09 09:29:57.049999 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/opentelemetry/integration.txt
+-rw-r--r--   0        0        0     3731 2024-05-09 09:29:57.050128 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/opentelemetry/propagator.txt
+-rw-r--r--   0        0        0    12355 2024-05-09 09:29:57.050285 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/opentelemetry/span_processor.txt
+-rw-r--r--   0        0        0     4554 2024-05-09 09:29:57.042318 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/pure_eval.txt
+-rw-r--r--   0        0        0     6007 2024-05-09 09:29:57.044362 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/pymongo.txt
+-rw-r--r--   0        0        0     7447 2024-05-09 09:29:57.041983 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/pyramid.txt
+-rw-r--r--   0        0        0     7494 2024-05-09 09:29:57.041275 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/quart.txt
+-rw-r--r--   0        0        0    11998 2024-05-09 09:29:57.049412 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/redis/__init__.txt
+-rw-r--r--   0        0        0     2630 2024-05-09 09:29:57.049192 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/redis/asyncio.txt
+-rw-r--r--   0        0        0     5591 2024-05-09 09:29:57.043571 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/rq.txt
+-rw-r--r--   0        0        0    13424 2024-05-09 09:29:57.047678 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/sanic.txt
+-rw-r--r--   0        0        0     1975 2024-05-09 09:29:57.040752 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/serverless.txt
+-rw-r--r--   0        0        0     2945 2024-05-09 09:29:57.047198 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/socket.txt
+-rw-r--r--   0        0        0      208 2024-05-09 09:29:57.051492 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/spark/__init__.txt
+-rw-r--r--   0        0        0     8483 2024-05-09 09:29:57.051700 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/spark/spark_driver.txt
+-rw-r--r--   0        0        0     4013 2024-05-09 09:29:57.051374 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/spark/spark_worker.txt
+-rw-r--r--   0        0        0     5052 2024-05-09 09:29:57.045286 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/sqlalchemy.txt
+-rw-r--r--   0        0        0    24295 2024-05-09 09:29:57.040853 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/starlette.txt
+-rw-r--r--   0        0        0    10211 2024-05-09 09:29:57.044072 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/starlite.txt
+-rw-r--r--   0        0        0     8326 2024-05-09 09:29:57.046611 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/stdlib.txt
+-rw-r--r--   0        0        0    14466 2024-05-09 09:29:57.041605 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/strawberry.txt
+-rw-r--r--   0        0        0     2937 2024-05-09 09:29:57.044499 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/threading.txt
+-rw-r--r--   0        0        0     7337 2024-05-09 09:29:57.045409 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/tornado.txt
+-rw-r--r--   0        0        0     1745 2024-05-09 09:29:57.042872 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/trytond.txt
+-rw-r--r--   0        0        0     9570 2024-05-09 09:29:57.048322 cognee-0.1.8/cognee/.data/example/sentry_sdk/integrations/wsgi.txt
+-rw-r--r--   0        0        0    29551 2024-05-09 09:29:57.036871 cognee-0.1.8/cognee/.data/example/sentry_sdk/metrics.txt
+-rw-r--r--   0        0        0     3728 2024-05-09 09:29:57.037398 cognee-0.1.8/cognee/.data/example/sentry_sdk/monitor.txt
+-rw-r--r--   0        0        0    33083 2024-05-09 09:29:57.040230 cognee-0.1.8/cognee/.data/example/sentry_sdk/profiler.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.039787 cognee-0.1.8/cognee/.data/example/sentry_sdk/py.txt
+-rw-r--r--   0        0        0    44786 2024-05-09 09:29:57.040370 cognee-0.1.8/cognee/.data/example/sentry_sdk/scope.txt
+-rw-r--r--   0        0        0     5230 2024-05-09 09:29:57.037938 cognee-0.1.8/cognee/.data/example/sentry_sdk/scrubber.txt
+-rw-r--r--   0        0        0    13301 2024-05-09 09:29:57.039928 cognee-0.1.8/cognee/.data/example/sentry_sdk/serializer.txt
+-rw-r--r--   0        0        0     5612 2024-05-09 09:29:57.038280 cognee-0.1.8/cognee/.data/example/sentry_sdk/session.txt
+-rw-r--r--   0        0        0     6488 2024-05-09 09:29:57.037077 cognee-0.1.8/cognee/.data/example/sentry_sdk/sessions.txt
+-rw-r--r--   0        0        0     1443 2024-05-09 09:29:57.036975 cognee-0.1.8/cognee/.data/example/sentry_sdk/spotlight.txt
+-rw-r--r--   0        0        0    36352 2024-05-09 09:29:57.037187 cognee-0.1.8/cognee/.data/example/sentry_sdk/tracing.txt
+-rw-r--r--   0        0        0    15841 2024-05-09 09:29:57.037737 cognee-0.1.8/cognee/.data/example/sentry_sdk/tracing_utils.txt
+-rw-r--r--   0        0        0     1244 2024-05-09 09:29:57.036769 cognee-0.1.8/cognee/.data/example/sentry_sdk/tracing_utils_py2.txt
+-rw-r--r--   0        0        0     2146 2024-05-09 09:29:57.037501 cognee-0.1.8/cognee/.data/example/sentry_sdk/tracing_utils_py3.txt
+-rw-r--r--   0        0        0    21702 2024-05-09 09:29:57.037607 cognee-0.1.8/cognee/.data/example/sentry_sdk/transport.txt
+-rw-r--r--   0        0        0      732 2024-05-09 09:29:57.038864 cognee-0.1.8/cognee/.data/example/sentry_sdk/types.txt
+-rw-r--r--   0        0        0    54025 2024-05-09 09:29:57.039580 cognee-0.1.8/cognee/.data/example/sentry_sdk/utils.txt
+-rw-r--r--   0        0        0     4485 2024-05-09 09:29:57.036658 cognee-0.1.8/cognee/.data/example/sentry_sdk/worker.txt
+-rw-r--r--   0        0        0     4122 2024-05-09 09:29:57.011213 cognee-0.1.8/cognee/.data/example/setup.txt
+-rw-r--r--   0        0        0      480 2024-05-09 09:29:56.995867 cognee-0.1.8/cognee/.data/example/test-requirements.txt
+-rw-r--r--   0        0        0      433 2024-05-09 09:29:57.013056 cognee-0.1.8/cognee/.data/example/tests/__init__.txt
+-rw-r--r--   0        0        0    20029 2024-05-09 09:29:57.012191 cognee-0.1.8/cognee/.data/example/tests/conftest.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.036393 cognee-0.1.8/cognee/.data/example/tests/crons/__init__.txt
+-rw-r--r--   0        0        0     9713 2024-05-09 09:29:57.036322 cognee-0.1.8/cognee/.data/example/tests/crons/test_crons.txt
+-rw-r--r--   0        0        0     4240 2024-05-09 09:29:57.036502 cognee-0.1.8/cognee/.data/example/tests/crons/test_crons_async_py3.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.016035 cognee-0.1.8/cognee/.data/example/tests/integrations/__init__.txt
+-rw-r--r--   0        0        0       46 2024-05-09 09:29:57.016847 cognee-0.1.8/cognee/.data/example/tests/integrations/aiohttp/__init__.txt
+-rw-r--r--   0        0        0    16055 2024-05-09 09:29:57.016677 cognee-0.1.8/cognee/.data/example/tests/integrations/aiohttp/test_aiohttp.txt
+-rw-r--r--   0        0        0      420 2024-05-09 09:29:57.022727 cognee-0.1.8/cognee/.data/example/tests/integrations/argv/test_argv.txt
+-rw-r--r--   0        0        0      106 2024-05-09 09:29:57.017767 cognee-0.1.8/cognee/.data/example/tests/integrations/ariadne/__init__.txt
+-rw-r--r--   0        0        0     7492 2024-05-09 09:29:57.017895 cognee-0.1.8/cognee/.data/example/tests/integrations/ariadne/test_ariadne.txt
+-rw-r--r--   0        0        0       42 2024-05-09 09:29:57.029021 cognee-0.1.8/cognee/.data/example/tests/integrations/arq/__init__.txt
+-rw-r--r--   0        0        0     7441 2024-05-09 09:29:57.029147 cognee-0.1.8/cognee/.data/example/tests/integrations/arq/test_arq.txt
+-rw-r--r--   0        0        0      129 2024-05-09 09:29:57.017418 cognee-0.1.8/cognee/.data/example/tests/integrations/asgi/__init__.txt
+-rw-r--r--   0        0        0    19269 2024-05-09 09:29:57.017304 cognee-0.1.8/cognee/.data/example/tests/integrations/asgi/test_asgi.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.033896 cognee-0.1.8/cognee/.data/example/tests/integrations/asyncio/__init__.txt
+-rw-r--r--   0        0        0    10705 2024-05-09 09:29:57.033806 cognee-0.1.8/cognee/.data/example/tests/integrations/asyncio/test_asyncio_py3.txt
+-rw-r--r--   0        0        0      324 2024-05-09 09:29:57.019807 cognee-0.1.8/cognee/.data/example/tests/integrations/asyncpg/__init__.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.019908 cognee-0.1.8/cognee/.data/example/tests/integrations/asyncpg/asyncpg_helpers/__init__.txt
+-rw-r--r--   0        0        0       94 2024-05-09 09:29:57.020039 cognee-0.1.8/cognee/.data/example/tests/integrations/asyncpg/asyncpg_helpers/helpers.txt
+-rw-r--r--   0        0        0    21423 2024-05-09 09:29:57.019699 cognee-0.1.8/cognee/.data/example/tests/integrations/asyncpg/test_asyncpg.txt
+-rw-r--r--   0        0        0       44 2024-05-09 09:29:57.029812 cognee-0.1.8/cognee/.data/example/tests/integrations/aws_lambda/__init__.txt
+-rw-r--r--   0        0        0    12514 2024-05-09 09:29:57.029697 cognee-0.1.8/cognee/.data/example/tests/integrations/aws_lambda/client.txt
+-rw-r--r--   0        0        0    28565 2024-05-09 09:29:57.029563 cognee-0.1.8/cognee/.data/example/tests/integrations/aws_lambda/test_aws.txt
+-rw-r--r--   0        0        0       50 2024-05-09 09:29:57.028442 cognee-0.1.8/cognee/.data/example/tests/integrations/beam/__init__.txt
+-rw-r--r--   0        0        0     5932 2024-05-09 09:29:57.028546 cognee-0.1.8/cognee/.data/example/tests/integrations/beam/test_beam.txt
+-rw-r--r--   0        0        0      230 2024-05-09 09:29:57.035552 cognee-0.1.8/cognee/.data/example/tests/integrations/boto3/__init__.txt
+-rw-r--r--   0        0        0      883 2024-05-09 09:29:57.035756 cognee-0.1.8/cognee/.data/example/tests/integrations/boto3/aws_mock.txt
+-rw-r--r--   0        0        0      869 2024-05-09 09:29:57.035662 cognee-0.1.8/cognee/.data/example/tests/integrations/boto3/s3_list.txt
+-rw-r--r--   0        0        0     4335 2024-05-09 09:29:57.035866 cognee-0.1.8/cognee/.data/example/tests/integrations/boto3/test_s3.txt
+-rw-r--r--   0        0        0       45 2024-05-09 09:29:57.034716 cognee-0.1.8/cognee/.data/example/tests/integrations/bottle/__init__.txt
+-rw-r--r--   0        0        0    12198 2024-05-09 09:29:57.034606 cognee-0.1.8/cognee/.data/example/tests/integrations/bottle/test_bottle.txt
+-rw-r--r--   0        0        0       45 2024-05-09 09:29:57.028760 cognee-0.1.8/cognee/.data/example/tests/integrations/celery/__init__.txt
+-rw-r--r--   0        0        0    18668 2024-05-09 09:29:57.028664 cognee-0.1.8/cognee/.data/example/tests/integrations/celery/test_celery.txt
+-rw-r--r--   0        0        0    16058 2024-05-09 09:29:57.028884 cognee-0.1.8/cognee/.data/example/tests/integrations/celery/test_celery_beat_crons.txt
+-rw-r--r--   0        0        0       46 2024-05-09 09:29:57.025974 cognee-0.1.8/cognee/.data/example/tests/integrations/chalice/__init__.txt
+-rw-r--r--   0        0        0     4389 2024-05-09 09:29:57.026110 cognee-0.1.8/cognee/.data/example/tests/integrations/chalice/test_chalice.txt
+-rw-r--r--   0        0        0       56 2024-05-09 09:29:57.017020 cognee-0.1.8/cognee/.data/example/tests/integrations/clickhouse_driver/__init__.txt
+-rw-r--r--   0        0        0    28896 2024-05-09 09:29:57.017158 cognee-0.1.8/cognee/.data/example/tests/integrations/clickhouse_driver/test_clickhouse_driver.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.035968 cognee-0.1.8/cognee/.data/example/tests/integrations/cloud_resource_context/__init__.txt
+-rw-r--r--   0        0        0    12836 2024-05-09 09:29:57.036097 cognee-0.1.8/cognee/.data/example/tests/integrations/cloud_resource_context/test_cloud_resource_context.txt
+-rw-r--r--   0        0        0      560 2024-05-09 09:29:57.015962 cognee-0.1.8/cognee/.data/example/tests/integrations/conftest.txt
+-rw-r--r--   0        0        0      284 2024-05-09 09:29:57.030192 cognee-0.1.8/cognee/.data/example/tests/integrations/django/__init__.txt
+-rw-r--r--   0        0        0       47 2024-05-09 09:29:57.031017 cognee-0.1.8/cognee/.data/example/tests/integrations/django/asgi/__init__.txt
+-rw-r--r--   0        0        0      308 2024-05-09 09:29:57.031144 cognee-0.1.8/cognee/.data/example/tests/integrations/django/asgi/image.txt
+-rw-r--r--   0        0        0    16055 2024-05-09 09:29:57.030892 cognee-0.1.8/cognee/.data/example/tests/integrations/django/asgi/test_asgi.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.030628 cognee-0.1.8/cognee/.data/example/tests/integrations/django/django_helpers/__init__.txt
+-rw-r--r--   0        0        0      302 2024-05-09 09:29:57.030737 cognee-0.1.8/cognee/.data/example/tests/integrations/django/django_helpers/views.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.031355 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/__init__.txt
+-rw-r--r--   0        0        0      487 2024-05-09 09:29:57.031276 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/asgi.txt
+-rw-r--r--   0        0        0     1020 2024-05-09 09:29:57.031796 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/custom_urls.txt
+-rw-r--r--   0        0        0      284 2024-05-09 09:29:57.031695 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/manage.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.032366 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/management/__init__.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.032465 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/management/commands/__init__.txt
+-rw-r--r--   0        0        0      187 2024-05-09 09:29:57.032577 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/management/commands/mycrash.txt
+-rw-r--r--   0        0        0      784 2024-05-09 09:29:57.032028 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/middleware.txt
+-rw-r--r--   0        0        0      494 2024-05-09 09:29:57.031471 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/routing.txt
+-rw-r--r--   0        0        0     5143 2024-05-09 09:29:57.031582 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/settings.txt
+-rw-r--r--   0        0        0       75 2024-05-09 09:29:57.033264 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/templates/error.txt
+-rw-r--r--   0        0        0       24 2024-05-09 09:29:57.032917 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/templates/trace_meta.txt
+-rw-r--r--   0        0        0       35 2024-05-09 09:29:57.033115 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/templates/user_name.txt
+-rw-r--r--   0        0        0     4349 2024-05-09 09:29:57.031918 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/urls.txt
+-rw-r--r--   0        0        0     6039 2024-05-09 09:29:57.032156 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/views.txt
+-rw-r--r--   0        0        0      419 2024-05-09 09:29:57.032272 cognee-0.1.8/cognee/.data/example/tests/integrations/django/myapp/wsgi.txt
+-rw-r--r--   0        0        0    43217 2024-05-09 09:29:57.029965 cognee-0.1.8/cognee/.data/example/tests/integrations/django/test_basic.txt
+-rw-r--r--   0        0        0     2440 2024-05-09 09:29:57.030078 cognee-0.1.8/cognee/.data/example/tests/integrations/django/test_data_scrubbing.txt
+-rw-r--r--   0        0        0    15173 2024-05-09 09:29:57.030522 cognee-0.1.8/cognee/.data/example/tests/integrations/django/test_db_query_data.txt
+-rw-r--r--   0        0        0     4077 2024-05-09 09:29:57.030290 cognee-0.1.8/cognee/.data/example/tests/integrations/django/test_transactions.txt
+-rw-r--r--   0        0        0      729 2024-05-09 09:29:57.030404 cognee-0.1.8/cognee/.data/example/tests/integrations/django/utils.txt
+-rw-r--r--   0        0        0     1733 2024-05-09 09:29:57.018268 cognee-0.1.8/cognee/.data/example/tests/integrations/excepthook/test_excepthook.txt
+-rw-r--r--   0        0        0       45 2024-05-09 09:29:57.033580 cognee-0.1.8/cognee/.data/example/tests/integrations/falcon/__init__.txt
+-rw-r--r--   0        0        0    12435 2024-05-09 09:29:57.033459 cognee-0.1.8/cognee/.data/example/tests/integrations/falcon/test_falcon.txt
+-rw-r--r--   0        0        0       46 2024-05-09 09:29:57.027067 cognee-0.1.8/cognee/.data/example/tests/integrations/fastapi/__init__.txt
+-rw-r--r--   0        0        0    14337 2024-05-09 09:29:57.026952 cognee-0.1.8/cognee/.data/example/tests/integrations/fastapi/test_fastapi.txt
+-rw-r--r--   0        0        0       44 2024-05-09 09:29:57.016386 cognee-0.1.8/cognee/.data/example/tests/integrations/flask/__init__.txt
+-rw-r--r--   0        0        0    27402 2024-05-09 09:29:57.016489 cognee-0.1.8/cognee/.data/example/tests/integrations/flask/test_flask.txt
+-rw-r--r--   0        0        0    17513 2024-05-09 09:29:57.024038 cognee-0.1.8/cognee/.data/example/tests/integrations/gcp/test_gcp.txt
+-rw-r--r--   0        0        0       42 2024-05-09 09:29:57.021775 cognee-0.1.8/cognee/.data/example/tests/integrations/gql/__init__.txt
+-rw-r--r--   0        0        0     7366 2024-05-09 09:29:57.021884 cognee-0.1.8/cognee/.data/example/tests/integrations/gql/test_gql.txt
+-rw-r--r--   0        0        0      107 2024-05-09 09:29:57.026643 cognee-0.1.8/cognee/.data/example/tests/integrations/graphene/__init__.txt
+-rw-r--r--   0        0        0     5663 2024-05-09 09:29:57.026783 cognee-0.1.8/cognee/.data/example/tests/integrations/graphene/test_graphene_py3.txt
+-rw-r--r--   0        0        0      177 2024-05-09 09:29:57.018972 cognee-0.1.8/cognee/.data/example/tests/integrations/grpc/__init__.txt
+-rw-r--r--   0        0        0      403 2024-05-09 09:29:57.019314 cognee-0.1.8/cognee/.data/example/tests/integrations/grpc/compile_test_services.txt
+-rw-r--r--   0        0        0     1608 2024-05-09 09:29:57.019197 cognee-0.1.8/cognee/.data/example/tests/integrations/grpc/grpc_test_service_pb2.txt
+-rw-r--r--   0        0        0     7557 2024-05-09 09:29:57.019100 cognee-0.1.8/cognee/.data/example/tests/integrations/grpc/grpc_test_service_pb2_grpc.txt
+-rw-r--r--   0        0        0      409 2024-05-09 09:29:57.019566 cognee-0.1.8/cognee/.data/example/tests/integrations/grpc/protos/grpc_test_service.txt
+-rw-r--r--   0        0        0    10556 2024-05-09 09:29:57.018737 cognee-0.1.8/cognee/.data/example/tests/integrations/grpc/test_grpc.txt
+-rw-r--r--   0        0        0     8185 2024-05-09 09:29:57.019428 cognee-0.1.8/cognee/.data/example/tests/integrations/grpc/test_grpc_aio.txt
+-rw-r--r--   0        0        0       44 2024-05-09 09:29:57.026263 cognee-0.1.8/cognee/.data/example/tests/integrations/httpx/__init__.txt
+-rw-r--r--   0        0        0     8965 2024-05-09 09:29:57.026483 cognee-0.1.8/cognee/.data/example/tests/integrations/httpx/test_httpx.txt
+-rw-r--r--   0        0        0       43 2024-05-09 09:29:57.022292 cognee-0.1.8/cognee/.data/example/tests/integrations/huey/__init__.txt
+-rw-r--r--   0        0        0     5071 2024-05-09 09:29:57.022163 cognee-0.1.8/cognee/.data/example/tests/integrations/huey/test_huey.txt
+-rw-r--r--   0        0        0     6912 2024-05-09 09:29:57.034033 cognee-0.1.8/cognee/.data/example/tests/integrations/logging/test_logging.txt
+-rw-r--r--   0        0        0       45 2024-05-09 09:29:57.027978 cognee-0.1.8/cognee/.data/example/tests/integrations/loguru/__init__.txt
+-rw-r--r--   0        0        0     3266 2024-05-09 09:29:57.027868 cognee-0.1.8/cognee/.data/example/tests/integrations/loguru/test_loguru.txt
+-rw-r--r--   0        0        0      367 2024-05-09 09:29:57.029424 cognee-0.1.8/cognee/.data/example/tests/integrations/modules/test_modules.txt
+-rw-r--r--   0        0        0       45 2024-05-09 09:29:57.035193 cognee-0.1.8/cognee/.data/example/tests/integrations/openai/__init__.txt
+-rw-r--r--   0        0        0     7535 2024-05-09 09:29:57.035087 cognee-0.1.8/cognee/.data/example/tests/integrations/openai/test_openai.txt
+-rw-r--r--   0        0        0       52 2024-05-09 09:29:57.021548 cognee-0.1.8/cognee/.data/example/tests/integrations/opentelemetry/__init__.txt
+-rw-r--r--   0        0        0      993 2024-05-09 09:29:57.021650 cognee-0.1.8/cognee/.data/example/tests/integrations/opentelemetry/test_experimental.txt
+-rw-r--r--   0        0        0     7951 2024-05-09 09:29:57.021447 cognee-0.1.8/cognee/.data/example/tests/integrations/opentelemetry/test_propagator.txt
+-rw-r--r--   0        0        0    21486 2024-05-09 09:29:57.021335 cognee-0.1.8/cognee/.data/example/tests/integrations/opentelemetry/test_span_processor.txt
+-rw-r--r--   0        0        0       48 2024-05-09 09:29:57.018031 cognee-0.1.8/cognee/.data/example/tests/integrations/pure_eval/__init__.txt
+-rw-r--r--   0        0        0     2445 2024-05-09 09:29:57.018140 cognee-0.1.8/cognee/.data/example/tests/integrations/pure_eval/test_pure_eval.txt
+-rw-r--r--   0        0        0       46 2024-05-09 09:29:57.024908 cognee-0.1.8/cognee/.data/example/tests/integrations/pymongo/__init__.txt
+-rw-r--r--   0        0        0    14425 2024-05-09 09:29:57.024783 cognee-0.1.8/cognee/.data/example/tests/integrations/pymongo/test_pymongo.txt
+-rw-r--r--   0        0        0       46 2024-05-09 09:29:57.023114 cognee-0.1.8/cognee/.data/example/tests/integrations/pyramid/__init__.txt
+-rw-r--r--   0        0        0    11072 2024-05-09 09:29:57.022983 cognee-0.1.8/cognee/.data/example/tests/integrations/pyramid/test_pyramid.txt
+-rw-r--r--   0        0        0       44 2024-05-09 09:29:57.022440 cognee-0.1.8/cognee/.data/example/tests/integrations/quart/__init__.txt
+-rw-r--r--   0        0        0    14540 2024-05-09 09:29:57.022568 cognee-0.1.8/cognee/.data/example/tests/integrations/quart/test_quart.txt
+-rw-r--r--   0        0        0       44 2024-05-09 09:29:57.020398 cognee-0.1.8/cognee/.data/example/tests/integrations/redis/__init__.txt
+-rw-r--r--   0        0        0       57 2024-05-09 09:29:57.021036 cognee-0.1.8/cognee/.data/example/tests/integrations/redis/asyncio/__init__.txt
+-rw-r--r--   0        0        0     2423 2024-05-09 09:29:57.021170 cognee-0.1.8/cognee/.data/example/tests/integrations/redis/asyncio/test_redis_asyncio.txt
+-rw-r--r--   0        0        0       52 2024-05-09 09:29:57.020530 cognee-0.1.8/cognee/.data/example/tests/integrations/redis/cluster/__init__.txt
+-rw-r--r--   0        0        0     4441 2024-05-09 09:29:57.020647 cognee-0.1.8/cognee/.data/example/tests/integrations/redis/cluster/test_redis_cluster.txt
+-rw-r--r--   0        0        0       60 2024-05-09 09:29:57.020778 cognee-0.1.8/cognee/.data/example/tests/integrations/redis/cluster_asyncio/__init__.txt
+-rw-r--r--   0        0        0     4188 2024-05-09 09:29:57.020894 cognee-0.1.8/cognee/.data/example/tests/integrations/redis/cluster_asyncio/test_redis_cluster_asyncio.txt
+-rw-r--r--   0        0        0     9022 2024-05-09 09:29:57.020291 cognee-0.1.8/cognee/.data/example/tests/integrations/redis/test_redis.txt
+-rw-r--r--   0        0        0       51 2024-05-09 09:29:57.018400 cognee-0.1.8/cognee/.data/example/tests/integrations/rediscluster/__init__.txt
+-rw-r--r--   0        0        0     5016 2024-05-09 09:29:57.018513 cognee-0.1.8/cognee/.data/example/tests/integrations/rediscluster/test_rediscluster.txt
+-rw-r--r--   0        0        0       47 2024-05-09 09:29:57.025377 cognee-0.1.8/cognee/.data/example/tests/integrations/requests/__init__.txt
+-rw-r--r--   0        0        0     2061 2024-05-09 09:29:57.025513 cognee-0.1.8/cognee/.data/example/tests/integrations/requests/test_requests.txt
+-rw-r--r--   0        0        0       41 2024-05-09 09:29:57.034380 cognee-0.1.8/cognee/.data/example/tests/integrations/rq/__init__.txt
+-rw-r--r--   0        0        0     8582 2024-05-09 09:29:57.034258 cognee-0.1.8/cognee/.data/example/tests/integrations/rq/test_rq.txt
+-rw-r--r--   0        0        0       44 2024-05-09 09:29:57.027210 cognee-0.1.8/cognee/.data/example/tests/integrations/sanic/__init__.txt
+-rw-r--r--   0        0        0    13506 2024-05-09 09:29:57.027348 cognee-0.1.8/cognee/.data/example/tests/integrations/sanic/test_sanic.txt
+-rw-r--r--   0        0        0     1042 2024-05-09 09:29:57.022011 cognee-0.1.8/cognee/.data/example/tests/integrations/serverless/test_serverless.txt
+-rw-r--r--   0        0        0       45 2024-05-09 09:29:57.035431 cognee-0.1.8/cognee/.data/example/tests/integrations/socket/__init__.txt
+-rw-r--r--   0        0        0     1641 2024-05-09 09:29:57.035327 cognee-0.1.8/cognee/.data/example/tests/integrations/socket/test_socket.txt
+-rw-r--r--   0        0        0       74 2024-05-09 09:29:57.034953 cognee-0.1.8/cognee/.data/example/tests/integrations/spark/__init__.txt
+-rw-r--r--   0        0        0     6598 2024-05-09 09:29:57.034849 cognee-0.1.8/cognee/.data/example/tests/integrations/spark/test_spark.txt
+-rw-r--r--   0        0        0      292 2024-05-09 09:29:57.024338 cognee-0.1.8/cognee/.data/example/tests/integrations/sqlalchemy/__init__.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.024459 cognee-0.1.8/cognee/.data/example/tests/integrations/sqlalchemy/sqlalchemy_helpers/__init__.txt
+-rw-r--r--   0        0        0      192 2024-05-09 09:29:57.024603 cognee-0.1.8/cognee/.data/example/tests/integrations/sqlalchemy/sqlalchemy_helpers/helpers.txt
+-rw-r--r--   0        0        0    21401 2024-05-09 09:29:57.024205 cognee-0.1.8/cognee/.data/example/tests/integrations/sqlalchemy/test_sqlalchemy.txt
+-rw-r--r--   0        0        0       48 2024-05-09 09:29:57.023271 cognee-0.1.8/cognee/.data/example/tests/integrations/starlette/__init__.txt
+-rw-r--r--   0        0        0    21014 2024-05-09 09:29:57.023405 cognee-0.1.8/cognee/.data/example/tests/integrations/starlette/photo.txt
+-rw-r--r--   0        0        0       24 2024-05-09 09:29:57.023706 cognee-0.1.8/cognee/.data/example/tests/integrations/starlette/templates/trace_meta.txt
+-rw-r--r--   0        0        0    35093 2024-05-09 09:29:57.023542 cognee-0.1.8/cognee/.data/example/tests/integrations/starlette/test_starlette.txt
+-rw-r--r--   0        0        0       47 2024-05-09 09:29:57.028320 cognee-0.1.8/cognee/.data/example/tests/integrations/starlite/__init__.txt
+-rw-r--r--   0        0        0     9647 2024-05-09 09:29:57.028209 cognee-0.1.8/cognee/.data/example/tests/integrations/starlite/test_starlite.txt
+-rw-r--r--   0        0        0    10655 2024-05-09 09:29:57.027727 cognee-0.1.8/cognee/.data/example/tests/integrations/stdlib/test_httplib.txt
+-rw-r--r--   0        0        0     5045 2024-05-09 09:29:57.027509 cognee-0.1.8/cognee/.data/example/tests/integrations/stdlib/test_subprocess.txt
+-rw-r--r--   0        0        0        0 2024-05-09 09:29:57.017516 cognee-0.1.8/cognee/.data/example/tests/integrations/strawberry/__init__.txt
+-rw-r--r--   0        0        0    19273 2024-05-09 09:29:57.017631 cognee-0.1.8/cognee/.data/example/tests/integrations/strawberry/test_strawberry_py3.txt
+-rw-r--r--   0        0        0    10881 2024-05-09 09:29:57.016250 cognee-0.1.8/cognee/.data/example/tests/integrations/test_gnu_backtrace.txt
+-rw-r--r--   0        0        0     5769 2024-05-09 09:29:57.029284 cognee-0.1.8/cognee/.data/example/tests/integrations/threading/test_threading.txt
+-rw-r--r--   0        0        0       46 2024-05-09 09:29:57.025691 cognee-0.1.8/cognee/.data/example/tests/integrations/tornado/__init__.txt
+-rw-r--r--   0        0        0    13348 2024-05-09 09:29:57.025828 cognee-0.1.8/cognee/.data/example/tests/integrations/tornado/test_tornado.txt
+-rw-r--r--   0        0        0       46 2024-05-09 09:29:57.025073 cognee-0.1.8/cognee/.data/example/tests/integrations/trytond/__init__.txt
+-rw-r--r--   0        0        0     3584 2024-05-09 09:29:57.025212 cognee-0.1.8/cognee/.data/example/tests/integrations/trytond/test_trytond.txt
+-rw-r--r--   0        0        0    13237 2024-05-09 09:29:57.023890 cognee-0.1.8/cognee/.data/example/tests/integrations/wsgi/test_wsgi.txt
+-rw-r--r--   0        0        0     3681 2024-05-09 09:29:57.013923 cognee-0.1.8/cognee/.data/example/tests/test_api.txt
+-rw-r--r--   0        0        0    23643 2024-05-09 09:29:57.012396 cognee-0.1.8/cognee/.data/example/tests/test_basics.txt
+-rw-r--r--   0        0        0    41119 2024-05-09 09:29:57.014041 cognee-0.1.8/cognee/.data/example/tests/test_client.txt
+-rw-r--r--   0        0        0     3417 2024-05-09 09:29:57.012616 cognee-0.1.8/cognee/.data/example/tests/test_conftest.txt
+-rw-r--r--   0        0        0     8137 2024-05-09 09:29:57.013721 cognee-0.1.8/cognee/.data/example/tests/test_envelope.txt
+-rw-r--r--   0        0        0     8578 2024-05-09 09:29:57.013472 cognee-0.1.8/cognee/.data/example/tests/test_exceptiongroup.txt
+-rw-r--r--   0        0        0      784 2024-05-09 09:29:57.013826 cognee-0.1.8/cognee/.data/example/tests/test_lru_cache.txt
+-rw-r--r--   0        0        0    31466 2024-05-09 09:29:57.012506 cognee-0.1.8/cognee/.data/example/tests/test_metrics.txt
+-rw-r--r--   0        0        0     2702 2024-05-09 09:29:57.011977 cognee-0.1.8/cognee/.data/example/tests/test_monitor.txt
+-rw-r--r--   0        0        0    24427 2024-05-09 09:29:57.013272 cognee-0.1.8/cognee/.data/example/tests/test_profiler.txt
+-rw-r--r--   0        0        0     4058 2024-05-09 09:29:57.012951 cognee-0.1.8/cognee/.data/example/tests/test_scope.txt
+-rw-r--r--   0        0        0     5357 2024-05-09 09:29:57.012302 cognee-0.1.8/cognee/.data/example/tests/test_scrubber.txt
+-rw-r--r--   0        0        0     4816 2024-05-09 09:29:57.012842 cognee-0.1.8/cognee/.data/example/tests/test_serializer.txt
+-rw-r--r--   0        0        0     4184 2024-05-09 09:29:57.012737 cognee-0.1.8/cognee/.data/example/tests/test_sessions.txt
+-rw-r--r--   0        0        0     1490 2024-05-09 09:29:57.013600 cognee-0.1.8/cognee/.data/example/tests/test_spotlight.txt
+-rw-r--r--   0        0        0    18416 2024-05-09 09:29:57.013163 cognee-0.1.8/cognee/.data/example/tests/test_transport.txt
+-rw-r--r--   0        0        0      760 2024-05-09 09:29:57.014146 cognee-0.1.8/cognee/.data/example/tests/test_types.txt
+-rw-r--r--   0        0        0    22888 2024-05-09 09:29:57.012082 cognee-0.1.8/cognee/.data/example/tests/test_utils.txt
+-rw-r--r--   0        0        0     2699 2024-05-09 09:29:57.015252 cognee-0.1.8/cognee/.data/example/tests/tracing/test_baggage.txt
+-rw-r--r--   0        0        0     1820 2024-05-09 09:29:57.014647 cognee-0.1.8/cognee/.data/example/tests/tracing/test_decorator_async_py3.txt
+-rw-r--r--   0        0        0     1665 2024-05-09 09:29:57.015353 cognee-0.1.8/cognee/.data/example/tests/tracing/test_decorator_sync.txt
+-rw-r--r--   0        0        0      575 2024-05-09 09:29:57.014757 cognee-0.1.8/cognee/.data/example/tests/tracing/test_deprecated.txt
+-rw-r--r--   0        0        0     1813 2024-05-09 09:29:57.014855 cognee-0.1.8/cognee/.data/example/tests/tracing/test_http_headers.txt
+-rw-r--r--   0        0        0     9610 2024-05-09 09:29:57.014389 cognee-0.1.8/cognee/.data/example/tests/tracing/test_integration_tests.txt
+-rw-r--r--   0        0        0    12757 2024-05-09 09:29:57.014533 cognee-0.1.8/cognee/.data/example/tests/tracing/test_misc.txt
+-rw-r--r--   0        0        0     1792 2024-05-09 09:29:57.014957 cognee-0.1.8/cognee/.data/example/tests/tracing/test_noop_span.txt
+-rw-r--r--   0        0        0    10643 2024-05-09 09:29:57.015148 cognee-0.1.8/cognee/.data/example/tests/tracing/test_sampling.txt
+-rw-r--r--   0        0        0       40 2024-05-09 09:29:57.015690 cognee-0.1.8/cognee/.data/example/tests/utils/__init__.txt
+-rw-r--r--   0        0        0      797 2024-05-09 09:29:57.015572 cognee-0.1.8/cognee/.data/example/tests/utils/test_contextvars.txt
+-rw-r--r--   0        0        0    17196 2024-05-09 09:29:57.015804 cognee-0.1.8/cognee/.data/example/tests/utils/test_general.txt
+-rw-r--r--   0        0        0     1539 2024-05-09 09:29:57.015472 cognee-0.1.8/cognee/.data/example/tests/utils/test_transaction.txt
+-rw-r--r--   0        0        0    20053 2024-05-09 09:29:57.011668 cognee-0.1.8/cognee/.data/example/tox.txt
+-rw-r--r--   0        0        0      123 2024-04-23 06:52:58.178501 cognee-0.1.8/cognee/.data/example_dataset/271fd0a1a088575885fddc726c4dba04.txt
+-rw-r--r--   0        0        0      426 2024-05-21 06:59:15.075082 cognee-0.1.8/cognee/.data/example_dataset/8e944490a15f563780e6c3f040880b19.txt
+-rw-r--r--   0        0        0     3087 2024-04-02 07:24:38.404088 cognee-0.1.8/cognee/.data/explanations/062c22df-d99b-599f-90cd-2d325c8bcf69.txt
+-rw-r--r--   0        0        0     9041 2024-04-23 07:36:22.827937 cognee-0.1.8/cognee/.data/explanations/6dfe01b6-07d2-5b77-83c8-1d6c11ce2aa7.txt
+-rw-r--r--   0        0        0      985 2024-03-30 19:01:36.385908 cognee-0.1.8/cognee/.data/explanations/Natural language processing.txt
+-rw-r--r--   0        0        0       51 2024-04-18 08:17:53.704561 cognee-0.1.8/cognee/.data/explanations/bab90046-1d9b-598c-8711-dab30f501915.txt
+-rw-r--r--   0        0        0       36 2024-05-21 09:16:37.925545 cognee-0.1.8/cognee/.data/initial_test/14a27354cb3f50ffaaace292d5b7aa58.txt
+-rw-r--r--   0        0        0       44 2024-05-21 09:16:37.923975 cognee-0.1.8/cognee/.data/initial_test/15a66b1d75a45fbfa2d5f8d7b2506d88.txt
+-rw-r--r--   0        0        0       58 2024-05-21 09:16:37.924807 cognee-0.1.8/cognee/.data/initial_test/a881954da33b5e3c8bcf1bc63e50ae20.txt
+-rw-r--r--   0        0        0      186 2024-04-29 18:24:10.776372 cognee-0.1.8/cognee/.data/test/e6ac18788c6a51dfaaf9b963d5bc094b.txt
+-rw-r--r--   0        0        0      249 2024-04-23 05:20:06.890311 cognee-0.1.8/cognee/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.230717 cognee-0.1.8/cognee/api/__init__.py
+-rw-r--r--   0        0        0     8753 2024-05-27 05:37:00.861835 cognee-0.1.8/cognee/api/client.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.230960 cognee-0.1.8/cognee/api/v1/__init__.py
+-rw-r--r--   0        0        0       21 2024-03-14 09:23:35.231099 cognee-0.1.8/cognee/api/v1/add/__init__.py
+-rw-r--r--   0        0        0     5216 2024-05-26 19:03:19.264649 cognee-0.1.8/cognee/api/v1/add/add.py
+-rw-r--r--   0        0        0     1629 2024-05-26 19:03:19.265636 cognee-0.1.8/cognee/api/v1/add/add_standalone.py
+-rw-r--r--   0        0        0      626 2024-03-29 12:59:22.978997 cognee-0.1.8/cognee/api/v1/add/remember.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.234848 cognee-0.1.8/cognee/api/v1/cognify/__init__.py
+-rw-r--r--   0        0        0    12092 2024-05-27 05:37:00.862456 cognee-0.1.8/cognee/api/v1/cognify/cognify.py
+-rw-r--r--   0        0        0     6884 2024-04-25 08:56:45.148041 cognee-0.1.8/cognee/api/v1/cognify/tst.py
+-rw-r--r--   0        0        0       27 2024-03-29 12:59:22.979399 cognee-0.1.8/cognee/api/v1/config/__init__.py
+-rw-r--r--   0        0        0     2552 2024-05-27 05:37:00.864513 cognee-0.1.8/cognee/api/v1/config/config.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.235161 cognee-0.1.8/cognee/api/v1/datasets/__init__.py
+-rw-r--r--   0        0        0     1184 2024-05-27 05:37:00.864752 cognee-0.1.8/cognee/api/v1/datasets/datasets.py
+-rw-r--r--   0        0        0       25 2024-04-23 05:20:06.891056 cognee-0.1.8/cognee/api/v1/prune/__init__.py
+-rw-r--r--   0        0        0     1236 2024-05-26 19:03:19.266837 cognee-0.1.8/cognee/api/v1/prune/prune.py
+-rw-r--r--   0        0        0       39 2024-03-21 16:01:22.628858 cognee-0.1.8/cognee/api/v1/search/__init__.py
+-rw-r--r--   0        0        0     3973 2024-05-26 19:03:19.267387 cognee-0.1.8/cognee/api/v1/search/search.py
+-rw-r--r--   0        0        0        0 2024-05-25 06:16:34.118332 cognee-0.1.8/cognee/api/v1/topology/__init__.py
+-rw-r--r--   0        0        0     3845 2024-05-26 19:03:19.267657 cognee-0.1.8/cognee/api/v1/topology/add_topology.py
+-rw-r--r--   0        0        0     2836 2024-05-19 13:52:43.158383 cognee-0.1.8/cognee/api/v1/topology/rrrr.py
+-rw-r--r--   0        0        0      781 2024-05-27 05:37:00.865047 cognee-0.1.8/cognee/base_config.py
+-rw-r--r--   0        0        0     5730 2024-05-26 19:03:19.268694 cognee-0.1.8/cognee/config.py
+-rw-r--r--   0        0        0     1778 2024-04-28 19:24:05.618264 cognee-0.1.8/cognee/fetch_secret.py
+-rw-r--r--   0        0        0     7145 2024-05-27 05:37:00.865343 cognee-0.1.8/cognee/infrastructure/InfrastructureConfig.py
+-rw-r--r--   0        0        0       56 2024-03-14 09:23:35.235336 cognee-0.1.8/cognee/infrastructure/__init__.py
+-rw-r--r--   0        0        0      110 2024-03-29 12:59:22.980107 cognee-0.1.8/cognee/infrastructure/data/__init__.py
+-rw-r--r--   0        0        0     4457 2024-05-25 06:16:34.119439 cognee-0.1.8/cognee/infrastructure/data/chunking/DefaultChunkEngine.py
+-rw-r--r--   0        0        0        0 2024-05-25 06:16:34.119461 cognee-0.1.8/cognee/infrastructure/data/chunking/HaystackChunkEngine.py
+-rw-r--r--   0        0        0     1661 2024-05-25 06:16:34.119789 cognee-0.1.8/cognee/infrastructure/data/chunking/LangchainChunkingEngine.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.236173 cognee-0.1.8/cognee/infrastructure/data/chunking/__init__.py
+-rw-r--r--   0        0        0      763 2024-05-26 19:03:19.270005 cognee-0.1.8/cognee/infrastructure/data/chunking/config.py
+-rw-r--r--   0        0        0      889 2024-03-14 09:23:35.235567 cognee-0.1.8/cognee/infrastructure/data/models/Data.py
+-rw-r--r--   0        0        0      721 2024-03-14 09:23:35.235631 cognee-0.1.8/cognee/infrastructure/data/models/Dataset.py
+-rw-r--r--   0        0        0      553 2024-03-14 09:23:35.235756 cognee-0.1.8/cognee/infrastructure/data/models/DatasetData.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.235800 cognee-0.1.8/cognee/infrastructure/data/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.236240 cognee-0.1.8/cognee/infrastructure/data/utils/__init__.py
+-rw-r--r--   0        0        0      756 2024-04-23 05:20:06.895346 cognee-0.1.8/cognee/infrastructure/data/utils/extract_keywords.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.235884 cognee-0.1.8/cognee/infrastructure/databases/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.235957 cognee-0.1.8/cognee/infrastructure/databases/graph/__init__.py
+-rw-r--r--   0        0        0     1640 2024-05-26 19:03:19.270423 cognee-0.1.8/cognee/infrastructure/databases/graph/config.py
+-rw-r--r--   0        0        0        0 2024-05-25 06:16:34.119846 cognee-0.1.8/cognee/infrastructure/databases/graph/falkordb/__init__.py
+-rw-r--r--   0        0        0     6177 2024-05-25 06:16:34.120113 cognee-0.1.8/cognee/infrastructure/databases/graph/falkordb/adapter.py
+-rw-r--r--   0        0        0     1553 2024-05-26 19:03:19.271191 cognee-0.1.8/cognee/infrastructure/databases/graph/get_graph_client.py
+-rw-r--r--   0        0        0     1162 2024-04-23 05:20:06.895582 cognee-0.1.8/cognee/infrastructure/databases/graph/graph_db_interface.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:20:06.895611 cognee-0.1.8/cognee/infrastructure/databases/graph/neo4j_driver/__init__.py
+-rw-r--r--   0        0        0     6154 2024-05-26 19:03:19.271548 cognee-0.1.8/cognee/infrastructure/databases/graph/neo4j_driver/adapter.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.236389 cognee-0.1.8/cognee/infrastructure/databases/graph/networkx/__init__.py
+-rw-r--r--   0        0        0     5360 2024-05-25 06:16:34.120573 cognee-0.1.8/cognee/infrastructure/databases/graph/networkx/adapter.py
+-rw-r--r--   0        0        0      462 2024-03-14 09:23:35.236879 cognee-0.1.8/cognee/infrastructure/databases/relational/DatabaseEngine.py
+-rw-r--r--   0        0        0       76 2024-03-14 09:23:35.236991 cognee-0.1.8/cognee/infrastructure/databases/relational/ModelBase.py
+-rw-r--r--   0        0        0      170 2024-03-14 09:23:35.237089 cognee-0.1.8/cognee/infrastructure/databases/relational/__init__.py
+-rw-r--r--   0        0        0     1353 2024-05-27 05:37:00.865581 cognee-0.1.8/cognee/infrastructure/databases/relational/config.py
+-rw-r--r--   0        0        0     6666 2024-05-27 05:37:00.866108 cognee-0.1.8/cognee/infrastructure/databases/relational/duckdb/DuckDBAdapter.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.237764 cognee-0.1.8/cognee/infrastructure/databases/relational/duckdb/__init__.py
+-rw-r--r--   0        0        0     1006 2024-03-14 09:23:35.237616 cognee-0.1.8/cognee/infrastructure/databases/relational/relational_db_interface.py
+-rw-r--r--   0        0        0     2847 2024-03-14 09:23:35.237690 cognee-0.1.8/cognee/infrastructure/databases/relational/sqlite/SqliteEngine.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.237716 cognee-0.1.8/cognee/infrastructure/databases/relational/sqlite/__init__.py
+-rw-r--r--   0        0        0       41 2024-03-14 09:23:35.237829 cognee-0.1.8/cognee/infrastructure/databases/relational/utils/__init__.py
+-rw-r--r--   0        0        0      595 2024-03-14 09:23:35.237896 cognee-0.1.8/cognee/infrastructure/databases/relational/utils/with_rollback.py
+-rw-r--r--   0        0        0      230 2024-05-27 05:37:00.866399 cognee-0.1.8/cognee/infrastructure/databases/vector/__init__.py
+-rw-r--r--   0        0        0     1549 2024-05-27 05:37:00.866518 cognee-0.1.8/cognee/infrastructure/databases/vector/config.py
+-rw-r--r--   0        0        0     1368 2024-05-27 05:37:00.866669 cognee-0.1.8/cognee/infrastructure/databases/vector/create_vector_engine.py
+-rw-r--r--   0        0        0     2381 2024-05-26 19:03:19.273200 cognee-0.1.8/cognee/infrastructure/databases/vector/embeddings/DefaultEmbeddingEngine.py
+-rw-r--r--   0        0        0      243 2024-05-25 06:16:34.121382 cognee-0.1.8/cognee/infrastructure/databases/vector/embeddings/EmbeddingEngine.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.237831 cognee-0.1.8/cognee/infrastructure/databases/vector/embeddings/__init__.py
+-rw-r--r--   0        0        0     1091 2024-05-26 19:03:19.273824 cognee-0.1.8/cognee/infrastructure/databases/vector/embeddings/config.py
+-rw-r--r--   0        0        0     1474 2024-05-26 19:03:19.274145 cognee-0.1.8/cognee/infrastructure/databases/vector/falkordb/FalkorDBAdapter.py
+-rw-r--r--   0        0        0     5331 2024-05-25 06:16:34.121496 cognee-0.1.8/cognee/infrastructure/databases/vector/lancedb/LanceDBAdapter.py
+-rw-r--r--   0        0        0        0 2024-05-25 06:16:34.121519 cognee-0.1.8/cognee/infrastructure/databases/vector/lancedb/__init__.py
+-rw-r--r--   0        0        0      138 2024-03-21 16:01:22.631437 cognee-0.1.8/cognee/infrastructure/databases/vector/models/CollectionConfig.py
+-rw-r--r--   0        0        0      398 2024-05-25 06:16:34.121821 cognee-0.1.8/cognee/infrastructure/databases/vector/models/DataPoint.py
+-rw-r--r--   0        0        0       69 2024-05-25 06:16:34.122276 cognee-0.1.8/cognee/infrastructure/databases/vector/models/PayloadSchema.py
+-rw-r--r--   0        0        0      171 2024-03-21 16:01:22.632343 cognee-0.1.8/cognee/infrastructure/databases/vector/models/ScoredResult.py
+-rw-r--r--   0        0        0      143 2024-03-21 16:01:22.633028 cognee-0.1.8/cognee/infrastructure/databases/vector/models/VectorConfig.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.238226 cognee-0.1.8/cognee/infrastructure/databases/vector/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.238287 cognee-0.1.8/cognee/infrastructure/databases/vector/pinecone/__init__.py
+-rw-r--r--   0        0        0      256 2024-03-14 09:23:35.238527 cognee-0.1.8/cognee/infrastructure/databases/vector/pinecone/adapter.py
+-rw-r--r--   0        0        0     6652 2024-05-25 06:16:34.122417 cognee-0.1.8/cognee/infrastructure/databases/vector/qdrant/QDrantAdapter.py
+-rw-r--r--   0        0        0       96 2024-04-23 05:20:06.897060 cognee-0.1.8/cognee/infrastructure/databases/vector/qdrant/__init__.py
+-rw-r--r--   0        0        0     1362 2024-05-25 06:16:34.122602 cognee-0.1.8/cognee/infrastructure/databases/vector/vector_db_interface.py
+-rw-r--r--   0        0        0     4548 2024-05-25 06:16:34.122724 cognee-0.1.8/cognee/infrastructure/databases/vector/weaviate_db/WeaviateAdapter.py
+-rw-r--r--   0        0        0       45 2024-03-21 16:01:22.635439 cognee-0.1.8/cognee/infrastructure/databases/vector/weaviate_db/__init__.py
+-rw-r--r--   0        0        0      185 2024-03-14 09:23:35.239234 cognee-0.1.8/cognee/infrastructure/files/__init__.py
+-rw-r--r--   0        0        0      364 2024-03-14 09:23:35.239315 cognee-0.1.8/cognee/infrastructure/files/add_file_to_storage.py
+-rw-r--r--   0        0        0      320 2024-03-14 09:23:35.239384 cognee-0.1.8/cognee/infrastructure/files/remove_file_from_storage.py
+-rw-r--r--   0        0        0     1549 2024-05-25 06:16:34.122827 cognee-0.1.8/cognee/infrastructure/files/storage/LocalStorage.py
+-rw-r--r--   0        0        0      640 2024-03-14 09:23:35.239533 cognee-0.1.8/cognee/infrastructure/files/storage/StorageManager.py
+-rw-r--r--   0        0        0       39 2024-03-14 09:23:35.239601 cognee-0.1.8/cognee/infrastructure/files/storage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.239635 cognee-0.1.8/cognee/infrastructure/files/utils/__init__.py
+-rw-r--r--   0        0        0      427 2024-05-26 19:03:19.274436 cognee-0.1.8/cognee/infrastructure/files/utils/extract_text_from_file.py
+-rw-r--r--   0        0        0     1001 2024-05-26 19:03:19.274786 cognee-0.1.8/cognee/infrastructure/files/utils/get_file_metadata.py
+-rw-r--r--   0        0        0      117 2024-05-26 19:03:19.275134 cognee-0.1.8/cognee/infrastructure/files/utils/get_file_size.py
+-rw-r--r--   0        0        0     1144 2024-05-26 19:03:19.286545 cognee-0.1.8/cognee/infrastructure/files/utils/guess_file_type.py
+-rw-r--r--   0        0        0      865 2024-05-26 19:03:19.286780 cognee-0.1.8/cognee/infrastructure/files/utils/is_text_content.py
+-rw-r--r--   0        0        0       35 2024-05-26 19:03:19.287399 cognee-0.1.8/cognee/infrastructure/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-29 12:59:22.982620 cognee-0.1.8/cognee/infrastructure/llm/anthropic/__init__.py
+-rw-r--r--   0        0        0     1807 2024-05-25 06:16:34.123242 cognee-0.1.8/cognee/infrastructure/llm/anthropic/adapter.py
+-rw-r--r--   0        0        0      597 2024-05-26 19:03:19.287741 cognee-0.1.8/cognee/infrastructure/llm/config.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.238931 cognee-0.1.8/cognee/infrastructure/llm/generic_llm_api/__init__.py
+-rw-r--r--   0        0        0     5423 2024-05-26 19:03:19.288073 cognee-0.1.8/cognee/infrastructure/llm/generic_llm_api/adapter.py
+-rw-r--r--   0        0        0     1296 2024-05-27 05:37:00.866830 cognee-0.1.8/cognee/infrastructure/llm/get_llm_client.py
+-rw-r--r--   0        0        0      738 2024-05-26 19:03:19.289342 cognee-0.1.8/cognee/infrastructure/llm/llm_interface.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.240172 cognee-0.1.8/cognee/infrastructure/llm/openai/__init__.py
+-rw-r--r--   0        0        0     5562 2024-05-26 19:03:19.289967 cognee-0.1.8/cognee/infrastructure/llm/openai/adapter.py
+-rw-r--r--   0        0        0       90 2024-03-21 16:01:22.637734 cognee-0.1.8/cognee/infrastructure/llm/prompts/__init__.py
+-rw-r--r--   0        0        0      112 2024-05-25 06:16:34.123926 cognee-0.1.8/cognee/infrastructure/llm/prompts/categorize_categories.txt
+-rw-r--r--   0        0        0      110 2024-05-25 06:16:34.124196 cognee-0.1.8/cognee/infrastructure/llm/prompts/categorize_summary.txt
+-rw-r--r--   0        0        0     5614 2024-03-29 12:59:14.138687 cognee-0.1.8/cognee/infrastructure/llm/prompts/classify_content.txt
+-rw-r--r--   0        0        0      348 2024-05-25 06:16:34.124497 cognee-0.1.8/cognee/infrastructure/llm/prompts/extract_topology.txt
+-rw-r--r--   0        0        0     1323 2024-04-23 05:20:06.898436 cognee-0.1.8/cognee/infrastructure/llm/prompts/generate_cog_layers.txt
+-rw-r--r--   0        0        0     2192 2024-04-23 05:20:06.898603 cognee-0.1.8/cognee/infrastructure/llm/prompts/generate_graph_prompt.txt
+-rw-r--r--   0        0        0      613 2024-03-21 16:01:22.638556 cognee-0.1.8/cognee/infrastructure/llm/prompts/read_query_prompt.py
+-rw-r--r--   0        0        0      962 2024-03-21 16:01:22.638746 cognee-0.1.8/cognee/infrastructure/llm/prompts/render_prompt.py
+-rw-r--r--   0        0        0       86 2024-03-21 16:01:22.639254 cognee-0.1.8/cognee/infrastructure/llm/prompts/summarize_content.txt
+-rw-r--r--   0        0        0      889 2024-03-14 09:23:35.240981 cognee-0.1.8/cognee/infrastructure/pipeline/models/Operation.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.239072 cognee-0.1.8/cognee/infrastructure/pipeline/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.241109 cognee-0.1.8/cognee/modules/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:20:06.898696 cognee-0.1.8/cognee/modules/cognify/__init__.py
+-rw-r--r--   0        0        0     1531 2024-05-26 19:03:19.290477 cognee-0.1.8/cognee/modules/cognify/config.py
+-rw-r--r--   0        0        0     3298 2024-04-23 05:20:06.898825 cognee-0.1.8/cognee/modules/cognify/dataset.py
+-rw-r--r--   0        0        0     2618 2024-05-25 06:16:34.124690 cognee-0.1.8/cognee/modules/cognify/evaluate.py
+-rw-r--r--   0        0        0        1 2024-03-14 09:23:35.241331 cognee-0.1.8/cognee/modules/cognify/graph/__init__.py
+-rw-r--r--   0        0        0     1136 2024-05-25 06:16:34.124946 cognee-0.1.8/cognee/modules/cognify/graph/add_classification_nodes.py
+-rw-r--r--   0        0        0     5209 2024-05-27 05:37:00.867184 cognee-0.1.8/cognee/modules/cognify/graph/add_cognitive_layer_graphs.py
+-rw-r--r--   0        0        0     1140 2024-05-25 06:16:34.125521 cognee-0.1.8/cognee/modules/cognify/graph/add_cognitive_layers.py
+-rw-r--r--   0        0        0     2798 2024-05-27 05:37:00.867424 cognee-0.1.8/cognee/modules/cognify/graph/add_data_chunks.py
+-rw-r--r--   0        0        0     1057 2024-05-25 06:16:34.125767 cognee-0.1.8/cognee/modules/cognify/graph/add_document_node.py
+-rw-r--r--   0        0        0     2303 2024-05-26 19:03:19.292218 cognee-0.1.8/cognee/modules/cognify/graph/add_label_nodes.py
+-rw-r--r--   0        0        0     7146 2024-05-26 19:03:19.293222 cognee-0.1.8/cognee/modules/cognify/graph/add_node_connections.py
+-rw-r--r--   0        0        0      879 2024-05-25 06:16:34.126234 cognee-0.1.8/cognee/modules/cognify/graph/add_summary_nodes.py
+-rw-r--r--   0        0        0    13112 2024-05-26 19:03:19.296197 cognee-0.1.8/cognee/modules/cognify/graph/create.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.242124 cognee-0.1.8/cognee/modules/cognify/llm/__init__.py
+-rw-r--r--   0        0        0     1364 2024-05-27 05:37:00.867528 cognee-0.1.8/cognee/modules/cognify/llm/resolve_cross_graph_references.py
+-rw-r--r--   0        0        0     7185 2024-05-25 06:16:34.128123 cognee-0.1.8/cognee/modules/cognify/test.py
+-rw-r--r--   0        0        0     2667 2024-05-25 06:16:34.128231 cognee-0.1.8/cognee/modules/cognify/train.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.239641 cognee-0.1.8/cognee/modules/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.239714 cognee-0.1.8/cognee/modules/data/extraction/__init__.py
+-rw-r--r--   0        0        0      960 2024-04-23 05:20:06.900831 cognee-0.1.8/cognee/modules/data/extraction/extract_categories.py
+-rw-r--r--   0        0        0      490 2024-04-23 05:20:06.900898 cognee-0.1.8/cognee/modules/data/extraction/extract_cognitive_layers.py
+-rw-r--r--   0        0        0      497 2024-04-23 05:20:06.900968 cognee-0.1.8/cognee/modules/data/extraction/extract_summary.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.239777 cognee-0.1.8/cognee/modules/data/extraction/knowledge_graph/__init__.py
+-rw-r--r--   0        0        0      542 2024-04-23 05:20:06.901111 cognee-0.1.8/cognee/modules/data/extraction/knowledge_graph/extract_content_graph.py
+-rw-r--r--   0        0        0     1041 2024-05-25 06:16:34.128718 cognee-0.1.8/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph.py
+-rw-r--r--   0        0        0     4715 2024-05-25 06:16:34.128835 cognee-0.1.8/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph_module.py
+-rw-r--r--   0        0        0      699 2024-05-26 19:03:19.297517 cognee-0.1.8/cognee/modules/data/get_cognitive_layers.py
+-rw-r--r--   0        0        0      520 2024-05-26 19:03:19.298211 cognee-0.1.8/cognee/modules/data/get_content_categories.py
+-rw-r--r--   0        0        0      559 2024-05-26 19:03:19.298864 cognee-0.1.8/cognee/modules/data/get_content_summary.py
+-rw-r--r--   0        0        0     1009 2024-05-26 19:03:19.300631 cognee-0.1.8/cognee/modules/data/get_layer_graphs.py
+-rw-r--r--   0        0        0       69 2024-04-23 05:20:06.901709 cognee-0.1.8/cognee/modules/discovery/__init__.py
+-rw-r--r--   0        0        0      756 2024-04-23 05:20:06.901775 cognee-0.1.8/cognee/modules/discovery/discover_directory_datasets.py
+-rw-r--r--   0        0        0       62 2024-03-29 12:59:22.987121 cognee-0.1.8/cognee/modules/ingestion/__init__.py
+-rw-r--r--   0        0        0     1853 2024-05-26 19:03:19.301006 cognee-0.1.8/cognee/modules/ingestion/add_data_to_dataset.py
+-rw-r--r--   0        0        0      549 2024-05-25 06:16:34.128937 cognee-0.1.8/cognee/modules/ingestion/classify.py
+-rw-r--r--   0        0        0      941 2024-05-25 06:16:34.129049 cognee-0.1.8/cognee/modules/ingestion/data_types/BinaryData.py
+-rw-r--r--   0        0        0      309 2024-05-26 19:03:19.301455 cognee-0.1.8/cognee/modules/ingestion/data_types/IngestionData.py
+-rw-r--r--   0        0        0      764 2024-04-23 05:20:06.902759 cognee-0.1.8/cognee/modules/ingestion/data_types/TextData.py
+-rw-r--r--   0        0        0      145 2024-03-14 09:23:35.243502 cognee-0.1.8/cognee/modules/ingestion/data_types/__init__.py
+-rw-r--r--   0        0        0      125 2024-03-14 09:23:35.243619 cognee-0.1.8/cognee/modules/ingestion/exceptions.py
+-rw-r--r--   0        0        0      275 2024-04-23 05:20:06.902967 cognee-0.1.8/cognee/modules/ingestion/identify.py
+-rw-r--r--   0        0        0      796 2024-03-29 12:59:22.988225 cognee-0.1.8/cognee/modules/ingestion/save.py
+-rw-r--r--   0        0        0     1109 2024-04-23 05:20:06.903064 cognee-0.1.8/cognee/modules/search/CogneeSearch.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.244581 cognee-0.1.8/cognee/modules/search/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.244654 cognee-0.1.8/cognee/modules/search/graph/__init__.py
+-rw-r--r--   0        0        0     2086 2024-05-26 19:03:19.301634 cognee-0.1.8/cognee/modules/search/graph/search_adjacent.py
+-rw-r--r--   0        0        0     3192 2024-05-26 19:03:19.301803 cognee-0.1.8/cognee/modules/search/graph/search_categories.py
+-rw-r--r--   0        0        0      875 2024-05-26 19:03:19.302100 cognee-0.1.8/cognee/modules/search/graph/search_cypher.py
+-rw-r--r--   0        0        0     2962 2024-05-26 19:03:19.302265 cognee-0.1.8/cognee/modules/search/graph/search_neighbour.py
+-rw-r--r--   0        0        0     2999 2024-05-26 19:03:19.302427 cognee-0.1.8/cognee/modules/search/graph/search_summary.py
+-rw-r--r--   0        0        0        0 2024-05-26 19:03:19.302457 cognee-0.1.8/cognee/modules/search/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-26 19:03:19.302527 cognee-0.1.8/cognee/modules/search/llm/extraction/__init__.py
+-rw-r--r--   0        0        0      667 2024-05-25 06:16:34.130219 cognee-0.1.8/cognee/modules/search/llm/extraction/categorize_relevant_category.py
+-rw-r--r--   0        0        0      703 2024-05-25 06:16:34.130413 cognee-0.1.8/cognee/modules/search/llm/extraction/categorize_relevant_summary.py
+-rw-r--r--   0        0        0      650 2024-05-25 06:16:34.130695 cognee-0.1.8/cognee/modules/search/llm/get_relevant_summary.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.244937 cognee-0.1.8/cognee/modules/search/vector/__init__.py
+-rw-r--r--   0        0        0       42 2024-05-25 06:16:34.130807 cognee-0.1.8/cognee/modules/search/vector/bm25.py
+-rw-r--r--   0        0        0       51 2024-05-25 06:16:34.130913 cognee-0.1.8/cognee/modules/search/vector/fusion.py
+-rw-r--r--   0        0        0     2047 2024-05-27 05:37:00.867637 cognee-0.1.8/cognee/modules/search/vector/search_similarity.py
+-rw-r--r--   0        0        0      141 2024-05-25 06:16:34.131198 cognee-0.1.8/cognee/modules/settings/__init__.py
+-rw-r--r--   0        0        0     2643 2024-05-27 05:37:00.867737 cognee-0.1.8/cognee/modules/settings/get_settings.py
+-rw-r--r--   0        0        0      678 2024-05-27 05:37:00.868700 cognee-0.1.8/cognee/modules/settings/save_llm_config.py
+-rw-r--r--   0        0        0      606 2024-05-27 05:37:00.868820 cognee-0.1.8/cognee/modules/settings/save_vector_db_config.py
+-rw-r--r--   0        0        0      159 2024-05-27 05:37:00.868950 cognee-0.1.8/cognee/modules/tasks/__init__.py
+-rw-r--r--   0        0        0      502 2024-05-26 19:03:19.303139 cognee-0.1.8/cognee/modules/tasks/create_task_status_table.py
+-rw-r--r--   0        0        0      632 2024-05-27 05:37:00.869016 cognee-0.1.8/cognee/modules/tasks/get_task_status.py
+-rw-r--r--   0        0        0      376 2024-05-26 19:03:19.303304 cognee-0.1.8/cognee/modules/tasks/update_task_status.py
+-rw-r--r--   0        0        0        0 2024-05-25 06:16:34.131739 cognee-0.1.8/cognee/modules/topology/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-26 19:03:19.303341 cognee-0.1.8/cognee/modules/topology/extraction/__init__.py
+-rw-r--r--   0        0        0      505 2024-05-25 06:16:34.132108 cognee-0.1.8/cognee/modules/topology/extraction/extract_topology.py
+-rw-r--r--   0        0        0      735 2024-05-26 19:03:19.303516 cognee-0.1.8/cognee/modules/topology/infer_data_topology.py
+-rw-r--r--   0        0        0     5986 2024-05-26 19:03:19.303736 cognee-0.1.8/cognee/modules/topology/topology.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.245146 cognee-0.1.8/cognee/modules/users/__init__.py
+-rw-r--r--   0        0        0      179 2024-04-28 19:24:05.619936 cognee-0.1.8/cognee/modules/users/memory/__init__.py
+-rw-r--r--   0        0        0      802 2024-03-14 09:23:35.245545 cognee-0.1.8/cognee/modules/users/memory/create_information_points.py
+-rw-r--r--   0        0        0      229 2024-04-28 19:24:05.620017 cognee-0.1.8/cognee/modules/users/memory/is_existing_memory.py
+-rw-r--r--   0        0        0      203 2024-04-28 19:24:05.620093 cognee-0.1.8/cognee/modules/users/memory/register_memory_for_user.py
+-rw-r--r--   0        0        0   124245 2024-04-23 05:20:06.904069 cognee-0.1.8/cognee/programs/extract_knowledge_graph/extract_knowledge_graph.json
+-rw-r--r--   0        0        0      719 2024-05-26 19:03:19.304532 cognee-0.1.8/cognee/root_dir.py
+-rw-r--r--   0        0        0      803 2024-05-25 06:16:34.132721 cognee-0.1.8/cognee/shared/GithubClassification.py
+-rw-r--r--   0        0        0      984 2024-05-25 06:16:34.132929 cognee-0.1.8/cognee/shared/GithubTopology.py
+-rw-r--r--   0        0        0     2009 2024-05-25 06:16:34.133146 cognee-0.1.8/cognee/shared/SourceCodeGraph.py
+-rw-r--r--   0        0        0        0 2024-03-14 09:23:35.246078 cognee-0.1.8/cognee/shared/__init__.py
+-rw-r--r--   0        0        0     8940 2024-05-26 19:03:19.304823 cognee-0.1.8/cognee/shared/data_models.py
+-rw-r--r--   0        0        0      365 2024-03-21 16:01:22.651774 cognee-0.1.8/cognee/shared/encode_uuid.py
+-rw-r--r--   0        0        0       72 2024-04-29 19:00:12.026208 cognee-0.1.8/cognee/tests/Untitled.ipynb
+-rw-r--r--   0        0        0        0 2024-04-26 13:52:41.240049 cognee-0.1.8/cognee/tests/__init__.py
+-rw-r--r--   0        0        0      985 2024-04-26 13:52:41.240261 cognee-0.1.8/cognee/tests/test_data/Natural_language_processing.txt
+-rwxr-xr-x   0        0        0     6242 2024-05-26 19:03:19.305141 cognee-0.1.8/cognee/tests/test_library.py
+-rw-r--r--   0        0        0     9603 2024-05-25 06:16:34.133633 cognee-0.1.8/cognee/utils.py
+-rw-r--r--   0        0        0     3028 2024-05-27 05:37:19.734614 cognee-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     7464 1970-01-01 00:00:00.000000 cognee-0.1.8/PKG-INFO
```

### Comparing `cognee-0.1.7/LICENSE` & `cognee-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/README.md` & `cognee-0.1.8/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -27,59 +27,55 @@
   <a href="https://github.com/topoteretes/cognee/releases">
     <img src="https://img.shields.io/github/release/topoteretes/cognee?&label=Latest&style=for-the-badge" alt="cognee releases" />
   </a>
 </p>
 
 ![Cognee Demo](assets/cognee_demo.gif)
 
-Try it in a Google collab  <a href="https://colab.research.google.com/drive/11k0GtbrKRVGTxhcgad4Wl8YvCnWJVWPl?usp=sharing">notebook</a>  or have a look at our <a href="https://topoteretes.github.io/cognee">documentation</a>
 
-Join our  <a href="https://discord.gg/NQPKmU5CCg">Discord</a> community
+Try it in a Google collab  <a href="https://colab.research.google.com/drive/184Kpe9XGjrt8nVss0WDiPsPRrPk5lZ6o?usp=sharing">notebook</a>  or have a look at our <a href="https://topoteretes.github.io/cognee">documentation</a>
+
+If you have questions, join our  <a href="https://discord.gg/NQPKmU5CCg">Discord</a> community
 
 
 
 
 
 ## 📦 Installation
 
 ### With pip
 
 ```bash
 pip install cognee
 ```
 
-Use Weaviate vector storage:
-```bash
-pip install "cognee[weaviate]"
-```
 
 ### With poetry
 
 ```bash
 poetry add cognee
 ```
 
-Use Weaviate vector storage:
-```bash
-poetry add "cognee[weaviate]"
-```
 
 ## 💻 Usage
 
 ### Setup
 
 ```
 import os
 
-os.environ["WEAVIATE_URL"] = "YOUR_WEAVIATE_URL"
-os.environ["WEAVIATE_API_KEY"] = "YOUR_WEAVIATE_API_KEY"
-
-os.environ["OPENAI_API_KEY"] = "YOUR_OPENAI_API_KEY"
+os.environ["LLM_API_KEY"] = "YOUR OPENAI_API_KEY"
 
 ```
+or 
+```
+import cognee
+cognee.config.llm_api_key = "YOUR_OPENAI_API_KEY"
+```
+
 You can also use Ollama or Anyscale as your LLM provider. For more info on local models check our [docs](https://topoteretes.github.io/cognee)
 
 ### Run
 
 ```
 import cognee
 
@@ -115,14 +111,26 @@
 #
 # cognee.add("data://{absolute_path_to_root}", "reports.2024")
 # This will add just directory 2024 under reports.
 ```
 
 Read more [here](docs/index.md#run).
 
+## Vector retrieval, Graphs and LLMs
+
+Cognee supports a variety of tools and services for different operations:
+
+- **Local Setup**: By default, LanceDB runs locally with NetworkX and OpenAI.
+
+- **Vector Stores**: Cognee supports Qdrant and Weaviate for vector storage.
+
+- **Language Models (LLMs)**: You can use either Anyscale or Ollama as your LLM provider.
+
+- **Graph Stores**: In addition to LanceDB, Neo4j is also supported for graph storage.
+
 ## Demo
 
 Check out our demo notebook [here](https://github.com/topoteretes/cognee/blob/main/notebooks/cognee%20-%20Get%20Started.ipynb)
 
 
 
 [<img src="https://i3.ytimg.com/vi/-ARUfIzhzC4/maxresdefault.jpg" width="100%">](https://www.youtube.com/watch?v=BDFt4xVPmro "Learn about cognee: 55")
@@ -136,13 +144,11 @@
 
 
 
 
 ![Image](assets/architecture.png)
 
 
-## 🚀 It's alive
+## Star History
 
-<p>
-Try it yourself on Whatsapp with one of our <a href="https://keepi.ai" target="_blank">partners</a> by typing `/save {content you want to save}` followed by `/query {knowledge you saved previously}`
-For more info here are the <a href="https://topoteretes.github.io/cognee">docs</a>
-</p>
+
+[![Star History Chart](https://api.star-history.com/svg?repos=topoteretes/cognee&type=Date)](https://star-history.com/#topoteretes/cognee&Date)
```

#### html2text {}

```diff
@@ -1,37 +1,39 @@
 # cognee Deterministic LLMs Outputs for AI Engineers using graphs, LLMs and
 vector retrieval
 _[_C_o_g_n_e_e_ _l_o_g_o_]
 Open-source framework for creating self-improving deterministic outputs for
 LLMs.
 _[_c_o_g_n_e_e_ _f_o_r_k_s_]_[_c_o_g_n_e_e_ _s_t_a_r_s_]_[_c_o_g_n_e_e_ _p_u_l_l_-_r_e_q_u_e_s_t_s_]_[_c_o_g_n_e_e_ _r_e_l_e_a_s_e_s_]
 ![Cognee Demo](assets/cognee_demo.gif) Try it in a Google collab _n_o_t_e_b_o_o_k or
-have a look at our _d_o_c_u_m_e_n_t_a_t_i_o_n Join our _D_i_s_c_o_r_d community ## ð¦
-Installation ### With pip ```bash pip install cognee ``` Use Weaviate vector
-storage: ```bash pip install "cognee[weaviate]" ``` ### With poetry ```bash
-poetry add cognee ``` Use Weaviate vector storage: ```bash poetry add "cognee
-[weaviate]" ``` ## ð» Usage ### Setup ``` import os os.environ
-["WEAVIATE_URL"] = "YOUR_WEAVIATE_URL" os.environ["WEAVIATE_API_KEY"] =
-"YOUR_WEAVIATE_API_KEY" os.environ["OPENAI_API_KEY"] = "YOUR_OPENAI_API_KEY"
-``` You can also use Ollama or Anyscale as your LLM provider. For more info on
-local models check our [docs](https://topoteretes.github.io/cognee) ### Run ```
-import cognee text = """Natural language processing (NLP) is an
-interdisciplinary subfield of computer science and information retrieval"""
-cognee.add([text], "example_dataset") # Add a new piece of information
-cognee.cognify() # Use LLMs and cognee to create knowledge search_results =
-cognee.search("SIMILARITY", "computer science") # Query cognee for the
-knowledge for result_text in search_results[0]: print(result_text) ``` Add
-alternative data types: ``` cognee.add("file://{absolute_path_to_file}",
-dataset_name) ``` Or ``` cognee.add("data://{absolute_path_to_directory}",
-dataset_name) # This is useful if you have a directory with files organized in
-subdirectories. # You can target which directory to add by providing
-dataset_name. # Example: # root # / \ # reports bills # / \ # 2024 2023 # #
-cognee.add("data://{absolute_path_to_root}", "reports.2024") # This will add
-just directory 2024 under reports. ``` Read more [here](docs/index.md#run). ##
-Demo Check out our demo notebook [here](https://github.com/topoteretes/cognee/
-blob/main/notebooks/cognee%20-%20Get%20Started.ipynb) [[https://i3.ytimg.com/
-vi/-ARUfIzhzC4/maxresdefault.jpg]](https://www.youtube.com/watch?v=BDFt4xVPmro
-"Learn about cognee: 55") ## How it works ![Image](assets/architecture.png) ##
-ð It's alive
-Try it yourself on Whatsapp with one of our _p_a_r_t_n_e_r_s by typing `/save {content
-you want to save}` followed by `/query {knowledge you saved previously}` For
-more info here are the _d_o_c_s
+have a look at our _d_o_c_u_m_e_n_t_a_t_i_o_n If you have questions, join our _D_i_s_c_o_r_d
+community ## ð¦ Installation ### With pip ```bash pip install cognee ``` ###
+With poetry ```bash poetry add cognee ``` ## ð» Usage ### Setup ``` import os
+os.environ["LLM_API_KEY"] = "YOUR OPENAI_API_KEY" ``` or ``` import cognee
+cognee.config.llm_api_key = "YOUR_OPENAI_API_KEY" ``` You can also use Ollama
+or Anyscale as your LLM provider. For more info on local models check our
+[docs](https://topoteretes.github.io/cognee) ### Run ``` import cognee text =
+"""Natural language processing (NLP) is an interdisciplinary subfield of
+computer science and information retrieval""" cognee.add([text],
+"example_dataset") # Add a new piece of information cognee.cognify() # Use LLMs
+and cognee to create knowledge search_results = cognee.search("SIMILARITY",
+"computer science") # Query cognee for the knowledge for result_text in
+search_results[0]: print(result_text) ``` Add alternative data types: ```
+cognee.add("file://{absolute_path_to_file}", dataset_name) ``` Or ```
+cognee.add("data://{absolute_path_to_directory}", dataset_name) # This is
+useful if you have a directory with files organized in subdirectories. # You
+can target which directory to add by providing dataset_name. # Example: # root
+# / \ # reports bills # / \ # 2024 2023 # # cognee.add("data://
+{absolute_path_to_root}", "reports.2024") # This will add just directory 2024
+under reports. ``` Read more [here](docs/index.md#run). ## Vector retrieval,
+Graphs and LLMs Cognee supports a variety of tools and services for different
+operations: - **Local Setup**: By default, LanceDB runs locally with NetworkX
+and OpenAI. - **Vector Stores**: Cognee supports Qdrant and Weaviate for vector
+storage. - **Language Models (LLMs)**: You can use either Anyscale or Ollama as
+your LLM provider. - **Graph Stores**: In addition to LanceDB, Neo4j is also
+supported for graph storage. ## Demo Check out our demo notebook [here](https:/
+/github.com/topoteretes/cognee/blob/main/notebooks/cognee%20-
+%20Get%20Started.ipynb) [[https://i3.ytimg.com/vi/-ARUfIzhzC4/
+maxresdefault.jpg]](https://www.youtube.com/watch?v=BDFt4xVPmro "Learn about
+cognee: 55") ## How it works ![Image](assets/architecture.png) ## Star History
+[![Star History Chart](https://api.star-history.com/svg?repos=topoteretes/
+cognee&type=Date)](https://star-history.com/#topoteretes/cognee&Date)
```

### Comparing `cognee-0.1.7/cognee/api/v1/add/add.py` & `cognee-0.1.8/cognee/api/v1/add/add.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,64 @@
-from typing import List, Union
+from typing import List, Union, BinaryIO
 from os import path
 import asyncio
 import dlt
 import duckdb
 import cognee.modules.ingestion as ingestion
 from cognee.infrastructure import infrastructure_config
 from cognee.infrastructure.files.storage import LocalStorage
 from cognee.modules.discovery import discover_directory_datasets
 from cognee.utils import send_telemetry
-
-
-async def add(data_path: Union[str, List[str]], dataset_name: str = None):
-    if isinstance(data_path, str):
-        # data_path is a data directory path
-        if "data://" in data_path:
-            return await add_data_directory(data_path.replace("data://", ""), dataset_name)
-        # data_path is a file path
-        if "file://" in data_path:
-            return await add([data_path], dataset_name)
-        # data_path is a text
+from cognee.base_config import get_base_config
+base_config = get_base_config()
+from cognee.infrastructure.databases.relational.config import get_relationaldb_config
+
+relational_config = get_relationaldb_config()
+
+
+async def add(data: Union[BinaryIO, List[BinaryIO], str, List[str]], dataset_name: str = None):
+    if isinstance(data, str):
+        # data is a data directory path
+        if "data://" in data:
+            return await add_data_directory(data.replace("data://", ""), dataset_name)
+        # data is a file path
+        if "file://" in data:
+            return await add([data], dataset_name)
+        # data is a text
         else:
-            file_path = save_text_to_file(data_path, dataset_name)
+            file_path = save_data_to_file(data, dataset_name)
             return await add([file_path], dataset_name)
 
-    # data_path is a list of file paths or texts
-    file_paths = []
-    texts = []
-
-    for file_path in data_path:
-        if file_path.startswith("/") or file_path.startswith("file://"):
-            file_paths.append(file_path)
-        else:
-            texts.append(file_path)
+    if hasattr(data, "file"):
+        file_path = save_data_to_file(data.file, dataset_name, filename = data.filename)
+        return await add([file_path], dataset_name)
 
-    awaitables = []
+    # data is a list of file paths or texts
+    file_paths = []
 
-    if len(texts) > 0:
-        for text in texts:
-            file_paths.append(save_text_to_file(text, dataset_name))
+    for data_item in data:
+        if hasattr(data_item, "file"):
+            file_paths.append(save_data_to_file(data_item, dataset_name, filename = data_item.filename))
+        elif isinstance(data_item, str) and (
+            data_item.startswith("/") or data_item.startswith("file://")
+        ):
+            file_paths.append(data_item)
+        elif isinstance(data_item, str):
+            file_paths.append(save_data_to_file(data_item, dataset_name))
 
     if len(file_paths) > 0:
-        awaitables.append(add_files(file_paths, dataset_name))
+        return await add_files(file_paths, dataset_name)
 
-    return await asyncio.gather(*awaitables)
+    return []
 
 async def add_files(file_paths: List[str], dataset_name: str):
-    infra_config = infrastructure_config.get_config()
-    data_directory_path = infra_config["data_root_directory"]
+    # infra_config = infrastructure_config.get_config()
+    data_directory_path = base_config.data_root_directory
 
-    LocalStorage.ensure_directory_exists(infra_config["database_directory_path"])
+    LocalStorage.ensure_directory_exists(relational_config.database_directory_path)
 
     processed_file_paths = []
 
     for file_path in file_paths:
         file_path = file_path.replace("file://", "")
 
         if data_directory_path not in file_path:
@@ -63,15 +69,15 @@
             LocalStorage.ensure_directory_exists(file_directory_path)
 
             LocalStorage.copy_file(file_path, dataset_file_path)
             processed_file_paths.append(dataset_file_path)
         else:
             processed_file_paths.append(file_path)
 
-    db = duckdb.connect(infra_config["database_path"])
+    db = duckdb.connect(relational_config.db_file_path)
 
     destination = dlt.destinations.duckdb(
         credentials = db,
     )
 
     pipeline = dlt.pipeline(
         pipeline_name = "file_load_from_filesystem",
@@ -114,20 +120,21 @@
 
     for key in datasets.keys():
         if dataset_name is None or key.startswith(dataset_name):
             results.append(add(datasets[key], dataset_name = key))
 
     return await asyncio.gather(*results)
 
-def save_text_to_file(text: str, dataset_name: str):
-    data_directory_path = infrastructure_config.get_config()["data_root_directory"]
+def save_data_to_file(data: Union[str, BinaryIO], dataset_name: str, filename: str = None):
+    data_directory_path = base_config.data_root_directory
 
-    classified_data = ingestion.classify(text)
-    data_id = ingestion.identify(classified_data)
+    classified_data = ingestion.classify(data, filename)
+    # data_id = ingestion.identify(classified_data)
 
     storage_path = data_directory_path + "/" + dataset_name.replace(".", "/")
     LocalStorage.ensure_directory_exists(storage_path)
 
-    text_file_name = data_id + ".txt"
-    LocalStorage(storage_path).store(text_file_name, classified_data.get_data())
+    file_metadata = classified_data.get_metadata()
+    file_name = file_metadata["name"]
+    LocalStorage(storage_path).store(file_name, classified_data.get_data())
 
-    return "file://" + storage_path + "/" + text_file_name
+    return "file://" + storage_path + "/" + file_name
```

### Comparing `cognee-0.1.7/cognee/api/v1/add/add_standalone.py` & `cognee-0.1.8/cognee/api/v1/add/add_standalone.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import asyncio
 from uuid import UUID, uuid4
 from typing import Union, BinaryIO, List
 import cognee.modules.ingestion as ingestion
 from cognee.infrastructure import infrastructure_config
+from cognee.infrastructure.databases.relational.config import get_relationaldb_config
 
+relational_config = get_relationaldb_config()
 class DatasetException(Exception):
     message: str
 
     def __init__(self, message: str):
         self.message = message
 
 
 async def add_standalone(
     data: Union[str, BinaryIO, List[Union[str, BinaryIO]]],
     dataset_id: UUID = uuid4(),
     dataset_name: str = None
 ):
-    db_engine = infrastructure_config.get_config()["database_engine"]
+    db_engine = relational_config.database_engine
     if db_engine.is_db_done is not True:
         await db_engine.ensure_tables()
 
     if not data:
         raise DatasetException("Data must be provided to cognee.add(data: str)")
 
     if isinstance(data, list):
```

### Comparing `cognee-0.1.7/cognee/api/v1/add/remember.py` & `cognee-0.1.8/cognee/api/v1/add/remember.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/api/v1/cognify/cognify.py` & `cognee-0.1.8/cognee/api/v1/cognify/cognify.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,148 +1,237 @@
 import asyncio
 from uuid import uuid4
 from typing import List, Union
 import logging
-import instructor
 import nltk
-from openai import OpenAI
 from nltk.corpus import stopwords
 from cognee.config import Config
-from cognee.modules.cognify.graph.add_data_chunks import add_data_chunks
+from cognee.infrastructure.data.chunking.LangchainChunkingEngine import LangchainChunkEngine
+from cognee.infrastructure.databases.graph.config import get_graph_config
+from cognee.infrastructure.databases.vector.embeddings.DefaultEmbeddingEngine import LiteLLMEmbeddingEngine
+from cognee.modules.cognify.graph.add_node_connections import group_nodes_by_layer, \
+    graph_ready_output, connect_nodes_in_graph
+from cognee.modules.cognify.graph.add_data_chunks import add_data_chunks, add_data_chunks_basic_rag
 from cognee.modules.cognify.graph.add_document_node import add_document_node
 from cognee.modules.cognify.graph.add_classification_nodes import add_classification_nodes
 from cognee.modules.cognify.graph.add_cognitive_layer_graphs import add_cognitive_layer_graphs
 from cognee.modules.cognify.graph.add_summary_nodes import add_summary_nodes
-from cognee.modules.cognify.graph.add_node_connections import group_nodes_by_layer, \
-    graph_ready_output, connect_nodes_in_graph
 from cognee.modules.cognify.llm.resolve_cross_graph_references import resolve_cross_graph_references
 from cognee.infrastructure.databases.graph.get_graph_client import get_graph_client
 from cognee.modules.cognify.graph.add_cognitive_layers import add_cognitive_layers
 # from cognee.modules.cognify.graph.initialize_graph import initialize_graph
 from cognee.infrastructure.files.utils.guess_file_type import guess_file_type, FileTypeException
 from cognee.infrastructure.files.utils.extract_text_from_file import extract_text_from_file
 from cognee.infrastructure import infrastructure_config
 from cognee.modules.data.get_content_categories import get_content_categories
 from cognee.modules.data.get_content_summary import get_content_summary
 from cognee.modules.data.get_cognitive_layers import get_cognitive_layers
 from cognee.modules.data.get_layer_graphs import get_layer_graphs
+from cognee.shared.data_models import ChunkStrategy, KnowledgeGraph
 from cognee.utils import send_telemetry
+from cognee.modules.tasks import create_task_status_table, update_task_status
+from cognee.shared.SourceCodeGraph import SourceCodeGraph
+from asyncio import Lock
+from cognee.modules.tasks import get_task_status
+from cognee.base_config import get_base_config
+from cognee.infrastructure.data.chunking.config import get_chunk_config
+from cognee.modules.cognify.config import get_cognify_config
+from cognee.infrastructure.databases.vector.embeddings.config import get_embedding_config
+from cognee.infrastructure.databases.relational.config import get_relationaldb_config
 
-
+graph_config = get_graph_config()
 config = Config()
 config.load()
 
-aclient = instructor.patch(OpenAI())
+
+relational_config = get_relationaldb_config()
+
+
+cognify_config = get_cognify_config()
+chunk_config = get_chunk_config()
+base_config = get_base_config()
+embedding_config = get_embedding_config()
+
+# aclient = instructor.patch(OpenAI())
 
 USER_ID = "default_user"
 
 logger = logging.getLogger("cognify")
 
+update_status_lock = Lock()
+
 async def cognify(datasets: Union[str, List[str]] = None):
     """This function is responsible for the cognitive processing of the content."""
     # Has to be loaded in advance, multithreading doesn't work without it.
     nltk.download("stopwords", quiet=True)
     stopwords.ensure_loaded()
+    create_task_status_table()
 
-    graph_db_type = infrastructure_config.get_config()["graph_engine"]
+    graph_db_type = graph_config.graph_engine
 
     graph_client = await get_graph_client(graph_db_type)
 
-    db_engine = infrastructure_config.get_config()["database_engine"]
+    db_engine = relational_config.database_engine
 
     if datasets is None or len(datasets) == 0:
         datasets = db_engine.get_datasets()
 
     awaitables = []
 
+    async def handle_cognify_task(dataset_name: str):
+        async with update_status_lock:
+            task_status = get_task_status([dataset_name])
+
+            if task_status == "DATASET_PROCESSING_STARTED":
+                logger.error(f"Dataset {dataset_name} is already being processed.")
+                return
+
+        update_task_status(dataset_name, "DATASET_PROCESSING_STARTED")
+        await cognify(dataset_name)
+        update_task_status(dataset_name, "DATASET_PROCESSING_FINISHED")
+
     # datasets is a list of dataset names
     if isinstance(datasets, list):
-        for dataset in datasets:
-            awaitables.append(cognify(dataset))
+        for dataset_name in datasets:
+            awaitables.append(handle_cognify_task(dataset_name))
 
         graphs = await asyncio.gather(*awaitables)
         return graphs[0]
 
     added_datasets = db_engine.get_datasets()
 
     dataset_files = []
     # datasets is a dataset name string
     dataset_name = datasets.replace(".", "_").replace(" ", "_")
 
     for added_dataset in added_datasets:
         if dataset_name in added_dataset:
             dataset_files.append((added_dataset, db_engine.get_files_metadata(added_dataset)))
 
-    # await initialize_graph(USER_ID, graph_data_model, graph_client)
 
-    data_chunks = {}
+    chunk_engine = chunk_config.chunk_engine
+    chunk_strategy = chunk_config.chunk_strategy
 
-    chunk_engine = infrastructure_config.get_config()["chunk_engine"]
-    chunk_strategy = infrastructure_config.get_config()["chunk_strategy"]
+    async def process_batch(files_batch):
+        data_chunks = {}
 
-    for (dataset_name, files) in dataset_files:
-        for file_metadata in files:
+        for dataset_name, file_metadata, document_id in files_batch:
             with open(file_metadata["file_path"], "rb") as file:
                 try:
-                    document_id = await add_document_node(
-                        graph_client,
-                        parent_node_id = f"DefaultGraphModel__{USER_ID}",
-                        document_metadata = file_metadata,
-                    )
-
                     file_type = guess_file_type(file)
                     text = extract_text_from_file(file, file_type)
-                    subchunks = chunk_engine.chunk_data(chunk_strategy, text, config.chunk_size, config.chunk_overlap)
+                    if text is None:
+                        text = "empty file"
+                    if text == "":
+                        text = "empty file"
+                    subchunks = chunk_engine.chunk_data(chunk_strategy, text, chunk_config.chunk_size, chunk_config.chunk_overlap)
 
                     if dataset_name not in data_chunks:
                         data_chunks[dataset_name] = []
 
                     for subchunk in subchunks:
-                        data_chunks[dataset_name].append(dict(document_id = document_id, chunk_id = str(uuid4()), text = subchunk))
+                        data_chunks[dataset_name].append(dict(
+                            document_id = document_id,
+                            chunk_id = str(uuid4()),
+                            text = subchunk,
+                            file_metadata = file_metadata,
+                        ))
+
                 except FileTypeException:
                     logger.warning("File (%s) has an unknown file type. We are skipping it.", file_metadata["id"])
 
-    added_chunks: list[tuple[str, str, dict]] = await add_data_chunks(data_chunks)
+        added_chunks = await add_data_chunks(data_chunks)
+        await add_data_chunks_basic_rag(data_chunks)
 
-    await asyncio.gather(
-        *[process_text(chunk["document_id"], chunk["chunk_id"], chunk["collection"], chunk["text"]) for chunk in added_chunks]
-    )
+        await asyncio.gather(
+            *[process_text(
+              chunk["collection"],
+              chunk["chunk_id"],
+              chunk["text"],
+              chunk["file_metadata"],
+              chunk["document_id"]
+            ) for chunk in added_chunks]
+        )
+
+    batch_size = 20
+    file_count = 0
+    files_batch = []
+
+    for (dataset_name, files) in dataset_files:
+        for file_metadata in files:
+            graph_topology = graph_config.graph_model
+
+            if graph_topology == SourceCodeGraph:
+                parent_node_id = f"{file_metadata['name']}.{file_metadata['extension']}"
+            else:
+                parent_node_id = f"DefaultGraphModel__{USER_ID}"
+
+            document_id = await add_document_node(
+                graph_client,
+                parent_node_id=parent_node_id,
+                document_metadata=file_metadata,
+            )
+
+            files_batch.append((dataset_name, file_metadata, document_id))
+            file_count += 1
+
+            if file_count >= batch_size:
+                await process_batch(files_batch)
+                files_batch = []
+                file_count = 0
+
+    # Process any remaining files in the last batch
+    if len(files_batch) > 0:
+        await process_batch(files_batch)
 
     return graph_client.graph
 
-async def process_text(document_id: str, chunk_id: str, chunk_collection: str, input_text: str):
-    raw_document_id = document_id.split("__")[-1]
 
-    print(f"Processing chunk ({chunk_id}) from document ({raw_document_id}).")
+async def process_text(chunk_collection: str, chunk_id: str, input_text: str, file_metadata: dict, document_id: str):
+    print(f"Processing chunk ({chunk_id}) from document ({file_metadata['id']}).")
+
+    graph_client = await get_graph_client(graph_config.graph_engine)
+    print("graph_client", graph_client)
 
-    graph_client = await get_graph_client(infrastructure_config.get_config()["graph_engine"])
+    graph_topology = cognify_config.graph_model
+    if graph_topology == SourceCodeGraph:
+        classified_categories = [{"data_type": "text", "category_name": "Code and functions"}]
+    elif graph_topology == KnowledgeGraph:
+        classified_categories = await get_content_categories(input_text)
+    else:
+        classified_categories = [{"data_type": "text", "category_name": "Unclassified text"}]
+
+    # await add_label_nodes(graph_client, document_id, chunk_id, file_metadata["keywords"].split("|"))
 
-    classified_categories = await get_content_categories(input_text)
     await add_classification_nodes(
         graph_client,
         parent_node_id = document_id,
         categories = classified_categories,
     )
-
     print(f"Chunk ({chunk_id}) classified.")
 
     content_summary = await get_content_summary(input_text)
     await add_summary_nodes(graph_client, document_id, content_summary)
-
     print(f"Chunk ({chunk_id}) summarized.")
 
     cognitive_layers = await get_cognitive_layers(input_text, classified_categories)
-    cognitive_layers = (await add_cognitive_layers(graph_client, document_id, cognitive_layers))[:2]
+    cognitive_layers = cognitive_layers[:cognify_config.cognitive_layers_limit]
+
+    try:
+        cognitive_layers = (await add_cognitive_layers(graph_client, document_id, cognitive_layers))[:2]
+        print("cognitive_layers", cognitive_layers)
+        layer_graphs = await get_layer_graphs(input_text, cognitive_layers)
+        await add_cognitive_layer_graphs(graph_client, chunk_collection, chunk_id, layer_graphs)
+    except:
+        pass
 
-    layer_graphs = await get_layer_graphs(input_text, cognitive_layers)
-    await add_cognitive_layer_graphs(graph_client, chunk_collection, chunk_id, layer_graphs)
 
-    if infrastructure_config.get_config()["connect_documents"] is True:
-        db_engine = infrastructure_config.get_config()["database_engine"]
-        relevant_documents_to_connect = db_engine.fetch_cognify_data(excluded_document_id = raw_document_id)
+    if cognify_config.connect_documents is True:
+        db_engine = relational_config.database_engine
+        relevant_documents_to_connect = db_engine.fetch_cognify_data(excluded_document_id = document_id)
 
         list_of_nodes = []
 
         relevant_documents_to_connect.append({
             "layer_id": document_id,
         })
 
@@ -155,31 +244,65 @@
         results = await resolve_cross_graph_references(nodes_by_layer)
 
         relationships = graph_ready_output(results)
 
         await connect_nodes_in_graph(
             graph_client,
             relationships,
-            score_threshold = infrastructure_config.get_config()["intra_layer_score_treshold"]
+            score_threshold = cognify_config.intra_layer_score_treshold
         )
 
     send_telemetry("cognee.cognify")
 
     print(f"Chunk ({chunk_id}) cognified.")
 
 
+
 if __name__ == "__main__":
 
     async def test():
+        # await prune.prune_system()
+        # #
+        # from cognee.api.v1.add import add
+        # data_directory_path = os.path.abspath("../../../.data")
+        # # print(data_directory_path)
+        # # config.data_root_directory(data_directory_path)
+        # # cognee_directory_path = os.path.abspath("../.cognee_system")
+        # # config.system_root_directory(cognee_directory_path)
+        #
+        # await add("data://" +data_directory_path, "example")
+
+        text = """import subprocess
+                def show_all_processes():
+                    process = subprocess.Popen(['ps', 'aux'], stdout=subprocess.PIPE)
+                    output, error = process.communicate()
+                
+                    if error:
+                        print(f"Error: {error}")
+                    else:
+                        print(output.decode())
+                
+                show_all_processes()"""
 
         from cognee.api.v1.add import add
 
-        await add(["A large language model (LLM) is a language model notable for its ability to achieve general-purpose language generation and other natural language processing tasks such as classification"], "test")
-
-        graph = await cognify()
-
-        from cognee.utils import render_graph
+        await add([text], "example_dataset")
 
-        await render_graph(graph, include_color=True, include_nodes=True, include_size=True)
+        infrastructure_config.set_config( {"chunk_engine": LangchainChunkEngine() , "chunk_strategy": ChunkStrategy.CODE,'embedding_engine': LiteLLMEmbeddingEngine() })
+        from cognee.shared.SourceCodeGraph import SourceCodeGraph
+        from cognee.api.v1.config import config
+
+        # config.set_graph_model(SourceCodeGraph)
+        # config.set_classification_model(CodeContentPrediction)
+        # graph = await cognify()
+        vector_client = infrastructure_config.get_config("vector_engine")
+
+        out = await vector_client.search(collection_name ="basic_rag", query_text="show_all_processes", limit=10)
+
+        print("results", out)
+        #
+        # from cognee.utils import render_graph
+        #
+        # await render_graph(graph, include_color=True, include_nodes=False, include_size=False)
 
     import asyncio
     asyncio.run(test())
```

### Comparing `cognee-0.1.7/cognee/api/v1/config/config.py` & `cognee-0.1.8/cognee/api/v1/config/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,83 @@
 """ This module is used to set the configuration of the system."""
-from cognee.infrastructure import infrastructure_config
+from cognee.base_config import get_base_config
+from cognee.infrastructure.databases.graph.config import get_graph_config
+from cognee.infrastructure.data.chunking.config import get_chunk_config
+from cognee.modules.cognify.config import get_cognify_config
+
+
+cognify_config = get_cognify_config()
+chunk_config = get_chunk_config()
+graph_config = get_graph_config()
+base_config = get_base_config()
 
 class config():
     @staticmethod
     def system_root_directory(system_root_directory: str):
-        infrastructure_config.set_config({
-            "system_root_directory": system_root_directory
-        })
+        base_config.system_root_directory = system_root_directory
 
     @staticmethod
     def data_root_directory(data_root_directory: str):
-        infrastructure_config.set_config({
-            "data_root_directory": data_root_directory
-        })
+        base_config.data_root_directory = data_root_directory
+
+    @staticmethod
+    def monitoring_tool(monitoring_tool: object):
+        base_config.monitoring_tool = monitoring_tool
 
     @staticmethod
     def set_classification_model(classification_model: object):
-        infrastructure_config.set_config({
-            "classification_model": classification_model
-        })
+        cognify_config.classification_model =  classification_model
 
     @staticmethod
     def set_summarization_model(summarization_model: object):
-        infrastructure_config.set_config({
-            "summarization_model": summarization_model
-        })
+        cognify_config.summarization_model=summarization_model
+
 
     @staticmethod
     def set_labeling_model(labeling_model: object):
-        infrastructure_config.set_config({
-            "labeling_model": labeling_model
-        })
+        cognify_config.labeling_model =labeling_model
+
 
     @staticmethod
     def set_graph_model(graph_model: object):
-        infrastructure_config.set_config({
-            "graph_model": graph_model
-        })
+        graph_config.graph_model =graph_model
+
 
     @staticmethod
     def set_cognitive_layer_model(cognitive_layer_model: object):
-        infrastructure_config.set_config({
-            "cognitive_layer_model": cognitive_layer_model
-        })
+        cognify_config.cognitive_layer_model =cognitive_layer_model
+
 
     @staticmethod
     def set_graph_engine(graph_engine: object):
-        infrastructure_config.set_config({
-            "graph_engine": graph_engine
-        })
+        graph_config.graph_engine =graph_engine
 
     @staticmethod
     def llm_provider(llm_provider: str):
-        infrastructure_config.set_config({
-            "llm_provider": llm_provider
-        })
+        graph_config.llm_provider = llm_provider
+
+    @staticmethod
+    def llm_endpoint(llm_endpoint: str):
+        graph_config.llm_endpoint = llm_endpoint
+
+    @staticmethod
+    def llm_model(llm_model: str):
+        graph_config.llm_model = llm_model
 
     @staticmethod
     def intra_layer_score_treshold(intra_layer_score_treshold: str):
-        infrastructure_config.set_config({
-            "intra_layer_score_treshold": intra_layer_score_treshold
-        })
+        cognify_config.intra_layer_score_treshold =intra_layer_score_treshold
+
 
     @staticmethod
     def connect_documents(connect_documents: bool):
-        infrastructure_config.set_config({
-            "connect_documents": connect_documents
-        })
+        cognify_config.connect_documents = connect_documents
+
     @staticmethod
     def set_chunk_strategy(chunk_strategy: object):
-        infrastructure_config.set_config({
-            "chunk_strategy": chunk_strategy
-        })
+        chunk_config.chunk_strategy = chunk_strategy
+
+
+    @staticmethod
+    def set_graph_topology(graph_topology: object):
+        get_cognify_config.graph_topology =graph_topology
+
```

### Comparing `cognee-0.1.7/cognee/api/v1/prune/prune.py` & `cognee-0.1.8/cognee/api/v1/prune/prune.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,33 @@
+from cognee.base_config import get_base_config
 from cognee.infrastructure.files.storage import LocalStorage
 from cognee.infrastructure import infrastructure_config
 from cognee.infrastructure.databases.graph.get_graph_client import get_graph_client
+base_config =get_base_config()
+from cognee.infrastructure.databases.graph.config import get_graph_config
+from cognee.infrastructure.databases.vector.config import get_vectordb_config
+graph_config = get_graph_config()
+vector_config = get_vectordb_config()
 
 class prune():
     @staticmethod
     async def prune_data():
-        data_root_directory = infrastructure_config.get_config()["data_root_directory"]
+        data_root_directory = base_config.data_root_directory
         LocalStorage.remove_all(data_root_directory)
 
     @staticmethod
     async def prune_system(graph = True, vector = True):
         infra_config = infrastructure_config.get_config()
 
         if graph:
-            graph_client = await get_graph_client(infra_config["graph_engine"])
+            graph_client = await get_graph_client(graph_config.graph_engine)
             await graph_client.delete_graph()
 
         if vector:
-            vector_client = infra_config["vector_engine"]
+            vector_client = vector_config.vector_engine
             await vector_client.prune()
 
 
 if __name__ == "__main__":
     import asyncio
     async def main():
         await prune.prune_data()
```

### Comparing `cognee-0.1.7/cognee/api/v1/search/search.py` & `cognee-0.1.8/cognee/api/v1/search/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 """ This module contains the search function that is used to search for nodes in the graph."""
 import asyncio
 from enum import Enum
 from typing import Dict, Any, Callable, List
 from pydantic import BaseModel, field_validator
+
+from cognee.modules.search.graph import search_cypher
 from cognee.modules.search.graph.search_adjacent import search_adjacent
 from cognee.modules.search.vector.search_similarity import search_similarity
 from cognee.modules.search.graph.search_categories import search_categories
 from cognee.modules.search.graph.search_neighbour import search_neighbour
 from cognee.modules.search.graph.search_summary import search_summary
 from cognee.infrastructure.databases.graph.get_graph_client import get_graph_client
 from cognee.infrastructure import infrastructure_config
 from cognee.utils import send_telemetry
+from cognee.infrastructure.databases.graph.config import get_graph_config
+graph_config = get_graph_config()
 
 class SearchType(Enum):
     ADJACENT = 'ADJACENT'
     SIMILARITY = 'SIMILARITY'
     CATEGORIES = 'CATEGORIES'
     NEIGHBOR = 'NEIGHBOR'
     SUMMARY = 'SUMMARY'
+    SUMMARY_CLASSIFICATION = 'SUMMARY_CLASSIFICATION'
+    NODE_CLASSIFICATION = 'NODE_CLASSIFICATION'
+    DOCUMENT_CLASSIFICATION = 'DOCUMENT_CLASSIFICATION',
+    CYPHER = 'CYPHER'
 
     @staticmethod
     def from_str(name: str):
         try:
             return SearchType[name.upper()]
         except KeyError:
             raise ValueError(f"{name} is not a valid SearchType")
@@ -39,23 +47,25 @@
 
 async def search(search_type: str, params: Dict[str, Any]) -> List:
     search_params = SearchParameters(search_type = search_type, params = params)
     return await specific_search([search_params])
 
 
 async def specific_search(query_params: List[SearchParameters]) -> List:
-    graph_client = await get_graph_client(infrastructure_config.get_config()["graph_engine"])
+    graph_client = await get_graph_client(graph_config.graph_engine)
     graph = graph_client.graph
 
     search_functions: Dict[SearchType, Callable] = {
         SearchType.ADJACENT: search_adjacent,
         SearchType.SIMILARITY: search_similarity,
         SearchType.CATEGORIES: search_categories,
         SearchType.NEIGHBOR: search_neighbour,
-        SearchType.SUMMARY: search_summary
+        SearchType.SUMMARY: search_summary,
+        SearchType.CYPHER: search_cypher
+
     }
 
     results = []
     search_tasks = []
 
     for search_param in query_params:
         search_func = search_functions.get(search_param.search_type)
```

### Comparing `cognee-0.1.7/cognee/config.py` & `cognee-0.1.8/cognee/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,21 +4,26 @@
 import configparser
 import uuid
 from typing import Optional, Dict, Any
 from dataclasses import dataclass, field
 from pathlib import Path
 from dotenv import load_dotenv
 from cognee.root_dir import get_absolute_path
-from cognee.shared.data_models import ChunkStrategy
-
-base_dir = Path(__file__).resolve().parent.parent
-# Load the .env file from the base directory
-dotenv_path = base_dir / ".env"
-load_dotenv(dotenv_path=dotenv_path)
-
+from cognee.shared.data_models import ChunkStrategy, DefaultGraphModel
+logging.basicConfig(level=logging.DEBUG)
+def load_dontenv():
+    base_dir = Path(__file__).resolve().parent.parent
+    # Load the .env file from the base directory
+    dotenv_path = base_dir / ".env"
+    load_dotenv(dotenv_path=dotenv_path, override = True)
+
+try:
+    load_dontenv()
+except:
+    pass
 
 @dataclass
 class Config:
     """ Configuration for cognee - cognitive architecture framework. """
     cognee_dir: str = field(
         default_factory=lambda: os.getenv("COG_ARCH_DIR", "cognee")
     )
@@ -26,107 +31,87 @@
         default_factory=lambda: os.path.join(
             os.getenv("COG_ARCH_DIR", "cognee"), "config"
         )
     )
 
 
     system_root_directory = get_absolute_path(".cognee_system")
+    logging.info("system_root_directory: %s", system_root_directory)
     data_root_directory = os.getenv("DATA_PATH", get_absolute_path(".data"))
 
     vectordb: str = os.getenv("VECTORDB", "weaviate")
 
     qdrant_path: str = os.getenv("QDRANT_PATH", None)
     qdrant_url: str = os.getenv("QDRANT_URL", None)
     qdrant_api_key: str = os.getenv("QDRANT_API_KEY", None)
 
-    db_path = str = os.getenv("COGNEE_DB_PATH", "databases")
-    db_name: str = os.getenv("DB_NAME", "cognee.db")
-    db_host: str = os.getenv("DB_HOST", "localhost")
-    db_port: str = os.getenv("DB_PORT", "5432")
-    db_user: str = os.getenv("DB_USER", "cognee")
-    db_password: str = os.getenv("DB_PASSWORD", "cognee")
 
-    sqlalchemy_logging: bool = os.getenv("SQLALCHEMY_LOGGING", True)
 
     graph_filename = os.getenv("GRAPH_NAME", "cognee_graph.pkl")
 
     # Model parameters
-    llm_provider: str = os.getenv("LLM_PROVIDER","openai") #openai, or custom or ollama
-    custom_model: str = os.getenv("CUSTOM_LLM_MODEL", "mistralai/Mixtral-8x7B-Instruct-v0.1") #"mistralai/Mixtral-8x7B-Instruct-v0.1"
-    custom_endpoint: str = os.getenv("CUSTOM_ENDPOINT", "https://api.endpoints.anyscale.com/v1") #"https://api.endpoints.anyscale.com/v1" # pass claude endpoint
-    custom_key: Optional[str] = os.getenv("CUSTOM_LLM_API_KEY")
-    ollama_endpoint: str = os.getenv("CUSTOM_OLLAMA_ENDPOINT", "http://localhost:11434/v1") #"http://localhost:11434/v1"
-    ollama_key: Optional[str] = "ollama"
-    ollama_model: str = os.getenv("CUSTOM_OLLAMA_MODEL", "mistral:instruct") #"mistral:instruct"
-    openai_model: str = os.getenv("OPENAI_MODEL", "gpt-4-1106-preview" ) #"gpt-4-1106-preview"
-    model_endpoint: str = "openai"
-    openai_key: Optional[str] = os.getenv("OPENAI_API_KEY")
+    llm_provider: str = os.getenv("LLM_PROVIDER", "openai") #openai, or custom or ollama
+    llm_model: str = os.getenv("LLM_MODEL", "gpt-4")
+    llm_api_key: str = os.getenv("LLM_API_KEY", os.getenv("OPENAI_API_KEY"))
+    llm_endpoint: str = os.getenv("LLM_ENDPOINT", None)
+
+    # custom_model: str = os.getenv("CUSTOM_LLM_MODEL", "llama3-70b-8192") #"mistralai/Mixtral-8x7B-Instruct-v0.1"
+    # custom_endpoint: str = os.getenv("CUSTOM_ENDPOINT", "https://api.endpoints.anyscale.com/v1") #"https://api.endpoints.anyscale.com/v1" # pass claude endpoint
+    # custom_key: Optional[str] = os.getenv("CUSTOM_LLM_API_KEY")
+    # ollama_endpoint: str = os.getenv("CUSTOM_OLLAMA_ENDPOINT", "http://localhost:11434/v1") #"http://localhost:11434/v1"
+    # ollama_key: Optional[str] = "ollama"
+    # ollama_model: str = os.getenv("CUSTOM_OLLAMA_MODEL", "mistral:instruct") #"mistral:instruct"
+    # openai_model: str = os.getenv("OPENAI_MODEL", "gpt-4o" ) #"gpt-4o"
+    # model_endpoint: str = "openai"
+    # llm_api_key: Optional[str] = os.getenv("OPENAI_API_KEY")
     openai_temperature: float = float(os.getenv("OPENAI_TEMPERATURE", 0.0))
-    openai_embedding_model = "text-embedding-3-large"
-    openai_embedding_dimensions = 3072
+    # openai_embedding_model = "text-embedding-3-large"
+    # openai_embedding_dimensions = 3072
+    # litellm_embedding_model = "text-embedding-3-large"
+    # litellm_embedding_dimensions = 3072
 
     graphistry_username = os.getenv("GRAPHISTRY_USERNAME")
     graphistry_password = os.getenv("GRAPHISTRY_PASSWORD")
 
     # Embedding parameters
     embedding_model: str = "BAAI/bge-large-en-v1.5"
     embedding_dimensions: int = 1024
     connect_documents: bool = False
 
     # Database parameters
     graph_database_provider: str = os.getenv("GRAPH_DB_PROVIDER", "NETWORKX")
+    graph_topology:str = DefaultGraphModel
+    cognitive_layers_limit: int = 2
 
-    if (
-        os.getenv("ENV") == "prod"
-        or os.getenv("ENV") == "dev"
-        or os.getenv("AWS_ENV") == "dev"
-        or os.getenv("AWS_ENV") == "prd"
-    ):
-        load_dotenv()
-        logging.info("graph_db_url: %s", os.getenv("GRAPH_DB_URL_PROD"))
-        graph_database_url: str = os.getenv("GRAPH_DB_URL_PROD")
-        graph_database_username: str = os.getenv("GRAPH_DB_USER")
-        graph_database_password: str = os.getenv("GRAPH_DB_PW")
-    else:
-        logging.info("graph_db_url: %s", os.getenv("GRAPH_DB_URL"))
-        graph_database_url: str = os.getenv("GRAPH_DB_URL")
-        graph_database_username: str = os.getenv("GRAPH_DB_USER")
-        graph_database_password: str = os.getenv("GRAPH_DB_PW")
+    from cognee.shared.data_models import MonitoringTool
+
+    # Monitoring tool
+    monitoring_tool: str = os.getenv("MONITORING_TOOL", MonitoringTool.LANGFUSE)
 
     weaviate_url: str = os.getenv("WEAVIATE_URL")
     weaviate_api_key: str = os.getenv("WEAVIATE_API_KEY")
 
-    if (
-        os.getenv("ENV") == "prod"
-        or os.getenv("ENV") == "dev"
-        or os.getenv("AWS_ENV") == "dev"
-        or os.getenv("AWS_ENV") == "prd"
-    ):
-        load_dotenv()
-
-        db_host: str = os.getenv("POSTGRES_HOST")
-        logging.info("db_host: %s", db_host)
-        db_user: str = os.getenv("POSTGRES_USER")
-        db_password: str = os.getenv("POSTGRES_PASSWORD")
-        db_name: str = os.getenv("POSTGRES_DB")
-
     # Model parameters and configuration for interlayer scoring
     intra_layer_score_treshold: float = 0.98
 
 
     # Client ID
     anon_clientid: Optional[str] = field(default_factory=lambda: uuid.uuid4().hex)
 
     #Chunking parameters
-    chunk_size: int = 1500
-    chunk_overlap: int = 0
-    chunk_strategy: str = ChunkStrategy.PARAGRAPH
+    # chunk_size: int = 1500
+    # chunk_overlap: int = 0
+    # chunk_strategy: str = ChunkStrategy.PARAGRAPH
 
     def load(self):
         """Loads the configuration from a file or environment variables."""
+        try:
+            load_dontenv()
+        except:
+            pass
         config = configparser.ConfigParser()
         config.read(self.config_path)
 
         # Override with environment variables if they exist
         for attr in self.__annotations__:
             env_value = os.getenv(attr.upper())
             if env_value is not None:
```

### Comparing `cognee-0.1.7/cognee/fetch_secret.py` & `cognee-0.1.8/cognee/fetch_secret.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/infrastructure/InfrastructureConfig.py` & `cognee-0.1.8/cognee/infrastructure/InfrastructureConfig.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,64 @@
+import logging
+import os
+
 from cognee.config import Config
-from .databases.relational import DuckDBAdapter, DatabaseEngine
-from .databases.vector.vector_db_interface import VectorDBInterface
-from .databases.vector.embeddings.DefaultEmbeddingEngine import DefaultEmbeddingEngine
+from .data.chunking.config import get_chunk_config
+from .databases.relational import DatabaseEngine
 from .llm.llm_interface import LLMInterface
-from .llm.openai.adapter import OpenAIAdapter
+from .llm.get_llm_client import get_llm_client
 from .files.storage import LocalStorage
-from .data.chunking.DefaultChunkEngine import DefaultChunkEngine
 from ..shared.data_models import GraphDBType, DefaultContentPrediction, KnowledgeGraph, SummarizedContent, \
     LabeledContent, DefaultCognitiveLayer
 
+logging.basicConfig(level=logging.DEBUG)
 config = Config()
 config.load()
-
+from cognee.infrastructure.databases.relational.config import get_relationaldb_config
+from cognee.infrastructure.databases.vector.config import get_vectordb_config
+vector_db_config = get_vectordb_config()
+relational = get_relationaldb_config()
+chunk_config = get_chunk_config()
 class InfrastructureConfig():
+
     system_root_directory: str = config.system_root_directory
     data_root_directory: str = config.data_root_directory
     llm_provider: str = config.llm_provider
     database_engine: DatabaseEngine = None
-    vector_engine: VectorDBInterface = None
     graph_engine: GraphDBType = None
     llm_engine: LLMInterface = None
     classification_model = None
     summarization_model = None
     labeling_model = None
     graph_model = None
     cognitive_layer_model = None
     intra_layer_score_treshold = None
     embedding_engine = None
     connect_documents = config.connect_documents
     database_directory_path: str = None
     database_file_path: str = None
-    chunk_strategy = config.chunk_strategy
+    chunk_strategy = chunk_config.chunk_strategy
     chunk_engine = None
+    graph_topology = config.graph_topology
+    monitoring_tool = config.monitoring_tool
+    llm_provider: str = None
+    llm_model: str = None
+    llm_endpoint: str = None
+    llm_api_key: str = None
 
     def get_config(self, config_entity: str = None) -> dict:
+
         if (config_entity is None or config_entity == "database_engine") and self.database_engine is None:
-            db_path = self.system_root_directory + "/" + config.db_path
+
+
+            db_path = os.path.join(self.system_root_directory,relational.db_path)
 
             LocalStorage.ensure_directory_exists(db_path)
 
-            self.database_engine = DuckDBAdapter(
-                db_name = config.db_name,
-                db_path = db_path
-            )
+            self.database_engine = relational.db_engine
 
         if self.graph_engine is None:
             self.graph_engine = GraphDBType.NETWORKX
 
         if self.classification_model is None:
             self.classification_model = DefaultContentPrediction
 
@@ -61,73 +73,42 @@
 
         if self.cognitive_layer_model is None:
             self.cognitive_layer_model = DefaultCognitiveLayer
 
         if self.intra_layer_score_treshold is None:
             self.intra_layer_score_treshold = config.intra_layer_score_treshold
 
-        if self.embedding_engine is None:
-            self.embedding_engine = DefaultEmbeddingEngine()
-
         if self.connect_documents is None:
             self.connect_documents = config.connect_documents
 
         if self.chunk_strategy is None:
-            self.chunk_strategy = config.chunk_strategy
+            self.chunk_strategy = chunk_config.chunk_strategy
 
         if self.chunk_engine is None:
-            self.chunk_engine = DefaultChunkEngine()
+            self.chunk_engine = chunk_config.chunk_engine
+
+        if self.graph_topology is None:
+            self.graph_topology = config.graph_topology
 
         if (config_entity is None or config_entity == "llm_engine") and self.llm_engine is None:
-            self.llm_engine = OpenAIAdapter(config.openai_key, config.openai_model)
+            self.llm_engine = get_llm_client()
 
         if (config_entity is None or config_entity == "database_directory_path") and self.database_directory_path is None:
-            self.database_directory_path = self.system_root_directory + "/" + config.db_path
+            self.database_directory_path = self.system_root_directory + "/" + relational.db_path
+        if self.database_directory_path is None:
+            self.database_directory_path = self.system_root_directory + "/" + relational.db_path
 
         if (config_entity is None or config_entity == "database_file_path") and self.database_file_path is None:
-            self.database_file_path = self.system_root_directory + "/" + config.db_path + "/" + config.db_name
-
-        if (config_entity is None or config_entity == "vector_engine") and self.vector_engine is None:
-            try:
-                from .databases.vector.weaviate_db import WeaviateAdapter
-
-                if config.weaviate_url is None and config.weaviate_api_key is None:
-                    raise EnvironmentError("Weaviate is not configured!")
-
-                self.vector_engine = WeaviateAdapter(
-                    config.weaviate_url,
-                    config.weaviate_api_key,
-                    embedding_engine = self.embedding_engine
-                )
-            except (EnvironmentError, ModuleNotFoundError):
-                if config.qdrant_url and config.qdrant_api_key:
-                    from .databases.vector.qdrant.QDrantAdapter import QDrantAdapter
-
-                    self.vector_engine = QDrantAdapter(
-                        qdrant_url = config.qdrant_url,
-                        qdrant_api_key = config.qdrant_api_key,
-                        embedding_engine = self.embedding_engine
-                    )
-                else:
-                    from .databases.vector.lancedb.LanceDBAdapter import LanceDBAdapter
-                    lance_db_path = self.database_directory_path + "/cognee.lancedb"
-                    LocalStorage.ensure_directory_exists(lance_db_path)
-
-                    self.vector_engine = LanceDBAdapter(
-                        uri = lance_db_path,
-                        api_key = None,
-                        embedding_engine = self.embedding_engine,
-                    )
+            self.database_file_path = self.system_root_directory + "/" + relational.db_path + "/" + relational.db_name
 
         if config_entity is not None:
             return getattr(self, config_entity)
 
         return {
             "llm_engine": self.llm_engine,
-            "vector_engine": self.vector_engine,
             "database_engine": self.database_engine,
             "system_root_directory": self.system_root_directory,
             "data_root_directory": self.data_root_directory,
             "graph_engine": self.graph_engine,
             "classification_model": self.classification_model,
             "summarization_model": self.summarization_model,
             "labeling_model": self.labeling_model,
@@ -137,29 +118,27 @@
             "intra_layer_score_treshold": self.intra_layer_score_treshold,
             "embedding_engine": self.embedding_engine,
             "connect_documents": self.connect_documents,
             "database_directory_path": self.database_directory_path,
             "database_path": self.database_file_path,
             "chunk_strategy": self.chunk_strategy,
             "chunk_engine": self.chunk_engine,
+            "graph_topology": self.graph_topology
         }
 
     def set_config(self, new_config: dict):
         if "system_root_directory" in new_config:
             self.system_root_directory = new_config["system_root_directory"]
 
         if "data_root_directory" in new_config:
             self.data_root_directory = new_config["data_root_directory"]
 
         if "database_engine" in new_config:
             self.database_engine = new_config["database_engine"]
 
-        if "vector_engine" in new_config:
-            self.vector_engine = new_config["vector_engine"]
-
         if "llm_engine" in new_config:
             self.llm_engine = new_config["llm_engine"]
 
         if "graph_engine" in new_config:
             self.graph_engine = new_config["graph_engine"]
 
         if "classification_model" in new_config:
@@ -191,8 +170,11 @@
 
         if "chunk_strategy" in new_config:
             self.chunk_strategy = new_config["chunk_strategy"]
 
         if "chunk_engine" in new_config:
             self.chunk_engine = new_config["chunk_engine"]
 
+        if "graph_topology" in new_config:
+            self.graph_topology = new_config["graph_topology"]
+
 infrastructure_config = InfrastructureConfig()
```

### Comparing `cognee-0.1.7/cognee/infrastructure/data/chunking/DefaultChunkEngine.py` & `cognee-0.1.8/cognee/infrastructure/data/chunking/DefaultChunkEngine.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         if chunk_strategy == ChunkStrategy.PARAGRAPH:
             chunked_data = DefaultChunkEngine.chunk_data_by_paragraph(source_data,chunk_size, chunk_overlap)
         elif chunk_strategy == ChunkStrategy.SENTENCE:
             chunked_data = DefaultChunkEngine.chunk_by_sentence(source_data, chunk_size, chunk_overlap)
         elif chunk_strategy == ChunkStrategy.EXACT:
             chunked_data = DefaultChunkEngine.chunk_data_exact(source_data, chunk_size, chunk_overlap)
 
+
         return chunked_data
 
 
     @staticmethod
     def chunk_data_exact(data_chunks, chunk_size, chunk_overlap):
         data = "".join(data_chunks)
         chunks = []
```

### Comparing `cognee-0.1.7/cognee/infrastructure/data/models/Data.py` & `cognee-0.1.8/cognee/infrastructure/data/models/Data.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/infrastructure/data/models/Dataset.py` & `cognee-0.1.8/cognee/infrastructure/data/models/Dataset.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/infrastructure/data/models/DatasetData.py` & `cognee-0.1.8/cognee/infrastructure/data/models/DatasetData.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/infrastructure/data/utils/extract_keywords.py` & `cognee-0.1.8/cognee/infrastructure/data/utils/extract_keywords.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/infrastructure/databases/graph/get_graph_client.py` & `cognee-0.1.8/cognee/infrastructure/databases/graph/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,40 @@
-"""Factory function to get the appropriate graph client based on the graph type."""
-
-from cognee.config import Config
-from cognee.shared.data_models import GraphDBType
-from cognee.infrastructure import infrastructure_config
-from .graph_db_interface import GraphDBInterface
-from .networkx.adapter import NetworkXAdapter
-
-config = Config()
-config.load()
-
-
-async def get_graph_client(graph_type: GraphDBType, graph_file_name: str = None) -> GraphDBInterface :
-    """Factory function to get the appropriate graph client based on the graph type."""
-    graph_file_path = f"{infrastructure_config.get_config('database_directory_path')}/{graph_file_name if graph_file_name else config.graph_filename}"
-
-    if graph_type == GraphDBType.NEO4J:
-        try:
-            from .neo4j_driver.adapter import Neo4jAdapter
-
-            return Neo4jAdapter(
-                graph_database_url = config.graph_database_url,
-                graph_database_username = config.graph_database_username,
-                graph_database_password = config.graph_database_password
-            )
-        except:
-            pass
-            
-    graph_client = NetworkXAdapter(filename = graph_file_path)
-
-
-    if (graph_client.graph is None):
-        await graph_client.load_graph_from_file()
-
-    return graph_client
+""" This module contains the configuration for the graph database. """
+import os
+from functools import lru_cache
+from pydantic_settings import BaseSettings, SettingsConfigDict
+from cognee.base_config import get_base_config
+from cognee.infrastructure.databases.relational.config import get_relationaldb_config
+from cognee.shared.data_models import DefaultGraphModel, GraphDBType
+relational_config = get_relationaldb_config()
+base_config = get_base_config()
+
+class GraphConfig(BaseSettings):
+    graph_filename: str = "cognee_graph.pkl"
+    graph_database_provider: str = "NETWORKX"
+    graph_database_url: str = ""
+    graph_database_username: str = ""
+    graph_database_password: str = ""
+    graph_database_port: int = 123
+    graph_file_path: str = os.path.join(relational_config.database_directory_path,graph_filename)
+    graph_engine: object =  GraphDBType.NETWORKX
+    graph_model: object = DefaultGraphModel
+
+    model_config = SettingsConfigDict(env_file = ".env", extra = "allow")
+
+    def to_dict(self) -> dict:
+        return {
+            "graph_filename": self.graph_filename,
+            "graph_database_provider": self.graph_database_provider,
+            "graph_topology": self.graph_topology,
+            "graph_file_path": self.graph_file_path,
+            "graph_database_url": self.graph_database_url,
+            "graph_database_username": self.graph_database_username,
+            "graph_database_password": self.graph_database_password,
+            "graph_database_port": self.graph_database_port,
+            "graph_engine": self.graph_engine
+
+        }
+
+@lru_cache
+def get_graph_config():
+    return GraphConfig()
```

### Comparing `cognee-0.1.7/cognee/infrastructure/databases/graph/graph_db_interface.py` & `cognee-0.1.8/cognee/infrastructure/databases/graph/graph_db_interface.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/infrastructure/databases/graph/neo4j_driver/adapter.py` & `cognee-0.1.8/cognee/infrastructure/databases/graph/falkordb/adapter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,53 @@
-""" Neo4j Adapter for Graph Database"""
+""" FalcorDB Adapter for Graph Database"""
 import json
 import logging
 from typing import Optional, Any, List, Dict
 from contextlib import asynccontextmanager
-from neo4j import AsyncSession
-from neo4j import AsyncGraphDatabase
-from neo4j.exceptions import Neo4jError
+
+
+from falkordb.asyncio import FalkorDB
 from cognee.infrastructure.databases.graph.graph_db_interface import GraphDBInterface
 
-logger = logging.getLogger("Neo4jAdapter")
+logger = logging.getLogger("FalcorDBAdapter")
 
-class Neo4jAdapter(GraphDBInterface):
+class FalcorDBAdapter(GraphDBInterface):
     def __init__(
         self,
         graph_database_url: str,
         graph_database_username: str,
         graph_database_password: str,
+        graph_database_port: int,
         driver: Optional[Any] = None,
+        graph_name: str = "DefaultGraph",
     ):
-        self.driver = driver or AsyncGraphDatabase.driver(
-            graph_database_url,
-            auth = (graph_database_username, graph_database_password)
-        )
-
-    async def close(self) -> None:
-        await self.driver.close()
-
-    @asynccontextmanager
-    async def get_session(self) -> AsyncSession:
-        async with self.driver.session() as session:
-            yield session
+        self.driver = FalkorDB(
+            host = graph_database_url,
+            port = graph_database_port)
+        self.graph_name = graph_name
+
+
 
     async def query(
         self,
         query: str,
         params: Optional[Dict[str, Any]] = None,
     ) -> List[Dict[str, Any]]:
         try:
-            async with self.get_session() as session:
-                result = await session.run(query, parameters=params)
-                data = await result.data()
-                await self.close()
-                return data
-        except Neo4jError as error:
-            logger.error("Neo4j query error: %s", error, exc_info = True)
+                selected_graph = self.driver.select_graph(self.graph_name)
+
+                result = await selected_graph.query(query)
+                return result.result_set
+
+        except Exception as error:
+            logger.error("Falkor query error: %s", error, exc_info = True)
             raise error
 
     async def graph(self):
-        return await self.get_session()
+        return  self.driver
 
     async def add_node(self, node_id: str, node_properties: Dict[str, Any] = None):
         node_id = node_id.replace(":", "_")
 
         serialized_properties = self.serialize_properties(node_properties)
 
         if "name" not in serialized_properties:
@@ -82,36 +78,14 @@
 
             await self.add_node(
                 node_id = node_id,
                 node_properties = node_properties,
             )
 
 
-        #     serialized_properties = self.serialize_properties(node_properties)
-
-        #     if "name" not in serialized_properties:
-        #         serialized_properties["name"] = node_id
-
-        #     nodes_data.append({
-        #         "node_id": node_id,
-        #         "properties": serialized_properties,
-        #     })
-
-        # query = """UNWIND $nodes_data AS node_data
-        #         MERGE (node:{id: node_data.node_id})
-        #         ON CREATE SET node += node_data.properties
-        #         RETURN ID(node) AS internal_id, node.id AS id"""
-
-        # params = {"nodes_data": nodes_data}
-
-        # result = await self.query(query, params)
-
-        # await self.close()
-
-        # return result
 
     async def extract_node_description(self, node_id: str):
         query = """MATCH (n)-[r]->(m)
                     WHERE n.id = $node_id
                     AND NOT m.id CONTAINS 'DefaultGraphModel'
                     RETURN m
                     """
@@ -188,37 +162,14 @@
             await self.add_edge(
                 from_node = from_node,
                 to_node = to_node,
                 relationship_name = relationship_name,
                 edge_properties = edge_properties
             )
 
-            # Filter out None values and do not serialize; Neo4j can handle complex types like arrays directly
-        #     serialized_properties = self.serialize_properties(edge_properties)
-
-        #     edges_data.append({
-        #         "from_node": from_node,
-        #         "to_node": to_node,
-        #         "relationship_name": relationship_name,
-        #         "properties": serialized_properties
-        #     })
-
-        # query = """UNWIND $edges_data AS edge_data
-        #         MATCH (from_node:{id: edge_data.from_node}), (to_node:{id: edge_data.to_node})
-        #         MERGE (from_node)-[r:{edge_data.relationship_name}]->(to_node)
-        #         ON CREATE SET r += edge_data.properties
-        #         RETURN r"""
-
-        # params = {"edges_data": edges_data}
-
-        # result = await self.query(query, params)
-
-        # await self.close()
-
-        # return result
 
 
     async def filter_nodes(self, search_criteria):
         query = f"""MATCH (node)
                 WHERE node.id CONTAINS '{search_criteria}'
                 RETURN node"""
```

### Comparing `cognee-0.1.7/cognee/infrastructure/databases/graph/networkx/adapter.py` & `cognee-0.1.8/cognee/infrastructure/databases/graph/networkx/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 
     async def add_nodes(
         self,
         nodes: List[tuple[str, dict]],
     ) -> None:
         self.graph.add_nodes_from(nodes)
         await self.save_graph_to_file(self.filename)
+
+    async def get_graph(self):
+        return self.graph
     
     async def add_edge(
         self,
         from_node: str,
         to_node: str,
         relationship_name: str,
         edge_properties: Dict[str, Any] = None,
```

### Comparing `cognee-0.1.7/cognee/infrastructure/databases/relational/relational_db_interface.py` & `cognee-0.1.8/cognee/infrastructure/databases/relational/relational_db_interface.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/infrastructure/databases/relational/sqlite/SqliteEngine.py` & `cognee-0.1.8/cognee/infrastructure/databases/relational/sqlite/SqliteEngine.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/infrastructure/databases/relational/utils/with_rollback.py` & `cognee-0.1.8/cognee/infrastructure/databases/relational/utils/with_rollback.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/infrastructure/databases/vector/lancedb/LanceDBAdapter.py` & `cognee-0.1.8/cognee/infrastructure/databases/vector/lancedb/LanceDBAdapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 from typing import List, Optional, get_type_hints, Generic, TypeVar
 import asyncio
-from pydantic import BaseModel, Field
 import lancedb
 from lancedb.pydantic import Vector, LanceModel
 from cognee.infrastructure.files.storage import LocalStorage
 from ..models.ScoredResult import ScoredResult
 from ..vector_db_interface import VectorDBInterface, DataPoint
 from ..embeddings.EmbeddingEngine import EmbeddingEngine
 
 class LanceDBAdapter(VectorDBInterface):
+    name = "LanceDB"
+    url: str
+    api_key: str
     connection: lancedb.AsyncConnection = None
 
+
     def __init__(
         self,
-        uri: Optional[str],
+        url: Optional[str],
         api_key: Optional[str],
         embedding_engine: EmbeddingEngine,
     ):
-        self.uri = uri
+        self.url = url
         self.api_key = api_key
         self.embedding_engine = embedding_engine
 
     async def get_connection(self):
         if self.connection is None:
-            self.connection = await lancedb.connect_async(self.uri, api_key = self.api_key)
+            self.connection = await lancedb.connect_async(self.url, api_key = self.api_key)
 
         return self.connection
 
     async def embed_data(self, data: list[str]) -> list[list[float]]:
         return await self.embedding_engine.embed_text(data)
 
     async def collection_exists(self, collection_name: str) -> bool:
         connection = await self.get_connection()
         collection_names = await connection.table_names()
         return collection_name in collection_names
 
-    async def create_collection(self, collection_name: str, payload_schema: BaseModel):
+    async def create_collection(self, collection_name: str, payload_schema = None):
         data_point_types = get_type_hints(DataPoint)
+        vector_size = self.embedding_engine.get_vector_size()
 
         class LanceDataPoint(LanceModel):
-            id: data_point_types["id"] = Field(...)
-            vector: Vector(self.embedding_engine.get_vector_size())
+            id: data_point_types["id"]
+            vector: Vector(vector_size)
             payload: payload_schema
 
         if not await self.collection_exists(collection_name):
             connection = await self.get_connection()
             return await connection.create_table(
                 name = collection_name,
                 schema = LanceDataPoint,
@@ -64,18 +68,19 @@
 
         data_vectors = await self.embed_data(
             [data_point.get_embeddable_data() for data_point in data_points]
         )
 
         IdType = TypeVar("IdType")
         PayloadSchema = TypeVar("PayloadSchema")
+        vector_size = self.embedding_engine.get_vector_size()
 
         class LanceDataPoint(LanceModel, Generic[IdType, PayloadSchema]):
             id: IdType
-            vector: Vector(self.embedding_engine.get_vector_size())
+            vector: Vector(vector_size)
             payload: PayloadSchema
 
         lance_data_points = [
             LanceDataPoint[type(data_point.id), type(data_point.payload)](
                 id = data_point.id,
                 vector = data_vectors[data_index],
                 payload = data_point.payload,
@@ -122,24 +127,24 @@
         ) for result in results.to_dict("index").values()]
 
     async def batch_search(
         self,
         collection_name: str,
         query_texts: List[str],
         limit: int = None,
-        with_vector: bool = False,
+        with_vectors: bool = False,
     ):
         query_vectors = await self.embedding_engine.embed_text(query_texts)
 
         return asyncio.gather(
             *[self.search(
                 collection_name = collection_name,
                 query_vector = query_vector,
                 limit = limit,
-                with_vector = with_vector,
+                with_vector = with_vectors,
             ) for query_vector in query_vectors]
         )
 
     async def prune(self):
         # Clean up the database if it was set up as temporary
-        if self.uri.startswith("/"):
-            LocalStorage.remove_all(self.uri) # Remove the temporary directory and files inside
+        if self.url.startswith("/"):
+            LocalStorage.remove_all(self.url) # Remove the temporary directory and files inside
```

### Comparing `cognee-0.1.7/cognee/infrastructure/databases/vector/qdrant/QDrantAdapter.py` & `cognee-0.1.8/cognee/infrastructure/databases/vector/qdrant/QDrantAdapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,37 +22,37 @@
 
 def create_quantization_config(quantization_config: Dict):
     if quantization_config is not None:
         return models.QuantizationConfig()
     return None
 
 class QDrantAdapter(VectorDBInterface):
-    qdrant_url: str = None
+    name = "Qdrant"
+    url: str = None
+    api_key: str = None
     qdrant_path: str = None
-    qdrant_api_key: str = None
 
-    def __init__(self, qdrant_url, qdrant_api_key, embedding_engine: EmbeddingEngine, qdrant_path = None):
+    def __init__(self, url, api_key, embedding_engine: EmbeddingEngine, qdrant_path = None):
         self.embedding_engine = embedding_engine
 
         if qdrant_path is not None:
             self.qdrant_path = qdrant_path
         else:
-            self.qdrant_url = qdrant_url
-
-        self.qdrant_api_key = qdrant_api_key
+            self.url = url
+            self.api_key = api_key
 
     def get_qdrant_client(self) -> AsyncQdrantClient:
         if self.qdrant_path is not None:
             return AsyncQdrantClient(
                 path = self.qdrant_path, port=6333
             )
-        elif self.qdrant_url is not None:
+        elif self.url is not None:
             return AsyncQdrantClient(
-                url = self.qdrant_url,
-                api_key = self.qdrant_api_key,
+                url = self.url,
+                api_key = self.api_key,
                 port = 6333
             )
 
         return AsyncQdrantClient(
             location = ":memory:"
         )
```

### Comparing `cognee-0.1.7/cognee/infrastructure/databases/vector/vector_db_interface.py` & `cognee-0.1.8/cognee/infrastructure/databases/vector/vector_db_interface.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/infrastructure/databases/vector/weaviate_db/WeaviateAdapter.py` & `cognee-0.1.8/cognee/infrastructure/databases/vector/weaviate_db/WeaviateAdapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import asyncio
 from uuid import UUID
 from typing import List, Optional
-from multiprocessing import Pool
 from ..vector_db_interface import VectorDBInterface
 from ..models.DataPoint import DataPoint
 from ..models.ScoredResult import ScoredResult
 from ..embeddings.EmbeddingEngine import EmbeddingEngine
 
 
 class WeaviateAdapter(VectorDBInterface):
-    async_pool: Pool = None
+    name = "Weaviate"
+    url: str
+    api_key: str
     embedding_engine: EmbeddingEngine = None
 
     def __init__(self, url: str, api_key: str, embedding_engine: EmbeddingEngine):
         import weaviate
         import weaviate.classes as wvc
-      
+
+        self.url = url
+        self.api_key = api_key
+
         self.embedding_engine = embedding_engine
 
         self.client = weaviate.connect_to_wcs(
-            cluster_url=url,
-            auth_credentials=weaviate.auth.AuthApiKey(api_key),
-            additional_config=wvc.init.AdditionalConfig(timeout=wvc.init.Timeout(init=30))
+            cluster_url = url,
+            auth_credentials = weaviate.auth.AuthApiKey(api_key),
+            additional_config = wvc.init.AdditionalConfig(timeout = wvc.init.Timeout(init=30))
         )
 
     async def embed_data(self, data: List[str]) -> List[float]:
         return await self.embedding_engine.embed_text(data)
 
     async def collection_exists(self, collection_name: str) -> bool:
         future = asyncio.Future()
```

### Comparing `cognee-0.1.7/cognee/infrastructure/files/storage/LocalStorage.py` & `cognee-0.1.8/cognee/infrastructure/files/storage/LocalStorage.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,20 +15,25 @@
         LocalStorage.ensure_directory_exists(self.storage_path)
 
         with open(
             full_file_path,
             mode = "w" if isinstance(data, str) else "wb",
             encoding = "utf-8" if isinstance(data, str) else None
         ) as f:
-            f.write(data if isinstance(data, str) else data.read())
+            if hasattr(data, "read"):
+                data.seek(0)
+                f.write(data.read())
+            else:
+                f.write(data)
 
     def retrieve(self, file_path: str, mode: str = "rb"):
         full_file_path = self.storage_path + "/" + file_path
 
         with open(full_file_path, mode = mode) as f:
+            f.seek(0)
             return f.read()
 
     @staticmethod
     def ensure_directory_exists(file_path: str):
         if not os.path.exists(file_path):
             os.makedirs(file_path)
```

### Comparing `cognee-0.1.7/cognee/infrastructure/files/storage/StorageManager.py` & `cognee-0.1.8/cognee/infrastructure/files/storage/StorageManager.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/infrastructure/files/utils/get_file_metadata.py` & `cognee-0.1.8/cognee/infrastructure/files/utils/get_file_metadata.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,23 +7,31 @@
 class FileMetadata(TypedDict):
     name: str
     mime_type: str
     extension: str
     keywords: list[str]
 
 def get_file_metadata(file: BinaryIO) -> FileMetadata:
+    """Get metadata from a file"""
     file.seek(0)
     file_type = guess_file_type(file)
 
     file.seek(0)
     file_text = extract_text_from_file(file, file_type)
-    keywords = extract_keywords(file_text)
+
+    import uuid
+
+    try:
+        keywords = extract_keywords(file_text)
+    except:
+        keywords = ["no keywords detected" + str(uuid.uuid4())]
+
 
     file_path = file.name
-    file_name = file_path.split("/")[-1].split(".")[0]
+    file_name = file_path.split("/")[-1].split(".")[0] if file_path else None
 
     return FileMetadata(
         name = file_name,
         file_path = file_path,
         mime_type = file_type.mime,
         extension = file_type.extension,
         keywords = keywords
```

### Comparing `cognee-0.1.7/cognee/infrastructure/files/utils/is_text_content.py` & `cognee-0.1.8/cognee/infrastructure/files/utils/is_text_content.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 def is_text_content(content):
+    """Check if the content is text."""
     # Check for null bytes
     if b'\0' in content:
         return False
 
     # Check for common text encodings (BOMs)
     if content.startswith((b'\xEF\xBB\xBF',  # UTF-8
                             b'\xFF\xFE',      # UTF-16 LE
```

### Comparing `cognee-0.1.7/cognee/infrastructure/llm/anthropic/adapter.py` & `cognee-0.1.8/cognee/infrastructure/llm/anthropic/adapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 from tenacity import retry, stop_after_attempt
 import anthropic
 from cognee.infrastructure.llm.llm_interface import LLMInterface
 from cognee.infrastructure.llm.prompts import read_query_prompt
 
 
 class AnthropicAdapter(LLMInterface):
-    """Adapter for Ollama's API"""
+    """Adapter for Anthropic API"""
+    name = "Anthropic"
+    model: str
 
     def __init__(self, model: str = None):
         self.aclient = instructor.patch(
             create = anthropic.Anthropic().messages.create,
             mode = instructor.Mode.ANTHROPIC_TOOLS
         )
         self.model = model
```

### Comparing `cognee-0.1.7/cognee/infrastructure/llm/generic_llm_api/adapter.py` & `cognee-0.1.8/cognee/infrastructure/llm/generic_llm_api/adapter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,62 @@
+'''Adapter for Generic API LLM provider API'''
 import asyncio
 from typing import List, Type
 from pydantic import BaseModel
 import instructor
 from tenacity import retry, stop_after_attempt
-from openai import AsyncOpenAI
 import openai
+
+
+from cognee.infrastructure import infrastructure_config
 from cognee.infrastructure.llm.llm_interface import LLMInterface
 from cognee.infrastructure.llm.prompts import read_query_prompt
-
+from cognee.shared.data_models import MonitoringTool
+from cognee.base_config import get_base_config
+from cognee.infrastructure.llm.config import get_llm_config
+
+llm_config = get_llm_config()
+base_config = get_base_config()
+
+if base_config.monitoring_tool == MonitoringTool.LANGFUSE:
+    from langfuse.openai import AsyncOpenAI, OpenAI
+elif base_config.monitoring_tool == MonitoringTool.LANGSMITH:
+    from langsmith import wrappers
+    from openai import AsyncOpenAI
+    AsyncOpenAI = wrappers.wrap_openai(AsyncOpenAI())
+else:
+    from openai import AsyncOpenAI, OpenAI
 
 class GenericAPIAdapter(LLMInterface):
-    """Adapter for Ollama's API"""
+    """Adapter for Generic API LLM provider API """
+    name: str
+    model: str
+    api_key: str
 
-    def __init__(self, api_endpoint, api_key: str, model: str):
-        self.aclient =  instructor.patch(
-            AsyncOpenAI(
-                base_url = api_endpoint,
-                api_key = api_key,  # required, but unused
-            ),
-            mode = instructor.Mode.JSON,
-        )
+    def __init__(self, api_endpoint, api_key: str, model: str, name: str):
+        self.name = name
         self.model = model
+        self.api_key = api_key
+
+        if llm_config.llm_provider == "groq":
+            from groq import groq
+            self.aclient = instructor.from_openai(
+                client = groq.Groq(
+                  api_key = api_key,
+                ),
+                mode = instructor.Mode.MD_JSON
+            )
+        else:
+            self.aclient = instructor.patch(
+                AsyncOpenAI(
+                    base_url = api_endpoint,
+                    api_key = api_key,  # required, but unused
+                ),
+                mode = instructor.Mode.JSON,
+            )
 
     @retry(stop = stop_after_attempt(5))
     def completions_with_backoff(self, **kwargs):
         """Wrapper around ChatCompletion.create w/ backoff"""
         # Local model
         return openai.chat.completions.create(**kwargs)
 
@@ -71,28 +103,29 @@
                       for text, model in zip(texts, models))
 
         # Run the coroutines in parallel and gather the results
         embeddings = await asyncio.gather(*coroutines)
 
         return embeddings
 
-    @retry(stop=stop_after_attempt(5))
-    async def acreate_structured_output(self, text_input: str, system_prompt: str,
-                                        response_model: Type[BaseModel]) -> BaseModel:
+    @retry(stop = stop_after_attempt(5))
+    async def acreate_structured_output(self, text_input: str, system_prompt: str, response_model: Type[BaseModel]) -> BaseModel:
         """Generate a response from a user query."""
+
         return await self.aclient.chat.completions.create(
-            model=self.model,
-            messages=[
+            model = self.model,
+            messages = [
                 {
                     "role": "user",
                     "content": f"""Use the given format to
-                    extract information from the following input: {text_input}. {system_prompt} """,
-                }
+                    extract information from the following input: {text_input}. """,
+                },
+                {"role": "system", "content": system_prompt},
             ],
-            response_model=response_model,
+            response_model = response_model,
         )
 
     def show_prompt(self, text_input: str, system_prompt: str) -> str:
         """Format and display the prompt for a user query."""
         if not text_input:
             text_input = "No user input provided."
         if not system_prompt:
```

### Comparing `cognee-0.1.7/cognee/infrastructure/llm/openai/adapter.py` & `cognee-0.1.8/cognee/infrastructure/llm/openai/adapter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,46 @@
 import asyncio
 from typing import List, Type
 import openai
 import instructor
-from openai import AsyncOpenAI, OpenAI
 from pydantic import BaseModel
 from tenacity import retry, stop_after_attempt
+
+from cognee.base_config import get_base_config
+from cognee.config import Config
+from cognee.infrastructure.llm import get_llm_config
 from cognee.infrastructure.llm.llm_interface import LLMInterface
 from cognee.infrastructure.llm.prompts import read_query_prompt
+from cognee.shared.data_models import MonitoringTool
+
+config = Config()
+config.load()
+llm_config = get_llm_config()
+base_config = get_base_config()
+
+if base_config.monitoring_tool == MonitoringTool.LANGFUSE:
+    from langfuse.openai import AsyncOpenAI, OpenAI
+elif base_config.monitoring_tool == MonitoringTool.LANGSMITH:
+    from langsmith import wrappers
+    from openai import AsyncOpenAI
+    AsyncOpenAI = wrappers.wrap_openai(AsyncOpenAI())
+else:
+    from openai import AsyncOpenAI, OpenAI
 
 class OpenAIAdapter(LLMInterface):
+    name = "OpenAI"
+    model: str
+    api_key: str
+  
     """Adapter for OpenAI's GPT-3, GPT=4 API"""
     def __init__(self, api_key: str, model:str):
-        openai.api_key = api_key
-        self.aclient = instructor.from_openai(AsyncOpenAI())
-        self.client = instructor.from_openai(OpenAI())
+        self.aclient = instructor.from_openai(AsyncOpenAI(api_key = api_key))
+        self.client = instructor.from_openai(OpenAI(api_key = api_key))
         self.model = model
+        self.api_key = api_key
 
     @retry(stop = stop_after_attempt(5))
     def completions_with_backoff(self, **kwargs):
         """Wrapper around ChatCompletion.create w/ backoff"""
         return openai.chat.completions.create(**kwargs)
 
     @retry(stop = stop_after_attempt(5))
```

### Comparing `cognee-0.1.7/cognee/infrastructure/llm/prompts/classify_content.txt` & `cognee-0.1.8/cognee/infrastructure/llm/prompts/classify_content.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/infrastructure/llm/prompts/generate_cog_layers.txt` & `cognee-0.1.8/cognee/infrastructure/llm/prompts/generate_cog_layers.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/infrastructure/llm/prompts/generate_graph_prompt.txt` & `cognee-0.1.8/cognee/infrastructure/llm/prompts/generate_graph_prompt.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/infrastructure/llm/prompts/read_query_prompt.py` & `cognee-0.1.8/cognee/infrastructure/llm/prompts/read_query_prompt.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/infrastructure/llm/prompts/render_prompt.py` & `cognee-0.1.8/cognee/infrastructure/llm/prompts/render_prompt.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/infrastructure/pipeline/models/Operation.py` & `cognee-0.1.8/cognee/infrastructure/pipeline/models/Operation.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/modules/cognify/dataset.py` & `cognee-0.1.8/cognee/modules/cognify/dataset.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/modules/cognify/evaluate.py` & `cognee-0.1.8/cognee/modules/cognify/evaluate.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         ) for example in dataset.dev
     ]
 
     devset = [example.with_inputs("context", "question") for example in evaluate_examples]
 
     evaluate_on_hotpotqa = Evaluate(devset = devset, num_threads = 1, display_progress = True, display_table = 5, max_tokens = 4096)
 
-    gpt4 = dspy.OpenAI(model = config.openai_model, api_key = config.openai_key, model_type = "chat", max_tokens = 4096)
+    gpt4 = dspy.OpenAI(model = config.llm_model, api_key = config.llm_api_key, model_type = "chat", max_tokens = 4096)
     compiled_extract_knowledge_graph = ExtractKnowledgeGraph(lm = gpt4)
     compiled_extract_knowledge_graph.load(get_absolute_path("./programs/extract_knowledge_graph/extract_knowledge_graph.json"))
 
     def evaluate_answer(example, graph_prediction, trace = None):
         llm_client = get_llm_client()
 
         try:
@@ -54,15 +54,15 @@
             )
         except:
             return False
 
         return dsp.answer_match(example.answer, [answer_prediction.answer], frac = 0.8) or \
             dsp.passage_match([example.answer], [answer_prediction.answer])
 
-    gpt4 = dspy.OpenAI(model = config.openai_model, api_key = config.openai_key, model_type = "chat", max_tokens = 4096)
+    gpt4 = dspy.OpenAI(model = config.llm_model, api_key = config.llm_api_key, model_type = "chat", max_tokens = 4096)
     dspy.settings.configure(lm = gpt4)
 
     evaluate_on_hotpotqa(compiled_extract_knowledge_graph, metric = evaluate_answer)
 
 
 if __name__ == "__main__":
     evaluate()
```

### Comparing `cognee-0.1.7/cognee/modules/cognify/graph/add_classification_nodes.py` & `cognee-0.1.8/cognee/modules/cognify/graph/add_classification_nodes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import List
 
 async def add_classification_nodes(graph_client, parent_node_id: str, categories: List) -> None:
     for category in categories:
         data_type = category["data_type"].upper().replace(" ", "_")
         category_name = category["category_name"].upper().replace(" ", "_").replace("'", "").replace("/", "_")
 
-        data_type_node_id = f"DATA_TYPE__{data_type}"
+        data_type_node_id = data_type
 
         data_type_node = await graph_client.extract_node(data_type_node_id)
 
         if not data_type_node:
-            data_type_node = await graph_client.add_node(data_type_node_id, dict(name = data_type, entity_type = "DataType"))
+            data_type_node = await graph_client.add_node(data_type_node_id, dict(name = data_type, type = "DataType"))
 
         await graph_client.add_edge(data_type_node_id, parent_node_id, "classified_as", dict(relationship_name = "classified_as"))
 
-        category_node_id = f"DATA_CATEGORY__{category_name}"
+        category_node_id = category_name
 
         category_node = await graph_client.extract_node(category_node_id)
 
         if not category_node:
-            category_node = await graph_client.add_node(category_node_id, dict(name = category_name, entity_type = "DataCategory"))
+            category_node = await graph_client.add_node(category_node_id, dict(name = category_name, type = "DataCategory"))
 
         await graph_client.add_edge(category_node_id, parent_node_id, "classified_as", dict(relationship_name = "classified_as"))
```

### Comparing `cognee-0.1.7/cognee/modules/cognify/graph/add_cognitive_layer_graphs.py` & `cognee-0.1.8/cognee/modules/cognify/graph/add_cognitive_layer_graphs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,108 +1,117 @@
 from datetime import datetime
 from uuid import uuid4
 from typing import List, Tuple, TypedDict
 from pydantic import BaseModel
-from cognee.infrastructure import infrastructure_config
 from cognee.infrastructure.databases.vector import DataPoint
-from cognee.shared.data_models import KnowledgeGraph
-from cognee.utils import extract_pos_tags, extract_named_entities, extract_sentiment_vader
-
+# from cognee.utils import extract_pos_tags, extract_named_entities, extract_sentiment_vader
+from cognee.infrastructure.databases.graph.config import get_graph_config
+from cognee.infrastructure.databases.vector.config import get_vectordb_config
+graph_config = get_graph_config()
+vectordb_config = get_vectordb_config()
 class GraphLike(TypedDict):
     nodes: List
     edges: List
 
 
 async def add_cognitive_layer_graphs(
     graph_client,
     chunk_collection: str,
     chunk_id: str,
     layer_graphs: List[Tuple[str, GraphLike]],
 ):
-    vector_client = infrastructure_config.get_config("vector_engine")
+    vector_client = vectordb_config.vector_engine
+    graph_model = graph_config.graph_model
 
     for (layer_id, layer_graph) in layer_graphs:
         graph_nodes = []
         graph_edges = []
 
-        if not isinstance(layer_graph, KnowledgeGraph):
-            layer_graph = KnowledgeGraph.parse_obj(layer_graph)
+        if not isinstance(layer_graph, graph_model):
+            layer_graph = graph_model.parse_obj(layer_graph)
 
         for node in layer_graph.nodes:
-            node_id = generate_proposition_node_id(node.id)
+            node_id = generate_node_id(node.id)
 
-            entity_type_node_id = generate_type_node_id(node.entity_type)
-            entity_type_node = await graph_client.extract_node(entity_type_node_id)
+            type_node_id = generate_node_id(node.type)
+            type_node = await graph_client.extract_node(type_node_id)
 
-            if not entity_type_node:
-                node_name = node.entity_type.lower().capitalize()
+            if not type_node:
+                node_name = node.type.lower().capitalize()
               
-                entity_type_node = (
-                    entity_type_node_id,
+                type_node = (
+                    type_node_id,
                     dict(
-                        id = entity_type_node_id,
+                        id = type_node_id,
                         name = node_name,
-                        entity_type = node_name,
+                        type = node_name,
                         created_at = datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
                         updated_at = datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
                     )
                 )
 
-                graph_nodes.append(entity_type_node)
+                graph_nodes.append(type_node)
 
                 # Add relationship between document and entity type: "Document contains Person"
                 graph_edges.append((
                     layer_id,
-                    entity_type_node_id,
+                    type_node_id,
                     "contains",
                     dict(relationship_name = "contains"),
                 ))
 
-            pos_tags = extract_pos_tags(node.entity_description)
-            named_entities = extract_named_entities(node.entity_description)
-            sentiment = extract_sentiment_vader(node.entity_description)
+            # pos_tags = extract_pos_tags(node.description)
+            # named_entities = extract_named_entities(node.description)
+            # sentiment = extract_sentiment_vader(node.description)
+
+            id, type, name, description, *node_properties = node
+
+            print("Node properties: ", node_properties)
+
+            node_properties = dict(node_properties)
 
             graph_nodes.append((
                 node_id,
                 dict(
                     id = node_id,
                     layer_id = layer_id,
                     chunk_id = chunk_id,
                     chunk_collection = chunk_collection,
-                    name = node.entity_name,
-                    entity_type = node.entity_type.lower().capitalize(),
-                    description = node.entity_description,
-                    pos_tags = pos_tags,
-                    sentiment = sentiment,
-                    named_entities = named_entities,
+                    name = node.name,
+                    type = node.type.lower().capitalize(),
+                    description = node.description,
+                    # pos_tags = pos_tags,
+                    # sentiment = sentiment,
+                    # named_entities = named_entities,
                     created_at = datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
                     updated_at = datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
+                    **node_properties,
                 )
             ))
 
             # Add relationship between entity type and entity itself: "Jake is Person"
             graph_edges.append((
                 node_id,
-                entity_type_node_id,
+                type_node_id,
                 "is",
                 dict(relationship_name = "is"),
             ))
 
             graph_edges.append((
                 layer_id,
                 node_id,
                 "contains",
                 dict(relationship_name = "contains"),
             ))
 
         # Add relationship that came from graphs.
         for edge in layer_graph.edges:
             graph_edges.append((
-                generate_proposition_node_id(edge.source_node_id),
-                generate_proposition_node_id(edge.target_node_id),
+                generate_node_id(edge.source_node_id),
+                generate_node_id(edge.target_node_id),
                 edge.relationship_name,
                 dict(relationship_name = edge.relationship_name),
             ))
 
         await graph_client.add_nodes(graph_nodes)
 
         await graph_client.add_edges(graph_edges)
@@ -134,12 +143,9 @@
                 embed_field = "value"
             ) for (node_id, node_data) in graph_nodes
         ]
 
         await vector_client.create_data_points(layer_id, data_points)
 
 
-def generate_proposition_node_id(node_id: str) -> str:
-    return f"PROPOSITION_NODE__{node_id.upper().replace(' ', '_')}".replace("'", "")
-
-def generate_type_node_id(node_id: str) -> str:
-    return f"PROPOSITION_TYPE_NODE__{node_id.upper().replace(' ', '_')}".replace("'", "")
+def generate_node_id(node_id: str) -> str:
+    return node_id.upper().replace(' ', '_').replace("'", "")
```

### Comparing `cognee-0.1.7/cognee/modules/cognify/graph/add_cognitive_layers.py` & `cognee-0.1.8/cognee/modules/cognify/graph/add_cognitive_layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,9 +25,11 @@
 
 def fix_layer_name(layer_name):
     sanitized_name = re.sub(r'[^a-zA-Z0-9_]', '', layer_name)
     return sanitized_name
 
 
 def generate_cognitive_layer_id(layer_id: str) -> str:
+
     layer = f"COGNITIVE_LAYER__{layer_id.upper().replace(' ', '_')}".replace("'", "").replace("/", "_")
     return fix_layer_name(layer)
+
```

### Comparing `cognee-0.1.7/cognee/modules/cognify/graph/add_data_chunks.py` & `cognee-0.1.8/cognee/modules/cognify/graph/add_data_chunks.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+
 from typing import TypedDict
 from pydantic import BaseModel, Field
-from cognee.infrastructure import infrastructure_config
+from cognee.infrastructure.databases.vector.config import get_vectordb_config
+
 from cognee.infrastructure.databases.vector import DataPoint
 
+config = get_vectordb_config()
+
 class TextChunk(TypedDict):
     text: str
     chunk_id: str
     file_metadata: dict
 
 async def add_data_chunks(dataset_data_chunks: dict[str, list[TextChunk]]):
-    vector_client = infrastructure_config.get_config("vector_engine")
+    vector_client = config.vector_engine
 
     identified_chunks = []
 
     class PayloadSchema(BaseModel):
         text: str = Field(...)
 
     for (dataset_name, chunks) in dataset_data_chunks.items():
@@ -26,24 +30,66 @@
 
         dataset_chunks = [
             dict(
                 chunk_id = chunk["chunk_id"],
                 collection = dataset_name,
                 text = chunk["text"],
                 document_id = chunk["document_id"],
+                file_metadata = chunk["file_metadata"],
             ) for chunk in chunks
         ]
 
         identified_chunks.extend(dataset_chunks)
 
         await vector_client.create_data_points(
             dataset_name,
             [
                 DataPoint[PayloadSchema](
                     id = chunk["chunk_id"],
                     payload = PayloadSchema.parse_obj(dict(text = chunk["text"])),
                     embed_field = "text",
                 ) for chunk in dataset_chunks
             ],
+        )
+
+    return identified_chunks
+
+
+async def add_data_chunks_basic_rag(dataset_data_chunks: dict[str, list[TextChunk]]):
+    vector_client = config.vector_engine
+
+    identified_chunks = []
+
+    class PayloadSchema(BaseModel):
+        text: str = Field(...)
+
+    for (dataset_name, chunks) in dataset_data_chunks.items():
+        try:
+
+            await vector_client.create_collection("basic_rag", payload_schema = PayloadSchema)
+        except Exception as error:
+            print(error)
+
+        dataset_chunks = [
+            dict(
+                chunk_id = chunk["chunk_id"],
+                collection = "basic_rag",
+                text = chunk["text"],
+                document_id = chunk["document_id"],
+                file_metadata = chunk["file_metadata"],
+            ) for chunk in chunks
+        ]
+
+        identified_chunks.extend(dataset_chunks)
+
+        await vector_client.create_data_points(
+            "basic_rag",
+            [
+                DataPoint[PayloadSchema](
+                    id = chunk["chunk_id"],
+                    payload = PayloadSchema.parse_obj(dict(text = chunk["text"])),
+                    embed_field = "text",
+                ) for chunk in dataset_chunks
+            ],
         )
 
     return identified_chunks
```

### Comparing `cognee-0.1.7/cognee/modules/cognify/graph/add_document_node.py` & `cognee-0.1.8/cognee/modules/cognify/graph/add_document_node.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from cognee.shared.data_models import Document
-from cognee.modules.cognify.graph.add_label_nodes import add_label_nodes
+# from cognee.modules.cognify.graph.add_label_nodes import add_label_nodes
 from cognee.infrastructure.databases.graph.graph_db_interface import GraphDBInterface
 
 async def add_document_node(graph_client: GraphDBInterface, parent_node_id, document_metadata):
     document_id = f"DOCUMENT__{document_metadata['id']}"
 
     document = await graph_client.extract_node(document_id)
 
     if not document:
         document = Document(
             id = document_id,
             title = document_metadata["name"],
             file_path = document_metadata["file_path"],
         ).model_dump()
 
-    document["entity_type"] = "Document"
+    document["type"] = "Document"
 
     await graph_client.add_node(document_id, document)
+    print(f"Added document node: {document_id}")
 
     await graph_client.add_edge(
         parent_node_id,
         document_id,
         "has_document",
         dict(relationship_name = "has_document"),
     )
 
-    await add_label_nodes(graph_client, document_id, document_metadata["keywords"].split("|"))
+    #
+    # await add_label_nodes(graph_client, document_id, document_metadata["keywords"].split("|"))
 
     return document_id
```

### Comparing `cognee-0.1.7/cognee/modules/cognify/graph/add_label_nodes.py` & `cognee-0.1.8/cognee/modules/cognify/graph/add_label_nodes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from uuid import uuid4
 from typing import List
 from datetime import datetime
 from pydantic import BaseModel
-from cognee.infrastructure import infrastructure_config
-from cognee.infrastructure.databases.vector import DataPoint
 
+from cognee.infrastructure.databases.vector import DataPoint
+from cognee.infrastructure.databases.graph.config import get_graph_config
+from cognee.infrastructure.databases.vector.config import get_vectordb_config
+graph_config = get_graph_config()
+vectordb_config = get_vectordb_config()
 async def add_label_nodes(graph_client, parent_node_id: str, keywords: List[str]) -> None:
-    vector_client = infrastructure_config.get_config("vector_engine")
+    vector_client = vectordb_config.vector_engine
 
     keyword_nodes = []
 
     for keyword in keywords:
         keyword_id = f"DATA_LABEL_{keyword.upper().replace(' ', '_')}"
 
         keyword_nodes.append((
@@ -57,12 +60,12 @@
             ),
             embed_field = "value"
         ) for (keyword_node_id, keyword_data) in keyword_nodes
     ]
 
     try:
         await vector_client.create_collection(parent_node_id, payload_schema = PayloadSchema)
-    except Exception:
+    except Exception as e:
         # It's ok if the collection already exists.
-        pass
+        print(e)
 
-    await vector_client.create_data_points(parent_node_id, keyword_data_points)
+    await vector_client.create_data_points(parent_node_id, keyword_data_points)
```

### Comparing `cognee-0.1.7/cognee/modules/cognify/graph/add_node_connections.py` & `cognee-0.1.8/cognee/modules/cognify/graph/add_node_connections.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import uuid
 
-from cognee.infrastructure import infrastructure_config
+# from cognee.infrastructure import infrastructure_config
 from cognee.infrastructure.databases.graph.get_graph_client import get_graph_client
 from cognee.shared.data_models import GraphDBType
-
+from cognee.infrastructure.databases.graph.config import get_graph_config
+from cognee.infrastructure.databases.vector.config import get_vectordb_config
+graph_config = get_graph_config()
+vectordb_config = get_vectordb_config()
 
 
 async def group_nodes_by_layer(node_descriptions):
     """ Group nodes by layer decomposition uuid """
     grouped_data = {}
 
     for item in node_descriptions:
@@ -37,28 +40,28 @@
 
     for _, relationships in relationship_dict.items():
         for relationship in relationships:
 
             if relationship['score'] > score_threshold:
 
                 # For NetworkX
-                if infrastructure_config.get_config()["graph_engine"] == GraphDBType.NETWORKX:
+                if graph_config.graph_engine == GraphDBType.NETWORKX:
                     searched_node_id_found = await get_node_by_unique_id(graph.graph, relationship['searched_node_id'])
                     original_id_for_search_found = await get_node_by_unique_id(graph.graph, relationship['original_id_for_search'])
                     if searched_node_id_found and original_id_for_search_found:
                         await graph.add_edge(
                             searched_node_id_found,
                             original_id_for_search_found,
                             weight=relationship['score'],
                             score_metadata=relationship.get('score_metadata', {}),
                             id = f""" SEMANTIC_CONNECTION_{searched_node_id_found}_{original_id_for_search_found}_{str(uuid.uuid4())}"""
                         )
 
                 # For Neo4j
-                elif infrastructure_config.get_config()["graph_engine"] == GraphDBType.NEO4J:
+                elif graph_config.graph_engine == GraphDBType.NEO4J:
                     # Neo4j specific logic to add an edge
                     # This is just a placeholder, replace it with actual Neo4j logic
                     print("query is ", f"""MATCH (a), (b) WHERE a.unique_id = '{relationship['searched_node_id']}' AND b.unique_id = '{relationship['original_id_for_search']}' CREATE (a)-[:CONNECTED {{weight:{relationship['score']}}}]->(b)""")
                     result = await graph.query(f"""MATCH (a), (b) WHERE a.unique_id = '{relationship['searched_node_id']}' AND b.unique_id = '{relationship['original_id_for_search']}'
                               CREATE (a)-[:SEMANTIC_CONNECTION {{weight:{relationship['score']}}}]->(b)""")
                     await graph.close()
```

### Comparing `cognee-0.1.7/cognee/modules/cognify/graph/add_summary_nodes.py` & `cognee-0.1.8/cognee/modules/cognify/graph/add_summary_nodes.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 async def add_summary_nodes(graph_client, document_id, summary):
     summary_node_id = f"DATA_SUMMARY__{document_id}"
 
     await graph_client.add_node(
         summary_node_id,
         dict(
             name = "Summary",
+            document_id = document_id,
             summary = summary["summary"],
         ),
     )
 
     await graph_client.add_edge(document_id, summary_node_id, relationship_name = "summarized_as")
 
 
     description_node_id = f"DATA_DESCRIPTION__{document_id}"
 
     await graph_client.add_node(
         description_node_id,
         dict(
             name = "Description",
-            summary = summary["description"],
+            document_id= document_id,
+            description = summary["description"],
         ),
     )
 
     await graph_client.add_edge(document_id, description_node_id, relationship_name = "described_as")
```

### Comparing `cognee-0.1.7/cognee/modules/cognify/graph/create.py` & `cognee-0.1.8/cognee/modules/cognify/graph/create.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """ This module is responsible for creating a semantic graph """
 from typing import  Optional, Any
 from pydantic import BaseModel
 
-from cognee.infrastructure import infrastructure_config
+# from cognee.infrastructure import infrastructure_config
 from cognee.shared.data_models import GraphDBType
 
-
+from cognee.infrastructure.databases.graph.config import get_graph_config
+from cognee.infrastructure.databases.vector.config import get_vectordb_config
+graph_config = get_graph_config()
+vectordb_config = get_vectordb_config()
 async def generate_node_id(instance: BaseModel) -> str:
     for field in ["id", "doc_id", "location_id", "type_id", "node_id"]:
         if hasattr(instance, field):
             return f"{instance.__class__.__name__}:{getattr(instance, field)}"
     return f"{instance.__class__.__name__}_default"
 
 
@@ -26,29 +29,38 @@
     Returns:
     - The result of the node addition operation if successful, otherwise None. This could be the newly added node object, a confirmation message, or any relevant data returned by the database client.
 
     Raises:
     - Exception: If there is an error during the node or edge addition process, it logs the error and continues without interrupting the execution flow.
 
     Note:
-    - The function currently supports adding edges only if the graph database engine is NETWORKX, as specified in the global `infrastructure_config`.
+    - The function currently supports adding edges only if the graph database engine is NETWORKX, as specified in the graph configuration.
     """
 
     # Initialize result to None to ensure a clear return path
     result = None
 
     # Proceed only if the node_id is not meant for default relationships
     if node_id != "Relationship_default":
         try:
             # Attempt to add the node to the graph database
+            # print('NODE ID', node_id)
+            # print('NODE DATA', node_data)
             result = await client.add_node(node_id, node_properties = node_data)
+            print("added node", result)
 
             # Add an edge if a parent ID is provided and the graph engine is NETWORKX
-            if parent_id and "default_relationship" in node_data and infrastructure_config.get_config()["graph_engine"] == GraphDBType.NETWORKX:
-                await client.add_edge(parent_id, node_id, relationship_name = node_data["default_relationship"]["type"], edge_properties = node_data)
+            if parent_id and "default_relationship" in node_data and graph_config.graph_engine == GraphDBType.NETWORKX:
+
+                try:
+                    await client.add_edge(parent_id, node_id, relationship_name = node_data["default_relationship"]["type"], edge_properties = node_data)
+                    print("added edge")
+                except Exception as e:
+                    print(f"Error adding edge: {e}")
+                    pass
         except Exception as e:
             # Log the exception; consider a logging framework for production use
             print(f"Error adding node or edge: {e}")
             # Depending on requirements, you may want to handle the exception differently
 
     return result
 
@@ -99,14 +111,15 @@
 #
 #             # Add an edge between the source and target nodes using the client
 #             await client.add_edge(source, target, relationship_name=relationship_details['type'])
 
 
 
 async def add_edge(client, parent_id: Optional[str], node_id: str, node_data: dict, created_node_ids):
+    print('NODE ID', node_data)
 
     if node_id == "Relationship_default" and parent_id:
         # Initialize source and target variables outside the loop
         source, target = None, None
 
         # Assuming 'source' and 'target' are keys in node_data
         source_key = node_data.get('source', '').lower()
@@ -133,47 +146,75 @@
             # If you need to do something with relationship_details (e.g., add an edge), do it here
             # For demonstration, we'll just print the results
             print("RELATIONSHIP DETAILS", relationship_details)
 
             await client.add_edge(relationship_details['source'], relationship_details['target'], relationship_name = relationship_details['type'])
 
 
-
-
 async def process_attribute(graph_client, parent_id: Optional[str], attribute: str, value: Any, created_node_ids=None):
-
     if created_node_ids is None:
         created_node_ids = []
+
     if isinstance(value, BaseModel):
         node_id = await generate_node_id(value)
         node_data = value.model_dump()
 
-        # Use the specified default relationship for the edge between the parent node and the current node
-
+        # Add node to the graph
         created_node_id = await add_node(graph_client, parent_id, node_id, node_data)
+        created_node_ids.append(node_id)
 
-        created_node_ids.append(created_node_id)
-
-        # await add_edge(graph_client, parent_id, node_id, node_data, relationship_data,created_node_ids)
+        # Add an edge if a default_relationship exists
+        if hasattr(value, 'default_relationship') and value.default_relationship:
+            await add_edge(graph_client, parent_id, node_id, value.default_relationship.dict())
 
         # Recursively process nested attributes to ensure all nodes and relationships are added to the graph
-        for sub_attr, sub_val in value.__dict__.items():  # Access attributes and their values directly
-
-            out = await process_attribute(graph_client, node_id, sub_attr, sub_val)
-
-            created_node_ids.extend(out)
+        for sub_attr, sub_val in value.dict().items():
+            if isinstance(sub_val, (BaseModel, list)):  # Check if the value is a model or list
+                await process_attribute(graph_client, node_id, sub_attr, sub_val, created_node_ids)
 
     elif isinstance(value, list) and all(isinstance(item, BaseModel) for item in value):
         # For lists of BaseModel instances, process each item in the list
         for item in value:
-            out = await process_attribute(graph_client, parent_id, attribute, item, created_node_ids)
-            created_node_ids.extend(out)
+            await process_attribute(graph_client, parent_id, attribute, item, created_node_ids)
 
     return created_node_ids
 
+# async def process_attribute(graph_client, parent_id: Optional[str], attribute: str, value: Any, created_node_ids=None):
+#
+#     if created_node_ids is None:
+#         created_node_ids = []
+#     if isinstance(value, BaseModel):
+#         node_id = await generate_node_id(value)
+#         node_data = value.model_dump()
+#
+#         # Use the specified default relationship for the edge between the parent node and the current node
+#
+#         created_node_id = await add_node(graph_client, parent_id, node_id, node_data)
+#
+#         created_node_ids.append(created_node_id)
+#
+#         # await add_edge(graph_client, parent_id, node_id, node_data, relationship_data,created_node_ids)
+#
+#         # Recursively process nested attributes to ensure all nodes and relationships are added to the graph
+#         # for sub_attr, sub_val in value.__dict__.items(): # Access attributes and their values directly
+#         #     print('SUB ATTR', sub_attr)
+#         #     print('SUB VAL', sub_val)
+#         #
+#         #     out = await process_attribute(graph_client, node_id, sub_attr, sub_val)
+#         #
+#         #     created_node_ids.extend(out)
+#
+#     elif isinstance(value, list) and all(isinstance(item, BaseModel) for item in value):
+#         # For lists of BaseModel instances, process each item in the list
+#         for item in value:
+#             out = await process_attribute(graph_client, parent_id, attribute, item, created_node_ids)
+#             created_node_ids.extend(out)
+#
+#     return created_node_ids
+
 
 async def process_attribute_edge(graph_client, parent_id: Optional[str], attribute: str, value: Any, created_node_ids=None):
 
     if isinstance(value, BaseModel):
         node_id = await generate_node_id(value)
 
 
@@ -206,27 +247,29 @@
 
     created_node_ids = []
 
     out = await graph_client.add_node(root_id, node_properties = node_data)
 
     created_node_ids.append(out)
 
-    for attribute_name, attribute_value in graph_model:
-        ids = await process_attribute(graph_client, root_id, attribute_name, attribute_value)
-        created_node_ids.extend(ids)
-
-    flattened_and_deduplicated = list({
-        item["nodeId"]: item
-            # Use the 'nodeId' as the unique key in the dictionary comprehension
-            for sublist in created_node_ids if sublist  # Ensure sublist is not None
-            for item in sublist  # Iterate over items in the sublist
-    }.values())
+    print('CREATED NODE IDS', created_node_ids)
 
     for attribute_name, attribute_value in graph_model:
-        ids = await process_attribute_edge(graph_client, root_id, attribute_name, attribute_value, flattened_and_deduplicated)
-
+        ids = await process_attribute(graph_client, root_id, attribute_name, attribute_value)
+    #     created_node_ids.extend(ids)
+    #
+    # flattened_and_deduplicated = list({
+    #     item["nodeId"]: item
+    #         # Use the 'nodeId' as the unique key in the dictionary comprehension
+    #         for sublist in created_node_ids if sublist  # Ensure sublist is not None
+    #         for item in sublist  # Iterate over items in the sublist
+    # }.values())
+    #
+    # for attribute_name, attribute_value in graph_model:
+    #     ids = await process_attribute_edge(graph_client, root_id, attribute_name, attribute_value, flattened_and_deduplicated)
+    #
     return graph_client
 
 
 async def create_semantic_graph(graph_model_instance, graph_client):
     # Dynamic graph creation based on the provided graph model instance
     return await create_dynamic(graph_model_instance, graph_client)
```

### Comparing `cognee-0.1.7/cognee/modules/cognify/llm/resolve_cross_graph_references.py` & `cognee-0.1.8/cognee/modules/cognify/llm/resolve_cross_graph_references.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from typing import Dict, List
-from cognee.infrastructure import infrastructure_config
+from cognee.infrastructure.databases.graph.config import get_graph_config
+from cognee.infrastructure.databases.vector.config import get_vectordb_config
+graph_config = get_graph_config()
+vectordb_config = get_vectordb_config()
 
 async def resolve_cross_graph_references(nodes_by_layer: Dict):
     results = []
 
     unique_layers = nodes_by_layer.keys()
 
     for layer_id, layer_nodes in nodes_by_layer.items():
@@ -12,15 +15,15 @@
 
         for other_layer in other_layers:
             results.append(await get_nodes_by_layer(other_layer, layer_nodes))
 
     return results
 
 async def get_nodes_by_layer(layer_id: str, layer_nodes: List):
-    vector_engine = infrastructure_config.get_config()["vector_engine"]
+    vector_engine = vectordb_config.vector_engine
 
     score_points = await vector_engine.batch_search(
         layer_id,
         [layer_node["description"] for layer_node in layer_nodes],
         limit = 2
     )
```

### Comparing `cognee-0.1.7/cognee/modules/cognify/test.py` & `cognee-0.1.8/cognee/modules/cognify/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from cognee.root_dir import get_absolute_path
 from cognee.config import Config
 
 config = Config()
 config.load()
 
 def run():
-    gpt4 = dspy.OpenAI(model = config.openai_model, api_key = config.openai_key, model_type = "chat", max_tokens = 4096)
+    gpt4 = dspy.OpenAI(model = config.llm_model, api_key = config.llm_api_key, model_type = "chat", max_tokens = 4096)
     compiled_extract_knowledge_graph = ExtractKnowledgeGraph(lm = gpt4)
     compiled_extract_knowledge_graph.load(get_absolute_path("./programs/extract_knowledge_graph/extract_knowledge_graph.json"))
 
     text = """The 1985 FA Charity Shield (also known as the General Motors FA
               Charity Shield for sponsorship reasons) was the 63rd FA Charity Shield,
               an annual football match played between the winners of the previous
               season's First Division and FA Cup competitions. The match was played on
```

### Comparing `cognee-0.1.7/cognee/modules/cognify/train.py` & `cognee-0.1.8/cognee/modules/cognify/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             context = "\r\n".join("".join(sentences) for sentences in example.context["sentences"]),
             answer = example.answer,
         ) for example in dataset.train
     ]
 
     trainset = [example.with_inputs("context", "question") for example in train_examples]
 
-    gpt4 = dspy.OpenAI(model = config.openai_model, api_key = config.openai_key, model_type = "chat", max_tokens = 4096)
+    gpt4 = dspy.OpenAI(model = config.llm_model, api_key = config.llm_api_key, model_type = "chat", max_tokens = 4096)
 
     compiled_extract_knowledge_graph = optimizer.compile(ExtractKnowledgeGraph(lm = gpt4), trainset = trainset)
 
     # Save program
     LocalStorage.ensure_directory_exists(get_absolute_path("./programs/extract_knowledge_graph"))
     compiled_extract_knowledge_graph.save(get_absolute_path("./programs/extract_knowledge_graph/extract_knowledge_graph.json"))
```

### Comparing `cognee-0.1.7/cognee/modules/data/extraction/extract_categories.py` & `cognee-0.1.8/cognee/modules/data/extraction/extract_categories.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/modules/data/extraction/knowledge_graph/extract_content_graph.py` & `cognee-0.1.8/cognee/modules/data/extraction/knowledge_graph/extract_content_graph.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph.py` & `cognee-0.1.8/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,8 +17,8 @@
             return compiled_extract_knowledge_graph(context = text, question = "")
 
         return (await event_loop.run_in_executor(None, sync_extract_knowledge_graph)).graph
         # return compiled_extract_knowledge_graph(text, question = "").graph
     except Exception as error:
         # TODO: Log error to Sentry
 
-        return await extract_content_graph(text, cognitive_layer, graph_model)
+        return await extract_content_graph(text, cognitive_layer, graph_model)
```

### Comparing `cognee-0.1.7/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph_module.py` & `cognee-0.1.8/cognee/modules/data/extraction/knowledge_graph/extract_knowledge_graph_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,42 +25,42 @@
     Extract information from the text and build a detailed knowledge graph."""
 
     text: str = dspy.InputField()
     graph: KnowledgeGraph = dspy.OutputField()
 
 
 def are_all_nodes_and_edges_valid(graph: KnowledgeGraph) -> bool:
-    return all([getattr(node, "entity_type", "").strip() != "" for node in graph.nodes]) and \
-        all([getattr(node, "entity_name", "").strip() != "" for node in graph.nodes]) and \
+    return all([getattr(node, "type", "").strip() != "" for node in graph.nodes]) and \
+        all([getattr(node, "name", "").strip() != "" for node in graph.nodes]) and \
         all([getattr(edge, "relationship_name", "").strip() != "" for edge in graph.edges])
 
 def is_node_connected(node: Node, edges: List[Edge]) -> bool:
     return any([(edge.source_node_id == node.id or edge.target_node_id == node.id) for edge in edges])
 
 def are_all_nodes_connected(graph: KnowledgeGraph) -> bool:
     return all([is_node_connected(node, graph.edges) for node in graph.nodes])
 
 
 class ExtractKnowledgeGraph(dspy.Module):
-    def __init__(self, lm = dspy.OpenAI(model = config.openai_model, api_key = config.openai_key, model_type = "chat", max_tokens = 4096)):
+    def __init__(self, lm = dspy.OpenAI(model = config.llm_model, api_key = config.llm_api_key, model_type = "chat", max_tokens = 4096)):
         super().__init__()
         self.lm = lm
         dspy.settings.configure(lm=self.lm)
         self.generate_graph = dspy.TypedChainOfThought(GraphFromText)
         nltk.download("stopwords", quiet = True)
 
     def forward(self, context: str, question: str):
         context = remove_stop_words(context)
-        context = trim_text_to_max_tokens(context, 1500, config.openai_model)
+        context = trim_text_to_max_tokens(context, 1500, config.llm_model)
       
         with dspy.context(lm = self.lm):
             graph = self.generate_graph(text = context).graph
 
             not_valid_nodes_or_edges_message = """
-                All nodes must contain "entity_name".
+                All nodes must contain "name".
                 All edges must contain "relationship_name".
                 Please add mandatory fields to nodes and edges."""
 
             dspy.Suggest(are_all_nodes_and_edges_valid(graph), not_valid_nodes_or_edges_message)
 
             # not_connected_graph_message = """
             #     Output must be a graph that has all nodes connected to it.
@@ -75,15 +75,15 @@
     stop_words = set(stopwords.words("english"))
     word_tokens = word_tokenize(text)
     filtered_text = [word for word in word_tokens if word.lower() not in stop_words]
     return " ".join(filtered_text)
 
 #
 # if __name__ == "__main__":
-#     gpt_4_turbo = dspy.OpenAI(model="gpt-4", max_tokens=4000, api_key=config.openai_key, model_type="chat")
+#     gpt_4_turbo = dspy.OpenAI(model="gpt-4", max_tokens=4000, api_key=config.llm_api_key, model_type="chat")
 #     dspy.settings.configure(lm=gpt_4_turbo)
 
 
 #     extract_knowledge_graph = ExtractKnowledgeGraph(lm=gpt_4_turbo)
 #     # graph_text = extract_knowledge_graph("cognitive_layer", "text")
 #     graph = extract_knowledge_graph("analysis_layer", """A large language model (LLM) is a language model notable for its ability to achieve general-purpose language generation and other natural language processing tasks such as classification. LLMs acquire these abilities by learning statistical relationships from text documents during a computationally intensive self-supervised and semi-supervised training process. LLMs can be used for text generation, a form of generative AI, by taking an input text and repeatedly predicting the next token or word.
 # LLMs are artificial neural networks. The largest and most capable, as of March 2024""", question="What is a large language model?")
```

### Comparing `cognee-0.1.7/cognee/modules/data/get_layer_graphs.py` & `cognee-0.1.8/cognee/modules/data/get_layer_graphs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import logging
 import asyncio
 from cognee.infrastructure import infrastructure_config
 from .extraction.knowledge_graph.extract_knowledge_graph import extract_knowledge_graph
-
+from.extraction.extract_summary import extract_summary
+from cognee.modules.cognify.config import get_cognify_config
+config = get_cognify_config()
 logger = logging.getLogger(__name__)
 
 async def get_layer_graphs(content: str, cognitive_layers: list[tuple[str, dict]]):
     try:
         graph_awaitables = [
             extract_knowledge_graph(
                 content,
                 cognitive_layer_data["name"],
-                infrastructure_config.get_config()["graph_model"]
+                config.graph_model
             ) for (_, cognitive_layer_data) in cognitive_layers
         ]
 
         graphs = await asyncio.gather(*graph_awaitables)
 
         return [(layer_id, graphs[layer_index]) for (layer_index, (layer_id, __)) in enumerate(cognitive_layers)]
     except Exception as error:
```

### Comparing `cognee-0.1.7/cognee/modules/discovery/discover_directory_datasets.py` & `cognee-0.1.8/cognee/modules/discovery/discover_directory_datasets.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/modules/ingestion/add_data_to_dataset.py` & `cognee-0.1.8/cognee/modules/ingestion/add_data_to_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import logging
 from cognee.infrastructure import infrastructure_config
 from cognee.infrastructure.data import Dataset, Data
 from cognee.infrastructure.files import remove_file_from_storage
 from cognee.infrastructure.databases.relational import DatabaseEngine
+from cognee.infrastructure.databases.relational.config import get_relationaldb_config
+config = get_relationaldb_config()
 
 logger = logging.getLogger(__name__)
 
 async def add_data_to_dataset(dataset: Dataset, data: Data):
-    db_engine: DatabaseEngine = infrastructure_config.get_config()["database_engine"]
+    db_engine: DatabaseEngine = config.database_engine
 
     existing_dataset = (await db_engine.query_entity(dataset)).scalar()
     existing_data = (await db_engine.query_entity(data)).scalar()
 
     if existing_dataset:
         if existing_data:
             await remove_old_raw_data(existing_data.raw_data_location)
```

### Comparing `cognee-0.1.7/cognee/modules/ingestion/data_types/BinaryData.py` & `cognee-0.1.8/cognee/modules/ingestion/data_types/BinaryData.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 from cognee.infrastructure.files import get_file_metadata, FileMetadata
 from .IngestionData import IngestionData
 
 def create_binary_data(data: BinaryIO):
     return BinaryData(data)
 
 class BinaryData(IngestionData):
+    name: str = None
     data: BinaryIO = None
     metadata: FileMetadata = None
 
-    def __init__(self, data: BinaryIO):
+    def __init__(self, data: BinaryIO, name: str = None):
+        self.name = name
         self.data = data
 
     def get_identifier(self):
         metadata = self.get_metadata()
 
         return metadata["mime_type"] + "_" + "|".join(metadata["keywords"])
 
@@ -22,9 +24,12 @@
 
         return self.metadata
 
     def ensure_metadata(self):
         if self.metadata is None:
             self.metadata = get_file_metadata(self.data)
 
+            if self.metadata["name"] is None:
+                self.metadata["name"] = self.name
+
     def get_data(self):
         return self.data
```

### Comparing `cognee-0.1.7/cognee/modules/ingestion/data_types/TextData.py` & `cognee-0.1.8/cognee/modules/ingestion/data_types/TextData.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/modules/ingestion/save.py` & `cognee-0.1.8/cognee/modules/ingestion/save.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/modules/search/CogneeSearch.py` & `cognee-0.1.8/cognee/modules/search/CogneeSearch.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/modules/search/graph/search_adjacent.py` & `cognee-0.1.8/cognee/modules/search/graph/search_adjacent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 """ This module contains the function to find the neighbours of a given node in the graph"""
 
 
 from typing import Union, Dict
 import networkx as nx
 from cognee.shared.data_models import GraphDBType
-async def search_adjacent(graph: Union[nx.Graph, any], query: str, infrastructure_config: Dict, other_param: dict = None) -> Dict[str, str]:
+from cognee.infrastructure.databases.graph.config import get_graph_config
+graph_config = get_graph_config()
+async def search_adjacent(graph: Union[nx.Graph, any], query: str, other_param: dict = None) -> Dict[str, str]:
     """
     Find the neighbours of a given node in the graph and return their descriptions.
     Supports both NetworkX graphs and Neo4j graph databases based on the configuration.
 
     Parameters:
     - graph (Union[nx.Graph, AsyncSession]): The graph object or Neo4j session.
     - query (str): Unused in this implementation but could be used for future enhancements.
-    - infrastructure_config (Dict): Configuration that includes the graph engine type.
     - other_param (dict, optional): A dictionary that may contain 'node_id' to specify the node.
 
     Returns:
     - Dict[str, str]: A dictionary containing the unique identifiers and descriptions of the neighbours of the given node.
     """
-    node_id = other_param.get('node_id') if other_param else None
+    node_id = other_param.get('node_id') if other_param else query
 
     if node_id is None:
         return {}
-
-    if infrastructure_config.get_config()["graph_engine"] == GraphDBType.NETWORKX:
+    from cognee.infrastructure import infrastructure_config
+    if graph_config.graph_engine == GraphDBType.NETWORKX:
         if node_id not in graph:
             return {}
 
         neighbors = list(graph.neighbors(node_id))
         neighbor_descriptions = {neighbor: graph.nodes[neighbor].get('description') for neighbor in neighbors}
         return neighbor_descriptions
 
-    elif infrastructure_config.get_config()["graph_engine"] == GraphDBType.NEO4J:
+    elif graph_config.graph_engine  == GraphDBType.NEO4J:
         cypher_query = """
         MATCH (node {id: $node_id})-[:CONNECTED_TO]->(neighbor)
         RETURN neighbor.id AS neighbor_id, neighbor.description AS description
         """
         results = await graph.run(cypher_query, node_id=node_id)
         neighbor_descriptions = {record["neighbor_id"]: record["description"] for record in await results.list() if "description" in record}
         return neighbor_descriptions
```

### Comparing `cognee-0.1.7/cognee/modules/search/graph/search_neighbour.py` & `cognee-0.1.8/cognee/modules/search/graph/search_neighbour.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 """ Fetches the context of a given node in the graph"""
 from typing import Union, Dict
 
+from neo4j import AsyncSession
+
 from cognee.infrastructure.databases.graph.get_graph_client import get_graph_client
 import networkx as nx
 from cognee.shared.data_models import GraphDBType
-
-async def search_neighbour(graph: Union[nx.Graph, any], id: str, infrastructure_config: Dict,
+from cognee.infrastructure.databases.graph.config import get_graph_config
+graph_config = get_graph_config()
+from cognee.infrastructure.databases.vector.config import get_vectordb_config
+vector_config = get_vectordb_config()
+async def search_neighbour(graph: Union[nx.Graph, any], query: str,
                            other_param: dict = None):
     """
     Search for nodes that share the same 'layer_uuid' as the specified node and return their descriptions.
     Adapts to both NetworkX graphs and Neo4j graph databases based on the configuration.
 
     Parameters:
     - graph (Union[nx.Graph, AsyncSession]): The graph object or Neo4j session.
     - id (str): The identifier of the node to match against.
     - infrastructure_config (Dict): Configuration that includes the graph engine type.
     - other_param (dict, optional): A dictionary that may contain 'node_id' to specify the node.
 
     Returns:
     - List[str]: A list of 'description' attributes of nodes that share the same 'layer_uuid' with the specified node.
     """
-    node_id = other_param.get('node_id') if other_param else None
+    from cognee.infrastructure import infrastructure_config
+    node_id = other_param.get('node_id') if other_param else query
 
     if node_id is None:
         return []
 
-    if infrastructure_config.get_config()["graph_engine"] == GraphDBType.NETWORKX:
-        if isinstance(graph, nx.Graph):
-            if node_id not in graph:
-                return []
-
-            relevant_context = []
-            target_layer_uuid = graph.nodes[node_id].get('layer_uuid')
-
-            for n, attr in graph.nodes(data=True):
-                if attr.get('layer_uuid') == target_layer_uuid and 'description' in attr:
-                    relevant_context.append(attr['description'])
-
-            return relevant_context
-        else:
-            raise ValueError("Graph object does not match the specified graph engine type in the configuration.")
+    if graph_config.graph_engine == GraphDBType.NETWORKX:
+        relevant_context = []
+        target_layer_uuid = graph.nodes[node_id].get('layer_uuid')
+
+        for n, attr in graph.nodes(data=True):
+            if attr.get('layer_uuid') == target_layer_uuid and 'description' in attr:
+                relevant_context.append(attr['description'])
+
+        return relevant_context
+
 
-    elif infrastructure_config.get_config()["graph_engine"] == GraphDBType.NEO4J:
+    elif graph_config.graph_engine  == GraphDBType.NEO4J:
         if isinstance(graph, AsyncSession):
             cypher_query = """
             MATCH (target {id: $node_id})
             WITH target.layer_uuid AS layer
             MATCH (n)
             WHERE n.layer_uuid = layer AND EXISTS(n.description)
             RETURN n.description AS description
```

### Comparing `cognee-0.1.7/cognee/modules/search/graph/search_summary.py` & `cognee-0.1.8/cognee/modules/search/graph/search_summary.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,61 @@
 
 
 
 from typing import Union, Dict
 import networkx as nx
-from cognee.shared.data_models import GraphDBType
+from cognee.infrastructure import infrastructure_config
 
-async def search_summary(graph: Union[nx.Graph, any], query: str, infrastructure_config: Dict, other_param: str = None) -> Dict[str, str]:
+from cognee.modules.search.llm.extraction.categorize_relevant_summary import categorize_relevant_summary
+from cognee.shared.data_models import GraphDBType, ResponseSummaryModel
+from cognee.infrastructure.databases.graph.config import get_graph_config
+graph_config = get_graph_config()
+from cognee.infrastructure.databases.vector.config import get_vectordb_config
+vector_config = get_vectordb_config()
+import re
+
+def strip_exact_regex(s, substring):
+    # Escaping substring to be used in a regex pattern
+    pattern = re.escape(substring)
+    # Regex to match the exact substring at the start and end
+    return re.sub(f"^{pattern}|{pattern}$", "", s)
+async def search_summary( query: str,  graph: Union[nx.Graph, any]) -> Dict[str, str]:
     """
     Filter nodes based on a condition (such as containing 'SUMMARY' in their identifiers) and return their summary attributes.
     Supports both NetworkX graphs and Neo4j graph databases based on the configuration.
 
     Parameters:
     - graph (Union[nx.Graph, AsyncSession]): The graph object or Neo4j session.
     - query (str): The query string to filter nodes by, e.g., 'SUMMARY'.
     - infrastructure_config (Dict): Configuration that includes the graph engine type.
     - other_param (str, optional): An additional parameter, unused in this implementation but could be for future enhancements.
 
     Returns:
     - Dict[str, str]: A dictionary where keys are node identifiers containing the query string, and values are their 'summary' attributes.
     """
-    if infrastructure_config.get_config()["graph_engine"] == GraphDBType.NETWORKX:
-        return {node: data.get('summary') for node, data in graph.nodes(data=True) if query in node and 'summary' in data}
 
-    elif infrastructure_config.get_config()["graph_engine"] == GraphDBType.NEO4J:
+    if graph_config.graph_engine == GraphDBType.NETWORKX:
+        print("graph", graph)
+        summaries_and_ids = [
+            {'document_id': strip_exact_regex(_, "DATA_SUMMARY__"), 'Summary': data['summary']}
+            for _, data in graph.nodes(data=True)
+            if 'summary' in data
+        ]
+        print("summaries_and_ids", summaries_and_ids)
+        check_relevant_summary = await categorize_relevant_summary(query, summaries_and_ids, response_model=ResponseSummaryModel)
+        print("check_relevant_summary", check_relevant_summary)
+
+        connected_nodes = list(graph.neighbors(check_relevant_summary['document_id']))
+        print("connected_nodes", connected_nodes)
+        descriptions = {node: graph.nodes[node].get('description', 'No desc available') for node in connected_nodes}
+        print("descs", descriptions)
+        return descriptions
+
+
+    elif graph_config.graph_engine == GraphDBType.NEO4J:
         cypher_query = f"""
         MATCH (n)
         WHERE n.id CONTAINS $query AND EXISTS(n.summary)
         RETURN n.id AS nodeId, n.summary AS summary
         """
         results = await graph.run(cypher_query, query=query)
         summary_data = {record["nodeId"]: record["summary"] for record in await results.list()}
```

### Comparing `cognee-0.1.7/cognee/modules/search/vector/search_similarity.py` & `cognee-0.1.8/cognee/modules/search/vector/search_similarity.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,62 @@
-from dsp.utils import deduplicate
-from cognee.infrastructure import infrastructure_config
 from cognee.infrastructure.databases.graph.get_graph_client import get_graph_client
-
+from cognee.infrastructure.databases.graph.config import get_graph_config
+graph_config = get_graph_config()
+from cognee.infrastructure.databases.vector.config import get_vectordb_config
+vector_config = get_vectordb_config()
 
 async def search_similarity(query: str, graph):
-    graph_db_type = infrastructure_config.get_config()["graph_engine"]
+    graph_db_type = graph_config.graph_engine
 
     graph_client = await get_graph_client(graph_db_type)
 
     layer_nodes = await graph_client.get_layer_nodes()
 
     unique_layer_uuids = set(node["layer_id"] for node in layer_nodes)
+    print("unique_layer_uuids", unique_layer_uuids)
+
 
     graph_nodes = []
 
     for layer_id in unique_layer_uuids:
-        vector_engine = infrastructure_config.get_config()["vector_engine"]
+        vector_engine = vector_config.vector_engine
 
         results = await vector_engine.search(layer_id, query_text = query, limit = 10)
+        print("results", results)
+        print("len_rs", len(results))
 
         if len(results) > 0:
             graph_nodes.extend([
                 dict(
                     layer_id = result.payload["references"]["cognitive_layer"],
                     node_id = result.payload["references"]["node_id"],
                     score = result.score,
-                ) for result in results if result.score > 0.8
+                ) for result in results if result.score > 0.3
             ])
 
     if len(graph_nodes) == 0:
         return []
 
-    relevant_context = []
-
-    for graph_node_data in graph_nodes:
-        graph_node = await graph_client.extract_node(graph_node_data["node_id"])
 
-        if "chunk_collection" not in graph_node and "chunk_id" not in graph_node:
-            continue
+    return graph_nodes
 
-        vector_point = await vector_engine.retrieve(
-            graph_node["chunk_collection"],
-            graph_node["chunk_id"],
-        )
 
-        relevant_context.append(vector_point.payload["text"])
 
-    return deduplicate(relevant_context)
+    # for graph_node_data in graph_nodes:
+    #     if graph_node_data['score'] >0.8:
+    #         graph_node = await graph_client.extract_node(graph_node_data["node_id"])
+    #
+    #         if "chunk_collection" not in graph_node and "chunk_id" not in graph_node:
+    #             continue
+    #
+    #         vector_point = await vector_engine.retrieve(
+    #             graph_node["chunk_collection"],
+    #             graph_node["chunk_id"],
+    #         )
+    #
+    #         print("vector_point", vector_point.payload["text"])
+    #
+    #         relevant_context.append(vector_point.payload["text"])
+    #
+    # print(relevant_context)
+    #
+    # return deduplicate(relevant_context)
```

### Comparing `cognee-0.1.7/cognee/modules/users/memory/create_information_points.py` & `cognee-0.1.8/cognee/modules/users/memory/create_information_points.py`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/programs/extract_knowledge_graph/extract_knowledge_graph.json` & `cognee-0.1.8/cognee/programs/extract_knowledge_graph/extract_knowledge_graph.json`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/shared/data_models.py` & `cognee-0.1.8/cognee/shared/data_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from enum import Enum, auto
 from typing import Optional, List, Union, Dict, Any
 from pydantic import BaseModel, Field
 
 class Node(BaseModel):
     """Node in a knowledge graph."""
     id: str
-    entity_name: str
-    entity_type: str
-    entity_description: str
+    name: str
+    type: str
+    description: str
 
 class Edge(BaseModel):
     """Edge in a knowledge graph."""
     source_node_id: str
     target_node_id: str
     relationship_name: str
 
@@ -22,31 +22,29 @@
     nodes: List[Node] = Field(..., default_factory=list)
     edges: List[Edge] = Field(..., default_factory=list)
 
 class GraphQLQuery(BaseModel):
     """GraphQL query."""
     query: str
 
-
-
 class Answer(BaseModel):
     """Answer."""
     answer: str
 
 class ChunkStrategy(Enum):
     EXACT = "exact"
     PARAGRAPH = "paragraph"
     SENTENCE = "sentence"
+    CODE    = "code"
 
 class MemorySummary(BaseModel):
     """ Memory summary. """
     nodes: List[Node] = Field(..., default_factory=list)
     edges: List[Edge] = Field(..., default_factory=list)
 
-
 class TextSubclass(str, Enum):
     ARTICLES = "Articles, essays, and reports"
     BOOKS = "Books and manuscripts"
     NEWS_STORIES = "News stories and blog posts"
     RESEARCH_PAPERS = "Research papers and academic publications"
     SOCIAL_MEDIA = "Social media posts and comments"
     WEBSITE_CONTENT = "Website content and product descriptions"
@@ -103,15 +101,14 @@
     PHOTOGRAPHS = "Photographs and digital images"
     ILLUSTRATIONS = "Illustrations, diagrams, and charts"
     INFOGRAPHICS = "Infographics and visual data representations"
     ARTWORK = "Artwork and paintings"
     SCREENSHOTS = "Screenshots and graphical user interfaces"
     OTHER_IMAGES = "Other types of images"
 
-
 class VideoSubclass(str, Enum):
     MOVIES = "Movies and short films"
     DOCUMENTARIES = "Documentaries and educational videos"
     TUTORIALS = "Video tutorials and how-to guides"
     ANIMATED_FEATURES = "Animated features and cartoons"
     LIVE_EVENTS = "Live event recordings and sports broadcasts"
     OTHER_VIDEOS = "Other types of video content"
@@ -179,26 +176,24 @@
         ImageContent,
         VideoContent,
         MultimediaContent,
         Model3DContent,
         ProceduralContent,
     ]
 
-
 class SummarizedContent(BaseModel):
     """Class for a single class label summary and description."""
     summary: str
     description: str
 
 class LabeledContent(BaseModel):
     """Class for a single class label summary."""
     content_labels: str
 
 
-
 class CognitiveLayerSubgroup(BaseModel):
     """ CognitiveLayerSubgroup in a general layer """
     id: int
     name: str
     description: str
 
 
@@ -207,14 +202,15 @@
     category_name: str
     cognitive_layers: List[CognitiveLayerSubgroup] = Field(..., default_factory=list)
 
 
 class GraphDBType(Enum):
     NETWORKX = auto()
     NEO4J = auto()
+    FALKORDB = auto()
 
 
 # Models for representing different entities
 class Relationship(BaseModel):
     type: str
     source: Optional[str] = None
     target: Optional[str] = None
@@ -246,7 +242,21 @@
 
 class DefaultGraphModel(BaseModel):
     node_id: str
     user_properties: UserProperties = UserProperties()
     documents: List[Document] = []
     default_fields: Optional[Dict[str, Any]] = {}
     default_relationship: Relationship = Relationship(type = "has_properties")
+
+
+class ResponseSummaryModel(BaseModel):
+    """ Response summary model and existing document id """
+    document_id: str
+    response_summary: str
+
+
+class MonitoringTool(str, Enum):
+    """ Monitoring tools """
+    LANGFUSE = "langfuse"
+    LLMLITE = "llmlite"
+    LANGSMITH = "langsmith"
+
```

### Comparing `cognee-0.1.7/cognee/tests/test_data/Natural_language_processing.txt` & `cognee-0.1.8/cognee/.data/explanations/Natural language processing.txt`

 * *Files identical despite different names*

### Comparing `cognee-0.1.7/cognee/tests/test_library.py` & `cognee-0.1.8/cognee/tests/test_library.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,39 @@
+
+import logging
+import os
+
+logging.basicConfig(level=logging.DEBUG)
 async def  main():
     from os import path
     import pathlib
     import cognee
+    logging.basicConfig(level=logging.DEBUG)
+
+    # print("Working dir: ", str(pathlib.Path(__file__).parent))
+    # data_directory_path = str(pathlib.Path(path.join(pathlib.Path(__file__).parent, "../../.data")).resolve())
+    # print("Data dir: ", data_directory_path)
+    # cognee.config.data_root_directory(data_directory_path)
+    #
+    # cognee_directory_path = str(pathlib.Path(path.join(pathlib.Path(__file__).parent, "../../.cognee_system")).resolve())
+    # print("System dir: ", cognee_directory_path)
+    # cognee.config.system_root_directory(cognee_directory_path)
 
-    print("Working dir: ", str(pathlib.Path(__file__).parent))
-    data_directory_path = str(pathlib.Path(path.join(pathlib.Path(__file__).parent, "../../.data")).resolve())
-    print("Data dir: ", data_directory_path)
-    cognee.config.data_root_directory(data_directory_path)
-
-    cognee_directory_path = str(pathlib.Path(path.join(pathlib.Path(__file__).parent, "../../.cognee_system")).resolve())
-    print("System dir: ", cognee_directory_path)
-    cognee.config.system_root_directory(cognee_directory_path)
+    logging.debug("CURRENCT CWD: %s", pathlib.Path(__file__).parent)
+    logging.debug("CURRENCT CWD: %s", os.getcwd())
 
-    await cognee.prune.prune_system()
 
     dataset_name = "cs_explanations"
-    explanation_file_path = path.join(pathlib.Path(__file__).parent, "test_data/Natural_language_processing.txt")
+
+    explanation_file_path = os.path.join(pathlib.Path(__file__).parent, "test_data/Natural_language_processing.txt")
     await cognee.add([explanation_file_path], dataset_name)
     
-    dataset_name = "short_stories"
-    # data_directory_path is defined above
-    await cognee.add("data://" + data_directory_path, dataset_name)
+    # dataset_name = "short_stories"
+    # # data_directory_path is defined above
+    # await cognee.add("data://" + "/Users/runner/work/cognee/cognee/./cognee/tests", dataset_name)
 
     text_1 = """A quantum computer is a computer that takes advantage of quantum mechanical phenomena.
     At small scales, physical matter exhibits properties of both particles and waves, and quantum computing leverages this behavior, specifically quantum superposition and entanglement, using specialized hardware that supports the preparation and manipulation of quantum states.
     Classical physics cannot explain the operation of these quantum devices, and a scalable quantum computer could perform some calculations exponentially faster (with respect to input size scaling) than any modern "classical" computer. In particular, a large-scale quantum computer could break widely used encryption schemes and aid physicists in performing physical simulations; however, the current state of the technology is largely experimental and impractical, with several obstacles to useful applications. Moreover, scalable quantum computers do not hold promise for many practical tasks, and for many important tasks quantum speedups are proven impossible.
     The basic unit of information in quantum computing is the qubit, similar to the bit in traditional digital electronics. Unlike a classical bit, a qubit can exist in a superposition of its two "basis" states. When measuring a qubit, the result is a probabilistic output of a classical bit, therefore making quantum computers nondeterministic in general. If a quantum computer manipulates the qubit in a particular way, wave interference effects can amplify the desired measurement results. The design of quantum algorithms involves creating procedures that allow a quantum computer to perform calculations efficiently and quickly.
     Physically engineering high-quality qubits has proven challenging. If a physical qubit is not sufficiently isolated from its environment, it suffers from quantum decoherence, introducing noise into calculations. Paradoxically, perfectly isolating qubits is also undesirable because quantum computations typically need to initialize qubits, perform controlled qubit interactions, and measure the resulting quantum states. Each of those operations introduces errors and suffers from noise, and such inaccuracies accumulate.
     In principle, a non-quantum (classical) computer can solve the same computational problems as a quantum computer, given enough time. Quantum advantage comes in the form of time complexity rather than computability, and quantum complexity theory shows that some quantum algorithms for carefully selected tasks require exponentially fewer computational steps than the best known non-quantum algorithms. Such tasks can in theory be solved on a large-scale quantum computer whereas classical computers would not finish computations in any reasonable amount of time. However, quantum speedup is not universal or even typical across computational tasks, since basic tasks such as sorting are proven to not allow any asymptotic quantum speedup. Claims of quantum supremacy have drawn significant attention to the discipline, but are demonstrated on contrived tasks, while near-term practical use cases remain limited.
@@ -32,23 +41,23 @@
 
     text_2 = """A large language model (LLM) is a language model notable for its ability to achieve general-purpose language generation and other natural language processing tasks such as classification. LLMs acquire these abilities by learning statistical relationships from text documents during a computationally intensive self-supervised and semi-supervised training process. LLMs can be used for text generation, a form of generative AI, by taking an input text and repeatedly predicting the next token or word.
     LLMs are artificial neural networks. The largest and most capable, as of March 2024, are built with a decoder-only transformer-based architecture while some recent implementations are based on other architectures, such as recurrent neural network variants and Mamba (a state space model).
     Up to 2020, fine tuning was the only way a model could be adapted to be able to accomplish specific tasks. Larger sized models, such as GPT-3, however, can be prompt-engineered to achieve similar results.[6] They are thought to acquire knowledge about syntax, semantics and "ontology" inherent in human language corpora, but also inaccuracies and biases present in the corpora.
     Some notable LLMs are OpenAI's GPT series of models (e.g., GPT-3.5 and GPT-4, used in ChatGPT and Microsoft Copilot), Google's PaLM and Gemini (the latter of which is currently used in the chatbot of the same name), xAI's Grok, Meta's LLaMA family of open-source models, Anthropic's Claude models, Mistral AI's open source models, and Databricks' open source DBRX.
     """
 
+    #
+    # dataset_name = "cs_explanations"
+    # await cognee.add(
+    #     [
+    #         text_1,
+    #         text_2
+    #     ],
+    #     dataset_name
+    # )
 
-    dataset_name = "cs_explanations"
-    await cognee.add(
-        [
-            text_1,
-            text_2
-        ],
-        dataset_name
-    )
-
-    await cognee.cognify(["short_stories", "cs_explanations"])
+    await cognee.cognify([ "cs_explanations"])
 
 
 if __name__ == "__main__":
     import asyncio
     asyncio.run(main())
```

### Comparing `cognee-0.1.7/cognee/utils.py` & `cognee-0.1.8/cognee/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """ This module contains utility functions for the cognee. """
-
+import logging
 import os
 import uuid
 import datetime
 import graphistry
 import networkx as nx
 import numpy as np
 import pandas as pd
@@ -16,14 +16,16 @@
 
 config = Config()
 config.load()
 
 
 def send_telemetry(event_name: str):
     if os.getenv("TELEMETRY_DISABLED"):
+        print("Telemetry is disabled.")
+        logging.info("Telemetry is disabled.")
         return
 
     env = os.getenv("ENV")
     if env in ["local", "test", "dev"]:
         return
 
     posthog = Posthog(
@@ -208,14 +210,15 @@
             plotter = plotter.bind(point_label = "layer_description")
 
 
 
     # Visualization
     url = plotter.plot(render=False, as_files=True, memoize=False)
     print(f"Graph is visualized at: {url}")
+    return url
 
 
 def sanitize_df(df):
     """Replace NaNs and infinities in a DataFrame with None, making it JSON compliant."""
     return df.replace([np.inf, -np.inf, np.nan], None)
```

### Comparing `cognee-0.1.7/pyproject.toml` & `cognee-0.1.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognee"
-version = "0.1.7"
+version = "0.1.8"
 description = "Cognee - is a library for enriching LLM context with a semantic layer for better understanding and reasoning."
 authors = ["Vasilije Markovic", "Boris Arzentar"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://www.cognee.ai"
 repository = "https://github.com/topoteretes/cognee"
 classifiers = [
@@ -34,15 +34,15 @@
 pylint = "^3.0.3"
 aiosqlite = "^0.20.0"
 pandas = "^2.2.0"
 greenlet = "^3.0.3"
 ruff = "^0.2.2"
 filetype = "^1.2.0"
 nltk = "^3.8.1"
-dlt = "^0.4.7"
+dlt = "0.4.10"
 duckdb = {version = "^0.10.0", extras = ["dlt"]}
 overrides = "^7.7.0"
 aiofiles = "^23.2.1"
 qdrant-client = "^1.9.0"
 duckdb-engine = "^0.11.2"
 graphistry = "^0.33.5"
 tenacity = "^8.2.3"
@@ -56,15 +56,26 @@
 matplotlib = "^3.8.3"
 nest-asyncio = "^1.6.0"
 structlog = "^24.1.0"
 tiktoken = "^0.6.0"
 dspy-ai = "2.4.3"
 posthog = "^3.5.0"
 lancedb = "^0.6.10"
+importlib-metadata = "6.8.0"
+litellm = "^1.37.3"
+groq = "^0.5.0"
 tantivy = "^0.21.0"
+python-multipart = "^0.0.9"
+langfuse = "^2.32.0"
+spacy = "^3.7.4"
+protobuf = "<5.0.0"
+langchain-community = "0.0.38"
+deepeval = "^0.21.42"
+falkordb = "^1.0.4"
+pydantic-settings = "^2.2.1"
 
 
 [tool.poetry.extras]
 parquet = ["pyarrow"]
 duckdb = ["duckdb"]
 filesystem = ["s3fs", "botocore"]
 motherduck = ["duckdb", "pyarrow"]
```

### Comparing `cognee-0.1.7/PKG-INFO` & `cognee-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognee
-Version: 0.1.7
+Version: 0.1.8
 Summary: Cognee - is a library for enriching LLM context with a semantic layer for better understanding and reasoning.
 Home-page: https://www.cognee.ai
 License: Apache-2.0
 Author: Vasilije Markovic
 Requires-Python: >=3.9.0,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -27,44 +27,55 @@
 Provides-Extra: qdrant
 Provides-Extra: weaviate
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: aiosqlite (>=0.20.0,<0.21.0)
 Requires-Dist: anthropic (>=0.21.3,<0.22.0)
 Requires-Dist: boto3 (>=1.26.125,<2.0.0)
 Requires-Dist: debugpy (>=1.8.0,<2.0.0)
-Requires-Dist: dlt (>=0.4.7,<0.5.0)
+Requires-Dist: deepeval (>=0.21.42,<0.22.0)
+Requires-Dist: dlt (==0.4.10)
 Requires-Dist: dspy-ai (==2.4.3)
 Requires-Dist: duckdb-engine (>=0.11.2,<0.12.0)
 Requires-Dist: duckdb[dlt] (>=0.10.0,<0.11.0) ; extra == "duckdb" or extra == "motherduck"
+Requires-Dist: falkordb (>=1.0.4,<2.0.0)
 Requires-Dist: fastapi (>=0.109.2,<0.110.0)
 Requires-Dist: fastembed (>=0.2.5,<0.3.0)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: graphistry (>=0.33.5,<0.34.0)
 Requires-Dist: greenlet (>=3.0.3,<4.0.0)
+Requires-Dist: groq (>=0.5.0,<0.6.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
+Requires-Dist: importlib-metadata (==6.8.0)
 Requires-Dist: instructor (==1.2.1)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: lancedb (>=0.6.10,<0.7.0)
+Requires-Dist: langchain-community (==0.0.38)
+Requires-Dist: langfuse (>=2.32.0,<3.0.0)
+Requires-Dist: litellm (>=1.37.3,<2.0.0)
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: neo4j (>=5.18.0,<6.0.0) ; extra == "neo4j"
 Requires-Dist: nest-asyncio (>=1.6.0,<2.0.0)
 Requires-Dist: networkx (>=3.2.1,<4.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: openai (==1.14.3)
 Requires-Dist: overrides (>=7.7.0,<8.0.0) ; extra == "notebook"
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: posthog (>=3.5.0,<4.0.0)
+Requires-Dist: protobuf (<5.0.0)
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0) ; extra == "parquet" or extra == "motherduck"
 Requires-Dist: pydantic (>=2.5.0,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: pylint (>=3.0.3,<4.0.0)
 Requires-Dist: pypdf (>=4.1.0,<5.0.0)
 Requires-Dist: python-dotenv (==1.0.1)
+Requires-Dist: python-multipart (>=0.0.9,<0.0.10)
 Requires-Dist: qdrant-client (>=1.9.0,<2.0.0) ; extra == "qdrant"
 Requires-Dist: ruff (>=0.2.2,<0.3.0)
 Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0)
+Requires-Dist: spacy (>=3.7.4,<4.0.0)
 Requires-Dist: sqlalchemy (>=2.0.21,<3.0.0)
 Requires-Dist: structlog (>=24.1.0,<25.0.0)
 Requires-Dist: tantivy (>=0.21.0,<0.22.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: uvicorn (==0.22.0)
 Requires-Dist: weaviate-client (>=4.5.4,<5.0.0) ; extra == "weaviate"
@@ -100,59 +111,55 @@
   <a href="https://github.com/topoteretes/cognee/releases">
     <img src="https://img.shields.io/github/release/topoteretes/cognee?&label=Latest&style=for-the-badge" alt="cognee releases" />
   </a>
 </p>
 
 ![Cognee Demo](assets/cognee_demo.gif)
 
-Try it in a Google collab  <a href="https://colab.research.google.com/drive/11k0GtbrKRVGTxhcgad4Wl8YvCnWJVWPl?usp=sharing">notebook</a>  or have a look at our <a href="https://topoteretes.github.io/cognee">documentation</a>
 
-Join our  <a href="https://discord.gg/NQPKmU5CCg">Discord</a> community
+Try it in a Google collab  <a href="https://colab.research.google.com/drive/184Kpe9XGjrt8nVss0WDiPsPRrPk5lZ6o?usp=sharing">notebook</a>  or have a look at our <a href="https://topoteretes.github.io/cognee">documentation</a>
+
+If you have questions, join our  <a href="https://discord.gg/NQPKmU5CCg">Discord</a> community
 
 
 
 
 
 ## 📦 Installation
 
 ### With pip
 
 ```bash
 pip install cognee
 ```
 
-Use Weaviate vector storage:
-```bash
-pip install "cognee[weaviate]"
-```
 
 ### With poetry
 
 ```bash
 poetry add cognee
 ```
 
-Use Weaviate vector storage:
-```bash
-poetry add "cognee[weaviate]"
-```
 
 ## 💻 Usage
 
 ### Setup
 
 ```
 import os
 
-os.environ["WEAVIATE_URL"] = "YOUR_WEAVIATE_URL"
-os.environ["WEAVIATE_API_KEY"] = "YOUR_WEAVIATE_API_KEY"
-
-os.environ["OPENAI_API_KEY"] = "YOUR_OPENAI_API_KEY"
+os.environ["LLM_API_KEY"] = "YOUR OPENAI_API_KEY"
 
 ```
+or 
+```
+import cognee
+cognee.config.llm_api_key = "YOUR_OPENAI_API_KEY"
+```
+
 You can also use Ollama or Anyscale as your LLM provider. For more info on local models check our [docs](https://topoteretes.github.io/cognee)
 
 ### Run
 
 ```
 import cognee
 
@@ -188,14 +195,26 @@
 #
 # cognee.add("data://{absolute_path_to_root}", "reports.2024")
 # This will add just directory 2024 under reports.
 ```
 
 Read more [here](docs/index.md#run).
 
+## Vector retrieval, Graphs and LLMs
+
+Cognee supports a variety of tools and services for different operations:
+
+- **Local Setup**: By default, LanceDB runs locally with NetworkX and OpenAI.
+
+- **Vector Stores**: Cognee supports Qdrant and Weaviate for vector storage.
+
+- **Language Models (LLMs)**: You can use either Anyscale or Ollama as your LLM provider.
+
+- **Graph Stores**: In addition to LanceDB, Neo4j is also supported for graph storage.
+
 ## Demo
 
 Check out our demo notebook [here](https://github.com/topoteretes/cognee/blob/main/notebooks/cognee%20-%20Get%20Started.ipynb)
 
 
 
 [<img src="https://i3.ytimg.com/vi/-ARUfIzhzC4/maxresdefault.jpg" width="100%">](https://www.youtube.com/watch?v=BDFt4xVPmro "Learn about cognee: 55")
@@ -209,14 +228,12 @@
 
 
 
 
 ![Image](assets/architecture.png)
 
 
-## 🚀 It's alive
+## Star History
 
-<p>
-Try it yourself on Whatsapp with one of our <a href="https://keepi.ai" target="_blank">partners</a> by typing `/save {content you want to save}` followed by `/query {knowledge you saved previously}`
-For more info here are the <a href="https://topoteretes.github.io/cognee">docs</a>
-</p>
+
+[![Star History Chart](https://api.star-history.com/svg?repos=topoteretes/cognee&type=Date)](https://star-history.com/#topoteretes/cognee&Date)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognee Version: 0.1.7 Summary: Cognee - is a
+Metadata-Version: 2.1 Name: cognee Version: 0.1.8 Summary: Cognee - is a
 library for enriching LLM context with a semantic layer for better
 understanding and reasoning. Home-page: https://www.cognee.ai License: Apache-
 2.0 Author: Vasilije Markovic Requires-Python: >=3.9.0,<3.12 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows Classifier: Operating System :: POSIX :: Linux Classifier:
@@ -11,68 +11,76 @@
 Programming Language :: Python :: 3.11 Classifier: Topic :: Software
 Development :: Libraries Provides-Extra: cli Provides-Extra: duckdb Provides-
 Extra: filesystem Provides-Extra: motherduck Provides-Extra: neo4j Provides-
 Extra: notebook Provides-Extra: parquet Provides-Extra: qdrant Provides-Extra:
 weaviate Requires-Dist: aiofiles (>=23.2.1,<24.0.0) Requires-Dist: aiosqlite
 (>=0.20.0,<0.21.0) Requires-Dist: anthropic (>=0.21.3,<0.22.0) Requires-Dist:
 boto3 (>=1.26.125,<2.0.0) Requires-Dist: debugpy (>=1.8.0,<2.0.0) Requires-
-Dist: dlt (>=0.4.7,<0.5.0) Requires-Dist: dspy-ai (==2.4.3) Requires-Dist:
-duckdb-engine (>=0.11.2,<0.12.0) Requires-Dist: duckdb[dlt] (>=0.10.0,<0.11.0)
-; extra == "duckdb" or extra == "motherduck" Requires-Dist: fastapi
+Dist: deepeval (>=0.21.42,<0.22.0) Requires-Dist: dlt (==0.4.10) Requires-Dist:
+dspy-ai (==2.4.3) Requires-Dist: duckdb-engine (>=0.11.2,<0.12.0) Requires-
+Dist: duckdb[dlt] (>=0.10.0,<0.11.0) ; extra == "duckdb" or extra ==
+"motherduck" Requires-Dist: falkordb (>=1.0.4,<2.0.0) Requires-Dist: fastapi
 (>=0.109.2,<0.110.0) Requires-Dist: fastembed (>=0.2.5,<0.3.0) Requires-Dist:
 filetype (>=1.2.0,<2.0.0) Requires-Dist: graphistry (>=0.33.5,<0.34.0)
-Requires-Dist: greenlet (>=3.0.3,<4.0.0) Requires-Dist: gunicorn
-(>=20.1.0,<21.0.0) Requires-Dist: instructor (==1.2.1) Requires-Dist: jinja2
+Requires-Dist: greenlet (>=3.0.3,<4.0.0) Requires-Dist: groq (>=0.5.0,<0.6.0)
+Requires-Dist: gunicorn (>=20.1.0,<21.0.0) Requires-Dist: importlib-metadata
+(==6.8.0) Requires-Dist: instructor (==1.2.1) Requires-Dist: jinja2
 (>=3.1.3,<4.0.0) Requires-Dist: lancedb (>=0.6.10,<0.7.0) Requires-Dist:
-matplotlib (>=3.8.3,<4.0.0) Requires-Dist: neo4j (>=5.18.0,<6.0.0) ; extra ==
-"neo4j" Requires-Dist: nest-asyncio (>=1.6.0,<2.0.0) Requires-Dist: networkx
+langchain-community (==0.0.38) Requires-Dist: langfuse (>=2.32.0,<3.0.0)
+Requires-Dist: litellm (>=1.37.3,<2.0.0) Requires-Dist: matplotlib
+(>=3.8.3,<4.0.0) Requires-Dist: neo4j (>=5.18.0,<6.0.0) ; extra == "neo4j"
+Requires-Dist: nest-asyncio (>=1.6.0,<2.0.0) Requires-Dist: networkx
 (>=3.2.1,<4.0.0) Requires-Dist: nltk (>=3.8.1,<4.0.0) Requires-Dist: openai
 (==1.14.3) Requires-Dist: overrides (>=7.7.0,<8.0.0) ; extra == "notebook"
 Requires-Dist: pandas (>=2.2.0,<3.0.0) Requires-Dist: posthog (>=3.5.0,<4.0.0)
-Requires-Dist: pyarrow (>=15.0.0,<16.0.0) ; extra == "parquet" or extra ==
-"motherduck" Requires-Dist: pydantic (>=2.5.0,<3.0.0) Requires-Dist: pylint
-(>=3.0.3,<4.0.0) Requires-Dist: pypdf (>=4.1.0,<5.0.0) Requires-Dist: python-
-dotenv (==1.0.1) Requires-Dist: qdrant-client (>=1.9.0,<2.0.0) ; extra ==
-"qdrant" Requires-Dist: ruff (>=0.2.2,<0.3.0) Requires-Dist: scikit-learn
-(>=1.4.1.post1,<2.0.0) Requires-Dist: sqlalchemy (>=2.0.21,<3.0.0) Requires-
-Dist: structlog (>=24.1.0,<25.0.0) Requires-Dist: tantivy (>=0.21.0,<0.22.0)
-Requires-Dist: tenacity (>=8.2.3,<9.0.0) Requires-Dist: tiktoken
-(>=0.6.0,<0.7.0) Requires-Dist: uvicorn (==0.22.0) Requires-Dist: weaviate-
-client (>=4.5.4,<5.0.0) ; extra == "weaviate" Project-URL: Repository, https://
-github.com/topoteretes/cognee Description-Content-Type: text/markdown # cognee
-Deterministic LLMs Outputs for AI Engineers using graphs, LLMs and vector
-retrieval
+Requires-Dist: protobuf (<5.0.0) Requires-Dist: pyarrow (>=15.0.0,<16.0.0) ;
+extra == "parquet" or extra == "motherduck" Requires-Dist: pydantic
+(>=2.5.0,<3.0.0) Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0) Requires-
+Dist: pylint (>=3.0.3,<4.0.0) Requires-Dist: pypdf (>=4.1.0,<5.0.0) Requires-
+Dist: python-dotenv (==1.0.1) Requires-Dist: python-multipart (>=0.0.9,<0.0.10)
+Requires-Dist: qdrant-client (>=1.9.0,<2.0.0) ; extra == "qdrant" Requires-
+Dist: ruff (>=0.2.2,<0.3.0) Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0)
+Requires-Dist: spacy (>=3.7.4,<4.0.0) Requires-Dist: sqlalchemy
+(>=2.0.21,<3.0.0) Requires-Dist: structlog (>=24.1.0,<25.0.0) Requires-Dist:
+tantivy (>=0.21.0,<0.22.0) Requires-Dist: tenacity (>=8.2.3,<9.0.0) Requires-
+Dist: tiktoken (>=0.6.0,<0.7.0) Requires-Dist: uvicorn (==0.22.0) Requires-
+Dist: weaviate-client (>=4.5.4,<5.0.0) ; extra == "weaviate" Project-URL:
+Repository, https://github.com/topoteretes/cognee Description-Content-Type:
+text/markdown # cognee Deterministic LLMs Outputs for AI Engineers using
+graphs, LLMs and vector retrieval
 _[_C_o_g_n_e_e_ _l_o_g_o_]
 Open-source framework for creating self-improving deterministic outputs for
 LLMs.
 _[_c_o_g_n_e_e_ _f_o_r_k_s_]_[_c_o_g_n_e_e_ _s_t_a_r_s_]_[_c_o_g_n_e_e_ _p_u_l_l_-_r_e_q_u_e_s_t_s_]_[_c_o_g_n_e_e_ _r_e_l_e_a_s_e_s_]
 ![Cognee Demo](assets/cognee_demo.gif) Try it in a Google collab _n_o_t_e_b_o_o_k or
-have a look at our _d_o_c_u_m_e_n_t_a_t_i_o_n Join our _D_i_s_c_o_r_d community ## ð¦
-Installation ### With pip ```bash pip install cognee ``` Use Weaviate vector
-storage: ```bash pip install "cognee[weaviate]" ``` ### With poetry ```bash
-poetry add cognee ``` Use Weaviate vector storage: ```bash poetry add "cognee
-[weaviate]" ``` ## ð» Usage ### Setup ``` import os os.environ
-["WEAVIATE_URL"] = "YOUR_WEAVIATE_URL" os.environ["WEAVIATE_API_KEY"] =
-"YOUR_WEAVIATE_API_KEY" os.environ["OPENAI_API_KEY"] = "YOUR_OPENAI_API_KEY"
-``` You can also use Ollama or Anyscale as your LLM provider. For more info on
-local models check our [docs](https://topoteretes.github.io/cognee) ### Run ```
-import cognee text = """Natural language processing (NLP) is an
-interdisciplinary subfield of computer science and information retrieval"""
-cognee.add([text], "example_dataset") # Add a new piece of information
-cognee.cognify() # Use LLMs and cognee to create knowledge search_results =
-cognee.search("SIMILARITY", "computer science") # Query cognee for the
-knowledge for result_text in search_results[0]: print(result_text) ``` Add
-alternative data types: ``` cognee.add("file://{absolute_path_to_file}",
-dataset_name) ``` Or ``` cognee.add("data://{absolute_path_to_directory}",
-dataset_name) # This is useful if you have a directory with files organized in
-subdirectories. # You can target which directory to add by providing
-dataset_name. # Example: # root # / \ # reports bills # / \ # 2024 2023 # #
-cognee.add("data://{absolute_path_to_root}", "reports.2024") # This will add
-just directory 2024 under reports. ``` Read more [here](docs/index.md#run). ##
-Demo Check out our demo notebook [here](https://github.com/topoteretes/cognee/
-blob/main/notebooks/cognee%20-%20Get%20Started.ipynb) [[https://i3.ytimg.com/
-vi/-ARUfIzhzC4/maxresdefault.jpg]](https://www.youtube.com/watch?v=BDFt4xVPmro
-"Learn about cognee: 55") ## How it works ![Image](assets/architecture.png) ##
-ð It's alive
-Try it yourself on Whatsapp with one of our _p_a_r_t_n_e_r_s by typing `/save {content
-you want to save}` followed by `/query {knowledge you saved previously}` For
-more info here are the _d_o_c_s
+have a look at our _d_o_c_u_m_e_n_t_a_t_i_o_n If you have questions, join our _D_i_s_c_o_r_d
+community ## ð¦ Installation ### With pip ```bash pip install cognee ``` ###
+With poetry ```bash poetry add cognee ``` ## ð» Usage ### Setup ``` import os
+os.environ["LLM_API_KEY"] = "YOUR OPENAI_API_KEY" ``` or ``` import cognee
+cognee.config.llm_api_key = "YOUR_OPENAI_API_KEY" ``` You can also use Ollama
+or Anyscale as your LLM provider. For more info on local models check our
+[docs](https://topoteretes.github.io/cognee) ### Run ``` import cognee text =
+"""Natural language processing (NLP) is an interdisciplinary subfield of
+computer science and information retrieval""" cognee.add([text],
+"example_dataset") # Add a new piece of information cognee.cognify() # Use LLMs
+and cognee to create knowledge search_results = cognee.search("SIMILARITY",
+"computer science") # Query cognee for the knowledge for result_text in
+search_results[0]: print(result_text) ``` Add alternative data types: ```
+cognee.add("file://{absolute_path_to_file}", dataset_name) ``` Or ```
+cognee.add("data://{absolute_path_to_directory}", dataset_name) # This is
+useful if you have a directory with files organized in subdirectories. # You
+can target which directory to add by providing dataset_name. # Example: # root
+# / \ # reports bills # / \ # 2024 2023 # # cognee.add("data://
+{absolute_path_to_root}", "reports.2024") # This will add just directory 2024
+under reports. ``` Read more [here](docs/index.md#run). ## Vector retrieval,
+Graphs and LLMs Cognee supports a variety of tools and services for different
+operations: - **Local Setup**: By default, LanceDB runs locally with NetworkX
+and OpenAI. - **Vector Stores**: Cognee supports Qdrant and Weaviate for vector
+storage. - **Language Models (LLMs)**: You can use either Anyscale or Ollama as
+your LLM provider. - **Graph Stores**: In addition to LanceDB, Neo4j is also
+supported for graph storage. ## Demo Check out our demo notebook [here](https:/
+/github.com/topoteretes/cognee/blob/main/notebooks/cognee%20-
+%20Get%20Started.ipynb) [[https://i3.ytimg.com/vi/-ARUfIzhzC4/
+maxresdefault.jpg]](https://www.youtube.com/watch?v=BDFt4xVPmro "Learn about
+cognee: 55") ## How it works ![Image](assets/architecture.png) ## Star History
+[![Star History Chart](https://api.star-history.com/svg?repos=topoteretes/
+cognee&type=Date)](https://star-history.com/#topoteretes/cognee&Date)
```

