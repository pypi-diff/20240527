# Comparing `tmp/django_customvueadmin-0.2.5.tar.gz` & `tmp/django_customvueadmin-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_customvueadmin-0.2.5.tar", last modified: Mon May 27 09:43:43 2024, max compression
+gzip compressed data, was "django_customvueadmin-0.2.6.tar", last modified: Mon May 27 09:58:44 2024, max compression
```

## Comparing `django_customvueadmin-0.2.5.tar` & `django_customvueadmin-0.2.6.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.322184 django_customvueadmin-0.2.5/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1073 2024-04-26 14:57:56.000000 django_customvueadmin-0.2.5/LICENSE
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      209 2024-04-11 14:26:38.000000 django_customvueadmin-0.2.5/MANIFEST.in
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2886 2024-05-27 09:43:43.322184 django_customvueadmin-0.2.5/PKG-INFO
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2053 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/README.rst
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.305517 django_customvueadmin-0.2.5/custom_admin/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       45 2024-05-27 09:43:34.000000 django_customvueadmin-0.2.5/custom_admin/__init__.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.305517 django_customvueadmin-0.2.5/custom_admin/api/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       86 2024-04-19 14:02:39.000000 django_customvueadmin-0.2.5/custom_admin/api/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1529 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/api/action_functions.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.305517 django_customvueadmin-0.2.5/custom_admin/api/actions/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      139 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.5/custom_admin/api/actions/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      985 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/api/actions/delete_action.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2538 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/api/actions/export_csv_action.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2723 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/api/actions/view_actions_mixin.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1724 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/api/backends.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.308850 django_customvueadmin-0.2.5/custom_admin/api/fields/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      403 2024-05-06 15:09:48.000000 django_customvueadmin-0.2.5/custom_admin/api/fields/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      381 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.5/custom_admin/api/fields/base.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      811 2024-04-23 15:22:53.000000 django_customvueadmin-0.2.5/custom_admin/api/fields/char.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1233 2024-04-23 15:23:30.000000 django_customvueadmin-0.2.5/custom_admin/api/fields/choice.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3695 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/api/fields/files.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      157 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.5/custom_admin/api/fields/int.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      326 2024-05-06 16:10:42.000000 django_customvueadmin-0.2.5/custom_admin/api/fields/json.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      343 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.5/custom_admin/api/fields/numbers.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3871 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.5/custom_admin/api/fields/relation.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.308850 django_customvueadmin-0.2.5/custom_admin/api/filters/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      165 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/api/filters/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1623 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/api/filters/base_admin_filter.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.5/custom_admin/api/filters/choices.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      733 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/api/filters/date_range.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1445 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/api/inline_relation.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.308850 django_customvueadmin-0.2.5/custom_admin/api/inlines/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      305 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.5/custom_admin/api/inlines/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      601 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.5/custom_admin/api/inlines/export_csv_inline.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1595 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/api/inlines/inline_graph.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2129 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.5/custom_admin/api/inlines/inline_table.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       61 2024-03-29 18:33:05.000000 django_customvueadmin-0.2.5/custom_admin/api/inlines/inlines_type.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      135 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.5/custom_admin/api/inlines/interfaces.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4154 2024-04-02 18:13:36.000000 django_customvueadmin-0.2.5/custom_admin/api/inlines/view_inline_mixin.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      893 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.5/custom_admin/api/permissions.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.308850 django_customvueadmin-0.2.5/custom_admin/api/serializers/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      207 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.5/custom_admin/api/serializers/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      737 2024-04-19 13:32:46.000000 django_customvueadmin-0.2.5/custom_admin/api/serializers/auth_response.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5491 2024-05-06 15:09:50.000000 django_customvueadmin-0.2.5/custom_admin/api/serializers/base_serializer.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.308850 django_customvueadmin-0.2.5/custom_admin/api/tests/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/api/tests/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2317 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/api/tests/test_filters.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      517 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/api/tests/test_scheme_get.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      550 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/api/tests/urls.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      599 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/api/urls.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.308850 django_customvueadmin-0.2.5/custom_admin/api/views/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      414 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/api/views/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5829 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/api/views/autocomplete.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     8432 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/api/views/base_admin_viewset.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.312184 django_customvueadmin-0.2.5/custom_admin/api/views/defaults/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      131 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/api/views/defaults/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2080 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/api/views/defaults/admin_log.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      366 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/api/views/defaults/groups.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      529 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/api/views/defaults/permissions.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      909 2024-04-23 23:45:01.000000 django_customvueadmin-0.2.5/custom_admin/api/views/get_sections.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1517 2024-04-11 17:29:22.000000 django_customvueadmin-0.2.5/custom_admin/api/views/token_auth.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      974 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/api/viewset_info.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.312184 django_customvueadmin-0.2.5/custom_admin/controllers/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-04-19 14:01:33.000000 django_customvueadmin-0.2.5/custom_admin/controllers/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3475 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/controllers/admin_log_manager.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3823 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/controllers/custom_metadata.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3078 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/controllers/filters_schema.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     9232 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.5/custom_admin/controllers/schema_generator.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.312184 django_customvueadmin-0.2.5/custom_admin/management/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-04-15 16:06:07.000000 django_customvueadmin-0.2.5/custom_admin/management/__init__.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.312184 django_customvueadmin-0.2.5/custom_admin/management/commands/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-04-15 16:06:19.000000 django_customvueadmin-0.2.5/custom_admin/management/commands/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1300 2024-04-15 16:52:15.000000 django_customvueadmin-0.2.5/custom_admin/management/commands/custom_admin_viewsets_list.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.312184 django_customvueadmin-0.2.5/custom_admin/migrations/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1695 2024-04-11 18:20:54.000000 django_customvueadmin-0.2.5/custom_admin/migrations/0001_initial.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 18:20:54.000000 django_customvueadmin-0.2.5/custom_admin/migrations/__init__.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.312184 django_customvueadmin-0.2.5/custom_admin/models/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       32 2024-03-11 07:49:25.000000 django_customvueadmin-0.2.5/custom_admin/models/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1469 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.5/custom_admin/models/admin_log.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.305517 django_customvueadmin-0.2.5/custom_admin/static/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.318851 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2238 2024-05-27 09:43:23.000000 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/favicon.ico
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1681598 2024-05-27 09:43:23.000000 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/index-CKHFT4s-.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)   752741 2024-05-27 09:43:23.000000 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/index-Dtvf0MB6.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)   385360 2024-05-27 09:43:23.000000 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/materialdesignicons-webfont-CYDMK1kx.woff2
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)   561776 2024-05-27 09:43:23.000000 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/materialdesignicons-webfont-CgCzGbLl.woff
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1243500 2024-05-27 09:43:23.000000 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/materialdesignicons-webfont-D3kAzl71.ttf
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1243720 2024-05-27 09:43:23.000000 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/materialdesignicons-webfont-DttUABo4.eot
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.318851 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.318851 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/dark-first/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4788 2024-05-27 09:43:23.000000 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/dark-first/content.min.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    50376 2024-05-27 09:43:23.000000 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/dark-first/skin.min.css
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.318851 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/dark-slim/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4730 2024-05-27 09:43:23.000000 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/dark-slim/content.min.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    49965 2024-05-27 09:43:23.000000 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/dark-slim/skin.min.css
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.318851 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/img/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    14708 2024-05-27 09:43:23.000000 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/img/example.png
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    15764 2024-05-27 09:43:23.000000 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/img/tinymce.woff2
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.322184 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/lightgray/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3193 2024-05-27 09:43:23.000000 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/lightgray/content.min.css
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.322184 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/lightgray/fonts/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     7664 2024-05-27 09:43:23.000000 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/lightgray/fonts/tinymce.woff
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    38232 2024-05-27 09:43:23.000000 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/lightgray/skin.min.css
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.305517 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/plugins/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.322184 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/plugins/accordion/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.322184 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/plugins/accordion/css/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-05-27 09:43:23.000000 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/plugins/accordion/css/accordion.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1251 2024-05-27 09:43:23.000000 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/plugins/accordion/plugin.js
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.305517 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/plugins/codesample/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.322184 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1736 2024-05-27 09:43:23.000000 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/prism.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1171290 2024-05-27 09:43:23.000000 django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/tinymce.min.js
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.305517 django_customvueadmin-0.2.5/custom_admin/templates/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.322184 django_customvueadmin-0.2.5/custom_admin/templates/custom_admin/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1351 2024-05-27 09:43:23.000000 django_customvueadmin-0.2.5/custom_admin/templates/custom_admin/admin_index.html
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.322184 django_customvueadmin-0.2.5/custom_admin/utils/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       35 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.5/custom_admin/utils/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1976 2024-04-11 17:58:41.000000 django_customvueadmin-0.2.5/custom_admin/utils/async_mixin.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2425 2024-04-09 09:57:39.000000 django_customvueadmin-0.2.5/custom_admin/utils/colors.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      570 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.5/custom_admin/utils/get_schema.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      593 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.5/custom_admin/utils/register_admin_viewsets.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.322184 django_customvueadmin-0.2.5/custom_admin/views/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       40 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.5/custom_admin/views/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1316 2024-05-27 09:42:41.000000 django_customvueadmin-0.2.5/custom_admin/views/admin_page.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:43:43.322184 django_customvueadmin-0.2.5/django_customvueadmin.egg-info/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2886 2024-05-27 09:43:43.000000 django_customvueadmin-0.2.5/django_customvueadmin.egg-info/PKG-INFO
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4196 2024-05-27 09:43:43.000000 django_customvueadmin-0.2.5/django_customvueadmin.egg-info/SOURCES.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-05-27 09:43:43.000000 django_customvueadmin-0.2.5/django_customvueadmin.egg-info/dependency_links.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-05-27 09:43:43.000000 django_customvueadmin-0.2.5/django_customvueadmin.egg-info/not-zip-safe
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       13 2024-05-27 09:43:43.000000 django_customvueadmin-0.2.5/django_customvueadmin.egg-info/top_level.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      222 2024-04-11 09:22:36.000000 django_customvueadmin-0.2.5/pyproject.toml
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1000 2024-05-27 09:43:43.322184 django_customvueadmin-0.2.5/setup.cfg
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.134348 django_customvueadmin-0.2.6/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1073 2024-04-26 14:57:56.000000 django_customvueadmin-0.2.6/LICENSE
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      209 2024-04-11 14:26:38.000000 django_customvueadmin-0.2.6/MANIFEST.in
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2886 2024-05-27 09:58:44.134348 django_customvueadmin-0.2.6/PKG-INFO
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2053 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/README.rst
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.117680 django_customvueadmin-0.2.6/custom_admin/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       45 2024-05-27 09:57:51.000000 django_customvueadmin-0.2.6/custom_admin/__init__.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.117680 django_customvueadmin-0.2.6/custom_admin/api/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       86 2024-04-19 14:02:39.000000 django_customvueadmin-0.2.6/custom_admin/api/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1529 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/api/action_functions.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.117680 django_customvueadmin-0.2.6/custom_admin/api/actions/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      139 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.6/custom_admin/api/actions/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      985 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/api/actions/delete_action.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2538 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/api/actions/export_csv_action.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2723 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/api/actions/view_actions_mixin.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1724 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/api/backends.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.117680 django_customvueadmin-0.2.6/custom_admin/api/fields/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      403 2024-05-06 15:09:48.000000 django_customvueadmin-0.2.6/custom_admin/api/fields/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      381 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.6/custom_admin/api/fields/base.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      811 2024-04-23 15:22:53.000000 django_customvueadmin-0.2.6/custom_admin/api/fields/char.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1233 2024-04-23 15:23:30.000000 django_customvueadmin-0.2.6/custom_admin/api/fields/choice.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3695 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/api/fields/files.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      157 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.6/custom_admin/api/fields/int.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      326 2024-05-06 16:10:42.000000 django_customvueadmin-0.2.6/custom_admin/api/fields/json.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      343 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.6/custom_admin/api/fields/numbers.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3871 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.6/custom_admin/api/fields/relation.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.121014 django_customvueadmin-0.2.6/custom_admin/api/filters/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      165 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/api/filters/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1623 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/api/filters/base_admin_filter.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.6/custom_admin/api/filters/choices.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      733 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/api/filters/date_range.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1445 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/api/inline_relation.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.121014 django_customvueadmin-0.2.6/custom_admin/api/inlines/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      305 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.6/custom_admin/api/inlines/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      601 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.6/custom_admin/api/inlines/export_csv_inline.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1595 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/api/inlines/inline_graph.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2129 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.6/custom_admin/api/inlines/inline_table.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       61 2024-03-29 18:33:05.000000 django_customvueadmin-0.2.6/custom_admin/api/inlines/inlines_type.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      135 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.6/custom_admin/api/inlines/interfaces.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4154 2024-04-02 18:13:36.000000 django_customvueadmin-0.2.6/custom_admin/api/inlines/view_inline_mixin.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      893 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.6/custom_admin/api/permissions.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.121014 django_customvueadmin-0.2.6/custom_admin/api/serializers/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      207 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.6/custom_admin/api/serializers/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      737 2024-04-19 13:32:46.000000 django_customvueadmin-0.2.6/custom_admin/api/serializers/auth_response.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5491 2024-05-06 15:09:50.000000 django_customvueadmin-0.2.6/custom_admin/api/serializers/base_serializer.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.121014 django_customvueadmin-0.2.6/custom_admin/api/tests/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/api/tests/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2317 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/api/tests/test_filters.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      517 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/api/tests/test_scheme_get.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      550 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/api/tests/urls.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      599 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/api/urls.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.121014 django_customvueadmin-0.2.6/custom_admin/api/views/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      414 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/api/views/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5829 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/api/views/autocomplete.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     8432 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/api/views/base_admin_viewset.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.121014 django_customvueadmin-0.2.6/custom_admin/api/views/defaults/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      131 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/api/views/defaults/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2080 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/api/views/defaults/admin_log.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      366 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/api/views/defaults/groups.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      529 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/api/views/defaults/permissions.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      909 2024-04-23 23:45:01.000000 django_customvueadmin-0.2.6/custom_admin/api/views/get_sections.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1517 2024-04-11 17:29:22.000000 django_customvueadmin-0.2.6/custom_admin/api/views/token_auth.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      974 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/api/viewset_info.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.124347 django_customvueadmin-0.2.6/custom_admin/controllers/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-04-19 14:01:33.000000 django_customvueadmin-0.2.6/custom_admin/controllers/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3475 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/controllers/admin_log_manager.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3823 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/controllers/custom_metadata.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3078 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/controllers/filters_schema.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     9232 2024-05-27 09:16:40.000000 django_customvueadmin-0.2.6/custom_admin/controllers/schema_generator.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.124347 django_customvueadmin-0.2.6/custom_admin/management/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-04-15 16:06:07.000000 django_customvueadmin-0.2.6/custom_admin/management/__init__.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.124347 django_customvueadmin-0.2.6/custom_admin/management/commands/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-04-15 16:06:19.000000 django_customvueadmin-0.2.6/custom_admin/management/commands/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1300 2024-04-15 16:52:15.000000 django_customvueadmin-0.2.6/custom_admin/management/commands/custom_admin_viewsets_list.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.124347 django_customvueadmin-0.2.6/custom_admin/migrations/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1695 2024-04-11 18:20:54.000000 django_customvueadmin-0.2.6/custom_admin/migrations/0001_initial.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 18:20:54.000000 django_customvueadmin-0.2.6/custom_admin/migrations/__init__.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.124347 django_customvueadmin-0.2.6/custom_admin/models/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       32 2024-03-11 07:49:25.000000 django_customvueadmin-0.2.6/custom_admin/models/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1469 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.6/custom_admin/models/admin_log.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.114347 django_customvueadmin-0.2.6/custom_admin/static/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.127681 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2238 2024-05-27 09:58:38.000000 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/favicon.ico
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)   752746 2024-05-27 09:58:38.000000 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/index-C6_9c0_p.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1681722 2024-05-27 09:58:38.000000 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/index-DYa2T7lY.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)   385360 2024-05-27 09:58:38.000000 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/materialdesignicons-webfont-CYDMK1kx.woff2
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)   561776 2024-05-27 09:58:38.000000 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/materialdesignicons-webfont-CgCzGbLl.woff
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1243500 2024-05-27 09:58:38.000000 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/materialdesignicons-webfont-D3kAzl71.ttf
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1243720 2024-05-27 09:58:38.000000 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/materialdesignicons-webfont-DttUABo4.eot
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.131014 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.131014 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/dark-first/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4788 2024-05-27 09:58:38.000000 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/dark-first/content.min.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    50376 2024-05-27 09:58:38.000000 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/dark-first/skin.min.css
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.131014 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/dark-slim/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4730 2024-05-27 09:58:38.000000 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/dark-slim/content.min.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    49965 2024-05-27 09:58:38.000000 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/dark-slim/skin.min.css
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.131014 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/img/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    14708 2024-05-27 09:58:38.000000 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/img/example.png
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    15764 2024-05-27 09:58:38.000000 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/img/tinymce.woff2
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.131014 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/lightgray/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3193 2024-05-27 09:58:38.000000 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/lightgray/content.min.css
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.131014 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/lightgray/fonts/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     7664 2024-05-27 09:58:38.000000 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/lightgray/fonts/tinymce.woff
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    38232 2024-05-27 09:58:38.000000 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/lightgray/skin.min.css
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.117680 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/plugins/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.131014 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/plugins/accordion/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.131014 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/plugins/accordion/css/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-05-27 09:58:38.000000 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/plugins/accordion/css/accordion.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1251 2024-05-27 09:58:38.000000 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/plugins/accordion/plugin.js
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.117680 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/plugins/codesample/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.131014 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1736 2024-05-27 09:58:38.000000 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/prism.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1171290 2024-05-27 09:58:38.000000 django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/tinymce.min.js
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.117680 django_customvueadmin-0.2.6/custom_admin/templates/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.131014 django_customvueadmin-0.2.6/custom_admin/templates/custom_admin/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1351 2024-05-27 09:58:38.000000 django_customvueadmin-0.2.6/custom_admin/templates/custom_admin/admin_index.html
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.134348 django_customvueadmin-0.2.6/custom_admin/utils/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       35 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.6/custom_admin/utils/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1976 2024-04-11 17:58:41.000000 django_customvueadmin-0.2.6/custom_admin/utils/async_mixin.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2425 2024-04-09 09:57:39.000000 django_customvueadmin-0.2.6/custom_admin/utils/colors.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      570 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.6/custom_admin/utils/get_schema.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      593 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.6/custom_admin/utils/register_admin_viewsets.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.134348 django_customvueadmin-0.2.6/custom_admin/views/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       40 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.6/custom_admin/views/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1316 2024-05-27 09:42:41.000000 django_customvueadmin-0.2.6/custom_admin/views/admin_page.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 09:58:44.134348 django_customvueadmin-0.2.6/django_customvueadmin.egg-info/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2886 2024-05-27 09:58:44.000000 django_customvueadmin-0.2.6/django_customvueadmin.egg-info/PKG-INFO
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4196 2024-05-27 09:58:44.000000 django_customvueadmin-0.2.6/django_customvueadmin.egg-info/SOURCES.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-05-27 09:58:44.000000 django_customvueadmin-0.2.6/django_customvueadmin.egg-info/dependency_links.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-05-27 09:58:43.000000 django_customvueadmin-0.2.6/django_customvueadmin.egg-info/not-zip-safe
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       13 2024-05-27 09:58:44.000000 django_customvueadmin-0.2.6/django_customvueadmin.egg-info/top_level.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      222 2024-04-11 09:22:36.000000 django_customvueadmin-0.2.6/pyproject.toml
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1000 2024-05-27 09:58:44.134348 django_customvueadmin-0.2.6/setup.cfg
```

### Comparing `django_customvueadmin-0.2.5/LICENSE` & `django_customvueadmin-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/PKG-INFO` & `django_customvueadmin-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-customvueadmin
-Version: 0.2.5
+Version: 0.2.6
 Summary: A custom admin interface providing backend via DRF and frontend via Vue and Element UI that tries to Keep It Simple.
 Home-page: https://innova-group-llc.github.io/custom_admin_docs/
 License: BSD-3-Clause
 Project-URL: Documentation, https://innova-group-llc.github.io/custom_admin_docs/
 Project-URL: Source, https://github.com/Innova-Group-LLC/custom_admin
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `django_customvueadmin-0.2.5/README.rst` & `django_customvueadmin-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/action_functions.py` & `django_customvueadmin-0.2.6/custom_admin/api/action_functions.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/actions/delete_action.py` & `django_customvueadmin-0.2.6/custom_admin/api/actions/delete_action.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/actions/export_csv_action.py` & `django_customvueadmin-0.2.6/custom_admin/api/actions/export_csv_action.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/actions/view_actions_mixin.py` & `django_customvueadmin-0.2.6/custom_admin/api/actions/view_actions_mixin.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/backends.py` & `django_customvueadmin-0.2.6/custom_admin/api/backends.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/fields/char.py` & `django_customvueadmin-0.2.6/custom_admin/api/fields/char.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/fields/choice.py` & `django_customvueadmin-0.2.6/custom_admin/api/fields/choice.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/fields/files.py` & `django_customvueadmin-0.2.6/custom_admin/api/fields/files.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/fields/relation.py` & `django_customvueadmin-0.2.6/custom_admin/api/fields/relation.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/filters/base_admin_filter.py` & `django_customvueadmin-0.2.6/custom_admin/api/filters/base_admin_filter.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/filters/date_range.py` & `django_customvueadmin-0.2.6/custom_admin/api/filters/date_range.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/inline_relation.py` & `django_customvueadmin-0.2.6/custom_admin/api/inline_relation.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/inlines/export_csv_inline.py` & `django_customvueadmin-0.2.6/custom_admin/api/inlines/export_csv_inline.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/inlines/inline_graph.py` & `django_customvueadmin-0.2.6/custom_admin/api/inlines/inline_graph.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/inlines/inline_table.py` & `django_customvueadmin-0.2.6/custom_admin/api/inlines/inline_table.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/inlines/view_inline_mixin.py` & `django_customvueadmin-0.2.6/custom_admin/api/inlines/view_inline_mixin.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/permissions.py` & `django_customvueadmin-0.2.6/custom_admin/api/permissions.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/serializers/auth_response.py` & `django_customvueadmin-0.2.6/custom_admin/api/serializers/auth_response.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/serializers/base_serializer.py` & `django_customvueadmin-0.2.6/custom_admin/api/serializers/base_serializer.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/tests/test_filters.py` & `django_customvueadmin-0.2.6/custom_admin/api/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/tests/test_scheme_get.py` & `django_customvueadmin-0.2.6/custom_admin/api/tests/test_scheme_get.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/tests/urls.py` & `django_customvueadmin-0.2.6/custom_admin/api/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/urls.py` & `django_customvueadmin-0.2.6/custom_admin/api/urls.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/views/autocomplete.py` & `django_customvueadmin-0.2.6/custom_admin/api/views/autocomplete.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/views/base_admin_viewset.py` & `django_customvueadmin-0.2.6/custom_admin/api/views/base_admin_viewset.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/views/defaults/admin_log.py` & `django_customvueadmin-0.2.6/custom_admin/api/views/defaults/admin_log.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/views/defaults/permissions.py` & `django_customvueadmin-0.2.6/custom_admin/api/views/defaults/permissions.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/views/get_sections.py` & `django_customvueadmin-0.2.6/custom_admin/api/views/get_sections.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/views/token_auth.py` & `django_customvueadmin-0.2.6/custom_admin/api/views/token_auth.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/api/viewset_info.py` & `django_customvueadmin-0.2.6/custom_admin/api/viewset_info.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/controllers/admin_log_manager.py` & `django_customvueadmin-0.2.6/custom_admin/controllers/admin_log_manager.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/controllers/custom_metadata.py` & `django_customvueadmin-0.2.6/custom_admin/controllers/custom_metadata.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/controllers/filters_schema.py` & `django_customvueadmin-0.2.6/custom_admin/controllers/filters_schema.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/controllers/schema_generator.py` & `django_customvueadmin-0.2.6/custom_admin/controllers/schema_generator.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/management/commands/custom_admin_viewsets_list.py` & `django_customvueadmin-0.2.6/custom_admin/management/commands/custom_admin_viewsets_list.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/migrations/0001_initial.py` & `django_customvueadmin-0.2.6/custom_admin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/models/admin_log.py` & `django_customvueadmin-0.2.6/custom_admin/models/admin_log.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/static/custom_admin/favicon.ico` & `django_customvueadmin-0.2.6/custom_admin/static/custom_admin/favicon.ico`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/static/custom_admin/index-CKHFT4s-.js` & `django_customvueadmin-0.2.6/custom_admin/static/custom_admin/index-DYa2T7lY.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
     writable: !0,
     value: n
 }) : e[t] = n;
 var u9 = (e, t) => () => (t || e((t = {
     exports: {}
 }).exports, t), t.exports);
 var Ye = (e, t, n) => (l9(e, typeof t != "symbol" ? t + "" : t, n), n);
-var r7e = u9((d7e, ob) => {
+var a7e = u9((f7e, ob) => {
     (function() {
         const t = document.createElement("link").relList;
         if (t && t.supports && t.supports("modulepreload")) return;
         for (const a of document.querySelectorAll('link[rel="modulepreload"]')) r(a);
         new MutationObserver(a => {
             for (const i of a)
                 if (i.type === "childList")
@@ -48,15 +48,15 @@
             s: n
         }),
         d9 = e => JSON.stringify(e).replace(/\u2028/g, "\\u2028").replace(/\u2029/g, "\\u2029").replace(/\u0027/g, "\\u0027"),
         Da = e => typeof e == "number" && isFinite(e),
         f9 = e => IV(e) === "[object Date]",
         wc = e => IV(e) === "[object RegExp]",
         g_ = e => en(e) && Object.keys(e).length === 0,
-        ii = Object.assign;
+        si = Object.assign;
     let vD;
     const Kl = () => vD || (vD = typeof globalThis < "u" ? globalThis : typeof self < "u" ? self : typeof window < "u" ? window : typeof global < "u" ? global : {});
 
     function gD(e) {
         return e.replace(/</g, "&lt;").replace(/>/g, "&gt;").replace(/"/g, "&quot;").replace(/'/g, "&apos;")
     }
     const h9 = Object.prototype.hasOwnProperty;
@@ -1412,15 +1412,15 @@
                         R = E === "vnode" && Tr(O) && A ? O[0] : O;
                     return A ? h(A)(R, E) : R
                 },
                 message: f,
                 type: _,
                 interpolate: g,
                 normalize: p,
-                values: ii({}, s, u)
+                values: si({}, s, u)
             };
         return w
     }
     let vv = null;
 
     function d7(e) {
         vv = e
@@ -1583,15 +1583,15 @@
             },
             o = en(e.datetimeFormats) ? e.datetimeFormats : {
                 [a]: {}
             },
             u = en(e.numberFormats) ? e.numberFormats : {
                 [a]: {}
             },
-            c = ii({}, e.modifiers || {}, _7()),
+            c = si({}, e.modifiers || {}, _7()),
             f = e.pluralRules || {},
             h = vr(e.missing) ? e.missing : null,
             p = gn(e.missingWarn) || wc(e.missingWarn) ? e.missingWarn : !0,
             g = gn(e.fallbackWarn) || wc(e.fallbackWarn) ? e.fallbackWarn : !0,
             _ = !!e.fallbackFormat,
             y = !!e.unresolving,
             w = vr(e.postTranslation) ? e.postTranslation : null,
@@ -1801,15 +1801,15 @@
             const W = {
                 timestamp: Date.now(),
                 key: wt(u) ? u : Fs(x) ? x.key : "",
                 locale: k || (Fs(x) ? x.locale : ""),
                 format: wt(x) ? x : Fs(x) ? x.source : "",
                 message: B
             };
-            W.meta = ii({}, e.__meta, $7() || {}), h7(W)
+            W.meta = si({}, e.__meta, $7() || {}), h7(W)
         }
         return B
     }
 
     function M7(e) {
         Tr(e.list) ? e.list = e.list.map(t => wt(t) ? gD(t) : t) : Jn(e.named) && Object.keys(e.named).forEach(t => {
             wt(e.named[t]) && (e.named[t] = gD(e.named[t]))
@@ -1854,15 +1854,15 @@
         return t(n)
     }
 
     function Bk(...e) {
         const [t, n, r] = e, a = {};
         if (!wt(t) && !Da(t) && !Fs(t) && !Ih(t)) throw rl(yo.INVALID_ARGUMENT);
         const i = Da(t) ? String(t) : (Fs(t), t);
-        return Da(n) ? a.plural = n : wt(n) ? a.default = n : en(n) && !g_(n) ? a.named = n : Tr(n) && (a.list = n), Da(r) ? a.plural = r : wt(r) ? a.default = r : en(r) && ii(a, r), [i, a]
+        return Da(n) ? a.plural = n : wt(n) ? a.default = n : en(n) && !g_(n) ? a.named = n : Tr(n) && (a.list = n), Da(r) ? a.plural = r : wt(r) ? a.default = r : en(r) && si(a, r), [i, a]
     }
 
     function I7(e, t, n, r, a, i) {
         return {
             locale: t,
             key: n,
             warnHtmlMessage: a,
@@ -1923,15 +1923,15 @@
             S, k = null;
         const C = "datetime format";
         for (let A = 0; A < y.length && (S = y[A], w = n[S] || {}, k = w[u], !en(k)); A++) eT(e, u, S, p, C);
         if (!en(k) || !wt(S)) return r ? b_ : u;
         let x = `${S}__${u}`;
         g_(h) || (x = `${x}__${JSON.stringify(h)}`);
         let E = o.get(x);
-        return E || (E = new Intl.DateTimeFormat(S, ii({}, k, h)), o.set(x, E)), g ? E.formatToParts(c) : E.format(c)
+        return E || (E = new Intl.DateTimeFormat(S, si({}, k, h)), o.set(x, E)), g ? E.formatToParts(c) : E.format(c)
     }
     const XV = ["localeMatcher", "weekday", "era", "year", "month", "day", "hour", "minute", "second", "timeZoneName", "formatMatcher", "hour12", "timeZone", "dateStyle", "timeStyle", "calendar", "dayPeriod", "numberingSystem", "hourCycle", "fractionalSecondDigits"];
 
     function Hk(...e) {
         const [t, n, r, a] = e, i = {};
         let s = {},
             o;
@@ -1982,15 +1982,15 @@
             S, k = null;
         const C = "number format";
         for (let A = 0; A < y.length && (S = y[A], w = n[S] || {}, k = w[u], !en(k)); A++) eT(e, u, S, p, C);
         if (!en(k) || !wt(S)) return r ? b_ : u;
         let x = `${S}__${u}`;
         g_(h) || (x = `${x}__${JSON.stringify(h)}`);
         let E = o.get(x);
-        return E || (E = new Intl.NumberFormat(S, ii({}, k, h)), o.set(x, E)), g ? E.formatToParts(c) : E.format(c)
+        return E || (E = new Intl.NumberFormat(S, si({}, k, h)), o.set(x, E)), g ? E.formatToParts(c) : E.format(c)
     }
     const JV = ["localeMatcher", "style", "currency", "currencyDisplay", "currencySign", "useGrouping", "minimumIntegerDigits", "minimumFractionDigits", "maximumFractionDigits", "minimumSignificantDigits", "maximumSignificantDigits", "compactDisplay", "notation", "signDisplay", "unit", "unitDisplay", "roundingMode", "roundingPriority", "roundingIncrement", "trailingZeroDisplay"];
 
     function Wk(...e) {
         const [t, n, r, a] = e, i = {};
         let s = {};
         if (!Da(t)) throw rl(yo.INVALID_ARGUMENT);
@@ -3142,15 +3142,15 @@
     }
 
     function Sa(e) {
         return gT(xK, e)
     }
 
     function gT(e, t, n = !0, r = !1) {
-        const a = La || ai;
+        const a = La || ii;
         if (a) {
             const i = a.type;
             if (e === vT) {
                 const o = SX(i, !1);
                 if (o && (o === t || o === qs(t) || o === yl(qs(t)))) return i
             }
             const s = GD(a[e] || i[e], t) || GD(a.appContext[e], t);
@@ -3395,15 +3395,15 @@
     } = kr) {
         if (t && i) {
             const A = t;
             t = (...O) => {
                 A(...O), E()
             }
         }
-        const u = ai,
+        const u = ii,
             c = A => r === !0 ? A : Dd(A, r === !1 ? 1 : void 0);
         let f, h = !1,
             p = !1;
         if (Pr(e) ? (f = () => e.value, h = fb(e)) : Um(e) ? (f = () => c(e), h = !0) : Ht(e) ? (p = !0, h = e.some(A => Um(A) || fb(A)), f = () => e.map(A => {
                 if (Pr(A)) return A.value;
                 if (Um(A)) return c(A);
                 if (Zt(A)) return hc(A, u, 2)
@@ -3706,15 +3706,15 @@
         jj(e, "a", t)
     }
 
     function Vj(e, t) {
         jj(e, "da", t)
     }
 
-    function jj(e, t, n = ai) {
+    function jj(e, t, n = ii) {
         const r = e.__wdc || (e.__wdc = () => {
             let a = n;
             for (; a;) {
                 if (a.isDeactivated) return;
                 a = a.parent
             }
             return e()
@@ -3728,39 +3728,39 @@
     function WK(e, t, n, r) {
         const a = E_(t, e, r, !0);
         Io(() => {
             rT(r[t], a)
         }, n)
     }
 
-    function E_(e, t, n = ai, r = !1) {
+    function E_(e, t, n = ii, r = !1) {
         if (n) {
             const a = n[e] || (n[e] = []),
                 i = t.__weh || (t.__weh = (...s) => {
                     if (n.isUnmounted) return;
                     Ic();
                     const o = ig(n),
                         u = Ws(t, n, e, s);
                     return o(), Lc(), u
                 });
             return r ? a.unshift(i) : a.push(i), i
         }
     }
-    const gu = e => (t, n = ai) => (!x_ || e === "sp") && E_(e, (...r) => t(...r), n),
+    const gu = e => (t, n = ii) => (!x_ || e === "sp") && E_(e, (...r) => t(...r), n),
         ag = gu("bm"),
         zn = gu("m"),
         wT = gu("bu"),
         ST = gu("u"),
         Ei = gu("bum"),
         Io = gu("um"),
         UK = gu("sp"),
         zK = gu("rtg"),
         YK = gu("rtc");
 
-    function qK(e, t = ai) {
+    function qK(e, t = ii) {
         E_("ec", e, t)
     }
 
     function Et(e, t, n, r) {
         let a;
         const i = n;
         if (Ht(e) || Ur(e)) {
@@ -3779,15 +3779,15 @@
                     a[o] = t(e[c], c, o, i)
                 }
             }
         else a = [];
         return a
     }
 
-    function si(e, t) {
+    function oi(e, t) {
         for (let n = 0; n < t.length; n++) {
             const r = t[n];
             if (Ht(r))
                 for (let a = 0; a < r.length; a++) e[r[a].name] = r[a].fn;
             else r && (e[r.name] = r.key ? (...a) => {
                 const i = r.fn(...a);
                 return i && (i.key = r.key), i
@@ -4203,23 +4203,23 @@
             };
             return u
         }
     }
     let qm = null;
 
     function ur(e, t) {
-        if (ai) {
-            let n = ai.provides;
-            const r = ai.parent && ai.parent.provides;
-            r === n && (n = ai.provides = Object.create(r)), n[e] = t
+        if (ii) {
+            let n = ii.provides;
+            const r = ii.parent && ii.parent.provides;
+            r === n && (n = ii.provides = Object.create(r)), n[e] = t
         }
     }
 
     function Ut(e, t, n = !1) {
-        const r = ai || La;
+        const r = ii || La;
         if (r || qm) {
             const a = r ? r.parent == null ? r.vnode.appContext && r.vnode.appContext.provides : r.parent.provides : qm._context.provides;
             if (a && e in a) return a[e];
             if (arguments.length > 1) return n && Zt(t) ? t.call(r && r.proxy) : t
         }
     }
     const Uj = {},
@@ -4763,20 +4763,20 @@
                     else
                         for (yt = Fe; yt <= Ke; yt++)
                             if (sa[yt - Fe] === 0 && Jo(Ie, J[yt])) {
                                 Se = yt;
                                 break
                             } Se === void 0 ? q(Ie, ye, De, !0) : (sa[Se - Fe] = we + 1, Se >= Nr ? Nr = Se : Vn = !0, y(Ie, J[Se], oe, null, ye, De, He, re, ie), At++)
                 }
-                const Ka = Vn ? dX(sa) : yh;
-                for (yt = Ka.length - 1, we = Ln - 1; we >= 0; we--) {
+                const Xa = Vn ? dX(sa) : yh;
+                for (yt = Xa.length - 1, we = Ln - 1; we >= 0; we--) {
                     const Ie = Fe + we,
                         Se = J[Ie],
                         Qe = Ie + 1 < Re ? J[Ie + 1].el : le;
-                    sa[we] === 0 ? y(null, Se, oe, Qe, ye, De, He, re, ie) : Vn && (yt < 0 || we !== Ka[yt] ? N(Se, oe, Qe, 2) : yt--)
+                    sa[we] === 0 ? y(null, Se, oe, Qe, ye, De, He, re, ie) : Vn && (yt < 0 || we !== Xa[yt] ? N(Se, oe, Qe, 2) : yt--)
                 }
             }
         }, N = (K, J, oe, le, ye = null) => {
             const {
                 el: De,
                 type: He,
                 transition: re,
@@ -5373,35 +5373,35 @@
                 ec: null,
                 sp: null
             };
         return i.ctx = {
             _: i
         }, i.root = t ? t.root : i, i.emit = $K.bind(null, i), e.ce && e.ce(i), i
     }
-    let ai = null;
-    const cu = () => ai || La;
+    let ii = null;
+    const cu = () => ii || La;
     let mb, r$;
     {
         const e = aj(),
             t = (n, r) => {
                 let a;
                 return (a = e[n]) || (a = e[n] = []), a.push(r), i => {
                     a.length > 1 ? a.forEach(s => s(i)) : a[0](i)
                 }
             };
-        mb = t("__VUE_INSTANCE_SETTERS__", n => ai = n), r$ = t("__VUE_SSR_SETTERS__", n => x_ = n)
+        mb = t("__VUE_INSTANCE_SETTERS__", n => ii = n), r$ = t("__VUE_SSR_SETTERS__", n => x_ = n)
     }
     const ig = e => {
-            const t = ai;
+            const t = ii;
             return mb(e), e.scope.on(), () => {
                 e.scope.off(), mb(t)
             }
         },
         lI = () => {
-            ai && ai.scope.off(), mb(null)
+            ii && ii.scope.off(), mb(null)
         };
 
     function aB(e) {
         return e.vnode.shapeFlag & 4
     }
     let x_ = !1;
 
@@ -6410,15 +6410,15 @@
         function q(...Pe) {
             return N(Fe => Reflect.apply(DD, null, [Fe, ...Pe]), () => Bk(...Pe), "translate", Fe => Reflect.apply(Fe.t, Fe, [...Pe]), Fe => Fe, Fe => wt(Fe))
         }
 
         function M(...Pe) {
             const [Fe, bt, yt] = Pe;
             if (yt && !Jn(yt)) throw qa(Fa.INVALID_ARGUMENT);
-            return q(Fe, bt, ii({
+            return q(Fe, bt, si({
                 resolvedMessage: !0
             }, yt || {}))
         }
 
         function P(...Pe) {
             return N(Fe => Reflect.apply(ID, null, [Fe, ...Pe]), () => Hk(...Pe), "datetime format", Fe => Reflect.apply(Fe.d, Fe, [...Pe]), () => TD, Fe => wt(Fe))
         }
@@ -6520,27 +6520,27 @@
         }
 
         function re(Pe, Fe) {
             p.value[Pe] = Fe, F.datetimeFormats = p.value, LD(F, Pe, Fe)
         }
 
         function ie(Pe, Fe) {
-            p.value[Pe] = ii(p.value[Pe] || {}, Fe), F.datetimeFormats = p.value, LD(F, Pe, Fe)
+            p.value[Pe] = si(p.value[Pe] || {}, Fe), F.datetimeFormats = p.value, LD(F, Pe, Fe)
         }
 
         function we(Pe) {
             return g.value[Pe] || {}
         }
 
         function Re(Pe, Fe) {
             g.value[Pe] = Fe, F.numberFormats = g.value, ND(F, Pe, Fe)
         }
 
         function nt(Pe, Fe) {
-            g.value[Pe] = ii(g.value[Pe] || {}, Fe), F.numberFormats = g.value, ND(F, Pe, Fe)
+            g.value[Pe] = si(g.value[Pe] || {}, Fe), F.numberFormats = g.value, ND(F, Pe, Fe)
         }
         OI++, n && lb && (st(n.locale, Pe => {
             u && (c.value = Pe, F.locale = Pe, pm(F, c.value, f.value))
         }), st(n.fallbackLocale, Pe => {
             u && (f.value = Pe, F.fallbackLocale = Pe, pm(F, c.value, f.value))
         }));
         const Ke = {
@@ -6630,15 +6630,15 @@
             p = !!e.escapeParameterHtml,
             g = gn(e.sync) ? e.sync : !0;
         let _ = e.messages;
         if (en(e.sharedMessages)) {
             const A = e.sharedMessages;
             _ = Object.keys(A).reduce((R, F) => {
                 const U = R[F] || (R[F] = {});
-                return ii(U, A[F]), R
+                return si(U, A[F]), R
             }, _ || {})
         }
         const {
             __i18n: y,
             __root: w,
             __injectWithOption: S
         } = e, k = e.datetimeFormats, C = e.numberFormats, x = e.flatJson, E = e.translateExistCompatible;
@@ -6861,15 +6861,15 @@
     }
 
     function $B(e) {
         return Ne
     }
     const dJ = Tt({
             name: "i18n-t",
-            props: ii({
+            props: si({
                 keypath: {
                     type: String,
                     required: !0
                 },
                 plural: {
                     type: [Number, String],
                     validator: e => Da(e) || !isNaN(e)
@@ -6885,15 +6885,15 @@
                 });
                 return () => {
                     const i = Object.keys(n).filter(h => h !== "_"),
                         s = {};
                     e.locale && (s.locale = e.locale), e.plural !== void 0 && (s.plural = wt(e.plural) ? +e.plural : e.plural);
                     const o = cJ(t, i),
                         u = a[i$](e.keypath, o, s),
-                        c = ii({}, r),
+                        c = si({}, r),
                         f = wt(e.tag) || Jn(e.tag) ? e.tag : $B();
                     return ba(f, c, u)
                 }
             }
         }),
         MI = dJ;
 
@@ -6907,36 +6907,36 @@
             attrs: i
         } = t;
         return () => {
             const s = {
                 part: !0
             };
             let o = {};
-            e.locale && (s.locale = e.locale), wt(e.format) ? s.key = e.format : Jn(e.format) && (wt(e.format.key) && (s.key = e.format.key), o = Object.keys(e.format).reduce((p, g) => n.includes(g) ? ii({}, p, {
+            e.locale && (s.locale = e.locale), wt(e.format) ? s.key = e.format : Jn(e.format) && (wt(e.format.key) && (s.key = e.format.key), o = Object.keys(e.format).reduce((p, g) => n.includes(g) ? si({}, p, {
                 [g]: e.format[g]
             }) : p, {}));
             const u = r(e.value, s, o);
             let c = [s.key];
             Tr(u) ? c = u.map((p, g) => {
                 const _ = a[p.type],
                     y = _ ? _({
                         [p.type]: p.value,
                         index: g,
                         parts: u
                     }) : [p.value];
                 return fJ(y) && (y[0].key = `${p.type}-${g}`), y
             }) : wt(u) && (c = [u]);
-            const f = ii({}, i),
+            const f = si({}, i),
                 h = wt(e.tag) || Jn(e.tag) ? e.tag : $B();
             return ba(h, f, c)
         }
     }
     const hJ = Tt({
             name: "i18n-n",
-            props: ii({
+            props: si({
                 value: {
                     type: Number,
                     required: !0
                 },
                 format: {
                     type: [String, Object]
                 }
@@ -6948,15 +6948,15 @@
                 });
                 return CB(e, t, JV, (...r) => n[o$](...r))
             }
         }),
         DI = hJ,
         pJ = Tt({
             name: "i18n-d",
-            props: ii({
+            props: si({
                 value: {
                     type: [Number, Date],
                     required: !0
                 },
                 format: {
                     type: [String, Object]
                 }
@@ -7165,15 +7165,15 @@
         if (i === "parent") {
             let u = CJ(n, t, e.__useComponent);
             return u == null && (u = r), u
         }
         const s = n;
         let o = s.__getInstance(t);
         if (o == null) {
-            const u = ii({}, e);
+            const u = si({}, e);
             "__i18n" in a && (u.__i18n = a.__i18n), r && (u.__root = r), o = ET(u), s.__composerExtend && (o[l$] = s.__composerExtend(o)), PJ(s, t, o), s.__setInstance(t, o)
         }
         return o
     }
 
     function wJ(e, t, n) {
         const r = k_();
@@ -7689,15 +7689,15 @@
             clearTimeout(n), n = setTimeout(() => e(...i), ke(t))
         };
         return r.clear = () => {
             clearTimeout(n)
         }, r.immediate = e, r
     }
 
-    function oi(e) {
+    function li(e) {
         let t = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 0,
             n = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : 1;
         return Math.max(t, Math.min(n, e))
     }
 
     function bb(e) {
         const t = e.toString().trim();
@@ -8145,15 +8145,15 @@
         ],
         iZ = e => e <= .04045 ? e / 12.92 : ((e + .055) / 1.055) ** 2.4;
 
     function jB(e) {
         const t = Array(3),
             n = rZ,
             r = nZ;
-        for (let a = 0; a < 3; ++a) t[a] = Math.round(oi(n(r[a][0] * e[0] + r[a][1] * e[1] + r[a][2] * e[2])) * 255);
+        for (let a = 0; a < 3; ++a) t[a] = Math.round(li(n(r[a][0] * e[0] + r[a][1] * e[1] + r[a][2] * e[2])) * 255);
         return {
             r: t[0],
             g: t[1],
             b: t[2]
         }
     }
 
@@ -9166,21 +9166,22 @@
         },
         VT = _J({
             legacy: !1,
             locale: hp(),
             fallbackLocale: "en",
             messages: EZ
         });
-    var li = {
+    var Ga = {
         title: "Dev Admin",
-        backend_prefix: "http://localhost:8001/custom_admin/"
+        backend_prefix: "http://localhost:8001/custom_admin/",
+        static_prefix: "/static/custom_admin"
     };
-    li = JSON.parse(document.getElementById("settings").dataset.json);
-    var li;
-    console.log("config_dataset", li, "prod", !0);
+    Ga = JSON.parse(document.getElementById("settings").dataset.json), Ga.static_prefix = "/static/custom_admin";
+    var Ga;
+    console.log("config_dataset", Ga, "prod", !0);
     const JB = "SETTINGS",
         xZ = {
             page_size: 25,
             theme: "light",
             wysiwygSkin: "dark-first"
         };
 
@@ -10325,15 +10326,15 @@
         }
         f += i.offset, f = PQ(u, f, !!s, !!n);
         const h = u[a] ?? 0;
         if (f === h) return Promise.resolve(f);
         const p = performance.now();
         return new Promise(g => requestAnimationFrame(function _(y) {
             const S = (y - p) / i.duration,
-                k = Math.floor(h + (f - h) * c(oi(S, 0, 1)));
+                k = Math.floor(h + (f - h) * c(li(S, 0, 1)));
             if (u[a] = k, S >= 1 && Math.abs(k - u[a]) < 10) return g(f);
             if (S > 2) return g(u[a]);
             requestAnimationFrame(_)
         }))
     }
 
     function TQ() {
@@ -12637,15 +12638,15 @@
 
     function $$(e) {
         var t, n, r;
         const a = typeof e == "string" ? e : ((t = e.currentTarget) == null ? void 0 : t.id) || ((n = e.target) == null ? void 0 : n.id),
             i = document.getElementById(a);
         i && i.removeEventListener("animationend", $$, !1);
         try {
-            Dv[a].unmount(), (r = document.getElementById(a)) == null || r.remove(), delete Dv[a], delete ti[a]
+            Dv[a].unmount(), (r = document.getElementById(a)) == null || r.remove(), delete Dv[a], delete ni[a]
         } catch {}
     }
     const Dv = lr({});
 
     function Qee(e, t) {
         const n = document.getElementById(String(t));
         n && (Dv[n.id] = e)
@@ -12673,17 +12674,17 @@
             };
             const a = r.appendPosition ? "".concat(r.exit, "--").concat(r.position) : r.exit;
             n.className += " ".concat(a), t && t(n)
         }
     }
 
     function tte(e) {
-        for (const t in ti)
+        for (const t in ni)
             if (t === e)
-                for (const n of ti[t] || []) x3(n)
+                for (const n of ni[t] || []) x3(n)
     }
 
     function nte(e) {
         const t = Wh().find(n => n.toastId === e);
         return t == null ? void 0 : t.containerId
     }
 
@@ -12708,21 +12709,21 @@
 
     function ite() {
         if (ml.items.length > 0) {
             const e = ml.items.shift();
             O0(e == null ? void 0 : e.toastContent, e == null ? void 0 : e.toastProps)
         }
     }
-    const ti = lr({}),
+    const ni = lr({}),
         ml = lr({
             items: []
         });
 
     function Wh() {
-        const e = It(ti);
+        const e = It(ni);
         return Object.values(e).reduce((t, n) => [...t, ...n], [])
     }
 
     function ste(e) {
         return Wh().find(t => t.toastId === e)
     }
 
@@ -12732,15 +12733,15 @@
             n && n.addEventListener("animationend", T$.bind(null, e, t), !1)
         } else T$(e, t)
     }
 
     function T$(e, t = {}) {
         const n = UT(t.containerId);
         n && n.removeEventListener("animationend", T$.bind(null, e, t), !1);
-        const r = ti[t.containerId] || [],
+        const r = ni[t.containerId] || [],
             a = r.length > 0;
         if (!a && !Kee(t.position)) {
             const i = Zee(t),
                 s = gB(Cte, t);
             s.mount(i), Qee(s, i.id)
         }
         a && !t.updateId && (t.position = r[0].position), Qt(() => {
@@ -12748,38 +12749,38 @@
         })
     }
     const _s = {
             add(e, t) {
                 const {
                     containerId: n = ""
                 } = t;
-                n && (ti[n] = ti[n] || [], ti[n].find(r => r.toastId === t.toastId) || setTimeout(() => {
+                n && (ni[n] = ni[n] || [], ni[n].find(r => r.toastId === t.toastId) || setTimeout(() => {
                     var r, a;
-                    t.newestOnTop ? (r = ti[n]) == null || r.unshift(t) : (a = ti[n]) == null || a.push(t), t.onOpen && t.onOpen(FL(t))
+                    t.newestOnTop ? (r = ni[n]) == null || r.unshift(t) : (a = ni[n]) == null || a.push(t), t.onOpen && t.onOpen(FL(t))
                 }, t.delay || 0))
             },
             remove(e) {
                 if (e) {
                     const t = nte(e);
                     if (t) {
-                        const n = ti[t];
+                        const n = ni[t];
                         let r = n.find(a => a.toastId === e);
-                        ti[t] = n.filter(a => a.toastId !== e), !ti[t].length && !ate(t) && C$(t, !1), ite(), Qt(() => {
+                        ni[t] = n.filter(a => a.toastId !== e), !ni[t].length && !ate(t) && C$(t, !1), ite(), Qt(() => {
                             r != null && r.onClose && (r.onClose(FL(r)), r = void 0)
                         })
                     }
                 }
             },
             update(e = {}) {
                 const {
                     containerId: t = ""
                 } = e;
                 if (t && e.updateId) {
-                    ti[t] = ti[t] || [];
-                    const n = ti[t].find(i => i.toastId === e.toastId),
+                    ni[t] = ni[t] || [];
+                    const n = ni[t].find(i => i.toastId === e.toastId),
                         r = (n == null ? void 0 : n.position) !== e.position || (n == null ? void 0 : n.transition) !== e.transition,
                         a = {
                             ...e,
                             disabledEnterTransition: !r,
                             updateId: void 0
                         };
                     _s.dismissForce(e == null ? void 0 : e.toastId), setTimeout(() => {
@@ -13432,15 +13433,15 @@
     }
     const Cte = Tt({
         name: "ToastifyContainer",
         inheritAttrs: !1,
         props: M3,
         setup(e) {
             const t = Y(() => e.containerId),
-                n = Y(() => ti[t.value] || []),
+                n = Y(() => ni[t.value] || []),
                 r = Y(() => n.value.filter(a => a.position === e.position));
             return zn(() => {
                 typeof window < "u" && e.clearOnUrlChange && window.requestAnimationFrame(D3)
             }), Io(() => {
                 typeof window < "u" && Zm && (window.cancelAnimationFrame(Zm), Pb.lastUrl = "")
             }), () => T(Ne, null, [r.value.map(a => {
                 const {
@@ -15034,27 +15035,27 @@
     wa.mergeConfig = Uh;
     wa.AxiosHeaders = Ys;
     wa.formToJSON = e => X3(Je.isHTMLForm(e) ? new FormData(e) : e);
     wa.getAdapter = Q3.getAdapter;
     wa.HttpStatusCode = D$;
     wa.default = wa;
     const yu = wa.create({
-        baseURL: li.backend_prefix,
+        baseURL: Ga.backend_prefix,
         timeout: null
     });
     yu.interceptors.request.use(e => {
         let t = N_();
         if (t != null) {
-            const n = li.auth_header_prefix || "Token";
+            const n = Ga.auth_header_prefix || "Token";
             e.headers.Authorization = `${n} ${t}`
         }
         return e.headers.Accept = "application/json", e
     }, e => (console.error("Config error: " + e), Promise.reject(e)));
     yu.interceptors.response.use(e => e, e => (e.response && e.response.status === 403 && FT(), Promise.reject(e)));
-    const zne = li.backend_prefix + "get_sections/";
+    const zne = Ga.backend_prefix + "get_sections/";
     async function Yne() {
         return await new Promise((e, t) => {
             if (!N_()) {
                 console.error("getApiInfo error: getToken is empty");
                 return
             }
             yu({
@@ -15115,15 +15116,15 @@
         if (!(e in t)) {
             console.error(`getMethods error: apiInfo does not contains viewname "${e}"`);
             return
         }
         let n = {};
         for (const [r, a] of Object.entries(t[e].routers))
             for (const [i, s] of Object.entries(a.mapping)) {
-                let o = li.backend_prefix + `${e}/`;
+                let o = Ga.backend_prefix + `${e}/`;
                 a.detail && (o = `${o}{id}/`), a.inline_type && (o = `${o}${s}/`);
                 const u = {
                     name: a.name,
                     detail: a.detail,
                     methodHttp: i,
                     url: o,
                     routeKey: r,
@@ -16411,15 +16412,15 @@
                         style: r.value
                     }, null), (i = n.additional) == null ? void 0 : i.call(n), n.default && T("div", {
                         class: ["v-responsive__content", e.contentClass]
                     }, [n.default()])])
                 }), {}
             }
         }),
-        Ga = qe({
+        Ka = qe({
             rounded: {
                 type: [Boolean, Number, String],
                 default: void 0
             },
             tile: Boolean
         }, "rounded");
 
@@ -16500,15 +16501,15 @@
             },
             crossorigin: String,
             referrerpolicy: String,
             srcset: String,
             position: String,
             ...mH(),
             ...Vt(),
-            ...Ga(),
+            ...Ka(),
             ...Vc()
         }, "VImg"),
         vp = at()({
             name: "VImg",
             directives: {
                 intersect: eP
             },
@@ -16778,15 +16779,15 @@
             start: Boolean,
             end: Boolean,
             icon: rn,
             image: String,
             text: String,
             ...Vt(),
             ...zi(),
-            ...Ga(),
+            ...Ka(),
             ...mp(),
             ...An(),
             ...br(),
             ...wl({
                 variant: "flat"
             })
         }, "VAvatar"),
@@ -17167,15 +17168,15 @@
             onClick: os(),
             onClickOnce: os(),
             ...bu(),
             ...Vt(),
             ...zi(),
             ...Lo(),
             ...Ks(),
-            ...Ga(),
+            ...Ka(),
             ...pg(),
             ...An(),
             ...br(),
             ...wl({
                 variant: "text"
             })
         }, "VListItem"),
@@ -17655,15 +17656,15 @@
             ...Lo(),
             ...Ks(),
             itemType: {
                 type: String,
                 default: "type"
             },
             ...EH(),
-            ...Ga(),
+            ...Ka(),
             ...An(),
             ...br(),
             ...wl({
                 variant: "text"
             })
         }, "VList"),
         bp = at()({
@@ -18103,15 +18104,15 @@
             ...Vt(),
             ...nP(),
             ...sg({
                 mobile: null
             }),
             ...Ks(),
             ...d3(),
-            ...Ga(),
+            ...Ka(),
             ...An({
                 tag: "nav"
             }),
             ...br()
         }, "VNavigationDrawer"),
         Hre = at()({
             name: "VNavigationDrawer",
@@ -18287,15 +18288,15 @@
                 }
             },
             created() {
                 this.navigation_info = nH(this.$router, this.apiInfo)
             },
             methods: {
                 getTitle() {
-                    return li.title
+                    return Ga.title
                 },
                 toggleDrawer() {
                     this.drawer = !this.drawer
                 }
             }
         },
         Ure = {
@@ -18347,15 +18348,15 @@
         AH = qe({
             baseColor: String,
             divided: Boolean,
             ...bu(),
             ...Vt(),
             ...zi(),
             ...Ks(),
-            ...Ga(),
+            ...Ka(),
             ...An(),
             ...br(),
             ...wl()
         }, "VBtnGroup"),
         rR = at()({
             name: "VBtnGroup",
             props: AH(),
@@ -18813,15 +18814,15 @@
             stream: Boolean,
             striped: Boolean,
             roundedBar: Boolean,
             ...Vt(),
             ...vg({
                 location: "top"
             }),
-            ...Ga(),
+            ...Ka(),
             ...An(),
             ...br()
         }, "VProgressLinear"),
         Zre = at()({
             name: "VProgressLinear",
             props: Jre(),
             emits: {
@@ -18863,16 +18864,16 @@
                     } = ui(e),
                     {
                         intersectionRef: S,
                         isIntersecting: k
                     } = IH(),
                     C = Y(() => parseFloat(e.max)),
                     x = Y(() => parseFloat(e.height)),
-                    E = Y(() => oi(parseFloat(e.bufferValue) / C.value * 100, 0, 100)),
-                    A = Y(() => oi(parseFloat(r.value) / C.value * 100, 0, 100)),
+                    E = Y(() => li(parseFloat(e.bufferValue) / C.value * 100, 0, 100)),
+                    A = Y(() => li(parseFloat(r.value) / C.value * 100, 0, 100)),
                     O = Y(() => a.value !== e.reverse),
                     R = Y(() => e.indeterminate ? "fade-transition" : "slide-x-transition");
 
                 function F(U) {
                     if (!S.value) return;
                     const {
                         left: G,
@@ -19041,15 +19042,15 @@
             ...zi(),
             ...Lo(),
             ...Ks(),
             ...X_(),
             ...Q_(),
             ...vg(),
             ...aP(),
-            ...Ga(),
+            ...Ka(),
             ...pg(),
             ...mp(),
             ...An({
                 tag: "button"
             }),
             ...br(),
             ...wl({
@@ -19386,15 +19387,15 @@
             ...Vt(),
             ...zi(),
             ...Lo(),
             ...Ks(),
             ...Q_(),
             ...vg(),
             ...aP(),
-            ...Ga(),
+            ...Ka(),
             ...pg(),
             ...An(),
             ...br(),
             ...wl({
                 variant: "elevated"
             })
         }, "VCard"),
@@ -19766,16 +19767,16 @@
             return Object.assign(n.value, {
                 "--v-overlay-anchor-origin": `${C.anchor.side} ${C.anchor.align}`,
                 transformOrigin: `${C.origin.side} ${C.origin.align}`,
                 top: Pt(RS(A)),
                 left: e.isRtl.value ? void 0 : Pt(RS(E)),
                 right: e.isRtl.value ? Pt(RS(-E)) : void 0,
                 minWidth: Pt(U === "y" ? Math.min(s.value, _.width) : s.value),
-                maxWidth: Pt(sR(oi(O.x, s.value === 1 / 0 ? 0 : s.value, u.value))),
-                maxHeight: Pt(sR(oi(O.y, o.value === 1 / 0 ? 0 : o.value, c.value)))
+                maxWidth: Pt(sR(li(O.x, s.value === 1 / 0 ? 0 : s.value, u.value))),
+                maxHeight: Pt(sR(li(O.y, o.value === 1 / 0 ? 0 : o.value, c.value)))
             }), {
                 available: O,
                 contentBox: y
             }
         }
         return st(() => [a.value, i.value, t.offset, t.minWidth, t.minHeight, t.maxWidth, t.maxHeight], () => g()), Qt(() => {
             const _ = g();
@@ -20818,15 +20819,15 @@
                 default: 64
             },
             image: String,
             title: String,
             ...bu(),
             ...Vt(),
             ...Ks(),
-            ...Ga(),
+            ...Ka(),
             ...An({
                 tag: "header"
             }),
             ...br()
         }, "VToolbar"),
         Fv = at()({
             name: "VToolbar",
@@ -20952,15 +20953,15 @@
         const a = Te(null),
             i = ht(0),
             s = ht(0),
             o = ht(0),
             u = ht(!1),
             c = ht(!1),
             f = Y(() => Number(e.scrollThreshold)),
-            h = Y(() => oi((f.value - i.value) / f.value || 0)),
+            h = Y(() => li((f.value - i.value) / f.value || 0)),
             p = () => {
                 const g = a.value;
                 !g || n && !n.value || (r = i.value, i.value = "window" in g ? g.pageYOffset : g.scrollTop, c.value = i.value < r, o.value = Math.abs(i.value - f.value))
             };
         return st(c, () => {
             s.value = s.value || i.value
         }), st(u, () => {
@@ -21197,15 +21198,15 @@
             icon: rn,
             items: {
                 type: Array,
                 default: () => []
             },
             ...Vt(),
             ...zi(),
-            ...Ga(),
+            ...Ka(),
             ...An({
                 tag: "ul"
             })
         }, "VBreadcrumbs"),
         qae = at()({
             name: "VBreadcrumbs",
             props: Yae(),
@@ -21837,15 +21838,15 @@
             }, 1024)]),
             _: 2
         }, 1032, ["prepend-icon"])]))), 128))])
     }
     const gie = xr(hie, [
             ["render", vie]
         ]),
-        yie = li.backend_prefix + "token-auth/";
+        yie = Ga.backend_prefix + "token-auth/";
 
     function bie(e) {
         var t = {
             username: e.username,
             password: e.password,
             phone: ""
         };
@@ -21853,15 +21854,15 @@
             url: yie,
             method: "post",
             data: t
         })
     }
 
     function _ie(e, t) {
-        return console.assert(li.backend_prefix, "backend url is not set!"), new Promise((n, r) => {
+        return console.assert(Ga.backend_prefix, "backend url is not set!"), new Promise((n, r) => {
             bie({
                 username: e.trim(),
                 password: t
             }).then(a => {
                 PZ(a.data.token, a.data.token), localStorage.setItem("name", a.data.username), localStorage.setItem("user_id", a.data.pk), n()
             }).catch(a => {
                 r(a)
@@ -22086,15 +22087,15 @@
                 validator: e => Tie.includes(e)
             },
             "onClick:clear": os(),
             "onClick:appendInner": os(),
             "onClick:prependInner": os(),
             ...Vt(),
             ...Q_(),
-            ...Ga(),
+            ...Ka(),
             ...br()
         }, "VField"),
         a1 = at()({
             name: "VField",
             inheritAttrs: !1,
             props: {
                 id: String,
@@ -22847,15 +22848,15 @@
                 async validate() {
                     const {
                         valid: e
                     } = await this.$refs.form.validate();
                     e && alert("Form is valid")
                 },
                 getTitle() {
-                    return li.title
+                    return Ga.title
                 },
                 login() {
                     this.loading = !0, _ie(this.username, this.password).then(() => {
                         this.$router.push("/"), this.loading = !1
                     }).catch(e => {
                         this.loading = !1;
                         let t = e.message;
@@ -23603,15 +23604,15 @@
                         const G = getComputedStyle(A.value),
                             B = getComputedStyle(g.value.$el),
                             W = parseFloat(G.getPropertyValue("--v-field-padding-top")) + parseFloat(G.getPropertyValue("--v-input-padding-top")) + parseFloat(G.getPropertyValue("--v-field-padding-bottom")),
                             ee = A.value.scrollHeight,
                             D = parseFloat(G.lineHeight),
                             Q = Math.max(parseFloat(e.rows) * D + W, parseFloat(B.getPropertyValue("--v-input-control-height"))),
                             se = parseFloat(e.maxRows) * D + W || 1 / 0,
-                            ue = oi(ee ?? 0, Q, se);
+                            ue = li(ee ?? 0, Q, se);
                         O.value = Math.floor((ue - W) / D), _.value = Pt(ue)
                     })
                 }
                 zn(F), st(i, F), st(() => e.rows, F), st(() => e.maxRows, F), st(() => e.density, F);
                 let U;
                 return st(A, G => {
                     G ? (U = new ResizeObserver(F), U.observe(A.value)) : U == null || U.disconnect()
@@ -23829,15 +23830,15 @@
                 } = t;
                 const i = Gt(e, "modelValue"),
                     s = Y(() => bb(e.step)),
                     o = Y(() => i.value != null ? bb(i.value) : 0),
                     u = Y(() => i.value == null ? !0 : i.value + e.step <= e.max),
                     c = Y(() => i.value == null ? !0 : i.value - e.step >= e.min);
                 ra(() => {
-                    i.value != null && (i.value < e.min || i.value > e.max) && (i.value = oi(i.value, e.min, e.max))
+                    i.value != null && (i.value < e.min || i.value > e.max) && (i.value = li(i.value, e.min, e.max))
                 });
                 const f = Y(() => e.hideInput ? "stacked" : e.controlVariant),
                     h = Y(() => ({
                         click: _
                     })),
                     p = Y(() => ({
                         click: y
@@ -24594,15 +24595,15 @@
             onClick: os(),
             onClickOnce: os(),
             ...bu(),
             ...Vt(),
             ...zi(),
             ...Ks(),
             ...X_(),
-            ...Ga(),
+            ...Ka(),
             ...pg(),
             ...mp(),
             ...An({
                 tag: "span"
             }),
             ...br(),
             ...wl({
@@ -25012,15 +25013,15 @@
         function A(he, X) {
             const N = y[he],
                 q = r.value;
             r.value = q ? Math.min(r.value, X) : X, (N !== X || q !== r.value) && (y[he] = X, x())
         }
 
         function O(he) {
-            return he = oi(he, 0, t.value.length - 1), w[he] || 0
+            return he = li(he, 0, t.value.length - 1), w[he] || 0
         }
 
         function R(he) {
             return pse(w, he)
         }
         let F = 0,
             U = 0,
@@ -25048,17 +25049,17 @@
         }
 
         function Q() {
             if (!u.value || !g.value) return;
             const he = F - f,
                 X = Math.sign(U),
                 N = Math.max(0, he - VS),
-                q = oi(R(N), 0, t.value.length),
+                q = li(R(N), 0, t.value.length),
                 M = he + g.value + VS,
-                P = oi(R(M) + 1, q + 1, t.value.length);
+                P = li(R(M) + 1, q + 1, t.value.length);
             if ((X !== cse || q < a.value) && (X !== dse || P > i.value)) {
                 const L = O(a.value) - O(q),
                     H = O(P) - O(i.value);
                 Math.max(L, H) > VS ? (a.value = q, i.value = P) : (q <= 0 && (a.value = q), P >= t.value.length && (i.value = P))
             }
             s.value = O(a.value), o.value = O(t.value.length) - O(i.value)
         }
@@ -25975,15 +25976,15 @@
                     }
                 }
             }
         },
         Ese = ["advlist anchor autolink autosave code codesample colorpicker colorpicker contextmenu directionality emoticons fullscreen hr image imagetools insertdatetime link lists media nonbreaking noneditable pagebreak paste preview print save searchreplace spellchecker tabfocus table template textcolor textpattern visualblocks visualchars wordcount accordion"],
         xse = ["searchreplace undo redo | bold italic underline strikethrough blockquote removeformat | alignleft aligncenter alignright outdent indent | subscript superscript code codesample", "hr bullist numlist link image charmap anchor pagebreak insertdatetime media table emoticons forecolor backcolor add-accordion | preview fullscreen"],
         Ose = "file edit insert view format table",
-        Ase = `${li.static_prefix}/tinymce/tinymce.min.js`,
+        Ase = `${Ga.static_prefix}/tinymce/tinymce.min.js`,
         Mse = {
             name: "TinyMCE",
             props: {
                 ...Cl
             },
             data(e) {
                 return {
@@ -26003,15 +26004,19 @@
                     const e = this.width;
                     return /^[\d]+(\.[\d]+)?$/.test(e) ? `${e}px` : e
                 }
             },
             mounted() {
                 Tl(this), Pse(Ase, e => {
                     if (e) {
-                        this.$message.error(e.message);
+                        console.error(e.message), tn(e.message, {
+                            theme: "auto",
+                            type: "error",
+                            position: "top-center"
+                        });
                         return
                     }
                     this.initTinymce()
                 })
             },
             activated() {
                 window.tinymce && this.initTinymce()
@@ -26028,17 +26033,17 @@
                     this.initTinymce()
                 },
                 initTinymce() {
                     const e = this;
                     window.tinymce.init({
                         theme: this.theme,
                         skin: this.skin,
-                        skin_url: `${li.static_prefix}/tinymce/${this.skin}`,
+                        skin_url: `${Ga.static_prefix}/tinymce/${this.skin}`,
                         external_plugins: {
-                            accordion: `${li.static_prefix}/tinymce/plugins/accordion/plugin.js`
+                            accordion: `${Ga.static_prefix}/tinymce/plugins/accordion/plugin.js`
                         },
                         plugin_preview_width: "1200",
                         plugin_preview_height: "800",
                         selector: `#${this.tinymceId}`,
                         language: "en",
                         height: this.height,
                         body_class: "panel-body",
@@ -31773,15 +31778,15 @@
         compositeRule: r,
         createErrors: a,
         allErrors: i
     }) {
         r !== void 0 && (e.compositeRule = r), a !== void 0 && (e.createErrors = a), i !== void 0 && (e.allErrors = i), e.jtdDiscriminator = t, e.jtdMetadata = n
     }
     mc.extendSubschemaMode = kPe;
-    var ni = {},
+    var ri = {},
         S1 = function e(t, n) {
             if (t === n) return !0;
             if (t && n && typeof t == "object" && typeof n == "object") {
                 if (t.constructor !== n.constructor) return !1;
                 var r, a, i;
                 if (Array.isArray(t)) {
                     if (r = t.length, r != n.length) return !1;
@@ -31874,27 +31879,27 @@
         }
     }
 
     function $Pe(e) {
         return e.replace(/~/g, "~0").replace(/\//g, "~1")
     }
     var CPe = u5.exports;
-    Object.defineProperty(ni, "__esModule", {
+    Object.defineProperty(ri, "__esModule", {
         value: !0
     });
-    ni.getSchemaRefs = ni.resolveUrl = ni.normalizeId = ni._getFullPath = ni.getFullPath = ni.inlineRef = void 0;
+    ri.getSchemaRefs = ri.resolveUrl = ri.normalizeId = ri._getFullPath = ri.getFullPath = ri.inlineRef = void 0;
     const TPe = $t,
         PPe = S1,
         EPe = CPe,
         xPe = new Set(["type", "format", "pattern", "maxLength", "minLength", "maxProperties", "minProperties", "maxItems", "minItems", "maximum", "minimum", "uniqueItems", "multipleOf", "required", "enum", "const"]);
 
     function OPe(e, t = !0) {
         return typeof e == "boolean" ? !0 : t === !0 ? !eC(e) : t ? c5(e) <= t : !1
     }
-    ni.inlineRef = OPe;
+    ri.inlineRef = OPe;
     const APe = new Set(["$ref", "$recursiveRef", "$recursiveAnchor", "$dynamicRef", "$dynamicAnchor"]);
 
     function eC(e) {
         for (const t in e) {
             if (APe.has(t)) return !0;
             const n = e[t];
             if (Array.isArray(n) && n.some(eC) || typeof n == "object" && eC(n)) return !0
@@ -31912,31 +31917,31 @@
     }
 
     function d5(e, t = "", n) {
         n !== !1 && (t = $h(t));
         const r = e.parse(t);
         return f5(e, r)
     }
-    ni.getFullPath = d5;
+    ri.getFullPath = d5;
 
     function f5(e, t) {
         return e.serialize(t).split("#")[0] + "#"
     }
-    ni._getFullPath = f5;
+    ri._getFullPath = f5;
     const MPe = /#\/?$/;
 
     function $h(e) {
         return e ? e.replace(MPe, "") : ""
     }
-    ni.normalizeId = $h;
+    ri.normalizeId = $h;
 
     function DPe(e, t, n) {
         return n = $h(n), e.resolve(t, n)
     }
-    ni.resolveUrl = DPe;
+    ri.resolveUrl = DPe;
     const IPe = /^[a-z_][-a-z0-9._]*$/i;
 
     function LPe(e, t) {
         if (typeof e == "boolean") return {};
         const {
             schemaId: n,
             uriResolver: r
@@ -31971,29 +31976,29 @@
             if (p !== void 0 && !PPe(h, p)) throw f(g)
         }
 
         function f(h) {
             return new Error(`reference "${h}" resolves to more than one schema`)
         }
     }
-    ni.getSchemaRefs = LPe;
+    ri.getSchemaRefs = LPe;
     Object.defineProperty(So, "__esModule", {
         value: !0
     });
     So.getData = So.KeywordCxt = So.validateFunctionCode = void 0;
     const h5 = qh,
         BN = Aa,
         nE = ru,
         Fb = Aa,
         RPe = w1,
         Qm = ll,
         QS = mc,
         Rt = yn,
         Xt = El,
-        NPe = ni,
+        NPe = ri,
         au = $t,
         Sm = Og;
 
     function FPe(e) {
         if (v5(e) && (g5(e), m5(e))) {
             BPe(e);
             return
@@ -32419,30 +32424,30 @@
         }
     };
     Ag.default = iEe;
     var Mg = {};
     Object.defineProperty(Mg, "__esModule", {
         value: !0
     });
-    const ek = ni;
+    const ek = ri;
     let sEe = class extends Error {
         constructor(t, n, r, a) {
             super(a || `can't resolve reference ${r} from id ${n}`), this.missingRef = (0, ek.resolveUrl)(t, n, r), this.missingSchema = (0, ek.normalizeId)((0, ek.getFullPath)(t, this.missingRef))
         }
     };
     Mg.default = sEe;
     var ns = {};
     Object.defineProperty(ns, "__esModule", {
         value: !0
     });
     ns.resolveSchema = ns.getCompilingSchema = ns.resolveRef = ns.compileSchema = ns.SchemaEnv = void 0;
     const io = yn,
         oEe = Ag,
         pd = El,
-        ho = ni,
+        ho = ri,
         zN = $t,
         lEe = So;
     let k1 = class {
         constructor(t) {
             var n;
             this.refs = {}, this.dynamicAnchors = {};
             let r;
@@ -32718,20 +32723,20 @@
                     er = a(pn + "\\." + pn + "\\." + pn + "\\." + pn),
                     Wt = a(We + "{1,4}"),
                     Bn = a(a(Wt + "\\:" + Wt) + "|" + er),
                     tr = a(a(Wt + "\\:") + "{6}" + Bn),
                     Hn = a("\\:\\:" + a(Wt + "\\:") + "{5}" + Bn),
                     $a = a(a(Wt) + "?\\:\\:" + a(Wt + "\\:") + "{4}" + Bn),
                     ci = a(a(a(Wt + "\\:") + "{0,1}" + Wt) + "?\\:\\:" + a(Wt + "\\:") + "{3}" + Bn),
-                    Xa = a(a(a(Wt + "\\:") + "{0,2}" + Wt) + "?\\:\\:" + a(Wt + "\\:") + "{2}" + Bn),
+                    Ja = a(a(a(Wt + "\\:") + "{0,2}" + Wt) + "?\\:\\:" + a(Wt + "\\:") + "{2}" + Bn),
                     qn = a(a(a(Wt + "\\:") + "{0,3}" + Wt) + "?\\:\\:" + Wt + "\\:" + Bn),
                     St = a(a(a(Wt + "\\:") + "{0,4}" + Wt) + "?\\:\\:" + Bn),
                     Xr = a(a(a(Wt + "\\:") + "{0,5}" + Wt) + "?\\:\\:" + Wt),
                     di = a(a(a(Wt + "\\:") + "{0,6}" + Wt) + "?\\:\\:"),
-                    oa = a([tr, Hn, $a, ci, Xa, qn, St, Xr, di].join("|")),
+                    oa = a([tr, Hn, $a, ci, Ja, qn, St, Xr, di].join("|")),
                     te = a(a(Yt + "|" + je) + "+");
                 a("[vV]" + We + "+\\." + r(Yt, Lt, "[\\:]") + "+"), a(a(je + "|" + r(Yt, Lt)) + "*");
                 var be = a(je + "|" + r(Yt, Lt, "[\\:\\@]"));
                 return a(a(je + "|" + r(Yt, Lt, "[\\@]")) + "+"), a(a(be + "|" + r("[\\/\\?]", sr)) + "*"), {
                     NOT_SCHEME: new RegExp(r("[^]", ge, Ce, "[\\+\\-\\.]"), "g"),
                     NOT_USERINFO: new RegExp(r("[^\\%\\:]", Yt, Lt), "g"),
                     NOT_HOST: new RegExp(r("[^\\%\\[\\]\\:]", Yt, Lt), "g"),
@@ -32895,23 +32900,23 @@
                         Bn = Wt;
                     for (Wt && Ce.push(A); Bn < We;) {
                         var tr = _,
                             Hn = !0,
                             $a = !1,
                             ci = void 0;
                         try {
-                            for (var Xa = ge[Symbol.iterator](), qn; !(Hn = (qn = Xa.next()).done); Hn = !0) {
+                            for (var Ja = ge[Symbol.iterator](), qn; !(Hn = (qn = Ja.next()).done); Hn = !0) {
                                 var St = qn.value;
                                 St >= je && St < tr && (tr = St)
                             }
                         } catch (Ds) {
                             $a = !0, ci = Ds
                         } finally {
                             try {
-                                !Hn && Xa.return && Xa.return()
+                                !Hn && Ja.return && Ja.return()
                             } finally {
                                 if ($a) throw ci
                             }
                         }
                         var Xr = Bn + 1;
                         tr - je > B((_ - Ot) / Xr) && ee("overflow"), Ot += (tr - je) * Xr, je = tr;
                         var di = !0,
@@ -33030,21 +33035,21 @@
                                 })
                             }
                             return Xr
                         }, []),
                         ci = $a.sort(function(Xr, di) {
                             return di.length - Xr.length
                         })[0],
-                        Xa = void 0;
+                        Ja = void 0;
                     if (ci && ci.length > 1) {
                         var qn = tr.slice(0, ci.index),
                             St = tr.slice(ci.index + ci.length);
-                        Xa = qn.join(":") + "::" + St.join(":")
-                    } else Xa = tr.join(":");
-                    return Ot && (Xa += "%" + Ot), Xa
+                        Ja = qn.join(":") + "::" + St.join(":")
+                    } else Ja = tr.join(":");
+                    return Ot && (Ja += "%" + Ot), Ja
                 } else return $e
             }
             var J = /^(?:([^:\/?#]+):)?(?:\/\/((?:([^\/?#@]*)@)?(\[[^\/?#\]]+\]|[^\/?#:]*)(?:\:(\d*))?))?([^?#]*)(?:\?([^#]*))?(?:#((?:.|\n|\r)*))?/i,
                 oe = "".match(/(){0}/)[1] === void 0;
 
             function le($e) {
                 var ge = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : {},
@@ -33187,15 +33192,15 @@
                 },
                 sa = {
                     scheme: "wss",
                     domainHost: Nr.domainHost,
                     parse: Nr.parse,
                     serialize: Nr.serialize
                 },
-                Ka = {},
+                Xa = {},
                 Ie = "[A-Za-z0-9\\-\\.\\_\\~\\xA0-\\u200D\\u2010-\\u2029\\u202F-\\uD7FF\\uF900-\\uFDCF\\uFDF0-\\uFFEF]",
                 Se = "[0-9A-Fa-f]",
                 Qe = a(a("%[EFef]" + Se + "%" + Se + Se + "%" + Se + Se) + "|" + a("%[89A-Fa-f]" + Se + "%" + Se + Se) + "|" + a("%" + Se + Se)),
                 Ue = "[A-Za-z0-9\\!\\$\\%\\'\\*\\+\\-\\^\\_\\`\\{\\|\\}\\~]",
                 an = "[\\!\\$\\%\\'\\(\\)\\*\\+\\,\\-\\.0-9\\<\\>A-Z\\x5E-\\x7E]",
                 bn = r(an, '[\\"\\\\]'),
                 Pn = "[\\!\\$\\'\\(\\)\\*\\+\\,\\;\\:\\@]",
@@ -33264,15 +33269,15 @@
                                 je[Ot] = sr + "@" + Yt
                             }
                             We.path = je.join(",")
                         }
                         var pn = ge.headers = ge.headers || {};
                         ge.subject && (pn.subject = ge.subject), ge.body && (pn.body = ge.body);
                         var er = [];
-                        for (var Wt in pn) pn[Wt] !== Ka[Wt] && er.push(Wt.replace(Mr, Ms).replace(Mr, s).replace(Fr, ae) + "=" + pn[Wt].replace(Mr, Ms).replace(Mr, s).replace(Vr, ae));
+                        for (var Wt in pn) pn[Wt] !== Xa[Wt] && er.push(Wt.replace(Mr, Ms).replace(Mr, s).replace(Fr, ae) + "=" + pn[Wt].replace(Mr, Ms).replace(Mr, s).replace(Vr, ae));
                         return er.length && (We.query = er.join("&")), We
                     }
                 },
                 Bo = /^([^\:]+)\:(.*)/,
                 Cu = {
                     scheme: "urn",
                     parse: function(ge, Ce) {
@@ -33367,15 +33372,15 @@
             }
         });
         const r = Ag,
             a = Mg,
             i = tf,
             s = ns,
             o = yn,
-            u = ni,
+            u = ri,
             c = Aa,
             f = $t,
             h = _Ee,
             p = iE,
             g = (X, N) => new RegExp(X, N);
         g.code = "new RegExp";
         const _ = ["removeAdditional", "useDefaults", "coerceTypes"],
@@ -34298,30 +34303,30 @@
     const x5 = S1;
     x5.code = 'require("ajv/dist/runtime/equal").default';
     Dg.default = x5;
     Object.defineProperty(yE, "__esModule", {
         value: !0
     });
     const nk = Aa,
-        Qa = yn,
+        ei = yn,
         zEe = $t,
         YEe = Dg,
         qEe = {
             message: ({
                 params: {
                     i: e,
                     j: t
                 }
-            }) => (0, Qa.str)`must NOT have duplicate items (items ## ${t} and ${e} are identical)`,
+            }) => (0, ei.str)`must NOT have duplicate items (items ## ${t} and ${e} are identical)`,
             params: ({
                 params: {
                     i: e,
                     j: t
                 }
-            }) => (0, Qa._)`{i: ${e}, j: ${t}}`
+            }) => (0, ei._)`{i: ${e}, j: ${t}}`
         },
         GEe = {
             keyword: "uniqueItems",
             type: "array",
             schemaType: "boolean",
             $data: !0,
             error: qEe,
@@ -34334,44 +34339,44 @@
                     parentSchema: i,
                     schemaCode: s,
                     it: o
                 } = e;
                 if (!r && !a) return;
                 const u = t.let("valid"),
                     c = i.items ? (0, nk.getSchemaTypes)(i.items) : [];
-                e.block$data(u, f, (0, Qa._)`${s} === false`), e.ok(u);
+                e.block$data(u, f, (0, ei._)`${s} === false`), e.ok(u);
 
                 function f() {
-                    const _ = t.let("i", (0, Qa._)`${n}.length`),
+                    const _ = t.let("i", (0, ei._)`${n}.length`),
                         y = t.let("j");
                     e.setParams({
                         i: _,
                         j: y
-                    }), t.assign(u, !0), t.if((0, Qa._)`${_} > 1`, () => (h() ? p : g)(_, y))
+                    }), t.assign(u, !0), t.if((0, ei._)`${_} > 1`, () => (h() ? p : g)(_, y))
                 }
 
                 function h() {
                     return c.length > 0 && !c.some(_ => _ === "object" || _ === "array")
                 }
 
                 function p(_, y) {
                     const w = t.name("item"),
                         S = (0, nk.checkDataTypes)(c, w, o.opts.strictNumbers, nk.DataType.Wrong),
-                        k = t.const("indices", (0, Qa._)`{}`);
-                    t.for((0, Qa._)`;${_}--;`, () => {
-                        t.let(w, (0, Qa._)`${n}[${_}]`), t.if(S, (0, Qa._)`continue`), c.length > 1 && t.if((0, Qa._)`typeof ${w} == "string"`, (0, Qa._)`${w} += "_"`), t.if((0, Qa._)`typeof ${k}[${w}] == "number"`, () => {
-                            t.assign(y, (0, Qa._)`${k}[${w}]`), e.error(), t.assign(u, !1).break()
-                        }).code((0, Qa._)`${k}[${w}] = ${_}`)
+                        k = t.const("indices", (0, ei._)`{}`);
+                    t.for((0, ei._)`;${_}--;`, () => {
+                        t.let(w, (0, ei._)`${n}[${_}]`), t.if(S, (0, ei._)`continue`), c.length > 1 && t.if((0, ei._)`typeof ${w} == "string"`, (0, ei._)`${w} += "_"`), t.if((0, ei._)`typeof ${k}[${w}] == "number"`, () => {
+                            t.assign(y, (0, ei._)`${k}[${w}]`), e.error(), t.assign(u, !1).break()
+                        }).code((0, ei._)`${k}[${w}] = ${_}`)
                     })
                 }
 
                 function g(_, y) {
                     const w = (0, zEe.useFunc)(t, YEe.default),
                         S = t.name("outer");
-                    t.label(S).for((0, Qa._)`;${_}--;`, () => t.for((0, Qa._)`${y} = ${_}; ${y}--;`, () => t.if((0, Qa._)`${w}(${n}[${_}], ${n}[${y}])`, () => {
+                    t.label(S).for((0, ei._)`;${_}--;`, () => t.for((0, ei._)`${y} = ${_}; ${y}--;`, () => t.if((0, ei._)`${w}(${n}[${_}], ${n}[${y}])`, () => {
                         e.error(), t.assign(u, !1).break(S)
                     })))
                 }
             }
         };
     yE.default = GEe;
     var bE = {};
@@ -37876,15 +37881,15 @@
         compositeRule: r,
         createErrors: a,
         allErrors: i
     }) {
         r !== void 0 && (e.compositeRule = r), a !== void 0 && (e.createErrors = a), i !== void 0 && (e.allErrors = i), e.jtdDiscriminator = t, e.jtdMetadata = n
     }
     vc.extendSubschemaMode = IAe;
-    var ri = {},
+    var ai = {},
         Q5 = {
             exports: {}
         },
         nc = Q5.exports = function(e, t, n) {
             typeof t == "function" && (n = t, t = {}), n = t.cb || n;
             var r = typeof n == "function" ? n : n.pre || function() {},
                 a = n.post || function() {};
@@ -37952,27 +37957,27 @@
         }
     }
 
     function LAe(e) {
         return e.replace(/~/g, "~0").replace(/\//g, "~1")
     }
     var RAe = Q5.exports;
-    Object.defineProperty(ri, "__esModule", {
+    Object.defineProperty(ai, "__esModule", {
         value: !0
     });
-    ri.getSchemaRefs = ri.resolveUrl = ri.normalizeId = ri._getFullPath = ri.getFullPath = ri.inlineRef = void 0;
+    ai.getSchemaRefs = ai.resolveUrl = ai.normalizeId = ai._getFullPath = ai.getFullPath = ai.inlineRef = void 0;
     const NAe = Ct,
         FAe = S1,
         VAe = RAe,
         jAe = new Set(["type", "format", "pattern", "maxLength", "minLength", "maxProperties", "minProperties", "maxItems", "minItems", "maximum", "minimum", "uniqueItems", "multipleOf", "required", "enum", "const"]);
 
     function BAe(e, t = !0) {
         return typeof e == "boolean" ? !0 : t === !0 ? !cC(e) : t ? ez(e) <= t : !1
     }
-    ri.inlineRef = BAe;
+    ai.inlineRef = BAe;
     const HAe = new Set(["$ref", "$recursiveRef", "$recursiveAnchor", "$dynamicRef", "$dynamicAnchor"]);
 
     function cC(e) {
         for (const t in e) {
             if (HAe.has(t)) return !0;
             const n = e[t];
             if (Array.isArray(n) && n.some(cC) || typeof n == "object" && cC(n)) return !0
@@ -37990,31 +37995,31 @@
     }
 
     function tz(e, t = "", n) {
         n !== !1 && (t = Th(t));
         const r = e.parse(t);
         return nz(e, r)
     }
-    ri.getFullPath = tz;
+    ai.getFullPath = tz;
 
     function nz(e, t) {
         return e.serialize(t).split("#")[0] + "#"
     }
-    ri._getFullPath = nz;
+    ai._getFullPath = nz;
     const WAe = /#\/?$/;
 
     function Th(e) {
         return e ? e.replace(WAe, "") : ""
     }
-    ri.normalizeId = Th;
+    ai.normalizeId = Th;
 
     function UAe(e, t, n) {
         return n = Th(n), e.resolve(t, n)
     }
-    ri.resolveUrl = UAe;
+    ai.resolveUrl = UAe;
     const zAe = /^[a-z_][-a-z0-9._]*$/i;
 
     function YAe(e, t) {
         if (typeof e == "boolean") return {};
         const {
             schemaId: n,
             uriResolver: r
@@ -38049,29 +38054,29 @@
             if (p !== void 0 && !FAe(h, p)) throw f(g)
         }
 
         function f(h) {
             return new Error(`reference "${h}" resolves to more than one schema`)
         }
     }
-    ri.getSchemaRefs = YAe;
+    ai.getSchemaRefs = YAe;
     Object.defineProperty(ko, "__esModule", {
         value: !0
     });
     ko.getData = ko.KeywordCxt = ko.validateFunctionCode = void 0;
     const rz = Kh,
         u2 = Ma,
         UE = iu,
         Wb = Ma,
         qAe = P1,
         av = ul,
         ak = vc,
         Nt = hn,
         Jt = xl,
-        GAe = ri,
+        GAe = ai,
         su = Ct,
         $m = Ig;
 
     function KAe(e) {
         if (sz(e) && (oz(e), iz(e))) {
             ZAe(e);
             return
@@ -38497,30 +38502,30 @@
         }
     }
     Lg.default = vMe;
     var Rg = {};
     Object.defineProperty(Rg, "__esModule", {
         value: !0
     });
-    const ik = ri;
+    const ik = ai;
     class gMe extends Error {
         constructor(t, n, r, a) {
             super(a || `can't resolve reference ${r} from id ${n}`), this.missingRef = (0, ik.resolveUrl)(t, n, r), this.missingSchema = (0, ik.normalizeId)((0, ik.getFullPath)(t, this.missingRef))
         }
     }
     Rg.default = gMe;
     var rs = {};
     Object.defineProperty(rs, "__esModule", {
         value: !0
     });
     rs.resolveSchema = rs.getCompilingSchema = rs.resolveRef = rs.compileSchema = rs.SchemaEnv = void 0;
     const so = hn,
         yMe = Lg,
         md = xl,
-        po = ri,
+        po = ai,
         h2 = Ct,
         bMe = ko;
     class E1 {
         constructor(t) {
             var n;
             this.refs = {}, this.dynamicAnchors = {};
             let r;
@@ -38791,15 +38796,15 @@
             }
         });
         const r = Lg,
             a = Rg,
             i = rf,
             s = rs,
             o = hn,
-            u = ri,
+            u = ai,
             c = Ma,
             f = Ct,
             h = AMe,
             p = qE,
             g = (X, N) => new RegExp(X, N);
         g.code = "new RegExp";
         const _ = ["removeAdditional", "useDefaults", "coerceTypes"],
@@ -39722,30 +39727,30 @@
     const yz = S1;
     yz.code = 'require("ajv/dist/runtime/equal").default';
     Ng.default = yz;
     Object.defineProperty(sx, "__esModule", {
         value: !0
     });
     const ok = Ma,
-        ei = hn,
+        ti = hn,
         nDe = Ct,
         rDe = Ng,
         aDe = {
             message: ({
                 params: {
                     i: e,
                     j: t
                 }
-            }) => (0, ei.str)`must NOT have duplicate items (items ## ${t} and ${e} are identical)`,
+            }) => (0, ti.str)`must NOT have duplicate items (items ## ${t} and ${e} are identical)`,
             params: ({
                 params: {
                     i: e,
                     j: t
                 }
-            }) => (0, ei._)`{i: ${e}, j: ${t}}`
+            }) => (0, ti._)`{i: ${e}, j: ${t}}`
         },
         iDe = {
             keyword: "uniqueItems",
             type: "array",
             schemaType: "boolean",
             $data: !0,
             error: aDe,
@@ -39758,44 +39763,44 @@
                     parentSchema: i,
                     schemaCode: s,
                     it: o
                 } = e;
                 if (!r && !a) return;
                 const u = t.let("valid"),
                     c = i.items ? (0, ok.getSchemaTypes)(i.items) : [];
-                e.block$data(u, f, (0, ei._)`${s} === false`), e.ok(u);
+                e.block$data(u, f, (0, ti._)`${s} === false`), e.ok(u);
 
                 function f() {
-                    const _ = t.let("i", (0, ei._)`${n}.length`),
+                    const _ = t.let("i", (0, ti._)`${n}.length`),
                         y = t.let("j");
                     e.setParams({
                         i: _,
                         j: y
-                    }), t.assign(u, !0), t.if((0, ei._)`${_} > 1`, () => (h() ? p : g)(_, y))
+                    }), t.assign(u, !0), t.if((0, ti._)`${_} > 1`, () => (h() ? p : g)(_, y))
                 }
 
                 function h() {
                     return c.length > 0 && !c.some(_ => _ === "object" || _ === "array")
                 }
 
                 function p(_, y) {
                     const w = t.name("item"),
                         S = (0, ok.checkDataTypes)(c, w, o.opts.strictNumbers, ok.DataType.Wrong),
-                        k = t.const("indices", (0, ei._)`{}`);
-                    t.for((0, ei._)`;${_}--;`, () => {
-                        t.let(w, (0, ei._)`${n}[${_}]`), t.if(S, (0, ei._)`continue`), c.length > 1 && t.if((0, ei._)`typeof ${w} == "string"`, (0, ei._)`${w} += "_"`), t.if((0, ei._)`typeof ${k}[${w}] == "number"`, () => {
-                            t.assign(y, (0, ei._)`${k}[${w}]`), e.error(), t.assign(u, !1).break()
-                        }).code((0, ei._)`${k}[${w}] = ${_}`)
+                        k = t.const("indices", (0, ti._)`{}`);
+                    t.for((0, ti._)`;${_}--;`, () => {
+                        t.let(w, (0, ti._)`${n}[${_}]`), t.if(S, (0, ti._)`continue`), c.length > 1 && t.if((0, ti._)`typeof ${w} == "string"`, (0, ti._)`${w} += "_"`), t.if((0, ti._)`typeof ${k}[${w}] == "number"`, () => {
+                            t.assign(y, (0, ti._)`${k}[${w}]`), e.error(), t.assign(u, !1).break()
+                        }).code((0, ti._)`${k}[${w}] = ${_}`)
                     })
                 }
 
                 function g(_, y) {
                     const w = (0, nDe.useFunc)(t, rDe.default),
                         S = t.name("outer");
-                    t.label(S).for((0, ei._)`;${_}--;`, () => t.for((0, ei._)`${y} = ${_}; ${y}--;`, () => t.if((0, ei._)`${w}(${n}[${_}], ${n}[${y}])`, () => {
+                    t.label(S).for((0, ti._)`;${_}--;`, () => t.for((0, ti._)`${y} = ${_}; ${y}--;`, () => t.if((0, ti._)`${w}(${n}[${_}], ${n}[${y}])`, () => {
                         e.error(), t.assign(u, !1).break(S)
                     })))
                 }
             }
         };
     sx.default = iDe;
     var ox = {};
@@ -43126,15 +43131,15 @@
             },
             ...Vt(),
             ...zi(),
             ...Lo(),
             ...Ks(),
             ...vg(),
             ...aP(),
-            ...Ga(),
+            ...Ka(),
             ...An(),
             ...br(),
             ...wl({
                 variant: "flat"
             })
         }, "VAlert"),
         i4 = at()({
@@ -43744,15 +43749,15 @@
             offsetX: [Number, String],
             offsetY: [Number, String],
             textColor: String,
             ...Vt(),
             ...vg({
                 location: "top end"
             }),
-            ...Ga(),
+            ...Ka(),
             ...An(),
             ...br(),
             ...Vc({
                 transition: "scale-rotate-transition"
             })
         }, "VBadge"),
         yNe = at()({
@@ -44213,15 +44218,15 @@
             },
             direction: {
                 type: String,
                 default: "horizontal",
                 validator: e => ["vertical", "horizontal"].includes(e)
             },
             reverse: Boolean,
-            ...Ga(),
+            ...Ka(),
             ...Ks({
                 elevation: 2
             }),
             ripple: {
                 type: Boolean,
                 default: !0
             }
@@ -44230,15 +44235,15 @@
             const t = Y(() => parseFloat(e.min)),
                 n = Y(() => parseFloat(e.max)),
                 r = Y(() => +e.step > 0 ? parseFloat(e.step) : 0),
                 a = Y(() => Math.max(bb(r.value), bb(t.value)));
 
             function i(s) {
                 if (s = parseFloat(s), r.value <= 0) return s;
-                const o = oi(s, t.value, n.value),
+                const o = li(s, t.value, n.value),
                     u = t.value % r.value,
                     c = Math.round((o - u) / r.value) * r.value + u;
                 return parseFloat(Math.min(c, n.value).toFixed(a.value))
             }
             return {
                 min: t,
                 max: n,
@@ -44322,15 +44327,15 @@
             function X(H) {
                 H.preventDefault(), ee(H), window.addEventListener("mousemove", Q, D), window.addEventListener("mouseup", se, {
                     passive: !1
                 })
             }
             const N = H => {
                     const V = (H - h.value) / (p.value - h.value) * 100;
-                    return oi(isNaN(V) ? 0 : V, 0, 100)
+                    return li(isNaN(V) ? 0 : V, 0, 100)
                 },
                 q = Ze(t, "showTicks"),
                 M = Y(() => q.value ? t.ticks ? Array.isArray(t.ticks) ? t.ticks.map(H => ({
                     value: H,
                     position: N(H),
                     label: H.toString()
                 })) : Object.keys(t.ticks).map(H => ({
@@ -45383,23 +45388,23 @@
         });
 
         function o(p) {
             n.value = p, t.value = 1
         }
 
         function u() {
-            t.value = oi(t.value + 1, 1, s.value)
+            t.value = li(t.value + 1, 1, s.value)
         }
 
         function c() {
-            t.value = oi(t.value - 1, 1, s.value)
+            t.value = li(t.value - 1, 1, s.value)
         }
 
         function f(p) {
-            t.value = oi(p, 1, s.value)
+            t.value = li(p, 1, s.value)
         }
         const h = {
             page: t,
             itemsPerPage: n,
             startIndex: a,
             stopIndex: i,
             pageCount: s,
@@ -45802,15 +45807,15 @@
                 default: "..."
             },
             showFirstLastPage: Boolean,
             ...bu(),
             ...Vt(),
             ...zi(),
             ...Ks(),
-            ...Ga(),
+            ...Ka(),
             ...mp(),
             ...An({
                 tag: "nav"
             }),
             ...br(),
             ...wl({
                 variant: "text"
@@ -47267,15 +47272,15 @@
         }),
         L4 = qe({
             title: String,
             text: String,
             bgColor: String,
             ...Ks(),
             ...X_(),
-            ...Ga(),
+            ...Ka(),
             ...An(),
             ...I4(),
             ...D4()
         }, "VExpansionPanel"),
         T2e = at()({
             name: "VExpansionPanel",
             props: L4(),
@@ -53502,15 +53507,15 @@
                     var I = l[$];
                     (I.from < v && I.to > d || d == v && I.to == d) && (m(Math.max(I.from, d), Math.min(I.to, v), I.level == 1 ? "rtl" : "ltr", $), b = !0)
                 }
                 b || m(d, v, "ltr")
             }
             var sa = null;
 
-            function Ka(l, d, v) {
+            function Xa(l, d, v) {
                 var m;
                 sa = null;
                 for (var b = 0; b < l.length; ++b) {
                     var $ = l[b];
                     if ($.from < d && $.to > d) return b;
                     $.to == d && ($.from != $.to && v == "before" ? m = b : sa = b), $.from == d && ($.from != $.to && v != "before" ? m = b : sa = b)
                 }
@@ -53564,33 +53569,33 @@
                     }
                     for (var ya = 0; ya < Ae; ++ya)
                         if (b.test(xe[ya])) {
                             var ua = void 0;
                             for (ua = ya + 1; ua < Ae && b.test(xe[ua]); ++ua);
                             for (var jr = (ya ? xe[ya - 1] : _e) == "L", Li = (ua < Ae ? xe[ua] : _e) == "L", Hf = jr == Li ? jr ? "L" : "R" : _e, Iu = ya; Iu < ua; ++Iu) xe[Iu] = Hf;
                             ya = ua - 1
-                        } for (var Za = [], zo, xa = 0; xa < Ae;)
+                        } for (var Qa = [], zo, xa = 0; xa < Ae;)
                         if (I.test(xe[xa])) {
                             var iS = xa;
                             for (++xa; xa < Ae && I.test(xe[xa]); ++xa);
-                            Za.push(new z(0, iS, xa))
+                            Qa.push(new z(0, iS, xa))
                         } else {
                             var Nl = xa,
-                                id = Za.length,
+                                id = Qa.length,
                                 sd = me == "rtl" ? 1 : 0;
                             for (++xa; xa < Ae && xe[xa] != "L"; ++xa);
                             for (var hi = Nl; hi < xa;)
                                 if (j.test(xe[hi])) {
-                                    Nl < hi && (Za.splice(id, 0, new z(1, Nl, hi)), id += sd);
+                                    Nl < hi && (Qa.splice(id, 0, new z(1, Nl, hi)), id += sd);
                                     var Wf = hi;
                                     for (++hi; hi < xa && j.test(xe[hi]); ++hi);
-                                    Za.splice(id, 0, new z(2, Wf, hi)), id += sd, Nl = hi
+                                    Qa.splice(id, 0, new z(2, Wf, hi)), id += sd, Nl = hi
                                 } else ++hi;
-                            Nl < xa && Za.splice(id, 0, new z(1, Nl, xa))
-                        } return me == "ltr" && (Za[0].level == 1 && (zo = Z.match(/^\s+/)) && (Za[0].from = zo[0].length, Za.unshift(new z(0, 0, zo[0].length))), re(Za).level == 1 && (zo = Z.match(/\s+$/)) && (re(Za).to -= zo[0].length, Za.push(new z(0, Ae - zo[0].length, Ae)))), me == "rtl" ? Za.reverse() : Za
+                            Nl < xa && Qa.splice(id, 0, new z(1, Nl, xa))
+                        } return me == "ltr" && (Qa[0].level == 1 && (zo = Z.match(/^\s+/)) && (Qa[0].from = zo[0].length, Qa.unshift(new z(0, 0, zo[0].length))), re(Qa).level == 1 && (zo = Z.match(/\s+$/)) && (re(Qa).to -= zo[0].length, Qa.push(new z(0, Ae - zo[0].length, Ae)))), me == "rtl" ? Qa.reverse() : Qa
                 }
             }();
 
             function Se(l, d) {
                 var v = l.order;
                 return v == null && (v = l.order = Ie(l.text, d)), v
             }
@@ -53807,15 +53812,15 @@
                 for (var v; l.innerMode && (v = l.innerMode(d), !(!v || v.mode == l));) d = v.state, l = v.mode;
                 return v || {
                     mode: l,
                     state: d
                 }
             }
 
-            function Xa(l, d, v) {
+            function Ja(l, d, v) {
                 return l.startState ? l.startState(d, v) : !0
             }
             var qn = function(l, d, v) {
                 this.pos = this.start = 0, this.string = l, this.tabSize = d || 8, this.lastColumnPos = this.lastColumnValue = 0, this.lineStart = 0, this.lineOracle = v
             };
             qn.prototype.eol = function() {
                 return this.pos >= this.string.length
@@ -54063,15 +54068,15 @@
 
             function Bp(l, d, v) {
                 var m = l.doc,
                     b = l.display;
                 if (!m.mode.startState) return new Ho(m, !0, d);
                 var $ = uq(l, d, v),
                     I = $ > m.first && St(m, $ - 1).stateAfter,
-                    j = I ? Ho.fromSaved(m, I, $) : new Ho(m, Xa(m.mode), $);
+                    j = I ? Ho.fromSaved(m, I, $) : new Ho(m, Ja(m.mode), $);
                 return m.iter($, d, function(z) {
                     pw(l, z.text, j);
                     var Z = j.line;
                     z.stateAfter = Z == d - 1 || Z % 5 == 0 || Z >= b.viewFrom && Z < b.viewTo ? j.save() : null, j.nextLine()
                 }), v && (m.modeFrontier = j.line), j
             }
 
@@ -55104,15 +55109,15 @@
                 if (z >= m.text.length ? (z = m.text.length, Z = "before") : z <= 0 && (z = 0, Z = "after"), !j) return I(Z == "before" ? z - 1 : z, Z == "before");
 
                 function me(ze, Xe, rt) {
                     var lt = j[Xe],
                         pt = lt.level == 1;
                     return I(rt ? ze - 1 : ze, pt != rt)
                 }
-                var _e = Ka(j, z, Z),
+                var _e = Xa(j, z, Z),
                     Ae = sa,
                     xe = me(z, _e, Z == "before");
                 return Ae != null && (xe.other = me(z, Ae, Z != "before")), xe
             }
 
             function QA(l, d) {
                 var v = 0;
@@ -55485,25 +55490,25 @@
                     var Di = Se(Dt, b.direction);
                     return Nr(Di, _t || 0, Ft ?? nn, function(la, Ii, Wa, ya) {
                         var ua = Wa == "ltr",
                             jr = Dr(la, ua ? "left" : "right"),
                             Li = Dr(Ii - 1, ua ? "right" : "left"),
                             Hf = _t == null && la == 0,
                             Iu = Ft == null && Ii == nn,
-                            Za = ya == 0,
+                            Qa = ya == 0,
                             zo = !Di || ya == Di.length - 1;
                         if (Li.top - jr.top <= 3) {
-                            var xa = (Z ? Hf : Iu) && Za,
+                            var xa = (Z ? Hf : Iu) && Qa,
                                 iS = (Z ? Iu : Hf) && zo,
                                 Nl = xa ? j : (ua ? jr : Li).left,
                                 id = iS ? z : (ua ? Li : jr).right;
                             me(Nl, jr.top, id - Nl, jr.bottom)
                         } else {
                             var sd, hi, Wf, sS;
-                            ua ? (sd = Z && Hf && Za ? j : jr.left, hi = Z ? z : Gi(la, Wa, "before"), Wf = Z ? j : Gi(Ii, Wa, "after"), sS = Z && Iu && zo ? z : Li.right) : (sd = Z ? Gi(la, Wa, "before") : j, hi = !Z && Hf && Za ? z : jr.right, Wf = !Z && Iu && zo ? j : Li.left, sS = Z ? Gi(Ii, Wa, "after") : z), me(sd, jr.top, hi - sd, jr.bottom), jr.bottom < Li.top && me(j, jr.bottom, null, Li.top), me(Wf, Li.top, sS - Wf, Li.bottom)
+                            ua ? (sd = Z && Hf && Qa ? j : jr.left, hi = Z ? z : Gi(la, Wa, "before"), Wf = Z ? j : Gi(Ii, Wa, "after"), sS = Z && Iu && zo ? z : Li.right) : (sd = Z ? Gi(la, Wa, "before") : j, hi = !Z && Hf && Qa ? z : jr.right, Wf = !Z && Iu && zo ? j : Li.left, sS = Z ? Gi(Ii, Wa, "after") : z), me(sd, jr.top, hi - sd, jr.bottom), jr.bottom < Li.top && me(j, jr.bottom, null, Li.top), me(Wf, Li.top, sS - Wf, Li.bottom)
                         }(!or || uy(jr, or) < 0) && (or = jr), uy(Li, or) < 0 && (or = Li), (!Ea || uy(jr, Ea) < 0) && (Ea = jr), uy(Li, Ea) < 0 && (Ea = Li)
                     }), {
                         start: or,
                         end: Ea
                     }
                 }
                 var Ae = d.from(),
@@ -56552,30 +56557,30 @@
                         $ != ot(v, b) < 0 ? (b = d, d = v) : $ != ot(d, v) < 0 && (d = v)
                     }
                     return new Rn(b, d)
                 } else return new Rn(v || d, d)
             }
 
             function gy(l, d, v, m, b) {
-                b == null && (b = l.cm && (l.cm.display.shift || l.extend)), Ja(l, new vs([qw(l.sel.primary(), d, v, b)], 0), m)
+                b == null && (b = l.cm && (l.cm.display.shift || l.extend)), Za(l, new vs([qw(l.sel.primary(), d, v, b)], 0), m)
             }
 
             function PM(l, d, v) {
                 for (var m = [], b = l.cm && (l.cm.display.shift || l.extend), $ = 0; $ < l.sel.ranges.length; $++) m[$] = qw(l.sel.ranges[$], d[$], null, b);
                 var I = no(l.cm, m, l.sel.primIndex);
-                Ja(l, I, v)
+                Za(l, I, v)
             }
 
             function Gw(l, d, v, m) {
                 var b = l.sel.ranges.slice(0);
-                b[d] = v, Ja(l, no(l.cm, b, l.sel.primIndex), m)
+                b[d] = v, Za(l, no(l.cm, b, l.sel.primIndex), m)
             }
 
             function EM(l, d, v, m) {
-                Ja(l, xu(d, v), m)
+                Za(l, xu(d, v), m)
             }
 
             function _G(l, d, v) {
                 var m = {
                     ranges: d.ranges,
                     update: function(b) {
                         this.ranges = [];
@@ -56585,18 +56590,18 @@
                 };
                 return Pn(l, "beforeSelectionChange", l, m), l.cm && Pn(l.cm, "beforeSelectionChange", l.cm, m), m.ranges != d.ranges ? no(l.cm, m.ranges, m.ranges.length - 1) : d
             }
 
             function xM(l, d, v) {
                 var m = l.history.done,
                     b = re(m);
-                b && b.ranges ? (m[m.length - 1] = d, yy(l, d, v)) : Ja(l, d, v)
+                b && b.ranges ? (m[m.length - 1] = d, yy(l, d, v)) : Za(l, d, v)
             }
 
-            function Ja(l, d, v) {
+            function Za(l, d, v) {
                 yy(l, d, v), gG(l, l.sel, l.cm ? l.cm.curOp.id : NaN, v)
             }
 
             function yy(l, d, v) {
                 (Kr(l, "beforeSelectionChange") || l.cm && Kr(l.cm, "beforeSelectionChange")) && (d = _G(l, d, v));
                 var m = v && v.bias || (ot(d.primary().head, l.sel.primary().head) < 0 ? -1 : 1);
                 OM(l, MM(l, d, m, !0)), !(v && v.scroll === !1) && l.cm && l.cm.getOption("readOnly") != "nocursor" && Af(l.cm)
@@ -56716,15 +56721,15 @@
                 var m = l.cm && l.cm.state.suppressEdits;
                 if (!(m && !v)) {
                     for (var b = l.history, $, I = l.sel, j = d == "undo" ? b.done : b.undone, z = d == "undo" ? b.undone : b.done, Z = 0; Z < j.length && ($ = j[Z], !(v ? $.ranges && !$.equals(l.sel) : !$.ranges)); Z++);
                     if (Z != j.length) {
                         for (b.lastOrigin = b.lastSelOrigin = null;;)
                             if ($ = j.pop(), $.ranges) {
                                 if (vy($, z), v && !$.equals(l.sel)) {
-                                    Ja(l, $, {
+                                    Za(l, $, {
                                         clearRedo: !1
                                     });
                                     return
                                 }
                                 I = $
                             } else if (m) {
                             j.push($);
@@ -57189,15 +57194,15 @@
                     if (!(this instanceof Mi)) return new Mi(l, d, v, m, b);
                     v == null && (v = 0), am.call(this, [new rm([new Cf("", null)])]), this.first = v, this.scrollTop = this.scrollLeft = 0, this.cantEdit = !1, this.cleanGeneration = 1, this.modeFrontier = this.highlightFrontier = v;
                     var $ = Be(v, 0);
                     this.sel = xu($), this.history = new my(null), this.id = ++TG, this.modeOption = d, this.lineSep = m, this.direction = b == "rtl" ? "rtl" : "ltr", this.extend = !1, typeof l == "string" && (l = this.splitLines(l)), zw(this, {
                         from: $,
                         to: $,
                         text: l
-                    }), Ja(this, xu($), J)
+                    }), Za(this, xu($), J)
                 };
             Mi.prototype = nt(am.prototype, {
                 constructor: Mi,
                 iter: function(l, d, v) {
                     v ? this.iterN(l - this.first, d - l, v) : this.iterN(this.first, this.first + this.size, l)
                 },
                 insert: function(l, d) {
@@ -57216,15 +57221,15 @@
                         v = this.first + this.size - 1;
                     Lf(this, {
                         from: d,
                         to: Be(v, St(this, v).text.length),
                         text: this.splitLines(l),
                         origin: "setValue",
                         full: !0
-                    }, !0), this.cm && Gp(this.cm, 0, 0), Ja(this, xu(d), J)
+                    }, !0), this.cm && Gp(this.cm, 0, 0), Za(this, xu(d), J)
                 }),
                 replaceRange: function(l, d, v, m) {
                     d = qt(this, d), v = v ? qt(this, v) : d, Rf(this, l, d, v, m)
                 },
                 getRange: function(l, d, v) {
                     var m = Xr(this, qt(this, l), qt(this, d));
                     return v === !1 ? m : v === "" ? m.join("") : m.join(v || this.lineSeparator())
@@ -57280,20 +57285,20 @@
                 extendSelectionsBy: Pa(function(l, d) {
                     var v = ie(this.sel.ranges, l);
                     PM(this, yA(this, v), d)
                 }),
                 setSelections: Pa(function(l, d, v) {
                     if (l.length) {
                         for (var m = [], b = 0; b < l.length; b++) m[b] = new Rn(qt(this, l[b].anchor), qt(this, l[b].head || l[b].anchor));
-                        d == null && (d = Math.min(l.length - 1, this.sel.primIndex)), Ja(this, no(this.cm, m, d), v)
+                        d == null && (d = Math.min(l.length - 1, this.sel.primIndex)), Za(this, no(this.cm, m, d), v)
                     }
                 }),
                 addSelection: Pa(function(l, d, v) {
                     var m = this.sel.ranges.slice(0);
-                    m.push(new Rn(qt(this, l), qt(this, d || l))), Ja(this, no(this.cm, m, m.length - 1), v)
+                    m.push(new Rn(qt(this, l), qt(this, d || l))), Za(this, no(this.cm, m, m.length - 1), v)
                 }),
                 getSelection: function(l) {
                     for (var d = this.sel.ranges, v, m = 0; m < d.length; m++) {
                         var b = Xr(this, d[m].from(), d[m].to());
                         v = v ? v.concat(b) : b
                     }
                     return l === !1 ? v : v.join(l || this.lineSeparator())
@@ -57948,15 +57953,15 @@
                 return new Be(m, b < 0 ? v.text.length : 0, b < 0 ? "before" : "after")
             }
 
             function LG(l, d, v, m) {
                 var b = Se(d, l.doc.direction);
                 if (!b) return Xw(d, v, m);
                 v.ch >= d.text.length ? (v.ch = d.text.length, v.sticky = "before") : v.ch <= 0 && (v.ch = 0, v.sticky = "after");
-                var $ = Ka(b, v.ch, v.sticky),
+                var $ = Xa(b, v.ch, v.sticky),
                     I = b[$];
                 if (l.doc.direction == "ltr" && I.level % 2 == 0 && (m > 0 ? I.to > v.ch : I.from < v.ch)) return Xw(d, v, m);
                 var j = function(lt, pt) {
                         return Kw(d, lt instanceof Be ? lt.ch : lt, pt)
                     },
                     z, Z = function(lt) {
                         return l.options.lineWrapping ? (z = z || Pf(l, d), tM(l, d, z, lt)) : {
@@ -58457,43 +58462,43 @@
                 var I, j, z = $.sel,
                     Z = z.ranges;
                 if (m.addNew && !m.extend ? (j = $.sel.contains(v), j > -1 ? I = Z[j] : I = new Rn(v, v)) : (I = $.sel.primary(), j = $.sel.primIndex), m.unit == "rectangle") m.addNew || (I = new Rn(v, v)), v = Qc(l, d, !0, !0), j = -1;
                 else {
                     var me = iD(l, v, m.unit);
                     m.extend ? I = qw(I, me.anchor, me.head, m.extend) : I = me
                 }
-                m.addNew ? j == -1 ? (j = Z.length, Ja($, no(l, Z.concat([I]), j), {
+                m.addNew ? j == -1 ? (j = Z.length, Za($, no(l, Z.concat([I]), j), {
                     scroll: !1,
                     origin: "*mouse"
-                })) : Z.length > 1 && Z[j].empty() && m.unit == "char" && !m.extend ? (Ja($, no(l, Z.slice(0, j).concat(Z.slice(j + 1)), 0), {
+                })) : Z.length > 1 && Z[j].empty() && m.unit == "char" && !m.extend ? (Za($, no(l, Z.slice(0, j).concat(Z.slice(j + 1)), 0), {
                     scroll: !1,
                     origin: "*mouse"
-                }), z = $.sel) : Gw($, j, I, oe) : (j = 0, Ja($, new vs([I], 0), oe), z = $.sel);
+                }), z = $.sel) : Gw($, j, I, oe) : (j = 0, Za($, new vs([I], 0), oe), z = $.sel);
                 var _e = v;
 
                 function Ae(ut) {
                     if (ot(_e, ut) != 0)
                         if (_e = ut, m.unit == "rectangle") {
                             for (var _t = [], Ft = l.options.tabSize, Dt = pe(St($, v.line).text, v.ch, Ft), nn = pe(St($, ut.line).text, ut.ch, Ft), or = Math.min(Dt, nn), Ea = Math.max(Dt, nn), Dr = Math.min(v.line, ut.line), Gi = Math.min(l.lastLine(), Math.max(v.line, ut.line)); Dr <= Gi; Dr++) {
                                 var Di = St($, Dr).text,
                                     la = ye(Di, or, Ft);
                                 or == Ea ? _t.push(new Rn(Be(Dr, la), Be(Dr, la))) : Di.length > la && _t.push(new Rn(Be(Dr, la), Be(Dr, ye(Di, Ea, Ft))))
                             }
-                            _t.length || _t.push(new Rn(v, v)), Ja($, no(l, z.ranges.slice(0, j).concat(_t), j), {
+                            _t.length || _t.push(new Rn(v, v)), Za($, no(l, z.ranges.slice(0, j).concat(_t), j), {
                                 origin: "*mouse",
                                 scroll: !1
                             }), l.scrollIntoView(ut)
                         } else {
                             var Ii = I,
                                 Wa = iD(l, ut, m.unit),
                                 ya = Ii.anchor,
                                 ua;
                             ot(Wa.anchor, ya) > 0 ? (ua = Wa.head, ya = Ds(Ii.from(), Wa.anchor)) : (ua = Wa.anchor, ya = Ha(Ii.to(), Wa.head));
                             var jr = z.ranges.slice(0);
-                            jr[j] = GG(l, new Rn(qt($, ya), ua)), Ja($, no(l, jr, j), oe)
+                            jr[j] = GG(l, new Rn(qt($, ya), ua)), Za($, no(l, jr, j), oe)
                         }
                 }
                 var xe = b.wrapper.getBoundingClientRect(),
                     ze = 0;
 
                 function Xe(ut) {
                     var _t = ++ze,
@@ -58526,23 +58531,23 @@
             function GG(l, d) {
                 var v = d.anchor,
                     m = d.head,
                     b = St(l.doc, v.line);
                 if (ot(v, m) == 0 && v.sticky == m.sticky) return d;
                 var $ = Se(b);
                 if (!$) return d;
-                var I = Ka($, v.ch, v.sticky),
+                var I = Xa($, v.ch, v.sticky),
                     j = $[I];
                 if (j.from != v.ch && j.to != v.ch) return d;
                 var z = I + (j.from == v.ch == (j.level != 1) ? 0 : 1);
                 if (z == 0 || z == $.length) return d;
                 var Z;
                 if (m.line != v.line) Z = (m.line - v.line) * (l.doc.direction == "ltr" ? 1 : -1) > 0;
                 else {
-                    var me = Ka($, m.ch, m.sticky),
+                    var me = Xa($, m.ch, m.sticky),
                         _e = me - I || (m.ch - v.ch) * (j.level == 1 ? -1 : 1);
                     me == z - 1 || me == z ? Z = _e < 0 : Z = _e > 0
                 }
                 var Ae = $[z + (Z ? -1 : 0)],
                     xe = Z == (Ae.level == 1),
                     ze = xe ? Ae.from : Ae.to,
                     Xe = xe ? "after" : "before";
@@ -59534,15 +59539,15 @@
                         return
                     }
                     if (!this.composing) {
                         this.rememberSelection();
                         var v = Ty(d, l.anchorNode, l.anchorOffset),
                             m = Ty(d, l.focusNode, l.focusOffset);
                         v && m && qi(d, function() {
-                            Ja(d.doc, xu(v, m), J), (v.bad || m.bad) && (d.curOp.selectionChanged = !0)
+                            Za(d.doc, xu(v, m), J), (v.bad || m.bad) && (d.curOp.selectionChanged = !0)
                         })
                     }
                 }
             }, Gn.prototype.pollContent = function() {
                 this.readDOMTimeout != null && (clearTimeout(this.readDOMTimeout), this.readDOMTimeout = null);
                 var l = this.cm,
                     d = l.display,
@@ -59598,15 +59603,15 @@
                 var v = $w(l, d.line);
                 if (!v || v.hidden) return null;
                 var m = St(l.doc, d.line),
                     b = UA(v, m, d.line),
                     $ = Se(m, l.doc.direction),
                     I = "left";
                 if ($) {
-                    var j = Ka($, d.ch);
+                    var j = Xa($, d.ch);
                     I = j % 2 ? "right" : "left"
                 }
                 var z = qA(b.map, d.ch, I);
                 return z.offset = z.collapse == "right" ? z.end : z.start, z
             }
 
             function t9(l) {
@@ -59862,15 +59867,15 @@
                     m = v.display,
                     b = d.textarea;
                 d.contextMenuPending && d.contextMenuPending();
                 var $ = Qc(v, l),
                     I = m.scroller.scrollTop;
                 if (!$ || _) return;
                 var j = v.options.resetSelectionOnContextMenu;
-                j && v.doc.sel.contains($) == -1 && Ta(v, Ja)(v.doc, xu($), J);
+                j && v.doc.sel.contains($) == -1 && Ta(v, Za)(v.doc, xu($), J);
                 var z = b.style.cssText,
                     Z = d.wrapper.style.cssText,
                     me = d.wrapper.offsetParent.getBoundingClientRect();
                 d.wrapper.style.cssText = "position: static", b.style.cssText = `position: absolute; width: 30px; height: 30px;
       top: ` + (l.clientY - me.top - 5) + "px; left: " + (l.clientX - me.left - 5) + `px;
       z-index: 1000; background: ` + (u ? "rgba(255, 255, 255, .05)" : "transparent") + `;
       outline: none; border-width: 0; outline: none; overflow: hidden; opacity: .05; filter: alpha(opacity=5);`;
@@ -59935,15 +59940,15 @@
                 var j = _r(function(z) {
                     return l.parentNode.insertBefore(z, l.nextSibling)
                 }, d);
                 return j
             }
 
             function i9(l) {
-                l.off = bn, l.on = Ue, l.wheelEventPixels = fG, l.Doc = Mi, l.splitLines = je, l.countColumn = pe, l.findColumn = ye, l.isWordChar = Pe, l.Pass = K, l.signal = Pn, l.Line = Cf, l.changeEnd = Ou, l.scrollbarModel = cM, l.Pos = Be, l.cmpPos = ot, l.modes = sr, l.mimeModes = Yt, l.resolveMode = Wt, l.getMode = Bn, l.modeExtensions = tr, l.extendMode = Hn, l.copyState = $a, l.startState = Xa, l.innerMode = ci, l.commands = um, l.keyMap = Rl, l.keyName = XM, l.isModifierKey = GM, l.lookupKey = Ff, l.normalizeKeyMap = IG, l.StringStream = qn, l.SharedTextMarker = sm, l.TextMarker = Mu, l.LineWidget = im, l.e_preventDefault = Vr, l.e_stopPropagation = Ms, l.e_stop = Bo, l.addClass = X, l.contains = ue, l.rmClass = B, l.keyNames = Du
+                l.off = bn, l.on = Ue, l.wheelEventPixels = fG, l.Doc = Mi, l.splitLines = je, l.countColumn = pe, l.findColumn = ye, l.isWordChar = Pe, l.Pass = K, l.signal = Pn, l.Line = Cf, l.changeEnd = Ou, l.scrollbarModel = cM, l.Pos = Be, l.cmpPos = ot, l.modes = sr, l.mimeModes = Yt, l.resolveMode = Wt, l.getMode = Bn, l.modeExtensions = tr, l.extendMode = Hn, l.copyState = $a, l.startState = Ja, l.innerMode = ci, l.commands = um, l.keyMap = Rl, l.keyName = XM, l.isModifierKey = GM, l.lookupKey = Ff, l.normalizeKeyMap = IG, l.StringStream = qn, l.SharedTextMarker = sm, l.TextMarker = Mu, l.LineWidget = im, l.e_preventDefault = Vr, l.e_stopPropagation = Ms, l.e_stop = Bo, l.addClass = X, l.contains = ue, l.rmClass = B, l.keyNames = Du
             }
             XG(_r), e9(_r);
             var s9 = "iter insert remove copy getEditor constructor".split(" ");
             for (var Py in Mi.prototype) Mi.prototype.hasOwnProperty(Py) && ve(s9, Py) < 0 && (_r.prototype[Py] = function(l) {
                 return function() {
                     return l.apply(this.doc, arguments)
                 }
@@ -60444,15 +60449,15 @@
                     }
                 }
 
                 function sa(te, be) {
                     if (f && (te == ":" || be == "in")) return D(Se)
                 }
 
-                function Ka(te) {
+                function Xa(te) {
                     if (f && te == ":") return W.stream.match(/^\s*\w+\s+is\b/, !1) ? D(ve, Ie, Se) : D(Se)
                 }
 
                 function Ie(te, be) {
                     if (be == "is") return W.marked = "keyword", D()
                 }
 
@@ -60561,22 +60566,22 @@
                 function We(te, be) {
                     return te == ")" ? D() : te == ";" ? D(We) : be == "in" || be == "of" ? (W.marked = "keyword", D(ve, We)) : ee(ve, We)
                 }
 
                 function je(te, be) {
                     if (be == "*") return W.marked = "keyword", D(je);
                     if (te == "variable") return se(be), D(je);
-                    if (te == "(") return D(M, H(")"), At(Kt, ")"), V, Ka, pe, L);
+                    if (te == "(") return D(M, H(")"), At(Kt, ")"), V, Xa, pe, L);
                     if (f && be == "<") return D(H(">"), At(Fr, ">"), V, je)
                 }
 
                 function Ot(te, be) {
                     if (be == "*") return W.marked = "keyword", D(Ot);
                     if (te == "variable") return se(be), D(Ot);
-                    if (te == "(") return D(M, H(")"), At(Kt, ")"), V, Ka, L);
+                    if (te == "(") return D(M, H(")"), At(Kt, ")"), V, Xa, L);
                     if (f && be == "<") return D(H(">"), At(Fr, ">"), V, Ot)
                 }
 
                 function Lt(te, be) {
                     if (te == "keyword" || te == "variable") return W.marked = "type", D(Lt);
                     if (be == "<") return D(H(">"), At(Fr, ">"), V)
                 }
@@ -60617,39 +60622,39 @@
                     if (be == "=") return D(ne);
                     var Ge = W.state.lexical.prev,
                         tt = Ge && Ge.info == "interface";
                     return ee(tt ? Ot : je)
                 }
 
                 function Wt(te, be) {
-                    return be == "*" ? (W.marked = "keyword", D(Xa, ae(";"))) : be == "default" ? (W.marked = "keyword", D(ve, ae(";"))) : te == "{" ? D(At(Bn, "}"), Xa, ae(";")) : ee(pe)
+                    return be == "*" ? (W.marked = "keyword", D(Ja, ae(";"))) : be == "default" ? (W.marked = "keyword", D(ve, ae(";"))) : te == "{" ? D(At(Bn, "}"), Ja, ae(";")) : ee(pe)
                 }
 
                 function Bn(te, be) {
                     if (be == "as") return W.marked = "keyword", D(ae("variable"));
                     if (te == "variable") return ee(ne, Bn)
                 }
 
                 function tr(te) {
-                    return te == "string" ? D() : te == "(" ? ee(ve) : te == "." ? ee(le) : ee(Hn, $a, Xa)
+                    return te == "string" ? D() : te == "(" ? ee(ve) : te == "." ? ee(le) : ee(Hn, $a, Ja)
                 }
 
                 function Hn(te, be) {
                     return te == "{" ? Ln(Hn, "}") : (te == "variable" && se(be), be == "*" && (W.marked = "keyword"), D(ci))
                 }
 
                 function $a(te) {
                     if (te == ",") return D(Hn, $a)
                 }
 
                 function ci(te, be) {
                     if (be == "as") return W.marked = "keyword", D(Hn)
                 }
 
-                function Xa(te, be) {
+                function Ja(te, be) {
                     if (be == "from") return W.marked = "keyword", D(ve)
                 }
 
                 function qn(te) {
                     return te == "]" ? D() : ee(At(ne, "]"))
                 }
 
@@ -61679,15 +61684,15 @@
         ["render", zje]
     ]);
     async function qje(e, t, n, r, a, i, s, o) {
         if (!N_()) return;
         let u = {};
         for (const [c, f] of Object.entries(s || {})) f != null && (typeof f != "string" || f.length < 1e3) && (u[c] = f);
         return await new Promise((c, f) => {
-            const h = `${li.backend_prefix}autocompete/${t}/${e}/`;
+            const h = `${Ga.backend_prefix}autocompete/${t}/${e}/`;
             yu({
                 url: h,
                 method: "post",
                 data: {
                     search_string: n,
                     limit: r,
                     viewname: a,
@@ -70286,15 +70291,15 @@
                             config: y.config,
                             "is-last": y.autoApply && !ke(s).keepActionRow,
                             "hide-navigation": y.hideNavigation,
                             "aria-labels": y.ariaLabels,
                             type: "year",
                             onToggle: p,
                             onSelected: w[4] || (w[4] = x => g(x))
-                        }, si({
+                        }, oi({
                             "button-icon": fe(() => [y.$slots["calendar-icon"] ? kt(y.$slots, "calendar-icon", {
                                 key: 0
                             }) : Ve("", !0), y.$slots["calendar-icon"] ? Ve("", !0) : (ce(), Le(ke(jp), {
                                 key: 1
                             }))]),
                             _: 2
                         }, [y.$slots["year-overlay-value"] ? {
@@ -70650,25 +70655,25 @@
                         height: ke(p).modeHeight,
                         config: O.config,
                         "no-overlay-focus": !!(O.noOverlayFocus || O.textInput),
                         "use-relative": "",
                         type: "month",
                         onSelected: U => ke(S)(U, F),
                         onHoverValue: U => ke(w)(U, F)
-                    }, si({
+                    }, oi({
                         header: fe(() => [T(Q8, Ee(O.$props, {
                             items: ke(u)(F),
                             instance: F,
                             "show-year-picker": ke(g)[F],
                             year: ke(c)(F),
                             "is-disabled": U => ke(f)(F, U),
                             onHandleYear: U => ke(E)(F, U),
                             onYearSelect: U => ke(x)(U, F),
                             onToggleYearPicker: U => ke(C)(F, U == null ? void 0 : U.flow, U == null ? void 0 : U.show)
-                        }), si({
+                        }), oi({
                             _: 2
                         }, [Et(ke(i), (U, G) => ({
                             name: U,
                             fn: fe(B => [kt(O.$slots, U, hr(ea(B)))])
                         }))]), 1040, ["items", "instance", "show-year-picker", "year", "is-disabled", "onHandleYear", "onYearSelect", "onToggleYearPicker"])]),
                         _: 2
                     }, [O.$slots["month-overlay-value"] ? {
@@ -70778,15 +70783,15 @@
                     config: h.config,
                     "no-overlay-focus": !!(h.noOverlayFocus || h.textInput),
                     "focus-value": ke(o),
                     type: "year",
                     "use-relative": "",
                     onSelected: ke(u),
                     onHoverValue: ke(c)
-                }, si({
+                }, oi({
                     _: 2
                 }, [h.$slots["year-overlay-value"] ? {
                     name: "item",
                     fn: fe(({
                         item: g
                     }) => [kt(h.$slots, "year-overlay-value", {
                         text: g.text,
@@ -71142,15 +71147,15 @@
                             "text-input": ne.textInput,
                             config: ne.config,
                             "arrow-navigation": ne.arrowNavigation,
                             "aria-labels": ne.ariaLabels,
                             onSelected: ye => ve(oe.type, ye),
                             onToggle: ye => M(oe.type),
                             onResetFlow: K[1] || (K[1] = ye => ne.$emit("reset-flow"))
-                        }, si({
+                        }, oi({
                             "button-icon": fe(() => [ne.$slots["clock-icon"] ? kt(ne.$slots, "clock-icon", {
                                 key: 0
                             }) : Ve("", !0), ne.$slots["clock-icon"] ? Ve("", !0) : (ce(), Le(Cs(ne.timePickerInline ? ke(jp) : ke(UO)), {
                                 key: 1
                             }))]),
                             _: 2
                         }, [ne.$slots[`${oe.type}-overlay-value`] ? {
@@ -71363,15 +71368,15 @@
                                 "onUpdate:hours": M => B(G(M, q, "hours")),
                                 "onUpdate:minutes": M => W(G(M, q, "minutes")),
                                 "onUpdate:seconds": M => ee(G(M, q, "seconds")),
                                 onMounted: D,
                                 onOverlayClosed: Q,
                                 onOverlayOpened: ue[2] || (ue[2] = M => se.$emit("overlay-opened", M)),
                                 onAmPmChange: ue[3] || (ue[3] = M => se.$emit("am-pm-change", M))
-                            }), si({
+                            }), oi({
                                 _: 2
                             }, [Et(ke(U), (M, P) => ({
                                 name: M,
                                 fn: fe(L => [kt(se.$slots, M, Ee({
                                     ref_for: !0
                                 }, L))])
                             }))]), 1040, ["validate-time", "onUpdate:hours", "onUpdate:minutes", "onUpdate:seconds"])), [
@@ -71605,15 +71610,15 @@
                             open: !1,
                             overlay: y
                         })),
                         onOverlayOpened: _[6] || (_[6] = y => g.$emit("overlay-toggle", {
                             open: !0,
                             overlay: y
                         }))
-                    }), si({
+                    }), oi({
                         _: 2
                     }, [Et(ke(s), (y, w) => ({
                         name: y,
                         fn: fe(S => [kt(g.$slots, y, hr(ea(S)))])
                     }))]), 1040, ["hours", "minutes", "seconds", "internal-model-value", "disabled-times-config", "validate-time"])]),
                     _: 3
                 }))
@@ -71852,15 +71857,15 @@
                             "header-refs": [],
                             "esc-close": N.escClose,
                             "menu-wrap-ref": N.menuWrapRef,
                             "text-input": N.textInput,
                             "aria-labels": N.ariaLabels,
                             onSelected: H.updateModelValue,
                             onToggle: H.toggle
-                        }, si({
+                        }, oi({
                             "button-icon": fe(() => [N.$slots["calendar-icon"] ? kt(N.$slots, "calendar-icon", {
                                 key: 0
                             }) : Ve("", !0), N.$slots["calendar-icon"] ? Ve("", !0) : (ce(), Le(ke(jp), {
                                 key: 1
                             }))]),
                             _: 2
                         }, [N.$slots[`${H.type}-overlay-value`] ? {
@@ -72538,21 +72543,21 @@
                 },
                 Nr = () => {
                     g.value.enabled ? o.value && Array.isArray(o.value) && o.value[0] ? o.value = Qr(et(), o.value[0]) ? [et(), o.value[0]] : [o.value[0], et()] : o.value = [et()] : o.value = et(), Q()
                 },
                 sa = () => {
                     if (Array.isArray(o.value))
                         if (S.value.enabled) {
-                            const Ie = Ka();
+                            const Ie = Xa();
                             o.value[o.value.length - 1] = O(Ie)
                         } else o.value = o.value.map((Ie, Se) => Ie && O(Ie, Se));
                     else o.value = O(o.value);
                     t("time-update")
                 },
-                Ka = () => Array.isArray(o.value) && o.value.length ? o.value[o.value.length - 1] : null;
+                Xa = () => Array.isArray(o.value) && o.value.length ? o.value[o.value.length - 1] : null;
             return {
                 calendars: u,
                 modelValue: o,
                 month: B,
                 year: W,
                 time: c,
                 disabledTimesConfig: G,
@@ -72743,15 +72748,15 @@
                         onResetFlow: ne[1] || (ne[1] = oe => ve.$emit("reset-flow")),
                         onUpdateMonthYear: oe => ke(C)(K, oe),
                         onOverlayClosed: de,
                         onOverlayOpened: ne[2] || (ne[2] = oe => ve.$emit("overlay-toggle", {
                             open: !0,
                             overlay: oe
                         }))
-                    }), si({
+                    }), oi({
                         _: 2
                     }, [Et(ke(Q), (oe, le) => ({
                         name: oe,
                         fn: fe(ye => [kt(ve.$slots, oe, hr(ea(ye)))])
                     }))]), 1040, ["months", "years", "month", "year", "instance", "onUpdateMonthYear"])), T(I4e, Ee({
                         ref: oe => {
                             oe && (W.value[J] = oe)
@@ -72766,15 +72771,15 @@
                         onSetHoverDate: ne[3] || (ne[3] = oe => ke(R)(oe)),
                         onHandleScroll: oe => ke(w)(oe, K),
                         onHandleSwipe: oe => ke(S)(oe, K),
                         onMount: ne[4] || (ne[4] = oe => ue(ke(Gd).calendar)),
                         onResetFlow: ne[5] || (ne[5] = oe => ve.$emit("reset-flow")),
                         onTooltipOpen: ne[6] || (ne[6] = oe => ve.$emit("tooltip-open", oe)),
                         onTooltipClose: ne[7] || (ne[7] = oe => ve.$emit("tooltip-close", oe))
-                    }), si({
+                    }), oi({
                         _: 2
                     }, [Et(ke(D), (oe, le) => ({
                         name: oe,
                         fn: fe(ye => [kt(ve.$slots, oe, hr(ea({
                             ...ye
                         })))])
                     }))]), 1040, ["mapped-dates", "month", "year", "instance", "onSelectDate", "onHandleSpace", "onHandleScroll", "onHandleSwipe"])]),
@@ -72799,15 +72804,15 @@
                     "onUpdate:hours": ne[9] || (ne[9] = K => ke(A)(K)),
                     "onUpdate:minutes": ne[10] || (ne[10] = K => ke(A)(K, !1)),
                     "onUpdate:seconds": ne[11] || (ne[11] = K => ke(A)(K, !1, !0)),
                     onResetFlow: ne[12] || (ne[12] = K => ve.$emit("reset-flow")),
                     onOverlayClosed: ne[13] || (ne[13] = K => pe(K, !1)),
                     onOverlayOpened: ne[14] || (ne[14] = K => pe(K, !0)),
                     onAmPmChange: ne[15] || (ne[15] = K => ve.$emit("am-pm-change", K))
-                }), si({
+                }), oi({
                     _: 2
                 }, [Et(ke(se), (K, J) => ({
                     name: K,
                     fn: fe(oe => [kt(ve.$slots, K, hr(ea(oe)))])
                 }))]), 1040, ["hours", "minutes", "seconds", "internal-model-value", "disabled-times-config", "validate-time"]))])) : Ve("", !0)], 64))
             }
         }),
@@ -72987,15 +72992,15 @@
                         instance: A,
                         "show-year-picker": ke(_)[A],
                         year: ke(f)(A),
                         "is-disabled": O => ke(h)(A, O),
                         onHandleYear: O => ke(C)(A, O),
                         onYearSelect: O => ke(k)(O, A),
                         onToggleYearPicker: O => ke(S)(A, O == null ? void 0 : O.flow, O == null ? void 0 : O.show)
-                    }), si({
+                    }), oi({
                         _: 2
                     }, [Et(ke(s), (O, R) => ({
                         name: O,
                         fn: fe(F => [kt(x.$slots, O, hr(ea(F)))])
                     }))]), 1040, ["items", "instance", "show-year-picker", "year", "is-disabled", "onHandleYear", "onYearSelect", "onToggleYearPicker"])]), mt("div", V4e, [(ce(!0), Oe(Ne, null, Et(ke(p)(A), (O, R) => (ce(), Oe("div", {
                         key: R
                     }, [mt("button", {
@@ -73328,15 +73333,15 @@
                         onTimePickerClose: H,
                         onRecalculatePosition: Q,
                         onUpdateMonthYear: ye[11] || (ye[11] = ie => le.$emit("update-month-year", ie)),
                         onAutoApplyInvalid: ye[12] || (ye[12] = ie => le.$emit("auto-apply-invalid", ie)),
                         onInvalidDate: ye[13] || (ye[13] = ie => le.$emit("invalid-date", ie)),
                         onOverlayToggle: ye[14] || (ye[14] = ie => le.$emit("overlay-toggle", ie)),
                         "onUpdate:internalModelValue": ye[15] || (ye[15] = ie => le.$emit("update:internal-model-value", ie))
-                    }), si({
+                    }), oi({
                         _: 2
                     }, [Et(ue.value, (ie, we) => ({
                         name: ie,
                         fn: fe(Re => [kt(le.$slots, ie, hr(ea({
                             ...Re
                         })))])
                     }))]), 1040, ["flow-step", "onMount", "onUpdateFlowStep", "onResetFlow"]))], 512), le.$slots["right-sidebar"] ? (ce(), Oe("div", G4e, [kt(le.$slots, "right-sidebar", hr(ea(D.value)))])) : Ve("", !0), le.$slots["action-extra"] ? (ce(), Oe("div", K4e, [le.$slots["action-extra"] ? kt(le.$slots, "action-extra", {
@@ -73347,15 +73352,15 @@
                         "menu-mount": S.value
                     }, s.value, {
                         "calendar-width": y.value,
                         onClosePicker: ye[16] || (ye[16] = ie => le.$emit("close-picker")),
                         onSelectDate: ye[17] || (ye[17] = ie => le.$emit("select-date")),
                         onInvalidSelect: ye[18] || (ye[18] = ie => le.$emit("invalid-select")),
                         onSelectNow: de
-                    }), si({
+                    }), oi({
                         _: 2
                     }, [Et(ke(se), (ie, we) => ({
                         name: ie,
                         fn: fe(Re => [kt(le.$slots, ie, hr(ea({
                             ...Re
                         })))])
                     }))]), 1040, ["menu-mount", "calendar-width"])) : Ve("", !0)], 46, H4e)
@@ -73557,29 +73562,29 @@
                 }, Nr = Se => {
                     f.value && f.value.updateMonthYear(0, {
                         month: rF(Se.month),
                         year: rF(Se.year)
                     })
                 }, sa = Se => {
                     P(Se ?? a.modelValue)
-                }, Ka = (Se, Qe) => {
+                }, Xa = (Se, Qe) => {
                     var Ue;
                     (Ue = f.value) == null || Ue.switchView(Se, Qe)
                 }, Ie = Se => F.value.onClickOutside ? F.value.onClickOutside(Se) : Pe();
                 return Q4e(c, h, () => Ie(re)), t({
                     closeMenu: Pe,
                     selectDate: ie,
                     clearValue: He,
                     openMenu: De,
                     onScroll: J,
                     formatInputValue: H,
                     updateInternalModelValue: At,
                     setMonthYear: Nr,
                     parseModel: sa,
-                    switchView: Ka,
+                    switchView: Xa,
                     toggleMenu: yt
                 }), (Se, Qe) => (ce(), Oe("div", {
                     ref_key: "pickerWrapperRef",
                     ref: g,
                     class: Mt(ae.value),
                     "data-datepicker-instance": ""
                 }, [T(Hze, Ee({
@@ -73595,15 +73600,15 @@
                     onSetEmptyDate: ke(L),
                     onSelectDate: ie,
                     onToggle: yt,
                     onClose: Pe,
                     onFocus: Ln,
                     onBlur: Vn,
                     onRealBlur: Qe[1] || (Qe[1] = Ue => p.value = !1)
-                }), si({
+                }), oi({
                     _: 2
                 }, [Et(ke(D), (Ue, an) => ({
                     name: Ue,
                     fn: fe(bn => [kt(Se.$slots, Ue, hr(ea(bn)))])
                 }))]), 1040, ["input-value", "is-menu-open", "onSetEmptyDate"]), (ce(), Le(Cs(Se.teleport ? Qj : "div"), hr(ea(de.value)), {
                     default: fe(() => [T($i, {
                         name: ke(B)(ke(Q)),
@@ -73648,15 +73653,15 @@
                             onTimePickerClose: Qe[11] || (Qe[11] = Ue => Se.$emit("time-picker-close", Ue)),
                             onAmPmChange: Qe[12] || (Qe[12] = Ue => Se.$emit("am-pm-change", Ue)),
                             onRangeStart: Qe[13] || (Qe[13] = Ue => Se.$emit("range-start", Ue)),
                             onRangeEnd: Qe[14] || (Qe[14] = Ue => Se.$emit("range-end", Ue)),
                             onDateUpdate: Qe[15] || (Qe[15] = Ue => Se.$emit("date-update", Ue)),
                             onInvalidDate: Qe[16] || (Qe[16] = Ue => Se.$emit("invalid-date", Ue)),
                             onOverlayToggle: Qe[17] || (Qe[17] = Ue => Se.$emit("overlay-toggle", Ue))
-                        }), si({
+                        }), oi({
                             _: 2
                         }, [Et(ke(ee), (Ue, an) => ({
                             name: Ue,
                             fn: fe(bn => [kt(Se.$slots, Ue, hr(ea({
                                 ...bn
                             })))])
                         }))]), 1040, ["internal-model-value", "class", "open-on-top", "no-overlay-focus", "collapse", "onRecalculatePosition"])], 16)) : Ve("", !0)]),
@@ -73894,15 +73899,15 @@
                 getRefString(e) {
                     return `field_${e}`
                 },
                 updateErrors(e) {
                     this.errors = e
                 },
                 updateFormData(e) {
-                    updateFormData("updateFormData", e), this.formData = e;
+                    this.formData = e;
                     for (const [t, n] of Object.entries(this.serializer)) {
                         const r = this.getRefString(t),
                             a = this.$refs[r];
                         a !== void 0 && a[0].updateFormData(this.formData)
                     }
                 },
                 _updateValue(e, t) {
@@ -73919,22 +73924,25 @@
                     for (const t of Object.keys(this.errors))
                         if (e.fields.indexOf(t) !== -1) return !0;
                     return !1
                 }
             }
         },
         s6e = {
+            class: "form-title"
+        },
+        o6e = {
             key: 0,
             class: "required-title"
         },
-        o6e = {
+        l6e = {
             class: "form-error"
         };
 
-    function l6e(e, t, n, r, a, i) {
+    function u6e(e, t, n, r, a, i) {
         return ce(), Le($l, {
             fluid: "",
             class: "fields-container"
         }, {
             default: fe(() => [T(Qh, {
                 class: Mt({
                     "hide-element": i.getGroups().length <= 1,
@@ -73973,15 +73981,15 @@
                         key: 0,
                         class: "fields-cell"
                     }, {
                         default: fe(() => [T(xo, {
                             cols: "3"
                         }, {
                             default: fe(() => [T(TH, null, {
-                                default: fe(() => [mt("p", null, vt(u.label), 1), ct(), u.required ? (ce(), Oe("p", s6e, "*")) : Ve("", !0)]),
+                                default: fe(() => [mt("p", s6e, vt(u.label), 1), ct(), u.required ? (ce(), Oe("p", o6e, "*")) : Ve("", !0)]),
                                 _: 2
                             }, 1024)]),
                             _: 2
                         }, 1024), T(xo, {
                             cols: "9",
                             class: "form-field-container"
                         }, {
@@ -74042,28 +74050,28 @@
                                 viewname: n.viewname,
                                 loading: n.loading,
                                 onChanged: f => i._updateValue(f, c)
                             }, null, 40, ["field", "field-slug", "viewname", "loading", "onChanged"])) : (ce(), Oe(Ne, {
                                 key: 1
                             }, [ct(vt(u), 1)], 64))], 64)), a.errors && a.errors[c] ? (ce(!0), Oe(Ne, {
                                 key: 2
-                            }, Et(a.errors[c], f => (ce(), Oe("p", o6e, vt(f), 1))), 256)) : Ve("", !0)]),
+                            }, Et(a.errors[c], f => (ce(), Oe("p", l6e, vt(f), 1))), 256)) : Ve("", !0)]),
                             _: 2
                         }, 1024)]),
                         _: 2
                     }, 1024)) : Ve("", !0)]))), 256))]),
                     _: 2
                 }, 1032, ["text"]))), 128))]),
                 _: 1
             }, 8, ["modelValue"])]),
             _: 1
         })
     }
     const eA = xr(i6e, [
-        ["render", l6e]
+        ["render", u6e]
     ]);
     async function sY(e, t, n, r, a) {
         return new Promise((i, s) => {
             let o = {},
                 u = new URLSearchParams(o);
             const c = `${e}?${u}`;
             for (const [f, h] of Object.entries(n)) h instanceof Date && (field = dt(h).format("YYYY-MM-DDTHH:mm"));
@@ -74074,15 +74082,15 @@
                 headers: {
                     "Accept-Language": hp()
                 },
                 timeout: 1e3 * 5
             }).then(f => i(f.data)).catch(f => s(f))
         })
     }
-    const u6e = {
+    const c6e = {
         props: {
             apiInfo: {
                 type: Object,
                 required: !0
             },
             viewname: {
                 type: String,
@@ -74139,15 +74147,15 @@
                         position: "top-center"
                     })
                 })
             }
         }
     };
 
-    function c6e(e, t, n, r, a, i) {
+    function d6e(e, t, n, r, a, i) {
         const s = eA;
         return ce(), Le($c, {
             "max-width": "1200",
             "content-class": "dialog-top-position",
             persistent: "",
             modelValue: a.open,
             "onUpdate:modelValue": t[3] || (t[3] = o => a.open = o)
@@ -74198,18 +74206,18 @@
                     _: 1
                 })]),
                 _: 2
             }, 1024)) : Ve("", !0)]),
             _: 1
         }, 8, ["modelValue"])
     }
-    const oY = xr(u6e, [
-            ["render", c6e]
+    const oY = xr(c6e, [
+            ["render", d6e]
         ]),
-        d6e = {
+        f6e = {
             props: {
                 settings: {
                     type: Object,
                     required: !0
                 },
                 searchFields: {
                     type: Object,
@@ -74252,61 +74260,61 @@
                     this.filterInfo.filters[t] = e
                 },
                 applyFilter() {
                     this.$emit("filtered", this.filterInfo)
                 }
             }
         },
-        f6e = {
+        h6e = {
             class: "filters-container"
         },
-        h6e = {
+        p6e = {
             key: 0,
             class: "filter-element"
         },
-        p6e = {
+        m6e = {
             class: "filter-element"
         },
-        m6e = {
+        v6e = {
             class: "filter-element"
         };
 
-    function v6e(e, t, n, r, a, i) {
-        return ce(), Oe("div", f6e, [n.searchFields ? (ce(), Oe("div", h6e, [T(aa, {
+    function g6e(e, t, n, r, a, i) {
+        return ce(), Oe("div", h6e, [n.searchFields ? (ce(), Oe("div", p6e, [T(aa, {
             density: "compact",
             variant: "solo",
             "prepend-inner-icon": "mdi-magnify",
             modelValue: a.filterInfo.search,
             "onUpdate:modelValue": t[0] || (t[0] = s => a.filterInfo.search = s),
             clearable: !0,
             label: e.$t("search")
         }, null, 8, ["modelValue", "label"])])) : Ve("", !0), n.filtersetFields ? (ce(!0), Oe(Ne, {
             key: 1
-        }, Et(n.filtersetFields, (s, o) => (ce(), Oe("div", p6e, [i.getFieldComponent(s) ? (ce(), Le(Cs(i.getFieldComponent(s)), {
+        }, Et(n.filtersetFields, (s, o) => (ce(), Oe("div", m6e, [i.getFieldComponent(s) ? (ce(), Le(Cs(i.getFieldComponent(s)), {
             key: 0,
             density: "compact",
             variant: "solo",
             viewname: n.viewname,
             field: s,
             "field-slug": o,
             loading: !1,
             onChanged: u => i._updateValue(u, o)
         }, null, 40, ["viewname", "field", "field-slug", "onChanged"])) : (ce(), Oe(Ne, {
             key: 1
-        }, [ct(vt(s), 1)], 64))]))), 256)) : Ve("", !0), mt("div", m6e, [T(dn, {
+        }, [ct(vt(s), 1)], 64))]))), 256)) : Ve("", !0), mt("div", v6e, [T(dn, {
             onClick: i.applyFilter,
             class: "filter-apply-button",
             "prepend-icon": "mdi-magnify"
         }, {
             default: fe(() => [ct(vt(e.$t("apply")), 1)]),
             _: 1
         }, 8, ["onClick"])])])
     }
-    const ow = xr(d6e, [
-        ["render", v6e]
+    const ow = xr(f6e, [
+        ["render", g6e]
     ]);
 
     function tA(e) {
         return new Promise((t, n) => {
             let r = JSON.parse(JSON.stringify(e.pageInfo || {}));
             e.search && (r.search = e.search), e.relationNameFilter && (r.relfilter = e.relationNameFilter, r.relfilterid = e.filterId), e.inline_action && (r.inline_action = e.inline_action), r.filter_info = encodeURIComponent(JSON.stringify(e.filter_info));
             let a = new URLSearchParams;
@@ -74326,27 +74334,27 @@
                     return
                 }
                 t(s.data)
             }).catch(s => n(s))
         })
     }
 
-    function g6e(e, t, n) {
+    function y6e(e, t, n) {
         const r = document.createEvent("MouseEvents"),
             a = document.createElement("a");
         a.download = t;
         const i = new Blob([e], {
             type: n
         });
         a.href = window.URL.createObjectURL(i), a.dataset.downloadurl = [n, a.download, a.href].join(":"), r.initEvent("click", !0, !1, window, 0, 0, 0, 0, 0, !1, !1, !1, !1, 0, null), a.dispatchEvent(r)
     }
-    async function y6e(e, t, n, r, a) {
+    async function b6e(e, t, n, r, a) {
         return new Promise((i, s) => {
             console.log("Send action", t, n, r, a);
-            const o = `${li.backend_prefix}${e}/send_action/`;
+            const o = `${Ga.backend_prefix}${e}/send_action/`;
             yu({
                 url: o,
                 method: "post",
                 data: {
                     action: t,
                     ids: n,
                     send_to_all: r,
@@ -74354,15 +74362,15 @@
                 },
                 headers: {
                     "Accept-Language": hp()
                 }
             }).then(u => {
                 if (u.headers["content-type"] !== "application/json") {
                     const c = u.headers.pragma || `${dt().format("DD.MM.YYYY_HH:MM")}.csv`;
-                    g6e(u.data, c, u.headers["content-type"])
+                    y6e(u.data, c, u.headers["content-type"])
                 } else tn(u.data.action_messages.join("<br>"), {
                     type: "success",
                     position: "top-center",
                     dangerouslyHTMLString: !0
                 });
                 i(u)
             }).catch(u => {
@@ -74374,15 +74382,15 @@
                     type: "error",
                     position: "top-center",
                     dangerouslyHTMLString: !0
                 }), s(null)))
             })
         })
     }
-    const b6e = {
+    const _6e = {
             components: {
                 ModelFormCreate: oY,
                 Filters: ow
             },
             props: {
                 apiInfo: {
                     type: Object,
@@ -74577,74 +74585,74 @@
                     }
                     this.actionFormData = null, this.actionMeta = null, this.actionSelected = t, e.form_serializer ? this.actionFormDialogOpen = !0 : e.confirmation_text ? this.actionDialogConfirmation = !0 : this.applyAction()
                 },
                 getActionInfo() {
                     return this.sectionData.meta.actions[this.actionSelected]
                 },
                 applyAction() {
-                    this.actionLoading = !1, y6e(this.viewname, this.actionSelected, this.selected, this.actionToAll, this.actionFormData || {}).then(e => {
+                    this.actionLoading = !1, b6e(this.viewname, this.actionSelected, this.selected, this.actionToAll, this.actionFormData || {}).then(e => {
                         this.actionDialogConfirmation = !1, this.actionFormDialogOpen = !1, this.actionLoading = !1, this.getListData()
                     }).catch(e => {
                         this.actionLoading = !1, e.data && this.$refs.fieldscontainer.updateErrors(e.data)
                     })
                 }
             }
         },
-        _6e = {
+        w6e = {
             class: "list-page"
         },
-        w6e = {
+        S6e = {
             class: "list-above-block"
         },
-        S6e = {
+        k6e = {
             class: "header-row-filters"
         },
-        k6e = {
+        $6e = {
             class: "header-row-actions"
         },
-        $6e = ["onClick"],
-        C6e = {
+        C6e = ["onClick"],
+        T6e = {
             key: 4,
             class: "cell-string"
         },
-        T6e = {
+        P6e = {
             key: 6,
             class: "cell-string"
         },
-        P6e = {
+        E6e = {
             class: "table-bottom"
         },
-        E6e = {
+        x6e = {
             key: 0,
             class: "table-bottom-cell"
         },
-        x6e = {
+        O6e = {
             class: "selected-count"
         },
-        O6e = {
+        A6e = {
             class: "table-bottom-cell actions-cell"
         },
-        A6e = {
+        M6e = {
             class: "table-bottom-cell"
         },
-        M6e = {
+        D6e = {
             class: "selected-count"
         };
 
-    function D6e(e, t, n, r, a, i) {
+    function I6e(e, t, n, r, a, i) {
         const s = ow,
             o = oY,
             u = eA;
-        return ce(), Oe("div", _6e, [mt("div", w6e, [mt("div", S6e, [T(s, {
+        return ce(), Oe("div", w6e, [mt("div", S6e, [mt("div", k6e, [T(s, {
             "filterset-fields": n.apiInfo[n.viewname].meta.filterset_fields,
             "search-fields": n.apiInfo[n.viewname].meta.search_fields,
             "filter-info-init": a.filterInfo,
             settings: n.settings,
             onFiltered: i.handleFilter
-        }, null, 8, ["filterset-fields", "search-fields", "filter-info-init", "settings", "onFiltered"])]), mt("div", k6e, [i.canAdd() ? (ce(), Le(o, {
+        }, null, 8, ["filterset-fields", "search-fields", "filter-info-init", "settings", "onFiltered"])]), mt("div", $6e, [i.canAdd() ? (ce(), Le(o, {
             key: 0,
             "api-info": n.apiInfo,
             viewname: n.viewname,
             "relation-name-filter": n.relationNameFilter,
             "filter-id": n.filterId
         }, null, 8, ["api-info", "viewname", "relation-name-filter", "filter-id"])) : Ve("", !0)])]), T(M4, {
             class: "model-table",
@@ -74654,15 +74662,15 @@
             items: a.pageData.data || [],
             headers: a.headers,
             loading: a.listLoading,
             "show-select": !0,
             "items-per-page": a.pageInfo.limit,
             page: a.pageInfo.page,
             "onUpdate:sortBy": i.updateSortBy
-        }, si({
+        }, oi({
             bottom: fe(() => []),
             "header.data-table-select": fe(({
                 on: c,
                 props: f
             }) => [T(Yd, {
                 text: e.$t("applyToAllRecords")
             }, {
@@ -74734,40 +74742,40 @@
                 size: "small",
                 color: c.field.tag_style[h[c.key].value]
             }, {
                 default: fe(() => [ct(vt(h[c.key].text), 1)]),
                 _: 2
             }, 1032, ["color"])) : (ce(), Oe(Ne, {
                 key: 1
-            }, [ct(vt(h[c.key].text), 1)], 64))], 64)) : Ve("", !0)], 64)) : c.field.type === "datetime" ? (ce(), Oe("span", C6e, vt(i.formatDateTime(h[c.key])), 1)) : c.field.type === "image upload" && c.field.list_preview ? (ce(), Oe(Ne, {
+            }, [ct(vt(h[c.key].text), 1)], 64))], 64)) : Ve("", !0)], 64)) : c.field.type === "datetime" ? (ce(), Oe("span", T6e, vt(i.formatDateTime(h[c.key])), 1)) : c.field.type === "image upload" && c.field.list_preview ? (ce(), Oe(Ne, {
                 key: 5
             }, [h[c.key] && h[c.key].url ? (ce(), Le(vp, {
                 key: 0,
                 class: "image-preview",
                 width: "100",
                 "max-height": "100",
                 cover: "",
                 src: h[c.key].url
-            }, null, 8, ["src"])) : Ve("", !0)], 64)) : (ce(), Oe("span", T6e, vt(h[c.key]), 1))], 10, $6e)])
-        }))]), 1032, ["modelValue", "items", "headers", "loading", "items-per-page", "page", "onUpdate:sortBy"]), mt("div", P6e, [i.hasActons() ? (ce(), Oe("div", E6e, [T(wo, {
+            }, null, 8, ["src"])) : Ve("", !0)], 64)) : (ce(), Oe("span", P6e, vt(h[c.key]), 1))], 10, C6e)])
+        }))]), 1032, ["modelValue", "items", "headers", "loading", "items-per-page", "page", "onUpdate:sortBy"]), mt("div", E6e, [i.hasActons() ? (ce(), Oe("div", x6e, [T(wo, {
             class: "info"
         }, {
-            default: fe(() => [ct(vt(e.$t("selected")) + " ", 1), mt("p", x6e, vt(i.getSelectedCount()) + "/" + vt(i.getTotalCount()), 1)]),
+            default: fe(() => [ct(vt(e.$t("selected")) + " ", 1), mt("p", O6e, vt(i.getSelectedCount()) + "/" + vt(i.getTotalCount()), 1)]),
             _: 1
-        })])) : Ve("", !0), mt("div", O6e, [(ce(!0), Oe(Ne, null, Et(this.sectionData.meta.actions, (c, f) => (ce(), Le(dn, {
+        })])) : Ve("", !0), mt("div", A6e, [(ce(!0), Oe(Ne, null, Et(this.sectionData.meta.actions, (c, f) => (ce(), Le(dn, {
             size: "small",
             class: "action-button",
             variant: c.variant || "flat",
             "prepend-icon": c.icon,
             "base-color": c.base_color || "var(--color-light-3)",
             onClick: h => i.pressAction(c, f)
         }, {
             default: fe(() => [ct(vt(c.name), 1)]),
             _: 2
-        }, 1032, ["variant", "prepend-icon", "base-color", "onClick"]))), 256))]), mt("div", A6e, [T(Yd, {
+        }, 1032, ["variant", "prepend-icon", "base-color", "onClick"]))), 256))]), mt("div", M6e, [T(Yd, {
             location: "start",
             text: e.$t("itemsPerPage")
         }, {
             activator: fe(({
                 props: c
             }) => [mt("div", hr(ea(c)), [T(Pl, {
                 class: "list-pagination-per-page",
@@ -74804,15 +74812,15 @@
                         onClick: t[4] || (t[4] = c => a.actionDialogConfirmation = !1)
                     })]),
                     _: 1
                 }), T(Sl, null, {
                     default: fe(() => [mt("p", null, vt(i.getActionInfo().confirmation_text), 1), T(wo, {
                         class: "info"
                     }, {
-                        default: fe(() => [ct(vt(e.$t("selected")) + " ", 1), mt("p", M6e, vt(i.getSelectedCount()) + "/" + vt(i.getTotalCount()), 1)]),
+                        default: fe(() => [ct(vt(e.$t("selected")) + " ", 1), mt("p", D6e, vt(i.getSelectedCount()) + "/" + vt(i.getTotalCount()), 1)]),
                         _: 1
                     })]),
                     _: 1
                 }), T(ef, null, {
                     default: fe(() => [T(fu), T(dn, {
                         text: e.$t("cancel"),
                         variant: "elevated",
@@ -74866,29 +74874,29 @@
                     _: 1
                 })]),
                 _: 1
             })]),
             _: 1
         }, 8, ["modelValue"])])
     }
-    const lY = xr(b6e, [
-        ["render", D6e]
+    const lY = xr(_6e, [
+        ["render", I6e]
     ]);
 
-    function I6e(e, t, n) {
+    function L6e(e, t, n) {
         return new Promise((r, a) => {
             yu({
                 url: e,
                 method: t
             }).then(i => {
                 r(i)
             }).catch(i => a(i))
         })
     }
-    const L6e = {
+    const R6e = {
             props: {
                 apiInfo: {
                     type: Object,
                     required: !0
                 },
                 viewname: {
                     type: String,
@@ -74914,15 +74922,15 @@
             async created() {
                 this.apiMethods = G_(this.viewname, this.apiInfo), this.retrieveData()
             },
             methods: {
                 retrieveData() {
                     this.loading = !0;
                     const e = this.apiMethods.retrieve;
-                    e || console.error(`${this.viewname} apiMethods is not contain retrieve method`), I6e(e.url.replace("{id}", this.id), e.methodHttp, this.sectionData).then(t => {
+                    e || console.error(`${this.viewname} apiMethods is not contain retrieve method`), L6e(e.url.replace("{id}", this.id), e.methodHttp, this.sectionData).then(t => {
                         this.loading = !1, this.formData = t.data, this.$refs.fieldscontainer.updateFormData(t.data)
                     }).catch(t => {
                         this.loading = !1, t.response && t.response.status === 404 && this.$router.push({
                             path: "/404"
                         }), console.error("Get detail error:", t), tn(t, {
                             theme: "auto",
                             type: "error",
@@ -74958,36 +74966,36 @@
                             type: "error",
                             position: "top-center"
                         })
                     })
                 }
             }
         },
-        R6e = {
+        N6e = {
             class: "model-form-bottom-actions"
         };
 
-    function N6e(e, t, n, r, a, i) {
+    function F6e(e, t, n, r, a, i) {
         const s = eA;
         return ce(), Oe("div", null, [T(s, {
             ref: "fieldscontainer",
             formType: "edit",
             "api-info": n.apiInfo,
             viewname: n.viewname,
             loading: a.loading,
             onChanged: t[0] || (t[0] = o => a.formData = o)
-        }, null, 8, ["api-info", "viewname", "loading"]), mt("div", R6e, [T(dn, {
+        }, null, 8, ["api-info", "viewname", "loading"]), mt("div", N6e, [T(dn, {
             text: e.$t("update"),
             variant: "tonal",
             color: "primary",
             onClick: i.updateModel
         }, null, 8, ["text", "onClick"])])])
     }
-    const uY = xr(L6e, [
-        ["render", N6e]
+    const uY = xr(R6e, [
+        ["render", F6e]
     ]);
     /*!
      * @kurkle/color v0.3.2
      * https://github.com/kurkle/color#readme
      * (c) 2023 Jukka Kurkela
      * Released under the MIT License
      */
@@ -75032,118 +75040,118 @@
             b: 11,
             c: 12,
             d: 13,
             e: 14,
             f: 15
         },
         FC = [..."0123456789ABCDEF"],
-        F6e = e => FC[e & 15],
-        V6e = e => FC[(e & 240) >> 4] + FC[e & 15],
+        V6e = e => FC[e & 15],
+        j6e = e => FC[(e & 240) >> 4] + FC[e & 15],
         o0 = e => (e & 240) >> 4 === (e & 15),
-        j6e = e => o0(e.r) && o0(e.g) && o0(e.b) && o0(e.a);
+        B6e = e => o0(e.r) && o0(e.g) && o0(e.b) && o0(e.a);
 
-    function B6e(e) {
+    function H6e(e) {
         var t = e.length,
             n;
         return e[0] === "#" && (t === 4 || t === 5 ? n = {
             r: 255 & Ls[e[1]] * 17,
             g: 255 & Ls[e[2]] * 17,
             b: 255 & Ls[e[3]] * 17,
             a: t === 5 ? Ls[e[4]] * 17 : 255
         } : (t === 7 || t === 9) && (n = {
             r: Ls[e[1]] << 4 | Ls[e[2]],
             g: Ls[e[3]] << 4 | Ls[e[4]],
             b: Ls[e[5]] << 4 | Ls[e[6]],
             a: t === 9 ? Ls[e[7]] << 4 | Ls[e[8]] : 255
         })), n
     }
-    const H6e = (e, t) => e < 255 ? t(e) : "";
+    const W6e = (e, t) => e < 255 ? t(e) : "";
 
-    function W6e(e) {
-        var t = j6e(e) ? F6e : V6e;
-        return e ? "#" + t(e.r) + t(e.g) + t(e.b) + H6e(e.a, t) : void 0
+    function U6e(e) {
+        var t = B6e(e) ? V6e : j6e;
+        return e ? "#" + t(e.r) + t(e.g) + t(e.b) + W6e(e.a, t) : void 0
     }
-    const U6e = /^(hsla?|hwb|hsv)\(\s*([-+.e\d]+)(?:deg)?[\s,]+([-+.e\d]+)%[\s,]+([-+.e\d]+)%(?:[\s,]+([-+.e\d]+)(%)?)?\s*\)$/;
+    const z6e = /^(hsla?|hwb|hsv)\(\s*([-+.e\d]+)(?:deg)?[\s,]+([-+.e\d]+)%[\s,]+([-+.e\d]+)%(?:[\s,]+([-+.e\d]+)(%)?)?\s*\)$/;
 
     function cY(e, t, n) {
         const r = t * Math.min(n, 1 - n),
             a = (i, s = (i + e / 30) % 12) => n - r * Math.max(Math.min(s - 3, 9 - s, 1), -1);
         return [a(0), a(8), a(4)]
     }
 
-    function z6e(e, t, n) {
+    function Y6e(e, t, n) {
         const r = (a, i = (a + e / 60) % 6) => n - n * t * Math.max(Math.min(i, 4 - i, 1), 0);
         return [r(5), r(3), r(1)]
     }
 
-    function Y6e(e, t, n) {
+    function q6e(e, t, n) {
         const r = cY(e, 1, .5);
         let a;
         for (t + n > 1 && (a = 1 / (t + n), t *= a, n *= a), a = 0; a < 3; a++) r[a] *= 1 - t - n, r[a] += t;
         return r
     }
 
-    function q6e(e, t, n, r, a) {
+    function G6e(e, t, n, r, a) {
         return e === a ? (t - n) / r + (t < n ? 6 : 0) : t === a ? (n - e) / r + 2 : (e - t) / r + 4
     }
 
     function nA(e) {
         const n = e.r / 255,
             r = e.g / 255,
             a = e.b / 255,
             i = Math.max(n, r, a),
             s = Math.min(n, r, a),
             o = (i + s) / 2;
         let u, c, f;
-        return i !== s && (f = i - s, c = o > .5 ? f / (2 - i - s) : f / (i + s), u = q6e(n, r, a, f, i), u = u * 60 + .5), [u | 0, c || 0, o]
+        return i !== s && (f = i - s, c = o > .5 ? f / (2 - i - s) : f / (i + s), u = G6e(n, r, a, f, i), u = u * 60 + .5), [u | 0, c || 0, o]
     }
 
     function rA(e, t, n, r) {
         return (Array.isArray(t) ? e(t[0], t[1], t[2]) : e(t, n, r)).map(_c)
     }
 
     function aA(e, t, n) {
         return rA(cY, e, t, n)
     }
 
-    function G6e(e, t, n) {
-        return rA(Y6e, e, t, n)
+    function K6e(e, t, n) {
+        return rA(q6e, e, t, n)
     }
 
-    function K6e(e, t, n) {
-        return rA(z6e, e, t, n)
+    function X6e(e, t, n) {
+        return rA(Y6e, e, t, n)
     }
 
     function dY(e) {
         return (e % 360 + 360) % 360
     }
 
-    function X6e(e) {
-        const t = U6e.exec(e);
+    function J6e(e) {
+        const t = z6e.exec(e);
         let n = 255,
             r;
         if (!t) return;
         t[5] !== r && (n = t[6] ? jm(+t[5]) : _c(+t[5]));
         const a = dY(+t[2]),
             i = +t[3] / 100,
             s = +t[4] / 100;
-        return t[1] === "hwb" ? r = G6e(a, i, s) : t[1] === "hsv" ? r = K6e(a, i, s) : r = aA(a, i, s), {
+        return t[1] === "hwb" ? r = K6e(a, i, s) : t[1] === "hsv" ? r = X6e(a, i, s) : r = aA(a, i, s), {
             r: r[0],
             g: r[1],
             b: r[2],
             a: n
         }
     }
 
-    function J6e(e, t) {
+    function Z6e(e, t) {
         var n = nA(e);
         n[0] = dY(n[0] + t), n = aA(n), e.r = n[0], e.g = n[1], e.b = n[2]
     }
 
-    function Z6e(e) {
+    function Q6e(e) {
         if (!e) return;
         const t = nA(e),
             n = t[0],
             r = dF(t[1]),
             a = dF(t[2]);
         return e.a < 255 ? `hsla(${n}, ${r}%, ${a}%, ${Gl(e.a)})` : `hsl(${n}, ${r}%, ${a}%)`
     }
@@ -75323,41 +75331,41 @@
             JHt: "f5deb3",
             wEte: "ffffff",
             wEtesmoke: "f5f5f5",
             Lw: "ffff00",
             LwgYF: "9acd32"
         };
 
-    function Q6e() {
+    function e8e() {
         const e = {},
             t = Object.keys(hF),
             n = Object.keys(fF);
         let r, a, i, s, o;
         for (r = 0; r < t.length; r++) {
             for (s = o = t[r], a = 0; a < n.length; a++) i = n[a], o = o.replace(i, fF[i]);
             i = parseInt(hF[s], 16), e[o] = [i >> 16 & 255, i >> 8 & 255, i & 255]
         }
         return e
     }
     let l0;
 
-    function e8e(e) {
-        l0 || (l0 = Q6e(), l0.transparent = [0, 0, 0, 0]);
+    function t8e(e) {
+        l0 || (l0 = e8e(), l0.transparent = [0, 0, 0, 0]);
         const t = l0[e.toLowerCase()];
         return t && {
             r: t[0],
             g: t[1],
             b: t[2],
             a: t.length === 4 ? t[3] : 255
         }
     }
-    const t8e = /^rgba?\(\s*([-+.\d]+)(%)?[\s,]+([-+.e\d]+)(%)?[\s,]+([-+.e\d]+)(%)?(?:[\s,/]+([-+.e\d]+)(%)?)?\s*\)$/;
+    const n8e = /^rgba?\(\s*([-+.\d]+)(%)?[\s,]+([-+.e\d]+)(%)?[\s,]+([-+.e\d]+)(%)?(?:[\s,/]+([-+.e\d]+)(%)?)?\s*\)$/;
 
-    function n8e(e) {
-        const t = t8e.exec(e);
+    function r8e(e) {
+        const t = n8e.exec(e);
         let n = 255,
             r, a, i;
         if (t) {
             if (t[7] !== r) {
                 const s = +t[7];
                 n = t[8] ? jm(s) : oc(s * 255, 0, 255)
             }
@@ -75366,21 +75374,21 @@
                 g: a,
                 b: i,
                 a: n
             }
         }
     }
 
-    function r8e(e) {
+    function a8e(e) {
         return e && (e.a < 255 ? `rgba(${e.r}, ${e.g}, ${e.b}, ${Gl(e.a)})` : `rgb(${e.r}, ${e.g}, ${e.b})`)
     }
     const Ek = e => e <= .0031308 ? e * 12.92 : Math.pow(e, 1 / 2.4) * 1.055 - .055,
         rh = e => e <= .04045 ? e / 12.92 : Math.pow((e + .055) / 1.055, 2.4);
 
-    function a8e(e, t, n) {
+    function i8e(e, t, n) {
         const r = rh(Gl(e.r)),
             a = rh(Gl(e.g)),
             i = rh(Gl(e.b));
         return {
             r: _c(Ek(r + n * (rh(Gl(t.r)) - r))),
             g: _c(Ek(a + n * (rh(Gl(t.g)) - a))),
             b: _c(Ek(i + n * (rh(Gl(t.b)) - i))),
@@ -75415,42 +75423,42 @@
             r: 0,
             g: 0,
             b: 0,
             a: 1
         }), t.a = _c(t.a)), t
     }
 
-    function i8e(e) {
-        return e.charAt(0) === "r" ? n8e(e) : X6e(e)
+    function s8e(e) {
+        return e.charAt(0) === "r" ? r8e(e) : J6e(e)
     }
     class Jv {
         constructor(t) {
             if (t instanceof Jv) return t;
             const n = typeof t;
             let r;
-            n === "object" ? r = pF(t) : n === "string" && (r = B6e(t) || e8e(t) || i8e(t)), this._rgb = r, this._valid = !!r
+            n === "object" ? r = pF(t) : n === "string" && (r = H6e(t) || t8e(t) || s8e(t)), this._rgb = r, this._valid = !!r
         }
         get valid() {
             return this._valid
         }
         get rgb() {
             var t = fY(this._rgb);
             return t && (t.a = Gl(t.a)), t
         }
         set rgb(t) {
             this._rgb = pF(t)
         }
         rgbString() {
-            return this._valid ? r8e(this._rgb) : void 0
+            return this._valid ? a8e(this._rgb) : void 0
         }
         hexString() {
-            return this._valid ? W6e(this._rgb) : void 0
+            return this._valid ? U6e(this._rgb) : void 0
         }
         hslString() {
-            return this._valid ? Z6e(this._rgb) : void 0
+            return this._valid ? Q6e(this._rgb) : void 0
         }
         mix(t, n) {
             if (t) {
                 const r = this.rgb,
                     a = t.rgb;
                 let i;
                 const s = n === i ? .5 : n,
@@ -75458,15 +75466,15 @@
                     u = r.a - a.a,
                     c = ((o * u === -1 ? o : (o + u) / (1 + o * u)) + 1) / 2;
                 i = 1 - c, r.r = 255 & c * r.r + i * a.r + .5, r.g = 255 & c * r.g + i * a.g + .5, r.b = 255 & c * r.b + i * a.b + .5, r.a = s * r.a + (1 - s) * a.a, this.rgb = r
             }
             return this
         }
         interpolate(t, n) {
-            return t && (this._rgb = a8e(this._rgb, t._rgb, n)), this
+            return t && (this._rgb = i8e(this._rgb, t._rgb, n)), this
         }
         clone() {
             return new Jv(this.rgb)
         }
         alpha(t) {
             return this._rgb.a = _c(t), this
         }
@@ -75496,25 +75504,25 @@
         saturate(t) {
             return u0(this._rgb, 1, t), this
         }
         desaturate(t) {
             return u0(this._rgb, 1, -t), this
         }
         rotate(t) {
-            return J6e(this._rgb, t), this
+            return Z6e(this._rgb, t), this
         }
     }
     /*!
      * Chart.js v4.4.3
      * https://www.chartjs.org
      * (c) 2024 Chart.js Contributors
      * Released under the MIT License
      */
     function Hl() {}
-    const s8e = (() => {
+    const o8e = (() => {
         let e = 0;
         return () => e++
     })();
 
     function Xn(e) {
         return e === null || typeof e > "u"
     }
@@ -75536,15 +75544,15 @@
     function gs(e, t) {
         return ta(e) ? e : t
     }
 
     function un(e, t) {
         return typeof e > "u" ? t : e
     }
-    const o8e = (e, t) => typeof e == "string" && e.endsWith("%") ? parseFloat(e) / 100 : +e / t,
+    const l8e = (e, t) => typeof e == "string" && e.endsWith("%") ? parseFloat(e) / 100 : +e / t,
         hY = (e, t) => typeof e == "string" && e.endsWith("%") ? parseFloat(e) / 100 * t : +e;
 
     function mr(e, t, n) {
         if (e && typeof e.call == "function") return e.apply(n, t)
     }
 
     function ar(e, t, n, r) {
@@ -75576,97 +75584,97 @@
         return e
     }
 
     function pY(e) {
         return ["__proto__", "prototype", "constructor"].indexOf(e) === -1
     }
 
-    function l8e(e, t, n, r) {
+    function u8e(e, t, n, r) {
         if (!pY(e)) return;
         const a = t[e],
             i = n[e];
         Tn(a) && Tn(i) ? Zv(a, i, r) : t[e] = u_(i)
     }
 
     function Zv(e, t, n) {
         const r = Lr(t) ? t : [t],
             a = r.length;
         if (!Tn(e)) return e;
         n = n || {};
-        const i = n.merger || l8e;
+        const i = n.merger || u8e;
         let s;
         for (let o = 0; o < a; ++o) {
             if (s = r[o], !Tn(s)) continue;
             const u = Object.keys(s);
             for (let c = 0, f = u.length; c < f; ++c) i(u[c], e, s, n)
         }
         return e
     }
 
     function fv(e, t) {
         return Zv(e, t, {
-            merger: u8e
+            merger: c8e
         })
     }
 
-    function u8e(e, t, n) {
+    function c8e(e, t, n) {
         if (!pY(e)) return;
         const r = t[e],
             a = n[e];
         Tn(r) && Tn(a) ? fv(r, a) : Object.prototype.hasOwnProperty.call(t, e) || (t[e] = u_(a))
     }
     const mF = {
         "": e => e,
         x: e => e.x,
         y: e => e.y
     };
 
-    function c8e(e) {
+    function d8e(e) {
         const t = e.split("."),
             n = [];
         let r = "";
         for (const a of t) r += a, r.endsWith("\\") ? r = r.slice(0, -1) + "." : (n.push(r), r = "");
         return n
     }
 
-    function d8e(e) {
-        const t = c8e(e);
+    function f8e(e) {
+        const t = d8e(e);
         return n => {
             for (const r of t) {
                 if (r === "") break;
                 n = n && n[r]
             }
             return n
         }
     }
 
     function Oc(e, t) {
-        return (mF[t] || (mF[t] = d8e(t)))(e)
+        return (mF[t] || (mF[t] = f8e(t)))(e)
     }
 
     function iA(e) {
         return e.charAt(0).toUpperCase() + e.slice(1)
     }
     const Qv = e => typeof e < "u",
         Ac = e => typeof e == "function",
         vF = (e, t) => {
             if (e.size !== t.size) return !1;
             for (const n of e)
                 if (!t.has(n)) return !1;
             return !0
         };
 
-    function f8e(e) {
+    function h8e(e) {
         return e.type === "mouseup" || e.type === "click" || e.type === "contextmenu"
     }
     const Wr = Math.PI,
         Ya = 2 * Wr,
-        h8e = Ya + Wr,
+        p8e = Ya + Wr,
         c_ = Number.POSITIVE_INFINITY,
-        p8e = Wr / 180,
+        m8e = Wr / 180,
         Bi = Wr / 2,
         gd = Wr / 4,
         gF = Wr * 2 / 3,
         lc = Math.log10,
         hl = Math.sign;
 
     function hv(e, t, n) {
@@ -75677,27 +75685,27 @@
         const t = Math.round(e);
         e = hv(e, t, e / 1e3) ? t : e;
         const n = Math.pow(10, Math.floor(lc(e))),
             r = e / n;
         return (r <= 1 ? 1 : r <= 2 ? 2 : r <= 5 ? 5 : 10) * n
     }
 
-    function m8e(e) {
+    function v8e(e) {
         const t = [],
             n = Math.sqrt(e);
         let r;
         for (r = 1; r < n; r++) e % r === 0 && (t.push(r), t.push(e / r));
         return n === (n | 0) && t.push(n), t.sort((a, i) => a - i).pop(), t
     }
 
     function sp(e) {
         return !isNaN(parseFloat(e)) && isFinite(e)
     }
 
-    function v8e(e, t) {
+    function g8e(e, t) {
         const n = Math.round(e);
         return n - t <= e && n + t >= e
     }
 
     function mY(e, t, n) {
         let r, a, i;
         for (r = 0, a = e.length; r < a; r++) i = e[r][n], isNaN(i) || (t.min = Math.min(t.min, i), t.max = Math.max(t.max, i))
@@ -75715,31 +75723,31 @@
         if (!ta(e)) return;
         let t = 1,
             n = 0;
         for (; Math.round(e * t) / t !== e;) t *= 10, n++;
         return n
     }
 
-    function g8e(e, t) {
+    function y8e(e, t) {
         const n = t.x - e.x,
             r = t.y - e.y,
             a = Math.sqrt(n * n + r * r);
         let i = Math.atan2(r, n);
         return i < -.5 * Wr && (i += Ya), {
             angle: i,
             distance: a
         }
     }
 
     function VC(e, t) {
         return Math.sqrt(Math.pow(t.x - e.x, 2) + Math.pow(t.y - e.y, 2))
     }
 
-    function y8e(e, t) {
-        return (e - t + h8e) % Ya - Wr
+    function b8e(e, t) {
+        return (e - t + p8e) % Ya - Wr
     }
 
     function bs(e) {
         return (e % Ya + Ya) % Ya
     }
 
     function d_(e, t, n, r) {
@@ -75753,15 +75761,15 @@
         return a === i || a === s || r && i === s || o > u && c < f
     }
 
     function ks(e, t, n) {
         return Math.max(t, Math.min(n, e))
     }
 
-    function b8e(e) {
+    function _8e(e) {
         return ks(e, -32768, 32767)
     }
 
     function uc(e, t, n, r = 1e-6) {
         return e >= Math.min(t, n) - r && e <= Math.max(t, n) + r
     }
 
@@ -75776,26 +75784,26 @@
             hi: r
         }
     }
     const Vd = (e, t, n, r) => oA(e, n, r ? a => {
             const i = e[a][t];
             return i < n || i === n && e[a + 1][t] === n
         } : a => e[a][t] < n),
-        _8e = (e, t, n) => oA(e, n, r => e[r][t] >= n);
+        w8e = (e, t, n) => oA(e, n, r => e[r][t] >= n);
 
-    function w8e(e, t, n) {
+    function S8e(e, t, n) {
         let r = 0,
             a = e.length;
         for (; r < a && e[r] < t;) r++;
         for (; a > r && e[a - 1] > n;) a--;
         return r > 0 || a < e.length ? e.slice(r, a) : e
     }
     const vY = ["push", "pop", "shift", "splice", "unshift"];
 
-    function S8e(e, t) {
+    function k8e(e, t) {
         if (e._chartjs) {
             e._chartjs.listeners.push(t);
             return
         }
         Object.defineProperty(e, "_chartjs", {
             configurable: !0,
             enumerable: !1,
@@ -75844,23 +75852,23 @@
         return function(...a) {
             n = a, r || (r = !0, yY.call(window, () => {
                 r = !1, e.apply(t, n)
             }))
         }
     }
 
-    function k8e(e, t) {
+    function $8e(e, t) {
         let n;
         return function(...r) {
             return t ? (clearTimeout(n), n = setTimeout(e, t, r)) : e.apply(this, r), t
         }
     }
     const lA = e => e === "start" ? "left" : e === "end" ? "right" : "center",
         yi = (e, t, n) => e === "start" ? t : e === "end" ? n : (t + n) / 2,
-        $8e = (e, t, n, r) => e === (r ? "left" : "right") ? n : e === "center" ? (t + n) / 2 : t;
+        C8e = (e, t, n, r) => e === (r ? "left" : "right") ? n : e === "center" ? (t + n) / 2 : t;
 
     function _Y(e, t, n) {
         const r = t.length;
         let a = 0,
             i = r;
         if (e._sorted) {
             const {
@@ -75954,18 +75962,18 @@
     function kF(e) {
         return uA(e) ? e : new Jv(e)
     }
 
     function xk(e) {
         return uA(e) ? e : new Jv(e).saturate(.5).darken(.1).hexString()
     }
-    const C8e = ["x", "y", "borderWidth", "radius", "tension"],
-        T8e = ["color", "borderColor", "backgroundColor"];
+    const T8e = ["x", "y", "borderWidth", "radius", "tension"],
+        P8e = ["color", "borderColor", "backgroundColor"];
 
-    function P8e(e) {
+    function E8e(e) {
         e.set("animation", {
             delay: void 0,
             duration: 1e3,
             easing: "easeOutQuart",
             fn: void 0,
             from: void 0,
             loop: void 0,
@@ -75974,19 +75982,19 @@
         }), e.describe("animation", {
             _fallback: !1,
             _indexable: !1,
             _scriptable: t => t !== "onProgress" && t !== "onComplete" && t !== "fn"
         }), e.set("animations", {
             colors: {
                 type: "color",
-                properties: T8e
+                properties: P8e
             },
             numbers: {
                 type: "number",
-                properties: C8e
+                properties: T8e
             }
         }), e.describe("animations", {
             _fallback: "animation"
         }), e.set("transitions", {
             active: {
                 animation: {
                     duration: 400
@@ -76019,48 +76027,48 @@
                         fn: t => t | 0
                     }
                 }
             }
         })
     }
 
-    function E8e(e) {
+    function x8e(e) {
         e.set("layout", {
             autoPadding: !0,
             padding: {
                 top: 0,
                 right: 0,
                 bottom: 0,
                 left: 0
             }
         })
     }
     const $F = new Map;
 
-    function x8e(e, t) {
+    function O8e(e, t) {
         t = t || {};
         const n = e + JSON.stringify(t);
         let r = $F.get(n);
         return r || (r = new Intl.NumberFormat(e, t), $F.set(n, r)), r
     }
 
     function Kg(e, t, n) {
-        return x8e(t, n).format(e)
+        return O8e(t, n).format(e)
     }
     const SY = {
         values(e) {
             return Lr(e) ? e : "" + e
         },
         numeric(e, t, n) {
             if (e === 0) return "0";
             const r = this.chart.options.locale;
             let a, i = e;
             if (n.length > 1) {
                 const c = Math.max(Math.abs(n[0].value), Math.abs(n[n.length - 1].value));
-                (c < 1e-4 || c > 1e15) && (a = "scientific"), i = O8e(e, n)
+                (c < 1e-4 || c > 1e15) && (a = "scientific"), i = A8e(e, n)
             }
             const s = lc(Math.abs(i)),
                 o = isNaN(s) ? 1 : Math.max(Math.min(-1 * Math.floor(s), 20), 0),
                 u = {
                     notation: a,
                     minimumFractionDigits: o,
                     maximumFractionDigits: o
@@ -76070,23 +76078,23 @@
         logarithmic(e, t, n) {
             if (e === 0) return "0";
             const r = n[t].significand || e / Math.pow(10, Math.floor(lc(e)));
             return [1, 2, 3, 5, 10, 15].includes(r) || t > .8 * n.length ? SY.numeric.call(this, e, t, n) : ""
         }
     };
 
-    function O8e(e, t) {
+    function A8e(e, t) {
         let n = t.length > 3 ? t[2].value - t[1].value : t[1].value - t[0].value;
         return Math.abs(n) >= 1 && e !== Math.floor(e) && (n = e - Math.floor(e)), n
     }
     var lw = {
         formatters: SY
     };
 
-    function A8e(e) {
+    function M8e(e) {
         e.set("scale", {
             display: !0,
             offset: !1,
             reverse: !1,
             beginAtZero: !1,
             bounds: "ticks",
             clip: !0,
@@ -76158,15 +76166,15 @@
         }
         return e
     }
 
     function Ok(e, t, n) {
         return typeof t == "string" ? Zv(mv(e, t), n) : Zv(mv(e, ""), t)
     }
-    class M8e {
+    class D8e {
         constructor(t, n) {
             this.animation = void 0, this.backgroundColor = "rgba(0,0,0,0.1)", this.borderColor = "rgba(0,0,0,0.1)", this.color = "#666", this.datasets = {}, this.devicePixelRatio = r => r.chart.platform.getDevicePixelRatio(), this.elements = {}, this.events = ["mousemove", "mouseout", "click", "touchstart", "touchmove"], this.font = {
                 family: "'Helvetica Neue', 'Helvetica', 'Arial', sans-serif",
                 size: 12,
                 style: "normal",
                 lineHeight: 1.2,
                 weight: null
@@ -76210,36 +76218,36 @@
                 }
             })
         }
         apply(t) {
             t.forEach(n => n(this))
         }
     }
-    var na = new M8e({
+    var na = new D8e({
         _scriptable: e => !e.startsWith("on"),
         _indexable: e => e !== "events",
         hover: {
             _fallback: "interaction"
         },
         interaction: {
             _scriptable: !1,
             _indexable: !1
         }
-    }, [P8e, E8e, A8e]);
+    }, [E8e, x8e, M8e]);
 
-    function D8e(e) {
+    function I8e(e) {
         return !e || Xn(e.size) || Xn(e.family) ? null : (e.style ? e.style + " " : "") + (e.weight ? e.weight + " " : "") + e.size + "px " + e.family
     }
 
     function f_(e, t, n, r, a) {
         let i = t[a];
         return i || (i = t[a] = e.measureText(a).width, n.push(a)), i > r && (r = i), r
     }
 
-    function I8e(e, t, n, r) {
+    function L8e(e, t, n, r) {
         r = r || {};
         let a = r.data = r.data || {},
             i = r.garbageCollect = r.garbageCollect || [];
         r.font !== t && (a = r.data = {}, i = r.garbageCollect = [], r.font = t), e.save(), e.font = t;
         let s = 0;
         const o = n.length;
         let u, c, f, h, p;
@@ -76271,15 +76279,15 @@
     }
 
     function kY(e, t, n, r, a) {
         let i, s, o, u, c, f, h, p;
         const g = t.pointStyle,
             _ = t.rotation,
             y = t.radius;
-        let w = (_ || 0) * p8e;
+        let w = (_ || 0) * m8e;
         if (g && typeof g == "object" && (i = g.toString(), i === "[object HTMLImageElement]" || i === "[object HTMLCanvasElement]")) {
             e.save(), e.translate(n, r), e.rotate(w), e.drawImage(g, -g.width / 2, -g.height / 2, g.width, g.height), e.restore();
             return
         }
         if (!(isNaN(y) || y <= 0)) {
             switch (e.beginPath(), g) {
                 default:
@@ -76330,90 +76338,90 @@
         e.save(), e.beginPath(), e.rect(t.left, t.top, t.right - t.left, t.bottom - t.top), e.clip()
     }
 
     function cw(e) {
         e.restore()
     }
 
-    function L8e(e, t, n, r, a) {
+    function R8e(e, t, n, r, a) {
         if (!t) return e.lineTo(n.x, n.y);
         if (a === "middle") {
             const i = (t.x + n.x) / 2;
             e.lineTo(i, t.y), e.lineTo(i, n.y)
         } else a === "after" != !!r ? e.lineTo(t.x, n.y) : e.lineTo(n.x, t.y);
         e.lineTo(n.x, n.y)
     }
 
-    function R8e(e, t, n, r) {
+    function N8e(e, t, n, r) {
         if (!t) return e.lineTo(n.x, n.y);
         e.bezierCurveTo(r ? t.cp1x : t.cp2x, r ? t.cp1y : t.cp2y, r ? n.cp2x : n.cp1x, r ? n.cp2y : n.cp1y, n.x, n.y)
     }
 
-    function N8e(e, t) {
+    function F8e(e, t) {
         t.translation && e.translate(t.translation[0], t.translation[1]), Xn(t.rotation) || e.rotate(t.rotation), t.color && (e.fillStyle = t.color), t.textAlign && (e.textAlign = t.textAlign), t.textBaseline && (e.textBaseline = t.textBaseline)
     }
 
-    function F8e(e, t, n, r, a) {
+    function V8e(e, t, n, r, a) {
         if (a.strikethrough || a.underline) {
             const i = e.measureText(r),
                 s = t - i.actualBoundingBoxLeft,
                 o = t + i.actualBoundingBoxRight,
                 u = n - i.actualBoundingBoxAscent,
                 c = n + i.actualBoundingBoxDescent,
                 f = a.strikethrough ? (u + c) / 2 : c;
             e.strokeStyle = e.fillStyle, e.beginPath(), e.lineWidth = a.decorationWidth || 2, e.moveTo(s, f), e.lineTo(o, f), e.stroke()
         }
     }
 
-    function V8e(e, t) {
+    function j8e(e, t) {
         const n = e.fillStyle;
         e.fillStyle = t.color, e.fillRect(t.left, t.top, t.width, t.height), e.fillStyle = n
     }
 
     function cf(e, t, n, r, a, i = {}) {
         const s = Lr(t) ? t : [t],
             o = i.strokeWidth > 0 && i.strokeColor !== "";
         let u, c;
-        for (e.save(), e.font = a.string, N8e(e, i), u = 0; u < s.length; ++u) c = s[u], i.backdrop && V8e(e, i.backdrop), o && (i.strokeColor && (e.strokeStyle = i.strokeColor), Xn(i.strokeWidth) || (e.lineWidth = i.strokeWidth), e.strokeText(c, n, r, i.maxWidth)), e.fillText(c, n, r, i.maxWidth), F8e(e, n, r, c, i), r += Number(a.lineHeight);
+        for (e.save(), e.font = a.string, F8e(e, i), u = 0; u < s.length; ++u) c = s[u], i.backdrop && j8e(e, i.backdrop), o && (i.strokeColor && (e.strokeStyle = i.strokeColor), Xn(i.strokeWidth) || (e.lineWidth = i.strokeWidth), e.strokeText(c, n, r, i.maxWidth)), e.fillText(c, n, r, i.maxWidth), V8e(e, n, r, c, i), r += Number(a.lineHeight);
         e.restore()
     }
 
     function eg(e, t) {
         const {
             x: n,
             y: r,
             w: a,
             h: i,
             radius: s
         } = t;
         e.arc(n + s.topLeft, r + s.topLeft, s.topLeft, 1.5 * Wr, Wr, !0), e.lineTo(n, r + i - s.bottomLeft), e.arc(n + s.bottomLeft, r + i - s.bottomLeft, s.bottomLeft, Wr, Bi, !0), e.lineTo(n + a - s.bottomRight, r + i), e.arc(n + a - s.bottomRight, r + i - s.bottomRight, s.bottomRight, Bi, 0, !0), e.lineTo(n + a, r + s.topRight), e.arc(n + a - s.topRight, r + s.topRight, s.topRight, 0, -Bi, !0), e.lineTo(n + s.topLeft, r)
     }
-    const j8e = /^(normal|(\d+(?:\.\d+)?)(px|em|%)?)$/,
-        B8e = /^(normal|italic|initial|inherit|unset|(oblique( -?[0-9]?[0-9]deg)?))$/;
+    const B8e = /^(normal|(\d+(?:\.\d+)?)(px|em|%)?)$/,
+        H8e = /^(normal|italic|initial|inherit|unset|(oblique( -?[0-9]?[0-9]deg)?))$/;
 
-    function H8e(e, t) {
-        const n = ("" + e).match(j8e);
+    function W8e(e, t) {
+        const n = ("" + e).match(B8e);
         if (!n || n[1] === "normal") return t * 1.2;
         switch (e = +n[2], n[3]) {
             case "px":
                 return e;
             case "%":
                 e /= 100;
                 break
         }
         return t * e
     }
-    const W8e = e => +e || 0;
+    const U8e = e => +e || 0;
 
     function $Y(e, t) {
         const n = {},
             r = Tn(t),
             a = r ? Object.keys(t) : t,
             i = Tn(e) ? r ? s => un(e[s], e[t[s]]) : s => e[s] : () => e;
-        for (const s of a) n[s] = W8e(i(s));
+        for (const s of a) n[s] = U8e(i(s));
         return n
     }
 
     function CY(e) {
         return $Y(e, {
             top: "y",
             right: "x",
@@ -76432,33 +76440,33 @@
     }
 
     function Na(e, t) {
         e = e || {}, t = t || na.font;
         let n = un(e.size, t.size);
         typeof n == "string" && (n = parseInt(n, 10));
         let r = un(e.style, t.style);
-        r && !("" + r).match(B8e) && (console.warn('Invalid font style specified: "' + r + '"'), r = void 0);
+        r && !("" + r).match(H8e) && (console.warn('Invalid font style specified: "' + r + '"'), r = void 0);
         const a = {
             family: un(e.family, t.family),
-            lineHeight: H8e(un(e.lineHeight, t.lineHeight), n),
+            lineHeight: W8e(un(e.lineHeight, t.lineHeight), n),
             size: n,
             style: r,
             weight: un(e.weight, t.weight),
             string: ""
         };
-        return a.string = D8e(a), a
+        return a.string = I8e(a), a
     }
 
     function d0(e, t, n, r) {
         let a, i, s;
         for (a = 0, i = e.length; a < i; ++a)
             if (s = e[a], s !== void 0 && s !== void 0) return s
     }
 
-    function U8e(e, t, n) {
+    function z8e(e, t, n) {
         const {
             min: r,
             max: a
         } = e, i = hY(t, (a - r) / 2), s = (o, u) => n && o === 0 ? 0 : o + u;
         return {
             min: s(r, -Math.abs(i)),
             max: s(a, i)
@@ -76482,15 +76490,15 @@
             override: o => cA([o, ...e], t, i, r)
         };
         return new Proxy(s, {
             deleteProperty(o, u) {
                 return delete o[u], delete o._keys, delete e[0][u], !0
             },
             get(o, u) {
-                return PY(o, u, () => Z8e(u, t, e, o))
+                return PY(o, u, () => Q8e(u, t, e, o))
             },
             getOwnPropertyDescriptor(o, u) {
                 return Reflect.getOwnPropertyDescriptor(o._scopes[0], u)
             },
             getPrototypeOf() {
                 return Reflect.getPrototypeOf(e[0])
             },
@@ -76519,15 +76527,15 @@
             override: i => op(e.override(i), t, n, r)
         };
         return new Proxy(a, {
             deleteProperty(i, s) {
                 return delete i[s], delete e[s], !0
             },
             get(i, s, o) {
-                return PY(i, s, () => Y8e(i, s, o))
+                return PY(i, s, () => q8e(i, s, o))
             },
             getOwnPropertyDescriptor(i, s) {
                 return i._descriptors.allKeys ? Reflect.has(e, s) ? {
                     enumerable: !0,
                     configurable: !0
                 } : void 0 : Reflect.getOwnPropertyDescriptor(e, s)
             },
@@ -76559,48 +76567,48 @@
             allKeys: a,
             scriptable: n,
             indexable: r,
             isScriptable: Ac(n) ? n : () => n,
             isIndexable: Ac(r) ? r : () => r
         }
     }
-    const z8e = (e, t) => e ? e + iA(t) : t,
+    const Y8e = (e, t) => e ? e + iA(t) : t,
         dA = (e, t) => Tn(t) && e !== "adapters" && (Object.getPrototypeOf(t) === null || t.constructor === Object);
 
     function PY(e, t, n) {
         if (Object.prototype.hasOwnProperty.call(e, t) || t === "constructor") return e[t];
         const r = n();
         return e[t] = r, r
     }
 
-    function Y8e(e, t, n) {
+    function q8e(e, t, n) {
         const {
             _proxy: r,
             _context: a,
             _subProxy: i,
             _descriptors: s
         } = e;
         let o = r[t];
-        return Ac(o) && s.isScriptable(t) && (o = q8e(t, o, e, n)), Lr(o) && o.length && (o = G8e(t, o, e, s.isIndexable)), dA(t, o) && (o = op(o, a, i && i[t], s)), o
+        return Ac(o) && s.isScriptable(t) && (o = G8e(t, o, e, n)), Lr(o) && o.length && (o = K8e(t, o, e, s.isIndexable)), dA(t, o) && (o = op(o, a, i && i[t], s)), o
     }
 
-    function q8e(e, t, n, r) {
+    function G8e(e, t, n, r) {
         const {
             _proxy: a,
             _context: i,
             _subProxy: s,
             _stack: o
         } = n;
         if (o.has(e)) throw new Error("Recursion detected: " + Array.from(o).join("->") + "->" + e);
         o.add(e);
         let u = t(i, s || r);
         return o.delete(e), dA(e, u) && (u = fA(a._scopes, a, e, u)), u
     }
 
-    function G8e(e, t, n, r) {
+    function K8e(e, t, n, r) {
         const {
             _proxy: a,
             _context: i,
             _subProxy: s,
             _descriptors: o
         } = n;
         if (typeof i.index < "u" && r(e)) return t[i.index % t.length];
@@ -76615,19 +76623,19 @@
         }
         return t
     }
 
     function EY(e, t, n) {
         return Ac(e) ? e(t, n) : e
     }
-    const K8e = (e, t) => e === !0 ? t : typeof e == "string" ? Oc(t, e) : void 0;
+    const X8e = (e, t) => e === !0 ? t : typeof e == "string" ? Oc(t, e) : void 0;
 
-    function X8e(e, t, n, r, a) {
+    function J8e(e, t, n, r, a) {
         for (const i of t) {
-            const s = K8e(n, i);
+            const s = X8e(n, i);
             if (s) {
                 e.add(s);
                 const o = EY(s._fallback, n, a);
                 if (typeof o < "u" && o !== n && o !== r) return o
             } else if (s === !1 && typeof r < "u" && n !== r) return null
         }
         return !1
@@ -76636,49 +76644,49 @@
     function fA(e, t, n, r) {
         const a = t._rootScopes,
             i = EY(t._fallback, n, r),
             s = [...e, ...a],
             o = new Set;
         o.add(r);
         let u = TF(o, s, n, i || n, r);
-        return u === null || typeof i < "u" && i !== n && (u = TF(o, s, i, u, r), u === null) ? !1 : cA(Array.from(o), [""], a, i, () => J8e(t, n, r))
+        return u === null || typeof i < "u" && i !== n && (u = TF(o, s, i, u, r), u === null) ? !1 : cA(Array.from(o), [""], a, i, () => Z8e(t, n, r))
     }
 
     function TF(e, t, n, r, a) {
-        for (; n;) n = X8e(e, t, n, r, a);
+        for (; n;) n = J8e(e, t, n, r, a);
         return n
     }
 
-    function J8e(e, t, n) {
+    function Z8e(e, t, n) {
         const r = e._getTarget();
         t in r || (r[t] = {});
         const a = r[t];
         return Lr(a) && Tn(n) ? n : a || {}
     }
 
-    function Z8e(e, t, n, r) {
+    function Q8e(e, t, n, r) {
         let a;
         for (const i of t)
-            if (a = xY(z8e(i, e), n), typeof a < "u") return dA(e, a) ? fA(n, r, e, a) : a
+            if (a = xY(Y8e(i, e), n), typeof a < "u") return dA(e, a) ? fA(n, r, e, a) : a
     }
 
     function xY(e, t) {
         for (const n of t) {
             if (!n) continue;
             const r = n[e];
             if (typeof r < "u") return r
         }
     }
 
     function PF(e) {
         let t = e._keys;
-        return t || (t = e._keys = Q8e(e._scopes)), t
+        return t || (t = e._keys = eYe(e._scopes)), t
     }
 
-    function Q8e(e) {
+    function eYe(e) {
         const t = new Set;
         for (const n of e)
             for (const r of Object.keys(n).filter(a => !a.startsWith("_"))) t.add(r);
         return Array.from(t)
     }
 
     function OY(e, t, n, r) {
@@ -76689,19 +76697,19 @@
         } = this._parsing, s = new Array(r);
         let o, u, c, f;
         for (o = 0, u = r; o < u; ++o) c = o + n, f = t[c], s[o] = {
             r: a.parse(Oc(f, i), c)
         };
         return s
     }
-    const eYe = Number.EPSILON || 1e-14,
+    const tYe = Number.EPSILON || 1e-14,
         lp = (e, t) => t < e.length && !e[t].skip && e[t],
         AY = e => e === "x" ? "y" : "x";
 
-    function tYe(e, t, n, r) {
+    function nYe(e, t, n, r) {
         const a = e.skip ? t : e,
             i = t,
             s = n.skip ? t : n,
             o = VC(i, a),
             u = VC(s, i);
         let c = o / (o + u),
             f = u / (o + u);
@@ -76716,72 +76724,72 @@
             next: {
                 x: i.x + p * (s.x - a.x),
                 y: i.y + p * (s.y - a.y)
             }
         }
     }
 
-    function nYe(e, t, n) {
+    function rYe(e, t, n) {
         const r = e.length;
         let a, i, s, o, u, c = lp(e, 0);
         for (let f = 0; f < r - 1; ++f)
             if (u = c, c = lp(e, f + 1), !(!u || !c)) {
-                if (hv(t[f], 0, eYe)) {
+                if (hv(t[f], 0, tYe)) {
                     n[f] = n[f + 1] = 0;
                     continue
                 }
                 a = n[f] / t[f], i = n[f + 1] / t[f], o = Math.pow(a, 2) + Math.pow(i, 2), !(o <= 9) && (s = 3 / Math.sqrt(o), n[f] = a * s * t[f], n[f + 1] = i * s * t[f])
             }
     }
 
-    function rYe(e, t, n = "x") {
+    function aYe(e, t, n = "x") {
         const r = AY(n),
             a = e.length;
         let i, s, o, u = lp(e, 0);
         for (let c = 0; c < a; ++c) {
             if (s = o, o = u, u = lp(e, c + 1), !o) continue;
             const f = o[n],
                 h = o[r];
             s && (i = (f - s[n]) / 3, o[`cp1${n}`] = f - i, o[`cp1${r}`] = h - i * t[c]), u && (i = (u[n] - f) / 3, o[`cp2${n}`] = f + i, o[`cp2${r}`] = h + i * t[c])
         }
     }
 
-    function aYe(e, t = "x") {
+    function iYe(e, t = "x") {
         const n = AY(t),
             r = e.length,
             a = Array(r).fill(0),
             i = Array(r);
         let s, o, u, c = lp(e, 0);
         for (s = 0; s < r; ++s)
             if (o = u, u = c, c = lp(e, s + 1), !!u) {
                 if (c) {
                     const f = c[t] - u[t];
                     a[s] = f !== 0 ? (c[n] - u[n]) / f : 0
                 }
                 i[s] = o ? c ? hl(a[s - 1]) !== hl(a[s]) ? 0 : (a[s - 1] + a[s]) / 2 : a[s - 1] : a[s]
-            } nYe(e, a, i), rYe(e, i, t)
+            } rYe(e, a, i), aYe(e, i, t)
     }
 
     function f0(e, t, n) {
         return Math.max(Math.min(e, n), t)
     }
 
-    function iYe(e, t) {
+    function sYe(e, t) {
         let n, r, a, i, s, o = eu(e[0], t);
         for (n = 0, r = e.length; n < r; ++n) s = i, i = o, o = n < r - 1 && eu(e[n + 1], t), i && (a = e[n], s && (a.cp1x = f0(a.cp1x, t.left, t.right), a.cp1y = f0(a.cp1y, t.top, t.bottom)), o && (a.cp2x = f0(a.cp2x, t.left, t.right), a.cp2y = f0(a.cp2y, t.top, t.bottom)))
     }
 
-    function sYe(e, t, n, r, a) {
+    function oYe(e, t, n, r, a) {
         let i, s, o, u;
-        if (t.spanGaps && (e = e.filter(c => !c.skip)), t.cubicInterpolationMode === "monotone") aYe(e, a);
+        if (t.spanGaps && (e = e.filter(c => !c.skip)), t.cubicInterpolationMode === "monotone") iYe(e, a);
         else {
             let c = r ? e[e.length - 1] : e[0];
-            for (i = 0, s = e.length; i < s; ++i) o = e[i], u = tYe(c, o, e[Math.min(i + 1, s - (r ? 0 : 1)) % s], t.tension), o.cp1x = u.previous.x, o.cp1y = u.previous.y, o.cp2x = u.next.x, o.cp2y = u.next.y, c = o
+            for (i = 0, s = e.length; i < s; ++i) o = e[i], u = nYe(c, o, e[Math.min(i + 1, s - (r ? 0 : 1)) % s], t.tension), o.cp1x = u.previous.x, o.cp1y = u.previous.y, o.cp2x = u.next.x, o.cp2y = u.next.y, c = o
         }
-        t.capBezierPoints && iYe(e, n)
+        t.capBezierPoints && sYe(e, n)
     }
 
     function hA() {
         return typeof window < "u" && typeof document < "u"
     }
 
     function pA(e) {
@@ -76791,40 +76799,40 @@
 
     function h_(e, t, n) {
         let r;
         return typeof e == "string" ? (r = parseInt(e, 10), e.indexOf("%") !== -1 && (r = r / 100 * t.parentNode[n])) : r = e, r
     }
     const dw = e => e.ownerDocument.defaultView.getComputedStyle(e, null);
 
-    function oYe(e, t) {
+    function lYe(e, t) {
         return dw(e).getPropertyValue(t)
     }
-    const lYe = ["top", "right", "bottom", "left"];
+    const uYe = ["top", "right", "bottom", "left"];
 
     function Jd(e, t, n) {
         const r = {};
         n = n ? "-" + n : "";
         for (let a = 0; a < 4; a++) {
-            const i = lYe[a];
+            const i = uYe[a];
             r[i] = parseFloat(e[t + "-" + i + n]) || 0
         }
         return r.width = r.left + r.right, r.height = r.top + r.bottom, r
     }
-    const uYe = (e, t, n) => (e > 0 || t > 0) && (!n || !n.shadowRoot);
+    const cYe = (e, t, n) => (e > 0 || t > 0) && (!n || !n.shadowRoot);
 
-    function cYe(e, t) {
+    function dYe(e, t) {
         const n = e.touches,
             r = n && n.length ? n[0] : e,
             {
                 offsetX: a,
                 offsetY: i
             } = r;
         let s = !1,
             o, u;
-        if (uYe(a, i, e.target)) o = a, u = i;
+        if (cYe(a, i, e.target)) o = a, u = i;
         else {
             const c = t.getBoundingClientRect();
             o = r.clientX - c.left, u = r.clientY - c.top, s = !0
         }
         return {
             x: o,
             y: u,
@@ -76837,26 +76845,26 @@
         const {
             canvas: n,
             currentDevicePixelRatio: r
         } = t, a = dw(n), i = a.boxSizing === "border-box", s = Jd(a, "padding"), o = Jd(a, "border", "width"), {
             x: u,
             y: c,
             box: f
-        } = cYe(e, n), h = s.left + (f && o.left), p = s.top + (f && o.top);
+        } = dYe(e, n), h = s.left + (f && o.left), p = s.top + (f && o.top);
         let {
             width: g,
             height: _
         } = t;
         return i && (g -= s.width + o.width, _ -= s.height + o.height), {
             x: Math.round((u - h) / g * n.width / r),
             y: Math.round((c - p) / _ * n.height / r)
         }
     }
 
-    function dYe(e, t, n) {
+    function fYe(e, t, n) {
         let r, a;
         if (t === void 0 || n === void 0) {
             const i = e && pA(e);
             if (!i) t = e.clientWidth, n = e.clientHeight;
             else {
                 const s = i.getBoundingClientRect(),
                     o = dw(i),
@@ -76870,20 +76878,20 @@
             height: n,
             maxWidth: r || c_,
             maxHeight: a || c_
         }
     }
     const h0 = e => Math.round(e * 10) / 10;
 
-    function fYe(e, t, n, r) {
+    function hYe(e, t, n, r) {
         const a = dw(e),
             i = Jd(a, "margin"),
             s = h_(a.maxWidth, e, "clientWidth") || c_,
             o = h_(a.maxHeight, e, "clientHeight") || c_,
-            u = dYe(e, t, n);
+            u = fYe(e, t, n);
         let {
             width: c,
             height: f
         } = u;
         if (a.boxSizing === "content-box") {
             const p = Jd(a, "border", "width"),
                 g = Jd(a, "padding");
@@ -76899,48 +76907,48 @@
         const r = t || 1,
             a = Math.floor(e.height * r),
             i = Math.floor(e.width * r);
         e.height = Math.floor(e.height), e.width = Math.floor(e.width);
         const s = e.canvas;
         return s.style && (n || !s.style.height && !s.style.width) && (s.style.height = `${e.height}px`, s.style.width = `${e.width}px`), e.currentDevicePixelRatio !== r || s.height !== a || s.width !== i ? (e.currentDevicePixelRatio = r, s.height = a, s.width = i, e.ctx.setTransform(r, 0, 0, r, 0, 0), !0) : !1
     }
-    const hYe = function() {
+    const pYe = function() {
         let e = !1;
         try {
             const t = {
                 get passive() {
                     return e = !0, !1
                 }
             };
             hA() && (window.addEventListener("test", null, t), window.removeEventListener("test", null, t))
         } catch {}
         return e
     }();
 
     function xF(e, t) {
-        const n = oYe(e, t),
+        const n = lYe(e, t),
             r = n && n.match(/^(\d+)(\.\d+)?px$/);
         return r ? +r[1] : void 0
     }
 
     function Cd(e, t, n, r) {
         return {
             x: e.x + n * (t.x - e.x),
             y: e.y + n * (t.y - e.y)
         }
     }
 
-    function pYe(e, t, n, r) {
+    function mYe(e, t, n, r) {
         return {
             x: e.x + n * (t.x - e.x),
             y: r === "middle" ? n < .5 ? e.y : t.y : r === "after" ? n < 1 ? e.y : t.y : n > 0 ? t.y : e.y
         }
     }
 
-    function mYe(e, t, n, r) {
+    function vYe(e, t, n, r) {
         const a = {
                 x: e.cp2x,
                 y: e.cp2y
             },
             i = {
                 x: t.cp1x,
                 y: t.cp1y
@@ -76948,15 +76956,15 @@
             s = Cd(e, a, n),
             o = Cd(a, i, n),
             u = Cd(i, t, n),
             c = Cd(s, o, n),
             f = Cd(o, u, n);
         return Cd(c, f, n)
     }
-    const vYe = function(e, t) {
+    const gYe = function(e, t) {
             return {
                 x(n) {
                     return e + e + t - n
                 },
                 setWidth(n) {
                     t = n
                 },
@@ -76967,15 +76975,15 @@
                     return n - r
                 },
                 leftForLtr(n, r) {
                     return n - r
                 }
             }
         },
-        gYe = function() {
+        yYe = function() {
             return {
                 x(e) {
                     return e
                 },
                 setWidth(e) {},
                 textAlign(e) {
                     return e
@@ -76986,30 +76994,30 @@
                 leftForLtr(e, t) {
                     return e
                 }
             }
         };
 
     function Ah(e, t, n) {
-        return e ? vYe(t, n) : gYe()
+        return e ? gYe(t, n) : yYe()
     }
 
     function MY(e, t) {
         let n, r;
         (t === "ltr" || t === "rtl") && (n = e.canvas.style, r = [n.getPropertyValue("direction"), n.getPropertyPriority("direction")], n.setProperty("direction", t, "important"), e.prevTextDirection = r)
     }
 
     function DY(e, t) {
         t !== void 0 && (delete e.prevTextDirection, e.canvas.style.setProperty("direction", t[0], t[1]))
     }
 
     function IY(e) {
         return e === "angle" ? {
             between: d_,
-            compare: y8e,
+            compare: b8e,
             normalize: bs
         } : {
             between: uc,
             compare: (t, n) => t - n,
             normalize: t => t
         }
     }
@@ -77025,15 +77033,15 @@
             start: e % n,
             end: t % n,
             loop: r && (t - e + 1) % n === 0,
             style: a
         }
     }
 
-    function yYe(e, t, n) {
+    function bYe(e, t, n) {
         const {
             property: r,
             start: a,
             end: i
         } = n, {
             between: s,
             normalize: o
@@ -77066,15 +77074,15 @@
             between: u,
             normalize: c
         } = IY(r), {
             start: f,
             end: h,
             loop: p,
             style: g
-        } = yYe(e, t, n), _ = [];
+        } = bYe(e, t, n), _ = [];
         let y = !1,
             w = null,
             S, k, C;
         const x = () => u(a, C, S) && o(a, C) !== 0,
             E = () => o(i, S) === 0 || u(i, C, S),
             A = () => y || x(),
             O = () => !y || E();
@@ -77100,28 +77108,28 @@
         for (let a = 0; a < r.length; a++) {
             const i = LY(r[a], e.points, t);
             i.length && n.push(...i)
         }
         return n
     }
 
-    function bYe(e, t, n, r) {
+    function _Ye(e, t, n, r) {
         let a = 0,
             i = t - 1;
         if (n && !r)
             for (; a < t && !e[a].skip;) a++;
         for (; a < t && e[a].skip;) a++;
         for (a %= t, n && (i += a); i > a && e[i % t].skip;) i--;
         return i %= t, {
             start: a,
             end: i
         }
     }
 
-    function _Ye(e, t, n, r) {
+    function wYe(e, t, n, r) {
         const a = e.length,
             i = [];
         let s = t,
             o = e[t],
             u;
         for (u = t + 1; u <= n; ++u) {
             const c = e[u % a];
@@ -77134,39 +77142,39 @@
         return s !== null && i.push({
             start: t % a,
             end: s % a,
             loop: r
         }), i
     }
 
-    function wYe(e, t) {
+    function SYe(e, t) {
         const n = e.points,
             r = e.options.spanGaps,
             a = n.length;
         if (!a) return [];
         const i = !!e._loop,
             {
                 start: s,
                 end: o
-            } = bYe(n, a, i, r);
+            } = _Ye(n, a, i, r);
         if (r === !0) return AF(e, [{
             start: s,
             end: o,
             loop: i
         }], n, t);
         const u = o < s ? o + a : o,
             c = !!e._fullLoop && s === 0 && o === a - 1;
-        return AF(e, _Ye(n, s, u, c), n, t)
+        return AF(e, wYe(n, s, u, c), n, t)
     }
 
     function AF(e, t, n, r) {
-        return !r || !r.setContext || !n ? t : SYe(e, t, n, r)
+        return !r || !r.setContext || !n ? t : kYe(e, t, n, r)
     }
 
-    function SYe(e, t, n, r) {
+    function kYe(e, t, n, r) {
         const a = e._chart.getContext(),
             i = MF(e.options),
             {
                 _datasetIndex: s,
                 options: {
                     spanGaps: o
                 }
@@ -77199,15 +77207,15 @@
                 w = MF(r.setContext(Gc(a, {
                     type: "segment",
                     p0: y,
                     p1: S,
                     p0DataIndex: (p - 1) % u,
                     p1DataIndex: p % u,
                     datasetIndex: s
-                }))), kYe(w, f) && g(h, p - 1, _.loop, f), y = S, f = w
+                }))), $Ye(w, f) && g(h, p - 1, _.loop, f), y = S, f = w
             }
             h < p - 1 && g(h, p - 1, _.loop, f)
         }
         return c
     }
 
     function MF(e) {
@@ -77218,29 +77226,29 @@
             borderDashOffset: e.borderDashOffset,
             borderJoinStyle: e.borderJoinStyle,
             borderWidth: e.borderWidth,
             borderColor: e.borderColor
         }
     }
 
-    function kYe(e, t) {
+    function $Ye(e, t) {
         if (!t) return !1;
         const n = [],
             r = function(a, i) {
                 return uA(i) ? (n.includes(i) || n.push(i), n.indexOf(i)) : i
             };
         return JSON.stringify(e, r) !== JSON.stringify(t, r)
     }
     /*!
      * Chart.js v4.4.3
      * https://www.chartjs.org
      * (c) 2024 Chart.js Contributors
      * Released under the MIT License
      */
-    class $Ye {
+    class CYe {
         constructor() {
             this._request = null, this._charts = new Map, this._running = !1, this._lastDate = void 0
         }
         _notify(t, n, r, a) {
             const i = n.listeners[a],
                 s = n.duration;
             i.forEach(o => o({
@@ -77306,35 +77314,35 @@
             for (; a >= 0; --a) r[a].cancel();
             n.items = [], this._notify(t, n, Date.now(), "complete")
         }
         remove(t) {
             return this._charts.delete(t)
         }
     }
-    var Ul = new $Ye;
+    var Ul = new CYe;
     const DF = "transparent",
-        CYe = {
+        TYe = {
             boolean(e, t, n) {
                 return n > .5 ? t : e
             },
             color(e, t, n) {
                 const r = kF(e || DF),
                     a = r.valid && kF(t || DF);
                 return a && a.valid ? a.mix(r, n).hexString() : t
             },
             number(e, t, n) {
                 return e + (t - e) * n
             }
         };
-    class TYe {
+    class PYe {
         constructor(t, n, r, a) {
             const i = n[r];
             a = d0([t.to, a, i, t.from]);
             const s = d0([t.from, i, a]);
-            this._active = !0, this._fn = t.fn || CYe[t.type || typeof s], this._easing = pv[t.easing] || pv.linear, this._start = Math.floor(Date.now() + (t.delay || 0)), this._duration = this._total = Math.floor(t.duration), this._loop = !!t.loop, this._target = n, this._prop = r, this._from = s, this._to = a, this._promises = void 0
+            this._active = !0, this._fn = t.fn || TYe[t.type || typeof s], this._easing = pv[t.easing] || pv.linear, this._start = Math.floor(Date.now() + (t.delay || 0)), this._duration = this._total = Math.floor(t.duration), this._loop = !!t.loop, this._target = n, this._prop = r, this._from = s, this._to = a, this._promises = void 0
         }
         active() {
             return this._active
         }
         update(t, n, r) {
             if (this._active) {
                 this._notify(!1);
@@ -77396,18 +77404,18 @@
                 (Lr(i.properties) && i.properties || [a]).forEach(o => {
                     (o === a || !r.has(o)) && r.set(o, s)
                 })
             })
         }
         _animateOptions(t, n) {
             const r = n.options,
-                a = EYe(t, r);
+                a = xYe(t, r);
             if (!a) return [];
             const i = this._createAnimations(a, r);
-            return r.$shared && PYe(t.options.$animations, r).then(() => {
+            return r.$shared && EYe(t.options.$animations, r).then(() => {
                 t.options = r
             }, () => {}), i
         }
         _createAnimations(t, n) {
             const r = this._properties,
                 a = [],
                 i = t.$animations || (t.$animations = {}),
@@ -77429,39 +77437,39 @@
                         h.update(p, f, o);
                         continue
                     } else h.cancel();
                 if (!p || !p.duration) {
                     t[c] = f;
                     continue
                 }
-                i[c] = h = new TYe(p, t, c, f), a.push(h)
+                i[c] = h = new PYe(p, t, c, f), a.push(h)
             }
             return a
         }
         update(t, n) {
             if (this._properties.size === 0) {
                 Object.assign(t, n);
                 return
             }
             const r = this._createAnimations(t, n);
             if (r.length) return Ul.add(this._chart, r), !0
         }
     }
 
-    function PYe(e, t) {
+    function EYe(e, t) {
         const n = [],
             r = Object.keys(t);
         for (let a = 0; a < r.length; a++) {
             const i = e[r[a]];
             i && i.active() && n.push(i.wait())
         }
         return Promise.all(n)
     }
 
-    function EYe(e, t) {
+    function xYe(e, t) {
         if (!t) return;
         let n = e.options;
         if (!n) {
             e.options = t;
             return
         }
         return n.$shared && (e.options = n = Object.assign({}, n, {
@@ -77477,27 +77485,27 @@
             i = n.max === void 0 ? t : 0;
         return {
             start: r ? i : a,
             end: r ? a : i
         }
     }
 
-    function xYe(e, t, n) {
+    function OYe(e, t, n) {
         if (n === !1) return !1;
         const r = IF(e, n),
             a = IF(t, n);
         return {
             top: a.end,
             right: r.end,
             bottom: a.start,
             left: r.start
         }
     }
 
-    function OYe(e) {
+    function AYe(e) {
         let t, n, r, a;
         return Tn(e) ? (t = e.top, n = e.right, r = e.bottom, a = e.left) : t = n = r = a = e, {
             top: t,
             right: n,
             bottom: r,
             left: a,
             disabled: e === !1
@@ -77524,15 +77532,15 @@
                 }
                 c = e.values[u], ta(c) && (i || t === 0 || hl(t) === hl(c)) && (t += c)
             }
             return t
         }
     }
 
-    function AYe(e, t) {
+    function MYe(e, t) {
         const {
             iScale: n,
             vScale: r
         } = t, a = n.axis === "x" ? "x" : "y", i = r.axis === "x" ? "x" : "y", s = Object.keys(e), o = new Array(s.length);
         let u, c, f;
         for (u = 0, c = s.length; u < c; ++u) f = s[u], o[u] = {
             [a]: f,
@@ -77542,32 +77550,32 @@
     }
 
     function RF(e, t) {
         const n = e && e.options.stacked;
         return n || n === void 0 && t.stack !== void 0
     }
 
-    function MYe(e, t, n) {
+    function DYe(e, t, n) {
         return `${e.id}.${t.id}.${n.stack||n.type}`
     }
 
-    function DYe(e) {
+    function IYe(e) {
         const {
             min: t,
             max: n,
             minDefined: r,
             maxDefined: a
         } = e.getUserBounds();
         return {
             min: r ? t : Number.NEGATIVE_INFINITY,
             max: a ? n : Number.POSITIVE_INFINITY
         }
     }
 
-    function IYe(e, t, n) {
+    function LYe(e, t, n) {
         const r = e[t] || (e[t] = {});
         return r[n] || (r[n] = {})
     }
 
     function NF(e, t, n, r) {
         for (const a of t.getMatchingVisibleMetas(r).reverse()) {
             const i = e[a.index];
@@ -77580,46 +77588,46 @@
         const {
             chart: n,
             _cachedMeta: r
         } = e, a = n._stacks || (n._stacks = {}), {
             iScale: i,
             vScale: s,
             index: o
-        } = r, u = i.axis, c = s.axis, f = MYe(i, s, r), h = t.length;
+        } = r, u = i.axis, c = s.axis, f = DYe(i, s, r), h = t.length;
         let p;
         for (let g = 0; g < h; ++g) {
             const _ = t[g],
                 {
                     [u]: y,
                     [c]: w
                 } = _,
                 S = _._stacks || (_._stacks = {});
-            p = S[c] = IYe(a, f, y), p[o] = w, p._top = NF(p, s, !0, r.type), p._bottom = NF(p, s, !1, r.type);
+            p = S[c] = LYe(a, f, y), p[o] = w, p._top = NF(p, s, !0, r.type), p._bottom = NF(p, s, !1, r.type);
             const k = p._visualValues || (p._visualValues = {});
             k[o] = w
         }
     }
 
     function Ak(e, t) {
         const n = e.scales;
         return Object.keys(n).filter(r => n[r].axis === t).shift()
     }
 
-    function LYe(e, t) {
+    function RYe(e, t) {
         return Gc(e, {
             active: !1,
             dataset: void 0,
             datasetIndex: t,
             index: t,
             mode: "default",
             type: "dataset"
         })
     }
 
-    function RYe(e, t, n) {
+    function NYe(e, t, n) {
         return Gc(e, {
             active: !1,
             dataIndex: t,
             parsed: void 0,
             raw: void 0,
             element: n,
             index: t,
@@ -77638,15 +77646,15 @@
                 if (!i || i[r] === void 0 || i[r][n] === void 0) return;
                 delete i[r][n], i[r]._visualValues !== void 0 && i[r]._visualValues[n] !== void 0 && delete i[r]._visualValues[n]
             }
         }
     }
     const Mk = e => e === "reset" || e === "none",
         VF = (e, t) => t ? e : Object.assign({}, e),
-        NYe = (e, t, n) => e && !t.hidden && t._stacked && {
+        FYe = (e, t, n) => e && !t.hidden && t._stacked && {
             keys: FY(n, !0),
             values: null
         };
     class Co {
         constructor(t, n) {
             this.chart = t, this._ctx = t.ctx, this.index = n, this._cachedDataOpts = {}, this._cachedMeta = this.getMeta(), this._type = this._cachedMeta.type, this.options = void 0, this._parsing = !1, this._data = void 0, this._objectData = void 0, this._sharedOptions = void 0, this._drawStart = void 0, this._drawCount = void 0, this.enableOptionSharing = !1, this.supportsDecimation = !1, this.$context = void 0, this._syncList = [], this.datasetElementType = new.target.datasetElementType, this.dataElementType = new.target.dataElementType, this.initialize()
         }
@@ -77692,22 +77700,22 @@
         }
         _dataCheck() {
             const t = this.getDataset(),
                 n = t.data || (t.data = []),
                 r = this._data;
             if (Tn(n)) {
                 const a = this._cachedMeta;
-                this._data = AYe(n, a)
+                this._data = MYe(n, a)
             } else if (r !== n) {
                 if (r) {
                     _F(r, this);
                     const a = this._cachedMeta;
                     Am(a), a._parsed = []
                 }
-                n && Object.isExtensible(n) && S8e(n, this), this._syncList = [], this._data = n
+                n && Object.isExtensible(n) && k8e(n, this), this._syncList = [], this._data = n
             }
         }
         addElements() {
             const t = this._cachedMeta;
             this._dataCheck(), this.datasetElementType && (t.dataset = new this.datasetElementType)
         }
         buildOrUpdateElements(t) {
@@ -77809,23 +77817,23 @@
         }
         getMinMax(t, n) {
             const r = this._cachedMeta,
                 a = r._parsed,
                 i = r._sorted && t === r.iScale,
                 s = a.length,
                 o = this._getOtherScale(t),
-                u = NYe(n, r, this.chart),
+                u = FYe(n, r, this.chart),
                 c = {
                     min: Number.POSITIVE_INFINITY,
                     max: Number.NEGATIVE_INFINITY
                 },
                 {
                     min: f,
                     max: h
-                } = DYe(o);
+                } = IYe(o);
             let p, g;
 
             function _() {
                 g = a[p];
                 const y = g[o.axis];
                 return !ta(g[t.axis]) || f > y || h < y
             }
@@ -77857,15 +77865,15 @@
             return {
                 label: r ? "" + r.getLabelForValue(i[r.axis]) : "",
                 value: a ? "" + a.getLabelForValue(i[a.axis]) : ""
             }
         }
         _update(t) {
             const n = this._cachedMeta;
-            this.update(t || "default"), n._clip = OYe(un(this.options.clip, xYe(n.xScale, n.yScale, this.getMaxOverflow())))
+            this.update(t || "default"), n._clip = AYe(un(this.options.clip, OYe(n.xScale, n.yScale, this.getMaxOverflow())))
         }
         update(t) {}
         draw() {
             const t = this._ctx,
                 n = this.chart,
                 r = this._cachedMeta,
                 a = r.data || [],
@@ -77886,16 +77894,16 @@
             return t === void 0 && this._cachedMeta.dataset ? this.resolveDatasetElementOptions(r) : this.resolveDataElementOptions(t || 0, r)
         }
         getContext(t, n, r) {
             const a = this.getDataset();
             let i;
             if (t >= 0 && t < this._cachedMeta.data.length) {
                 const s = this._cachedMeta.data[t];
-                i = s.$context || (s.$context = RYe(this.getContext(), t, s)), i.parsed = this.getParsed(t), i.raw = a.data[t], i.index = i.dataIndex = t
-            } else i = this.$context || (this.$context = LYe(this.chart.getContext(), this.index)), i.dataset = a, i.index = i.datasetIndex = this.index;
+                i = s.$context || (s.$context = NYe(this.getContext(), t, s)), i.parsed = this.getParsed(t), i.raw = a.data[t], i.index = i.dataIndex = t
+            } else i = this.$context || (this.$context = RYe(this.chart.getContext(), this.index)), i.dataset = a, i.index = i.datasetIndex = this.index;
             return i.active = !!n, i.mode = r, i
         }
         resolveDatasetElementOptions(t) {
             return this._resolveElementOptions(this.datasetElementType.id, t)
         }
         resolveDataElementOptions(t, n) {
             return this._resolveElementOptions(this.dataElementType.id, n, t)
@@ -78030,63 +78038,63 @@
         }
         _onDataUnshift() {
             this._sync(["_insertElements", 0, arguments.length])
         }
     }
     Ye(Co, "defaults", {}), Ye(Co, "datasetElementType", null), Ye(Co, "dataElementType", null);
 
-    function FYe(e, t) {
+    function VYe(e, t) {
         if (!e._cache.$bar) {
             const n = e.getMatchingVisibleMetas(t);
             let r = [];
             for (let a = 0, i = n.length; a < i; a++) r = r.concat(n[a].controller.getAllParsedValues(e));
             e._cache.$bar = gY(r.sort((a, i) => a - i))
         }
         return e._cache.$bar
     }
 
-    function VYe(e) {
+    function jYe(e) {
         const t = e.iScale,
-            n = FYe(t, e.type);
+            n = VYe(t, e.type);
         let r = t._length,
             a, i, s, o;
         const u = () => {
             s === 32767 || s === -32768 || (Qv(o) && (r = Math.min(r, Math.abs(s - o) || r)), o = s)
         };
         for (a = 0, i = n.length; a < i; ++a) s = t.getPixelForValue(n[a]), u();
         for (o = void 0, a = 0, i = t.ticks.length; a < i; ++a) s = t.getPixelForTick(a), u();
         return r
     }
 
-    function jYe(e, t, n, r) {
+    function BYe(e, t, n, r) {
         const a = n.barThickness;
         let i, s;
         return Xn(a) ? (i = t.min * n.categoryPercentage, s = n.barPercentage) : (i = a * r, s = 1), {
             chunk: i / r,
             ratio: s,
             start: t.pixels[e] - i / 2
         }
     }
 
-    function BYe(e, t, n, r) {
+    function HYe(e, t, n, r) {
         const a = t.pixels,
             i = a[e];
         let s = e > 0 ? a[e - 1] : null,
             o = e < a.length - 1 ? a[e + 1] : null;
         const u = n.categoryPercentage;
         s === null && (s = i - (o === null ? t.end - t.start : o - i)), o === null && (o = i + i - s);
         const c = i - (i - Math.min(s, o)) / 2 * u;
         return {
             chunk: Math.abs(o - s) / 2 * u / r,
             ratio: n.barPercentage,
             start: c
         }
     }
 
-    function HYe(e, t, n, r) {
+    function WYe(e, t, n, r) {
         const a = n.parse(e[0], r),
             i = n.parse(e[1], r),
             s = Math.min(a, i),
             o = Math.max(a, i);
         let u = s,
             c = o;
         Math.abs(s) > Math.abs(o) && (u = o, c = s), t[n.axis] = c, t._custom = {
@@ -78096,15 +78104,15 @@
             end: i,
             min: s,
             max: o
         }
     }
 
     function VY(e, t, n, r) {
-        return Lr(e) ? HYe(e, t, n, r) : t[n.axis] = n.parse(e, r), t
+        return Lr(e) ? WYe(e, t, n, r) : t[n.axis] = n.parse(e, r), t
     }
 
     function jF(e, t, n, r) {
         const a = e.iScale,
             i = e.vScale,
             s = a.getLabels(),
             o = a === i,
@@ -78114,30 +78122,30 @@
         return u
     }
 
     function Dk(e) {
         return e && e.barStart !== void 0 && e.barEnd !== void 0
     }
 
-    function WYe(e, t, n) {
+    function UYe(e, t, n) {
         return e !== 0 ? hl(e) : (t.isHorizontal() ? 1 : -1) * (t.min >= n ? 1 : -1)
     }
 
-    function UYe(e) {
+    function zYe(e) {
         let t, n, r, a, i;
         return e.horizontal ? (t = e.base > e.x, n = "left", r = "right") : (t = e.base < e.y, n = "bottom", r = "top"), t ? (a = "end", i = "start") : (a = "start", i = "end"), {
             start: n,
             end: r,
             reverse: t,
             top: a,
             bottom: i
         }
     }
 
-    function zYe(e, t, n, r) {
+    function YYe(e, t, n, r) {
         let a = t.borderSkipped;
         const i = {};
         if (!a) {
             e.borderSkipped = i;
             return
         }
         if (a === !0) {
@@ -78151,31 +78159,31 @@
         }
         const {
             start: s,
             end: o,
             reverse: u,
             top: c,
             bottom: f
-        } = UYe(e);
+        } = zYe(e);
         a === "middle" && n && (e.enableBorderRadius = !0, (n._top || 0) === r ? a = c : (n._bottom || 0) === r ? a = f : (i[BF(f, s, o, u)] = !0, a = c)), i[BF(a, s, o, u)] = !0, e.borderSkipped = i
     }
 
     function BF(e, t, n, r) {
-        return r ? (e = YYe(e, t, n), e = HF(e, n, t)) : e = HF(e, t, n), e
+        return r ? (e = qYe(e, t, n), e = HF(e, n, t)) : e = HF(e, t, n), e
     }
 
-    function YYe(e, t, n) {
+    function qYe(e, t, n) {
         return e === t ? n : e === n ? t : e
     }
 
     function HF(e, t, n) {
         return e === "start" ? t : e === "end" ? n : e
     }
 
-    function qYe(e, {
+    function GYe(e, {
         inflateAmount: t
     }, n) {
         e.inflateAmount = t === "auto" ? n === 1 ? .33 : 0 : t
     }
     class J0 extends Co {
         parsePrimitiveData(t, n, r, a) {
             return jF(t, n, r, a)
@@ -78256,15 +78264,15 @@
                         x: c ? y.head : w.center,
                         y: c ? w.center : y.head,
                         height: c ? w.size : Math.abs(y.size),
                         width: c ? Math.abs(y.size) : w.size
                     };
                 p && (k.options = h || this.resolveDataElementOptions(g, t[g].active ? "active" : a));
                 const C = k.options || t[g].options;
-                zYe(k, C, S, s), qYe(k, C, f.ratio), this.updateElement(t[g], g, k, a)
+                YYe(k, C, S, s), GYe(k, C, f.ratio), this.updateElement(t[g], g, k, a)
             }
         }
         _getStacks(t, n) {
             const {
                 iScale: r
             } = this._cachedMeta, a = r.getMatchingVisibleMetas(this._type).filter(u => u.controller.options.grouped), i = r.options.stacked, s = [], o = u => {
                 const c = u.controller.getParsed(n),
@@ -78288,15 +78296,15 @@
                 n = this._cachedMeta,
                 r = n.iScale,
                 a = [];
             let i, s;
             for (i = 0, s = n.data.length; i < s; ++i) a.push(r.getPixelForValue(this.getParsed(i)[r.axis], i));
             const o = t.barThickness;
             return {
-                min: o || VYe(n),
+                min: o || jYe(n),
                 pixels: a,
                 start: r._startPixel,
                 end: r._endPixel,
                 stackCount: this._getStackCount(),
                 scale: r,
                 grouped: t.grouped,
                 ratio: o ? 1 : t.categoryPercentage * t.barPercentage
@@ -78318,15 +78326,15 @@
                 p = 0,
                 g = r ? this.applyStack(n, u, r) : h,
                 _, y;
             g !== h && (p = g - h, g = h), f && (h = c.barStart, g = c.barEnd - c.barStart, h !== 0 && hl(h) !== hl(c.barEnd) && (p = 0), p += h);
             const w = !Xn(i) && !f ? i : p;
             let S = n.getPixelForValue(w);
             if (this.chart.getDataVisibility(t) ? _ = n.getPixelForValue(p + g) : _ = S, y = _ - S, Math.abs(y) < s) {
-                y = WYe(y, n, o) * s, h === o && (S -= y / 2);
+                y = UYe(y, n, o) * s, h === o && (S -= y / 2);
                 const k = n.getPixelForDecimal(0),
                     C = n.getPixelForDecimal(1),
                     x = Math.min(k, C),
                     E = Math.max(k, C);
                 S = Math.max(Math.min(S, E), x), _ = S + y, r && !f && (u._stacks[n.axis]._visualValues[a] = n.getValueForPixel(_) - n.getValueForPixel(S))
             }
             if (S === n.getPixelForValue(o)) {
@@ -78344,15 +78352,15 @@
             const r = n.scale,
                 a = this.options,
                 i = a.skipNull,
                 s = un(a.maxBarThickness, 1 / 0);
             let o, u;
             if (n.grouped) {
                 const c = i ? this._getStackCount(t) : n.stackCount,
-                    f = a.barThickness === "flex" ? BYe(t, n, a, c) : jYe(t, n, a, c),
+                    f = a.barThickness === "flex" ? HYe(t, n, a, c) : BYe(t, n, a, c),
                     h = this._getStackIndex(this.index, this._cachedMeta.stack, i ? t : void 0);
                 o = f.start + f.chunk * h + f.chunk / 2, u = Math.min(s, f.chunk * f.ratio)
             } else o = r.getPixelForValue(this.getParsed(t)[r.axis], t), u = Math.min(s, n.min * n.ratio);
             return {
                 base: o - u / 2,
                 head: o + u / 2,
                 center: o,
@@ -78493,15 +78501,15 @@
             },
             y: {
                 type: "linear"
             }
         }
     });
 
-    function GYe(e, t, n) {
+    function KYe(e, t, n) {
         let r = 1,
             a = 1,
             i = 0,
             s = 0;
         if (t < Ya) {
             const o = e,
                 u = o + t,
@@ -78570,26 +78578,26 @@
                 {
                     chartArea: r
                 } = n,
                 a = this._cachedMeta,
                 i = a.data,
                 s = this.getMaxBorderWidth() + this.getMaxOffset(i) + this.options.spacing,
                 o = Math.max((Math.min(r.width, r.height) - s) / 2, 0),
-                u = Math.min(o8e(this.options.cutout, o), 1),
+                u = Math.min(l8e(this.options.cutout, o), 1),
                 c = this._getRingWeight(this.index),
                 {
                     circumference: f,
                     rotation: h
                 } = this._getRotationExtents(),
                 {
                     ratioX: p,
                     ratioY: g,
                     offsetX: _,
                     offsetY: y
-                } = GYe(h, f, u),
+                } = KYe(h, f, u),
                 w = (r.width - s) / p,
                 S = (r.height - s) / g,
                 k = Math.max(Math.min(w, S) / 2, 0),
                 C = hY(this.options.radius, k),
                 x = Math.max(C * u, 0),
                 E = (C - x) / this._getVisibleDatasetWeightTotal();
             this.offsetX = _ * C, this.offsetY = y * C, a.total = this.calculateTotal(), this.outerRadius = C - E * this._getRingWeightOffset(this.index), this.innerRadius = Math.max(this.outerRadius - E * c, 0), this.updateElements(i, 0, i.length, t)
@@ -79208,26 +79216,26 @@
         startOf() {
             return bd()
         }
         endOf() {
             return bd()
         }
     }
-    var KYe = {
+    var XYe = {
         _date: mA
     };
 
-    function XYe(e, t, n, r) {
+    function JYe(e, t, n, r) {
         const {
             controller: a,
             data: i,
             _sorted: s
         } = e, o = a._cachedMeta.iScale;
         if (o && t === o.axis && t !== "r" && s && i.length) {
-            const u = o._reversePixels ? _8e : Vd;
+            const u = o._reversePixels ? w8e : Vd;
             if (r) {
                 if (a._sharedOptions) {
                     const c = i[0],
                         f = typeof c.getRange == "function" && c.getRange(t);
                     if (f) {
                         const h = u(i, t, n - f),
                             p = u(i, t, n + f);
@@ -79251,23 +79259,23 @@
         for (let o = 0, u = i.length; o < u; ++o) {
             const {
                 index: c,
                 data: f
             } = i[o], {
                 lo: h,
                 hi: p
-            } = XYe(i[o], t, s, a);
+            } = JYe(i[o], t, s, a);
             for (let g = h; g <= p; ++g) {
                 const _ = f[g];
                 _.skip || r(_, c, g)
             }
         }
     }
 
-    function JYe(e) {
+    function ZYe(e) {
         const t = e.indexOf("x") !== -1,
             n = e.indexOf("y") !== -1;
         return function(r, a) {
             const i = t ? Math.abs(r.x - a.x) : 0,
                 s = n ? Math.abs(r.y - a.y) : 0;
             return Math.sqrt(Math.pow(i, 2) + Math.pow(s, 2))
         }
@@ -79280,39 +79288,39 @@
                 element: o,
                 datasetIndex: u,
                 index: c
             })
         }, !0), i
     }
 
-    function ZYe(e, t, n, r) {
+    function QYe(e, t, n, r) {
         let a = [];
 
         function i(s, o, u) {
             const {
                 startAngle: c,
                 endAngle: f
             } = s.getProps(["startAngle", "endAngle"], r), {
                 angle: h
-            } = g8e(s, {
+            } = y8e(s, {
                 x: t.x,
                 y: t.y
             });
             d_(h, c, f) && a.push({
                 element: s,
                 datasetIndex: o,
                 index: u
             })
         }
         return Xg(e, n, t, i), a
     }
 
-    function QYe(e, t, n, r, a, i) {
+    function eqe(e, t, n, r, a, i) {
         let s = [];
-        const o = JYe(n);
+        const o = ZYe(n);
         let u = Number.POSITIVE_INFINITY;
 
         function c(f, h, p) {
             const g = f.inRange(t.x, t.y, a);
             if (r && !g) return;
             const _ = f.getCenterPoint(a);
             if (!(!!i || e.isPointInArea(_)) && !g) return;
@@ -79327,30 +79335,30 @@
                 index: p
             })
         }
         return Xg(e, n, t, c), s
     }
 
     function Lk(e, t, n, r, a, i) {
-        return !i && !e.isPointInArea(t) ? [] : n === "r" && !r ? ZYe(e, t, n, a) : QYe(e, t, n, r, a, i)
+        return !i && !e.isPointInArea(t) ? [] : n === "r" && !r ? QYe(e, t, n, a) : eqe(e, t, n, r, a, i)
     }
 
     function WF(e, t, n, r, a) {
         const i = [],
             s = n === "x" ? "inXRange" : "inYRange";
         let o = !1;
         return Xg(e, n, t, (u, c, f) => {
             u[s](t[n], a) && (i.push({
                 element: u,
                 datasetIndex: c,
                 index: f
             }), o = o || u.inRange(t.x, t.y, a))
         }), r && !o ? [] : i
     }
-    var eqe = {
+    var tqe = {
         evaluateInteractionItems: Xg,
         modes: {
             index(e, t, n, r) {
                 const a = $d(t, e),
                     i = n.axis || "x",
                     s = n.includeInvisible || !1,
                     o = n.intersect ? Ik(e, a, i, r, s) : Lk(e, a, i, !1, r, s),
@@ -79418,15 +79426,15 @@
         return e.sort((n, r) => {
             const a = t ? r : n,
                 i = t ? n : r;
             return a.weight === i.weight ? a.index - i.index : a.weight - i.weight
         })
     }
 
-    function tqe(e) {
+    function nqe(e) {
         const t = [];
         let n, r, a, i, s, o;
         for (n = 0, r = (e || []).length; n < r; ++n) a = e[n], {
             position: i,
             options: {
                 stack: s,
                 stackWeight: o = 1
@@ -79439,15 +79447,15 @@
             weight: a.weight,
             stack: s && i + s,
             stackWeight: o
         });
         return t
     }
 
-    function nqe(e) {
+    function rqe(e) {
         const t = {};
         for (const n of e) {
             const {
                 stack: r,
                 pos: a,
                 stackWeight: i
             } = n;
@@ -79459,16 +79467,16 @@
                 size: 0
             });
             s.count++, s.weight += i
         }
         return t
     }
 
-    function rqe(e, t) {
-        const n = nqe(e),
+    function aqe(e, t) {
+        const n = rqe(e),
             {
                 vBoxMaxWidth: r,
                 hBoxMaxHeight: a
             } = t;
         let i, s, o;
         for (i = 0, s = e.length; i < s; ++i) {
             o = e[i];
@@ -79476,16 +79484,16 @@
                 fullSize: u
             } = o.box, c = n[o.stack], f = c && o.stackWeight / c.weight;
             o.horizontal ? (o.width = f ? f * r : u && t.availableWidth, o.height = a) : (o.width = r, o.height = f ? f * a : u && t.availableHeight)
         }
         return n
     }
 
-    function aqe(e) {
-        const t = tqe(e),
+    function iqe(e) {
+        const t = nqe(e),
             n = Dm(t.filter(c => c.box.fullSize), !0),
             r = Dm(Mm(t, "left"), !0),
             a = Dm(Mm(t, "right")),
             i = Dm(Mm(t, "top"), !0),
             s = Dm(Mm(t, "bottom")),
             o = UF(t, "x"),
             u = UF(t, "y");
@@ -79503,15 +79511,15 @@
         return Math.max(e[n], t[n]) + Math.max(e[r], t[r])
     }
 
     function BY(e, t) {
         e.top = Math.max(e.top, t.top), e.left = Math.max(e.left, t.left), e.bottom = Math.max(e.bottom, t.bottom), e.right = Math.max(e.right, t.right)
     }
 
-    function iqe(e, t, n, r) {
+    function sqe(e, t, n, r) {
         const {
             pos: a,
             box: i
         } = n, s = e.maxPadding;
         if (!Tn(a)) {
             n.size && (e[a] -= n.size);
             const h = r[n.stack] || {
@@ -79530,25 +79538,25 @@
             other: f
         } : {
             same: f,
             other: c
         }
     }
 
-    function sqe(e) {
+    function oqe(e) {
         const t = e.maxPadding;
 
         function n(r) {
             const a = Math.max(t[r] - e[r], 0);
             return e[r] += a, a
         }
         e.y += n("top"), e.x += n("left"), n("right"), n("bottom")
     }
 
-    function oqe(e, t) {
+    function lqe(e, t) {
         const n = t.maxPadding;
 
         function r(a) {
             const i = {
                 left: 0,
                 top: 0,
                 right: 0,
@@ -79561,19 +79569,19 @@
         return r(e ? ["left", "right"] : ["top", "bottom"])
     }
 
     function Bm(e, t, n, r) {
         const a = [];
         let i, s, o, u, c, f;
         for (i = 0, s = e.length, c = 0; i < s; ++i) {
-            o = e[i], u = o.box, u.update(o.width || t.w, o.height || t.h, oqe(o.horizontal, t));
+            o = e[i], u = o.box, u.update(o.width || t.w, o.height || t.h, lqe(o.horizontal, t));
             const {
                 same: h,
                 other: p
-            } = iqe(t, n, o, r);
+            } = sqe(t, n, o, r);
             c |= h && a.length, f = f || p, u.fullSize || a.push(o)
         }
         return c && Bm(a, t, n, r) || f
     }
 
     function p0(e, t, n, r, a) {
         e.top = n, e.left = t, e.right = t + r, e.bottom = n + a, e.width = r, e.height = a
@@ -79624,15 +79632,15 @@
             t.fullSize = n.fullSize, t.position = n.position, t.weight = n.weight
         },
         update(e, t, n, r) {
             if (!e) return;
             const a = Ti(e.options.layout.padding),
                 i = Math.max(t - a.width, 0),
                 s = Math.max(n - a.height, 0),
-                o = aqe(e.boxes),
+                o = iqe(e.boxes),
                 u = o.vertical,
                 c = o.horizontal;
             ar(e.boxes, y => {
                 typeof y.beforeLayout == "function" && y.beforeLayout()
             });
             const f = u.reduce((y, w) => w.box.options && w.box.options.display === !1 ? y : y + 1, 0) || 1,
                 h = Object.freeze({
@@ -79649,16 +79657,16 @@
             const g = Object.assign({
                     maxPadding: p,
                     w: i,
                     h: s,
                     x: a.left,
                     y: a.top
                 }, a),
-                _ = rqe(u.concat(c), h);
-            Bm(o.fullSize, g, h, _), Bm(u, g, h, _), Bm(c, g, h, _) && Bm(u, g, h, _), sqe(g), YF(o.leftAndTop, g, h, _), g.x += g.w, g.y += g.h, YF(o.rightAndBottom, g, h, _), e.chartArea = {
+                _ = aqe(u.concat(c), h);
+            Bm(o.fullSize, g, h, _), Bm(u, g, h, _), Bm(c, g, h, _) && Bm(u, g, h, _), oqe(g), YF(o.leftAndTop, g, h, _), g.x += g.w, g.y += g.h, YF(o.rightAndBottom, g, h, _), e.chartArea = {
                 left: g.left,
                 top: g.top,
                 right: g.left + g.w,
                 bottom: g.top + g.h,
                 height: g.h,
                 width: g.w
             }, ar(o.chartArea, y => {
@@ -79689,37 +79697,37 @@
             }
         }
         isAttached(t) {
             return !0
         }
         updateConfig(t) {}
     }
-    class lqe extends HY {
+    class uqe extends HY {
         acquireContext(t) {
             return t && t.getContext && t.getContext("2d") || null
         }
         updateConfig(t) {
             t.options.animation = !1
         }
     }
     const rb = "$chartjs",
-        uqe = {
+        cqe = {
             touchstart: "mousedown",
             touchmove: "mousemove",
             touchend: "mouseup",
             pointerenter: "mouseenter",
             pointerdown: "mousedown",
             pointermove: "mousemove",
             pointerup: "mouseup",
             pointerleave: "mouseout",
             pointerout: "mouseout"
         },
         qF = e => e === null || e === "";
 
-    function cqe(e, t) {
+    function dqe(e, t) {
         const n = e.style,
             r = e.getAttribute("height"),
             a = e.getAttribute("width");
         if (e[rb] = {
                 initial: {
                     height: r,
                     width: a,
@@ -79736,28 +79744,28 @@
         if (qF(r))
             if (e.style.height === "") e.height = e.width / (t || 2);
             else {
                 const i = xF(e, "height");
                 i !== void 0 && (e.height = i)
             } return e
     }
-    const WY = hYe ? {
+    const WY = pYe ? {
         passive: !0
     } : !1;
 
-    function dqe(e, t, n) {
+    function fqe(e, t, n) {
         e && e.addEventListener(t, n, WY)
     }
 
-    function fqe(e, t, n) {
+    function hqe(e, t, n) {
         e && e.canvas && e.canvas.removeEventListener(t, n, WY)
     }
 
-    function hqe(e, t) {
-        const n = uqe[e.type] || e.type,
+    function pqe(e, t) {
+        const n = cqe[e.type] || e.type,
             {
                 x: r,
                 y: a
             } = $d(e, t);
         return {
             type: n,
             chart: t,
@@ -79768,28 +79776,28 @@
     }
 
     function p_(e, t) {
         for (const n of e)
             if (n === t || n.contains(t)) return !0
     }
 
-    function pqe(e, t, n) {
+    function mqe(e, t, n) {
         const r = e.canvas,
             a = new MutationObserver(i => {
                 let s = !1;
                 for (const o of i) s = s || p_(o.addedNodes, r), s = s && !p_(o.removedNodes, r);
                 s && n()
             });
         return a.observe(document, {
             childList: !0,
             subtree: !0
         }), a
     }
 
-    function mqe(e, t, n) {
+    function vqe(e, t, n) {
         const r = e.canvas,
             a = new MutationObserver(i => {
                 let s = !1;
                 for (const o of i) s = s || p_(o.removedNodes, r), s = s && !p_(o.addedNodes, r);
                 s && n()
             });
         return a.observe(document, {
@@ -79803,54 +79811,54 @@
     function UY() {
         const e = window.devicePixelRatio;
         e !== GF && (GF = e, tg.forEach((t, n) => {
             n.currentDevicePixelRatio !== e && t()
         }))
     }
 
-    function vqe(e, t) {
+    function gqe(e, t) {
         tg.size || window.addEventListener("resize", UY), tg.set(e, t)
     }
 
-    function gqe(e) {
+    function yqe(e) {
         tg.delete(e), tg.size || window.removeEventListener("resize", UY)
     }
 
-    function yqe(e, t, n) {
+    function bqe(e, t, n) {
         const r = e.canvas,
             a = r && pA(r);
         if (!a) return;
         const i = bY((o, u) => {
                 const c = a.clientWidth;
                 n(o, u), c < a.clientWidth && n()
             }, window),
             s = new ResizeObserver(o => {
                 const u = o[0],
                     c = u.contentRect.width,
                     f = u.contentRect.height;
                 c === 0 && f === 0 || i(c, f)
             });
-        return s.observe(a), vqe(e, i), s
+        return s.observe(a), gqe(e, i), s
     }
 
     function Rk(e, t, n) {
-        n && n.disconnect(), t === "resize" && gqe(e)
+        n && n.disconnect(), t === "resize" && yqe(e)
     }
 
-    function bqe(e, t, n) {
+    function _qe(e, t, n) {
         const r = e.canvas,
             a = bY(i => {
-                e.ctx !== null && n(hqe(i, e))
+                e.ctx !== null && n(pqe(i, e))
             }, e);
-        return dqe(r, t, a), a
+        return fqe(r, t, a), a
     }
-    class _qe extends HY {
+    class wqe extends HY {
         acquireContext(t, n) {
             const r = t && t.getContext && t.getContext("2d");
-            return r && r.canvas === t ? (cqe(t, n), r) : null
+            return r && r.canvas === t ? (dqe(t, n), r) : null
         }
         releaseContext(t) {
             const n = t.canvas;
             if (!n[rb]) return !1;
             const r = n[rb].initial;
             ["height", "width"].forEach(i => {
                 const s = r[i];
@@ -79861,44 +79869,44 @@
                 n.style[i] = a[i]
             }), n.width = n.width, delete n[rb], !0
         }
         addEventListener(t, n, r) {
             this.removeEventListener(t, n);
             const a = t.$proxies || (t.$proxies = {}),
                 s = {
-                    attach: pqe,
-                    detach: mqe,
-                    resize: yqe
-                } [n] || bqe;
+                    attach: mqe,
+                    detach: vqe,
+                    resize: bqe
+                } [n] || _qe;
             a[n] = s(t, n, r)
         }
         removeEventListener(t, n) {
             const r = t.$proxies || (t.$proxies = {}),
                 a = r[n];
             if (!a) return;
             ({
                 attach: Rk,
                 detach: Rk,
                 resize: Rk
-            } [n] || fqe)(t, n, a), r[n] = void 0
+            } [n] || hqe)(t, n, a), r[n] = void 0
         }
         getDevicePixelRatio() {
             return window.devicePixelRatio
         }
         getMaximumSize(t, n, r, a) {
-            return fYe(t, n, r, a)
+            return hYe(t, n, r, a)
         }
         isAttached(t) {
             const n = t && pA(t);
             return !!(n && n.isConnected)
         }
     }
 
-    function wqe(e) {
-        return !hA() || typeof OffscreenCanvas < "u" && e instanceof OffscreenCanvas ? lqe : _qe
+    function Sqe(e) {
+        return !hA() || typeof OffscreenCanvas < "u" && e instanceof OffscreenCanvas ? uqe : wqe
     }
     var S0;
     let Kc = (S0 = class {
         constructor() {
             Ye(this, "x");
             Ye(this, "y");
             Ye(this, "active", !1);
@@ -79924,62 +79932,62 @@
             const a = {};
             return t.forEach(i => {
                 a[i] = r[i] && r[i].active() ? r[i]._to : this[i]
             }), a
         }
     }, Ye(S0, "defaults", {}), Ye(S0, "defaultRoutes"), S0);
 
-    function Sqe(e, t) {
+    function kqe(e, t) {
         const n = e.options.ticks,
-            r = kqe(e),
+            r = $qe(e),
             a = Math.min(n.maxTicksLimit || r, r),
-            i = n.major.enabled ? Cqe(t) : [],
+            i = n.major.enabled ? Tqe(t) : [],
             s = i.length,
             o = i[0],
             u = i[s - 1],
             c = [];
-        if (s > a) return Tqe(t, c, i, s / a), c;
-        const f = $qe(i, t, a);
+        if (s > a) return Pqe(t, c, i, s / a), c;
+        const f = Cqe(i, t, a);
         if (s > 0) {
             let h, p;
             const g = s > 1 ? Math.round((u - o) / (s - 1)) : null;
             for (m0(t, c, f, Xn(g) ? 0 : o - g, o), h = 0, p = s - 1; h < p; h++) m0(t, c, f, i[h], i[h + 1]);
             return m0(t, c, f, u, Xn(g) ? t.length : u + g), c
         }
         return m0(t, c, f), c
     }
 
-    function kqe(e) {
+    function $qe(e) {
         const t = e.options.offset,
             n = e._tickSize(),
             r = e._length / n + (t ? 0 : 1),
             a = e._maxLength / n;
         return Math.floor(Math.min(r, a))
     }
 
-    function $qe(e, t, n) {
-        const r = Pqe(e),
+    function Cqe(e, t, n) {
+        const r = Eqe(e),
             a = t.length / n;
         if (!r) return Math.max(a, 1);
-        const i = m8e(r);
+        const i = v8e(r);
         for (let s = 0, o = i.length - 1; s < o; s++) {
             const u = i[s];
             if (u > a) return u
         }
         return Math.max(a, 1)
     }
 
-    function Cqe(e) {
+    function Tqe(e) {
         const t = [];
         let n, r;
         for (n = 0, r = e.length; n < r; n++) e[n].major && t.push(n);
         return t
     }
 
-    function Tqe(e, t, n, r) {
+    function Pqe(e, t, n, r) {
         let a = 0,
             i = n[0],
             s;
         for (r = Math.ceil(r), s = 0; s < e.length; s++) s === i && (t.push(e[s]), a++, i = n[a * r])
     }
 
     function m0(e, t, n, r, a) {
@@ -79987,47 +79995,47 @@
             s = Math.min(un(a, e.length), e.length);
         let o = 0,
             u, c, f;
         for (n = Math.ceil(n), a && (u = a - r, n = u / Math.floor(u / n)), f = i; f < 0;) o++, f = Math.round(i + o * n);
         for (c = Math.max(i, 0); c < s; c++) c === f && (t.push(e[c]), o++, f = Math.round(i + o * n))
     }
 
-    function Pqe(e) {
+    function Eqe(e) {
         const t = e.length;
         let n, r;
         if (t < 2) return !1;
         for (r = e[0], n = 1; n < t; ++n)
             if (e[n] - e[n - 1] !== r) return !1;
         return r
     }
-    const Eqe = e => e === "left" ? "right" : e === "right" ? "left" : e,
+    const xqe = e => e === "left" ? "right" : e === "right" ? "left" : e,
         KF = (e, t, n) => t === "top" || t === "left" ? e[t] + n : e[t] - n,
         XF = (e, t) => Math.min(t || e, e);
 
     function JF(e, t) {
         const n = [],
             r = e.length / t,
             a = e.length;
         let i = 0;
         for (; i < a; i += r) n.push(e[Math.floor(i)]);
         return n
     }
 
-    function xqe(e, t, n) {
+    function Oqe(e, t, n) {
         const r = e.ticks.length,
             a = Math.min(t, r - 1),
             i = e._startPixel,
             s = e._endPixel,
             o = 1e-6;
         let u = e.getPixelForTick(a),
             c;
         if (!(n && (r === 1 ? c = Math.max(u - i, s - u) : t === 0 ? c = (e.getPixelForTick(1) - u) / 2 : c = (u - e.getPixelForTick(a - 1)) / 2, u += a < t ? c : -c, u < i - o || u > s + o))) return u
     }
 
-    function Oqe(e, t) {
+    function Aqe(e, t) {
         ar(e, n => {
             const r = n.gc,
                 a = r.length / 2;
             let i;
             if (a > t) {
                 for (i = 0; i < a; ++i) delete n.data[r[i]];
                 r.splice(0, a)
@@ -80042,35 +80050,35 @@
     function ZF(e, t) {
         if (!e.display) return 0;
         const n = Na(e.font, t),
             r = Ti(e.padding);
         return (Lr(e.text) ? e.text.length : 1) * n.lineHeight + r.height
     }
 
-    function Aqe(e, t) {
+    function Mqe(e, t) {
         return Gc(e, {
             scale: t,
             type: "scale"
         })
     }
 
-    function Mqe(e, t, n) {
+    function Dqe(e, t, n) {
         return Gc(e, {
             tick: n,
             index: t,
             type: "tick"
         })
     }
 
-    function Dqe(e, t, n) {
+    function Iqe(e, t, n) {
         let r = lA(e);
-        return (n && t !== "right" || !n && t === "right") && (r = Eqe(r)), r
+        return (n && t !== "right" || !n && t === "right") && (r = xqe(r)), r
     }
 
-    function Iqe(e, t, n, r) {
+    function Lqe(e, t, n, r) {
         const {
             top: a,
             left: i,
             bottom: s,
             right: o,
             chart: u
         } = e, {
@@ -80181,17 +80189,17 @@
                 ticks: s
             } = this.options, o = s.sampleSize;
             this.beforeUpdate(), this.maxWidth = t, this.maxHeight = n, this._margins = r = Object.assign({
                 left: 0,
                 right: 0,
                 top: 0,
                 bottom: 0
-            }, r), this.ticks = null, this._labelSizes = null, this._gridLineItems = null, this._labelItems = null, this.beforeSetDimensions(), this.setDimensions(), this.afterSetDimensions(), this._maxLength = this.isHorizontal() ? this.width + r.left + r.right : this.height + r.top + r.bottom, this._dataLimitsCached || (this.beforeDataLimits(), this.determineDataLimits(), this.afterDataLimits(), this._range = U8e(this, i, a), this._dataLimitsCached = !0), this.beforeBuildTicks(), this.ticks = this.buildTicks() || [], this.afterBuildTicks();
+            }, r), this.ticks = null, this._labelSizes = null, this._gridLineItems = null, this._labelItems = null, this.beforeSetDimensions(), this.setDimensions(), this.afterSetDimensions(), this._maxLength = this.isHorizontal() ? this.width + r.left + r.right : this.height + r.top + r.bottom, this._dataLimitsCached || (this.beforeDataLimits(), this.determineDataLimits(), this.afterDataLimits(), this._range = z8e(this, i, a), this._dataLimitsCached = !0), this.beforeBuildTicks(), this.ticks = this.buildTicks() || [], this.afterBuildTicks();
             const u = o < this.ticks.length;
-            this._convertTicksToLabels(u ? JF(this.ticks, o) : this.ticks), this.configure(), this.beforeCalculateLabelRotation(), this.calculateLabelRotation(), this.afterCalculateLabelRotation(), s.display && (s.autoSkip || s.source === "auto") && (this.ticks = Sqe(this, this.ticks), this._labelSizes = null, this.afterAutoSkip()), u && this._convertTicksToLabels(this.ticks), this.beforeFit(), this.fit(), this.afterFit(), this.afterUpdate()
+            this._convertTicksToLabels(u ? JF(this.ticks, o) : this.ticks), this.configure(), this.beforeCalculateLabelRotation(), this.calculateLabelRotation(), this.afterCalculateLabelRotation(), s.display && (s.autoSkip || s.source === "auto") && (this.ticks = kqe(this, this.ticks), this._labelSizes = null, this.afterAutoSkip()), u && this._convertTicksToLabels(this.ticks), this.beforeFit(), this.fit(), this.afterFit(), this.afterUpdate()
         }
         configure() {
             let t = this.options.reverse,
                 n, r;
             this.isHorizontal() ? (n = this.left, r = this.right) : (n = this.top, r = this.bottom, t = !t), this._startPixel = n, this._endPixel = r, this._reversePixels = t, this._length = r - n, this._alignToPixels = this.options.alignToPixels
         }
         afterUpdate() {
@@ -80364,15 +80372,15 @@
                         data: {},
                         gc: []
                     }, k = y.lineHeight, C = x = 0, !Xn(_) && !Lr(_)) C = f_(a, S.data, S.gc, C, _), x = k;
                 else if (Lr(_))
                     for (p = 0, g = _.length; p < g; ++p) E = _[p], !Xn(E) && !Lr(E) && (C = f_(a, S.data, S.gc, C, E), x += k);
                 s.push(C), o.push(x), c = Math.max(C, c), f = Math.max(x, f)
             }
-            Oqe(i, n);
+            Aqe(i, n);
             const A = s.indexOf(c),
                 O = o.indexOf(f),
                 R = F => ({
                     width: s[F] || 0,
                     height: o[F] || 0
                 });
             return {
@@ -80394,15 +80402,15 @@
         getPixelForTick(t) {
             const n = this.ticks;
             return t < 0 || t > n.length - 1 ? null : this.getPixelForValue(n[t].value)
         }
         getPixelForDecimal(t) {
             this._reversePixels && (t = 1 - t);
             const n = this._startPixel + t * this._length;
-            return b8e(this._alignToPixels ? yd(this.chart, n, 0) : n)
+            return _8e(this._alignToPixels ? yd(this.chart, n, 0) : n)
         }
         getDecimalForPixel(t) {
             const n = (t - this._startPixel) / this._length;
             return this._reversePixels ? 1 - n : n
         }
         getBasePixel() {
             return this.getPixelForValue(this.getBaseValue())
@@ -80414,17 +80422,17 @@
             } = this;
             return t < 0 && n < 0 ? n : t > 0 && n > 0 ? t : 0
         }
         getContext(t) {
             const n = this.ticks || [];
             if (t >= 0 && t < n.length) {
                 const r = n[t];
-                return r.$context || (r.$context = Mqe(this.getContext(), t, r))
+                return r.$context || (r.$context = Dqe(this.getContext(), t, r))
             }
-            return this.$context || (this.$context = Aqe(this.chart.getContext(), this))
+            return this.$context || (this.$context = Mqe(this.chart.getContext(), this))
         }
         _tickSize() {
             const t = this.options.ticks,
                 n = _o(this.labelRotation),
                 r = Math.abs(Math.cos(n)),
                 a = Math.abs(Math.sin(n)),
                 i = this._getLabelSizes(),
@@ -80489,15 +80497,15 @@
                     X = se.color,
                     N = ue.dash || [],
                     q = ue.dashOffset,
                     M = se.tickWidth,
                     P = se.tickColor,
                     L = se.tickBorderDash || [],
                     H = se.tickBorderDashOffset;
-                x = xqe(this, C, u), x !== void 0 && (E = yd(r, x, he), c ? A = R = U = B = E : O = F = G = W = E, g.push({
+                x = Oqe(this, C, u), x !== void 0 && (E = yd(r, x, he), c ? A = R = U = B = E : O = F = G = W = E, g.push({
                     tx1: A,
                     ty1: O,
                     tx2: R,
                     ty2: F,
                     x1: U,
                     y1: G,
                     x2: B,
@@ -80761,20 +80769,20 @@
             let u = i.lineHeight / 2;
             n === "bottom" || n === "center" || Tn(n) ? (u += s.bottom, Lr(r.text) && (u += i.lineHeight * (r.text.length - 1))) : u += s.top;
             const {
                 titleX: c,
                 titleY: f,
                 maxWidth: h,
                 rotation: p
-            } = Iqe(this, u, n, o);
+            } = Lqe(this, u, n, o);
             cf(t, r.text, 0, 0, i, {
                 color: r.color,
                 maxWidth: h,
                 rotation: p,
-                textAlign: Dqe(o, n, a),
+                textAlign: Iqe(o, n, a),
                 textBaseline: "middle",
                 translation: [c, f]
             })
         }
         draw(t) {
             this._isVisible() && (this.drawBackground(), this.drawGrid(t), this.drawBorder(), this.drawTitle(), this.drawLabels(t))
         }
@@ -80831,53 +80839,53 @@
         }
         isForType(t) {
             return Object.prototype.isPrototypeOf.call(this.type.prototype, t.prototype)
         }
         register(t) {
             const n = Object.getPrototypeOf(t);
             let r;
-            Nqe(n) && (r = this.register(n));
+            Fqe(n) && (r = this.register(n));
             const a = this.items,
                 i = t.id,
                 s = this.scope + "." + i;
             if (!i) throw new Error("class does not have id: " + t);
-            return i in a || (a[i] = t, Lqe(t, s, r), this.override && na.override(t.id, t.overrides)), s
+            return i in a || (a[i] = t, Rqe(t, s, r), this.override && na.override(t.id, t.overrides)), s
         }
         get(t) {
             return this.items[t]
         }
         unregister(t) {
             const n = this.items,
                 r = t.id,
                 a = this.scope;
             r in n && delete n[r], a && r in na[a] && (delete na[a][r], this.override && delete uf[r])
         }
     }
 
-    function Lqe(e, t, n) {
+    function Rqe(e, t, n) {
         const r = Zv(Object.create(null), [n ? na.get(n) : {}, na.get(t), e.defaults]);
-        na.set(t, r), e.defaultRoutes && Rqe(t, e.defaultRoutes), e.descriptors && na.describe(t, e.descriptors)
+        na.set(t, r), e.defaultRoutes && Nqe(t, e.defaultRoutes), e.descriptors && na.describe(t, e.descriptors)
     }
 
-    function Rqe(e, t) {
+    function Nqe(e, t) {
         Object.keys(t).forEach(n => {
             const r = n.split("."),
                 a = r.pop(),
                 i = [e].concat(r).join("."),
                 s = t[n].split("."),
                 o = s.pop(),
                 u = s.join(".");
             na.route(i, a, u, o)
         })
     }
 
-    function Nqe(e) {
+    function Fqe(e) {
         return "id" in e && "defaults" in e
     }
-    class Fqe {
+    class Vqe {
         constructor() {
             this.controllers = new v0(Co, "datasets", !0), this.elements = new v0(Kc, "elements"), this.plugins = new v0(Object, "plugins"), this.scales = new v0(kf, "scales"), this._typedRegistries = [this.controllers, this.scales, this.elements]
         }
         add(...t) {
             this._each("register", t)
         }
         remove(...t) {
@@ -80941,16 +80949,16 @@
         }
         _get(t, n, r) {
             const a = n.get(t);
             if (a === void 0) throw new Error('"' + t + '" is not a registered ' + r + ".");
             return a
         }
     }
-    var Ko = new Fqe;
-    class Vqe {
+    var Ko = new Vqe;
+    class jqe {
         constructor() {
             this._init = []
         }
         notify(t, n, r, a) {
             n === "beforeInit" && (this._init = this._createDescriptors(t, !0), this._notify(this._init, t, "install"));
             const i = a ? this._descriptors(t).filter(a) : this._descriptors(t),
                 s = this._notify(i, t, n, r);
@@ -80973,26 +80981,26 @@
             if (this._cache) return this._cache;
             const n = this._cache = this._createDescriptors(t);
             return this._notifyStateChanges(t), n
         }
         _createDescriptors(t, n) {
             const r = t && t.config,
                 a = un(r.options && r.options.plugins, {}),
-                i = jqe(r);
-            return a === !1 && !n ? [] : Hqe(t, i, a, n)
+                i = Bqe(r);
+            return a === !1 && !n ? [] : Wqe(t, i, a, n)
         }
         _notifyStateChanges(t) {
             const n = this._oldCache || [],
                 r = this._cache,
                 a = (i, s) => i.filter(o => !s.some(u => o.plugin.id === u.plugin.id));
             this._notify(a(n, r), t, "stop"), this._notify(a(r, n), t, "start")
         }
     }
 
-    function jqe(e) {
+    function Bqe(e) {
         const t = {},
             n = [],
             r = Object.keys(Ko.plugins.items);
         for (let i = 0; i < r.length; i++) n.push(Ko.getPlugin(r[i]));
         const a = e.plugins || [];
         for (let i = 0; i < a.length; i++) {
             const s = a[i];
@@ -81000,39 +81008,39 @@
         }
         return {
             plugins: n,
             localIds: t
         }
     }
 
-    function Bqe(e, t) {
+    function Hqe(e, t) {
         return !t && e === !1 ? null : e === !0 ? {} : e
     }
 
-    function Hqe(e, {
+    function Wqe(e, {
         plugins: t,
         localIds: n
     }, r, a) {
         const i = [],
             s = e.getContext();
         for (const o of t) {
             const u = o.id,
-                c = Bqe(r[u], a);
+                c = Hqe(r[u], a);
             c !== null && i.push({
                 plugin: o,
-                options: Wqe(e.config, {
+                options: Uqe(e.config, {
                     plugin: o,
                     local: n[u]
                 }, c, s)
             })
         }
         return i
     }
 
-    function Wqe(e, {
+    function Uqe(e, {
         plugin: t,
         local: n
     }, r, a) {
         const i = e.pluginScopeKeys(t),
             s = e.getOptionScopes(r, i);
         return n && t.defaults && s.push(t.defaults), e.createResolver(s, a, [""], {
             scriptable: !1,
@@ -81042,115 +81050,115 @@
     }
 
     function WC(e, t) {
         const n = na.datasets[e] || {};
         return ((t.datasets || {})[e] || {}).indexAxis || t.indexAxis || n.indexAxis || "x"
     }
 
-    function Uqe(e, t) {
+    function zqe(e, t) {
         let n = e;
         return e === "_index_" ? n = t : e === "_value_" && (n = t === "x" ? "y" : "x"), n
     }
 
-    function zqe(e, t) {
+    function Yqe(e, t) {
         return e === t ? "_index_" : "_value_"
     }
 
     function QF(e) {
         if (e === "x" || e === "y" || e === "r") return e
     }
 
-    function Yqe(e) {
+    function qqe(e) {
         if (e === "top" || e === "bottom") return "x";
         if (e === "left" || e === "right") return "y"
     }
 
     function UC(e, ...t) {
         if (QF(e)) return e;
         for (const n of t) {
-            const r = n.axis || Yqe(n.position) || e.length > 1 && QF(e[0].toLowerCase());
+            const r = n.axis || qqe(n.position) || e.length > 1 && QF(e[0].toLowerCase());
             if (r) return r
         }
         throw new Error(`Cannot determine type of '${e}' axis. Please provide 'axis' or 'position' option.`)
     }
 
     function eV(e, t, n) {
         if (n[t + "AxisID"] === e) return {
             axis: t
         }
     }
 
-    function qqe(e, t) {
+    function Gqe(e, t) {
         if (t.data && t.data.datasets) {
             const n = t.data.datasets.filter(r => r.xAxisID === e || r.yAxisID === e);
             if (n.length) return eV(e, "x", n[0]) || eV(e, "y", n[0])
         }
         return {}
     }
 
-    function Gqe(e, t) {
+    function Kqe(e, t) {
         const n = uf[e.type] || {
                 scales: {}
             },
             r = t.scales || {},
             a = WC(e.type, t),
             i = Object.create(null);
         return Object.keys(r).forEach(s => {
             const o = r[s];
             if (!Tn(o)) return console.error(`Invalid scale configuration for scale: ${s}`);
             if (o._proxy) return console.warn(`Ignoring resolver passed as options for scale: ${s}`);
-            const u = UC(s, o, qqe(s, e), na.scales[o.type]),
-                c = zqe(u, a),
+            const u = UC(s, o, Gqe(s, e), na.scales[o.type]),
+                c = Yqe(u, a),
                 f = n.scales || {};
             i[s] = fv(Object.create(null), [{
                 axis: u
             }, o, f[u], f[c]])
         }), e.data.datasets.forEach(s => {
             const o = s.type || e.type,
                 u = s.indexAxis || WC(o, t),
                 f = (uf[o] || {}).scales || {};
             Object.keys(f).forEach(h => {
-                const p = Uqe(h, u),
+                const p = zqe(h, u),
                     g = s[p + "AxisID"] || p;
                 i[g] = i[g] || Object.create(null), fv(i[g], [{
                     axis: p
                 }, r[g], f[h]])
             })
         }), Object.keys(i).forEach(s => {
             const o = i[s];
             fv(o, [na.scales[o.type], na.scale])
         }), i
     }
 
     function zY(e) {
         const t = e.options || (e.options = {});
-        t.plugins = un(t.plugins, {}), t.scales = Gqe(e, t)
+        t.plugins = un(t.plugins, {}), t.scales = Kqe(e, t)
     }
 
     function YY(e) {
         return e = e || {}, e.datasets = e.datasets || [], e.labels = e.labels || [], e
     }
 
-    function Kqe(e) {
+    function Xqe(e) {
         return e = e || {}, e.data = YY(e.data), zY(e), e
     }
     const tV = new Map,
         qY = new Set;
 
     function g0(e, t) {
         let n = tV.get(e);
         return n || (n = t(), tV.set(e, n), qY.add(n)), n
     }
     const Lm = (e, t, n) => {
         const r = Oc(t, n);
         r !== void 0 && e.add(r)
     };
-    class Xqe {
+    class Jqe {
         constructor(t) {
-            this._config = Kqe(t), this._scopeCache = new Map, this._resolverCache = new Map
+            this._config = Xqe(t), this._scopeCache = new Map, this._resolverCache = new Map
         }
         get platform() {
             return this._config.platform
         }
         get type() {
             return this._config.type
         }
@@ -81234,15 +81242,15 @@
                     $shared: !0
                 },
                 {
                     resolver: s,
                     subPrefixes: o
                 } = nV(this._resolverCache, t, a);
             let u = s;
-            if (Zqe(s, n)) {
+            if (Qqe(s, n)) {
                 i.$shared = !1, r = Ac(r) ? r() : r;
                 const c = this.createResolver(t, r, o);
                 u = op(s, r, c)
             }
             for (const c of n) i[c] = u[c];
             return i
         }
@@ -81260,83 +81268,83 @@
         const a = n.join();
         let i = r.get(a);
         return i || (i = {
             resolver: cA(t, n),
             subPrefixes: n.filter(o => !o.toLowerCase().includes("hover"))
         }, r.set(a, i)), i
     }
-    const Jqe = e => Tn(e) && Object.getOwnPropertyNames(e).some(t => Ac(e[t]));
+    const Zqe = e => Tn(e) && Object.getOwnPropertyNames(e).some(t => Ac(e[t]));
 
-    function Zqe(e, t) {
+    function Qqe(e, t) {
         const {
             isScriptable: n,
             isIndexable: r
         } = TY(e);
         for (const a of t) {
             const i = n(a),
                 s = r(a),
                 o = (s || i) && e[a];
-            if (i && (Ac(o) || Jqe(o)) || s && Lr(o)) return !0
+            if (i && (Ac(o) || Zqe(o)) || s && Lr(o)) return !0
         }
         return !1
     }
-    var Qqe = "4.4.3";
-    const eGe = ["top", "bottom", "left", "right", "chartArea"];
+    var eGe = "4.4.3";
+    const tGe = ["top", "bottom", "left", "right", "chartArea"];
 
     function rV(e, t) {
-        return e === "top" || e === "bottom" || eGe.indexOf(e) === -1 && t === "x"
+        return e === "top" || e === "bottom" || tGe.indexOf(e) === -1 && t === "x"
     }
 
     function aV(e, t) {
         return function(n, r) {
             return n[e] === r[e] ? n[t] - r[t] : n[e] - r[e]
         }
     }
 
     function iV(e) {
         const t = e.chart,
             n = t.options.animation;
         t.notifyPlugins("afterRender"), mr(n && n.onComplete, [e], t)
     }
 
-    function tGe(e) {
+    function nGe(e) {
         const t = e.chart,
             n = t.options.animation;
         mr(n && n.onProgress, [e], t)
     }
 
     function GY(e) {
         return hA() && typeof e == "string" ? e = document.getElementById(e) : e && e.length && (e = e[0]), e && e.canvas && (e = e.canvas), e
     }
     const ab = {},
         sV = e => {
             const t = GY(e);
             return Object.values(ab).filter(n => n.canvas === t).pop()
         };
 
-    function nGe(e, t, n) {
+    function rGe(e, t, n) {
         const r = Object.keys(e);
         for (const a of r) {
             const i = +a;
             if (i >= t) {
                 const s = e[a];
                 delete e[a], (n > 0 || i > t) && (e[i + n] = s)
             }
         }
     }
 
-    function rGe(e, t, n, r) {
+    function aGe(e, t, n, r) {
         return !n || e.type === "mouseout" ? null : r ? t : e
     }
 
     function y0(e, t, n) {
         return e.options.clip ? e[n] : t[n]
     }
 
-    function aGe(e, t) {
+    function iGe(e, t) {
         const {
             xScale: n,
             yScale: r
         } = e;
         return n && r ? {
             left: y0(n, t, "left"),
             right: y0(n, t, "right"),
@@ -81349,29 +81357,29 @@
         static register(...t) {
             Ko.add(...t), oV()
         }
         static unregister(...t) {
             Ko.remove(...t), oV()
         }
         constructor(t, n) {
-            const r = this.config = new Xqe(n),
+            const r = this.config = new Jqe(n),
                 a = GY(t),
                 i = sV(a);
             if (i) throw new Error("Canvas is already in use. Chart with ID '" + i.id + "' must be destroyed before the canvas with ID '" + i.canvas.id + "' can be reused.");
             const s = r.createResolver(r.chartOptionScopes(), this.getContext());
-            this.platform = new(r.platform || wqe(a)), this.platform.updateConfig(r);
+            this.platform = new(r.platform || Sqe(a)), this.platform.updateConfig(r);
             const o = this.platform.acquireContext(a, s.aspectRatio),
                 u = o && o.canvas,
                 c = u && u.height,
                 f = u && u.width;
-            if (this.id = s8e(), this.ctx = o, this.canvas = u, this.width = f, this.height = c, this._options = s, this._aspectRatio = this.aspectRatio, this._layers = [], this._metasets = [], this._stacks = void 0, this.boxes = [], this.currentDevicePixelRatio = void 0, this.chartArea = void 0, this._active = [], this._lastEvent = void 0, this._listeners = {}, this._responsiveListeners = void 0, this._sortedMetasets = [], this.scales = {}, this._plugins = new Vqe, this.$proxies = {}, this._hiddenIndices = {}, this.attached = !1, this._animationsDisabled = void 0, this.$context = void 0, this._doResize = k8e(h => this.update(h), s.resizeDelay || 0), this._dataChanges = [], ab[this.id] = this, !o || !u) {
+            if (this.id = o8e(), this.ctx = o, this.canvas = u, this.width = f, this.height = c, this._options = s, this._aspectRatio = this.aspectRatio, this._layers = [], this._metasets = [], this._stacks = void 0, this.boxes = [], this.currentDevicePixelRatio = void 0, this.chartArea = void 0, this._active = [], this._lastEvent = void 0, this._listeners = {}, this._responsiveListeners = void 0, this._sortedMetasets = [], this.scales = {}, this._plugins = new jqe, this.$proxies = {}, this._hiddenIndices = {}, this.attached = !1, this._animationsDisabled = void 0, this.$context = void 0, this._doResize = $8e(h => this.update(h), s.resizeDelay || 0), this._dataChanges = [], ab[this.id] = this, !o || !u) {
                 console.error("Failed to create chart: can't acquire context from the given item");
                 return
             }
-            Ul.listen(this, "complete", iV), Ul.listen(this, "progress", tGe), this._initialize(), this.attached && this.update()
+            Ul.listen(this, "complete", iV), Ul.listen(this, "progress", nGe), this._initialize(), this.attached && this.update()
         }
         get aspectRatio() {
             const {
                 options: {
                     aspectRatio: t,
                     maintainAspectRatio: n
                 },
@@ -81567,15 +81575,15 @@
             for (const {
                     method: r,
                     start: a,
                     count: i
                 }
                 of n) {
                 const s = r === "_removeElements" ? -i : i;
-                nGe(t, a, s)
+                rGe(t, a, s)
             }
         }
         _getUniformDataChanges() {
             const t = this._dataChanges;
             if (!t || !t.length) return;
             this._dataChanges = [];
             const n = this.data.datasets.length,
@@ -81671,15 +81679,15 @@
             for (let n = t.length - 1; n >= 0; --n) this._drawDataset(t[n]);
             this.notifyPlugins("afterDatasetsDraw")
         }
         _drawDataset(t) {
             const n = this.ctx,
                 r = t._clip,
                 a = !r.disabled,
-                i = aGe(t, this.chartArea),
+                i = iGe(t, this.chartArea),
                 s = {
                     meta: t,
                     index: t.index,
                     cancelable: !0
                 };
             this.notifyPlugins("beforeDatasetDraw", s) !== !1 && (a && uw(n, {
                 left: r.left === !1 ? 0 : i.left - r.left,
@@ -81688,15 +81696,15 @@
                 bottom: r.bottom === !1 ? this.height : i.bottom + r.bottom
             }), t.controller.draw(), a && cw(n), s.cancelable = !1, this.notifyPlugins("afterDatasetDraw", s))
         }
         isPointInArea(t) {
             return eu(t, this.chartArea, this._minPadding)
         }
         getElementsAtEventForMode(t, n, r, a) {
-            const i = eqe.modes[n];
+            const i = tqe.modes[n];
             return typeof i == "function" ? i(this, t, r, a) : []
         }
         getDatasetMeta(t) {
             const n = this.data.datasets[t],
                 r = this._metasets;
             let a = r.filter(i => i && i._dataset === n).pop();
             return a || (a = {
@@ -81867,41 +81875,41 @@
             const i = this._handleEvent(t, n, r.inChartArea);
             return r.cancelable = !1, this.notifyPlugins("afterEvent", r, a), (i || r.changed) && this.render(), this
         }
         _handleEvent(t, n, r) {
             const {
                 _active: a = [],
                 options: i
-            } = this, s = n, o = this._getActiveElements(t, a, r, s), u = f8e(t), c = rGe(t, this._lastEvent, r, u);
+            } = this, s = n, o = this._getActiveElements(t, a, r, s), u = h8e(t), c = aGe(t, this._lastEvent, r, u);
             r && (this._lastEvent = null, mr(i.onHover, [t, o, this], this), u && mr(i.onClick, [t, o, this], this));
             const f = !l_(o, a);
             return (f || n) && (this._active = o, this._updateHoverStyles(o, a, n)), this._lastEvent = c, f
         }
         _getActiveElements(t, n, r, a) {
             if (t.type === "mouseout") return [];
             if (!r) return n;
             const i = this.options.hover;
             return this.getElementsAtEventForMode(t, i.mode, i, a)
         }
-    }, Ye(Yu, "defaults", na), Ye(Yu, "instances", ab), Ye(Yu, "overrides", uf), Ye(Yu, "registry", Ko), Ye(Yu, "version", Qqe), Ye(Yu, "getChart", sV), Yu);
+    }, Ye(Yu, "defaults", na), Ye(Yu, "instances", ab), Ye(Yu, "overrides", uf), Ye(Yu, "registry", Ko), Ye(Yu, "version", eGe), Ye(Yu, "getChart", sV), Yu);
 
     function oV() {
         return ar(fw.instances, e => e._plugins.invalidate())
     }
 
     function KY(e, t, n = t) {
         e.lineCap = un(n.borderCapStyle, t.borderCapStyle), e.setLineDash(un(n.borderDash, t.borderDash)), e.lineDashOffset = un(n.borderDashOffset, t.borderDashOffset), e.lineJoin = un(n.borderJoinStyle, t.borderJoinStyle), e.lineWidth = un(n.borderWidth, t.borderWidth), e.strokeStyle = un(n.borderColor, t.borderColor)
     }
 
-    function iGe(e, t, n) {
+    function sGe(e, t, n) {
         e.lineTo(n.x, n.y)
     }
 
-    function sGe(e) {
-        return e.stepped ? L8e : e.tension || e.cubicInterpolationMode === "monotone" ? R8e : iGe
+    function oGe(e) {
+        return e.stepped ? R8e : e.tension || e.cubicInterpolationMode === "monotone" ? N8e : sGe
     }
 
     function XY(e, t, n = {}) {
         const r = e.length,
             {
                 start: a = 0,
                 end: i = r - 1
@@ -81917,33 +81925,33 @@
             count: r,
             start: u,
             loop: t.loop,
             ilen: c < u && !f ? r + c - u : c - u
         }
     }
 
-    function oGe(e, t, n, r) {
+    function lGe(e, t, n, r) {
         const {
             points: a,
             options: i
         } = t, {
             count: s,
             start: o,
             loop: u,
             ilen: c
-        } = XY(a, n, r), f = sGe(i);
+        } = XY(a, n, r), f = oGe(i);
         let {
             move: h = !0,
             reverse: p
         } = r || {}, g, _, y;
         for (g = 0; g <= c; ++g) _ = a[(o + (p ? c - g : g)) % s], !_.skip && (h ? (e.moveTo(_.x, _.y), h = !1) : f(e, y, _, p, i.stepped), y = _);
         return u && (_ = a[(o + (p ? c : 0)) % s], f(e, y, _, p, i.stepped)), !!u
     }
 
-    function lGe(e, t, n, r) {
+    function uGe(e, t, n, r) {
         const a = t.points,
             {
                 count: i,
                 start: s,
                 ilen: o
             } = XY(a, n, r),
             {
@@ -81966,60 +81974,60 @@
         }
         C()
     }
 
     function zC(e) {
         const t = e.options,
             n = t.borderDash && t.borderDash.length;
-        return !e._decimated && !e._loop && !t.tension && t.cubicInterpolationMode !== "monotone" && !t.stepped && !n ? lGe : oGe
+        return !e._decimated && !e._loop && !t.tension && t.cubicInterpolationMode !== "monotone" && !t.stepped && !n ? uGe : lGe
     }
 
-    function uGe(e) {
-        return e.stepped ? pYe : e.tension || e.cubicInterpolationMode === "monotone" ? mYe : Cd
+    function cGe(e) {
+        return e.stepped ? mYe : e.tension || e.cubicInterpolationMode === "monotone" ? vYe : Cd
     }
 
-    function cGe(e, t, n, r) {
+    function dGe(e, t, n, r) {
         let a = t._path;
         a || (a = t._path = new Path2D, t.path(a, n, r) && a.closePath()), KY(e, t.options), e.stroke(a)
     }
 
-    function dGe(e, t, n, r) {
+    function fGe(e, t, n, r) {
         const {
             segments: a,
             options: i
         } = t, s = zC(t);
         for (const o of a) KY(e, i, o.style), e.beginPath(), s(e, t, o, {
             start: n,
             end: n + r - 1
         }) && e.closePath(), e.stroke()
     }
-    const fGe = typeof Path2D == "function";
+    const hGe = typeof Path2D == "function";
 
-    function hGe(e, t, n, r) {
-        fGe && !t.options.segment ? cGe(e, t, n, r) : dGe(e, t, n, r)
+    function pGe(e, t, n, r) {
+        hGe && !t.options.segment ? dGe(e, t, n, r) : fGe(e, t, n, r)
     }
     class cc extends Kc {
         constructor(t) {
             super(), this.animated = !0, this.options = void 0, this._chart = void 0, this._loop = void 0, this._fullLoop = void 0, this._path = void 0, this._points = void 0, this._segments = void 0, this._decimated = !1, this._pointsUpdated = !1, this._datasetIndex = void 0, t && Object.assign(this, t)
         }
         updateControlPoints(t, n) {
             const r = this.options;
             if ((r.tension || r.cubicInterpolationMode === "monotone") && !r.stepped && !this._pointsUpdated) {
                 const a = r.spanGaps ? this._loop : this._fullLoop;
-                sYe(this._points, r, t, a, n), this._pointsUpdated = !0
+                oYe(this._points, r, t, a, n), this._pointsUpdated = !0
             }
         }
         set points(t) {
             this._points = t, delete this._segments, delete this._path, this._pointsUpdated = !1
         }
         get points() {
             return this._points
         }
         get segments() {
-            return this._segments || (this._segments = wYe(this, this.options.segment))
+            return this._segments || (this._segments = SYe(this, this.options.segment))
         }
         first() {
             const t = this.segments,
                 n = this.points;
             return t.length && n[t[0].start]
         }
         last() {
@@ -82035,15 +82043,15 @@
                 s = RY(this, {
                     property: n,
                     start: a,
                     end: a
                 });
             if (!s.length) return;
             const o = [],
-                u = uGe(r);
+                u = cGe(r);
             let c, f;
             for (c = 0, f = s.length; c < f; ++c) {
                 const {
                     start: h,
                     end: p
                 } = s[c], g = i[h], _ = i[p];
                 if (g === _) {
@@ -82068,15 +82076,15 @@
                 start: n,
                 end: n + r - 1
             });
             return !!s
         }
         draw(t, n, r, a) {
             const i = this.options || {};
-            (this.points || []).length && i.borderWidth && (t.save(), hGe(t, this, r, a), t.restore()), this.animated && (this._pointsUpdated = !1, this._path = void 0)
+            (this.points || []).length && i.borderWidth && (t.save(), pGe(t, this, r, a), t.restore()), this.animated && (this._pointsUpdated = !1, this._path = void 0)
         }
     }
     Ye(cc, "id", "line"), Ye(cc, "defaults", {
         borderCapStyle: "butt",
         borderDash: [],
         borderDashOffset: 0,
         borderJoinStyle: "miter",
@@ -82180,44 +82188,44 @@
         }
     }
 
     function dc(e, t, n, r) {
         return e ? 0 : ks(t, n, r)
     }
 
-    function pGe(e, t, n) {
+    function mGe(e, t, n) {
         const r = e.options.borderWidth,
             a = e.borderSkipped,
             i = CY(r);
         return {
             t: dc(a.top, i.top, 0, n),
             r: dc(a.right, i.right, 0, t),
             b: dc(a.bottom, i.bottom, 0, n),
             l: dc(a.left, i.left, 0, t)
         }
     }
 
-    function mGe(e, t, n) {
+    function vGe(e, t, n) {
         const {
             enableBorderRadius: r
         } = e.getProps(["enableBorderRadius"]), a = e.options.borderRadius, i = Xd(a), s = Math.min(t, n), o = e.borderSkipped, u = r || Tn(a);
         return {
             topLeft: dc(!u || o.top || o.left, i.topLeft, 0, s),
             topRight: dc(!u || o.top || o.right, i.topRight, 0, s),
             bottomLeft: dc(!u || o.bottom || o.left, i.bottomLeft, 0, s),
             bottomRight: dc(!u || o.bottom || o.right, i.bottomRight, 0, s)
         }
     }
 
-    function vGe(e) {
+    function gGe(e) {
         const t = JY(e),
             n = t.right - t.left,
             r = t.bottom - t.top,
-            a = pGe(e, n / 2, r / 2),
-            i = mGe(e, n / 2, r / 2);
+            a = mGe(e, n / 2, r / 2),
+            i = vGe(e, n / 2, r / 2);
         return {
             outer: {
                 x: t.left,
                 y: t.top,
                 w: n,
                 h: r,
                 radius: i
@@ -82240,19 +82248,19 @@
     function Nk(e, t, n, r) {
         const a = t === null,
             i = n === null,
             o = e && !(a && i) && JY(e, r);
         return o && (a || uc(t, o.left, o.right)) && (i || uc(n, o.top, o.bottom))
     }
 
-    function gGe(e) {
+    function yGe(e) {
         return e.topLeft || e.topRight || e.bottomLeft || e.bottomRight
     }
 
-    function yGe(e, t) {
+    function bGe(e, t) {
         e.rect(t.x, t.y, t.w, t.h)
     }
 
     function Fk(e, t, n = {}) {
         const r = e.x !== n.x ? -t : 0,
             a = e.y !== n.y ? -t : 0,
             i = (e.x + e.w !== n.x + n.w ? t : 0) - r,
@@ -82275,15 +82283,15 @@
                 options: {
                     borderColor: r,
                     backgroundColor: a
                 }
             } = this, {
                 inner: i,
                 outer: s
-            } = vGe(this), o = gGe(s.radius) ? eg : yGe;
+            } = gGe(this), o = yGe(s.radius) ? eg : bGe;
             t.save(), (s.w !== i.w || s.h !== i.h) && (t.beginPath(), o(t, Fk(s, n, i)), t.clip(), o(t, Fk(i, -n, s)), t.fillStyle = r, t.fill("evenodd")), t.beginPath(), o(t, Fk(i, n)), t.fillStyle = a, t.fill(), t.restore()
         }
         inRange(t, n, r) {
             return Nk(this, t, n, r)
         }
         inXRange(t, n) {
             return Nk(this, t, null, n)
@@ -82314,15 +82322,15 @@
         inflateAmount: "auto",
         pointStyle: void 0
     }), Ye(sb, "defaultRoutes", {
         backgroundColor: "backgroundColor",
         borderColor: "borderColor"
     });
 
-    function bGe(e, t, n) {
+    function _Ge(e, t, n) {
         const r = e.segments,
             a = e.points,
             i = t.points,
             s = [];
         for (const o of r) {
             let {
                 start: u,
@@ -82365,15 +82373,15 @@
         return e === "angle" && (a = bs(a), i = bs(i)), {
             property: e,
             start: a,
             end: i
         }
     }
 
-    function _Ge(e, t) {
+    function wGe(e, t) {
         const {
             x: n = null,
             y: r = null
         } = e || {}, a = t.points, i = [];
         return t.segments.forEach(({
             start: s,
             end: o
@@ -82408,119 +82416,119 @@
     function uV(e, t, n, r) {
         return e && t ? r(e[n], t[n]) : e ? e[n] : t ? t[n] : 0
     }
 
     function ZY(e, t) {
         let n = [],
             r = !1;
-        return Lr(e) ? (r = !0, n = e) : n = _Ge(e, t), n.length ? new cc({
+        return Lr(e) ? (r = !0, n = e) : n = wGe(e, t), n.length ? new cc({
             points: n,
             options: {
                 tension: 0
             },
             _loop: r,
             _fullLoop: r
         }) : null
     }
 
     function cV(e) {
         return e && e.fill !== !1
     }
 
-    function wGe(e, t, n) {
+    function SGe(e, t, n) {
         let a = e[t].fill;
         const i = [t];
         let s;
         if (!n) return a;
         for (; a !== !1 && i.indexOf(a) === -1;) {
             if (!ta(a)) return a;
             if (s = e[a], !s) return !1;
             if (s.visible) return a;
             i.push(a), a = s.fill
         }
         return !1
     }
 
-    function SGe(e, t, n) {
-        const r = TGe(e);
+    function kGe(e, t, n) {
+        const r = PGe(e);
         if (Tn(r)) return isNaN(r.value) ? !1 : r;
         let a = parseFloat(r);
-        return ta(a) && Math.floor(a) === a ? kGe(r[0], t, a, n) : ["origin", "start", "end", "stack", "shape"].indexOf(r) >= 0 && r
+        return ta(a) && Math.floor(a) === a ? $Ge(r[0], t, a, n) : ["origin", "start", "end", "stack", "shape"].indexOf(r) >= 0 && r
     }
 
-    function kGe(e, t, n, r) {
+    function $Ge(e, t, n, r) {
         return (e === "-" || e === "+") && (n = t + n), n === t || n < 0 || n >= r ? !1 : n
     }
 
-    function $Ge(e, t) {
+    function CGe(e, t) {
         let n = null;
         return e === "start" ? n = t.bottom : e === "end" ? n = t.top : Tn(e) ? n = t.getPixelForValue(e.value) : t.getBasePixel && (n = t.getBasePixel()), n
     }
 
-    function CGe(e, t, n) {
+    function TGe(e, t, n) {
         let r;
         return e === "start" ? r = n : e === "end" ? r = t.options.reverse ? t.min : t.max : Tn(e) ? r = e.value : r = t.getBaseValue(), r
     }
 
-    function TGe(e) {
+    function PGe(e) {
         const t = e.options,
             n = t.fill;
         let r = un(n && n.target, n);
         return r === void 0 && (r = !!t.backgroundColor), r === !1 || r === null ? !1 : r === !0 ? "origin" : r
     }
 
-    function PGe(e) {
+    function EGe(e) {
         const {
             scale: t,
             index: n,
             line: r
-        } = e, a = [], i = r.segments, s = r.points, o = EGe(t, n);
+        } = e, a = [], i = r.segments, s = r.points, o = xGe(t, n);
         o.push(ZY({
             x: null,
             y: t.bottom
         }, r));
         for (let u = 0; u < i.length; u++) {
             const c = i[u];
-            for (let f = c.start; f <= c.end; f++) xGe(a, s[f], o)
+            for (let f = c.start; f <= c.end; f++) OGe(a, s[f], o)
         }
         return new cc({
             points: a,
             options: {}
         })
     }
 
-    function EGe(e, t) {
+    function xGe(e, t) {
         const n = [],
             r = e.getMatchingVisibleMetas("line");
         for (let a = 0; a < r.length; a++) {
             const i = r[a];
             if (i.index === t) break;
             i.hidden || n.unshift(i.dataset)
         }
         return n
     }
 
-    function xGe(e, t, n) {
+    function OGe(e, t, n) {
         const r = [];
         for (let a = 0; a < n.length; a++) {
             const i = n[a],
                 {
                     first: s,
                     last: o,
                     point: u
-                } = OGe(i, t, "x");
+                } = AGe(i, t, "x");
             if (!(!u || s && o)) {
                 if (s) r.unshift(u);
                 else if (e.push(u), !o) break
             }
         }
         e.push(...r)
     }
 
-    function OGe(e, t, n) {
+    function AGe(e, t, n) {
         const r = e.interpolate(t, n);
         if (!r) return {};
         const a = r[n],
             i = e.segments,
             s = e.points;
         let o = !1,
             u = !1;
@@ -82564,94 +82572,94 @@
                 x: n + Math.cos(i) * a,
                 y: r + Math.sin(i) * a,
                 angle: i
             }
         }
     }
 
-    function AGe(e) {
+    function MGe(e) {
         const {
             chart: t,
             fill: n,
             line: r
         } = e;
-        if (ta(n)) return MGe(t, n);
-        if (n === "stack") return PGe(e);
+        if (ta(n)) return DGe(t, n);
+        if (n === "stack") return EGe(e);
         if (n === "shape") return !0;
-        const a = DGe(e);
+        const a = IGe(e);
         return a instanceof QY ? a : ZY(a, r)
     }
 
-    function MGe(e, t) {
+    function DGe(e, t) {
         const n = e.getDatasetMeta(t);
         return n && e.isDatasetVisible(t) ? n.dataset : null
     }
 
-    function DGe(e) {
-        return (e.scale || {}).getPointPositionForValue ? LGe(e) : IGe(e)
+    function IGe(e) {
+        return (e.scale || {}).getPointPositionForValue ? RGe(e) : LGe(e)
     }
 
-    function IGe(e) {
+    function LGe(e) {
         const {
             scale: t = {},
             fill: n
-        } = e, r = $Ge(n, t);
+        } = e, r = CGe(n, t);
         if (ta(r)) {
             const a = t.isHorizontal();
             return {
                 x: a ? r : null,
                 y: a ? null : r
             }
         }
         return null
     }
 
-    function LGe(e) {
+    function RGe(e) {
         const {
             scale: t,
             fill: n
-        } = e, r = t.options, a = t.getLabels().length, i = r.reverse ? t.max : t.min, s = CGe(n, t, i), o = [];
+        } = e, r = t.options, a = t.getLabels().length, i = r.reverse ? t.max : t.min, s = TGe(n, t, i), o = [];
         if (r.grid.circular) {
             const u = t.getPointPositionForValue(0, i);
             return new QY({
                 x: u.x,
                 y: u.y,
                 radius: t.getDistanceFromCenterForValue(s)
             })
         }
         for (let u = 0; u < a; ++u) o.push(t.getPointPositionForValue(u, s));
         return o
     }
 
     function Vk(e, t, n) {
-        const r = AGe(t),
+        const r = MGe(t),
             {
                 line: a,
                 scale: i,
                 axis: s
             } = t,
             o = a.options,
             u = o.fill,
             c = o.backgroundColor,
             {
                 above: f = c,
                 below: h = c
             } = u || {};
-        r && a.points.length && (uw(e, n), RGe(e, {
+        r && a.points.length && (uw(e, n), NGe(e, {
             line: a,
             target: r,
             above: f,
             below: h,
             area: n,
             scale: i,
             axis: s
         }), cw(e))
     }
 
-    function RGe(e, t) {
+    function NGe(e, t) {
         const {
             line: n,
             target: r,
             above: a,
             below: i,
             area: s,
             scale: o
@@ -82694,43 +82702,43 @@
     function fV(e, t) {
         const {
             line: n,
             target: r,
             property: a,
             color: i,
             scale: s
-        } = t, o = bGe(n, r, a);
+        } = t, o = _Ge(n, r, a);
         for (const {
                 source: u,
                 target: c,
                 start: f,
                 end: h
             }
             of o) {
             const {
                 style: {
                     backgroundColor: p = i
                 } = {}
             } = u, g = r !== !0;
-            e.save(), e.fillStyle = p, NGe(e, s, g && YC(a, f, h)), e.beginPath();
+            e.save(), e.fillStyle = p, FGe(e, s, g && YC(a, f, h)), e.beginPath();
             const _ = !!n.pathSegment(e, u);
             let y;
             if (g) {
                 _ ? e.closePath() : hV(e, r, h, a);
                 const w = !!r.pathSegment(e, c, {
                     move: _,
                     reverse: !0
                 });
                 y = _ && w, y || hV(e, r, f, a)
             }
             e.closePath(), e.fill(y ? "evenodd" : "nonzero"), e.restore()
         }
     }
 
-    function NGe(e, t, n) {
+    function FGe(e, t, n) {
         const {
             top: r,
             bottom: a
         } = t.chart.chartArea, {
             property: i,
             start: s,
             end: o
@@ -82738,30 +82746,30 @@
         i === "x" && (e.beginPath(), e.rect(s, r, o - s, a - r), e.clip())
     }
 
     function hV(e, t, n, r) {
         const a = t.interpolate(n, r);
         a && e.lineTo(a.x, a.y)
     }
-    var FGe = {
+    var VGe = {
         id: "filler",
         afterDatasetsUpdate(e, t, n) {
             const r = (e.data.datasets || []).length,
                 a = [];
             let i, s, o, u;
             for (s = 0; s < r; ++s) i = e.getDatasetMeta(s), o = i.dataset, u = null, o && o.options && o instanceof cc && (u = {
                 visible: e.isDatasetVisible(s),
                 index: s,
-                fill: SGe(o, s, r),
+                fill: kGe(o, s, r),
                 chart: e,
                 axis: i.controller.options.indexAxis,
                 scale: i.vScale,
                 line: o
             }), i.$filler = u, a.push(u);
-            for (s = 0; s < r; ++s) u = a[s], !(!u || u.fill === !1) && (u.fill = wGe(a, s, n.propagate))
+            for (s = 0; s < r; ++s) u = a[s], !(!u || u.fill === !1) && (u.fill = SGe(a, s, n.propagate))
         },
         beforeDraw(e, t, n) {
             const r = n.drawTime === "beforeDraw",
                 a = e.getSortedVisibleDatasetMetas(),
                 i = e.chartArea;
             for (let s = a.length - 1; s >= 0; --s) {
                 const o = a[s].$filler;
@@ -82792,15 +82800,15 @@
             } = e;
             return e.usePointStyle && (n = Math.min(n, t), r = e.pointStyleWidth || Math.min(r, t)), {
                 boxWidth: r,
                 boxHeight: n,
                 itemHeight: Math.max(t, n)
             }
         },
-        VGe = (e, t) => e !== null && t !== null && e.datasetIndex === t.datasetIndex && e.index === t.index;
+        jGe = (e, t) => e !== null && t !== null && e.datasetIndex === t.datasetIndex && e.index === t.index;
     class mV extends Kc {
         constructor(t) {
             super(), this._added = !1, this.legendHitBoxes = [], this._hoveredItem = null, this.doughnutMode = !1, this.chart = t.chart, this.options = t.options, this.ctx = t.ctx, this.legendItems = void 0, this.columnSizes = void 0, this.lineWidths = void 0, this.maxHeight = void 0, this.maxWidth = void 0, this.top = void 0, this.bottom = void 0, this.left = void 0, this.right = void 0, this.height = void 0, this.width = void 0, this._margins = void 0, this.position = void 0, this.weight = void 0, this.fullSize = void 0
         }
         update(t, n, r) {
             this.maxWidth = t, this.maxHeight = n, this._margins = r, this.setDimensions(), this.buildLabels(), this.fit()
         }
@@ -82872,15 +82880,15 @@
                 g = 0,
                 _ = 0,
                 y = 0;
             return this.legendItems.forEach((w, S) => {
                 const {
                     itemWidth: k,
                     itemHeight: C
-                } = jGe(r, n, i, w, a);
+                } = BGe(r, n, i, w, a);
                 S > 0 && g + C + 2 * o > f && (h += p + o, c.push({
                     width: p,
                     height: g
                 }), _ += p + o, y++, p = g = 0), u[S] = {
                     left: _,
                     top: g,
                     col: y,
@@ -82991,15 +82999,15 @@
                 const R = a.measureText(A.text).width,
                     F = u.textAlign(A.textAlign || (A.textAlign = s.textAlign)),
                     U = _ + p + R;
                 let G = g.x,
                     B = g.y;
                 u.setWidth(this.width), C ? O > 0 && G + U + f > this.right && (B = g.y += E, g.line++, G = g.x = yi(i, this.left + f, this.right - r[g.line])) : O > 0 && B + E > this.bottom && (G = g.x = G + n[g.line].width + f, g.line++, B = g.y = yi(i, this.top + x + f, this.bottom - n[g.line].height));
                 const W = u.x(G);
-                if (S(W, B, A), G = $8e(F, G + _ + p, C ? G + U : this.right, t.rtl), k(u.x(G), B, A), C) g.x += U + f;
+                if (S(W, B, A), G = C8e(F, G + _ + p, C ? G + U : this.right, t.rtl), k(u.x(G), B, A), C) g.x += U + f;
                 else if (typeof A.text != "string") {
                     const ee = c.lineHeight;
                     g.y += eq(A, ee) + f
                 } else g.y += E
             }), DY(this.ctx, t.textDirection)
         }
         drawTitle() {
@@ -83035,52 +83043,52 @@
                 for (i = this.legendHitBoxes, r = 0; r < i.length; ++r)
                     if (a = i[r], uc(t, a.left, a.left + a.width) && uc(n, a.top, a.top + a.height)) return this.legendItems[r]
             }
             return null
         }
         handleEvent(t) {
             const n = this.options;
-            if (!WGe(t.type, n)) return;
+            if (!UGe(t.type, n)) return;
             const r = this._getLegendItemAt(t.x, t.y);
             if (t.type === "mousemove" || t.type === "mouseout") {
                 const a = this._hoveredItem,
-                    i = VGe(a, r);
+                    i = jGe(a, r);
                 a && !i && mr(n.onLeave, [t, a, this], this), this._hoveredItem = r, r && !i && mr(n.onHover, [t, r, this], this)
             } else r && mr(n.onClick, [t, r, this], this)
         }
     }
 
-    function jGe(e, t, n, r, a) {
-        const i = BGe(r, e, t, n),
-            s = HGe(a, r, t.lineHeight);
+    function BGe(e, t, n, r, a) {
+        const i = HGe(r, e, t, n),
+            s = WGe(a, r, t.lineHeight);
         return {
             itemWidth: i,
             itemHeight: s
         }
     }
 
-    function BGe(e, t, n, r) {
+    function HGe(e, t, n, r) {
         let a = e.text;
         return a && typeof a != "string" && (a = a.reduce((i, s) => i.length > s.length ? i : s)), t + n.size / 2 + r.measureText(a).width
     }
 
-    function HGe(e, t, n) {
+    function WGe(e, t, n) {
         let r = e;
         return typeof t.text != "string" && (r = eq(t, n)), r
     }
 
     function eq(e, t) {
         const n = e.text ? e.text.length : 0;
         return t * n
     }
 
-    function WGe(e, t) {
+    function UGe(e, t) {
         return !!((e === "mousemove" || e === "mouseout") && (t.onHover || t.onLeave) || t.onClick && (e === "click" || e === "mouseup"))
     }
-    var UGe = {
+    var zGe = {
         id: "legend",
         _element: mV,
         start(e, t, n) {
             const r = e.legend = new mV({
                 ctx: e.ctx,
                 options: n,
                 chart: e
@@ -83224,27 +83232,27 @@
                 textAlign: lA(n.align),
                 textBaseline: "middle",
                 translation: [s, o]
             })
         }
     }
 
-    function zGe(e, t) {
+    function YGe(e, t) {
         const n = new tq({
             ctx: e.ctx,
             options: t,
             chart: e
         });
         Hs.configure(e, n, t), Hs.addBox(e, n), e.titleBlock = n
     }
-    var YGe = {
+    var qGe = {
         id: "title",
         _element: tq,
         start(e, t, n) {
-            zGe(e, n)
+            YGe(e, n)
         },
         stop(e) {
             const t = e.titleBlock;
             Hs.removeBox(e, t), delete e.titleBlock
         },
         beforeUpdate(e, t, n) {
             const r = e.titleBlock;
@@ -83319,15 +83327,15 @@
 
     function zl(e) {
         return (typeof e == "string" || e instanceof String) && e.indexOf(`
 `) > -1 ? e.split(`
 `) : e
     }
 
-    function qGe(e, t) {
+    function GGe(e, t) {
         const {
             element: n,
             datasetIndex: r,
             index: a
         } = t, i = e.getDatasetMeta(r).controller, {
             label: s,
             value: o
@@ -83379,62 +83387,62 @@
             ar(x.before, C), ar(x.lines, C), ar(x.after, C)
         }), k = 0, n.font = f.string, ar(e.footer, C), n.restore(), w += _.width, {
             width: w,
             height: y
         }
     }
 
-    function GGe(e, t) {
+    function KGe(e, t) {
         const {
             y: n,
             height: r
         } = t;
         return n < r / 2 ? "top" : n > e.height - r / 2 ? "bottom" : "center"
     }
 
-    function KGe(e, t, n, r) {
+    function XGe(e, t, n, r) {
         const {
             x: a,
             width: i
         } = r, s = n.caretSize + n.caretPadding;
         if (e === "left" && a + i + s > t.width || e === "right" && a - i - s < 0) return !0
     }
 
-    function XGe(e, t, n, r) {
+    function JGe(e, t, n, r) {
         const {
             x: a,
             width: i
         } = n, {
             width: s,
             chartArea: {
                 left: o,
                 right: u
             }
         } = e;
         let c = "center";
-        return r === "center" ? c = a <= (o + u) / 2 ? "left" : "right" : a <= i / 2 ? c = "left" : a >= s - i / 2 && (c = "right"), KGe(c, e, t, n) && (c = "center"), c
+        return r === "center" ? c = a <= (o + u) / 2 ? "left" : "right" : a <= i / 2 ? c = "left" : a >= s - i / 2 && (c = "right"), XGe(c, e, t, n) && (c = "center"), c
     }
 
     function gV(e, t, n) {
-        const r = n.yAlign || t.yAlign || GGe(e, n);
+        const r = n.yAlign || t.yAlign || KGe(e, n);
         return {
-            xAlign: n.xAlign || t.xAlign || XGe(e, t, n, r),
+            xAlign: n.xAlign || t.xAlign || JGe(e, t, n, r),
             yAlign: r
         }
     }
 
-    function JGe(e, t) {
+    function ZGe(e, t) {
         let {
             x: n,
             width: r
         } = e;
         return t === "right" ? n -= r : t === "center" && (n -= r / 2), n
     }
 
-    function ZGe(e, t, n) {
+    function QGe(e, t, n) {
         let {
             y: r,
             height: a
         } = e;
         return t === "top" ? r += n : t === "bottom" ? r -= a + n : r -= a / 2, r
     }
 
@@ -83448,16 +83456,16 @@
             yAlign: u
         } = n, c = a + i, {
             topLeft: f,
             topRight: h,
             bottomLeft: p,
             bottomRight: g
         } = Xd(s);
-        let _ = JGe(t, o);
-        const y = ZGe(t, u, c);
+        let _ = ZGe(t, o);
+        const y = QGe(t, u, c);
         return u === "center" ? o === "left" ? _ += c : o === "right" && (_ -= c) : o === "left" ? _ -= Math.max(f, p) + a : o === "right" && (_ += Math.max(h, g) + a), {
             x: ks(_, 0, r.width - t.width),
             y: ks(y, 0, r.height - t.height)
         }
     }
 
     function b0(e, t, n) {
@@ -83465,15 +83473,15 @@
         return t === "center" ? e.x + e.width / 2 : t === "right" ? e.x + e.width - r.right : e.x + r.left
     }
 
     function bV(e) {
         return Go([], zl(e))
     }
 
-    function QGe(e, t, n) {
+    function e9e(e, t, n) {
         return Gc(e, {
             tooltip: t,
             tooltipItems: n,
             type: "tooltip"
         })
     }
 
@@ -83549,15 +83557,15 @@
             const n = this.chart,
                 r = this.options.setContext(this.getContext()),
                 a = r.enabled && n.options.animation && r.animations,
                 i = new NY(this.chart, a);
             return a._cacheable && (this._cachedAnimations = Object.freeze(i)), i
         }
         getContext() {
-            return this.$context || (this.$context = QGe(this.chart.getContext(), this, this._tooltipItems))
+            return this.$context || (this.$context = e9e(this.chart.getContext(), this, this._tooltipItems))
         }
         getTitle(t, n) {
             const {
                 callbacks: r
             } = n, a = Xi(r, "beforeTitle", this, t), i = Xi(r, "title", this, t), s = Xi(r, "afterTitle", this, t);
             let o = [];
             return o = Go(o, zl(a)), o = Go(o, zl(i)), o = Go(o, zl(s)), o
@@ -83593,15 +83601,15 @@
             const n = this._active,
                 r = this.chart.data,
                 a = [],
                 i = [],
                 s = [];
             let o = [],
                 u, c;
-            for (u = 0, c = n.length; u < c; ++u) o.push(qGe(this.chart, n[u]));
+            for (u = 0, c = n.length; u < c; ++u) o.push(GGe(this.chart, n[u]));
             return t.filter && (o = o.filter((f, h, p) => t.filter(f, h, p, r))), t.itemSort && (o = o.sort((f, h) => t.itemSort(f, h, r))), ar(o, f => {
                 const h = _V(t.callbacks, f);
                 a.push(Xi(h, "labelColor", this, f)), i.push(Xi(h, "labelPointStyle", this, f)), s.push(Xi(h, "labelTextColor", this, f))
             }), this.labelColors = a, this.labelPointStyles = i, this.labelTextColors = s, this.dataPoints = o, o
         }
         update(t, n) {
             const r = this.options.setContext(this.getContext()),
@@ -83853,15 +83861,15 @@
                 caretY: a,
                 options: i
             } = this, s = Hm[i.position].call(this, t, n);
             return s !== !1 && (r !== s.x || a !== s.y)
         }
     }
     Ye(qC, "positioners", Hm);
-    var e9e = {
+    var t9e = {
         id: "tooltip",
         _element: qC,
         positioners: Hm,
         afterInit(e, t, n) {
             n && (e.tooltip = new qC({
                 chart: e,
                 options: n
@@ -83959,26 +83967,26 @@
             },
             animations: {
                 _fallback: "animation"
             }
         },
         additionalOptionScopes: ["interaction"]
     };
-    const t9e = (e, t, n, r) => (typeof t == "string" ? (n = e.push(t) - 1, r.unshift({
+    const n9e = (e, t, n, r) => (typeof t == "string" ? (n = e.push(t) - 1, r.unshift({
         index: n,
         label: t
     })) : isNaN(t) && (n = null), n);
 
-    function n9e(e, t, n, r) {
+    function r9e(e, t, n, r) {
         const a = e.indexOf(t);
-        if (a === -1) return t9e(e, t, n, r);
+        if (a === -1) return n9e(e, t, n, r);
         const i = e.lastIndexOf(t);
         return a !== i ? n : a
     }
-    const r9e = (e, t) => e === null ? null : ks(Math.round(e), 0, t);
+    const a9e = (e, t) => e === null ? null : ks(Math.round(e), 0, t);
 
     function wV(e) {
         const t = this.getLabels();
         return e >= 0 && e < t.length ? t[e] : e
     }
     class GC extends kf {
         constructor(t) {
@@ -83996,15 +84004,15 @@
                 this._addedLabels = []
             }
             super.init(t)
         }
         parse(t, n) {
             if (Xn(t)) return null;
             const r = this.getLabels();
-            return n = isFinite(n) && r[n] === t ? n : n9e(r, t, un(n, t), this._addedLabels), r9e(n, r.length - 1)
+            return n = isFinite(n) && r[n] === t ? n : r9e(r, t, un(n, t), this._addedLabels), a9e(n, r.length - 1)
         }
         determineDataLimits() {
             const {
                 minDefined: t,
                 maxDefined: n
             } = this.getUserBounds();
             let {
@@ -84047,15 +84055,15 @@
     }
     Ye(GC, "id", "category"), Ye(GC, "defaults", {
         ticks: {
             callback: wV
         }
     });
 
-    function a9e(e, t) {
+    function i9e(e, t) {
         const n = [],
             {
                 bounds: a,
                 step: i,
                 min: s,
                 max: o,
                 precision: u,
@@ -84077,15 +84085,15 @@
         let E = yF((w - y) / _ / g) * g,
             A, O, R, F;
         if (E < 1e-14 && !S && !k) return [{
             value: y
         }, {
             value: w
         }];
-        F = Math.ceil(w / E) - Math.floor(y / E), F > _ && (E = yF(F * E / _ / g) * g), Xn(u) || (A = Math.pow(10, u), E = Math.ceil(E * A) / A), a === "ticks" ? (O = Math.floor(y / E) * E, R = Math.ceil(w / E) * E) : (O = y, R = w), S && k && i && v8e((o - s) / i, E / 1e3) ? (F = Math.round(Math.min((o - s) / E, f)), E = (o - s) / F, O = s, R = o) : C ? (O = S ? s : O, R = k ? o : R, F = c - 1, E = (R - O) / F) : (F = (R - O) / E, hv(F, Math.round(F), E / 1e3) ? F = Math.round(F) : F = Math.ceil(F));
+        F = Math.ceil(w / E) - Math.floor(y / E), F > _ && (E = yF(F * E / _ / g) * g), Xn(u) || (A = Math.pow(10, u), E = Math.ceil(E * A) / A), a === "ticks" ? (O = Math.floor(y / E) * E, R = Math.ceil(w / E) * E) : (O = y, R = w), S && k && i && g8e((o - s) / i, E / 1e3) ? (F = Math.round(Math.min((o - s) / E, f)), E = (o - s) / F, O = s, R = o) : C ? (O = S ? s : O, R = k ? o : R, F = c - 1, E = (R - O) / F) : (F = (R - O) / E, hv(F, Math.round(F), E / 1e3) ? F = Math.round(F) : F = Math.ceil(F));
         const U = Math.max(bF(E), bF(O));
         A = Math.pow(10, Xn(u) ? U : u), O = Math.round(O * A) / A, R = Math.round(R * A) / A;
         let G = 0;
         for (S && (p && O !== s ? (n.push({
                 value: s
             }), O < s && G++, hv(Math.round((O + G * E) * A) / A, s, SV(s, x, e)) && G++) : O < s && G++); G < F; ++G) {
             const B = Math.round((O + G * E) * A) / A;
@@ -84167,15 +84175,15 @@
                     count: n.count,
                     maxDigits: this._maxDigits(),
                     horizontal: this.isHorizontal(),
                     minRotation: n.minRotation || 0,
                     includeBounds: n.includeBounds !== !1
                 },
                 i = this._range || this,
-                s = a9e(a, i);
+                s = i9e(a, i);
             return t.bounds === "ticks" && mY(s, this, "value"), t.reverse ? (s.reverse(), this.start = this.max, this.end = this.min) : (this.start = this.min, this.end = this.max), s
         }
         configure() {
             const t = this.ticks;
             let n = this.min,
                 r = this.max;
             if (super.configure(), this.options.offset && t.length) {
@@ -84225,30 +84233,30 @@
 
     function $V(e, t, n) {
         const r = Math.pow(10, n),
             a = Math.floor(e / r);
         return Math.ceil(t / r) - a
     }
 
-    function i9e(e, t) {
+    function s9e(e, t) {
         const n = t - e;
         let r = ng(n);
         for (; $V(e, t, r) > 10;) r++;
         for (; $V(e, t, r) < 10;) r--;
         return Math.min(r, ng(e))
     }
 
-    function s9e(e, {
+    function o9e(e, {
         min: t,
         max: n
     }) {
         t = gs(e.min, t);
         const r = [],
             a = ng(t);
-        let i = i9e(t, n),
+        let i = s9e(t, n),
             s = i < 0 ? Math.pow(10, Math.abs(i)) : 1;
         const o = Math.pow(10, i),
             u = a > i ? Math.pow(10, a) : 0,
             c = Math.round((t - u) * s) / s,
             f = Math.floor((t - u) / o / 10) * o * 10;
         let h = Math.floor((c - f) / Math.pow(10, i)),
             p = gs(e.min, Math.round((u + f + h * Math.pow(10, i)) * s) / s);
@@ -84296,15 +84304,15 @@
         }
         buildTicks() {
             const t = this.options,
                 n = {
                     min: this._userMin,
                     max: this._userMax
                 },
-                r = s9e(n, this);
+                r = o9e(n, this);
             return t.bounds === "ticks" && mY(r, this, "value"), t.reverse ? (r.reverse(), this.start = this.max, this.end = this.min) : (this.start = this.min, this.end = this.max), r
         }
         getLabelForValue(t) {
             return t === void 0 ? "0" : Kg(t, this.chart.options.locale, this.options.ticks.format)
         }
         configure() {
             const t = this.min;
@@ -84332,17 +84340,17 @@
         if (t.display && e.display) {
             const n = Ti(t.backdropPadding);
             return un(t.font && t.font.size, na.font.size) + n.height
         }
         return 0
     }
 
-    function o9e(e, t, n) {
+    function l9e(e, t, n) {
         return n = Lr(n) ? n : [n], {
-            w: I8e(e, t.string, n),
+            w: L8e(e, t.string, n),
             h: n.length * t.lineHeight
         }
     }
 
     function TV(e, t, n, r, a) {
         return e === r || e === a ? {
             start: t - n / 2,
@@ -84352,15 +84360,15 @@
             end: t
         } : {
             start: t,
             end: t + n
         }
     }
 
-    function l9e(e) {
+    function u9e(e) {
         const t = {
                 l: e.left + e._padding.left,
                 r: e.right - e._padding.right,
                 t: e.top + e._padding.top,
                 b: e.bottom - e._padding.bottom
             },
             n = Object.assign({}, t),
@@ -84370,59 +84378,59 @@
             s = e.options.pointLabels,
             o = s.centerPointLabels ? Wr / i : 0;
         for (let u = 0; u < i; u++) {
             const c = s.setContext(e.getPointLabelContext(u));
             a[u] = c.padding;
             const f = e.getPointPosition(u, e.drawingArea + a[u], o),
                 h = Na(c.font),
-                p = o9e(e.ctx, h, e._pointLabels[u]);
+                p = l9e(e.ctx, h, e._pointLabels[u]);
             r[u] = p;
             const g = bs(e.getIndexAngle(u) + o),
                 _ = Math.round(sA(g)),
                 y = TV(_, f.x, p.w, 0, 180),
                 w = TV(_, f.y, p.h, 90, 270);
-            u9e(n, t, g, y, w)
+            c9e(n, t, g, y, w)
         }
-        e.setCenterPoint(t.l - n.l, n.r - t.r, t.t - n.t, n.b - t.b), e._pointLabelItems = f9e(e, r, a)
+        e.setCenterPoint(t.l - n.l, n.r - t.r, t.t - n.t, n.b - t.b), e._pointLabelItems = h9e(e, r, a)
     }
 
-    function u9e(e, t, n, r, a) {
+    function c9e(e, t, n, r, a) {
         const i = Math.abs(Math.sin(n)),
             s = Math.abs(Math.cos(n));
         let o = 0,
             u = 0;
         r.start < t.l ? (o = (t.l - r.start) / i, e.l = Math.min(e.l, t.l - o)) : r.end > t.r && (o = (r.end - t.r) / i, e.r = Math.max(e.r, t.r + o)), a.start < t.t ? (u = (t.t - a.start) / s, e.t = Math.min(e.t, t.t - u)) : a.end > t.b && (u = (a.end - t.b) / s, e.b = Math.max(e.b, t.b + u))
     }
 
-    function c9e(e, t, n) {
+    function d9e(e, t, n) {
         const r = e.drawingArea,
             {
                 extra: a,
                 additionalAngle: i,
                 padding: s,
                 size: o
             } = n,
             u = e.getPointPosition(t, r + a + s, i),
             c = Math.round(sA(bs(u.angle + Bi))),
-            f = m9e(u.y, o.h, c),
-            h = h9e(c),
-            p = p9e(u.x, o.w, h);
+            f = v9e(u.y, o.h, c),
+            h = p9e(c),
+            p = m9e(u.x, o.w, h);
         return {
             visible: !0,
             x: u.x,
             y: f,
             textAlign: h,
             left: p,
             top: f,
             right: p + o.w,
             bottom: f + o.h
         }
     }
 
-    function d9e(e, t) {
+    function f9e(e, t) {
         if (!t) return !0;
         const {
             left: n,
             top: r,
             right: a,
             bottom: i
         } = e;
@@ -84437,48 +84445,48 @@
             y: r
         }, t) || eu({
             x: a,
             y: i
         }, t))
     }
 
-    function f9e(e, t, n) {
+    function h9e(e, t, n) {
         const r = [],
             a = e._pointLabels.length,
             i = e.options,
             {
                 centerPointLabels: s,
                 display: o
             } = i.pointLabels,
             u = {
                 extra: XC(i) / 2,
                 additionalAngle: s ? Wr / a : 0
             };
         let c;
         for (let f = 0; f < a; f++) {
             u.padding = n[f], u.size = t[f];
-            const h = c9e(e, f, u);
-            r.push(h), o === "auto" && (h.visible = d9e(h, c), h.visible && (c = h))
+            const h = d9e(e, f, u);
+            r.push(h), o === "auto" && (h.visible = f9e(h, c), h.visible && (c = h))
         }
         return r
     }
 
-    function h9e(e) {
+    function p9e(e) {
         return e === 0 || e === 180 ? "center" : e < 180 ? "left" : "right"
     }
 
-    function p9e(e, t, n) {
+    function m9e(e, t, n) {
         return n === "right" ? e -= t : n === "center" && (e -= t / 2), e
     }
 
-    function m9e(e, t, n) {
+    function v9e(e, t, n) {
         return n === 90 || n === 270 ? e -= t / 2 : (n > 270 || n < 90) && (e -= t), e
     }
 
-    function v9e(e, t, n) {
+    function g9e(e, t, n) {
         const {
             left: r,
             top: a,
             right: i,
             bottom: s
         } = n, {
             backdropColor: o
@@ -84497,26 +84505,26 @@
                 w: p,
                 h: g,
                 radius: u
             }), e.fill()) : e.fillRect(f, h, p, g)
         }
     }
 
-    function g9e(e, t) {
+    function y9e(e, t) {
         const {
             ctx: n,
             options: {
                 pointLabels: r
             }
         } = e;
         for (let a = t - 1; a >= 0; a--) {
             const i = e._pointLabelItems[a];
             if (!i.visible) continue;
             const s = r.setContext(e.getPointLabelContext(a));
-            v9e(n, s, i);
+            g9e(n, s, i);
             const o = Na(s.font),
                 {
                     x: u,
                     y: c,
                     textAlign: f
                 } = i;
             cf(n, e._pointLabels[a], u, c + o.lineHeight / 2, o, {
@@ -84535,25 +84543,25 @@
         else {
             let i = e.getPointPosition(0, t);
             a.moveTo(i.x, i.y);
             for (let s = 1; s < r; s++) i = e.getPointPosition(s, t), a.lineTo(i.x, i.y)
         }
     }
 
-    function y9e(e, t, n, r, a) {
+    function b9e(e, t, n, r, a) {
         const i = e.ctx,
             s = t.circular,
             {
                 color: o,
                 lineWidth: u
             } = t;
         !s && !r || !o || !u || n < 0 || (i.save(), i.strokeStyle = o, i.lineWidth = u, i.setLineDash(a.dash), i.lineDashOffset = a.dashOffset, i.beginPath(), rq(e, n, s, r), i.closePath(), i.stroke(), i.restore())
     }
 
-    function b9e(e, t, n) {
+    function _9e(e, t, n) {
         return Gc(e, {
             label: n,
             index: t,
             type: "pointLabel"
         })
     }
     class _0 extends m_ {
@@ -84580,15 +84588,15 @@
             m_.prototype.generateTickLabels.call(this, t), this._pointLabels = this.getLabels().map((n, r) => {
                 const a = mr(this.options.pointLabels.callback, [n, r], this);
                 return a || a === 0 ? a : ""
             }).filter((n, r) => this.chart.getDataVisibility(r))
         }
         fit() {
             const t = this.options;
-            t.display && t.pointLabels.display ? l9e(this) : this.setCenterPoint(0, 0, 0, 0)
+            t.display && t.pointLabels.display ? u9e(this) : this.setCenterPoint(0, 0, 0, 0)
         }
         setCenterPoint(t, n, r, a) {
             this.xCenter += Math.floor((t - n) / 2), this.yCenter += Math.floor((r - a) / 2), this.drawingArea -= Math.min(this.drawingArea / 2, Math.max(t, n, r, a))
         }
         getIndexAngle(t) {
             const n = Ya / (this._pointLabels.length || 1),
                 r = this.options.startAngle || 0;
@@ -84604,15 +84612,15 @@
             const n = t / (this.drawingArea / (this.max - this.min));
             return this.options.reverse ? this.max - n : this.min + n
         }
         getPointLabelContext(t) {
             const n = this._pointLabels || [];
             if (t >= 0 && t < n.length) {
                 const r = n[t];
-                return b9e(this.getContext(), t, r)
+                return _9e(this.getContext(), t, r)
             }
         }
         getPointPosition(t, n, r = 0) {
             const a = this.getIndexAngle(t) - Bi + r;
             return {
                 x: Math.cos(a) * n + this.xCenter,
                 y: Math.sin(a) * n + this.yCenter,
@@ -84657,21 +84665,21 @@
                 {
                     angleLines: r,
                     grid: a,
                     border: i
                 } = n,
                 s = this._pointLabels.length;
             let o, u, c;
-            if (n.pointLabels.display && g9e(this, s), a.display && this.ticks.forEach((f, h) => {
+            if (n.pointLabels.display && y9e(this, s), a.display && this.ticks.forEach((f, h) => {
                     if (h !== 0 || h === 0 && this.min < 0) {
                         u = this.getDistanceFromCenterForValue(f.value);
                         const p = this.getContext(h),
                             g = a.setContext(p),
                             _ = i.setContext(p);
-                        y9e(this, g, u, s, _)
+                        b9e(this, g, u, s, _)
                     }
                 }), r.display) {
                 for (t.save(), o = s - 1; o >= 0; o--) {
                     const f = r.setContext(this.getPointLabelContext(o)),
                         {
                             color: h,
                             lineWidth: p
@@ -84817,23 +84825,23 @@
             const s = hw[as[i]],
                 o = s.steps ? s.steps : Number.MAX_SAFE_INTEGER;
             if (s.common && Math.ceil((n - t) / (o * s.size)) <= r) return as[i]
         }
         return as[a - 1]
     }
 
-    function _9e(e, t, n, r, a) {
+    function w9e(e, t, n, r, a) {
         for (let i = as.length - 1; i >= as.indexOf(n); i--) {
             const s = as[i];
             if (hw[s].common && e._adapter.diff(a, r, s) >= t - 1) return s
         }
         return as[n ? as.indexOf(n) : 0]
     }
 
-    function w9e(e) {
+    function S9e(e) {
         for (let t = as.indexOf(e) + 1, n = as.length; t < n; ++t)
             if (hw[as[t]].common) return as[t]
     }
 
     function OV(e, t, n) {
         if (!n) e[t] = !0;
         else if (n.length) {
@@ -84841,15 +84849,15 @@
                 lo: r,
                 hi: a
             } = oA(n, t), i = n[r] >= t ? n[r] : n[a];
             e[i] = !0
         }
     }
 
-    function S9e(e, t, n, r) {
+    function k9e(e, t, n, r) {
         const a = e._adapter,
             i = +a.startOf(t[0].value, r),
             s = t[t.length - 1].value;
         let o, u;
         for (o = i; o <= s; o = +a.add(o, 1, r)) u = n[o], u >= 0 && (t[u].major = !0);
         return t
     }
@@ -84859,27 +84867,27 @@
             a = {},
             i = t.length;
         let s, o;
         for (s = 0; s < i; ++s) o = t[s], a[o] = s, r.push({
             value: o,
             major: !1
         });
-        return i === 0 || !n ? r : S9e(e, r, a, n)
+        return i === 0 || !n ? r : k9e(e, r, a, n)
     }
     class v_ extends kf {
         constructor(t) {
             super(t), this._cache = {
                 data: [],
                 labels: [],
                 all: []
             }, this._unit = "day", this._majorUnit = void 0, this._offsets = {}, this._normalized = !1, this._parseOpts = void 0
         }
         init(t, n = {}) {
             const r = t.time || (t.time = {}),
-                a = this._adapter = new KYe._date(t.adapters.date);
+                a = this._adapter = new XYe._date(t.adapters.date);
             a.init(n), fv(r.displayFormats, a.formats()), this._parseOpts = {
                 parser: r.parser,
                 round: r.round,
                 isoWeekday: r.isoWeekday
             }, super.init(t), this._normalized = n.normalized
         }
         parse(t, n) {
@@ -84920,16 +84928,16 @@
             const t = this.options,
                 n = t.time,
                 r = t.ticks,
                 a = r.source === "labels" ? this.getLabelTimestamps() : this._generate();
             t.bounds === "ticks" && a.length && (this.min = this._userMin || a[0], this.max = this._userMax || a[a.length - 1]);
             const i = this.min,
                 s = this.max,
-                o = w8e(a, i, s);
-            return this._unit = n.unit || (r.autoSkip ? xV(n.minUnit, this.min, this.max, this._getLabelCapacity(i)) : _9e(this, o.length, n.minUnit, this.min, this.max)), this._majorUnit = !r.major.enabled || this._unit === "year" ? void 0 : w9e(this._unit), this.initOffsets(a), t.reverse && o.reverse(), AV(this, o, this._majorUnit)
+                o = S8e(a, i, s);
+            return this._unit = n.unit || (r.autoSkip ? xV(n.minUnit, this.min, this.max, this._getLabelCapacity(i)) : w9e(this, o.length, n.minUnit, this.min, this.max)), this._majorUnit = !r.major.enabled || this._unit === "year" ? void 0 : S9e(this._unit), this.initOffsets(a), t.reverse && o.reverse(), AV(this, o, this._majorUnit)
         }
         afterAutoSkip() {
             this.options.offsetAfterAutoskip && this.initOffsets(this.ticks.map(t => +t.value))
         }
         initOffsets(t = []) {
             let n = 0,
                 r = 0,
@@ -85159,48 +85167,48 @@
                 default: "label"
             },
             updateMode: {
                 type: String,
                 default: void 0
             }
         },
-        k9e = {
+        $9e = {
             ariaLabel: {
                 type: String
             },
             ariaDescribedby: {
                 type: String
             }
         },
-        $9e = {
+        C9e = {
             type: {
                 type: String,
                 required: !0
             },
             destroyDelay: {
                 type: Number,
                 default: 0
             },
             ...aq,
-            ...k9e
+            ...$9e
         },
-        C9e = oB[0] === "2" ? (e, t) => Object.assign(e, {
+        T9e = oB[0] === "2" ? (e, t) => Object.assign(e, {
             attrs: t
         }) : (e, t) => Object.assign(e, t);
 
     function ah(e) {
         return C_(e) ? It(e) : e
     }
 
-    function T9e(e) {
+    function P9e(e) {
         let t = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : e;
         return C_(t) ? new Proxy(e, {}) : e
     }
 
-    function P9e(e, t) {
+    function E9e(e, t) {
         const n = e.options;
         n && t && Object.assign(n, t)
     }
 
     function iq(e, t) {
         e.labels = t
     }
@@ -85211,23 +85219,23 @@
             const i = e.datasets.find(s => s[n] === a[n]);
             return !i || !a.data || r.includes(i) ? {
                 ...a
             } : (r.push(i), Object.assign(i, a), i)
         })
     }
 
-    function E9e(e, t) {
+    function x9e(e, t) {
         const n = {
             labels: [],
             datasets: []
         };
         return iq(n, e.labels), sq(n, e.datasets, t), n
     }
-    const x9e = Tt({
-        props: $9e,
+    const O9e = Tt({
+        props: C9e,
         setup(e, t) {
             let {
                 expose: n,
                 slots: r
             } = t;
             const a = Te(null),
                 i = ht(null);
@@ -85238,15 +85246,15 @@
                     if (!a.value) return;
                     const {
                         type: c,
                         data: f,
                         options: h,
                         plugins: p,
                         datasetIdKey: g
-                    } = e, _ = E9e(f, g), y = T9e(_, f);
+                    } = e, _ = x9e(f, g), y = P9e(_, f);
                     i.value = new fw(a.value, {
                         type: c,
                         data: y,
                         options: {
                             ...h
                         },
                         plugins: p
@@ -85265,15 +85273,15 @@
                 let [h, p] = c, [g, _] = f;
                 const y = It(i.value);
                 if (!y) return;
                 let w = !1;
                 if (h) {
                     const S = ah(h),
                         k = ah(g);
-                    S && S !== k && (P9e(y, S), w = !0)
+                    S && S !== k && (E9e(y, S), w = !0)
                 }
                 if (p) {
                     const S = ah(p.labels),
                         k = ah(_.labels),
                         C = ah(p.datasets),
                         x = ah(_.datasets);
                     S !== k && (iq(y.config.data, S), w = !0), C && C !== x && (sq(y.config.data, C, e.datasetIdKey), w = !0)
@@ -85301,33 +85309,33 @@
                 } = r;
                 const i = ht(null),
                     s = o => {
                         i.value = o == null ? void 0 : o.chart
                     };
                 return a({
                     chart: i
-                }), () => ba(x9e, C9e({
+                }), () => ba(O9e, T9e({
                     ref: s
                 }, {
                     type: e,
                     ...n
                 }))
             }
         })
     }
-    const O9e = Xc("bar", J0),
-        A9e = Xc("doughnut", gh),
-        M9e = Xc("line", Q0),
-        D9e = Xc("pie", HC),
-        I9e = Xc("polarArea", eb),
-        L9e = Xc("radar", tb),
-        R9e = Xc("bubble", Z0),
-        N9e = Xc("scatter", nb);
-    fw.register(YGe, e9e, UGe, cc, KC, GC, ib, FGe, sb);
-    const F9e = {
+    const A9e = Xc("bar", J0),
+        M9e = Xc("doughnut", gh),
+        D9e = Xc("line", Q0),
+        I9e = Xc("pie", HC),
+        L9e = Xc("polarArea", eb),
+        R9e = Xc("radar", tb),
+        N9e = Xc("bubble", Z0),
+        F9e = Xc("scatter", nb);
+    fw.register(qGe, t9e, zGe, cc, KC, GC, ib, VGe, sb);
+    const V9e = {
             components: {
                 Filters: ow
             },
             props: {
                 settings: {
                     type: Object,
                     required: !0
@@ -85347,22 +85355,22 @@
                     loadData: !0,
                     responseData: null,
                     filterInfo: {
                         search: null,
                         filters: {}
                     },
                     types: {
-                        line: M9e,
-                        bar: O9e,
-                        bubble: R9e,
-                        doughnut: A9e,
-                        pie: D9e,
-                        polararea: I9e,
-                        radar: L9e,
-                        scatter: N9e
+                        line: D9e,
+                        bar: A9e,
+                        bubble: N9e,
+                        doughnut: M9e,
+                        pie: I9e,
+                        polararea: L9e,
+                        radar: R9e,
+                        scatter: F9e
                     }
                 }
             },
             async created() {
                 this.getInlineData()
             },
             methods: {
@@ -85397,63 +85405,63 @@
                             position: "top-center",
                             dangerouslyHTMLString: !0
                         })
                     })
                 }
             }
         },
-        V9e = {
+        j9e = {
             class: "inline-container"
         },
-        j9e = {
+        B9e = {
             key: 2
         },
-        B9e = {
+        H9e = {
             key: 3,
             class: "chart-loader"
         };
 
-    function H9e(e, t, n, r, a, i) {
+    function W9e(e, t, n, r, a, i) {
         const s = ow;
-        return ce(), Oe("div", V9e, [n.method.filterset_fields ? (ce(), Le(s, {
+        return ce(), Oe("div", j9e, [n.method.filterset_fields ? (ce(), Le(s, {
             key: 0,
             settings: n.settings,
             "filterset-fields": n.method.filterset_fields,
             "filter-info-init": a.filterInfo,
             onFiltered: i.handleFilter
         }, null, 8, ["settings", "filterset-fields", "filter-info-init", "onFiltered"])) : Ve("", !0), a.responseData && a.responseData.messages ? (ce(!0), Oe(Ne, {
             key: 1
         }, Et(a.responseData.messages, o => (ce(), Le(i4, {
             key: o.title,
             title: o.title,
             type: o.type,
             density: "compact",
             variant: "tonal"
-        }, null, 8, ["title", "type"]))), 128)) : Ve("", !0), a.responseData ? (ce(), Oe("div", j9e, [(ce(!0), Oe(Ne, null, Et(a.responseData.charts, o => (ce(), Le(Cs(i.getComponent(o)), {
+        }, null, 8, ["title", "type"]))), 128)) : Ve("", !0), a.responseData ? (ce(), Oe("div", B9e, [(ce(!0), Oe(Ne, null, Et(a.responseData.charts, o => (ce(), Le(Cs(i.getComponent(o)), {
             options: o.options,
             data: o,
             width: o.options.width,
             height: o.options.height,
             fill: o.fill,
             pointBorderColor: o.pointBorderColor,
             borderColor: o.borderColor,
             backgroundColor: o.backgroundColor,
             pointBorderWidth: o.pointBorderWidth,
             tension: o.tension,
             borderWidth: o.borderWidth
-        }, null, 8, ["options", "data", "width", "height", "fill", "pointBorderColor", "borderColor", "backgroundColor", "pointBorderWidth", "tension", "borderWidth"]))), 256))])) : Ve("", !0), a.loadData ? (ce(), Oe("div", B9e, [T(Z_, {
+        }, null, 8, ["options", "data", "width", "height", "fill", "pointBorderColor", "borderColor", "backgroundColor", "pointBorderWidth", "tension", "borderWidth"]))), 256))])) : Ve("", !0), a.loadData ? (ce(), Oe("div", H9e, [T(Z_, {
             size: 50,
             color: "primary",
             indeterminate: ""
         })])) : Ve("", !0)])
     }
-    const W9e = xr(F9e, [
-            ["render", H9e]
+    const U9e = xr(V9e, [
+            ["render", W9e]
         ]),
-        U9e = {
+        z9e = {
             props: {
                 id: {
                     type: String,
                     required: !0
                 },
                 method: {
                     type: Object,
@@ -85514,28 +85522,28 @@
                 },
                 changePagination() {
                     let e = Zd();
                     e.page_size = this.pageInfo.limit, jT(e), this.getInlineData()
                 }
             }
         },
-        z9e = {
+        Y9e = {
             class: "table-bottom"
         };
 
-    function Y9e(e, t, n, r, a, i) {
+    function q9e(e, t, n, r, a, i) {
         return ce(), Oe("div", null, [T(M4, {
             class: "model-table",
             items: a.inlineData.data || [],
             loading: a.listLoading,
             "items-per-page": a.pageInfo.limit,
             page: a.pageInfo.page,
             height: "unset"
         }, {
-            bottom: fe(() => [mt("div", z9e, [T($s, {
+            bottom: fe(() => [mt("div", Y9e, [T($s, {
                 justify: "end",
                 "no-gutters": ""
             }, {
                 default: fe(() => [T(Pl, {
                     class: "list-pagination-per-page",
                     modelValue: a.pageInfo.limit,
                     "onUpdate:modelValue": [t[0] || (t[0] = s => a.pageInfo.limit = s), i.changePagination],
@@ -85550,18 +85558,18 @@
                     size: "40"
                 }, null, 8, ["modelValue", "length", "onUpdate:modelValue"])) : Ve("", !0)]),
                 _: 1
             })])]),
             _: 1
         }, 8, ["items", "loading", "items-per-page", "page"])])
     }
-    const q9e = xr(U9e, [
-            ["render", Y9e]
+    const G9e = xr(z9e, [
+            ["render", q9e]
         ]),
-        G9e = {
+        K9e = {
             props: {
                 apiInfo: {
                     type: Object,
                     required: !0
                 },
                 settings: {
                     type: Object,
@@ -85599,16 +85607,16 @@
                 }
             },
             created() {
                 this.apiMethods = G_(this.viewname, this.apiInfo), this.sectionData = this.apiInfo[this.viewname], this.deserializeQuery()
             },
             methods: {
                 getInlineComponent(e) {
-                    if (e.inline_type === "table") return q9e;
-                    if (e.inline_type === "graph") return W9e;
+                    if (e.inline_type === "table") return G9e;
+                    if (e.inline_type === "graph") return U9e;
                     console.error(`Inline not found for inline_type "${e.inline_type}"`)
                 },
                 isDisplayMainTab() {
                     return this.sectionData && this.sectionData.meta && this.sectionData.meta.filds_list
                 },
                 deserializeQuery() {
                     const e = this.inline ? this.$route.query.inlineTab : this.$route.query.tab;
@@ -85628,29 +85636,29 @@
                     const e = `/${this.group}/${this.viewname}/list`;
                     this.$router.push({
                         path: e
                     })
                 }
             }
         },
-        K9e = {
+        X9e = {
             class: "edit-card-container"
         };
 
-    function X9e(e, t, n, r, a, i) {
+    function J9e(e, t, n, r, a, i) {
         const s = uY,
             o = Me("List"),
             u = Me("Edit", !0);
         return ce(), Oe("div", {
             class: Mt({
                 "edit-content": !0,
                 "inline-view": n.inline
             })
         }, [T(Wi, null, {
-            default: fe(() => [mt("div", K9e, [T(Qh, {
+            default: fe(() => [mt("div", X9e, [T(Qh, {
                 modelValue: a.currentTab,
                 "onUpdate:modelValue": [t[0] || (t[0] = c => a.currentTab = c), i.updateTab],
                 direction: n.inline ? "horizontal" : "vertical"
             }, {
                 default: fe(() => [i.isDisplayMainTab() ? (ce(), Le(ou, {
                     key: 0,
                     text: e.$t("general"),
@@ -85725,18 +85733,18 @@
                     _: 2
                 }, 1032, ["value"])) : Ve("", !0)], 64))), 256))]),
                 _: 1
             }, 8, ["modelValue"])])]),
             _: 1
         })], 2)
     }
-    const oq = xr(G9e, [
-            ["render", X9e]
+    const oq = xr(K9e, [
+            ["render", J9e]
         ]),
-        J9e = [{
+        Z9e = [{
             path: "",
             redirect: "/dashboard"
         }, {
             path: "/login",
             component: Rie
         }, {
             path: "",
@@ -85757,32 +85765,32 @@
                 component: lY
             }]
         }, {
             path: "/:pathMatch(.*)*",
             redirect: "/404",
             hidden: !0
         }],
-        Z9e = jee({
-            history: mee(li.base_admin_url || "admin/"),
-            routes: J9e
+        Q9e = jee({
+            history: mee(Ga.base_admin_url || "admin/"),
+            routes: Z9e
         });
 
-    function Q9e(e) {
-        e.use(FQ).use(Z9e).use(VT)
+    function e7e(e) {
+        e.use(FQ).use(Q9e).use(VT)
     }
-    const e7e = {};
+    const t7e = {};
 
-    function t7e(e, t) {
+    function n7e(e, t) {
         const n = Me("router-view");
         return ce(), Le(n)
     }
-    const n7e = xr(e7e, [
-            ["render", t7e]
+    const r7e = xr(t7e, [
+            ["render", n7e]
         ]),
-        Jg = gB(n7e);
+        Jg = gB(r7e);
     Jg.component("JsonForms", a4);
     Jg.component("List", lY);
     Jg.component("Edit", oq);
-    Q9e(Jg);
+    e7e(Jg);
     Jg.mount("#app")
 });
-export default r7e();
+export default a7e();
```

### Comparing `django_customvueadmin-0.2.5/custom_admin/static/custom_admin/index-Dtvf0MB6.css` & `django_customvueadmin-0.2.6/custom_admin/static/custom_admin/index-C6_9c0_p.css`

 * *Files 0% similar despite different names*

```diff
@@ -1,5 +1,5 @@
 @charset "UTF-8";@font-face{font-family:Material Design Icons;src:url(/static/custom_admin/materialdesignicons-webfont-DttUABo4.eot?v=7.0.96);src:url(/static/custom_admin/materialdesignicons-webfont-DttUABo4.eot?#iefix&v=7.0.96) format("embedded-opentype"),url(/static/custom_admin/materialdesignicons-webfont-CYDMK1kx.woff2?v=7.0.96) format("woff2"),url(/static/custom_admin/materialdesignicons-webfont-CgCzGbLl.woff?v=7.0.96) format("woff"),url(/static/custom_admin/materialdesignicons-webfont-D3kAzl71.ttf?v=7.0.96) format("truetype");font-weight:400;font-style:normal}.mdi:before,.mdi-set{display:inline-block;font: 24px/1 Material Design Icons;font-size:inherit;text-rendering:auto;line-height:inherit;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.mdi-ab-testing:before{content:"󰇉"}.mdi-abacus:before{content:"󱛠"}.mdi-abjad-arabic:before{content:"󱌨"}.mdi-abjad-hebrew:before{content:"󱌩"}.mdi-abugida-devanagari:before{content:"󱌪"}.mdi-abugida-thai:before{content:"󱌫"}.mdi-access-point:before{content:"󰀃"}.mdi-access-point-check:before{content:"󱔸"}.mdi-access-point-minus:before{content:"󱔹"}.mdi-access-point-network:before{content:"󰀂"}.mdi-access-point-network-off:before{content:"󰯡"}.mdi-access-point-off:before{content:"󱔑"}.mdi-access-point-plus:before{content:"󱔺"}.mdi-access-point-remove:before{content:"󱔻"}.mdi-account:before{content:"󰀄"}.mdi-account-alert:before{content:"󰀅"}.mdi-account-alert-outline:before{content:"󰭐"}.mdi-account-arrow-down:before{content:"󱡨"}.mdi-account-arrow-down-outline:before{content:"󱡩"}.mdi-account-arrow-left:before{content:"󰭑"}.mdi-account-arrow-left-outline:before{content:"󰭒"}.mdi-account-arrow-right:before{content:"󰭓"}.mdi-account-arrow-right-outline:before{content:"󰭔"}.mdi-account-arrow-up:before{content:"󱡧"}.mdi-account-arrow-up-outline:before{content:"󱡪"}.mdi-account-badge:before{content:"󱬊"}.mdi-account-badge-outline:before{content:"󱬋"}.mdi-account-box:before{content:"󰀆"}.mdi-account-box-multiple:before{content:"󰤴"}.mdi-account-box-multiple-outline:before{content:"󱀊"}.mdi-account-box-outline:before{content:"󰀇"}.mdi-account-cancel:before{content:"󱋟"}.mdi-account-cancel-outline:before{content:"󱋠"}.mdi-account-card:before{content:"󱮤"}.mdi-account-card-outline:before{content:"󱮥"}.mdi-account-cash:before{content:"󱂗"}.mdi-account-cash-outline:before{content:"󱂘"}.mdi-account-check:before{content:"󰀈"}.mdi-account-check-outline:before{content:"󰯢"}.mdi-account-child:before{content:"󰪉"}.mdi-account-child-circle:before{content:"󰪊"}.mdi-account-child-outline:before{content:"󱃈"}.mdi-account-circle:before{content:"󰀉"}.mdi-account-circle-outline:before{content:"󰭕"}.mdi-account-clock:before{content:"󰭖"}.mdi-account-clock-outline:before{content:"󰭗"}.mdi-account-cog:before{content:"󱍰"}.mdi-account-cog-outline:before{content:"󱍱"}.mdi-account-convert:before{content:"󰀊"}.mdi-account-convert-outline:before{content:"󱌁"}.mdi-account-cowboy-hat:before{content:"󰺛"}.mdi-account-cowboy-hat-outline:before{content:"󱟳"}.mdi-account-credit-card:before{content:"󱮦"}.mdi-account-credit-card-outline:before{content:"󱮧"}.mdi-account-details:before{content:"󰘱"}.mdi-account-details-outline:before{content:"󱍲"}.mdi-account-edit:before{content:"󰚼"}.mdi-account-edit-outline:before{content:"󰿻"}.mdi-account-eye:before{content:"󰐠"}.mdi-account-eye-outline:before{content:"󱉻"}.mdi-account-filter:before{content:"󰤶"}.mdi-account-filter-outline:before{content:"󰾝"}.mdi-account-group:before{content:"󰡉"}.mdi-account-group-outline:before{content:"󰭘"}.mdi-account-hard-hat:before{content:"󰖵"}.mdi-account-hard-hat-outline:before{content:"󱨟"}.mdi-account-heart:before{content:"󰢙"}.mdi-account-heart-outline:before{content:"󰯣"}.mdi-account-injury:before{content:"󱠕"}.mdi-account-injury-outline:before{content:"󱠖"}.mdi-account-key:before{content:"󰀋"}.mdi-account-key-outline:before{content:"󰯤"}.mdi-account-lock:before{content:"󱅞"}.mdi-account-lock-open:before{content:"󱥠"}.mdi-account-lock-open-outline:before{content:"󱥡"}.mdi-account-lock-outline:before{content:"󱅟"}.mdi-account-minus:before{content:"󰀍"}.mdi-account-minus-outline:before{content:"󰫬"}.mdi-account-multiple:before{content:"󰀎"}.mdi-account-multiple-check:before{content:"󰣅"}.mdi-account-multiple-check-outline:before{content:"󱇾"}.mdi-account-multiple-minus:before{content:"󰗓"}.mdi-account-multiple-minus-outline:before{content:"󰯥"}.mdi-account-multiple-outline:before{content:"󰀏"}.mdi-account-multiple-plus:before{content:"󰀐"}.mdi-account-multiple-plus-outline:before{content:"󰠀"}.mdi-account-multiple-remove:before{content:"󱈊"}.mdi-account-multiple-remove-outline:before{content:"󱈋"}.mdi-account-music:before{content:"󰠃"}.mdi-account-music-outline:before{content:"󰳩"}.mdi-account-network:before{content:"󰀑"}.mdi-account-network-off:before{content:"󱫱"}.mdi-account-network-off-outline:before{content:"󱫲"}.mdi-account-network-outline:before{content:"󰯦"}.mdi-account-off:before{content:"󰀒"}.mdi-account-off-outline:before{content:"󰯧"}.mdi-account-outline:before{content:"󰀓"}.mdi-account-plus:before{content:"󰀔"}.mdi-account-plus-outline:before{content:"󰠁"}.mdi-account-question:before{content:"󰭙"}.mdi-account-question-outline:before{content:"󰭚"}.mdi-account-reactivate:before{content:"󱔫"}.mdi-account-reactivate-outline:before{content:"󱔬"}.mdi-account-remove:before{content:"󰀕"}.mdi-account-remove-outline:before{content:"󰫭"}.mdi-account-school:before{content:"󱨠"}.mdi-account-school-outline:before{content:"󱨡"}.mdi-account-search:before{content:"󰀖"}.mdi-account-search-outline:before{content:"󰤵"}.mdi-account-settings:before{content:"󰘰"}.mdi-account-settings-outline:before{content:"󱃉"}.mdi-account-star:before{content:"󰀗"}.mdi-account-star-outline:before{content:"󰯨"}.mdi-account-supervisor:before{content:"󰪋"}.mdi-account-supervisor-circle:before{content:"󰪌"}.mdi-account-supervisor-circle-outline:before{content:"󱓬"}.mdi-account-supervisor-outline:before{content:"󱄭"}.mdi-account-switch:before{content:"󰀙"}.mdi-account-switch-outline:before{content:"󰓋"}.mdi-account-sync:before{content:"󱤛"}.mdi-account-sync-outline:before{content:"󱤜"}.mdi-account-tie:before{content:"󰳣"}.mdi-account-tie-hat:before{content:"󱢘"}.mdi-account-tie-hat-outline:before{content:"󱢙"}.mdi-account-tie-outline:before{content:"󱃊"}.mdi-account-tie-voice:before{content:"󱌈"}.mdi-account-tie-voice-off:before{content:"󱌊"}.mdi-account-tie-voice-off-outline:before{content:"󱌋"}.mdi-account-tie-voice-outline:before{content:"󱌉"}.mdi-account-tie-woman:before{content:"󱪌"}.mdi-account-voice:before{content:"󰗋"}.mdi-account-voice-off:before{content:"󰻔"}.mdi-account-wrench:before{content:"󱢚"}.mdi-account-wrench-outline:before{content:"󱢛"}.mdi-adjust:before{content:"󰀚"}.mdi-advertisements:before{content:"󱤪"}.mdi-advertisements-off:before{content:"󱤫"}.mdi-air-conditioner:before{content:"󰀛"}.mdi-air-filter:before{content:"󰵃"}.mdi-air-horn:before{content:"󰶬"}.mdi-air-humidifier:before{content:"󱂙"}.mdi-air-humidifier-off:before{content:"󱑦"}.mdi-air-purifier:before{content:"󰵄"}.mdi-air-purifier-off:before{content:"󱭗"}.mdi-airbag:before{content:"󰯩"}.mdi-airballoon:before{content:"󰀜"}.mdi-airballoon-outline:before{content:"󱀋"}.mdi-airplane:before{content:"󰀝"}.mdi-airplane-alert:before{content:"󱡺"}.mdi-airplane-check:before{content:"󱡻"}.mdi-airplane-clock:before{content:"󱡼"}.mdi-airplane-cog:before{content:"󱡽"}.mdi-airplane-edit:before{content:"󱡾"}.mdi-airplane-landing:before{content:"󰗔"}.mdi-airplane-marker:before{content:"󱡿"}.mdi-airplane-minus:before{content:"󱢀"}.mdi-airplane-off:before{content:"󰀞"}.mdi-airplane-plus:before{content:"󱢁"}.mdi-airplane-remove:before{content:"󱢂"}.mdi-airplane-search:before{content:"󱢃"}.mdi-airplane-settings:before{content:"󱢄"}.mdi-airplane-takeoff:before{content:"󰗕"}.mdi-airport:before{content:"󰡋"}.mdi-alarm:before{content:"󰀠"}.mdi-alarm-bell:before{content:"󰞎"}.mdi-alarm-check:before{content:"󰀡"}.mdi-alarm-light:before{content:"󰞏"}.mdi-alarm-light-off:before{content:"󱜞"}.mdi-alarm-light-off-outline:before{content:"󱜟"}.mdi-alarm-light-outline:before{content:"󰯪"}.mdi-alarm-multiple:before{content:"󰀢"}.mdi-alarm-note:before{content:"󰹱"}.mdi-alarm-note-off:before{content:"󰹲"}.mdi-alarm-off:before{content:"󰀣"}.mdi-alarm-panel:before{content:"󱗄"}.mdi-alarm-panel-outline:before{content:"󱗅"}.mdi-alarm-plus:before{content:"󰀤"}.mdi-alarm-snooze:before{content:"󰚎"}.mdi-album:before{content:"󰀥"}.mdi-alert:before{content:"󰀦"}.mdi-alert-box:before{content:"󰀧"}.mdi-alert-box-outline:before{content:"󰳤"}.mdi-alert-circle:before{content:"󰀨"}.mdi-alert-circle-check:before{content:"󱇭"}.mdi-alert-circle-check-outline:before{content:"󱇮"}.mdi-alert-circle-outline:before{content:"󰗖"}.mdi-alert-decagram:before{content:"󰚽"}.mdi-alert-decagram-outline:before{content:"󰳥"}.mdi-alert-minus:before{content:"󱒻"}.mdi-alert-minus-outline:before{content:"󱒾"}.mdi-alert-octagon:before{content:"󰀩"}.mdi-alert-octagon-outline:before{content:"󰳦"}.mdi-alert-octagram:before{content:"󰝧"}.mdi-alert-octagram-outline:before{content:"󰳧"}.mdi-alert-outline:before{content:"󰀪"}.mdi-alert-plus:before{content:"󱒺"}.mdi-alert-plus-outline:before{content:"󱒽"}.mdi-alert-remove:before{content:"󱒼"}.mdi-alert-remove-outline:before{content:"󱒿"}.mdi-alert-rhombus:before{content:"󱇎"}.mdi-alert-rhombus-outline:before{content:"󱇏"}.mdi-alien:before{content:"󰢚"}.mdi-alien-outline:before{content:"󱃋"}.mdi-align-horizontal-center:before{content:"󱇃"}.mdi-align-horizontal-distribute:before{content:"󱥢"}.mdi-align-horizontal-left:before{content:"󱇂"}.mdi-align-horizontal-right:before{content:"󱇄"}.mdi-align-vertical-bottom:before{content:"󱇅"}.mdi-align-vertical-center:before{content:"󱇆"}.mdi-align-vertical-distribute:before{content:"󱥣"}.mdi-align-vertical-top:before{content:"󱇇"}.mdi-all-inclusive:before{content:"󰚾"}.mdi-all-inclusive-box:before{content:"󱢍"}.mdi-all-inclusive-box-outline:before{content:"󱢎"}.mdi-allergy:before{content:"󱉘"}.mdi-alpha:before{content:"󰀫"}.mdi-alpha-a:before{content:"󰫮"}.mdi-alpha-a-box:before{content:"󰬈"}.mdi-alpha-a-box-outline:before{content:"󰯫"}.mdi-alpha-a-circle:before{content:"󰯬"}.mdi-alpha-a-circle-outline:before{content:"󰯭"}.mdi-alpha-b:before{content:"󰫯"}.mdi-alpha-b-box:before{content:"󰬉"}.mdi-alpha-b-box-outline:before{content:"󰯮"}.mdi-alpha-b-circle:before{content:"󰯯"}.mdi-alpha-b-circle-outline:before{content:"󰯰"}.mdi-alpha-c:before{content:"󰫰"}.mdi-alpha-c-box:before{content:"󰬊"}.mdi-alpha-c-box-outline:before{content:"󰯱"}.mdi-alpha-c-circle:before{content:"󰯲"}.mdi-alpha-c-circle-outline:before{content:"󰯳"}.mdi-alpha-d:before{content:"󰫱"}.mdi-alpha-d-box:before{content:"󰬋"}.mdi-alpha-d-box-outline:before{content:"󰯴"}.mdi-alpha-d-circle:before{content:"󰯵"}.mdi-alpha-d-circle-outline:before{content:"󰯶"}.mdi-alpha-e:before{content:"󰫲"}.mdi-alpha-e-box:before{content:"󰬌"}.mdi-alpha-e-box-outline:before{content:"󰯷"}.mdi-alpha-e-circle:before{content:"󰯸"}.mdi-alpha-e-circle-outline:before{content:"󰯹"}.mdi-alpha-f:before{content:"󰫳"}.mdi-alpha-f-box:before{content:"󰬍"}.mdi-alpha-f-box-outline:before{content:"󰯺"}.mdi-alpha-f-circle:before{content:"󰯻"}.mdi-alpha-f-circle-outline:before{content:"󰯼"}.mdi-alpha-g:before{content:"󰫴"}.mdi-alpha-g-box:before{content:"󰬎"}.mdi-alpha-g-box-outline:before{content:"󰯽"}.mdi-alpha-g-circle:before{content:"󰯾"}.mdi-alpha-g-circle-outline:before{content:"󰯿"}.mdi-alpha-h:before{content:"󰫵"}.mdi-alpha-h-box:before{content:"󰬏"}.mdi-alpha-h-box-outline:before{content:"󰰀"}.mdi-alpha-h-circle:before{content:"󰰁"}.mdi-alpha-h-circle-outline:before{content:"󰰂"}.mdi-alpha-i:before{content:"󰫶"}.mdi-alpha-i-box:before{content:"󰬐"}.mdi-alpha-i-box-outline:before{content:"󰰃"}.mdi-alpha-i-circle:before{content:"󰰄"}.mdi-alpha-i-circle-outline:before{content:"󰰅"}.mdi-alpha-j:before{content:"󰫷"}.mdi-alpha-j-box:before{content:"󰬑"}.mdi-alpha-j-box-outline:before{content:"󰰆"}.mdi-alpha-j-circle:before{content:"󰰇"}.mdi-alpha-j-circle-outline:before{content:"󰰈"}.mdi-alpha-k:before{content:"󰫸"}.mdi-alpha-k-box:before{content:"󰬒"}.mdi-alpha-k-box-outline:before{content:"󰰉"}.mdi-alpha-k-circle:before{content:"󰰊"}.mdi-alpha-k-circle-outline:before{content:"󰰋"}.mdi-alpha-l:before{content:"󰫹"}.mdi-alpha-l-box:before{content:"󰬓"}.mdi-alpha-l-box-outline:before{content:"󰰌"}.mdi-alpha-l-circle:before{content:"󰰍"}.mdi-alpha-l-circle-outline:before{content:"󰰎"}.mdi-alpha-m:before{content:"󰫺"}.mdi-alpha-m-box:before{content:"󰬔"}.mdi-alpha-m-box-outline:before{content:"󰰏"}.mdi-alpha-m-circle:before{content:"󰰐"}.mdi-alpha-m-circle-outline:before{content:"󰰑"}.mdi-alpha-n:before{content:"󰫻"}.mdi-alpha-n-box:before{content:"󰬕"}.mdi-alpha-n-box-outline:before{content:"󰰒"}.mdi-alpha-n-circle:before{content:"󰰓"}.mdi-alpha-n-circle-outline:before{content:"󰰔"}.mdi-alpha-o:before{content:"󰫼"}.mdi-alpha-o-box:before{content:"󰬖"}.mdi-alpha-o-box-outline:before{content:"󰰕"}.mdi-alpha-o-circle:before{content:"󰰖"}.mdi-alpha-o-circle-outline:before{content:"󰰗"}.mdi-alpha-p:before{content:"󰫽"}.mdi-alpha-p-box:before{content:"󰬗"}.mdi-alpha-p-box-outline:before{content:"󰰘"}.mdi-alpha-p-circle:before{content:"󰰙"}.mdi-alpha-p-circle-outline:before{content:"󰰚"}.mdi-alpha-q:before{content:"󰫾"}.mdi-alpha-q-box:before{content:"󰬘"}.mdi-alpha-q-box-outline:before{content:"󰰛"}.mdi-alpha-q-circle:before{content:"󰰜"}.mdi-alpha-q-circle-outline:before{content:"󰰝"}.mdi-alpha-r:before{content:"󰫿"}.mdi-alpha-r-box:before{content:"󰬙"}.mdi-alpha-r-box-outline:before{content:"󰰞"}.mdi-alpha-r-circle:before{content:"󰰟"}.mdi-alpha-r-circle-outline:before{content:"󰰠"}.mdi-alpha-s:before{content:"󰬀"}.mdi-alpha-s-box:before{content:"󰬚"}.mdi-alpha-s-box-outline:before{content:"󰰡"}.mdi-alpha-s-circle:before{content:"󰰢"}.mdi-alpha-s-circle-outline:before{content:"󰰣"}.mdi-alpha-t:before{content:"󰬁"}.mdi-alpha-t-box:before{content:"󰬛"}.mdi-alpha-t-box-outline:before{content:"󰰤"}.mdi-alpha-t-circle:before{content:"󰰥"}.mdi-alpha-t-circle-outline:before{content:"󰰦"}.mdi-alpha-u:before{content:"󰬂"}.mdi-alpha-u-box:before{content:"󰬜"}.mdi-alpha-u-box-outline:before{content:"󰰧"}.mdi-alpha-u-circle:before{content:"󰰨"}.mdi-alpha-u-circle-outline:before{content:"󰰩"}.mdi-alpha-v:before{content:"󰬃"}.mdi-alpha-v-box:before{content:"󰬝"}.mdi-alpha-v-box-outline:before{content:"󰰪"}.mdi-alpha-v-circle:before{content:"󰰫"}.mdi-alpha-v-circle-outline:before{content:"󰰬"}.mdi-alpha-w:before{content:"󰬄"}.mdi-alpha-w-box:before{content:"󰬞"}.mdi-alpha-w-box-outline:before{content:"󰰭"}.mdi-alpha-w-circle:before{content:"󰰮"}.mdi-alpha-w-circle-outline:before{content:"󰰯"}.mdi-alpha-x:before{content:"󰬅"}.mdi-alpha-x-box:before{content:"󰬟"}.mdi-alpha-x-box-outline:before{content:"󰰰"}.mdi-alpha-x-circle:before{content:"󰰱"}.mdi-alpha-x-circle-outline:before{content:"󰰲"}.mdi-alpha-y:before{content:"󰬆"}.mdi-alpha-y-box:before{content:"󰬠"}.mdi-alpha-y-box-outline:before{content:"󰰳"}.mdi-alpha-y-circle:before{content:"󰰴"}.mdi-alpha-y-circle-outline:before{content:"󰰵"}.mdi-alpha-z:before{content:"󰬇"}.mdi-alpha-z-box:before{content:"󰬡"}.mdi-alpha-z-box-outline:before{content:"󰰶"}.mdi-alpha-z-circle:before{content:"󰰷"}.mdi-alpha-z-circle-outline:before{content:"󰰸"}.mdi-alphabet-aurebesh:before{content:"󱌬"}.mdi-alphabet-cyrillic:before{content:"󱌭"}.mdi-alphabet-greek:before{content:"󱌮"}.mdi-alphabet-latin:before{content:"󱌯"}.mdi-alphabet-piqad:before{content:"󱌰"}.mdi-alphabet-tengwar:before{content:"󱌷"}.mdi-alphabetical:before{content:"󰀬"}.mdi-alphabetical-off:before{content:"󱀌"}.mdi-alphabetical-variant:before{content:"󱀍"}.mdi-alphabetical-variant-off:before{content:"󱀎"}.mdi-altimeter:before{content:"󰗗"}.mdi-ambulance:before{content:"󰀯"}.mdi-ammunition:before{content:"󰳨"}.mdi-ampersand:before{content:"󰪍"}.mdi-amplifier:before{content:"󰀰"}.mdi-amplifier-off:before{content:"󱆵"}.mdi-anchor:before{content:"󰀱"}.mdi-android:before{content:"󰀲"}.mdi-android-studio:before{content:"󰀴"}.mdi-angle-acute:before{content:"󰤷"}.mdi-angle-obtuse:before{content:"󰤸"}.mdi-angle-right:before{content:"󰤹"}.mdi-angular:before{content:"󰚲"}.mdi-angularjs:before{content:"󰚿"}.mdi-animation:before{content:"󰗘"}.mdi-animation-outline:before{content:"󰪏"}.mdi-animation-play:before{content:"󰤺"}.mdi-animation-play-outline:before{content:"󰪐"}.mdi-ansible:before{content:"󱂚"}.mdi-antenna:before{content:"󱄙"}.mdi-anvil:before{content:"󰢛"}.mdi-apache-kafka:before{content:"󱀏"}.mdi-api:before{content:"󱂛"}.mdi-api-off:before{content:"󱉗"}.mdi-apple:before{content:"󰀵"}.mdi-apple-finder:before{content:"󰀶"}.mdi-apple-icloud:before{content:"󰀸"}.mdi-apple-ios:before{content:"󰀷"}.mdi-apple-keyboard-caps:before{content:"󰘲"}.mdi-apple-keyboard-command:before{content:"󰘳"}.mdi-apple-keyboard-control:before{content:"󰘴"}.mdi-apple-keyboard-option:before{content:"󰘵"}.mdi-apple-keyboard-shift:before{content:"󰘶"}.mdi-apple-safari:before{content:"󰀹"}.mdi-application:before{content:"󰣆"}.mdi-application-array:before{content:"󱃵"}.mdi-application-array-outline:before{content:"󱃶"}.mdi-application-braces:before{content:"󱃷"}.mdi-application-braces-outline:before{content:"󱃸"}.mdi-application-brackets:before{content:"󰲋"}.mdi-application-brackets-outline:before{content:"󰲌"}.mdi-application-cog:before{content:"󰙵"}.mdi-application-cog-outline:before{content:"󱕷"}.mdi-application-edit:before{content:"󰂮"}.mdi-application-edit-outline:before{content:"󰘙"}.mdi-application-export:before{content:"󰶭"}.mdi-application-import:before{content:"󰶮"}.mdi-application-outline:before{content:"󰘔"}.mdi-application-parentheses:before{content:"󱃹"}.mdi-application-parentheses-outline:before{content:"󱃺"}.mdi-application-settings:before{content:"󰭠"}.mdi-application-settings-outline:before{content:"󱕕"}.mdi-application-variable:before{content:"󱃻"}.mdi-application-variable-outline:before{content:"󱃼"}.mdi-approximately-equal:before{content:"󰾞"}.mdi-approximately-equal-box:before{content:"󰾟"}.mdi-apps:before{content:"󰀻"}.mdi-apps-box:before{content:"󰵆"}.mdi-arch:before{content:"󰣇"}.mdi-archive:before{content:"󰀼"}.mdi-archive-alert:before{content:"󱓽"}.mdi-archive-alert-outline:before{content:"󱓾"}.mdi-archive-arrow-down:before{content:"󱉙"}.mdi-archive-arrow-down-outline:before{content:"󱉚"}.mdi-archive-arrow-up:before{content:"󱉛"}.mdi-archive-arrow-up-outline:before{content:"󱉜"}.mdi-archive-cancel:before{content:"󱝋"}.mdi-archive-cancel-outline:before{content:"󱝌"}.mdi-archive-check:before{content:"󱝍"}.mdi-archive-check-outline:before{content:"󱝎"}.mdi-archive-clock:before{content:"󱝏"}.mdi-archive-clock-outline:before{content:"󱝐"}.mdi-archive-cog:before{content:"󱝑"}.mdi-archive-cog-outline:before{content:"󱝒"}.mdi-archive-edit:before{content:"󱝓"}.mdi-archive-edit-outline:before{content:"󱝔"}.mdi-archive-eye:before{content:"󱝕"}.mdi-archive-eye-outline:before{content:"󱝖"}.mdi-archive-lock:before{content:"󱝗"}.mdi-archive-lock-open:before{content:"󱝘"}.mdi-archive-lock-open-outline:before{content:"󱝙"}.mdi-archive-lock-outline:before{content:"󱝚"}.mdi-archive-marker:before{content:"󱝛"}.mdi-archive-marker-outline:before{content:"󱝜"}.mdi-archive-minus:before{content:"󱝝"}.mdi-archive-minus-outline:before{content:"󱝞"}.mdi-archive-music:before{content:"󱝟"}.mdi-archive-music-outline:before{content:"󱝠"}.mdi-archive-off:before{content:"󱝡"}.mdi-archive-off-outline:before{content:"󱝢"}.mdi-archive-outline:before{content:"󱈎"}.mdi-archive-plus:before{content:"󱝣"}.mdi-archive-plus-outline:before{content:"󱝤"}.mdi-archive-refresh:before{content:"󱝥"}.mdi-archive-refresh-outline:before{content:"󱝦"}.mdi-archive-remove:before{content:"󱝧"}.mdi-archive-remove-outline:before{content:"󱝨"}.mdi-archive-search:before{content:"󱝩"}.mdi-archive-search-outline:before{content:"󱝪"}.mdi-archive-settings:before{content:"󱝫"}.mdi-archive-settings-outline:before{content:"󱝬"}.mdi-archive-star:before{content:"󱝭"}.mdi-archive-star-outline:before{content:"󱝮"}.mdi-archive-sync:before{content:"󱝯"}.mdi-archive-sync-outline:before{content:"󱝰"}.mdi-arm-flex:before{content:"󰿗"}.mdi-arm-flex-outline:before{content:"󰿖"}.mdi-arrange-bring-forward:before{content:"󰀽"}.mdi-arrange-bring-to-front:before{content:"󰀾"}.mdi-arrange-send-backward:before{content:"󰀿"}.mdi-arrange-send-to-back:before{content:"󰁀"}.mdi-arrow-all:before{content:"󰁁"}.mdi-arrow-bottom-left:before{content:"󰁂"}.mdi-arrow-bottom-left-bold-box:before{content:"󱥤"}.mdi-arrow-bottom-left-bold-box-outline:before{content:"󱥥"}.mdi-arrow-bottom-left-bold-outline:before{content:"󰦷"}.mdi-arrow-bottom-left-thick:before{content:"󰦸"}.mdi-arrow-bottom-left-thin:before{content:"󱦶"}.mdi-arrow-bottom-left-thin-circle-outline:before{content:"󱖖"}.mdi-arrow-bottom-right:before{content:"󰁃"}.mdi-arrow-bottom-right-bold-box:before{content:"󱥦"}.mdi-arrow-bottom-right-bold-box-outline:before{content:"󱥧"}.mdi-arrow-bottom-right-bold-outline:before{content:"󰦹"}.mdi-arrow-bottom-right-thick:before{content:"󰦺"}.mdi-arrow-bottom-right-thin:before{content:"󱦷"}.mdi-arrow-bottom-right-thin-circle-outline:before{content:"󱖕"}.mdi-arrow-collapse:before{content:"󰘕"}.mdi-arrow-collapse-all:before{content:"󰁄"}.mdi-arrow-collapse-down:before{content:"󰞒"}.mdi-arrow-collapse-horizontal:before{content:"󰡌"}.mdi-arrow-collapse-left:before{content:"󰞓"}.mdi-arrow-collapse-right:before{content:"󰞔"}.mdi-arrow-collapse-up:before{content:"󰞕"}.mdi-arrow-collapse-vertical:before{content:"󰡍"}.mdi-arrow-decision:before{content:"󰦻"}.mdi-arrow-decision-auto:before{content:"󰦼"}.mdi-arrow-decision-auto-outline:before{content:"󰦽"}.mdi-arrow-decision-outline:before{content:"󰦾"}.mdi-arrow-down:before{content:"󰁅"}.mdi-arrow-down-bold:before{content:"󰜮"}.mdi-arrow-down-bold-box:before{content:"󰜯"}.mdi-arrow-down-bold-box-outline:before{content:"󰜰"}.mdi-arrow-down-bold-circle:before{content:"󰁇"}.mdi-arrow-down-bold-circle-outline:before{content:"󰁈"}.mdi-arrow-down-bold-hexagon-outline:before{content:"󰁉"}.mdi-arrow-down-bold-outline:before{content:"󰦿"}.mdi-arrow-down-box:before{content:"󰛀"}.mdi-arrow-down-circle:before{content:"󰳛"}.mdi-arrow-down-circle-outline:before{content:"󰳜"}.mdi-arrow-down-drop-circle:before{content:"󰁊"}.mdi-arrow-down-drop-circle-outline:before{content:"󰁋"}.mdi-arrow-down-left:before{content:"󱞡"}.mdi-arrow-down-left-bold:before{content:"󱞢"}.mdi-arrow-down-right:before{content:"󱞣"}.mdi-arrow-down-right-bold:before{content:"󱞤"}.mdi-arrow-down-thick:before{content:"󰁆"}.mdi-arrow-down-thin:before{content:"󱦳"}.mdi-arrow-down-thin-circle-outline:before{content:"󱖙"}.mdi-arrow-expand:before{content:"󰘖"}.mdi-arrow-expand-all:before{content:"󰁌"}.mdi-arrow-expand-down:before{content:"󰞖"}.mdi-arrow-expand-horizontal:before{content:"󰡎"}.mdi-arrow-expand-left:before{content:"󰞗"}.mdi-arrow-expand-right:before{content:"󰞘"}.mdi-arrow-expand-up:before{content:"󰞙"}.mdi-arrow-expand-vertical:before{content:"󰡏"}.mdi-arrow-horizontal-lock:before{content:"󱅛"}.mdi-arrow-left:before{content:"󰁍"}.mdi-arrow-left-bold:before{content:"󰜱"}.mdi-arrow-left-bold-box:before{content:"󰜲"}.mdi-arrow-left-bold-box-outline:before{content:"󰜳"}.mdi-arrow-left-bold-circle:before{content:"󰁏"}.mdi-arrow-left-bold-circle-outline:before{content:"󰁐"}.mdi-arrow-left-bold-hexagon-outline:before{content:"󰁑"}.mdi-arrow-left-bold-outline:before{content:"󰧀"}.mdi-arrow-left-bottom:before{content:"󱞥"}.mdi-arrow-left-bottom-bold:before{content:"󱞦"}.mdi-arrow-left-box:before{content:"󰛁"}.mdi-arrow-left-circle:before{content:"󰳝"}.mdi-arrow-left-circle-outline:before{content:"󰳞"}.mdi-arrow-left-drop-circle:before{content:"󰁒"}.mdi-arrow-left-drop-circle-outline:before{content:"󰁓"}.mdi-arrow-left-right:before{content:"󰹳"}.mdi-arrow-left-right-bold:before{content:"󰹴"}.mdi-arrow-left-right-bold-outline:before{content:"󰧁"}.mdi-arrow-left-thick:before{content:"󰁎"}.mdi-arrow-left-thin:before{content:"󱦱"}.mdi-arrow-left-thin-circle-outline:before{content:"󱖚"}.mdi-arrow-left-top:before{content:"󱞧"}.mdi-arrow-left-top-bold:before{content:"󱞨"}.mdi-arrow-projectile:before{content:"󱡀"}.mdi-arrow-projectile-multiple:before{content:"󱠿"}.mdi-arrow-right:before{content:"󰁔"}.mdi-arrow-right-bold:before{content:"󰜴"}.mdi-arrow-right-bold-box:before{content:"󰜵"}.mdi-arrow-right-bold-box-outline:before{content:"󰜶"}.mdi-arrow-right-bold-circle:before{content:"󰁖"}.mdi-arrow-right-bold-circle-outline:before{content:"󰁗"}.mdi-arrow-right-bold-hexagon-outline:before{content:"󰁘"}.mdi-arrow-right-bold-outline:before{content:"󰧂"}.mdi-arrow-right-bottom:before{content:"󱞩"}.mdi-arrow-right-bottom-bold:before{content:"󱞪"}.mdi-arrow-right-box:before{content:"󰛂"}.mdi-arrow-right-circle:before{content:"󰳟"}.mdi-arrow-right-circle-outline:before{content:"󰳠"}.mdi-arrow-right-drop-circle:before{content:"󰁙"}.mdi-arrow-right-drop-circle-outline:before{content:"󰁚"}.mdi-arrow-right-thick:before{content:"󰁕"}.mdi-arrow-right-thin:before{content:"󱦰"}.mdi-arrow-right-thin-circle-outline:before{content:"󱖘"}.mdi-arrow-right-top:before{content:"󱞫"}.mdi-arrow-right-top-bold:before{content:"󱞬"}.mdi-arrow-split-horizontal:before{content:"󰤻"}.mdi-arrow-split-vertical:before{content:"󰤼"}.mdi-arrow-top-left:before{content:"󰁛"}.mdi-arrow-top-left-bold-box:before{content:"󱥨"}.mdi-arrow-top-left-bold-box-outline:before{content:"󱥩"}.mdi-arrow-top-left-bold-outline:before{content:"󰧃"}.mdi-arrow-top-left-bottom-right:before{content:"󰹵"}.mdi-arrow-top-left-bottom-right-bold:before{content:"󰹶"}.mdi-arrow-top-left-thick:before{content:"󰧄"}.mdi-arrow-top-left-thin:before{content:"󱦵"}.mdi-arrow-top-left-thin-circle-outline:before{content:"󱖓"}.mdi-arrow-top-right:before{content:"󰁜"}.mdi-arrow-top-right-bold-box:before{content:"󱥪"}.mdi-arrow-top-right-bold-box-outline:before{content:"󱥫"}.mdi-arrow-top-right-bold-outline:before{content:"󰧅"}.mdi-arrow-top-right-bottom-left:before{content:"󰹷"}.mdi-arrow-top-right-bottom-left-bold:before{content:"󰹸"}.mdi-arrow-top-right-thick:before{content:"󰧆"}.mdi-arrow-top-right-thin:before{content:"󱦴"}.mdi-arrow-top-right-thin-circle-outline:before{content:"󱖔"}.mdi-arrow-u-down-left:before{content:"󱞭"}.mdi-arrow-u-down-left-bold:before{content:"󱞮"}.mdi-arrow-u-down-right:before{content:"󱞯"}.mdi-arrow-u-down-right-bold:before{content:"󱞰"}.mdi-arrow-u-left-bottom:before{content:"󱞱"}.mdi-arrow-u-left-bottom-bold:before{content:"󱞲"}.mdi-arrow-u-left-top:before{content:"󱞳"}.mdi-arrow-u-left-top-bold:before{content:"󱞴"}.mdi-arrow-u-right-bottom:before{content:"󱞵"}.mdi-arrow-u-right-bottom-bold:before{content:"󱞶"}.mdi-arrow-u-right-top:before{content:"󱞷"}.mdi-arrow-u-right-top-bold:before{content:"󱞸"}.mdi-arrow-u-up-left:before{content:"󱞹"}.mdi-arrow-u-up-left-bold:before{content:"󱞺"}.mdi-arrow-u-up-right:before{content:"󱞻"}.mdi-arrow-u-up-right-bold:before{content:"󱞼"}.mdi-arrow-up:before{content:"󰁝"}.mdi-arrow-up-bold:before{content:"󰜷"}.mdi-arrow-up-bold-box:before{content:"󰜸"}.mdi-arrow-up-bold-box-outline:before{content:"󰜹"}.mdi-arrow-up-bold-circle:before{content:"󰁟"}.mdi-arrow-up-bold-circle-outline:before{content:"󰁠"}.mdi-arrow-up-bold-hexagon-outline:before{content:"󰁡"}.mdi-arrow-up-bold-outline:before{content:"󰧇"}.mdi-arrow-up-box:before{content:"󰛃"}.mdi-arrow-up-circle:before{content:"󰳡"}.mdi-arrow-up-circle-outline:before{content:"󰳢"}.mdi-arrow-up-down:before{content:"󰹹"}.mdi-arrow-up-down-bold:before{content:"󰹺"}.mdi-arrow-up-down-bold-outline:before{content:"󰧈"}.mdi-arrow-up-drop-circle:before{content:"󰁢"}.mdi-arrow-up-drop-circle-outline:before{content:"󰁣"}.mdi-arrow-up-left:before{content:"󱞽"}.mdi-arrow-up-left-bold:before{content:"󱞾"}.mdi-arrow-up-right:before{content:"󱞿"}.mdi-arrow-up-right-bold:before{content:"󱟀"}.mdi-arrow-up-thick:before{content:"󰁞"}.mdi-arrow-up-thin:before{content:"󱦲"}.mdi-arrow-up-thin-circle-outline:before{content:"󱖗"}.mdi-arrow-vertical-lock:before{content:"󱅜"}.mdi-artboard:before{content:"󱮚"}.mdi-artstation:before{content:"󰭛"}.mdi-aspect-ratio:before{content:"󰨤"}.mdi-assistant:before{content:"󰁤"}.mdi-asterisk:before{content:"󰛄"}.mdi-asterisk-circle-outline:before{content:"󱨧"}.mdi-at:before{content:"󰁥"}.mdi-atlassian:before{content:"󰠄"}.mdi-atm:before{content:"󰵇"}.mdi-atom:before{content:"󰝨"}.mdi-atom-variant:before{content:"󰹻"}.mdi-attachment:before{content:"󰁦"}.mdi-attachment-check:before{content:"󱫁"}.mdi-attachment-lock:before{content:"󱧄"}.mdi-attachment-minus:before{content:"󱫂"}.mdi-attachment-off:before{content:"󱫃"}.mdi-attachment-plus:before{content:"󱫄"}.mdi-attachment-remove:before{content:"󱫅"}.mdi-atv:before{content:"󱭰"}.mdi-audio-input-rca:before{content:"󱡫"}.mdi-audio-input-stereo-minijack:before{content:"󱡬"}.mdi-audio-input-xlr:before{content:"󱡭"}.mdi-audio-video:before{content:"󰤽"}.mdi-audio-video-off:before{content:"󱆶"}.mdi-augmented-reality:before{content:"󰡐"}.mdi-auto-download:before{content:"󱍾"}.mdi-auto-fix:before{content:"󰁨"}.mdi-auto-upload:before{content:"󰁩"}.mdi-autorenew:before{content:"󰁪"}.mdi-autorenew-off:before{content:"󱧧"}.mdi-av-timer:before{content:"󰁫"}.mdi-awning:before{content:"󱮇"}.mdi-awning-outline:before{content:"󱮈"}.mdi-aws:before{content:"󰸏"}.mdi-axe:before{content:"󰣈"}.mdi-axe-battle:before{content:"󱡂"}.mdi-axis:before{content:"󰵈"}.mdi-axis-arrow:before{content:"󰵉"}.mdi-axis-arrow-info:before{content:"󱐎"}.mdi-axis-arrow-lock:before{content:"󰵊"}.mdi-axis-lock:before{content:"󰵋"}.mdi-axis-x-arrow:before{content:"󰵌"}.mdi-axis-x-arrow-lock:before{content:"󰵍"}.mdi-axis-x-rotate-clockwise:before{content:"󰵎"}.mdi-axis-x-rotate-counterclockwise:before{content:"󰵏"}.mdi-axis-x-y-arrow-lock:before{content:"󰵐"}.mdi-axis-y-arrow:before{content:"󰵑"}.mdi-axis-y-arrow-lock:before{content:"󰵒"}.mdi-axis-y-rotate-clockwise:before{content:"󰵓"}.mdi-axis-y-rotate-counterclockwise:before{content:"󰵔"}.mdi-axis-z-arrow:before{content:"󰵕"}.mdi-axis-z-arrow-lock:before{content:"󰵖"}.mdi-axis-z-rotate-clockwise:before{content:"󰵗"}.mdi-axis-z-rotate-counterclockwise:before{content:"󰵘"}.mdi-babel:before{content:"󰨥"}.mdi-baby:before{content:"󰁬"}.mdi-baby-bottle:before{content:"󰼹"}.mdi-baby-bottle-outline:before{content:"󰼺"}.mdi-baby-buggy:before{content:"󱏠"}.mdi-baby-buggy-off:before{content:"󱫳"}.mdi-baby-carriage:before{content:"󰚏"}.mdi-baby-carriage-off:before{content:"󰾠"}.mdi-baby-face:before{content:"󰹼"}.mdi-baby-face-outline:before{content:"󰹽"}.mdi-backburger:before{content:"󰁭"}.mdi-backspace:before{content:"󰁮"}.mdi-backspace-outline:before{content:"󰭜"}.mdi-backspace-reverse:before{content:"󰹾"}.mdi-backspace-reverse-outline:before{content:"󰹿"}.mdi-backup-restore:before{content:"󰁯"}.mdi-bacteria:before{content:"󰻕"}.mdi-bacteria-outline:before{content:"󰻖"}.mdi-badge-account:before{content:"󰶧"}.mdi-badge-account-alert:before{content:"󰶨"}.mdi-badge-account-alert-outline:before{content:"󰶩"}.mdi-badge-account-horizontal:before{content:"󰸍"}.mdi-badge-account-horizontal-outline:before{content:"󰸎"}.mdi-badge-account-outline:before{content:"󰶪"}.mdi-badminton:before{content:"󰡑"}.mdi-bag-carry-on:before{content:"󰼻"}.mdi-bag-carry-on-check:before{content:"󰵥"}.mdi-bag-carry-on-off:before{content:"󰼼"}.mdi-bag-checked:before{content:"󰼽"}.mdi-bag-personal:before{content:"󰸐"}.mdi-bag-personal-off:before{content:"󰸑"}.mdi-bag-personal-off-outline:before{content:"󰸒"}.mdi-bag-personal-outline:before{content:"󰸓"}.mdi-bag-personal-tag:before{content:"󱬌"}.mdi-bag-personal-tag-outline:before{content:"󱬍"}.mdi-bag-suitcase:before{content:"󱖋"}.mdi-bag-suitcase-off:before{content:"󱖍"}.mdi-bag-suitcase-off-outline:before{content:"󱖎"}.mdi-bag-suitcase-outline:before{content:"󱖌"}.mdi-baguette:before{content:"󰼾"}.mdi-balcony:before{content:"󱠗"}.mdi-balloon:before{content:"󰨦"}.mdi-ballot:before{content:"󰧉"}.mdi-ballot-outline:before{content:"󰧊"}.mdi-ballot-recount:before{content:"󰰹"}.mdi-ballot-recount-outline:before{content:"󰰺"}.mdi-bandage:before{content:"󰶯"}.mdi-bank:before{content:"󰁰"}.mdi-bank-check:before{content:"󱙕"}.mdi-bank-minus:before{content:"󰶰"}.mdi-bank-off:before{content:"󱙖"}.mdi-bank-off-outline:before{content:"󱙗"}.mdi-bank-outline:before{content:"󰺀"}.mdi-bank-plus:before{content:"󰶱"}.mdi-bank-remove:before{content:"󰶲"}.mdi-bank-transfer:before{content:"󰨧"}.mdi-bank-transfer-in:before{content:"󰨨"}.mdi-bank-transfer-out:before{content:"󰨩"}.mdi-barcode:before{content:"󰁱"}.mdi-barcode-off:before{content:"󱈶"}.mdi-barcode-scan:before{content:"󰁲"}.mdi-barley:before{content:"󰁳"}.mdi-barley-off:before{content:"󰭝"}.mdi-barn:before{content:"󰭞"}.mdi-barrel:before{content:"󰁴"}.mdi-barrel-outline:before{content:"󱨨"}.mdi-baseball:before{content:"󰡒"}.mdi-baseball-bat:before{content:"󰡓"}.mdi-baseball-diamond:before{content:"󱗬"}.mdi-baseball-diamond-outline:before{content:"󱗭"}.mdi-bash:before{content:"󱆃"}.mdi-basket:before{content:"󰁶"}.mdi-basket-check:before{content:"󱣥"}.mdi-basket-check-outline:before{content:"󱣦"}.mdi-basket-fill:before{content:"󰁷"}.mdi-basket-minus:before{content:"󱔣"}.mdi-basket-minus-outline:before{content:"󱔤"}.mdi-basket-off:before{content:"󱔥"}.mdi-basket-off-outline:before{content:"󱔦"}.mdi-basket-outline:before{content:"󱆁"}.mdi-basket-plus:before{content:"󱔧"}.mdi-basket-plus-outline:before{content:"󱔨"}.mdi-basket-remove:before{content:"󱔩"}.mdi-basket-remove-outline:before{content:"󱔪"}.mdi-basket-unfill:before{content:"󰁸"}.mdi-basketball:before{content:"󰠆"}.mdi-basketball-hoop:before{content:"󰰻"}.mdi-basketball-hoop-outline:before{content:"󰰼"}.mdi-bat:before{content:"󰭟"}.mdi-bathtub:before{content:"󱠘"}.mdi-bathtub-outline:before{content:"󱠙"}.mdi-battery:before{content:"󰁹"}.mdi-battery-10:before{content:"󰁺"}.mdi-battery-10-bluetooth:before{content:"󰤾"}.mdi-battery-20:before{content:"󰁻"}.mdi-battery-20-bluetooth:before{content:"󰤿"}.mdi-battery-30:before{content:"󰁼"}.mdi-battery-30-bluetooth:before{content:"󰥀"}.mdi-battery-40:before{content:"󰁽"}.mdi-battery-40-bluetooth:before{content:"󰥁"}.mdi-battery-50:before{content:"󰁾"}.mdi-battery-50-bluetooth:before{content:"󰥂"}.mdi-battery-60:before{content:"󰁿"}.mdi-battery-60-bluetooth:before{content:"󰥃"}.mdi-battery-70:before{content:"󰂀"}.mdi-battery-70-bluetooth:before{content:"󰥄"}.mdi-battery-80:before{content:"󰂁"}.mdi-battery-80-bluetooth:before{content:"󰥅"}.mdi-battery-90:before{content:"󰂂"}.mdi-battery-90-bluetooth:before{content:"󰥆"}.mdi-battery-alert:before{content:"󰂃"}.mdi-battery-alert-bluetooth:before{content:"󰥇"}.mdi-battery-alert-variant:before{content:"󱃌"}.mdi-battery-alert-variant-outline:before{content:"󱃍"}.mdi-battery-arrow-down:before{content:"󱟞"}.mdi-battery-arrow-down-outline:before{content:"󱟟"}.mdi-battery-arrow-up:before{content:"󱟠"}.mdi-battery-arrow-up-outline:before{content:"󱟡"}.mdi-battery-bluetooth:before{content:"󰥈"}.mdi-battery-bluetooth-variant:before{content:"󰥉"}.mdi-battery-charging:before{content:"󰂄"}.mdi-battery-charging-10:before{content:"󰢜"}.mdi-battery-charging-100:before{content:"󰂅"}.mdi-battery-charging-20:before{content:"󰂆"}.mdi-battery-charging-30:before{content:"󰂇"}.mdi-battery-charging-40:before{content:"󰂈"}.mdi-battery-charging-50:before{content:"󰢝"}.mdi-battery-charging-60:before{content:"󰂉"}.mdi-battery-charging-70:before{content:"󰢞"}.mdi-battery-charging-80:before{content:"󰂊"}.mdi-battery-charging-90:before{content:"󰂋"}.mdi-battery-charging-high:before{content:"󱊦"}.mdi-battery-charging-low:before{content:"󱊤"}.mdi-battery-charging-medium:before{content:"󱊥"}.mdi-battery-charging-outline:before{content:"󰢟"}.mdi-battery-charging-wireless:before{content:"󰠇"}.mdi-battery-charging-wireless-10:before{content:"󰠈"}.mdi-battery-charging-wireless-20:before{content:"󰠉"}.mdi-battery-charging-wireless-30:before{content:"󰠊"}.mdi-battery-charging-wireless-40:before{content:"󰠋"}.mdi-battery-charging-wireless-50:before{content:"󰠌"}.mdi-battery-charging-wireless-60:before{content:"󰠍"}.mdi-battery-charging-wireless-70:before{content:"󰠎"}.mdi-battery-charging-wireless-80:before{content:"󰠏"}.mdi-battery-charging-wireless-90:before{content:"󰠐"}.mdi-battery-charging-wireless-alert:before{content:"󰠑"}.mdi-battery-charging-wireless-outline:before{content:"󰠒"}.mdi-battery-check:before{content:"󱟢"}.mdi-battery-check-outline:before{content:"󱟣"}.mdi-battery-clock:before{content:"󱧥"}.mdi-battery-clock-outline:before{content:"󱧦"}.mdi-battery-heart:before{content:"󱈏"}.mdi-battery-heart-outline:before{content:"󱈐"}.mdi-battery-heart-variant:before{content:"󱈑"}.mdi-battery-high:before{content:"󱊣"}.mdi-battery-lock:before{content:"󱞜"}.mdi-battery-lock-open:before{content:"󱞝"}.mdi-battery-low:before{content:"󱊡"}.mdi-battery-medium:before{content:"󱊢"}.mdi-battery-minus:before{content:"󱟤"}.mdi-battery-minus-outline:before{content:"󱟥"}.mdi-battery-minus-variant:before{content:"󰂌"}.mdi-battery-negative:before{content:"󰂍"}.mdi-battery-off:before{content:"󱉝"}.mdi-battery-off-outline:before{content:"󱉞"}.mdi-battery-outline:before{content:"󰂎"}.mdi-battery-plus:before{content:"󱟦"}.mdi-battery-plus-outline:before{content:"󱟧"}.mdi-battery-plus-variant:before{content:"󰂏"}.mdi-battery-positive:before{content:"󰂐"}.mdi-battery-remove:before{content:"󱟨"}.mdi-battery-remove-outline:before{content:"󱟩"}.mdi-battery-sync:before{content:"󱠴"}.mdi-battery-sync-outline:before{content:"󱠵"}.mdi-battery-unknown:before{content:"󰂑"}.mdi-battery-unknown-bluetooth:before{content:"󰥊"}.mdi-beach:before{content:"󰂒"}.mdi-beaker:before{content:"󰳪"}.mdi-beaker-alert:before{content:"󱈩"}.mdi-beaker-alert-outline:before{content:"󱈪"}.mdi-beaker-check:before{content:"󱈫"}.mdi-beaker-check-outline:before{content:"󱈬"}.mdi-beaker-minus:before{content:"󱈭"}.mdi-beaker-minus-outline:before{content:"󱈮"}.mdi-beaker-outline:before{content:"󰚐"}.mdi-beaker-plus:before{content:"󱈯"}.mdi-beaker-plus-outline:before{content:"󱈰"}.mdi-beaker-question:before{content:"󱈱"}.mdi-beaker-question-outline:before{content:"󱈲"}.mdi-beaker-remove:before{content:"󱈳"}.mdi-beaker-remove-outline:before{content:"󱈴"}.mdi-bed:before{content:"󰋣"}.mdi-bed-clock:before{content:"󱮔"}.mdi-bed-double:before{content:"󰿔"}.mdi-bed-double-outline:before{content:"󰿓"}.mdi-bed-empty:before{content:"󰢠"}.mdi-bed-king:before{content:"󰿒"}.mdi-bed-king-outline:before{content:"󰿑"}.mdi-bed-outline:before{content:"󰂙"}.mdi-bed-queen:before{content:"󰿐"}.mdi-bed-queen-outline:before{content:"󰿛"}.mdi-bed-single:before{content:"󱁭"}.mdi-bed-single-outline:before{content:"󱁮"}.mdi-bee:before{content:"󰾡"}.mdi-bee-flower:before{content:"󰾢"}.mdi-beehive-off-outline:before{content:"󱏭"}.mdi-beehive-outline:before{content:"󱃎"}.mdi-beekeeper:before{content:"󱓢"}.mdi-beer:before{content:"󰂘"}.mdi-beer-outline:before{content:"󱌌"}.mdi-bell:before{content:"󰂚"}.mdi-bell-alert:before{content:"󰵙"}.mdi-bell-alert-outline:before{content:"󰺁"}.mdi-bell-badge:before{content:"󱅫"}.mdi-bell-badge-outline:before{content:"󰅸"}.mdi-bell-cancel:before{content:"󱏧"}.mdi-bell-cancel-outline:before{content:"󱏨"}.mdi-bell-check:before{content:"󱇥"}.mdi-bell-check-outline:before{content:"󱇦"}.mdi-bell-circle:before{content:"󰵚"}.mdi-bell-circle-outline:before{content:"󰵛"}.mdi-bell-cog:before{content:"󱨩"}.mdi-bell-cog-outline:before{content:"󱨪"}.mdi-bell-minus:before{content:"󱏩"}.mdi-bell-minus-outline:before{content:"󱏪"}.mdi-bell-off:before{content:"󰂛"}.mdi-bell-off-outline:before{content:"󰪑"}.mdi-bell-outline:before{content:"󰂜"}.mdi-bell-plus:before{content:"󰂝"}.mdi-bell-plus-outline:before{content:"󰪒"}.mdi-bell-remove:before{content:"󱏫"}.mdi-bell-remove-outline:before{content:"󱏬"}.mdi-bell-ring:before{content:"󰂞"}.mdi-bell-ring-outline:before{content:"󰂟"}.mdi-bell-sleep:before{content:"󰂠"}.mdi-bell-sleep-outline:before{content:"󰪓"}.mdi-beta:before{content:"󰂡"}.mdi-betamax:before{content:"󰧋"}.mdi-biathlon:before{content:"󰸔"}.mdi-bicycle:before{content:"󱂜"}.mdi-bicycle-basket:before{content:"󱈵"}.mdi-bicycle-cargo:before{content:"󱢜"}.mdi-bicycle-electric:before{content:"󱖴"}.mdi-bicycle-penny-farthing:before{content:"󱗩"}.mdi-bike:before{content:"󰂣"}.mdi-bike-fast:before{content:"󱄟"}.mdi-billboard:before{content:"󱀐"}.mdi-billiards:before{content:"󰭡"}.mdi-billiards-rack:before{content:"󰭢"}.mdi-binoculars:before{content:"󰂥"}.mdi-bio:before{content:"󰂦"}.mdi-biohazard:before{content:"󰂧"}.mdi-bird:before{content:"󱗆"}.mdi-bitbucket:before{content:"󰂨"}.mdi-bitcoin:before{content:"󰠓"}.mdi-black-mesa:before{content:"󰂩"}.mdi-blender:before{content:"󰳫"}.mdi-blender-outline:before{content:"󱠚"}.mdi-blender-software:before{content:"󰂫"}.mdi-blinds:before{content:"󰂬"}.mdi-blinds-horizontal:before{content:"󱨫"}.mdi-blinds-horizontal-closed:before{content:"󱨬"}.mdi-blinds-open:before{content:"󱀑"}.mdi-blinds-vertical:before{content:"󱨭"}.mdi-blinds-vertical-closed:before{content:"󱨮"}.mdi-block-helper:before{content:"󰂭"}.mdi-blood-bag:before{content:"󰳬"}.mdi-bluetooth:before{content:"󰂯"}.mdi-bluetooth-audio:before{content:"󰂰"}.mdi-bluetooth-connect:before{content:"󰂱"}.mdi-bluetooth-off:before{content:"󰂲"}.mdi-bluetooth-settings:before{content:"󰂳"}.mdi-bluetooth-transfer:before{content:"󰂴"}.mdi-blur:before{content:"󰂵"}.mdi-blur-linear:before{content:"󰂶"}.mdi-blur-off:before{content:"󰂷"}.mdi-blur-radial:before{content:"󰂸"}.mdi-bolt:before{content:"󰶳"}.mdi-bomb:before{content:"󰚑"}.mdi-bomb-off:before{content:"󰛅"}.mdi-bone:before{content:"󰂹"}.mdi-bone-off:before{content:"󱧠"}.mdi-book:before{content:"󰂺"}.mdi-book-account:before{content:"󱎭"}.mdi-book-account-outline:before{content:"󱎮"}.mdi-book-alert:before{content:"󱙼"}.mdi-book-alert-outline:before{content:"󱙽"}.mdi-book-alphabet:before{content:"󰘝"}.mdi-book-arrow-down:before{content:"󱙾"}.mdi-book-arrow-down-outline:before{content:"󱙿"}.mdi-book-arrow-left:before{content:"󱚀"}.mdi-book-arrow-left-outline:before{content:"󱚁"}.mdi-book-arrow-right:before{content:"󱚂"}.mdi-book-arrow-right-outline:before{content:"󱚃"}.mdi-book-arrow-up:before{content:"󱚄"}.mdi-book-arrow-up-outline:before{content:"󱚅"}.mdi-book-cancel:before{content:"󱚆"}.mdi-book-cancel-outline:before{content:"󱚇"}.mdi-book-check:before{content:"󱓳"}.mdi-book-check-outline:before{content:"󱓴"}.mdi-book-clock:before{content:"󱚈"}.mdi-book-clock-outline:before{content:"󱚉"}.mdi-book-cog:before{content:"󱚊"}.mdi-book-cog-outline:before{content:"󱚋"}.mdi-book-cross:before{content:"󰂢"}.mdi-book-edit:before{content:"󱚌"}.mdi-book-edit-outline:before{content:"󱚍"}.mdi-book-education:before{content:"󱛉"}.mdi-book-education-outline:before{content:"󱛊"}.mdi-book-heart:before{content:"󱨝"}.mdi-book-heart-outline:before{content:"󱨞"}.mdi-book-information-variant:before{content:"󱁯"}.mdi-book-lock:before{content:"󰞚"}.mdi-book-lock-open:before{content:"󰞛"}.mdi-book-lock-open-outline:before{content:"󱚎"}.mdi-book-lock-outline:before{content:"󱚏"}.mdi-book-marker:before{content:"󱚐"}.mdi-book-marker-outline:before{content:"󱚑"}.mdi-book-minus:before{content:"󰗙"}.mdi-book-minus-multiple:before{content:"󰪔"}.mdi-book-minus-multiple-outline:before{content:"󰤋"}.mdi-book-minus-outline:before{content:"󱚒"}.mdi-book-multiple:before{content:"󰂻"}.mdi-book-multiple-outline:before{content:"󰐶"}.mdi-book-music:before{content:"󰁧"}.mdi-book-music-outline:before{content:"󱚓"}.mdi-book-off:before{content:"󱚔"}.mdi-book-off-outline:before{content:"󱚕"}.mdi-book-open:before{content:"󰂽"}.mdi-book-open-blank-variant:before{content:"󰂾"}.mdi-book-open-outline:before{content:"󰭣"}.mdi-book-open-page-variant:before{content:"󰗚"}.mdi-book-open-page-variant-outline:before{content:"󱗖"}.mdi-book-open-variant:before{content:"󱓷"}.mdi-book-outline:before{content:"󰭤"}.mdi-book-play:before{content:"󰺂"}.mdi-book-play-outline:before{content:"󰺃"}.mdi-book-plus:before{content:"󰗛"}.mdi-book-plus-multiple:before{content:"󰪕"}.mdi-book-plus-multiple-outline:before{content:"󰫞"}.mdi-book-plus-outline:before{content:"󱚖"}.mdi-book-refresh:before{content:"󱚗"}.mdi-book-refresh-outline:before{content:"󱚘"}.mdi-book-remove:before{content:"󰪗"}.mdi-book-remove-multiple:before{content:"󰪖"}.mdi-book-remove-multiple-outline:before{content:"󰓊"}.mdi-book-remove-outline:before{content:"󱚙"}.mdi-book-search:before{content:"󰺄"}.mdi-book-search-outline:before{content:"󰺅"}.mdi-book-settings:before{content:"󱚚"}.mdi-book-settings-outline:before{content:"󱚛"}.mdi-book-sync:before{content:"󱚜"}.mdi-book-sync-outline:before{content:"󱛈"}.mdi-book-variant:before{content:"󰂿"}.mdi-bookmark:before{content:"󰃀"}.mdi-bookmark-box:before{content:"󱭵"}.mdi-bookmark-box-multiple:before{content:"󱥬"}.mdi-bookmark-box-multiple-outline:before{content:"󱥭"}.mdi-bookmark-box-outline:before{content:"󱭶"}.mdi-bookmark-check:before{content:"󰃁"}.mdi-bookmark-check-outline:before{content:"󱍻"}.mdi-bookmark-minus:before{content:"󰧌"}.mdi-bookmark-minus-outline:before{content:"󰧍"}.mdi-bookmark-multiple:before{content:"󰸕"}.mdi-bookmark-multiple-outline:before{content:"󰸖"}.mdi-bookmark-music:before{content:"󰃂"}.mdi-bookmark-music-outline:before{content:"󱍹"}.mdi-bookmark-off:before{content:"󰧎"}.mdi-bookmark-off-outline:before{content:"󰧏"}.mdi-bookmark-outline:before{content:"󰃃"}.mdi-bookmark-plus:before{content:"󰃅"}.mdi-bookmark-plus-outline:before{content:"󰃄"}.mdi-bookmark-remove:before{content:"󰃆"}.mdi-bookmark-remove-outline:before{content:"󱍺"}.mdi-bookshelf:before{content:"󱉟"}.mdi-boom-gate:before{content:"󰺆"}.mdi-boom-gate-alert:before{content:"󰺇"}.mdi-boom-gate-alert-outline:before{content:"󰺈"}.mdi-boom-gate-arrow-down:before{content:"󰺉"}.mdi-boom-gate-arrow-down-outline:before{content:"󰺊"}.mdi-boom-gate-arrow-up:before{content:"󰺌"}.mdi-boom-gate-arrow-up-outline:before{content:"󰺍"}.mdi-boom-gate-outline:before{content:"󰺋"}.mdi-boom-gate-up:before{content:"󱟹"}.mdi-boom-gate-up-outline:before{content:"󱟺"}.mdi-boombox:before{content:"󰗜"}.mdi-boomerang:before{content:"󱃏"}.mdi-bootstrap:before{content:"󰛆"}.mdi-border-all:before{content:"󰃇"}.mdi-border-all-variant:before{content:"󰢡"}.mdi-border-bottom:before{content:"󰃈"}.mdi-border-bottom-variant:before{content:"󰢢"}.mdi-border-color:before{content:"󰃉"}.mdi-border-horizontal:before{content:"󰃊"}.mdi-border-inside:before{content:"󰃋"}.mdi-border-left:before{content:"󰃌"}.mdi-border-left-variant:before{content:"󰢣"}.mdi-border-none:before{content:"󰃍"}.mdi-border-none-variant:before{content:"󰢤"}.mdi-border-outside:before{content:"󰃎"}.mdi-border-radius:before{content:"󱫴"}.mdi-border-right:before{content:"󰃏"}.mdi-border-right-variant:before{content:"󰢥"}.mdi-border-style:before{content:"󰃐"}.mdi-border-top:before{content:"󰃑"}.mdi-border-top-variant:before{content:"󰢦"}.mdi-border-vertical:before{content:"󰃒"}.mdi-bottle-soda:before{content:"󱁰"}.mdi-bottle-soda-classic:before{content:"󱁱"}.mdi-bottle-soda-classic-outline:before{content:"󱍣"}.mdi-bottle-soda-outline:before{content:"󱁲"}.mdi-bottle-tonic:before{content:"󱄮"}.mdi-bottle-tonic-outline:before{content:"󱄯"}.mdi-bottle-tonic-plus:before{content:"󱄰"}.mdi-bottle-tonic-plus-outline:before{content:"󱄱"}.mdi-bottle-tonic-skull:before{content:"󱄲"}.mdi-bottle-tonic-skull-outline:before{content:"󱄳"}.mdi-bottle-wine:before{content:"󰡔"}.mdi-bottle-wine-outline:before{content:"󱌐"}.mdi-bow-arrow:before{content:"󱡁"}.mdi-bow-tie:before{content:"󰙸"}.mdi-bowl:before{content:"󰊎"}.mdi-bowl-mix:before{content:"󰘗"}.mdi-bowl-mix-outline:before{content:"󰋤"}.mdi-bowl-outline:before{content:"󰊩"}.mdi-bowling:before{content:"󰃓"}.mdi-box:before{content:"󰃔"}.mdi-box-cutter:before{content:"󰃕"}.mdi-box-cutter-off:before{content:"󰭊"}.mdi-box-shadow:before{content:"󰘷"}.mdi-boxing-glove:before{content:"󰭥"}.mdi-braille:before{content:"󰧐"}.mdi-brain:before{content:"󰧑"}.mdi-bread-slice:before{content:"󰳮"}.mdi-bread-slice-outline:before{content:"󰳯"}.mdi-bridge:before{content:"󰘘"}.mdi-briefcase:before{content:"󰃖"}.mdi-briefcase-account:before{content:"󰳰"}.mdi-briefcase-account-outline:before{content:"󰳱"}.mdi-briefcase-arrow-left-right:before{content:"󱪍"}.mdi-briefcase-arrow-left-right-outline:before{content:"󱪎"}.mdi-briefcase-arrow-up-down:before{content:"󱪏"}.mdi-briefcase-arrow-up-down-outline:before{content:"󱪐"}.mdi-briefcase-check:before{content:"󰃗"}.mdi-briefcase-check-outline:before{content:"󱌞"}.mdi-briefcase-clock:before{content:"󱃐"}.mdi-briefcase-clock-outline:before{content:"󱃑"}.mdi-briefcase-download:before{content:"󰃘"}.mdi-briefcase-download-outline:before{content:"󰰽"}.mdi-briefcase-edit:before{content:"󰪘"}.mdi-briefcase-edit-outline:before{content:"󰰾"}.mdi-briefcase-eye:before{content:"󱟙"}.mdi-briefcase-eye-outline:before{content:"󱟚"}.mdi-briefcase-minus:before{content:"󰨪"}.mdi-briefcase-minus-outline:before{content:"󰰿"}.mdi-briefcase-off:before{content:"󱙘"}.mdi-briefcase-off-outline:before{content:"󱙙"}.mdi-briefcase-outline:before{content:"󰠔"}.mdi-briefcase-plus:before{content:"󰨫"}.mdi-briefcase-plus-outline:before{content:"󰱀"}.mdi-briefcase-remove:before{content:"󰨬"}.mdi-briefcase-remove-outline:before{content:"󰱁"}.mdi-briefcase-search:before{content:"󰨭"}.mdi-briefcase-search-outline:before{content:"󰱂"}.mdi-briefcase-upload:before{content:"󰃙"}.mdi-briefcase-upload-outline:before{content:"󰱃"}.mdi-briefcase-variant:before{content:"󱒔"}.mdi-briefcase-variant-off:before{content:"󱙚"}.mdi-briefcase-variant-off-outline:before{content:"󱙛"}.mdi-briefcase-variant-outline:before{content:"󱒕"}.mdi-brightness-1:before{content:"󰃚"}.mdi-brightness-2:before{content:"󰃛"}.mdi-brightness-3:before{content:"󰃜"}.mdi-brightness-4:before{content:"󰃝"}.mdi-brightness-5:before{content:"󰃞"}.mdi-brightness-6:before{content:"󰃟"}.mdi-brightness-7:before{content:"󰃠"}.mdi-brightness-auto:before{content:"󰃡"}.mdi-brightness-percent:before{content:"󰳲"}.mdi-broadcast:before{content:"󱜠"}.mdi-broadcast-off:before{content:"󱜡"}.mdi-broom:before{content:"󰃢"}.mdi-brush:before{content:"󰃣"}.mdi-brush-off:before{content:"󱝱"}.mdi-brush-outline:before{content:"󱨍"}.mdi-brush-variant:before{content:"󱠓"}.mdi-bucket:before{content:"󱐕"}.mdi-bucket-outline:before{content:"󱐖"}.mdi-buffet:before{content:"󰕸"}.mdi-bug:before{content:"󰃤"}.mdi-bug-check:before{content:"󰨮"}.mdi-bug-check-outline:before{content:"󰨯"}.mdi-bug-outline:before{content:"󰨰"}.mdi-bug-pause:before{content:"󱫵"}.mdi-bug-pause-outline:before{content:"󱫶"}.mdi-bug-play:before{content:"󱫷"}.mdi-bug-play-outline:before{content:"󱫸"}.mdi-bug-stop:before{content:"󱫹"}.mdi-bug-stop-outline:before{content:"󱫺"}.mdi-bugle:before{content:"󰶴"}.mdi-bulkhead-light:before{content:"󱨯"}.mdi-bulldozer:before{content:"󰬢"}.mdi-bullet:before{content:"󰳳"}.mdi-bulletin-board:before{content:"󰃥"}.mdi-bullhorn:before{content:"󰃦"}.mdi-bullhorn-outline:before{content:"󰬣"}.mdi-bullhorn-variant:before{content:"󱥮"}.mdi-bullhorn-variant-outline:before{content:"󱥯"}.mdi-bullseye:before{content:"󰗝"}.mdi-bullseye-arrow:before{content:"󰣉"}.mdi-bulma:before{content:"󱋧"}.mdi-bunk-bed:before{content:"󱌂"}.mdi-bunk-bed-outline:before{content:"󰂗"}.mdi-bus:before{content:"󰃧"}.mdi-bus-alert:before{content:"󰪙"}.mdi-bus-articulated-end:before{content:"󰞜"}.mdi-bus-articulated-front:before{content:"󰞝"}.mdi-bus-clock:before{content:"󰣊"}.mdi-bus-double-decker:before{content:"󰞞"}.mdi-bus-electric:before{content:"󱤝"}.mdi-bus-marker:before{content:"󱈒"}.mdi-bus-multiple:before{content:"󰼿"}.mdi-bus-school:before{content:"󰞟"}.mdi-bus-side:before{content:"󰞠"}.mdi-bus-stop:before{content:"󱀒"}.mdi-bus-stop-covered:before{content:"󱀓"}.mdi-bus-stop-uncovered:before{content:"󱀔"}.mdi-butterfly:before{content:"󱖉"}.mdi-butterfly-outline:before{content:"󱖊"}.mdi-button-cursor:before{content:"󱭏"}.mdi-button-pointer:before{content:"󱭐"}.mdi-cabin-a-frame:before{content:"󱢌"}.mdi-cable-data:before{content:"󱎔"}.mdi-cached:before{content:"󰃨"}.mdi-cactus:before{content:"󰶵"}.mdi-cake:before{content:"󰃩"}.mdi-cake-layered:before{content:"󰃪"}.mdi-cake-variant:before{content:"󰃫"}.mdi-cake-variant-outline:before{content:"󱟰"}.mdi-calculator:before{content:"󰃬"}.mdi-calculator-variant:before{content:"󰪚"}.mdi-calculator-variant-outline:before{content:"󱖦"}.mdi-calendar:before{content:"󰃭"}.mdi-calendar-account:before{content:"󰻗"}.mdi-calendar-account-outline:before{content:"󰻘"}.mdi-calendar-alert:before{content:"󰨱"}.mdi-calendar-alert-outline:before{content:"󱭢"}.mdi-calendar-arrow-left:before{content:"󱄴"}.mdi-calendar-arrow-right:before{content:"󱄵"}.mdi-calendar-badge:before{content:"󱮝"}.mdi-calendar-badge-outline:before{content:"󱮞"}.mdi-calendar-blank:before{content:"󰃮"}.mdi-calendar-blank-multiple:before{content:"󱁳"}.mdi-calendar-blank-outline:before{content:"󰭦"}.mdi-calendar-check:before{content:"󰃯"}.mdi-calendar-check-outline:before{content:"󰱄"}.mdi-calendar-clock:before{content:"󰃰"}.mdi-calendar-clock-outline:before{content:"󱛡"}.mdi-calendar-collapse-horizontal:before{content:"󱢝"}.mdi-calendar-collapse-horizontal-outline:before{content:"󱭣"}.mdi-calendar-cursor:before{content:"󱕻"}.mdi-calendar-cursor-outline:before{content:"󱭤"}.mdi-calendar-edit:before{content:"󰢧"}.mdi-calendar-edit-outline:before{content:"󱭥"}.mdi-calendar-end:before{content:"󱙬"}.mdi-calendar-end-outline:before{content:"󱭦"}.mdi-calendar-expand-horizontal:before{content:"󱢞"}.mdi-calendar-expand-horizontal-outline:before{content:"󱭧"}.mdi-calendar-export:before{content:"󰬤"}.mdi-calendar-export-outline:before{content:"󱭨"}.mdi-calendar-filter:before{content:"󱨲"}.mdi-calendar-filter-outline:before{content:"󱨳"}.mdi-calendar-heart:before{content:"󰧒"}.mdi-calendar-heart-outline:before{content:"󱭩"}.mdi-calendar-import:before{content:"󰬥"}.mdi-calendar-import-outline:before{content:"󱭪"}.mdi-calendar-lock:before{content:"󱙁"}.mdi-calendar-lock-open:before{content:"󱭛"}.mdi-calendar-lock-open-outline:before{content:"󱭜"}.mdi-calendar-lock-outline:before{content:"󱙂"}.mdi-calendar-minus:before{content:"󰵜"}.mdi-calendar-minus-outline:before{content:"󱭫"}.mdi-calendar-month:before{content:"󰸗"}.mdi-calendar-month-outline:before{content:"󰸘"}.mdi-calendar-multiple:before{content:"󰃱"}.mdi-calendar-multiple-check:before{content:"󰃲"}.mdi-calendar-multiselect:before{content:"󰨲"}.mdi-calendar-multiselect-outline:before{content:"󱭕"}.mdi-calendar-outline:before{content:"󰭧"}.mdi-calendar-plus:before{content:"󰃳"}.mdi-calendar-plus-outline:before{content:"󱭬"}.mdi-calendar-question:before{content:"󰚒"}.mdi-calendar-question-outline:before{content:"󱭭"}.mdi-calendar-range:before{content:"󰙹"}.mdi-calendar-range-outline:before{content:"󰭨"}.mdi-calendar-refresh:before{content:"󰇡"}.mdi-calendar-refresh-outline:before{content:"󰈃"}.mdi-calendar-remove:before{content:"󰃴"}.mdi-calendar-remove-outline:before{content:"󰱅"}.mdi-calendar-search:before{content:"󰥌"}.mdi-calendar-search-outline:before{content:"󱭮"}.mdi-calendar-star:before{content:"󰧓"}.mdi-calendar-star-outline:before{content:"󱭓"}.mdi-calendar-start:before{content:"󱙭"}.mdi-calendar-start-outline:before{content:"󱭯"}.mdi-calendar-sync:before{content:"󰺎"}.mdi-calendar-sync-outline:before{content:"󰺏"}.mdi-calendar-text:before{content:"󰃵"}.mdi-calendar-text-outline:before{content:"󰱆"}.mdi-calendar-today:before{content:"󰃶"}.mdi-calendar-today-outline:before{content:"󱨰"}.mdi-calendar-week:before{content:"󰨳"}.mdi-calendar-week-begin:before{content:"󰨴"}.mdi-calendar-week-begin-outline:before{content:"󱨱"}.mdi-calendar-week-outline:before{content:"󱨴"}.mdi-calendar-weekend:before{content:"󰻙"}.mdi-calendar-weekend-outline:before{content:"󰻚"}.mdi-call-made:before{content:"󰃷"}.mdi-call-merge:before{content:"󰃸"}.mdi-call-missed:before{content:"󰃹"}.mdi-call-received:before{content:"󰃺"}.mdi-call-split:before{content:"󰃻"}.mdi-camcorder:before{content:"󰃼"}.mdi-camcorder-off:before{content:"󰃿"}.mdi-camera:before{content:"󰄀"}.mdi-camera-account:before{content:"󰣋"}.mdi-camera-burst:before{content:"󰚓"}.mdi-camera-control:before{content:"󰭩"}.mdi-camera-document:before{content:"󱡱"}.mdi-camera-document-off:before{content:"󱡲"}.mdi-camera-enhance:before{content:"󰄁"}.mdi-camera-enhance-outline:before{content:"󰭪"}.mdi-camera-flip:before{content:"󱗙"}.mdi-camera-flip-outline:before{content:"󱗚"}.mdi-camera-front:before{content:"󰄂"}.mdi-camera-front-variant:before{content:"󰄃"}.mdi-camera-gopro:before{content:"󰞡"}.mdi-camera-image:before{content:"󰣌"}.mdi-camera-iris:before{content:"󰄄"}.mdi-camera-lock:before{content:"󱨔"}.mdi-camera-lock-outline:before{content:"󱨕"}.mdi-camera-marker:before{content:"󱦧"}.mdi-camera-marker-outline:before{content:"󱦨"}.mdi-camera-metering-center:before{content:"󰞢"}.mdi-camera-metering-matrix:before{content:"󰞣"}.mdi-camera-metering-partial:before{content:"󰞤"}.mdi-camera-metering-spot:before{content:"󰞥"}.mdi-camera-off:before{content:"󰗟"}.mdi-camera-off-outline:before{content:"󱦿"}.mdi-camera-outline:before{content:"󰵝"}.mdi-camera-party-mode:before{content:"󰄅"}.mdi-camera-plus:before{content:"󰻛"}.mdi-camera-plus-outline:before{content:"󰻜"}.mdi-camera-rear:before{content:"󰄆"}.mdi-camera-rear-variant:before{content:"󰄇"}.mdi-camera-retake:before{content:"󰸙"}.mdi-camera-retake-outline:before{content:"󰸚"}.mdi-camera-switch:before{content:"󰄈"}.mdi-camera-switch-outline:before{content:"󰡊"}.mdi-camera-timer:before{content:"󰄉"}.mdi-camera-wireless:before{content:"󰶶"}.mdi-camera-wireless-outline:before{content:"󰶷"}.mdi-campfire:before{content:"󰻝"}.mdi-cancel:before{content:"󰜺"}.mdi-candelabra:before{content:"󱟒"}.mdi-candelabra-fire:before{content:"󱟓"}.mdi-candle:before{content:"󰗢"}.mdi-candy:before{content:"󱥰"}.mdi-candy-off:before{content:"󱥱"}.mdi-candy-off-outline:before{content:"󱥲"}.mdi-candy-outline:before{content:"󱥳"}.mdi-candycane:before{content:"󰄊"}.mdi-cannabis:before{content:"󰞦"}.mdi-cannabis-off:before{content:"󱙮"}.mdi-caps-lock:before{content:"󰪛"}.mdi-car:before{content:"󰄋"}.mdi-car-2-plus:before{content:"󱀕"}.mdi-car-3-plus:before{content:"󱀖"}.mdi-car-arrow-left:before{content:"󱎲"}.mdi-car-arrow-right:before{content:"󱎳"}.mdi-car-back:before{content:"󰸛"}.mdi-car-battery:before{content:"󰄌"}.mdi-car-brake-abs:before{content:"󰱇"}.mdi-car-brake-alert:before{content:"󰱈"}.mdi-car-brake-fluid-level:before{content:"󱤉"}.mdi-car-brake-hold:before{content:"󰵞"}.mdi-car-brake-low-pressure:before{content:"󱤊"}.mdi-car-brake-parking:before{content:"󰵟"}.mdi-car-brake-retarder:before{content:"󱀗"}.mdi-car-brake-temperature:before{content:"󱤋"}.mdi-car-brake-worn-linings:before{content:"󱤌"}.mdi-car-child-seat:before{content:"󰾣"}.mdi-car-clock:before{content:"󱥴"}.mdi-car-clutch:before{content:"󱀘"}.mdi-car-cog:before{content:"󱏌"}.mdi-car-connected:before{content:"󰄍"}.mdi-car-convertible:before{content:"󰞧"}.mdi-car-coolant-level:before{content:"󱀙"}.mdi-car-cruise-control:before{content:"󰵠"}.mdi-car-defrost-front:before{content:"󰵡"}.mdi-car-defrost-rear:before{content:"󰵢"}.mdi-car-door:before{content:"󰭫"}.mdi-car-door-lock:before{content:"󱂝"}.mdi-car-electric:before{content:"󰭬"}.mdi-car-electric-outline:before{content:"󱖵"}.mdi-car-emergency:before{content:"󱘏"}.mdi-car-esp:before{content:"󰱉"}.mdi-car-estate:before{content:"󰞨"}.mdi-car-hatchback:before{content:"󰞩"}.mdi-car-info:before{content:"󱆾"}.mdi-car-key:before{content:"󰭭"}.mdi-car-lifted-pickup:before{content:"󱔭"}.mdi-car-light-alert:before{content:"󱤍"}.mdi-car-light-dimmed:before{content:"󰱊"}.mdi-car-light-fog:before{content:"󰱋"}.mdi-car-light-high:before{content:"󰱌"}.mdi-car-limousine:before{content:"󰣍"}.mdi-car-multiple:before{content:"󰭮"}.mdi-car-off:before{content:"󰸜"}.mdi-car-outline:before{content:"󱓭"}.mdi-car-parking-lights:before{content:"󰵣"}.mdi-car-pickup:before{content:"󰞪"}.mdi-car-search:before{content:"󱮍"}.mdi-car-search-outline:before{content:"󱮎"}.mdi-car-seat:before{content:"󰾤"}.mdi-car-seat-cooler:before{content:"󰾥"}.mdi-car-seat-heater:before{content:"󰾦"}.mdi-car-select:before{content:"󱡹"}.mdi-car-settings:before{content:"󱏍"}.mdi-car-shift-pattern:before{content:"󰽀"}.mdi-car-side:before{content:"󰞫"}.mdi-car-speed-limiter:before{content:"󱤎"}.mdi-car-sports:before{content:"󰞬"}.mdi-car-tire-alert:before{content:"󰱍"}.mdi-car-traction-control:before{content:"󰵤"}.mdi-car-turbocharger:before{content:"󱀚"}.mdi-car-wash:before{content:"󰄎"}.mdi-car-windshield:before{content:"󱀛"}.mdi-car-windshield-outline:before{content:"󱀜"}.mdi-car-wireless:before{content:"󱡸"}.mdi-car-wrench:before{content:"󱠔"}.mdi-carabiner:before{content:"󱓀"}.mdi-caravan:before{content:"󰞭"}.mdi-card:before{content:"󰭯"}.mdi-card-account-details:before{content:"󰗒"}.mdi-card-account-details-outline:before{content:"󰶫"}.mdi-card-account-details-star:before{content:"󰊣"}.mdi-card-account-details-star-outline:before{content:"󰛛"}.mdi-card-account-mail:before{content:"󰆎"}.mdi-card-account-mail-outline:before{content:"󰺘"}.mdi-card-account-phone:before{content:"󰺙"}.mdi-card-account-phone-outline:before{content:"󰺚"}.mdi-card-bulleted:before{content:"󰭰"}.mdi-card-bulleted-off:before{content:"󰭱"}.mdi-card-bulleted-off-outline:before{content:"󰭲"}.mdi-card-bulleted-outline:before{content:"󰭳"}.mdi-card-bulleted-settings:before{content:"󰭴"}.mdi-card-bulleted-settings-outline:before{content:"󰭵"}.mdi-card-minus:before{content:"󱘀"}.mdi-card-minus-outline:before{content:"󱘁"}.mdi-card-multiple:before{content:"󱟱"}.mdi-card-multiple-outline:before{content:"󱟲"}.mdi-card-off:before{content:"󱘂"}.mdi-card-off-outline:before{content:"󱘃"}.mdi-card-outline:before{content:"󰭶"}.mdi-card-plus:before{content:"󱇿"}.mdi-card-plus-outline:before{content:"󱈀"}.mdi-card-remove:before{content:"󱘄"}.mdi-card-remove-outline:before{content:"󱘅"}.mdi-card-search:before{content:"󱁴"}.mdi-card-search-outline:before{content:"󱁵"}.mdi-card-text:before{content:"󰭷"}.mdi-card-text-outline:before{content:"󰭸"}.mdi-cards:before{content:"󰘸"}.mdi-cards-club:before{content:"󰣎"}.mdi-cards-club-outline:before{content:"󱢟"}.mdi-cards-diamond:before{content:"󰣏"}.mdi-cards-diamond-outline:before{content:"󱀝"}.mdi-cards-heart:before{content:"󰣐"}.mdi-cards-heart-outline:before{content:"󱢠"}.mdi-cards-outline:before{content:"󰘹"}.mdi-cards-playing:before{content:"󱢡"}.mdi-cards-playing-club:before{content:"󱢢"}.mdi-cards-playing-club-multiple:before{content:"󱢣"}.mdi-cards-playing-club-multiple-outline:before{content:"󱢤"}.mdi-cards-playing-club-outline:before{content:"󱢥"}.mdi-cards-playing-diamond:before{content:"󱢦"}.mdi-cards-playing-diamond-multiple:before{content:"󱢧"}.mdi-cards-playing-diamond-multiple-outline:before{content:"󱢨"}.mdi-cards-playing-diamond-outline:before{content:"󱢩"}.mdi-cards-playing-heart:before{content:"󱢪"}.mdi-cards-playing-heart-multiple:before{content:"󱢫"}.mdi-cards-playing-heart-multiple-outline:before{content:"󱢬"}.mdi-cards-playing-heart-outline:before{content:"󱢭"}.mdi-cards-playing-outline:before{content:"󰘺"}.mdi-cards-playing-spade:before{content:"󱢮"}.mdi-cards-playing-spade-multiple:before{content:"󱢯"}.mdi-cards-playing-spade-multiple-outline:before{content:"󱢰"}.mdi-cards-playing-spade-outline:before{content:"󱢱"}.mdi-cards-spade:before{content:"󰣑"}.mdi-cards-spade-outline:before{content:"󱢲"}.mdi-cards-variant:before{content:"󰛇"}.mdi-carrot:before{content:"󰄏"}.mdi-cart:before{content:"󰄐"}.mdi-cart-arrow-down:before{content:"󰵦"}.mdi-cart-arrow-right:before{content:"󰱎"}.mdi-cart-arrow-up:before{content:"󰵧"}.mdi-cart-check:before{content:"󱗪"}.mdi-cart-heart:before{content:"󱣠"}.mdi-cart-minus:before{content:"󰵨"}.mdi-cart-off:before{content:"󰙫"}.mdi-cart-outline:before{content:"󰄑"}.mdi-cart-percent:before{content:"󱮮"}.mdi-cart-plus:before{content:"󰄒"}.mdi-cart-remove:before{content:"󰵩"}.mdi-cart-variant:before{content:"󱗫"}.mdi-case-sensitive-alt:before{content:"󰄓"}.mdi-cash:before{content:"󰄔"}.mdi-cash-100:before{content:"󰄕"}.mdi-cash-check:before{content:"󱓮"}.mdi-cash-clock:before{content:"󱪑"}.mdi-cash-fast:before{content:"󱡜"}.mdi-cash-lock:before{content:"󱓪"}.mdi-cash-lock-open:before{content:"󱓫"}.mdi-cash-marker:before{content:"󰶸"}.mdi-cash-minus:before{content:"󱉠"}.mdi-cash-multiple:before{content:"󰄖"}.mdi-cash-plus:before{content:"󱉡"}.mdi-cash-refund:before{content:"󰪜"}.mdi-cash-register:before{content:"󰳴"}.mdi-cash-remove:before{content:"󱉢"}.mdi-cash-sync:before{content:"󱪒"}.mdi-cassette:before{content:"󰧔"}.mdi-cast:before{content:"󰄘"}.mdi-cast-audio:before{content:"󱀞"}.mdi-cast-audio-variant:before{content:"󱝉"}.mdi-cast-connected:before{content:"󰄙"}.mdi-cast-education:before{content:"󰸝"}.mdi-cast-off:before{content:"󰞊"}.mdi-cast-variant:before{content:"󰀟"}.mdi-castle:before{content:"󰄚"}.mdi-cat:before{content:"󰄛"}.mdi-cctv:before{content:"󰞮"}.mdi-cctv-off:before{content:"󱡟"}.mdi-ceiling-fan:before{content:"󱞗"}.mdi-ceiling-fan-light:before{content:"󱞘"}.mdi-ceiling-light:before{content:"󰝩"}.mdi-ceiling-light-multiple:before{content:"󱣝"}.mdi-ceiling-light-multiple-outline:before{content:"󱣞"}.mdi-ceiling-light-outline:before{content:"󱟇"}.mdi-cellphone:before{content:"󰄜"}.mdi-cellphone-arrow-down:before{content:"󰧕"}.mdi-cellphone-arrow-down-variant:before{content:"󱧅"}.mdi-cellphone-basic:before{content:"󰄞"}.mdi-cellphone-charging:before{content:"󱎗"}.mdi-cellphone-check:before{content:"󱟽"}.mdi-cellphone-cog:before{content:"󰥑"}.mdi-cellphone-dock:before{content:"󰄟"}.mdi-cellphone-information:before{content:"󰽁"}.mdi-cellphone-key:before{content:"󰥎"}.mdi-cellphone-link:before{content:"󰄡"}.mdi-cellphone-link-off:before{content:"󰄢"}.mdi-cellphone-lock:before{content:"󰥏"}.mdi-cellphone-marker:before{content:"󱠺"}.mdi-cellphone-message:before{content:"󰣓"}.mdi-cellphone-message-off:before{content:"󱃒"}.mdi-cellphone-nfc:before{content:"󰺐"}.mdi-cellphone-nfc-off:before{content:"󱋘"}.mdi-cellphone-off:before{content:"󰥐"}.mdi-cellphone-play:before{content:"󱀟"}.mdi-cellphone-remove:before{content:"󰥍"}.mdi-cellphone-screenshot:before{content:"󰨵"}.mdi-cellphone-settings:before{content:"󰄣"}.mdi-cellphone-sound:before{content:"󰥒"}.mdi-cellphone-text:before{content:"󰣒"}.mdi-cellphone-wireless:before{content:"󰠕"}.mdi-centos:before{content:"󱄚"}.mdi-certificate:before{content:"󰄤"}.mdi-certificate-outline:before{content:"󱆈"}.mdi-chair-rolling:before{content:"󰽈"}.mdi-chair-school:before{content:"󰄥"}.mdi-chandelier:before{content:"󱞓"}.mdi-charity:before{content:"󰱏"}.mdi-chart-arc:before{content:"󰄦"}.mdi-chart-areaspline:before{content:"󰄧"}.mdi-chart-areaspline-variant:before{content:"󰺑"}.mdi-chart-bar:before{content:"󰄨"}.mdi-chart-bar-stacked:before{content:"󰝪"}.mdi-chart-bell-curve:before{content:"󰱐"}.mdi-chart-bell-curve-cumulative:before{content:"󰾧"}.mdi-chart-box:before{content:"󱕍"}.mdi-chart-box-outline:before{content:"󱕎"}.mdi-chart-box-plus-outline:before{content:"󱕏"}.mdi-chart-bubble:before{content:"󰗣"}.mdi-chart-donut:before{content:"󰞯"}.mdi-chart-donut-variant:before{content:"󰞰"}.mdi-chart-gantt:before{content:"󰙬"}.mdi-chart-histogram:before{content:"󰄩"}.mdi-chart-line:before{content:"󰄪"}.mdi-chart-line-stacked:before{content:"󰝫"}.mdi-chart-line-variant:before{content:"󰞱"}.mdi-chart-multiline:before{content:"󰣔"}.mdi-chart-multiple:before{content:"󱈓"}.mdi-chart-pie:before{content:"󰄫"}.mdi-chart-ppf:before{content:"󱎀"}.mdi-chart-sankey:before{content:"󱇟"}.mdi-chart-sankey-variant:before{content:"󱇠"}.mdi-chart-scatter-plot:before{content:"󰺒"}.mdi-chart-scatter-plot-hexbin:before{content:"󰙭"}.mdi-chart-timeline:before{content:"󰙮"}.mdi-chart-timeline-variant:before{content:"󰺓"}.mdi-chart-timeline-variant-shimmer:before{content:"󱖶"}.mdi-chart-tree:before{content:"󰺔"}.mdi-chart-waterfall:before{content:"󱤘"}.mdi-chat:before{content:"󰭹"}.mdi-chat-alert:before{content:"󰭺"}.mdi-chat-alert-outline:before{content:"󱋉"}.mdi-chat-minus:before{content:"󱐐"}.mdi-chat-minus-outline:before{content:"󱐓"}.mdi-chat-outline:before{content:"󰻞"}.mdi-chat-plus:before{content:"󱐏"}.mdi-chat-plus-outline:before{content:"󱐒"}.mdi-chat-processing:before{content:"󰭻"}.mdi-chat-processing-outline:before{content:"󱋊"}.mdi-chat-question:before{content:"󱜸"}.mdi-chat-question-outline:before{content:"󱜹"}.mdi-chat-remove:before{content:"󱐑"}.mdi-chat-remove-outline:before{content:"󱐔"}.mdi-chat-sleep:before{content:"󱋑"}.mdi-chat-sleep-outline:before{content:"󱋒"}.mdi-check:before{content:"󰄬"}.mdi-check-all:before{content:"󰄭"}.mdi-check-bold:before{content:"󰸞"}.mdi-check-circle:before{content:"󰗠"}.mdi-check-circle-outline:before{content:"󰗡"}.mdi-check-decagram:before{content:"󰞑"}.mdi-check-decagram-outline:before{content:"󱝀"}.mdi-check-network:before{content:"󰱓"}.mdi-check-network-outline:before{content:"󰱔"}.mdi-check-outline:before{content:"󰡕"}.mdi-check-underline:before{content:"󰸟"}.mdi-check-underline-circle:before{content:"󰸠"}.mdi-check-underline-circle-outline:before{content:"󰸡"}.mdi-checkbook:before{content:"󰪝"}.mdi-checkbox-blank:before{content:"󰄮"}.mdi-checkbox-blank-badge:before{content:"󱅶"}.mdi-checkbox-blank-badge-outline:before{content:"󰄗"}.mdi-checkbox-blank-circle:before{content:"󰄯"}.mdi-checkbox-blank-circle-outline:before{content:"󰄰"}.mdi-checkbox-blank-off:before{content:"󱋬"}.mdi-checkbox-blank-off-outline:before{content:"󱋭"}.mdi-checkbox-blank-outline:before{content:"󰄱"}.mdi-checkbox-intermediate:before{content:"󰡖"}.mdi-checkbox-intermediate-variant:before{content:"󱭔"}.mdi-checkbox-marked:before{content:"󰄲"}.mdi-checkbox-marked-circle:before{content:"󰄳"}.mdi-checkbox-marked-circle-outline:before{content:"󰄴"}.mdi-checkbox-marked-circle-plus-outline:before{content:"󱤧"}.mdi-checkbox-marked-outline:before{content:"󰄵"}.mdi-checkbox-multiple-blank:before{content:"󰄶"}.mdi-checkbox-multiple-blank-circle:before{content:"󰘻"}.mdi-checkbox-multiple-blank-circle-outline:before{content:"󰘼"}.mdi-checkbox-multiple-blank-outline:before{content:"󰄷"}.mdi-checkbox-multiple-marked:before{content:"󰄸"}.mdi-checkbox-multiple-marked-circle:before{content:"󰘽"}.mdi-checkbox-multiple-marked-circle-outline:before{content:"󰘾"}.mdi-checkbox-multiple-marked-outline:before{content:"󰄹"}.mdi-checkbox-multiple-outline:before{content:"󰱑"}.mdi-checkbox-outline:before{content:"󰱒"}.mdi-checkerboard:before{content:"󰄺"}.mdi-checkerboard-minus:before{content:"󱈂"}.mdi-checkerboard-plus:before{content:"󱈁"}.mdi-checkerboard-remove:before{content:"󱈃"}.mdi-cheese:before{content:"󱊹"}.mdi-cheese-off:before{content:"󱏮"}.mdi-chef-hat:before{content:"󰭼"}.mdi-chemical-weapon:before{content:"󰄻"}.mdi-chess-bishop:before{content:"󰡜"}.mdi-chess-king:before{content:"󰡗"}.mdi-chess-knight:before{content:"󰡘"}.mdi-chess-pawn:before{content:"󰡙"}.mdi-chess-queen:before{content:"󰡚"}.mdi-chess-rook:before{content:"󰡛"}.mdi-chevron-double-down:before{content:"󰄼"}.mdi-chevron-double-left:before{content:"󰄽"}.mdi-chevron-double-right:before{content:"󰄾"}.mdi-chevron-double-up:before{content:"󰄿"}.mdi-chevron-down:before{content:"󰅀"}.mdi-chevron-down-box:before{content:"󰧖"}.mdi-chevron-down-box-outline:before{content:"󰧗"}.mdi-chevron-down-circle:before{content:"󰬦"}.mdi-chevron-down-circle-outline:before{content:"󰬧"}.mdi-chevron-left:before{content:"󰅁"}.mdi-chevron-left-box:before{content:"󰧘"}.mdi-chevron-left-box-outline:before{content:"󰧙"}.mdi-chevron-left-circle:before{content:"󰬨"}.mdi-chevron-left-circle-outline:before{content:"󰬩"}.mdi-chevron-right:before{content:"󰅂"}.mdi-chevron-right-box:before{content:"󰧚"}.mdi-chevron-right-box-outline:before{content:"󰧛"}.mdi-chevron-right-circle:before{content:"󰬪"}.mdi-chevron-right-circle-outline:before{content:"󰬫"}.mdi-chevron-triple-down:before{content:"󰶹"}.mdi-chevron-triple-left:before{content:"󰶺"}.mdi-chevron-triple-right:before{content:"󰶻"}.mdi-chevron-triple-up:before{content:"󰶼"}.mdi-chevron-up:before{content:"󰅃"}.mdi-chevron-up-box:before{content:"󰧜"}.mdi-chevron-up-box-outline:before{content:"󰧝"}.mdi-chevron-up-circle:before{content:"󰬬"}.mdi-chevron-up-circle-outline:before{content:"󰬭"}.mdi-chili-alert:before{content:"󱟪"}.mdi-chili-alert-outline:before{content:"󱟫"}.mdi-chili-hot:before{content:"󰞲"}.mdi-chili-hot-outline:before{content:"󱟬"}.mdi-chili-medium:before{content:"󰞳"}.mdi-chili-medium-outline:before{content:"󱟭"}.mdi-chili-mild:before{content:"󰞴"}.mdi-chili-mild-outline:before{content:"󱟮"}.mdi-chili-off:before{content:"󱑧"}.mdi-chili-off-outline:before{content:"󱟯"}.mdi-chip:before{content:"󰘚"}.mdi-church:before{content:"󰅄"}.mdi-church-outline:before{content:"󱬂"}.mdi-cigar:before{content:"󱆉"}.mdi-cigar-off:before{content:"󱐛"}.mdi-circle:before{content:"󰝥"}.mdi-circle-box:before{content:"󱗜"}.mdi-circle-box-outline:before{content:"󱗝"}.mdi-circle-double:before{content:"󰺕"}.mdi-circle-edit-outline:before{content:"󰣕"}.mdi-circle-expand:before{content:"󰺖"}.mdi-circle-half:before{content:"󱎕"}.mdi-circle-half-full:before{content:"󱎖"}.mdi-circle-medium:before{content:"󰧞"}.mdi-circle-multiple:before{content:"󰬸"}.mdi-circle-multiple-outline:before{content:"󰚕"}.mdi-circle-off-outline:before{content:"󱃓"}.mdi-circle-opacity:before{content:"󱡓"}.mdi-circle-outline:before{content:"󰝦"}.mdi-circle-slice-1:before{content:"󰪞"}.mdi-circle-slice-2:before{content:"󰪟"}.mdi-circle-slice-3:before{content:"󰪠"}.mdi-circle-slice-4:before{content:"󰪡"}.mdi-circle-slice-5:before{content:"󰪢"}.mdi-circle-slice-6:before{content:"󰪣"}.mdi-circle-slice-7:before{content:"󰪤"}.mdi-circle-slice-8:before{content:"󰪥"}.mdi-circle-small:before{content:"󰧟"}.mdi-circular-saw:before{content:"󰸢"}.mdi-city:before{content:"󰅆"}.mdi-city-variant:before{content:"󰨶"}.mdi-city-variant-outline:before{content:"󰨷"}.mdi-clipboard:before{content:"󰅇"}.mdi-clipboard-account:before{content:"󰅈"}.mdi-clipboard-account-outline:before{content:"󰱕"}.mdi-clipboard-alert:before{content:"󰅉"}.mdi-clipboard-alert-outline:before{content:"󰳷"}.mdi-clipboard-arrow-down:before{content:"󰅊"}.mdi-clipboard-arrow-down-outline:before{content:"󰱖"}.mdi-clipboard-arrow-left:before{content:"󰅋"}.mdi-clipboard-arrow-left-outline:before{content:"󰳸"}.mdi-clipboard-arrow-right:before{content:"󰳹"}.mdi-clipboard-arrow-right-outline:before{content:"󰳺"}.mdi-clipboard-arrow-up:before{content:"󰱗"}.mdi-clipboard-arrow-up-outline:before{content:"󰱘"}.mdi-clipboard-check:before{content:"󰅎"}.mdi-clipboard-check-multiple:before{content:"󱉣"}.mdi-clipboard-check-multiple-outline:before{content:"󱉤"}.mdi-clipboard-check-outline:before{content:"󰢨"}.mdi-clipboard-clock:before{content:"󱛢"}.mdi-clipboard-clock-outline:before{content:"󱛣"}.mdi-clipboard-edit:before{content:"󱓥"}.mdi-clipboard-edit-outline:before{content:"󱓦"}.mdi-clipboard-file:before{content:"󱉥"}.mdi-clipboard-file-outline:before{content:"󱉦"}.mdi-clipboard-flow:before{content:"󰛈"}.mdi-clipboard-flow-outline:before{content:"󱄗"}.mdi-clipboard-list:before{content:"󱃔"}.mdi-clipboard-list-outline:before{content:"󱃕"}.mdi-clipboard-minus:before{content:"󱘘"}.mdi-clipboard-minus-outline:before{content:"󱘙"}.mdi-clipboard-multiple:before{content:"󱉧"}.mdi-clipboard-multiple-outline:before{content:"󱉨"}.mdi-clipboard-off:before{content:"󱘚"}.mdi-clipboard-off-outline:before{content:"󱘛"}.mdi-clipboard-outline:before{content:"󰅌"}.mdi-clipboard-play:before{content:"󰱙"}.mdi-clipboard-play-multiple:before{content:"󱉩"}.mdi-clipboard-play-multiple-outline:before{content:"󱉪"}.mdi-clipboard-play-outline:before{content:"󰱚"}.mdi-clipboard-plus:before{content:"󰝑"}.mdi-clipboard-plus-outline:before{content:"󱌟"}.mdi-clipboard-pulse:before{content:"󰡝"}.mdi-clipboard-pulse-outline:before{content:"󰡞"}.mdi-clipboard-remove:before{content:"󱘜"}.mdi-clipboard-remove-outline:before{content:"󱘝"}.mdi-clipboard-search:before{content:"󱘞"}.mdi-clipboard-search-outline:before{content:"󱘟"}.mdi-clipboard-text:before{content:"󰅍"}.mdi-clipboard-text-clock:before{content:"󱣹"}.mdi-clipboard-text-clock-outline:before{content:"󱣺"}.mdi-clipboard-text-multiple:before{content:"󱉫"}.mdi-clipboard-text-multiple-outline:before{content:"󱉬"}.mdi-clipboard-text-off:before{content:"󱘠"}.mdi-clipboard-text-off-outline:before{content:"󱘡"}.mdi-clipboard-text-outline:before{content:"󰨸"}.mdi-clipboard-text-play:before{content:"󰱛"}.mdi-clipboard-text-play-outline:before{content:"󰱜"}.mdi-clipboard-text-search:before{content:"󱘢"}.mdi-clipboard-text-search-outline:before{content:"󱘣"}.mdi-clippy:before{content:"󰅏"}.mdi-clock:before{content:"󰥔"}.mdi-clock-alert:before{content:"󰥕"}.mdi-clock-alert-outline:before{content:"󰗎"}.mdi-clock-check:before{content:"󰾨"}.mdi-clock-check-outline:before{content:"󰾩"}.mdi-clock-digital:before{content:"󰺗"}.mdi-clock-edit:before{content:"󱦺"}.mdi-clock-edit-outline:before{content:"󱦻"}.mdi-clock-end:before{content:"󰅑"}.mdi-clock-fast:before{content:"󰅒"}.mdi-clock-in:before{content:"󰅓"}.mdi-clock-minus:before{content:"󱡣"}.mdi-clock-minus-outline:before{content:"󱡤"}.mdi-clock-out:before{content:"󰅔"}.mdi-clock-outline:before{content:"󰅐"}.mdi-clock-plus:before{content:"󱡡"}.mdi-clock-plus-outline:before{content:"󱡢"}.mdi-clock-remove:before{content:"󱡥"}.mdi-clock-remove-outline:before{content:"󱡦"}.mdi-clock-start:before{content:"󰅕"}.mdi-clock-time-eight:before{content:"󱑆"}.mdi-clock-time-eight-outline:before{content:"󱑒"}.mdi-clock-time-eleven:before{content:"󱑉"}.mdi-clock-time-eleven-outline:before{content:"󱑕"}.mdi-clock-time-five:before{content:"󱑃"}.mdi-clock-time-five-outline:before{content:"󱑏"}.mdi-clock-time-four:before{content:"󱑂"}.mdi-clock-time-four-outline:before{content:"󱑎"}.mdi-clock-time-nine:before{content:"󱑇"}.mdi-clock-time-nine-outline:before{content:"󱑓"}.mdi-clock-time-one:before{content:"󱐿"}.mdi-clock-time-one-outline:before{content:"󱑋"}.mdi-clock-time-seven:before{content:"󱑅"}.mdi-clock-time-seven-outline:before{content:"󱑑"}.mdi-clock-time-six:before{content:"󱑄"}.mdi-clock-time-six-outline:before{content:"󱑐"}.mdi-clock-time-ten:before{content:"󱑈"}.mdi-clock-time-ten-outline:before{content:"󱑔"}.mdi-clock-time-three:before{content:"󱑁"}.mdi-clock-time-three-outline:before{content:"󱑍"}.mdi-clock-time-twelve:before{content:"󱑊"}.mdi-clock-time-twelve-outline:before{content:"󱑖"}.mdi-clock-time-two:before{content:"󱑀"}.mdi-clock-time-two-outline:before{content:"󱑌"}.mdi-close:before{content:"󰅖"}.mdi-close-box:before{content:"󰅗"}.mdi-close-box-multiple:before{content:"󰱝"}.mdi-close-box-multiple-outline:before{content:"󰱞"}.mdi-close-box-outline:before{content:"󰅘"}.mdi-close-circle:before{content:"󰅙"}.mdi-close-circle-multiple:before{content:"󰘪"}.mdi-close-circle-multiple-outline:before{content:"󰢃"}.mdi-close-circle-outline:before{content:"󰅚"}.mdi-close-network:before{content:"󰅛"}.mdi-close-network-outline:before{content:"󰱟"}.mdi-close-octagon:before{content:"󰅜"}.mdi-close-octagon-outline:before{content:"󰅝"}.mdi-close-outline:before{content:"󰛉"}.mdi-close-thick:before{content:"󱎘"}.mdi-closed-caption:before{content:"󰅞"}.mdi-closed-caption-outline:before{content:"󰶽"}.mdi-cloud:before{content:"󰅟"}.mdi-cloud-alert:before{content:"󰧠"}.mdi-cloud-braces:before{content:"󰞵"}.mdi-cloud-check:before{content:"󰅠"}.mdi-cloud-check-outline:before{content:"󱋌"}.mdi-cloud-circle:before{content:"󰅡"}.mdi-cloud-download:before{content:"󰅢"}.mdi-cloud-download-outline:before{content:"󰭽"}.mdi-cloud-lock:before{content:"󱇱"}.mdi-cloud-lock-outline:before{content:"󱇲"}.mdi-cloud-off-outline:before{content:"󰅤"}.mdi-cloud-outline:before{content:"󰅣"}.mdi-cloud-percent:before{content:"󱨵"}.mdi-cloud-percent-outline:before{content:"󱨶"}.mdi-cloud-print:before{content:"󰅥"}.mdi-cloud-print-outline:before{content:"󰅦"}.mdi-cloud-question:before{content:"󰨹"}.mdi-cloud-refresh:before{content:"󰔪"}.mdi-cloud-search:before{content:"󰥖"}.mdi-cloud-search-outline:before{content:"󰥗"}.mdi-cloud-sync:before{content:"󰘿"}.mdi-cloud-sync-outline:before{content:"󱋖"}.mdi-cloud-tags:before{content:"󰞶"}.mdi-cloud-upload:before{content:"󰅧"}.mdi-cloud-upload-outline:before{content:"󰭾"}.mdi-clouds:before{content:"󱮕"}.mdi-clover:before{content:"󰠖"}.mdi-coach-lamp:before{content:"󱀠"}.mdi-coach-lamp-variant:before{content:"󱨷"}.mdi-coat-rack:before{content:"󱂞"}.mdi-code-array:before{content:"󰅨"}.mdi-code-braces:before{content:"󰅩"}.mdi-code-braces-box:before{content:"󱃖"}.mdi-code-brackets:before{content:"󰅪"}.mdi-code-equal:before{content:"󰅫"}.mdi-code-greater-than:before{content:"󰅬"}.mdi-code-greater-than-or-equal:before{content:"󰅭"}.mdi-code-json:before{content:"󰘦"}.mdi-code-less-than:before{content:"󰅮"}.mdi-code-less-than-or-equal:before{content:"󰅯"}.mdi-code-not-equal:before{content:"󰅰"}.mdi-code-not-equal-variant:before{content:"󰅱"}.mdi-code-parentheses:before{content:"󰅲"}.mdi-code-parentheses-box:before{content:"󱃗"}.mdi-code-string:before{content:"󰅳"}.mdi-code-tags:before{content:"󰅴"}.mdi-code-tags-check:before{content:"󰚔"}.mdi-codepen:before{content:"󰅵"}.mdi-coffee:before{content:"󰅶"}.mdi-coffee-maker:before{content:"󱂟"}.mdi-coffee-maker-check:before{content:"󱤱"}.mdi-coffee-maker-check-outline:before{content:"󱤲"}.mdi-coffee-maker-outline:before{content:"󱠛"}.mdi-coffee-off:before{content:"󰾪"}.mdi-coffee-off-outline:before{content:"󰾫"}.mdi-coffee-outline:before{content:"󰛊"}.mdi-coffee-to-go:before{content:"󰅷"}.mdi-coffee-to-go-outline:before{content:"󱌎"}.mdi-coffin:before{content:"󰭿"}.mdi-cog:before{content:"󰒓"}.mdi-cog-box:before{content:"󰒔"}.mdi-cog-clockwise:before{content:"󱇝"}.mdi-cog-counterclockwise:before{content:"󱇞"}.mdi-cog-off:before{content:"󱏎"}.mdi-cog-off-outline:before{content:"󱏏"}.mdi-cog-outline:before{content:"󰢻"}.mdi-cog-pause:before{content:"󱤳"}.mdi-cog-pause-outline:before{content:"󱤴"}.mdi-cog-play:before{content:"󱤵"}.mdi-cog-play-outline:before{content:"󱤶"}.mdi-cog-refresh:before{content:"󱑞"}.mdi-cog-refresh-outline:before{content:"󱑟"}.mdi-cog-stop:before{content:"󱤷"}.mdi-cog-stop-outline:before{content:"󱤸"}.mdi-cog-sync:before{content:"󱑠"}.mdi-cog-sync-outline:before{content:"󱑡"}.mdi-cog-transfer:before{content:"󱁛"}.mdi-cog-transfer-outline:before{content:"󱁜"}.mdi-cogs:before{content:"󰣖"}.mdi-collage:before{content:"󰙀"}.mdi-collapse-all:before{content:"󰪦"}.mdi-collapse-all-outline:before{content:"󰪧"}.mdi-color-helper:before{content:"󰅹"}.mdi-comma:before{content:"󰸣"}.mdi-comma-box:before{content:"󰸫"}.mdi-comma-box-outline:before{content:"󰸤"}.mdi-comma-circle:before{content:"󰸥"}.mdi-comma-circle-outline:before{content:"󰸦"}.mdi-comment:before{content:"󰅺"}.mdi-comment-account:before{content:"󰅻"}.mdi-comment-account-outline:before{content:"󰅼"}.mdi-comment-alert:before{content:"󰅽"}.mdi-comment-alert-outline:before{content:"󰅾"}.mdi-comment-arrow-left:before{content:"󰧡"}.mdi-comment-arrow-left-outline:before{content:"󰧢"}.mdi-comment-arrow-right:before{content:"󰧣"}.mdi-comment-arrow-right-outline:before{content:"󰧤"}.mdi-comment-bookmark:before{content:"󱖮"}.mdi-comment-bookmark-outline:before{content:"󱖯"}.mdi-comment-check:before{content:"󰅿"}.mdi-comment-check-outline:before{content:"󰆀"}.mdi-comment-edit:before{content:"󱆿"}.mdi-comment-edit-outline:before{content:"󱋄"}.mdi-comment-eye:before{content:"󰨺"}.mdi-comment-eye-outline:before{content:"󰨻"}.mdi-comment-flash:before{content:"󱖰"}.mdi-comment-flash-outline:before{content:"󱖱"}.mdi-comment-minus:before{content:"󱗟"}.mdi-comment-minus-outline:before{content:"󱗠"}.mdi-comment-multiple:before{content:"󰡟"}.mdi-comment-multiple-outline:before{content:"󰆁"}.mdi-comment-off:before{content:"󱗡"}.mdi-comment-off-outline:before{content:"󱗢"}.mdi-comment-outline:before{content:"󰆂"}.mdi-comment-plus:before{content:"󰧥"}.mdi-comment-plus-outline:before{content:"󰆃"}.mdi-comment-processing:before{content:"󰆄"}.mdi-comment-processing-outline:before{content:"󰆅"}.mdi-comment-question:before{content:"󰠗"}.mdi-comment-question-outline:before{content:"󰆆"}.mdi-comment-quote:before{content:"󱀡"}.mdi-comment-quote-outline:before{content:"󱀢"}.mdi-comment-remove:before{content:"󰗞"}.mdi-comment-remove-outline:before{content:"󰆇"}.mdi-comment-search:before{content:"󰨼"}.mdi-comment-search-outline:before{content:"󰨽"}.mdi-comment-text:before{content:"󰆈"}.mdi-comment-text-multiple:before{content:"󰡠"}.mdi-comment-text-multiple-outline:before{content:"󰡡"}.mdi-comment-text-outline:before{content:"󰆉"}.mdi-compare:before{content:"󰆊"}.mdi-compare-horizontal:before{content:"󱒒"}.mdi-compare-remove:before{content:"󱢳"}.mdi-compare-vertical:before{content:"󱒓"}.mdi-compass:before{content:"󰆋"}.mdi-compass-off:before{content:"󰮀"}.mdi-compass-off-outline:before{content:"󰮁"}.mdi-compass-outline:before{content:"󰆌"}.mdi-compass-rose:before{content:"󱎂"}.mdi-compost:before{content:"󱨸"}.mdi-cone:before{content:"󱥌"}.mdi-cone-off:before{content:"󱥍"}.mdi-connection:before{content:"󱘖"}.mdi-console:before{content:"󰆍"}.mdi-console-line:before{content:"󰞷"}.mdi-console-network:before{content:"󰢩"}.mdi-console-network-outline:before{content:"󰱠"}.mdi-consolidate:before{content:"󱃘"}.mdi-contactless-payment:before{content:"󰵪"}.mdi-contactless-payment-circle:before{content:"󰌡"}.mdi-contactless-payment-circle-outline:before{content:"󰐈"}.mdi-contacts:before{content:"󰛋"}.mdi-contacts-outline:before{content:"󰖸"}.mdi-contain:before{content:"󰨾"}.mdi-contain-end:before{content:"󰨿"}.mdi-contain-start:before{content:"󰩀"}.mdi-content-copy:before{content:"󰆏"}.mdi-content-cut:before{content:"󰆐"}.mdi-content-duplicate:before{content:"󰆑"}.mdi-content-paste:before{content:"󰆒"}.mdi-content-save:before{content:"󰆓"}.mdi-content-save-alert:before{content:"󰽂"}.mdi-content-save-alert-outline:before{content:"󰽃"}.mdi-content-save-all:before{content:"󰆔"}.mdi-content-save-all-outline:before{content:"󰽄"}.mdi-content-save-check:before{content:"󱣪"}.mdi-content-save-check-outline:before{content:"󱣫"}.mdi-content-save-cog:before{content:"󱑛"}.mdi-content-save-cog-outline:before{content:"󱑜"}.mdi-content-save-edit:before{content:"󰳻"}.mdi-content-save-edit-outline:before{content:"󰳼"}.mdi-content-save-minus:before{content:"󱭃"}.mdi-content-save-minus-outline:before{content:"󱭄"}.mdi-content-save-move:before{content:"󰸧"}.mdi-content-save-move-outline:before{content:"󰸨"}.mdi-content-save-off:before{content:"󱙃"}.mdi-content-save-off-outline:before{content:"󱙄"}.mdi-content-save-outline:before{content:"󰠘"}.mdi-content-save-plus:before{content:"󱭁"}.mdi-content-save-plus-outline:before{content:"󱭂"}.mdi-content-save-settings:before{content:"󰘛"}.mdi-content-save-settings-outline:before{content:"󰬮"}.mdi-contrast:before{content:"󰆕"}.mdi-contrast-box:before{content:"󰆖"}.mdi-contrast-circle:before{content:"󰆗"}.mdi-controller:before{content:"󰊴"}.mdi-controller-classic:before{content:"󰮂"}.mdi-controller-classic-outline:before{content:"󰮃"}.mdi-controller-off:before{content:"󰊵"}.mdi-cookie:before{content:"󰆘"}.mdi-cookie-alert:before{content:"󱛐"}.mdi-cookie-alert-outline:before{content:"󱛑"}.mdi-cookie-check:before{content:"󱛒"}.mdi-cookie-check-outline:before{content:"󱛓"}.mdi-cookie-clock:before{content:"󱛤"}.mdi-cookie-clock-outline:before{content:"󱛥"}.mdi-cookie-cog:before{content:"󱛔"}.mdi-cookie-cog-outline:before{content:"󱛕"}.mdi-cookie-edit:before{content:"󱛦"}.mdi-cookie-edit-outline:before{content:"󱛧"}.mdi-cookie-lock:before{content:"󱛨"}.mdi-cookie-lock-outline:before{content:"󱛩"}.mdi-cookie-minus:before{content:"󱛚"}.mdi-cookie-minus-outline:before{content:"󱛛"}.mdi-cookie-off:before{content:"󱛪"}.mdi-cookie-off-outline:before{content:"󱛫"}.mdi-cookie-outline:before{content:"󱛞"}.mdi-cookie-plus:before{content:"󱛖"}.mdi-cookie-plus-outline:before{content:"󱛗"}.mdi-cookie-refresh:before{content:"󱛬"}.mdi-cookie-refresh-outline:before{content:"󱛭"}.mdi-cookie-remove:before{content:"󱛘"}.mdi-cookie-remove-outline:before{content:"󱛙"}.mdi-cookie-settings:before{content:"󱛜"}.mdi-cookie-settings-outline:before{content:"󱛝"}.mdi-coolant-temperature:before{content:"󰏈"}.mdi-copyleft:before{content:"󱤹"}.mdi-copyright:before{content:"󰗦"}.mdi-cordova:before{content:"󰥘"}.mdi-corn:before{content:"󰞸"}.mdi-corn-off:before{content:"󱏯"}.mdi-cosine-wave:before{content:"󱑹"}.mdi-counter:before{content:"󰆙"}.mdi-countertop:before{content:"󱠜"}.mdi-countertop-outline:before{content:"󱠝"}.mdi-cow:before{content:"󰆚"}.mdi-cow-off:before{content:"󱣼"}.mdi-cpu-32-bit:before{content:"󰻟"}.mdi-cpu-64-bit:before{content:"󰻠"}.mdi-cradle:before{content:"󱦋"}.mdi-cradle-outline:before{content:"󱦑"}.mdi-crane:before{content:"󰡢"}.mdi-creation:before{content:"󰙴"}.mdi-creative-commons:before{content:"󰵫"}.mdi-credit-card:before{content:"󰿯"}.mdi-credit-card-check:before{content:"󱏐"}.mdi-credit-card-check-outline:before{content:"󱏑"}.mdi-credit-card-chip:before{content:"󱤏"}.mdi-credit-card-chip-outline:before{content:"󱤐"}.mdi-credit-card-clock:before{content:"󰻡"}.mdi-credit-card-clock-outline:before{content:"󰻢"}.mdi-credit-card-edit:before{content:"󱟗"}.mdi-credit-card-edit-outline:before{content:"󱟘"}.mdi-credit-card-fast:before{content:"󱤑"}.mdi-credit-card-fast-outline:before{content:"󱤒"}.mdi-credit-card-lock:before{content:"󱣧"}.mdi-credit-card-lock-outline:before{content:"󱣨"}.mdi-credit-card-marker:before{content:"󰚨"}.mdi-credit-card-marker-outline:before{content:"󰶾"}.mdi-credit-card-minus:before{content:"󰾬"}.mdi-credit-card-minus-outline:before{content:"󰾭"}.mdi-credit-card-multiple:before{content:"󰿰"}.mdi-credit-card-multiple-outline:before{content:"󰆜"}.mdi-credit-card-off:before{content:"󰿱"}.mdi-credit-card-off-outline:before{content:"󰗤"}.mdi-credit-card-outline:before{content:"󰆛"}.mdi-credit-card-plus:before{content:"󰿲"}.mdi-credit-card-plus-outline:before{content:"󰙶"}.mdi-credit-card-refresh:before{content:"󱙅"}.mdi-credit-card-refresh-outline:before{content:"󱙆"}.mdi-credit-card-refund:before{content:"󰿳"}.mdi-credit-card-refund-outline:before{content:"󰪨"}.mdi-credit-card-remove:before{content:"󰾮"}.mdi-credit-card-remove-outline:before{content:"󰾯"}.mdi-credit-card-scan:before{content:"󰿴"}.mdi-credit-card-scan-outline:before{content:"󰆝"}.mdi-credit-card-search:before{content:"󱙇"}.mdi-credit-card-search-outline:before{content:"󱙈"}.mdi-credit-card-settings:before{content:"󰿵"}.mdi-credit-card-settings-outline:before{content:"󰣗"}.mdi-credit-card-sync:before{content:"󱙉"}.mdi-credit-card-sync-outline:before{content:"󱙊"}.mdi-credit-card-wireless:before{content:"󰠂"}.mdi-credit-card-wireless-off:before{content:"󰕺"}.mdi-credit-card-wireless-off-outline:before{content:"󰕻"}.mdi-credit-card-wireless-outline:before{content:"󰵬"}.mdi-cricket:before{content:"󰵭"}.mdi-crop:before{content:"󰆞"}.mdi-crop-free:before{content:"󰆟"}.mdi-crop-landscape:before{content:"󰆠"}.mdi-crop-portrait:before{content:"󰆡"}.mdi-crop-rotate:before{content:"󰚖"}.mdi-crop-square:before{content:"󰆢"}.mdi-cross:before{content:"󰥓"}.mdi-cross-bolnisi:before{content:"󰳭"}.mdi-cross-celtic:before{content:"󰳵"}.mdi-cross-outline:before{content:"󰳶"}.mdi-crosshairs:before{content:"󰆣"}.mdi-crosshairs-gps:before{content:"󰆤"}.mdi-crosshairs-off:before{content:"󰽅"}.mdi-crosshairs-question:before{content:"󱄶"}.mdi-crowd:before{content:"󱥵"}.mdi-crown:before{content:"󰆥"}.mdi-crown-circle:before{content:"󱟜"}.mdi-crown-circle-outline:before{content:"󱟝"}.mdi-crown-outline:before{content:"󱇐"}.mdi-cryengine:before{content:"󰥙"}.mdi-crystal-ball:before{content:"󰬯"}.mdi-cube:before{content:"󰆦"}.mdi-cube-off:before{content:"󱐜"}.mdi-cube-off-outline:before{content:"󱐝"}.mdi-cube-outline:before{content:"󰆧"}.mdi-cube-scan:before{content:"󰮄"}.mdi-cube-send:before{content:"󰆨"}.mdi-cube-unfolded:before{content:"󰆩"}.mdi-cup:before{content:"󰆪"}.mdi-cup-off:before{content:"󰗥"}.mdi-cup-off-outline:before{content:"󱍽"}.mdi-cup-outline:before{content:"󱌏"}.mdi-cup-water:before{content:"󰆫"}.mdi-cupboard:before{content:"󰽆"}.mdi-cupboard-outline:before{content:"󰽇"}.mdi-cupcake:before{content:"󰥚"}.mdi-curling:before{content:"󰡣"}.mdi-currency-bdt:before{content:"󰡤"}.mdi-currency-brl:before{content:"󰮅"}.mdi-currency-btc:before{content:"󰆬"}.mdi-currency-cny:before{content:"󰞺"}.mdi-currency-eth:before{content:"󰞻"}.mdi-currency-eur:before{content:"󰆭"}.mdi-currency-eur-off:before{content:"󱌕"}.mdi-currency-fra:before{content:"󱨹"}.mdi-currency-gbp:before{content:"󰆮"}.mdi-currency-ils:before{content:"󰱡"}.mdi-currency-inr:before{content:"󰆯"}.mdi-currency-jpy:before{content:"󰞼"}.mdi-currency-krw:before{content:"󰞽"}.mdi-currency-kzt:before{content:"󰡥"}.mdi-currency-mnt:before{content:"󱔒"}.mdi-currency-ngn:before{content:"󰆰"}.mdi-currency-php:before{content:"󰧦"}.mdi-currency-rial:before{content:"󰺜"}.mdi-currency-rub:before{content:"󰆱"}.mdi-currency-rupee:before{content:"󱥶"}.mdi-currency-sign:before{content:"󰞾"}.mdi-currency-try:before{content:"󰆲"}.mdi-currency-twd:before{content:"󰞿"}.mdi-currency-uah:before{content:"󱮛"}.mdi-currency-usd:before{content:"󰇁"}.mdi-currency-usd-off:before{content:"󰙺"}.mdi-current-ac:before{content:"󱒀"}.mdi-current-dc:before{content:"󰥜"}.mdi-cursor-default:before{content:"󰇀"}.mdi-cursor-default-click:before{content:"󰳽"}.mdi-cursor-default-click-outline:before{content:"󰳾"}.mdi-cursor-default-gesture:before{content:"󱄧"}.mdi-cursor-default-gesture-outline:before{content:"󱄨"}.mdi-cursor-default-outline:before{content:"󰆿"}.mdi-cursor-move:before{content:"󰆾"}.mdi-cursor-pointer:before{content:"󰆽"}.mdi-cursor-text:before{content:"󰗧"}.mdi-curtains:before{content:"󱡆"}.mdi-curtains-closed:before{content:"󱡇"}.mdi-cylinder:before{content:"󱥎"}.mdi-cylinder-off:before{content:"󱥏"}.mdi-dance-ballroom:before{content:"󱗻"}.mdi-dance-pole:before{content:"󱕸"}.mdi-data-matrix:before{content:"󱔼"}.mdi-data-matrix-edit:before{content:"󱔽"}.mdi-data-matrix-minus:before{content:"󱔾"}.mdi-data-matrix-plus:before{content:"󱔿"}.mdi-data-matrix-remove:before{content:"󱕀"}.mdi-data-matrix-scan:before{content:"󱕁"}.mdi-database:before{content:"󰆼"}.mdi-database-alert:before{content:"󱘺"}.mdi-database-alert-outline:before{content:"󱘤"}.mdi-database-arrow-down:before{content:"󱘻"}.mdi-database-arrow-down-outline:before{content:"󱘥"}.mdi-database-arrow-left:before{content:"󱘼"}.mdi-database-arrow-left-outline:before{content:"󱘦"}.mdi-database-arrow-right:before{content:"󱘽"}.mdi-database-arrow-right-outline:before{content:"󱘧"}.mdi-database-arrow-up:before{content:"󱘾"}.mdi-database-arrow-up-outline:before{content:"󱘨"}.mdi-database-check:before{content:"󰪩"}.mdi-database-check-outline:before{content:"󱘩"}.mdi-database-clock:before{content:"󱘿"}.mdi-database-clock-outline:before{content:"󱘪"}.mdi-database-cog:before{content:"󱙋"}.mdi-database-cog-outline:before{content:"󱙌"}.mdi-database-edit:before{content:"󰮆"}.mdi-database-edit-outline:before{content:"󱘫"}.mdi-database-export:before{content:"󰥞"}.mdi-database-export-outline:before{content:"󱘬"}.mdi-database-eye:before{content:"󱤟"}.mdi-database-eye-off:before{content:"󱤠"}.mdi-database-eye-off-outline:before{content:"󱤡"}.mdi-database-eye-outline:before{content:"󱤢"}.mdi-database-import:before{content:"󰥝"}.mdi-database-import-outline:before{content:"󱘭"}.mdi-database-lock:before{content:"󰪪"}.mdi-database-lock-outline:before{content:"󱘮"}.mdi-database-marker:before{content:"󱋶"}.mdi-database-marker-outline:before{content:"󱘯"}.mdi-database-minus:before{content:"󰆻"}.mdi-database-minus-outline:before{content:"󱘰"}.mdi-database-off:before{content:"󱙀"}.mdi-database-off-outline:before{content:"󱘱"}.mdi-database-outline:before{content:"󱘲"}.mdi-database-plus:before{content:"󰆺"}.mdi-database-plus-outline:before{content:"󱘳"}.mdi-database-refresh:before{content:"󰗂"}.mdi-database-refresh-outline:before{content:"󱘴"}.mdi-database-remove:before{content:"󰴀"}.mdi-database-remove-outline:before{content:"󱘵"}.mdi-database-search:before{content:"󰡦"}.mdi-database-search-outline:before{content:"󱘶"}.mdi-database-settings:before{content:"󰴁"}.mdi-database-settings-outline:before{content:"󱘷"}.mdi-database-sync:before{content:"󰳿"}.mdi-database-sync-outline:before{content:"󱘸"}.mdi-death-star:before{content:"󰣘"}.mdi-death-star-variant:before{content:"󰣙"}.mdi-deathly-hallows:before{content:"󰮇"}.mdi-debian:before{content:"󰣚"}.mdi-debug-step-into:before{content:"󰆹"}.mdi-debug-step-out:before{content:"󰆸"}.mdi-debug-step-over:before{content:"󰆷"}.mdi-decagram:before{content:"󰝬"}.mdi-decagram-outline:before{content:"󰝭"}.mdi-decimal:before{content:"󱂡"}.mdi-decimal-comma:before{content:"󱂢"}.mdi-decimal-comma-decrease:before{content:"󱂣"}.mdi-decimal-comma-increase:before{content:"󱂤"}.mdi-decimal-decrease:before{content:"󰆶"}.mdi-decimal-increase:before{content:"󰆵"}.mdi-delete:before{content:"󰆴"}.mdi-delete-alert:before{content:"󱂥"}.mdi-delete-alert-outline:before{content:"󱂦"}.mdi-delete-circle:before{content:"󰚃"}.mdi-delete-circle-outline:before{content:"󰮈"}.mdi-delete-clock:before{content:"󱕖"}.mdi-delete-clock-outline:before{content:"󱕗"}.mdi-delete-empty:before{content:"󰛌"}.mdi-delete-empty-outline:before{content:"󰺝"}.mdi-delete-forever:before{content:"󰗨"}.mdi-delete-forever-outline:before{content:"󰮉"}.mdi-delete-off:before{content:"󱂧"}.mdi-delete-off-outline:before{content:"󱂨"}.mdi-delete-outline:before{content:"󰧧"}.mdi-delete-restore:before{content:"󰠙"}.mdi-delete-sweep:before{content:"󰗩"}.mdi-delete-sweep-outline:before{content:"󰱢"}.mdi-delete-variant:before{content:"󰆳"}.mdi-delta:before{content:"󰇂"}.mdi-desk:before{content:"󱈹"}.mdi-desk-lamp:before{content:"󰥟"}.mdi-desk-lamp-off:before{content:"󱬟"}.mdi-desk-lamp-on:before{content:"󱬠"}.mdi-deskphone:before{content:"󰇃"}.mdi-desktop-classic:before{content:"󰟀"}.mdi-desktop-tower:before{content:"󰇅"}.mdi-desktop-tower-monitor:before{content:"󰪫"}.mdi-details:before{content:"󰇆"}.mdi-dev-to:before{content:"󰵮"}.mdi-developer-board:before{content:"󰚗"}.mdi-deviantart:before{content:"󰇇"}.mdi-devices:before{content:"󰾰"}.mdi-dharmachakra:before{content:"󰥋"}.mdi-diabetes:before{content:"󱄦"}.mdi-dialpad:before{content:"󰘜"}.mdi-diameter:before{content:"󰱣"}.mdi-diameter-outline:before{content:"󰱤"}.mdi-diameter-variant:before{content:"󰱥"}.mdi-diamond:before{content:"󰮊"}.mdi-diamond-outline:before{content:"󰮋"}.mdi-diamond-stone:before{content:"󰇈"}.mdi-dice-1:before{content:"󰇊"}.mdi-dice-1-outline:before{content:"󱅊"}.mdi-dice-2:before{content:"󰇋"}.mdi-dice-2-outline:before{content:"󱅋"}.mdi-dice-3:before{content:"󰇌"}.mdi-dice-3-outline:before{content:"󱅌"}.mdi-dice-4:before{content:"󰇍"}.mdi-dice-4-outline:before{content:"󱅍"}.mdi-dice-5:before{content:"󰇎"}.mdi-dice-5-outline:before{content:"󱅎"}.mdi-dice-6:before{content:"󰇏"}.mdi-dice-6-outline:before{content:"󱅏"}.mdi-dice-d10:before{content:"󱅓"}.mdi-dice-d10-outline:before{content:"󰝯"}.mdi-dice-d12:before{content:"󱅔"}.mdi-dice-d12-outline:before{content:"󰡧"}.mdi-dice-d20:before{content:"󱅕"}.mdi-dice-d20-outline:before{content:"󰗪"}.mdi-dice-d4:before{content:"󱅐"}.mdi-dice-d4-outline:before{content:"󰗫"}.mdi-dice-d6:before{content:"󱅑"}.mdi-dice-d6-outline:before{content:"󰗭"}.mdi-dice-d8:before{content:"󱅒"}.mdi-dice-d8-outline:before{content:"󰗬"}.mdi-dice-multiple:before{content:"󰝮"}.mdi-dice-multiple-outline:before{content:"󱅖"}.mdi-digital-ocean:before{content:"󱈷"}.mdi-dip-switch:before{content:"󰟁"}.mdi-directions:before{content:"󰇐"}.mdi-directions-fork:before{content:"󰙁"}.mdi-disc:before{content:"󰗮"}.mdi-disc-alert:before{content:"󰇑"}.mdi-disc-player:before{content:"󰥠"}.mdi-dishwasher:before{content:"󰪬"}.mdi-dishwasher-alert:before{content:"󱆸"}.mdi-dishwasher-off:before{content:"󱆹"}.mdi-disqus:before{content:"󰇒"}.mdi-distribute-horizontal-center:before{content:"󱇉"}.mdi-distribute-horizontal-left:before{content:"󱇈"}.mdi-distribute-horizontal-right:before{content:"󱇊"}.mdi-distribute-vertical-bottom:before{content:"󱇋"}.mdi-distribute-vertical-center:before{content:"󱇌"}.mdi-distribute-vertical-top:before{content:"󱇍"}.mdi-diversify:before{content:"󱡷"}.mdi-diving:before{content:"󱥷"}.mdi-diving-flippers:before{content:"󰶿"}.mdi-diving-helmet:before{content:"󰷀"}.mdi-diving-scuba:before{content:"󱭷"}.mdi-diving-scuba-flag:before{content:"󰷂"}.mdi-diving-scuba-mask:before{content:"󰷁"}.mdi-diving-scuba-tank:before{content:"󰷃"}.mdi-diving-scuba-tank-multiple:before{content:"󰷄"}.mdi-diving-snorkel:before{content:"󰷅"}.mdi-division:before{content:"󰇔"}.mdi-division-box:before{content:"󰇕"}.mdi-dlna:before{content:"󰩁"}.mdi-dna:before{content:"󰚄"}.mdi-dns:before{content:"󰇖"}.mdi-dns-outline:before{content:"󰮌"}.mdi-dock-bottom:before{content:"󱂩"}.mdi-dock-left:before{content:"󱂪"}.mdi-dock-right:before{content:"󱂫"}.mdi-dock-top:before{content:"󱔓"}.mdi-dock-window:before{content:"󱂬"}.mdi-docker:before{content:"󰡨"}.mdi-doctor:before{content:"󰩂"}.mdi-dog:before{content:"󰩃"}.mdi-dog-service:before{content:"󰪭"}.mdi-dog-side:before{content:"󰩄"}.mdi-dog-side-off:before{content:"󱛮"}.mdi-dolby:before{content:"󰚳"}.mdi-dolly:before{content:"󰺞"}.mdi-dolphin:before{content:"󱢴"}.mdi-domain:before{content:"󰇗"}.mdi-domain-off:before{content:"󰵯"}.mdi-domain-plus:before{content:"󱂭"}.mdi-domain-remove:before{content:"󱂮"}.mdi-dome-light:before{content:"󱐞"}.mdi-domino-mask:before{content:"󱀣"}.mdi-donkey:before{content:"󰟂"}.mdi-door:before{content:"󰠚"}.mdi-door-closed:before{content:"󰠛"}.mdi-door-closed-lock:before{content:"󱂯"}.mdi-door-open:before{content:"󰠜"}.mdi-door-sliding:before{content:"󱠞"}.mdi-door-sliding-lock:before{content:"󱠟"}.mdi-door-sliding-open:before{content:"󱠠"}.mdi-doorbell:before{content:"󱋦"}.mdi-doorbell-video:before{content:"󰡩"}.mdi-dot-net:before{content:"󰪮"}.mdi-dots-circle:before{content:"󱥸"}.mdi-dots-grid:before{content:"󱗼"}.mdi-dots-hexagon:before{content:"󱗿"}.mdi-dots-horizontal:before{content:"󰇘"}.mdi-dots-horizontal-circle:before{content:"󰟃"}.mdi-dots-horizontal-circle-outline:before{content:"󰮍"}.mdi-dots-square:before{content:"󱗽"}.mdi-dots-triangle:before{content:"󱗾"}.mdi-dots-vertical:before{content:"󰇙"}.mdi-dots-vertical-circle:before{content:"󰟄"}.mdi-dots-vertical-circle-outline:before{content:"󰮎"}.mdi-download:before{content:"󰇚"}.mdi-download-box:before{content:"󱑢"}.mdi-download-box-outline:before{content:"󱑣"}.mdi-download-circle:before{content:"󱑤"}.mdi-download-circle-outline:before{content:"󱑥"}.mdi-download-lock:before{content:"󱌠"}.mdi-download-lock-outline:before{content:"󱌡"}.mdi-download-multiple:before{content:"󰧩"}.mdi-download-network:before{content:"󰛴"}.mdi-download-network-outline:before{content:"󰱦"}.mdi-download-off:before{content:"󱂰"}.mdi-download-off-outline:before{content:"󱂱"}.mdi-download-outline:before{content:"󰮏"}.mdi-drag:before{content:"󰇛"}.mdi-drag-horizontal:before{content:"󰇜"}.mdi-drag-horizontal-variant:before{content:"󱋰"}.mdi-drag-variant:before{content:"󰮐"}.mdi-drag-vertical:before{content:"󰇝"}.mdi-drag-vertical-variant:before{content:"󱋱"}.mdi-drama-masks:before{content:"󰴂"}.mdi-draw:before{content:"󰽉"}.mdi-draw-pen:before{content:"󱦹"}.mdi-drawing:before{content:"󰇞"}.mdi-drawing-box:before{content:"󰇟"}.mdi-dresser:before{content:"󰽊"}.mdi-dresser-outline:before{content:"󰽋"}.mdi-drone:before{content:"󰇢"}.mdi-dropbox:before{content:"󰇣"}.mdi-drupal:before{content:"󰇤"}.mdi-duck:before{content:"󰇥"}.mdi-dumbbell:before{content:"󰇦"}.mdi-dump-truck:before{content:"󰱧"}.mdi-ear-hearing:before{content:"󰟅"}.mdi-ear-hearing-loop:before{content:"󱫮"}.mdi-ear-hearing-off:before{content:"󰩅"}.mdi-earbuds:before{content:"󱡏"}.mdi-earbuds-off:before{content:"󱡐"}.mdi-earbuds-off-outline:before{content:"󱡑"}.mdi-earbuds-outline:before{content:"󱡒"}.mdi-earth:before{content:"󰇧"}.mdi-earth-arrow-right:before{content:"󱌑"}.mdi-earth-box:before{content:"󰛍"}.mdi-earth-box-minus:before{content:"󱐇"}.mdi-earth-box-off:before{content:"󰛎"}.mdi-earth-box-plus:before{content:"󱐆"}.mdi-earth-box-remove:before{content:"󱐈"}.mdi-earth-minus:before{content:"󱐄"}.mdi-earth-off:before{content:"󰇨"}.mdi-earth-plus:before{content:"󱐃"}.mdi-earth-remove:before{content:"󱐅"}.mdi-egg:before{content:"󰪯"}.mdi-egg-easter:before{content:"󰪰"}.mdi-egg-fried:before{content:"󱡊"}.mdi-egg-off:before{content:"󱏰"}.mdi-egg-off-outline:before{content:"󱏱"}.mdi-egg-outline:before{content:"󱏲"}.mdi-eiffel-tower:before{content:"󱕫"}.mdi-eight-track:before{content:"󰧪"}.mdi-eject:before{content:"󰇪"}.mdi-eject-circle:before{content:"󱬣"}.mdi-eject-circle-outline:before{content:"󱬤"}.mdi-eject-outline:before{content:"󰮑"}.mdi-electric-switch:before{content:"󰺟"}.mdi-electric-switch-closed:before{content:"󱃙"}.mdi-electron-framework:before{content:"󱀤"}.mdi-elephant:before{content:"󰟆"}.mdi-elevation-decline:before{content:"󰇫"}.mdi-elevation-rise:before{content:"󰇬"}.mdi-elevator:before{content:"󰇭"}.mdi-elevator-down:before{content:"󱋂"}.mdi-elevator-passenger:before{content:"󱎁"}.mdi-elevator-passenger-off:before{content:"󱥹"}.mdi-elevator-passenger-off-outline:before{content:"󱥺"}.mdi-elevator-passenger-outline:before{content:"󱥻"}.mdi-elevator-up:before{content:"󱋁"}.mdi-ellipse:before{content:"󰺠"}.mdi-ellipse-outline:before{content:"󰺡"}.mdi-email:before{content:"󰇮"}.mdi-email-alert:before{content:"󰛏"}.mdi-email-alert-outline:before{content:"󰵂"}.mdi-email-arrow-left:before{content:"󱃚"}.mdi-email-arrow-left-outline:before{content:"󱃛"}.mdi-email-arrow-right:before{content:"󱃜"}.mdi-email-arrow-right-outline:before{content:"󱃝"}.mdi-email-box:before{content:"󰴃"}.mdi-email-check:before{content:"󰪱"}.mdi-email-check-outline:before{content:"󰪲"}.mdi-email-edit:before{content:"󰻣"}.mdi-email-edit-outline:before{content:"󰻤"}.mdi-email-fast:before{content:"󱡯"}.mdi-email-fast-outline:before{content:"󱡰"}.mdi-email-lock:before{content:"󰇱"}.mdi-email-lock-outline:before{content:"󱭡"}.mdi-email-mark-as-unread:before{content:"󰮒"}.mdi-email-minus:before{content:"󰻥"}.mdi-email-minus-outline:before{content:"󰻦"}.mdi-email-multiple:before{content:"󰻧"}.mdi-email-multiple-outline:before{content:"󰻨"}.mdi-email-newsletter:before{content:"󰾱"}.mdi-email-off:before{content:"󱏣"}.mdi-email-off-outline:before{content:"󱏤"}.mdi-email-open:before{content:"󰇯"}.mdi-email-open-multiple:before{content:"󰻩"}.mdi-email-open-multiple-outline:before{content:"󰻪"}.mdi-email-open-outline:before{content:"󰗯"}.mdi-email-outline:before{content:"󰇰"}.mdi-email-plus:before{content:"󰧫"}.mdi-email-plus-outline:before{content:"󰧬"}.mdi-email-remove:before{content:"󱙡"}.mdi-email-remove-outline:before{content:"󱙢"}.mdi-email-seal:before{content:"󱥛"}.mdi-email-seal-outline:before{content:"󱥜"}.mdi-email-search:before{content:"󰥡"}.mdi-email-search-outline:before{content:"󰥢"}.mdi-email-sync:before{content:"󱋇"}.mdi-email-sync-outline:before{content:"󱋈"}.mdi-email-variant:before{content:"󰗰"}.mdi-ember:before{content:"󰬰"}.mdi-emby:before{content:"󰚴"}.mdi-emoticon:before{content:"󰱨"}.mdi-emoticon-angry:before{content:"󰱩"}.mdi-emoticon-angry-outline:before{content:"󰱪"}.mdi-emoticon-confused:before{content:"󱃞"}.mdi-emoticon-confused-outline:before{content:"󱃟"}.mdi-emoticon-cool:before{content:"󰱫"}.mdi-emoticon-cool-outline:before{content:"󰇳"}.mdi-emoticon-cry:before{content:"󰱬"}.mdi-emoticon-cry-outline:before{content:"󰱭"}.mdi-emoticon-dead:before{content:"󰱮"}.mdi-emoticon-dead-outline:before{content:"󰚛"}.mdi-emoticon-devil:before{content:"󰱯"}.mdi-emoticon-devil-outline:before{content:"󰇴"}.mdi-emoticon-excited:before{content:"󰱰"}.mdi-emoticon-excited-outline:before{content:"󰚜"}.mdi-emoticon-frown:before{content:"󰽌"}.mdi-emoticon-frown-outline:before{content:"󰽍"}.mdi-emoticon-happy:before{content:"󰱱"}.mdi-emoticon-happy-outline:before{content:"󰇵"}.mdi-emoticon-kiss:before{content:"󰱲"}.mdi-emoticon-kiss-outline:before{content:"󰱳"}.mdi-emoticon-lol:before{content:"󱈔"}.mdi-emoticon-lol-outline:before{content:"󱈕"}.mdi-emoticon-neutral:before{content:"󰱴"}.mdi-emoticon-neutral-outline:before{content:"󰇶"}.mdi-emoticon-outline:before{content:"󰇲"}.mdi-emoticon-poop:before{content:"󰇷"}.mdi-emoticon-poop-outline:before{content:"󰱵"}.mdi-emoticon-sad:before{content:"󰱶"}.mdi-emoticon-sad-outline:before{content:"󰇸"}.mdi-emoticon-sick:before{content:"󱕼"}.mdi-emoticon-sick-outline:before{content:"󱕽"}.mdi-emoticon-tongue:before{content:"󰇹"}.mdi-emoticon-tongue-outline:before{content:"󰱷"}.mdi-emoticon-wink:before{content:"󰱸"}.mdi-emoticon-wink-outline:before{content:"󰱹"}.mdi-engine:before{content:"󰇺"}.mdi-engine-off:before{content:"󰩆"}.mdi-engine-off-outline:before{content:"󰩇"}.mdi-engine-outline:before{content:"󰇻"}.mdi-epsilon:before{content:"󱃠"}.mdi-equal:before{content:"󰇼"}.mdi-equal-box:before{content:"󰇽"}.mdi-equalizer:before{content:"󰺢"}.mdi-equalizer-outline:before{content:"󰺣"}.mdi-eraser:before{content:"󰇾"}.mdi-eraser-variant:before{content:"󰙂"}.mdi-escalator:before{content:"󰇿"}.mdi-escalator-box:before{content:"󱎙"}.mdi-escalator-down:before{content:"󱋀"}.mdi-escalator-up:before{content:"󱊿"}.mdi-eslint:before{content:"󰱺"}.mdi-et:before{content:"󰪳"}.mdi-ethereum:before{content:"󰡪"}.mdi-ethernet:before{content:"󰈀"}.mdi-ethernet-cable:before{content:"󰈁"}.mdi-ethernet-cable-off:before{content:"󰈂"}.mdi-ev-plug-ccs1:before{content:"󱔙"}.mdi-ev-plug-ccs2:before{content:"󱔚"}.mdi-ev-plug-chademo:before{content:"󱔛"}.mdi-ev-plug-tesla:before{content:"󱔜"}.mdi-ev-plug-type1:before{content:"󱔝"}.mdi-ev-plug-type2:before{content:"󱔞"}.mdi-ev-station:before{content:"󰗱"}.mdi-evernote:before{content:"󰈄"}.mdi-excavator:before{content:"󱀥"}.mdi-exclamation:before{content:"󰈅"}.mdi-exclamation-thick:before{content:"󱈸"}.mdi-exit-run:before{content:"󰩈"}.mdi-exit-to-app:before{content:"󰈆"}.mdi-expand-all:before{content:"󰪴"}.mdi-expand-all-outline:before{content:"󰪵"}.mdi-expansion-card:before{content:"󰢮"}.mdi-expansion-card-variant:before{content:"󰾲"}.mdi-exponent:before{content:"󰥣"}.mdi-exponent-box:before{content:"󰥤"}.mdi-export:before{content:"󰈇"}.mdi-export-variant:before{content:"󰮓"}.mdi-eye:before{content:"󰈈"}.mdi-eye-arrow-left:before{content:"󱣽"}.mdi-eye-arrow-left-outline:before{content:"󱣾"}.mdi-eye-arrow-right:before{content:"󱣿"}.mdi-eye-arrow-right-outline:before{content:"󱤀"}.mdi-eye-check:before{content:"󰴄"}.mdi-eye-check-outline:before{content:"󰴅"}.mdi-eye-circle:before{content:"󰮔"}.mdi-eye-circle-outline:before{content:"󰮕"}.mdi-eye-minus:before{content:"󱀦"}.mdi-eye-minus-outline:before{content:"󱀧"}.mdi-eye-off:before{content:"󰈉"}.mdi-eye-off-outline:before{content:"󰛑"}.mdi-eye-outline:before{content:"󰛐"}.mdi-eye-plus:before{content:"󰡫"}.mdi-eye-plus-outline:before{content:"󰡬"}.mdi-eye-refresh:before{content:"󱥼"}.mdi-eye-refresh-outline:before{content:"󱥽"}.mdi-eye-remove:before{content:"󱗣"}.mdi-eye-remove-outline:before{content:"󱗤"}.mdi-eye-settings:before{content:"󰡭"}.mdi-eye-settings-outline:before{content:"󰡮"}.mdi-eyedropper:before{content:"󰈊"}.mdi-eyedropper-minus:before{content:"󱏝"}.mdi-eyedropper-off:before{content:"󱏟"}.mdi-eyedropper-plus:before{content:"󱏜"}.mdi-eyedropper-remove:before{content:"󱏞"}.mdi-eyedropper-variant:before{content:"󰈋"}.mdi-face-agent:before{content:"󰵰"}.mdi-face-man:before{content:"󰙃"}.mdi-face-man-outline:before{content:"󰮖"}.mdi-face-man-profile:before{content:"󰙄"}.mdi-face-man-shimmer:before{content:"󱗌"}.mdi-face-man-shimmer-outline:before{content:"󱗍"}.mdi-face-mask:before{content:"󱖆"}.mdi-face-mask-outline:before{content:"󱖇"}.mdi-face-recognition:before{content:"󰱻"}.mdi-face-woman:before{content:"󱁷"}.mdi-face-woman-outline:before{content:"󱁸"}.mdi-face-woman-profile:before{content:"󱁶"}.mdi-face-woman-shimmer:before{content:"󱗎"}.mdi-face-woman-shimmer-outline:before{content:"󱗏"}.mdi-facebook:before{content:"󰈌"}.mdi-facebook-gaming:before{content:"󰟝"}.mdi-facebook-messenger:before{content:"󰈎"}.mdi-facebook-workplace:before{content:"󰬱"}.mdi-factory:before{content:"󰈏"}.mdi-family-tree:before{content:"󱘎"}.mdi-fan:before{content:"󰈐"}.mdi-fan-alert:before{content:"󱑬"}.mdi-fan-auto:before{content:"󱜝"}.mdi-fan-chevron-down:before{content:"󱑭"}.mdi-fan-chevron-up:before{content:"󱑮"}.mdi-fan-clock:before{content:"󱨺"}.mdi-fan-minus:before{content:"󱑰"}.mdi-fan-off:before{content:"󰠝"}.mdi-fan-plus:before{content:"󱑯"}.mdi-fan-remove:before{content:"󱑱"}.mdi-fan-speed-1:before{content:"󱑲"}.mdi-fan-speed-2:before{content:"󱑳"}.mdi-fan-speed-3:before{content:"󱑴"}.mdi-fast-forward:before{content:"󰈑"}.mdi-fast-forward-10:before{content:"󰵱"}.mdi-fast-forward-15:before{content:"󱤺"}.mdi-fast-forward-30:before{content:"󰴆"}.mdi-fast-forward-45:before{content:"󱬒"}.mdi-fast-forward-5:before{content:"󱇸"}.mdi-fast-forward-60:before{content:"󱘋"}.mdi-fast-forward-outline:before{content:"󰛒"}.mdi-faucet:before{content:"󱬩"}.mdi-faucet-variant:before{content:"󱬪"}.mdi-fax:before{content:"󰈒"}.mdi-feather:before{content:"󰛓"}.mdi-feature-search:before{content:"󰩉"}.mdi-feature-search-outline:before{content:"󰩊"}.mdi-fedora:before{content:"󰣛"}.mdi-fence:before{content:"󱞚"}.mdi-fence-electric:before{content:"󱟶"}.mdi-fencing:before{content:"󱓁"}.mdi-ferris-wheel:before{content:"󰺤"}.mdi-ferry:before{content:"󰈓"}.mdi-file:before{content:"󰈔"}.mdi-file-account:before{content:"󰜻"}.mdi-file-account-outline:before{content:"󱀨"}.mdi-file-alert:before{content:"󰩋"}.mdi-file-alert-outline:before{content:"󰩌"}.mdi-file-arrow-left-right:before{content:"󱪓"}.mdi-file-arrow-left-right-outline:before{content:"󱪔"}.mdi-file-arrow-up-down:before{content:"󱪕"}.mdi-file-arrow-up-down-outline:before{content:"󱪖"}.mdi-file-cabinet:before{content:"󰪶"}.mdi-file-cad:before{content:"󰻫"}.mdi-file-cad-box:before{content:"󰻬"}.mdi-file-cancel:before{content:"󰷆"}.mdi-file-cancel-outline:before{content:"󰷇"}.mdi-file-certificate:before{content:"󱆆"}.mdi-file-certificate-outline:before{content:"󱆇"}.mdi-file-chart:before{content:"󰈕"}.mdi-file-chart-check:before{content:"󱧆"}.mdi-file-chart-check-outline:before{content:"󱧇"}.mdi-file-chart-outline:before{content:"󱀩"}.mdi-file-check:before{content:"󰈖"}.mdi-file-check-outline:before{content:"󰸩"}.mdi-file-clock:before{content:"󱋡"}.mdi-file-clock-outline:before{content:"󱋢"}.mdi-file-cloud:before{content:"󰈗"}.mdi-file-cloud-outline:before{content:"󱀪"}.mdi-file-code:before{content:"󰈮"}.mdi-file-code-outline:before{content:"󱀫"}.mdi-file-cog:before{content:"󱁻"}.mdi-file-cog-outline:before{content:"󱁼"}.mdi-file-compare:before{content:"󰢪"}.mdi-file-delimited:before{content:"󰈘"}.mdi-file-delimited-outline:before{content:"󰺥"}.mdi-file-document:before{content:"󰈙"}.mdi-file-document-alert:before{content:"󱪗"}.mdi-file-document-alert-outline:before{content:"󱪘"}.mdi-file-document-check:before{content:"󱪙"}.mdi-file-document-check-outline:before{content:"󱪚"}.mdi-file-document-edit:before{content:"󰷈"}.mdi-file-document-edit-outline:before{content:"󰷉"}.mdi-file-document-minus:before{content:"󱪛"}.mdi-file-document-minus-outline:before{content:"󱪜"}.mdi-file-document-multiple:before{content:"󱔗"}.mdi-file-document-multiple-outline:before{content:"󱔘"}.mdi-file-document-outline:before{content:"󰧮"}.mdi-file-document-plus:before{content:"󱪝"}.mdi-file-document-plus-outline:before{content:"󱪞"}.mdi-file-document-remove:before{content:"󱪟"}.mdi-file-document-remove-outline:before{content:"󱪠"}.mdi-file-download:before{content:"󰥥"}.mdi-file-download-outline:before{content:"󰥦"}.mdi-file-edit:before{content:"󱇧"}.mdi-file-edit-outline:before{content:"󱇨"}.mdi-file-excel:before{content:"󰈛"}.mdi-file-excel-box:before{content:"󰈜"}.mdi-file-excel-box-outline:before{content:"󱀬"}.mdi-file-excel-outline:before{content:"󱀭"}.mdi-file-export:before{content:"󰈝"}.mdi-file-export-outline:before{content:"󱀮"}.mdi-file-eye:before{content:"󰷊"}.mdi-file-eye-outline:before{content:"󰷋"}.mdi-file-find:before{content:"󰈞"}.mdi-file-find-outline:before{content:"󰮗"}.mdi-file-gif-box:before{content:"󰵸"}.mdi-file-hidden:before{content:"󰘓"}.mdi-file-image:before{content:"󰈟"}.mdi-file-image-marker:before{content:"󱝲"}.mdi-file-image-marker-outline:before{content:"󱝳"}.mdi-file-image-minus:before{content:"󱤻"}.mdi-file-image-minus-outline:before{content:"󱤼"}.mdi-file-image-outline:before{content:"󰺰"}.mdi-file-image-plus:before{content:"󱤽"}.mdi-file-image-plus-outline:before{content:"󱤾"}.mdi-file-image-remove:before{content:"󱤿"}.mdi-file-image-remove-outline:before{content:"󱥀"}.mdi-file-import:before{content:"󰈠"}.mdi-file-import-outline:before{content:"󱀯"}.mdi-file-jpg-box:before{content:"󰈥"}.mdi-file-key:before{content:"󱆄"}.mdi-file-key-outline:before{content:"󱆅"}.mdi-file-link:before{content:"󱅷"}.mdi-file-link-outline:before{content:"󱅸"}.mdi-file-lock:before{content:"󰈡"}.mdi-file-lock-open:before{content:"󱧈"}.mdi-file-lock-open-outline:before{content:"󱧉"}.mdi-file-lock-outline:before{content:"󱀰"}.mdi-file-marker:before{content:"󱝴"}.mdi-file-marker-outline:before{content:"󱝵"}.mdi-file-minus:before{content:"󱪡"}.mdi-file-minus-outline:before{content:"󱪢"}.mdi-file-move:before{content:"󰪹"}.mdi-file-move-outline:before{content:"󱀱"}.mdi-file-multiple:before{content:"󰈢"}.mdi-file-multiple-outline:before{content:"󱀲"}.mdi-file-music:before{content:"󰈣"}.mdi-file-music-outline:before{content:"󰸪"}.mdi-file-outline:before{content:"󰈤"}.mdi-file-pdf-box:before{content:"󰈦"}.mdi-file-percent:before{content:"󰠞"}.mdi-file-percent-outline:before{content:"󱀳"}.mdi-file-phone:before{content:"󱅹"}.mdi-file-phone-outline:before{content:"󱅺"}.mdi-file-plus:before{content:"󰝒"}.mdi-file-plus-outline:before{content:"󰻭"}.mdi-file-png-box:before{content:"󰸭"}.mdi-file-powerpoint:before{content:"󰈧"}.mdi-file-powerpoint-box:before{content:"󰈨"}.mdi-file-powerpoint-box-outline:before{content:"󱀴"}.mdi-file-powerpoint-outline:before{content:"󱀵"}.mdi-file-presentation-box:before{content:"󰈩"}.mdi-file-question:before{content:"󰡯"}.mdi-file-question-outline:before{content:"󱀶"}.mdi-file-refresh:before{content:"󰤘"}.mdi-file-refresh-outline:before{content:"󰕁"}.mdi-file-remove:before{content:"󰮘"}.mdi-file-remove-outline:before{content:"󱀷"}.mdi-file-replace:before{content:"󰬲"}.mdi-file-replace-outline:before{content:"󰬳"}.mdi-file-restore:before{content:"󰙰"}.mdi-file-restore-outline:before{content:"󱀸"}.mdi-file-rotate-left:before{content:"󱨻"}.mdi-file-rotate-left-outline:before{content:"󱨼"}.mdi-file-rotate-right:before{content:"󱨽"}.mdi-file-rotate-right-outline:before{content:"󱨾"}.mdi-file-search:before{content:"󰱼"}.mdi-file-search-outline:before{content:"󰱽"}.mdi-file-send:before{content:"󰈪"}.mdi-file-send-outline:before{content:"󱀹"}.mdi-file-settings:before{content:"󱁹"}.mdi-file-settings-outline:before{content:"󱁺"}.mdi-file-sign:before{content:"󱧃"}.mdi-file-star:before{content:"󱀺"}.mdi-file-star-outline:before{content:"󱀻"}.mdi-file-swap:before{content:"󰾴"}.mdi-file-swap-outline:before{content:"󰾵"}.mdi-file-sync:before{content:"󱈖"}.mdi-file-sync-outline:before{content:"󱈗"}.mdi-file-table:before{content:"󰱾"}.mdi-file-table-box:before{content:"󱃡"}.mdi-file-table-box-multiple:before{content:"󱃢"}.mdi-file-table-box-multiple-outline:before{content:"󱃣"}.mdi-file-table-box-outline:before{content:"󱃤"}.mdi-file-table-outline:before{content:"󰱿"}.mdi-file-tree:before{content:"󰙅"}.mdi-file-tree-outline:before{content:"󱏒"}.mdi-file-undo:before{content:"󰣜"}.mdi-file-undo-outline:before{content:"󱀼"}.mdi-file-upload:before{content:"󰩍"}.mdi-file-upload-outline:before{content:"󰩎"}.mdi-file-video:before{content:"󰈫"}.mdi-file-video-outline:before{content:"󰸬"}.mdi-file-word:before{content:"󰈬"}.mdi-file-word-box:before{content:"󰈭"}.mdi-file-word-box-outline:before{content:"󱀽"}.mdi-file-word-outline:before{content:"󱀾"}.mdi-file-xml-box:before{content:"󱭋"}.mdi-film:before{content:"󰈯"}.mdi-filmstrip:before{content:"󰈰"}.mdi-filmstrip-box:before{content:"󰌲"}.mdi-filmstrip-box-multiple:before{content:"󰴘"}.mdi-filmstrip-off:before{content:"󰈱"}.mdi-filter:before{content:"󰈲"}.mdi-filter-check:before{content:"󱣬"}.mdi-filter-check-outline:before{content:"󱣭"}.mdi-filter-cog:before{content:"󱪣"}.mdi-filter-cog-outline:before{content:"󱪤"}.mdi-filter-menu:before{content:"󱃥"}.mdi-filter-menu-outline:before{content:"󱃦"}.mdi-filter-minus:before{content:"󰻮"}.mdi-filter-minus-outline:before{content:"󰻯"}.mdi-filter-multiple:before{content:"󱨿"}.mdi-filter-multiple-outline:before{content:"󱩀"}.mdi-filter-off:before{content:"󱓯"}.mdi-filter-off-outline:before{content:"󱓰"}.mdi-filter-outline:before{content:"󰈳"}.mdi-filter-plus:before{content:"󰻰"}.mdi-filter-plus-outline:before{content:"󰻱"}.mdi-filter-remove:before{content:"󰈴"}.mdi-filter-remove-outline:before{content:"󰈵"}.mdi-filter-settings:before{content:"󱪥"}.mdi-filter-settings-outline:before{content:"󱪦"}.mdi-filter-variant:before{content:"󰈶"}.mdi-filter-variant-minus:before{content:"󱄒"}.mdi-filter-variant-plus:before{content:"󱄓"}.mdi-filter-variant-remove:before{content:"󱀿"}.mdi-finance:before{content:"󰠟"}.mdi-find-replace:before{content:"󰛔"}.mdi-fingerprint:before{content:"󰈷"}.mdi-fingerprint-off:before{content:"󰺱"}.mdi-fire:before{content:"󰈸"}.mdi-fire-alert:before{content:"󱗗"}.mdi-fire-circle:before{content:"󱠇"}.mdi-fire-extinguisher:before{content:"󰻲"}.mdi-fire-hydrant:before{content:"󱄷"}.mdi-fire-hydrant-alert:before{content:"󱄸"}.mdi-fire-hydrant-off:before{content:"󱄹"}.mdi-fire-off:before{content:"󱜢"}.mdi-fire-truck:before{content:"󰢫"}.mdi-firebase:before{content:"󰥧"}.mdi-firefox:before{content:"󰈹"}.mdi-fireplace:before{content:"󰸮"}.mdi-fireplace-off:before{content:"󰸯"}.mdi-firewire:before{content:"󰖾"}.mdi-firework:before{content:"󰸰"}.mdi-firework-off:before{content:"󱜣"}.mdi-fish:before{content:"󰈺"}.mdi-fish-off:before{content:"󱏳"}.mdi-fishbowl:before{content:"󰻳"}.mdi-fishbowl-outline:before{content:"󰻴"}.mdi-fit-to-page:before{content:"󰻵"}.mdi-fit-to-page-outline:before{content:"󰻶"}.mdi-fit-to-screen:before{content:"󱣴"}.mdi-fit-to-screen-outline:before{content:"󱣵"}.mdi-flag:before{content:"󰈻"}.mdi-flag-checkered:before{content:"󰈼"}.mdi-flag-minus:before{content:"󰮙"}.mdi-flag-minus-outline:before{content:"󱂲"}.mdi-flag-off:before{content:"󱣮"}.mdi-flag-off-outline:before{content:"󱣯"}.mdi-flag-outline:before{content:"󰈽"}.mdi-flag-plus:before{content:"󰮚"}.mdi-flag-plus-outline:before{content:"󱂳"}.mdi-flag-remove:before{content:"󰮛"}.mdi-flag-remove-outline:before{content:"󱂴"}.mdi-flag-triangle:before{content:"󰈿"}.mdi-flag-variant:before{content:"󰉀"}.mdi-flag-variant-minus:before{content:"󱮴"}.mdi-flag-variant-minus-outline:before{content:"󱮵"}.mdi-flag-variant-off:before{content:"󱮰"}.mdi-flag-variant-off-outline:before{content:"󱮱"}.mdi-flag-variant-outline:before{content:"󰈾"}.mdi-flag-variant-plus:before{content:"󱮲"}.mdi-flag-variant-plus-outline:before{content:"󱮳"}.mdi-flag-variant-remove:before{content:"󱮶"}.mdi-flag-variant-remove-outline:before{content:"󱮷"}.mdi-flare:before{content:"󰵲"}.mdi-flash:before{content:"󰉁"}.mdi-flash-alert:before{content:"󰻷"}.mdi-flash-alert-outline:before{content:"󰻸"}.mdi-flash-auto:before{content:"󰉂"}.mdi-flash-off:before{content:"󰉃"}.mdi-flash-off-outline:before{content:"󱭅"}.mdi-flash-outline:before{content:"󰛕"}.mdi-flash-red-eye:before{content:"󰙻"}.mdi-flash-triangle:before{content:"󱬝"}.mdi-flash-triangle-outline:before{content:"󱬞"}.mdi-flashlight:before{content:"󰉄"}.mdi-flashlight-off:before{content:"󰉅"}.mdi-flask:before{content:"󰂓"}.mdi-flask-empty:before{content:"󰂔"}.mdi-flask-empty-minus:before{content:"󱈺"}.mdi-flask-empty-minus-outline:before{content:"󱈻"}.mdi-flask-empty-off:before{content:"󱏴"}.mdi-flask-empty-off-outline:before{content:"󱏵"}.mdi-flask-empty-outline:before{content:"󰂕"}.mdi-flask-empty-plus:before{content:"󱈼"}.mdi-flask-empty-plus-outline:before{content:"󱈽"}.mdi-flask-empty-remove:before{content:"󱈾"}.mdi-flask-empty-remove-outline:before{content:"󱈿"}.mdi-flask-minus:before{content:"󱉀"}.mdi-flask-minus-outline:before{content:"󱉁"}.mdi-flask-off:before{content:"󱏶"}.mdi-flask-off-outline:before{content:"󱏷"}.mdi-flask-outline:before{content:"󰂖"}.mdi-flask-plus:before{content:"󱉂"}.mdi-flask-plus-outline:before{content:"󱉃"}.mdi-flask-remove:before{content:"󱉄"}.mdi-flask-remove-outline:before{content:"󱉅"}.mdi-flask-round-bottom:before{content:"󱉋"}.mdi-flask-round-bottom-empty:before{content:"󱉌"}.mdi-flask-round-bottom-empty-outline:before{content:"󱉍"}.mdi-flask-round-bottom-outline:before{content:"󱉎"}.mdi-fleur-de-lis:before{content:"󱌃"}.mdi-flip-horizontal:before{content:"󱃧"}.mdi-flip-to-back:before{content:"󰉇"}.mdi-flip-to-front:before{content:"󰉈"}.mdi-flip-vertical:before{content:"󱃨"}.mdi-floor-lamp:before{content:"󰣝"}.mdi-floor-lamp-dual:before{content:"󱁀"}.mdi-floor-lamp-dual-outline:before{content:"󱟎"}.mdi-floor-lamp-outline:before{content:"󱟈"}.mdi-floor-lamp-torchiere:before{content:"󱝇"}.mdi-floor-lamp-torchiere-outline:before{content:"󱟖"}.mdi-floor-lamp-torchiere-variant:before{content:"󱁁"}.mdi-floor-lamp-torchiere-variant-outline:before{content:"󱟏"}.mdi-floor-plan:before{content:"󰠡"}.mdi-floppy:before{content:"󰉉"}.mdi-floppy-variant:before{content:"󰧯"}.mdi-flower:before{content:"󰉊"}.mdi-flower-outline:before{content:"󰧰"}.mdi-flower-pollen:before{content:"󱢅"}.mdi-flower-pollen-outline:before{content:"󱢆"}.mdi-flower-poppy:before{content:"󰴈"}.mdi-flower-tulip:before{content:"󰧱"}.mdi-flower-tulip-outline:before{content:"󰧲"}.mdi-focus-auto:before{content:"󰽎"}.mdi-focus-field:before{content:"󰽏"}.mdi-focus-field-horizontal:before{content:"󰽐"}.mdi-focus-field-vertical:before{content:"󰽑"}.mdi-folder:before{content:"󰉋"}.mdi-folder-account:before{content:"󰉌"}.mdi-folder-account-outline:before{content:"󰮜"}.mdi-folder-alert:before{content:"󰷌"}.mdi-folder-alert-outline:before{content:"󰷍"}.mdi-folder-arrow-down:before{content:"󱧨"}.mdi-folder-arrow-down-outline:before{content:"󱧩"}.mdi-folder-arrow-left:before{content:"󱧪"}.mdi-folder-arrow-left-outline:before{content:"󱧫"}.mdi-folder-arrow-left-right:before{content:"󱧬"}.mdi-folder-arrow-left-right-outline:before{content:"󱧭"}.mdi-folder-arrow-right:before{content:"󱧮"}.mdi-folder-arrow-right-outline:before{content:"󱧯"}.mdi-folder-arrow-up:before{content:"󱧰"}.mdi-folder-arrow-up-down:before{content:"󱧱"}.mdi-folder-arrow-up-down-outline:before{content:"󱧲"}.mdi-folder-arrow-up-outline:before{content:"󱧳"}.mdi-folder-cancel:before{content:"󱧴"}.mdi-folder-cancel-outline:before{content:"󱧵"}.mdi-folder-check:before{content:"󱥾"}.mdi-folder-check-outline:before{content:"󱥿"}.mdi-folder-clock:before{content:"󰪺"}.mdi-folder-clock-outline:before{content:"󰪻"}.mdi-folder-cog:before{content:"󱁿"}.mdi-folder-cog-outline:before{content:"󱂀"}.mdi-folder-download:before{content:"󰉍"}.mdi-folder-download-outline:before{content:"󱃩"}.mdi-folder-edit:before{content:"󰣞"}.mdi-folder-edit-outline:before{content:"󰷎"}.mdi-folder-eye:before{content:"󱞊"}.mdi-folder-eye-outline:before{content:"󱞋"}.mdi-folder-file:before{content:"󱧶"}.mdi-folder-file-outline:before{content:"󱧷"}.mdi-folder-google-drive:before{content:"󰉎"}.mdi-folder-heart:before{content:"󱃪"}.mdi-folder-heart-outline:before{content:"󱃫"}.mdi-folder-hidden:before{content:"󱞞"}.mdi-folder-home:before{content:"󱂵"}.mdi-folder-home-outline:before{content:"󱂶"}.mdi-folder-image:before{content:"󰉏"}.mdi-folder-information:before{content:"󱂷"}.mdi-folder-information-outline:before{content:"󱂸"}.mdi-folder-key:before{content:"󰢬"}.mdi-folder-key-network:before{content:"󰢭"}.mdi-folder-key-network-outline:before{content:"󰲀"}.mdi-folder-key-outline:before{content:"󱃬"}.mdi-folder-lock:before{content:"󰉐"}.mdi-folder-lock-open:before{content:"󰉑"}.mdi-folder-lock-open-outline:before{content:"󱪧"}.mdi-folder-lock-outline:before{content:"󱪨"}.mdi-folder-marker:before{content:"󱉭"}.mdi-folder-marker-outline:before{content:"󱉮"}.mdi-folder-minus:before{content:"󱭉"}.mdi-folder-minus-outline:before{content:"󱭊"}.mdi-folder-move:before{content:"󰉒"}.mdi-folder-move-outline:before{content:"󱉆"}.mdi-folder-multiple:before{content:"󰉓"}.mdi-folder-multiple-image:before{content:"󰉔"}.mdi-folder-multiple-outline:before{content:"󰉕"}.mdi-folder-multiple-plus:before{content:"󱑾"}.mdi-folder-multiple-plus-outline:before{content:"󱑿"}.mdi-folder-music:before{content:"󱍙"}.mdi-folder-music-outline:before{content:"󱍚"}.mdi-folder-network:before{content:"󰡰"}.mdi-folder-network-outline:before{content:"󰲁"}.mdi-folder-off:before{content:"󱧸"}.mdi-folder-off-outline:before{content:"󱧹"}.mdi-folder-open:before{content:"󰝰"}.mdi-folder-open-outline:before{content:"󰷏"}.mdi-folder-outline:before{content:"󰉖"}.mdi-folder-play:before{content:"󱧺"}.mdi-folder-play-outline:before{content:"󱧻"}.mdi-folder-plus:before{content:"󰉗"}.mdi-folder-plus-outline:before{content:"󰮝"}.mdi-folder-pound:before{content:"󰴉"}.mdi-folder-pound-outline:before{content:"󰴊"}.mdi-folder-question:before{content:"󱧊"}.mdi-folder-question-outline:before{content:"󱧋"}.mdi-folder-refresh:before{content:"󰝉"}.mdi-folder-refresh-outline:before{content:"󰕂"}.mdi-folder-remove:before{content:"󰉘"}.mdi-folder-remove-outline:before{content:"󰮞"}.mdi-folder-search:before{content:"󰥨"}.mdi-folder-search-outline:before{content:"󰥩"}.mdi-folder-settings:before{content:"󱁽"}.mdi-folder-settings-outline:before{content:"󱁾"}.mdi-folder-star:before{content:"󰚝"}.mdi-folder-star-multiple:before{content:"󱏓"}.mdi-folder-star-multiple-outline:before{content:"󱏔"}.mdi-folder-star-outline:before{content:"󰮟"}.mdi-folder-swap:before{content:"󰾶"}.mdi-folder-swap-outline:before{content:"󰾷"}.mdi-folder-sync:before{content:"󰴋"}.mdi-folder-sync-outline:before{content:"󰴌"}.mdi-folder-table:before{content:"󱋣"}.mdi-folder-table-outline:before{content:"󱋤"}.mdi-folder-text:before{content:"󰲂"}.mdi-folder-text-outline:before{content:"󰲃"}.mdi-folder-upload:before{content:"󰉙"}.mdi-folder-upload-outline:before{content:"󱃭"}.mdi-folder-wrench:before{content:"󱧼"}.mdi-folder-wrench-outline:before{content:"󱧽"}.mdi-folder-zip:before{content:"󰛫"}.mdi-folder-zip-outline:before{content:"󰞹"}.mdi-font-awesome:before{content:"󰀺"}.mdi-food:before{content:"󰉚"}.mdi-food-apple:before{content:"󰉛"}.mdi-food-apple-outline:before{content:"󰲄"}.mdi-food-croissant:before{content:"󰟈"}.mdi-food-drumstick:before{content:"󱐟"}.mdi-food-drumstick-off:before{content:"󱑨"}.mdi-food-drumstick-off-outline:before{content:"󱑩"}.mdi-food-drumstick-outline:before{content:"󱐠"}.mdi-food-fork-drink:before{content:"󰗲"}.mdi-food-halal:before{content:"󱕲"}.mdi-food-hot-dog:before{content:"󱡋"}.mdi-food-kosher:before{content:"󱕳"}.mdi-food-off:before{content:"󰗳"}.mdi-food-off-outline:before{content:"󱤕"}.mdi-food-outline:before{content:"󱤖"}.mdi-food-steak:before{content:"󱑪"}.mdi-food-steak-off:before{content:"󱑫"}.mdi-food-takeout-box:before{content:"󱠶"}.mdi-food-takeout-box-outline:before{content:"󱠷"}.mdi-food-turkey:before{content:"󱜜"}.mdi-food-variant:before{content:"󰉜"}.mdi-food-variant-off:before{content:"󱏥"}.mdi-foot-print:before{content:"󰽒"}.mdi-football:before{content:"󰉝"}.mdi-football-australian:before{content:"󰉞"}.mdi-football-helmet:before{content:"󰉟"}.mdi-forest:before{content:"󱢗"}.mdi-forklift:before{content:"󰟉"}.mdi-form-dropdown:before{content:"󱐀"}.mdi-form-select:before{content:"󱐁"}.mdi-form-textarea:before{content:"󱂕"}.mdi-form-textbox:before{content:"󰘎"}.mdi-form-textbox-lock:before{content:"󱍝"}.mdi-form-textbox-password:before{content:"󰟵"}.mdi-format-align-bottom:before{content:"󰝓"}.mdi-format-align-center:before{content:"󰉠"}.mdi-format-align-justify:before{content:"󰉡"}.mdi-format-align-left:before{content:"󰉢"}.mdi-format-align-middle:before{content:"󰝔"}.mdi-format-align-right:before{content:"󰉣"}.mdi-format-align-top:before{content:"󰝕"}.mdi-format-annotation-minus:before{content:"󰪼"}.mdi-format-annotation-plus:before{content:"󰙆"}.mdi-format-bold:before{content:"󰉤"}.mdi-format-clear:before{content:"󰉥"}.mdi-format-color-fill:before{content:"󰉦"}.mdi-format-color-highlight:before{content:"󰸱"}.mdi-format-color-marker-cancel:before{content:"󱌓"}.mdi-format-color-text:before{content:"󰚞"}.mdi-format-columns:before{content:"󰣟"}.mdi-format-float-center:before{content:"󰉧"}.mdi-format-float-left:before{content:"󰉨"}.mdi-format-float-none:before{content:"󰉩"}.mdi-format-float-right:before{content:"󰉪"}.mdi-format-font:before{content:"󰛖"}.mdi-format-font-size-decrease:before{content:"󰧳"}.mdi-format-font-size-increase:before{content:"󰧴"}.mdi-format-header-1:before{content:"󰉫"}.mdi-format-header-2:before{content:"󰉬"}.mdi-format-header-3:before{content:"󰉭"}.mdi-format-header-4:before{content:"󰉮"}.mdi-format-header-5:before{content:"󰉯"}.mdi-format-header-6:before{content:"󰉰"}.mdi-format-header-decrease:before{content:"󰉱"}.mdi-format-header-equal:before{content:"󰉲"}.mdi-format-header-increase:before{content:"󰉳"}.mdi-format-header-pound:before{content:"󰉴"}.mdi-format-horizontal-align-center:before{content:"󰘞"}.mdi-format-horizontal-align-left:before{content:"󰘟"}.mdi-format-horizontal-align-right:before{content:"󰘠"}.mdi-format-indent-decrease:before{content:"󰉵"}.mdi-format-indent-increase:before{content:"󰉶"}.mdi-format-italic:before{content:"󰉷"}.mdi-format-letter-case:before{content:"󰬴"}.mdi-format-letter-case-lower:before{content:"󰬵"}.mdi-format-letter-case-upper:before{content:"󰬶"}.mdi-format-letter-ends-with:before{content:"󰾸"}.mdi-format-letter-matches:before{content:"󰾹"}.mdi-format-letter-spacing:before{content:"󱥖"}.mdi-format-letter-spacing-variant:before{content:"󱫻"}.mdi-format-letter-starts-with:before{content:"󰾺"}.mdi-format-line-height:before{content:"󱫼"}.mdi-format-line-spacing:before{content:"󰉸"}.mdi-format-line-style:before{content:"󰗈"}.mdi-format-line-weight:before{content:"󰗉"}.mdi-format-list-bulleted:before{content:"󰉹"}.mdi-format-list-bulleted-square:before{content:"󰷐"}.mdi-format-list-bulleted-triangle:before{content:"󰺲"}.mdi-format-list-bulleted-type:before{content:"󰉺"}.mdi-format-list-checkbox:before{content:"󰥪"}.mdi-format-list-checks:before{content:"󰝖"}.mdi-format-list-group:before{content:"󱡠"}.mdi-format-list-group-plus:before{content:"󱭖"}.mdi-format-list-numbered:before{content:"󰉻"}.mdi-format-list-numbered-rtl:before{content:"󰴍"}.mdi-format-list-text:before{content:"󱉯"}.mdi-format-overline:before{content:"󰺳"}.mdi-format-page-break:before{content:"󰛗"}.mdi-format-page-split:before{content:"󱤗"}.mdi-format-paint:before{content:"󰉼"}.mdi-format-paragraph:before{content:"󰉽"}.mdi-format-paragraph-spacing:before{content:"󱫽"}.mdi-format-pilcrow:before{content:"󰛘"}.mdi-format-pilcrow-arrow-left:before{content:"󰊆"}.mdi-format-pilcrow-arrow-right:before{content:"󰊅"}.mdi-format-quote-close:before{content:"󰉾"}.mdi-format-quote-close-outline:before{content:"󱆨"}.mdi-format-quote-open:before{content:"󰝗"}.mdi-format-quote-open-outline:before{content:"󱆧"}.mdi-format-rotate-90:before{content:"󰚪"}.mdi-format-section:before{content:"󰚟"}.mdi-format-size:before{content:"󰉿"}.mdi-format-strikethrough:before{content:"󰊀"}.mdi-format-strikethrough-variant:before{content:"󰊁"}.mdi-format-subscript:before{content:"󰊂"}.mdi-format-superscript:before{content:"󰊃"}.mdi-format-text:before{content:"󰊄"}.mdi-format-text-rotation-angle-down:before{content:"󰾻"}.mdi-format-text-rotation-angle-up:before{content:"󰾼"}.mdi-format-text-rotation-down:before{content:"󰵳"}.mdi-format-text-rotation-down-vertical:before{content:"󰾽"}.mdi-format-text-rotation-none:before{content:"󰵴"}.mdi-format-text-rotation-up:before{content:"󰾾"}.mdi-format-text-rotation-vertical:before{content:"󰾿"}.mdi-format-text-variant:before{content:"󰸲"}.mdi-format-text-variant-outline:before{content:"󱔏"}.mdi-format-text-wrapping-clip:before{content:"󰴎"}.mdi-format-text-wrapping-overflow:before{content:"󰴏"}.mdi-format-text-wrapping-wrap:before{content:"󰴐"}.mdi-format-textbox:before{content:"󰴑"}.mdi-format-title:before{content:"󰗴"}.mdi-format-underline:before{content:"󰊇"}.mdi-format-underline-wavy:before{content:"󱣩"}.mdi-format-vertical-align-bottom:before{content:"󰘡"}.mdi-format-vertical-align-center:before{content:"󰘢"}.mdi-format-vertical-align-top:before{content:"󰘣"}.mdi-format-wrap-inline:before{content:"󰊈"}.mdi-format-wrap-square:before{content:"󰊉"}.mdi-format-wrap-tight:before{content:"󰊊"}.mdi-format-wrap-top-bottom:before{content:"󰊋"}.mdi-forum:before{content:"󰊌"}.mdi-forum-minus:before{content:"󱪩"}.mdi-forum-minus-outline:before{content:"󱪪"}.mdi-forum-outline:before{content:"󰠢"}.mdi-forum-plus:before{content:"󱪫"}.mdi-forum-plus-outline:before{content:"󱪬"}.mdi-forum-remove:before{content:"󱪭"}.mdi-forum-remove-outline:before{content:"󱪮"}.mdi-forward:before{content:"󰊍"}.mdi-forwardburger:before{content:"󰵵"}.mdi-fountain:before{content:"󰥫"}.mdi-fountain-pen:before{content:"󰴒"}.mdi-fountain-pen-tip:before{content:"󰴓"}.mdi-fraction-one-half:before{content:"󱦒"}.mdi-freebsd:before{content:"󰣠"}.mdi-french-fries:before{content:"󱥗"}.mdi-frequently-asked-questions:before{content:"󰺴"}.mdi-fridge:before{content:"󰊐"}.mdi-fridge-alert:before{content:"󱆱"}.mdi-fridge-alert-outline:before{content:"󱆲"}.mdi-fridge-bottom:before{content:"󰊒"}.mdi-fridge-industrial:before{content:"󱗮"}.mdi-fridge-industrial-alert:before{content:"󱗯"}.mdi-fridge-industrial-alert-outline:before{content:"󱗰"}.mdi-fridge-industrial-off:before{content:"󱗱"}.mdi-fridge-industrial-off-outline:before{content:"󱗲"}.mdi-fridge-industrial-outline:before{content:"󱗳"}.mdi-fridge-off:before{content:"󱆯"}.mdi-fridge-off-outline:before{content:"󱆰"}.mdi-fridge-outline:before{content:"󰊏"}.mdi-fridge-top:before{content:"󰊑"}.mdi-fridge-variant:before{content:"󱗴"}.mdi-fridge-variant-alert:before{content:"󱗵"}.mdi-fridge-variant-alert-outline:before{content:"󱗶"}.mdi-fridge-variant-off:before{content:"󱗷"}.mdi-fridge-variant-off-outline:before{content:"󱗸"}.mdi-fridge-variant-outline:before{content:"󱗹"}.mdi-fruit-cherries:before{content:"󱁂"}.mdi-fruit-cherries-off:before{content:"󱏸"}.mdi-fruit-citrus:before{content:"󱁃"}.mdi-fruit-citrus-off:before{content:"󱏹"}.mdi-fruit-grapes:before{content:"󱁄"}.mdi-fruit-grapes-outline:before{content:"󱁅"}.mdi-fruit-pear:before{content:"󱨎"}.mdi-fruit-pineapple:before{content:"󱁆"}.mdi-fruit-watermelon:before{content:"󱁇"}.mdi-fuel:before{content:"󰟊"}.mdi-fuel-cell:before{content:"󱢵"}.mdi-fullscreen:before{content:"󰊓"}.mdi-fullscreen-exit:before{content:"󰊔"}.mdi-function:before{content:"󰊕"}.mdi-function-variant:before{content:"󰡱"}.mdi-furigana-horizontal:before{content:"󱂁"}.mdi-furigana-vertical:before{content:"󱂂"}.mdi-fuse:before{content:"󰲅"}.mdi-fuse-alert:before{content:"󱐭"}.mdi-fuse-blade:before{content:"󰲆"}.mdi-fuse-off:before{content:"󱐬"}.mdi-gamepad:before{content:"󰊖"}.mdi-gamepad-circle:before{content:"󰸳"}.mdi-gamepad-circle-down:before{content:"󰸴"}.mdi-gamepad-circle-left:before{content:"󰸵"}.mdi-gamepad-circle-outline:before{content:"󰸶"}.mdi-gamepad-circle-right:before{content:"󰸷"}.mdi-gamepad-circle-up:before{content:"󰸸"}.mdi-gamepad-down:before{content:"󰸹"}.mdi-gamepad-left:before{content:"󰸺"}.mdi-gamepad-outline:before{content:"󱤙"}.mdi-gamepad-right:before{content:"󰸻"}.mdi-gamepad-round:before{content:"󰸼"}.mdi-gamepad-round-down:before{content:"󰸽"}.mdi-gamepad-round-left:before{content:"󰸾"}.mdi-gamepad-round-outline:before{content:"󰸿"}.mdi-gamepad-round-right:before{content:"󰹀"}.mdi-gamepad-round-up:before{content:"󰹁"}.mdi-gamepad-square:before{content:"󰺵"}.mdi-gamepad-square-outline:before{content:"󰺶"}.mdi-gamepad-up:before{content:"󰹂"}.mdi-gamepad-variant:before{content:"󰊗"}.mdi-gamepad-variant-outline:before{content:"󰺷"}.mdi-gamma:before{content:"󱃮"}.mdi-gantry-crane:before{content:"󰷑"}.mdi-garage:before{content:"󰛙"}.mdi-garage-alert:before{content:"󰡲"}.mdi-garage-alert-variant:before{content:"󱋕"}.mdi-garage-lock:before{content:"󱟻"}.mdi-garage-open:before{content:"󰛚"}.mdi-garage-open-variant:before{content:"󱋔"}.mdi-garage-variant:before{content:"󱋓"}.mdi-garage-variant-lock:before{content:"󱟼"}.mdi-gas-burner:before{content:"󱨛"}.mdi-gas-cylinder:before{content:"󰙇"}.mdi-gas-station:before{content:"󰊘"}.mdi-gas-station-off:before{content:"󱐉"}.mdi-gas-station-off-outline:before{content:"󱐊"}.mdi-gas-station-outline:before{content:"󰺸"}.mdi-gate:before{content:"󰊙"}.mdi-gate-alert:before{content:"󱟸"}.mdi-gate-and:before{content:"󰣡"}.mdi-gate-arrow-left:before{content:"󱟷"}.mdi-gate-arrow-right:before{content:"󱅩"}.mdi-gate-buffer:before{content:"󱫾"}.mdi-gate-nand:before{content:"󰣢"}.mdi-gate-nor:before{content:"󰣣"}.mdi-gate-not:before{content:"󰣤"}.mdi-gate-open:before{content:"󱅪"}.mdi-gate-or:before{content:"󰣥"}.mdi-gate-xnor:before{content:"󰣦"}.mdi-gate-xor:before{content:"󰣧"}.mdi-gatsby:before{content:"󰹃"}.mdi-gauge:before{content:"󰊚"}.mdi-gauge-empty:before{content:"󰡳"}.mdi-gauge-full:before{content:"󰡴"}.mdi-gauge-low:before{content:"󰡵"}.mdi-gavel:before{content:"󰊛"}.mdi-gender-female:before{content:"󰊜"}.mdi-gender-male:before{content:"󰊝"}.mdi-gender-male-female:before{content:"󰊞"}.mdi-gender-male-female-variant:before{content:"󱄿"}.mdi-gender-non-binary:before{content:"󱅀"}.mdi-gender-transgender:before{content:"󰊟"}.mdi-gentoo:before{content:"󰣨"}.mdi-gesture:before{content:"󰟋"}.mdi-gesture-double-tap:before{content:"󰜼"}.mdi-gesture-pinch:before{content:"󰪽"}.mdi-gesture-spread:before{content:"󰪾"}.mdi-gesture-swipe:before{content:"󰵶"}.mdi-gesture-swipe-down:before{content:"󰜽"}.mdi-gesture-swipe-horizontal:before{content:"󰪿"}.mdi-gesture-swipe-left:before{content:"󰜾"}.mdi-gesture-swipe-right:before{content:"󰜿"}.mdi-gesture-swipe-up:before{content:"󰝀"}.mdi-gesture-swipe-vertical:before{content:"󰫀"}.mdi-gesture-tap:before{content:"󰝁"}.mdi-gesture-tap-box:before{content:"󱊩"}.mdi-gesture-tap-button:before{content:"󱊨"}.mdi-gesture-tap-hold:before{content:"󰵷"}.mdi-gesture-two-double-tap:before{content:"󰝂"}.mdi-gesture-two-tap:before{content:"󰝃"}.mdi-ghost:before{content:"󰊠"}.mdi-ghost-off:before{content:"󰧵"}.mdi-ghost-off-outline:before{content:"󱙜"}.mdi-ghost-outline:before{content:"󱙝"}.mdi-gift:before{content:"󰹄"}.mdi-gift-off:before{content:"󱛯"}.mdi-gift-off-outline:before{content:"󱛰"}.mdi-gift-open:before{content:"󱛱"}.mdi-gift-open-outline:before{content:"󱛲"}.mdi-gift-outline:before{content:"󰊡"}.mdi-git:before{content:"󰊢"}.mdi-github:before{content:"󰊤"}.mdi-gitlab:before{content:"󰮠"}.mdi-glass-cocktail:before{content:"󰍖"}.mdi-glass-cocktail-off:before{content:"󱗦"}.mdi-glass-flute:before{content:"󰊥"}.mdi-glass-fragile:before{content:"󱡳"}.mdi-glass-mug:before{content:"󰊦"}.mdi-glass-mug-off:before{content:"󱗧"}.mdi-glass-mug-variant:before{content:"󱄖"}.mdi-glass-mug-variant-off:before{content:"󱗨"}.mdi-glass-pint-outline:before{content:"󱌍"}.mdi-glass-stange:before{content:"󰊧"}.mdi-glass-tulip:before{content:"󰊨"}.mdi-glass-wine:before{content:"󰡶"}.mdi-glasses:before{content:"󰊪"}.mdi-globe-light:before{content:"󰙯"}.mdi-globe-light-outline:before{content:"󱋗"}.mdi-globe-model:before{content:"󰣩"}.mdi-gmail:before{content:"󰊫"}.mdi-gnome:before{content:"󰊬"}.mdi-go-kart:before{content:"󰵹"}.mdi-go-kart-track:before{content:"󰵺"}.mdi-gog:before{content:"󰮡"}.mdi-gold:before{content:"󱉏"}.mdi-golf:before{content:"󰠣"}.mdi-golf-cart:before{content:"󱆤"}.mdi-golf-tee:before{content:"󱂃"}.mdi-gondola:before{content:"󰚆"}.mdi-goodreads:before{content:"󰵻"}.mdi-google:before{content:"󰊭"}.mdi-google-ads:before{content:"󰲇"}.mdi-google-analytics:before{content:"󰟌"}.mdi-google-assistant:before{content:"󰟍"}.mdi-google-cardboard:before{content:"󰊮"}.mdi-google-chrome:before{content:"󰊯"}.mdi-google-circles:before{content:"󰊰"}.mdi-google-circles-communities:before{content:"󰊱"}.mdi-google-circles-extended:before{content:"󰊲"}.mdi-google-circles-group:before{content:"󰊳"}.mdi-google-classroom:before{content:"󰋀"}.mdi-google-cloud:before{content:"󱇶"}.mdi-google-downasaur:before{content:"󱍢"}.mdi-google-drive:before{content:"󰊶"}.mdi-google-earth:before{content:"󰊷"}.mdi-google-fit:before{content:"󰥬"}.mdi-google-glass:before{content:"󰊸"}.mdi-google-hangouts:before{content:"󰋉"}.mdi-google-keep:before{content:"󰛜"}.mdi-google-lens:before{content:"󰧶"}.mdi-google-maps:before{content:"󰗵"}.mdi-google-my-business:before{content:"󱁈"}.mdi-google-nearby:before{content:"󰊹"}.mdi-google-play:before{content:"󰊼"}.mdi-google-plus:before{content:"󰊽"}.mdi-google-podcast:before{content:"󰺹"}.mdi-google-spreadsheet:before{content:"󰧷"}.mdi-google-street-view:before{content:"󰲈"}.mdi-google-translate:before{content:"󰊿"}.mdi-gradient-horizontal:before{content:"󱝊"}.mdi-gradient-vertical:before{content:"󰚠"}.mdi-grain:before{content:"󰵼"}.mdi-graph:before{content:"󱁉"}.mdi-graph-outline:before{content:"󱁊"}.mdi-graphql:before{content:"󰡷"}.mdi-grass:before{content:"󱔐"}.mdi-grave-stone:before{content:"󰮢"}.mdi-grease-pencil:before{content:"󰙈"}.mdi-greater-than:before{content:"󰥭"}.mdi-greater-than-or-equal:before{content:"󰥮"}.mdi-greenhouse:before{content:"󰀭"}.mdi-grid:before{content:"󰋁"}.mdi-grid-large:before{content:"󰝘"}.mdi-grid-off:before{content:"󰋂"}.mdi-grill:before{content:"󰹅"}.mdi-grill-outline:before{content:"󱆊"}.mdi-group:before{content:"󰋃"}.mdi-guitar-acoustic:before{content:"󰝱"}.mdi-guitar-electric:before{content:"󰋄"}.mdi-guitar-pick:before{content:"󰋅"}.mdi-guitar-pick-outline:before{content:"󰋆"}.mdi-guy-fawkes-mask:before{content:"󰠥"}.mdi-gymnastics:before{content:"󱩁"}.mdi-hail:before{content:"󰫁"}.mdi-hair-dryer:before{content:"󱃯"}.mdi-hair-dryer-outline:before{content:"󱃰"}.mdi-halloween:before{content:"󰮣"}.mdi-hamburger:before{content:"󰚅"}.mdi-hamburger-check:before{content:"󱝶"}.mdi-hamburger-minus:before{content:"󱝷"}.mdi-hamburger-off:before{content:"󱝸"}.mdi-hamburger-plus:before{content:"󱝹"}.mdi-hamburger-remove:before{content:"󱝺"}.mdi-hammer:before{content:"󰣪"}.mdi-hammer-screwdriver:before{content:"󱌢"}.mdi-hammer-sickle:before{content:"󱢇"}.mdi-hammer-wrench:before{content:"󱌣"}.mdi-hand-back-left:before{content:"󰹆"}.mdi-hand-back-left-off:before{content:"󱠰"}.mdi-hand-back-left-off-outline:before{content:"󱠲"}.mdi-hand-back-left-outline:before{content:"󱠬"}.mdi-hand-back-right:before{content:"󰹇"}.mdi-hand-back-right-off:before{content:"󱠱"}.mdi-hand-back-right-off-outline:before{content:"󱠳"}.mdi-hand-back-right-outline:before{content:"󱠭"}.mdi-hand-clap:before{content:"󱥋"}.mdi-hand-clap-off:before{content:"󱩂"}.mdi-hand-coin:before{content:"󱢏"}.mdi-hand-coin-outline:before{content:"󱢐"}.mdi-hand-cycle:before{content:"󱮜"}.mdi-hand-extended:before{content:"󱢶"}.mdi-hand-extended-outline:before{content:"󱢷"}.mdi-hand-front-left:before{content:"󱠫"}.mdi-hand-front-left-outline:before{content:"󱠮"}.mdi-hand-front-right:before{content:"󰩏"}.mdi-hand-front-right-outline:before{content:"󱠯"}.mdi-hand-heart:before{content:"󱃱"}.mdi-hand-heart-outline:before{content:"󱕾"}.mdi-hand-okay:before{content:"󰩐"}.mdi-hand-peace:before{content:"󰩑"}.mdi-hand-peace-variant:before{content:"󰩒"}.mdi-hand-pointing-down:before{content:"󰩓"}.mdi-hand-pointing-left:before{content:"󰩔"}.mdi-hand-pointing-right:before{content:"󰋇"}.mdi-hand-pointing-up:before{content:"󰩕"}.mdi-hand-saw:before{content:"󰹈"}.mdi-hand-wash:before{content:"󱕿"}.mdi-hand-wash-outline:before{content:"󱖀"}.mdi-hand-water:before{content:"󱎟"}.mdi-hand-wave:before{content:"󱠡"}.mdi-hand-wave-outline:before{content:"󱠢"}.mdi-handball:before{content:"󰽓"}.mdi-handcuffs:before{content:"󱄾"}.mdi-hands-pray:before{content:"󰕹"}.mdi-handshake:before{content:"󱈘"}.mdi-handshake-outline:before{content:"󱖡"}.mdi-hanger:before{content:"󰋈"}.mdi-hard-hat:before{content:"󰥯"}.mdi-harddisk:before{content:"󰋊"}.mdi-harddisk-plus:before{content:"󱁋"}.mdi-harddisk-remove:before{content:"󱁌"}.mdi-hat-fedora:before{content:"󰮤"}.mdi-hazard-lights:before{content:"󰲉"}.mdi-hdmi-port:before{content:"󱮸"}.mdi-hdr:before{content:"󰵽"}.mdi-hdr-off:before{content:"󰵾"}.mdi-head:before{content:"󱍞"}.mdi-head-alert:before{content:"󱌸"}.mdi-head-alert-outline:before{content:"󱌹"}.mdi-head-check:before{content:"󱌺"}.mdi-head-check-outline:before{content:"󱌻"}.mdi-head-cog:before{content:"󱌼"}.mdi-head-cog-outline:before{content:"󱌽"}.mdi-head-dots-horizontal:before{content:"󱌾"}.mdi-head-dots-horizontal-outline:before{content:"󱌿"}.mdi-head-flash:before{content:"󱍀"}.mdi-head-flash-outline:before{content:"󱍁"}.mdi-head-heart:before{content:"󱍂"}.mdi-head-heart-outline:before{content:"󱍃"}.mdi-head-lightbulb:before{content:"󱍄"}.mdi-head-lightbulb-outline:before{content:"󱍅"}.mdi-head-minus:before{content:"󱍆"}.mdi-head-minus-outline:before{content:"󱍇"}.mdi-head-outline:before{content:"󱍟"}.mdi-head-plus:before{content:"󱍈"}.mdi-head-plus-outline:before{content:"󱍉"}.mdi-head-question:before{content:"󱍊"}.mdi-head-question-outline:before{content:"󱍋"}.mdi-head-remove:before{content:"󱍌"}.mdi-head-remove-outline:before{content:"󱍍"}.mdi-head-snowflake:before{content:"󱍎"}.mdi-head-snowflake-outline:before{content:"󱍏"}.mdi-head-sync:before{content:"󱍐"}.mdi-head-sync-outline:before{content:"󱍑"}.mdi-headphones:before{content:"󰋋"}.mdi-headphones-bluetooth:before{content:"󰥰"}.mdi-headphones-box:before{content:"󰋌"}.mdi-headphones-off:before{content:"󰟎"}.mdi-headphones-settings:before{content:"󰋍"}.mdi-headset:before{content:"󰋎"}.mdi-headset-dock:before{content:"󰋏"}.mdi-headset-off:before{content:"󰋐"}.mdi-heart:before{content:"󰋑"}.mdi-heart-box:before{content:"󰋒"}.mdi-heart-box-outline:before{content:"󰋓"}.mdi-heart-broken:before{content:"󰋔"}.mdi-heart-broken-outline:before{content:"󰴔"}.mdi-heart-circle:before{content:"󰥱"}.mdi-heart-circle-outline:before{content:"󰥲"}.mdi-heart-cog:before{content:"󱙣"}.mdi-heart-cog-outline:before{content:"󱙤"}.mdi-heart-flash:before{content:"󰻹"}.mdi-heart-half:before{content:"󰛟"}.mdi-heart-half-full:before{content:"󰛞"}.mdi-heart-half-outline:before{content:"󰛠"}.mdi-heart-minus:before{content:"󱐯"}.mdi-heart-minus-outline:before{content:"󱐲"}.mdi-heart-multiple:before{content:"󰩖"}.mdi-heart-multiple-outline:before{content:"󰩗"}.mdi-heart-off:before{content:"󰝙"}.mdi-heart-off-outline:before{content:"󱐴"}.mdi-heart-outline:before{content:"󰋕"}.mdi-heart-plus:before{content:"󱐮"}.mdi-heart-plus-outline:before{content:"󱐱"}.mdi-heart-pulse:before{content:"󰗶"}.mdi-heart-remove:before{content:"󱐰"}.mdi-heart-remove-outline:before{content:"󱐳"}.mdi-heart-settings:before{content:"󱙥"}.mdi-heart-settings-outline:before{content:"󱙦"}.mdi-heat-pump:before{content:"󱩃"}.mdi-heat-pump-outline:before{content:"󱩄"}.mdi-heat-wave:before{content:"󱩅"}.mdi-heating-coil:before{content:"󱪯"}.mdi-helicopter:before{content:"󰫂"}.mdi-help:before{content:"󰋖"}.mdi-help-box:before{content:"󰞋"}.mdi-help-circle:before{content:"󰋗"}.mdi-help-circle-outline:before{content:"󰘥"}.mdi-help-network:before{content:"󰛵"}.mdi-help-network-outline:before{content:"󰲊"}.mdi-help-rhombus:before{content:"󰮥"}.mdi-help-rhombus-outline:before{content:"󰮦"}.mdi-hexadecimal:before{content:"󱊧"}.mdi-hexagon:before{content:"󰋘"}.mdi-hexagon-multiple:before{content:"󰛡"}.mdi-hexagon-multiple-outline:before{content:"󱃲"}.mdi-hexagon-outline:before{content:"󰋙"}.mdi-hexagon-slice-1:before{content:"󰫃"}.mdi-hexagon-slice-2:before{content:"󰫄"}.mdi-hexagon-slice-3:before{content:"󰫅"}.mdi-hexagon-slice-4:before{content:"󰫆"}.mdi-hexagon-slice-5:before{content:"󰫇"}.mdi-hexagon-slice-6:before{content:"󰫈"}.mdi-hexagram:before{content:"󰫉"}.mdi-hexagram-outline:before{content:"󰫊"}.mdi-high-definition:before{content:"󰟏"}.mdi-high-definition-box:before{content:"󰡸"}.mdi-highway:before{content:"󰗷"}.mdi-hiking:before{content:"󰵿"}.mdi-history:before{content:"󰋚"}.mdi-hockey-puck:before{content:"󰡹"}.mdi-hockey-sticks:before{content:"󰡺"}.mdi-hololens:before{content:"󰋛"}.mdi-home:before{content:"󰋜"}.mdi-home-account:before{content:"󰠦"}.mdi-home-alert:before{content:"󰡻"}.mdi-home-alert-outline:before{content:"󱗐"}.mdi-home-analytics:before{content:"󰺺"}.mdi-home-assistant:before{content:"󰟐"}.mdi-home-automation:before{content:"󰟑"}.mdi-home-battery:before{content:"󱤁"}.mdi-home-battery-outline:before{content:"󱤂"}.mdi-home-circle:before{content:"󰟒"}.mdi-home-circle-outline:before{content:"󱁍"}.mdi-home-city:before{content:"󰴕"}.mdi-home-city-outline:before{content:"󰴖"}.mdi-home-clock:before{content:"󱨒"}.mdi-home-clock-outline:before{content:"󱨓"}.mdi-home-edit:before{content:"󱅙"}.mdi-home-edit-outline:before{content:"󱅚"}.mdi-home-export-outline:before{content:"󰾛"}.mdi-home-flood:before{content:"󰻺"}.mdi-home-floor-0:before{content:"󰷒"}.mdi-home-floor-1:before{content:"󰶀"}.mdi-home-floor-2:before{content:"󰶁"}.mdi-home-floor-3:before{content:"󰶂"}.mdi-home-floor-a:before{content:"󰶃"}.mdi-home-floor-b:before{content:"󰶄"}.mdi-home-floor-g:before{content:"󰶅"}.mdi-home-floor-l:before{content:"󰶆"}.mdi-home-floor-negative-1:before{content:"󰷓"}.mdi-home-group:before{content:"󰷔"}.mdi-home-group-minus:before{content:"󱧁"}.mdi-home-group-plus:before{content:"󱧀"}.mdi-home-group-remove:before{content:"󱧂"}.mdi-home-heart:before{content:"󰠧"}.mdi-home-import-outline:before{content:"󰾜"}.mdi-home-lightbulb:before{content:"󱉑"}.mdi-home-lightbulb-outline:before{content:"󱉒"}.mdi-home-lightning-bolt:before{content:"󱤃"}.mdi-home-lightning-bolt-outline:before{content:"󱤄"}.mdi-home-lock:before{content:"󰣫"}.mdi-home-lock-open:before{content:"󰣬"}.mdi-home-map-marker:before{content:"󰗸"}.mdi-home-minus:before{content:"󰥴"}.mdi-home-minus-outline:before{content:"󱏕"}.mdi-home-modern:before{content:"󰋝"}.mdi-home-off:before{content:"󱩆"}.mdi-home-off-outline:before{content:"󱩇"}.mdi-home-outline:before{content:"󰚡"}.mdi-home-plus:before{content:"󰥵"}.mdi-home-plus-outline:before{content:"󱏖"}.mdi-home-remove:before{content:"󱉇"}.mdi-home-remove-outline:before{content:"󱏗"}.mdi-home-roof:before{content:"󱄫"}.mdi-home-search:before{content:"󱎰"}.mdi-home-search-outline:before{content:"󱎱"}.mdi-home-silo:before{content:"󱮠"}.mdi-home-silo-outline:before{content:"󱮡"}.mdi-home-switch:before{content:"󱞔"}.mdi-home-switch-outline:before{content:"󱞕"}.mdi-home-thermometer:before{content:"󰽔"}.mdi-home-thermometer-outline:before{content:"󰽕"}.mdi-home-variant:before{content:"󰋞"}.mdi-home-variant-outline:before{content:"󰮧"}.mdi-hook:before{content:"󰛢"}.mdi-hook-off:before{content:"󰛣"}.mdi-hoop-house:before{content:"󰹖"}.mdi-hops:before{content:"󰋟"}.mdi-horizontal-rotate-clockwise:before{content:"󱃳"}.mdi-horizontal-rotate-counterclockwise:before{content:"󱃴"}.mdi-horse:before{content:"󱖿"}.mdi-horse-human:before{content:"󱗀"}.mdi-horse-variant:before{content:"󱗁"}.mdi-horse-variant-fast:before{content:"󱡮"}.mdi-horseshoe:before{content:"󰩘"}.mdi-hospital:before{content:"󰿶"}.mdi-hospital-box:before{content:"󰋠"}.mdi-hospital-box-outline:before{content:"󰿷"}.mdi-hospital-building:before{content:"󰋡"}.mdi-hospital-marker:before{content:"󰋢"}.mdi-hot-tub:before{content:"󰠨"}.mdi-hours-24:before{content:"󱑸"}.mdi-hubspot:before{content:"󰴗"}.mdi-hulu:before{content:"󰠩"}.mdi-human:before{content:"󰋦"}.mdi-human-baby-changing-table:before{content:"󱎋"}.mdi-human-cane:before{content:"󱖁"}.mdi-human-capacity-decrease:before{content:"󱖛"}.mdi-human-capacity-increase:before{content:"󱖜"}.mdi-human-child:before{content:"󰋧"}.mdi-human-dolly:before{content:"󱦀"}.mdi-human-edit:before{content:"󱓨"}.mdi-human-female:before{content:"󰙉"}.mdi-human-female-boy:before{content:"󰩙"}.mdi-human-female-dance:before{content:"󱗉"}.mdi-human-female-female:before{content:"󰩚"}.mdi-human-female-girl:before{content:"󰩛"}.mdi-human-greeting:before{content:"󱟄"}.mdi-human-greeting-proximity:before{content:"󱖝"}.mdi-human-greeting-variant:before{content:"󰙊"}.mdi-human-handsdown:before{content:"󰙋"}.mdi-human-handsup:before{content:"󰙌"}.mdi-human-male:before{content:"󰙍"}.mdi-human-male-board:before{content:"󰢐"}.mdi-human-male-board-poll:before{content:"󰡆"}.mdi-human-male-boy:before{content:"󰩜"}.mdi-human-male-child:before{content:"󱎌"}.mdi-human-male-female:before{content:"󰋨"}.mdi-human-male-female-child:before{content:"󱠣"}.mdi-human-male-girl:before{content:"󰩝"}.mdi-human-male-height:before{content:"󰻻"}.mdi-human-male-height-variant:before{content:"󰻼"}.mdi-human-male-male:before{content:"󰩞"}.mdi-human-non-binary:before{content:"󱡈"}.mdi-human-pregnant:before{content:"󰗏"}.mdi-human-queue:before{content:"󱕱"}.mdi-human-scooter:before{content:"󱇩"}.mdi-human-walker:before{content:"󱭱"}.mdi-human-wheelchair:before{content:"󱎍"}.mdi-human-white-cane:before{content:"󱦁"}.mdi-humble-bundle:before{content:"󰝄"}.mdi-hvac:before{content:"󱍒"}.mdi-hvac-off:before{content:"󱖞"}.mdi-hydraulic-oil-level:before{content:"󱌤"}.mdi-hydraulic-oil-temperature:before{content:"󱌥"}.mdi-hydro-power:before{content:"󱋥"}.mdi-hydrogen-station:before{content:"󱢔"}.mdi-ice-cream:before{content:"󰠪"}.mdi-ice-cream-off:before{content:"󰹒"}.mdi-ice-pop:before{content:"󰻽"}.mdi-id-card:before{content:"󰿀"}.mdi-identifier:before{content:"󰻾"}.mdi-ideogram-cjk:before{content:"󱌱"}.mdi-ideogram-cjk-variant:before{content:"󱌲"}.mdi-image:before{content:"󰋩"}.mdi-image-album:before{content:"󰋪"}.mdi-image-area:before{content:"󰋫"}.mdi-image-area-close:before{content:"󰋬"}.mdi-image-auto-adjust:before{content:"󰿁"}.mdi-image-broken:before{content:"󰋭"}.mdi-image-broken-variant:before{content:"󰋮"}.mdi-image-check:before{content:"󱬥"}.mdi-image-check-outline:before{content:"󱬦"}.mdi-image-edit:before{content:"󱇣"}.mdi-image-edit-outline:before{content:"󱇤"}.mdi-image-filter-black-white:before{content:"󰋰"}.mdi-image-filter-center-focus:before{content:"󰋱"}.mdi-image-filter-center-focus-strong:before{content:"󰻿"}.mdi-image-filter-center-focus-strong-outline:before{content:"󰼀"}.mdi-image-filter-center-focus-weak:before{content:"󰋲"}.mdi-image-filter-drama:before{content:"󰋳"}.mdi-image-filter-frames:before{content:"󰋴"}.mdi-image-filter-hdr:before{content:"󰋵"}.mdi-image-filter-none:before{content:"󰋶"}.mdi-image-filter-tilt-shift:before{content:"󰋷"}.mdi-image-filter-vintage:before{content:"󰋸"}.mdi-image-frame:before{content:"󰹉"}.mdi-image-lock:before{content:"󱪰"}.mdi-image-lock-outline:before{content:"󱪱"}.mdi-image-marker:before{content:"󱝻"}.mdi-image-marker-outline:before{content:"󱝼"}.mdi-image-minus:before{content:"󱐙"}.mdi-image-minus-outline:before{content:"󱭇"}.mdi-image-move:before{content:"󰧸"}.mdi-image-multiple:before{content:"󰋹"}.mdi-image-multiple-outline:before{content:"󰋯"}.mdi-image-off:before{content:"󰠫"}.mdi-image-off-outline:before{content:"󱇑"}.mdi-image-outline:before{content:"󰥶"}.mdi-image-plus:before{content:"󰡼"}.mdi-image-plus-outline:before{content:"󱭆"}.mdi-image-refresh:before{content:"󱧾"}.mdi-image-refresh-outline:before{content:"󱧿"}.mdi-image-remove:before{content:"󱐘"}.mdi-image-remove-outline:before{content:"󱭈"}.mdi-image-search:before{content:"󰥷"}.mdi-image-search-outline:before{content:"󰥸"}.mdi-image-size-select-actual:before{content:"󰲍"}.mdi-image-size-select-large:before{content:"󰲎"}.mdi-image-size-select-small:before{content:"󰲏"}.mdi-image-sync:before{content:"󱨀"}.mdi-image-sync-outline:before{content:"󱨁"}.mdi-image-text:before{content:"󱘍"}.mdi-import:before{content:"󰋺"}.mdi-inbox:before{content:"󰚇"}.mdi-inbox-arrow-down:before{content:"󰋻"}.mdi-inbox-arrow-down-outline:before{content:"󱉰"}.mdi-inbox-arrow-up:before{content:"󰏑"}.mdi-inbox-arrow-up-outline:before{content:"󱉱"}.mdi-inbox-full:before{content:"󱉲"}.mdi-inbox-full-outline:before{content:"󱉳"}.mdi-inbox-multiple:before{content:"󰢰"}.mdi-inbox-multiple-outline:before{content:"󰮨"}.mdi-inbox-outline:before{content:"󱉴"}.mdi-inbox-remove:before{content:"󱖟"}.mdi-inbox-remove-outline:before{content:"󱖠"}.mdi-incognito:before{content:"󰗹"}.mdi-incognito-circle:before{content:"󱐡"}.mdi-incognito-circle-off:before{content:"󱐢"}.mdi-incognito-off:before{content:"󰁵"}.mdi-induction:before{content:"󱡌"}.mdi-infinity:before{content:"󰛤"}.mdi-information:before{content:"󰋼"}.mdi-information-off:before{content:"󱞌"}.mdi-information-off-outline:before{content:"󱞍"}.mdi-information-outline:before{content:"󰋽"}.mdi-information-variant:before{content:"󰙎"}.mdi-instagram:before{content:"󰋾"}.mdi-instrument-triangle:before{content:"󱁎"}.mdi-integrated-circuit-chip:before{content:"󱤓"}.mdi-invert-colors:before{content:"󰌁"}.mdi-invert-colors-off:before{content:"󰹊"}.mdi-iobroker:before{content:"󱋨"}.mdi-ip:before{content:"󰩟"}.mdi-ip-network:before{content:"󰩠"}.mdi-ip-network-outline:before{content:"󰲐"}.mdi-ip-outline:before{content:"󱦂"}.mdi-ipod:before{content:"󰲑"}.mdi-iron:before{content:"󱠤"}.mdi-iron-board:before{content:"󱠸"}.mdi-iron-outline:before{content:"󱠥"}.mdi-island:before{content:"󱁏"}.mdi-iv-bag:before{content:"󱂹"}.mdi-jabber:before{content:"󰷕"}.mdi-jeepney:before{content:"󰌂"}.mdi-jellyfish:before{content:"󰼁"}.mdi-jellyfish-outline:before{content:"󰼂"}.mdi-jira:before{content:"󰌃"}.mdi-jquery:before{content:"󰡽"}.mdi-jsfiddle:before{content:"󰌄"}.mdi-jump-rope:before{content:"󱋿"}.mdi-kabaddi:before{content:"󰶇"}.mdi-kangaroo:before{content:"󱕘"}.mdi-karate:before{content:"󰠬"}.mdi-kayaking:before{content:"󰢯"}.mdi-keg:before{content:"󰌅"}.mdi-kettle:before{content:"󰗺"}.mdi-kettle-alert:before{content:"󱌗"}.mdi-kettle-alert-outline:before{content:"󱌘"}.mdi-kettle-off:before{content:"󱌛"}.mdi-kettle-off-outline:before{content:"󱌜"}.mdi-kettle-outline:before{content:"󰽖"}.mdi-kettle-pour-over:before{content:"󱜼"}.mdi-kettle-steam:before{content:"󱌙"}.mdi-kettle-steam-outline:before{content:"󱌚"}.mdi-kettlebell:before{content:"󱌀"}.mdi-key:before{content:"󰌆"}.mdi-key-alert:before{content:"󱦃"}.mdi-key-alert-outline:before{content:"󱦄"}.mdi-key-arrow-right:before{content:"󱌒"}.mdi-key-chain:before{content:"󱕴"}.mdi-key-chain-variant:before{content:"󱕵"}.mdi-key-change:before{content:"󰌇"}.mdi-key-link:before{content:"󱆟"}.mdi-key-minus:before{content:"󰌈"}.mdi-key-outline:before{content:"󰷖"}.mdi-key-plus:before{content:"󰌉"}.mdi-key-remove:before{content:"󰌊"}.mdi-key-star:before{content:"󱆞"}.mdi-key-variant:before{content:"󰌋"}.mdi-key-wireless:before{content:"󰿂"}.mdi-keyboard:before{content:"󰌌"}.mdi-keyboard-backspace:before{content:"󰌍"}.mdi-keyboard-caps:before{content:"󰌎"}.mdi-keyboard-close:before{content:"󰌏"}.mdi-keyboard-esc:before{content:"󱊷"}.mdi-keyboard-f1:before{content:"󱊫"}.mdi-keyboard-f10:before{content:"󱊴"}.mdi-keyboard-f11:before{content:"󱊵"}.mdi-keyboard-f12:before{content:"󱊶"}.mdi-keyboard-f2:before{content:"󱊬"}.mdi-keyboard-f3:before{content:"󱊭"}.mdi-keyboard-f4:before{content:"󱊮"}.mdi-keyboard-f5:before{content:"󱊯"}.mdi-keyboard-f6:before{content:"󱊰"}.mdi-keyboard-f7:before{content:"󱊱"}.mdi-keyboard-f8:before{content:"󱊲"}.mdi-keyboard-f9:before{content:"󱊳"}.mdi-keyboard-off:before{content:"󰌐"}.mdi-keyboard-off-outline:before{content:"󰹋"}.mdi-keyboard-outline:before{content:"󰥻"}.mdi-keyboard-return:before{content:"󰌑"}.mdi-keyboard-settings:before{content:"󰧹"}.mdi-keyboard-settings-outline:before{content:"󰧺"}.mdi-keyboard-space:before{content:"󱁐"}.mdi-keyboard-tab:before{content:"󰌒"}.mdi-keyboard-tab-reverse:before{content:"󰌥"}.mdi-keyboard-variant:before{content:"󰌓"}.mdi-khanda:before{content:"󱃽"}.mdi-kickstarter:before{content:"󰝅"}.mdi-kite:before{content:"󱦅"}.mdi-kite-outline:before{content:"󱦆"}.mdi-kitesurfing:before{content:"󱝄"}.mdi-klingon:before{content:"󱍛"}.mdi-knife:before{content:"󰧻"}.mdi-knife-military:before{content:"󰧼"}.mdi-knob:before{content:"󱮖"}.mdi-koala:before{content:"󱜿"}.mdi-kodi:before{content:"󰌔"}.mdi-kubernetes:before{content:"󱃾"}.mdi-label:before{content:"󰌕"}.mdi-label-multiple:before{content:"󱍵"}.mdi-label-multiple-outline:before{content:"󱍶"}.mdi-label-off:before{content:"󰫋"}.mdi-label-off-outline:before{content:"󰫌"}.mdi-label-outline:before{content:"󰌖"}.mdi-label-percent:before{content:"󱋪"}.mdi-label-percent-outline:before{content:"󱋫"}.mdi-label-variant:before{content:"󰫍"}.mdi-label-variant-outline:before{content:"󰫎"}.mdi-ladder:before{content:"󱖢"}.mdi-ladybug:before{content:"󰠭"}.mdi-lambda:before{content:"󰘧"}.mdi-lamp:before{content:"󰚵"}.mdi-lamp-outline:before{content:"󱟐"}.mdi-lamps:before{content:"󱕶"}.mdi-lamps-outline:before{content:"󱟑"}.mdi-lan:before{content:"󰌗"}.mdi-lan-check:before{content:"󱊪"}.mdi-lan-connect:before{content:"󰌘"}.mdi-lan-disconnect:before{content:"󰌙"}.mdi-lan-pending:before{content:"󰌚"}.mdi-land-fields:before{content:"󱪲"}.mdi-land-plots:before{content:"󱪳"}.mdi-land-plots-circle:before{content:"󱪴"}.mdi-land-plots-circle-variant:before{content:"󱪵"}.mdi-land-rows-horizontal:before{content:"󱪶"}.mdi-land-rows-vertical:before{content:"󱪷"}.mdi-landslide:before{content:"󱩈"}.mdi-landslide-outline:before{content:"󱩉"}.mdi-language-c:before{content:"󰙱"}.mdi-language-cpp:before{content:"󰙲"}.mdi-language-csharp:before{content:"󰌛"}.mdi-language-css3:before{content:"󰌜"}.mdi-language-fortran:before{content:"󱈚"}.mdi-language-go:before{content:"󰟓"}.mdi-language-haskell:before{content:"󰲒"}.mdi-language-html5:before{content:"󰌝"}.mdi-language-java:before{content:"󰬷"}.mdi-language-javascript:before{content:"󰌞"}.mdi-language-kotlin:before{content:"󱈙"}.mdi-language-lua:before{content:"󰢱"}.mdi-language-markdown:before{content:"󰍔"}.mdi-language-markdown-outline:before{content:"󰽛"}.mdi-language-php:before{content:"󰌟"}.mdi-language-python:before{content:"󰌠"}.mdi-language-r:before{content:"󰟔"}.mdi-language-ruby:before{content:"󰴭"}.mdi-language-ruby-on-rails:before{content:"󰫏"}.mdi-language-rust:before{content:"󱘗"}.mdi-language-swift:before{content:"󰛥"}.mdi-language-typescript:before{content:"󰛦"}.mdi-language-xaml:before{content:"󰙳"}.mdi-laptop:before{content:"󰌢"}.mdi-laptop-account:before{content:"󱩊"}.mdi-laptop-off:before{content:"󰛧"}.mdi-laravel:before{content:"󰫐"}.mdi-laser-pointer:before{content:"󱒄"}.mdi-lasso:before{content:"󰼃"}.mdi-lastpass:before{content:"󰑆"}.mdi-latitude:before{content:"󰽗"}.mdi-launch:before{content:"󰌧"}.mdi-lava-lamp:before{content:"󰟕"}.mdi-layers:before{content:"󰌨"}.mdi-layers-edit:before{content:"󱢒"}.mdi-layers-minus:before{content:"󰹌"}.mdi-layers-off:before{content:"󰌩"}.mdi-layers-off-outline:before{content:"󰧽"}.mdi-layers-outline:before{content:"󰧾"}.mdi-layers-plus:before{content:"󰹍"}.mdi-layers-remove:before{content:"󰹎"}.mdi-layers-search:before{content:"󱈆"}.mdi-layers-search-outline:before{content:"󱈇"}.mdi-layers-triple:before{content:"󰽘"}.mdi-layers-triple-outline:before{content:"󰽙"}.mdi-lead-pencil:before{content:"󰙏"}.mdi-leaf:before{content:"󰌪"}.mdi-leaf-circle:before{content:"󱤅"}.mdi-leaf-circle-outline:before{content:"󱤆"}.mdi-leaf-maple:before{content:"󰲓"}.mdi-leaf-maple-off:before{content:"󱋚"}.mdi-leaf-off:before{content:"󱋙"}.mdi-leak:before{content:"󰷗"}.mdi-leak-off:before{content:"󰷘"}.mdi-lectern:before{content:"󱫰"}.mdi-led-off:before{content:"󰌫"}.mdi-led-on:before{content:"󰌬"}.mdi-led-outline:before{content:"󰌭"}.mdi-led-strip:before{content:"󰟖"}.mdi-led-strip-variant:before{content:"󱁑"}.mdi-led-strip-variant-off:before{content:"󱩋"}.mdi-led-variant-off:before{content:"󰌮"}.mdi-led-variant-on:before{content:"󰌯"}.mdi-led-variant-outline:before{content:"󰌰"}.mdi-leek:before{content:"󱅽"}.mdi-less-than:before{content:"󰥼"}.mdi-less-than-or-equal:before{content:"󰥽"}.mdi-library:before{content:"󰌱"}.mdi-library-outline:before{content:"󱨢"}.mdi-library-shelves:before{content:"󰮩"}.mdi-license:before{content:"󰿃"}.mdi-lifebuoy:before{content:"󰡾"}.mdi-light-flood-down:before{content:"󱦇"}.mdi-light-flood-up:before{content:"󱦈"}.mdi-light-recessed:before{content:"󱞛"}.mdi-light-switch:before{content:"󰥾"}.mdi-light-switch-off:before{content:"󱨤"}.mdi-lightbulb:before{content:"󰌵"}.mdi-lightbulb-alert:before{content:"󱧡"}.mdi-lightbulb-alert-outline:before{content:"󱧢"}.mdi-lightbulb-auto:before{content:"󱠀"}.mdi-lightbulb-auto-outline:before{content:"󱠁"}.mdi-lightbulb-cfl:before{content:"󱈈"}.mdi-lightbulb-cfl-off:before{content:"󱈉"}.mdi-lightbulb-cfl-spiral:before{content:"󱉵"}.mdi-lightbulb-cfl-spiral-off:before{content:"󱋃"}.mdi-lightbulb-fluorescent-tube:before{content:"󱠄"}.mdi-lightbulb-fluorescent-tube-outline:before{content:"󱠅"}.mdi-lightbulb-group:before{content:"󱉓"}.mdi-lightbulb-group-off:before{content:"󱋍"}.mdi-lightbulb-group-off-outline:before{content:"󱋎"}.mdi-lightbulb-group-outline:before{content:"󱉔"}.mdi-lightbulb-multiple:before{content:"󱉕"}.mdi-lightbulb-multiple-off:before{content:"󱋏"}.mdi-lightbulb-multiple-off-outline:before{content:"󱋐"}.mdi-lightbulb-multiple-outline:before{content:"󱉖"}.mdi-lightbulb-night:before{content:"󱩌"}.mdi-lightbulb-night-outline:before{content:"󱩍"}.mdi-lightbulb-off:before{content:"󰹏"}.mdi-lightbulb-off-outline:before{content:"󰹐"}.mdi-lightbulb-on:before{content:"󰛨"}.mdi-lightbulb-on-10:before{content:"󱩎"}.mdi-lightbulb-on-20:before{content:"󱩏"}.mdi-lightbulb-on-30:before{content:"󱩐"}.mdi-lightbulb-on-40:before{content:"󱩑"}.mdi-lightbulb-on-50:before{content:"󱩒"}.mdi-lightbulb-on-60:before{content:"󱩓"}.mdi-lightbulb-on-70:before{content:"󱩔"}.mdi-lightbulb-on-80:before{content:"󱩕"}.mdi-lightbulb-on-90:before{content:"󱩖"}.mdi-lightbulb-on-outline:before{content:"󰛩"}.mdi-lightbulb-outline:before{content:"󰌶"}.mdi-lightbulb-question:before{content:"󱧣"}.mdi-lightbulb-question-outline:before{content:"󱧤"}.mdi-lightbulb-spot:before{content:"󱟴"}.mdi-lightbulb-spot-off:before{content:"󱟵"}.mdi-lightbulb-variant:before{content:"󱠂"}.mdi-lightbulb-variant-outline:before{content:"󱠃"}.mdi-lighthouse:before{content:"󰧿"}.mdi-lighthouse-on:before{content:"󰨀"}.mdi-lightning-bolt:before{content:"󱐋"}.mdi-lightning-bolt-circle:before{content:"󰠠"}.mdi-lightning-bolt-outline:before{content:"󱐌"}.mdi-line-scan:before{content:"󰘤"}.mdi-lingerie:before{content:"󱑶"}.mdi-link:before{content:"󰌷"}.mdi-link-box:before{content:"󰴚"}.mdi-link-box-outline:before{content:"󰴛"}.mdi-link-box-variant:before{content:"󰴜"}.mdi-link-box-variant-outline:before{content:"󰴝"}.mdi-link-lock:before{content:"󱂺"}.mdi-link-off:before{content:"󰌸"}.mdi-link-plus:before{content:"󰲔"}.mdi-link-variant:before{content:"󰌹"}.mdi-link-variant-minus:before{content:"󱃿"}.mdi-link-variant-off:before{content:"󰌺"}.mdi-link-variant-plus:before{content:"󱄀"}.mdi-link-variant-remove:before{content:"󱄁"}.mdi-linkedin:before{content:"󰌻"}.mdi-linux:before{content:"󰌽"}.mdi-linux-mint:before{content:"󰣭"}.mdi-lipstick:before{content:"󱎵"}.mdi-liquid-spot:before{content:"󱠦"}.mdi-liquor:before{content:"󱤞"}.mdi-list-box:before{content:"󱭻"}.mdi-list-box-outline:before{content:"󱭼"}.mdi-list-status:before{content:"󱖫"}.mdi-litecoin:before{content:"󰩡"}.mdi-loading:before{content:"󰝲"}.mdi-location-enter:before{content:"󰿄"}.mdi-location-exit:before{content:"󰿅"}.mdi-lock:before{content:"󰌾"}.mdi-lock-alert:before{content:"󰣮"}.mdi-lock-alert-outline:before{content:"󱗑"}.mdi-lock-check:before{content:"󱎚"}.mdi-lock-check-outline:before{content:"󱚨"}.mdi-lock-clock:before{content:"󰥿"}.mdi-lock-minus:before{content:"󱚩"}.mdi-lock-minus-outline:before{content:"󱚪"}.mdi-lock-off:before{content:"󱙱"}.mdi-lock-off-outline:before{content:"󱙲"}.mdi-lock-open:before{content:"󰌿"}.mdi-lock-open-alert:before{content:"󱎛"}.mdi-lock-open-alert-outline:before{content:"󱗒"}.mdi-lock-open-check:before{content:"󱎜"}.mdi-lock-open-check-outline:before{content:"󱚫"}.mdi-lock-open-minus:before{content:"󱚬"}.mdi-lock-open-minus-outline:before{content:"󱚭"}.mdi-lock-open-outline:before{content:"󰍀"}.mdi-lock-open-plus:before{content:"󱚮"}.mdi-lock-open-plus-outline:before{content:"󱚯"}.mdi-lock-open-remove:before{content:"󱚰"}.mdi-lock-open-remove-outline:before{content:"󱚱"}.mdi-lock-open-variant:before{content:"󰿆"}.mdi-lock-open-variant-outline:before{content:"󰿇"}.mdi-lock-outline:before{content:"󰍁"}.mdi-lock-pattern:before{content:"󰛪"}.mdi-lock-plus:before{content:"󰗻"}.mdi-lock-plus-outline:before{content:"󱚲"}.mdi-lock-question:before{content:"󰣯"}.mdi-lock-remove:before{content:"󱚳"}.mdi-lock-remove-outline:before{content:"󱚴"}.mdi-lock-reset:before{content:"󰝳"}.mdi-lock-smart:before{content:"󰢲"}.mdi-locker:before{content:"󰟗"}.mdi-locker-multiple:before{content:"󰟘"}.mdi-login:before{content:"󰍂"}.mdi-login-variant:before{content:"󰗼"}.mdi-logout:before{content:"󰍃"}.mdi-logout-variant:before{content:"󰗽"}.mdi-longitude:before{content:"󰽚"}.mdi-looks:before{content:"󰍄"}.mdi-lotion:before{content:"󱖂"}.mdi-lotion-outline:before{content:"󱖃"}.mdi-lotion-plus:before{content:"󱖄"}.mdi-lotion-plus-outline:before{content:"󱖅"}.mdi-loupe:before{content:"󰍅"}.mdi-lumx:before{content:"󰍆"}.mdi-lungs:before{content:"󱂄"}.mdi-mace:before{content:"󱡃"}.mdi-magazine-pistol:before{content:"󰌤"}.mdi-magazine-rifle:before{content:"󰌣"}.mdi-magic-staff:before{content:"󱡄"}.mdi-magnet:before{content:"󰍇"}.mdi-magnet-on:before{content:"󰍈"}.mdi-magnify:before{content:"󰍉"}.mdi-magnify-close:before{content:"󰦀"}.mdi-magnify-expand:before{content:"󱡴"}.mdi-magnify-minus:before{content:"󰍊"}.mdi-magnify-minus-cursor:before{content:"󰩢"}.mdi-magnify-minus-outline:before{content:"󰛬"}.mdi-magnify-plus:before{content:"󰍋"}.mdi-magnify-plus-cursor:before{content:"󰩣"}.mdi-magnify-plus-outline:before{content:"󰛭"}.mdi-magnify-remove-cursor:before{content:"󱈌"}.mdi-magnify-remove-outline:before{content:"󱈍"}.mdi-magnify-scan:before{content:"󱉶"}.mdi-mail:before{content:"󰺻"}.mdi-mailbox:before{content:"󰛮"}.mdi-mailbox-open:before{content:"󰶈"}.mdi-mailbox-open-outline:before{content:"󰶉"}.mdi-mailbox-open-up:before{content:"󰶊"}.mdi-mailbox-open-up-outline:before{content:"󰶋"}.mdi-mailbox-outline:before{content:"󰶌"}.mdi-mailbox-up:before{content:"󰶍"}.mdi-mailbox-up-outline:before{content:"󰶎"}.mdi-manjaro:before{content:"󱘊"}.mdi-map:before{content:"󰍍"}.mdi-map-check:before{content:"󰺼"}.mdi-map-check-outline:before{content:"󰺽"}.mdi-map-clock:before{content:"󰴞"}.mdi-map-clock-outline:before{content:"󰴟"}.mdi-map-legend:before{content:"󰨁"}.mdi-map-marker:before{content:"󰍎"}.mdi-map-marker-account:before{content:"󱣣"}.mdi-map-marker-account-outline:before{content:"󱣤"}.mdi-map-marker-alert:before{content:"󰼅"}.mdi-map-marker-alert-outline:before{content:"󰼆"}.mdi-map-marker-check:before{content:"󰲕"}.mdi-map-marker-check-outline:before{content:"󱋻"}.mdi-map-marker-circle:before{content:"󰍏"}.mdi-map-marker-distance:before{content:"󰣰"}.mdi-map-marker-down:before{content:"󱄂"}.mdi-map-marker-left:before{content:"󱋛"}.mdi-map-marker-left-outline:before{content:"󱋝"}.mdi-map-marker-minus:before{content:"󰙐"}.mdi-map-marker-minus-outline:before{content:"󱋹"}.mdi-map-marker-multiple:before{content:"󰍐"}.mdi-map-marker-multiple-outline:before{content:"󱉷"}.mdi-map-marker-off:before{content:"󰍑"}.mdi-map-marker-off-outline:before{content:"󱋽"}.mdi-map-marker-outline:before{content:"󰟙"}.mdi-map-marker-path:before{content:"󰴠"}.mdi-map-marker-plus:before{content:"󰙑"}.mdi-map-marker-plus-outline:before{content:"󱋸"}.mdi-map-marker-question:before{content:"󰼇"}.mdi-map-marker-question-outline:before{content:"󰼈"}.mdi-map-marker-radius:before{content:"󰍒"}.mdi-map-marker-radius-outline:before{content:"󱋼"}.mdi-map-marker-remove:before{content:"󰼉"}.mdi-map-marker-remove-outline:before{content:"󱋺"}.mdi-map-marker-remove-variant:before{content:"󰼊"}.mdi-map-marker-right:before{content:"󱋜"}.mdi-map-marker-right-outline:before{content:"󱋞"}.mdi-map-marker-star:before{content:"󱘈"}.mdi-map-marker-star-outline:before{content:"󱘉"}.mdi-map-marker-up:before{content:"󱄃"}.mdi-map-minus:before{content:"󰦁"}.mdi-map-outline:before{content:"󰦂"}.mdi-map-plus:before{content:"󰦃"}.mdi-map-search:before{content:"󰦄"}.mdi-map-search-outline:before{content:"󰦅"}.mdi-mapbox:before{content:"󰮪"}.mdi-margin:before{content:"󰍓"}.mdi-marker:before{content:"󰙒"}.mdi-marker-cancel:before{content:"󰷙"}.mdi-marker-check:before{content:"󰍕"}.mdi-mastodon:before{content:"󰫑"}.mdi-material-design:before{content:"󰦆"}.mdi-material-ui:before{content:"󰍗"}.mdi-math-compass:before{content:"󰍘"}.mdi-math-cos:before{content:"󰲖"}.mdi-math-integral:before{content:"󰿈"}.mdi-math-integral-box:before{content:"󰿉"}.mdi-math-log:before{content:"󱂅"}.mdi-math-norm:before{content:"󰿊"}.mdi-math-norm-box:before{content:"󰿋"}.mdi-math-sin:before{content:"󰲗"}.mdi-math-tan:before{content:"󰲘"}.mdi-matrix:before{content:"󰘨"}.mdi-medal:before{content:"󰦇"}.mdi-medal-outline:before{content:"󱌦"}.mdi-medical-bag:before{content:"󰛯"}.mdi-medical-cotton-swab:before{content:"󱪸"}.mdi-medication:before{content:"󱬔"}.mdi-medication-outline:before{content:"󱬕"}.mdi-meditation:before{content:"󱅻"}.mdi-memory:before{content:"󰍛"}.mdi-menorah:before{content:"󱟔"}.mdi-menorah-fire:before{content:"󱟕"}.mdi-menu:before{content:"󰍜"}.mdi-menu-down:before{content:"󰍝"}.mdi-menu-down-outline:before{content:"󰚶"}.mdi-menu-left:before{content:"󰍞"}.mdi-menu-left-outline:before{content:"󰨂"}.mdi-menu-open:before{content:"󰮫"}.mdi-menu-right:before{content:"󰍟"}.mdi-menu-right-outline:before{content:"󰨃"}.mdi-menu-swap:before{content:"󰩤"}.mdi-menu-swap-outline:before{content:"󰩥"}.mdi-menu-up:before{content:"󰍠"}.mdi-menu-up-outline:before{content:"󰚷"}.mdi-merge:before{content:"󰽜"}.mdi-message:before{content:"󰍡"}.mdi-message-alert:before{content:"󰍢"}.mdi-message-alert-outline:before{content:"󰨄"}.mdi-message-arrow-left:before{content:"󱋲"}.mdi-message-arrow-left-outline:before{content:"󱋳"}.mdi-message-arrow-right:before{content:"󱋴"}.mdi-message-arrow-right-outline:before{content:"󱋵"}.mdi-message-badge:before{content:"󱥁"}.mdi-message-badge-outline:before{content:"󱥂"}.mdi-message-bookmark:before{content:"󱖬"}.mdi-message-bookmark-outline:before{content:"󱖭"}.mdi-message-bulleted:before{content:"󰚢"}.mdi-message-bulleted-off:before{content:"󰚣"}.mdi-message-check:before{content:"󱮊"}.mdi-message-check-outline:before{content:"󱮋"}.mdi-message-cog:before{content:"󰛱"}.mdi-message-cog-outline:before{content:"󱅲"}.mdi-message-draw:before{content:"󰍣"}.mdi-message-fast:before{content:"󱧌"}.mdi-message-fast-outline:before{content:"󱧍"}.mdi-message-flash:before{content:"󱖩"}.mdi-message-flash-outline:before{content:"󱖪"}.mdi-message-image:before{content:"󰍤"}.mdi-message-image-outline:before{content:"󱅬"}.mdi-message-lock:before{content:"󰿌"}.mdi-message-lock-outline:before{content:"󱅭"}.mdi-message-minus:before{content:"󱅮"}.mdi-message-minus-outline:before{content:"󱅯"}.mdi-message-off:before{content:"󱙍"}.mdi-message-off-outline:before{content:"󱙎"}.mdi-message-outline:before{content:"󰍥"}.mdi-message-plus:before{content:"󰙓"}.mdi-message-plus-outline:before{content:"󱂻"}.mdi-message-processing:before{content:"󰍦"}.mdi-message-processing-outline:before{content:"󱅰"}.mdi-message-question:before{content:"󱜺"}.mdi-message-question-outline:before{content:"󱜻"}.mdi-message-reply:before{content:"󰍧"}.mdi-message-reply-outline:before{content:"󱜽"}.mdi-message-reply-text:before{content:"󰍨"}.mdi-message-reply-text-outline:before{content:"󱜾"}.mdi-message-settings:before{content:"󰛰"}.mdi-message-settings-outline:before{content:"󱅱"}.mdi-message-star:before{content:"󰚚"}.mdi-message-star-outline:before{content:"󱉐"}.mdi-message-text:before{content:"󰍩"}.mdi-message-text-clock:before{content:"󱅳"}.mdi-message-text-clock-outline:before{content:"󱅴"}.mdi-message-text-fast:before{content:"󱧎"}.mdi-message-text-fast-outline:before{content:"󱧏"}.mdi-message-text-lock:before{content:"󰿍"}.mdi-message-text-lock-outline:before{content:"󱅵"}.mdi-message-text-outline:before{content:"󰍪"}.mdi-message-video:before{content:"󰍫"}.mdi-meteor:before{content:"󰘩"}.mdi-meter-electric:before{content:"󱩗"}.mdi-meter-electric-outline:before{content:"󱩘"}.mdi-meter-gas:before{content:"󱩙"}.mdi-meter-gas-outline:before{content:"󱩚"}.mdi-metronome:before{content:"󰟚"}.mdi-metronome-tick:before{content:"󰟛"}.mdi-micro-sd:before{content:"󰟜"}.mdi-microphone:before{content:"󰍬"}.mdi-microphone-message:before{content:"󰔊"}.mdi-microphone-message-off:before{content:"󰔋"}.mdi-microphone-minus:before{content:"󰢳"}.mdi-microphone-off:before{content:"󰍭"}.mdi-microphone-outline:before{content:"󰍮"}.mdi-microphone-plus:before{content:"󰢴"}.mdi-microphone-question:before{content:"󱦉"}.mdi-microphone-question-outline:before{content:"󱦊"}.mdi-microphone-settings:before{content:"󰍯"}.mdi-microphone-variant:before{content:"󰍰"}.mdi-microphone-variant-off:before{content:"󰍱"}.mdi-microscope:before{content:"󰙔"}.mdi-microsoft:before{content:"󰍲"}.mdi-microsoft-access:before{content:"󱎎"}.mdi-microsoft-azure:before{content:"󰠅"}.mdi-microsoft-azure-devops:before{content:"󰿕"}.mdi-microsoft-bing:before{content:"󰂤"}.mdi-microsoft-dynamics-365:before{content:"󰦈"}.mdi-microsoft-edge:before{content:"󰇩"}.mdi-microsoft-excel:before{content:"󱎏"}.mdi-microsoft-internet-explorer:before{content:"󰌀"}.mdi-microsoft-office:before{content:"󰏆"}.mdi-microsoft-onedrive:before{content:"󰏊"}.mdi-microsoft-onenote:before{content:"󰝇"}.mdi-microsoft-outlook:before{content:"󰴢"}.mdi-microsoft-powerpoint:before{content:"󱎐"}.mdi-microsoft-sharepoint:before{content:"󱎑"}.mdi-microsoft-teams:before{content:"󰊻"}.mdi-microsoft-visual-studio:before{content:"󰘐"}.mdi-microsoft-visual-studio-code:before{content:"󰨞"}.mdi-microsoft-windows:before{content:"󰖳"}.mdi-microsoft-windows-classic:before{content:"󰨡"}.mdi-microsoft-word:before{content:"󱎒"}.mdi-microsoft-xbox:before{content:"󰖹"}.mdi-microsoft-xbox-controller:before{content:"󰖺"}.mdi-microsoft-xbox-controller-battery-alert:before{content:"󰝋"}.mdi-microsoft-xbox-controller-battery-charging:before{content:"󰨢"}.mdi-microsoft-xbox-controller-battery-empty:before{content:"󰝌"}.mdi-microsoft-xbox-controller-battery-full:before{content:"󰝍"}.mdi-microsoft-xbox-controller-battery-low:before{content:"󰝎"}.mdi-microsoft-xbox-controller-battery-medium:before{content:"󰝏"}.mdi-microsoft-xbox-controller-battery-unknown:before{content:"󰝐"}.mdi-microsoft-xbox-controller-menu:before{content:"󰹯"}.mdi-microsoft-xbox-controller-off:before{content:"󰖻"}.mdi-microsoft-xbox-controller-view:before{content:"󰹰"}.mdi-microwave:before{content:"󰲙"}.mdi-microwave-off:before{content:"󱐣"}.mdi-middleware:before{content:"󰽝"}.mdi-middleware-outline:before{content:"󰽞"}.mdi-midi:before{content:"󰣱"}.mdi-midi-port:before{content:"󰣲"}.mdi-mine:before{content:"󰷚"}.mdi-minecraft:before{content:"󰍳"}.mdi-mini-sd:before{content:"󰨅"}.mdi-minidisc:before{content:"󰨆"}.mdi-minus:before{content:"󰍴"}.mdi-minus-box:before{content:"󰍵"}.mdi-minus-box-multiple:before{content:"󱅁"}.mdi-minus-box-multiple-outline:before{content:"󱅂"}.mdi-minus-box-outline:before{content:"󰛲"}.mdi-minus-circle:before{content:"󰍶"}.mdi-minus-circle-multiple:before{content:"󰍚"}.mdi-minus-circle-multiple-outline:before{content:"󰫓"}.mdi-minus-circle-off:before{content:"󱑙"}.mdi-minus-circle-off-outline:before{content:"󱑚"}.mdi-minus-circle-outline:before{content:"󰍷"}.mdi-minus-network:before{content:"󰍸"}.mdi-minus-network-outline:before{content:"󰲚"}.mdi-minus-thick:before{content:"󱘹"}.mdi-mirror:before{content:"󱇽"}.mdi-mirror-rectangle:before{content:"󱞟"}.mdi-mirror-variant:before{content:"󱞠"}.mdi-mixed-martial-arts:before{content:"󰶏"}.mdi-mixed-reality:before{content:"󰡿"}.mdi-molecule:before{content:"󰮬"}.mdi-molecule-co:before{content:"󱋾"}.mdi-molecule-co2:before{content:"󰟤"}.mdi-monitor:before{content:"󰍹"}.mdi-monitor-account:before{content:"󱩛"}.mdi-monitor-arrow-down:before{content:"󱧐"}.mdi-monitor-arrow-down-variant:before{content:"󱧑"}.mdi-monitor-cellphone:before{content:"󰦉"}.mdi-monitor-cellphone-star:before{content:"󰦊"}.mdi-monitor-dashboard:before{content:"󰨇"}.mdi-monitor-edit:before{content:"󱋆"}.mdi-monitor-eye:before{content:"󱎴"}.mdi-monitor-lock:before{content:"󰷛"}.mdi-monitor-multiple:before{content:"󰍺"}.mdi-monitor-off:before{content:"󰶐"}.mdi-monitor-screenshot:before{content:"󰹑"}.mdi-monitor-share:before{content:"󱒃"}.mdi-monitor-shimmer:before{content:"󱄄"}.mdi-monitor-small:before{content:"󱡶"}.mdi-monitor-speaker:before{content:"󰽟"}.mdi-monitor-speaker-off:before{content:"󰽠"}.mdi-monitor-star:before{content:"󰷜"}.mdi-moon-first-quarter:before{content:"󰽡"}.mdi-moon-full:before{content:"󰽢"}.mdi-moon-last-quarter:before{content:"󰽣"}.mdi-moon-new:before{content:"󰽤"}.mdi-moon-waning-crescent:before{content:"󰽥"}.mdi-moon-waning-gibbous:before{content:"󰽦"}.mdi-moon-waxing-crescent:before{content:"󰽧"}.mdi-moon-waxing-gibbous:before{content:"󰽨"}.mdi-moped:before{content:"󱂆"}.mdi-moped-electric:before{content:"󱖷"}.mdi-moped-electric-outline:before{content:"󱖸"}.mdi-moped-outline:before{content:"󱖹"}.mdi-more:before{content:"󰍻"}.mdi-mortar-pestle:before{content:"󱝈"}.mdi-mortar-pestle-plus:before{content:"󰏱"}.mdi-mosque:before{content:"󰵅"}.mdi-mosque-outline:before{content:"󱠧"}.mdi-mother-heart:before{content:"󱌔"}.mdi-mother-nurse:before{content:"󰴡"}.mdi-motion:before{content:"󱖲"}.mdi-motion-outline:before{content:"󱖳"}.mdi-motion-pause:before{content:"󱖐"}.mdi-motion-pause-outline:before{content:"󱖒"}.mdi-motion-play:before{content:"󱖏"}.mdi-motion-play-outline:before{content:"󱖑"}.mdi-motion-sensor:before{content:"󰶑"}.mdi-motion-sensor-off:before{content:"󱐵"}.mdi-motorbike:before{content:"󰍼"}.mdi-motorbike-electric:before{content:"󱖺"}.mdi-motorbike-off:before{content:"󱬖"}.mdi-mouse:before{content:"󰍽"}.mdi-mouse-bluetooth:before{content:"󰦋"}.mdi-mouse-move-down:before{content:"󱕐"}.mdi-mouse-move-up:before{content:"󱕑"}.mdi-mouse-move-vertical:before{content:"󱕒"}.mdi-mouse-off:before{content:"󰍾"}.mdi-mouse-variant:before{content:"󰍿"}.mdi-mouse-variant-off:before{content:"󰎀"}.mdi-move-resize:before{content:"󰙕"}.mdi-move-resize-variant:before{content:"󰙖"}.mdi-movie:before{content:"󰎁"}.mdi-movie-check:before{content:"󱛳"}.mdi-movie-check-outline:before{content:"󱛴"}.mdi-movie-cog:before{content:"󱛵"}.mdi-movie-cog-outline:before{content:"󱛶"}.mdi-movie-edit:before{content:"󱄢"}.mdi-movie-edit-outline:before{content:"󱄣"}.mdi-movie-filter:before{content:"󱄤"}.mdi-movie-filter-outline:before{content:"󱄥"}.mdi-movie-minus:before{content:"󱛷"}.mdi-movie-minus-outline:before{content:"󱛸"}.mdi-movie-off:before{content:"󱛹"}.mdi-movie-off-outline:before{content:"󱛺"}.mdi-movie-open:before{content:"󰿎"}.mdi-movie-open-check:before{content:"󱛻"}.mdi-movie-open-check-outline:before{content:"󱛼"}.mdi-movie-open-cog:before{content:"󱛽"}.mdi-movie-open-cog-outline:before{content:"󱛾"}.mdi-movie-open-edit:before{content:"󱛿"}.mdi-movie-open-edit-outline:before{content:"󱜀"}.mdi-movie-open-minus:before{content:"󱜁"}.mdi-movie-open-minus-outline:before{content:"󱜂"}.mdi-movie-open-off:before{content:"󱜃"}.mdi-movie-open-off-outline:before{content:"󱜄"}.mdi-movie-open-outline:before{content:"󰿏"}.mdi-movie-open-play:before{content:"󱜅"}.mdi-movie-open-play-outline:before{content:"󱜆"}.mdi-movie-open-plus:before{content:"󱜇"}.mdi-movie-open-plus-outline:before{content:"󱜈"}.mdi-movie-open-remove:before{content:"󱜉"}.mdi-movie-open-remove-outline:before{content:"󱜊"}.mdi-movie-open-settings:before{content:"󱜋"}.mdi-movie-open-settings-outline:before{content:"󱜌"}.mdi-movie-open-star:before{content:"󱜍"}.mdi-movie-open-star-outline:before{content:"󱜎"}.mdi-movie-outline:before{content:"󰷝"}.mdi-movie-play:before{content:"󱜏"}.mdi-movie-play-outline:before{content:"󱜐"}.mdi-movie-plus:before{content:"󱜑"}.mdi-movie-plus-outline:before{content:"󱜒"}.mdi-movie-remove:before{content:"󱜓"}.mdi-movie-remove-outline:before{content:"󱜔"}.mdi-movie-roll:before{content:"󰟞"}.mdi-movie-search:before{content:"󱇒"}.mdi-movie-search-outline:before{content:"󱇓"}.mdi-movie-settings:before{content:"󱜕"}.mdi-movie-settings-outline:before{content:"󱜖"}.mdi-movie-star:before{content:"󱜗"}.mdi-movie-star-outline:before{content:"󱜘"}.mdi-mower:before{content:"󱙯"}.mdi-mower-bag:before{content:"󱙰"}.mdi-mower-bag-on:before{content:"󱭠"}.mdi-mower-on:before{content:"󱭟"}.mdi-muffin:before{content:"󰦌"}.mdi-multicast:before{content:"󱢓"}.mdi-multimedia:before{content:"󱮗"}.mdi-multiplication:before{content:"󰎂"}.mdi-multiplication-box:before{content:"󰎃"}.mdi-mushroom:before{content:"󰟟"}.mdi-mushroom-off:before{content:"󱏺"}.mdi-mushroom-off-outline:before{content:"󱏻"}.mdi-mushroom-outline:before{content:"󰟠"}.mdi-music:before{content:"󰝚"}.mdi-music-accidental-double-flat:before{content:"󰽩"}.mdi-music-accidental-double-sharp:before{content:"󰽪"}.mdi-music-accidental-flat:before{content:"󰽫"}.mdi-music-accidental-natural:before{content:"󰽬"}.mdi-music-accidental-sharp:before{content:"󰽭"}.mdi-music-box:before{content:"󰎄"}.mdi-music-box-multiple:before{content:"󰌳"}.mdi-music-box-multiple-outline:before{content:"󰼄"}.mdi-music-box-outline:before{content:"󰎅"}.mdi-music-circle:before{content:"󰎆"}.mdi-music-circle-outline:before{content:"󰫔"}.mdi-music-clef-alto:before{content:"󰽮"}.mdi-music-clef-bass:before{content:"󰽯"}.mdi-music-clef-treble:before{content:"󰽰"}.mdi-music-note:before{content:"󰎇"}.mdi-music-note-bluetooth:before{content:"󰗾"}.mdi-music-note-bluetooth-off:before{content:"󰗿"}.mdi-music-note-eighth:before{content:"󰎈"}.mdi-music-note-eighth-dotted:before{content:"󰽱"}.mdi-music-note-half:before{content:"󰎉"}.mdi-music-note-half-dotted:before{content:"󰽲"}.mdi-music-note-minus:before{content:"󱮉"}.mdi-music-note-off:before{content:"󰎊"}.mdi-music-note-off-outline:before{content:"󰽳"}.mdi-music-note-outline:before{content:"󰽴"}.mdi-music-note-plus:before{content:"󰷞"}.mdi-music-note-quarter:before{content:"󰎋"}.mdi-music-note-quarter-dotted:before{content:"󰽵"}.mdi-music-note-sixteenth:before{content:"󰎌"}.mdi-music-note-sixteenth-dotted:before{content:"󰽶"}.mdi-music-note-whole:before{content:"󰎍"}.mdi-music-note-whole-dotted:before{content:"󰽷"}.mdi-music-off:before{content:"󰝛"}.mdi-music-rest-eighth:before{content:"󰽸"}.mdi-music-rest-half:before{content:"󰽹"}.mdi-music-rest-quarter:before{content:"󰽺"}.mdi-music-rest-sixteenth:before{content:"󰽻"}.mdi-music-rest-whole:before{content:"󰽼"}.mdi-mustache:before{content:"󱗞"}.mdi-nail:before{content:"󰷟"}.mdi-nas:before{content:"󰣳"}.mdi-nativescript:before{content:"󰢀"}.mdi-nature:before{content:"󰎎"}.mdi-nature-people:before{content:"󰎏"}.mdi-navigation:before{content:"󰎐"}.mdi-navigation-outline:before{content:"󱘇"}.mdi-navigation-variant:before{content:"󱣰"}.mdi-navigation-variant-outline:before{content:"󱣱"}.mdi-near-me:before{content:"󰗍"}.mdi-necklace:before{content:"󰼋"}.mdi-needle:before{content:"󰎑"}.mdi-needle-off:before{content:"󱧒"}.mdi-netflix:before{content:"󰝆"}.mdi-network:before{content:"󰛳"}.mdi-network-off:before{content:"󰲛"}.mdi-network-off-outline:before{content:"󰲜"}.mdi-network-outline:before{content:"󰲝"}.mdi-network-pos:before{content:"󱫋"}.mdi-network-strength-1:before{content:"󰣴"}.mdi-network-strength-1-alert:before{content:"󰣵"}.mdi-network-strength-2:before{content:"󰣶"}.mdi-network-strength-2-alert:before{content:"󰣷"}.mdi-network-strength-3:before{content:"󰣸"}.mdi-network-strength-3-alert:before{content:"󰣹"}.mdi-network-strength-4:before{content:"󰣺"}.mdi-network-strength-4-alert:before{content:"󰣻"}.mdi-network-strength-4-cog:before{content:"󱤚"}.mdi-network-strength-off:before{content:"󰣼"}.mdi-network-strength-off-outline:before{content:"󰣽"}.mdi-network-strength-outline:before{content:"󰣾"}.mdi-new-box:before{content:"󰎔"}.mdi-newspaper:before{content:"󰎕"}.mdi-newspaper-check:before{content:"󱥃"}.mdi-newspaper-minus:before{content:"󰼌"}.mdi-newspaper-plus:before{content:"󰼍"}.mdi-newspaper-remove:before{content:"󱥄"}.mdi-newspaper-variant:before{content:"󱀁"}.mdi-newspaper-variant-multiple:before{content:"󱀂"}.mdi-newspaper-variant-multiple-outline:before{content:"󱀃"}.mdi-newspaper-variant-outline:before{content:"󱀄"}.mdi-nfc:before{content:"󰎖"}.mdi-nfc-search-variant:before{content:"󰹓"}.mdi-nfc-tap:before{content:"󰎗"}.mdi-nfc-variant:before{content:"󰎘"}.mdi-nfc-variant-off:before{content:"󰹔"}.mdi-ninja:before{content:"󰝴"}.mdi-nintendo-game-boy:before{content:"󱎓"}.mdi-nintendo-switch:before{content:"󰟡"}.mdi-nintendo-wii:before{content:"󰖫"}.mdi-nintendo-wiiu:before{content:"󰜭"}.mdi-nix:before{content:"󱄅"}.mdi-nodejs:before{content:"󰎙"}.mdi-noodles:before{content:"󱅾"}.mdi-not-equal:before{content:"󰦍"}.mdi-not-equal-variant:before{content:"󰦎"}.mdi-note:before{content:"󰎚"}.mdi-note-alert:before{content:"󱝽"}.mdi-note-alert-outline:before{content:"󱝾"}.mdi-note-check:before{content:"󱝿"}.mdi-note-check-outline:before{content:"󱞀"}.mdi-note-edit:before{content:"󱞁"}.mdi-note-edit-outline:before{content:"󱞂"}.mdi-note-minus:before{content:"󱙏"}.mdi-note-minus-outline:before{content:"󱙐"}.mdi-note-multiple:before{content:"󰚸"}.mdi-note-multiple-outline:before{content:"󰚹"}.mdi-note-off:before{content:"󱞃"}.mdi-note-off-outline:before{content:"󱞄"}.mdi-note-outline:before{content:"󰎛"}.mdi-note-plus:before{content:"󰎜"}.mdi-note-plus-outline:before{content:"󰎝"}.mdi-note-remove:before{content:"󱙑"}.mdi-note-remove-outline:before{content:"󱙒"}.mdi-note-search:before{content:"󱙓"}.mdi-note-search-outline:before{content:"󱙔"}.mdi-note-text:before{content:"󰎞"}.mdi-note-text-outline:before{content:"󱇗"}.mdi-notebook:before{content:"󰠮"}.mdi-notebook-check:before{content:"󱓵"}.mdi-notebook-check-outline:before{content:"󱓶"}.mdi-notebook-edit:before{content:"󱓧"}.mdi-notebook-edit-outline:before{content:"󱓩"}.mdi-notebook-heart:before{content:"󱨋"}.mdi-notebook-heart-outline:before{content:"󱨌"}.mdi-notebook-minus:before{content:"󱘐"}.mdi-notebook-minus-outline:before{content:"󱘑"}.mdi-notebook-multiple:before{content:"󰹕"}.mdi-notebook-outline:before{content:"󰺿"}.mdi-notebook-plus:before{content:"󱘒"}.mdi-notebook-plus-outline:before{content:"󱘓"}.mdi-notebook-remove:before{content:"󱘔"}.mdi-notebook-remove-outline:before{content:"󱘕"}.mdi-notification-clear-all:before{content:"󰎟"}.mdi-npm:before{content:"󰛷"}.mdi-nuke:before{content:"󰚤"}.mdi-null:before{content:"󰟢"}.mdi-numeric:before{content:"󰎠"}.mdi-numeric-0:before{content:"󰬹"}.mdi-numeric-0-box:before{content:"󰎡"}.mdi-numeric-0-box-multiple:before{content:"󰼎"}.mdi-numeric-0-box-multiple-outline:before{content:"󰎢"}.mdi-numeric-0-box-outline:before{content:"󰎣"}.mdi-numeric-0-circle:before{content:"󰲞"}.mdi-numeric-0-circle-outline:before{content:"󰲟"}.mdi-numeric-1:before{content:"󰬺"}.mdi-numeric-1-box:before{content:"󰎤"}.mdi-numeric-1-box-multiple:before{content:"󰼏"}.mdi-numeric-1-box-multiple-outline:before{content:"󰎥"}.mdi-numeric-1-box-outline:before{content:"󰎦"}.mdi-numeric-1-circle:before{content:"󰲠"}.mdi-numeric-1-circle-outline:before{content:"󰲡"}.mdi-numeric-10:before{content:"󰿩"}.mdi-numeric-10-box:before{content:"󰽽"}.mdi-numeric-10-box-multiple:before{content:"󰿪"}.mdi-numeric-10-box-multiple-outline:before{content:"󰿫"}.mdi-numeric-10-box-outline:before{content:"󰽾"}.mdi-numeric-10-circle:before{content:"󰿬"}.mdi-numeric-10-circle-outline:before{content:"󰿭"}.mdi-numeric-2:before{content:"󰬻"}.mdi-numeric-2-box:before{content:"󰎧"}.mdi-numeric-2-box-multiple:before{content:"󰼐"}.mdi-numeric-2-box-multiple-outline:before{content:"󰎨"}.mdi-numeric-2-box-outline:before{content:"󰎩"}.mdi-numeric-2-circle:before{content:"󰲢"}.mdi-numeric-2-circle-outline:before{content:"󰲣"}.mdi-numeric-3:before{content:"󰬼"}.mdi-numeric-3-box:before{content:"󰎪"}.mdi-numeric-3-box-multiple:before{content:"󰼑"}.mdi-numeric-3-box-multiple-outline:before{content:"󰎫"}.mdi-numeric-3-box-outline:before{content:"󰎬"}.mdi-numeric-3-circle:before{content:"󰲤"}.mdi-numeric-3-circle-outline:before{content:"󰲥"}.mdi-numeric-4:before{content:"󰬽"}.mdi-numeric-4-box:before{content:"󰎭"}.mdi-numeric-4-box-multiple:before{content:"󰼒"}.mdi-numeric-4-box-multiple-outline:before{content:"󰎲"}.mdi-numeric-4-box-outline:before{content:"󰎮"}.mdi-numeric-4-circle:before{content:"󰲦"}.mdi-numeric-4-circle-outline:before{content:"󰲧"}.mdi-numeric-5:before{content:"󰬾"}.mdi-numeric-5-box:before{content:"󰎱"}.mdi-numeric-5-box-multiple:before{content:"󰼓"}.mdi-numeric-5-box-multiple-outline:before{content:"󰎯"}.mdi-numeric-5-box-outline:before{content:"󰎰"}.mdi-numeric-5-circle:before{content:"󰲨"}.mdi-numeric-5-circle-outline:before{content:"󰲩"}.mdi-numeric-6:before{content:"󰬿"}.mdi-numeric-6-box:before{content:"󰎳"}.mdi-numeric-6-box-multiple:before{content:"󰼔"}.mdi-numeric-6-box-multiple-outline:before{content:"󰎴"}.mdi-numeric-6-box-outline:before{content:"󰎵"}.mdi-numeric-6-circle:before{content:"󰲪"}.mdi-numeric-6-circle-outline:before{content:"󰲫"}.mdi-numeric-7:before{content:"󰭀"}.mdi-numeric-7-box:before{content:"󰎶"}.mdi-numeric-7-box-multiple:before{content:"󰼕"}.mdi-numeric-7-box-multiple-outline:before{content:"󰎷"}.mdi-numeric-7-box-outline:before{content:"󰎸"}.mdi-numeric-7-circle:before{content:"󰲬"}.mdi-numeric-7-circle-outline:before{content:"󰲭"}.mdi-numeric-8:before{content:"󰭁"}.mdi-numeric-8-box:before{content:"󰎹"}.mdi-numeric-8-box-multiple:before{content:"󰼖"}.mdi-numeric-8-box-multiple-outline:before{content:"󰎺"}.mdi-numeric-8-box-outline:before{content:"󰎻"}.mdi-numeric-8-circle:before{content:"󰲮"}.mdi-numeric-8-circle-outline:before{content:"󰲯"}.mdi-numeric-9:before{content:"󰭂"}.mdi-numeric-9-box:before{content:"󰎼"}.mdi-numeric-9-box-multiple:before{content:"󰼗"}.mdi-numeric-9-box-multiple-outline:before{content:"󰎽"}.mdi-numeric-9-box-outline:before{content:"󰎾"}.mdi-numeric-9-circle:before{content:"󰲰"}.mdi-numeric-9-circle-outline:before{content:"󰲱"}.mdi-numeric-9-plus:before{content:"󰿮"}.mdi-numeric-9-plus-box:before{content:"󰎿"}.mdi-numeric-9-plus-box-multiple:before{content:"󰼘"}.mdi-numeric-9-plus-box-multiple-outline:before{content:"󰏀"}.mdi-numeric-9-plus-box-outline:before{content:"󰏁"}.mdi-numeric-9-plus-circle:before{content:"󰲲"}.mdi-numeric-9-plus-circle-outline:before{content:"󰲳"}.mdi-numeric-negative-1:before{content:"󱁒"}.mdi-numeric-off:before{content:"󱧓"}.mdi-numeric-positive-1:before{content:"󱗋"}.mdi-nut:before{content:"󰛸"}.mdi-nutrition:before{content:"󰏂"}.mdi-nuxt:before{content:"󱄆"}.mdi-oar:before{content:"󰙼"}.mdi-ocarina:before{content:"󰷠"}.mdi-oci:before{content:"󱋩"}.mdi-ocr:before{content:"󱄺"}.mdi-octagon:before{content:"󰏃"}.mdi-octagon-outline:before{content:"󰏄"}.mdi-octagram:before{content:"󰛹"}.mdi-octagram-outline:before{content:"󰝵"}.mdi-octahedron:before{content:"󱥐"}.mdi-octahedron-off:before{content:"󱥑"}.mdi-odnoklassniki:before{content:"󰏅"}.mdi-offer:before{content:"󱈛"}.mdi-office-building:before{content:"󰦑"}.mdi-office-building-cog:before{content:"󱥉"}.mdi-office-building-cog-outline:before{content:"󱥊"}.mdi-office-building-marker:before{content:"󱔠"}.mdi-office-building-marker-outline:before{content:"󱔡"}.mdi-office-building-minus:before{content:"󱮪"}.mdi-office-building-minus-outline:before{content:"󱮫"}.mdi-office-building-outline:before{content:"󱔟"}.mdi-office-building-plus:before{content:"󱮨"}.mdi-office-building-plus-outline:before{content:"󱮩"}.mdi-office-building-remove:before{content:"󱮬"}.mdi-office-building-remove-outline:before{content:"󱮭"}.mdi-oil:before{content:"󰏇"}.mdi-oil-lamp:before{content:"󰼙"}.mdi-oil-level:before{content:"󱁓"}.mdi-oil-temperature:before{content:"󰿸"}.mdi-om:before{content:"󰥳"}.mdi-omega:before{content:"󰏉"}.mdi-one-up:before{content:"󰮭"}.mdi-onepassword:before{content:"󰢁"}.mdi-opacity:before{content:"󰗌"}.mdi-open-in-app:before{content:"󰏋"}.mdi-open-in-new:before{content:"󰏌"}.mdi-open-source-initiative:before{content:"󰮮"}.mdi-openid:before{content:"󰏍"}.mdi-opera:before{content:"󰏎"}.mdi-orbit:before{content:"󰀘"}.mdi-orbit-variant:before{content:"󱗛"}.mdi-order-alphabetical-ascending:before{content:"󰈍"}.mdi-order-alphabetical-descending:before{content:"󰴇"}.mdi-order-bool-ascending:before{content:"󰊾"}.mdi-order-bool-ascending-variant:before{content:"󰦏"}.mdi-order-bool-descending:before{content:"󱎄"}.mdi-order-bool-descending-variant:before{content:"󰦐"}.mdi-order-numeric-ascending:before{content:"󰕅"}.mdi-order-numeric-descending:before{content:"󰕆"}.mdi-origin:before{content:"󰭃"}.mdi-ornament:before{content:"󰏏"}.mdi-ornament-variant:before{content:"󰏐"}.mdi-outdoor-lamp:before{content:"󱁔"}.mdi-overscan:before{content:"󱀅"}.mdi-owl:before{content:"󰏒"}.mdi-pac-man:before{content:"󰮯"}.mdi-package:before{content:"󰏓"}.mdi-package-check:before{content:"󱭑"}.mdi-package-down:before{content:"󰏔"}.mdi-package-up:before{content:"󰏕"}.mdi-package-variant:before{content:"󰏖"}.mdi-package-variant-closed:before{content:"󰏗"}.mdi-package-variant-closed-check:before{content:"󱭒"}.mdi-package-variant-closed-minus:before{content:"󱧔"}.mdi-package-variant-closed-plus:before{content:"󱧕"}.mdi-package-variant-closed-remove:before{content:"󱧖"}.mdi-package-variant-minus:before{content:"󱧗"}.mdi-package-variant-plus:before{content:"󱧘"}.mdi-package-variant-remove:before{content:"󱧙"}.mdi-page-first:before{content:"󰘀"}.mdi-page-last:before{content:"󰘁"}.mdi-page-layout-body:before{content:"󰛺"}.mdi-page-layout-footer:before{content:"󰛻"}.mdi-page-layout-header:before{content:"󰛼"}.mdi-page-layout-header-footer:before{content:"󰽿"}.mdi-page-layout-sidebar-left:before{content:"󰛽"}.mdi-page-layout-sidebar-right:before{content:"󰛾"}.mdi-page-next:before{content:"󰮰"}.mdi-page-next-outline:before{content:"󰮱"}.mdi-page-previous:before{content:"󰮲"}.mdi-page-previous-outline:before{content:"󰮳"}.mdi-pail:before{content:"󱐗"}.mdi-pail-minus:before{content:"󱐷"}.mdi-pail-minus-outline:before{content:"󱐼"}.mdi-pail-off:before{content:"󱐹"}.mdi-pail-off-outline:before{content:"󱐾"}.mdi-pail-outline:before{content:"󱐺"}.mdi-pail-plus:before{content:"󱐶"}.mdi-pail-plus-outline:before{content:"󱐻"}.mdi-pail-remove:before{content:"󱐸"}.mdi-pail-remove-outline:before{content:"󱐽"}.mdi-palette:before{content:"󰏘"}.mdi-palette-advanced:before{content:"󰏙"}.mdi-palette-outline:before{content:"󰸌"}.mdi-palette-swatch:before{content:"󰢵"}.mdi-palette-swatch-outline:before{content:"󱍜"}.mdi-palette-swatch-variant:before{content:"󱥚"}.mdi-palm-tree:before{content:"󱁕"}.mdi-pan:before{content:"󰮴"}.mdi-pan-bottom-left:before{content:"󰮵"}.mdi-pan-bottom-right:before{content:"󰮶"}.mdi-pan-down:before{content:"󰮷"}.mdi-pan-horizontal:before{content:"󰮸"}.mdi-pan-left:before{content:"󰮹"}.mdi-pan-right:before{content:"󰮺"}.mdi-pan-top-left:before{content:"󰮻"}.mdi-pan-top-right:before{content:"󰮼"}.mdi-pan-up:before{content:"󰮽"}.mdi-pan-vertical:before{content:"󰮾"}.mdi-panda:before{content:"󰏚"}.mdi-pandora:before{content:"󰏛"}.mdi-panorama:before{content:"󰏜"}.mdi-panorama-fisheye:before{content:"󰏝"}.mdi-panorama-horizontal:before{content:"󱤨"}.mdi-panorama-horizontal-outline:before{content:"󰏞"}.mdi-panorama-outline:before{content:"󱦌"}.mdi-panorama-sphere:before{content:"󱦍"}.mdi-panorama-sphere-outline:before{content:"󱦎"}.mdi-panorama-variant:before{content:"󱦏"}.mdi-panorama-variant-outline:before{content:"󱦐"}.mdi-panorama-vertical:before{content:"󱤩"}.mdi-panorama-vertical-outline:before{content:"󰏟"}.mdi-panorama-wide-angle:before{content:"󱥟"}.mdi-panorama-wide-angle-outline:before{content:"󰏠"}.mdi-paper-cut-vertical:before{content:"󰏡"}.mdi-paper-roll:before{content:"󱅗"}.mdi-paper-roll-outline:before{content:"󱅘"}.mdi-paperclip:before{content:"󰏢"}.mdi-paperclip-check:before{content:"󱫆"}.mdi-paperclip-lock:before{content:"󱧚"}.mdi-paperclip-minus:before{content:"󱫇"}.mdi-paperclip-off:before{content:"󱫈"}.mdi-paperclip-plus:before{content:"󱫉"}.mdi-paperclip-remove:before{content:"󱫊"}.mdi-parachute:before{content:"󰲴"}.mdi-parachute-outline:before{content:"󰲵"}.mdi-paragliding:before{content:"󱝅"}.mdi-parking:before{content:"󰏣"}.mdi-party-popper:before{content:"󱁖"}.mdi-passport:before{content:"󰟣"}.mdi-passport-biometric:before{content:"󰷡"}.mdi-pasta:before{content:"󱅠"}.mdi-patio-heater:before{content:"󰾀"}.mdi-patreon:before{content:"󰢂"}.mdi-pause:before{content:"󰏤"}.mdi-pause-box:before{content:"󰂼"}.mdi-pause-box-outline:before{content:"󱭺"}.mdi-pause-circle:before{content:"󰏥"}.mdi-pause-circle-outline:before{content:"󰏦"}.mdi-pause-octagon:before{content:"󰏧"}.mdi-pause-octagon-outline:before{content:"󰏨"}.mdi-paw:before{content:"󰏩"}.mdi-paw-off:before{content:"󰙗"}.mdi-paw-off-outline:before{content:"󱙶"}.mdi-paw-outline:before{content:"󱙵"}.mdi-peace:before{content:"󰢄"}.mdi-peanut:before{content:"󰿼"}.mdi-peanut-off:before{content:"󰿽"}.mdi-peanut-off-outline:before{content:"󰿿"}.mdi-peanut-outline:before{content:"󰿾"}.mdi-pen:before{content:"󰏪"}.mdi-pen-lock:before{content:"󰷢"}.mdi-pen-minus:before{content:"󰷣"}.mdi-pen-off:before{content:"󰷤"}.mdi-pen-plus:before{content:"󰷥"}.mdi-pen-remove:before{content:"󰷦"}.mdi-pencil:before{content:"󰏫"}.mdi-pencil-box:before{content:"󰏬"}.mdi-pencil-box-multiple:before{content:"󱅄"}.mdi-pencil-box-multiple-outline:before{content:"󱅅"}.mdi-pencil-box-outline:before{content:"󰏭"}.mdi-pencil-circle:before{content:"󰛿"}.mdi-pencil-circle-outline:before{content:"󰝶"}.mdi-pencil-lock:before{content:"󰏮"}.mdi-pencil-lock-outline:before{content:"󰷧"}.mdi-pencil-minus:before{content:"󰷨"}.mdi-pencil-minus-outline:before{content:"󰷩"}.mdi-pencil-off:before{content:"󰏯"}.mdi-pencil-off-outline:before{content:"󰷪"}.mdi-pencil-outline:before{content:"󰲶"}.mdi-pencil-plus:before{content:"󰷫"}.mdi-pencil-plus-outline:before{content:"󰷬"}.mdi-pencil-remove:before{content:"󰷭"}.mdi-pencil-remove-outline:before{content:"󰷮"}.mdi-pencil-ruler:before{content:"󱍓"}.mdi-penguin:before{content:"󰻀"}.mdi-pentagon:before{content:"󰜁"}.mdi-pentagon-outline:before{content:"󰜀"}.mdi-pentagram:before{content:"󱙧"}.mdi-percent:before{content:"󰏰"}.mdi-percent-box:before{content:"󱨂"}.mdi-percent-box-outline:before{content:"󱨃"}.mdi-percent-circle:before{content:"󱨄"}.mdi-percent-circle-outline:before{content:"󱨅"}.mdi-percent-outline:before{content:"󱉸"}.mdi-periodic-table:before{content:"󰢶"}.mdi-perspective-less:before{content:"󰴣"}.mdi-perspective-more:before{content:"󰴤"}.mdi-ph:before{content:"󱟅"}.mdi-phone:before{content:"󰏲"}.mdi-phone-alert:before{content:"󰼚"}.mdi-phone-alert-outline:before{content:"󱆎"}.mdi-phone-bluetooth:before{content:"󰏳"}.mdi-phone-bluetooth-outline:before{content:"󱆏"}.mdi-phone-cancel:before{content:"󱂼"}.mdi-phone-cancel-outline:before{content:"󱆐"}.mdi-phone-check:before{content:"󱆩"}.mdi-phone-check-outline:before{content:"󱆪"}.mdi-phone-classic:before{content:"󰘂"}.mdi-phone-classic-off:before{content:"󱉹"}.mdi-phone-clock:before{content:"󱧛"}.mdi-phone-dial:before{content:"󱕙"}.mdi-phone-dial-outline:before{content:"󱕚"}.mdi-phone-forward:before{content:"󰏴"}.mdi-phone-forward-outline:before{content:"󱆑"}.mdi-phone-hangup:before{content:"󰏵"}.mdi-phone-hangup-outline:before{content:"󱆒"}.mdi-phone-in-talk:before{content:"󰏶"}.mdi-phone-in-talk-outline:before{content:"󱆂"}.mdi-phone-incoming:before{content:"󰏷"}.mdi-phone-incoming-outgoing:before{content:"󱬿"}.mdi-phone-incoming-outgoing-outline:before{content:"󱭀"}.mdi-phone-incoming-outline:before{content:"󱆓"}.mdi-phone-lock:before{content:"󰏸"}.mdi-phone-lock-outline:before{content:"󱆔"}.mdi-phone-log:before{content:"󰏹"}.mdi-phone-log-outline:before{content:"󱆕"}.mdi-phone-message:before{content:"󱆖"}.mdi-phone-message-outline:before{content:"󱆗"}.mdi-phone-minus:before{content:"󰙘"}.mdi-phone-minus-outline:before{content:"󱆘"}.mdi-phone-missed:before{content:"󰏺"}.mdi-phone-missed-outline:before{content:"󱆥"}.mdi-phone-off:before{content:"󰷯"}.mdi-phone-off-outline:before{content:"󱆦"}.mdi-phone-outgoing:before{content:"󰏻"}.mdi-phone-outgoing-outline:before{content:"󱆙"}.mdi-phone-outline:before{content:"󰷰"}.mdi-phone-paused:before{content:"󰏼"}.mdi-phone-paused-outline:before{content:"󱆚"}.mdi-phone-plus:before{content:"󰙙"}.mdi-phone-plus-outline:before{content:"󱆛"}.mdi-phone-refresh:before{content:"󱦓"}.mdi-phone-refresh-outline:before{content:"󱦔"}.mdi-phone-remove:before{content:"󱔯"}.mdi-phone-remove-outline:before{content:"󱔰"}.mdi-phone-return:before{content:"󰠯"}.mdi-phone-return-outline:before{content:"󱆜"}.mdi-phone-ring:before{content:"󱆫"}.mdi-phone-ring-outline:before{content:"󱆬"}.mdi-phone-rotate-landscape:before{content:"󰢅"}.mdi-phone-rotate-portrait:before{content:"󰢆"}.mdi-phone-settings:before{content:"󰏽"}.mdi-phone-settings-outline:before{content:"󱆝"}.mdi-phone-sync:before{content:"󱦕"}.mdi-phone-sync-outline:before{content:"󱦖"}.mdi-phone-voip:before{content:"󰏾"}.mdi-pi:before{content:"󰏿"}.mdi-pi-box:before{content:"󰐀"}.mdi-pi-hole:before{content:"󰷱"}.mdi-piano:before{content:"󰙽"}.mdi-piano-off:before{content:"󰚘"}.mdi-pickaxe:before{content:"󰢷"}.mdi-picture-in-picture-bottom-right:before{content:"󰹗"}.mdi-picture-in-picture-bottom-right-outline:before{content:"󰹘"}.mdi-picture-in-picture-top-right:before{content:"󰹙"}.mdi-picture-in-picture-top-right-outline:before{content:"󰹚"}.mdi-pier:before{content:"󰢇"}.mdi-pier-crane:before{content:"󰢈"}.mdi-pig:before{content:"󰐁"}.mdi-pig-variant:before{content:"󱀆"}.mdi-pig-variant-outline:before{content:"󱙸"}.mdi-piggy-bank:before{content:"󱀇"}.mdi-piggy-bank-outline:before{content:"󱙹"}.mdi-pill:before{content:"󰐂"}.mdi-pill-multiple:before{content:"󱭌"}.mdi-pill-off:before{content:"󱩜"}.mdi-pillar:before{content:"󰜂"}.mdi-pin:before{content:"󰐃"}.mdi-pin-off:before{content:"󰐄"}.mdi-pin-off-outline:before{content:"󰤰"}.mdi-pin-outline:before{content:"󰤱"}.mdi-pine-tree:before{content:"󰐅"}.mdi-pine-tree-box:before{content:"󰐆"}.mdi-pine-tree-fire:before{content:"󱐚"}.mdi-pinterest:before{content:"󰐇"}.mdi-pinwheel:before{content:"󰫕"}.mdi-pinwheel-outline:before{content:"󰫖"}.mdi-pipe:before{content:"󰟥"}.mdi-pipe-disconnected:before{content:"󰟦"}.mdi-pipe-leak:before{content:"󰢉"}.mdi-pipe-valve:before{content:"󱡍"}.mdi-pipe-wrench:before{content:"󱍔"}.mdi-pirate:before{content:"󰨈"}.mdi-pistol:before{content:"󰜃"}.mdi-piston:before{content:"󰢊"}.mdi-pitchfork:before{content:"󱕓"}.mdi-pizza:before{content:"󰐉"}.mdi-plane-car:before{content:"󱫿"}.mdi-plane-train:before{content:"󱬀"}.mdi-play:before{content:"󰐊"}.mdi-play-box:before{content:"󱉺"}.mdi-play-box-lock:before{content:"󱨖"}.mdi-play-box-lock-open:before{content:"󱨗"}.mdi-play-box-lock-open-outline:before{content:"󱨘"}.mdi-play-box-lock-outline:before{content:"󱨙"}.mdi-play-box-multiple:before{content:"󰴙"}.mdi-play-box-multiple-outline:before{content:"󱏦"}.mdi-play-box-outline:before{content:"󰐋"}.mdi-play-circle:before{content:"󰐌"}.mdi-play-circle-outline:before{content:"󰐍"}.mdi-play-network:before{content:"󰢋"}.mdi-play-network-outline:before{content:"󰲷"}.mdi-play-outline:before{content:"󰼛"}.mdi-play-pause:before{content:"󰐎"}.mdi-play-protected-content:before{content:"󰐏"}.mdi-play-speed:before{content:"󰣿"}.mdi-playlist-check:before{content:"󰗇"}.mdi-playlist-edit:before{content:"󰤀"}.mdi-playlist-minus:before{content:"󰐐"}.mdi-playlist-music:before{content:"󰲸"}.mdi-playlist-music-outline:before{content:"󰲹"}.mdi-playlist-play:before{content:"󰐑"}.mdi-playlist-plus:before{content:"󰐒"}.mdi-playlist-remove:before{content:"󰐓"}.mdi-playlist-star:before{content:"󰷲"}.mdi-plex:before{content:"󰚺"}.mdi-pliers:before{content:"󱦤"}.mdi-plus:before{content:"󰐕"}.mdi-plus-box:before{content:"󰐖"}.mdi-plus-box-multiple:before{content:"󰌴"}.mdi-plus-box-multiple-outline:before{content:"󱅃"}.mdi-plus-box-outline:before{content:"󰜄"}.mdi-plus-circle:before{content:"󰐗"}.mdi-plus-circle-multiple:before{content:"󰍌"}.mdi-plus-circle-multiple-outline:before{content:"󰐘"}.mdi-plus-circle-outline:before{content:"󰐙"}.mdi-plus-lock:before{content:"󱩝"}.mdi-plus-lock-open:before{content:"󱩞"}.mdi-plus-minus:before{content:"󰦒"}.mdi-plus-minus-box:before{content:"󰦓"}.mdi-plus-minus-variant:before{content:"󱓉"}.mdi-plus-network:before{content:"󰐚"}.mdi-plus-network-outline:before{content:"󰲺"}.mdi-plus-outline:before{content:"󰜅"}.mdi-plus-thick:before{content:"󱇬"}.mdi-podcast:before{content:"󰦔"}.mdi-podium:before{content:"󰴥"}.mdi-podium-bronze:before{content:"󰴦"}.mdi-podium-gold:before{content:"󰴧"}.mdi-podium-silver:before{content:"󰴨"}.mdi-point-of-sale:before{content:"󰶒"}.mdi-pokeball:before{content:"󰐝"}.mdi-pokemon-go:before{content:"󰨉"}.mdi-poker-chip:before{content:"󰠰"}.mdi-polaroid:before{content:"󰐞"}.mdi-police-badge:before{content:"󱅧"}.mdi-police-badge-outline:before{content:"󱅨"}.mdi-police-station:before{content:"󱠹"}.mdi-poll:before{content:"󰐟"}.mdi-polo:before{content:"󱓃"}.mdi-polymer:before{content:"󰐡"}.mdi-pool:before{content:"󰘆"}.mdi-pool-thermometer:before{content:"󱩟"}.mdi-popcorn:before{content:"󰐢"}.mdi-post:before{content:"󱀈"}.mdi-post-lamp:before{content:"󱩠"}.mdi-post-outline:before{content:"󱀉"}.mdi-postage-stamp:before{content:"󰲻"}.mdi-pot:before{content:"󰋥"}.mdi-pot-mix:before{content:"󰙛"}.mdi-pot-mix-outline:before{content:"󰙷"}.mdi-pot-outline:before{content:"󰋿"}.mdi-pot-steam:before{content:"󰙚"}.mdi-pot-steam-outline:before{content:"󰌦"}.mdi-pound:before{content:"󰐣"}.mdi-pound-box:before{content:"󰐤"}.mdi-pound-box-outline:before{content:"󱅿"}.mdi-power:before{content:"󰐥"}.mdi-power-cycle:before{content:"󰤁"}.mdi-power-off:before{content:"󰤂"}.mdi-power-on:before{content:"󰤃"}.mdi-power-plug:before{content:"󰚥"}.mdi-power-plug-off:before{content:"󰚦"}.mdi-power-plug-off-outline:before{content:"󱐤"}.mdi-power-plug-outline:before{content:"󱐥"}.mdi-power-settings:before{content:"󰐦"}.mdi-power-sleep:before{content:"󰤄"}.mdi-power-socket:before{content:"󰐧"}.mdi-power-socket-au:before{content:"󰤅"}.mdi-power-socket-ch:before{content:"󰾳"}.mdi-power-socket-de:before{content:"󱄇"}.mdi-power-socket-eu:before{content:"󰟧"}.mdi-power-socket-fr:before{content:"󱄈"}.mdi-power-socket-it:before{content:"󱓿"}.mdi-power-socket-jp:before{content:"󱄉"}.mdi-power-socket-uk:before{content:"󰟨"}.mdi-power-socket-us:before{content:"󰟩"}.mdi-power-standby:before{content:"󰤆"}.mdi-powershell:before{content:"󰨊"}.mdi-prescription:before{content:"󰜆"}.mdi-presentation:before{content:"󰐨"}.mdi-presentation-play:before{content:"󰐩"}.mdi-pretzel:before{content:"󱕢"}.mdi-printer:before{content:"󰐪"}.mdi-printer-3d:before{content:"󰐫"}.mdi-printer-3d-nozzle:before{content:"󰹛"}.mdi-printer-3d-nozzle-alert:before{content:"󱇀"}.mdi-printer-3d-nozzle-alert-outline:before{content:"󱇁"}.mdi-printer-3d-nozzle-heat:before{content:"󱢸"}.mdi-printer-3d-nozzle-heat-outline:before{content:"󱢹"}.mdi-printer-3d-nozzle-off:before{content:"󱬙"}.mdi-printer-3d-nozzle-off-outline:before{content:"󱬚"}.mdi-printer-3d-nozzle-outline:before{content:"󰹜"}.mdi-printer-3d-off:before{content:"󱬎"}.mdi-printer-alert:before{content:"󰐬"}.mdi-printer-check:before{content:"󱅆"}.mdi-printer-eye:before{content:"󱑘"}.mdi-printer-off:before{content:"󰹝"}.mdi-printer-off-outline:before{content:"󱞅"}.mdi-printer-outline:before{content:"󱞆"}.mdi-printer-pos:before{content:"󱁗"}.mdi-printer-search:before{content:"󱑗"}.mdi-printer-settings:before{content:"󰜇"}.mdi-printer-wireless:before{content:"󰨋"}.mdi-priority-high:before{content:"󰘃"}.mdi-priority-low:before{content:"󰘄"}.mdi-professional-hexagon:before{content:"󰐭"}.mdi-progress-alert:before{content:"󰲼"}.mdi-progress-check:before{content:"󰦕"}.mdi-progress-clock:before{content:"󰦖"}.mdi-progress-close:before{content:"󱄊"}.mdi-progress-download:before{content:"󰦗"}.mdi-progress-helper:before{content:"󱮢"}.mdi-progress-pencil:before{content:"󱞇"}.mdi-progress-question:before{content:"󱔢"}.mdi-progress-star:before{content:"󱞈"}.mdi-progress-upload:before{content:"󰦘"}.mdi-progress-wrench:before{content:"󰲽"}.mdi-projector:before{content:"󰐮"}.mdi-projector-off:before{content:"󱨣"}.mdi-projector-screen:before{content:"󰐯"}.mdi-projector-screen-off:before{content:"󱠍"}.mdi-projector-screen-off-outline:before{content:"󱠎"}.mdi-projector-screen-outline:before{content:"󱜤"}.mdi-projector-screen-variant:before{content:"󱠏"}.mdi-projector-screen-variant-off:before{content:"󱠐"}.mdi-projector-screen-variant-off-outline:before{content:"󱠑"}.mdi-projector-screen-variant-outline:before{content:"󱠒"}.mdi-propane-tank:before{content:"󱍗"}.mdi-propane-tank-outline:before{content:"󱍘"}.mdi-protocol:before{content:"󰿘"}.mdi-publish:before{content:"󰚧"}.mdi-publish-off:before{content:"󱥅"}.mdi-pulse:before{content:"󰐰"}.mdi-pump:before{content:"󱐂"}.mdi-pump-off:before{content:"󱬢"}.mdi-pumpkin:before{content:"󰮿"}.mdi-purse:before{content:"󰼜"}.mdi-purse-outline:before{content:"󰼝"}.mdi-puzzle:before{content:"󰐱"}.mdi-puzzle-check:before{content:"󱐦"}.mdi-puzzle-check-outline:before{content:"󱐧"}.mdi-puzzle-edit:before{content:"󱓓"}.mdi-puzzle-edit-outline:before{content:"󱓙"}.mdi-puzzle-heart:before{content:"󱓔"}.mdi-puzzle-heart-outline:before{content:"󱓚"}.mdi-puzzle-minus:before{content:"󱓑"}.mdi-puzzle-minus-outline:before{content:"󱓗"}.mdi-puzzle-outline:before{content:"󰩦"}.mdi-puzzle-plus:before{content:"󱓐"}.mdi-puzzle-plus-outline:before{content:"󱓖"}.mdi-puzzle-remove:before{content:"󱓒"}.mdi-puzzle-remove-outline:before{content:"󱓘"}.mdi-puzzle-star:before{content:"󱓕"}.mdi-puzzle-star-outline:before{content:"󱓛"}.mdi-pyramid:before{content:"󱥒"}.mdi-pyramid-off:before{content:"󱥓"}.mdi-qi:before{content:"󰦙"}.mdi-qqchat:before{content:"󰘅"}.mdi-qrcode:before{content:"󰐲"}.mdi-qrcode-edit:before{content:"󰢸"}.mdi-qrcode-minus:before{content:"󱆌"}.mdi-qrcode-plus:before{content:"󱆋"}.mdi-qrcode-remove:before{content:"󱆍"}.mdi-qrcode-scan:before{content:"󰐳"}.mdi-quadcopter:before{content:"󰐴"}.mdi-quality-high:before{content:"󰐵"}.mdi-quality-low:before{content:"󰨌"}.mdi-quality-medium:before{content:"󰨍"}.mdi-quora:before{content:"󰴩"}.mdi-rabbit:before{content:"󰤇"}.mdi-rabbit-variant:before{content:"󱩡"}.mdi-rabbit-variant-outline:before{content:"󱩢"}.mdi-racing-helmet:before{content:"󰶓"}.mdi-racquetball:before{content:"󰶔"}.mdi-radar:before{content:"󰐷"}.mdi-radiator:before{content:"󰐸"}.mdi-radiator-disabled:before{content:"󰫗"}.mdi-radiator-off:before{content:"󰫘"}.mdi-radio:before{content:"󰐹"}.mdi-radio-am:before{content:"󰲾"}.mdi-radio-fm:before{content:"󰲿"}.mdi-radio-handheld:before{content:"󰐺"}.mdi-radio-off:before{content:"󱈜"}.mdi-radio-tower:before{content:"󰐻"}.mdi-radioactive:before{content:"󰐼"}.mdi-radioactive-circle:before{content:"󱡝"}.mdi-radioactive-circle-outline:before{content:"󱡞"}.mdi-radioactive-off:before{content:"󰻁"}.mdi-radiobox-blank:before{content:"󰐽"}.mdi-radiobox-marked:before{content:"󰐾"}.mdi-radiology-box:before{content:"󱓅"}.mdi-radiology-box-outline:before{content:"󱓆"}.mdi-radius:before{content:"󰳀"}.mdi-radius-outline:before{content:"󰳁"}.mdi-railroad-light:before{content:"󰼞"}.mdi-rake:before{content:"󱕄"}.mdi-raspberry-pi:before{content:"󰐿"}.mdi-raw:before{content:"󱨏"}.mdi-raw-off:before{content:"󱨐"}.mdi-ray-end:before{content:"󰑀"}.mdi-ray-end-arrow:before{content:"󰑁"}.mdi-ray-start:before{content:"󰑂"}.mdi-ray-start-arrow:before{content:"󰑃"}.mdi-ray-start-end:before{content:"󰑄"}.mdi-ray-start-vertex-end:before{content:"󱗘"}.mdi-ray-vertex:before{content:"󰑅"}.mdi-razor-double-edge:before{content:"󱦗"}.mdi-razor-single-edge:before{content:"󱦘"}.mdi-react:before{content:"󰜈"}.mdi-read:before{content:"󰑇"}.mdi-receipt:before{content:"󰠤"}.mdi-receipt-outline:before{content:"󰓷"}.mdi-receipt-text:before{content:"󰑉"}.mdi-receipt-text-check:before{content:"󱩣"}.mdi-receipt-text-check-outline:before{content:"󱩤"}.mdi-receipt-text-minus:before{content:"󱩥"}.mdi-receipt-text-minus-outline:before{content:"󱩦"}.mdi-receipt-text-outline:before{content:"󱧜"}.mdi-receipt-text-plus:before{content:"󱩧"}.mdi-receipt-text-plus-outline:before{content:"󱩨"}.mdi-receipt-text-remove:before{content:"󱩩"}.mdi-receipt-text-remove-outline:before{content:"󱩪"}.mdi-record:before{content:"󰑊"}.mdi-record-circle:before{content:"󰻂"}.mdi-record-circle-outline:before{content:"󰻃"}.mdi-record-player:before{content:"󰦚"}.mdi-record-rec:before{content:"󰑋"}.mdi-rectangle:before{content:"󰹞"}.mdi-rectangle-outline:before{content:"󰹟"}.mdi-recycle:before{content:"󰑌"}.mdi-recycle-variant:before{content:"󱎝"}.mdi-reddit:before{content:"󰑍"}.mdi-redhat:before{content:"󱄛"}.mdi-redo:before{content:"󰑎"}.mdi-redo-variant:before{content:"󰑏"}.mdi-reflect-horizontal:before{content:"󰨎"}.mdi-reflect-vertical:before{content:"󰨏"}.mdi-refresh:before{content:"󰑐"}.mdi-refresh-auto:before{content:"󱣲"}.mdi-refresh-circle:before{content:"󱍷"}.mdi-regex:before{content:"󰑑"}.mdi-registered-trademark:before{content:"󰩧"}.mdi-reiterate:before{content:"󱖈"}.mdi-relation-many-to-many:before{content:"󱒖"}.mdi-relation-many-to-one:before{content:"󱒗"}.mdi-relation-many-to-one-or-many:before{content:"󱒘"}.mdi-relation-many-to-only-one:before{content:"󱒙"}.mdi-relation-many-to-zero-or-many:before{content:"󱒚"}.mdi-relation-many-to-zero-or-one:before{content:"󱒛"}.mdi-relation-one-or-many-to-many:before{content:"󱒜"}.mdi-relation-one-or-many-to-one:before{content:"󱒝"}.mdi-relation-one-or-many-to-one-or-many:before{content:"󱒞"}.mdi-relation-one-or-many-to-only-one:before{content:"󱒟"}.mdi-relation-one-or-many-to-zero-or-many:before{content:"󱒠"}.mdi-relation-one-or-many-to-zero-or-one:before{content:"󱒡"}.mdi-relation-one-to-many:before{content:"󱒢"}.mdi-relation-one-to-one:before{content:"󱒣"}.mdi-relation-one-to-one-or-many:before{content:"󱒤"}.mdi-relation-one-to-only-one:before{content:"󱒥"}.mdi-relation-one-to-zero-or-many:before{content:"󱒦"}.mdi-relation-one-to-zero-or-one:before{content:"󱒧"}.mdi-relation-only-one-to-many:before{content:"󱒨"}.mdi-relation-only-one-to-one:before{content:"󱒩"}.mdi-relation-only-one-to-one-or-many:before{content:"󱒪"}.mdi-relation-only-one-to-only-one:before{content:"󱒫"}.mdi-relation-only-one-to-zero-or-many:before{content:"󱒬"}.mdi-relation-only-one-to-zero-or-one:before{content:"󱒭"}.mdi-relation-zero-or-many-to-many:before{content:"󱒮"}.mdi-relation-zero-or-many-to-one:before{content:"󱒯"}.mdi-relation-zero-or-many-to-one-or-many:before{content:"󱒰"}.mdi-relation-zero-or-many-to-only-one:before{content:"󱒱"}.mdi-relation-zero-or-many-to-zero-or-many:before{content:"󱒲"}.mdi-relation-zero-or-many-to-zero-or-one:before{content:"󱒳"}.mdi-relation-zero-or-one-to-many:before{content:"󱒴"}.mdi-relation-zero-or-one-to-one:before{content:"󱒵"}.mdi-relation-zero-or-one-to-one-or-many:before{content:"󱒶"}.mdi-relation-zero-or-one-to-only-one:before{content:"󱒷"}.mdi-relation-zero-or-one-to-zero-or-many:before{content:"󱒸"}.mdi-relation-zero-or-one-to-zero-or-one:before{content:"󱒹"}.mdi-relative-scale:before{content:"󰑒"}.mdi-reload:before{content:"󰑓"}.mdi-reload-alert:before{content:"󱄋"}.mdi-reminder:before{content:"󰢌"}.mdi-remote:before{content:"󰑔"}.mdi-remote-desktop:before{content:"󰢹"}.mdi-remote-off:before{content:"󰻄"}.mdi-remote-tv:before{content:"󰻅"}.mdi-remote-tv-off:before{content:"󰻆"}.mdi-rename-box:before{content:"󰑕"}.mdi-reorder-horizontal:before{content:"󰚈"}.mdi-reorder-vertical:before{content:"󰚉"}.mdi-repeat:before{content:"󰑖"}.mdi-repeat-off:before{content:"󰑗"}.mdi-repeat-once:before{content:"󰑘"}.mdi-repeat-variant:before{content:"󰕇"}.mdi-replay:before{content:"󰑙"}.mdi-reply:before{content:"󰑚"}.mdi-reply-all:before{content:"󰑛"}.mdi-reply-all-outline:before{content:"󰼟"}.mdi-reply-circle:before{content:"󱆮"}.mdi-reply-outline:before{content:"󰼠"}.mdi-reproduction:before{content:"󰑜"}.mdi-resistor:before{content:"󰭄"}.mdi-resistor-nodes:before{content:"󰭅"}.mdi-resize:before{content:"󰩨"}.mdi-resize-bottom-right:before{content:"󰑝"}.mdi-responsive:before{content:"󰑞"}.mdi-restart:before{content:"󰜉"}.mdi-restart-alert:before{content:"󱄌"}.mdi-restart-off:before{content:"󰶕"}.mdi-restore:before{content:"󰦛"}.mdi-restore-alert:before{content:"󱄍"}.mdi-rewind:before{content:"󰑟"}.mdi-rewind-10:before{content:"󰴪"}.mdi-rewind-15:before{content:"󱥆"}.mdi-rewind-30:before{content:"󰶖"}.mdi-rewind-45:before{content:"󱬓"}.mdi-rewind-5:before{content:"󱇹"}.mdi-rewind-60:before{content:"󱘌"}.mdi-rewind-outline:before{content:"󰜊"}.mdi-rhombus:before{content:"󰜋"}.mdi-rhombus-medium:before{content:"󰨐"}.mdi-rhombus-medium-outline:before{content:"󱓜"}.mdi-rhombus-outline:before{content:"󰜌"}.mdi-rhombus-split:before{content:"󰨑"}.mdi-rhombus-split-outline:before{content:"󱓝"}.mdi-ribbon:before{content:"󰑠"}.mdi-rice:before{content:"󰟪"}.mdi-rickshaw:before{content:"󱖻"}.mdi-rickshaw-electric:before{content:"󱖼"}.mdi-ring:before{content:"󰟫"}.mdi-rivet:before{content:"󰹠"}.mdi-road:before{content:"󰑡"}.mdi-road-variant:before{content:"󰑢"}.mdi-robber:before{content:"󱁘"}.mdi-robot:before{content:"󰚩"}.mdi-robot-angry:before{content:"󱚝"}.mdi-robot-angry-outline:before{content:"󱚞"}.mdi-robot-confused:before{content:"󱚟"}.mdi-robot-confused-outline:before{content:"󱚠"}.mdi-robot-dead:before{content:"󱚡"}.mdi-robot-dead-outline:before{content:"󱚢"}.mdi-robot-excited:before{content:"󱚣"}.mdi-robot-excited-outline:before{content:"󱚤"}.mdi-robot-happy:before{content:"󱜙"}.mdi-robot-happy-outline:before{content:"󱜚"}.mdi-robot-industrial:before{content:"󰭆"}.mdi-robot-industrial-outline:before{content:"󱨚"}.mdi-robot-love:before{content:"󱚥"}.mdi-robot-love-outline:before{content:"󱚦"}.mdi-robot-mower:before{content:"󱇷"}.mdi-robot-mower-outline:before{content:"󱇳"}.mdi-robot-off:before{content:"󱚧"}.mdi-robot-off-outline:before{content:"󱙻"}.mdi-robot-outline:before{content:"󱙺"}.mdi-robot-vacuum:before{content:"󰜍"}.mdi-robot-vacuum-alert:before{content:"󱭝"}.mdi-robot-vacuum-variant:before{content:"󰤈"}.mdi-robot-vacuum-variant-alert:before{content:"󱭞"}.mdi-rocket:before{content:"󰑣"}.mdi-rocket-launch:before{content:"󱓞"}.mdi-rocket-launch-outline:before{content:"󱓟"}.mdi-rocket-outline:before{content:"󱎯"}.mdi-rodent:before{content:"󱌧"}.mdi-roller-shade:before{content:"󱩫"}.mdi-roller-shade-closed:before{content:"󱩬"}.mdi-roller-skate:before{content:"󰴫"}.mdi-roller-skate-off:before{content:"󰅅"}.mdi-rollerblade:before{content:"󰴬"}.mdi-rollerblade-off:before{content:"󰀮"}.mdi-rollupjs:before{content:"󰯀"}.mdi-rolodex:before{content:"󱪹"}.mdi-rolodex-outline:before{content:"󱪺"}.mdi-roman-numeral-1:before{content:"󱂈"}.mdi-roman-numeral-10:before{content:"󱂑"}.mdi-roman-numeral-2:before{content:"󱂉"}.mdi-roman-numeral-3:before{content:"󱂊"}.mdi-roman-numeral-4:before{content:"󱂋"}.mdi-roman-numeral-5:before{content:"󱂌"}.mdi-roman-numeral-6:before{content:"󱂍"}.mdi-roman-numeral-7:before{content:"󱂎"}.mdi-roman-numeral-8:before{content:"󱂏"}.mdi-roman-numeral-9:before{content:"󱂐"}.mdi-room-service:before{content:"󰢍"}.mdi-room-service-outline:before{content:"󰶗"}.mdi-rotate-360:before{content:"󱦙"}.mdi-rotate-3d:before{content:"󰻇"}.mdi-rotate-3d-variant:before{content:"󰑤"}.mdi-rotate-left:before{content:"󰑥"}.mdi-rotate-left-variant:before{content:"󰑦"}.mdi-rotate-orbit:before{content:"󰶘"}.mdi-rotate-right:before{content:"󰑧"}.mdi-rotate-right-variant:before{content:"󰑨"}.mdi-rounded-corner:before{content:"󰘇"}.mdi-router:before{content:"󱇢"}.mdi-router-network:before{content:"󱂇"}.mdi-router-wireless:before{content:"󰑩"}.mdi-router-wireless-off:before{content:"󱖣"}.mdi-router-wireless-settings:before{content:"󰩩"}.mdi-routes:before{content:"󰑪"}.mdi-routes-clock:before{content:"󱁙"}.mdi-rowing:before{content:"󰘈"}.mdi-rss:before{content:"󰑫"}.mdi-rss-box:before{content:"󰑬"}.mdi-rss-off:before{content:"󰼡"}.mdi-rug:before{content:"󱑵"}.mdi-rugby:before{content:"󰶙"}.mdi-ruler:before{content:"󰑭"}.mdi-ruler-square:before{content:"󰳂"}.mdi-ruler-square-compass:before{content:"󰺾"}.mdi-run:before{content:"󰜎"}.mdi-run-fast:before{content:"󰑮"}.mdi-rv-truck:before{content:"󱇔"}.mdi-sack:before{content:"󰴮"}.mdi-sack-percent:before{content:"󰴯"}.mdi-safe:before{content:"󰩪"}.mdi-safe-square:before{content:"󱉼"}.mdi-safe-square-outline:before{content:"󱉽"}.mdi-safety-goggles:before{content:"󰴰"}.mdi-sail-boat:before{content:"󰻈"}.mdi-sail-boat-sink:before{content:"󱫯"}.mdi-sale:before{content:"󰑯"}.mdi-sale-outline:before{content:"󱨆"}.mdi-salesforce:before{content:"󰢎"}.mdi-sass:before{content:"󰟬"}.mdi-satellite:before{content:"󰑰"}.mdi-satellite-uplink:before{content:"󰤉"}.mdi-satellite-variant:before{content:"󰑱"}.mdi-sausage:before{content:"󰢺"}.mdi-sausage-off:before{content:"󱞉"}.mdi-saw-blade:before{content:"󰹡"}.mdi-sawtooth-wave:before{content:"󱑺"}.mdi-saxophone:before{content:"󰘉"}.mdi-scale:before{content:"󰑲"}.mdi-scale-balance:before{content:"󰗑"}.mdi-scale-bathroom:before{content:"󰑳"}.mdi-scale-off:before{content:"󱁚"}.mdi-scale-unbalanced:before{content:"󱦸"}.mdi-scan-helper:before{content:"󱏘"}.mdi-scanner:before{content:"󰚫"}.mdi-scanner-off:before{content:"󰤊"}.mdi-scatter-plot:before{content:"󰻉"}.mdi-scatter-plot-outline:before{content:"󰻊"}.mdi-scent:before{content:"󱥘"}.mdi-scent-off:before{content:"󱥙"}.mdi-school:before{content:"󰑴"}.mdi-school-outline:before{content:"󱆀"}.mdi-scissors-cutting:before{content:"󰩫"}.mdi-scooter:before{content:"󱖽"}.mdi-scooter-electric:before{content:"󱖾"}.mdi-scoreboard:before{content:"󱉾"}.mdi-scoreboard-outline:before{content:"󱉿"}.mdi-screen-rotation:before{content:"󰑵"}.mdi-screen-rotation-lock:before{content:"󰑸"}.mdi-screw-flat-top:before{content:"󰷳"}.mdi-screw-lag:before{content:"󰷴"}.mdi-screw-machine-flat-top:before{content:"󰷵"}.mdi-screw-machine-round-top:before{content:"󰷶"}.mdi-screw-round-top:before{content:"󰷷"}.mdi-screwdriver:before{content:"󰑶"}.mdi-script:before{content:"󰯁"}.mdi-script-outline:before{content:"󰑷"}.mdi-script-text:before{content:"󰯂"}.mdi-script-text-key:before{content:"󱜥"}.mdi-script-text-key-outline:before{content:"󱜦"}.mdi-script-text-outline:before{content:"󰯃"}.mdi-script-text-play:before{content:"󱜧"}.mdi-script-text-play-outline:before{content:"󱜨"}.mdi-sd:before{content:"󰑹"}.mdi-seal:before{content:"󰑺"}.mdi-seal-variant:before{content:"󰿙"}.mdi-search-web:before{content:"󰜏"}.mdi-seat:before{content:"󰳃"}.mdi-seat-flat:before{content:"󰑻"}.mdi-seat-flat-angled:before{content:"󰑼"}.mdi-seat-individual-suite:before{content:"󰑽"}.mdi-seat-legroom-extra:before{content:"󰑾"}.mdi-seat-legroom-normal:before{content:"󰑿"}.mdi-seat-legroom-reduced:before{content:"󰒀"}.mdi-seat-outline:before{content:"󰳄"}.mdi-seat-passenger:before{content:"󱉉"}.mdi-seat-recline-extra:before{content:"󰒁"}.mdi-seat-recline-normal:before{content:"󰒂"}.mdi-seatbelt:before{content:"󰳅"}.mdi-security:before{content:"󰒃"}.mdi-security-network:before{content:"󰒄"}.mdi-seed:before{content:"󰹢"}.mdi-seed-off:before{content:"󱏽"}.mdi-seed-off-outline:before{content:"󱏾"}.mdi-seed-outline:before{content:"󰹣"}.mdi-seed-plus:before{content:"󱩭"}.mdi-seed-plus-outline:before{content:"󱩮"}.mdi-seesaw:before{content:"󱖤"}.mdi-segment:before{content:"󰻋"}.mdi-select:before{content:"󰒅"}.mdi-select-all:before{content:"󰒆"}.mdi-select-arrow-down:before{content:"󱭙"}.mdi-select-arrow-up:before{content:"󱭘"}.mdi-select-color:before{content:"󰴱"}.mdi-select-compare:before{content:"󰫙"}.mdi-select-drag:before{content:"󰩬"}.mdi-select-group:before{content:"󰾂"}.mdi-select-inverse:before{content:"󰒇"}.mdi-select-marker:before{content:"󱊀"}.mdi-select-multiple:before{content:"󱊁"}.mdi-select-multiple-marker:before{content:"󱊂"}.mdi-select-off:before{content:"󰒈"}.mdi-select-place:before{content:"󰿚"}.mdi-select-remove:before{content:"󱟁"}.mdi-select-search:before{content:"󱈄"}.mdi-selection:before{content:"󰒉"}.mdi-selection-drag:before{content:"󰩭"}.mdi-selection-ellipse:before{content:"󰴲"}.mdi-selection-ellipse-arrow-inside:before{content:"󰼢"}.mdi-selection-ellipse-remove:before{content:"󱟂"}.mdi-selection-marker:before{content:"󱊃"}.mdi-selection-multiple:before{content:"󱊅"}.mdi-selection-multiple-marker:before{content:"󱊄"}.mdi-selection-off:before{content:"󰝷"}.mdi-selection-remove:before{content:"󱟃"}.mdi-selection-search:before{content:"󱈅"}.mdi-semantic-web:before{content:"󱌖"}.mdi-send:before{content:"󰒊"}.mdi-send-check:before{content:"󱅡"}.mdi-send-check-outline:before{content:"󱅢"}.mdi-send-circle:before{content:"󰷸"}.mdi-send-circle-outline:before{content:"󰷹"}.mdi-send-clock:before{content:"󱅣"}.mdi-send-clock-outline:before{content:"󱅤"}.mdi-send-lock:before{content:"󰟭"}.mdi-send-lock-outline:before{content:"󱅦"}.mdi-send-outline:before{content:"󱅥"}.mdi-serial-port:before{content:"󰙜"}.mdi-server:before{content:"󰒋"}.mdi-server-minus:before{content:"󰒌"}.mdi-server-network:before{content:"󰒍"}.mdi-server-network-off:before{content:"󰒎"}.mdi-server-off:before{content:"󰒏"}.mdi-server-plus:before{content:"󰒐"}.mdi-server-remove:before{content:"󰒑"}.mdi-server-security:before{content:"󰒒"}.mdi-set-all:before{content:"󰝸"}.mdi-set-center:before{content:"󰝹"}.mdi-set-center-right:before{content:"󰝺"}.mdi-set-left:before{content:"󰝻"}.mdi-set-left-center:before{content:"󰝼"}.mdi-set-left-right:before{content:"󰝽"}.mdi-set-merge:before{content:"󱓠"}.mdi-set-none:before{content:"󰝾"}.mdi-set-right:before{content:"󰝿"}.mdi-set-split:before{content:"󱓡"}.mdi-set-square:before{content:"󱑝"}.mdi-set-top-box:before{content:"󰦟"}.mdi-settings-helper:before{content:"󰩮"}.mdi-shaker:before{content:"󱄎"}.mdi-shaker-outline:before{content:"󱄏"}.mdi-shape:before{content:"󰠱"}.mdi-shape-circle-plus:before{content:"󰙝"}.mdi-shape-outline:before{content:"󰠲"}.mdi-shape-oval-plus:before{content:"󱇺"}.mdi-shape-plus:before{content:"󰒕"}.mdi-shape-polygon-plus:before{content:"󰙞"}.mdi-shape-rectangle-plus:before{content:"󰙟"}.mdi-shape-square-plus:before{content:"󰙠"}.mdi-shape-square-rounded-plus:before{content:"󱓺"}.mdi-share:before{content:"󰒖"}.mdi-share-all:before{content:"󱇴"}.mdi-share-all-outline:before{content:"󱇵"}.mdi-share-circle:before{content:"󱆭"}.mdi-share-off:before{content:"󰼣"}.mdi-share-off-outline:before{content:"󰼤"}.mdi-share-outline:before{content:"󰤲"}.mdi-share-variant:before{content:"󰒗"}.mdi-share-variant-outline:before{content:"󱔔"}.mdi-shark:before{content:"󱢺"}.mdi-shark-fin:before{content:"󱙳"}.mdi-shark-fin-outline:before{content:"󱙴"}.mdi-shark-off:before{content:"󱢻"}.mdi-sheep:before{content:"󰳆"}.mdi-shield:before{content:"󰒘"}.mdi-shield-account:before{content:"󰢏"}.mdi-shield-account-outline:before{content:"󰨒"}.mdi-shield-account-variant:before{content:"󱖧"}.mdi-shield-account-variant-outline:before{content:"󱖨"}.mdi-shield-airplane:before{content:"󰚻"}.mdi-shield-airplane-outline:before{content:"󰳇"}.mdi-shield-alert:before{content:"󰻌"}.mdi-shield-alert-outline:before{content:"󰻍"}.mdi-shield-bug:before{content:"󱏚"}.mdi-shield-bug-outline:before{content:"󱏛"}.mdi-shield-car:before{content:"󰾃"}.mdi-shield-check:before{content:"󰕥"}.mdi-shield-check-outline:before{content:"󰳈"}.mdi-shield-cross:before{content:"󰳉"}.mdi-shield-cross-outline:before{content:"󰳊"}.mdi-shield-crown:before{content:"󱢼"}.mdi-shield-crown-outline:before{content:"󱢽"}.mdi-shield-edit:before{content:"󱆠"}.mdi-shield-edit-outline:before{content:"󱆡"}.mdi-shield-half:before{content:"󱍠"}.mdi-shield-half-full:before{content:"󰞀"}.mdi-shield-home:before{content:"󰚊"}.mdi-shield-home-outline:before{content:"󰳋"}.mdi-shield-key:before{content:"󰯄"}.mdi-shield-key-outline:before{content:"󰯅"}.mdi-shield-link-variant:before{content:"󰴳"}.mdi-shield-link-variant-outline:before{content:"󰴴"}.mdi-shield-lock:before{content:"󰦝"}.mdi-shield-lock-open:before{content:"󱦚"}.mdi-shield-lock-open-outline:before{content:"󱦛"}.mdi-shield-lock-outline:before{content:"󰳌"}.mdi-shield-moon:before{content:"󱠨"}.mdi-shield-moon-outline:before{content:"󱠩"}.mdi-shield-off:before{content:"󰦞"}.mdi-shield-off-outline:before{content:"󰦜"}.mdi-shield-outline:before{content:"󰒙"}.mdi-shield-plus:before{content:"󰫚"}.mdi-shield-plus-outline:before{content:"󰫛"}.mdi-shield-refresh:before{content:"󰂪"}.mdi-shield-refresh-outline:before{content:"󰇠"}.mdi-shield-remove:before{content:"󰫜"}.mdi-shield-remove-outline:before{content:"󰫝"}.mdi-shield-search:before{content:"󰶚"}.mdi-shield-star:before{content:"󱄻"}.mdi-shield-star-outline:before{content:"󱄼"}.mdi-shield-sun:before{content:"󱁝"}.mdi-shield-sun-outline:before{content:"󱁞"}.mdi-shield-sword:before{content:"󱢾"}.mdi-shield-sword-outline:before{content:"󱢿"}.mdi-shield-sync:before{content:"󱆢"}.mdi-shield-sync-outline:before{content:"󱆣"}.mdi-shimmer:before{content:"󱕅"}.mdi-ship-wheel:before{content:"󰠳"}.mdi-shipping-pallet:before{content:"󱡎"}.mdi-shoe-ballet:before{content:"󱗊"}.mdi-shoe-cleat:before{content:"󱗇"}.mdi-shoe-formal:before{content:"󰭇"}.mdi-shoe-heel:before{content:"󰭈"}.mdi-shoe-print:before{content:"󰷺"}.mdi-shoe-sneaker:before{content:"󱗈"}.mdi-shopping:before{content:"󰒚"}.mdi-shopping-music:before{content:"󰒛"}.mdi-shopping-outline:before{content:"󱇕"}.mdi-shopping-search:before{content:"󰾄"}.mdi-shopping-search-outline:before{content:"󱩯"}.mdi-shore:before{content:"󱓹"}.mdi-shovel:before{content:"󰜐"}.mdi-shovel-off:before{content:"󰜑"}.mdi-shower:before{content:"󰦠"}.mdi-shower-head:before{content:"󰦡"}.mdi-shredder:before{content:"󰒜"}.mdi-shuffle:before{content:"󰒝"}.mdi-shuffle-disabled:before{content:"󰒞"}.mdi-shuffle-variant:before{content:"󰒟"}.mdi-shuriken:before{content:"󱍿"}.mdi-sickle:before{content:"󱣀"}.mdi-sigma:before{content:"󰒠"}.mdi-sigma-lower:before{content:"󰘫"}.mdi-sign-caution:before{content:"󰒡"}.mdi-sign-direction:before{content:"󰞁"}.mdi-sign-direction-minus:before{content:"󱀀"}.mdi-sign-direction-plus:before{content:"󰿜"}.mdi-sign-direction-remove:before{content:"󰿝"}.mdi-sign-language:before{content:"󱭍"}.mdi-sign-language-outline:before{content:"󱭎"}.mdi-sign-pole:before{content:"󱓸"}.mdi-sign-real-estate:before{content:"󱄘"}.mdi-sign-text:before{content:"󰞂"}.mdi-sign-yield:before{content:"󱮯"}.mdi-signal:before{content:"󰒢"}.mdi-signal-2g:before{content:"󰜒"}.mdi-signal-3g:before{content:"󰜓"}.mdi-signal-4g:before{content:"󰜔"}.mdi-signal-5g:before{content:"󰩯"}.mdi-signal-cellular-1:before{content:"󰢼"}.mdi-signal-cellular-2:before{content:"󰢽"}.mdi-signal-cellular-3:before{content:"󰢾"}.mdi-signal-cellular-outline:before{content:"󰢿"}.mdi-signal-distance-variant:before{content:"󰹤"}.mdi-signal-hspa:before{content:"󰜕"}.mdi-signal-hspa-plus:before{content:"󰜖"}.mdi-signal-off:before{content:"󰞃"}.mdi-signal-variant:before{content:"󰘊"}.mdi-signature:before{content:"󰷻"}.mdi-signature-freehand:before{content:"󰷼"}.mdi-signature-image:before{content:"󰷽"}.mdi-signature-text:before{content:"󰷾"}.mdi-silo:before{content:"󱮟"}.mdi-silo-outline:before{content:"󰭉"}.mdi-silverware:before{content:"󰒣"}.mdi-silverware-clean:before{content:"󰿞"}.mdi-silverware-fork:before{content:"󰒤"}.mdi-silverware-fork-knife:before{content:"󰩰"}.mdi-silverware-spoon:before{content:"󰒥"}.mdi-silverware-variant:before{content:"󰒦"}.mdi-sim:before{content:"󰒧"}.mdi-sim-alert:before{content:"󰒨"}.mdi-sim-alert-outline:before{content:"󱗓"}.mdi-sim-off:before{content:"󰒩"}.mdi-sim-off-outline:before{content:"󱗔"}.mdi-sim-outline:before{content:"󱗕"}.mdi-simple-icons:before{content:"󱌝"}.mdi-sina-weibo:before{content:"󰫟"}.mdi-sine-wave:before{content:"󰥛"}.mdi-sitemap:before{content:"󰒪"}.mdi-sitemap-outline:before{content:"󱦜"}.mdi-size-l:before{content:"󱎦"}.mdi-size-m:before{content:"󱎥"}.mdi-size-s:before{content:"󱎤"}.mdi-size-xl:before{content:"󱎧"}.mdi-size-xs:before{content:"󱎣"}.mdi-size-xxl:before{content:"󱎨"}.mdi-size-xxs:before{content:"󱎢"}.mdi-size-xxxl:before{content:"󱎩"}.mdi-skate:before{content:"󰴵"}.mdi-skate-off:before{content:"󰚙"}.mdi-skateboard:before{content:"󱓂"}.mdi-skateboarding:before{content:"󰔁"}.mdi-skew-less:before{content:"󰴶"}.mdi-skew-more:before{content:"󰴷"}.mdi-ski:before{content:"󱌄"}.mdi-ski-cross-country:before{content:"󱌅"}.mdi-ski-water:before{content:"󱌆"}.mdi-skip-backward:before{content:"󰒫"}.mdi-skip-backward-outline:before{content:"󰼥"}.mdi-skip-forward:before{content:"󰒬"}.mdi-skip-forward-outline:before{content:"󰼦"}.mdi-skip-next:before{content:"󰒭"}.mdi-skip-next-circle:before{content:"󰙡"}.mdi-skip-next-circle-outline:before{content:"󰙢"}.mdi-skip-next-outline:before{content:"󰼧"}.mdi-skip-previous:before{content:"󰒮"}.mdi-skip-previous-circle:before{content:"󰙣"}.mdi-skip-previous-circle-outline:before{content:"󰙤"}.mdi-skip-previous-outline:before{content:"󰼨"}.mdi-skull:before{content:"󰚌"}.mdi-skull-crossbones:before{content:"󰯆"}.mdi-skull-crossbones-outline:before{content:"󰯇"}.mdi-skull-outline:before{content:"󰯈"}.mdi-skull-scan:before{content:"󱓇"}.mdi-skull-scan-outline:before{content:"󱓈"}.mdi-skype:before{content:"󰒯"}.mdi-skype-business:before{content:"󰒰"}.mdi-slack:before{content:"󰒱"}.mdi-slash-forward:before{content:"󰿟"}.mdi-slash-forward-box:before{content:"󰿠"}.mdi-sledding:before{content:"󰐛"}.mdi-sleep:before{content:"󰒲"}.mdi-sleep-off:before{content:"󰒳"}.mdi-slide:before{content:"󱖥"}.mdi-slope-downhill:before{content:"󰷿"}.mdi-slope-uphill:before{content:"󰸀"}.mdi-slot-machine:before{content:"󱄔"}.mdi-slot-machine-outline:before{content:"󱄕"}.mdi-smart-card:before{content:"󱂽"}.mdi-smart-card-off:before{content:"󱣷"}.mdi-smart-card-off-outline:before{content:"󱣸"}.mdi-smart-card-outline:before{content:"󱂾"}.mdi-smart-card-reader:before{content:"󱂿"}.mdi-smart-card-reader-outline:before{content:"󱃀"}.mdi-smog:before{content:"󰩱"}.mdi-smoke:before{content:"󱞙"}.mdi-smoke-detector:before{content:"󰎒"}.mdi-smoke-detector-alert:before{content:"󱤮"}.mdi-smoke-detector-alert-outline:before{content:"󱤯"}.mdi-smoke-detector-off:before{content:"󱠉"}.mdi-smoke-detector-off-outline:before{content:"󱠊"}.mdi-smoke-detector-outline:before{content:"󱠈"}.mdi-smoke-detector-variant:before{content:"󱠋"}.mdi-smoke-detector-variant-alert:before{content:"󱤰"}.mdi-smoke-detector-variant-off:before{content:"󱠌"}.mdi-smoking:before{content:"󰒴"}.mdi-smoking-off:before{content:"󰒵"}.mdi-smoking-pipe:before{content:"󱐍"}.mdi-smoking-pipe-off:before{content:"󱐨"}.mdi-snail:before{content:"󱙷"}.mdi-snake:before{content:"󱔎"}.mdi-snapchat:before{content:"󰒶"}.mdi-snowboard:before{content:"󱌇"}.mdi-snowflake:before{content:"󰜗"}.mdi-snowflake-alert:before{content:"󰼩"}.mdi-snowflake-check:before{content:"󱩰"}.mdi-snowflake-melt:before{content:"󱋋"}.mdi-snowflake-off:before{content:"󱓣"}.mdi-snowflake-thermometer:before{content:"󱩱"}.mdi-snowflake-variant:before{content:"󰼪"}.mdi-snowman:before{content:"󰒷"}.mdi-snowmobile:before{content:"󰛝"}.mdi-snowshoeing:before{content:"󱩲"}.mdi-soccer:before{content:"󰒸"}.mdi-soccer-field:before{content:"󰠴"}.mdi-social-distance-2-meters:before{content:"󱕹"}.mdi-social-distance-6-feet:before{content:"󱕺"}.mdi-sofa:before{content:"󰒹"}.mdi-sofa-outline:before{content:"󱕭"}.mdi-sofa-single:before{content:"󱕮"}.mdi-sofa-single-outline:before{content:"󱕯"}.mdi-solar-panel:before{content:"󰶛"}.mdi-solar-panel-large:before{content:"󰶜"}.mdi-solar-power:before{content:"󰩲"}.mdi-solar-power-variant:before{content:"󱩳"}.mdi-solar-power-variant-outline:before{content:"󱩴"}.mdi-soldering-iron:before{content:"󱂒"}.mdi-solid:before{content:"󰚍"}.mdi-sony-playstation:before{content:"󰐔"}.mdi-sort:before{content:"󰒺"}.mdi-sort-alphabetical-ascending:before{content:"󰖽"}.mdi-sort-alphabetical-ascending-variant:before{content:"󱅈"}.mdi-sort-alphabetical-descending:before{content:"󰖿"}.mdi-sort-alphabetical-descending-variant:before{content:"󱅉"}.mdi-sort-alphabetical-variant:before{content:"󰒻"}.mdi-sort-ascending:before{content:"󰒼"}.mdi-sort-bool-ascending:before{content:"󱎅"}.mdi-sort-bool-ascending-variant:before{content:"󱎆"}.mdi-sort-bool-descending:before{content:"󱎇"}.mdi-sort-bool-descending-variant:before{content:"󱎈"}.mdi-sort-calendar-ascending:before{content:"󱕇"}.mdi-sort-calendar-descending:before{content:"󱕈"}.mdi-sort-clock-ascending:before{content:"󱕉"}.mdi-sort-clock-ascending-outline:before{content:"󱕊"}.mdi-sort-clock-descending:before{content:"󱕋"}.mdi-sort-clock-descending-outline:before{content:"󱕌"}.mdi-sort-descending:before{content:"󰒽"}.mdi-sort-numeric-ascending:before{content:"󱎉"}.mdi-sort-numeric-ascending-variant:before{content:"󰤍"}.mdi-sort-numeric-descending:before{content:"󱎊"}.mdi-sort-numeric-descending-variant:before{content:"󰫒"}.mdi-sort-numeric-variant:before{content:"󰒾"}.mdi-sort-reverse-variant:before{content:"󰌼"}.mdi-sort-variant:before{content:"󰒿"}.mdi-sort-variant-lock:before{content:"󰳍"}.mdi-sort-variant-lock-open:before{content:"󰳎"}.mdi-sort-variant-off:before{content:"󱪻"}.mdi-sort-variant-remove:before{content:"󱅇"}.mdi-soundbar:before{content:"󱟛"}.mdi-soundcloud:before{content:"󰓀"}.mdi-source-branch:before{content:"󰘬"}.mdi-source-branch-check:before{content:"󱓏"}.mdi-source-branch-minus:before{content:"󱓋"}.mdi-source-branch-plus:before{content:"󱓊"}.mdi-source-branch-refresh:before{content:"󱓍"}.mdi-source-branch-remove:before{content:"󱓌"}.mdi-source-branch-sync:before{content:"󱓎"}.mdi-source-commit:before{content:"󰜘"}.mdi-source-commit-end:before{content:"󰜙"}.mdi-source-commit-end-local:before{content:"󰜚"}.mdi-source-commit-local:before{content:"󰜛"}.mdi-source-commit-next-local:before{content:"󰜜"}.mdi-source-commit-start:before{content:"󰜝"}.mdi-source-commit-start-next-local:before{content:"󰜞"}.mdi-source-fork:before{content:"󰓁"}.mdi-source-merge:before{content:"󰘭"}.mdi-source-pull:before{content:"󰓂"}.mdi-source-repository:before{content:"󰳏"}.mdi-source-repository-multiple:before{content:"󰳐"}.mdi-soy-sauce:before{content:"󰟮"}.mdi-soy-sauce-off:before{content:"󱏼"}.mdi-spa:before{content:"󰳑"}.mdi-spa-outline:before{content:"󰳒"}.mdi-space-invaders:before{content:"󰯉"}.mdi-space-station:before{content:"󱎃"}.mdi-spade:before{content:"󰹥"}.mdi-speaker:before{content:"󰓃"}.mdi-speaker-bluetooth:before{content:"󰦢"}.mdi-speaker-message:before{content:"󱬑"}.mdi-speaker-multiple:before{content:"󰴸"}.mdi-speaker-off:before{content:"󰓄"}.mdi-speaker-pause:before{content:"󱭳"}.mdi-speaker-play:before{content:"󱭲"}.mdi-speaker-stop:before{content:"󱭴"}.mdi-speaker-wireless:before{content:"󰜟"}.mdi-spear:before{content:"󱡅"}.mdi-speedometer:before{content:"󰓅"}.mdi-speedometer-medium:before{content:"󰾅"}.mdi-speedometer-slow:before{content:"󰾆"}.mdi-spellcheck:before{content:"󰓆"}.mdi-sphere:before{content:"󱥔"}.mdi-sphere-off:before{content:"󱥕"}.mdi-spider:before{content:"󱇪"}.mdi-spider-thread:before{content:"󱇫"}.mdi-spider-web:before{content:"󰯊"}.mdi-spirit-level:before{content:"󱓱"}.mdi-spoon-sugar:before{content:"󱐩"}.mdi-spotify:before{content:"󰓇"}.mdi-spotlight:before{content:"󰓈"}.mdi-spotlight-beam:before{content:"󰓉"}.mdi-spray:before{content:"󰙥"}.mdi-spray-bottle:before{content:"󰫠"}.mdi-sprinkler:before{content:"󱁟"}.mdi-sprinkler-fire:before{content:"󱦝"}.mdi-sprinkler-variant:before{content:"󱁠"}.mdi-sprout:before{content:"󰹦"}.mdi-sprout-outline:before{content:"󰹧"}.mdi-square:before{content:"󰝤"}.mdi-square-circle:before{content:"󱔀"}.mdi-square-edit-outline:before{content:"󰤌"}.mdi-square-medium:before{content:"󰨓"}.mdi-square-medium-outline:before{content:"󰨔"}.mdi-square-off:before{content:"󱋮"}.mdi-square-off-outline:before{content:"󱋯"}.mdi-square-opacity:before{content:"󱡔"}.mdi-square-outline:before{content:"󰝣"}.mdi-square-root:before{content:"󰞄"}.mdi-square-root-box:before{content:"󰦣"}.mdi-square-rounded:before{content:"󱓻"}.mdi-square-rounded-badge:before{content:"󱨇"}.mdi-square-rounded-badge-outline:before{content:"󱨈"}.mdi-square-rounded-outline:before{content:"󱓼"}.mdi-square-small:before{content:"󰨕"}.mdi-square-wave:before{content:"󱑻"}.mdi-squeegee:before{content:"󰫡"}.mdi-ssh:before{content:"󰣀"}.mdi-stack-exchange:before{content:"󰘋"}.mdi-stack-overflow:before{content:"󰓌"}.mdi-stackpath:before{content:"󰍙"}.mdi-stadium:before{content:"󰿹"}.mdi-stadium-outline:before{content:"󱬃"}.mdi-stadium-variant:before{content:"󰜠"}.mdi-stairs:before{content:"󰓍"}.mdi-stairs-box:before{content:"󱎞"}.mdi-stairs-down:before{content:"󱊾"}.mdi-stairs-up:before{content:"󱊽"}.mdi-stamper:before{content:"󰴹"}.mdi-standard-definition:before{content:"󰟯"}.mdi-star:before{content:"󰓎"}.mdi-star-box:before{content:"󰩳"}.mdi-star-box-multiple:before{content:"󱊆"}.mdi-star-box-multiple-outline:before{content:"󱊇"}.mdi-star-box-outline:before{content:"󰩴"}.mdi-star-check:before{content:"󱕦"}.mdi-star-check-outline:before{content:"󱕪"}.mdi-star-circle:before{content:"󰓏"}.mdi-star-circle-outline:before{content:"󰦤"}.mdi-star-cog:before{content:"󱙨"}.mdi-star-cog-outline:before{content:"󱙩"}.mdi-star-crescent:before{content:"󰥹"}.mdi-star-david:before{content:"󰥺"}.mdi-star-face:before{content:"󰦥"}.mdi-star-four-points:before{content:"󰫢"}.mdi-star-four-points-outline:before{content:"󰫣"}.mdi-star-half:before{content:"󰉆"}.mdi-star-half-full:before{content:"󰓐"}.mdi-star-minus:before{content:"󱕤"}.mdi-star-minus-outline:before{content:"󱕨"}.mdi-star-off:before{content:"󰓑"}.mdi-star-off-outline:before{content:"󱕛"}.mdi-star-outline:before{content:"󰓒"}.mdi-star-plus:before{content:"󱕣"}.mdi-star-plus-outline:before{content:"󱕧"}.mdi-star-remove:before{content:"󱕥"}.mdi-star-remove-outline:before{content:"󱕩"}.mdi-star-settings:before{content:"󱙪"}.mdi-star-settings-outline:before{content:"󱙫"}.mdi-star-shooting:before{content:"󱝁"}.mdi-star-shooting-outline:before{content:"󱝂"}.mdi-star-three-points:before{content:"󰫤"}.mdi-star-three-points-outline:before{content:"󰫥"}.mdi-state-machine:before{content:"󱇯"}.mdi-steam:before{content:"󰓓"}.mdi-steering:before{content:"󰓔"}.mdi-steering-off:before{content:"󰤎"}.mdi-step-backward:before{content:"󰓕"}.mdi-step-backward-2:before{content:"󰓖"}.mdi-step-forward:before{content:"󰓗"}.mdi-step-forward-2:before{content:"󰓘"}.mdi-stethoscope:before{content:"󰓙"}.mdi-sticker:before{content:"󱍤"}.mdi-sticker-alert:before{content:"󱍥"}.mdi-sticker-alert-outline:before{content:"󱍦"}.mdi-sticker-check:before{content:"󱍧"}.mdi-sticker-check-outline:before{content:"󱍨"}.mdi-sticker-circle-outline:before{content:"󰗐"}.mdi-sticker-emoji:before{content:"󰞅"}.mdi-sticker-minus:before{content:"󱍩"}.mdi-sticker-minus-outline:before{content:"󱍪"}.mdi-sticker-outline:before{content:"󱍫"}.mdi-sticker-plus:before{content:"󱍬"}.mdi-sticker-plus-outline:before{content:"󱍭"}.mdi-sticker-remove:before{content:"󱍮"}.mdi-sticker-remove-outline:before{content:"󱍯"}.mdi-sticker-text:before{content:"󱞎"}.mdi-sticker-text-outline:before{content:"󱞏"}.mdi-stocking:before{content:"󰓚"}.mdi-stomach:before{content:"󱂓"}.mdi-stool:before{content:"󱥝"}.mdi-stool-outline:before{content:"󱥞"}.mdi-stop:before{content:"󰓛"}.mdi-stop-circle:before{content:"󰙦"}.mdi-stop-circle-outline:before{content:"󰙧"}.mdi-storage-tank:before{content:"󱩵"}.mdi-storage-tank-outline:before{content:"󱩶"}.mdi-store:before{content:"󰓜"}.mdi-store-24-hour:before{content:"󰓝"}.mdi-store-alert:before{content:"󱣁"}.mdi-store-alert-outline:before{content:"󱣂"}.mdi-store-check:before{content:"󱣃"}.mdi-store-check-outline:before{content:"󱣄"}.mdi-store-clock:before{content:"󱣅"}.mdi-store-clock-outline:before{content:"󱣆"}.mdi-store-cog:before{content:"󱣇"}.mdi-store-cog-outline:before{content:"󱣈"}.mdi-store-edit:before{content:"󱣉"}.mdi-store-edit-outline:before{content:"󱣊"}.mdi-store-marker:before{content:"󱣋"}.mdi-store-marker-outline:before{content:"󱣌"}.mdi-store-minus:before{content:"󱙞"}.mdi-store-minus-outline:before{content:"󱣍"}.mdi-store-off:before{content:"󱣎"}.mdi-store-off-outline:before{content:"󱣏"}.mdi-store-outline:before{content:"󱍡"}.mdi-store-plus:before{content:"󱙟"}.mdi-store-plus-outline:before{content:"󱣐"}.mdi-store-remove:before{content:"󱙠"}.mdi-store-remove-outline:before{content:"󱣑"}.mdi-store-search:before{content:"󱣒"}.mdi-store-search-outline:before{content:"󱣓"}.mdi-store-settings:before{content:"󱣔"}.mdi-store-settings-outline:before{content:"󱣕"}.mdi-storefront:before{content:"󰟇"}.mdi-storefront-check:before{content:"󱭽"}.mdi-storefront-check-outline:before{content:"󱭾"}.mdi-storefront-edit:before{content:"󱭿"}.mdi-storefront-edit-outline:before{content:"󱮀"}.mdi-storefront-minus:before{content:"󱮃"}.mdi-storefront-minus-outline:before{content:"󱮄"}.mdi-storefront-outline:before{content:"󱃁"}.mdi-storefront-plus:before{content:"󱮁"}.mdi-storefront-plus-outline:before{content:"󱮂"}.mdi-storefront-remove:before{content:"󱮅"}.mdi-storefront-remove-outline:before{content:"󱮆"}.mdi-stove:before{content:"󰓞"}.mdi-strategy:before{content:"󱇖"}.mdi-stretch-to-page:before{content:"󰼫"}.mdi-stretch-to-page-outline:before{content:"󰼬"}.mdi-string-lights:before{content:"󱊺"}.mdi-string-lights-off:before{content:"󱊻"}.mdi-subdirectory-arrow-left:before{content:"󰘌"}.mdi-subdirectory-arrow-right:before{content:"󰘍"}.mdi-submarine:before{content:"󱕬"}.mdi-subtitles:before{content:"󰨖"}.mdi-subtitles-outline:before{content:"󰨗"}.mdi-subway:before{content:"󰚬"}.mdi-subway-alert-variant:before{content:"󰶝"}.mdi-subway-variant:before{content:"󰓟"}.mdi-summit:before{content:"󰞆"}.mdi-sun-angle:before{content:"󱬧"}.mdi-sun-angle-outline:before{content:"󱬨"}.mdi-sun-clock:before{content:"󱩷"}.mdi-sun-clock-outline:before{content:"󱩸"}.mdi-sun-compass:before{content:"󱦥"}.mdi-sun-snowflake:before{content:"󱞖"}.mdi-sun-snowflake-variant:before{content:"󱩹"}.mdi-sun-thermometer:before{content:"󱣖"}.mdi-sun-thermometer-outline:before{content:"󱣗"}.mdi-sun-wireless:before{content:"󱟾"}.mdi-sun-wireless-outline:before{content:"󱟿"}.mdi-sunglasses:before{content:"󰓠"}.mdi-surfing:before{content:"󱝆"}.mdi-surround-sound:before{content:"󰗅"}.mdi-surround-sound-2-0:before{content:"󰟰"}.mdi-surround-sound-2-1:before{content:"󱜩"}.mdi-surround-sound-3-1:before{content:"󰟱"}.mdi-surround-sound-5-1:before{content:"󰟲"}.mdi-surround-sound-5-1-2:before{content:"󱜪"}.mdi-surround-sound-7-1:before{content:"󰟳"}.mdi-svg:before{content:"󰜡"}.mdi-swap-horizontal:before{content:"󰓡"}.mdi-swap-horizontal-bold:before{content:"󰯍"}.mdi-swap-horizontal-circle:before{content:"󰿡"}.mdi-swap-horizontal-circle-outline:before{content:"󰿢"}.mdi-swap-horizontal-variant:before{content:"󰣁"}.mdi-swap-vertical:before{content:"󰓢"}.mdi-swap-vertical-bold:before{content:"󰯎"}.mdi-swap-vertical-circle:before{content:"󰿣"}.mdi-swap-vertical-circle-outline:before{content:"󰿤"}.mdi-swap-vertical-variant:before{content:"󰣂"}.mdi-swim:before{content:"󰓣"}.mdi-switch:before{content:"󰓤"}.mdi-sword:before{content:"󰓥"}.mdi-sword-cross:before{content:"󰞇"}.mdi-syllabary-hangul:before{content:"󱌳"}.mdi-syllabary-hiragana:before{content:"󱌴"}.mdi-syllabary-katakana:before{content:"󱌵"}.mdi-syllabary-katakana-halfwidth:before{content:"󱌶"}.mdi-symbol:before{content:"󱔁"}.mdi-symfony:before{content:"󰫦"}.mdi-synagogue:before{content:"󱬄"}.mdi-synagogue-outline:before{content:"󱬅"}.mdi-sync:before{content:"󰓦"}.mdi-sync-alert:before{content:"󰓧"}.mdi-sync-circle:before{content:"󱍸"}.mdi-sync-off:before{content:"󰓨"}.mdi-tab:before{content:"󰓩"}.mdi-tab-minus:before{content:"󰭋"}.mdi-tab-plus:before{content:"󰝜"}.mdi-tab-remove:before{content:"󰭌"}.mdi-tab-search:before{content:"󱦞"}.mdi-tab-unselected:before{content:"󰓪"}.mdi-table:before{content:"󰓫"}.mdi-table-account:before{content:"󱎹"}.mdi-table-alert:before{content:"󱎺"}.mdi-table-arrow-down:before{content:"󱎻"}.mdi-table-arrow-left:before{content:"󱎼"}.mdi-table-arrow-right:before{content:"󱎽"}.mdi-table-arrow-up:before{content:"󱎾"}.mdi-table-border:before{content:"󰨘"}.mdi-table-cancel:before{content:"󱎿"}.mdi-table-chair:before{content:"󱁡"}.mdi-table-check:before{content:"󱏀"}.mdi-table-clock:before{content:"󱏁"}.mdi-table-cog:before{content:"󱏂"}.mdi-table-column:before{content:"󰠵"}.mdi-table-column-plus-after:before{content:"󰓬"}.mdi-table-column-plus-before:before{content:"󰓭"}.mdi-table-column-remove:before{content:"󰓮"}.mdi-table-column-width:before{content:"󰓯"}.mdi-table-edit:before{content:"󰓰"}.mdi-table-eye:before{content:"󱂔"}.mdi-table-eye-off:before{content:"󱏃"}.mdi-table-filter:before{content:"󱮌"}.mdi-table-furniture:before{content:"󰖼"}.mdi-table-headers-eye:before{content:"󱈝"}.mdi-table-headers-eye-off:before{content:"󱈞"}.mdi-table-heart:before{content:"󱏄"}.mdi-table-key:before{content:"󱏅"}.mdi-table-large:before{content:"󰓱"}.mdi-table-large-plus:before{content:"󰾇"}.mdi-table-large-remove:before{content:"󰾈"}.mdi-table-lock:before{content:"󱏆"}.mdi-table-merge-cells:before{content:"󰦦"}.mdi-table-minus:before{content:"󱏇"}.mdi-table-multiple:before{content:"󱏈"}.mdi-table-network:before{content:"󱏉"}.mdi-table-of-contents:before{content:"󰠶"}.mdi-table-off:before{content:"󱏊"}.mdi-table-picnic:before{content:"󱝃"}.mdi-table-pivot:before{content:"󱠼"}.mdi-table-plus:before{content:"󰩵"}.mdi-table-question:before{content:"󱬡"}.mdi-table-refresh:before{content:"󱎠"}.mdi-table-remove:before{content:"󰩶"}.mdi-table-row:before{content:"󰠷"}.mdi-table-row-height:before{content:"󰓲"}.mdi-table-row-plus-after:before{content:"󰓳"}.mdi-table-row-plus-before:before{content:"󰓴"}.mdi-table-row-remove:before{content:"󰓵"}.mdi-table-search:before{content:"󰤏"}.mdi-table-settings:before{content:"󰠸"}.mdi-table-split-cell:before{content:"󱐪"}.mdi-table-star:before{content:"󱏋"}.mdi-table-sync:before{content:"󱎡"}.mdi-table-tennis:before{content:"󰹨"}.mdi-tablet:before{content:"󰓶"}.mdi-tablet-cellphone:before{content:"󰦧"}.mdi-tablet-dashboard:before{content:"󰻎"}.mdi-taco:before{content:"󰝢"}.mdi-tag:before{content:"󰓹"}.mdi-tag-arrow-down:before{content:"󱜫"}.mdi-tag-arrow-down-outline:before{content:"󱜬"}.mdi-tag-arrow-left:before{content:"󱜭"}.mdi-tag-arrow-left-outline:before{content:"󱜮"}.mdi-tag-arrow-right:before{content:"󱜯"}.mdi-tag-arrow-right-outline:before{content:"󱜰"}.mdi-tag-arrow-up:before{content:"󱜱"}.mdi-tag-arrow-up-outline:before{content:"󱜲"}.mdi-tag-check:before{content:"󱩺"}.mdi-tag-check-outline:before{content:"󱩻"}.mdi-tag-faces:before{content:"󰓺"}.mdi-tag-heart:before{content:"󰚋"}.mdi-tag-heart-outline:before{content:"󰯏"}.mdi-tag-minus:before{content:"󰤐"}.mdi-tag-minus-outline:before{content:"󱈟"}.mdi-tag-multiple:before{content:"󰓻"}.mdi-tag-multiple-outline:before{content:"󱋷"}.mdi-tag-off:before{content:"󱈠"}.mdi-tag-off-outline:before{content:"󱈡"}.mdi-tag-outline:before{content:"󰓼"}.mdi-tag-plus:before{content:"󰜢"}.mdi-tag-plus-outline:before{content:"󱈢"}.mdi-tag-remove:before{content:"󰜣"}.mdi-tag-remove-outline:before{content:"󱈣"}.mdi-tag-search:before{content:"󱤇"}.mdi-tag-search-outline:before{content:"󱤈"}.mdi-tag-text:before{content:"󱈤"}.mdi-tag-text-outline:before{content:"󰓽"}.mdi-tailwind:before{content:"󱏿"}.mdi-tally-mark-1:before{content:"󱪼"}.mdi-tally-mark-2:before{content:"󱪽"}.mdi-tally-mark-3:before{content:"󱪾"}.mdi-tally-mark-4:before{content:"󱪿"}.mdi-tally-mark-5:before{content:"󱫀"}.mdi-tangram:before{content:"󰓸"}.mdi-tank:before{content:"󰴺"}.mdi-tanker-truck:before{content:"󰿥"}.mdi-tape-drive:before{content:"󱛟"}.mdi-tape-measure:before{content:"󰭍"}.mdi-target:before{content:"󰓾"}.mdi-target-account:before{content:"󰯐"}.mdi-target-variant:before{content:"󰩷"}.mdi-taxi:before{content:"󰓿"}.mdi-tea:before{content:"󰶞"}.mdi-tea-outline:before{content:"󰶟"}.mdi-teamviewer:before{content:"󰔀"}.mdi-teddy-bear:before{content:"󱣻"}.mdi-telescope:before{content:"󰭎"}.mdi-television:before{content:"󰔂"}.mdi-television-ambient-light:before{content:"󱍖"}.mdi-television-box:before{content:"󰠹"}.mdi-television-classic:before{content:"󰟴"}.mdi-television-classic-off:before{content:"󰠺"}.mdi-television-guide:before{content:"󰔃"}.mdi-television-off:before{content:"󰠻"}.mdi-television-pause:before{content:"󰾉"}.mdi-television-play:before{content:"󰻏"}.mdi-television-shimmer:before{content:"󱄐"}.mdi-television-speaker:before{content:"󱬛"}.mdi-television-speaker-off:before{content:"󱬜"}.mdi-television-stop:before{content:"󰾊"}.mdi-temperature-celsius:before{content:"󰔄"}.mdi-temperature-fahrenheit:before{content:"󰔅"}.mdi-temperature-kelvin:before{content:"󰔆"}.mdi-temple-buddhist:before{content:"󱬆"}.mdi-temple-buddhist-outline:before{content:"󱬇"}.mdi-temple-hindu:before{content:"󱬈"}.mdi-temple-hindu-outline:before{content:"󱬉"}.mdi-tennis:before{content:"󰶠"}.mdi-tennis-ball:before{content:"󰔇"}.mdi-tent:before{content:"󰔈"}.mdi-terraform:before{content:"󱁢"}.mdi-terrain:before{content:"󰔉"}.mdi-test-tube:before{content:"󰙨"}.mdi-test-tube-empty:before{content:"󰤑"}.mdi-test-tube-off:before{content:"󰤒"}.mdi-text:before{content:"󰦨"}.mdi-text-account:before{content:"󱕰"}.mdi-text-box:before{content:"󰈚"}.mdi-text-box-check:before{content:"󰺦"}.mdi-text-box-check-outline:before{content:"󰺧"}.mdi-text-box-edit:before{content:"󱩼"}.mdi-text-box-edit-outline:before{content:"󱩽"}.mdi-text-box-minus:before{content:"󰺨"}.mdi-text-box-minus-outline:before{content:"󰺩"}.mdi-text-box-multiple:before{content:"󰪷"}.mdi-text-box-multiple-outline:before{content:"󰪸"}.mdi-text-box-outline:before{content:"󰧭"}.mdi-text-box-plus:before{content:"󰺪"}.mdi-text-box-plus-outline:before{content:"󰺫"}.mdi-text-box-remove:before{content:"󰺬"}.mdi-text-box-remove-outline:before{content:"󰺭"}.mdi-text-box-search:before{content:"󰺮"}.mdi-text-box-search-outline:before{content:"󰺯"}.mdi-text-long:before{content:"󰦪"}.mdi-text-recognition:before{content:"󱄽"}.mdi-text-search:before{content:"󱎸"}.mdi-text-search-variant:before{content:"󱩾"}.mdi-text-shadow:before{content:"󰙩"}.mdi-text-short:before{content:"󰦩"}.mdi-texture:before{content:"󰔌"}.mdi-texture-box:before{content:"󰿦"}.mdi-theater:before{content:"󰔍"}.mdi-theme-light-dark:before{content:"󰔎"}.mdi-thermometer:before{content:"󰔏"}.mdi-thermometer-alert:before{content:"󰸁"}.mdi-thermometer-auto:before{content:"󱬏"}.mdi-thermometer-bluetooth:before{content:"󱢕"}.mdi-thermometer-check:before{content:"󱩿"}.mdi-thermometer-chevron-down:before{content:"󰸂"}.mdi-thermometer-chevron-up:before{content:"󰸃"}.mdi-thermometer-high:before{content:"󱃂"}.mdi-thermometer-lines:before{content:"󰔐"}.mdi-thermometer-low:before{content:"󱃃"}.mdi-thermometer-minus:before{content:"󰸄"}.mdi-thermometer-off:before{content:"󱔱"}.mdi-thermometer-plus:before{content:"󰸅"}.mdi-thermometer-probe:before{content:"󱬫"}.mdi-thermometer-probe-off:before{content:"󱬬"}.mdi-thermometer-water:before{content:"󱪀"}.mdi-thermostat:before{content:"󰎓"}.mdi-thermostat-auto:before{content:"󱬗"}.mdi-thermostat-box:before{content:"󰢑"}.mdi-thermostat-box-auto:before{content:"󱬘"}.mdi-thought-bubble:before{content:"󰟶"}.mdi-thought-bubble-outline:before{content:"󰟷"}.mdi-thumb-down:before{content:"󰔑"}.mdi-thumb-down-outline:before{content:"󰔒"}.mdi-thumb-up:before{content:"󰔓"}.mdi-thumb-up-outline:before{content:"󰔔"}.mdi-thumbs-up-down:before{content:"󰔕"}.mdi-thumbs-up-down-outline:before{content:"󱤔"}.mdi-ticket:before{content:"󰔖"}.mdi-ticket-account:before{content:"󰔗"}.mdi-ticket-confirmation:before{content:"󰔘"}.mdi-ticket-confirmation-outline:before{content:"󱎪"}.mdi-ticket-outline:before{content:"󰤓"}.mdi-ticket-percent:before{content:"󰜤"}.mdi-ticket-percent-outline:before{content:"󱐫"}.mdi-tie:before{content:"󰔙"}.mdi-tilde:before{content:"󰜥"}.mdi-tilde-off:before{content:"󱣳"}.mdi-timelapse:before{content:"󰔚"}.mdi-timeline:before{content:"󰯑"}.mdi-timeline-alert:before{content:"󰾕"}.mdi-timeline-alert-outline:before{content:"󰾘"}.mdi-timeline-check:before{content:"󱔲"}.mdi-timeline-check-outline:before{content:"󱔳"}.mdi-timeline-clock:before{content:"󱇻"}.mdi-timeline-clock-outline:before{content:"󱇼"}.mdi-timeline-minus:before{content:"󱔴"}.mdi-timeline-minus-outline:before{content:"󱔵"}.mdi-timeline-outline:before{content:"󰯒"}.mdi-timeline-plus:before{content:"󰾖"}.mdi-timeline-plus-outline:before{content:"󰾗"}.mdi-timeline-question:before{content:"󰾙"}.mdi-timeline-question-outline:before{content:"󰾚"}.mdi-timeline-remove:before{content:"󱔶"}.mdi-timeline-remove-outline:before{content:"󱔷"}.mdi-timeline-text:before{content:"󰯓"}.mdi-timeline-text-outline:before{content:"󰯔"}.mdi-timer:before{content:"󱎫"}.mdi-timer-10:before{content:"󰔜"}.mdi-timer-3:before{content:"󰔝"}.mdi-timer-alert:before{content:"󱫌"}.mdi-timer-alert-outline:before{content:"󱫍"}.mdi-timer-cancel:before{content:"󱫎"}.mdi-timer-cancel-outline:before{content:"󱫏"}.mdi-timer-check:before{content:"󱫐"}.mdi-timer-check-outline:before{content:"󱫑"}.mdi-timer-cog:before{content:"󱤥"}.mdi-timer-cog-outline:before{content:"󱤦"}.mdi-timer-edit:before{content:"󱫒"}.mdi-timer-edit-outline:before{content:"󱫓"}.mdi-timer-lock:before{content:"󱫔"}.mdi-timer-lock-open:before{content:"󱫕"}.mdi-timer-lock-open-outline:before{content:"󱫖"}.mdi-timer-lock-outline:before{content:"󱫗"}.mdi-timer-marker:before{content:"󱫘"}.mdi-timer-marker-outline:before{content:"󱫙"}.mdi-timer-minus:before{content:"󱫚"}.mdi-timer-minus-outline:before{content:"󱫛"}.mdi-timer-music:before{content:"󱫜"}.mdi-timer-music-outline:before{content:"󱫝"}.mdi-timer-off:before{content:"󱎬"}.mdi-timer-off-outline:before{content:"󰔞"}.mdi-timer-outline:before{content:"󰔛"}.mdi-timer-pause:before{content:"󱫞"}.mdi-timer-pause-outline:before{content:"󱫟"}.mdi-timer-play:before{content:"󱫠"}.mdi-timer-play-outline:before{content:"󱫡"}.mdi-timer-plus:before{content:"󱫢"}.mdi-timer-plus-outline:before{content:"󱫣"}.mdi-timer-refresh:before{content:"󱫤"}.mdi-timer-refresh-outline:before{content:"󱫥"}.mdi-timer-remove:before{content:"󱫦"}.mdi-timer-remove-outline:before{content:"󱫧"}.mdi-timer-sand:before{content:"󰔟"}.mdi-timer-sand-complete:before{content:"󱦟"}.mdi-timer-sand-empty:before{content:"󰚭"}.mdi-timer-sand-full:before{content:"󰞌"}.mdi-timer-sand-paused:before{content:"󱦠"}.mdi-timer-settings:before{content:"󱤣"}.mdi-timer-settings-outline:before{content:"󱤤"}.mdi-timer-star:before{content:"󱫨"}.mdi-timer-star-outline:before{content:"󱫩"}.mdi-timer-stop:before{content:"󱫪"}.mdi-timer-stop-outline:before{content:"󱫫"}.mdi-timer-sync:before{content:"󱫬"}.mdi-timer-sync-outline:before{content:"󱫭"}.mdi-timetable:before{content:"󰔠"}.mdi-tire:before{content:"󱢖"}.mdi-toaster:before{content:"󱁣"}.mdi-toaster-off:before{content:"󱆷"}.mdi-toaster-oven:before{content:"󰳓"}.mdi-toggle-switch:before{content:"󰔡"}.mdi-toggle-switch-off:before{content:"󰔢"}.mdi-toggle-switch-off-outline:before{content:"󰨙"}.mdi-toggle-switch-outline:before{content:"󰨚"}.mdi-toggle-switch-variant:before{content:"󱨥"}.mdi-toggle-switch-variant-off:before{content:"󱨦"}.mdi-toilet:before{content:"󰦫"}.mdi-toolbox:before{content:"󰦬"}.mdi-toolbox-outline:before{content:"󰦭"}.mdi-tools:before{content:"󱁤"}.mdi-tooltip:before{content:"󰔣"}.mdi-tooltip-account:before{content:"󰀌"}.mdi-tooltip-cellphone:before{content:"󱠻"}.mdi-tooltip-check:before{content:"󱕜"}.mdi-tooltip-check-outline:before{content:"󱕝"}.mdi-tooltip-edit:before{content:"󰔤"}.mdi-tooltip-edit-outline:before{content:"󱋅"}.mdi-tooltip-image:before{content:"󰔥"}.mdi-tooltip-image-outline:before{content:"󰯕"}.mdi-tooltip-minus:before{content:"󱕞"}.mdi-tooltip-minus-outline:before{content:"󱕟"}.mdi-tooltip-outline:before{content:"󰔦"}.mdi-tooltip-plus:before{content:"󰯖"}.mdi-tooltip-plus-outline:before{content:"󰔧"}.mdi-tooltip-remove:before{content:"󱕠"}.mdi-tooltip-remove-outline:before{content:"󱕡"}.mdi-tooltip-text:before{content:"󰔨"}.mdi-tooltip-text-outline:before{content:"󰯗"}.mdi-tooth:before{content:"󰣃"}.mdi-tooth-outline:before{content:"󰔩"}.mdi-toothbrush:before{content:"󱄩"}.mdi-toothbrush-electric:before{content:"󱄬"}.mdi-toothbrush-paste:before{content:"󱄪"}.mdi-torch:before{content:"󱘆"}.mdi-tortoise:before{content:"󰴻"}.mdi-toslink:before{content:"󱊸"}.mdi-tournament:before{content:"󰦮"}.mdi-tow-truck:before{content:"󰠼"}.mdi-tower-beach:before{content:"󰚁"}.mdi-tower-fire:before{content:"󰚂"}.mdi-town-hall:before{content:"󱡵"}.mdi-toy-brick:before{content:"󱊈"}.mdi-toy-brick-marker:before{content:"󱊉"}.mdi-toy-brick-marker-outline:before{content:"󱊊"}.mdi-toy-brick-minus:before{content:"󱊋"}.mdi-toy-brick-minus-outline:before{content:"󱊌"}.mdi-toy-brick-outline:before{content:"󱊍"}.mdi-toy-brick-plus:before{content:"󱊎"}.mdi-toy-brick-plus-outline:before{content:"󱊏"}.mdi-toy-brick-remove:before{content:"󱊐"}.mdi-toy-brick-remove-outline:before{content:"󱊑"}.mdi-toy-brick-search:before{content:"󱊒"}.mdi-toy-brick-search-outline:before{content:"󱊓"}.mdi-track-light:before{content:"󰤔"}.mdi-track-light-off:before{content:"󱬁"}.mdi-trackpad:before{content:"󰟸"}.mdi-trackpad-lock:before{content:"󰤳"}.mdi-tractor:before{content:"󰢒"}.mdi-tractor-variant:before{content:"󱓄"}.mdi-trademark:before{content:"󰩸"}.mdi-traffic-cone:before{content:"󱍼"}.mdi-traffic-light:before{content:"󰔫"}.mdi-traffic-light-outline:before{content:"󱠪"}.mdi-train:before{content:"󰔬"}.mdi-train-car:before{content:"󰯘"}.mdi-train-car-autorack:before{content:"󱬭"}.mdi-train-car-box:before{content:"󱬮"}.mdi-train-car-box-full:before{content:"󱬯"}.mdi-train-car-box-open:before{content:"󱬰"}.mdi-train-car-caboose:before{content:"󱬱"}.mdi-train-car-centerbeam:before{content:"󱬲"}.mdi-train-car-centerbeam-full:before{content:"󱬳"}.mdi-train-car-container:before{content:"󱬴"}.mdi-train-car-flatbed:before{content:"󱬵"}.mdi-train-car-flatbed-car:before{content:"󱬶"}.mdi-train-car-flatbed-tank:before{content:"󱬷"}.mdi-train-car-gondola:before{content:"󱬸"}.mdi-train-car-gondola-full:before{content:"󱬹"}.mdi-train-car-hopper:before{content:"󱬺"}.mdi-train-car-hopper-covered:before{content:"󱬻"}.mdi-train-car-hopper-full:before{content:"󱬼"}.mdi-train-car-intermodal:before{content:"󱬽"}.mdi-train-car-passenger:before{content:"󱜳"}.mdi-train-car-passenger-door:before{content:"󱜴"}.mdi-train-car-passenger-door-open:before{content:"󱜵"}.mdi-train-car-passenger-variant:before{content:"󱜶"}.mdi-train-car-tank:before{content:"󱬾"}.mdi-train-variant:before{content:"󰣄"}.mdi-tram:before{content:"󰔭"}.mdi-tram-side:before{content:"󰿧"}.mdi-transcribe:before{content:"󰔮"}.mdi-transcribe-close:before{content:"󰔯"}.mdi-transfer:before{content:"󱁥"}.mdi-transfer-down:before{content:"󰶡"}.mdi-transfer-left:before{content:"󰶢"}.mdi-transfer-right:before{content:"󰔰"}.mdi-transfer-up:before{content:"󰶣"}.mdi-transit-connection:before{content:"󰴼"}.mdi-transit-connection-horizontal:before{content:"󱕆"}.mdi-transit-connection-variant:before{content:"󰴽"}.mdi-transit-detour:before{content:"󰾋"}.mdi-transit-skip:before{content:"󱔕"}.mdi-transit-transfer:before{content:"󰚮"}.mdi-transition:before{content:"󰤕"}.mdi-transition-masked:before{content:"󰤖"}.mdi-translate:before{content:"󰗊"}.mdi-translate-off:before{content:"󰸆"}.mdi-translate-variant:before{content:"󱮙"}.mdi-transmission-tower:before{content:"󰴾"}.mdi-transmission-tower-export:before{content:"󱤬"}.mdi-transmission-tower-import:before{content:"󱤭"}.mdi-transmission-tower-off:before{content:"󱧝"}.mdi-trash-can:before{content:"󰩹"}.mdi-trash-can-outline:before{content:"󰩺"}.mdi-tray:before{content:"󱊔"}.mdi-tray-alert:before{content:"󱊕"}.mdi-tray-arrow-down:before{content:"󰄠"}.mdi-tray-arrow-up:before{content:"󰄝"}.mdi-tray-full:before{content:"󱊖"}.mdi-tray-minus:before{content:"󱊗"}.mdi-tray-plus:before{content:"󱊘"}.mdi-tray-remove:before{content:"󱊙"}.mdi-treasure-chest:before{content:"󰜦"}.mdi-tree:before{content:"󰔱"}.mdi-tree-outline:before{content:"󰹩"}.mdi-trello:before{content:"󰔲"}.mdi-trending-down:before{content:"󰔳"}.mdi-trending-neutral:before{content:"󰔴"}.mdi-trending-up:before{content:"󰔵"}.mdi-triangle:before{content:"󰔶"}.mdi-triangle-outline:before{content:"󰔷"}.mdi-triangle-small-down:before{content:"󱨉"}.mdi-triangle-small-up:before{content:"󱨊"}.mdi-triangle-wave:before{content:"󱑼"}.mdi-triforce:before{content:"󰯙"}.mdi-trophy:before{content:"󰔸"}.mdi-trophy-award:before{content:"󰔹"}.mdi-trophy-broken:before{content:"󰶤"}.mdi-trophy-outline:before{content:"󰔺"}.mdi-trophy-variant:before{content:"󰔻"}.mdi-trophy-variant-outline:before{content:"󰔼"}.mdi-truck:before{content:"󰔽"}.mdi-truck-alert:before{content:"󱧞"}.mdi-truck-alert-outline:before{content:"󱧟"}.mdi-truck-cargo-container:before{content:"󱣘"}.mdi-truck-check:before{content:"󰳔"}.mdi-truck-check-outline:before{content:"󱊚"}.mdi-truck-delivery:before{content:"󰔾"}.mdi-truck-delivery-outline:before{content:"󱊛"}.mdi-truck-fast:before{content:"󰞈"}.mdi-truck-fast-outline:before{content:"󱊜"}.mdi-truck-flatbed:before{content:"󱢑"}.mdi-truck-minus:before{content:"󱦮"}.mdi-truck-minus-outline:before{content:"󱦽"}.mdi-truck-outline:before{content:"󱊝"}.mdi-truck-plus:before{content:"󱦭"}.mdi-truck-plus-outline:before{content:"󱦼"}.mdi-truck-remove:before{content:"󱦯"}.mdi-truck-remove-outline:before{content:"󱦾"}.mdi-truck-snowflake:before{content:"󱦦"}.mdi-truck-trailer:before{content:"󰜧"}.mdi-trumpet:before{content:"󱂖"}.mdi-tshirt-crew:before{content:"󰩻"}.mdi-tshirt-crew-outline:before{content:"󰔿"}.mdi-tshirt-v:before{content:"󰩼"}.mdi-tshirt-v-outline:before{content:"󰕀"}.mdi-tsunami:before{content:"󱪁"}.mdi-tumble-dryer:before{content:"󰤗"}.mdi-tumble-dryer-alert:before{content:"󱆺"}.mdi-tumble-dryer-off:before{content:"󱆻"}.mdi-tune:before{content:"󰘮"}.mdi-tune-variant:before{content:"󱕂"}.mdi-tune-vertical:before{content:"󰙪"}.mdi-tune-vertical-variant:before{content:"󱕃"}.mdi-tunnel:before{content:"󱠽"}.mdi-tunnel-outline:before{content:"󱠾"}.mdi-turbine:before{content:"󱪂"}.mdi-turkey:before{content:"󱜛"}.mdi-turnstile:before{content:"󰳕"}.mdi-turnstile-outline:before{content:"󰳖"}.mdi-turtle:before{content:"󰳗"}.mdi-twitch:before{content:"󰕃"}.mdi-twitter:before{content:"󰕄"}.mdi-two-factor-authentication:before{content:"󰦯"}.mdi-typewriter:before{content:"󰼭"}.mdi-ubisoft:before{content:"󰯚"}.mdi-ubuntu:before{content:"󰕈"}.mdi-ufo:before{content:"󱃄"}.mdi-ufo-outline:before{content:"󱃅"}.mdi-ultra-high-definition:before{content:"󰟹"}.mdi-umbraco:before{content:"󰕉"}.mdi-umbrella:before{content:"󰕊"}.mdi-umbrella-beach:before{content:"󱢊"}.mdi-umbrella-beach-outline:before{content:"󱢋"}.mdi-umbrella-closed:before{content:"󰦰"}.mdi-umbrella-closed-outline:before{content:"󱏢"}.mdi-umbrella-closed-variant:before{content:"󱏡"}.mdi-umbrella-outline:before{content:"󰕋"}.mdi-undo:before{content:"󰕌"}.mdi-undo-variant:before{content:"󰕍"}.mdi-unfold-less-horizontal:before{content:"󰕎"}.mdi-unfold-less-vertical:before{content:"󰝠"}.mdi-unfold-more-horizontal:before{content:"󰕏"}.mdi-unfold-more-vertical:before{content:"󰝡"}.mdi-ungroup:before{content:"󰕐"}.mdi-unicode:before{content:"󰻐"}.mdi-unicorn:before{content:"󱗂"}.mdi-unicorn-variant:before{content:"󱗃"}.mdi-unicycle:before{content:"󱗥"}.mdi-unity:before{content:"󰚯"}.mdi-unreal:before{content:"󰦱"}.mdi-update:before{content:"󰚰"}.mdi-upload:before{content:"󰕒"}.mdi-upload-lock:before{content:"󱍳"}.mdi-upload-lock-outline:before{content:"󱍴"}.mdi-upload-multiple:before{content:"󰠽"}.mdi-upload-network:before{content:"󰛶"}.mdi-upload-network-outline:before{content:"󰳘"}.mdi-upload-off:before{content:"󱃆"}.mdi-upload-off-outline:before{content:"󱃇"}.mdi-upload-outline:before{content:"󰸇"}.mdi-usb:before{content:"󰕓"}.mdi-usb-flash-drive:before{content:"󱊞"}.mdi-usb-flash-drive-outline:before{content:"󱊟"}.mdi-usb-port:before{content:"󱇰"}.mdi-vacuum:before{content:"󱦡"}.mdi-vacuum-outline:before{content:"󱦢"}.mdi-valve:before{content:"󱁦"}.mdi-valve-closed:before{content:"󱁧"}.mdi-valve-open:before{content:"󱁨"}.mdi-van-passenger:before{content:"󰟺"}.mdi-van-utility:before{content:"󰟻"}.mdi-vanish:before{content:"󰟼"}.mdi-vanish-quarter:before{content:"󱕔"}.mdi-vanity-light:before{content:"󱇡"}.mdi-variable:before{content:"󰫧"}.mdi-variable-box:before{content:"󱄑"}.mdi-vector-arrange-above:before{content:"󰕔"}.mdi-vector-arrange-below:before{content:"󰕕"}.mdi-vector-bezier:before{content:"󰫨"}.mdi-vector-circle:before{content:"󰕖"}.mdi-vector-circle-variant:before{content:"󰕗"}.mdi-vector-combine:before{content:"󰕘"}.mdi-vector-curve:before{content:"󰕙"}.mdi-vector-difference:before{content:"󰕚"}.mdi-vector-difference-ab:before{content:"󰕛"}.mdi-vector-difference-ba:before{content:"󰕜"}.mdi-vector-ellipse:before{content:"󰢓"}.mdi-vector-intersection:before{content:"󰕝"}.mdi-vector-line:before{content:"󰕞"}.mdi-vector-link:before{content:"󰿨"}.mdi-vector-point:before{content:"󰇄"}.mdi-vector-point-edit:before{content:"󰧨"}.mdi-vector-point-minus:before{content:"󱭸"}.mdi-vector-point-plus:before{content:"󱭹"}.mdi-vector-point-select:before{content:"󰕟"}.mdi-vector-polygon:before{content:"󰕠"}.mdi-vector-polygon-variant:before{content:"󱡖"}.mdi-vector-polyline:before{content:"󰕡"}.mdi-vector-polyline-edit:before{content:"󱈥"}.mdi-vector-polyline-minus:before{content:"󱈦"}.mdi-vector-polyline-plus:before{content:"󱈧"}.mdi-vector-polyline-remove:before{content:"󱈨"}.mdi-vector-radius:before{content:"󰝊"}.mdi-vector-rectangle:before{content:"󰗆"}.mdi-vector-selection:before{content:"󰕢"}.mdi-vector-square:before{content:"󰀁"}.mdi-vector-square-close:before{content:"󱡗"}.mdi-vector-square-edit:before{content:"󱣙"}.mdi-vector-square-minus:before{content:"󱣚"}.mdi-vector-square-open:before{content:"󱡘"}.mdi-vector-square-plus:before{content:"󱣛"}.mdi-vector-square-remove:before{content:"󱣜"}.mdi-vector-triangle:before{content:"󰕣"}.mdi-vector-union:before{content:"󰕤"}.mdi-vhs:before{content:"󰨛"}.mdi-vibrate:before{content:"󰕦"}.mdi-vibrate-off:before{content:"󰳙"}.mdi-video:before{content:"󰕧"}.mdi-video-2d:before{content:"󱨜"}.mdi-video-3d:before{content:"󰟽"}.mdi-video-3d-off:before{content:"󱏙"}.mdi-video-3d-variant:before{content:"󰻑"}.mdi-video-4k-box:before{content:"󰠾"}.mdi-video-account:before{content:"󰤙"}.mdi-video-box:before{content:"󰃽"}.mdi-video-box-off:before{content:"󰃾"}.mdi-video-check:before{content:"󱁩"}.mdi-video-check-outline:before{content:"󱁪"}.mdi-video-high-definition:before{content:"󱔮"}.mdi-video-image:before{content:"󰤚"}.mdi-video-input-antenna:before{content:"󰠿"}.mdi-video-input-component:before{content:"󰡀"}.mdi-video-input-hdmi:before{content:"󰡁"}.mdi-video-input-scart:before{content:"󰾌"}.mdi-video-input-svideo:before{content:"󰡂"}.mdi-video-marker:before{content:"󱦩"}.mdi-video-marker-outline:before{content:"󱦪"}.mdi-video-minus:before{content:"󰦲"}.mdi-video-minus-outline:before{content:"󰊺"}.mdi-video-off:before{content:"󰕨"}.mdi-video-off-outline:before{content:"󰯛"}.mdi-video-outline:before{content:"󰯜"}.mdi-video-plus:before{content:"󰦳"}.mdi-video-plus-outline:before{content:"󰇓"}.mdi-video-stabilization:before{content:"󰤛"}.mdi-video-switch:before{content:"󰕩"}.mdi-video-switch-outline:before{content:"󰞐"}.mdi-video-vintage:before{content:"󰨜"}.mdi-video-wireless:before{content:"󰻒"}.mdi-video-wireless-outline:before{content:"󰻓"}.mdi-view-agenda:before{content:"󰕪"}.mdi-view-agenda-outline:before{content:"󱇘"}.mdi-view-array:before{content:"󰕫"}.mdi-view-array-outline:before{content:"󱒅"}.mdi-view-carousel:before{content:"󰕬"}.mdi-view-carousel-outline:before{content:"󱒆"}.mdi-view-column:before{content:"󰕭"}.mdi-view-column-outline:before{content:"󱒇"}.mdi-view-comfy:before{content:"󰹪"}.mdi-view-comfy-outline:before{content:"󱒈"}.mdi-view-compact:before{content:"󰹫"}.mdi-view-compact-outline:before{content:"󰹬"}.mdi-view-dashboard:before{content:"󰕮"}.mdi-view-dashboard-edit:before{content:"󱥇"}.mdi-view-dashboard-edit-outline:before{content:"󱥈"}.mdi-view-dashboard-outline:before{content:"󰨝"}.mdi-view-dashboard-variant:before{content:"󰡃"}.mdi-view-dashboard-variant-outline:before{content:"󱒉"}.mdi-view-day:before{content:"󰕯"}.mdi-view-day-outline:before{content:"󱒊"}.mdi-view-gallery:before{content:"󱢈"}.mdi-view-gallery-outline:before{content:"󱢉"}.mdi-view-grid:before{content:"󰕰"}.mdi-view-grid-outline:before{content:"󱇙"}.mdi-view-grid-plus:before{content:"󰾍"}.mdi-view-grid-plus-outline:before{content:"󱇚"}.mdi-view-headline:before{content:"󰕱"}.mdi-view-list:before{content:"󰕲"}.mdi-view-list-outline:before{content:"󱒋"}.mdi-view-module:before{content:"󰕳"}.mdi-view-module-outline:before{content:"󱒌"}.mdi-view-parallel:before{content:"󰜨"}.mdi-view-parallel-outline:before{content:"󱒍"}.mdi-view-quilt:before{content:"󰕴"}.mdi-view-quilt-outline:before{content:"󱒎"}.mdi-view-sequential:before{content:"󰜩"}.mdi-view-sequential-outline:before{content:"󱒏"}.mdi-view-split-horizontal:before{content:"󰯋"}.mdi-view-split-vertical:before{content:"󰯌"}.mdi-view-stream:before{content:"󰕵"}.mdi-view-stream-outline:before{content:"󱒐"}.mdi-view-week:before{content:"󰕶"}.mdi-view-week-outline:before{content:"󱒑"}.mdi-vimeo:before{content:"󰕷"}.mdi-violin:before{content:"󰘏"}.mdi-virtual-reality:before{content:"󰢔"}.mdi-virus:before{content:"󱎶"}.mdi-virus-off:before{content:"󱣡"}.mdi-virus-off-outline:before{content:"󱣢"}.mdi-virus-outline:before{content:"󱎷"}.mdi-vlc:before{content:"󰕼"}.mdi-voicemail:before{content:"󰕽"}.mdi-volcano:before{content:"󱪃"}.mdi-volcano-outline:before{content:"󱪄"}.mdi-volleyball:before{content:"󰦴"}.mdi-volume-equal:before{content:"󱬐"}.mdi-volume-high:before{content:"󰕾"}.mdi-volume-low:before{content:"󰕿"}.mdi-volume-medium:before{content:"󰖀"}.mdi-volume-minus:before{content:"󰝞"}.mdi-volume-mute:before{content:"󰝟"}.mdi-volume-off:before{content:"󰖁"}.mdi-volume-plus:before{content:"󰝝"}.mdi-volume-source:before{content:"󱄠"}.mdi-volume-variant-off:before{content:"󰸈"}.mdi-volume-vibrate:before{content:"󱄡"}.mdi-vote:before{content:"󰨟"}.mdi-vote-outline:before{content:"󰨠"}.mdi-vpn:before{content:"󰖂"}.mdi-vuejs:before{content:"󰡄"}.mdi-vuetify:before{content:"󰹭"}.mdi-walk:before{content:"󰖃"}.mdi-wall:before{content:"󰟾"}.mdi-wall-fire:before{content:"󱨑"}.mdi-wall-sconce:before{content:"󰤜"}.mdi-wall-sconce-flat:before{content:"󰤝"}.mdi-wall-sconce-flat-outline:before{content:"󱟉"}.mdi-wall-sconce-flat-variant:before{content:"󰐜"}.mdi-wall-sconce-flat-variant-outline:before{content:"󱟊"}.mdi-wall-sconce-outline:before{content:"󱟋"}.mdi-wall-sconce-round:before{content:"󰝈"}.mdi-wall-sconce-round-outline:before{content:"󱟌"}.mdi-wall-sconce-round-variant:before{content:"󰤞"}.mdi-wall-sconce-round-variant-outline:before{content:"󱟍"}.mdi-wallet:before{content:"󰖄"}.mdi-wallet-giftcard:before{content:"󰖅"}.mdi-wallet-membership:before{content:"󰖆"}.mdi-wallet-outline:before{content:"󰯝"}.mdi-wallet-plus:before{content:"󰾎"}.mdi-wallet-plus-outline:before{content:"󰾏"}.mdi-wallet-travel:before{content:"󰖇"}.mdi-wallpaper:before{content:"󰸉"}.mdi-wan:before{content:"󰖈"}.mdi-wardrobe:before{content:"󰾐"}.mdi-wardrobe-outline:before{content:"󰾑"}.mdi-warehouse:before{content:"󰾁"}.mdi-washing-machine:before{content:"󰜪"}.mdi-washing-machine-alert:before{content:"󱆼"}.mdi-washing-machine-off:before{content:"󱆽"}.mdi-watch:before{content:"󰖉"}.mdi-watch-export:before{content:"󰖊"}.mdi-watch-export-variant:before{content:"󰢕"}.mdi-watch-import:before{content:"󰖋"}.mdi-watch-import-variant:before{content:"󰢖"}.mdi-watch-variant:before{content:"󰢗"}.mdi-watch-vibrate:before{content:"󰚱"}.mdi-watch-vibrate-off:before{content:"󰳚"}.mdi-water:before{content:"󰖌"}.mdi-water-alert:before{content:"󱔂"}.mdi-water-alert-outline:before{content:"󱔃"}.mdi-water-boiler:before{content:"󰾒"}.mdi-water-boiler-alert:before{content:"󱆳"}.mdi-water-boiler-auto:before{content:"󱮘"}.mdi-water-boiler-off:before{content:"󱆴"}.mdi-water-check:before{content:"󱔄"}.mdi-water-check-outline:before{content:"󱔅"}.mdi-water-circle:before{content:"󱠆"}.mdi-water-minus:before{content:"󱔆"}.mdi-water-minus-outline:before{content:"󱔇"}.mdi-water-off:before{content:"󰖍"}.mdi-water-off-outline:before{content:"󱔈"}.mdi-water-opacity:before{content:"󱡕"}.mdi-water-outline:before{content:"󰸊"}.mdi-water-percent:before{content:"󰖎"}.mdi-water-percent-alert:before{content:"󱔉"}.mdi-water-plus:before{content:"󱔊"}.mdi-water-plus-outline:before{content:"󱔋"}.mdi-water-polo:before{content:"󱊠"}.mdi-water-pump:before{content:"󰖏"}.mdi-water-pump-off:before{content:"󰾓"}.mdi-water-remove:before{content:"󱔌"}.mdi-water-remove-outline:before{content:"󱔍"}.mdi-water-sync:before{content:"󱟆"}.mdi-water-thermometer:before{content:"󱪅"}.mdi-water-thermometer-outline:before{content:"󱪆"}.mdi-water-well:before{content:"󱁫"}.mdi-water-well-outline:before{content:"󱁬"}.mdi-waterfall:before{content:"󱡉"}.mdi-watering-can:before{content:"󱒁"}.mdi-watering-can-outline:before{content:"󱒂"}.mdi-watermark:before{content:"󰘒"}.mdi-wave:before{content:"󰼮"}.mdi-waveform:before{content:"󱑽"}.mdi-waves:before{content:"󰞍"}.mdi-waves-arrow-left:before{content:"󱡙"}.mdi-waves-arrow-right:before{content:"󱡚"}.mdi-waves-arrow-up:before{content:"󱡛"}.mdi-waze:before{content:"󰯞"}.mdi-weather-cloudy:before{content:"󰖐"}.mdi-weather-cloudy-alert:before{content:"󰼯"}.mdi-weather-cloudy-arrow-right:before{content:"󰹮"}.mdi-weather-cloudy-clock:before{content:"󱣶"}.mdi-weather-dust:before{content:"󱭚"}.mdi-weather-fog:before{content:"󰖑"}.mdi-weather-hail:before{content:"󰖒"}.mdi-weather-hazy:before{content:"󰼰"}.mdi-weather-hurricane:before{content:"󰢘"}.mdi-weather-lightning:before{content:"󰖓"}.mdi-weather-lightning-rainy:before{content:"󰙾"}.mdi-weather-night:before{content:"󰖔"}.mdi-weather-night-partly-cloudy:before{content:"󰼱"}.mdi-weather-partly-cloudy:before{content:"󰖕"}.mdi-weather-partly-lightning:before{content:"󰼲"}.mdi-weather-partly-rainy:before{content:"󰼳"}.mdi-weather-partly-snowy:before{content:"󰼴"}.mdi-weather-partly-snowy-rainy:before{content:"󰼵"}.mdi-weather-pouring:before{content:"󰖖"}.mdi-weather-rainy:before{content:"󰖗"}.mdi-weather-snowy:before{content:"󰖘"}.mdi-weather-snowy-heavy:before{content:"󰼶"}.mdi-weather-snowy-rainy:before{content:"󰙿"}.mdi-weather-sunny:before{content:"󰖙"}.mdi-weather-sunny-alert:before{content:"󰼷"}.mdi-weather-sunny-off:before{content:"󱓤"}.mdi-weather-sunset:before{content:"󰖚"}.mdi-weather-sunset-down:before{content:"󰖛"}.mdi-weather-sunset-up:before{content:"󰖜"}.mdi-weather-tornado:before{content:"󰼸"}.mdi-weather-windy:before{content:"󰖝"}.mdi-weather-windy-variant:before{content:"󰖞"}.mdi-web:before{content:"󰖟"}.mdi-web-box:before{content:"󰾔"}.mdi-web-cancel:before{content:"󱞐"}.mdi-web-check:before{content:"󰞉"}.mdi-web-clock:before{content:"󱉊"}.mdi-web-minus:before{content:"󱂠"}.mdi-web-off:before{content:"󰪎"}.mdi-web-plus:before{content:"󰀳"}.mdi-web-refresh:before{content:"󱞑"}.mdi-web-remove:before{content:"󰕑"}.mdi-web-sync:before{content:"󱞒"}.mdi-webcam:before{content:"󰖠"}.mdi-webcam-off:before{content:"󱜷"}.mdi-webhook:before{content:"󰘯"}.mdi-webpack:before{content:"󰜫"}.mdi-webrtc:before{content:"󱉈"}.mdi-wechat:before{content:"󰘑"}.mdi-weight:before{content:"󰖡"}.mdi-weight-gram:before{content:"󰴿"}.mdi-weight-kilogram:before{content:"󰖢"}.mdi-weight-lifter:before{content:"󱅝"}.mdi-weight-pound:before{content:"󰦵"}.mdi-whatsapp:before{content:"󰖣"}.mdi-wheel-barrow:before{content:"󱓲"}.mdi-wheelchair:before{content:"󱪇"}.mdi-wheelchair-accessibility:before{content:"󰖤"}.mdi-whistle:before{content:"󰦶"}.mdi-whistle-outline:before{content:"󱊼"}.mdi-white-balance-auto:before{content:"󰖥"}.mdi-white-balance-incandescent:before{content:"󰖦"}.mdi-white-balance-iridescent:before{content:"󰖧"}.mdi-white-balance-sunny:before{content:"󰖨"}.mdi-widgets:before{content:"󰜬"}.mdi-widgets-outline:before{content:"󱍕"}.mdi-wifi:before{content:"󰖩"}.mdi-wifi-alert:before{content:"󱚵"}.mdi-wifi-arrow-down:before{content:"󱚶"}.mdi-wifi-arrow-left:before{content:"󱚷"}.mdi-wifi-arrow-left-right:before{content:"󱚸"}.mdi-wifi-arrow-right:before{content:"󱚹"}.mdi-wifi-arrow-up:before{content:"󱚺"}.mdi-wifi-arrow-up-down:before{content:"󱚻"}.mdi-wifi-cancel:before{content:"󱚼"}.mdi-wifi-check:before{content:"󱚽"}.mdi-wifi-cog:before{content:"󱚾"}.mdi-wifi-lock:before{content:"󱚿"}.mdi-wifi-lock-open:before{content:"󱛀"}.mdi-wifi-marker:before{content:"󱛁"}.mdi-wifi-minus:before{content:"󱛂"}.mdi-wifi-off:before{content:"󰖪"}.mdi-wifi-plus:before{content:"󱛃"}.mdi-wifi-refresh:before{content:"󱛄"}.mdi-wifi-remove:before{content:"󱛅"}.mdi-wifi-settings:before{content:"󱛆"}.mdi-wifi-star:before{content:"󰸋"}.mdi-wifi-strength-1:before{content:"󰤟"}.mdi-wifi-strength-1-alert:before{content:"󰤠"}.mdi-wifi-strength-1-lock:before{content:"󰤡"}.mdi-wifi-strength-1-lock-open:before{content:"󱛋"}.mdi-wifi-strength-2:before{content:"󰤢"}.mdi-wifi-strength-2-alert:before{content:"󰤣"}.mdi-wifi-strength-2-lock:before{content:"󰤤"}.mdi-wifi-strength-2-lock-open:before{content:"󱛌"}.mdi-wifi-strength-3:before{content:"󰤥"}.mdi-wifi-strength-3-alert:before{content:"󰤦"}.mdi-wifi-strength-3-lock:before{content:"󰤧"}.mdi-wifi-strength-3-lock-open:before{content:"󱛍"}.mdi-wifi-strength-4:before{content:"󰤨"}.mdi-wifi-strength-4-alert:before{content:"󰤩"}.mdi-wifi-strength-4-lock:before{content:"󰤪"}.mdi-wifi-strength-4-lock-open:before{content:"󱛎"}.mdi-wifi-strength-alert-outline:before{content:"󰤫"}.mdi-wifi-strength-lock-open-outline:before{content:"󱛏"}.mdi-wifi-strength-lock-outline:before{content:"󰤬"}.mdi-wifi-strength-off:before{content:"󰤭"}.mdi-wifi-strength-off-outline:before{content:"󰤮"}.mdi-wifi-strength-outline:before{content:"󰤯"}.mdi-wifi-sync:before{content:"󱛇"}.mdi-wikipedia:before{content:"󰖬"}.mdi-wind-power:before{content:"󱪈"}.mdi-wind-power-outline:before{content:"󱪉"}.mdi-wind-turbine:before{content:"󰶥"}.mdi-wind-turbine-alert:before{content:"󱦫"}.mdi-wind-turbine-check:before{content:"󱦬"}.mdi-window-close:before{content:"󰖭"}.mdi-window-closed:before{content:"󰖮"}.mdi-window-closed-variant:before{content:"󱇛"}.mdi-window-maximize:before{content:"󰖯"}.mdi-window-minimize:before{content:"󰖰"}.mdi-window-open:before{content:"󰖱"}.mdi-window-open-variant:before{content:"󱇜"}.mdi-window-restore:before{content:"󰖲"}.mdi-window-shutter:before{content:"󱄜"}.mdi-window-shutter-alert:before{content:"󱄝"}.mdi-window-shutter-auto:before{content:"󱮣"}.mdi-window-shutter-cog:before{content:"󱪊"}.mdi-window-shutter-open:before{content:"󱄞"}.mdi-window-shutter-settings:before{content:"󱪋"}.mdi-windsock:before{content:"󱗺"}.mdi-wiper:before{content:"󰫩"}.mdi-wiper-wash:before{content:"󰶦"}.mdi-wiper-wash-alert:before{content:"󱣟"}.mdi-wizard-hat:before{content:"󱑷"}.mdi-wordpress:before{content:"󰖴"}.mdi-wrap:before{content:"󰖶"}.mdi-wrap-disabled:before{content:"󰯟"}.mdi-wrench:before{content:"󰖷"}.mdi-wrench-check:before{content:"󱮏"}.mdi-wrench-check-outline:before{content:"󱮐"}.mdi-wrench-clock:before{content:"󱦣"}.mdi-wrench-clock-outline:before{content:"󱮓"}.mdi-wrench-cog:before{content:"󱮑"}.mdi-wrench-cog-outline:before{content:"󱮒"}.mdi-wrench-outline:before{content:"󰯠"}.mdi-xamarin:before{content:"󰡅"}.mdi-xml:before{content:"󰗀"}.mdi-xmpp:before{content:"󰟿"}.mdi-yahoo:before{content:"󰭏"}.mdi-yeast:before{content:"󰗁"}.mdi-yin-yang:before{content:"󰚀"}.mdi-yoga:before{content:"󱅼"}.mdi-youtube:before{content:"󰗃"}.mdi-youtube-gaming:before{content:"󰡈"}.mdi-youtube-studio:before{content:"󰡇"}.mdi-youtube-subscription:before{content:"󰵀"}.mdi-youtube-tv:before{content:"󰑈"}.mdi-yurt:before{content:"󱔖"}.mdi-z-wave:before{content:"󰫪"}.mdi-zend:before{content:"󰫫"}.mdi-zigbee:before{content:"󰵁"}.mdi-zip-box:before{content:"󰗄"}.mdi-zip-box-outline:before{content:"󰿺"}.mdi-zip-disk:before{content:"󰨣"}.mdi-zodiac-aquarius:before{content:"󰩽"}.mdi-zodiac-aries:before{content:"󰩾"}.mdi-zodiac-cancer:before{content:"󰩿"}.mdi-zodiac-capricorn:before{content:"󰪀"}.mdi-zodiac-gemini:before{content:"󰪁"}.mdi-zodiac-leo:before{content:"󰪂"}.mdi-zodiac-libra:before{content:"󰪃"}.mdi-zodiac-pisces:before{content:"󰪄"}.mdi-zodiac-sagittarius:before{content:"󰪅"}.mdi-zodiac-scorpio:before{content:"󰪆"}.mdi-zodiac-taurus:before{content:"󰪇"}.mdi-zodiac-virgo:before{content:"󰪈"}.mdi-blank:before{content:"";visibility:hidden}.mdi-18px.mdi-set,.mdi-18px.mdi:before{font-size:18px}.mdi-24px.mdi-set,.mdi-24px.mdi:before{font-size:24px}.mdi-36px.mdi-set,.mdi-36px.mdi:before{font-size:36px}.mdi-48px.mdi-set,.mdi-48px.mdi:before{font-size:48px}.mdi-dark:before{color:#0000008a}.mdi-dark.mdi-inactive:before{color:#00000042}.mdi-light:before{color:#fff}.mdi-light.mdi-inactive:before{color:#ffffff4d}.mdi-rotate-45:before{-webkit-transform:rotate(45deg);-ms-transform:rotate(45deg);transform:rotate(45deg)}.mdi-rotate-90:before{-webkit-transform:rotate(90deg);-ms-transform:rotate(90deg);transform:rotate(90deg)}.mdi-rotate-135:before{-webkit-transform:rotate(135deg);-ms-transform:rotate(135deg);transform:rotate(135deg)}.mdi-rotate-180:before{-webkit-transform:rotate(180deg);-ms-transform:rotate(180deg);transform:rotate(180deg)}.mdi-rotate-225:before{-webkit-transform:rotate(225deg);-ms-transform:rotate(225deg);transform:rotate(225deg)}.mdi-rotate-270:before{-webkit-transform:rotate(270deg);-ms-transform:rotate(270deg);transform:rotate(270deg)}.mdi-rotate-315:before{-webkit-transform:rotate(315deg);-ms-transform:rotate(315deg);transform:rotate(315deg)}.mdi-flip-h:before{-webkit-transform:scaleX(-1);transform:scaleX(-1);filter:FlipH;-ms-filter:"FlipH"}.mdi-flip-v:before{-webkit-transform:scaleY(-1);transform:scaleY(-1);filter:FlipV;-ms-filter:"FlipV"}.mdi-spin:before{-webkit-animation:mdi-spin 2s infinite linear;animation:mdi-spin 2s infinite linear}@-webkit-keyframes mdi-spin{0%{-webkit-transform:rotate(0deg);transform:rotate(0)}to{-webkit-transform:rotate(359deg);transform:rotate(359deg)}}@keyframes mdi-spin{0%{-webkit-transform:rotate(0deg);transform:rotate(0)}to{-webkit-transform:rotate(359deg);transform:rotate(359deg)}}@keyframes v-shake{59%{margin-left:0}60%,80%{margin-left:2px}70%,90%{margin-left:-2px}}.bg-black{background-color:#000!important;color:#fff!important}.bg-white{background-color:#fff!important;color:#000!important}.bg-transparent{background-color:transparent!important;color:currentColor!important}.bg-red{background-color:#f44336!important;color:#fff!important}.bg-red-lighten-5{background-color:#ffebee!important;color:#000!important}.bg-red-lighten-4{background-color:#ffcdd2!important;color:#000!important}.bg-red-lighten-3{background-color:#ef9a9a!important;color:#000!important}.bg-red-lighten-2{background-color:#e57373!important;color:#fff!important}.bg-red-lighten-1{background-color:#ef5350!important;color:#fff!important}.bg-red-darken-1{background-color:#e53935!important;color:#fff!important}.bg-red-darken-2{background-color:#d32f2f!important;color:#fff!important}.bg-red-darken-3{background-color:#c62828!important;color:#fff!important}.bg-red-darken-4{background-color:#b71c1c!important;color:#fff!important}.bg-red-accent-1{background-color:#ff8a80!important;color:#000!important}.bg-red-accent-2{background-color:#ff5252!important;color:#fff!important}.bg-red-accent-3{background-color:#ff1744!important;color:#fff!important}.bg-red-accent-4{background-color:#d50000!important;color:#fff!important}.bg-pink{background-color:#e91e63!important;color:#fff!important}.bg-pink-lighten-5{background-color:#fce4ec!important;color:#000!important}.bg-pink-lighten-4{background-color:#f8bbd0!important;color:#000!important}.bg-pink-lighten-3{background-color:#f48fb1!important;color:#000!important}.bg-pink-lighten-2{background-color:#f06292!important;color:#fff!important}.bg-pink-lighten-1{background-color:#ec407a!important;color:#fff!important}.bg-pink-darken-1{background-color:#d81b60!important;color:#fff!important}.bg-pink-darken-2{background-color:#c2185b!important;color:#fff!important}.bg-pink-darken-3{background-color:#ad1457!important;color:#fff!important}.bg-pink-darken-4{background-color:#880e4f!important;color:#fff!important}.bg-pink-accent-1{background-color:#ff80ab!important;color:#fff!important}.bg-pink-accent-2{background-color:#ff4081!important;color:#fff!important}.bg-pink-accent-3{background-color:#f50057!important;color:#fff!important}.bg-pink-accent-4{background-color:#c51162!important;color:#fff!important}.bg-purple{background-color:#9c27b0!important;color:#fff!important}.bg-purple-lighten-5{background-color:#f3e5f5!important;color:#000!important}.bg-purple-lighten-4{background-color:#e1bee7!important;color:#000!important}.bg-purple-lighten-3{background-color:#ce93d8!important;color:#fff!important}.bg-purple-lighten-2{background-color:#ba68c8!important;color:#fff!important}.bg-purple-lighten-1{background-color:#ab47bc!important;color:#fff!important}.bg-purple-darken-1{background-color:#8e24aa!important;color:#fff!important}.bg-purple-darken-2{background-color:#7b1fa2!important;color:#fff!important}.bg-purple-darken-3{background-color:#6a1b9a!important;color:#fff!important}.bg-purple-darken-4{background-color:#4a148c!important;color:#fff!important}.bg-purple-accent-1{background-color:#ea80fc!important;color:#fff!important}.bg-purple-accent-2{background-color:#e040fb!important;color:#fff!important}.bg-purple-accent-3{background-color:#d500f9!important;color:#fff!important}.bg-purple-accent-4{background-color:#a0f!important;color:#fff!important}.bg-deep-purple{background-color:#673ab7!important;color:#fff!important}.bg-deep-purple-lighten-5{background-color:#ede7f6!important;color:#000!important}.bg-deep-purple-lighten-4{background-color:#d1c4e9!important;color:#000!important}.bg-deep-purple-lighten-3{background-color:#b39ddb!important;color:#fff!important}.bg-deep-purple-lighten-2{background-color:#9575cd!important;color:#fff!important}.bg-deep-purple-lighten-1{background-color:#7e57c2!important;color:#fff!important}.bg-deep-purple-darken-1{background-color:#5e35b1!important;color:#fff!important}.bg-deep-purple-darken-2{background-color:#512da8!important;color:#fff!important}.bg-deep-purple-darken-3{background-color:#4527a0!important;color:#fff!important}.bg-deep-purple-darken-4{background-color:#311b92!important;color:#fff!important}.bg-deep-purple-accent-1{background-color:#b388ff!important;color:#fff!important}.bg-deep-purple-accent-2{background-color:#7c4dff!important;color:#fff!important}.bg-deep-purple-accent-3{background-color:#651fff!important;color:#fff!important}.bg-deep-purple-accent-4{background-color:#6200ea!important;color:#fff!important}.bg-indigo{background-color:#3f51b5!important;color:#fff!important}.bg-indigo-lighten-5{background-color:#e8eaf6!important;color:#000!important}.bg-indigo-lighten-4{background-color:#c5cae9!important;color:#000!important}.bg-indigo-lighten-3{background-color:#9fa8da!important;color:#fff!important}.bg-indigo-lighten-2{background-color:#7986cb!important;color:#fff!important}.bg-indigo-lighten-1{background-color:#5c6bc0!important;color:#fff!important}.bg-indigo-darken-1{background-color:#3949ab!important;color:#fff!important}.bg-indigo-darken-2{background-color:#303f9f!important;color:#fff!important}.bg-indigo-darken-3{background-color:#283593!important;color:#fff!important}.bg-indigo-darken-4{background-color:#1a237e!important;color:#fff!important}.bg-indigo-accent-1{background-color:#8c9eff!important;color:#fff!important}.bg-indigo-accent-2{background-color:#536dfe!important;color:#fff!important}.bg-indigo-accent-3{background-color:#3d5afe!important;color:#fff!important}.bg-indigo-accent-4{background-color:#304ffe!important;color:#fff!important}.bg-blue{background-color:#2196f3!important;color:#fff!important}.bg-blue-lighten-5{background-color:#e3f2fd!important;color:#000!important}.bg-blue-lighten-4{background-color:#bbdefb!important;color:#000!important}.bg-blue-lighten-3{background-color:#90caf9!important;color:#000!important}.bg-blue-lighten-2{background-color:#64b5f6!important;color:#000!important}.bg-blue-lighten-1{background-color:#42a5f5!important;color:#fff!important}.bg-blue-darken-1{background-color:#1e88e5!important;color:#fff!important}.bg-blue-darken-2{background-color:#1976d2!important;color:#fff!important}.bg-blue-darken-3{background-color:#1565c0!important;color:#fff!important}.bg-blue-darken-4{background-color:#0d47a1!important;color:#fff!important}.bg-blue-accent-1{background-color:#82b1ff!important;color:#000!important}.bg-blue-accent-2{background-color:#448aff!important;color:#fff!important}.bg-blue-accent-3{background-color:#2979ff!important;color:#fff!important}.bg-blue-accent-4{background-color:#2962ff!important;color:#fff!important}.bg-light-blue{background-color:#03a9f4!important;color:#fff!important}.bg-light-blue-lighten-5{background-color:#e1f5fe!important;color:#000!important}.bg-light-blue-lighten-4{background-color:#b3e5fc!important;color:#000!important}.bg-light-blue-lighten-3{background-color:#81d4fa!important;color:#000!important}.bg-light-blue-lighten-2{background-color:#4fc3f7!important;color:#000!important}.bg-light-blue-lighten-1{background-color:#29b6f6!important;color:#000!important}.bg-light-blue-darken-1{background-color:#039be5!important;color:#fff!important}.bg-light-blue-darken-2{background-color:#0288d1!important;color:#fff!important}.bg-light-blue-darken-3{background-color:#0277bd!important;color:#fff!important}.bg-light-blue-darken-4{background-color:#01579b!important;color:#fff!important}.bg-light-blue-accent-1{background-color:#80d8ff!important;color:#000!important}.bg-light-blue-accent-2{background-color:#40c4ff!important;color:#000!important}.bg-light-blue-accent-3{background-color:#00b0ff!important;color:#fff!important}.bg-light-blue-accent-4{background-color:#0091ea!important;color:#fff!important}.bg-cyan{background-color:#00bcd4!important;color:#000!important}.bg-cyan-lighten-5{background-color:#e0f7fa!important;color:#000!important}.bg-cyan-lighten-4{background-color:#b2ebf2!important;color:#000!important}.bg-cyan-lighten-3{background-color:#80deea!important;color:#000!important}.bg-cyan-lighten-2{background-color:#4dd0e1!important;color:#000!important}.bg-cyan-lighten-1{background-color:#26c6da!important;color:#000!important}.bg-cyan-darken-1{background-color:#00acc1!important;color:#fff!important}.bg-cyan-darken-2{background-color:#0097a7!important;color:#fff!important}.bg-cyan-darken-3{background-color:#00838f!important;color:#fff!important}.bg-cyan-darken-4{background-color:#006064!important;color:#fff!important}.bg-cyan-accent-1{background-color:#84ffff!important;color:#000!important}.bg-cyan-accent-2{background-color:#18ffff!important;color:#000!important}.bg-cyan-accent-3{background-color:#00e5ff!important;color:#000!important}.bg-cyan-accent-4{background-color:#00b8d4!important;color:#fff!important}.bg-teal{background-color:#009688!important;color:#fff!important}.bg-teal-lighten-5{background-color:#e0f2f1!important;color:#000!important}.bg-teal-lighten-4{background-color:#b2dfdb!important;color:#000!important}.bg-teal-lighten-3{background-color:#80cbc4!important;color:#000!important}.bg-teal-lighten-2{background-color:#4db6ac!important;color:#fff!important}.bg-teal-lighten-1{background-color:#26a69a!important;color:#fff!important}.bg-teal-darken-1{background-color:#00897b!important;color:#fff!important}.bg-teal-darken-2{background-color:#00796b!important;color:#fff!important}.bg-teal-darken-3{background-color:#00695c!important;color:#fff!important}.bg-teal-darken-4{background-color:#004d40!important;color:#fff!important}.bg-teal-accent-1{background-color:#a7ffeb!important;color:#000!important}.bg-teal-accent-2{background-color:#64ffda!important;color:#000!important}.bg-teal-accent-3{background-color:#1de9b6!important;color:#000!important}.bg-teal-accent-4{background-color:#00bfa5!important;color:#fff!important}.bg-green{background-color:#4caf50!important;color:#fff!important}.bg-green-lighten-5{background-color:#e8f5e9!important;color:#000!important}.bg-green-lighten-4{background-color:#c8e6c9!important;color:#000!important}.bg-green-lighten-3{background-color:#a5d6a7!important;color:#000!important}.bg-green-lighten-2{background-color:#81c784!important;color:#000!important}.bg-green-lighten-1{background-color:#66bb6a!important;color:#fff!important}.bg-green-darken-1{background-color:#43a047!important;color:#fff!important}.bg-green-darken-2{background-color:#388e3c!important;color:#fff!important}.bg-green-darken-3{background-color:#2e7d32!important;color:#fff!important}.bg-green-darken-4{background-color:#1b5e20!important;color:#fff!important}.bg-green-accent-1{background-color:#b9f6ca!important;color:#000!important}.bg-green-accent-2{background-color:#69f0ae!important;color:#000!important}.bg-green-accent-3{background-color:#00e676!important;color:#000!important}.bg-green-accent-4{background-color:#00c853!important;color:#000!important}.bg-light-green{background-color:#8bc34a!important;color:#000!important}.bg-light-green-lighten-5{background-color:#f1f8e9!important;color:#000!important}.bg-light-green-lighten-4{background-color:#dcedc8!important;color:#000!important}.bg-light-green-lighten-3{background-color:#c5e1a5!important;color:#000!important}.bg-light-green-lighten-2{background-color:#aed581!important;color:#000!important}.bg-light-green-lighten-1{background-color:#9ccc65!important;color:#000!important}.bg-light-green-darken-1{background-color:#7cb342!important;color:#fff!important}.bg-light-green-darken-2{background-color:#689f38!important;color:#fff!important}.bg-light-green-darken-3{background-color:#558b2f!important;color:#fff!important}.bg-light-green-darken-4{background-color:#33691e!important;color:#fff!important}.bg-light-green-accent-1{background-color:#ccff90!important;color:#000!important}.bg-light-green-accent-2{background-color:#b2ff59!important;color:#000!important}.bg-light-green-accent-3{background-color:#76ff03!important;color:#000!important}.bg-light-green-accent-4{background-color:#64dd17!important;color:#000!important}.bg-lime{background-color:#cddc39!important;color:#000!important}.bg-lime-lighten-5{background-color:#f9fbe7!important;color:#000!important}.bg-lime-lighten-4{background-color:#f0f4c3!important;color:#000!important}.bg-lime-lighten-3{background-color:#e6ee9c!important;color:#000!important}.bg-lime-lighten-2{background-color:#dce775!important;color:#000!important}.bg-lime-lighten-1{background-color:#d4e157!important;color:#000!important}.bg-lime-darken-1{background-color:#c0ca33!important;color:#000!important}.bg-lime-darken-2{background-color:#afb42b!important;color:#000!important}.bg-lime-darken-3{background-color:#9e9d24!important;color:#fff!important}.bg-lime-darken-4{background-color:#827717!important;color:#fff!important}.bg-lime-accent-1{background-color:#f4ff81!important;color:#000!important}.bg-lime-accent-2{background-color:#eeff41!important;color:#000!important}.bg-lime-accent-3{background-color:#c6ff00!important;color:#000!important}.bg-lime-accent-4{background-color:#aeea00!important;color:#000!important}.bg-yellow{background-color:#ffeb3b!important;color:#000!important}.bg-yellow-lighten-5{background-color:#fffde7!important;color:#000!important}.bg-yellow-lighten-4{background-color:#fff9c4!important;color:#000!important}.bg-yellow-lighten-3{background-color:#fff59d!important;color:#000!important}.bg-yellow-lighten-2{background-color:#fff176!important;color:#000!important}.bg-yellow-lighten-1{background-color:#ffee58!important;color:#000!important}.bg-yellow-darken-1{background-color:#fdd835!important;color:#000!important}.bg-yellow-darken-2{background-color:#fbc02d!important;color:#000!important}.bg-yellow-darken-3{background-color:#f9a825!important;color:#000!important}.bg-yellow-darken-4{background-color:#f57f17!important;color:#fff!important}.bg-yellow-accent-1{background-color:#ffff8d!important;color:#000!important}.bg-yellow-accent-2{background-color:#ff0!important;color:#000!important}.bg-yellow-accent-3{background-color:#ffea00!important;color:#000!important}.bg-yellow-accent-4{background-color:#ffd600!important;color:#000!important}.bg-amber{background-color:#ffc107!important;color:#000!important}.bg-amber-lighten-5{background-color:#fff8e1!important;color:#000!important}.bg-amber-lighten-4{background-color:#ffecb3!important;color:#000!important}.bg-amber-lighten-3{background-color:#ffe082!important;color:#000!important}.bg-amber-lighten-2{background-color:#ffd54f!important;color:#000!important}.bg-amber-lighten-1{background-color:#ffca28!important;color:#000!important}.bg-amber-darken-1{background-color:#ffb300!important;color:#000!important}.bg-amber-darken-2{background-color:#ffa000!important;color:#000!important}.bg-amber-darken-3{background-color:#ff8f00!important;color:#000!important}.bg-amber-darken-4{background-color:#ff6f00!important;color:#fff!important}.bg-amber-accent-1{background-color:#ffe57f!important;color:#000!important}.bg-amber-accent-2{background-color:#ffd740!important;color:#000!important}.bg-amber-accent-3{background-color:#ffc400!important;color:#000!important}.bg-amber-accent-4{background-color:#ffab00!important;color:#000!important}.bg-orange{background-color:#ff9800!important;color:#000!important}.bg-orange-lighten-5{background-color:#fff3e0!important;color:#000!important}.bg-orange-lighten-4{background-color:#ffe0b2!important;color:#000!important}.bg-orange-lighten-3{background-color:#ffcc80!important;color:#000!important}.bg-orange-lighten-2{background-color:#ffb74d!important;color:#000!important}.bg-orange-lighten-1{background-color:#ffa726!important;color:#000!important}.bg-orange-darken-1{background-color:#fb8c00!important;color:#fff!important}.bg-orange-darken-2{background-color:#f57c00!important;color:#fff!important}.bg-orange-darken-3{background-color:#ef6c00!important;color:#fff!important}.bg-orange-darken-4{background-color:#e65100!important;color:#fff!important}.bg-orange-accent-1{background-color:#ffd180!important;color:#000!important}.bg-orange-accent-2{background-color:#ffab40!important;color:#000!important}.bg-orange-accent-3{background-color:#ff9100!important;color:#000!important}.bg-orange-accent-4{background-color:#ff6d00!important;color:#fff!important}.bg-deep-orange{background-color:#ff5722!important;color:#fff!important}.bg-deep-orange-lighten-5{background-color:#fbe9e7!important;color:#000!important}.bg-deep-orange-lighten-4{background-color:#ffccbc!important;color:#000!important}.bg-deep-orange-lighten-3{background-color:#ffab91!important;color:#000!important}.bg-deep-orange-lighten-2{background-color:#ff8a65!important;color:#000!important}.bg-deep-orange-lighten-1{background-color:#ff7043!important;color:#fff!important}.bg-deep-orange-darken-1{background-color:#f4511e!important;color:#fff!important}.bg-deep-orange-darken-2{background-color:#e64a19!important;color:#fff!important}.bg-deep-orange-darken-3{background-color:#d84315!important;color:#fff!important}.bg-deep-orange-darken-4{background-color:#bf360c!important;color:#fff!important}.bg-deep-orange-accent-1{background-color:#ff9e80!important;color:#000!important}.bg-deep-orange-accent-2{background-color:#ff6e40!important;color:#fff!important}.bg-deep-orange-accent-3{background-color:#ff3d00!important;color:#fff!important}.bg-deep-orange-accent-4{background-color:#dd2c00!important;color:#fff!important}.bg-brown{background-color:#795548!important;color:#fff!important}.bg-brown-lighten-5{background-color:#efebe9!important;color:#000!important}.bg-brown-lighten-4{background-color:#d7ccc8!important;color:#000!important}.bg-brown-lighten-3{background-color:#bcaaa4!important;color:#000!important}.bg-brown-lighten-2{background-color:#a1887f!important;color:#fff!important}.bg-brown-lighten-1{background-color:#8d6e63!important;color:#fff!important}.bg-brown-darken-1{background-color:#6d4c41!important;color:#fff!important}.bg-brown-darken-2{background-color:#5d4037!important;color:#fff!important}.bg-brown-darken-3{background-color:#4e342e!important;color:#fff!important}.bg-brown-darken-4{background-color:#3e2723!important;color:#fff!important}.bg-blue-grey{background-color:#607d8b!important;color:#fff!important}.bg-blue-grey-lighten-5{background-color:#eceff1!important;color:#000!important}.bg-blue-grey-lighten-4{background-color:#cfd8dc!important;color:#000!important}.bg-blue-grey-lighten-3{background-color:#b0bec5!important;color:#000!important}.bg-blue-grey-lighten-2{background-color:#90a4ae!important;color:#fff!important}.bg-blue-grey-lighten-1{background-color:#78909c!important;color:#fff!important}.bg-blue-grey-darken-1{background-color:#546e7a!important;color:#fff!important}.bg-blue-grey-darken-2{background-color:#455a64!important;color:#fff!important}.bg-blue-grey-darken-3{background-color:#37474f!important;color:#fff!important}.bg-blue-grey-darken-4{background-color:#263238!important;color:#fff!important}.bg-grey{background-color:#9e9e9e!important;color:#fff!important}.bg-grey-lighten-5{background-color:#fafafa!important;color:#000!important}.bg-grey-lighten-4{background-color:#f5f5f5!important;color:#000!important}.bg-grey-lighten-3{background-color:#eee!important;color:#000!important}.bg-grey-lighten-2{background-color:#e0e0e0!important;color:#000!important}.bg-grey-lighten-1{background-color:#bdbdbd!important;color:#000!important}.bg-grey-darken-1{background-color:#757575!important;color:#fff!important}.bg-grey-darken-2{background-color:#616161!important;color:#fff!important}.bg-grey-darken-3{background-color:#424242!important;color:#fff!important}.bg-grey-darken-4{background-color:#212121!important;color:#fff!important}.bg-shades-black{background-color:#000!important;color:#fff!important}.bg-shades-white{background-color:#fff!important;color:#000!important}.bg-shades-transparent{background-color:transparent!important;color:currentColor!important}.text-black{color:#000!important}.text-white{color:#fff!important}.text-transparent{color:transparent!important}.text-red{color:#f44336!important}.text-red-lighten-5{color:#ffebee!important}.text-red-lighten-4{color:#ffcdd2!important}.text-red-lighten-3{color:#ef9a9a!important}.text-red-lighten-2{color:#e57373!important}.text-red-lighten-1{color:#ef5350!important}.text-red-darken-1{color:#e53935!important}.text-red-darken-2{color:#d32f2f!important}.text-red-darken-3{color:#c62828!important}.text-red-darken-4{color:#b71c1c!important}.text-red-accent-1{color:#ff8a80!important}.text-red-accent-2{color:#ff5252!important}.text-red-accent-3{color:#ff1744!important}.text-red-accent-4{color:#d50000!important}.text-pink{color:#e91e63!important}.text-pink-lighten-5{color:#fce4ec!important}.text-pink-lighten-4{color:#f8bbd0!important}.text-pink-lighten-3{color:#f48fb1!important}.text-pink-lighten-2{color:#f06292!important}.text-pink-lighten-1{color:#ec407a!important}.text-pink-darken-1{color:#d81b60!important}.text-pink-darken-2{color:#c2185b!important}.text-pink-darken-3{color:#ad1457!important}.text-pink-darken-4{color:#880e4f!important}.text-pink-accent-1{color:#ff80ab!important}.text-pink-accent-2{color:#ff4081!important}.text-pink-accent-3{color:#f50057!important}.text-pink-accent-4{color:#c51162!important}.text-purple{color:#9c27b0!important}.text-purple-lighten-5{color:#f3e5f5!important}.text-purple-lighten-4{color:#e1bee7!important}.text-purple-lighten-3{color:#ce93d8!important}.text-purple-lighten-2{color:#ba68c8!important}.text-purple-lighten-1{color:#ab47bc!important}.text-purple-darken-1{color:#8e24aa!important}.text-purple-darken-2{color:#7b1fa2!important}.text-purple-darken-3{color:#6a1b9a!important}.text-purple-darken-4{color:#4a148c!important}.text-purple-accent-1{color:#ea80fc!important}.text-purple-accent-2{color:#e040fb!important}.text-purple-accent-3{color:#d500f9!important}.text-purple-accent-4{color:#a0f!important}.text-deep-purple{color:#673ab7!important}.text-deep-purple-lighten-5{color:#ede7f6!important}.text-deep-purple-lighten-4{color:#d1c4e9!important}.text-deep-purple-lighten-3{color:#b39ddb!important}.text-deep-purple-lighten-2{color:#9575cd!important}.text-deep-purple-lighten-1{color:#7e57c2!important}.text-deep-purple-darken-1{color:#5e35b1!important}.text-deep-purple-darken-2{color:#512da8!important}.text-deep-purple-darken-3{color:#4527a0!important}.text-deep-purple-darken-4{color:#311b92!important}.text-deep-purple-accent-1{color:#b388ff!important}.text-deep-purple-accent-2{color:#7c4dff!important}.text-deep-purple-accent-3{color:#651fff!important}.text-deep-purple-accent-4{color:#6200ea!important}.text-indigo{color:#3f51b5!important}.text-indigo-lighten-5{color:#e8eaf6!important}.text-indigo-lighten-4{color:#c5cae9!important}.text-indigo-lighten-3{color:#9fa8da!important}.text-indigo-lighten-2{color:#7986cb!important}.text-indigo-lighten-1{color:#5c6bc0!important}.text-indigo-darken-1{color:#3949ab!important}.text-indigo-darken-2{color:#303f9f!important}.text-indigo-darken-3{color:#283593!important}.text-indigo-darken-4{color:#1a237e!important}.text-indigo-accent-1{color:#8c9eff!important}.text-indigo-accent-2{color:#536dfe!important}.text-indigo-accent-3{color:#3d5afe!important}.text-indigo-accent-4{color:#304ffe!important}.text-blue{color:#2196f3!important}.text-blue-lighten-5{color:#e3f2fd!important}.text-blue-lighten-4{color:#bbdefb!important}.text-blue-lighten-3{color:#90caf9!important}.text-blue-lighten-2{color:#64b5f6!important}.text-blue-lighten-1{color:#42a5f5!important}.text-blue-darken-1{color:#1e88e5!important}.text-blue-darken-2{color:#1976d2!important}.text-blue-darken-3{color:#1565c0!important}.text-blue-darken-4{color:#0d47a1!important}.text-blue-accent-1{color:#82b1ff!important}.text-blue-accent-2{color:#448aff!important}.text-blue-accent-3{color:#2979ff!important}.text-blue-accent-4{color:#2962ff!important}.text-light-blue{color:#03a9f4!important}.text-light-blue-lighten-5{color:#e1f5fe!important}.text-light-blue-lighten-4{color:#b3e5fc!important}.text-light-blue-lighten-3{color:#81d4fa!important}.text-light-blue-lighten-2{color:#4fc3f7!important}.text-light-blue-lighten-1{color:#29b6f6!important}.text-light-blue-darken-1{color:#039be5!important}.text-light-blue-darken-2{color:#0288d1!important}.text-light-blue-darken-3{color:#0277bd!important}.text-light-blue-darken-4{color:#01579b!important}.text-light-blue-accent-1{color:#80d8ff!important}.text-light-blue-accent-2{color:#40c4ff!important}.text-light-blue-accent-3{color:#00b0ff!important}.text-light-blue-accent-4{color:#0091ea!important}.text-cyan{color:#00bcd4!important}.text-cyan-lighten-5{color:#e0f7fa!important}.text-cyan-lighten-4{color:#b2ebf2!important}.text-cyan-lighten-3{color:#80deea!important}.text-cyan-lighten-2{color:#4dd0e1!important}.text-cyan-lighten-1{color:#26c6da!important}.text-cyan-darken-1{color:#00acc1!important}.text-cyan-darken-2{color:#0097a7!important}.text-cyan-darken-3{color:#00838f!important}.text-cyan-darken-4{color:#006064!important}.text-cyan-accent-1{color:#84ffff!important}.text-cyan-accent-2{color:#18ffff!important}.text-cyan-accent-3{color:#00e5ff!important}.text-cyan-accent-4{color:#00b8d4!important}.text-teal{color:#009688!important}.text-teal-lighten-5{color:#e0f2f1!important}.text-teal-lighten-4{color:#b2dfdb!important}.text-teal-lighten-3{color:#80cbc4!important}.text-teal-lighten-2{color:#4db6ac!important}.text-teal-lighten-1{color:#26a69a!important}.text-teal-darken-1{color:#00897b!important}.text-teal-darken-2{color:#00796b!important}.text-teal-darken-3{color:#00695c!important}.text-teal-darken-4{color:#004d40!important}.text-teal-accent-1{color:#a7ffeb!important}.text-teal-accent-2{color:#64ffda!important}.text-teal-accent-3{color:#1de9b6!important}.text-teal-accent-4{color:#00bfa5!important}.text-green{color:#4caf50!important}.text-green-lighten-5{color:#e8f5e9!important}.text-green-lighten-4{color:#c8e6c9!important}.text-green-lighten-3{color:#a5d6a7!important}.text-green-lighten-2{color:#81c784!important}.text-green-lighten-1{color:#66bb6a!important}.text-green-darken-1{color:#43a047!important}.text-green-darken-2{color:#388e3c!important}.text-green-darken-3{color:#2e7d32!important}.text-green-darken-4{color:#1b5e20!important}.text-green-accent-1{color:#b9f6ca!important}.text-green-accent-2{color:#69f0ae!important}.text-green-accent-3{color:#00e676!important}.text-green-accent-4{color:#00c853!important}.text-light-green{color:#8bc34a!important}.text-light-green-lighten-5{color:#f1f8e9!important}.text-light-green-lighten-4{color:#dcedc8!important}.text-light-green-lighten-3{color:#c5e1a5!important}.text-light-green-lighten-2{color:#aed581!important}.text-light-green-lighten-1{color:#9ccc65!important}.text-light-green-darken-1{color:#7cb342!important}.text-light-green-darken-2{color:#689f38!important}.text-light-green-darken-3{color:#558b2f!important}.text-light-green-darken-4{color:#33691e!important}.text-light-green-accent-1{color:#ccff90!important}.text-light-green-accent-2{color:#b2ff59!important}.text-light-green-accent-3{color:#76ff03!important}.text-light-green-accent-4{color:#64dd17!important}.text-lime{color:#cddc39!important}.text-lime-lighten-5{color:#f9fbe7!important}.text-lime-lighten-4{color:#f0f4c3!important}.text-lime-lighten-3{color:#e6ee9c!important}.text-lime-lighten-2{color:#dce775!important}.text-lime-lighten-1{color:#d4e157!important}.text-lime-darken-1{color:#c0ca33!important}.text-lime-darken-2{color:#afb42b!important}.text-lime-darken-3{color:#9e9d24!important}.text-lime-darken-4{color:#827717!important}.text-lime-accent-1{color:#f4ff81!important}.text-lime-accent-2{color:#eeff41!important}.text-lime-accent-3{color:#c6ff00!important}.text-lime-accent-4{color:#aeea00!important}.text-yellow{color:#ffeb3b!important}.text-yellow-lighten-5{color:#fffde7!important}.text-yellow-lighten-4{color:#fff9c4!important}.text-yellow-lighten-3{color:#fff59d!important}.text-yellow-lighten-2{color:#fff176!important}.text-yellow-lighten-1{color:#ffee58!important}.text-yellow-darken-1{color:#fdd835!important}.text-yellow-darken-2{color:#fbc02d!important}.text-yellow-darken-3{color:#f9a825!important}.text-yellow-darken-4{color:#f57f17!important}.text-yellow-accent-1{color:#ffff8d!important}.text-yellow-accent-2{color:#ff0!important}.text-yellow-accent-3{color:#ffea00!important}.text-yellow-accent-4{color:#ffd600!important}.text-amber{color:#ffc107!important}.text-amber-lighten-5{color:#fff8e1!important}.text-amber-lighten-4{color:#ffecb3!important}.text-amber-lighten-3{color:#ffe082!important}.text-amber-lighten-2{color:#ffd54f!important}.text-amber-lighten-1{color:#ffca28!important}.text-amber-darken-1{color:#ffb300!important}.text-amber-darken-2{color:#ffa000!important}.text-amber-darken-3{color:#ff8f00!important}.text-amber-darken-4{color:#ff6f00!important}.text-amber-accent-1{color:#ffe57f!important}.text-amber-accent-2{color:#ffd740!important}.text-amber-accent-3{color:#ffc400!important}.text-amber-accent-4{color:#ffab00!important}.text-orange{color:#ff9800!important}.text-orange-lighten-5{color:#fff3e0!important}.text-orange-lighten-4{color:#ffe0b2!important}.text-orange-lighten-3{color:#ffcc80!important}.text-orange-lighten-2{color:#ffb74d!important}.text-orange-lighten-1{color:#ffa726!important}.text-orange-darken-1{color:#fb8c00!important}.text-orange-darken-2{color:#f57c00!important}.text-orange-darken-3{color:#ef6c00!important}.text-orange-darken-4{color:#e65100!important}.text-orange-accent-1{color:#ffd180!important}.text-orange-accent-2{color:#ffab40!important}.text-orange-accent-3{color:#ff9100!important}.text-orange-accent-4{color:#ff6d00!important}.text-deep-orange{color:#ff5722!important}.text-deep-orange-lighten-5{color:#fbe9e7!important}.text-deep-orange-lighten-4{color:#ffccbc!important}.text-deep-orange-lighten-3{color:#ffab91!important}.text-deep-orange-lighten-2{color:#ff8a65!important}.text-deep-orange-lighten-1{color:#ff7043!important}.text-deep-orange-darken-1{color:#f4511e!important}.text-deep-orange-darken-2{color:#e64a19!important}.text-deep-orange-darken-3{color:#d84315!important}.text-deep-orange-darken-4{color:#bf360c!important}.text-deep-orange-accent-1{color:#ff9e80!important}.text-deep-orange-accent-2{color:#ff6e40!important}.text-deep-orange-accent-3{color:#ff3d00!important}.text-deep-orange-accent-4{color:#dd2c00!important}.text-brown{color:#795548!important}.text-brown-lighten-5{color:#efebe9!important}.text-brown-lighten-4{color:#d7ccc8!important}.text-brown-lighten-3{color:#bcaaa4!important}.text-brown-lighten-2{color:#a1887f!important}.text-brown-lighten-1{color:#8d6e63!important}.text-brown-darken-1{color:#6d4c41!important}.text-brown-darken-2{color:#5d4037!important}.text-brown-darken-3{color:#4e342e!important}.text-brown-darken-4{color:#3e2723!important}.text-blue-grey{color:#607d8b!important}.text-blue-grey-lighten-5{color:#eceff1!important}.text-blue-grey-lighten-4{color:#cfd8dc!important}.text-blue-grey-lighten-3{color:#b0bec5!important}.text-blue-grey-lighten-2{color:#90a4ae!important}.text-blue-grey-lighten-1{color:#78909c!important}.text-blue-grey-darken-1{color:#546e7a!important}.text-blue-grey-darken-2{color:#455a64!important}.text-blue-grey-darken-3{color:#37474f!important}.text-blue-grey-darken-4{color:#263238!important}.text-grey{color:#9e9e9e!important}.text-grey-lighten-5{color:#fafafa!important}.text-grey-lighten-4{color:#f5f5f5!important}.text-grey-lighten-3{color:#eee!important}.text-grey-lighten-2{color:#e0e0e0!important}.text-grey-lighten-1{color:#bdbdbd!important}.text-grey-darken-1{color:#757575!important}.text-grey-darken-2{color:#616161!important}.text-grey-darken-3{color:#424242!important}.text-grey-darken-4{color:#212121!important}.text-shades-black{color:#000!important}.text-shades-white{color:#fff!important}.text-shades-transparent{color:transparent!important}/*!
  * ress.css • v2.0.4
  * MIT License
  * github.com/filipelinhares/ress
```

### Comparing `django_customvueadmin-0.2.5/custom_admin/static/custom_admin/materialdesignicons-webfont-CYDMK1kx.woff2` & `django_customvueadmin-0.2.6/custom_admin/static/custom_admin/materialdesignicons-webfont-CYDMK1kx.woff2`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/static/custom_admin/materialdesignicons-webfont-CgCzGbLl.woff` & `django_customvueadmin-0.2.6/custom_admin/static/custom_admin/materialdesignicons-webfont-CgCzGbLl.woff`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/static/custom_admin/materialdesignicons-webfont-D3kAzl71.ttf` & `django_customvueadmin-0.2.6/custom_admin/static/custom_admin/materialdesignicons-webfont-D3kAzl71.ttf`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/static/custom_admin/materialdesignicons-webfont-DttUABo4.eot` & `django_customvueadmin-0.2.6/custom_admin/static/custom_admin/materialdesignicons-webfont-DttUABo4.eot`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/dark-first/content.min.css` & `django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/dark-first/content.min.css`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/dark-first/skin.min.css` & `django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/dark-first/skin.min.css`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/dark-slim/content.min.css` & `django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/dark-slim/content.min.css`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/dark-slim/skin.min.css` & `django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/dark-slim/skin.min.css`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/img/example.png` & `django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/img/example.png`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/img/tinymce.woff2` & `django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/img/tinymce.woff2`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/lightgray/content.min.css` & `django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/lightgray/content.min.css`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/lightgray/fonts/tinymce.woff` & `django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/lightgray/fonts/tinymce.woff`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/lightgray/skin.min.css` & `django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/lightgray/skin.min.css`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/plugins/accordion/plugin.js` & `django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/plugins/accordion/plugin.js`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/prism.css` & `django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/prism.css`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/static/custom_admin/tinymce/tinymce.min.js` & `django_customvueadmin-0.2.6/custom_admin/static/custom_admin/tinymce/tinymce.min.js`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/templates/custom_admin/admin_index.html` & `django_customvueadmin-0.2.6/custom_admin/templates/custom_admin/admin_index.html`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
   <link rel="preload" as="font" type="font/woff" href="/static/custom_admin/materialdesignicons-webfont-CgCzGbLl.woff" crossorigin="anonymous">
   <link rel="preload" as="font" type="font/ttf" href="/static/custom_admin/materialdesignicons-webfont-D3kAzl71.ttf" crossorigin="anonymous">
 
   <meta charset="UTF-8" />
   <link rel="icon" href="/custom_admin/favicon.ico" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   <title>{{ SETTINGS.title }}</title>
-  <script type="module" crossorigin src="/static/custom_admin/index-CKHFT4s-.js"></script>
-  <link rel="stylesheet" crossorigin href="/static/custom_admin/index-Dtvf0MB6.css">
+  <script type="module" crossorigin src="/static/custom_admin/index-DYa2T7lY.js"></script>
+  <link rel="stylesheet" crossorigin href="/static/custom_admin/index-C6_9c0_p.css">
 </head>
 
 <body>
   <div id="app"></div>
   <span id="settings" data-json="{{ SETTINGS_JSON }}"></span>
 </body>
```

### Comparing `django_customvueadmin-0.2.5/custom_admin/utils/async_mixin.py` & `django_customvueadmin-0.2.6/custom_admin/utils/async_mixin.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/utils/colors.py` & `django_customvueadmin-0.2.6/custom_admin/utils/colors.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/utils/get_schema.py` & `django_customvueadmin-0.2.6/custom_admin/utils/get_schema.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/utils/register_admin_viewsets.py` & `django_customvueadmin-0.2.6/custom_admin/utils/register_admin_viewsets.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/custom_admin/views/admin_page.py` & `django_customvueadmin-0.2.6/custom_admin/views/admin_page.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.5/django_customvueadmin.egg-info/PKG-INFO` & `django_customvueadmin-0.2.6/django_customvueadmin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-customvueadmin
-Version: 0.2.5
+Version: 0.2.6
 Summary: A custom admin interface providing backend via DRF and frontend via Vue and Element UI that tries to Keep It Simple.
 Home-page: https://innova-group-llc.github.io/custom_admin_docs/
 License: BSD-3-Clause
 Project-URL: Documentation, https://innova-group-llc.github.io/custom_admin_docs/
 Project-URL: Source, https://github.com/Innova-Group-LLC/custom_admin
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `django_customvueadmin-0.2.5/django_customvueadmin.egg-info/SOURCES.txt` & `django_customvueadmin-0.2.6/django_customvueadmin.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -60,16 +60,16 @@
 custom_admin/management/commands/__init__.py
 custom_admin/management/commands/custom_admin_viewsets_list.py
 custom_admin/migrations/0001_initial.py
 custom_admin/migrations/__init__.py
 custom_admin/models/__init__.py
 custom_admin/models/admin_log.py
 custom_admin/static/custom_admin/favicon.ico
-custom_admin/static/custom_admin/index-CKHFT4s-.js
-custom_admin/static/custom_admin/index-Dtvf0MB6.css
+custom_admin/static/custom_admin/index-C6_9c0_p.css
+custom_admin/static/custom_admin/index-DYa2T7lY.js
 custom_admin/static/custom_admin/materialdesignicons-webfont-CYDMK1kx.woff2
 custom_admin/static/custom_admin/materialdesignicons-webfont-CgCzGbLl.woff
 custom_admin/static/custom_admin/materialdesignicons-webfont-D3kAzl71.ttf
 custom_admin/static/custom_admin/materialdesignicons-webfont-DttUABo4.eot
 custom_admin/static/custom_admin/tinymce/tinymce.min.js
 custom_admin/static/custom_admin/tinymce/dark-first/content.min.css
 custom_admin/static/custom_admin/tinymce/dark-first/skin.min.css
```

### Comparing `django_customvueadmin-0.2.5/setup.cfg` & `django_customvueadmin-0.2.6/setup.cfg`

 * *Files identical despite different names*
