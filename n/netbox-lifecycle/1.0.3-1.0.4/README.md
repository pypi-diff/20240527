# Comparing `tmp/netbox_lifecycle-1.0.3.tar.gz` & `tmp/netbox_lifecycle-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_lifecycle-1.0.3.tar", last modified: Tue May  7 18:55:08 2024, max compression
+gzip compressed data, was "netbox_lifecycle-1.0.4.tar", last modified: Mon May 27 19:12:06 2024, max compression
```

## Comparing `netbox_lifecycle-1.0.3.tar` & `netbox_lifecycle-1.0.4.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.136794 netbox_lifecycle-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-07 18:55:08.136794 netbox_lifecycle-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.124794 netbox_lifecycle-1.0.3/netbox_lifecycle/
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.124794 netbox_lifecycle-1.0.3/netbox_lifecycle/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.128794 netbox_lifecycle-1.0.3/netbox_lifecycle/api/nested_serializers/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/nested_serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/nested_serializers/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/nested_serializers/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/nested_serializers/license.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.128794 netbox_lifecycle-1.0.3/netbox_lifecycle/api/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/serializers/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/serializers/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/serializers/license.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.128794 netbox_lifecycle-1.0.3/netbox_lifecycle/api/views/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/views/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/views/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/api/views/license.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.128794 netbox_lifecycle-1.0.3/netbox_lifecycle/filtersets/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/filtersets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/filtersets/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/filtersets/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/filtersets/license.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.128794 netbox_lifecycle-1.0.3/netbox_lifecycle/forms/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/forms/bulk_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/forms/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/forms/model_forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.132794 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0002_license_licenseassignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0003_remove_supportcontract_devices_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0004_supportcontractassignment_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0005_remove_supportcontract_manufacturer_supportsku_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0006_alter_supportcontractassignment_assigned_object_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0007_alter_hardwarelifecycle_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0008_alter_supportcontractassignment_contract_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0009_alter_licenseassignment_device.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0010_licenseassignment_quantity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0011_alter_supportcontractassignment.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.132794 netbox_lifecycle-1.0.3/netbox_lifecycle/models/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/models/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/models/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/models/license.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/models/netbox_polymprohic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.132794 netbox_lifecycle-1.0.3/netbox_lifecycle/tables/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/tables/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/tables/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/tables/license.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.124794 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.136794 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.136794 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/generic/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/generic/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/hardwarelifecycle.html
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/hardwarelifecycle_edit.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.136794 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/license/
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/license/assignments.html
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/license.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.136794 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/supportcontract/
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/supportcontract/assignments.html
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/supportcontract.html
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/supportcontractassignment_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/supportsku.html
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/vendor.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.136794 netbox_lifecycle-1.0.3/netbox_lifecycle/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.136794 netbox_lifecycle-1.0.3/netbox_lifecycle/views/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/views/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/views/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/netbox_lifecycle/views/license.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:55:08.136794 netbox_lifecycle-1.0.3/netbox_lifecycle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-07 18:55:08.000000 netbox_lifecycle-1.0.3/netbox_lifecycle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-07 18:55:08.000000 netbox_lifecycle-1.0.3/netbox_lifecycle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:55:08.000000 netbox_lifecycle-1.0.3/netbox_lifecycle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:55:08.000000 netbox_lifecycle-1.0.3/netbox_lifecycle.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 18:55:08.000000 netbox_lifecycle-1.0.3/netbox_lifecycle.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 18:55:08.136794 netbox_lifecycle-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-07 18:55:03.000000 netbox_lifecycle-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:12:06.624480 netbox_lifecycle-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-27 19:12:06.624480 netbox_lifecycle-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:12:06.612480 netbox_lifecycle-1.0.4/netbox_lifecycle/
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:12:06.612480 netbox_lifecycle-1.0.4/netbox_lifecycle/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:12:06.616480 netbox_lifecycle-1.0.4/netbox_lifecycle/api/nested_serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/api/nested_serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/api/nested_serializers/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/api/nested_serializers/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/api/nested_serializers/license.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:12:06.616480 netbox_lifecycle-1.0.4/netbox_lifecycle/api/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/api/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/api/serializers/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/api/serializers/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/api/serializers/license.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:12:06.616480 netbox_lifecycle-1.0.4/netbox_lifecycle/api/views/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/api/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/api/views/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/api/views/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/api/views/license.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:12:06.616480 netbox_lifecycle-1.0.4/netbox_lifecycle/filtersets/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/filtersets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/filtersets/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/filtersets/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/filtersets/license.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:12:06.616480 netbox_lifecycle-1.0.4/netbox_lifecycle/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/forms/bulk_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/forms/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/forms/model_forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:12:06.620480 netbox_lifecycle-1.0.4/netbox_lifecycle/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/migrations/0002_license_licenseassignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/migrations/0003_remove_supportcontract_devices_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/migrations/0004_supportcontractassignment_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/migrations/0005_remove_supportcontract_manufacturer_supportsku_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/migrations/0006_alter_supportcontractassignment_assigned_object_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/migrations/0007_alter_hardwarelifecycle_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/migrations/0008_alter_supportcontractassignment_contract_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/migrations/0009_alter_licenseassignment_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/migrations/0010_licenseassignment_quantity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/migrations/0011_alter_supportcontractassignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:12:06.620480 netbox_lifecycle-1.0.4/netbox_lifecycle/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/models/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/models/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/models/license.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/models/netbox_polymprohic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:12:06.620480 netbox_lifecycle-1.0.4/netbox_lifecycle/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/tables/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/tables/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/tables/license.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:12:06.612480 netbox_lifecycle-1.0.4/netbox_lifecycle/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:12:06.624480 netbox_lifecycle-1.0.4/netbox_lifecycle/templates/netbox_lifecycle/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:12:06.624480 netbox_lifecycle-1.0.4/netbox_lifecycle/templates/netbox_lifecycle/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/templates/netbox_lifecycle/generic/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/templates/netbox_lifecycle/hardwarelifecycle.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/templates/netbox_lifecycle/hardwarelifecycle_edit.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:12:06.624480 netbox_lifecycle-1.0.4/netbox_lifecycle/templates/netbox_lifecycle/license/
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/templates/netbox_lifecycle/license/assignments.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/templates/netbox_lifecycle/license.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:12:06.624480 netbox_lifecycle-1.0.4/netbox_lifecycle/templates/netbox_lifecycle/supportcontract/
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/templates/netbox_lifecycle/supportcontract/assignments.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/templates/netbox_lifecycle/supportcontract.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/templates/netbox_lifecycle/supportcontractassignment_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/templates/netbox_lifecycle/supportsku.html
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/templates/netbox_lifecycle/vendor.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:12:06.624480 netbox_lifecycle-1.0.4/netbox_lifecycle/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:12:06.624480 netbox_lifecycle-1.0.4/netbox_lifecycle/views/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/views/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/views/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/netbox_lifecycle/views/license.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:12:06.624480 netbox_lifecycle-1.0.4/netbox_lifecycle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-27 19:12:06.000000 netbox_lifecycle-1.0.4/netbox_lifecycle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-27 19:12:06.000000 netbox_lifecycle-1.0.4/netbox_lifecycle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:12:06.000000 netbox_lifecycle-1.0.4/netbox_lifecycle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:12:06.000000 netbox_lifecycle-1.0.4/netbox_lifecycle.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 19:12:06.000000 netbox_lifecycle-1.0.4/netbox_lifecycle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 19:12:06.624480 netbox_lifecycle-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-27 19:12:03.000000 netbox_lifecycle-1.0.4/setup.py
```

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/__init__.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/api/nested_serializers/contract.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/api/nested_serializers/contract.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/api/nested_serializers/hardware.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/api/nested_serializers/hardware.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/api/nested_serializers/license.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/api/nested_serializers/license.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/api/serializers/contract.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/api/serializers/contract.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/api/serializers/hardware.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/api/serializers/hardware.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/api/serializers/license.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/api/serializers/license.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/api/views/contract.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/api/views/contract.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/api/views/license.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/api/views/license.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/filtersets/contract.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/filtersets/contract.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/filtersets/hardware.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/filtersets/hardware.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/filtersets/license.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/filtersets/license.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/forms/bulk_edit.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/forms/bulk_edit.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/forms/filtersets.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/forms/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/forms/model_forms.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/forms/model_forms.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0001_initial.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0002_license_licenseassignment.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/migrations/0002_license_licenseassignment.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0003_remove_supportcontract_devices_and_more.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/migrations/0003_remove_supportcontract_devices_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0004_supportcontractassignment_and_more.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/migrations/0004_supportcontractassignment_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0005_remove_supportcontract_manufacturer_supportsku_and_more.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/migrations/0005_remove_supportcontract_manufacturer_supportsku_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0006_alter_supportcontractassignment_assigned_object_type.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/migrations/0006_alter_supportcontractassignment_assigned_object_type.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0007_alter_hardwarelifecycle_options_and_more.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/migrations/0007_alter_hardwarelifecycle_options_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0008_alter_supportcontractassignment_contract_and_more.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/migrations/0008_alter_supportcontractassignment_contract_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0009_alter_licenseassignment_device.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/migrations/0009_alter_licenseassignment_device.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/migrations/0011_alter_supportcontractassignment.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/migrations/0011_alter_supportcontractassignment.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/models/contract.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/models/contract.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/models/hardware.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/models/hardware.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/models/license.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/models/license.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/navigation.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/tables/contract.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/tables/contract.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/tables/hardware.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/tables/hardware.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/tables/license.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/tables/license.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/hardwarelifecycle.html` & `netbox_lifecycle-1.0.4/netbox_lifecycle/templates/netbox_lifecycle/hardwarelifecycle.html`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/hardwarelifecycle_edit.html` & `netbox_lifecycle-1.0.4/netbox_lifecycle/templates/netbox_lifecycle/hardwarelifecycle_edit.html`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/license/assignments.html` & `netbox_lifecycle-1.0.4/netbox_lifecycle/templates/netbox_lifecycle/license/assignments.html`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/license.html` & `netbox_lifecycle-1.0.4/netbox_lifecycle/templates/netbox_lifecycle/license.html`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/supportcontract/assignments.html` & `netbox_lifecycle-1.0.4/netbox_lifecycle/templates/netbox_lifecycle/supportcontract/assignments.html`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/supportcontract.html` & `netbox_lifecycle-1.0.4/netbox_lifecycle/templates/netbox_lifecycle/supportcontract.html`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/supportcontractassignment_edit.html` & `netbox_lifecycle-1.0.4/netbox_lifecycle/templates/netbox_lifecycle/supportcontractassignment_edit.html`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/supportsku.html` & `netbox_lifecycle-1.0.4/netbox_lifecycle/templates/netbox_lifecycle/supportsku.html`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/templates/netbox_lifecycle/vendor.html` & `netbox_lifecycle-1.0.4/netbox_lifecycle/templates/netbox_lifecycle/vendor.html`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/tests/test_models.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/urls.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/views/contract.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/views/contract.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,15 +97,19 @@
 @register_model_view(SupportContract, name='assignments')
 class SupportContractAssignmentView(ObjectChildrenView):
     template_name = 'netbox_lifecycle/supportcontract/assignments.html'
     queryset = SupportContract.objects.all()
     child_model = SupportContractAssignment
     table = SupportContractAssignmentTable
     filterset = SupportContractAssignmentFilterSet
-    actions = ['add', 'edit', 'delete']
+    actions = {
+        'add': {'add'},
+        'edit': {'change'},
+        'delete': {'delete'}
+    }
     tab = ViewTab(
         label='Assignments',
         badge=lambda obj: SupportContractAssignment.objects.filter(contract=obj).count(),
     )
 
     def get_children(self, request, parent):
         return self.child_model.objects.filter(contract=parent)
@@ -136,15 +140,21 @@
 
 @register_model_view(SupportContractAssignment, name='list')
 class SupportContractAssignmentListView(ObjectListView):
     queryset = SupportContractAssignment.objects.all()
     table = SupportContractAssignmentTable
     filterset = SupportContractAssignmentFilterSet
     filterset_form = SupportContractAssignmentFilterForm
-    actions = ['add', 'edit', 'delete', 'bulk_edit', 'bulk_delete']
+    actions = {
+        'add': {'add'},
+        'edit': {'change'},
+        'delete': {'delete'},
+        'bulk_edit': {'change'},
+        'bulk_delete': {'delete'}
+    }
 
 
 class SupportContractAssignmentBulkEditView(BulkEditView):
     queryset = SupportContractAssignment.objects.all()
     filterset = SupportContractAssignmentFilterSet
     table = SupportContractAssignmentTable
     form = SupportContractAssignmentBulkEditForm
```

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/views/hardware.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/views/hardware.py`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle/views/license.py` & `netbox_lifecycle-1.0.4/netbox_lifecycle/views/license.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,15 +50,19 @@
 class LicenseAssignmentView(ObjectChildrenView):
     template_name = 'netbox_lifecycle/license/assignments.html'
     queryset = License.objects.all()
     child_model = LicenseAssignment
     table = LicenseAssignmentTable
     filterset = LicenseAssignmentFilterSet
     viewname = None
-    actions = ['add', 'edit', 'delete']
+    actions = {
+        'add': {'add'},
+        'edit': {'change'},
+        'delete': {'delete'}
+    }
     tab = ViewTab(
         label='License Assignments',
         badge=lambda obj: LicenseAssignment.objects.filter(license=obj).count(),
     )
 
     def get_children(self, request, parent):
         return self.child_model.objects.filter(license=parent)
```

### Comparing `netbox_lifecycle-1.0.3/netbox_lifecycle.egg-info/SOURCES.txt` & `netbox_lifecycle-1.0.4/netbox_lifecycle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox_lifecycle-1.0.3/setup.py` & `netbox_lifecycle-1.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='netbox-lifecycle',
-    version='1.0.3',
+    version='1.0.4',
     description='NetBox Lifecycle',
     long_description='NetBox Support Contract and EOL/EOS management',
     url='https://github.com/dansheps/netbox-lifecycle/',
     download_url='https://pypi.org/project/netbox-lifecycle/',
     author='Daniel Sheppard',
     author_email='dans@dansheps.com',
     maintainer='Daniel Sheppard',
```

