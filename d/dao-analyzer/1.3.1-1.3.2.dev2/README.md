# Comparing `tmp/dao_analyzer-1.3.1.tar.gz` & `tmp/dao_analyzer-1.3.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dao_analyzer-1.3.1.tar", last modified: Mon May 27 08:18:08 2024, max compression
+gzip compressed data, was "dao_analyzer-1.3.2.dev2.tar", last modified: Mon May 27 08:22:10 2024, max compression
```

## Comparing `dao_analyzer-1.3.1.tar` & `dao_analyzer-1.3.2.dev2.tar`

### file list

```diff
@@ -1,412 +1,412 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.558170 dao_analyzer-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.494170 dao_analyzer-1.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.494170 dao_analyzer-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/.hintrc
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/ABOUT.md
--rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12136 2024-05-27 08:18:08.558170 dao_analyzer-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9755 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.482170 dao_analyzer-1.3.1/dao_analyzer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.498170 dao_analyzer-1.3.1/dao_analyzer/web/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-27 08:18:08.000000 dao_analyzer-1.3.1/dao_analyzer/web/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.498170 dao_analyzer-1.3.1/dao_analyzer/web/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.498170 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.498170 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/business/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/business/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16209 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/business/app_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.502170 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/business/metric_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/business/metric_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/business/metric_adapter/basic_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/business/metric_adapter/cast_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/business/metric_adapter/installed_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/business/metric_adapter/vote_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)   399465 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/class_diagram.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.502170 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.502170 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.502170 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/metric_dao_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/srcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.502170 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_token_holders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_voters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_approval_vote_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_assets_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_assets_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_cast_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_voters_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_installed_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_new_additions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_organization_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_total_token_holders.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_vote_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/platform_dao.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.506170 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/presentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/presentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.506170 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/resources/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.506170 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.506170 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.506170 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/api/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/api/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/api/graphql/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/api/graphql/query_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.506170 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/i_metric_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.506170 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/transfers/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/transfers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/transfers/hierarchical_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/transfers/n_stacked_serie.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.506170 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/transfers/organization/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/transfers/organization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/transfers/organization/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/transfers/organization/organization_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/transfers/organization/organization_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/transfers/organization/participation_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/transfers/organization/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/transfers/serie.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/transfers/stacked_serie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/transfers/tabular_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.510170 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.510170 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.510170 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/daos/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/daos/metric/metric_dao.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/daos/metric/srcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.510170 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/imetric_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/daos/platform_dao.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/pandas_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.510170 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/requesters/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/requesters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/requesters/cache_requester.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/requesters/irequester.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/requesters/join_cache_requester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.510170 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.510170 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/about_view/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/about_view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/about_view/about_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.510170 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/chart_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/chart_sum_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/dt_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.514170 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/data_table_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/data_table_layout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.514170 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/figure/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/figure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/figure/bar_figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/figure/calplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/figure/double_scatter_figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/figure/multi_bar_figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/figure/treemap_figure.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/ilayout.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/layout_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.514170 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/dashboard_view/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/dashboard_view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/dashboard_view/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/dashboard_view/dashboard_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.514170 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/main_view/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/main_view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/main_view/main_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/main_view/main_view_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.518170 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/resources/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/common/resources/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.518170 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.518170 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/business/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/business/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16026 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/business/app_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.518170 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/business/metric_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/business/metric_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/business/metric_adapter/basic_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/business/metric_adapter/votes_type.py
--rw-r--r--   0 runner    (1001) docker     (127)   418772 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/class_diagram.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.518170 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.518170 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.522170 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/metric_dao_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/srcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.522170 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_voters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_approval_proposal_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_assets_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_assets_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_new_additions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_organization_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_total_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_voters_percentage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_voters_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/platform_dao.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.522170 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/presentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/presentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.522170 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/resources/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.522170 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.526170 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/business/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/business/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/business/app_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.526170 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/business/metric_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/business/metric_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/business/metric_adapter/majority_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/business/metric_adapter/metric_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/business/metric_adapter/proposal_boost_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/business/metric_adapter/success_ratio_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/business/metric_adapter/vote_type.py
--rw-r--r--   0 runner    (1001) docker     (127)   461806 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/class_diagram.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.526170 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.526170 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.526170 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/metric_dao_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/srcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.530170 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_approval_proposal_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_assets_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_assets_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_different_voters_stakers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_organization_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_majority.py
--rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_time_serie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_reputation_holders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_votes_stakes_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_voters_percentage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_voters_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/platform_dao.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.530170 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/presentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/presentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.530170 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/resources/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.534170 dao_analyzer-1.3.1/dao_analyzer/web/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/assets/ABOUT.md
--rw-r--r--   0 runner    (1001) docker     (127)    65944 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/assets/aragon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/assets/callbacks.js
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/assets/cc-by.png
--rw-r--r--   0 runner    (1001) docker     (127)    18045 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/assets/dao-analyzer_header.svg
--rw-r--r--   0 runner    (1001) docker     (127)    36174 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/assets/dao-analyzer_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    54135 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/assets/daohaus.png
--rw-r--r--   0 runner    (1001) docker     (127)    16481 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/assets/daostack.png
--rw-r--r--   0 runner    (1001) docker     (127)   101409 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    58578 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/assets/github_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/assets/ico-github.svg
--rw-r--r--   0 runner    (1001) docker     (127)    17972 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/assets/img_header.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   129808 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/assets/kaggle_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/assets/logo-GPL.png
--rw-r--r--   0 runner    (1001) docker     (127)    10979 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/assets/logo-erc.png
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/assets/logo-grasia.png
--rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/assets/logo-ministerio.png
--rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/assets/logo-ucm.png
--rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/assets/logo_dao_analyzer.png
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/assets/logo_dao_analyzer.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/assets/logo_dao_analyzer_orig.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/assets/stylesheet.css
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer/web/matomo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.554170 dao_analyzer-1.3.1/dao_analyzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12136 2024-05-27 08:18:08.000000 dao_analyzer-1.3.1/dao_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18845 2024-05-27 08:18:08.000000 dao_analyzer-1.3.1/dao_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 08:18:08.000000 dao_analyzer-1.3.1/dao_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-27 08:18:08.000000 dao_analyzer-1.3.1/dao_analyzer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 08:18:08.000000 dao_analyzer-1.3.1/dao_analyzer.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-27 08:18:08.000000 dao_analyzer-1.3.1/dao_analyzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-27 08:18:08.000000 dao_analyzer-1.3.1/dao_analyzer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.538170 dao_analyzer-1.3.1/dao_analyzer_components/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/.babelrc
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/.eslintrc
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/_validate_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.542170 dao_analyzer-1.3.1/dao_analyzer_components/dao_analyzer_components/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/dao_analyzer_components/DAOInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/dao_analyzer_components/DataPoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/dao_analyzer_components/ParticipationStat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/dao_analyzer_components/PlatformInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/dao_analyzer_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/dao_analyzer_components/_imports_.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.css
--rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    19068 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/dao_analyzer_components/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/dao_analyzer_components/package-info.json
--rw-r--r--   0 runner    (1001) docker     (127)   369525 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.542170 dao_analyzer-1.3.1/dao_analyzer_components/public/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/public/index.html
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.486170 dao_analyzer-1.3.1/dao_analyzer_components/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.542170 dao_analyzer-1.3.1/dao_analyzer_components/src/demo/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/src/demo/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.542170 dao_analyzer-1.3.1/dao_analyzer_components/src/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.542170 dao_analyzer-1.3.1/dao_analyzer_components/src/lib/components/
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/src/lib/components/DAOInfo.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/src/lib/components/DataPoint.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/src/lib/components/ParticipationStat.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/src/lib/components/PlatformInfo.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/src/lib/index.js
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/dao_analyzer_components/webpack.demo.config.js
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/gunicorn_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      197 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/init.sh
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.542170 dao_analyzer-1.3.1/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.546170 dao_analyzer-1.3.1/scripts/archive/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/scripts/archive/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)   339476 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/scripts/archive/names.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (127)     1010 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/scripts/archive/uploadToKaggle.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1790 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/scripts/checkContinue.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     4349 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/scripts/datawarehouseDiff.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      251 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/scripts/deploy.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      111 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/scripts/printArrow.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1148 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/scripts/updateAragonNames.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2900 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/scripts/uploadDataWarehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-27 08:18:08.558170 dao_analyzer-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.546170 dao_analyzer-1.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.546170 dao_analyzer-1.3.1/test/mocks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/mocks/api_requester_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/mocks/unix_date_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.546170 dao_analyzer-1.3.1/test/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.546170 dao_analyzer-1.3.1/test/unit/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.546170 dao_analyzer-1.3.1/test/unit/apps/aragon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/aragon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.546170 dao_analyzer-1.3.1/test/unit/apps/aragon/data_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/aragon/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.546170 dao_analyzer-1.3.1/test/unit/apps/aragon/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/aragon/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.546170 dao_analyzer-1.3.1/test/unit/apps/aragon/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/aragon/data_access/daos/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.546170 dao_analyzer-1.3.1/test/unit/apps/aragon/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/aragon/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/aragon/data_access/daos/metric/strategy/test_aragon_st_new_additions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_organization_aragon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_token_holders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_cast_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_installed_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_vote_outcome.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.546170 dao_analyzer-1.3.1/test/unit/apps/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.546170 dao_analyzer-1.3.1/test/unit/apps/common/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/common/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.546170 dao_analyzer-1.3.1/test/unit/apps/common/api/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/common/api/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/common/api/graphql/test_query_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.546170 dao_analyzer-1.3.1/test/unit/apps/common/business/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/common/business/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.550170 dao_analyzer-1.3.1/test/unit/apps/common/business/transfers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/common/business/transfers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/common/business/transfers/test_organization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.550170 dao_analyzer-1.3.1/test/unit/apps/common/data_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/common/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.550170 dao_analyzer-1.3.1/test/unit/apps/common/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/common/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.550170 dao_analyzer-1.3.1/test/unit/apps/daohaus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daohaus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.550170 dao_analyzer-1.3.1/test/unit/apps/daohaus/data_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daohaus/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.550170 dao_analyzer-1.3.1/test/unit/apps/daohaus/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daohaus/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.550170 dao_analyzer-1.3.1/test/unit/apps/daohaus/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daohaus/data_access/daos/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.550170 dao_analyzer-1.3.1/test/unit/apps/daohaus/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daohaus/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_organization_daohaus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_voters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_dproposal_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_new_additions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_proposal_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_total_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_votes_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.550170 dao_analyzer-1.3.1/test/unit/apps/daostack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daostack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.550170 dao_analyzer-1.3.1/test/unit/apps/daostack/data_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daostack/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.550170 dao_analyzer-1.3.1/test/unit/apps/daostack/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daostack/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.550170 dao_analyzer-1.3.1/test/unit/apps/daostack/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daostack/data_access/daos/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.554170 dao_analyzer-1.3.1/test/unit/apps/daostack/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daostack/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_organization_daostack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_diff_voters_stakers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_majority.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_time_serie.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_voters_percentage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.554170 dao_analyzer-1.3.1/test/unit/apps/daostack/data_access/requesters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/apps/daostack/data_access/requesters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:18:08.554170 dao_analyzer-1.3.1/test/unit/components/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-27 08:17:58.000000 dao_analyzer-1.3.1/test/unit/components/test_dao_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.294793 dao_analyzer-1.3.2.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.234793 dao_analyzer-1.3.2.dev2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.234793 dao_analyzer-1.3.2.dev2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/.hintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/ABOUT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12141 2024-05-27 08:22:10.294793 dao_analyzer-1.3.2.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9755 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.222793 dao_analyzer-1.3.2.dev2/dao_analyzer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.238793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-27 08:22:10.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.238793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.238793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.238793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/business/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/business/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16209 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/business/app_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.238793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/business/metric_adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/business/metric_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/business/metric_adapter/basic_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/business/metric_adapter/cast_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/business/metric_adapter/installed_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/business/metric_adapter/vote_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)   399465 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/class_diagram.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.238793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.238793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.242793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/metric_dao_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/srcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.242793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_token_holders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_voters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_approval_vote_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_assets_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_assets_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_cast_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_voters_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_installed_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_new_additions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_organization_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_total_token_holders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_vote_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/platform_dao.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.242793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/presentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/presentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.242793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/resources/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.242793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.242793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.246793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/api/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/api/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/api/graphql/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/api/graphql/query_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.246793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/i_metric_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.246793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/transfers/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/transfers/hierarchical_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/transfers/n_stacked_serie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.246793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/transfers/organization/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/transfers/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/transfers/organization/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/transfers/organization/organization_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/transfers/organization/organization_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/transfers/organization/participation_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/transfers/organization/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/transfers/serie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/transfers/stacked_serie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/transfers/tabular_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.246793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.246793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.250793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/daos/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/daos/metric/metric_dao.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/daos/metric/srcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.250793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/imetric_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/daos/platform_dao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/pandas_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.250793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/requesters/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/requesters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/requesters/cache_requester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/requesters/irequester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/requesters/join_cache_requester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.250793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.250793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/about_view/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/about_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/about_view/about_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.250793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/chart_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/chart_sum_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/dt_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.254793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/data_table_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/data_table_layout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.254793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/figure/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/figure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/figure/bar_figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/figure/calplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/figure/double_scatter_figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/figure/multi_bar_figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/figure/treemap_figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/ilayout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/layout_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.254793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/dashboard_view/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/dashboard_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/dashboard_view/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/dashboard_view/dashboard_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.254793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/main_view/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/main_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/main_view/main_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/main_view/main_view_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.254793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/resources/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/resources/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.254793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.258793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/business/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/business/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16026 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/business/app_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.258793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/business/metric_adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/business/metric_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/business/metric_adapter/basic_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/business/metric_adapter/votes_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)   418772 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/class_diagram.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.258793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.258793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.258793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/metric_dao_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/srcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.262793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_voters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_approval_proposal_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_assets_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_assets_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_new_additions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_organization_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_total_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_voters_percentage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_voters_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/platform_dao.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.262793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/presentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/presentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.262793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/resources/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.262793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.262793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/business/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/business/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/business/app_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.266793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/business/metric_adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/business/metric_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/business/metric_adapter/majority_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/business/metric_adapter/metric_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/business/metric_adapter/proposal_boost_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/business/metric_adapter/success_ratio_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/business/metric_adapter/vote_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)   461806 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/class_diagram.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.266793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.266793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.266793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/metric_dao_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/srcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.270793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_approval_proposal_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_assets_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_assets_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_different_voters_stakers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_organization_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_majority.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_time_serie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_reputation_holders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_votes_stakes_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_voters_percentage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_voters_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/platform_dao.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.270793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/presentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/presentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.270793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/resources/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.274793 dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/ABOUT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    65944 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/aragon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/callbacks.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/cc-by.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18045 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/dao-analyzer_header.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    36174 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/dao-analyzer_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    54135 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/daohaus.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16481 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/daostack.png
+-rw-r--r--   0 runner    (1001) docker     (127)   101409 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    58578 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/github_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/ico-github.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    17972 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/img_header.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   129808 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/kaggle_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/logo-GPL.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10979 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/logo-erc.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/logo-grasia.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/logo-ministerio.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/logo-ucm.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/logo_dao_analyzer.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/logo_dao_analyzer.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/logo_dao_analyzer_orig.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/stylesheet.css
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer/web/matomo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.294793 dao_analyzer-1.3.2.dev2/dao_analyzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12141 2024-05-27 08:22:10.000000 dao_analyzer-1.3.2.dev2/dao_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18845 2024-05-27 08:22:10.000000 dao_analyzer-1.3.2.dev2/dao_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 08:22:10.000000 dao_analyzer-1.3.2.dev2/dao_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-27 08:22:10.000000 dao_analyzer-1.3.2.dev2/dao_analyzer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 08:22:10.000000 dao_analyzer-1.3.2.dev2/dao_analyzer.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-27 08:22:10.000000 dao_analyzer-1.3.2.dev2/dao_analyzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-27 08:22:10.000000 dao_analyzer-1.3.2.dev2/dao_analyzer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.278793 dao_analyzer-1.3.2.dev2/dao_analyzer_components/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/.babelrc
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/.eslintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/_validate_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.278793 dao_analyzer-1.3.2.dev2/dao_analyzer_components/dao_analyzer_components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-27 08:22:02.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/dao_analyzer_components/DAOInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-27 08:22:02.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/dao_analyzer_components/DataPoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-27 08:22:02.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/dao_analyzer_components/ParticipationStat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-27 08:22:02.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/dao_analyzer_components/PlatformInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-27 08:22:02.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/dao_analyzer_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-27 08:22:02.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/dao_analyzer_components/_imports_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-27 08:22:02.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.css
+-rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-05-27 08:22:02.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19068 2024-05-27 08:22:02.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-05-27 08:22:02.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/dao_analyzer_components/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-27 08:22:02.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/dao_analyzer_components/package-info.json
+-rw-r--r--   0 runner    (1001) docker     (127)   369532 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.278793 dao_analyzer-1.3.2.dev2/dao_analyzer_components/public/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.226793 dao_analyzer-1.3.2.dev2/dao_analyzer_components/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.278793 dao_analyzer-1.3.2.dev2/dao_analyzer_components/src/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/src/demo/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.278793 dao_analyzer-1.3.2.dev2/dao_analyzer_components/src/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.282793 dao_analyzer-1.3.2.dev2/dao_analyzer_components/src/lib/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/src/lib/components/DAOInfo.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/src/lib/components/DataPoint.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/src/lib/components/ParticipationStat.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/src/lib/components/PlatformInfo.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/src/lib/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/dao_analyzer_components/webpack.demo.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/gunicorn_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      197 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/init.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.282793 dao_analyzer-1.3.2.dev2/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.282793 dao_analyzer-1.3.2.dev2/scripts/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/scripts/archive/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   339476 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/scripts/archive/names.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1010 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/scripts/archive/uploadToKaggle.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1790 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/scripts/checkContinue.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4349 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/scripts/datawarehouseDiff.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      251 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/scripts/deploy.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      111 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/scripts/printArrow.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1148 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/scripts/updateAragonNames.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2900 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/scripts/uploadDataWarehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-27 08:22:10.294793 dao_analyzer-1.3.2.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.282793 dao_analyzer-1.3.2.dev2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.282793 dao_analyzer-1.3.2.dev2/test/mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/mocks/api_requester_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/mocks/unix_date_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.282793 dao_analyzer-1.3.2.dev2/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.282793 dao_analyzer-1.3.2.dev2/test/unit/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.286793 dao_analyzer-1.3.2.dev2/test/unit/apps/aragon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/aragon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.286793 dao_analyzer-1.3.2.dev2/test/unit/apps/aragon/data_access/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/aragon/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.286793 dao_analyzer-1.3.2.dev2/test/unit/apps/aragon/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/aragon/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.286793 dao_analyzer-1.3.2.dev2/test/unit/apps/aragon/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/aragon/data_access/daos/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.286793 dao_analyzer-1.3.2.dev2/test/unit/apps/aragon/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/aragon/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/aragon/data_access/daos/metric/strategy/test_aragon_st_new_additions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_organization_aragon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_token_holders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_cast_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_installed_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_vote_outcome.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.286793 dao_analyzer-1.3.2.dev2/test/unit/apps/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.286793 dao_analyzer-1.3.2.dev2/test/unit/apps/common/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/common/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.286793 dao_analyzer-1.3.2.dev2/test/unit/apps/common/api/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/common/api/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/common/api/graphql/test_query_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.286793 dao_analyzer-1.3.2.dev2/test/unit/apps/common/business/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/common/business/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.286793 dao_analyzer-1.3.2.dev2/test/unit/apps/common/business/transfers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/common/business/transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/common/business/transfers/test_organization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.286793 dao_analyzer-1.3.2.dev2/test/unit/apps/common/data_access/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/common/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.286793 dao_analyzer-1.3.2.dev2/test/unit/apps/common/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/common/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.286793 dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.286793 dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/data_access/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.286793 dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.286793 dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/data_access/daos/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.290794 dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_organization_daohaus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_voters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_dproposal_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_new_additions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_proposal_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_total_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_votes_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.290794 dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.290794 dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/data_access/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.290794 dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.290794 dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/data_access/daos/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.290794 dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_organization_daostack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_diff_voters_stakers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_majority.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_time_serie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_voters_percentage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.290794 dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/data_access/requesters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/data_access/requesters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:22:10.294793 dao_analyzer-1.3.2.dev2/test/unit/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-27 08:22:01.000000 dao_analyzer-1.3.2.dev2/test/unit/components/test_dao_info.py
```

### Comparing `dao_analyzer-1.3.1/.github/dependabot.yml` & `dao_analyzer-1.3.2.dev2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/.github/workflows/ci.yml` & `dao_analyzer-1.3.2.dev2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/.gitignore` & `dao_analyzer-1.3.2.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/ABOUT.md` & `dao_analyzer-1.3.2.dev2/ABOUT.md`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/CHANGELOG.md` & `dao_analyzer-1.3.2.dev2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/CITATION.cff` & `dao_analyzer-1.3.2.dev2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/Dockerfile` & `dao_analyzer-1.3.2.dev2/Dockerfile`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/LICENSE` & `dao_analyzer-1.3.2.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/PKG-INFO` & `dao_analyzer-1.3.2.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dao-analyzer
-Version: 1.3.1
+Version: 1.3.2.dev2
 Summary: "A tool to monitor DAO activity"
 Home-page: https://dao-analyzer.science
 Author: David Davó
 Author-email: ddavo@ucm.es
 Project-URL: Source, https://github.com/Grasia/dao-analyzer
 Project-URL: Bug Tracker, https://github.com/Grasia/dao-analyzer/issues
 Project-URL: Changelog, https://github.com/Grasia/dao-analyzer/blob/master/CHANGELOG.md
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: dao-analyzer Version: 1.3.1 Summary: "A tool to
-monitor DAO activity" Home-page: https://dao-analyzer.science Author: David
+Metadata-Version: 2.1 Name: dao-analyzer Version: 1.3.2.dev2 Summary: "A tool
+to monitor DAO activity" Home-page: https://dao-analyzer.science Author: David
 DavÃ³ Author-email: ddavo@ucm.es Project-URL: Source, https://github.com/
 Grasia/dao-analyzer Project-URL: Bug Tracker, https://github.com/Grasia/dao-
 analyzer/issues Project-URL: Changelog, https://github.com/Grasia/dao-analyzer/
 blob/master/CHANGELOG.md Classifier: Development Status :: 5 - Production/
 Stable Classifier: Environment :: Console Classifier: Environment :: Web
 Environment Classifier: Framework :: Dash Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: GNU General Public
```

### Comparing `dao_analyzer-1.3.1/README.md` & `dao_analyzer-1.3.2.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/app.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/app.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/business/app_service.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/business/app_service.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_tokens.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_tokens.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_values.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_values.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/business/metric_adapter/basic_adapter.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/business/metric_adapter/basic_adapter.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/business/metric_adapter/cast_type.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/business/metric_adapter/cast_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/business/metric_adapter/installed_apps.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/business/metric_adapter/installed_apps.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/business/metric_adapter/vote_outcome.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/business/metric_adapter/vote_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/class_diagram.png` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/class_diagram.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/metric_dao_factory.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/metric_dao_factory.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/srcs.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/srcs.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_organization.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_organization.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_token_holders.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_token_holders.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_voters.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_voters.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_approval_vote_rate.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_approval_vote_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_cast_type.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_cast_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_rate.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_voters_rate.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_voters_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_installed_apps.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_installed_apps.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_new_additions.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_new_additions.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_organization_activity.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_organization_activity.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_total_token_holders.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_total_token_holders.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_vote_outcome.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_vote_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/data_access/daos/platform_dao.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/data_access/daos/platform_dao.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/aragon/resources/strings.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/aragon/resources/strings.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/api/graphql/query.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/api/graphql/query.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/api/graphql/query_builder.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/api/graphql/query_builder.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/i_metric_adapter.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/i_metric_adapter.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/singleton.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/singleton.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/transfers/hierarchical_data.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/transfers/hierarchical_data.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/transfers/n_stacked_serie.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/transfers/n_stacked_serie.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/transfers/organization/organization.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/transfers/organization/organization.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/transfers/organization/organization_filter.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/transfers/organization/organization_filter.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/transfers/organization/organization_list.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/transfers/organization/organization_list.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/transfers/organization/participation_stats.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/transfers/organization/participation_stats.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/transfers/organization/platform.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/transfers/organization/platform.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/transfers/serie.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/transfers/serie.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/transfers/stacked_serie.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/transfers/stacked_serie.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/business/transfers/tabular_data.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/business/transfers/tabular_data.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/daos/metric/metric_dao.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/daos/metric/metric_dao.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/imetric_strategy.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/imetric_strategy.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_tokens.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_tokens.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_values.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_values.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/daos/platform_dao.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/daos/platform_dao.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/pandas_utils.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/requesters/cache_requester.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/requesters/cache_requester.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/requesters/irequester.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/requesters/irequester.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/data_access/requesters/join_cache_requester.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/data_access/requesters/join_cache_requester.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/about_view/about_view.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/about_view/about_view.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/chart_controller.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/chart_controller.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/chart_sum_controller.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/chart_sum_controller.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/dt_controller.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/dt_controller.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_configuration.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_configuration.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_layout.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_layout.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/data_table_layout.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/data_table_layout.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/figure/bar_figure.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/figure/bar_figure.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/figure/calplot.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/figure/calplot.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/figure/double_scatter_figure.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/figure/double_scatter_figure.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure_configuration.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure_configuration.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/figure/multi_bar_figure.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/figure/multi_bar_figure.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/figure/treemap_figure.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/figure/treemap_figure.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/charts/layout/layout_configuration.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/charts/layout/layout_configuration.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/dashboard_view/controller.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/dashboard_view/controller.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/dashboard_view/dashboard_view.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/dashboard_view/dashboard_view.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/main_view/main_view.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/main_view/main_view.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/presentation/main_view/main_view_controller.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/presentation/main_view/main_view_controller.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/resources/colors.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/resources/colors.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/common/resources/strings.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/common/resources/strings.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/business/app_service.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/business/app_service.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_tokens.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_tokens.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_values.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_values.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/business/metric_adapter/basic_adapter.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/business/metric_adapter/basic_adapter.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_outcome.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_type.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/business/metric_adapter/votes_type.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/business/metric_adapter/votes_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/class_diagram.png` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/class_diagram.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/metric_dao_factory.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/metric_dao_factory.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/srcs.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/srcs.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_members.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_members.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_organization.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_organization.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_voters.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_voters.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_approval_proposal_rate.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_approval_proposal_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_new_additions.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_new_additions.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_organization_activity.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_organization_activity.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_outcome.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_type.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_total_members.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_total_members.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_voters_percentage.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_voters_percentage.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_rate.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_type.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_voters_rate.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_voters_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/data_access/daos/platform_dao.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/data_access/daos/platform_dao.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daohaus/resources/strings.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daohaus/resources/strings.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/business/app_service.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/business/app_service.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_tokens.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_tokens.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_values.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_values.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/business/metric_adapter/majority_type.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/business/metric_adapter/majority_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/business/metric_adapter/metric_adapter.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/business/metric_adapter/metric_adapter.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/business/metric_adapter/proposal_boost_outcome.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/business/metric_adapter/proposal_boost_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/business/metric_adapter/success_ratio_type.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/business/metric_adapter/success_ratio_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/business/metric_adapter/vote_type.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/business/metric_adapter/vote_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/class_diagram.png` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/class_diagram.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/metric_dao_factory.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/metric_dao_factory.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/srcs.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/srcs.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_organization.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_organization.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_users.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_users.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_approval_proposal_rate.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_approval_proposal_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_different_voters_stakers.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_different_voters_stakers.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_organization_activity.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_organization_activity.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_majority.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_majority.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_outcome.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_time_serie.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_time_serie.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_reputation_holders.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_reputation_holders.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_votes_stakes_option.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_votes_stakes_option.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_voters_percentage.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_voters_percentage.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_rate.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_voters_rate.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_voters_rate.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/data_access/daos/platform_dao.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/data_access/daos/platform_dao.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/apps/daostack/resources/strings.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/apps/daostack/resources/strings.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/assets/ABOUT.md` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/ABOUT.md`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/assets/aragon.png` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/aragon.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/assets/callbacks.js` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/callbacks.js`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/assets/cc-by.png` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/cc-by.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/assets/dao-analyzer_header.svg` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/dao-analyzer_header.svg`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/assets/dao-analyzer_logo.svg` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/dao-analyzer_logo.svg`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/assets/daohaus.png` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/daohaus.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/assets/daostack.png` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/daostack.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/assets/favicon.ico` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/assets/github_logo.png` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/github_logo.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/assets/ico-github.svg` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/ico-github.svg`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/assets/img_header.jpg` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/img_header.jpg`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/assets/kaggle_logo.png` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/kaggle_logo.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/assets/logo-GPL.png` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/logo-GPL.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/assets/logo-erc.png` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/logo-erc.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/assets/logo-grasia.png` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/logo-grasia.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/assets/logo-ministerio.png` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/logo-ministerio.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/assets/logo-ucm.png` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/logo-ucm.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/assets/logo_dao_analyzer.png` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/logo_dao_analyzer.png`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/assets/logo_dao_analyzer.svg` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/logo_dao_analyzer.svg`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/assets/logo_dao_analyzer_orig.svg` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/logo_dao_analyzer_orig.svg`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/assets/stylesheet.css` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/assets/stylesheet.css`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/logs.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/logs.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer/web/matomo.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer/web/matomo.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer.egg-info/PKG-INFO` & `dao_analyzer-1.3.2.dev2/dao_analyzer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dao-analyzer
-Version: 1.3.1
+Version: 1.3.2.dev2
 Summary: "A tool to monitor DAO activity"
 Home-page: https://dao-analyzer.science
 Author: David Davó
 Author-email: ddavo@ucm.es
 Project-URL: Source, https://github.com/Grasia/dao-analyzer
 Project-URL: Bug Tracker, https://github.com/Grasia/dao-analyzer/issues
 Project-URL: Changelog, https://github.com/Grasia/dao-analyzer/blob/master/CHANGELOG.md
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: dao-analyzer Version: 1.3.1 Summary: "A tool to
-monitor DAO activity" Home-page: https://dao-analyzer.science Author: David
+Metadata-Version: 2.1 Name: dao-analyzer Version: 1.3.2.dev2 Summary: "A tool
+to monitor DAO activity" Home-page: https://dao-analyzer.science Author: David
 DavÃ³ Author-email: ddavo@ucm.es Project-URL: Source, https://github.com/
 Grasia/dao-analyzer Project-URL: Bug Tracker, https://github.com/Grasia/dao-
 analyzer/issues Project-URL: Changelog, https://github.com/Grasia/dao-analyzer/
 blob/master/CHANGELOG.md Classifier: Development Status :: 5 - Production/
 Stable Classifier: Environment :: Console Classifier: Environment :: Web
 Environment Classifier: Framework :: Dash Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: GNU General Public
```

### Comparing `dao_analyzer-1.3.1/dao_analyzer.egg-info/SOURCES.txt` & `dao_analyzer-1.3.2.dev2/dao_analyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer_components/.eslintrc` & `dao_analyzer-1.3.2.dev2/dao_analyzer_components/.eslintrc`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer_components/MANIFEST.in` & `dao_analyzer-1.3.2.dev2/dao_analyzer_components/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer_components/_validate_init.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer_components/_validate_init.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer_components/dao_analyzer_components/DAOInfo.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer_components/dao_analyzer_components/DAOInfo.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer_components/dao_analyzer_components/DataPoint.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer_components/dao_analyzer_components/DataPoint.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer_components/dao_analyzer_components/ParticipationStat.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer_components/dao_analyzer_components/ParticipationStat.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer_components/dao_analyzer_components/PlatformInfo.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer_components/dao_analyzer_components/PlatformInfo.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer_components/dao_analyzer_components/__init__.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer_components/dao_analyzer_components/__init__.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.css` & `dao_analyzer-1.3.2.dev2/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.css`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js` & `dao_analyzer-1.3.2.dev2/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -42,15 +42,15 @@
             var e = function(t) {
                     return /\/_dash-component-suites\//.test(t.src)
                 }(r()),
                 o = n(t);
             if (!e) return o;
             var i = o.split("/"),
                 a = i.slice(-1)[0].split(".");
-            return a.splice(1, 0, "v0_0_23m1716797304"), i.splice(-1, 1, a.join(".")), i.join("/")
+            return a.splice(1, 0, "v0_0_23m1716797542"), i.splice(-1, 1, a.join(".")), i.join("/")
         }
     }
     var o = {};
     e.r(o), e.d(o, {
         DAOInfo: () => g,
         DataPoint: () => C,
         ParticipationStat: () => m,
```

### Comparing `dao_analyzer-1.3.1/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js.map` & `dao_analyzer-1.3.2.dev2/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.989010989010989%*

 * *Differences: {"'sourcesContent'": "{insert: [(1, 'var getCurrentScript = function() {\\n    var script = "*

 * *                     'document.currentScript;\\n    if (!script) {\\n        /* Shim for IE11 and '*

 * *                     'below */\\n        /* Do not take into account async scripts and inline '*

 * *                     'scripts */\\n\\n        var doc_scripts = '*

 * *                     "document.getElementsByTagName(\\'script\\');\\n        var scripts = "*

 * *                     '[];\\n\\n        for (var i = 0; i < doc_ […]*

```diff
@@ -118,15 +118,15 @@
         "webpack:///./src/lib/components/ParticipationStat.jsx",
         "webpack:///./src/lib/components/DAOInfo.jsx",
         "webpack:///./src/lib/components/PlatformInfo.jsx",
         "webpack:///./src/lib/components/DataPoint.jsx"
     ],
     "sourcesContent": [
         "// The require scope\nvar __webpack_require__ = {};\n\n",
-        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_23m1716797304\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
+        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_23m1716797542\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "const __WEBPACK_NAMESPACE_OBJECT__ = window[\"React\"];",
         "const __WEBPACK_NAMESPACE_OBJECT__ = window[\"PropTypes\"];",
         "import React, { Component } from 'react';\nimport PropTypes from 'prop-types';\n\n/** \n * This class will be used by DAOInfo and PlatformInfo\n */\nexport default class ParticipationStat extends Component {\n    render () {\n        const { text, value } = this.props;\n        if (value) {\n            return (<div><b>{value}</b> {text}</div>);\n        } else {\n            return (<div>{text}</div>);\n        }\n    }\n}\n\nParticipationStat.propTypes = {\n    /**\n     * The text to show\n     */\n    text: PropTypes.string.isRequired,\n\n    /**\n     * The value to highlight, which will be appended to text\n     */\n    value: PropTypes.string,\n\n    /**\n     * The key used by React for optimization\n     */\n    key: PropTypes.string,\n}\n",
```

### Comparing `dao_analyzer-1.3.1/dao_analyzer_components/dao_analyzer_components/metadata.json` & `dao_analyzer-1.3.2.dev2/dao_analyzer_components/dao_analyzer_components/metadata.json`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer_components/dao_analyzer_components/package-info.json` & `dao_analyzer-1.3.2.dev2/dao_analyzer_components/dao_analyzer_components/package-info.json`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer_components/package-lock.json` & `dao_analyzer-1.3.2.dev2/dao_analyzer_components/package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996674057539682%*

 * *Differences: {"'packages'": "{'node_modules/@jridgewell/gen-mapping': {'version': '0.3.5', 'resolved': "*

 * *               "'https://registry.npmjs.org/@jridgewell/gen-mapping/-/gen-mapping-0.3.5.tgz', "*

 * *               "'integrity': "*

 * *               "'sha512-IzL8ZoEDIBRWEzlCcRhOaCupYyN5gdIK+Q6fbFdPDg6HqX6jpkItn7DFIpW9LQzXG6Df9sA7+OKnq0qlz/GaQg==', "*

 * *               "'dependencies': {'@jridgewell/set-array': '^1.2.1', '@jridgewell/trace-mapping': "*

 * *               "'^0.3.24'}}, 'node_modules/@jridgewell/set-array': {'version' […]*

```diff
@@ -1966,25 +1966,25 @@
             },
             "integrity": "sha512-ZXRY4jNvVgSVQ8DL3LTcakaAtXwTVUxE81hslsyD2AtoXW/wVob10HkOJ1X/pAlcI7D+2YoZKg5do8G/w6RYgA==",
             "resolved": "https://registry.npmjs.org/@istanbuljs/schema/-/schema-0.1.3.tgz",
             "version": "0.1.3"
         },
         "node_modules/@jridgewell/gen-mapping": {
             "dependencies": {
-                "@jridgewell/set-array": "^1.0.1",
+                "@jridgewell/set-array": "^1.2.1",
                 "@jridgewell/sourcemap-codec": "^1.4.10",
-                "@jridgewell/trace-mapping": "^0.3.9"
+                "@jridgewell/trace-mapping": "^0.3.24"
             },
             "dev": true,
             "engines": {
                 "node": ">=6.0.0"
             },
-            "integrity": "sha512-HLhSWOLRi875zjjMG/r+Nv0oCW8umGb0BgEhyX3dDX3egwZtB8PqLnjz3yedt8R5StBrzcg4aBpnh8UA9D1BoQ==",
-            "resolved": "https://registry.npmjs.org/@jridgewell/gen-mapping/-/gen-mapping-0.3.3.tgz",
-            "version": "0.3.3"
+            "integrity": "sha512-IzL8ZoEDIBRWEzlCcRhOaCupYyN5gdIK+Q6fbFdPDg6HqX6jpkItn7DFIpW9LQzXG6Df9sA7+OKnq0qlz/GaQg==",
+            "resolved": "https://registry.npmjs.org/@jridgewell/gen-mapping/-/gen-mapping-0.3.5.tgz",
+            "version": "0.3.5"
         },
         "node_modules/@jridgewell/resolve-uri": {
             "dev": true,
             "engines": {
                 "node": ">=6.0.0"
             },
             "integrity": "sha512-dSYZh7HhCDtCKm4QakX0xFpsRDqjjtZf/kjI/v3T3Nwt5r8/qz/M19F9ySyOqU94SXBmeG9ttTul+YnR4LOxFA==",
@@ -1992,43 +1992,43 @@
             "version": "3.1.1"
         },
         "node_modules/@jridgewell/set-array": {
             "dev": true,
             "engines": {
                 "node": ">=6.0.0"
             },
-            "integrity": "sha512-xnkseuNADM0gt2bs+BvhO0p78Mk762YnZdsuzFV018NoG1Sj1SCQvpSqa7XUaTam5vAGasABV9qXASMKnFMwMw==",
-            "resolved": "https://registry.npmjs.org/@jridgewell/set-array/-/set-array-1.1.2.tgz",
-            "version": "1.1.2"
+            "integrity": "sha512-R8gLRTZeyp03ymzP/6Lil/28tGeGEzhx1q2k703KGWRAI1VdvPIXdG70VJc2pAMw3NA6JKL5hhFu1sJX0Mnn/A==",
+            "resolved": "https://registry.npmjs.org/@jridgewell/set-array/-/set-array-1.2.1.tgz",
+            "version": "1.2.1"
         },
         "node_modules/@jridgewell/source-map": {
             "dependencies": {
-                "@jridgewell/gen-mapping": "^0.3.0",
-                "@jridgewell/trace-mapping": "^0.3.9"
+                "@jridgewell/gen-mapping": "^0.3.5",
+                "@jridgewell/trace-mapping": "^0.3.25"
             },
             "dev": true,
-            "integrity": "sha512-UTYAUj/wviwdsMfzoSJspJxbkH5o1snzwX0//0ENX1u/55kkZZkcTZP6u9bwKGkv+dkk9at4m1Cpt0uY80kcpQ==",
-            "resolved": "https://registry.npmjs.org/@jridgewell/source-map/-/source-map-0.3.5.tgz",
-            "version": "0.3.5"
+            "integrity": "sha512-1ZJTZebgqllO79ue2bm3rIGud/bOe0pP5BjSRCRxxYkEZS8STV7zN84UBbiYu7jy+eCKSnVIUgoWWE/tt+shMQ==",
+            "resolved": "https://registry.npmjs.org/@jridgewell/source-map/-/source-map-0.3.6.tgz",
+            "version": "0.3.6"
         },
         "node_modules/@jridgewell/sourcemap-codec": {
             "dev": true,
             "integrity": "sha512-eF2rxCRulEKXHTRiDrDy6erMYWqNw4LPdQ8UQA4huuxaQsVeRPFl2oM8oDGxMFhJUWZf9McpLtJasDDZb/Bpeg==",
             "resolved": "https://registry.npmjs.org/@jridgewell/sourcemap-codec/-/sourcemap-codec-1.4.15.tgz",
             "version": "1.4.15"
         },
         "node_modules/@jridgewell/trace-mapping": {
             "dependencies": {
                 "@jridgewell/resolve-uri": "^3.1.0",
                 "@jridgewell/sourcemap-codec": "^1.4.14"
             },
             "dev": true,
-            "integrity": "sha512-kf37QtfW+Hwx/buWGMPcR60iF9ziHa6r/CZJIHbmcm4+0qrXiVdxegAH0F6yddEVQ7zdkjcGCgCzUu+BcbhQxw==",
-            "resolved": "https://registry.npmjs.org/@jridgewell/trace-mapping/-/trace-mapping-0.3.19.tgz",
-            "version": "0.3.19"
+            "integrity": "sha512-vNk6aEwybGtawWmy/PzwnGDOjCkLWSD2wqvjGGAgOAwCGWySYXfYoxt00IJkTF+8Lb57DwOb3Aa0o9CApepiYQ==",
+            "resolved": "https://registry.npmjs.org/@jridgewell/trace-mapping/-/trace-mapping-0.3.25.tgz",
+            "version": "0.3.25"
         },
         "node_modules/@leichtgewicht/ip-codec": {
             "dev": true,
             "integrity": "sha512-Hcv+nVC0kZnQ3tD9GVu5xSMR4VVYOteQIr/hwFPVEvPdlXqgGEuRjiheChHgdM+JyqdgNcmzZOX/tnl0JOiI7A==",
             "resolved": "https://registry.npmjs.org/@leichtgewicht/ip-codec/-/ip-codec-2.0.4.tgz",
             "version": "2.0.4"
         },
@@ -2201,17 +2201,17 @@
             "dev": true,
             "integrity": "sha512-9K4zoImiZc3HlIp6AVUDE4CWYx22a+lhSZMYNpbjW04+YF0KWj4pJXnEMjdnFTiQibFFmElcsasJXDbdI/EPhA==",
             "resolved": "https://registry.npmjs.org/@types/eslint-scope/-/eslint-scope-3.7.4.tgz",
             "version": "3.7.4"
         },
         "node_modules/@types/estree": {
             "dev": true,
-            "integrity": "sha512-LG4opVs2ANWZ1TJoKc937iMmNstM/d0ae1vNbnBvBhqCSezgVUOzcLCqbI5elV8Vy6WKwKjaqR+zO9VKirBBCA==",
-            "resolved": "https://registry.npmjs.org/@types/estree/-/estree-1.0.1.tgz",
-            "version": "1.0.1"
+            "integrity": "sha512-/kYRxGDLWzHOB7q+wtSUQlFrtcdUccpfy+X+9iMBpHK8QLLhx2wIPYuS5DYtR9Wa/YlZAbIovy7qVdB1Aq6Lyw==",
+            "resolved": "https://registry.npmjs.org/@types/estree/-/estree-1.0.5.tgz",
+            "version": "1.0.5"
         },
         "node_modules/@types/express": {
             "dependencies": {
                 "@types/body-parser": "*",
                 "@types/express-serve-static-core": "^4.17.33",
                 "@types/qs": "*",
                 "@types/serve-static": "*"
@@ -2346,17 +2346,17 @@
         },
         "node_modules/@webassemblyjs/ast": {
             "dependencies": {
                 "@webassemblyjs/helper-numbers": "1.11.6",
                 "@webassemblyjs/helper-wasm-bytecode": "1.11.6"
             },
             "dev": true,
-            "integrity": "sha512-IN1xI7PwOvLPgjcf180gC1bqn3q/QaOCwYUahIOhbYUu8KA/3tw2RT/T0Gidi1l7Hhj5D/INhJxiICObqpMu4Q==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.6.tgz",
-            "version": "1.11.6"
+            "integrity": "sha512-EKfMUOPRRUTy5UII4qJDGPpqfwjOmZ5jeGFwid9mnoqIFK+e0vqoi1qH56JpmZSzEL53jKnNzScdmftJyG5xWg==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.12.1.tgz",
+            "version": "1.12.1"
         },
         "node_modules/@webassemblyjs/floating-point-hex-parser": {
             "dev": true,
             "integrity": "sha512-ejAj9hfRJ2XMsNHk/v6Fu2dGS+i4UaXBXGemOfQ/JfQ6mdQg/WXtwleQRLLS4OvfDhv8rYnVwH27YJLMyYsxhw==",
             "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.6.tgz",
             "version": "1.11.6"
         },
@@ -2364,17 +2364,17 @@
             "dev": true,
             "integrity": "sha512-o0YkoP4pVu4rN8aTJgAyj9hC2Sv5UlkzCHhxqWj8butaLvnpdc2jOwh4ewE6CX0txSfLn/UYaV/pheS2Txg//Q==",
             "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.6.tgz",
             "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/helper-buffer": {
             "dev": true,
-            "integrity": "sha512-z3nFzdcp1mb8nEOFFk8DrYLpHvhKC3grJD2ardfKOzmbmJvEf/tPIqCY+sNcwZIY8ZD7IkB2l7/pqhUhqm7hLA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.6.tgz",
-            "version": "1.11.6"
+            "integrity": "sha512-nzJwQw99DNDKr9BVCOZcLuJJUlqkJh+kVzVl6Fmq/tI5ZtEyWT1KZMyOXltXLZJmDtvLCDgwsyrkohEtopTXCw==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.12.1.tgz",
+            "version": "1.12.1"
         },
         "node_modules/@webassemblyjs/helper-numbers": {
             "dependencies": {
                 "@webassemblyjs/floating-point-hex-parser": "1.11.6",
                 "@webassemblyjs/helper-api-error": "1.11.6",
                 "@xtuc/long": "4.2.2"
             },
@@ -2387,23 +2387,23 @@
             "dev": true,
             "integrity": "sha512-sFFHKwcmBprO9e7Icf0+gddyWYDViL8bpPjJJl0WHxCdETktXdmtWLGVzoHbqUcY4Be1LkNfwTmXOJUFZYSJdA==",
             "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.6.tgz",
             "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/helper-wasm-section": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.6",
-                "@webassemblyjs/helper-buffer": "1.11.6",
+                "@webassemblyjs/ast": "1.12.1",
+                "@webassemblyjs/helper-buffer": "1.12.1",
                 "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
-                "@webassemblyjs/wasm-gen": "1.11.6"
+                "@webassemblyjs/wasm-gen": "1.12.1"
             },
             "dev": true,
-            "integrity": "sha512-LPpZbSOwTpEC2cgn4hTydySy1Ke+XEu+ETXuoyvuyezHO3Kjdu90KK95Sh9xTbmjrCsUwvWwCOQQNta37VrS9g==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.6.tgz",
-            "version": "1.11.6"
+            "integrity": "sha512-Jif4vfB6FJlUlSbgEMHUyk1j234GTNG9dBJ4XJdOySoj518Xj0oGsNi59cUQF4RRMS9ouBUxDDdyBVfPTypa5g==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.12.1.tgz",
+            "version": "1.12.1"
         },
         "node_modules/@webassemblyjs/ieee754": {
             "dependencies": {
                 "@xtuc/ieee754": "^1.2.0"
             },
             "dev": true,
             "integrity": "sha512-LM4p2csPNvbij6U1f19v6WR56QZ8JcHg3QIJTlSwzFcmx6WSORicYj6I63f9yU1kEUtrpG+kjkiIAkevHpDXrg==",
@@ -2423,76 +2423,76 @@
             "dev": true,
             "integrity": "sha512-vtXf2wTQ3+up9Zsg8sa2yWiQpzSsMyXj0qViVP6xKGCUT8p8YJ6HqI7l5eCnWx1T/FYdsv07HQs2wTFbbof/RA==",
             "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.6.tgz",
             "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/wasm-edit": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.6",
-                "@webassemblyjs/helper-buffer": "1.11.6",
+                "@webassemblyjs/ast": "1.12.1",
+                "@webassemblyjs/helper-buffer": "1.12.1",
                 "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
-                "@webassemblyjs/helper-wasm-section": "1.11.6",
-                "@webassemblyjs/wasm-gen": "1.11.6",
-                "@webassemblyjs/wasm-opt": "1.11.6",
-                "@webassemblyjs/wasm-parser": "1.11.6",
-                "@webassemblyjs/wast-printer": "1.11.6"
+                "@webassemblyjs/helper-wasm-section": "1.12.1",
+                "@webassemblyjs/wasm-gen": "1.12.1",
+                "@webassemblyjs/wasm-opt": "1.12.1",
+                "@webassemblyjs/wasm-parser": "1.12.1",
+                "@webassemblyjs/wast-printer": "1.12.1"
             },
             "dev": true,
-            "integrity": "sha512-Ybn2I6fnfIGuCR+Faaz7YcvtBKxvoLV3Lebn1tM4o/IAJzmi9AWYIPWpyBfU8cC+JxAO57bk4+zdsTjJR+VTOw==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.6.tgz",
-            "version": "1.11.6"
+            "integrity": "sha512-1DuwbVvADvS5mGnXbE+c9NfA8QRcZ6iKquqjjmR10k6o+zzsRVesil54DKexiowcFCPdr/Q0qaMgB01+SQ1u6g==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.12.1.tgz",
+            "version": "1.12.1"
         },
         "node_modules/@webassemblyjs/wasm-gen": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/ast": "1.12.1",
                 "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
                 "@webassemblyjs/ieee754": "1.11.6",
                 "@webassemblyjs/leb128": "1.11.6",
                 "@webassemblyjs/utf8": "1.11.6"
             },
             "dev": true,
-            "integrity": "sha512-3XOqkZP/y6B4F0PBAXvI1/bky7GryoogUtfwExeP/v7Nzwo1QLcq5oQmpKlftZLbT+ERUOAZVQjuNVak6UXjPA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.6.tgz",
-            "version": "1.11.6"
+            "integrity": "sha512-TDq4Ojh9fcohAw6OIMXqiIcTq5KUXTGRkVxbSo1hQnSy6lAM5GSdfwWeSxpAo0YzgsgF182E/U0mDNhuA0tW7w==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.12.1.tgz",
+            "version": "1.12.1"
         },
         "node_modules/@webassemblyjs/wasm-opt": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.6",
-                "@webassemblyjs/helper-buffer": "1.11.6",
-                "@webassemblyjs/wasm-gen": "1.11.6",
-                "@webassemblyjs/wasm-parser": "1.11.6"
+                "@webassemblyjs/ast": "1.12.1",
+                "@webassemblyjs/helper-buffer": "1.12.1",
+                "@webassemblyjs/wasm-gen": "1.12.1",
+                "@webassemblyjs/wasm-parser": "1.12.1"
             },
             "dev": true,
-            "integrity": "sha512-cOrKuLRE7PCe6AsOVl7WasYf3wbSo4CeOk6PkrjS7g57MFfVUF9u6ysQBBODX0LdgSvQqRiGz3CXvIDKcPNy4g==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.6.tgz",
-            "version": "1.11.6"
+            "integrity": "sha512-Jg99j/2gG2iaz3hijw857AVYekZe2SAskcqlWIZXjji5WStnOpVoat3gQfT/Q5tb2djnCjBtMocY/Su1GfxPBg==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.12.1.tgz",
+            "version": "1.12.1"
         },
         "node_modules/@webassemblyjs/wasm-parser": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/ast": "1.12.1",
                 "@webassemblyjs/helper-api-error": "1.11.6",
                 "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
                 "@webassemblyjs/ieee754": "1.11.6",
                 "@webassemblyjs/leb128": "1.11.6",
                 "@webassemblyjs/utf8": "1.11.6"
             },
             "dev": true,
-            "integrity": "sha512-6ZwPeGzMJM3Dqp3hCsLgESxBGtT/OeCvCZ4TA1JUPYgmhAx38tTPR9JaKy0S5H3evQpO/h2uWs2j6Yc/fjkpTQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.6.tgz",
-            "version": "1.11.6"
+            "integrity": "sha512-xikIi7c2FHXysxXe3COrVUPSheuBtpcfhbpFj4gmu7KRLYOzANztwUU0IbsqvMqzuNK2+glRGWCEqZo1WCLyAQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.12.1.tgz",
+            "version": "1.12.1"
         },
         "node_modules/@webassemblyjs/wast-printer": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/ast": "1.12.1",
                 "@xtuc/long": "4.2.2"
             },
             "dev": true,
-            "integrity": "sha512-JM7AhRcE+yW2GWYaKeHL5vt4xqee5N2WcezptmgyhNS+ScggqcT1OtXykhAb13Sn5Yas0j2uv9tHgrjwvzAP4A==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.6.tgz",
-            "version": "1.11.6"
+            "integrity": "sha512-+X4WAlOisVWQMikjbcvY2e0rwPsKQ9F688lksZhBcPycBBuii3O7m8FACbDMWDojpAqvjIncrG8J0XHKyQfVeA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.12.1.tgz",
+            "version": "1.12.1"
         },
         "node_modules/@webpack-cli/configtest": {
             "dev": true,
             "engines": {
                 "node": ">=14.15.0"
             },
             "integrity": "sha512-wy0mglZpDSiSS0XHrVR+BAdId2+yxPSoJW8fsna3ZpYSlufjvxnP4YbKTCBZnNIcGN4r6ZPXV55X4mYExOfLmw==",
@@ -3799,17 +3799,17 @@
                 "graceful-fs": "^4.2.4",
                 "tapable": "^2.2.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=10.13.0"
             },
-            "integrity": "sha512-LXYT42KJ7lpIKECr2mAXIaMldcNCh/7E0KBKOu4KSfkHmP+mZmSs+8V5gBAqisWBy0OO4W5Oyys0GO1Y8KtdKg==",
-            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.15.0.tgz",
-            "version": "5.15.0"
+            "integrity": "sha512-4U5pNsuDl0EhuZpq46M5xPslstkviJuhrdobaRDBk2Jy2KO37FDAJl4lb2KlNabxT0m4MTK2UHNrsAcphE8nyw==",
+            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.16.1.tgz",
+            "version": "5.16.1"
         },
         "node_modules/envinfo": {
             "bin": {
                 "envinfo": "dist/cli.js"
             },
             "dev": true,
             "engines": {
@@ -8791,51 +8791,51 @@
                 "commander": "^2.20.0",
                 "source-map-support": "~0.5.20"
             },
             "dev": true,
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-6p1DjHeuluwxDXcuT9VR8p64klWJKo1ILiy19s6C9+0Bh2+NWTX6nD9EPppiER4ICkHDVB1RkVpin/YW2nQn/g==",
-            "resolved": "https://registry.npmjs.org/terser/-/terser-5.19.4.tgz",
-            "version": "5.19.4"
+            "integrity": "sha512-Q1JFAoUKE5IMfI4Z/lkE/E6+SwgzO+x4tq4v1AyBLRj8VSYvRO6A/rQrPg1yud4g0En9EKI1TvFRF2tQFcoUkg==",
+            "resolved": "https://registry.npmjs.org/terser/-/terser-5.31.0.tgz",
+            "version": "5.31.0"
         },
         "node_modules/terser-webpack-plugin": {
             "dependencies": {
-                "@jridgewell/trace-mapping": "^0.3.17",
+                "@jridgewell/trace-mapping": "^0.3.20",
                 "jest-worker": "^27.4.5",
                 "schema-utils": "^3.1.1",
                 "serialize-javascript": "^6.0.1",
-                "terser": "^5.16.8"
+                "terser": "^5.26.0"
             },
             "dev": true,
             "engines": {
                 "node": ">= 10.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-ZuXsqE07EcggTWQjXUj+Aot/OMcD0bMKGgF63f7UxYcu5/AJF53aIpK1YoP5xR9l6s/Hy2b+t1AM0bLNPRuhwA==",
+            "integrity": "sha512-BKFPWlPDndPs+NGGCr1U59t0XScL5317Y0UReNrHaw9/FwhPENlq6bfgs+4yPfyP51vqC1bQ4rp1EfXW5ZSH9w==",
             "peerDependencies": {
                 "webpack": "^5.1.0"
             },
             "peerDependenciesMeta": {
                 "@swc/core": {
                     "optional": true
                 },
                 "esbuild": {
                     "optional": true
                 },
                 "uglify-js": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.9.tgz",
-            "version": "5.3.9"
+            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.10.tgz",
+            "version": "5.3.10"
         },
         "node_modules/terser-webpack-plugin/node_modules/schema-utils": {
             "dependencies": {
                 "@types/json-schema": "^7.0.8",
                 "ajv": "^6.12.5",
                 "ajv-keywords": "^3.5.2"
             },
@@ -9294,17 +9294,17 @@
                 "glob-to-regexp": "^0.4.1",
                 "graceful-fs": "^4.1.2"
             },
             "dev": true,
             "engines": {
                 "node": ">=10.13.0"
             },
-            "integrity": "sha512-Lcvm7MGST/4fup+ifyKi2hjyIAwcdI4HRgtvTpIUxBRhB+RFtUh8XtDOxUfctVCnhVi+QQj49i91OyvzkJl6cg==",
-            "resolved": "https://registry.npmjs.org/watchpack/-/watchpack-2.4.0.tgz",
-            "version": "2.4.0"
+            "integrity": "sha512-8wrBCMtVhqcXP2Sup1ctSkga6uc2Bx0IIvKyT7yTFier5AXHooSI+QyQQAtTb7+E0IUCCKyTFmXqdqgum2XWGg==",
+            "resolved": "https://registry.npmjs.org/watchpack/-/watchpack-2.4.1.tgz",
+            "version": "2.4.1"
         },
         "node_modules/wbuf": {
             "dependencies": {
                 "minimalistic-assert": "^1.0.0"
             },
             "dev": true,
             "integrity": "sha512-O84QOnr0icsbFGLS0O3bI5FswxzRr8/gHwWkDlQFskhSPryQXvrTMxjxGP4+iWYoauLoBvfDpkrOauZ+0iZpDA==",
@@ -9313,54 +9313,54 @@
         },
         "node_modules/webpack": {
             "bin": {
                 "webpack": "bin/webpack.js"
             },
             "dependencies": {
                 "@types/eslint-scope": "^3.7.3",
-                "@types/estree": "^1.0.0",
-                "@webassemblyjs/ast": "^1.11.5",
-                "@webassemblyjs/wasm-edit": "^1.11.5",
-                "@webassemblyjs/wasm-parser": "^1.11.5",
+                "@types/estree": "^1.0.5",
+                "@webassemblyjs/ast": "^1.12.1",
+                "@webassemblyjs/wasm-edit": "^1.12.1",
+                "@webassemblyjs/wasm-parser": "^1.12.1",
                 "acorn": "^8.7.1",
                 "acorn-import-assertions": "^1.9.0",
-                "browserslist": "^4.14.5",
+                "browserslist": "^4.21.10",
                 "chrome-trace-event": "^1.0.2",
-                "enhanced-resolve": "^5.15.0",
+                "enhanced-resolve": "^5.16.0",
                 "es-module-lexer": "^1.2.1",
                 "eslint-scope": "5.1.1",
                 "events": "^3.2.0",
                 "glob-to-regexp": "^0.4.1",
-                "graceful-fs": "^4.2.9",
+                "graceful-fs": "^4.2.11",
                 "json-parse-even-better-errors": "^2.3.1",
                 "loader-runner": "^4.2.0",
                 "mime-types": "^2.1.27",
                 "neo-async": "^2.6.2",
                 "schema-utils": "^3.2.0",
                 "tapable": "^2.1.1",
-                "terser-webpack-plugin": "^5.3.7",
-                "watchpack": "^2.4.0",
+                "terser-webpack-plugin": "^5.3.10",
+                "watchpack": "^2.4.1",
                 "webpack-sources": "^3.2.3"
             },
             "dev": true,
             "engines": {
                 "node": ">=10.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-JmcgNZ1iKj+aiR0OvTYtWQqJwq37Pf683dY9bVORwVbUrDhLhdn/PlO2sHsFHPkj7sHNQF3JwaAkp49V+Sq1tQ==",
+            "integrity": "sha512-rzVwlLeBWHJbmgTC/8TvAcu5vpJNII+MelQpylD4jNERPwpBJOE2lEcko1zJX3QJeLjTTAnQxn/OJ8bjDzVQaw==",
             "peerDependenciesMeta": {
                 "webpack-cli": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.88.2.tgz",
-            "version": "5.88.2"
+            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.91.0.tgz",
+            "version": "5.91.0"
         },
         "node_modules/webpack-cli": {
             "bin": {
                 "webpack-cli": "bin/cli.js"
             },
             "dependencies": {
                 "@discoveryjs/json-ext": "^0.5.0",
```

### Comparing `dao_analyzer-1.3.1/dao_analyzer_components/package.json` & `dao_analyzer-1.3.2.dev2/dao_analyzer_components/package.json`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer_components/setup.py` & `dao_analyzer-1.3.2.dev2/dao_analyzer_components/setup.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer_components/src/lib/components/DAOInfo.jsx` & `dao_analyzer-1.3.2.dev2/dao_analyzer_components/src/lib/components/DAOInfo.jsx`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer_components/src/lib/components/DataPoint.jsx` & `dao_analyzer-1.3.2.dev2/dao_analyzer_components/src/lib/components/DataPoint.jsx`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer_components/src/lib/components/ParticipationStat.jsx` & `dao_analyzer-1.3.2.dev2/dao_analyzer_components/src/lib/components/ParticipationStat.jsx`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer_components/src/lib/components/PlatformInfo.jsx` & `dao_analyzer-1.3.2.dev2/dao_analyzer_components/src/lib/components/PlatformInfo.jsx`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/dao_analyzer_components/webpack.config.js` & `dao_analyzer-1.3.2.dev2/dao_analyzer_components/webpack.config.js`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/scripts/archive/names.ipynb` & `dao_analyzer-1.3.2.dev2/scripts/archive/names.ipynb`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/scripts/archive/uploadToKaggle.sh` & `dao_analyzer-1.3.2.dev2/scripts/archive/uploadToKaggle.sh`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/scripts/checkContinue.sh` & `dao_analyzer-1.3.2.dev2/scripts/checkContinue.sh`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/scripts/datawarehouseDiff.py` & `dao_analyzer-1.3.2.dev2/scripts/datawarehouseDiff.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/scripts/updateAragonNames.py` & `dao_analyzer-1.3.2.dev2/scripts/updateAragonNames.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/scripts/uploadDataWarehouse.py` & `dao_analyzer-1.3.2.dev2/scripts/uploadDataWarehouse.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/setup.cfg` & `dao_analyzer-1.3.2.dev2/setup.cfg`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/setup.py` & `dao_analyzer-1.3.2.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/mocks/api_requester_mock.py` & `dao_analyzer-1.3.2.dev2/test/mocks/api_requester_mock.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/mocks/unix_date_builder.py` & `dao_analyzer-1.3.2.dev2/test/mocks/unix_date_builder.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/unit/apps/aragon/data_access/daos/metric/strategy/test_aragon_st_new_additions.py` & `dao_analyzer-1.3.2.dev2/test/unit/apps/aragon/data_access/daos/metric/strategy/test_aragon_st_new_additions.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_organization_aragon.py` & `dao_analyzer-1.3.2.dev2/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_organization_aragon.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_token_holders.py` & `dao_analyzer-1.3.2.dev2/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_token_holders.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_cast_type.py` & `dao_analyzer-1.3.2.dev2/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_cast_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_installed_apps.py` & `dao_analyzer-1.3.2.dev2/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_installed_apps.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_vote_outcome.py` & `dao_analyzer-1.3.2.dev2/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_vote_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/unit/apps/common/api/graphql/test_query_builder.py` & `dao_analyzer-1.3.2.dev2/test/unit/apps/common/api/graphql/test_query_builder.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/unit/apps/common/business/transfers/test_organization.py` & `dao_analyzer-1.3.2.dev2/test/unit/apps/common/business/transfers/test_organization.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_members.py` & `dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_members.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_organization_daohaus.py` & `dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_organization_daohaus.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_voters.py` & `dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_voters.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_dproposal_outcome.py` & `dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_dproposal_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_new_additions.py` & `dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_new_additions.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_proposal_type.py` & `dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_proposal_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_total_members.py` & `dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_total_members.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_votes_type.py` & `dao_analyzer-1.3.2.dev2/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_votes_type.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_organization_daostack.py` & `dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_organization_daostack.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_users.py` & `dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_users.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_diff_voters_stakers.py` & `dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_diff_voters_stakers.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_majority.py` & `dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_majority.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_outcome.py` & `dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_outcome.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_time_serie.py` & `dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_time_serie.py`

 * *Files identical despite different names*

### Comparing `dao_analyzer-1.3.1/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_voters_percentage.py` & `dao_analyzer-1.3.2.dev2/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_voters_percentage.py`

 * *Files identical despite different names*

