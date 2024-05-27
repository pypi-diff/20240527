# Comparing `tmp/superlinked-5.4.0.tar.gz` & `tmp/superlinked-5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superlinked-5.4.0.tar", max compression
+gzip compressed data, was "superlinked-5.4.1.tar", max compression
```

## Comparing `superlinked-5.4.0.tar` & `superlinked-5.4.1.tar`

### file list

```diff
@@ -1,215 +1,214 @@
--rw-r--r--   0        0        0    11354 2024-05-27 14:19:00.632236 superlinked-5.4.0/LICENSE
--rw-r--r--   0        0        0    28655 2024-05-27 14:19:00.632236 superlinked-5.4.0/NOTICE
--rw-r--r--   0        0        0     6840 2024-05-27 14:19:00.632236 superlinked-5.4.0/PYPI_README.md
--rw-r--r--   0        0        0     3698 2024-05-27 14:22:13.568568 superlinked-5.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/evaluation/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/evaluation/charts/__init__.py
--rw-r--r--   0        0        0     5601 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/evaluation/charts/recency_plotter.py
--rw-r--r--   0        0        0     9028 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/evaluation/vector_sampler.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/calculation/__init__.py
--rw-r--r--   0        0        0      742 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/calculation/distance_metric.py
--rw-r--r--   0        0        0     1510 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/calculation/vector_similarity.py
--rw-r--r--   0        0        0      805 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/const.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/__init__.py
--rw-r--r--   0        0        0     3644 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/aggregation_node.py
--rw-r--r--   0        0        0     2509 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/categorical_similarity_node.py
--rw-r--r--   0        0        0     1520 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/chunking_node.py
--rw-r--r--   0        0        0     2095 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/comparison_filter_node.py
--rw-r--r--   0        0        0     2606 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/concatenation_node.py
--rw-r--r--   0        0        0     1106 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/constant_node.py
--rw-r--r--   0        0        0     4985 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/context.py
--rw-r--r--   0        0        0     1854 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/custom_node.py
--rw-r--r--   0        0        0     5923 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/dag.py
--rw-r--r--   0        0        0     1338 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/dag_effect.py
--rw-r--r--   0        0        0     3687 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/event_aggregation_node.py
--rw-r--r--   0        0        0     1004 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/exception.py
--rw-r--r--   0        0        0     2043 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/index_node.py
--rw-r--r--   0        0        0     1428 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/named_function_node.py
--rw-r--r--   0        0        0     4723 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/node.py
--rw-r--r--   0        0        0     3083 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/number_embedding_node.py
--rw-r--r--   0        0        0     1620 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/period_time.py
--rw-r--r--   0        0        0      897 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/persistence_params.py
--rw-r--r--   0        0        0     2487 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/recency_node.py
--rw-r--r--   0        0        0     1128 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/resolved_schema_reference.py
--rw-r--r--   0        0        0     2019 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/schema_dag.py
--rw-r--r--   0        0        0     1463 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/schema_field_node.py
--rw-r--r--   0        0        0     1378 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/schema_object_reference.py
--rw-r--r--   0        0        0     2250 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/text_embedding_node.py
--rw-r--r--   0        0        0     8107 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/data_types.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/embedding/__init__.py
--rw-r--r--   0        0        0     5201 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/embedding/categorical_similarity_embedding.py
--rw-r--r--   0        0        0     5890 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/embedding/chunking_util.py
--rw-r--r--   0        0        0     1507 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/embedding/custom_embedding.py
--rw-r--r--   0        0        0     1280 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/embedding/embedding.py
--rw-r--r--   0        0        0     3772 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/embedding/number_embedding.py
--rw-r--r--   0        0        0     8046 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/embedding/recency_embedding.py
--rw-r--r--   0        0        0     2134 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/embedding/sentence_transformer_embedding.py
--rw-r--r--   0        0        0     1250 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/exception.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/interface/__init__.py
--rw-r--r--   0        0        0     5851 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/interface/comparison_operand.py
--rw-r--r--   0        0        0      841 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/interface/comparison_operation_type.py
--rw-r--r--   0        0        0      808 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/interface/has_aggregation.py
--rw-r--r--   0        0        0      796 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/interface/has_default_vector.py
--rw-r--r--   0        0        0      718 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/interface/has_length.py
--rw-r--r--   0        0        0      836 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/interface/has_multiplier.py
--rw-r--r--   0        0        0      940 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/interface/weighted.py
--rw-r--r--   0        0        0     1322 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/observable.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/parser/__init__.py
--rw-r--r--   0        0        0     5829 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/parser/data_parser.py
--rw-r--r--   0        0        0     5402 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/parser/dataframe_parser.py
--rw-r--r--   0        0        0      814 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/parser/exception.py
--rw-r--r--   0        0        0     4628 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/parser/json_parser.py
--rw-r--r--   0        0        0     1354 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/parser/parsed_schema.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/__init__.py
--rw-r--r--   0        0        0     1072 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/event_schema.py
--rw-r--r--   0        0        0     1964 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/event_schema_object.py
--rw-r--r--   0        0        0     1014 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/exception.py
--rw-r--r--   0        0        0      627 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/general_type.py
--rw-r--r--   0        0        0     1392 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/id_schema_object.py
--rw-r--r--   0        0        0     1178 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/schema.py
--rw-r--r--   0        0        0     3189 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/schema_decorator.py
--rw-r--r--   0        0        0     3228 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/schema_factory.py
--rw-r--r--   0        0        0     5701 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/schema_object.py
--rw-r--r--   0        0        0     3170 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/schema_reference.py
--rw-r--r--   0        0        0      686 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/schema_type.py
--rw-r--r--   0        0        0     3220 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/schema_validator.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/source/__init__.py
--rw-r--r--   0        0        0      857 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/source/source.py
--rw-r--r--   0        0        0      647 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/source/types.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/space/__init__.py
--rw-r--r--   0        0        0     4492 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/space/aggregation.py
--rw-r--r--   0        0        0     2055 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/space/normalization.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/__init__.py
--rw-r--r--   0        0        0      820 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/entity.py
--rw-r--r--   0        0        0      855 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/entity_data.py
--rw-r--r--   0        0        0      696 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/entity_id.py
--rw-r--r--   0        0        0      627 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/exception.py
--rw-r--r--   0        0        0     1656 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/field.py
--rw-r--r--   0        0        0     2616 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/field_data.py
--rw-r--r--   0        0        0      757 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/field_data_type.py
--rw-r--r--   0        0        0     3514 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/field_encoder.py
--rw-r--r--   0        0        0     2772 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/field_type_converter.py
--rw-r--r--   0        0        0      746 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/persistence_type.py
--rw-r--r--   0        0        0      769 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/result_entity_data.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/search_index_creation/__init__.py
--rw-r--r--   0        0        0     1242 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py
--rw-r--r--   0        0        0      671 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/search_index_creation/search_algorithm.py
--rw-r--r--   0        0        0      692 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py
--rw-r--r--   0        0        0     2397 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/vdb_connector.py
--rw-r--r--   0        0        0     1095 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/vdb_knn_search_params.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage_manager/__init__.py
--rw-r--r--   0        0        0     5459 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage_manager/admin_fields.py
--rw-r--r--   0        0        0     5549 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage_manager/entity_builder.py
--rw-r--r--   0        0        0      720 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage_manager/header.py
--rw-r--r--   0        0        0     1079 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage_manager/knn_search_params.py
--rw-r--r--   0        0        0      932 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage_manager/search_result_item.py
--rw-r--r--   0        0        0    16654 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage_manager/storage_manager.py
--rw-r--r--   0        0        0     1533 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage_manager/storage_naming.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/util/__init__.py
--rw-r--r--   0        0        0      787 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/util/collection_util.py
--rw-r--r--   0        0        0     2074 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/util/dot_separated_path_util.py
--rw-r--r--   0        0        0     1777 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/util/generic_class_util.py
--rw-r--r--   0        0        0      707 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/util/immutable_model.py
--rw-r--r--   0        0        0     1058 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/util/named_function_evaluator.py
--rw-r--r--   0        0        0     1642 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/util/string_util.py
--rw-r--r--   0        0        0      907 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/util/time_util.py
--rw-r--r--   0        0        0     4383 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/util/type_validator.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/compiler/__init__.py
--rw-r--r--   0        0        0     2399 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/compiler/online_schema_dag_compiler.py
--rw-r--r--   0        0        0      108 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/__init__.py
--rw-r--r--   0        0        0      221 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/executor/__init__.py
--rw-r--r--   0        0        0      719 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/executor/exception.py
--rw-r--r--   0        0        0     3836 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/executor/executor.py
--rw-r--r--   0        0        0      124 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/executor/in_memory/__init__.py
--rw-r--r--   0        0        0     7115 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py
--rw-r--r--   0        0        0      119 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/executor/query/__init__.py
--rw-r--r--   0        0        0     6804 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/executor/query/query_executor.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/executor/rest/__init__.py
--rw-r--r--   0        0        0     1540 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/executor/rest/rest_configuration.py
--rw-r--r--   0        0        0      818 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/executor/rest/rest_descriptor.py
--rw-r--r--   0        0        0     4834 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/executor/rest/rest_executor.py
--rw-r--r--   0        0        0     3236 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/executor/rest/rest_handler.py
--rw-r--r--   0        0        0      176 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/index/__init__.py
--rw-r--r--   0        0        0     1904 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/index/effect.py
--rw-r--r--   0        0        0    10985 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/index/index.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/index/util/__init__.py
--rw-r--r--   0        0        0     1516 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/index/util/aggregation_effect_group.py
--rw-r--r--   0        0        0     2448 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/index/util/aggregation_node_util.py
--rw-r--r--   0        0        0     6203 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py
--rw-r--r--   0        0        0     2557 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py
--rw-r--r--   0        0        0     3673 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/index/util/event_aggregation_node_util.py
--rw-r--r--   0        0        0      192 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/__init__.py
--rw-r--r--   0        0        0     1183 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/param.py
--rw-r--r--   0        0        0     3798 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/param_evaluator.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/predicate/__init__.py
--rw-r--r--   0        0        0      756 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/predicate/binary_op.py
--rw-r--r--   0        0        0     1521 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/predicate/binary_predicate.py
--rw-r--r--   0        0        0      924 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/predicate/evaluated_binary_predicate.py
--rw-r--r--   0        0        0     1128 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/predicate/query_predicate.py
--rw-r--r--   0        0        0    13227 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/query.py
--rw-r--r--   0        0        0     6223 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/query_filters.py
--rw-r--r--   0        0        0     6842 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/query_vector_factory.py
--rw-r--r--   0        0        0     3329 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/query_weighting.py
--rw-r--r--   0        0        0     2613 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/result.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/registry/__init__.py
--rw-r--r--   0        0        0      636 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/registry/exception.py
--rw-r--r--   0        0        0     1330 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/registry/superlinked_registry.py
--rw-r--r--   0        0        0      214 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/source/__init__.py
--rw-r--r--   0        0        0     2225 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/source/data_loader_source.py
--rw-r--r--   0        0        0     2773 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/source/in_memory_source.py
--rw-r--r--   0        0        0     1987 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/source/rest_source.py
--rw-r--r--   0        0        0     1144 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/source/source.py
--rw-r--r--   0        0        0      183 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/space/__init__.py
--rw-r--r--   0        0        0     7479 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/space/categorical_similarity_space.py
--rw-r--r--   0        0        0     5509 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/space/custom_space.py
--rw-r--r--   0        0        0      856 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/space/exception.py
--rw-r--r--   0        0        0     7702 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/space/number_space.py
--rw-r--r--   0        0        0     8456 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/space/recency_space.py
--rw-r--r--   0        0        0     2743 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/space/space.py
--rw-r--r--   0        0        0     1295 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/space/space_field_set.py
--rw-r--r--   0        0        0     4804 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/space/text_similarity_space.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/evaluator/__init__.py
--rw-r--r--   0        0        0     1043 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/evaluator/dag_evaluator.py
--rw-r--r--   0        0        0     4807 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/evaluator/online_dag_evaluator.py
--rw-r--r--   0        0        0     2237 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/evaluator/query_dag_evaluator.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/__init__.py
--rw-r--r--   0        0        0      801 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/batched_chunk_input_item.py
--rw-r--r--   0        0        0     7597 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/default_online_node.py
--rw-r--r--   0        0        0     1213 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/evaluation_result.py
--rw-r--r--   0        0        0      768 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/exception.py
--rw-r--r--   0        0        0     6312 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_aggregation_node.py
--rw-r--r--   0        0        0     3206 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_categorical_similarity_node.py
--rw-r--r--   0        0        0     3457 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_chunking_node.py
--rw-r--r--   0        0        0     2247 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_comparison_filter_node.py
--rw-r--r--   0        0        0     5138 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_concatenation_node.py
--rw-r--r--   0        0        0     2032 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_constant_node.py
--rw-r--r--   0        0        0     3283 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_custom_node.py
--rw-r--r--   0        0        0     7908 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_event_aggregation_node.py
--rw-r--r--   0        0        0     4052 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_index_node.py
--rw-r--r--   0        0        0     2351 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_named_function_node.py
--rw-r--r--   0        0        0     5086 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_node.py
--rw-r--r--   0        0        0     5547 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_node_registry.py
--rw-r--r--   0        0        0     3704 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_number_embedding_node.py
--rw-r--r--   0        0        0     2713 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/online/dag/online_recency_node.py
--rw-r--r--   0        0        0     3732 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/online/dag/online_schema_dag.py
--rw-r--r--   0        0        0     3426 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/online/dag/online_schema_field_node.py
--rw-r--r--   0        0        0     3256 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/online/dag/online_text_embedding_node.py
--rw-r--r--   0        0        0      794 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/online/dag/parent_results.py
--rw-r--r--   0        0        0     1322 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/online/dag/parent_validator.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/online/source/__init__.py
--rw-r--r--   0        0        0     3486 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/online/source/in_memory_data_processor.py
--rw-r--r--   0        0        0     1437 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/online/source/in_memory_object_writer.py
--rw-r--r--   0        0        0     1752 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/online/source/in_memory_source.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/storage/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/storage/in_memory/__init__.py
--rw-r--r--   0        0        0      787 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/storage/in_memory/exception.py
--rw-r--r--   0        0        0     6725 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/storage/in_memory/in_memory_search.py
--rw-r--r--   0        0        0     7121 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/storage/in_memory/in_memory_vdb.py
--rw-r--r--   0        0        0      921 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/storage/in_memory/index_config.py
--rw-r--r--   0        0        0     1305 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/storage/in_memory/json_codec.py
--rw-r--r--   0        0        0     1562 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/storage/in_memory/object_serializer.py
--rw-r--r--   0        0        0        0 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/py.typed
--rw-r--r--   0        0        0     8320 1970-01-01 00:00:00.000000 superlinked-5.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11354 2024-05-27 14:52:32.189675 superlinked-5.4.1/LICENSE
+-rw-r--r--   0        0        0    28655 2024-05-27 14:52:32.189675 superlinked-5.4.1/NOTICE
+-rw-r--r--   0        0        0     6840 2024-05-27 14:52:32.189675 superlinked-5.4.1/PYPI_README.md
+-rw-r--r--   0        0        0     3698 2024-05-27 14:55:35.242219 superlinked-5.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/evaluation/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/evaluation/charts/__init__.py
+-rw-r--r--   0        0        0     5601 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/evaluation/charts/recency_plotter.py
+-rw-r--r--   0        0        0     9028 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/evaluation/vector_sampler.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/calculation/__init__.py
+-rw-r--r--   0        0        0      742 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/calculation/distance_metric.py
+-rw-r--r--   0        0        0     1510 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/calculation/vector_similarity.py
+-rw-r--r--   0        0        0      805 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/const.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/__init__.py
+-rw-r--r--   0        0        0     3644 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/aggregation_node.py
+-rw-r--r--   0        0        0     2509 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/categorical_similarity_node.py
+-rw-r--r--   0        0        0     1520 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/chunking_node.py
+-rw-r--r--   0        0        0     2095 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/comparison_filter_node.py
+-rw-r--r--   0        0        0     2606 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/concatenation_node.py
+-rw-r--r--   0        0        0     1106 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/constant_node.py
+-rw-r--r--   0        0        0     4985 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/context.py
+-rw-r--r--   0        0        0     1854 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/custom_node.py
+-rw-r--r--   0        0        0     5923 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/dag.py
+-rw-r--r--   0        0        0     1338 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/dag_effect.py
+-rw-r--r--   0        0        0     3687 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/event_aggregation_node.py
+-rw-r--r--   0        0        0     1004 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/exception.py
+-rw-r--r--   0        0        0     2043 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/index_node.py
+-rw-r--r--   0        0        0     1428 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/named_function_node.py
+-rw-r--r--   0        0        0     5016 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/node.py
+-rw-r--r--   0        0        0     3083 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/number_embedding_node.py
+-rw-r--r--   0        0        0     1620 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/period_time.py
+-rw-r--r--   0        0        0      897 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/persistence_params.py
+-rw-r--r--   0        0        0     2487 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/recency_node.py
+-rw-r--r--   0        0        0     1128 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/resolved_schema_reference.py
+-rw-r--r--   0        0        0     2019 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/schema_dag.py
+-rw-r--r--   0        0        0     1463 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/schema_field_node.py
+-rw-r--r--   0        0        0     1378 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/schema_object_reference.py
+-rw-r--r--   0        0        0     2250 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/text_embedding_node.py
+-rw-r--r--   0        0        0     8107 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/data_types.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/embedding/__init__.py
+-rw-r--r--   0        0        0     5201 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/embedding/categorical_similarity_embedding.py
+-rw-r--r--   0        0        0     5890 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/embedding/chunking_util.py
+-rw-r--r--   0        0        0     1507 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/embedding/custom_embedding.py
+-rw-r--r--   0        0        0     1280 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/embedding/embedding.py
+-rw-r--r--   0        0        0     3772 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/embedding/number_embedding.py
+-rw-r--r--   0        0        0     8046 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/embedding/recency_embedding.py
+-rw-r--r--   0        0        0     2134 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/embedding/sentence_transformer_embedding.py
+-rw-r--r--   0        0        0     1250 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/exception.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/interface/__init__.py
+-rw-r--r--   0        0        0     5851 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/interface/comparison_operand.py
+-rw-r--r--   0        0        0      841 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/interface/comparison_operation_type.py
+-rw-r--r--   0        0        0      808 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/interface/has_aggregation.py
+-rw-r--r--   0        0        0      796 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/interface/has_default_vector.py
+-rw-r--r--   0        0        0      718 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/interface/has_length.py
+-rw-r--r--   0        0        0      836 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/interface/has_multiplier.py
+-rw-r--r--   0        0        0      940 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/interface/weighted.py
+-rw-r--r--   0        0        0     1322 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/observable.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/parser/__init__.py
+-rw-r--r--   0        0        0     5829 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/parser/data_parser.py
+-rw-r--r--   0        0        0     5402 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/parser/dataframe_parser.py
+-rw-r--r--   0        0        0      814 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/parser/exception.py
+-rw-r--r--   0        0        0     4634 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/parser/json_parser.py
+-rw-r--r--   0        0        0     1396 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/parser/parsed_schema.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/__init__.py
+-rw-r--r--   0        0        0     1072 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/event_schema.py
+-rw-r--r--   0        0        0     1964 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/event_schema_object.py
+-rw-r--r--   0        0        0     1014 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/exception.py
+-rw-r--r--   0        0        0      627 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/general_type.py
+-rw-r--r--   0        0        0     1533 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/id_schema_object.py
+-rw-r--r--   0        0        0     1178 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/schema.py
+-rw-r--r--   0        0        0     3189 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/schema_decorator.py
+-rw-r--r--   0        0        0     3228 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/schema_factory.py
+-rw-r--r--   0        0        0     6448 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/schema_object.py
+-rw-r--r--   0        0        0     3170 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/schema_reference.py
+-rw-r--r--   0        0        0      686 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/schema_type.py
+-rw-r--r--   0        0        0     3220 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/schema_validator.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/source/__init__.py
+-rw-r--r--   0        0        0      857 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/source/source.py
+-rw-r--r--   0        0        0      647 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/source/types.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/space/__init__.py
+-rw-r--r--   0        0        0     4492 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/space/aggregation.py
+-rw-r--r--   0        0        0     2055 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/space/normalization.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/__init__.py
+-rw-r--r--   0        0        0      820 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/entity.py
+-rw-r--r--   0        0        0      855 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/entity_data.py
+-rw-r--r--   0        0        0      696 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/entity_id.py
+-rw-r--r--   0        0        0      627 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/exception.py
+-rw-r--r--   0        0        0     1656 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/field.py
+-rw-r--r--   0        0        0     2616 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/field_data.py
+-rw-r--r--   0        0        0      757 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/field_data_type.py
+-rw-r--r--   0        0        0     3514 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/field_encoder.py
+-rw-r--r--   0        0        0     2772 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/field_type_converter.py
+-rw-r--r--   0        0        0      746 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/persistence_type.py
+-rw-r--r--   0        0        0      769 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/result_entity_data.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/search_index_creation/__init__.py
+-rw-r--r--   0        0        0     1242 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py
+-rw-r--r--   0        0        0      671 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/search_index_creation/search_algorithm.py
+-rw-r--r--   0        0        0      692 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py
+-rw-r--r--   0        0        0     2397 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/vdb_connector.py
+-rw-r--r--   0        0        0     1095 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/vdb_knn_search_params.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage_manager/__init__.py
+-rw-r--r--   0        0        0     5459 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage_manager/admin_fields.py
+-rw-r--r--   0        0        0     5549 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage_manager/entity_builder.py
+-rw-r--r--   0        0        0      720 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage_manager/header.py
+-rw-r--r--   0        0        0     1079 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage_manager/knn_search_params.py
+-rw-r--r--   0        0        0      932 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage_manager/search_result_item.py
+-rw-r--r--   0        0        0    16654 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage_manager/storage_manager.py
+-rw-r--r--   0        0        0     1533 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage_manager/storage_naming.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/util/__init__.py
+-rw-r--r--   0        0        0      787 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/util/collection_util.py
+-rw-r--r--   0        0        0     2074 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/util/dot_separated_path_util.py
+-rw-r--r--   0        0        0     1777 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/util/generic_class_util.py
+-rw-r--r--   0        0        0      707 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/util/immutable_model.py
+-rw-r--r--   0        0        0     1058 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/util/named_function_evaluator.py
+-rw-r--r--   0        0        0     1642 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/util/string_util.py
+-rw-r--r--   0        0        0      907 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/util/time_util.py
+-rw-r--r--   0        0        0     4383 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/util/type_validator.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/compiler/__init__.py
+-rw-r--r--   0        0        0     2399 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/compiler/online_schema_dag_compiler.py
+-rw-r--r--   0        0        0      108 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/dsl/__init__.py
+-rw-r--r--   0        0        0      221 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/dsl/executor/__init__.py
+-rw-r--r--   0        0        0      719 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/dsl/executor/exception.py
+-rw-r--r--   0        0        0     3836 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/dsl/executor/executor.py
+-rw-r--r--   0        0        0      124 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/dsl/executor/in_memory/__init__.py
+-rw-r--r--   0        0        0     7115 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py
+-rw-r--r--   0        0        0      119 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/dsl/executor/query/__init__.py
+-rw-r--r--   0        0        0     6902 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/dsl/executor/query/query_executor.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/executor/rest/__init__.py
+-rw-r--r--   0        0        0     1540 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/executor/rest/rest_configuration.py
+-rw-r--r--   0        0        0      818 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/executor/rest/rest_descriptor.py
+-rw-r--r--   0        0        0     4834 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/executor/rest/rest_executor.py
+-rw-r--r--   0        0        0     3236 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/executor/rest/rest_handler.py
+-rw-r--r--   0        0        0      176 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/index/__init__.py
+-rw-r--r--   0        0        0     1904 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/index/effect.py
+-rw-r--r--   0        0        0    10985 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/index/index.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/index/util/__init__.py
+-rw-r--r--   0        0        0     1516 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/index/util/aggregation_effect_group.py
+-rw-r--r--   0        0        0     2448 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/index/util/aggregation_node_util.py
+-rw-r--r--   0        0        0     6203 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py
+-rw-r--r--   0        0        0     2557 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py
+-rw-r--r--   0        0        0     3673 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/index/util/event_aggregation_node_util.py
+-rw-r--r--   0        0        0      192 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/query/__init__.py
+-rw-r--r--   0        0        0     1183 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/query/param.py
+-rw-r--r--   0        0        0     3503 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/query/param_evaluator.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/query/predicate/__init__.py
+-rw-r--r--   0        0        0      756 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/query/predicate/binary_op.py
+-rw-r--r--   0        0        0     2739 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/query/predicate/binary_predicate.py
+-rw-r--r--   0        0        0     1128 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/query/predicate/query_predicate.py
+-rw-r--r--   0        0        0    13577 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/query/query.py
+-rw-r--r--   0        0        0     6144 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/query/query_filters.py
+-rw-r--r--   0        0        0    11142 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/query/query_vector_factory.py
+-rw-r--r--   0        0        0     3329 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/query/query_weighting.py
+-rw-r--r--   0        0        0     2613 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/query/result.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/registry/__init__.py
+-rw-r--r--   0        0        0      636 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/registry/exception.py
+-rw-r--r--   0        0        0     1330 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/registry/superlinked_registry.py
+-rw-r--r--   0        0        0      214 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/source/__init__.py
+-rw-r--r--   0        0        0     2225 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/source/data_loader_source.py
+-rw-r--r--   0        0        0     2773 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/source/in_memory_source.py
+-rw-r--r--   0        0        0     1987 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/source/rest_source.py
+-rw-r--r--   0        0        0     1144 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/source/source.py
+-rw-r--r--   0        0        0      183 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/space/__init__.py
+-rw-r--r--   0        0        0     7479 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/space/categorical_similarity_space.py
+-rw-r--r--   0        0        0     5509 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/space/custom_space.py
+-rw-r--r--   0        0        0      856 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/space/exception.py
+-rw-r--r--   0        0        0     7702 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/space/number_space.py
+-rw-r--r--   0        0        0     8456 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/space/recency_space.py
+-rw-r--r--   0        0        0     2743 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/space/space.py
+-rw-r--r--   0        0        0     1295 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/space/space_field_set.py
+-rw-r--r--   0        0        0     4804 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/space/text_similarity_space.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/evaluator/__init__.py
+-rw-r--r--   0        0        0     1043 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/evaluator/dag_evaluator.py
+-rw-r--r--   0        0        0     4807 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/evaluator/online_dag_evaluator.py
+-rw-r--r--   0        0        0     2237 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/evaluator/query_dag_evaluator.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/__init__.py
+-rw-r--r--   0        0        0      801 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/batched_chunk_input_item.py
+-rw-r--r--   0        0        0     7597 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/default_online_node.py
+-rw-r--r--   0        0        0     1213 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/evaluation_result.py
+-rw-r--r--   0        0        0      768 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/exception.py
+-rw-r--r--   0        0        0     6312 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_aggregation_node.py
+-rw-r--r--   0        0        0     3206 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_categorical_similarity_node.py
+-rw-r--r--   0        0        0     3457 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_chunking_node.py
+-rw-r--r--   0        0        0     2247 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_comparison_filter_node.py
+-rw-r--r--   0        0        0     5138 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_concatenation_node.py
+-rw-r--r--   0        0        0     2032 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_constant_node.py
+-rw-r--r--   0        0        0     3283 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_custom_node.py
+-rw-r--r--   0        0        0     7908 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_event_aggregation_node.py
+-rw-r--r--   0        0        0     4052 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_index_node.py
+-rw-r--r--   0        0        0     2351 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_named_function_node.py
+-rw-r--r--   0        0        0     5086 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_node.py
+-rw-r--r--   0        0        0     5547 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_node_registry.py
+-rw-r--r--   0        0        0     3704 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_number_embedding_node.py
+-rw-r--r--   0        0        0     2713 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_recency_node.py
+-rw-r--r--   0        0        0     3732 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_schema_dag.py
+-rw-r--r--   0        0        0     3426 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_schema_field_node.py
+-rw-r--r--   0        0        0     3256 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_text_embedding_node.py
+-rw-r--r--   0        0        0      794 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/parent_results.py
+-rw-r--r--   0        0        0     1322 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/parent_validator.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/source/__init__.py
+-rw-r--r--   0        0        0     3486 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/source/in_memory_data_processor.py
+-rw-r--r--   0        0        0     1437 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/source/in_memory_object_writer.py
+-rw-r--r--   0        0        0     1752 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/source/in_memory_source.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/storage/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.249675 superlinked-5.4.1/superlinked/framework/storage/in_memory/__init__.py
+-rw-r--r--   0        0        0      787 2024-05-27 14:52:32.249675 superlinked-5.4.1/superlinked/framework/storage/in_memory/exception.py
+-rw-r--r--   0        0        0     6725 2024-05-27 14:52:32.249675 superlinked-5.4.1/superlinked/framework/storage/in_memory/in_memory_search.py
+-rw-r--r--   0        0        0     7121 2024-05-27 14:52:32.249675 superlinked-5.4.1/superlinked/framework/storage/in_memory/in_memory_vdb.py
+-rw-r--r--   0        0        0      921 2024-05-27 14:52:32.249675 superlinked-5.4.1/superlinked/framework/storage/in_memory/index_config.py
+-rw-r--r--   0        0        0     1305 2024-05-27 14:52:32.249675 superlinked-5.4.1/superlinked/framework/storage/in_memory/json_codec.py
+-rw-r--r--   0        0        0     1562 2024-05-27 14:52:32.249675 superlinked-5.4.1/superlinked/framework/storage/in_memory/object_serializer.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:52:32.249675 superlinked-5.4.1/superlinked/py.typed
+-rw-r--r--   0        0        0     8320 1970-01-01 00:00:00.000000 superlinked-5.4.1/PKG-INFO
```

### Comparing `superlinked-5.4.0/LICENSE` & `superlinked-5.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/NOTICE` & `superlinked-5.4.1/NOTICE`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/PYPI_README.md` & `superlinked-5.4.1/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/pyproject.toml` & `superlinked-5.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "superlinked"
-version = "5.4.0"  # The version will be dynamically updated
+version = "5.4.1"  # The version will be dynamically updated
 description = "The Superlinked vector computing library"
 authors = ["Superlinked Release <release@superlinked.com>"]
 readme = "PYPI_README.md"
 license = "Apache-2.0"
 include = ["NOTICE"]
 
 [tool.poetry.dependencies]
```

### Comparing `superlinked-5.4.0/superlinked/evaluation/charts/recency_plotter.py` & `superlinked-5.4.1/superlinked/evaluation/charts/recency_plotter.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/evaluation/vector_sampler.py` & `superlinked-5.4.1/superlinked/evaluation/vector_sampler.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/calculation/distance_metric.py` & `superlinked-5.4.1/superlinked/framework/common/calculation/distance_metric.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/calculation/vector_similarity.py` & `superlinked-5.4.1/superlinked/framework/common/calculation/vector_similarity.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/const.py` & `superlinked-5.4.1/superlinked/framework/common/const.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/dag/aggregation_node.py` & `superlinked-5.4.1/superlinked/framework/common/dag/aggregation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/dag/categorical_similarity_node.py` & `superlinked-5.4.1/superlinked/framework/common/dag/categorical_similarity_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/dag/chunking_node.py` & `superlinked-5.4.1/superlinked/framework/common/dag/chunking_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/dag/comparison_filter_node.py` & `superlinked-5.4.1/superlinked/framework/common/dag/comparison_filter_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/dag/concatenation_node.py` & `superlinked-5.4.1/superlinked/framework/common/dag/concatenation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/dag/constant_node.py` & `superlinked-5.4.1/superlinked/framework/common/dag/constant_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/dag/context.py` & `superlinked-5.4.1/superlinked/framework/common/dag/context.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/dag/custom_node.py` & `superlinked-5.4.1/superlinked/framework/common/dag/custom_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/dag/dag.py` & `superlinked-5.4.1/superlinked/framework/common/dag/dag.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/dag/dag_effect.py` & `superlinked-5.4.1/superlinked/framework/common/dag/dag_effect.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/dag/event_aggregation_node.py` & `superlinked-5.4.1/superlinked/framework/common/dag/event_aggregation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/dag/exception.py` & `superlinked-5.4.1/superlinked/framework/common/dag/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/dag/index_node.py` & `superlinked-5.4.1/superlinked/framework/common/dag/index_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/dag/named_function_node.py` & `superlinked-5.4.1/superlinked/framework/common/dag/named_function_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/dag/node.py` & `superlinked-5.4.1/superlinked/framework/common/dag/node.py`

 * *Files 9% similar despite different names*

```diff
@@ -126,7 +126,16 @@
 
     def project_parents_for_dag_effect(self, dag_effect: DagEffect) -> list[Node]:
         if dag_effect in self.dag_effects:
             return [
                 parent for parent in self.parents if dag_effect in parent.dag_effects
             ]
         return []
+
+    def find_ancestor(self, type_: type[Node]) -> Node[Any] | None:
+        queue = self.parents.copy()
+        while queue:
+            parent = queue.pop(0)
+            if isinstance(parent, type_):
+                return parent
+            queue.extend(parent.parents)
+        return None
```

### Comparing `superlinked-5.4.0/superlinked/framework/common/dag/number_embedding_node.py` & `superlinked-5.4.1/superlinked/framework/common/dag/number_embedding_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/dag/period_time.py` & `superlinked-5.4.1/superlinked/framework/common/dag/period_time.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/dag/persistence_params.py` & `superlinked-5.4.1/superlinked/framework/common/dag/persistence_params.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/dag/recency_node.py` & `superlinked-5.4.1/superlinked/framework/common/dag/recency_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/dag/resolved_schema_reference.py` & `superlinked-5.4.1/superlinked/framework/common/dag/resolved_schema_reference.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/dag/schema_dag.py` & `superlinked-5.4.1/superlinked/framework/common/dag/schema_dag.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/dag/schema_field_node.py` & `superlinked-5.4.1/superlinked/framework/common/dag/schema_field_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/dag/schema_object_reference.py` & `superlinked-5.4.1/superlinked/framework/common/dag/schema_object_reference.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/dag/text_embedding_node.py` & `superlinked-5.4.1/superlinked/framework/common/dag/text_embedding_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/data_types.py` & `superlinked-5.4.1/superlinked/framework/common/data_types.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/embedding/categorical_similarity_embedding.py` & `superlinked-5.4.1/superlinked/framework/common/embedding/categorical_similarity_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/embedding/chunking_util.py` & `superlinked-5.4.1/superlinked/framework/common/embedding/chunking_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/embedding/custom_embedding.py` & `superlinked-5.4.1/superlinked/framework/common/embedding/custom_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/embedding/embedding.py` & `superlinked-5.4.1/superlinked/framework/common/embedding/embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/embedding/number_embedding.py` & `superlinked-5.4.1/superlinked/framework/common/embedding/number_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/embedding/recency_embedding.py` & `superlinked-5.4.1/superlinked/framework/common/embedding/recency_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/embedding/sentence_transformer_embedding.py` & `superlinked-5.4.1/superlinked/framework/common/embedding/sentence_transformer_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/exception.py` & `superlinked-5.4.1/superlinked/framework/common/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/interface/comparison_operand.py` & `superlinked-5.4.1/superlinked/framework/common/interface/comparison_operand.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/interface/comparison_operation_type.py` & `superlinked-5.4.1/superlinked/framework/common/interface/comparison_operation_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/interface/has_aggregation.py` & `superlinked-5.4.1/superlinked/framework/common/interface/has_aggregation.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/interface/has_default_vector.py` & `superlinked-5.4.1/superlinked/framework/common/interface/has_default_vector.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/interface/has_length.py` & `superlinked-5.4.1/superlinked/framework/common/interface/has_length.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/interface/has_multiplier.py` & `superlinked-5.4.1/superlinked/framework/common/interface/has_multiplier.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/interface/weighted.py` & `superlinked-5.4.1/superlinked/framework/common/interface/weighted.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/observable.py` & `superlinked-5.4.1/superlinked/framework/common/observable.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/parser/data_parser.py` & `superlinked-5.4.1/superlinked/framework/common/parser/data_parser.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/parser/dataframe_parser.py` & `superlinked-5.4.1/superlinked/framework/common/parser/dataframe_parser.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/parser/exception.py` & `superlinked-5.4.1/superlinked/framework/common/parser/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/parser/json_parser.py` & `superlinked-5.4.1/superlinked/framework/common/parser/json_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,10 +113,10 @@
 
     def __get_path(self, field: SchemaField[SFT]) -> str:
         return self.mapping.get(field, field.name)
 
     def __get_all_fields_from_parsed_schema(
         self, parsed_schema: ParsedSchema
     ) -> list[ParsedSchemaField]:
-        return parsed_schema.fields + [
+        return list(parsed_schema.fields) + [
             ParsedSchemaField.from_schema_field(self._schema.id, parsed_schema.id_)
         ]
```

### Comparing `superlinked-5.4.0/superlinked/framework/common/parser/parsed_schema.py` & `superlinked-5.4.1/superlinked/framework/common/parser/parsed_schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Generic
 
+from beartype.typing import Sequence
+
 from superlinked.framework.common.schema.id_schema_object import IdSchemaObject
 from superlinked.framework.common.schema.schema_object import SFT, SchemaField
 
 
 class ParsedSchemaField(Generic[SFT]):
     def __init__(self, schema_field: SchemaField[SFT], value: SFT) -> None:
         self.schema_field = schema_field
@@ -33,9 +35,9 @@
         return cls(schema_field, value)
 
 
 @dataclass
 class ParsedSchema:
     schema: IdSchemaObject
     id_: str
-    fields: list[ParsedSchemaField]
+    fields: Sequence[ParsedSchemaField]
     event_parsed_schema: ParsedSchema | None = None
```

### Comparing `superlinked-5.4.0/superlinked/framework/common/schema/event_schema.py` & `superlinked-5.4.1/superlinked/framework/common/schema/event_schema.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/schema/event_schema_object.py` & `superlinked-5.4.1/superlinked/framework/common/schema/event_schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/schema/exception.py` & `superlinked-5.4.1/superlinked/framework/common/schema/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/schema/general_type.py` & `superlinked-5.4.1/superlinked/framework/common/schema/general_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/schema/id_schema_object.py` & `superlinked-5.4.1/superlinked/framework/common/schema/id_schema_object.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import TypeVar
 
+from beartype.typing import Sequence
+
 from superlinked.framework.common.schema.schema_object import (
     SchemaField,
     SchemaObject,
     SchemaObjectT,
 )
 
 IdSchemaObjectT = TypeVar("IdSchemaObjectT", bound="IdSchemaObject")
@@ -27,14 +29,18 @@
     """
     A class representing an ID field in a schema object.
     """
 
     def __init__(self, schema_obj: SchemaObjectT, id_field_name: str) -> None:
         super().__init__(id_field_name, schema_obj, str)
 
+    @staticmethod
+    def join_values(values: Sequence[str]) -> str:
+        return ", ".join(values)
+
 
 class IdSchemaObject(SchemaObject):
     """
     Schema object with required ID field.
     """
 
     def __init__(self, base_cls: type, schema_name: str, id_field_name: str) -> None:
```

### Comparing `superlinked-5.4.0/superlinked/framework/common/schema/schema.py` & `superlinked-5.4.1/superlinked/framework/common/schema/schema.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/schema/schema_decorator.py` & `superlinked-5.4.1/superlinked/framework/common/schema/schema_decorator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/schema/schema_factory.py` & `superlinked-5.4.1/superlinked/framework/common/schema/schema_factory.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/schema/schema_object.py` & `superlinked-5.4.1/superlinked/framework/common/schema/schema_object.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+from abc import abstractmethod
 from dataclasses import dataclass
 from typing import Any, Generic, TypeVar
 
+import numpy as np
 from beartype.typing import Sequence
 
 from superlinked.framework.common.data_types import NPArray, PythonTypes
 from superlinked.framework.common.interface.comparison_operand import ComparisonOperand
 
 # Exclude from documentation.
 # A better approach would be to separate this file into atomic objects,
@@ -112,36 +114,49 @@
 
     @staticmethod
     def _built_in_not_equal(
         left_operand: ComparisonOperand[SchemaField], right_operand: object
     ) -> bool:
         return not SchemaField._built_in_equal(left_operand, right_operand)
 
+    @staticmethod
+    @abstractmethod
+    def join_values(values: Sequence[SFT]) -> SFT:
+        pass
+
 
 class String(SchemaField[str]):
     """
     Field of a schema that represents a string value.
 
     e.g.: `TextEmbeddingSpace` expects a String field as an input.
     """
 
     def __init__(self, name: str, schema_obj: SchemaObjectT) -> None:
         super().__init__(name, schema_obj, str)
 
+    @staticmethod
+    def join_values(values: Sequence[str]) -> str:
+        return ", ".join(values)
+
 
 class Timestamp(SchemaField[int]):
     """
     Field of a schema that represents a unix timestamp.
 
     e.g.: `RecencySpace` expects a Timestamp field as an input.
     """
 
     def __init__(self, name: str, schema_obj: SchemaObjectT) -> None:
         super().__init__(name, schema_obj, int)
 
+    @staticmethod
+    def join_values(values: Sequence[int]) -> int:
+        return int(sum(values) / len(values))
+
 
 NSFT = TypeVar("NSFT", float, int)
 
 
 class Number(Generic[NSFT], SchemaField[NSFT]):
     """
     Field of a schema that represents a union of Float and Integer.
@@ -154,32 +169,46 @@
     """
     Field of a schema that represents a float.
     """
 
     def __init__(self, name: str, schema_obj: SchemaObjectT) -> None:
         super().__init__(name, schema_obj, float)
 
+    @staticmethod
+    def join_values(values: Sequence[float]) -> float:
+        return sum(values) / len(values)
+
 
 class Integer(Number[int]):
     """
     Field of a schema that represents an integer.
     """
 
     def __init__(self, name: str, schema_obj: SchemaObjectT) -> None:
         super().__init__(name, schema_obj, int)
 
+    @staticmethod
+    def join_values(values: Sequence[int]) -> int:
+        return int(sum(values) / len(values))
+
 
 class Array(SchemaField[NPArray]):
     """
     Field of a schema that represents a vector.
     """
 
     def __init__(self, name: str, schema_obj: SchemaObjectT) -> None:
         super().__init__(name, schema_obj, NPArray)
 
+    @staticmethod
+    def join_values(
+        values: Sequence[NPArray],
+    ) -> NPArray:
+        return np.array(list(values)).mean(axis=0)
+
 
 ConcreteSchemaField = String | Timestamp | Float | Integer | Array
 ConcreteSchemaFieldT = TypeVar("ConcreteSchemaFieldT", bound="ConcreteSchemaField")
 
 
 @dataclass
 class SchemaFieldDescriptor:
```

### Comparing `superlinked-5.4.0/superlinked/framework/common/schema/schema_reference.py` & `superlinked-5.4.1/superlinked/framework/common/schema/schema_reference.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/schema/schema_type.py` & `superlinked-5.4.1/superlinked/framework/common/schema/schema_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/schema/schema_validator.py` & `superlinked-5.4.1/superlinked/framework/common/schema/schema_validator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/source/source.py` & `superlinked-5.4.1/superlinked/framework/common/source/source.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/source/types.py` & `superlinked-5.4.1/superlinked/framework/common/source/types.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/space/aggregation.py` & `superlinked-5.4.1/superlinked/framework/common/space/aggregation.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/space/normalization.py` & `superlinked-5.4.1/superlinked/framework/common/space/normalization.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/storage/entity.py` & `superlinked-5.4.1/superlinked/framework/common/storage/entity.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/storage/entity_data.py` & `superlinked-5.4.1/superlinked/framework/common/storage/entity_data.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/storage/entity_id.py` & `superlinked-5.4.1/superlinked/framework/common/storage/entity_id.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/storage/exception.py` & `superlinked-5.4.1/superlinked/framework/common/storage/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/storage/field.py` & `superlinked-5.4.1/superlinked/framework/common/storage/field.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/storage/field_data.py` & `superlinked-5.4.1/superlinked/framework/common/storage/field_data.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/storage/field_data_type.py` & `superlinked-5.4.1/superlinked/framework/common/storage/field_data_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/storage/field_encoder.py` & `superlinked-5.4.1/superlinked/framework/common/storage/field_encoder.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/storage/field_type_converter.py` & `superlinked-5.4.1/superlinked/framework/common/storage/field_type_converter.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/storage/persistence_type.py` & `superlinked-5.4.1/superlinked/framework/common/storage/persistence_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/storage/result_entity_data.py` & `superlinked-5.4.1/superlinked/framework/common/storage/result_entity_data.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py` & `superlinked-5.4.1/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/storage/search_index_creation/search_algorithm.py` & `superlinked-5.4.1/superlinked/framework/common/storage/search_index_creation/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py` & `superlinked-5.4.1/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/storage/vdb_connector.py` & `superlinked-5.4.1/superlinked/framework/common/storage/vdb_connector.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/storage/vdb_knn_search_params.py` & `superlinked-5.4.1/superlinked/framework/common/storage/vdb_knn_search_params.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/storage_manager/admin_fields.py` & `superlinked-5.4.1/superlinked/framework/common/storage_manager/admin_fields.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/storage_manager/entity_builder.py` & `superlinked-5.4.1/superlinked/framework/common/storage_manager/entity_builder.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/storage_manager/header.py` & `superlinked-5.4.1/superlinked/framework/common/storage_manager/header.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/storage_manager/knn_search_params.py` & `superlinked-5.4.1/superlinked/framework/common/storage_manager/knn_search_params.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/storage_manager/search_result_item.py` & `superlinked-5.4.1/superlinked/framework/common/storage_manager/search_result_item.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/storage_manager/storage_manager.py` & `superlinked-5.4.1/superlinked/framework/common/storage_manager/storage_manager.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/storage_manager/storage_naming.py` & `superlinked-5.4.1/superlinked/framework/common/storage_manager/storage_naming.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/util/collection_util.py` & `superlinked-5.4.1/superlinked/framework/common/util/collection_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/util/dot_separated_path_util.py` & `superlinked-5.4.1/superlinked/framework/common/util/dot_separated_path_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/util/generic_class_util.py` & `superlinked-5.4.1/superlinked/framework/common/util/generic_class_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/util/immutable_model.py` & `superlinked-5.4.1/superlinked/framework/common/util/immutable_model.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/util/named_function_evaluator.py` & `superlinked-5.4.1/superlinked/framework/common/util/named_function_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/util/string_util.py` & `superlinked-5.4.1/superlinked/framework/common/util/string_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/util/time_util.py` & `superlinked-5.4.1/superlinked/framework/common/util/time_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/common/util/type_validator.py` & `superlinked-5.4.1/superlinked/framework/common/util/type_validator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/compiler/online_schema_dag_compiler.py` & `superlinked-5.4.1/superlinked/framework/compiler/online_schema_dag_compiler.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/executor/exception.py` & `superlinked-5.4.1/superlinked/framework/dsl/executor/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/executor/executor.py` & `superlinked-5.4.1/superlinked/framework/dsl/executor/executor.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py` & `superlinked-5.4.1/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/executor/query/query_executor.py` & `superlinked-5.4.1/superlinked/framework/dsl/executor/query/query_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,19 @@
             query_filters,
             space_weight_map,
             self.query_obj.schema,
             self._create_query_context_base(),
         )
 
     def _create_query_filters(self, param_evaluator: ParamEvaluator) -> QueryFilters:
-        return QueryFilters(self.query_obj.filters, param_evaluator)
+        return QueryFilters(
+            self.query_obj.looks_like_filter,
+            self.query_obj.similar_filters_by_space,
+            param_evaluator,
+        )
 
     def _create_query_context_base(self) -> ExecutionContext:
         eval_context = ExecutionContext(
             environment=ExecutionEnvironment.QUERY,
             data=self.app.executor.context.data,
             now_strategy=NowStrategy.CONTEXT_TIME,
         )
```

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/executor/rest/rest_configuration.py` & `superlinked-5.4.1/superlinked/framework/dsl/executor/rest/rest_configuration.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/executor/rest/rest_descriptor.py` & `superlinked-5.4.1/superlinked/framework/dsl/executor/rest/rest_descriptor.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/executor/rest/rest_executor.py` & `superlinked-5.4.1/superlinked/framework/dsl/executor/rest/rest_executor.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/executor/rest/rest_handler.py` & `superlinked-5.4.1/superlinked/framework/dsl/executor/rest/rest_handler.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/index/effect.py` & `superlinked-5.4.1/superlinked/framework/dsl/index/effect.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/index/index.py` & `superlinked-5.4.1/superlinked/framework/dsl/index/index.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/index/util/aggregation_effect_group.py` & `superlinked-5.4.1/superlinked/framework/dsl/index/util/aggregation_effect_group.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/index/util/aggregation_node_util.py` & `superlinked-5.4.1/superlinked/framework/dsl/index/util/aggregation_node_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py` & `superlinked-5.4.1/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py` & `superlinked-5.4.1/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/index/util/event_aggregation_node_util.py` & `superlinked-5.4.1/superlinked/framework/dsl/index/util/event_aggregation_node_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/query/param.py` & `superlinked-5.4.1/superlinked/framework/dsl/query/param.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/query/param_evaluator.py` & `superlinked-5.4.1/superlinked/framework/dsl/query/param_evaluator.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,37 +12,35 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Any
 
 from superlinked.framework.common.const import DEFAULT_WEIGHT
 from superlinked.framework.common.exception import QueryException
-from superlinked.framework.dsl.query.param import IntParamType, NumericParamType, Param
-from superlinked.framework.dsl.query.predicate.binary_predicate import BinaryPredicate
-from superlinked.framework.dsl.query.predicate.evaluated_binary_predicate import (
+from superlinked.framework.dsl.query.param import (
+    IntParamType,
+    NumericParamType,
+    Param,
+    ParamInputType,
+    ParamType,
+)
+from superlinked.framework.dsl.query.predicate.binary_predicate import (
+    BPT,
     EvaluatedBinaryPredicate,
 )
 
 # Exclude from documentation.
 __pdoc__ = {}
 __pdoc__["ParamEvaluator"] = False
 
 
 class ParamEvaluator:
     def __init__(self, params: dict[str, Any]) -> None:
         self.params = params
 
-    def evaluate_filters(
-        self,
-        filters: list[BinaryPredicate],
-    ) -> list[EvaluatedBinaryPredicate]:
-        return [
-            self._evaluate_binary_predicate(query_filter) for query_filter in filters
-        ]
-
     def evaluate_weight_param(
         self,
         param: NumericParamType,
         default: float = DEFAULT_WEIGHT,
     ) -> float:
         value = self.evaluate_numeric_param(param, "Weight", default)
         if value is None:
@@ -80,26 +78,28 @@
         param: IntParamType | None,
     ) -> int | None:
         value = self._evaluate_param(param)
         if value is None or isinstance(value, int):
             return value
         raise QueryException(f"Limit should be int, got {value.__class__.__name__}")
 
-    def _evaluate_binary_predicate(
-        self, predicate: BinaryPredicate
-    ) -> EvaluatedBinaryPredicate:
+    def evaluate_binary_predicate(
+        self, predicate: BPT
+    ) -> EvaluatedBinaryPredicate[BPT]:
         return EvaluatedBinaryPredicate(
             predicate,
             self.evaluate_weight_param(predicate.weight_param),
             self._evaluate_param(predicate.right_param),
         )
 
     def _evaluate_param(
-        self, param: Param | int | str | float | None, default_value: Any = None
-    ) -> int | str | float | None:
+        self,
+        param: ParamType,
+        default_value: Any = None,
+    ) -> ParamInputType:
         if isinstance(param, Param):
             if param.name in self.params:
                 return self.params[param.name]
             if default_value is not None:
                 return default_value
             raise QueryException(
                 f"Though parameter '{param.name}' was defined in "
```

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/query/predicate/binary_op.py` & `superlinked-5.4.1/superlinked/framework/dsl/query/predicate/binary_op.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/query/predicate/binary_predicate.py` & `superlinked-5.4.1/superlinked/framework/online/dag/online_named_function_node.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,31 +8,60 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from superlinked.framework.common.dag.node import Node
-from superlinked.framework.common.schema.schema_object import SchemaField
-from superlinked.framework.dsl.query.param import NumericParamType, Param
-from superlinked.framework.dsl.query.predicate.binary_op import BinaryOp
-from superlinked.framework.dsl.query.predicate.query_predicate import QueryPredicate
-
-# Exclude from documentation.
-__pdoc__ = {}
-__pdoc__["BinaryPredicate"] = False
+from __future__ import annotations
 
+from typing import cast
 
-class BinaryPredicate(QueryPredicate[BinaryOp]):
+from typing_extensions import override
+
+from superlinked.framework.common.dag.context import ExecutionContext
+from superlinked.framework.common.dag.named_function_node import NamedFunctionNode
+from superlinked.framework.common.dag.node import NDT
+from superlinked.framework.common.parser.parsed_schema import ParsedSchema
+from superlinked.framework.common.storage_manager.storage_manager import StorageManager
+from superlinked.framework.common.util.named_function_evaluator import (
+    NamedFunctionEvaluator,
+)
+from superlinked.framework.online.dag.evaluation_result import EvaluationResult
+from superlinked.framework.online.dag.online_node import OnlineNode
+from superlinked.framework.online.dag.parent_validator import ParentValidationType
+
+
+class OnlineNamedFunctionNode(OnlineNode[NamedFunctionNode[NDT], NDT]):
     def __init__(
         self,
-        op: BinaryOp,
-        left_param: SchemaField,
-        right_param: Param | str | int | float | None,
-        weight: NumericParamType,
-        left_param_node: Node | None = None,
+        node: NamedFunctionNode,
+        parents: list[OnlineNode],
+        storage_manager: StorageManager,
     ) -> None:
-        super().__init__(op=op, params=[left_param, right_param], weight_param=weight)
-        self.left_param = left_param
-        self.right_param = right_param
-        self.left_param_node = left_param_node
+        super().__init__(
+            node,
+            parents,
+            storage_manager,
+            ParentValidationType.NO_PARENTS,
+        )
+
+    @override
+    def evaluate_self(
+        self,
+        parsed_schemas: list[ParsedSchema],
+        context: ExecutionContext,
+    ) -> list[EvaluationResult[NDT]]:
+        result = EvaluationResult(
+            self._get_single_evaluation_result(self._evaluate_single(context))
+        )
+        return [result for _ in parsed_schemas]
+
+    def _evaluate_single(
+        self,
+        context: ExecutionContext,
+    ) -> NDT:
+        result = cast(
+            NDT,
+            NamedFunctionEvaluator().evaluate(self.node.named_function, context),
+        )
+        return result
```

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/query/predicate/evaluated_binary_predicate.py` & `superlinked-5.4.1/superlinked/framework/online/dag/parent_results.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,21 +8,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from dataclasses import dataclass
+from superlinked.framework.online.dag.evaluation_result import SingleEvaluationResult
+from superlinked.framework.online.dag.online_node import OnlineNode
 
-from superlinked.framework.dsl.query.predicate.binary_predicate import BinaryPredicate
-
-# Exclude from documentation.
-__pdoc__ = {}
-__pdoc__["EvaluatedBinaryPredicate"] = False
-
-
-@dataclass
-class EvaluatedBinaryPredicate:
-    predicate: BinaryPredicate
-    weight: float
-    value: int | str | float | None
+ParentResults = dict[OnlineNode, SingleEvaluationResult]
```

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/query/predicate/query_predicate.py` & `superlinked-5.4.1/superlinked/framework/dsl/query/predicate/query_predicate.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/query/query.py` & `superlinked-5.4.1/superlinked/framework/dsl/query/query.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from typing import Annotated, TypedDict, cast
+from typing import Annotated, Sequence, TypedDict, cast
 
 from superlinked.framework.common.const import DEFAULT_WEIGHT
 from superlinked.framework.common.exception import (
     InvalidSchemaException,
     QueryException,
 )
 from superlinked.framework.common.interface.comparison_operand import (
@@ -35,17 +35,18 @@
 from superlinked.framework.dsl.index.index import Index
 from superlinked.framework.dsl.query.param import (
     IntParamType,
     NumericParamType,
     Param,
     ParamType,
 )
-from superlinked.framework.dsl.query.predicate.binary_op import BinaryOp
-from superlinked.framework.dsl.query.predicate.binary_predicate import BinaryPredicate
-from superlinked.framework.dsl.query.predicate.query_predicate import QueryPredicate
+from superlinked.framework.dsl.query.predicate.binary_predicate import (
+    LooksLikePredicate,
+    SimilarPredicate,
+)
 from superlinked.framework.dsl.space.space import Space
 from superlinked.framework.dsl.space.space_field_set import SpaceFieldSet
 
 # Exclude from documentation.
 __pdoc__ = {}
 __pdoc__["QueryObjInternalProperty"] = False
 
@@ -55,20 +56,20 @@
     ComparisonOperationType.NOT_EQUAL,
 ]
 
 
 class QueryObjInternalProperty(TypedDict, total=False):
     """Only intended for self initialization inside QueryObj functions, not for external initialization"""
 
-    filters: list[QueryPredicate]
+    looks_like_filter: LooksLikePredicate | None
+    similar_filters_by_space: dict[Space, Sequence[SimilarPredicate]]
     limit: IntParamType | None
     radius: NumericParamType | None
     hard_filters: list[ComparisonOperation[SchemaField]]
     override_now: int | None
-    filtered_spaces: set[Space]
 
 
 @TypeValidator.wrap
 class QueryObj:  # pylint: disable=too-many-instance-attributes
     """
     A class representing a query object. Use .with_vector to run queries using a stored
     vector, or use .similar for queries where you supply the query at query-time. Or combine
@@ -93,23 +94,25 @@
             builder (Query): The query builder.
             schema (IdSchemaObject): The schema object.
         """
         self.builder = builder
         self.schema = cast(IdSchemaObject, schema)
         if not internal_property:
             internal_property = {}
-        self.filters = internal_property.get("filters", list[QueryPredicate]())
+        self.looks_like_filter = internal_property.get("looks_like_filter")
+        self.similar_filters_by_space = internal_property.get(
+            "similar_filters_by_space", dict[Space, Sequence[SimilarPredicate]]()
+        )
         self.hard_filters = internal_property.get(
             "hard_filters", list[ComparisonOperation[SchemaField]]()
         )
         self.limit_ = internal_property.get("limit")
         self.radius_ = internal_property.get("radius")
         # by default now in queries is the system time, but it can be overridden for testing/reproducible notebooks
         self._override_now = internal_property.get("override_now")
-        self.__filtered_spaces = internal_property.get("filtered_spaces", set[Space]())
 
     @property
     def index(self) -> Index:
         """
         The index the query is executed on.
         """
         return self.builder.index
@@ -144,27 +147,32 @@
         if not self.__is_indexed_space(field_set.space):
             raise QueryException("Space isn't present in the index.")
 
         if self.__is_space_bound(field_set.space):
             raise QueryException("Space attempted to bound in query multiple times.")
 
         if relevant_field := field_set.get_field_for_schema(self.schema):
-            similar_filter = BinaryPredicate(
-                BinaryOp.SIMILAR,
+            similar_filter = SimilarPredicate(
                 relevant_field,
                 param,
                 weight,
                 field_set.space._get_node(self.schema),
             )
-            filtered_spaces = self.__filtered_spaces.copy()
-            filters = self.filters.copy()
-            filtered_spaces.add(field_set.space)
-            filters.append(similar_filter)
+
+            similar_filters_by_space = self.similar_filters_by_space.copy()
+            if field_set.space not in similar_filters_by_space:
+                similar_filters_by_space[field_set.space] = []
+            similar_filters = list(similar_filters_by_space[field_set.space])
+            similar_filters.append(similar_filter)
+            similar_filters_by_space[field_set.space] = similar_filters
+
             return self.__alter(
-                {"filters": filters, "filtered_spaces": filtered_spaces}
+                {
+                    "similar_filters_by_space": similar_filters_by_space,
+                }
             )
         raise InvalidSchemaException(
             f"'find' ({type(self.schema)}) is not in similarity field's schema types."
         )
 
     def limit(self, limit: IntParamType | None) -> QueryObj:
         """
@@ -220,24 +228,24 @@
         Returns:
             Self: The query object itself.
         """
         if not isinstance(schema_obj, IdSchemaObject):
             raise InvalidSchemaException(
                 f"'with_vector': {type(self.schema)} is not a schema."
             )
-        filters = self.filters.copy()
-        filters.append(
-            BinaryPredicate(
-                op=BinaryOp.LOOKS_LIKE,
-                left_param=schema_obj.id,
-                right_param=id_param,
-                weight=weight,
+        if self.looks_like_filter is not None:
+            raise QueryException(
+                "One query cannot have more than one 'with vector' filter."
             )
+        looks_like_filter = LooksLikePredicate(
+            left_param=schema_obj.id,
+            right_param=id_param,
+            weight=weight,
         )
-        return self.__alter({"filters": filters})
+        return self.__alter({"looks_like_filter": looks_like_filter})
 
     def filter(
         self, comparison_operation: ComparisonOperation[SchemaField]
     ) -> QueryObj:
         """
         Add a 'filter' clause to the query. This filters the results from the db
         to only contain items based on the filtering input.
@@ -268,23 +276,23 @@
         hard_filters.append(comparison_operation)
         return self.__alter({"hard_filters": hard_filters})
 
     def __is_indexed_space(self, space: Space) -> bool:
         return self.builder.index.has_space(space)
 
     def __is_space_bound(self, space: Space) -> bool:
-        return space in self.__filtered_spaces
+        return space in self.similar_filters_by_space.keys()
 
     def __alter(self, properties: QueryObjInternalProperty) -> QueryObj:
         properties_use: QueryObjInternalProperty = {
-            "filters": self.filters,
+            "looks_like_filter": self.looks_like_filter,
+            "similar_filters_by_space": self.similar_filters_by_space,
             "limit": self.limit_,
             "radius": self.radius_,
             "override_now": self._override_now,
-            "filtered_spaces": self.__filtered_spaces,
         }
         properties_use.update(properties)
         return QueryObj(
             builder=self.builder,
             schema=self.schema,
             internal_property=properties_use,
         )
```

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/query/query_weighting.py` & `superlinked-5.4.1/superlinked/framework/dsl/query/query_weighting.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/query/result.py` & `superlinked-5.4.1/superlinked/framework/dsl/query/result.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/registry/exception.py` & `superlinked-5.4.1/superlinked/framework/dsl/registry/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/registry/superlinked_registry.py` & `superlinked-5.4.1/superlinked/framework/dsl/registry/superlinked_registry.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/source/data_loader_source.py` & `superlinked-5.4.1/superlinked/framework/dsl/source/data_loader_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/source/in_memory_source.py` & `superlinked-5.4.1/superlinked/framework/dsl/source/in_memory_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/source/rest_source.py` & `superlinked-5.4.1/superlinked/framework/dsl/source/rest_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/source/source.py` & `superlinked-5.4.1/superlinked/framework/dsl/source/source.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/space/categorical_similarity_space.py` & `superlinked-5.4.1/superlinked/framework/dsl/space/categorical_similarity_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/space/custom_space.py` & `superlinked-5.4.1/superlinked/framework/dsl/space/custom_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/space/exception.py` & `superlinked-5.4.1/superlinked/framework/dsl/space/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/space/number_space.py` & `superlinked-5.4.1/superlinked/framework/dsl/space/number_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/space/recency_space.py` & `superlinked-5.4.1/superlinked/framework/dsl/space/recency_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/space/space.py` & `superlinked-5.4.1/superlinked/framework/dsl/space/space.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/space/space_field_set.py` & `superlinked-5.4.1/superlinked/framework/dsl/space/space_field_set.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/dsl/space/text_similarity_space.py` & `superlinked-5.4.1/superlinked/framework/dsl/space/text_similarity_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/evaluator/dag_evaluator.py` & `superlinked-5.4.1/superlinked/framework/evaluator/dag_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/evaluator/online_dag_evaluator.py` & `superlinked-5.4.1/superlinked/framework/evaluator/online_dag_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/evaluator/query_dag_evaluator.py` & `superlinked-5.4.1/superlinked/framework/evaluator/query_dag_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/online/dag/batched_chunk_input_item.py` & `superlinked-5.4.1/superlinked/framework/online/dag/batched_chunk_input_item.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/online/dag/default_online_node.py` & `superlinked-5.4.1/superlinked/framework/online/dag/default_online_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/online/dag/evaluation_result.py` & `superlinked-5.4.1/superlinked/framework/online/dag/evaluation_result.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/online/dag/exception.py` & `superlinked-5.4.1/superlinked/framework/online/dag/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/online/dag/online_aggregation_node.py` & `superlinked-5.4.1/superlinked/framework/online/dag/online_aggregation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/online/dag/online_categorical_similarity_node.py` & `superlinked-5.4.1/superlinked/framework/online/dag/online_categorical_similarity_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/online/dag/online_chunking_node.py` & `superlinked-5.4.1/superlinked/framework/online/dag/online_chunking_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/online/dag/online_comparison_filter_node.py` & `superlinked-5.4.1/superlinked/framework/online/dag/online_comparison_filter_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/online/dag/online_concatenation_node.py` & `superlinked-5.4.1/superlinked/framework/online/dag/online_concatenation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/online/dag/online_constant_node.py` & `superlinked-5.4.1/superlinked/framework/online/dag/online_constant_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/online/dag/online_custom_node.py` & `superlinked-5.4.1/superlinked/framework/online/dag/online_custom_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/online/dag/online_event_aggregation_node.py` & `superlinked-5.4.1/superlinked/framework/online/dag/online_event_aggregation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/online/dag/online_index_node.py` & `superlinked-5.4.1/superlinked/framework/online/dag/online_index_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/online/dag/online_node.py` & `superlinked-5.4.1/superlinked/framework/online/dag/online_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/online/dag/online_node_registry.py` & `superlinked-5.4.1/superlinked/framework/online/dag/online_node_registry.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/online/dag/online_number_embedding_node.py` & `superlinked-5.4.1/superlinked/framework/online/dag/online_number_embedding_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/online/dag/online_recency_node.py` & `superlinked-5.4.1/superlinked/framework/online/dag/online_recency_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/online/dag/online_schema_dag.py` & `superlinked-5.4.1/superlinked/framework/online/dag/online_schema_dag.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/online/dag/online_schema_field_node.py` & `superlinked-5.4.1/superlinked/framework/online/dag/online_schema_field_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/online/dag/online_text_embedding_node.py` & `superlinked-5.4.1/superlinked/framework/online/dag/online_text_embedding_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/online/dag/parent_validator.py` & `superlinked-5.4.1/superlinked/framework/online/dag/parent_validator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/online/source/in_memory_data_processor.py` & `superlinked-5.4.1/superlinked/framework/online/source/in_memory_data_processor.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/online/source/in_memory_object_writer.py` & `superlinked-5.4.1/superlinked/framework/online/source/in_memory_object_writer.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/online/source/in_memory_source.py` & `superlinked-5.4.1/superlinked/framework/online/source/in_memory_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/storage/in_memory/exception.py` & `superlinked-5.4.1/superlinked/framework/storage/in_memory/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/storage/in_memory/in_memory_search.py` & `superlinked-5.4.1/superlinked/framework/storage/in_memory/in_memory_search.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/storage/in_memory/in_memory_vdb.py` & `superlinked-5.4.1/superlinked/framework/storage/in_memory/in_memory_vdb.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/storage/in_memory/index_config.py` & `superlinked-5.4.1/superlinked/framework/storage/in_memory/index_config.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/storage/in_memory/json_codec.py` & `superlinked-5.4.1/superlinked/framework/storage/in_memory/json_codec.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/superlinked/framework/storage/in_memory/object_serializer.py` & `superlinked-5.4.1/superlinked/framework/storage/in_memory/object_serializer.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.0/PKG-INFO` & `superlinked-5.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superlinked
-Version: 5.4.0
+Version: 5.4.1
 Summary: The Superlinked vector computing library
 License: Apache-2.0
 Author: Superlinked Release
 Author-email: release@superlinked.com
 Requires-Python: >=3.10,<=3.12.3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

