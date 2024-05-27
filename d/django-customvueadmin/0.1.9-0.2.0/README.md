# Comparing `tmp/django-customvueadmin-0.1.9.tar.gz` & `tmp/django_customvueadmin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-customvueadmin-0.1.9.tar", last modified: Thu Apr 11 16:02:21 2024, max compression
+gzip compressed data, was "django_customvueadmin-0.2.0.tar", last modified: Mon May 27 08:40:47 2024, max compression
```

## Comparing `django-customvueadmin-0.1.9.tar` & `django_customvueadmin-0.2.0.tar`

### file list

```diff
@@ -1,144 +1,133 @@
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.763549 django-customvueadmin-0.1.9/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      209 2024-04-11 14:26:38.000000 django-customvueadmin-0.1.9/MANIFEST.in
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2907 2024-04-11 16:02:21.763549 django-customvueadmin-0.1.9/PKG-INFO
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2057 2024-04-11 16:01:08.000000 django-customvueadmin-0.1.9/README.rst
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.746881 django-customvueadmin-0.1.9/custom_admin/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       45 2024-04-11 15:58:01.000000 django-customvueadmin-0.1.9/custom_admin/__init__.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.750214 django-customvueadmin-0.1.9/custom_admin/api/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/__init__.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.750214 django-customvueadmin-0.1.9/custom_admin/api/actions/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      139 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/actions/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      738 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/actions/delete_action.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2466 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/actions/export_csv_action.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2161 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/actions/view_actions_mixin.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.750214 django-customvueadmin-0.1.9/custom_admin/api/fields/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      370 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/fields/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      381 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/fields/base.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      706 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/fields/char.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1091 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/fields/choice.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3057 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/fields/files.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      157 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/fields/int.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      343 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/fields/numbers.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3871 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/fields/relation.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.750214 django-customvueadmin-0.1.9/custom_admin/api/filters/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      114 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/filters/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1558 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/filters/base_admin_filter.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/filters/choices.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.750214 django-customvueadmin-0.1.9/custom_admin/api/inlines/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      305 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/inlines/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      601 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/inlines/export_csv_inline.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1627 2024-04-09 09:57:39.000000 django-customvueadmin-0.1.9/custom_admin/api/inlines/inline_graph.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2129 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/inlines/inline_table.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       61 2024-03-29 18:33:05.000000 django-customvueadmin-0.1.9/custom_admin/api/inlines/inlines_type.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      135 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/inlines/interfaces.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4154 2024-04-02 18:13:36.000000 django-customvueadmin-0.1.9/custom_admin/api/inlines/view_inline_mixin.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      893 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/permissions.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.750214 django-customvueadmin-0.1.9/custom_admin/api/serializers/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      207 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/serializers/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5559 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/serializers/base_serializer.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      761 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/urls.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.750214 django-customvueadmin-0.1.9/custom_admin/api/views/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      509 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/views/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1984 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/views/admin_log.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5735 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/views/autocomplete.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     9283 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/views/base_admin_viewset.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      588 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/views/change_language.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      748 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/views/get_sections.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3440 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/views/token_auth.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      983 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/api/viewset_info.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.753548 django-customvueadmin-0.1.9/custom_admin/controllers/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-03-23 13:11:18.000000 django-customvueadmin-0.1.9/custom_admin/controllers/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3505 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/controllers/admin_log_manager.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3909 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/controllers/custom_metadata.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2911 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/controllers/filters_schema.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     8985 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/controllers/schema_generator.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.753548 django-customvueadmin-0.1.9/custom_admin/migrations/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1790 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.9/custom_admin/migrations/0001_initial.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1006 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.9/custom_admin/migrations/0002_auto_20220826_1734.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      751 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/migrations/0003_remove_adminlog_hall_alter_adminlog_staff.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.9/custom_admin/migrations/__init__.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.753548 django-customvueadmin-0.1.9/custom_admin/models/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       32 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.9/custom_admin/models/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1469 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/models/admin_log.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.746881 django-customvueadmin-0.1.9/custom_admin/static/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.753548 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.753548 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/css/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    27506 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/css/app.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      131 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/css/chunk-3ef8a5a8.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4748 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/css/chunk-7402f562.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      762 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/css/chunk-8b69702c.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1632 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/css/chunk-a7c7287a.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       71 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/css/chunk-ecedfa6a.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)   233306 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/css/chunk-elementUI.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    10292 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/css/chunk-fdcfea10.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3568 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/css/chunk-libs.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2238 2024-04-11 15:50:41.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/favicon.ico
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.753548 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/fonts/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    55956 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/fonts/element-icons.ttf
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    28200 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/fonts/element-icons.woff
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.753548 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/img/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    98071 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/img/404.png
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4766 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/img/404_cloud.png
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.756882 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/js/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    53669 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/js/app.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      925 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/js/chunk-2d0c14f9.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    11162 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/js/chunk-2d2080da.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    21542 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/js/chunk-3ef8a5a8.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)   122331 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/js/chunk-5148deb9.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)   200033 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/js/chunk-6786f71b.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1792 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/js/chunk-7402f562.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    39131 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/js/chunk-8b69702c.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4166 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/js/chunk-a7c7287a.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3542 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/js/chunk-ecedfa6a.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)   672429 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/js/chunk-elementUI.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)   215439 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/js/chunk-fdcfea10.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)   579815 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/js/chunk-libs.js
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3273 2024-04-11 16:01:04.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/js/runtime.js
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.756882 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.760216 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/dark-first/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4788 2024-04-11 15:50:47.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/dark-first/content.min.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    50376 2024-04-11 15:50:47.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/dark-first/skin.min.css
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.760216 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/dark-slim/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4730 2024-04-11 15:50:47.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/dark-slim/content.min.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    49965 2024-04-11 15:50:47.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/dark-slim/skin.min.css
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.760216 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/img/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    14708 2024-04-11 15:50:47.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/img/example.png
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    15764 2024-04-11 15:50:47.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/img/tinymce.woff2
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.760216 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/lightgray/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3193 2024-04-11 15:50:47.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/lightgray/content.min.css
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.760216 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/lightgray/fonts/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     7664 2024-04-11 15:50:47.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/lightgray/fonts/tinymce.woff
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)    38232 2024-04-11 15:50:47.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/lightgray/skin.min.css
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.746881 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/plugins/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.760216 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/plugins/accordion/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.760216 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/plugins/accordion/css/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-04-11 15:50:47.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/plugins/accordion/css/accordion.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1251 2024-04-11 15:50:47.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/plugins/accordion/plugin.js
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.746881 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/plugins/codesample/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.760216 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1736 2024-04-11 15:50:47.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/prism.css
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1171290 2024-04-11 15:50:47.000000 django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/tinymce.min.js
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.746881 django-customvueadmin-0.1.9/custom_admin/templates/
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.760216 django-customvueadmin-0.1.9/custom_admin/templates/custom_admin/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3369 2024-04-11 14:42:58.000000 django-customvueadmin-0.1.9/custom_admin/templates/custom_admin/admin_index.html
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.760216 django-customvueadmin-0.1.9/custom_admin/tests/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.9/custom_admin/tests/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      581 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.9/custom_admin/tests/test_language.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      460 2024-03-11 07:49:25.000000 django-customvueadmin-0.1.9/custom_admin/tests/test_scheme_get.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.763549 django-customvueadmin-0.1.9/custom_admin/utils/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       35 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/utils/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2425 2024-04-09 09:57:39.000000 django-customvueadmin-0.1.9/custom_admin/utils/colors.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      570 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/utils/get_schema.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      593 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/utils/register_admin_viewsets.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.763549 django-customvueadmin-0.1.9/custom_admin/views/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       40 2024-03-27 15:35:55.000000 django-customvueadmin-0.1.9/custom_admin/views/__init__.py
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1327 2024-04-11 14:32:14.000000 django-customvueadmin-0.1.9/custom_admin/views/admin_page.py
-drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 16:02:21.763549 django-customvueadmin-0.1.9/django_customvueadmin.egg-info/
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2907 2024-04-11 16:02:21.000000 django-customvueadmin-0.1.9/django_customvueadmin.egg-info/PKG-INFO
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4852 2024-04-11 16:02:21.000000 django-customvueadmin-0.1.9/django_customvueadmin.egg-info/SOURCES.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-04-11 16:02:21.000000 django-customvueadmin-0.1.9/django_customvueadmin.egg-info/dependency_links.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-04-11 14:11:51.000000 django-customvueadmin-0.1.9/django_customvueadmin.egg-info/not-zip-safe
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-04-11 16:02:21.000000 django-customvueadmin-0.1.9/django_customvueadmin.egg-info/requires.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)       13 2024-04-11 16:02:21.000000 django-customvueadmin-0.1.9/django_customvueadmin.egg-info/top_level.txt
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      222 2024-04-11 09:22:36.000000 django-customvueadmin-0.1.9/pyproject.toml
--rw-r--r--   0 honnisha  (1000) honnisha  (1000)      992 2024-04-11 16:02:21.763549 django-customvueadmin-0.1.9/setup.cfg
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.140870 django_customvueadmin-0.2.0/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1073 2024-04-26 14:57:56.000000 django_customvueadmin-0.2.0/LICENSE
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      209 2024-04-11 14:26:38.000000 django_customvueadmin-0.2.0/MANIFEST.in
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2812 2024-05-27 08:40:47.140870 django_customvueadmin-0.2.0/PKG-INFO
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1979 2024-05-27 08:39:38.000000 django_customvueadmin-0.2.0/README.rst
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.114200 django_customvueadmin-0.2.0/custom_admin/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       45 2024-05-27 07:51:30.000000 django_customvueadmin-0.2.0/custom_admin/__init__.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.117534 django_customvueadmin-0.2.0/custom_admin/api/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       86 2024-04-19 14:02:39.000000 django_customvueadmin-0.2.0/custom_admin/api/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1529 2024-05-25 10:30:35.000000 django_customvueadmin-0.2.0/custom_admin/api/action_functions.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.117534 django_customvueadmin-0.2.0/custom_admin/api/actions/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      139 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/api/actions/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      985 2024-05-25 10:29:03.000000 django_customvueadmin-0.2.0/custom_admin/api/actions/delete_action.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2538 2024-05-24 12:45:37.000000 django_customvueadmin-0.2.0/custom_admin/api/actions/export_csv_action.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2723 2024-05-24 15:46:18.000000 django_customvueadmin-0.2.0/custom_admin/api/actions/view_actions_mixin.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1724 2024-05-22 00:15:55.000000 django_customvueadmin-0.2.0/custom_admin/api/backends.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.120868 django_customvueadmin-0.2.0/custom_admin/api/fields/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      403 2024-05-06 15:09:48.000000 django_customvueadmin-0.2.0/custom_admin/api/fields/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      381 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/api/fields/base.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      811 2024-04-23 15:22:53.000000 django_customvueadmin-0.2.0/custom_admin/api/fields/char.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1233 2024-04-23 15:23:30.000000 django_customvueadmin-0.2.0/custom_admin/api/fields/choice.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3695 2024-05-26 16:28:48.000000 django_customvueadmin-0.2.0/custom_admin/api/fields/files.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      157 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/api/fields/int.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      326 2024-05-06 16:10:42.000000 django_customvueadmin-0.2.0/custom_admin/api/fields/json.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      343 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/api/fields/numbers.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3871 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/api/fields/relation.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.120868 django_customvueadmin-0.2.0/custom_admin/api/filters/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      165 2024-05-21 23:11:51.000000 django_customvueadmin-0.2.0/custom_admin/api/filters/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1623 2024-05-21 23:13:58.000000 django_customvueadmin-0.2.0/custom_admin/api/filters/base_admin_filter.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/api/filters/choices.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      733 2024-05-22 00:17:36.000000 django_customvueadmin-0.2.0/custom_admin/api/filters/date_range.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1445 2024-05-08 17:32:46.000000 django_customvueadmin-0.2.0/custom_admin/api/inline_relation.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.124202 django_customvueadmin-0.2.0/custom_admin/api/inlines/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      305 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/api/inlines/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      601 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/api/inlines/export_csv_inline.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1595 2024-05-21 13:46:54.000000 django_customvueadmin-0.2.0/custom_admin/api/inlines/inline_graph.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2129 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/api/inlines/inline_table.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       61 2024-03-29 18:33:05.000000 django_customvueadmin-0.2.0/custom_admin/api/inlines/inlines_type.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      135 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/api/inlines/interfaces.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4154 2024-04-02 18:13:36.000000 django_customvueadmin-0.2.0/custom_admin/api/inlines/view_inline_mixin.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      893 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/api/permissions.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.124202 django_customvueadmin-0.2.0/custom_admin/api/serializers/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      207 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/api/serializers/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      737 2024-04-19 13:32:46.000000 django_customvueadmin-0.2.0/custom_admin/api/serializers/auth_response.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5491 2024-05-06 15:09:50.000000 django_customvueadmin-0.2.0/custom_admin/api/serializers/base_serializer.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.124202 django_customvueadmin-0.2.0/custom_admin/api/tests/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-03-11 07:49:25.000000 django_customvueadmin-0.2.0/custom_admin/api/tests/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2317 2024-05-21 23:39:40.000000 django_customvueadmin-0.2.0/custom_admin/api/tests/test_filters.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      517 2024-05-21 20:22:03.000000 django_customvueadmin-0.2.0/custom_admin/api/tests/test_scheme_get.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      550 2024-05-21 19:31:58.000000 django_customvueadmin-0.2.0/custom_admin/api/tests/urls.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      599 2024-05-26 18:19:08.000000 django_customvueadmin-0.2.0/custom_admin/api/urls.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.124202 django_customvueadmin-0.2.0/custom_admin/api/views/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      414 2024-05-21 19:10:33.000000 django_customvueadmin-0.2.0/custom_admin/api/views/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     5829 2024-05-26 20:56:51.000000 django_customvueadmin-0.2.0/custom_admin/api/views/autocomplete.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     8432 2024-05-26 18:11:53.000000 django_customvueadmin-0.2.0/custom_admin/api/views/base_admin_viewset.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.127535 django_customvueadmin-0.2.0/custom_admin/api/views/defaults/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      131 2024-05-21 19:10:56.000000 django_customvueadmin-0.2.0/custom_admin/api/views/defaults/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2080 2024-05-21 19:58:42.000000 django_customvueadmin-0.2.0/custom_admin/api/views/defaults/admin_log.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      366 2024-05-21 19:06:40.000000 django_customvueadmin-0.2.0/custom_admin/api/views/defaults/groups.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      529 2024-05-21 19:09:36.000000 django_customvueadmin-0.2.0/custom_admin/api/views/defaults/permissions.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      909 2024-04-23 23:45:01.000000 django_customvueadmin-0.2.0/custom_admin/api/views/get_sections.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1517 2024-04-11 17:29:22.000000 django_customvueadmin-0.2.0/custom_admin/api/views/token_auth.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      974 2024-05-08 17:32:54.000000 django_customvueadmin-0.2.0/custom_admin/api/viewset_info.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.127535 django_customvueadmin-0.2.0/custom_admin/controllers/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       47 2024-04-19 14:01:33.000000 django_customvueadmin-0.2.0/custom_admin/controllers/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3475 2024-05-20 10:10:21.000000 django_customvueadmin-0.2.0/custom_admin/controllers/admin_log_manager.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3823 2024-05-26 16:40:34.000000 django_customvueadmin-0.2.0/custom_admin/controllers/custom_metadata.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3078 2024-05-20 19:45:54.000000 django_customvueadmin-0.2.0/custom_admin/controllers/filters_schema.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     9232 2024-05-24 13:28:46.000000 django_customvueadmin-0.2.0/custom_admin/controllers/schema_generator.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.127535 django_customvueadmin-0.2.0/custom_admin/management/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-04-15 16:06:07.000000 django_customvueadmin-0.2.0/custom_admin/management/__init__.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.127535 django_customvueadmin-0.2.0/custom_admin/management/commands/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-04-15 16:06:19.000000 django_customvueadmin-0.2.0/custom_admin/management/commands/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1300 2024-04-15 16:52:15.000000 django_customvueadmin-0.2.0/custom_admin/management/commands/custom_admin_viewsets_list.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.127535 django_customvueadmin-0.2.0/custom_admin/migrations/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1695 2024-04-11 18:20:54.000000 django_customvueadmin-0.2.0/custom_admin/migrations/0001_initial.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        0 2024-04-11 18:20:54.000000 django_customvueadmin-0.2.0/custom_admin/migrations/__init__.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.127535 django_customvueadmin-0.2.0/custom_admin/models/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       32 2024-03-11 07:49:25.000000 django_customvueadmin-0.2.0/custom_admin/models/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1469 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/models/admin_log.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.110867 django_customvueadmin-0.2.0/custom_admin/static/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.134203 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2238 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/favicon.ico
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)   752706 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/index-C4Cutzkc.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1681833 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/index-OjzvLInB.js
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)   385360 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/materialdesignicons-webfont-CYDMK1kx.woff2
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)   561776 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/materialdesignicons-webfont-CgCzGbLl.woff
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1243500 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/materialdesignicons-webfont-D3kAzl71.ttf
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1243720 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/materialdesignicons-webfont-DttUABo4.eot
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.134203 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.137536 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/dark-first/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4788 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/dark-first/content.min.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    50376 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/dark-first/skin.min.css
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.137536 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/dark-slim/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4730 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/dark-slim/content.min.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    49965 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/dark-slim/skin.min.css
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.137536 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/img/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    14708 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/img/example.png
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    15764 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/img/tinymce.woff2
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.137536 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/lightgray/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     3193 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/lightgray/content.min.css
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.137536 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/lightgray/fonts/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     7664 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/lightgray/fonts/tinymce.woff
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)    38232 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/lightgray/skin.min.css
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.114200 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/plugins/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.137536 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/plugins/accordion/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.137536 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/plugins/accordion/css/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      282 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/plugins/accordion/css/accordion.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1251 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/plugins/accordion/plugin.js
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.114200 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/plugins/codesample/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.137536 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1736 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/prism.css
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)  1171290 2024-05-27 08:39:25.000000 django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/tinymce.min.js
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.114200 django_customvueadmin-0.2.0/custom_admin/templates/
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.137536 django_customvueadmin-0.2.0/custom_admin/templates/custom_admin/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1309 2024-05-27 08:38:31.000000 django_customvueadmin-0.2.0/custom_admin/templates/custom_admin/admin_index.html
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.140870 django_customvueadmin-0.2.0/custom_admin/utils/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       35 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/utils/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1976 2024-04-11 17:58:41.000000 django_customvueadmin-0.2.0/custom_admin/utils/async_mixin.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2425 2024-04-09 09:57:39.000000 django_customvueadmin-0.2.0/custom_admin/utils/colors.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      570 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/utils/get_schema.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      593 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/utils/register_admin_viewsets.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.140870 django_customvueadmin-0.2.0/custom_admin/views/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       40 2024-03-27 15:35:55.000000 django_customvueadmin-0.2.0/custom_admin/views/__init__.py
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1769 2024-04-15 18:01:09.000000 django_customvueadmin-0.2.0/custom_admin/views/admin_page.py
+drwxr-xr-x   0 honnisha  (1000) honnisha  (1000)        0 2024-05-27 08:40:47.140870 django_customvueadmin-0.2.0/django_customvueadmin.egg-info/
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     2812 2024-05-27 08:40:47.000000 django_customvueadmin-0.2.0/django_customvueadmin.egg-info/PKG-INFO
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     4196 2024-05-27 08:40:47.000000 django_customvueadmin-0.2.0/django_customvueadmin.egg-info/SOURCES.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-05-27 08:40:47.000000 django_customvueadmin-0.2.0/django_customvueadmin.egg-info/dependency_links.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)        1 2024-05-27 08:40:46.000000 django_customvueadmin-0.2.0/django_customvueadmin.egg-info/not-zip-safe
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)       13 2024-05-27 08:40:47.000000 django_customvueadmin-0.2.0/django_customvueadmin.egg-info/top_level.txt
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)      222 2024-04-11 09:22:36.000000 django_customvueadmin-0.2.0/pyproject.toml
+-rw-r--r--   0 honnisha  (1000) honnisha  (1000)     1000 2024-05-27 08:40:47.140870 django_customvueadmin-0.2.0/setup.cfg
```

### Comparing `django-customvueadmin-0.1.9/PKG-INFO` & `django_customvueadmin-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: django-customvueadmin
-Version: 0.1.9
-Summary: A custom admin interface providing backend via DRF and frontend via Vue and Element UI that tries Keep It Simple.
+Version: 0.2.0
+Summary: A custom admin interface providing backend via DRF and frontend via Vue and Element UI that tries to Keep It Simple.
 Home-page: https://innova-group-llc.github.io/custom_admin_docs/
 License: BSD-3-Clause
 Project-URL: Documentation, https://innova-group-llc.github.io/custom_admin_docs/
 Project-URL: Source, https://github.com/Innova-Group-LLC/custom_admin
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.10
-Provides-Extra: argon2
-Requires-Dist: argon2-cffi>=19.1.0; extra == "argon2"
-Provides-Extra: bcrypt
-Requires-Dist: bcrypt; extra == "bcrypt"
+Requires-Python: >=3.8
+License-File: LICENSE
 
 Django Custom Admin
 ===================
 
 |logo|
 
 A custom admin interface providing backend via DRF and frontend via Vue
-and Element UI that tries Keep It Simple.
+and Element UI that tries to Keep It Simple.
 
 |PyPI version| |GitHub stars|
 
 `Documentation <https://innova-group-llc.github.io/custom_admin_docs/>`__
 
 Features
 --------
@@ -60,18 +59,17 @@
 Build
 -----
 
 ::
 
    npm run build --prefix vue_frontend
    rm -r custom_admin/static/custom_admin/*
-   cp vue_frontend/dist/favicon.ico custom_admin/static/custom_admin/favicon.ico
-   cp vue_frontend/dist/manifest.json custom_admin/static/custom_admin/manifest.json
-   cp -r vue_frontend/dist/tinymce/ custom_admin/static/custom_admin/tinymce/
-   cp -r vue_frontend/dist/static/ custom_admin/
+   rm -r custom_admin/templates/custom_admin/admin_index.html
+   cp vue_frontend/dist/index.html custom_admin/templates/custom_admin/admin_index.html
+   cp -r vue_frontend/dist/custom_admin/ custom_admin/static/
 
 .. |logo| image:: https://github.com/Innova-Group-LLC/custom_admin/blob/master/logo.png?raw=true
    :target: https://innova-group-llc.github.io/custom_admin_docs/
 .. |PyPI version| image:: https://badge.fury.io/py/django-customvueadmin.svg
    :target: https://pypi.org/project/django-customvueadmin/
 .. |GitHub stars| image:: https://img.shields.io/github/stars/Innova-Group-LLC/custom_admin
    :target: https://github.com/Innova-Group-LLC/custom_admin
```

### Comparing `django-customvueadmin-0.1.9/README.rst` & `django_customvueadmin-0.2.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Django Custom Admin
 ===================
 
 |logo|
 
 A custom admin interface providing backend via DRF and frontend via Vue
-and Element UI that tries Keep It Simple.
+and Element UI that tries to Keep It Simple.
 
 |PyPI version| |GitHub stars|
 
 `Documentation <https://innova-group-llc.github.io/custom_admin_docs/>`__
 
 Features
 --------
@@ -41,18 +41,17 @@
 Build
 -----
 
 ::
 
    npm run build --prefix vue_frontend
    rm -r custom_admin/static/custom_admin/*
-   cp vue_frontend/dist/favicon.ico custom_admin/static/custom_admin/favicon.ico
-   cp vue_frontend/dist/manifest.json custom_admin/static/custom_admin/manifest.json
-   cp -r vue_frontend/dist/tinymce/ custom_admin/static/custom_admin/tinymce/
-   cp -r vue_frontend/dist/static/ custom_admin/
+   rm -r custom_admin/templates/custom_admin/admin_index.html
+   cp vue_frontend/dist/index.html custom_admin/templates/custom_admin/admin_index.html
+   cp -r vue_frontend/dist/custom_admin/ custom_admin/static/
 
 .. |logo| image:: https://github.com/Innova-Group-LLC/custom_admin/blob/master/logo.png?raw=true
    :target: https://innova-group-llc.github.io/custom_admin_docs/
 .. |PyPI version| image:: https://badge.fury.io/py/django-customvueadmin.svg
    :target: https://pypi.org/project/django-customvueadmin/
 .. |GitHub stars| image:: https://img.shields.io/github/stars/Innova-Group-LLC/custom_admin
    :target: https://github.com/Innova-Group-LLC/custom_admin
```

### Comparing `django-customvueadmin-0.1.9/custom_admin/api/actions/delete_action.py` & `django_customvueadmin-0.2.0/custom_admin/api/actions/delete_action.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-import typing
-
 from django.db.models.deletion import ProtectedError
 from django.utils.translation import gettext as _
 
+from custom_admin.api.action_functions import admin_action
+
 
+@admin_action(
+    short_description=_("Удалить"),
+    icon='mdi-delete-forever',
+    base_color='#ff3333',
+    variant='outlined',
+    confirmation_text=_('Вы уверены, что хотите удалить выбранные записи?'),
+)
 def delete_action(view, request, queryset, *args, **kwargs):
     try:
         queryset.delete()
     except ProtectedError as e:
         return _(
             'Невозможно удалить некоторые экземпляры модели, '
             'поскольку на них ссылаются через защищенные внешние ключи: %(objects)s') % {
                    'objects': ", ".join([str(obj) for obj in e.protected_objects])
                }, 400
 
     return _('Записи успешно удалены!'), 200
-
-
-delete_action.short_description = _("Удалить")
```

### Comparing `django-customvueadmin-0.1.9/custom_admin/api/actions/export_csv_action.py` & `django_customvueadmin-0.2.0/custom_admin/api/actions/export_csv_action.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import datetime
 import typing
 from io import BytesIO
 
-import unicodecsv as csv
 from django.http import HttpResponse
 from django.utils.translation import gettext_lazy as _
 
+from custom_admin.api.action_functions import admin_action
+
 
 def get_list_display(view):
     list_display = getattr(view, 'list_display', None)
     if list_display:
         return list_display
 
     meta = view.metadata_class()
@@ -37,28 +38,33 @@
             headers.append(column)
 
     return headers
 
 
 def base_export_csv(filename: str, columns: typing.List, lines: typing.List):
     f = BytesIO()
+    import unicodecsv as csv
     writer = csv.writer(f, dialect=csv.excel, encoding='utf-8')
     writer.writerow(columns)
 
     for line in lines:
         writer.writerow(line)
     f.seek(0)
 
     response = HttpResponse(f, content_type='text/csv')
     response['Pragma'] = filename
     response['Content-Disposition'] = f'attachment; filename="{filename}"'
     f.close()
     return response
 
 
+@admin_action(
+    short_description=_("Выгрузить в csv"),
+    icon='mdi-application-export',
+)
 def export_csv_action(view, request, queryset, *args, **kwargs):
     serializer_class = view.get_serializer_class()
     serializer = serializer_class(queryset, many=True, context={'request': request})
 
     columns = _get_headers(view, serializer, serializer_class)
     filename = f'{view.get_view_viewname()}_{datetime.datetime.now()}.csv'
 
@@ -72,10 +78,7 @@
                 value = value.get('text', value)
 
             line_data.append(value)
 
         lines.append(line_data)
 
     return base_export_csv(filename, columns, lines)
-
-
-export_csv_action.short_description = _("Выгрузить в csv (кодировка UTF-8)")
```

### Comparing `django-customvueadmin-0.1.9/custom_admin/api/actions/view_actions_mixin.py` & `django_customvueadmin-0.2.0/custom_admin/api/actions/view_actions_mixin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 import asyncio as aio
 import logging
 
 from asgiref.sync import sync_to_async
 from django.http import HttpResponse
+from rest_framework import serializers
 from rest_framework.decorators import action
 from rest_framework.response import Response
 
 from custom_admin.api.actions.delete_action import delete_action
 from custom_admin.api.actions.export_csv_action import export_csv_action
 from custom_admin.controllers import AdminLogManager
 
 log = logging.getLogger('admin')
 
 
+class ActionSerializer(serializers.Serializer):
+    action = serializers.CharField(required=True)
+    ids = serializers.ListField(child=serializers.CharField(), required=False)
+    send_to_all = serializers.BooleanField(default=False)
+    form_data = serializers.JSONField(required=False, allow_null=True)
+
+
 class AdminActionMixIn:
 
     actions = [
         delete_action, export_csv_action,
     ]
 
     @action(detail=False, methods=['post'])
     async def send_action(self, request, pk=None):
-        action_name = request.data['action']
-        ids = request.data['ids']
-        send_to_all = request.data['send_to_all']
-        form_data = request.data['form_data']
+        serializer = ActionSerializer(data=request.data)
+        serializer.is_valid(raise_exception=True)
+
+        action_name = serializer.validated_data['action']
+        ids = serializer.validated_data['ids']
+        send_to_all = serializer.validated_data['send_to_all']
+        form_data = serializer.validated_data['form_data']
 
         actions_dict = {
             action.__name__: action
             for action in self.actions
         }
 
         if action_name not in actions_dict:
@@ -44,15 +55,15 @@
             action_fn = sync_to_async(action_fn)
 
         actions_result = await action_fn(self, request, qs, form_data)
 
         if isinstance(actions_result, (tuple, list)):
             action_messages, code = actions_result
 
-            if isinstance(action_messages, str):
+            if isinstance(action_messages, (str)) or action_messages.__class__.__name__ == '__proxy__':
                 action_messages = [action_messages]
 
             action_request = Response({'action_messages': action_messages}, status=code)
 
         elif isinstance(actions_result, (Response, HttpResponse)):
             action_request = actions_result
```

### Comparing `django-customvueadmin-0.1.9/custom_admin/api/fields/char.py` & `django_customvueadmin-0.2.0/custom_admin/api/fields/char.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import typing
+
 from rest_framework import serializers
 
 from .base import AdminBaseFieldMixin
 
 
 class AdminCharField(AdminBaseFieldMixin, serializers.CharField):
     '''
@@ -9,12 +11,14 @@
     визуального редактора текста. Он сохраняет текст в формате html.
 
     multilined - для отображения текстового поля в несколько строк
     '''
 
     wysiwyg: bool
     multilined: bool
+    tag_style: typing.Optional[dict]
 
     def __init__(self, **kwargs):
         self.wysiwyg = kwargs.pop('wysiwyg', False)
+        self.tag_style = kwargs.pop('tag_style', {})
         self.multilined = kwargs.pop('multilined', False)
         super().__init__(**kwargs)
```

### Comparing `django-customvueadmin-0.1.9/custom_admin/api/fields/choice.py` & `django_customvueadmin-0.2.0/custom_admin/api/fields/choice.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,20 @@
-from rest_framework import serializers
+import typing
+
 from django.utils.translation import gettext as _
+from rest_framework import serializers
 
 
 class AdminChoiceField(serializers.ChoiceField):
+    tag_style: typing.Optional[dict]
+    max_width: typing.Optional[int]
+
     def __init__(self, *args, **kwargs):
         kwargs.pop("child", None)
+        self.tag_style = kwargs.pop('tag_style', {})
         self.max_width = kwargs.pop("max_width", None)
         super().__init__(*args, **kwargs)
 
     def to_representation(self, value):
         if isinstance(value, list):
             return value
```

### Comparing `django-customvueadmin-0.1.9/custom_admin/api/fields/files.py` & `django_customvueadmin-0.2.0/custom_admin/api/fields/files.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,36 +7,59 @@
 from django.core.exceptions import ValidationError
 from django.core.files.uploadedfile import UploadedFile
 from django.forms import FileField as DjangoFileField
 from django.utils.translation import gettext as _
 from rest_framework import fields, serializers
 
 
+class Base64Serializer(serializers.Serializer):
+    name = serializers.CharField(required=False)
+    file = serializers.CharField(required=False)
+
+    def validate_file(self, file):
+        if not file.startswith('data:image'):
+            raise ValidationError('Bad base64 format')
+        return file
+
+
 class Base64FileField(fields.FileField):
+    list_preview: bool = False
+
+    def __init__(self, *args, **kwargs):
+        self.list_preview = kwargs.pop('list_preview', False)
+        super().__init__(*args, **kwargs)
+
     def to_internal_value(self, data):
-        if not isinstance(data, str):
-            return super().to_internal_value(data)
+        if not data:
+            return
+
+        serializer = Base64Serializer(data=data)
+        serializer.is_valid(raise_exception=True)
 
-        file_name, content_type, base64_str = data.split(",")
+        content_type, base64_str = serializer.validated_data['file'].split(",")
         upload_file = io.BytesIO(base64.b64decode(base64_str))
         file_object = UploadedFile(
             file=upload_file,
-            name=file_name,
+            name=serializer.validated_data['name'],
             content_type=content_type,
             size=sys.getsizeof(upload_file),
         )
         return super().to_internal_value(file_object)
 
-    def to_representation(self, value):
-        url = super().to_representation(value)
+    def to_representation(self, file):
+        url = super().to_representation(file)
         if not url:
             return url
+
         request = self.context['request']
-        url = request.build_absolute_uri(url)
-        return urllib.parse.unquote(url)
+        url = urllib.parse.unquote(request.build_absolute_uri(url))
+        return {
+            'name': file.name,
+            'url': url,
+        }
 
 
 def validate_image_file_extension(value):
     additional = ['svg']
     return validators.FileExtensionValidator(
         allowed_extensions=validators.get_available_image_extensions() + additional
     )(value)
```

### Comparing `django-customvueadmin-0.1.9/custom_admin/api/fields/relation.py` & `django_customvueadmin-0.2.0/custom_admin/api/fields/relation.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.9/custom_admin/api/filters/base_admin_filter.py` & `django_customvueadmin-0.2.0/custom_admin/api/filters/base_admin_filter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from collections import OrderedDict
 
 from django.db import models
-from django_filters import filters, filterset, fields
+from django_filters import filters, filterset
 from django_filters import rest_framework as drf_filters
 from rest_framework import fields as drf_fields
 
+from custom_admin.api.filters.date_range import AdminDateFromToRangeFilter
+
 
 class AdminFilterSetMetaclass(filterset.FilterSetMetaclass):
     @classmethod
     def get_declared_filters(cls, bases, attrs):
         new_filters = [
             (filter_name, attrs.pop(filter_name))
             for filter_name, obj in list(attrs.items())
@@ -39,9 +41,9 @@
     FILTER_DEFAULTS[models.ForeignKey] = {
         'filter_class': filters.ModelMultipleChoiceFilter,
         'extra': lambda f: {
             'queryset': filterset.remote_queryset(f),
         }
     }
     FILTER_DEFAULTS[models.DateTimeField] = {
-        'filter_class': filters.DateFromToRangeFilter,
+        'filter_class': AdminDateFromToRangeFilter,
     }
```

### Comparing `django-customvueadmin-0.1.9/custom_admin/api/inlines/export_csv_inline.py` & `django_customvueadmin-0.2.0/custom_admin/api/inlines/export_csv_inline.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.9/custom_admin/api/inlines/inline_graph.py` & `django_customvueadmin-0.2.0/custom_admin/api/inlines/inline_graph.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,18 +12,16 @@
         'intersect': False,
     },
 }
 
 
 @dataclass
 class ChartOptions:
-    width: int = 400
-    height: int = 400
-    responsive: bool = True
-    maintainAspectRatio: bool = False
+    width: typing.Optional[int] = None
+    height: typing.Optional[int] = 80
 
     plugins: typing.Dict[str, dict] = field(default_factory=lambda: PLUGINS)
 
 
 @dataclass
 class GraphDataset:
     # читаемое название
```

### Comparing `django-customvueadmin-0.1.9/custom_admin/api/inlines/inline_table.py` & `django_customvueadmin-0.2.0/custom_admin/api/inlines/inline_table.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.9/custom_admin/api/inlines/view_inline_mixin.py` & `django_customvueadmin-0.2.0/custom_admin/api/inlines/view_inline_mixin.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.9/custom_admin/api/permissions.py` & `django_customvueadmin-0.2.0/custom_admin/api/permissions.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.9/custom_admin/api/serializers/base_serializer.py` & `django_customvueadmin-0.2.0/custom_admin/api/serializers/base_serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import logging
 
-from django.db import models
-from modeltranslation.translator import translator
-from modeltranslation.utils import get_translation_fields
 from rest_framework import relations, serializers
 
-from backend.fields import models as custom_model_fields
+from django.db import models
+
 from custom_admin.api import fields
-from custom_admin.api import fields as admin_fields
 from custom_admin.controllers import AdminLogManager
 
 log = logging.getLogger("custom_admin")
 
 
 class AdminFieldsMixin:
     serializer_related_field = fields.AdminPrimaryKeyRelatedField
@@ -19,17 +16,17 @@
     serializer_choice_field = fields.AdminChoiceField
 
     serializer_field_mapping = serializers.ModelSerializer.serializer_field_mapping
     serializer_field_mapping[models.FileField] = fields.Base64FileField
     serializer_field_mapping[models.ImageField] = fields.Base64ImageField
     serializer_field_mapping[models.CharField] = fields.AdminCharField
     serializer_field_mapping[models.TextField] = fields.AdminCharField
+    serializer_field_mapping[models.JSONField] = fields.AdminJsonField
 
-    serializer_field_mapping[models.PositiveIntegerField] = admin_fields.PositiveIntegerField
-    serializer_field_mapping[custom_model_fields.PositiveDecimalField] = admin_fields.PositiveDecimalField
+    serializer_field_mapping[models.PositiveIntegerField] = fields.PositiveIntegerField
 
 
 class AdminSerializer(AdminFieldsMixin, serializers.Serializer):
     pass
 
 
 class AdminModelSerializer(AdminFieldsMixin, serializers.ModelSerializer):
@@ -51,25 +48,28 @@
         return obj
 
 
 class TranslatedModelSerializer(AdminModelSerializer):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
+        from modeltranslation.translator import translator
         self.trans_opts = translator.get_options_for_model(self.Meta.model)
 
     def get_field_names(self, declared_fields, info):
+        from modeltranslation.utils import get_translation_fields
         result = super().get_field_names(declared_fields, info)
         for f in self.trans_opts.fields:
             trans_fields = get_translation_fields(f)
             result += tuple(trans_fields)
 
         return result
 
     def get_extra_kwargs(self):
+        from modeltranslation.utils import get_translation_fields
         extra_kwargs = super().get_extra_kwargs()
         for field in self.trans_opts.fields:
 
             if field not in extra_kwargs:
                 extra_kwargs[field] = {}
 
             extra_kwargs[field]['required'] = False
```

### Comparing `django-customvueadmin-0.1.9/custom_admin/api/views/admin_log.py` & `django_customvueadmin-0.2.0/custom_admin/api/views/defaults/admin_log.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django.utils.functional import lazy
 from django.utils.translation import gettext_lazy as _
 from rest_framework import serializers
 
 from custom_admin.api import filters as admin_filters
-from custom_admin.models import AdminLog
 from custom_admin.api.serializers.base_serializer import AdminModelSerializer
 from custom_admin.api.views.base_admin_viewset import WithoutCreateBaseAdminViewSet
+from custom_admin.models import AdminLog
 
 
 def get_views_choices():
     from custom_admin.utils.register_admin_viewsets import _ADMIN_VIEWS
     return [
         (viewname, f'{view._info.title} - {view.get_view_title()}')
         for viewname, view in _ADMIN_VIEWS.items()
@@ -20,26 +20,34 @@
     section = admin_filters.ChoiceFilter(
         label=_('Раздел'), choices=lazy(get_views_choices, tuple),
     )
 
     class Meta:
         model = AdminLog
         fields = (
-            'section', 'staff', 'action_type', 'created_at',
+            'section',
+            'staff',
+            'action_type',
+            'created_at',
         )
 
 
 class AdminLogAdminSerializer(AdminModelSerializer):
     section = serializers.SerializerMethodField(label=_('Раздел'))
 
     class Meta:
         model = AdminLog
         fields = '__all__'
         read_only_fields = (
-            'content', 'created_at', 'section', 'action_type', 'staff', 'title',
+            'content',
+            'created_at',
+            'section',
+            'action_type',
+            'staff',
+            'title',
         )
 
     def get_section(self, obj):
         from custom_admin.utils.register_admin_viewsets import _ADMIN_VIEWS
         view = _ADMIN_VIEWS.get(obj.section)
         if not view:
             return obj.section
```

### Comparing `django-customvueadmin-0.1.9/custom_admin/api/views/autocomplete.py` & `django_customvueadmin-0.2.0/custom_admin/api/views/autocomplete.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,33 +7,43 @@
 from django.db.models import Manager, Q
 from django.db.models.query import QuerySet
 from django_filters.utils import get_model_field
 from rest_framework import serializers
 from rest_framework.response import Response
 from rest_framework.views import APIView
 
-from api.permissions import IsStaffPermission
+from custom_admin.api.permissions import AdminPermission
 
 log = logging.getLogger("admin")
 
 INT_FIELDS = (
     models.PositiveIntegerField,
     models.IntegerField,
     models.AutoField,
     models.BigIntegerField,
 )
 
 
-class ModelNotFound(Exception):
-    pass
+class AutoCompeteSerializer(serializers.Serializer):
+    viewname = serializers.CharField(required=False)
+    field_slug = serializers.JSONField(required=False)
+
+    search_string = serializers.CharField(required=False, allow_null=True, allow_blank=True)
+    limit = serializers.IntegerField(required=False, allow_null=True)
+    existed_choices = serializers.ListField(
+        child=serializers.IntegerField(),
+        required=False,
+        allow_empty=True,
+        allow_null=True,
+    )
 
 
 class AutoCompeteView(APIView):
     throttle_classes = []
-    permission_classes = (IsStaffPermission,)
+    permission_classes = (AdminPermission,)
 
     default_fields = {
         'Permission': ('id', 'codename', 'name'),
         'Group': ('id', 'name'),
         'Country': ('id', 'name', 'alt_names__name'),
         'City': ('id', 'name', 'alt_names__name'),
         'ContentType': ('id', 'model', 'app_label')
@@ -68,107 +78,96 @@
                 filters.append(field_filter)
 
         if not filters:
             return None
 
         return reduce(operator.or_, filters)
 
-    def get_model(self, request):
-        app_label = request.data.get('app_label')
-        if not app_label:
-            raise ModelNotFound('app_label is required field')
-
-        model_name = request.data.get('model_name')
-        if not model_name:
-            raise ModelNotFound('model_name is required field')
+    def get_queryset_by_view(self, model, viewname, form_data, field_slug):
 
-        model = apps.get_model(app_label=app_label, model_name=model_name)
-        if not model:
-            raise ModelNotFound(f'Model {app_label}.{model_name} not found')
+        if not viewname:
+            return model.objects.all()
+
+        from custom_admin.utils.register_admin_viewsets import _ADMIN_VIEWS
+        view = _ADMIN_VIEWS[viewname]
+        serializer = view.get_serializer_class()()
+
+        field = serializer.fields.get(field_slug)
+        if not field:
+            raise serializers.ValidationError(f'Model {self.app_label}.{self.model_name} view "{viewname}" field slug "{field_slug}" is not found')
+
+        if isinstance(field, serializers.ManyRelatedField):
+            field = field.child_relation
 
-        return model
+        filter_queryset = getattr(field, 'filter_queryset', None)
+        qs = getattr(field, 'queryset')
 
-    def get_queryset_by_view(self, model, request):
-        viewname = request.data.get('viewname')
-        if viewname:
-            from custom_admin.utils.register_admin_viewsets import _ADMIN_VIEWS
-            view = _ADMIN_VIEWS[viewname]
-            serializer = view.get_serializer_class()()
-
-            field_slug = request.data.get('field_slug')
-            field = serializer.fields.get(field_slug)
-
-            if field:
-
-                if isinstance(field, serializers.ManyRelatedField):
-                    field = field.child_relation
-
-                filter_queryset = getattr(field, 'filter_queryset', None)
-                qs = getattr(field, 'queryset')
-
-                form_data = request.data.get('form_data')
-                if form_data is None:
-                    form_data = dict()
-
-                if filter_queryset:
-                    filtered_qs = filter_queryset(qs, form_data, request)
-                    log.debug(
-                        'AUTOCOMPLETE view:%s using:%s init form_data.keys:%s result:%s',
-                        viewname, filter_queryset.__name__, form_data.keys(), filtered_qs,
-                    )
-                    return filtered_qs
-
-                if qs and isinstance(qs, (QuerySet, Manager)):
-                    return qs.all()
-        return model.objects.all()
+        if form_data is None:
+            form_data = {}
+
+        if filter_queryset:
+            filtered_qs = filter_queryset(qs, form_data, self.request)
+            log.debug(
+                'AUTOCOMPLETE view:%s using:%s init form_data.keys:%s result:%s',
+                viewname, filter_queryset.__name__, form_data.keys(), filtered_qs,
+            )
+            return filtered_qs
+
+        if not isinstance(qs, (QuerySet, Manager)):
+            raise serializers.ValidationError(f'Model {self.app_label}.{self.model_name} view "{viewname}" autocomplete for {field_slug}')
+
+        return qs.all()
 
     @staticmethod
     def _get_str_value(obj):
-        if obj:
-            try:
-                return str(obj) or str(obj.id)
-            except TypeError as e:
-                log.error('Admin autocomplete: error get __str__ for %s', obj)
-                return str(obj.id)
-
-    def post(self, request, format=None):
-        search_string = request.data.get('search_string')
-        limit = request.data.get('limit')
+        if not obj:
+            return
 
         try:
-            model = self.get_model(request)
-        except ModelNotFound as e:
-            return Response(str(e))
+            return str(obj) or str(obj.id)
+        except TypeError as e:
+            log.error('Admin autocomplete: error get __str__ for %s', obj)
+            return str(obj.id)
+
+    def post(self, request, model_name, app_label, *args, **kwargs):
+        self.app_label = app_label
+        self.model_name = model_name
+
+        serializer = AutoCompeteSerializer(data=request.data)
+        serializer.is_valid(raise_exception=True)
+
+        search_string = serializer.validated_data.get('search_string')
+        limit = serializer.validated_data.get('limit')
+
+        model = apps.get_model(app_label=app_label, model_name=model_name)
+        if not model:
+            raise serializers.ValidationError(f'Model {self.app_label}.{self.model_name} not found')
+
+        view_queryset = self.get_queryset_by_view(
+            model,
+            viewname=serializer.validated_data.get('viewname'),
+            form_data=serializer.validated_data.get('form_data'),
+            field_slug=serializer.validated_data.get('field_slug'),
+        )
 
-        view_queryset = self.get_queryset_by_view(model, request)
         qs = view_queryset
         if search_string:
             filters = self.get_search_filter(model, search_string)
             if not filters:
                 return Response([])
             qs = qs.filter(filters).order_by('id').distinct('id')
 
-        # TODO: Зарефакторить этот костыль, исправлялось срочно
-        # bonuses/playerbonus/list, KAZ-259
-        if model.__name__ == 'BonusCurrency':
-            try:
-                qs = qs.distinct('currency__code')
-            except Exception as e:
-                log.error(str(e))
-
         if limit:
             qs = qs[:limit]
 
-        existed_choices = request.data.get('existed_choices', [])
+        existed_choices = serializer.validated_data.get('existed_choices', [])
         if existed_choices:
-            # Добавляет в результат уже выбранные варианты
 
-            existed_choices_ids = [i['id'] for i in existed_choices]
-
-            filter_ids = view_queryset.filter(id__in=existed_choices_ids)
+            # Добавляет в результат уже выбранные варианты
+            filter_ids = view_queryset.filter(id__in=existed_choices)
             if qs:
                 qs = qs.union(filter_ids)
             else:
                 qs = filter_ids
 
         formated_values = [
             {'id': obj.id, 'text': self._get_str_value(obj)}
```

### Comparing `django-customvueadmin-0.1.9/custom_admin/api/views/base_admin_viewset.py` & `django_customvueadmin-0.2.0/custom_admin/api/views/base_admin_viewset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,37 @@
 import asyncio as aio
 import logging
 import typing
 
 from asgiref.sync import sync_to_async
 from django.db.models.fields.related_descriptors import ForwardManyToOneDescriptor, ManyToManyDescriptor
-from django.http import QueryDict
 from django.utils.decorators import classonlymethod
 from django.utils.translation import gettext as _
-from django_filters import rest_framework
-from rest_framework import filters, mixins, viewsets
+from rest_framework import mixins, serializers, viewsets
 from rest_framework.pagination import PageNumberPagination
 from rest_framework.parsers import JSONParser, MultiPartParser
 
-from backend.utils.async_tools import AsyncMixin
 from custom_admin.api.actions import AdminActionMixIn, export_csv_action
-from custom_admin.api.filters.base_admin_filter import BaseAdminFilterSet
+from custom_admin.api.backends import CustomFilterBackend, CustomOrderingFilter, CustomSearchFilter
+from custom_admin.api.inline_relation import RelatedInline
 from custom_admin.api.inlines import ViewActionsInlineMixIn
 from custom_admin.api.permissions import AdminPermission
 from custom_admin.controllers.custom_metadata import CustomMetadata
+from custom_admin.utils.async_mixin import AsyncMixin
 
 log = logging.getLogger('admin')
 
 
-class CustomSearchFilter(filters.SearchFilter):
-    def get_search_terms(self, request):
-        search = super().get_search_terms(request)
-
-        if request.data and 'filter_info' in request.data:
-            search = request.data['filter_info'].get('search')
-            if search:
-                return [search]
-
-        return search
-
-
-class CustomOrderingFilter(filters.OrderingFilter):
-    def get_ordering(self, request, queryset, view):
-        ordering = super().get_ordering(request, queryset, view)
-
-        if request.data and 'filter_info' in request.data:
-            ordering = request.data['filter_info'].get('ordering')
-            if ordering:
-                return [ordering]
-
-        return ordering
-
-
-class CustomFilterBackend(rest_framework.DjangoFilterBackend):
-    filterset_base = BaseAdminFilterSet
-
-    def get_filterset_kwargs(self, request, queryset, view):
-        data = request.query_params
-
-        if request.data and 'filter_info' in request.data:
-            _filters = request.data['filter_info'].get('filters')
-            if _filters:
-                data = QueryDict('', mutable=True)
-                for k, v in _filters.items():
-                    data.setlist(k, v)
-
-        return {
-            'data': data,
-            'queryset': queryset,
-            'request': request,
-        }
-
-
 class AdminPaginator(PageNumberPagination):
     page_size = 25
     page_size_query_param = 'limit'
 
 
 class BaseAdminDataViewSet(ViewActionsInlineMixIn, viewsets.ViewSet):
-    icon: typing.Optional[str] = None  # https://element.eleme.io/#/en-US/component/icon
+    icon: typing.Optional[str] = None  # # https://pictogrammers.com/library/mdi/
     hide_in_navigation: typing.Optional[bool] = None
 
     throttle_classes = []
     parser_classes = (MultiPartParser, JSONParser)
     metadata_class = CustomMetadata
     permission_classes = (AdminPermission, )
 
@@ -183,15 +138,28 @@
     filterset_fields = []
 
     fixed_columns = ('id',)
 
     # Set None for diplay all fields
     filds_list = ['id']
 
-    related_inlines = []
+    related_inlines: typing.List[RelatedInline] = []
+
+    @classmethod
+    def get_related_inlines(cls) -> typing.List[dict]:
+        result = []
+        for i, inline in enumerate(cls.related_inlines):
+
+            if not isinstance(inline, RelatedInline):
+                raise serializers.ValidationError(f'View {cls.__name__}.related_inlines[{i}] error: is not an instance of RelatedInline')
+
+            inline.validate(cls, i)
+            result.append(inline.asdict())
+
+        return result
 
     @classmethod
     def get_model(cls) -> typing.Optional[typing.Any]:
         return cls.get_serializer_class().Meta.model
 
     def get_queryset(self):
         qs = super().get_queryset()
```

### Comparing `django-customvueadmin-0.1.9/custom_admin/api/views/get_sections.py` & `django_customvueadmin-0.2.0/custom_admin/api/views/get_sections.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 
 from django.conf import settings
+from django.utils import translation
 from rest_framework.response import Response
 from rest_framework.views import APIView
 
 from custom_admin.api.permissions import AdminPermission
 from custom_admin.utils import get_schema
 
 log = logging.getLogger("request")
@@ -15,13 +16,15 @@
     Get all scheme for admin frontend
     '''
     throttle_classes = []
     permission_classes = (AdminPermission, )
     router = None
 
     def get(self, request, *args, **kwargs):
+        lang = request.headers.get('Accept-Language') or getattr(settings, 'LANGUAGE_CODE', None) or 'en'
+        translation.activate(lang)
         response = Response({
             'sections': get_schema(self.router, request),
-            'language': request.LANGUAGE_CODE,
+            'language': lang,
             'languages': {lang[0]: lang[1] for lang in settings.LANGUAGES},
         })
         return response
```

### Comparing `django-customvueadmin-0.1.9/custom_admin/api/viewset_info.py` & `django_customvueadmin-0.2.0/custom_admin/api/viewset_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 @dataclass
 class AdminViewSetInfo:
     group_slug: str
     title: str
 
     views: typing.List[str]
 
-    # https://element.eleme.io/#/en-US/component/icon
+    # https://pictogrammers.com/library/mdi/
     icon: typing.Optional[str] = None
 
     def __post_init__(self):
         assert len(self.views) > 0, 'AdminViewSetInfo.views is empty'
 
     def iterate_views(self):
         from custom_admin.api.views import BaseAdminDataViewSet, BaseAdminViewSet
```

### Comparing `django-customvueadmin-0.1.9/custom_admin/controllers/admin_log_manager.py` & `django_customvueadmin-0.2.0/custom_admin/controllers/admin_log_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,11 +89,11 @@
             staff=self.staff,
             section=view.get_view_viewname(),
             action_type=AdminLogType.ACTION,
             content=request.data,
             title=short_description,
         )
         log.info(
-            'ADMIN %s #%s ACTION "%s" admin_log:%s request.data:%s short_description:%s',
-            self.staff.username, self.staff.id, action_name, admin_log.section, request.data, short_description,
+            'ADMIN %s #%s ACTION "%s" admin_log:%s short_description:%s',
+            self.staff.username, self.staff.id, action_name, admin_log.section, short_description,
         )
         return admin_log
```

### Comparing `django-customvueadmin-0.1.9/custom_admin/controllers/custom_metadata.py` & `django_customvueadmin-0.2.0/custom_admin/controllers/custom_metadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,33 +14,29 @@
         """
         Given an instance of a serializer field, return a dictionary
         of metadata about it.
         """
         field_info = OrderedDict()
         field_info['type'] = self.label_lookup[field]
         field_info['required'] = getattr(field, 'required', False)
+        field_info['help_text'] = False
+
         attrs = [
             'read_only', 'label', 'help_text',
             'min_length', 'max_length',
             'min_value', 'max_value', 'write_only', 'max_width', 'initial',
-            'wysiwyg', 'multilined',
+            'wysiwyg', 'multilined', 'tag_style', 'json_forms', 'list_preview',
         ]
 
         for attr in attrs:
             value = getattr(field, attr, None)
             if value is not None and value != '':
-                field_info[attr] = force_str(value, strings_only=True)
-
-        if isinstance(field.label, str):
-            field_info['label'] = field_info['label']
-        else:
-            field_info['label'] = _(field_info['label'])
-
-        if 'help_text' in field_info:
-            field_info['help_text'] = _(field_info['help_text'])
+                field_info[attr] = value
+                if not isinstance(value, (dict, list)):
+                    field_info[attr] = force_str(value, strings_only=True)
 
         if getattr(field, 'child', None):
             field_info['child'] = self.get_field_info(field.child)
         elif getattr(field, 'fields', None):
             field_info['children'] = self.get_serializer_info(field)
 
         is_inst = isinstance(field, (serializers.RelatedField, serializers.ManyRelatedField))
```

### Comparing `django-customvueadmin-0.1.9/custom_admin/controllers/filters_schema.py` & `django_customvueadmin-0.2.0/custom_admin/controllers/filters_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,24 +22,27 @@
         elif isinstance(f, (list, tuple)):
             filter_name = f[0]
             filter_field = f[1]
 
         result[filter_name] = {'type': filter_field.__class__.__name__}
 
         if result[filter_name]['type'] == 'ManyToManyRel':
-            result[filter_name]['name'] = str(_(filter_field.related_model._meta.verbose_name))
+            result[filter_name]['label'] = str(_(filter_field.related_model._meta.verbose_name))
         else:
-            result[filter_name]['name'] = str(_(filter_field.verbose_name))
+            result[filter_name]['label'] = str(_(filter_field.verbose_name))
 
         if result[filter_name]['type'] in ('ForeignKey', 'ManyToManyField', 'OneToOneField', 'ManyToManyRel'):
-            result[filter_name]['model'] = filter_field.related_model.__name__
+            result[filter_name]['model_name'] = filter_field.related_model.__name__
             result[filter_name]['app_label'] = filter_field.related_model._meta.app_label
 
         if hasattr(filter_field, 'choices') and filter_field.choices:
-            choices = tuple((c[0], str(_(c[1]))) for c in filter_field.choices)
+            choices = tuple({
+                'value': c[0],
+                'display_name': str(_(c[1]))
+            } for c in filter_field.choices)
             if choices:
                 result[filter_name]['choices'] = choices
 
     return result
 
 
 def get_filters_class_data(model, filter_class, request) -> dict:
@@ -50,32 +53,35 @@
         if not name:
             field = get_model_field(model, filter_field.field_name)
             if field:
                 name = _(field.verbose_name)
 
         result[filter_name] = {
             'type': filter_field.__class__.__name__,
-            'name': str(name),
+            'label': str(name),
         }
 
         filter_model = None
 
         if result[filter_name]['type'] in ('ModelChoiceFilter', 'OneToOneField', 'ModelMultipleChoiceFilter'):
             filter_model = filter_field.get_queryset(request).model
 
         elif result[filter_name]['type'] in ('ManyRelatedField', 'AdminManyRelatedField'):
             filter_model = filter_field.child_relation.queryset.model
 
         if filter_model:
             model_name = filter_model.__name__
             app_label = filter_model._meta.app_label
-            result[filter_name]['model'] = model_name
+            result[filter_name]['model_name'] = model_name
             result[filter_name]['app_label'] = app_label
 
         if isinstance(filter_field, filters.Filter):
             choices = filter_field.extra.get('choices')
             if choices:
-                choices = tuple((c[0], str(_(c[1]))) for c in choices)
+                choices = tuple({
+                    'value': c[0],
+                    'display_name': str(_(c[1]))
+                } for c in choices)
                 if choices:
                     result[filter_name]['choices'] = choices
 
     return result
```

### Comparing `django-customvueadmin-0.1.9/custom_admin/controllers/schema_generator.py` & `django_customvueadmin-0.2.0/custom_admin/controllers/schema_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import typing
 
 from django.conf import settings
 from django.utils.translation import gettext as _
 from django_filters.utils import get_model_field
-from modeltranslation.translator import NotRegistered, translator
 
+from custom_admin.api.action_functions import ACTION_ATTRIBUTES
 from custom_admin.api.serializers.base_serializer import AdminModelSerializer
 from custom_admin.api.viewset_info import AdminViewSetInfo
-from custom_admin.controllers.filters_schema import ModelFieldException, get_filters_class_data, get_filters_fields_data
+from custom_admin.controllers.filters_schema import (
+    ModelFieldException,
+    get_filters_class_data,
+    get_filters_fields_data,
+)
 
 
 class ViewSetSchemaGenerator:
     viewset = None
     router = None
     basename = None
     request = None
@@ -154,26 +158,30 @@
 
     def _get_actions_info(self, view_actions) -> dict:
         actions = {}
         for action in view_actions:
             name = getattr(action, 'short_description', action.__name__)
             actions[action.__name__] = {'name': name}
 
-            description = getattr(action, 'description', None)
-            if description:
-                actions[action.__name__]['description'] = description
+            for attr in ACTION_ATTRIBUTES:
+                actions[action.__name__][attr] = getattr(action, attr, None)
 
             form_serializer = getattr(action, 'form_serializer', None)
             if form_serializer:
                 meta = self.viewset.metadata_class()
                 serializer_info = meta.get_serializer_info(form_serializer())
                 actions[action.__name__]['form_serializer'] = serializer_info
         return actions
 
     def _get_translations_info(self, serializer):
+        try:
+            from modeltranslation.translator import NotRegistered, translator
+        except ModuleNotFoundError:
+            return {}
+
         if not self.model:
             return {}
 
         result = {}
         try:
             for field in translator.get_options_for_model(self.model).fields:
                 result[field] = []
@@ -201,19 +209,23 @@
 
         title = str(_(self.viewset.get_view_title()))
         filters_data = self._get_filters_data()
         serializer, serializer_info = self._get_serializer_info()
         list_display = self._get_list_display(serializer_info, serializer)
         search_fields = self._get_search_fields()
 
+        related_inlines = []
+        if hasattr(self.viewset, 'get_related_inlines'):
+            related_inlines = self.viewset.get_related_inlines()
+
         meta_data = {
             'serializer': serializer_info,
             'search_fields': search_fields,
             'ordering_fields': getattr(self.viewset, 'ordering_fields', []),
-            'related_inlines': getattr(self.viewset, 'related_inlines', []),
+            'related_inlines': related_inlines,
             'field_groups': getattr(serializer.Meta, 'groups', None) if serializer else None,
             'filterset_fields': filters_data,
             'filds_list': list_display,
             'fixed_columns': getattr(self.viewset, 'fixed_columns', []),
             'actions': self._get_actions_info(getattr(self.viewset, "actions", [])),
             'translations': self._get_translations_info(serializer),
         }
```

### Comparing `django-customvueadmin-0.1.9/custom_admin/models/admin_log.py` & `django_customvueadmin-0.2.0/custom_admin/models/admin_log.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.9/custom_admin/static/custom_admin/favicon.ico` & `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/dark-first/content.min.css` & `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/dark-first/content.min.css`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/dark-first/skin.min.css` & `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/dark-first/skin.min.css`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/dark-slim/content.min.css` & `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/dark-slim/content.min.css`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/dark-slim/skin.min.css` & `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/dark-slim/skin.min.css`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/img/example.png` & `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/img/example.png`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/img/tinymce.woff2` & `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/img/tinymce.woff2`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/lightgray/content.min.css` & `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/lightgray/content.min.css`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/lightgray/fonts/tinymce.woff` & `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/lightgray/fonts/tinymce.woff`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/lightgray/skin.min.css` & `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/lightgray/skin.min.css`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/plugins/accordion/plugin.js` & `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/plugins/accordion/plugin.js`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/prism.css` & `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/plugins/codesample/css/prism.css`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.9/custom_admin/static/custom_admin/tinymce/tinymce.min.js` & `django_customvueadmin-0.2.0/custom_admin/static/custom_admin/tinymce/tinymce.min.js`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.9/custom_admin/utils/colors.py` & `django_customvueadmin-0.2.0/custom_admin/utils/colors.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.9/custom_admin/utils/get_schema.py` & `django_customvueadmin-0.2.0/custom_admin/utils/get_schema.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.9/custom_admin/utils/register_admin_viewsets.py` & `django_customvueadmin-0.2.0/custom_admin/utils/register_admin_viewsets.py`

 * *Files identical despite different names*

### Comparing `django-customvueadmin-0.1.9/custom_admin/views/admin_page.py` & `django_customvueadmin-0.2.0/custom_admin/views/admin_page.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import json
 
-from django.conf import settings
+from django.conf import os, settings
 from django.shortcuts import render
 from django.template.exceptions import TemplateDoesNotExist
 from django.views import View
 
+from custom_admin.utils import get_schema
+
 TEMPLATE_NOT_FOUND = '''
 Custom admin cannot find template "{template}".
 Make sure settings.TEMPLATES contains 'APP_DIRS': True
 '''
 
 
 class CustomAdminView(View):
@@ -17,18 +19,25 @@
     USE_X_FORWARDED_HOST = True
     SECURE_PROXY_SSL_HEADER = ('HTTP_X_FORWARDED_PROTO', 'https')
     '''
 
     template = 'custom_admin/admin_index.html'
 
     def get(self, request):
+        custom_admin = getattr(settings, 'CUSTOM_ADMIN', {})
+
+        static_prefix = custom_admin.get('static_prefix') or '/static/custom_admin'
+
         admin_settings = {
-            'title': settings.CUSTOM_ADMIN.get('title'),
-            'base_admin_url': settings.CUSTOM_ADMIN.get('base_admin_url') or 'admin/',
-            'static_prefix': settings.CUSTOM_ADMIN.get('static_prefix') or '/static/custom_admin',
+            'title': custom_admin.get('title', 'Admin'),
+            'base_admin_url': custom_admin.get('base_admin_url') or 'admin/',
+            'static_prefix': static_prefix,
+            'favicon_path': custom_admin.get('favicon_path') or os.path.join(static_prefix, 'favicon.ico'),
+            'logo_image_path': custom_admin.get('logo_image_path') or os.path.join(static_prefix, 'default-logo.png'),
+            'auth_header_prefix': custom_admin.get('auth_header_prefix') or 'Token',
         }
 
         if not admin_settings.get('backend_prefix'):
             admin_settings['backend_prefix'] = request.build_absolute_uri('/custom_admin/')
 
         context = {
             'SETTINGS': admin_settings,
```

### Comparing `django-customvueadmin-0.1.9/django_customvueadmin.egg-info/PKG-INFO` & `django_customvueadmin-0.2.0/django_customvueadmin.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: django-customvueadmin
-Version: 0.1.9
-Summary: A custom admin interface providing backend via DRF and frontend via Vue and Element UI that tries Keep It Simple.
+Version: 0.2.0
+Summary: A custom admin interface providing backend via DRF and frontend via Vue and Element UI that tries to Keep It Simple.
 Home-page: https://innova-group-llc.github.io/custom_admin_docs/
 License: BSD-3-Clause
 Project-URL: Documentation, https://innova-group-llc.github.io/custom_admin_docs/
 Project-URL: Source, https://github.com/Innova-Group-LLC/custom_admin
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.10
-Provides-Extra: argon2
-Requires-Dist: argon2-cffi>=19.1.0; extra == "argon2"
-Provides-Extra: bcrypt
-Requires-Dist: bcrypt; extra == "bcrypt"
+Requires-Python: >=3.8
+License-File: LICENSE
 
 Django Custom Admin
 ===================
 
 |logo|
 
 A custom admin interface providing backend via DRF and frontend via Vue
-and Element UI that tries Keep It Simple.
+and Element UI that tries to Keep It Simple.
 
 |PyPI version| |GitHub stars|
 
 `Documentation <https://innova-group-llc.github.io/custom_admin_docs/>`__
 
 Features
 --------
@@ -60,18 +59,17 @@
 Build
 -----
 
 ::
 
    npm run build --prefix vue_frontend
    rm -r custom_admin/static/custom_admin/*
-   cp vue_frontend/dist/favicon.ico custom_admin/static/custom_admin/favicon.ico
-   cp vue_frontend/dist/manifest.json custom_admin/static/custom_admin/manifest.json
-   cp -r vue_frontend/dist/tinymce/ custom_admin/static/custom_admin/tinymce/
-   cp -r vue_frontend/dist/static/ custom_admin/
+   rm -r custom_admin/templates/custom_admin/admin_index.html
+   cp vue_frontend/dist/index.html custom_admin/templates/custom_admin/admin_index.html
+   cp -r vue_frontend/dist/custom_admin/ custom_admin/static/
 
 .. |logo| image:: https://github.com/Innova-Group-LLC/custom_admin/blob/master/logo.png?raw=true
    :target: https://innova-group-llc.github.io/custom_admin_docs/
 .. |PyPI version| image:: https://badge.fury.io/py/django-customvueadmin.svg
    :target: https://pypi.org/project/django-customvueadmin/
 .. |GitHub stars| image:: https://img.shields.io/github/stars/Innova-Group-LLC/custom_admin
    :target: https://github.com/Innova-Group-LLC/custom_admin
```

### Comparing `django-customvueadmin-0.1.9/django_customvueadmin.egg-info/SOURCES.txt` & `django_customvueadmin-0.2.0/django_customvueadmin.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,108 +1,98 @@
+LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
 custom_admin/__init__.py
 custom_admin/api/__init__.py
+custom_admin/api/action_functions.py
+custom_admin/api/backends.py
+custom_admin/api/inline_relation.py
 custom_admin/api/permissions.py
 custom_admin/api/urls.py
 custom_admin/api/viewset_info.py
 custom_admin/api/actions/__init__.py
 custom_admin/api/actions/delete_action.py
 custom_admin/api/actions/export_csv_action.py
 custom_admin/api/actions/view_actions_mixin.py
 custom_admin/api/fields/__init__.py
 custom_admin/api/fields/base.py
 custom_admin/api/fields/char.py
 custom_admin/api/fields/choice.py
 custom_admin/api/fields/files.py
 custom_admin/api/fields/int.py
+custom_admin/api/fields/json.py
 custom_admin/api/fields/numbers.py
 custom_admin/api/fields/relation.py
 custom_admin/api/filters/__init__.py
 custom_admin/api/filters/base_admin_filter.py
 custom_admin/api/filters/choices.py
+custom_admin/api/filters/date_range.py
 custom_admin/api/inlines/__init__.py
 custom_admin/api/inlines/export_csv_inline.py
 custom_admin/api/inlines/inline_graph.py
 custom_admin/api/inlines/inline_table.py
 custom_admin/api/inlines/inlines_type.py
 custom_admin/api/inlines/interfaces.py
 custom_admin/api/inlines/view_inline_mixin.py
 custom_admin/api/serializers/__init__.py
+custom_admin/api/serializers/auth_response.py
 custom_admin/api/serializers/base_serializer.py
+custom_admin/api/tests/__init__.py
+custom_admin/api/tests/test_filters.py
+custom_admin/api/tests/test_scheme_get.py
+custom_admin/api/tests/urls.py
 custom_admin/api/views/__init__.py
-custom_admin/api/views/admin_log.py
 custom_admin/api/views/autocomplete.py
 custom_admin/api/views/base_admin_viewset.py
-custom_admin/api/views/change_language.py
 custom_admin/api/views/get_sections.py
 custom_admin/api/views/token_auth.py
+custom_admin/api/views/defaults/__init__.py
+custom_admin/api/views/defaults/admin_log.py
+custom_admin/api/views/defaults/groups.py
+custom_admin/api/views/defaults/permissions.py
 custom_admin/controllers/__init__.py
 custom_admin/controllers/admin_log_manager.py
 custom_admin/controllers/custom_metadata.py
 custom_admin/controllers/filters_schema.py
 custom_admin/controllers/schema_generator.py
+custom_admin/management/__init__.py
+custom_admin/management/commands/__init__.py
+custom_admin/management/commands/custom_admin_viewsets_list.py
 custom_admin/migrations/0001_initial.py
-custom_admin/migrations/0002_auto_20220826_1734.py
-custom_admin/migrations/0003_remove_adminlog_hall_alter_adminlog_staff.py
 custom_admin/migrations/__init__.py
 custom_admin/models/__init__.py
 custom_admin/models/admin_log.py
 custom_admin/static/custom_admin/favicon.ico
-custom_admin/static/custom_admin/css/app.css
-custom_admin/static/custom_admin/css/chunk-3ef8a5a8.css
-custom_admin/static/custom_admin/css/chunk-7402f562.css
-custom_admin/static/custom_admin/css/chunk-8b69702c.css
-custom_admin/static/custom_admin/css/chunk-a7c7287a.css
-custom_admin/static/custom_admin/css/chunk-ecedfa6a.css
-custom_admin/static/custom_admin/css/chunk-elementUI.css
-custom_admin/static/custom_admin/css/chunk-fdcfea10.css
-custom_admin/static/custom_admin/css/chunk-libs.css
-custom_admin/static/custom_admin/fonts/element-icons.ttf
-custom_admin/static/custom_admin/fonts/element-icons.woff
-custom_admin/static/custom_admin/img/404.png
-custom_admin/static/custom_admin/img/404_cloud.png
-custom_admin/static/custom_admin/js/app.js
-custom_admin/static/custom_admin/js/chunk-2d0c14f9.js
-custom_admin/static/custom_admin/js/chunk-2d2080da.js
-custom_admin/static/custom_admin/js/chunk-3ef8a5a8.js
-custom_admin/static/custom_admin/js/chunk-5148deb9.js
-custom_admin/static/custom_admin/js/chunk-6786f71b.js
-custom_admin/static/custom_admin/js/chunk-7402f562.js
-custom_admin/static/custom_admin/js/chunk-8b69702c.js
-custom_admin/static/custom_admin/js/chunk-a7c7287a.js
-custom_admin/static/custom_admin/js/chunk-ecedfa6a.js
-custom_admin/static/custom_admin/js/chunk-elementUI.js
-custom_admin/static/custom_admin/js/chunk-fdcfea10.js
-custom_admin/static/custom_admin/js/chunk-libs.js
-custom_admin/static/custom_admin/js/runtime.js
+custom_admin/static/custom_admin/index-C4Cutzkc.css
+custom_admin/static/custom_admin/index-OjzvLInB.js
+custom_admin/static/custom_admin/materialdesignicons-webfont-CYDMK1kx.woff2
+custom_admin/static/custom_admin/materialdesignicons-webfont-CgCzGbLl.woff
+custom_admin/static/custom_admin/materialdesignicons-webfont-D3kAzl71.ttf
+custom_admin/static/custom_admin/materialdesignicons-webfont-DttUABo4.eot
 custom_admin/static/custom_admin/tinymce/tinymce.min.js
 custom_admin/static/custom_admin/tinymce/dark-first/content.min.css
 custom_admin/static/custom_admin/tinymce/dark-first/skin.min.css
 custom_admin/static/custom_admin/tinymce/dark-slim/content.min.css
 custom_admin/static/custom_admin/tinymce/dark-slim/skin.min.css
 custom_admin/static/custom_admin/tinymce/img/example.png
 custom_admin/static/custom_admin/tinymce/img/tinymce.woff2
 custom_admin/static/custom_admin/tinymce/lightgray/content.min.css
 custom_admin/static/custom_admin/tinymce/lightgray/skin.min.css
 custom_admin/static/custom_admin/tinymce/lightgray/fonts/tinymce.woff
 custom_admin/static/custom_admin/tinymce/plugins/accordion/plugin.js
 custom_admin/static/custom_admin/tinymce/plugins/accordion/css/accordion.css
 custom_admin/static/custom_admin/tinymce/plugins/codesample/css/prism.css
 custom_admin/templates/custom_admin/admin_index.html
-custom_admin/tests/__init__.py
-custom_admin/tests/test_language.py
-custom_admin/tests/test_scheme_get.py
 custom_admin/utils/__init__.py
+custom_admin/utils/async_mixin.py
 custom_admin/utils/colors.py
 custom_admin/utils/get_schema.py
 custom_admin/utils/register_admin_viewsets.py
 custom_admin/views/__init__.py
 custom_admin/views/admin_page.py
 django_customvueadmin.egg-info/PKG-INFO
 django_customvueadmin.egg-info/SOURCES.txt
 django_customvueadmin.egg-info/dependency_links.txt
 django_customvueadmin.egg-info/not-zip-safe
-django_customvueadmin.egg-info/requires.txt
 django_customvueadmin.egg-info/top_level.txt
```

