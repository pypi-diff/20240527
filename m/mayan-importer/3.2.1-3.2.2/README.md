# Comparing `tmp/mayan-importer-3.2.1.tar.gz` & `tmp/mayan-importer-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mayan-importer-3.2.1.tar", last modified: Sat May  4 21:14:56 2024, max compression
+gzip compressed data, was "mayan-importer-3.2.2.tar", last modified: Thu May  9 22:14:04 2024, max compression
```

## Comparing `mayan-importer-3.2.1.tar` & `mayan-importer-3.2.2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-04 21:14:56.684674 mayan-importer-3.2.1/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6690 2024-05-04 20:15:00.000000 mayan-importer-3.2.1/HISTORY.rst
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      555 2020-10-02 10:42:37.000000 mayan-importer-3.2.1/LICENSE
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       39 2020-10-02 10:42:37.000000 mayan-importer-3.2.1/MANIFEST.in
--rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9582 2024-05-04 21:14:56.684674 mayan-importer-3.2.1/PKG-INFO
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1628 2020-10-02 10:42:37.000000 mayan-importer-3.2.1/README.rst
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-04 21:14:56.676674 mayan-importer-3.2.1/importer/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       49 2020-10-02 10:42:37.000000 mayan-importer-3.2.1/importer/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      405 2024-04-01 10:00:47.000000 mayan-importer-3.2.1/importer/admin.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4643 2024-04-01 10:00:47.000000 mayan-importer-3.2.1/importer/api_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7817 2024-05-04 06:47:22.000000 mayan-importer-3.2.1/importer/apps.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7165 2024-05-03 23:02:13.000000 mayan-importer-3.2.1/importer/classes.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      145 2024-04-01 10:00:47.000000 mayan-importer-3.2.1/importer/dependencies.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1729 2024-04-01 10:00:47.000000 mayan-importer-3.2.1/importer/events.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       93 2024-04-01 10:00:47.000000 mayan-importer-3.2.1/importer/exceptions.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-04 21:14:56.676674 mayan-importer-3.2.1/importer/forms/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 06:18:39.000000 mayan-importer-3.2.1/importer/forms/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      327 2024-05-04 21:13:39.000000 mayan-importer-3.2.1/importer/forms/filer_forms.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      431 2024-05-03 08:05:46.000000 mayan-importer-3.2.1/importer/forms/form_mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      949 2024-05-03 06:38:56.000000 mayan-importer-3.2.1/importer/forms/import_setup_forms.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      591 2024-05-03 06:40:26.000000 mayan-importer-3.2.1/importer/forms/import_setup_item_forms.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-04 21:14:56.677674 mayan-importer-3.2.1/importer/icons/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-05-02 06:30:26.000000 mayan-importer-3.2.1/importer/icons/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      222 2024-05-03 06:38:56.000000 mayan-importer-3.2.1/importer/icons/import_setup_filer_icons.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      914 2024-05-03 06:38:56.000000 mayan-importer-3.2.1/importer/icons/import_setup_icons.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      710 2024-05-03 06:38:56.000000 mayan-importer-3.2.1/importer/icons/import_setup_item_icons.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8715 2024-05-03 08:31:33.000000 mayan-importer-3.2.1/importer/importers.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-04 21:14:56.678674 mayan-importer-3.2.1/importer/links/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-05-02 06:05:24.000000 mayan-importer-3.2.1/importer/links/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      974 2024-05-03 06:38:56.000000 mayan-importer-3.2.1/importer/links/import_setup_filer_links.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2534 2024-05-03 06:38:56.000000 mayan-importer-3.2.1/importer/links/import_setup_item_links.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3461 2024-05-03 06:37:19.000000 mayan-importer-3.2.1/importer/links/import_setup_links.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1205 2024-05-02 22:28:59.000000 mayan-importer-3.2.1/importer/literals.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-04 21:14:56.681674 mayan-importer-3.2.1/importer/migrations/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4126 2020-10-02 10:42:37.000000 mayan-importer-3.2.1/importer/migrations/0001_initial.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1475 2020-10-02 10:42:37.000000 mayan-importer-3.2.1/importer/migrations/0002_auto_20200908_0458.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      669 2020-10-02 10:42:37.000000 mayan-importer-3.2.1/importer/migrations/0003_importsetup_metadata_map.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      795 2023-04-12 05:57:59.000000 mayan-importer-3.2.1/importer/migrations/0004_auto_20200908_0853.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      607 2023-04-12 05:57:59.000000 mayan-importer-3.2.1/importer/migrations/0005_importsetup_state.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      333 2023-04-12 05:57:59.000000 mayan-importer-3.2.1/importer/migrations/0006_auto_20200924_0802.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      428 2023-04-12 05:57:59.000000 mayan-importer-3.2.1/importer/migrations/0007_auto_20200924_0802.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      603 2023-04-12 05:57:59.000000 mayan-importer-3.2.1/importer/migrations/0008_auto_20200924_0903.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2451 2023-04-12 05:57:59.000000 mayan-importer-3.2.1/importer/migrations/0009_importsetupaction.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      287 2024-05-02 22:00:10.000000 mayan-importer-3.2.1/importer/migrations/0010_remove_importsetup_metadata_map.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      568 2023-04-12 05:57:59.000000 mayan-importer-3.2.1/importer/migrations/0011_auto_20201004_0042.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      522 2023-04-12 05:57:59.000000 mayan-importer-3.2.1/importer/migrations/0012_importsetupitem_documents.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1796 2023-04-12 05:57:59.000000 mayan-importer-3.2.1/importer/migrations/0013_auto_20201225_0155.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      396 2023-04-12 05:57:59.000000 mayan-importer-3.2.1/importer/migrations/0014_auto_20201227_0610.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      848 2023-04-12 05:57:59.000000 mayan-importer-3.2.1/importer/migrations/0015_auto_20220901_0932.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      526 2023-04-12 05:57:59.000000 mayan-importer-3.2.1/importer/migrations/0016_importsetup_item_time_buffer.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      239 2024-04-01 10:00:47.000000 mayan-importer-3.2.1/importer/migrations/0017_delete_importsetuplog.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1064 2024-04-01 10:00:47.000000 mayan-importer-3.2.1/importer/migrations/0018_auto_20240401_0808.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1326 2024-04-02 11:02:22.000000 mayan-importer-3.2.1/importer/migrations/0019_auto_20240402_1101.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1449 2024-05-02 19:09:03.000000 mayan-importer-3.2.1/importer/migrations/0020_auto_20240502_1907.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2344 2024-05-04 19:37:51.000000 mayan-importer-3.2.1/importer/migrations/0021_migrate_state_codes.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1063 2024-05-03 08:53:58.000000 mayan-importer-3.2.1/importer/migrations/0022_auto_20240503_0853.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2020-10-02 10:42:37.000000 mayan-importer-3.2.1/importer/migrations/__init__.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-04 21:14:56.681674 mayan-importer-3.2.1/importer/models/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       91 2024-05-04 07:48:41.000000 mayan-importer-3.2.1/importer/models/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4172 2024-05-03 08:45:32.000000 mayan-importer-3.2.1/importer/models/import_setup_item_model_mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2945 2024-05-03 07:37:19.000000 mayan-importer-3.2.1/importer/models/import_setup_item_models.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6055 2024-05-04 06:55:03.000000 mayan-importer-3.2.1/importer/models/import_setup_model_mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2421 2024-05-04 06:55:15.000000 mayan-importer-3.2.1/importer/models/import_setup_models.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3256 2024-05-04 19:50:33.000000 mayan-importer-3.2.1/importer/models/model_mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1386 2024-04-01 10:00:47.000000 mayan-importer-3.2.1/importer/permissions.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1197 2024-04-01 10:00:47.000000 mayan-importer-3.2.1/importer/queues.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3473 2024-04-01 10:00:47.000000 mayan-importer-3.2.1/importer/serializers.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2314 2024-05-03 08:30:22.000000 mayan-importer-3.2.1/importer/tasks.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-04 21:14:56.682674 mayan-importer-3.2.1/importer/tests/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:00:47.000000 mayan-importer-3.2.1/importer/tests/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1650 2024-05-03 08:30:22.000000 mayan-importer-3.2.1/importer/tests/importers.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      695 2024-05-04 07:00:01.000000 mayan-importer-3.2.1/importer/tests/literals.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1294 2024-05-04 07:47:44.000000 mayan-importer-3.2.1/importer/tests/test_filer_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8230 2024-05-04 06:59:12.000000 mayan-importer-3.2.1/importer/tests/test_import_setup_api.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7720 2024-05-04 07:46:59.000000 mayan-importer-3.2.1/importer/tests/test_import_setup_item_api.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    11484 2024-05-04 07:46:59.000000 mayan-importer-3.2.1/importer/tests/test_import_setup_item_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6309 2024-05-04 07:46:59.000000 mayan-importer-3.2.1/importer/tests/test_import_setup_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5787 2024-05-04 06:26:52.000000 mayan-importer-3.2.1/importer/urls.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-04 21:14:56.683674 mayan-importer-3.2.1/importer/views/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2023-04-12 05:57:59.000000 mayan-importer-3.2.1/importer/views/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3693 2024-05-04 21:13:39.000000 mayan-importer-3.2.1/importer/views/import_setup_filer_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8134 2024-05-03 08:02:03.000000 mayan-importer-3.2.1/importer/views/import_setup_item_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     9643 2024-05-03 08:07:00.000000 mayan-importer-3.2.1/importer/views/import_setup_views.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-04 21:14:56.684674 mayan-importer-3.2.1/mayan_importer.egg-info/
--rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9582 2024-05-04 21:14:56.000000 mayan-importer-3.2.1/mayan_importer.egg-info/PKG-INFO
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2832 2024-05-04 21:14:56.000000 mayan-importer-3.2.1/mayan_importer.egg-info/SOURCES.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-05-04 21:14:56.000000 mayan-importer-3.2.1/mayan_importer.egg-info/dependency_links.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-05-04 21:14:56.000000 mayan-importer-3.2.1/mayan_importer.egg-info/not-zip-safe
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       16 2024-05-04 21:14:56.000000 mayan-importer-3.2.1/mayan_importer.egg-info/requires.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        9 2024-05-04 21:14:56.000000 mayan-importer-3.2.1/mayan_importer.egg-info/top_level.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      129 2024-05-04 21:14:56.685674 mayan-importer-3.2.1/setup.cfg
--rwxrwxr-x   0 rosarior  (1000) rosarior  (1000)     3038 2024-05-04 21:14:36.000000 mayan-importer-3.2.1/setup.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-09 22:14:04.611231 mayan-importer-3.2.2/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6690 2024-05-04 20:15:00.000000 mayan-importer-3.2.2/HISTORY.rst
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      555 2020-10-02 10:42:37.000000 mayan-importer-3.2.2/LICENSE
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       39 2020-10-02 10:42:37.000000 mayan-importer-3.2.2/MANIFEST.in
+-rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9582 2024-05-09 22:14:04.611231 mayan-importer-3.2.2/PKG-INFO
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1628 2020-10-02 10:42:37.000000 mayan-importer-3.2.2/README.rst
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-09 22:14:04.601231 mayan-importer-3.2.2/importer/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       49 2020-10-02 10:42:37.000000 mayan-importer-3.2.2/importer/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      405 2024-04-01 10:00:47.000000 mayan-importer-3.2.2/importer/admin.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4643 2024-04-01 10:00:47.000000 mayan-importer-3.2.2/importer/api_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7817 2024-05-04 06:47:22.000000 mayan-importer-3.2.2/importer/apps.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7165 2024-05-03 23:02:13.000000 mayan-importer-3.2.2/importer/classes.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      145 2024-04-01 10:00:47.000000 mayan-importer-3.2.2/importer/dependencies.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1729 2024-04-01 10:00:47.000000 mayan-importer-3.2.2/importer/events.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       93 2024-04-01 10:00:47.000000 mayan-importer-3.2.2/importer/exceptions.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-09 22:14:04.602231 mayan-importer-3.2.2/importer/forms/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 06:18:39.000000 mayan-importer-3.2.2/importer/forms/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      327 2024-05-04 21:13:39.000000 mayan-importer-3.2.2/importer/forms/filer_forms.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      431 2024-05-03 08:05:46.000000 mayan-importer-3.2.2/importer/forms/form_mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      949 2024-05-03 06:38:56.000000 mayan-importer-3.2.2/importer/forms/import_setup_forms.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      591 2024-05-03 06:40:26.000000 mayan-importer-3.2.2/importer/forms/import_setup_item_forms.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-09 22:14:04.602231 mayan-importer-3.2.2/importer/icons/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-05-02 06:30:26.000000 mayan-importer-3.2.2/importer/icons/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      222 2024-05-03 06:38:56.000000 mayan-importer-3.2.2/importer/icons/import_setup_filer_icons.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      914 2024-05-03 06:38:56.000000 mayan-importer-3.2.2/importer/icons/import_setup_icons.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      710 2024-05-03 06:38:56.000000 mayan-importer-3.2.2/importer/icons/import_setup_item_icons.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8715 2024-05-03 08:31:33.000000 mayan-importer-3.2.2/importer/importers.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-09 22:14:04.603231 mayan-importer-3.2.2/importer/links/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-05-02 06:05:24.000000 mayan-importer-3.2.2/importer/links/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      974 2024-05-03 06:38:56.000000 mayan-importer-3.2.2/importer/links/import_setup_filer_links.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2534 2024-05-03 06:38:56.000000 mayan-importer-3.2.2/importer/links/import_setup_item_links.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3461 2024-05-03 06:37:19.000000 mayan-importer-3.2.2/importer/links/import_setup_links.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1205 2024-05-02 22:28:59.000000 mayan-importer-3.2.2/importer/literals.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-09 22:14:04.607231 mayan-importer-3.2.2/importer/migrations/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4126 2020-10-02 10:42:37.000000 mayan-importer-3.2.2/importer/migrations/0001_initial.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1475 2020-10-02 10:42:37.000000 mayan-importer-3.2.2/importer/migrations/0002_auto_20200908_0458.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      669 2020-10-02 10:42:37.000000 mayan-importer-3.2.2/importer/migrations/0003_importsetup_metadata_map.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      795 2023-04-12 05:57:59.000000 mayan-importer-3.2.2/importer/migrations/0004_auto_20200908_0853.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      607 2023-04-12 05:57:59.000000 mayan-importer-3.2.2/importer/migrations/0005_importsetup_state.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      333 2023-04-12 05:57:59.000000 mayan-importer-3.2.2/importer/migrations/0006_auto_20200924_0802.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      428 2023-04-12 05:57:59.000000 mayan-importer-3.2.2/importer/migrations/0007_auto_20200924_0802.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      603 2023-04-12 05:57:59.000000 mayan-importer-3.2.2/importer/migrations/0008_auto_20200924_0903.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2451 2023-04-12 05:57:59.000000 mayan-importer-3.2.2/importer/migrations/0009_importsetupaction.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      287 2024-05-02 22:00:10.000000 mayan-importer-3.2.2/importer/migrations/0010_remove_importsetup_metadata_map.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      568 2023-04-12 05:57:59.000000 mayan-importer-3.2.2/importer/migrations/0011_auto_20201004_0042.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      522 2023-04-12 05:57:59.000000 mayan-importer-3.2.2/importer/migrations/0012_importsetupitem_documents.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1796 2023-04-12 05:57:59.000000 mayan-importer-3.2.2/importer/migrations/0013_auto_20201225_0155.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      396 2023-04-12 05:57:59.000000 mayan-importer-3.2.2/importer/migrations/0014_auto_20201227_0610.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      848 2023-04-12 05:57:59.000000 mayan-importer-3.2.2/importer/migrations/0015_auto_20220901_0932.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      526 2023-04-12 05:57:59.000000 mayan-importer-3.2.2/importer/migrations/0016_importsetup_item_time_buffer.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      239 2024-04-01 10:00:47.000000 mayan-importer-3.2.2/importer/migrations/0017_delete_importsetuplog.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1064 2024-04-01 10:00:47.000000 mayan-importer-3.2.2/importer/migrations/0018_auto_20240401_0808.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1326 2024-04-02 11:02:22.000000 mayan-importer-3.2.2/importer/migrations/0019_auto_20240402_1101.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1449 2024-05-02 19:09:03.000000 mayan-importer-3.2.2/importer/migrations/0020_auto_20240502_1907.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2344 2024-05-04 19:37:51.000000 mayan-importer-3.2.2/importer/migrations/0021_migrate_state_codes.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1063 2024-05-03 08:53:58.000000 mayan-importer-3.2.2/importer/migrations/0022_auto_20240503_0853.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2020-10-02 10:42:37.000000 mayan-importer-3.2.2/importer/migrations/__init__.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-09 22:14:04.607231 mayan-importer-3.2.2/importer/models/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       91 2024-05-04 07:48:41.000000 mayan-importer-3.2.2/importer/models/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4125 2024-05-09 22:12:02.000000 mayan-importer-3.2.2/importer/models/import_setup_item_model_mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2945 2024-05-03 07:37:19.000000 mayan-importer-3.2.2/importer/models/import_setup_item_models.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6055 2024-05-09 22:12:23.000000 mayan-importer-3.2.2/importer/models/import_setup_model_mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2421 2024-05-04 06:55:15.000000 mayan-importer-3.2.2/importer/models/import_setup_models.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3256 2024-05-04 19:50:33.000000 mayan-importer-3.2.2/importer/models/model_mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1386 2024-04-01 10:00:47.000000 mayan-importer-3.2.2/importer/permissions.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1197 2024-04-01 10:00:47.000000 mayan-importer-3.2.2/importer/queues.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3473 2024-04-01 10:00:47.000000 mayan-importer-3.2.2/importer/serializers.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2314 2024-05-03 08:30:22.000000 mayan-importer-3.2.2/importer/tasks.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-09 22:14:04.609231 mayan-importer-3.2.2/importer/tests/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:00:47.000000 mayan-importer-3.2.2/importer/tests/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1650 2024-05-03 08:30:22.000000 mayan-importer-3.2.2/importer/tests/importers.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      695 2024-05-04 07:00:01.000000 mayan-importer-3.2.2/importer/tests/literals.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1294 2024-05-04 07:47:44.000000 mayan-importer-3.2.2/importer/tests/test_filer_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8230 2024-05-04 06:59:12.000000 mayan-importer-3.2.2/importer/tests/test_import_setup_api.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7720 2024-05-04 07:46:59.000000 mayan-importer-3.2.2/importer/tests/test_import_setup_item_api.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    11484 2024-05-04 07:46:59.000000 mayan-importer-3.2.2/importer/tests/test_import_setup_item_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6309 2024-05-04 07:46:59.000000 mayan-importer-3.2.2/importer/tests/test_import_setup_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5787 2024-05-04 06:26:52.000000 mayan-importer-3.2.2/importer/urls.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-09 22:14:04.609231 mayan-importer-3.2.2/importer/views/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2023-04-12 05:57:59.000000 mayan-importer-3.2.2/importer/views/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3693 2024-05-04 21:13:39.000000 mayan-importer-3.2.2/importer/views/import_setup_filer_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8134 2024-05-03 08:02:03.000000 mayan-importer-3.2.2/importer/views/import_setup_item_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     9643 2024-05-03 08:07:00.000000 mayan-importer-3.2.2/importer/views/import_setup_views.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-09 22:14:04.610231 mayan-importer-3.2.2/mayan_importer.egg-info/
+-rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9582 2024-05-09 22:14:04.000000 mayan-importer-3.2.2/mayan_importer.egg-info/PKG-INFO
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2832 2024-05-09 22:14:04.000000 mayan-importer-3.2.2/mayan_importer.egg-info/SOURCES.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-05-09 22:14:04.000000 mayan-importer-3.2.2/mayan_importer.egg-info/dependency_links.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-05-09 22:14:04.000000 mayan-importer-3.2.2/mayan_importer.egg-info/not-zip-safe
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       16 2024-05-09 22:14:04.000000 mayan-importer-3.2.2/mayan_importer.egg-info/requires.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        9 2024-05-09 22:14:04.000000 mayan-importer-3.2.2/mayan_importer.egg-info/top_level.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      129 2024-05-09 22:14:04.611231 mayan-importer-3.2.2/setup.cfg
+-rwxrwxr-x   0 rosarior  (1000) rosarior  (1000)     3038 2024-05-09 22:12:45.000000 mayan-importer-3.2.2/setup.py
```

### Comparing `mayan-importer-3.2.1/HISTORY.rst` & `mayan-importer-3.2.2/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/LICENSE` & `mayan-importer-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/PKG-INFO` & `mayan-importer-3.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayan-importer
-Version: 3.2.1
+Version: 3.2.2
 Summary: Mayan EDMS importer
 Home-page: https://gitlab.com/mayan-edms/importer
 Author: Roberto Rosario
 Author-email: roberto.rosario@mayan-edms.com
 License: Apache 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mayan-importer-3.2.1/README.rst` & `mayan-importer-3.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/api_views.py` & `mayan-importer-3.2.2/importer/api_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/apps.py` & `mayan-importer-3.2.2/importer/apps.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/classes.py` & `mayan-importer-3.2.2/importer/classes.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/events.py` & `mayan-importer-3.2.2/importer/events.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/forms/import_setup_forms.py` & `mayan-importer-3.2.2/importer/forms/import_setup_forms.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/forms/import_setup_item_forms.py` & `mayan-importer-3.2.2/importer/forms/import_setup_item_forms.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/icons/import_setup_icons.py` & `mayan-importer-3.2.2/importer/icons/import_setup_icons.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/icons/import_setup_item_icons.py` & `mayan-importer-3.2.2/importer/icons/import_setup_item_icons.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/importers.py` & `mayan-importer-3.2.2/importer/importers.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/links/import_setup_filer_links.py` & `mayan-importer-3.2.2/importer/links/import_setup_filer_links.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/links/import_setup_item_links.py` & `mayan-importer-3.2.2/importer/links/import_setup_item_links.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/links/import_setup_links.py` & `mayan-importer-3.2.2/importer/links/import_setup_links.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/literals.py` & `mayan-importer-3.2.2/importer/literals.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/migrations/0001_initial.py` & `mayan-importer-3.2.2/importer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/migrations/0002_auto_20200908_0458.py` & `mayan-importer-3.2.2/importer/migrations/0002_auto_20200908_0458.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/migrations/0003_importsetup_metadata_map.py` & `mayan-importer-3.2.2/importer/migrations/0003_importsetup_metadata_map.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/migrations/0004_auto_20200908_0853.py` & `mayan-importer-3.2.2/importer/migrations/0004_auto_20200908_0853.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/migrations/0005_importsetup_state.py` & `mayan-importer-3.2.2/importer/migrations/0005_importsetup_state.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/migrations/0008_auto_20200924_0903.py` & `mayan-importer-3.2.2/importer/migrations/0008_auto_20200924_0903.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/migrations/0009_importsetupaction.py` & `mayan-importer-3.2.2/importer/migrations/0009_importsetupaction.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/migrations/0011_auto_20201004_0042.py` & `mayan-importer-3.2.2/importer/migrations/0011_auto_20201004_0042.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/migrations/0012_importsetupitem_documents.py` & `mayan-importer-3.2.2/importer/migrations/0012_importsetupitem_documents.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/migrations/0013_auto_20201225_0155.py` & `mayan-importer-3.2.2/importer/migrations/0013_auto_20201225_0155.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/migrations/0015_auto_20220901_0932.py` & `mayan-importer-3.2.2/importer/migrations/0015_auto_20220901_0932.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/migrations/0016_importsetup_item_time_buffer.py` & `mayan-importer-3.2.2/importer/migrations/0016_importsetup_item_time_buffer.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/migrations/0018_auto_20240401_0808.py` & `mayan-importer-3.2.2/importer/migrations/0018_auto_20240401_0808.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/migrations/0019_auto_20240402_1101.py` & `mayan-importer-3.2.2/importer/migrations/0019_auto_20240402_1101.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/migrations/0020_auto_20240502_1907.py` & `mayan-importer-3.2.2/importer/migrations/0020_auto_20240502_1907.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/migrations/0021_migrate_state_codes.py` & `mayan-importer-3.2.2/importer/migrations/0021_migrate_state_codes.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/migrations/0022_auto_20240503_0853.py` & `mayan-importer-3.2.2/importer/migrations/0022_auto_20240503_0853.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/models/import_setup_item_model_mixins.py` & `mayan-importer-3.2.2/importer/models/import_setup_item_model_mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 )
 
 
 class ImportSetupItemBusinessLogicMixin:
     @classmethod
     def get_process_allowed_state_list(self):
         return (
-            IMPORT_SETUP_ITEM_STATE_PROCESSED, IMPORT_SETUP_ITEM_STATE_ERROR,
-            IMPORT_SETUP_ITEM_STATE_NONE
+            IMPORT_SETUP_ITEM_STATE_ERROR, IMPORT_SETUP_ITEM_STATE_NONE
         )
 
     @property
     def data(self):
         return self.load_data()
 
     def do_check_valid(self):
```

### Comparing `mayan-importer-3.2.1/importer/models/import_setup_item_models.py` & `mayan-importer-3.2.2/importer/models/import_setup_item_models.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/models/import_setup_model_mixins.py` & `mayan-importer-3.2.2/importer/models/import_setup_model_mixins.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/models/import_setup_models.py` & `mayan-importer-3.2.2/importer/models/import_setup_models.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/models/model_mixins.py` & `mayan-importer-3.2.2/importer/models/model_mixins.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/permissions.py` & `mayan-importer-3.2.2/importer/permissions.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/queues.py` & `mayan-importer-3.2.2/importer/queues.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/serializers.py` & `mayan-importer-3.2.2/importer/serializers.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/tasks.py` & `mayan-importer-3.2.2/importer/tasks.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/tests/importers.py` & `mayan-importer-3.2.2/importer/tests/importers.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/tests/literals.py` & `mayan-importer-3.2.2/importer/tests/literals.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/tests/test_filer_views.py` & `mayan-importer-3.2.2/importer/tests/test_filer_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/tests/test_import_setup_api.py` & `mayan-importer-3.2.2/importer/tests/test_import_setup_api.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/tests/test_import_setup_item_api.py` & `mayan-importer-3.2.2/importer/tests/test_import_setup_item_api.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/tests/test_import_setup_item_views.py` & `mayan-importer-3.2.2/importer/tests/test_import_setup_item_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/tests/test_import_setup_views.py` & `mayan-importer-3.2.2/importer/tests/test_import_setup_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/urls.py` & `mayan-importer-3.2.2/importer/urls.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/views/import_setup_filer_views.py` & `mayan-importer-3.2.2/importer/views/import_setup_filer_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/views/import_setup_item_views.py` & `mayan-importer-3.2.2/importer/views/import_setup_item_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/importer/views/import_setup_views.py` & `mayan-importer-3.2.2/importer/views/import_setup_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/mayan_importer.egg-info/PKG-INFO` & `mayan-importer-3.2.2/mayan_importer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayan-importer
-Version: 3.2.1
+Version: 3.2.2
 Summary: Mayan EDMS importer
 Home-page: https://gitlab.com/mayan-edms/importer
 Author: Roberto Rosario
 Author-email: roberto.rosario@mayan-edms.com
 License: Apache 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mayan-importer-3.2.1/mayan_importer.egg-info/SOURCES.txt` & `mayan-importer-3.2.2/mayan_importer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.2.1/setup.py` & `mayan-importer-3.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,10 +94,10 @@
     license='Apache 2.0',
     long_description=readme + '\n\n' + history,
     name=PACKAGE_NAME,
     packages=find_packages(PACKAGE_DIR),
     platforms=['any'],
     python_requires='!=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*',
     url='https://gitlab.com/mayan-edms/importer',
-    version='3.2.1',
+    version='3.2.2',
     zip_safe=False,
 )
```

