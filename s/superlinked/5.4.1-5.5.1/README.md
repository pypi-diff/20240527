# Comparing `tmp/superlinked-5.4.1.tar.gz` & `tmp/superlinked-5.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superlinked-5.4.1.tar", max compression
+gzip compressed data, was "superlinked-5.5.1.tar", max compression
```

## Comparing `superlinked-5.4.1.tar` & `superlinked-5.5.1.tar`

### file list

```diff
@@ -1,214 +1,214 @@
--rw-r--r--   0        0        0    11354 2024-05-27 14:52:32.189675 superlinked-5.4.1/LICENSE
--rw-r--r--   0        0        0    28655 2024-05-27 14:52:32.189675 superlinked-5.4.1/NOTICE
--rw-r--r--   0        0        0     6840 2024-05-27 14:52:32.189675 superlinked-5.4.1/PYPI_README.md
--rw-r--r--   0        0        0     3698 2024-05-27 14:55:35.242219 superlinked-5.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/evaluation/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/evaluation/charts/__init__.py
--rw-r--r--   0        0        0     5601 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/evaluation/charts/recency_plotter.py
--rw-r--r--   0        0        0     9028 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/evaluation/vector_sampler.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/calculation/__init__.py
--rw-r--r--   0        0        0      742 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/calculation/distance_metric.py
--rw-r--r--   0        0        0     1510 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/calculation/vector_similarity.py
--rw-r--r--   0        0        0      805 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/const.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/__init__.py
--rw-r--r--   0        0        0     3644 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/aggregation_node.py
--rw-r--r--   0        0        0     2509 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/categorical_similarity_node.py
--rw-r--r--   0        0        0     1520 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/chunking_node.py
--rw-r--r--   0        0        0     2095 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/comparison_filter_node.py
--rw-r--r--   0        0        0     2606 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/concatenation_node.py
--rw-r--r--   0        0        0     1106 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/constant_node.py
--rw-r--r--   0        0        0     4985 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/context.py
--rw-r--r--   0        0        0     1854 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/custom_node.py
--rw-r--r--   0        0        0     5923 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/dag.py
--rw-r--r--   0        0        0     1338 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/dag_effect.py
--rw-r--r--   0        0        0     3687 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/event_aggregation_node.py
--rw-r--r--   0        0        0     1004 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/exception.py
--rw-r--r--   0        0        0     2043 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/index_node.py
--rw-r--r--   0        0        0     1428 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/named_function_node.py
--rw-r--r--   0        0        0     5016 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/node.py
--rw-r--r--   0        0        0     3083 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/number_embedding_node.py
--rw-r--r--   0        0        0     1620 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/period_time.py
--rw-r--r--   0        0        0      897 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/persistence_params.py
--rw-r--r--   0        0        0     2487 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/recency_node.py
--rw-r--r--   0        0        0     1128 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/resolved_schema_reference.py
--rw-r--r--   0        0        0     2019 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/schema_dag.py
--rw-r--r--   0        0        0     1463 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/schema_field_node.py
--rw-r--r--   0        0        0     1378 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/schema_object_reference.py
--rw-r--r--   0        0        0     2250 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/dag/text_embedding_node.py
--rw-r--r--   0        0        0     8107 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/data_types.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/embedding/__init__.py
--rw-r--r--   0        0        0     5201 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/embedding/categorical_similarity_embedding.py
--rw-r--r--   0        0        0     5890 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/embedding/chunking_util.py
--rw-r--r--   0        0        0     1507 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/embedding/custom_embedding.py
--rw-r--r--   0        0        0     1280 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/embedding/embedding.py
--rw-r--r--   0        0        0     3772 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/embedding/number_embedding.py
--rw-r--r--   0        0        0     8046 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/embedding/recency_embedding.py
--rw-r--r--   0        0        0     2134 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/embedding/sentence_transformer_embedding.py
--rw-r--r--   0        0        0     1250 2024-05-27 14:52:32.237675 superlinked-5.4.1/superlinked/framework/common/exception.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/interface/__init__.py
--rw-r--r--   0        0        0     5851 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/interface/comparison_operand.py
--rw-r--r--   0        0        0      841 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/interface/comparison_operation_type.py
--rw-r--r--   0        0        0      808 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/interface/has_aggregation.py
--rw-r--r--   0        0        0      796 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/interface/has_default_vector.py
--rw-r--r--   0        0        0      718 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/interface/has_length.py
--rw-r--r--   0        0        0      836 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/interface/has_multiplier.py
--rw-r--r--   0        0        0      940 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/interface/weighted.py
--rw-r--r--   0        0        0     1322 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/observable.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/parser/__init__.py
--rw-r--r--   0        0        0     5829 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/parser/data_parser.py
--rw-r--r--   0        0        0     5402 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/parser/dataframe_parser.py
--rw-r--r--   0        0        0      814 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/parser/exception.py
--rw-r--r--   0        0        0     4634 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/parser/json_parser.py
--rw-r--r--   0        0        0     1396 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/parser/parsed_schema.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/__init__.py
--rw-r--r--   0        0        0     1072 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/event_schema.py
--rw-r--r--   0        0        0     1964 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/event_schema_object.py
--rw-r--r--   0        0        0     1014 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/exception.py
--rw-r--r--   0        0        0      627 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/general_type.py
--rw-r--r--   0        0        0     1533 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/id_schema_object.py
--rw-r--r--   0        0        0     1178 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/schema.py
--rw-r--r--   0        0        0     3189 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/schema_decorator.py
--rw-r--r--   0        0        0     3228 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/schema_factory.py
--rw-r--r--   0        0        0     6448 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/schema_object.py
--rw-r--r--   0        0        0     3170 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/schema_reference.py
--rw-r--r--   0        0        0      686 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/schema_type.py
--rw-r--r--   0        0        0     3220 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/schema/schema_validator.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/source/__init__.py
--rw-r--r--   0        0        0      857 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/source/source.py
--rw-r--r--   0        0        0      647 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/source/types.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/space/__init__.py
--rw-r--r--   0        0        0     4492 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/space/aggregation.py
--rw-r--r--   0        0        0     2055 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/space/normalization.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/__init__.py
--rw-r--r--   0        0        0      820 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/entity.py
--rw-r--r--   0        0        0      855 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/entity_data.py
--rw-r--r--   0        0        0      696 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/entity_id.py
--rw-r--r--   0        0        0      627 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/exception.py
--rw-r--r--   0        0        0     1656 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/field.py
--rw-r--r--   0        0        0     2616 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/field_data.py
--rw-r--r--   0        0        0      757 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/field_data_type.py
--rw-r--r--   0        0        0     3514 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/field_encoder.py
--rw-r--r--   0        0        0     2772 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/field_type_converter.py
--rw-r--r--   0        0        0      746 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/persistence_type.py
--rw-r--r--   0        0        0      769 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/result_entity_data.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/search_index_creation/__init__.py
--rw-r--r--   0        0        0     1242 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py
--rw-r--r--   0        0        0      671 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/search_index_creation/search_algorithm.py
--rw-r--r--   0        0        0      692 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py
--rw-r--r--   0        0        0     2397 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/vdb_connector.py
--rw-r--r--   0        0        0     1095 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage/vdb_knn_search_params.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage_manager/__init__.py
--rw-r--r--   0        0        0     5459 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage_manager/admin_fields.py
--rw-r--r--   0        0        0     5549 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage_manager/entity_builder.py
--rw-r--r--   0        0        0      720 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage_manager/header.py
--rw-r--r--   0        0        0     1079 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage_manager/knn_search_params.py
--rw-r--r--   0        0        0      932 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage_manager/search_result_item.py
--rw-r--r--   0        0        0    16654 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage_manager/storage_manager.py
--rw-r--r--   0        0        0     1533 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/storage_manager/storage_naming.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/util/__init__.py
--rw-r--r--   0        0        0      787 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/util/collection_util.py
--rw-r--r--   0        0        0     2074 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/util/dot_separated_path_util.py
--rw-r--r--   0        0        0     1777 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/util/generic_class_util.py
--rw-r--r--   0        0        0      707 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/util/immutable_model.py
--rw-r--r--   0        0        0     1058 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/util/named_function_evaluator.py
--rw-r--r--   0        0        0     1642 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/util/string_util.py
--rw-r--r--   0        0        0      907 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/util/time_util.py
--rw-r--r--   0        0        0     4383 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/common/util/type_validator.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/compiler/__init__.py
--rw-r--r--   0        0        0     2399 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/compiler/online_schema_dag_compiler.py
--rw-r--r--   0        0        0      108 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/dsl/__init__.py
--rw-r--r--   0        0        0      221 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/dsl/executor/__init__.py
--rw-r--r--   0        0        0      719 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/dsl/executor/exception.py
--rw-r--r--   0        0        0     3836 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/dsl/executor/executor.py
--rw-r--r--   0        0        0      124 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/dsl/executor/in_memory/__init__.py
--rw-r--r--   0        0        0     7115 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py
--rw-r--r--   0        0        0      119 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/dsl/executor/query/__init__.py
--rw-r--r--   0        0        0     6902 2024-05-27 14:52:32.241675 superlinked-5.4.1/superlinked/framework/dsl/executor/query/query_executor.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/executor/rest/__init__.py
--rw-r--r--   0        0        0     1540 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/executor/rest/rest_configuration.py
--rw-r--r--   0        0        0      818 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/executor/rest/rest_descriptor.py
--rw-r--r--   0        0        0     4834 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/executor/rest/rest_executor.py
--rw-r--r--   0        0        0     3236 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/executor/rest/rest_handler.py
--rw-r--r--   0        0        0      176 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/index/__init__.py
--rw-r--r--   0        0        0     1904 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/index/effect.py
--rw-r--r--   0        0        0    10985 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/index/index.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/index/util/__init__.py
--rw-r--r--   0        0        0     1516 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/index/util/aggregation_effect_group.py
--rw-r--r--   0        0        0     2448 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/index/util/aggregation_node_util.py
--rw-r--r--   0        0        0     6203 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py
--rw-r--r--   0        0        0     2557 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py
--rw-r--r--   0        0        0     3673 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/index/util/event_aggregation_node_util.py
--rw-r--r--   0        0        0      192 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/query/__init__.py
--rw-r--r--   0        0        0     1183 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/query/param.py
--rw-r--r--   0        0        0     3503 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/query/param_evaluator.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/query/predicate/__init__.py
--rw-r--r--   0        0        0      756 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/query/predicate/binary_op.py
--rw-r--r--   0        0        0     2739 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/query/predicate/binary_predicate.py
--rw-r--r--   0        0        0     1128 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/query/predicate/query_predicate.py
--rw-r--r--   0        0        0    13577 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/query/query.py
--rw-r--r--   0        0        0     6144 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/query/query_filters.py
--rw-r--r--   0        0        0    11142 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/query/query_vector_factory.py
--rw-r--r--   0        0        0     3329 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/query/query_weighting.py
--rw-r--r--   0        0        0     2613 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/query/result.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/registry/__init__.py
--rw-r--r--   0        0        0      636 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/registry/exception.py
--rw-r--r--   0        0        0     1330 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/registry/superlinked_registry.py
--rw-r--r--   0        0        0      214 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/source/__init__.py
--rw-r--r--   0        0        0     2225 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/source/data_loader_source.py
--rw-r--r--   0        0        0     2773 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/source/in_memory_source.py
--rw-r--r--   0        0        0     1987 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/source/rest_source.py
--rw-r--r--   0        0        0     1144 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/source/source.py
--rw-r--r--   0        0        0      183 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/space/__init__.py
--rw-r--r--   0        0        0     7479 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/space/categorical_similarity_space.py
--rw-r--r--   0        0        0     5509 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/space/custom_space.py
--rw-r--r--   0        0        0      856 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/space/exception.py
--rw-r--r--   0        0        0     7702 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/space/number_space.py
--rw-r--r--   0        0        0     8456 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/space/recency_space.py
--rw-r--r--   0        0        0     2743 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/space/space.py
--rw-r--r--   0        0        0     1295 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/space/space_field_set.py
--rw-r--r--   0        0        0     4804 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/dsl/space/text_similarity_space.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/evaluator/__init__.py
--rw-r--r--   0        0        0     1043 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/evaluator/dag_evaluator.py
--rw-r--r--   0        0        0     4807 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/evaluator/online_dag_evaluator.py
--rw-r--r--   0        0        0     2237 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/evaluator/query_dag_evaluator.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/__init__.py
--rw-r--r--   0        0        0      801 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/batched_chunk_input_item.py
--rw-r--r--   0        0        0     7597 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/default_online_node.py
--rw-r--r--   0        0        0     1213 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/evaluation_result.py
--rw-r--r--   0        0        0      768 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/exception.py
--rw-r--r--   0        0        0     6312 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_aggregation_node.py
--rw-r--r--   0        0        0     3206 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_categorical_similarity_node.py
--rw-r--r--   0        0        0     3457 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_chunking_node.py
--rw-r--r--   0        0        0     2247 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_comparison_filter_node.py
--rw-r--r--   0        0        0     5138 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_concatenation_node.py
--rw-r--r--   0        0        0     2032 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_constant_node.py
--rw-r--r--   0        0        0     3283 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_custom_node.py
--rw-r--r--   0        0        0     7908 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_event_aggregation_node.py
--rw-r--r--   0        0        0     4052 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_index_node.py
--rw-r--r--   0        0        0     2351 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_named_function_node.py
--rw-r--r--   0        0        0     5086 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_node.py
--rw-r--r--   0        0        0     5547 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_node_registry.py
--rw-r--r--   0        0        0     3704 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_number_embedding_node.py
--rw-r--r--   0        0        0     2713 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_recency_node.py
--rw-r--r--   0        0        0     3732 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_schema_dag.py
--rw-r--r--   0        0        0     3426 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_schema_field_node.py
--rw-r--r--   0        0        0     3256 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/online_text_embedding_node.py
--rw-r--r--   0        0        0      794 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/parent_results.py
--rw-r--r--   0        0        0     1322 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/dag/parent_validator.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/source/__init__.py
--rw-r--r--   0        0        0     3486 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/source/in_memory_data_processor.py
--rw-r--r--   0        0        0     1437 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/source/in_memory_object_writer.py
--rw-r--r--   0        0        0     1752 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/online/source/in_memory_source.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.245675 superlinked-5.4.1/superlinked/framework/storage/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.249675 superlinked-5.4.1/superlinked/framework/storage/in_memory/__init__.py
--rw-r--r--   0        0        0      787 2024-05-27 14:52:32.249675 superlinked-5.4.1/superlinked/framework/storage/in_memory/exception.py
--rw-r--r--   0        0        0     6725 2024-05-27 14:52:32.249675 superlinked-5.4.1/superlinked/framework/storage/in_memory/in_memory_search.py
--rw-r--r--   0        0        0     7121 2024-05-27 14:52:32.249675 superlinked-5.4.1/superlinked/framework/storage/in_memory/in_memory_vdb.py
--rw-r--r--   0        0        0      921 2024-05-27 14:52:32.249675 superlinked-5.4.1/superlinked/framework/storage/in_memory/index_config.py
--rw-r--r--   0        0        0     1305 2024-05-27 14:52:32.249675 superlinked-5.4.1/superlinked/framework/storage/in_memory/json_codec.py
--rw-r--r--   0        0        0     1562 2024-05-27 14:52:32.249675 superlinked-5.4.1/superlinked/framework/storage/in_memory/object_serializer.py
--rw-r--r--   0        0        0        0 2024-05-27 14:52:32.249675 superlinked-5.4.1/superlinked/py.typed
--rw-r--r--   0        0        0     8320 1970-01-01 00:00:00.000000 superlinked-5.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11354 2024-05-27 17:01:58.262537 superlinked-5.5.1/LICENSE
+-rw-r--r--   0        0        0    28655 2024-05-27 17:01:58.262537 superlinked-5.5.1/NOTICE
+-rw-r--r--   0        0        0     6840 2024-05-27 17:01:58.262537 superlinked-5.5.1/PYPI_README.md
+-rw-r--r--   0        0        0     3698 2024-05-27 17:05:06.179776 superlinked-5.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.310537 superlinked-5.5.1/superlinked/evaluation/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.310537 superlinked-5.5.1/superlinked/evaluation/charts/__init__.py
+-rw-r--r--   0        0        0     5601 2024-05-27 17:01:58.310537 superlinked-5.5.1/superlinked/evaluation/charts/recency_plotter.py
+-rw-r--r--   0        0        0     9028 2024-05-27 17:01:58.310537 superlinked-5.5.1/superlinked/evaluation/vector_sampler.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.310537 superlinked-5.5.1/superlinked/framework/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.310537 superlinked-5.5.1/superlinked/framework/common/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.310537 superlinked-5.5.1/superlinked/framework/common/calculation/__init__.py
+-rw-r--r--   0        0        0      742 2024-05-27 17:01:58.310537 superlinked-5.5.1/superlinked/framework/common/calculation/distance_metric.py
+-rw-r--r--   0        0        0     1510 2024-05-27 17:01:58.310537 superlinked-5.5.1/superlinked/framework/common/calculation/vector_similarity.py
+-rw-r--r--   0        0        0      805 2024-05-27 17:01:58.310537 superlinked-5.5.1/superlinked/framework/common/const.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.310537 superlinked-5.5.1/superlinked/framework/common/dag/__init__.py
+-rw-r--r--   0        0        0     3644 2024-05-27 17:01:58.310537 superlinked-5.5.1/superlinked/framework/common/dag/aggregation_node.py
+-rw-r--r--   0        0        0     2509 2024-05-27 17:01:58.310537 superlinked-5.5.1/superlinked/framework/common/dag/categorical_similarity_node.py
+-rw-r--r--   0        0        0     1520 2024-05-27 17:01:58.310537 superlinked-5.5.1/superlinked/framework/common/dag/chunking_node.py
+-rw-r--r--   0        0        0     2095 2024-05-27 17:01:58.310537 superlinked-5.5.1/superlinked/framework/common/dag/comparison_filter_node.py
+-rw-r--r--   0        0        0     2606 2024-05-27 17:01:58.310537 superlinked-5.5.1/superlinked/framework/common/dag/concatenation_node.py
+-rw-r--r--   0        0        0     1106 2024-05-27 17:01:58.310537 superlinked-5.5.1/superlinked/framework/common/dag/constant_node.py
+-rw-r--r--   0        0        0     4985 2024-05-27 17:01:58.310537 superlinked-5.5.1/superlinked/framework/common/dag/context.py
+-rw-r--r--   0        0        0     1854 2024-05-27 17:01:58.310537 superlinked-5.5.1/superlinked/framework/common/dag/custom_node.py
+-rw-r--r--   0        0        0     5923 2024-05-27 17:01:58.310537 superlinked-5.5.1/superlinked/framework/common/dag/dag.py
+-rw-r--r--   0        0        0     1338 2024-05-27 17:01:58.310537 superlinked-5.5.1/superlinked/framework/common/dag/dag_effect.py
+-rw-r--r--   0        0        0     3687 2024-05-27 17:01:58.310537 superlinked-5.5.1/superlinked/framework/common/dag/event_aggregation_node.py
+-rw-r--r--   0        0        0     1004 2024-05-27 17:01:58.310537 superlinked-5.5.1/superlinked/framework/common/dag/exception.py
+-rw-r--r--   0        0        0     2043 2024-05-27 17:01:58.310537 superlinked-5.5.1/superlinked/framework/common/dag/index_node.py
+-rw-r--r--   0        0        0     1428 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/dag/named_function_node.py
+-rw-r--r--   0        0        0     5016 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/dag/node.py
+-rw-r--r--   0        0        0     3083 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/dag/number_embedding_node.py
+-rw-r--r--   0        0        0     1620 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/dag/period_time.py
+-rw-r--r--   0        0        0      897 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/dag/persistence_params.py
+-rw-r--r--   0        0        0     2487 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/dag/recency_node.py
+-rw-r--r--   0        0        0     1128 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/dag/resolved_schema_reference.py
+-rw-r--r--   0        0        0     2019 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/dag/schema_dag.py
+-rw-r--r--   0        0        0     1463 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/dag/schema_field_node.py
+-rw-r--r--   0        0        0     1378 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/dag/schema_object_reference.py
+-rw-r--r--   0        0        0     2250 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/dag/text_embedding_node.py
+-rw-r--r--   0        0        0     8111 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/data_types.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/embedding/__init__.py
+-rw-r--r--   0        0        0     5201 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/embedding/categorical_similarity_embedding.py
+-rw-r--r--   0        0        0     5890 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/embedding/chunking_util.py
+-rw-r--r--   0        0        0     1535 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/embedding/custom_embedding.py
+-rw-r--r--   0        0        0     1280 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/embedding/embedding.py
+-rw-r--r--   0        0        0     3772 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/embedding/number_embedding.py
+-rw-r--r--   0        0        0     8046 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/embedding/recency_embedding.py
+-rw-r--r--   0        0        0     2134 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/embedding/sentence_transformer_embedding.py
+-rw-r--r--   0        0        0     1250 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/exception.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/interface/__init__.py
+-rw-r--r--   0        0        0     5851 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/interface/comparison_operand.py
+-rw-r--r--   0        0        0      841 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/interface/comparison_operation_type.py
+-rw-r--r--   0        0        0      808 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/interface/has_aggregation.py
+-rw-r--r--   0        0        0      796 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/interface/has_default_vector.py
+-rw-r--r--   0        0        0      718 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/interface/has_length.py
+-rw-r--r--   0        0        0      836 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/interface/has_multiplier.py
+-rw-r--r--   0        0        0      940 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/interface/weighted.py
+-rw-r--r--   0        0        0     1322 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/observable.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/parser/__init__.py
+-rw-r--r--   0        0        0     5829 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/parser/data_parser.py
+-rw-r--r--   0        0        0     5402 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/parser/dataframe_parser.py
+-rw-r--r--   0        0        0      814 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/parser/exception.py
+-rw-r--r--   0        0        0     4634 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/parser/json_parser.py
+-rw-r--r--   0        0        0     1396 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/parser/parsed_schema.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/schema/__init__.py
+-rw-r--r--   0        0        0     1072 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/schema/event_schema.py
+-rw-r--r--   0        0        0     1964 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/schema/event_schema_object.py
+-rw-r--r--   0        0        0     1014 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/schema/exception.py
+-rw-r--r--   0        0        0      627 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/schema/general_type.py
+-rw-r--r--   0        0        0     1533 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/schema/id_schema_object.py
+-rw-r--r--   0        0        0     1178 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/schema/schema.py
+-rw-r--r--   0        0        0     3189 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/schema/schema_decorator.py
+-rw-r--r--   0        0        0     3228 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/schema/schema_factory.py
+-rw-r--r--   0        0        0     6462 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/schema/schema_object.py
+-rw-r--r--   0        0        0     3170 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/schema/schema_reference.py
+-rw-r--r--   0        0        0      686 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/schema/schema_type.py
+-rw-r--r--   0        0        0     3220 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/schema/schema_validator.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/source/__init__.py
+-rw-r--r--   0        0        0      857 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/source/source.py
+-rw-r--r--   0        0        0      647 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/source/types.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/space/__init__.py
+-rw-r--r--   0        0        0     4492 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/space/aggregation.py
+-rw-r--r--   0        0        0     2055 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/space/normalization.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/storage/__init__.py
+-rw-r--r--   0        0        0      820 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/storage/entity.py
+-rw-r--r--   0        0        0      855 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/storage/entity_data.py
+-rw-r--r--   0        0        0      696 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/storage/entity_id.py
+-rw-r--r--   0        0        0      627 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/storage/exception.py
+-rw-r--r--   0        0        0     1656 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/storage/field.py
+-rw-r--r--   0        0        0     2627 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/storage/field_data.py
+-rw-r--r--   0        0        0      763 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/storage/field_data_type.py
+-rw-r--r--   0        0        0     3537 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/storage/field_encoder.py
+-rw-r--r--   0        0        0     2888 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/storage/field_type_converter.py
+-rw-r--r--   0        0        0      746 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/storage/persistence_type.py
+-rw-r--r--   0        0        0      769 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/storage/result_entity_data.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/storage/search_index_creation/__init__.py
+-rw-r--r--   0        0        0     1242 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py
+-rw-r--r--   0        0        0      671 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/storage/search_index_creation/search_algorithm.py
+-rw-r--r--   0        0        0      692 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py
+-rw-r--r--   0        0        0     2397 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/storage/vdb_connector.py
+-rw-r--r--   0        0        0     1095 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/storage/vdb_knn_search_params.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/storage_manager/__init__.py
+-rw-r--r--   0        0        0     5459 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/storage_manager/admin_fields.py
+-rw-r--r--   0        0        0     5549 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/storage_manager/entity_builder.py
+-rw-r--r--   0        0        0      720 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/storage_manager/header.py
+-rw-r--r--   0        0        0     1065 2024-05-27 17:01:58.314537 superlinked-5.5.1/superlinked/framework/common/storage_manager/knn_search_params.py
+-rw-r--r--   0        0        0      932 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/common/storage_manager/search_result_item.py
+-rw-r--r--   0        0        0    16295 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/common/storage_manager/storage_manager.py
+-rw-r--r--   0        0        0     1533 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/common/storage_manager/storage_naming.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/common/util/__init__.py
+-rw-r--r--   0        0        0      787 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/common/util/collection_util.py
+-rw-r--r--   0        0        0     2074 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/common/util/dot_separated_path_util.py
+-rw-r--r--   0        0        0     1721 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/common/util/generic_class_util.py
+-rw-r--r--   0        0        0      707 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/common/util/immutable_model.py
+-rw-r--r--   0        0        0     1058 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/common/util/named_function_evaluator.py
+-rw-r--r--   0        0        0     1642 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/common/util/string_util.py
+-rw-r--r--   0        0        0      907 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/common/util/time_util.py
+-rw-r--r--   0        0        0     4383 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/common/util/type_validator.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/compiler/__init__.py
+-rw-r--r--   0        0        0     2399 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/compiler/online_schema_dag_compiler.py
+-rw-r--r--   0        0        0      108 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/__init__.py
+-rw-r--r--   0        0        0      221 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/executor/__init__.py
+-rw-r--r--   0        0        0      719 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/executor/exception.py
+-rw-r--r--   0        0        0     3836 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/executor/executor.py
+-rw-r--r--   0        0        0      124 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/executor/in_memory/__init__.py
+-rw-r--r--   0        0        0     7202 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py
+-rw-r--r--   0        0        0      119 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/executor/query/__init__.py
+-rw-r--r--   0        0        0     7323 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/executor/query/query_executor.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/executor/rest/__init__.py
+-rw-r--r--   0        0        0     1540 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/executor/rest/rest_configuration.py
+-rw-r--r--   0        0        0      818 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/executor/rest/rest_descriptor.py
+-rw-r--r--   0        0        0     4834 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/executor/rest/rest_executor.py
+-rw-r--r--   0        0        0     3236 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/executor/rest/rest_handler.py
+-rw-r--r--   0        0        0      176 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/index/__init__.py
+-rw-r--r--   0        0        0     1904 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/index/effect.py
+-rw-r--r--   0        0        0    10985 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/index/index.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/index/util/__init__.py
+-rw-r--r--   0        0        0     1516 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/index/util/aggregation_effect_group.py
+-rw-r--r--   0        0        0     2448 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/index/util/aggregation_node_util.py
+-rw-r--r--   0        0        0     6203 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py
+-rw-r--r--   0        0        0     2557 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py
+-rw-r--r--   0        0        0     3673 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/index/util/event_aggregation_node_util.py
+-rw-r--r--   0        0        0      192 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/query/__init__.py
+-rw-r--r--   0        0        0     1183 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/query/param.py
+-rw-r--r--   0        0        0     4155 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/query/param_evaluator.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/query/predicate/__init__.py
+-rw-r--r--   0        0        0      756 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/query/predicate/binary_op.py
+-rw-r--r--   0        0        0     2739 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/query/predicate/binary_predicate.py
+-rw-r--r--   0        0        0     1128 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/query/predicate/query_predicate.py
+-rw-r--r--   0        0        0    13548 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/query/query.py
+-rw-r--r--   0        0        0     6144 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/query/query_filters.py
+-rw-r--r--   0        0        0    11142 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/query/query_vector_factory.py
+-rw-r--r--   0        0        0     3329 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/query/query_weighting.py
+-rw-r--r--   0        0        0     2613 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/query/result.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/registry/__init__.py
+-rw-r--r--   0        0        0      636 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/registry/exception.py
+-rw-r--r--   0        0        0     1330 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/registry/superlinked_registry.py
+-rw-r--r--   0        0        0      214 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/source/__init__.py
+-rw-r--r--   0        0        0     2225 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/source/data_loader_source.py
+-rw-r--r--   0        0        0     2773 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/source/in_memory_source.py
+-rw-r--r--   0        0        0     1987 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/source/rest_source.py
+-rw-r--r--   0        0        0     1144 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/source/source.py
+-rw-r--r--   0        0        0      183 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/space/__init__.py
+-rw-r--r--   0        0        0     7479 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/space/categorical_similarity_space.py
+-rw-r--r--   0        0        0     5509 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/space/custom_space.py
+-rw-r--r--   0        0        0      856 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/space/exception.py
+-rw-r--r--   0        0        0     7702 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/space/number_space.py
+-rw-r--r--   0        0        0     8456 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/space/recency_space.py
+-rw-r--r--   0        0        0     2743 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/space/space.py
+-rw-r--r--   0        0        0     1295 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/space/space_field_set.py
+-rw-r--r--   0        0        0     4804 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/dsl/space/text_similarity_space.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/evaluator/__init__.py
+-rw-r--r--   0        0        0     1043 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/evaluator/dag_evaluator.py
+-rw-r--r--   0        0        0     4808 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/evaluator/online_dag_evaluator.py
+-rw-r--r--   0        0        0     2237 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/evaluator/query_dag_evaluator.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/online/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/online/dag/__init__.py
+-rw-r--r--   0        0        0      801 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/online/dag/batched_chunk_input_item.py
+-rw-r--r--   0        0        0     7597 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/online/dag/default_online_node.py
+-rw-r--r--   0        0        0     1213 2024-05-27 17:01:58.318537 superlinked-5.5.1/superlinked/framework/online/dag/evaluation_result.py
+-rw-r--r--   0        0        0      768 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/online/dag/exception.py
+-rw-r--r--   0        0        0     6312 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/online/dag/online_aggregation_node.py
+-rw-r--r--   0        0        0     3206 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/online/dag/online_categorical_similarity_node.py
+-rw-r--r--   0        0        0     3457 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/online/dag/online_chunking_node.py
+-rw-r--r--   0        0        0     2247 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/online/dag/online_comparison_filter_node.py
+-rw-r--r--   0        0        0     5138 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/online/dag/online_concatenation_node.py
+-rw-r--r--   0        0        0     2032 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/online/dag/online_constant_node.py
+-rw-r--r--   0        0        0     3282 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/online/dag/online_custom_node.py
+-rw-r--r--   0        0        0     7908 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/online/dag/online_event_aggregation_node.py
+-rw-r--r--   0        0        0     4052 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/online/dag/online_index_node.py
+-rw-r--r--   0        0        0     2351 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/online/dag/online_named_function_node.py
+-rw-r--r--   0        0        0     5086 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/online/dag/online_node.py
+-rw-r--r--   0        0        0     5547 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/online/dag/online_node_registry.py
+-rw-r--r--   0        0        0     3704 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/online/dag/online_number_embedding_node.py
+-rw-r--r--   0        0        0     2713 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/online/dag/online_recency_node.py
+-rw-r--r--   0        0        0     3732 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/online/dag/online_schema_dag.py
+-rw-r--r--   0        0        0     3426 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/online/dag/online_schema_field_node.py
+-rw-r--r--   0        0        0     3256 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/online/dag/online_text_embedding_node.py
+-rw-r--r--   0        0        0      794 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/online/dag/parent_results.py
+-rw-r--r--   0        0        0     1322 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/online/dag/parent_validator.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/online/source/__init__.py
+-rw-r--r--   0        0        0     3877 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/online/source/in_memory_data_processor.py
+-rw-r--r--   0        0        0     1437 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/online/source/in_memory_object_writer.py
+-rw-r--r--   0        0        0     1752 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/online/source/in_memory_source.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/storage/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/storage/in_memory/__init__.py
+-rw-r--r--   0        0        0      787 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/storage/in_memory/exception.py
+-rw-r--r--   0        0        0     6725 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/storage/in_memory/in_memory_search.py
+-rw-r--r--   0        0        0     7121 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/storage/in_memory/in_memory_vdb.py
+-rw-r--r--   0        0        0      921 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/storage/in_memory/index_config.py
+-rw-r--r--   0        0        0     1305 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/storage/in_memory/json_codec.py
+-rw-r--r--   0        0        0     1562 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/framework/storage/in_memory/object_serializer.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:01:58.322537 superlinked-5.5.1/superlinked/py.typed
+-rw-r--r--   0        0        0     8320 1970-01-01 00:00:00.000000 superlinked-5.5.1/PKG-INFO
```

### Comparing `superlinked-5.4.1/LICENSE` & `superlinked-5.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/NOTICE` & `superlinked-5.5.1/NOTICE`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/PYPI_README.md` & `superlinked-5.5.1/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/pyproject.toml` & `superlinked-5.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "superlinked"
-version = "5.4.1"  # The version will be dynamically updated
+version = "5.5.1"  # The version will be dynamically updated
 description = "The Superlinked vector computing library"
 authors = ["Superlinked Release <release@superlinked.com>"]
 readme = "PYPI_README.md"
 license = "Apache-2.0"
 include = ["NOTICE"]
 
 [tool.poetry.dependencies]
```

### Comparing `superlinked-5.4.1/superlinked/evaluation/charts/recency_plotter.py` & `superlinked-5.5.1/superlinked/evaluation/charts/recency_plotter.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/evaluation/vector_sampler.py` & `superlinked-5.5.1/superlinked/evaluation/vector_sampler.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/calculation/distance_metric.py` & `superlinked-5.5.1/superlinked/framework/common/calculation/distance_metric.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/calculation/vector_similarity.py` & `superlinked-5.5.1/superlinked/framework/common/calculation/vector_similarity.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/const.py` & `superlinked-5.5.1/superlinked/framework/common/const.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/dag/aggregation_node.py` & `superlinked-5.5.1/superlinked/framework/common/dag/aggregation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/dag/categorical_similarity_node.py` & `superlinked-5.5.1/superlinked/framework/common/dag/categorical_similarity_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/dag/chunking_node.py` & `superlinked-5.5.1/superlinked/framework/common/dag/chunking_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/dag/comparison_filter_node.py` & `superlinked-5.5.1/superlinked/framework/common/dag/comparison_filter_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/dag/concatenation_node.py` & `superlinked-5.5.1/superlinked/framework/common/dag/concatenation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/dag/constant_node.py` & `superlinked-5.5.1/superlinked/framework/common/dag/constant_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/dag/context.py` & `superlinked-5.5.1/superlinked/framework/common/dag/context.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/dag/custom_node.py` & `superlinked-5.5.1/superlinked/framework/common/dag/custom_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/dag/dag.py` & `superlinked-5.5.1/superlinked/framework/common/dag/dag.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/dag/dag_effect.py` & `superlinked-5.5.1/superlinked/framework/common/dag/dag_effect.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/dag/event_aggregation_node.py` & `superlinked-5.5.1/superlinked/framework/common/dag/event_aggregation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/dag/exception.py` & `superlinked-5.5.1/superlinked/framework/common/dag/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/dag/index_node.py` & `superlinked-5.5.1/superlinked/framework/common/dag/index_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/dag/named_function_node.py` & `superlinked-5.5.1/superlinked/framework/common/dag/named_function_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/dag/node.py` & `superlinked-5.5.1/superlinked/framework/common/dag/node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/dag/number_embedding_node.py` & `superlinked-5.5.1/superlinked/framework/common/dag/number_embedding_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/dag/period_time.py` & `superlinked-5.5.1/superlinked/framework/common/dag/period_time.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/dag/persistence_params.py` & `superlinked-5.5.1/superlinked/framework/common/dag/persistence_params.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/dag/recency_node.py` & `superlinked-5.5.1/superlinked/framework/common/dag/recency_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/dag/resolved_schema_reference.py` & `superlinked-5.5.1/superlinked/framework/common/dag/resolved_schema_reference.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/dag/schema_dag.py` & `superlinked-5.5.1/superlinked/framework/common/dag/schema_dag.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/dag/schema_field_node.py` & `superlinked-5.5.1/superlinked/framework/common/dag/schema_field_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/dag/schema_object_reference.py` & `superlinked-5.5.1/superlinked/framework/common/dag/schema_object_reference.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/dag/text_embedding_node.py` & `superlinked-5.5.1/superlinked/framework/common/dag/text_embedding_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/data_types.py` & `superlinked-5.5.1/superlinked/framework/common/data_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,8 +223,8 @@
 
     def __copy(self) -> Vector:
         if self.is_empty:
             return self
         return self.copy_with_new()
 
 
-PythonTypes = float | int | str | Vector | NPArray
+PythonTypes = float | int | str | Vector | list[float]
```

### Comparing `superlinked-5.4.1/superlinked/framework/common/embedding/categorical_similarity_embedding.py` & `superlinked-5.5.1/superlinked/framework/common/embedding/categorical_similarity_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/embedding/chunking_util.py` & `superlinked-5.5.1/superlinked/framework/common/embedding/chunking_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/embedding/custom_embedding.py` & `superlinked-5.5.1/superlinked/framework/common/embedding/custom_embedding.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,32 +8,33 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import numpy as np
 from typing_extensions import override
 
 from superlinked.framework.common.dag.context import ExecutionContext
-from superlinked.framework.common.data_types import NPArray, Vector
+from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.embedding.embedding import Embedding
 from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.common.space.normalization import Normalization
 
 
-class CustomEmbedding(Embedding[NPArray], HasLength):
+class CustomEmbedding(Embedding[list[float]], HasLength):
     def __init__(self, length: int, normalization: Normalization) -> None:
         self.__length: int = length
         self._normalization: Normalization = normalization
 
     @override
     def embed(
         self,
-        input_: NPArray,
+        input_: list[float],
         context: ExecutionContext,  # pylint: disable=unused-argument
     ) -> Vector:
-        return Vector(input_).normalize(self._normalization.norm(input_))
+        return Vector(input_).normalize(self._normalization.norm(np.array(input_)))
 
     @property
     def length(self) -> int:
         return self.__length
```

### Comparing `superlinked-5.4.1/superlinked/framework/common/embedding/embedding.py` & `superlinked-5.5.1/superlinked/framework/common/embedding/embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/embedding/number_embedding.py` & `superlinked-5.5.1/superlinked/framework/common/embedding/number_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/embedding/recency_embedding.py` & `superlinked-5.5.1/superlinked/framework/common/embedding/recency_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/embedding/sentence_transformer_embedding.py` & `superlinked-5.5.1/superlinked/framework/common/embedding/sentence_transformer_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/exception.py` & `superlinked-5.5.1/superlinked/framework/common/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/interface/comparison_operand.py` & `superlinked-5.5.1/superlinked/framework/common/interface/comparison_operand.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/interface/comparison_operation_type.py` & `superlinked-5.5.1/superlinked/framework/common/interface/comparison_operation_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/interface/has_aggregation.py` & `superlinked-5.5.1/superlinked/framework/common/interface/has_aggregation.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/interface/has_default_vector.py` & `superlinked-5.5.1/superlinked/framework/common/interface/has_default_vector.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/interface/has_length.py` & `superlinked-5.5.1/superlinked/framework/common/interface/has_length.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/interface/has_multiplier.py` & `superlinked-5.5.1/superlinked/framework/common/interface/has_multiplier.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/interface/weighted.py` & `superlinked-5.5.1/superlinked/framework/common/interface/weighted.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/observable.py` & `superlinked-5.5.1/superlinked/framework/common/observable.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/parser/data_parser.py` & `superlinked-5.5.1/superlinked/framework/common/parser/data_parser.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/parser/dataframe_parser.py` & `superlinked-5.5.1/superlinked/framework/common/parser/dataframe_parser.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/parser/exception.py` & `superlinked-5.5.1/superlinked/framework/common/parser/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/parser/json_parser.py` & `superlinked-5.5.1/superlinked/framework/common/parser/json_parser.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/parser/parsed_schema.py` & `superlinked-5.5.1/superlinked/framework/common/parser/parsed_schema.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/schema/event_schema.py` & `superlinked-5.5.1/superlinked/framework/common/schema/event_schema.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/schema/event_schema_object.py` & `superlinked-5.5.1/superlinked/framework/common/schema/event_schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/schema/exception.py` & `superlinked-5.5.1/superlinked/framework/common/schema/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/schema/general_type.py` & `superlinked-5.5.1/superlinked/framework/common/schema/general_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/schema/id_schema_object.py` & `superlinked-5.5.1/superlinked/framework/common/schema/id_schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/schema/schema.py` & `superlinked-5.5.1/superlinked/framework/common/schema/schema.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/schema/schema_decorator.py` & `superlinked-5.5.1/superlinked/framework/common/schema/schema_decorator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/schema/schema_factory.py` & `superlinked-5.5.1/superlinked/framework/common/schema/schema_factory.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/schema/schema_object.py` & `superlinked-5.5.1/superlinked/framework/common/schema/schema_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 from abc import abstractmethod
 from dataclasses import dataclass
+from itertools import chain
 from typing import Any, Generic, TypeVar
 
-import numpy as np
 from beartype.typing import Sequence
 
-from superlinked.framework.common.data_types import NPArray, PythonTypes
+from superlinked.framework.common.data_types import PythonTypes
 from superlinked.framework.common.interface.comparison_operand import ComparisonOperand
 
 # Exclude from documentation.
 # A better approach would be to separate this file into atomic objects,
 # which is blocked due to circular dependency issues.
 __pdoc__ = {}
 __pdoc__["SchemaFieldDescriptor"] = False
@@ -187,27 +187,27 @@
         super().__init__(name, schema_obj, int)
 
     @staticmethod
     def join_values(values: Sequence[int]) -> int:
         return int(sum(values) / len(values))
 
 
-class Array(SchemaField[NPArray]):
+class Array(SchemaField[list[float]]):
     """
     Field of a schema that represents a vector.
     """
 
     def __init__(self, name: str, schema_obj: SchemaObjectT) -> None:
-        super().__init__(name, schema_obj, NPArray)
+        super().__init__(name, schema_obj, list[float])
 
     @staticmethod
     def join_values(
-        values: Sequence[NPArray],
-    ) -> NPArray:
-        return np.array(list(values)).mean(axis=0)
+        values: Sequence[list[float]],
+    ) -> list[float]:
+        return list(chain.from_iterable(values))
 
 
 ConcreteSchemaField = String | Timestamp | Float | Integer | Array
 ConcreteSchemaFieldT = TypeVar("ConcreteSchemaFieldT", bound="ConcreteSchemaField")
 
 
 @dataclass
```

### Comparing `superlinked-5.4.1/superlinked/framework/common/schema/schema_reference.py` & `superlinked-5.5.1/superlinked/framework/common/schema/schema_reference.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/schema/schema_type.py` & `superlinked-5.5.1/superlinked/framework/common/schema/schema_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/schema/schema_validator.py` & `superlinked-5.5.1/superlinked/framework/common/schema/schema_validator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/source/source.py` & `superlinked-5.5.1/superlinked/framework/common/source/source.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/source/types.py` & `superlinked-5.5.1/superlinked/framework/common/source/types.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/space/aggregation.py` & `superlinked-5.5.1/superlinked/framework/common/space/aggregation.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/space/normalization.py` & `superlinked-5.5.1/superlinked/framework/common/space/normalization.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/storage/entity.py` & `superlinked-5.5.1/superlinked/framework/common/storage/entity.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/storage/entity_data.py` & `superlinked-5.5.1/superlinked/framework/common/storage/entity_data.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/storage/entity_id.py` & `superlinked-5.5.1/superlinked/framework/common/storage/entity_id.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/storage/exception.py` & `superlinked-5.5.1/superlinked/framework/common/storage/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/storage/field.py` & `superlinked-5.5.1/superlinked/framework/common/storage/field.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/storage/field_data.py` & `superlinked-5.5.1/superlinked/framework/common/storage/field_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 
 from __future__ import annotations
 
 from typing import Generic, TypeVar
 
-from superlinked.framework.common.data_types import NPArray, Vector
+from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.storage.field import Field
 from superlinked.framework.common.storage.field_data_type import FieldDataType
 from superlinked.framework.common.storage.field_type_converter import FieldTypeConverter
 
 # FieldType
 FT = TypeVar("FT")
 
@@ -29,16 +29,16 @@
 class FieldData(Field, Generic[FT]):
     def __init__(self, type_: FieldDataType, name: str, value: FT) -> None:
         super().__init__(type_, name)
         self.__validate_value(type_, value)
         self.value = value
 
     def __validate_value(self, data_type: FieldDataType, value: FT) -> None:
-        valid_type = FieldTypeConverter.get_valid_python_types(data_type)
-        if not isinstance(value, valid_type):
+        valid_types = FieldTypeConverter.get_valid_python_types(data_type)
+        if not isinstance(value, tuple(valid_types)):
             raise ValueError(
                 f"Invalid value {value} for the given field data type {data_type}"
             )
 
     @classmethod
     def from_field(cls, field: Field, value: FT) -> FieldData:
         return cls(field.data_type, field.name, value)
@@ -55,17 +55,17 @@
 
 
 class IntFieldData(FieldData[int]):
     def __init__(self, name: str, value: int) -> None:
         super().__init__(FieldDataType.INT, name, value)
 
 
-class NPArrayFieldData(FieldData[NPArray]):
-    def __init__(self, name: str, value: NPArray) -> None:
-        super().__init__(FieldDataType.NPARRAY, name, value)
+class NPArrayFieldData(FieldData[list[float]]):
+    def __init__(self, name: str, value: list[float]) -> None:
+        super().__init__(FieldDataType.FLOAT_LIST, name, value)
 
 
 class StringFieldData(FieldData[str]):
     def __init__(self, name: str, value: str) -> None:
         super().__init__(FieldDataType.STRING, name, value)
```

### Comparing `superlinked-5.4.1/superlinked/framework/common/storage/field_data_type.py` & `superlinked-5.5.1/superlinked/framework/dsl/registry/exception.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,17 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from enum import Enum
 
-
-class FieldDataType(Enum):
-    BLOB = "BLOB"
-    DOUBLE = "DOUBLE"
-    INT = "INT"
-    NPARRAY = "NPARRAY"
-    STRING = "STRING"
-    VECTOR = "VECTOR"
+class DuplicateElementException(Exception):
+    pass
```

### Comparing `superlinked-5.4.1/superlinked/framework/common/storage/field_encoder.py` & `superlinked-5.5.1/superlinked/framework/common/storage/field_encoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from abc import ABC, abstractmethod
 from typing import Any, Callable, Generic, TypeVar
 
-from superlinked.framework.common.data_types import NPArray, Vector
+from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.storage.exception import EncoderException
 from superlinked.framework.common.storage.field import Field
 from superlinked.framework.common.storage.field_data import FieldData
 from superlinked.framework.common.storage.field_data_type import FieldDataType
 
 # Encoded type
 ET = TypeVar("ET")
@@ -27,23 +27,23 @@
 
 class FieldEncoder(ABC, Generic[ET]):
     def __init__(self) -> None:
         self._encode_map: dict[FieldDataType, Callable[..., ET]] = {
             FieldDataType.BLOB: self._encode_blob,
             FieldDataType.DOUBLE: self._encode_double,
             FieldDataType.INT: self._encode_int,
-            FieldDataType.NPARRAY: self._encode_nparray,
+            FieldDataType.FLOAT_LIST: self._encode_float_list,
             FieldDataType.STRING: self._encode_string,
             FieldDataType.VECTOR: self._encode_vector,
         }
         self._decode_map: dict[FieldDataType, Callable[[ET], Any]] = {
             FieldDataType.BLOB: self._decode_blob,
             FieldDataType.DOUBLE: self._decode_double,
             FieldDataType.INT: self._decode_int,
-            FieldDataType.NPARRAY: self._decode_nparray,
+            FieldDataType.FLOAT_LIST: self._decode_float_list,
             FieldDataType.STRING: self._decode_string,
             FieldDataType.VECTOR: self._decode_vector,
         }
 
     @abstractmethod
     def _encode_blob(self, blob: str) -> ET:
         pass
@@ -65,19 +65,19 @@
         pass
 
     @abstractmethod
     def _decode_int(self, int_: ET) -> int:
         pass
 
     @abstractmethod
-    def _encode_nparray(self, nparray: NPArray) -> ET:
+    def _encode_float_list(self, float_list: list[float]) -> ET:
         pass
 
     @abstractmethod
-    def _decode_nparray(self, nparray: ET) -> NPArray:
+    def _decode_float_list(self, float_list: ET) -> list[float]:
         pass
 
     @abstractmethod
     def _encode_string(self, string: str) -> ET:
         pass
 
     @abstractmethod
```

### Comparing `superlinked-5.4.1/superlinked/framework/common/storage/field_type_converter.py` & `superlinked-5.5.1/superlinked/framework/common/storage/field_type_converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,50 +10,52 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Any, cast
 
-from superlinked.framework.common.data_types import NPArray, PythonTypes, Vector
+from beartype.typing import Sequence
+
+from superlinked.framework.common.data_types import PythonTypes, Vector
 from superlinked.framework.common.schema.schema_object import (
     Array,
     ConcreteSchemaField,
     Float,
     Integer,
     SchemaField,
     String,
     Timestamp,
 )
 from superlinked.framework.common.storage.field_data_type import FieldDataType
 from superlinked.framework.common.util.generic_class_util import GenericClassUtil
 
 FIELD_DATA_TYPE_BY_SCHEMA_FIELD_TYPE: dict[type[ConcreteSchemaField], FieldDataType] = {
-    Array: FieldDataType.NPARRAY,
+    Array: FieldDataType.FLOAT_LIST,
     Float: FieldDataType.DOUBLE,
     Integer: FieldDataType.INT,
     String: FieldDataType.STRING,
     Timestamp: FieldDataType.INT,
 }
 
 FIELD_DATA_TYPE_BY_PYTHON_TYPE: dict[type[PythonTypes], FieldDataType] = {
     float: FieldDataType.DOUBLE,
     int: FieldDataType.INT,
     str: FieldDataType.STRING,
-    NPArray: FieldDataType.NPARRAY,
+    list[float]: FieldDataType.FLOAT_LIST,
     Vector: FieldDataType.VECTOR,
 }
 
-VALID_TYPE_BY_FIELD_DATA_TYPE: dict[FieldDataType, type[PythonTypes]] = {
-    FieldDataType.BLOB: str,
-    FieldDataType.DOUBLE: float,
-    FieldDataType.INT: int,
-    FieldDataType.NPARRAY: NPArray,
-    FieldDataType.STRING: str,
-    FieldDataType.VECTOR: Vector,
+VALID_TYPE_BY_FIELD_DATA_TYPE: dict[FieldDataType, Sequence[type[PythonTypes]]] = {
+    FieldDataType.BLOB: [str],
+    FieldDataType.DOUBLE: [int, float],
+    FieldDataType.INT: [int],
+    FieldDataType.FLOAT_LIST: [list[float]],
+    FieldDataType.STRING: [str],
+    FieldDataType.VECTOR: [Vector],
 }
 
 
 class FieldTypeConverter:
     @staticmethod
     def convert_schema_field_type(
         schema_field_cls: type[SchemaField[Any]],
@@ -71,11 +73,12 @@
         if field_data_type := FIELD_DATA_TYPE_BY_PYTHON_TYPE.get(
             cast(type[PythonTypes], type_)
         ):
             return field_data_type
         raise NotImplementedError(f"Unknown python type: {type_}")
 
     @staticmethod
-    def get_valid_python_types(data_type: FieldDataType) -> type[PythonTypes]:
-        return GenericClassUtil.if_not_class_get_origin(
-            VALID_TYPE_BY_FIELD_DATA_TYPE[data_type]
-        )
+    def get_valid_python_types(data_type: FieldDataType) -> Sequence[type[PythonTypes]]:
+        return [
+            GenericClassUtil.if_not_class_get_origin(type_)
+            for type_ in VALID_TYPE_BY_FIELD_DATA_TYPE[data_type]
+        ]
```

### Comparing `superlinked-5.4.1/superlinked/framework/common/storage/persistence_type.py` & `superlinked-5.5.1/superlinked/framework/common/storage/persistence_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/storage/result_entity_data.py` & `superlinked-5.5.1/superlinked/framework/common/storage/result_entity_data.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py` & `superlinked-5.5.1/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/storage/search_index_creation/search_algorithm.py` & `superlinked-5.5.1/superlinked/framework/common/storage/search_index_creation/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py` & `superlinked-5.5.1/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/storage/vdb_connector.py` & `superlinked-5.5.1/superlinked/framework/common/storage/vdb_connector.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/storage/vdb_knn_search_params.py` & `superlinked-5.5.1/superlinked/framework/common/storage/vdb_knn_search_params.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/storage_manager/admin_fields.py` & `superlinked-5.5.1/superlinked/framework/common/storage_manager/admin_fields.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/storage_manager/entity_builder.py` & `superlinked-5.5.1/superlinked/framework/common/storage_manager/entity_builder.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/storage_manager/header.py` & `superlinked-5.5.1/superlinked/framework/common/storage_manager/header.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/storage_manager/knn_search_params.py` & `superlinked-5.5.1/superlinked/framework/common/storage_manager/knn_search_params.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,9 +23,9 @@
 from superlinked.framework.common.schema.schema_object import SchemaField
 
 
 @dataclass(frozen=True)
 class KNNSearchParams:
     vector: Vector
     limit: int | None
-    filters: Sequence[ComparisonOperation[SchemaField]] | None = None
+    filters: Sequence[ComparisonOperation[SchemaField]]
     radius: float | None = None
```

### Comparing `superlinked-5.4.1/superlinked/framework/common/storage_manager/search_result_item.py` & `superlinked-5.5.1/superlinked/framework/common/storage_manager/search_result_item.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/storage_manager/storage_manager.py` & `superlinked-5.5.1/superlinked/framework/common/storage_manager/storage_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,21 +74,23 @@
 
     def close_connection(self) -> None:
         self._vdb_connector.close_connection()
 
     def create_search_index(
         self,
         dag: Dag,
+        indexed_fields: Sequence[SchemaField],
         distance_metric: DistanceMetric = DistanceMetric.INNER_PRODUCT,
         search_algorithm: SearchAlgorithm = SearchAlgorithm.FLAT,
         vector_coordinate_type: VectorComponentPrecision = VectorComponentPrecision.FLOAT32,
     ) -> None:
         vector_index_field_descriptor, index_field_descriptors = (
             self._get_index_field_descriptors_from_dag(
                 dag,
+                indexed_fields,
                 distance_metric,
                 search_algorithm,
                 vector_coordinate_type,
             )
         )
         self._vdb_connector.create_search_index(
             self._storage_naming.get_index_name_from_index_node(dag.index_node),
@@ -126,17 +128,15 @@
             index_name,
             schema._schema_name,
             list(returned_fields.keys())
             + list(self._entity_builder._admin_fields.header_fields),
             VDBKNNSearchParams(
                 vector_field,
                 knn_search_params.limit,
-                self._compose_filter_field_data(
-                    schema, knn_search_params.filters or []
-                ),
+                self._compose_filter_field_data(schema, knn_search_params.filters),
                 knn_search_params.radius,
             ),
             **params,
         )
         schema_field_by_field_name = self._create_schema_field_by_field_name(
             returned_fields
         )
@@ -378,27 +378,27 @@
             for field_data in entity_data.field_data.values()
         }
         return node_data
 
     def _get_index_field_descriptors_from_dag(
         self,
         dag: Dag,
+        indexed_fields: Sequence[SchemaField],
         distance_metric: DistanceMetric,
         search_algorithm: SearchAlgorithm,
         vector_coordinate_type: VectorComponentPrecision,
     ) -> tuple[VectorIndexFieldDescriptor, Sequence[IndexFieldDescriptor]]:
         index_node = dag.index_node
         vector_index_field_descriptor = VectorIndexFieldDescriptor(
             index_node.node_id,
             index_node.length,
             distance_metric,
             search_algorithm,
             vector_coordinate_type,
         )
-        indexed_fields = StorageManager._get_indexed_schema_fields_of_dag(dag)
 
         return (
             vector_index_field_descriptor,
             [
                 IndexFieldDescriptor(
                     self._storage_naming.generate_field_name_from_schema_field(
                         indexed_field
@@ -423,16 +423,7 @@
     ) -> dict[str, Field]:
         return {
             key: self._entity_builder.compose_field_from_node_data_descriptor(
                 node_id, key, cast(type[PythonTypes], type_)
             )
             for key, type_ in node_data_descriptor.items()
         }
-
-    @staticmethod
-    def _get_indexed_schema_fields_of_dag(dag: Dag) -> Sequence[SchemaField]:
-        # TODO FAI-1814: this should be filtered by the soon-to-be introduced Indexed property of the SchemaField.
-        return [
-            schema_field
-            for schema in dag.schemas
-            for schema_field in schema._get_schema_fields()
-        ]
```

### Comparing `superlinked-5.4.1/superlinked/framework/common/storage_manager/storage_naming.py` & `superlinked-5.5.1/superlinked/framework/common/storage_manager/storage_naming.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/util/collection_util.py` & `superlinked-5.5.1/superlinked/framework/common/util/collection_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/util/dot_separated_path_util.py` & `superlinked-5.5.1/superlinked/framework/common/util/dot_separated_path_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/util/generic_class_util.py` & `superlinked-5.5.1/superlinked/framework/common/util/generic_class_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,24 +13,23 @@
 # limitations under the License.
 
 import inspect
 from typing import Any, cast, get_args, get_origin
 
 from beartype.typing import Sequence
 
-from superlinked.framework.common.data_types import NPArray
 from superlinked.framework.common.schema.general_type import T
 
 
 class GenericClassUtil:
     @staticmethod
     def if_not_class_get_origin(type_: type[T]) -> type:
         if inspect.isclass(type_):
             # For backward compatibility!
-            if type_ == NPArray:
+            if type_ == list[float]:
                 return type_.__origin__
             return type_
         return cast(type, get_origin(type_))
 
     @staticmethod
     def get_generic_types(object_: Any) -> Sequence[Any]:
         generic_base_class = next(
```

### Comparing `superlinked-5.4.1/superlinked/framework/common/util/immutable_model.py` & `superlinked-5.5.1/superlinked/framework/common/util/immutable_model.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/util/named_function_evaluator.py` & `superlinked-5.5.1/superlinked/framework/common/util/named_function_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/util/string_util.py` & `superlinked-5.5.1/superlinked/framework/common/util/string_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/util/time_util.py` & `superlinked-5.5.1/superlinked/framework/common/util/time_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/common/util/type_validator.py` & `superlinked-5.5.1/superlinked/framework/common/util/type_validator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/compiler/online_schema_dag_compiler.py` & `superlinked-5.5.1/superlinked/framework/compiler/online_schema_dag_compiler.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/executor/exception.py` & `superlinked-5.5.1/superlinked/framework/dsl/executor/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/executor/executor.py` & `superlinked-5.5.1/superlinked/framework/dsl/executor/executor.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py` & `superlinked-5.5.1/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
             executor (InMemoryExecutor): An instance of InMemoryExecutor.
         """
         super().__init__(
             executor,
             InMemoryVDB(),
         )
         for index in self.executor._indices:
-            self.storage_manager.create_search_index(index._dag)
+            self.storage_manager.create_search_index(index._dag, index._fields)
         self._object_writer = InMemoryObjectWriter(self._storage_manager)
         self._index_online_dag_evaluator_map = {
             index: OnlineDagEvaluator(
                 index._dag,
                 set(index._space_schemas).union(index._effect_schemas),
                 self._storage_manager,
             )
@@ -121,15 +121,18 @@
             index: QueryVectorFactory(
                 index._dag, set(index._space_schemas), self._storage_manager
             )
             for index in self.executor._indices
         }
         self._data_processors = [
             InMemoryDataProcessor(
-                self._index_online_dag_evaluator_map[index], executor._context, index
+                self._index_online_dag_evaluator_map[index],
+                self._storage_manager,
+                executor._context,
+                index,
             )
             for index in self._executor._indices
         ]
         for source in self._executor._sources:
             source._source.register(self._object_writer)
         for data_processor, index in zip(
             self._data_processors, self._executor._indices
```

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/executor/query/query_executor.py` & `superlinked-5.5.1/superlinked/framework/dsl/executor/query/query_executor.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,19 @@
     CONTEXT_COMMON_NOW,
     ExecutionContext,
     ExecutionEnvironment,
     NowStrategy,
 )
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.exception import QueryException
+from superlinked.framework.common.interface.comparison_operand import (
+    ComparisonOperation,
+)
 from superlinked.framework.common.schema.id_schema_object import IdSchemaObject
+from superlinked.framework.common.schema.schema_object import SchemaField
 from superlinked.framework.common.storage_manager.knn_search_params import (
     KNNSearchParams,
 )
 from superlinked.framework.common.storage_manager.search_result_item import (
     SearchResultItem,
 )
 from superlinked.framework.common.util import time_util
@@ -78,17 +82,19 @@
         Raises:
             QueryException: If the query index is not amongst the executor's indices.
         """
         self.__check_executor_has_index()
         param_evaluator = ParamEvaluator(params)
         limit = param_evaluator.evaluate_limit_param(self.query_obj.limit_)
         radius = param_evaluator.evaluate_radius_param(self.query_obj.radius_)
-        # TODO FAI-1838 use self.query_obj.hard_filters in self._knn_search
+        hard_filters = param_evaluator.evaluate_hard_filters_param(
+            self.query_obj.hard_filters
+        )
         entities: Sequence[SearchResultItem] = self._knn(
-            self._get_query_vector(param_evaluator), limit, radius
+            self._get_query_vector(param_evaluator), limit, radius, hard_filters
         )
         return Result(
             self.query_obj.schema,
             self._map_entities_to_result_entries(self.query_obj.schema, entities),
         )
 
     def _get_query_vector(self, param_evaluator: ParamEvaluator) -> Vector:
@@ -117,21 +123,30 @@
         )
         eval_context.update_data(
             {CONTEXT_COMMON: {CONTEXT_COMMON_NOW: self.__query_now()}}
         )
         return eval_context
 
     def _knn(
-        self, vector: Vector, limit: int | None, radius: float | None
+        self,
+        vector: Vector,
+        limit: int | None,
+        radius: float | None,
+        hard_filters: Sequence[ComparisonOperation[SchemaField]],
     ) -> Sequence[SearchResultItem]:
         return self.app.storage_manager.knn_search(
             self.query_obj.index._node,
             self.query_obj.schema,
             [],
-            KNNSearchParams(vector=vector, limit=limit, radius=radius),
+            KNNSearchParams(
+                vector=vector,
+                limit=limit,
+                filters=hard_filters,
+                radius=radius,
+            ),
         )
 
     def _map_entities_to_result_entries(
         self, schema: IdSchemaObject, result_items: Sequence[SearchResultItem]
     ) -> Sequence[ResultEntry]:
         return [
             ResultEntry(
```

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/executor/rest/rest_configuration.py` & `superlinked-5.5.1/superlinked/framework/dsl/executor/rest/rest_configuration.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/executor/rest/rest_descriptor.py` & `superlinked-5.5.1/superlinked/framework/dsl/executor/rest/rest_descriptor.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/executor/rest/rest_executor.py` & `superlinked-5.5.1/superlinked/framework/dsl/executor/rest/rest_executor.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/executor/rest/rest_handler.py` & `superlinked-5.5.1/superlinked/framework/dsl/executor/rest/rest_handler.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/index/effect.py` & `superlinked-5.5.1/superlinked/framework/dsl/index/effect.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/index/index.py` & `superlinked-5.5.1/superlinked/framework/dsl/index/index.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/index/util/aggregation_effect_group.py` & `superlinked-5.5.1/superlinked/framework/dsl/index/util/aggregation_effect_group.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/index/util/aggregation_node_util.py` & `superlinked-5.5.1/superlinked/framework/dsl/index/util/aggregation_node_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py` & `superlinked-5.5.1/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py` & `superlinked-5.5.1/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/index/util/event_aggregation_node_util.py` & `superlinked-5.5.1/superlinked/framework/dsl/index/util/event_aggregation_node_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/query/param.py` & `superlinked-5.5.1/superlinked/framework/dsl/query/param.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/query/param_evaluator.py` & `superlinked-5.5.1/superlinked/framework/dsl/query/param_evaluator.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,18 +8,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Any
+from typing import Any, cast
+
+from beartype.typing import Sequence
 
 from superlinked.framework.common.const import DEFAULT_WEIGHT
 from superlinked.framework.common.exception import QueryException
+from superlinked.framework.common.interface.comparison_operand import (
+    ComparisonOperation,
+)
+from superlinked.framework.common.schema.schema_object import SchemaField
 from superlinked.framework.dsl.query.param import (
     IntParamType,
     NumericParamType,
     Param,
     ParamInputType,
     ParamType,
 )
@@ -54,14 +60,27 @@
         value = self.evaluate_numeric_param(param, "Radius")
         if value is not None and (value > 1 or value < 0):
             raise ValueError(
                 f"Not a valid Radius value ({value}). It should be between 0 and 1."
             )
         return value
 
+    def evaluate_hard_filters_param(
+        self,
+        hard_filters: Sequence[ComparisonOperation[SchemaField]],
+    ) -> Sequence[ComparisonOperation[SchemaField]]:
+        return [
+            ComparisonOperation(
+                hard_filter._op,
+                hard_filter._operand,
+                self._evaluate_param(cast(ParamType, hard_filter._other)),
+            )
+            for hard_filter in hard_filters
+        ]
+
     def evaluate_numeric_param(
         self,
         param: NumericParamType | None,
         param_name: str,
         default: float | None = None,
     ) -> float | None:
         value = self._evaluate_param(param, default)
```

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/query/predicate/binary_op.py` & `superlinked-5.5.1/superlinked/framework/dsl/query/predicate/binary_op.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/query/predicate/binary_predicate.py` & `superlinked-5.5.1/superlinked/framework/dsl/query/predicate/binary_predicate.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/query/predicate/query_predicate.py` & `superlinked-5.5.1/superlinked/framework/dsl/query/predicate/query_predicate.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/query/query.py` & `superlinked-5.5.1/superlinked/framework/dsl/query/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from typing import Annotated, Sequence, TypedDict, cast
+from typing import Annotated, TypedDict, cast
+
+from beartype.typing import Sequence
 
 from superlinked.framework.common.const import DEFAULT_WEIGHT
 from superlinked.framework.common.exception import (
     InvalidSchemaException,
     QueryException,
 )
 from superlinked.framework.common.interface.comparison_operand import (
@@ -60,15 +62,15 @@
 class QueryObjInternalProperty(TypedDict, total=False):
     """Only intended for self initialization inside QueryObj functions, not for external initialization"""
 
     looks_like_filter: LooksLikePredicate | None
     similar_filters_by_space: dict[Space, Sequence[SimilarPredicate]]
     limit: IntParamType | None
     radius: NumericParamType | None
-    hard_filters: list[ComparisonOperation[SchemaField]]
+    hard_filters: Sequence[ComparisonOperation[SchemaField]]
     override_now: int | None
 
 
 @TypeValidator.wrap
 class QueryObj:  # pylint: disable=too-many-instance-attributes
     """
     A class representing a query object. Use .with_vector to run queries using a stored
@@ -98,17 +100,15 @@
         self.schema = cast(IdSchemaObject, schema)
         if not internal_property:
             internal_property = {}
         self.looks_like_filter = internal_property.get("looks_like_filter")
         self.similar_filters_by_space = internal_property.get(
             "similar_filters_by_space", dict[Space, Sequence[SimilarPredicate]]()
         )
-        self.hard_filters = internal_property.get(
-            "hard_filters", list[ComparisonOperation[SchemaField]]()
-        )
+        self.hard_filters = internal_property.get("hard_filters", [])
         self.limit_ = internal_property.get("limit")
         self.radius_ = internal_property.get("radius")
         # by default now in queries is the system time, but it can be overridden for testing/reproducible notebooks
         self._override_now = internal_property.get("override_now")
 
     @property
     def index(self) -> Index:
@@ -268,15 +268,15 @@
             Param,
             GenericClassUtil.get_single_generic_type(comparison_operation._operand),
         ]
         if type(comparison_operation._other) not in allowed_types:
             raise QueryException(
                 f"Unsupported filter operand type: {comparison_operation._other.__class__.__name__}."
             )
-        hard_filters = self.hard_filters.copy()
+        hard_filters = list(self.hard_filters)
         hard_filters.append(comparison_operation)
         return self.__alter({"hard_filters": hard_filters})
 
     def __is_indexed_space(self, space: Space) -> bool:
         return self.builder.index.has_space(space)
 
     def __is_space_bound(self, space: Space) -> bool:
```

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/query/query_filters.py` & `superlinked-5.5.1/superlinked/framework/dsl/query/query_filters.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/query/query_vector_factory.py` & `superlinked-5.5.1/superlinked/framework/dsl/query/query_vector_factory.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/query/query_weighting.py` & `superlinked-5.5.1/superlinked/framework/dsl/query/query_weighting.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/query/result.py` & `superlinked-5.5.1/superlinked/framework/dsl/query/result.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/registry/exception.py` & `superlinked-5.5.1/superlinked/framework/online/dag/batched_chunk_input_item.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,10 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from dataclasses import dataclass
 
-class DuplicateElementException(Exception):
-    pass
+from superlinked.framework.online.dag.parent_results import ParentResults
+
+
+@dataclass(frozen=True)
+class BatchedChunkInputItem:
+    parsed_schema_index: int
+    input_: ParentResults
```

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/registry/superlinked_registry.py` & `superlinked-5.5.1/superlinked/framework/dsl/registry/superlinked_registry.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/source/data_loader_source.py` & `superlinked-5.5.1/superlinked/framework/dsl/source/data_loader_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/source/in_memory_source.py` & `superlinked-5.5.1/superlinked/framework/dsl/source/in_memory_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/source/rest_source.py` & `superlinked-5.5.1/superlinked/framework/dsl/source/rest_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/source/source.py` & `superlinked-5.5.1/superlinked/framework/dsl/source/source.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/space/categorical_similarity_space.py` & `superlinked-5.5.1/superlinked/framework/dsl/space/categorical_similarity_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/space/custom_space.py` & `superlinked-5.5.1/superlinked/framework/dsl/space/custom_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/space/exception.py` & `superlinked-5.5.1/superlinked/framework/dsl/space/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/space/number_space.py` & `superlinked-5.5.1/superlinked/framework/dsl/space/number_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/space/recency_space.py` & `superlinked-5.5.1/superlinked/framework/dsl/space/recency_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/space/space.py` & `superlinked-5.5.1/superlinked/framework/dsl/space/space.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/space/space_field_set.py` & `superlinked-5.5.1/superlinked/framework/dsl/space/space_field_set.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/dsl/space/text_similarity_space.py` & `superlinked-5.5.1/superlinked/framework/dsl/space/text_similarity_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/evaluator/dag_evaluator.py` & `superlinked-5.5.1/superlinked/framework/evaluator/dag_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/evaluator/online_dag_evaluator.py` & `superlinked-5.5.1/superlinked/framework/evaluator/online_dag_evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         context: ExecutionContext,
     ) -> list[EvaluationResult[Vector]]:
         index_schema = self.__get_single_schema(parsed_schemas)
         if (
             online_schema_dag := self._schema_online_schema_dag_mapper.get(index_schema)
         ) is not None:
             return online_schema_dag.evaluate(parsed_schemas, context)
+
         raise InvalidSchemaException(
             f"Schema ({index_schema._schema_name}) isn't present in the index."
         )
 
     def evaluate_by_dag_effect(
         self,
         parsed_schema: ParsedSchema,
```

### Comparing `superlinked-5.4.1/superlinked/framework/evaluator/query_dag_evaluator.py` & `superlinked-5.5.1/superlinked/framework/evaluator/query_dag_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/online/dag/batched_chunk_input_item.py` & `superlinked-5.5.1/superlinked/framework/common/storage/field_data_type.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from dataclasses import dataclass
+from enum import Enum
 
-from superlinked.framework.online.dag.parent_results import ParentResults
 
-
-@dataclass(frozen=True)
-class BatchedChunkInputItem:
-    parsed_schema_index: int
-    input_: ParentResults
+class FieldDataType(Enum):
+    BLOB = "BLOB"
+    DOUBLE = "DOUBLE"
+    INT = "INT"
+    FLOAT_LIST = "FLOAT_LIST"
+    STRING = "STRING"
+    VECTOR = "VECTOR"
```

### Comparing `superlinked-5.4.1/superlinked/framework/online/dag/default_online_node.py` & `superlinked-5.5.1/superlinked/framework/online/dag/default_online_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/online/dag/evaluation_result.py` & `superlinked-5.5.1/superlinked/framework/online/dag/evaluation_result.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/online/dag/exception.py` & `superlinked-5.5.1/superlinked/framework/online/dag/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/online/dag/online_aggregation_node.py` & `superlinked-5.5.1/superlinked/framework/online/dag/online_aggregation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/online/dag/online_categorical_similarity_node.py` & `superlinked-5.5.1/superlinked/framework/online/dag/online_categorical_similarity_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/online/dag/online_chunking_node.py` & `superlinked-5.5.1/superlinked/framework/online/dag/online_chunking_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/online/dag/online_comparison_filter_node.py` & `superlinked-5.5.1/superlinked/framework/online/dag/online_comparison_filter_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/online/dag/online_concatenation_node.py` & `superlinked-5.5.1/superlinked/framework/online/dag/online_concatenation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/online/dag/online_constant_node.py` & `superlinked-5.5.1/superlinked/framework/online/dag/online_constant_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/online/dag/online_custom_node.py` & `superlinked-5.5.1/superlinked/framework/online/dag/online_custom_node.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from typing import cast
 
 from typing_extensions import override
 
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.dag.custom_node import CustomVectorEmbeddingNode
 from superlinked.framework.common.dag.node import Node
-from superlinked.framework.common.data_types import NPArray, Vector
+from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.exception import ValidationException
 from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
 from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 from superlinked.framework.online.dag.evaluation_result import EvaluationResult
 from superlinked.framework.online.dag.online_node import OnlineNode
 from superlinked.framework.online.dag.parent_validator import ParentValidationType
@@ -64,16 +64,16 @@
         parsed_schema: ParsedSchema,
         context: ExecutionContext,
     ) -> EvaluationResult[Vector]:
         if len(self.parents) == 0:
             stored_result = self.load_stored_result_or_raise_exception(parsed_schema)
             return EvaluationResult(self._get_single_evaluation_result(stored_result))
 
-        input_: EvaluationResult[NPArray] = cast(
-            OnlineNode[Node[Vector], NPArray], self.parents[0]
+        input_: EvaluationResult[list[float]] = cast(
+            OnlineNode[Node[Vector], list[float]], self.parents[0]
         ).evaluate_next_single(parsed_schema, context)
         input_value = input_.main.value
         if len(input_value) != self.length:
             raise ValidationException(
                 f"{self.class_name} can only process `Vector` inputs"
                 + f" of size {self.length}"
                 + f", got {len(input_value)}"
```

### Comparing `superlinked-5.4.1/superlinked/framework/online/dag/online_event_aggregation_node.py` & `superlinked-5.5.1/superlinked/framework/online/dag/online_event_aggregation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/online/dag/online_index_node.py` & `superlinked-5.5.1/superlinked/framework/online/dag/online_index_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/online/dag/online_named_function_node.py` & `superlinked-5.5.1/superlinked/framework/online/dag/online_named_function_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/online/dag/online_node.py` & `superlinked-5.5.1/superlinked/framework/online/dag/online_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/online/dag/online_node_registry.py` & `superlinked-5.5.1/superlinked/framework/online/dag/online_node_registry.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/online/dag/online_number_embedding_node.py` & `superlinked-5.5.1/superlinked/framework/online/dag/online_number_embedding_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/online/dag/online_recency_node.py` & `superlinked-5.5.1/superlinked/framework/online/dag/online_recency_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/online/dag/online_schema_dag.py` & `superlinked-5.5.1/superlinked/framework/online/dag/online_schema_dag.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/online/dag/online_schema_field_node.py` & `superlinked-5.5.1/superlinked/framework/online/dag/online_schema_field_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/online/dag/online_text_embedding_node.py` & `superlinked-5.5.1/superlinked/framework/online/dag/online_text_embedding_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/online/dag/parent_results.py` & `superlinked-5.5.1/superlinked/framework/online/dag/parent_results.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/online/dag/parent_validator.py` & `superlinked-5.5.1/superlinked/framework/online/dag/parent_validator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/online/source/in_memory_data_processor.py` & `superlinked-5.5.1/superlinked/framework/online/source/in_memory_data_processor.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,39 +13,49 @@
 # limitations under the License.
 
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.dag.dag_effect import DagEffect
 from superlinked.framework.common.exception import InvalidDagEffectException
 from superlinked.framework.common.observable import Subscriber
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
+from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 from superlinked.framework.dsl.index.index import Index
 from superlinked.framework.evaluator.online_dag_evaluator import OnlineDagEvaluator
 
 
 class InMemoryDataProcessor(Subscriber[ParsedSchema]):
     MAX_SAVE_DEPTH = 10
 
     def __init__(
-        self, evaluator: OnlineDagEvaluator, context: ExecutionContext, index: Index
+        self,
+        evaluator: OnlineDagEvaluator,
+        storage_manager: StorageManager,
+        context: ExecutionContext,
+        index: Index,
     ) -> None:
         super().__init__()
         self.evaluator = evaluator
         self.context = context
+        self.storage_manager = storage_manager
         self.effect_schemas = set(index._effect_schemas)
         self._schema_type_schema_mapper = index._schema_type_schema_mapper
         self._dag_effects = index._dag_effects
 
     def update(self, messages: list[ParsedSchema]) -> None:
         regular_msgs: list[ParsedSchema] = []
         for message in messages:
             if message.schema in self.effect_schemas:
                 self._process_event(message)
             else:
                 regular_msgs.append(message)
         if regular_msgs:
+            for parsed_schema in regular_msgs:
+                self.storage_manager.write_parsed_schema_fields(
+                    parsed_schema.id_, parsed_schema.fields
+                )
             self.evaluator.evaluate(regular_msgs, self.context)
 
     def _process_event(
         self,
         event_parsed_schema: ParsedSchema,
     ) -> None:
         effect_parsed_schema_map = self._map_event_parsed_schema_by_dag_effects(
```

### Comparing `superlinked-5.4.1/superlinked/framework/online/source/in_memory_object_writer.py` & `superlinked-5.5.1/superlinked/framework/online/source/in_memory_object_writer.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/online/source/in_memory_source.py` & `superlinked-5.5.1/superlinked/framework/online/source/in_memory_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/storage/in_memory/exception.py` & `superlinked-5.5.1/superlinked/framework/storage/in_memory/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/storage/in_memory/in_memory_search.py` & `superlinked-5.5.1/superlinked/framework/storage/in_memory/in_memory_search.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/storage/in_memory/in_memory_vdb.py` & `superlinked-5.5.1/superlinked/framework/storage/in_memory/in_memory_vdb.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/storage/in_memory/index_config.py` & `superlinked-5.5.1/superlinked/framework/storage/in_memory/index_config.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/storage/in_memory/json_codec.py` & `superlinked-5.5.1/superlinked/framework/storage/in_memory/json_codec.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/superlinked/framework/storage/in_memory/object_serializer.py` & `superlinked-5.5.1/superlinked/framework/storage/in_memory/object_serializer.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.4.1/PKG-INFO` & `superlinked-5.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superlinked
-Version: 5.4.1
+Version: 5.5.1
 Summary: The Superlinked vector computing library
 License: Apache-2.0
 Author: Superlinked Release
 Author-email: release@superlinked.com
 Requires-Python: >=3.10,<=3.12.3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

