# Comparing `tmp/pilot-platform-common-1.0.0.tar.gz` & `tmp/pilot-platform-common-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilot-platform-common-1.0.0.tar", last modified: Fri May 24 16:18:06 2024, max compression
+gzip compressed data, was "pilot-platform-common-1.0.1.tar", last modified: Mon May 27 20:10:51 2024, max compression
```

## Comparing `pilot-platform-common-1.0.0.tar` & `pilot-platform-common-1.0.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.722060 pilot-platform-common-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-24 16:18:06.722060 pilot-platform-common-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.714060 pilot-platform-common-1.0.0/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.714060 pilot-platform-common-1.0.0/common/geid/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/geid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/geid/geid_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.714060 pilot-platform-common-1.0.0/common/jwt_handler/
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/jwt_handler/JWTHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/jwt_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/jwt_handler/jwt_handler_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/jwt_handler/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.718060 pilot-platform-common-1.0.0/common/logging/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/logging/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/logging/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.718060 pilot-platform-common-1.0.0/common/models/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/models/config_center_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/models/service_id_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.718060 pilot-platform-common-1.0.0/common/object_storage_adaptor/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/object_storage_adaptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/object_storage_adaptor/base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/object_storage_adaptor/boto3_admin_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17073 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/object_storage_adaptor/boto3_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/object_storage_adaptor/minio_policy_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.718060 pilot-platform-common-1.0.0/common/permissions/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/permissions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/permissions/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/permissions/permissions_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/permissions/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.718060 pilot-platform-common-1.0.0/common/project/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/project/project_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/project/project_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.718060 pilot-platform-common-1.0.0/common/services/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/services/auth_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.718060 pilot-platform-common-1.0.0/common/vault/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/vault/vault_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/vault/vault_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.718060 pilot-platform-common-1.0.0/pilot_platform_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-24 16:18:06.000000 pilot-platform-common-1.0.0/pilot_platform_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-24 16:18:06.000000 pilot-platform-common-1.0.0/pilot_platform_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 16:18:06.000000 pilot-platform-common-1.0.0/pilot_platform_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-24 16:18:06.000000 pilot-platform-common-1.0.0/pilot_platform_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 16:18:06.000000 pilot-platform-common-1.0.0/pilot_platform_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 16:18:06.722060 pilot-platform-common-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.722060 pilot-platform-common-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.722060 pilot-platform-common-1.0.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/fixtures/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/fixtures/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.722060 pilot-platform-common-1.0.0/tests/permissions/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/permissions/test_auth_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    19843 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/permissions/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/permissions/test_permissions_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/test_geid_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/test_jwt_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/test_project_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/test_vault_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:10:51.714830 pilot-platform-common-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-27 20:10:51.714830 pilot-platform-common-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:10:51.702830 pilot-platform-common-1.0.1/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:10:51.706830 pilot-platform-common-1.0.1/common/geid/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/geid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/geid/geid_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:10:51.706830 pilot-platform-common-1.0.1/common/jwt_handler/
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/jwt_handler/JWTHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/jwt_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/jwt_handler/jwt_handler_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/jwt_handler/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:10:51.706830 pilot-platform-common-1.0.1/common/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/logging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/logging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:10:51.706830 pilot-platform-common-1.0.1/common/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/models/config_center_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/models/service_id_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:10:51.706830 pilot-platform-common-1.0.1/common/object_storage_adaptor/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/object_storage_adaptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/object_storage_adaptor/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/object_storage_adaptor/boto3_admin_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17073 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/object_storage_adaptor/boto3_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/object_storage_adaptor/minio_policy_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:10:51.706830 pilot-platform-common-1.0.1/common/permissions/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/permissions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/permissions/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/permissions/permissions_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/permissions/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:10:51.710830 pilot-platform-common-1.0.1/common/project/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/project/project_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/project/project_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:10:51.710830 pilot-platform-common-1.0.1/common/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/services/auth_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:10:51.710830 pilot-platform-common-1.0.1/common/vault/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/vault/vault_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/common/vault/vault_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:10:51.710830 pilot-platform-common-1.0.1/pilot_platform_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-27 20:10:51.000000 pilot-platform-common-1.0.1/pilot_platform_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-27 20:10:51.000000 pilot-platform-common-1.0.1/pilot_platform_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:10:51.000000 pilot-platform-common-1.0.1/pilot_platform_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-27 20:10:51.000000 pilot-platform-common-1.0.1/pilot_platform_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 20:10:51.000000 pilot-platform-common-1.0.1/pilot_platform_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:10:51.714830 pilot-platform-common-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:10:51.710830 pilot-platform-common-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:10:51.710830 pilot-platform-common-1.0.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/tests/fixtures/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/tests/fixtures/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:10:51.710830 pilot-platform-common-1.0.1/tests/permissions/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/tests/permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/tests/permissions/test_auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19843 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/tests/permissions/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/tests/permissions/test_permissions_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/tests/test_geid_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/tests/test_jwt_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/tests/test_project_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-27 20:09:54.000000 pilot-platform-common-1.0.1/tests/test_vault_client.py
```

### Comparing `pilot-platform-common-1.0.0/PKG-INFO` & `pilot-platform-common-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilot-platform-common
-Version: 1.0.0
+Version: 1.0.1
 Summary: Generates entity ID and connects with Vault (secret engine) to retrieve credentials
 Author: Indoc Systems
 Author-email: etaylor@indocresearch.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `pilot-platform-common-1.0.0/README.md` & `pilot-platform-common-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/common/__init__.py` & `pilot-platform-common-1.0.1/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/common/geid/geid_client.py` & `pilot-platform-common-1.0.1/common/geid/geid_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/common/jwt_handler/JWTHandler.py` & `pilot-platform-common-1.0.1/common/jwt_handler/JWTHandler.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/common/jwt_handler/models.py` & `pilot-platform-common-1.0.1/common/jwt_handler/models.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/common/logging/formatter.py` & `pilot-platform-common-1.0.1/common/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/common/logging/logging.py` & `pilot-platform-common-1.0.1/common/logging/logging.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/common/models/config_center_policy.py` & `pilot-platform-common-1.0.1/common/models/config_center_policy.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/common/object_storage_adaptor/base_client.py` & `pilot-platform-common-1.0.1/common/object_storage_adaptor/base_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/common/object_storage_adaptor/boto3_admin_client.py` & `pilot-platform-common-1.0.1/common/object_storage_adaptor/boto3_admin_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/common/object_storage_adaptor/boto3_client.py` & `pilot-platform-common-1.0.1/common/object_storage_adaptor/boto3_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/common/object_storage_adaptor/minio_policy_client.py` & `pilot-platform-common-1.0.1/common/object_storage_adaptor/minio_policy_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/common/permissions/exceptions.py` & `pilot-platform-common-1.0.1/common/permissions/exceptions.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/common/permissions/permissions.py` & `pilot-platform-common-1.0.1/common/permissions/permissions.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/common/permissions/permissions_manager.py` & `pilot-platform-common-1.0.1/common/permissions/permissions_manager.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/common/permissions/schemas.py` & `pilot-platform-common-1.0.1/common/permissions/schemas.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/common/project/project_client.py` & `pilot-platform-common-1.0.1/common/project/project_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/common/project/project_exceptions.py` & `pilot-platform-common-1.0.1/common/project/project_exceptions.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/common/services/auth_client.py` & `pilot-platform-common-1.0.1/common/services/auth_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/common/vault/vault_client.py` & `pilot-platform-common-1.0.1/common/vault/vault_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/pilot_platform_common.egg-info/PKG-INFO` & `pilot-platform-common-1.0.1/pilot_platform_common.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilot-platform-common
-Version: 1.0.0
+Version: 1.0.1
 Summary: Generates entity ID and connects with Vault (secret engine) to retrieve credentials
 Author: Indoc Systems
 Author-email: etaylor@indocresearch.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `pilot-platform-common-1.0.0/pilot_platform_common.egg-info/SOURCES.txt` & `pilot-platform-common-1.0.1/pilot_platform_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/pyproject.toml` & `pilot-platform-common-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "common"
-version = "1.0.0"
+version = "1.0.1"
 description = ""
 authors = ["Indoc Systems"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = ">=0.19.1"
 python-json-logger = ">= 0.1.11, <= 2.02"
```

### Comparing `pilot-platform-common-1.0.0/setup.py` & `pilot-platform-common-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setuptools.setup(
     name='pilot-platform-common',
-    version='1.0.0',
+    version='1.0.1',
     author='Indoc Systems',
     author_email='etaylor@indocresearch.org',
     description='Generates entity ID and connects with Vault (secret engine) to retrieve credentials',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.9',
     install_requires=[
-        'python-dotenv==0.19.1',
+        'python-dotenv>=0.19.1',
         'httpx>=0.23.0,<0.27.0',
         'redis>=4.5.0,<5.0.0',
         'aioboto3==9.6.0',
         'xmltodict==0.13.0',
         'minio==7.1.8',
         'python-json-logger==2.0.2',
         'pyjwt==2.6.0',
```

### Comparing `pilot-platform-common-1.0.0/tests/conftest.py` & `pilot-platform-common-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/tests/fixtures/metadata.py` & `pilot-platform-common-1.0.1/tests/fixtures/metadata.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/tests/permissions/test_auth_client.py` & `pilot-platform-common-1.0.1/tests/permissions/test_auth_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/tests/permissions/test_permissions.py` & `pilot-platform-common-1.0.1/tests/permissions/test_permissions.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/tests/permissions/test_permissions_manager.py` & `pilot-platform-common-1.0.1/tests/permissions/test_permissions_manager.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/tests/test_formatter.py` & `pilot-platform-common-1.0.1/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/tests/test_geid_client.py` & `pilot-platform-common-1.0.1/tests/test_geid_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/tests/test_jwt_handler.py` & `pilot-platform-common-1.0.1/tests/test_jwt_handler.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/tests/test_logging.py` & `pilot-platform-common-1.0.1/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/tests/test_project_client.py` & `pilot-platform-common-1.0.1/tests/test_project_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-1.0.0/tests/test_vault_client.py` & `pilot-platform-common-1.0.1/tests/test_vault_client.py`

 * *Files identical despite different names*

