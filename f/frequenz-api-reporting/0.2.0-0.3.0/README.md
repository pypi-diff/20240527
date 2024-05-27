# Comparing `tmp/frequenz-api-reporting-0.2.0.tar.gz` & `tmp/frequenz-api-reporting-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-api-reporting-0.2.0.tar", last modified: Wed Apr 24 12:47:26 2024, max compression
+gzip compressed data, was "frequenz-api-reporting-0.3.0.tar", last modified: Mon May 27 12:03:13 2024, max compression
```

## Comparing `frequenz-api-reporting-0.2.0.tar` & `frequenz-api-reporting-0.3.0.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.661279 frequenz-api-reporting-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/RELEASE_NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.641279 frequenz-api-reporting-0.2.0/proto/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.641279 frequenz-api-reporting-0.2.0/proto/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.641279 frequenz-api-reporting-0.2.0/proto/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.641279 frequenz-api-reporting-0.2.0/proto/frequenz/api/reporting/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.645279 frequenz-api-reporting-0.2.0/proto/frequenz/api/reporting/v1/
--rw-r--r--   0 runner    (1001) docker     (127)    22178 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/proto/frequenz/api/reporting/v1/reporting.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.641279 frequenz-api-reporting-0.2.0/py/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.641279 frequenz-api-reporting-0.2.0/py/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.641279 frequenz-api-reporting-0.2.0/py/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.645279 frequenz-api-reporting-0.2.0/py/frequenz/api/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/py/frequenz/api/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/py/frequenz/api/reporting/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/py/frequenz/api/reporting/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.645279 frequenz-api-reporting-0.2.0/py/frequenz/api/reporting/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/py/frequenz/api/reporting/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.649279 frequenz-api-reporting-0.2.0/py/frequenz_api_reporting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-24 12:47:26.000000 frequenz-api-reporting-0.2.0/py/frequenz_api_reporting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-24 12:47:26.000000 frequenz-api-reporting-0.2.0/py/frequenz_api_reporting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:47:26.000000 frequenz-api-reporting-0.2.0/py/frequenz_api_reporting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-24 12:47:26.000000 frequenz-api-reporting-0.2.0/py/frequenz_api_reporting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 12:47:26.000000 frequenz-api-reporting-0.2.0/py/frequenz_api_reporting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 12:47:26.661279 frequenz-api-reporting-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.645279 frequenz-api-reporting-0.2.0/submodules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.641279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.645279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.653279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/annotations.proto
--rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/auth.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/backend.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/billing.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/client.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/config_change.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/consumer.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/context.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/control.proto
--rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/distribution.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/documentation.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/endpoint.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/field_behavior.proto
--rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/http.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/httpbody.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/label.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/launch_stage.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/log.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/logging.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/metric.proto
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/monitored_resource.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/monitoring.proto
--rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/quota.proto
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/resource.proto
--rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/routing.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/service.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/source_info.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/system_parameter.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/usage.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.653279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/cloud/extended_operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.641279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.641279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.653279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/admin/v1/
--rw-r--r--   0 runner    (1001) docker     (127)    41483 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.653279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.653279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/v1/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/v1/options.proto
--rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/v1/policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.641279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/logging/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.653279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/logging/type/
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/logging/type/http_request.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/logging/type/log_severity.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.653279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/longrunning/
--rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/longrunning/operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.653279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/rpc/
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/rpc/code.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.653279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/rpc/context/
--rw-r--r--   0 runner    (1001) docker     (127)    12015 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto
--rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/rpc/error_details.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/rpc/status.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/calendar_period.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/color.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/date.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/datetime.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/dayofweek.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/expr.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/fraction.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/latlng.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/money.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/month.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/postal_address.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/quaternion.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/timeofday.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.645279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.645279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.645279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.645279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/location.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_area.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_duration.proto
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/location.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/energy.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/price.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/bounds.proto
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/metric_sample.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/battery.proto
--rw-r--r--   0 runner    (1001) docker     (127)    17511 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/components.proto
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/fuse.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/grid.proto
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/inverter.proto
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/transformer.proto
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/lifetime.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/microgrid.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_info.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/types/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/types/decimal.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.190571 frequenz-api-reporting-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-27 12:03:00.000000 frequenz-api-reporting-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-27 12:03:00.000000 frequenz-api-reporting-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-05-27 12:03:13.190571 frequenz-api-reporting-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-27 12:03:00.000000 frequenz-api-reporting-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-27 12:03:00.000000 frequenz-api-reporting-0.3.0/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.174571 frequenz-api-reporting-0.3.0/proto/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.174571 frequenz-api-reporting-0.3.0/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.174571 frequenz-api-reporting-0.3.0/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.174571 frequenz-api-reporting-0.3.0/proto/frequenz/api/reporting/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.178571 frequenz-api-reporting-0.3.0/proto/frequenz/api/reporting/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    22522 2024-05-27 12:03:00.000000 frequenz-api-reporting-0.3.0/proto/frequenz/api/reporting/v1/reporting.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.174571 frequenz-api-reporting-0.3.0/py/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.174571 frequenz-api-reporting-0.3.0/py/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.174571 frequenz-api-reporting-0.3.0/py/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.178571 frequenz-api-reporting-0.3.0/py/frequenz/api/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-27 12:03:00.000000 frequenz-api-reporting-0.3.0/py/frequenz/api/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-27 12:03:00.000000 frequenz-api-reporting-0.3.0/py/frequenz/api/reporting/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:00.000000 frequenz-api-reporting-0.3.0/py/frequenz/api/reporting/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.178571 frequenz-api-reporting-0.3.0/py/frequenz/api/reporting/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-27 12:03:00.000000 frequenz-api-reporting-0.3.0/py/frequenz/api/reporting/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.182571 frequenz-api-reporting-0.3.0/py/frequenz_api_reporting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-05-27 12:03:13.000000 frequenz-api-reporting-0.3.0/py/frequenz_api_reporting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-27 12:03:13.000000 frequenz-api-reporting-0.3.0/py/frequenz_api_reporting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:03:13.000000 frequenz-api-reporting-0.3.0/py/frequenz_api_reporting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-27 12:03:13.000000 frequenz-api-reporting-0.3.0/py/frequenz_api_reporting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-27 12:03:13.000000 frequenz-api-reporting-0.3.0/py/frequenz_api_reporting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-05-27 12:03:00.000000 frequenz-api-reporting-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 12:03:13.190571 frequenz-api-reporting-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.178571 frequenz-api-reporting-0.3.0/submodules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.174571 frequenz-api-reporting-0.3.0/submodules/api-common-protos/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.178571 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.186571 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/annotations.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/auth.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/backend.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/billing.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/client.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/config_change.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/consumer.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/context.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/control.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/distribution.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/documentation.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/endpoint.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/field_behavior.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/http.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/httpbody.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/label.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/launch_stage.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/log.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/logging.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/metric.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/monitored_resource.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/monitoring.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/quota.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/resource.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/routing.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/service.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/source_info.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/system_parameter.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/usage.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.186571 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/cloud/extended_operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.178571 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/iam/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.178571 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/iam/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.186571 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/iam/admin/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    41483 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.186571 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/iam/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.186571 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/iam/v1/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/iam/v1/options.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/iam/v1/policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.178571 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/logging/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.186571 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/logging/type/
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/logging/type/http_request.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/logging/type/log_severity.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.186571 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/longrunning/
+-rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/longrunning/operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.186571 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/rpc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/rpc/code.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.186571 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/rpc/context/
+-rw-r--r--   0 runner    (1001) docker     (127)    12015 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/rpc/error_details.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/rpc/status.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.186571 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/calendar_period.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/color.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/date.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/datetime.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/dayofweek.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/expr.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/fraction.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/latlng.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/money.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/month.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/postal_address.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/quaternion.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-27 12:03:01.000000 frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/timeofday.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.178571 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.178571 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.178571 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.178571 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.186571 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-27 12:03:02.000000 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-27 12:03:02.000000 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/location.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.190571 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-05-27 12:03:02.000000 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-27 12:03:02.000000 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.190571 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.190571 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-27 12:03:02.000000 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_area.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-27 12:03:02.000000 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_duration.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-27 12:03:02.000000 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/location.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.190571 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-27 12:03:02.000000 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/energy.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-27 12:03:02.000000 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/price.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.190571 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-27 12:03:02.000000 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/bounds.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-05-27 12:03:02.000000 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/metric_sample.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.190571 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.190571 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-27 12:03:02.000000 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/battery.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    17511 2024-05-27 12:03:02.000000 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/components.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-27 12:03:02.000000 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-27 12:03:02.000000 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/fuse.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-27 12:03:02.000000 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/grid.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-27 12:03:02.000000 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/inverter.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-27 12:03:02.000000 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/transformer.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-27 12:03:02.000000 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/lifetime.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-27 12:03:02.000000 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/microgrid.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.190571 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-27 12:03:02.000000 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.190571 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-27 12:03:02.000000 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_info.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-27 12:03:02.000000 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:13.190571 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-27 12:03:02.000000 frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/types/decimal.proto
```

### Comparing `frequenz-api-reporting-0.2.0/LICENSE` & `frequenz-api-reporting-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/PKG-INFO` & `frequenz-api-reporting-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-api-reporting
-Version: 0.2.0
+Version: 0.3.0
 Summary: Frequenz gRPC API to aggregate component data from microgrids
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-api-reporting/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-reporting/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-reporting/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-reporting
```

### Comparing `frequenz-api-reporting-0.2.0/README.md` & `frequenz-api-reporting-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/proto/frequenz/api/reporting/v1/reporting.proto` & `frequenz-api-reporting-0.3.0/proto/frequenz/api/reporting/v1/reporting.proto`

 * *Files 1% similar despite different names*

```diff
@@ -304,14 +304,18 @@
   message StreamFilter {
     // Optional resampling options like resolution for the data, represented in seconds.
     // If omitted, data will be returned in its original representation.
     ResamplingOptions resampling_options = 1;
 
     // Include options specifying additional fields to be included in the response.
     IncludeOptions include_options = 2;
+
+    // Optional time-based filter criteria.
+    // If omitted, data will start streaming from the timestamp that the request was received.
+    TimeFilter time_filter = 3;
   }
 
   // Encapsulates the microgrid ID and the component IDs within that microgrid for which
   // the historical data should be retrieved.
   //
   // !!! note
   //     Each entry in this repeated field associates a microgrid ID with its respective
@@ -495,14 +499,18 @@
 //
 message ReceiveAggregatedMicrogridComponentsDataStreamRequest {
   // General filter criteria for querying microgrid components data.
   message AggregationStreamFilter {
     // Optional resampling options like resolution for the data, represented in seconds.
     // If omitted, data will be returned in its original representation.
     ResamplingOptions resampling_options = 1;
+
+    // Optional time-based filter criteria.
+    // If omitted, data will start streaming from the timestamp that the request was received.
+    TimeFilter time_filter = 2;
   }
 
   // List of pairs of metric and corresponding aggregation formula.
   repeated AggregationConfig aggregation_configs = 1;
 
   // General streaming filter that applies to all formula aggregations.
   AggregationStreamFilter filter = 2;
```

### Comparing `frequenz-api-reporting-0.2.0/py/frequenz_api_reporting.egg-info/PKG-INFO` & `frequenz-api-reporting-0.3.0/py/frequenz_api_reporting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-api-reporting
-Version: 0.2.0
+Version: 0.3.0
 Summary: Frequenz gRPC API to aggregate component data from microgrids
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-api-reporting/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-reporting/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-reporting/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-reporting
```

### Comparing `frequenz-api-reporting-0.2.0/py/frequenz_api_reporting.egg-info/SOURCES.txt` & `frequenz-api-reporting-0.3.0/py/frequenz_api_reporting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/py/frequenz_api_reporting.egg-info/requires.txt` & `frequenz-api-reporting-0.3.0/py/frequenz_api_reporting.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 mkdocs-macros-plugin==1.0.4
 mkdocs-material==9.3.1
 mkdocstrings[python]==0.23.0
 frequenz-repo-config[api]==0.7.0
 
 [dev-mypy]
 mypy==1.5.1
-grpc-stubs==1.53.0.2
+grpc-stubs==1.53.0.5
 types-Markdown==3.4.2.10
 frequenz-api-reporting[dev-mkdocs,dev-noxfile,dev-pytest]
 
 [dev-noxfile]
 nox==2023.4.22
 frequenz-repo-config[api]==0.7.0
```

### Comparing `frequenz-api-reporting-0.2.0/pyproject.toml` & `frequenz-api-reporting-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
   "mkdocs-macros-plugin == 1.0.4",
   "mkdocs-material == 9.3.1",
   "mkdocstrings[python] == 0.23.0",
   "frequenz-repo-config[api] == 0.7.0",
 ]
 dev-mypy = [
   "mypy == 1.5.1",
-  "grpc-stubs == 1.53.0.2",
+  "grpc-stubs == 1.53.0.5",
   "types-Markdown == 3.4.2.10",
   # For checking the noxfile, docs/ script, and tests
   "frequenz-api-reporting[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
 dev-noxfile = [
   "nox == 2023.4.22",
   "frequenz-repo-config[api] == 0.7.0",
```

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/annotations.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/auth.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/auth.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/backend.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/backend.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/billing.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/billing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/client.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/client.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/config_change.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/config_change.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/consumer.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/consumer.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/context.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/control.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/control.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/distribution.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/distribution.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/documentation.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/documentation.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/endpoint.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/endpoint.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/field_behavior.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/field_behavior.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/http.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/httpbody.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/httpbody.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/label.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/label.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/launch_stage.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/launch_stage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/log.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/log.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/logging.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/logging.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/metric.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/metric.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/monitored_resource.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/monitored_resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/monitoring.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/monitoring.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/quota.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/quota.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/resource.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/routing.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/routing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/service.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/service.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/source_info.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/source_info.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/system_parameter.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/system_parameter.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/usage.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/api/usage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/cloud/extended_operations.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/cloud/extended_operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/v1/options.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/iam/v1/options.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/v1/policy.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/iam/v1/policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/logging/type/http_request.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/logging/type/http_request.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/logging/type/log_severity.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/logging/type/log_severity.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/longrunning/operations.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/longrunning/operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/rpc/code.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/rpc/code.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/rpc/error_details.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/rpc/error_details.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/rpc/status.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/rpc/status.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/calendar_period.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/calendar_period.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/color.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/color.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/date.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/date.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/datetime.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/datetime.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/dayofweek.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/dayofweek.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/expr.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/expr.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/fraction.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/fraction.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/latlng.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/latlng.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/money.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/money.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/month.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/month.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/postal_address.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/postal_address.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/quaternion.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/quaternion.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/timeofday.proto` & `frequenz-api-reporting-0.3.0/submodules/api-common-protos/google/type/timeofday.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto` & `frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/location.proto` & `frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/location.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto` & `frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto` & `frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_area.proto` & `frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_area.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_duration.proto` & `frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_duration.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/location.proto` & `frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/location.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/energy.proto` & `frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/energy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/price.proto` & `frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/price.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/metric_sample.proto` & `frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/metric_sample.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/battery.proto` & `frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/battery.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/components.proto` & `frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/components.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto` & `frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/fuse.proto` & `frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/fuse.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/grid.proto` & `frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/grid.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/inverter.proto` & `frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/inverter.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/transformer.proto` & `frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/transformer.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/lifetime.proto` & `frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/lifetime.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/microgrid.proto` & `frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/microgrid.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto` & `frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_info.proto` & `frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_info.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto` & `frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/types/decimal.proto` & `frequenz-api-reporting-0.3.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/types/decimal.proto`

 * *Files identical despite different names*

