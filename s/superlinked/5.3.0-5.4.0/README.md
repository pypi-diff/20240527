# Comparing `tmp/superlinked-5.3.0.tar.gz` & `tmp/superlinked-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superlinked-5.3.0.tar", max compression
+gzip compressed data, was "superlinked-5.4.0.tar", max compression
```

## Comparing `superlinked-5.3.0.tar` & `superlinked-5.4.0.tar`

### file list

```diff
@@ -1,217 +1,215 @@
--rw-r--r--   0        0        0    11354 2024-05-24 14:18:57.324514 superlinked-5.3.0/LICENSE
--rw-r--r--   0        0        0    28655 2024-05-24 14:18:57.324514 superlinked-5.3.0/NOTICE
--rw-r--r--   0        0        0     6840 2024-05-24 14:18:57.324514 superlinked-5.3.0/PYPI_README.md
--rw-r--r--   0        0        0     3698 2024-05-24 14:22:04.365064 superlinked-5.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.372514 superlinked-5.3.0/superlinked/evaluation/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.372514 superlinked-5.3.0/superlinked/evaluation/charts/__init__.py
--rw-r--r--   0        0        0     5601 2024-05-24 14:18:57.372514 superlinked-5.3.0/superlinked/evaluation/charts/recency_plotter.py
--rw-r--r--   0        0        0     9028 2024-05-24 14:18:57.372514 superlinked-5.3.0/superlinked/evaluation/vector_sampler.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.372514 superlinked-5.3.0/superlinked/framework/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.372514 superlinked-5.3.0/superlinked/framework/common/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.372514 superlinked-5.3.0/superlinked/framework/common/calculation/__init__.py
--rw-r--r--   0        0        0      742 2024-05-24 14:18:57.372514 superlinked-5.3.0/superlinked/framework/common/calculation/distance_metric.py
--rw-r--r--   0        0        0     1510 2024-05-24 14:18:57.372514 superlinked-5.3.0/superlinked/framework/common/calculation/vector_similarity.py
--rw-r--r--   0        0        0      805 2024-05-24 14:18:57.372514 superlinked-5.3.0/superlinked/framework/common/const.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.372514 superlinked-5.3.0/superlinked/framework/common/dag/__init__.py
--rw-r--r--   0        0        0     3644 2024-05-24 14:18:57.372514 superlinked-5.3.0/superlinked/framework/common/dag/aggregation_node.py
--rw-r--r--   0        0        0     2288 2024-05-24 14:18:57.372514 superlinked-5.3.0/superlinked/framework/common/dag/categorical_similarity_node.py
--rw-r--r--   0        0        0     1520 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/dag/chunking_node.py
--rw-r--r--   0        0        0     2095 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/dag/comparison_filter_node.py
--rw-r--r--   0        0        0     2606 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/dag/concatenation_node.py
--rw-r--r--   0        0        0     1106 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/dag/constant_node.py
--rw-r--r--   0        0        0     4985 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/dag/context.py
--rw-r--r--   0        0        0     1854 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/dag/custom_node.py
--rw-r--r--   0        0        0     5923 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/dag/dag.py
--rw-r--r--   0        0        0     1338 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/dag/dag_effect.py
--rw-r--r--   0        0        0     3687 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/dag/event_aggregation_node.py
--rw-r--r--   0        0        0     1004 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/dag/exception.py
--rw-r--r--   0        0        0     2043 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/dag/index_node.py
--rw-r--r--   0        0        0     1428 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/dag/named_function_node.py
--rw-r--r--   0        0        0     4723 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/dag/node.py
--rw-r--r--   0        0        0     2422 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/dag/number_embedding_node.py
--rw-r--r--   0        0        0     2376 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/dag/number_similarity_node.py
--rw-r--r--   0        0        0     1620 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/dag/period_time.py
--rw-r--r--   0        0        0      897 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/dag/persistence_params.py
--rw-r--r--   0        0        0     2457 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/dag/recency_node.py
--rw-r--r--   0        0        0     1128 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/dag/resolved_schema_reference.py
--rw-r--r--   0        0        0     2019 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/dag/schema_dag.py
--rw-r--r--   0        0        0     1463 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/dag/schema_field_node.py
--rw-r--r--   0        0        0     1378 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/dag/schema_object_reference.py
--rw-r--r--   0        0        0     2035 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/dag/text_embedding_node.py
--rw-r--r--   0        0        0     8107 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/data_types.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/embedding/__init__.py
--rw-r--r--   0        0        0     5201 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/embedding/categorical_similarity_embedding.py
--rw-r--r--   0        0        0     5890 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/embedding/chunking_util.py
--rw-r--r--   0        0        0     1507 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/embedding/custom_embedding.py
--rw-r--r--   0        0        0     1280 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/embedding/embedding.py
--rw-r--r--   0        0        0     3138 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/embedding/number_embedding.py
--rw-r--r--   0        0        0     2424 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/embedding/number_similarity_embedding.py
--rw-r--r--   0        0        0     8046 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/embedding/recency_embedding.py
--rw-r--r--   0        0        0     2134 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/embedding/sentence_transformer_embedding.py
--rw-r--r--   0        0        0     1250 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/exception.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/interface/__init__.py
--rw-r--r--   0        0        0     5851 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/interface/comparison_operand.py
--rw-r--r--   0        0        0      841 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/interface/comparison_operation_type.py
--rw-r--r--   0        0        0      808 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/interface/has_aggregation.py
--rw-r--r--   0        0        0      718 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/interface/has_length.py
--rw-r--r--   0        0        0      836 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/interface/has_multiplier.py
--rw-r--r--   0        0        0      940 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/interface/weighted.py
--rw-r--r--   0        0        0     1322 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/observable.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/parser/__init__.py
--rw-r--r--   0        0        0     5829 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/parser/data_parser.py
--rw-r--r--   0        0        0     5402 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/parser/dataframe_parser.py
--rw-r--r--   0        0        0      814 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/parser/exception.py
--rw-r--r--   0        0        0     4628 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/parser/json_parser.py
--rw-r--r--   0        0        0     1354 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/parser/parsed_schema.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/schema/__init__.py
--rw-r--r--   0        0        0     1072 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/schema/event_schema.py
--rw-r--r--   0        0        0     1964 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/schema/event_schema_object.py
--rw-r--r--   0        0        0     1014 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/schema/exception.py
--rw-r--r--   0        0        0      627 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/schema/general_type.py
--rw-r--r--   0        0        0     1392 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/schema/id_schema_object.py
--rw-r--r--   0        0        0     1178 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/schema/schema.py
--rw-r--r--   0        0        0     3189 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/schema/schema_decorator.py
--rw-r--r--   0        0        0     3228 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/schema/schema_factory.py
--rw-r--r--   0        0        0     5701 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/schema/schema_object.py
--rw-r--r--   0        0        0     3170 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/schema/schema_reference.py
--rw-r--r--   0        0        0      686 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/schema/schema_type.py
--rw-r--r--   0        0        0     3220 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/schema/schema_validator.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/source/__init__.py
--rw-r--r--   0        0        0      857 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/source/source.py
--rw-r--r--   0        0        0      647 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/source/types.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/space/__init__.py
--rw-r--r--   0        0        0     4398 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/space/aggregation.py
--rw-r--r--   0        0        0     2055 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/space/normalization.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/storage/__init__.py
--rw-r--r--   0        0        0      820 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/storage/entity.py
--rw-r--r--   0        0        0      855 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/storage/entity_data.py
--rw-r--r--   0        0        0      696 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/storage/entity_id.py
--rw-r--r--   0        0        0      627 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/storage/exception.py
--rw-r--r--   0        0        0     1656 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/storage/field.py
--rw-r--r--   0        0        0     2616 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/storage/field_data.py
--rw-r--r--   0        0        0      757 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/storage/field_data_type.py
--rw-r--r--   0        0        0     3514 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/storage/field_encoder.py
--rw-r--r--   0        0        0     2772 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/storage/field_type_converter.py
--rw-r--r--   0        0        0      746 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/storage/persistence_type.py
--rw-r--r--   0        0        0      769 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/storage/result_entity_data.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/storage/search_index_creation/__init__.py
--rw-r--r--   0        0        0     1242 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py
--rw-r--r--   0        0        0      671 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/storage/search_index_creation/search_algorithm.py
--rw-r--r--   0        0        0      692 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py
--rw-r--r--   0        0        0     2397 2024-05-24 14:18:57.376514 superlinked-5.3.0/superlinked/framework/common/storage/vdb_connector.py
--rw-r--r--   0        0        0     1095 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/common/storage/vdb_knn_search_params.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/common/storage_manager/__init__.py
--rw-r--r--   0        0        0     5459 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/common/storage_manager/admin_fields.py
--rw-r--r--   0        0        0     5549 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/common/storage_manager/entity_builder.py
--rw-r--r--   0        0        0      720 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/common/storage_manager/header.py
--rw-r--r--   0        0        0     1079 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/common/storage_manager/knn_search_params.py
--rw-r--r--   0        0        0      932 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/common/storage_manager/search_result_item.py
--rw-r--r--   0        0        0    16654 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/common/storage_manager/storage_manager.py
--rw-r--r--   0        0        0     1533 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/common/storage_manager/storage_naming.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/common/util/__init__.py
--rw-r--r--   0        0        0      787 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/common/util/collection_util.py
--rw-r--r--   0        0        0     2074 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/common/util/dot_separated_path_util.py
--rw-r--r--   0        0        0     1777 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/common/util/generic_class_util.py
--rw-r--r--   0        0        0      707 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/common/util/immutable_model.py
--rw-r--r--   0        0        0     1058 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/common/util/named_function_evaluator.py
--rw-r--r--   0        0        0     1642 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/common/util/string_util.py
--rw-r--r--   0        0        0      907 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/common/util/time_util.py
--rw-r--r--   0        0        0     4383 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/common/util/type_validator.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/compiler/__init__.py
--rw-r--r--   0        0        0     2399 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/compiler/online_schema_dag_compiler.py
--rw-r--r--   0        0        0      108 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/__init__.py
--rw-r--r--   0        0        0      221 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/executor/__init__.py
--rw-r--r--   0        0        0      719 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/executor/exception.py
--rw-r--r--   0        0        0     3836 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/executor/executor.py
--rw-r--r--   0        0        0      124 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/executor/in_memory/__init__.py
--rw-r--r--   0        0        0     7115 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py
--rw-r--r--   0        0        0      119 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/executor/query/__init__.py
--rw-r--r--   0        0        0     6804 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/executor/query/query_executor.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/executor/rest/__init__.py
--rw-r--r--   0        0        0     1540 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/executor/rest/rest_configuration.py
--rw-r--r--   0        0        0      818 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/executor/rest/rest_descriptor.py
--rw-r--r--   0        0        0     4834 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/executor/rest/rest_executor.py
--rw-r--r--   0        0        0     3236 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/executor/rest/rest_handler.py
--rw-r--r--   0        0        0      176 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/index/__init__.py
--rw-r--r--   0        0        0     1904 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/index/effect.py
--rw-r--r--   0        0        0    10985 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/index/index.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/index/util/__init__.py
--rw-r--r--   0        0        0     1516 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/index/util/aggregation_effect_group.py
--rw-r--r--   0        0        0     2448 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/index/util/aggregation_node_util.py
--rw-r--r--   0        0        0     6203 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py
--rw-r--r--   0        0        0     2557 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py
--rw-r--r--   0        0        0     3673 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/index/util/event_aggregation_node_util.py
--rw-r--r--   0        0        0      192 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/query/__init__.py
--rw-r--r--   0        0        0     1183 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/query/param.py
--rw-r--r--   0        0        0     3798 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/query/param_evaluator.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/query/predicate/__init__.py
--rw-r--r--   0        0        0      756 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/query/predicate/binary_op.py
--rw-r--r--   0        0        0     1521 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/query/predicate/binary_predicate.py
--rw-r--r--   0        0        0      924 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/query/predicate/evaluated_binary_predicate.py
--rw-r--r--   0        0        0     1128 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/query/predicate/query_predicate.py
--rw-r--r--   0        0        0    13227 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/query/query.py
--rw-r--r--   0        0        0     6223 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/query/query_filters.py
--rw-r--r--   0        0        0     6842 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/query/query_vector_factory.py
--rw-r--r--   0        0        0     3329 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/query/query_weighting.py
--rw-r--r--   0        0        0     2613 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/query/result.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/registry/__init__.py
--rw-r--r--   0        0        0      636 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/registry/exception.py
--rw-r--r--   0        0        0     1330 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/registry/superlinked_registry.py
--rw-r--r--   0        0        0      214 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/source/__init__.py
--rw-r--r--   0        0        0     2225 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/source/data_loader_source.py
--rw-r--r--   0        0        0     2773 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/source/in_memory_source.py
--rw-r--r--   0        0        0     1987 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/source/rest_source.py
--rw-r--r--   0        0        0     1144 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/source/source.py
--rw-r--r--   0        0        0      183 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/space/__init__.py
--rw-r--r--   0        0        0     7479 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/space/categorical_similarity_space.py
--rw-r--r--   0        0        0     5509 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/space/custom_space.py
--rw-r--r--   0        0        0      856 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/space/exception.py
--rw-r--r--   0        0        0     8215 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/space/number_space.py
--rw-r--r--   0        0        0     8456 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/space/recency_space.py
--rw-r--r--   0        0        0     2743 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/space/space.py
--rw-r--r--   0        0        0     1295 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/space/space_field_set.py
--rw-r--r--   0        0        0     4804 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/dsl/space/text_similarity_space.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.380514 superlinked-5.3.0/superlinked/framework/evaluator/__init__.py
--rw-r--r--   0        0        0     1043 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/evaluator/dag_evaluator.py
--rw-r--r--   0        0        0     4807 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/evaluator/online_dag_evaluator.py
--rw-r--r--   0        0        0     2237 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/evaluator/query_dag_evaluator.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/__init__.py
--rw-r--r--   0        0        0      801 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/batched_chunk_input_item.py
--rw-r--r--   0        0        0     7597 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/default_online_node.py
--rw-r--r--   0        0        0     1213 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/evaluation_result.py
--rw-r--r--   0        0        0      768 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/exception.py
--rw-r--r--   0        0        0     6312 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/online_aggregation_node.py
--rw-r--r--   0        0        0     3205 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/online_categorical_similarity_node.py
--rw-r--r--   0        0        0     3457 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/online_chunking_node.py
--rw-r--r--   0        0        0     2247 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/online_comparison_filter_node.py
--rw-r--r--   0        0        0     5138 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/online_concatenation_node.py
--rw-r--r--   0        0        0     2032 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/online_constant_node.py
--rw-r--r--   0        0        0     3283 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/online_custom_node.py
--rw-r--r--   0        0        0     7908 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/online_event_aggregation_node.py
--rw-r--r--   0        0        0     4052 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/online_index_node.py
--rw-r--r--   0        0        0     2351 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/online_named_function_node.py
--rw-r--r--   0        0        0     5089 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/online_node.py
--rw-r--r--   0        0        0     5690 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/online_node_registry.py
--rw-r--r--   0        0        0     3079 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/online_number_embedding_node.py
--rw-r--r--   0        0        0     3189 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/online_number_similarity_node.py
--rw-r--r--   0        0        0     2713 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/online_recency_node.py
--rw-r--r--   0        0        0     3732 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/online_schema_dag.py
--rw-r--r--   0        0        0     3426 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/online_schema_field_node.py
--rw-r--r--   0        0        0     3255 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/online_text_embedding_node.py
--rw-r--r--   0        0        0      794 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/parent_results.py
--rw-r--r--   0        0        0     1322 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/dag/parent_validator.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/source/__init__.py
--rw-r--r--   0        0        0     3486 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/source/in_memory_data_processor.py
--rw-r--r--   0        0        0     1437 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/source/in_memory_object_writer.py
--rw-r--r--   0        0        0     1752 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/online/source/in_memory_source.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/storage/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/storage/in_memory/__init__.py
--rw-r--r--   0        0        0      787 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/storage/in_memory/exception.py
--rw-r--r--   0        0        0     6725 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/storage/in_memory/in_memory_search.py
--rw-r--r--   0        0        0     7121 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/storage/in_memory/in_memory_vdb.py
--rw-r--r--   0        0        0      921 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/storage/in_memory/index_config.py
--rw-r--r--   0        0        0     1305 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/storage/in_memory/json_codec.py
--rw-r--r--   0        0        0     1562 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/framework/storage/in_memory/object_serializer.py
--rw-r--r--   0        0        0        0 2024-05-24 14:18:57.384514 superlinked-5.3.0/superlinked/py.typed
--rw-r--r--   0        0        0     8320 1970-01-01 00:00:00.000000 superlinked-5.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11354 2024-05-27 14:19:00.632236 superlinked-5.4.0/LICENSE
+-rw-r--r--   0        0        0    28655 2024-05-27 14:19:00.632236 superlinked-5.4.0/NOTICE
+-rw-r--r--   0        0        0     6840 2024-05-27 14:19:00.632236 superlinked-5.4.0/PYPI_README.md
+-rw-r--r--   0        0        0     3698 2024-05-27 14:22:13.568568 superlinked-5.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/evaluation/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/evaluation/charts/__init__.py
+-rw-r--r--   0        0        0     5601 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/evaluation/charts/recency_plotter.py
+-rw-r--r--   0        0        0     9028 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/evaluation/vector_sampler.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/calculation/__init__.py
+-rw-r--r--   0        0        0      742 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/calculation/distance_metric.py
+-rw-r--r--   0        0        0     1510 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/calculation/vector_similarity.py
+-rw-r--r--   0        0        0      805 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/const.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/__init__.py
+-rw-r--r--   0        0        0     3644 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/aggregation_node.py
+-rw-r--r--   0        0        0     2509 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/categorical_similarity_node.py
+-rw-r--r--   0        0        0     1520 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/chunking_node.py
+-rw-r--r--   0        0        0     2095 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/comparison_filter_node.py
+-rw-r--r--   0        0        0     2606 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/concatenation_node.py
+-rw-r--r--   0        0        0     1106 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/constant_node.py
+-rw-r--r--   0        0        0     4985 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/context.py
+-rw-r--r--   0        0        0     1854 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/custom_node.py
+-rw-r--r--   0        0        0     5923 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/dag.py
+-rw-r--r--   0        0        0     1338 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/dag_effect.py
+-rw-r--r--   0        0        0     3687 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/event_aggregation_node.py
+-rw-r--r--   0        0        0     1004 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/exception.py
+-rw-r--r--   0        0        0     2043 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/index_node.py
+-rw-r--r--   0        0        0     1428 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/named_function_node.py
+-rw-r--r--   0        0        0     4723 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/node.py
+-rw-r--r--   0        0        0     3083 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/number_embedding_node.py
+-rw-r--r--   0        0        0     1620 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/period_time.py
+-rw-r--r--   0        0        0      897 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/persistence_params.py
+-rw-r--r--   0        0        0     2487 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/recency_node.py
+-rw-r--r--   0        0        0     1128 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/resolved_schema_reference.py
+-rw-r--r--   0        0        0     2019 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/schema_dag.py
+-rw-r--r--   0        0        0     1463 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/schema_field_node.py
+-rw-r--r--   0        0        0     1378 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/schema_object_reference.py
+-rw-r--r--   0        0        0     2250 2024-05-27 14:19:00.680236 superlinked-5.4.0/superlinked/framework/common/dag/text_embedding_node.py
+-rw-r--r--   0        0        0     8107 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/data_types.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/embedding/__init__.py
+-rw-r--r--   0        0        0     5201 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/embedding/categorical_similarity_embedding.py
+-rw-r--r--   0        0        0     5890 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/embedding/chunking_util.py
+-rw-r--r--   0        0        0     1507 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/embedding/custom_embedding.py
+-rw-r--r--   0        0        0     1280 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/embedding/embedding.py
+-rw-r--r--   0        0        0     3772 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/embedding/number_embedding.py
+-rw-r--r--   0        0        0     8046 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/embedding/recency_embedding.py
+-rw-r--r--   0        0        0     2134 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/embedding/sentence_transformer_embedding.py
+-rw-r--r--   0        0        0     1250 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/exception.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/interface/__init__.py
+-rw-r--r--   0        0        0     5851 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/interface/comparison_operand.py
+-rw-r--r--   0        0        0      841 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/interface/comparison_operation_type.py
+-rw-r--r--   0        0        0      808 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/interface/has_aggregation.py
+-rw-r--r--   0        0        0      796 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/interface/has_default_vector.py
+-rw-r--r--   0        0        0      718 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/interface/has_length.py
+-rw-r--r--   0        0        0      836 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/interface/has_multiplier.py
+-rw-r--r--   0        0        0      940 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/interface/weighted.py
+-rw-r--r--   0        0        0     1322 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/observable.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/parser/__init__.py
+-rw-r--r--   0        0        0     5829 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/parser/data_parser.py
+-rw-r--r--   0        0        0     5402 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/parser/dataframe_parser.py
+-rw-r--r--   0        0        0      814 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/parser/exception.py
+-rw-r--r--   0        0        0     4628 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/parser/json_parser.py
+-rw-r--r--   0        0        0     1354 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/parser/parsed_schema.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/__init__.py
+-rw-r--r--   0        0        0     1072 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/event_schema.py
+-rw-r--r--   0        0        0     1964 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/event_schema_object.py
+-rw-r--r--   0        0        0     1014 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/exception.py
+-rw-r--r--   0        0        0      627 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/general_type.py
+-rw-r--r--   0        0        0     1392 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/id_schema_object.py
+-rw-r--r--   0        0        0     1178 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/schema.py
+-rw-r--r--   0        0        0     3189 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/schema_decorator.py
+-rw-r--r--   0        0        0     3228 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/schema_factory.py
+-rw-r--r--   0        0        0     5701 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/schema_object.py
+-rw-r--r--   0        0        0     3170 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/schema_reference.py
+-rw-r--r--   0        0        0      686 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/schema_type.py
+-rw-r--r--   0        0        0     3220 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/schema/schema_validator.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/source/__init__.py
+-rw-r--r--   0        0        0      857 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/source/source.py
+-rw-r--r--   0        0        0      647 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/source/types.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/space/__init__.py
+-rw-r--r--   0        0        0     4492 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/space/aggregation.py
+-rw-r--r--   0        0        0     2055 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/space/normalization.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/__init__.py
+-rw-r--r--   0        0        0      820 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/entity.py
+-rw-r--r--   0        0        0      855 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/entity_data.py
+-rw-r--r--   0        0        0      696 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/entity_id.py
+-rw-r--r--   0        0        0      627 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/exception.py
+-rw-r--r--   0        0        0     1656 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/field.py
+-rw-r--r--   0        0        0     2616 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/field_data.py
+-rw-r--r--   0        0        0      757 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/field_data_type.py
+-rw-r--r--   0        0        0     3514 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/field_encoder.py
+-rw-r--r--   0        0        0     2772 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/field_type_converter.py
+-rw-r--r--   0        0        0      746 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/persistence_type.py
+-rw-r--r--   0        0        0      769 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/result_entity_data.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/search_index_creation/__init__.py
+-rw-r--r--   0        0        0     1242 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py
+-rw-r--r--   0        0        0      671 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/search_index_creation/search_algorithm.py
+-rw-r--r--   0        0        0      692 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py
+-rw-r--r--   0        0        0     2397 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/vdb_connector.py
+-rw-r--r--   0        0        0     1095 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage/vdb_knn_search_params.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage_manager/__init__.py
+-rw-r--r--   0        0        0     5459 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage_manager/admin_fields.py
+-rw-r--r--   0        0        0     5549 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage_manager/entity_builder.py
+-rw-r--r--   0        0        0      720 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage_manager/header.py
+-rw-r--r--   0        0        0     1079 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage_manager/knn_search_params.py
+-rw-r--r--   0        0        0      932 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage_manager/search_result_item.py
+-rw-r--r--   0        0        0    16654 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage_manager/storage_manager.py
+-rw-r--r--   0        0        0     1533 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/storage_manager/storage_naming.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/util/__init__.py
+-rw-r--r--   0        0        0      787 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/util/collection_util.py
+-rw-r--r--   0        0        0     2074 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/util/dot_separated_path_util.py
+-rw-r--r--   0        0        0     1777 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/util/generic_class_util.py
+-rw-r--r--   0        0        0      707 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/util/immutable_model.py
+-rw-r--r--   0        0        0     1058 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/util/named_function_evaluator.py
+-rw-r--r--   0        0        0     1642 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/util/string_util.py
+-rw-r--r--   0        0        0      907 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/util/time_util.py
+-rw-r--r--   0        0        0     4383 2024-05-27 14:19:00.684236 superlinked-5.4.0/superlinked/framework/common/util/type_validator.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/compiler/__init__.py
+-rw-r--r--   0        0        0     2399 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/compiler/online_schema_dag_compiler.py
+-rw-r--r--   0        0        0      108 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/__init__.py
+-rw-r--r--   0        0        0      221 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/executor/__init__.py
+-rw-r--r--   0        0        0      719 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/executor/exception.py
+-rw-r--r--   0        0        0     3836 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/executor/executor.py
+-rw-r--r--   0        0        0      124 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/executor/in_memory/__init__.py
+-rw-r--r--   0        0        0     7115 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py
+-rw-r--r--   0        0        0      119 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/executor/query/__init__.py
+-rw-r--r--   0        0        0     6804 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/executor/query/query_executor.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/executor/rest/__init__.py
+-rw-r--r--   0        0        0     1540 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/executor/rest/rest_configuration.py
+-rw-r--r--   0        0        0      818 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/executor/rest/rest_descriptor.py
+-rw-r--r--   0        0        0     4834 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/executor/rest/rest_executor.py
+-rw-r--r--   0        0        0     3236 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/executor/rest/rest_handler.py
+-rw-r--r--   0        0        0      176 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/index/__init__.py
+-rw-r--r--   0        0        0     1904 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/index/effect.py
+-rw-r--r--   0        0        0    10985 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/index/index.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/index/util/__init__.py
+-rw-r--r--   0        0        0     1516 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/index/util/aggregation_effect_group.py
+-rw-r--r--   0        0        0     2448 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/index/util/aggregation_node_util.py
+-rw-r--r--   0        0        0     6203 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py
+-rw-r--r--   0        0        0     2557 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py
+-rw-r--r--   0        0        0     3673 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/index/util/event_aggregation_node_util.py
+-rw-r--r--   0        0        0      192 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/__init__.py
+-rw-r--r--   0        0        0     1183 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/param.py
+-rw-r--r--   0        0        0     3798 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/param_evaluator.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/predicate/__init__.py
+-rw-r--r--   0        0        0      756 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/predicate/binary_op.py
+-rw-r--r--   0        0        0     1521 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/predicate/binary_predicate.py
+-rw-r--r--   0        0        0      924 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/predicate/evaluated_binary_predicate.py
+-rw-r--r--   0        0        0     1128 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/predicate/query_predicate.py
+-rw-r--r--   0        0        0    13227 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/query.py
+-rw-r--r--   0        0        0     6223 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/query_filters.py
+-rw-r--r--   0        0        0     6842 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/query_vector_factory.py
+-rw-r--r--   0        0        0     3329 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/query_weighting.py
+-rw-r--r--   0        0        0     2613 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/query/result.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/registry/__init__.py
+-rw-r--r--   0        0        0      636 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/registry/exception.py
+-rw-r--r--   0        0        0     1330 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/registry/superlinked_registry.py
+-rw-r--r--   0        0        0      214 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/source/__init__.py
+-rw-r--r--   0        0        0     2225 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/source/data_loader_source.py
+-rw-r--r--   0        0        0     2773 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/source/in_memory_source.py
+-rw-r--r--   0        0        0     1987 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/source/rest_source.py
+-rw-r--r--   0        0        0     1144 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/source/source.py
+-rw-r--r--   0        0        0      183 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/space/__init__.py
+-rw-r--r--   0        0        0     7479 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/space/categorical_similarity_space.py
+-rw-r--r--   0        0        0     5509 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/space/custom_space.py
+-rw-r--r--   0        0        0      856 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/space/exception.py
+-rw-r--r--   0        0        0     7702 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/space/number_space.py
+-rw-r--r--   0        0        0     8456 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/space/recency_space.py
+-rw-r--r--   0        0        0     2743 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/space/space.py
+-rw-r--r--   0        0        0     1295 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/space/space_field_set.py
+-rw-r--r--   0        0        0     4804 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/dsl/space/text_similarity_space.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/evaluator/__init__.py
+-rw-r--r--   0        0        0     1043 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/evaluator/dag_evaluator.py
+-rw-r--r--   0        0        0     4807 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/evaluator/online_dag_evaluator.py
+-rw-r--r--   0        0        0     2237 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/evaluator/query_dag_evaluator.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/__init__.py
+-rw-r--r--   0        0        0      801 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/batched_chunk_input_item.py
+-rw-r--r--   0        0        0     7597 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/default_online_node.py
+-rw-r--r--   0        0        0     1213 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/evaluation_result.py
+-rw-r--r--   0        0        0      768 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/exception.py
+-rw-r--r--   0        0        0     6312 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_aggregation_node.py
+-rw-r--r--   0        0        0     3206 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_categorical_similarity_node.py
+-rw-r--r--   0        0        0     3457 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_chunking_node.py
+-rw-r--r--   0        0        0     2247 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_comparison_filter_node.py
+-rw-r--r--   0        0        0     5138 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_concatenation_node.py
+-rw-r--r--   0        0        0     2032 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_constant_node.py
+-rw-r--r--   0        0        0     3283 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_custom_node.py
+-rw-r--r--   0        0        0     7908 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_event_aggregation_node.py
+-rw-r--r--   0        0        0     4052 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_index_node.py
+-rw-r--r--   0        0        0     2351 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_named_function_node.py
+-rw-r--r--   0        0        0     5086 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_node.py
+-rw-r--r--   0        0        0     5547 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_node_registry.py
+-rw-r--r--   0        0        0     3704 2024-05-27 14:19:00.688236 superlinked-5.4.0/superlinked/framework/online/dag/online_number_embedding_node.py
+-rw-r--r--   0        0        0     2713 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/online/dag/online_recency_node.py
+-rw-r--r--   0        0        0     3732 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/online/dag/online_schema_dag.py
+-rw-r--r--   0        0        0     3426 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/online/dag/online_schema_field_node.py
+-rw-r--r--   0        0        0     3256 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/online/dag/online_text_embedding_node.py
+-rw-r--r--   0        0        0      794 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/online/dag/parent_results.py
+-rw-r--r--   0        0        0     1322 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/online/dag/parent_validator.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/online/source/__init__.py
+-rw-r--r--   0        0        0     3486 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/online/source/in_memory_data_processor.py
+-rw-r--r--   0        0        0     1437 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/online/source/in_memory_object_writer.py
+-rw-r--r--   0        0        0     1752 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/online/source/in_memory_source.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/storage/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/storage/in_memory/__init__.py
+-rw-r--r--   0        0        0      787 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/storage/in_memory/exception.py
+-rw-r--r--   0        0        0     6725 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/storage/in_memory/in_memory_search.py
+-rw-r--r--   0        0        0     7121 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/storage/in_memory/in_memory_vdb.py
+-rw-r--r--   0        0        0      921 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/storage/in_memory/index_config.py
+-rw-r--r--   0        0        0     1305 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/storage/in_memory/json_codec.py
+-rw-r--r--   0        0        0     1562 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/framework/storage/in_memory/object_serializer.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:19:00.692236 superlinked-5.4.0/superlinked/py.typed
+-rw-r--r--   0        0        0     8320 1970-01-01 00:00:00.000000 superlinked-5.4.0/PKG-INFO
```

### Comparing `superlinked-5.3.0/LICENSE` & `superlinked-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/NOTICE` & `superlinked-5.4.0/NOTICE`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/PYPI_README.md` & `superlinked-5.4.0/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/pyproject.toml` & `superlinked-5.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "superlinked"
-version = "5.3.0"  # The version will be dynamically updated
+version = "5.4.0"  # The version will be dynamically updated
 description = "The Superlinked vector computing library"
 authors = ["Superlinked Release <release@superlinked.com>"]
 readme = "PYPI_README.md"
 license = "Apache-2.0"
 include = ["NOTICE"]
 
 [tool.poetry.dependencies]
```

### Comparing `superlinked-5.3.0/superlinked/evaluation/charts/recency_plotter.py` & `superlinked-5.4.0/superlinked/evaluation/charts/recency_plotter.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/evaluation/vector_sampler.py` & `superlinked-5.4.0/superlinked/evaluation/vector_sampler.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/calculation/distance_metric.py` & `superlinked-5.4.0/superlinked/framework/common/calculation/distance_metric.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/calculation/vector_similarity.py` & `superlinked-5.4.0/superlinked/framework/common/calculation/vector_similarity.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/const.py` & `superlinked-5.4.0/superlinked/framework/common/const.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/dag/aggregation_node.py` & `superlinked-5.4.0/superlinked/framework/common/dag/aggregation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/dag/categorical_similarity_node.py` & `superlinked-5.4.0/superlinked/framework/common/dag/categorical_similarity_node.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,23 +19,26 @@
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.embedding.categorical_similarity_embedding import (
     CategoricalSimilarityEmbedding,
     CategoricalSimilarityParams,
 )
 from superlinked.framework.common.interface.has_aggregation import HasAggregation
+from superlinked.framework.common.interface.has_default_vector import HasDefaultVector
 from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.common.space.aggregation import (
     Aggregation,
     VectorAggregation,
 )
 from superlinked.framework.common.space.normalization import L2Norm
 
 
-class CategoricalSimilarityNode(Node[Vector], HasLength, HasAggregation):
+class CategoricalSimilarityNode(
+    Node[Vector], HasLength, HasAggregation, HasDefaultVector
+):
     def __init__(
         self,
         parent: Node[str],
         categorical_similarity_param: CategoricalSimilarityParams,
     ) -> None:
         super().__init__(Vector, [parent])
         self.__aggregation = VectorAggregation(L2Norm())
@@ -49,14 +52,19 @@
         return self.embedding.length
 
     @property
     @override
     def aggregation(self) -> Aggregation:
         return self.__aggregation
 
+    @property
+    @override
+    def default_vector(self) -> Vector:
+        return Vector([0] * self.length)
+
     @override
     def _get_node_id_parameters(self) -> dict[str, Any]:
         return {
             "categories": self.embedding.categories,
             "negative_filter": self.embedding.negative_filter,
             "uncategorized_as_category": self.embedding.uncategorized_as_category,
             "aggregation": self.__aggregation,
```

### Comparing `superlinked-5.3.0/superlinked/framework/common/dag/chunking_node.py` & `superlinked-5.4.0/superlinked/framework/common/dag/chunking_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/dag/comparison_filter_node.py` & `superlinked-5.4.0/superlinked/framework/common/dag/comparison_filter_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/dag/concatenation_node.py` & `superlinked-5.4.0/superlinked/framework/common/dag/concatenation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/dag/constant_node.py` & `superlinked-5.4.0/superlinked/framework/common/dag/constant_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/dag/context.py` & `superlinked-5.4.0/superlinked/framework/common/dag/context.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/dag/custom_node.py` & `superlinked-5.4.0/superlinked/framework/common/dag/custom_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/dag/dag.py` & `superlinked-5.4.0/superlinked/framework/common/dag/dag.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/dag/dag_effect.py` & `superlinked-5.4.0/superlinked/framework/common/dag/dag_effect.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/dag/event_aggregation_node.py` & `superlinked-5.4.0/superlinked/framework/common/dag/event_aggregation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/dag/exception.py` & `superlinked-5.4.0/superlinked/framework/common/dag/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/dag/index_node.py` & `superlinked-5.4.0/superlinked/framework/common/dag/index_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/dag/named_function_node.py` & `superlinked-5.4.0/superlinked/framework/common/dag/named_function_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/dag/node.py` & `superlinked-5.4.0/superlinked/framework/common/dag/node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/dag/number_embedding_node.py` & `superlinked-5.4.0/superlinked/framework/common/dag/number_embedding_node.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,52 +21,72 @@
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.embedding.number_embedding import (
     Mode,
     NumberEmbedding,
 )
 from superlinked.framework.common.interface.has_aggregation import HasAggregation
+from superlinked.framework.common.interface.has_default_vector import HasDefaultVector
 from superlinked.framework.common.interface.has_length import HasLength
-from superlinked.framework.common.space.aggregation import Aggregation, VectorAvg
+from superlinked.framework.common.space.aggregation import (
+    Aggregation,
+    InputAggregation,
+    InputAggregationMode,
+)
 from superlinked.framework.common.space.normalization import NoNorm
 
 
 @dataclass
 class NumberEmbeddingParams:
     min_value: float
     max_value: float
     mode: Mode
     negative_filter: float
 
 
-class NumberEmbeddingNode(Node[Vector], HasLength, HasAggregation):
+class NumberEmbeddingNode(Node[Vector], HasLength, HasAggregation, HasDefaultVector):
     def __init__(
         self,
         parent: Node[float | int],
         embedding_params: NumberEmbeddingParams,
+        aggregation_mode: InputAggregationMode,
     ) -> None:
         super().__init__(Vector, [parent])
-        self.__aggregation = VectorAvg(NoNorm())
+        normalization = NoNorm()
         self.embedding = NumberEmbedding(
             embedding_params.min_value,
             embedding_params.max_value,
             embedding_params.mode,
             embedding_params.negative_filter,
-            self.__aggregation.normalization,
+            normalization,
+        )
+        self.__aggregation: InputAggregation = InputAggregation.from_aggregation_mode(
+            aggregation_mode, normalization, self.embedding
         )
+        self.mode = embedding_params.mode
+        self.__default_vector = {
+            Mode.SIMILAR: [0.0, 0.0, 0.0],
+            Mode.MINIMUM: [0.0, 1.0, 1.0],
+            Mode.MAXIMUM: [1.0, 0.0, 1.0],
+        }[self.mode]
 
     @property
     def length(self) -> int:
         return self.embedding.length
 
     @property
     @override
     def aggregation(self) -> Aggregation:
         return self.__aggregation
 
+    @property
+    @override
+    def default_vector(self) -> Vector:
+        return Vector(self.__default_vector)
+
     @override
     def _get_node_id_parameters(self) -> dict[str, Any]:
         return {
             "min_value": self.embedding._min_value,
             "max_value": self.embedding._max_value,
             "mode": self.embedding._mode,
             "negative_filter": self.embedding._negative_filter,
```

### Comparing `superlinked-5.3.0/superlinked/framework/common/dag/number_similarity_node.py` & `superlinked-5.4.0/superlinked/framework/common/dag/recency_node.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,51 +8,53 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from datetime import timedelta
 from typing import Any
 
 from typing_extensions import override
 
 from superlinked.framework.common.dag.node import Node
+from superlinked.framework.common.dag.period_time import PeriodTime
 from superlinked.framework.common.data_types import Vector
-from superlinked.framework.common.embedding.number_similarity_embedding import (
-    NumberSimilarityEmbedding,
+from superlinked.framework.common.embedding.recency_embedding import (
+    RecencyEmbedding,
+    calculate_recency_normalization,
 )
 from superlinked.framework.common.interface.has_aggregation import HasAggregation
 from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.common.space.aggregation import (
     Aggregation,
+    InputAggregation,
     InputAggregationMode,
-    get_input_aggregation,
 )
-from superlinked.framework.common.space.normalization import NoNorm
 
 
-class NumberSimilarityNode(Node[Vector], HasLength, HasAggregation):
+class RecencyNode(Node[Vector], HasLength, HasAggregation):
     def __init__(
         self,
-        parent: Node[float | int],
-        min_value: float,
-        max_value: float,
-        negative_filter: float,
+        parent: Node[int],
+        time_period_hour_offset: timedelta,
+        period_time_list: list[PeriodTime],
         aggregation_mode: InputAggregationMode,
+        negative_filter: float,
     ) -> None:
         super().__init__(Vector, [parent])
-        normalization = NoNorm()
-        self.embedding = NumberSimilarityEmbedding(
-            min_value,
-            max_value,
-            negative_filter,
+        normalization = calculate_recency_normalization(period_time_list)
+        self.embedding = RecencyEmbedding(
+            period_time_list,
             normalization,
+            time_period_hour_offset,
+            negative_filter,
         )
-        self.__aggregation = get_input_aggregation(
+        self.__aggregation: InputAggregation = InputAggregation.from_aggregation_mode(
             aggregation_mode, normalization, self.embedding
         )
 
     @property
     def length(self) -> int:
         return self.embedding.length
 
@@ -60,12 +62,11 @@
     @override
     def aggregation(self) -> Aggregation:
         return self.__aggregation
 
     @override
     def _get_node_id_parameters(self) -> dict[str, Any]:
         return {
-            "min_value": self.embedding._min_value,
-            "max_value": self.embedding._max_value,
-            "negative_filter": self.embedding._negative_filter,
+            "period_time_list": self.embedding.period_time_list,
+            "negative_filter": self.embedding.negative_filter,
             "aggregation": self.__aggregation,
         }
```

### Comparing `superlinked-5.3.0/superlinked/framework/common/dag/period_time.py` & `superlinked-5.4.0/superlinked/framework/common/dag/period_time.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/dag/persistence_params.py` & `superlinked-5.4.0/superlinked/framework/common/dag/persistence_params.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/dag/resolved_schema_reference.py` & `superlinked-5.4.0/superlinked/framework/common/dag/resolved_schema_reference.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/dag/schema_dag.py` & `superlinked-5.4.0/superlinked/framework/common/dag/schema_dag.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/dag/schema_field_node.py` & `superlinked-5.4.0/superlinked/framework/common/dag/schema_field_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/dag/schema_object_reference.py` & `superlinked-5.4.0/superlinked/framework/common/dag/schema_object_reference.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/dag/text_embedding_node.py` & `superlinked-5.4.0/superlinked/framework/common/dag/text_embedding_node.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,23 +18,24 @@
 
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.embedding.sentence_transformer_embedding import (
     SentenceTransformerEmbedding,
 )
 from superlinked.framework.common.interface.has_aggregation import HasAggregation
+from superlinked.framework.common.interface.has_default_vector import HasDefaultVector
 from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.common.space.aggregation import (
     Aggregation,
     VectorAggregation,
 )
 from superlinked.framework.common.space.normalization import L2Norm
 
 
-class TextEmbeddingNode(Node[Vector], HasLength, HasAggregation):
+class TextEmbeddingNode(Node[Vector], HasLength, HasAggregation, HasDefaultVector):
     def __init__(
         self,
         parent: Node[str],
         model_name: str,
     ) -> None:
         super().__init__(Vector, [parent])
         self.model_name = model_name
@@ -51,10 +52,15 @@
         return self.embedding.length
 
     @property
     @override
     def aggregation(self) -> Aggregation:
         return self.__aggregation
 
+    @property
+    @override
+    def default_vector(self) -> Vector:
+        return Vector([0] * self.length)
+
     @override
     def _get_node_id_parameters(self) -> dict[str, Any]:
         return {"model_name": self.model_name, "aggregation": self.__aggregation}
```

### Comparing `superlinked-5.3.0/superlinked/framework/common/data_types.py` & `superlinked-5.4.0/superlinked/framework/common/data_types.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/embedding/categorical_similarity_embedding.py` & `superlinked-5.4.0/superlinked/framework/common/embedding/categorical_similarity_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/embedding/chunking_util.py` & `superlinked-5.4.0/superlinked/framework/common/embedding/chunking_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/embedding/custom_embedding.py` & `superlinked-5.4.0/superlinked/framework/common/embedding/custom_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/embedding/embedding.py` & `superlinked-5.4.0/superlinked/framework/common/embedding/embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/embedding/number_embedding.py` & `superlinked-5.4.0/superlinked/framework/common/embedding/number_embedding.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import math
 from enum import Enum
 
 import numpy as np
 from typing_extensions import override
 
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.data_types import Vector
@@ -35,55 +36,76 @@
         self,
         min_value: float,
         max_value: float,
         mode: Mode,
         negative_filter: float,
         normalization: Normalization,
     ) -> None:
-        self.__length = 1
+        self.__circle_size_in_rad = math.pi / 2
+        self.__length = 3
         self._min_value = min_value
         self._max_value = max_value
         self._mode = mode
-        self._negative_filter = float(negative_filter)
+        self._negative_filter = negative_filter
         self._normalization = normalization
 
     @override
     def embed(
         self,
         input_: float,
         context: ExecutionContext,  # pylint: disable=unused-argument
     ) -> Vector:
+        if (
+            input_ < self._min_value
+            and self._mode
+            in {
+                Mode.MAXIMUM,
+                Mode.SIMILAR,
+            }
+        ) or (
+            input_ > self._max_value
+            and self._mode
+            in {
+                Mode.MINIMUM,
+                Mode.SIMILAR,
+            }
+        ):
+            return Vector([0.0, 0.0, self._negative_filter], {2})
         constrained_input: float = min(max(self._min_value, input_), self._max_value)
-        transformed_number: float = (constrained_input - self._min_value) / (
+        normalized_input = (constrained_input - self._min_value) / (
             self._max_value - self._min_value
         )
-        if self._mode == Mode.MINIMUM:
-            transformed_number = 1 - transformed_number
-        if transformed_number <= 0:
-            transformed_number = self._negative_filter
-        vector_input = np.array([transformed_number])
-        vector = Vector(vector_input)
-        return vector.normalize(self._normalization.norm(vector_input))
+        angle_in_radians = normalized_input * self.__circle_size_in_rad
+        vector_input = np.array(
+            [math.sin(angle_in_radians), math.cos(angle_in_radians)]
+        )
+        vector = Vector(np.append(vector_input, [0.0]), {2}).normalize(
+            self._normalization.norm(vector_input)
+        )
+        return vector
 
     @override
     def inverse_embed(
         self,
         vector: Vector,
         context: ExecutionContext,  # pylint: disable=unused-argument
     ) -> float:
         """
         This function might seem complex,
         but it essentially performs the inverse operation of the embed function.
         """
         denormalized = self._normalization.denormalize(vector)
-        transformed_number = denormalized.value[0]
-        if transformed_number == self._negative_filter:
-            transformed_number = -1
-        if self._mode == Mode.MINIMUM:
-            transformed_number = 1 - transformed_number
+        if vector.value[2] == self._negative_filter:
+            if self._mode == Mode.MAXIMUM:
+                return self._min_value - 1
+            # INFO: for similar it doesn't matter, which direction is it out of bounds
+            return self._max_value + 1
+
+        angle_in_radians = math.atan2(denormalized.value[0], denormalized.value[1])
+        transformed_number = angle_in_radians / self.__circle_size_in_rad
         transformed_number = (
             transformed_number * (self._max_value - self._min_value) + self._min_value
         )
         return transformed_number
 
     @property
     def length(self) -> int:
```

### Comparing `superlinked-5.3.0/superlinked/framework/common/embedding/number_similarity_embedding.py` & `superlinked-5.4.0/superlinked/framework/online/dag/online_named_function_node.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,59 +8,60 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import math
+from __future__ import annotations
+
+from typing import cast
 
-import numpy as np
 from typing_extensions import override
 
 from superlinked.framework.common.dag.context import ExecutionContext
-from superlinked.framework.common.data_types import Vector
-from superlinked.framework.common.embedding.embedding import Embedding
-from superlinked.framework.common.interface.has_length import HasLength
-from superlinked.framework.common.space.normalization import Normalization
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
 
 
-class NumberSimilarityEmbedding(Embedding[float], HasLength):
+class OnlineNamedFunctionNode(OnlineNode[NamedFunctionNode[NDT], NDT]):
     def __init__(
         self,
-        min_value: float,
-        max_value: float,
-        negative_filter: float,
-        normalization: Normalization,
+        node: NamedFunctionNode,
+        parents: list[OnlineNode],
+        storage_manager: StorageManager,
     ) -> None:
-        self.__length = 3
-        self.__circle_size_in_rad = math.pi / 2
-        self._min_value = min_value
-        self._max_value = max_value
-        self._negative_filter = negative_filter
-        self._normalization = normalization
+        super().__init__(
+            node,
+            parents,
+            storage_manager,
+            ParentValidationType.NO_PARENTS,
+        )
 
     @override
-    def embed(self, input_: float, context: ExecutionContext) -> Vector:
-        if input_ < self._min_value or input_ > self._max_value:
-            return Vector([0.0, 0.0, self._negative_filter])
-
-        constrained_input: float = min(max(self._min_value, input_), self._max_value)
-        normalized_input = (constrained_input - self._min_value) / (
-            self._max_value - self._min_value
-        )
-        angle_in_radians = normalized_input * self.__circle_size_in_rad
-        vector_input = np.array(
-            [
-                math.sin(angle_in_radians),
-                math.cos(angle_in_radians),
-            ]
-        )
-        vector = Vector(vector_input).normalize(self._normalization.norm(vector_input))
-        vector = vector.concatenate(
-            Vector([1.0 if context.is_query_context() else 0.0])
+    def evaluate_self(
+        self,
+        parsed_schemas: list[ParsedSchema],
+        context: ExecutionContext,
+    ) -> list[EvaluationResult[NDT]]:
+        result = EvaluationResult(
+            self._get_single_evaluation_result(self._evaluate_single(context))
         )
-        return vector
+        return [result for _ in parsed_schemas]
 
-    @property
-    def length(self) -> int:
-        return self.__length
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

### Comparing `superlinked-5.3.0/superlinked/framework/common/embedding/recency_embedding.py` & `superlinked-5.4.0/superlinked/framework/common/embedding/recency_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/embedding/sentence_transformer_embedding.py` & `superlinked-5.4.0/superlinked/framework/common/embedding/sentence_transformer_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/exception.py` & `superlinked-5.4.0/superlinked/framework/common/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/interface/comparison_operand.py` & `superlinked-5.4.0/superlinked/framework/common/interface/comparison_operand.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/interface/comparison_operation_type.py` & `superlinked-5.4.0/superlinked/framework/common/interface/comparison_operation_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/interface/has_aggregation.py` & `superlinked-5.4.0/superlinked/framework/common/interface/has_aggregation.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/interface/has_length.py` & `superlinked-5.4.0/superlinked/framework/common/interface/has_length.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/interface/has_multiplier.py` & `superlinked-5.4.0/superlinked/framework/common/interface/has_multiplier.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/interface/weighted.py` & `superlinked-5.4.0/superlinked/framework/common/interface/weighted.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/observable.py` & `superlinked-5.4.0/superlinked/framework/common/observable.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/parser/data_parser.py` & `superlinked-5.4.0/superlinked/framework/common/parser/data_parser.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/parser/dataframe_parser.py` & `superlinked-5.4.0/superlinked/framework/common/parser/dataframe_parser.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/parser/exception.py` & `superlinked-5.4.0/superlinked/framework/common/parser/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/parser/json_parser.py` & `superlinked-5.4.0/superlinked/framework/common/parser/json_parser.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/parser/parsed_schema.py` & `superlinked-5.4.0/superlinked/framework/common/parser/parsed_schema.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/schema/event_schema.py` & `superlinked-5.4.0/superlinked/framework/common/schema/event_schema.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/schema/event_schema_object.py` & `superlinked-5.4.0/superlinked/framework/common/schema/event_schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/schema/exception.py` & `superlinked-5.4.0/superlinked/framework/common/schema/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/schema/general_type.py` & `superlinked-5.4.0/superlinked/framework/common/schema/general_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/schema/id_schema_object.py` & `superlinked-5.4.0/superlinked/framework/common/schema/id_schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/schema/schema.py` & `superlinked-5.4.0/superlinked/framework/common/schema/schema.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/schema/schema_decorator.py` & `superlinked-5.4.0/superlinked/framework/common/schema/schema_decorator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/schema/schema_factory.py` & `superlinked-5.4.0/superlinked/framework/common/schema/schema_factory.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/schema/schema_object.py` & `superlinked-5.4.0/superlinked/framework/common/schema/schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/schema/schema_reference.py` & `superlinked-5.4.0/superlinked/framework/common/schema/schema_reference.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/schema/schema_type.py` & `superlinked-5.4.0/superlinked/framework/common/schema/schema_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/schema/schema_validator.py` & `superlinked-5.4.0/superlinked/framework/common/schema/schema_validator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/source/source.py` & `superlinked-5.4.0/superlinked/framework/common/source/source.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/source/types.py` & `superlinked-5.4.0/superlinked/framework/common/source/types.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/space/aggregation.py` & `superlinked-5.4.0/superlinked/framework/common/space/aggregation.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from __future__ import annotations
+
 from abc import abstractmethod
 from enum import Enum
 from functools import reduce
 from typing import Any, Generic, Mapping
 
 from beartype.typing import Sequence
 from typing_extensions import override
@@ -93,14 +95,25 @@
         items = (
             {k: str(v) for k, v in self.__dict__.items() if k != "embedding"}
             if self.__dict__
             else ""
         )
         return f"{self.__class__.__name__}({items})"
 
+    @staticmethod
+    def from_aggregation_mode(
+        aggregation_mode: InputAggregationMode,
+        normalization: Normalization,
+        embedding: Embedding,
+    ) -> InputAggregation[EIT]:
+        agg_class = INPUT_TYPE_BY_AGG_MODE.get(aggregation_mode)
+        if agg_class is None:
+            raise ValueError(f"Unknown aggregation mode: {aggregation_mode}")
+        return agg_class(normalization, embedding)
+
 
 class InputAvg(InputAggregation):
     @override
     def _aggregate_inputs(self, inputs: Sequence[float]) -> float:
         return sum(inputs) / len(inputs)
 
 
@@ -117,18 +130,7 @@
 
 
 INPUT_TYPE_BY_AGG_MODE: Mapping[InputAggregationMode, type[InputAggregation]] = {
     InputAggregationMode.INPUT_AVERAGE: InputAvg,
     InputAggregationMode.INPUT_MINIMUM: InputMin,
     InputAggregationMode.INPUT_MAXIMUM: InputMax,
 }
-
-
-def get_input_aggregation(
-    aggregation_mode: InputAggregationMode,
-    normalization: Normalization,
-    embedding: Embedding,
-) -> InputAggregation:
-    agg_class = INPUT_TYPE_BY_AGG_MODE.get(aggregation_mode)
-    if agg_class is None:
-        raise ValueError(f"Unknown aggregation mode: {aggregation_mode}")
-    return agg_class(normalization, embedding)
```

### Comparing `superlinked-5.3.0/superlinked/framework/common/space/normalization.py` & `superlinked-5.4.0/superlinked/framework/common/space/normalization.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/storage/entity.py` & `superlinked-5.4.0/superlinked/framework/common/storage/entity.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/storage/entity_data.py` & `superlinked-5.4.0/superlinked/framework/common/storage/entity_data.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/storage/entity_id.py` & `superlinked-5.4.0/superlinked/framework/common/storage/entity_id.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/storage/exception.py` & `superlinked-5.4.0/superlinked/framework/common/storage/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/storage/field.py` & `superlinked-5.4.0/superlinked/framework/common/storage/field.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/storage/field_data.py` & `superlinked-5.4.0/superlinked/framework/common/storage/field_data.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/storage/field_data_type.py` & `superlinked-5.4.0/superlinked/framework/common/storage/field_data_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/storage/field_encoder.py` & `superlinked-5.4.0/superlinked/framework/common/storage/field_encoder.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/storage/field_type_converter.py` & `superlinked-5.4.0/superlinked/framework/common/storage/field_type_converter.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/storage/persistence_type.py` & `superlinked-5.4.0/superlinked/framework/common/storage/persistence_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/storage/result_entity_data.py` & `superlinked-5.4.0/superlinked/framework/common/storage/result_entity_data.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py` & `superlinked-5.4.0/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/storage/search_index_creation/search_algorithm.py` & `superlinked-5.4.0/superlinked/framework/common/storage/search_index_creation/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py` & `superlinked-5.4.0/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/storage/vdb_connector.py` & `superlinked-5.4.0/superlinked/framework/common/storage/vdb_connector.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/storage/vdb_knn_search_params.py` & `superlinked-5.4.0/superlinked/framework/common/storage/vdb_knn_search_params.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/storage_manager/admin_fields.py` & `superlinked-5.4.0/superlinked/framework/common/storage_manager/admin_fields.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/storage_manager/entity_builder.py` & `superlinked-5.4.0/superlinked/framework/common/storage_manager/entity_builder.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/storage_manager/header.py` & `superlinked-5.4.0/superlinked/framework/common/storage_manager/header.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/storage_manager/knn_search_params.py` & `superlinked-5.4.0/superlinked/framework/common/storage_manager/knn_search_params.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/storage_manager/search_result_item.py` & `superlinked-5.4.0/superlinked/framework/common/storage_manager/search_result_item.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/storage_manager/storage_manager.py` & `superlinked-5.4.0/superlinked/framework/common/storage_manager/storage_manager.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/storage_manager/storage_naming.py` & `superlinked-5.4.0/superlinked/framework/common/storage_manager/storage_naming.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/util/collection_util.py` & `superlinked-5.4.0/superlinked/framework/common/util/collection_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/util/dot_separated_path_util.py` & `superlinked-5.4.0/superlinked/framework/common/util/dot_separated_path_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/util/generic_class_util.py` & `superlinked-5.4.0/superlinked/framework/common/util/generic_class_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/util/immutable_model.py` & `superlinked-5.4.0/superlinked/framework/common/util/immutable_model.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/util/named_function_evaluator.py` & `superlinked-5.4.0/superlinked/framework/common/util/named_function_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/util/string_util.py` & `superlinked-5.4.0/superlinked/framework/common/util/string_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/util/time_util.py` & `superlinked-5.4.0/superlinked/framework/common/util/time_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/common/util/type_validator.py` & `superlinked-5.4.0/superlinked/framework/common/util/type_validator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/compiler/online_schema_dag_compiler.py` & `superlinked-5.4.0/superlinked/framework/compiler/online_schema_dag_compiler.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/executor/exception.py` & `superlinked-5.4.0/superlinked/framework/dsl/executor/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/executor/executor.py` & `superlinked-5.4.0/superlinked/framework/dsl/executor/executor.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py` & `superlinked-5.4.0/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/executor/query/query_executor.py` & `superlinked-5.4.0/superlinked/framework/dsl/executor/query/query_executor.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/executor/rest/rest_configuration.py` & `superlinked-5.4.0/superlinked/framework/dsl/executor/rest/rest_configuration.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/executor/rest/rest_descriptor.py` & `superlinked-5.4.0/superlinked/framework/dsl/executor/rest/rest_descriptor.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/executor/rest/rest_executor.py` & `superlinked-5.4.0/superlinked/framework/dsl/executor/rest/rest_executor.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/executor/rest/rest_handler.py` & `superlinked-5.4.0/superlinked/framework/dsl/executor/rest/rest_handler.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/index/effect.py` & `superlinked-5.4.0/superlinked/framework/dsl/index/effect.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/index/index.py` & `superlinked-5.4.0/superlinked/framework/dsl/index/index.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/index/util/aggregation_effect_group.py` & `superlinked-5.4.0/superlinked/framework/dsl/index/util/aggregation_effect_group.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/index/util/aggregation_node_util.py` & `superlinked-5.4.0/superlinked/framework/dsl/index/util/aggregation_node_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py` & `superlinked-5.4.0/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py` & `superlinked-5.4.0/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/index/util/event_aggregation_node_util.py` & `superlinked-5.4.0/superlinked/framework/dsl/index/util/event_aggregation_node_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/query/param.py` & `superlinked-5.4.0/superlinked/framework/dsl/query/param.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/query/param_evaluator.py` & `superlinked-5.4.0/superlinked/framework/dsl/query/param_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/query/predicate/binary_op.py` & `superlinked-5.4.0/superlinked/framework/dsl/query/predicate/binary_op.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/query/predicate/binary_predicate.py` & `superlinked-5.4.0/superlinked/framework/dsl/query/predicate/binary_predicate.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/query/predicate/evaluated_binary_predicate.py` & `superlinked-5.4.0/superlinked/framework/dsl/query/predicate/evaluated_binary_predicate.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/query/predicate/query_predicate.py` & `superlinked-5.4.0/superlinked/framework/dsl/query/predicate/query_predicate.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/query/query.py` & `superlinked-5.4.0/superlinked/framework/dsl/query/query.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/query/query_filters.py` & `superlinked-5.4.0/superlinked/framework/dsl/query/query_filters.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/query/query_vector_factory.py` & `superlinked-5.4.0/superlinked/framework/dsl/query/query_vector_factory.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/query/query_weighting.py` & `superlinked-5.4.0/superlinked/framework/dsl/query/query_weighting.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/query/result.py` & `superlinked-5.4.0/superlinked/framework/dsl/query/result.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/registry/exception.py` & `superlinked-5.4.0/superlinked/framework/dsl/registry/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/registry/superlinked_registry.py` & `superlinked-5.4.0/superlinked/framework/dsl/registry/superlinked_registry.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/source/data_loader_source.py` & `superlinked-5.4.0/superlinked/framework/dsl/source/data_loader_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/source/in_memory_source.py` & `superlinked-5.4.0/superlinked/framework/dsl/source/in_memory_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/source/rest_source.py` & `superlinked-5.4.0/superlinked/framework/dsl/source/rest_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/source/source.py` & `superlinked-5.4.0/superlinked/framework/dsl/source/source.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/space/categorical_similarity_space.py` & `superlinked-5.4.0/superlinked/framework/dsl/space/categorical_similarity_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/space/custom_space.py` & `superlinked-5.4.0/superlinked/framework/dsl/space/custom_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/space/exception.py` & `superlinked-5.4.0/superlinked/framework/dsl/space/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/space/number_space.py` & `superlinked-5.4.0/superlinked/framework/dsl/space/number_space.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 from superlinked.framework.common.dag.constant_node import ConstantNode
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.dag.number_embedding_node import (
     NumberEmbeddingNode,
     NumberEmbeddingParams,
 )
-from superlinked.framework.common.dag.number_similarity_node import NumberSimilarityNode
 from superlinked.framework.common.dag.schema_field_node import SchemaFieldNode
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.embedding.number_embedding import Mode
 from superlinked.framework.common.schema.schema_object import Number, SchemaObject
 from superlinked.framework.common.space.aggregation import InputAggregationMode
 from superlinked.framework.dsl.space.exception import (
     InvalidSpaceParamException,
@@ -101,53 +100,40 @@
         self.aggregation_mode = aggregation_mode
         self.embedding_params = NumberEmbeddingParams(
             min_value=float(min_value),
             max_value=float(max_value),
             mode=mode,
             negative_filter=negative_filter,
         )
-        number_node_map = {
-            num: self.__create_node(SchemaFieldNode(num)) for num in self._field_set
-        }
-        self.number = SpaceFieldSet(self, set(number_node_map.keys()))
-        self.__schema_node_map: dict[SchemaObject, Node] = {
-            schema_field.schema_obj: node
-            for schema_field, node in number_node_map.items()
-        }
         self.default_constant_node_input: int | float | None
         match mode:
             case Mode.MAXIMUM:
                 self.default_constant_node_input = max_value
             case Mode.MINIMUM:
                 self.default_constant_node_input = min_value
             case Mode.SIMILAR:
                 self.default_constant_node_input = None
             case _:
                 raise ValueError(f"Unknown mode: {mode}")
+        number_node_map = {
+            num: NumberEmbeddingNode(
+                SchemaFieldNode(num), self.embedding_params, self.aggregation_mode
+            )
+            for num in self._field_set
+        }
+        self.number = SpaceFieldSet(self, set(number_node_map.keys()))
+        self.__schema_node_map: dict[SchemaObject, Node] = {
+            schema_field.schema_obj: node
+            for schema_field, node in number_node_map.items()
+        }
 
     @property
     def _node_by_schema(self) -> Mapping[SchemaObject, Node[Vector]]:
         return self.__schema_node_map
 
-    def __create_node(
-        self,
-        schema_field_node: SchemaFieldNode,
-    ) -> Node:
-        return (
-            NumberSimilarityNode(
-                schema_field_node,
-                self.embedding_params.min_value,
-                self.embedding_params.max_value,
-                self.embedding_params.negative_filter,
-                self.aggregation_mode,
-            )
-            if self.embedding_params.mode == Mode.SIMILAR
-            else NumberEmbeddingNode(schema_field_node, self.embedding_params)
-        )
-
     def __validate_parameters(
         self, min_value: float | int, max_value: float | int, negative_filter: float
     ) -> None:
         if min_value >= max_value:
             raise InvalidSpaceParamException(
                 f"The maximum value ({max_value}) should be greater than the minimum value ({min_value})."
             )
@@ -164,11 +150,11 @@
                 "clause is needed in the query."
             )
         constant_node = cast(
             Node, ConstantNode(value=self.default_constant_node_input, schema=schema)
         )
 
         number_embedding_node = NumberEmbeddingNode(
-            constant_node, self.embedding_params
+            constant_node, self.embedding_params, self.aggregation_mode
         )
         self.__schema_node_map[schema] = number_embedding_node
         return number_embedding_node
```

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/space/recency_space.py` & `superlinked-5.4.0/superlinked/framework/dsl/space/recency_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/space/space.py` & `superlinked-5.4.0/superlinked/framework/dsl/space/space.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/space/space_field_set.py` & `superlinked-5.4.0/superlinked/framework/dsl/space/space_field_set.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/dsl/space/text_similarity_space.py` & `superlinked-5.4.0/superlinked/framework/dsl/space/text_similarity_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/evaluator/dag_evaluator.py` & `superlinked-5.4.0/superlinked/framework/evaluator/dag_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/evaluator/online_dag_evaluator.py` & `superlinked-5.4.0/superlinked/framework/evaluator/online_dag_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/evaluator/query_dag_evaluator.py` & `superlinked-5.4.0/superlinked/framework/evaluator/query_dag_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/online/dag/batched_chunk_input_item.py` & `superlinked-5.4.0/superlinked/framework/online/dag/batched_chunk_input_item.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/online/dag/default_online_node.py` & `superlinked-5.4.0/superlinked/framework/online/dag/default_online_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/online/dag/evaluation_result.py` & `superlinked-5.4.0/superlinked/framework/online/dag/evaluation_result.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/online/dag/exception.py` & `superlinked-5.4.0/superlinked/framework/online/dag/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/online/dag/online_aggregation_node.py` & `superlinked-5.4.0/superlinked/framework/online/dag/online_aggregation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/online/dag/online_categorical_similarity_node.py` & `superlinked-5.4.0/superlinked/framework/online/dag/online_categorical_similarity_node.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,18 +54,19 @@
 
     @override
     def evaluate_self(
         self,
         parsed_schemas: list[ParsedSchema],
         context: ExecutionContext,
     ) -> list[EvaluationResult[Vector]]:
-        if self._is_query_without_similar_clause(parsed_schemas, context):
-            vector = Vector([0] * self.node.length)
+        if self._should_return_default_vector(parsed_schemas, context):
             return [
-                EvaluationResult(self._get_single_evaluation_result(vector))
+                EvaluationResult(
+                    self._get_single_evaluation_result(self.node.default_vector)
+                )
                 for _ in parsed_schemas
             ]
         return [self.evaluate_self_single(schema, context) for schema in parsed_schemas]
 
     def evaluate_self_single(
         self,
         parsed_schema: ParsedSchema,
```

### Comparing `superlinked-5.3.0/superlinked/framework/online/dag/online_chunking_node.py` & `superlinked-5.4.0/superlinked/framework/online/dag/online_chunking_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/online/dag/online_comparison_filter_node.py` & `superlinked-5.4.0/superlinked/framework/online/dag/online_comparison_filter_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/online/dag/online_concatenation_node.py` & `superlinked-5.4.0/superlinked/framework/online/dag/online_concatenation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/online/dag/online_constant_node.py` & `superlinked-5.4.0/superlinked/framework/online/dag/online_constant_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/online/dag/online_custom_node.py` & `superlinked-5.4.0/superlinked/framework/online/dag/online_custom_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/online/dag/online_event_aggregation_node.py` & `superlinked-5.4.0/superlinked/framework/online/dag/online_event_aggregation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/online/dag/online_index_node.py` & `superlinked-5.4.0/superlinked/framework/online/dag/online_index_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/online/dag/online_node.py` & `superlinked-5.4.0/superlinked/framework/online/dag/online_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         parent_validation_type: ParentValidationType,
     ) -> None:
         if not parent_validation_type.validator(len(self.parents)):
             raise ParentCountException(
                 f"{type(self).__name__} must have {parent_validation_type.description}."
             )
 
-    def _is_query_without_similar_clause(
+    def _should_return_default_vector(
         self,
         parsed_schemas: list[ParsedSchema],
         context: ExecutionContext,
     ) -> bool:
         return context.is_query_context() and not any(
             schema.fields for schema in parsed_schemas
         )
```

### Comparing `superlinked-5.3.0/superlinked/framework/online/dag/online_node_registry.py` & `superlinked-5.4.0/superlinked/framework/online/dag/online_node_registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,17 +43,14 @@
 from superlinked.framework.online.dag.online_named_function_node import (
     OnlineNamedFunctionNode,
 )
 from superlinked.framework.online.dag.online_node import OnlineNode
 from superlinked.framework.online.dag.online_number_embedding_node import (
     OnlineNumberEmbeddingNode,
 )
-from superlinked.framework.online.dag.online_number_similarity_node import (
-    OnlineNumberSimilarityNode,
-)
 from superlinked.framework.online.dag.online_recency_node import OnlineRecencyNode
 from superlinked.framework.online.dag.online_schema_field_node import (
     OnlineSchemaFieldNode,
 )
 from superlinked.framework.online.dag.online_text_embedding_node import (
     OnlineTextEmbeddingNode,
 )
@@ -67,15 +64,14 @@
     OnlineConcatenationNode,
     OnlineConstantNode,
     OnlineCustomVectorEmbeddingNode,
     OnlineEventAggregationNode,
     OnlineIndexNode,
     OnlineNamedFunctionNode,
     OnlineNumberEmbeddingNode,
-    OnlineNumberSimilarityNode,
     OnlineRecencyNode,
     OnlineSchemaFieldNode,
     OnlineTextEmbeddingNode,
     # * Add new OnlineNode implementations here
 ]
```

### Comparing `superlinked-5.3.0/superlinked/framework/online/dag/online_number_embedding_node.py` & `superlinked-5.4.0/superlinked/framework/online/dag/online_number_embedding_node.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from typing_extensions import override
 
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.dag.number_embedding_node import NumberEmbeddingNode
 from superlinked.framework.common.data_types import Vector
+from superlinked.framework.common.embedding.number_embedding import Mode
 from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
 from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 from superlinked.framework.online.dag.evaluation_result import EvaluationResult
 from superlinked.framework.online.dag.online_node import OnlineNode
 from superlinked.framework.online.dag.parent_validator import ParentValidationType
 
@@ -50,25 +51,39 @@
 
     @override
     def evaluate_self(
         self,
         parsed_schemas: list[ParsedSchema],
         context: ExecutionContext,
     ) -> list[EvaluationResult[Vector]]:
+        if self._should_return_default_vector(parsed_schemas, context):
+            return [
+                EvaluationResult(
+                    self._get_single_evaluation_result(self.node.default_vector)
+                )
+                for _ in parsed_schemas
+            ]
         return [self.evaluate_self_single(schema, context) for schema in parsed_schemas]
 
+    @override
+    def _should_return_default_vector(
+        self,
+        parsed_schemas: list[ParsedSchema],
+        context: ExecutionContext,
+    ) -> bool:
+        is_query_context = context.is_query_context()
+        is_mode_similar = self.node.mode == Mode.SIMILAR
+        has_no_fields_in_schemas = not any(schema.fields for schema in parsed_schemas)
+        return is_query_context and (not is_mode_similar or has_no_fields_in_schemas)
+
     def evaluate_self_single(
         self,
         parsed_schema: ParsedSchema,
         context: ExecutionContext,
     ) -> EvaluationResult[Vector]:
-        if context.is_query_context():
-            vector = Vector([1.0] * self.node.length)
-            return EvaluationResult(self._get_single_evaluation_result(vector))
-
         if len(self.parents) == 0:
             stored_result = self.load_stored_result_or_raise_exception(parsed_schema)
             return EvaluationResult(self._get_single_evaluation_result(stored_result))
 
         input_: EvaluationResult[float | int] = cast(
             OnlineNode[Node[float | int], float | int], self.parents[0]
         ).evaluate_next_single(parsed_schema, context)
```

### Comparing `superlinked-5.3.0/superlinked/framework/online/dag/online_number_similarity_node.py` & `superlinked-5.4.0/superlinked/framework/online/dag/online_schema_field_node.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,70 +10,86 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from typing import cast
+from typing import Generic, cast
 
 from typing_extensions import override
 
 from superlinked.framework.common.dag.context import ExecutionContext
-from superlinked.framework.common.dag.node import Node
-from superlinked.framework.common.dag.number_similarity_node import NumberSimilarityNode
-from superlinked.framework.common.data_types import Vector
-from superlinked.framework.common.interface.has_length import HasLength
-from superlinked.framework.common.parser.parsed_schema import ParsedSchema
+from superlinked.framework.common.dag.schema_field_node import SchemaFieldNode
+from superlinked.framework.common.parser.parsed_schema import (
+    ParsedSchema,
+    ParsedSchemaField,
+)
+from superlinked.framework.common.schema.schema_object import SFT, Timestamp
 from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 from superlinked.framework.online.dag.evaluation_result import EvaluationResult
+from superlinked.framework.online.dag.exception import ValueNotProvidedException
 from superlinked.framework.online.dag.online_node import OnlineNode
 from superlinked.framework.online.dag.parent_validator import ParentValidationType
 
 
-class OnlineNumberSimilarityNode(OnlineNode[NumberSimilarityNode, Vector], HasLength):
+class OnlineSchemaFieldNode(Generic[SFT], OnlineNode[SchemaFieldNode, SFT]):
     def __init__(
         self,
-        node: NumberSimilarityNode,
+        node: SchemaFieldNode,
         parents: list[OnlineNode],
         storage_manager: StorageManager,
     ) -> None:
         super().__init__(
             node,
             parents,
             storage_manager,
-            ParentValidationType.LESS_THAN_TWO_PARENTS,
+            ParentValidationType.NO_PARENTS,
         )
 
-    @property
-    def length(self) -> int:
-        return self.node.length
-
     @override
     def evaluate_self(
         self,
         parsed_schemas: list[ParsedSchema],
         context: ExecutionContext,
-    ) -> list[EvaluationResult[Vector]]:
-        if self._is_query_without_similar_clause(parsed_schemas, context):
-            vector = Vector([0] * self.node.length)
-            return [
-                EvaluationResult(self._get_single_evaluation_result(vector))
-                for _ in parsed_schemas
-            ]
+    ) -> list[EvaluationResult[SFT]]:
         return [self.evaluate_self_single(schema, context) for schema in parsed_schemas]
 
     def evaluate_self_single(
         self,
         parsed_schema: ParsedSchema,
         context: ExecutionContext,
-    ) -> EvaluationResult[Vector]:
-        if len(self.parents) == 0:
-            stored_result = self.load_stored_result_or_raise_exception(parsed_schema)
-            return EvaluationResult(self._get_single_evaluation_result(stored_result))
-
-        input_: EvaluationResult[float | int] = cast(
-            OnlineNode[Node[float | int], float | int], self.parents[0]
-        ).evaluate_next_single(parsed_schema, context)
-        transformed_input_value = self.node.embedding.embed(input_.main.value, context)
-        main = self._get_single_evaluation_result(transformed_input_value)
-        return EvaluationResult(main)
+    ) -> EvaluationResult[SFT]:
+        parsed_nodes: list[ParsedSchemaField] = [
+            field
+            for field in parsed_schema.fields
+            if field.schema_field == self.node.schema_field
+        ]
+        result: SFT
+        if parsed_nodes:
+            result = parsed_nodes[0].value
+        else:
+            result = self.__get_default_result(parsed_schema, context)
+        return EvaluationResult(self._get_single_evaluation_result(result))
+
+    def __get_default_result(
+        self,
+        parsed_schema: ParsedSchema,
+        context: ExecutionContext,
+    ) -> SFT:
+        stored_result = self.load_stored_result(parsed_schema.id_, parsed_schema.schema)
+        if stored_result:
+            return stored_result
+        if isinstance(self.node.schema_field, Timestamp):
+            return cast(SFT, context.now())
+        field_name = ".".join(
+            [
+                self.node.schema_field.schema_obj._schema_name,
+                self.node.schema_field.name,
+            ]
+        )
+        raise ValueNotProvidedException(
+            (
+                f"The SchemaField {field_name} "
+                + "doesn't have a default value and was not provided in the ParsedSchema.",
+            )
+        )
```

### Comparing `superlinked-5.3.0/superlinked/framework/online/dag/online_recency_node.py` & `superlinked-5.4.0/superlinked/framework/online/dag/online_recency_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/online/dag/online_schema_dag.py` & `superlinked-5.4.0/superlinked/framework/online/dag/online_schema_dag.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/online/dag/online_schema_field_node.py` & `superlinked-5.4.0/superlinked/framework/online/dag/online_text_embedding_node.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,86 +10,79 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from typing import Generic, cast
+from typing import cast
 
+from beartype.typing import Sequence
 from typing_extensions import override
 
 from superlinked.framework.common.dag.context import ExecutionContext
-from superlinked.framework.common.dag.schema_field_node import SchemaFieldNode
-from superlinked.framework.common.parser.parsed_schema import (
-    ParsedSchema,
-    ParsedSchemaField,
-)
-from superlinked.framework.common.schema.schema_object import SFT, Timestamp
+from superlinked.framework.common.dag.text_embedding_node import TextEmbeddingNode
+from superlinked.framework.common.data_types import Vector
+from superlinked.framework.common.interface.has_length import HasLength
+from superlinked.framework.common.parser.parsed_schema import ParsedSchema
 from superlinked.framework.common.storage_manager.storage_manager import StorageManager
-from superlinked.framework.online.dag.evaluation_result import EvaluationResult
-from superlinked.framework.online.dag.exception import ValueNotProvidedException
+from superlinked.framework.online.dag.default_online_node import DefaultOnlineNode
+from superlinked.framework.online.dag.evaluation_result import (
+    EvaluationResult,
+    SingleEvaluationResult,
+)
 from superlinked.framework.online.dag.online_node import OnlineNode
-from superlinked.framework.online.dag.parent_validator import ParentValidationType
 
 
-class OnlineSchemaFieldNode(Generic[SFT], OnlineNode[SchemaFieldNode, SFT]):
+class OnlineTextEmbeddingNode(DefaultOnlineNode[TextEmbeddingNode, Vector], HasLength):
     def __init__(
         self,
-        node: SchemaFieldNode,
+        node: TextEmbeddingNode,
         parents: list[OnlineNode],
         storage_manager: StorageManager,
     ) -> None:
-        super().__init__(
-            node,
-            parents,
-            storage_manager,
-            ParentValidationType.NO_PARENTS,
-        )
+        super().__init__(node, parents, storage_manager)
+
+    @property
+    def length(self) -> int:
+        return self.node.length
 
     @override
     def evaluate_self(
         self,
         parsed_schemas: list[ParsedSchema],
         context: ExecutionContext,
-    ) -> list[EvaluationResult[SFT]]:
-        return [self.evaluate_self_single(schema, context) for schema in parsed_schemas]
+    ) -> list[EvaluationResult[Vector]]:
+        if self._should_return_default_vector(parsed_schemas, context):
+            return [
+                EvaluationResult(
+                    self._get_single_evaluation_result(self.node.default_vector)
+                )
+                for _ in parsed_schemas
+            ]
+        return super().evaluate_self(parsed_schemas, context)
 
-    def evaluate_self_single(
+    @override
+    def _evaluate_singles(
         self,
-        parsed_schema: ParsedSchema,
+        parent_results: list[dict[OnlineNode, SingleEvaluationResult]],
         context: ExecutionContext,
-    ) -> EvaluationResult[SFT]:
-        parsed_nodes: list[ParsedSchemaField] = [
-            field
-            for field in parsed_schema.fields
-            if field.schema_field == self.node.schema_field
+    ) -> Sequence[Vector | None]:
+        none_indices = [
+            i for i, parent_result in enumerate(parent_results) if not parent_result
         ]
-        result: SFT
-        if parsed_nodes:
-            result = parsed_nodes[0].value
-        else:
-            result = self.__get_default_result(parsed_schema, context)
-        return EvaluationResult(self._get_single_evaluation_result(result))
-
-    def __get_default_result(
-        self,
-        parsed_schema: ParsedSchema,
-        context: ExecutionContext,
-    ) -> SFT:
-        stored_result = self.load_stored_result(parsed_schema.id_, parsed_schema.schema)
-        if stored_result:
-            return stored_result
-        if isinstance(self.node.schema_field, Timestamp):
-            return cast(SFT, context.now())
-        field_name = ".".join(
-            [
-                self.node.schema_field.schema_obj._schema_name,
-                self.node.schema_field.name,
-            ]
-        )
-        raise ValueNotProvidedException(
-            (
-                f"The SchemaField {field_name} "
-                + "doesn't have a default value and was not provided in the ParsedSchema.",
+        non_none_parent_results = [
+            parent_result for parent_result in parent_results if parent_result
+        ]
+        input_ = list(
+            map(
+                lambda parent_result: list(parent_result.values())[0].value,
+                non_none_parent_results,
             )
         )
+        embedded_texts = cast(list[Vector | None], self.__embed_texts(input_))
+        for i in none_indices:
+            embedded_texts.insert(i, None)
+        return embedded_texts
+
+    def __embed_texts(self, texts: list[str]) -> list[Vector]:
+        return self.node.embedding.embed_multiple(texts)
```

### Comparing `superlinked-5.3.0/superlinked/framework/online/dag/parent_results.py` & `superlinked-5.4.0/superlinked/framework/online/dag/parent_results.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/online/dag/parent_validator.py` & `superlinked-5.4.0/superlinked/framework/online/dag/parent_validator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/online/source/in_memory_data_processor.py` & `superlinked-5.4.0/superlinked/framework/online/source/in_memory_data_processor.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/online/source/in_memory_object_writer.py` & `superlinked-5.4.0/superlinked/framework/online/source/in_memory_object_writer.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/online/source/in_memory_source.py` & `superlinked-5.4.0/superlinked/framework/online/source/in_memory_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/storage/in_memory/exception.py` & `superlinked-5.4.0/superlinked/framework/storage/in_memory/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/storage/in_memory/in_memory_search.py` & `superlinked-5.4.0/superlinked/framework/storage/in_memory/in_memory_search.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/storage/in_memory/in_memory_vdb.py` & `superlinked-5.4.0/superlinked/framework/storage/in_memory/in_memory_vdb.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/storage/in_memory/index_config.py` & `superlinked-5.4.0/superlinked/framework/storage/in_memory/index_config.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/storage/in_memory/json_codec.py` & `superlinked-5.4.0/superlinked/framework/storage/in_memory/json_codec.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/superlinked/framework/storage/in_memory/object_serializer.py` & `superlinked-5.4.0/superlinked/framework/storage/in_memory/object_serializer.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.3.0/PKG-INFO` & `superlinked-5.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superlinked
-Version: 5.3.0
+Version: 5.4.0
 Summary: The Superlinked vector computing library
 License: Apache-2.0
 Author: Superlinked Release
 Author-email: release@superlinked.com
 Requires-Python: >=3.10,<=3.12.3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

