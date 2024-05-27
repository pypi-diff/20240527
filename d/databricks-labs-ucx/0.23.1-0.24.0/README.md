# Comparing `tmp/databricks_labs_ucx-0.23.1.tar.gz` & `tmp/databricks_labs_ucx-0.24.0.tar.gz`

## Comparing `databricks_labs_ucx-0.23.1.tar` & `databricks_labs_ucx-0.24.0.tar`

### file list

```diff
@@ -1,172 +1,185 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/__about__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/__init__.py
--rw-r--r--   0        0        0    19819 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/cli.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/config.py
--rw-r--r--   0        0        0    30024 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/install.py
--rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/runtime.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/account/__init__.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/account/aggregate.py
--rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/account/metastores.py
--rw-r--r--   0        0        0    14043 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/account/workspaces.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/__init__.py
--rw-r--r--   0        0        0    16138 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/aws.py
--rw-r--r--   0        0        0     9793 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/azure.py
--rw-r--r--   0        0        0     9415 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/clusters.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/crawlers.py
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/init_scripts.py
--rw-r--r--   0        0        0    14899 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/jobs.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/pipelines.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/secrets.py
--rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/workflows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/aws/__init__.py
--rw-r--r--   0        0        0    13546 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/aws/access.py
--rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/aws/credentials.py
--rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/aws/locations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/azure/__init__.py
--rw-r--r--   0        0        0    17739 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/azure/access.py
--rw-r--r--   0        0        0    15098 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/azure/credentials.py
--rw-r--r--   0        0        0    10721 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/azure/locations.py
--rw-r--r--   0        0        0    25091 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/azure/resources.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/contexts/__init__.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/contexts/account_cli.py
--rw-r--r--   0        0        0    15204 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/contexts/application.py
--rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/contexts/workflow_task.py
--rw-r--r--   0        0        0     6192 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/contexts/workspace_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/framework/__init__.py
--rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/framework/crawlers.py
--rw-r--r--   0        0        0    15783 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/framework/dashboards.py
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/framework/tasks.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/framework/utils.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/__init__.py
--rw-r--r--   0        0        0     7530 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/catalog_schema.py
--rw-r--r--   0        0        0    29222 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/grants.py
--rw-r--r--   0        0        0    20209 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/locations.py
--rw-r--r--   0        0        0    10115 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/mapping.py
--rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/migration_status.py
--rw-r--r--   0        0        0    22506 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/table_migrate.py
--rw-r--r--   0        0        0    12269 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/table_move.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/table_size.py
--rw-r--r--   0        0        0    17578 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/tables.py
--rw-r--r--   0        0        0     5796 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/tables.scala
--rw-r--r--   0        0        0     6507 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/udfs.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/verification.py
--rw-r--r--   0        0        0     7347 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/view_migrate.py
--rw-r--r--   0        0        0     8835 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/workflows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/installer/__init__.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/installer/hms_lineage.py
--rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/installer/logs.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/installer/mixins.py
--rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/installer/policy.py
--rw-r--r--   0        0        0    33434 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/installer/workflows.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/mixins/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/mixins/__init__.py
--rw-r--r--   0        0        0    47495 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/mixins/fixtures.py
--rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/mixins/redash.py
--rw-r--r--   0        0        0    14144 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/mixins/wspath.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/azure/05_0_azure_service_principals.sql
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/00_0_metastore_assignment.md
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/00_4_is_incompatible_submit_run_detected.sql
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/01_0_group_migration.md
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/01_2_group_migration.sql
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/01_5_group_migration_complexity.sql
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/02_0_data_modeling.md
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/02_2_uc_data_modeling.sql
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/02_5_uc_data_modeling_complexity.sql
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/03_0_data_migration.md
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/03_2_data_migration_summary.sql
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/03_5_data_migration_complexity.sql
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/interactive/00_0_interactive.md
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/interactive/01_0_compute_access_mode_limitation_summary.sql
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/interactive/02_0_cluster_summary.md
--rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/interactive/03_0_cluster_summary.sql
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/00_0_compatibility.sql
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/00_1_count_total_databases.sql
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/00_2_count_table_failures.sql
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/00_3_count_total_tables.sql
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/00_4_count_external_locations.sql
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/00_5_count_total_views.sql
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/00_6_count_total_udfs.sql
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/00___assessment_overview.md
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/01_0_count_jobs.sql
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/02_2_count_table_by_storage.sql
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/05_0_object_readiness.sql
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/05_2_assessment_summary.sql
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/05___findings_summary.md
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/10_0_all_tables.sql
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/10_0_all_udfs.sql
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/10_0_database_summary.sql
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/10___data_summary.md
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/15_0_external_locations.sql
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/15_3_mount_points.sql
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/15___storage_summary.md
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/20_0_cluster_policies.sql
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/20_0_clusters.sql
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/20___compute_summary.md
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/30_0_job_summary.md
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/30_3_job_details.sql
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/30_3_jobs.sql
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/30_4_submit_runs.sql
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/30_5_submit_runs.sql
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/40_0_pipelines.sql
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/40_2_logs.sql
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/40_3_global_init_scripts.sql
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/40___last_summary.md
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/README.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/migration/main/00_0_migration_overview.md
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/migration/main/01_0_data_object_migration_status.md
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/migration/main/01_1_data_object_migration_status.sql
--rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/views/code_patterns.sql
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/views/grant_detail.sql
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/views/misc_patterns.sql
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/views/objects.sql
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/views/table_estimates.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/__init__.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/ast_helpers.py
--rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/base.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/dbfs.py
--rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/files.py
--rw-r--r--   0        0        0    16733 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/graph.py
--rw-r--r--   0        0        0    10736 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/jobs.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/languages.py
--rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/lsp.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/path_lookup.py
--rw-r--r--   0        0        0    16508 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/pyspark.py
--rw-r--r--   0        0        0    11559 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/python_linter.py
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/queries.py
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/redash.py
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/site_packages.py
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/spark_connect.py
--rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/table_creation.py
--rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/whitelist.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/workflows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/notebooks/__init__.py
--rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/notebooks/cells.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/notebooks/loaders.py
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/notebooks/migrator.py
--rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/notebooks/sources.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/upgrades/v0.15.0_added_cluster_policy.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/upgrades/v0.16.0_changing_cluster_table_schema.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/upgrades/v0.20.0_add_is_partitioned_column.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/upgrades/v0.23.0_add_assessment_to_udf.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/upgrades/v0.4.0_added_log_dir.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/__init__.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/base.py
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/clusters.py
--rw-r--r--   0        0        0    18962 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/generic.py
--rw-r--r--   0        0        0    34574 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/groups.py
--rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/listing.py
--rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/manager.py
--rw-r--r--   0        0        0    12579 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/redash.py
--rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/scim.py
--rw-r--r--   0        0        0     5966 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/secrets.py
--rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/tacl.py
--rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/workflows.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/.gitignore
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/LICENSE
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/NOTICE
--rw-r--r--   0        0        0    65891 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/README.md
--rw-r--r--   0        0        0    28530 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/pyproject.toml
--rw-r--r--   0        0        0    67573 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/__about__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/__init__.py
+-rw-r--r--   0        0        0    20289 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/cli.py
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/config.py
+-rw-r--r--   0        0        0    34228 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/install.py
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/runtime.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/uninstall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/account/__init__.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/account/aggregate.py
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/account/metastores.py
+-rw-r--r--   0        0        0    14043 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/account/workspaces.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/assessment/__init__.py
+-rw-r--r--   0        0        0    16630 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/assessment/aws.py
+-rw-r--r--   0        0        0     9793 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/assessment/azure.py
+-rw-r--r--   0        0        0     9415 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/assessment/clusters.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/assessment/crawlers.py
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/assessment/init_scripts.py
+-rw-r--r--   0        0        0    14899 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/assessment/jobs.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/assessment/pipelines.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/assessment/secrets.py
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/assessment/workflows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/aws/__init__.py
+-rw-r--r--   0        0        0    13663 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/aws/access.py
+-rw-r--r--   0        0        0     8811 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/aws/credentials.py
+-rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/aws/locations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/azure/__init__.py
+-rw-r--r--   0        0        0    17739 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/azure/access.py
+-rw-r--r--   0        0        0    15098 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/azure/credentials.py
+-rw-r--r--   0        0        0    10721 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/azure/locations.py
+-rw-r--r--   0        0        0    25091 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/azure/resources.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/contexts/__init__.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/contexts/account_cli.py
+-rw-r--r--   0        0        0    16550 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/contexts/application.py
+-rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/contexts/workflow_task.py
+-rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/contexts/workspace_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/framework/__init__.py
+-rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/framework/crawlers.py
+-rw-r--r--   0        0        0    15783 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/framework/dashboards.py
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/framework/tasks.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/framework/utils.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/__init__.py
+-rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/catalog_schema.py
+-rw-r--r--   0        0        0    29222 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/grants.py
+-rw-r--r--   0        0        0    20447 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/locations.py
+-rw-r--r--   0        0        0    11876 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/mapping.py
+-rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/migration_status.py
+-rw-r--r--   0        0        0    24296 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/table_migrate.py
+-rw-r--r--   0        0        0    12269 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/table_move.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/table_size.py
+-rw-r--r--   0        0        0    18072 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/tables.py
+-rw-r--r--   0        0        0     5796 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/tables.scala
+-rw-r--r--   0        0        0     6507 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/udfs.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/verification.py
+-rw-r--r--   0        0        0     7347 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/view_migrate.py
+-rw-r--r--   0        0        0    10009 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/workflows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/installer/__init__.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/installer/hms_lineage.py
+-rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/installer/logs.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/installer/mixins.py
+-rw-r--r--   0        0        0    11316 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/installer/policy.py
+-rw-r--r--   0        0        0    34544 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/installer/workflows.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/mixins/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/mixins/__init__.py
+-rw-r--r--   0        0        0    49659 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/mixins/fixtures.py
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/mixins/redash.py
+-rw-r--r--   0        0        0    14173 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/mixins/wspath.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/azure/05_0_azure_service_principals.sql
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/estimates/00_0_metastore_assignment.md
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/estimates/00_4_is_incompatible_submit_run_detected.sql
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/estimates/01_0_group_migration.md
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/estimates/01_2_group_migration.sql
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/estimates/01_5_group_migration_complexity.sql
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/estimates/02_0_data_modeling.md
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/estimates/02_2_uc_data_modeling.sql
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/estimates/02_5_uc_data_modeling_complexity.sql
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/estimates/03_0_data_migration.md
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/estimates/03_2_data_migration_summary.sql
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/estimates/03_5_data_migration_complexity.sql
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/interactive/00_0_interactive.md
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/interactive/01_0_compute_access_mode_limitation_summary.sql
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/interactive/02_0_cluster_summary.md
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/interactive/03_0_cluster_summary.sql
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/00_0_compatibility.sql
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/00_1_count_total_databases.sql
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/00_2_count_table_failures.sql
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/00_3_count_total_tables.sql
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/00_4_count_external_locations.sql
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/00_5_count_total_views.sql
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/00_6_count_total_udfs.sql
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/00___assessment_overview.md
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/01_0_count_jobs.sql
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/02_2_count_table_by_storage.sql
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/05_0_object_readiness.sql
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/05_2_assessment_summary.sql
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/05___findings_summary.md
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/10_0_all_tables.sql
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/10_0_all_udfs.sql
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/10_0_database_summary.sql
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/10___data_summary.md
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/15_0_external_locations.sql
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/15_3_mount_points.sql
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/15___storage_summary.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/20_0_cluster_policies.sql
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/20_0_clusters.sql
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/20___compute_summary.md
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/30_0_job_summary.md
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/30_3_job_details.sql
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/30_3_jobs.sql
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/30_4_submit_runs.sql
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/30_5_submit_runs.sql
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/40_0_pipelines.sql
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/40_2_logs.sql
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/40_3_global_init_scripts.sql
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/40___last_summary.md
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/README.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/migration/main/00_0_migration_overview.md
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/migration/main/01_0_data_object_migration_status.md
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/migration/main/01_1_data_object_migration_summary.sql
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/migration/main/02_0_code_compatibility_problems.md
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/migration/main/02_1_code_compatibility_problems.sql
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/migration/main/02_1_data_reconciliation_summary.sql
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/migration/main/03_1_data_reconciliation_status.sql
+-rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/views/code_patterns.sql
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/views/grant_detail.sql
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/views/misc_patterns.sql
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/views/objects.sql
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/views/reconciliation_results.sql
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/views/table_estimates.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/recon/__init__.py
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/recon/base.py
+-rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/recon/data_comparator.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/recon/data_profiler.py
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/recon/metadata_retriever.py
+-rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/recon/migration_recon.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/recon/schema_comparator.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/recon/workflows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/__init__.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/ast_helpers.py
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/base.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/dbfs.py
+-rw-r--r--   0        0        0    12340 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/files.py
+-rw-r--r--   0        0        0    19099 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/graph.py
+-rw-r--r--   0        0        0    11975 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/jobs.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/languages.py
+-rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/lsp.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/path_lookup.py
+-rw-r--r--   0        0        0    16503 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/pyspark.py
+-rw-r--r--   0        0        0     9467 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/python_libraries.py
+-rw-r--r--   0        0        0    12127 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/python_linter.py
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/queries.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/redash.py
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/spark_connect.py
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/table_creation.py
+-rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/whitelist.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/workflows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/notebooks/__init__.py
+-rw-r--r--   0        0        0    11671 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/notebooks/cells.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/notebooks/loaders.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/notebooks/migrator.py
+-rw-r--r--   0        0        0     6751 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/notebooks/sources.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/upgrades/v0.15.0_added_cluster_policy.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/upgrades/v0.16.0_changing_cluster_table_schema.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/upgrades/v0.20.0_add_is_partitioned_column.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/upgrades/v0.23.0_add_assessment_to_udf.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/upgrades/v0.4.0_added_log_dir.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/workspace_access/__init__.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/workspace_access/base.py
+-rw-r--r--   0        0        0     6002 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/workspace_access/clusters.py
+-rw-r--r--   0        0        0    18962 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/workspace_access/generic.py
+-rw-r--r--   0        0        0    34574 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/workspace_access/groups.py
+-rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/workspace_access/listing.py
+-rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/workspace_access/manager.py
+-rw-r--r--   0        0        0    12579 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/workspace_access/redash.py
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/workspace_access/scim.py
+-rw-r--r--   0        0        0     5966 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/workspace_access/secrets.py
+-rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/workspace_access/tacl.py
+-rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/databricks/labs/ucx/workspace_access/workflows.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/.gitignore
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/LICENSE
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/NOTICE
+-rw-r--r--   0        0        0    70518 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/README.md
+-rw-r--r--   0        0        0    28630 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/pyproject.toml
+-rw-r--r--   0        0        0    72196 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.24.0/PKG-INFO
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/cli.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from databricks.labs.blueprint.installation import Installation, SerdeError
 from databricks.labs.blueprint.tui import Prompts
 from databricks.sdk import AccountClient, WorkspaceClient
 from databricks.sdk.errors import NotFound
 
 from databricks.labs.ucx.config import WorkspaceConfig
 from databricks.labs.ucx.contexts.account_cli import AccountContext
-from databricks.labs.ucx.contexts.workspace_cli import WorkspaceContext
+from databricks.labs.ucx.contexts.workspace_cli import WorkspaceContext, LocalCheckoutContext
 from databricks.labs.ucx.hive_metastore.tables import What
 
 ucx = App(__file__)
 logger = get_logger(__file__)
 
 CANT_FIND_UCX_MSG = (
     "Couldn't find UCX configuration in the user's home folder. "
@@ -289,25 +289,27 @@
 
 
 @ucx.command
 def create_missing_principals(
     w: WorkspaceClient,
     prompts: Prompts,
     ctx: WorkspaceContext | None = None,
-    single_role: bool = True,
+    single_role: bool = False,
+    role_name="UC_ROLE",
+    policy_name="UC_POLICY",
     **named_parameters,
 ):
     """Not supported for Azure.
     For AWS, this command identifies all the S3 locations that are missing a UC compatible role and creates them.
-    By default, it will create a single role for all S3. Set the optional single_role parameter to False, to create one role per S3 location.
+    By default, it will create a  role per S3 location. Set the optional single_role parameter to True to create a single role for all S3 locations.
     """
     if not ctx:
         ctx = WorkspaceContext(w, named_parameters)
     if ctx.is_aws:
-        return ctx.iam_role_creation.run(prompts, single_role=single_role)
+        return ctx.iam_role_creation.run(prompts, single_role=single_role, role_name=role_name, policy_name=policy_name)
     raise ValueError("Unsupported cloud provider")
 
 
 @ucx.command
 def migrate_credentials(w: WorkspaceClient, prompts: Prompts, ctx: WorkspaceContext | None = None, **named_parameters):
     """For Azure, this command prompts to i) create UC storage credentials for the access connectors with a
     managed identity created for each storage account present in the ADLS Gen2 locations, the access connectors are
@@ -392,15 +394,15 @@
     )
     ctx.cluster_access.revert_cluster_remap(cluster_list, cluster_ids)
 
 
 @ucx.command
 def migrate_local_code(w: WorkspaceClient, prompts: Prompts):
     """Fix the code files based on their language."""
-    ctx = WorkspaceContext(w)
+    ctx = LocalCheckoutContext(w)
     working_directory = Path.cwd()
     if not prompts.confirm("Do you want to apply UC migration to all files in the current directory?"):
         return
     ctx.local_file_migrator.apply(working_directory)
 
 
 @ucx.command(is_account=True)
@@ -465,9 +467,19 @@
 @ucx.command
 def revert_dbsql_dashboards(w: WorkspaceClient, dashboard_id: str | None = None):
     """Revert migrated DBSQL Dashboard queries back to their original state"""
     ctx = WorkspaceContext(w)
     ctx.redash.revert_dashboards(dashboard_id)
 
 
+@ucx.command
+def lint_local_code(
+    w: WorkspaceClient, prompts: Prompts, path: str | None = None, ctx: LocalCheckoutContext | None = None
+):
+    """Lint local code files looking for problems."""
+    if ctx is None:
+        ctx = LocalCheckoutContext(w)
+    ctx.local_code_linter.lint(prompts, None if path is None else Path(path))
+
+
 if __name__ == "__main__":
     ucx()
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/config.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,14 +54,20 @@
 
     # Whether to trigger assessment job after installation
     trigger_job: bool = False
 
     # List of workspace ids ucx is installed on, only applied to account-level installation
     installed_workspace_ids: list[int] | None = None
 
+    # Threshold for row count comparison during data reconciliation, in percentage
+    recon_tolerance_percent: int = 5
+
+    # Whether to upload dependent libraries to the workspace
+    upload_dependencies: bool = False
+
     # [INTERNAL ONLY] Whether the assessment should capture only specific object permissions.
     include_object_permissions: list[str] | None = None
 
     def replace_inventory_variable(self, text: str) -> str:
         return text.replace("$inventory", f"hive_metastore.{self.inventory_database}")
 
     @classmethod
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/install.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/install.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 from databricks.labs.ucx.hive_metastore.tables import Table, TableError
 from databricks.labs.ucx.hive_metastore.udfs import Udf
 from databricks.labs.ucx.installer.hms_lineage import HiveMetastoreLineageEnabler
 from databricks.labs.ucx.installer.logs import LogRecord
 from databricks.labs.ucx.installer.mixins import InstallationMixin
 from databricks.labs.ucx.installer.policy import ClusterPolicyInstaller
 from databricks.labs.ucx.installer.workflows import WorkflowsDeployment
+from databricks.labs.ucx.recon.migration_recon import ReconResult
 from databricks.labs.ucx.runtime import Workflows
 from databricks.labs.ucx.source_code.jobs import JobProblem
 from databricks.labs.ucx.workspace_access.base import Permissions
 from databricks.labs.ucx.workspace_access.generic import WorkspaceObjectInfo
 from databricks.labs.ucx.workspace_access.groups import ConfigureGroups, MigratedGroup
 
 TAG_STEP = "step"
@@ -101,21 +102,23 @@
             functools.partial(table, "permissions", Permissions),
             functools.partial(table, "submit_runs", SubmitRunInfo),
             functools.partial(table, "policies", PolicyInfo),
             functools.partial(table, "migration_status", MigrationStatus),
             functools.partial(table, "workflow_problems", JobProblem),
             functools.partial(table, "udfs", Udf),
             functools.partial(table, "logs", LogRecord),
+            functools.partial(table, "recon_results", ReconResult),
         ],
     )
     deployer.deploy_view("objects", "queries/views/objects.sql")
     deployer.deploy_view("grant_detail", "queries/views/grant_detail.sql")
     deployer.deploy_view("table_estimates", "queries/views/table_estimates.sql")
     deployer.deploy_view("misc_patterns", "queries/views/misc_patterns.sql")
     deployer.deploy_view("code_patterns", "queries/views/code_patterns.sql")
+    deployer.deploy_view("reconciliation_results", "queries/views/reconciliation_results.sql")
 
 
 def extract_major_minor(version_string):
     match = re.search(r'(\d+\.\d+)', version_string)
     if match:
         return match.group(1)
     return None
@@ -209,27 +212,35 @@
             "Inventory Database stored in hive_metastore", default=default_database, valid_regex=r"^\w+$"
         )
         log_level = self.prompts.question("Log level", default="INFO").upper()
         num_threads = int(self.prompts.question("Number of threads", default="8", valid_number=True))
         configure_groups = ConfigureGroups(self.prompts)
         configure_groups.run()
         include_databases = self._select_databases()
+        upload_dependencies = self.prompts.confirm(
+            f"Does given workspace {self.workspace_client.get_workspace_id()} " f"block Internet access?"
+        )
         trigger_job = self.prompts.confirm("Do you want to trigger assessment job after installation?")
+        recon_tolerance_percent = int(
+            self.prompts.question("Reconciliation threshold, in percentage", default="5", valid_number=True)
+        )
         return WorkspaceConfig(
             inventory_database=inventory_database,
             workspace_group_regex=configure_groups.workspace_group_regex,
             workspace_group_replace=configure_groups.workspace_group_replace,
             account_group_regex=configure_groups.account_group_regex,
             group_match_by_external_id=configure_groups.group_match_by_external_id,  # type: ignore[arg-type]
             include_group_names=configure_groups.include_group_names,
             renamed_group_prefix=configure_groups.renamed_group_prefix,
             log_level=log_level,
             num_threads=num_threads,
             include_databases=include_databases,
             trigger_job=trigger_job,
+            recon_tolerance_percent=recon_tolerance_percent,
+            upload_dependencies=upload_dependencies,
         )
 
     def _compare_remote_local_versions(self):
         try:
             local_version = self.product_info.released_version()
             remote_version = self.installation.load(Version).version
             if extract_major_minor(remote_version) == extract_major_minor(local_version):
@@ -648,20 +659,95 @@
         for workspace in installed_workspaces:
             installer = self._get_installer(workspace)
             installer.replace_config(installed_workspace_ids=installed_workspace_ids)
 
         # upload the json dump of workspace info in the .ucx folder
         ctx.account_workspaces.sync_workspace_info(installed_workspaces)
 
+    def join_collection(
+        self,
+        current_workspace_id: int,
+    ):
+        if not self.is_account_install and self.prompts.confirm(
+            "Do you want to join the current installation to an existing collection?"
+        ):
+
+            installed_workspaces: list[Workspace] | None = []
+            accessible_workspaces: list[Workspace] = []
+            account_client = self._get_safe_account_client()
+            ctx = AccountContext(account_client)
+            try:
+                accessible_workspaces = ctx.account_workspaces.get_accessible_workspaces()
+            except PermissionDenied:
+                logger.warning("User doesnt have account admin permission, cant join a collection, skipping...")
+            collection_workspace = self._get_collection_workspace(accessible_workspaces, account_client)
+            if collection_workspace is not None:
+                installed_workspaces = self._sync_collection(collection_workspace, current_workspace_id, account_client)
+            if installed_workspaces is not None:
+                ctx.account_workspaces.sync_workspace_info(installed_workspaces)
+
+    def _sync_collection(
+        self,
+        collection_workspace: Workspace,
+        current_workspace_id: int,
+        account_client: AccountClient,
+    ) -> list[Workspace] | None:
+        installer = self._get_installer(collection_workspace)
+        installed_workspace_ids = installer.config.installed_workspace_ids
+        if installed_workspace_ids is None:
+            installed_workspace_ids = []
+            logger.warning(
+                f"Workspace {collection_workspace.deployment_name} does not belong to any existing "
+                f"collection, creating a new collection"
+            )
+        installed_workspace_ids.append(current_workspace_id)
+        installed_workspaces = []
+        for account_workspace in account_client.workspaces.list():
+            if account_workspace.workspace_id in installed_workspace_ids:
+                installed_workspaces.append(account_workspace)
+
+        for installed_workspace in installed_workspaces:
+            installer = self._get_installer(installed_workspace)
+            installer.replace_config(installed_workspace_ids=installed_workspace_ids)
+        return installed_workspaces
+
+    def _get_collection_workspace(
+        self,
+        accessible_workspaces: list[Workspace],
+        account_client: AccountClient,
+    ) -> Workspace | None:
+        installed_workspaces = []
+        for workspace in accessible_workspaces:
+            workspace_client = account_client.get_workspace_client(workspace)
+            workspace_installation = Installation.existing(workspace_client, self.product_info.product_name())
+            if len(workspace_installation) > 0:
+                installed_workspaces.append(workspace)
+
+        if len(installed_workspaces) == 0:
+            logger.warning("No existing installation found , setting up new installation without")
+            return None
+        workspaces = {
+            workspace.deployment_name: workspace
+            for workspace in installed_workspaces
+            if workspace.deployment_name is not None
+        }
+        workspace = self.prompts.choice_from_dict(
+            "Please select a workspace, the current installation of ucx will be grouped as a "
+            "collection with the selected workspace",
+            workspaces,
+        )
+        return workspace
+
 
 if __name__ == "__main__":
     logger = get_logger(__file__)
     if is_in_debug():
         logging.getLogger('databricks').setLevel(logging.DEBUG)
     env = dict(os.environ.items())
     force_install = env.get("UCX_FORCE_INSTALL")
+    account_installer = AccountInstaller(AccountClient(product="ucx", product_version=__version__))
     if force_install == "account":
-        account_installer = AccountInstaller(AccountClient(product="ucx", product_version=__version__))
         account_installer.install_on_account()
     else:
         workspace_installer = WorkspaceInstaller(WorkspaceClient(product="ucx", product_version=__version__))
         workspace_installer.run()
+        account_installer.join_collection(workspace_installer.workspace_client.get_workspace_id())
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/runtime.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/runtime.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 
 from databricks.labs.ucx.__about__ import __version__
 from databricks.labs.ucx.assessment.workflows import Assessment, Failing
 from databricks.labs.ucx.contexts.workflow_task import RuntimeContext
 from databricks.labs.ucx.framework.tasks import Task, Workflow, parse_args
 from databricks.labs.ucx.installer.logs import TaskLogger
 from databricks.labs.ucx.hive_metastore.workflows import (
-    MigrateTablesInMounts,
+    ScanTablesInMounts,
     TableMigration,
+    MigrateTablesInMounts,
     MigrateHiveSerdeTablesInPlace,
     MigrateExternalTablesCTAS,
 )
+from databricks.labs.ucx.recon.workflows import MigrationRecon
 from databricks.labs.ucx.source_code.workflows import ExperimentalWorkflowLinter
 from databricks.labs.ucx.workspace_access.workflows import (
     GroupMigration,
     PermissionsMigrationAPI,
     RemoveWorkspaceLocalGroups,
     ValidateGroupPermissions,
 )
@@ -45,17 +47,19 @@
                 Assessment(),
                 GroupMigration(),
                 TableMigration(),
                 MigrateHiveSerdeTablesInPlace(),
                 MigrateExternalTablesCTAS(),
                 ValidateGroupPermissions(),
                 RemoveWorkspaceLocalGroups(),
+                ScanTablesInMounts(),
                 MigrateTablesInMounts(),
                 PermissionsMigrationAPI(),
                 ExperimentalWorkflowLinter(),
+                MigrationRecon(),
                 Failing(),
             ]
         )
 
     def tasks(self) -> list[Task]:
         return self._tasks
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/account/aggregate.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/account/aggregate.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/account/metastores.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/account/metastores.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/account/workspaces.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/account/workspaces.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/aws.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/assessment/aws.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,32 +42,30 @@
     role_arn: str
     resource_type: str
     privilege: str
     resource_path: str
 
     @property
     def role_name(self):
-        role_match = re.match(AWSInstanceProfile.ROLE_NAME_REGEX, self.role_arn)
+        role_match = re.match(AWSResources.ROLE_NAME_REGEX, self.role_arn)
         return role_match.group(1)
 
 
 @dataclass
 class AWSInstanceProfile:
     instance_profile_arn: str
     iam_role_arn: str | None = None
 
-    ROLE_NAME_REGEX = r"arn:aws:iam::[0-9]+:(?:instance-profile|role)\/([a-zA-Z0-9+=,.@_-]*)$"
-
     @property
     def role_name(self) -> str | None:
         if self.iam_role_arn:
             arn = self.iam_role_arn
         else:
             arn = self.instance_profile_arn
-        role_match = re.match(self.ROLE_NAME_REGEX, arn)
+        role_match = re.match(AWSResources.ROLE_NAME_REGEX, arn)
         if not role_match:
             logger.error(f"Role ARN is mismatched {self.iam_role_arn}")
             return None
         return role_match.group(1)
 
 
 @lru_cache(maxsize=1024)
@@ -84,14 +82,15 @@
     S3_REGEX: typing.ClassVar[str] = r"arn:aws:s3:::([a-zA-Z0-9\/+=,.@_-]*)\/\*$"
     S3_PREFIX: typing.ClassVar[str] = "arn:aws:s3:::"
     S3_PATH_REGEX: typing.ClassVar[str] = r"((s3:\/\/)|(s3a:\/\/))(.*)"
     UC_MASTER_ROLES_ARN: typing.ClassVar[list[str]] = [
         "arn:aws:iam::414351767826:role/unity-catalog-prod-UCMasterRole-14S5ZJVKOTYTL",
         "arn:aws:iam::707343435239:role/unity-catalog-dev-UCMasterRole-G3MMN8SP21FO",
     ]
+    ROLE_NAME_REGEX = r"arn:aws:iam::[0-9]+:(?:instance-profile|role)\/([a-zA-Z0-9+=,.@_-]*)$"
 
     def __init__(self, profile: str, command_runner: Callable[[str], tuple[int, str, str]] = run_command):
         self._profile = profile
         self._command_runner = command_runner
 
     def validate_connection(self):
         validate_command = "sts get-caller-identity"
@@ -327,15 +326,20 @@
             f"iam update-assume-role-policy --role-name {role_name} --policy-document {policy_document_json}"
         )
         if not update_role:
             return None
         return update_role["Role"]["Arn"]
 
     def put_role_policy(
-        self, role_name: str, policy_name: str, s3_prefixes: set[str], account_id: str, kms_key=None
+        self,
+        role_name: str,
+        policy_name: str,
+        s3_prefixes: set[str],
+        account_id: str,
+        kms_key=None,
     ) -> bool:
         if not self._run_command(
             f"iam put-role-policy --role-name {role_name} --policy-name {policy_name} "
             f"--policy-document {self._aws_s3_policy(s3_prefixes, account_id, role_name, kms_key)}"
         ):
             return False
         return True
@@ -346,24 +350,37 @@
             "Statement": [
                 {"Effect": "Allow", "Principal": {"Service": "ec2.amazonaws.com"}, "Action": "sts:AssumeRole"}
             ],
         }
         assume_role_json = self._get_json_for_cli(aws_role_trust_doc)
         return self._create_role(role_name, assume_role_json)
 
-    def get_instance_profile(self, instance_profile_name: str) -> str | None:
+    def get_instance_profile_arn(self, instance_profile_name: str) -> str | None:
         instance_profile = self._run_json_command(
             f"iam get-instance-profile --instance-profile-name {instance_profile_name}"
         )
 
         if not instance_profile:
             return None
 
         return instance_profile["InstanceProfile"]["Arn"]
 
+    def get_instance_profile_role_arn(self, instance_profile_name: str) -> str | None:
+        instance_profile = self._run_json_command(
+            f"iam get-instance-profile --instance-profile-name {instance_profile_name}"
+        )
+
+        if not instance_profile:
+            return None
+
+        try:
+            return instance_profile["InstanceProfile"]["Roles"][0]["Arn"]
+        except (KeyError, IndexError):
+            return None
+
     def create_instance_profile(self, instance_profile_name: str) -> str | None:
         instance_profile = self._run_json_command(
             f"iam create-instance-profile --instance-profile-name {instance_profile_name}"
         )
 
         if not instance_profile:
             return None
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/azure.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/assessment/azure.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/clusters.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/assessment/clusters.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/crawlers.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/assessment/crawlers.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/init_scripts.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/assessment/init_scripts.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/jobs.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/assessment/jobs.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/pipelines.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/assessment/pipelines.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/secrets.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/assessment/secrets.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/workflows.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/assessment/workflows.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/aws/access.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/aws/access.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,22 +29,21 @@
 
     def __init__(
         self,
         installation: Installation,
         ws: WorkspaceClient,
         aws_resources: AWSResources,
         external_locations: ExternalLocations,
-        aws_account_id=None,
         kms_key=None,
     ):
         self._installation = installation
         self._aws_resources = aws_resources
         self._ws = ws
         self._locations = external_locations
-        self._aws_account_id = aws_account_id
+        self._aws_account_id = aws_resources.validate_connection().get("Account")
         self._kms_key = kms_key
 
     def list_uc_roles(self, *, single_role=True, role_name="UC_ROLE", policy_name="UC_POLICY"):
         """
         Get the missing paths
         Identify the S3 prefixes
         Create the roles and policies for the missing S3 prefixes
@@ -107,21 +106,20 @@
     def role_exists(self, role_name: str) -> bool:
         return self._aws_resources.role_exists(role_name)
 
     def _get_instance_profiles(self) -> Iterable[AWSInstanceProfile]:
         instance_profiles = self._ws.instance_profiles.list()
         result_instance_profiles = []
         for instance_profile in instance_profiles:
-            if not instance_profile.iam_role_arn:
-                instance_profile.iam_role_arn = instance_profile.instance_profile_arn.replace(
-                    "instance-profile", "role"
-                )
-            result_instance_profiles.append(
-                AWSInstanceProfile(instance_profile.instance_profile_arn, instance_profile.iam_role_arn)
-            )
+            iam_role_arn = instance_profile.iam_role_arn
+            role_match = re.match(AWSResources.ROLE_NAME_REGEX, instance_profile.instance_profile_arn)
+            if role_match is not None:
+                instance_profile_name = role_match.group(1)
+                iam_role_arn = self._aws_resources.get_instance_profile_role_arn(instance_profile_name)
+            result_instance_profiles.append(AWSInstanceProfile(instance_profile.instance_profile_arn, iam_role_arn))
 
         return result_instance_profiles
 
     def _get_instance_profiles_access(self):
         instance_profiles = list(self._get_instance_profiles())
         tasks = []
         for instance_profile in instance_profiles:
@@ -226,15 +224,15 @@
         self._ws.warehouses.set_workspace_warehouse_config(
             data_access_config=warehouse_config.data_access_config,
             sql_configuration_parameters=warehouse_config.sql_configuration_parameters,
             instance_profile_arn=iam_instance_profile.instance_profile_arn,
         )
 
     def get_instance_profile(self, instance_profile_name: str) -> AWSInstanceProfile | None:
-        instance_profile_arn = self._aws_resources.get_instance_profile(instance_profile_name)
+        instance_profile_arn = self._aws_resources.get_instance_profile_arn(instance_profile_name)
 
         if not instance_profile_arn:
             return None
 
         return AWSInstanceProfile(instance_profile_arn)
 
     def _create_uber_instance_profile(self, iam_role_name):
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/aws/credentials.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/aws/credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,18 +201,20 @@
         # print action plan to console for customer to review.
         for iam in iam_list:
             logger.info(f"Role:{iam.role_name} Policy:{iam.policy_name} Paths:{iam.resource_paths}")
 
     def save(self, migration_results: list[CredentialValidationResult]) -> str:
         return self._installation.save(migration_results, filename=self._output_file)
 
-    def run(self, prompts: Prompts, *, single_role=True, role_name="UC_ROLE", policy_name="UC_POLICY"):
+    def run(self, prompts: Prompts, *, single_role=False, role_name="UC_ROLE", policy_name="UC_POLICY"):
 
         iam_list = self._resource_permissions.list_uc_roles(
-            single_role=single_role, role_name=role_name, policy_name=policy_name
+            single_role=single_role,
+            role_name=role_name,
+            policy_name=policy_name,
         )
         if not iam_list:
             logger.info("No IAM Role created")
             return
         self._print_action_plan(iam_list)
         plan_confirmed = prompts.confirm(
             "Above UC Compatible IAM roles will be created and granted access to the corresponding paths, "
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/aws/locations.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/aws/locations.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/azure/access.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/azure/access.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/azure/credentials.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/azure/credentials.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/azure/locations.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/azure/locations.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/azure/resources.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/azure/resources.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/contexts/account_cli.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/contexts/account_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from functools import cached_property
+from os import environ
 
 from databricks.sdk import AccountClient
 
 
 from databricks.labs.ucx.account.aggregate import AccountAggregate
 from databricks.labs.ucx.account.metastores import AccountMetastores
 from databricks.labs.ucx.account.workspaces import AccountWorkspaces
@@ -27,9 +28,13 @@
         return AccountWorkspaces(self.account_client, self.workspace_ids)
 
     @cached_property
     def account_aggregate(self):
         return AccountAggregate(self.account_workspaces)
 
     @cached_property
+    def is_account_install(self):
+        return environ.get("UCX_FORCE_INSTALL") == "account"
+
+    @cached_property
     def account_metastores(self):
         return AccountMetastores(self.account_client)
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/contexts/application.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/contexts/application.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,23 @@
 from pathlib import Path
 
 from databricks.labs.blueprint.installation import Installation
 from databricks.labs.blueprint.installer import InstallState
 from databricks.labs.blueprint.tui import Prompts
 from databricks.labs.blueprint.wheels import ProductInfo, WheelsV2
 from databricks.labs.lsql.backends import SqlBackend
+
+from databricks.labs.ucx.recon.data_comparator import StandardDataComparator
+from databricks.labs.ucx.recon.data_profiler import StandardDataProfiler
+from databricks.labs.ucx.recon.metadata_retriever import DatabricksTableMetadataRetriever
+from databricks.labs.ucx.recon.migration_recon import MigrationRecon
+from databricks.labs.ucx.recon.schema_comparator import StandardSchemaComparator
+from databricks.labs.ucx.source_code.python_libraries import PipResolver
 from databricks.sdk import AccountClient, WorkspaceClient, core
+from databricks.sdk.errors import ResourceDoesNotExist
 from databricks.sdk.service import sql
 
 from databricks.labs.ucx.account.workspaces import WorkspaceInfo
 from databricks.labs.ucx.assessment.azure import AzureServicePrincipalCrawler
 from databricks.labs.ucx.aws.credentials import CredentialManager
 from databricks.labs.ucx.config import WorkspaceConfig
 from databricks.labs.ucx.hive_metastore import ExternalLocations, Mounts, TablesCrawler
@@ -35,29 +43,28 @@
 from databricks.labs.ucx.hive_metastore.verification import VerifyHasMetastore
 from databricks.labs.ucx.installer.workflows import DeployedWorkflows
 from databricks.labs.ucx.source_code.jobs import WorkflowLinter
 from databricks.labs.ucx.source_code.notebooks.loaders import (
     NotebookResolver,
     NotebookLoader,
 )
-from databricks.labs.ucx.source_code.files import FileLoader, LocalFileResolver
+from databricks.labs.ucx.source_code.files import FileLoader, FolderLoader, ImportFileResolver
 from databricks.labs.ucx.source_code.path_lookup import PathLookup
 from databricks.labs.ucx.source_code.graph import DependencyResolver
-from databricks.labs.ucx.source_code.whitelist import WhitelistResolver, Whitelist
-from databricks.labs.ucx.source_code.site_packages import SitePackageResolver, SitePackages
+from databricks.labs.ucx.source_code.whitelist import Whitelist
 from databricks.labs.ucx.source_code.languages import Languages
 from databricks.labs.ucx.source_code.redash import Redash
 from databricks.labs.ucx.workspace_access import generic, redash
 from databricks.labs.ucx.workspace_access.groups import GroupManager
 from databricks.labs.ucx.workspace_access.manager import PermissionManager
 from databricks.labs.ucx.workspace_access.scim import ScimSupport
 from databricks.labs.ucx.workspace_access.secrets import SecretScopesSupport
 from databricks.labs.ucx.workspace_access.tacl import TableAclSupport
 
-# "Service Factories" would always have a lot of pulic methods.
+# "Service Factories" would always have a lot of public methods.
 # This is because they are responsible for creating objects that are
 # used throughout the application. That being said, we'll do best
 # effort of splitting the instances between Global, Runtime,
 # Workspace CLI, and Account CLI contexts.
 # pylint: disable=too-many-public-methods
 
 logger = logging.getLogger(__name__)
@@ -276,20 +283,23 @@
             self.sql_backend,
             self.installation,
         )
 
     @cached_property
     def principal_locations(self):
         eligible_locations = {}
-        if self.is_azure:
-            eligible_locations = self.azure_acl.get_eligible_locations_principals()
-        if self.is_aws:
-            eligible_locations = self.aws_acl.get_eligible_locations_principals()
-        if self.is_gcp:
-            raise NotImplementedError("Not implemented for GCP.")
+        try:
+            if self.is_azure:
+                eligible_locations = self.azure_acl.get_eligible_locations_principals()
+            if self.is_aws:
+                eligible_locations = self.aws_acl.get_eligible_locations_principals()
+            if self.is_gcp:
+                raise NotImplementedError("Not implemented for GCP.")
+        except ResourceDoesNotExist:
+            pass
         return eligible_locations
 
     @cached_property
     def principal_acl(self):
         return PrincipalACL(
             self.workspace_client,
             self.sql_backend,
@@ -347,57 +357,56 @@
         return WorkspaceInfo(self.installation, self.workspace_client)
 
     @cached_property
     def verify_has_metastore(self):
         return VerifyHasMetastore(self.workspace_client)
 
     @cached_property
+    def pip_resolver(self):
+        return PipResolver(self.file_loader, self.whitelist)
+
+    @cached_property
     def notebook_loader(self) -> NotebookLoader:
         return NotebookLoader()
 
     @cached_property
     def notebook_resolver(self):
         return NotebookResolver(self.notebook_loader)
 
     @cached_property
-    def site_packages(self):
-        # TODO: actually load the site packages
-        return SitePackages([])
+    def site_packages_path(self):
+        lookup = self.path_lookup
+        return next(path for path in lookup.paths if "site-packages" in path.as_posix())
 
     @cached_property
     def path_lookup(self):
         # TODO find a solution to enable a different cwd per job/task (maybe it's not necessary or possible?)
         return PathLookup.from_sys_path(Path.cwd())
 
     @cached_property
     def file_loader(self):
         return FileLoader()
 
     @cached_property
-    def site_packages_resolver(self):
-        return SitePackageResolver(self.site_packages, self.file_loader, self.path_lookup)
+    def folder_loader(self):
+        return FolderLoader(self.file_loader)
 
     @cached_property
     def whitelist(self):
         # TODO: fill in the whitelist
         return Whitelist()
 
     @cached_property
-    def whitelist_resolver(self):
-        return WhitelistResolver(self.whitelist)
-
-    @cached_property
     def file_resolver(self):
-        return LocalFileResolver(self.file_loader)
+        return ImportFileResolver(self.file_loader, self.whitelist)
 
     @cached_property
     def dependency_resolver(self):
-        # TODO: link back self.site_packages_resolver
-        resolvers = [self.notebook_resolver, self.file_resolver, self.whitelist_resolver]
-        return DependencyResolver(resolvers, self.path_lookup)
+        library_resolvers = [self.pip_resolver]
+        return DependencyResolver(library_resolvers, self.notebook_resolver, self.file_resolver, self.path_lookup)
 
     @cached_property
     def workflow_linter(self):
         return WorkflowLinter(
             self.workspace_client,
             self.dependency_resolver,
             self.path_lookup,
@@ -408,12 +417,40 @@
     def redash(self):
         return Redash(
             self.migration_status_refresher.index(),
             self.workspace_client,
             self.installation,
         )
 
+    @cached_property
+    def metadata_retriever(self):
+        return DatabricksTableMetadataRetriever(self.sql_backend)
+
+    @cached_property
+    def schema_comparator(self):
+        return StandardSchemaComparator(self.metadata_retriever)
+
+    @cached_property
+    def data_profiler(self):
+        return StandardDataProfiler(self.sql_backend, self.metadata_retriever)
+
+    @cached_property
+    def data_comparator(self):
+        return StandardDataComparator(self.sql_backend, self.data_profiler)
+
+    @cached_property
+    def migration_recon(self):
+        return MigrationRecon(
+            self.sql_backend,
+            self.inventory_database,
+            self.migration_status_refresher,
+            self.table_mapping,
+            self.schema_comparator,
+            self.data_comparator,
+            self.config.recon_tolerance_percent,
+        )
+
 
 class CliContext(GlobalContext, abc.ABC):
     @cached_property
     def prompts(self) -> Prompts:
         return Prompts()
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/contexts/workflow_task.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/contexts/workflow_task.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/contexts/workspace_cli.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/contexts/workspace_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 
 from databricks.labs.lsql.backends import SqlBackend, StatementExecutionBackend
 from databricks.sdk import WorkspaceClient
 
 from databricks.labs.ucx.assessment.aws import run_command, AWSResources
 from databricks.labs.ucx.aws.access import AWSResourcePermissions
 from databricks.labs.ucx.aws.credentials import IamRoleMigration, IamRoleCreation
+from databricks.labs.ucx.aws.locations import AWSExternalLocationsMigration
 from databricks.labs.ucx.azure.access import AzureResourcePermissions
 from databricks.labs.ucx.azure.credentials import StorageCredentialManager, ServicePrincipalMigration
 from databricks.labs.ucx.azure.locations import ExternalLocationsMigration
-from databricks.labs.ucx.aws.locations import AWSExternalLocationsMigration
 from databricks.labs.ucx.azure.resources import AzureAPIClient, AzureResources
 from databricks.labs.ucx.contexts.application import CliContext
-from databricks.labs.ucx.source_code.files import LocalFileMigrator
+from databricks.labs.ucx.source_code.files import LocalFileMigrator, LocalCodeLinter
+from databricks.labs.ucx.source_code.notebooks.loaders import NotebookLoader
 from databricks.labs.ucx.workspace_access.clusters import ClusterAccess
 
 
 class WorkspaceContext(CliContext):
     def __init__(self, ws: WorkspaceClient, named_parameters: dict[str, str] | None = None):
         super().__init__(named_parameters)
         self._ws = ws
@@ -28,18 +29,14 @@
         return self._ws
 
     @cached_property
     def sql_backend(self) -> SqlBackend:
         return StatementExecutionBackend(self.workspace_client, self.config.warehouse_id)
 
     @cached_property
-    def local_file_migrator(self):
-        return LocalFileMigrator(self.languages)
-
-    @cached_property
     def cluster_access(self):
         return ClusterAccess(self.installation, self.workspace_client, self.prompts)
 
     @cached_property
     def azure_cli_authenticated(self):
         if not self.is_azure:
             raise NotImplementedError("Azure only")
@@ -147,15 +144,14 @@
     @cached_property
     def aws_resource_permissions(self):
         return AWSResourcePermissions(
             self.installation,
             self.workspace_client,
             self.aws_resources,
             self.external_locations,
-            self.named_parameters.get("aws_account_id"),
             self.named_parameters.get("kms_key"),
         )
 
     @cached_property
     def iam_role_migration(self):
         return IamRoleMigration(
             self.installation,
@@ -166,7 +162,26 @@
     @cached_property
     def iam_role_creation(self):
         return IamRoleCreation(
             self.installation,
             self.workspace_client,
             self.aws_resource_permissions,
         )
+
+    @cached_property
+    def notebook_loader(self) -> NotebookLoader:
+        return NotebookLoader()
+
+
+class LocalCheckoutContext(WorkspaceContext):
+    """Local context extends Workspace context to provide extra properties
+    for running local operations."""
+
+    @cached_property
+    def local_file_migrator(self):
+        return LocalFileMigrator(self.languages)
+
+    @cached_property
+    def local_code_linter(self):
+        return LocalCodeLinter(
+            self.file_loader, self.folder_loader, self.path_lookup, self.dependency_resolver, lambda: self.languages
+        )
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/framework/crawlers.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/framework/crawlers.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/framework/dashboards.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/framework/dashboards.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/framework/tasks.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/framework/tasks.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/framework/utils.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/framework/utils.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/catalog_schema.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/catalog_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import collections
 import logging
 from dataclasses import replace
+import fnmatch
 from pathlib import PurePath
 
 from databricks.labs.blueprint.tui import Prompts
 from databricks.labs.lsql.backends import SqlBackend
 from databricks.labs.ucx.hive_metastore.grants import PrincipalACL, Grant
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors import NotFound
@@ -133,22 +134,22 @@
                 target_schemas[catalog] = target_schemas[catalog] - schemas
         return target_catalogs, target_schemas
 
     def _validate_location(self, location: str):
         if location == "metastore":
             return True
         try:
-            location_path = PurePath(location)
+            PurePath(location)
         except ValueError:
             logger.error(f"Invalid location path {location}")
             return False
         for external_location in self._external_locations:
             if location == external_location.url:
                 return True
-            if location_path.match(f"{external_location.url}/*"):
+            if external_location.url is not None and fnmatch.fnmatch(location, external_location.url + '*'):
                 return True
         return False
 
     def _create_catalog(self, catalog, catalog_storage):
         logger.info(f"Creating UC catalog: {catalog}")
         if catalog_storage == "metastore":
             self._ws.catalogs.create(catalog, comment="Created by UCX")
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/grants.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/grants.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/locations.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/locations.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,32 +133,38 @@
 
     def _try_fetch(self) -> Iterable[ExternalLocation]:
         for row in self._fetch(
             f"SELECT * FROM {escape_sql_identifier(self._schema)}.{escape_sql_identifier(self._table)}"
         ):
             yield ExternalLocation(*row)
 
-    def _get_ext_location_definitions(self, missing_locations: list[ExternalLocation]) -> list:
+    @staticmethod
+    def _get_ext_location_definitions(missing_locations: list[ExternalLocation]) -> list:
         tf_script = []
         cnt = 1
+        res_name = ""
+        supported_prefixes = ("s3://", "s3a://", "s3n://", "gcs://", "abfss://")
         for loc in missing_locations:
-            if loc.location.startswith("s3://"):
-                res_name = loc.location[5:].rstrip("/").replace("/", "_")
-            elif loc.location.startswith("gcs://"):
-                res_name = loc.location[6:].rstrip("/").replace("/", "_")
-            elif loc.location.startswith("abfss://"):
-                container_name = loc.location[8 : loc.location.index("@")]
-                res_name = (
-                    loc.location[loc.location.index("@") + 1 :]
-                    .replace(".dfs.core.windows.net", "")
-                    .rstrip("/")
-                    .replace("/", "_")
-                )
-                res_name = f"{container_name}_{res_name}"
-            else:
+            for prefix in supported_prefixes:
+                prefix_len = len(prefix)
+                if not loc.location.startswith(prefix):
+                    continue
+                if prefix == "abfss://":
+                    container_sep_loc = loc.location.index("@")
+                    container_name = loc.location[prefix_len:container_sep_loc]
+                    res_name = (
+                        loc.location[container_sep_loc + 1 :]
+                        .replace(".dfs.core.windows.net", "")
+                        .rstrip("/")
+                        .replace("/", "_")
+                    )
+                    res_name = f"{container_name}_{res_name}"
+                else:
+                    res_name = loc.location[prefix_len:].rstrip("/").replace("/", "_")
+            if res_name == "":
                 # if the cloud storage url doesn't match the above condition or incorrect (example wasb://)
                 # dont generate tf script and ignore
                 logger.warning(f"unsupported storage format {loc.location}")
                 continue
             script = f'resource "databricks_external_location" "{res_name}" {{ \n'
             script += f'    name = "{res_name}"\n'
             script += f'    url  = "{loc.location.rstrip("/")}"\n'
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/mapping.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/mapping.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,49 +11,57 @@
 from databricks.sdk.errors import BadRequest, NotFound, ResourceConflict, DatabricksError
 from databricks.sdk.service.catalog import TableInfo, SchemaInfo
 
 from databricks.labs.ucx.account.workspaces import WorkspaceInfo
 from databricks.labs.ucx.framework.utils import escape_sql_identifier
 from databricks.labs.ucx.hive_metastore import TablesCrawler
 from databricks.labs.ucx.hive_metastore.tables import Table
+from databricks.labs.ucx.recon.base import TableIdentifier
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class Rule:
     workspace_name: str
     catalog_name: str
     src_schema: str
     dst_schema: str
     src_table: str
     dst_table: str
+    recon_tolerance_percent: int = 0  # threshold for row count comparison
+    compare_rows: bool = False  # whether to compare row by row
 
     @classmethod
-    def initial(cls, workspace_name: str, catalog_name: str, table: Table) -> "Rule":
+    def initial(cls, workspace_name: str, catalog_name: str, table: Table, recon_tolerance_percent: int) -> "Rule":
         return cls(
             workspace_name=workspace_name,
             catalog_name=catalog_name,
             src_schema=table.database,
             dst_schema=table.database,
             src_table=table.name,
             dst_table=table.name,
+            recon_tolerance_percent=recon_tolerance_percent,
         )
 
     @classmethod
     def from_src_dst(cls, src_table: TableInfo, dst_schema: SchemaInfo) -> "Rule":
         return cls(
             workspace_name="workspace",
             catalog_name=str(dst_schema.catalog_name or ""),
             src_schema=str(src_table.schema_name or ""),
             dst_schema=str(dst_schema.name or ""),
             src_table=str(src_table.name or ""),
             dst_table=str(src_table.name or ""),
+            recon_tolerance_percent=0,
         )
 
+    def match(self, table: TableIdentifier) -> bool:
+        return table.catalog == "hive_metastore" and self.src_schema == table.schema and self.src_table == table.table
+
     @property
     def as_uc_table_key(self):
         return f"{self.catalog_name}.{self.dst_schema}.{self.dst_table}"
 
     @property
     def as_hms_table_key(self):
         return f"hive_metastore.{self.src_schema}.{self.src_table}"
@@ -71,26 +79,33 @@
         return isinstance(other, TableToMigrate) and self.src == other.src
 
 
 class TableMapping:
     FILENAME = 'mapping.csv'
     UCX_SKIP_PROPERTY = "databricks.labs.ucx.skip"
 
-    def __init__(self, installation: Installation, ws: WorkspaceClient, sql_backend: SqlBackend):
+    def __init__(
+        self,
+        installation: Installation,
+        ws: WorkspaceClient,
+        sql_backend: SqlBackend,
+        recon_tolerance_percent: int = 0,
+    ):
         self._installation = installation
         self._ws = ws
         self._sql_backend = sql_backend
+        self._recon_tolerance_percent = recon_tolerance_percent
 
     def current_tables(self, tables: TablesCrawler, workspace_name: str, catalog_name: str):
         tables_snapshot = tables.snapshot()
         if len(tables_snapshot) == 0:
             msg = "No tables found. Please run: databricks labs ucx ensure-assessment-run"
             raise ValueError(msg)
         for table in tables_snapshot:
-            yield Rule.initial(workspace_name, catalog_name, table)
+            yield Rule.initial(workspace_name, catalog_name, table, self._recon_tolerance_percent)
 
     def save(self, tables: TablesCrawler, workspace_info: WorkspaceInfo) -> str:
         workspace_name = workspace_info.current()
         default_catalog_name = re.sub(r"\W+", "_", workspace_name)
         current_tables = self.current_tables(tables, workspace_name, default_catalog_name)
         return self._installation.save(list(current_tables), filename=self.FILENAME)
 
@@ -154,14 +169,16 @@
     def _get_databases_in_scope(self, databases: set[str]):
         tasks = []
         for database in databases:
             tasks.append(partial(self._get_database_in_scope_task, database))
         return Threads.strict("checking databases for skip property", tasks)
 
     def _get_database_in_scope_task(self, database: str) -> str | None:
+        if database.startswith("mounted_"):
+            return database
         describe = {}
         try:
             for value in self._sql_backend.fetch(f"DESCRIBE SCHEMA EXTENDED {escape_sql_identifier(database)}"):
                 describe[value["database_description_item"]] = value["database_description_value"]
         except NotFound:
             logger.warning(
                 f"Schema hive_metastore.{database} no longer exists. Skipping its properties check and migration."
@@ -178,22 +195,19 @@
     def _get_table_in_scope_task(self, table_to_migrate: TableToMigrate) -> TableToMigrate | None:
         table = table_to_migrate.src
         rule = table_to_migrate.rule
 
         if self.exists_in_uc(table, rule.as_uc_table_key):
             logger.info(f"The intended target for {table.key}, {rule.as_uc_table_key}, already exists.")
             return None
-        try:
-            result = self._sql_backend.fetch(
-                f"SHOW TBLPROPERTIES {escape_sql_identifier(table.database)}.{escape_sql_identifier(table.name)}"
-            )
-        except DatabricksError as err:
-            logger.warning(f"Failed to get properties for Table {table.key}: {err}")
+        properties = self._get_table_properties(table)
+        if not properties:
             return None
-        for value in result:
+
+        for value in properties:
             if value["key"] == self.UCX_SKIP_PROPERTY:
                 logger.info(f"{table.key} is marked to be skipped")
                 return None
             if value["key"] == "upgraded_to":
                 logger.info(f"{table.key} is set as upgraded to {value['value']}")
                 if self.exists_in_uc(table, value["value"]):
                     logger.info(
@@ -206,24 +220,49 @@
                 try:
                     self._sql_backend.execute(table.sql_unset_upgraded_to())
                 except DatabricksError as err:
                     logger.warning(f"Failed to unset upgraded_to property for Table {table.key}: {err}")
 
         return table_to_migrate
 
+    def _get_table_properties(self, table: Table):
+        table_identifier = f"{escape_sql_identifier(table.database)}.{escape_sql_identifier(table.name)}"
+        if table.is_table_in_mount:
+            table_identifier = f"delta.`{table.location}`"
+
+        try:
+            return self._sql_backend.fetch(f"SHOW TBLPROPERTIES {table_identifier}")
+        except DatabricksError as err:
+            logger.warning(f"Failed to get properties for Table {table.key}: {err}")
+            return None
+
     def exists_in_uc(self, src_table: Table, target_key: str):
         # Attempts to get the target table info from UC returns True if it exists.
-        try:
-            table_info = self._ws.tables.get(target_key)
-            if not table_info.properties:
-                return True
-            upgraded_from = table_info.properties.get("upgraded_from")
-            if upgraded_from and upgraded_from != src_table.key:
-                raise ResourceConflict(
-                    f"Expected to be migrated from {src_table.key}, but got {upgraded_from}. "
-                    "You can skip this error using the CLI command: "
-                    "databricks labs ucx skip "
-                    f"--schema {src_table.database} --table {src_table.name}"
-                )
+        table_info = self._try_get_table_in_uc(target_key)
+        if not table_info:
+            return False
+        # Corner case for tables in mounts where the table exists in UC, but the location is not the same
+        # from the one provided in the mapping
+        if src_table.is_table_in_mount and table_info.storage_location != src_table.location:
+            raise ResourceConflict(
+                f"Expected to be migrated from {src_table.key}, but got {table_info.storage_location}. "
+                "You can skip this error using the CLI command: "
+                "databricks labs ucx skip "
+                f"--schema {src_table.database} --table {src_table.name}"
+            )
+        if not table_info.properties:
             return True
+        upgraded_from = table_info.properties.get("upgraded_from")
+        if upgraded_from and upgraded_from != src_table.key and not src_table.is_table_in_mount:
+            raise ResourceConflict(
+                f"Expected to be migrated from {src_table.key}, but got {upgraded_from}. "
+                "You can skip this error using the CLI command: "
+                "databricks labs ucx skip "
+                f"--schema {src_table.database} --table {src_table.name}"
+            )
+        return True
+
+    def _try_get_table_in_uc(self, target_key: str):
+        try:
+            return self._ws.tables.get(target_key)
         except NotFound:
-            return False
+            return None
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/migration_status.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/migration_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 import logging
 from dataclasses import dataclass, replace
-from collections.abc import Iterable
+from collections.abc import Iterable, KeysView
 
 from databricks.labs.lsql.backends import SqlBackend
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors import NotFound
 
 from databricks.labs.ucx.framework.crawlers import CrawlerBase
 from databricks.labs.ucx.framework.utils import escape_sql_identifier
@@ -49,14 +49,17 @@
     def get(self, schema: str, table: str) -> MigrationStatus | None:
         """Get the migration status for a table. If the table is not migrated, return None."""
         dst = self._index.get((schema.lower(), table.lower()))
         if not dst or not dst.dst_table:
             return None
         return dst
 
+    def snapshot(self) -> KeysView[tuple[str, str]]:
+        return self._index.keys()
+
 
 class MigrationStatusRefresher(CrawlerBase[MigrationStatus]):
     def __init__(self, ws: WorkspaceClient, sbe: SqlBackend, schema, table_crawler: TablesCrawler):
         super().__init__(sbe, "hive_metastore", schema, "migration_status", MigrationStatus)
         self._ws = ws
         self._table_crawler = table_crawler
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/table_migrate.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/table_migrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 from collections import defaultdict
 from collections.abc import Iterable
 from functools import partial
 
 from databricks.labs.blueprint.parallel import Threads
 from databricks.labs.lsql.backends import SqlBackend
+from databricks.labs.ucx.framework.utils import escape_sql_identifier
 from databricks.sdk import WorkspaceClient
 
 from databricks.labs.ucx.hive_metastore import TablesCrawler, Mounts
 from databricks.labs.ucx.hive_metastore.grants import Grant, GrantsCrawler, PrincipalACL
 from databricks.labs.ucx.hive_metastore.locations import Mount, ExternalLocations
 from databricks.labs.ucx.hive_metastore.mapping import (
     Rule,
@@ -164,14 +165,16 @@
             return True
         if src_table.src.what == What.DBFS_ROOT_DELTA:
             return self._migrate_dbfs_root_table(src_table.src, src_table.rule, grants)
         if src_table.src.what == What.DBFS_ROOT_NON_DELTA:
             return self._migrate_table_create_ctas(src_table.src, src_table.rule, grants, mounts)
         if src_table.src.what == What.EXTERNAL_SYNC:
             return self._migrate_external_table(src_table.src, src_table.rule, grants)
+        if src_table.src.what == What.TABLE_IN_MOUNT:
+            return self._migrate_table_in_mount(src_table.src, src_table.rule, grants)
         if src_table.src.what == What.EXTERNAL_HIVESERDE:
             # This hiveserde_in_place_migrate is used to determine if current hiveserde migration should use in-place migration or CTAS.
             # We will provide two workflows for hiveserde table migration:
             # 1. One will migrate all hiveserde tables using CTAS which we officially support.
             # 2. The other one will migrate certain types of hiveserde in place, which is technically working, but the user
             # need to accept the risk that the old files created by hiveserde may not be processed correctly by Spark
             # datasource in corner cases.
@@ -208,17 +211,17 @@
         return True
 
     def _migrate_view_table(self, src_view: ViewToMigrate, grants: list[Grant] | None = None):
         view_migrate_sql = self._sql_migrate_view(src_view)
         logger.debug(f"Migrating view {src_view.src.key} to using SQL query: {view_migrate_sql}")
         try:
             self._backend.execute(view_migrate_sql)
-            self._backend.execute(src_view.src.sql_alter_to(src_view.rule.as_uc_table_key))
+            self._backend.execute(self._sql_alter_to(src_view.src, src_view.rule.as_uc_table_key))
             self._backend.execute(
-                src_view.src.sql_alter_from(src_view.rule.as_uc_table_key, self._ws.get_workspace_id())
+                self._sql_alter_from(src_view.src, src_view.rule.as_uc_table_key, self._ws.get_workspace_id())
             )
         except DatabricksError as e:
             logger.warning(f"Failed to migrate view {src_view.src.key} to {src_view.rule.as_uc_table_key}: {e}")
             return False
         return self._migrate_acl(src_view.src, src_view.rule, grants)
 
     def _sql_migrate_view(self, src_view: ViewToMigrate) -> str:
@@ -237,15 +240,15 @@
         sync_result = next(iter(self._backend.fetch(table_migrate_sql)))
         if sync_result.status_code != "SUCCESS":
             logger.warning(
                 f"SYNC command failed to migrate table {src_table.key} to {target_table_key}. "
                 f"Status code: {sync_result.status_code}. Description: {sync_result.description}"
             )
             return False
-        self._backend.execute(src_table.sql_alter_from(rule.as_uc_table_key, self._ws.get_workspace_id()))
+        self._backend.execute(self._sql_alter_from(src_table, rule.as_uc_table_key, self._ws.get_workspace_id()))
         return self._migrate_acl(src_table, rule, grants)
 
     def _migrate_external_table_hiveserde_in_place(
         self,
         src_table: Table,
         rule: Rule,
         grants: list[Grant],
@@ -276,31 +279,31 @@
             return False
 
         logger.debug(
             f"Migrating external table {src_table.key} to {rule.as_uc_table_key} using SQL query: {table_migrate_sql}"
         )
         try:
             self._backend.execute(table_migrate_sql)
-            self._backend.execute(src_table.sql_alter_to(rule.as_uc_table_key))
-            self._backend.execute(src_table.sql_alter_from(rule.as_uc_table_key, self._ws.get_workspace_id()))
+            self._backend.execute(self._sql_alter_to(src_table, rule.as_uc_table_key))
+            self._backend.execute(self._sql_alter_from(src_table, rule.as_uc_table_key, self._ws.get_workspace_id()))
         except DatabricksError as e:
             logger.warning(f"Failed to migrate table {src_table.key} to {rule.as_uc_table_key}: {e}")
             return False
         return self._migrate_acl(src_table, rule, grants)
 
     def _migrate_dbfs_root_table(self, src_table: Table, rule: Rule, grants: list[Grant] | None = None):
         target_table_key = rule.as_uc_table_key
         table_migrate_sql = src_table.sql_migrate_dbfs(target_table_key)
         logger.debug(
             f"Migrating managed table {src_table.key} to {rule.as_uc_table_key} using SQL query: {table_migrate_sql}"
         )
         try:
             self._backend.execute(table_migrate_sql)
-            self._backend.execute(src_table.sql_alter_to(rule.as_uc_table_key))
-            self._backend.execute(src_table.sql_alter_from(rule.as_uc_table_key, self._ws.get_workspace_id()))
+            self._backend.execute(self._sql_alter_to(src_table, rule.as_uc_table_key))
+            self._backend.execute(self._sql_alter_from(src_table, rule.as_uc_table_key, self._ws.get_workspace_id()))
         except DatabricksError as e:
             logger.warning(f"Failed to migrate table {src_table.key} to {rule.as_uc_table_key}: {e}")
             return False
         return self._migrate_acl(src_table, rule, grants)
 
     def _migrate_table_create_ctas(self, src_table: Table, rule: Rule, grants: list[Grant], mounts: list[Mount]):
         if src_table.what not in [What.EXTERNAL_NO_SYNC, What.EXTERNAL_HIVESERDE]:
@@ -312,16 +315,31 @@
             dst_table_location = src_table.location + "_ctas_migrated"
             if mounts and src_table.is_dbfs_mnt:
                 dst_table_location = ExternalLocations.resolve_mount(src_table.location, mounts) + "_ctas_migrated"
             table_migrate_sql = src_table.sql_migrate_ctas_external(rule.as_uc_table_key, dst_table_location)
         logger.debug(f"Migrating table {src_table.key} to {rule.as_uc_table_key} using SQL query: {table_migrate_sql}")
         try:
             self._backend.execute(table_migrate_sql)
-            self._backend.execute(src_table.sql_alter_to(rule.as_uc_table_key))
-            self._backend.execute(src_table.sql_alter_from(rule.as_uc_table_key, self._ws.get_workspace_id()))
+            self._backend.execute(self._sql_alter_to(src_table, rule.as_uc_table_key))
+            self._backend.execute(self._sql_alter_from(src_table, rule.as_uc_table_key, self._ws.get_workspace_id()))
+        except DatabricksError as e:
+            logger.warning(f"Failed to migrate table {src_table.key} to {rule.as_uc_table_key}: {e}")
+            return False
+        return self._migrate_acl(src_table, rule, grants)
+
+    def _migrate_table_in_mount(self, src_table: Table, rule: Rule, grants: list[Grant] | None = None):
+        target_table_key = rule.as_uc_table_key
+        try:
+            table_schema = self._backend.fetch(f"DESCRIBE TABLE delta.`{src_table.location}`;")
+            table_migrate_sql = src_table.sql_migrate_table_in_mount(target_table_key, table_schema)
+            logger.info(
+                f"Migrating table in mount {src_table.location} to UC table {rule.as_uc_table_key} using SQL query: {table_migrate_sql}"
+            )
+            self._backend.execute(table_migrate_sql)
+            self._backend.execute(self._sql_alter_from(src_table, rule.as_uc_table_key, self._ws.get_workspace_id()))
         except DatabricksError as e:
             logger.warning(f"Failed to migrate table {src_table.key} to {rule.as_uc_table_key}: {e}")
             return False
         return self._migrate_acl(src_table, rule, grants)
 
     def _migrate_acl(self, src: Table, rule: Rule, grants: list[Grant] | None):
         if grants is None:
@@ -456,7 +474,18 @@
             if table.name not in (grant.table, grant.view):
                 continue
             matched_group = [g.name_in_account for g in migrated_groups if g.name_in_workspace == grant.principal]
             if len(matched_group) > 0:
                 grant = dataclasses.replace(grant, principal=matched_group[0])
             matched_grants.append(grant)
         return matched_grants
+
+    def _sql_alter_to(self, table: Table, target_table_key: str):
+        return f"ALTER {table.kind} {escape_sql_identifier(table.key)} SET TBLPROPERTIES ('upgraded_to' = '{target_table_key}');"
+
+    def _sql_alter_from(self, table: Table, target_table_key: str, ws_id: int):
+        source = table.location if table.is_table_in_mount else table.key
+        return (
+            f"ALTER {table.kind} {escape_sql_identifier(target_table_key)} SET TBLPROPERTIES "
+            f"('upgraded_from' = '{source}'"
+            f" , '{table.UPGRADED_FROM_WS_PARAM}' = '{ws_id}');"
+        )
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/table_move.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/table_move.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/table_size.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/table_size.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,16 @@
             list[Table]: A list of Table objects representing the snapshot of tables.
         """
         return self._snapshot(partial(self._try_load), partial(self._crawl))
 
     def _safe_get_table_size(self, table_full_name: str) -> int | None:
         logger.debug(f"Evaluating {table_full_name} table size.")
         try:
+            # refresh table statistics to avoid stale stats in HMS
+            self._backend.execute(f"ANALYZE table {table_full_name} compute STATISTICS NOSCAN")
             # pylint: disable-next=protected-access
             return self._spark._jsparkSession.table(table_full_name).queryExecution().analyzed().stats().sizeInBytes()
         except Exception as e:  # pylint: disable=broad-exception-caught
             if "[TABLE_OR_VIEW_NOT_FOUND]" in str(e) or "[DELTA_TABLE_NOT_FOUND]" in str(e):
                 logger.warning(f"Failed to evaluate {table_full_name} table size. Table not found.")
                 return None
             if "[DELTA_MISSING_TRANSACTION_LOG]" in str(e):
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/tables.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/tables.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import re
 import typing
-from collections.abc import Iterable
+from collections.abc import Iterable, Iterator
 from dataclasses import dataclass
 from enum import Enum, auto
 from functools import partial
 
 import sqlglot
 from sqlglot import expressions
 from sqlglot.expressions import LocationProperty
@@ -24,14 +24,15 @@
 class What(Enum):
     EXTERNAL_SYNC = auto()
     EXTERNAL_HIVESERDE = auto()
     EXTERNAL_NO_SYNC = auto()
     DBFS_ROOT_DELTA = auto()
     DBFS_ROOT_NON_DELTA = auto()
     VIEW = auto()
+    TABLE_IN_MOUNT = auto()
     DB_DATASET = auto()
     UNKNOWN = auto()
 
 
 class HiveSerdeType(Enum):
     PARQUET = auto()
     AVRO = auto()
@@ -83,14 +84,16 @@
     def is_delta(self) -> bool:
         if self.table_format is None:
             return False
         return self.table_format.upper() == "DELTA"
 
     @property
     def key(self) -> str:
+        if self.is_table_in_mount:
+            return f"{self.catalog}.{self.database}.{self.location}".lower()
         return f"{self.catalog}.{self.database}.{self.name}".lower()
 
     @property
     def safe_sql_key(self) -> str:
         return escape_sql_identifier(self.key)
 
     def __hash__(self):
@@ -99,24 +102,14 @@
     def __eq__(self, other):
         return isinstance(other, Table) and self.key == other.key
 
     @property
     def kind(self) -> str:
         return "VIEW" if self.view_text is not None else "TABLE"
 
-    def sql_alter_to(self, target_table_key):
-        return f"ALTER {self.kind} {escape_sql_identifier(self.key)} SET TBLPROPERTIES ('upgraded_to' = '{target_table_key}');"
-
-    def sql_alter_from(self, target_table_key, ws_id):
-        return (
-            f"ALTER {self.kind} {escape_sql_identifier(target_table_key)} SET TBLPROPERTIES "
-            f"('upgraded_from' = '{self.key}'"
-            f" , '{self.UPGRADED_FROM_WS_PARAM}' = '{ws_id}');"
-        )
-
     def sql_unset_upgraded_to(self):
         return f"ALTER {self.kind} {escape_sql_identifier(self.key)} UNSET TBLPROPERTIES IF EXISTS('upgraded_to');"
 
     @property
     def is_dbfs_root(self) -> bool:
         if not self.location:
             return False
@@ -144,34 +137,32 @@
     @property
     def is_format_supported_for_sync(self) -> bool:
         if self.table_format is None:
             return False
         return self.table_format.upper() in {"DELTA", "PARQUET", "CSV", "JSON", "ORC", "TEXT", "AVRO"}
 
     @property
-    def is_format_supported_for_create_like(self) -> bool:
-        # Based on documentation
-        # https://docs.databricks.com/en/sql/language-manual/sql-ref-syntax-ddl-create-table-like.html
-        if self.table_format is None:
-            return False
-        return self.table_format.upper() in {"DELTA", "PARQUET", "CSV", "JSON", "TEXT"}
-
-    @property
     def is_databricks_dataset(self) -> bool:
         if not self.location:
             return False
         for db_datasets in self.DBFS_DATABRICKS_DATASETS:
             if self.location.startswith(db_datasets):
                 return True
         return False
 
     @property
+    def is_table_in_mount(self) -> bool:
+        return self.database.startswith("mounted_") and self.is_delta
+
+    @property
     def what(self) -> What:
         if self.is_databricks_dataset:
             return What.DB_DATASET
+        if self.is_table_in_mount:
+            return What.TABLE_IN_MOUNT
         if self.is_dbfs_root and self.table_format == "DELTA":
             return What.DBFS_ROOT_DELTA
         if self.is_dbfs_root:
             return What.DBFS_ROOT_NON_DELTA
         if self.kind == "TABLE" and self.is_format_supported_for_sync:
             return What.EXTERNAL_SYNC
         if self.kind == "TABLE" and self.table_format.upper() == "HIVE":
@@ -303,14 +294,37 @@
             msg = f"{self.key} is not DELTA: {self.table_format}"
             raise ValueError(msg)
         return f"CREATE TABLE IF NOT EXISTS {escape_sql_identifier(target_table_key)} DEEP CLONE {escape_sql_identifier(self.key)};"
 
     def sql_migrate_view(self, target_table_key):
         return f"CREATE VIEW IF NOT EXISTS {escape_sql_identifier(target_table_key)} AS {self.view_text};"
 
+    def sql_migrate_table_in_mount(self, target_table_key: str, table_schema: Iterator[typing.Any]):
+        fields = []
+        partitioned_fields = []
+        next_fileds_are_partitioned = False
+        for key, value, _ in table_schema:
+            if key == "# Partition Information":
+                continue
+            if key == "# col_name":
+                next_fileds_are_partitioned = True
+                continue
+            if next_fileds_are_partitioned:
+                partitioned_fields.append(f"{key}")
+            else:
+                fields.append(f"{key} {value}")
+
+        partitioned_str = ""
+        if partitioned_fields:
+            partitioning_columns = ", ".join(partitioned_fields)
+            partitioned_str = f"PARTITIONED BY ({partitioning_columns})"
+        schema = ", ".join(fields)
+
+        return f"CREATE TABLE IF NOT EXISTS {escape_sql_identifier(target_table_key)} ({schema}) {partitioned_str} LOCATION '{self.location}';"
+
 
 @dataclass
 class TableError:
     catalog: str
     database: str
     name: str | None = None
     error: str | None = None
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/tables.scala` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/tables.scala`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/udfs.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/udfs.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/verification.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/verification.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/view_migrate.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/view_migrate.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/workflows.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/hive_metastore/workflows.py`

 * *Files 10% similar despite different names*

```diff
@@ -175,17 +175,17 @@
 
     @job_task(dashboard="migration_main", depends_on=[refresh_migration_status])
     def migration_report(self, ctx: RuntimeContext):
         """Refreshes the migration dashboard after all previous tasks have been completed. Note that you can access the
         dashboard _before_ all tasks have been completed, but then only already completed information is shown."""
 
 
-class MigrateTablesInMounts(Workflow):
+class ScanTablesInMounts(Workflow):
     def __init__(self):
-        super().__init__('migrate-tables-in-mounts-experimental')
+        super().__init__('scan-tables-in-mounts-experimental')
 
     @job_task
     def scan_tables_in_mounts_experimental(self, ctx: RuntimeContext):
         """[EXPERIMENTAL] This workflow scans for Delta tables inside all mount points
         captured during the assessment. It will store the results under the `tables` table
         located under the assessment."""
         ctx.tables_in_mounts.snapshot()
@@ -194,8 +194,28 @@
     def refresh_migration_status(self, ctx: RuntimeContext):
         """Refresh the migration status to present it in the dashboard."""
         ctx.tables_migrator.index_full_refresh()
 
     @job_task(dashboard="migration_main", depends_on=[refresh_migration_status])
     def migration_report(self, ctx: RuntimeContext):
         """Refreshes the migration dashboard after all previous tasks have been completed. Note that you can access the
+        dashboard _before_ all tasks have been completed, but then only already completed information is shown."""
+
+
+class MigrateTablesInMounts(Workflow):
+    def __init__(self):
+        super().__init__('migrate-tables-in-mounts-experimental')
+
+    @job_task(job_cluster="table_migration", depends_on=[ScanTablesInMounts.scan_tables_in_mounts_experimental])
+    def migrate_tables_in_mounts_experimental(self, ctx: RuntimeContext):
+        """[EXPERIMENTAL] This workflow migrates `delta tables stored in mount points` to Unity Catalog using a Create Table statement."""
+        ctx.tables_migrator.migrate_tables(what=What.TABLE_IN_MOUNT)
+
+    @job_task(job_cluster="table_migration", depends_on=[migrate_tables_in_mounts_experimental])
+    def refresh_migration_status(self, ctx: RuntimeContext):
+        """Refresh the migration status to present it in the dashboard."""
+        ctx.tables_migrator.index_full_refresh()
+
+    @job_task(dashboard="migration_main", depends_on=[refresh_migration_status])
+    def migration_report(self, ctx: RuntimeContext):
+        """Refreshes the migration dashboard after all previous tasks have been completed. Note that you can access the
         dashboard _before_ all tasks have been completed, but then only already completed information is shown."""
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/installer/hms_lineage.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/installer/hms_lineage.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/installer/logs.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/installer/logs.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/installer/mixins.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/installer/mixins.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/installer/policy.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/installer/policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,43 +94,46 @@
         except NotFound:
             logger.warning(
                 f"Instance pool id {instance_pool_id} does not exist. Will not set instance pool in the cluster policy. You can manually edit the cluster policy after installation."
             )
             return None
 
     def _definition(self, conf: dict, instance_profile: str | None, instance_pool_id: str | None) -> str:
-        latest_lts_dbr = self._ws.clusters.select_spark_version(latest=True, long_term_support=True)
+        latest_lts_dbr = self._ws.clusters.select_spark_version(latest=True)
         node_type_id = self._ws.clusters.select_node_type(local_disk=True, min_memory_gb=16)
         policy_definition = {
             "spark_version": self._policy_config(latest_lts_dbr),
             "node_type_id": self._policy_config(node_type_id),
         }
         for key, value in conf.items():
             policy_definition[f"spark_conf.{key}"] = self._policy_config(value)
         # set the availability to on demand
         if self._ws.config.is_aws:
             if instance_profile:
                 policy_definition["aws_attributes.instance_profile_arn"] = self._policy_config(instance_profile)
             policy_definition["aws_attributes.availability"] = self._policy_config(
                 compute.AwsAvailability.ON_DEMAND.value
             )
+            policy_definition["aws_attributes.zone_id"] = self._policy_config("auto")
         elif self._ws.config.is_azure:
             policy_definition["azure_attributes.availability"] = self._policy_config(
                 compute.AzureAvailability.ON_DEMAND_AZURE.value
             )
         else:
             policy_definition["gcp_attributes.availability"] = self._policy_config(
                 compute.GcpAvailability.ON_DEMAND_GCP.value
             )
         if instance_pool_id:
             policy_definition["instance_pool_id"] = self._policy_config(instance_pool_id)
             # 'node_type_id' cannot be supplied when an instance pool ID is provided
             policy_definition.pop("node_type_id")
             # 'availability' cannot be supplied when an instance pool ID is provided
             policy_definition.pop("aws_attributes.availability", "")
+            # 'zone_id' cannot be supplied when an instance pool ID is provided
+            policy_definition.pop("aws_attributes.zone_id", "")
             policy_definition.pop("azure_attributes.availability", "")
             policy_definition.pop("gcp_attributes.availability", "")
         return json.dumps(policy_definition)
 
     @staticmethod
     def _extract_external_hive_metastore_conf(cluster_policy):
         spark_conf_dict = {}
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/installer/workflows.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/installer/workflows.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 from databricks.labs.ucx.config import WorkspaceConfig
 from databricks.labs.ucx.framework.tasks import Task
 from databricks.labs.ucx.installer.logs import PartialLogRecord, parse_logs
 from databricks.labs.ucx.installer.mixins import InstallationMixin
 
 logger = logging.getLogger(__name__)
 
+TEST_JOBS_PURGE_TIMEOUT = timedelta(hours=1, minutes=15)
 EXTRA_TASK_PARAMS = {
     "job_id": "{{job_id}}",
     "run_id": "{{run_id}}",
     "attempt": "{{job.repair_count}}",
     "parent_run_id": "{{parent_run_id}}",
 }
 DEBUG_NOTEBOOK = """# Databricks notebook source
@@ -64,15 +65,15 @@
 # MAGIC
 # MAGIC Production runs are supposed to be triggered through the following jobs: {job_links}
 # MAGIC
 # MAGIC **This notebook is overwritten with each UCX update/(re)install.**
 
 # COMMAND ----------
 
-# MAGIC %pip install /Workspace{remote_wheel}
+# MAGIC %pip install {remote_wheel}
 dbutils.library.restartPython()
 
 # COMMAND ----------
 
 import logging
 from pathlib import Path
 from databricks.labs.blueprint.installation import Installation
@@ -87,15 +88,15 @@
 cfg = Installation.load_local(WorkspaceConfig, Path("/Workspace{config_file}"))
 ws = WorkspaceClient()
 
 print(__version__)
 """
 
 TEST_RUNNER_NOTEBOOK = """# Databricks notebook source
-# MAGIC %pip install /Workspace{remote_wheel}
+# MAGIC %pip install {remote_wheel}
 dbutils.library.restartPython()
 
 # COMMAND ----------
 
 from databricks.labs.ucx.runtime import main
 
 main(f'--config=/Workspace{config_file}',
@@ -398,22 +399,22 @@
         self._verify_timeout = verify_timeout
         self._tasks = tasks
         self._this_file = Path(__file__)
         self._skip_dashboards = skip_dashboards
         super().__init__(config, installation, ws)
 
     def create_jobs(self):
-        remote_wheel = self._upload_wheel()
+        remote_wheels = self._upload_wheel()
         desired_workflows = {t.workflow for t in self._tasks if t.cloud_compatible(self._ws.config)}
         wheel_runner = None
 
         if self._config.override_clusters:
-            wheel_runner = self._upload_wheel_runner(remote_wheel)
+            wheel_runner = self._upload_wheel_runner(remote_wheels)
         for workflow_name in desired_workflows:
-            settings = self._job_settings(workflow_name, remote_wheel)
+            settings = self._job_settings(workflow_name, remote_wheels)
             if self._config.override_clusters:
                 settings = self._apply_cluster_overrides(
                     workflow_name,
                     settings,
                     self._config.override_clusters,
                     wheel_runner,
                 )
@@ -425,24 +426,28 @@
                     logger.info(f"Removing job_id={job_id}, as it is no longer needed")
                     self._ws.jobs.delete(job_id)
                 except InvalidParameterValue:
                     logger.warning(f"step={workflow_name} does not exist anymore for some reason")
                     continue
 
         self._install_state.save()
-        self._create_debug(remote_wheel)
+        self._create_debug(remote_wheels)
         return self._create_readme()
 
     @property
     def _config_file(self):
         return f"{self._installation.install_folder()}/config.yml"
 
     def _is_testing(self):
         return self._product_info.product_name() != "ucx"
 
+    @staticmethod
+    def _get_test_purge_time() -> str:
+        return (datetime.utcnow() + TEST_JOBS_PURGE_TIMEOUT).strftime("%Y%m%d%H")
+
     def _create_readme(self) -> str:
         debug_notebook_link = self._installation.workspace_markdown_link('debug notebook', 'DEBUG.py')
         markdown = [
             "# UCX - The Unity Catalog Migration Assistant",
             f'To troubleshoot, see {debug_notebook_link}.\n',
             "Here are the URLs and descriptions of workflows that trigger various stages of migration.",
             "All jobs are defined with necessary cluster configurations and DBR versions.\n",
@@ -520,21 +525,38 @@
                 return self._deploy_workflow(step_name, settings)
         logger.info(f"Creating new job configuration for step={step_name}")
         new_job = self._ws.jobs.create(**settings)
         assert new_job.job_id is not None
         self._install_state.jobs[step_name] = str(new_job.job_id)
         return None
 
+    @staticmethod
+    def _library_dep_order(library: str):
+        match library:
+            case library if 'sdk' in library:
+                return 0
+            case library if 'blueprint' in library:
+                return 1
+            case _:
+                return 2
+
     def _upload_wheel(self):
+        wheel_paths = []
         with self._wheels:
-            return self._wheels.upload_to_wsfs()
+            if self._config.upload_dependencies:
+                wheel_paths = self._wheels.upload_wheel_dependencies(["databricks", "sqlglot"])
+            wheel_paths.sort(key=WorkflowsDeployment._library_dep_order)
+            wheel_paths.append(self._wheels.upload_to_wsfs())
+            wheel_paths = [f"/Workspace{wheel}" for wheel in wheel_paths]
+            return wheel_paths
 
-    def _upload_wheel_runner(self, remote_wheel: str):
+    def _upload_wheel_runner(self, remote_wheels: list[str]):
         # TODO: we have to be doing this workaround until ES-897453 is solved in the platform
-        code = TEST_RUNNER_NOTEBOOK.format(remote_wheel=remote_wheel, config_file=self._config_file).encode("utf8")
+        remote_wheels_str = " ".join(remote_wheels)
+        code = TEST_RUNNER_NOTEBOOK.format(remote_wheel=remote_wheels_str, config_file=self._config_file).encode("utf8")
         return self._installation.upload(f"wheels/wheel-test-runner-{self._product_info.version()}.py", code)
 
     @staticmethod
     def _apply_cluster_overrides(
         workflow_name: str,
         settings: dict[str, Any],
         overrides: dict[str, str],
@@ -550,56 +572,62 @@
                 job_task.libraries = None
             if job_task.python_wheel_task is not None:
                 job_task.python_wheel_task = None
                 widget_values = {"task": job_task.task_key, 'workflow': workflow_name} | EXTRA_TASK_PARAMS
                 job_task.notebook_task = jobs.NotebookTask(notebook_path=wheel_runner, base_parameters=widget_values)
         return settings
 
-    def _job_settings(self, step_name: str, remote_wheel: str):
+    def _job_settings(self, step_name: str, remote_wheels: list[str]) -> dict[str, Any]:
         email_notifications = None
         if not self._config.override_clusters and "@" in self._my_username:
             # set email notifications only if we're running the real
             # installation and not the integration test.
             email_notifications = jobs.JobEmailNotifications(
                 on_success=[self._my_username], on_failure=[self._my_username]
             )
+
         job_tasks = []
         job_clusters: set[str] = {Task.job_cluster}
         for task in self._tasks:
             if task.workflow != step_name:
                 continue
             if self._skip_dashboards and task.dashboard:
                 continue
             job_clusters.add(task.job_cluster)
-            job_tasks.append(self._job_task(task, remote_wheel))
-        job_tasks.append(self._job_parse_logs_task(job_tasks, step_name, remote_wheel))
+            job_tasks.append(self._job_task(task, remote_wheels))
+        job_tasks.append(self._job_parse_logs_task(job_tasks, step_name, remote_wheels))
         version = self._product_info.version()
         version = version if not self._ws.config.is_gcp else version.replace("+", "-")
+        tags = {"version": f"v{version}"}
+        if self._is_testing():
+            # add RemoveAfter tag for test job cleanup
+            date_to_remove = self._get_test_purge_time()
+            tags.update({"RemoveAfter": date_to_remove})
         return {
             "name": self._name(step_name),
-            "tags": {"version": f"v{version}"},
+            "tags": tags,
             "job_clusters": self._job_clusters(job_clusters),
             "email_notifications": email_notifications,
             "tasks": job_tasks,
         }
 
-    def _job_task(self, task: Task, remote_wheel: str) -> jobs.Task:
+    def _job_task(self, task: Task, remote_wheels: list[str]) -> jobs.Task:
         jobs_task = jobs.Task(
             task_key=task.name,
             job_cluster_key=task.job_cluster,
             depends_on=[jobs.TaskDependency(task_key=d) for d in task.dependencies()],
         )
         if task.dashboard:
             # dashboards are created in parallel to wheel uploads, so we'll just retry
             retry_on_attribute_error = retried(on=[KeyError], timeout=self._verify_timeout)
             retried_job_dashboard_task = retry_on_attribute_error(self._job_dashboard_task)
             return retried_job_dashboard_task(jobs_task, task)
         if task.notebook:
             return self._job_notebook_task(jobs_task, task)
-        return self._job_wheel_task(jobs_task, task.workflow, remote_wheel)
+        return self._job_wheel_task(jobs_task, task.workflow, remote_wheels)
 
     def _job_dashboard_task(self, jobs_task: jobs.Task, task: Task) -> jobs.Task:
         assert task.dashboard is not None
         dashboard_id = self._install_state.dashboards[task.dashboard]
         return replace(
             jobs_task,
             job_cluster_key=None,
@@ -623,16 +651,18 @@
                     "task": task.name,
                     "config": f"/Workspace{self._config_file}",
                 }
                 | EXTRA_TASK_PARAMS,
             ),
         )
 
-    def _job_wheel_task(self, jobs_task: jobs.Task, workflow: str, remote_wheel: str) -> jobs.Task:
-        libraries = [compute.Library(whl=f"/Workspace{remote_wheel}")]
+    def _job_wheel_task(self, jobs_task: jobs.Task, workflow: str, remote_wheels: list[str]) -> jobs.Task:
+        libraries = []
+        for wheel in remote_wheels:
+            libraries.append(compute.Library(whl=wheel))
         named_parameters = {
             "config": f"/Workspace{self._config_file}",
             "workflow": workflow,
             "task": jobs_task.task_key,
         }
         return replace(
             jobs_task,
@@ -685,74 +715,72 @@
                             min_workers=self._config.min_workers,
                         ),
                     ),
                 )
             )
         return clusters
 
-    def _job_parse_logs_task(self, job_tasks: list[jobs.Task], workflow: str, remote_wheel: str) -> jobs.Task:
+    def _job_parse_logs_task(self, job_tasks: list[jobs.Task], workflow: str, remote_wheels: list[str]) -> jobs.Task:
         jobs_task = jobs.Task(
             task_key="parse_logs",
             job_cluster_key=Task.job_cluster,
             # The task dependents on all previous tasks.
             depends_on=[jobs.TaskDependency(task_key=task.task_key) for task in job_tasks],
             run_if=jobs.RunIf.ALL_DONE,
         )
-        return self._job_wheel_task(jobs_task, workflow, remote_wheel)
+        return self._job_wheel_task(jobs_task, workflow, remote_wheels)
 
-    def _create_debug(self, remote_wheel: str):
+    def _create_debug(self, remote_wheels: list[str]):
         readme_link = self._installation.workspace_link('README')
         job_links = ", ".join(
             f"[{self._name(step_name)}]({self._ws.config.host}#job/{job_id})"
             for step_name, job_id in self._install_state.jobs.items()
         )
         content = DEBUG_NOTEBOOK.format(
-            remote_wheel=remote_wheel, readme_link=readme_link, job_links=job_links, config_file=self._config_file
+            remote_wheel=remote_wheels, readme_link=readme_link, job_links=job_links, config_file=self._config_file
         ).encode("utf8")
         self._installation.upload('DEBUG.py', content)
 
 
 class MaxedStreamHandler(logging.StreamHandler):
 
     MAX_STREAM_SIZE = 2**20 - 2**6  # 1 Mb minus some buffer
     _installed_handlers: dict[str, tuple[logging.Logger, MaxedStreamHandler]] = {}
+    _sent_bytes = 0
 
     @classmethod
     def install_handler(cls, logger_: logging.Logger):
         if logger_.handlers:
             # already installed ?
             installed = next((h for h in logger_.handlers if isinstance(h, MaxedStreamHandler)), None)
             if installed:
                 return
             # any handler to override ?
             handler = next((h for h in logger_.handlers if isinstance(h, logging.StreamHandler)), None)
             if handler:
-                to_install = MaxedStreamHandler(cls.MAX_STREAM_SIZE, handler)
+                to_install = MaxedStreamHandler(handler)
                 cls._installed_handlers[logger_.name] = (logger_, to_install)
                 logger_.removeHandler(handler)
                 logger_.addHandler(to_install)
                 return
         if logger_.parent:
             cls.install_handler(logger_.parent)
         if logger_.root:
             cls.install_handler(logger_.root)
 
     @classmethod
     def uninstall_handlers(cls):
-        for pair in cls._installed_handlers.values():
-            logger_ = pair[0]
-            handler = pair[1]
+        for logger_, handler in cls._installed_handlers.values():
             logger_.removeHandler(handler)
             logger_.addHandler(handler.original_handler)
         cls._installed_handlers.clear()
+        cls._sent_bytes = 0
 
-    def __init__(self, max_bytes: int, original_handler: logging.StreamHandler):
+    def __init__(self, original_handler: logging.StreamHandler):
         super().__init__()
-        self._max_bytes = max_bytes
-        self._sent_bytes = 0
         self._original_handler = original_handler
 
     @property
     def original_handler(self):
         return self._original_handler
 
     def emit(self, record):
@@ -768,13 +796,13 @@
         # so ensuring not to break the logging logic
         # pylint: disable=broad-exception-caught
         except Exception:
             self.handleError(record)
 
     def _prevent_overflow(self, msg: str):
         data = msg.encode("utf-8")
-        if self._sent_bytes + len(data) > self._max_bytes:
+        if self._sent_bytes + len(data) > self.MAX_STREAM_SIZE:
             # ensure readers are aware of why the logs are incomplete
             self.stream.write(f"MAX LOGS SIZE REACHED: {self._sent_bytes} bytes!!!")
             self.flush()
             return True
         return False
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/mixins/fixtures.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/mixins/fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import pathlib
 import shutil
 import string
 import subprocess
 import sys
 from collections.abc import Callable, Generator, MutableMapping
-from datetime import timedelta
+from datetime import timedelta, datetime
 from pathlib import Path
 from typing import BinaryIO
 
 import pytest
 from databricks.labs.lsql.backends import StatementExecutionBackend
 from databricks.labs.blueprint.commands import CommandExecutor
 from databricks.sdk import AccountClient, WorkspaceClient
@@ -42,23 +42,26 @@
     CreateWarehouseRequestWarehouseType,
     GetResponse,
     ObjectTypePlural,
     Query,
     Dashboard,
     WidgetOptions,
     WidgetPosition,
+    EndpointTagPair,
+    EndpointTags,
 )
 from databricks.sdk.service.workspace import ImportFormat, Language
 
 from databricks.labs.ucx.workspace_access.groups import MigratedGroup
 
 # this file will get to databricks-labs-pytester project and be maintained/refactored there
 # pylint: disable=redefined-outer-name,too-many-try-statements,import-outside-toplevel,unnecessary-lambda,too-complex,invalid-name
 
 logger = logging.getLogger(__name__)
+TEST_JOBS_PURGE_TIMEOUT = timedelta(hours=1, minutes=15)  # 15 minutes grace for jobs starting at the end of the hour
 
 
 def factory(name, create, remove):
     cleanup = []
 
     def inner(**kwargs):
         x = create(**kwargs)
@@ -716,14 +719,18 @@
                 }
             else:
                 kwargs["spark_conf"] = {"spark.databricks.cluster.profile": "singleNode", "spark.master": "local[*]"}
             kwargs["custom_tags"] = {"ResourceClass": "SingleNode"}
         if "instance_pool_id" not in kwargs:
             kwargs["node_type_id"] = ws.clusters.select_node_type(local_disk=True, min_memory_gb=16)
 
+        if "custom_tags" not in kwargs:
+            kwargs["custom_tags"] = {"RemoveAfter": get_test_purge_time()}
+        else:
+            kwargs["custom_tags"]["RemoveAfter"] = get_test_purge_time()
         return ws.clusters.create(
             cluster_name=cluster_name,
             spark_version=spark_version,
             autotermination_minutes=autotermination_minutes,
             **kwargs,
         )
 
@@ -756,28 +763,33 @@
 @pytest.fixture
 def make_instance_pool(ws, make_random):
     def create(*, instance_pool_name=None, node_type_id=None, **kwargs):
         if instance_pool_name is None:
             instance_pool_name = f"sdk-{make_random(4)}"
         if node_type_id is None:
             node_type_id = ws.clusters.select_node_type(local_disk=True, min_memory_gb=16)
-        return ws.instance_pools.create(instance_pool_name, node_type_id, **kwargs)
+        return ws.instance_pools.create(
+            instance_pool_name, node_type_id, custom_tags={"RemoveAfter": get_test_purge_time()}, **kwargs
+        )
 
     yield from factory("instance pool", create, lambda item: ws.instance_pools.delete(item.instance_pool_id))
 
 
 @pytest.fixture
 def make_job(ws, make_random, make_notebook):
     def create(notebook_path: str | Path | None = None, **kwargs):
         task_spark_conf = None
         if "name" not in kwargs:
             kwargs["name"] = f"sdk-{make_random(4)}"
         if "spark_conf" in kwargs:
             task_spark_conf = kwargs["spark_conf"]
             kwargs.pop("spark_conf")
+        libraries = None
+        if "libraries" in kwargs:
+            libraries = kwargs.pop("libraries")
         if isinstance(notebook_path, pathlib.Path):
             notebook_path = str(notebook_path)
         if not notebook_path:
             notebook_path = make_notebook()
         assert notebook_path is not None
         if "tasks" not in kwargs:
             kwargs["tasks"] = [
@@ -787,17 +799,28 @@
                     new_cluster=compute.ClusterSpec(
                         num_workers=1,
                         node_type_id=ws.clusters.select_node_type(local_disk=True, min_memory_gb=16),
                         spark_version=ws.clusters.select_spark_version(latest=True),
                         spark_conf=task_spark_conf,
                     ),
                     notebook_task=jobs.NotebookTask(notebook_path=str(notebook_path)),
+                    libraries=libraries,
                     timeout_seconds=0,
                 )
             ]
+
+        # add RemoveAfter tag for test job cleanup
+        date_to_remove = get_test_purge_time()
+        remove_after_tag = {"key": "RemoveAfter", "value": date_to_remove}
+
+        if 'tags' not in kwargs:
+            kwargs["tags"] = [remove_after_tag]
+        else:
+            kwargs["tags"].append(remove_after_tag)
+
         job = ws.jobs.create(**kwargs)
         logger.info(f"Job: {ws.config.host}#job/{job.job_id}")
         return job
 
     yield from factory("job", create, lambda item: ws.jobs.delete(item.job_id))
 
 
@@ -855,20 +878,22 @@
         if warehouse_name is None:
             warehouse_name = f"sdk-{make_random(4)}"
         if warehouse_type is None:
             warehouse_type = CreateWarehouseRequestWarehouseType.PRO
         if cluster_size is None:
             cluster_size = "2X-Small"
 
+        remove_after_tags = EndpointTags(custom_tags=[EndpointTagPair(key="RemoveAfter", value=get_test_purge_time())])
         return ws.warehouses.create(
             name=warehouse_name,
             cluster_size=cluster_size,
             warehouse_type=warehouse_type,
             max_num_clusters=max_num_clusters,
             enable_serverless_compute=enable_serverless_compute,
+            tags=remove_after_tags,
             **kwargs,
         )
 
     yield from factory("warehouse", create, lambda item: ws.warehouses.delete(item.id))
 
 
 def _is_in_debug() -> bool:
@@ -945,15 +970,15 @@
 
 @pytest.fixture
 def make_schema(ws, sql_backend, make_random) -> Generator[Callable[..., SchemaInfo], None, None]:
     def create(*, catalog_name: str = "hive_metastore", name: str | None = None) -> SchemaInfo:
         if name is None:
             name = f"ucx_S{make_random(4)}".lower()
         full_name = f"{catalog_name}.{name}".lower()
-        sql_backend.execute(f"CREATE SCHEMA {full_name}")
+        sql_backend.execute(f"CREATE SCHEMA {full_name} WITH DBPROPERTIES (RemoveAfter={get_test_purge_time()})")
         schema_info = SchemaInfo(catalog_name=catalog_name, name=name, full_name=full_name)
         logger.info(
             f"Schema {schema_info.full_name}: "
             f"{ws.config.host}/explore/data/{schema_info.catalog_name}/{schema_info.name}"
         )
         return schema_info
 
@@ -968,23 +993,24 @@
 
     yield from factory("schema", create, remove)
 
 
 @pytest.fixture
 # pylint: disable-next=too-many-statements
 def make_table(ws, sql_backend, make_schema, make_random) -> Generator[Callable[..., TableInfo], None, None]:
-    def create(  # pylint: disable=too-many-locals,too-many-arguments
+    def create(  # pylint: disable=too-many-locals,too-many-arguments,too-many-statements
         *,
         catalog_name="hive_metastore",
         schema_name: str | None = None,
         name: str | None = None,
         ctas: str | None = None,
         non_delta: bool = False,
         external: bool = False,
         external_csv: str | None = None,
+        external_delta: str | None = None,
         view: bool = False,
         tbl_properties: dict[str, str] | None = None,
         hiveserde_ddl: str | None = None,
         storage_override: str | None = None,
     ) -> TableInfo:
         if schema_name is None:
             schema = make_schema(catalog_name=catalog_name)
@@ -1014,38 +1040,60 @@
                 f"JSON.`dbfs:/databricks-datasets/iot-stream/data-device`"
             )
         elif external_csv is not None:
             table_type = TableType.EXTERNAL
             data_source_format = DataSourceFormat.CSV
             storage_location = external_csv
             ddl = f"{ddl} USING CSV OPTIONS (header=true) LOCATION '{storage_location}'"
+        elif external_delta is not None:
+            table_type = TableType.EXTERNAL
+            data_source_format = DataSourceFormat.DELTA
+            storage_location = external_delta
+            ddl = f"{ddl} (id string) LOCATION '{storage_location}'"
         elif external:
             # external table
             table_type = TableType.EXTERNAL
             data_source_format = DataSourceFormat.DELTASHARING
             url = "s3a://databricks-datasets-oregon/delta-sharing/share/open-datasets.share"
             storage_location = f"{url}#delta_sharing.default.lending_club"
             ddl = f"{ddl} USING deltaSharing LOCATION '{storage_location}'"
         else:
             # managed table
             table_type = TableType.MANAGED
             data_source_format = DataSourceFormat.DELTA
             storage_location = f"dbfs:/user/hive/warehouse/{schema_name}/{name}"
             ddl = f"{ddl} (id INT, value STRING)"
         if tbl_properties:
-            str_properties = ",".join([f" '{k}' = '{v}' " for k, v in tbl_properties.items()])
+            tbl_properties.update({"RemoveAfter": get_test_purge_time()})
+        else:
+            tbl_properties = {"RemoveAfter": get_test_purge_time()}
+
+        str_properties = ",".join([f" '{k}' = '{v}' " for k, v in tbl_properties.items()])
+
+        # table properties fails with CTAS statements
+        alter_table_tbl_properties = ""
+        if ctas or non_delta:
+            alter_table_tbl_properties = (
+                f'ALTER {"VIEW" if view else "TABLE"} {full_name} SET TBLPROPERTIES ({str_properties})'
+            )
+        else:
             ddl = f"{ddl} TBLPROPERTIES ({str_properties})"
 
         if hiveserde_ddl:
             ddl = hiveserde_ddl
             data_source_format = None
             table_type = TableType.EXTERNAL
             storage_location = storage_override
 
         sql_backend.execute(ddl)
+
+        # CTAS AND NON_DELTA does not support TBLPROPERTIES
+        if ctas or non_delta:
+            sql_backend.execute(alter_table_tbl_properties)
+
         table_info = TableInfo(
             catalog_name=catalog_name,
             schema_name=schema_name,
             name=name,
             full_name=full_name,
             properties=tbl_properties,
             storage_location=storage_location,
@@ -1318,7 +1366,11 @@
     def remove(dashboard: Dashboard):
         try:
             ws.dashboards.delete(dashboard_id=dashboard.id)
         except RuntimeError as e:
             logger.info(f"Can't delete dashboard {e}")
 
     yield from factory("dashboard", create, remove)
+
+
+def get_test_purge_time() -> str:
+    return (datetime.utcnow() + TEST_JOBS_PURGE_TIMEOUT).strftime("%Y%m%d%H")
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/mixins/redash.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/mixins/redash.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/mixins/wspath.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/mixins/wspath.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,14 @@
     _SUFFIXES = {'.py': Language.PYTHON, '.sql': Language.SQL, '.scala': Language.SCALA, '.R': Language.R}
 
     _ws: WorkspaceClient
     _flavour: _DatabricksFlavour
     _accessor: _DatabricksAccessor
 
     cwd = _na('cwd')
-    resolve = _na('resolve')
     stat = _na('stat')
     chmod = _na('chmod')
     lchmod = _na('lchmod')
     lstat = _na('lstat')
     owner = _na('owner')
     group = _na('group')
     readlink = _na('readlink')
@@ -386,14 +385,17 @@
     is_block_device = _return_false
     is_char_device = _return_false
     is_fifo = _return_false
     is_socket = _return_false
     is_mount = _return_false
     is_junction = _return_false
 
+    def resolve(self, strict=False):
+        return self
+
     def is_dir(self):
         try:
             return self._object_info.object_type == ObjectType.DIRECTORY
         except DatabricksError:
             return False
 
     def is_file(self):
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/00_0_metastore_assignment.md` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/estimates/00_0_metastore_assignment.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/01_0_group_migration.md` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/estimates/01_0_group_migration.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/02_0_data_modeling.md` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/estimates/02_0_data_modeling.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/03_0_data_migration.md` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/estimates/03_0_data_migration.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/03_5_data_migration_complexity.sql` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/estimates/03_5_data_migration_complexity.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/interactive/00_0_interactive.md` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/interactive/00_0_interactive.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/interactive/01_0_compute_access_mode_limitation_summary.sql` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/interactive/01_0_compute_access_mode_limitation_summary.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/interactive/02_0_cluster_summary.md` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/interactive/02_0_cluster_summary.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/interactive/03_0_cluster_summary.sql` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/interactive/03_0_cluster_summary.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/02_2_count_table_by_storage.sql` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/02_2_count_table_by_storage.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/10_0_all_tables.sql` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/10_0_all_tables.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/10_0_database_summary.sql` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/10_0_database_summary.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/40_2_logs.sql` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/assessment/main/40_2_logs.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/views/code_patterns.sql` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/views/code_patterns.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/views/grant_detail.sql` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/views/grant_detail.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/views/misc_patterns.sql` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/views/misc_patterns.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/views/objects.sql` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/views/objects.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/views/table_estimates.sql` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/queries/views/table_estimates.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/ast_helpers.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/ast_helpers.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/base.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 from abc import abstractmethod
 from collections.abc import Iterable
 from dataclasses import dataclass
+from pathlib import Path
+
 
 # Code mapping between LSP, PyLint, and our own diagnostics:
 # | LSP                       | PyLint     | Our            |
 # |---------------------------|------------|----------------|
 # | Severity.ERROR            | Error      | Failure()      |
 # | Severity.WARN             | Warning    | Advisory()     |
 # | DiagnosticTag.DEPRECATED  | Warning    | Deprecation()  |
@@ -50,14 +52,23 @@
 
     def as_deprecation(self) -> 'Deprecation':
         return Deprecation(**self.__dict__)
 
     def as_convention(self) -> 'Convention':
         return Convention(**self.__dict__)
 
+    def for_path(self, path: Path) -> LocatedAdvice:
+        return LocatedAdvice(self, path)
+
+
+@dataclass
+class LocatedAdvice:
+    advice: Advice
+    path: Path
+
 
 class Advisory(Advice):
     """A warning that does not prevent the code from running."""
 
 
 class Failure(Advisory):
     """An error that prevents the code from running."""
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/dbfs.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/dbfs.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/graph.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/graph.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 import abc
+import ast
 from dataclasses import dataclass
 from pathlib import Path
 from collections.abc import Callable
+from typing import cast
 
 from databricks.labs.ucx.source_code.base import Advisory
 from databricks.labs.ucx.source_code.python_linter import (
     ASTLinter,
     PythonLinter,
     SysPathChange,
     NotebookRunCall,
@@ -40,20 +42,22 @@
     def dependency(self):
         return self._dependency
 
     @property
     def path(self):
         return self._dependency.path
 
-    def register_library(self, name: str) -> MaybeGraph:
-        # TODO: use DistInfoResolver to load wheel/egg/pypi dependencies
-        # TODO: https://github.com/databrickslabs/ucx/issues/1642
+    def register_library(self, library: str) -> list[DependencyProblem]:
         # TODO: https://github.com/databrickslabs/ucx/issues/1643
         # TODO: https://github.com/databrickslabs/ucx/issues/1640
-        return MaybeGraph(None, [DependencyProblem('not-yet-implemented', f'Library dependency: {name}')])
+        maybe = self._resolver.resolve_library(self.path_lookup, library)
+        if not maybe.dependency:
+            return maybe.problems
+        maybe_graph = self.register_dependency(maybe.dependency)
+        return maybe_graph.problems
 
     def register_notebook(self, path: Path) -> list[DependencyProblem]:
         maybe = self._resolver.resolve_notebook(self.path_lookup, path)
         if not maybe.dependency:
             return maybe.problems
         maybe_graph = self.register_dependency(maybe.dependency)
         return maybe_graph.problems
@@ -65,24 +69,25 @@
         if not maybe.dependency:
             return maybe.problems
         maybe_graph = self.register_dependency(maybe.dependency)
         return maybe_graph.problems
 
     def register_dependency(self, dependency: Dependency) -> MaybeGraph:
         # TODO: this has to be a private method, because we don't want to allow free-form dependencies.
-        # the only case we have for this method to be used outside of this class is for SitePackages (or DistInfo)
-        # See databricks.labs.ucx.source_code.site_packages.SitePackageContainer.build_dependency_graph for reference
+        # the only case we have for this method to be used outside of this class is for DistInfoPackage
+        # See databricks.labs.ucx.source_code.python_libraries.DistInfoContainer.build_dependency_graph for reference
         maybe = self.locate_dependency(dependency.path)
         if maybe.graph is not None:
             self._dependencies[dependency] = maybe.graph
             return maybe
         # nay, create the child graph and populate it
         child_graph = DependencyGraph(dependency, self, self._resolver, self._path_lookup)
         self._dependencies[dependency] = child_graph
         container = dependency.load(self.path_lookup)
+        # TODO: Return either (child) graph OR problems
         if not container:
             problem = DependencyProblem('dependency-register-failed', 'Failed to register dependency', dependency.path)
             return MaybeGraph(child_graph, [problem])
         problems = container.build_dependency_graph(child_graph)
         return MaybeGraph(
             child_graph,
             [
@@ -92,24 +97,17 @@
                 for problem in problems
             ],
         )
 
     def locate_dependency(self, path: Path) -> MaybeGraph:
         # need a list since unlike JS, Python won't let you assign closure variables
         found: list[DependencyGraph] = []
-        # TODO https://github.com/databrickslabs/ucx/issues/1287
-        posix_path = path.as_posix()
-        posix_path = posix_path[2:] if posix_path.startswith('./') else posix_path
 
         def check_registered_dependency(graph):
-            # TODO https://github.com/databrickslabs/ucx/issues/1287
-            graph_posix_path = graph.path.as_posix()
-            if graph_posix_path.startswith('./'):
-                graph_posix_path = graph_posix_path[2:]
-            if graph_posix_path == posix_path:
+            if graph.path == path:
                 found.append(graph)
                 return True
             return False
 
         self.root.visit(check_registered_dependency, set())
         if not found:
             return MaybeGraph(None, [DependencyProblem('dependency-not-found', 'Dependency not found')])
@@ -160,15 +158,16 @@
         return False
 
     def build_graph_from_python_source(self, python_code: str) -> list[DependencyProblem]:
         problems: list[DependencyProblem] = []
         linter = ASTLinter.parse(python_code)
         syspath_changes = PythonLinter.list_sys_path_changes(linter)
         run_calls = PythonLinter.list_dbutils_notebook_run_calls(linter)
-        import_sources = PythonLinter.list_import_sources(linter)
+        import_sources, import_problems = PythonLinter.list_import_sources(linter, DependencyProblem)
+        problems.extend(cast(list[DependencyProblem], import_problems))
         nodes = syspath_changes + run_calls + import_sources
         # need to execute things in intertwined sequence so concat and sort
         for base_node in sorted(nodes, key=lambda node: node.node.lineno * 10000 + node.node.col_offset):
             for problem in self._process_node(base_node):
                 problem = problem.replace(
                     start_line=base_node.node.lineno,
                     start_col=base_node.node.col_offset,
@@ -184,15 +183,17 @@
         if isinstance(base_node, NotebookRunCall):
             strpath = base_node.get_constant_path()
             if strpath is None:
                 yield DependencyProblem('dependency-not-constant', "Can't check dependency not provided as a constant")
             else:
                 yield from self.register_notebook(Path(strpath))
         if isinstance(base_node, ImportSource):
-            yield from self.register_import(base_node.name)
+            prefix = ("." * base_node.node.level) if isinstance(base_node.node, ast.ImportFrom) else ""
+            name = base_node.name or ""
+            yield from self.register_import(prefix + name)
 
     def _mutate_path_lookup(self, change: SysPathChange):
         path = Path(change.path)
         if not path.is_absolute():
             path = self._path_lookup.cwd / path
         if change.is_append:
             self._path_lookup.append_path(path)
@@ -226,148 +227,202 @@
         return f"Dependency<{self.path}>"
 
 
 class SourceContainer(abc.ABC):
 
     @abc.abstractmethod
     def build_dependency_graph(self, parent: DependencyGraph) -> list[DependencyProblem]:
-        raise NotImplementedError()
+        """builds a dependency graph from the contents of this container"""
 
 
 class DependencyLoader(abc.ABC):
     @abc.abstractmethod
     def load_dependency(self, path_lookup: PathLookup, dependency: Dependency) -> SourceContainer | None:
-        raise NotImplementedError()
+        """loads a dependency"""
 
 
 class WrappingLoader(DependencyLoader):
 
     def __init__(self, source_container: SourceContainer):
         self._source_container = source_container
 
     def load_dependency(self, path_lookup: PathLookup, dependency: Dependency) -> SourceContainer | None:
         return self._source_container
 
     def __repr__(self):
         return f"<WrappingLoader source_container={self._source_container}>"
 
 
-class BaseDependencyResolver(abc.ABC):
+class BaseLibraryResolver(abc.ABC):
 
-    def __init__(self, next_resolver: BaseDependencyResolver | None):
+    def __init__(self, next_resolver: BaseLibraryResolver | None):
         self._next_resolver = next_resolver
 
     @abc.abstractmethod
-    def with_next_resolver(self, resolver: BaseDependencyResolver) -> BaseDependencyResolver:
-        raise NotImplementedError()
+    def with_next_resolver(self, resolver: BaseLibraryResolver) -> BaseLibraryResolver:
+        """required to create a linked list of resolvers"""
 
-    @property
-    def next_resolver(self):
-        return self._next_resolver
+    def resolve_library(self, path_lookup: PathLookup, library: Path) -> MaybeDependency:
+        assert self._next_resolver is not None
+        return self._next_resolver.resolve_library(path_lookup, library)
 
+
+class BaseNotebookResolver(abc.ABC):
+
+    @abc.abstractmethod
     def resolve_notebook(self, path_lookup: PathLookup, path: Path) -> MaybeDependency:
-        # TODO: remove StubResolver and return MaybeDependency(None, [...])
-        assert self._next_resolver is not None
-        return self._next_resolver.resolve_notebook(path_lookup, path)
+        """locates a notebook"""
+
+    @staticmethod
+    def _fail(code: str, message: str) -> MaybeDependency:
+        return MaybeDependency(None, [DependencyProblem(code, message)])
 
-    def resolve_local_file(self, path_lookup, path: Path) -> MaybeDependency:
-        assert self._next_resolver is not None
-        return self._next_resolver.resolve_local_file(path_lookup, path)
 
+class BaseImportResolver(abc.ABC):
+
+    @abc.abstractmethod
     def resolve_import(self, path_lookup: PathLookup, name: str) -> MaybeDependency:
-        # TODO: remove StubResolver and return MaybeDependency(None, [...])
-        assert self._next_resolver is not None
-        return self._next_resolver.resolve_import(path_lookup, name)
+        """resolve a simple or composite import name"""
+
+
+class BaseFileResolver(abc.ABC):
+
+    @abc.abstractmethod
+    def resolve_local_file(self, path_lookup, path: Path) -> MaybeDependency:
+        """locates a file"""
 
 
-class StubResolver(BaseDependencyResolver):
+class StubLibraryResolver(BaseLibraryResolver):
 
     def __init__(self):
         super().__init__(None)
 
-    def with_next_resolver(self, resolver: BaseDependencyResolver) -> BaseDependencyResolver:
+    def with_next_resolver(self, resolver: BaseLibraryResolver) -> BaseLibraryResolver:
         raise NotImplementedError("Should never happen!")
 
-    def resolve_notebook(self, path_lookup: PathLookup, path: Path) -> MaybeDependency:
-        return self._fail('notebook-not-found', f"Notebook not found: {path.as_posix()}")
-
-    def resolve_local_file(self, path_lookup: PathLookup, path: Path) -> MaybeDependency:
-        return self._fail('file-not-found', f"File not found: {path.as_posix()}")
-
-    def resolve_import(self, path_lookup: PathLookup, name: str) -> MaybeDependency:
-        return self._fail('import-not-found', f"Could not locate import: {name}")
+    def resolve_library(self, path_lookup: PathLookup, library: Path) -> MaybeDependency:
+        return self._fail('library-not-found', f"Could not resolve library: {library.as_posix()}")
 
     @staticmethod
     def _fail(code: str, message: str):
         return MaybeDependency(None, [DependencyProblem(code, message)])
 
 
 @dataclass
 class MaybeDependency:
     dependency: Dependency | None
     problems: list[DependencyProblem]
 
 
 class DependencyResolver:
-    def __init__(self, resolvers: list[BaseDependencyResolver], path_lookup: PathLookup):
-        previous: BaseDependencyResolver = StubResolver()
-        for resolver in resolvers:
+    """the DependencyResolver is responsible for locating "stuff", mimicking the Databricks runtime behavior.
+    There are specific resolution algorithms for import and for Notebooks (executed via %run or dbutils.notebook.run)
+    so we're using 2 distinct resolvers for notebooks (instance) and imports (linked list of specialized sub-resolvers)
+    resolving imports is affected by cwd and sys.paths, the latter being itself influenced by Python code
+    we therefore need a PathLookup to convey these during import resolution
+    """
+
+    def __init__(
+        self,
+        library_resolvers: list[BaseLibraryResolver],
+        notebook_resolver: BaseNotebookResolver,
+        import_resolver: BaseImportResolver,
+        path_lookup: PathLookup,
+    ):
+        self._library_resolver = self._chain_library_resolvers(library_resolvers)
+        self._notebook_resolver = notebook_resolver
+        self._import_resolver = import_resolver
+        self._path_lookup = path_lookup
+
+    @staticmethod
+    def _chain_library_resolvers(library_resolvers: list[BaseLibraryResolver]) -> BaseLibraryResolver:
+        previous: BaseLibraryResolver = StubLibraryResolver()
+        for resolver in library_resolvers:
             resolver = resolver.with_next_resolver(previous)
             previous = resolver
-        self._resolver: BaseDependencyResolver = previous
-        self._path_lookup = path_lookup
+        return previous
 
     def resolve_notebook(self, path_lookup: PathLookup, path: Path) -> MaybeDependency:
-        return self._resolver.resolve_notebook(path_lookup, path)
-
-    def resolve_local_file(self, path_lookup: PathLookup, path: Path) -> MaybeDependency:
-        return self._resolver.resolve_local_file(path_lookup, path)
+        return self._notebook_resolver.resolve_notebook(path_lookup, path)
 
     def resolve_import(self, path_lookup: PathLookup, name: str) -> MaybeDependency:
-        return self._resolver.resolve_import(path_lookup, name)
+        return self._import_resolver.resolve_import(path_lookup, name)
+
+    def resolve_library(self, path_lookup: PathLookup, library: str) -> MaybeDependency:
+        return self._library_resolver.resolve_library(path_lookup, Path(library))
 
     def build_local_file_dependency_graph(self, path: Path) -> MaybeGraph:
         """Builds a dependency graph starting from a file. This method is mainly intended for testing purposes.
         In case of problems, the paths in the problems will be relative to the starting path lookup."""
-        maybe = self._resolver.resolve_local_file(self._path_lookup, path)
+        resolver = self._local_file_resolver
+        if not resolver:
+            problem = DependencyProblem("missing-file-resolver", "Missing resolver for local files")
+            return MaybeGraph(None, [problem])
+        maybe = resolver.resolve_local_file(self._path_lookup, path)
         if not maybe.dependency:
             return MaybeGraph(None, self._make_relative_paths(maybe.problems, path))
         graph = DependencyGraph(maybe.dependency, None, self, self._path_lookup)
         container = maybe.dependency.load(graph.path_lookup)
-        if container is not None:
-            problems = container.build_dependency_graph(graph)
-            if problems:
-                return MaybeGraph(None, self._make_relative_paths(problems, path))
-        return MaybeGraph(graph, [])
+        if container is None:
+            problem = DependencyProblem('cannot-load-file', f"Could not load file {path}")
+            return MaybeGraph(None, [problem])
+        problems = container.build_dependency_graph(graph)
+        if problems:
+            problems = self._make_relative_paths(problems, path)
+        return MaybeGraph(graph, problems)
+
+    @property
+    def _local_file_resolver(self) -> BaseFileResolver | None:
+        if isinstance(self._import_resolver, BaseFileResolver):
+            return self._import_resolver
+        return None
 
     def build_notebook_dependency_graph(self, path: Path) -> MaybeGraph:
         """Builds a dependency graph starting from a notebook. This method is mainly intended for testing purposes.
         In case of problems, the paths in the problems will be relative to the starting path lookup."""
-        maybe = self._resolver.resolve_notebook(self._path_lookup, path)
+        maybe = self._notebook_resolver.resolve_notebook(self._path_lookup, path)
         if not maybe.dependency:
             return MaybeGraph(None, self._make_relative_paths(maybe.problems, path))
         graph = DependencyGraph(maybe.dependency, None, self, self._path_lookup)
         container = maybe.dependency.load(graph.path_lookup)
-        if container is not None:
-            problems = container.build_dependency_graph(graph)
-            if problems:
-                return MaybeGraph(None, self._make_relative_paths(problems, path))
-        return MaybeGraph(graph, [])
+        if container is None:
+            problem = DependencyProblem('cannot-load-notebook', f"Could not load notebook {path}")
+            return MaybeGraph(None, [problem])
+        problems = container.build_dependency_graph(graph)
+        if problems:
+            problems = self._make_relative_paths(problems, path)
+        return MaybeGraph(graph, problems)
 
     def _make_relative_paths(self, problems: list[DependencyProblem], path: Path) -> list[DependencyProblem]:
         adjusted_problems = []
         for problem in problems:
             out_path = path if problem.is_path_missing() else problem.source_path
             if out_path.is_absolute() and out_path.is_relative_to(self._path_lookup.cwd):
                 out_path = out_path.relative_to(self._path_lookup.cwd)
             adjusted_problems.append(problem.replace(source_path=out_path))
         return adjusted_problems
 
+    def build_library_dependency_graph(self, path: Path):
+        """Builds a dependency graph starting from a library. This method is mainly intended for testing purposes.
+        In case of problems, the paths in the problems will be relative to the starting path lookup."""
+        maybe = self._library_resolver.resolve_library(self._path_lookup, path)
+        if not maybe.dependency:
+            return MaybeGraph(None, self._make_relative_paths(maybe.problems, path))
+        graph = DependencyGraph(maybe.dependency, None, self, self._path_lookup)
+        container = maybe.dependency.load(graph.path_lookup)
+        if container is None:
+            problem = DependencyProblem('cannot-load-library', f"Could not load library {path}")
+            return MaybeGraph(None, [problem])
+        problems = container.build_dependency_graph(graph)
+        if problems:
+            problems = self._make_relative_paths(problems, path)
+        return MaybeGraph(graph, problems)
+
     def __repr__(self):
-        return f"<DependencyResolver {self._resolver} {self._path_lookup}>"
+        return f"<DependencyResolver {self._notebook_resolver} {self._import_resolver} {self._path_lookup}>"
 
 
 MISSING_SOURCE_PATH = "<MISSING_SOURCE_PATH>"
 
 
 @dataclass
 class DependencyProblem:
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/jobs.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/jobs.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 from pathlib import Path
 
 from databricks.labs.blueprint.parallel import Threads
 from databricks.labs.lsql.backends import SqlBackend
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors import NotFound
 from databricks.sdk.service import compute, jobs
+from databricks.sdk.service.workspace import ExportFormat
 
 from databricks.labs.ucx.hive_metastore.migration_status import MigrationIndex
 from databricks.labs.ucx.mixins.wspath import WorkspacePath
 from databricks.labs.ucx.source_code.base import CurrentSessionState
 from databricks.labs.ucx.source_code.files import LocalFile
 from databricks.labs.ucx.source_code.graph import (
+    Dependency,
     DependencyGraph,
-    SourceContainer,
     DependencyProblem,
-    Dependency,
-    WrappingLoader,
     DependencyResolver,
+    SourceContainer,
+    WrappingLoader,
 )
 from databricks.labs.ucx.source_code.languages import Languages
 from databricks.labs.ucx.source_code.notebooks.sources import Notebook, NotebookLinter, FileLinter
 from databricks.labs.ucx.source_code.path_lookup import PathLookup
 
 logger = logging.getLogger(__name__)
 
@@ -38,14 +39,18 @@
     code: str
     message: str
     start_line: int
     start_col: int
     end_line: int
     end_col: int
 
+    def as_message(self) -> str:
+        message = f"{self.path}:{self.start_line} [{self.code}] {self.message}"
+        return message
+
 
 class WorkflowTask(Dependency):
     def __init__(self, ws: WorkspaceClient, task: jobs.Task, job: jobs.Job):
         loader = WrappingLoader(WorkflowTaskContainer(ws, task))
         super().__init__(loader, Path(f'/jobs/{task.task_key}'))
         self._task = task
         self._job = job
@@ -72,50 +77,54 @@
         yield from self._register_python_wheel_task(graph)
         yield from self._register_spark_jar_task(graph)
         yield from self._register_run_job_task(graph)
         yield from self._register_pipeline_task(graph)
         yield from self._register_existing_cluster_id(graph)
         yield from self._register_spark_submit_task(graph)
 
-    def _register_libraries(self, graph: DependencyGraph):
+    def _register_libraries(self, graph: DependencyGraph) -> Iterable[DependencyProblem]:
         if not self._task.libraries:
             return
         for library in self._task.libraries:
-            yield from self._lint_library(library, graph)
+            yield from self._register_library(graph, library)
 
-    def _lint_library(self, library: compute.Library, graph: DependencyGraph) -> Iterable[DependencyProblem]:
+    def _register_library(self, graph: DependencyGraph, library: compute.Library) -> Iterable[DependencyProblem]:
         if library.pypi:
-            # TODO: https://github.com/databrickslabs/ucx/issues/1642
-            maybe = graph.register_library(library.pypi.package)
-            if maybe.problems:
-                yield from maybe.problems
-        if library.jar:
-            # TODO: https://github.com/databrickslabs/ucx/issues/1641
-            yield DependencyProblem('not-yet-implemented', 'Jar library is not yet implemented')
+            problems = graph.register_library(library.pypi.package)
+            if problems:
+                yield from problems
         if library.egg:
             # TODO: https://github.com/databrickslabs/ucx/issues/1643
-            maybe = graph.register_library(library.egg)
-            if maybe.problems:
-                yield from maybe.problems
+            yield DependencyProblem("not-yet-implemented", "Egg library is not yet implemented")
         if library.whl:
             # TODO: download the wheel somewhere local and add it to "virtual sys.path" via graph.path_lookup.push_path
             # TODO: https://github.com/databrickslabs/ucx/issues/1640
-            maybe = graph.register_library(library.whl)
-            if maybe.problems:
-                yield from maybe.problems
-        if library.requirements:
-            # TODO: download and add every entry via graph.register_library
-            # TODO: https://github.com/databrickslabs/ucx/issues/1644
-            yield DependencyProblem('not-yet-implemented', 'Requirements library is not yet implemented')
+            yield DependencyProblem("not-yet-implemented", "Wheel library is not yet implemented")
+        if library.requirements:  # https://pip.pypa.io/en/stable/reference/requirements-file-format/
+            logger.info(f"Registering libraries from {library.requirements}")
+            with self._ws.workspace.download(library.requirements, format=ExportFormat.AUTO) as remote_file:
+                contents = remote_file.read().decode()
+                for requirement in contents.splitlines():
+                    clean_requirement = requirement.replace(" ", "")  # requirements.txt may contain spaces
+                    if clean_requirement.startswith("-r"):
+                        logger.warning(f"References to other requirements file is not supported: {requirement}")
+                        continue
+                    if clean_requirement.startswith("-c"):
+                        logger.warning(f"References to constrains file is not supported: {requirement}")
+                        continue
+                    yield from graph.register_library(clean_requirement)
+        if library.jar:
+            # TODO: https://github.com/databrickslabs/ucx/issues/1641
+            yield DependencyProblem('not-yet-implemented', 'Jar library is not yet implemented')
 
     def _register_notebook(self, graph: DependencyGraph) -> Iterable[DependencyProblem]:
         if not self._task.notebook_task:
             return []
         notebook_path = self._task.notebook_task.notebook_path
-        logger.info(f'Disovering {self._task.task_key} entrypoint: {notebook_path}')
+        logger.info(f'Discovering {self._task.task_key} entrypoint: {notebook_path}')
         path = WorkspacePath(self._ws, notebook_path)
         return graph.register_notebook(path)
 
     def _register_spark_python_task(self, graph: DependencyGraph):  # pylint: disable=unused-argument
         if not self._task.spark_python_task:
             return
         # TODO: https://github.com/databrickslabs/ucx/issues/1639
@@ -169,29 +178,38 @@
         self._ws = ws
         self._resolver = resolver
         self._path_lookup = path_lookup
         self._migration_index = migration_index
 
     def refresh_report(self, sql_backend: SqlBackend, inventory_database: str):
         tasks = []
-        for job in self._ws.jobs.list():
+        all_jobs = list(self._ws.jobs.list())
+        logger.info(f"Preparing {len(all_jobs)} linting jobs...")
+        for job in all_jobs:
             tasks.append(functools.partial(self.lint_job, job.job_id))
         problems: list[JobProblem] = []
+        logger.info(f"Running {tasks} linting tasks in parallel...")
         for batch in Threads.strict('linting workflows', tasks):
             problems.extend(batch)
+        logger.info(f"Saving {len(problems)} linting problems...")
         sql_backend.save_table(f'{inventory_database}.workflow_problems', problems, JobProblem, mode='overwrite')
 
     def lint_job(self, job_id: int) -> list[JobProblem]:
         try:
             job = self._ws.jobs.get(job_id)
-            return list(self._lint_job(job))
         except NotFound:
             logger.warning(f'Could not find job: {job_id}')
             return []
 
+        problems = self._lint_job(job)
+        if len(problems) > 0:
+            problem_messages = "\n".join([problem.as_message() for problem in problems])
+            logger.warning(f"Found job problems:\n{problem_messages}")
+        return problems
+
     _UNKNOWN = Path('<UNKNOWN>')
 
     def _lint_job(self, job: jobs.Job) -> list[JobProblem]:
         problems: list[JobProblem] = []
         assert job.job_id is not None
         assert job.settings is not None
         assert job.settings.name is not None
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/languages.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/languages.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/lsp.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/lsp.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/path_lookup.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/path_lookup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import logging
 import sys
 from pathlib import Path
 
+
 logger = logging.getLogger(__name__)
 
 
 class PathLookup:
 
     @classmethod
     def from_pathlike_string(cls, cwd: Path, syspath: str):
@@ -23,20 +24,22 @@
         self._sys_paths = sys_paths
 
     def change_directory(self, new_working_directory: Path) -> PathLookup:
         return PathLookup(new_working_directory, self._sys_paths)
 
     def resolve(self, path: Path) -> Path | None:
         if path.is_absolute() and path.exists():
-            return path
+            # eliminate “..” components
+            return path.resolve()
         for parent in self.paths:
             absolute_path = parent / path
             try:
                 if absolute_path.exists():
-                    return absolute_path
+                    # eliminate “..” components
+                    return absolute_path.resolve()
             except PermissionError:
                 logger.warning(f"Permission denied to access {absolute_path}")
         return None
 
     def has_path(self, path: Path):
         return next(p for p in self._sys_paths if path == p) is not None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/pyspark.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/pyspark.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,25 +29,24 @@
             isinstance(node, ast.Call)
             and isinstance(node.func, ast.Attribute)
             and self._get_table_arg(node) is not None
         )
 
     @abstractmethod
     def lint(self, from_table: FromTable, index: MigrationIndex, node: ast.Call) -> Iterator[Advice]:
-        raise NotImplementedError()
+        """raises Advices by linting the code"""
 
     @abstractmethod
     def apply(self, from_table: FromTable, index: MigrationIndex, node: ast.Call) -> None:
-        raise NotImplementedError()
+        """applies recommendations"""
 
     def _get_table_arg(self, node: ast.Call):
         if len(node.args) > 0:
             return node.args[self.table_arg_index] if self.min_args <= len(node.args) <= self.max_args else None
-        assert self.table_arg_name is not None
-        if not node.keywords:
+        if not self.table_arg_name or not node.keywords:
             return None
         arg = next(kw for kw in node.keywords if kw.arg == self.table_arg_name)
         return arg.value if arg is not None else None
 
     def _check_call_context(self, node: ast.Call) -> bool:
         assert isinstance(node.func, ast.Attribute)  # Avoid linter warning
         func_name = node.func.attr
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/python_linter.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/python_linter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import abc
 import ast
 import logging
-from collections.abc import Iterable
+from collections.abc import Iterable, Callable
 from typing import TypeVar, Generic, cast
 
 from databricks.labs.ucx.source_code.base import Linter, Advice, Advisory
 
 logger = logging.getLogger(__name__)
 
 
@@ -266,14 +266,17 @@
     def get_constant_path(self) -> str | None:
         path = PythonLinter.get_dbutils_notebook_run_path_arg(cast(ast.Call, self.node))
         if isinstance(path, ast.Constant):
             return path.value.strip().strip("'").strip('"')
         return None
 
 
+P = TypeVar("P", bound=Callable)
+
+
 class PythonLinter(Linter):
 
     def lint(self, code: str) -> Iterable[Advice]:
         linter = ASTLinter.parse(code)
         nodes = self.list_dbutils_notebook_run_calls(linter)
         return [self._convert_dbutils_notebook_run_to_advice(node.node) for node in nodes]
 
@@ -308,26 +311,38 @@
 
     @staticmethod
     def list_dbutils_notebook_run_calls(linter: ASTLinter) -> list[NotebookRunCall]:
         calls = linter.locate(ast.Call, [("run", ast.Attribute), ("notebook", ast.Attribute), ("dbutils", ast.Name)])
         return [NotebookRunCall(call) for call in calls]
 
     @staticmethod
-    def list_import_sources(linter: ASTLinter) -> list[ImportSource]:
-        # TODO: make this code more robust, because it fails detecting imports on UCX codebase
+    def list_import_sources(linter: ASTLinter, problem_type: P) -> tuple[list[ImportSource], list[P]]:
+        problems: list[P] = []
         try:  # pylint: disable=too-many-try-statements
             nodes = linter.locate(ast.Import, [])
             sources = [ImportSource(node, alias.name) for node in nodes for alias in node.names]
             nodes = linter.locate(ast.ImportFrom, [])
             sources.extend(ImportSource(node, node.module) for node in nodes)
             nodes = linter.locate(ast.Call, [("import_module", ast.Attribute), ("importlib", ast.Name)])
-            sources.extend(ImportSource(node, node.args[0].value) for node in nodes)
-            nodes = linter.locate(ast.Call, [("__import__", ast.Attribute), ("importlib", ast.Name)])
-            sources.extend(ImportSource(node, node.args[0].value) for node in nodes)
-            return sources
+            nodes.extend(linter.locate(ast.Call, [("__import__", ast.Attribute), ("importlib", ast.Name)]))
+            for node in nodes:
+                if isinstance(node.args[0], ast.Constant):
+                    sources.append(ImportSource(node, node.args[0].value))
+                    continue
+                problem = problem_type(
+                    'dependency-not-constant',
+                    "Can't check dependency not provided as a constant",
+                    start_line=node.lineno,
+                    start_col=node.col_offset,
+                    end_line=node.end_lineno or 0,
+                    end_col=node.end_col_offset or 0,
+                )
+                problems.append(problem)
+            return sources, problems
         except Exception as e:  # pylint: disable=broad-except
-            logger.warning(f"{linter} imports: {e}")
-            return []
+            problem = problem_type('internal-error', f"While linter {linter} was checking imports: {e}")
+            problems.append(problem)
+            return [], problems
 
     @staticmethod
     def list_sys_path_changes(linter: ASTLinter) -> list[SysPathChange]:
         return linter.collect_sys_paths_changes()
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/queries.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/queries.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/redash.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/redash.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/spark_connect.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/spark_connect.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/table_creation.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/table_creation.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/whitelist.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/whitelist.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,51 +5,24 @@
 import sys
 from dataclasses import dataclass, field
 from enum import Enum
 from collections.abc import Iterable
 
 from yaml import load_all as load_yaml, Loader
 
-from databricks.labs.ucx.source_code.path_lookup import PathLookup
 
 from databricks.labs.ucx.source_code.graph import (
-    SourceContainer,
     DependencyGraph,
-    BaseDependencyResolver,
     DependencyProblem,
-    MaybeDependency,
+    SourceContainer,
 )
 
 logger = logging.getLogger(__name__)
 
 
-class WhitelistResolver(BaseDependencyResolver):
-
-    def __init__(self, whitelist: Whitelist, next_resolver: BaseDependencyResolver | None = None):
-        super().__init__(next_resolver)
-        self._whitelist = whitelist
-
-    def with_next_resolver(self, resolver: BaseDependencyResolver) -> BaseDependencyResolver:
-        return WhitelistResolver(self._whitelist, resolver)
-
-    def resolve_import(self, path_lookup: PathLookup, name: str) -> MaybeDependency:
-        # TODO attach compatibility to dependency, see https://github.com/databrickslabs/ucx/issues/1382
-        compatibility = self._whitelist.compatibility(name)
-        if compatibility == UCCompatibility.FULL:
-            return MaybeDependency(None, [])
-        if compatibility == UCCompatibility.NONE:
-            # TODO move to linter, see https://github.com/databrickslabs/ucx/issues/1527
-            problem = DependencyProblem("dependency-check", f"Use of dependency {name} is deprecated")
-            return MaybeDependency(None, [problem])
-        if compatibility == UCCompatibility.PARTIAL:
-            problem = DependencyProblem("dependency-check", f"Package {name} is only partially supported by UC")
-            return MaybeDependency(None, [problem])
-        return super().resolve_import(path_lookup, name)
-
-
 class StubContainer(SourceContainer):
 
     def build_dependency_graph(self, parent: DependencyGraph) -> list[DependencyProblem]:
         return []
 
 
 class UCCompatibility(Enum):
@@ -78,15 +51,15 @@
 @dataclass
 class KnownPackage(abc.ABC):
     identifier: Identifier
     top_level: str
 
     @abc.abstractmethod
     def compatibility_of(self, name: str) -> UCCompatibility:
-        raise NotImplementedError()
+        """returns the compatibility of a symbol"""
 
 
 @dataclass
 class PythonBuiltinPackage(KnownPackage):
 
     def compatibility_of(self, name: str) -> UCCompatibility:
         return UCCompatibility.FULL
@@ -127,46 +100,49 @@
                 return UCCompatibility.NONE
             name = ".".join(parts[0:-1])
         return UCCompatibility.NONE
 
 
 class Whitelist:
     @classmethod
-    def parse(cls, data: str):
+    def parse(cls, data: str, use_defaults=True):
         yamls = load_yaml(data, Loader=Loader)
         # @dataclass(kw_only=True) fails to convert inner structs, so deserialize manually
         pips: list[PipPackage] = []
         for yaml in yamls:
             identifier = Identifier(**yaml['identifier'])
             top_level = yaml['top_level']
             packages = {p.name: p for p in [PythonPackage(**package) for package in yaml['packages']]}
             pips.append(PipPackage(identifier, top_level, packages))
-        return Whitelist(pips)
+        return Whitelist(use_defaults, pips)
 
-    def __init__(self, pips: Iterable[PipPackage] | None = None):
+    def __init__(self, use_defaults=True, pips: Iterable[PipPackage] | None = None):
         python_version = sys.version
         known_packages: list[KnownPackage] = [
             PythonBuiltinPackage(Identifier(**{"name": name, "version": python_version}), name)
             for name in sys.stdlib_module_names
         ]
+        if use_defaults:
+            # default white list
+            known_packages.extend(
+                [
+                    PipPackage.compatible("click"),
+                    PipPackage.compatible("databricks"),
+                    PipPackage.compatible("google"),
+                    PipPackage.compatible("pandas"),
+                    PipPackage.compatible("pytest"),
+                    PipPackage.compatible("requests"),
+                    PipPackage.compatible("sqlglot"),
+                    PipPackage.compatible("urllib3"),
+                    PipPackage.compatible("yaml"),
+                ]
+            )
         if pips is not None:
             known_packages.extend(pips)
-        known_packages.extend(
-            [
-                PipPackage.compatible("click"),
-                PipPackage.compatible("databricks"),
-                PipPackage.compatible("google"),
-                PipPackage.compatible("pandas"),
-                PipPackage.compatible("pytest"),
-                PipPackage.compatible("requests"),
-                PipPackage.compatible("sqlglot"),
-                PipPackage.compatible("urllib3"),
-                PipPackage.compatible("yaml"),
-            ]
-        )
+
         self._known_packages: dict[str, list[KnownPackage]] = {}
         for known in known_packages:
             top_levels: list[str] = known.top_level if isinstance(known.top_level, list) else [known.top_level]
             for top_level in top_levels:
                 packs = self._known_packages.get(top_level, None)
                 if packs is None:
                     packs = []
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/notebooks/cells.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/notebooks/cells.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import logging
+import re
 from abc import ABC, abstractmethod
 from ast import parse as parse_python
 from enum import Enum
 from pathlib import Path
 from sqlglot import parse as parse_sql, ParseError as SQLParseError
 
 from databricks.sdk.service.workspace import Language
@@ -43,19 +44,19 @@
     @migrated_code.setter
     def migrated_code(self, value: str):
         self._migrated_code = value
 
     @property
     @abstractmethod
     def language(self) -> CellLanguage:
-        raise NotImplementedError()
+        """returns the language of this cell"""
 
     @abstractmethod
     def is_runnable(self) -> bool:
-        raise NotImplementedError()
+        """whether of not this cell can be run"""
 
     def build_dependency_graph(self, _: DependencyGraph) -> list[DependencyProblem]:
         return []
 
     def __repr__(self):
         return f"{self.language.name}: {self._original_code[:20]}"
 
@@ -178,17 +179,24 @@
     @property
     def language(self):
         return CellLanguage.PIP
 
     def is_runnable(self) -> bool:
         return True  # TODO
 
-    def build_dependency_graph(self, _: DependencyGraph) -> list[DependencyProblem]:
-        # TODO: https://github.com/databrickslabs/ucx/issues/1642
-        return []
+    def build_dependency_graph(self, graph: DependencyGraph) -> list[DependencyProblem]:
+        # TODO: this is very basic code, we need to improve it
+        splits = re.split(r" |\n", self.original_code)
+        if len(splits) < 3:
+            return [DependencyProblem("library-install-failed", f"Missing arguments in '{self.original_code}'")]
+        if splits[1] != "install":
+            return [DependencyProblem("library-install-failed", f"Unsupported %pip command: {splits[1]}")]
+        # TODO: we need to support different formats of the library name and etc
+        library = splits[2]
+        return graph.register_library(library)
 
 
 class CellLanguage(Enum):
     # long magic_names must come first to avoid shorter ones being matched
     PYTHON = Language.PYTHON, 'python', '#', True, PythonCell
     SCALA = Language.SCALA, 'scala', '//', True, ScalaCell
     SQL = Language.SQL, 'sql', '--', True, SQLCell
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/notebooks/loaders.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/notebooks/loaders.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,40 +3,37 @@
 import abc
 import logging
 from pathlib import Path
 
 from databricks.sdk.errors import NotFound
 
 from databricks.labs.ucx.source_code.graph import (
-    BaseDependencyResolver,
+    BaseNotebookResolver,
     Dependency,
     DependencyLoader,
-    SourceContainer,
     MaybeDependency,
+    SourceContainer,
 )
 from databricks.labs.ucx.source_code.notebooks.cells import CellLanguage
 from databricks.labs.ucx.source_code.notebooks.sources import Notebook
 from databricks.labs.ucx.source_code.path_lookup import PathLookup
 
 logger = logging.getLogger(__name__)
 
 
-class NotebookResolver(BaseDependencyResolver):
+class NotebookResolver(BaseNotebookResolver):
 
-    def __init__(self, notebook_loader: NotebookLoader, next_resolver: BaseDependencyResolver | None = None):
-        super().__init__(next_resolver)
+    def __init__(self, notebook_loader: NotebookLoader):
+        super().__init__()
         self._notebook_loader = notebook_loader
 
-    def with_next_resolver(self, resolver: BaseDependencyResolver) -> BaseDependencyResolver:
-        return NotebookResolver(self._notebook_loader, resolver)
-
     def resolve_notebook(self, path_lookup: PathLookup, path: Path) -> MaybeDependency:
         absolute_path = self._notebook_loader.resolve(path_lookup, path)
         if not absolute_path:
-            return super().resolve_notebook(path_lookup, path)
+            return self._fail('notebook-not-found', f"Notebook not found: {path.as_posix()}")
         dependency = Dependency(self._notebook_loader, absolute_path)
         return MaybeDependency(dependency, [])
 
 
 class NotebookLoader(DependencyLoader, abc.ABC):
     def resolve(self, path_lookup: PathLookup, path: Path) -> Path | None:
         """When exported through Git, notebooks are saved with a .py extension. If the path is a notebook, return the
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/notebooks/migrator.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/notebooks/migrator.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/notebooks/sources.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/source_code/notebooks/sources.py`

 * *Files 15% similar despite different names*

```diff
@@ -100,51 +100,104 @@
                 )
 
     @staticmethod
     def name() -> str:
         return "notebook-linter"
 
 
+SUPPORTED_EXTENSION_LANGUAGES = {
+    '.py': Language.PYTHON,
+    '.sql': Language.SQL,
+}
+
+
 class FileLinter:
-    _EXT = {
-        '.py': Language.PYTHON,
-        '.sql': Language.SQL,
+    _NOT_YET_SUPPORTED_SUFFIXES = {
+        '.scala',
+        '.sh',
+        '.r',
+    }
+    _IGNORED_SUFFIXES = {
+        '.json',
+        '.md',
+        '.txt',
+        '.xml',
+        '.yml',
+        '.toml',
+        '.cfg',
+        '.bmp',
+        '.gif',
+        '.png',
+        '.tif',
+        '.tiff',
+        '.svg',
+        '.jpg',
+        '.jpeg',
+        '.pyc',
+        '.whl',
+        '.egg',
+        '.class',
+        '.iml',
+        '.gz',
+    }
+    _IGNORED_NAMES = {
+        '.ds_store',
+        '.gitignore',
+        '.coverage',
+        'license',
+        'codeowners',
+        'makefile',
+        'pkg-info',
+        'metadata',
+        'wheel',
+        'record',
+        'notice',
+        'zip-safe',
     }
 
-    def __init__(self, langs: Languages, path: Path):
+    def __init__(self, langs: Languages, path: Path, content: str | None = None):
         self._languages: Languages = langs
         self._path: Path = path
+        self._content = content
 
     @cached_property
-    def _content(self) -> str:
-        return self._path.read_text()
+    def _source_code(self) -> str:
+        return self._path.read_text() if self._content is None else self._content
 
     def _file_language(self):
-        return self._EXT.get(self._path.suffix)
+        return SUPPORTED_EXTENSION_LANGUAGES.get(self._path.suffix.lower())
 
     def _is_notebook(self):
         language = self._file_language()
         if not language:
             return False
-        cell_language = CellLanguage.of_language(language)
-        return self._content.startswith(cell_language.file_magic_header)
+        return self._source_code.startswith(CellLanguage.of_language(language).file_magic_header)
 
     def lint(self) -> Iterable[Advice]:
         if self._is_notebook():
             yield from self._lint_notebook()
         else:
             yield from self._lint_file()
 
     def _lint_file(self):
         language = self._file_language()
         if not language:
-            yield Failure("unsupported-language", f"Cannot detect language for {self._path}", 0, 0, 1, 1)
-        try:
-            linter = self._languages.linter(language)
-            yield from linter.lint(self._content)
-        except ValueError as err:
-            yield Failure("unsupported-language", str(err), 0, 0, 1, 1)
+            suffix = self._path.suffix.lower()
+            if suffix in self._IGNORED_SUFFIXES or self._path.name.lower() in self._IGNORED_NAMES:
+                yield from []
+            elif suffix in self._NOT_YET_SUPPORTED_SUFFIXES:
+                yield Failure("unsupported-language", f"Language not supported yet for {self._path}", 0, 0, 1, 1)
+            else:
+                yield Failure("unknown-language", f"Cannot detect language for {self._path}", 0, 0, 1, 1)
+        else:
+            try:
+                linter = self._languages.linter(language)
+                yield from linter.lint(self._source_code)
+            except ValueError as err:
+                yield Failure(
+                    "unsupported-content", f"Error while parsing content of {self._path.as_posix()}: {err}", 0, 0, 1, 1
+                )
 
     def _lint_notebook(self):
-        notebook = Notebook.parse(self._path, self._content, self._file_language())
+        notebook = Notebook.parse(self._path, self._source_code, self._file_language())
         notebook_linter = NotebookLinter(self._languages, notebook)
         yield from notebook_linter.lint()
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/upgrades/v0.15.0_added_cluster_policy.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/upgrades/v0.15.0_added_cluster_policy.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/upgrades/v0.16.0_changing_cluster_table_schema.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/upgrades/v0.16.0_changing_cluster_table_schema.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/upgrades/v0.20.0_add_is_partitioned_column.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/upgrades/v0.20.0_add_is_partitioned_column.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/upgrades/v0.23.0_add_assessment_to_udf.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/upgrades/v0.23.0_add_assessment_to_udf.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/base.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/workspace_access/base.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/clusters.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/workspace_access/clusters.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,14 @@
                     autotermination_minutes=cluster.autotermination_minutes,
                     custom_tags=cluster.custom_tags,
                     init_scripts=cluster.init_scripts,
                     cluster_log_conf=cluster.cluster_log_conf,
                     aws_attributes=cluster.aws_attributes,
                     ssh_public_keys=cluster.ssh_public_keys,
                     enable_elastic_disk=cluster.enable_elastic_disk,
-                    cluster_source=cluster.cluster_source,
                     instance_pool_id=cluster.instance_pool_id,
                     enable_local_disk_encryption=cluster.enable_local_disk_encryption,
                     driver_instance_pool_id=cluster.driver_instance_pool_id,
                 )
             except InvalidParameterValue as e:
                 logger.warning(f"skipping cluster remapping: {e}")
 
@@ -101,14 +100,13 @@
                     autotermination_minutes=cluster_details.autotermination_minutes,
                     custom_tags=cluster_details.custom_tags,
                     init_scripts=cluster_details.init_scripts,
                     cluster_log_conf=cluster_details.cluster_log_conf,
                     aws_attributes=cluster_details.aws_attributes,
                     ssh_public_keys=cluster_details.ssh_public_keys,
                     enable_elastic_disk=cluster_details.enable_elastic_disk,
-                    cluster_source=cluster_details.cluster_source,
                     instance_pool_id=cluster_details.instance_pool_id,
                     enable_local_disk_encryption=cluster_details.enable_local_disk_encryption,
                     driver_instance_pool_id=cluster_details.driver_instance_pool_id,
                 )
             except InvalidParameterValue as e:
                 logger.warning(f"skipping cluster remapping: {e}")
```

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/generic.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/workspace_access/generic.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/groups.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/workspace_access/groups.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/listing.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/workspace_access/listing.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/manager.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/workspace_access/manager.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/redash.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/workspace_access/redash.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/scim.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/workspace_access/scim.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/secrets.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/workspace_access/secrets.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/tacl.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/workspace_access/tacl.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/workflows.py` & `databricks_labs_ucx-0.24.0/databricks/labs/ucx/workspace_access/workflows.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/.gitignore` & `databricks_labs_ucx-0.24.0/.gitignore`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/LICENSE` & `databricks_labs_ucx-0.24.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/NOTICE` & `databricks_labs_ucx-0.24.0/NOTICE`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.1/README.md` & `databricks_labs_ucx-0.24.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,17 @@
   * [Assessment workflow](#assessment-workflow)
   * [Group migration workflow](#group-migration-workflow)
   * [Debug notebook](#debug-notebook)
   * [Debug logs](#debug-logs)
   * [Table Migration Workflow](#table-migration-workflow)
     * [Dependency CLI commands](#dependency-cli-commands)
     * [Table Migration Workflow Tasks](#table-migration-workflow-tasks)
+    * [Post Migration Data Reconciliation Task](#post-migration-data-reconciliation-task)
     * [Other considerations](#other-considerations)
+  * [Jobs Static Code Analysis Workflow](#jobs-static-code-analysis-workflow)
 * [Utility commands](#utility-commands)
   * [`logs` command](#logs-command)
   * [`ensure-assessment-run` command](#ensure-assessment-run-command)
   * [`repair-run` command](#repair-run-command)
   * [`workflows` command](#workflows-command)
   * [`open-remote-config` command](#open-remote-config-command)
   * [`installations` command](#installations-command)
@@ -62,14 +64,15 @@
   * [`skip` command](#skip-command)
   * [`create-catalogs-schemas` command](#create-catalogs-schemas-command)
   * [`migrate-tables` command](#migrate-tables-command)
   * [`revert-migrated-tables` command](#revert-migrated-tables-command)
   * [`move` command](#move-command)
   * [`alias` command](#alias-command)
 * [Code migration commands](#code-migration-commands)
+  * [`lint-local-code` command](#lint-local-code-command)
   * [`migrate-local-code` command](#migrate-local-code-command)
   * [`migrate-dbsql-dashboards` command](#migrate-dbsql-dashboards-command)
   * [`revert-dbsql-dashboards` command](#revert-dbsql-dashboards-command)
 * [Cross-workspace installations](#cross-workspace-installations)
   * [`sync-workspace-info` command](#sync-workspace-info-command)
   * [`manual-workspace-info` command](#manual-workspace-info-command)
   * [`create-account-groups` command](#create-account-groups-command)
@@ -80,14 +83,15 @@
 * [Project Support](#project-support)
 <!-- TOC -->
 
 # Installation
 
 - Databricks CLI v0.213 or later. See [instructions](#authenticate-databricks-cli). 
 - Python 3.10 or later. See [Windows](https://www.python.org/downloads/windows/) instructions.
+- Databricks Premium or Enterprise workspace.
 - Network access to your Databricks Workspace used for the [installation process](#install-ucx).
 - Network access to the Internet for [pypi.org](https://pypi.org) and [github.com](https://github.com) from machine running the installation.
 - Databricks Workspace Administrator privileges for the user, that runs the installation. Running UCX as a Service Principal is not supported.
 - Account level Identity Setup. See instructions for [AWS](https://docs.databricks.com/en/administration-guide/users-groups/best-practices.html), [Azure](https://learn.microsoft.com/en-us/azure/databricks/administration-guide/users-groups/best-practices), and [GCP](https://docs.gcp.databricks.com/administration-guide/users-groups/best-practices.html).
 - Unity Catalog Metastore Created (per region). See instructions for [AWS](https://docs.databricks.com/en/data-governance/unity-catalog/create-metastore.html), [Azure](https://learn.microsoft.com/en-us/azure/databricks/data-governance/unity-catalog/create-metastore), and [GCP](https://docs.gcp.databricks.com/data-governance/unity-catalog/create-metastore.html).
 - If your Databricks Workspace relies on an external Hive Metastore (such as AWS Glue), make sure to read [this guide](docs/external_hms_glue.md).
 - Databricks Workspace has to have network access to [pypi.org](https://pypi.org) to download `databricks-sdk`, `databricks-labs-lsql`, `databricks-labs-blueprint`, `sqlglot` and `pyyaml` packages.
@@ -139,14 +143,17 @@
 The [`WorkspaceInstallation`](src/databricks/labs/ucx/install.py) manages the installation and uninstallation of UCX in a workspace. It handles 
 the configuration and exception management during the installation process. The installation process creates dashboards, databases, and jobs. 
 It also includes the creation of a database with given configuration and the deployment of workflows with specific settings. The installation 
 process can handle exceptions and infer errors from job runs and task runs. The workspace installation uploads wheels, creates cluster policies, 
 and wheel runners to the workspace. It can also handle the creation of job tasks for a given task, such as job dashboard tasks, job notebook tasks, 
 and job wheel tasks. The class handles the installation of UCX, including configuring the workspace, installing necessary libraries, and verifying 
 the installation, making it easier for users to migrate their workspaces to UCX.
+At the end of the installation, the user will be prompted if the current installation needs to join an existing collection (create new collection if none present).
+For large organization with many workspaces, grouping workspaces into collection helps in managing UCX migration at collection level (instead of workspaces level)
+User should be an account admin to be able to join a collection.
 
 After this, UCX will be installed locally and a number of assets will be deployed in the selected workspace. 
 These assets are available under the installation folder, i.e. `/Users/<your user>/.ucx/`.
 
 You can also install a specific version by specifying it like `@v0.13.2` - `databricks labs install ucx@v0.13.2`.
 
 ![macos_install_ucx](docs/macos_2_databrickslabsmac_installucx.gif)
@@ -451,22 +458,71 @@
   - `migrate_external_tables_sync` - Migrate external tables using [`SYNC`](https://docs.databricks.com/en/sql/language-manual/sql-ref-syntax-aux-sync.html) command. This does not create copy of the tables.
 - `migrate-external-hiveserde-tables-in-place-experimental` - Experimental in-place migration of HiveSerde tables. HiveSerDe tables include ParquetHiveSerDe, OrcSerde, AvroSerDe, LazySimpleSerDe, JsonSerDe, OpenCSVSerde tables.
   - `migrate_external_hiveserde_tables_in_place_experimental` - Migrate HiveSerde tables in place.
 - Following workflows/tasks are on the roadmap and being developed:
   - Migrate tables using CTAS 
   - Experimentally migrate Delta and Parquet data found in dbfs mount but not registered as Hive Metastore table into UC tables.
 
+### Post Migration Data Reconciliation Task
+UCX also provides `migrate-data-reconciliation` workflow to validate the integrity of the migrated tables:
+- Compare the schema of the source and target tables. The result is `schema_matches`, and column by column comparison
+is stored as `column_comparison` struct.
+- Compare the row counts of the source and target tables. If the row count is within the reconciliation threshold
+(defaults to 5%), `data_matches` is True.
+- Compare the content of individual row between source and target tables to identify any discrepancies (when `compare_rows` 
+flag is enabled). This is done using hash comparison, and number of missing rows are stored as `source_missing_count`
+and `target_missing_count`
+
+Once the workflow completes, the output will be stored in `$inventory_database.reconciliation_results` view, and displayed
+in the Migration dashboard.
+
+![reconciliation results](docs/recon_results.png)
+
 ### Other considerations
 - You may need to run the workflow multiple times to ensure all the tables are migrated successfully in phases.
 - If your Delta tables in DBFS root have a large number of files, consider:
   - Setting higher `Min` and `Max workers for auto-scale` when being asked during the UCX installation. More cores in the cluster means more concurrency for calling cloud storage API to copy files when deep cloning the Delta tables.
   - Setting higher `Parallelism for migrating DBFS root Delta tables with deep clone` (default 200) when being asked during the UCX installation. This controls the number of Spark tasks/partitions to be created for deep clone.
 - Consider creating an instance pool, and setting its id when prompted during the UCX installation. This instance pool will be specified in the cluster policy used by all UCX workflows job clusters.
 - You may also manually edit the job cluster configration per job or per task after the workflows are deployed.
 
+### [EXPERIMENTAL] Scan tables in mounts Workflow
+#### <b>Always run this workflow AFTER the assessment has finished</b>
+- This experimental workflow attemps to find all Tables inside mount points that are present on your workspace.
+- If you do not run this workflow, then `migrate-tables-in-mounts-experimental` won't do anything.
+- It writes all results to `hive_metastore.<inventory_database>.tables`, you can query those tables found by filtering on database values that starts with `mounted_`
+- This command is incremental, meaning that each time you run it, it will overwrite the previous tables in mounts found.
+- Current format are supported:
+  - DELTA - PARQUET - CSV - JSON
+  - Also detects partitioned DELTA and PARQUET
+- You can configure these workflows with the following options available on conf.yml:
+  - include_mounts : A list of mount points to scans, by default the workflow scans for all mount points
+  - exclude_paths_in_mount : A list of paths to exclude in all mount points
+  - include_paths_in_mount : A list of paths to include in all mount points 
+
+### [EXPERIMENTAL] Migrate tables in mounts Workflow
+- An experimental workflow that migrates tables in mount points using a `CREATE TABLE` command, optinally sets a default tables owner if provided in `default_table_owner` conf parameter. 
+- You must do the following in order to make this work: 
+  - run the Assessment [workflow](#assessment-workflow)
+  - run the scan tables in mounts [workflow](#EXPERIMENTAL-scan-tables-in-mounts-workflow)
+  - run the [`create-table-mapping` command](#create-table-mapping-command)
+    - or manually create a `mapping.csv` file in Workspace -> Applications -> ucx
+
+
+[[back to top](#databricks-labs-ucx)]
+
+## Jobs Static Code Analysis Workflow
+
+> Please note that this is an experimental workflow.
+
+The `experimental-workflow-linter` workflow lints accessible code belonging to all workflows/jobs present in the
+workspace. The linting emits problems indicating what to resolve for making the code Unity Catalog compatible.
+
+![code compatibility problems](docs/code_compatibility_problems.png)
+
 [[back to top](#databricks-labs-ucx)]
 
 # Utility commands
 
 ## `logs` command
 
 ```text
@@ -914,14 +970,33 @@
 After you're done with the [table migration](#table-migration-workflow), you can proceed to the code migration.
 
 Once you're done with the code migration, you can run the [`cluster-remap` command](#cluster-remap-command) to remap the
 clusters to be UC compatible.
 
 [[back to top](#databricks-labs-ucx)]
 
+## `lint-local-code` command
+
+```text
+databricks labs ucx lint-local-code
+```
+
+At any time, you can run this command to assess all migrations required in a local directory or a file. It only takes seconds to run and it
+gives you an initial overview of what needs to be migrated without actually performing any migration. A great way to start a migration!
+
+This command detects all dependencies, and analyzes them. It is still experimental and at the moment only supports Python and SQL files.
+We expect this command to run within a minute on code bases up to 50.000 lines of code.
+Future versions of `ucx` will add support for more source types, and more migration details.
+
+When run from an IDE terminal, this command generates output as follows:
+![img.png](docs/lint-local-code-output.png)
+With modern IDEs, clicking on the file link opens the file at the problematic line
+
+[[back to top](#databricks-labs-ucx)]
+
 ## `migrate-local-code` command
 
 ```text
 databricks labs ucx migrate-local-code
 ```
 
 **(Experimental)** Once [table migration](#table-migration-workflow) is complete, you can run this command to
```

### Comparing `databricks_labs_ucx-0.23.1/pyproject.toml` & `databricks_labs_ucx-0.24.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -40,19 +40,19 @@
     "Intended Audience :: System Administrators",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
     "Topic :: Software Development :: Libraries",
     "Topic :: Utilities",
 ]
 
-dependencies = ["databricks-sdk~=0.27.0",
+dependencies = ["databricks-sdk>=0.27,<0.29",
                 "databricks-labs-lsql~=0.4.0",
-                "databricks-labs-blueprint>=0.4.3,<0.6.0",
+                "databricks-labs-blueprint>=0.6.0",
                 "PyYAML>=6.0.0,<7.0.0",
-                "sqlglot>=23.9,<23.15"]
+                "sqlglot>=23.9,<24.1"]
 
 [project.entry-points.databricks]
 runtime = "databricks.labs.ucx.runtime:main"
 
 [project.urls]
 Issues = "https://github.com/databricks/ucx/issues"
 Source = "https://github.com/databricks/ucx"
@@ -83,19 +83,19 @@
 # store virtual env as the child of this folder. Helps VSCode (and PyCharm) to run better
 path = ".venv"
 
 [tool.hatch.envs.default.scripts]
 test        = "pytest -n 4 --cov src --cov-report=xml --timeout 30 tests/unit --durations 20"
 coverage    = "pytest -n auto --cov src tests/unit --timeout 30 --cov-report=html --durations 20"
 integration = "pytest -n 10 --cov src tests/integration --durations 20"
-fmt         = ["black .",
+fmt         = ["black . --extend-exclude 'tests/unit/source_code/samples/*'",
                "ruff check . --fix",
                "mypy --disable-error-code 'annotation-unchecked' --exclude 'tests/unit/source_code/samples/*' .",
                "pylint --output-format=colorized -j 0 src tests"]
-verify      = ["black --check .",
+verify      = ["black --check . --extend-exclude 'tests/unit/source_code/samples/*'",
                "ruff .",
                "mypy --exclude 'tests/unit/source_code/samples/*' .",
                "pylint --output-format=colorized -j 0 src tests"]
 lint         = ["pylint --output-format=colorized -j 0 src tests"]
 
 [tool.pytest.ini_options]
 # TODO: remove `-p no:warnings`
```

### Comparing `databricks_labs_ucx-0.23.1/PKG-INFO` & `databricks_labs_ucx-0.24.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: databricks-labs-ucx
-Version: 0.23.1
+Version: 0.24.0
 Summary: UCX - Unity Catalog Migration Toolkit
 Project-URL: Issues, https://github.com/databricks/ucx/issues
 Project-URL: Source, https://github.com/databricks/ucx
 Author-email: Serge Smertin <serge.smertin@databricks.com>
 Maintainer-email: Serge Smertin <serge.smertin@databricks.com>, Liran Bareket <liran.bareket@databricks.com>, Marcin Wojtyczka <marcin.wojtyczka@databricks.com>, Ziyuan Qin <ziyuan.qin@databricks.com>, William Conti <william.conti@databricks.com>, Hari Selvarajan <hari.selvarajan@databricks.com>, Vuong Nguyen <vuong.nguyen@databricks.com>
 License-File: LICENSE
 License-File: NOTICE
@@ -21,19 +21,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
-Requires-Dist: databricks-labs-blueprint<0.6.0,>=0.4.3
+Requires-Dist: databricks-labs-blueprint>=0.6.0
 Requires-Dist: databricks-labs-lsql~=0.4.0
-Requires-Dist: databricks-sdk~=0.27.0
+Requires-Dist: databricks-sdk<0.29,>=0.27
 Requires-Dist: pyyaml<7.0.0,>=6.0.0
-Requires-Dist: sqlglot<23.15,>=23.9
+Requires-Dist: sqlglot<24.1,>=23.9
 Description-Content-Type: text/markdown
 
 Databricks Labs UCX
 ===
 ![UCX by Databricks Labs](docs/logo-no-background.png)
 
 The companion for upgrading to Unity Catalog. 
@@ -68,15 +68,17 @@
   * [Assessment workflow](#assessment-workflow)
   * [Group migration workflow](#group-migration-workflow)
   * [Debug notebook](#debug-notebook)
   * [Debug logs](#debug-logs)
   * [Table Migration Workflow](#table-migration-workflow)
     * [Dependency CLI commands](#dependency-cli-commands)
     * [Table Migration Workflow Tasks](#table-migration-workflow-tasks)
+    * [Post Migration Data Reconciliation Task](#post-migration-data-reconciliation-task)
     * [Other considerations](#other-considerations)
+  * [Jobs Static Code Analysis Workflow](#jobs-static-code-analysis-workflow)
 * [Utility commands](#utility-commands)
   * [`logs` command](#logs-command)
   * [`ensure-assessment-run` command](#ensure-assessment-run-command)
   * [`repair-run` command](#repair-run-command)
   * [`workflows` command](#workflows-command)
   * [`open-remote-config` command](#open-remote-config-command)
   * [`installations` command](#installations-command)
@@ -96,14 +98,15 @@
   * [`skip` command](#skip-command)
   * [`create-catalogs-schemas` command](#create-catalogs-schemas-command)
   * [`migrate-tables` command](#migrate-tables-command)
   * [`revert-migrated-tables` command](#revert-migrated-tables-command)
   * [`move` command](#move-command)
   * [`alias` command](#alias-command)
 * [Code migration commands](#code-migration-commands)
+  * [`lint-local-code` command](#lint-local-code-command)
   * [`migrate-local-code` command](#migrate-local-code-command)
   * [`migrate-dbsql-dashboards` command](#migrate-dbsql-dashboards-command)
   * [`revert-dbsql-dashboards` command](#revert-dbsql-dashboards-command)
 * [Cross-workspace installations](#cross-workspace-installations)
   * [`sync-workspace-info` command](#sync-workspace-info-command)
   * [`manual-workspace-info` command](#manual-workspace-info-command)
   * [`create-account-groups` command](#create-account-groups-command)
@@ -114,14 +117,15 @@
 * [Project Support](#project-support)
 <!-- TOC -->
 
 # Installation
 
 - Databricks CLI v0.213 or later. See [instructions](#authenticate-databricks-cli). 
 - Python 3.10 or later. See [Windows](https://www.python.org/downloads/windows/) instructions.
+- Databricks Premium or Enterprise workspace.
 - Network access to your Databricks Workspace used for the [installation process](#install-ucx).
 - Network access to the Internet for [pypi.org](https://pypi.org) and [github.com](https://github.com) from machine running the installation.
 - Databricks Workspace Administrator privileges for the user, that runs the installation. Running UCX as a Service Principal is not supported.
 - Account level Identity Setup. See instructions for [AWS](https://docs.databricks.com/en/administration-guide/users-groups/best-practices.html), [Azure](https://learn.microsoft.com/en-us/azure/databricks/administration-guide/users-groups/best-practices), and [GCP](https://docs.gcp.databricks.com/administration-guide/users-groups/best-practices.html).
 - Unity Catalog Metastore Created (per region). See instructions for [AWS](https://docs.databricks.com/en/data-governance/unity-catalog/create-metastore.html), [Azure](https://learn.microsoft.com/en-us/azure/databricks/data-governance/unity-catalog/create-metastore), and [GCP](https://docs.gcp.databricks.com/data-governance/unity-catalog/create-metastore.html).
 - If your Databricks Workspace relies on an external Hive Metastore (such as AWS Glue), make sure to read [this guide](docs/external_hms_glue.md).
 - Databricks Workspace has to have network access to [pypi.org](https://pypi.org) to download `databricks-sdk`, `databricks-labs-lsql`, `databricks-labs-blueprint`, `sqlglot` and `pyyaml` packages.
@@ -173,14 +177,17 @@
 The [`WorkspaceInstallation`](src/databricks/labs/ucx/install.py) manages the installation and uninstallation of UCX in a workspace. It handles 
 the configuration and exception management during the installation process. The installation process creates dashboards, databases, and jobs. 
 It also includes the creation of a database with given configuration and the deployment of workflows with specific settings. The installation 
 process can handle exceptions and infer errors from job runs and task runs. The workspace installation uploads wheels, creates cluster policies, 
 and wheel runners to the workspace. It can also handle the creation of job tasks for a given task, such as job dashboard tasks, job notebook tasks, 
 and job wheel tasks. The class handles the installation of UCX, including configuring the workspace, installing necessary libraries, and verifying 
 the installation, making it easier for users to migrate their workspaces to UCX.
+At the end of the installation, the user will be prompted if the current installation needs to join an existing collection (create new collection if none present).
+For large organization with many workspaces, grouping workspaces into collection helps in managing UCX migration at collection level (instead of workspaces level)
+User should be an account admin to be able to join a collection.
 
 After this, UCX will be installed locally and a number of assets will be deployed in the selected workspace. 
 These assets are available under the installation folder, i.e. `/Users/<your user>/.ucx/`.
 
 You can also install a specific version by specifying it like `@v0.13.2` - `databricks labs install ucx@v0.13.2`.
 
 ![macos_install_ucx](docs/macos_2_databrickslabsmac_installucx.gif)
@@ -485,22 +492,71 @@
   - `migrate_external_tables_sync` - Migrate external tables using [`SYNC`](https://docs.databricks.com/en/sql/language-manual/sql-ref-syntax-aux-sync.html) command. This does not create copy of the tables.
 - `migrate-external-hiveserde-tables-in-place-experimental` - Experimental in-place migration of HiveSerde tables. HiveSerDe tables include ParquetHiveSerDe, OrcSerde, AvroSerDe, LazySimpleSerDe, JsonSerDe, OpenCSVSerde tables.
   - `migrate_external_hiveserde_tables_in_place_experimental` - Migrate HiveSerde tables in place.
 - Following workflows/tasks are on the roadmap and being developed:
   - Migrate tables using CTAS 
   - Experimentally migrate Delta and Parquet data found in dbfs mount but not registered as Hive Metastore table into UC tables.
 
+### Post Migration Data Reconciliation Task
+UCX also provides `migrate-data-reconciliation` workflow to validate the integrity of the migrated tables:
+- Compare the schema of the source and target tables. The result is `schema_matches`, and column by column comparison
+is stored as `column_comparison` struct.
+- Compare the row counts of the source and target tables. If the row count is within the reconciliation threshold
+(defaults to 5%), `data_matches` is True.
+- Compare the content of individual row between source and target tables to identify any discrepancies (when `compare_rows` 
+flag is enabled). This is done using hash comparison, and number of missing rows are stored as `source_missing_count`
+and `target_missing_count`
+
+Once the workflow completes, the output will be stored in `$inventory_database.reconciliation_results` view, and displayed
+in the Migration dashboard.
+
+![reconciliation results](docs/recon_results.png)
+
 ### Other considerations
 - You may need to run the workflow multiple times to ensure all the tables are migrated successfully in phases.
 - If your Delta tables in DBFS root have a large number of files, consider:
   - Setting higher `Min` and `Max workers for auto-scale` when being asked during the UCX installation. More cores in the cluster means more concurrency for calling cloud storage API to copy files when deep cloning the Delta tables.
   - Setting higher `Parallelism for migrating DBFS root Delta tables with deep clone` (default 200) when being asked during the UCX installation. This controls the number of Spark tasks/partitions to be created for deep clone.
 - Consider creating an instance pool, and setting its id when prompted during the UCX installation. This instance pool will be specified in the cluster policy used by all UCX workflows job clusters.
 - You may also manually edit the job cluster configration per job or per task after the workflows are deployed.
 
+### [EXPERIMENTAL] Scan tables in mounts Workflow
+#### <b>Always run this workflow AFTER the assessment has finished</b>
+- This experimental workflow attemps to find all Tables inside mount points that are present on your workspace.
+- If you do not run this workflow, then `migrate-tables-in-mounts-experimental` won't do anything.
+- It writes all results to `hive_metastore.<inventory_database>.tables`, you can query those tables found by filtering on database values that starts with `mounted_`
+- This command is incremental, meaning that each time you run it, it will overwrite the previous tables in mounts found.
+- Current format are supported:
+  - DELTA - PARQUET - CSV - JSON
+  - Also detects partitioned DELTA and PARQUET
+- You can configure these workflows with the following options available on conf.yml:
+  - include_mounts : A list of mount points to scans, by default the workflow scans for all mount points
+  - exclude_paths_in_mount : A list of paths to exclude in all mount points
+  - include_paths_in_mount : A list of paths to include in all mount points 
+
+### [EXPERIMENTAL] Migrate tables in mounts Workflow
+- An experimental workflow that migrates tables in mount points using a `CREATE TABLE` command, optinally sets a default tables owner if provided in `default_table_owner` conf parameter. 
+- You must do the following in order to make this work: 
+  - run the Assessment [workflow](#assessment-workflow)
+  - run the scan tables in mounts [workflow](#EXPERIMENTAL-scan-tables-in-mounts-workflow)
+  - run the [`create-table-mapping` command](#create-table-mapping-command)
+    - or manually create a `mapping.csv` file in Workspace -> Applications -> ucx
+
+
+[[back to top](#databricks-labs-ucx)]
+
+## Jobs Static Code Analysis Workflow
+
+> Please note that this is an experimental workflow.
+
+The `experimental-workflow-linter` workflow lints accessible code belonging to all workflows/jobs present in the
+workspace. The linting emits problems indicating what to resolve for making the code Unity Catalog compatible.
+
+![code compatibility problems](docs/code_compatibility_problems.png)
+
 [[back to top](#databricks-labs-ucx)]
 
 # Utility commands
 
 ## `logs` command
 
 ```text
@@ -948,14 +1004,33 @@
 After you're done with the [table migration](#table-migration-workflow), you can proceed to the code migration.
 
 Once you're done with the code migration, you can run the [`cluster-remap` command](#cluster-remap-command) to remap the
 clusters to be UC compatible.
 
 [[back to top](#databricks-labs-ucx)]
 
+## `lint-local-code` command
+
+```text
+databricks labs ucx lint-local-code
+```
+
+At any time, you can run this command to assess all migrations required in a local directory or a file. It only takes seconds to run and it
+gives you an initial overview of what needs to be migrated without actually performing any migration. A great way to start a migration!
+
+This command detects all dependencies, and analyzes them. It is still experimental and at the moment only supports Python and SQL files.
+We expect this command to run within a minute on code bases up to 50.000 lines of code.
+Future versions of `ucx` will add support for more source types, and more migration details.
+
+When run from an IDE terminal, this command generates output as follows:
+![img.png](docs/lint-local-code-output.png)
+With modern IDEs, clicking on the file link opens the file at the problematic line
+
+[[back to top](#databricks-labs-ucx)]
+
 ## `migrate-local-code` command
 
 ```text
 databricks labs ucx migrate-local-code
 ```
 
 **(Experimental)** Once [table migration](#table-migration-workflow) is complete, you can run this command to
```

