# Comparing `tmp/resc_backend-3.3.0.tar.gz` & `tmp/resc_backend-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_backend-3.3.0.tar", last modified: Fri May 24 15:29:42 2024, max compression
+gzip compressed data, was "resc_backend-3.3.1.tar", last modified: Mon May 27 15:38:22 2024, max compression
```

## Comparing `resc_backend-3.3.0.tar` & `resc_backend-3.3.1.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.221480 resc_backend-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-24 15:29:36.000000 resc_backend-3.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-05-24 15:29:42.221480 resc_backend-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-05-24 15:29:36.000000 resc_backend-3.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-24 15:29:36.000000 resc_backend-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-24 15:29:36.000000 resc_backend-3.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-24 15:29:42.221480 resc_backend-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-24 15:29:36.000000 resc_backend-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.189479 resc_backend-3.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.193479 resc_backend-3.3.0/src/resc_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.197480 resc_backend-3.3.0/src/resc_backend/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/bin/rabbitmq_bootup.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.197480 resc_backend-3.3.0/src/resc_backend/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/engine_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.197480 resc_backend-3.3.0/src/resc_backend/db/model/
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/model/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/model/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/model/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/model/rule_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/model/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/model/rule_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/model/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/model/scan_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/model/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/model/vcs_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.197480 resc_backend-3.3.0/src/resc_backend/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/helpers/dict_remapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/helpers/environment_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/helpers/list_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.197480 resc_backend-3.3.0/src/resc_backend/helpers/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/helpers/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/helpers/rabbitmq/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.201480 resc_backend-3.3.0/src/resc_backend/resc_web_service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/cache_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.201480 resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/detailed_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)    36235 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)    15505 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     6385 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/rule_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/scan_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/vcs_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.205479 resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py
--rw-r--r--   0 runner    (1001) docker     (127)    17780 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/findings.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/health.py
--rw-r--r--   0 runner    (1001) docker     (127)    12791 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    20433 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)    17302 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    16686 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/scans.py
--rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.205479 resc_backend-3.3.0/src/resc_backend/resc_web_service/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/helpers/exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/helpers/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/helpers/toml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.217480 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/audit_count_over_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/date_count_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/date_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/detailed_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/finding_count_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/finding_count_over_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/finding_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/pagination_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/personal_audit_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/repository_enriched.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/rule_count_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/scan_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/status_count.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/time_period.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/vcs_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/vcs_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.217480 resc_backend-3.3.0/src/resc_backend/resc_web_service_interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service_interface/findings.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service_interface/repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service_interface/rule_packs.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service_interface/scans.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service_interface/vcs_instances.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.217480 resc_backend-3.3.0/src/resc_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-05-24 15:29:42.000000 resc_backend-3.3.0/src/resc_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-24 15:29:42.000000 resc_backend-3.3.0/src/resc_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:29:42.000000 resc_backend-3.3.0/src/resc_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-24 15:29:42.000000 resc_backend-3.3.0/src/resc_backend.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:29:42.000000 resc_backend-3.3.0/src/resc_backend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-24 15:29:42.000000 resc_backend-3.3.0/src/resc_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 15:29:42.000000 resc_backend-3.3.0/src/resc_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:22.023723 resc_backend-3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-27 15:38:16.000000 resc_backend-3.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-05-27 15:38:22.023723 resc_backend-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-05-27 15:38:16.000000 resc_backend-3.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-27 15:38:16.000000 resc_backend-3.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-27 15:38:16.000000 resc_backend-3.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-27 15:38:22.023723 resc_backend-3.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-27 15:38:16.000000 resc_backend-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:22.003723 resc_backend-3.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:22.007723 resc_backend-3.3.1/src/resc_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:22.007723 resc_backend-3.3.1/src/resc_backend/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/bin/rabbitmq_bootup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:22.007723 resc_backend-3.3.1/src/resc_backend/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/db/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/db/engine_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:22.011723 resc_backend-3.3.1/src/resc_backend/db/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/db/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/db/model/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/db/model/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/db/model/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/db/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/db/model/rule_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/db/model/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/db/model/rule_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/db/model/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/db/model/scan_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/db/model/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/db/model/vcs_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:22.011723 resc_backend-3.3.1/src/resc_backend/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/helpers/dict_remapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/helpers/environment_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/helpers/list_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:22.011723 resc_backend-3.3.1/src/resc_backend/helpers/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/helpers/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/helpers/rabbitmq/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:22.011723 resc_backend-3.3.1/src/resc_backend/resc_web_service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/cache_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:22.015723 resc_backend-3.3.1/src/resc_backend/resc_web_service/crud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/crud/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/crud/detailed_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37721 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/crud/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15505 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/crud/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6385 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/crud/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/crud/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/crud/rule_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/crud/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/crud/scan_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/crud/vcs_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:22.019723 resc_backend-3.3.1/src/resc_backend/resc_web_service/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/endpoints/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/endpoints/detailed_findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17780 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/endpoints/findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/endpoints/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12791 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/endpoints/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20433 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/endpoints/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17302 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/endpoints/rule_packs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/endpoints/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17107 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/endpoints/scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/endpoints/vcs_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:22.019723 resc_backend-3.3.1/src/resc_backend/resc_web_service/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/helpers/exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/helpers/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/helpers/toml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:22.023723 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/audit_count_over_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/date_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/date_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/detailed_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/finding_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/finding_count_over_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/finding_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/pagination_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/personal_audit_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/repository_enriched.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/rule_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/rule_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/scan_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/status_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/time_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/vcs_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/vcs_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:22.023723 resc_backend-3.3.1/src/resc_backend/resc_web_service_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service_interface/findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service_interface/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service_interface/rule_packs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service_interface/scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-27 15:38:16.000000 resc_backend-3.3.1/src/resc_backend/resc_web_service_interface/vcs_instances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:38:22.023723 resc_backend-3.3.1/src/resc_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-05-27 15:38:21.000000 resc_backend-3.3.1/src/resc_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-27 15:38:21.000000 resc_backend-3.3.1/src/resc_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 15:38:21.000000 resc_backend-3.3.1/src/resc_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-27 15:38:21.000000 resc_backend-3.3.1/src/resc_backend.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 15:38:21.000000 resc_backend-3.3.1/src/resc_backend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-27 15:38:21.000000 resc_backend-3.3.1/src/resc_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 15:38:21.000000 resc_backend-3.3.1/src/resc_backend.egg-info/top_level.txt
```

### Comparing `resc_backend-3.3.0/LICENSE.md` & `resc_backend-3.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/PKG-INFO` & `resc_backend-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc_backend
-Version: 3.3.0
+Version: 3.3.1
 Summary: Repository Scanner - Backend
 Home-page: https://github.com/abnamro/resc-backend
 Download-URL: 
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `resc_backend-3.3.0/README.md` & `resc_backend-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/pyproject.toml` & `resc_backend-3.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/setup.cfg` & `resc_backend-3.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = resc_backend
 description = Repository Scanner - Backend
-version = 3.3.0
+version = 3.3.1
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
 url = https://github.com/abnamro/resc-backend
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE.md
```

### Comparing `resc_backend-3.3.0/src/resc_backend/bin/rabbitmq_bootup.py` & `resc_backend-3.3.1/src/resc_backend/bin/rabbitmq_bootup.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/common.py` & `resc_backend-3.3.1/src/resc_backend/common.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/constants.py` & `resc_backend-3.3.1/src/resc_backend/constants.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/db/connection.py` & `resc_backend-3.3.1/src/resc_backend/db/connection.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/db/engine_azure.py` & `resc_backend-3.3.1/src/resc_backend/db/engine_azure.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/db/model/__init__.py` & `resc_backend-3.3.1/src/resc_backend/db/model/__init__.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/db/model/audit.py` & `resc_backend-3.3.1/src/resc_backend/db/model/audit.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/db/model/finding.py` & `resc_backend-3.3.1/src/resc_backend/db/model/finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/db/model/repository.py` & `resc_backend-3.3.1/src/resc_backend/db/model/repository.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/db/model/rule.py` & `resc_backend-3.3.1/src/resc_backend/db/model/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/db/model/rule_allow_list.py` & `resc_backend-3.3.1/src/resc_backend/db/model/rule_allow_list.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/db/model/rule_pack.py` & `resc_backend-3.3.1/src/resc_backend/db/model/rule_pack.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/db/model/scan.py` & `resc_backend-3.3.1/src/resc_backend/db/model/scan.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/db/model/vcs_instance.py` & `resc_backend-3.3.1/src/resc_backend/db/model/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/helpers/dict_remapper.py` & `resc_backend-3.3.1/src/resc_backend/helpers/dict_remapper.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/helpers/environment_wrapper.py` & `resc_backend-3.3.1/src/resc_backend/helpers/environment_wrapper.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/helpers/rabbitmq/configuration.py` & `resc_backend-3.3.1/src/resc_backend/helpers/rabbitmq/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py` & `resc_backend-3.3.1/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/api.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/api.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/cache_manager.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/cache_manager.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/configuration.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/audit.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/crud/audit.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,16 @@
         db_connection (Session): Session of the database connection
         findings_ids (list[int]): list of id to audit
         status (FindingStatus): status to apply
 
     Returns:
         list[DBaudit]: newly created audits
     """
+    db_connection.execute(update(DBaudit).where(DBaudit.finding_id.in_(findings_ids)).values(is_latest=False))
+
     db_audits = [DBaudit.create_automated(finding_id, status) for finding_id in findings_ids]
     db_connection.add_all(db_audits)
     db_connection.commit()
 
     logger.debug(f"Automated audit of {len(db_audits)} findings.")
 
     return db_audits
```

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/detailed_finding.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/crud/detailed_finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/finding.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/crud/finding.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,26 +257,68 @@
 
     Returns:
         list[int]: list of ids of findings which are to be audited
     """
 
     query = select(DBfinding.id_)
     query = query.join(DBrule, DBrule.rule_name == DBfinding.rule_name)
+    query = query.join(
+        DBaudit,
+        (DBaudit.finding_id == DBfinding.id_) & (DBaudit.is_latest == True),  # noqa: E712
+        isouter=True,
+    )
     query = query.where(DBrule.rule_pack == scan.rule_pack)
     query = query.where(DBfinding.repository_id == scan.repository_id)
     query = query.where(DBfinding.is_dir_scan == True)  # noqa: E712
+    query = query.where(
+        (DBaudit.status != FindingStatus.OUTDATED) | (DBaudit.status == None)  # noqa: E711
+    )
 
     sub_query: Query = select(DBscanFinding.finding_id)
     sub_query = sub_query.where(DBscanFinding.scan_id == scan.id_)
     sub_query = sub_query.subquery()
     query = query.where(DBfinding.id_.not_in(sub_query))
 
     return db_connection.execute(query).scalars().all()
 
 
+def get_untriaged_finding_outdated_for_current_rule_pack(db_connection: Session, scan: DBscan) -> list[int]:
+    """
+    Retrieve all the findings which are:
+     - tied to the repository of the scan
+     - where the rule is not in the rule pack of the scan
+     - which are not analyzed
+
+    Args:
+        db_connection (Session): session
+        scan (DBscan): scan to restrict with
+
+    Returns:
+        list[int]: list of ids of findings which are to be audited
+    """
+
+    sub_query_rule_name: Query = select(DBrule.rule_name)
+    sub_query_rule_name = sub_query_rule_name.where(DBrule.rule_pack == scan.rule_pack)
+    sub_query_rule_name = sub_query_rule_name.subquery()
+
+    query = select(DBfinding.id_)
+    query = query.where(DBfinding.repository_id == scan.repository_id)
+    query = query.where(DBfinding.rule_name.not_in(sub_query_rule_name))
+    query = query.join(
+        DBaudit,
+        (DBaudit.finding_id == DBfinding.id_) & (DBaudit.is_latest == True),  # noqa: E712
+        isouter=True,
+    )
+    query = query.where(
+        (DBaudit.status == FindingStatus.NOT_ANALYZED) | (DBaudit.status == None)  # noqa: E711
+    )
+
+    return db_connection.execute(query).scalars().all()
+
+
 def get_total_findings_count(db_connection: Session, findings_filter: FindingsFilter = None) -> int:
     """
         Retrieve count of finding records of a given scan
     :param findings_filter:
     :param db_connection:
         Session of the database connection
     :return: total_count
```

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/repository.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/crud/repository.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/rule.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/crud/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/rule_pack.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/crud/rule_pack.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/rule_tag.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/crud/rule_tag.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/scan.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/crud/scan.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/scan_finding.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/crud/scan_finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/vcs_instance.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/crud/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/dependencies.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/dependencies.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/common.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/endpoints/common.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/endpoints/detailed_findings.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/findings.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/endpoints/findings.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/health.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/metrics.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/endpoints/metrics.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/repositories.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/endpoints/repositories.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/endpoints/rule_packs.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/rules.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/endpoints/rules.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/scans.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/endpoints/scans.py`

 * *Files 2% similar despite different names*

```diff
@@ -285,14 +285,22 @@
     findings_to_audit: list[int] = finding_crud.get_findings_from_repo_of_scan_as_dir(
         db_connection=db_connection, scan=db_scan
     )
     audit_crud.create_automated_audit(
         db_connection=db_connection, findings_ids=findings_to_audit, status=FindingStatus.OUTDATED
     )
 
+    # 8. Mark findings which are no longer in rule pack (i.e. rule name not in current rule pack) as outdated
+    old_findings_to_audit: list[int] = finding_crud.get_untriaged_finding_outdated_for_current_rule_pack(
+        db_connection=db_connection, scan=db_scan
+    )
+    audit_crud.create_automated_audit(
+        db_connection=db_connection, findings_ids=old_findings_to_audit, status=FindingStatus.OUTDATED
+    )
+
     # Clear cache related to findings
     await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_FINDING)
     await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_RULE)
 
     return len(created_findings)
```

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/endpoints/vcs_instances.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/filters.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/filters.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/helpers/exception_handler.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/helpers/exception_handler.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/helpers/rule.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/helpers/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/helpers/toml.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/helpers/toml.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/audit.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/audit.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/detailed_finding.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/detailed_finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/finding.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/finding_count_model.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/finding_count_model.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/finding_status.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/finding_status.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/pagination_model.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/pagination_model.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/repository.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/repository.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/repository_enriched.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/repository_enriched.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/rule.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/rule_allow_list.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/rule_pack.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/rule_pack.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/scan.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/scan.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/vcs_instance.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service/schema/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service_interface/findings.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service_interface/findings.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service_interface/repositories.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service_interface/repositories.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service_interface/rule_packs.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service_interface/rule_packs.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend/resc_web_service_interface/vcs_instances.py` & `resc_backend-3.3.1/src/resc_backend/resc_web_service_interface/vcs_instances.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.3.0/src/resc_backend.egg-info/PKG-INFO` & `resc_backend-3.3.1/src/resc_backend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc_backend
-Version: 3.3.0
+Version: 3.3.1
 Summary: Repository Scanner - Backend
 Home-page: https://github.com/abnamro/resc-backend
 Download-URL: 
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `resc_backend-3.3.0/src/resc_backend.egg-info/SOURCES.txt` & `resc_backend-3.3.1/src/resc_backend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

