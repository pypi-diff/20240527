# Comparing `tmp/vectice-24.2.6.0.tar.gz` & `tmp/vectice-24.2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectice-24.2.6.0.tar", last modified: Mon May 20 08:13:37 2024, max compression
+gzip compressed data, was "vectice-24.2.7.0.tar", last modified: Mon May 27 12:27:12 2024, max compression
```

## Comparing `vectice-24.2.6.0.tar` & `vectice-24.2.7.0.tar`

### file list

```diff
@@ -1,168 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.068563 vectice-24.2.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-20 08:13:27.000000 vectice-24.2.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-20 08:13:37.068563 vectice-24.2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-20 08:13:27.000000 vectice-24.2.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-20 08:13:27.000000 vectice-24.2.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-20 08:13:37.068563 vectice-24.2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-20 08:13:27.000000 vectice-24.2.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.028563 vectice-24.2.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.028563 vectice-24.2.6.0/src/vectice/
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.036563 vectice-24.2.6.0/src/vectice/api/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)    21452 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/gql_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/gql_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/gql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/gql_entity_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/gql_feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/gql_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/gql_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/gql_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/gql_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/gql_user_workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/http_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    13467 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/http_error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12109 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/iteration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.040563 vectice-24.2.6.0/src/vectice/api/json/
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/artifact_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/code_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/dataset_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/dataset_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/entity_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/json_to_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/json_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/model_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/model_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/model_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/organization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/paged_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/property.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/public_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/requirement.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/section.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/user_and_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.044563 vectice-24.2.6.0/src/vectice/autolog/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.044563 vectice-24.2.6.0/src/vectice/autolog/asset_services/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/asset_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/asset_services/catboost_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/asset_services/keras_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/asset_services/lightgbm_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/asset_services/metric_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/asset_services/pandas_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/asset_services/pyspark_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/asset_services/pytorch_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/asset_services/sklearn_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/asset_services/vectice_asset_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/autolog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/autolog_asset_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    31444 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/autolog_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/model_library.py
--rw-r--r--   0 runner    (1001) docker     (127)    22308 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.048563 vectice-24.2.6.0/src/vectice/models/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/additional_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/attachment_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/code_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    19022 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/model_exp_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/model_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.048563 vectice-24.2.6.0/src/vectice/models/representation/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/representation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/representation/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/representation/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/representation/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/representation/model_version_representation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.052563 vectice-24.2.6.0/src/vectice/models/resource/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/bigquery_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/databricks_table_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/file_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/gcs_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.052563 vectice-24.2.6.0/src/vectice/models/resource/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/column_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/dataframe_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/db_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/df_wrapper_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/extra_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/pyspark_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/no_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/s3_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/snowflake_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.056563 vectice-24.2.6.0/src/vectice/models/test_library/
--rw-r--r--   0 runner    (1001) docker     (127)    11948 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/test_library/binary_classification_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.056563 vectice-24.2.6.0/src/vectice/services/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/services/iteration_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/services/phase_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.056563 vectice-24.2.6.0/src/vectice/types/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.056563 vectice-24.2.6.0/src/vectice/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/utils/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/utils/code_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    15222 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/utils/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/utils/dataframe_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/utils/instance_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/utils/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/utils/vectice_ids_regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.056563 vectice-24.2.6.0/src/vectice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-20 08:13:37.000000 vectice-24.2.6.0/src/vectice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-05-20 08:13:37.000000 vectice-24.2.6.0/src/vectice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 08:13:37.000000 vectice-24.2.6.0/src/vectice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-20 08:13:37.000000 vectice-24.2.6.0/src/vectice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 08:13:37.000000 vectice-24.2.6.0/src/vectice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.893410 vectice-24.2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-27 12:27:07.000000 vectice-24.2.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-05-27 12:27:12.893410 vectice-24.2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-27 12:27:07.000000 vectice-24.2.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-27 12:27:07.000000 vectice-24.2.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 12:27:12.893410 vectice-24.2.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-27 12:27:07.000000 vectice-24.2.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.853410 vectice-24.2.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.857410 vectice-24.2.7.0/src/vectice/
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.861410 vectice-24.2.7.0/src/vectice/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23447 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/gql_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/gql_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/gql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/gql_entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/gql_feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/gql_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/gql_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/gql_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/gql_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/gql_user_workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13467 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/http_error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12109 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.869410 vectice-24.2.7.0/src/vectice/api/json/
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/artifact_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/dataset_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/dataset_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/json_to_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/json_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/model_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/model_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/model_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/organization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/paged_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/public_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/requirement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/section.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/user_and_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/json_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.869410 vectice-24.2.7.0/src/vectice/autolog/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.873410 vectice-24.2.7.0/src/vectice/autolog/asset_services/
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/asset_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/asset_services/catboost_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/asset_services/keras_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/asset_services/lightgbm_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/asset_services/metric_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/asset_services/pandas_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/asset_services/pyspark_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/asset_services/pytorch_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/asset_services/sklearn_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/asset_services/statsmodel_wrapper_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/asset_services/vectice_asset_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/autolog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/autolog_asset_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33379 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/autolog_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/autolog/model_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22308 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.873410 vectice-24.2.7.0/src/vectice/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/additional_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/attachment_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19022 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/model_exp_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/model_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.877410 vectice-24.2.7.0/src/vectice/models/representation/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/representation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/representation/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/representation/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/representation/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/representation/model_version_representation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.877410 vectice-24.2.7.0/src/vectice/models/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/bigquery_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11795 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/databricks_table_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/gcs_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.881410 vectice-24.2.7.0/src/vectice/models/resource/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/column_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/dataframe_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/db_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/df_wrapper_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/extra_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/pyspark_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/metadata/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/no_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8986 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/s3_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/resource/snowflake_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.881410 vectice-24.2.7.0/src/vectice/models/test_library/
+-rw-r--r--   0 runner    (1001) docker     (127)    11948 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/test_library/binary_classification_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.881410 vectice-24.2.7.0/src/vectice/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/services/iteration_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/services/phase_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.881410 vectice-24.2.7.0/src/vectice/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.885410 vectice-24.2.7.0/src/vectice/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/utils/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/utils/code_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15222 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/utils/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/utils/dataframe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/utils/instance_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/utils/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-27 12:27:07.000000 vectice-24.2.7.0/src/vectice/utils/vectice_ids_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:27:12.885410 vectice-24.2.7.0/src/vectice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-05-27 12:27:12.000000 vectice-24.2.7.0/src/vectice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-27 12:27:12.000000 vectice-24.2.7.0/src/vectice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:27:12.000000 vectice-24.2.7.0/src/vectice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-27 12:27:12.000000 vectice-24.2.7.0/src/vectice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 12:27:12.000000 vectice-24.2.7.0/src/vectice.egg-info/top_level.txt
```

### Comparing `vectice-24.2.6.0/LICENSE` & `vectice-24.2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/PKG-INFO` & `vectice-24.2.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 24.2.6.0
+Version: 24.2.7.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
@@ -26,15 +26,15 @@
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: types-python-dateutil
 Requires-Dist: python-dotenv>=0.11.0
-Requires-Dist: requests>=2.5.0
+Requires-Dist: requests<=2.30.0
 Requires-Dist: rich
 Requires-Dist: urllib3
 Requires-Dist: gql[requests]
 Requires-Dist: GitPython
 Requires-Dist: packaging
 Requires-Dist: Pillow
 Requires-Dist: pandas
@@ -62,15 +62,15 @@
 Requires-Dist: mkdocs-section-index>=0.3; extra == "doc"
 Requires-Dist: mkdocstrings[python]>=0.18; extra == "doc"
 Provides-Extra: test
 Requires-Dist: docker-compose; extra == "test"
 Requires-Dist: dslr[psycopg2-binary]; extra == "test"
 Requires-Dist: mock>=1.0.1; extra == "test"
 Requires-Dist: numpy; extra == "test"
-Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest==8.2.0; extra == "test"
 Requires-Dist: pytest-randomly; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pydrive2; extra == "test"
 Requires-Dist: scikit-learn; extra == "test"
 Requires-Dist: testcontainers==3.7.1; extra == "test"
 Requires-Dist: db-dtypes>=1.1.1; extra == "test"
@@ -86,25 +86,26 @@
 Requires-Dist: nbformat; extra == "test"
 Requires-Dist: lightgbm; extra == "test"
 Requires-Dist: catboost; extra == "test"
 Requires-Dist: tensorflow; extra == "test"
 Requires-Dist: keras; extra == "test"
 Requires-Dist: snowflake-snowpark-python; extra == "test"
 Requires-Dist: seaborn; extra == "test"
+Requires-Dist: statsmodels; extra == "test"
 Requires-Dist: xgboost; extra == "test"
 Requires-Dist: kaleido; extra == "test"
 Requires-Dist: catboost; extra == "test"
 Requires-Dist: torch; extra == "test"
 Provides-Extra: gcs
 Requires-Dist: google-cloud-storage>=1.17.0; extra == "gcs"
 Requires-Dist: google-cloud-bigquery; extra == "gcs"
 Provides-Extra: s3
 Requires-Dist: boto3; extra == "s3"
 Provides-Extra: validation
-Requires-Dist: shap; extra == "validation"
-Requires-Dist: scipy; extra == "validation"
+Requires-Dist: shap==0.44.1; extra == "validation"
+Requires-Dist: scipy<=1.12; extra == "validation"
 
 Auto-documentation for ML projects & their governance. View https://github.com/vectice/GettingStarted to get started.
 
 # Documentation
 
 Official documentation for Vectice can be found at https://docs.vectice.com.
```

### Comparing `vectice-24.2.6.0/pyproject.toml` & `vectice-24.2.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/setup.py` & `vectice-24.2.7.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     license="Apache License 2.0",
     keywords=["Vectice", "Client", "API", "Adapter"],
     platforms=["Linux", "MacOS X", "Windows"],
     python_requires=version_requires,
     install_requires=[
         "types-python-dateutil",
         "python-dotenv>=0.11.0",
-        "requests>=2.5.0",
+        "requests<=2.30.0",
         "rich",
         "urllib3",
         "gql[requests]",
         "GitPython",
         "packaging",
         "Pillow",
         "pandas",
@@ -71,15 +71,15 @@
             "mkdocstrings[python]>=0.18",
         ],
         "test": [
             "docker-compose",
             "dslr[psycopg2-binary]",
             "mock>=1.0.1",
             "numpy",
-            "pytest",
+            "pytest==8.2.0",
             "pytest-randomly",
             "coverage",
             "pytest-cov",
             "pydrive2",
             "scikit-learn",
             "testcontainers==3.7.1",
             "db-dtypes>=1.1.1",
@@ -95,22 +95,23 @@
             "nbformat",
             "lightgbm",
             "catboost",
             "tensorflow",
             "keras",
             "snowflake-snowpark-python",
             "seaborn",
+            "statsmodels",
             "xgboost",
             "kaleido",
             "catboost",
             "torch",
         ],
         "gcs": ["google-cloud-storage>=1.17.0", "google-cloud-bigquery"],
         "s3": ["boto3"],
-        "validation": ["shap", "scipy"],
+        "validation": ["shap==0.44.1", "scipy<=1.12"],
     },
     classifiers=[
         "Topic :: Internet",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
```

### Comparing `vectice-24.2.6.0/src/vectice/__init__.py` & `vectice-24.2.7.0/src/vectice/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/_auth.py` & `vectice-24.2.7.0/src/vectice/api/_auth.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/attachment.py` & `vectice-24.2.7.0/src/vectice/api/attachment.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/client.py` & `vectice-24.2.7.0/src/vectice/api/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 from vectice.api.workspace import WorkspaceApi
 from vectice.models.dataset import Dataset
 from vectice.models.iteration import Iteration
 from vectice.models.model import Model
 from vectice.models.phase import Phase
 from vectice.models.representation.dataset_version_representation import DatasetVersionRepresentation
 from vectice.models.representation.model_version_representation import ModelVersionRepresentation
-from vectice.models.resource.metadata.base import MetadataSettings
+from vectice.models.resource.metadata.base import DatasetSourceType, MetadataSettings
 from vectice.models.table import Table
 from vectice.types.version import TVersion
 from vectice.utils.vectice_ids_regex import WORKSPACE_VID_REG
 
 if TYPE_CHECKING:
     from io import BytesIO, IOBase
 
@@ -370,37 +370,54 @@
         section: str | None = None,
     ) -> DatasetRegisterOutput:
         if dataset._has_snowflake_resource:  # pyright: ignore[reportPrivateUsage]
             self.assert_feature_flag_or_raise("snowflake-resource")
 
         name = self.get_dataset_name(dataset)
         derived_from = self.get_derived_from(dataset)
-        metadata_asdict = self._transform_resource_to_metadata_dict(dataset)
+        metadata_asdict, is_updating_columns = self._transform_resource_to_metadata_dict(dataset)
         properties, _ = self.get_properties_and_metrics(dataset)
 
         dataset_register_input = DatasetRegisterInput(
             name=name,
             type=dataset.type.value,
             datasetSources=metadata_asdict,
             inputs=derived_from,
             codeVersion=code_version.asdict() if code_version is not None else None,
             properties=properties,
         )
 
         iteration_context = IterationContextInput(iterationId=iteration_id, stepName=section)
         dataset_register_output = self.register_dataset(dataset_register_input, iteration_context=iteration_context)
-        dataset.latest_version_id = dataset_register_output["datasetVersion"]["vecticeId"]
+        dtv_id = dataset_register_output["datasetVersion"]["vecticeId"]
+
+        if is_updating_columns:
+            self.warn_if_dataset_version_columns_are_missing_description(dtv_id)
+
+        dataset.latest_version_id = dtv_id
         return dataset_register_output
 
+    def warn_if_dataset_version_columns_are_missing_description(self, dataset_version_id: str):
+        has_columns_without_description = GqlDatasetApi(
+            self._gql_client, self.auth
+        ).get_dataset_version_has_columns_without_description(dataset_version_id)
+        if has_columns_without_description is True:
+            _logger.warning(
+                "Some column descriptions are missing. Consider adding descriptions for improved data clarity."
+            )
+
     def get_dataset(self, id: str) -> DatasetRepresentationOutput:
         return GqlDatasetApi(self._gql_client, self.auth).get_dataset(id)
 
     def get_dataset_version(self, id: str) -> DatasetVersionRepresentationOutput:
         return GqlDatasetApi(self._gql_client, self.auth).get_dataset_version(id)
 
+    def update_dataset_version(self, id: str, columns_description: list[dict[str, str]]):
+        return GqlDatasetApi(self._gql_client, self.auth).update_dataset_version(id, columns_description)
+
     def get_model(self, id: str) -> ModelRepresentationOutput:
         return GqlModelApi(self._gql_client, self.auth).get_model(id)
 
     def get_model_version_list(self, id: str, size: int) -> PagedResponse[ModelVersionRepresentationOutput]:
         return GqlModelApi(self._gql_client, self.auth).get_model_version_list(id, size)
 
     def get_model_version(self, id: str) -> ModelVersionRepresentationOutput:
@@ -429,26 +446,49 @@
         metrics = (
             [vars(MetricInput(met.key, met.value)) for met in obj.metrics]
             if (isinstance(obj, Model) and obj.metrics)
             else None
         )
         return properties, metrics
 
-    def _transform_resource_to_metadata_dict(self, dataset: Dataset) -> list[dict[str, Any]]:
+    def _transform_resource_to_metadata_dict(self, dataset: Dataset):
         resources = dataset.resource if isinstance(dataset.resource, tuple) else [dataset.resource]
         metadata_asdict = []
+        is_updating_columns = False
         for resource in resources:
             if resource is not None and resource.metadata:
                 resource.metadata.set_settings(
                     MetadataSettings(
                         minimum_rows_for_statistics=self._org_config.configuration.df_statistics_row_threshold
                     )
                 )
-                metadata_asdict.append(resource.metadata.asdict())
-        return metadata_asdict
+
+                metadata, columns_description = resource.metadata, resource.columns_description
+                is_updating_columns = is_updating_columns is False and columns_description is not None
+                columns = columns_description or {}
+                metadata_dict, type = metadata.asdict(), metadata.type
+                if type == DatasetSourceType.DB:
+                    for db in metadata_dict["dbs"]:
+                        db["columns"] = self._combine_source_column_description(db, columns)
+                else:
+                    for file in metadata_dict["files"]:
+                        file["columns"] = self._combine_source_column_description(file, columns)
+
+                metadata_asdict.append(metadata_dict)
+        return metadata_asdict, is_updating_columns
+
+    def _combine_source_column_description(self, source: dict, columns_description: dict[str, str]):
+        def _map_columns(col: dict):
+            col_name = col["name"]
+            if col_name in columns_description:
+                column_desc = columns_description[col_name]
+                return {**col, "description": column_desc}
+            return col
+
+        return list(map(_map_columns, source["columns"]))
 
     def register_dataset(
         self,
         dataset_register_input: DatasetRegisterInput,
         iteration_context: IterationContextInput,
     ) -> DatasetRegisterOutput:
         data: DatasetRegisterOutput = GqlDatasetApi(self._gql_client, self.auth).register_dataset(
```

### Comparing `vectice-24.2.6.0/src/vectice/api/gql_api.py` & `vectice-24.2.7.0/src/vectice/api/gql_api.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/gql_attachment.py` & `vectice-24.2.7.0/src/vectice/api/gql_attachment.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/gql_dataset.py` & `vectice-24.2.7.0/src/vectice/api/gql_dataset.py`

 * *Files 23% similar despite different names*

```diff
@@ -89,14 +89,20 @@
                 key
                 value
             }
             __typename
 """
 
 
+_RETURNS_EMPTY_DATASET_VERSION = """
+            vecticeId
+            __typename
+"""
+
+
 class GqlDatasetApi(GqlApi):
     def get_dataset(self, id: str) -> DatasetRepresentationOutput:
         variable_types = "$datasetId:VecticeId!"
         kw = "datasetId:$datasetId"
         variables = {"datasetId": id}
         query = GqlApi.build_query(
             gql_query="getDataset",
@@ -126,14 +132,30 @@
         try:
             response = self.execute(query_built, variables)
             dataset_output: DatasetVersionRepresentationOutput = Parser().parse_item(response["getDatasetVersion"])
             return dataset_output
         except TransportQueryError as e:
             self._error_handler.handle_post_gql_error(e, "dataset_version", id)
 
+    def get_dataset_version_has_columns_without_description(self, id: str) -> bool:
+        variable_types = "$datasetVersionId:VecticeId!"
+        kw = "datasetVersionId:$datasetVersionId"
+        variables = {"datasetVersionId": id}
+        query = GqlApi.build_query(
+            gql_query="getDatasetVersion",
+            variable_types=variable_types,
+            returns="hasColumnWithoutDescription",
+            keyword_arguments=kw,
+        )
+        query_built = gql(query)
+        try:
+            return self.execute(query_built, variables)["getDatasetVersion"]["hasColumnWithoutDescription"]
+        except TransportQueryError as e:
+            self._error_handler.handle_post_gql_error(e, "dataset_version", id)
+
     def register_dataset(
         self,
         data: DatasetRegisterInput,
         iteration_context: IterationContextInput,
     ) -> DatasetRegisterOutput:
         variables: dict[str, Any] = {"iterationContext": iteration_context, "data": data}
         kw = "iterationContext:$iterationContext,data:$data"
@@ -149,7 +171,24 @@
         query_built = gql(query)
         try:
             response = self.execute(query_built, variables)
             dataset_output: DatasetRegisterOutput = Parser().parse_item(response["registerDataset"])
             return dataset_output
         except TransportQueryError as e:
             self._error_handler.handle_post_gql_error(e, "dataset", "register dataset")
+
+    def update_dataset_version(self, id: str, columns_description: list[dict[str, str]]):
+        variable_types = "$datasetVersionId:VecticeId!,$data:DatasetVersionUpdateInput!"
+        kw = "datasetVersionId:$datasetVersionId,data:$data"
+        variables = {"datasetVersionId": id, "data": {"columnsDescription": columns_description}}
+        query = GqlApi.build_query(
+            gql_query="updateDatasetVersion",
+            variable_types=variable_types,
+            returns=_RETURNS_EMPTY_DATASET_VERSION,
+            keyword_arguments=kw,
+            query=False,
+        )
+        query_built = gql(query)
+        try:
+            self.execute(query_built, variables)
+        except TransportQueryError as e:
+            self._error_handler.handle_post_gql_error(e, "dataset_version", id)
```

### Comparing `vectice-24.2.6.0/src/vectice/api/gql_entity_file.py` & `vectice-24.2.7.0/src/vectice/api/gql_entity_file.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/gql_feature_flag.py` & `vectice-24.2.7.0/src/vectice/api/gql_feature_flag.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/gql_metric.py` & `vectice-24.2.7.0/src/vectice/api/gql_metric.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/gql_model.py` & `vectice-24.2.7.0/src/vectice/api/gql_model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/gql_organization.py` & `vectice-24.2.7.0/src/vectice/api/gql_organization.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/gql_property.py` & `vectice-24.2.7.0/src/vectice/api/gql_property.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/gql_user_workspace_api.py` & `vectice-24.2.7.0/src/vectice/api/gql_user_workspace_api.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/http_error.py` & `vectice-24.2.7.0/src/vectice/api/http_error.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/http_error_handlers.py` & `vectice-24.2.7.0/src/vectice/api/http_error_handlers.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/iteration.py` & `vectice-24.2.7.0/src/vectice/api/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/__init__.py` & `vectice-24.2.7.0/src/vectice/api/json/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/artifact_version.py` & `vectice-24.2.7.0/src/vectice/api/json/artifact_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/code.py` & `vectice-24.2.7.0/src/vectice/api/json/code.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/code_version.py` & `vectice-24.2.7.0/src/vectice/api/json/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/dataset_register.py` & `vectice-24.2.7.0/src/vectice/api/json/dataset_register.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/dataset_representation.py` & `vectice-24.2.7.0/src/vectice/api/json/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/dataset_version.py` & `vectice-24.2.7.0/src/vectice/api/json/dataset_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/dataset_version_representation.py` & `vectice-24.2.7.0/src/vectice/api/json/dataset_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/files_metadata.py` & `vectice-24.2.7.0/src/vectice/api/json/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/iteration.py` & `vectice-24.2.7.0/src/vectice/api/json/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/json_to_class.py` & `vectice-24.2.7.0/src/vectice/api/json/json_to_class.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/last_assets.py` & `vectice-24.2.7.0/src/vectice/api/json/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/metric.py` & `vectice-24.2.7.0/src/vectice/api/json/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/model.py` & `vectice-24.2.7.0/src/vectice/api/json/model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/model_register.py` & `vectice-24.2.7.0/src/vectice/api/json/model_register.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/model_representation.py` & `vectice-24.2.7.0/src/vectice/api/json/model_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/model_version.py` & `vectice-24.2.7.0/src/vectice/api/json/model_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/model_version_representation.py` & `vectice-24.2.7.0/src/vectice/api/json/model_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/paged_response.py` & `vectice-24.2.7.0/src/vectice/api/json/paged_response.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/phase.py` & `vectice-24.2.7.0/src/vectice/api/json/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/project.py` & `vectice-24.2.7.0/src/vectice/api/json/project.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/property.py` & `vectice-24.2.7.0/src/vectice/api/json/property.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/public_config.py` & `vectice-24.2.7.0/src/vectice/api/json/public_config.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/requirement.py` & `vectice-24.2.7.0/src/vectice/api/json/requirement.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/user_and_workspace.py` & `vectice-24.2.7.0/src/vectice/api/json/user_and_workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/json/workspace.py` & `vectice-24.2.7.0/src/vectice/api/json/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/phase.py` & `vectice-24.2.7.0/src/vectice/api/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/project.py` & `vectice-24.2.7.0/src/vectice/api/project.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/rest_api.py` & `vectice-24.2.7.0/src/vectice/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/version.py` & `vectice-24.2.7.0/src/vectice/api/version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/api/workspace.py` & `vectice-24.2.7.0/src/vectice/api/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/autolog/asset_services/__init__.py` & `vectice-24.2.7.0/src/vectice/autolog/asset_services/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from vectice.autolog.asset_services.catboost_service import AutologCatboostService
 from vectice.autolog.asset_services.keras_service import AutologKerasService
 from vectice.autolog.asset_services.lightgbm_service import AutologLightgbmService
 from vectice.autolog.asset_services.pandas_service import AutologPandasService
 from vectice.autolog.asset_services.pyspark_service import AutologPysparkService
 from vectice.autolog.asset_services.pytorch_service import AutologPytorchService
 from vectice.autolog.asset_services.sklearn_service import AutologSklearnService
+from vectice.autolog.asset_services.statsmodel_wrapper_service import AutologStatsModelWrapperService
 from vectice.autolog.asset_services.vectice_asset_service import (
     AutologVecticeAssetService,
     TVecticeObjects,
     VecticeObjectClasses,
     VecticeObjectTypes,
 )
 
@@ -16,12 +17,13 @@
     "AutologPandasService",
     "AutologPysparkService",
     "AutologPytorchService",
     "AutologCatboostService",
     "AutologKerasService",
     "AutologLightgbmService",
     "AutologSklearnService",
+    "AutologStatsModelWrapperService",
     "AutologVecticeAssetService",
     "TVecticeObjects",
     "VecticeObjectTypes",
     "VecticeObjectClasses",
 ]
```

### Comparing `vectice-24.2.6.0/src/vectice/autolog/asset_services/catboost_service.py` & `vectice-24.2.7.0/src/vectice/autolog/asset_services/catboost_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/autolog/asset_services/keras_service.py` & `vectice-24.2.7.0/src/vectice/autolog/asset_services/keras_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/autolog/asset_services/lightgbm_service.py` & `vectice-24.2.7.0/src/vectice/autolog/asset_services/lightgbm_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/autolog/asset_services/pytorch_service.py` & `vectice-24.2.7.0/src/vectice/autolog/asset_services/pytorch_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/autolog/asset_services/sklearn_service.py` & `vectice-24.2.7.0/src/vectice/autolog/asset_services/sklearn_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/autolog/asset_services/vectice_asset_service.py` & `vectice-24.2.7.0/src/vectice/autolog/asset_services/vectice_asset_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/autolog/autolog.py` & `vectice-24.2.7.0/src/vectice/autolog/autolog.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/autolog/autolog_asset_factory.py` & `vectice-24.2.7.0/src/vectice/autolog/autolog_asset_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     AutologCatboostService,
     AutologKerasService,
     AutologLightgbmService,
     AutologPandasService,
     AutologPysparkService,
     AutologPytorchService,
     AutologSklearnService,
+    AutologStatsModelWrapperService,
     AutologVecticeAssetService,
     VecticeObjectClasses,
 )
 
 
 class IAutologService(Protocol):
     @abstractmethod
@@ -28,14 +29,15 @@
     def get_asset_service(key: str, asset: Any, data: dict) -> IAutologService:
         is_pandas = find_spec("pandas") is not None
         is_pyspark = find_spec("pyspark") is not None
         is_lgbm = find_spec("lightgbm") is not None
         is_sklearn = find_spec("sklearn") is not None
         is_catboost = find_spec("catboost") is not None
         is_keras = find_spec("keras") is not None
+        is_statsmodels = find_spec("statsmodels") is not None
         is_pytorch = find_spec("torch") is not None
 
         if is_pandas:
             from pandas import DataFrame
 
             if isinstance(asset, DataFrame):
                 return AutologPandasService(key, asset)
@@ -69,11 +71,17 @@
 
             if isinstance(asset, Module):
                 return AutologPytorchService(key, asset, data)
 
         if isinstance(asset, VecticeObjectClasses):
             return AutologVecticeAssetService(key, asset)  # type: ignore[reportArgumentType]
 
+        if is_statsmodels:
+            from statsmodels.base.wrapper import ResultsWrapper
+
+            if isinstance(asset, ResultsWrapper):
+                return AutologStatsModelWrapperService(key, asset, data)
+
         if is_sklearn:
             return AutologSklearnService(key, asset, data)
 
         raise VecticeException(f"Asset {asset} of type ({type(asset)!r}) not handled")
```

### Comparing `vectice-24.2.6.0/src/vectice/autolog/autolog_class.py` & `vectice-24.2.7.0/src/vectice/autolog/autolog_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import ast
 import logging
 import os
 import re
 import tempfile
-from ast import literal_eval
 from base64 import b64decode
 from collections import OrderedDict
 from importlib.util import find_spec
 from io import BytesIO
 from typing import TYPE_CHECKING, Any, TypeVar
 
 import PIL.Image as Image
@@ -29,14 +28,15 @@
     from catboost.core import CatBoost
     from keras import Model as KerasModel  # type: ignore[reportMissingImports]
     from keras.layers import InputLayer  # type: ignore[reportMissingImports]
     from lightgbm.basic import Booster
     from pandas import DataFrame
     from pyspark.sql import DataFrame as SparkDF
     from sklearn.base import BaseEstimator
+    from statsmodels.base.wrapper import ResultsWrapper
     from torch.nn import Module as TorchModel
 
     # Vectice Object types
     from vectice.autolog.asset_services import TVecticeObjects
     from vectice.models import Phase
     from vectice.models.resource.metadata.db_metadata import TableType
 
@@ -136,15 +136,15 @@
         # get commented lines and not lines with comments
         lines = cell_content.split("\n")
         matched_lines = "\n".join(
             [line for line in lines if (remove and re.search(r"^#.*", line)) or not re.search(r"^#.*", line)]
         )
         cell = preprocess_code(matched_lines)
         tree = ast.parse(cell)
-        visitor = FilePathVisitor()
+        visitor = FilePathVisitor(is_graph_path=True)
         visitor.visit(tree)
 
         graph_paths = []
         for graph in visitor.file_paths:
             if is_valid_matplotlib_extension(graph) and "http" not in graph:
                 graph_paths.append(graph)
         return graph_paths
@@ -546,26 +546,39 @@
     def _get_catboost_info(self, model: CatBoost) -> tuple[str, dict[str, Any]] | tuple[None, None]:
         try:
             params = {str(key): value for key, value in model.get_all_params().items() if value is not None}
             return "catboost", params
         except AttributeError:
             return None, None
 
+    def _get_statsmodel_info(self, model: ResultsWrapper) -> tuple[str, dict[str, Any]] | tuple[None, None]:
+        try:
+            # model params
+            model_params = {"model_type": model.model.__class__.__name__, "formula": model.model.formula}
+            # statsmodels fitted/Resultswrapper
+            params = {str(key): value for key, value in model.params.items() if value is not None}
+            model_params.update(params)
+            return "statsmodel", model_params
+        except AttributeError:
+            return None, None
+
     def _get_model_params(self, asset: TModel) -> tuple[str, dict[str, Any]] | tuple[None, None]:
         library = asset["library"]
         model = asset["model"]
 
         if library is ModelLibrary.SKLEARN:
             return self._get_sklearn_or_xgboost_or_lgbm_info(model)  # pyright: ignore[reportArgumentType]
         if library is ModelLibrary.LIGHTGBM:
             return self._get_lightgbm_info(model)  # pyright: ignore[reportArgumentType]
         if library is ModelLibrary.CATBOOST:
             return self._get_catboost_info(model)  # pyright: ignore[reportArgumentType]
         if library is ModelLibrary.KERAS:
             return self._get_keras_info(model)  # pyright: ignore[reportArgumentType]
+        if library is ModelLibrary.STATSMODEL:
+            return self._get_statsmodel_info(model)  # pyright: ignore[reportArgumentType]
         if library is ModelLibrary.PYTORCH:
             return self._get_pytorch_info(model)  # pyright: ignore[reportArgumentType]
         return None, None
 
     def _check_for_single_model(self):
         model_list = [asset for asset in self._assets if "model" in asset]
         if len(model_list) > 1:
@@ -606,34 +619,45 @@
                     )
 
             except Exception as e:
                 _logger.info(
                     f"Unable to generate the model plot. Ensure that the Keras library is correctly installed and up-to-date. Error details: {e}"
                 )
 
+        model_object = model["model"]
+
         library, params = self._get_model_params(model)
+        if model["library"] is ModelLibrary.STATSMODEL:
+            algorithm = str(model_object.model.__class__).split(".")[-1]  # type: ignore[reportAttributeAccessIssue]
+            model_summary = model_object.summary().as_text()  # type: ignore[reportAttributeAccessIssue]
+        else:
+            algorithm = str(model_object.__class__).split(".")[-1]
+            model_summary = None
 
-        algorithm = str(model["model"].__class__).split(".")[-1]
         algorithm = algorithm.replace("'>", "")
         model_name = f"{self._iteration.phase.id}-{model['variable']}"
         # safety check, if no metrics and single model, get metrics
         model_metrics = model["metrics"] if model["metrics"] else self._get_single_model_metrics()
         self._iteration_service.log_model(
             Model(
                 library=library,
                 technique=algorithm,
                 metrics=model_metrics,
                 properties=params,
                 name=model_name,
-                predictor=model["model"],
+                predictor=model_object,
                 attachments=temp_file_path,
             )
         )
         _logger.info(f"Model {model_name!r} logged in iteration {self._iteration.name!r}.")
 
+        if model_summary:
+            # log statsmodel summary
+            self._iteration_service.log_comment(model_summary)
+
         if temp_dir is not None:
             temp_dir.cleanup()
 
     def _log_vectice_asset(self, asset: TVecticeObjects) -> None:
         asset_to_log = asset["vectice_object"]
         asset_name = asset["variable"]
         if isinstance(asset_to_log, Dataset):
@@ -688,22 +712,38 @@
     def _get_dataset_resource(self, dataset: TDataset) -> str | None:
         import re
 
         if not self._cell_content:
             return None
         try:
             # Avoid getting stray dataset with autolog.notebook()
+
             match = []
             for cell in self._cell_content:
-                match += re.findall(rf"(?<={dataset['variable']} = pd.read_csv\().*[^,)\n]", cell)
+                cell = preprocess_code(cell)
+                tree = ast.parse(cell)
+                visitor = FilePathVisitor(is_dataset_path=True)
+                visitor.visit(tree)
+                for resource_info in visitor.dataset_file_paths:
+                    path_var, file_path = resource_info["variable"], resource_info["path"]
+                    dataset_variable = re.escape(dataset["variable"])
+                    if path_var:
+                        pattern = rf"{dataset_variable}\s*=\s*pd\.read_csv\(\s*{path_var}\s*\).*\n"
+                    else:
+                        regex_path = re.escape(file_path)
+                        pattern = rf"{dataset_variable}\s*=\s*pd\.read_csv\(.*?{regex_path}.*?\).*\n"
+                    match_dataset_path = re.search(pattern, cell)
+                    if match_dataset_path:
+                        match.append(file_path)
+
             if len(match) < 1:
                 return None
             # TODO update regex
             # check if read csv has comma dominated arguments
-            return literal_eval(match[0].split(",")[0]) if match[0].find(",") else literal_eval(match[0])
+            return match[0]
         except TypeError:
             return None
 
     def _get_image_data(self, graph: str) -> str | None:
         try:
             captured = self._local_vars[graph]
         except KeyError:
```

### Comparing `vectice-24.2.6.0/src/vectice/connection.py` & `vectice-24.2.7.0/src/vectice/connection.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/__init__.py` & `vectice-24.2.7.0/src/vectice/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/additional_info.py` & `vectice-24.2.7.0/src/vectice/models/additional_info.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/attachment_container.py` & `vectice-24.2.7.0/src/vectice/models/attachment_container.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/code_version.py` & `vectice-24.2.7.0/src/vectice/models/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/dataset.py` & `vectice-24.2.7.0/src/vectice/models/dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/iteration.py` & `vectice-24.2.7.0/src/vectice/models/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/metric.py` & `vectice-24.2.7.0/src/vectice/models/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/model.py` & `vectice-24.2.7.0/src/vectice/models/model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/model_exp_tracker.py` & `vectice-24.2.7.0/src/vectice/models/model_exp_tracker.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/model_mlflow.py` & `vectice-24.2.7.0/src/vectice/models/model_mlflow.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/phase.py` & `vectice-24.2.7.0/src/vectice/models/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/project.py` & `vectice-24.2.7.0/src/vectice/models/project.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/property.py` & `vectice-24.2.7.0/src/vectice/models/property.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/representation/dataset_representation.py` & `vectice-24.2.7.0/src/vectice/models/representation/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/representation/dataset_version_representation.py` & `vectice-24.2.7.0/src/vectice/models/representation/dataset_version_representation.py`

 * *Files 13% similar despite different names*

```diff
@@ -107,33 +107,45 @@
             }
         return flattened_resource
 
     def update(
         self,
         properties: dict[str, str | int] | list[Property] | Property | None = None,
         attachments: str | list[str] | None = None,
+        columns_description: dict[str, str] | None = None,
     ) -> None:
         """Update the Dataset Version from the API.
 
         Parameters:
             properties: The new properties of the dataset.
             attachments: The new attachments of the dataset.
+            columns_description: A dictionary to map the column's name to a specific description. Should follow the format { "column_name": "Description", ... }
 
         Returns:
             None
         """
         if properties is not None:
             self._upsert_properties(properties)
 
         if attachments is not None:
             self._update_attachments(attachments)
 
+        if columns_description is not None:
+            self._update_dataset_version(columns_description)
+
     def _upsert_properties(self, properties: dict[str, str | int] | list[Property] | Property):
         clean_properties = list(map(lambda property: property.key_val_dict(), format_properties(properties)))
         new_properties = self._client.upsert_properties("dataSetVersion", self.id, clean_properties)
         self.properties = strip_dict_list(new_properties)
         _logger.info(f"Dataset version {self.id!r} properties successfully updated.")
 
     def _update_attachments(self, attachments: TAttachment):
         container = AttachmentContainer(self._output, self._client)
         container.upsert_attachments(format_attachments(attachments))
         _logger.info(f"Dataset version {self.id!r} attachments successfully updated.")
+
+    def _update_dataset_version(self, columns_description: dict[str, str]):
+        items = columns_description.items()
+        list_columns_description = list(map(lambda x: {"name": x[0], "description": x[1]}, items))
+        self._client.update_dataset_version(self.id, list_columns_description)
+        self._client.warn_if_dataset_version_columns_are_missing_description(self.id)
+        _logger.info(f"Dataset version {self.id!r} columns descriptions successfully updated.")
```

### Comparing `vectice-24.2.6.0/src/vectice/models/representation/model_representation.py` & `vectice-24.2.7.0/src/vectice/models/representation/model_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/representation/model_version_representation.py` & `vectice-24.2.7.0/src/vectice/models/representation/model_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/resource/__init__.py` & `vectice-24.2.7.0/src/vectice/models/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/resource/base.py` & `vectice-24.2.7.0/src/vectice/models/resource/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 
     @abstractmethod
     def __init__(
         self,
         paths: list[str] | str,
         dataframes: TDataFrameType | list[TDataFrameType] | None = None,
         capture_schema_only: bool = False,
+        columns_description: dict[str, str] | None = None,
     ):
         """Initialize a resource."""
         self._metadata: Metadata | None = None
         self._data: dict | None = None
         if paths:
             self._paths = paths if isinstance(paths, list) else [paths]
         else:
@@ -89,14 +90,16 @@
                 if dataframe is not None and not isinstance(  # pyright: ignore[reportUnnecessaryComparison]
                     dataframe, get_args(DataFrameType)
                 ):
                     raise ValueError(
                         f"Argument 'dataframe' of type '{type(dataframe)}' is invalid, only Pandas or Spark DataFrame are supported."
                     )
 
+        self.columns_description = columns_description
+
     @property
     def data(self) -> dict:
         """The resource's data.
 
         Returns:
             The resource's data.
         """
```

### Comparing `vectice-24.2.6.0/src/vectice/models/resource/bigquery_resource.py` & `vectice-24.2.7.0/src/vectice/models/resource/bigquery_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,25 +42,32 @@
 
     def __init__(
         self,
         paths: str | list[str],
         dataframes: TDataFrameType | list[TDataFrameType] | None = None,
         bq_client: BQClient | None = None,
         capture_schema_only: bool = False,
+        columns_description: dict[str, str] | None = None,
     ):
         """Initialize a BigQuery resource.
 
         Parameters:
             paths: The paths to retrieve the datasets or the tables.
             dataframes (Optional): The dataframes allowing vectice to optionally compute more metadata about this resource such as columns stats. (Support Pandas, Spark)
             bq_client (Optional): The `google.cloud.bigquery.Client` to optionally retrieve file size, creation date and updated date (used for auto-versioning).
             capture_schema_only (Optional): A boolean parameter indicating whether to capture only the schema or both the schema and column statistics of the dataframes.
+            columns_description (Optional): A dictionary to map the column's name to a specific description. Should follow the format { "column_name": "Description", ... }
 
         """
-        super().__init__(paths=paths, dataframes=dataframes, capture_schema_only=capture_schema_only)
+        super().__init__(
+            paths=paths,
+            dataframes=dataframes,
+            capture_schema_only=capture_schema_only,
+            columns_description=columns_description,
+        )
         self.bq_client = bq_client
 
     def _fetch_data(self) -> dict[str, tuple[Table | None, TDataFrameType | None]]:
         tables: dict[str, tuple[Table | None, TDataFrameType | None]] = {}
         df_index = 0
         for path in self._paths:
             path_tables, new_df_index = self._fetch_path_data(index=df_index, path=path)
```

### Comparing `vectice-24.2.6.0/src/vectice/models/resource/databricks_table_resource.py` & `vectice-24.2.7.0/src/vectice/models/resource/databricks_table_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,26 +51,33 @@
 
     def __init__(
         self,
         paths: str | list[str],
         dataframes: TDataFrameType | list[TDataFrameType] | None = None,
         spark_client: SparkSession | None = None,
         capture_schema_only: bool = False,
+        columns_description: dict[str, str] | None = None,
     ):
         """Initialize a DatabricksTableResource resource.
 
         Parameters:
             paths: The paths to retrieve the tables. Should be either the table name or the location of the table.
             dataframes (Optional): The dataframes allowing vectice to optionally compute more metadata about this resource such as columns stats. (Support Pandas, Spark)
             spark_client (Optional): The spark session allowing vectice to capture the table metadata.
             capture_schema_only (Optional): A boolean parameter indicating whether to capture only the schema or both the schema and column statistics of the dataframes.
+            columns_description (Optional): A dictionary to map the column's name to a specific description. Should follow the format { "column_name": "Description", ... }
         """
         if spark_imported is False:
             raise ImportError("Pyspark is not installed.")
-        super().__init__(paths=paths, dataframes=dataframes, capture_schema_only=capture_schema_only)
+        super().__init__(
+            paths=paths,
+            dataframes=dataframes,
+            capture_schema_only=capture_schema_only,
+            columns_description=columns_description,
+        )
         self._spark_client = spark_client
 
     def _fetch_data(self):
         tables: dict[str, tuple[dict | None, TDataFrameType | None]] = {}
         df_index = 0
         for path in self._paths:
             path_tables, new_df_index = self._fetch_table_data(index=df_index, path=path)
```

### Comparing `vectice-24.2.6.0/src/vectice/models/resource/description.py` & `vectice-24.2.7.0/src/vectice/models/resource/description.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/resource/file_resource.py` & `vectice-24.2.7.0/src/vectice/models/resource/file_resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,32 +35,39 @@
     _origin = DatasetSourceOrigin.LOCAL.value
 
     def __init__(
         self,
         paths: str | list[str],
         dataframes: TDataFrameType | list[TDataFrameType] | None = None,
         capture_schema_only: bool = False,
+        columns_description: dict[str, str] | None = None,
     ):
         """Initialize a file resource.
 
         Parameters:
             paths: The paths of the files to wrap.
             dataframes (Optional): The dataframes allowing vectice to optionally compute more metadata about this resource such as columns stats. (Support Pandas, Spark)
             capture_schema_only (Optional): A boolean parameter indicating whether to capture only the schema or both the schema and column statistics of the dataframes.
+            columns_description (Optional): A dictionary to map the column's name to a specific description. Should follow the format { "column_name": "Description", ... }
 
         Examples:
             The following example shows how to wrap a CSV file
             called `iris.csv` in the current directory:
 
             ```python
             from vectice import FileResource
             iris_trainset = FileResource(paths="iris.csv")
             ```
         """
-        super().__init__(paths=paths, dataframes=dataframes, capture_schema_only=capture_schema_only)
+        super().__init__(
+            paths=paths,
+            dataframes=dataframes,
+            capture_schema_only=capture_schema_only,
+            columns_description=columns_description,
+        )
         paths_log = ", ".join(self._paths) if len(self._paths) > 1 else self._paths[0]
         _logger.info(f"File: {paths_log} wrapped successfully.")
 
     def _fetch_data(self) -> dict[str, bytes]:
         datas = {}
         metadata: FilesMetadata = self.metadata  # type:ignore[assignment]
         for file in metadata.files:
```

### Comparing `vectice-24.2.6.0/src/vectice/models/resource/gcs_resource.py` & `vectice-24.2.7.0/src/vectice/models/resource/gcs_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,25 +44,31 @@
 
     def __init__(
         self,
         uris: str | list[str],
         dataframes: TDataFrameType | list[TDataFrameType] | None = None,
         gcs_client: Client | None = None,
         capture_schema_only: bool = False,
+        columns_description: dict[str, str] | None = None,
     ):
         """Initialize a GCS resource.
 
         Parameters:
             uris: The uris of the referenced resources. Should follow the pattern 'gs://<bucket_name>/<file_path_inside_bucket>'
             dataframes (Optional): The dataframes allowing vectice to optionally compute more metadata about this resource such as columns stats. (Support Pandas, Spark)
             gcs_client (Optional): The `google.cloud.storage.Client` to optionally retrieve file size, creation date and updated date (used for auto-versioning) up to 5000 files.
             capture_schema_only (Optional): A boolean parameter indicating whether to capture only the schema or both the schema and column statistics of the dataframes.
-
+            columns_description (Optional): A dictionary to map the column's name to a specific description. Should follow the format { "column_name": "Description", ... }
         """
-        super().__init__(paths=uris, dataframes=dataframes, capture_schema_only=capture_schema_only)
+        super().__init__(
+            paths=uris,
+            dataframes=dataframes,
+            capture_schema_only=capture_schema_only,
+            columns_description=columns_description,
+        )
         self.gcs_client = gcs_client
 
         for uri in self._paths:
             if not re.search(GS_URI_REG, uri):
                 raise ValueError(
                     f"Uri '{uri}' is not following the right pattern 'gs://<bucket_name>/<file_path_inside_bucket>'"
                 )
```

### Comparing `vectice-24.2.6.0/src/vectice/models/resource/metadata/__init__.py` & `vectice-24.2.7.0/src/vectice/models/resource/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/resource/metadata/base.py` & `vectice-24.2.7.0/src/vectice/models/resource/metadata/base.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/resource/metadata/column_metadata.py` & `vectice-24.2.7.0/src/vectice/models/resource/metadata/column_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/resource/metadata/dataframe_config.py` & `vectice-24.2.7.0/src/vectice/models/resource/metadata/dataframe_config.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/resource/metadata/db_metadata.py` & `vectice-24.2.7.0/src/vectice/models/resource/metadata/db_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py` & `vectice-24.2.7.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py` & `vectice-24.2.7.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py` & `vectice-24.2.7.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/resource/metadata/df_wrapper_resource.py` & `vectice-24.2.7.0/src/vectice/models/resource/metadata/df_wrapper_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py` & `vectice-24.2.7.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/resource/metadata/files_metadata.py` & `vectice-24.2.7.0/src/vectice/models/resource/metadata/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py` & `vectice-24.2.7.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/resource/metadata/source.py` & `vectice-24.2.7.0/src/vectice/models/resource/metadata/source.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/resource/no_resource.py` & `vectice-24.2.7.0/src/vectice/models/resource/no_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
     def __init__(
         self,
         origin: str,
         dataframes: TDataFrameType | list[TDataFrameType] | None = None,
         capture_schema_only: bool = False,
         type: TableType = TableType.UNKNOWN,
+        columns_description: dict[str, str] | None = None,
     ):
         """Initialize a file resource.
 
         Parameters:
             paths: The paths of the files to wrap.
             dataframes (Optional): The dataframes allowing vectice to optionally compute more metadata about this resource such as columns stats. (Support Pandas, Spark)
             capture_schema_only (Optional): A boolean parameter indicating whether to capture only the schema or both the schema and column statistics of the dataframes.
@@ -50,15 +51,20 @@
             called `iris.csv` in the current directory:
 
             ```python
             from vectice import FileResource
             iris_trainset = FileResource(paths="iris.csv")
             ```
         """
-        super().__init__(paths="", dataframes=dataframes, capture_schema_only=capture_schema_only)
+        super().__init__(
+            paths="",
+            dataframes=dataframes,
+            capture_schema_only=capture_schema_only,
+            columns_description=columns_description,
+        )
         self._origin = origin
         self._type = type
 
     def _fetch_data(
         self,
     ) -> dict:
         return {}
```

### Comparing `vectice-24.2.6.0/src/vectice/models/resource/s3_resource.py` & `vectice-24.2.7.0/src/vectice/models/resource/s3_resource.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,25 +47,32 @@
 
     def __init__(
         self,
         uris: str | list[str],
         dataframes: TDataFrameType | list[TDataFrameType] | None = None,
         s3_client: Client | None = None,
         capture_schema_only: bool = False,
+        columns_description: dict[str, str] | None = None,
     ):
         """Initialize an S3 resource.
 
         Parameters:
             uris: The uris of the resources to get. Should follow the pattern 's3://<bucket_name>/<file_path_inside_bucket>'
             dataframes (Optional): The dataframes allowing vectice to optionally compute more metadata about this resource such as columns stats. (Support Pandas, Spark)
             s3_client (Optional): The Amazon s3 client to optionally retrieve file size, creation date and updated date (used for auto-versioning) up to 5000 files.
             capture_schema_only (Optional): A boolean parameter indicating whether to capture only the schema or both the schema and column statistics of the dataframes.
+            columns_description (Optional): A dictionary to map the column's name to a specific description. Should follow the format { "column_name": "Description", ... }
 
         """
-        super().__init__(paths=uris, dataframes=dataframes, capture_schema_only=capture_schema_only)
+        super().__init__(
+            paths=uris,
+            dataframes=dataframes,
+            capture_schema_only=capture_schema_only,
+            columns_description=columns_description,
+        )
         self.s3_client = s3_client
         for uri in self._paths:
             if not re.search(S3_URI_REG, uri):
                 raise ValueError(
                     f"Uri '{uri}' is not following the right pattern 's3://<bucket_name>/<file_path_inside_bucket>'"
                 )
```

### Comparing `vectice-24.2.6.0/src/vectice/models/resource/snowflake_resource.py` & `vectice-24.2.7.0/src/vectice/models/resource/snowflake_resource.py`

 * *Files 17% similar despite different names*

```diff
@@ -64,16 +64,33 @@
     def __init__(
         self,
         paths: str | list[str],
         dataframes: TDataFrameType | list[TDataFrameType] | None = None,
         snowflake_client: Session | None = None,
         capture_schema_only: bool = False,
         force_dataframe: bool = False,
+        columns_description: dict[str, str] | None = None,
     ):
-        super().__init__(paths=paths, dataframes=dataframes, capture_schema_only=capture_schema_only)
+        """Initialize a Snowflake resource.
+
+        Parameters:
+            paths: The pahts of the resources to get.
+            dataframes (Optional): The dataframes allowing vectice to optionally compute more metadata about this resource such as columns stats. (Support Pandas, Spark)
+            snowflake_client (Optional): The Snowflake client to retrieve table metadatas.
+            capture_schema_only (Optional): A boolean parameter indicating whether to capture only the schema or both the schema and column statistics of the dataframes.
+            force_dataframe (Optional): A boolean parameter indicating whether the dataframe should be inferred from the table itself.
+            columns_description (Optional): A dictionary to map the column's name to a specific description. Should follow the format { "column_name": "Description", ... }
+
+        """
+        super().__init__(
+            paths=paths,
+            dataframes=dataframes,
+            capture_schema_only=capture_schema_only,
+            columns_description=columns_description,
+        )
         self.snowflake_client = snowflake_client
         self.force_dataframe = force_dataframe
 
     def _fetch_data(self) -> dict[str, tuple[TTable | None, TDataFrameType | None]]:
         tables: dict[str, tuple[TTable | None, TDataFrameType | None]] = {}
         df_index = 0
         for path in self._paths:
```

### Comparing `vectice-24.2.6.0/src/vectice/models/table.py` & `vectice-24.2.7.0/src/vectice/models/table.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/test_library/binary_classification_test.py` & `vectice-24.2.7.0/src/vectice/models/test_library/binary_classification_test.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/validation.py` & `vectice-24.2.7.0/src/vectice/models/validation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/models/workspace.py` & `vectice-24.2.7.0/src/vectice/models/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/services/iteration_service.py` & `vectice-24.2.7.0/src/vectice/services/iteration_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     def log_table(self, asset: Table, section: str | None = None):
         data = transform_table_to_metadata_dict(asset)
         entity_metadata = IterationStepArtifactEntityMetadataInput(name=asset.name, content={"data": data})
 
         artifact_inp: list[IterationStepArtifactInput] = [
             IterationStepArtifactInput(type="EntityMetadata", entityMetadata=entity_metadata)
         ]
-        self._client.assert_feature_flag_or_raise("vectice-table")
         self._client.add_iteration_artifacts(iteration_id=self._iteration.id, artifacts=artifact_inp, section=section)
 
     def log_model(self, asset: Model, section: str | None = None):
         from vectice import code_file_capture
 
         global code_source_file
```

### Comparing `vectice-24.2.6.0/src/vectice/services/phase_service.py` & `vectice-24.2.7.0/src/vectice/services/phase_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/types/version.py` & `vectice-24.2.7.0/src/vectice/types/version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/utils/code_parser.py` & `vectice-24.2.7.0/src/vectice/utils/code_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,42 +4,63 @@
 import os
 import re
 from collections import OrderedDict
 from typing import Any
 
 
 class FilePathVisitor(ast.NodeVisitor):
-    def __init__(self):
+    def __init__(self, is_graph_path: bool = False, is_dataset_path: bool = False):
         self.file_paths = set()
+        self.dataset_file_paths = []
+        self.is_graph_path = is_graph_path
+        self.is_dataset_path = is_dataset_path
 
     def visit_Call(self, node: ast.Call) -> None:  # noqa: N802
         if isinstance(node.func, ast.Name) or isinstance(node.func, ast.Attribute):
             # Record function args, kwargs.
+            path_var_and_path = {"variable": None, "path": None}
+            supported_path = False
             try:
                 func_name = node.func.attr  # pyright: ignore[reportAttributeAccessIssue]
-                supported_graph = self._is_supported_graph_library(func_name)
+                if self.is_graph_path:
+                    supported_path = self._is_supported_graph_library(func_name)
+                if self.is_dataset_path:
+                    supported_path = self._is_supported_dataset_library(func_name)
             except AttributeError:
-                supported_graph = False
+                pass
 
             args = node.args + node.keywords
             for arg in args:
                 arg_value = self._get_arg_or_kwarg_val(arg)
-                if arg_value and self._is_valid_file(arg_value) and supported_graph:
-                    self.file_paths.add(arg_value)
+                if arg_value and self._is_valid_file(arg_value) and supported_path:
+                    if self.is_dataset_path:
+                        path_var_and_path["path"] = arg_value
+                        self.dataset_file_paths.append(path_var_and_path)
+                    if self.is_graph_path:
+                        self.file_paths.add(arg_value)
+
         self.generic_visit(node)
 
     def visit_Assign(self, node: ast.Assign) -> None:
+        path_var_and_path = {"variable": None, "path": None}
+
         try:
             if len(node.targets) == 1 and isinstance(
                 node.targets[0], ast.Name
             ):  # pyright: ignore[reportAttributeAccessIssue]
+                var_name = node.targets[0].id
+                path_var_and_path["variable"] = var_name  # pyright: ignore[reportArgumentType]
                 if isinstance(node.value, ast.Str):  # pyright: ignore[reportDeprecated]
                     path = node.value.s  # pyright: ignore[reportAttributeAccessIssue]
                     if self._is_valid_file(path):
-                        self.file_paths.add(path)
+                        if self.is_dataset_path:
+                            path_var_and_path["path"] = path  # pyright: ignore[reportArgumentType]
+                            self.dataset_file_paths.append(path_var_and_path)
+                        if self.is_graph_path:
+                            self.file_paths.add(path)
         except Exception:
             pass
         self.generic_visit(node)
 
     def _get_arg_or_kwarg_val(self, arg: Any) -> Any | None:
         try:
             # arg value
@@ -78,14 +99,22 @@
             "savefig",
             "write_image",
         ]
         if func_name in vectice_supported_graphs:
             return True
         return False
 
+    def _is_supported_dataset_library(self, func_name: str) -> bool:
+        vectice_supported_datasets = [
+            "read_csv",
+        ]
+        if func_name in vectice_supported_datasets:
+            return True
+        return False
+
 
 class VariableVisitor(ast.NodeVisitor):
     def __init__(self, model_metrics: bool = False):
         self.variables: OrderedDict[str, None] = OrderedDict()
         self.processed_variables: set[str] = set()
         self.function_call_args: set[str] = set()
         self.function_call_kwargs: set[str] = set()
```

### Comparing `vectice-24.2.6.0/src/vectice/utils/common_utils.py` & `vectice-24.2.7.0/src/vectice/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/utils/configuration.py` & `vectice-24.2.7.0/src/vectice/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/utils/deprecation.py` & `vectice-24.2.7.0/src/vectice/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/utils/instance_helper.py` & `vectice-24.2.7.0/src/vectice/utils/instance_helper.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/utils/last_assets.py` & `vectice-24.2.7.0/src/vectice/utils/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice/utils/logging_utils.py` & `vectice-24.2.7.0/src/vectice/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.6.0/src/vectice.egg-info/PKG-INFO` & `vectice-24.2.7.0/src/vectice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 24.2.6.0
+Version: 24.2.7.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
@@ -26,15 +26,15 @@
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: types-python-dateutil
 Requires-Dist: python-dotenv>=0.11.0
-Requires-Dist: requests>=2.5.0
+Requires-Dist: requests<=2.30.0
 Requires-Dist: rich
 Requires-Dist: urllib3
 Requires-Dist: gql[requests]
 Requires-Dist: GitPython
 Requires-Dist: packaging
 Requires-Dist: Pillow
 Requires-Dist: pandas
@@ -62,15 +62,15 @@
 Requires-Dist: mkdocs-section-index>=0.3; extra == "doc"
 Requires-Dist: mkdocstrings[python]>=0.18; extra == "doc"
 Provides-Extra: test
 Requires-Dist: docker-compose; extra == "test"
 Requires-Dist: dslr[psycopg2-binary]; extra == "test"
 Requires-Dist: mock>=1.0.1; extra == "test"
 Requires-Dist: numpy; extra == "test"
-Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest==8.2.0; extra == "test"
 Requires-Dist: pytest-randomly; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pydrive2; extra == "test"
 Requires-Dist: scikit-learn; extra == "test"
 Requires-Dist: testcontainers==3.7.1; extra == "test"
 Requires-Dist: db-dtypes>=1.1.1; extra == "test"
@@ -86,25 +86,26 @@
 Requires-Dist: nbformat; extra == "test"
 Requires-Dist: lightgbm; extra == "test"
 Requires-Dist: catboost; extra == "test"
 Requires-Dist: tensorflow; extra == "test"
 Requires-Dist: keras; extra == "test"
 Requires-Dist: snowflake-snowpark-python; extra == "test"
 Requires-Dist: seaborn; extra == "test"
+Requires-Dist: statsmodels; extra == "test"
 Requires-Dist: xgboost; extra == "test"
 Requires-Dist: kaleido; extra == "test"
 Requires-Dist: catboost; extra == "test"
 Requires-Dist: torch; extra == "test"
 Provides-Extra: gcs
 Requires-Dist: google-cloud-storage>=1.17.0; extra == "gcs"
 Requires-Dist: google-cloud-bigquery; extra == "gcs"
 Provides-Extra: s3
 Requires-Dist: boto3; extra == "s3"
 Provides-Extra: validation
-Requires-Dist: shap; extra == "validation"
-Requires-Dist: scipy; extra == "validation"
+Requires-Dist: shap==0.44.1; extra == "validation"
+Requires-Dist: scipy<=1.12; extra == "validation"
 
 Auto-documentation for ML projects & their governance. View https://github.com/vectice/GettingStarted to get started.
 
 # Documentation
 
 Official documentation for Vectice can be found at https://docs.vectice.com.
```

### Comparing `vectice-24.2.6.0/src/vectice.egg-info/SOURCES.txt` & `vectice-24.2.7.0/src/vectice.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 src/vectice/autolog/asset_services/keras_service.py
 src/vectice/autolog/asset_services/lightgbm_service.py
 src/vectice/autolog/asset_services/metric_service.py
 src/vectice/autolog/asset_services/pandas_service.py
 src/vectice/autolog/asset_services/pyspark_service.py
 src/vectice/autolog/asset_services/pytorch_service.py
 src/vectice/autolog/asset_services/sklearn_service.py
+src/vectice/autolog/asset_services/statsmodel_wrapper_service.py
 src/vectice/autolog/asset_services/vectice_asset_service.py
 src/vectice/models/__init__.py
 src/vectice/models/additional_info.py
 src/vectice/models/attachment.py
 src/vectice/models/attachment_container.py
 src/vectice/models/code_version.py
 src/vectice/models/dataset.py
```

### Comparing `vectice-24.2.6.0/src/vectice.egg-info/requires.txt` & `vectice-24.2.7.0/src/vectice.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 types-python-dateutil
 python-dotenv>=0.11.0
-requests>=2.5.0
+requests<=2.30.0
 rich
 urllib3
 gql[requests]
 GitPython
 packaging
 Pillow
 pandas
@@ -42,15 +42,15 @@
 boto3
 
 [test]
 docker-compose
 dslr[psycopg2-binary]
 mock>=1.0.1
 numpy
-pytest
+pytest==8.2.0
 pytest-randomly
 coverage
 pytest-cov
 pydrive2
 scikit-learn
 testcontainers==3.7.1
 db-dtypes>=1.1.1
@@ -66,14 +66,15 @@
 nbformat
 lightgbm
 catboost
 tensorflow
 keras
 snowflake-snowpark-python
 seaborn
+statsmodels
 xgboost
 kaleido
 torch
 
 [validation]
-shap
-scipy
+shap==0.44.1
+scipy<=1.12
```

