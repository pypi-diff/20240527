# Comparing `tmp/django_customvueadmin-0.2.7.tar.gz` & `tmp/django_customvueadmin-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_customvueadmin-0.2.7.tar", last modified: Mon May 27 15:49:01 2024, max compression
+gzip compressed data, was "django_customvueadmin-0.2.8.tar", last modified: Mon May 27 19:09:12 2024, max compression
```

## Comparing `django_customvueadmin-0.2.7.tar` & `django_customvueadmin-0.2.8.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.110689 django_customvueadmin-0.2.7/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1073 2024-04-26 14:57:56.000000 django_customvueadmin-0.2.7/LICENSE
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      209 2024-04-11 14:26:38.000000 django_customvueadmin-0.2.7/MANIFEST.in
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2886 2024-05-27 15:49:01.107355 django_customvueadmin-0.2.7/PKG-INFO
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2053 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/README.rst
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.090687 django_customvueadmin-0.2.7/custom_admin/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       45 2024-05-27 15:48:55.000000 django_customvueadmin-0.2.7/custom_admin/__init__.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.090687 django_customvueadmin-0.2.7/custom_admin/api/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       86 2024-04-19 14:02:39.000000 django_customvueadmin-0.2.7/custom_admin/api/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1529 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/api/action_functions.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.090687 django_customvueadmin-0.2.7/custom_admin/api/actions/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      139 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.7/custom_admin/api/actions/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      985 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/api/actions/delete_action.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2538 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/api/actions/export_csv_action.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2723 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/api/actions/view_actions_mixin.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1766 2024-05-27 15:12:53.000000 django_customvueadmin-0.2.7/custom_admin/api/backends.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.094020 django_customvueadmin-0.2.7/custom_admin/api/fields/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      403 2024-05-06 15:09:48.000000 django_customvueadmin-0.2.7/custom_admin/api/fields/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      381 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.7/custom_admin/api/fields/base.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      811 2024-04-23 15:22:53.000000 django_customvueadmin-0.2.7/custom_admin/api/fields/char.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1120 2024-05-27 15:31:55.000000 django_customvueadmin-0.2.7/custom_admin/api/fields/choice.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3695 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/api/fields/files.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      157 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.7/custom_admin/api/fields/int.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      326 2024-05-06 16:10:42.000000 django_customvueadmin-0.2.7/custom_admin/api/fields/json.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      343 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.7/custom_admin/api/fields/numbers.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3871 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.7/custom_admin/api/fields/relation.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.094020 django_customvueadmin-0.2.7/custom_admin/api/filters/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      165 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/api/filters/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1623 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/api/filters/base_admin_filter.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.7/custom_admin/api/filters/choices.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      733 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/api/filters/date_range.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1445 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/api/inline_relation.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.094020 django_customvueadmin-0.2.7/custom_admin/api/inlines/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      305 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.7/custom_admin/api/inlines/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      601 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.7/custom_admin/api/inlines/export_csv_inline.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1595 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/api/inlines/inline_graph.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2129 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.7/custom_admin/api/inlines/inline_table.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       61 2024-03-29 18:33:05.000000 django_customvueadmin-0.2.7/custom_admin/api/inlines/inlines_type.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      135 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.7/custom_admin/api/inlines/interfaces.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4154 2024-04-02 18:13:36.000000 django_customvueadmin-0.2.7/custom_admin/api/inlines/view_inline_mixin.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      893 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.7/custom_admin/api/permissions.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.094020 django_customvueadmin-0.2.7/custom_admin/api/serializers/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      207 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.7/custom_admin/api/serializers/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      737 2024-04-19 13:32:46.000000 django_customvueadmin-0.2.7/custom_admin/api/serializers/auth_response.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5491 2024-05-06 15:09:50.000000 django_customvueadmin-0.2.7/custom_admin/api/serializers/base_serializer.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.094020 django_customvueadmin-0.2.7/custom_admin/api/tests/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/api/tests/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2317 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/api/tests/test_filters.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      517 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/api/tests/test_scheme_get.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      550 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/api/tests/urls.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      599 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/api/urls.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.094020 django_customvueadmin-0.2.7/custom_admin/api/views/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      414 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/api/views/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5829 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/api/views/autocomplete.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     8513 2024-05-27 14:55:57.000000 django_customvueadmin-0.2.7/custom_admin/api/views/base_admin_viewset.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.094020 django_customvueadmin-0.2.7/custom_admin/api/views/defaults/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      131 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/api/views/defaults/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2080 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/api/views/defaults/admin_log.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      366 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/api/views/defaults/groups.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      529 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/api/views/defaults/permissions.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      909 2024-04-23 23:45:01.000000 django_customvueadmin-0.2.7/custom_admin/api/views/get_sections.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1517 2024-04-11 17:29:22.000000 django_customvueadmin-0.2.7/custom_admin/api/views/token_auth.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      974 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/api/viewset_info.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.097354 django_customvueadmin-0.2.7/custom_admin/controllers/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-04-19 14:01:33.000000 django_customvueadmin-0.2.7/custom_admin/controllers/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3475 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/controllers/admin_log_manager.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3823 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/controllers/custom_metadata.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3078 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/controllers/filters_schema.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     9232 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.7/custom_admin/controllers/schema_generator.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.097354 django_customvueadmin-0.2.7/custom_admin/management/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-04-15 16:06:07.000000 django_customvueadmin-0.2.7/custom_admin/management/__init__.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.097354 django_customvueadmin-0.2.7/custom_admin/management/commands/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-04-15 16:06:19.000000 django_customvueadmin-0.2.7/custom_admin/management/commands/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1300 2024-04-15 16:52:15.000000 django_customvueadmin-0.2.7/custom_admin/management/commands/custom_admin_viewsets_list.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.097354 django_customvueadmin-0.2.7/custom_admin/migrations/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1695 2024-04-11 18:20:54.000000 django_customvueadmin-0.2.7/custom_admin/migrations/0001_initial.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 18:20:54.000000 django_customvueadmin-0.2.7/custom_admin/migrations/__init__.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.097354 django_customvueadmin-0.2.7/custom_admin/models/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       32 2024-03-11 07:49:25.000000 django_customvueadmin-0.2.7/custom_admin/models/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1469 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.7/custom_admin/models/admin_log.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.090687 django_customvueadmin-0.2.7/custom_admin/static/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.104021 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2238 2024-05-27 15:48:47.000000 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/favicon.ico
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)  2668814 2024-05-27 15:48:47.000000 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/index-DaxJfUgR.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)   742561 2024-05-27 15:48:47.000000 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/index-DijOZrPh.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)   385360 2024-05-27 15:48:47.000000 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/materialdesignicons-webfont-CYDMK1kx.woff2
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)   561776 2024-05-27 15:48:47.000000 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/materialdesignicons-webfont-CgCzGbLl.woff
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1243500 2024-05-27 15:48:47.000000 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/materialdesignicons-webfont-D3kAzl71.ttf
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1243720 2024-05-27 15:48:47.000000 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/materialdesignicons-webfont-DttUABo4.eot
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.104021 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.107355 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/dark-first/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4788 2024-05-27 15:48:47.000000 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/dark-first/content.min.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    50376 2024-05-27 15:48:47.000000 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/dark-first/skin.min.css
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.107355 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/dark-slim/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4730 2024-05-27 15:48:47.000000 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/dark-slim/content.min.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    49965 2024-05-27 15:48:47.000000 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/dark-slim/skin.min.css
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.107355 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/img/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    14708 2024-05-27 15:48:47.000000 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/img/example.png
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    15764 2024-05-27 15:48:47.000000 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/img/tinymce.woff2
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.107355 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/lightgray/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3193 2024-05-27 15:48:47.000000 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/lightgray/content.min.css
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.107355 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/lightgray/fonts/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     7664 2024-05-27 15:48:47.000000 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/lightgray/fonts/tinymce.woff
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    38232 2024-05-27 15:48:47.000000 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/lightgray/skin.min.css
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.090687 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/plugins/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.107355 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/plugins/accordion/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.107355 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/plugins/accordion/css/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-05-27 15:48:47.000000 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/plugins/accordion/css/accordion.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1251 2024-05-27 15:48:47.000000 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/plugins/accordion/plugin.js
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.090687 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/plugins/codesample/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.107355 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1736 2024-05-27 15:48:47.000000 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/prism.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1171290 2024-05-27 15:48:47.000000 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/tinymce.min.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    18804 2024-05-27 15:48:47.000000 django_customvueadmin-0.2.7/custom_admin/static/custom_admin/vanilla-picker-B6E6ObS_.js
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.090687 django_customvueadmin-0.2.7/custom_admin/templates/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.107355 django_customvueadmin-0.2.7/custom_admin/templates/custom_admin/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1351 2024-05-27 15:48:47.000000 django_customvueadmin-0.2.7/custom_admin/templates/custom_admin/admin_index.html
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.107355 django_customvueadmin-0.2.7/custom_admin/utils/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       35 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.7/custom_admin/utils/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1976 2024-04-11 17:58:41.000000 django_customvueadmin-0.2.7/custom_admin/utils/async_mixin.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2425 2024-04-09 09:57:39.000000 django_customvueadmin-0.2.7/custom_admin/utils/colors.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      570 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.7/custom_admin/utils/get_schema.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      593 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.7/custom_admin/utils/register_admin_viewsets.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.107355 django_customvueadmin-0.2.7/custom_admin/views/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       40 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.7/custom_admin/views/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1316 2024-05-27 09:42:41.000000 django_customvueadmin-0.2.7/custom_admin/views/admin_page.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 15:49:01.107355 django_customvueadmin-0.2.7/django_customvueadmin.egg-info/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2886 2024-05-27 15:49:01.000000 django_customvueadmin-0.2.7/django_customvueadmin.egg-info/PKG-INFO
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4256 2024-05-27 15:49:01.000000 django_customvueadmin-0.2.7/django_customvueadmin.egg-info/SOURCES.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-05-27 15:49:01.000000 django_customvueadmin-0.2.7/django_customvueadmin.egg-info/dependency_links.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-05-27 15:49:00.000000 django_customvueadmin-0.2.7/django_customvueadmin.egg-info/not-zip-safe
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       13 2024-05-27 15:49:01.000000 django_customvueadmin-0.2.7/django_customvueadmin.egg-info/top_level.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      222 2024-04-11 09:22:36.000000 django_customvueadmin-0.2.7/pyproject.toml
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1000 2024-05-27 15:49:01.110689 django_customvueadmin-0.2.7/setup.cfg
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.048662 django_customvueadmin-0.2.8/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1073 2024-04-26 14:57:56.000000 django_customvueadmin-0.2.8/LICENSE
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      209 2024-04-11 14:26:38.000000 django_customvueadmin-0.2.8/MANIFEST.in
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2886 2024-05-27 19:09:12.048662 django_customvueadmin-0.2.8/PKG-INFO
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2053 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/README.rst
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.031993 django_customvueadmin-0.2.8/custom_admin/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       45 2024-05-27 19:08:59.000000 django_customvueadmin-0.2.8/custom_admin/__init__.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.031993 django_customvueadmin-0.2.8/custom_admin/api/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       86 2024-04-19 14:02:39.000000 django_customvueadmin-0.2.8/custom_admin/api/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1529 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/api/action_functions.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.031993 django_customvueadmin-0.2.8/custom_admin/api/actions/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      139 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.8/custom_admin/api/actions/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      985 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/api/actions/delete_action.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2538 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/api/actions/export_csv_action.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2723 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/api/actions/view_actions_mixin.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1697 2024-05-27 18:30:24.000000 django_customvueadmin-0.2.8/custom_admin/api/backends.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.031993 django_customvueadmin-0.2.8/custom_admin/api/fields/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      403 2024-05-06 15:09:48.000000 django_customvueadmin-0.2.8/custom_admin/api/fields/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      381 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.8/custom_admin/api/fields/base.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      811 2024-04-23 15:22:53.000000 django_customvueadmin-0.2.8/custom_admin/api/fields/char.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1120 2024-05-27 15:31:55.000000 django_customvueadmin-0.2.8/custom_admin/api/fields/choice.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3695 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/api/fields/files.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      157 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.8/custom_admin/api/fields/int.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      326 2024-05-06 16:10:42.000000 django_customvueadmin-0.2.8/custom_admin/api/fields/json.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      343 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.8/custom_admin/api/fields/numbers.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3871 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.8/custom_admin/api/fields/relation.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.035327 django_customvueadmin-0.2.8/custom_admin/api/filters/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      165 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/api/filters/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1623 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/api/filters/base_admin_filter.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.8/custom_admin/api/filters/choices.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      733 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/api/filters/date_range.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1445 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/api/inline_relation.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.035327 django_customvueadmin-0.2.8/custom_admin/api/inlines/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      305 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.8/custom_admin/api/inlines/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      601 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.8/custom_admin/api/inlines/export_csv_inline.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1595 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/api/inlines/inline_graph.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2129 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.8/custom_admin/api/inlines/inline_table.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       61 2024-03-29 18:33:05.000000 django_customvueadmin-0.2.8/custom_admin/api/inlines/inlines_type.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      135 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.8/custom_admin/api/inlines/interfaces.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4154 2024-04-02 18:13:36.000000 django_customvueadmin-0.2.8/custom_admin/api/inlines/view_inline_mixin.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      893 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.8/custom_admin/api/permissions.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.035327 django_customvueadmin-0.2.8/custom_admin/api/serializers/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      207 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.8/custom_admin/api/serializers/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      737 2024-04-19 13:32:46.000000 django_customvueadmin-0.2.8/custom_admin/api/serializers/auth_response.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5491 2024-05-06 15:09:50.000000 django_customvueadmin-0.2.8/custom_admin/api/serializers/base_serializer.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.035327 django_customvueadmin-0.2.8/custom_admin/api/tests/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/api/tests/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2317 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/api/tests/test_filters.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      517 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/api/tests/test_scheme_get.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      550 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/api/tests/urls.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      599 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/api/urls.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.035327 django_customvueadmin-0.2.8/custom_admin/api/views/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      414 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/api/views/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5829 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/api/views/autocomplete.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     8513 2024-05-27 14:55:57.000000 django_customvueadmin-0.2.8/custom_admin/api/views/base_admin_viewset.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.035327 django_customvueadmin-0.2.8/custom_admin/api/views/defaults/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      131 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/api/views/defaults/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2080 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/api/views/defaults/admin_log.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      366 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/api/views/defaults/groups.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      529 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/api/views/defaults/permissions.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      909 2024-04-23 23:45:01.000000 django_customvueadmin-0.2.8/custom_admin/api/views/get_sections.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1517 2024-04-11 17:29:22.000000 django_customvueadmin-0.2.8/custom_admin/api/views/token_auth.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      974 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/api/viewset_info.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.038660 django_customvueadmin-0.2.8/custom_admin/controllers/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-04-19 14:01:33.000000 django_customvueadmin-0.2.8/custom_admin/controllers/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3475 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/controllers/admin_log_manager.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3823 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/controllers/custom_metadata.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3078 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/controllers/filters_schema.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     9232 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.8/custom_admin/controllers/schema_generator.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.038660 django_customvueadmin-0.2.8/custom_admin/management/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-04-15 16:06:07.000000 django_customvueadmin-0.2.8/custom_admin/management/__init__.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.038660 django_customvueadmin-0.2.8/custom_admin/management/commands/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-04-15 16:06:19.000000 django_customvueadmin-0.2.8/custom_admin/management/commands/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1300 2024-04-15 16:52:15.000000 django_customvueadmin-0.2.8/custom_admin/management/commands/custom_admin_viewsets_list.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.038660 django_customvueadmin-0.2.8/custom_admin/migrations/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1695 2024-04-11 18:20:54.000000 django_customvueadmin-0.2.8/custom_admin/migrations/0001_initial.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 18:20:54.000000 django_customvueadmin-0.2.8/custom_admin/migrations/__init__.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.038660 django_customvueadmin-0.2.8/custom_admin/models/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       32 2024-03-11 07:49:25.000000 django_customvueadmin-0.2.8/custom_admin/models/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1469 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.8/custom_admin/models/admin_log.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.028659 django_customvueadmin-0.2.8/custom_admin/static/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.045328 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2238 2024-05-27 19:08:35.000000 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/favicon.ico
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)  2668896 2024-05-27 19:08:35.000000 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/index-BadLqHeD.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)   742561 2024-05-27 19:08:35.000000 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/index-DijOZrPh.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)   385360 2024-05-27 19:08:35.000000 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/materialdesignicons-webfont-CYDMK1kx.woff2
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)   561776 2024-05-27 19:08:35.000000 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/materialdesignicons-webfont-CgCzGbLl.woff
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1243500 2024-05-27 19:08:35.000000 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/materialdesignicons-webfont-D3kAzl71.ttf
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1243720 2024-05-27 19:08:35.000000 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/materialdesignicons-webfont-DttUABo4.eot
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.045328 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.045328 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/dark-first/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4788 2024-05-27 19:08:35.000000 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/dark-first/content.min.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    50376 2024-05-27 19:08:35.000000 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/dark-first/skin.min.css
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.045328 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/dark-slim/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4730 2024-05-27 19:08:35.000000 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/dark-slim/content.min.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    49965 2024-05-27 19:08:35.000000 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/dark-slim/skin.min.css
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.048662 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/img/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    14708 2024-05-27 19:08:35.000000 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/img/example.png
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    15764 2024-05-27 19:08:35.000000 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/img/tinymce.woff2
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.048662 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/lightgray/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3193 2024-05-27 19:08:35.000000 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/lightgray/content.min.css
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.048662 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/lightgray/fonts/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     7664 2024-05-27 19:08:35.000000 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/lightgray/fonts/tinymce.woff
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    38232 2024-05-27 19:08:35.000000 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/lightgray/skin.min.css
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.028659 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/plugins/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.048662 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/plugins/accordion/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.048662 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/plugins/accordion/css/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-05-27 19:08:35.000000 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/plugins/accordion/css/accordion.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1251 2024-05-27 19:08:35.000000 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/plugins/accordion/plugin.js
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.028659 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/plugins/codesample/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.048662 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1736 2024-05-27 19:08:35.000000 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/prism.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1171290 2024-05-27 19:08:35.000000 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/tinymce.min.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    18804 2024-05-27 19:08:35.000000 django_customvueadmin-0.2.8/custom_admin/static/custom_admin/vanilla-picker-B6E6ObS_.js
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.031993 django_customvueadmin-0.2.8/custom_admin/templates/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.048662 django_customvueadmin-0.2.8/custom_admin/templates/custom_admin/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1351 2024-05-27 19:08:35.000000 django_customvueadmin-0.2.8/custom_admin/templates/custom_admin/admin_index.html
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.048662 django_customvueadmin-0.2.8/custom_admin/utils/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       35 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.8/custom_admin/utils/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1976 2024-04-11 17:58:41.000000 django_customvueadmin-0.2.8/custom_admin/utils/async_mixin.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2425 2024-04-09 09:57:39.000000 django_customvueadmin-0.2.8/custom_admin/utils/colors.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      570 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.8/custom_admin/utils/get_schema.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      593 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.8/custom_admin/utils/register_admin_viewsets.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.048662 django_customvueadmin-0.2.8/custom_admin/views/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       40 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.8/custom_admin/views/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1316 2024-05-27 09:42:41.000000 django_customvueadmin-0.2.8/custom_admin/views/admin_page.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 19:09:12.048662 django_customvueadmin-0.2.8/django_customvueadmin.egg-info/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2886 2024-05-27 19:09:12.000000 django_customvueadmin-0.2.8/django_customvueadmin.egg-info/PKG-INFO
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4256 2024-05-27 19:09:12.000000 django_customvueadmin-0.2.8/django_customvueadmin.egg-info/SOURCES.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-05-27 19:09:12.000000 django_customvueadmin-0.2.8/django_customvueadmin.egg-info/dependency_links.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-05-27 19:09:11.000000 django_customvueadmin-0.2.8/django_customvueadmin.egg-info/not-zip-safe
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       13 2024-05-27 19:09:12.000000 django_customvueadmin-0.2.8/django_customvueadmin.egg-info/top_level.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      222 2024-04-11 09:22:36.000000 django_customvueadmin-0.2.8/pyproject.toml
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1000 2024-05-27 19:09:12.048662 django_customvueadmin-0.2.8/setup.cfg
```

### Comparing `django_customvueadmin-0.2.7/LICENSE` & `django_customvueadmin-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/PKG-INFO` & `django_customvueadmin-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-customvueadmin
-Version: 0.2.7
+Version: 0.2.8
 Summary: A custom admin interface providing backend via DRF and frontend via Vue and Element UI that tries to Keep It Simple.
 Home-page: https://innova-group-llc.github.io/custom_admin_docs/
 License: BSD-3-Clause
 Project-URL: Documentation, https://innova-group-llc.github.io/custom_admin_docs/
 Project-URL: Source, https://github.com/Innova-Group-LLC/custom_admin
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `django_customvueadmin-0.2.7/README.rst` & `django_customvueadmin-0.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/action_functions.py` & `django_customvueadmin-0.2.8/custom_admin/api/action_functions.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/actions/delete_action.py` & `django_customvueadmin-0.2.8/custom_admin/api/actions/delete_action.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/actions/export_csv_action.py` & `django_customvueadmin-0.2.8/custom_admin/api/actions/export_csv_action.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/actions/view_actions_mixin.py` & `django_customvueadmin-0.2.8/custom_admin/api/actions/view_actions_mixin.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/backends.py` & `django_customvueadmin-0.2.8/custom_admin/api/backends.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
         filter_info = get_filter_info(request)
         if filter_info:
             _ordering = filter_info.get('ordering')
             if _ordering:
                 return _ordering
 
-        print('ordering', ordering, getattr(view, 'ordering', None))
         return ordering
 
 
 class CustomFilterBackend(rest_framework.DjangoFilterBackend):
     filterset_base = BaseAdminFilterSet
 
     def get_filterset_kwargs(self, request, queryset, view):
```

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/fields/char.py` & `django_customvueadmin-0.2.8/custom_admin/api/fields/char.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/fields/choice.py` & `django_customvueadmin-0.2.8/custom_admin/api/fields/choice.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/fields/files.py` & `django_customvueadmin-0.2.8/custom_admin/api/fields/files.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/fields/relation.py` & `django_customvueadmin-0.2.8/custom_admin/api/fields/relation.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/filters/base_admin_filter.py` & `django_customvueadmin-0.2.8/custom_admin/api/filters/base_admin_filter.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/filters/date_range.py` & `django_customvueadmin-0.2.8/custom_admin/api/filters/date_range.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/inline_relation.py` & `django_customvueadmin-0.2.8/custom_admin/api/inline_relation.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/inlines/export_csv_inline.py` & `django_customvueadmin-0.2.8/custom_admin/api/inlines/export_csv_inline.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/inlines/inline_graph.py` & `django_customvueadmin-0.2.8/custom_admin/api/inlines/inline_graph.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/inlines/inline_table.py` & `django_customvueadmin-0.2.8/custom_admin/api/inlines/inline_table.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/inlines/view_inline_mixin.py` & `django_customvueadmin-0.2.8/custom_admin/api/inlines/view_inline_mixin.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/permissions.py` & `django_customvueadmin-0.2.8/custom_admin/api/permissions.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/serializers/auth_response.py` & `django_customvueadmin-0.2.8/custom_admin/api/serializers/auth_response.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/serializers/base_serializer.py` & `django_customvueadmin-0.2.8/custom_admin/api/serializers/base_serializer.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/tests/test_filters.py` & `django_customvueadmin-0.2.8/custom_admin/api/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/tests/test_scheme_get.py` & `django_customvueadmin-0.2.8/custom_admin/api/tests/test_scheme_get.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/tests/urls.py` & `django_customvueadmin-0.2.8/custom_admin/api/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/urls.py` & `django_customvueadmin-0.2.8/custom_admin/api/urls.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/views/autocomplete.py` & `django_customvueadmin-0.2.8/custom_admin/api/views/autocomplete.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/views/base_admin_viewset.py` & `django_customvueadmin-0.2.8/custom_admin/api/views/base_admin_viewset.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/views/defaults/admin_log.py` & `django_customvueadmin-0.2.8/custom_admin/api/views/defaults/admin_log.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/views/defaults/permissions.py` & `django_customvueadmin-0.2.8/custom_admin/api/views/defaults/permissions.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/views/get_sections.py` & `django_customvueadmin-0.2.8/custom_admin/api/views/get_sections.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/views/token_auth.py` & `django_customvueadmin-0.2.8/custom_admin/api/views/token_auth.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/api/viewset_info.py` & `django_customvueadmin-0.2.8/custom_admin/api/viewset_info.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/controllers/admin_log_manager.py` & `django_customvueadmin-0.2.8/custom_admin/controllers/admin_log_manager.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/controllers/custom_metadata.py` & `django_customvueadmin-0.2.8/custom_admin/controllers/custom_metadata.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/controllers/filters_schema.py` & `django_customvueadmin-0.2.8/custom_admin/controllers/filters_schema.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/controllers/schema_generator.py` & `django_customvueadmin-0.2.8/custom_admin/controllers/schema_generator.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/management/commands/custom_admin_viewsets_list.py` & `django_customvueadmin-0.2.8/custom_admin/management/commands/custom_admin_viewsets_list.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/migrations/0001_initial.py` & `django_customvueadmin-0.2.8/custom_admin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/models/admin_log.py` & `django_customvueadmin-0.2.8/custom_admin/models/admin_log.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/static/custom_admin/favicon.ico` & `django_customvueadmin-0.2.8/custom_admin/static/custom_admin/favicon.ico`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/static/custom_admin/index-DaxJfUgR.js` & `django_customvueadmin-0.2.8/custom_admin/static/custom_admin/index-BadLqHeD.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -119529,21 +119529,21 @@
             }))], 64)) : u.field.type === "choice" ? (ue(), Me(He, {
                 key: 3
             }, [d[u.key] ? (ue(), Me(He, {
                 key: 0
             }, [Object.keys(u.field.tag_style || {}).length > 0 ? (ue(), Be(Ff, {
                 key: 0,
                 size: "small",
-                color: u.field.tag_style[d[u.key].value]
+                color: u.field.tag_style[d[u.key]]
             }, {
-                default: pe(() => [jt(It(d[u.key].text), 1)]),
+                default: pe(() => [jt(It(d[u.key]), 1)]),
                 _: 2
             }, 1032, ["color"])) : (ue(), Me(He, {
                 key: 1
-            }, [jt(It(d[u.key].text), 1)], 64))], 64)) : We("", !0)], 64)) : u.field.type === "datetime" ? (ue(), Me("span", gFt, It(o.formatDateTime(d[u.key])), 1)) : u.field.type === "image upload" && u.field.list_preview ? (ue(), Me(He, {
+            }, [jt(It(d[u.key]), 1)], 64))], 64)) : We("", !0)], 64)) : u.field.type === "datetime" ? (ue(), Me("span", gFt, It(o.formatDateTime(d[u.key])), 1)) : u.field.type === "image upload" && u.field.list_preview ? (ue(), Me(He, {
                 key: 5
             }, [d[u.key] && d[u.key].url ? (ue(), Be(p1, {
                 key: 0,
                 class: "image-preview",
                 width: "100",
                 "max-height": "100",
                 cover: "",
@@ -119728,14 +119728,17 @@
                             theme: "auto",
                             type: "error",
                             position: "top-center",
                             dangerouslyHTMLString: !0
                         })
                     })
                 },
+                canUpdate() {
+                    return this.apiMethods.partial_update !== void 0
+                },
                 updateModel() {
                     this.$refs.fieldscontainer.updateErrors({}), this.loading = !0;
                     let e = "partial_update";
                     Qge(this.apiMethods[e].url.replace("{id}", this.id), this.apiMethods[e].methodHttp, this.formData).then(t => {
                         if (this.loading = !1, t) {
                             let n = this.$t("modelUpdated").replace("{id}", t.id);
                             Qn(n, {
@@ -119772,20 +119775,21 @@
         return ue(), Me("div", null, [M(a, {
             ref: "fieldscontainer",
             formType: "edit",
             "api-info": n.apiInfo,
             viewname: n.viewname,
             loading: i.loading,
             onChanged: t[0] || (t[0] = s => i.formData = s)
-        }, null, 8, ["api-info", "viewname", "loading"]), Nt("div", OFt, [M(gr, {
+        }, null, 8, ["api-info", "viewname", "loading"]), Nt("div", OFt, [o.canUpdate() ? (ue(), Be(gr, {
+            key: 0,
             text: e.$t("update"),
             variant: "tonal",
             color: "primary",
             onClick: o.updateModel
-        }, null, 8, ["text", "onClick"])])])
+        }, null, 8, ["text", "onClick"])) : We("", !0)])])
     }
     const t0e = fo(jFt, [
         ["render", PFt]
     ]);
     /*!
      * @kurkle/color v0.3.2
      * https://github.com/kurkle/color#readme
```

### Comparing `django_customvueadmin-0.2.7/custom_admin/static/custom_admin/index-DijOZrPh.css` & `django_customvueadmin-0.2.8/custom_admin/static/custom_admin/index-DijOZrPh.css`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/static/custom_admin/materialdesignicons-webfont-CYDMK1kx.woff2` & `django_customvueadmin-0.2.8/custom_admin/static/custom_admin/materialdesignicons-webfont-CYDMK1kx.woff2`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/static/custom_admin/materialdesignicons-webfont-CgCzGbLl.woff` & `django_customvueadmin-0.2.8/custom_admin/static/custom_admin/materialdesignicons-webfont-CgCzGbLl.woff`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/static/custom_admin/materialdesignicons-webfont-D3kAzl71.ttf` & `django_customvueadmin-0.2.8/custom_admin/static/custom_admin/materialdesignicons-webfont-D3kAzl71.ttf`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/static/custom_admin/materialdesignicons-webfont-DttUABo4.eot` & `django_customvueadmin-0.2.8/custom_admin/static/custom_admin/materialdesignicons-webfont-DttUABo4.eot`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/dark-first/content.min.css` & `django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/dark-first/content.min.css`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/dark-first/skin.min.css` & `django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/dark-first/skin.min.css`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/dark-slim/content.min.css` & `django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/dark-slim/content.min.css`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/dark-slim/skin.min.css` & `django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/dark-slim/skin.min.css`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/img/example.png` & `django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/img/example.png`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/img/tinymce.woff2` & `django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/img/tinymce.woff2`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/lightgray/content.min.css` & `django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/lightgray/content.min.css`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/lightgray/fonts/tinymce.woff` & `django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/lightgray/fonts/tinymce.woff`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/lightgray/skin.min.css` & `django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/lightgray/skin.min.css`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/plugins/accordion/plugin.js` & `django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/plugins/accordion/plugin.js`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/prism.css` & `django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/prism.css`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/static/custom_admin/tinymce/tinymce.min.js` & `django_customvueadmin-0.2.8/custom_admin/static/custom_admin/tinymce/tinymce.min.js`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/static/custom_admin/vanilla-picker-B6E6ObS_.js` & `django_customvueadmin-0.2.8/custom_admin/static/custom_admin/vanilla-picker-B6E6ObS_.js`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/templates/custom_admin/admin_index.html` & `django_customvueadmin-0.2.8/custom_admin/templates/custom_admin/admin_index.html`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   <link rel="preload" as="font" type="font/woff" href="/static/custom_admin/materialdesignicons-webfont-CgCzGbLl.woff" crossorigin="anonymous">
   <link rel="preload" as="font" type="font/ttf" href="/static/custom_admin/materialdesignicons-webfont-D3kAzl71.ttf" crossorigin="anonymous">
 
   <meta charset="UTF-8" />
   <link rel="icon" href="/custom_admin/favicon.ico" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   <title>{{ SETTINGS.title }}</title>
-  <script type="module" crossorigin src="/static/custom_admin/index-DaxJfUgR.js"></script>
+  <script type="module" crossorigin src="/static/custom_admin/index-BadLqHeD.js"></script>
   <link rel="stylesheet" crossorigin href="/static/custom_admin/index-DijOZrPh.css">
 </head>
 
 <body>
   <div id="app"></div>
   <span id="settings" data-json="{{ SETTINGS_JSON }}"></span>
 </body>
```

### Comparing `django_customvueadmin-0.2.7/custom_admin/utils/async_mixin.py` & `django_customvueadmin-0.2.8/custom_admin/utils/async_mixin.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/utils/colors.py` & `django_customvueadmin-0.2.8/custom_admin/utils/colors.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/utils/get_schema.py` & `django_customvueadmin-0.2.8/custom_admin/utils/get_schema.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/utils/register_admin_viewsets.py` & `django_customvueadmin-0.2.8/custom_admin/utils/register_admin_viewsets.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/custom_admin/views/admin_page.py` & `django_customvueadmin-0.2.8/custom_admin/views/admin_page.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.7/django_customvueadmin.egg-info/PKG-INFO` & `django_customvueadmin-0.2.8/django_customvueadmin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-customvueadmin
-Version: 0.2.7
+Version: 0.2.8
 Summary: A custom admin interface providing backend via DRF and frontend via Vue and Element UI that tries to Keep It Simple.
 Home-page: https://innova-group-llc.github.io/custom_admin_docs/
 License: BSD-3-Clause
 Project-URL: Documentation, https://innova-group-llc.github.io/custom_admin_docs/
 Project-URL: Source, https://github.com/Innova-Group-LLC/custom_admin
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `django_customvueadmin-0.2.7/django_customvueadmin.egg-info/SOURCES.txt` & `django_customvueadmin-0.2.8/django_customvueadmin.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 custom_admin/management/commands/__init__.py
 custom_admin/management/commands/custom_admin_viewsets_list.py
 custom_admin/migrations/0001_initial.py
 custom_admin/migrations/__init__.py
 custom_admin/models/__init__.py
 custom_admin/models/admin_log.py
 custom_admin/static/custom_admin/favicon.ico
-custom_admin/static/custom_admin/index-DaxJfUgR.js
+custom_admin/static/custom_admin/index-BadLqHeD.js
 custom_admin/static/custom_admin/index-DijOZrPh.css
 custom_admin/static/custom_admin/materialdesignicons-webfont-CYDMK1kx.woff2
 custom_admin/static/custom_admin/materialdesignicons-webfont-CgCzGbLl.woff
 custom_admin/static/custom_admin/materialdesignicons-webfont-D3kAzl71.ttf
 custom_admin/static/custom_admin/materialdesignicons-webfont-DttUABo4.eot
 custom_admin/static/custom_admin/vanilla-picker-B6E6ObS_.js
 custom_admin/static/custom_admin/tinymce/tinymce.min.js
```

### Comparing `django_customvueadmin-0.2.7/setup.cfg` & `django_customvueadmin-0.2.8/setup.cfg`

 * *Files identical despite different names*
