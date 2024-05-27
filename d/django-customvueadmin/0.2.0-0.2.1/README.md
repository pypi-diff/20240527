# Comparing `tmp/django_customvueadmin-0.2.0.tar.gz` & `tmp/django_customvueadmin-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_customvueadmin-0.2.0.tar", last modified: Mon May 27 08:40:47 2024, max compression
+gzip compressed data, was "django_customvueadmin-0.2.1.tar", last modified: Mon May 27 08:50:02 2024, max compression
```

## Comparing `django_customvueadmin-0.2.0.tar` & `django_customvueadmin-0.2.1.tar`

### file list

```diff
@@ -1,133 +1,127 @@
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.140870 django_customvueadmin-0.2.0/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1073 2024-04-26 14:57:56.000000 django_customvueadmin-0.2.0/LICENSE
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      209 2024-04-11 14:26:38.000000 django_customvueadmin-0.2.0/MANIFEST.in
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2812 2024-05-27 08:40:47.140870 django_customvueadmin-0.2.0/PKG-INFO
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1979 2024-05-27 08:39:38.000000 django_customvueadmin-0.2.0/README.rst
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.114200 django_customvueadmin-0.2.0/custom_admin/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       45 2024-05-27 07:51:30.000000 django_customvueadmin-0.2.0/custom_admin/__init__.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.117534 django_customvueadmin-0.2.0/custom_admin/api/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       86 2024-04-19 14:02:39.000000 django_customvueadmin-0.2.0/custom_admin/api/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1529 2024-05-25 10:30:35.000000 django_customvueadmin-0.2.0/custom_admin/api/action_functions.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.117534 django_customvueadmin-0.2.0/custom_admin/api/actions/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      139 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/api/actions/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      985 2024-05-25 10:29:03.000000 django_customvueadmin-0.2.0/custom_admin/api/actions/delete_action.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2538 2024-05-24 12:45:37.000000 django_customvueadmin-0.2.0/custom_admin/api/actions/export_csv_action.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2723 2024-05-24 15:46:18.000000 django_customvueadmin-0.2.0/custom_admin/api/actions/view_actions_mixin.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1724 2024-05-22 00:15:55.000000 django_customvueadmin-0.2.0/custom_admin/api/backends.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.120868 django_customvueadmin-0.2.0/custom_admin/api/fields/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      403 2024-05-06 15:09:48.000000 django_customvueadmin-0.2.0/custom_admin/api/fields/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      381 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/api/fields/base.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      811 2024-04-23 15:22:53.000000 django_customvueadmin-0.2.0/custom_admin/api/fields/char.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1233 2024-04-23 15:23:30.000000 django_customvueadmin-0.2.0/custom_admin/api/fields/choice.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3695 2024-05-26 16:28:48.000000 django_customvueadmin-0.2.0/custom_admin/api/fields/files.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      157 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/api/fields/int.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      326 2024-05-06 16:10:42.000000 django_customvueadmin-0.2.0/custom_admin/api/fields/json.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      343 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/api/fields/numbers.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3871 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/api/fields/relation.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.120868 django_customvueadmin-0.2.0/custom_admin/api/filters/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      165 2024-05-21 23:11:51.000000 django_customvueadmin-0.2.0/custom_admin/api/filters/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1623 2024-05-21 23:13:58.000000 django_customvueadmin-0.2.0/custom_admin/api/filters/base_admin_filter.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/api/filters/choices.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      733 2024-05-22 00:17:36.000000 django_customvueadmin-0.2.0/custom_admin/api/filters/date_range.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1445 2024-05-08 17:32:46.000000 django_customvueadmin-0.2.0/custom_admin/api/inline_relation.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.124202 django_customvueadmin-0.2.0/custom_admin/api/inlines/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      305 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/api/inlines/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      601 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/api/inlines/export_csv_inline.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1595 2024-05-21 13:46:54.000000 django_customvueadmin-0.2.0/custom_admin/api/inlines/inline_graph.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2129 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/api/inlines/inline_table.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       61 2024-03-29 18:33:05.000000 django_customvueadmin-0.2.0/custom_admin/api/inlines/inlines_type.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      135 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/api/inlines/interfaces.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4154 2024-04-02 18:13:36.000000 django_customvueadmin-0.2.0/custom_admin/api/inlines/view_inline_mixin.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      893 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/api/permissions.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.124202 django_customvueadmin-0.2.0/custom_admin/api/serializers/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      207 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/api/serializers/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      737 2024-04-19 13:32:46.000000 django_customvueadmin-0.2.0/custom_admin/api/serializers/auth_response.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5491 2024-05-06 15:09:50.000000 django_customvueadmin-0.2.0/custom_admin/api/serializers/base_serializer.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.124202 django_customvueadmin-0.2.0/custom_admin/api/tests/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-11 07:49:25.000000 django_customvueadmin-0.2.0/custom_admin/api/tests/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2317 2024-05-21 23:39:40.000000 django_customvueadmin-0.2.0/custom_admin/api/tests/test_filters.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      517 2024-05-21 20:22:03.000000 django_customvueadmin-0.2.0/custom_admin/api/tests/test_scheme_get.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      550 2024-05-21 19:31:58.000000 django_customvueadmin-0.2.0/custom_admin/api/tests/urls.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      599 2024-05-26 18:19:08.000000 django_customvueadmin-0.2.0/custom_admin/api/urls.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.124202 django_customvueadmin-0.2.0/custom_admin/api/views/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      414 2024-05-21 19:10:33.000000 django_customvueadmin-0.2.0/custom_admin/api/views/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5829 2024-05-26 20:56:51.000000 django_customvueadmin-0.2.0/custom_admin/api/views/autocomplete.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     8432 2024-05-26 18:11:53.000000 django_customvueadmin-0.2.0/custom_admin/api/views/base_admin_viewset.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.127535 django_customvueadmin-0.2.0/custom_admin/api/views/defaults/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      131 2024-05-21 19:10:56.000000 django_customvueadmin-0.2.0/custom_admin/api/views/defaults/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2080 2024-05-21 19:58:42.000000 django_customvueadmin-0.2.0/custom_admin/api/views/defaults/admin_log.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      366 2024-05-21 19:06:40.000000 django_customvueadmin-0.2.0/custom_admin/api/views/defaults/groups.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      529 2024-05-21 19:09:36.000000 django_customvueadmin-0.2.0/custom_admin/api/views/defaults/permissions.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      909 2024-04-23 23:45:01.000000 django_customvueadmin-0.2.0/custom_admin/api/views/get_sections.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1517 2024-04-11 17:29:22.000000 django_customvueadmin-0.2.0/custom_admin/api/views/token_auth.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      974 2024-05-08 17:32:54.000000 django_customvueadmin-0.2.0/custom_admin/api/viewset_info.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.127535 django_customvueadmin-0.2.0/custom_admin/controllers/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-04-19 14:01:33.000000 django_customvueadmin-0.2.0/custom_admin/controllers/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3475 2024-05-20 10:10:21.000000 django_customvueadmin-0.2.0/custom_admin/controllers/admin_log_manager.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3823 2024-05-26 16:40:34.000000 django_customvueadmin-0.2.0/custom_admin/controllers/custom_metadata.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3078 2024-05-20 19:45:54.000000 django_customvueadmin-0.2.0/custom_admin/controllers/filters_schema.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     9232 2024-05-24 13:28:46.000000 django_customvueadmin-0.2.0/custom_admin/controllers/schema_generator.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.127535 django_customvueadmin-0.2.0/custom_admin/management/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-04-15 16:06:07.000000 django_customvueadmin-0.2.0/custom_admin/management/__init__.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.127535 django_customvueadmin-0.2.0/custom_admin/management/commands/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-04-15 16:06:19.000000 django_customvueadmin-0.2.0/custom_admin/management/commands/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1300 2024-04-15 16:52:15.000000 django_customvueadmin-0.2.0/custom_admin/management/commands/custom_admin_viewsets_list.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.127535 django_customvueadmin-0.2.0/custom_admin/migrations/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1695 2024-04-11 18:20:54.000000 django_customvueadmin-0.2.0/custom_admin/migrations/0001_initial.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 18:20:54.000000 django_customvueadmin-0.2.0/custom_admin/migrations/__init__.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.127535 django_customvueadmin-0.2.0/custom_admin/models/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       32 2024-03-11 07:49:25.000000 django_customvueadmin-0.2.0/custom_admin/models/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1469 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/models/admin_log.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.110867 django_customvueadmin-0.2.0/custom_admin/static/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.134203 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2238 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/favicon.ico
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)   752706 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/index-C4Cutzkc.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1681833 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/index-OjzvLInB.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)   385360 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/materialdesignicons-webfont-CYDMK1kx.woff2
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)   561776 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/materialdesignicons-webfont-CgCzGbLl.woff
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1243500 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/materialdesignicons-webfont-D3kAzl71.ttf
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1243720 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/materialdesignicons-webfont-DttUABo4.eot
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.134203 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.137536 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/dark-first/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4788 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/dark-first/content.min.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    50376 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/dark-first/skin.min.css
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.137536 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/dark-slim/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4730 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/dark-slim/content.min.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    49965 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/dark-slim/skin.min.css
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.137536 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/img/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    14708 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/img/example.png
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    15764 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/img/tinymce.woff2
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.137536 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/lightgray/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3193 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/lightgray/content.min.css
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.137536 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/lightgray/fonts/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     7664 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/lightgray/fonts/tinymce.woff
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    38232 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/lightgray/skin.min.css
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.114200 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/plugins/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.137536 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/plugins/accordion/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.137536 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/plugins/accordion/css/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/plugins/accordion/css/accordion.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1251 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/plugins/accordion/plugin.js
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.114200 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/plugins/codesample/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.137536 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1736 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/prism.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1171290 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/tinymce.min.js
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.114200 django_customvueadmin-0.2.0/custom_admin/templates/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.137536 django_customvueadmin-0.2.0/custom_admin/templates/custom_admin/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1309 2024-05-27 08:38:31.000000 django_customvueadmin-0.2.0/custom_admin/templates/custom_admin/admin_index.html
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.140870 django_customvueadmin-0.2.0/custom_admin/utils/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       35 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/utils/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1976 2024-04-11 17:58:41.000000 django_customvueadmin-0.2.0/custom_admin/utils/async_mixin.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2425 2024-04-09 09:57:39.000000 django_customvueadmin-0.2.0/custom_admin/utils/colors.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      570 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/utils/get_schema.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      593 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/utils/register_admin_viewsets.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.140870 django_customvueadmin-0.2.0/custom_admin/views/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       40 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/views/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1769 2024-04-15 18:01:09.000000 django_customvueadmin-0.2.0/custom_admin/views/admin_page.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.140870 django_customvueadmin-0.2.0/django_customvueadmin.egg-info/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2812 2024-05-27 08:40:47.000000 django_customvueadmin-0.2.0/django_customvueadmin.egg-info/PKG-INFO
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4196 2024-05-27 08:40:47.000000 django_customvueadmin-0.2.0/django_customvueadmin.egg-info/SOURCES.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-05-27 08:40:47.000000 django_customvueadmin-0.2.0/django_customvueadmin.egg-info/dependency_links.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-05-27 08:40:46.000000 django_customvueadmin-0.2.0/django_customvueadmin.egg-info/not-zip-safe
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       13 2024-05-27 08:40:47.000000 django_customvueadmin-0.2.0/django_customvueadmin.egg-info/top_level.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      222 2024-04-11 09:22:36.000000 django_customvueadmin-0.2.0/pyproject.toml
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1000 2024-05-27 08:40:47.140870 django_customvueadmin-0.2.0/setup.cfg
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.816001 django_customvueadmin-0.2.1/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1073 2024-04-26 14:57:56.000000 django_customvueadmin-0.2.1/LICENSE
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      209 2024-04-11 14:26:38.000000 django_customvueadmin-0.2.1/MANIFEST.in
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2884 2024-05-27 08:50:02.816001 django_customvueadmin-0.2.1/PKG-INFO
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2051 2024-05-27 08:49:51.000000 django_customvueadmin-0.2.1/README.rst
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.806000 django_customvueadmin-0.2.1/custom_admin/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       45 2024-05-27 08:49:58.000000 django_customvueadmin-0.2.1/custom_admin/__init__.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.806000 django_customvueadmin-0.2.1/custom_admin/api/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       86 2024-04-19 14:02:39.000000 django_customvueadmin-0.2.1/custom_admin/api/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1529 2024-05-25 10:30:35.000000 django_customvueadmin-0.2.1/custom_admin/api/action_functions.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.806000 django_customvueadmin-0.2.1/custom_admin/api/actions/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      139 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.1/custom_admin/api/actions/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      985 2024-05-25 10:29:03.000000 django_customvueadmin-0.2.1/custom_admin/api/actions/delete_action.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2538 2024-05-24 12:45:37.000000 django_customvueadmin-0.2.1/custom_admin/api/actions/export_csv_action.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2723 2024-05-24 15:46:18.000000 django_customvueadmin-0.2.1/custom_admin/api/actions/view_actions_mixin.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1724 2024-05-22 00:15:55.000000 django_customvueadmin-0.2.1/custom_admin/api/backends.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.809334 django_customvueadmin-0.2.1/custom_admin/api/fields/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      403 2024-05-06 15:09:48.000000 django_customvueadmin-0.2.1/custom_admin/api/fields/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      381 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.1/custom_admin/api/fields/base.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      811 2024-04-23 15:22:53.000000 django_customvueadmin-0.2.1/custom_admin/api/fields/char.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1233 2024-04-23 15:23:30.000000 django_customvueadmin-0.2.1/custom_admin/api/fields/choice.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3695 2024-05-26 16:28:48.000000 django_customvueadmin-0.2.1/custom_admin/api/fields/files.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      157 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.1/custom_admin/api/fields/int.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      326 2024-05-06 16:10:42.000000 django_customvueadmin-0.2.1/custom_admin/api/fields/json.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      343 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.1/custom_admin/api/fields/numbers.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3871 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.1/custom_admin/api/fields/relation.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.809334 django_customvueadmin-0.2.1/custom_admin/api/filters/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      165 2024-05-21 23:11:51.000000 django_customvueadmin-0.2.1/custom_admin/api/filters/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1623 2024-05-21 23:13:58.000000 django_customvueadmin-0.2.1/custom_admin/api/filters/base_admin_filter.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.1/custom_admin/api/filters/choices.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      733 2024-05-22 00:17:36.000000 django_customvueadmin-0.2.1/custom_admin/api/filters/date_range.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1445 2024-05-08 17:32:46.000000 django_customvueadmin-0.2.1/custom_admin/api/inline_relation.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.809334 django_customvueadmin-0.2.1/custom_admin/api/inlines/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      305 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.1/custom_admin/api/inlines/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      601 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.1/custom_admin/api/inlines/export_csv_inline.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1595 2024-05-21 13:46:54.000000 django_customvueadmin-0.2.1/custom_admin/api/inlines/inline_graph.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2129 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.1/custom_admin/api/inlines/inline_table.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       61 2024-03-29 18:33:05.000000 django_customvueadmin-0.2.1/custom_admin/api/inlines/inlines_type.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      135 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.1/custom_admin/api/inlines/interfaces.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4154 2024-04-02 18:13:36.000000 django_customvueadmin-0.2.1/custom_admin/api/inlines/view_inline_mixin.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      893 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.1/custom_admin/api/permissions.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.809334 django_customvueadmin-0.2.1/custom_admin/api/serializers/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      207 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.1/custom_admin/api/serializers/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      737 2024-04-19 13:32:46.000000 django_customvueadmin-0.2.1/custom_admin/api/serializers/auth_response.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5491 2024-05-06 15:09:50.000000 django_customvueadmin-0.2.1/custom_admin/api/serializers/base_serializer.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.809334 django_customvueadmin-0.2.1/custom_admin/api/tests/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-11 07:49:25.000000 django_customvueadmin-0.2.1/custom_admin/api/tests/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2317 2024-05-21 23:39:40.000000 django_customvueadmin-0.2.1/custom_admin/api/tests/test_filters.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      517 2024-05-21 20:22:03.000000 django_customvueadmin-0.2.1/custom_admin/api/tests/test_scheme_get.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      550 2024-05-21 19:31:58.000000 django_customvueadmin-0.2.1/custom_admin/api/tests/urls.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      599 2024-05-26 18:19:08.000000 django_customvueadmin-0.2.1/custom_admin/api/urls.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.812667 django_customvueadmin-0.2.1/custom_admin/api/views/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      414 2024-05-21 19:10:33.000000 django_customvueadmin-0.2.1/custom_admin/api/views/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5829 2024-05-26 20:56:51.000000 django_customvueadmin-0.2.1/custom_admin/api/views/autocomplete.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     8432 2024-05-26 18:11:53.000000 django_customvueadmin-0.2.1/custom_admin/api/views/base_admin_viewset.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.812667 django_customvueadmin-0.2.1/custom_admin/api/views/defaults/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      131 2024-05-21 19:10:56.000000 django_customvueadmin-0.2.1/custom_admin/api/views/defaults/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2080 2024-05-21 19:58:42.000000 django_customvueadmin-0.2.1/custom_admin/api/views/defaults/admin_log.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      366 2024-05-21 19:06:40.000000 django_customvueadmin-0.2.1/custom_admin/api/views/defaults/groups.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      529 2024-05-21 19:09:36.000000 django_customvueadmin-0.2.1/custom_admin/api/views/defaults/permissions.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      909 2024-04-23 23:45:01.000000 django_customvueadmin-0.2.1/custom_admin/api/views/get_sections.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1517 2024-04-11 17:29:22.000000 django_customvueadmin-0.2.1/custom_admin/api/views/token_auth.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      974 2024-05-08 17:32:54.000000 django_customvueadmin-0.2.1/custom_admin/api/viewset_info.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.812667 django_customvueadmin-0.2.1/custom_admin/controllers/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-04-19 14:01:33.000000 django_customvueadmin-0.2.1/custom_admin/controllers/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3475 2024-05-20 10:10:21.000000 django_customvueadmin-0.2.1/custom_admin/controllers/admin_log_manager.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3823 2024-05-26 16:40:34.000000 django_customvueadmin-0.2.1/custom_admin/controllers/custom_metadata.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3078 2024-05-20 19:45:54.000000 django_customvueadmin-0.2.1/custom_admin/controllers/filters_schema.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     9232 2024-05-24 13:28:46.000000 django_customvueadmin-0.2.1/custom_admin/controllers/schema_generator.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.812667 django_customvueadmin-0.2.1/custom_admin/management/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-04-15 16:06:07.000000 django_customvueadmin-0.2.1/custom_admin/management/__init__.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.812667 django_customvueadmin-0.2.1/custom_admin/management/commands/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-04-15 16:06:19.000000 django_customvueadmin-0.2.1/custom_admin/management/commands/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1300 2024-04-15 16:52:15.000000 django_customvueadmin-0.2.1/custom_admin/management/commands/custom_admin_viewsets_list.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.812667 django_customvueadmin-0.2.1/custom_admin/migrations/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1695 2024-04-11 18:20:54.000000 django_customvueadmin-0.2.1/custom_admin/migrations/0001_initial.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 18:20:54.000000 django_customvueadmin-0.2.1/custom_admin/migrations/__init__.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.812667 django_customvueadmin-0.2.1/custom_admin/models/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       32 2024-03-11 07:49:25.000000 django_customvueadmin-0.2.1/custom_admin/models/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1469 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.1/custom_admin/models/admin_log.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.806000 django_customvueadmin-0.2.1/custom_admin/static/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.812667 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2238 2024-05-27 08:49:35.000000 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/favicon.ico
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.812667 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.812667 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/dark-first/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4788 2024-05-27 08:49:35.000000 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/dark-first/content.min.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    50376 2024-05-27 08:49:35.000000 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/dark-first/skin.min.css
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.816001 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/dark-slim/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4730 2024-05-27 08:49:35.000000 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/dark-slim/content.min.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    49965 2024-05-27 08:49:35.000000 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/dark-slim/skin.min.css
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.816001 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/img/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    14708 2024-05-27 08:49:35.000000 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/img/example.png
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    15764 2024-05-27 08:49:35.000000 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/img/tinymce.woff2
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.816001 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/lightgray/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3193 2024-05-27 08:49:35.000000 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/lightgray/content.min.css
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.816001 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/lightgray/fonts/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     7664 2024-05-27 08:49:35.000000 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/lightgray/fonts/tinymce.woff
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    38232 2024-05-27 08:49:35.000000 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/lightgray/skin.min.css
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.806000 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/plugins/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.816001 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/plugins/accordion/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.816001 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/plugins/accordion/css/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-05-27 08:49:35.000000 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/plugins/accordion/css/accordion.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1251 2024-05-27 08:49:35.000000 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/plugins/accordion/plugin.js
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.806000 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/plugins/codesample/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.816001 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1736 2024-05-27 08:49:35.000000 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/prism.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1171290 2024-05-27 08:49:35.000000 django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/tinymce.min.js
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.806000 django_customvueadmin-0.2.1/custom_admin/templates/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.816001 django_customvueadmin-0.2.1/custom_admin/templates/custom_admin/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1351 2024-05-27 08:49:33.000000 django_customvueadmin-0.2.1/custom_admin/templates/custom_admin/admin_index.html
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.816001 django_customvueadmin-0.2.1/custom_admin/utils/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       35 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.1/custom_admin/utils/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1976 2024-04-11 17:58:41.000000 django_customvueadmin-0.2.1/custom_admin/utils/async_mixin.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2425 2024-04-09 09:57:39.000000 django_customvueadmin-0.2.1/custom_admin/utils/colors.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      570 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.1/custom_admin/utils/get_schema.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      593 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.1/custom_admin/utils/register_admin_viewsets.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.816001 django_customvueadmin-0.2.1/custom_admin/views/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       40 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.1/custom_admin/views/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1335 2024-05-27 08:43:53.000000 django_customvueadmin-0.2.1/custom_admin/views/admin_page.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:50:02.816001 django_customvueadmin-0.2.1/django_customvueadmin.egg-info/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2884 2024-05-27 08:50:02.000000 django_customvueadmin-0.2.1/django_customvueadmin.egg-info/PKG-INFO
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3794 2024-05-27 08:50:02.000000 django_customvueadmin-0.2.1/django_customvueadmin.egg-info/SOURCES.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-05-27 08:50:02.000000 django_customvueadmin-0.2.1/django_customvueadmin.egg-info/dependency_links.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-05-27 08:50:02.000000 django_customvueadmin-0.2.1/django_customvueadmin.egg-info/not-zip-safe
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       13 2024-05-27 08:50:02.000000 django_customvueadmin-0.2.1/django_customvueadmin.egg-info/top_level.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      222 2024-04-11 09:22:36.000000 django_customvueadmin-0.2.1/pyproject.toml
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1000 2024-05-27 08:50:02.816001 django_customvueadmin-0.2.1/setup.cfg
```

### Comparing `django_customvueadmin-0.2.0/LICENSE` & `django_customvueadmin-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/PKG-INFO` & `django_customvueadmin-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-customvueadmin
-Version: 0.2.0
+Version: 0.2.1
 Summary: A custom admin interface providing backend via DRF and frontend via Vue and Element UI that tries to Keep It Simple.
 Home-page: https://innova-group-llc.github.io/custom_admin_docs/
 License: BSD-3-Clause
 Project-URL: Documentation, https://innova-group-llc.github.io/custom_admin_docs/
 Project-URL: Source, https://github.com/Innova-Group-LLC/custom_admin
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -63,13 +63,16 @@
 
    npm run build --prefix vue_frontend
    rm -r custom_admin/static/custom_admin/*
    rm -r custom_admin/templates/custom_admin/admin_index.html
    cp vue_frontend/dist/index.html custom_admin/templates/custom_admin/admin_index.html
    cp -r vue_frontend/dist/custom_admin/ custom_admin/static/
 
+   python -m build
+   python3 -m twine upload --repository pypi dist/*
+
 .. |logo| image:: https://github.com/Innova-Group-LLC/custom_admin/blob/master/logo.png?raw=true
    :target: https://innova-group-llc.github.io/custom_admin_docs/
 .. |PyPI version| image:: https://badge.fury.io/py/django-customvueadmin.svg
    :target: https://pypi.org/project/django-customvueadmin/
 .. |GitHub stars| image:: https://img.shields.io/github/stars/Innova-Group-LLC/custom_admin
    :target: https://github.com/Innova-Group-LLC/custom_admin
```

### Comparing `django_customvueadmin-0.2.0/README.rst` & `django_customvueadmin-0.2.1/django_customvueadmin.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: django-customvueadmin
+Version: 0.2.1
+Summary: A custom admin interface providing backend via DRF and frontend via Vue and Element UI that tries to Keep It Simple.
+Home-page: https://innova-group-llc.github.io/custom_admin_docs/
+License: BSD-3-Clause
+Project-URL: Documentation, https://innova-group-llc.github.io/custom_admin_docs/
+Project-URL: Source, https://github.com/Innova-Group-LLC/custom_admin
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+License-File: LICENSE
+
 Django Custom Admin
 ===================
 
 |logo|
 
 A custom admin interface providing backend via DRF and frontend via Vue
 and Element UI that tries to Keep It Simple.
@@ -45,13 +63,16 @@
 
    npm run build --prefix vue_frontend
    rm -r custom_admin/static/custom_admin/*
    rm -r custom_admin/templates/custom_admin/admin_index.html
    cp vue_frontend/dist/index.html custom_admin/templates/custom_admin/admin_index.html
    cp -r vue_frontend/dist/custom_admin/ custom_admin/static/
 
+   python -m build
+   python3 -m twine upload --repository pypi dist/*
+
 .. |logo| image:: https://github.com/Innova-Group-LLC/custom_admin/blob/master/logo.png?raw=true
    :target: https://innova-group-llc.github.io/custom_admin_docs/
 .. |PyPI version| image:: https://badge.fury.io/py/django-customvueadmin.svg
    :target: https://pypi.org/project/django-customvueadmin/
 .. |GitHub stars| image:: https://img.shields.io/github/stars/Innova-Group-LLC/custom_admin
    :target: https://github.com/Innova-Group-LLC/custom_admin
```

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/action_functions.py` & `django_customvueadmin-0.2.1/custom_admin/api/action_functions.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/actions/delete_action.py` & `django_customvueadmin-0.2.1/custom_admin/api/actions/delete_action.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/actions/export_csv_action.py` & `django_customvueadmin-0.2.1/custom_admin/api/actions/export_csv_action.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/actions/view_actions_mixin.py` & `django_customvueadmin-0.2.1/custom_admin/api/actions/view_actions_mixin.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/backends.py` & `django_customvueadmin-0.2.1/custom_admin/api/backends.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/fields/char.py` & `django_customvueadmin-0.2.1/custom_admin/api/fields/char.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/fields/choice.py` & `django_customvueadmin-0.2.1/custom_admin/api/fields/choice.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/fields/files.py` & `django_customvueadmin-0.2.1/custom_admin/api/fields/files.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/fields/relation.py` & `django_customvueadmin-0.2.1/custom_admin/api/fields/relation.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/filters/base_admin_filter.py` & `django_customvueadmin-0.2.1/custom_admin/api/filters/base_admin_filter.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/filters/date_range.py` & `django_customvueadmin-0.2.1/custom_admin/api/filters/date_range.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/inline_relation.py` & `django_customvueadmin-0.2.1/custom_admin/api/inline_relation.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/inlines/export_csv_inline.py` & `django_customvueadmin-0.2.1/custom_admin/api/inlines/export_csv_inline.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/inlines/inline_graph.py` & `django_customvueadmin-0.2.1/custom_admin/api/inlines/inline_graph.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/inlines/inline_table.py` & `django_customvueadmin-0.2.1/custom_admin/api/inlines/inline_table.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/inlines/view_inline_mixin.py` & `django_customvueadmin-0.2.1/custom_admin/api/inlines/view_inline_mixin.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/permissions.py` & `django_customvueadmin-0.2.1/custom_admin/api/permissions.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/serializers/auth_response.py` & `django_customvueadmin-0.2.1/custom_admin/api/serializers/auth_response.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/serializers/base_serializer.py` & `django_customvueadmin-0.2.1/custom_admin/api/serializers/base_serializer.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/tests/test_filters.py` & `django_customvueadmin-0.2.1/custom_admin/api/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/tests/test_scheme_get.py` & `django_customvueadmin-0.2.1/custom_admin/api/tests/test_scheme_get.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/tests/urls.py` & `django_customvueadmin-0.2.1/custom_admin/api/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/urls.py` & `django_customvueadmin-0.2.1/custom_admin/api/urls.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/views/autocomplete.py` & `django_customvueadmin-0.2.1/custom_admin/api/views/autocomplete.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/views/base_admin_viewset.py` & `django_customvueadmin-0.2.1/custom_admin/api/views/base_admin_viewset.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/views/defaults/admin_log.py` & `django_customvueadmin-0.2.1/custom_admin/api/views/defaults/admin_log.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/views/defaults/permissions.py` & `django_customvueadmin-0.2.1/custom_admin/api/views/defaults/permissions.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/views/get_sections.py` & `django_customvueadmin-0.2.1/custom_admin/api/views/get_sections.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/views/token_auth.py` & `django_customvueadmin-0.2.1/custom_admin/api/views/token_auth.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/api/viewset_info.py` & `django_customvueadmin-0.2.1/custom_admin/api/viewset_info.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/controllers/admin_log_manager.py` & `django_customvueadmin-0.2.1/custom_admin/controllers/admin_log_manager.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/controllers/custom_metadata.py` & `django_customvueadmin-0.2.1/custom_admin/controllers/custom_metadata.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/controllers/filters_schema.py` & `django_customvueadmin-0.2.1/custom_admin/controllers/filters_schema.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/controllers/schema_generator.py` & `django_customvueadmin-0.2.1/custom_admin/controllers/schema_generator.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/management/commands/custom_admin_viewsets_list.py` & `django_customvueadmin-0.2.1/custom_admin/management/commands/custom_admin_viewsets_list.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/migrations/0001_initial.py` & `django_customvueadmin-0.2.1/custom_admin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/models/admin_log.py` & `django_customvueadmin-0.2.1/custom_admin/models/admin_log.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/favicon.ico` & `django_customvueadmin-0.2.1/custom_admin/static/custom_admin/favicon.ico`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/dark-first/content.min.css` & `django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/dark-first/content.min.css`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/dark-first/skin.min.css` & `django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/dark-first/skin.min.css`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/dark-slim/content.min.css` & `django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/dark-slim/content.min.css`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/dark-slim/skin.min.css` & `django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/dark-slim/skin.min.css`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/img/example.png` & `django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/img/example.png`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/img/tinymce.woff2` & `django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/img/tinymce.woff2`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/lightgray/content.min.css` & `django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/lightgray/content.min.css`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/lightgray/fonts/tinymce.woff` & `django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/lightgray/fonts/tinymce.woff`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/lightgray/skin.min.css` & `django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/lightgray/skin.min.css`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/plugins/accordion/plugin.js` & `django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/plugins/accordion/plugin.js`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/prism.css` & `django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/prism.css`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/tinymce.min.js` & `django_customvueadmin-0.2.1/custom_admin/static/custom_admin/tinymce/tinymce.min.js`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/templates/custom_admin/admin_index.html` & `django_customvueadmin-0.2.1/custom_admin/templates/custom_admin/admin_index.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <!DOCTYPE html>
 <html lang="en">
 
 <head>
   <link rel="preconnect" href="https://fonts.gstatic.com/" crossorigin="anonymous">
   <link rel="preload" as="style" onload="this.rel='stylesheet'" href="https://fonts.googleapis.com/css2?family=Roboto:wght@100;300;400;500;700;900&display=swap">
-  <link rel="preload" as="font" type="font/eot" href="/custom_admin/materialdesignicons-webfont-DttUABo4.eot" crossorigin="anonymous">
-  <link rel="preload" as="font" type="font/woff2" href="/custom_admin/materialdesignicons-webfont-CYDMK1kx.woff2" crossorigin="anonymous">
-  <link rel="preload" as="font" type="font/woff" href="/custom_admin/materialdesignicons-webfont-CgCzGbLl.woff" crossorigin="anonymous">
-  <link rel="preload" as="font" type="font/ttf" href="/custom_admin/materialdesignicons-webfont-D3kAzl71.ttf" crossorigin="anonymous">
+  <link rel="preload" as="font" type="font/eot" href="/static/custom_admin/materialdesignicons-webfont-DttUABo4.eot" crossorigin="anonymous">
+  <link rel="preload" as="font" type="font/woff2" href="/static/custom_admin/materialdesignicons-webfont-CYDMK1kx.woff2" crossorigin="anonymous">
+  <link rel="preload" as="font" type="font/woff" href="/static/custom_admin/materialdesignicons-webfont-CgCzGbLl.woff" crossorigin="anonymous">
+  <link rel="preload" as="font" type="font/ttf" href="/static/custom_admin/materialdesignicons-webfont-D3kAzl71.ttf" crossorigin="anonymous">
 
   <meta charset="UTF-8" />
   <link rel="icon" href="/custom_admin/favicon.ico" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   <title>{{ SETTINGS.title }}</title>
-  <script type="module" crossorigin src="/custom_admin/index-OjzvLInB.js"></script>
-  <link rel="stylesheet" crossorigin href="/custom_admin/index-C4Cutzkc.css">
+  <script type="module" crossorigin src="/static/custom_admin/index-BoVV6dkV.js"></script>
+  <link rel="stylesheet" crossorigin href="/static/custom_admin/index-Dtvf0MB6.css">
 </head>
 
 <body>
   <div id="app"></div>
   <span id="settings" data-json="{{ SETTINGS_JSON }}"></span>
 </body>
```

### Comparing `django_customvueadmin-0.2.0/custom_admin/utils/async_mixin.py` & `django_customvueadmin-0.2.1/custom_admin/utils/async_mixin.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/utils/colors.py` & `django_customvueadmin-0.2.1/custom_admin/utils/colors.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/utils/get_schema.py` & `django_customvueadmin-0.2.1/custom_admin/utils/get_schema.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/custom_admin/utils/register_admin_viewsets.py` & `django_customvueadmin-0.2.1/custom_admin/utils/register_admin_viewsets.py`

 * *Files identical despite different names*

### Comparing `django_customvueadmin-0.2.0/django_customvueadmin.egg-info/PKG-INFO` & `django_customvueadmin-0.2.1/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: django-customvueadmin
-Version: 0.2.0
-Summary: A custom admin interface providing backend via DRF and frontend via Vue and Element UI that tries to Keep It Simple.
-Home-page: https://innova-group-llc.github.io/custom_admin_docs/
-License: BSD-3-Clause
-Project-URL: Documentation, https://innova-group-llc.github.io/custom_admin_docs/
-Project-URL: Source, https://github.com/Innova-Group-LLC/custom_admin
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
-License-File: LICENSE
-
 Django Custom Admin
 ===================
 
 |logo|
 
 A custom admin interface providing backend via DRF and frontend via Vue
 and Element UI that tries to Keep It Simple.
@@ -63,13 +45,16 @@
 
    npm run build --prefix vue_frontend
    rm -r custom_admin/static/custom_admin/*
    rm -r custom_admin/templates/custom_admin/admin_index.html
    cp vue_frontend/dist/index.html custom_admin/templates/custom_admin/admin_index.html
    cp -r vue_frontend/dist/custom_admin/ custom_admin/static/
 
+   python -m build
+   python3 -m twine upload --repository pypi dist/*
+
 .. |logo| image:: https://github.com/Innova-Group-LLC/custom_admin/blob/master/logo.png?raw=true
    :target: https://innova-group-llc.github.io/custom_admin_docs/
 .. |PyPI version| image:: https://badge.fury.io/py/django-customvueadmin.svg
    :target: https://pypi.org/project/django-customvueadmin/
 .. |GitHub stars| image:: https://img.shields.io/github/stars/Innova-Group-LLC/custom_admin
    :target: https://github.com/Innova-Group-LLC/custom_admin
```

### Comparing `django_customvueadmin-0.2.0/django_customvueadmin.egg-info/SOURCES.txt` & `django_customvueadmin-0.2.1/django_customvueadmin.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -60,20 +60,14 @@
 custom_admin/management/commands/__init__.py
 custom_admin/management/commands/custom_admin_viewsets_list.py
 custom_admin/migrations/0001_initial.py
 custom_admin/migrations/__init__.py
 custom_admin/models/__init__.py
 custom_admin/models/admin_log.py
 custom_admin/static/custom_admin/favicon.ico
-custom_admin/static/custom_admin/index-C4Cutzkc.css
-custom_admin/static/custom_admin/index-OjzvLInB.js
-custom_admin/static/custom_admin/materialdesignicons-webfont-CYDMK1kx.woff2
-custom_admin/static/custom_admin/materialdesignicons-webfont-CgCzGbLl.woff
-custom_admin/static/custom_admin/materialdesignicons-webfont-D3kAzl71.ttf
-custom_admin/static/custom_admin/materialdesignicons-webfont-DttUABo4.eot
 custom_admin/static/custom_admin/tinymce/tinymce.min.js
 custom_admin/static/custom_admin/tinymce/dark-first/content.min.css
 custom_admin/static/custom_admin/tinymce/dark-first/skin.min.css
 custom_admin/static/custom_admin/tinymce/dark-slim/content.min.css
 custom_admin/static/custom_admin/tinymce/dark-slim/skin.min.css
 custom_admin/static/custom_admin/tinymce/img/example.png
 custom_admin/static/custom_admin/tinymce/img/tinymce.woff2
```

### Comparing `django_customvueadmin-0.2.0/setup.cfg` & `django_customvueadmin-0.2.1/setup.cfg`

 * *Files identical despite different names*

